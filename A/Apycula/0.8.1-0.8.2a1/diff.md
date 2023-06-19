# Comparing `tmp/Apycula-0.8.1.tar.gz` & `tmp/Apycula-0.8.2a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Apycula-0.8.1.tar", last modified: Mon May 29 07:47:20 2023, max compression
+gzip compressed data, was "Apycula-0.8.2a1.tar", last modified: Mon Jun 19 13:12:22 2023, max compression
```

## Comparing `Apycula-0.8.1.tar` & `Apycula-0.8.2a1.tar`

### file list

```diff
@@ -1,286 +1,289 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.254105 Apycula-0.8.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.118097 Apycula-0.8.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.122098 Apycula-0.8.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     8314 2023-05-29 07:46:49.000000 Apycula-0.8.1/.github/workflows/chipdb.yml
--rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-29 07:46:49.000000 Apycula-0.8.1/.github/workflows/yowasp_examples.yml
--rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-29 07:46:49.000000 Apycula-0.8.1/.gitignore
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.122098 Apycula-0.8.1/Apycula.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-05-29 07:47:19.000000 Apycula-0.8.1/Apycula.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6889 2023-05-29 07:47:20.000000 Apycula-0.8.1/Apycula.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-29 07:47:19.000000 Apycula-0.8.1/Apycula.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-29 07:47:19.000000 Apycula-0.8.1/Apycula.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-29 07:47:19.000000 Apycula-0.8.1/Apycula.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-29 07:47:19.000000 Apycula-0.8.1/Apycula.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-29 07:46:49.000000 Apycula-0.8.1/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-29 07:46:49.000000 Apycula-0.8.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-05-29 07:46:49.000000 Apycula-0.8.1/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)    10641 2023-05-29 07:47:20.254105 Apycula-0.8.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.222103 Apycula-0.8.1/apycula/
--rw-r--r--   0 runner    (1001) docker     (123)  5875340 2023-05-29 07:46:50.000000 Apycula-0.8.1/apycula/GW1N-1.pickle
--rw-r--r--   0 runner    (1001) docker     (123) 13631415 2023-05-29 07:46:53.000000 Apycula-0.8.1/apycula/GW1N-4.pickle
--rw-r--r--   0 runner    (1001) docker     (123) 21788633 2023-05-29 07:46:54.000000 Apycula-0.8.1/apycula/GW1N-9.pickle
--rw-r--r--   0 runner    (1001) docker     (123) 21813161 2023-05-29 07:46:55.000000 Apycula-0.8.1/apycula/GW1N-9C.pickle
--rw-r--r--   0 runner    (1001) docker     (123)  7230327 2023-05-29 07:46:56.000000 Apycula-0.8.1/apycula/GW1NS-2.pickle
--rw-r--r--   0 runner    (1001) docker     (123) 13196089 2023-05-29 07:46:57.000000 Apycula-0.8.1/apycula/GW1NS-4.pickle
--rw-r--r--   0 runner    (1001) docker     (123)  5560266 2023-05-29 07:46:51.000000 Apycula-0.8.1/apycula/GW1NZ-1.pickle
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-29 07:46:49.000000 Apycula-0.8.1/apycula/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26023 2023-05-29 07:46:49.000000 Apycula-0.8.1/apycula/attrids.py
--rw-r--r--   0 runner    (1001) docker     (123)     4641 2023-05-29 07:46:49.000000 Apycula-0.8.1/apycula/bslib.py
--rw-r--r--   0 runner    (1001) docker     (123)    51888 2023-05-29 07:46:49.000000 Apycula-0.8.1/apycula/chipdb.py
--rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-05-29 07:46:49.000000 Apycula-0.8.1/apycula/clock_fuzzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4400 2023-05-29 07:46:49.000000 Apycula-0.8.1/apycula/codegen.py
--rw-r--r--   0 runner    (1001) docker     (123)    14047 2023-05-29 07:46:49.000000 Apycula-0.8.1/apycula/dat19_h4x.py
--rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-05-29 07:46:49.000000 Apycula-0.8.1/apycula/fuse_h4x.py
--rw-r--r--   0 runner    (1001) docker     (123)     8389 2023-05-29 07:46:49.000000 Apycula-0.8.1/apycula/gowin_bba.py
--rw-r--r--   0 runner    (1001) docker     (123)    43007 2023-05-29 07:46:49.000000 Apycula-0.8.1/apycula/gowin_pack.py
--rw-r--r--   0 runner    (1001) docker     (123)    45669 2023-05-29 07:46:49.000000 Apycula-0.8.1/apycula/gowin_unpack.py
--rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-05-29 07:46:49.000000 Apycula-0.8.1/apycula/pindef.py
--rw-r--r--   0 runner    (1001) docker     (123)    10062 2023-05-29 07:46:49.000000 Apycula-0.8.1/apycula/tiled_fuzzer.py
--rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-05-29 07:46:49.000000 Apycula-0.8.1/apycula/tm_h4x.py
--rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-05-29 07:46:49.000000 Apycula-0.8.1/apycula/wirenames.py
--rw-r--r--   0 runner    (1001) docker     (123)    84965 2023-05-29 07:46:49.000000 Apycula-0.8.1/clock_experiments.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.226103 Apycula-0.8.1/doc/
--rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-05-29 07:46:49.000000 Apycula-0.8.1/doc/alu.md
--rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-05-29 07:46:49.000000 Apycula-0.8.1/doc/architecture.md
--rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-05-29 07:46:49.000000 Apycula-0.8.1/doc/commandstructure.md
--rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-05-29 07:46:49.000000 Apycula-0.8.1/doc/compression.md
--rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-05-29 07:46:49.000000 Apycula-0.8.1/doc/device_grouping.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.230104 Apycula-0.8.1/doc/fig/
--rw-r--r--   0 runner    (1001) docker     (123)    17770 2023-05-29 07:46:49.000000 Apycula-0.8.1/doc/fig/alu_logic.png
--rw-r--r--   0 runner    (1001) docker     (123)    64550 2023-05-29 07:46:49.000000 Apycula-0.8.1/doc/fig/alu_tile.png
--rw-r--r--   0 runner    (1001) docker     (123)   285739 2023-05-29 07:46:49.000000 Apycula-0.8.1/doc/fig/blinky.jpg
--rw-r--r--   0 runner    (1001) docker     (123)    17036 2023-05-29 07:46:49.000000 Apycula-0.8.1/doc/fig/clocks.png
--rw-r--r--   0 runner    (1001) docker     (123)    31670 2023-05-29 07:46:49.000000 Apycula-0.8.1/doc/fig/clu.png
--rw-r--r--   0 runner    (1001) docker     (123)    50702 2023-05-29 07:46:49.000000 Apycula-0.8.1/doc/fig/floorplanner.png
--rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-05-29 07:46:49.000000 Apycula-0.8.1/doc/fig/fuse.png
--rw-r--r--   0 runner    (1001) docker     (123)   462042 2023-05-29 07:46:49.000000 Apycula-0.8.1/doc/fig/lw.png
--rw-r--r--   0 runner    (1001) docker     (123)  1358038 2023-05-29 07:46:49.000000 Apycula-0.8.1/doc/fig/lw.svg
--rw-r--r--   0 runner    (1001) docker     (123)    20031 2023-05-29 07:46:49.000000 Apycula-0.8.1/doc/fig/mux.png
--rw-r--r--   0 runner    (1001) docker     (123)    49730 2023-05-29 07:46:49.000000 Apycula-0.8.1/doc/fig/muxes-wiring.png
--rw-r--r--   0 runner    (1001) docker     (123)   102610 2023-05-29 07:46:49.000000 Apycula-0.8.1/doc/fig/post_pnr.png
--rw-r--r--   0 runner    (1001) docker     (123)    53504 2023-05-29 07:46:49.000000 Apycula-0.8.1/doc/fig/post_syn.png
--rw-r--r--   0 runner    (1001) docker     (123)    37892 2023-05-29 07:46:49.000000 Apycula-0.8.1/doc/fig/tile.png
--rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-05-29 07:46:49.000000 Apycula-0.8.1/doc/filestructure.md
--rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-05-29 07:46:49.000000 Apycula-0.8.1/doc/longval-tables.md
--rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-05-29 07:46:49.000000 Apycula-0.8.1/doc/longwires.md
--rw-r--r--   0 runner    (1001) docker     (123)      591 2023-05-29 07:46:49.000000 Apycula-0.8.1/doc/muxes.md
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-29 07:46:49.000000 Apycula-0.8.1/doc/sdram.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.230104 Apycula-0.8.1/examples/
--rw-r--r--   0 runner    (1001) docker     (123)    11557 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.234104 Apycula-0.8.1/examples/attosoc/
--rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/attosoc/attosoc.v
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/attosoc/firmware.hex
--rw-r--r--   0 runner    (1001) docker     (123)    94292 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/attosoc/picorv32.v
--rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/blinky-oddr.v
--rw-r--r--   0 runner    (1001) docker     (123)      598 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/blinky-osc.v
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/blinky-tbuf.v
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/blinky.v
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.242104 Apycula-0.8.1/examples/deser/
--rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/iddr-szfpga.cst
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/iddr-tangnano.cst
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/iddr-tangnano1k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/iddr-tangnano4k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/iddr-tangnano9k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/iddr.v
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/iddrc-szfpga.cst
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/iddrc-tangnano.cst
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/iddrc-tangnano1k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/iddrc-tangnano4k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/iddrc-tangnano9k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/iddrc.v
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ides10-szfpga.cst
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ides10-tangnano.cst
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ides10-tangnano1k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ides10-tangnano4k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ides10-tangnano9k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      902 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ides10.v
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ides16-szfpga.cst
--rw-r--r--   0 runner    (1001) docker     (123)      350 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ides16-tangnano4k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ides16-tangnano9k.cst
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ides16.v
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ides4-szfpga.cst
--rw-r--r--   0 runner    (1001) docker     (123)      831 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ides4-tangnano.cst
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ides4-tangnano1k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ides4-tangnano4k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ides4-tangnano9k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ides4.v
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ides8-szfpga.cst
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ides8-tangnano.cst
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ides8-tangnano1k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ides8-tangnano4k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ides8-tangnano9k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      706 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ides8.v
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ivideo-szfpga.cst
--rw-r--r--   0 runner    (1001) docker     (123)      993 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ivideo-tangnano.cst
--rw-r--r--   0 runner    (1001) docker     (123)      937 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ivideo-tangnano1k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ivideo-tangnano4k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      936 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ivideo-tangnano9k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ivideo.v
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser10-szfpga.cst
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser10-tangnano.cst
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser10-tangnano4k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser10-tangnano9k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser10-tec0117.cst
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser10-tlvds-tangnano4k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser10-tlvds-tangnano9k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser10-tlvds-tec0117.cst
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser10-tlvds.v
--rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser10.v
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser16-szfpga.cst
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser16-tangnano4k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser16-tangnano9k.cst
--rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser16.v
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser4-szfpga.cst
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser4-tangnano.cst
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser4-tangnano4k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser4-tangnano9k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser4-tec0117.cst
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser4-tlvds-tangnano4k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser4-tlvds-tangnano9k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser4-tlvds-tec0117.cst
--rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser4-tlvds.v
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser4.v
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser8-szfpga.cst
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser8-tangnano.cst
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser8-tangnano4k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser8-tangnano9k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser8-tec0117.cst
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser8-tlvds-tangnano4k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser8-tlvds-tangnano9k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser8-tlvds-tec0117.cst
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser8-tlvds.v
--rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/oser8.v
--rw-r--r--   0 runner    (1001) docker     (123)      592 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ovideo-szfpga.cst
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ovideo-tangnano.cst
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ovideo-tangnano4k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ovideo-tangnano9k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ovideo-tec0117.cst
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ovideo-tlvds-tangnano4k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ovideo-tlvds-tangnano9k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ovideo-tlvds-tec0117.cst
--rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ovideo-tlvds.v
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/deser/ovideo.v
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/elvds.v
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/honeycomb.cst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.242104 Apycula-0.8.1/examples/longwires/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/longwires/honeycomb.cst
--rw-r--r--   0 runner    (1001) docker     (123)      394 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/longwires/runber.cst
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/longwires/tangnano.cst
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/longwires/tangnano1k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/longwires/tangnano4k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      399 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/longwires/tangnano9k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/longwires/tec0117.cst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.242104 Apycula-0.8.1/examples/lutram/
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/lutram/README.md
--rwxr-xr-x   0 runner    (1001) docker     (123)      300 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/lutram/build.sh
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/lutram/lutram.v
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/lutram/prbs.v
--rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/lutram/top.v
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/lvds-szfpga.cst
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/lvds-tangnano.cst
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/lvds-tangnano1k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/lvds-tangnano4k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/lvds-tangnano9k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/lvds-tec0117.cst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.242104 Apycula-0.8.1/examples/nanolcd/
--rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/nanolcd/TOP.v
--rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/nanolcd/VGAMod.v
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/oddr-elvds.v
--rw-r--r--   0 runner    (1001) docker     (123)      787 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/oddr-tlvds.v
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.246105 Apycula-0.8.1/examples/pll/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/pll/GW1N-1-52.vh
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/pll/GW1N-1-80.vh
--rw-r--r--   0 runner    (1001) docker     (123)      254 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/pll/GW1N-1-dyn.vh
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/pll/GW1N-4-dyn.vh
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/pll/GW1N-9-dyn.vh
--rw-r--r--   0 runner    (1001) docker     (123)      461 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/pll/GW1N-9C-dyn.vh
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/pll/GW1NS-2C-dyn.vh
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/pll/GW1NZ-1-54.vh
--rw-r--r--   0 runner    (1001) docker     (123)      127 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/pll/GW1NZ-1-81.vh
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/pll/GW1NZ-1-dyn.vh
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/pll/pllvr.v
--rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/pll/rpll.v
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.246105 Apycula-0.8.1/examples/pll-nanolcd/
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/pll-nanolcd/TOP.v
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/pll-nanolcd/VGAMod.v
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/pll-tangnano4k.v
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/pll.v
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/pll2.v
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/runber-tlvds.cst
--rw-r--r--   0 runner    (1001) docker     (123)      357 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/runber.cst
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/shift.v
--rw-r--r--   0 runner    (1001) docker     (123)      584 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/tangnano.cst
--rw-r--r--   0 runner    (1001) docker     (123)      403 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/tangnano1k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      243 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/tangnano4k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/tangnano9k.cst
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/tec0117.cst
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/tlvds.v
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.246105 Apycula-0.8.1/examples/tonegen/
--rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/tonegen/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/tonegen/cordic.v
--rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/tonegen/sddac.v
--rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-05-29 07:46:49.000000 Apycula-0.8.1/examples/tonegen/top.v
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.246105 Apycula-0.8.1/legacy/
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.246105 Apycula-0.8.1/legacy/empty/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/empty/device.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/empty/empty.v
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/empty/pnr.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/empty/run.tcl
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.246105 Apycula-0.8.1/legacy/example/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/example/example.cst
--rw-r--r--   0 runner    (1001) docker     (123)      206 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/example/example.v
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/example/pnr.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/example/run.tcl
--rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/fuzzer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.246105 Apycula-0.8.1/legacy/generic/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.250105 Apycula-0.8.1/legacy/generic/attosoc/
--rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/generic/attosoc/attosoc.v
--rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/generic/attosoc/firmware.hex
--rw-r--r--   0 runner    (1001) docker     (123)    94292 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/generic/attosoc/picorv32.v
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/generic/attosoc/top.v
--rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/generic/bitstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/generic/blinky.v
--rw-r--r--   0 runner    (1001) docker     (123)      549 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/generic/blinkygw1n1.v
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.250105 Apycula-0.8.1/legacy/generic/nanolcd/
--rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/generic/nanolcd/TOP.v
--rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/generic/nanolcd/VGAMod.v
--rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/generic/simple.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      339 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/generic/simple.sh
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/generic/simple_timing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.250105 Apycula-0.8.1/legacy/generic/synth/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/generic/synth/cells_map.v
--rw-r--r--   0 runner    (1001) docker     (123)      920 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/generic/synth/prims.v
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/generic/synth/synth_generic.tcl
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/generic/write_fasm.py
--rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/indices.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.250105 Apycula-0.8.1/legacy/iob/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/iob/device.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/iob/iob.cst.mk
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/iob/iob.sdc
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/iob/iob.v
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/iob/pnr.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/iob/run.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/iob.sh
--rw-r--r--   0 runner    (1001) docker     (123)      528 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/json_display.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.250105 Apycula-0.8.1/legacy/lut4/
--rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/lut4/device.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/lut4/lut4.cst.mk
--rw-r--r--   0 runner    (1001) docker     (123)      256 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/lut4/lut4.sdc
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/lut4/lut4.v
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/lut4/pnr.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/lut4/run.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/lut4.sh
--rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/report.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-29 07:47:20.250105 Apycula-0.8.1/legacy/sdram/
--rwxr-xr-x   0 runner    (1001) docker     (123)     2251 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/sdram/find_sdram_pins.py
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/sdram/findpin.tcl
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/sdram/findpin.vhd
--rwxr-xr-x   0 runner    (1001) docker     (123)       71 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/sdram/run.sh
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/sdram/template.vhd
--rw-r--r--   0 runner    (1001) docker     (123)   813455 2023-05-29 07:46:49.000000 Apycula-0.8.1/legacy/sdram/unpack.v
--rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-05-29 07:46:49.000000 Apycula-0.8.1/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-29 07:47:20.254105 Apycula-0.8.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-05-29 07:46:49.000000 Apycula-0.8.1/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-05-29 07:46:49.000000 Apycula-0.8.1/test_clk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.074183 Apycula-0.8.2a1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.010182 Apycula-0.8.2a1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.014183 Apycula-0.8.2a1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     9035 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/.github/workflows/chipdb.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/.github/workflows/yowasp_examples.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.014183 Apycula-0.8.2a1/Apycula.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-06-19 13:12:21.000000 Apycula-0.8.2a1/Apycula.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6948 2023-06-19 13:12:21.000000 Apycula-0.8.2a1/Apycula.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-06-19 13:12:21.000000 Apycula-0.8.2a1/Apycula.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-06-19 13:12:21.000000 Apycula-0.8.2a1/Apycula.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-06-19 13:12:21.000000 Apycula-0.8.2a1/Apycula.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-06-19 13:12:21.000000 Apycula-0.8.2a1/Apycula.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      662 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)    10643 2023-06-19 13:12:22.074183 Apycula-0.8.2a1/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.030183 Apycula-0.8.2a1/apycula/
+-rw-r--r--   0 runner    (1001) docker     (123)   596845 2023-06-19 13:12:00.000000 Apycula-0.8.2a1/apycula/GW1N-1.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)   897220 2023-06-19 13:12:01.000000 Apycula-0.8.2a1/apycula/GW1N-4.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)  1111202 2023-06-19 13:12:02.000000 Apycula-0.8.2a1/apycula/GW1N-9.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)  1114504 2023-06-19 13:12:02.000000 Apycula-0.8.2a1/apycula/GW1N-9C.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)   690272 2023-06-19 13:12:03.000000 Apycula-0.8.2a1/apycula/GW1NS-2.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)   865769 2023-06-19 13:12:04.000000 Apycula-0.8.2a1/apycula/GW1NS-4.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)   603589 2023-06-19 13:12:01.000000 Apycula-0.8.2a1/apycula/GW1NZ-1.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)  1535793 2023-06-19 13:12:04.000000 Apycula-0.8.2a1/apycula/GW2A-18.pickle
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/apycula/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26023 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/apycula/attrids.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4745 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/apycula/bslib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    52156 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/apycula/chipdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12866 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/apycula/clock_fuzzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4411 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/apycula/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14047 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/apycula/dat19_h4x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8564 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/apycula/fuse_h4x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8421 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/apycula/gowin_bba.py
+-rw-r--r--   0 runner    (1001) docker     (123)    43038 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/apycula/gowin_pack.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45701 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/apycula/gowin_unpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4543 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/apycula/pindef.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10351 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/apycula/tiled_fuzzer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8138 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/apycula/tm_h4x.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7676 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/apycula/wirenames.py
+-rw-r--r--   0 runner    (1001) docker     (123)    84965 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/clock_experiments.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.030183 Apycula-0.8.2a1/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3650 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/doc/alu.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2890 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/doc/architecture.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3228 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/doc/commandstructure.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1726 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/doc/compression.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4674 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/doc/device_grouping.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.034183 Apycula-0.8.2a1/doc/fig/
+-rw-r--r--   0 runner    (1001) docker     (123)    17770 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/doc/fig/alu_logic.png
+-rw-r--r--   0 runner    (1001) docker     (123)    64550 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/doc/fig/alu_tile.png
+-rw-r--r--   0 runner    (1001) docker     (123)   285739 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/doc/fig/blinky.jpg
+-rw-r--r--   0 runner    (1001) docker     (123)    17036 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/doc/fig/clocks.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31670 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/doc/fig/clu.png
+-rw-r--r--   0 runner    (1001) docker     (123)    50702 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/doc/fig/floorplanner.png
+-rw-r--r--   0 runner    (1001) docker     (123)     6941 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/doc/fig/fuse.png
+-rw-r--r--   0 runner    (1001) docker     (123)   462042 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/doc/fig/lw.png
+-rw-r--r--   0 runner    (1001) docker     (123)  1358038 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/doc/fig/lw.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    20031 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/doc/fig/mux.png
+-rw-r--r--   0 runner    (1001) docker     (123)    49730 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/doc/fig/muxes-wiring.png
+-rw-r--r--   0 runner    (1001) docker     (123)   102610 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/doc/fig/post_pnr.png
+-rw-r--r--   0 runner    (1001) docker     (123)    53504 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/doc/fig/post_syn.png
+-rw-r--r--   0 runner    (1001) docker     (123)    37892 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/doc/fig/tile.png
+-rw-r--r--   0 runner    (1001) docker     (123)     8133 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/doc/filestructure.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4953 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/doc/longval-tables.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13330 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/doc/longwires.md
+-rw-r--r--   0 runner    (1001) docker     (123)      591 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/doc/muxes.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/doc/sdram.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.042183 Apycula-0.8.2a1/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)    11895 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.042183 Apycula-0.8.2a1/examples/attosoc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/attosoc/attosoc.v
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/attosoc/firmware.hex
+-rw-r--r--   0 runner    (1001) docker     (123)    94292 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/attosoc/picorv32.v
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/blinky-oddr.v
+-rw-r--r--   0 runner    (1001) docker     (123)      598 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/blinky-osc.v
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/blinky-tbuf.v
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/blinky.v
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.054183 Apycula-0.8.2a1/examples/deser/
+-rw-r--r--   0 runner    (1001) docker     (123)     6083 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/iddr-szfpga.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/iddr-tangnano.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/iddr-tangnano1k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/iddr-tangnano4k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/iddr-tangnano9k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/iddr.v
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/iddrc-szfpga.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/iddrc-tangnano.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/iddrc-tangnano1k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/iddrc-tangnano4k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/iddrc-tangnano9k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/iddrc.v
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ides10-szfpga.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ides10-tangnano.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ides10-tangnano1k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ides10-tangnano4k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ides10-tangnano9k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      902 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ides10.v
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ides16-szfpga.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ides16-tangnano4k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ides16-tangnano9k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ides16.v
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ides4-szfpga.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      831 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ides4-tangnano.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ides4-tangnano1k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ides4-tangnano4k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ides4-tangnano9k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ides4.v
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ides8-szfpga.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ides8-tangnano.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ides8-tangnano1k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ides8-tangnano4k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ides8-tangnano9k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      706 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ides8.v
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ivideo-szfpga.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      993 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ivideo-tangnano.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      937 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ivideo-tangnano1k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      348 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ivideo-tangnano4k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      936 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ivideo-tangnano9k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ivideo.v
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser10-szfpga.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser10-tangnano.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser10-tangnano4k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser10-tangnano9k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser10-tec0117.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser10-tlvds-tangnano4k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser10-tlvds-tangnano9k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser10-tlvds-tec0117.cst
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser10-tlvds.v
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser10.v
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser16-szfpga.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser16-tangnano4k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser16-tangnano9k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)     1437 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser16.v
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser4-szfpga.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser4-tangnano.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser4-tangnano4k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser4-tangnano9k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser4-tec0117.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser4-tlvds-tangnano4k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser4-tlvds-tangnano9k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser4-tlvds-tec0117.cst
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser4-tlvds.v
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser4.v
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser8-szfpga.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser8-tangnano.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser8-tangnano4k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser8-tangnano9k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser8-tec0117.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser8-tlvds-tangnano4k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser8-tlvds-tangnano9k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser8-tlvds-tec0117.cst
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser8-tlvds.v
+-rw-r--r--   0 runner    (1001) docker     (123)     1421 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/oser8.v
+-rw-r--r--   0 runner    (1001) docker     (123)      592 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ovideo-szfpga.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ovideo-tangnano.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ovideo-tangnano4k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ovideo-tangnano9k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ovideo-tec0117.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      362 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ovideo-tlvds-tangnano4k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ovideo-tlvds-tangnano9k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ovideo-tlvds-tec0117.cst
+-rw-r--r--   0 runner    (1001) docker     (123)     1387 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ovideo-tlvds.v
+-rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/deser/ovideo.v
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/elvds.v
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/honeycomb.cst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.058183 Apycula-0.8.2a1/examples/longwires/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/longwires/honeycomb.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      394 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/longwires/runber.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/longwires/tangnano.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/longwires/tangnano1k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/longwires/tangnano4k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      399 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/longwires/tangnano9k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      810 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/longwires/tec0117.cst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.058183 Apycula-0.8.2a1/examples/lutram/
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/lutram/README.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)      300 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/lutram/build.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/lutram/lutram.v
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/lutram/prbs.v
+-rw-r--r--   0 runner    (1001) docker     (123)     1813 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/lutram/top.v
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/lvds-szfpga.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/lvds-tangnano.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/lvds-tangnano1k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/lvds-tangnano4k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/lvds-tangnano9k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/lvds-tec0117.cst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.058183 Apycula-0.8.2a1/examples/nanolcd/
+-rw-r--r--   0 runner    (1001) docker     (123)     1450 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/nanolcd/TOP.v
+-rw-r--r--   0 runner    (1001) docker     (123)     4164 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/nanolcd/VGAMod.v
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/oddr-elvds.v
+-rw-r--r--   0 runner    (1001) docker     (123)      787 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/oddr-tlvds.v
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.058183 Apycula-0.8.2a1/examples/pll/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/pll/GW1N-1-52.vh
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/pll/GW1N-1-80.vh
+-rw-r--r--   0 runner    (1001) docker     (123)      254 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/pll/GW1N-1-dyn.vh
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/pll/GW1N-4-dyn.vh
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/pll/GW1N-9-dyn.vh
+-rw-r--r--   0 runner    (1001) docker     (123)      461 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/pll/GW1N-9C-dyn.vh
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/pll/GW1NS-2C-dyn.vh
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/pll/GW1NZ-1-54.vh
+-rw-r--r--   0 runner    (1001) docker     (123)      127 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/pll/GW1NZ-1-81.vh
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/pll/GW1NZ-1-dyn.vh
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/pll/pllvr.v
+-rw-r--r--   0 runner    (1001) docker     (123)     2039 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/pll/rpll.v
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.058183 Apycula-0.8.2a1/examples/pll-nanolcd/
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/pll-nanolcd/TOP.v
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/pll-nanolcd/VGAMod.v
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/pll-tangnano4k.v
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/pll.v
+-rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/pll2.v
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/primer20k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/runber-tlvds.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      357 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/runber.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/shift.v
+-rw-r--r--   0 runner    (1001) docker     (123)      584 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/tangnano.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      403 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/tangnano1k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      243 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/tangnano4k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/tangnano9k.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/tec0117.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/tlvds.v
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.062183 Apycula-0.8.2a1/examples/tonegen/
+-rw-r--r--   0 runner    (1001) docker     (123)     2323 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/tonegen/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/tonegen/cordic.v
+-rw-r--r--   0 runner    (1001) docker     (123)     2280 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/tonegen/sddac.v
+-rw-r--r--   0 runner    (1001) docker     (123)     1525 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/examples/tonegen/top.v
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8041 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/gowin-pll.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.062183 Apycula-0.8.2a1/legacy/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.062183 Apycula-0.8.2a1/legacy/empty/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/empty/device.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/empty/empty.v
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/empty/pnr.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/empty/run.tcl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.062183 Apycula-0.8.2a1/legacy/example/
+-rw-r--r--   0 runner    (1001) docker     (123)      248 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/example/example.cst
+-rw-r--r--   0 runner    (1001) docker     (123)      206 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/example/example.v
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/example/pnr.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/example/run.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)    20544 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/fuzzer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.066183 Apycula-0.8.2a1/legacy/generic/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.066183 Apycula-0.8.2a1/legacy/generic/attosoc/
+-rw-r--r--   0 runner    (1001) docker     (123)     3300 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/generic/attosoc/attosoc.v
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/generic/attosoc/firmware.hex
+-rw-r--r--   0 runner    (1001) docker     (123)    94292 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/generic/attosoc/picorv32.v
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/generic/attosoc/top.v
+-rw-r--r--   0 runner    (1001) docker     (123)     3248 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/generic/bitstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1061 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/generic/blinky.v
+-rw-r--r--   0 runner    (1001) docker     (123)      549 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/generic/blinkygw1n1.v
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.066183 Apycula-0.8.2a1/legacy/generic/nanolcd/
+-rw-r--r--   0 runner    (1001) docker     (123)     2853 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/generic/nanolcd/TOP.v
+-rw-r--r--   0 runner    (1001) docker     (123)     4129 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/generic/nanolcd/VGAMod.v
+-rw-r--r--   0 runner    (1001) docker     (123)     5758 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/generic/simple.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      339 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/generic/simple.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/generic/simple_timing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.066183 Apycula-0.8.2a1/legacy/generic/synth/
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/generic/synth/cells_map.v
+-rw-r--r--   0 runner    (1001) docker     (123)      920 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/generic/synth/prims.v
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/generic/synth/synth_generic.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/generic/write_fasm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/indices.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.070183 Apycula-0.8.2a1/legacy/iob/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/iob/device.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/iob/iob.cst.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/iob/iob.sdc
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/iob/iob.v
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/iob/pnr.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/iob/run.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/iob.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      528 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/json_display.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.070183 Apycula-0.8.2a1/legacy/lut4/
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/lut4/device.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/lut4/lut4.cst.mk
+-rw-r--r--   0 runner    (1001) docker     (123)      256 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/lut4/lut4.sdc
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/lut4/lut4.v
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/lut4/pnr.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/lut4/run.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/lut4.sh
+-rw-r--r--   0 runner    (1001) docker     (123)     4141 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/report.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-06-19 13:12:22.070183 Apycula-0.8.2a1/legacy/sdram/
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2251 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/sdram/find_sdram_pins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/sdram/findpin.tcl
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/sdram/findpin.vhd
+-rwxr-xr-x   0 runner    (1001) docker     (123)       71 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/sdram/run.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/sdram/template.vhd
+-rw-r--r--   0 runner    (1001) docker     (123)   813455 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/legacy/sdram/unpack.v
+-rw-r--r--   0 runner    (1001) docker     (123)     9033 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-06-19 13:12:22.074183 Apycula-0.8.2a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1031 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-06-19 13:11:59.000000 Apycula-0.8.2a1/test_clk.py
```

### Comparing `Apycula-0.8.1/.github/workflows/chipdb.yml` & `Apycula-0.8.2a1/.github/workflows/chipdb.yml`

 * *Files 6% similar despite different names*

```diff
@@ -133,17 +133,35 @@
           name: gw1ns-4-chipdb
           path: apycula/GW1NS-4.pickle
     - name: Archive stage artifact
       uses: actions/upload-artifact@v3
       with:
           name: gw1ns-4-stage
           path: GW1NS-4*
