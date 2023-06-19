# Comparing `tmp/pybiotk-1.1.1.tar.gz` & `tmp/pybiotk-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybiotk-1.1.1.tar", last modified: Tue Jan 31 08:23:13 2023, max compression
+gzip compressed data, was "pybiotk-1.2.0.tar", last modified: Mon Jun 19 02:25:39 2023, max compression
```

## Comparing `pybiotk-1.1.1.tar` & `pybiotk-1.2.0.tar`

### file list

```diff
@@ -1,133 +1,137 @@
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-01-31 08:23:13.914969 pybiotk-1.1.1/
--rw-r--r--   0 mac        (501) staff       (20)      590 2022-10-10 07:39:18.000000 pybiotk-1.1.1/.coveragerc
--rw-r--r--   0 mac        (501) staff       (20)      583 2022-10-10 07:39:18.000000 pybiotk-1.1.1/.gitignore
--rw-r--r--   0 mac        (501) staff       (20)      490 2022-10-10 07:39:18.000000 pybiotk-1.1.1/.readthedocs.yml
--rw-r--r--   0 mac        (501) staff       (20)       77 2022-10-10 07:39:18.000000 pybiotk-1.1.1/AUTHORS.rst
--rw-r--r--   0 mac        (501) staff       (20)      128 2022-10-10 07:39:18.000000 pybiotk-1.1.1/CHANGELOG.rst
--rw-r--r--   0 mac        (501) staff       (20)    13815 2022-10-10 07:39:18.000000 pybiotk-1.1.1/CONTRIBUTING.rst
--rw-r--r--   0 mac        (501) staff       (20)     1079 2022-10-10 07:39:18.000000 pybiotk-1.1.1/LICENSE.txt
--rw-r--r--   0 mac        (501) staff       (20)     3780 2023-01-31 08:23:13.915149 pybiotk-1.1.1/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     3375 2022-10-28 07:10:30.000000 pybiotk-1.1.1/README.md
--rw-r--r--   0 mac        (501) staff       (20)     3950 2022-10-10 07:39:18.000000 pybiotk-1.1.1/README.rst
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-01-31 08:23:13.879051 pybiotk-1.1.1/docs/
--rw-r--r--   0 mac        (501) staff       (20)     1154 2023-01-30 02:10:43.000000 pybiotk-1.1.1/docs/Makefile
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-01-31 08:23:13.879350 pybiotk-1.1.1/docs/_static/
--rw-r--r--   0 mac        (501) staff       (20)       18 2023-01-30 02:10:43.000000 pybiotk-1.1.1/docs/_static/.gitignore
--rw-r--r--   0 mac        (501) staff       (20)       41 2023-01-30 02:10:43.000000 pybiotk-1.1.1/docs/authors.rst
--rw-r--r--   0 mac        (501) staff       (20)       43 2023-01-30 02:10:43.000000 pybiotk-1.1.1/docs/changelog.rst
--rw-r--r--   0 mac        (501) staff       (20)     9734 2023-01-30 02:10:43.000000 pybiotk-1.1.1/docs/conf.py
--rw-r--r--   0 mac        (501) staff       (20)       33 2023-01-30 02:10:43.000000 pybiotk-1.1.1/docs/contributing.rst
--rw-r--r--   0 mac        (501) staff       (20)     2313 2023-01-30 02:10:43.000000 pybiotk-1.1.1/docs/index.rst
--rw-r--r--   0 mac        (501) staff       (20)       67 2023-01-30 02:10:43.000000 pybiotk-1.1.1/docs/license.rst
--rw-r--r--   0 mac        (501) staff       (20)       39 2023-01-30 02:10:43.000000 pybiotk-1.1.1/docs/readme.rst
--rw-r--r--   0 mac        (501) staff       (20)      122 2023-01-30 02:10:43.000000 pybiotk-1.1.1/docs/requirements.txt
--rw-r--r--   0 mac        (501) staff       (20)      408 2022-10-10 07:39:18.000000 pybiotk-1.1.1/pyproject.toml
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-01-31 08:23:13.883633 pybiotk-1.1.1/rscripts/
--rwxr-xr-x   0 mac        (501) staff       (20)     4706 2022-10-10 07:39:18.000000 pybiotk-1.1.1/rscripts/diff_expr_DESeq2.R
--rwxr-xr-x   0 mac        (501) staff       (20)     5704 2022-10-10 07:39:18.000000 pybiotk-1.1.1/rscripts/diff_expr_edgeR.R
--rwxr-xr-x   0 mac        (501) staff       (20)     9915 2022-10-10 07:39:18.000000 pybiotk-1.1.1/rscripts/diff_expr_plot.R
--rwxr-xr-x   0 mac        (501) staff       (20)     3017 2022-10-10 07:39:18.000000 pybiotk-1.1.1/rscripts/peak_anno.R
--rwxr-xr-x   0 mac        (501) staff       (20)     3112 2022-10-10 07:39:18.000000 pybiotk-1.1.1/rscripts/plot_FRiPs.R
--rwxr-xr-x   0 mac        (501) staff       (20)     2517 2022-10-10 07:39:18.000000 pybiotk-1.1.1/rscripts/plot_bar.R
--rwxr-xr-x   0 mac        (501) staff       (20)     3661 2022-10-10 07:39:18.000000 pybiotk-1.1.1/rscripts/plot_corr.R
--rwxr-xr-x   0 mac        (501) staff       (20)     3921 2022-10-10 07:39:18.000000 pybiotk-1.1.1/rscripts/plot_deeptools_fragmentsize.R
--rwxr-xr-x   0 mac        (501) staff       (20)     1918 2022-10-10 07:39:18.000000 pybiotk-1.1.1/rscripts/plot_hist.R
--rwxr-xr-x   0 mac        (501) staff       (20)     4114 2022-10-10 07:39:18.000000 pybiotk-1.1.1/rscripts/plot_peak_width.R
--rwxr-xr-x   0 mac        (501) staff       (20)     3078 2022-12-07 02:51:18.000000 pybiotk-1.1.1/rscripts/plot_rep_cor.R
--rwxr-xr-x   0 mac        (501) staff       (20)     8523 2022-10-10 07:39:18.000000 pybiotk-1.1.1/rscripts/plot_summary.R
--rwxr-xr-x   0 mac        (501) staff       (20)     2079 2022-10-10 07:39:18.000000 pybiotk-1.1.1/rscripts/plot_venn.R
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-01-31 08:23:13.885862 pybiotk-1.1.1/scripts/
--rwxr-xr-x   0 mac        (501) staff       (20)      196 2022-10-10 07:39:18.000000 pybiotk-1.1.1/scripts/fasta_len.sh
--rwxr-xr-x   0 mac        (501) staff       (20)      147 2022-10-10 07:39:18.000000 pybiotk-1.1.1/scripts/fasta_u2t.sh
--rwxr-xr-x   0 mac        (501) staff       (20)      206 2022-10-10 07:39:18.000000 pybiotk-1.1.1/scripts/fastq_len.sh
--rwxr-xr-x   0 mac        (501) staff       (20)      165 2022-10-10 07:39:18.000000 pybiotk-1.1.1/scripts/get_chrom_length.sh
--rwxr-xr-x   0 mac        (501) staff       (20)     1010 2022-10-10 07:39:18.000000 pybiotk-1.1.1/scripts/gtfparser.sh
--rwxr-xr-x   0 mac        (501) staff       (20)      555 2022-10-10 07:39:18.000000 pybiotk-1.1.1/scripts/merge_subseq.sh
--rwxr-xr-x   0 mac        (501) staff       (20)     1296 2022-10-10 07:39:18.000000 pybiotk-1.1.1/scripts/remove_duplicates.sh
--rw-r--r--   0 mac        (501) staff       (20)     2307 2023-01-31 08:23:13.916190 pybiotk-1.1.1/setup.cfg
--rw-r--r--   0 mac        (501) staff       (20)     1222 2022-10-10 07:39:18.000000 pybiotk-1.1.1/setup.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-01-31 08:23:13.870370 pybiotk-1.1.1/src/
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-01-31 08:23:13.889824 pybiotk-1.1.1/src/bx/
--rw-r--r--   0 mac        (501) staff       (20)     7429 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/bx/binBits.c
--rw-r--r--   0 mac        (501) staff       (20)      830 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/bx/binBits.h
--rw-r--r--   0 mac        (501) staff       (20)     6253 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/bx/bits.c
--rw-r--r--   0 mac        (501) staff       (20)     1814 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/bx/bits.h
--rw-r--r--   0 mac        (501) staff       (20)     9273 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/bx/bitset.pyx
--rw-r--r--   0 mac        (501) staff       (20)     8110 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/bx/cluster.c
--rw-r--r--   0 mac        (501) staff       (20)      905 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/bx/cluster.h
--rw-r--r--   0 mac        (501) staff       (20)     3795 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/bx/cluster.pyx
--rw-r--r--   0 mac        (501) staff       (20)     1508 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/bx/common.c
--rw-r--r--   0 mac        (501) staff       (20)      639 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/bx/common.h
--rw-r--r--   0 mac        (501) staff       (20)    17210 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/bx/intersection.pyx
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-01-31 08:23:13.890230 pybiotk-1.1.1/src/pybiotk/
--rw-r--r--   0 mac        (501) staff       (20)        0 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/__init__.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-01-31 08:23:13.894453 pybiotk-1.1.1/src/pybiotk/annodb/
--rw-r--r--   0 mac        (501) staff       (20)       99 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/annodb/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     7267 2022-10-26 08:53:54.000000 pybiotk-1.1.1/src/pybiotk/annodb/anno.py
--rw-r--r--   0 mac        (501) staff       (20)     8702 2022-10-25 09:28:50.000000 pybiotk-1.1.1/src/pybiotk/annodb/gene.py
--rw-r--r--   0 mac        (501) staff       (20)     8634 2023-01-30 02:09:44.000000 pybiotk-1.1.1/src/pybiotk/annodb/merged_transcript.py
--rw-r--r--   0 mac        (501) staff       (20)     6068 2022-10-25 09:28:14.000000 pybiotk-1.1.1/src/pybiotk/annodb/transcript.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-01-31 08:23:13.896413 pybiotk-1.1.1/src/pybiotk/convert/
--rw-r--r--   0 mac        (501) staff       (20)        0 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/convert/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     3813 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/convert/bam2fastx.py
--rw-r--r--   0 mac        (501) staff       (20)     1149 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/convert/bampe_order_by_name.py
--rw-r--r--   0 mac        (501) staff       (20)     1697 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/convert/bed2bedgraph.py
--rw-r--r--   0 mac        (501) staff       (20)      709 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/convert/fq2fasta.py
--rw-r--r--   0 mac        (501) staff       (20)     4691 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/convert/gtf2bed.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-01-31 08:23:13.897699 pybiotk-1.1.1/src/pybiotk/data/
--rw-r--r--   0 mac        (501) staff       (20)        0 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/data/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    11177 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/data/hg38.chrom.sizes
--rw-r--r--   0 mac        (501) staff       (20)     2410 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/data/mm10.chrom.sizes
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-01-31 08:23:13.899159 pybiotk-1.1.1/src/pybiotk/intervals/
--rw-r--r--   0 mac        (501) staff       (20)       79 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/intervals/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     4555 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/intervals/grange.py
--rw-r--r--   0 mac        (501) staff       (20)     2441 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/intervals/merge_bed3.py
--rw-r--r--   0 mac        (501) staff       (20)     2642 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/intervals/merge_intervals.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-01-31 08:23:13.901435 pybiotk-1.1.1/src/pybiotk/io/
--rw-r--r--   0 mac        (501) staff       (20)      117 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/io/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    10840 2022-10-10 08:44:51.000000 pybiotk-1.1.1/src/pybiotk/io/bam.py
--rw-r--r--   0 mac        (501) staff       (20)     6230 2022-11-10 02:56:39.000000 pybiotk-1.1.1/src/pybiotk/io/bed.py
--rw-r--r--   0 mac        (501) staff       (20)     7710 2023-01-31 08:04:35.000000 pybiotk-1.1.1/src/pybiotk/io/bw.py
--rw-r--r--   0 mac        (501) staff       (20)     4157 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/io/fasta.py
--rw-r--r--   0 mac        (501) staff       (20)     4346 2022-11-10 02:54:51.000000 pybiotk-1.1.1/src/pybiotk/io/fastq.py
--rw-r--r--   0 mac        (501) staff       (20)    18739 2022-11-09 02:25:42.000000 pybiotk-1.1.1/src/pybiotk/io/gtf.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-01-31 08:23:13.913048 pybiotk-1.1.1/src/pybiotk/utils/
--rw-r--r--   0 mac        (501) staff       (20)       21 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/utils/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)     2525 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/utils/bam_random.py
--rw-r--r--   0 mac        (501) staff       (20)     1022 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/utils/fasta_filter.py
--rw-r--r--   0 mac        (501) staff       (20)     5292 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/utils/fastq_join.py
--rw-r--r--   0 mac        (501) staff       (20)     3985 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/utils/fastq_uniq.py
--rw-r--r--   0 mac        (501) staff       (20)     1708 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/utils/fastx_rename.py
--rw-r--r--   0 mac        (501) staff       (20)     4182 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/utils/fragment_size.py
--rw-r--r--   0 mac        (501) staff       (20)     9984 2022-10-28 08:48:24.000000 pybiotk-1.1.1/src/pybiotk/utils/genomefetcher.py
--rw-r--r--   0 mac        (501) staff       (20)     2936 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/utils/gtf_filter.py
--rw-r--r--   0 mac        (501) staff       (20)     5831 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/utils/merge_row.py
--rw-r--r--   0 mac        (501) staff       (20)     2391 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/utils/merge_subseq.py
--rw-r--r--   0 mac        (501) staff       (20)     3692 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/utils/normalize.py
--rw-r--r--   0 mac        (501) staff       (20)     9623 2022-10-27 09:15:53.000000 pybiotk-1.1.1/src/pybiotk/utils/pyanno.py
--rw-r--r--   0 mac        (501) staff       (20)     3121 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/utils/read_tables.py
--rw-r--r--   0 mac        (501) staff       (20)     2234 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/utils/reference_count.py
--rw-r--r--   0 mac        (501) staff       (20)     1620 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/utils/reverse_fastx.py
--rw-r--r--   0 mac        (501) staff       (20)     3003 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/utils/rmats_filter.py
--rw-r--r--   0 mac        (501) staff       (20)     2778 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/utils/seq_random.py
--rw-r--r--   0 mac        (501) staff       (20)     4093 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/utils/subseq_analysis.py
--rw-r--r--   0 mac        (501) staff       (20)     8457 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/utils/summary_log.py
--rw-r--r--   0 mac        (501) staff       (20)     8311 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/pybiotk/utils/utils.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-01-31 08:23:13.892652 pybiotk-1.1.1/src/pybiotk.egg-info/
--rw-r--r--   0 mac        (501) staff       (20)     3780 2023-01-31 08:23:13.000000 pybiotk-1.1.1/src/pybiotk.egg-info/PKG-INFO
--rw-r--r--   0 mac        (501) staff       (20)     2866 2023-01-31 08:23:13.000000 pybiotk-1.1.1/src/pybiotk.egg-info/SOURCES.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2023-01-31 08:23:13.000000 pybiotk-1.1.1/src/pybiotk.egg-info/dependency_links.txt
--rw-r--r--   0 mac        (501) staff       (20)     1058 2023-01-31 08:23:13.000000 pybiotk-1.1.1/src/pybiotk.egg-info/entry_points.txt
--rw-r--r--   0 mac        (501) staff       (20)        1 2022-10-11 06:43:47.000000 pybiotk-1.1.1/src/pybiotk.egg-info/not-zip-safe
--rw-r--r--   0 mac        (501) staff       (20)       88 2023-01-31 08:23:13.000000 pybiotk-1.1.1/src/pybiotk.egg-info/requires.txt
--rw-r--r--   0 mac        (501) staff       (20)       15 2023-01-31 08:23:13.000000 pybiotk-1.1.1/src/pybiotk.egg-info/top_level.txt
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-01-31 08:23:13.913939 pybiotk-1.1.1/src/stream/
--rw-r--r--   0 mac        (501) staff       (20)       42 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/stream/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)    10613 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/stream/pipe.py
--rw-r--r--   0 mac        (501) staff       (20)     7886 2022-10-10 07:39:18.000000 pybiotk-1.1.1/src/stream/stream.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-01-31 08:23:13.914456 pybiotk-1.1.1/tests/
--rw-r--r--   0 mac        (501) staff       (20)        0 2022-10-10 07:39:18.000000 pybiotk-1.1.1/tests/__init__.py
--rw-r--r--   0 mac        (501) staff       (20)      132 2022-10-10 07:39:18.000000 pybiotk-1.1.1/tests/conftest.py
-drwxr-xr-x   0 mac        (501) staff       (20)        0 2023-01-31 08:23:13.914735 pybiotk-1.1.1/tests/test_stream/
--rw-r--r--   0 mac        (501) staff       (20)      195 2022-10-10 07:39:18.000000 pybiotk-1.1.1/tests/test_stream/test_pipe.py
--rw-r--r--   0 mac        (501) staff       (20)     2575 2022-10-10 07:39:18.000000 pybiotk-1.1.1/tox.ini
+drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:39.000000 pybiotk-1.2.0/
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      590 2022-07-04 07:56:59.000000 pybiotk-1.2.0/.coveragerc
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      583 2022-07-07 06:33:07.000000 pybiotk-1.2.0/.gitignore
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      490 2022-07-04 07:56:59.000000 pybiotk-1.2.0/.readthedocs.yml
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       77 2022-07-04 07:56:59.000000 pybiotk-1.2.0/AUTHORS.rst
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      128 2022-07-04 07:56:59.000000 pybiotk-1.2.0/CHANGELOG.rst
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    13815 2022-07-04 07:56:59.000000 pybiotk-1.2.0/CONTRIBUTING.rst
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1079 2022-07-04 07:56:59.000000 pybiotk-1.2.0/LICENSE.txt
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3351 2023-06-19 02:25:39.000000 pybiotk-1.2.0/PKG-INFO
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2932 2023-05-15 09:36:22.000000 pybiotk-1.2.0/README.md
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     4004 2023-05-15 09:36:22.000000 pybiotk-1.2.0/README.rst
+drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:38.000000 pybiotk-1.2.0/docs/
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1154 2022-07-04 07:56:59.000000 pybiotk-1.2.0/docs/Makefile
+drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:38.000000 pybiotk-1.2.0/docs/_static/
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       18 2022-07-04 07:57:00.000000 pybiotk-1.2.0/docs/_static/.gitignore
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       41 2022-07-04 07:57:00.000000 pybiotk-1.2.0/docs/authors.rst
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       43 2022-07-04 07:57:00.000000 pybiotk-1.2.0/docs/changelog.rst
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     9734 2022-07-04 07:57:00.000000 pybiotk-1.2.0/docs/conf.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       33 2022-07-04 07:57:00.000000 pybiotk-1.2.0/docs/contributing.rst
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2313 2022-07-04 07:57:00.000000 pybiotk-1.2.0/docs/index.rst
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       67 2022-07-04 07:57:00.000000 pybiotk-1.2.0/docs/license.rst
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       39 2022-07-04 07:57:00.000000 pybiotk-1.2.0/docs/readme.rst
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      122 2022-08-02 09:43:12.000000 pybiotk-1.2.0/docs/requirements.txt
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      408 2022-07-19 02:24:18.000000 pybiotk-1.2.0/pyproject.toml
+drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:38.000000 pybiotk-1.2.0/rscripts/
+-rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     7058 2023-06-08 09:57:01.000000 pybiotk-1.2.0/rscripts/diff_expr_DESeq2.R
+-rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     5704 2023-04-02 13:07:58.000000 pybiotk-1.2.0/rscripts/diff_expr_edgeR.R
+-rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)    16758 2023-06-08 09:57:01.000000 pybiotk-1.2.0/rscripts/diff_expr_plot.R
+-rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     3017 2022-07-04 07:57:00.000000 pybiotk-1.2.0/rscripts/peak_anno.R
+-rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     3112 2022-07-04 07:57:00.000000 pybiotk-1.2.0/rscripts/plot_FRiPs.R
+-rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     2517 2022-07-04 07:57:00.000000 pybiotk-1.2.0/rscripts/plot_bar.R
+-rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     8523 2023-04-02 13:09:25.000000 pybiotk-1.2.0/rscripts/plot_chip_summary.R
+-rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     3661 2022-07-04 07:57:00.000000 pybiotk-1.2.0/rscripts/plot_corr.R
+-rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     3921 2022-07-04 07:57:00.000000 pybiotk-1.2.0/rscripts/plot_deeptools_fragmentsize.R
+-rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     1918 2022-07-04 07:57:00.000000 pybiotk-1.2.0/rscripts/plot_hist.R
+-rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     4114 2022-07-04 07:57:00.000000 pybiotk-1.2.0/rscripts/plot_peak_width.R
+-rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     3086 2023-04-14 12:58:41.000000 pybiotk-1.2.0/rscripts/plot_rep_cor.R
+-rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     2079 2022-07-04 07:57:00.000000 pybiotk-1.2.0/rscripts/plot_venn.R
+drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:38.000000 pybiotk-1.2.0/scripts/
+-rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)      196 2022-07-04 07:57:00.000000 pybiotk-1.2.0/scripts/fasta_len.sh
+-rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)      147 2022-07-04 07:57:00.000000 pybiotk-1.2.0/scripts/fasta_u2t.sh
+-rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)      206 2022-07-04 07:57:00.000000 pybiotk-1.2.0/scripts/fastq_len.sh
+-rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)      165 2022-07-04 07:57:00.000000 pybiotk-1.2.0/scripts/get_chrom_length.sh
+-rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     1010 2022-07-04 07:57:00.000000 pybiotk-1.2.0/scripts/gtfparser.sh
+-rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)      555 2022-07-04 07:57:00.000000 pybiotk-1.2.0/scripts/merge_subseq.sh
+-rwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)     1296 2022-07-04 07:57:00.000000 pybiotk-1.2.0/scripts/remove_duplicates.sh
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2358 2023-06-19 02:22:37.000000 pybiotk-1.2.0/setup.cfg
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1222 2022-07-19 09:16:34.000000 pybiotk-1.2.0/setup.py
+drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:37.000000 pybiotk-1.2.0/src/
+drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:38.000000 pybiotk-1.2.0/src/bx/
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     7429 2022-07-07 06:33:07.000000 pybiotk-1.2.0/src/bx/binBits.c
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      830 2022-07-07 06:33:07.000000 pybiotk-1.2.0/src/bx/binBits.h
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     6253 2022-07-19 09:16:34.000000 pybiotk-1.2.0/src/bx/bits.c
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1814 2022-07-07 06:33:07.000000 pybiotk-1.2.0/src/bx/bits.h
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     9273 2022-07-19 09:16:34.000000 pybiotk-1.2.0/src/bx/bitset.pyx
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     8110 2022-07-07 06:33:07.000000 pybiotk-1.2.0/src/bx/cluster.c
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      905 2022-07-07 06:33:07.000000 pybiotk-1.2.0/src/bx/cluster.h
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3795 2022-07-19 09:16:34.000000 pybiotk-1.2.0/src/bx/cluster.pyx
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1508 2022-07-07 06:33:07.000000 pybiotk-1.2.0/src/bx/common.c
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      639 2022-07-07 06:33:07.000000 pybiotk-1.2.0/src/bx/common.h
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    17210 2022-07-19 09:16:34.000000 pybiotk-1.2.0/src/bx/intersection.pyx
+drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:38.000000 pybiotk-1.2.0/src/pybiotk/
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)        0 2022-07-04 07:57:01.000000 pybiotk-1.2.0/src/pybiotk/__init__.py
+drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:38.000000 pybiotk-1.2.0/src/pybiotk/annodb/
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       99 2022-08-02 07:19:20.000000 pybiotk-1.2.0/src/pybiotk/annodb/__init__.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     7267 2022-10-26 08:57:07.000000 pybiotk-1.2.0/src/pybiotk/annodb/anno.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     8702 2022-10-25 09:30:11.000000 pybiotk-1.2.0/src/pybiotk/annodb/gene.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     8634 2023-01-30 02:31:13.000000 pybiotk-1.2.0/src/pybiotk/annodb/merged_transcript.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     6068 2022-10-25 09:30:11.000000 pybiotk-1.2.0/src/pybiotk/annodb/transcript.py
+drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:38.000000 pybiotk-1.2.0/src/pybiotk/convert/
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)        0 2022-07-04 07:57:02.000000 pybiotk-1.2.0/src/pybiotk/convert/__init__.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3813 2022-09-06 07:47:21.000000 pybiotk-1.2.0/src/pybiotk/convert/bam2fastx.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1149 2022-08-02 07:19:20.000000 pybiotk-1.2.0/src/pybiotk/convert/bampe_order_by_name.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1697 2022-08-02 07:19:20.000000 pybiotk-1.2.0/src/pybiotk/convert/bed2bedgraph.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      709 2022-10-04 08:52:33.000000 pybiotk-1.2.0/src/pybiotk/convert/fq2fasta.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     4691 2022-10-04 08:52:33.000000 pybiotk-1.2.0/src/pybiotk/convert/gtf2bed.py
+drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:38.000000 pybiotk-1.2.0/src/pybiotk/data/
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)        0 2022-07-04 07:57:02.000000 pybiotk-1.2.0/src/pybiotk/data/__init__.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    11177 2022-07-04 07:57:02.000000 pybiotk-1.2.0/src/pybiotk/data/hg38.chrom.sizes
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2410 2022-07-04 07:57:02.000000 pybiotk-1.2.0/src/pybiotk/data/mm10.chrom.sizes
+drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:38.000000 pybiotk-1.2.0/src/pybiotk/intervals/
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       79 2022-08-02 07:19:20.000000 pybiotk-1.2.0/src/pybiotk/intervals/__init__.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     4555 2022-08-02 07:19:20.000000 pybiotk-1.2.0/src/pybiotk/intervals/grange.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2441 2022-08-02 07:19:20.000000 pybiotk-1.2.0/src/pybiotk/intervals/merge_bed3.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2642 2022-08-02 07:19:20.000000 pybiotk-1.2.0/src/pybiotk/intervals/merge_intervals.py
+drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:38.000000 pybiotk-1.2.0/src/pybiotk/io/
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      451 2023-04-26 11:55:13.000000 pybiotk-1.2.0/src/pybiotk/io/__init__.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    10840 2022-10-10 08:54:31.000000 pybiotk-1.2.0/src/pybiotk/io/bam.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     6230 2022-09-26 13:01:34.000000 pybiotk-1.2.0/src/pybiotk/io/bed.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     7710 2023-02-01 07:48:01.000000 pybiotk-1.2.0/src/pybiotk/io/bw.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     4575 2023-04-26 12:15:18.000000 pybiotk-1.2.0/src/pybiotk/io/fasta.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     4346 2022-09-14 15:02:58.000000 pybiotk-1.2.0/src/pybiotk/io/fastq.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    19645 2023-05-15 09:36:23.000000 pybiotk-1.2.0/src/pybiotk/io/gtf.py
+drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:39.000000 pybiotk-1.2.0/src/pybiotk/string/
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       44 2023-06-08 09:57:01.000000 pybiotk-1.2.0/src/pybiotk/string/__init__.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      946 2023-06-08 09:57:01.000000 pybiotk-1.2.0/src/pybiotk/string/motif.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      714 2023-06-08 09:57:01.000000 pybiotk-1.2.0/src/pybiotk/string/sequence.py
+drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:39.000000 pybiotk-1.2.0/src/pybiotk/utils/
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       21 2022-07-04 07:57:03.000000 pybiotk-1.2.0/src/pybiotk/utils/__init__.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2525 2022-10-04 08:52:33.000000 pybiotk-1.2.0/src/pybiotk/utils/bam_random.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1230 2023-04-26 11:55:13.000000 pybiotk-1.2.0/src/pybiotk/utils/fasta_filter.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     5292 2022-09-14 15:02:58.000000 pybiotk-1.2.0/src/pybiotk/utils/fastq_join.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3985 2022-10-04 08:52:33.000000 pybiotk-1.2.0/src/pybiotk/utils/fastq_uniq.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1708 2022-10-04 08:52:33.000000 pybiotk-1.2.0/src/pybiotk/utils/fastx_rename.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     4182 2022-08-02 09:43:12.000000 pybiotk-1.2.0/src/pybiotk/utils/fragment_size.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     9967 2023-06-08 09:57:01.000000 pybiotk-1.2.0/src/pybiotk/utils/genomefetcher.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2936 2022-10-04 08:52:33.000000 pybiotk-1.2.0/src/pybiotk/utils/gtf_filter.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     5805 2023-04-02 13:09:25.000000 pybiotk-1.2.0/src/pybiotk/utils/merge_row.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2391 2022-08-02 07:19:20.000000 pybiotk-1.2.0/src/pybiotk/utils/merge_subseq.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3664 2023-06-08 09:57:01.000000 pybiotk-1.2.0/src/pybiotk/utils/normalize.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    10682 2023-04-26 11:55:14.000000 pybiotk-1.2.0/src/pybiotk/utils/pyanno.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3284 2023-06-08 09:57:01.000000 pybiotk-1.2.0/src/pybiotk/utils/read_tables.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2234 2022-08-02 07:19:20.000000 pybiotk-1.2.0/src/pybiotk/utils/reference_count.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1620 2022-10-04 08:52:33.000000 pybiotk-1.2.0/src/pybiotk/utils/reverse_fastx.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3114 2023-05-15 09:36:23.000000 pybiotk-1.2.0/src/pybiotk/utils/rmats_filter.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2778 2022-10-04 08:52:33.000000 pybiotk-1.2.0/src/pybiotk/utils/seq_random.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     4093 2022-09-06 07:47:21.000000 pybiotk-1.2.0/src/pybiotk/utils/subseq_analysis.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    14283 2023-04-02 13:09:25.000000 pybiotk-1.2.0/src/pybiotk/utils/summary_log.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     9118 2023-06-08 10:23:58.000000 pybiotk-1.2.0/src/pybiotk/utils/utils.py
+drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:38.000000 pybiotk-1.2.0/src/pybiotk.egg-info/
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     3351 2023-06-19 02:22:35.000000 pybiotk-1.2.0/src/pybiotk.egg-info/PKG-INFO
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2961 2023-06-19 02:22:35.000000 pybiotk-1.2.0/src/pybiotk.egg-info/SOURCES.txt
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)        1 2023-06-19 02:22:35.000000 pybiotk-1.2.0/src/pybiotk.egg-info/dependency_links.txt
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     1102 2023-06-19 02:22:35.000000 pybiotk-1.2.0/src/pybiotk.egg-info/entry_points.txt
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)        1 2022-07-04 07:59:58.000000 pybiotk-1.2.0/src/pybiotk.egg-info/not-zip-safe
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       93 2023-06-19 02:22:35.000000 pybiotk-1.2.0/src/pybiotk.egg-info/requires.txt
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       15 2023-06-19 02:22:35.000000 pybiotk-1.2.0/src/pybiotk.egg-info/top_level.txt
+drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:39.000000 pybiotk-1.2.0/src/stream/
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)       20 2023-06-08 09:57:01.000000 pybiotk-1.2.0/src/stream/__init__.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)    10873 2023-06-08 10:05:34.000000 pybiotk-1.2.0/src/stream/pipe.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     7886 2022-09-14 14:59:43.000000 pybiotk-1.2.0/src/stream/stream.py
+drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:39.000000 pybiotk-1.2.0/tests/
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)        0 2022-07-04 07:57:03.000000 pybiotk-1.2.0/tests/__init__.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      132 2022-07-04 07:57:03.000000 pybiotk-1.2.0/tests/conftest.py
+drwxr-xr-x   0 liqiming  (1036) zhoulab   (1003)        0 2023-06-19 02:25:39.000000 pybiotk-1.2.0/tests/test_stream/
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)      195 2022-07-04 07:57:03.000000 pybiotk-1.2.0/tests/test_stream/test_pipe.py
+-rw-r--r--   0 liqiming  (1036) zhoulab   (1003)     2575 2022-07-04 07:57:03.000000 pybiotk-1.2.0/tox.ini
```

### Comparing `pybiotk-1.1.1/.coveragerc` & `pybiotk-1.2.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/.gitignore` & `pybiotk-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/CONTRIBUTING.rst` & `pybiotk-1.2.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/LICENSE.txt` & `pybiotk-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/PKG-INFO` & `pybiotk-1.2.0/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pybiotk
-Version: 1.1.1
+Version: 1.2.0
 Summary: pybiotk: A python toolkit for bioinformatics analysis.
 Home-page: https://github.com/liqiming-whu/pybiotk
 Author: liqiming_whu
 Author-email: liqiming@whu.edu.cn
 License: MIT
 Project-URL: Documentation, https://github.com/liqiming-whu/pybiotk
 Platform: any
