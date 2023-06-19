# Comparing `tmp/nwon_baseline-0.1.33.tar.gz` & `tmp/nwon_baseline-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nwon_baseline-0.1.33.tar", max compression
+gzip compressed data, was "nwon_baseline-0.2.1.tar", max compression
```

## Comparing `nwon_baseline-0.1.33.tar` & `nwon_baseline-0.2.1.tar`

### file list

```diff
@@ -1,743 +1,742 @@
--rw-r--r--   0        0        0    15100 2022-04-05 08:26:32.639168 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/attr/__init__.pyi
--rw-r--r--   0        0        0      317 2022-04-05 08:26:32.651168 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/attr/_cmp.pyi
--rw-r--r--   0        0        0      209 2022-04-05 08:26:32.659168 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/attr/_version_info.pyi
--rw-r--r--   0        0        0      416 2022-04-05 08:26:32.663168 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/attr/converters.pyi
--rw-r--r--   0        0        0      539 2022-04-05 08:26:32.671168 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/attr/exceptions.pyi
--rw-r--r--   0        0        0      215 2022-04-05 08:26:32.671168 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/attr/filters.pyi
--rw-r--r--   0        0        0      573 2022-04-05 08:26:32.671168 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/attr/setters.pyi
--rw-r--r--   0        0        0     2268 2022-04-05 08:26:32.671168 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/attr/validators.pyi
--rw-r--r--   0        0        0     1982 2022-04-05 08:26:32.671168 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/attrs/__init__.pyi
--rw-r--r--   0        0        0      572 2022-04-05 08:26:34.267165 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/humps/main.pyi
--rw-r--r--   0        0        0     1205 2022-04-05 08:26:32.211169 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/iniconfig/__init__.pyi
--rw-r--r--   0        0        0     1747 2022-04-05 08:26:35.351163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/BaseHTTPServer.pyi
--rw-r--r--   0        0        0      187 2022-04-05 08:26:35.359163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/CGIHTTPServer.pyi
--rw-r--r--   0        0        0     3869 2022-04-05 08:26:35.355163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ConfigParser.pyi
--rw-r--r--   0        0        0     1342 2022-04-05 08:26:35.339163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/Cookie.pyi
--rw-r--r--   0        0        0     1064 2022-04-05 08:26:35.347163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/HTMLParser.pyi
--rw-r--r--   0        0        0      895 2022-04-05 08:26:35.359163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/Queue.pyi
--rw-r--r--   0        0        0      648 2022-04-05 08:26:35.339163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/SimpleHTTPServer.pyi
--rw-r--r--   0        0        0     4559 2022-04-05 08:26:35.351163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/SocketServer.pyi
--rw-r--r--   0        0        0     1146 2022-04-05 08:26:35.351163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/StringIO.pyi
--rw-r--r--   0        0        0     1663 2022-04-05 08:26:35.355163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/UserDict.pyi
--rw-r--r--   0        0        0      630 2022-04-05 08:26:35.339163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/UserList.pyi
--rw-r--r--   0        0        0     3934 2022-04-05 08:26:35.355163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/UserString.pyi
--rw-r--r--   0        0        0    48689 2022-04-05 08:26:35.359163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/__builtin__.pyi
--rw-r--r--   0        0        0     5726 2022-04-05 08:26:35.359163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_ast.pyi
--rw-r--r--   0        0        0     1430 2022-04-05 08:26:35.351163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_collections.pyi
--rw-r--r--   0        0        0      577 2022-04-05 08:26:35.355163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_functools.pyi
--rw-r--r--   0        0        0      635 2022-04-05 08:26:35.339163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_hotshot.pyi
--rw-r--r--   0        0        0     7016 2022-04-05 08:26:35.343163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_io.pyi
--rw-r--r--   0        0        0      226 2022-04-05 08:26:35.351163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_json.pyi
--rw-r--r--   0        0        0      300 2022-04-05 08:26:35.351163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_md5.pyi
--rw-r--r--   0        0        0      348 2022-04-05 08:26:35.339163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_sha.pyi
--rw-r--r--   0        0        0      632 2022-04-05 08:26:35.343163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_sha256.pyi
--rw-r--r--   0        0        0      632 2022-04-05 08:26:35.339163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_sha512.pyi
--rw-r--r--   0        0        0     6286 2022-04-05 08:26:35.339163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_socket.pyi
--rw-r--r--   0        0        0     1934 2022-04-05 08:26:35.351163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_sre.pyi
--rw-r--r--   0        0        0      767 2022-04-05 08:26:35.359163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_struct.pyi
--rw-r--r--   0        0        0      677 2022-04-05 08:26:35.351163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_symtable.pyi
--rw-r--r--   0        0        0      319 2022-04-05 08:26:35.355163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_threading_local.pyi
--rw-r--r--   0        0        0     3696 2022-04-05 08:26:35.351163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_winreg.pyi
--rw-r--r--   0        0        0     1147 2022-04-05 08:26:35.347163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/abc.pyi
--rw-r--r--   0        0        0     1199 2022-04-05 08:26:35.339163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ast.pyi
--rw-r--r--   0        0        0      117 2022-04-05 08:26:35.347163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/atexit.pyi
--rw-r--r--   0        0        0    48689 2022-04-05 08:26:35.339163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/builtins.pyi
--rw-r--r--   0        0        0      795 2022-04-05 08:26:35.339163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cPickle.pyi
--rw-r--r--   0        0        0     1870 2022-04-05 08:26:35.351163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cStringIO.pyi
--rw-r--r--   0        0        0     4050 2022-04-05 08:26:35.339163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cgi.pyi
--rw-r--r--   0        0        0     4913 2022-04-05 08:26:35.351163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/collections.pyi
--rw-r--r--   0        0        0      329 2022-04-05 08:26:35.339163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/commands.pyi
--rw-r--r--   0        0        0      628 2022-04-05 08:26:35.351163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/compileall.pyi
--rw-r--r--   0        0        0     4716 2022-04-05 08:26:35.351163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cookielib.pyi
--rw-r--r--   0        0        0      750 2022-04-05 08:26:35.359163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/copy_reg.pyi
--rw-r--r--   0        0        0      273 2022-04-05 08:26:35.355163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/dircache.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.367163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/__init__.pyi
--rw-r--r--   0        0        0      447 2022-04-05 08:26:35.363163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/archive_util.pyi
--rw-r--r--   0        0        0       78 2022-04-05 08:26:35.367163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/bcppcompiler.pyi
--rw-r--r--   0        0        0     6449 2022-04-05 08:26:35.367163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/ccompiler.pyi
--rw-r--r--   0        0        0     2817 2022-04-05 08:26:35.367163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/cmd.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/__init__.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.375163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/bdist.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/bdist_dumb.pyi
--rw-r--r--   0        0        0      182 2022-04-05 08:26:35.371163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/bdist_msi.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/bdist_packager.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/bdist_rpm.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/bdist_wininst.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/build.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/build_clib.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/build_ext.pyi
--rw-r--r--   0        0        0      181 2022-04-05 08:26:35.371163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/build_py.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/build_scripts.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.375163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/check.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/clean.pyi
--rw-r--r--   0        0        0     3059 2022-04-05 08:26:35.375163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/config.pyi
--rw-r--r--   0        0        0      338 2022-04-05 08:26:35.375163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/install.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/install_data.pyi
--rw-r--r--   0        0        0      380 2022-04-05 08:26:35.371163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/install_egg_info.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/install_headers.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/install_lib.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/install_scripts.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/register.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/sdist.pyi
--rw-r--r--   0        0        0      296 2022-04-05 08:26:35.371163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/upload.pyi
--rw-r--r--   0        0        0      523 2022-04-05 08:26:35.371163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/config.pyi
--rw-r--r--   0        0        0     1688 2022-04-05 08:26:35.367163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/core.pyi
--rw-r--r--   0        0        0      138 2022-04-05 08:26:35.367163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/cygwinccompiler.pyi
--rw-r--r--   0        0        0       12 2022-04-05 08:26:35.363163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/debug.pyi
--rw-r--r--   0        0        0      252 2022-04-05 08:26:35.363163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/dep_util.pyi
--rw-r--r--   0        0        0      555 2022-04-05 08:26:35.367163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/dir_util.pyi
--rw-r--r--   0        0        0      508 2022-04-05 08:26:35.367163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/dist.pyi
--rw-r--r--   0        0        0       90 2022-04-05 08:26:35.367163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/emxccompiler.pyi
--rw-r--r--   0        0        0      852 2022-04-05 08:26:35.367163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/errors.pyi
--rw-r--r--   0        0        0      706 2022-04-05 08:26:35.367163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/extension.pyi
--rw-r--r--   0        0        0      859 2022-04-05 08:26:35.363163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/fancy_getopt.pyi
--rw-r--r--   0        0        0      439 2022-04-05 08:26:35.367163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/file_util.pyi
--rw-r--r--   0        0        0       20 2022-04-05 08:26:35.367163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/filelist.pyi
--rw-r--r--   0        0        0      863 2022-04-05 08:26:35.371163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/log.pyi
--rw-r--r--   0        0        0       78 2022-04-05 08:26:35.367163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/msvccompiler.pyi
--rw-r--r--   0        0        0      227 2022-04-05 08:26:35.367163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/spawn.pyi
--rw-r--r--   0        0        0      620 2022-04-05 08:26:35.367163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/sysconfig.pyi
--rw-r--r--   0        0        0      716 2022-04-05 08:26:35.367163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/text_file.pyi
--rw-r--r--   0        0        0       79 2022-04-05 08:26:35.367163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/unixccompiler.pyi
--rw-r--r--   0        0        0      829 2022-04-05 08:26:35.367163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/util.pyi
--rw-r--r--   0        0        0     1160 2022-04-05 08:26:35.367163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/version.pyi
--rw-r--r--   0        0        0      794 2022-04-05 08:26:35.355163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/dummy_thread.pyi
--rw-r--r--   0        0        0      159 2022-04-05 08:26:35.363163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/MIMEText.pyi
--rw-r--r--   0        0        0      270 2022-04-05 08:26:35.363163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/__init__.pyi
--rw-r--r--   0        0        0     1072 2022-04-05 08:26:35.363163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/_parseaddr.pyi
--rw-r--r--   0        0        0      303 2022-04-05 08:26:35.363163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/base64mime.pyi
--rw-r--r--   0        0        0      902 2022-04-05 08:26:35.363163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/charset.pyi
--rw-r--r--   0        0        0      143 2022-04-05 08:26:35.359163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/encoders.pyi
--rw-r--r--   0        0        0      536 2022-04-05 08:26:35.363163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/feedparser.pyi
--rw-r--r--   0        0        0      377 2022-04-05 08:26:35.359163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/generator.pyi
--rw-r--r--   0        0        0      457 2022-04-05 08:26:35.359163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/header.pyi
--rw-r--r--   0        0        0      256 2022-04-05 08:26:35.363163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/iterators.pyi
--rw-r--r--   0        0        0     1950 2022-04-05 08:26:35.363163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/message.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.363163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/__init__.pyi
--rw-r--r--   0        0        0      371 2022-04-05 08:26:35.363163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/application.pyi
--rw-r--r--   0        0        0      176 2022-04-05 08:26:35.363163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/audio.pyi
--rw-r--r--   0        0        0      128 2022-04-05 08:26:35.363163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/base.pyi
--rw-r--r--   0        0        0      176 2022-04-05 08:26:35.363163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/image.pyi
--rw-r--r--   0        0        0      147 2022-04-05 08:26:35.363163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/message.pyi
--rw-r--r--   0        0        0      159 2022-04-05 08:26:35.363163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/multipart.pyi
--rw-r--r--   0        0        0      107 2022-04-05 08:26:35.363163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/nonmultipart.pyi
--rw-r--r--   0        0        0      159 2022-04-05 08:26:35.363163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/text.pyi
--rw-r--r--   0        0        0      415 2022-04-05 08:26:35.363163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/parser.pyi
--rw-r--r--   0        0        0      490 2022-04-05 08:26:35.359163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/quoprimime.pyi
--rw-r--r--   0        0        0      760 2022-04-05 08:26:35.359163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/utils.pyi
--rw-r--r--   0        0        0      184 2022-04-05 08:26:35.375163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/encodings/__init__.pyi
--rw-r--r--   0        0        0      573 2022-04-05 08:26:35.375163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/encodings/utf_8.pyi
--rw-r--r--   0        0        0     1756 2022-04-05 08:26:35.343163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/exceptions.pyi
--rw-r--r--   0        0        0     1580 2022-04-05 08:26:35.359163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/fcntl.pyi
--rw-r--r--   0        0        0      348 2022-04-05 08:26:35.343163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/fnmatch.pyi
--rw-r--r--   0        0        0     1181 2022-04-05 08:26:35.347163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/functools.pyi
--rw-r--r--   0        0        0      194 2022-04-05 08:26:35.355163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/future_builtins.pyi
--rw-r--r--   0        0        0      752 2022-04-05 08:26:35.343163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/gc.pyi
--rw-r--r--   0        0        0      448 2022-04-05 08:26:35.351163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/getopt.pyi
--rw-r--r--   0        0        0      160 2022-04-05 08:26:35.343163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/getpass.pyi
--rw-r--r--   0        0        0     2285 2022-04-05 08:26:35.343163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/gettext.pyi
--rw-r--r--   0        0        0      375 2022-04-05 08:26:35.347163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/glob.pyi
--rw-r--r--   0        0        0      997 2022-04-05 08:26:35.347163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/gzip.pyi
--rw-r--r--   0        0        0      971 2022-04-05 08:26:35.355163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/hashlib.pyi
--rw-r--r--   0        0        0      756 2022-04-05 08:26:35.343163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/heapq.pyi
--rw-r--r--   0        0        0      114 2022-04-05 08:26:35.343163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/htmlentitydefs.pyi
--rw-r--r--   0        0        0     5929 2022-04-05 08:26:35.339163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/httplib.pyi
--rw-r--r--   0        0        0     1290 2022-04-05 08:26:35.343163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/imp.pyi
--rw-r--r--   0        0        0      134 2022-04-05 08:26:35.343163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/importlib.pyi
--rw-r--r--   0        0        0     4692 2022-04-05 08:26:35.359163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/inspect.pyi
--rw-r--r--   0        0        0     1136 2022-04-05 08:26:35.355163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/io.pyi
--rw-r--r--   0        0        0     5976 2022-04-05 08:26:35.355163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/itertools.pyi
--rw-r--r--   0        0        0     3206 2022-04-05 08:26:35.347163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/json.pyi
--rw-r--r--   0        0        0     9541 2022-04-05 08:26:35.375163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/logging/__init__.pyi
--rw-r--r--   0        0        0      458 2022-04-05 08:26:35.375163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/logging/config.pyi
--rw-r--r--   0        0        0     4237 2022-04-05 08:26:35.375163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/logging/handlers.pyi
--rw-r--r--   0        0        0      264 2022-04-05 08:26:35.339163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/markupbase.pyi
--rw-r--r--   0        0        0       74 2022-04-05 08:26:35.347163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/md5.pyi
--rw-r--r--   0        0        0      703 2022-04-05 08:26:35.351163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/mimetools.pyi
--rw-r--r--   0        0        0     1921 2022-04-05 08:26:35.375163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/__init__.pyi
--rw-r--r--   0        0        0     1392 2022-04-05 08:26:35.375163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/dummy/__init__.pyi
--rw-r--r--   0        0        0      673 2022-04-05 08:26:35.375163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/dummy/connection.pyi
--rw-r--r--   0        0        0     2038 2022-04-05 08:26:35.375163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/pool.pyi
--rw-r--r--   0        0        0      906 2022-04-05 08:26:35.375163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/process.pyi
--rw-r--r--   0        0        0      758 2022-04-05 08:26:35.375163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/util.pyi
--rw-r--r--   0        0        0      339 2022-04-05 08:26:35.355163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/mutex.pyi
--rw-r--r--   0        0        0     2937 2022-04-05 08:26:35.343163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ntpath.pyi
--rw-r--r--   0        0        0      115 2022-04-05 08:26:35.347163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/nturl2path.pyi
--rw-r--r--   0        0        0    13260 2022-04-05 08:26:35.359163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/os/__init__.pyi
--rw-r--r--   0        0        0     2935 2022-04-05 08:26:35.359163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/os/path.pyi
--rw-r--r--   0        0        0     2937 2022-04-05 08:26:35.351163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/os2emxpath.pyi
--rw-r--r--   0        0        0      467 2022-04-05 08:26:35.343163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pipes.pyi
--rw-r--r--   0        0        0     1809 2022-04-05 08:26:35.339163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/platform.pyi
--rw-r--r--   0        0        0      999 2022-04-05 08:26:35.355163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/popen2.pyi
--rw-r--r--   0        0        0     6396 2022-04-05 08:26:35.355163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/posix.pyi
--rw-r--r--   0        0        0     2937 2022-04-05 08:26:35.343163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/posixpath.pyi
--rw-r--r--   0        0        0     3156 2022-04-05 08:26:35.351163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/random.pyi
--rw-r--r--   0        0        0     3641 2022-04-05 08:26:35.355163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/re.pyi
--rw-r--r--   0        0        0     1095 2022-04-05 08:26:35.343163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/repr.pyi
--rw-r--r--   0        0        0      877 2022-04-05 08:26:35.347163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/resource.pyi
--rw-r--r--   0        0        0     2163 2022-04-05 08:26:35.347163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/rfc822.pyi
--rw-r--r--   0        0        0      230 2022-04-05 08:26:35.355163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/robotparser.pyi
--rw-r--r--   0        0        0      541 2022-04-05 08:26:35.355163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/runpy.pyi
--rw-r--r--   0        0        0     2975 2022-04-05 08:26:35.359163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sets.pyi
--rw-r--r--   0        0        0      236 2022-04-05 08:26:35.347163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sha.pyi
--rw-r--r--   0        0        0     1612 2022-04-05 08:26:35.359163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/shelve.pyi
--rw-r--r--   0        0        0     1025 2022-04-05 08:26:35.347163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/shlex.pyi
--rw-r--r--   0        0        0     1571 2022-04-05 08:26:35.343163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/signal.pyi
--rw-r--r--   0        0        0     2542 2022-04-05 08:26:35.355163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/smtplib.pyi
--rw-r--r--   0        0        0      308 2022-04-05 08:26:35.351163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/spwd.pyi
--rw-r--r--   0        0        0     1744 2022-04-05 08:26:35.347163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sre_constants.pyi
--rw-r--r--   0        0        0     2311 2022-04-05 08:26:35.339163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sre_parse.pyi
--rw-r--r--   0        0        0      992 2022-04-05 08:26:35.343163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/stat.pyi
--rw-r--r--   0        0        0     3567 2022-04-05 08:26:35.339163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/string.pyi
--rw-r--r--   0        0        0     2010 2022-04-05 08:26:35.347163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/stringold.pyi
--rw-r--r--   0        0        0     1157 2022-04-05 08:26:35.339163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/strop.pyi
--rw-r--r--   0        0        0     3282 2022-04-05 08:26:35.355163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/subprocess.pyi
--rw-r--r--   0        0        0     1341 2022-04-05 08:26:35.339163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/symbol.pyi
--rw-r--r--   0        0        0     3616 2022-04-05 08:26:35.359163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sys.pyi
--rw-r--r--   0        0        0     3696 2022-04-05 08:26:35.347163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/tempfile.pyi
--rw-r--r--   0        0        0     1854 2022-04-05 08:26:35.347163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/textwrap.pyi
--rw-r--r--   0        0        0      920 2022-04-05 08:26:35.339163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/thread.pyi
--rw-r--r--   0        0        0      243 2022-04-05 08:26:35.347163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/toaiff.pyi
--rw-r--r--   0        0        0     2686 2022-04-05 08:26:35.339163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/tokenize.pyi
--rw-r--r--   0        0        0     5465 2022-04-05 08:26:35.339163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/types.pyi
--rw-r--r--   0        0        0    17748 2022-04-05 08:26:35.347163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/typing.pyi
--rw-r--r--   0        0        0    12726 2022-04-05 08:26:35.351163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/unittest.pyi
--rw-r--r--   0        0        0     4765 2022-04-05 08:26:35.359163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/urllib.pyi
--rw-r--r--   0        0        0     8409 2022-04-05 08:26:35.355163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/urllib2.pyi
--rw-r--r--   0        0        0     1944 2022-04-05 08:26:35.343163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/urlparse.pyi
--rw-r--r--   0        0        0       83 2022-04-05 08:26:35.343163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/user.pyi
--rw-r--r--   0        0        0       85 2022-04-05 08:26:35.347163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/whichdb.pyi
--rw-r--r--   0        0        0     9769 2022-04-05 08:26:35.339163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xmlrpclib.pyi
--rw-r--r--   0        0        0      716 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/__future__.pyi
--rw-r--r--   0        0        0       63 2022-04-05 08:26:35.319163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/__main__.pyi
--rw-r--r--   0        0        0     8975 2022-04-05 08:26:35.335163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_ast.pyi
--rw-r--r--   0        0        0     1358 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_bisect.pyi
--rw-r--r--   0        0        0       63 2022-04-05 08:26:35.319163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_bootlocale.pyi
--rw-r--r--   0        0        0     5309 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_codecs.pyi
--rw-r--r--   0        0        0     1210 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_collections_abc.pyi
--rw-r--r--   0        0        0      388 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_compat_pickle.pyi
--rw-r--r--   0        0        0      915 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_compression.pyi
--rw-r--r--   0        0        0     1574 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_csv.pyi
--rw-r--r--   0        0        0    14505 2022-04-05 08:26:35.335163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_curses.pyi
--rw-r--r--   0        0        0       22 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_decimal.pyi
--rw-r--r--   0        0        0      800 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_dummy_thread.pyi
--rw-r--r--   0        0        0     6460 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_dummy_threading.pyi
--rw-r--r--   0        0        0      613 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_heapq.pyi
--rw-r--r--   0        0        0      705 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_imp.pyi
--rw-r--r--   0        0        0     1124 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_json.pyi
--rw-r--r--   0        0        0      256 2022-04-05 08:26:35.335163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_markupbase.pyi
--rw-r--r--   0        0        0     2168 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_msi.pyi
--rw-r--r--   0        0        0     1310 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_operator.pyi
--rw-r--r--   0        0        0     1796 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_osx_support.pyi
--rw-r--r--   0        0        0      557 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_posixsubprocess.pyi
--rw-r--r--   0        0        0      376 2022-04-05 08:26:35.335163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_py_abc.pyi
--rw-r--r--   0        0        0      157 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_pydecimal.pyi
--rw-r--r--   0        0        0      478 2022-04-05 08:26:35.303163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_random.pyi
--rw-r--r--   0        0        0      534 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_sitebuiltins.pyi
--rw-r--r--   0        0        0     1179 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_stat.pyi
--rw-r--r--   0        0        0     1451 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_thread.pyi
--rw-r--r--   0        0        0      490 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_threading_local.pyi
--rw-r--r--   0        0        0     2709 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_tkinter.pyi
--rw-r--r--   0        0        0      563 2022-04-05 08:26:35.319163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_tracemalloc.pyi
--rw-r--r--   0        0        0     4926 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_typeshed/__init__.pyi
--rw-r--r--   0        0        0      249 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_typeshed/tkinter.pyi
--rw-r--r--   0        0        0     1293 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_typeshed/wsgi.pyi
--rw-r--r--   0        0        0      528 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_typeshed/xml.pyi
--rw-r--r--   0        0        0     2233 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_warnings.pyi
--rw-r--r--   0        0        0     1226 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_weakref.pyi
--rw-r--r--   0        0        0     2410 2022-04-05 08:26:35.339163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_weakrefset.pyi
--rw-r--r--   0        0        0     4507 2022-04-05 08:26:35.335163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_winapi.pyi
--rw-r--r--   0        0        0      596 2022-04-05 08:26:35.319163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/abc.pyi
--rw-r--r--   0        0        0     3393 2022-04-05 08:26:35.319163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/aifc.pyi
--rw-r--r--   0        0        0      123 2022-04-05 08:26:35.319163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/antigravity.pyi
--rw-r--r--   0        0        0    18345 2022-04-05 08:26:35.335163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/argparse.pyi
--rw-r--r--   0        0        0     3623 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/array.pyi
--rw-r--r--   0        0        0     9090 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ast.pyi
--rw-r--r--   0        0        0     1555 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asynchat.pyi
--rw-r--r--   0        0        0     4242 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/__init__.pyi
--rw-r--r--   0        0        0    14883 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/base_events.pyi
--rw-r--r--   0        0        0      733 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/base_futures.pyi
--rw-r--r--   0        0        0     3239 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/base_subprocess.pyi
--rw-r--r--   0        0        0      412 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/base_tasks.pyi
--rw-r--r--   0        0        0      180 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/compat.pyi
--rw-r--r--   0        0        0      327 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/constants.pyi
--rw-r--r--   0        0        0      226 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/coroutines.pyi
--rw-r--r--   0        0        0    19207 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/events.pyi
--rw-r--r--   0        0        0      562 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/exceptions.pyi
--rw-r--r--   0        0        0      931 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/format_helpers.pyi
--rw-r--r--   0        0        0     2581 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/futures.pyi
--rw-r--r--   0        0        0     2806 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/locks.pyi
--rw-r--r--   0        0        0       39 2022-04-05 08:26:35.403163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/log.pyi
--rw-r--r--   0        0        0     3178 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/proactor_events.pyi
--rw-r--r--   0        0        0     1072 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/protocols.pyi
--rw-r--r--   0        0        0     1166 2022-04-05 08:26:35.403163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/queues.pyi
--rw-r--r--   0        0        0      314 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/runners.pyi
--rw-r--r--   0        0        0      215 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/selector_events.pyi
--rw-r--r--   0        0        0     5420 2022-04-05 08:26:35.403163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/sslproto.pyi
--rw-r--r--   0        0        0      396 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/staggered.pyi
--rw-r--r--   0        0        0     4021 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/streams.pyi
--rw-r--r--   0        0        0     6000 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/subprocess.pyi
--rw-r--r--   0        0        0    12113 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/tasks.pyi
--rw-r--r--   0        0        0      194 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/threads.pyi
--rw-r--r--   0        0        0     1886 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/transports.pyi
--rw-r--r--   0        0        0     4592 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/trsock.pyi
--rw-r--r--   0        0        0     2548 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/unix_events.pyi
--rw-r--r--   0        0        0     3554 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/windows_events.pyi
--rw-r--r--   0        0        0      983 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/windows_utils.pyi
--rw-r--r--   0        0        0     5534 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncore.pyi
--rw-r--r--   0        0        0      271 2022-04-05 08:26:35.319163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/atexit.pyi
--rw-r--r--   0        0        0     2119 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/audioop.pyi
--rw-r--r--   0        0        0     1772 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/base64.pyi
--rw-r--r--   0        0        0     4644 2022-04-05 08:26:35.303163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/bdb.pyi
--rw-r--r--   0        0        0     1555 2022-04-05 08:26:35.335163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/binascii.pyi
--rw-r--r--   0        0        0     1147 2022-04-05 08:26:35.303163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/binhex.pyi
--rw-r--r--   0        0        0       67 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/bisect.pyi
--rw-r--r--   0        0        0    57130 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/builtins.pyi
--rw-r--r--   0        0        0     2836 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/bz2.pyi
--rw-r--r--   0        0        0     1481 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/cProfile.pyi
--rw-r--r--   0        0        0     5796 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/calendar.pyi
--rw-r--r--   0        0        0     3746 2022-04-05 08:26:35.303163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/cgi.pyi
--rw-r--r--   0        0        0     1447 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/cgitb.pyi
--rw-r--r--   0        0        0      613 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/chunk.pyi
--rw-r--r--   0        0        0     1226 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/cmath.pyi
--rw-r--r--   0        0        0     1658 2022-04-05 08:26:35.319163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/cmd.pyi
--rw-r--r--   0        0        0     1522 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/code.pyi
--rw-r--r--   0        0        0    12435 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/codecs.pyi
--rw-r--r--   0        0        0      489 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/codeop.pyi
--rw-r--r--   0        0        0    14106 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/collections/__init__.pyi
--rw-r--r--   0        0        0       79 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/collections/abc.pyi
--rw-r--r--   0        0        0      578 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/colorsys.pyi
--rw-r--r--   0        0        0     3369 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/compileall.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/__init__.pyi
--rw-r--r--   0        0        0      629 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/__init__.pyi
--rw-r--r--   0        0        0     4702 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/_base.pyi
--rw-r--r--   0        0        0      804 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/process.pyi
--rw-r--r--   0        0        0     1431 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/thread.pyi
--rw-r--r--   0        0        0    10201 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/configparser.pyi
--rw-r--r--   0        0        0     4930 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/contextlib.pyi
--rw-r--r--   0        0        0     1696 2022-04-05 08:26:35.335163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/contextvars.pyi
--rw-r--r--   0        0        0      328 2022-04-05 08:26:35.319163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/copy.pyi
--rw-r--r--   0        0        0      750 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/copyreg.pyi
--rw-r--r--   0        0        0      648 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/crypt.pyi
--rw-r--r--   0        0        0     3119 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/csv.pyi
--rw-r--r--   0        0        0    12218 2022-04-05 08:26:35.379163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ctypes/__init__.pyi
--rw-r--r--   0        0        0      163 2022-04-05 08:26:35.379163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ctypes/util.pyi
--rw-r--r--   0        0        0     4642 2022-04-05 08:26:35.379163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ctypes/wintypes.pyi
--rw-r--r--   0        0        0      370 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/curses/__init__.pyi
--rw-r--r--   0        0        0     1236 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/curses/ascii.pyi
--rw-r--r--   0        0        0      801 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/curses/panel.pyi
--rw-r--r--   0        0        0      457 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/curses/textpad.pyi
--rw-r--r--   0        0        0     4123 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dataclasses.pyi
--rw-r--r--   0        0        0    13048 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/datetime.pyi
--rw-r--r--   0        0        0      997 2022-04-05 08:26:35.379163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/__init__.pyi
--rw-r--r--   0        0        0     1010 2022-04-05 08:26:35.379163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/dumb.pyi
--rw-r--r--   0        0        0     1363 2022-04-05 08:26:35.379163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/gnu.pyi
--rw-r--r--   0        0        0     1236 2022-04-05 08:26:35.379163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/ndbm.pyi
--rw-r--r--   0        0        0    17787 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/decimal.pyi
--rw-r--r--   0        0        0     4936 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/difflib.pyi
--rw-r--r--   0        0        0     3089 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dis.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/__init__.pyi
--rw-r--r--   0        0        0      598 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/archive_util.pyi
--rw-r--r--   0        0        0       78 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/bcppcompiler.pyi
--rw-r--r--   0        0        0     6449 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/ccompiler.pyi
--rw-r--r--   0        0        0     2803 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/cmd.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/__init__.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/bdist.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/bdist_dumb.pyi
--rw-r--r--   0        0        0      182 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/bdist_msi.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/bdist_packager.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/bdist_rpm.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/bdist_wininst.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/build.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/build_clib.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/build_ext.pyi
--rw-r--r--   0        0        0      217 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/build_py.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/build_scripts.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/check.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/clean.pyi
--rw-r--r--   0        0        0     3059 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/config.pyi
--rw-r--r--   0        0        0      365 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/install.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/install_data.pyi
--rw-r--r--   0        0        0      380 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/install_egg_info.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/install_headers.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/install_lib.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/install_scripts.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/register.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/sdist.pyi
--rw-r--r--   0        0        0      294 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/upload.pyi
--rw-r--r--   0        0        0      523 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/config.pyi
--rw-r--r--   0        0        0     1688 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/core.pyi
--rw-r--r--   0        0        0      138 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/cygwinccompiler.pyi
--rw-r--r--   0        0        0       51 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/debug.pyi
--rw-r--r--   0        0        0      252 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/dep_util.pyi
--rw-r--r--   0        0        0      555 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/dir_util.pyi
--rw-r--r--   0        0        0     2557 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/dist.pyi
--rw-r--r--   0        0        0      852 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/errors.pyi
--rw-r--r--   0        0        0      866 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/extension.pyi
--rw-r--r--   0        0        0      931 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/fancy_getopt.pyi
--rw-r--r--   0        0        0      439 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/file_util.pyi
--rw-r--r--   0        0        0     2383 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/filelist.pyi
--rw-r--r--   0        0        0      845 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/log.pyi
--rw-r--r--   0        0        0       78 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/msvccompiler.pyi
--rw-r--r--   0        0        0      227 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/spawn.pyi
--rw-r--r--   0        0        0      584 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/sysconfig.pyi
--rw-r--r--   0        0        0      726 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/text_file.pyi
--rw-r--r--   0        0        0       79 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/unixccompiler.pyi
--rw-r--r--   0        0        0      829 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/util.pyi
--rw-r--r--   0        0        0     1429 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/version.pyi
--rw-r--r--   0        0        0     7083 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/doctest.pyi
--rw-r--r--   0        0        0       79 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dummy_threading.pyi
--rw-r--r--   0        0        0      757 2022-04-05 08:26:35.383163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/__init__.pyi
--rw-r--r--   0        0        0    12252 2022-04-05 08:26:35.383163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/_header_value_parser.pyi
--rw-r--r--   0        0        0     1062 2022-04-05 08:26:35.383163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/charset.pyi
--rw-r--r--   0        0        0      489 2022-04-05 08:26:35.383163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/contentmanager.pyi
--rw-r--r--   0        0        0      214 2022-04-05 08:26:35.379163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/encoders.pyi
--rw-r--r--   0        0        0     1566 2022-04-05 08:26:35.383163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/errors.pyi
--rw-r--r--   0        0        0      823 2022-04-05 08:26:35.383163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/feedparser.pyi
--rw-r--r--   0        0        0     1252 2022-04-05 08:26:35.383163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/generator.pyi
--rw-r--r--   0        0        0     1025 2022-04-05 08:26:35.379163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/header.pyi
--rw-r--r--   0        0        0     4465 2022-04-05 08:26:35.383163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/headerregistry.pyi
--rw-r--r--   0        0        0      266 2022-04-05 08:26:35.383163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/iterators.pyi
--rw-r--r--   0        0        0     4929 2022-04-05 08:26:35.383163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/message.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.383163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/__init__.pyi
--rw-r--r--   0        0        0      499 2022-04-05 08:26:35.383163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/application.pyi
--rw-r--r--   0        0        0      502 2022-04-05 08:26:35.383163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/audio.pyi
--rw-r--r--   0        0        0      325 2022-04-05 08:26:35.383163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/base.pyi
--rw-r--r--   0        0        0      502 2022-04-05 08:26:35.383163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/image.pyi
--rw-r--r--   0        0        0      292 2022-04-05 08:26:35.383163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/message.pyi
--rw-r--r--   0        0        0      507 2022-04-05 08:26:35.383163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/multipart.pyi
--rw-r--r--   0        0        0       76 2022-04-05 08:26:35.383163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/nonmultipart.pyi
--rw-r--r--   0        0        0      297 2022-04-05 08:26:35.383163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/text.pyi
--rw-r--r--   0        0        0     1358 2022-04-05 08:26:35.383163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/parser.pyi
--rw-r--r--   0        0        0     2159 2022-04-05 08:26:35.383163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/policy.pyi
--rw-r--r--   0        0        0     1846 2022-04-05 08:26:35.383163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/utils.pyi
--rw-r--r--   0        0        0      332 2022-04-05 08:26:35.399163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/encodings/__init__.pyi
--rw-r--r--   0        0        0      875 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/encodings/utf_8.pyi
--rw-r--r--   0        0        0      562 2022-04-05 08:26:35.383163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ensurepip/__init__.pyi
--rw-r--r--   0        0        0     3431 2022-04-05 08:26:35.303163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/enum.pyi
--rw-r--r--   0        0        0     2011 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/errno.pyi
--rw-r--r--   0        0        0      644 2022-04-05 08:26:35.335163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/faulthandler.pyi
--rw-r--r--   0        0        0     2251 2022-04-05 08:26:35.335163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/fcntl.pyi
--rw-r--r--   0        0        0     2566 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/filecmp.pyi
--rw-r--r--   0        0        0     2601 2022-04-05 08:26:35.335163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/fileinput.pyi
--rw-r--r--   0        0        0      257 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/fnmatch.pyi
--rw-r--r--   0        0        0     4639 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/formatter.pyi
--rw-r--r--   0        0        0     6011 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/fractions.pyi
--rw-r--r--   0        0        0     6260 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ftplib.pyi
--rw-r--r--   0        0        0     5350 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/functools.pyi
--rw-r--r--   0        0        0     1135 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/gc.pyi
--rw-r--r--   0        0        0     1373 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/genericpath.pyi
--rw-r--r--   0        0        0      382 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/getopt.pyi
--rw-r--r--   0        0        0      178 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/getpass.pyi
--rw-r--r--   0        0        0     3210 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/gettext.pyi
--rw-r--r--   0        0        0      859 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/glob.pyi
--rw-r--r--   0        0        0      592 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/graphlib.pyi
--rw-r--r--   0        0        0      294 2022-04-05 08:26:35.319163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/grp.pyi
--rw-r--r--   0        0        0     4804 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/gzip.pyi
--rw-r--r--   0        0        0     4360 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/hashlib.pyi
--rw-r--r--   0        0        0      800 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/heapq.pyi
--rw-r--r--   0        0        0     1607 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/hmac.pyi
--rw-r--r--   0        0        0      122 2022-04-05 08:26:35.403163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/html/__init__.pyi
--rw-r--r--   0        0        0      136 2022-04-05 08:26:35.403163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/html/entities.pyi
--rw-r--r--   0        0        0     1645 2022-04-05 08:26:35.403163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/html/parser.pyi
--rw-r--r--   0        0        0     1940 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/__init__.pyi
--rw-r--r--   0        0        0     7031 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/client.pyi
--rw-r--r--   0        0        0     5845 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/cookiejar.pyi
--rw-r--r--   0        0        0     1934 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/cookies.pyi
--rw-r--r--   0        0        0     2853 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/server.pyi
--rw-r--r--   0        0        0     8034 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/imaplib.pyi
--rw-r--r--   0        0        0      604 2022-04-05 08:26:35.335163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/imghdr.pyi
--rw-r--r--   0        0        0     2343 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/imp.pyi
--rw-r--r--   0        0        0      571 2022-04-05 08:26:35.379163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/__init__.pyi
--rw-r--r--   0        0        0     4381 2022-04-05 08:26:35.375163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/abc.pyi
--rw-r--r--   0        0        0     4652 2022-04-05 08:26:35.375163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/machinery.pyi
--rw-r--r--   0        0        0     3743 2022-04-05 08:26:35.379163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/metadata.pyi
--rw-r--r--   0        0        0     1176 2022-04-05 08:26:35.375163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/resources.pyi
--rw-r--r--   0        0        0     1762 2022-04-05 08:26:35.375163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/util.pyi
--rw-r--r--   0        0        0    11110 2022-04-05 08:26:35.335163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/inspect.pyi
--rw-r--r--   0        0        0     7558 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/io.pyi
--rw-r--r--   0        0        0     5252 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ipaddress.pyi
--rw-r--r--   0        0        0     7901 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/itertools.pyi
--rw-r--r--   0        0        0     1977 2022-04-05 08:26:35.379163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/json/__init__.pyi
--rw-r--r--   0        0        0     1090 2022-04-05 08:26:35.379163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/json/decoder.pyi
--rw-r--r--   0        0        0      779 2022-04-05 08:26:35.379163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/json/encoder.pyi
--rw-r--r--   0        0        0       24 2022-04-05 08:26:35.379163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/json/tool.pyi
--rw-r--r--   0        0        0      210 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/keyword.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/__init__.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/__init__.pyi
--rw-r--r--   0        0        0      956 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/driver.pyi
--rw-r--r--   0        0        0      733 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/grammar.pyi
--rw-r--r--   0        0        0      172 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/literals.pyi
--rw-r--r--   0        0        0     1107 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/parse.pyi
--rw-r--r--   0        0        0     2140 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/pgen.pyi
--rw-r--r--   0        0        0     1065 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/token.pyi
--rw-r--r--   0        0        0      883 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/tokenize.pyi
--rw-r--r--   0        0        0     2208 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pygram.pyi
--rw-r--r--   0        0        0     3322 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pytree.pyi
--rw-r--r--   0        0        0      591 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/linecache.pyi
--rw-r--r--   0        0        0     2557 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/locale.pyi
--rw-r--r--   0        0        0    24560 2022-04-05 08:26:35.415163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/logging/__init__.pyi
--rw-r--r--   0        0        0     1218 2022-04-05 08:26:35.415163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/logging/config.pyi
--rw-r--r--   0        0        0     9986 2022-04-05 08:26:35.415163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/logging/handlers.pyi
--rw-r--r--   0        0        0     4587 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lzma.pyi
--rw-r--r--   0        0        0     3190 2022-04-05 08:26:35.319163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/macpath.pyi
--rw-r--r--   0        0        0      172 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/macurl2path.pyi
--rw-r--r--   0        0        0     8112 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/mailbox.pyi
--rw-r--r--   0        0        0      330 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/mailcap.pyi
--rw-r--r--   0        0        0      253 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/marshal.pyi
--rw-r--r--   0        0        0     3835 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/math.pyi
--rw-r--r--   0        0        0     1637 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/mimetypes.pyi
--rw-r--r--   0        0        0     4570 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/mmap.pyi
--rw-r--r--   0        0        0     3674 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/modulefinder.pyi
--rw-r--r--   0        0        0     6306 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/msilib/__init__.pyi
--rw-r--r--   0        0        0     2214 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/msilib/schema.pyi
--rw-r--r--   0        0        0      356 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/msilib/sequence.pyi
--rw-r--r--   0        0        0      202 2022-04-05 08:26:35.387163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/msilib/text.pyi
--rw-r--r--   0        0        0      795 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/msvcrt.pyi
--rw-r--r--   0        0        0     3553 2022-04-05 08:26:35.415163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/__init__.pyi
--rw-r--r--   0        0        0     2602 2022-04-05 08:26:35.415163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/connection.pyi
--rw-r--r--   0        0        0     7475 2022-04-05 08:26:35.415163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/context.pyi
--rw-r--r--   0        0        0     1572 2022-04-05 08:26:35.415163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/dummy/__init__.pyi
--rw-r--r--   0        0        0     1431 2022-04-05 08:26:35.415163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/dummy/connection.pyi
--rw-r--r--   0        0        0     4850 2022-04-05 08:26:35.415163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/managers.pyi
--rw-r--r--   0        0        0     3534 2022-04-05 08:26:35.415163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/pool.pyi
--rw-r--r--   0        0        0     1143 2022-04-05 08:26:35.415163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/process.pyi
--rw-r--r--   0        0        0     1288 2022-04-05 08:26:35.415163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/queues.pyi
--rw-r--r--   0        0        0     1302 2022-04-05 08:26:35.415163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/shared_memory.pyi
--rw-r--r--   0        0        0     3941 2022-04-05 08:26:35.415163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/sharedctypes.pyi
--rw-r--r--   0        0        0      690 2022-04-05 08:26:35.415163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/spawn.pyi
--rw-r--r--   0        0        0     1799 2022-04-05 08:26:35.415163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/synchronize.pyi
--rw-r--r--   0        0        0      598 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/netrc.pyi
--rw-r--r--   0        0        0      322 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/nis.pyi
--rw-r--r--   0        0        0     4321 2022-04-05 08:26:35.303163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/nntplib.pyi
--rw-r--r--   0        0        0     1936 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ntpath.pyi
--rw-r--r--   0        0        0       76 2022-04-05 08:26:35.319163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/nturl2path.pyi
--rw-r--r--   0        0        0     4335 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/numbers.pyi
--rw-r--r--   0        0        0      609 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/opcode.pyi
--rw-r--r--   0        0        0     8146 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/operator.pyi
--rw-r--r--   0        0        0    10261 2022-04-05 08:26:35.303163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/optparse.pyi
--rw-r--r--   0        0        0    30354 2022-04-05 08:26:35.379163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/os/__init__.pyi
--rw-r--r--   0        0        0       99 2022-04-05 08:26:35.379163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/os/path.pyi
--rw-r--r--   0        0        0     3065 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ossaudiodev.pyi
--rw-r--r--   0        0        0      966 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/parser.pyi
--rw-r--r--   0        0        0     6650 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pathlib.pyi
--rw-r--r--   0        0        0    10325 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pdb.pyi
--rw-r--r--   0        0        0     5322 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pickle.pyi
--rw-r--r--   0        0        0     4510 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pickletools.pyi
--rw-r--r--   0        0        0      514 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pipes.pyi
--rw-r--r--   0        0        0     1629 2022-04-05 08:26:35.319163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pkgutil.pyi
--rw-r--r--   0        0        0     2272 2022-04-05 08:26:35.303163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/platform.pyi
--rw-r--r--   0        0        0     2742 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/plistlib.pyi
--rw-r--r--   0        0        0     2500 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/poplib.pyi
--rw-r--r--   0        0        0     3006 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/posix.pyi
--rw-r--r--   0        0        0     2822 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/posixpath.pyi
--rw-r--r--   0        0        0     4231 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pprint.pyi
--rw-r--r--   0        0        0     1344 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/profile.pyi
--rw-r--r--   0        0        0     2213 2022-04-05 08:26:35.319163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pstats.pyi
--rw-r--r--   0        0        0      592 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pty.pyi
--rw-r--r--   0        0        0      354 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pwd.pyi
--rw-r--r--   0        0        0     1646 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/py_compile.pyi
--rw-r--r--   0        0        0     1192 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pyclbr.pyi
--rw-r--r--   0        0        0    10660 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pydoc.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.415163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pydoc_data/__init__.pyi
--rw-r--r--   0        0        0       48 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pydoc_data/topics.pyi
--rw-r--r--   0        0        0     3414 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pyexpat/__init__.pyi
--rw-r--r--   0        0        0     1275 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pyexpat/errors.pyi
--rw-r--r--   0        0        0      205 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pyexpat/model.pyi
--rw-r--r--   0        0        0     1884 2022-04-05 08:26:35.303163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/queue.pyi
--rw-r--r--   0        0        0      343 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/quopri.pyi
--rw-r--r--   0        0        0     4018 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/random.pyi
--rw-r--r--   0        0        0     4378 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/re.pyi
--rw-r--r--   0        0        0     1709 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/readline.pyi
--rw-r--r--   0        0        0     1228 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/reprlib.pyi
--rw-r--r--   0        0        0     1445 2022-04-05 08:26:35.319163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/resource.pyi
--rw-r--r--   0        0        0      308 2022-04-05 08:26:35.335163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/rlcompleter.pyi
--rw-r--r--   0        0        0      776 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/runpy.pyi
--rw-r--r--   0        0        0     1497 2022-04-05 08:26:35.319163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sched.pyi
--rw-r--r--   0        0        0      467 2022-04-05 08:26:35.319163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/secrets.pyi
--rw-r--r--   0        0        0     4828 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/select.pyi
--rw-r--r--   0        0        0     3673 2022-04-05 08:26:35.335163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/selectors.pyi
--rw-r--r--   0        0        0     1613 2022-04-05 08:26:35.335163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/shelve.pyi
--rw-r--r--   0        0        0     1354 2022-04-05 08:26:35.319163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/shlex.pyi
--rw-r--r--   0        0        0     6004 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/shutil.pyi
--rw-r--r--   0        0        0     5279 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/signal.pyi
--rw-r--r--   0        0        0      406 2022-04-05 08:26:35.335163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/site.pyi
--rw-r--r--   0        0        0     3282 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/smtpd.pyi
--rw-r--r--   0        0        0     5608 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/smtplib.pyi
--rw-r--r--   0        0        0      501 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sndhdr.pyi
--rw-r--r--   0        0        0    22875 2022-04-05 08:26:35.319163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/socket.pyi
--rw-r--r--   0        0        0     5134 2022-04-05 08:26:35.303163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/socketserver.pyi
--rw-r--r--   0        0        0      311 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/spwd.pyi
--rw-r--r--   0        0        0       43 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sqlite3/__init__.pyi
--rw-r--r--   0        0        0    11447 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sqlite3/dbapi2.pyi
--rw-r--r--   0        0        0     1073 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sre_compile.pyi
--rw-r--r--   0        0        0     3460 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sre_constants.pyi
--rw-r--r--   0        0        0     3820 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sre_parse.pyi
--rw-r--r--   0        0        0    16955 2022-04-05 08:26:35.335163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ssl.pyi
--rw-r--r--   0        0        0     1805 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/stat.pyi
--rw-r--r--   0        0        0     3798 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/statistics.pyi
--rw-r--r--   0        0        0     1423 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/string.pyi
--rw-r--r--   0        0        0      817 2022-04-05 08:26:35.303163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/stringprep.pyi
--rw-r--r--   0        0        0     1573 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/struct.pyi
--rw-r--r--   0        0        0    34838 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/subprocess.pyi
--rw-r--r--   0        0        0     2924 2022-04-05 08:26:35.335163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sunau.pyi
--rw-r--r--   0        0        0     1383 2022-04-05 08:26:35.303163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/symbol.pyi
--rw-r--r--   0        0        0     2051 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/symtable.pyi
--rw-r--r--   0        0        0     6810 2022-04-05 08:26:35.335163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sys.pyi
--rw-r--r--   0        0        0      871 2022-04-05 08:26:35.319163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sysconfig.pyi
--rw-r--r--   0        0        0      821 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/syslog.pyi
--rw-r--r--   0        0        0      447 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tabnanny.pyi
--rw-r--r--   0        0        0    11588 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tarfile.pyi
--rw-r--r--   0        0        0     2728 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/telnetlib.pyi
--rw-r--r--   0        0        0    12993 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tempfile.pyi
--rw-r--r--   0        0        0     3526 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/termios.pyi
--rw-r--r--   0        0        0     3234 2022-04-05 08:26:35.319163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/textwrap.pyi
--rw-r--r--   0        0        0       50 2022-04-05 08:26:35.335163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/this.pyi
--rw-r--r--   0        0        0     6460 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/threading.pyi
--rw-r--r--   0        0        0     4063 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/time.pyi
--rw-r--r--   0        0        0     1731 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/timeit.pyi
--rw-r--r--   0        0        0   118206 2022-04-05 08:26:35.403163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/__init__.pyi
--rw-r--r--   0        0        0      299 2022-04-05 08:26:35.403163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/colorchooser.pyi
--rw-r--r--   0        0        0      297 2022-04-05 08:26:35.403163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/commondialog.pyi
--rw-r--r--   0        0        0     1886 2022-04-05 08:26:35.403163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/constants.pyi
--rw-r--r--   0        0        0      291 2022-04-05 08:26:35.403163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/dialog.pyi
--rw-r--r--   0        0        0      568 2022-04-05 08:26:35.403163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/dnd.pyi
--rw-r--r--   0        0        0     2287 2022-04-05 08:26:35.403163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/filedialog.pyi
--rw-r--r--   0        0        0     3840 2022-04-05 08:26:35.403163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/font.pyi
--rw-r--r--   0        0        0     1170 2022-04-05 08:26:35.403163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/messagebox.pyi
--rw-r--r--   0        0        0      333 2022-04-05 08:26:35.403163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/scrolledtext.pyi
--rw-r--r--   0        0        0      990 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/simpledialog.pyi
--rw-r--r--   0        0        0    14945 2022-04-05 08:26:35.403163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/tix.pyi
--rw-r--r--   0        0        0    38044 2022-04-05 08:26:35.403163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/ttk.pyi
--rw-r--r--   0        0        0     1468 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/token.pyi
--rw-r--r--   0        0        0     3110 2022-04-05 08:26:35.303163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tokenize.pyi
--rw-r--r--   0        0        0     2457 2022-04-05 08:26:35.319163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/trace.pyi
--rw-r--r--   0        0        0     7350 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/traceback.pyi
--rw-r--r--   0        0        0     2795 2022-04-05 08:26:35.335163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tracemalloc.pyi
--rw-r--r--   0        0        0      275 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tty.pyi
--rw-r--r--   0        0        0    19727 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/turtle.pyi
--rw-r--r--   0        0        0    11394 2022-04-05 08:26:35.303163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/types.pyi
--rw-r--r--   0        0        0    25751 2022-04-05 08:26:35.319163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/typing.pyi
--rw-r--r--   0        0        0     4039 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/typing_extensions.pyi
--rw-r--r--   0        0        0     1794 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unicodedata.pyi
--rw-r--r--   0        0        0      689 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/__init__.pyi
--rw-r--r--   0        0        0      372 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/async_case.pyi
--rw-r--r--   0        0        0    12439 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/case.pyi
--rw-r--r--   0        0        0     2067 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/loader.pyi
--rw-r--r--   0        0        0     1691 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/main.pyi
--rw-r--r--   0        0        0    13313 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/mock.pyi
--rw-r--r--   0        0        0     1859 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/result.pyi
--rw-r--r--   0        0        0     1339 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/runner.pyi
--rw-r--r--   0        0        0      402 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/signals.pyi
--rw-r--r--   0        0        0      892 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/suite.pyi
--rw-r--r--   0        0        0      906 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/util.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/__init__.pyi
--rw-r--r--   0        0        0      643 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/error.pyi
--rw-r--r--   0        0        0     5009 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/parse.pyi
--rw-r--r--   0        0        0    16281 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/request.pyi
--rw-r--r--   0        0        0     2107 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/response.pyi
--rw-r--r--   0        0        0      703 2022-04-05 08:26:35.411163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/robotparser.pyi
--rw-r--r--   0        0        0      549 2022-04-05 08:26:35.303163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/uu.pyi
--rw-r--r--   0        0        0     3448 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/uuid.pyi
--rw-r--r--   0        0        0     2459 2022-04-05 08:26:35.379163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/venv/__init__.pyi
--rw-r--r--   0        0        0     2583 2022-04-05 08:26:35.311163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/warnings.pyi
--rw-r--r--   0        0        0     2653 2022-04-05 08:26:35.307163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wave.pyi
--rw-r--r--   0        0        0     4545 2022-04-05 08:26:35.319163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/weakref.pyi
--rw-r--r--   0        0        0     3253 2022-04-05 08:26:35.323163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/webbrowser.pyi
--rw-r--r--   0        0        0     3729 2022-04-05 08:26:35.327163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/winreg.pyi
--rw-r--r--   0        0        0      811 2022-04-05 08:26:35.335163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/winsound.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/__init__.pyi
--rw-r--r--   0        0        0     3125 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/handlers.pyi
--rw-r--r--   0        0        0     1250 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/headers.pyi
--rw-r--r--   0        0        0     1532 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/simple_server.pyi
--rw-r--r--   0        0        0       71 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/types.pyi
--rw-r--r--   0        0        0      896 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/util.pyi
--rw-r--r--   0        0        0     1867 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/validate.pyi
--rw-r--r--   0        0        0     2315 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xdrlib.pyi
--rw-r--r--   0        0        0       30 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/__init__.pyi
--rw-r--r--   0        0        0      457 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/NodeFilter.pyi
--rw-r--r--   0        0        0     1844 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/__init__.pyi
--rw-r--r--   0        0        0      457 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/domreg.pyi
--rw-r--r--   0        0        0       77 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/expatbuilder.pyi
--rw-r--r--   0        0        0      530 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/minicompat.pyi
--rw-r--r--   0        0        0    11040 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/minidom.pyi
--rw-r--r--   0        0        0       77 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/pulldom.pyi
--rw-r--r--   0        0        0      173 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/xmlbuilder.pyi
--rw-r--r--   0        0        0      873 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/ElementInclude.pyi
--rw-r--r--   0        0        0     1588 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/ElementPath.pyi
--rw-r--r--   0        0        0    15071 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/ElementTree.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/__init__.pyi
--rw-r--r--   0        0        0       50 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/cElementTree.pyi
--rw-r--r--   0        0        0       34 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/parsers/__init__.pyi
--rw-r--r--   0        0        0       22 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/parsers/expat/__init__.pyi
--rw-r--r--   0        0        0       29 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/parsers/expat/errors.pyi
--rw-r--r--   0        0        0       28 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/parsers/expat/model.pyi
--rw-r--r--   0        0        0     1389 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/__init__.pyi
--rw-r--r--   0        0        0     1391 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/handler.pyi
--rw-r--r--   0        0        0     2825 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/saxutils.pyi
--rw-r--r--   0        0        0     2444 2022-04-05 08:26:35.395163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/xmlreader.pyi
--rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xmlrpc/__init__.pyi
--rw-r--r--   0        0        0    12367 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xmlrpc/client.pyi
--rw-r--r--   0        0        0     6835 2022-04-05 08:26:35.391163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xmlrpc/server.pyi
--rw-r--r--   0        0        0      294 2022-04-05 08:26:35.319163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xxlimited.pyi
--rw-r--r--   0        0        0      678 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/zipapp.pyi
--rw-r--r--   0        0        0     7659 2022-04-05 08:26:35.315163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/zipfile.pyi
--rw-r--r--   0        0        0     1244 2022-04-05 08:26:35.303163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/zipimport.pyi
--rw-r--r--   0        0        0     1777 2022-04-05 08:26:35.331163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/zlib.pyi
--rw-r--r--   0        0        0     1183 2022-04-05 08:26:35.407163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/zoneinfo/__init__.pyi
--rw-r--r--   0        0        0     2216 2022-04-05 08:26:35.415163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stubs/mypy-extensions/mypy_extensions.pyi
--rw-r--r--   0        0        0     4831 2022-04-05 08:26:35.455163 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypyc/test-data/fixtures/typing-full.pyi
--rw-r--r--   0        0        0      341 2022-04-05 08:26:32.939168 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/py/__init__.pyi
--rw-r--r--   0        0        0     1205 2022-04-05 08:26:32.975168 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/py/_vendored_packages/iniconfig/__init__.pyi
--rw-r--r--   0        0        0     3409 2022-04-05 08:26:32.939168 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/py/error.pyi
--rw-r--r--   0        0        0     1205 2022-04-05 08:26:32.939168 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/py/iniconfig.pyi
--rw-r--r--   0        0        0     5277 2022-04-05 08:26:32.943168 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/py/io.pyi
--rw-r--r--   0        0        0     7168 2022-04-05 08:26:32.943168 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/py/path.pyi
--rw-r--r--   0        0        0      787 2022-04-05 08:26:32.943168 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/py/xml.pyi
--rw-r--r--   0        0        0     1762 2022-04-12 13:55:32.354372 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/pytz-stubs/__init__.pyi
--rw-r--r--   0        0        0      312 2022-04-12 13:55:32.354372 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/pytz-stubs/exceptions.pyi
--rw-r--r--   0        0        0     2219 2022-04-12 13:55:32.354372 nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/pytz-stubs/tzinfo.pyi
--rw-r--r--   0        0        0     1745 2022-04-05 09:39:19.126134 nwon_baseline-0.1.33/README.md
--rw-r--r--   0        0        0        0 2022-03-30 13:01:02.168845 nwon_baseline-0.1.33/nwon_baseline/__init__.py
--rw-r--r--   0        0        0      431 2022-04-12 14:14:45.868752 nwon_baseline-0.1.33/nwon_baseline/date_helper/__init__.py
--rw-r--r--   0        0        0      726 2022-06-21 09:50:39.516257 nwon_baseline-0.1.33/nwon_baseline/date_helper/country.py
--rw-r--r--   0        0        0      529 2022-04-12 14:03:37.577729 nwon_baseline-0.1.33/nwon_baseline/date_helper/datetime.py
--rw-r--r--   0        0        0      514 2022-04-12 14:03:47.313716 nwon_baseline-0.1.33/nwon_baseline/date_helper/time_differences.py
--rw-r--r--   0        0        0      606 2022-04-25 13:53:13.627090 nwon_baseline-0.1.33/nwon_baseline/directory_helper/__init__.py
--rw-r--r--   0        0        0     2212 2022-04-12 08:40:56.233856 nwon_baseline-0.1.33/nwon_baseline/directory_helper/directory_content.py
--rw-r--r--   0        0        0     1057 2022-04-12 08:44:33.265854 nwon_baseline-0.1.33/nwon_baseline/directory_helper/directory_interactions.py
--rw-r--r--   0        0        0      531 2022-05-12 07:08:30.597454 nwon_baseline-0.1.33/nwon_baseline/file_helper/__init__.py
--rw-r--r--   0        0        0     1452 2022-04-07 13:42:29.856122 nwon_baseline-0.1.33/nwon_baseline/file_helper/file.py
--rw-r--r--   0        0        0      718 2022-05-12 07:08:33.205452 nwon_baseline-0.1.33/nwon_baseline/file_helper/filename_from_url.py
--rw-r--r--   0        0        0      232 2022-04-05 08:48:23.005685 nwon_baseline-0.1.33/nwon_baseline/image_helper/__init__.py
--rw-r--r--   0        0        0      640 2022-04-04 06:36:54.202585 nwon_baseline-0.1.33/nwon_baseline/image_helper/image.py
--rw-r--r--   0        0        0      116 2022-04-05 08:47:47.541699 nwon_baseline-0.1.33/nwon_baseline/import_helper/__init__.py
--rw-r--r--   0        0        0     2026 2022-04-04 06:36:54.194585 nwon_baseline-0.1.33/nwon_baseline/import_helper/import_from_file.py
--rw-r--r--   0        0        0      224 2022-04-05 08:47:02.149711 nwon_baseline-0.1.33/nwon_baseline/poetry/__init__.py
--rw-r--r--   0        0        0      644 2022-04-04 06:36:54.194585 nwon_baseline-0.1.33/nwon_baseline/poetry/checking_version_argument.py
--rw-r--r--   0        0        0     1002 2022-04-04 06:36:54.194585 nwon_baseline-0.1.33/nwon_baseline/poetry/package_version.py
--rw-r--r--   0        0        0      463 2022-06-23 08:01:15.992282 nwon_baseline-0.1.33/nwon_baseline/print_helper/__init__.py
--rw-r--r--   0        0        0      570 2022-06-23 08:00:40.928324 nwon_baseline-0.1.33/nwon_baseline/print_helper/colored_printing.py
--rw-r--r--   0        0        0      490 2022-06-23 08:06:42.895903 nwon_baseline-0.1.33/nwon_baseline/print_helper/print_with_style.py
--rw-r--r--   0        0        0        0 2022-04-05 08:00:37.317785 nwon_baseline-0.1.33/nwon_baseline/py.typed
--rw-r--r--   0        0        0      403 2022-05-23 11:12:00.460291 nwon_baseline-0.1.33/nwon_baseline/pydantic/__init__.py
--rw-r--r--   0        0        0      667 2022-04-27 13:35:06.007169 nwon_baseline-0.1.33/nwon_baseline/pydantic/path_to_write_pydantic_model.py
--rw-r--r--   0        0        0      221 2022-05-23 11:10:23.684409 nwon_baseline-0.1.33/nwon_baseline/pydantic/pydantic_model_to_dict.py
--rw-r--r--   0        0        0      623 2022-04-27 13:35:38.467129 nwon_baseline-0.1.33/nwon_baseline/pydantic/save_pydantic_model_instance.py
--rw-r--r--   0        0        0      654 2022-04-27 13:35:16.363156 nwon_baseline-0.1.33/nwon_baseline/pydantic/save_pydantic_model_schema.py
--rw-r--r--   0        0        0      288 2022-06-15 11:29:44.664464 nwon_baseline-0.1.33/nwon_baseline/shell_helper/__init__.py
--rw-r--r--   0        0        0      645 2022-03-29 12:19:02.136741 nwon_baseline-0.1.33/nwon_baseline/shell_helper/execute_command.py
--rw-r--r--   0        0        0     1106 2022-06-15 09:34:18.102339 nwon_baseline-0.1.33/nwon_baseline/shell_helper/get_environment_variable.py
--rw-r--r--   0        0        0      274 2022-04-05 08:50:03.033631 nwon_baseline-0.1.33/nwon_baseline/type_helper/__init__.py
--rw-r--r--   0        0        0      476 2022-04-25 13:57:42.090917 nwon_baseline-0.1.33/nwon_baseline/type_helper/enum_type_guard.py
--rw-r--r--   0        0        0      557 2022-04-01 13:03:10.337749 nwon_baseline-0.1.33/nwon_baseline/type_helper/enum_value_list.py
--rw-r--r--   0        0        0      612 2022-04-25 14:00:15.618795 nwon_baseline-0.1.33/nwon_baseline/typings/__init__.py
--rw-r--r--   0        0        0       78 2022-04-25 14:03:36.534617 nwon_baseline-0.1.33/nwon_baseline/typings/any_dict.py
--rw-r--r--   0        0        0      242 2022-03-29 11:55:17.603051 nwon_baseline-0.1.33/nwon_baseline/typings/bounding_box.py
--rw-r--r--   0        0        0       63 2022-03-31 06:53:03.720819 nwon_baseline-0.1.33/nwon_baseline/typings/celery_return.py
--rw-r--r--   0        0        0      135 2022-03-29 09:54:50.423452 nwon_baseline-0.1.33/nwon_baseline/typings/request_body_format.py
--rw-r--r--   0        0        0      349 2022-03-31 07:14:17.268870 nwon_baseline-0.1.33/nwon_baseline/typings/terminal_colors.py
--rw-r--r--   0        0        0      141 2022-03-29 12:01:55.262340 nwon_baseline-0.1.33/nwon_baseline/typings/version_change.py
--rw-r--r--   0        0        0     1052 2022-06-23 08:06:49.659896 nwon_baseline-0.1.33/pyproject.toml
--rw-r--r--   0        0        0     2902 2022-06-23 08:06:50.680198 nwon_baseline-0.1.33/setup.py
--rw-r--r--   0        0        0     2479 2022-06-23 08:06:50.680464 nwon_baseline-0.1.33/PKG-INFO
+-rw-r--r--   0        0        0    15100 2022-04-05 08:26:32.639168 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/attr/__init__.pyi
+-rw-r--r--   0        0        0      317 2022-04-05 08:26:32.651168 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/attr/_cmp.pyi
+-rw-r--r--   0        0        0      209 2022-04-05 08:26:32.659168 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/attr/_version_info.pyi
+-rw-r--r--   0        0        0      416 2022-04-05 08:26:32.663168 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/attr/converters.pyi
+-rw-r--r--   0        0        0      539 2022-04-05 08:26:32.671168 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/attr/exceptions.pyi
+-rw-r--r--   0        0        0      215 2022-04-05 08:26:32.671168 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/attr/filters.pyi
+-rw-r--r--   0        0        0      573 2022-04-05 08:26:32.671168 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/attr/setters.pyi
+-rw-r--r--   0        0        0     2268 2022-04-05 08:26:32.671168 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/attr/validators.pyi
+-rw-r--r--   0        0        0     1982 2022-04-05 08:26:32.671168 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/attrs/__init__.pyi
+-rw-r--r--   0        0        0      572 2022-04-05 08:26:34.267165 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/humps/main.pyi
+-rw-r--r--   0        0        0     1205 2022-04-05 08:26:32.211169 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/iniconfig/__init__.pyi
+-rw-r--r--   0        0        0     1747 2022-04-05 08:26:35.351163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/BaseHTTPServer.pyi
+-rw-r--r--   0        0        0      187 2022-04-05 08:26:35.359163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/CGIHTTPServer.pyi
+-rw-r--r--   0        0        0     3869 2022-04-05 08:26:35.355163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ConfigParser.pyi
+-rw-r--r--   0        0        0     1342 2022-04-05 08:26:35.339163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/Cookie.pyi
+-rw-r--r--   0        0        0     1064 2022-04-05 08:26:35.347163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/HTMLParser.pyi
+-rw-r--r--   0        0        0      895 2022-04-05 08:26:35.359163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/Queue.pyi
+-rw-r--r--   0        0        0      648 2022-04-05 08:26:35.339163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/SimpleHTTPServer.pyi
+-rw-r--r--   0        0        0     4559 2022-04-05 08:26:35.351163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/SocketServer.pyi
+-rw-r--r--   0        0        0     1146 2022-04-05 08:26:35.351163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/StringIO.pyi
+-rw-r--r--   0        0        0     1663 2022-04-05 08:26:35.355163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/UserDict.pyi
+-rw-r--r--   0        0        0      630 2022-04-05 08:26:35.339163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/UserList.pyi
+-rw-r--r--   0        0        0     3934 2022-04-05 08:26:35.355163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/UserString.pyi
+-rw-r--r--   0        0        0    48689 2022-04-05 08:26:35.359163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/__builtin__.pyi
+-rw-r--r--   0        0        0     5726 2022-04-05 08:26:35.359163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_ast.pyi
+-rw-r--r--   0        0        0     1430 2022-04-05 08:26:35.351163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_collections.pyi
+-rw-r--r--   0        0        0      577 2022-04-05 08:26:35.355163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_functools.pyi
+-rw-r--r--   0        0        0      635 2022-04-05 08:26:35.339163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_hotshot.pyi
+-rw-r--r--   0        0        0     7016 2022-04-05 08:26:35.343163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_io.pyi
+-rw-r--r--   0        0        0      226 2022-04-05 08:26:35.351163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_json.pyi
+-rw-r--r--   0        0        0      300 2022-04-05 08:26:35.351163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_md5.pyi
+-rw-r--r--   0        0        0      348 2022-04-05 08:26:35.339163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_sha.pyi
+-rw-r--r--   0        0        0      632 2022-04-05 08:26:35.343163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_sha256.pyi
+-rw-r--r--   0        0        0      632 2022-04-05 08:26:35.339163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_sha512.pyi
+-rw-r--r--   0        0        0     6286 2022-04-05 08:26:35.339163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_socket.pyi
+-rw-r--r--   0        0        0     1934 2022-04-05 08:26:35.351163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_sre.pyi
+-rw-r--r--   0        0        0      767 2022-04-05 08:26:35.359163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_struct.pyi
+-rw-r--r--   0        0        0      677 2022-04-05 08:26:35.351163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_symtable.pyi
+-rw-r--r--   0        0        0      319 2022-04-05 08:26:35.355163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_threading_local.pyi
+-rw-r--r--   0        0        0     3696 2022-04-05 08:26:35.351163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_winreg.pyi
+-rw-r--r--   0        0        0     1147 2022-04-05 08:26:35.347163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/abc.pyi
+-rw-r--r--   0        0        0     1199 2022-04-05 08:26:35.339163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ast.pyi
+-rw-r--r--   0        0        0      117 2022-04-05 08:26:35.347163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/atexit.pyi
+-rw-r--r--   0        0        0    48689 2022-04-05 08:26:35.339163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/builtins.pyi
+-rw-r--r--   0        0        0      795 2022-04-05 08:26:35.339163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cPickle.pyi
+-rw-r--r--   0        0        0     1870 2022-04-05 08:26:35.351163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cStringIO.pyi
+-rw-r--r--   0        0        0     4050 2022-04-05 08:26:35.339163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cgi.pyi
+-rw-r--r--   0        0        0     4913 2022-04-05 08:26:35.351163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/collections.pyi
+-rw-r--r--   0        0        0      329 2022-04-05 08:26:35.339163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/commands.pyi
+-rw-r--r--   0        0        0      628 2022-04-05 08:26:35.351163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/compileall.pyi
+-rw-r--r--   0        0        0     4716 2022-04-05 08:26:35.351163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cookielib.pyi
+-rw-r--r--   0        0        0      750 2022-04-05 08:26:35.359163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/copy_reg.pyi
+-rw-r--r--   0        0        0      273 2022-04-05 08:26:35.355163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/dircache.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.367163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/__init__.pyi
+-rw-r--r--   0        0        0      447 2022-04-05 08:26:35.363163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/archive_util.pyi
+-rw-r--r--   0        0        0       78 2022-04-05 08:26:35.367163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/bcppcompiler.pyi
+-rw-r--r--   0        0        0     6449 2022-04-05 08:26:35.367163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/ccompiler.pyi
+-rw-r--r--   0        0        0     2817 2022-04-05 08:26:35.367163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/cmd.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/__init__.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.375163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/bdist.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/bdist_dumb.pyi
+-rw-r--r--   0        0        0      182 2022-04-05 08:26:35.371163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/bdist_msi.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/bdist_packager.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/bdist_rpm.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/bdist_wininst.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/build.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/build_clib.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/build_ext.pyi
+-rw-r--r--   0        0        0      181 2022-04-05 08:26:35.371163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/build_py.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/build_scripts.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.375163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/check.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/clean.pyi
+-rw-r--r--   0        0        0     3059 2022-04-05 08:26:35.375163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/config.pyi
+-rw-r--r--   0        0        0      338 2022-04-05 08:26:35.375163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/install.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/install_data.pyi
+-rw-r--r--   0        0        0      380 2022-04-05 08:26:35.371163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/install_egg_info.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/install_headers.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/install_lib.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/install_scripts.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/register.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.371163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/sdist.pyi
+-rw-r--r--   0        0        0      296 2022-04-05 08:26:35.371163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/upload.pyi
+-rw-r--r--   0        0        0      523 2022-04-05 08:26:35.371163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/config.pyi
+-rw-r--r--   0        0        0     1688 2022-04-05 08:26:35.367163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/core.pyi
+-rw-r--r--   0        0        0      138 2022-04-05 08:26:35.367163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/cygwinccompiler.pyi
+-rw-r--r--   0        0        0       12 2022-04-05 08:26:35.363163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/debug.pyi
+-rw-r--r--   0        0        0      252 2022-04-05 08:26:35.363163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/dep_util.pyi
+-rw-r--r--   0        0        0      555 2022-04-05 08:26:35.367163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/dir_util.pyi
+-rw-r--r--   0        0        0      508 2022-04-05 08:26:35.367163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/dist.pyi
+-rw-r--r--   0        0        0       90 2022-04-05 08:26:35.367163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/emxccompiler.pyi
+-rw-r--r--   0        0        0      852 2022-04-05 08:26:35.367163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/errors.pyi
+-rw-r--r--   0        0        0      706 2022-04-05 08:26:35.367163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/extension.pyi
+-rw-r--r--   0        0        0      859 2022-04-05 08:26:35.363163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/fancy_getopt.pyi
+-rw-r--r--   0        0        0      439 2022-04-05 08:26:35.367163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/file_util.pyi
+-rw-r--r--   0        0        0       20 2022-04-05 08:26:35.367163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/filelist.pyi
+-rw-r--r--   0        0        0      863 2022-04-05 08:26:35.371163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/log.pyi
+-rw-r--r--   0        0        0       78 2022-04-05 08:26:35.367163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/msvccompiler.pyi
+-rw-r--r--   0        0        0      227 2022-04-05 08:26:35.367163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/spawn.pyi
+-rw-r--r--   0        0        0      620 2022-04-05 08:26:35.367163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/sysconfig.pyi
+-rw-r--r--   0        0        0      716 2022-04-05 08:26:35.367163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/text_file.pyi
+-rw-r--r--   0        0        0       79 2022-04-05 08:26:35.367163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/unixccompiler.pyi
+-rw-r--r--   0        0        0      829 2022-04-05 08:26:35.367163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/util.pyi
+-rw-r--r--   0        0        0     1160 2022-04-05 08:26:35.367163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/version.pyi
+-rw-r--r--   0        0        0      794 2022-04-05 08:26:35.355163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/dummy_thread.pyi
+-rw-r--r--   0        0        0      159 2022-04-05 08:26:35.363163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/MIMEText.pyi
+-rw-r--r--   0        0        0      270 2022-04-05 08:26:35.363163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/__init__.pyi
+-rw-r--r--   0        0        0     1072 2022-04-05 08:26:35.363163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/_parseaddr.pyi
+-rw-r--r--   0        0        0      303 2022-04-05 08:26:35.363163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/base64mime.pyi
+-rw-r--r--   0        0        0      902 2022-04-05 08:26:35.363163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/charset.pyi
+-rw-r--r--   0        0        0      143 2022-04-05 08:26:35.359163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/encoders.pyi
+-rw-r--r--   0        0        0      536 2022-04-05 08:26:35.363163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/feedparser.pyi
+-rw-r--r--   0        0        0      377 2022-04-05 08:26:35.359163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/generator.pyi
+-rw-r--r--   0        0        0      457 2022-04-05 08:26:35.359163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/header.pyi
+-rw-r--r--   0        0        0      256 2022-04-05 08:26:35.363163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/iterators.pyi
+-rw-r--r--   0        0        0     1950 2022-04-05 08:26:35.363163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/message.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.363163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/__init__.pyi
+-rw-r--r--   0        0        0      371 2022-04-05 08:26:35.363163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/application.pyi
+-rw-r--r--   0        0        0      176 2022-04-05 08:26:35.363163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/audio.pyi
+-rw-r--r--   0        0        0      128 2022-04-05 08:26:35.363163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/base.pyi
+-rw-r--r--   0        0        0      176 2022-04-05 08:26:35.363163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/image.pyi
+-rw-r--r--   0        0        0      147 2022-04-05 08:26:35.363163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/message.pyi
+-rw-r--r--   0        0        0      159 2022-04-05 08:26:35.363163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/multipart.pyi
+-rw-r--r--   0        0        0      107 2022-04-05 08:26:35.363163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/nonmultipart.pyi
+-rw-r--r--   0        0        0      159 2022-04-05 08:26:35.363163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/mime/text.pyi
+-rw-r--r--   0        0        0      415 2022-04-05 08:26:35.363163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/parser.pyi
+-rw-r--r--   0        0        0      490 2022-04-05 08:26:35.359163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/quoprimime.pyi
+-rw-r--r--   0        0        0      760 2022-04-05 08:26:35.359163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/utils.pyi
+-rw-r--r--   0        0        0      184 2022-04-05 08:26:35.375163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/encodings/__init__.pyi
+-rw-r--r--   0        0        0      573 2022-04-05 08:26:35.375163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/encodings/utf_8.pyi
+-rw-r--r--   0        0        0     1756 2022-04-05 08:26:35.343163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/exceptions.pyi
+-rw-r--r--   0        0        0     1580 2022-04-05 08:26:35.359163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/fcntl.pyi
+-rw-r--r--   0        0        0      348 2022-04-05 08:26:35.343163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/fnmatch.pyi
+-rw-r--r--   0        0        0     1181 2022-04-05 08:26:35.347163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/functools.pyi
+-rw-r--r--   0        0        0      194 2022-04-05 08:26:35.355163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/future_builtins.pyi
+-rw-r--r--   0        0        0      752 2022-04-05 08:26:35.343163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/gc.pyi
+-rw-r--r--   0        0        0      448 2022-04-05 08:26:35.351163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/getopt.pyi
+-rw-r--r--   0        0        0      160 2022-04-05 08:26:35.343163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/getpass.pyi
+-rw-r--r--   0        0        0     2285 2022-04-05 08:26:35.343163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/gettext.pyi
+-rw-r--r--   0        0        0      375 2022-04-05 08:26:35.347163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/glob.pyi
+-rw-r--r--   0        0        0      997 2022-04-05 08:26:35.347163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/gzip.pyi
+-rw-r--r--   0        0        0      971 2022-04-05 08:26:35.355163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/hashlib.pyi
+-rw-r--r--   0        0        0      756 2022-04-05 08:26:35.343163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/heapq.pyi
+-rw-r--r--   0        0        0      114 2022-04-05 08:26:35.343163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/htmlentitydefs.pyi
+-rw-r--r--   0        0        0     5929 2022-04-05 08:26:35.339163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/httplib.pyi
+-rw-r--r--   0        0        0     1290 2022-04-05 08:26:35.343163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/imp.pyi
+-rw-r--r--   0        0        0      134 2022-04-05 08:26:35.343163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/importlib.pyi
+-rw-r--r--   0        0        0     4692 2022-04-05 08:26:35.359163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/inspect.pyi
+-rw-r--r--   0        0        0     1136 2022-04-05 08:26:35.355163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/io.pyi
+-rw-r--r--   0        0        0     5976 2022-04-05 08:26:35.355163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/itertools.pyi
+-rw-r--r--   0        0        0     3206 2022-04-05 08:26:35.347163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/json.pyi
+-rw-r--r--   0        0        0     9541 2022-04-05 08:26:35.375163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/logging/__init__.pyi
+-rw-r--r--   0        0        0      458 2022-04-05 08:26:35.375163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/logging/config.pyi
+-rw-r--r--   0        0        0     4237 2022-04-05 08:26:35.375163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/logging/handlers.pyi
+-rw-r--r--   0        0        0      264 2022-04-05 08:26:35.339163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/markupbase.pyi
+-rw-r--r--   0        0        0       74 2022-04-05 08:26:35.347163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/md5.pyi
+-rw-r--r--   0        0        0      703 2022-04-05 08:26:35.351163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/mimetools.pyi
+-rw-r--r--   0        0        0     1921 2022-04-05 08:26:35.375163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/__init__.pyi
+-rw-r--r--   0        0        0     1392 2022-04-05 08:26:35.375163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/dummy/__init__.pyi
+-rw-r--r--   0        0        0      673 2022-04-05 08:26:35.375163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/dummy/connection.pyi
+-rw-r--r--   0        0        0     2038 2022-04-05 08:26:35.375163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/pool.pyi
+-rw-r--r--   0        0        0      906 2022-04-05 08:26:35.375163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/process.pyi
+-rw-r--r--   0        0        0      758 2022-04-05 08:26:35.375163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/util.pyi
+-rw-r--r--   0        0        0      339 2022-04-05 08:26:35.355163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/mutex.pyi
+-rw-r--r--   0        0        0     2937 2022-04-05 08:26:35.343163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ntpath.pyi
+-rw-r--r--   0        0        0      115 2022-04-05 08:26:35.347163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/nturl2path.pyi
+-rw-r--r--   0        0        0    13260 2022-04-05 08:26:35.359163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/os/__init__.pyi
+-rw-r--r--   0        0        0     2935 2022-04-05 08:26:35.359163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/os/path.pyi
+-rw-r--r--   0        0        0     2937 2022-04-05 08:26:35.351163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/os2emxpath.pyi
+-rw-r--r--   0        0        0      467 2022-04-05 08:26:35.343163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/pipes.pyi
+-rw-r--r--   0        0        0     1809 2022-04-05 08:26:35.339163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/platform.pyi
+-rw-r--r--   0        0        0      999 2022-04-05 08:26:35.355163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/popen2.pyi
+-rw-r--r--   0        0        0     6396 2022-04-05 08:26:35.355163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/posix.pyi
+-rw-r--r--   0        0        0     2937 2022-04-05 08:26:35.343163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/posixpath.pyi
+-rw-r--r--   0        0        0     3156 2022-04-05 08:26:35.351163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/random.pyi
+-rw-r--r--   0        0        0     3641 2022-04-05 08:26:35.355163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/re.pyi
+-rw-r--r--   0        0        0     1095 2022-04-05 08:26:35.343163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/repr.pyi
+-rw-r--r--   0        0        0      877 2022-04-05 08:26:35.347163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/resource.pyi
+-rw-r--r--   0        0        0     2163 2022-04-05 08:26:35.347163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/rfc822.pyi
+-rw-r--r--   0        0        0      230 2022-04-05 08:26:35.355163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/robotparser.pyi
+-rw-r--r--   0        0        0      541 2022-04-05 08:26:35.355163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/runpy.pyi
+-rw-r--r--   0        0        0     2975 2022-04-05 08:26:35.359163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sets.pyi
+-rw-r--r--   0        0        0      236 2022-04-05 08:26:35.347163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sha.pyi
+-rw-r--r--   0        0        0     1612 2022-04-05 08:26:35.359163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/shelve.pyi
+-rw-r--r--   0        0        0     1025 2022-04-05 08:26:35.347163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/shlex.pyi
+-rw-r--r--   0        0        0     1571 2022-04-05 08:26:35.343163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/signal.pyi
+-rw-r--r--   0        0        0     2542 2022-04-05 08:26:35.355163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/smtplib.pyi
+-rw-r--r--   0        0        0      308 2022-04-05 08:26:35.351163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/spwd.pyi
+-rw-r--r--   0        0        0     1744 2022-04-05 08:26:35.347163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sre_constants.pyi
+-rw-r--r--   0        0        0     2311 2022-04-05 08:26:35.339163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sre_parse.pyi
+-rw-r--r--   0        0        0      992 2022-04-05 08:26:35.343163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/stat.pyi
+-rw-r--r--   0        0        0     3567 2022-04-05 08:26:35.339163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/string.pyi
+-rw-r--r--   0        0        0     2010 2022-04-05 08:26:35.347163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/stringold.pyi
+-rw-r--r--   0        0        0     1157 2022-04-05 08:26:35.339163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/strop.pyi
+-rw-r--r--   0        0        0     3282 2022-04-05 08:26:35.355163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/subprocess.pyi
+-rw-r--r--   0        0        0     1341 2022-04-05 08:26:35.339163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/symbol.pyi
+-rw-r--r--   0        0        0     3616 2022-04-05 08:26:35.359163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sys.pyi
+-rw-r--r--   0        0        0     3696 2022-04-05 08:26:35.347163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/tempfile.pyi
+-rw-r--r--   0        0        0     1854 2022-04-05 08:26:35.347163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/textwrap.pyi
+-rw-r--r--   0        0        0      920 2022-04-05 08:26:35.339163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/thread.pyi
+-rw-r--r--   0        0        0      243 2022-04-05 08:26:35.347163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/toaiff.pyi
+-rw-r--r--   0        0        0     2686 2022-04-05 08:26:35.339163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/tokenize.pyi
+-rw-r--r--   0        0        0     5465 2022-04-05 08:26:35.339163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/types.pyi
+-rw-r--r--   0        0        0    17748 2022-04-05 08:26:35.347163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/typing.pyi
+-rw-r--r--   0        0        0    12726 2022-04-05 08:26:35.351163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/unittest.pyi
+-rw-r--r--   0        0        0     4765 2022-04-05 08:26:35.359163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/urllib.pyi
+-rw-r--r--   0        0        0     8409 2022-04-05 08:26:35.355163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/urllib2.pyi
+-rw-r--r--   0        0        0     1944 2022-04-05 08:26:35.343163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/urlparse.pyi
+-rw-r--r--   0        0        0       83 2022-04-05 08:26:35.343163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/user.pyi
+-rw-r--r--   0        0        0       85 2022-04-05 08:26:35.347163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/whichdb.pyi
+-rw-r--r--   0        0        0     9769 2022-04-05 08:26:35.339163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xmlrpclib.pyi
+-rw-r--r--   0        0        0      716 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/__future__.pyi
+-rw-r--r--   0        0        0       63 2022-04-05 08:26:35.319163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/__main__.pyi
+-rw-r--r--   0        0        0     8975 2022-04-05 08:26:35.335163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_ast.pyi
+-rw-r--r--   0        0        0     1358 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_bisect.pyi
+-rw-r--r--   0        0        0       63 2022-04-05 08:26:35.319163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_bootlocale.pyi
+-rw-r--r--   0        0        0     5309 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_codecs.pyi
+-rw-r--r--   0        0        0     1210 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_collections_abc.pyi
+-rw-r--r--   0        0        0      388 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_compat_pickle.pyi
+-rw-r--r--   0        0        0      915 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_compression.pyi
+-rw-r--r--   0        0        0     1574 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_csv.pyi
+-rw-r--r--   0        0        0    14505 2022-04-05 08:26:35.335163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_curses.pyi
+-rw-r--r--   0        0        0       22 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_decimal.pyi
+-rw-r--r--   0        0        0      800 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_dummy_thread.pyi
+-rw-r--r--   0        0        0     6460 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_dummy_threading.pyi
+-rw-r--r--   0        0        0      613 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_heapq.pyi
+-rw-r--r--   0        0        0      705 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_imp.pyi
+-rw-r--r--   0        0        0     1124 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_json.pyi
+-rw-r--r--   0        0        0      256 2022-04-05 08:26:35.335163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_markupbase.pyi
+-rw-r--r--   0        0        0     2168 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_msi.pyi
+-rw-r--r--   0        0        0     1310 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_operator.pyi
+-rw-r--r--   0        0        0     1796 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_osx_support.pyi
+-rw-r--r--   0        0        0      557 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_posixsubprocess.pyi
+-rw-r--r--   0        0        0      376 2022-04-05 08:26:35.335163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_py_abc.pyi
+-rw-r--r--   0        0        0      157 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_pydecimal.pyi
+-rw-r--r--   0        0        0      478 2022-04-05 08:26:35.303163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_random.pyi
+-rw-r--r--   0        0        0      534 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_sitebuiltins.pyi
+-rw-r--r--   0        0        0     1179 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_stat.pyi
+-rw-r--r--   0        0        0     1451 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_thread.pyi
+-rw-r--r--   0        0        0      490 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_threading_local.pyi
+-rw-r--r--   0        0        0     2709 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_tkinter.pyi
+-rw-r--r--   0        0        0      563 2022-04-05 08:26:35.319163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_tracemalloc.pyi
+-rw-r--r--   0        0        0     4926 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_typeshed/__init__.pyi
+-rw-r--r--   0        0        0      249 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_typeshed/tkinter.pyi
+-rw-r--r--   0        0        0     1293 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_typeshed/wsgi.pyi
+-rw-r--r--   0        0        0      528 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_typeshed/xml.pyi
+-rw-r--r--   0        0        0     2233 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_warnings.pyi
+-rw-r--r--   0        0        0     1226 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_weakref.pyi
+-rw-r--r--   0        0        0     2410 2022-04-05 08:26:35.339163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_weakrefset.pyi
+-rw-r--r--   0        0        0     4507 2022-04-05 08:26:35.335163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_winapi.pyi
+-rw-r--r--   0        0        0      596 2022-04-05 08:26:35.319163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/abc.pyi
+-rw-r--r--   0        0        0     3393 2022-04-05 08:26:35.319163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/aifc.pyi
+-rw-r--r--   0        0        0      123 2022-04-05 08:26:35.319163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/antigravity.pyi
+-rw-r--r--   0        0        0    18345 2022-04-05 08:26:35.335163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/argparse.pyi
+-rw-r--r--   0        0        0     3623 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/array.pyi
+-rw-r--r--   0        0        0     9090 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ast.pyi
+-rw-r--r--   0        0        0     1555 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asynchat.pyi
+-rw-r--r--   0        0        0     4242 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/__init__.pyi
+-rw-r--r--   0        0        0    14883 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/base_events.pyi
+-rw-r--r--   0        0        0      733 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/base_futures.pyi
+-rw-r--r--   0        0        0     3239 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/base_subprocess.pyi
+-rw-r--r--   0        0        0      412 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/base_tasks.pyi
+-rw-r--r--   0        0        0      180 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/compat.pyi
+-rw-r--r--   0        0        0      327 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/constants.pyi
+-rw-r--r--   0        0        0      226 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/coroutines.pyi
+-rw-r--r--   0        0        0    19207 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/events.pyi
+-rw-r--r--   0        0        0      562 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/exceptions.pyi
+-rw-r--r--   0        0        0      931 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/format_helpers.pyi
+-rw-r--r--   0        0        0     2581 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/futures.pyi
+-rw-r--r--   0        0        0     2806 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/locks.pyi
+-rw-r--r--   0        0        0       39 2022-04-05 08:26:35.403163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/log.pyi
+-rw-r--r--   0        0        0     3178 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/proactor_events.pyi
+-rw-r--r--   0        0        0     1072 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/protocols.pyi
+-rw-r--r--   0        0        0     1166 2022-04-05 08:26:35.403163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/queues.pyi
+-rw-r--r--   0        0        0      314 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/runners.pyi
+-rw-r--r--   0        0        0      215 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/selector_events.pyi
+-rw-r--r--   0        0        0     5420 2022-04-05 08:26:35.403163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/sslproto.pyi
+-rw-r--r--   0        0        0      396 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/staggered.pyi
+-rw-r--r--   0        0        0     4021 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/streams.pyi
+-rw-r--r--   0        0        0     6000 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/subprocess.pyi
+-rw-r--r--   0        0        0    12113 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/tasks.pyi
+-rw-r--r--   0        0        0      194 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/threads.pyi
+-rw-r--r--   0        0        0     1886 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/transports.pyi
+-rw-r--r--   0        0        0     4592 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/trsock.pyi
+-rw-r--r--   0        0        0     2548 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/unix_events.pyi
+-rw-r--r--   0        0        0     3554 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/windows_events.pyi
+-rw-r--r--   0        0        0      983 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/windows_utils.pyi
+-rw-r--r--   0        0        0     5534 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncore.pyi
+-rw-r--r--   0        0        0      271 2022-04-05 08:26:35.319163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/atexit.pyi
+-rw-r--r--   0        0        0     2119 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/audioop.pyi
+-rw-r--r--   0        0        0     1772 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/base64.pyi
+-rw-r--r--   0        0        0     4644 2022-04-05 08:26:35.303163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/bdb.pyi
+-rw-r--r--   0        0        0     1555 2022-04-05 08:26:35.335163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/binascii.pyi
+-rw-r--r--   0        0        0     1147 2022-04-05 08:26:35.303163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/binhex.pyi
+-rw-r--r--   0        0        0       67 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/bisect.pyi
+-rw-r--r--   0        0        0    57130 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/builtins.pyi
+-rw-r--r--   0        0        0     2836 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/bz2.pyi
+-rw-r--r--   0        0        0     1481 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/cProfile.pyi
+-rw-r--r--   0        0        0     5796 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/calendar.pyi
+-rw-r--r--   0        0        0     3746 2022-04-05 08:26:35.303163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/cgi.pyi
+-rw-r--r--   0        0        0     1447 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/cgitb.pyi
+-rw-r--r--   0        0        0      613 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/chunk.pyi
+-rw-r--r--   0        0        0     1226 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/cmath.pyi
+-rw-r--r--   0        0        0     1658 2022-04-05 08:26:35.319163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/cmd.pyi
+-rw-r--r--   0        0        0     1522 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/code.pyi
+-rw-r--r--   0        0        0    12435 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/codecs.pyi
+-rw-r--r--   0        0        0      489 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/codeop.pyi
+-rw-r--r--   0        0        0    14106 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/collections/__init__.pyi
+-rw-r--r--   0        0        0       79 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/collections/abc.pyi
+-rw-r--r--   0        0        0      578 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/colorsys.pyi
+-rw-r--r--   0        0        0     3369 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/compileall.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/__init__.pyi
+-rw-r--r--   0        0        0      629 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/__init__.pyi
+-rw-r--r--   0        0        0     4702 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/_base.pyi
+-rw-r--r--   0        0        0      804 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/process.pyi
+-rw-r--r--   0        0        0     1431 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/thread.pyi
+-rw-r--r--   0        0        0    10201 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/configparser.pyi
+-rw-r--r--   0        0        0     4930 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/contextlib.pyi
+-rw-r--r--   0        0        0     1696 2022-04-05 08:26:35.335163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/contextvars.pyi
+-rw-r--r--   0        0        0      328 2022-04-05 08:26:35.319163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/copy.pyi
+-rw-r--r--   0        0        0      750 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/copyreg.pyi
+-rw-r--r--   0        0        0      648 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/crypt.pyi
+-rw-r--r--   0        0        0     3119 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/csv.pyi
+-rw-r--r--   0        0        0    12218 2022-04-05 08:26:35.379163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ctypes/__init__.pyi
+-rw-r--r--   0        0        0      163 2022-04-05 08:26:35.379163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ctypes/util.pyi
+-rw-r--r--   0        0        0     4642 2022-04-05 08:26:35.379163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ctypes/wintypes.pyi
+-rw-r--r--   0        0        0      370 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/curses/__init__.pyi
+-rw-r--r--   0        0        0     1236 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/curses/ascii.pyi
+-rw-r--r--   0        0        0      801 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/curses/panel.pyi
+-rw-r--r--   0        0        0      457 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/curses/textpad.pyi
+-rw-r--r--   0        0        0     4123 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dataclasses.pyi
+-rw-r--r--   0        0        0    13048 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/datetime.pyi
+-rw-r--r--   0        0        0      997 2022-04-05 08:26:35.379163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/__init__.pyi
+-rw-r--r--   0        0        0     1010 2022-04-05 08:26:35.379163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/dumb.pyi
+-rw-r--r--   0        0        0     1363 2022-04-05 08:26:35.379163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/gnu.pyi
+-rw-r--r--   0        0        0     1236 2022-04-05 08:26:35.379163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/ndbm.pyi
+-rw-r--r--   0        0        0    17787 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/decimal.pyi
+-rw-r--r--   0        0        0     4936 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/difflib.pyi
+-rw-r--r--   0        0        0     3089 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dis.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/__init__.pyi
+-rw-r--r--   0        0        0      598 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/archive_util.pyi
+-rw-r--r--   0        0        0       78 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/bcppcompiler.pyi
+-rw-r--r--   0        0        0     6449 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/ccompiler.pyi
+-rw-r--r--   0        0        0     2803 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/cmd.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/__init__.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/bdist.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/bdist_dumb.pyi
+-rw-r--r--   0        0        0      182 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/bdist_msi.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/bdist_packager.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/bdist_rpm.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/bdist_wininst.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/build.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/build_clib.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/build_ext.pyi
+-rw-r--r--   0        0        0      217 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/build_py.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/build_scripts.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/check.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/clean.pyi
+-rw-r--r--   0        0        0     3059 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/config.pyi
+-rw-r--r--   0        0        0      365 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/install.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/install_data.pyi
+-rw-r--r--   0        0        0      380 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/install_egg_info.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/install_headers.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/install_lib.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/install_scripts.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/register.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/sdist.pyi
+-rw-r--r--   0        0        0      294 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/upload.pyi
+-rw-r--r--   0        0        0      523 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/config.pyi
+-rw-r--r--   0        0        0     1688 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/core.pyi
+-rw-r--r--   0        0        0      138 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/cygwinccompiler.pyi
+-rw-r--r--   0        0        0       51 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/debug.pyi
+-rw-r--r--   0        0        0      252 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/dep_util.pyi
+-rw-r--r--   0        0        0      555 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/dir_util.pyi
+-rw-r--r--   0        0        0     2557 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/dist.pyi
+-rw-r--r--   0        0        0      852 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/errors.pyi
+-rw-r--r--   0        0        0      866 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/extension.pyi
+-rw-r--r--   0        0        0      931 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/fancy_getopt.pyi
+-rw-r--r--   0        0        0      439 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/file_util.pyi
+-rw-r--r--   0        0        0     2383 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/filelist.pyi
+-rw-r--r--   0        0        0      845 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/log.pyi
+-rw-r--r--   0        0        0       78 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/msvccompiler.pyi
+-rw-r--r--   0        0        0      227 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/spawn.pyi
+-rw-r--r--   0        0        0      584 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/sysconfig.pyi
+-rw-r--r--   0        0        0      726 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/text_file.pyi
+-rw-r--r--   0        0        0       79 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/unixccompiler.pyi
+-rw-r--r--   0        0        0      829 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/util.pyi
+-rw-r--r--   0        0        0     1429 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/version.pyi
+-rw-r--r--   0        0        0     7083 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/doctest.pyi
+-rw-r--r--   0        0        0       79 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dummy_threading.pyi
+-rw-r--r--   0        0        0      757 2022-04-05 08:26:35.383163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/__init__.pyi
+-rw-r--r--   0        0        0    12252 2022-04-05 08:26:35.383163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/_header_value_parser.pyi
+-rw-r--r--   0        0        0     1062 2022-04-05 08:26:35.383163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/charset.pyi
+-rw-r--r--   0        0        0      489 2022-04-05 08:26:35.383163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/contentmanager.pyi
+-rw-r--r--   0        0        0      214 2022-04-05 08:26:35.379163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/encoders.pyi
+-rw-r--r--   0        0        0     1566 2022-04-05 08:26:35.383163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/errors.pyi
+-rw-r--r--   0        0        0      823 2022-04-05 08:26:35.383163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/feedparser.pyi
+-rw-r--r--   0        0        0     1252 2022-04-05 08:26:35.383163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/generator.pyi
+-rw-r--r--   0        0        0     1025 2022-04-05 08:26:35.379163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/header.pyi
+-rw-r--r--   0        0        0     4465 2022-04-05 08:26:35.383163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/headerregistry.pyi
+-rw-r--r--   0        0        0      266 2022-04-05 08:26:35.383163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/iterators.pyi
+-rw-r--r--   0        0        0     4929 2022-04-05 08:26:35.383163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/message.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.383163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/__init__.pyi
+-rw-r--r--   0        0        0      499 2022-04-05 08:26:35.383163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/application.pyi
+-rw-r--r--   0        0        0      502 2022-04-05 08:26:35.383163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/audio.pyi
+-rw-r--r--   0        0        0      325 2022-04-05 08:26:35.383163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/base.pyi
+-rw-r--r--   0        0        0      502 2022-04-05 08:26:35.383163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/image.pyi
+-rw-r--r--   0        0        0      292 2022-04-05 08:26:35.383163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/message.pyi
+-rw-r--r--   0        0        0      507 2022-04-05 08:26:35.383163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/multipart.pyi
+-rw-r--r--   0        0        0       76 2022-04-05 08:26:35.383163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/nonmultipart.pyi
+-rw-r--r--   0        0        0      297 2022-04-05 08:26:35.383163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/mime/text.pyi
+-rw-r--r--   0        0        0     1358 2022-04-05 08:26:35.383163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/parser.pyi
+-rw-r--r--   0        0        0     2159 2022-04-05 08:26:35.383163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/policy.pyi
+-rw-r--r--   0        0        0     1846 2022-04-05 08:26:35.383163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/utils.pyi
+-rw-r--r--   0        0        0      332 2022-04-05 08:26:35.399163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/encodings/__init__.pyi
+-rw-r--r--   0        0        0      875 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/encodings/utf_8.pyi
+-rw-r--r--   0        0        0      562 2022-04-05 08:26:35.383163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ensurepip/__init__.pyi
+-rw-r--r--   0        0        0     3431 2022-04-05 08:26:35.303163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/enum.pyi
+-rw-r--r--   0        0        0     2011 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/errno.pyi
+-rw-r--r--   0        0        0      644 2022-04-05 08:26:35.335163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/faulthandler.pyi
+-rw-r--r--   0        0        0     2251 2022-04-05 08:26:35.335163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/fcntl.pyi
+-rw-r--r--   0        0        0     2566 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/filecmp.pyi
+-rw-r--r--   0        0        0     2601 2022-04-05 08:26:35.335163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/fileinput.pyi
+-rw-r--r--   0        0        0      257 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/fnmatch.pyi
+-rw-r--r--   0        0        0     4639 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/formatter.pyi
+-rw-r--r--   0        0        0     6011 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/fractions.pyi
+-rw-r--r--   0        0        0     6260 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ftplib.pyi
+-rw-r--r--   0        0        0     5350 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/functools.pyi
+-rw-r--r--   0        0        0     1135 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/gc.pyi
+-rw-r--r--   0        0        0     1373 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/genericpath.pyi
+-rw-r--r--   0        0        0      382 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/getopt.pyi
+-rw-r--r--   0        0        0      178 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/getpass.pyi
+-rw-r--r--   0        0        0     3210 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/gettext.pyi
+-rw-r--r--   0        0        0      859 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/glob.pyi
+-rw-r--r--   0        0        0      592 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/graphlib.pyi
+-rw-r--r--   0        0        0      294 2022-04-05 08:26:35.319163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/grp.pyi
+-rw-r--r--   0        0        0     4804 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/gzip.pyi
+-rw-r--r--   0        0        0     4360 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/hashlib.pyi
+-rw-r--r--   0        0        0      800 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/heapq.pyi
+-rw-r--r--   0        0        0     1607 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/hmac.pyi
+-rw-r--r--   0        0        0      122 2022-04-05 08:26:35.403163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/html/__init__.pyi
+-rw-r--r--   0        0        0      136 2022-04-05 08:26:35.403163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/html/entities.pyi
+-rw-r--r--   0        0        0     1645 2022-04-05 08:26:35.403163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/html/parser.pyi
+-rw-r--r--   0        0        0     1940 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/__init__.pyi
+-rw-r--r--   0        0        0     7031 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/client.pyi
+-rw-r--r--   0        0        0     5845 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/cookiejar.pyi
+-rw-r--r--   0        0        0     1934 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/cookies.pyi
+-rw-r--r--   0        0        0     2853 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/server.pyi
+-rw-r--r--   0        0        0     8034 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/imaplib.pyi
+-rw-r--r--   0        0        0      604 2022-04-05 08:26:35.335163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/imghdr.pyi
+-rw-r--r--   0        0        0     2343 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/imp.pyi
+-rw-r--r--   0        0        0      571 2022-04-05 08:26:35.379163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/__init__.pyi
+-rw-r--r--   0        0        0     4381 2022-04-05 08:26:35.375163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/abc.pyi
+-rw-r--r--   0        0        0     4652 2022-04-05 08:26:35.375163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/machinery.pyi
+-rw-r--r--   0        0        0     3743 2022-04-05 08:26:35.379163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/metadata.pyi
+-rw-r--r--   0        0        0     1176 2022-04-05 08:26:35.375163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/resources.pyi
+-rw-r--r--   0        0        0     1762 2022-04-05 08:26:35.375163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/util.pyi
+-rw-r--r--   0        0        0    11110 2022-04-05 08:26:35.335163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/inspect.pyi
+-rw-r--r--   0        0        0     7558 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/io.pyi
+-rw-r--r--   0        0        0     5252 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ipaddress.pyi
+-rw-r--r--   0        0        0     7901 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/itertools.pyi
+-rw-r--r--   0        0        0     1977 2022-04-05 08:26:35.379163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/json/__init__.pyi
+-rw-r--r--   0        0        0     1090 2022-04-05 08:26:35.379163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/json/decoder.pyi
+-rw-r--r--   0        0        0      779 2022-04-05 08:26:35.379163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/json/encoder.pyi
+-rw-r--r--   0        0        0       24 2022-04-05 08:26:35.379163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/json/tool.pyi
+-rw-r--r--   0        0        0      210 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/keyword.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/__init__.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/__init__.pyi
+-rw-r--r--   0        0        0      956 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/driver.pyi
+-rw-r--r--   0        0        0      733 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/grammar.pyi
+-rw-r--r--   0        0        0      172 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/literals.pyi
+-rw-r--r--   0        0        0     1107 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/parse.pyi
+-rw-r--r--   0        0        0     2140 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/pgen.pyi
+-rw-r--r--   0        0        0     1065 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/token.pyi
+-rw-r--r--   0        0        0      883 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/tokenize.pyi
+-rw-r--r--   0        0        0     2208 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pygram.pyi
+-rw-r--r--   0        0        0     3322 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pytree.pyi
+-rw-r--r--   0        0        0      591 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/linecache.pyi
+-rw-r--r--   0        0        0     2557 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/locale.pyi
+-rw-r--r--   0        0        0    24560 2022-04-05 08:26:35.415163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/logging/__init__.pyi
+-rw-r--r--   0        0        0     1218 2022-04-05 08:26:35.415163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/logging/config.pyi
+-rw-r--r--   0        0        0     9986 2022-04-05 08:26:35.415163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/logging/handlers.pyi
+-rw-r--r--   0        0        0     4587 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lzma.pyi
+-rw-r--r--   0        0        0     3190 2022-04-05 08:26:35.319163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/macpath.pyi
+-rw-r--r--   0        0        0      172 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/macurl2path.pyi
+-rw-r--r--   0        0        0     8112 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/mailbox.pyi
+-rw-r--r--   0        0        0      330 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/mailcap.pyi
+-rw-r--r--   0        0        0      253 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/marshal.pyi
+-rw-r--r--   0        0        0     3835 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/math.pyi
+-rw-r--r--   0        0        0     1637 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/mimetypes.pyi
+-rw-r--r--   0        0        0     4570 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/mmap.pyi
+-rw-r--r--   0        0        0     3674 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/modulefinder.pyi
+-rw-r--r--   0        0        0     6306 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/msilib/__init__.pyi
+-rw-r--r--   0        0        0     2214 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/msilib/schema.pyi
+-rw-r--r--   0        0        0      356 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/msilib/sequence.pyi
+-rw-r--r--   0        0        0      202 2022-04-05 08:26:35.387163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/msilib/text.pyi
+-rw-r--r--   0        0        0      795 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/msvcrt.pyi
+-rw-r--r--   0        0        0     3553 2022-04-05 08:26:35.415163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/__init__.pyi
+-rw-r--r--   0        0        0     2602 2022-04-05 08:26:35.415163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/connection.pyi
+-rw-r--r--   0        0        0     7475 2022-04-05 08:26:35.415163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/context.pyi
+-rw-r--r--   0        0        0     1572 2022-04-05 08:26:35.415163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/dummy/__init__.pyi
+-rw-r--r--   0        0        0     1431 2022-04-05 08:26:35.415163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/dummy/connection.pyi
+-rw-r--r--   0        0        0     4850 2022-04-05 08:26:35.415163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/managers.pyi
+-rw-r--r--   0        0        0     3534 2022-04-05 08:26:35.415163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/pool.pyi
+-rw-r--r--   0        0        0     1143 2022-04-05 08:26:35.415163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/process.pyi
+-rw-r--r--   0        0        0     1288 2022-04-05 08:26:35.415163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/queues.pyi
+-rw-r--r--   0        0        0     1302 2022-04-05 08:26:35.415163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/shared_memory.pyi
+-rw-r--r--   0        0        0     3941 2022-04-05 08:26:35.415163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/sharedctypes.pyi
+-rw-r--r--   0        0        0      690 2022-04-05 08:26:35.415163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/spawn.pyi
+-rw-r--r--   0        0        0     1799 2022-04-05 08:26:35.415163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/synchronize.pyi
+-rw-r--r--   0        0        0      598 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/netrc.pyi
+-rw-r--r--   0        0        0      322 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/nis.pyi
+-rw-r--r--   0        0        0     4321 2022-04-05 08:26:35.303163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/nntplib.pyi
+-rw-r--r--   0        0        0     1936 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ntpath.pyi
+-rw-r--r--   0        0        0       76 2022-04-05 08:26:35.319163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/nturl2path.pyi
+-rw-r--r--   0        0        0     4335 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/numbers.pyi
+-rw-r--r--   0        0        0      609 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/opcode.pyi
+-rw-r--r--   0        0        0     8146 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/operator.pyi
+-rw-r--r--   0        0        0    10261 2022-04-05 08:26:35.303163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/optparse.pyi
+-rw-r--r--   0        0        0    30354 2022-04-05 08:26:35.379163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/os/__init__.pyi
+-rw-r--r--   0        0        0       99 2022-04-05 08:26:35.379163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/os/path.pyi
+-rw-r--r--   0        0        0     3065 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ossaudiodev.pyi
+-rw-r--r--   0        0        0      966 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/parser.pyi
+-rw-r--r--   0        0        0     6650 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pathlib.pyi
+-rw-r--r--   0        0        0    10325 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pdb.pyi
+-rw-r--r--   0        0        0     5322 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pickle.pyi
+-rw-r--r--   0        0        0     4510 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pickletools.pyi
+-rw-r--r--   0        0        0      514 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pipes.pyi
+-rw-r--r--   0        0        0     1629 2022-04-05 08:26:35.319163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pkgutil.pyi
+-rw-r--r--   0        0        0     2272 2022-04-05 08:26:35.303163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/platform.pyi
+-rw-r--r--   0        0        0     2742 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/plistlib.pyi
+-rw-r--r--   0        0        0     2500 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/poplib.pyi
+-rw-r--r--   0        0        0     3006 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/posix.pyi
+-rw-r--r--   0        0        0     2822 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/posixpath.pyi
+-rw-r--r--   0        0        0     4231 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pprint.pyi
+-rw-r--r--   0        0        0     1344 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/profile.pyi
+-rw-r--r--   0        0        0     2213 2022-04-05 08:26:35.319163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pstats.pyi
+-rw-r--r--   0        0        0      592 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pty.pyi
+-rw-r--r--   0        0        0      354 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pwd.pyi
+-rw-r--r--   0        0        0     1646 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/py_compile.pyi
+-rw-r--r--   0        0        0     1192 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pyclbr.pyi
+-rw-r--r--   0        0        0    10660 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pydoc.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.415163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pydoc_data/__init__.pyi
+-rw-r--r--   0        0        0       48 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pydoc_data/topics.pyi
+-rw-r--r--   0        0        0     3414 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pyexpat/__init__.pyi
+-rw-r--r--   0        0        0     1275 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pyexpat/errors.pyi
+-rw-r--r--   0        0        0      205 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pyexpat/model.pyi
+-rw-r--r--   0        0        0     1884 2022-04-05 08:26:35.303163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/queue.pyi
+-rw-r--r--   0        0        0      343 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/quopri.pyi
+-rw-r--r--   0        0        0     4018 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/random.pyi
+-rw-r--r--   0        0        0     4378 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/re.pyi
+-rw-r--r--   0        0        0     1709 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/readline.pyi
+-rw-r--r--   0        0        0     1228 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/reprlib.pyi
+-rw-r--r--   0        0        0     1445 2022-04-05 08:26:35.319163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/resource.pyi
+-rw-r--r--   0        0        0      308 2022-04-05 08:26:35.335163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/rlcompleter.pyi
+-rw-r--r--   0        0        0      776 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/runpy.pyi
+-rw-r--r--   0        0        0     1497 2022-04-05 08:26:35.319163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sched.pyi
+-rw-r--r--   0        0        0      467 2022-04-05 08:26:35.319163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/secrets.pyi
+-rw-r--r--   0        0        0     4828 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/select.pyi
+-rw-r--r--   0        0        0     3673 2022-04-05 08:26:35.335163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/selectors.pyi
+-rw-r--r--   0        0        0     1613 2022-04-05 08:26:35.335163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/shelve.pyi
+-rw-r--r--   0        0        0     1354 2022-04-05 08:26:35.319163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/shlex.pyi
+-rw-r--r--   0        0        0     6004 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/shutil.pyi
+-rw-r--r--   0        0        0     5279 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/signal.pyi
+-rw-r--r--   0        0        0      406 2022-04-05 08:26:35.335163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/site.pyi
+-rw-r--r--   0        0        0     3282 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/smtpd.pyi
+-rw-r--r--   0        0        0     5608 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/smtplib.pyi
+-rw-r--r--   0        0        0      501 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sndhdr.pyi
+-rw-r--r--   0        0        0    22875 2022-04-05 08:26:35.319163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/socket.pyi
+-rw-r--r--   0        0        0     5134 2022-04-05 08:26:35.303163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/socketserver.pyi
+-rw-r--r--   0        0        0      311 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/spwd.pyi
+-rw-r--r--   0        0        0       43 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sqlite3/__init__.pyi
+-rw-r--r--   0        0        0    11447 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sqlite3/dbapi2.pyi
+-rw-r--r--   0        0        0     1073 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sre_compile.pyi
+-rw-r--r--   0        0        0     3460 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sre_constants.pyi
+-rw-r--r--   0        0        0     3820 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sre_parse.pyi
+-rw-r--r--   0        0        0    16955 2022-04-05 08:26:35.335163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ssl.pyi
+-rw-r--r--   0        0        0     1805 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/stat.pyi
+-rw-r--r--   0        0        0     3798 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/statistics.pyi
+-rw-r--r--   0        0        0     1423 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/string.pyi
+-rw-r--r--   0        0        0      817 2022-04-05 08:26:35.303163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/stringprep.pyi
+-rw-r--r--   0        0        0     1573 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/struct.pyi
+-rw-r--r--   0        0        0    34838 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/subprocess.pyi
+-rw-r--r--   0        0        0     2924 2022-04-05 08:26:35.335163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sunau.pyi
+-rw-r--r--   0        0        0     1383 2022-04-05 08:26:35.303163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/symbol.pyi
+-rw-r--r--   0        0        0     2051 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/symtable.pyi
+-rw-r--r--   0        0        0     6810 2022-04-05 08:26:35.335163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sys.pyi
+-rw-r--r--   0        0        0      871 2022-04-05 08:26:35.319163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sysconfig.pyi
+-rw-r--r--   0        0        0      821 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/syslog.pyi
+-rw-r--r--   0        0        0      447 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tabnanny.pyi
+-rw-r--r--   0        0        0    11588 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tarfile.pyi
+-rw-r--r--   0        0        0     2728 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/telnetlib.pyi
+-rw-r--r--   0        0        0    12993 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tempfile.pyi
+-rw-r--r--   0        0        0     3526 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/termios.pyi
+-rw-r--r--   0        0        0     3234 2022-04-05 08:26:35.319163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/textwrap.pyi
+-rw-r--r--   0        0        0       50 2022-04-05 08:26:35.335163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/this.pyi
+-rw-r--r--   0        0        0     6460 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/threading.pyi
+-rw-r--r--   0        0        0     4063 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/time.pyi
+-rw-r--r--   0        0        0     1731 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/timeit.pyi
+-rw-r--r--   0        0        0   118206 2022-04-05 08:26:35.403163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/__init__.pyi
+-rw-r--r--   0        0        0      299 2022-04-05 08:26:35.403163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/colorchooser.pyi
+-rw-r--r--   0        0        0      297 2022-04-05 08:26:35.403163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/commondialog.pyi
+-rw-r--r--   0        0        0     1886 2022-04-05 08:26:35.403163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/constants.pyi
+-rw-r--r--   0        0        0      291 2022-04-05 08:26:35.403163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/dialog.pyi
+-rw-r--r--   0        0        0      568 2022-04-05 08:26:35.403163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/dnd.pyi
+-rw-r--r--   0        0        0     2287 2022-04-05 08:26:35.403163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/filedialog.pyi
+-rw-r--r--   0        0        0     3840 2022-04-05 08:26:35.403163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/font.pyi
+-rw-r--r--   0        0        0     1170 2022-04-05 08:26:35.403163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/messagebox.pyi
+-rw-r--r--   0        0        0      333 2022-04-05 08:26:35.403163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/scrolledtext.pyi
+-rw-r--r--   0        0        0      990 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/simpledialog.pyi
+-rw-r--r--   0        0        0    14945 2022-04-05 08:26:35.403163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/tix.pyi
+-rw-r--r--   0        0        0    38044 2022-04-05 08:26:35.403163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/ttk.pyi
+-rw-r--r--   0        0        0     1468 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/token.pyi
+-rw-r--r--   0        0        0     3110 2022-04-05 08:26:35.303163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tokenize.pyi
+-rw-r--r--   0        0        0     2457 2022-04-05 08:26:35.319163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/trace.pyi
+-rw-r--r--   0        0        0     7350 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/traceback.pyi
+-rw-r--r--   0        0        0     2795 2022-04-05 08:26:35.335163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tracemalloc.pyi
+-rw-r--r--   0        0        0      275 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tty.pyi
+-rw-r--r--   0        0        0    19727 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/turtle.pyi
+-rw-r--r--   0        0        0    11394 2022-04-05 08:26:35.303163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/types.pyi
+-rw-r--r--   0        0        0    25751 2022-04-05 08:26:35.319163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/typing.pyi
+-rw-r--r--   0        0        0     4039 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/typing_extensions.pyi
+-rw-r--r--   0        0        0     1794 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unicodedata.pyi
+-rw-r--r--   0        0        0      689 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/__init__.pyi
+-rw-r--r--   0        0        0      372 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/async_case.pyi
+-rw-r--r--   0        0        0    12439 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/case.pyi
+-rw-r--r--   0        0        0     2067 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/loader.pyi
+-rw-r--r--   0        0        0     1691 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/main.pyi
+-rw-r--r--   0        0        0    13313 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/mock.pyi
+-rw-r--r--   0        0        0     1859 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/result.pyi
+-rw-r--r--   0        0        0     1339 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/runner.pyi
+-rw-r--r--   0        0        0      402 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/signals.pyi
+-rw-r--r--   0        0        0      892 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/suite.pyi
+-rw-r--r--   0        0        0      906 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/util.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/__init__.pyi
+-rw-r--r--   0        0        0      643 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/error.pyi
+-rw-r--r--   0        0        0     5009 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/parse.pyi
+-rw-r--r--   0        0        0    16281 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/request.pyi
+-rw-r--r--   0        0        0     2107 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/response.pyi
+-rw-r--r--   0        0        0      703 2022-04-05 08:26:35.411163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/robotparser.pyi
+-rw-r--r--   0        0        0      549 2022-04-05 08:26:35.303163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/uu.pyi
+-rw-r--r--   0        0        0     3448 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/uuid.pyi
+-rw-r--r--   0        0        0     2459 2022-04-05 08:26:35.379163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/venv/__init__.pyi
+-rw-r--r--   0        0        0     2583 2022-04-05 08:26:35.311163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/warnings.pyi
+-rw-r--r--   0        0        0     2653 2022-04-05 08:26:35.307163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wave.pyi
+-rw-r--r--   0        0        0     4545 2022-04-05 08:26:35.319163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/weakref.pyi
+-rw-r--r--   0        0        0     3253 2022-04-05 08:26:35.323163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/webbrowser.pyi
+-rw-r--r--   0        0        0     3729 2022-04-05 08:26:35.327163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/winreg.pyi
+-rw-r--r--   0        0        0      811 2022-04-05 08:26:35.335163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/winsound.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/__init__.pyi
+-rw-r--r--   0        0        0     3125 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/handlers.pyi
+-rw-r--r--   0        0        0     1250 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/headers.pyi
+-rw-r--r--   0        0        0     1532 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/simple_server.pyi
+-rw-r--r--   0        0        0       71 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/types.pyi
+-rw-r--r--   0        0        0      896 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/util.pyi
+-rw-r--r--   0        0        0     1867 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/validate.pyi
+-rw-r--r--   0        0        0     2315 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xdrlib.pyi
+-rw-r--r--   0        0        0       30 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/__init__.pyi
+-rw-r--r--   0        0        0      457 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/NodeFilter.pyi
+-rw-r--r--   0        0        0     1844 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/__init__.pyi
+-rw-r--r--   0        0        0      457 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/domreg.pyi
+-rw-r--r--   0        0        0       77 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/expatbuilder.pyi
+-rw-r--r--   0        0        0      530 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/minicompat.pyi
+-rw-r--r--   0        0        0    11040 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/minidom.pyi
+-rw-r--r--   0        0        0       77 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/pulldom.pyi
+-rw-r--r--   0        0        0      173 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/xmlbuilder.pyi
+-rw-r--r--   0        0        0      873 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/ElementInclude.pyi
+-rw-r--r--   0        0        0     1588 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/ElementPath.pyi
+-rw-r--r--   0        0        0    15071 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/ElementTree.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/__init__.pyi
+-rw-r--r--   0        0        0       50 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/cElementTree.pyi
+-rw-r--r--   0        0        0       34 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/parsers/__init__.pyi
+-rw-r--r--   0        0        0       22 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/parsers/expat/__init__.pyi
+-rw-r--r--   0        0        0       29 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/parsers/expat/errors.pyi
+-rw-r--r--   0        0        0       28 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/parsers/expat/model.pyi
+-rw-r--r--   0        0        0     1389 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/__init__.pyi
+-rw-r--r--   0        0        0     1391 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/handler.pyi
+-rw-r--r--   0        0        0     2825 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/saxutils.pyi
+-rw-r--r--   0        0        0     2444 2022-04-05 08:26:35.395163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/xmlreader.pyi
+-rw-r--r--   0        0        0        0 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xmlrpc/__init__.pyi
+-rw-r--r--   0        0        0    12367 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xmlrpc/client.pyi
+-rw-r--r--   0        0        0     6835 2022-04-05 08:26:35.391163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xmlrpc/server.pyi
+-rw-r--r--   0        0        0      294 2022-04-05 08:26:35.319163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xxlimited.pyi
+-rw-r--r--   0        0        0      678 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/zipapp.pyi
+-rw-r--r--   0        0        0     7659 2022-04-05 08:26:35.315163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/zipfile.pyi
+-rw-r--r--   0        0        0     1244 2022-04-05 08:26:35.303163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/zipimport.pyi
+-rw-r--r--   0        0        0     1777 2022-04-05 08:26:35.331163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/zlib.pyi
+-rw-r--r--   0        0        0     1183 2022-04-05 08:26:35.407163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/zoneinfo/__init__.pyi
+-rw-r--r--   0        0        0     2216 2022-04-05 08:26:35.415163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stubs/mypy-extensions/mypy_extensions.pyi
+-rw-r--r--   0        0        0     4831 2022-04-05 08:26:35.455163 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypyc/test-data/fixtures/typing-full.pyi
+-rw-r--r--   0        0        0      341 2022-04-05 08:26:32.939168 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/py/__init__.pyi
+-rw-r--r--   0        0        0     1205 2022-04-05 08:26:32.975168 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/py/_vendored_packages/iniconfig/__init__.pyi
+-rw-r--r--   0        0        0     3409 2022-04-05 08:26:32.939168 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/py/error.pyi
+-rw-r--r--   0        0        0     1205 2022-04-05 08:26:32.939168 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/py/iniconfig.pyi
+-rw-r--r--   0        0        0     5277 2022-04-05 08:26:32.943168 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/py/io.pyi
+-rw-r--r--   0        0        0     7168 2022-04-05 08:26:32.943168 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/py/path.pyi
+-rw-r--r--   0        0        0      787 2022-04-05 08:26:32.943168 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/py/xml.pyi
+-rw-r--r--   0        0        0     1762 2022-04-12 13:55:32.354372 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/pytz-stubs/__init__.pyi
+-rw-r--r--   0        0        0      312 2022-04-12 13:55:32.354372 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/pytz-stubs/exceptions.pyi
+-rw-r--r--   0        0        0     2219 2022-04-12 13:55:32.354372 nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/pytz-stubs/tzinfo.pyi
+-rw-r--r--   0        0        0     1745 2022-04-05 09:39:19.126134 nwon_baseline-0.2.1/README.md
+-rw-r--r--   0        0        0        0 2022-03-30 13:01:02.168845 nwon_baseline-0.2.1/nwon_baseline/__init__.py
+-rw-r--r--   0        0        0      431 2022-04-12 14:14:45.868752 nwon_baseline-0.2.1/nwon_baseline/date_helper/__init__.py
+-rw-r--r--   0        0        0      726 2022-06-21 09:50:39.516257 nwon_baseline-0.2.1/nwon_baseline/date_helper/country.py
+-rw-r--r--   0        0        0      529 2022-04-12 14:03:37.577729 nwon_baseline-0.2.1/nwon_baseline/date_helper/datetime.py
+-rw-r--r--   0        0        0      514 2022-04-12 14:03:47.313716 nwon_baseline-0.2.1/nwon_baseline/date_helper/time_differences.py
+-rw-r--r--   0        0        0      604 2023-06-19 10:24:00.138663 nwon_baseline-0.2.1/nwon_baseline/directory_helper/__init__.py
+-rw-r--r--   0        0        0     2212 2022-04-12 08:40:56.233856 nwon_baseline-0.2.1/nwon_baseline/directory_helper/directory_content.py
+-rw-r--r--   0        0        0      991 2023-06-19 10:24:12.394682 nwon_baseline-0.2.1/nwon_baseline/directory_helper/directory_interactions.py
+-rw-r--r--   0        0        0      531 2022-05-12 07:08:30.597454 nwon_baseline-0.2.1/nwon_baseline/file_helper/__init__.py
+-rw-r--r--   0        0        0     1452 2022-04-07 13:42:29.856122 nwon_baseline-0.2.1/nwon_baseline/file_helper/file.py
+-rw-r--r--   0        0        0      718 2022-05-12 07:08:33.205452 nwon_baseline-0.2.1/nwon_baseline/file_helper/filename_from_url.py
+-rw-r--r--   0        0        0      232 2022-04-05 08:48:23.005685 nwon_baseline-0.2.1/nwon_baseline/image_helper/__init__.py
+-rw-r--r--   0        0        0      640 2022-04-04 06:36:54.202585 nwon_baseline-0.2.1/nwon_baseline/image_helper/image.py
+-rw-r--r--   0        0        0      116 2022-04-05 08:47:47.541699 nwon_baseline-0.2.1/nwon_baseline/import_helper/__init__.py
+-rw-r--r--   0        0        0     2026 2022-04-04 06:36:54.194585 nwon_baseline-0.2.1/nwon_baseline/import_helper/import_from_file.py
+-rw-r--r--   0        0        0      224 2022-04-05 08:47:02.149711 nwon_baseline-0.2.1/nwon_baseline/poetry/__init__.py
+-rw-r--r--   0        0        0      644 2022-04-04 06:36:54.194585 nwon_baseline-0.2.1/nwon_baseline/poetry/checking_version_argument.py
+-rw-r--r--   0        0        0     1002 2022-04-04 06:36:54.194585 nwon_baseline-0.2.1/nwon_baseline/poetry/package_version.py
+-rw-r--r--   0        0        0      463 2022-06-23 08:01:15.992282 nwon_baseline-0.2.1/nwon_baseline/print_helper/__init__.py
+-rw-r--r--   0        0        0      570 2022-06-23 08:00:40.928324 nwon_baseline-0.2.1/nwon_baseline/print_helper/colored_printing.py
+-rw-r--r--   0        0        0      490 2022-06-23 08:06:42.895903 nwon_baseline-0.2.1/nwon_baseline/print_helper/print_with_style.py
+-rw-r--r--   0        0        0        0 2022-04-05 08:00:37.317785 nwon_baseline-0.2.1/nwon_baseline/py.typed
+-rw-r--r--   0        0        0      403 2022-05-23 11:12:00.460291 nwon_baseline-0.2.1/nwon_baseline/pydantic/__init__.py
+-rw-r--r--   0        0        0      667 2022-04-27 13:35:06.007169 nwon_baseline-0.2.1/nwon_baseline/pydantic/path_to_write_pydantic_model.py
+-rw-r--r--   0        0        0      221 2022-05-23 11:10:23.684409 nwon_baseline-0.2.1/nwon_baseline/pydantic/pydantic_model_to_dict.py
+-rw-r--r--   0        0        0      623 2022-04-27 13:35:38.467129 nwon_baseline-0.2.1/nwon_baseline/pydantic/save_pydantic_model_instance.py
+-rw-r--r--   0        0        0      654 2022-04-27 13:35:16.363156 nwon_baseline-0.2.1/nwon_baseline/pydantic/save_pydantic_model_schema.py
+-rw-r--r--   0        0        0      288 2022-06-15 11:29:44.664464 nwon_baseline-0.2.1/nwon_baseline/shell_helper/__init__.py
+-rw-r--r--   0        0        0      645 2022-03-29 12:19:02.136741 nwon_baseline-0.2.1/nwon_baseline/shell_helper/execute_command.py
+-rw-r--r--   0        0        0     1106 2022-09-02 13:00:03.416942 nwon_baseline-0.2.1/nwon_baseline/shell_helper/get_environment_variable.py
+-rw-r--r--   0        0        0      274 2022-04-05 08:50:03.033631 nwon_baseline-0.2.1/nwon_baseline/type_helper/__init__.py
+-rw-r--r--   0        0        0      476 2022-04-25 13:57:42.090917 nwon_baseline-0.2.1/nwon_baseline/type_helper/enum_type_guard.py
+-rw-r--r--   0        0        0      557 2022-04-01 13:03:10.337749 nwon_baseline-0.2.1/nwon_baseline/type_helper/enum_value_list.py
+-rw-r--r--   0        0        0      612 2022-04-25 14:00:15.618795 nwon_baseline-0.2.1/nwon_baseline/typings/__init__.py
+-rw-r--r--   0        0        0       78 2022-04-25 14:03:36.534617 nwon_baseline-0.2.1/nwon_baseline/typings/any_dict.py
+-rw-r--r--   0        0        0      242 2022-03-29 11:55:17.603051 nwon_baseline-0.2.1/nwon_baseline/typings/bounding_box.py
+-rw-r--r--   0        0        0       63 2022-03-31 06:53:03.720819 nwon_baseline-0.2.1/nwon_baseline/typings/celery_return.py
+-rw-r--r--   0        0        0      135 2022-03-29 09:54:50.423452 nwon_baseline-0.2.1/nwon_baseline/typings/request_body_format.py
+-rw-r--r--   0        0        0      349 2022-03-31 07:14:17.268870 nwon_baseline-0.2.1/nwon_baseline/typings/terminal_colors.py
+-rw-r--r--   0        0        0      141 2022-03-29 12:01:55.262340 nwon_baseline-0.2.1/nwon_baseline/typings/version_change.py
+-rw-r--r--   0        0        0     1051 2023-06-19 10:24:26.386703 nwon_baseline-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2529 1970-01-01 00:00:00.000000 nwon_baseline-0.2.1/PKG-INFO
```

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/attr/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/attr/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/attr/exceptions.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/attr/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/attr/setters.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/attr/setters.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/attr/validators.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/attr/validators.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/attrs/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/attrs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/humps/main.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/humps/main.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/iniconfig/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/iniconfig/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/BaseHTTPServer.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/BaseHTTPServer.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ConfigParser.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ConfigParser.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/Cookie.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/Cookie.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/HTMLParser.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/HTMLParser.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/Queue.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/Queue.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/SimpleHTTPServer.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/SimpleHTTPServer.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/SocketServer.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/SocketServer.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/StringIO.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/StringIO.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/UserDict.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/UserDict.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/UserList.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/UserList.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/UserString.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/UserString.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/__builtin__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/__builtin__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_ast.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_ast.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_collections.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_collections.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_functools.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_functools.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_hotshot.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_hotshot.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_io.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_io.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_sha256.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_sha256.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_sha512.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_sha512.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_socket.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_socket.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_sre.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_sre.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_struct.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_struct.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_symtable.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_symtable.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_winreg.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/_winreg.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/abc.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/abc.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ast.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ast.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/builtins.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/builtins.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cPickle.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cPickle.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cStringIO.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cStringIO.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cgi.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cgi.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/collections.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/collections.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/compileall.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/compileall.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cookielib.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/cookielib.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/copy_reg.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/copy_reg.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/ccompiler.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/ccompiler.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/cmd.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/cmd.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/config.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/command/config.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/config.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/config.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/core.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/core.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/dir_util.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/dir_util.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/errors.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/errors.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/extension.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/extension.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/fancy_getopt.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/fancy_getopt.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/log.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/log.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/sysconfig.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/sysconfig.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/text_file.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/text_file.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/util.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/util.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/version.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/distutils/version.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/dummy_thread.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/dummy_thread.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/_parseaddr.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/_parseaddr.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/charset.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/charset.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/feedparser.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/feedparser.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/message.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/message.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/utils.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/email/utils.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/encodings/utf_8.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/encodings/utf_8.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/exceptions.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/fcntl.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/fcntl.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/functools.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/functools.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/gc.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/gc.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/gettext.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/gettext.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/gzip.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/gzip.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/hashlib.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/hashlib.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/heapq.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/heapq.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/httplib.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/httplib.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/imp.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/imp.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/inspect.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/inspect.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/io.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/io.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/itertools.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/itertools.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/json.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/json.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/logging/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/logging/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/logging/handlers.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/logging/handlers.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/mimetools.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/mimetools.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/dummy/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/dummy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/dummy/connection.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/dummy/connection.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/pool.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/pool.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/process.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/process.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/util.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/multiprocessing/util.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ntpath.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/ntpath.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/os/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/os/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/os/path.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/os/path.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/os2emxpath.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/os2emxpath.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/platform.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/platform.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/popen2.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/popen2.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/posix.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/posix.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/posixpath.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/posixpath.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/random.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/random.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/re.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/re.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/repr.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/repr.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/resource.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/resource.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/rfc822.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/rfc822.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/runpy.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/runpy.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sets.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sets.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/shelve.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/shelve.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/shlex.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/shlex.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/signal.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/signal.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/smtplib.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/smtplib.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sre_constants.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sre_constants.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sre_parse.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sre_parse.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/stat.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/stat.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/string.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/string.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/stringold.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/stringold.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/strop.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/strop.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/subprocess.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/subprocess.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/symbol.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/symbol.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sys.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/sys.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/tempfile.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/tempfile.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/textwrap.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/textwrap.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/thread.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/thread.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/tokenize.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/tokenize.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/types.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/types.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/typing.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/typing.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/unittest.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/unittest.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/urllib.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/urllib.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/urllib2.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/urllib2.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/urlparse.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/urlparse.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xmlrpclib.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/@python2/xmlrpclib.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/__future__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/__future__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_ast.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_ast.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_bisect.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_bisect.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_codecs.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_codecs.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_collections_abc.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_collections_abc.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_compression.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_compression.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_csv.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_csv.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_curses.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_curses.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_dummy_thread.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_dummy_thread.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_dummy_threading.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_dummy_threading.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_heapq.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_heapq.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_imp.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_imp.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_json.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_json.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_msi.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_msi.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_operator.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_operator.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_osx_support.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_osx_support.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_posixsubprocess.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_posixsubprocess.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_sitebuiltins.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_sitebuiltins.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_stat.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_stat.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_thread.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_thread.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_tkinter.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_tkinter.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_tracemalloc.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_tracemalloc.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_typeshed/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_typeshed/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_typeshed/wsgi.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_typeshed/wsgi.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_typeshed/xml.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_typeshed/xml.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_warnings.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_warnings.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_weakref.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_weakref.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_weakrefset.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_weakrefset.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_winapi.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/_winapi.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/abc.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/abc.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/aifc.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/aifc.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/argparse.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/argparse.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/array.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/array.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ast.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ast.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asynchat.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asynchat.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/base_events.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/base_events.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/base_futures.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/base_futures.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/base_subprocess.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/base_subprocess.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/events.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/events.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/exceptions.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/exceptions.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/format_helpers.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/format_helpers.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/futures.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/futures.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/locks.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/locks.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/proactor_events.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/proactor_events.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/protocols.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/protocols.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/queues.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/queues.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/sslproto.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/sslproto.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/streams.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/streams.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/subprocess.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/subprocess.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/tasks.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/tasks.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/transports.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/transports.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/trsock.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/trsock.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/unix_events.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/unix_events.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/windows_events.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/windows_events.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/windows_utils.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncio/windows_utils.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncore.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/asyncore.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/audioop.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/audioop.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/base64.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/base64.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/bdb.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/bdb.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/binascii.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/binascii.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/binhex.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/binhex.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/builtins.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/builtins.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/bz2.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/bz2.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/cProfile.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/cProfile.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/calendar.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/calendar.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/cgi.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/cgi.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/cgitb.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/cgitb.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/chunk.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/chunk.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/cmath.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/cmath.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/cmd.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/cmd.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/code.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/code.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/codecs.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/codecs.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/collections/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/collections/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/colorsys.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/colorsys.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/compileall.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/compileall.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/_base.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/_base.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/process.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/process.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/thread.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/concurrent/futures/thread.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/configparser.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/configparser.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/contextlib.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/contextlib.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/contextvars.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/contextvars.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/copyreg.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/copyreg.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/crypt.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/crypt.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/csv.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/csv.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ctypes/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ctypes/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ctypes/wintypes.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ctypes/wintypes.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/curses/ascii.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/curses/ascii.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/curses/panel.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/curses/panel.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dataclasses.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dataclasses.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/datetime.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/datetime.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/dumb.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/dumb.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/gnu.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/gnu.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/ndbm.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dbm/ndbm.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/decimal.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/decimal.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/difflib.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/difflib.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dis.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/dis.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/archive_util.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/archive_util.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/ccompiler.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/ccompiler.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/cmd.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/cmd.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/config.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/command/config.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/config.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/config.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/core.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/core.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/dir_util.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/dir_util.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/dist.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/dist.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/errors.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/errors.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/extension.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/extension.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/fancy_getopt.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/fancy_getopt.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/filelist.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/filelist.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/log.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/log.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/sysconfig.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/sysconfig.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/text_file.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/text_file.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/util.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/util.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/version.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/distutils/version.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/doctest.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/doctest.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/_header_value_parser.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/_header_value_parser.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/charset.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/charset.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/errors.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/errors.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/feedparser.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/feedparser.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/generator.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/generator.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/header.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/header.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/headerregistry.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/headerregistry.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/message.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/message.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/parser.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/parser.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/policy.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/policy.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/utils.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/email/utils.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/encodings/utf_8.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/encodings/utf_8.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ensurepip/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ensurepip/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/enum.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/enum.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/errno.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/errno.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/faulthandler.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/faulthandler.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/fcntl.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/fcntl.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/filecmp.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/filecmp.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/fileinput.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/fileinput.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/formatter.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/formatter.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/fractions.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/fractions.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ftplib.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ftplib.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/functools.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/functools.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/gc.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/gc.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/genericpath.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/genericpath.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/gettext.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/gettext.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/glob.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/glob.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/graphlib.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/graphlib.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/gzip.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/gzip.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/hashlib.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/hashlib.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/heapq.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/heapq.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/hmac.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/hmac.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/html/parser.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/html/parser.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/client.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/client.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/cookiejar.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/cookiejar.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/cookies.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/cookies.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/server.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/http/server.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/imaplib.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/imaplib.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/imghdr.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/imghdr.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/imp.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/imp.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/abc.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/abc.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/machinery.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/machinery.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/metadata.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/metadata.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/resources.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/resources.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/util.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/importlib/util.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/inspect.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/inspect.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/io.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/io.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ipaddress.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ipaddress.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/itertools.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/itertools.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/json/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/json/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/json/decoder.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/json/decoder.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/json/encoder.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/json/encoder.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/driver.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/driver.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/grammar.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/grammar.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/parse.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/parse.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/pgen.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/pgen.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/token.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/token.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/tokenize.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pgen2/tokenize.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pygram.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pygram.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pytree.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lib2to3/pytree.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/linecache.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/linecache.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/locale.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/locale.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/logging/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/logging/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/logging/config.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/logging/config.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/logging/handlers.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/logging/handlers.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lzma.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/lzma.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/macpath.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/macpath.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/mailbox.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/mailbox.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/math.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/math.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/mimetypes.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/mimetypes.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/mmap.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/mmap.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/modulefinder.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/modulefinder.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/msilib/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/msilib/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/msilib/schema.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/msilib/schema.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/msvcrt.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/msvcrt.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/connection.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/connection.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/context.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/context.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/dummy/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/dummy/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/dummy/connection.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/dummy/connection.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/managers.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/managers.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/pool.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/pool.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/process.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/process.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/queues.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/queues.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/shared_memory.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/shared_memory.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/sharedctypes.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/sharedctypes.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/spawn.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/spawn.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/synchronize.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/multiprocessing/synchronize.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/netrc.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/netrc.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/nntplib.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/nntplib.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ntpath.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ntpath.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/numbers.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/numbers.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/opcode.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/opcode.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/operator.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/operator.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/optparse.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/optparse.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/os/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/os/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ossaudiodev.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ossaudiodev.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/parser.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/parser.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pathlib.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pathlib.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pdb.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pdb.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pickle.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pickle.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pickletools.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pickletools.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pipes.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pipes.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pkgutil.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pkgutil.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/platform.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/platform.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/plistlib.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/plistlib.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/poplib.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/poplib.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/posix.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/posix.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/posixpath.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/posixpath.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pprint.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pprint.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/profile.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/profile.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pstats.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pstats.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pty.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pty.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/py_compile.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/py_compile.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pyclbr.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pyclbr.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pydoc.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pydoc.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pyexpat/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pyexpat/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pyexpat/errors.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/pyexpat/errors.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/queue.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/queue.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/random.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/random.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/re.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/re.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/readline.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/readline.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/reprlib.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/reprlib.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/resource.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/resource.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/runpy.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/runpy.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sched.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sched.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/select.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/select.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/selectors.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/selectors.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/shelve.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/shelve.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/shlex.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/shlex.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/shutil.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/shutil.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/signal.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/signal.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/smtpd.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/smtpd.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/smtplib.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/smtplib.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/socket.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/socket.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/socketserver.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/socketserver.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sqlite3/dbapi2.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sqlite3/dbapi2.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sre_compile.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sre_compile.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sre_constants.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sre_constants.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sre_parse.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sre_parse.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ssl.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/ssl.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/stat.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/stat.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/statistics.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/statistics.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/string.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/string.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/stringprep.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/stringprep.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/struct.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/struct.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/subprocess.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/subprocess.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sunau.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sunau.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/symbol.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/symbol.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/symtable.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/symtable.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sys.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sys.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sysconfig.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/sysconfig.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/syslog.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/syslog.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tarfile.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tarfile.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/telnetlib.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/telnetlib.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tempfile.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tempfile.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/termios.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/termios.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/textwrap.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/textwrap.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/threading.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/threading.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/time.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/time.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/timeit.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/timeit.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/constants.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/constants.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/dnd.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/dnd.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/filedialog.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/filedialog.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/font.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/font.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/messagebox.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/messagebox.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/simpledialog.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/simpledialog.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/tix.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/tix.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/ttk.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tkinter/ttk.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/token.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/token.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tokenize.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tokenize.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/trace.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/trace.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/traceback.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/traceback.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tracemalloc.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/tracemalloc.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/turtle.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/turtle.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/types.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/types.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/typing.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/typing.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/typing_extensions.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/typing_extensions.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unicodedata.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unicodedata.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/case.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/case.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/loader.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/loader.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/main.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/main.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/mock.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/mock.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/result.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/result.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/runner.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/runner.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/suite.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/suite.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/util.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/unittest/util.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/error.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/error.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/parse.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/parse.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/request.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/request.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/response.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/response.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/robotparser.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/urllib/robotparser.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/uu.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/uu.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/uuid.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/uuid.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/venv/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/venv/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/warnings.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/warnings.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wave.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wave.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/weakref.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/weakref.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/webbrowser.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/webbrowser.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/winreg.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/winreg.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/winsound.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/winsound.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/handlers.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/handlers.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/headers.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/headers.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/simple_server.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/simple_server.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/util.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/util.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/validate.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/wsgiref/validate.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xdrlib.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xdrlib.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/minicompat.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/minicompat.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/minidom.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/dom/minidom.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/ElementInclude.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/ElementInclude.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/ElementPath.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/ElementPath.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/ElementTree.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/etree/ElementTree.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/handler.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/handler.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/saxutils.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/saxutils.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/xmlreader.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xml/sax/xmlreader.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xmlrpc/client.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xmlrpc/client.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xmlrpc/server.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/xmlrpc/server.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/zipapp.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/zipapp.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/zipfile.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/zipfile.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/zipimport.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/zipimport.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/zlib.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/zlib.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/zoneinfo/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stdlib/zoneinfo/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypy/typeshed/stubs/mypy-extensions/mypy_extensions.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypy/typeshed/stubs/mypy-extensions/mypy_extensions.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/mypyc/test-data/fixtures/typing-full.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/mypyc/test-data/fixtures/typing-full.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/py/_vendored_packages/iniconfig/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/py/_vendored_packages/iniconfig/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/py/error.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/py/error.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/py/iniconfig.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/py/iniconfig.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/py/io.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/py/io.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/py/path.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/py/path.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/py/xml.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/py/xml.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/pytz-stubs/__init__.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/pytz-stubs/__init__.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/.venv/lib/python3.9/site-packages/pytz-stubs/tzinfo.pyi` & `nwon_baseline-0.2.1/.venv/lib/python3.9/site-packages/pytz-stubs/tzinfo.pyi`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/README.md` & `nwon_baseline-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/nwon_baseline/date_helper/country.py` & `nwon_baseline-0.2.1/nwon_baseline/date_helper/country.py`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/nwon_baseline/date_helper/datetime.py` & `nwon_baseline-0.2.1/nwon_baseline/date_helper/datetime.py`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/nwon_baseline/date_helper/time_differences.py` & `nwon_baseline-0.2.1/nwon_baseline/date_helper/time_differences.py`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/nwon_baseline/directory_helper/__init__.py` & `nwon_baseline-0.2.1/nwon_baseline/directory_helper/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,20 +4,20 @@
     file_names_in_directory,
     file_paths_in_directory,
     get_latest_file_in_directory,
 )
 from nwon_baseline.directory_helper.directory_interactions import (
     clean_directory,
     copy_directory,
-    create_pathes,
+    create_paths,
 )
 
 __all__ = [
     "clean_directory",
     "copy_directory",
     "directory_names_in_directory",
     "file_names_in_directory",
     "file_paths_in_directory",
     "get_latest_file_in_directory",
-    "create_pathes",
+    "create_paths",
     "directory_paths_in_directory",
 ]
```

