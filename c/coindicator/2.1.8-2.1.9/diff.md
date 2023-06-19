# Comparing `tmp/coindicator-2.1.8.tar.gz` & `tmp/coindicator-2.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "coindicator-2.1.8.tar", last modified: Mon Jun 19 12:08:52 2023, max compression
+gzip compressed data, was "coindicator-2.1.9.tar", last modified: Mon Jun 19 12:28:40 2023, max compression
```

## Comparing `coindicator-2.1.8.tar` & `coindicator-2.1.9.tar`

### file list

```diff
@@ -1,62 +1,62 @@
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:08:52.308895 coindicator-2.1.8/
--rw-rw-r--   0 sander    (1000) sander    (1000)       83 2023-06-16 13:19:52.000000 coindicator-2.1.8/.gitignore
--rw-rw-r--   0 sander    (1000) sander    (1000)      899 2022-10-30 19:56:43.000000 coindicator-2.1.8/.pre-commit-config.yaml
--rw-r--r--   0 sander    (1000) sander    (1000)     1106 2020-04-16 00:57:46.000000 coindicator-2.1.8/LICENSE
--rw-rw-r--   0 sander    (1000) sander    (1000)       29 2023-06-16 13:19:52.000000 coindicator-2.1.8/MANIFEST.in
--rw-rw-r--   0 sander    (1000) sander    (1000)     4402 2023-06-19 12:08:52.308895 coindicator-2.1.8/PKG-INFO
--rw-rw-r--   0 sander    (1000) sander    (1000)     3891 2023-06-19 12:03:38.000000 coindicator-2.1.8/README.md
--rw-rw-r--   0 sander    (1000) sander    (1000)      369 2023-06-16 13:19:52.000000 coindicator-2.1.8/coindicator.desktop
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:08:52.292895 coindicator-2.1.8/img/
--rw-rw-r--   0 sander    (1000) sander    (1000)    27147 2022-10-30 19:56:43.000000 coindicator-2.1.8/img/gitcoin.png
--rw-rw-r--   0 sander    (1000) sander    (1000)   172307 2022-10-30 19:56:43.000000 coindicator-2.1.8/img/screenshot.png
--rwxrwxr-x   0 sander    (1000) sander    (1000)     1559 2023-06-19 12:08:13.000000 coindicator-2.1.8/install.sh
--rw-rw-r--   0 sander    (1000) sander    (1000)      294 2023-06-16 13:19:52.000000 coindicator-2.1.8/pyproject.toml
--rw-rw-r--   0 sander    (1000) sander    (1000)      742 2023-06-19 12:07:56.000000 coindicator-2.1.8/requirements.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)     1202 2023-06-19 12:08:52.308895 coindicator-2.1.8/setup.cfg
--rw-rw-r--   0 sander    (1000) sander    (1000)      521 2023-06-16 13:19:52.000000 coindicator-2.1.8/setup.py
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:08:52.284895 coindicator-2.1.8/src/
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:08:52.296895 coindicator-2.1.8/src/coin/
--rw-rw-r--   0 sander    (1000) sander    (1000)        0 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/__init__.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1537 2023-06-16 13:19:52.000000 coindicator-2.1.8/src/coin/about.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     6537 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/alarm.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     5794 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/asset_selection.py
--rwxrwxr-x   0 sander    (1000) sander    (1000)    12303 2023-06-19 12:08:02.000000 coindicator-2.1.8/src/coin/coin.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1751 2023-06-16 13:19:52.000000 coindicator-2.1.8/src/coin/coingecko_client.py
--rw-rw-r--   0 sander    (1000) sander    (1000)      609 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/config.py
--rw-rw-r--   0 sander    (1000) sander    (1000)      977 2023-06-16 13:19:52.000000 coindicator-2.1.8/src/coin/config.yaml
--rw-rw-r--   0 sander    (1000) sander    (1000)     1422 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/downloader.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1177 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/error.py
--rw-rw-r--   0 sander    (1000) sander    (1000)    10640 2023-06-19 12:08:35.000000 coindicator-2.1.8/src/coin/exchange.py
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:08:52.300895 coindicator-2.1.8/src/coin/exchanges/
--rw-rw-r--   0 sander    (1000) sander    (1000)     1761 2023-06-19 12:04:55.000000 coindicator-2.1.8/src/coin/exchanges/binance.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1569 2023-06-19 12:04:53.000000 coindicator-2.1.8/src/coin/exchanges/bitfinex.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1824 2023-06-19 12:04:53.000000 coindicator-2.1.8/src/coin/exchanges/bitkub.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1483 2023-06-19 12:04:53.000000 coindicator-2.1.8/src/coin/exchanges/bitstamp.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     2031 2023-06-19 12:03:08.000000 coindicator-2.1.8/src/coin/exchanges/bittrex.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1473 2023-06-19 12:03:08.000000 coindicator-2.1.8/src/coin/exchanges/cexio.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1489 2023-06-19 12:04:53.000000 coindicator-2.1.8/src/coin/exchanges/gemini.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1708 2023-06-19 12:04:53.000000 coindicator-2.1.8/src/coin/exchanges/hitbtc.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     2073 2023-06-19 12:04:53.000000 coindicator-2.1.8/src/coin/exchanges/kraken.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1273 2023-06-19 12:05:15.000000 coindicator-2.1.8/src/coin/exchanges/okcoin.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1547 2023-06-19 12:03:08.000000 coindicator-2.1.8/src/coin/exchanges/poloniex.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     1271 2023-06-19 12:04:53.000000 coindicator-2.1.8/src/coin/exchanges/unocoin.py
--rw-rw-r--   0 sander    (1000) sander    (1000)    10370 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/indicator.py
--rw-rw-r--   0 sander    (1000) sander    (1000)     2608 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/plugin_selection.py
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:08:52.304895 coindicator-2.1.8/src/coin/resources/
--rw-rw-r--   0 sander    (1000) sander    (1000)   294232 2023-06-16 13:19:52.000000 coindicator-2.1.8/src/coin/resources/ca-ching.wav
--rw-rw-r--   0 sander    (1000) sander    (1000)     5060 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/resources/icon.png
--rw-rw-r--   0 sander    (1000) sander    (1000)      983 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/resources/icon_32px.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     1440 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/resources/icon_48px.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     1673 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/resources/icon_64px.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     1889 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/resources/loading.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     4619 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/resources/logo_124px.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     7329 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/resources/logo_124pxs.png
--rw-rw-r--   0 sander    (1000) sander    (1000)     6508 2022-10-30 19:56:43.000000 coindicator-2.1.8/src/coin/resources/logo_248px.png
-drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:08:52.308895 coindicator-2.1.8/src/coindicator.egg-info/
--rw-rw-r--   0 sander    (1000) sander    (1000)     4402 2023-06-19 12:08:52.000000 coindicator-2.1.8/src/coindicator.egg-info/PKG-INFO
--rw-rw-r--   0 sander    (1000) sander    (1000)     1388 2023-06-19 12:08:52.000000 coindicator-2.1.8/src/coindicator.egg-info/SOURCES.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-19 12:08:52.000000 coindicator-2.1.8/src/coindicator.egg-info/dependency_links.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)       47 2023-06-19 12:08:52.000000 coindicator-2.1.8/src/coindicator.egg-info/entry_points.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-16 11:50:35.000000 coindicator-2.1.8/src/coindicator.egg-info/not-zip-safe
--rw-rw-r--   0 sander    (1000) sander    (1000)      227 2023-06-19 12:08:52.000000 coindicator-2.1.8/src/coindicator.egg-info/requires.txt
--rw-rw-r--   0 sander    (1000) sander    (1000)        5 2023-06-19 12:08:52.000000 coindicator-2.1.8/src/coindicator.egg-info/top_level.txt
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:28:40.740574 coindicator-2.1.9/
+-rw-rw-r--   0 sander    (1000) sander    (1000)       83 2023-06-16 13:19:52.000000 coindicator-2.1.9/.gitignore
+-rw-rw-r--   0 sander    (1000) sander    (1000)      899 2022-10-30 19:56:43.000000 coindicator-2.1.9/.pre-commit-config.yaml
+-rw-r--r--   0 sander    (1000) sander    (1000)     1106 2020-04-16 00:57:46.000000 coindicator-2.1.9/LICENSE
+-rw-rw-r--   0 sander    (1000) sander    (1000)       29 2023-06-16 13:19:52.000000 coindicator-2.1.9/MANIFEST.in
+-rw-rw-r--   0 sander    (1000) sander    (1000)     4402 2023-06-19 12:28:40.740574 coindicator-2.1.9/PKG-INFO
+-rw-rw-r--   0 sander    (1000) sander    (1000)     3891 2023-06-19 12:03:38.000000 coindicator-2.1.9/README.md
+-rw-rw-r--   0 sander    (1000) sander    (1000)      369 2023-06-16 13:19:52.000000 coindicator-2.1.9/coindicator.desktop
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:28:40.728574 coindicator-2.1.9/img/
+-rw-rw-r--   0 sander    (1000) sander    (1000)    27147 2022-10-30 19:56:43.000000 coindicator-2.1.9/img/gitcoin.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)   172307 2022-10-30 19:56:43.000000 coindicator-2.1.9/img/screenshot.png
+-rwxrwxr-x   0 sander    (1000) sander    (1000)     1542 2023-06-19 12:18:20.000000 coindicator-2.1.9/install.sh
+-rw-rw-r--   0 sander    (1000) sander    (1000)      294 2023-06-16 13:19:52.000000 coindicator-2.1.9/pyproject.toml
+-rw-rw-r--   0 sander    (1000) sander    (1000)      667 2023-06-19 12:20:03.000000 coindicator-2.1.9/requirements.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1165 2023-06-19 12:28:40.744574 coindicator-2.1.9/setup.cfg
+-rw-rw-r--   0 sander    (1000) sander    (1000)      521 2023-06-16 13:19:52.000000 coindicator-2.1.9/setup.py
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:28:40.720574 coindicator-2.1.9/src/
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:28:40.732574 coindicator-2.1.9/src/coin/
+-rw-rw-r--   0 sander    (1000) sander    (1000)        0 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/__init__.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1537 2023-06-16 13:19:52.000000 coindicator-2.1.9/src/coin/about.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     6527 2023-06-19 12:22:07.000000 coindicator-2.1.9/src/coin/alarm.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     5794 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/asset_selection.py
+-rwxrwxr-x   0 sander    (1000) sander    (1000)    12085 2023-06-19 12:22:14.000000 coindicator-2.1.9/src/coin/coin.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1751 2023-06-16 13:19:52.000000 coindicator-2.1.9/src/coin/coingecko_client.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)      609 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/config.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)      977 2023-06-16 13:19:52.000000 coindicator-2.1.9/src/coin/config.yaml
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1422 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/downloader.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1177 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/error.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)    10640 2023-06-19 12:08:35.000000 coindicator-2.1.9/src/coin/exchange.py
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:28:40.736574 coindicator-2.1.9/src/coin/exchanges/
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1761 2023-06-19 12:04:55.000000 coindicator-2.1.9/src/coin/exchanges/binance.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1569 2023-06-19 12:04:53.000000 coindicator-2.1.9/src/coin/exchanges/bitfinex.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1824 2023-06-19 12:04:53.000000 coindicator-2.1.9/src/coin/exchanges/bitkub.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1483 2023-06-19 12:04:53.000000 coindicator-2.1.9/src/coin/exchanges/bitstamp.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2031 2023-06-19 12:03:08.000000 coindicator-2.1.9/src/coin/exchanges/bittrex.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1473 2023-06-19 12:03:08.000000 coindicator-2.1.9/src/coin/exchanges/cexio.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1489 2023-06-19 12:04:53.000000 coindicator-2.1.9/src/coin/exchanges/gemini.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1708 2023-06-19 12:04:53.000000 coindicator-2.1.9/src/coin/exchanges/hitbtc.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2073 2023-06-19 12:04:53.000000 coindicator-2.1.9/src/coin/exchanges/kraken.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1273 2023-06-19 12:05:15.000000 coindicator-2.1.9/src/coin/exchanges/okcoin.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1547 2023-06-19 12:03:08.000000 coindicator-2.1.9/src/coin/exchanges/poloniex.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1271 2023-06-19 12:04:53.000000 coindicator-2.1.9/src/coin/exchanges/unocoin.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)    10370 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/indicator.py
+-rw-rw-r--   0 sander    (1000) sander    (1000)     2528 2023-06-19 12:22:38.000000 coindicator-2.1.9/src/coin/plugin_selection.py
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:28:40.740574 coindicator-2.1.9/src/coin/resources/
+-rw-rw-r--   0 sander    (1000) sander    (1000)   294232 2023-06-16 13:19:52.000000 coindicator-2.1.9/src/coin/resources/ca-ching.wav
+-rw-rw-r--   0 sander    (1000) sander    (1000)     5060 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/resources/icon.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)      983 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/resources/icon_32px.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1440 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/resources/icon_48px.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1673 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/resources/icon_64px.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1889 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/resources/loading.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     4619 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/resources/logo_124px.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     7329 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/resources/logo_124pxs.png
+-rw-rw-r--   0 sander    (1000) sander    (1000)     6508 2022-10-30 19:56:43.000000 coindicator-2.1.9/src/coin/resources/logo_248px.png
+drwxrwxr-x   0 sander    (1000) sander    (1000)        0 2023-06-19 12:28:40.740574 coindicator-2.1.9/src/coindicator.egg-info/
+-rw-rw-r--   0 sander    (1000) sander    (1000)     4402 2023-06-19 12:28:40.000000 coindicator-2.1.9/src/coindicator.egg-info/PKG-INFO
+-rw-rw-r--   0 sander    (1000) sander    (1000)     1388 2023-06-19 12:28:40.000000 coindicator-2.1.9/src/coindicator.egg-info/SOURCES.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-19 12:28:40.000000 coindicator-2.1.9/src/coindicator.egg-info/dependency_links.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)       47 2023-06-19 12:28:40.000000 coindicator-2.1.9/src/coindicator.egg-info/entry_points.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)        1 2023-06-16 11:50:35.000000 coindicator-2.1.9/src/coindicator.egg-info/not-zip-safe
+-rw-rw-r--   0 sander    (1000) sander    (1000)      192 2023-06-19 12:28:40.000000 coindicator-2.1.9/src/coindicator.egg-info/requires.txt
+-rw-rw-r--   0 sander    (1000) sander    (1000)        5 2023-06-19 12:28:40.000000 coindicator-2.1.9/src/coindicator.egg-info/top_level.txt
```

### Comparing `coindicator-2.1.8/.pre-commit-config.yaml` & `coindicator-2.1.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/LICENSE` & `coindicator-2.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/PKG-INFO` & `coindicator-2.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coindicator
-Version: 2.1.8
+Version: 2.1.9
 Summary: Coinprice Indicator
 Home-page: https://github.com/bluppfisk/coindicator/
 Author: Sander Van de Moortel
 Author-email: sander.vandemoortel@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/bluppfisk/coindicator/
 Platform: Linux
