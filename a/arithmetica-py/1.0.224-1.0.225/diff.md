# Comparing `tmp/arithmetica-py-1.0.224.tar.gz` & `tmp/arithmetica-py-1.0.225.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arithmetica-py-1.0.224.tar", last modified: Wed Jun 14 15:46:00 2023, max compression
+gzip compressed data, was "arithmetica-py-1.0.225.tar", last modified: Mon Jun 19 12:58:15 2023, max compression
```

## Comparing `arithmetica-py-1.0.224.tar` & `arithmetica-py-1.0.225.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:46:00.555984 arithmetica-py-1.0.224/
--rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-06-14 15:45:41.000000 arithmetica-py-1.0.224/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-14 15:46:00.555984 arithmetica-py-1.0.224/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-06-14 15:45:41.000000 arithmetica-py-1.0.224/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:46:00.551984 arithmetica-py-1.0.224/arithmetica_py.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-14 15:46:00.000000 arithmetica-py-1.0.224/arithmetica_py.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-14 15:46:00.000000 arithmetica-py-1.0.224/arithmetica_py.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-14 15:46:00.000000 arithmetica-py-1.0.224/arithmetica_py.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-14 15:46:00.000000 arithmetica-py-1.0.224/arithmetica_py.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-14 15:46:00.555984 arithmetica-py-1.0.224/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-14 15:45:41.000000 arithmetica-py-1.0.224/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:46:00.551984 arithmetica-py-1.0.224/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-14 15:46:00.551984 arithmetica-py-1.0.224/src/python-module/
--rw-r--r--   0 runner    (1001) docker     (123)   187278 2023-06-14 15:46:00.000000 arithmetica-py-1.0.224/src/python-module/libarithmetica.a
--rw-r--r--   0 runner    (1001) docker     (123)    75528 2023-06-14 15:46:00.000000 arithmetica-py-1.0.224/src/python-module/libbasic_math_operations.a
--rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-06-14 15:45:41.000000 arithmetica-py-1.0.224/src/python-module/module.c
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-14 15:46:00.000000 arithmetica-py-1.0.224/src/python-module/version.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:58:15.309144 arithmetica-py-1.0.225/
+-rw-r--r--   0 runner    (1001) docker     (123)    35823 2023-06-19 12:57:55.000000 arithmetica-py-1.0.225/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-19 12:58:15.305144 arithmetica-py-1.0.225/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10561 2023-06-19 12:57:55.000000 arithmetica-py-1.0.225/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:58:15.305144 arithmetica-py-1.0.225/arithmetica_py.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-06-19 12:58:15.000000 arithmetica-py-1.0.225/arithmetica_py.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-06-19 12:58:15.000000 arithmetica-py-1.0.225/arithmetica_py.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 12:58:15.000000 arithmetica-py-1.0.225/arithmetica_py.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-06-19 12:58:15.000000 arithmetica-py-1.0.225/arithmetica_py.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 12:58:15.309144 arithmetica-py-1.0.225/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-06-19 12:57:55.000000 arithmetica-py-1.0.225/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:58:15.305144 arithmetica-py-1.0.225/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 12:58:15.305144 arithmetica-py-1.0.225/src/python-module/
+-rw-r--r--   0 runner    (1001) docker     (123)   187678 2023-06-19 12:58:15.000000 arithmetica-py-1.0.225/src/python-module/libarithmetica.a
+-rw-r--r--   0 runner    (1001) docker     (123)    75560 2023-06-19 12:58:15.000000 arithmetica-py-1.0.225/src/python-module/libbasic_math_operations.a
+-rw-r--r--   0 runner    (1001) docker     (123)    13601 2023-06-19 12:57:55.000000 arithmetica-py-1.0.225/src/python-module/module.c
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-06-19 12:58:15.000000 arithmetica-py-1.0.225/src/python-module/version.txt
```

### Comparing `arithmetica-py-1.0.224/LICENSE` & `arithmetica-py-1.0.225/LICENSE`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.224/README.md` & `arithmetica-py-1.0.225/README.md`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.224/setup.py` & `arithmetica-py-1.0.225/setup.py`

 * *Files identical despite different names*

### Comparing `arithmetica-py-1.0.224/src/python-module/libarithmetica.a` & `arithmetica-py-1.0.225/src/python-module/libarithmetica.a`

 * *Files 1% similar despite different names*

#### nm -s {}

```diff
@@ -621,28 +621,31 @@
                  U simplify_parsed_fraction
                  U strchr
                  U strcpy
                  U strlen
                  U strncpy
 
 power_fraction.c.o:
+0000000000000000 r .LC0
                  U __stack_chk_fail
 0000000000000000 T arithmetica_power_fraction_round_decimal
                  U calloc
                  U delete_fraction
                  U divide
                  U free
                  U memcpy
                  U memmove
                  U parse_fraction
                  U power
 00000000000000f0 T power_fraction
                  U realloc
+                 U square_root
                  U stpcpy
                  U strchr
+                 U strcmp
                  U strlen
                  U strncpy
 
 simplify_parsed_fraction.c.o:
 0000000000000000 r .LC0
 0000000000000002 r .LC1
                  U calloc
```

#### file list

```diff
@@ -1,40 +1,40 @@
 ----------   0        0        0     3744 1970-01-01 00:00:00.000000 /
 ----------   0        0        0        0 1970-01-01 00:00:00.000000 //
 ?rw-r--r--   0        0        0    22216 1970-01-01 00:00:00.000000 arithmetica.cpp.o
 ?rw-r--r--   0        0        0     3024 1970-01-01 00:00:00.000000 arccos.c.o
 ?rw-r--r--   0        0        0     4056 1970-01-01 00:00:00.000000 arcsin.c.o
 ?rw-r--r--   0        0        0     2328 1970-01-01 00:00:00.000000 arctan.c.o
 ?rw-r--r--   0        0        0     1768 1970-01-01 00:00:00.000000 check_accuracy.c.o
-?rw-r--r--   0        0        0     2528 1970-01-01 00:00:00.000000 continued_fraction_to_fraction.c.o
+?rw-r--r--   0        0        0     2536 1970-01-01 00:00:00.000000 continued_fraction_to_fraction.c.o
 ?rw-r--r--   0        0        0     3968 1970-01-01 00:00:00.000000 cosine.c.o
 ?rw-r--r--   0        0        0     3896 1970-01-01 00:00:00.000000 exponential.c.o
 ?rw-r--r--   0        0        0     3752 1970-01-01 00:00:00.000000 factorial.c.o
-?rw-r--r--   0        0        0    13168 1970-01-01 00:00:00.000000 find_roots_of_polynomial.c.o
+?rw-r--r--   0        0        0    13176 1970-01-01 00:00:00.000000 find_roots_of_polynomial.c.o
 ?rw-r--r--   0        0        0     2656 1970-01-01 00:00:00.000000 fraction_to_continued_fraction.c.o
-?rw-r--r--   0        0        0     2616 1970-01-01 00:00:00.000000 igcd.c.o
+?rw-r--r--   0        0        0     2624 1970-01-01 00:00:00.000000 igcd.c.o
 ?rw-r--r--   0        0        0     1912 1970-01-01 00:00:00.000000 ilcm.c.o
 ?rw-r--r--   0        0        0     2632 1970-01-01 00:00:00.000000 natural_logarithm.c.o
 ?rw-r--r--   0        0        0     3104 1970-01-01 00:00:00.000000 power.c.o
 ?rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 power_integer.c.o
 ?rw-r--r--   0        0        0     2672 1970-01-01 00:00:00.000000 repeating_decimal_to_fraction.c.o
 ?rw-r--r--   0        0        0    18336 1970-01-01 00:00:00.000000 simplify_arithmetic_expression.c.o
 ?rw-r--r--   0        0        0     4712 1970-01-01 00:00:00.000000 sine.c.o
 ?rw-r--r--   0        0        0     4736 1970-01-01 00:00:00.000000 square_root.c.o
-?rw-r--r--   0        0        0     1808 1970-01-01 00:00:00.000000 tangent.c.o
+?rw-r--r--   0        0        0     1816 1970-01-01 00:00:00.000000 tangent.c.o
 ?rw-r--r--   0        0        0     2856 1970-01-01 00:00:00.000000 terminating_decimal_to_fraction.c.o
 ?rw-r--r--   0        0        0    20024 1970-01-01 00:00:00.000000 Fraction.cpp.o
 ?rw-r--r--   0        0        0     1896 1970-01-01 00:00:00.000000 fraction.c.o
 ?rw-r--r--   0        0        0     2320 1970-01-01 00:00:00.000000 add_fraction.c.o
 ?rw-r--r--   0        0        0     1944 1970-01-01 00:00:00.000000 multiply_fraction.c.o
 ?rw-r--r--   0        0        0     3464 1970-01-01 00:00:00.000000 parse_fraction.c.o
-?rw-r--r--   0        0        0     4376 1970-01-01 00:00:00.000000 power_fraction.c.o
+?rw-r--r--   0        0        0     4736 1970-01-01 00:00:00.000000 power_fraction.c.o
 ?rw-r--r--   0        0        0     2736 1970-01-01 00:00:00.000000 simplify_parsed_fraction.c.o
 ?rw-r--r--   0        0        0     2336 1970-01-01 00:00:00.000000 subtract_fraction.c.o
-?rw-r--r--   0        0        0     1568 1970-01-01 00:00:00.000000 equal_fraction.c.o
+?rw-r--r--   0        0        0     1576 1970-01-01 00:00:00.000000 equal_fraction.c.o
 ?rw-r--r--   0        0        0     1920 1970-01-01 00:00:00.000000 complex_arithmetica.c.o
 ?rw-r--r--   0        0        0     1768 1970-01-01 00:00:00.000000 add_complex.c.o
 ?rw-r--r--   0        0        0     3032 1970-01-01 00:00:00.000000 divide_complex.c.o
 ?rw-r--r--   0        0        0     2064 1970-01-01 00:00:00.000000 exponential_complex.c.o
 ?rw-r--r--   0        0        0     2512 1970-01-01 00:00:00.000000 multiply_complex.c.o
 ?rw-r--r--   0        0        0     3944 1970-01-01 00:00:00.000000 square_root_complex.c.o
 ?rw-r--r--   0        0        0     1784 1970-01-01 00:00:00.000000 subtract_complex.c.o
```

#### arithmetica.cpp.o

##### readelf --wide --sections {}

```diff
@@ -22,16 +22,16 @@
   [17] .init_array       INIT_ARRAY      0000000000000000 001c50 000008 08  WA  0   0  8
   [18] .rela.init_array  RELA            0000000000000000 004908 000018 18   I 29  17  8
   [19] .rodata.cst8      PROGBITS        0000000000000000 001c58 000008 08  AM  0   0  8
   [20] .rodata.cst4      PROGBITS        0000000000000000 001c60 000010 04  AM  0   0  4
   [21] .rodata.cst16     PROGBITS        0000000000000000 001c70 000010 10  AM  0   0 16
   [22] .data.rel.local.DW.ref.__gxx_personality_v0 PROGBITS        0000000000000000 001c80 000008 00 WAG  0   0  8
   [23] .rela.data.rel.local.DW.ref.__gxx_personality_v0 RELA            0000000000000000 004920 000018 18  IG 29  22  8
