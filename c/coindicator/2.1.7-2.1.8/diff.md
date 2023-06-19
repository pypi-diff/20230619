# Comparing `tmp/coindicator-2.1.7.tar.gz` & `tmp/coindicator-2.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coindicator-2.1.7.tar", last modified: Mon Jun 19 09:26:18 2023, max compression
+gzip compressed data, was "coindicator-2.1.8.tar", last modified: Mon Jun 19 12:08:52 2023, max compression
```

## Comparing `coindicator-2.1.7.tar` & `coindicator-2.1.8.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 09:26:18.639954 coindicator-2.1.7/
--rw-rw-r--   0 sander    (1000) sander    (1000)       83 2023-06-16 13:19:52.000000 coindicator-2.1.7/.gitignore
--rw-rw-r--   0 sander    (1000) sander    (1000)      899 2022-10-30 19:56:43.000000 coindicator-2.1.7/.pre-commit-config.yaml
--rw-r--r--   0 sander    (1000) sander    (1000)     1106 2020-04-16 00:57:46.000000 coindicator-2.1.7/LICENSE
--rw-rw-r--   0 sander    (1000) sander    (1000)       29 2023-06-16 13:19:52.000000 coindicator-2.1.7/MANIFEST.in
--rw-rw-r--   0 sander    (1000) sander    (1000)     4402 2023-06-19 09:26:18.639954 coindicator-2.1.7/PKG-INFO
--rw-rw-r--   0 sander    (1000) sander    (1000)     3891 2023-06-19 09:10:17.000000 coindicator-2.1.7/README.md
--rw-rw-r--   0 sander    (1000) sander    (1000)      369 2023-06-16 13:19:52.000000 coindicator-2.1.7/coindicator.desktop
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 09:26:18.619957 coindicator-2.1.7/img/
--rw-rw-r--   0 sander    (1000) sander    (1000)    27147 2022-10-30 19:56:43.000000 coindicator-2.1.7/img/gitcoin.png
--rw-rw-r--   0 sander    (1000) sander    (1000)   172307 2022-10-30 19:56:43.000000 coindicator-2.1.7/img/screenshot.png
--rwxrwxr-x   0 sander    (1000) sander    (1000)     1576 2023-06-16 15:26:25.000000 coindicator-2.1.7/install.sh
--rw-rw-r--   0 sander    (1000) sander    (1000)      294 2023-06-16 13:19:52.000000 coindicator-2.1.7/pyproject.toml
--rw-rw-r--   0 sander    (1000) sander    (1000)      794 2023-06-16 13:19:52.000000 coindicator-2.1.7/requirements.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)     1202 2023-06-19 09:26:18.639954 coindicator-2.1.7/setup.cfg
--rw-rw-r--   0 sander    (1000) sander    (1000)      521 2023-06-16 13:19:52.000000 coindicator-2.1.7/setup.py
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 09:26:18.615957 coindicator-2.1.7/src/
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 09:26:18.627956 coindicator-2.1.7/src/coin/
--rw-rw-r--   0 sander    (1000) sander    (1000)        0 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/__init__.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1537 2023-06-16 13:19:52.000000 coindicator-2.1.7/src/coin/about.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     6537 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/alarm.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     5794 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/asset_selection.py
--rwxrwxr-x   0 sander    (1000) sander    (1000)    12615 2023-06-19 08:32:25.000000 coindicator-2.1.7/src/coin/coin.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1751 2023-06-16 13:19:52.000000 coindicator-2.1.7/src/coin/coingecko_client.py
--rw-rw-r--   0 sander    (1000) sander    (1000)      609 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/config.py
--rw-rw-r--   0 sander    (1000) sander    (1000)      977 2023-06-16 13:19:52.000000 coindicator-2.1.7/src/coin/config.yaml
--rw-rw-r--   0 sander    (1000) sander    (1000)     1422 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/downloader.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1177 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/error.py
--rw-rw-r--   0 sander    (1000) sander    (1000)    10369 2023-06-19 09:22:15.000000 coindicator-2.1.7/src/coin/exchange.py
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 09:26:18.631955 coindicator-2.1.7/src/coin/exchanges/
--rw-rw-r--   0 sander    (1000) sander    (1000)     1746 2023-06-19 09:24:08.000000 coindicator-2.1.7/src/coin/exchanges/binance.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1554 2023-06-19 09:24:13.000000 coindicator-2.1.7/src/coin/exchanges/bitfinex.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1809 2023-06-19 09:24:16.000000 coindicator-2.1.7/src/coin/exchanges/bitkub.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1468 2023-06-19 09:24:20.000000 coindicator-2.1.7/src/coin/exchanges/bitstamp.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     2016 2023-06-19 09:22:47.000000 coindicator-2.1.7/src/coin/exchanges/bittrex.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1458 2023-06-19 09:22:55.000000 coindicator-2.1.7/src/coin/exchanges/cexio.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1474 2023-06-19 09:24:26.000000 coindicator-2.1.7/src/coin/exchanges/gemini.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1693 2023-06-19 09:24:00.000000 coindicator-2.1.7/src/coin/exchanges/hitbtc.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     2058 2023-06-19 09:23:56.000000 coindicator-2.1.7/src/coin/exchanges/kraken.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1252 2023-06-19 09:25:24.000000 coindicator-2.1.7/src/coin/exchanges/okcoin.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1532 2023-06-19 09:23:19.000000 coindicator-2.1.7/src/coin/exchanges/poloniex.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1256 2023-06-19 09:24:44.000000 coindicator-2.1.7/src/coin/exchanges/unocoin.py
--rw-rw-r--   0 sander    (1000) sander    (1000)    10370 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/indicator.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     2608 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/plugin_selection.py
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 09:26:18.635955 coindicator-2.1.7/src/coin/resources/
--rw-rw-r--   0 sander    (1000) sander    (1000)   294232 2023-06-16 13:19:52.000000 coindicator-2.1.7/src/coin/resources/ca-ching.wav
--rw-rw-r--   0 sander    (1000) sander    (1000)     5060 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/resources/icon.png
--rw-rw-r--   0 sander    (1000) sander    (1000)      983 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/resources/icon_32px.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     1440 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/resources/icon_48px.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     1673 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/resources/icon_64px.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     1889 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/resources/loading.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     4619 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/resources/logo_124px.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     7329 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/resources/logo_124pxs.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     6508 2022-10-30 19:56:43.000000 coindicator-2.1.7/src/coin/resources/logo_248px.png
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 09:26:18.639954 coindicator-2.1.7/src/coindicator.egg-info/
--rw-rw-r--   0 sander    (1000) sander    (1000)     4402 2023-06-19 09:26:18.000000 coindicator-2.1.7/src/coindicator.egg-info/PKG-INFO
--rw-rw-r--   0 sander    (1000) sander    (1000)     1388 2023-06-19 09:26:18.000000 coindicator-2.1.7/src/coindicator.egg-info/SOURCES.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-19 09:26:18.000000 coindicator-2.1.7/src/coindicator.egg-info/dependency_links.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)       47 2023-06-19 09:26:18.000000 coindicator-2.1.7/src/coindicator.egg-info/entry_points.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-16 11:50:35.000000 coindicator-2.1.7/src/coindicator.egg-info/not-zip-safe
--rw-rw-r--   0 sander    (1000) sander    (1000)      227 2023-06-19 09:26:18.000000 coindicator-2.1.7/src/coindicator.egg-info/requires.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)        5 2023-06-19 09:26:18.000000 coindicator-2.1.7/src/coindicator.egg-info/top_level.txt
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:08:52.308895 coindicator-2.1.8/
+-rw-rw-r--   0 sander    (1000) sander    (1000)       83 2023-06-16 13:19:52.000000 coindicator-2.1.8/.gitignore
+-rw-rw-r--   0 sander    (1000) sander    (1000)      899 2022-10-30 19:56:43.000000 coindicator-2.1.8/.pre-commit-config.yaml
+-rw-r--r--   0 sander    (1000) sander    (1000)     1106 2020-04-16 00:57:46.000000 coindicator-2.1.8/LICENSE
+-rw-rw-r--   0 sander    (1000) sander    (1000)       29 2023-06-16 13:19:52.000000 coindicator-2.1.8/MANIFEST.in
+-rw-rw-r--   0 sander    (1000) sander    (1000)     4402 2023-06-19 12:08:52.308895 coindicator-2.1.8/PKG-INFO
+-rw-rw-r--   0 sander    (1000) sander    (1000)     3891 2023-06-19 12:03:38.000000 coindicator-2.1.8/README.md
+-rw-rw-r--   0 sander    (1000) sander    (1000)      369 2023-06-16 13:19:52.000000 coindicator-2.1.8/coindicator.desktop
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:08:52.292895 coindicator-2.1.8/img/
+-rw-rw-r--   0 sander    (1000) sander    (1000)    27147 2022-10-30 19:56:43.000000 coindicator-2.1.8/img/gitcoin.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)   172307 2022-10-30 19:56:43.000000 coindicator-2.1.8/img/screenshot.png
+-rwxrwxr-x   0 sander    (1000) sander    (1000)     1559 2023-06-19 12:08:13.000000 coindicator-2.1.8/install.sh
+-rw-rw-r--   0 sander    (1000) sander    (1000)      294 2023-06-16 13:19:52.000000 coindicator-2.1.8/pyproject.toml
+-rw-rw-r--   0 sander    (1000) sander    (1000)      742 2023-06-19 12:07:56.000000 coindicator-2.1.8/requirements.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1202 2023-06-19 12:08:52.308895 coindicator-2.1.8/setup.cfg
+-rw-rw-r--   0 sander    (1000) sander    (1000)      521 2023-06-16 13:19:52.000000 coindicator-2.1.8/setup.py
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:08:52.284895 coindicator-2.1.8/src/
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:08:52.296895 coindicator-2.1.8/src/coin/
+-rw-rw-r--   0 sander    (1000) sander    (1000)        0 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/__init__.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1537 2023-06-16 13:19:52.000000 coindicator-2.1.8/src/coin/about.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     6537 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/alarm.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     5794 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/asset_selection.py
+-rwxrwxr-x   0 sander    (1000) sander    (1000)    12303 2023-06-19 12:08:02.000000 coindicator-2.1.8/src/coin/coin.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1751 2023-06-16 13:19:52.000000 coindicator-2.1.8/src/coin/coingecko_client.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)      609 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/config.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)      977 2023-06-16 13:19:52.000000 coindicator-2.1.8/src/coin/config.yaml
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1422 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/downloader.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1177 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/error.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)    10640 2023-06-19 12:08:35.000000 coindicator-2.1.8/src/coin/exchange.py
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:08:52.300895 coindicator-2.1.8/src/coin/exchanges/
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1761 2023-06-19 12:04:55.000000 coindicator-2.1.8/src/coin/exchanges/binance.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1569 2023-06-19 12:04:53.000000 coindicator-2.1.8/src/coin/exchanges/bitfinex.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1824 2023-06-19 12:04:53.000000 coindicator-2.1.8/src/coin/exchanges/bitkub.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1483 2023-06-19 12:04:53.000000 coindicator-2.1.8/src/coin/exchanges/bitstamp.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2031 2023-06-19 12:03:08.000000 coindicator-2.1.8/src/coin/exchanges/bittrex.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1473 2023-06-19 12:03:08.000000 coindicator-2.1.8/src/coin/exchanges/cexio.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1489 2023-06-19 12:04:53.000000 coindicator-2.1.8/src/coin/exchanges/gemini.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1708 2023-06-19 12:04:53.000000 coindicator-2.1.8/src/coin/exchanges/hitbtc.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2073 2023-06-19 12:04:53.000000 coindicator-2.1.8/src/coin/exchanges/kraken.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1273 2023-06-19 12:05:15.000000 coindicator-2.1.8/src/coin/exchanges/okcoin.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1547 2023-06-19 12:03:08.000000 coindicator-2.1.8/src/coin/exchanges/poloniex.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1271 2023-06-19 12:04:53.000000 coindicator-2.1.8/src/coin/exchanges/unocoin.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)    10370 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/indicator.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2608 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/plugin_selection.py
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:08:52.304895 coindicator-2.1.8/src/coin/resources/
+-rw-rw-r--   0 sander    (1000) sander    (1000)   294232 2023-06-16 13:19:52.000000 coindicator-2.1.8/src/coin/resources/ca-ching.wav
+-rw-rw-r--   0 sander    (1000) sander    (1000)     5060 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/resources/icon.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)      983 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/resources/icon_32px.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1440 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/resources/icon_48px.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1673 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/resources/icon_64px.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1889 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/resources/loading.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     4619 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/resources/logo_124px.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     7329 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/resources/logo_124pxs.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     6508 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/resources/logo_248px.png
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:08:52.308895 coindicator-2.1.8/src/coindicator.egg-info/
+-rw-rw-r--   0 sander    (1000) sander    (1000)     4402 2023-06-19 12:08:52.000000 coindicator-2.1.8/src/coindicator.egg-info/PKG-INFO
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1388 2023-06-19 12:08:52.000000 coindicator-2.1.8/src/coindicator.egg-info/SOURCES.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-19 12:08:52.000000 coindicator-2.1.8/src/coindicator.egg-info/dependency_links.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)       47 2023-06-19 12:08:52.000000 coindicator-2.1.8/src/coindicator.egg-info/entry_points.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-16 11:50:35.000000 coindicator-2.1.8/src/coindicator.egg-info/not-zip-safe
+-rw-rw-r--   0 sander    (1000) sander    (1000)      227 2023-06-19 12:08:52.000000 coindicator-2.1.8/src/coindicator.egg-info/requires.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)        5 2023-06-19 12:08:52.000000 coindicator-2.1.8/src/coindicator.egg-info/top_level.txt
```

### Comparing `coindicator-2.1.7/.pre-commit-config.yaml` & `coindicator-2.1.8/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/LICENSE` & `coindicator-2.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/PKG-INFO` & `coindicator-2.1.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coindicator
-Version: 2.1.7
+Version: 2.1.8
 Summary: Coinprice Indicator
 Home-page: https://github.com/bluppfisk/coindicator/
 Author: Sander Van de Moortel
 Author-email: sander.vandemoortel@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/bluppfisk/coindicator/
 Platform: Linux
