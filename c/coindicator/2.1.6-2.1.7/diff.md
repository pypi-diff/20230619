# Comparing `tmp/coindicator-2.1.6.tar.gz` & `tmp/coindicator-2.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coindicator-2.1.6.tar", last modified: Mon Jun 19 08:56:00 2023, max compression
+gzip compressed data, was "coindicator-2.1.7.tar", last modified: Mon Jun 19 09:26:18 2023, max compression
```

## Comparing `coindicator-2.1.6.tar` & `coindicator-2.1.7.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 08:56:00.618748 coindicator-2.1.6/
--rw-rw-r--   0 sander    (1000) sander    (1000)       83 2023-06-16 13:19:52.000000 coindicator-2.1.6/.gitignore
--rw-rw-r--   0 sander    (1000) sander    (1000)      899 2022-10-30 19:56:43.000000 coindicator-2.1.6/.pre-commit-config.yaml
--rw-r--r--   0 sander    (1000) sander    (1000)     1106 2020-04-16 00:57:46.000000 coindicator-2.1.6/LICENSE
--rw-rw-r--   0 sander    (1000) sander    (1000)       29 2023-06-16 13:19:52.000000 coindicator-2.1.6/MANIFEST.in
--rw-rw-r--   0 sander    (1000) sander    (1000)     4823 2023-06-19 08:56:00.618748 coindicator-2.1.6/PKG-INFO
--rw-rw-r--   0 sander    (1000) sander    (1000)     4312 2023-06-16 13:19:52.000000 coindicator-2.1.6/README.md
--rw-rw-r--   0 sander    (1000) sander    (1000)      369 2023-06-16 13:19:52.000000 coindicator-2.1.6/coindicator.desktop
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 08:56:00.606748 coindicator-2.1.6/img/
--rw-rw-r--   0 sander    (1000) sander    (1000)    27147 2022-10-30 19:56:43.000000 coindicator-2.1.6/img/gitcoin.png
--rw-rw-r--   0 sander    (1000) sander    (1000)   172307 2022-10-30 19:56:43.000000 coindicator-2.1.6/img/screenshot.png
--rwxrwxr-x   0 sander    (1000) sander    (1000)     1576 2023-06-16 15:26:25.000000 coindicator-2.1.6/install.sh
--rw-rw-r--   0 sander    (1000) sander    (1000)      294 2023-06-16 13:19:52.000000 coindicator-2.1.6/pyproject.toml
--rw-rw-r--   0 sander    (1000) sander    (1000)      794 2023-06-16 13:19:52.000000 coindicator-2.1.6/requirements.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)     1202 2023-06-19 08:56:00.622748 coindicator-2.1.6/setup.cfg
--rw-rw-r--   0 sander    (1000) sander    (1000)      521 2023-06-16 13:19:52.000000 coindicator-2.1.6/setup.py
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 08:56:00.602748 coindicator-2.1.6/src/
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 08:56:00.610748 coindicator-2.1.6/src/coin/
--rw-rw-r--   0 sander    (1000) sander    (1000)        0 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/__init__.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1537 2023-06-16 13:19:52.000000 coindicator-2.1.6/src/coin/about.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     6537 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/alarm.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     5794 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/asset_selection.py
--rwxrwxr-x   0 sander    (1000) sander    (1000)    12615 2023-06-19 08:32:25.000000 coindicator-2.1.6/src/coin/coin.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1751 2023-06-16 13:19:52.000000 coindicator-2.1.6/src/coin/coingecko_client.py
--rw-rw-r--   0 sander    (1000) sander    (1000)      609 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/config.py
--rw-rw-r--   0 sander    (1000) sander    (1000)      977 2023-06-16 13:19:52.000000 coindicator-2.1.6/src/coin/config.yaml
--rw-rw-r--   0 sander    (1000) sander    (1000)     1422 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/downloader.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1177 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/error.py
--rw-rw-r--   0 sander    (1000) sander    (1000)    10482 2023-06-19 08:54:53.000000 coindicator-2.1.6/src/coin/exchange.py
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 08:56:00.614748 coindicator-2.1.6/src/coin/exchanges/
--rw-rw-r--   0 sander    (1000) sander    (1000)     1771 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/exchanges/binance.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1579 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/exchanges/bitfinex.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1834 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/exchanges/bitkub.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1493 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/exchanges/bitstamp.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     2031 2023-06-16 13:19:52.000000 coindicator-2.1.6/src/coin/exchanges/bittrex.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1473 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/exchanges/cexio.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1499 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/exchanges/gemini.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1718 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/exchanges/hitbtc.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     2083 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/exchanges/kraken.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1273 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/exchanges/okcoin.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1547 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/exchanges/poloniex.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1281 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/exchanges/unocoin.py
--rw-rw-r--   0 sander    (1000) sander    (1000)    10370 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/indicator.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     2608 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/plugin_selection.py
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 08:56:00.618748 coindicator-2.1.6/src/coin/resources/
--rw-rw-r--   0 sander    (1000) sander    (1000)   294232 2023-06-16 13:19:52.000000 coindicator-2.1.6/src/coin/resources/ca-ching.wav
--rw-rw-r--   0 sander    (1000) sander    (1000)     5060 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/resources/icon.png
--rw-rw-r--   0 sander    (1000) sander    (1000)      983 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/resources/icon_32px.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     1440 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/resources/icon_48px.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     1673 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/resources/icon_64px.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     1889 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/resources/loading.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     4619 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/resources/logo_124px.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     7329 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/resources/logo_124pxs.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     6508 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/resources/logo_248px.png
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 08:56:00.618748 coindicator-2.1.6/src/coindicator.egg-info/
--rw-rw-r--   0 sander    (1000) sander    (1000)     4823 2023-06-19 08:56:00.000000 coindicator-2.1.6/src/coindicator.egg-info/PKG-INFO
--rw-rw-r--   0 sander    (1000) sander    (1000)     1388 2023-06-19 08:56:00.000000 coindicator-2.1.6/src/coindicator.egg-info/SOURCES.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-19 08:56:00.000000 coindicator-2.1.6/src/coindicator.egg-info/dependency_links.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)       47 2023-06-19 08:56:00.000000 coindicator-2.1.6/src/coindicator.egg-info/entry_points.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-16 11:50:35.000000 coindicator-2.1.6/src/coindicator.egg-info/not-zip-safe
--rw-rw-r--   0 sander    (1000) sander    (1000)      227 2023-06-19 08:56:00.000000 coindicator-2.1.6/src/coindicator.egg-info/requires.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)        5 2023-06-19 08:56:00.000000 coindicator-2.1.6/src/coindicator.egg-info/top_level.txt
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 09:26:18.639954 coindicator-2.1.7/
+-rw-rw-r--   0 sander    (1000) sander    (1000)       83 2023-06-16 13:19:52.000000 coindicator-2.1.7/.gitignore
+-rw-rw-r--   0 sander    (1000) sander    (1000)      899 2022-10-30 19:56:43.000000 coindicator-2.1.7/.pre-commit-config.yaml
+-rw-r--r--   0 sander    (1000) sander    (1000)     1106 2020-04-16 00:57:46.000000 coindicator-2.1.7/LICENSE
+-rw-rw-r--   0 sander    (1000) sander    (1000)       29 2023-06-16 13:19:52.000000 coindicator-2.1.7/MANIFEST.in
+-rw-rw-r--   0 sander    (1000) sander    (1000)     4402 2023-06-19 09:26:18.639954 coindicator-2.1.7/PKG-INFO
+-rw-rw-r--   0 sander    (1000) sander    (1000)     3891 2023-06-19 09:10:17.000000 coindicator-2.1.7/README.md
+-rw-rw-r--   0 sander    (1000) sander    (1000)      369 2023-06-16 13:19:52.000000 coindicator-2.1.7/coindicator.desktop
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 09:26:18.619957 coindicator-2.1.7/img/
+-rw-rw-r--   0 sander    (1000) sander    (1000)    27147 2022-10-30 19:56:43.000000 coindicator-2.1.7/img/gitcoin.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)   172307 2022-10-30 19:56:43.000000 coindicator-2.1.7/img/screenshot.png
+-rwxrwxr-x   0 sander    (1000) sander    (1000)     1576 2023-06-16 15:26:25.000000 coindicator-2.1.7/install.sh
+-rw-rw-r--   0 sander    (1000) sander    (1000)      294 2023-06-16 13:19:52.000000 coindicator-2.1.7/pyproject.toml
+-rw-rw-r--   0 sander    (1000) sander    (1000)      794 2023-06-16 13:19:52.000000 coindicator-2.1.7/requirements.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1202 2023-06-19 09:26:18.639954 coindicator-2.1.7/setup.cfg
+-rw-rw-r--   0 sander    (1000) sander    (1000)      521 2023-06-16 13:19:52.000000 coindicator-2.1.7/setup.py
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 09:26:18.615957 coindicator-2.1.7/src/
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 09:26:18.627956 coindicator-2.1.7/src/coin/
+-rw-rw-r--   0 sander    (1000) sander    (1000)        0 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/__init__.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1537 2023-06-16 13:19:52.000000 coindicator-2.1.7/src/coin/about.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     6537 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/alarm.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     5794 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/asset_selection.py
+-rwxrwxr-x   0 sander    (1000) sander    (1000)    12615 2023-06-19 08:32:25.000000 coindicator-2.1.7/src/coin/coin.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1751 2023-06-16 13:19:52.000000 coindicator-2.1.7/src/coin/coingecko_client.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)      609 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/config.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)      977 2023-06-16 13:19:52.000000 coindicator-2.1.7/src/coin/config.yaml
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1422 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/downloader.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1177 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/error.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)    10369 2023-06-19 09:22:15.000000 coindicator-2.1.7/src/coin/exchange.py
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 09:26:18.631955 coindicator-2.1.7/src/coin/exchanges/
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1746 2023-06-19 09:24:08.000000 coindicator-2.1.7/src/coin/exchanges/binance.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1554 2023-06-19 09:24:13.000000 coindicator-2.1.7/src/coin/exchanges/bitfinex.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1809 2023-06-19 09:24:16.000000 coindicator-2.1.7/src/coin/exchanges/bitkub.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1468 2023-06-19 09:24:20.000000 coindicator-2.1.7/src/coin/exchanges/bitstamp.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2016 2023-06-19 09:22:47.000000 coindicator-2.1.7/src/coin/exchanges/bittrex.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1458 2023-06-19 09:22:55.000000 coindicator-2.1.7/src/coin/exchanges/cexio.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1474 2023-06-19 09:24:26.000000 coindicator-2.1.7/src/coin/exchanges/gemini.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1693 2023-06-19 09:24:00.000000 coindicator-2.1.7/src/coin/exchanges/hitbtc.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2058 2023-06-19 09:23:56.000000 coindicator-2.1.7/src/coin/exchanges/kraken.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1252 2023-06-19 09:25:24.000000 coindicator-2.1.7/src/coin/exchanges/okcoin.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1532 2023-06-19 09:23:19.000000 coindicator-2.1.7/src/coin/exchanges/poloniex.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1256 2023-06-19 09:24:44.000000 coindicator-2.1.7/src/coin/exchanges/unocoin.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)    10370 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/indicator.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2608 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/plugin_selection.py
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 09:26:18.635955 coindicator-2.1.7/src/coin/resources/
+-rw-rw-r--   0 sander    (1000) sander    (1000)   294232 2023-06-16 13:19:52.000000 coindicator-2.1.7/src/coin/resources/ca-ching.wav
+-rw-rw-r--   0 sander    (1000) sander    (1000)     5060 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/resources/icon.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)      983 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/resources/icon_32px.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1440 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/resources/icon_48px.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1673 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/resources/icon_64px.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1889 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/resources/loading.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     4619 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/resources/logo_124px.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     7329 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/resources/logo_124pxs.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     6508 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/resources/logo_248px.png
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 09:26:18.639954 coindicator-2.1.7/src/coindicator.egg-info/
+-rw-rw-r--   0 sander    (1000) sander    (1000)     4402 2023-06-19 09:26:18.000000 coindicator-2.1.7/src/coindicator.egg-info/PKG-INFO
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1388 2023-06-19 09:26:18.000000 coindicator-2.1.7/src/coindicator.egg-info/SOURCES.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-19 09:26:18.000000 coindicator-2.1.7/src/coindicator.egg-info/dependency_links.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)       47 2023-06-19 09:26:18.000000 coindicator-2.1.7/src/coindicator.egg-info/entry_points.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-16 11:50:35.000000 coindicator-2.1.7/src/coindicator.egg-info/not-zip-safe
+-rw-rw-r--   0 sander    (1000) sander    (1000)      227 2023-06-19 09:26:18.000000 coindicator-2.1.7/src/coindicator.egg-info/requires.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)        5 2023-06-19 09:26:18.000000 coindicator-2.1.7/src/coindicator.egg-info/top_level.txt
```

### Comparing `coindicator-2.1.6/.pre-commit-config.yaml` & `coindicator-2.1.7/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/LICENSE` & `coindicator-2.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/PKG-INFO` & `coindicator-2.1.7/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coindicator
-Version: 2.1.6
+Version: 2.1.7
 Summary: Coinprice Indicator
 Home-page: https://github.com/bluppfisk/coindicator/
 Author: Sander Van de Moortel
 Author-email: sander.vandemoortel@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/bluppfisk/coindicator/
 Platform: Linux
