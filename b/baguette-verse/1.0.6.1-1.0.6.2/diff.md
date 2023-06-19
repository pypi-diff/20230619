# Comparing `tmp/baguette_verse-1.0.6.1.tar.gz` & `tmp/baguette_verse-1.0.6.2.tar.gz`

## Comparing `baguette_verse-1.0.6.1.tar` & `baguette_verse-1.0.6.2.tar`

### file list

```diff
@@ -1,69 +1,69 @@
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/__init__.py
--rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/baguette.py
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/logger.py
--rw-r--r--   0        0        0    16694 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/rack.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/__init__.py
--rw-r--r--   0        0        0    23828 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/bake.py
--rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/compiler.py
--rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/__init__.py
--rw-r--r--   0        0        0    13119 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/build.py
--rw-r--r--   0        0        0    17960 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/colors.py
--rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/config.py
--rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/event.py
--rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/filters.py
--rw-r--r--   0        0        0    34141 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/graph.py
--rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/record.py
--rw-r--r--   0        0        0     7635 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/utils.py
--rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/__init__.py
--rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/utils.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/data/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/data/__proc__.py
--rw-r--r--   0        0        0    13656 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/data/entities.py
--rw-r--r--   0        0        0     7833 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/data/integration.py
--rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/data/relations.py
--rw-r--r--   0        0        0     9533 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/data/utils.py
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/execution/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/execution/__proc__.py
--rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/execution/entities.py
--rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/execution/integration.py
--rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/execution/relations.py
--rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/execution/utils.py
--rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/filesystem/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/filesystem/__proc__.py
--rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/filesystem/entities.py
--rw-r--r--   0        0        0    13702 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/filesystem/integration.py
--rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/filesystem/relations.py
--rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/imports/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/imports/__proc__.py
--rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/imports/entities.py
--rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/imports/integration.py
--rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/imports/relations.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/network/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/network/__proc__.py
--rw-r--r--   0        0        0    10482 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/network/entities.py
--rw-r--r--   0        0        0     9931 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/network/integration.py
--rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/network/relations.py
--rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/registry/__init__.py
--rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/registry/__proc__.py
--rw-r--r--   0        0        0    11045 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/registry/entities.py
--rw-r--r--   0        0        0    16630 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/registry/integration.py
--rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/bakery/source/types/registry/relations.py
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/croutons/__init__.py
--rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/croutons/extractor.py
--rw-r--r--   0        0        0    20675 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/croutons/toast.py
--rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/croutons/metalib/__init__.py
--rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/croutons/metalib/interact.py
--rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/croutons/metalib/utils.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/croutons/source/__init__.py
--rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/croutons/source/evaluator.py
--rw-r--r--   0        0        0    35062 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/croutons/source/metagraph.py
--rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/croutons/source/utils.py
--rw-r--r--   0        0        0  9439185 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/tutorial/data.zip
--rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/tutorial/scripts.py
--rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/tutorial/state.txt
--rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/baguette/tutorial/utils.py
--rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/.gitignore
--rw-r--r--   0        0        0    35123 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/LICENSE
--rw-r--r--   0        0        0     8463 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/README.md
--rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/pyproject.toml
--rw-r--r--   0        0        0    48841 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.1/PKG-INFO
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/__init__.py
+-rw-r--r--   0        0        0      940 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/baguette.py
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/logger.py
+-rw-r--r--   0        0        0    17408 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/rack.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/__init__.py
+-rw-r--r--   0        0        0    23828 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/bake.py
+-rw-r--r--   0        0        0     6109 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/compiler.py
+-rw-r--r--   0        0        0      173 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/__init__.py
+-rw-r--r--   0        0        0    13119 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/build.py
+-rw-r--r--   0        0        0    17960 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/colors.py
+-rw-r--r--   0        0        0     7862 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/config.py
+-rw-r--r--   0        0        0     4570 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/event.py
+-rw-r--r--   0        0        0     9262 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/filters.py
+-rw-r--r--   0        0        0    34141 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/graph.py
+-rw-r--r--   0        0        0     4633 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/record.py
+-rw-r--r--   0        0        0     7635 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/utils.py
+-rw-r--r--   0        0        0     1620 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/__init__.py
+-rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/utils.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/data/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/data/__proc__.py
+-rw-r--r--   0        0        0    13656 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/data/entities.py
+-rw-r--r--   0        0        0     7833 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/data/integration.py
+-rw-r--r--   0        0        0     3898 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/data/relations.py
+-rw-r--r--   0        0        0     9533 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/data/utils.py
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/execution/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/execution/__proc__.py
+-rw-r--r--   0        0        0    10104 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/execution/entities.py
+-rw-r--r--   0        0        0     3725 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/execution/integration.py
+-rw-r--r--   0        0        0     3144 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/execution/relations.py
+-rw-r--r--   0        0        0     3533 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/execution/utils.py
+-rw-r--r--   0        0        0      328 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/filesystem/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/filesystem/__proc__.py
+-rw-r--r--   0        0        0     6524 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/filesystem/entities.py
+-rw-r--r--   0        0        0    13702 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/filesystem/integration.py
+-rw-r--r--   0        0        0     3743 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/filesystem/relations.py
+-rw-r--r--   0        0        0      323 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/imports/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/imports/__proc__.py
+-rw-r--r--   0        0        0     2071 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/imports/entities.py
+-rw-r--r--   0        0        0     1021 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/imports/integration.py
+-rw-r--r--   0        0        0      855 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/imports/relations.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/network/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/network/__proc__.py
+-rw-r--r--   0        0        0    10482 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/network/entities.py
+-rw-r--r--   0        0        0     9931 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/network/integration.py
+-rw-r--r--   0        0        0     5164 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/network/relations.py
+-rw-r--r--   0        0        0      322 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/registry/__init__.py
+-rw-r--r--   0        0        0      381 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/registry/__proc__.py
+-rw-r--r--   0        0        0    11045 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/registry/entities.py
+-rw-r--r--   0        0        0    16630 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/registry/integration.py
+-rw-r--r--   0        0        0     2659 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/bakery/source/types/registry/relations.py
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/croutons/__init__.py
+-rw-r--r--   0        0        0     5559 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/croutons/extractor.py
+-rw-r--r--   0        0        0    20675 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/croutons/toast.py
+-rw-r--r--   0        0        0      680 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/croutons/metalib/__init__.py
+-rw-r--r--   0        0        0      833 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/croutons/metalib/interact.py
+-rw-r--r--   0        0        0     4784 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/croutons/metalib/utils.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/croutons/source/__init__.py
+-rw-r--r--   0        0        0     2488 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/croutons/source/evaluator.py
+-rw-r--r--   0        0        0    35062 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/croutons/source/metagraph.py
+-rw-r--r--   0        0        0     4103 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/croutons/source/utils.py
+-rw-r--r--   0        0        0  9439185 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/tutorial/data.zip
+-rw-r--r--   0        0        0    16890 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/tutorial/scripts.py
+-rw-r--r--   0        0        0       11 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/tutorial/state.txt
+-rw-r--r--   0        0        0     4603 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/baguette/tutorial/utils.py
+-rw-r--r--   0        0        0     2078 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/.gitignore
+-rw-r--r--   0        0        0    35123 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/LICENSE
+-rw-r--r--   0        0        0     8463 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/README.md
+-rw-r--r--   0        0        0     1645 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/pyproject.toml
+-rw-r--r--   0        0        0    48841 2020-02-02 00:00:00.000000 baguette_verse-1.0.6.2/PKG-INFO
```

