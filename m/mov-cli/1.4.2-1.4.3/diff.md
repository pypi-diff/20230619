# Comparing `tmp/mov_cli-1.4.2.tar.gz` & `tmp/mov_cli-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mov_cli-1.4.2.tar", max compression
+gzip compressed data, was "mov_cli-1.4.3.tar", max compression
```

## Comparing `mov_cli-1.4.2.tar` & `mov_cli-1.4.3.tar`

### file list

```diff
@@ -1,59 +1,58 @@
--rw-r--r--   0        0        0    35149 2023-06-08 17:52:38.724717 mov_cli-1.4.2/LICENSE
--rw-r--r--   0        0        0     7155 2023-06-08 17:52:38.724717 mov_cli-1.4.2/README.md
--rw-r--r--   0        0        0      235 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/__init__.py
--rw-r--r--   0        0        0     2700 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/__main__.py
--rw-r--r--   0        0        0        1 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/__init__.py
--rw-r--r--   0        0        0      823 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/doodstream.py
--rw-r--r--   0        0        0       71 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/NOTICE
--rw-r--r--   0        0        0        1 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/__init__.py
--rw-r--r--   0        0        0      169 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/allsportsdaily.py
--rw-r--r--   0        0        0      958 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/cr7sports.py
--rw-r--r--   0        0        0      256 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/enjoy4hd.py
--rw-r--r--   0        0        0      141 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/fabtech.py
--rw-r--r--   0        0        0      218 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/gameshdlive.py
--rw-r--r--   0        0        0      457 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/livestreames.py
--rw-r--r--   0        0        0      318 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/methstreams.py
--rw-r--r--   0        0        0      156 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/motornews.py
--rw-r--r--   0        0        0      873 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/onestream.py
--rw-r--r--   0        0        0      891 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/onionlive.py
--rw-r--r--   0        0        0      615 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/onionstream.py
--rw-r--r--   0        0        0      457 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/poscitech.py
--rw-r--r--   0        0        0      638 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/rainostreams.py
--rw-r--r--   0        0        0      358 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/ripple.py
--rw-r--r--   0        0        0      406 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/techclips.py
--rw-r--r--   0        0        0      417 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/techstips.py
--rw-r--r--   0        0        0     1333 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/extractors/scdn/weakstream.py
--rw-r--r--   0        0        0        0 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/players/__init__.py
--rw-r--r--   0        0        0     2559 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/players/player.py
--rw-r--r--   0        0        0        0 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/utils/__init__.py
--rw-r--r--   0        0        0     1483 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/utils/dbs.py
--rw-r--r--   0        0        0     2731 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/utils/httpclient.py
--rw-r--r--   0        0        0     6133 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/utils/jsunpack.py
--rw-r--r--   0        0        0     2269 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/utils/lang.py
--rw-r--r--   0        0        0     1592 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/utils/player.py
--rw-r--r--   0        0        0      941 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/utils/provider.py
--rw-r--r--   0        0        0     8714 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/utils/scraper.py
--rw-r--r--   0        0        0        0 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/__init__.py
--rw-r--r--   0        0        0    11020 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/actvid.py
--rw-r--r--   0        0        0     4177 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/animefox.py
--rw-r--r--   0        0        0     4112 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/dopebox.py
--rw-r--r--   0        0        0     1943 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/einthusan.py
--rw-r--r--   0        0        0     1724 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/eja.py
--rw-r--r--   0        0        0     3210 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/gogoanime.py
--rw-r--r--   0        0        0     7122 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/kinox.py
--rw-r--r--   0        0        0     3736 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/kisscartoon.py
--rw-r--r--   0        0        0     2509 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/openloadmov.py
--rw-r--r--   0        0        0     2563 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/redundant_kimcartoon.py
--rw-r--r--   0        0        0     4662 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/remotestream.py
--rw-r--r--   0        0        0     4422 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/scdn.py
--rw-r--r--   0        0        0     4121 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/sflix.py
--rw-r--r--   0        0        0     1622 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/solar.py
--rw-r--r--   0        0        0     2132 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/streamblasters.py
--rw-r--r--   0        0        0     1358 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/tamilyogi.py
--rw-r--r--   0        0        0     2895 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/turkish123.py
--rw-r--r--   0        0        0     4516 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/viewasian.py
--rw-r--r--   0        0        0     3395 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/watchasian.py
--rw-r--r--   0        0        0     3983 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/wlext.py
--rw-r--r--   0        0        0     3503 2023-06-08 17:52:38.728717 mov_cli-1.4.2/mov_cli/websites/yoturkish.py
--rw-r--r--   0        0        0      743 2023-06-08 17:52:38.728717 mov_cli-1.4.2/pyproject.toml
--rw-r--r--   0        0        0     8150 1970-01-01 00:00:00.000000 mov_cli-1.4.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-06-19 12:44:14.044129 mov_cli-1.4.3/LICENSE
+-rw-r--r--   0        0        0     7144 2023-06-19 12:44:14.044129 mov_cli-1.4.3/README.md
+-rw-r--r--   0        0        0      235 2023-06-19 12:44:14.044129 mov_cli-1.4.3/mov_cli/__init__.py
+-rw-r--r--   0        0        0     2617 2023-06-19 12:44:14.044129 mov_cli-1.4.3/mov_cli/__main__.py
+-rw-r--r--   0        0        0        1 2023-06-19 12:44:14.044129 mov_cli-1.4.3/mov_cli/extractors/__init__.py
+-rw-r--r--   0        0        0      823 2023-06-19 12:44:14.044129 mov_cli-1.4.3/mov_cli/extractors/doodstream.py
+-rw-r--r--   0        0        0       71 2023-06-19 12:44:14.044129 mov_cli-1.4.3/mov_cli/extractors/scdn/NOTICE
+-rw-r--r--   0        0        0        1 2023-06-19 12:44:14.044129 mov_cli-1.4.3/mov_cli/extractors/scdn/__init__.py
+-rw-r--r--   0        0        0      169 2023-06-19 12:44:14.044129 mov_cli-1.4.3/mov_cli/extractors/scdn/allsportsdaily.py
+-rw-r--r--   0        0        0      958 2023-06-19 12:44:14.044129 mov_cli-1.4.3/mov_cli/extractors/scdn/cr7sports.py
+-rw-r--r--   0        0        0      256 2023-06-19 12:44:14.044129 mov_cli-1.4.3/mov_cli/extractors/scdn/enjoy4hd.py
+-rw-r--r--   0        0        0      141 2023-06-19 12:44:14.044129 mov_cli-1.4.3/mov_cli/extractors/scdn/fabtech.py
+-rw-r--r--   0        0        0      218 2023-06-19 12:44:14.044129 mov_cli-1.4.3/mov_cli/extractors/scdn/gameshdlive.py
+-rw-r--r--   0        0        0      457 2023-06-19 12:44:14.044129 mov_cli-1.4.3/mov_cli/extractors/scdn/livestreames.py
+-rw-r--r--   0        0        0      318 2023-06-19 12:44:14.044129 mov_cli-1.4.3/mov_cli/extractors/scdn/methstreams.py
+-rw-r--r--   0        0        0      156 2023-06-19 12:44:14.044129 mov_cli-1.4.3/mov_cli/extractors/scdn/motornews.py
+-rw-r--r--   0        0        0      873 2023-06-19 12:44:14.044129 mov_cli-1.4.3/mov_cli/extractors/scdn/onestream.py
+-rw-r--r--   0        0        0      891 2023-06-19 12:44:14.044129 mov_cli-1.4.3/mov_cli/extractors/scdn/onionlive.py
+-rw-r--r--   0        0        0      615 2023-06-19 12:44:14.044129 mov_cli-1.4.3/mov_cli/extractors/scdn/onionstream.py
+-rw-r--r--   0        0        0      457 2023-06-19 12:44:14.044129 mov_cli-1.4.3/mov_cli/extractors/scdn/poscitech.py
+-rw-r--r--   0        0        0      638 2023-06-19 12:44:14.044129 mov_cli-1.4.3/mov_cli/extractors/scdn/rainostreams.py
+-rw-r--r--   0        0        0      358 2023-06-19 12:44:14.044129 mov_cli-1.4.3/mov_cli/extractors/scdn/ripple.py
+-rw-r--r--   0        0        0      406 2023-06-19 12:44:14.044129 mov_cli-1.4.3/mov_cli/extractors/scdn/techclips.py
+-rw-r--r--   0        0        0      417 2023-06-19 12:44:14.044129 mov_cli-1.4.3/mov_cli/extractors/scdn/techstips.py
+-rw-r--r--   0        0        0     1333 2023-06-19 12:44:14.044129 mov_cli-1.4.3/mov_cli/extractors/scdn/weakstream.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:44:14.044129 mov_cli-1.4.3/mov_cli/players/__init__.py
+-rw-r--r--   0        0        0     2559 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/players/player.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/utils/__init__.py
+-rw-r--r--   0        0        0     1484 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/utils/dbs.py
+-rw-r--r--   0        0        0     2731 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/utils/httpclient.py
+-rw-r--r--   0        0        0     6133 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/utils/jsunpack.py
+-rw-r--r--   0        0        0     2269 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/utils/lang.py
+-rw-r--r--   0        0        0     1584 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/utils/player.py
+-rw-r--r--   0        0        0      958 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/utils/provider.py
+-rw-r--r--   0        0        0     8708 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/utils/scraper.py
+-rw-r--r--   0        0        0        0 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/websites/__init__.py
+-rw-r--r--   0        0        0    10970 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/websites/actvid.py
+-rw-r--r--   0        0        0     4177 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/websites/animefox.py
+-rw-r--r--   0        0        0     4208 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/websites/dopebox.py
+-rw-r--r--   0        0        0     1943 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/websites/einthusan.py
+-rw-r--r--   0        0        0     1724 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/websites/eja.py
+-rw-r--r--   0        0        0     3210 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/websites/gogoanime.py
+-rw-r--r--   0        0        0     3736 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/websites/kisscartoon.py
+-rw-r--r--   0        0        0     2509 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/websites/openloadmov.py
+-rw-r--r--   0        0        0     2563 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/websites/redundant_kimcartoon.py
+-rw-r--r--   0        0        0     4662 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/websites/remotestream.py
+-rw-r--r--   0        0        0     4422 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/websites/scdn.py
+-rw-r--r--   0        0        0     4217 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/websites/sflix.py
+-rw-r--r--   0        0        0     1644 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/websites/solar.py
+-rw-r--r--   0        0        0     2132 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/websites/streamblasters.py
+-rw-r--r--   0        0        0     1358 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/websites/tamilyogi.py
+-rw-r--r--   0        0        0     2895 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/websites/turkish123.py
+-rw-r--r--   0        0        0     4516 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/websites/viewasian.py
+-rw-r--r--   0        0        0     3395 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/websites/watchasian.py
+-rw-r--r--   0        0        0     3983 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/websites/wlext.py
+-rw-r--r--   0        0        0     3503 2023-06-19 12:44:14.048129 mov_cli-1.4.3/mov_cli/websites/yoturkish.py
+-rw-r--r--   0        0        0      731 2023-06-19 12:44:14.048129 mov_cli-1.4.3/pyproject.toml
+-rw-r--r--   0        0        0     8127 1970-01-01 00:00:00.000000 mov_cli-1.4.3/PKG-INFO
```

### Comparing `mov_cli-1.4.2/LICENSE` & `mov_cli-1.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/README.md` & `mov_cli-1.4.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -191,17 +191,17 @@
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- CONTACT -->
 ## Contact
 