@@ -66,15 +66,15 @@
 ## Running
 
 * A launcher icon "Coindicator" should have been installed that can be used to start the app
 * Alternatively, go to the install folder, activate the environment `source venv/bin/activate` and run the app with `coindicator`. Add ` &` to run it in the background.
 
 ## Configuring
 
-Use the GUI to add and remove indicators (find the piggy icon), to pick assets, to set refresh frequency and to set alarms. Alternatively, edit the **user.conf** YAML file in the project root.
+Use the GUI to add and remove indicators (find the piggy icon), to pick assets, to set refresh frequency and to set alarms. Alternatively, edit the **~/.config/coindicator/user.conf** YAML file.
 
 `max_decimals`: default 8. Lower if you want fewer decimals (takes priority over `significant_digits`)
 `significant_digits`: default 3. Set to higher if you want more significant digits.
 
 ## Extending (Plug-ins)
 
 Adding your own exchange plug-in is easy. Just create class file with methods for returning a ticker URL, a discovery URL, and parsing the responses from the ticker and discovery APIs. Then add the file to the `exchanges` folder.
@@ -95,22 +95,15 @@
 * Ubuntu Linux 17.10 (Artful Aardvark) with GNOME 3 and Unity 7
 * Ubuntu Linux 18.04 (Bionic Beaver) with GNOME 3 and Unity 7
 * Ubuntu Linux 19.04 (Disco Dingo) with GNOME 3 and Unity 7
 * Ubuntu Linux 19.10 (Eoan Ermine) with GNOME 3 and Unity 7
 * Ubuntu Linux 20.04 (Focal Fossa) with GNOME 3
 * Ubuntu Linux 20.10 (Groovy Gorilla) with GNOME 3
 * Ubuntu Linux 21.04 (Hirsute Hippo) with GNOME 3
