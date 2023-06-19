# Comparing `tmp/fparser-0.1.1.tar.gz` & `tmp/fparser-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fparser-0.1.1.tar", last modified: Fri Apr 28 16:00:39 2023, max compression
+gzip compressed data, was "fparser-0.1.2.tar", last modified: Mon Jun 19 09:44:19 2023, max compression
```

## Comparing `fparser-0.1.1.tar` & `fparser-0.1.2.tar`

### file list

```diff
@@ -1,242 +1,247 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.167790 fparser-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-28 16:00:25.000000 fparser-0.1.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.131790 fparser-0.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.135790 fparser-0.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-04-28 16:00:25.000000 fparser-0.1.1/.github/workflows/python_publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-04-28 16:00:25.000000 fparser-0.1.1/.github/workflows/unit-tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-28 16:00:25.000000 fparser-0.1.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    17107 2023-04-28 16:00:25.000000 fparser-0.1.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-04-28 16:00:25.000000 fparser-0.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-04-28 16:00:25.000000 fparser-0.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-28 16:00:39.167790 fparser-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2389 2023-04-28 16:00:25.000000 fparser-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.135790 fparser-0.1.1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-28 16:00:25.000000 fparser-0.1.1/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)   114630 2023-04-28 16:00:25.000000 fparser-0.1.1/doc/doxygen.config
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-28 16:00:25.000000 fparser-0.1.1/doc/pip_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.139790 fparser-0.1.1/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-04-28 16:00:25.000000 fparser-0.1.1/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    42926 2023-04-28 16:00:25.000000 fparser-0.1.1/doc/source/developers_guide.rst
--rw-r--r--   0 runner    (1001) docker     (123)    19397 2023-04-28 16:00:25.000000 fparser-0.1.1/doc/source/fparser.rst
--rw-r--r--   0 runner    (1001) docker     (123)    21088 2023-04-28 16:00:25.000000 fparser-0.1.1/doc/source/fparser2.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-04-28 16:00:25.000000 fparser-0.1.1/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-04-28 16:00:25.000000 fparser-0.1.1/doc/source/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-04-28 16:00:25.000000 fparser-0.1.1/doc/source/license.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-04-28 16:00:25.000000 fparser-0.1.1/doc/source/reference_guide.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.139790 fparser-0.1.1/example/
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-28 16:00:25.000000 fparser-0.1.1/example/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-28 16:00:25.000000 fparser-0.1.1/example/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     6102 2023-04-28 16:00:25.000000 fparser-0.1.1/example/create_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-04-28 16:00:25.000000 fparser-0.1.1/example/fparser2_f2008.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.139790 fparser-0.1.1/example/test_files/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-28 16:00:25.000000 fparser-0.1.1/example/test_files/a.f90
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-04-28 16:00:25.000000 fparser-0.1.1/example/test_files/b.f90
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-04-28 16:00:25.000000 fparser-0.1.1/example/test_files/c.f90
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-04-28 16:00:25.000000 fparser-0.1.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-04-28 16:00:39.167790 fparser-0.1.1/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)     3618 2023-04-28 16:00:25.000000 fparser-0.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.131790 fparser-0.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.139790 fparser-0.1.1/src/fparser/
--rw-r--r--   0 runner    (1001) docker     (123)      614 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-28 16:00:39.000000 fparser-0.1.1/src/fparser/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)    10705 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.139790 fparser-0.1.1/src/fparser/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    35934 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    62920 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/readfortran.py
--rw-r--r--   0 runner    (1001) docker     (123)    12263 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/sourceinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    15228 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/splitline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.143790 fparser-0.1.1/src/fparser/common/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/tests/logging_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/tests/modfile.f95
--rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/tests/test_base_classes.py
--rw-r--r--   0 runner    (1001) docker     (123)    48185 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/tests/test_readfortran.py
--rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/tests/test_sourceinfo.py
--rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/tests/test_splitline.py
--rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/tests/utf.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/tests/utf_in_code.f90
--rw-r--r--   0 runner    (1001) docker     (123)    12533 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/common/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.143790 fparser-0.1.1/src/fparser/one/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    51336 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/block_statements.py
--rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/parsefortran.py
--rw-r--r--   0 runner    (1001) docker     (123)    78902 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/statements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.143790 fparser-0.1.1/src/fparser/one/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/tests/bad_char.f90
--rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/tests/test_block_stmts.py
--rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/tests/test_do_block_r814.py
--rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/tests/test_parsefortran.py
--rw-r--r--   0 runner    (1001) docker     (123)    38497 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/tests/test_scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)    17066 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/tests/test_select.py
--rw-r--r--   0 runner    (1001) docker     (123)    24502 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/one/typedecl_statements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.147790 fparser-0.1.1/src/fparser/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/scripts/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5268 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/scripts/fparser2.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3985 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/scripts/fparser2_bench.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4640 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/scripts/parse.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4934 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/scripts/read.py
--rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/scripts/script_options.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.147790 fparser-0.1.1/src/fparser/scripts/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/scripts/tests/test_fparser2_bench.py
--rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/scripts/tests/test_scripts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.151790 fparser-0.1.1/src/fparser/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/funcfile.f95
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/modfile.f95
--rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_blank_lines.py
--rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_comment.py
--rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_f90comment_f77source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_fparser_module.py
--rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_functional.py
--rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_issue10.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_issue11.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_issue23.py
--rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_issue25.py
--rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_issue26.py
--rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_issue33.py
--rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_issue4.py
--rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_issue5.py
--rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_issue7.py
--rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_issue8.py
--rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_issue9.py
--rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/tests/test_mod_private.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.151790 fparser-0.1.1/src/fparser/two/
--rw-r--r--   0 runner    (1001) docker     (123)    24469 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/C99Preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)   379425 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/Fortran2003.py
--rw-r--r--   0 runner    (1001) docker     (123)    55113 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/Fortran2008.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12517 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    19850 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/pattern_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    26435 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/symbol_table.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.151790 fparser-0.1.1/src/fparser/two/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.163790 fparser-0.1.1/src/fparser/two/tests/fortran2003/
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_add_operand_r705.py
--rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_allocate_stmt_r623.py
--rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_array_constructor_implied_do_ctl_r471.py
--rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_array_constructor_implied_do_r470.py
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_array_constructor_r465.py
--rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_array_constructor_spec_r466.py
--rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_associate_construct_r816.py
--rw-r--r--   0 runner    (1001) docker     (123)     8630 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_block_do_construct_r826.py
--rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_case_construct_r808.py
--rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_char_expr_r725.py
--rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_char_literal_constant_r427.py
--rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_component_part_r438.py
--rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_control_edit_descriptor_r1011.py
--rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_cray_pointee_array_spec.py
--rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_cray_pointee_decl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_cray_pointer_decl.py
--rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_cray_pointer_stmt.py
--rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_data_edit_desc_c1002.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_data_ref_r612.py
--rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_declaration_construct_r207.py
--rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_default_char_expr_r726.py
--rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_defined_operator_r311.py
--rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_defined_operators_r703_r723.py
--rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_derived_type_stmt_r430.py
--rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_designator_r603.py
--rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_entity_decl_r504.py
--rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_executable_construct_r213.py
--rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_extended_intrinsic_op_r312.py
--rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_forall_header_r754.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_forall_stmt_r759.py
--rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_format_item_c1002.py
--rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_format_item_list.py
--rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_format_item_r1003.py
--rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_format_specification_r1002.py
--rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_function_stmt_r1224.py
--rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_hollerith_item.py
--rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_if_construct_r802.py
--rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_if_stmt_r807.py
--rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_import_stmt_r1209.py
--rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_include_filename.py
--rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_include_statement.py
--rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_int_expr_r727.py
--rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_intrinsics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_io_control_spec_r913.py
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_kindselector_r404.py
--rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_level_2_expr_r706.py
--rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_logical_expr_r724.py
--rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_main_program_r1101.py
--rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_module_r1104.py
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_name_r304.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_nonblock_do_construct_r835.py
--rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_numeric_expr_r728.py
--rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_position_edit_desc_r1013.py
--rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_prefix_r1227.py
--rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_primary_r701.py
--rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_program_r201.py
--rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_program_stmt_r1102.py
--rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_rename_r1111.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_select_type_construct_r821.py
--rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_specific_binding_r451.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_stmt_function_stmt_r1238.py
--rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_subroutine_stmt_r1232.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_type_decl_stmt_r501.py
--rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_usestmt_r1109.py
--rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_where_construct_r744.py
--rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2003/test_write_stmt_r911.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.167790 fparser-0.1.1/src/fparser/two/tests/fortran2008/
--rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_action_stmt_r214.py
--rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_alloc_opt_r627.py
--rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_attr_spec_r502.py
--rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_block.py
--rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_coarray_spec_r509.py
--rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_component_attr_spec_r437.py
--rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_critical.py
--rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_data_component_def_stmt_r436.py
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_deferred_coshape_spec_r510.py
--rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_end_submodule_stmt_r1119.py
--rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_error_stop_stmt_r856.py
--rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_explicit_coshape_spec_r511.py
--rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_if_stmt_r837.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_lower_cobound_r512.py
--rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_open_stmt_r904.py
--rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_parent_identifier_r1118.py
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_procedure_stmt_r1206.py
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_program_unit_r202.py
--rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_submodule_r1116.py
--rw-r--r--   0 runner    (1001) docker     (123)     5422 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_submodule_stmt_r1117.py
--rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_type_declaration_stmt_r501.py
--rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/fortran2008/test_upper_cobound_r513.py
--rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/test_bases.py
--rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/test_c99preprocessor.py
--rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/test_comments.py
--rw-r--r--   0 runner    (1001) docker     (123)   100962 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/test_fortran2003.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/test_module_use.py
--rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/test_pattern_tools.py
--rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/test_symbol_table.py
--rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/test_symbol_tables.py
--rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.167790 fparser-0.1.1/src/fparser/two/tests/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/utils/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/utils/test_binaryopbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     9674 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/utils/test_blockbase.py
--rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/utils/test_bracket_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/utils/test_call_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/utils/test_get_child.py
--rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/utils/test_sequencebase.py
--rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/utils/test_stringbase_upper.py
--rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/utils/test_walk.py
--rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/tests/utils/test_wordclsbase.py
--rw-r--r--   0 runner    (1001) docker     (123)    70927 2023-04-28 16:00:25.000000 fparser-0.1.1/src/fparser/two/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 16:00:39.139790 fparser-0.1.1/src/fparser.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3450 2023-04-28 16:00:39.000000 fparser-0.1.1/src/fparser.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9780 2023-04-28 16:00:39.000000 fparser-0.1.1/src/fparser.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 16:00:39.000000 fparser-0.1.1/src/fparser.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-28 16:00:39.000000 fparser-0.1.1/src/fparser.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-28 16:00:39.000000 fparser-0.1.1/src/fparser.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-28 16:00:39.000000 fparser-0.1.1/src/fparser.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:19.263142 fparser-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-06-19 09:44:05.000000 fparser-0.1.2/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:19.235142 fparser-0.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:19.235142 fparser-0.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-06-19 09:44:05.000000 fparser-0.1.2/.github/workflows/python_publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-06-19 09:44:05.000000 fparser-0.1.2/.github/workflows/unit-tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-19 09:44:05.000000 fparser-0.1.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    17588 2023-06-19 09:44:05.000000 fparser-0.1.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-06-19 09:44:05.000000 fparser-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3540 2023-06-19 09:44:05.000000 fparser-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-06-19 09:44:19.263142 fparser-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2513 2023-06-19 09:44:05.000000 fparser-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:19.235142 fparser-0.1.2/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-06-19 09:44:05.000000 fparser-0.1.2/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)   114630 2023-06-19 09:44:05.000000 fparser-0.1.2/doc/doxygen.config
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-06-19 09:44:05.000000 fparser-0.1.2/doc/pip_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:19.239142 fparser-0.1.2/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1833 2023-06-19 09:44:05.000000 fparser-0.1.2/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42926 2023-06-19 09:44:05.000000 fparser-0.1.2/doc/source/developers_guide.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    19397 2023-06-19 09:44:05.000000 fparser-0.1.2/doc/source/fparser.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    21119 2023-06-19 09:44:05.000000 fparser-0.1.2/doc/source/fparser2.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3932 2023-06-19 09:44:05.000000 fparser-0.1.2/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-06-19 09:44:05.000000 fparser-0.1.2/doc/source/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3490 2023-06-19 09:44:05.000000 fparser-0.1.2/doc/source/license.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-06-19 09:44:05.000000 fparser-0.1.2/doc/source/reference_guide.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:19.239142 fparser-0.1.2/example/
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-06-19 09:44:05.000000 fparser-0.1.2/example/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-06-19 09:44:05.000000 fparser-0.1.2/example/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6102 2023-06-19 09:44:05.000000 fparser-0.1.2/example/create_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2127 2023-06-19 09:44:05.000000 fparser-0.1.2/example/fparser2_f2008.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:19.239142 fparser-0.1.2/example/test_files/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-19 09:44:05.000000 fparser-0.1.2/example/test_files/a.f90
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-06-19 09:44:05.000000 fparser-0.1.2/example/test_files/b.f90
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-06-19 09:44:05.000000 fparser-0.1.2/example/test_files/c.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-06-19 09:44:05.000000 fparser-0.1.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-06-19 09:44:19.263142 fparser-0.1.2/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3618 2023-06-19 09:44:05.000000 fparser-0.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:19.235142 fparser-0.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:19.239142 fparser-0.1.2/src/fparser/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-06-19 09:44:19.000000 fparser-0.1.2/src/fparser/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10705 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:19.239142 fparser-0.1.2/src/fparser/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35934 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/common/base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63373 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/common/readfortran.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12263 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/common/sourceinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15228 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/common/splitline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:19.243142 fparser-0.1.2/src/fparser/common/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/common/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1993 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/common/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3557 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/common/tests/logging_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/common/tests/modfile.f95
+-rw-r--r--   0 runner    (1001) docker     (123)     6903 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/common/tests/test_base_classes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49110 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/common/tests/test_readfortran.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12954 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/common/tests/test_sourceinfo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10699 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/common/tests/test_splitline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5081 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/common/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/common/tests/utf.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/common/tests/utf_in_code.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    12533 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/common/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2578 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:19.243142 fparser-0.1.2/src/fparser/one/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/one/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51336 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/one/block_statements.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6169 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/one/parsefortran.py
+-rw-r--r--   0 runner    (1001) docker     (123)    78902 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/one/statements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:19.243142 fparser-0.1.2/src/fparser/one/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/one/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1838 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/one/tests/bad_char.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     5131 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/one/tests/test_block_stmts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7017 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/one/tests/test_do_block_r814.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8656 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/one/tests/test_parsefortran.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38497 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/one/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3647 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/one/tests/test_scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17066 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/one/tests/test_select.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24502 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/one/typedecl_statements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:19.243142 fparser-0.1.2/src/fparser/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1870 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/scripts/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5268 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/scripts/fparser2.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3985 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/scripts/fparser2_bench.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4640 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/scripts/parse.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4934 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/scripts/read.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5319 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/scripts/script_options.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:19.243142 fparser-0.1.2/src/fparser/scripts/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2869 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/scripts/tests/test_fparser2_bench.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21396 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/scripts/tests/test_scripts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:19.247142 fparser-0.1.2/src/fparser/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/tests/funcfile.f95
+-rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/tests/modfile.f95
+-rw-r--r--   0 runner    (1001) docker     (123)     7978 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4263 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/tests/test_blank_lines.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5670 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/tests/test_comment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3863 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/tests/test_f90comment_f77source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3700 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/tests/test_fparser_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/tests/test_functional.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3895 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/tests/test_issue10.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/tests/test_issue11.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/tests/test_issue23.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4117 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/tests/test_issue25.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4169 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/tests/test_issue26.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3988 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/tests/test_issue33.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5584 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/tests/test_issue4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4408 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/tests/test_issue5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7198 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/tests/test_issue7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6569 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/tests/test_issue8.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4035 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/tests/test_issue9.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4267 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/tests/test_mod_private.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:19.247142 fparser-0.1.2/src/fparser/two/
+-rw-r--r--   0 runner    (1001) docker     (123)    24469 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/C99Preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)   380626 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/Fortran2003.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:19.247142 fparser-0.1.2/src/fparser/two/Fortran2008/
+-rw-r--r--   0 runner    (1001) docker     (123)    59240 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/Fortran2008/Fortran2008.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4634 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/Fortran2008/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12586 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19850 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/pattern_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26435 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/symbol_table.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:19.251142 fparser-0.1.2/src/fparser/two/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1791 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     2749 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:19.259142 fparser-0.1.2/src/fparser/two/tests/fortran2003/
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_add_operand_r705.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4038 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_allocate_stmt_r623.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_array_constructor_implied_do_ctl_r471.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2818 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_array_constructor_implied_do_r470.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_array_constructor_r465.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_array_constructor_spec_r466.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5951 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_associate_construct_r816.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8630 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_block_do_construct_r826.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5895 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_case_construct_r808.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3462 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_char_expr_r725.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5994 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_char_literal_constant_r427.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4262 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_component_part_r438.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5235 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_control_edit_descriptor_r1011.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2862 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_cray_pointee_array_spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2900 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_cray_pointee_decl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4867 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_cray_pointer_decl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4495 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_cray_pointer_stmt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6967 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_data_edit_desc_c1002.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_data_ref_r612.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5574 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_declaration_construct_r207.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3523 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_default_char_expr_r726.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2916 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_defined_operator_r311.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3237 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_defined_operators_r703_r723.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5441 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_derived_type_stmt_r430.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7630 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_designator_r603.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2856 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_entity_decl_r504.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4292 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_executable_construct_r213.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3115 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_extended_intrinsic_op_r312.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4392 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_forall_header_r754.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_forall_stmt_r759.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4368 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_format_item_c1002.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7202 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_format_item_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7391 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_format_item_r1003.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11518 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_format_specification_r1002.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2714 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_function_stmt_r1224.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5051 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_hollerith_item.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8547 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_if_construct_r802.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3458 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_if_stmt_r807.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3000 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_import_stmt_r1209.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3483 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_include_filename.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_include_statement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3328 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_int_expr_r727.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_intrinsics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10401 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_io_control_spec_r913.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_kindselector_r404.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_level_2_expr_r706.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3839 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_logical_expr_r724.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4177 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_loop_control_r830.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7005 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_main_program_r1101.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2593 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_module_r1104.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_name_r304.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3179 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_namelist_stmt_r552.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_nonblock_do_construct_r835.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5475 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_numeric_expr_r728.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4844 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_position_edit_desc_r1013.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5628 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_prefix_r1227.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_primary_r701.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13292 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_program_r201.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3451 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_program_stmt_r1102.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2759 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_rename_r1111.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_select_type_construct_r821.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6104 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_specific_binding_r451.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_stmt_function_stmt_r1238.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2718 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_subroutine_stmt_r1232.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_type_decl_stmt_r501.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_usestmt_r1109.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7251 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_where_construct_r744.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5487 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2003/test_write_stmt_r911.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:19.259142 fparser-0.1.2/src/fparser/two/tests/fortran2008/
+-rw-r--r--   0 runner    (1001) docker     (123)     2275 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2008/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6560 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2008/test_action_stmt_r214.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2832 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2008/test_alloc_opt_r627.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2008/test_attr_spec_r502.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6649 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2008/test_block.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2922 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2008/test_coarray_spec_r509.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5019 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2008/test_component_attr_spec_r437.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4381 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2008/test_critical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1898 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2008/test_data_component_def_stmt_r436.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2008/test_deferred_coshape_spec_r510.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3440 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2008/test_end_submodule_stmt_r1119.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3494 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2008/test_error_stop_stmt_r856.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2008/test_explicit_coshape_spec_r511.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3493 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2008/test_if_stmt_r837.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2008/test_loop_control_r818.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2008/test_lower_cobound_r512.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6121 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2008/test_open_stmt_r904.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4233 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2008/test_parent_identifier_r1118.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2008/test_procedure_stmt_r1206.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2008/test_program_unit_r202.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7801 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2008/test_submodule_r1116.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5448 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2008/test_submodule_stmt_r1117.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4493 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2008/test_type_declaration_stmt_r501.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2682 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/fortran2008/test_upper_cobound_r513.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6016 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/test_bases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17753 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/test_c99preprocessor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/test_comments.py
+-rw-r--r--   0 runner    (1001) docker     (123)    99863 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/test_fortran2003.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/test_module_use.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3834 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5730 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/test_pattern_tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12803 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/test_symbol_table.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6657 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/test_symbol_tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5768 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:19.263142 fparser-0.1.2/src/fparser/two/tests/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     3611 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/utils/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7854 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/utils/test_binaryopbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9674 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/utils/test_blockbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7581 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/utils/test_bracket_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4376 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/utils/test_call_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2987 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/utils/test_get_child.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5179 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/utils/test_sequencebase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4903 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/utils/test_stringbase_upper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4838 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/utils/test_walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7596 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/tests/utils/test_wordclsbase.py
+-rw-r--r--   0 runner    (1001) docker     (123)    70927 2023-06-19 09:44:05.000000 fparser-0.1.2/src/fparser/two/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 09:44:19.239142 fparser-0.1.2/src/fparser.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-06-19 09:44:19.000000 fparser-0.1.2/src/fparser.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10013 2023-06-19 09:44:19.000000 fparser-0.1.2/src/fparser.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 09:44:19.000000 fparser-0.1.2/src/fparser.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-06-19 09:44:19.000000 fparser-0.1.2/src/fparser.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-06-19 09:44:19.000000 fparser-0.1.2/src/fparser.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 09:44:19.000000 fparser-0.1.2/src/fparser.egg-info/top_level.txt
```

### Comparing `fparser-0.1.1/.github/workflows/python_publish.yml` & `fparser-0.1.2/.github/workflows/python_publish.yml`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/.github/workflows/unit-tests.yml` & `fparser-0.1.2/.github/workflows/unit-tests.yml`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/.gitignore` & `fparser-0.1.2/.gitignore`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/CHANGELOG.md` & `fparser-0.1.2/CHANGELOG.md`

 * *Files 3% similar despite different names*