-  [24] .comment          PROGBITS        0000000000000000 001c88 00002c 01  MS  0   0  1
-  [25] .note.GNU-stack   PROGBITS        0000000000000000 001cb4 000000 00      0   0  1
+  [24] .comment          PROGBITS        0000000000000000 001c88 00002e 01  MS  0   0  1
+  [25] .note.GNU-stack   PROGBITS        0000000000000000 001cb6 000000 00      0   0  1
   [26] .note.gnu.property NOTE            0000000000000000 001cb8 000020 00   A  0   0  8
   [27] .eh_frame         PROGBITS        0000000000000000 001cd8 0005c8 00   A  0   0  8
   [28] .rela.eh_frame    RELA            0000000000000000 004938 000318 18   I 29  27  8
   [29] .symtab           SYMTAB          0000000000000000 0022a0 0007c8 18     30  25  8
   [30] .strtab           STRTAB          0000000000000000 002a68 000b36 00      0   0  1
   [31] .shstrtab         STRTAB          0000000000000000 004c50 000274 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -6,15 +6,15 @@
 []A\A]A^
 []A\A]A^A_
 basic_string::_M_construct null not valid
 basic_string::append
 vector::_M_realloc_insert
 AWAVAUATUSH
 ([]A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 _ZN11arithmetica29repeating_decimal_to_fractionERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES7_.cold
 _ZN11arithmetica31terminating_decimal_to_fractionERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE.cold
 _ZN11arithmetica9to_stringB5cxx11ERKNS_8FractionE.cold
 _ZN11arithmetica30fraction_to_continued_fractionENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES5_.cold
 _GLOBAL__sub_I_arithmetica.cpp
 _ZStL8__ioinit
 _ZN11arithmetica6arccosENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEEm
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### arccos.c.o

##### readelf --wide --sections {}

```diff
@@ -5,16 +5,16 @@
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 000183 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 000540 000228 18   I 12   1  8
   [ 3] .data             PROGBITS        0000000000000000 0001c3 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 0001c3 000000 00  WA  0   0  1
   [ 5] .rodata.str1.1    PROGBITS        0000000000000000 0001c3 000002 01 AMS  0   0  1
   [ 6] .rodata.cst16     PROGBITS        0000000000000000 0001d0 000060 10  AM  0   0 16
-  [ 7] .comment          PROGBITS        0000000000000000 000230 00002c 01  MS  0   0  1
-  [ 8] .note.GNU-stack   PROGBITS        0000000000000000 00025c 000000 00      0   0  1
+  [ 7] .comment          PROGBITS        0000000000000000 000230 00002e 01  MS  0   0  1
+  [ 8] .note.GNU-stack   PROGBITS        0000000000000000 00025e 000000 00      0   0  1
   [ 9] .note.gnu.property NOTE            0000000000000000 000260 000020 00   A  0   0  8
   [10] .eh_frame         PROGBITS        0000000000000000 000280 000060 00   A  0   0  8
   [11] .rela.eh_frame    RELA            0000000000000000 000768 000018 18   I 12  10  8
   [12] .symtab           SYMTAB          0000000000000000 0002e0 0001e0 18     13  10  8
   [13] .strtab           STRTAB          0000000000000000 0004c0 00007f 00      0   0  1
   [14] .shstrtab         STRTAB          0000000000000000 000780 000089 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,10 +1,10 @@
 ]A\A]A^A_
 1.5707963267948966192313216916397514420985846996875529104874722961539082031431044993140174126710
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 arccos.c
 subtract
 truncate
 __stack_chk_fail
 .shstrtab
 .rela.text
 .rodata.str1.1
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### arcsin.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 0003a8 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 0006a0 000570 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 0003e8 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 0003e8 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 0003e8 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000414 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 0003e8 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000416 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000418 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 000438 000068 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 000c10 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 0004a0 000180 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 000620 00007e 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 000c28 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,10 +1,10 @@
 AWAVAUATUH
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 arcsin.c
 multiply
 increment_whole
 check_accuracy
 __stack_chk_fail
 .shstrtab
 .rela.text
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### arctan.c.o

##### readelf --wide --sections {}

```diff
@@ -4,16 +4,16 @@
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 0000ef 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 000368 000198 18   I 11   1  8
   [ 3] .data             PROGBITS        0000000000000000 00012f 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 00012f 000000 00  WA  0   0  1
   [ 5] .rodata.str1.1    PROGBITS        0000000000000000 00012f 000002 01 AMS  0   0  1
-  [ 6] .comment          PROGBITS        0000000000000000 000131 00002c 01  MS  0   0  1
-  [ 7] .note.GNU-stack   PROGBITS        0000000000000000 00015d 000000 00      0   0  1
+  [ 6] .comment          PROGBITS        0000000000000000 000131 00002e 01  MS  0   0  1
+  [ 7] .note.GNU-stack   PROGBITS        0000000000000000 00015f 000000 00      0   0  1
   [ 8] .note.gnu.property NOTE            0000000000000000 000160 000020 00   A  0   0  8
   [ 9] .eh_frame         PROGBITS        0000000000000000 000180 000060 00   A  0   0  8
   [10] .rela.eh_frame    RELA            0000000000000000 000500 000018 18   I 11   9  8
   [11] .symtab           SYMTAB          0000000000000000 0001e0 000138 18     12   4  8
   [12] .strtab           STRTAB          0000000000000000 000318 000050 00      0   0  1
   [13] .shstrtab         STRTAB          0000000000000000 000518 00007b 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,9 +1,9 @@
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 arctan.c
 multiply
 square_root
 .shstrtab
 .rela.text
 .rodata.str1.1
 .comment
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### check_accuracy.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 0000ce 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 0002a8 000078 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 00010e 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 00010e 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 00010e 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 00013a 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 00010e 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 00013c 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000140 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 000160 000068 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 000320 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 0001c8 0000a8 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 000270 000036 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 000338 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,9 +1,9 @@
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 check_accuracy.c
 check_accuracy
 .shstrtab
 .rela.text
 .comment
 .note.GNU-stack
 .note.gnu.property
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### continued_fraction_to_fraction.c.o

##### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              REL (Relocatable file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          0 (bytes into file)
-  Start of section headers:          1696 (bytes into file)
+  Start of section headers:          1704 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           0 (bytes)
   Number of program headers:         0
   Size of section headers:           64 (bytes)
   Number of section headers:         13
   Section header string table index: 12
```

##### readelf --wide --sections {}

```diff
@@ -1,22 +1,22 @@
-There are 13 section headers, starting at offset 0x6a0:
+There are 13 section headers, starting at offset 0x6a8:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 0001ab 00  AX  0   0 16
-  [ 2] .rela.text        RELA            0000000000000000 000438 0001e0 18   I 10   1  8
+  [ 2] .rela.text        RELA            0000000000000000 000440 0001e0 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 0001eb 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 0001eb 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 0001eb 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000217 000000 00      0   0  1
-  [ 7] .note.gnu.property NOTE            0000000000000000 000218 000020 00   A  0   0  8
-  [ 8] .eh_frame         PROGBITS        0000000000000000 000238 000068 00   A  0   0  8
-  [ 9] .rela.eh_frame    RELA            0000000000000000 000618 000018 18   I 10   8  8
-  [10] .symtab           SYMTAB          0000000000000000 0002a0 000120 18     11   3  8
-  [11] .strtab           STRTAB          0000000000000000 0003c0 000076 00      0   0  1
-  [12] .shstrtab         STRTAB          0000000000000000 000630 00006c 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 0001eb 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000219 000000 00      0   0  1
+  [ 7] .note.gnu.property NOTE            0000000000000000 000220 000020 00   A  0   0  8
+  [ 8] .eh_frame         PROGBITS        0000000000000000 000240 000068 00   A  0   0  8
+  [ 9] .rela.eh_frame    RELA            0000000000000000 000620 000018 18   I 10   8  8
+  [10] .symtab           SYMTAB          0000000000000000 0002a8 000120 18     11   3  8
+  [11] .strtab           STRTAB          0000000000000000 0003c8 000076 00      0   0  1
+  [12] .shstrtab         STRTAB          0000000000000000 000638 00006c 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --relocs {}

```diff
@@ -1,9 +1,9 @@
 
-Relocation section '.rela.text' at offset 0x438 contains 20 entries:
+Relocation section '.rela.text' at offset 0x440 contains 20 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 000000000000003d  0000000400000004 R_X86_64_PLT32         0000000000000000 malloc - 4
 0000000000000056  0000000500000004 R_X86_64_PLT32         0000000000000000 strlen - 4
 000000000000005f  0000000400000004 R_X86_64_PLT32         0000000000000000 malloc - 4
 0000000000000077  0000000600000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
 0000000000000084  0000000500000004 R_X86_64_PLT32         0000000000000000 strlen - 4
 000000000000009c  0000000500000004 R_X86_64_PLT32         0000000000000000 strlen - 4
@@ -18,10 +18,10 @@
 000000000000013e  0000000400000004 R_X86_64_PLT32         0000000000000000 malloc - 4
 000000000000014b  0000000400000004 R_X86_64_PLT32         0000000000000000 malloc - 4
 000000000000016f  0000000500000004 R_X86_64_PLT32         0000000000000000 strlen - 4
 000000000000017b  0000000400000004 R_X86_64_PLT32         0000000000000000 malloc - 4
 0000000000000188  0000000400000004 R_X86_64_PLT32         0000000000000000 malloc - 4
 0000000000000199  0000000b00000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
 
-Relocation section '.rela.eh_frame' at offset 0x618 contains 1 entry:
+Relocation section '.rela.eh_frame' at offset 0x620 contains 1 entry:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000020  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 0
```

##### strings --all --bytes=8 {}

```diff
@@ -1,10 +1,10 @@
 AWAVAUATUSH
 ([]A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 continued_fraction_to_fraction.c
 continued_fraction_to_fraction
 multiply
 .shstrtab
 .rela.text
 .comment
 .note.GNU-stack
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### cosine.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 000389 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 0006c0 0004f8 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 0003c9 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 0003c9 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 0003c9 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 0003f5 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 0003c9 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 0003f7 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 0003f8 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 000418 000068 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 000bb8 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 000480 0001b0 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 000630 000090 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 000bd0 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,9 +1,9 @@
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 cosine.c
 multiply
 check_accuracy
 increment_whole
 truncate
 __stack_chk_fail
 .shstrtab
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### exponential.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 0003a2 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 0006d8 000498 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 0003e2 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 0003e2 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 0003e2 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 00040e 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 0003e2 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000410 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000410 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 000430 000068 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 000b70 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 000498 0001b0 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 000648 00008e 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 000b88 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,10 +1,10 @@
 AWAVAUATUSH
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 exponential.c
 exponential
 remove_zeroes
 multiply
 truncate
 __stack_chk_fail
 .shstrtab
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### factorial.c.o

##### readelf --wide --sections {}

```diff
@@ -5,16 +5,16 @@
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 00034c 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 0006a0 0003a8 18   I 12   1  8
   [ 3] .data             PROGBITS        0000000000000000 00038c 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 00038c 000000 00  WA  0   0  1
   [ 5] .rodata.cst8      PROGBITS        0000000000000000 000390 000020 08  AM  0   0  8
   [ 6] .rodata.cst16     PROGBITS        0000000000000000 0003b0 000010 10  AM  0   0 16
-  [ 7] .comment          PROGBITS        0000000000000000 0003c0 00002c 01  MS  0   0  1
-  [ 8] .note.GNU-stack   PROGBITS        0000000000000000 0003ec 000000 00      0   0  1
+  [ 7] .comment          PROGBITS        0000000000000000 0003c0 00002e 01  MS  0   0  1
+  [ 8] .note.GNU-stack   PROGBITS        0000000000000000 0003ee 000000 00      0   0  1
   [ 9] .note.gnu.property NOTE            0000000000000000 0003f0 000020 00   A  0   0  8
   [10] .eh_frame         PROGBITS        0000000000000000 000410 000068 00   A  0   0  8
   [11] .rela.eh_frame    RELA            0000000000000000 000a48 000018 18   I 12  10  8
   [12] .symtab           SYMTAB          0000000000000000 000478 0001b0 18     13   8  8
   [13] .strtab           STRTAB          0000000000000000 000628 000075 00      0   0  1
   [14] .shstrtab         STRTAB          0000000000000000 000a60 000087 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,10 +1,10 @@
 AWAVAUATUSH
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 factorial.c
 factorial
 multiply
 __stack_chk_fail
 .shstrtab
 .rela.text
 .rodata.cst8
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### find_roots_of_polynomial.c.o

##### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              REL (Relocatable file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          0 (bytes into file)
-  Start of section headers:          12272 (bytes into file)
+  Start of section headers:          12280 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           0 (bytes)
   Number of program headers:         0
   Size of section headers:           64 (bytes)
   Number of section headers:         14
   Section header string table index: 13
```

##### readelf --wide --sections {}

```diff
@@ -1,23 +1,23 @@
-There are 14 section headers, starting at offset 0x2ff0:
+There are 14 section headers, starting at offset 0x2ff8:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 0013db 00  AX  0   0 16
-  [ 2] .rela.text        RELA            0000000000000000 001b48 0013c8 18   I 11   1  8
+  [ 2] .rela.text        RELA            0000000000000000 001b50 0013c8 18   I 11   1  8
   [ 3] .data             PROGBITS        0000000000000000 00141b 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 00141b 000000 00  WA  0   0  1
   [ 5] .rodata.str1.1    PROGBITS        0000000000000000 00141b 000008 01 AMS  0   0  1
-  [ 6] .comment          PROGBITS        0000000000000000 001423 00002c 01  MS  0   0  1
-  [ 7] .note.GNU-stack   PROGBITS        0000000000000000 00144f 000000 00      0   0  1
-  [ 8] .note.gnu.property NOTE            0000000000000000 001450 000020 00   A  0   0  8
-  [ 9] .eh_frame         PROGBITS        0000000000000000 001470 000150 00   A  0   0  8
-  [10] .rela.eh_frame    RELA            0000000000000000 002f10 000060 18   I 11   9  8
-  [11] .symtab           SYMTAB          0000000000000000 0015c0 000378 18     12   5  8
-  [12] .strtab           STRTAB          0000000000000000 001938 00020e 00      0   0  1
-  [13] .shstrtab         STRTAB          0000000000000000 002f70 00007b 00      0   0  1
+  [ 6] .comment          PROGBITS        0000000000000000 001423 00002e 01  MS  0   0  1
+  [ 7] .note.GNU-stack   PROGBITS        0000000000000000 001451 000000 00      0   0  1
+  [ 8] .note.gnu.property NOTE            0000000000000000 001458 000020 00   A  0   0  8
+  [ 9] .eh_frame         PROGBITS        0000000000000000 001478 000150 00   A  0   0  8
+  [10] .rela.eh_frame    RELA            0000000000000000 002f18 000060 18   I 11   9  8
+  [11] .symtab           SYMTAB          0000000000000000 0015c8 000378 18     12   5  8
+  [12] .strtab           STRTAB          0000000000000000 001940 00020e 00      0   0  1
+  [13] .shstrtab         STRTAB          0000000000000000 002f78 00007b 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --relocs {}

```diff
@@ -1,9 +1,9 @@
 
-Relocation section '.rela.text' at offset 0x1b48 contains 211 entries:
+Relocation section '.rela.text' at offset 0x1b50 contains 211 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000036  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
 0000000000000044  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
 000000000000004f  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
 000000000000005b  0000000800000004 R_X86_64_PLT32         0000000000000000 malloc - 4
 0000000000000071  0000000900000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
 000000000000007d  0000000a00000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
@@ -209,13 +209,13 @@
 000000000000137b  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
 000000000000138f  0000002200000004 R_X86_64_PLT32         0000000000000000 realloc - 4
 000000000000139a  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
 00000000000013aa  0000002300000004 R_X86_64_PLT32         0000000000000000 memmove - 4
 00000000000013c0  0000002300000004 R_X86_64_PLT32         0000000000000000 memmove - 4
 00000000000013d7  0000002400000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
 
-Relocation section '.rela.eh_frame' at offset 0x2f10 contains 4 entries:
+Relocation section '.rela.eh_frame' at offset 0x2f18 contains 4 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000020  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 0
 000000000000006c  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 180
 00000000000000b8  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 2d0
 0000000000000104  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 410
```

##### strings --all --bytes=8 {}

```diff
@@ -1,14 +1,14 @@
 AWAVAUE1
 []A\A]A^A_
 []A\A]A^A_
 AWAVAUATI
 ([]A\A]A^A_
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 find_roots_of_polynomial.c
 find_roots_of_polynomial_substitute
 multiply
 find_roots_of_polynomial_substitute_fraction
 parse_fraction
 multiply_fraction
 add_fraction
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### fraction_to_continued_fraction.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 0001f1 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 0004b8 0001e0 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 000231 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 000231 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 000231 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 00025d 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 000231 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 00025f 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000260 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 000280 000068 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 000698 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 0002e8 000138 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 000420 000094 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 0006b0 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,10 +1,10 @@
 AWAVAUATUSH
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 fraction_to_continued_fraction.c
 fraction_to_continued_fraction
 divide_whole_with_remainder
 .shstrtab
 .rela.text
 .comment
 .note.GNU-stack
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### igcd.c.o

##### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              REL (Relocatable file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          0 (bytes into file)
-  Start of section headers:          1784 (bytes into file)
+  Start of section headers:          1792 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           0 (bytes)
   Number of program headers:         0
   Size of section headers:           64 (bytes)
   Number of section headers:         13
   Section header string table index: 12
```

##### readelf --wide --sections {}

```diff
@@ -1,22 +1,22 @@
-There are 13 section headers, starting at offset 0x6f8:
+There are 13 section headers, starting at offset 0x700:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 00020c 00  AX  0   0 16
-  [ 2] .rela.text        RELA            0000000000000000 000490 0001e0 18   I 10   1  8
+  [ 2] .rela.text        RELA            0000000000000000 000498 0001e0 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 00024c 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 00024c 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 00024c 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000278 000000 00      0   0  1
-  [ 7] .note.gnu.property NOTE            0000000000000000 000278 000020 00   A  0   0  8
-  [ 8] .eh_frame         PROGBITS        0000000000000000 000298 000098 00   A  0   0  8
-  [ 9] .rela.eh_frame    RELA            0000000000000000 000670 000018 18   I 10   8  8
-  [10] .symtab           SYMTAB          0000000000000000 000330 000108 18     11   3  8
-  [11] .strtab           STRTAB          0000000000000000 000438 000051 00      0   0  1
-  [12] .shstrtab         STRTAB          0000000000000000 000688 00006c 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 00024c 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 00027a 000000 00      0   0  1
+  [ 7] .note.gnu.property NOTE            0000000000000000 000280 000020 00   A  0   0  8
+  [ 8] .eh_frame         PROGBITS        0000000000000000 0002a0 000098 00   A  0   0  8
+  [ 9] .rela.eh_frame    RELA            0000000000000000 000678 000018 18   I 10   8  8
+  [10] .symtab           SYMTAB          0000000000000000 000338 000108 18     11   3  8
+  [11] .strtab           STRTAB          0000000000000000 000440 000051 00      0   0  1
+  [12] .shstrtab         STRTAB          0000000000000000 000690 00006c 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --relocs {}

```diff
@@ -1,9 +1,9 @@
 
-Relocation section '.rela.text' at offset 0x490 contains 20 entries:
+Relocation section '.rela.text' at offset 0x498 contains 20 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000079  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen - 4
 000000000000008b  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen - 4
 00000000000000a2  0000000500000004 R_X86_64_PLT32         0000000000000000 calloc - 4
 00000000000000b2  0000000500000004 R_X86_64_PLT32         0000000000000000 calloc - 4
 00000000000000c2  0000000500000004 R_X86_64_PLT32         0000000000000000 calloc - 4
 00000000000000d2  0000000500000004 R_X86_64_PLT32         0000000000000000 calloc - 4
@@ -18,10 +18,10 @@
 000000000000019d  0000000a00000004 R_X86_64_PLT32         0000000000000000 free - 4
 00000000000001a5  0000000a00000004 R_X86_64_PLT32         0000000000000000 free - 4
 00000000000001ad  0000000a00000004 R_X86_64_PLT32         0000000000000000 free - 4
 00000000000001e8  0000000700000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
 00000000000001f8  0000000700000004 R_X86_64_PLT32         0000000000000000 strcpy - 4
 00000000000001c3  0000000a00000004 R_X86_64_PLT32         0000000000000000 free - 4
 
-Relocation section '.rela.eh_frame' at offset 0x670 contains 1 entry:
+Relocation section '.rela.eh_frame' at offset 0x678 contains 1 entry:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000020  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 0
```

##### strings --all --bytes=8 {}

```diff
@@ -1,10 +1,10 @@
 8[]A\A]A^A_
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 divide_whole_with_remainder
 .shstrtab
 .rela.text
 .comment
 .note.GNU-stack
 .note.gnu.property
 .rela.eh_frame
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### ilcm.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 0000a0 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 0002d8 0000d8 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 0000e0 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 0000e0 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 0000e0 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 00010c 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 0000e0 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 00010e 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000110 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 000130 000060 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 0003b0 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 000190 000108 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 000298 00003c 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 0003c8 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,9 +1,9 @@
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 multiply
 .shstrtab
 .rela.text
 .comment
 .note.GNU-stack
 .note.gnu.property
 .rela.eh_frame
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### natural_logarithm.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 000198 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 000488 0001f8 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 0001d8 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 0001d8 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 0001d8 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000204 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 0001d8 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000206 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000208 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 000228 000068 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 000680 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 000290 000168 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 0003f8 00008d 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 000698 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,9 +1,9 @@
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 natural_logarithm.c
 natural_logarithm
 power_integer
 square_root
 subtract
 multiply
 __stack_chk_fail
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### power.c.o