@@ -14,42 +14,28 @@
 Provides-Extra: testing
 License-File: LICENSE.txt
 
 # pybiotk: A python toolkit for bioinformatics analysis
 
 ## Install
 
-> **SetuptoolsDeprecationWarning: setup.py install is deprecated. Use build and pip and other standards-based tools.**
-
 ### use PyPi(official)
 
 ```
 pip install pybiotk
 ```
 
 **An older version may be installed**
 
-### use build frontend([build: A simple, correct PEP 517 build frontend.](https://pypi.org/project/build/))
-
-```
-git clone https://gitee.com/liqiming_whu/pybiotk.git
-cd pybiotk
-pip install build
-python -m build
-pip install dist/*tar.gz
-```
-
-### use setup.py sdist
+### or
 
 ```
 git clone https://gitee.com/liqiming_whu/pybiotk.git
 cd pybiotk
-pip install cython
-python setup.py sdist
-pip install dist/*tar.gz
+pip install .
 ```
 
 ## Modules
 
 ```
 console_scripts =
     gtf2bed = pybiotk.convert.gtf2bed:run
```

### Comparing `pybiotk-1.1.1/README.md` & `pybiotk-1.2.0/src/pybiotk.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,88 +1,90 @@
-# pybiotk: A python toolkit for bioinformatics analysis
-
-## Install
-
-> **SetuptoolsDeprecationWarning: setup.py install is deprecated. Use build and pip and other standards-based tools.**
-
-### use PyPi(official)
-
-```
-pip install pybiotk
-```
-
-**An older version may be installed**
-
-### use build frontend([build: A simple, correct PEP 517 build frontend.](https://pypi.org/project/build/))
-
-```
-git clone https://gitee.com/liqiming_whu/pybiotk.git
-cd pybiotk
-pip install build
-python -m build
-pip install dist/*tar.gz
-```
-
-### use setup.py sdist
-
-```
-git clone https://gitee.com/liqiming_whu/pybiotk.git
-cd pybiotk
-pip install cython
-python setup.py sdist
-pip install dist/*tar.gz
-```
-
-## Modules
-
-```
-console_scripts =
-    gtf2bed = pybiotk.convert.gtf2bed:run
-    bed2bedgraph = pybiotk.convert.bed2bedgraph:run
-    fq2fasta = pybiotk.convert.fq2fasta:run
-    bam2fastx = pybiotk.convert.bam2fastx:run
-    bampe_order_by_name = pybiotk.convert.bampe_order_by_name:run
-    bam_random = pybiotk.utils.bam_random:run
-    gtf_filter = pybiotk.utils.gtf_filter:run
-    fasta_filter = pybiotk.utils.fasta_filter:run
-    fastq_uniq = pybiotk.utils.fastq_uniq:run
-    fastq_join = pybiotk.utils.fastq_join:run
-    fastx_rename = pybiotk.utils.fastx_rename:run
-    genomefetcher = pybiotk.utils.genomefetcher:run
-    reverse_fastx = pybiotk.utils.reverse_fastx:run
-    seq_random = pybiotk.utils.seq_random:run
-    merge_row = pybiotk.utils.merge_row:run
-    read_tables = pybiotk.utils.read_tables:run
-    rmats_filter = pybiotk.utils.rmats_filter:run
-    count_normalize = pybiotk.utils.normalize:run
-    reference_count = pybiotk.utils.reference_count:run
-    pyanno = pybiotk.utils.pyanno:run
-    rna_fragment_size = pybiotk.utils.fragment_size:run
-    merge_subseq = pybiotk.utils.merge_subseq:run
-    subseq_analysis = pybiotk.utils.subseq_analysis:run
-```
-
-## Usage
-
-```
-usage: pyanno [-h] -i INPUT -o OUTPUT -g GTF [-l {transcript,gene}] [--tss_region TSS_REGION [TSS_REGION ...]] [--downstream DOWNSTREAM] [-s]
-              [--rule {1+-,1-+,2++,2--,1++,1--,2+-,2-+,+-,-+,++,--}] [-p] [--ordered_by_name]
-
-optional arguments:
-  -h, --help            show this help message and exit
-  -i INPUT, --input INPUT
-                        input file, bam or bed. The file type will be inferred from the filename suffix ['*.bam', '*.bed']. (default: None)
-  -o OUTPUT, --output OUTPUT
-                        output file name. (default: None)
-  -g GTF, --gtf GTF     gtf file download from Genecode, or a sorted gtf file. (default: None)
-  -l {transcript,gene}, --level {transcript,gene}
-                        annotation level, transcript or gene. (default: transcript)
-  --tss_region TSS_REGION [TSS_REGION ...]
-                        choose region from tss. (default: [-1000, 1000])
-  --downstream DOWNSTREAM
-                        downstream length from tes. (default: 3000)
-  -s, --strand          require same strandedness. (default: False)
-  --rule {1+-,1-+,2++,2--,1++,1--,2+-,2-+,+-,-+,++,--}
-                        how read(s) were stranded during sequencing. only for bam. (default: 1+-,1-+,2++,2--)
-  -p, --pair            annotate fragments instead of reads. (default: False)
-  --ordered_by_name     if input bam is ordered by name, only for pair-end bam. (default: False)
-```
+Metadata-Version: 2.1
+Name: pybiotk
+Version: 1.2.0
+Summary: pybiotk: A python toolkit for bioinformatics analysis.
+Home-page: https://github.com/liqiming-whu/pybiotk
+Author: liqiming_whu
+Author-email: liqiming@whu.edu.cn
+License: MIT
+Project-URL: Documentation, https://github.com/liqiming-whu/pybiotk
+Platform: any
+Classifier: Development Status :: 4 - Beta
+Classifier: Programming Language :: Python
+Description-Content-Type: text/markdown
+Provides-Extra: testing
+License-File: LICENSE.txt
+
+# pybiotk: A python toolkit for bioinformatics analysis
+
+## Install
+
+### use PyPi(official)
+
+```
+pip install pybiotk
+```
+
+**An older version may be installed**
+
+### or
+
+```
+git clone https://gitee.com/liqiming_whu/pybiotk.git
+cd pybiotk
+pip install .
+```
+
+## Modules
+
+```
+console_scripts =
+    gtf2bed = pybiotk.convert.gtf2bed:run
+    bed2bedgraph = pybiotk.convert.bed2bedgraph:run
+    fq2fasta = pybiotk.convert.fq2fasta:run
+    bam2fastx = pybiotk.convert.bam2fastx:run
+    bampe_order_by_name = pybiotk.convert.bampe_order_by_name:run
+    bam_random = pybiotk.utils.bam_random:run
+    gtf_filter = pybiotk.utils.gtf_filter:run
+    fasta_filter = pybiotk.utils.fasta_filter:run
+    fastq_uniq = pybiotk.utils.fastq_uniq:run
+    fastq_join = pybiotk.utils.fastq_join:run
+    fastx_rename = pybiotk.utils.fastx_rename:run
+    genomefetcher = pybiotk.utils.genomefetcher:run
+    reverse_fastx = pybiotk.utils.reverse_fastx:run
+    seq_random = pybiotk.utils.seq_random:run
+    merge_row = pybiotk.utils.merge_row:run
+    read_tables = pybiotk.utils.read_tables:run
+    rmats_filter = pybiotk.utils.rmats_filter:run
+    count_normalize = pybiotk.utils.normalize:run
+    reference_count = pybiotk.utils.reference_count:run
+    pyanno = pybiotk.utils.pyanno:run
+    rna_fragment_size = pybiotk.utils.fragment_size:run
+    merge_subseq = pybiotk.utils.merge_subseq:run
+    subseq_analysis = pybiotk.utils.subseq_analysis:run
+```
+
+## Usage
+
+```
+usage: pyanno [-h] -i INPUT -o OUTPUT -g GTF [-l {transcript,gene}] [--tss_region TSS_REGION [TSS_REGION ...]] [--downstream DOWNSTREAM] [-s]
+              [--rule {1+-,1-+,2++,2--,1++,1--,2+-,2-+,+-,-+,++,--}] [-p] [--ordered_by_name]
+
+optional arguments:
+  -h, --help            show this help message and exit
+  -i INPUT, --input INPUT
+                        input file, bam or bed. The file type will be inferred from the filename suffix ['*.bam', '*.bed']. (default: None)
+  -o OUTPUT, --output OUTPUT
+                        output file name. (default: None)
+  -g GTF, --gtf GTF     gtf file download from Genecode, or a sorted gtf file. (default: None)
+  -l {transcript,gene}, --level {transcript,gene}
+                        annotation level, transcript or gene. (default: transcript)
+  --tss_region TSS_REGION [TSS_REGION ...]
+                        choose region from tss. (default: [-1000, 1000])
+  --downstream DOWNSTREAM
+                        downstream length from tes. (default: 3000)
+  -s, --strand          require same strandedness. (default: False)
+  --rule {1+-,1-+,2++,2--,1++,1--,2+-,2-+,+-,-+,++,--}
+                        how read(s) were stranded during sequencing. only for bam. (default: 1+-,1-+,2++,2--)
+  -p, --pair            annotate fragments instead of reads. (default: False)
+  --ordered_by_name     if input bam is ordered by name, only for pair-end bam. (default: False)
+```
```

### Comparing `pybiotk-1.1.1/README.rst` & `pybiotk-1.2.0/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,17 @@
 
 pybiotk: A python toolkit for bioinformatics analysis
 
 
 Install
 ====
 