```

### Comparing `coindicator-2.1.8/README.md` & `coindicator-2.1.9/README.md`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/img/gitcoin.png` & `coindicator-2.1.9/img/gitcoin.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/img/screenshot.png` & `coindicator-2.1.9/img/screenshot.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/install.sh` & `coindicator-2.1.9/install.sh`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
         exit 1
 fi
 
 args=("$@")
 
 echo Installing to ${args[0]}
 
-sudo apt-get install python3-venv python3-setuptools-scm python3-wheel python3-gi python3-gi-cairo gir1.2-gtk-3.0 gir1.2-appindicator3-0.1 python3-pip patchelf -y
+sudo apt-get install python3-venv python3-setuptools-scm python3-wheel python3-gi gir1.2-gtk-3.0 gir1.2-appindicator3-0.1 python3-pip patchelf -y
 
 # some users report requiring libgirepository1.0-dev libdbus-1-dev, libcairo2-dev, build-essential
 # some report having to install a newer version of cmake
 
 # sudo apt purge --auto-remove cmake
 # wget -O - https://apt.kitware.com/keys/kitware-archive-latest.asc 2>/dev/null | gpg --dearmor - | sudo tee /etc/apt/trusted.gpg.d/kitware.gpg >/dev/null
 # sudo apt-add-repository 'deb https://apt.kitware.com/ubuntu/ focal main'