##### readelf --wide --sections {}

```diff
@@ -4,16 +4,16 @@
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 000234 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 000568 0002a0 18   I 11   1  8
   [ 3] .data             PROGBITS        0000000000000000 000274 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 000274 000000 00  WA  0   0  1
   [ 5] .rodata.cst8      PROGBITS        0000000000000000 000278 000018 08  AM  0   0  8
-  [ 6] .comment          PROGBITS        0000000000000000 000290 00002c 01  MS  0   0  1
-  [ 7] .note.GNU-stack   PROGBITS        0000000000000000 0002bc 000000 00      0   0  1
+  [ 6] .comment          PROGBITS        0000000000000000 000290 00002e 01  MS  0   0  1
+  [ 7] .note.GNU-stack   PROGBITS        0000000000000000 0002be 000000 00      0   0  1
   [ 8] .note.gnu.property NOTE            0000000000000000 0002c0 000020 00   A  0   0  8
   [ 9] .eh_frame         PROGBITS        0000000000000000 0002e0 000068 00   A  0   0  8
   [10] .rela.eh_frame    RELA            0000000000000000 000808 000018 18   I 11   9  8
   [11] .symtab           SYMTAB          0000000000000000 000348 000198 18     12   6  8
   [12] .strtab           STRTAB          0000000000000000 0004e0 000082 00      0   0  1
   [13] .shstrtab         STRTAB          0000000000000000 000820 000079 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,10 +1,10 @@
 AVAUATUH
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 remove_zeroes
 natural_logarithm
 multiply
 exponential
 power_integer
 .shstrtab
 .rela.text
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### power_integer.c.o

##### readelf --wide --sections {}

```diff
@@ -4,16 +4,16 @@
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 00018f 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 000430 000228 18   I 11   1  8
   [ 3] .data             PROGBITS        0000000000000000 0001cf 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 0001cf 000000 00  WA  0   0  1
   [ 5] .rodata.str1.1    PROGBITS        0000000000000000 0001cf 000002 01 AMS  0   0  1
-  [ 6] .comment          PROGBITS        0000000000000000 0001d1 00002c 01  MS  0   0  1
-  [ 7] .note.GNU-stack   PROGBITS        0000000000000000 0001fd 000000 00      0   0  1
+  [ 6] .comment          PROGBITS        0000000000000000 0001d1 00002e 01  MS  0   0  1
+  [ 7] .note.GNU-stack   PROGBITS        0000000000000000 0001ff 000000 00      0   0  1
   [ 8] .note.gnu.property NOTE            0000000000000000 000200 000020 00   A  0   0  8
   [ 9] .eh_frame         PROGBITS        0000000000000000 000220 000058 00   A  0   0  8
   [10] .rela.eh_frame    RELA            0000000000000000 000658 000018 18   I 11   9  8
   [11] .symtab           SYMTAB          0000000000000000 000278 000150 18     12   4  8
   [12] .strtab           STRTAB          0000000000000000 0003c8 000064 00      0   0  1
   [13] .shstrtab         STRTAB          0000000000000000 000670 00007b 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,8 +1,8 @@
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 power_integer.c
 power_integer
 multiply
 .shstrtab
 .rela.text
 .rodata.str1.1
 .comment
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### repeating_decimal_to_fraction.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 0001fd 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 0004b0 0001f8 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 00023d 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 00023d 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 00023d 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000269 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 00023d 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 00026b 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000270 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 000290 000068 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 0006a8 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 0002f8 000138 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 000430 000079 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 0006c0 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,9 +1,9 @@
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 repeating_decimal_to_fraction.c
 repeating_decimal_to_fraction
 multiply
 .shstrtab
 .rela.text
 .comment
 .note.GNU-stack
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### simplify_arithmetic_expression.c.o

##### readelf --wide --sections {}

```diff
@@ -4,16 +4,16 @@
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 002084 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 002cc0 001620 18   I 11   1  8
   [ 3] .data             PROGBITS        0000000000000000 0020c4 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 0020c4 000000 00  WA  0   0  1
   [ 5] .rodata.str1.1    PROGBITS        0000000000000000 0020c4 000039 01 AMS  0   0  1
-  [ 6] .comment          PROGBITS        0000000000000000 0020fd 00002c 01  MS  0   0  1
-  [ 7] .note.GNU-stack   PROGBITS        0000000000000000 002129 000000 00      0   0  1
+  [ 6] .comment          PROGBITS        0000000000000000 0020fd 00002e 01  MS  0   0  1
+  [ 7] .note.GNU-stack   PROGBITS        0000000000000000 00212b 000000 00      0   0  1
   [ 8] .note.gnu.property NOTE            0000000000000000 002130 000020 00   A  0   0  8
   [ 9] .eh_frame         PROGBITS        0000000000000000 002150 000280 00   A  0   0  8
   [10] .rela.eh_frame    RELA            0000000000000000 0042e0 0000c0 18   I 11   9  8
   [11] .symtab           SYMTAB          0000000000000000 0023d0 000600 18     12  35  8
   [12] .strtab           STRTAB          0000000000000000 0029d0 0002ea 00      0   0  1
   [13] .shstrtab         STRTAB          0000000000000000 0043a0 00007b 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -6,15 +6,15 @@
 []A\A]A^
 []A\A]A^A_
 []A\A]A^A_
 AWAVAUE1
 ([]A\A]A^A_
 D$`H;D$p
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 simplify_arithmetic_expression.c
 str_replace_all
 replace_substring_from_position
 find_operational_sign
 remove_misplaced_and_redundant_signs
 get_numerical_arguments.constprop.1
 get_numerical_arguments.constprop.0
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### sine.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 0004fa 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 000828 000678 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 00053a 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 00053a 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 00053a 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000566 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 00053a 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000568 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000568 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 000588 000068 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 000ea0 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 0005f0 0001b0 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 0007a0 000082 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 000eb8 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,9 +1,9 @@
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 multiply
 subtract
 increment_whole
 __stack_chk_fail
 .shstrtab
 .rela.text
 .comment
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### square_root.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 000560 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 000870 000648 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 0005a0 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 0005a0 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 0005a0 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 0005cc 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 0005a0 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 0005ce 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 0005d0 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 0005f0 000068 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 000eb8 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 000658 000198 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 0007f0 00007e 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 000ed0 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,10 +1,10 @@
 AWAVAUATI
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 square_root.c
 square_root
 multiply
 subtract
 remove_zeroes
 .shstrtab
 .rela.text
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### tangent.c.o

##### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              REL (Relocatable file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          0 (bytes into file)
-  Start of section headers:          976 (bytes into file)
+  Start of section headers:          984 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           0 (bytes)
   Number of program headers:         0
   Size of section headers:           64 (bytes)
   Number of section headers:         13
   Section header string table index: 12
```

##### readelf --wide --sections {}

```diff
@@ -1,22 +1,22 @@
-There are 13 section headers, starting at offset 0x3d0:
+There are 13 section headers, starting at offset 0x3d8:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 000083 00  AX  0   0 16
-  [ 2] .rela.text        RELA            0000000000000000 000288 0000c0 18   I 10   1  8
+  [ 2] .rela.text        RELA            0000000000000000 000290 0000c0 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 0000c3 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 0000c3 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 0000c3 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 0000ef 000000 00      0   0  1
-  [ 7] .note.gnu.property NOTE            0000000000000000 0000f0 000020 00   A  0   0  8
-  [ 8] .eh_frame         PROGBITS        0000000000000000 000110 000050 00   A  0   0  8
-  [ 9] .rela.eh_frame    RELA            0000000000000000 000348 000018 18   I 10   8  8
-  [10] .symtab           SYMTAB          0000000000000000 000160 0000f0 18     11   3  8
-  [11] .strtab           STRTAB          0000000000000000 000250 000034 00      0   0  1
-  [12] .shstrtab         STRTAB          0000000000000000 000360 00006c 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 0000c3 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 0000f1 000000 00      0   0  1
+  [ 7] .note.gnu.property NOTE            0000000000000000 0000f8 000020 00   A  0   0  8
+  [ 8] .eh_frame         PROGBITS        0000000000000000 000118 000050 00   A  0   0  8
+  [ 9] .rela.eh_frame    RELA            0000000000000000 000350 000018 18   I 10   8  8
+  [10] .symtab           SYMTAB          0000000000000000 000168 0000f0 18     11   3  8
+  [11] .strtab           STRTAB          0000000000000000 000258 000034 00      0   0  1
+  [12] .shstrtab         STRTAB          0000000000000000 000368 00006c 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --relocs {}

```diff
@@ -1,15 +1,15 @@
 
-Relocation section '.rela.text' at offset 0x288 contains 8 entries:
+Relocation section '.rela.text' at offset 0x290 contains 8 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000016  0000000400000004 R_X86_64_PLT32         0000000000000000 sine - 4
 0000000000000024  0000000500000004 R_X86_64_PLT32         0000000000000000 cosine - 4
 000000000000002f  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
 000000000000003a  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
 000000000000004c  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
 0000000000000060  0000000800000004 R_X86_64_PLT32         0000000000000000 divide - 4
 0000000000000068  0000000900000004 R_X86_64_PLT32         0000000000000000 free - 4
 0000000000000070  0000000900000004 R_X86_64_PLT32         0000000000000000 free - 4
 
-Relocation section '.rela.eh_frame' at offset 0x348 contains 1 entry:
+Relocation section '.rela.eh_frame' at offset 0x350 contains 1 entry:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000020  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 0
```

##### strings --all --bytes=8 {}

```diff
@@ -1,8 +1,8 @@
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 tangent.c
 .shstrtab
 .rela.text
 .comment
 .note.GNU-stack
 .note.gnu.property
 .rela.eh_frame
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### terminating_decimal_to_fraction.c.o

##### readelf --wide --sections {}

```diff
@@ -4,16 +4,16 @@
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 0002a5 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 000590 000180 18   I 11   1  8
   [ 3] .data             PROGBITS        0000000000000000 0002e5 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 0002e5 000000 00  WA  0   0  1
   [ 5] .rodata.cst16     PROGBITS        0000000000000000 0002f0 000010 10  AM  0   0 16
-  [ 6] .comment          PROGBITS        0000000000000000 000300 00002c 01  MS  0   0  1
-  [ 7] .note.GNU-stack   PROGBITS        0000000000000000 00032c 000000 00      0   0  1
+  [ 6] .comment          PROGBITS        0000000000000000 000300 00002e 01  MS  0   0  1
+  [ 7] .note.GNU-stack   PROGBITS        0000000000000000 00032e 000000 00      0   0  1
   [ 8] .note.gnu.property NOTE            0000000000000000 000330 000020 00   A  0   0  8
   [ 9] .eh_frame         PROGBITS        0000000000000000 000350 000068 00   A  0   0  8
   [10] .rela.eh_frame    RELA            0000000000000000 000710 000018 18   I 11   9  8
   [11] .symtab           SYMTAB          0000000000000000 0003b8 000150 18     12   5  8
   [12] .strtab           STRTAB          0000000000000000 000508 000082 00      0   0  1
   [13] .shstrtab         STRTAB          0000000000000000 000728 00007a 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,10 +1,10 @@
 []A\A]A^A_
 0000000000000000
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 terminating_decimal_to_fraction.c
 terminating_decimal_to_fraction
 .shstrtab
 .rela.text
 .rodata.cst16
 .comment
 .note.GNU-stack
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### Fraction.cpp.o

##### readelf --wide --sections {}