```

### Comparing `coindicator-2.1.7/README.md` & `coindicator-2.1.8/README.md`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/img/gitcoin.png` & `coindicator-2.1.8/img/gitcoin.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/img/screenshot.png` & `coindicator-2.1.8/img/screenshot.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/install.sh` & `coindicator-2.1.8/install.sh`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         exit 1
 fi
 
 args=("$@")
 
 echo Installing to ${args[0]}
 
-sudo apt-get install python3-venv python3-setuptools-scm python3-wheel python3-gi python3-gi-cairo gir1.2-gtk-3.0 libdbus-glib-1-2 gir1.2-appindicator3-0.1 python3-pip patchelf -y
+sudo apt-get install python3-venv python3-setuptools-scm python3-wheel python3-gi python3-gi-cairo gir1.2-gtk-3.0 gir1.2-appindicator3-0.1 python3-pip patchelf -y
 
 # some users report requiring libgirepository1.0-dev libdbus-1-dev, libcairo2-dev, build-essential
 # some report having to install a newer version of cmake
 
 # sudo apt purge --auto-remove cmake
 # wget -O - https://apt.kitware.com/keys/kitware-archive-latest.asc 2>/dev/null | gpg --dearmor - | sudo tee /etc/apt/trusted.gpg.d/kitware.gpg >/dev/null
 # sudo apt-add-repository 'deb https://apt.kitware.com/ubuntu/ focal main'