### Comparing `baguette_verse-1.0.6.1/baguette/baguette.py` & `baguette_verse-1.0.6.2/baguette/baguette.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/logger.py` & `baguette_verse-1.0.6.2/baguette/logger.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/rack.py` & `baguette_verse-1.0.6.2/baguette/rack.py`

 * *Files 3% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 from pathlib import Path
 from traceback import TracebackException
 from typing import Any, Literal, TypeVar
 
 from .croutons.source.metagraph import MetaGraph
 from .bakery.source.filters import Filter
+from .bakery.source.graph import Graph
 from .bakery.source.colors import Color
 
 __all__ = ["BaguetteRack", "TimeoutExit"]
 
 
 
 
@@ -453,11 +454,28 @@
         if self.visual.is_file():
             remove(self.visual)
         if self.extracted.is_file():
             remove(self.extracted)
         if not list(self.working_directory.iterdir()):
             rmdir(self.working_directory)
 
+    def load(self) -> Graph:
+        """
+        Loads and returns the baguette associated to this graph.
+        """
+        if not self.baguette.exists():
+            raise FileNotFoundError("Baguette file does not exist")
+        if not self.baguette.is_file():
+            raise FileExistsError("Baguette path exists but is not a file")
+        from pickle import load
+        from baguette.bakery.source.graph import Graph
+        with self.baguette.open("rb") as f:
+            bag = load(f)
+            if not isinstance(bag, Graph):
+                raise RuntimeError("Given baguette file did not contain a BAGUETTE graph")
+            return bag
+
+
 
 
 
 del Path, T, TypeVar, Any, TracebackException
