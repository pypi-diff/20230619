# Comparing `tmp/coindicator-2.1.5.tar.gz` & `tmp/coindicator-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coindicator-2.1.5.tar", last modified: Fri Jun 16 13:14:32 2023, max compression
+gzip compressed data, was "coindicator-2.1.6.tar", last modified: Mon Jun 19 08:56:00 2023, max compression
```

## Comparing `coindicator-2.1.5.tar` & `coindicator-2.1.6.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-16 13:14:32.455260 coindicator-2.1.5/
--rw-rw-r--   0 sander    (1000) sander    (1000)       83 2023-06-16 13:04:41.000000 coindicator-2.1.5/.gitignore
--rw-rw-r--   0 sander    (1000) sander    (1000)      899 2022-10-30 19:56:43.000000 coindicator-2.1.5/.pre-commit-config.yaml
--rw-r--r--   0 sander    (1000) sander    (1000)     1106 2020-04-16 00:57:46.000000 coindicator-2.1.5/LICENSE
--rw-rw-r--   0 sander    (1000) sander    (1000)       29 2023-06-16 13:04:41.000000 coindicator-2.1.5/MANIFEST.in
--rw-rw-r--   0 sander    (1000) sander    (1000)     4724 2023-06-16 13:14:32.455260 coindicator-2.1.5/PKG-INFO
--rw-rw-r--   0 sander    (1000) sander    (1000)     4213 2023-06-16 13:04:41.000000 coindicator-2.1.5/README.md
--rw-rw-r--   0 sander    (1000) sander    (1000)      369 2023-06-16 13:04:41.000000 coindicator-2.1.5/coindicator.desktop
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-16 13:14:32.443260 coindicator-2.1.5/img/
--rw-rw-r--   0 sander    (1000) sander    (1000)    27147 2022-10-30 19:56:43.000000 coindicator-2.1.5/img/gitcoin.png
--rw-rw-r--   0 sander    (1000) sander    (1000)   172307 2022-10-30 19:56:43.000000 coindicator-2.1.5/img/screenshot.png
--rwxrwxr-x   0 sander    (1000) sander    (1000)     1624 2023-06-16 13:04:41.000000 coindicator-2.1.5/install.sh
--rw-rw-r--   0 sander    (1000) sander    (1000)      294 2023-06-16 13:04:41.000000 coindicator-2.1.5/pyproject.toml
--rw-rw-r--   0 sander    (1000) sander    (1000)      794 2023-06-16 13:09:25.000000 coindicator-2.1.5/requirements.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)     1202 2023-06-16 13:14:32.459260 coindicator-2.1.5/setup.cfg
--rw-rw-r--   0 sander    (1000) sander    (1000)      521 2023-06-16 13:04:41.000000 coindicator-2.1.5/setup.py
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-16 13:14:32.439260 coindicator-2.1.5/src/
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-16 13:14:32.447260 coindicator-2.1.5/src/coin/
--rw-rw-r--   0 sander    (1000) sander    (1000)        0 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/__init__.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1537 2022-11-16 17:06:14.000000 coindicator-2.1.5/src/coin/about.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     6537 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/alarm.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     5794 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/asset_selection.py
--rwxrwxr-x   0 sander    (1000) sander    (1000)    12627 2023-06-16 13:04:41.000000 coindicator-2.1.5/src/coin/coin.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1751 2023-06-16 13:04:41.000000 coindicator-2.1.5/src/coin/coingecko_client.py
--rw-rw-r--   0 sander    (1000) sander    (1000)      609 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/config.py
--rw-rw-r--   0 sander    (1000) sander    (1000)      977 2022-11-16 17:07:14.000000 coindicator-2.1.5/src/coin/config.yaml
--rw-rw-r--   0 sander    (1000) sander    (1000)     1422 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/downloader.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1177 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/error.py
--rw-rw-r--   0 sander    (1000) sander    (1000)    10512 2023-06-16 12:11:35.000000 coindicator-2.1.5/src/coin/exchange.py
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-16 13:14:32.451260 coindicator-2.1.5/src/coin/exchanges/
--rw-rw-r--   0 sander    (1000) sander    (1000)     1771 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/exchanges/binance.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1579 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/exchanges/bitfinex.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1834 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/exchanges/bitkub.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1493 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/exchanges/bitstamp.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     2031 2022-11-16 17:02:06.000000 coindicator-2.1.5/src/coin/exchanges/bittrex.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1473 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/exchanges/cexio.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1499 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/exchanges/gemini.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1718 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/exchanges/hitbtc.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     2083 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/exchanges/kraken.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1273 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/exchanges/okcoin.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1547 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/exchanges/poloniex.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1281 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/exchanges/unocoin.py
--rw-rw-r--   0 sander    (1000) sander    (1000)    10370 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/indicator.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     2608 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/plugin_selection.py
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-16 13:14:32.455260 coindicator-2.1.5/src/coin/resources/
--rw-rw-r--   0 sander    (1000) sander    (1000)   294232 2023-06-16 13:04:41.000000 coindicator-2.1.5/src/coin/resources/ca-ching.wav
--rw-rw-r--   0 sander    (1000) sander    (1000)     5060 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/resources/icon.png
--rw-rw-r--   0 sander    (1000) sander    (1000)      983 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/resources/icon_32px.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     1440 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/resources/icon_48px.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     1673 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/resources/icon_64px.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     1889 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/resources/loading.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     4619 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/resources/logo_124px.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     7329 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/resources/logo_124pxs.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     6508 2022-10-30 19:56:43.000000 coindicator-2.1.5/src/coin/resources/logo_248px.png
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-16 13:14:32.455260 coindicator-2.1.5/src/coindicator.egg-info/
--rw-rw-r--   0 sander    (1000) sander    (1000)     4724 2023-06-16 13:14:32.000000 coindicator-2.1.5/src/coindicator.egg-info/PKG-INFO
--rw-rw-r--   0 sander    (1000) sander    (1000)     1388 2023-06-16 13:14:32.000000 coindicator-2.1.5/src/coindicator.egg-info/SOURCES.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-16 13:14:32.000000 coindicator-2.1.5/src/coindicator.egg-info/dependency_links.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)       47 2023-06-16 13:14:32.000000 coindicator-2.1.5/src/coindicator.egg-info/entry_points.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-16 11:50:35.000000 coindicator-2.1.5/src/coindicator.egg-info/not-zip-safe
--rw-rw-r--   0 sander    (1000) sander    (1000)      227 2023-06-16 13:14:32.000000 coindicator-2.1.5/src/coindicator.egg-info/requires.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)        5 2023-06-16 13:14:32.000000 coindicator-2.1.5/src/coindicator.egg-info/top_level.txt
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 08:56:00.618748 coindicator-2.1.6/
+-rw-rw-r--   0 sander    (1000) sander    (1000)       83 2023-06-16 13:19:52.000000 coindicator-2.1.6/.gitignore
+-rw-rw-r--   0 sander    (1000) sander    (1000)      899 2022-10-30 19:56:43.000000 coindicator-2.1.6/.pre-commit-config.yaml
+-rw-r--r--   0 sander    (1000) sander    (1000)     1106 2020-04-16 00:57:46.000000 coindicator-2.1.6/LICENSE
+-rw-rw-r--   0 sander    (1000) sander    (1000)       29 2023-06-16 13:19:52.000000 coindicator-2.1.6/MANIFEST.in
+-rw-rw-r--   0 sander    (1000) sander    (1000)     4823 2023-06-19 08:56:00.618748 coindicator-2.1.6/PKG-INFO
+-rw-rw-r--   0 sander    (1000) sander    (1000)     4312 2023-06-16 13:19:52.000000 coindicator-2.1.6/README.md
+-rw-rw-r--   0 sander    (1000) sander    (1000)      369 2023-06-16 13:19:52.000000 coindicator-2.1.6/coindicator.desktop
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 08:56:00.606748 coindicator-2.1.6/img/
+-rw-rw-r--   0 sander    (1000) sander    (1000)    27147 2022-10-30 19:56:43.000000 coindicator-2.1.6/img/gitcoin.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)   172307 2022-10-30 19:56:43.000000 coindicator-2.1.6/img/screenshot.png
+-rwxrwxr-x   0 sander    (1000) sander    (1000)     1576 2023-06-16 15:26:25.000000 coindicator-2.1.6/install.sh
+-rw-rw-r--   0 sander    (1000) sander    (1000)      294 2023-06-16 13:19:52.000000 coindicator-2.1.6/pyproject.toml
+-rw-rw-r--   0 sander    (1000) sander    (1000)      794 2023-06-16 13:19:52.000000 coindicator-2.1.6/requirements.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1202 2023-06-19 08:56:00.622748 coindicator-2.1.6/setup.cfg
+-rw-rw-r--   0 sander    (1000) sander    (1000)      521 2023-06-16 13:19:52.000000 coindicator-2.1.6/setup.py
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 08:56:00.602748 coindicator-2.1.6/src/
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 08:56:00.610748 coindicator-2.1.6/src/coin/
+-rw-rw-r--   0 sander    (1000) sander    (1000)        0 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/__init__.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1537 2023-06-16 13:19:52.000000 coindicator-2.1.6/src/coin/about.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     6537 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/alarm.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     5794 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/asset_selection.py
+-rwxrwxr-x   0 sander    (1000) sander    (1000)    12615 2023-06-19 08:32:25.000000 coindicator-2.1.6/src/coin/coin.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1751 2023-06-16 13:19:52.000000 coindicator-2.1.6/src/coin/coingecko_client.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)      609 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/config.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)      977 2023-06-16 13:19:52.000000 coindicator-2.1.6/src/coin/config.yaml
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1422 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/downloader.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1177 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/error.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)    10482 2023-06-19 08:54:53.000000 coindicator-2.1.6/src/coin/exchange.py
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 08:56:00.614748 coindicator-2.1.6/src/coin/exchanges/
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1771 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/exchanges/binance.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1579 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/exchanges/bitfinex.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1834 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/exchanges/bitkub.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1493 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/exchanges/bitstamp.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2031 2023-06-16 13:19:52.000000 coindicator-2.1.6/src/coin/exchanges/bittrex.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1473 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/exchanges/cexio.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1499 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/exchanges/gemini.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1718 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/exchanges/hitbtc.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2083 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/exchanges/kraken.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1273 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/exchanges/okcoin.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1547 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/exchanges/poloniex.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1281 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/exchanges/unocoin.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)    10370 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/indicator.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2608 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/plugin_selection.py
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 08:56:00.618748 coindicator-2.1.6/src/coin/resources/
+-rw-rw-r--   0 sander    (1000) sander    (1000)   294232 2023-06-16 13:19:52.000000 coindicator-2.1.6/src/coin/resources/ca-ching.wav
+-rw-rw-r--   0 sander    (1000) sander    (1000)     5060 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/resources/icon.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)      983 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/resources/icon_32px.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1440 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/resources/icon_48px.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1673 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/resources/icon_64px.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1889 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/resources/loading.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     4619 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/resources/logo_124px.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     7329 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/resources/logo_124pxs.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     6508 2022-10-30 19:56:43.000000 coindicator-2.1.6/src/coin/resources/logo_248px.png
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 08:56:00.618748 coindicator-2.1.6/src/coindicator.egg-info/
+-rw-rw-r--   0 sander    (1000) sander    (1000)     4823 2023-06-19 08:56:00.000000 coindicator-2.1.6/src/coindicator.egg-info/PKG-INFO
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1388 2023-06-19 08:56:00.000000 coindicator-2.1.6/src/coindicator.egg-info/SOURCES.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-19 08:56:00.000000 coindicator-2.1.6/src/coindicator.egg-info/dependency_links.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)       47 2023-06-19 08:56:00.000000 coindicator-2.1.6/src/coindicator.egg-info/entry_points.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-16 11:50:35.000000 coindicator-2.1.6/src/coindicator.egg-info/not-zip-safe
+-rw-rw-r--   0 sander    (1000) sander    (1000)      227 2023-06-19 08:56:00.000000 coindicator-2.1.6/src/coindicator.egg-info/requires.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)        5 2023-06-19 08:56:00.000000 coindicator-2.1.6/src/coindicator.egg-info/top_level.txt
```

### Comparing `coindicator-2.1.5/.pre-commit-config.yaml` & `coindicator-2.1.6/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/LICENSE` & `coindicator-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/PKG-INFO` & `coindicator-2.1.6/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coindicator
-Version: 2.1.5
+Version: 2.1.6
 Summary: Coinprice Indicator
 Home-page: https://github.com/bluppfisk/coindicator/
 Author: Sander Van de Moortel
 Author-email: sander.vandemoortel@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/bluppfisk/coindicator/
 Platform: Linux