-Author: Poseidon444 | ```Discord: P A I N 4 4 4#4736```
+Author: Poseidon444 | ```Discord: pain444```
 
-Maintainer: HLOAnanas | ```Discord: Ananas#2000```
+Maintainer: HLOAnanas | ```Discord: r3tr0ananas```
 
 Project Link: [https://github.com/mov-cli/mov-cli](https://github.com/mov-cli/mov-cli)
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- Inspiration -->
 ## Inspiration
```

#### html2text {}

```diff
@@ -56,17 +56,17 @@
 changes, please open an issue first to discuss what you would like to change.
 Contributors: [https://contrib.rocks/image?repo=mov-cli/mov-cli]
                                                                   (back_to_top)
  ## Add a Language Please go to [mov-cli/translations](https://github.com/mov-
 cli/translations) there are instructions on how to add a Language.  ## License
 Distributed under the GPL-3.0 License. See `LICENSE` for more information.
                                                                   (back_to_top)
- ## Contact Author: Poseidon444 | ```Discord: P A I N 4 4 4#4736``` Maintainer:
-HLOAnanas | ```Discord: Ananas#2000``` Project Link: [https://github.com/mov-
-cli/mov-cli](https://github.com/mov-cli/mov-cli)
+ ## Contact Author: Poseidon444 | ```Discord: pain444``` Maintainer: HLOAnanas
+| ```Discord: r3tr0ananas``` Project Link: [https://github.com/mov-cli/mov-cli]
+(https://github.com/mov-cli/mov-cli)
                                                                   (back_to_top)
  ## Inspiration Heavily inspired from [ani-cli](https://github.com/pystardust/
 ani-cli)
                                                                   (back_to_top)
   [contributors-shield]: https://img.shields.io/github/contributors/mov-cli/
 mov-cli.svg?style=for-the-badge [contributors-url]: https://github.com/mov-cli/
 mov-cli/graphs/contributors [forks-shield]: https://img.shields.io/github/
```

### Comparing `mov_cli-1.4.2/mov_cli/__main__.py` & `mov_cli-1.4.3/mov_cli/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from .websites.sflix import sflix
 from .websites.solar import solar
 from .websites.viewasian import viewasian
 from .websites.gogoanime import gogoanime
 from .websites.watchasian import watchasian
 from .websites.wlext import wlext
 from .websites.streamblasters import streamblasters
-from .websites.kinox import kinox
 from .websites.tamilyogi import tamilyogi
 from .websites.einthusan import einthusan
 from .websites.turkish123 import turkish123
 from .websites.animefox import animefox
 from .websites.scdn import scdn
 from .websites.openloadmov import openloadmov
 from .websites.remotestream import remotestream
@@ -34,15 +33,14 @@
     "solar": [solar, "https://solarmovie.pe"],
     "dopebox": [dopebox, "https://dopebox.to"],
     "viewasian": [viewasian, "https://viewasian.co"],
     "gogoanime": [gogoanime, "https://gogoanime.cl"],
     "watchasian": [watchasian, "https://www1.watchasian.id"],
     "wlext": [wlext, "https://wlext.is"],
     "streamblasters": [streamblasters, "https://streamblasters.pro"],
-    "kinox": [kinox, "https://ww17.kinox.to"],
     "tamilyogi": [tamilyogi, "https://tamilyogi.cash"],
     "einthusan": [einthusan, "https://einthusan.tv"],
     "turkish123": [turkish123, "https://turkish123.ac"],
     "animefox": [animefox, "https://animefox.to"],
     "scdn": [scdn, ""],
     "openloadmov": [openloadmov, "https://openloadmov.com"],
     "remotestream": [remotestream, "https://remotestre.am"],
```

### Comparing `mov_cli-1.4.2/mov_cli/extractors/doodstream.py` & `mov_cli-1.4.3/mov_cli/extractors/doodstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/extractors/scdn/cr7sports.py` & `mov_cli-1.4.3/mov_cli/extractors/scdn/cr7sports.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/extractors/scdn/onestream.py` & `mov_cli-1.4.3/mov_cli/extractors/scdn/onestream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/extractors/scdn/onionlive.py` & `mov_cli-1.4.3/mov_cli/extractors/scdn/onionlive.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/extractors/scdn/onionstream.py` & `mov_cli-1.4.3/mov_cli/extractors/scdn/onionstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/extractors/scdn/rainostreams.py` & `mov_cli-1.4.3/mov_cli/extractors/scdn/rainostreams.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/extractors/scdn/weakstream.py` & `mov_cli-1.4.3/mov_cli/extractors/scdn/weakstream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/players/player.py` & `mov_cli-1.4.3/mov_cli/players/player.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/utils/dbs.py` & `mov_cli-1.4.3/mov_cli/utils/dbs.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import re
 
 import httpx
 from bs4 import BeautifulSoup as BS
 
+
 def get_imdb_id(query: str) -> str:
     query = query.replace(" ", "_")
     req = httpx.get(
         f"https://v2.sg.media-imdb.com/suggestion/{query[0].lower()}/{query}.json"
     ).json()["d"]
     print(req)
     return req[0]["id"]
```

### Comparing `mov_cli-1.4.2/mov_cli/utils/httpclient.py` & `mov_cli-1.4.3/mov_cli/utils/httpclient.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/utils/jsunpack.py` & `mov_cli-1.4.3/mov_cli/utils/jsunpack.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/utils/lang.py` & `mov_cli-1.4.3/mov_cli/utils/lang.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/utils/player.py` & `mov_cli-1.4.3/mov_cli/utils/player.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 class Player:
     """A base class for players in mov-cli."""
 
     def __init__(self, display_name: str) -> None:
         self.__display_name = display_name
 
         self.__os = platform.system()
-        
+
         self.__platform = platform.platform()
 
     @property
     def display_name(self) -> str:
         """Returns display name of player."""
         return self.__display_name
```

### Comparing `mov_cli-1.4.2/mov_cli/utils/provider.py` & `mov_cli-1.4.3/mov_cli/utils/provider.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from fzf import fzf_prompt
 
 english = ["actvid", "sflix", "solar", "dopebox", "openloadmov", "remotestream"]
 
-german = ["kinox"]
+# german = ["kinox"] kinox was removed, as it didn't function really.
 
 indian = [
     "streamblasters",
     "tamilyogi",
     "einthusan",
 ]
 
@@ -29,15 +29,14 @@
 
 inter = [
     "wlext",
 ]
 
 preselction = {
     "English Providers": [english],
-    "German Providers": [german],
     "Indian Providers": [indian],
     "Asian Providers": [asian],
     "LIVE TV Providers": [tv],
     "Cartoons Providers": [cartoons],
     "Turkish Providers": [turkish],
     "Anime Providers": [anime],
     "Sports Providers": [sports],
```

### Comparing `mov_cli-1.4.2/mov_cli/utils/scraper.py` & `mov_cli-1.4.3/mov_cli/utils/scraper.py`

 * *Files 1% similar despite different names*

```diff
@@ -50,18 +50,19 @@
         ) = (0, 1, 2, 3, 4, 5, 6, 7, 8, 9)
         self.scraper = self.parser()
         pass
 
     def parser(self):
         try:
             import lxml
+
             return "lxml"
         except ModuleNotFoundError:
             return "html.parser"
-        
+
     @staticmethod
     def parse(txt: str) -> str:
         return re.sub(r"\W+", "-", txt.lower())
 
     def dl(
         self,
         url: str,
```

### Comparing `mov_cli-1.4.2/mov_cli/websites/actvid.py` & `mov_cli-1.4.3/mov_cli/websites/actvid.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,15 +92,17 @@
             for i in urls
         ]
         ids = [i.split("-")[-1] for i in urls]
         return [list(sublist) for sublist in zip(title, urls, ids, mov_or_tv)]
 
     def ask(self, series_id: str) -> tuple:
         r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
-        season_ids = [i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")]
+        season_ids = [
+            i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")
+        ]
         season = self.askseason(len(season_ids))
         z = f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}"
         rf = self.client.get(z)
         episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".nav-item > a")]
         episode = episodes[int(self.askepisode(len(episodes))) - 1]
         ep = self.getep(
             url=f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}",
@@ -153,20 +155,17 @@
         data = json.loads(predata)
         print(predata)
         return data[0]['file']"""
 
     def cdn_url(self, final_link: str, rabb_id: str) -> str:
         self.client.set_headers({"X-Requested-With": "XMLHttpRequest"})
         data = self.client.get(f"{final_link}getSources?id={rabb_id}").json()
-        source = data["sources"]
-        link = f"{source}"
-        if link.endswith("==") or link.endswith("="):
-            n = json.loads(self.decrypt(data["sources"], self.gh_key()))
-            return n[0]["file"]
-        return source[0]["file"]
+        n = json.loads(self.decrypt(data["sources"], self.gh_key()))
+        return n[0]["file"]
+        
 
     def server_id(self, mov_id: str) -> str:
         req = self.client.get(f"{self.base_url}/ajax/movie/episodes/{mov_id}")
         soup = BS(req, self.scraper)
         return [i["data-linkid"] for i in soup.select(".nav-item > a")][0]
 
     def ep_server_id(self, ep_id: str) -> str:
@@ -226,34 +225,40 @@
         dec_key = k[:32]
         iv = k[32:]
         p = AES.new(dec_key, AES.MODE_CBC, iv=iv).decrypt(base64.b64decode(data)[16:])
         return self.unpad(p).decode()
 
     def ds(self, series_id: str, name):
         r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
-        season_ids = [i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")]
+        season_ids = [
+            i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")
+        ]
         season = self.askseason(len(season_ids))
         z = f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}"
         rf = self.client.get(z)
         episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".nav-item > a")]
         for e in range(len(episodes)):
             episode = episodes[e]
             sid = self.ep_server_id(episode)
             iframe_url, tv_id = self.get_link(sid)
             iframe_link, iframe_id = self.rabbit_id(iframe_url)
             url = self.cdn_url(iframe_link, iframe_id)
             self.dl(url, name, season=season, episode=e + 1)
 
     def sd(self, series_id: str, name):
         r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
-        season_ids = [i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")]
+        season_ids = [
+            i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")
+        ]
         for s in range(len(season_ids)):
             z = f"{self.base_url}/ajax/v2/season/episodes/{season_ids[s]}"
             rf = self.client.get(z)
-            episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".nav-item > a")]
+            episodes = [
+                i["data-id"] for i in BS(rf, self.scraper).select(".nav-item > a")
+            ]
             for e in range(len(episodes)):
                 episode = episodes[e]
                 sid = self.ep_server_id(episode)
                 iframe_url, tv_id = self.get_link(sid)
                 iframe_link, iframe_id = self.rabbit_id(iframe_url)
                 url = self.cdn_url(iframe_link, iframe_id)
                 self.dl(url, name, season=s + 1, episode=e + 1)
```

### Comparing `mov_cli-1.4.2/mov_cli/websites/animefox.py` & `mov_cli-1.4.3/mov_cli/websites/animefox.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/websites/dopebox.py` & `mov_cli-1.4.3/mov_cli/websites/dopebox.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,17 @@
                 f"https://rabbitstream.net/ajax/embed-4/getSources?id={rabbid}&_token={rose}&_number={num}"
             ).text
         )["sources"][0]["file"]
         return data"""
 
     def ask(self, series_id):
         r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
-        season_ids = [i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")]
+        season_ids = [
+            i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")
+        ]
         season = self.askseason(len(season_ids))
         rf = self.client.get(
             f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}"
         )
         episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".episode-item")]
         episode = episodes[int(self.askepisode(len(episodes))) - 1]
         ep = self.getep(
@@ -61,15 +63,17 @@
             f"{self.base_url}/ajax/v2/episode/servers/{ep_id}/#servers-list"
         )
         soup = BS(rem, self.scraper)
         return [i["data-id"] for i in soup.select(".link-item")][0]
 
     def ds(self, series_id: str, name):
         r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