```

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/bake.py` & `baguette_verse-1.0.6.2/baguette/bakery/bake.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/compiler.py` & `baguette_verse-1.0.6.2/baguette/bakery/compiler.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/build.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/build.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/colors.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/colors.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/config.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/config.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/event.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/event.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/filters.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/filters.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/graph.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/graph.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/record.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/record.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/utils.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/types/__init__.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/types/__init__.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/types/utils.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/types/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/types/data/entities.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/types/data/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/types/data/integration.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/types/data/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/types/data/relations.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/types/data/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/types/data/utils.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/types/data/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/types/execution/entities.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/types/execution/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/types/execution/integration.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/types/execution/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/types/execution/relations.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/types/execution/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/types/execution/utils.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/types/execution/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/types/filesystem/entities.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/types/filesystem/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/types/filesystem/integration.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/types/filesystem/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/types/filesystem/relations.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/types/filesystem/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/types/imports/entities.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/types/imports/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/types/imports/integration.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/types/imports/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/types/imports/relations.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/types/imports/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/types/network/entities.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/types/network/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/types/network/integration.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/types/network/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/types/network/relations.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/types/network/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/types/registry/entities.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/types/registry/entities.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/types/registry/integration.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/types/registry/integration.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/bakery/source/types/registry/relations.py` & `baguette_verse-1.0.6.2/baguette/bakery/source/types/registry/relations.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/croutons/extractor.py` & `baguette_verse-1.0.6.2/baguette/croutons/extractor.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/croutons/toast.py` & `baguette_verse-1.0.6.2/baguette/croutons/toast.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/croutons/metalib/__init__.py` & `baguette_verse-1.0.6.2/baguette/croutons/metalib/__init__.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/croutons/metalib/interact.py` & `baguette_verse-1.0.6.2/baguette/croutons/metalib/interact.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/croutons/metalib/utils.py` & `baguette_verse-1.0.6.2/baguette/croutons/metalib/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/croutons/source/evaluator.py` & `baguette_verse-1.0.6.2/baguette/croutons/source/evaluator.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/croutons/source/metagraph.py` & `baguette_verse-1.0.6.2/baguette/croutons/source/metagraph.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/croutons/source/utils.py` & `baguette_verse-1.0.6.2/baguette/croutons/source/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/tutorial/data.zip` & `baguette_verse-1.0.6.2/baguette/tutorial/data.zip`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/tutorial/scripts.py` & `baguette_verse-1.0.6.2/baguette/tutorial/scripts.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/baguette/tutorial/utils.py` & `baguette_verse-1.0.6.2/baguette/tutorial/utils.py`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/.gitignore` & `baguette_verse-1.0.6.2/.gitignore`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/LICENSE` & `baguette_verse-1.0.6.2/LICENSE`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/README.md` & `baguette_verse-1.0.6.2/README.md`

 * *Files identical despite different names*

### Comparing `baguette_verse-1.0.6.1/pyproject.toml` & `baguette_verse-1.0.6.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "baguette-verse"
-version = "1.0.6.1"
+version = "1.0.6.2"
 authors = [
   { name="Vincent Raulin", email="vincent.raulin@inria.fr" },
 ]
 description = "A malware behavioral analysis framework centered around BAGUETTE!"
 readme = "README.md"
 license = {file = "LICENSE"}
 requires-python = ">=3.10"
```

### Comparing `baguette_verse-1.0.6.1/PKG-INFO` & `baguette_verse-1.0.6.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: baguette-verse
-Version: 1.0.6.1
+Version: 1.0.6.2
 Summary: A malware behavioral analysis framework centered around BAGUETTE!
 Project-URL: Repository, https://gitlab.inria.fr/vraulin/baguette-verse
 Project-URL: Bug Tracker, https://gitlab.inria.fr/vraulin/baguette-verse/-/issues
 Author-email: Vincent Raulin <vincent.raulin@inria.fr>
 License:                     GNU AFFERO GENERAL PUBLIC LICENSE
                                Version 3, 19 November 2007
```

