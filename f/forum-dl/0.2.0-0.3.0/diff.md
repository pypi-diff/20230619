# Comparing `tmp/forum_dl-0.2.0.tar.gz` & `tmp/forum_dl-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "forum_dl-0.2.0.tar", last modified: Fri May 26 17:46:54 2023, max compression
+gzip compressed data, was "forum_dl-0.3.0.tar", last modified: Mon Jun 19 21:08:23 2023, max compression
```

## Comparing `forum_dl-0.2.0.tar` & `forum_dl-0.3.0.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-05-26 17:46:54.116119 forum_dl-0.2.0/
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1072 2023-02-05 02:04:17.000000 forum_dl-0.2.0/LICENSE
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     4939 2023-05-26 17:46:54.116119 forum_dl-0.2.0/PKG-INFO
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     4323 2023-05-26 17:36:07.000000 forum_dl-0.2.0/README.md
-drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-05-26 17:46:54.112786 forum_dl-0.2.0/forum_dl/
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1776 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/__init__.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       85 2023-05-18 01:32:50.000000 forum_dl-0.2.0/forum_dl/__main__.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      489 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/exceptions.py
-drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-05-26 17:46:54.116119 forum_dl-0.2.0/forum_dl/extractors/
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1244 2023-04-26 17:47:41.000000 forum_dl-0.2.0/forum_dl/extractors/__init__.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    10283 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/extractors/common.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     8521 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/extractors/discourse.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    10911 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/extractors/hackernews.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    11669 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/extractors/hyperkitty.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     7394 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/extractors/hypermail.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     8648 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/extractors/invision.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    13814 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/extractors/phpbb.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    11956 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/extractors/pipermail.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    13624 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/extractors/proboards.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    17288 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/extractors/simplemachines.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    14240 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/extractors/vbulletin.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    14012 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/extractors/xenforo.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1475 2023-05-18 18:51:44.000000 forum_dl-0.2.0/forum_dl/forumdl.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     4323 2023-05-26 17:33:51.000000 forum_dl-0.2.0/forum_dl/options.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     4780 2023-05-26 01:03:43.000000 forum_dl-0.2.0/forum_dl/session.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     5207 2023-05-18 23:13:35.000000 forum_dl-0.2.0/forum_dl/soup.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       93 2023-04-20 02:45:45.000000 forum_dl-0.2.0/forum_dl/version.py
-drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-05-26 17:46:54.116119 forum_dl-0.2.0/forum_dl/writers/
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1057 2023-05-26 01:03:26.000000 forum_dl-0.2.0/forum_dl/writers/__init__.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      487 2023-04-28 23:15:46.000000 forum_dl-0.2.0/forum_dl/writers/babyl.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     8243 2023-05-21 03:00:29.000000 forum_dl-0.2.0/forum_dl/writers/common.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      293 2023-05-04 19:53:33.000000 forum_dl-0.2.0/forum_dl/writers/jsonl.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      544 2023-04-28 23:39:06.000000 forum_dl-0.2.0/forum_dl/writers/maildir.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      466 2023-04-28 23:15:14.000000 forum_dl-0.2.0/forum_dl/writers/mbox.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      519 2023-04-28 23:39:11.000000 forum_dl-0.2.0/forum_dl/writers/mh.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      482 2023-04-28 23:15:32.000000 forum_dl-0.2.0/forum_dl/writers/mmdf.py
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      278 2023-05-26 01:03:30.000000 forum_dl-0.2.0/forum_dl/writers/warc.py
-drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-05-26 17:46:54.112786 forum_dl-0.2.0/forum_dl.egg-info/
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     4939 2023-05-26 17:46:54.000000 forum_dl-0.2.0/forum_dl.egg-info/PKG-INFO
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1047 2023-05-26 17:46:54.000000 forum_dl-0.2.0/forum_dl.egg-info/SOURCES.txt
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        1 2023-05-26 17:46:54.000000 forum_dl-0.2.0/forum_dl.egg-info/dependency_links.txt
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       52 2023-05-26 17:46:54.000000 forum_dl-0.2.0/forum_dl.egg-info/entry_points.txt
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       92 2023-05-26 17:46:54.000000 forum_dl-0.2.0/forum_dl.egg-info/requires.txt
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        9 2023-05-26 17:46:54.000000 forum_dl-0.2.0/forum_dl.egg-info/top_level.txt
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      992 2023-05-26 17:46:46.000000 forum_dl-0.2.0/pyproject.toml
--rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       38 2023-05-26 17:46:54.116119 forum_dl-0.2.0/setup.cfg
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-06-19 21:08:23.715952 forum_dl-0.3.0/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1072 2023-02-05 02:04:17.000000 forum_dl-0.3.0/LICENSE
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     5649 2023-06-19 21:08:23.715952 forum_dl-0.3.0/PKG-INFO
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     5035 2023-06-14 22:22:07.000000 forum_dl-0.3.0/README.md
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-06-19 21:08:23.712618 forum_dl-0.3.0/forum_dl/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     2062 2023-06-14 01:13:15.000000 forum_dl-0.3.0/forum_dl/__init__.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       85 2023-05-18 01:32:50.000000 forum_dl-0.3.0/forum_dl/__main__.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      489 2023-05-31 21:05:25.000000 forum_dl-0.3.0/forum_dl/exceptions.py
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-06-19 21:08:23.712618 forum_dl-0.3.0/forum_dl/extractors/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1244 2023-05-31 21:05:25.000000 forum_dl-0.3.0/forum_dl/extractors/__init__.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    16992 2023-06-18 22:31:38.000000 forum_dl-0.3.0/forum_dl/extractors/common.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     8568 2023-06-17 17:59:10.000000 forum_dl-0.3.0/forum_dl/extractors/discourse.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    10987 2023-05-31 22:32:23.000000 forum_dl-0.3.0/forum_dl/extractors/hackernews.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    11838 2023-05-31 22:32:23.000000 forum_dl-0.3.0/forum_dl/extractors/hyperkitty.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     7422 2023-06-17 00:36:49.000000 forum_dl-0.3.0/forum_dl/extractors/hypermail.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     7989 2023-06-17 18:09:55.000000 forum_dl-0.3.0/forum_dl/extractors/invision.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    16249 2023-06-15 20:49:58.000000 forum_dl-0.3.0/forum_dl/extractors/phpbb.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    11967 2023-06-17 00:36:49.000000 forum_dl-0.3.0/forum_dl/extractors/pipermail.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    12742 2023-06-18 22:32:38.000000 forum_dl-0.3.0/forum_dl/extractors/proboards.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    15757 2023-06-17 22:49:42.000000 forum_dl-0.3.0/forum_dl/extractors/simplemachines.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    13576 2023-06-17 00:37:18.000000 forum_dl-0.3.0/forum_dl/extractors/vbulletin.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    15275 2023-06-17 00:37:18.000000 forum_dl-0.3.0/forum_dl/extractors/xenforo.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1475 2023-05-31 21:05:25.000000 forum_dl-0.3.0/forum_dl/forumdl.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     5425 2023-06-14 22:20:38.000000 forum_dl-0.3.0/forum_dl/options.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     5366 2023-06-18 18:58:29.000000 forum_dl-0.3.0/forum_dl/session.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     5496 2023-06-18 18:58:11.000000 forum_dl-0.3.0/forum_dl/soup.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       93 2023-04-20 02:45:45.000000 forum_dl-0.3.0/forum_dl/version.py
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-06-19 21:08:23.715952 forum_dl-0.3.0/forum_dl/writers/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1057 2023-05-31 21:05:25.000000 forum_dl-0.3.0/forum_dl/writers/__init__.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      556 2023-06-11 23:58:32.000000 forum_dl-0.3.0/forum_dl/writers/babyl.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)    12885 2023-06-19 00:20:23.000000 forum_dl-0.3.0/forum_dl/writers/common.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      256 2023-06-06 18:57:42.000000 forum_dl-0.3.0/forum_dl/writers/jsonl.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      613 2023-06-11 23:58:32.000000 forum_dl-0.3.0/forum_dl/writers/maildir.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      535 2023-06-11 23:58:32.000000 forum_dl-0.3.0/forum_dl/writers/mbox.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      588 2023-06-11 23:58:32.000000 forum_dl-0.3.0/forum_dl/writers/mh.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      551 2023-06-11 23:58:32.000000 forum_dl-0.3.0/forum_dl/writers/mmdf.py
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      278 2023-05-26 01:03:30.000000 forum_dl-0.3.0/forum_dl/writers/warc.py
+drwxr-xr-x   0 mikolaj   (1000) mikolaj   (1000)        0 2023-06-19 21:08:23.712618 forum_dl-0.3.0/forum_dl.egg-info/
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     5649 2023-06-19 21:08:23.000000 forum_dl-0.3.0/forum_dl.egg-info/PKG-INFO
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1047 2023-06-19 21:08:23.000000 forum_dl-0.3.0/forum_dl.egg-info/SOURCES.txt
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        1 2023-06-19 21:08:23.000000 forum_dl-0.3.0/forum_dl.egg-info/dependency_links.txt
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       52 2023-06-19 21:08:23.000000 forum_dl-0.3.0/forum_dl.egg-info/entry_points.txt
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)      112 2023-06-19 21:08:23.000000 forum_dl-0.3.0/forum_dl.egg-info/requires.txt
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)        9 2023-06-19 21:08:23.000000 forum_dl-0.3.0/forum_dl.egg-info/top_level.txt
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)     1013 2023-06-19 21:06:42.000000 forum_dl-0.3.0/pyproject.toml
+-rw-r--r--   0 mikolaj   (1000) mikolaj   (1000)       38 2023-06-19 21:08:23.715952 forum_dl-0.3.0/setup.cfg
```

### Comparing `forum_dl-0.2.0/LICENSE` & `forum_dl-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `forum_dl-0.2.0/PKG-INFO` & `forum_dl-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: forum_dl
-Version: 0.2.0
-Summary: Download posts and threads from forums, news aggregators, mail archives
+Version: 0.3.0
+Summary: Scrape posts and threads from forums, news aggregators, mail archives
 Author-email: Mikolaj Wielgus <wielgusmikolaj@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/mikwielgus/forum-dl
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -21,44 +21,44 @@
 
 <sub>The project is currently in alpha stage. Please do not hesitate to [file](https://github.com/mikwielgus/forum-dl/issues) bug reports and feature requests.</sub>
 
 ![image](https://github.com/mikwielgus/forum-dl/assets/58011230/e677d1aa-efa3-4cfc-9283-38408842b278)
 
 # Installation
 
-You can install Forum-dl from [PIP](#pip) or directly from the [repository](#repository).
+You can install stable Forum-dl from [PIP](#pip) or directly from the [repository](#repository).
 
 ## PIP
 
-Install the latest stable version of Forum-dl from PIP:
+Install the latest stable version from PIP:
 
 ```
 pip install forum-dl
 ```
 
 ## Repository 
 
-Clone the repository and install it in editable mode:
+Clone the repository and install the development branch in editable mode:
 
 ```
 git clone https://github.com/mikwielgus/forum-dl && pip install -e forum-dl
 ```
 
 # Usage examples
 
 Download a Simple Machines Forum thread in JSONL format:
 
 ```
 forum-dl "https://www.simplemachines.org/community/index.php?topic=584230.0"
 ```
 
-Download an entire PhpBB board into JSONL format, write to stdout (`-o -`) and record a WARC file in `phpbb.warc`:
+Download a PhpBB subboard into JSONL format, write to stdout (`-o -`) and record a WARC file in `phpbb.warc`:
 
 ```
-forum-dl -o - "https://www.phpbb.com/community/viewforum.php?f=696"
+forum-dl -o - --warc-output phpbb.warc "https://www.phpbb.com/community/viewforum.php?f=696"
 ```
 
 <sub>(due to current architectural limitations, `forum-dl` will scan the first page of each board in the entire forum before downloading the target board. This will be fixed in future releases)</sub>
 
 Download Hacker News top stories and write them to a Maildir directory `hn`:
 
 ```
@@ -95,17 +95,18 @@
 - MH
 - MMDF
 - WARC
 
 # Usage
 
 ```
-forum-dl [--help] [--version] [--list-extractors] [--list-output-formats] [-R RETRIES] [--retry-sleep RETRY_SLEEP]
-         [--retry-sleep-multiplier RETRY_SLEEP_MULTIPLIER] [--user-agent USER_AGENT] [-q] [-v] [-g] [-o FILE] [-f FORMAT]
-         [--warc-output FILE] [--no-boards] [--no-threads] [--no-posts] [--textify] [--content-as-title]
+forum-dl [--help] [--version] [--list-extractors] [--list-output-formats] [--timeout SECONDS] [-R N] [--retry-sleep SECONDS]
+         [--retry-sleep-multiplier K] [--user-agent UA] [-q] [-v] [-g] [-o OUTFILE] [-f FORMAT] [--warc-output FILE]
+         [--files-output DIR] [--boards | --no-boards] [--threads | --no-threads] [--posts | --no-posts]
+         [--files | --no-files] [--outside-files | --no-outside-files] [--textify] [--content-as-title]
          [--author-as-addr-spec]
 ```
 
 ## General Options:
 
 ```
   --help                Show this help message and exit
@@ -114,34 +115,42 @@
   --list-output-formats
                         List all supported output formats and exit
 ```
 
 ## Session Options:
 
 ```
+  --timeout SECONDS     HTTP connection timeout
   -R N, --retries N     Maximum number of retries for failed HTTP requests or -1 to retry infinitely (default: 4)
   --retry-sleep SECONDS
                         Time to sleep between retries, in seconds (default: 1)
   --retry-sleep-multiplier K
                         A constant by which sleep time is multiplied on each retry (default: 2)
   --user-agent UA       User-Agent request header
 ```
 
 ## Output Options:
 
 ```
   -q, --quiet           Activate quiet mode
   -v, --verbose         Print various debugging information
   -g, --get-urls        Print URLs instead of downloading
-  -o FILE, --output FILE
-                        Output all results concatenated to FILE, or stdout if FILE is -
+  -o OUTFILE, --output OUTFILE
+                        Output all results concatenated to OUTFILE, or stdout if OUTFILE is - (default: -)
   -f FORMAT, --output-format FORMAT
                         Output format. Use --list-output-formats for a list of possible arguments
   --warc-output FILE    Record HTTP requests, store them in FILE in WARC format
-  --no-boards           Do not write board objects
-  --no-threads          Do not write thread objects
-  --no-posts            Do not write post objects
+  --files-output DIR    Store files in DIR instead of OUTFILE
+  --boards, --no-boards
+                        Write board objects (default: True, --no-boards to negate)
+  --threads, --no-threads
+                        Write thread objects (default: True, --no-threads to negate)
+  --posts, --no-posts   Write post objects (default: True, --no-posts to negate)
+  --files, --no-files   Write embedded files (--no-files to negate)
+  --outside-files, --no-outside-files
+                        Write embedded files outside post content. Auto-enabled by --warc-output and -f warc (default: False, --no-
+                        outside-files to negate)
   --textify             Lossily convert HTML content to plaintext
   --content-as-title    Write 98 initial characters of content in title field of each post
   --author-as-addr-spec
                         Append author and domain as an addr-spec in the From header
 ```
