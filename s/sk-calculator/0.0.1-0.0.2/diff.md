# Comparing `tmp/sk_calculator-0.0.1.tar.gz` & `tmp/sk_calculator-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sk_calculator-0.0.1.tar", last modified: Mon Jun 12 05:50:37 2023, max compression
+gzip compressed data, was "sk_calculator-0.0.2.tar", last modified: Mon Jun 19 13:20:24 2023, max compression
```

## Comparing `sk_calculator-0.0.1.tar` & `sk_calculator-0.0.2.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxrwxrwx   0        0        0        0 2023-06-12 05:50:37.480065 sk_calculator-0.0.1/
--rw-rw-rw-   0        0        0     1055 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/LICENSE.txt
--rw-rw-rw-   0        0        0     7592 2023-06-12 05:50:37.477071 sk_calculator-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     7117 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/README.md
--rw-rw-rw-   0        0        0       42 2023-06-12 05:50:37.480065 sk_calculator-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      814 2023-06-12 05:50:21.000000 sk_calculator-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-06-12 05:50:37.125429 sk_calculator-0.0.1/sk_calculator/
--rw-rw-rw-   0        0        0     3590 2023-06-12 05:38:27.000000 sk_calculator-0.0.1/sk_calculator/__init__.py
-drwxrwxrwx   0        0        0        0 2023-06-12 05:50:37.212906 sk_calculator-0.0.1/sk_calculator/controller/
--rw-rw-rw-   0        0        0        0 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/controller/__init__.py
--rw-rw-rw-   0        0        0     1384 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/controller/base.py
--rw-rw-rw-   0        0        0     1169 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/controller/bracket.py
--rw-rw-rw-   0        0        0      689 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/controller/default.py
--rw-rw-rw-   0        0        0      841 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/controller/error.py
--rw-rw-rw-   0        0        0     4859 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/controller/function.py
--rw-rw-rw-   0        0        0     1038 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/controller/process.py
--rw-rw-rw-   0        0        0      837 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/controller/recorder.py
--rw-rw-rw-   0        0        0     3170 2023-06-12 05:40:47.000000 sk_calculator-0.0.1/sk_calculator/controller/validation.py
-drwxrwxrwx   0        0        0        0 2023-06-12 05:50:37.243862 sk_calculator-0.0.1/sk_calculator/function/
--rw-rw-rw-   0        0        0        0 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/function/__init__.py
--rw-rw-rw-   0        0        0      651 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/function/abs.py
--rw-rw-rw-   0        0        0      700 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/function/default.py
--rw-rw-rw-   0        0        0      669 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/function/exp.py
--rw-rw-rw-   0        0        0      829 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/function/ln.py
--rw-rw-rw-   0        0        0     1091 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/function/log.py
--rw-rw-rw-   0        0        0      691 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/function/sqrt.py
-drwxrwxrwx   0        0        0        0 2023-06-12 05:50:37.277887 sk_calculator-0.0.1/sk_calculator/function/trigonometric_function/
--rw-rw-rw-   0        0        0        0 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/function/trigonometric_function/__init__.py
--rw-rw-rw-   0        0        0      764 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/function/trigonometric_function/cos.py
--rw-rw-rw-   0        0        0     1030 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/function/trigonometric_function/cosec.py
--rw-rw-rw-   0        0        0     1056 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/function/trigonometric_function/cot.py
--rw-rw-rw-   0        0        0     1059 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/function/trigonometric_function/sec.py
--rw-rw-rw-   0        0        0      773 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/function/trigonometric_function/sin.py
--rw-rw-rw-   0        0        0     1050 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/function/trigonometric_function/tan.py
-drwxrwxrwx   0        0        0        0 2023-06-12 05:50:37.310003 sk_calculator-0.0.1/sk_calculator/function/trigonometric_inverse_function/
--rw-rw-rw-   0        0        0        0 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/function/trigonometric_inverse_function/__init__.py
--rw-rw-rw-   0        0        0      817 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/function/trigonometric_inverse_function/acos.py
--rw-rw-rw-   0        0        0      815 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/function/trigonometric_inverse_function/acosec.py
--rw-rw-rw-   0        0        0      809 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/function/trigonometric_inverse_function/acot.py
--rw-rw-rw-   0        0        0      811 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/function/trigonometric_inverse_function/asec.py
--rw-rw-rw-   0        0        0      819 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/function/trigonometric_inverse_function/asin.py
--rw-rw-rw-   0        0        0      631 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/function/trigonometric_inverse_function/atan.py
-drwxrwxrwx   0        0        0        0 2023-06-12 05:50:37.357002 sk_calculator-0.0.1/sk_calculator/operations/
--rw-rw-rw-   0        0        0        0 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/operations/__init__.py
--rw-rw-rw-   0        0        0     1150 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/operations/addition.py
--rw-rw-rw-   0        0        0      885 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/operations/bracket.py
--rw-rw-rw-   0        0        0     1297 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/operations/division.py
--rw-rw-rw-   0        0        0      964 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/operations/mod.py
--rw-rw-rw-   0        0        0     1131 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/operations/multiplication.py
--rw-rw-rw-   0        0        0      967 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/operations/power.py
--rw-rw-rw-   0        0        0     1136 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/operations/substraction.py
--rw-rw-rw-   0        0        0     1045 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/operations/unary.py
-drwxrwxrwx   0        0        0        0 2023-06-12 05:50:37.380003 sk_calculator-0.0.1/sk_calculator/process/
--rw-rw-rw-   0        0        0        0 2023-06-12 05:38:13.000000 sk_calculator-0.0.1/sk_calculator/process/__init__.py
--rw-rw-rw-   0        0        0      220 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/process/default.py
--rw-rw-rw-   0        0        0      588 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/process/e.py
--rw-rw-rw-   0        0        0      592 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/process/pi.py
--rw-rw-rw-   0        0        0      345 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/process/space.py
--rw-rw-rw-   0        0        0    29669 2023-06-11 06:01:27.000000 sk_calculator-0.0.1/sk_calculator/test_calculator.py
--rw-rw-rw-   0        0        0     8549 2023-06-11 05:59:29.000000 sk_calculator-0.0.1/sk_calculator/test_validation.py
-drwxrwxrwx   0        0        0        0 2023-06-12 05:50:37.441070 sk_calculator-0.0.1/sk_calculator/validations/
--rw-rw-rw-   0        0        0        0 2023-06-12 05:38:13.000000 sk_calculator-0.0.1/sk_calculator/validations/__init__.py
--rw-rw-rw-   0        0        0        0 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/validations/base.py
--rw-rw-rw-   0        0        0      652 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/validations/completion_check.py
--rw-rw-rw-   0        0        0      852 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/validations/constant_check.py
--rw-rw-rw-   0        0        0      329 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/validations/default.py
--rw-rw-rw-   0        0        0      633 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/validations/division_check.py
--rw-rw-rw-   0        0        0     1550 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/validations/function_check.py
--rw-rw-rw-   0        0        0      629 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/validations/key_check.py
--rw-rw-rw-   0        0        0      885 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/validations/keyword_check.py
--rw-rw-rw-   0        0        0      621 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/validations/number_check.py
-drwxrwxrwx   0        0        0        0 2023-06-12 05:50:37.469070 sk_calculator-0.0.1/sk_calculator/validations/operator/
--rw-rw-rw-   0        0        0        0 2023-06-12 05:38:13.000000 sk_calculator-0.0.1/sk_calculator/validations/operator/__init__.py
--rw-rw-rw-   0        0        0      940 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/validations/operator/opc1.py
--rw-rw-rw-   0        0        0      642 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/validations/operator/opc2.py
--rw-rw-rw-   0        0        0      802 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/validations/operator/opc3.py
--rw-rw-rw-   0        0        0      675 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/validations/operator/opc4.py
--rw-rw-rw-   0        0        0      659 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/validations/operator/opc5.py
--rw-rw-rw-   0        0        0     1391 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/validations/operator_check.py
--rw-rw-rw-   0        0        0      721 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/validations/parentheses_check.py
--rw-rw-rw-   0        0        0      570 2023-06-08 17:52:35.000000 sk_calculator-0.0.1/sk_calculator/validations/type_check.py
-drwxrwxrwx   0        0        0        0 2023-06-12 05:50:37.172903 sk_calculator-0.0.1/sk_calculator.egg-info/
--rw-rw-rw-   0        0        0     7592 2023-06-12 05:50:36.000000 sk_calculator-0.0.1/sk_calculator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2956 2023-06-12 05:50:36.000000 sk_calculator-0.0.1/sk_calculator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-06-12 05:50:36.000000 sk_calculator-0.0.1/sk_calculator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2023-06-12 05:50:36.000000 sk_calculator-0.0.1/sk_calculator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-06-12 05:50:36.000000 sk_calculator-0.0.1/sk_calculator.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-06-19 13:20:24.559364 sk_calculator-0.0.2/
+-rw-rw-rw-   0        0        0     1055 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/LICENSE.txt
+-rw-rw-rw-   0        0        0     7592 2023-06-19 13:20:24.559364 sk_calculator-0.0.2/PKG-INFO
+-rw-rw-rw-   0        0        0     7117 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-06-19 13:20:24.559364 sk_calculator-0.0.2/setup.cfg
+-rw-rw-rw-   0        0        0      800 2023-06-19 13:18:14.000000 sk_calculator-0.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:20:24.468472 sk_calculator-0.0.2/sk_calculator/
+-rw-rw-rw-   0        0        0     3680 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/__init__.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:20:24.498451 sk_calculator-0.0.2/sk_calculator/controller/
+-rw-rw-rw-   0        0        0        0 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/controller/__init__.py
+-rw-rw-rw-   0        0        0     1384 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/controller/base.py
+-rw-rw-rw-   0        0        0     1169 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/controller/bracket.py
+-rw-rw-rw-   0        0        0      689 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/controller/default.py
+-rw-rw-rw-   0        0        0      841 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/controller/error.py
+-rw-rw-rw-   0        0        0     4859 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/controller/function.py
+-rw-rw-rw-   0        0        0     1038 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/controller/process.py
+-rw-rw-rw-   0        0        0      837 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/controller/recorder.py
+-rw-rw-rw-   0        0        0     3170 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/controller/validation.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:20:24.508444 sk_calculator-0.0.2/sk_calculator/function/
+-rw-rw-rw-   0        0        0        0 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/function/__init__.py
+-rw-rw-rw-   0        0        0      651 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/function/abs.py
+-rw-rw-rw-   0        0        0      700 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/function/default.py
+-rw-rw-rw-   0        0        0      669 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/function/exp.py
+-rw-rw-rw-   0        0        0      829 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/function/ln.py
+-rw-rw-rw-   0        0        0     1091 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/function/log.py
+-rw-rw-rw-   0        0        0      691 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/function/sqrt.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:20:24.513441 sk_calculator-0.0.2/sk_calculator/function/trigonometric_function/
+-rw-rw-rw-   0        0        0        0 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/function/trigonometric_function/__init__.py
+-rw-rw-rw-   0        0        0      764 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/function/trigonometric_function/cos.py
+-rw-rw-rw-   0        0        0     1030 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/function/trigonometric_function/cosec.py
+-rw-rw-rw-   0        0        0     1056 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/function/trigonometric_function/cot.py
+-rw-rw-rw-   0        0        0     1059 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/function/trigonometric_function/sec.py
+-rw-rw-rw-   0        0        0      773 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/function/trigonometric_function/sin.py
+-rw-rw-rw-   0        0        0     1050 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/function/trigonometric_function/tan.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:20:24.523441 sk_calculator-0.0.2/sk_calculator/function/trigonometric_inverse_function/
+-rw-rw-rw-   0        0        0        0 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/function/trigonometric_inverse_function/__init__.py
+-rw-rw-rw-   0        0        0      817 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/function/trigonometric_inverse_function/acos.py
+-rw-rw-rw-   0        0        0      815 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/function/trigonometric_inverse_function/acosec.py
+-rw-rw-rw-   0        0        0      809 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/function/trigonometric_inverse_function/acot.py
+-rw-rw-rw-   0        0        0      811 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/function/trigonometric_inverse_function/asec.py
+-rw-rw-rw-   0        0        0      819 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/function/trigonometric_inverse_function/asin.py
+-rw-rw-rw-   0        0        0      631 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/function/trigonometric_inverse_function/atan.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:20:24.533669 sk_calculator-0.0.2/sk_calculator/operations/
+-rw-rw-rw-   0        0        0        0 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/operations/__init__.py
+-rw-rw-rw-   0        0        0     1150 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/operations/addition.py
+-rw-rw-rw-   0        0        0      885 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/operations/bracket.py
+-rw-rw-rw-   0        0        0     1297 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/operations/division.py
+-rw-rw-rw-   0        0        0      964 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/operations/mod.py
+-rw-rw-rw-   0        0        0     1131 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/operations/multiplication.py
+-rw-rw-rw-   0        0        0      967 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/operations/power.py
+-rw-rw-rw-   0        0        0     1136 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/operations/substraction.py
+-rw-rw-rw-   0        0        0     1045 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/operations/unary.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:20:24.538674 sk_calculator-0.0.2/sk_calculator/process/
+-rw-rw-rw-   0        0        0        0 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/process/__init__.py
+-rw-rw-rw-   0        0        0      220 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/process/default.py
+-rw-rw-rw-   0        0        0      588 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/process/e.py
+-rw-rw-rw-   0        0        0      592 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/process/pi.py
+-rw-rw-rw-   0        0        0      345 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/process/space.py
+-rw-rw-rw-   0        0        0    29669 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/test_calculator.py
+-rw-rw-rw-   0        0        0     8549 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/test_validation.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:20:24.554128 sk_calculator-0.0.2/sk_calculator/validations/
+-rw-rw-rw-   0        0        0        0 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/validations/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/validations/base.py
+-rw-rw-rw-   0        0        0      652 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/validations/completion_check.py
+-rw-rw-rw-   0        0        0      852 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/validations/constant_check.py
+-rw-rw-rw-   0        0        0      329 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/validations/default.py
+-rw-rw-rw-   0        0        0      633 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/validations/division_check.py
+-rw-rw-rw-   0        0        0     1550 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/validations/function_check.py
+-rw-rw-rw-   0        0        0      629 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/validations/key_check.py
+-rw-rw-rw-   0        0        0      885 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/validations/keyword_check.py
+-rw-rw-rw-   0        0        0      621 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/validations/number_check.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:20:24.559364 sk_calculator-0.0.2/sk_calculator/validations/operator/
+-rw-rw-rw-   0        0        0        0 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/validations/operator/__init__.py
+-rw-rw-rw-   0        0        0      940 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/validations/operator/opc1.py
+-rw-rw-rw-   0        0        0      642 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/validations/operator/opc2.py
+-rw-rw-rw-   0        0        0      802 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/validations/operator/opc3.py
+-rw-rw-rw-   0        0        0      675 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/validations/operator/opc4.py
+-rw-rw-rw-   0        0        0      659 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/validations/operator/opc5.py
+-rw-rw-rw-   0        0        0     1391 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/validations/operator_check.py
+-rw-rw-rw-   0        0        0      721 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/validations/parentheses_check.py
+-rw-rw-rw-   0        0        0      570 2023-06-19 13:17:07.000000 sk_calculator-0.0.2/sk_calculator/validations/type_check.py
+drwxrwxrwx   0        0        0        0 2023-06-19 13:20:24.488539 sk_calculator-0.0.2/sk_calculator.egg-info/
+-rw-rw-rw-   0        0        0     7592 2023-06-19 13:20:24.000000 sk_calculator-0.0.2/sk_calculator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2956 2023-06-19 13:20:24.000000 sk_calculator-0.0.2/sk_calculator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-06-19 13:20:24.000000 sk_calculator-0.0.2/sk_calculator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        6 2023-06-19 13:20:24.000000 sk_calculator-0.0.2/sk_calculator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-06-19 13:20:24.000000 sk_calculator-0.0.2/sk_calculator.egg-info/top_level.txt
```

### Comparing `sk_calculator-0.0.1/LICENSE.txt` & `sk_calculator-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/PKG-INFO` & `sk_calculator-0.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sk_calculator
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple calculator program
 Author: gkibria
 Author-email: gkibria121@gmail.com
 Keywords: python,calculator,python calculator,gk calculator,advanced calculator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sk_calculator-0.0.1/README.md` & `sk_calculator-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/setup.py` & `sk_calculator-0.0.2/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='sk_calculator',