```diff
@@ -14,16 +14,16 @@
   [ 9] .gcc_except_table PROGBITS        0000000000000000 001788 00015f 00   A  0   0  1
   [10] .rodata.str1.8    PROGBITS        0000000000000000 0018e8 00002a 01 AMS  0   0  8
   [11] .rodata.str1.1    PROGBITS        0000000000000000 001912 00001e 01 AMS  0   0  1
   [12] .text._ZN11arithmetica8FractionD2Ev PROGBITS        0000000000000000 001930 000042 00 AXG  0   0 16
   [13] .rela.text._ZN11arithmetica8FractionD2Ev RELA            0000000000000000 0042a0 000030 18  IG 21  12  8
   [14] .data.rel.local.DW.ref.__gxx_personality_v0 PROGBITS        0000000000000000 001978 000008 00 WAG  0   0  8
   [15] .rela.data.rel.local.DW.ref.__gxx_personality_v0 RELA            0000000000000000 0042d0 000018 18  IG 21  14  8
-  [16] .comment          PROGBITS        0000000000000000 001980 00002c 01  MS  0   0  1
-  [17] .note.GNU-stack   PROGBITS        0000000000000000 0019ac 000000 00      0   0  1
+  [16] .comment          PROGBITS        0000000000000000 001980 00002e 01  MS  0   0  1
+  [17] .note.GNU-stack   PROGBITS        0000000000000000 0019ae 000000 00      0   0  1
   [18] .note.gnu.property NOTE            0000000000000000 0019b0 000020 00   A  0   0  8
   [19] .eh_frame         PROGBITS        0000000000000000 0019d0 000588 00   A  0   0  8
   [20] .rela.eh_frame    RELA            0000000000000000 0042e8 000438 18   I 21  19  8
   [21] .symtab           SYMTAB          0000000000000000 001f58 000630 18     22  23  8
   [22] .strtab           STRTAB          0000000000000000 002588 000848 00      0   0  1
   [23] .shstrtab         STRTAB          0000000000000000 004720 000111 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -11,15 +11,15 @@
 AWAVAUATUH
 []A\A]A^A_
 AWAVAUATUH
 []A\A]A^A_
 []A\A]A^A_
 basic_string::_M_construct null not valid
 basic_string::append
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 Fraction.cpp
 _ZN11arithmetica8FractionC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEES8_.cold
 _ZN11arithmetica8FractionC2ERKNSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE.cold
 _ZN11arithmetica8FractionC2EPKc.cold
 _ZN11arithmetica8FractionC2ERK8fraction.cold
 _ZN11arithmetica8Fraction9to_stringB5cxx11Ev.cold
 _ZN11arithmetica8FractionplERKS0_.cold
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### fraction.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 000096 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 0002c8 0000c0 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 0000d6 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 0000d6 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 0000d6 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000102 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 0000d6 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000104 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000108 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 000128 000080 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 000388 000030 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 0001a8 0000d8 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 000280 000046 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 0003b8 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,10 +1,10 @@
 AVAUATUH
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 fraction.c
 create_fraction
 delete_fraction
 .shstrtab
 .rela.text
 .comment
 .note.GNU-stack
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### add_fraction.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 000132 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 000398 0001b0 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 000172 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 000172 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 000172 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 00019e 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 000172 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 0001a0 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 0001a0 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 0001c0 000068 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 000548 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 000228 000108 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 000330 000066 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 000560 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,9 +1,9 @@
 ([]A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 add_fraction.c
 add_fraction
 multiply
 simplify_parsed_fraction
 delete_fraction
 .shstrtab
 .rela.text
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### multiply_fraction.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 0000b2 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 0002e0 0000f0 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 0000f2 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 0000f2 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 0000f2 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 00011e 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 0000f2 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000120 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000120 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 000140 000060 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 0003d0 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 0001a0 0000d8 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 000278 000067 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 0003e8 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,9 +1,9 @@
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 multiply_fraction.c
 multiply_fraction
 multiply
 simplify_parsed_fraction
 delete_fraction
 .shstrtab
 .rela.text
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### parse_fraction.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 000315 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 0006d8 0002d0 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 000355 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 000355 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 000355 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000381 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 000355 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000383 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000388 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 0003a8 0000b0 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 0009a8 000030 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 000458 0001b0 18     11   4  8
   [11] .strtab           STRTAB          0000000000000000 000608 0000cb 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 0009d8 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,11 +1,11 @@
 []A\A]A^A_
 AVAUATUH
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 parse_fraction.c
 return_decimals_and_remove_decimal_point
 parse_fraction
 simplify_parsed_fraction
 delete_fraction
 __stack_chk_fail
 .shstrtab
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### power_fraction.c.o

##### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              REL (Relocatable file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          0 (bytes into file)
-  Start of section headers:          3544 (bytes into file)
+  Start of section headers:          3840 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           0 (bytes)
   Number of program headers:         0
   Size of section headers:           64 (bytes)
-  Number of section headers:         13
-  Section header string table index: 12
+  Number of section headers:         14
+  Section header string table index: 13
```

##### readelf --wide --sections {}

```diff
@@ -1,22 +1,23 @@
-There are 13 section headers, starting at offset 0xdd8:
+There are 14 section headers, starting at offset 0xf00:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
-  [ 1] .text             PROGBITS        0000000000000000 000040 0004c3 00  AX  0   0 16
-  [ 2] .rela.text        RELA            0000000000000000 000870 0004c8 18   I 10   1  8
-  [ 3] .data             PROGBITS        0000000000000000 000503 000000 00  WA  0   0  1
-  [ 4] .bss              NOBITS          0000000000000000 000503 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 000503 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 00052f 000000 00      0   0  1
-  [ 7] .note.gnu.property NOTE            0000000000000000 000530 000020 00   A  0   0  8
-  [ 8] .eh_frame         PROGBITS        0000000000000000 000550 000090 00   A  0   0  8
-  [ 9] .rela.eh_frame    RELA            0000000000000000 000d38 000030 18   I 10   8  8
-  [10] .symtab           SYMTAB          0000000000000000 0005e0 0001c8 18     11   3  8
-  [11] .strtab           STRTAB          0000000000000000 0007a8 0000c7 00      0   0  1
-  [12] .shstrtab         STRTAB          0000000000000000 000d68 00006c 00      0   0  1
+  [ 1] .text             PROGBITS        0000000000000000 000040 000513 00  AX  0   0 16
+  [ 2] .rela.text        RELA            0000000000000000 000928 000528 18   I 11   1  8
+  [ 3] .data             PROGBITS        0000000000000000 000553 000000 00  WA  0   0  1
+  [ 4] .bss              NOBITS          0000000000000000 000553 000000 00  WA  0   0  1
+  [ 5] .rodata.str1.1    PROGBITS        0000000000000000 000553 000004 01 AMS  0   0  1
+  [ 6] .comment          PROGBITS        0000000000000000 000557 00002e 01  MS  0   0  1
+  [ 7] .note.GNU-stack   PROGBITS        0000000000000000 000585 000000 00      0   0  1
+  [ 8] .note.gnu.property NOTE            0000000000000000 000588 000020 00   A  0   0  8
+  [ 9] .eh_frame         PROGBITS        0000000000000000 0005a8 000090 00   A  0   0  8
+  [10] .rela.eh_frame    RELA            0000000000000000 000e50 000030 18   I 11   9  8
+  [11] .symtab           SYMTAB          0000000000000000 000638 000210 18     12   4  8
+  [12] .strtab           STRTAB          0000000000000000 000848 0000df 00      0   0  1
+  [13] .shstrtab         STRTAB          0000000000000000 000e80 00007b 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --symbols {}

```diff
@@ -1,22 +1,25 @@
 
-Symbol table '.symtab' contains 19 entries:
+Symbol table '.symtab' contains 22 entries:
    Num:    Value          Size Type    Bind   Vis      Ndx Name
      0: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT  UND 
      1: 0000000000000000     0 FILE    LOCAL  DEFAULT  ABS power_fraction.c
      2: 0000000000000000     0 SECTION LOCAL  DEFAULT    1 .text
-     3: 0000000000000000   226 FUNC    GLOBAL DEFAULT    1 arithmetica_power_fraction_round_decimal
-     4: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strchr
-     5: 00000000000000f0   979 FUNC    GLOBAL DEFAULT    1 power_fraction
-     6: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strlen
-     7: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND calloc
-     8: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memcpy
-     9: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND divide
-    10: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND power
-    11: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strncpy
-    12: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND parse_fraction
-    13: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND free
-    14: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND delete_fraction
-    15: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memmove
-    16: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND realloc
-    17: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND stpcpy
-    18: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND __stack_chk_fail
+     3: 0000000000000000     0 NOTYPE  LOCAL  DEFAULT    5 .LC0
+     4: 0000000000000000   226 FUNC    GLOBAL DEFAULT    1 arithmetica_power_fraction_round_decimal
+     5: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strchr
+     6: 00000000000000f0  1059 FUNC    GLOBAL DEFAULT    1 power_fraction
+     7: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strlen
+     8: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND calloc
+     9: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memcpy
+    10: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND divide
+    11: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strcmp
+    12: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND square_root
+    13: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND strncpy
+    14: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND parse_fraction
+    15: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND free
+    16: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND delete_fraction
+    17: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND power
+    18: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND memmove
+    19: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND realloc
+    20: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND stpcpy
+    21: 0000000000000000     0 NOTYPE  GLOBAL DEFAULT  UND __stack_chk_fail
```

##### readelf --wide --relocs {}

```diff
@@ -1,59 +1,63 @@
 
-Relocation section '.rela.text' at offset 0x870 contains 51 entries:
+Relocation section '.rela.text' at offset 0x928 contains 55 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
-0000000000000011  0000000400000004 R_X86_64_PLT32         0000000000000000 strchr - 4
-0000000000000128  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-000000000000013e  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000152  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-000000000000016c  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-000000000000017c  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000197  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-00000000000001a7  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-00000000000001c2  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-00000000000001d5  0000000800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-00000000000001e6  0000000800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-00000000000001f8  0000000800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-000000000000020a  0000000800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-0000000000000220  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000234  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000249  0000000900000004 R_X86_64_PLT32         0000000000000000 divide - 4
-0000000000000258  0000000a00000004 R_X86_64_PLT32         0000000000000000 power - 4
-0000000000000274  0000000a00000004 R_X86_64_PLT32         0000000000000000 power - 4
-0000000000000286  0000000300000004 R_X86_64_PLT32         0000000000000000 arithmetica_power_fraction_round_decimal - 4
-0000000000000293  0000000300000004 R_X86_64_PLT32         0000000000000000 arithmetica_power_fraction_round_decimal - 4
-00000000000002a4  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-00000000000002b9  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-00000000000002c8  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-00000000000002da  0000000b00000004 R_X86_64_PLT32         0000000000000000 strncpy - 4
-00000000000002eb  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000301  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-000000000000030e  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen - 4
-0000000000000320  0000000b00000004 R_X86_64_PLT32         0000000000000000 strncpy - 4
-0000000000000328  0000000c00000004 R_X86_64_PLT32         0000000000000000 parse_fraction - 4
-000000000000033b  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000345  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-000000000000034f  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000357  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000362  0000000e00000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-000000000000036d  0000000e00000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
-00000000000003b1  0000000f00000004 R_X86_64_PLT32         0000000000000000 memmove - 4
-00000000000003cf  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-00000000000003e2  0000000800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-00000000000003ee  0000001000000004 R_X86_64_PLT32         0000000000000000 realloc - 4
-0000000000000400  0000000800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-000000000000040b  0000001000000004 R_X86_64_PLT32         0000000000000000 realloc - 4
-0000000000000425  0000000800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-000000000000042e  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-0000000000000446  0000000700000004 R_X86_64_PLT32         0000000000000000 calloc - 4
-0000000000000458  0000001100000004 R_X86_64_PLT32         0000000000000000 stpcpy - 4
-000000000000046c  0000001000000004 R_X86_64_PLT32         0000000000000000 realloc - 4
-000000000000047f  0000000800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-000000000000049a  0000001000000004 R_X86_64_PLT32         0000000000000000 realloc - 4
-00000000000004ac  0000000800000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
-00000000000004b5  0000000d00000004 R_X86_64_PLT32         0000000000000000 free - 4
-00000000000004bf  0000001200000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
+0000000000000011  0000000500000004 R_X86_64_PLT32         0000000000000000 strchr - 4
+0000000000000128  0000000700000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+000000000000013e  0000000800000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000152  0000000700000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+000000000000016c  0000000800000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+000000000000017c  0000000700000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000197  0000000800000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000001a7  0000000700000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+00000000000001c2  0000000800000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000001d5  0000000900000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+00000000000001e6  0000000900000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+00000000000001f8  0000000900000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+000000000000020a  0000000900000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+000000000000021c  0000000700000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000230  0000000800000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+000000000000024c  0000000a00000004 R_X86_64_PLT32         0000000000000000 divide - 4
+0000000000000253  0000000300000002 R_X86_64_PC32          0000000000000000 .LC0 - 4
+000000000000025b  0000000b00000004 R_X86_64_PLT32         0000000000000000 strcmp - 4
+0000000000000272  0000000c00000004 R_X86_64_PLT32         0000000000000000 square_root - 4
+0000000000000283  0000000c00000004 R_X86_64_PLT32         0000000000000000 square_root - 4
+0000000000000295  0000000400000004 R_X86_64_PLT32         0000000000000000 arithmetica_power_fraction_round_decimal - 4
+00000000000002a2  0000000400000004 R_X86_64_PLT32         0000000000000000 arithmetica_power_fraction_round_decimal - 4
+00000000000002b4  0000000700000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+00000000000002ca  0000000700000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+00000000000002dd  0000000800000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000002f8  0000000d00000004 R_X86_64_PLT32         0000000000000000 strncpy - 4
+0000000000000309  0000000700000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000318  0000000700000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+0000000000000326  0000000700000004 R_X86_64_PLT32         0000000000000000 strlen - 4
+000000000000033d  0000000d00000004 R_X86_64_PLT32         0000000000000000 strncpy - 4
+0000000000000345  0000000e00000004 R_X86_64_PLT32         0000000000000000 parse_fraction - 4
+0000000000000356  0000000f00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000360  0000000f00000004 R_X86_64_PLT32         0000000000000000 free - 4
+000000000000036a  0000000f00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000372  0000000f00000004 R_X86_64_PLT32         0000000000000000 free - 4
+000000000000037d  0000001000000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+0000000000000388  0000001000000004 R_X86_64_PLT32         0000000000000000 delete_fraction - 4
+00000000000003ce  0000001100000004 R_X86_64_PLT32         0000000000000000 power - 4
+00000000000003e2  0000001100000004 R_X86_64_PLT32         0000000000000000 power - 4
+0000000000000401  0000001200000004 R_X86_64_PLT32         0000000000000000 memmove - 4
+000000000000041f  0000000800000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+0000000000000432  0000000900000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+000000000000043e  0000001300000004 R_X86_64_PLT32         0000000000000000 realloc - 4
+0000000000000450  0000000900000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+000000000000045b  0000001300000004 R_X86_64_PLT32         0000000000000000 realloc - 4
+0000000000000475  0000000900000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+000000000000047e  0000000f00000004 R_X86_64_PLT32         0000000000000000 free - 4
+0000000000000496  0000000800000004 R_X86_64_PLT32         0000000000000000 calloc - 4
+00000000000004a8  0000001400000004 R_X86_64_PLT32         0000000000000000 stpcpy - 4
+00000000000004bc  0000001300000004 R_X86_64_PLT32         0000000000000000 realloc - 4
+00000000000004cf  0000000900000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+00000000000004ea  0000001300000004 R_X86_64_PLT32         0000000000000000 realloc - 4
+00000000000004fc  0000000900000004 R_X86_64_PLT32         0000000000000000 memcpy - 4
+0000000000000505  0000000f00000004 R_X86_64_PLT32         0000000000000000 free - 4
+000000000000050f  0000001500000004 R_X86_64_PLT32         0000000000000000 __stack_chk_fail - 4
 
-Relocation section '.rela.eh_frame' at offset 0xd38 contains 2 entries:
+Relocation section '.rela.eh_frame' at offset 0xe50 contains 2 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000020  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 0
 0000000000000044  0000000200000002 R_X86_64_PC32          0000000000000000 .text + f0