+  gw2a18:
+    runs-on: ubuntu-latest
+    steps:
+    - uses: actions/checkout@v3
+    - name: Build gw2a-18 chipdb
+      run: |
+        docker pull pepijndevos/apicula:1.9.8
+        docker run -v $(pwd):/usr/src/apicula pepijndevos/apicula:1.9.8 make apycula/GW2A-18.pickle
+    - name: Archive artifact
+      uses: actions/upload-artifact@v3
+      with:
+          name: gw2a-18-chipdb
+          path: apycula/GW2A-18.pickle
+    - name: Archive stage artifact
+      uses: actions/upload-artifact@v3
+      with:
+          name: gw2a-18-stage
+          path: GW2A-18*
   pypi:
     runs-on: ubuntu-latest
-    needs: [gw1n1, gw1nz1, gw1n9, gw1n9c, gw1n4, gw1ns2, gw1ns4]
+    needs: [gw1n1, gw1nz1, gw1n9, gw1n9c, gw1n4, gw1ns2, gw1ns4, gw2a18]
     steps:
     - uses: actions/checkout@v3
     - name: Download gw1n-1 chipdb
       uses: actions/download-artifact@v3
       with:
         name: gw1n-1-chipdb
         path: apycula
@@ -173,14 +191,19 @@
         name: gw1ns-2-chipdb
         path: apycula
     - name: Download gw1ns-4 chipdb
       uses: actions/download-artifact@v3
       with:
         name: gw1ns-4-chipdb
         path: apycula