-    version='0.0.1',
+    version='0.0.2',
     description='A simple calculator program',
     author='gkibria',
     long_description=long_description,
     long_description_content_type="text/markdown",  # Specify the content type as Markdown
     author_email='gkibria121@gmail.com',
     packages=find_packages(),
-    install_requires=['setuptools', 'regex'],
+    install_requires=['regex'],
     python_requires='>=3.6',
     keywords='python, calculator, python calculator, gk calculator, advanced calculator',
     classifiers=[
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
     ],
```

### Comparing `sk_calculator-0.0.1/sk_calculator/__init__.py` & `sk_calculator-0.0.2/sk_calculator/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,11 +82,12 @@
 
     def evaluate(self,expression):
 
         self.error_handle.set_expression(expression)
         self.recorder.set_expression(expression)
         self.expression =  self.validation.evaluate(expression)
         self.recorder.record(expression,self.expression,self.__class__.__name__)
-        return self.expression
+        result = int(self.expression) if str(self.expression).endswith('.0') else self.expression
+        return result
 
 
 __all__ = ['controller', 'function','operations','process','validations']
```

### Comparing `sk_calculator-0.0.1/sk_calculator/controller/base.py` & `sk_calculator-0.0.2/sk_calculator/controller/base.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/controller/bracket.py` & `sk_calculator-0.0.2/sk_calculator/controller/bracket.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/controller/default.py` & `sk_calculator-0.0.2/sk_calculator/controller/default.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/controller/error.py` & `sk_calculator-0.0.2/sk_calculator/controller/error.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/controller/function.py` & `sk_calculator-0.0.2/sk_calculator/controller/function.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/controller/process.py` & `sk_calculator-0.0.2/sk_calculator/controller/process.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/controller/recorder.py` & `sk_calculator-0.0.2/sk_calculator/controller/recorder.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/controller/validation.py` & `sk_calculator-0.0.2/sk_calculator/controller/validation.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/function/abs.py` & `sk_calculator-0.0.2/sk_calculator/function/abs.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/function/default.py` & `sk_calculator-0.0.2/sk_calculator/function/default.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/function/exp.py` & `sk_calculator-0.0.2/sk_calculator/function/exp.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/function/ln.py` & `sk_calculator-0.0.2/sk_calculator/function/ln.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/function/log.py` & `sk_calculator-0.0.2/sk_calculator/function/log.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/function/sqrt.py` & `sk_calculator-0.0.2/sk_calculator/function/sqrt.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/function/trigonometric_function/cos.py` & `sk_calculator-0.0.2/sk_calculator/function/trigonometric_function/cos.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/function/trigonometric_function/cosec.py` & `sk_calculator-0.0.2/sk_calculator/function/trigonometric_function/cosec.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/function/trigonometric_function/cot.py` & `sk_calculator-0.0.2/sk_calculator/function/trigonometric_function/cot.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/function/trigonometric_function/sec.py` & `sk_calculator-0.0.2/sk_calculator/function/trigonometric_function/sec.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/function/trigonometric_function/sin.py` & `sk_calculator-0.0.2/sk_calculator/function/trigonometric_function/sin.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/function/trigonometric_function/tan.py` & `sk_calculator-0.0.2/sk_calculator/function/trigonometric_function/tan.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/function/trigonometric_inverse_function/acos.py` & `sk_calculator-0.0.2/sk_calculator/function/trigonometric_inverse_function/acos.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/function/trigonometric_inverse_function/acosec.py` & `sk_calculator-0.0.2/sk_calculator/function/trigonometric_inverse_function/acosec.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/function/trigonometric_inverse_function/acot.py` & `sk_calculator-0.0.2/sk_calculator/function/trigonometric_inverse_function/acot.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/function/trigonometric_inverse_function/asec.py` & `sk_calculator-0.0.2/sk_calculator/function/trigonometric_inverse_function/asec.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/function/trigonometric_inverse_function/asin.py` & `sk_calculator-0.0.2/sk_calculator/function/trigonometric_inverse_function/asin.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/function/trigonometric_inverse_function/atan.py` & `sk_calculator-0.0.2/sk_calculator/function/trigonometric_inverse_function/atan.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/operations/addition.py` & `sk_calculator-0.0.2/sk_calculator/operations/addition.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/operations/bracket.py` & `sk_calculator-0.0.2/sk_calculator/operations/bracket.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/operations/division.py` & `sk_calculator-0.0.2/sk_calculator/operations/division.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/operations/mod.py` & `sk_calculator-0.0.2/sk_calculator/operations/mod.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/operations/multiplication.py` & `sk_calculator-0.0.2/sk_calculator/operations/multiplication.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/operations/power.py` & `sk_calculator-0.0.2/sk_calculator/operations/power.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/operations/substraction.py` & `sk_calculator-0.0.2/sk_calculator/operations/substraction.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/operations/unary.py` & `sk_calculator-0.0.2/sk_calculator/operations/unary.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/process/e.py` & `sk_calculator-0.0.2/sk_calculator/process/e.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/process/pi.py` & `sk_calculator-0.0.2/sk_calculator/process/pi.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/test_calculator.py` & `sk_calculator-0.0.2/sk_calculator/test_calculator.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/test_validation.py` & `sk_calculator-0.0.2/sk_calculator/test_validation.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/validations/completion_check.py` & `sk_calculator-0.0.2/sk_calculator/validations/completion_check.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/validations/constant_check.py` & `sk_calculator-0.0.2/sk_calculator/validations/constant_check.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/validations/division_check.py` & `sk_calculator-0.0.2/sk_calculator/validations/division_check.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/validations/function_check.py` & `sk_calculator-0.0.2/sk_calculator/validations/function_check.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/validations/key_check.py` & `sk_calculator-0.0.2/sk_calculator/validations/key_check.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/validations/keyword_check.py` & `sk_calculator-0.0.2/sk_calculator/validations/keyword_check.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/validations/number_check.py` & `sk_calculator-0.0.2/sk_calculator/validations/number_check.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/validations/operator/opc1.py` & `sk_calculator-0.0.2/sk_calculator/validations/operator/opc1.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/validations/operator/opc2.py` & `sk_calculator-0.0.2/sk_calculator/validations/operator/opc2.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/validations/operator/opc3.py` & `sk_calculator-0.0.2/sk_calculator/validations/operator/opc3.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/validations/operator/opc4.py` & `sk_calculator-0.0.2/sk_calculator/validations/operator/opc4.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/validations/operator/opc5.py` & `sk_calculator-0.0.2/sk_calculator/validations/operator/opc5.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/validations/operator_check.py` & `sk_calculator-0.0.2/sk_calculator/validations/operator_check.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/validations/parentheses_check.py` & `sk_calculator-0.0.2/sk_calculator/validations/parentheses_check.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator/validations/type_check.py` & `sk_calculator-0.0.2/sk_calculator/validations/type_check.py`

 * *Files identical despite different names*

### Comparing `sk_calculator-0.0.1/sk_calculator.egg-info/PKG-INFO` & `sk_calculator-0.0.2/sk_calculator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sk-calculator
-Version: 0.0.1
+Version: 0.0.2
 Summary: A simple calculator program
 Author: gkibria
 Author-email: gkibria121@gmail.com
 Keywords: python,calculator,python calculator,gk calculator,advanced calculator
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `sk_calculator-0.0.1/sk_calculator.egg-info/SOURCES.txt` & `sk_calculator-0.0.2/sk_calculator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

