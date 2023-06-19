# Comparing `tmp/cdhist-3.6.tar.gz` & `tmp/cdhist-3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdhist-3.6.tar", last modified: Sun Feb 12 10:42:20 2023, max compression
+gzip compressed data, was "cdhist-3.7.tar", last modified: Mon Jun 19 03:48:26 2023, max compression
```

## Comparing `cdhist-3.6.tar` & `cdhist-3.7.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-02-12 10:42:20.086303 cdhist-3.6/
--rw-r--r--   0 mark      (1000) mark      (1000)    16103 2023-02-12 10:42:20.086303 cdhist-3.6/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)    15709 2023-02-12 10:19:42.000000 cdhist-3.6/README.md
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-02-12 10:42:20.086303 cdhist-3.6/cdhist/
--rw-r--r--   0 mark      (1000) mark      (1000)        0 2022-09-20 03:37:27.000000 cdhist-3.6/cdhist/__init__.py
--rw-r--r--   0 mark      (1000) mark      (1000)       90 2022-10-01 21:49:57.000000 cdhist-3.6/cdhist/__main__.py
--rw-r--r--   0 mark      (1000) mark      (1000)     9144 2023-02-12 10:28:34.000000 cdhist-3.6/cdhist/cdhist.py
--rw-r--r--   0 mark      (1000) mark      (1000)     4489 2023-01-16 10:03:18.000000 cdhist-3.6/cdhist/git_worktree.py
--rw-r--r--   0 mark      (1000) mark      (1000)     2849 2023-01-15 07:05:36.000000 cdhist-3.6/cdhist/utils.py
--rw-r--r--   0 mark      (1000) mark      (1000)      331 2023-02-12 10:32:56.000000 cdhist-3.6/cdhist/version.py
-drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-02-12 10:42:20.086303 cdhist-3.6/cdhist.egg-info/
--rw-r--r--   0 mark      (1000) mark      (1000)    16103 2023-02-12 10:42:20.000000 cdhist-3.6/cdhist.egg-info/PKG-INFO
--rw-r--r--   0 mark      (1000) mark      (1000)      312 2023-02-12 10:42:20.000000 cdhist-3.6/cdhist.egg-info/SOURCES.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-02-12 10:42:20.000000 cdhist-3.6/cdhist.egg-info/dependency_links.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       46 2023-02-12 10:42:20.000000 cdhist-3.6/cdhist.egg-info/entry_points.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       51 2023-02-12 10:42:20.000000 cdhist-3.6/cdhist.egg-info/requires.txt
--rw-r--r--   0 mark      (1000) mark      (1000)        7 2023-02-12 10:42:20.000000 cdhist-3.6/cdhist.egg-info/top_level.txt
--rw-r--r--   0 mark      (1000) mark      (1000)       38 2023-02-12 10:42:20.086303 cdhist-3.6/setup.cfg
--rw-r--r--   0 mark      (1000) mark      (1000)      956 2023-02-12 10:38:00.000000 cdhist-3.6/setup.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-06-19 03:48:26.418992 cdhist-3.7/
+-rw-r--r--   0 mark      (1000) mark      (1000)       74 2023-06-19 03:15:16.000000 cdhist-3.7/.flake8
+-rw-r--r--   0 mark      (1000) mark      (1000)       72 2023-03-30 00:30:45.000000 cdhist-3.7/.gitignore
+-rw-r--r--   0 mark      (1000) mark      (1000)      343 2023-06-19 03:26:25.000000 cdhist-3.7/Makefile
+-rw-r--r--   0 mark      (1000) mark      (1000)    15976 2023-06-19 03:48:26.418992 cdhist-3.7/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)    15576 2023-06-19 03:27:42.000000 cdhist-3.7/README.md
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-06-19 03:48:26.418992 cdhist-3.7/cdhist/
+-rw-r--r--   0 mark      (1000) mark      (1000)        0 2022-09-20 03:37:27.000000 cdhist-3.7/cdhist/__init__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)       90 2022-10-01 21:49:57.000000 cdhist-3.7/cdhist/__main__.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     9425 2023-06-19 03:43:27.000000 cdhist-3.7/cdhist/cdhist.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     4474 2023-06-19 03:24:01.000000 cdhist-3.7/cdhist/git_worktree.py
+-rw-r--r--   0 mark      (1000) mark      (1000)     2834 2023-06-19 03:43:27.000000 cdhist-3.7/cdhist/utils.py
+drwxr-xr-x   0 mark      (1000) mark      (1000)        0 2023-06-19 03:48:26.418992 cdhist-3.7/cdhist.egg-info/
+-rw-r--r--   0 mark      (1000) mark      (1000)    15976 2023-06-19 03:48:26.000000 cdhist-3.7/cdhist.egg-info/PKG-INFO
+-rw-r--r--   0 mark      (1000) mark      (1000)      328 2023-06-19 03:48:26.000000 cdhist-3.7/cdhist.egg-info/SOURCES.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        1 2023-06-19 03:48:26.000000 cdhist-3.7/cdhist.egg-info/dependency_links.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       39 2023-06-19 03:48:26.000000 cdhist-3.7/cdhist.egg-info/entry_points.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)       51 2023-06-19 03:48:26.000000 cdhist-3.7/cdhist.egg-info/requires.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)        7 2023-06-19 03:48:26.000000 cdhist-3.7/cdhist.egg-info/top_level.txt
+-rw-r--r--   0 mark      (1000) mark      (1000)     1009 2023-06-19 03:26:01.000000 cdhist-3.7/pyproject.toml
+-rw-r--r--   0 mark      (1000) mark      (1000)       38 2023-06-19 03:48:26.418992 cdhist-3.7/setup.cfg
```

### Comparing `cdhist-3.6/PKG-INFO` & `cdhist-3.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,7 @@
-Metadata-Version: 2.1
-Name: cdhist
-Version: 3.6
-Summary: Program to provide a Linux cd history directory stack
-Home-page: https://github.com/bulletmark/cdhist
-Author: Mark Blakeney
-Author-email: mark.blakeney@bullet-systems.net
-License: GPLv3
-Keywords: bash zsh cd fzf git worktree
-Classifier: Programming Language :: Python :: 3
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-
 ## Linux Directory History
 [![PyPi](https://img.shields.io/pypi/v/cdhist)](https://pypi.org/project/cdhist/)
 [![AUR](https://img.shields.io/aur/version/cdhist)](https://aur.archlinux.org/packages/cdhist/)
 
 [cdhist](http://github.com/bulletmark/cdhist) is a utility which
 provides a Linux shell **cd history** directory stack. A shell `cd`
 wrapper function calls cdhist to intercept your typed `cd` command and
@@ -98,30 +85,33 @@
 
 ## Installation
 
 Arch users can install [cdhist from the
 AUR](https://aur.archlinux.org/packages/cdhist/) and skip to the next
 section.
 
-Ensure `pip3` is installed. Python 3.7 or later is required.
+Python 3.7 or later is required. Note [cdhist is on
+PyPI](https://pypi.org/project/cdhist/) so just ensure that
+[`pipx`](https://pypa.github.io/pipx/) is installed then type the
+following:
 
-Note [cdhist is on PyPI](https://pypi.org/project/cdhist/) so you can
-just type `sudo pip3 install -U cdhist`. Or do the following to install
-from this repository:
+```
+$ pipx install cdhist
+```
 
-```sh
-$ git clone http://github.com/bulletmark/cdhist
-$ cd cdhist
-$ sudo pip3 install -U .
+To upgrade:
+
+```
+$ pipx upgrade cdhist
 ```
 
 ## Setup
 
-Each user who wants to use the cdhist facility should add the following
-lines to their `~/.bashrc` or `~.zshrc` file (after where your PATH is
+A user who wants to use the cdhist facility should add the following
+lines to their `~/.bashrc` or `~/.zshrc` file (after where your PATH is
 set up so that the command `cdhist` can be found). This creates the `cd`
 wrapper command in your interactive shell session as a tiny function.
 Note you can [customize the command name](#alternative-command-name) if
 you want.
 
 ```sh
 if type cdhist &>/dev/null; then
@@ -186,15 +176,15 @@
 ## Alternative Command Name
 
 Some people may prefer not to alias their system `cd` command to this
 utility and just use an alternative unique command name. To do this,
 simply add your desired command name as an extra argument to the
 `cdhist` command in your shell initialization code. E.g, to use the
 command name `xd` rather than `cd`, use the following in
-your `~/.bashrc` or `~.zshrc` file:
+your `~/.bashrc` or `~/.zshrc` file:
 
 ```sh
 if type cdhist &>/dev/null; then
     . <(cdhist -i xd)
 fi
 ```
 
@@ -281,15 +271,15 @@
 Some users may want the git worktree functionality provided by cdhist
 but are not interested in the standard `cd` history functionality, or
 alternately, want to use a completely separate command for the git
 worktree functionality. To do this, simply add your desired command name
 and the git option as an extra argument to the `cdhist` command in your
 shell initialization code. E.g, to use the command name `wt` for git
 worktree functionality (only), add the following in your
-`~/.bashrc` or `~.zshrc` file:
+`~/.bashrc` or `~/.zshrc` file:
 
 ```sh
 if type cdhist &>/dev/null; then
     . <(cdhist -i "wt -g")
 fi
 ```
 
@@ -367,51 +357,36 @@
                         alternative command name as argument, default="cd"
   -h, --help            show help/usage
   -p, --purge           just purge non-existent directories from history
   -a, --purge-always    always purge non-existent directories every write
   -g, --git             show git worktree directories instead
   -r, --git-relative    show relative git worktree paths instead of absolute
   -R, --no-git-relative
-                        do not show relative git worktree paths
+                        do not show relative git worktree paths (default)
   -u, --no-user         do not substitute "~" for home directory
-  -U, --user            do substitute "~" for home directory
+  -U, --user            do substitute "~" for home directory (default)
   -l, --list            just list directory history
   -m SIZE, --size SIZE  maximum size of directory history (default=50)
   -n NUM_LINES, --num-lines NUM_LINES
                         limit output to specified number of lines
   -L, --follow-links    follow symbolic links (default=true)
   -P, --follow-physical
                         follow links to physical directory
-  -V, --version         just output version
+  -V, --version         just output cdhist version
 
 Note you can set default options in ~/.config/cdhist-flags.conf.
 ```
 
 ## Limitations
 
 Regular `cd`, e.g. as provided by the bash builtin, offers some esoteric
 command line options such as `-e` and `-@`, and shell options such as
 `autocd`, `cdspell`, `cdable_vars`. These rarely used options are not
 supported by cdhist.
 
-## Upgrade
-
-```sh
-$ cd cdhist  # Source dir, as above
-$ git pull
-$ sudo pip3 install -U .
-```
-
-## Removal
-
-```sh
-$ unset cd
-$ sudo pip3 uninstall cdhist
-```
-
 ## Major Version Change History
 
 Version 3.0 changes and new features:
 
 1. Added function to `cd` between [`git
 worktrees`](https://git-scm.com/docs/git-worktree). Can configure this
 as separate command if preferred, with option to display relative paths.
@@ -446,15 +421,16 @@
 but now we validate it ourself before passing to `cd`. So net
 performance is quicker than previous version, at least for the vanilla
 case of changing directory. This is not noticeable on normal PC's but is
 on constrained platforms like Raspberry Pi 2/3 using SD card.
 
 12. If you were previously setting `CDHISTSIZE` or `CDHISTTILDE` settings
 via environment variables then you now need to set them using `--size`
-and `--no-user` in `~/.config/cdhist-flags.conf`.
+and `--no-user` in `~/.config/cdhist-flags.conf`, or add those options
+in your shell initialization code.
 
 13. The `-s` option to return a `cdhist.rc` file name for initialisation
 is still currently supported for backwards-compatibility but is
 undocumented and depreciated (a temporary file is created and returned).
 It will likely eventually be removed.
 
 ## License
```

### Comparing `cdhist-3.6/README.md` & `cdhist-3.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,19 @@
+Metadata-Version: 2.1
+Name: cdhist
+Version: 3.7
+Summary: Program to provide a Linux cd history directory stack
+Author-email: Mark Blakeney <mark.blakeney@bullet-systems.net>
+License: GPLv3
+Project-URL: Homepage, https://github.com/bulletmark/cdhist
+Keywords: bash,zsh,cd,fzf,git,worktree
+Classifier: Programming Language :: Python :: 3
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+
 ## Linux Directory History
 [![PyPi](https://img.shields.io/pypi/v/cdhist)](https://pypi.org/project/cdhist/)
 [![AUR](https://img.shields.io/aur/version/cdhist)](https://aur.archlinux.org/packages/cdhist/)
 
 [cdhist](http://github.com/bulletmark/cdhist) is a utility which
 provides a Linux shell **cd history** directory stack. A shell `cd`
 wrapper function calls cdhist to intercept your typed `cd` command and
@@ -85,30 +97,33 @@
 
 ## Installation
 
 Arch users can install [cdhist from the
 AUR](https://aur.archlinux.org/packages/cdhist/) and skip to the next
 section.
 
-Ensure `pip3` is installed. Python 3.7 or later is required.
+Python 3.7 or later is required. Note [cdhist is on
+PyPI](https://pypi.org/project/cdhist/) so just ensure that
+[`pipx`](https://pypa.github.io/pipx/) is installed then type the
+following:
 
-Note [cdhist is on PyPI](https://pypi.org/project/cdhist/) so you can
-just type `sudo pip3 install -U cdhist`. Or do the following to install
-from this repository:
+```
+$ pipx install cdhist
+```
 
-```sh
-$ git clone http://github.com/bulletmark/cdhist
-$ cd cdhist
-$ sudo pip3 install -U .
+To upgrade:
+
+```
+$ pipx upgrade cdhist
 ```
 
 ## Setup
 
-Each user who wants to use the cdhist facility should add the following
-lines to their `~/.bashrc` or `~.zshrc` file (after where your PATH is
+A user who wants to use the cdhist facility should add the following
+lines to their `~/.bashrc` or `~/.zshrc` file (after where your PATH is
 set up so that the command `cdhist` can be found). This creates the `cd`
 wrapper command in your interactive shell session as a tiny function.
 Note you can [customize the command name](#alternative-command-name) if
 you want.
 
 ```sh
 if type cdhist &>/dev/null; then
@@ -173,15 +188,15 @@
 ## Alternative Command Name
 
 Some people may prefer not to alias their system `cd` command to this
 utility and just use an alternative unique command name. To do this,
 simply add your desired command name as an extra argument to the
 `cdhist` command in your shell initialization code. E.g, to use the
 command name `xd` rather than `cd`, use the following in
-your `~/.bashrc` or `~.zshrc` file:
+your `~/.bashrc` or `~/.zshrc` file:
 
 ```sh
 if type cdhist &>/dev/null; then
     . <(cdhist -i xd)
 fi
 ```
 
@@ -268,15 +283,15 @@
 Some users may want the git worktree functionality provided by cdhist
 but are not interested in the standard `cd` history functionality, or
 alternately, want to use a completely separate command for the git
 worktree functionality. To do this, simply add your desired command name
 and the git option as an extra argument to the `cdhist` command in your
 shell initialization code. E.g, to use the command name `wt` for git
 worktree functionality (only), add the following in your
-`~/.bashrc` or `~.zshrc` file:
+`~/.bashrc` or `~/.zshrc` file:
 
 ```sh
 if type cdhist &>/dev/null; then
     . <(cdhist -i "wt -g")
 fi
 ```
 
@@ -354,51 +369,36 @@
                         alternative command name as argument, default="cd"
   -h, --help            show help/usage
   -p, --purge           just purge non-existent directories from history
   -a, --purge-always    always purge non-existent directories every write
   -g, --git             show git worktree directories instead
   -r, --git-relative    show relative git worktree paths instead of absolute
   -R, --no-git-relative
-                        do not show relative git worktree paths
+                        do not show relative git worktree paths (default)
   -u, --no-user         do not substitute "~" for home directory
-  -U, --user            do substitute "~" for home directory
+  -U, --user            do substitute "~" for home directory (default)
   -l, --list            just list directory history
   -m SIZE, --size SIZE  maximum size of directory history (default=50)
   -n NUM_LINES, --num-lines NUM_LINES
                         limit output to specified number of lines
   -L, --follow-links    follow symbolic links (default=true)
   -P, --follow-physical
                         follow links to physical directory
-  -V, --version         just output version
+  -V, --version         just output cdhist version
 
 Note you can set default options in ~/.config/cdhist-flags.conf.
 ```
 
 ## Limitations
 
 Regular `cd`, e.g. as provided by the bash builtin, offers some esoteric
 command line options such as `-e` and `-@`, and shell options such as
 `autocd`, `cdspell`, `cdable_vars`. These rarely used options are not
 supported by cdhist.
 
-## Upgrade
-
-```sh
-$ cd cdhist  # Source dir, as above
-$ git pull
-$ sudo pip3 install -U .
-```
-
-## Removal
-
-```sh
-$ unset cd
-$ sudo pip3 uninstall cdhist
-```
-
 ## Major Version Change History
 
 Version 3.0 changes and new features:
 
 1. Added function to `cd` between [`git
 worktrees`](https://git-scm.com/docs/git-worktree). Can configure this
 as separate command if preferred, with option to display relative paths.
@@ -433,15 +433,16 @@
 but now we validate it ourself before passing to `cd`. So net
 performance is quicker than previous version, at least for the vanilla
 case of changing directory. This is not noticeable on normal PC's but is
 on constrained platforms like Raspberry Pi 2/3 using SD card.
 
 12. If you were previously setting `CDHISTSIZE` or `CDHISTTILDE` settings
 via environment variables then you now need to set them using `--size`
-and `--no-user` in `~/.config/cdhist-flags.conf`.
+and `--no-user` in `~/.config/cdhist-flags.conf`, or add those options
+in your shell initialization code.
 
 13. The `-s` option to return a `cdhist.rc` file name for initialisation
 is still currently supported for backwards-compatibility but is
 undocumented and depreciated (a temporary file is created and returned).
 It will likely eventually be removed.
 
 ## License
```

### Comparing `cdhist-3.6/cdhist/cdhist.py` & `cdhist-3.7/cdhist/cdhist.py`

 * *Files 5% similar despite different names*

```diff
@@ -149,33 +149,33 @@
     opt.add_argument('-g', '--git', action='store_true',
                      help='show git worktree directories instead')
     opt.add_argument('-r', '--git-relative', action='store_true',
                      help='show relative git worktree paths instead '
                      'of absolute')
     opt.add_argument('-R', '--no-git-relative', action='store_false',
                      dest='git_relative',
-                     help='do not show relative git worktree paths')
+                     help='do not show relative git worktree paths (default)')
     opt.add_argument('-u', '--no-user', action='store_true',
                      help='do not substitute "~" for home directory')
     opt.add_argument('-U', '--user', action='store_false', dest='no_user',
-                     help='do substitute "~" for home directory')
+                     help='do substitute "~" for home directory (default)')
     opt.add_argument('-l', '--list', action='store_true',
                      help='just list directory history')
     opt.add_argument('-m', '--size', type=int, default=50,
                      help='maximum size of directory history '
                      '(default=%(default)s)')
     opt.add_argument('-n', '--num-lines', type=int, default=-1,
                      help='limit output to specified number of lines')
     opt.add_argument('-L', '--follow-links', action='store_false',
                      dest='follow_physical',
                      help='follow symbolic links (default=true)')
     opt.add_argument('-P', '--follow-physical', action='store_true',
                      help='follow links to physical directory')
     opt.add_argument('-V', '--version', action='store_true',
-                     help='just output version')
+                     help=f'just output {PROG} version')
     opt.add_argument('directory', nargs='?', help='directory (or '
                      'branch for git worktree) to cd to, '
                      'or "--" to list history and prompt, '
                      'or "-n" for n\'th entry in list '
                      'or "-/<string>" to match for "string" in dir')
 
     # Argparse will not allow "-/search" so we fudge it before arg parsing
@@ -184,30 +184,40 @@
         del sys.argv[-1]
     else:
         search = None
 
     # Merge in default args from user config file. Then parse the
     # command line.
     cnffile = CNFFILE.expanduser()
-    try:
+    if cnffile.exists():
         with cnffile.open() as fp:
-            cnflines = [re.sub(r'#.*$', '', line).strip() for line in fp]
-    except FileNotFoundError:
-        cnflines = ''
+            lines = [re.sub(r'#.*$', '', line).strip() for line in fp]
+        cnflines = ' '.join(lines).strip()
     else:
-        cnflines = ' '.join(cnflines).strip()
+        cnflines = ''
 
     args = opt.parse_args(shlex.split(cnflines) + sys.argv[1:])
 
     if args.help:
         return opt.format_help().strip()
 
     if args.version:
-        from .version import Version
-        return Version()
+        if sys.version_info >= (3, 8):
+            from importlib import metadata
+        else:
+            import importlib_metadata as metadata
+
+        pkg = Path(sys.argv[0]).stem.replace('-', '_')
+        try:
+            version = metadata.version(pkg)
+        except Exception:
+            version = '?'
+
+        print(version)
+        return
 
     # Just output shell init code if asked
     if args.init:
         print(init_code(args))
         return
 
     # This is temporary back-compatibility code until the previously
@@ -258,9 +268,7 @@
     path = str(path)
     newhist = [path] + [p for p in hist if p != path]
     write_cd_hist(newhist, args.size, args.purge_always)
     print(path)
 
 if __name__ == '__main__':
     sys.exit(main())
-
-# vim: se et:
```

### Comparing `cdhist-3.6/cdhist/git_worktree.py` & `cdhist-3.7/cdhist/git_worktree.py`

 * *Files 2% similar despite different names*

```diff
@@ -150,9 +150,7 @@
             path = utils.check_digit(arg, trees.paths) or \
                     trees.get_path_from_branch(arg)
 
     if not path:
         sys.exit(f'fatal: no worktree for "{arg}".')
 
     return path
-
-# vim: se et:
```

### Comparing `cdhist-3.6/cdhist/utils.py` & `cdhist-3.7/cdhist/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -92,9 +92,7 @@
         if match_start:
             return match_start
         elif match_any:
             return match_any
 
         if complete:
             sys.exit(f'No match on "{arg}".')
-
-# vim: se et:
```

### Comparing `cdhist-3.6/cdhist.egg-info/PKG-INFO` & `cdhist-3.7/cdhist.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 Metadata-Version: 2.1
 Name: cdhist
-Version: 3.6
+Version: 3.7
 Summary: Program to provide a Linux cd history directory stack
-Home-page: https://github.com/bulletmark/cdhist
-Author: Mark Blakeney
-Author-email: mark.blakeney@bullet-systems.net
+Author-email: Mark Blakeney <mark.blakeney@bullet-systems.net>
 License: GPLv3
-Keywords: bash zsh cd fzf git worktree
+Project-URL: Homepage, https://github.com/bulletmark/cdhist
+Keywords: bash,zsh,cd,fzf,git,worktree
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 ## Linux Directory History
 [![PyPi](https://img.shields.io/pypi/v/cdhist)](https://pypi.org/project/cdhist/)
 [![AUR](https://img.shields.io/aur/version/cdhist)](https://aur.archlinux.org/packages/cdhist/)
@@ -98,30 +97,33 @@
 
 ## Installation
 
 Arch users can install [cdhist from the
 AUR](https://aur.archlinux.org/packages/cdhist/) and skip to the next
 section.
 
-Ensure `pip3` is installed. Python 3.7 or later is required.
+Python 3.7 or later is required. Note [cdhist is on
+PyPI](https://pypi.org/project/cdhist/) so just ensure that
+[`pipx`](https://pypa.github.io/pipx/) is installed then type the
+following:
 
-Note [cdhist is on PyPI](https://pypi.org/project/cdhist/) so you can
-just type `sudo pip3 install -U cdhist`. Or do the following to install
-from this repository:
+```
+$ pipx install cdhist
+```
+
+To upgrade:
 
-```sh
-$ git clone http://github.com/bulletmark/cdhist
-$ cd cdhist
-$ sudo pip3 install -U .
+```
+$ pipx upgrade cdhist
 ```
 
 ## Setup
 
-Each user who wants to use the cdhist facility should add the following
-lines to their `~/.bashrc` or `~.zshrc` file (after where your PATH is
+A user who wants to use the cdhist facility should add the following
+lines to their `~/.bashrc` or `~/.zshrc` file (after where your PATH is
 set up so that the command `cdhist` can be found). This creates the `cd`
 wrapper command in your interactive shell session as a tiny function.
 Note you can [customize the command name](#alternative-command-name) if
 you want.
 
 ```sh
 if type cdhist &>/dev/null; then
@@ -186,15 +188,15 @@
 ## Alternative Command Name
 
 Some people may prefer not to alias their system `cd` command to this
 utility and just use an alternative unique command name. To do this,
 simply add your desired command name as an extra argument to the
 `cdhist` command in your shell initialization code. E.g, to use the
 command name `xd` rather than `cd`, use the following in
-your `~/.bashrc` or `~.zshrc` file:
+your `~/.bashrc` or `~/.zshrc` file:
 
 ```sh
 if type cdhist &>/dev/null; then
     . <(cdhist -i xd)
 fi
 ```
 
@@ -281,15 +283,15 @@
 Some users may want the git worktree functionality provided by cdhist
 but are not interested in the standard `cd` history functionality, or
 alternately, want to use a completely separate command for the git
 worktree functionality. To do this, simply add your desired command name
 and the git option as an extra argument to the `cdhist` command in your
 shell initialization code. E.g, to use the command name `wt` for git
 worktree functionality (only), add the following in your
-`~/.bashrc` or `~.zshrc` file:
+`~/.bashrc` or `~/.zshrc` file:
 
 ```sh
 if type cdhist &>/dev/null; then
     . <(cdhist -i "wt -g")
 fi
 ```
 
@@ -367,51 +369,36 @@
                         alternative command name as argument, default="cd"
   -h, --help            show help/usage
   -p, --purge           just purge non-existent directories from history
   -a, --purge-always    always purge non-existent directories every write
   -g, --git             show git worktree directories instead
   -r, --git-relative    show relative git worktree paths instead of absolute
   -R, --no-git-relative
-                        do not show relative git worktree paths
+                        do not show relative git worktree paths (default)
   -u, --no-user         do not substitute "~" for home directory
-  -U, --user            do substitute "~" for home directory
+  -U, --user            do substitute "~" for home directory (default)
   -l, --list            just list directory history
   -m SIZE, --size SIZE  maximum size of directory history (default=50)
   -n NUM_LINES, --num-lines NUM_LINES
                         limit output to specified number of lines
   -L, --follow-links    follow symbolic links (default=true)
   -P, --follow-physical
                         follow links to physical directory
-  -V, --version         just output version
+  -V, --version         just output cdhist version
 
 Note you can set default options in ~/.config/cdhist-flags.conf.
 ```
 
 ## Limitations
 
 Regular `cd`, e.g. as provided by the bash builtin, offers some esoteric
 command line options such as `-e` and `-@`, and shell options such as
 `autocd`, `cdspell`, `cdable_vars`. These rarely used options are not
 supported by cdhist.
 
-## Upgrade
-
-```sh
-$ cd cdhist  # Source dir, as above
-$ git pull
-$ sudo pip3 install -U .
-```
-
-## Removal
-
-```sh
-$ unset cd
-$ sudo pip3 uninstall cdhist
-```
-
 ## Major Version Change History
 
 Version 3.0 changes and new features:
 
 1. Added function to `cd` between [`git
 worktrees`](https://git-scm.com/docs/git-worktree). Can configure this
 as separate command if preferred, with option to display relative paths.
@@ -446,15 +433,16 @@
 but now we validate it ourself before passing to `cd`. So net
 performance is quicker than previous version, at least for the vanilla
 case of changing directory. This is not noticeable on normal PC's but is
 on constrained platforms like Raspberry Pi 2/3 using SD card.
 
 12. If you were previously setting `CDHISTSIZE` or `CDHISTTILDE` settings
 via environment variables then you now need to set them using `--size`
-and `--no-user` in `~/.config/cdhist-flags.conf`.
+and `--no-user` in `~/.config/cdhist-flags.conf`, or add those options
+in your shell initialization code.
 
 13. The `-s` option to return a `cdhist.rc` file name for initialisation
 is still currently supported for backwards-compatibility but is
 undocumented and depreciated (a temporary file is created and returned).
 It will likely eventually be removed.
 
 ## License
```