```diff
@@ -14,14 +14,26 @@
 * A. R. Porter, Science & Technology Facilities Council, UK
 * B. Reuter, ECMWF, UK
 * S. Siso, Science & Technology Facilities Council, UK
 * J. Tiira, University of Helsinki, Finland
 * P. Vitt, University of Siegen, Germany
 * A. Voysey, UK Met Office
 
+12/06/2023 PR #417 towards #411. Moves Fortran2008.py into a 'Fortran2008'
+           directory and moves the associated class generation into an '__init__.py'
+           in that directory.
+
+16/05/2023 PR #414 for #412. Bug fix for disappearing line when parsing
+           include files.
+
+15/05/2023 PR #415 for #165. Bug fix for code aborting when trying to match
+           'NAMELIST' in certain contexts.
+
+15/05/2023 PR #408 for #403. Add support for the F2008 DO CONCURRENT.
+
 26/04/2023 PR #406 for #405. Add support for F2008 optional "::" in PROCEDURE
            statement.
 
 03/04/2023 PR #392 for #326. Add support for F2008 block and critical constructs.
 
 30/03/2023 PR #396 for #395. Fix trailing whitespace bug in CallBase.
```

### Comparing `fparser-0.1.1/LICENSE` & `fparser-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/MANIFEST.in` & `fparser-0.1.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/PKG-INFO` & `fparser-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fparser
-Version: 0.1.1
+Version: 0.1.2
 Summary: The fparser project
 Home-page: https://github.com/stfc/fparser
 Author: Pearu Peterson, Rupert Ford, Andrew Porter
 Author-email: andrew.porter@stfc.ac.uk
 License: BSD 3-Clause License
 Project-URL: Source, https://github.com/stfc/fparser
 Project-URL: Tracker, https://github.com/stfc/fparser/issues