```

##### readelf --wide --debug-dump=frames {}

```diff
@@ -24,15 +24,15 @@
   DW_CFA_restore_state
   DW_CFA_advance_loc1: 101 to 00000000000000c5
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 8
   DW_CFA_advance_loc: 11 to 00000000000000d0
   DW_CFA_restore_state
 
-0000003c 0000000000000050 00000040 FDE cie=00000000 pc=00000000000000f0..00000000000004c3
+0000003c 0000000000000050 00000040 FDE cie=00000000 pc=00000000000000f0..0000000000000513
   DW_CFA_advance_loc: 6 to 00000000000000f6
   DW_CFA_def_cfa_offset: 16
   DW_CFA_offset: r15 (r15) at cfa-16
   DW_CFA_advance_loc: 5 to 00000000000000fb
   DW_CFA_def_cfa_offset: 24
   DW_CFA_offset: r14 (r14) at cfa-24
   DW_CFA_advance_loc: 5 to 0000000000000100
@@ -45,30 +45,30 @@
   DW_CFA_def_cfa_offset: 48
   DW_CFA_offset: r6 (rbp) at cfa-48
   DW_CFA_advance_loc: 4 to 0000000000000107
   DW_CFA_def_cfa_offset: 56
   DW_CFA_offset: r3 (rbx) at cfa-56
   DW_CFA_advance_loc: 7 to 000000000000010e
   DW_CFA_def_cfa_offset: 192
-  DW_CFA_advance_loc2: 647 to 0000000000000395
+  DW_CFA_advance_loc2: 674 to 00000000000003b0
   DW_CFA_remember_state
   DW_CFA_def_cfa_offset: 56
-  DW_CFA_advance_loc: 1 to 0000000000000396
+  DW_CFA_advance_loc: 1 to 00000000000003b1
   DW_CFA_def_cfa_offset: 48
-  DW_CFA_advance_loc: 1 to 0000000000000397
+  DW_CFA_advance_loc: 1 to 00000000000003b2
   DW_CFA_def_cfa_offset: 40
-  DW_CFA_advance_loc: 2 to 0000000000000399
+  DW_CFA_advance_loc: 2 to 00000000000003b4
   DW_CFA_def_cfa_offset: 32
-  DW_CFA_advance_loc: 2 to 000000000000039b
+  DW_CFA_advance_loc: 2 to 00000000000003b6
   DW_CFA_def_cfa_offset: 24
-  DW_CFA_advance_loc: 2 to 000000000000039d
+  DW_CFA_advance_loc: 2 to 00000000000003b8
   DW_CFA_def_cfa_offset: 16
-  DW_CFA_advance_loc: 2 to 000000000000039f
+  DW_CFA_advance_loc: 2 to 00000000000003ba
   DW_CFA_def_cfa_offset: 8
-  DW_CFA_advance_loc: 1 to 00000000000003a0
+  DW_CFA_advance_loc: 6 to 00000000000003c0
   DW_CFA_restore_state
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
   DW_CFA_nop
```

##### strings --all --bytes=8 {}

```diff
@@ -1,14 +1,16 @@
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 power_fraction.c
 arithmetica_power_fraction_round_decimal
 power_fraction
+square_root
 parse_fraction
 delete_fraction
 __stack_chk_fail
 .shstrtab
 .rela.text
+.rodata.str1.1
 .comment
 .note.GNU-stack
 .note.gnu.property
 .rela.eh_frame
```

##### objdump --line-numbers --disassemble --demangle --reloc --no-show-raw-insn --section=.text {}

```diff
@@ -156,212 +156,234 @@
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x28(%rsp),%rdx
 	mov    0x20(%rsp),%rsi
 	mov    %r15,%rdi
 	call   20e <power_fraction+0x11e>
  R_X86_64_PLT32	memcpy-0x4
 	cmpb   $0x2d,0x0(%rbp)
-	je     3a0 <power_fraction+0x2b0>
+	je     3f0 <power_fraction+0x300>
 	mov    %rbp,%rdi
-	lea    0x3(%r14),%rbx
-	call   224 <power_fraction+0x134>
+	call   220 <power_fraction+0x130>
  R_X86_64_PLT32	strlen-0x4
 	mov    $0x1,%esi
 	lea    0x6(%r14,%rax,1),%rdi
 	add    0x10(%rsp),%rdi
-	call   238 <power_fraction+0x148>
+	call   234 <power_fraction+0x144>
  R_X86_64_PLT32	calloc-0x4
-	mov    %rbx,%rcx
+	lea    0x3(%r14),%r8
 	mov    %r15,%rsi
 	mov    %rbp,%rdi
+	mov    %rax,%rbx
+	mov    %r8,%rcx
 	mov    %rax,%rdx
-	mov    %rax,(%rsp)
-	call   24d <power_fraction+0x15d>
+	mov    %r8,(%rsp)
+	call   250 <power_fraction+0x160>
  R_X86_64_PLT32	divide-0x4
-	mov    (%rsp),%rsi
-	mov    %rbx,%rdx
-	mov    %r12,%rdi
-	call   25c <power_fraction+0x16c>
- R_X86_64_PLT32	power-0x4
+	lea    0x0(%rip),%rsi        
+ R_X86_64_PC32	.LC0-0x4
+	mov    %rbx,%rdi
+	call   25f <power_fraction+0x16f>
+ R_X86_64_PLT32	strcmp-0x4
 	mov    (%rsp),%r8
-	mov    %rbx,%rdx
+	test   %eax,%eax
+	jne    3c0 <power_fraction+0x2d0>
+	mov    %r8,%rsi
+	mov    %r12,%rdi
+	call   276 <power_fraction+0x186>
+ R_X86_64_PLT32	square_root-0x4
+	mov    (%rsp),%rsi
 	mov    %r13,%rdi
 	mov    %rax,0x68(%rsp)
-	mov    %r8,%rsi
-	mov    %r8,0x20(%rsp)
-	call   278 <power_fraction+0x188>
- R_X86_64_PLT32	power-0x4
+	call   287 <power_fraction+0x197>
+ R_X86_64_PLT32	square_root-0x4
 	mov    %r14,%rsi
 	lea    0x68(%rsp),%rdi
 	mov    %rax,0x70(%rsp)
-	call   28a <power_fraction+0x19a>
+	call   299 <power_fraction+0x1a9>
  R_X86_64_PLT32	arithmetica_power_fraction_round_decimal-0x4
 	mov    %r14,%rsi
 	lea    0x70(%rsp),%rdi
-	call   297 <power_fraction+0x1a7>
+	call   2a6 <power_fraction+0x1b6>
  R_X86_64_PLT32	arithmetica_power_fraction_round_decimal-0x4
 	mov    0x68(%rsp),%r9
 	mov    %r9,%rdi
-	mov    %r9,(%rsp)
-	call   2a8 <power_fraction+0x1b8>
+	mov    %r9,0x18(%rsp)
+	call   2b8 <power_fraction+0x1c8>
  R_X86_64_PLT32	strlen-0x4
 	mov    0x70(%rsp),%r10
-	mov    %rax,%rbx
+	mov    %rax,(%rsp)
 	mov    %r10,%rdi
-	mov    %r10,0x18(%rsp)
-	call   2bd <power_fraction+0x1cd>
+	mov    %r10,0x10(%rsp)
+	call   2ce <power_fraction+0x1de>
  R_X86_64_PLT32	strlen-0x4
+	mov    (%rsp),%rdx
 	mov    $0x1,%esi
-	lea    0x2(%rbx,%rax,1),%rdi
-	call   2cc <power_fraction+0x1dc>
+	lea    0x2(%rdx,%rax,1),%rdi
+	call   2e1 <power_fraction+0x1f1>
  R_X86_64_PLT32	calloc-0x4
-	mov    (%rsp),%rsi
-	mov    %rbx,%rdx
+	mov    0x18(%rsp),%r9
+	mov    (%rsp),%rdx
 	mov    %rax,%rdi
 	mov    %rax,%r14
-	call   2de <power_fraction+0x1ee>
+	mov    %r9,%rsi
+	mov    %r9,(%rsp)
+	call   2fc <power_fraction+0x20c>
  R_X86_64_PLT32	strncpy-0x4
 	mov    (%rsp),%r9
 	mov    %r9,%rdi
-	mov    %r9,0x10(%rsp)
-	call   2ef <power_fraction+0x1ff>
+	mov    %r9,0x18(%rsp)
+	call   30d <power_fraction+0x21d>
  R_X86_64_PLT32	strlen-0x4
-	mov    0x18(%rsp),%r10
+	mov    0x10(%rsp),%rdi
 	movb   $0x2f,(%r14,%rax,1)
-	mov    %r10,%rdi
-	mov    %r10,(%rsp)
-	call   305 <power_fraction+0x215>
+	call   31c <power_fraction+0x22c>
  R_X86_64_PLT32	strlen-0x4
-	mov    0x10(%rsp),%rdi
-	mov    %rax,%rbx
-	call   312 <power_fraction+0x222>
+	mov    0x18(%rsp),%rdi
+	mov    %rax,(%rsp)
+	call   32a <power_fraction+0x23a>
  R_X86_64_PLT32	strlen-0x4
-	mov    (%rsp),%rsi
-	lea    0x1(%rbx),%rdx
+	mov    (%rsp),%rdx
+	mov    0x10(%rsp),%rsi
 	lea    0x1(%r14,%rax,1),%rdi
-	call   324 <power_fraction+0x234>
+	add    $0x1,%rdx
+	call   341 <power_fraction+0x251>
  R_X86_64_PLT32	strncpy-0x4
 	mov    %r14,%rdi
-	call   32c <power_fraction+0x23c>
+	call   349 <power_fraction+0x259>
  R_X86_64_PLT32	parse_fraction-0x4
-	mov    0x20(%rsp),%rdi
+	mov    %rbx,%rdi
 	mov    %rax,(%rsp)
 	mov    %rdx,0x8(%rsp)
-	call   33f <power_fraction+0x24f>
+	call   35a <power_fraction+0x26a>
  R_X86_64_PLT32	free-0x4
 	mov    0x68(%rsp),%rdi
-	call   349 <power_fraction+0x259>
+	call   364 <power_fraction+0x274>
  R_X86_64_PLT32	free-0x4
 	mov    0x70(%rsp),%rdi
-	call   353 <power_fraction+0x263>
+	call   36e <power_fraction+0x27e>
  R_X86_64_PLT32	free-0x4
 	mov    %r14,%rdi
-	call   35b <power_fraction+0x26b>
+	call   376 <power_fraction+0x286>
  R_X86_64_PLT32	free-0x4
 	mov    %r12,%rdi
 	mov    %r13,%rsi
-	call   366 <power_fraction+0x276>
+	call   381 <power_fraction+0x291>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    %rbp,%rdi
 	mov    %r15,%rsi
-	call   371 <power_fraction+0x281>
+	call   38c <power_fraction+0x29c>
  R_X86_64_PLT32	delete_fraction-0x4
 	mov    (%rsp),%rax
 	mov    0x8(%rsp),%rdx
 	mov    0x78(%rsp),%rcx
 	sub    %fs:0x28,%rcx
-	jne    4be <power_fraction+0x3ce>
+	jne    50e <power_fraction+0x41e>
 	add    $0x88,%rsp
 	pop    %rbx
 	pop    %rbp
 	pop    %r12
 	pop    %r13
 	pop    %r14
 	pop    %r15
 	ret
+	nopl   0x0(%rax,%rax,1)
+	mov    %r8,%rdx
+	mov    %rbx,%rsi
+	mov    %r12,%rdi
+	mov    %r8,(%rsp)
+	call   3d2 <power_fraction+0x2e2>
+ R_X86_64_PLT32	power-0x4
+	mov    (%rsp),%rdx
+	mov    %rbx,%rsi
+	mov    %r13,%rdi
+	mov    %rax,0x68(%rsp)
+	call   3e6 <power_fraction+0x2f6>
+ R_X86_64_PLT32	power-0x4
+	jmp    287 <power_fraction+0x197>
+	nopl   0x0(%rax,%rax,1)
 	mov    0x48(%rsp),%rax
 	lea    0x1(%rbp),%rsi
 	mov    %rbp,%rdi
 	lea    -0x1(%rax),%rdx
-	call   3b5 <power_fraction+0x2c5>
+	call   405 <power_fraction+0x315>
  R_X86_64_PLT32	memmove-0x4
 	mov    0x48(%rsp),%rax
 	cmpb   $0x2d,(%r12)
 	mov    $0x1,%esi
 	movb   $0x0,-0x1(%rbp,%rax,1)
-	je     440 <power_fraction+0x350>
+	je     490 <power_fraction+0x3a0>
 	mov    %rbx,%rdi
-	call   3d3 <power_fraction+0x2e3>
+	call   423 <power_fraction+0x333>
  R_X86_64_PLT32	calloc-0x4
 	mov    %rbx,%rdx
 	mov    %r12,%rsi
 	mov    %rax,%rdi
 	mov    %rax,0x18(%rsp)
-	call   3e6 <power_fraction+0x2f6>
+	call   436 <power_fraction+0x346>
  R_X86_64_PLT32	memcpy-0x4
 	mov    (%rsp),%rsi
 	mov    %r12,%rdi
-	call   3f2 <power_fraction+0x302>
+	call   442 <power_fraction+0x352>
  R_X86_64_PLT32	realloc-0x4
 	mov    (%rsp),%rdx
 	mov    %r13,%rsi
 	mov    %rax,%rdi
 	mov    %rax,%r12
-	call   404 <power_fraction+0x314>
+	call   454 <power_fraction+0x364>
  R_X86_64_PLT32	memcpy-0x4
 	mov    %rbx,%rsi
 	mov    %r13,%rdi
-	call   40f <power_fraction+0x31f>
+	call   45f <power_fraction+0x36f>
  R_X86_64_PLT32	realloc-0x4
 	mov    0x18(%rsp),%r9
 	mov    %rbx,%rdx
 	mov    %rax,%rdi
 	mov    %rax,%r13
 	mov    %r9,%rsi
 	mov    %r9,(%rsp)
-	call   429 <power_fraction+0x339>
+	call   479 <power_fraction+0x389>
  R_X86_64_PLT32	memcpy-0x4
 	mov    (%rsp),%rdi
-	call   432 <power_fraction+0x342>
+	call   482 <power_fraction+0x392>
  R_X86_64_PLT32	free-0x4
 	jmp    218 <power_fraction+0x128>
 	nopw   0x0(%rax,%rax,1)
 	mov    0x50(%rsp),%rdi
-	call   44a <power_fraction+0x35a>
+	call   49a <power_fraction+0x3aa>
  R_X86_64_PLT32	calloc-0x4
 	lea    0x1(%r12),%rsi
 	mov    %rax,%rdi
 	mov    %rax,0x18(%rsp)
-	call   45c <power_fraction+0x36c>
+	call   4ac <power_fraction+0x3bc>
  R_X86_64_PLT32	stpcpy-0x4
 	mov    0x58(%rsp),%rsi
 	mov    %r12,%rdi
 	mov    %rax,%rbx
 	add    $0x2,%rsi
-	call   470 <power_fraction+0x380>
+	call   4c0 <power_fraction+0x3d0>
  R_X86_64_PLT32	realloc-0x4
 	mov    (%rsp),%rdx
 	mov    %r13,%rsi
 	lea    0x1(%rax),%rdi
 	mov    %rax,%r12