```

### Comparing `forum_dl-0.2.0/README.md` & `forum_dl-0.3.0/README.md`

 * *Files 12% similar despite different names*

```diff
@@ -4,44 +4,44 @@
 
 <sub>The project is currently in alpha stage. Please do not hesitate to [file](https://github.com/mikwielgus/forum-dl/issues) bug reports and feature requests.</sub>
 
 ![image](https://github.com/mikwielgus/forum-dl/assets/58011230/e677d1aa-efa3-4cfc-9283-38408842b278)
 
 # Installation
 
-You can install Forum-dl from [PIP](#pip) or directly from the [repository](#repository).
+You can install stable Forum-dl from [PIP](#pip) or directly from the [repository](#repository).
 
 ## PIP
 
-Install the latest stable version of Forum-dl from PIP:
+Install the latest stable version from PIP:
 
 ```
 pip install forum-dl
 ```
 
 ## Repository 
 
-Clone the repository and install it in editable mode:
+Clone the repository and install the development branch in editable mode:
 
 ```
 git clone https://github.com/mikwielgus/forum-dl && pip install -e forum-dl
 ```
 
 # Usage examples
 
 Download a Simple Machines Forum thread in JSONL format:
 
 ```
 forum-dl "https://www.simplemachines.org/community/index.php?topic=584230.0"
 ```
 
-Download an entire PhpBB board into JSONL format, write to stdout (`-o -`) and record a WARC file in `phpbb.warc`:
+Download a PhpBB subboard into JSONL format, write to stdout (`-o -`) and record a WARC file in `phpbb.warc`:
 
 ```
-forum-dl -o - "https://www.phpbb.com/community/viewforum.php?f=696"
+forum-dl -o - --warc-output phpbb.warc "https://www.phpbb.com/community/viewforum.php?f=696"
 ```
 
 <sub>(due to current architectural limitations, `forum-dl` will scan the first page of each board in the entire forum before downloading the target board. This will be fixed in future releases)</sub>
 
 Download Hacker News top stories and write them to a Maildir directory `hn`:
 
 ```
@@ -78,17 +78,18 @@
 - MH
 - MMDF
 - WARC
 
 # Usage
 
 ```
-forum-dl [--help] [--version] [--list-extractors] [--list-output-formats] [-R RETRIES] [--retry-sleep RETRY_SLEEP]
-         [--retry-sleep-multiplier RETRY_SLEEP_MULTIPLIER] [--user-agent USER_AGENT] [-q] [-v] [-g] [-o FILE] [-f FORMAT]
-         [--warc-output FILE] [--no-boards] [--no-threads] [--no-posts] [--textify] [--content-as-title]
+forum-dl [--help] [--version] [--list-extractors] [--list-output-formats] [--timeout SECONDS] [-R N] [--retry-sleep SECONDS]
+         [--retry-sleep-multiplier K] [--user-agent UA] [-q] [-v] [-g] [-o OUTFILE] [-f FORMAT] [--warc-output FILE]
+         [--files-output DIR] [--boards | --no-boards] [--threads | --no-threads] [--posts | --no-posts]
+         [--files | --no-files] [--outside-files | --no-outside-files] [--textify] [--content-as-title]
          [--author-as-addr-spec]
 ```
 
 ## General Options:
 
 ```
   --help                Show this help message and exit
@@ -97,34 +98,42 @@
   --list-output-formats
                         List all supported output formats and exit
 ```
 
 ## Session Options:
 
 ```
+  --timeout SECONDS     HTTP connection timeout
   -R N, --retries N     Maximum number of retries for failed HTTP requests or -1 to retry infinitely (default: 4)
   --retry-sleep SECONDS
                         Time to sleep between retries, in seconds (default: 1)
   --retry-sleep-multiplier K
                         A constant by which sleep time is multiplied on each retry (default: 2)
   --user-agent UA       User-Agent request header
 ```
 
 ## Output Options:
 
 ```
   -q, --quiet           Activate quiet mode
   -v, --verbose         Print various debugging information
   -g, --get-urls        Print URLs instead of downloading
-  -o FILE, --output FILE
-                        Output all results concatenated to FILE, or stdout if FILE is -
+  -o OUTFILE, --output OUTFILE
+                        Output all results concatenated to OUTFILE, or stdout if OUTFILE is - (default: -)
   -f FORMAT, --output-format FORMAT
                         Output format. Use --list-output-formats for a list of possible arguments
   --warc-output FILE    Record HTTP requests, store them in FILE in WARC format
-  --no-boards           Do not write board objects
-  --no-threads          Do not write thread objects
-  --no-posts            Do not write post objects
+  --files-output DIR    Store files in DIR instead of OUTFILE
+  --boards, --no-boards
+                        Write board objects (default: True, --no-boards to negate)
+  --threads, --no-threads
+                        Write thread objects (default: True, --no-threads to negate)
+  --posts, --no-posts   Write post objects (default: True, --no-posts to negate)
+  --files, --no-files   Write embedded files (--no-files to negate)
+  --outside-files, --no-outside-files
+                        Write embedded files outside post content. Auto-enabled by --warc-output and -f warc (default: False, --no-
+                        outside-files to negate)
   --textify             Lossily convert HTML content to plaintext
   --content-as-title    Write 98 initial characters of content in title field of each post
   --author-as-addr-spec
                         Append author and domain as an addr-spec in the From header
 ```
```

### Comparing `forum_dl-0.2.0/forum_dl/__init__.py` & `forum_dl-0.3.0/forum_dl/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,32 +25,37 @@
     elif not args.urls:
         parser.error(
             "The following arguments are required: URL\n"
             "Use 'forum-dl --help' to get a list of all options."
         )
     else:
         warc_output = args.output if args.output_format == "warc" else args.warc_output
+        write_outside_file_objects = args.outside_files or bool(warc_output)
 
         forumdl.download(
             urls=args.urls,
             output_format=args.output_format,
             session_options=SessionOptions(
+                timeout=args.timeout,
                 retries=args.retries,
                 retry_sleep=args.retry_sleep,
                 retry_sleep_multiplier=args.retry_sleep_multiplier,
                 warc_output=warc_output,
                 user_agent=args.user_agent,
                 get_urls=args.get_urls,
             ),
             extractor_options=ExtractorOptions(
                 path=False,
             ),
             writer_options=WriterOptions(
                 output_path=args.output,
+                files_output_path=args.files_output,
                 write_board_objects=args.boards,
                 write_thread_objects=args.threads,
                 write_post_objects=args.posts,
+                write_file_objects=args.files,
+                write_outside_file_objects=write_outside_file_objects,
                 textify=args.textify,
                 content_as_title=args.content_as_title,
                 author_as_addr_spec=args.author_as_addr_spec,
             ),
         )
```

### Comparing `forum_dl-0.2.0/forum_dl/extractors/__init__.py` & `forum_dl-0.3.0/forum_dl/extractors/__init__.py`

 * *Files identical despite different names*

### Comparing `forum_dl-0.2.0/forum_dl/extractors/common.py` & `forum_dl-0.3.0/forum_dl/extractors/common.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 # pyright: strict
 from __future__ import annotations
 from typing import *  # type: ignore
 
 from abc import ABC, abstractmethod
-from dataclasses import dataclass
-from urllib.parse import urlparse, urlunparse, parse_qs, urlencode
+from pydantic import BaseModel
+from urllib.parse import urljoin, urlparse, urlunparse, parse_qs, urlencode
 from pathlib import PurePosixPath
 import logging
 import traceback
 
 from ..session import Session
-from ..exceptions import SearchError
+from ..soup import Soup, SoupTag
+from ..exceptions import AttributeSearchError, SearchError
 from ..version import __version__
 
+if TYPE_CHECKING:
+    from requests import Response
+
 
 def get_relative_url(url: str, base_url: str):
     parsed_base_url = urlparse(base_url)
     parsed_url = urlparse(url)
 
     base_path = PurePosixPath(str(parsed_base_url.path))
     path = PurePosixPath(str(parsed_url.path))
@@ -79,50 +83,52 @@
 
         if result:
             return result
 
     raise ValueError
 
 
-@dataclass
-class ExtractorOptions:
+class ExtractorOptions(BaseModel):
     path: bool
 
 
-@dataclass  # (kw_only=True)
-class PageState:
+class PageState(BaseModel):
     url: str
+    page: int
 
 
-@dataclass
-class Item:
+class Item(BaseModel):
     path: tuple[str, ...]
     url: str
     origin: str
     data: dict[str, Any]
 
 
-@dataclass
 class Post(Item):
     subpath: tuple[str, ...]
     author: str
     creation_time: str
     content: str
 
 
-@dataclass
 class Thread(Item):
     title: str
 
 
-@dataclass
 class Board(Item):
     title: str
 
 
+class File(Item):
+    subpath: tuple[str, ...]
+    content_type: str | None = None
+    content: bytes | None = None
+    os_path: str | None = None
+
+
 class Extractor(ABC):
     tests: list[dict[str, Any]]
 
     @final
     @classmethod
     def detect(
         cls, session: Session, url: str, options: ExtractorOptions
@@ -301,63 +307,257 @@
 
     @abstractmethod
     def _fetch_lazy_subboards(self, board: Board) -> Generator[Board, None, None]:
         self._do_fetch_subboards(board)
         return iter(self._subboards[board.path])
 
     @final
+    def board_count(self):
+        return len(self._boards)
+
+    @final
     def subboards(self, board: Board):
         if not self._are_subboards_fetched[board.path]:
             for _ in self._fetch_lazy_subboards(board):
                 pass
 
             self._are_subboards_fetched[board.path] = True
 
         return self._subboards[board.path]
 
     @abstractmethod
     def _fetch_board_page_threads(
         self, board: Board, state: PageState
-    ) -> Generator[Thread, None, PageState | None]:
+    ) -> Generator[Thread | File, None, PageState | None]:
         pass
 
     @final
     def _fetch_board_threads(
         self, board: Board, initial_state: PageState | None = None
     ):
         try:
-            self.board_state = initial_state or PageState(url=board.url)
+            self.board_state = initial_state or PageState(url=board.url, page=1)
             while self.board_state:
                 self.board_state = yield from self._fetch_board_page_threads(
                     board, self.board_state
                 )
         except Exception as e:
             logging.warning(repr(e))
             logging.warning(traceback.format_exc())
 
     @abstractmethod
     def _fetch_thread_page_posts(
         self, thread: Thread, state: PageState
-    ) -> Generator[Post, None, PageState | None]:
+    ) -> Generator[Post | File, None, PageState | None]:
         pass
 
     @final
     def _fetch_thread_posts(
         self, thread: Thread, initial_state: PageState | None = None
     ):
         try:
-            self.thread_state = initial_state or PageState(url=thread.url)
+            self.thread_state = initial_state or PageState(url=thread.url, page=1)
             while self.thread_state:
                 self.thread_state = yield from self._fetch_thread_page_posts(
                     thread, self.thread_state
                 )
         except Exception as e:
             logging.warning(repr(e))
             logging.warning(traceback.format_exc())
 
     @final
     def threads(self, board: Board, initial_state: PageState | None = None):
+        for item in self._fetch_board_threads(board, initial_state):
+            # if isinstance(item, Thread):
+            match item:
+                case Thread():
+                    yield item
+                case File():
+                    pass
+
+    @final
+    def threads_with_files(self, board: Board, initial_state: PageState | None = None):
         yield from self._fetch_board_threads(board, initial_state)
 
     @final
     def posts(self, thread: Thread, initial_state: PageState | None = None):
+        for item in self._fetch_thread_posts(thread, initial_state):
+            match item:
+                case Post():
+                    yield item
+                case File():
+                    pass
+
+    @final
+    def posts_with_files(self, thread: Thread, initial_state: PageState | None = None):
         yield from self._fetch_thread_posts(thread, initial_state)
+
+    @final
+    def download_file(self, file: File):
+        try:
+            return self._session.try_get(file.url, should_cache=True)
+        except Exception as e:
+            logging.warning(repr(e))
+            logging.warning(traceback.format_exc())
+
+
+class HtmlExtractor(Extractor):
+    _board_item_css: str
+    _board_next_page_css: str
+    _thread_item_css: str
+    _thread_next_page_css: str
+
+    @final
+    def _fetch_board_page_threads(self, board: Board, state: PageState):
+        response = self._session.get(state.url)
+        soup = Soup(response.content)
+
+        for tag in soup.soup.select(self._board_item_css):
+            if thread := self._extract_board_page_thread(
+                board, state, response, SoupTag(tag)
+            ):
+                yield thread
+
+        yield from self._extract_file_objects((), (), soup, response)
+        return self._extract_board_next_page_state(board, state, response, soup)
+
+    @abstractmethod
+    def _extract_board_page_thread(
+        self, board: Board, state: PageState, response: Response, tag: SoupTag
+    ) -> Thread | None:
+        pass
+
+    def _extract_board_next_page_state(
+        self, board: Board, state: PageState, response: Response, soup: Soup
+    ):
+        if next_page_tag := soup.soup.select_one(self._board_next_page_css):
+            href = cast(str, next_page_tag.get("href"))
+
+            return PageState(url=urljoin(response.url, href), page=state.page + 1)
+
+    @final
+    def _fetch_thread_page_posts(self, thread: Thread, state: PageState):
+        response = self._session.get(state.url)
+        soup = Soup(response.content)
+
+        content_file_urls: list[str] = []
+
+        for tag in soup.soup.select(self._thread_item_css):
+            if post := self._extract_thread_page_post(
+                thread, state, response, SoupTag(tag)
+            ):
+                yield post
+
+                # TODO: Don't reparse text.
+                new_content_file_urls = yield from self._extract_file_objects(
+                    post.path, post.subpath, Soup(post.content), response
+                )
+                content_file_urls.extend(new_content_file_urls)
+
+        for file in self._extract_file_objects((), (), soup, response):
+            if file.url not in content_file_urls:
+                yield file
+
+        return self._extract_thread_next_page_state(thread, state, response, soup)
+
+    @abstractmethod
+    def _extract_thread_page_post(
+        self, thread: Thread, state: PageState, response: Response, tag: SoupTag
+    ) -> Post | None:
+        pass
+
+    def _extract_thread_next_page_state(
+        self, thread: Thread, state: PageState, response: Response, soup: Soup
+    ):
+        if next_page_tag := soup.soup.select_one(self._thread_next_page_css):
+            href = cast(str, next_page_tag.get("href"))
+
+            if not href:
+                return
+
+            return PageState(url=urljoin(response.url, href), page=state.page + 1)
+
+    @final
+    def _extract_file_objects(
+        self,
+        path: tuple[str, ...],
+        subpath: tuple[str, ...],
+        soup_or_tag: Soup | SoupTag,
+        response: Response,
+    ):
+        match soup_or_tag:
+            case Soup():
+                obj = soup_or_tag.soup
+            case SoupTag():
+                obj = soup_or_tag.tag
+
+        embeds = obj.select(
+            'link[rel="stylesheet"], embed, audio, img, object, svg, video'
+        )
+
+        urls: list[str] = []
+
+        for embed in embeds:
+            embed = SoupTag(embed)
+            url = None
+
+            if embed.tag.name == "link":
+                url = urljoin(response.url, embed.get("href"))
+                yield File(
+                    path=path,
+                    url=url,
+                    origin=response.url,
+                    data={},
+                    subpath=subpath + (url,),
+                )
+            elif embed.tag.name == "embed":
+                url = urljoin(response.url, embed.get("src"))
+                yield File(
+                    path=path,
+                    url=url,
+                    origin=response.url,
+                    data={},
+                    subpath=subpath + (url,),
+                )
+            elif embed.tag.name == "audio":
+                for source in embed.tag.find_all("source"):
+                    url = urljoin(response.url, source.get("src"))
+                    yield File(
+                        path=path,
+                        url=url,
+                        origin=response.url,
+                        data={},
+                        subpath=subpath + (url,),
+                    )
+            elif embed.tag.name == "img":
+                url = urljoin(response.url, embed.get("src"))
+                yield File(
+                    path=path,
+                    url=url,
+                    origin=response.url,
+                    data={},
+                    subpath=subpath + (url,),
+                )
+            elif embed.tag.name == "object":
+                url = urljoin(response.url, embed.get("data"))
+                yield File(
+                    path=path,
+                    url=url,
+                    origin=response.url,
+                    data={},
+                    subpath=subpath + (url,),
+                )
+            elif embed.tag.name == "svg":
+                yield File(
+                    path=path,
+                    url=response.url,
+                    origin=response.url,
+                    data={},
+                    subpath=subpath,
+                    content_type="image/svg+xml",
+                    content=embed.encode_contents(),
+                )
+
+            if url:
+                urls.append(url)
+
+        return urls
```

### Comparing `forum_dl-0.2.0/forum_dl/extractors/discourse.py` & `forum_dl-0.3.0/forum_dl/extractors/discourse.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,20 @@
 # pyright: strict
 from __future__ import annotations
 from typing import *  # type: ignore
 
 from pathlib import PurePosixPath
 from urllib.parse import urljoin, urlparse, urlunparse
-from dataclasses import dataclass
 
 from .common import get_relative_url, normalize_url
 from .common import Extractor, ExtractorOptions, Board, Thread, Post, PageState
 from ..session import Session
 from ..soup import Soup
 
 
-@dataclass
 class DiscourseThreadPageState(PageState):
     stream_data: list[int]
 
 
 class DiscourseExtractor(Extractor):
     tests = [
         {
@@ -43,15 +41,15 @@
                     "path": ("67", "68629"),
                 }
             },
         },
         {
             "url": "https://meta.discourse.org/t/welcome-to-meta-discourse-org/1",
             "test_base_url": "https://meta.discourse.org/",
-            "test_contents_hash": "36eab8dfa910b45bf8757d5d977743b90405f53f",
+            "test_contents_hash": "99f7dcb83911feeeda5c45b1ff4b0f5ec31468bc",
             "test_item_count": 1,
         },
         {
             "url": "https://meta.discourse.org/t/try-out-the-new-sidebar-and-notification-menus/238821",
             "test_base_url": "https://meta.discourse.org/",
             "test_min_item_count": 200,
         },
@@ -191,24 +189,27 @@
         if more_topics_url := page_json["topic_list"].get("more_topics_url", None):
             parsed_more_topics_url = urlparse(str(more_topics_url))
             parsed_more_topics_url = parsed_more_topics_url._replace(
                 path=f"{parsed_more_topics_url.path}.json"
             )
 
             return PageState(
-                url=urljoin(self.base_url, str(urlunparse(parsed_more_topics_url)))
+                url=urljoin(self.base_url, str(urlunparse(parsed_more_topics_url))),
+                page=state.page + 1,
             )
 
     def _fetch_thread_page_posts(self, thread: Thread, state: PageState):
         if state.url == thread.url:
             json_url = f"{state.url}.json"
             response = self._session.get(json_url)
             page_json = response.json()
             state = DiscourseThreadPageState(
-                url=response.url, stream_data=page_json["post_stream"]["stream"]
+                url=response.url,
+                stream_data=page_json["post_stream"]["stream"],
+                page=state.page + 1,
             )
         else:
             origin = state.url
             state = cast(DiscourseThreadPageState, state)
             post_ids = tuple(state.stream_data[:20])
             response = self._session.get(
                 origin,
```

### Comparing `forum_dl-0.2.0/forum_dl/extractors/hackernews.py` & `forum_dl-0.3.0/forum_dl/extractors/hackernews.py`

 * *Files 4% similar despite different names*

```diff
@@ -24,15 +24,17 @@
             "test_base_url": "https://news.ycombinator.com/",
             "test_contents_hash": "ead3fec1c434236fb09995727cb02c4b7e7dc3ca",
             "test_item_count": 18,
         },
         {
             "url": "https://news.ycombinator.com",
             "test_base_url": "https://news.ycombinator.com/",
-            "initial_page": PageState(url="https://news.ycombinator.com/item?id=1000"),
+            "initial_page": PageState(
+                url="https://news.ycombinator.com/item?id=1000", page=1
+            ),
             "item_count": 5,
             "test_titles_hash": "bd1ab966ced8daf8c68cc5ad9e51a7bd6c7b622c",
             "test_item_count": 5,
         },
         {
             "url": "https://news.ycombinator.com/newest",
             "test_base_url": "https://news.ycombinator.com/",
@@ -209,15 +211,16 @@
                 continue
 
             yield self._fetch_item_thread(item_id)
 
         if page_id > 0:
             new_state_item_id = self._calc_first_item_id(page_id) - 1
             return PageState(
-                url=f"https://news.ycombinator.com/item?id={new_state_item_id}"
+                url=f"https://news.ycombinator.com/item?id={new_state_item_id}",
+                page=state.page + 1,
             )
 
     def _fetch_thread_page_posts(self, thread: Thread, state: PageState):
         post_paths: list[tuple[str, ...]] = [()]
 
         i = 0
         while True:
```

### Comparing `forum_dl-0.2.0/forum_dl/extractors/hyperkitty.py` & `forum_dl-0.3.0/forum_dl/extractors/hyperkitty.py`

 * *Files 2% similar despite different names*

```diff
@@ -234,15 +234,18 @@
                 title=str(thread_anchor.tag.contents[-1]).strip(),
             )
 
         if page_link_tags := soup.find_all(class_="page-link"):
             last_page = int(page_link_tags[-2].string)
 
             if cur_page < last_page:
-                return PageState(url=urljoin(state.url, f"latest?page={cur_page + 1}"))
+                return PageState(
+                    url=urljoin(state.url, f"latest?page={cur_page + 1}"),
+                    page=state.page + 1,
+                )
 
     def _fetch_thread_page_posts(self, thread: Thread, state: PageState):
         origin = state.url
         response = self._session.get(origin)
 
         if state.url == thread.url:
             soup = Soup(response.content)
@@ -264,15 +267,17 @@
                 origin=origin,
                 data={},
                 author=str(email_author_div.find("a").string),
                 creation_time=dateutil.parser.parse(time).isoformat(),
                 content="".join(str(v) for v in email_body_div.contents),
             )
 
-            return PageState(url=urljoin(state.url, "replies?sort=thread"))
+            return PageState(
+                url=urljoin(state.url, "replies?sort=thread"), page=state.page + 1
+            )
 
         json = response.json()
 
         replies_html = json["replies_html"]
         soup = Soup(replies_html)
 
         reply_level_divs = soup.find_all("div", class_=["even", "odd"])
@@ -317,9 +322,10 @@
             )
 
             prev_reply_level = cur_reply_level
 
         if json["more_pending"]:
             next_offset = json["next_offset"]
             return PageState(
-                url=urljoin(state.url, f"replies?sort=thread&offset={next_offset}")
+                url=urljoin(state.url, f"replies?sort=thread&offset={next_offset}"),
+                page=state.page + 1,
             )
