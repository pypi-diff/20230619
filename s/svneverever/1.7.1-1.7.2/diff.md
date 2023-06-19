# Comparing `tmp/svneverever-1.7.1.tar.gz` & `tmp/svneverever-1.7.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "svneverever-1.7.1.tar", last modified: Thu Jul  8 22:51:27 2021, max compression
+gzip compressed data, was "svneverever-1.7.2.tar", last modified: Mon Jun 19 10:38:26 2023, max compression
```

## Comparing `svneverever-1.7.1.tar` & `svneverever-1.7.2.tar`

### file list

```diff
@@ -1,18 +1,24 @@
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-08 22:51:27.626762 svneverever-1.7.1/
--rw-r--r--   0 sping     (1000) sping     (1000)       22 2019-06-17 20:38:10.000000 svneverever-1.7.1/.gitignore
--rw-r--r--   0 sping     (1000) sping     (1000)      435 2021-07-03 11:26:38.000000 svneverever-1.7.1/.pre-commit-config.yaml
--rw-r--r--   0 sping     (1000) sping     (1000)      265 2020-05-04 15:29:59.000000 svneverever-1.7.1/Makefile
--rw-r--r--   0 sping     (1000) sping     (1000)     7528 2021-07-08 22:51:27.626762 svneverever-1.7.1/PKG-INFO
--rw-r--r--   0 sping     (1000) sping     (1000)     6488 2021-07-03 11:25:24.000000 svneverever-1.7.1/README.md
--rw-r--r--   0 sping     (1000) sping     (1000)       38 2021-07-08 22:51:27.626762 svneverever-1.7.1/setup.cfg
--rwxr-xr-x   0 sping     (1000) sping     (1000)     1767 2021-07-03 11:24:32.000000 svneverever-1.7.1/setup.py
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-08 22:51:27.625762 svneverever-1.7.1/svneverever/
--rw-r--r--   0 sping     (1000) sping     (1000)        0 2019-06-17 20:25:43.000000 svneverever-1.7.1/svneverever/__init__.py
--rwxr-xr-x   0 sping     (1000) sping     (1000)    15033 2021-07-08 22:50:17.000000 svneverever-1.7.1/svneverever/__main__.py
--rw-r--r--   0 sping     (1000) sping     (1000)      170 2021-07-08 22:50:40.000000 svneverever-1.7.1/svneverever/version.py
-drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2021-07-08 22:51:27.626762 svneverever-1.7.1/svneverever.egg-info/
--rw-r--r--   0 sping     (1000) sping     (1000)     7528 2021-07-08 22:51:27.000000 svneverever-1.7.1/svneverever.egg-info/PKG-INFO
--rw-r--r--   0 sping     (1000) sping     (1000)      311 2021-07-08 22:51:27.000000 svneverever-1.7.1/svneverever.egg-info/SOURCES.txt
--rw-r--r--   0 sping     (1000) sping     (1000)        1 2021-07-08 22:51:27.000000 svneverever-1.7.1/svneverever.egg-info/dependency_links.txt
--rw-r--r--   0 sping     (1000) sping     (1000)       59 2021-07-08 22:51:27.000000 svneverever-1.7.1/svneverever.egg-info/entry_points.txt
--rw-r--r--   0 sping     (1000) sping     (1000)       12 2021-07-08 22:51:27.000000 svneverever-1.7.1/svneverever.egg-info/top_level.txt
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-06-19 10:38:26.820754 svneverever-1.7.2/
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-06-19 10:38:26.817754 svneverever-1.7.2/.github/
+-rw-r--r--   0 sping     (1000) sping     (1000)      220 2022-03-08 01:32:35.000000 svneverever-1.7.2/.github/dependabot.yml
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-06-19 10:38:26.818755 svneverever-1.7.2/.github/workflows/
+-rw-r--r--   0 sping     (1000) sping     (1000)     2212 2023-06-13 16:36:19.000000 svneverever-1.7.2/.github/workflows/pre-commit-detect-outdated.yml
+-rw-r--r--   0 sping     (1000) sping     (1000)     1001 2023-06-13 16:36:19.000000 svneverever-1.7.2/.github/workflows/pre-commit-run.yml
+-rw-r--r--   0 sping     (1000) sping     (1000)     1188 2023-06-19 10:35:54.000000 svneverever-1.7.2/.github/workflows/run-tests.yml
+-rw-r--r--   0 sping     (1000) sping     (1000)       22 2019-06-17 20:38:10.000000 svneverever-1.7.2/.gitignore
+-rw-r--r--   0 sping     (1000) sping     (1000)      544 2023-06-19 10:13:45.000000 svneverever-1.7.2/.pre-commit-config.yaml
+-rw-r--r--   0 sping     (1000) sping     (1000)      265 2020-05-04 15:29:59.000000 svneverever-1.7.2/Makefile
+-rw-r--r--   0 sping     (1000) sping     (1000)     8104 2023-06-19 10:38:26.820754 svneverever-1.7.2/PKG-INFO
+-rw-r--r--   0 sping     (1000) sping     (1000)     7134 2023-06-19 10:13:35.000000 svneverever-1.7.2/README.md
+-rw-r--r--   0 sping     (1000) sping     (1000)       38 2023-06-19 10:38:26.821755 svneverever-1.7.2/setup.cfg
+-rwxr-xr-x   0 sping     (1000) sping     (1000)     1718 2022-03-09 02:24:54.000000 svneverever-1.7.2/setup.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-06-19 10:38:26.819754 svneverever-1.7.2/svneverever/
+-rw-r--r--   0 sping     (1000) sping     (1000)        0 2019-06-17 20:25:43.000000 svneverever-1.7.2/svneverever/__init__.py
+-rwxr-xr-x   0 sping     (1000) sping     (1000)    15211 2023-06-19 10:35:48.000000 svneverever-1.7.2/svneverever/__main__.py
+-rw-r--r--   0 sping     (1000) sping     (1000)      170 2023-06-19 10:38:16.000000 svneverever-1.7.2/svneverever/version.py
+drwxr-xr-x   0 sping     (1000) sping     (1000)        0 2023-06-19 10:38:26.820754 svneverever-1.7.2/svneverever.egg-info/
+-rw-r--r--   0 sping     (1000) sping     (1000)     8104 2023-06-19 10:38:26.000000 svneverever-1.7.2/svneverever.egg-info/PKG-INFO
+-rw-r--r--   0 sping     (1000) sping     (1000)      452 2023-06-19 10:38:26.000000 svneverever-1.7.2/svneverever.egg-info/SOURCES.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)        1 2023-06-19 10:38:26.000000 svneverever-1.7.2/svneverever.egg-info/dependency_links.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)       58 2023-06-19 10:38:26.000000 svneverever-1.7.2/svneverever.egg-info/entry_points.txt
+-rw-r--r--   0 sping     (1000) sping     (1000)       12 2023-06-19 10:38:26.000000 svneverever-1.7.2/svneverever.egg-info/top_level.txt
```

### Comparing `svneverever-1.7.1/PKG-INFO` & `svneverever-1.7.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 Metadata-Version: 2.1
 Name: svneverever