```

### Comparing `coindicator-2.1.8/requirements.txt` & `coindicator-2.1.9/requirements.txt`

 * *Files 6% similar despite different names*

```diff
@@ -14,18 +14,14 @@
     # via requests
 idna==2.10
     # via
     #   coindicator (setup.py)
     #   requests
 notify2==0.3.1
     # via coindicator (setup.py)
-pycairo==1.21.0
-    # via
-    #   coindicator (setup.py)
-    #   pygobject
 pygame==2.1.3
     # via coindicator (setup.py)
 pygobject==3.42.2
     # via coindicator (setup.py)
 pyyaml==6.0
     # via coindicator (setup.py)
 requests==2.31.0
```

### Comparing `coindicator-2.1.8/setup.cfg` & `coindicator-2.1.9/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -28,16 +28,14 @@
 	idna~=2.7
 	notify2~=0.3.1
 	PyYAML>=4.2b1
 	requests~=2.20
 	urllib3~=1.26.5
 	pygame~=2.1.2
 	PyGObject~=3.42.2
-	pycairo~=1.21.0
-	dbus-python~=1.3.2
 
 [options.packages.find]
 where = 
 	src
 
 [options.package_data]
 * =
```

### Comparing `coindicator-2.1.8/setup.py` & `coindicator-2.1.9/setup.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/about.py` & `coindicator-2.1.9/src/coin/about.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/alarm.py` & `coindicator-2.1.9/src/coin/alarm.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 # Lets the user set an alert for a certain price point
 