```

### Comparing `forum_dl-0.2.0/forum_dl/extractors/hypermail.py` & `forum_dl-0.3.0/forum_dl/extractors/hypermail.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 # pyright: strict
 from __future__ import annotations
 from typing import *  # type: ignore
 
 from pathlib import PurePosixPath
 from urllib.parse import urljoin, urlparse, urlunparse
-from dataclasses import dataclass
 from itertools import islice
 import bs4
 import re
 
 from .common import normalize_url, regex_match
 from .common import Extractor, ExtractorOptions, Board, Thread, Post, PageState
 from ..session import Session
 from ..soup import Soup
 
 
-@dataclass  # (kw_only=True)
 class HypermailPageState(PageState):
     relative_urls: list[str]
 
 
 class HypermailExtractor(Extractor):
     tests = [
         {
@@ -119,15 +117,17 @@
             page_anchors = soup.find_all("a", attrs={"href": self._page_href_regex})
             relative_urls = list(
                 reversed([page_anchor.get("href") for page_anchor in page_anchors])
             )
 
             relative_url = relative_urls.pop()
             return HypermailPageState(
-                url=urljoin(self.base_url, relative_url), relative_urls=relative_urls
+                url=urljoin(self.base_url, relative_url),
+                relative_urls=relative_urls,
+                page=state.page + 1,
             )
 
         state = cast(HypermailPageState, state)
 
         response = self._session.get(state.url)
         soup = Soup(response.content)
 
@@ -155,14 +155,15 @@
                 title="",  # TODO.
             )
 
         if state.relative_urls:
             relative_url = state.relative_urls.pop()
             return HypermailPageState(
                 url=urljoin(self.base_url, relative_url),
+                page=state.page + 1,
                 relative_urls=state.relative_urls,
             )
 
     def _fetch_thread_page_posts(self, thread: Thread, state: PageState):
         if state.url == thread.url:
             state.url = urljoin(thread.url, ".")
```

### Comparing `forum_dl-0.2.0/forum_dl/extractors/invision.py` & `forum_dl-0.3.0/forum_dl/extractors/invision.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,27 +1,30 @@
 # pyright: strict
 from __future__ import annotations
 from typing import *  # type: ignore
 
 import re
 
 from .common import (
-    Extractor,
+    HtmlExtractor,
     ExtractorOptions,
     Board,
     Thread,
     Post,
     PageState,
     regex_match,
 )
 from ..session import Session
-from ..soup import Soup
+from ..soup import Soup, SoupTag
 
+if TYPE_CHECKING:
+    from requests import Response
 
-class InvisionExtractor(Extractor):
+
+class InvisionExtractor(HtmlExtractor):
     tests = [
         {
             "url": "https://invisioncommunity.com/forums",
             "test_base_url": "https://invisioncommunity.com/forums/",
             "test_boards": {
                 ("180", "528"): {
                     "title": "Invision Community Insider",
@@ -65,14 +68,19 @@
             "url": "https://invisioncommunity.com/forums/topic/447328-guide-joels-guide-to-subscriptions/",
             "test_base_url": "https://invisioncommunity.com/forums/",
             "test_contents_hash": "1e0e0413cf82cf82bf83cfdf69813309594a06e4",
             "test_item_count": 52,
         },
     ]
 
+    _board_item_css = 'li[data-controller="forums.frontforum.topicRow"]'
+    _board_next_page_css = 'link[rel="next"]'
+    _thread_item_css = "article.ipsComment"
+    _thread_next_page_css = 'link[rel="next"]'
+
     @staticmethod
     def _detect(session: Session, url: str, options: ExtractorOptions):
         response = session.try_get(url, should_cache=True, should_retry=False)
         soup = Soup(response.content)
 
         breadcrumbs_ul = soup.find("ul", attrs={"data-role": "breadcrumbList"})
         breadcrumb_lis = breadcrumbs_ul.find_all("li")
@@ -178,67 +186,43 @@
 
     def _fetch_lazy_subboard(self, board: Board, subboard_id: str):
         pass
 
     def _fetch_lazy_subboards(self, board: Board):
         yield from ()
 
-    def _fetch_board_page_threads(self, board: Board, state: PageState):
-        if board is self.root:
-            return None
-
-        response = self._session.get(state.url)
-        soup = Soup(response.content)
-
-        thread_lis = soup.find_all(
-            "li", attrs={"data-controller": "forums.frontforum.topicRow"}
+    def _extract_board_page_thread(
+        self, board: Board, state: PageState, response: Response, tag: SoupTag
+    ):
+        thread_id = tag.get("data-rowid")
+        title_h4 = tag.find("h4", class_="ipsDataItem_title")
+        thread_anchor = title_h4.find("a", attrs={"title": True})
+
+        return Thread(
+            path=board.path + (thread_id,),
+            url=thread_anchor.get("href"),
+            origin=response.url,
+            data={},
+            title=thread_anchor.get("title"),
         )
-        for thread_li in thread_lis:
-            thread_id = thread_li.get("data-rowid")
-            title_h4 = thread_li.find("h4", class_="ipsDataItem_title")
-            thread_anchor = title_h4.find("a", attrs={"title": True})
-
-            yield Thread(
-                path=board.path + (thread_id,),
-                url=thread_anchor.get("href"),
-                origin=response.url,
-                data={},
-                title=thread_anchor.get("title"),
-            )
-
-        next_page_link = soup.try_find("link", attrs={"rel": "next"})
-        if next_page_link:
-            return PageState(url=next_page_link.get("href"))
 
-    def _fetch_thread_page_posts(self, thread: Thread, state: PageState):
-        response = self._session.get(state.url)
-        soup = Soup(response.content)
-
-        content_articles = soup.find_all("article", class_="ipsComment")
-
-        for content_article in content_articles:
-            content_div = content_article.find(
-                "div", attrs={"data-role": "commentContent"}
-            )
-            author_div = content_article.find("div", class_="cAuthorPane_content")
-            time_tag = author_div.find("time")
-
-            author_h3 = author_div.find("h3", class_="cAuthorPane_author")
-            url_div = author_div.find("div")
-            post_id = regex_match(
-                re.compile(r"^elComment_(\d+)"), content_article.get("id")
-            ).group(1)
-
-            yield Post(
-                path=thread.path,
-                subpath=(post_id,),
-                url=url_div.find("a").get("href"),
-                origin=response.url,
-                data={},
-                author=author_h3.find("a").string,
-                creation_time=time_tag.get("datetime"),
-                content="".join(str(v) for v in content_div.contents),
-            )
-
-        next_page_link = soup.try_find("link", attrs={"rel": "next"})
-        if next_page_link:
-            return PageState(url=next_page_link.get("href"))
+    def _extract_thread_page_post(
+        self, thread: Thread, state: PageState, response: Response, tag: SoupTag
+    ):
+        content_div = tag.find("div", attrs={"data-role": "commentContent"})
+        author_div = tag.find("div", class_="cAuthorPane_content")
+        time_tag = author_div.find("time")
+
+        author_h3 = author_div.find("h3", class_="cAuthorPane_author")
+        url_div = author_div.find("div")
+        post_id = regex_match(re.compile(r"^elComment_(\d+)"), tag.get("id")).group(1)
+
+        return Post(
+            path=thread.path,
+            subpath=(post_id,),
+            url=url_div.find("a").get("href"),
+            origin=response.url,
+            data={},
+            author=author_h3.find("a").string,
+            creation_time=time_tag.get("datetime"),
+            content="".join(str(v) for v in content_div.contents),
+        )
```

### Comparing `forum_dl-0.2.0/forum_dl/extractors/pipermail.py` & `forum_dl-0.3.0/forum_dl/extractors/pipermail.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,24 @@
 # pyright: strict
 from __future__ import annotations
 from typing import *  # type: ignore
 
 from pathlib import PurePosixPath
 from urllib.parse import urljoin, urlparse, urlunparse
-from dataclasses import dataclass
 import dateutil.parser
 import bs4
 import re
 
 from .common import normalize_url, regex_match
 from .common import Extractor, ExtractorOptions, Board, Thread, Post, PageState
 from ..exceptions import TagSearchError
 from ..session import Session
 from ..soup import Soup
 
 
-@dataclass  # (kw_only=True)
 class PipermailPageState(PageState):
     relative_urls: list[str]
 
 
 class PipermailExtractor(Extractor):
     tests = [
         {
@@ -218,14 +216,15 @@
             )
 
             relative_url = relative_urls.pop()
             return PipermailPageState(
                 url=urljoin(
                     urljoin(self.base_url, f"pipermail/{board_id}/"), relative_url
                 ),
+                page=state.page + 1,
                 relative_urls=relative_urls,
             )
 
         state = cast(PipermailPageState, state)
 
         response = self._session.get(state.url)
         soup = Soup(response.content)
@@ -253,14 +252,15 @@
         if state.relative_urls:
             relative_url = state.relative_urls.pop()
             board_id = board.path[0]
             return PipermailPageState(
                 url=urljoin(
                     urljoin(self.base_url, f"pipermail/{board_id}/"), relative_url
                 ),
+                page=state.page + 1,
                 relative_urls=state.relative_urls,
             )
 
     def _fetch_thread_page_posts(self, thread: Thread, state: PageState):
         if state.url == thread.url:
             state.url = urljoin(thread.url, "thread.html")
```

### Comparing `forum_dl-0.2.0/forum_dl/extractors/proboards.py` & `forum_dl-0.3.0/forum_dl/extractors/proboards.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,20 +4,23 @@
 
 from pathlib import PurePosixPath
 from urllib.parse import urljoin, urlparse
 from datetime import datetime
 import re
 
 from .common import regex_match
-from .common import Extractor, ExtractorOptions, Board, Thread, Post, PageState
+from .common import HtmlExtractor, ExtractorOptions, Board, Thread, Post, PageState
 from ..session import Session
-from ..soup import Soup
+from ..soup import Soup, SoupTag
 
+if TYPE_CHECKING:
+    from requests import Response
 
-class ProboardsExtractor(Extractor):
+
+class ProboardsExtractor(HtmlExtractor):
     tests = [
         {
             "url": "https://support.proboards.com",
             "test_base_url": "https://support.proboards.com/",
             "test_boards": {
                 ("4",): {
                     "title": "Tech Support",
@@ -55,15 +58,15 @@
                 ("32", "174"): {
                     "title": "ProBoards Contributions",
                 },
                 ("32", "176"): {
                     "title": "ProBoards v6 Beta",
                 },
                 ("16",): {
-                    "title": "Coding, Development and Design",
+                    "title": "Forum Customization",
                 },
                 ("16", "151"): {
                     "title": "Coding Help",
                 },
                 ("16", "38"): {
                     "title": "Plugins",
                 },
@@ -184,14 +187,19 @@
             "url": "https://support.proboards.com/thread/15052/visual-conceptions",
             "test_base_url": "https://support.proboards.com/",
             "test_contents_hash": "f655c7ddf487e7eb802c2123cef686f383433ee0",
             "test_item_count": 31,
         },
     ]
 
+    _board_item_css = 'a.thread-link:not([href^="/threads/recent"])'
+    _thread_item_css = "tr.item"
+    _board_next_page_css = ".next a[href]"
+    _thread_next_page_css = ".next a[href]"
+
     _category_name_regex = re.compile(r"^category-(\d+)$")
     _board_id_regex = re.compile(r"^board-(\d+)$")
     _thread_class_regex = re.compile(r"^thread-(\d+)$")
     _post_id_regex = re.compile(r"^post-(\d+)$")
 
     @staticmethod
     def _detect(session: Session, url: str, options: ExtractorOptions):
@@ -243,14 +251,17 @@
                     title=board_anchor.string,
                     are_subboards_fetched=True,
                 )
 
         self._fetch_lower_boards(self.root)
 
     def _do_fetch_subboards(self, board: Board):
+        if board is self.root:
+            return
+
         if not board.url:
             return
 
         response = self._session.get(board.url, should_cache=True)
         soup = Soup(response.content)
 
         subboard_trs = soup.find_all("tr", id=self._board_id_regex)
@@ -312,72 +323,41 @@
 
     def _fetch_lazy_subboard(self, board: Board, subboard_id: str):
         pass
 
     def _fetch_lazy_subboards(self, board: Board):
         yield from ()
 
-    def _fetch_board_page_threads(self, board: Board, state: PageState):
-        if board == self.root:
-            return None
-
-        response = self._session.get(state.url)
-        soup = Soup(response.content)
-
-        thread_anchors = soup.find_all("a", class_="thread-link")
-        for thread_anchor in thread_anchors:
-            thread_id = regex_match(
-                self._thread_class_regex, thread_anchor.get_list("class")
-            ).group(1)
-            yield Thread(
-                path=board.path + (thread_id,),
-                url=urljoin(self.base_url, thread_anchor.get("href")),
-                origin=response.url,
-                data={},
-                title=thread_anchor.string,
-            )
-
-        next_page_li = soup.try_find("li", class_="next")
-        if not next_page_li:
-            return None
-
-        next_page_anchor = next_page_li.try_find("a")
-
-        if next_page_anchor and next_page_anchor.try_get("href"):
-            return PageState(
-                url=urljoin(self.base_url, next_page_anchor.get("href")),
-            )
-
-    def _fetch_thread_page_posts(self, thread: Thread, state: PageState):
-        response = self._session.get(state.url)
-        soup = Soup(response.content)
-
-        post_trs = soup.find_all("tr", class_="item")
-        for post_tr in post_trs:
-            user_anchor = post_tr.try_find("a", class_="o-user-link")
-            time_abbr = post_tr.find("abbr", class_="time")
-            message_div = post_tr.find("div", class_="message")
-            post_id = regex_match(self._post_id_regex, post_tr.get("id")).group(1)
-
-            yield Post(
-                path=thread.path,
-                subpath=(post_id,),
-                url=urljoin(self.base_url, f"post/{post_id}/thread"),
-                origin=response.url,
-                data={},
-                author=user_anchor.string if user_anchor else "",
-                creation_time=datetime.fromtimestamp(
-                    int(time_abbr.get("data-timestamp")) / 1000
-                ).isoformat(),
-                content=str("".join(str(v) for v in message_div.contents)),
-            )
+    def _extract_board_page_thread(
+        self, board: Board, state: PageState, response: Response, tag: SoupTag
+    ):
+        thread_id = regex_match(self._thread_class_regex, tag.get_list("class")).group(
+            1
+        )
+        return Thread(
+            path=board.path + (thread_id,),
+            url=urljoin(self.base_url, tag.get("href")),
+            origin=response.url,
+            data={},
+            title=tag.string,
+        )
 
-        next_page_li = soup.try_find("li", class_="next")
-        if not next_page_li:
-            return None
-
-        next_page_anchor = next_page_li.try_find("a")
-
-        if next_page_anchor and next_page_anchor.try_get("href"):
-            return PageState(
-                url=urljoin(self.base_url, next_page_anchor.get("href")),
-            )
+    def _extract_thread_page_post(
+        self, thread: Thread, state: PageState, response: Response, tag: SoupTag
+    ):
+        user_anchor = tag.try_find("a", class_="o-user-link")
+        time_abbr = tag.find("abbr", class_="time")
+        message_div = tag.find("div", class_="message")
+        post_id = regex_match(self._post_id_regex, tag.get("id")).group(1)
+
+        return Post(
+            path=thread.path,
+            subpath=(post_id,),
+            url=urljoin(self.base_url, f"post/{post_id}/thread"),
+            origin=response.url,
+            data={},
+            author=user_anchor.string if user_anchor else "",
+            creation_time=datetime.fromtimestamp(
+                int(time_abbr.get("data-timestamp")) / 1000
+            ).isoformat(),
+            content=str("".join(str(v) for v in message_div.contents)),
+        )
```

### Comparing `forum_dl-0.2.0/forum_dl/extractors/simplemachines.py` & `forum_dl-0.3.0/forum_dl/extractors/vbulletin.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,483 +1,371 @@
 # pyright: strict
 from __future__ import annotations
 from typing import *  # type: ignore
 
-from dataclasses import dataclass
 from urllib.parse import urljoin
-import dateutil.parser
 import re
 
-from .common import normalize_url, regex_match, regex_search
-from .common import Extractor, ExtractorOptions, Board, Thread, Post, PageState
+from .common import regex_match
+from .common import HtmlExtractor, ExtractorOptions, Board, Thread, Post, PageState
 from ..session import Session
 from ..soup import Soup, SoupTag
 
+if TYPE_CHECKING:
+    from requests import Response
 
-@dataclass  # (kw_only=True)
-class SimplemachinesPageState(PageState):
-    page: int
 
-
-class SimplemachinesExtractor(Extractor):
+class VbulletinExtractor(HtmlExtractor):
     tests = [
         {
-            "url": "https://simplemachines.org/community",
-            "test_base_url": "https://www.simplemachines.org/community/",
+            "url": "https://forum.vbulletin.com",
+            "test_base_url": "https://forum.vbulletin.com/",
             "test_boards": {
-                ("2",): {
-                    "title": "Simple Machines",
+                ("14",): {
+                    "title": "vBulletin Announcements",
                 },
-                ("2", "1"): {
-                    "title": "News and Updates",
+                ("14", "28"): {
+                    "title": "vBulletin Announcements",
                 },
-                ("2", "244"): {
-                    "title": "Organizational News and Updates",
+                ("18",): {
+                    "title": "vBulletin Sales and Feedback",
                 },
-                ("3",): {
-                    "title": "SMF Support",
+                ("18", "40"): {
+                    "title": "vBulletin Pre-sales Questions",
                 },
-                ("3", "254"): {
-                    "title": "SMF 2.1.x Support",
+                ("18", "29"): {
+                    "title": "Site Feedback",
                 },
-                ("3", "254", "255"): {
-                    "title": "PostgreSQL Support",
+                ("24",): {
+                    "title": "vBulletin 5 Connect",
                 },
-                ("3", "147"): {
-                    "title": "SMF 2.0.x Support",
+                ("24", "72"): {
+                    "title": "vBulletin 5 Connect Feedback",
                 },
-                ("3", "147", "222"): {
-                    "title": "PostgreSQL and SQLite Support",
+                ("24", "111"): {
+                    "title": "Support Issues & Questions",
                 },
-                ("3", "9"): {
-                    "title": "SMF 1.1.x Support",
+                ("24", "111", "114"): {
+                    "title": "vBulletin 5 Tutorials",
                 },
-                ("3", "12"): {
-                    "title": "Language Specific Support",
+                ("24", "70"): {
+                    "title": "vBulletin 5 Suggestions",
                 },
-                ("3", "20"): {
-                    "title": "Converting to SMF",
+                ("24", "67"): {
+                    "title": "vBulletin 5 Installs & Upgrades",
                 },
-                ("3", "20", "132"): {
-                    "title": "IPB",
+                ("4014354",): {
+                    "title": "vBCloud",
                 },
-                ("3", "20", "11"): {
-                    "title": "MyBB",
+                ("4014354", "4014355"): {
+                    "title": "Account Management",
                 },
-                ("3", "20", "133"): {
-                    "title": "phpBB",
+                ("4014354", "4017486"): {
+                    "title": "vB Cloud Support & Troubleshooting.",
                 },
-                ("3", "20", "134"): {
-                    "title": "vBulletin",
+                ("4136723",): {
+                    "title": "International Support",
                 },
-                ("3", "20", "135"): {
-                    "title": "YaBB/YaBB SE",
+                ("4136723", "3954329"): {
+                    "title": "Deutschsprachiger Support",
                 },
-                ("18",): {
-                    "title": "Customizing SMF",
+                ("4136723", "3954329", "3967454"): {
+                    "title": "vBulletin 5 - Fragen und Probleme",
                 },
-                ("18", "60"): {
-                    "title": "SMF Coding Discussion",
+                ("4136723", "3954329", "3954332"): {
+                    "title": "vBulletin 5 - Installation & Upgrade",
                 },
-                ("18", "33"): {
-                    "title": "Bridges and Integrations",
+                ("4136723", "3954329", "3954333"): {
+                    "title": "vBulletin 5 - Tipps, Tricks & häufige Fragen",
                 },
-                ("18", "59"): {
-                    "title": "Modifications and Packages",
+                ("4136723", "3954329", "3954334"): {
+                    "title": "vBulletin 5 - Handbuch",
                 },
-                ("18", "59", "79"): {
-                    "title": "Mod Requests",
+                ("4136723", "4001685"): {
+                    "title": "Assistance francophone",
                 },
-                ("18", "34"): {
-                    "title": "Graphics and Templates",
+                ("4136723", "4055583"): {
+                    "title": "Soporte de Español",
                 },
-                ("18", "34", "106"): {
-                    "title": "Theme Site Themes",
+                ("3955117",): {
+                    "title": "vBulletin Mobile",
                 },
-                ("18", "34", "178"): {
-                    "title": "Theme Previews",
+                ("3955117", "62"): {
+                    "title": "vBulletin Mobile Suite",
                 },
-                ("18", "72"): {
-                    "title": "Tips and Tricks",
+                ("21",): {
+                    "title": "vBulletin 4",
                 },
-                ("18", "72", "115"): {
-                    "title": "Now Available",
+                ("21", "55"): {
+                    "title": "vB4 Support & Troubleshooting",
                 },
-                ("18", "116"): {
-                    "title": "Building Your Community and other Forum Advice",
+                ("21", "55", "101"): {
+                    "title": "vBulletin 4 Quick Tips and Customizations",
                 },
-                ("15",): {
-                    "title": "SMF Development",
+                ("21", "54"): {
+                    "title": "vBulletin 4 Installations and Upgrades",
                 },
-                ("15", "3"): {
-                    "title": "Feature Requests",
+                ("20",): {
+                    "title": "vBulletin 3.8",
                 },
-                ("15", "3", "38"): {
-                    "title": "Applied or Declined Requests",
+                ("20", "47"): {
+                    "title": "vBulletin 3.8 Support & Troubleshooting",
                 },
-                ("15", "3", "228"): {
-                    "title": "Next SMF Discussion",
+                ("20", "47", "97"): {
+                    "title": "vBulletin Quick Tips and Customizations",
                 },
-                ("15", "137"): {
-                    "title": "Bug Reports",
+                ("20", "48"): {
+                    "title": "vBulletin 3.8 Installation and Upgrades",
                 },
-                ("15", "137", "37"): {
-                    "title": "Fixed or Bogus Bugs",
+                ("13",): {
+                    "title": "Customizing vBulletin",
                 },
-                ("15", "137", "197"): {
-                    "title": "Bugtracker (Github)",
+                ("13", "42"): {
+                    "title": "vBulletin Languages & Phrases",
                 },
-                ("4",): {
-                    "title": "General Community",
+                ("13", "42", "105"): {
+                    "title": "vBulletin Mobile Languages",
                 },
-                ("4", "19"): {
-                    "title": "Site Comments, Issues and Concerns",
+                ("13", "31"): {
+                    "title": "vBulletin Templates, Graphics & Styles",
                 },
-                ("4", "8"): {
-                    "title": "Scripting Help",
+                ("13", "45"): {
+                    "title": "vBulletin Downloads",
                 },
-                ("4", "7"): {
-                    "title": "Test Board",
+                ("13", "45", "91"): {
+                    "title": "vBulletin Style Packs",
                 },
-                ("16",): {
-                    "title": "Simple Machines Blogs",
+                ("13", "45", "92"): {
+                    "title": "vBulletin Language Packs",
                 },
-                ("16", "128"): {
-                    "title": "SMF Team Blog",
+                ("13", "45", "93"): {
+                    "title": "vBulletin Graphics and Other Resources",
                 },
-                ("16", "129"): {
-                    "title": "Developers' Blog",
+                ("12",): {
+                    "title": "General",
                 },
-                ("5",): {
-                    "title": "Archived Boards and Threads...",
+                ("12", "79"): {
+                    "title": "vBulletin Showcase",
                 },
-                ("5", "136"): {
-                    "title": "Archived Boards",
+                ("12", "32"): {
+                    "title": "vBulletin Hosting Options",
                 },
-                ("5", "136", "2"): {
-                    "title": "SMF Feedback and Discussion",
+                ("12", "33"): {
+                    "title": "PHP & HTML Questions",
                 },
-                ("5", "136", "41"): {
-                    "title": "Parham's PHP Tutorials",
+                ("12", "30"): {
+                    "title": "Chit Chat",
                 },
-                ("5", "136", "96"): {
-                    "title": "Classic Themes",
+                ("19",): {
+                    "title": "vBulletin Legacy Versions & Products",
                 },
-                ("5", "136", "144"): {
-                    "title": "MotM Travel Blog",
+                ("19", "73"): {
+                    "title": "Legacy vBulletin Versions",
                 },
-                ("5", "136", "77"): {
-                    "title": "Mambo Bridge Support",
+                ("19", "73", "100"): {
+                    "title": "vBulletin 3.7 Questions, Problems and Troubleshooting",
                 },
-                ("5", "136", "138"): {
-                    "title": "Joomla Bridge Support",
+                ("19", "73", "96"): {
+                    "title": "vBulletin 3.6 Questions, Problems and Troubleshooting",
                 },
-                ("5", "136", "10"): {
-                    "title": "Install and Upgrade Help",
+                ("19", "73", "94"): {
+                    "title": "vBulletin 3.5 'How Do I' Questions and Troubleshooting",
                 },
-            },
-        },
-        {
-            "url": "https://www.simplemachines.org/community/index.php?board=255.0",
-            "test_base_url": "https://www.simplemachines.org/community/",
-            "test_boards": {
-                ("3", "254", "255"): {
-                    "title": "PostgreSQL Support",
+                ("19", "73", "86"): {
+                    "title": "vBulletin 3.0 How Do I and Troubleshooting Forum",
+                },
+                ("19", "73", "85"): {
+                    "title": "vBulletin 2 'How Do I' and Troubleshooting",
+                },
+                ("19", "73", "83"): {
+                    "title": "vBulletin 1.1.x Archives",
+                },
+                ("19", "73", "84"): {
+                    "title": "vBulletin Lite Archives",
                 },
-                ("3", "20", "134"): {
-                    "title": "vBulletin",
+                ("19", "74"): {
+                    "title": "Other Legacy Products",
                 },
-                ("4", "19"): {
-                    "title": "Site Comments, Issues and Concerns",
+                ("19", "74", "99"): {
+                    "title": "Pre-4.X Blog Archives",
+                },
+                ("19", "74", "98"): {
+                    "title": "Project Tools Archives",
+                },
+                ("19", "74", "64"): {
+                    "title": "vBulletin Facebook App",
+                },
+                ("19", "74", "44"): {
+                    "title": "vBulletin Impex Import System",
                 },
             },
         },
         {
-            "url": "https://www.simplemachines.org/community/index.php?topic=573.0",
-            "test_base_url": "https://www.simplemachines.org/community/",
-            "test_contents_hash": "daaf0300248ec6a1891aa1498c6637a89769dd7e",
-            "test_item_count": 6,
-        },
-        {
-            "url": "https://www.simplemachines.org/community/index.php?topic=197.0",
-            "test_base_url": "https://www.simplemachines.org/community/",
-            "test_contents_hash": "cd53463ffb3965590f925807902b6962893a1d5a",
-            "test_item_count": 50,
-        },
-        {
-            "url": "https://www.eevblog.com/forum/cooking/",
-            "test_base_url": "https://www.eevblog.com/forum/",
-            "test_min_item_count": 150,
-        },
-        {
-            "url": "https://www.eevblog.com/forum/eda/best-sub-$2k-pcb-design-software/",
-            "test_base_url": "https://www.eevblog.com/forum/",
-            # EEVBlog forum uses a PHPSESSID query for tracking, which makes the hash unpredictable.
-            # So, we don't test the hash.
-            # "test_contents_hash": "f9288cedb415d05e70887e658234a3c0976990c6",
-            "test_item_count": 69,
+            "url": "https://forum.vbulletin.com/forum/vbulletin-5-connect/vbulletin-5-connect-questions-problems-troubleshooting/vbulletin-5-tutorials/4131238-how-to-put-ads-after-first-post-in-thread-on-vb5-without-using-plugins",
+            "test_base_url": "https://forum.vbulletin.com/",
+            "test_contents_hash": "f369e03f9625e78acb0b070875c4f8ff83b62833",
+            "test_item_count": 66,
         },
         {
-            "url": "http://www.bay12forums.com/smf/index.php?board=10.0",
-            "test_base_url": "http://www.bay12forums.com/smf/",
-            "test_min_item_count": 150,
-        },
-        {
-            "url": "http://www.bay12forums.com/smf/index.php?topic=406.0",
-            "test_base_url": "http://www.bay12forums.com/smf/",
-            "test_item_count": 31,
-            "test_contents_hash": "4e2c2d065d83c23592379ef97c6d48dbea4f9f4f",
+            "url": "https://forum.vbulletin.com/forum/vbulletin-5-connect/vbulletin-5-connect-feedback/417300-cms-and-vbulletin-5",
+            "test_base_url": "https://forum.vbulletin.com/",
+            "test_contents_hash": "e358347798df127d65e4f96d9c95011063912ff2",
+            "test_item_count": 42,
         },
     ]
 
-    _category_id_regex = re.compile(r"^c(\d+)$")
-    _board_id_regex = re.compile(r"^b(\d+)$")
-    _span_id_regex = re.compile(r"^msg_(\d+)$")
-    _div_id_regex = re.compile(r"^msg_(\d+)$")
-    _post_wrapper_id_regex = re.compile(r"^msg(\d+)$")
-    _subject_id_regex = re.compile(r"^subject_(\d+)$")
+    _board_item_css = "tr.topic-item"
+    _board_next_page_css = "a.right-arrow[href]"
+    _thread_item_css = "li.b-post"
+    _thread_next_page_css = "a.right-arrow[href]"
+
+    _forum_id_regex = re.compile(r"^forum(\d+)$")
 
     @staticmethod
     def _detect(session: Session, url: str, options: ExtractorOptions):
         response = session.try_get(url, should_cache=True, should_retry=False)
         soup = Soup(response.content)
 
-        link = soup.find("link", attrs={"rel": "contents"})
-        base_url = normalize_url(link.get("href"))
-
-        simplemachines_anchor = soup.find(
-            "a",
-            attrs={
-                "href": re.compile(r"https?://www.simplemachines.org"),
-                "title": "Simple Machines",
-            },
-        )
+        generator_meta = soup.find("meta", attrs={"name": "generator"})
+        if not generator_meta.get("content").startswith("vBulletin"):
+            return None
 
-        if simplemachines_anchor:
-            return SimplemachinesExtractor(session, base_url, options)
+        base = soup.find("base")
+        return VbulletinExtractor(session, base.get("href"), options)
 
     def _fetch_top_boards(self):
         self._are_subboards_fetched[self.root.path] = True
 
         response = self._session.get(self.base_url, should_cache=True)
         soup = Soup(response.content)
 
-        category_anchors = soup.find_all("a", id=self._category_id_regex)
-        for category_anchor in category_anchors:
-            category_id = regex_match(
-                self._category_id_regex, category_anchor.get("id")
-            ).group(1)
-            category_title = str(category_anchor.next_sibling).strip()
+        trs = soup.find_all("tr", class_=["category-header", "forum-item"])
+        category_id = ""
 
-            self._set_board(
-                path=(category_id,),
-                url=urljoin(response.url, f"index.php#c{category_id}"),
-                origin=response.url,
-                data={},
-                title=category_title,
-                are_subboards_fetched=True,
-            )
+        for tr in trs:
+            if "category-header" in tr.get_list("class"):
+                category_id = regex_match(self._forum_id_regex, tr.get("id")).group(1)
+
+                category_anchor = tr.find("a", class_="category")
+                title = category_anchor.string
+
+                self._set_board(
+                    path=(category_id,),
+                    url=category_anchor.get("href"),
+                    origin=response.url,
+                    data={},
+                    title=title,
+                    are_subboards_fetched=True,
+                )
+            else:
+                board_id = regex_match(self._forum_id_regex, tr.get("id")).group(1)
 
-            for parent in category_anchor.parents:
-                board_anchors = parent.find_all("a", id=self._board_id_regex)
+                board_anchor = tr.find("a", class_="forum-title")
+                title = board_anchor.string
 
-                if not board_anchors:
-                    board_anchors = parent.find_all(
-                        "a", attrs={"name": self._board_id_regex}
-                    )
-
-                if board_anchors:
-                    for board_anchor in board_anchors:
-                        if board_anchor.get("id"):
-                            board_id = regex_match(
-                                self._board_id_regex, board_anchor.get("id")
-                            ).group(1)
-                        else:
-                            board_id = regex_match(
-                                self._board_id_regex, board_anchor.get("name")
-                            ).group(1)
-
-                        self._set_board(
-                            path=(category_id, board_id),
-                            url=board_anchor.get("href"),
-                            origin=response.url,
-                            data={},
-                            title=str(board_anchor.string).strip(),
-                            are_subboards_fetched=True,
-                        )
-                    break
+                self._set_board(
+                    path=(category_id, board_id),
+                    url=board_anchor.get("href"),
+                    origin=response.url,
+                    data={},
+                    title=title,
+                )
 
     def _do_fetch_subboards(self, board: Board):
-        if not board.url:
-            return
-
         # Don't fetch top boards.
         if len(board.path) <= 1:
             return
 
         response = self._session.get(board.url, should_cache=True)
         soup = Soup(response.content)
 
-        subboard_anchors = soup.find_all("a", attrs={"id": self._board_id_regex})
+        trs = soup.find_all("tr", class_="forum-item")
+        for tr in trs:
+            subboard_id = regex_match(self._forum_id_regex, tr.get("id")).group(1)
 
-        for subboard_anchor in subboard_anchors:
-            subboard_id = regex_match(
-                self._board_id_regex, subboard_anchor.get("id")
-            ).group(1)
+            subboard_anchor = tr.find("a", class_="forum-title")
             self._set_board(
                 path=board.path + (subboard_id,),
                 url=subboard_anchor.get("href"),
                 origin=response.url,
                 data={},
-                title=str(subboard_anchor.string).strip(),
-                are_subboards_fetched=True,
+                title=subboard_anchor.string.strip(),
             )
 
-    def _resolve_url(self, url: str):
-        return normalize_url(
-            self._session.get(url, should_cache=True).url,
-            append_slash=True,
-            keep_queries=["board", "topic"],
-        )
-
     def _get_node_from_url(self, url: str):
         response = self._session.get(url, should_cache=True)
         soup = Soup(response.content)
 
-        breadcrumbs = soup.try_find(class_="navigate_section")
-        if not breadcrumbs:
-            breadcrumbs = soup.find(class_="linktree")
+        breadcrumb_anchors = soup.find_all("a", class_="crumb-link")
 
-        breadcrumb_lis = breadcrumbs.find_all("li")
-        breadcrumb_as = [li.find("a") for li in breadcrumb_lis]
+        if len(breadcrumb_anchors) <= 1:
+            return self.root
 
         # Thread.
-        if soup.try_find("div", id="forumposts"):
-            breadcrumb_urls = [a.get("href") for a in breadcrumb_as]
-            board = self.find_board_from_urls(tuple(breadcrumb_urls[1:-1]))
-
-            topic_input = soup.find("input", attrs={"name": "topic"})
-            thread_id = topic_input.get("value")
-            title_title = soup.find("title")
+        if soup.try_find("h2", class_="b-post__title"):
+            breadcrumb_urls = [
+                self._resolve_url(anchor.get("href")) for anchor in breadcrumb_anchors
+            ]
+            board = self.find_board_from_urls(tuple(breadcrumb_urls[2:]))
+
+            thread_id = soup.find("input", attrs={"name": "nodeid"}).get("value")
+            title_h1 = soup.find("h1", class_="main-title")
 
             return Thread(
                 path=board.path + (thread_id,),
-                url=url,
+                url=urljoin(self.base_url, url),
                 origin=response.url,
                 data={},
-                title=str(title_title.string),
+                title=title_h1.string,
             )
-
         # Board.
         else:
             self._fetch_lower_boards(self.root)
 
-            board_href = self._resolve_url(breadcrumb_as[-1].get("href"))
+            board_title = breadcrumb_anchors[-1].string
 
             for cur_board in self._boards:
-                if cur_board.url == board_href:
+                if cur_board.title == board_title:
                     return cur_board
 
         raise ValueError
 
-    def _fetch_lazy_subboard(self, board: Board, subboard_id: str):
-        pass
-
     def _fetch_lazy_subboards(self, board: Board):
         yield from ()
 
-    def _fetch_board_page_threads(self, board: Board, state: PageState):
-        if board == self.root:
-            return None
-
-        if not state.url:
-            return None
-
-        if state.url == board.url:
-            state = SimplemachinesPageState(url=state.url, page=1)
-
-        state = cast(SimplemachinesPageState, state)
-
-        response = self._session.get(state.url)
-        soup = Soup(response.content)
-
-        msg_spans = soup.find_all("span", id=self._span_id_regex)
-
-        for msg_span in msg_spans:
-            thread_id = regex_match(self._span_id_regex, msg_span.get("id")).group(1)
-            msg_anchor = msg_span.tags[0]
-
-            yield Thread(
-                path=board.path + (thread_id,),
-                url=msg_anchor.get("href"),
-                origin=response.url,
-                data={},
-                title=str(msg_anchor.string),
-            )
-
-        next_page_anchor = soup.try_find(
-            "a", class_={"nav_page", "navPages"}, string=str(state.page + 1)
+    def _extract_board_page_thread(
+        self, board: Board, state: PageState, response: Response, tag: SoupTag
+    ):
+        thread_id = tag.get("data-node-id")
+        thread_anchor = tag.find("a", class_="topic-title")
+
+        return Thread(
+            path=board.path + (thread_id,),
+            url=thread_anchor.get("href"),
+            origin=response.url,
+            data={},
+            title=thread_anchor.string,
         )
-        if next_page_anchor:
-            return SimplemachinesPageState(
-                url=next_page_anchor.get("href"), page=state.page + 1
-            )
-
-    def _fetch_thread_page_posts(self, thread: Thread, state: PageState):
-        if state.url == thread.url:
-            state = SimplemachinesPageState(url=state.url, page=1)
 
-        state = cast(SimplemachinesPageState, state)
-
-        response = self._session.get(state.url)
-        soup = Soup(response.content)
-
-        post_wrapper_divs = soup.find_all("div", class_="post_wrapper")
-
-        if not post_wrapper_divs:
-            msg_as = soup.find_all("a", id=self._post_wrapper_id_regex)
-            post_wrapper_divs = [
-                SoupTag(a.tag.parent) for a in msg_as if a.tag.parent is not None
-            ]
-
-        for post_wrapper_div in post_wrapper_divs:
-            msg_div = post_wrapper_div.find("div", id=self._div_id_regex)
-            subject_tag = post_wrapper_div.find(
-                {"h5", "div"}, id=self._subject_id_regex
-            )
-
-            time_tag = subject_tag.find_next({"a", "div"}, class_="smalltext")
-
-            # This is ugly, but it's the best I can do for now.
-            date = regex_search(
-                re.compile(
-                    r"(January|February|March|April|May|June|July|August|September|October|November|December|Yesterday|Today) [a-zA-Z0-9,: ]+"
-                ),
-                time_tag.tag.get_text(),  # Get rid of HTML tags.
-            ).group(0)
-
-            poster_div = post_wrapper_div.find("div", class_="poster")
-            poster_h4 = poster_div.find("h4")
-
-            if poster_anchor := poster_h4.try_find("a"):
-                author = poster_anchor.string
-            else:
-                author = poster_h4.string.strip()
-
-            yield Post(
-                path=thread.path,
-                subpath=(regex_match(self._div_id_regex, msg_div.get("id")).group(1),),
-                url=subject_tag.find("a").get("href"),
-                origin=response.url,
-                data={},
-                author=author,
-                creation_time=dateutil.parser.parse(date, fuzzy=True).isoformat(),
-                content="".join(str(v) for v in msg_div.contents).strip(),
-            )
+    def _extract_thread_page_post(
+        self, thread: Thread, state: PageState, response: Response, tag: SoupTag
+    ):
+        # No support for comments for now.
+        if "b-comment" in tag.get_list("class"):
+            return
 
-        next_page_anchor = soup.try_find(
-            "a", class_={"nav_page", "navPages"}, string=str(state.page + 1)
+        url_anchor = tag.find("a", class_="b-post__count")
+        content_div = tag.find("div", class_="js-post__content-text")
+        author_anchor = tag.find("div", class_="author").find("a")
+        time_tag = tag.find("time", attrs={"itemprop": "dateCreated"})
+        post_id = tag.get("data-node-id")
+
+        return Post(
+            path=thread.path,
+            subpath=(post_id,),
+            url=url_anchor.get("href"),
+            origin=response.url,
+            data={},
+            author=author_anchor.string,
+            creation_time=time_tag.get("datetime"),
+            content="".join(str(v) for v in content_div.contents).strip(),
         )
-        if next_page_anchor:
-            return SimplemachinesPageState(
-                url=next_page_anchor.get("href"), page=state.page + 1
-            )
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `forum_dl-0.2.0/forum_dl/extractors/vbulletin.py` & `forum_dl-0.3.0/forum_dl/extractors/simplemachines.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,383 +1,436 @@
 # pyright: strict
 from __future__ import annotations
 from typing import *  # type: ignore
 
 from urllib.parse import urljoin
+import dateutil.parser
 import re
 
-from .common import regex_match
-from .common import Extractor, ExtractorOptions, Board, Thread, Post, PageState
+from .common import normalize_url, regex_match, regex_search
+from .common import HtmlExtractor, ExtractorOptions, Board, Thread, Post, PageState
 from ..session import Session
-from ..soup import Soup
+from ..soup import Soup, SoupTag
 
+if TYPE_CHECKING:
+    from requests import Response
 
-class VbulletinExtractor(Extractor):
+
+class SimplemachinesExtractor(HtmlExtractor):
     tests = [
         {
-            "url": "https://forum.vbulletin.com",
-            "test_base_url": "https://forum.vbulletin.com/",
+            "url": "https://simplemachines.org/community",
+            "test_base_url": "https://www.simplemachines.org/community/",
             "test_boards": {
-                ("14",): {
-                    "title": "vBulletin Announcements",
-                },
-                ("14", "28"): {
-                    "title": "vBulletin Announcements",
-                },
-                ("18",): {
-                    "title": "vBulletin Sales and Feedback",
-                },
-                ("18", "40"): {
-                    "title": "vBulletin Pre-sales Questions",
-                },
-                ("18", "29"): {
-                    "title": "Site Feedback",
-                },
-                ("24",): {
-                    "title": "vBulletin 5 Connect",
+                ("2",): {
+                    "title": "Simple Machines",
                 },
-                ("24", "72"): {
-                    "title": "vBulletin 5 Connect Feedback",
+                ("2", "1"): {
+                    "title": "News and Updates",
                 },
-                ("24", "111"): {
-                    "title": "Support Issues & Questions",
+                ("2", "244"): {
+                    "title": "Organizational News and Updates",
                 },
-                ("24", "111", "114"): {
-                    "title": "vBulletin 5 Tutorials",
+                ("3",): {
+                    "title": "SMF Support",
                 },
-                ("24", "70"): {
-                    "title": "vBulletin 5 Suggestions",
+                ("3", "254"): {
+                    "title": "SMF 2.1.x Support",
                 },
-                ("24", "67"): {
-                    "title": "vBulletin 5 Installs & Upgrades",
+                ("3", "254", "255"): {
+                    "title": "PostgreSQL Support",
                 },
-                ("4014354",): {
-                    "title": "vBCloud",
+                ("3", "147"): {
+                    "title": "SMF 2.0.x Support",
                 },
-                ("4014354", "4014355"): {
-                    "title": "Account Management",
+                ("3", "147", "222"): {
+                    "title": "PostgreSQL and SQLite Support",
                 },
-                ("4014354", "4017486"): {
-                    "title": "vB Cloud Support & Troubleshooting.",
+                ("3", "9"): {
+                    "title": "SMF 1.1.x Support",
                 },
-                ("4136723",): {
-                    "title": "International Support",
+                ("3", "12"): {
+                    "title": "Language Specific Support",
                 },
-                ("4136723", "3954329"): {
-                    "title": "Deutschsprachiger Support",
+                ("3", "20"): {
+                    "title": "Converting to SMF",
                 },
-                ("4136723", "3954329", "3967454"): {
-                    "title": "vBulletin 5 - Fragen und Probleme",
+                ("3", "20", "132"): {
+                    "title": "IPB",
                 },
-                ("4136723", "3954329", "3954332"): {
-                    "title": "vBulletin 5 - Installation & Upgrade",
+                ("3", "20", "11"): {
+                    "title": "MyBB",
                 },
-                ("4136723", "3954329", "3954333"): {
-                    "title": "vBulletin 5 - Tipps, Tricks & häufige Fragen",
+                ("3", "20", "133"): {
+                    "title": "phpBB",
                 },
-                ("4136723", "3954329", "3954334"): {
-                    "title": "vBulletin 5 - Handbuch",
+                ("3", "20", "134"): {
+                    "title": "vBulletin",
                 },
-                ("4136723", "4001685"): {
-                    "title": "Assistance francophone",
+                ("3", "20", "135"): {
+                    "title": "YaBB/YaBB SE",
                 },
-                ("4136723", "4055583"): {
-                    "title": "Soporte de Español",
-                },
-                ("3955117",): {
-                    "title": "vBulletin Mobile",
+                ("18",): {
+                    "title": "Customizing SMF",
                 },
-                ("3955117", "62"): {
-                    "title": "vBulletin Mobile Suite",
+                ("18", "60"): {
+                    "title": "SMF Coding Discussion",
                 },
-                ("21",): {
-                    "title": "vBulletin 4",
+                ("18", "33"): {
+                    "title": "Bridges and Integrations",
                 },
-                ("21", "55"): {
-                    "title": "vB4 Support & Troubleshooting",
+                ("18", "59"): {
+                    "title": "Modifications and Packages",
                 },
-                ("21", "55", "101"): {
-                    "title": "vBulletin 4 Quick Tips and Customizations",
+                ("18", "59", "79"): {
+                    "title": "Mod Requests",
                 },
-                ("21", "54"): {
-                    "title": "vBulletin 4 Installations and Upgrades",
+                ("18", "34"): {
+                    "title": "Graphics and Templates",
                 },
-                ("20",): {
-                    "title": "vBulletin 3.8",
+                ("18", "34", "106"): {
+                    "title": "Theme Site Themes",
                 },
-                ("20", "47"): {
-                    "title": "vBulletin 3.8 Support & Troubleshooting",
+                ("18", "34", "178"): {
+                    "title": "Theme Previews",
                 },
-                ("20", "47", "97"): {
-                    "title": "vBulletin Quick Tips and Customizations",
+                ("18", "72"): {
+                    "title": "Tips and Tricks",
                 },
-                ("20", "48"): {
-                    "title": "vBulletin 3.8 Installation and Upgrades",
+                ("18", "72", "115"): {
+                    "title": "Now Available",
                 },
-                ("13",): {
-                    "title": "Customizing vBulletin",
+                ("18", "116"): {
+                    "title": "Building Your Community and other Forum Advice",
                 },
-                ("13", "42"): {
-                    "title": "vBulletin Languages & Phrases",
+                ("15",): {
+                    "title": "SMF Development",
                 },
-                ("13", "42", "105"): {
-                    "title": "vBulletin Mobile Languages",
+                ("15", "3"): {
+                    "title": "Feature Requests",
                 },
-                ("13", "31"): {
-                    "title": "vBulletin Templates, Graphics & Styles",
+                ("15", "3", "38"): {
+                    "title": "Applied or Declined Requests",
                 },
-                ("13", "45"): {
-                    "title": "vBulletin Downloads",
+                ("15", "3", "228"): {
+                    "title": "Next SMF Discussion",
                 },
-                ("13", "45", "91"): {
-                    "title": "vBulletin Style Packs",
+                ("15", "137"): {
+                    "title": "Bug Reports",
                 },
-                ("13", "45", "92"): {
-                    "title": "vBulletin Language Packs",
+                ("15", "137", "37"): {
+                    "title": "Fixed or Bogus Bugs",
                 },
-                ("13", "45", "93"): {
-                    "title": "vBulletin Graphics and Other Resources",
+                ("15", "137", "197"): {
+                    "title": "Bugtracker (Github)",
                 },
-                ("12",): {
-                    "title": "General",
+                ("4",): {
+                    "title": "General Community",
                 },
-                ("12", "79"): {
-                    "title": "vBulletin Showcase",
+                ("4", "19"): {
+                    "title": "Site Comments, Issues and Concerns",
                 },
-                ("12", "32"): {
-                    "title": "vBulletin Hosting Options",
+                ("4", "8"): {
+                    "title": "Scripting Help",
                 },
-                ("12", "33"): {
-                    "title": "PHP & HTML Questions",
+                ("4", "7"): {
+                    "title": "Test Board",
                 },
-                ("12", "30"): {
-                    "title": "Chit Chat",
+                ("16",): {
+                    "title": "Simple Machines Blogs",
                 },
-                ("19",): {
-                    "title": "vBulletin Legacy Versions & Products",
+                ("16", "128"): {
+                    "title": "SMF Team Blog",
                 },
-                ("19", "73"): {
-                    "title": "Legacy vBulletin Versions",
+                ("16", "129"): {
+                    "title": "Developers' Blog",
                 },
-                ("19", "73", "100"): {
-                    "title": "vBulletin 3.7 Questions, Problems and Troubleshooting",
+                ("5",): {
+                    "title": "Archived Boards and Threads...",
                 },
-                ("19", "73", "96"): {
-                    "title": "vBulletin 3.6 Questions, Problems and Troubleshooting",
+                ("5", "136"): {
+                    "title": "Archived Boards",
                 },
-                ("19", "73", "94"): {
-                    "title": "vBulletin 3.5 'How Do I' Questions and Troubleshooting",
+                ("5", "136", "2"): {
+                    "title": "SMF Feedback and Discussion",
                 },
-                ("19", "73", "86"): {
-                    "title": "vBulletin 3.0 How Do I and Troubleshooting Forum",
+                ("5", "136", "41"): {
+                    "title": "Parham's PHP Tutorials",
                 },
-                ("19", "73", "85"): {
-                    "title": "vBulletin 2 'How Do I' and Troubleshooting",
+                ("5", "136", "96"): {
+                    "title": "Classic Themes",
                 },
-                ("19", "73", "83"): {
-                    "title": "vBulletin 1.1.x Archives",
+                ("5", "136", "144"): {
+                    "title": "MotM Travel Blog",
                 },
-                ("19", "73", "84"): {
-                    "title": "vBulletin Lite Archives",
+                ("5", "136", "77"): {
+                    "title": "Mambo Bridge Support",
                 },
-                ("19", "74"): {
-                    "title": "Other Legacy Products",
+                ("5", "136", "138"): {
+                    "title": "Joomla Bridge Support",
                 },
-                ("19", "74", "99"): {
-                    "title": "Pre-4.X Blog Archives",
+                ("5", "136", "10"): {
+                    "title": "Install and Upgrade Help",
                 },
-                ("19", "74", "98"): {
-                    "title": "Project Tools Archives",
+            },
+        },
+        {
+            "url": "https://www.simplemachines.org/community/index.php?board=255.0",
+            "test_base_url": "https://www.simplemachines.org/community/",
+            "test_boards": {
+                ("3", "254", "255"): {
+                    "title": "PostgreSQL Support",
                 },
-                ("19", "74", "64"): {
-                    "title": "vBulletin Facebook App",
+                ("3", "20", "134"): {
+                    "title": "vBulletin",
                 },
-                ("19", "74", "44"): {
-                    "title": "vBulletin Impex Import System",
+                ("4", "19"): {
+                    "title": "Site Comments, Issues and Concerns",
                 },
             },
         },
         {
-            "url": "https://forum.vbulletin.com/forum/vbulletin-5-connect/vbulletin-5-connect-questions-problems-troubleshooting/vbulletin-5-tutorials/4131238-how-to-put-ads-after-first-post-in-thread-on-vb5-without-using-plugins",
-            "test_base_url": "https://forum.vbulletin.com/",
-            "test_contents_hash": "1f6125f1221c38cbac359e3ad2d618762ebc2f02",
-            "test_item_count": 66,
+            "url": "https://www.simplemachines.org/community/index.php?topic=573.0",
+            "test_base_url": "https://www.simplemachines.org/community/",
+            "test_contents_hash": "daaf0300248ec6a1891aa1498c6637a89769dd7e",
+            "test_item_count": 6,
         },
         {
-            "url": "https://forum.vbulletin.com/forum/vbulletin-5-connect/vbulletin-5-connect-feedback/417300-cms-and-vbulletin-5",
-            "test_base_url": "https://forum.vbulletin.com/",
-            "test_contents_hash": "e358347798df127d65e4f96d9c95011063912ff2",
-            "test_item_count": 42,
+            "url": "https://www.simplemachines.org/community/index.php?topic=197.0",
+            "test_base_url": "https://www.simplemachines.org/community/",
+            "test_contents_hash": "cd53463ffb3965590f925807902b6962893a1d5a",
+            "test_item_count": 50,
+        },
+        {
+            "url": "https://www.eevblog.com/forum/cooking/",
+            "test_base_url": "https://www.eevblog.com/forum/",
+            "test_min_item_count": 150,
+        },
+        {
+            "url": "https://www.eevblog.com/forum/eda/best-sub-$2k-pcb-design-software/",
+            "test_base_url": "https://www.eevblog.com/forum/",
+            # EEVBlog forum uses a PHPSESSID query for tracking, which makes the hash unpredictable.
+            # So, we don't test the hash.
+            # "test_contents_hash": "f9288cedb415d05e70887e658234a3c0976990c6",
+            "test_item_count": 69,
+        },
+        {
+            "url": "http://www.bay12forums.com/smf/index.php?board=10.0",
+            "test_base_url": "http://www.bay12forums.com/smf/",
+            "test_min_item_count": 150,
+        },
+        {
+            "url": "http://www.bay12forums.com/smf/index.php?topic=406.0",
+            "test_base_url": "http://www.bay12forums.com/smf/",
+            "test_item_count": 31,
+            "test_contents_hash": "4e2c2d065d83c23592379ef97c6d48dbea4f9f4f",
         },
     ]
 
-    _forum_id_regex = re.compile(r"^forum(\d+)$")
+    _board_item_css = 'span[id^="msg_"]'
+    _thread_item_css = "div.post_wrapper, :has(> .postarea)"
+    _board_next_page_css = 'a.nav_page:has(span.next_page), a.navPages:-soup-contains("Next"), strong + a.navPages'
+    _thread_next_page_css = 'a.nav_page:has(span.next_page), a.navPages:-soup-contains("Next"), strong + a.navPages'
+
+    _category_id_regex = re.compile(r"^c(\d+)$")
+    _board_id_regex = re.compile(r"^b(\d+)$")
+    _div_id_regex = re.compile(r"^msg_(\d+)$")
+    _span_id_regex = re.compile(r"^msg_(\d+)$")
+    _subject_id_regex = re.compile(r"^subject_(\d+)$")
 
     @staticmethod
     def _detect(session: Session, url: str, options: ExtractorOptions):
         response = session.try_get(url, should_cache=True, should_retry=False)
         soup = Soup(response.content)
 
-        generator_meta = soup.find("meta", attrs={"name": "generator"})
-        if not generator_meta.get("content").startswith("vBulletin"):
-            return None
+        link = soup.find("link", attrs={"rel": "contents"})
+        base_url = normalize_url(link.get("href"))
+
+        simplemachines_anchor = soup.find(
+            "a",
+            attrs={
+                "href": re.compile(r"https?://www.simplemachines.org"),
+                "title": "Simple Machines",
+            },
+        )
 
-        base = soup.find("base")
-        return VbulletinExtractor(session, base.get("href"), options)
+        if simplemachines_anchor:
+            return SimplemachinesExtractor(session, base_url, options)
 
     def _fetch_top_boards(self):
         self._are_subboards_fetched[self.root.path] = True
 
         response = self._session.get(self.base_url, should_cache=True)
         soup = Soup(response.content)
 
-        trs = soup.find_all("tr", class_=["category-header", "forum-item"])
-        category_id = ""
+        category_anchors = soup.find_all("a", id=self._category_id_regex)
+        for category_anchor in category_anchors:
+            category_id = regex_match(
+                self._category_id_regex, category_anchor.get("id")
+            ).group(1)
+            category_title = str(category_anchor.next_sibling).strip()
+
+            self._set_board(
+                path=(category_id,),
+                url=urljoin(response.url, f"index.php#c{category_id}"),
+                origin=response.url,
+                data={},
+                title=category_title,
+                are_subboards_fetched=True,
+            )
+
+            for parent in category_anchor.parents:
+                board_anchors = parent.find_all("a", id=self._board_id_regex)
 
-        for tr in trs:
-            if "category-header" in tr.get_list("class"):
-                category_id = regex_match(self._forum_id_regex, tr.get("id")).group(1)
-
-                category_anchor = tr.find("a", class_="category")
-                title = category_anchor.string
-
-                self._set_board(
-                    path=(category_id,),
-                    url=category_anchor.get("href"),
-                    origin=response.url,
-                    data={},
-                    title=title,
-                    are_subboards_fetched=True,
-                )
-            else:
-                board_id = regex_match(self._forum_id_regex, tr.get("id")).group(1)
-
-                board_anchor = tr.find("a", class_="forum-title")
-                title = board_anchor.string
-
-                self._set_board(
-                    path=(category_id, board_id),
-                    url=board_anchor.get("href"),
-                    origin=response.url,
-                    data={},
-                    title=title,
-                )
+                if not board_anchors:
+                    board_anchors = parent.find_all(
+                        "a", attrs={"name": self._board_id_regex}
+                    )
+
+                if board_anchors:
+                    for board_anchor in board_anchors:
+                        if board_anchor.get("id"):
+                            board_id = regex_match(
+                                self._board_id_regex, board_anchor.get("id")
+                            ).group(1)
+                        else:
+                            board_id = regex_match(
+                                self._board_id_regex, board_anchor.get("name")
+                            ).group(1)
+
+                        self._set_board(
+                            path=(category_id, board_id),
+                            url=board_anchor.get("href"),
+                            origin=response.url,
+                            data={},
+                            title=str(board_anchor.string).strip(),
+                            are_subboards_fetched=True,
+                        )
+                    break
 
     def _do_fetch_subboards(self, board: Board):
+        if not board.url:
+            return
+
         # Don't fetch top boards.
         if len(board.path) <= 1:
             return
 
         response = self._session.get(board.url, should_cache=True)
         soup = Soup(response.content)
 
-        trs = soup.find_all("tr", class_="forum-item")
-        for tr in trs:
-            subboard_id = regex_match(self._forum_id_regex, tr.get("id")).group(1)
+        subboard_anchors = soup.find_all("a", attrs={"id": self._board_id_regex})
 
-            subboard_anchor = tr.find("a", class_="forum-title")
+        for subboard_anchor in subboard_anchors:
+            subboard_id = regex_match(
+                self._board_id_regex, subboard_anchor.get("id")
+            ).group(1)
             self._set_board(
                 path=board.path + (subboard_id,),
                 url=subboard_anchor.get("href"),
                 origin=response.url,
                 data={},
-                title=subboard_anchor.string.strip(),
+                title=str(subboard_anchor.string).strip(),
+                are_subboards_fetched=True,
             )
 
+    def _resolve_url(self, url: str):
+        return normalize_url(
+            self._session.get(url, should_cache=True).url,
+            append_slash=True,
+            keep_queries=["board", "topic"],
+        )
+
     def _get_node_from_url(self, url: str):
         response = self._session.get(url, should_cache=True)
         soup = Soup(response.content)
 
-        breadcrumb_anchors = soup.find_all("a", class_="crumb-link")
+        breadcrumbs = soup.try_find(class_="navigate_section")
+        if not breadcrumbs:
+            breadcrumbs = soup.find(class_="linktree")
 
-        if len(breadcrumb_anchors) <= 1:
-            return self.root
+        breadcrumb_lis = breadcrumbs.find_all("li")
+        breadcrumb_as = [li.find("a") for li in breadcrumb_lis]
 
         # Thread.
-        if soup.try_find("h2", class_="b-post__title"):
-            breadcrumb_urls = [
-                self._resolve_url(anchor.get("href")) for anchor in breadcrumb_anchors
-            ]
-            board = self.find_board_from_urls(tuple(breadcrumb_urls[2:]))
-
-            thread_id = soup.find("input", attrs={"name": "nodeid"}).get("value")
-            title_h1 = soup.find("h1", class_="main-title")
+        if soup.try_find("div", id="forumposts"):
+            breadcrumb_urls = [a.get("href") for a in breadcrumb_as]
+            board = self.find_board_from_urls(tuple(breadcrumb_urls[1:-1]))
+
+            topic_input = soup.find("input", attrs={"name": "topic"})
+            thread_id = topic_input.get("value")
+            title_title = soup.find("title")
 
             return Thread(
                 path=board.path + (thread_id,),
-                url=urljoin(self.base_url, url),
+                url=url,
                 origin=response.url,
                 data={},
-                title=title_h1.string,
+                title=str(title_title.string),
             )
+
         # Board.
         else:
             self._fetch_lower_boards(self.root)
 
-            board_title = breadcrumb_anchors[-1].string
+            board_href = self._resolve_url(breadcrumb_as[-1].get("href"))
 
             for cur_board in self._boards:
-                if cur_board.title == board_title:
+                if cur_board.url == board_href:
                     return cur_board
 
         raise ValueError
 
+    def _fetch_lazy_subboard(self, board: Board, subboard_id: str):
+        pass
+
     def _fetch_lazy_subboards(self, board: Board):
         yield from ()
 
-    def _fetch_board_page_threads(self, board: Board, state: PageState):
-        if board == self.root:
-            return None
-
-        if not state.url:
-            return None
-
-        response = self._session.get(state.url)
-        soup = Soup(response.content)
+    def _extract_board_page_thread(
+        self, board: Board, state: PageState, response: Response, tag: SoupTag
+    ):
+        thread_id = regex_match(self._span_id_regex, tag.get("id")).group(1)
+        msg_anchor = tag.tags[0]
+
+        return Thread(
+            path=board.path + (thread_id,),
+            url=msg_anchor.get("href"),
+            origin=response.url,
+            data={},
+            title=str(msg_anchor.string),
+        )
+
+    def _extract_thread_page_post(
+        self, thread: Thread, state: PageState, response: Response, tag: SoupTag
+    ):
+        msg_div = tag.find("div", id=self._div_id_regex)
+        subject_tag = tag.find({"h5", "div"}, id=self._subject_id_regex)
+
+        time_tag = subject_tag.find_next({"a", "div"}, class_="smalltext")
+
+        # This is ugly, but it's the best I can do for now.
+        date = regex_search(
+            re.compile(
+                r"(January|February|March|April|May|June|July|August|September|October|November|December|Yesterday|Today) [a-zA-Z0-9,: ]+"
+            ),
+            time_tag.tag.get_text(),  # Get rid of HTML tags.
+        ).group(0)
 
-        thread_trs = soup.find_all("tr", class_="topic-item")
-        for thread_tr in thread_trs:
-            thread_id = thread_tr.get("data-node-id")
-            thread_anchor = thread_tr.find("a", class_="topic-title")
+        poster_div = tag.find("div", class_="poster")
+        poster_h4 = poster_div.find("h4")
 
-            yield Thread(
-                path=board.path + (thread_id,),
-                url=thread_anchor.get("href"),
-                origin=response.url,
-                data={},
-                title=thread_anchor.string,
-            )
-
-        next_page_anchor = soup.try_find("a", class_="right-arrow")
-        if next_page_anchor and next_page_anchor.get("href"):
-            return PageState(url=next_page_anchor.get("href"))
-
-    def _fetch_thread_page_posts(self, thread: Thread, state: PageState):
-        response = self._session.get(state.url)
-        soup = Soup(response.content)
-
-        post_lis = soup.find_all("li", class_="b-post")
-        for post_li in post_lis:
-            # No support for comments for now.
-            if "b-comment" in post_li.get_list("class"):
-                continue
-
-            url_anchor = post_li.find("a", class_="b-post__count")
-            content_div = post_li.find("div", class_="js-post__content-text")
-            author_anchor = post_li.find("div", class_="author").find("a")
-            time_tag = post_li.find("time", attrs={"itemprop": "dateCreated"})
-            post_id = post_li.get("data-node-id")
-
-            yield Post(
-                path=thread.path,
-                subpath=(post_id,),
-                url=url_anchor.get("href"),
-                origin=response.url,
-                data={},
-                author=author_anchor.string,
-                creation_time=time_tag.get("datetime"),
-                content="".join(str(v) for v in content_div.contents).strip(),
-            )
+        if poster_anchor := poster_h4.try_find("a"):
+            author = poster_anchor.string
+        else:
+            author = poster_h4.string.strip()
 
-        next_page_anchor = soup.try_find("a", class_="right-arrow")
-        if next_page_anchor and next_page_anchor.try_get("href"):
-            return PageState(url=next_page_anchor.get("href"))
+        return Post(
+            path=thread.path,
+            subpath=(regex_match(self._div_id_regex, msg_div.get("id")).group(1),),
+            url=subject_tag.find("a").get("href"),
+            origin=response.url,
+            data={},
+            author=author,
+            creation_time=dateutil.parser.parse(date, fuzzy=True).isoformat(),
+            content="".join(str(v) for v in msg_div.contents).strip(),
+        )
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `forum_dl-0.2.0/forum_dl/extractors/xenforo.py` & `forum_dl-0.3.0/forum_dl/extractors/xenforo.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,20 +2,23 @@
 from __future__ import annotations
 from typing import *  # type: ignore
 
 from urllib.parse import urljoin
 import re
 
 from .common import normalize_url, regex_match
-from .common import Extractor, ExtractorOptions, Board, Thread, Post, PageState
+from .common import HtmlExtractor, ExtractorOptions, Board, Thread, Post, PageState
 from ..session import Session
-from ..soup import Soup
+from ..soup import Soup, SoupTag
 
+if TYPE_CHECKING:
+    from requests import Response
 
-class XenforoExtractor(Extractor):
+
+class XenforoExtractor(HtmlExtractor):
     tests = [
         {
             "url": "https://xenforo.com/community",
             "test_base_url": "https://xenforo.com/community/",
             "test_boards": {
                 ("1",): {
                     "title": "Official forums",
@@ -183,48 +186,108 @@
                     "title": "Example page",
                 },
             },
         },
         {
             "url": "https://xenforo.com/community/threads/darkness-free-xenforo-2-gaming-skin-deleted.154782/",
             "test_base_url": "https://xenforo.com/community/",
-            "test_contents_hash": "00cd24c8a7aba0f567d6a0868cfe27fada450ca4",
+            "test_contents_hash": "0c49d593c65d6a3a57a27115a7659391d889a78d",
             "test_item_count": 53,
         },
         {
             "url": "https://xenforo.com/community/threads/steam-authentication-deleted.141309/",
             "test_base_url": "https://xenforo.com/community/",
-            "test_contents_hash": "47091f2cb3f716ee16f5057f8350a2f514ed4bce",
+            "test_contents_hash": "ba129ef0ceb4fdb92aee79e2b0ba1a4eabf24557",
             "test_item_count": 26,
         },
+        {
+            "url": "https://forums.tomshardware.com/categories/hardware.1/",
+            "test_base_url": "https://forums.tomshardware.com/",
+            "test_boards": {
+                ("1", "9"): {
+                    "title": "Graphics Cards",
+                },
+                ("1", "7"): {
+                    "title": "Systems",
+                },
+                ("1", "3"): {
+                    "title": "Components",
+                },
+                ("1", "2"): {
+                    "title": "CPUs",
+                },
+                ("1", "5"): {
+                    "title": "Motherboards",
+                },
+                ("1", "8"): {
+                    "title": "Storage",
+                },
+                ("1", "4"): {
+                    "title": "Overclocking",
+                },
+                ("1", "6"): {
+                    "title": "Memory",
+                },
+                ("1", "10"): {
+                    "title": "Displays",
+                },
+                ("1", "44"): {
+                    "title": "Prebuilt & Enterprise",
+                },
+                ("1", "77"): {
+                    "title": "Cases",
+                },
+                ("1", "74"): {
+                    "title": "Cooling",
+                },
+                ("1", "75"): {
+                    "title": "Power Supplies",
+                },
+                ("1", "78"): {
+                    "title": "Raspberry Pi & Single Board Computers",
+                },
+            },
+        },
+        {
+            "url": "https://forums.tomshardware.com/threads/windows-11.3707807/",
+            "test_base_url": "https://forums.tomshardware.com/",
+            "test_contents_hash": "5c6b603554ae10ad04c1d75918edeed4ec5875f5",
+            "test_item_count": 96,
+        },
     ]
 
+    _board_item_css = "div.structItem--thread"
+    _board_next_page_css = "a.pageNav-jump--next"
+    _thread_item_css = "article.message"
+    _thread_next_page_css = "a.pageNav-jump--next"
+
     _category_class_regex = re.compile(r"^block--category(\d+)$")
     _board_class_regex = re.compile(r"^node--id(\d+)$")
     _thread_class_regex = re.compile(r"^js-threadListItem-(\d+)$")
     _thread_key_regex = re.compile(r"^thread-(\d+)$")
     _post_id_regex = re.compile(r"^post-(\d+)$")
 
     @staticmethod
     def _detect(session: Session, url: str, options: ExtractorOptions):
         response = session.try_get(
             normalize_url(url, remove_suffixes=[], append_slash=False),
             should_cache=True,
             should_retry=False,
         )
+
+        if not re.search(r'<html[^>]+id="XF"', response.text, re.MULTILINE):
+            return None
+
         soup = Soup(response.content)
 
         data_nav_id_anchor = soup.find("a", attrs={"data-nav-id": "forums"})
         base_url = normalize_url(urljoin(url, data_nav_id_anchor.get("href")))
         if not base_url:
             return None
 
-        if not soup.find("a", attrs={"rel": "sponsored noopener"}):
-            return None
-
         return XenforoExtractor(session, base_url, options)
 
     def _fetch_top_boards(self):
         self._are_subboards_fetched[self.root.path] = True
 
         response = self._session.get(self.base_url, should_cache=True)
         soup = Soup(response.content)
@@ -275,116 +338,94 @@
     def _do_fetch_subboards(self, board: Board):
         pass
 
     def _get_node_from_url(self, url: str):
         response = self._session.get(url, should_cache=True)
         soup = Soup(response.content)
 
-        breadcrumbs_ul = soup.find("ul", class_="p-breadcrumbs")
-        breadcrumb_anchors = breadcrumbs_ul.find_all("a", attrs={"itemprop": "item"})
+        if breadcrumbs_ul := soup.try_find("ul", class_="p-breadcrumbs"):
+            breadcrumb_anchors = breadcrumbs_ul.find_all(
+                "a", attrs={"itemprop": "item"}
+            )
 
-        if len(breadcrumb_anchors) <= 1:
+            if len(breadcrumb_anchors) <= 1:
+                return self.root
+        else:
             return self.root
 
         # Thread.
-        if soup.find("article"):
+        if soup.try_find("article"):
             board_url = urljoin(url, breadcrumb_anchors[-2].get("href"))
-            html = soup.find("html")
+            block_div = soup.find(
+                "div", class_="block-container", attrs={"data-lb-id": True}
+            )
             thread_id = regex_match(
-                self._thread_key_regex, html.get("data-content-key")
+                self._thread_key_regex, block_div.get("data-lb-id")
             ).group(1)
             title_h1 = soup.find("h1", class_="p-title-value")
 
             for cur_board in self._boards:
                 if cur_board.url == board_url:
                     return Thread(
                         path=cur_board.path + (thread_id,),
                         url=urljoin(self.base_url, url),
                         origin=response.url,
                         data={},
                         title=title_h1.string,
                     )
         # Board.
         else:
-            board_href = self._resolve_url(breadcrumb_anchors[-1].get("href"))
+            # Instead of normalizing the URL, we go the easy way: we get the OpenGraph URL.
+            board_href = soup.find("meta", attrs={"property": "og:url"}).get("content")
 
             for cur_board in self._boards:
                 if cur_board.url == board_href:
                     return cur_board
 
         raise ValueError
 
     def _fetch_lazy_subboard(self, board: Board, subboard_id: str):
         pass
 
     def _fetch_lazy_subboards(self, board: Board):
         yield from ()
 
-    def _fetch_board_page_threads(self, board: Board, state: PageState):
-        if board == self.root:
-            return None
-
-        if not state.url:
-            return None
-
-        response = self._session.get(state.url)
-        soup = Soup(response.content)
-
-        thread_divs = soup.find_all("div", class_=self._thread_class_regex)
-        for thread_div in thread_divs:
-            thread_id = regex_match(
-                self._thread_class_regex, thread_div.get_list("class")[-1]
-            ).group(1)
-
-            title_div = thread_div.find("div", class_="structItem-title")
-            title_anchor = title_div.find("a")
-
-            url = urljoin(self.base_url, title_anchor.get("href"))
-
-            yield Thread(
-                path=board.path + (thread_id,),
-                url=url,
-                origin=response.url,
-                data={},
-                title=title_anchor.string,
-            )
-
-        next_page_anchor = soup.try_find("a", class_="pageNav-jump--next")
-        if next_page_anchor:
-            return PageState(
-                url=urljoin(self.base_url, next_page_anchor.get("href")),
-            )
-
-    def _fetch_thread_page_posts(self, thread: Thread, state: PageState):
-        response = self._session.get(state.url)
-        soup = Soup(response.content)
-
-        message_articles = soup.find_all("article", class_="message")
-
-        for message_article in message_articles:
-            bbwrapper_div = message_article.find("div", class_="bbWrapper")
-            message_attribution_ul = message_article.find(
-                "ul", class_="message-attribution-main"
-            )
-            url_anchor = message_attribution_ul.find("a")
-            time_tag = message_attribution_ul.find("time")
-
-            yield Post(
-                path=thread.path,
-                subpath=(
-                    regex_match(
-                        self._post_id_regex, message_article.get("data-content")
-                    ).group(1),
-                ),
-                url=urljoin(state.url, url_anchor.get("href")),
-                origin=response.url,
-                data={},
-                author=message_article.get("data-author"),
-                creation_time=time_tag.get("datetime"),
-                content=str(bbwrapper_div.encode_contents()),
-            )
+    def _extract_board_page_thread(
+        self, board: Board, state: PageState, response: Response, tag: SoupTag
+    ):
+        thread_id = regex_match(
+            self._thread_class_regex, tag.get_list("class")[-1]
+        ).group(1)
+
+        title_div = tag.find("div", class_="structItem-title")
+        title_anchor = title_div.find("a", attrs={"data-tp-primary": True})
+
+        url = urljoin(self.base_url, title_anchor.get("href"))
+
+        return Thread(
+            path=board.path + (thread_id,),
+            url=url,
+            origin=response.url,
+            data={},
+            title=title_anchor.string,
+        )
 
-        next_page_anchor = soup.try_find("a", class_="pageNav-jump--next")
-        if next_page_anchor:
-            return PageState(
-                url=urljoin(self.base_url, next_page_anchor.get("href")),
-            )
+    def _extract_thread_page_post(
+        self, thread: Thread, state: PageState, response: Response, tag: SoupTag
+    ):
+        bbwrapper_div = tag.find("div", class_="bbWrapper")
+        message_attribution_ul = tag.find("ul", class_="message-attribution-main")
+        url_anchor = message_attribution_ul.find("a")
+        time_tag = message_attribution_ul.find("time")
+
+        return Post(
+            path=thread.path,
+            subpath=(
+                regex_match(self._post_id_regex, tag.get("data-content")).group(1),
+            ),
+            url=urljoin(state.url, url_anchor.get("href")),
+            origin=response.url,
+            data={},
+            author=tag.get("data-author"),
+            creation_time=time_tag.get("datetime"),
+            content=bbwrapper_div.string,
+        )
```

### Comparing `forum_dl-0.2.0/forum_dl/forumdl.py` & `forum_dl-0.3.0/forum_dl/forumdl.py`

 * *Files identical despite different names*

### Comparing `forum_dl-0.2.0/forum_dl/options.py` & `forum_dl-0.3.0/forum_dl/options.py`

 * *Files 12% similar despite different names*

```diff
@@ -36,14 +36,21 @@
         dest="list_output_formats",
         action="store_true",
         help="List all supported output formats and exit",
     )
 
     session = parser.add_argument_group("Session Options")
     session.add_argument(
+        "--timeout",
+        metavar="SECONDS",
+        dest="timeout",
+        default="5",
+        help="HTTP connection timeout",
+    )
+    session.add_argument(
         "-R",
         "--retries",
         metavar="N",
         dest="retries",
         default="4",
         help="Maximum number of retries for failed HTTP requests or -1 to retry infinitely (default: 4)",
     )
@@ -93,17 +100,18 @@
         dest="get_urls",
         action="store_true",
         help="Print URLs instead of downloading",
     )
     output.add_argument(
         "-o",
         "--output",
-        metavar="FILE",
+        metavar="OUTFILE",
         dest="output",
-        help="Output all results concatenated to FILE, or stdout if FILE is -",
+        default="-",
+        help="Output all results concatenated to OUTFILE, or stdout if OUTFILE is - (default: -)",
     )
     output.add_argument(
         "-f",
         "--output-format",
         metavar="FORMAT",
         dest="output_format",
         default="jsonl",
@@ -113,30 +121,54 @@
         "--warc-output",
         metavar="FILE",
         dest="warc_output",
         default="",
         help="Record HTTP requests, store them in FILE in WARC format",
     )
     output.add_argument(
-        "--no-boards",
+        "--files-output",
+        metavar="DIR",
+        dest="files_output",
+        default="",
+        help="Store files in DIR instead of OUTFILE",
+    )
+    output.add_argument(
+        "--boards",
         dest="boards",
-        action="store_false",
-        help="Do not write board objects",
+        default=True,
+        action=argparse.BooleanOptionalAction,
+        help="Write board objects (default: True, --no-boards to negate)",
     )
     output.add_argument(
-        "--no-threads",
+        "--threads",
         dest="threads",
-        action="store_false",
-        help="Do not write thread objects",
+        default=True,
+        action=argparse.BooleanOptionalAction,
+        help="Write thread objects (default: True, --no-threads to negate)",
     )
     output.add_argument(
-        "--no-posts",
+        "--posts",
         dest="posts",
-        action="store_false",
-        help="Do not write post objects",
+        default=True,
+        action=argparse.BooleanOptionalAction,
+        help="Write post objects (default: True, --no-posts to negate)",
+    )
+    output.add_argument(
+        "--files",
+        dest="files",
+        default=True,
+        action=argparse.BooleanOptionalAction,
+        help="Write embedded files (--no-files to negate)",
+    )
+    output.add_argument(
+        "--outside-files",
+        dest="outside_files",
+        default=False,
+        action=argparse.BooleanOptionalAction,
+        help="Write embedded files outside post content. Auto-enabled by --warc-output and -f warc (default: False, --no-outside-files to negate)",
     )
     output.add_argument(
         "--textify",
         dest="textify",
         action="store_true",
         help="Lossily convert HTML content to plaintext",
     )
```

### Comparing `forum_dl-0.2.0/forum_dl/session.py` & `forum_dl-0.3.0/forum_dl/session.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # type: ignore
 from __future__ import annotations
 from typing import *  # type: ignore
 
-from dataclasses import dataclass
+from pydantic import BaseModel
 from functools import lru_cache, wraps
 from tenacity import (
     retry,
     wait_random_exponential,
     stop_after_attempt,
     before_sleep_log,
 )
@@ -16,19 +16,19 @@
 from .exceptions import CrawlError
 from .version import __version__
 
 if TYPE_CHECKING:
     from requests import Response
 
 
-@dataclass  # (kw_only=True)
-class SessionOptions:
+class SessionOptions(BaseModel):
+    timeout: float
     retries: int
-    retry_sleep: int
-    retry_sleep_multiplier: int
+    retry_sleep: float
+    retry_sleep_multiplier: float
     warc_output: str
     user_agent: str
     get_urls: bool
 
 
 class Session:
     def __init__(self, options: SessionOptions):
@@ -103,15 +103,15 @@
             cached_response = self._cache[(url, frozen_params, frozen_headers)]
 
             if not should_cache:
                 del self._cache[(url, frozen_params, frozen_headers)]
 
             return cached_response
         elif (url, frozen_params, frozen_headers) in self._past_requests:
-            raise CrawlError
+            raise CrawlError(url, frozen_params, frozen_headers)
 
         if should_retry:
 
             @retry(
                 reraise=True,
                 wait=wait_random_exponential(
                     multiplier=self._options.retry_sleep,
@@ -132,15 +132,15 @@
             response = retrying_get(url, params=params, headers=headers, **kwargs)
         else:
             response = self._do_get(url, params=params, headers=headers, **kwargs)
 
         if should_cache:
             self._cache[(url, frozen_params, frozen_headers)] = response
         else:
-            self._past_requests.add(url)
+            self._past_requests.add((url, frozen_params, frozen_headers))
 
         return response
 
     def _after_retry(self):
         logging.warning(f"Waiting {self.delay} seconds.")
 
     def _do_get(
@@ -157,10 +157,30 @@
             logging.info(f"GET {url} {params} {headers}")
 
         if not headers:
             headers = {"User-Agent": self._options.user_agent}
 
         if self._warc_file:
             with self._capture_http(self._warc_writer):
-                return self._session.get(url, params=params, headers=headers, **kwargs)
+                return self._session.get(
+                    url,
+                    params=params,
+                    headers=headers,
+                    timeout=self._options.timeout,
+                    **kwargs,
+                )
         else:
-            return self._session.get(url, params=params, headers=headers, **kwargs)
+            return self._session.get(
+                url,
+                params=params,
+                headers=headers,
+                timeout=self._options.timeout,
+                **kwargs,
+            )
+
+    def validate_url(self, url: str):
+        try:
+            self._session.get_adapter(url)
+        except:  # `InvalidSchema`, not referencing it directly to avoid breaking WARC recording.
+            return False
+
+        return True
```

### Comparing `forum_dl-0.2.0/forum_dl/soup.py` & `forum_dl-0.3.0/forum_dl/soup.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,15 +20,15 @@
         recursive: bool = True,
         string: SoupInput | None = None,
         **kwargs: Any,
     ) -> SoupTag | None:
         result = self.soup.find(name, attrs, recursive, string, **kwargs)
 
         if result is not None and not isinstance(result, bs4.element.Tag):
-            raise TagSearchError
+            raise TagSearchError(self.soup, name, attrs, recursive, string, kwargs)
 
         if result:
             return SoupTag(result)
 
     def find(
         self,
         name: SoupInput | None = None,
@@ -36,15 +36,15 @@
         recursive: bool = True,
         string: SoupInput | None = None,
         **kwargs: Any,
     ) -> SoupTag:
         result = self.try_find(name, attrs, recursive, string, **kwargs)
 
         if not result:
-            raise TagSearchError
+            raise TagSearchError(self.soup, name, attrs, recursive, string, kwargs)
 
         return result
 
     def find_all(
         self,
         name: SoupInput | None = None,
         attrs: dict[str, Any] = {},
@@ -69,15 +69,15 @@
         recursive: bool = True,
         string: SoupInput | None = None,
         **kwargs: Any,
     ) -> SoupTag | None:
         result = self.tag.find(name, attrs, recursive, string, **kwargs)
 
         if result is not None and not isinstance(result, bs4.element.Tag):
-            raise TagSearchError
+            raise TagSearchError(self.tag, name, attrs, recursive, string, kwargs)
 
         if result:
             return SoupTag(result)
 
     def find(
         self,
         name: SoupInput | None = None,
@@ -85,15 +85,15 @@
         recursive: bool = True,
         string: SoupInput | None = None,
         **kwargs: Any,
     ):
         result = self.try_find(name, attrs, recursive, string, **kwargs)
 
         if not result:
-            raise TagSearchError
+            raise TagSearchError(self.tag, name, attrs, recursive, string, kwargs)
 
         return result
 
     def find_all(
         self,
         name: SoupInput | None = None,
         attrs: dict[str, Any] = {},
@@ -112,66 +112,63 @@
         attrs: dict[str, Any] = {},
         string: SoupInput | None = None,
         **kwargs: Any,
     ):
         result = self.tag.find_next(name, attrs, string, **kwargs)
 
         if not isinstance(result, bs4.element.Tag):
-            raise TagSearchError
+            raise TagSearchError(self.tag, name, attrs, string, kwargs)
 
         return SoupTag(result)
 
     def find_previous(
         self,
         name: SoupInput | None = None,
         attrs: dict[str, Any] = {},
         string: SoupInput | None = None,
         **kwargs: Any,
     ):
         result = self.tag.find_previous(name, attrs, string, **kwargs)
 
         if not isinstance(result, bs4.element.Tag):
-            raise TagSearchError
+            raise TagSearchError(self.tag, name, attrs, string, kwargs)
 
         return SoupTag(result)
 
     def try_get(self, key: str, default: str | list[str] | None = None):
         return self.tag.get(key, default)
 
     def get(self, key: str, default: str | list[str] | None = None):
         result = self.try_get(key, default)
 
         if not isinstance(result, str):
-            raise AttributeSearchError
+            raise AttributeSearchError(self.tag, key)
 
         return result
 
     def get_list(self, key: str, default: str | list[str] | None = None) -> list[str]:
         result = self.tag.get(key, default)
 
         if not isinstance(result, list):
-            raise AttributeSearchError
+            raise AttributeSearchError(self.tag, key)
 
         return result
 
     def encode_contents(self):
         # TODO: Error handling?
         return self.tag.encode_contents()
 
     @property
     def string(self):
-        if not self.tag.string:
-            raise PropertyError
-
-        return str(self.tag.string)
+        return "".join(str(v) for v in self.tag.contents)
 
     @property
     def contents(self):
         if not self.tag.contents:
-            raise PropertyError
+            raise PropertyError(self.tag, "contents")
 
         return self.tag.contents
 
     @property
     def tags(self):
         tags = [SoupTag(e) for e in self.contents if isinstance(e, bs4.element.Tag)]
```

### Comparing `forum_dl-0.2.0/forum_dl/writers/__init__.py` & `forum_dl-0.3.0/forum_dl/writers/__init__.py`

 * *Files identical despite different names*

### Comparing `forum_dl-0.2.0/forum_dl/writers/maildir.py` & `forum_dl-0.3.0/forum_dl/writers/maildir.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # pyright: strict
 from __future__ import annotations
 from typing import *  # type: ignore
 
 from mailbox import Maildir, MaildirMessage
+from email.mime.multipart import MIMEMultipart
 
 from .common import FolderedMailWriter, WriterOptions
 from ..extractors.common import Extractor
 
 
 class MaildirWriter(FolderedMailWriter):
     tests = []
@@ -15,8 +16,8 @@
         super().__init__(
             extractor,
             Maildir(options.output_path),
             options,
         )
 
     def _new_message(self):
-        return MaildirMessage()
+        return MaildirMessage(MIMEMultipart("mixed"))
```

### Comparing `forum_dl-0.2.0/forum_dl/writers/mh.py` & `forum_dl-0.3.0/forum_dl/writers/mh.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 # pyright: strict
 from __future__ import annotations
 from typing import *  # type: ignore
 
 from mailbox import MH, MHMessage
+from email.mime.multipart import MIMEMultipart
 
 from .common import FolderedMailWriter, WriterOptions
 from ..extractors.common import Extractor
 
 
 class MhWriter(FolderedMailWriter):
     tests = []
@@ -15,8 +16,8 @@
         super().__init__(
             extractor,
             MH(options.output_path),
             options,
         )
 
     def _new_message(self):
-        return MHMessage()
+        return MHMessage(MIMEMultipart("mixed"))
```

### Comparing `forum_dl-0.2.0/forum_dl.egg-info/PKG-INFO` & `forum_dl-0.3.0/forum_dl.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: forum-dl
-Version: 0.2.0
-Summary: Download posts and threads from forums, news aggregators, mail archives
+Version: 0.3.0
+Summary: Scrape posts and threads from forums, news aggregators, mail archives
 Author-email: Mikolaj Wielgus <wielgusmikolaj@gmail.com>
 License: MIT
 Project-URL: repository, https://github.com/mikwielgus/forum-dl
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -21,44 +21,44 @@
 
 <sub>The project is currently in alpha stage. Please do not hesitate to [file](https://github.com/mikwielgus/forum-dl/issues) bug reports and feature requests.</sub>
 
 ![image](https://github.com/mikwielgus/forum-dl/assets/58011230/e677d1aa-efa3-4cfc-9283-38408842b278)
 
 # Installation
 
-You can install Forum-dl from [PIP](#pip) or directly from the [repository](#repository).
+You can install stable Forum-dl from [PIP](#pip) or directly from the [repository](#repository).
 
 ## PIP
 
-Install the latest stable version of Forum-dl from PIP:
+Install the latest stable version from PIP:
 
 ```
 pip install forum-dl
 ```
 
 ## Repository 
 
-Clone the repository and install it in editable mode:
+Clone the repository and install the development branch in editable mode:
 
 ```
 git clone https://github.com/mikwielgus/forum-dl && pip install -e forum-dl
 ```
 
 # Usage examples
 
 Download a Simple Machines Forum thread in JSONL format:
 
 ```
 forum-dl "https://www.simplemachines.org/community/index.php?topic=584230.0"
 ```
 
-Download an entire PhpBB board into JSONL format, write to stdout (`-o -`) and record a WARC file in `phpbb.warc`:
+Download a PhpBB subboard into JSONL format, write to stdout (`-o -`) and record a WARC file in `phpbb.warc`:
 
 ```
-forum-dl -o - "https://www.phpbb.com/community/viewforum.php?f=696"
+forum-dl -o - --warc-output phpbb.warc "https://www.phpbb.com/community/viewforum.php?f=696"
 ```
 
 <sub>(due to current architectural limitations, `forum-dl` will scan the first page of each board in the entire forum before downloading the target board. This will be fixed in future releases)</sub>
 
 Download Hacker News top stories and write them to a Maildir directory `hn`:
 
 ```
@@ -95,17 +95,18 @@
 - MH
 - MMDF
 - WARC
 
 # Usage
 
 ```
-forum-dl [--help] [--version] [--list-extractors] [--list-output-formats] [-R RETRIES] [--retry-sleep RETRY_SLEEP]
-         [--retry-sleep-multiplier RETRY_SLEEP_MULTIPLIER] [--user-agent USER_AGENT] [-q] [-v] [-g] [-o FILE] [-f FORMAT]
-         [--warc-output FILE] [--no-boards] [--no-threads] [--no-posts] [--textify] [--content-as-title]
+forum-dl [--help] [--version] [--list-extractors] [--list-output-formats] [--timeout SECONDS] [-R N] [--retry-sleep SECONDS]
+         [--retry-sleep-multiplier K] [--user-agent UA] [-q] [-v] [-g] [-o OUTFILE] [-f FORMAT] [--warc-output FILE]
+         [--files-output DIR] [--boards | --no-boards] [--threads | --no-threads] [--posts | --no-posts]
+         [--files | --no-files] [--outside-files | --no-outside-files] [--textify] [--content-as-title]
          [--author-as-addr-spec]
 ```
 
 ## General Options:
 
 ```
   --help                Show this help message and exit
@@ -114,34 +115,42 @@
   --list-output-formats
                         List all supported output formats and exit
 ```
 
 ## Session Options:
 
 ```
+  --timeout SECONDS     HTTP connection timeout
   -R N, --retries N     Maximum number of retries for failed HTTP requests or -1 to retry infinitely (default: 4)
   --retry-sleep SECONDS
                         Time to sleep between retries, in seconds (default: 1)
   --retry-sleep-multiplier K
                         A constant by which sleep time is multiplied on each retry (default: 2)
   --user-agent UA       User-Agent request header
 ```
 
 ## Output Options:
 
 ```
   -q, --quiet           Activate quiet mode
   -v, --verbose         Print various debugging information
   -g, --get-urls        Print URLs instead of downloading
-  -o FILE, --output FILE
-                        Output all results concatenated to FILE, or stdout if FILE is -
+  -o OUTFILE, --output OUTFILE
+                        Output all results concatenated to OUTFILE, or stdout if OUTFILE is - (default: -)
   -f FORMAT, --output-format FORMAT
                         Output format. Use --list-output-formats for a list of possible arguments
   --warc-output FILE    Record HTTP requests, store them in FILE in WARC format
-  --no-boards           Do not write board objects
-  --no-threads          Do not write thread objects
-  --no-posts            Do not write post objects
+  --files-output DIR    Store files in DIR instead of OUTFILE
+  --boards, --no-boards
+                        Write board objects (default: True, --no-boards to negate)
+  --threads, --no-threads
+                        Write thread objects (default: True, --no-threads to negate)
+  --posts, --no-posts   Write post objects (default: True, --no-posts to negate)
+  --files, --no-files   Write embedded files (--no-files to negate)
+  --outside-files, --no-outside-files
+                        Write embedded files outside post content. Auto-enabled by --warc-output and -f warc (default: False, --no-
+                        outside-files to negate)
   --textify             Lossily convert HTML content to plaintext
   --content-as-title    Write 98 initial characters of content in title field of each post
   --author-as-addr-spec
                         Append author and domain as an addr-spec in the From header
 ```
```

### Comparing `forum_dl-0.2.0/forum_dl.egg-info/SOURCES.txt` & `forum_dl-0.3.0/forum_dl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `forum_dl-0.2.0/pyproject.toml` & `forum_dl-0.3.0/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -2,31 +2,31 @@
 requires = ["setuptools"]
 
 [tool.setuptools]
 packages = ["forum_dl", "forum_dl.extractors", "forum_dl.writers"]
 
 [project]
 name = "forum_dl"
-description = "Download posts and threads from forums, news aggregators, mail archives"
+description = "Scrape posts and threads from forums, news aggregators, mail archives"
 readme = "README.md"
 authors = [
     {name="Mikolaj Wielgus", email="wielgusmikolaj@gmail.com"}
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
     "Topic :: System :: Archiving",
 ]
 
-version = "0.2.0"
+version = "0.3.0"
 license = {text = "MIT"}
 
-dependencies = ["bs4", "lxml", "requests", "urllib3", "cchardet", "tenacity", "python-dateutil", "html2text", "warcio"]
+dependencies = ["pydantic", "beautifulsoup4", "lxml", "requests", "urllib3", "cchardet", "tenacity", "python-dateutil", "html2text", "warcio"]
 requires-python = ">=3.10.11"
 
 [project.urls]
 repository = "https://github.com/mikwielgus/forum-dl"
 
 [project.optional-dependencies]
 test = ["pytest"]
```

