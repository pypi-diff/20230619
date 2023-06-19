# Comparing `tmp/crosslinked-0.2.1.tar.gz` & `tmp/crosslinked-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crosslinked-0.2.1.tar", last modified: Mon Mar 13 11:36:00 2023, max compression
+gzip compressed data, was "crosslinked-0.3.0.tar", last modified: Mon Jun 19 14:10:41 2023, max compression
```

## Comparing `crosslinked-0.2.1.tar` & `crosslinked-0.3.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 11:36:00.605849 crosslinked-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-03-13 11:35:52.000000 crosslinked-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-03-13 11:36:00.605849 crosslinked-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4427 2023-03-13 11:35:52.000000 crosslinked-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 11:36:00.601848 crosslinked-0.2.1/crosslinked/
--rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-03-13 11:35:52.000000 crosslinked-0.2.1/crosslinked/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-03-13 11:35:52.000000 crosslinked-0.2.1/crosslinked/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6659 2023-03-13 11:35:52.000000 crosslinked-0.2.1/crosslinked/search.py
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-03-13 11:35:52.000000 crosslinked-0.2.1/crosslinked/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-13 11:36:00.605849 crosslinked-0.2.1/crosslinked.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-03-13 11:36:00.000000 crosslinked-0.2.1/crosslinked.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      327 2023-03-13 11:36:00.000000 crosslinked-0.2.1/crosslinked.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-13 11:36:00.000000 crosslinked-0.2.1/crosslinked.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-13 11:36:00.000000 crosslinked-0.2.1/crosslinked.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-03-13 11:36:00.000000 crosslinked-0.2.1/crosslinked.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-13 11:36:00.000000 crosslinked-0.2.1/crosslinked.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-13 11:36:00.605849 crosslinked-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-03-13 11:35:52.000000 crosslinked-0.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:10:41.656015 crosslinked-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-06-19 14:10:30.000000 crosslinked-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-06-19 14:10:41.656015 crosslinked-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6019 2023-06-19 14:10:30.000000 crosslinked-0.3.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:10:41.656015 crosslinked-0.3.0/crosslinked/
+-rw-r--r--   0 runner    (1001) docker     (123)     4889 2023-06-19 14:10:30.000000 crosslinked-0.3.0/crosslinked/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2412 2023-06-19 14:10:30.000000 crosslinked-0.3.0/crosslinked/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-06-19 14:10:30.000000 crosslinked-0.3.0/crosslinked/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      613 2023-06-19 14:10:30.000000 crosslinked-0.3.0/crosslinked/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 14:10:41.656015 crosslinked-0.3.0/crosslinked.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6414 2023-06-19 14:10:41.000000 crosslinked-0.3.0/crosslinked.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-06-19 14:10:41.000000 crosslinked-0.3.0/crosslinked.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 14:10:41.000000 crosslinked-0.3.0/crosslinked.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-06-19 14:10:41.000000 crosslinked-0.3.0/crosslinked.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-06-19 14:10:41.000000 crosslinked-0.3.0/crosslinked.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-06-19 14:10:41.000000 crosslinked-0.3.0/crosslinked.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 14:10:41.656015 crosslinked-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      837 2023-06-19 14:10:30.000000 crosslinked-0.3.0/setup.py
```

### Comparing `crosslinked-0.2.1/LICENSE` & `crosslinked-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `crosslinked-0.2.1/PKG-INFO` & `crosslinked-0.3.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,120 +1,152 @@
-Metadata-Version: 2.1
-Name: crosslinked
-Version: 0.2.1
-Home-page: https://github.com/m8sec/CrossLinked
-Author: m8sec
-License: GPLv3
-Classifier: Environment :: Console
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
-Classifier: Topic :: Security
-Description-Content-Type: text/markdown
-License-File: LICENSE
+<div align="center">
+    <h1>CrossLinked</h1>
+</div>
 
-# CrossLinked
 <p align="center">
-    <img src="https://img.shields.io/badge/License-GPL%20v3.0-green?style=plastic"/>&nbsp;
+    <img src="https://img.shields.io/badge/Version-v0.3.0-green"/>&nbsp;
     <a href="https://www.twitter.com/m8sec">
-        <img src="https://img.shields.io/badge/Twitter-@m8sec-blue?style=plastic&logo=twitter"/>
+        <img src="https://img.shields.io/badge/Twitter-@m8sec-gray?logo=twitter"/>
     </a>&nbsp;
-    <a href="https://github.com/sponsors/m8sec">
-        <img src="https://img.shields.io/badge/Sponsor-GitHub-red?style=plastic&logo=github"/>
-    </a>&nbsp;
- </p>
+    <img src="https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8%20|%203.9%20|%203.10%20-blue.svg"/>&nbsp;
+</p>
+
 
 CrossLinked is a LinkedIn enumeration tool that uses search engine scraping to collect valid employee names from an 
 organization. This technique provides accurate results without the use of API keys, credentials, or accessing 
 LinkedIn directly!
 
 
-## Install
+## Table of Contents
+- [Install](#install)
+- [Prerequisites](#prerequisites)
+    + [Naming Format](#naming-format)
+    + [Advanced Formatting](#advanced-formatting)
+- [Search](#search)
+  * [Example Usage](#example-usage)
+  * [Screenshots](#screenshots)
+- [Parse](#parse)
+  * [Example Usage](#example-usage-1)
+  * [Screenshots](#screenshots-1)
+- [Additional Options](#additional-options)
+  * [Proxy Rotation](#proxy-rotation)
+- [Command-Line Arguments](#command-line-arguments)
+- [Contribute](#contribute)
+
+
+# Sponsors
+> 🚩 Consider sponsoring this project to ensure the latest improvements, have your company logo listed here, and get priority support - visit [github.com/sponsors/m8sec](https://github.com/sponsors/m8sec)
+
+
+# Install
 Install the last stable release from PyPi:
 ```commandline
 pip3 install crosslinked
 ```
 Or, install the most recent code from GitHub:
 ```bash
 git clone https://github.com/m8sec/crosslinked
 cd crosslinked
 python3 setup.py install
 ```
 
 
-## Prerequisite
-CrossLinked assumes the organization's account naming convention has already been identified. This is required for execution and should be added to the CMD args based on your expected output. See the `Naming Format` and `Example Usage` sections below:
+# Prerequisites
+CrossLinked assumes the organization's account naming convention has already been identified. This is required for execution and should be added to the CMD args based on your expected output. See the [Naming Format](#naming-format) and [Example Usage](#example-usage) sections below:
 
 ### Naming Format
 ```text