### Comparing `nwon_baseline-0.1.33/nwon_baseline/directory_helper/directory_content.py` & `nwon_baseline-0.2.1/nwon_baseline/directory_helper/directory_content.py`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/nwon_baseline/directory_helper/directory_interactions.py` & `nwon_baseline-0.2.1/nwon_baseline/directory_helper/directory_interactions.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,23 +1,21 @@
 import os
 import shutil
 from os import path
 from pathlib import Path
 from typing import List
 
 from nwon_baseline.directory_helper.directory_content import (
-    directory_names_in_directory,
     directory_paths_in_directory,
-    file_names_in_directory,
     file_paths_in_directory,
 )
 
 
-def create_pathes(pathes: List[str]) -> None:
-    for path_to_create in pathes:
+def create_paths(paths: List[str]) -> None:
+    for path_to_create in paths:
         Path(path_to_create).mkdir(parents=True, exist_ok=True)
 
 
 def copy_directory(source_directory: str, target_directory: str) -> None:
     if path.exists(target_directory):
         shutil.rmtree(target_directory)
```

### Comparing `nwon_baseline-0.1.33/nwon_baseline/file_helper/__init__.py` & `nwon_baseline-0.2.1/nwon_baseline/file_helper/__init__.py`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/nwon_baseline/file_helper/file.py` & `nwon_baseline-0.2.1/nwon_baseline/file_helper/file.py`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/nwon_baseline/file_helper/filename_from_url.py` & `nwon_baseline-0.2.1/nwon_baseline/file_helper/filename_from_url.py`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/nwon_baseline/image_helper/image.py` & `nwon_baseline-0.2.1/nwon_baseline/image_helper/image.py`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/nwon_baseline/import_helper/import_from_file.py` & `nwon_baseline-0.2.1/nwon_baseline/import_helper/import_from_file.py`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/nwon_baseline/poetry/checking_version_argument.py` & `nwon_baseline-0.2.1/nwon_baseline/poetry/checking_version_argument.py`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/nwon_baseline/poetry/package_version.py` & `nwon_baseline-0.2.1/nwon_baseline/poetry/package_version.py`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/nwon_baseline/print_helper/colored_printing.py` & `nwon_baseline-0.2.1/nwon_baseline/print_helper/colored_printing.py`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/nwon_baseline/pydantic/path_to_write_pydantic_model.py` & `nwon_baseline-0.2.1/nwon_baseline/pydantic/path_to_write_pydantic_model.py`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/nwon_baseline/pydantic/save_pydantic_model_instance.py` & `nwon_baseline-0.2.1/nwon_baseline/pydantic/save_pydantic_model_instance.py`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/nwon_baseline/pydantic/save_pydantic_model_schema.py` & `nwon_baseline-0.2.1/nwon_baseline/pydantic/save_pydantic_model_schema.py`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/nwon_baseline/shell_helper/execute_command.py` & `nwon_baseline-0.2.1/nwon_baseline/shell_helper/execute_command.py`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/nwon_baseline/shell_helper/get_environment_variable.py` & `nwon_baseline-0.2.1/nwon_baseline/shell_helper/get_environment_variable.py`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/nwon_baseline/type_helper/enum_value_list.py` & `nwon_baseline-0.2.1/nwon_baseline/type_helper/enum_value_list.py`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/nwon_baseline/typings/__init__.py` & `nwon_baseline-0.2.1/nwon_baseline/typings/__init__.py`

 * *Files identical despite different names*

### Comparing `nwon_baseline-0.1.33/pyproject.toml` & `nwon_baseline-0.2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 description = "Python Code that is used in several projects"
 homepage = "https://nwon.de"
 include = ["README.md", "**/*.pyi"]
 license = "MIT"
 name = "nwon_baseline"
 readme = "README.md"
 repository = "https://gitlab.com/nvon/pypi-packages/nwon_baseline"
-version = "0.1.33"
+version = "0.2.1"
 
 [tool.poetry.dependencies]
 python = ">=3.7,<4.0"
 
 pydantic = ">=1.8.2"
 pytz = "^2022.1"
```

### Comparing `nwon_baseline-0.1.33/PKG-INFO` & `nwon_baseline-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: nwon-baseline
-Version: 0.1.33
+Version: 0.2.1
 Summary: Python Code that is used in several projects
 Home-page: https://nwon.de
 License: MIT
 Author: Reik Stiebeling
 Author-email: reik.stiebeling@nwon.de
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: pydantic (>=1.8.2)
 Requires-Dist: pytz (>=2022.1,<2023.0)
 Project-URL: Repository, https://gitlab.com/nvon/pypi-packages/nwon_baseline
 Description-Content-Type: text/markdown
 
 # NWON Python baseline package
```