@@ -25,14 +25,16 @@
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: tests
 License-File: LICENSE
 
 # News #
 
+  * 28/04/2023 Version 0.1.1 released (extends F2008 support with the optional
+    "::" in the MODULE PROCEDURE statement).
   * 18/04/2023 Version 0.1.0 released and status changed from `alpha` to `beta`. See the [CHANGELOG](CHANGELOG.md) for more details.
   * 16/06/2022 Version 0.0.16 released. See the [CHANGELOG](CHANGELOG.md)
     for details.
   * 30/05/2022 Version 0.0.15 released. See the [CHANGELOG](CHANGELOG.md)
     for details.
   * 10/03/2022 Version 0.0.14 released. See the [CHANGELOG](CHANGELOG.md)
     for details.
```

### Comparing `fparser-0.1.1/README.md` & `fparser-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # News #
 
+  * 28/04/2023 Version 0.1.1 released (extends F2008 support with the optional
+    "::" in the MODULE PROCEDURE statement).
   * 18/04/2023 Version 0.1.0 released and status changed from `alpha` to `beta`. See the [CHANGELOG](CHANGELOG.md) for more details.
   * 16/06/2022 Version 0.0.16 released. See the [CHANGELOG](CHANGELOG.md)
     for details.
   * 30/05/2022 Version 0.0.15 released. See the [CHANGELOG](CHANGELOG.md)
     for details.
   * 10/03/2022 Version 0.0.14 released. See the [CHANGELOG](CHANGELOG.md)
     for details.
```

### Comparing `fparser-0.1.1/doc/Makefile` & `fparser-0.1.2/doc/Makefile`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/doc/doxygen.config` & `fparser-0.1.2/doc/doxygen.config`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/doc/pip_requirements.txt` & `fparser-0.1.2/doc/pip_requirements.txt`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/doc/source/conf.py` & `fparser-0.1.2/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/doc/source/developers_guide.rst` & `fparser-0.1.2/doc/source/developers_guide.rst`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/doc/source/fparser.rst` & `fparser-0.1.2/doc/source/fparser.rst`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/doc/source/fparser2.rst` & `fparser-0.1.2/doc/source/fparser2.rst`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,16 @@
 Fortran 2003. This is implemented in the Fortran2003.py `file`__ and
 contains an entirely separate parser to fparser1 that includes rules
 for Fortran 2003 syntax. Support for Fortran 2008 is being added in
 the Fortran2008.py `file`__ which extends the Fortran2003 rules
 appropriately. At this time fparser2 supports the following
 Fortran2008 features: submodules, co-arrays, the 'mold' argument to
 allocate, the 'contiguous' keyword, the 'BLOCK' construct, the
-'CRITICAL' construct and the optional '::' for a procedure statement.
+'CRITICAL' construct, the optional '::' for a procedure statement and
+the 'do concurrent' construct.
 
 __ https://github.com/stfc/fparser/blob/master/src/fparser/two/Fortran2003.py
 __ https://github.com/stfc/fparser/blob/master/src/fparser/two/Fortran2008.py
 
 
 Getting Going : Script
 ----------------------
```

### Comparing `fparser-0.1.1/doc/source/index.rst` & `fparser-0.1.2/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/doc/source/introduction.rst` & `fparser-0.1.2/doc/source/introduction.rst`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/doc/source/license.rst` & `fparser-0.1.2/doc/source/license.rst`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/doc/source/reference_guide.rst` & `fparser-0.1.2/doc/source/reference_guide.rst`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/example/Makefile` & `fparser-0.1.2/example/Makefile`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/example/README.md` & `fparser-0.1.2/example/README.md`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/example/create_dependencies.py` & `fparser-0.1.2/example/create_dependencies.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/example/fparser2_f2008.py` & `fparser-0.1.2/example/fparser2_f2008.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/setup.cfg` & `fparser-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/setup.py` & `fparser-0.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/.pylintrc` & `fparser-0.1.2/src/fparser/.pylintrc`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/__init__.py` & `fparser-0.1.2/src/fparser/__init__.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/api.py` & `fparser-0.1.2/src/fparser/api.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/common/base_classes.py` & `fparser-0.1.2/src/fparser/common/base_classes.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/common/readfortran.py` & `fparser-0.1.2/src/fparser/common/readfortran.py`

 * *Files 1% similar despite different names*

```diff
@@ -741,16 +741,27 @@
         try:
             item = self.next(ignore_comments=ignore_comments)
         except StopIteration:
             return
         return item
 
     def put_item(self, item):
-        """Insert item to FIFO item buffer."""
-        self.fifo_item.insert(0, item)
+        """Insert item into FIFO buffer of 'innermost' reader object.
+
+        :param item: the item to insert into the FIFO.
+        :type item: :py:class:`fparser.common.readfortran.Line` | \
+                    :py:class:`fparser.common.readfortran.MultiLine` | \
+                    :py:class:`fparser.common.readfortran.Comment`
+        """
+        if self.reader:
+            # We are reading an INCLUDE file so put this item in the FIFO
+            # of the corresponding reader.
+            self.reader.put_item(item)
+        else:
+            self.fifo_item.insert(0, item)
 
     # Iterator methods:
 
     def __iter__(self):
         """Make FortranReader an iterator."""
         return self
 
@@ -763,28 +774,27 @@
 
         :param bool ignore_comments: When True then act as if Fortran \
         code does not contain any comments or blank lines. if this \
         optional arguement is not provided then use the default \
         value.
 
         :returns: the next line item. This can be from a local fifo \