-import gi
 import notify2
 import pygame
 
 from coin.config import Config
 
 from gi.repository import Gdk, GdkPixbuf, Gtk
 from gi.repository.Gdk import Color
```

### Comparing `coindicator-2.1.8/src/coin/asset_selection.py` & `coindicator-2.1.9/src/coin/asset_selection.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/coin.py` & `coindicator-2.1.9/src/coin/coin.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,20 +302,14 @@
             )
             n.set_urgency(1)
             n.timeout = 2000
             n.show()
 
         self.main_item.set_icon_full(str(self.icon), "App icon")
 
-    # Handle system resume by refreshing all tickers
-    def handle_resume(self, sleeping, *args):
-        if not sleeping:
-            for instance in self.instances:
-                instance.exchange.stop().start()
-
     def _select_plugins(self, _widget):
         PluginSelectionWindow(self)
 
     # Menu item to remove all tickers and quits the application
     def _quit_all(self, _widget):
         Gtk.main_quit()
```

### Comparing `coindicator-2.1.8/src/coin/coingecko_client.py` & `coindicator-2.1.9/src/coin/coingecko_client.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/config.py` & `coindicator-2.1.9/src/coin/config.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/config.yaml` & `coindicator-2.1.9/src/coin/config.yaml`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/downloader.py` & `coindicator-2.1.9/src/coin/downloader.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/error.py` & `coindicator-2.1.9/src/coin/error.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/exchange.py` & `coindicator-2.1.9/src/coin/exchange.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/exchanges/binance.py` & `coindicator-2.1.9/src/coin/exchanges/binance.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/exchanges/bitfinex.py` & `coindicator-2.1.9/src/coin/exchanges/bitfinex.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/exchanges/bitkub.py` & `coindicator-2.1.9/src/coin/exchanges/bitkub.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/exchanges/bitstamp.py` & `coindicator-2.1.9/src/coin/exchanges/bitstamp.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/exchanges/bittrex.py` & `coindicator-2.1.9/src/coin/exchanges/bittrex.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/exchanges/cexio.py` & `coindicator-2.1.9/src/coin/exchanges/cexio.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/exchanges/gemini.py` & `coindicator-2.1.9/src/coin/exchanges/gemini.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/exchanges/hitbtc.py` & `coindicator-2.1.9/src/coin/exchanges/hitbtc.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/exchanges/kraken.py` & `coindicator-2.1.9/src/coin/exchanges/kraken.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/exchanges/okcoin.py` & `coindicator-2.1.9/src/coin/exchanges/okcoin.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/exchanges/poloniex.py` & `coindicator-2.1.9/src/coin/exchanges/poloniex.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/exchanges/unocoin.py` & `coindicator-2.1.9/src/coin/exchanges/unocoin.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/indicator.py` & `coindicator-2.1.9/src/coin/indicator.py`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/plugin_selection.py` & `coindicator-2.1.9/src/coin/plugin_selection.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,11 @@
 # Plugin selection window
 