-	call   483 <power_fraction+0x393>
+	call   4d3 <power_fraction+0x3e3>
  R_X86_64_PLT32	memcpy-0x4
 	mov    0x18(%rsp),%r8
 	mov    %r13,%rdi
 	sub    %r8,%rbx
 	mov    %r8,(%rsp)
 	add    $0x1,%rbx
 	mov    %rbx,%rsi
-	call   49e <power_fraction+0x3ae>
+	call   4ee <power_fraction+0x3fe>
  R_X86_64_PLT32	realloc-0x4
 	mov    (%rsp),%rsi
 	mov    %rbx,%rdx
 	mov    %rax,%rdi
 	mov    %rax,%r13
-	call   4b0 <power_fraction+0x3c0>
+	call   500 <power_fraction+0x410>
  R_X86_64_PLT32	memcpy-0x4
 	mov    (%rsp),%rdi
-	call   4b9 <power_fraction+0x3c9>
+	call   509 <power_fraction+0x419>
  R_X86_64_PLT32	free-0x4
 	jmp    218 <power_fraction+0x128>
-	call   4c3 <power_fraction+0x3d3>
+	call   513 <power_fraction+0x423>
  R_X86_64_PLT32	__stack_chk_fail-0x4
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

##### readelf --wide --decompress --hex-dump=.eh_frame {}

```diff
@@ -1,13 +1,13 @@
 
 Hex dump of section '.eh_frame':
  NOTE: This section has relocations against it, but these have NOT been applied to this dump.
   0x00000000 14000000 00000000 017a5200 01781001 .........zR..x..
   0x00000010 1b0c0708 90010000 20000000 1c000000 ........ .......
   0x00000020 00000000 e2000000 00450e10 83020256 .........E.....V
   0x00000030 0a0e0845 0b02650a 0e084b0b 50000000 ...E..e...K.P...
-  0x00000040 40000000 00000000 d3030000 00460e10 @............F..
+  0x00000040 40000000 00000000 23040000 00460e10 @.......#....F..
   0x00000050 8f02450e 188e0345 0e208d04 420e288c ..E....E. ..B.(.
   0x00000060 05410e30 8606440e 38830747 0ec00103 .A.0..D.8..G....
-  0x00000070 87020a0e 38410e30 410e2842 0e20420e ....8A.0A.(B. B.
-  0x00000080 18420e10 420e0841 0b000000 00000000 .B..B..A........
+  0x00000070 a2020a0e 38410e30 410e2842 0e20420e ....8A.0A.(B. B.
+  0x00000080 18420e10 420e0846 0b000000 00000000 .B..B..F........
```

##### readelf --wide --decompress --hex-dump=.strtab {}

```diff
@@ -1,16 +1,17 @@
 
 Hex dump of section '.strtab':
   0x00000000 00706f77 65725f66 72616374 696f6e2e .power_fraction.
-  0x00000010 63006172 6974686d 65746963 615f706f c.arithmetica_po
-  0x00000020 7765725f 66726163 74696f6e 5f726f75 wer_fraction_rou
-  0x00000030 6e645f64 6563696d 616c0073 74726368 nd_decimal.strch
-  0x00000040 7200706f 7765725f 66726163 74696f6e r.power_fraction
-  0x00000050 00737472 6c656e00 63616c6c 6f63006d .strlen.calloc.m
-  0x00000060 656d6370 79006469 76696465 00706f77 emcpy.divide.pow
-  0x00000070 65720073 74726e63 70790070 61727365 er.strncpy.parse
-  0x00000080 5f667261 6374696f 6e006672 65650064 _fraction.free.d
-  0x00000090 656c6574 655f6672 61637469 6f6e006d elete_fraction.m
-  0x000000a0 656d6d6f 76650072 65616c6c 6f630073 emmove.realloc.s
-  0x000000b0 74706370 79005f5f 73746163 6b5f6368 tpcpy.__stack_ch
-  0x000000c0 6b5f6661 696c00                     k_fail.
+  0x00000010 63002e4c 43300061 72697468 6d657469 c..LC0.arithmeti
+  0x00000020 63615f70 6f776572 5f667261 6374696f ca_power_fractio
+  0x00000030 6e5f726f 756e645f 64656369 6d616c00 n_round_decimal.
+  0x00000040 73747263 68720070 6f776572 5f667261 strchr.power_fra
+  0x00000050 6374696f 6e007374 726c656e 0063616c ction.strlen.cal
+  0x00000060 6c6f6300 6d656d63 70790064 69766964 loc.memcpy.divid
+  0x00000070 65007374 72636d70 00737175 6172655f e.strcmp.square_
+  0x00000080 726f6f74 00737472 6e637079 00706172 root.strncpy.par
+  0x00000090 73655f66 72616374 696f6e00 66726565 se_fraction.free
+  0x000000a0 0064656c 6574655f 66726163 74696f6e .delete_fraction
+  0x000000b0 00706f77 6572006d 656d6d6f 76650072 .power.memmove.r
+  0x000000c0 65616c6c 6f630073 74706370 79005f5f ealloc.stpcpy.__
+  0x000000d0 73746163 6b5f6368 6b5f6661 696c00   stack_chk_fail.
```

##### readelf --wide --decompress --hex-dump=.shstrtab {}

```diff
@@ -1,10 +1,11 @@
 
 Hex dump of section '.shstrtab':
   0x00000000 002e7379 6d746162 002e7374 72746162 ..symtab..strtab
   0x00000010 002e7368 73747274 6162002e 72656c61 ..shstrtab..rela
   0x00000020 2e746578 74002e64 61746100 2e627373 .text..data..bss
-  0x00000030 002e636f 6d6d656e 74002e6e 6f74652e ..comment..note.
-  0x00000040 474e552d 73746163 6b002e6e 6f74652e GNU-stack..note.
-  0x00000050 676e752e 70726f70 65727479 002e7265 gnu.property..re
-  0x00000060 6c612e65 685f6672 616d6500          la.eh_frame.
+  0x00000030 002e726f 64617461 2e737472 312e3100 ..rodata.str1.1.
+  0x00000040 2e636f6d 6d656e74 002e6e6f 74652e47 .comment..note.G
+  0x00000050 4e552d73 7461636b 002e6e6f 74652e67 NU-stack..note.g
+  0x00000060 6e752e70 726f7065 72747900 2e72656c nu.property..rel
+  0x00000070 612e6568 5f667261 6d6500            a.eh_frame.
```

#### simplify_parsed_fraction.c.o

##### readelf --wide --sections {}

```diff
@@ -4,16 +4,16 @@
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 0001bd 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 000488 000210 18   I 11   1  8
   [ 3] .data             PROGBITS        0000000000000000 0001fd 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 0001fd 000000 00  WA  0   0  1
   [ 5] .rodata.str1.1    PROGBITS        0000000000000000 0001fd 000004 01 AMS  0   0  1
-  [ 6] .comment          PROGBITS        0000000000000000 000201 00002c 01  MS  0   0  1
-  [ 7] .note.GNU-stack   PROGBITS        0000000000000000 00022d 000000 00      0   0  1
+  [ 6] .comment          PROGBITS        0000000000000000 000201 00002e 01  MS  0   0  1
+  [ 7] .note.GNU-stack   PROGBITS        0000000000000000 00022f 000000 00      0   0  1
   [ 8] .note.gnu.property NOTE            0000000000000000 000230 000020 00   A  0   0  8
   [ 9] .eh_frame         PROGBITS        0000000000000000 000250 000068 00   A  0   0  8
   [10] .rela.eh_frame    RELA            0000000000000000 000698 000018 18   I 11   9  8
   [11] .symtab           SYMTAB          0000000000000000 0002b8 000150 18     12   5  8
   [12] .strtab           STRTAB          0000000000000000 000408 00007e 00      0   0  1
   [13] .shstrtab         STRTAB          0000000000000000 0006b0 00007b 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,10 +1,10 @@
 AWAVAUATUSH
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 simplify_parsed_fraction.c
 simplify_parsed_fraction
 create_fraction
 .shstrtab
 .rela.text
 .rodata.str1.1
 .comment
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### subtract_fraction.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 000132 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 0003a8 0001b0 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 000172 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 000172 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 000172 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 00019e 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 000172 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 0001a0 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 0001a0 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 0001c0 000068 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 000558 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 000228 000108 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 000330 000075 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 000570 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,9 +1,9 @@
 ([]A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 subtract_fraction.c
 subtract_fraction
 multiply
 subtract
 simplify_parsed_fraction
 delete_fraction
 .shstrtab
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### equal_fraction.c.o

##### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              REL (Relocatable file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          0 (bytes into file)
-  Start of section headers:          736 (bytes into file)
+  Start of section headers:          744 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           0 (bytes)
   Number of program headers:         0
   Size of section headers:           64 (bytes)
   Number of section headers:         13
   Section header string table index: 12
```

##### readelf --wide --sections {}

```diff
@@ -1,22 +1,22 @@
-There are 13 section headers, starting at offset 0x2e0:
+There are 13 section headers, starting at offset 0x2e8:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 0000a3 00  AX  0   0 16
-  [ 2] .rela.text        RELA            0000000000000000 000228 000030 18   I 10   1  8
+  [ 2] .rela.text        RELA            0000000000000000 000230 000030 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 0000e3 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 0000e3 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 0000e3 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 00010f 000000 00      0   0  1
-  [ 7] .note.gnu.property NOTE            0000000000000000 000110 000020 00   A  0   0  8
-  [ 8] .eh_frame         PROGBITS        0000000000000000 000130 000058 00   A  0   0  8
-  [ 9] .rela.eh_frame    RELA            0000000000000000 000258 000018 18   I 10   8  8
-  [10] .symtab           SYMTAB          0000000000000000 000188 000078 18     11   3  8
-  [11] .strtab           STRTAB          0000000000000000 000200 000028 00      0   0  1
-  [12] .shstrtab         STRTAB          0000000000000000 000270 00006c 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 0000e3 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000111 000000 00      0   0  1
+  [ 7] .note.gnu.property NOTE            0000000000000000 000118 000020 00   A  0   0  8
+  [ 8] .eh_frame         PROGBITS        0000000000000000 000138 000058 00   A  0   0  8
+  [ 9] .rela.eh_frame    RELA            0000000000000000 000260 000018 18   I 10   8  8
+  [10] .symtab           SYMTAB          0000000000000000 000190 000078 18     11   3  8
+  [11] .strtab           STRTAB          0000000000000000 000208 000028 00      0   0  1
+  [12] .shstrtab         STRTAB          0000000000000000 000278 00006c 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --relocs {}

```diff
@@ -1,9 +1,9 @@
 
-Relocation section '.rela.text' at offset 0x228 contains 2 entries:
+Relocation section '.rela.text' at offset 0x230 contains 2 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000061  0000000400000004 R_X86_64_PLT32         0000000000000000 strcmp - 4
 0000000000000076  0000000400000004 R_X86_64_PLT32         0000000000000000 strcmp - 4
 
-Relocation section '.rela.eh_frame' at offset 0x258 contains 1 entry:
+Relocation section '.rela.eh_frame' at offset 0x260 contains 1 entry:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000020  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 0
```

##### strings --all --bytes=8 {}

```diff
@@ -1,8 +1,8 @@
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 equal_fraction.c
 equal_fraction
 .shstrtab
 .rela.text
 .comment
 .note.GNU-stack
 .note.gnu.property
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### complex_arithmetica.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 000096 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 0002e0 0000c0 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 0000d6 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 0000d6 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 0000d6 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000102 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 0000d6 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000104 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000108 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 000128 000080 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 0003a0 000030 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 0001a8 0000d8 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 000280 00005d 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 0003d0 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,10 +1,10 @@
 AVAUATUH
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 complex_arithmetica.c
 create_complex_number
 delete_complex_number
 .shstrtab
 .rela.text
 .comment
 .note.GNU-stack
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### add_complex.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 000096 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 000260 0000c0 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 0000d6 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 0000d6 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 0000d6 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000102 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 0000d6 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000104 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000108 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 000128 000060 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 000320 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 000188 0000a8 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 000230 00002d 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 000338 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,9 +1,9 @@
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 add_complex.c
 add_complex
 .shstrtab
 .rela.text
 .comment
 .note.GNU-stack
 .note.gnu.property
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### divide_complex.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 00022a 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 0004e0 000330 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 00026a 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 00026a 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 00026a 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000296 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 00026a 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000298 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000298 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 0002b8 000068 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 000810 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 000320 000150 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 000470 000070 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 000828 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,9 +1,9 @@
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 divide_complex.c
 divide_complex
 multiply
 multiply_complex
 .shstrtab
 .rela.text
 .comment
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### exponential_complex.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 0000bd 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 000310 000138 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 0000fd 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 0000fd 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 0000fd 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000129 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 0000fd 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 00012b 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000130 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 000150 000058 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 000448 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 0001a8 000108 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 0002b0 00005a 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 000460 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,8 +1,8 @@
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 exponential_complex.c
 exponential_complex
 exponential
 multiply
 .shstrtab
 .rela.text
 .comment
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### multiply_complex.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 000190 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 0003c8 000240 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 0001d0 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 0001d0 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 0001d0 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 0001fc 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 0001d0 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 0001fe 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000200 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 000220 000068 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 000608 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 000288 0000f0 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 000378 00004e 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 000620 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,10 +1,10 @@
 AVAUATUSH
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 multiply_complex.c
 multiply_complex
 multiply
 subtract
 .shstrtab
 .rela.text
 .comment
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### square_root_complex.c.o

##### readelf --wide --sections {}

```diff
@@ -4,16 +4,16 @@
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 0002f6 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 000688 0004c8 18   I 11   1  8
   [ 3] .data             PROGBITS        0000000000000000 000336 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 000336 000000 00  WA  0   0  1
   [ 5] .rodata.str1.1    PROGBITS        0000000000000000 000336 000002 01 AMS  0   0  1
-  [ 6] .comment          PROGBITS        0000000000000000 000338 00002c 01  MS  0   0  1
-  [ 7] .note.GNU-stack   PROGBITS        0000000000000000 000364 000000 00      0   0  1
+  [ 6] .comment          PROGBITS        0000000000000000 000338 00002e 01  MS  0   0  1
+  [ 7] .note.GNU-stack   PROGBITS        0000000000000000 000366 000000 00      0   0  1
   [ 8] .note.gnu.property NOTE            0000000000000000 000368 000020 00   A  0   0  8
   [ 9] .eh_frame         PROGBITS        0000000000000000 000388 000080 00   A  0   0  8
   [10] .rela.eh_frame    RELA            0000000000000000 000b50 000018 18   I 11   9  8
   [11] .symtab           SYMTAB          0000000000000000 000408 0001c8 18     12   4  8
   [12] .strtab           STRTAB          0000000000000000 0005d0 0000b4 00      0   0  1
   [13] .shstrtab         STRTAB          0000000000000000 000b68 00007b 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,11 +1,11 @@
 AVAUATUH
 []A\A]A^A_
 ([]A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 square_root_complex.c
 square_root_complex
 remove_zeroes
 square_root
 __strcpy_chk
 multiply
 subtract
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### subtract_complex.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 000096 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 000270 0000c0 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 0000d6 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 0000d6 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 0000d6 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000102 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 0000d6 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000104 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000108 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 000128 000060 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 000330 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 000188 0000a8 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 000230 00003c 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 000348 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,9 +1,9 @@
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 subtract_complex.c
 subtract_complex
 subtract
 .shstrtab
 .rela.text
 .comment
 .note.GNU-stack
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### construct_regular_polygon.c.o

##### readelf --wide --sections {}

```diff
@@ -6,16 +6,16 @@
   [ 1] .text             PROGBITS        0000000000000000 000040 000cc1 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 001138 000f18 18   I 13   1  8
   [ 3] .data             PROGBITS        0000000000000000 000d01 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 000d01 000000 00  WA  0   0  1
   [ 5] .rodata.str1.1    PROGBITS        0000000000000000 000d01 000009 01 AMS  0   0  1
   [ 6] .rodata.cst8      PROGBITS        0000000000000000 000d10 000018 08  AM  0   0  8
   [ 7] .rodata.cst16     PROGBITS        0000000000000000 000d30 000010 10  AM  0   0 16