-* Ubuntu Linux 21.10 (Impish Indri) with GNOME 3
-* Ubuntu Linux 22.04 (Jammy Jellyfish) with GNOME 3
-* Ubuntu Linux 22.10 (Kinetic Kudu) with GNOME 3
+* Ubuntu Linux 21.10 (Impish Indri) with GNOME 40
+* Ubuntu Linux 22.04 (Jammy Jellyfish) with GNOME 42
+* Ubuntu Linux 22.10 (Kinetic Kudu) with GNOME 43
+* Ubuntu Linux 23.04 (Lunar Lobster) with GNOME 44
 
 For other systems, you may need to install LibAppIndicator support.
 
-Before reporting bugs or issues, please try removing **~/.config/coindicator/user.conf** first and then the files in **~/.config/coindicator/cache/**.
-
-## Sponsorship and Funding
-
-![Gitcoin logo](img/gitcoin.png)
-
-This project has been funded in the past by generous maecenas @ghettodev through [Gitcoin](https://gitcoin.co/), a platform that directs the attention of bounty hunters (coders) to open issues and feature requests on Github.
-
-If you would like to sponsor a feature request, bug report or just donate to the project, be sure to check out [Gitcoin](https://gitcoin.co/).
+Before reporting bugs or issues, please try removing/renaming the **~/.config/coindicator** folder first.
```

### Comparing `coindicator-2.1.6/README.md` & `coindicator-2.1.7/src/coindicator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,23 @@
+Metadata-Version: 2.1
+Name: coindicator
+Version: 2.1.7
+Summary: Coinprice Indicator
+Home-page: https://github.com/bluppfisk/coindicator/
+Author: Sander Van de Moortel
+Author-email: sander.vandemoortel@gmail.com
+License: MIT
+Project-URL: Documentation, https://github.com/bluppfisk/coindicator/
+Platform: Linux
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Programming Language :: Python
+Description-Content-Type: text/markdown; charset=UTF-8
+Provides-Extra: develop
+License-File: LICENSE
+
 # Coindicator
 
 ![Coin Price logo](src/coin/resources/logo_124px.png)
 
 Coindicator is a cryptocurrency price indicator applet for Linux.
 
 [![PyPI version](https://badge.fury.io/py/coindicator.svg)](https://badge.fury.io/py/coindicator)
@@ -50,15 +66,15 @@
 ## Running
 
 * A launcher icon "Coindicator" should have been installed that can be used to start the app
 * Alternatively, go to the install folder, activate the environment `source venv/bin/activate` and run the app with `coindicator`. Add ` &` to run it in the background.
 
 ## Configuring
 
-Use the GUI to add and remove indicators (find the piggy icon), to pick assets, to set refresh frequency and to set alarms. Alternatively, edit the **user.conf** YAML file in the project root.
+Use the GUI to add and remove indicators (find the piggy icon), to pick assets, to set refresh frequency and to set alarms. Alternatively, edit the **~/.config/coindicator/user.conf** YAML file.
 
 `max_decimals`: default 8. Lower if you want fewer decimals (takes priority over `significant_digits`)
 `significant_digits`: default 3. Set to higher if you want more significant digits.
 
 ## Extending (Plug-ins)
 
 Adding your own exchange plug-in is easy. Just create class file with methods for returning a ticker URL, a discovery URL, and parsing the responses from the ticker and discovery APIs. Then add the file to the `exchanges` folder.
@@ -79,22 +95,15 @@
 * Ubuntu Linux 17.10 (Artful Aardvark) with GNOME 3 and Unity 7
 * Ubuntu Linux 18.04 (Bionic Beaver) with GNOME 3 and Unity 7
 * Ubuntu Linux 19.04 (Disco Dingo) with GNOME 3 and Unity 7
 * Ubuntu Linux 19.10 (Eoan Ermine) with GNOME 3 and Unity 7
 * Ubuntu Linux 20.04 (Focal Fossa) with GNOME 3
 * Ubuntu Linux 20.10 (Groovy Gorilla) with GNOME 3
 * Ubuntu Linux 21.04 (Hirsute Hippo) with GNOME 3
-* Ubuntu Linux 21.10 (Impish Indri) with GNOME 3
-* Ubuntu Linux 22.04 (Jammy Jellyfish) with GNOME 3
-* Ubuntu Linux 22.10 (Kinetic Kudu) with GNOME 3
+* Ubuntu Linux 21.10 (Impish Indri) with GNOME 40
+* Ubuntu Linux 22.04 (Jammy Jellyfish) with GNOME 42
+* Ubuntu Linux 22.10 (Kinetic Kudu) with GNOME 43
+* Ubuntu Linux 23.04 (Lunar Lobster) with GNOME 44
 
 For other systems, you may need to install LibAppIndicator support.
 
-Before reporting bugs or issues, please try removing **~/.config/coindicator/user.conf** first and then the files in **~/.config/coindicator/cache/**.
-
-## Sponsorship and Funding
-
-![Gitcoin logo](img/gitcoin.png)
-
-This project has been funded in the past by generous maecenas @ghettodev through [Gitcoin](https://gitcoin.co/), a platform that directs the attention of bounty hunters (coders) to open issues and feature requests on Github.
-
-If you would like to sponsor a feature request, bug report or just donate to the project, be sure to check out [Gitcoin](https://gitcoin.co/).
+Before reporting bugs or issues, please try removing/renaming the **~/.config/coindicator** folder first.
```

### Comparing `coindicator-2.1.6/img/gitcoin.png` & `coindicator-2.1.7/img/gitcoin.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/img/screenshot.png` & `coindicator-2.1.7/img/screenshot.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/install.sh` & `coindicator-2.1.7/install.sh`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/requirements.txt` & `coindicator-2.1.7/requirements.txt`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/setup.cfg` & `coindicator-2.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/setup.py` & `coindicator-2.1.7/setup.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/src/coin/about.py` & `coindicator-2.1.7/src/coin/about.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/src/coin/alarm.py` & `coindicator-2.1.7/src/coin/alarm.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/src/coin/asset_selection.py` & `coindicator-2.1.7/src/coin/asset_selection.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/src/coin/coin.py` & `coindicator-2.1.7/src/coin/coin.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/src/coin/coingecko_client.py` & `coindicator-2.1.7/src/coin/coingecko_client.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/src/coin/config.py` & `coindicator-2.1.7/src/coin/config.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/src/coin/config.yaml` & `coindicator-2.1.7/src/coin/config.yaml`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/src/coin/downloader.py` & `coindicator-2.1.7/src/coin/downloader.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/src/coin/error.py` & `coindicator-2.1.7/src/coin/error.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/src/coin/exchange.py` & `coindicator-2.1.7/src/coin/exchange.py`

 * *Files 7% similar despite different names*

```diff
@@ -50,22 +50,20 @@
         self.started = False
         self.asset_pair = {}
         self.config = Config()
 
     ##
     # Abstract methods to be overwritten by the child classes
     #
-    @classmethod
     @abc.abstractmethod
-    def _get_discovery_url(cls):
+    def _get_discovery_url(self):
         pass
 
-    @classmethod
     @abc.abstractmethod
-    def _parse_discovery(cls, data):
+    def _parse_discovery(self, data):
         pass
 
     @abc.abstractmethod
     def _get_ticker_url(self):
         pass
 
     @abc.abstractmethod
@@ -123,25 +121,23 @@
         if not self.asset_pair:
             logging.warning(
                 "User.conf specifies unavailable asset pair, trying default. \
                 Run Asset Discovery again."
             )
             self.asset_pair = {}
 
-    @classmethod
-    def find_asset_pair_by_code(cls, code):
-        for ap in cls.asset_pairs:
+    def find_asset_pair_by_code(self, code):
+        for ap in self.asset_pairs:
             if ap.get("pair") == code:
                 return ap
 
         return {}
 
-    @classmethod
-    def find_asset_pair(cls, quote, base):
-        for ap in cls.asset_pairs:
+    def find_asset_pair(self, quote, base):
+        for ap in self.asset_pairs:
             if ap.get("quote") == quote and ap.get("base") == base:
                 return ap
 
         return {}
 
     @property
     def datafile(self):
@@ -162,73 +158,69 @@
         except IOError:
             # Faulty data file, return empty array
             return []
 
     ##
     # Saves asset pairs to disk
     #
-    @classmethod
-    def store_asset_pairs(cls, asset_pairs):
+    def store_asset_pairs(self, asset_pairs):
         try:
-            with open(cls.datafile, "wb") as stream:
+            with open(self.datafile, "wb") as stream:
                 pickle.dump(asset_pairs, stream)
         except IOError:
-            logging.error("Could not write to data file %s" % cls.datafile)
+            logging.error("Could not write to data file %s" % self.datafile)
 
     ##
     # Discovers assets from the exchange's API url retrieved
     # through the instance-specific method _get_discovery_url()
     #
-    @classmethod
-    def discover_assets(cls, downloader, callback):
-        if cls._get_discovery_url() is None:
-            cls.store_asset_pairs(cls._parse_discovery(None))
+    def discover_assets(self, downloader, callback):
+        if self._get_discovery_url() is None:
+            self.store_asset_pairs(self._parse_discovery(None))
         else:
-            command = DownloadCommand(cls._get_discovery_url(), callback)
-            downloader.execute(command, cls._handle_discovery_result)
+            command = DownloadCommand(self._get_discovery_url(), callback)
+            downloader.execute(command, self._handle_discovery_result)
 
     ##
     # Deals with the result from the discovery HTTP request
     # Should probably be merged with _handle_result() later
     #
-    @classmethod
-    def _handle_discovery_result(cls, command):
+    def _handle_discovery_result(self, command):
         logging.debug("Response from %s: %s" % (command.url, command.error))
 
         if command.error:
-            cls._handle_discovery_error(
-                f"{cls.name}: API server {command.url}\
+            self._handle_discovery_error(
+                f"{self.name}: API server {command.url}\
                      returned an error: {command.error}"
             )
 
         if command.response:
             data = command.response
 
             if data.status_code in [301, 302]:
                 # hooks will be called even when requests is following a redirect
                 # but we don't want to print any error messages here
                 return
 
             if data.status_code != 200:
-                cls._handle_discovery_error(
+                self._handle_discovery_error(
                     f"API server {command.url} returned \
                         an error: {str(data.status_code)}"
                 )
 
             try:
                 result = data.json()
-                asset_pairs = cls._parse_discovery(result)
-                cls.store_asset_pairs(asset_pairs)
+                asset_pairs = self._parse_discovery(result)
+                self.store_asset_pairs(asset_pairs)
             except Exception as e:
-                cls._handle_discovery_error(str(e))
+                self._handle_discovery_error(str(e))
 
         command.callback()  # update the asset menus of all instances
 
-    @classmethod
-    def _handle_discovery_error(cls, msg):
+    def _handle_discovery_error(self, msg):
         logging.warn("Asset Discovery: %s" % msg)
 
     ##
     # Start exchange
     #
     def start(self, error_refresh=None):
         if not self.started:
```

### Comparing `coindicator-2.1.6/src/coin/exchanges/binance.py` & `coindicator-2.1.7/src/coin/exchanges/binance.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # Binance
 # https://github.com/binance-exchange/binance-official-api-docs/blob/master/rest-api.md
 # By Lari Taskula <lari@taskula.fi>
 
-from coin.exchange import CURRENCY, Exchange
+from coin.exchange import Exchange
 
 
 class Binance(Exchange):
     name = "Binance"
     code = "binance"
 
     ticker = "https://www.binance.com/api/v1/ticker/24hr"
     discovery = "https://www.binance.com/api/v1/exchangeInfo"
 
     default_label = "cur"
 
-    @classmethod
-    def _get_discovery_url(cls):
-        return cls.discovery
+    def _get_discovery_url(self):
+        return self.discovery
 
     def _get_ticker_url(self):
         return self.ticker + "?symbol=" + self.pair
 
     @staticmethod
     def _parse_discovery(result):
         asset_pairs = []
```

### Comparing `coindicator-2.1.6/src/coin/exchanges/bitfinex.py` & `coindicator-2.1.7/src/coin/exchanges/bitfinex.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # Bitfinex
 # https://bitfinex.readme.io/v2/docs
 # By Alessio Carrafa <ruzzico@gmail.com>
 
-from coin.exchange import CURRENCY, Exchange
+from coin.exchange import Exchange
 
 
 class Bitfinex(Exchange):
     name = "Bitfinex"
     code = "bitfinex"
 
     ticker = "https://api.bitfinex.com/v2/ticker/"
     discovery = "https://api.bitfinex.com/v1/symbols"
 
     default_label = "cur"
 
-    @classmethod
-    def _get_discovery_url(cls):
-        return cls.discovery
+    def _get_discovery_url(self):
+        return self.discovery
 
     def _get_ticker_url(self):
         return self.ticker + self.pair
 
     @staticmethod
     def _parse_discovery(result):
         asset_pairs = []
```

### Comparing `coindicator-2.1.6/src/coin/exchanges/bitkub.py` & `coindicator-2.1.7/src/coin/exchanges/bitkub.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # Bitkub
 # https://github.com/bitkub/bitkub-official-api-docs/blob/master/restful-api.md
 # By Theppasith N. <tutorgaming@gmail.com>
 
-from coin.exchange import CURRENCY, Exchange
+from coin.exchange import Exchange
 
 
 class Bitkub(Exchange):
     name = "Bitkub"
     code = "bitkub"
 
     ticker = "https://api.bitkub.com/api/market/ticker"
     discovery = "https://api.bitkub.com/api/market/symbols"
 
     default_label = "cur"
 
-    @classmethod
-    def _get_discovery_url(cls):
-        return cls.discovery
+    def _get_discovery_url(self):
+        return self.discovery
 
     def _get_ticker_url(self):
         return self.ticker + "?sym=" + self.pair
 
     @staticmethod
     def _parse_discovery(result):
         asset_pairs = []
```

### Comparing `coindicator-2.1.6/src/coin/exchanges/bitstamp.py` & `coindicator-2.1.7/src/coin/exchanges/bitstamp.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # Bitstamp
 # https://www.bitstamp.net/api/
 # By Nil Gradisnik <nil.gradisnik@gmail.com>
 
-from coin.exchange import CURRENCY, Exchange
+from coin.exchange import Exchange
 
 
 class Bitstamp(Exchange):
     name = "Bitstamp"
     code = "bitstamp"
 
     ticker = "https://www.bitstamp.net/api/v2/ticker/"
     discovery = "https://www.bitstamp.net/api/v2/trading-pairs-info/"
 
     default_label = "cur"
 
-    @classmethod
-    def _get_discovery_url(cls):
-        return cls.discovery
+    def _get_discovery_url(self):
+        return self.discovery
 
     def _get_ticker_url(self):
         return self.ticker + self.pair
 
     @staticmethod
     def _parse_discovery(result):
         asset_pairs = []
```

### Comparing `coindicator-2.1.6/src/coin/exchanges/bittrex.py` & `coindicator-2.1.7/src/coin/exchanges/bittrex.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,16 @@
     code = "bittrex"
 
     ticker = "https://api.bittrex.com/v3/markets/{}/ticker"
     discovery = "https://api.bittrex.com/v3/markets"
 
     default_label = "ask"
 
-    @classmethod
-    def _get_discovery_url(cls):
-        return cls.discovery
+    def _get_discovery_url(self):
+        return self.discovery
 
     def _get_ticker_url(self):
         return self.ticker.format(self.pair)
 
     @staticmethod
     def _parse_discovery(result):
         asset_pairs = []
```

### Comparing `coindicator-2.1.6/src/coin/exchanges/cexio.py` & `coindicator-2.1.7/src/coin/exchanges/cexio.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,16 @@
     code = "cexio"
 
     ticker = "https://cex.io/api/ticker"
     discovery = "https://cex.io/api/currency_limits"
 
     default_label = "cur"
 
-    @classmethod
-    def _get_discovery_url(cls):
-        return cls.discovery
+    def _get_discovery_url(self):
+        return self.discovery
 
     def _get_ticker_url(self):
         return self.ticker + "/" + self.pair  # base/quote
 
     @staticmethod
     def _parse_discovery(result):
         asset_pairs = []
```

### Comparing `coindicator-2.1.6/src/coin/exchanges/gemini.py` & `coindicator-2.1.7/src/coin/exchanges/gemini.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # Gemini
 # https://docs.gemini.com/rest-api/
 # By Rick Ramstetter <rick@anteaterllc.com>
 
-from coin.exchange import CURRENCY, Exchange
+from coin.exchange import Exchange
 
 
 class Gemini(Exchange):
     name = "Gemini"
     code = "gemini"
 
     ticker = "https://api.gemini.com/v1/pubticker/"
     discovery = "https://api.gemini.com/v1/symbols"
 
     default_label = "cur"
 
-    @classmethod
-    def _get_discovery_url(cls):
-        return cls.discovery
+    def _get_discovery_url(self):
+        return self.discovery
 
     def _get_ticker_url(self):
         return self.ticker + self.pair
 
     @staticmethod
     def _parse_discovery(result):
         asset_pairs = []
```

### Comparing `coindicator-2.1.6/src/coin/exchanges/hitbtc.py` & `coindicator-2.1.7/src/coin/exchanges/hitbtc.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # HitBTC
 # https://github.com/hitbtc-com/hitbtc-api/blob/master/APIv1.md
 # By Sander Van de Moortel <sander.vandemoortel@gmail.com>
 
-from coin.exchange import CURRENCY, Exchange
+from coin.exchange import Exchange
 
 
 class Hitbtc(Exchange):
     name = "HitBTC"
     code = "hitbtc"
 
     ticker = "https://api.hitbtc.com/api/1/public/"
     discovery = "http://api.hitbtc.com/api/1/public/symbols"
 
     default_label = "cur"
 
-    @classmethod
-    def _get_discovery_url(cls):
-        return cls.discovery
+    def _get_discovery_url(self):
+        return self.discovery
 
     def _get_ticker_url(self):
         return self.ticker + self.pair + "/ticker"
 
     @staticmethod
     def _parse_discovery(result):
         asset_pairs = []
```

### Comparing `coindicator-2.1.6/src/coin/exchanges/kraken.py` & `coindicator-2.1.7/src/coin/exchanges/kraken.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # Kraken
 # https://www.kraken.com/help/api#public-market-data
 # By Nil Gradisnik <nil.gradisnik@gmail.com>
 
-from coin.exchange import CURRENCY, Exchange
+from coin.exchange import Exchange
 
 
 class Kraken(Exchange):
     name = "Kraken"
     code = "kraken"
 
     ticker = "https://api.kraken.com/0/public/Ticker"
     discovery = "https://api.kraken.com/0/public/AssetPairs"
 
     default_label = "cur"
 
-    @classmethod
-    def _get_discovery_url(cls):
-        return cls.discovery
+    def _get_discovery_url(self):
+        return self.discovery
 
     def _get_ticker_url(self):
         return self.ticker + "?pair=" + self.pair
 
     @staticmethod
     def _parse_discovery(result):
         asset_pairs = []
```

### Comparing `coindicator-2.1.6/src/coin/exchanges/okcoin.py` & `coindicator-2.1.7/src/coin/exchanges/okcoin.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,23 +10,22 @@
     code = "okcoin"
 
     ticker = "https://www.okcoin.cn/api/v1/ticker.do"
     discovery = False  # no discovery here
 
     default_label = "cur"
 
-    @classmethod
-    def _get_discovery_url(cls):
+    def _get_discovery_url(self):
         return None
 
     def _get_ticker_url(self):
         return self.ticker + "?symbol=" + self.pair  # base/quote
 
     @staticmethod
-    def _parse_discovery(result):
+    def _parse_discovery(_):
         return [
             {"pair": "btc_cny", "name": "BTC to CNY", "currency": CURRENCY["cny"]},
             {"pair": "ltc_cny", "name": "LTC to CNY", "currency": CURRENCY["cny"]},
             {"pair": "eth_cny", "name": "ETH to CNY", "currency": CURRENCY["cny"]},
         ]
 
     def _parse_ticker(self, asset):
```

### Comparing `coindicator-2.1.6/src/coin/exchanges/poloniex.py` & `coindicator-2.1.7/src/coin/exchanges/poloniex.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,17 +10,16 @@
     code = "poloniex"
 
     ticker = "https://poloniex.com/public?command=returnTicker"
     discovery = "https://poloniex.com/public?command=returnTicker"
 
     default_label = "cur"
 
-    @classmethod
-    def _get_discovery_url(cls):
-        return cls.discovery
+    def _get_discovery_url(self):
+        return self.discovery
 
     def _get_ticker_url(self):
         return self.ticker
 
     @staticmethod
     def _parse_discovery(result):
         asset_pairs = []
```

### Comparing `coindicator-2.1.6/src/coin/exchanges/unocoin.py` & `coindicator-2.1.7/src/coin/exchanges/unocoin.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,25 @@
 # Unocoin
 # https://www.unocoin.com/how-it-works?info=tickerapi
 # By Sander Van de Moortel <sander.vandemoortel@gmail.com>
 
-from coin.exchange import CURRENCY, Exchange
+from coin.exchange import Exchange
 
 
 class Unocoin(Exchange):
     name = "Unocoin"
     code = "unocoin"
 
     ticker = "https://api.unocoin.com/api/trades/{}/all"
     discovery = "https://api.unocoin.com/api/trades/all/all"
 
     default_label = "avg"
 
-    @classmethod
-    def _get_discovery_url(cls):
-        return cls.discovery
+    def _get_discovery_url(self):
+        return self.discovery
 
     def _get_ticker_url(self):
         return self.ticker.format(self.asset_pair.get("base").lower())
 
     @staticmethod
     def _parse_discovery(result):
         asset_pairs = []
```

### Comparing `coindicator-2.1.6/src/coin/indicator.py` & `coindicator-2.1.7/src/coin/indicator.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/src/coin/plugin_selection.py` & `coindicator-2.1.7/src/coin/plugin_selection.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/src/coin/resources/ca-ching.wav` & `coindicator-2.1.7/src/coin/resources/ca-ching.wav`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/src/coin/resources/icon.png` & `coindicator-2.1.7/src/coin/resources/icon.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/src/coin/resources/icon_32px.png` & `coindicator-2.1.7/src/coin/resources/icon_32px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/src/coin/resources/icon_48px.png` & `coindicator-2.1.7/src/coin/resources/icon_48px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/src/coin/resources/icon_64px.png` & `coindicator-2.1.7/src/coin/resources/icon_64px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/src/coin/resources/loading.png` & `coindicator-2.1.7/src/coin/resources/loading.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/src/coin/resources/logo_124px.png` & `coindicator-2.1.7/src/coin/resources/logo_124px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/src/coin/resources/logo_124pxs.png` & `coindicator-2.1.7/src/coin/resources/logo_124pxs.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/src/coin/resources/logo_248px.png` & `coindicator-2.1.7/src/coin/resources/logo_248px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.6/src/coindicator.egg-info/PKG-INFO` & `coindicator-2.1.7/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,23 +1,7 @@
-Metadata-Version: 2.1
-Name: coindicator
-Version: 2.1.6
-Summary: Coinprice Indicator
-Home-page: https://github.com/bluppfisk/coindicator/
-Author: Sander Van de Moortel
-Author-email: sander.vandemoortel@gmail.com
-License: MIT
-Project-URL: Documentation, https://github.com/bluppfisk/coindicator/
-Platform: Linux
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Programming Language :: Python
-Description-Content-Type: text/markdown; charset=UTF-8
-Provides-Extra: develop
-License-File: LICENSE
-
 # Coindicator
 
 ![Coin Price logo](src/coin/resources/logo_124px.png)
 
 Coindicator is a cryptocurrency price indicator applet for Linux.
 
 [![PyPI version](https://badge.fury.io/py/coindicator.svg)](https://badge.fury.io/py/coindicator)
@@ -66,15 +50,15 @@
 ## Running
 
 * A launcher icon "Coindicator" should have been installed that can be used to start the app
 * Alternatively, go to the install folder, activate the environment `source venv/bin/activate` and run the app with `coindicator`. Add ` &` to run it in the background.
 
 ## Configuring
 
-Use the GUI to add and remove indicators (find the piggy icon), to pick assets, to set refresh frequency and to set alarms. Alternatively, edit the **user.conf** YAML file in the project root.
+Use the GUI to add and remove indicators (find the piggy icon), to pick assets, to set refresh frequency and to set alarms. Alternatively, edit the **~/.config/coindicator/user.conf** YAML file.
 
 `max_decimals`: default 8. Lower if you want fewer decimals (takes priority over `significant_digits`)
 `significant_digits`: default 3. Set to higher if you want more significant digits.
 
 ## Extending (Plug-ins)
 
 Adding your own exchange plug-in is easy. Just create class file with methods for returning a ticker URL, a discovery URL, and parsing the responses from the ticker and discovery APIs. Then add the file to the `exchanges` folder.
@@ -95,22 +79,15 @@
 * Ubuntu Linux 17.10 (Artful Aardvark) with GNOME 3 and Unity 7
 * Ubuntu Linux 18.04 (Bionic Beaver) with GNOME 3 and Unity 7
 * Ubuntu Linux 19.04 (Disco Dingo) with GNOME 3 and Unity 7
 * Ubuntu Linux 19.10 (Eoan Ermine) with GNOME 3 and Unity 7
 * Ubuntu Linux 20.04 (Focal Fossa) with GNOME 3
 * Ubuntu Linux 20.10 (Groovy Gorilla) with GNOME 3
 * Ubuntu Linux 21.04 (Hirsute Hippo) with GNOME 3
-* Ubuntu Linux 21.10 (Impish Indri) with GNOME 3
-* Ubuntu Linux 22.04 (Jammy Jellyfish) with GNOME 3
-* Ubuntu Linux 22.10 (Kinetic Kudu) with GNOME 3
+* Ubuntu Linux 21.10 (Impish Indri) with GNOME 40
+* Ubuntu Linux 22.04 (Jammy Jellyfish) with GNOME 42
+* Ubuntu Linux 22.10 (Kinetic Kudu) with GNOME 43
+* Ubuntu Linux 23.04 (Lunar Lobster) with GNOME 44
 
 For other systems, you may need to install LibAppIndicator support.
 
-Before reporting bugs or issues, please try removing **~/.config/coindicator/user.conf** first and then the files in **~/.config/coindicator/cache/**.
-
-## Sponsorship and Funding
-
-![Gitcoin logo](img/gitcoin.png)
-
-This project has been funded in the past by generous maecenas @ghettodev through [Gitcoin](https://gitcoin.co/), a platform that directs the attention of bounty hunters (coders) to open issues and feature requests on Github.
-
-If you would like to sponsor a feature request, bug report or just donate to the project, be sure to check out [Gitcoin](https://gitcoin.co/).
+Before reporting bugs or issues, please try removing/renaming the **~/.config/coindicator** folder first.
```

### Comparing `coindicator-2.1.6/src/coindicator.egg-info/SOURCES.txt` & `coindicator-2.1.7/src/coindicator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