-import gi
 from gi.repository import Gdk, Gtk
 
-from .exchange import Exchange
-
 
 class PluginSelectionWindow(Gtk.Window):
     def __init__(self, parent):
         Gtk.Window.__init__(self, title="Plugins")
 
         self.parent = parent
         self.set_keep_above(True)
@@ -31,15 +28,14 @@
 
         rend_checkbox = Gtk.CellRendererToggle()
         rend_checkbox.connect("toggled", self._toggle)
         rend_plugin = Gtk.CellRendererText()
 
         col_chk = Gtk.TreeViewColumn("", rend_checkbox, active=0)
         col_plugin = Gtk.TreeViewColumn("Plugin", rend_plugin, text=1)
-        # col_plugin.set_sort_column_id(0)
 
         self.view_plugins.append_column(col_chk)
         self.view_plugins.append_column(col_plugin)
 
         self.set_focus_child(self.view_plugins)
 
         sw = Gtk.ScrolledWindow()
@@ -61,24 +57,24 @@
         buttonbox.pack_start(button_cancel, True, True, 0)
 
         grid.attach(buttonbox, 0, 245, 100, 50)
 
         self.show_all()
         self.present()
 
-    def _toggle(self, renderer, path):
+    def _toggle(self, _renderer, path):
         iter = self.plugin_store.get_iter(path)
         self.plugin_store[iter][0] = not self.plugin_store[iter][0]
 