-        season_ids = [i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")]
+        season_ids = [
+            i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")
+        ]
         season = self.askseason(len(season_ids))
         rf = self.client.get(
             f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}"
         )
         episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".episode-item")]
         for e in range(len(episodes)):
             episode = episodes[e]
@@ -77,20 +81,24 @@
             iframe_url, tv_id = self.get_link(sid)
             iframe_link, iframe_id = self.rabbit_id(iframe_url)
             url = self.cdn_url(iframe_link, iframe_id)
             self.dl(url, name, season=season, episode=e + 1)
 
     def sd(self, series_id: str, name):
         r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
-        season_ids = [i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")]
+        season_ids = [
+            i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")
+        ]
         for s in range(len(season_ids)):
             rf = self.client.get(
                 f"{self.base_url}/ajax/v2/season/episodes/{season_ids[s]}"
             )
-            episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".episode-item")]
+            episodes = [
+                i["data-id"] for i in BS(rf, self.scraper).select(".episode-item")
+            ]
             for e in range(len(episodes)):
                 episode = episodes[e]
                 sid = self.ep_server_id(episode)
                 iframe_url, tv_id = self.get_link(sid)
                 iframe_link, iframe_id = self.rabbit_id(iframe_url)
                 url = self.cdn_url(iframe_link, iframe_id)
                 self.dl(url, name, season=s + 1, episode=e + 1)