-        buffer, from an include reader or from this reader.
+                  buffer, from an include reader or from this reader.
         :rtype: py:class:`fparser.common.readfortran.Line`
 
         :raises StopIteration: if no more lines are found.
         :raises StopIteration: if a general error has occured.
 
         """
         if ignore_comments is None:
             ignore_comments = self._ignore_comments
         try:
             if self.reader is not None:
                 # inside INCLUDE statement
                 try:
-                    # Return a line from the include.
                     return self.reader.next(ignore_comments)
                 except StopIteration:
                     # There is nothing left in the include
                     # file. Setting reader to None indicates that
                     # we should now read from the main reader.
                     self.reader = None
             item = self._next(ignore_comments)
```

### Comparing `fparser-0.1.1/src/fparser/common/sourceinfo.py` & `fparser-0.1.2/src/fparser/common/sourceinfo.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/common/splitline.py` & `fparser-0.1.2/src/fparser/common/splitline.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/common/tests/conftest.py` & `fparser-0.1.2/src/fparser/common/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/common/tests/logging_utils.py` & `fparser-0.1.2/src/fparser/common/tests/logging_utils.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/common/tests/modfile.f95` & `fparser-0.1.2/src/fparser/common/tests/modfile.f95`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/common/tests/test_base_classes.py` & `fparser-0.1.2/src/fparser/common/tests/test_base_classes.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/common/tests/test_readfortran.py` & `fparser-0.1.2/src/fparser/common/tests/test_readfortran.py`

 * *Files 2% similar despite different names*

```diff
@@ -676,28 +676,54 @@
         if not orig_line:
             break
         reader.put_item(orig_line)
         fifo_line = reader.get_item()
         assert fifo_line == orig_line
 
 
-def test_put_item_include(ignore_comments):
+def test_put_item_include(ignore_comments, tmpdir):
     """Check that when a line that has been included via an include
     statement is consumed it can be pushed back so it can be consumed
     again. Test with and without ignoring comments.
 
     """
-    reader = FortranStringReader(FORTRAN_CODE, ignore_comments=ignore_comments)
+    _ = tmpdir.chdir()
+    cwd = str(tmpdir)
+    include_code = """
+    var1 = 1
+    var2 = 2
+    var3 = 3
+"""
+    with open(os.path.join(cwd, "my_include.h"), "w") as cfile:
+        cfile.write(include_code)
+    code = """
+program my_prog
+  integer :: var1, var2, var3
+  include 'my_include.h'
+end program my_prog
+"""
+    reader = FortranStringReader(code, ignore_comments=ignore_comments)
+    lines = []
     while True:
-        orig_line = reader.get_item()
-        if not orig_line:
+        lines.append(reader.get_item())
+        # Try immediately putting the line back and then requesting it again.
+        # This checks that the correct FIFO buffer is being used.
+        reader.put_item(lines[-1])
+        assert reader.get_item().line == lines[-1].line
+        if "var3 =" in lines[-1].line:
+            # Stop reading while we're still in the INCLUDE file so that we
+            # have a stack of readers when calling `put_item` below.
             break
-        reader.put_item(orig_line)
-        fifo_line = reader.get_item()
-        assert fifo_line == orig_line
+    # Put all the lines back in the same order that we saw them.
+    for line in reversed(lines):
+        reader.put_item(line)
+    # Check that the reader returns all those lines in the same order that
+    # we saw them originally.
+    for line in lines:
+        assert reader.get_item().line == line.line
 
 
 def test_multi_put_item(ignore_comments):
     """Check that multiple lines can be pushed back and will be returned
     correctly in the specified order (actually the reverse of the
     original). Test with and without ignoring comments.
```

### Comparing `fparser-0.1.1/src/fparser/common/tests/test_sourceinfo.py` & `fparser-0.1.2/src/fparser/common/tests/test_sourceinfo.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/common/tests/test_splitline.py` & `fparser-0.1.2/src/fparser/common/tests/test_splitline.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/common/tests/test_utils.py` & `fparser-0.1.2/src/fparser/common/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/common/tests/utf.f90` & `fparser-0.1.2/src/fparser/common/tests/utf.f90`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/common/tests/utf_in_code.f90` & `fparser-0.1.2/src/fparser/common/tests/utf_in_code.f90`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/common/utils.py` & `fparser-0.1.2/src/fparser/common/utils.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/conftest.py` & `fparser-0.1.2/src/fparser/conftest.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/one/block_statements.py` & `fparser-0.1.2/src/fparser/one/block_statements.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/one/parsefortran.py` & `fparser-0.1.2/src/fparser/one/parsefortran.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/one/statements.py` & `fparser-0.1.2/src/fparser/one/statements.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/one/tests/bad_char.f90` & `fparser-0.1.2/src/fparser/one/tests/bad_char.f90`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/one/tests/test_block_stmts.py` & `fparser-0.1.2/src/fparser/one/tests/test_block_stmts.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/one/tests/test_do_block_r814.py` & `fparser-0.1.2/src/fparser/one/tests/test_do_block_r814.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/one/tests/test_parsefortran.py` & `fparser-0.1.2/src/fparser/one/tests/test_parsefortran.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/one/tests/test_parser.py` & `fparser-0.1.2/src/fparser/one/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/one/tests/test_scripts.py` & `fparser-0.1.2/src/fparser/one/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/one/tests/test_select.py` & `fparser-0.1.2/src/fparser/one/tests/test_select.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/one/typedecl_statements.py` & `fparser-0.1.2/src/fparser/one/typedecl_statements.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/scripts/README.md` & `fparser-0.1.2/src/fparser/scripts/README.md`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/scripts/fparser2.py` & `fparser-0.1.2/src/fparser/scripts/fparser2.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/scripts/fparser2_bench.py` & `fparser-0.1.2/src/fparser/scripts/fparser2_bench.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/scripts/parse.py` & `fparser-0.1.2/src/fparser/scripts/parse.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/scripts/read.py` & `fparser-0.1.2/src/fparser/scripts/read.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/scripts/script_options.py` & `fparser-0.1.2/src/fparser/scripts/script_options.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/scripts/tests/test_fparser2_bench.py` & `fparser-0.1.2/src/fparser/scripts/tests/test_fparser2_bench.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/scripts/tests/test_scripts.py` & `fparser-0.1.2/src/fparser/scripts/tests/test_scripts.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/tests/funcfile.f95` & `fparser-0.1.2/src/fparser/tests/funcfile.f95`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/tests/modfile.f95` & `fparser-0.1.2/src/fparser/tests/modfile.f95`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/tests/test_api.py` & `fparser-0.1.2/src/fparser/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/tests/test_blank_lines.py` & `fparser-0.1.2/src/fparser/tests/test_blank_lines.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/tests/test_comment.py` & `fparser-0.1.2/src/fparser/tests/test_comment.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/tests/test_f90comment_f77source.py` & `fparser-0.1.2/src/fparser/tests/test_f90comment_f77source.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/tests/test_fparser_module.py` & `fparser-0.1.2/src/fparser/tests/test_fparser_module.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/tests/test_functional.py` & `fparser-0.1.2/src/fparser/tests/test_functional.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/tests/test_issue10.py` & `fparser-0.1.2/src/fparser/tests/test_issue10.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/tests/test_issue11.py` & `fparser-0.1.2/src/fparser/tests/test_issue11.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/tests/test_issue23.py` & `fparser-0.1.2/src/fparser/tests/test_issue23.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/tests/test_issue25.py` & `fparser-0.1.2/src/fparser/tests/test_issue25.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/tests/test_issue26.py` & `fparser-0.1.2/src/fparser/tests/test_issue26.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/tests/test_issue33.py` & `fparser-0.1.2/src/fparser/tests/test_issue33.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/tests/test_issue4.py` & `fparser-0.1.2/src/fparser/tests/test_issue4.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/tests/test_issue5.py` & `fparser-0.1.2/src/fparser/tests/test_issue5.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/tests/test_issue7.py` & `fparser-0.1.2/src/fparser/tests/test_issue7.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/tests/test_issue8.py` & `fparser-0.1.2/src/fparser/tests/test_issue8.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/tests/test_issue9.py` & `fparser-0.1.2/src/fparser/tests/test_issue9.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/tests/test_mod_private.py` & `fparser-0.1.2/src/fparser/tests/test_mod_private.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/C99Preprocessor.py` & `fparser-0.1.2/src/fparser/two/C99Preprocessor.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/Fortran2003.py` & `fparser-0.1.2/src/fparser/two/Fortran2003.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 #!/usr/bin/env python
 
-# Modified work Copyright (c) 2017-2022 Science and Technology
+# Modified work Copyright (c) 2017-2023 Science and Technology
 # Facilities Council.
 # Original work Copyright (c) 1999-2008 Pearu Peterson
 
 # All rights reserved.
 
 # Modifications made as part of the fparser project are distributed
 # under the following license:
@@ -4647,53 +4647,68 @@
         if self.items[1] is None:
             return str(self.items[0])
         return "%s - %s" % tuple(self.items)
 
 
 class Namelist_Stmt(StmtBase):  # R552
     """
-    ::
-
-        <namelist-stmt> = NAMELIST / <namelist-group-name> /
-            <namelist-group-object-list> [ [ , ] / <namelist-group-name> /
-            <namelist-group-object-list> ]...
-
-    Attributes::
+    Fortran 2003 rule R552::
 
-        items : (Namelist_Group_Name, Namelist_Group_Object_List)-tuple
+        namelist-stmt is NAMELIST
+                         / namelist-group-name / namelist-group-object-list
+                         [ [,] / namelist-group-name /
+                         namelist-group-object-list ] ...
 
     """
 
     subclass_names = []
     use_names = ["Namelist_Group_Name", "Namelist_Group_Object_List"]
 
     @staticmethod
     def match(string):
-        if string[:8].upper() != "NAMELIST":
-            return
-        line = string[8:].lstrip()
+        """Implements the matching for a Namelist_Stmt.
+
+        :param str string: a string containing the code to match.
+
+        :returns: `None` if there is no match, otherwise a `tuple` \
+            containing 2-tuples with a namelist name and a namelist object \
+            list.
+        :rtype: Optional[Tuple[Tuple[ \
+            fparser.two.Fortran2003.Namelist_Group_Name, \
+            fparser.two.Fortran2003.Namelist_Group_Object_List]]]
+
+        """
+        line = string.lstrip()
+        if line[:8].upper() != "NAMELIST":
+            return None
+        line = line[8:].lstrip()
+        if not line:
+            return None
         parts = line.split("/")
+        text_before_slash = parts.pop(0)
+        if text_before_slash:
+            return None
         items = []
-        fst = parts.pop(0)
-        assert not fst, repr((fst, parts))
         while len(parts) >= 2:
-            name, lst = parts[:2]
-            del parts[:2]
-            name = name.strip()
-            lst = lst.strip()
+            name = parts.pop(0).strip()
+            lst = parts.pop(0).strip()
             if lst.endswith(","):
                 lst = lst[:-1].rstrip()
             items.append((Namelist_Group_Name(name), Namelist_Group_Object_List(lst)))
-        assert not parts, repr(parts)
+        if parts:
+            # There is a missing second '/'
+            return None
         return tuple(items)
 
     def tostr(self):
-        return "NAMELIST " + ", ".join(
-            "/%s/ %s" % (name_lst) for name_lst in self.items
-        )
+        """
+        :returns: this Namelist_Stmt as a string.
+        :rtype: str
+        """
+        return "NAMELIST " + ", ".join(f"/{name}/ {lst}" for name, lst in self.items)
 
 
 class Namelist_Group_Object(Base):  # R553
     """
     ::
 
         <namelist-group-object> = <variable-name>
@@ -5245,15 +5260,15 @@
 class Allocate_Stmt(StmtBase):  # R623
     """
     Fortran2003 rule R623::
 
         allocate-stmt is ALLOCATE ( [ type-spec :: ] allocation-list
                                     [, alloc-opt-list ] )
 