```

### Comparing `coindicator-2.1.7/requirements.txt` & `coindicator-2.1.8/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -8,16 +8,14 @@
     # via
     #   coindicator (setup.py)
     #   requests
 chardet==3.0.4
     # via coindicator (setup.py)
 charset-normalizer==3.1.0
     # via requests
-dbus-python==1.3.2
-    # via coindicator (setup.py)
 idna==2.10
     # via
     #   coindicator (setup.py)
     #   requests
 notify2==0.3.1
     # via coindicator (setup.py)
 pycairo==1.21.0
```

### Comparing `coindicator-2.1.7/setup.cfg` & `coindicator-2.1.8/setup.cfg`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/setup.py` & `coindicator-2.1.8/setup.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/src/coin/about.py` & `coindicator-2.1.8/src/coin/about.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/src/coin/alarm.py` & `coindicator-2.1.8/src/coin/alarm.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/src/coin/asset_selection.py` & `coindicator-2.1.8/src/coin/asset_selection.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/src/coin/coin.py` & `coindicator-2.1.8/src/coin/coin.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,14 @@
 import importlib
 import logging
 import signal
 from pathlib import Path
 
 import notify2
 import yaml
-from dbus.mainloop.glib import DBusGMainLoop
 from gi.repository import Gtk
 
 from coin.about import AboutWindow
 from coin.downloader import AsyncDownloadService, DownloadService
 from coin.indicator import Indicator
 from coin.plugin_selection import PluginSelectionWindow
 from coin.coingecko_client import CoinGeckoClient
@@ -194,22 +193,14 @@
         )
         self.main_item.set_status(AppIndicator.IndicatorStatus.ACTIVE)
         self.main_item.set_ordering_index(0)
         self.main_item.set_menu(self._menu())
 
     def _start_gui(self):
         signal.signal(signal.SIGINT, Gtk.main_quit)  # ctrl+c exit
-        # DBusGMainLoop(set_as_default=True)
-        # bus = dbus.SystemBus()
-        # bus.add_signal_receiver(
-        #     self.handle_resume,
-        #     None,
-        #     "org.freedesktop.login1.Manager",
-        #     "org.freedesktop.login1",
-        # )
         Gtk.main()
 
     # Program main menu
     def _menu(self):
         menu = Gtk.Menu()
 
         self.add_item = Gtk.MenuItem.new_with_label("Add Ticker")
```