-    def _select_plugins(self, widget=None):
+    def _select_plugins(self, _widget=None):
         for item in self.plugin_store:
             item[2].active = item[0]
 
         self.parent.plugins_updated()
         self._close()
 
-    def _on_key_release(self, widget, ev, data=None):
+    def _on_key_release(self, _widget, ev, _data=None):
         if ev.keyval == Gdk.KEY_Escape:
             self._close()
 
-    def _close(self, widget=None):
+    def _close(self, _widget=None):
         self.destroy()
```

### Comparing `coindicator-2.1.8/src/coin/resources/ca-ching.wav` & `coindicator-2.1.9/src/coin/resources/ca-ching.wav`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/resources/icon.png` & `coindicator-2.1.9/src/coin/resources/icon.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/resources/icon_32px.png` & `coindicator-2.1.9/src/coin/resources/icon_32px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/resources/icon_48px.png` & `coindicator-2.1.9/src/coin/resources/icon_48px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/resources/icon_64px.png` & `coindicator-2.1.9/src/coin/resources/icon_64px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/resources/loading.png` & `coindicator-2.1.9/src/coin/resources/loading.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/resources/logo_124px.png` & `coindicator-2.1.9/src/coin/resources/logo_124px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/resources/logo_124pxs.png` & `coindicator-2.1.9/src/coin/resources/logo_124pxs.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coin/resources/logo_248px.png` & `coindicator-2.1.9/src/coin/resources/logo_248px.png`

 * *Files identical despite different names*

### Comparing `coindicator-2.1.8/src/coindicator.egg-info/PKG-INFO` & `coindicator-2.1.9/src/coindicator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coindicator
-Version: 2.1.8
+Version: 2.1.9
 Summary: Coinprice Indicator
 Home-page: https://github.com/bluppfisk/coindicator/
 Author: Sander Van de Moortel
 Author-email: sander.vandemoortel@gmail.com
 License: MIT
 Project-URL: Documentation, https://github.com/bluppfisk/coindicator/
 Platform: Linux
```

### Comparing `coindicator-2.1.8/src/coindicator.egg-info/SOURCES.txt` & `coindicator-2.1.9/src/coindicator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