-    Subject to the following constraints\:
+    Subject to the following constraints:
 
     C622 (R629) Each allocate-object shall be a nonprocedure pointer or an
                  allocatable variable.
     C623 (R623) If any allocate-object in the statement has a deferred type
                 parameter, either type-spec or SOURCE= shall appear.
     C624 (R623) If a type-spec appears, it shall specify a type with which
                 each allocate-object is type compatible.
@@ -7945,90 +7960,107 @@
         """
         :return: optional labeled "DO" statement name
         :rtype: string
         """
         return self.item.name
 
 
-class Loop_Control(Base):  # pylint: disable=invalid-name
+# pylint: disable=invalid-name
+class Loop_Control(Base):  # R830
     """
-    R830::
+    Fortran 2003 rule R830
 
-        <loop-control> = [ , ] <do-variable> = scalar-int-expr,
-                                               scalar-int-expr
-                                               [ , <scalar-int-expr> ]
-                         | [ , ] WHILE ( <scalar-logical-expr> )
+    loop-control is [ , ] do-variable = scalar-int-expr , scalar-int-expr
+                       [ , scalar-int-expr ]
+                    or [ , ] WHILE ( scalar-logical-expr )
+
+    This class would be better and more extensible if it called 2
+    classes, one for each of the above expressions. Something like the
+    suggestion below. However, this would result in a different
+    fparser tree, see issue #416.
+
+    F2003: While_Loop_Cntl: scalar-logical-expression, delim
+    F2003: Counter_Loop_Cntl: var, lower, upper, [step], delim
+    F2008: Concurrent_Loop_Cntl: conc_expr, delim
+    F2018: Concurrent_Loop_Cntl: conc_expr, local_x, delim
 
     """
 
     subclass_names = []
     use_names = ["Do_Variable", "Scalar_Int_Expr", "Scalar_Logical_Expr"]
 
     @staticmethod
     def match(string):
+        """Attempts to match the supplied text with this rule.
+
+        :param str string: Fortran code to check for a match.
+
+        :returns: None if there is no match, a 3-tuple with the first \
+            entry providing the result of matching the 'WHILE' part of \
+            the rule if there is a match, the second entry providing \
+            the result of matching the 'COUNTER' part of the rule if \
+            there is a match and the third entry indicating whether \
+            there is an optional preceding ','.
+        :rtype: Optional[Tuple[ \
+            Optional[ \
+                :py:class:`fparser.two.Fortran2003.Scalar_Logical_Expr`], \
+            Optional[Tuple[ \
+                :py:class:`fparser.two.Fortran2003.Do_Variable`, List[str]]], \
+            Optional[str]]]
+
         """
-        :param str string: Fortran code to check for a match
-        :return: 3-tuple containing strings and instances of the classes
-                 determining loop control (optional comma delimiter,
-                 optional scalar logical expression describing "WHILE"
-                 condition or optional counter expression containing loop
-                 counter and scalar integer expression)
-        :rtype: 3-tuple of objects or nothing for an "infinite loop"
-        """
-        # pylint: disable=unbalanced-tuple-unpacking
+        line = string.lstrip().rstrip()
+        # Try to match optional delimiter
         optional_delim = None
-        # Match optional delimiter
-        if string.startswith(","):
-            line, repmap = string_replace_map(string[1:].lstrip())
-            optional_delim = ", "
-        else:
-            line, repmap = string_replace_map(string)
-        # Match "WHILE" scalar logical expression
+        if line.startswith(","):
+            line = line[1:].lstrip()
+            optional_delim = ","
+        line, repmap = string_replace_map(line)
+        # Try to match with WHILE
         if line[:5].upper() == "WHILE" and line[5:].lstrip().startswith("("):
-            lbrak = line[5:].lstrip()
-            i = lbrak.find(")")
-            if i != -1 and i == len(lbrak) - 1:
-                scalar_logical_expr = Scalar_Logical_Expr(repmap(lbrak[1:i].strip()))
-                return scalar_logical_expr, None, optional_delim
-        # Match counter expression
-        # More than one '=' in counter expression
+            brackets = line[5:].lstrip()
+            rbrack_index = brackets.find(")")
+            if rbrack_index != -1 and rbrack_index == len(brackets) - 1:
+                scalar_logical_expr = Scalar_Logical_Expr(
+                    repmap(brackets[1:rbrack_index].strip())
+                )
+                return (scalar_logical_expr, None, optional_delim)
+        # Try to match counter expression
+        # More than one '=' in counter expression is not valid
         if line.count("=") != 1:
-            return
+            return None
         var, rhs = line.split("=")
-        rhs = [s.strip() for s in rhs.lstrip().split(",")]
+        rhs = [entry.strip() for entry in rhs.lstrip().split(",")]
         # Incorrect number of elements in counter expression
         if not 2 <= len(rhs) <= 3:
-            return
+            return None
         counter_expr = (
-            Variable(repmap(var.rstrip())),
+            Do_Variable(repmap(var.rstrip())),
             list(map(Scalar_Int_Expr, list(map(repmap, rhs)))),
         )
-        return None, counter_expr, optional_delim
+        return (None, counter_expr, optional_delim)
 
     def tostr(self):
         """
-        :return: parsed representation of loop control construct
-        :rtype: string
+        :returns: the Fortran representation of this object.
+        :rtype: str
         """
-        # pylint: disable=unbalanced-tuple-unpacking
-        scalar_logical_expr, counter_expr, optional_delim = self.items
-        # Return loop control construct containing "WHILE" condition and
-        # its <scalar-logical-expr>
-        if scalar_logical_expr is not None:
-            loopctrl = "WHILE (%s)" % scalar_logical_expr
-        # Return loop control construct containing counter expression:
-        # <do-variable> as LHS and <scalar-int-expr> list as RHS
-        elif counter_expr[0] is not None and counter_expr[1] is not None:
-            loopctrl = "%s = %s" % (
-                counter_expr[0],
-                ", ".join(map(str, counter_expr[1])),
+        if self.items[0]:
+            # Return loop control construct containing "WHILE" condition and
+            # its <scalar-logical-expr>
+            loopctrl = f"WHILE ({self.items[0]})"
+        else:  # counter expression
+            # Return loop control construct containing counter expression:
+            # <do-variable> as LHS and <scalar-int-expr> list as RHS
+            loopctrl = (
+                f"{self.items[1][0]} = " f"{', '.join(map(str, self.items[1][1]))}"
             )
         # Add optional delimiter to loop control construct if present
-        if optional_delim is not None:
-            loopctrl = optional_delim + loopctrl
+        if self.items[2]:
+            loopctrl = f"{self.items[2]} {loopctrl}"
         return loopctrl
 
 
 class Do_Variable(Base):  # pylint: disable=invalid-name
     """
     R831::
```

### Comparing `fparser-0.1.1/src/fparser/two/Fortran2008.py` & `fparser-0.1.2/src/fparser/two/Fortran2008/Fortran2008.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,17 +71,14 @@
 # pylint: disable=arguments-differ
 # pylint: disable=undefined-variable
 # pylint: disable=eval-used
 # These warnings are due to the auto-generation of classes when this
 # module is first imported.
 # pylint: disable=exec-used
 # pylint: disable=unused-import
-import inspect
-import sys
-
 from fparser.common.splitline import string_replace_map, splitparen
 from fparser.two import pattern_tools as pattern
 from fparser.two.utils import (
     BracketBase,
     CALLBase,
     KeywordValueBase,
     NoMatchError,
@@ -89,26 +86,30 @@
     SeparatorBase,
     StmtBase,
     STRINGBase,
     Type_Declaration_StmtBase,
     WORDClsBase,
 )
 
+# These pylint errors are due to the auto-generation of classes in the
+# Fortran2003 file.
+# pylint: disable=no-name-in-module
 from fparser.two.Fortran2003 import (
     Base,
     BlockBase,
     Component_Decl_List,
     Declaration_Construct,
     Declaration_Type_Spec,
     EndStmtBase,
     Entity_Decl_List,
     Errmsg_Variable,
     Execution_Part_Construct,
     File_Name_Expr,
     File_Unit_Number,
+    Forall_Header,
     Implicit_Part,
     Implicit_Part_Stmt,
     Import_Stmt,
     Iomsg_Variable,
     Label,
     Module_Subprogram_Part,
     Name,
@@ -116,14 +117,16 @@
     Source_Expr,
     Specification_Part,
     Stat_Variable,
     Stop_Code,
     Use_Stmt,
 )
 
+# pylint: enable=no-name-in-module
+
 # Import of F2003 classes that are updated in this standard.
 from fparser.two.Fortran2003 import (
     Action_Stmt as Action_Stmt_2003,
     Action_Stmt_C201 as Action_Stmt_C201_2003,
     Action_Stmt_C802 as Action_Stmt_C802_2003,
     Action_Stmt_C824 as Action_Stmt_C824_2003,
     Alloc_Opt as Alloc_Opt_2003,
@@ -132,14 +135,15 @@
     Component_Attr_Spec as Component_Attr_Spec_2003,
     Connect_Spec as Connect_Spec_2003,
     Data_Component_Def_Stmt as Data_Component_Def_Stmt_2003,
     Do_Term_Action_Stmt as Do_Term_Action_Stmt_2003,
     Executable_Construct as Executable_Construct_2003,
     Executable_Construct_C201 as Executable_Construct_C201_2003,
     If_Stmt as If_Stmt_2003,
+    Loop_Control as Loop_Control_2003,
     Open_Stmt as Open_Stmt_2003,
     Procedure_Stmt as Procedure_Stmt_2003,
     Program_Unit as Program_Unit_2003,
     Type_Declaration_Stmt as Type_Declaration_Stmt_2003,
 )
 
 
@@ -383,14 +387,18 @@
                  list if there is a match or None if there is no match.
         :rtype: `NoneType` or \
             (:py:class:`fparser.two.Fortran2003.Declaration_Type_Spec`, \
              :py:class:`fparser.two.Fortran2008.Component_Attr_Spec_List`, \
              :py:class:`fparser.two.Fortran2003.Component_Decl_List`)
 
         """
+        # Avoid circular dependencies by importing here.
+        # pylint: disable=import-outside-toplevel
+        from fparser.two.Fortran2008 import Component_Attr_Spec_List
+
         return Type_Declaration_StmtBase.match(
             Declaration_Type_Spec, Component_Attr_Spec_List, Component_Decl_List, string
         )
 
 
 class Component_Attr_Spec(Component_Attr_Spec_2003):  # R437
     """