### Comparing `coindicator-2.1.7/src/coin/coingecko_client.py` & `coindicator-2.1.8/src/coin/coingecko_client.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/src/coin/config.py` & `coindicator-2.1.8/src/coin/config.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/src/coin/config.yaml` & `coindicator-2.1.8/src/coin/config.yaml`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/src/coin/downloader.py` & `coindicator-2.1.8/src/coin/downloader.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/src/coin/error.py` & `coindicator-2.1.8/src/coin/error.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/src/coin/exchange.py` & `coindicator-2.1.8/src/coin/exchange.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,14 +32,22 @@
     "ask": "Ask",
     "vol": "Vol",
     "first": "First",
     "avg": "Avg",
 }
 
 
+class classproperty:
+    def __init__(self, func):
+        self.fget = func
+
+    def __get__(self, _instance, owner):
+        return self.fget(owner)
+
+
 class Exchange(abc.ABC):
     active = True
     name = "Must be overwritten"
     code = "Must be overwritten"
     default_label = "Must be overwritten"
 
     def __init__(self, indicator=None):
@@ -50,20 +58,22 @@
         self.started = False
         self.asset_pair = {}
         self.config = Config()
 
     ##
     # Abstract methods to be overwritten by the child classes
     #
+    @classmethod
     @abc.abstractmethod