-python setup.py install
+git clone https://gitee.com/liqiming_whu/pybiotk.git
+cd pybiotk
+pip install .
 
 Modules
 ====
 
 gtf2bed = pybiotk.convert.gtf2bed:run
 
 bed2bedgraph = pybiotk.convert.bed2bedgraph:run
```

### Comparing `pybiotk-1.1.1/docs/Makefile` & `pybiotk-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/docs/conf.py` & `pybiotk-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/docs/index.rst` & `pybiotk-1.2.0/docs/index.rst`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/rscripts/diff_expr_edgeR.R` & `pybiotk-1.2.0/rscripts/diff_expr_edgeR.R`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
 # 1.直接依据选定的count值过滤
 # keep <- rowSums(dgelist$counts) >= 50
 
 # 2.CPM标准化
 # keep <- rowSums(cpm(dgelist)>1) >= 1
 
 # 3.自动过滤
-keep<- filterByExpr(deglist, group=group)
+keep<- filterByExpr(dgelist, group=group)
 
 dgelist <- dgelist[keep, , keep.lib.sizes=FALSE]
 
 if(!is.null(spike_in)) {
 
     spike_table <- read_data(spike_in[1], samples_name[1])
     for (idx in seq_along(spike_in)[-1]) {
```

### Comparing `pybiotk-1.1.1/rscripts/peak_anno.R` & `pybiotk-1.2.0/rscripts/peak_anno.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/rscripts/plot_FRiPs.R` & `pybiotk-1.2.0/rscripts/plot_FRiPs.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/rscripts/plot_bar.R` & `pybiotk-1.2.0/rscripts/plot_bar.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/rscripts/plot_corr.R` & `pybiotk-1.2.0/rscripts/plot_corr.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/rscripts/plot_deeptools_fragmentsize.R` & `pybiotk-1.2.0/rscripts/plot_deeptools_fragmentsize.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/rscripts/plot_hist.R` & `pybiotk-1.2.0/rscripts/plot_hist.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/rscripts/plot_peak_width.R` & `pybiotk-1.2.0/rscripts/plot_peak_width.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/rscripts/plot_rep_cor.R` & `pybiotk-1.2.0/rscripts/plot_rep_cor.R`

 * *Files 4% similar despite different names*

```diff
@@ -77,12 +77,12 @@
     geom_point(aes(x=log10(x), y=log10(y)), color="blue") +
     geom_text(aes(x=min(log10_x) + 0.1*(max(log10_x) - min(log10_x)), y=max(log10(y))), label=label, size = 2, check_overlap=T) +
     labs(x=paste0(samples_name[1]," log10(FPKM)"), y=paste0(samples_name[2], " log10(FPKM)")) +
     theme_bw() +
     theme(panel.grid=element_blank(), legend.position="none", text = element_text(size = 8))
 
 if(args$density) {
-    p <- p + stat_density2d(geom = 'polygon', aes(x=log10(x), y=log10(y), fill=..level..)) +
+    p <- p + stat_density2d(geom = 'polygon', aes(x=log10(x), y=log10(y), fill=after_stat(level))) +
         scale_fill_viridis(begin = 0.1, end = 0.9, option = "turbo", alpha = 0.8)
 }
 
 ggsave(args$outfig, p, width=5, height=5, dpi=300, units="cm")
```

### Comparing `pybiotk-1.1.1/rscripts/plot_summary.R` & `pybiotk-1.2.0/rscripts/plot_chip_summary.R`

 * *Files 1% similar despite different names*

```diff
@@ -101,15 +101,15 @@
   theme_bw(base_size = 12) +
   theme(panel.grid=element_blank()) +
   scale_fill_viridis(discrete = TRUE, begin = 0.15, end = 0.85, option = "turbo", alpha = 0.8) +
   # scale_color_viridis(discrete = TRUE, begin = 0.15, end = 0.85) +
   ggpubr::rotate_x_text(angle = 20) +
   ylab("% of Mapped Fragments") +
   xlab("") +
-  ggtitle("2C. Alignment Rate")
+  ggtitle("2C. Alignment rate")
 
 fig2 <- ggarrange(fig2A, fig2B, fig2C, ncol = 3, common.legend = TRUE, legend="bottom")
 
 
 dupdata <- data.frame("group"=data$group, "replicate"=data$replicates,
                       "duprate"=data$duplication_rate,
                       "uniquefragments"=data$mapped_read_pairs * (100 - as.numeric(sub("%", "", data$duplication_rate)))/100,
@@ -121,17 +121,17 @@
   geom_jitter(aes(color = replicate), position = position_jitter(0.15))+
   geom_text_repel(aes(label=duprate, x=group, y=as.numeric(sub("%", "", duprate))), color="black", segment.color="grey", size=2, direction='both') +
   theme_bw(base_size = 12) +
   theme(panel.grid=element_blank()) +
   scale_fill_viridis(discrete = TRUE, begin = 0.15, end = 0.85, option = "turbo", alpha = 0.8) +
   # scale_color_viridis(discrete = TRUE, begin = 0.15, end = 0.85) +
   ggpubr::rotate_x_text(angle = 20) +
-  ylab("Duplication Rate (*100%)") +
+  ylab("Duplication rate (*100%)") +
   xlab("") +
-  ggtitle("3A. Duplication Rate")
+  ggtitle("3A. Duplication rate")
 
 
 fig3B <- ggplot(dupdata, aes(x=group, y=uniquefragments/1000000, fill=group))+
   geom_boxplot() +
   geom_jitter(aes(color = replicate), position = position_jitter(0.15))+
   geom_text_repel(aes(label=round(uniquefragments), x=group, y=uniquefragments/1000000), color="black", segment.color="grey", size=2, direction='both') +
   theme_bw(base_size = 12) +
```

### Comparing `pybiotk-1.1.1/rscripts/plot_venn.R` & `pybiotk-1.2.0/rscripts/plot_venn.R`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/scripts/gtfparser.sh` & `pybiotk-1.2.0/scripts/gtfparser.sh`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/scripts/merge_subseq.sh` & `pybiotk-1.2.0/scripts/merge_subseq.sh`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/scripts/remove_duplicates.sh` & `pybiotk-1.2.0/scripts/remove_duplicates.sh`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/setup.cfg` & `pybiotk-1.2.0/setup.cfg`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = pybiotk
-version = 1.1.1
+version = 1.2.0
 description = pybiotk: A python toolkit for bioinformatics analysis.
 author = liqiming_whu
 author_email = liqiming@whu.edu.cn
 license = MIT
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown
@@ -25,14 +25,15 @@
 install_requires = 
 	openpyxl
 	pandas
 	pysam
 	pyBigWig
 	matplotlib
 	scipy
+	rich
 
 [options.packages.find]
 where = src
 exclude = 
 	bx
 	tests
 
@@ -63,14 +64,15 @@
 	rmats_filter = pybiotk.utils.rmats_filter:run
 	count_normalize = pybiotk.utils.normalize:run
 	reference_count = pybiotk.utils.reference_count:run
 	pyanno = pybiotk.utils.pyanno:run
 	rna_fragment_size = pybiotk.utils.fragment_size:run
 	merge_subseq = pybiotk.utils.merge_subseq:run
 	subseq_analysis = pybiotk.utils.subseq_analysis:run
+	summary_log = pybiotk.utils.summary_log:run
 
 [tool:pytest]
 addopts = 
 	--cov src --cov-report term-missing
 	--verbose
 norecursedirs = 
 	dist
```

### Comparing `pybiotk-1.1.1/setup.py` & `pybiotk-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/bx/binBits.c` & `pybiotk-1.2.0/src/bx/binBits.c`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/bx/binBits.h` & `pybiotk-1.2.0/src/bx/binBits.h`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/bx/bits.c` & `pybiotk-1.2.0/src/bx/bits.c`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/bx/bits.h` & `pybiotk-1.2.0/src/bx/bits.h`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/bx/bitset.pyx` & `pybiotk-1.2.0/src/bx/bitset.pyx`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/bx/cluster.c` & `pybiotk-1.2.0/src/bx/cluster.c`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/bx/cluster.h` & `pybiotk-1.2.0/src/bx/cluster.h`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/bx/cluster.pyx` & `pybiotk-1.2.0/src/bx/cluster.pyx`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/bx/common.c` & `pybiotk-1.2.0/src/bx/common.c`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/bx/common.h` & `pybiotk-1.2.0/src/bx/common.h`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/bx/intersection.pyx` & `pybiotk-1.2.0/src/bx/intersection.pyx`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/annodb/anno.py` & `pybiotk-1.2.0/src/pybiotk/annodb/anno.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/annodb/gene.py` & `pybiotk-1.2.0/src/pybiotk/annodb/gene.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/annodb/merged_transcript.py` & `pybiotk-1.2.0/src/pybiotk/annodb/merged_transcript.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/annodb/transcript.py` & `pybiotk-1.2.0/src/pybiotk/annodb/transcript.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/convert/bam2fastx.py` & `pybiotk-1.2.0/src/pybiotk/convert/bam2fastx.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/convert/bampe_order_by_name.py` & `pybiotk-1.2.0/src/pybiotk/convert/bampe_order_by_name.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/convert/bed2bedgraph.py` & `pybiotk-1.2.0/src/pybiotk/convert/bed2bedgraph.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/convert/fq2fasta.py` & `pybiotk-1.2.0/src/pybiotk/convert/fq2fasta.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/convert/gtf2bed.py` & `pybiotk-1.2.0/src/pybiotk/convert/gtf2bed.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/data/hg38.chrom.sizes` & `pybiotk-1.2.0/src/pybiotk/data/hg38.chrom.sizes`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/data/mm10.chrom.sizes` & `pybiotk-1.2.0/src/pybiotk/data/mm10.chrom.sizes`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/intervals/grange.py` & `pybiotk-1.2.0/src/pybiotk/intervals/grange.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/intervals/merge_bed3.py` & `pybiotk-1.2.0/src/pybiotk/intervals/merge_bed3.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/intervals/merge_intervals.py` & `pybiotk-1.2.0/src/pybiotk/intervals/merge_intervals.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/io/bam.py` & `pybiotk-1.2.0/src/pybiotk/io/bam.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/io/bed.py` & `pybiotk-1.2.0/src/pybiotk/io/bed.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/io/bw.py` & `pybiotk-1.2.0/src/pybiotk/io/bw.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/io/fasta.py` & `pybiotk-1.2.0/src/pybiotk/io/fasta.py`

 * *Files 5% similar despite different names*

```diff
@@ -15,31 +15,40 @@
     def __init__(self, /, *args, **kwargs):
         super().__init__()
         self.reference_dict: Optional[Dict[str, str]] = None
 
     def __iter__(self) -> Iterator:
         for reference in self.references:
             yield reference, self[reference]
+            
+    def _stdout(self, reference:str, wrap: bool = True, wrap_len: int = 60):
+        sys.stdout.write(f">{reference}\n")
+        sequence = self[reference]
+        if wrap:
+            seqlen = len(sequence)
+            index = range(seqlen)
+            for i in itertools.islice(index, None, None, wrap_len):
+                sys.stdout.write(f"{sequence[i: i+wrap_len]}\n")
+        else:
+            sys.stdout.write(f"{sequence}\n")
 
-    def stdout(self, referenceList: Optional[Sequence[str]] = None, wrap: bool = True):
+    def stdout(self, referenceList: Optional[Sequence[str]] = None, wrap: bool = True, wrap_len: int = 60):
         if not referenceList:
             referenceList = self.references
-
-        for reference in referenceList:
-            if reference not in self.references:
-                continue
-            sys.stdout.write(f">{reference}\n")
-            sequence = self[reference]
-            if wrap:
-                seqlen = len(sequence)
-                index = range(seqlen)
-                for i in itertools.islice(index, None, None, 60):
-                    sys.stdout.write(f"{sequence[i: i+60]}\n")
-            else:
-                sys.stdout.write(f"{sequence}\n")
+            
+        if len(referenceList) == 1:
+            for reference in self.references:
+                if not re.match(referenceList[0], reference):
+                    continue
+                self._stdout(reference, wrap, wrap_len)
+        else:
+            for reference in referenceList:
+                if reference not in self.references:
+                    continue
+                self._stdout(reference, wrap, wrap_len)
 
     def load_into_dict(self) -> Dict[str, str]:
         self.reference_dict = dict((reference, seq) for reference, seq in self)
         return self.reference_dict
 
     def fetchs(self, reference: str, start: int, end: int, strand: Literal["+", "-"] = "+"):
         sequence = self.fetch(reference, int(start), int(end))
@@ -79,15 +88,15 @@
         seq = sequence if strand == '+' else reverse_seq(sequence)
 
         return seq
 
     def chroms_norm(self) -> List[str]:
         chroms = []
         for chrom in self.chroms:
-            if chrom.startswith("chr") or re.match(r"\d.*", chrom):
+            if chrom.startswith("chr") or re.match(r"\d.*|X|Y|M|MT", chrom):
                 chroms.append(chrom)
         return chroms
 
     def random(self, length: int = 50, random_on_chroms: Optional[Sequence[str]] = None) -> Tuple[GRange, str]:
         strand = ["+", "-"][random.randint(0, 1)]
         chroms = self.custom_chroms
         if random_on_chroms:
```

### Comparing `pybiotk-1.1.1/src/pybiotk/io/fastq.py` & `pybiotk-1.2.0/src/pybiotk/io/fastq.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/io/gtf.py` & `pybiotk-1.2.0/src/pybiotk/io/gtf.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 import re
 from dataclasses import dataclass, field
 from io import TextIOWrapper
-from typing import List, Sequence, Tuple, Literal, Iterable, Iterator, Optional, Union, TextIO
+from typing import List, Sequence, Tuple, Dict, Literal, Iterable, Iterator, Optional, Union, TextIO
 
 from pybiotk.annodb import Transcript
 from pybiotk.utils import logging
 from pybiotk.io.bed import Bed6, Bed12, Intron, GeneInfo, TransInfo
 from stream.pipe import Pipe, sort, drop_while, filter, kgroupby, groupby, apply, window
 
 
@@ -16,81 +16,97 @@
     source: str = field(default=None, repr=False)
     feature: str = field(default=None)
     start: int = field(default=0)
     end: int = field(default=0)
     score: str = field(default=None, repr=False)
     strand: Literal['+', '-'] = field(default='+')
     frame: str = field(default=None, repr=False)
-    attributes: str = field(default=None, repr=False)
+    attributes: str = field(default="", repr=False)
     chrom: str = field(init=False, repr=False)
+    attributes_dict: Dict[str, str] = field(init=False, repr=False)
 
     def __post_init__(self):
         self.chrom = self.seqname
         self.start = int(self.start)
         self.end = int(self.end)
+        self.attributes_dict = self.get_attributes_dict()
 
     def __str__(self):
-        return "\t".join(str(s) for s in list(self.__dict__.values())[:9])
+        return "\t".join(str(s) for s in list(vars(self).values())[:9])
 
     @staticmethod
     def parse_attributes(term: str, attributes: str) -> Optional[str]:
-        parse_attr = re.compile(f'{term} "([^"]+)"')
+        parse_attr = re.compile(f'{term} ("[^"]+"|[^"]+);')
         patterns = parse_attr.findall(attributes)
 
         if patterns:
-            return patterns[0]
+            if len(patterns) == 1:
+                attribute = patterns[0].strip('"')
+            else:
+                attribute = ",".join(i.strip('"') for i in patterns)
+            return attribute
+
+    def get_attributes_dict(self) -> Dict[str, str]:
+        attr_dict = {}
+        parse_attr = re.compile(r'(?P<key>\S+) (?P<value1>"(?P<value2>[^"]+)"|[^"]+);')
+        for p in parse_attr.finditer(self.attributes):
+            key = p.group("key")
+            value = p.group("value2")
+            value = p.group("value1") if value is None else value
+            if key not in attr_dict:
+                attr_dict[key] = value
+            else:
+                attr_dict[key] += f",{value}"
+        return attr_dict
 
     def gene_type(self):
         for term in ['gene_type', 'gene_biotype']:
-            attr = self.parse_attributes(term, self.attributes)
-            if attr is not None:
-                return attr
+            if term in self.attributes_dict:
+                return self.attributes_dict[term]
 
     def gene_id(self):
-        return self.parse_attributes("gene_id", self.attributes)
+        return self.attributes_dict.get("gene_id")
 
     def gene_name(self):
+        attr = None
         for term in ["gene_name", "gene"]:
-            attr = self.parse_attributes(term, self.attributes)
-            if attr is not None:
-                return attr
-        else:
-            return self.gene_id()
+            if term in self.attributes_dict:
+                attr = self.attributes_dict[term]
+        attr = self.gene_id() if attr is None else attr
+
+        return attr
 
     def transcript_type(self):
         for term in ["transcript_type", "transcript_biotype"]:
-            attr = self.parse_attributes(term, self.attributes)
-            if attr is not None:
-                return attr
+            if term in self.attributes_dict:
+                return self.attributes_dict[term]
 
     def transcript_id(self):
-        attr = self.parse_attributes("transcript_id", self.attributes)
-        if attr is None:
-            attr = self.gene_id()
+        attr = self.attributes_dict.get("transcript_id")
+        attr = self.gene_id() if attr is None else attr
         return attr
 
     def transcript_name(self):
-        attr = self.parse_attributes("transcript_name", self.attributes)
-        if attr is None:
-            attr = self.gene_name()
+        attr = self.attributes_dict.get("transcript_name")
+        attr = self.gene_name() if attr is None else attr
         return attr
 
     def get_attribute(self, attribute):
         if attribute == "gene_type":
             return self.gene_type()
         elif attribute == "gene_name":
             return self.gene_name()
         elif attribute == "transcript_id":
             return self.transcript_id()
         elif attribute == "transcript_type":
             return self.transcript_type()
         elif attribute == "transcript_name":
             return self.transcript_name()
         else:
-            return self.parse_attributes(attribute, self.attributes)
+            return self.attributes_dict.get(attribute)
 
 
 @Pipe
 def to_GTF(iterable: Iterable[str]) -> Iterator[GTF]:
     for line in iterable:
         yield GTF(*line.rstrip("\r\n").split("\t"))
 
@@ -110,19 +126,24 @@
 
 
 @Pipe
 def to_TransInfo(iterable: Iterable[Tuple[GTF, ...]]) -> Iterator[TransInfo]:
     for group in iterable:
         gene_gtf: Sequence[GTF] = []
         trans_gtf: Sequence[GTF] = []
+        last_gtf = None
         for gtf in group:
+            last_gtf = gtf
             if gtf.feature == "gene":
                 gene_gtf.append(gtf)
             else:
                 trans_gtf.append(gtf)
+        if not trans_gtf:
+
+            logging.warning(f"No transcript feature found for gene: {last_gtf.get_attribute('gene_name')}")
         for gtf in trans_gtf:
             trans_info = TransInfo.init_by_gtf(gtf)
             if gene_gtf :
                 if trans_info.gene_type is None:
                     trans_info.gene_type = gene_gtf[0].gene_type()
             yield trans_info
 
@@ -193,15 +214,15 @@
             if cds_exons:
                 cds_start = cds_exons[0].start - 1
                 cds_end = cds_exons[-1].end
                 transcript.cds_start = cds_start
                 transcript.cds_end = cds_end
             else:
                 transcript.cds_start = transcript.cds_end = None
-    
+
             if gene_gtf:
                 if transcript.gene_type is None:
                     transcript.gene_type = gene_gtf[0].gene_type()
             if transcript.transcript_type is None:
                 transcript.transcript_type = transcript.gene_type
 
             yield transcript
```

### Comparing `pybiotk-1.1.1/src/pybiotk/utils/bam_random.py` & `pybiotk-1.2.0/src/pybiotk/utils/bam_random.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/utils/fasta_filter.py` & `pybiotk-1.2.0/src/pybiotk/utils/fasta_filter.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,30 +3,31 @@
 import time
 from typing import Sequence
 
 from pybiotk.io import FastaFile
 from pybiotk.utils import logging, ignore
 
 
-def main(filename, chromList: Sequence[str], wrap: bool = True):
+def main(filename, chromList: Sequence[str], wrap: bool = True, wrap_len: int = 60):
     logging.info("reading fasta ....")
     start = time.perf_counter()
     with FastaFile(filename) as fa:
-        fa.stdout(referenceList=chromList, wrap=wrap)
+        fa.stdout(referenceList=chromList, wrap=wrap, wrap_len=wrap_len)
     end = time.perf_counter()
     logging.info(f"task finished in {end-start:.2f}s.")
 
 
 @ignore
 def run():
     parser = argparse.ArgumentParser(
         description=__doc__,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument(dest="fasta", type=str, help="Genome fasta file.")
-    parser.add_argument("-c", dest="chromlist", nargs="+", default=None, help="chrom list for split genome.")
+    parser.add_argument("-c", dest="chromlist", nargs="+", default=None, help="chrom list for split genome. one parameter will be regarded as a regular expression.")
     parser.add_argument("--wrap", dest="wrap", action="store_true", help="line-wrapped display.")
+    parser.add_argument("--wrap-len", dest="wrap_len", type=int, default=60, help="line length.")
     args = parser.parse_args()
-    main(args.fasta, args.chromlist, args.wrap)
+    main(args.fasta, args.chromlist, args.wrap, args.wrap_len)
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `pybiotk-1.1.1/src/pybiotk/utils/fastq_join.py` & `pybiotk-1.2.0/src/pybiotk/utils/fastq_join.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/utils/fastq_uniq.py` & `pybiotk-1.2.0/src/pybiotk/utils/fastq_uniq.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/utils/fastx_rename.py` & `pybiotk-1.2.0/src/pybiotk/utils/fastx_rename.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/utils/fragment_size.py` & `pybiotk-1.2.0/src/pybiotk/utils/fragment_size.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/utils/genomefetcher.py` & `pybiotk-1.2.0/src/pybiotk/utils/genomefetcher.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 #!/usr/bin/env python3
 # -*- coding: utf-8 -*-
 # Path: src/pybiotk/utils/genomefetcher.py
 """
 Fetch sequences from genome fasta file with gtf file.
 """
 import argparse
-import itertools
 import re
 import sys
 import time
 from typing import Sequence, Optional, TextIO
 
 from pybiotk.io import GenomeFile, GtfFile
 from pybiotk.utils import logging, ignore
```

### Comparing `pybiotk-1.1.1/src/pybiotk/utils/gtf_filter.py` & `pybiotk-1.2.0/src/pybiotk/utils/gtf_filter.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/utils/merge_row.py` & `pybiotk-1.2.0/src/pybiotk/utils/merge_row.py`

 * *Files 2% similar despite different names*

```diff
@@ -99,16 +99,16 @@
 @ignore
 def run():
     parser = argparse.ArgumentParser(
         description=__doc__,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument("-i", "--input", dest="input", type=str,
                         default=(None if sys.stdin.isatty() else "-"), help="Input table file.")
-    parser.add_argument("-o", "--output", dest="output", type=argparse.FileType('w'),
-                        default=sys.stdout, help="Output file, discard this parameter to print output to stdout.")
+    parser.add_argument("-o", "--output", dest="output", type=str,
+                        default="-", help="Output file, discard this parameter to print output to stdout.")
     parser.add_argument("--header", dest="header", type=int, default=0,
                         help="The selected row will be the header, 0 based.")
     parser.add_argument("--noheader", dest="noheader", action="store_true",
                         help="If no header, this option overrides --header.")
     parser.add_argument("-by", dest="by", type=str, default="0",
                         help="The same values in the selected columns will be merged, 0 based, use ',' to separate.")
     parser.add_argument("-c", "--columns", dest="columns", type=str, default=None,
```

### Comparing `pybiotk-1.1.1/src/pybiotk/utils/merge_subseq.py` & `pybiotk-1.2.0/src/pybiotk/utils/merge_subseq.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/utils/normalize.py` & `pybiotk-1.2.0/src/pybiotk/utils/normalize.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 #!/usr/bin/env python3
 import argparse
 import os
-import sys
 from typing import Sequence, Literal
 
 import pandas as pd
 
 from pybiotk.utils import write_table, ignore
 
 
@@ -97,17 +96,17 @@
 
 @ignore
 def run():
     parser = argparse.ArgumentParser(
         description=__doc__,
         formatter_class=argparse.ArgumentDefaultsHelpFormatter)
     parser.add_argument("input", type=str, help="featureCount out file.")
-    parser.add_argument("-c", dest="columns", type=int, nargs="+", default=[0, 6, 5], help="geneid, count, length(required by RPKM and TPM) column, 0 based.")
+    parser.add_argument("-c", dest="columns", type=int, nargs="+", default=[0, 5, 6], help="geneid, length(required by RPKM and TPM), count column, 0 based.")
     parser.add_argument("-m", dest="method", type=str, default="CPM", choices=("CPM", "RPKM", "TPM"), help="normalize method, [CPM|RPKM|TPM].")
-    parser.add_argument("-o", dest="output", type=argparse.FileType('w'), default=sys.stdout, help="output file.")
+    parser.add_argument("-o", dest="output", type=str, default="-", help="output file. [stdout]")
 
     args = parser.parse_args()
     main(args.input, args.columns, args.method, args.output)
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `pybiotk-1.1.1/src/pybiotk/utils/pyanno.py` & `pybiotk-1.2.0/src/pybiotk/utils/pyanno.py`

 * *Files 9% similar despite different names*

```diff
@@ -53,15 +53,17 @@
 
 
 def annobam(filename: str,
             file_obj: TextIO,
             grangetree: GRangeTree,
             anno_fragments: bool = False,
             tss_region: Tuple[int, int] = (-1000, 1000),
+            tss_region_name: str = "Upstream",
             downstream: int = 3000,
+            downstream_name: str = "Downstream",
             rule: str = "1+-,1-+,2++,2--",
             ordered_by_name: bool = False
             ):
     bamtype = check_bam_type(filename)
 
     def anno_read(_blocks, _strand, _read):
         start = int(_blocks[0][0])
@@ -71,15 +73,18 @@
         if not genes:
             file_obj.write(f"{_read.query_name}\t{_read.reference_name}\t{start}\t{end}\t{_blocks}\t{fragment_strand}\tIntergenic\t*\t*\t*\t*\t*\n")
         else:
             annoset = AnnoSet(gene.annotation(_blocks, tss_region, downstream) for gene in genes)
             gene_types = set(gene.gene_type for gene in genes if gene.id in set(annoset.id))
             if not ("protein_coding" in gene_types and "protein_coding" not in set(annoset.type)):
                 annoset.type = gene_types
-            file_obj.write(f"{_read.query_name}\t{_read.reference_name}\t{start}\t{end}\t{_blocks}\t{fragment_strand}\t{annoset}\n")
+            anno_str = str(annoset)
+            anno_str = tss_region_name if anno_str == "Promoter" else anno_str
+            anno_str = downstream_name if anno_str == "Downstream" else anno_str
+            file_obj.write(f"{_read.query_name}\t{_read.reference_name}\t{start}\t{end}\t{_blocks}\t{fragment_strand}\t{anno_str}\n")
 
     if bamtype is BamType.PE and anno_fragments:
         with BamPE(filename) as bam:
             bam.ordered_by_name = ordered_by_name
             for read1, read2 in bam.iter_pair(properly_paired=False):
                 if read1 is not None and read2 is not None:
                     strand1 = "-" if read1.is_reverse else "+"
@@ -111,39 +116,46 @@
             sys.stderr.write(f"annotate {i} reads.\n")
 
 
 def annobed(filename: str,
             file_obj: TextIO,
             grangetree: GRangeTree,
             tss_region: Tuple[int, int] = (-1000, 1000),
-            downstream: int = 3000
+            tss_region_name: str = "Upstream",
+            downstream: int = 3000,
+            downstream_name: str = "Downstream",
             ):
     with Openbed(filename) as bedfile:
         i = 0
         for bed in bedfile:
             genes = grangetree.find(bed.chrom, bed.start, bed.end, bed.strand)
             if not genes:
                 file_obj.write(f"{bed.name}\t{bed.chrom}\t{bed.start}\t{bed.end}\t{bed.strand}\tIntergenic\t*\t*\t*\t*\t*\n")
             else:
                 annoset = AnnoSet(gene.annotation([(bed.start, bed.end)], tss_region, downstream) for gene in genes)
                 gene_types = set(gene.gene_type for gene in genes if gene.id in set(annoset.id))
                 if not ("protein_coding" in gene_types and "protein_coding" not in set(annoset.type)):
                     annoset.type = gene_types
-                file_obj.write(f"{bed.name}\t{bed.chrom}\t{bed.start}\t{bed.end}\t{bed.strand}\t{annoset}\n")
+                anno_str = str(annoset)
+                anno_str = tss_region_name if anno_str == "Promoter" else anno_str
+                anno_str = downstream_name if anno_str == "Downstream" else anno_str
+                file_obj.write(f"{bed.name}\t{bed.chrom}\t{bed.start}\t{bed.end}\t{bed.strand}\t{anno_str}\n")
             i += 1
         sys.stderr.write(f"annotate {i} beds.\n")
 
 
 def main(
     filename: str,
     outfilename: str,
     gtf_file: str,
     level: Literal["transcript", "gene"] = "transcript",
     tss_region: Tuple[int, int] = (-3000, 0),
+    tss_region_name: str = "Upstream",
     downstream: int = 3000,
+    downstream_name: str = "Downstream",
     strand: bool = True,
     rule: str = "1+-,1-+,2++,2--",
     annofragments: bool = False,
     ordered_by_name: bool = False
 ):
     start = time.perf_counter()
     filetype = os.path.splitext(filename)[1]
@@ -152,19 +164,19 @@
         ostream = sys.stdout
     else:
         ostream = open(outfilename, "w", encoding="utf-8")
     with ostream as annofile:
         if filetype == ".bam":
             annofile.write("seqname\tchrom\tstart\tend\tblocks\tstrand\tannotation\tgeneStart\tgeneEnd\tgeneName\tid\tgeneType\n")
             logging.info("start annotating, use bam mode ...")
-            annobam(filename, annofile, grangetree, annofragments, tss_region, downstream, rule, ordered_by_name)
+            annobam(filename, annofile, grangetree, annofragments, tss_region, tss_region_name, downstream, downstream_name, rule, ordered_by_name)
         elif filetype.startswith(".bed"):
             annofile.write("seqname\tchrom\tstart\tend\tstrand\tannotation\tgeneStart\tgeneEnd\tgeneName\tid\tgeneType\n")
             logging.info("start annotating, use bed mode ...")
-            annobed(filename, annofile, grangetree, tss_region, downstream)
+            annobed(filename, annofile, grangetree, tss_region, tss_region_name, downstream, downstream_name)
         else:
             raise RuntimeError(f"Unable to infer file type as bam or bed from filename: {filename}.")
     end = time.perf_counter()
     logging.info(f"task completed in {end-start:.2f}s, annofile saved in {outfilename}")
 
 
 def run():
@@ -176,26 +188,30 @@
     parser.add_argument("-o", "--output", dest="output", type=str, default="-", help="output file name. [stdout]")
     parser.add_argument("-g", "--gtf", dest='gtf', required=True,
                         help="gtf file download from Genecode, or a sorted gtf file.")
     parser.add_argument("-l", "--level", dest="level", type=str, default="transcript", choices=("transcript", "gene"),
                         help="annotation level, transcript or gene.")
     parser.add_argument("--tss_region", dest="tss_region", type=int, nargs="+", default=[-3000, 0],
                         help="choose region from tss.")
+    parser.add_argument("--tss_region_name", dest="tss_region_name", type=str, default="Upstream", help="tss region name.")
     parser.add_argument("--downstream", dest="downstream", type=int, default=3000, help="downstream length from tes.")
+    parser.add_argument("--downstream_name", dest="downstream_name", type=str, default="Downstream", help="downstream name.")
     parser.add_argument("-s", "--strand", dest="strand", action="store_true", help="require same strandedness.")
     parser.add_argument("--rule", dest="rule", type=str, default="1+-,1-+,2++,2--",
                         choices=("1+-,1-+,2++,2--", "1++,1--,2+-,2-+", "+-,-+", "++,--"),
                         help="how read(s) were stranded during sequencing. only for bam.")
     parser.add_argument("-p", "--pair", dest="pair", action="store_true",
                         help="annotate fragments instead of reads.")
     parser.add_argument("--ordered_by_name", dest="ordered_by_name", action="store_true",
                         help="if input bam is ordered by name, only for pair-end bam.")
 
     args = parser.parse_args()
 
     if not len(args.tss_region) == 2:
         parser.error("--tss_region must be a tuple of 2 elements.")
-    main(args.input, args.output, args.gtf, args.level, args.tss_region, args.downstream, args.strand, args.rule, args.pair, args.ordered_by_name)
+    main(args.input, args.output, args.gtf, args.level,
+         args.tss_region, args.tss_region_name, args.downstream, args.downstream_name,
+         args.strand, args.rule, args.pair, args.ordered_by_name)
 
 
 if __name__ == "__main__":
     run()
```

### Comparing `pybiotk-1.1.1/src/pybiotk/utils/read_tables.py` & `pybiotk-1.2.0/src/pybiotk/utils/read_tables.py`

 * *Files 6% similar despite different names*

```diff
@@ -4,24 +4,28 @@
 """
 import argparse
 import csv
 import os
 import sys
 
 import pandas as pd
-from pybiotk.utils import ignore, read_table, write_table
+from pybiotk.utils import ignore, read_table, write_table, logging
 
 
 def main(table_list, outfile, namefile, noheader, column, delimiter=None, exclude=False, contains=False):
     df_list = []
     for table in table_list:
         header = None if noheader else 0
         df = read_table(table, header=header, dtype=str, comment="#")
         if namefile is not None:
-            names = set(j for i in namefile for j in i.split())
+            try:
+                names = set(j for i in namefile for j in i.split())
+            except Exception as e:
+                logging.warning("Failed to load namefile: "+str(e))
+                names = False
             if names:
                 if exclude:
                     if contains:
                         df = df.loc[~df.iloc[:, column].str.contains("|".join(names))]
                     else:
                         if delimiter is not None:
                             df = df.loc[~df.iloc[:, column].str.split(delimiter).apply(lambda x: any(set(x) & names))]
```

### Comparing `pybiotk-1.1.1/src/pybiotk/utils/reference_count.py` & `pybiotk-1.2.0/src/pybiotk/utils/reference_count.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/utils/reverse_fastx.py` & `pybiotk-1.2.0/src/pybiotk/utils/reverse_fastx.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/utils/rmats_filter.py` & `pybiotk-1.2.0/src/pybiotk/utils/rmats_filter.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,16 +10,17 @@
     if p_value:
         df = df[df['PValue'] < p_value]
     if fdr_value:
         df = df[df['FDR'] < fdr_value]
     if inclevel:
         df = df[abs(df['IncLevelDifference']) > inclevel]
     if readnumber:
-        df['AvgSAMPLE1'] = (df['IJC_SAMPLE_1'] + df['SJC_SAMPLE_1']) / 2
-        df['AvgSAMPLE2'] = (df['IJC_SAMPLE_2'] + df['SJC_SAMPLE_2']) / 2
+        func = lambda x:sum(int(i) for i in str(x).split(","))
+        df['AvgSAMPLE1'] = (df['IJC_SAMPLE_1'].apply(func) + df['SJC_SAMPLE_1'].apply(func)) / 2
+        df['AvgSAMPLE2'] = (df['IJC_SAMPLE_2'].apply(func) + df['SJC_SAMPLE_2'].apply(func)) / 2
         df = df[(df['AvgSAMPLE1'] > readnumber) & (df['AvgSAMPLE2'] > readnumber)]
         df = df.drop('AvgSAMPLE2', axis=1)
         df = df.drop('AvgSAMPLE1', axis=1)
 
     df['sort_key'] = df.IncLevelDifference.abs()
 
     df = df.sort_values(by=['sort_key', 'FDR'], ascending=[False, True])
```

### Comparing `pybiotk-1.1.1/src/pybiotk/utils/seq_random.py` & `pybiotk-1.2.0/src/pybiotk/utils/seq_random.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/utils/subseq_analysis.py` & `pybiotk-1.2.0/src/pybiotk/utils/subseq_analysis.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/src/pybiotk/utils/utils.py` & `pybiotk-1.2.0/src/pybiotk/utils/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 # -*- coding: utf-8 -*-
 import importlib
 import importlib.resources
 import logging
 import os
+import re
 import subprocess
 import sys
 import warnings
 from functools import wraps
 from io import TextIOWrapper
 from types import ModuleType
 from typing import List, Dict, Sequence, Tuple, Literal, Iterator, Iterable, Optional, Callable, Union, TextIO
 
 import pandas as pd
 
-logging.basicConfig(format="%(asctime)s %(levelname)s: %(message)s", datefmt='%Y-%m-%d %A %H:%M:%S', level=logging.INFO)
+from rich.logging import RichHandler
+from rich.console import Console
 
+Handler = RichHandler(console=Console(stderr=True), show_time=True, omit_repeated_times=False, show_level=True, markup=True, log_time_format='[%x %a %X]')
+logging.basicConfig(level="NOTSET", format="%(message)s", handlers=[Handler])
 
 def reverse_seq(seq: str) -> str:
     seq = seq.upper()
     complement = {
         "A": "T", "C": "G", "G": "C", "T": "A",
         "N": "N", "W": "W", "S": "S", "K": "M",
         "M": "K", "Y": "R", "R": "Y", "H": "D",
@@ -42,14 +46,20 @@
     for interval1 in intervals1:
         for interval2 in intervals2:
             if is_overlap(interval1, interval2):
                 return True
     return False
 
 
+def cigar2cigar_tuples(cigar: str) -> List[Tuple[int, int]]:
+    code2cigar = "MIDNSHP=XBp"
+    cigar_regex = re.compile("([-\d]+)([MIDNSHP=XBp])")
+    return [(code2cigar.find(x[1]), int(x[0])) for x in re.findall(cigar_regex, cigar)]
+
+
 def cigar_tuples2blocks(start: int, cigartuples: Sequence[Tuple[int, int]], shift: int = 0) -> List[Tuple[int, int]]:
     tmp_abs_start = shift + start
     blocks = []
     for cigar, length in cigartuples:
         if cigar in [0, 2]:
             blocks.append((tmp_abs_start, tmp_abs_start + length))
             tmp_abs_start += length
@@ -189,18 +199,23 @@
 
 def ignore(func: Callable):
     @wraps(func)
     def wrapper(*args, **kargs):
         try:
             traceback = func(*args, **kargs)
         except BrokenPipeError:
-            sys.stdout = None
+            # https://docs.python.org/3/library/signal.html#note-on-sigpipe
+            # Python flushes standard streams on exit; redirect remaining output
+            # to devnull to avoid another BrokenPipeError at shutdown
+            devnull = os.open(os.devnull, os.O_WRONLY)
+            os.dup2(devnull, sys.stdout.fileno())
             sys.exit(0)
         except KeyboardInterrupt:
-            sys.stdout = None
+            devnull = os.open(os.devnull, os.O_WRONLY)
+            os.dup2(devnull, sys.stdout.fileno())
             sys.exit(0)
         return traceback
     return wrapper
 
 
 def load_chrom_length_dict(filepath_or_buffer: Union[str, TextIOWrapper]) -> Dict[str, int]:
     if isinstance(filepath_or_buffer, TextIOWrapper):
```

### Comparing `pybiotk-1.1.1/src/pybiotk.egg-info/SOURCES.txt` & `pybiotk-1.2.0/src/pybiotk.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -23,20 +23,20 @@
 docs/_static/.gitignore
 rscripts/diff_expr_DESeq2.R
 rscripts/diff_expr_edgeR.R
 rscripts/diff_expr_plot.R
 rscripts/peak_anno.R
 rscripts/plot_FRiPs.R
 rscripts/plot_bar.R
+rscripts/plot_chip_summary.R
 rscripts/plot_corr.R
 rscripts/plot_deeptools_fragmentsize.R
 rscripts/plot_hist.R
 rscripts/plot_peak_width.R
 rscripts/plot_rep_cor.R
-rscripts/plot_summary.R
 rscripts/plot_venn.R
 scripts/fasta_len.sh
 scripts/fasta_u2t.sh
 scripts/fastq_len.sh
 scripts/get_chrom_length.sh
 scripts/gtfparser.sh
 scripts/merge_subseq.sh
@@ -81,14 +81,17 @@
 src/pybiotk/io/__init__.py
 src/pybiotk/io/bam.py
 src/pybiotk/io/bed.py
 src/pybiotk/io/bw.py
 src/pybiotk/io/fasta.py
 src/pybiotk/io/fastq.py
 src/pybiotk/io/gtf.py
+src/pybiotk/string/__init__.py
+src/pybiotk/string/motif.py
+src/pybiotk/string/sequence.py
 src/pybiotk/utils/__init__.py
 src/pybiotk/utils/bam_random.py
 src/pybiotk/utils/fasta_filter.py
 src/pybiotk/utils/fastq_join.py
 src/pybiotk/utils/fastq_uniq.py
 src/pybiotk/utils/fastx_rename.py
 src/pybiotk/utils/fragment_size.py
```

### Comparing `pybiotk-1.1.1/src/pybiotk.egg-info/entry_points.txt` & `pybiotk-1.2.0/src/pybiotk.egg-info/entry_points.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,7 +18,8 @@
 read_tables = pybiotk.utils.read_tables:run
 reference_count = pybiotk.utils.reference_count:run
 reverse_fastx = pybiotk.utils.reverse_fastx:run
 rmats_filter = pybiotk.utils.rmats_filter:run
 rna_fragment_size = pybiotk.utils.fragment_size:run
 seq_random = pybiotk.utils.seq_random:run
 subseq_analysis = pybiotk.utils.subseq_analysis:run
+summary_log = pybiotk.utils.summary_log:run
```

### Comparing `pybiotk-1.1.1/src/stream/pipe.py` & `pybiotk-1.2.0/src/stream/pipe.py`

 * *Files 0% similar despite different names*

```diff
@@ -103,28 +103,34 @@
     def __ror__(self, other: Iterable[_T]):
         return self.func(other)
 
     def __call__(self, *args, **kwargs):
         return Pipe(lambda x: self.func(x, *args, **kwargs))
 
 
-def cat(file: str) -> Iterator[str]:
-    with open(file) as f:
-        for line in f:
-            line = line.rstrip("\n")
-            if line:
-                yield line
-
-
-def zcat(file: str) -> Iterator[str]:
-    with gzip.open(file, "rb") as f:
-        for line in f:
-            line = line.decode().rstrip("\n")
-            if line:
-                yield line
+def cat(files: Union[str, Iterable[str]]) -> Iterator[str]:
+    if isinstance(files, str):
+        files = [files]
+    for file in files:
+        with open(file) as f:
+            for line in f:
+                line = line.rstrip("\r\n")
+                if line:
+                    yield line
+
+
+def zcat(files: Union[str, Iterable[str]]) -> Iterator[str]:
+    if isinstance(files, str):
+        files = [files]
+    for file in files:
+        with gzip.open(file, "rb") as f:
+            for line in f:
+                line = line.decode().rstrip("\r\n")
+                if line:
+                    yield line
 
 
 def stdin() -> Iterator[str]:
     for line in sys.stdin:
         line = line.rstrip("\n")
         if line:
             yield line
@@ -149,15 +155,15 @@
         os.makedirs(path)
 
 
 def cd(path):
     if os.path.exists(path):
         os.chdir(path)
     else:
-        raise RuntimeError(f'{path} not exist')
+        raise FileNotFoundError(f'No such directory: {path}')
 
 
 @Pipe
 def head(iterable: Iterable[_T], n: int = 10) -> Iterator[_T]:
     """Yield n of elements in the given iterable."""
     return itertools.islice(iterable, n)
```

### Comparing `pybiotk-1.1.1/src/stream/stream.py` & `pybiotk-1.2.0/src/stream/stream.py`

 * *Files identical despite different names*

### Comparing `pybiotk-1.1.1/tox.ini` & `pybiotk-1.2.0/tox.ini`

 * *Files identical despite different names*