```

### Comparing `mov_cli-1.4.2/mov_cli/websites/einthusan.py` & `mov_cli-1.4.3/mov_cli/websites/einthusan.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/websites/eja.py` & `mov_cli-1.4.3/mov_cli/websites/eja.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/websites/gogoanime.py` & `mov_cli-1.4.3/mov_cli/websites/gogoanime.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/websites/kisscartoon.py` & `mov_cli-1.4.3/mov_cli/websites/kisscartoon.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/websites/openloadmov.py` & `mov_cli-1.4.3/mov_cli/websites/openloadmov.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/websites/redundant_kimcartoon.py` & `mov_cli-1.4.3/mov_cli/websites/redundant_kimcartoon.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/websites/remotestream.py` & `mov_cli-1.4.3/mov_cli/websites/remotestream.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/websites/scdn.py` & `mov_cli-1.4.3/mov_cli/websites/scdn.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/websites/sflix.py` & `mov_cli-1.4.3/mov_cli/websites/sflix.py`

 * *Files 6% similar despite different names*

```diff
@@ -19,15 +19,17 @@
                 f"https://rabbitstream.net/ajax/embed-4/getSources?id={rabbid}&_token={rose}&_number={num}"
             ).text
         )["sources"][0]["file"]
         return data"""
 
     def ask(self, series_id):
         r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
-        season_ids = [i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")]
+        season_ids = [
+            i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")
+        ]
         season = self.askseason(len(season_ids))
         rf = self.client.get(
             f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}"
         )
         episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".episode-item")]
         episode = episodes[int(self.askepisode(len(episodes))) - 1]
         ep = self.getep(
@@ -60,15 +62,17 @@
             f"{self.base_url}/ajax/v2/episode/servers/{ep_id}/#servers-list"
         )
         soup = BS(rem, self.scraper)
         return [i["data-id"] for i in soup.select(".link-item")][0]
 
     def ds(self, series_id: str, name):
         r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
-        season_ids = [i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")]
+        season_ids = [
+            i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")
+        ]
         season = self.askseason(len(season_ids))
         rf = self.client.get(
             f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}"
         )
         episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".episode-item")]
         for e in range(len(episodes)):
             episode = episodes[e]
@@ -76,20 +80,24 @@
             iframe_url, tv_id = self.get_link(sid)
             iframe_link, iframe_id = self.rabbit_id(iframe_url)
             url = self.cdn_url(iframe_link, iframe_id)
             self.dl(url, name, season=season, episode=e + 1)
 
     def sd(self, series_id: str, name):
         r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
-        season_ids = [i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")]
+        season_ids = [
+            i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")
+        ]
         for s in range(len(season_ids)):
             rf = self.client.get(
                 f"{self.base_url}/ajax/v2/season/episodes/{season_ids[s]}"
             )
-            episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".episode-item")]
+            episodes = [
+                i["data-id"] for i in BS(rf, self.scraper).select(".episode-item")
+            ]
             for e in range(len(episodes)):
                 episode = episodes[e]
                 sid = self.ep_server_id(episode)
                 iframe_url, tv_id = self.get_link(sid)
                 iframe_link, iframe_id = self.rabbit_id(iframe_url)
                 url = self.cdn_url(iframe_link, iframe_id)
                 self.dl(url, name, season=s + 1, episode=e + 1)
```

### Comparing `mov_cli-1.4.2/mov_cli/websites/solar.py` & `mov_cli-1.4.3/mov_cli/websites/solar.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,17 @@
         super().__init__(base_url)
         self.base_url = base_url
         self.rep_key = "6LeWLCYeAAAAAL1caYzkrIY-M59Vu41vIblXQZ48"
         self.redo()
 
     def ask(self, series_id):
         r = self.client.get(f"{self.base_url}/ajax/v2/tv/seasons/{series_id}")
-        season_ids = [i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")]
+        season_ids = [
+            i["data-id"] for i in BS(r, self.scraper).select(".dropdown-item")
+        ]
         season = self.askseason(len(season_ids))
         rf = self.client.get(
             f"{self.base_url}/ajax/v2/season/episodes/{season_ids[int(season) - 1]}"
         )
         episodes = [i["data-id"] for i in BS(rf, self.scraper).select(".eps-item")]
         episode = episodes[int(self.askepisode(len(episodes))) - 1]
         ep = self.getep(
```

### Comparing `mov_cli-1.4.2/mov_cli/websites/streamblasters.py` & `mov_cli-1.4.3/mov_cli/websites/streamblasters.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/websites/tamilyogi.py` & `mov_cli-1.4.3/mov_cli/websites/tamilyogi.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/websites/turkish123.py` & `mov_cli-1.4.3/mov_cli/websites/turkish123.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/websites/viewasian.py` & `mov_cli-1.4.3/mov_cli/websites/viewasian.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/websites/watchasian.py` & `mov_cli-1.4.3/mov_cli/websites/watchasian.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/websites/wlext.py` & `mov_cli-1.4.3/mov_cli/websites/wlext.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/mov_cli/websites/yoturkish.py` & `mov_cli-1.4.3/mov_cli/websites/yoturkish.py`

 * *Files identical despite different names*

### Comparing `mov_cli-1.4.2/pyproject.toml` & `mov_cli-1.4.3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.poetry]
 name = "mov-cli"
-version = "1.4.2"
+version = "1.4.3"
 description = "A cli tool to browse and watch Movies/Shows/TV/Sports."
 authors = ["Pain <painedposeidon444@gmail.com>"]
-maintainers = ["Ananas <ananas@historylifeonline.xyz>"]
+maintainers = ["Ananas <ananas@ad1hl.xyz>"]
 license = "GPLv3"
 readme = "README.md"
 packages = [{include = "mov_cli"}]
 repository = "https://github.com/mov-cli/mov-cli"
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `mov_cli-1.4.2/PKG-INFO` & `mov_cli-1.4.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: mov-cli
-Version: 1.4.2
+Version: 1.4.3
 Summary: A cli tool to browse and watch Movies/Shows/TV/Sports.
 Home-page: https://github.com/mov-cli/mov-cli
 License: GPLv3
 Author: Pain
 Author-email: painedposeidon444@gmail.com
 Maintainer: Ananas
-Maintainer-email: ananas@historylifeonline.xyz
+Maintainer-email: ananas@ad1hl.xyz
 Requires-Python: >=3.9,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
@@ -217,17 +217,17 @@
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 
 <!-- CONTACT -->
 ## Contact
 
-Author: Poseidon444 | ```Discord: P A I N 4 4 4#4736```
+Author: Poseidon444 | ```Discord: pain444```
 
-Maintainer: HLOAnanas | ```Discord: Ananas#2000```
+Maintainer: HLOAnanas | ```Discord: r3tr0ananas```
 
 Project Link: [https://github.com/mov-cli/mov-cli](https://github.com/mov-cli/mov-cli)
 
 <p align="right">(<a href="#readme-top">back to top</a>)</p>
 
 <!-- Inspiration -->
 ## Inspiration
```

#### html2text {}

```diff
@@ -1,12 +1,12 @@
-Metadata-Version: 2.1 Name: mov-cli Version: 1.4.2 Summary: A cli tool to
+Metadata-Version: 2.1 Name: mov-cli Version: 1.4.3 Summary: A cli tool to
 browse and watch Movies/Shows/TV/Sports. Home-page: https://github.com/mov-cli/
 mov-cli License: GPLv3 Author: Pain Author-email: painedposeidon444@gmail.com
-Maintainer: Ananas Maintainer-email: ananas@historylifeonline.xyz Requires-
-Python: >=3.9,<4.0 Classifier: License :: Other/Proprietary License Classifier:
+Maintainer: Ananas Maintainer-email: ananas@ad1hl.xyz Requires-Python:
+>=3.9,<4.0 Classifier: License :: Other/Proprietary License Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.9 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.11 Requires-Dist: beautifulsoup4
 (>=4.11.2,<5.0.0) Requires-Dist: httpx (>=0.24.0,<0.25.0) Requires-Dist: krfzf-
 py (>=0.0.4,<0.0.5) Requires-Dist: pycryptodome (>=3.17,<4.0) Requires-Dist:
 six (>=1.16.0,<2.0.0) Requires-Dist: tldextract (>=3.4.3,<4.0.0) Project-URL:
 Bug Tracker, https://github.com/mov-cli/mov-cli/issues Project-URL: Repository,
@@ -69,17 +69,17 @@
 changes, please open an issue first to discuss what you would like to change.
 Contributors: [https://contrib.rocks/image?repo=mov-cli/mov-cli]
                                                                   (back_to_top)
  ## Add a Language Please go to [mov-cli/translations](https://github.com/mov-
 cli/translations) there are instructions on how to add a Language.  ## License
 Distributed under the GPL-3.0 License. See `LICENSE` for more information.
                                                                   (back_to_top)
- ## Contact Author: Poseidon444 | ```Discord: P A I N 4 4 4#4736``` Maintainer:
-HLOAnanas | ```Discord: Ananas#2000``` Project Link: [https://github.com/mov-
-cli/mov-cli](https://github.com/mov-cli/mov-cli)
+ ## Contact Author: Poseidon444 | ```Discord: pain444``` Maintainer: HLOAnanas
+| ```Discord: r3tr0ananas``` Project Link: [https://github.com/mov-cli/mov-cli]
+(https://github.com/mov-cli/mov-cli)
                                                                   (back_to_top)
  ## Inspiration Heavily inspired from [ani-cli](https://github.com/pystardust/
 ani-cli)
                                                                   (back_to_top)
   [contributors-shield]: https://img.shields.io/github/contributors/mov-cli/
 mov-cli.svg?style=for-the-badge [contributors-url]: https://github.com/mov-cli/
 mov-cli/graphs/contributors [forks-shield]: https://img.shields.io/github/
```