-{f}.{last}              = j.smith
 {first.{last}           = john.smith
 CMP\{first}{l}          = CMP\johns
 {f}{last}@company.com   = jsmith@company.com
 ```
 
-> ***Still Stuck?** Metadata is always a good place to check for hidden information such as account naming convention. see [PyMeta](https://github.com/m8sec/pymeta) for more.*
+> 🦖 ***Still Stuck?** Metadata is always a good place to check for hidden information such as account naming convention. see [PyMeta](https://github.com/m8sec/pymeta) for more.*
+<br>
+
+
+### Advanced Formatting
+:boom: **New Feature** :boom:
+
+To be compatible with alternate naming conventions CrossLinked allows users to control the index position of the name extracted from search text. Should the name not be long enough, or errors encountered with the search string, CrossLinked will revert back to its default format.
+
+***Note**: the search string array starts at `0`. Negative numbers can also be used to count backwards from the last value.*
+
+```
+# Default output
+crosslinked -f '{first}.{last}@company.com' Company
+John David Smith = john.smith@company.com
+
+# Use the second-to-last name as "last"
+crosslinked -f '{0:first}.{-2:last}@company.com' Company
+John David Smith    = john.david@company.com
+Jane Doe            = jane.doe@company.com
+
+# Use the second item in the array as "last"
+crosslinked -f '{first}.{1:last}@company.com' Company
+John David Smith    = john.david@company.com
+Jane Doe            = jane.doe@company.com
+```
 
 
-## Search
+# Search
 By default, CrossLinked will use `google` and `bing` search engines to identify employees of the target organization. After execution, two files (`names.txt` & `names.csv`) will appear in the current directory, unless modified in the CMD args.
 
 * *names.txt* - List of unique user accounts in the specified format.
 * *names.csv* - Raw search data. See the `Parse` section below for more.
 
 
-### Example Usage
+## Example Usage
 ```bash
 python3 crosslinked.py -f '{first}.{last}@domain.com' company_name
 ```
 
+
 ```bash
 python3 crosslinked.py -f 'domain\{f}{last}' -t 15 -j 2 company_name
 ```
+> ⚠️ For best results, use the company name as it appears on LinkedIn `"Target Company"` not the domain name.
 
-> ***Note:** For best results, use the company name as it appears on LinkedIn `"Target Company"` not the domain name.*
 
-
-### Screenshots
+## Screenshots
 ![](https://user-images.githubusercontent.com/13889819/190488899-0f4bea2d-6c31-422f-adce-b56f7be3d906.png)
 
 
-## Parse
-:boom: **New Feature** :boom:
-
+# Parse
 *Account naming convention changed after execution and now your hitting CAPTCHA requests? No Problem!*
 
-CrossLinked v0.2.0 now includes a `names.csv` output file, which stores all scraping data including: `first name`, `last name`, `job title`, and `url`. This can be ingested and parsed to reformat user accounts as needed.
+CrossLinked includes a `names.csv` output file, which stores all scraping data including: `name`, `job title`, and `url`. This can be ingested and parsed to reformat user accounts as needed.
 
-### Example Usage
+
+## Example Usage
 ```
 python3 crosslinked.py -f '{f}{last}@domain.com' names.csv
 ```
 
-### Screenshots
+## Screenshots
 ![](https://user-images.githubusercontent.com/13889819/190494309-c6da8cdc-4312-4e53-a0bb-1fffbc9698e4.png)
 
 
-## Additional Options
-### Proxy Rotation
+# Additional Options
+## Proxy Rotation
 The latest version of CrossLinked provides proxy support to rotate source addresses. Users can input a single proxy with `--proxy 127.0.0.1:8080` or use multiple via `--proxy-file proxies.txt`.
 
 
 ```bash
 > cat proxies.txt
 127.0.0.1:8080
 socks4://111.111.111.111
 socks5://222.222.222.222
 
 > python3 crosslinked.py --proxy-file proxies.txt -f '{first}.{last}@company.com' -t 10 "Company"
 ```
-
-> ***Note:** `HTTP/S` proxies can be added by IP:Port notation. However, socks proxies will require a `socks4://` or `socks5://` prefix.*
+> ⚠️ `HTTP/S` proxies can be added by IP:Port notation. However, socks proxies will require a `socks4://` or `socks5://` prefix.*
 
 
-### Usage
+# Command-Line Arguments
 ```
 positional arguments:
   company_name        Target company name
 
 optional arguments:
   -h, --help          show help message and exit
   -t TIMEOUT          Max timeout per search (Default=15)
@@ -129,12 +161,12 @@
 
 Proxy arguments:
   --proxy PROXY       Proxy requests (IP:Port)
   --proxy-file PROXY  Load proxies from file for rotation
 ```
 
 
-## Contribute
+# Contribute
 Contribute to the project by:
 * Like and share the tool!
 * Create an issue to report any problems or, better yet, initiate a PR.
 * Reach out with any potential features or improvements [@m8sec](https://twitter.com/m8sec).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,60 +1,76 @@
-Metadata-Version: 2.1 Name: crosslinked Version: 0.2.1 Home-page: https://
-github.com/m8sec/CrossLinked Author: m8sec License: GPLv3 Classifier:
-Environment :: Console Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: GNU General Public License v3 or later
-(GPLv3+) Classifier: Topic :: Security Description-Content-Type: text/markdown
-License-File: LICENSE # CrossLinked
-[https://img.shields.io/badge/License-GPL%20v3.0-green?style=plastic]  [https:/
-/img.shields.io/badge/Twitter-@m8sec-blue?style=plastic&logo=twitter]  [https:/
-     /img.shields.io/badge/Sponsor-GitHub-red?style=plastic&logo=github] 
+                           ****** CrossLinked ******
+ [https://img.shields.io/badge/Version-v0.3.0-green]  [https://img.shields.io/
+badge/Twitter-@m8sec-gray?logo=twitter]  [https://img.shields.io/badge/python-
+          3.6%20|%203.7%20|%203.8%20|%203.9%20|%203.10%20-blue.svg] 
 CrossLinked is a LinkedIn enumeration tool that uses search engine scraping to
 collect valid employee names from an organization. This technique provides
 accurate results without the use of API keys, credentials, or accessing
-LinkedIn directly! ## Install Install the last stable release from PyPi:
+LinkedIn directly! ## Table of Contents - [Install](#install) - [Prerequisites]
+(#prerequisites) + [Naming Format](#naming-format) + [Advanced Formatting]
+(#advanced-formatting) - [Search](#search) * [Example Usage](#example-usage) *
+[Screenshots](#screenshots) - [Parse](#parse) * [Example Usage](#example-usage-
+1) * [Screenshots](#screenshots-1) - [Additional Options](#additional-options)
+* [Proxy Rotation](#proxy-rotation) - [Command-Line Arguments](#command-line-
+arguments) - [Contribute](#contribute) # Sponsors > ð© Consider sponsoring
+this project to ensure the latest improvements, have your company logo listed
+here, and get priority support - visit [github.com/sponsors/m8sec](https://
+github.com/sponsors/m8sec) # Install Install the last stable release from PyPi:
 ```commandline pip3 install crosslinked ``` Or, install the most recent code
 from GitHub: ```bash git clone https://github.com/m8sec/crosslinked cd
-crosslinked python3 setup.py install ``` ## Prerequisite CrossLinked assumes
+crosslinked python3 setup.py install ``` # Prerequisites CrossLinked assumes
 the organization's account naming convention has already been identified. This
 is required for execution and should be added to the CMD args based on your
-expected output. See the `Naming Format` and `Example Usage` sections below:
-### Naming Format ```text {f}.{last} = j.smith {first.{last} = john.smith CMP\
-{first}{l} = CMP\johns {f}{last}@company.com = jsmith@company.com ``` >
-***Still Stuck?** Metadata is always a good place to check for hidden
-information such as account naming convention. see [PyMeta](https://github.com/
-m8sec/pymeta) for more.* ## Search By default, CrossLinked will use `google`
-and `bing` search engines to identify employees of the target organization.
-After execution, two files (`names.txt` & `names.csv`) will appear in the
-current directory, unless modified in the CMD args. * *names.txt* - List of
-unique user accounts in the specified format. * *names.csv* - Raw search data.
-See the `Parse` section below for more. ### Example Usage ```bash python3
-crosslinked.py -f '{first}.{last}@domain.com' company_name ``` ```bash python3
-crosslinked.py -f 'domain\{f}{last}' -t 15 -j 2 company_name ``` > ***Note:**
-For best results, use the company name as it appears on LinkedIn `"Target
-Company"` not the domain name.* ### Screenshots ![](https://user-
-images.githubusercontent.com/13889819/190488899-0f4bea2d-6c31-422f-adce-
-b56f7be3d906.png) ## Parse :boom: **New Feature** :boom: *Account naming
+expected output. See the [Naming Format](#naming-format) and [Example Usage]
+(#example-usage) sections below: ### Naming Format ```text {first.{last} =
+john.smith CMP\{first}{l} = CMP\johns {f}{last}@company.com =
+jsmith@company.com ``` > ð¦ ***Still Stuck?** Metadata is always a good place
+to check for hidden information such as account naming convention. see [PyMeta]
+(https://github.com/m8sec/pymeta) for more.*
+### Advanced Formatting :boom: **New Feature** :boom: To be compatible with
+alternate naming conventions CrossLinked allows users to control the index
+position of the name extracted from search text. Should the name not be long
+enough, or errors encountered with the search string, CrossLinked will revert
+back to its default format. ***Note**: the search string array starts at `0`.
+Negative numbers can also be used to count backwards from the last value.* ```
+# Default output crosslinked -f '{first}.{last}@company.com' Company John David
+Smith = john.smith@company.com # Use the second-to-last name as "last"
+crosslinked -f '{0:first}.{-2:last}@company.com' Company John David Smith =
+john.david@company.com Jane Doe = jane.doe@company.com # Use the second item in
+the array as "last" crosslinked -f '{first}.{1:last}@company.com' Company John
+David Smith = john.david@company.com Jane Doe = jane.doe@company.com ``` #
+Search By default, CrossLinked will use `google` and `bing` search engines to
+identify employees of the target organization. After execution, two files
+(`names.txt` & `names.csv`) will appear in the current directory, unless
+modified in the CMD args. * *names.txt* - List of unique user accounts in the
+specified format. * *names.csv* - Raw search data. See the `Parse` section
+below for more. ## Example Usage ```bash python3 crosslinked.py -f '{first}.
+{last}@domain.com' company_name ``` ```bash python3 crosslinked.py -f 'domain\
+{f}{last}' -t 15 -j 2 company_name ``` > â ï¸ For best results, use the
+company name as it appears on LinkedIn `"Target Company"` not the domain name.
+## Screenshots ![](https://user-images.githubusercontent.com/13889819/
+190488899-0f4bea2d-6c31-422f-adce-b56f7be3d906.png) # Parse *Account naming
 convention changed after execution and now your hitting CAPTCHA requests? No
-Problem!* CrossLinked v0.2.0 now includes a `names.csv` output file, which
-stores all scraping data including: `first name`, `last name`, `job title`, and
-`url`. This can be ingested and parsed to reformat user accounts as needed. ###
-Example Usage ``` python3 crosslinked.py -f '{f}{last}@domain.com' names.csv
-``` ### Screenshots ![](https://user-images.githubusercontent.com/13889819/
-190494309-c6da8cdc-4312-4e53-a0bb-1fffbc9698e4.png) ## Additional Options ###
-Proxy Rotation The latest version of CrossLinked provides proxy support to
-rotate source addresses. Users can input a single proxy with `--proxy
-127.0.0.1:8080` or use multiple via `--proxy-file proxies.txt`. ```bash > cat
-proxies.txt 127.0.0.1:8080 socks4://111.111.111.111 socks5://222.222.222.222 >
-python3 crosslinked.py --proxy-file proxies.txt -f '{first}.{last}@company.com'
--t 10 "Company" ``` > ***Note:** `HTTP/S` proxies can be added by IP:Port
-notation. However, socks proxies will require a `socks4://` or `socks5://
-` prefix.* ### Usage ``` positional arguments: company_name Target company name
-optional arguments: -h, --help show help message and exit -t TIMEOUT Max
-timeout per search (Default=15) -j JITTER Jitter between requests (Default=1)
-Search arguments: --search ENGINE Search Engine (Default='google,bing') Output
-arguments: -f NFORMAT Format names, ex: 'domain\{f}{last}', '{first}.
-{last}@domain.com' -o OUTFILE Change name of output file (omit_extension) Proxy
-arguments: --proxy PROXY Proxy requests (IP:Port) --proxy-file PROXY Load
-proxies from file for rotation ``` ## Contribute Contribute to the project by:
-* Like and share the tool! * Create an issue to report any problems or, better
-yet, initiate a PR. * Reach out with any potential features or improvements
-[@m8sec](https://twitter.com/m8sec).
+Problem!* CrossLinked includes a `names.csv` output file, which stores all
+scraping data including: `name`, `job title`, and `url`. This can be ingested
+and parsed to reformat user accounts as needed. ## Example Usage ``` python3
+crosslinked.py -f '{f}{last}@domain.com' names.csv ``` ## Screenshots ![]
+(https://user-images.githubusercontent.com/13889819/190494309-c6da8cdc-4312-
+4e53-a0bb-1fffbc9698e4.png) # Additional Options ## Proxy Rotation The latest
+version of CrossLinked provides proxy support to rotate source addresses. Users
+can input a single proxy with `--proxy 127.0.0.1:8080` or use multiple via `--
+proxy-file proxies.txt`. ```bash > cat proxies.txt 127.0.0.1:8080 socks4://
+111.111.111.111 socks5://222.222.222.222 > python3 crosslinked.py --proxy-file
+proxies.txt -f '{first}.{last}@company.com' -t 10 "Company" ``` > â ï¸ `HTTP/
+S` proxies can be added by IP:Port notation. However, socks proxies will
+require a `socks4://` or `socks5://` prefix.* # Command-Line Arguments ```
+positional arguments: company_name Target company name optional arguments: -h,
+--help show help message and exit -t TIMEOUT Max timeout per search
+(Default=15) -j JITTER Jitter between requests (Default=1) Search arguments: --
+search ENGINE Search Engine (Default='google,bing') Output arguments: -
+f NFORMAT Format names, ex: 'domain\{f}{last}', '{first}.{last}@domain.com' -
+o OUTFILE Change name of output file (omit_extension) Proxy arguments: --proxy
+PROXY Proxy requests (IP:Port) --proxy-file PROXY Load proxies from file for
+rotation ``` # Contribute Contribute to the project by: * Like and share the
+tool! * Create an issue to report any problems or, better yet, initiate a PR. *
+Reach out with any potential features or improvements [@m8sec](https://
+twitter.com/m8sec).
```

### Comparing `crosslinked-0.2.1/README.md` & `crosslinked-0.3.0/PKG-INFO`

 * *Files 24% similar despite different names*

```diff
@@ -1,107 +1,165 @@
-# CrossLinked
+Metadata-Version: 2.1
+Name: crosslinked
+Version: 0.3.0
+Home-page: https://github.com/m8sec/CrossLinked
+Author: m8sec
+License: GPLv3
+Classifier: Environment :: Console
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
+Classifier: Topic :: Security
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+<div align="center">
+    <h1>CrossLinked</h1>
+</div>
+
 <p align="center">
-    <img src="https://img.shields.io/badge/License-GPL%20v3.0-green?style=plastic"/>&nbsp;
+    <img src="https://img.shields.io/badge/Version-v0.3.0-green"/>&nbsp;
     <a href="https://www.twitter.com/m8sec">
-        <img src="https://img.shields.io/badge/Twitter-@m8sec-blue?style=plastic&logo=twitter"/>
-    </a>&nbsp;
-    <a href="https://github.com/sponsors/m8sec">
-        <img src="https://img.shields.io/badge/Sponsor-GitHub-red?style=plastic&logo=github"/>
+        <img src="https://img.shields.io/badge/Twitter-@m8sec-gray?logo=twitter"/>
     </a>&nbsp;
- </p>
+    <img src="https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8%20|%203.9%20|%203.10%20-blue.svg"/>&nbsp;
+</p>
+
 
 CrossLinked is a LinkedIn enumeration tool that uses search engine scraping to collect valid employee names from an 
 organization. This technique provides accurate results without the use of API keys, credentials, or accessing 
 LinkedIn directly!
 
 
-## Install
+## Table of Contents
+- [Install](#install)
+- [Prerequisites](#prerequisites)
+    + [Naming Format](#naming-format)
+    + [Advanced Formatting](#advanced-formatting)
+- [Search](#search)
+  * [Example Usage](#example-usage)
+  * [Screenshots](#screenshots)
+- [Parse](#parse)
+  * [Example Usage](#example-usage-1)
+  * [Screenshots](#screenshots-1)
+- [Additional Options](#additional-options)
+  * [Proxy Rotation](#proxy-rotation)
+- [Command-Line Arguments](#command-line-arguments)
+- [Contribute](#contribute)
+
+
+# Sponsors
+> 🚩 Consider sponsoring this project to ensure the latest improvements, have your company logo listed here, and get priority support - visit [github.com/sponsors/m8sec](https://github.com/sponsors/m8sec)
+
+
+# Install
 Install the last stable release from PyPi:
 ```commandline
 pip3 install crosslinked
 ```
 Or, install the most recent code from GitHub:
 ```bash
 git clone https://github.com/m8sec/crosslinked
 cd crosslinked
 python3 setup.py install
 ```
 
 
-## Prerequisite
-CrossLinked assumes the organization's account naming convention has already been identified. This is required for execution and should be added to the CMD args based on your expected output. See the `Naming Format` and `Example Usage` sections below:
+# Prerequisites
+CrossLinked assumes the organization's account naming convention has already been identified. This is required for execution and should be added to the CMD args based on your expected output. See the [Naming Format](#naming-format) and [Example Usage](#example-usage) sections below:
 
 ### Naming Format
 ```text
-{f}.{last}              = j.smith
 {first.{last}           = john.smith
 CMP\{first}{l}          = CMP\johns
 {f}{last}@company.com   = jsmith@company.com
 ```
 
-> ***Still Stuck?** Metadata is always a good place to check for hidden information such as account naming convention. see [PyMeta](https://github.com/m8sec/pymeta) for more.*
+> 🦖 ***Still Stuck?** Metadata is always a good place to check for hidden information such as account naming convention. see [PyMeta](https://github.com/m8sec/pymeta) for more.*
+<br>
+
+
+### Advanced Formatting
+:boom: **New Feature** :boom:
+
+To be compatible with alternate naming conventions CrossLinked allows users to control the index position of the name extracted from search text. Should the name not be long enough, or errors encountered with the search string, CrossLinked will revert back to its default format.
 
+***Note**: the search string array starts at `0`. Negative numbers can also be used to count backwards from the last value.*
 
-## Search
+```
+# Default output
+crosslinked -f '{first}.{last}@company.com' Company
+John David Smith = john.smith@company.com
+
+# Use the second-to-last name as "last"
+crosslinked -f '{0:first}.{-2:last}@company.com' Company
+John David Smith    = john.david@company.com
+Jane Doe            = jane.doe@company.com
+
+# Use the second item in the array as "last"
+crosslinked -f '{first}.{1:last}@company.com' Company
+John David Smith    = john.david@company.com
+Jane Doe            = jane.doe@company.com
+```
+
+
+# Search
 By default, CrossLinked will use `google` and `bing` search engines to identify employees of the target organization. After execution, two files (`names.txt` & `names.csv`) will appear in the current directory, unless modified in the CMD args.
 
 * *names.txt* - List of unique user accounts in the specified format.
 * *names.csv* - Raw search data. See the `Parse` section below for more.
 
 
-### Example Usage
+## Example Usage
 ```bash
 python3 crosslinked.py -f '{first}.{last}@domain.com' company_name
 ```
 
+
 ```bash
 python3 crosslinked.py -f 'domain\{f}{last}' -t 15 -j 2 company_name
 ```
+> ⚠️ For best results, use the company name as it appears on LinkedIn `"Target Company"` not the domain name.
 
-> ***Note:** For best results, use the company name as it appears on LinkedIn `"Target Company"` not the domain name.*
 
-
-### Screenshots
+## Screenshots
 ![](https://user-images.githubusercontent.com/13889819/190488899-0f4bea2d-6c31-422f-adce-b56f7be3d906.png)
 
 
-## Parse
-:boom: **New Feature** :boom:
-
+# Parse
 *Account naming convention changed after execution and now your hitting CAPTCHA requests? No Problem!*
 
-CrossLinked v0.2.0 now includes a `names.csv` output file, which stores all scraping data including: `first name`, `last name`, `job title`, and `url`. This can be ingested and parsed to reformat user accounts as needed.
+CrossLinked includes a `names.csv` output file, which stores all scraping data including: `name`, `job title`, and `url`. This can be ingested and parsed to reformat user accounts as needed.
 
-### Example Usage
+
+## Example Usage
 ```
 python3 crosslinked.py -f '{f}{last}@domain.com' names.csv
 ```
 
-### Screenshots
+## Screenshots
 ![](https://user-images.githubusercontent.com/13889819/190494309-c6da8cdc-4312-4e53-a0bb-1fffbc9698e4.png)
 
 
-## Additional Options
-### Proxy Rotation
+# Additional Options
+## Proxy Rotation
 The latest version of CrossLinked provides proxy support to rotate source addresses. Users can input a single proxy with `--proxy 127.0.0.1:8080` or use multiple via `--proxy-file proxies.txt`.
 
 
 ```bash
 > cat proxies.txt
 127.0.0.1:8080
 socks4://111.111.111.111
 socks5://222.222.222.222
 
 > python3 crosslinked.py --proxy-file proxies.txt -f '{first}.{last}@company.com' -t 10 "Company"
 ```
-
-> ***Note:** `HTTP/S` proxies can be added by IP:Port notation. However, socks proxies will require a `socks4://` or `socks5://` prefix.*
+> ⚠️ `HTTP/S` proxies can be added by IP:Port notation. However, socks proxies will require a `socks4://` or `socks5://` prefix.*
 
 
-### Usage
+# Command-Line Arguments
 ```
 positional arguments:
   company_name        Target company name
 
 optional arguments:
   -h, --help          show help message and exit
   -t TIMEOUT          Max timeout per search (Default=15)
@@ -116,12 +174,12 @@
 
 Proxy arguments:
   --proxy PROXY       Proxy requests (IP:Port)
   --proxy-file PROXY  Load proxies from file for rotation
 ```
 
 
-## Contribute
+# Contribute
 Contribute to the project by:
 * Like and share the tool!
 * Create an issue to report any problems or, better yet, initiate a PR.
 * Reach out with any potential features or improvements [@m8sec](https://twitter.com/m8sec).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,55 +1,82 @@
-# CrossLinked
-[https://img.shields.io/badge/License-GPL%20v3.0-green?style=plastic]  [https:/
-/img.shields.io/badge/Twitter-@m8sec-blue?style=plastic&logo=twitter]  [https:/
-     /img.shields.io/badge/Sponsor-GitHub-red?style=plastic&logo=github] 
+Metadata-Version: 2.1 Name: crosslinked Version: 0.3.0 Home-page: https://
+github.com/m8sec/CrossLinked Author: m8sec License: GPLv3 Classifier:
+Environment :: Console Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: GNU General Public License v3 or later
+(GPLv3+) Classifier: Topic :: Security Description-Content-Type: text/markdown
+License-File: LICENSE
+                           ****** CrossLinked ******
+ [https://img.shields.io/badge/Version-v0.3.0-green]  [https://img.shields.io/
+badge/Twitter-@m8sec-gray?logo=twitter]  [https://img.shields.io/badge/python-
+          3.6%20|%203.7%20|%203.8%20|%203.9%20|%203.10%20-blue.svg] 
 CrossLinked is a LinkedIn enumeration tool that uses search engine scraping to
 collect valid employee names from an organization. This technique provides
 accurate results without the use of API keys, credentials, or accessing
-LinkedIn directly! ## Install Install the last stable release from PyPi:
+LinkedIn directly! ## Table of Contents - [Install](#install) - [Prerequisites]
+(#prerequisites) + [Naming Format](#naming-format) + [Advanced Formatting]
+(#advanced-formatting) - [Search](#search) * [Example Usage](#example-usage) *
+[Screenshots](#screenshots) - [Parse](#parse) * [Example Usage](#example-usage-
+1) * [Screenshots](#screenshots-1) - [Additional Options](#additional-options)
+* [Proxy Rotation](#proxy-rotation) - [Command-Line Arguments](#command-line-
+arguments) - [Contribute](#contribute) # Sponsors > ð© Consider sponsoring
+this project to ensure the latest improvements, have your company logo listed
+here, and get priority support - visit [github.com/sponsors/m8sec](https://
+github.com/sponsors/m8sec) # Install Install the last stable release from PyPi:
 ```commandline pip3 install crosslinked ``` Or, install the most recent code
 from GitHub: ```bash git clone https://github.com/m8sec/crosslinked cd
-crosslinked python3 setup.py install ``` ## Prerequisite CrossLinked assumes
+crosslinked python3 setup.py install ``` # Prerequisites CrossLinked assumes
 the organization's account naming convention has already been identified. This
 is required for execution and should be added to the CMD args based on your
-expected output. See the `Naming Format` and `Example Usage` sections below:
-### Naming Format ```text {f}.{last} = j.smith {first.{last} = john.smith CMP\
-{first}{l} = CMP\johns {f}{last}@company.com = jsmith@company.com ``` >
-***Still Stuck?** Metadata is always a good place to check for hidden
-information such as account naming convention. see [PyMeta](https://github.com/
-m8sec/pymeta) for more.* ## Search By default, CrossLinked will use `google`
-and `bing` search engines to identify employees of the target organization.
-After execution, two files (`names.txt` & `names.csv`) will appear in the
-current directory, unless modified in the CMD args. * *names.txt* - List of
-unique user accounts in the specified format. * *names.csv* - Raw search data.
-See the `Parse` section below for more. ### Example Usage ```bash python3
-crosslinked.py -f '{first}.{last}@domain.com' company_name ``` ```bash python3
-crosslinked.py -f 'domain\{f}{last}' -t 15 -j 2 company_name ``` > ***Note:**
-For best results, use the company name as it appears on LinkedIn `"Target
-Company"` not the domain name.* ### Screenshots ![](https://user-
-images.githubusercontent.com/13889819/190488899-0f4bea2d-6c31-422f-adce-
-b56f7be3d906.png) ## Parse :boom: **New Feature** :boom: *Account naming
+expected output. See the [Naming Format](#naming-format) and [Example Usage]
+(#example-usage) sections below: ### Naming Format ```text {first.{last} =
+john.smith CMP\{first}{l} = CMP\johns {f}{last}@company.com =
+jsmith@company.com ``` > ð¦ ***Still Stuck?** Metadata is always a good place
+to check for hidden information such as account naming convention. see [PyMeta]
+(https://github.com/m8sec/pymeta) for more.*
+### Advanced Formatting :boom: **New Feature** :boom: To be compatible with
+alternate naming conventions CrossLinked allows users to control the index
+position of the name extracted from search text. Should the name not be long
+enough, or errors encountered with the search string, CrossLinked will revert
+back to its default format. ***Note**: the search string array starts at `0`.
+Negative numbers can also be used to count backwards from the last value.* ```
+# Default output crosslinked -f '{first}.{last}@company.com' Company John David
+Smith = john.smith@company.com # Use the second-to-last name as "last"
+crosslinked -f '{0:first}.{-2:last}@company.com' Company John David Smith =
+john.david@company.com Jane Doe = jane.doe@company.com # Use the second item in
+the array as "last" crosslinked -f '{first}.{1:last}@company.com' Company John
+David Smith = john.david@company.com Jane Doe = jane.doe@company.com ``` #
+Search By default, CrossLinked will use `google` and `bing` search engines to
+identify employees of the target organization. After execution, two files
+(`names.txt` & `names.csv`) will appear in the current directory, unless
+modified in the CMD args. * *names.txt* - List of unique user accounts in the
+specified format. * *names.csv* - Raw search data. See the `Parse` section
+below for more. ## Example Usage ```bash python3 crosslinked.py -f '{first}.
+{last}@domain.com' company_name ``` ```bash python3 crosslinked.py -f 'domain\
+{f}{last}' -t 15 -j 2 company_name ``` > â ï¸ For best results, use the
+company name as it appears on LinkedIn `"Target Company"` not the domain name.
+## Screenshots ![](https://user-images.githubusercontent.com/13889819/
+190488899-0f4bea2d-6c31-422f-adce-b56f7be3d906.png) # Parse *Account naming
 convention changed after execution and now your hitting CAPTCHA requests? No
-Problem!* CrossLinked v0.2.0 now includes a `names.csv` output file, which
-stores all scraping data including: `first name`, `last name`, `job title`, and
-`url`. This can be ingested and parsed to reformat user accounts as needed. ###
-Example Usage ``` python3 crosslinked.py -f '{f}{last}@domain.com' names.csv
-``` ### Screenshots ![](https://user-images.githubusercontent.com/13889819/
-190494309-c6da8cdc-4312-4e53-a0bb-1fffbc9698e4.png) ## Additional Options ###
-Proxy Rotation The latest version of CrossLinked provides proxy support to
-rotate source addresses. Users can input a single proxy with `--proxy
-127.0.0.1:8080` or use multiple via `--proxy-file proxies.txt`. ```bash > cat
-proxies.txt 127.0.0.1:8080 socks4://111.111.111.111 socks5://222.222.222.222 >
-python3 crosslinked.py --proxy-file proxies.txt -f '{first}.{last}@company.com'
--t 10 "Company" ``` > ***Note:** `HTTP/S` proxies can be added by IP:Port
-notation. However, socks proxies will require a `socks4://` or `socks5://
-` prefix.* ### Usage ``` positional arguments: company_name Target company name
-optional arguments: -h, --help show help message and exit -t TIMEOUT Max
-timeout per search (Default=15) -j JITTER Jitter between requests (Default=1)
-Search arguments: --search ENGINE Search Engine (Default='google,bing') Output
-arguments: -f NFORMAT Format names, ex: 'domain\{f}{last}', '{first}.
-{last}@domain.com' -o OUTFILE Change name of output file (omit_extension) Proxy
-arguments: --proxy PROXY Proxy requests (IP:Port) --proxy-file PROXY Load
-proxies from file for rotation ``` ## Contribute Contribute to the project by:
-* Like and share the tool! * Create an issue to report any problems or, better
-yet, initiate a PR. * Reach out with any potential features or improvements
-[@m8sec](https://twitter.com/m8sec).
+Problem!* CrossLinked includes a `names.csv` output file, which stores all
+scraping data including: `name`, `job title`, and `url`. This can be ingested
+and parsed to reformat user accounts as needed. ## Example Usage ``` python3
+crosslinked.py -f '{f}{last}@domain.com' names.csv ``` ## Screenshots ![]
+(https://user-images.githubusercontent.com/13889819/190494309-c6da8cdc-4312-
+4e53-a0bb-1fffbc9698e4.png) # Additional Options ## Proxy Rotation The latest
+version of CrossLinked provides proxy support to rotate source addresses. Users
+can input a single proxy with `--proxy 127.0.0.1:8080` or use multiple via `--
+proxy-file proxies.txt`. ```bash > cat proxies.txt 127.0.0.1:8080 socks4://
+111.111.111.111 socks5://222.222.222.222 > python3 crosslinked.py --proxy-file
+proxies.txt -f '{first}.{last}@company.com' -t 10 "Company" ``` > â ï¸ `HTTP/
+S` proxies can be added by IP:Port notation. However, socks proxies will
+require a `socks4://` or `socks5://` prefix.* # Command-Line Arguments ```
+positional arguments: company_name Target company name optional arguments: -h,
+--help show help message and exit -t TIMEOUT Max timeout per search
+(Default=15) -j JITTER Jitter between requests (Default=1) Search arguments: --
+search ENGINE Search Engine (Default='google,bing') Output arguments: -
+f NFORMAT Format names, ex: 'domain\{f}{last}', '{first}.{last}@domain.com' -
+o OUTFILE Change name of output file (omit_extension) Proxy arguments: --proxy
+PROXY Proxy requests (IP:Port) --proxy-file PROXY Load proxies from file for
+rotation ``` # Contribute Contribute to the project by: * Like and share the
+tool! * Create an issue to report any problems or, better yet, initiate a PR. *
+Reach out with any potential features or improvements [@m8sec](https://
+twitter.com/m8sec).
```

### Comparing `crosslinked-0.2.1/crosslinked/__init__.py` & `crosslinked-0.3.0/crosslinked/__init__.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 #!/usr/bin/env python3
 # Author: @m8sec
 # License: GPLv3
-
+import re
 import argparse
 from sys import exit
 from csv import reader
 from crosslinked import utils
 from crosslinked.logger import *
 from crosslinked.search import CrossLinked
 
 
 def banner():
 
-    VERSION = 'v0.2.1'
+    VERSION = 'v0.3.0'
 
     print('''
      _____                    _             _            _ 
     /  __ \                  | |   ({})     | |          | |
     | /  \/_ __ ___  ___ ___ | |    _ _ __ | | _____  __| |
     | |   | '__/ _ \/ __/ __|| |   | | '_ \| |/ / _ \/ _` |
     | \__/\ | | (_) \__ \__ \| |___| | | | |   <  __/ (_| | {}
@@ -60,44 +60,56 @@
 
 
 def start_parse(args):
     tmp = []
     utils.file_exists(args.company_name, contents=False)
     Log.info('Parsing employee names from \"{}\"'.format(args.company_name))
 
-    with open(args.company_name) as f:
+    with open(args.company_name, 'r') as f:
         csv_data = reader(f, delimiter=',')
         next(csv_data)
         for r in csv_data:
-            tmp.append({'fname': r[2], 'lname': r[3]})
+            tmp.append({'name': r[2].strip()}) if r[2] else False
     return tmp
 
 
 def format_names(args, data, logger):
     tmp = []
     Log.info('{} names collected'.format(len(data)))
 
     for d in data:
-        fname = d['fname'].lower().strip()
-        lname = d['lname'].lower().strip()
-        name = nformatter(args.nformat, fname, lname)
+        name = nformatter(args.nformat, d['name'])
         if name not in tmp:
             logger.info(name)
             tmp.append(name)
     Log.success("{} unique names added to {}!".format(len(tmp), args.outfile+".txt"))
 
 
-def nformatter(nformat, first, last):
-    # place names in user-defined format
-    name = nformat
-    name = name.replace('{f}', first[0])
-    name = name.replace('{first}', first)
-    name = name.replace('{l}', last[0])
-    name = name.replace('{last}', last)
-    return name
+def nformatter(nformat, name):
+    # Get position of name values in text
+    tmp = nformat.split('}')
+    f_position = int(re.search(r'(-?\d+)', tmp[0]).group(0)) if ':' in tmp[0] else 0
+    l_position = int(re.search(r'(-?\d+)', tmp[1]).group(0)) if ':' in tmp[1] else -1
+
+    # Extract names from raw text
+    tmp = name.split(' ')
+    try:
+        f_name = tmp[f_position] if len(tmp) > 2 else tmp[0]
+        l_name = tmp[l_position] if len(tmp) > 2 else tmp[-1]
+    except:
+        f_name = tmp[0]
+        l_name = tmp[-1]
+
+    # Use replace function to create final output
+    val = re.sub(r'-?\d+:', '', nformat)
+    val = val.replace('{f}', f_name[0])
+    val = val.replace('{first}', f_name)
+    val = val.replace('{l}', l_name[0])
+    val = val.replace('{last}', l_name)
+    return val
 
 
 def main():
     banner()
     args = cli()
 
     try:
```

### Comparing `crosslinked-0.2.1/crosslinked/logger.py` & `crosslinked-0.3.0/crosslinked/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,33 +55,30 @@
     root_logger.propagate = False
     root_logger.addHandler(streamHandler)
     root_logger.setLevel(logging.DEBUG)
     return root_logger
 
 
 def setup_file_logger(file_name, log_name='cLinked_file', file_mode='w'):
-    init = False if os.path.exists(file_name) else True
-
     formatter = logging.Formatter('%(message)s')
     fileHandler = logging.FileHandler(file_name, file_mode)
     fileHandler.setFormatter(formatter)
 
     logger = logging.getLogger(log_name)
     logger.propagate = False
     logger.addHandler(fileHandler)
     logger.setLevel(logging.INFO)
 
-    first_run(logger) if init else False
-
+    first_run(logger) if not os.path.exists(file_name) else False
     return logger
 
 
 def first_run(logger):
     # init headings in CSV log file
-    logger.info('Datetime, Search, First, Last, Title, URL, rawText')
+    logger.info('Datetime, Search, Name, Title, URL, rawText')
 
 
 def setup_cli_logger(log_level=logging.INFO, logger_name='cLinked'):
     formatter = logging.Formatter('%(message)s')
     StreamHandler = logging.StreamHandler(sys.stdout)
     StreamHandler.setFormatter(formatter)
```

### Comparing `crosslinked-0.2.1/crosslinked/search.py` & `crosslinked-0.3.0/crosslinked/search.py`

 * *Files 15% similar despite different names*

```diff
@@ -84,61 +84,54 @@
             except Exception as e:
                 Log.warn('Failed Parsing: {}- {}'.format(link.get('href'), e))
 
     def link_parser(self, url, link):
         u = {'url': url}
         u['text'] = unidecode(link.text.split("|")[0].split("...")[0])  # Capture link text before trailing chars
         u['title'] = self.parse_linkedin_title(u['text'])               # Extract job title
-        u['fname'] = self.parse_linkedin_fname(u['text'])               # Extract first name
-        u['lname'] = self.parse_linkedin_lname(u['text'])               # Extract last name
+        u['name'] = self.parse_linkedin_name(u['text'])                 # Extract whole name
         return u
 
     def parse_linkedin_title(self, data):
         try:
             title = data.split("-")[1].split('https:')[0]
             return title.split("...")[0].split("|")[0].strip()
         except:
             return 'N/A'
 
-    def parse_linkedin_fname(self, data):
+    def parse_linkedin_name(self, data):
         try:
-            fname = data.split("-")[0].split(' ')[0].strip()
-            fname = fname.replace("'", "")
-            return unidecode(fname)
-        except:
-            return False
-
-    def parse_linkedin_lname(self, data):
-        try:
-            name = list(filter(None, data.split("-")[0].split(' ')))
-            lname = name[-1].strip()
-            return unidecode(lname[:-1]) if lname.endswith(".") else unidecode(lname)
+            name = data.split("-")[0].strip()
+            return unidecode(name)
         except:
             return False
 
     def results_handler(self, link):
         url = str(link.get('href')).lower()
 
         if not extract_subdomain(url).endswith('linkedin.com'):
             return False
         elif 'linkedin.com/in' not in url:
             return False
 
         data = self.link_parser(url, link)
-        if data['fname'] and data['lname']:
-            self.log_results(data)
+        self.log_results(data) if data['name'] else False
+
 
-    def log_results(self, data):
-        if data in self.results:
+    def log_results(self, d):
+        # Prevent Duplicates & non-standard responses (i.e: "<span>linkedin.com</span></a>")
+        if d in self.results:
             return
-        self.results.append(data)
+        elif 'linkedin.com' in d['name']:
+            return
+
+        self.results.append(d)
         # Search results are logged to names.csv but names.txt is not generated until end to prevent duplicates
-        logging.debug('  Fname: {:13} Lname: {:13} RawTxt: {}'.format(data['fname'], data['lname'], data['text']))
-        csv.info('"{}","{}","{}","{}","{}","{}","{}",'.format(self.runtime, self.search_engine, data['fname'],
-                                                           data['lname'], data['title'], data['url'], data['text']))
+        logging.debug('name: {:25} RawTxt: {}'.format(d['name'], d['text']))
+        csv.info('"{}","{}","{}","{}","{}","{}",'.format(self.runtime, self.search_engine, d['name'], d['title'], d['url'], d['text']))
 
 
 def get_statuscode(resp):
     try:
         return resp.status_code
     except:
         return 0
@@ -147,20 +140,23 @@
 def get_proxy(proxies):
     tmp = choice(proxies) if proxies else False
     return {"http": tmp, "https": tmp} if tmp else {}
 
 
 def get_agent():
     return choice([
-        'Mozilla/5.0 (Macintosh; Intel Mac OS X 12.5; rv:104.0) Gecko/20100101 Firefox/104.0',
-        'Mozilla/5.0 (Windows NT 10.0) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/105.0.0.0 Safari/537.36',
-        'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/105.0.0.0 Safari/537.36',
-        'Mozilla/5.0 (Windows NT 10.0; WOW64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/105.0.0.0 Safari/537.36',
-        'Mozilla/5.0 (Macintosh; Intel Mac OS X 12_5_1) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/105.0.0.0 Safari/537.36',
         'Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:104.0) Gecko/20100101 Firefox/104.0'
+        'Mozilla/5.0 (Macintosh; Intel Mac OS X 12.5; rv:104.0) Gecko/20100101 Firefox/104.0',
+        'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36',
+        'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/109.0.0.0 Safari/537.36',
+        'Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36',
+        'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36',
+        'Mozilla/5.0 (X11; Linux x86_64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/108.0.0.0 Safari/537.36',
+        'Mozilla/5.0 (Macintosh; Intel Mac OS X 10_15_7) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.1 Safari/605.1.15',
+        'Mozilla/5.0 (Macintosh; Intel Mac OS X 13_1) AppleWebKit/605.1.15 (KHTML, like Gecko) Version/16.1 Safari/605.1.15'
     ])
 
 
 def web_request(url, timeout=3, proxies=[], **kwargs):
     try:
         s = requests.Session()
         r = requests.Request('GET', url, headers={'User-Agent': get_agent()}, cookies = {'CONSENT' : 'YES'}, **kwargs)
```

### Comparing `crosslinked-0.2.1/crosslinked/utils.py` & `crosslinked-0.3.0/crosslinked/utils.py`

 * *Files identical despite different names*

### Comparing `crosslinked-0.2.1/crosslinked.egg-info/PKG-INFO` & `crosslinked-0.3.0/crosslinked.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,120 +1,165 @@
 Metadata-Version: 2.1
 Name: crosslinked
-Version: 0.2.1
+Version: 0.3.0
 Home-page: https://github.com/m8sec/CrossLinked
 Author: m8sec
 License: GPLv3
 Classifier: Environment :: Console
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Classifier: Topic :: Security
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# CrossLinked
+<div align="center">
+    <h1>CrossLinked</h1>
+</div>
+
 <p align="center">
-    <img src="https://img.shields.io/badge/License-GPL%20v3.0-green?style=plastic"/>&nbsp;
+    <img src="https://img.shields.io/badge/Version-v0.3.0-green"/>&nbsp;
     <a href="https://www.twitter.com/m8sec">
-        <img src="https://img.shields.io/badge/Twitter-@m8sec-blue?style=plastic&logo=twitter"/>
-    </a>&nbsp;
-    <a href="https://github.com/sponsors/m8sec">
-        <img src="https://img.shields.io/badge/Sponsor-GitHub-red?style=plastic&logo=github"/>
+        <img src="https://img.shields.io/badge/Twitter-@m8sec-gray?logo=twitter"/>
     </a>&nbsp;
- </p>
+    <img src="https://img.shields.io/badge/python-3.6%20|%203.7%20|%203.8%20|%203.9%20|%203.10%20-blue.svg"/>&nbsp;
+</p>
+
 
 CrossLinked is a LinkedIn enumeration tool that uses search engine scraping to collect valid employee names from an 
 organization. This technique provides accurate results without the use of API keys, credentials, or accessing 
 LinkedIn directly!
 
 
-## Install
+## Table of Contents
+- [Install](#install)
+- [Prerequisites](#prerequisites)
+    + [Naming Format](#naming-format)
+    + [Advanced Formatting](#advanced-formatting)
+- [Search](#search)
+  * [Example Usage](#example-usage)
+  * [Screenshots](#screenshots)
+- [Parse](#parse)
+  * [Example Usage](#example-usage-1)
+  * [Screenshots](#screenshots-1)
+- [Additional Options](#additional-options)
+  * [Proxy Rotation](#proxy-rotation)
+- [Command-Line Arguments](#command-line-arguments)
+- [Contribute](#contribute)
+
+
+# Sponsors
+> 🚩 Consider sponsoring this project to ensure the latest improvements, have your company logo listed here, and get priority support - visit [github.com/sponsors/m8sec](https://github.com/sponsors/m8sec)
+
+
+# Install
 Install the last stable release from PyPi:
 ```commandline
 pip3 install crosslinked
 ```
 Or, install the most recent code from GitHub:
 ```bash
 git clone https://github.com/m8sec/crosslinked
 cd crosslinked
 python3 setup.py install
 ```
 
 
-## Prerequisite
-CrossLinked assumes the organization's account naming convention has already been identified. This is required for execution and should be added to the CMD args based on your expected output. See the `Naming Format` and `Example Usage` sections below:
+# Prerequisites
+CrossLinked assumes the organization's account naming convention has already been identified. This is required for execution and should be added to the CMD args based on your expected output. See the [Naming Format](#naming-format) and [Example Usage](#example-usage) sections below:
 
 ### Naming Format
 ```text
-{f}.{last}              = j.smith
 {first.{last}           = john.smith
 CMP\{first}{l}          = CMP\johns
 {f}{last}@company.com   = jsmith@company.com
 ```
 
-> ***Still Stuck?** Metadata is always a good place to check for hidden information such as account naming convention. see [PyMeta](https://github.com/m8sec/pymeta) for more.*
+> 🦖 ***Still Stuck?** Metadata is always a good place to check for hidden information such as account naming convention. see [PyMeta](https://github.com/m8sec/pymeta) for more.*
+<br>
+
+
+### Advanced Formatting
+:boom: **New Feature** :boom:
+
+To be compatible with alternate naming conventions CrossLinked allows users to control the index position of the name extracted from search text. Should the name not be long enough, or errors encountered with the search string, CrossLinked will revert back to its default format.
 
+***Note**: the search string array starts at `0`. Negative numbers can also be used to count backwards from the last value.*
 
-## Search
+```
+# Default output
+crosslinked -f '{first}.{last}@company.com' Company
+John David Smith = john.smith@company.com
+
+# Use the second-to-last name as "last"
+crosslinked -f '{0:first}.{-2:last}@company.com' Company
+John David Smith    = john.david@company.com
+Jane Doe            = jane.doe@company.com
+
+# Use the second item in the array as "last"
+crosslinked -f '{first}.{1:last}@company.com' Company
+John David Smith    = john.david@company.com
+Jane Doe            = jane.doe@company.com
+```
+
+
+# Search
 By default, CrossLinked will use `google` and `bing` search engines to identify employees of the target organization. After execution, two files (`names.txt` & `names.csv`) will appear in the current directory, unless modified in the CMD args.
 
 * *names.txt* - List of unique user accounts in the specified format.
 * *names.csv* - Raw search data. See the `Parse` section below for more.
 
 
-### Example Usage
+## Example Usage
 ```bash
 python3 crosslinked.py -f '{first}.{last}@domain.com' company_name
 ```
 
+
 ```bash
 python3 crosslinked.py -f 'domain\{f}{last}' -t 15 -j 2 company_name
 ```
+> ⚠️ For best results, use the company name as it appears on LinkedIn `"Target Company"` not the domain name.
 
-> ***Note:** For best results, use the company name as it appears on LinkedIn `"Target Company"` not the domain name.*
 
-
-### Screenshots
+## Screenshots
 ![](https://user-images.githubusercontent.com/13889819/190488899-0f4bea2d-6c31-422f-adce-b56f7be3d906.png)
 
 
-## Parse
-:boom: **New Feature** :boom:
-
+# Parse
 *Account naming convention changed after execution and now your hitting CAPTCHA requests? No Problem!*
 
-CrossLinked v0.2.0 now includes a `names.csv` output file, which stores all scraping data including: `first name`, `last name`, `job title`, and `url`. This can be ingested and parsed to reformat user accounts as needed.
+CrossLinked includes a `names.csv` output file, which stores all scraping data including: `name`, `job title`, and `url`. This can be ingested and parsed to reformat user accounts as needed.
 
-### Example Usage
+
+## Example Usage
 ```
 python3 crosslinked.py -f '{f}{last}@domain.com' names.csv
 ```
 
-### Screenshots
+## Screenshots
 ![](https://user-images.githubusercontent.com/13889819/190494309-c6da8cdc-4312-4e53-a0bb-1fffbc9698e4.png)
 
 
-## Additional Options
-### Proxy Rotation
+# Additional Options
+## Proxy Rotation
 The latest version of CrossLinked provides proxy support to rotate source addresses. Users can input a single proxy with `--proxy 127.0.0.1:8080` or use multiple via `--proxy-file proxies.txt`.
 
 
 ```bash
 > cat proxies.txt
 127.0.0.1:8080
 socks4://111.111.111.111
 socks5://222.222.222.222
 
 > python3 crosslinked.py --proxy-file proxies.txt -f '{first}.{last}@company.com' -t 10 "Company"
 ```
-
-> ***Note:** `HTTP/S` proxies can be added by IP:Port notation. However, socks proxies will require a `socks4://` or `socks5://` prefix.*
+> ⚠️ `HTTP/S` proxies can be added by IP:Port notation. However, socks proxies will require a `socks4://` or `socks5://` prefix.*
 
 
-### Usage
+# Command-Line Arguments
 ```
 positional arguments:
   company_name        Target company name
 
 optional arguments:
   -h, --help          show help message and exit
   -t TIMEOUT          Max timeout per search (Default=15)
@@ -129,12 +174,12 @@
 
 Proxy arguments:
   --proxy PROXY       Proxy requests (IP:Port)
   --proxy-file PROXY  Load proxies from file for rotation
 ```
 
 
-## Contribute
+# Contribute
 Contribute to the project by:
 * Like and share the tool!
 * Create an issue to report any problems or, better yet, initiate a PR.
 * Reach out with any potential features or improvements [@m8sec](https://twitter.com/m8sec).
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

#### html2text {}

```diff
@@ -1,60 +1,82 @@
-Metadata-Version: 2.1 Name: crosslinked Version: 0.2.1 Home-page: https://
+Metadata-Version: 2.1 Name: crosslinked Version: 0.3.0 Home-page: https://
 github.com/m8sec/CrossLinked Author: m8sec License: GPLv3 Classifier:
 Environment :: Console Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later
 (GPLv3+) Classifier: Topic :: Security Description-Content-Type: text/markdown
-License-File: LICENSE # CrossLinked
-[https://img.shields.io/badge/License-GPL%20v3.0-green?style=plastic]  [https:/
-/img.shields.io/badge/Twitter-@m8sec-blue?style=plastic&logo=twitter]  [https:/
-     /img.shields.io/badge/Sponsor-GitHub-red?style=plastic&logo=github] 
+License-File: LICENSE
+                           ****** CrossLinked ******
+ [https://img.shields.io/badge/Version-v0.3.0-green]  [https://img.shields.io/
+badge/Twitter-@m8sec-gray?logo=twitter]  [https://img.shields.io/badge/python-
+          3.6%20|%203.7%20|%203.8%20|%203.9%20|%203.10%20-blue.svg] 
 CrossLinked is a LinkedIn enumeration tool that uses search engine scraping to
 collect valid employee names from an organization. This technique provides
 accurate results without the use of API keys, credentials, or accessing
-LinkedIn directly! ## Install Install the last stable release from PyPi:
+LinkedIn directly! ## Table of Contents - [Install](#install) - [Prerequisites]
+(#prerequisites) + [Naming Format](#naming-format) + [Advanced Formatting]
+(#advanced-formatting) - [Search](#search) * [Example Usage](#example-usage) *
+[Screenshots](#screenshots) - [Parse](#parse) * [Example Usage](#example-usage-
+1) * [Screenshots](#screenshots-1) - [Additional Options](#additional-options)
+* [Proxy Rotation](#proxy-rotation) - [Command-Line Arguments](#command-line-
+arguments) - [Contribute](#contribute) # Sponsors > ð© Consider sponsoring
+this project to ensure the latest improvements, have your company logo listed
+here, and get priority support - visit [github.com/sponsors/m8sec](https://
+github.com/sponsors/m8sec) # Install Install the last stable release from PyPi:
 ```commandline pip3 install crosslinked ``` Or, install the most recent code
 from GitHub: ```bash git clone https://github.com/m8sec/crosslinked cd
-crosslinked python3 setup.py install ``` ## Prerequisite CrossLinked assumes
+crosslinked python3 setup.py install ``` # Prerequisites CrossLinked assumes
 the organization's account naming convention has already been identified. This
 is required for execution and should be added to the CMD args based on your
-expected output. See the `Naming Format` and `Example Usage` sections below:
-### Naming Format ```text {f}.{last} = j.smith {first.{last} = john.smith CMP\
-{first}{l} = CMP\johns {f}{last}@company.com = jsmith@company.com ``` >
-***Still Stuck?** Metadata is always a good place to check for hidden
-information such as account naming convention. see [PyMeta](https://github.com/
-m8sec/pymeta) for more.* ## Search By default, CrossLinked will use `google`
-and `bing` search engines to identify employees of the target organization.
-After execution, two files (`names.txt` & `names.csv`) will appear in the
-current directory, unless modified in the CMD args. * *names.txt* - List of
-unique user accounts in the specified format. * *names.csv* - Raw search data.
-See the `Parse` section below for more. ### Example Usage ```bash python3
-crosslinked.py -f '{first}.{last}@domain.com' company_name ``` ```bash python3
-crosslinked.py -f 'domain\{f}{last}' -t 15 -j 2 company_name ``` > ***Note:**
-For best results, use the company name as it appears on LinkedIn `"Target
-Company"` not the domain name.* ### Screenshots ![](https://user-
-images.githubusercontent.com/13889819/190488899-0f4bea2d-6c31-422f-adce-
-b56f7be3d906.png) ## Parse :boom: **New Feature** :boom: *Account naming
+expected output. See the [Naming Format](#naming-format) and [Example Usage]
+(#example-usage) sections below: ### Naming Format ```text {first.{last} =
+john.smith CMP\{first}{l} = CMP\johns {f}{last}@company.com =
+jsmith@company.com ``` > ð¦ ***Still Stuck?** Metadata is always a good place
+to check for hidden information such as account naming convention. see [PyMeta]
+(https://github.com/m8sec/pymeta) for more.*
+### Advanced Formatting :boom: **New Feature** :boom: To be compatible with
+alternate naming conventions CrossLinked allows users to control the index
+position of the name extracted from search text. Should the name not be long
+enough, or errors encountered with the search string, CrossLinked will revert
+back to its default format. ***Note**: the search string array starts at `0`.
+Negative numbers can also be used to count backwards from the last value.* ```
+# Default output crosslinked -f '{first}.{last}@company.com' Company John David
+Smith = john.smith@company.com # Use the second-to-last name as "last"
+crosslinked -f '{0:first}.{-2:last}@company.com' Company John David Smith =
+john.david@company.com Jane Doe = jane.doe@company.com # Use the second item in
+the array as "last" crosslinked -f '{first}.{1:last}@company.com' Company John
+David Smith = john.david@company.com Jane Doe = jane.doe@company.com ``` #
+Search By default, CrossLinked will use `google` and `bing` search engines to
+identify employees of the target organization. After execution, two files
+(`names.txt` & `names.csv`) will appear in the current directory, unless
+modified in the CMD args. * *names.txt* - List of unique user accounts in the
+specified format. * *names.csv* - Raw search data. See the `Parse` section
+below for more. ## Example Usage ```bash python3 crosslinked.py -f '{first}.
+{last}@domain.com' company_name ``` ```bash python3 crosslinked.py -f 'domain\
+{f}{last}' -t 15 -j 2 company_name ``` > â ï¸ For best results, use the
+company name as it appears on LinkedIn `"Target Company"` not the domain name.
+## Screenshots ![](https://user-images.githubusercontent.com/13889819/
+190488899-0f4bea2d-6c31-422f-adce-b56f7be3d906.png) # Parse *Account naming
 convention changed after execution and now your hitting CAPTCHA requests? No
-Problem!* CrossLinked v0.2.0 now includes a `names.csv` output file, which
-stores all scraping data including: `first name`, `last name`, `job title`, and
-`url`. This can be ingested and parsed to reformat user accounts as needed. ###
-Example Usage ``` python3 crosslinked.py -f '{f}{last}@domain.com' names.csv
-``` ### Screenshots ![](https://user-images.githubusercontent.com/13889819/
-190494309-c6da8cdc-4312-4e53-a0bb-1fffbc9698e4.png) ## Additional Options ###
-Proxy Rotation The latest version of CrossLinked provides proxy support to
-rotate source addresses. Users can input a single proxy with `--proxy
-127.0.0.1:8080` or use multiple via `--proxy-file proxies.txt`. ```bash > cat
-proxies.txt 127.0.0.1:8080 socks4://111.111.111.111 socks5://222.222.222.222 >
-python3 crosslinked.py --proxy-file proxies.txt -f '{first}.{last}@company.com'
--t 10 "Company" ``` > ***Note:** `HTTP/S` proxies can be added by IP:Port
-notation. However, socks proxies will require a `socks4://` or `socks5://
-` prefix.* ### Usage ``` positional arguments: company_name Target company name
-optional arguments: -h, --help show help message and exit -t TIMEOUT Max
-timeout per search (Default=15) -j JITTER Jitter between requests (Default=1)
-Search arguments: --search ENGINE Search Engine (Default='google,bing') Output
-arguments: -f NFORMAT Format names, ex: 'domain\{f}{last}', '{first}.
-{last}@domain.com' -o OUTFILE Change name of output file (omit_extension) Proxy
-arguments: --proxy PROXY Proxy requests (IP:Port) --proxy-file PROXY Load
-proxies from file for rotation ``` ## Contribute Contribute to the project by:
-* Like and share the tool! * Create an issue to report any problems or, better
-yet, initiate a PR. * Reach out with any potential features or improvements
-[@m8sec](https://twitter.com/m8sec).
+Problem!* CrossLinked includes a `names.csv` output file, which stores all
+scraping data including: `name`, `job title`, and `url`. This can be ingested
+and parsed to reformat user accounts as needed. ## Example Usage ``` python3
+crosslinked.py -f '{f}{last}@domain.com' names.csv ``` ## Screenshots ![]
+(https://user-images.githubusercontent.com/13889819/190494309-c6da8cdc-4312-
+4e53-a0bb-1fffbc9698e4.png) # Additional Options ## Proxy Rotation The latest
+version of CrossLinked provides proxy support to rotate source addresses. Users
+can input a single proxy with `--proxy 127.0.0.1:8080` or use multiple via `--
+proxy-file proxies.txt`. ```bash > cat proxies.txt 127.0.0.1:8080 socks4://
+111.111.111.111 socks5://222.222.222.222 > python3 crosslinked.py --proxy-file
+proxies.txt -f '{first}.{last}@company.com' -t 10 "Company" ``` > â ï¸ `HTTP/
+S` proxies can be added by IP:Port notation. However, socks proxies will
+require a `socks4://` or `socks5://` prefix.* # Command-Line Arguments ```
+positional arguments: company_name Target company name optional arguments: -h,
+--help show help message and exit -t TIMEOUT Max timeout per search
+(Default=15) -j JITTER Jitter between requests (Default=1) Search arguments: --
+search ENGINE Search Engine (Default='google,bing') Output arguments: -
+f NFORMAT Format names, ex: 'domain\{f}{last}', '{first}.{last}@domain.com' -
+o OUTFILE Change name of output file (omit_extension) Proxy arguments: --proxy
+PROXY Proxy requests (IP:Port) --proxy-file PROXY Load proxies from file for
+rotation ``` # Contribute Contribute to the project by: * Like and share the
+tool! * Create an issue to report any problems or, better yet, initiate a PR. *
+Reach out with any potential features or improvements [@m8sec](https://
+twitter.com/m8sec).
```

### Comparing `crosslinked-0.2.1/setup.py` & `crosslinked-0.3.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name='crosslinked',
-    version='0.2.1',
+    version='0.3.0',
     author='m8sec',
     license='GPLv3',
     long_description=long_description,
     long_description_content_type="text/markdown",
     url='https://github.com/m8sec/CrossLinked',
     packages=find_packages(include=[
         "crosslinked", "crosslinked.*"
     ]),
     install_requires=[
-        'bs4>=0.0.1',
-        'lxml>=4.9.1',
-        'requests>=2.28.1',
-        'Unidecode>=1.3.4'
+        'bs4',
+        'lxml',
+        'requests',
+        'Unidecode'
     ],
     classifiers=[
         "Environment :: Console",
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
         "Topic :: Security"
     ],
```