@@ -450,14 +458,18 @@
     @staticmethod
     def get_attr_spec_list_cls():
         """Return the type used to match the attr-spec-list
 
         This overwrites the Fortran 2003 type with the Fortran 2008 variant.
 
         """
+        # Avoid circular dependencies by importing here.
+        # pylint: disable=import-outside-toplevel
+        from fparser.two.Fortran2008 import Attr_Spec_List
+
         return Attr_Spec_List
 
 
 class Codimension_Attr_Spec(WORDClsBase):  # R502.d
     """
     codimension-attr-spec is CODIMENSION lbracket coarray-spec rbracket
 
@@ -641,14 +653,18 @@
                  containing matched coshape-spec-list or `None` and \
                  matched lower-cobound or `None`.
         :rtype: `NoneType` or \
             (:py:class:`fparser.two.Fortran2008.Coshape_Spec_List` or `None`, \
              :py:class:`fparser.two:Fortran2008.Lower_Cobound` or `None`)
 
         """
+        # Avoid circular dependencies by importing here.
+        # pylint: disable=import-outside-toplevel
+        from fparser.two.Fortran2008 import Coshape_Spec_List
+
         if not string.endswith("*"):
             return None
         line = string[:-1].rstrip()
         if not line:
             return (None, None)
         if line.endswith(":"):
             line, repmap = string_replace_map(line[:-1].rstrip())
@@ -810,17 +826,105 @@
 
     @classmethod
     def alloc_opt_list(cls):
         """
         :returns: the Fortran2008 flavour of Alloc_Opt_List.
         :rtype: type
         """
+        # Avoid circular dependencies by importing here.
+        # pylint: disable=import-outside-toplevel
+        from fparser.two.Fortran2008 import Alloc_Opt_List
+
         return Alloc_Opt_List
 
 
+class Loop_Control(Loop_Control_2003):  # R818
+    """Fortran 2008 rule R818
+
+    loop-control is [ , ] do-variable = scalar-int-expr , scalar-int-expr
+                       [ , scalar-int-expr ]
+                    or [ , ] WHILE ( scalar-logical-expr )
+                    or [ , ] CONCURRENT forall-header
+
+    Extends the Fortran2003 rule R830 with the additional CONCURRENT clause.
+
+    The F2003 Loop_Control class would be better and more extensible
+    if it called 2 classes, one for each of the above
+    expressions. This would then affect the implementation of this
+    class. Something like the suggestion below. However, this would
+    result in a different fparser tree, see issue #416.
+
+    F2003: While_Loop_Cntl: scalar-logical-expression, delim
+    F2003: Counter_Loop_Cntl: var, lower, upper, [step], delim
+    F2008: Concurrent_Loop_Cntl: conc_expr, delim
+    F2018: Concurrent_Loop_Cntl: conc_expr, local_x, delim
+
+    """
+
+    subclass_names = []
+    # This class' match method makes use of the Fortran2003 match
+    # method so 'use_names' should include any classes used within
+    # there as well as any used here.
+    use_names = Loop_Control_2003.use_names[:]
+    use_names.append("Forall_Header")
+
+    @staticmethod
+    def match(string):
+        """Attempts to match the supplied text with this rule.
+
+        :param str string: Fortran code to check for a match.
+
+        :returns: None if there is no match, a tuple with the first \
+            entry providing the result of matching the 'WHILE' part of \
+            the rule if there is a match, the second entry providing \
+            the result of matching the 'COUNTER' part of the rule if \
+            there is a match, the third entry indicating whether \
+            there is an optional preceding ',' and the fourth entry \
+            providing the result of matching the 'CONCURRENT' part of \
+            the rule if there is a match.
+
+        :rtype: Optional[Tuple[ \
+            Optional[ \
+                :py:class:`fparser.two.Fortran2003.Scalar_Logical_Expr`], \
+            Optional[Tuple[ \
+                :py:class:`fparser.two.Fortran2003.Do_Variable`, List[str]]], \
+            Optional[str], \
+            Optional[:py:class:`fparser.two.Fortran2003.Forall_Header`]]]
+
+        """
+        # Fortran2003 matches all but CONCURRENT so try this first
+        result = Loop_Control_2003.match(string)
+        if result:
+            return result + (None,)
+        # Try to match with CONCURRENT
+        line = string.lstrip()
+        optional_delim = None
+        if line.startswith(","):
+            line = line[1:].lstrip()
+            optional_delim = ","
+        if line[:10].upper() != "CONCURRENT":
+            return None
+        return (None, None, optional_delim, Forall_Header(line[10:].lstrip().rstrip()))
+
+    def tostr(self):
+        """
+        :returns: the Fortran representation of this object.
+        :rtype: str
+        """
+        if self.items[0] or self.items[1]:
+            # Use the F2003 tostr() implementation
+            return Loop_Control_2003.tostr(self)
+        # Return loop control construct containing "CONCURRENT" clause
+        loopctrl = f"CONCURRENT {self.items[3]}"
+        # Add optional delimiter to loop control construct if present
+        if self.items[2]:
+            loopctrl = f"{self.items[2]} {loopctrl}"
+        return loopctrl
+
+
 class If_Stmt(If_Stmt_2003):  # R837
     """
     Fortran 2008 rule R837
     if-stmt is IF ( scalar-logical-expr ) action-stmt
 
     The implementation of this rule only replaces the :py:attr:`use_names` and
     :py:attr:`action_stmt_class` attributes to use the Fortran 2008 variant
@@ -1052,14 +1156,18 @@
 
         :returns: instances of the Classes that have matched if there is a \
                   match or `None` if there is no match.
         :rtype: Optional[Tuple[:py:class:`fparser.two.Fortran2008.Parent_Identifier`, \
                                :py:class:`fparser.two.Fortran2008.Submodule_Name`]]
 
         """
+        # Avoid circular dependencies by importing here.
+        # pylint: disable=import-outside-toplevel
+        from fparser.two.Fortran2008 import Submodule_Name
+
         # First look for "SUBMODULE"
         name = "SUBMODULE"
         if fstring[: len(name)].upper() != name:
             # the string does not start with SUBMODULE so does not
             # match
             return None
         # "SUBMODULE is found so strip it out and split the remaining
@@ -1123,14 +1231,18 @@
         param string fstring : contains the Fortran that we are trying
         to match
 
         :return: instances of the Classes that have matched if there
         is a match or `None` if there is no match
 
         """
+        # Avoid circular dependencies by importing here.
+        # pylint: disable=import-outside-toplevel
+        from fparser.two.Fortran2008 import Submodule_Name
+
         return EndStmtBase.match("SUBMODULE", Submodule_Name, fstring)
 
     def get_name(self):  # C1114
         """Fortran 2008 constraint C1114 return the submodule name as
         specified by the end submodule statement or `None` if one is
         not specified. This is used by the base class to check whether
         this name matches the submodule name.
@@ -1164,14 +1276,18 @@
         param string fstring : contains the Fortran that we are trying
         to match
 
         :return: instances of the Classes that have matched if there
         is a match or `None` if there is no match
 
         """
+        # Avoid circular dependencies by importing here.
+        # pylint: disable=import-outside-toplevel
+        from fparser.two.Fortran2008 import Ancestor_Module_Name, Parent_SubModule_Name
+
         split_string = fstring.split(":")
         len_split_string = len(split_string)
         lhs_name = split_string[0].lstrip().rstrip()
         if len_split_string == 1:
             return Ancestor_Module_Name(lhs_name), None
         if len_split_string == 2:
             rhs_name = split_string[1].lstrip().rstrip()
@@ -1205,16 +1321,18 @@
 
         :param str string: the string to attempt to match.
 
         :returns: a new Open_Stmt object if the match is successful, None otherwise.
         :rtype: Optional[:py:class:`fparser.two.Fortran2008.Open_Stmt]
 
         """
-        # The Connect_Spec_List class is generated automatically
-        # by code at the end of this module
+        # Avoid circular dependencies by importing here.
+        # pylint: disable=import-outside-toplevel
+        from fparser.two.Fortran2008 import Connect_Spec_List
+
         obj = CALLBase.match("OPEN", Connect_Spec_List, string, require_rhs=True)
         if not obj:
             return None
 
         # Apply constraints now that we have the full Connect_Spec_List.
         have_unit = False
         have_newunit = False
@@ -1301,14 +1419,22 @@
         """
         :param str string: Fortran code to check for a match
 
         :returns: 2-tuple containing the keyword and value or None if the
                   supplied string is not a match
         :rtype: Optional[Tuple[str, Any]]
         """