-Version: 1.7.1
+Version: 1.7.2
 Summary: Tool collecting path entries across SVN history
 Home-page: https://github.com/hartwork/svneverever
 Author: Sebastian Pipping
 Author-email: sebastian@pipping.org
 License: GPL v3 or later
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
+
+
 # About
 **svneverever** helps you inspect the structure of a SVN repository and the changes made to it over time. Its most common use is in combination with [svn-all-fast-export](https://github.com/svn-all-fast-export/svn2git) (or "KDE's svn2git" if you wish).
 
 
 # Installation
 
 ## Dependencies
-**svneverever** requires Python 3.6 or higher
+**svneverever** requires Python 3.7 or higher
 and [PySVN](https://pysvn.sourceforge.io/)
 (the one on SourceForge, not the one on PyPI).
 If you want to install **svneverever** with **pip** you need a few additional packages.
 For Debian/Ubuntu the following should work:
 
 ```console
 # sudo apt install python3-svn python3-pip
@@ -61,17 +62,33 @@
 # python3 setup.py install --user
 # echo 'export PATH="${HOME}/.local/bin:${PATH}"' >> ~/.bashrc
 ```
 
 # Usage
 **svneverever** needs the "server-side" of the repository with full history. There are two ways to obtain this. Let's take the SVN history of [headphone effect library bs2b](http://bs2b.sourceforge.net/) as an example.
 
-The first way is to directly point **svneverever** to the server `svneverever svn://svn.code.sf.net/p/bs2b/code/`. However this is slow and it puts a lot of stress on the server.
+The first way is to directly point **svneverever** to the server `svneverever svn://svn.code.sf.net/p/bs2b/code/`. However this is slow and it puts a lot of stress on the server, and will be little fun to run multiple times.
+
+The second and recommended method is first downloading the history with
+`svnrdump dump` (that comes with Subversion >=1.7) or [`rsvndump`](https://github.com/jgehring/rsvndump) (with a slightly [different feature set](https://rsvndump.sourceforge.io/) and supporting older versions of Subversion).
+For this method we first need to use `svnadmin` to create an empty repository and then load the output of svnrdump/rsvndump into it. This can be done in the following way:
+
+## With `svnrdump dump`
+
+```console
+# svnadmin create bs2b_svn_store
+
+# time sh -c 'svnrdump dump svn://svn.code.sf.net/p/bs2b/code/ | svnadmin load bs2b_svn_store/'
+[..]
+real    0m3.008s
+user    0m0.309s
+sys     0m0.235s
+```
 
-The second, and recommended, method is first downloading the history with **rsvndump**. For this method we first need to use `svnadmin` to create an empty repository and then load the output of **rsvndump** into it. This can be done in the following way:
+## With `rsvndump`
 
 ```console
 # svnadmin create bs2b_svn_store
 
 # time sh -c 'rsvndump svn://svn.code.sf.net/p/bs2b/code/ | svnadmin load bs2b_svn_store/'
 [..]
 real    2m54.403s
@@ -202,9 +219,7 @@
 committer mode arguments:
   --unknown-committer NAME
                         Committer name to use for commits without a proper
                         svn:author property (default: "<unknown>")
 
 Please report bugs at https://github.com/hartwork/svneverever.  Thank you!
 ```
-
-
```

### Comparing `svneverever-1.7.1/README.md` & `svneverever-1.7.2/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,15 +1,18 @@
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
+
+
 # About
 **svneverever** helps you inspect the structure of a SVN repository and the changes made to it over time. Its most common use is in combination with [svn-all-fast-export](https://github.com/svn-all-fast-export/svn2git) (or "KDE's svn2git" if you wish).
 
 
 # Installation
 
 ## Dependencies
-**svneverever** requires Python 3.6 or higher
+**svneverever** requires Python 3.7 or higher
 and [PySVN](https://pysvn.sourceforge.io/)
 (the one on SourceForge, not the one on PyPI).
 If you want to install **svneverever** with **pip** you need a few additional packages.
 For Debian/Ubuntu the following should work:
 
 ```console
 # sudo apt install python3-svn python3-pip
@@ -35,17 +38,33 @@
 # python3 setup.py install --user
 # echo 'export PATH="${HOME}/.local/bin:${PATH}"' >> ~/.bashrc
 ```
 
 # Usage
 **svneverever** needs the "server-side" of the repository with full history. There are two ways to obtain this. Let's take the SVN history of [headphone effect library bs2b](http://bs2b.sourceforge.net/) as an example.
 
-The first way is to directly point **svneverever** to the server `svneverever svn://svn.code.sf.net/p/bs2b/code/`. However this is slow and it puts a lot of stress on the server.
+The first way is to directly point **svneverever** to the server `svneverever svn://svn.code.sf.net/p/bs2b/code/`. However this is slow and it puts a lot of stress on the server, and will be little fun to run multiple times.
+
+The second and recommended method is first downloading the history with
+`svnrdump dump` (that comes with Subversion >=1.7) or [`rsvndump`](https://github.com/jgehring/rsvndump) (with a slightly [different feature set](https://rsvndump.sourceforge.io/) and supporting older versions of Subversion).
+For this method we first need to use `svnadmin` to create an empty repository and then load the output of svnrdump/rsvndump into it. This can be done in the following way:
+
+## With `svnrdump dump`
+
+```console
+# svnadmin create bs2b_svn_store
+
+# time sh -c 'svnrdump dump svn://svn.code.sf.net/p/bs2b/code/ | svnadmin load bs2b_svn_store/'
+[..]
+real    0m3.008s
+user    0m0.309s
+sys     0m0.235s
+```
 
-The second, and recommended, method is first downloading the history with **rsvndump**. For this method we first need to use `svnadmin` to create an empty repository and then load the output of **rsvndump** into it. This can be done in the following way:
+## With `rsvndump`
 
 ```console
 # svnadmin create bs2b_svn_store
 
 # time sh -c 'rsvndump svn://svn.code.sf.net/p/bs2b/code/ | svnadmin load bs2b_svn_store/'
 [..]
 real    2m54.403s
```

### Comparing `svneverever-1.7.1/setup.py` & `svneverever-1.7.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     author_email='sebastian@pipping.org',
     packages=find_packages(),
     entry_points={
         'console_scripts': [
             'svneverever = svneverever.__main__:main',
         ],
     },
-    python_requires='>=3.6',
+    python_requires='>=3.7',
     setup_requires=[
         'setuptools>=38.6.0',  # for long_description_content_type
     ],
     install_requires=[
         # Package 'pysvn' on PyPI is not the PySVN off SourceForge
         # that we need!
     ],
@@ -38,15 +38,14 @@
         'Intended Audience :: Developers',
         'Intended Audience :: System Administrators',
         'License :: OSI Approved '
         ':: GNU General Public License v3 or later (GPLv3+)',
         'Natural Language :: English',
         'Programming Language :: Python',
         'Programming Language :: Python :: 3',
-        'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3 :: Only',
         'Topic :: Software Development :: Version Control',
         'Topic :: Utilities',
     ],
 )
```

### Comparing `svneverever-1.7.1/svneverever/__main__.py` & `svneverever-1.7.2/svneverever/__main__.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 #!/usr/bin/env python3
-# -*- coding: utf-8 -*-
 # Copyright (C) 2010-2021 Sebastian Pipping <sebastian@pipping.org>
 # Copyright (C) 2011      Wouter Haffmans <wouter@boxplosive.nl>
 # Copyright (C) 2019      Kevin Lane <kevin.lane84@outlook.com>
 # Licensed under GPL v3 or later
 #
-from __future__ import print_function
 
 import argparse
 import getpass
 import math
 import os
 import re
 import signal
@@ -62,32 +60,25 @@
             os.close(fd)
     except Exception:
         pass
 
     return _OsTerminalSize(columns=80, lines=24)
 
 
-def _for_print(text):
-    if sys.version_info >= (3, ):
-        return text
-
-    return text.encode(sys.stdout.encoding or 'UTF-8', 'replace')
-
-
 def dump_tree(t, revision_digits, latest_revision, config,
               level=0, branch_level=-3, tag_level=-3, parent_dir=''):
     def indent_print(line_start, text):
         if config.flat_tree:
             level_text = parent_dir
         else:
             level_text = ' '*(4*level)
         if config.show_numbers:
-            print('{}  {}{}'.format(line_start, level_text, _for_print(text)))
+            print(f'{line_start}  {level_text}{text}')
         else:
-            print('{}{}'.format(level_text, _for_print(text)))
+            print(f'{level_text}{text}')
 
     items = ((k, v) for k, v in t.items() if k)
 
     if ((branch_level + 2 == level) and not config.show_branches) \
             or ((tag_level + 2 == level) and not config.show_tags) \
             or level >= config.max_depth:
         if items and config.show_dots:
@@ -112,30 +103,30 @@
         tl = tag_level
         if k == 'branches':
             bl = level
         elif k == 'tags':
             tl = level
         dump_tree(children, revision_digits, latest_revision, config,
                   level=level + 1, branch_level=bl, tag_level=tl,
-                  parent_dir='{}/{}'.format(parent_dir, k))
+                  parent_dir=f'{parent_dir}/{k}')
 
 
 def dump_nick_stats(nick_stats, revision_digits, config):
     if config.show_numbers:
         format = "%%%dd (%%%dd; %%%dd)  %%s" % (revision_digits,
                                                 revision_digits,
                                                 revision_digits)
         for nick, (first_commit_rev, last_commit_rev, commit_count) \
                 in sorted(nick_stats.items()):
             print(format % (commit_count, first_commit_rev, last_commit_rev,
-                            _for_print(nick)))
+                            nick))
     else:
         for nick, (first_commit_rev, last_commit_rev, commit_count) \
                 in sorted(nick_stats.items()):
-            print(_for_print(nick))
+            print(nick)
 
 
 def ensure_uri(text):
     svn_uri_detector = re.compile('^[A-Za-z+]+://')
     if svn_uri_detector.search(text):
         return text
     else:
@@ -144,32 +135,32 @@
             raise _SvnCheckoutDetected(abspath)
         return 'file://%s' % urllib_parse_quote(abspath)
 
 
 def digit_count(n):
     if n == 0:
         return 1
-    assert(n > 0)
+    assert n > 0
     return int(math.floor(math.log10(n)) + 1)
 
 
 def hms(seconds):
     seconds = math.ceil(seconds)
     h = int(seconds / 3600)
     seconds = seconds - h*3600
     m = int(seconds / 60)
     seconds = seconds - m*60
     return h, m, seconds
 
 
 def make_progress_bar(percent, width, seconds_taken, seconds_expected):
     other_len = (6 + 1) + 2 + (1 + 8 + 1 + 9 + 1) + 3 + 1
-    assert(width > 0)
+    assert width > 0
     bar_content_len = width - other_len
-    assert(bar_content_len >= 0)
+    assert bar_content_len >= 0
     fill_len = int(percent * bar_content_len / 100)
     open_len = bar_content_len - fill_len
     seconds_remaining = seconds_expected - seconds_taken
     hr, mr, sr = hms(seconds_remaining)
     if hr > 99:
         hr = 99
     return ('%6.2f%%  (%02d:%02d:%02d remaining)  [%s%s]'
@@ -254,15 +245,15 @@
 def _login(realm, username, may_save, _tries):
     if _tries > 0:
         print('ERROR: Credentials not accepted by SVN, please try again.',
               file=sys.stderr)
 
     try:
         if username:
-            print('Username: {}  (as requested by SVN)'.format(username),
+            print(f'Username: {username}  (as requested by SVN)',
                   file=sys.stderr)
         else:
             print('Username: ', end='', file=sys.stderr)
             username = input('')
         password = getpass.getpass('Password: ')
         print(file=sys.stderr)
         return True, username, password, False
@@ -363,21 +354,31 @@
             nick_stats[committer_name] = (first_commit_rev, last_commit_rev,
                                           commit_count)
 
             if args.show_progress:
                 indicate_progress(rev)
             continue
 
-        summary = client.diff_summarize(
-            args.repo_uri,
-            revision1=pysvn.Revision(pysvn.opt_revision_kind.number, rev - 1),
-            url_or_path2=args.repo_uri,
-            revision2=pysvn.Revision(pysvn.opt_revision_kind.number, rev),
-            recurse=True,
-            ignore_ancestry=True)
+        try:
+            summary = client.diff_summarize(
+                args.repo_uri,
+                revision1=pysvn.Revision(pysvn.opt_revision_kind.number,
+                                         rev - 1),
+                url_or_path2=args.repo_uri,
+                revision2=pysvn.Revision(pysvn.opt_revision_kind.number,
+                                         rev),
+                recurse=True,
+                ignore_ancestry=True)
+        except pysvn.ClientError as e:
+            if not (rev == 1 and 'not found in the repository' in str(e)):
+                raise
+            print('ERROR: Path does not exist in the repository at revision 1'
+                  '. Please use svneverever with the root of the repository.',
+                  file=sys.stderr)
+            sys.exit(1)
 
         def is_directory_addition(summary_entry):
             return (summary_entry.summarize_kind
                     == pysvn.diff_summarize_kind.added
                     and summary_entry.node_kind == pysvn.node_kind.dir)
 
         def is_directory_deletion(summary_entry):
```

### Comparing `svneverever-1.7.1/svneverever.egg-info/PKG-INFO` & `svneverever-1.7.2/svneverever.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 Metadata-Version: 2.1
 Name: svneverever
-Version: 1.7.1
+Version: 1.7.2
 Summary: Tool collecting path entries across SVN history
 Home-page: https://github.com/hartwork/svneverever
 Author: Sebastian Pipping
 Author-email: sebastian@pipping.org
 License: GPL v3 or later
-Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Topic :: Software Development :: Version Control
 Classifier: Topic :: Utilities
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
+[![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit)](https://github.com/pre-commit/pre-commit)
+
+
 # About
 **svneverever** helps you inspect the structure of a SVN repository and the changes made to it over time. Its most common use is in combination with [svn-all-fast-export](https://github.com/svn-all-fast-export/svn2git) (or "KDE's svn2git" if you wish).
 
 
 # Installation
 
 ## Dependencies
-**svneverever** requires Python 3.6 or higher
+**svneverever** requires Python 3.7 or higher
 and [PySVN](https://pysvn.sourceforge.io/)
 (the one on SourceForge, not the one on PyPI).
 If you want to install **svneverever** with **pip** you need a few additional packages.
 For Debian/Ubuntu the following should work:
 
 ```console
 # sudo apt install python3-svn python3-pip
@@ -61,17 +62,33 @@
 # python3 setup.py install --user
 # echo 'export PATH="${HOME}/.local/bin:${PATH}"' >> ~/.bashrc
 ```
 
 # Usage
 **svneverever** needs the "server-side" of the repository with full history. There are two ways to obtain this. Let's take the SVN history of [headphone effect library bs2b](http://bs2b.sourceforge.net/) as an example.
 
-The first way is to directly point **svneverever** to the server `svneverever svn://svn.code.sf.net/p/bs2b/code/`. However this is slow and it puts a lot of stress on the server.
+The first way is to directly point **svneverever** to the server `svneverever svn://svn.code.sf.net/p/bs2b/code/`. However this is slow and it puts a lot of stress on the server, and will be little fun to run multiple times.
+
+The second and recommended method is first downloading the history with
+`svnrdump dump` (that comes with Subversion >=1.7) or [`rsvndump`](https://github.com/jgehring/rsvndump) (with a slightly [different feature set](https://rsvndump.sourceforge.io/) and supporting older versions of Subversion).
+For this method we first need to use `svnadmin` to create an empty repository and then load the output of svnrdump/rsvndump into it. This can be done in the following way:
+
+## With `svnrdump dump`
+
+```console
+# svnadmin create bs2b_svn_store
+
+# time sh -c 'svnrdump dump svn://svn.code.sf.net/p/bs2b/code/ | svnadmin load bs2b_svn_store/'
+[..]
+real    0m3.008s
+user    0m0.309s
+sys     0m0.235s
+```
 
-The second, and recommended, method is first downloading the history with **rsvndump**. For this method we first need to use `svnadmin` to create an empty repository and then load the output of **rsvndump** into it. This can be done in the following way:
+## With `rsvndump`
 
 ```console
 # svnadmin create bs2b_svn_store
 
 # time sh -c 'rsvndump svn://svn.code.sf.net/p/bs2b/code/ | svnadmin load bs2b_svn_store/'
 [..]
 real    2m54.403s
@@ -202,9 +219,7 @@
 committer mode arguments:
   --unknown-committer NAME
                         Committer name to use for commits without a proper
                         svn:author property (default: "<unknown>")
 
 Please report bugs at https://github.com/hartwork/svneverever.  Thank you!
 ```
-
-
```