-  [ 8] .comment          PROGBITS        0000000000000000 000d40 00002c 01  MS  0   0  1
-  [ 9] .note.GNU-stack   PROGBITS        0000000000000000 000d6c 000000 00      0   0  1
+  [ 8] .comment          PROGBITS        0000000000000000 000d40 00002e 01  MS  0   0  1
+  [ 9] .note.GNU-stack   PROGBITS        0000000000000000 000d6e 000000 00      0   0  1
   [10] .note.gnu.property NOTE            0000000000000000 000d70 000020 00   A  0   0  8
   [11] .eh_frame         PROGBITS        0000000000000000 000d90 000068 00   A  0   0  8
   [12] .rela.eh_frame    RELA            0000000000000000 002050 000018 18   I 13  11  8
   [13] .symtab           SYMTAB          0000000000000000 000df8 000270 18     14  10  8
   [14] .strtab           STRTAB          0000000000000000 001068 0000c9 00      0   0  1
   [15] .shstrtab         STRTAB          0000000000000000 002068 000096 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,10 +1,10 @@
 AUATUSHc
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 construct_regular_polygon.c
 construct_regular_polygon
 multiply
 subtract
 truncate
 square_root
 .shstrtab
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

### Comparing `arithmetica-py-1.0.224/src/python-module/libbasic_math_operations.a` & `arithmetica-py-1.0.225/src/python-module/libbasic_math_operations.a`

 * *Files 1% similar despite different names*

#### file list

```diff
@@ -2,22 +2,22 @@
 ----------   0        0        0        0 1970-01-01 00:00:00.000000 //
 ?rw-r--r--   0        0        0      952 1970-01-01 00:00:00.000000 basic_math_operations.c.o
 ?rw-r--r--   0        0        0    28944 1970-01-01 00:00:00.000000 basic_math_operations.cpp.o
 ?rw-r--r--   0        0        0      720 1970-01-01 00:00:00.000000 strlen_asm.asm.o
 ?rw-r--r--   0        0        0     1440 1970-01-01 00:00:00.000000 remove_leading_zeroes.asm.o
 ?rw-r--r--   0        0        0     1328 1970-01-01 00:00:00.000000 add_whole.asm.o
 ?rw-r--r--   0        0        0     1216 1970-01-01 00:00:00.000000 add_whole_same_length.asm.o
-?rw-r--r--   0        0        0     1952 1970-01-01 00:00:00.000000 add.c.o
+?rw-r--r--   0        0        0     1960 1970-01-01 00:00:00.000000 add.c.o
 ?rw-r--r--   0        0        0     1632 1970-01-01 00:00:00.000000 subtract_whole.asm.o
 ?rw-r--r--   0        0        0     1568 1970-01-01 00:00:00.000000 subtract_whole_same_length.asm.o
 ?rw-r--r--   0        0        0     2528 1970-01-01 00:00:00.000000 subtractp.c.o
-?rw-r--r--   0        0        0     1960 1970-01-01 00:00:00.000000 subtract.c.o
+?rw-r--r--   0        0        0     1968 1970-01-01 00:00:00.000000 subtract.c.o
 ?rw-r--r--   0        0        0     1488 1970-01-01 00:00:00.000000 _multiply_whole.asm.o
-?rw-r--r--   0        0        0     2552 1970-01-01 00:00:00.000000 multiplyp.c.o
-?rw-r--r--   0        0        0     2032 1970-01-01 00:00:00.000000 multiply.c.o
+?rw-r--r--   0        0        0     2560 1970-01-01 00:00:00.000000 multiplyp.c.o
+?rw-r--r--   0        0        0     2040 1970-01-01 00:00:00.000000 multiply.c.o
 ?rw-r--r--   0        0        0     2880 1970-01-01 00:00:00.000000 _divide_whole_with_remainder.asm.o
 ?rw-r--r--   0        0        0     2120 1970-01-01 00:00:00.000000 divide_whole_with_remainder.c.o
 ?rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 divide_whole.c.o
 ?rw-r--r--   0        0        0     2192 1970-01-01 00:00:00.000000 dividep.c.o
 ?rw-r--r--   0        0        0     2176 1970-01-01 00:00:00.000000 divide.c.o
 ?rw-r--r--   0        0        0     1752 1970-01-01 00:00:00.000000 abs_mod.c.o
 ?rw-r--r--   0        0        0      688 1970-01-01 00:00:00.000000 asmalloc.asm.o
```

#### basic_math_operations.c.o

##### readelf --wide --sections {}

```diff
@@ -2,16 +2,16 @@
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 000000 00  AX  0   0  1
   [ 2] .data             PROGBITS        0000000000000000 000040 000000 00  WA  0   0  1
   [ 3] .bss              NOBITS          0000000000000000 000040 000000 00  WA  0   0  1
-  [ 4] .comment          PROGBITS        0000000000000000 000040 00002c 01  MS  0   0  1
-  [ 5] .note.GNU-stack   PROGBITS        0000000000000000 00006c 000000 00      0   0  1
+  [ 4] .comment          PROGBITS        0000000000000000 000040 00002e 01  MS  0   0  1
+  [ 5] .note.GNU-stack   PROGBITS        0000000000000000 00006e 000000 00      0   0  1
   [ 6] .note.gnu.property NOTE            0000000000000000 000070 000020 00   A  0   0  8
   [ 7] .symtab           SYMTAB          0000000000000000 000090 000030 18      8   2  8
   [ 8] .strtab           STRTAB          0000000000000000 0000c0 000019 00      0   0  1
   [ 9] .shstrtab         STRTAB          0000000000000000 0000d9 000058 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
```

##### strings --all --bytes=8 {}

```diff
@@ -1,6 +1,6 @@
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 basic_math_operations.c
 .shstrtab
 .comment
 .note.GNU-stack
 .note.gnu.property
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### basic_math_operations.cpp.o

##### readelf --wide --sections {}

```diff
@@ -17,16 +17,16 @@
   [12] .rela.text.unlikely RELA            0000000000000000 005ef0 0003f0 18   I 24  11  8
   [13] .gcc_except_table PROGBITS        0000000000000000 002aab 0001c5 00   A  0   0  1
   [14] .text._ZNSt23mersenne_twister_engineImLm32ELm624ELm397ELm31ELm2567483615ELm11ELm4294967295ELm7ELm2636928640ELm15ELm4022730752ELm18ELm1812433253EE11_M_gen_randEv PROGBITS        0000000000000000 002c70 0000f3 00 AXG  0   0 16
   [15] .rodata._ZZNSt8__detail18__to_chars_10_implIjEEvPcjT_E8__digits PROGBITS        0000000000000000 002d80 0000c9 00  AG  0   0 32
   [16] .data._ZN21basic_math_operations17DIVISION_ACCURACYE PROGBITS        0000000000000000 002e50 000008 00 WAG  0   0  8
   [17] .data.rel.local.DW.ref.__gxx_personality_v0 PROGBITS        0000000000000000 002e58 000008 00 WAG  0   0  8
   [18] .rela.data.rel.local.DW.ref.__gxx_personality_v0 RELA            0000000000000000 0062e0 000018 18  IG 24  17  8
-  [19] .comment          PROGBITS        0000000000000000 002e60 00002c 01  MS  0   0  1
-  [20] .note.GNU-stack   PROGBITS        0000000000000000 002e8c 000000 00      0   0  1
+  [19] .comment          PROGBITS        0000000000000000 002e60 00002e 01  MS  0   0  1
+  [20] .note.GNU-stack   PROGBITS        0000000000000000 002e8e 000000 00      0   0  1
   [21] .note.gnu.property NOTE            0000000000000000 002e90 000020 00   A  0   0  8
   [22] .eh_frame         PROGBITS        0000000000000000 002eb0 000770 00   A  0   0  8
   [23] .rela.eh_frame    RELA            0000000000000000 0062f8 000558 18   I 24  22  8
   [24] .symtab           SYMTAB          0000000000000000 003620 000720 18     25  24  8
   [25] .strtab           STRTAB          0000000000000000 003d40 000c4e 00      0   0  1
   [26] .shstrtab         STRTAB          0000000000000000 006850 0001fe 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -21,15 +21,15 @@
 basic_string::_M_construct null not valid
 basic_string::append
 |$`H;<$t
 |$@H;|$(t
 |$`H;<$t
 |$`H;<$t
 00010203040506070809101112131415161718192021222324252627282930313233343536373839404142434445464748495051525354555657585960616263646566676869707172737475767778798081828384858687888990919293949596979899
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 basic_math_operations.cpp
 _ZN21basic_math_operations6BMONumC2Ev.cold
 _ZN21basic_math_operations6BMONumC2ENSt7__cxx1112basic_stringIcSt11char_traitsIcESaIcEEE.cold
 _ZN21basic_math_operations6BMONumC2EPKc.cold
 _ZN21basic_math_operations6BMONumplES0_.cold
 _ZN21basic_math_operations6BMONummiES0_.cold
 _ZN21basic_math_operations6BMONummlES0_.cold
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### add.c.o

##### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              REL (Relocatable file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          0 (bytes into file)
-  Start of section headers:          1120 (bytes into file)
+  Start of section headers:          1128 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           0 (bytes)
   Number of program headers:         0
   Size of section headers:           64 (bytes)
   Number of section headers:         13
   Section header string table index: 12
```

##### readelf --wide --sections {}

```diff
@@ -1,22 +1,22 @@
-There are 13 section headers, starting at offset 0x460:
+There are 13 section headers, starting at offset 0x468:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 00012b 00  AX  0   0 16
-  [ 2] .rela.text        RELA            0000000000000000 000330 0000a8 18   I 10   1  8
+  [ 2] .rela.text        RELA            0000000000000000 000338 0000a8 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 00016b 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 00016b 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 00016b 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000197 000000 00      0   0  1
-  [ 7] .note.gnu.property NOTE            0000000000000000 000198 000020 00   A  0   0  8
-  [ 8] .eh_frame         PROGBITS        0000000000000000 0001b8 000060 00   A  0   0  8
-  [ 9] .rela.eh_frame    RELA            0000000000000000 0003d8 000018 18   I 10   8  8
-  [10] .symtab           SYMTAB          0000000000000000 000218 0000d8 18     11   3  8
-  [11] .strtab           STRTAB          0000000000000000 0002f0 00003b 00      0   0  1
-  [12] .shstrtab         STRTAB          0000000000000000 0003f0 00006c 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 00016b 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000199 000000 00      0   0  1
+  [ 7] .note.gnu.property NOTE            0000000000000000 0001a0 000020 00   A  0   0  8
+  [ 8] .eh_frame         PROGBITS        0000000000000000 0001c0 000060 00   A  0   0  8
+  [ 9] .rela.eh_frame    RELA            0000000000000000 0003e0 000018 18   I 10   8  8
+  [10] .symtab           SYMTAB          0000000000000000 000220 0000d8 18     11   3  8
+  [11] .strtab           STRTAB          0000000000000000 0002f8 00003b 00      0   0  1
+  [12] .shstrtab         STRTAB          0000000000000000 0003f8 00006c 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --relocs {}

```diff
@@ -1,14 +1,14 @@
 
-Relocation section '.rela.text' at offset 0x330 contains 7 entries:
+Relocation section '.rela.text' at offset 0x338 contains 7 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000059  0000000400000004 R_X86_64_PLT32         0000000000000000 addp - 4
 00000000000000b1  0000000400000004 R_X86_64_PLT32         0000000000000000 addp - 4
 00000000000000b9  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
 00000000000000ce  0000000700000004 R_X86_64_PLT32         0000000000000000 memmove - 4
 00000000000000eb  0000000800000004 R_X86_64_PLT32         0000000000000000 subtractp - 4
 0000000000000113  0000000800000004 R_X86_64_PLT32         0000000000000000 subtractp - 4
 0000000000000079  0000000500000004 R_X86_64_PLT32         0000000000000000 remove_zeroes - 4
 
-Relocation section '.rela.eh_frame' at offset 0x3d8 contains 1 entry:
+Relocation section '.rela.eh_frame' at offset 0x3e0 contains 1 entry:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000020  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 0
```

##### strings --all --bytes=8 {}

```diff
@@ -1,8 +1,8 @@
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 remove_zeroes
 strlen_asm
 subtractp
 .shstrtab
 .rela.text
 .comment
 .note.GNU-stack
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### subtractp.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 00028d 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 0004c8 000150 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 0002cd 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 0002cd 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 0002cd 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 0002f9 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 0002cd 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 0002fb 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000300 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 000320 000068 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 000618 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 000388 0000f0 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 000478 00004c 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 000630 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,9 +1,9 @@
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 subtractp.c
 subtractp
 strlen_asm
 subtract_whole
 .shstrtab
 .rela.text
 .comment
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### subtract.c.o

##### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              REL (Relocatable file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          0 (bytes into file)
-  Start of section headers:          1128 (bytes into file)
+  Start of section headers:          1136 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           0 (bytes)
   Number of program headers:         0
   Size of section headers:           64 (bytes)
   Number of section headers:         13
   Section header string table index: 12
```

##### readelf --wide --sections {}

```diff
@@ -1,22 +1,22 @@
-There are 13 section headers, starting at offset 0x468:
+There are 13 section headers, starting at offset 0x470:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 00012b 00  AX  0   0 16
-  [ 2] .rela.text        RELA            0000000000000000 000338 0000a8 18   I 10   1  8
+  [ 2] .rela.text        RELA            0000000000000000 000340 0000a8 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 00016b 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 00016b 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 00016b 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000197 000000 00      0   0  1
-  [ 7] .note.gnu.property NOTE            0000000000000000 000198 000020 00   A  0   0  8
-  [ 8] .eh_frame         PROGBITS        0000000000000000 0001b8 000060 00   A  0   0  8
-  [ 9] .rela.eh_frame    RELA            0000000000000000 0003e0 000018 18   I 10   8  8
-  [10] .symtab           SYMTAB          0000000000000000 000218 0000d8 18     11   3  8
-  [11] .strtab           STRTAB          0000000000000000 0002f0 000045 00      0   0  1
-  [12] .shstrtab         STRTAB          0000000000000000 0003f8 00006c 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 00016b 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000199 000000 00      0   0  1
+  [ 7] .note.gnu.property NOTE            0000000000000000 0001a0 000020 00   A  0   0  8
+  [ 8] .eh_frame         PROGBITS        0000000000000000 0001c0 000060 00   A  0   0  8
+  [ 9] .rela.eh_frame    RELA            0000000000000000 0003e8 000018 18   I 10   8  8
+  [10] .symtab           SYMTAB          0000000000000000 000220 0000d8 18     11   3  8
+  [11] .strtab           STRTAB          0000000000000000 0002f8 000045 00      0   0  1
+  [12] .shstrtab         STRTAB          0000000000000000 000400 00006c 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --relocs {}