-    def _get_discovery_url(self):
+    def _get_discovery_url(cls):
         pass
 
+    @classmethod
     @abc.abstractmethod
-    def _parse_discovery(self, data):
+    def _parse_discovery(cls, data):
         pass
 
     @abc.abstractmethod
     def _get_ticker_url(self):
         pass
 
     @abc.abstractmethod
@@ -121,106 +131,112 @@
         if not self.asset_pair:
             logging.warning(
                 "User.conf specifies unavailable asset pair, trying default. \
                 Run Asset Discovery again."
             )
             self.asset_pair = {}
 
-    def find_asset_pair_by_code(self, code):
-        for ap in self.asset_pairs:
+    @classmethod
+    def find_asset_pair_by_code(cls, code):
+        for ap in cls.asset_pairs:
             if ap.get("pair") == code:
                 return ap
 
         return {}
 
-    def find_asset_pair(self, quote, base):
-        for ap in self.asset_pairs:
+    @classmethod
+    def find_asset_pair(cls, quote, base):
+        for ap in cls.asset_pairs:
             if ap.get("quote") == quote and ap.get("base") == base:
                 return ap
 
         return {}
 
-    @property
-    def datafile(self):
+    @classproperty
+    def datafile(cls):
         config = Config()
-        return config["user_data_dir"] / f"cache/{self.code}.cache"
+        return config["user_data_dir"] / f"cache/{cls.code}.cache"
 
     ##
     # Loads asset pairs from the config files or,
     # failing that, from the hard-coded lines
     #
-    @property
-    def asset_pairs(self):
+    @classproperty
+    def asset_pairs(cls):
         try:
-            with open(self.datafile, "rb") as stream:
+            with open(cls.datafile, "rb") as stream:
                 asset_pairs = pickle.load(stream)
                 return asset_pairs if asset_pairs else []
 
         except IOError:
             # Faulty data file, return empty array
             return []
 
     ##
     # Saves asset pairs to disk
     #
-    def store_asset_pairs(self, asset_pairs):
+    @classmethod
+    def store_asset_pairs(cls, asset_pairs):
         try:
-            with open(self.datafile, "wb") as stream:
+            with open(cls.datafile, "wb") as stream:
                 pickle.dump(asset_pairs, stream)
         except IOError:
-            logging.error("Could not write to data file %s" % self.datafile)
+            logging.error("Could not write to data file %s" % cls.datafile)
 
     ##
     # Discovers assets from the exchange's API url retrieved
     # through the instance-specific method _get_discovery_url()
     #
-    def discover_assets(self, downloader, callback):
-        if self._get_discovery_url() is None:
-            self.store_asset_pairs(self._parse_discovery(None))
+    @classmethod
+    def discover_assets(cls, downloader, callback):
+        if cls._get_discovery_url() is None:
+            cls.store_asset_pairs(cls._parse_discovery(None))
         else:
-            command = DownloadCommand(self._get_discovery_url(), callback)
-            downloader.execute(command, self._handle_discovery_result)
+            command = DownloadCommand(cls._get_discovery_url(), callback)
+            downloader.execute(command, cls._handle_discovery_result)
 
     ##
     # Deals with the result from the discovery HTTP request
     # Should probably be merged with _handle_result() later
     #
-    def _handle_discovery_result(self, command):
+    @classmethod
+    def _handle_discovery_result(cls, command):
         logging.debug("Response from %s: %s" % (command.url, command.error))
 
         if command.error:
-            self._handle_discovery_error(
-                f"{self.name}: API server {command.url}\
+            cls._handle_discovery_error(
+                f"{cls.name}: API server {command.url}\
                      returned an error: {command.error}"
             )
 
         if command.response:
             data = command.response
 
             if data.status_code in [301, 302]:
                 # hooks will be called even when requests is following a redirect
                 # but we don't want to print any error messages here
                 return
 
             if data.status_code != 200:
-                self._handle_discovery_error(
+                cls._handle_discovery_error(
                     f"API server {command.url} returned \
                         an error: {str(data.status_code)}"
                 )
 
             try:
                 result = data.json()
-                asset_pairs = self._parse_discovery(result)
-                self.store_asset_pairs(asset_pairs)
+                asset_pairs = cls._parse_discovery(result)
+                cls.store_asset_pairs(asset_pairs)
             except Exception as e:
-                self._handle_discovery_error(str(e))
+                cls._handle_discovery_error(str(e))
 
         command.callback()  # update the asset menus of all instances
 
-    def _handle_discovery_error(self, msg):
+    @classmethod
+    def _handle_discovery_error(cls, msg):
         logging.warn("Asset Discovery: %s" % msg)
 
     ##
     # Start exchange
     #
     def start(self, error_refresh=None):
         if not self.started:
```

### Comparing `coindicator-2.1.7/src/coin/exchanges/binance.py` & `coindicator-2.1.8/src/coin/exchanges/cexio.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,63 +1,57 @@
-# Binance
-# https://github.com/binance-exchange/binance-official-api-docs/blob/master/rest-api.md
-# By Lari Taskula <lari@taskula.fi>
+# CEX.io
+# https://cex.io/rest-api
+# By Sander Van de Moortel <sander.vandemoortel@gmail.com>
 
 from coin.exchange import Exchange
 
 
-class Binance(Exchange):
-    name = "Binance"
-    code = "binance"
+class Cexio(Exchange):
+    name = "CEX.io"
+    code = "cexio"
 
-    ticker = "https://www.binance.com/api/v1/ticker/24hr"
-    discovery = "https://www.binance.com/api/v1/exchangeInfo"
+    ticker = "https://cex.io/api/ticker"
+    discovery = "https://cex.io/api/currency_limits"
 
     default_label = "cur"
 
-    def _get_discovery_url(self):
-        return self.discovery
+    @classmethod
+    def _get_discovery_url(cls):
+        return cls.discovery
 
     def _get_ticker_url(self):
-        return self.ticker + "?symbol=" + self.pair
+        return self.ticker + "/" + self.pair  # base/quote
 
     @staticmethod
     def _parse_discovery(result):
         asset_pairs = []
-        assets = result.get("symbols")
-        for asset in assets:
-            base = asset.get("baseAsset")
-            quote = asset.get("quoteAsset")
-
-            names = {"XZC": "ZEC", "BCC": "BCH", "IOTA": "IOT"}
-            if base in names:
-                base = names[base]
-
-            if quote in names:
-                quote = names[quote]
+        data = result.get("data")
+        for asset in data.get("pairs"):
+            base = asset.get("symbol1")
+            quote = asset.get("symbol2")
 
             asset_pair = {
-                "pair": asset.get("symbol"),
+                "pair": base + "/" + quote,
                 "base": base,
                 "quote": quote,
                 "name": base + " to " + quote,
                 "currency": quote.lower(),
                 "volumecurrency": base,
             }
 
             asset_pairs.append(asset_pair)
 
         return asset_pairs
 
     def _parse_ticker(self, asset):
-        cur = asset.get("lastPrice")
-        bid = asset.get("bidPrice")
-        high = asset.get("highPrice")
-        low = asset.get("lowPrice")
-        ask = asset.get("askPrice")
+        cur = asset.get("last")
+        bid = asset.get("bid")
+        high = asset.get("high")
+        low = asset.get("low")
+        ask = asset.get("ask")
         vol = asset.get("volume")
 
         return {
             "cur": cur,
             "bid": bid,
             "high": high,
             "low": low,
```

### Comparing `coindicator-2.1.7/src/coin/exchanges/bitfinex.py` & `coindicator-2.1.8/src/coin/exchanges/bitfinex.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,16 +10,17 @@
     code = "bitfinex"
 
     ticker = "https://api.bitfinex.com/v2/ticker/"
     discovery = "https://api.bitfinex.com/v1/symbols"
 
     default_label = "cur"
 
-    def _get_discovery_url(self):
-        return self.discovery
+    @classmethod
+    def _get_discovery_url(cls):
+        return cls.discovery
 
     def _get_ticker_url(self):
         return self.ticker + self.pair
 
     @staticmethod
     def _parse_discovery(result):
         asset_pairs = []
```

### Comparing `coindicator-2.1.7/src/coin/exchanges/bitkub.py` & `coindicator-2.1.8/src/coin/exchanges/bitkub.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,17 @@
     code = "bitkub"
 
     ticker = "https://api.bitkub.com/api/market/ticker"
     discovery = "https://api.bitkub.com/api/market/symbols"
 
     default_label = "cur"
 
-    def _get_discovery_url(self):
-        return self.discovery
+    @classmethod
+    def _get_discovery_url(cls):
+        return cls.discovery
 
     def _get_ticker_url(self):
         return self.ticker + "?sym=" + self.pair
 
     @staticmethod
     def _parse_discovery(result):
         asset_pairs = []
```

### Comparing `coindicator-2.1.7/src/coin/exchanges/bitstamp.py` & `coindicator-2.1.8/src/coin/exchanges/bitstamp.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,17 @@
     code = "bitstamp"
 
     ticker = "https://www.bitstamp.net/api/v2/ticker/"
     discovery = "https://www.bitstamp.net/api/v2/trading-pairs-info/"
 
     default_label = "cur"
 
-    def _get_discovery_url(self):
-        return self.discovery
+    @classmethod
+    def _get_discovery_url(cls):
+        return cls.discovery
 
     def _get_ticker_url(self):
         return self.ticker + self.pair
 
     @staticmethod
     def _parse_discovery(result):
         asset_pairs = []
```

### Comparing `coindicator-2.1.7/src/coin/exchanges/bittrex.py` & `coindicator-2.1.8/src/coin/exchanges/bittrex.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,17 @@
     code = "bittrex"
 
     ticker = "https://api.bittrex.com/v3/markets/{}/ticker"
     discovery = "https://api.bittrex.com/v3/markets"
 
     default_label = "ask"
 
-    def _get_discovery_url(self):
-        return self.discovery
+    @classmethod
+    def _get_discovery_url(cls):
+        return cls.discovery
 
     def _get_ticker_url(self):
         return self.ticker.format(self.pair)
 
     @staticmethod
     def _parse_discovery(result):
         asset_pairs = []
```

### Comparing `coindicator-2.1.7/src/coin/exchanges/cexio.py` & `coindicator-2.1.8/src/coin/exchanges/gemini.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,59 +1,60 @@
-# CEX.io
-# https://cex.io/rest-api
-# By Sander Van de Moortel <sander.vandemoortel@gmail.com>
+# Gemini
+# https://docs.gemini.com/rest-api/
+# By Rick Ramstetter <rick@anteaterllc.com>
 
 from coin.exchange import Exchange
 
 
-class Cexio(Exchange):
-    name = "CEX.io"
-    code = "cexio"
+class Gemini(Exchange):
+    name = "Gemini"
+    code = "gemini"
 
-    ticker = "https://cex.io/api/ticker"
-    discovery = "https://cex.io/api/currency_limits"
+    ticker = "https://api.gemini.com/v1/pubticker/"
+    discovery = "https://api.gemini.com/v1/symbols"
 
     default_label = "cur"
 
-    def _get_discovery_url(self):
-        return self.discovery
+    @classmethod
+    def _get_discovery_url(cls):
+        return cls.discovery
 
     def _get_ticker_url(self):
-        return self.ticker + "/" + self.pair  # base/quote
+        return self.ticker + self.pair
 
     @staticmethod
     def _parse_discovery(result):
         asset_pairs = []
-        data = result.get("data")
-        for asset in data.get("pairs"):
-            base = asset.get("symbol1")
-            quote = asset.get("symbol2")
+        for asset in result:
+            base = asset[0:3].upper()
+            quote = asset[-3:].upper()
 
             asset_pair = {
-                "pair": base + "/" + quote,
+                "pair": asset,
                 "base": base,
                 "quote": quote,
                 "name": base + " to " + quote,
                 "currency": quote.lower(),
                 "volumecurrency": base,
             }
 
             asset_pairs.append(asset_pair)
 
         return asset_pairs
 
     def _parse_ticker(self, asset):
+        volumelabel = [
+            item for item in self.config["asset_pairs"] if item["pair"] == self.pair
+        ][0]["volumelabel"]
         cur = asset.get("last")
         bid = asset.get("bid")
-        high = asset.get("high")
-        low = asset.get("low")
         ask = asset.get("ask")
-        vol = asset.get("volume")
+        vol = asset.get("volume").get(volumelabel)
 
         return {
             "cur": cur,
             "bid": bid,
-            "high": high,
-            "low": low,
+            "high": None,
+            "low": None,
             "ask": ask,
             "vol": vol,
         }
```

### Comparing `coindicator-2.1.7/src/coin/exchanges/hitbtc.py` & `coindicator-2.1.8/src/coin/exchanges/hitbtc.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,17 @@
     code = "hitbtc"
 
     ticker = "https://api.hitbtc.com/api/1/public/"
     discovery = "http://api.hitbtc.com/api/1/public/symbols"
 
     default_label = "cur"
 
-    def _get_discovery_url(self):
-        return self.discovery
+    @classmethod
+    def _get_discovery_url(cls):
+        return cls.discovery
 
     def _get_ticker_url(self):
         return self.ticker + self.pair + "/ticker"
 
     @staticmethod
     def _parse_discovery(result):
         asset_pairs = []
```

### Comparing `coindicator-2.1.7/src/coin/exchanges/kraken.py` & `coindicator-2.1.8/src/coin/exchanges/kraken.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,17 @@
     code = "kraken"
 
     ticker = "https://api.kraken.com/0/public/Ticker"
     discovery = "https://api.kraken.com/0/public/AssetPairs"
 
     default_label = "cur"
 
-    def _get_discovery_url(self):
-        return self.discovery
+    @classmethod
+    def _get_discovery_url(cls):
+        return cls.discovery
 
     def _get_ticker_url(self):
         return self.ticker + "?pair=" + self.pair
 
     @staticmethod
     def _parse_discovery(result):
         asset_pairs = []
```

### Comparing `coindicator-2.1.7/src/coin/exchanges/okcoin.py` & `coindicator-2.1.8/src/coin/exchanges/okcoin.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,22 +10,23 @@
     code = "okcoin"
 
     ticker = "https://www.okcoin.cn/api/v1/ticker.do"
     discovery = False  # no discovery here
 
     default_label = "cur"
 
-    def _get_discovery_url(self):
+    @classmethod
+    def _get_discovery_url(cls):
         return None
 
     def _get_ticker_url(self):
         return self.ticker + "?symbol=" + self.pair  # base/quote
 
     @staticmethod
-    def _parse_discovery(_):
+    def _parse_discovery(result):
         return [
             {"pair": "btc_cny", "name": "BTC to CNY", "currency": CURRENCY["cny"]},
             {"pair": "ltc_cny", "name": "LTC to CNY", "currency": CURRENCY["cny"]},
             {"pair": "eth_cny", "name": "ETH to CNY", "currency": CURRENCY["cny"]},
         ]
 
     def _parse_ticker(self, asset):
```

### Comparing `coindicator-2.1.7/src/coin/exchanges/poloniex.py` & `coindicator-2.1.8/src/coin/exchanges/poloniex.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,16 +10,17 @@
     code = "poloniex"
 
     ticker = "https://poloniex.com/public?command=returnTicker"
     discovery = "https://poloniex.com/public?command=returnTicker"
 
     default_label = "cur"
 
-    def _get_discovery_url(self):
-        return self.discovery
+    @classmethod
+    def _get_discovery_url(cls):
+        return cls.discovery
 
     def _get_ticker_url(self):
         return self.ticker
 
     @staticmethod
     def _parse_discovery(result):
         asset_pairs = []
```

### Comparing `coindicator-2.1.7/src/coin/exchanges/unocoin.py` & `coindicator-2.1.8/src/coin/exchanges/unocoin.py`

 * *Files 3% similar despite different names*

```diff
@@ -10,16 +10,17 @@
     code = "unocoin"
 
     ticker = "https://api.unocoin.com/api/trades/{}/all"
     discovery = "https://api.unocoin.com/api/trades/all/all"
 
     default_label = "avg"
 
-    def _get_discovery_url(self):
-        return self.discovery
+    @classmethod
+    def _get_discovery_url(cls):
+        return cls.discovery
 
     def _get_ticker_url(self):
         return self.ticker.format(self.asset_pair.get("base").lower())
 
     @staticmethod
     def _parse_discovery(result):
         asset_pairs = []
```

### Comparing `coindicator-2.1.7/src/coin/indicator.py` & `coindicator-2.1.8/src/coin/indicator.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/src/coin/plugin_selection.py` & `coindicator-2.1.8/src/coin/plugin_selection.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/src/coin/resources/ca-ching.wav` & `coindicator-2.1.8/src/coin/resources/ca-ching.wav`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/src/coin/resources/icon.png` & `coindicator-2.1.8/src/coin/resources/icon.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/src/coin/resources/icon_32px.png` & `coindicator-2.1.8/src/coin/resources/icon_32px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/src/coin/resources/icon_48px.png` & `coindicator-2.1.8/src/coin/resources/icon_48px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/src/coin/resources/icon_64px.png` & `coindicator-2.1.8/src/coin/resources/icon_64px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/src/coin/resources/loading.png` & `coindicator-2.1.8/src/coin/resources/loading.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/src/coin/resources/logo_124px.png` & `coindicator-2.1.8/src/coin/resources/logo_124px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/src/coin/resources/logo_124pxs.png` & `coindicator-2.1.8/src/coin/resources/logo_124pxs.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/src/coin/resources/logo_248px.png` & `coindicator-2.1.8/src/coin/resources/logo_248px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.7/src/coindicator.egg-info/PKG-INFO` & `coindicator-2.1.8/src/coindicator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coindicator
-Version: 2.1.7
+Version: 2.1.8
 Summary: Coinprice Indicator
 Home-page: https://github.com/bluppfisk/coindicator/
 Author: Sander Van de Moortel
 Author-email: sander.vandemoortel@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/bluppfisk/coindicator/
 Platform: Linux
```

### Comparing `coindicator-2.1.7/src/coindicator.egg-info/SOURCES.txt` & `coindicator-2.1.8/src/coindicator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