+    - name: Download gw2a-18 chipdb
+      uses: actions/download-artifact@v3
+      with:
+        name: gw2a-18-chipdb
+        path: apycula
     - name: Set up Python
       uses: actions/setup-python@v4
       with:
         python-version: '3.8'
     - name: Install and build
       run: |
         python -m pip install --upgrade pip
@@ -194,15 +217,15 @@
           path: dist
     - name: Publish to Pypi
       if: startsWith(github.ref, 'refs/tags')
       env:
         TWINE_USERNAME: __token__
         TWINE_PASSWORD: ${{ secrets.PYPI_TOKEN }}
       run: |
-        twine upload dist/*
+        twine upload --verbose dist/*
     - name: Pack release data
       if: startsWith(github.ref, 'refs/heads/master')
       run: |
         tar cvfz linux-x64-gowin-data.tgz apycula/*.pickle
     - name: Upload to oss-cad-suite
       uses: ncipollo/release-action@v1
       if: hashFiles('linux-x64-gowin-data.tgz') != ''
```

### Comparing `Apycula-0.8.1/.github/workflows/yowasp_examples.yml` & `Apycula-0.8.2a1/.github/workflows/yowasp_examples.yml`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/Apycula.egg-info/PKG-INFO` & `Apycula-0.8.2a1/Apycula.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Apycula
-Version: 0.8.1
+Version: 0.8.2a1
 Summary: Open Source tools for Gowin FPGAs
 Home-page: https://github.com/YosysHQ/apicula
 Author: Pepijn de Vos
 Author-email: pepijndevos@gmail.com
 License: UNKNOWN
 Description: # Project Apicula
```

### Comparing `Apycula-0.8.1/Apycula.egg-info/SOURCES.txt` & `Apycula-0.8.2a1/Apycula.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .gitignore
 Dockerfile
 LICENSE
 Makefile
 clock_experiments.ipynb
+gowin-pll.py
 readme.md
 setup.py
 test_clk.py
 .github/workflows/chipdb.yml
 .github/workflows/yowasp_examples.yml
 Apycula.egg-info/PKG-INFO
 Apycula.egg-info/SOURCES.txt
@@ -17,14 +18,15 @@
 apycula/GW1N-1.pickle
 apycula/GW1N-4.pickle
 apycula/GW1N-9.pickle
 apycula/GW1N-9C.pickle
 apycula/GW1NS-2.pickle
 apycula/GW1NS-4.pickle
 apycula/GW1NZ-1.pickle
+apycula/GW2A-18.pickle
 apycula/__init__.py
 apycula/attrids.py
 apycula/bslib.py
 apycula/chipdb.py
 apycula/clock_fuzzer.py
 apycula/codegen.py
 apycula/dat19_h4x.py
@@ -74,14 +76,15 @@
 examples/lvds-tangnano9k.cst
 examples/lvds-tec0117.cst
 examples/oddr-elvds.v
 examples/oddr-tlvds.v
 examples/pll-tangnano4k.v
 examples/pll.v
 examples/pll2.v
+examples/primer20k.cst
 examples/runber-tlvds.cst
 examples/runber.cst
 examples/shift.v
 examples/tangnano.cst
 examples/tangnano1k.cst
 examples/tangnano4k.cst
 examples/tangnano9k.cst
```

### Comparing `Apycula-0.8.1/Dockerfile` & `Apycula-0.8.2a1/Dockerfile`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/LICENSE` & `Apycula-0.8.2a1/LICENSE`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/Makefile` & `Apycula-0.8.2a1/Makefile`

 * *Files 20% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 $(error GOWINHOME is not set. Must be location of Gowin EDA Tools)
 endif
 
 .SECONDARY:
 .PHONY: all clean
 all: apycula/GW1N-1.pickle apycula/GW1N-9.pickle apycula/GW1N-4.pickle \
 	 apycula/GW1NS-2.pickle apycula/GW1NS-4.pickle apycula/GW1N-9C.pickle \
-	 apycula/GW1NZ-1.pickle
+	 apycula/GW1NZ-1.pickle apycula/GW2A-18.pickle
 
 %.json: apycula/dat19_h4x.py
 	python3 -m apycula.dat19_h4x $*
 
 %_stage1.pickle: apycula/tiled_fuzzer.py %.json
 	python3 -m apycula.tiled_fuzzer $*
 
 %_stage2.pickle: apycula/clock_fuzzer.py %_stage1.pickle
 	python3 -m apycula.clock_fuzzer $*
 
 apycula/%.pickle: %_stage2.pickle
-	cp $< $@
+	gzip -c $< > $@
 
 clean:
 	rm *.json
 	rm *.pickle
 	rm apycula/*.pickle
```

### Comparing `Apycula-0.8.1/PKG-INFO` & `Apycula-0.8.2a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Apycula
-Version: 0.8.1
+Version: 0.8.2a1
 Summary: Open Source tools for Gowin FPGAs
 Home-page: https://github.com/YosysHQ/apicula
 Author: Pepijn de Vos
 Author-email: pepijndevos@gmail.com
 License: UNKNOWN
 Description: # Project Apicula
```

### Comparing `Apycula-0.8.1/apycula/attrids.py` & `Apycula-0.8.2a1/apycula/attrids.py`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/apycula/bslib.py` & `Apycula-0.8.2a1/apycula/bslib.py`

 * *Files 2% similar despite different names*

```diff
@@ -52,14 +52,16 @@
                         padding = 0
                     elif ba == b'\x06\x00\x00\x00\x01\x00h\x1b':
                         padding = 0
                     elif ba == b'\x06\x00\x00\x00\x03\x00\x18\x1b':
                         padding = 0
                     elif ba == b'\x06\x00\x00\x00\x01\x00\x98\x1b':
                         padding = 0
+                    elif ba == b'\x06\x00\x00\x00\x00\x00\x08\x1b':
+                        padding = 0
                     else:
                         raise ValueError("Unsupported device", ba)
                 preamble = max(0, preamble-1)
                 continue
             crcdat.extend(ba[:-8])
             crc1 = (ba[-7] << 8) + ba[-8]
             crc2 = crc16arc(crcdat)
```

### Comparing `Apycula-0.8.1/apycula/chipdb.py` & `Apycula-0.8.2a1/apycula/chipdb.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,15 +333,15 @@
             'DO': ("F0", "F1", "F2", "F3"),
         }
     return luts
 
 def fse_osc(device, fse, ttyp):
     osc = {}
 
-    if device in {'GW1N-4', 'GW1N-9', 'GW1N-9C'}:
+    if device in {'GW1N-4', 'GW1N-9', 'GW1N-9C', 'GW2A-18'}:
         bel = osc.setdefault(f"OSC", Bel())
     elif device in {'GW1NZ-1', 'GW1NS-4'}:
         bel = osc.setdefault(f"OSCZ", Bel())
     elif device == 'GW1NS-2':
         bel = osc.setdefault(f"OSCF", Bel())
     elif device == 'GW1N-1':
         bel = osc.setdefault(f"OSCH", Bel())
@@ -788,15 +788,15 @@
 def add_attr_val(dev, logic_table, attrs, attr, val):
     for idx, attr_val in enumerate(dev.logicinfo[logic_table]):
         if attr_val[0] == attr and attr_val[1] == val:
             attrs.add(idx)
             break
 
 def get_pins(device):
-    if device not in {"GW1N-1", "GW1NZ-1", "GW1N-4", "GW1N-9", "GW1NR-9", "GW1N-9C", "GW1NR-9C", "GW1NS-2", "GW1NS-2C", "GW1NS-4", "GW1NSR-4C"}:
+    if device not in {"GW1N-1", "GW1NZ-1", "GW1N-4", "GW1N-9", "GW1NR-9", "GW1N-9C", "GW1NR-9C", "GW1NS-2", "GW1NS-2C", "GW1NS-4", "GW1NSR-4C", "GW2A-18"}:
         raise Exception(f"unsupported device {device}")
     pkgs = pindef.all_packages(device)
     res = {}
     res_bank_pins = {}
     for pkg_rec in pkgs.values():
         pkg = pkg_rec[0]
         if pkg in res:
@@ -870,14 +870,19 @@
         res_bank_pins = {}
         res_bank_pins.update(bank_pins)
         res_bank_pins.update(bank_pins_c)
         return (res, {
             "GW1NS-2": pins,
             "GW1NS-2C": pins_c
         }, res_bank_pins)
+    if device == "GW2A-18":
+        pkgs, pins, bank_pins = get_pins("GW2A-18")
+        return (pkgs, {
+            "GW2A-18": pins
+        }, bank_pins)
     else:
         raise Exception("unsupported device")
 
 _pll_inputs = [(5, 'CLKFB'), (6, 'FBDSEL0'), (7, 'FBDSEL1'), (8, 'FBDSEL2'), (9, 'FBDSEL3'),
                (10, 'FBDSEL4'), (11, 'FBDSEL5'),
                (12, 'IDSEL0'), (13, 'IDSEL1'), (14, 'IDSEL2'), (15, 'IDSEL3'), (16, 'IDSEL4'),
                (17, 'IDSEL5'),
@@ -915,14 +920,16 @@
 _osc_ports = {('OSCZ', 'GW1NZ-1'): ({}, {'OSCOUT' : (0, 5, 'OF3'), 'OSCEN': (0, 2, 'A6')}),
               ('OSCZ', 'GW1NS-4'): ({'OSCOUT': 'Q4', 'OSCEN': 'D6'}, {}),
               ('OSCF', 'GW1NS-2'): ({}, {'OSCOUT': (10, 19, 'Q4'), 'OSCEN': (13, 19, 'B3')}),
               ('OSCH', 'GW1N-1'):  ({'OSCOUT': 'Q4'}, {}),
               ('OSC',  'GW1N-4'):  ({'OSCOUT': 'Q4'}, {}),
               ('OSC',  'GW1N-9'):  ({'OSCOUT': 'Q4'}, {}),
               ('OSC',  'GW1N-9C'):  ({'OSCOUT': 'Q4'}, {}),
+              # XXX check this!
+              ('OSC',  'GW2A-18'):  ({'OSCOUT': 'Q4'}, {}),
               # XXX unsupported boards, pure theorizing
               ('OSCO', 'GW1N-2'):  ({'OSCOUT': 'Q7'}, {'OSCEN': (9, 1, 'B4')}),
               ('OSCW', 'GW2AN-18'):  ({'OSCOUT': 'Q4'}, {}),
               }
 def dat_portmap(dat, dev, device):
     for row, row_dat in enumerate(dev.grid):
         for col, tile in enumerate(row_dat):
```

### Comparing `Apycula-0.8.1/apycula/clock_fuzzer.py` & `Apycula-0.8.2a1/apycula/clock_fuzzer.py`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/apycula/codegen.py` & `Apycula-0.8.2a1/apycula/codegen.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,15 +131,15 @@
 add_file -type netlist {netlist}
 set_device {device_desc}
 set_option {opt}
 run pnr
             """
 
         device_desc = self.partnumber
-        if self.device in ['GW1N-9', 'GW1N-4', 'GW1N-9C']:
+        if self.device in ['GW1N-9', 'GW1N-4', 'GW1N-9C', 'GW2A-18']:
             device_desc = f'-name {self.device} {device_desc}'
 
         f.write(template.format(
             cst=self.cst,
             netlist=self.netlist,
             device=self.device,
             device_desc=device_desc,
```

### Comparing `Apycula-0.8.1/apycula/dat19_h4x.py` & `Apycula-0.8.2a1/apycula/dat19_h4x.py`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/apycula/fuse_h4x.py` & `Apycula-0.8.2a1/apycula/fuse_h4x.py`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/apycula/gowin_bba.py` & `Apycula-0.8.2a1/apycula/gowin_bba.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import sys
 import importlib.resources
 import pickle
+import gzip
 import argparse
 import re
 from contextlib import contextmanager
 from collections import Counter
 from apycula import chipdb
 
 class Bba(object):
@@ -250,13 +251,13 @@
     parser = argparse.ArgumentParser(description='Make Gowin BBA')
     parser.add_argument('-d', '--device', required=True)
     parser.add_argument('-i', '--constids', type=argparse.FileType('r'), default=sys.stdin)
     parser.add_argument('-o', '--output', type=argparse.FileType('w'), default=sys.stdout)
 
     args = parser.parse_args()
     read_constids(args.constids)
-    with importlib.resources.open_binary("apycula", f"{args.device}.pickle") as f:
+    with gzip.open(importlib.resources.files("apycula").joinpath(f"{args.device}.pickle"), 'rb') as f:
         db = pickle.load(f)
     write_chipdb(db, args.output, args.device)
 
 if __name__ == "__main__":
     main()
```

### Comparing `Apycula-0.8.1/apycula/gowin_pack.py` & `Apycula-0.8.2a1/apycula/gowin_pack.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import sys
 import os
 import re
 import pickle
+import gzip
 import itertools
 import math
 import numpy as np
 import json
 import argparse
 import importlib.resources
 from collections import namedtuple
@@ -976,16 +977,15 @@
     device = args.device
     # For tool integration it is allowed to pass a full part number
     m = re.match("GW1N(S|Z)?[A-Z]*-(LV|UV|UX)([0-9])C?([A-Z]{2}[0-9]+P?)(C[0-9]/I[0-9])", device)
     if m:
         mods = m.group(1) or ""
         luts = m.group(3)
         device = f"GW1N{mods}-{luts}"
-
-    with importlib.resources.open_binary("apycula", f"{device}.pickle") as f:
+    with gzip.open(importlib.resources.files("apycula").joinpath(f"{device}.pickle"), 'rb') as f:
         db = pickle.load(f)
     with open(args.netlist) as f:
         pnr = json.load(f)
 
     _vcc_net = pnr['modules']['top']['netnames']['$PACKER_VCC_NET']['bits']
     _gnd_net = pnr['modules']['top']['netnames']['$PACKER_GND_NET']['bits']
```

### Comparing `Apycula-0.8.1/apycula/gowin_unpack.py` & `Apycula-0.8.2a1/apycula/gowin_unpack.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import sys
 import os
 import re
 import random
 import numpy as np
 from itertools import chain, count
 import pickle
+import gzip
 import argparse
 import importlib.resources
 from apycula import codegen
 from apycula import chipdb
 from apycula import attrids
 from apycula.bslib import read_bitstream
 from apycula.wirenames import wirenames
@@ -1043,15 +1044,15 @@
     # For tool integration it is allowed to pass a full part number
     m = re.match("GW1N(S?)[A-Z]*-(LV|UV|UX)([0-9])C?([A-Z]{2}[0-9]+P?)(C[0-9]/I[0-9])", _device)
     if m:
         mods = m.group(1)
         luts = m.group(3)
         _device = f"GW1N{mods}-{luts}"
 
-    with importlib.resources.open_binary("apycula", f"{_device}.pickle") as f:
+    with gzip.open(importlib.resources.files("apycula").joinpath(f"{_device}.pickle"), 'rb') as f:
         db = pickle.load(f)
 
     global _pinout
     _pinout = db.pinout[_device][_packages[_device]]
 
     bitmap = read_bitstream(args.bitstream)[0]
     bm = chipdb.tile_bitmap(db, bitmap)
```

### Comparing `Apycula-0.8.1/apycula/pindef.py` & `Apycula-0.8.2a1/apycula/pindef.py`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/apycula/tiled_fuzzer.py` & `Apycula-0.8.2a1/apycula/tiled_fuzzer.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,14 +64,19 @@
         "partnumber": "GW1N-LV1LQ144C6/I5",
     },
     "GW1NZ-1": {
         "package": "QFN48",
         "device": "GW1NZ-1-QFN48-6",
         "partnumber": "GW1NZ-LV1QN48C6/I5",
     },
+    "GW2A-18": {
+        "package": "PBGA256",
+        "device": "GW2A-18-PBGA256-8",
+        "partnumber": "GW2A-LV18PG256C8/I7",
+    },
 }[device]
 
 # utils
 name_idx = 0
 def make_name(bel, typ):
     global name_idx
     name_idx += 1
@@ -271,15 +276,18 @@
 
     # set template dual-mode pins to HW mode
     dualmode_pins = {'jtag', 'sspi', 'mspi', 'ready', 'done', 'reconfig', 'i2c'}
     for pin in dualmode_pins:
         name = pin.upper()
         cfg_attrs = set()
         chipdb.add_attr_val(db, 'CFG', cfg_attrs, attrids.cfg_attrids[f'{name}_AS_GPIO'], attrids.cfg_attrvals['YES'])
-        bits = chipdb.get_shortval_fuses(db, fse['header']['grid'][61][0][0], cfg_attrs, 'CFG')
+        if device == 'GW2A-18':
+            bits = chipdb.get_shortval_fuses(db, fse['header']['grid'][61][0][-1], cfg_attrs, 'CFG')
+        else:
+            bits = chipdb.get_shortval_fuses(db, fse['header']['grid'][61][0][0], cfg_attrs, 'CFG')
         tile = db.template
         for row_, col_ in bits:
             tile[row_][col_] = 0
         db.grid[0][0].bels.setdefault('CFG', chipdb.Bel()).flags[name] = bits
 
     # GSR
     db.grid[0][0].bels.setdefault('GSR0', chipdb.Bel()).portmap['GSRI'] = 'C4';
```

### Comparing `Apycula-0.8.1/apycula/tm_h4x.py` & `Apycula-0.8.2a1/apycula/tm_h4x.py`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/apycula/wirenames.py` & `Apycula-0.8.2a1/apycula/wirenames.py`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/clock_experiments.ipynb` & `Apycula-0.8.2a1/clock_experiments.ipynb`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/doc/alu.md` & `Apycula-0.8.2a1/doc/alu.md`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/doc/architecture.md` & `Apycula-0.8.2a1/doc/architecture.md`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/doc/commandstructure.md` & `Apycula-0.8.2a1/doc/commandstructure.md`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/doc/compression.md` & `Apycula-0.8.2a1/doc/compression.md`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/doc/device_grouping.md` & `Apycula-0.8.2a1/doc/device_grouping.md`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/doc/fig/alu_logic.png` & `Apycula-0.8.2a1/doc/fig/alu_logic.png`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/doc/fig/alu_tile.png` & `Apycula-0.8.2a1/doc/fig/alu_tile.png`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/doc/fig/blinky.jpg` & `Apycula-0.8.2a1/doc/fig/blinky.jpg`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/doc/fig/clocks.png` & `Apycula-0.8.2a1/doc/fig/clocks.png`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/doc/fig/clu.png` & `Apycula-0.8.2a1/doc/fig/clu.png`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/doc/fig/floorplanner.png` & `Apycula-0.8.2a1/doc/fig/floorplanner.png`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/doc/fig/fuse.png` & `Apycula-0.8.2a1/doc/fig/fuse.png`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/doc/fig/lw.png` & `Apycula-0.8.2a1/doc/fig/lw.png`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/doc/fig/lw.svg` & `Apycula-0.8.2a1/doc/fig/lw.svg`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/doc/fig/mux.png` & `Apycula-0.8.2a1/doc/fig/mux.png`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/doc/fig/muxes-wiring.png` & `Apycula-0.8.2a1/doc/fig/muxes-wiring.png`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/doc/fig/post_pnr.png` & `Apycula-0.8.2a1/doc/fig/post_pnr.png`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/doc/fig/post_syn.png` & `Apycula-0.8.2a1/doc/fig/post_syn.png`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/doc/fig/tile.png` & `Apycula-0.8.2a1/doc/fig/tile.png`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/doc/filestructure.md` & `Apycula-0.8.2a1/doc/filestructure.md`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/doc/longval-tables.md` & `Apycula-0.8.2a1/doc/longval-tables.md`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/doc/longwires.md` & `Apycula-0.8.2a1/doc/longwires.md`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/doc/muxes.md` & `Apycula-0.8.2a1/doc/muxes.md`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/doc/sdram.md` & `Apycula-0.8.2a1/doc/sdram.md`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/Makefile` & `Apycula-0.8.2a1/examples/Makefile`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,16 @@
 NEXTPNR ?= nextpnr-gowin
 
 .DEFAULT_GOAL := all
 
 include deser/Makefile
 
 all: attosoc-tec0117.fs nanolcd-tangnano.fs blinky-tec0117.fs blinky-runber.fs \
-	blinky-tangnano.fs blinky-honeycomb.fs shift-tec0117.fs shift-runber.fs \
+	blinky-tangnano.fs blinky-honeycomb.fs blinky-primer20k.fs \
+	shift-tec0117.fs shift-runber.fs \
 	shift-tangnano.fs shift-honeycomb.fs \
 	tonegen-tec0117.fs blinky-tangnano9k.fs blinky-tangnano1k.fs blinky-tangnano4k.fs \
 	blinky-tbuf-tangnano.fs blinky-tbuf-tangnano1k.fs blinky-tbuf-tangnano4k.fs \
 	blinky-tbuf-tangnano9k.fs blinky-tbuf-tec0117.fs blinky-tbuf-runber.fs \
 	blinky-tbuf-honeycomb.fs \
 	shift-tangnano9k.fs shift-tangnano1k.fs shift-tangnano4k.fs \
 	tlvds-tangnano4k.fs tlvds-tangnano9k.fs tlvds-tec0117.fs tlvds-szfpga.fs \
@@ -61,14 +62,20 @@
 	unpacked_deser
 	
 clean: clean_deser
 	rm -f *.json *.fs *-unpacked.v
 	
 .PHONY: all unpacked clean
 
+%-primer20k.fs: %-primer20k.json
+	gowin_pack -d GW2A-18 -o $@ $<
+
+%-primer20k.json: %-primer20k-synth.json primer20k.cst
+	$(NEXTPNR) --json $< --write $@ --device GW2A-LV18PG256C8/I7 --cst primer20k.cst
+
 %-tec0117.fs: %-tec0117.json
 	gowin_pack -d GW1N-9 -o $@ $<
 
 %-tec0117.json: %-tec0117-synth.json tec0117.cst
 	$(NEXTPNR) --json $< --write $@ --device GW1NR-LV9QN88C6/I5 --cst tec0117.cst
 
 %lvds-tec0117.json: %lvds-tec0117-synth.json lvds-tec0117.cst
@@ -157,14 +164,17 @@
 
 pll2-tec0117-synth.json: pll/GW1N-9-dyn.vh pll2.v pll/rpll.v
 	$(YOSYS) -D LEDS_NR=8 -D OSC_TYPE_OSC -p "read_verilog $^; synth_gowin -json $@"
 
 pll2-runber-synth.json: pll/GW1N-4-dyn.vh pll2.v pll/rpll.v
 	$(YOSYS) -p "read_verilog $^; synth_gowin -noalu -json $@"
 
+%-primer20k-synth.json: %.v
+	$(YOSYS) -D LEDS_NR=6 -D OSC_TYPE_OSC -p "read_verilog $^; synth_gowin -json $@"
+
 %-tec0117-synth.json: %.v
 	$(YOSYS) -D LEDS_NR=8 -D OSC_TYPE_OSC -p "read_verilog $^; synth_gowin -json $@"
 
 %-runber-synth.json: %.v
 	$(YOSYS) -D LEDS_NR=8 -D OSC_TYPE_OSC -p "read_verilog $^; synth_gowin -json $@"
 
 pll-%-tangnano-synth.json: pll/GW1N-1-%.vh pll.v pll/rpll.v
```

### Comparing `Apycula-0.8.1/examples/attosoc/attosoc.v` & `Apycula-0.8.2a1/examples/attosoc/attosoc.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/attosoc/picorv32.v` & `Apycula-0.8.2a1/examples/attosoc/picorv32.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/blinky-oddr.v` & `Apycula-0.8.2a1/examples/blinky-oddr.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/blinky-osc.v` & `Apycula-0.8.2a1/examples/blinky-osc.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/Makefile` & `Apycula-0.8.2a1/examples/deser/Makefile`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/iddr-szfpga.cst` & `Apycula-0.8.2a1/examples/deser/iddr-szfpga.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/iddr-tangnano.cst` & `Apycula-0.8.2a1/examples/deser/iddr-tangnano.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/iddr-tangnano1k.cst` & `Apycula-0.8.2a1/examples/deser/iddr-tangnano1k.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/iddr-tangnano9k.cst` & `Apycula-0.8.2a1/examples/deser/iddr-tangnano9k.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/iddrc-szfpga.cst` & `Apycula-0.8.2a1/examples/deser/iddrc-szfpga.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/iddrc-tangnano.cst` & `Apycula-0.8.2a1/examples/deser/iddrc-tangnano.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/iddrc-tangnano1k.cst` & `Apycula-0.8.2a1/examples/deser/iddrc-tangnano1k.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/iddrc-tangnano9k.cst` & `Apycula-0.8.2a1/examples/deser/iddrc-tangnano9k.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ides10-szfpga.cst` & `Apycula-0.8.2a1/examples/deser/ides10-szfpga.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ides10-tangnano.cst` & `Apycula-0.8.2a1/examples/deser/ides10-tangnano.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ides10-tangnano1k.cst` & `Apycula-0.8.2a1/examples/deser/ides10-tangnano1k.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ides10-tangnano9k.cst` & `Apycula-0.8.2a1/examples/deser/ides10-tangnano9k.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ides10.v` & `Apycula-0.8.2a1/examples/deser/ides10.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ides16-szfpga.cst` & `Apycula-0.8.2a1/examples/deser/ides16-szfpga.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ides16-tangnano9k.cst` & `Apycula-0.8.2a1/examples/deser/ides16-tangnano9k.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ides16.v` & `Apycula-0.8.2a1/examples/deser/ides16.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ides4-szfpga.cst` & `Apycula-0.8.2a1/examples/deser/ides4-szfpga.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ides4-tangnano.cst` & `Apycula-0.8.2a1/examples/deser/ides4-tangnano.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ides4-tangnano1k.cst` & `Apycula-0.8.2a1/examples/deser/ides4-tangnano1k.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ides4-tangnano9k.cst` & `Apycula-0.8.2a1/examples/deser/ides4-tangnano9k.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ides4.v` & `Apycula-0.8.2a1/examples/deser/ides4.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ides8-szfpga.cst` & `Apycula-0.8.2a1/examples/deser/ides8-szfpga.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ides8-tangnano.cst` & `Apycula-0.8.2a1/examples/deser/ides8-tangnano.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ides8-tangnano1k.cst` & `Apycula-0.8.2a1/examples/deser/ides8-tangnano1k.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ides8-tangnano9k.cst` & `Apycula-0.8.2a1/examples/deser/ides8-tangnano9k.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ides8.v` & `Apycula-0.8.2a1/examples/deser/ides8.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ivideo-szfpga.cst` & `Apycula-0.8.2a1/examples/deser/ivideo-szfpga.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ivideo-tangnano.cst` & `Apycula-0.8.2a1/examples/deser/ivideo-tangnano.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ivideo-tangnano1k.cst` & `Apycula-0.8.2a1/examples/deser/ivideo-tangnano1k.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ivideo-tangnano9k.cst` & `Apycula-0.8.2a1/examples/deser/ivideo-tangnano9k.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ivideo.v` & `Apycula-0.8.2a1/examples/deser/ivideo.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/oser10-szfpga.cst` & `Apycula-0.8.2a1/examples/deser/oser10-szfpga.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/oser10-tec0117.cst` & `Apycula-0.8.2a1/examples/deser/oser10-tec0117.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/oser10-tlvds-tangnano9k.cst` & `Apycula-0.8.2a1/examples/deser/oser10-tlvds-tangnano9k.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/oser10-tlvds-tec0117.cst` & `Apycula-0.8.2a1/examples/deser/oser10-tlvds-tec0117.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/oser10-tlvds.v` & `Apycula-0.8.2a1/examples/deser/oser10-tlvds.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/oser10.v` & `Apycula-0.8.2a1/examples/deser/oser10.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/oser16.v` & `Apycula-0.8.2a1/examples/deser/oser16.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/oser4-szfpga.cst` & `Apycula-0.8.2a1/examples/deser/oser4-szfpga.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/oser4-tec0117.cst` & `Apycula-0.8.2a1/examples/deser/oser4-tec0117.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/oser4-tlvds-tangnano9k.cst` & `Apycula-0.8.2a1/examples/deser/oser4-tlvds-tangnano9k.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/oser4-tlvds-tec0117.cst` & `Apycula-0.8.2a1/examples/deser/oser4-tlvds-tec0117.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/oser4-tlvds.v` & `Apycula-0.8.2a1/examples/deser/oser4-tlvds.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/oser4.v` & `Apycula-0.8.2a1/examples/deser/oser4.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/oser8-szfpga.cst` & `Apycula-0.8.2a1/examples/deser/oser8-szfpga.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/oser8-tec0117.cst` & `Apycula-0.8.2a1/examples/deser/oser8-tec0117.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/oser8-tlvds-tangnano9k.cst` & `Apycula-0.8.2a1/examples/deser/oser8-tlvds-tangnano9k.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/oser8-tlvds-tec0117.cst` & `Apycula-0.8.2a1/examples/deser/oser8-tlvds-tec0117.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/oser8-tlvds.v` & `Apycula-0.8.2a1/examples/deser/oser8-tlvds.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/oser8.v` & `Apycula-0.8.2a1/examples/deser/oser8.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ovideo-szfpga.cst` & `Apycula-0.8.2a1/examples/deser/ovideo-szfpga.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ovideo-tec0117.cst` & `Apycula-0.8.2a1/examples/deser/ovideo-tec0117.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ovideo-tlvds-tangnano9k.cst` & `Apycula-0.8.2a1/examples/deser/ovideo-tlvds-tangnano9k.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ovideo-tlvds-tec0117.cst` & `Apycula-0.8.2a1/examples/deser/ovideo-tlvds-tec0117.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ovideo-tlvds.v` & `Apycula-0.8.2a1/examples/deser/ovideo-tlvds.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/deser/ovideo.v` & `Apycula-0.8.2a1/examples/deser/ovideo.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/elvds.v` & `Apycula-0.8.2a1/examples/elvds.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/longwires/tangnano.cst` & `Apycula-0.8.2a1/examples/longwires/tangnano.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/longwires/tec0117.cst` & `Apycula-0.8.2a1/examples/longwires/tec0117.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/lutram/top.v` & `Apycula-0.8.2a1/examples/lutram/top.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/lvds-tec0117.cst` & `Apycula-0.8.2a1/examples/lvds-tec0117.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/nanolcd/TOP.v` & `Apycula-0.8.2a1/examples/nanolcd/TOP.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/nanolcd/VGAMod.v` & `Apycula-0.8.2a1/examples/nanolcd/VGAMod.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/oddr-elvds.v` & `Apycula-0.8.2a1/examples/oddr-elvds.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/oddr-tlvds.v` & `Apycula-0.8.2a1/examples/oddr-tlvds.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/pll/pllvr.v` & `Apycula-0.8.2a1/examples/pll/pllvr.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/pll/rpll.v` & `Apycula-0.8.2a1/examples/pll/rpll.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/pll-nanolcd/TOP.v` & `Apycula-0.8.2a1/examples/pll-nanolcd/TOP.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/pll-nanolcd/VGAMod.v` & `Apycula-0.8.2a1/examples/pll-nanolcd/VGAMod.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/pll-tangnano4k.v` & `Apycula-0.8.2a1/examples/pll-tangnano4k.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/pll.v` & `Apycula-0.8.2a1/examples/pll.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/pll2.v` & `Apycula-0.8.2a1/examples/pll2.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/shift.v` & `Apycula-0.8.2a1/examples/shift.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/tangnano.cst` & `Apycula-0.8.2a1/examples/tangnano.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/tangnano9k.cst` & `Apycula-0.8.2a1/examples/tangnano9k.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/tec0117.cst` & `Apycula-0.8.2a1/examples/tec0117.cst`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/tlvds.v` & `Apycula-0.8.2a1/examples/tlvds.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/tonegen/README.md` & `Apycula-0.8.2a1/examples/tonegen/README.md`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/tonegen/cordic.v` & `Apycula-0.8.2a1/examples/tonegen/cordic.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/tonegen/sddac.v` & `Apycula-0.8.2a1/examples/tonegen/sddac.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/examples/tonegen/top.v` & `Apycula-0.8.2a1/examples/tonegen/top.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/legacy/example/run.tcl` & `Apycula-0.8.2a1/legacy/example/run.tcl`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/legacy/fuzzer.py` & `Apycula-0.8.2a1/legacy/fuzzer.py`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/legacy/generic/attosoc/attosoc.v` & `Apycula-0.8.2a1/legacy/generic/attosoc/attosoc.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/legacy/generic/attosoc/picorv32.v` & `Apycula-0.8.2a1/legacy/generic/attosoc/picorv32.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/legacy/generic/attosoc/top.v` & `Apycula-0.8.2a1/legacy/generic/attosoc/top.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/legacy/generic/bitstream.py` & `Apycula-0.8.2a1/legacy/generic/bitstream.py`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/legacy/generic/blinky.v` & `Apycula-0.8.2a1/legacy/generic/blinky.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/legacy/generic/blinkygw1n1.v` & `Apycula-0.8.2a1/legacy/generic/blinkygw1n1.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/legacy/generic/nanolcd/TOP.v` & `Apycula-0.8.2a1/legacy/generic/nanolcd/TOP.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/legacy/generic/nanolcd/VGAMod.v` & `Apycula-0.8.2a1/legacy/generic/nanolcd/VGAMod.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/legacy/generic/simple.py` & `Apycula-0.8.2a1/legacy/generic/simple.py`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/legacy/generic/simple_timing.py` & `Apycula-0.8.2a1/legacy/generic/simple_timing.py`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/legacy/generic/synth/prims.v` & `Apycula-0.8.2a1/legacy/generic/synth/prims.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/legacy/generic/synth/synth_generic.tcl` & `Apycula-0.8.2a1/legacy/generic/synth/synth_generic.tcl`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/legacy/generic/write_fasm.py` & `Apycula-0.8.2a1/legacy/generic/write_fasm.py`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/legacy/iob.sh` & `Apycula-0.8.2a1/legacy/iob.sh`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/legacy/json_display.py` & `Apycula-0.8.2a1/legacy/json_display.py`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/legacy/lut4/lut4.v` & `Apycula-0.8.2a1/legacy/lut4/lut4.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/legacy/lut4.sh` & `Apycula-0.8.2a1/legacy/lut4.sh`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/legacy/report.py` & `Apycula-0.8.2a1/legacy/report.py`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/legacy/sdram/find_sdram_pins.py` & `Apycula-0.8.2a1/legacy/sdram/find_sdram_pins.py`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/legacy/sdram/unpack.v` & `Apycula-0.8.2a1/legacy/sdram/unpack.v`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/readme.md` & `Apycula-0.8.2a1/readme.md`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/setup.py` & `Apycula-0.8.2a1/setup.py`

 * *Files identical despite different names*

### Comparing `Apycula-0.8.1/test_clk.py` & `Apycula-0.8.2a1/test_clk.py`

 * *Files identical despite different names*

