# Comparing `tmp/chainfury-0.0.1a0.tar.gz` & `tmp/chainfury-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chainfury-0.0.1a0.tar", max compression
+gzip compressed data, was "chainfury-0.1.0.tar", max compression
```

## Comparing `chainfury-0.0.1a0.tar` & `chainfury-0.1.0.tar`

### file list

```diff
@@ -1,5 +1,11 @@
--rw-r--r--   0        0        0       12 2023-04-23 15:07:33.760461 chainfury-0.0.1a0/README.md
--rw-r--r--   0        0        0       67 2023-04-23 15:07:14.871373 chainfury-0.0.1a0/chainfury/__init__.py
--rw-r--r--   0        0        0      290 2023-04-23 15:06:06.778745 chainfury-0.0.1a0/pyproject.toml
--rw-r--r--   0        0        0      538 1970-01-01 00:00:00.000000 chainfury-0.0.1a0/setup.py
--rw-r--r--   0        0        0      373 1970-01-01 00:00:00.000000 chainfury-0.0.1a0/PKG-INFO
+-rw-r--r--   0        0        0    11351 2023-06-12 10:47:25.719426 chainfury-0.1.0/LICENSE
+-rw-r--r--   0        0        0     7783 2023-06-12 10:47:25.719584 chainfury-0.1.0/README.md
+-rw-r--r--   0        0        0      223 2023-06-19 10:26:36.047002 chainfury-0.1.0/chainfury/__init__.py
+-rw-r--r--   0        0        0    12524 2023-06-19 10:21:46.091911 chainfury-0.1.0/chainfury/agent.py
+-rw-r--r--   0        0        0    30518 2023-06-19 10:28:45.737597 chainfury-0.1.0/chainfury/base.py
+-rw-r--r--   0        0        0      545 2023-06-19 10:42:02.929669 chainfury-0.1.0/chainfury/cli.py
+-rw-r--r--   0        0        0      795 2023-06-19 10:20:57.258296 chainfury-0.1.0/chainfury/utils.py
+-rw-r--r--   0        0        0      113 2023-06-19 10:27:02.042189 chainfury-0.1.0/chainfury/version.py
+-rw-r--r--   0        0        0      628 2023-06-19 10:26:18.352503 chainfury-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     8882 1970-01-01 00:00:00.000000 chainfury-0.1.0/setup.py
+-rw-r--r--   0        0        0     8631 1970-01-01 00:00:00.000000 chainfury-0.1.0/PKG-INFO
```