+        # Avoid circular dependencies by importing here.
+        # pylint: disable=import-outside-toplevel
+        from fparser.two.Fortran2008 import (
+            Scalar_Default_Char_Expr,
+            Scalar_Int_Variable,
+            Scalar_Int_Expr,
+        )
+
         if "=" not in string:
             # The only argument which need not be named is the unit number
             return "UNIT", File_Unit_Number(string)
         # We have a keyword-value pair. Check whether it is valid...
         for keyword, value in [
             (
                 [
@@ -1464,14 +1590,18 @@
         :return: 2-tuple containing "BLOCK" and, optionally, an associated \
             Name or None if no match.
         :rtype: Optional[Tuple[
             str,
             Optional[:py:class:`fparser.two.Fortran2003.Block_Construct_Name`]]]
 
         """
+        # Avoid circular dependencies by importing here.
+        # pylint: disable=import-outside-toplevel
+        from fparser.two.Fortran2008 import Block_Construct_Name
+
         return EndStmtBase.match(
             "BLOCK", Block_Construct_Name, string, require_stmt_type=True
         )
 
 
 class Critical_Construct(BlockBase):
     """
@@ -1570,14 +1700,18 @@
         :returns: 2-tuple containing "CRITICAL" and, optionally, an associated \
             Name or None if there is no match.
         :rtype: Optional[Tuple[
             str, \
             Optional[:py:class:`fparser.two.Fortran2003.Critical_Construct_Name`]]]
 
         """
+        # Avoid circular dependencies by importing here.
+        # pylint: disable=import-outside-toplevel
+        from fparser.two.Fortran2008 import Critical_Construct_Name
+
         return EndStmtBase.match(
             "CRITICAL", Critical_Construct_Name, string, require_stmt_type=True
         )
 
 
 class Procedure_Stmt(Procedure_Stmt_2003):  # R1206
     """
@@ -1596,14 +1730,18 @@
             whether the optional '::' is included and a Procedure_Name_List \
             instance, or None if there is no match.
         :rtype: Optional[Tuple[ \
             bool, bool, \
             :py:class:`fparser.two.Fortran2003.Procedure_Name_List`]]]
 
         """
+        # Avoid circular dependencies by importing here.
+        # pylint: disable=import-outside-toplevel
+        from fparser.two.Fortran2008 import Procedure_Name_List
+
         line = string.lstrip()
         optional_module = None
         if line[:6].upper() == "MODULE":
             line = line[6:].lstrip()
             optional_module = "MODULE"
         if line[:9].upper() != "PROCEDURE":
             return None
@@ -1621,71 +1759,7 @@
         """
         result = "PROCEDURE"
         if self.items[1]:
             result = f"MODULE {result}"
         if self.items[2]:
             result = f"{result} ::"
         return f"{result} {self.items[0]}"
-
-
-#
-# GENERATE Scalar_, _List, _Name CLASSES
-#
-
-
-ClassType = type(Base)
-_names = dir()
-for clsname in _names:
-    new_cls = eval(clsname)
-    if not (
-        isinstance(new_cls, ClassType)
-        and issubclass(new_cls, Base)
-        and not new_cls.__name__.endswith("Base")
-    ):
-        continue
-
-    names = getattr(new_cls, "subclass_names", []) + getattr(new_cls, "use_names", [])
-    for n in names:
-        if n in _names:
-            continue
-        if n.endswith("_List"):
-            _names.append(n)
-            n = n[:-5]
-            # Generate 'list' class
-            exec(
-                f"""\
-class {n}_List(SequenceBase):
-    subclass_names = [\'{n}\']
-    use_names = []
-    @staticmethod
-    def match(string): return SequenceBase.match(r\',\', {n}, string)
-"""
-            )
-        elif n.endswith("_Name"):
-            _names.append(n)
-            n = n[:-5]
-            exec(
-                f"""\
-class {n}_Name(Base):
-    subclass_names = [\'Name\']
-"""
-            )
-        elif n.startswith("Scalar_"):
-            _names.append(n)
-            n = n[7:]
-            exec(
-                f"""\
-class Scalar_{n}(Base):
-    subclass_names = [\'{n}\']
-"""
-            )
-
-
-# Inspect the contents of this module and list all of the classes in __all__
-# for automatic documentation generation with AutoDoc.
-
-classes = inspect.getmembers(
-    sys.modules[__name__],
-    lambda member: inspect.isclass(member) and member.__module__ == __name__,
-)
-
-__all__ = [name[0] for name in classes]
```

### Comparing `fparser-0.1.1/src/fparser/two/parser.py` & `fparser-0.1.2/src/fparser/two/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -146,15 +146,17 @@
             # and Fortran2008 files and then ensure that where classes
             # have the same name we return the Fortran2008 class
             # i.e. where Fortran2008 extends Fortran2003 we return
             # Fortran2008.
             # First find all Fortran2008 classes.
             from fparser.two import Fortran2008
 
-            f2008_cls_members = get_module_classes(Fortran2008)
+            f2008_cls_members = inspect.getmembers(
+                sys.modules[Fortran2008.__name__], inspect.isclass
+            )
 
             # next add in Fortran2003 classes if they do not already
             # exist as a Fortran2008 class.
             f2008_class_names = [i[0] for i in f2008_cls_members]
             for local_cls in f2003_cls_members:
                 if local_cls[0] not in f2008_class_names:
                     f2008_cls_members.append(local_cls)
```

### Comparing `fparser-0.1.1/src/fparser/two/pattern_tools.py` & `fparser-0.1.2/src/fparser/two/pattern_tools.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/symbol_table.py` & `fparser-0.1.2/src/fparser/two/symbol_table.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/.pylintrc` & `fparser-0.1.2/src/fparser/two/tests/.pylintrc`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/conftest.py` & `fparser-0.1.2/src/fparser/two/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/conftest.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/conftest.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_add_operand_r705.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_add_operand_r705.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_allocate_stmt_r623.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_allocate_stmt_r623.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_array_constructor_implied_do_ctl_r471.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_array_constructor_implied_do_ctl_r471.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_array_constructor_implied_do_r470.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_array_constructor_implied_do_r470.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_array_constructor_r465.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_array_constructor_r465.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_array_constructor_spec_r466.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_array_constructor_spec_r466.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_associate_construct_r816.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_associate_construct_r816.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_block_do_construct_r826.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_block_do_construct_r826.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_case_construct_r808.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_case_construct_r808.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_char_expr_r725.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_char_expr_r725.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_char_literal_constant_r427.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_char_literal_constant_r427.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_component_part_r438.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_component_part_r438.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_control_edit_descriptor_r1011.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_control_edit_descriptor_r1011.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_cray_pointee_array_spec.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_cray_pointee_array_spec.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_cray_pointee_decl.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_cray_pointee_decl.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_cray_pointer_decl.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_cray_pointer_decl.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_cray_pointer_stmt.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_cray_pointer_stmt.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_data_edit_desc_c1002.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_data_edit_desc_c1002.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_data_ref_r612.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_data_ref_r612.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_declaration_construct_r207.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_declaration_construct_r207.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_default_char_expr_r726.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_default_char_expr_r726.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_defined_operator_r311.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_defined_operator_r311.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_defined_operators_r703_r723.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_defined_operators_r703_r723.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_derived_type_stmt_r430.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_derived_type_stmt_r430.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_designator_r603.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_designator_r603.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_entity_decl_r504.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_entity_decl_r504.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_executable_construct_r213.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_executable_construct_r213.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_extended_intrinsic_op_r312.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_extended_intrinsic_op_r312.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_forall_header_r754.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_forall_header_r754.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_forall_stmt_r759.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_forall_stmt_r759.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_format_item_c1002.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_format_item_c1002.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_format_item_list.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_format_item_list.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_format_item_r1003.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_format_item_r1003.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_format_specification_r1002.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_format_specification_r1002.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_function_stmt_r1224.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_function_stmt_r1224.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_hollerith_item.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_hollerith_item.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_if_construct_r802.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_if_construct_r802.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_if_stmt_r807.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_if_stmt_r807.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_import_stmt_r1209.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_import_stmt_r1209.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_include_filename.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_include_filename.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_include_statement.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_include_statement.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_int_expr_r727.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_int_expr_r727.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_intrinsics.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_intrinsics.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_io_control_spec_r913.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_io_control_spec_r913.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_kindselector_r404.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_kindselector_r404.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_level_2_expr_r706.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_level_2_expr_r706.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_logical_expr_r724.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_logical_expr_r724.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_main_program_r1101.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_main_program_r1101.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_module_r1104.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_module_r1104.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_name_r304.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_name_r304.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_nonblock_do_construct_r835.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_nonblock_do_construct_r835.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_numeric_expr_r728.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_numeric_expr_r728.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_position_edit_desc_r1013.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_position_edit_desc_r1013.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_prefix_r1227.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_prefix_r1227.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_primary_r701.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_primary_r701.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_program_r201.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_program_r201.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_program_stmt_r1102.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_program_stmt_r1102.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_rename_r1111.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_rename_r1111.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_select_type_construct_r821.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_select_type_construct_r821.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_specific_binding_r451.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_specific_binding_r451.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_stmt_function_stmt_r1238.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_stmt_function_stmt_r1238.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_subroutine_stmt_r1232.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_subroutine_stmt_r1232.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_type_decl_stmt_r501.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_type_decl_stmt_r501.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_usestmt_r1109.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_usestmt_r1109.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_where_construct_r744.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_where_construct_r744.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2003/test_write_stmt_r911.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2003/test_write_stmt_r911.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2008/conftest.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2008/conftest.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_action_stmt_r214.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2008/test_action_stmt_r214.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_alloc_opt_r627.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2008/test_alloc_opt_r627.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_attr_spec_r502.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2008/test_attr_spec_r502.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_block.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2008/test_block.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_coarray_spec_r509.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2008/test_coarray_spec_r509.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_component_attr_spec_r437.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2008/test_component_attr_spec_r437.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_critical.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2008/test_critical.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_data_component_def_stmt_r436.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2008/test_data_component_def_stmt_r436.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_deferred_coshape_spec_r510.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2008/test_deferred_coshape_spec_r510.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_end_submodule_stmt_r1119.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2008/test_end_submodule_stmt_r1119.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_error_stop_stmt_r856.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2008/test_error_stop_stmt_r856.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_explicit_coshape_spec_r511.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2008/test_explicit_coshape_spec_r511.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_if_stmt_r837.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2008/test_if_stmt_r837.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_lower_cobound_r512.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2008/test_lower_cobound_r512.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_open_stmt_r904.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2008/test_open_stmt_r904.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_parent_identifier_r1118.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2008/test_parent_identifier_r1118.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_procedure_stmt_r1206.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2008/test_procedure_stmt_r1206.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_program_unit_r202.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2008/test_program_unit_r202.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_submodule_r1116.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2008/test_submodule_r1116.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_submodule_stmt_r1117.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2008/test_submodule_stmt_r1117.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,17 @@
 def test_splitparen_error(monkeypatch):
     """Test that if the first argument of the splitparen is not empty then
     an error is returned.
 
     """
     # We must monkeypatch the splitparen function that has already been
     # imported into the F2008 module.
-    monkeypatch.setattr("fparser.two.Fortran2008.splitparen", lambda x: ["XXX", "", ""])
+    monkeypatch.setattr(
+        "fparser.two.Fortran2008.Fortran2008.splitparen", lambda x: ["XXX", "", ""]
+    )
     with pytest.raises(NoMatchError) as excinfo:
         dummy_ = Submodule_Stmt("submodule (id) name")
     assert "Submodule_Stmt: 'submodule (id) name'" in str(excinfo.value)
 
 
 def test_simple_error9():
     """Test the parsing of a submodule statement"""
```

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_type_declaration_stmt_r501.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2008/test_type_declaration_stmt_r501.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/fortran2008/test_upper_cobound_r513.py` & `fparser-0.1.2/src/fparser/two/tests/fortran2008/test_upper_cobound_r513.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/test_bases.py` & `fparser-0.1.2/src/fparser/two/tests/test_bases.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/test_c99preprocessor.py` & `fparser-0.1.2/src/fparser/two/tests/test_c99preprocessor.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/test_comments.py` & `fparser-0.1.2/src/fparser/two/tests/test_comments.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/test_fortran2003.py` & `fparser-0.1.2/src/fparser/two/tests/test_fortran2003.py`

 * *Files 0% similar despite different names*

```diff
@@ -1390,24 +1390,14 @@
     assert repr(obj) == "Letter_Spec('A', 'Z')"
 
     obj = tcls("d")
     assert isinstance(obj, tcls), repr(obj)
     assert str(obj) == "D"
 
 
-def test_namelist_stmt():  # R552
-    tcls = Namelist_Stmt
-    obj = tcls("namelist / nlist / a")
-    assert isinstance(obj, tcls), repr(obj)
-    assert str(obj) == "NAMELIST /nlist/ a"
-
-    obj = tcls("namelist / nlist / a, /mlist/ b,c /klist/ d,e")
-    assert str(obj) == "NAMELIST /nlist/ a, /mlist/ b, c, /klist/ d, e"
-
-
 def test_equivalence_stmt():  # R554
     tcls = Equivalence_Stmt
     obj = tcls("equivalence (a, b ,z)")
     assert isinstance(obj, tcls), repr(obj)
     assert str(obj) == "EQUIVALENCE(a, b, z)"
     assert (
         repr(obj) == "Equivalence_Stmt('EQUIVALENCE', Equivalence_Set_List(',', "
@@ -2109,34 +2099,14 @@
     tcls = Label_Do_Stmt
     obj = tcls("do 12")
     assert isinstance(obj, tcls), repr(obj)
     assert str(obj) == "DO 12"
     assert repr(obj) == "Label_Do_Stmt(None, Label('12'), None)"
 
 
-def test_loop_control():
-    """Tests incorrect loop control constructs (R829). Correct loop
-    control constructs are tested in test_block_label_do_construct()
-    and test_nonblock_label_do_construct()."""
-    tcls = Loop_Control
-
-    # More than one '=' in counter expression
-    with pytest.raises(NoMatchError) as excinfo:
-        _ = tcls("j = 1 = 10")
-    assert "Loop_Control: 'j = 1 = 10'" in str(excinfo.value)
-
-    # Incorrect number of elements in counter expression
-    with pytest.raises(NoMatchError) as excinfo:
-        _ = tcls("k = 10, -10, -2, -1")
-    assert "Loop_Control: 'k = 10, -10, -2, -1'" in str(excinfo.value)
-    with pytest.raises(NoMatchError) as excinfo:
-        _ = tcls("l = 5")
-    assert "Loop_Control: 'l = 5'" in str(excinfo.value)
-
-
 def test_continue_stmt():  # R848
     tcls = Continue_Stmt
     obj = tcls("continue")
     assert isinstance(obj, tcls), repr(obj)
     assert str(obj) == "CONTINUE"
     assert repr(obj) == "Continue_Stmt('CONTINUE')"
```

### Comparing `fparser-0.1.1/src/fparser/two/tests/test_module_use.py` & `fparser-0.1.2/src/fparser/two/tests/test_module_use.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/test_parser.py` & `fparser-0.1.2/src/fparser/two/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/test_pattern_tools.py` & `fparser-0.1.2/src/fparser/two/tests/test_pattern_tools.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/test_symbol_table.py` & `fparser-0.1.2/src/fparser/two/tests/test_symbol_table.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/test_symbol_tables.py` & `fparser-0.1.2/src/fparser/two/tests/test_symbol_tables.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/test_utils.py` & `fparser-0.1.2/src/fparser/two/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/utils/test_base.py` & `fparser-0.1.2/src/fparser/two/tests/utils/test_base.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/utils/test_binaryopbase.py` & `fparser-0.1.2/src/fparser/two/tests/utils/test_binaryopbase.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/utils/test_blockbase.py` & `fparser-0.1.2/src/fparser/two/tests/utils/test_blockbase.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/utils/test_bracket_base.py` & `fparser-0.1.2/src/fparser/two/tests/utils/test_bracket_base.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/utils/test_call_base.py` & `fparser-0.1.2/src/fparser/two/tests/utils/test_call_base.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/utils/test_get_child.py` & `fparser-0.1.2/src/fparser/two/tests/utils/test_get_child.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/utils/test_sequencebase.py` & `fparser-0.1.2/src/fparser/two/tests/utils/test_sequencebase.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/utils/test_stringbase_upper.py` & `fparser-0.1.2/src/fparser/two/tests/utils/test_stringbase_upper.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/utils/test_walk.py` & `fparser-0.1.2/src/fparser/two/tests/utils/test_walk.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/tests/utils/test_wordclsbase.py` & `fparser-0.1.2/src/fparser/two/tests/utils/test_wordclsbase.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser/two/utils.py` & `fparser-0.1.2/src/fparser/two/utils.py`

 * *Files identical despite different names*

### Comparing `fparser-0.1.1/src/fparser.egg-info/PKG-INFO` & `fparser-0.1.2/src/fparser.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fparser
-Version: 0.1.1
+Version: 0.1.2
 Summary: The fparser project
 Home-page: https://github.com/stfc/fparser
 Author: Pearu Peterson, Rupert Ford, Andrew Porter
 Author-email: andrew.porter@stfc.ac.uk
 License: BSD 3-Clause License
 Project-URL: Source, https://github.com/stfc/fparser
 Project-URL: Tracker, https://github.com/stfc/fparser/issues
@@ -25,14 +25,16 @@
 Description-Content-Type: text/markdown
 Provides-Extra: doc
 Provides-Extra: tests
 License-File: LICENSE
 
 # News #
 
+  * 28/04/2023 Version 0.1.1 released (extends F2008 support with the optional
+    "::" in the MODULE PROCEDURE statement).
   * 18/04/2023 Version 0.1.0 released and status changed from `alpha` to `beta`. See the [CHANGELOG](CHANGELOG.md) for more details.
   * 16/06/2022 Version 0.0.16 released. See the [CHANGELOG](CHANGELOG.md)
     for details.
   * 30/05/2022 Version 0.0.15 released. See the [CHANGELOG](CHANGELOG.md)
     for details.
   * 10/03/2022 Version 0.0.14 released. See the [CHANGELOG](CHANGELOG.md)
     for details.
```

### Comparing `fparser-0.1.1/src/fparser.egg-info/SOURCES.txt` & `fparser-0.1.2/src/fparser.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -95,20 +95,21 @@
 src/fparser/tests/test_issue5.py
 src/fparser/tests/test_issue7.py
 src/fparser/tests/test_issue8.py
 src/fparser/tests/test_issue9.py
 src/fparser/tests/test_mod_private.py
 src/fparser/two/C99Preprocessor.py
 src/fparser/two/Fortran2003.py
-src/fparser/two/Fortran2008.py
 src/fparser/two/__init__.py
 src/fparser/two/parser.py
 src/fparser/two/pattern_tools.py
 src/fparser/two/symbol_table.py
 src/fparser/two/utils.py
+src/fparser/two/Fortran2008/Fortran2008.py
+src/fparser/two/Fortran2008/__init__.py
 src/fparser/two/tests/.pylintrc
 src/fparser/two/tests/conftest.py
 src/fparser/two/tests/test_bases.py
 src/fparser/two/tests/test_c99preprocessor.py
 src/fparser/two/tests/test_comments.py
 src/fparser/two/tests/test_fortran2003.py
 src/fparser/two/tests/test_module_use.py
@@ -161,17 +162,19 @@
 src/fparser/two/tests/fortran2003/test_include_statement.py
 src/fparser/two/tests/fortran2003/test_int_expr_r727.py
 src/fparser/two/tests/fortran2003/test_intrinsics.py
 src/fparser/two/tests/fortran2003/test_io_control_spec_r913.py
 src/fparser/two/tests/fortran2003/test_kindselector_r404.py
 src/fparser/two/tests/fortran2003/test_level_2_expr_r706.py
 src/fparser/two/tests/fortran2003/test_logical_expr_r724.py
+src/fparser/two/tests/fortran2003/test_loop_control_r830.py
 src/fparser/two/tests/fortran2003/test_main_program_r1101.py
 src/fparser/two/tests/fortran2003/test_module_r1104.py
 src/fparser/two/tests/fortran2003/test_name_r304.py
+src/fparser/two/tests/fortran2003/test_namelist_stmt_r552.py
 src/fparser/two/tests/fortran2003/test_nonblock_do_construct_r835.py
 src/fparser/two/tests/fortran2003/test_numeric_expr_r728.py
 src/fparser/two/tests/fortran2003/test_position_edit_desc_r1013.py
 src/fparser/two/tests/fortran2003/test_prefix_r1227.py
 src/fparser/two/tests/fortran2003/test_primary_r701.py
 src/fparser/two/tests/fortran2003/test_program_r201.py
 src/fparser/two/tests/fortran2003/test_program_stmt_r1102.py
@@ -194,14 +197,15 @@
 src/fparser/two/tests/fortran2008/test_critical.py
 src/fparser/two/tests/fortran2008/test_data_component_def_stmt_r436.py
 src/fparser/two/tests/fortran2008/test_deferred_coshape_spec_r510.py
 src/fparser/two/tests/fortran2008/test_end_submodule_stmt_r1119.py
 src/fparser/two/tests/fortran2008/test_error_stop_stmt_r856.py
 src/fparser/two/tests/fortran2008/test_explicit_coshape_spec_r511.py
 src/fparser/two/tests/fortran2008/test_if_stmt_r837.py
+src/fparser/two/tests/fortran2008/test_loop_control_r818.py
 src/fparser/two/tests/fortran2008/test_lower_cobound_r512.py
 src/fparser/two/tests/fortran2008/test_open_stmt_r904.py
 src/fparser/two/tests/fortran2008/test_parent_identifier_r1118.py
 src/fparser/two/tests/fortran2008/test_procedure_stmt_r1206.py
 src/fparser/two/tests/fortran2008/test_program_unit_r202.py
 src/fparser/two/tests/fortran2008/test_submodule_r1116.py
 src/fparser/two/tests/fortran2008/test_submodule_stmt_r1117.py
```