@@ -47,31 +47,30 @@
 ![Screenshot](img/screenshot.png)
 
 ## Installing
 
 You will need Git and Python 3.5 or higher, as well as some system dependencies.
 
 For your convenience, I've included a small install script that will install (or upgrade)
-coindicator and its dependencies, as well as create a desktop icon.
+coindicator and its dependencies, as well as create a desktop icon. It will ask to elevate
+permissions to install dependencies. It takes the install location as an argument.
 
 ```bash
- git clone https://github.com/bluppfisk/coindicator.git
- cd coindicator
- ./install.sh
+ git clone https://github.com/bluppfisk/coindicator.git && cd coindicator
+ ./install.sh /opt/coindicator  # or wherever you want it installed.
 ```
 
 ## Upgrading from 1.x
 
 User data has moved to your home folder. To keep your settings, move the user.conf file to: **~/.config/coindicator/**.
 
 ## Running
 
-* A launcher icon "Coindicator" should be installed that can be used to start the app
-* Alternatively, run `./run.sh` to activate the virtual environment and start the app
-* You can also run the program manually with `source env/bin/activate` and then run `src/coin/coin.py &` or `python3 src/coin/coin.py &` to start the app
+* A launcher icon "Coindicator" should have been installed that can be used to start the app
+* Alternatively, go to the install folder, activate the environment `source venv/bin/activate` and run the app with `coindicator`. Add ` &` to run it in the background.
 
 ## Configuring
 
 Use the GUI to add and remove indicators (find the piggy icon), to pick assets, to set refresh frequency and to set alarms. Alternatively, edit the **user.conf** YAML file in the project root.
 
 `max_decimals`: default 8. Lower if you want fewer decimals (takes priority over `significant_digits`)
 `significant_digits`: default 3. Set to higher if you want more significant digits.
```

### Comparing `coindicator-2.1.5/README.md` & `coindicator-2.1.6/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -31,31 +31,30 @@
 ![Screenshot](img/screenshot.png)
 
 ## Installing
 
 You will need Git and Python 3.5 or higher, as well as some system dependencies.
 
 For your convenience, I've included a small install script that will install (or upgrade)
-coindicator and its dependencies, as well as create a desktop icon.
+coindicator and its dependencies, as well as create a desktop icon. It will ask to elevate
+permissions to install dependencies. It takes the install location as an argument.
 
 ```bash
- git clone https://github.com/bluppfisk/coindicator.git
- cd coindicator
- ./install.sh
+ git clone https://github.com/bluppfisk/coindicator.git && cd coindicator
+ ./install.sh /opt/coindicator  # or wherever you want it installed.
 ```
 
 ## Upgrading from 1.x
 
 User data has moved to your home folder. To keep your settings, move the user.conf file to: **~/.config/coindicator/**.
 
 ## Running
 
-* A launcher icon "Coindicator" should be installed that can be used to start the app
-* Alternatively, run `./run.sh` to activate the virtual environment and start the app
-* You can also run the program manually with `source env/bin/activate` and then run `src/coin/coin.py &` or `python3 src/coin/coin.py &` to start the app
+* A launcher icon "Coindicator" should have been installed that can be used to start the app
+* Alternatively, go to the install folder, activate the environment `source venv/bin/activate` and run the app with `coindicator`. Add ` &` to run it in the background.
 
 ## Configuring
 
 Use the GUI to add and remove indicators (find the piggy icon), to pick assets, to set refresh frequency and to set alarms. Alternatively, edit the **user.conf** YAML file in the project root.
 
 `max_decimals`: default 8. Lower if you want fewer decimals (takes priority over `significant_digits`)
 `significant_digits`: default 3. Set to higher if you want more significant digits.
```

### Comparing `coindicator-2.1.5/img/gitcoin.png` & `coindicator-2.1.6/img/gitcoin.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/img/screenshot.png` & `coindicator-2.1.6/img/screenshot.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/install.sh` & `coindicator-2.1.6/install.sh`

 * *Files 6% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 # sudo apt update
 # sudo apt install cmake
 
 # Install python packages
 sudo mkdir ${args[0]} 2>/dev/null
 sudo python3 -m venv ${args[0]}/venv
 source ${args[0]}/venv/bin/activate
-sudo -H -E env PATH=$PATH pip3 install --no-cache-dir --use-deprecated=legacy-resolver -U coindicator
+sudo -H -E env PATH=$PATH pip3 install -U coindicator
 
 # Install shortcut
 cat > /tmp/coindicator.desktop << EOL
 
 [Desktop Entry]
 Name=Coindicator
 GenericName=Cryptocoin price ticker
```

### Comparing `coindicator-2.1.5/requirements.txt` & `coindicator-2.1.6/requirements.txt`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/setup.cfg` & `coindicator-2.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/setup.py` & `coindicator-2.1.6/setup.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/about.py` & `coindicator-2.1.6/src/coin/about.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/alarm.py` & `coindicator-2.1.6/src/coin/alarm.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/asset_selection.py` & `coindicator-2.1.6/src/coin/asset_selection.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/coin.py` & `coindicator-2.1.6/src/coin/coin.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,14 @@
 os.environ["PYGAME_HIDE_SUPPORT_PROMPT"] = "hide"
 
 import importlib
 import logging
 import signal
 from pathlib import Path
 
-import dbus
 import notify2
 import yaml
 from dbus.mainloop.glib import DBusGMainLoop
 from gi.repository import Gtk
 
 from coin.about import AboutWindow
 from coin.downloader import AsyncDownloadService, DownloadService
```

### Comparing `coindicator-2.1.5/src/coin/coingecko_client.py` & `coindicator-2.1.6/src/coin/coingecko_client.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/config.py` & `coindicator-2.1.6/src/coin/config.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/config.yaml` & `coindicator-2.1.6/src/coin/config.yaml`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/downloader.py` & `coindicator-2.1.6/src/coin/downloader.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/error.py` & `coindicator-2.1.6/src/coin/error.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/exchange.py` & `coindicator-2.1.6/src/coin/exchange.py`

 * *Files 4% similar despite different names*

```diff
@@ -139,29 +139,27 @@
     def find_asset_pair(cls, quote, base):
         for ap in cls.asset_pairs:
             if ap.get("quote") == quote and ap.get("base") == base:
                 return ap
 
         return {}
 
-    @classmethod
     @property
-    def datafile(cls):
+    def datafile(self):
         config = Config()
-        return config["user_data_dir"] / f"cache/{cls.code}.cache"
+        return config["user_data_dir"] / f"cache/{self.code}.cache"
 
     ##
     # Loads asset pairs from the config files or,
     # failing that, from the hard-coded lines
     #
-    @classmethod
     @property
-    def asset_pairs(cls):
+    def asset_pairs(self):
         try:
-            with open(cls.datafile, "rb") as stream:
+            with open(self.datafile, "rb") as stream:
                 asset_pairs = pickle.load(stream)
                 return asset_pairs if asset_pairs else []
 
         except IOError:
             # Faulty data file, return empty array
             return []
```

### Comparing `coindicator-2.1.5/src/coin/exchanges/binance.py` & `coindicator-2.1.6/src/coin/exchanges/binance.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/exchanges/bitfinex.py` & `coindicator-2.1.6/src/coin/exchanges/bitfinex.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/exchanges/bitkub.py` & `coindicator-2.1.6/src/coin/exchanges/bitkub.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/exchanges/bitstamp.py` & `coindicator-2.1.6/src/coin/exchanges/bitstamp.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/exchanges/bittrex.py` & `coindicator-2.1.6/src/coin/exchanges/bittrex.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/exchanges/cexio.py` & `coindicator-2.1.6/src/coin/exchanges/cexio.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/exchanges/gemini.py` & `coindicator-2.1.6/src/coin/exchanges/gemini.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/exchanges/hitbtc.py` & `coindicator-2.1.6/src/coin/exchanges/hitbtc.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/exchanges/kraken.py` & `coindicator-2.1.6/src/coin/exchanges/kraken.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/exchanges/okcoin.py` & `coindicator-2.1.6/src/coin/exchanges/okcoin.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/exchanges/poloniex.py` & `coindicator-2.1.6/src/coin/exchanges/poloniex.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/exchanges/unocoin.py` & `coindicator-2.1.6/src/coin/exchanges/unocoin.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/indicator.py` & `coindicator-2.1.6/src/coin/indicator.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/plugin_selection.py` & `coindicator-2.1.6/src/coin/plugin_selection.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/resources/ca-ching.wav` & `coindicator-2.1.6/src/coin/resources/ca-ching.wav`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/resources/icon.png` & `coindicator-2.1.6/src/coin/resources/icon.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/resources/icon_32px.png` & `coindicator-2.1.6/src/coin/resources/icon_32px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/resources/icon_48px.png` & `coindicator-2.1.6/src/coin/resources/icon_48px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/resources/icon_64px.png` & `coindicator-2.1.6/src/coin/resources/icon_64px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/resources/loading.png` & `coindicator-2.1.6/src/coin/resources/loading.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/resources/logo_124px.png` & `coindicator-2.1.6/src/coin/resources/logo_124px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/resources/logo_124pxs.png` & `coindicator-2.1.6/src/coin/resources/logo_124pxs.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coin/resources/logo_248px.png` & `coindicator-2.1.6/src/coin/resources/logo_248px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.5/src/coindicator.egg-info/PKG-INFO` & `coindicator-2.1.6/src/coindicator.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coindicator
-Version: 2.1.5
+Version: 2.1.6
 Summary: Coinprice Indicator
 Home-page: https://github.com/bluppfisk/coindicator/
 Author: Sander Van de Moortel
 Author-email: sander.vandemoortel@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/bluppfisk/coindicator/
 Platform: Linux
@@ -47,31 +47,30 @@
 ![Screenshot](img/screenshot.png)
 
 ## Installing
 
 You will need Git and Python 3.5 or higher, as well as some system dependencies.
 
 For your convenience, I've included a small install script that will install (or upgrade)
-coindicator and its dependencies, as well as create a desktop icon.
+coindicator and its dependencies, as well as create a desktop icon. It will ask to elevate
+permissions to install dependencies. It takes the install location as an argument.
 
 ```bash
- git clone https://github.com/bluppfisk/coindicator.git
- cd coindicator
- ./install.sh
+ git clone https://github.com/bluppfisk/coindicator.git && cd coindicator
+ ./install.sh /opt/coindicator  # or wherever you want it installed.
 ```
 
 ## Upgrading from 1.x
 
 User data has moved to your home folder. To keep your settings, move the user.conf file to: **~/.config/coindicator/**.
 
 ## Running
 
-* A launcher icon "Coindicator" should be installed that can be used to start the app
-* Alternatively, run `./run.sh` to activate the virtual environment and start the app
-* You can also run the program manually with `source env/bin/activate` and then run `src/coin/coin.py &` or `python3 src/coin/coin.py &` to start the app
+* A launcher icon "Coindicator" should have been installed that can be used to start the app
+* Alternatively, go to the install folder, activate the environment `source venv/bin/activate` and run the app with `coindicator`. Add ` &` to run it in the background.
 
 ## Configuring
 
 Use the GUI to add and remove indicators (find the piggy icon), to pick assets, to set refresh frequency and to set alarms. Alternatively, edit the **user.conf** YAML file in the project root.
 
 `max_decimals`: default 8. Lower if you want fewer decimals (takes priority over `significant_digits`)
 `significant_digits`: default 3. Set to higher if you want more significant digits.
```

### Comparing `coindicator-2.1.5/src/coindicator.egg-info/SOURCES.txt` & `coindicator-2.1.6/src/coindicator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