```diff
@@ -1,14 +1,14 @@
 
-Relocation section '.rela.text' at offset 0x338 contains 7 entries:
+Relocation section '.rela.text' at offset 0x340 contains 7 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000059  0000000400000004 R_X86_64_PLT32         0000000000000000 subtractp - 4
 00000000000000b1  0000000400000004 R_X86_64_PLT32         0000000000000000 subtractp - 4
 00000000000000cb  0000000600000004 R_X86_64_PLT32         0000000000000000 addp - 4
 00000000000000d3  0000000700000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
 00000000000000e8  0000000800000004 R_X86_64_PLT32         0000000000000000 memmove - 4
 0000000000000113  0000000600000004 R_X86_64_PLT32         0000000000000000 addp - 4
 0000000000000079  0000000500000004 R_X86_64_PLT32         0000000000000000 remove_zeroes - 4
 
-Relocation section '.rela.eh_frame' at offset 0x3e0 contains 1 entry:
+Relocation section '.rela.eh_frame' at offset 0x3e8 contains 1 entry:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000020  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 0
```

##### strings --all --bytes=8 {}

```diff
@@ -1,8 +1,8 @@
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 subtract.c
 subtract
 subtractp
 remove_zeroes
 strlen_asm
 .shstrtab
 .rela.text
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### multiplyp.c.o

##### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              REL (Relocatable file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          0 (bytes into file)
-  Start of section headers:          1720 (bytes into file)
+  Start of section headers:          1728 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           0 (bytes)
   Number of program headers:         0
   Size of section headers:           64 (bytes)
   Number of section headers:         13
   Section header string table index: 12
```

##### readelf --wide --sections {}

```diff
@@ -1,22 +1,22 @@
-There are 13 section headers, starting at offset 0x6b8:
+There are 13 section headers, starting at offset 0x6c0:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 000224 00  AX  0   0 16
-  [ 2] .rela.text        RELA            0000000000000000 000438 0001f8 18   I 10   1  8
+  [ 2] .rela.text        RELA            0000000000000000 000440 0001f8 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 000264 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 000264 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 000264 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000290 000000 00      0   0  1
-  [ 7] .note.gnu.property NOTE            0000000000000000 000290 000020 00   A  0   0  8
-  [ 8] .eh_frame         PROGBITS        0000000000000000 0002b0 000068 00   A  0   0  8
-  [ 9] .rela.eh_frame    RELA            0000000000000000 000630 000018 18   I 10   8  8
-  [10] .symtab           SYMTAB          0000000000000000 000318 0000d8 18     11   3  8
-  [11] .strtab           STRTAB          0000000000000000 0003f0 000046 00      0   0  1
-  [12] .shstrtab         STRTAB          0000000000000000 000648 00006c 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 000264 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000292 000000 00      0   0  1
+  [ 7] .note.gnu.property NOTE            0000000000000000 000298 000020 00   A  0   0  8
+  [ 8] .eh_frame         PROGBITS        0000000000000000 0002b8 000068 00   A  0   0  8
+  [ 9] .rela.eh_frame    RELA            0000000000000000 000638 000018 18   I 10   8  8
+  [10] .symtab           SYMTAB          0000000000000000 000320 0000d8 18     11   3  8
+  [11] .strtab           STRTAB          0000000000000000 0003f8 000046 00      0   0  1
+  [12] .shstrtab         STRTAB          0000000000000000 000650 00006c 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --relocs {}

```diff
@@ -1,9 +1,9 @@
 
-Relocation section '.rela.text' at offset 0x438 contains 21 entries:
+Relocation section '.rela.text' at offset 0x440 contains 21 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 000000000000001c  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
 0000000000000029  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
 0000000000000040  0000000500000004 R_X86_64_PLT32         0000000000000000 calloc - 4
 0000000000000055  0000000500000004 R_X86_64_PLT32         0000000000000000 calloc - 4
 0000000000000111  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
 000000000000011c  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
@@ -19,10 +19,10 @@
 00000000000001da  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
 00000000000001ec  0000000500000004 R_X86_64_PLT32         0000000000000000 calloc - 4
 00000000000001fc  0000000500000004 R_X86_64_PLT32         0000000000000000 calloc - 4
 0000000000000213  0000000600000004 R_X86_64_PLT32         0000000000000000 _multiply_whole - 4
 000000000000021b  0000000400000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
 00000000000001b4  0000000800000004 R_X86_64_PLT32         0000000000000000 free - 4
 
-Relocation section '.rela.eh_frame' at offset 0x630 contains 1 entry:
+Relocation section '.rela.eh_frame' at offset 0x638 contains 1 entry:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000020  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 0
```

##### strings --all --bytes=8 {}

```diff
@@ -1,9 +1,9 @@
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 multiplyp.c
 multiplyp
 strlen_asm
 _multiply_whole
 .shstrtab
 .rela.text
 .comment
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### multiply.c.o

##### readelf --wide --file-header {}

```diff
@@ -6,15 +6,15 @@
   OS/ABI:                            UNIX - System V
   ABI Version:                       0
   Type:                              REL (Relocatable file)
   Machine:                           Advanced Micro Devices X86-64
   Version:                           0x1
   Entry point address:               0x0
   Start of program headers:          0 (bytes into file)
-  Start of section headers:          1200 (bytes into file)
+  Start of section headers:          1208 (bytes into file)
   Flags:                             0x0
   Size of this header:               64 (bytes)
   Size of program headers:           0 (bytes)
   Number of program headers:         0
   Size of section headers:           64 (bytes)
   Number of section headers:         13
   Section header string table index: 12
```

##### readelf --wide --sections {}

```diff
@@ -1,22 +1,22 @@
-There are 13 section headers, starting at offset 0x4b0:
+There are 13 section headers, starting at offset 0x4b8:
 
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 000153 00  AX  0   0 16
-  [ 2] .rela.text        RELA            0000000000000000 000350 0000d8 18   I 10   1  8
+  [ 2] .rela.text        RELA            0000000000000000 000358 0000d8 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 000193 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 000193 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 000193 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 0001bf 000000 00      0   0  1
-  [ 7] .note.gnu.property NOTE            0000000000000000 0001c0 000020 00   A  0   0  8
-  [ 8] .eh_frame         PROGBITS        0000000000000000 0001e0 000070 00   A  0   0  8
-  [ 9] .rela.eh_frame    RELA            0000000000000000 000428 000018 18   I 10   8  8
-  [10] .symtab           SYMTAB          0000000000000000 000250 0000c0 18     11   3  8
-  [11] .strtab           STRTAB          0000000000000000 000310 000040 00      0   0  1
-  [12] .shstrtab         STRTAB          0000000000000000 000440 00006c 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 000193 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 0001c1 000000 00      0   0  1
+  [ 7] .note.gnu.property NOTE            0000000000000000 0001c8 000020 00   A  0   0  8
+  [ 8] .eh_frame         PROGBITS        0000000000000000 0001e8 000070 00   A  0   0  8
+  [ 9] .rela.eh_frame    RELA            0000000000000000 000430 000018 18   I 10   8  8
+  [10] .symtab           SYMTAB          0000000000000000 000258 0000c0 18     11   3  8
+  [11] .strtab           STRTAB          0000000000000000 000318 000040 00      0   0  1
+  [12] .shstrtab         STRTAB          0000000000000000 000448 00006c 00      0   0  1
 Key to Flags:
   W (write), A (alloc), X (execute), M (merge), S (strings), I (info),
   L (link order), O (extra OS processing required), G (group), T (TLS),
   C (compressed), x (unknown), o (OS specific), E (exclude),
   D (mbind), l (large), p (processor specific)
```

##### readelf --wide --relocs {}

```diff
@@ -1,16 +1,16 @@
 
-Relocation section '.rela.text' at offset 0x350 contains 9 entries:
+Relocation section '.rela.text' at offset 0x358 contains 9 entries:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000068  0000000400000004 R_X86_64_PLT32         0000000000000000 multiplyp - 4
 00000000000000c3  0000000400000004 R_X86_64_PLT32         0000000000000000 multiplyp - 4
 00000000000000cb  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
 00000000000000e0  0000000700000004 R_X86_64_PLT32         0000000000000000 memmove - 4
 0000000000000103  0000000400000004 R_X86_64_PLT32         0000000000000000 multiplyp - 4
 000000000000010b  0000000600000004 R_X86_64_PLT32         0000000000000000 strlen_asm - 4
 0000000000000120  0000000700000004 R_X86_64_PLT32         0000000000000000 memmove - 4
 000000000000013b  0000000400000004 R_X86_64_PLT32         0000000000000000 multiplyp - 4
 000000000000008a  0000000500000004 R_X86_64_PLT32         0000000000000000 remove_zeroes - 4
 
-Relocation section '.rela.eh_frame' at offset 0x428 contains 1 entry:
+Relocation section '.rela.eh_frame' at offset 0x430 contains 1 entry:
     Offset             Info             Type               Symbol's Value  Symbol's Name + Addend
 0000000000000020  0000000200000002 R_X86_64_PC32          0000000000000000 .text + 0
```

##### strings --all --bytes=8 {}

```diff
@@ -1,8 +1,8 @@
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 multiply.c
 multiply
 multiplyp
 remove_zeroes
 strlen_asm
 .shstrtab
 .rela.text
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### divide_whole_with_remainder.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 000149 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 0003a8 0000d8 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 000189 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 000189 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 000189 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 0001b5 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 000189 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 0001b7 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 0001b8 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 0001d8 000080 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 000480 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 000258 0000d8 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 000330 000071 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 000498 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,10 +1,10 @@
 []A\A]A^A_
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 divide_whole_with_remainder.c
 strlen_asm
 _divide_whole_with_remainder
 remove_leading_zeroes_inplace
 .shstrtab
 .rela.text
 .comment
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### divide_whole.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 000109 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 000370 000108 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 000149 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 000149 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 000149 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000175 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 000149 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000177 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000178 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 000198 000068 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 000478 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 000200 000108 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 000308 000067 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 000490 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,9 +1,9 @@
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 divide_whole.c
 divide_whole
 strlen_asm
 _divide_whole_with_remainder
 .shstrtab
 .rela.text
 .comment
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### dividep.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 0001e1 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 0003f0 0000d8 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 000221 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 000221 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 000221 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 00024d 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 000221 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 00024f 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000250 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 000270 000068 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 0004c8 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 0002d8 0000d8 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 0003b0 00003e 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 0004e0 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,9 +1,9 @@
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 dividep.c
 strlen_asm
 divide_whole
 .shstrtab
 .rela.text
 .comment
 .note.GNU-stack
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### divide.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 0001d0 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 0003e0 0000d8 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 000210 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 000210 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 000210 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 00023c 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 000210 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 00023e 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000240 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 000260 000080 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 0004b8 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 0002e0 0000c0 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 0003a0 00003a 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 0004d0 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,8 +1,8 @@
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 divide.c
 strlen_asm
 remove_zeroes
 .shstrtab
 .rela.text
 .comment
 .note.GNU-stack
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### abs_mod.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 000090 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 000280 000090 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 0000d0 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 0000d0 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 0000d0 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 0000fc 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 0000d0 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 0000fe 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000100 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 000120 000058 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 000310 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 000178 0000c0 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 000238 000042 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 000328 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,8 +1,8 @@
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 abs_mod.c
 divide_whole_with_remainder
 .shstrtab
 .rela.text
 .comment
 .note.GNU-stack
 .note.gnu.property
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### addp.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 00028d 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 0004b8 000150 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 0002cd 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 0002cd 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 0002cd 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 0002f9 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 0002cd 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 0002fb 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000300 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 000320 000068 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 000608 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 000388 0000f0 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 000478 00003d 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 000620 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,9 +1,9 @@
 []A\A]A^A_
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 strlen_asm
 add_whole
 .shstrtab
 .rela.text
 .comment
 .note.GNU-stack
 .note.gnu.property
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### remove_zeroes.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 00012d 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 0002f8 000060 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 00016d 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 00016d 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 00016d 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000199 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 00016d 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 00019b 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 0001a0 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 0001c0 000058 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 000358 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 000218 0000a8 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 0002c0 000036 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 000370 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,8 +1,8 @@
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 remove_zeroes.c
 remove_zeroes
 strlen_asm
 .shstrtab
 .rela.text
 .comment
 .note.GNU-stack
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

#### increment_whole.c.o

##### readelf --wide --sections {}

```diff
@@ -3,16 +3,16 @@
 Section Headers:
   [Nr] Name              Type            Address          Off    Size   ES Flg Lk Inf Al
   [ 0]                   NULL            0000000000000000 000000 000000 00      0   0  0
   [ 1] .text             PROGBITS        0000000000000000 000040 000107 00  AX  0   0 16
   [ 2] .rela.text        RELA            0000000000000000 000308 000090 18   I 10   1  8
   [ 3] .data             PROGBITS        0000000000000000 000147 000000 00  WA  0   0  1
   [ 4] .bss              NOBITS          0000000000000000 000147 000000 00  WA  0   0  1
-  [ 5] .comment          PROGBITS        0000000000000000 000147 00002c 01  MS  0   0  1
-  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000173 000000 00      0   0  1
+  [ 5] .comment          PROGBITS        0000000000000000 000147 00002e 01  MS  0   0  1
+  [ 6] .note.GNU-stack   PROGBITS        0000000000000000 000175 000000 00      0   0  1
   [ 7] .note.gnu.property NOTE            0000000000000000 000178 000020 00   A  0   0  8
   [ 8] .eh_frame         PROGBITS        0000000000000000 000198 000068 00   A  0   0  8
   [ 9] .rela.eh_frame    RELA            0000000000000000 000398 000018 18   I 10   8  8
   [10] .symtab           SYMTAB          0000000000000000 000200 0000c0 18     11   3  8
   [11] .strtab           STRTAB          0000000000000000 0002c0 000041 00      0   0  1
   [12] .shstrtab         STRTAB          0000000000000000 0003b0 00006c 00      0   0  1
 Key to Flags:
```

##### strings --all --bytes=8 {}

```diff
@@ -1,8 +1,8 @@
-GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
 increment_whole.c
 increment_whole
 strlen_asm
 .shstrtab
 .rela.text
 .comment
 .note.GNU-stack
```

##### readelf --wide --decompress --string-dump=.comment {}

```diff
@@ -1,4 +1,4 @@
 
 String dump of section '.comment':
-  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04) 11.3.0
+  [     1]  GCC: (Ubuntu 11.3.0-1ubuntu1~22.04.1) 11.3.0
```

### Comparing `arithmetica-py-1.0.224/src/python-module/module.c` & `arithmetica-py-1.0.225/src/python-module/module.c`

 * *Files identical despite different names*

