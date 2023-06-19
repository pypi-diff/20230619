# Comparing `tmp/rp2-1.4.2.tar.gz` & `tmp/rp2-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rp2-1.4.2.tar", last modified: Sat Apr  1 22:40:25 2023, max compression
+gzip compressed data, was "rp2-1.5.0.tar", last modified: Mon Jun 19 10:31:02 2023, max compression
```

## Comparing `rp2-1.4.2.tar` & `rp2-1.5.0.tar`

### file list

```diff
@@ -1,257 +1,276 @@
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.557917 rp2-1.4.2/
--rw-r--r--   0 marcoz     (501) staff       (20)    13932 2023-04-01 22:34:03.000000 rp2-1.4.2/CHANGELOG.md
--rw-r--r--   0 marcoz     (501) staff       (20)     2761 2022-08-09 16:07:45.000000 rp2-1.4.2/CONTRIBUTING.md
--rw-r--r--   0 marcoz     (501) staff       (20)    11357 2022-08-09 16:07:45.000000 rp2-1.4.2/LICENSE
--rw-r--r--   0 marcoz     (501) staff       (20)      263 2022-09-03 21:25:38.000000 rp2-1.4.2/MANIFEST.in
--rw-r--r--   0 marcoz     (501) staff       (20)    33726 2023-04-01 22:40:25.558014 rp2-1.4.2/PKG-INFO
--rw-r--r--   0 marcoz     (501) staff       (20)    22255 2023-04-01 22:28:32.000000 rp2-1.4.2/README.dev.md
--rw-r--r--   0 marcoz     (501) staff       (20)    18102 2023-04-01 22:28:32.000000 rp2-1.4.2/README.md
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.509875 rp2-1.4.2/config/
--rw-r--r--   0 marcoz     (501) staff       (20)      636 2023-01-26 03:44:18.000000 rp2-1.4.2/config/crypto_example.ini
--rw-r--r--   0 marcoz     (501) staff       (20)      762 2023-01-26 03:44:18.000000 rp2-1.4.2/config/test_bad_data.ini
--rw-r--r--   0 marcoz     (501) staff       (20)      597 2023-01-26 03:44:18.000000 rp2-1.4.2/config/test_data.ini
--rw-r--r--   0 marcoz     (501) staff       (20)      556 2023-01-26 03:44:18.000000 rp2-1.4.2/config/test_data4.ini
--rw-r--r--   0 marcoz     (501) staff       (20)      675 2023-01-26 03:44:18.000000 rp2-1.4.2/config/test_data_multi_method.ini
--rw-r--r--   0 marcoz     (501) staff       (20)      516 2023-01-26 03:44:18.000000 rp2-1.4.2/config/test_large_input.ini
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.510600 rp2-1.4.2/docs/
--rw-r--r--   0 marcoz     (501) staff       (20)     2893 2022-08-09 16:07:45.000000 rp2-1.4.2/docs/developer_faq.md
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.512736 rp2-1.4.2/docs/images/
--rw-r--r--   0 marcoz     (501) staff       (20)    94354 2022-08-09 16:07:45.000000 rp2-1.4.2/docs/images/input_spreadsheet.png
--rw-r--r--   0 marcoz     (501) staff       (20)    66768 2022-08-09 16:07:45.000000 rp2-1.4.2/docs/images/open_positions_asset.png
--rw-r--r--   0 marcoz     (501) staff       (20)    87502 2022-08-09 16:07:45.000000 rp2-1.4.2/docs/images/open_positions_asset_exchange.png
--rw-r--r--   0 marcoz     (501) staff       (20)    16751 2022-08-09 16:07:45.000000 rp2-1.4.2/docs/images/open_positions_input.png
--rw-r--r--   0 marcoz     (501) staff       (20)   126454 2022-08-22 21:12:06.000000 rp2-1.4.2/docs/images/rp2_full_report_output_in_out.png
--rw-r--r--   0 marcoz     (501) staff       (20)    43264 2022-08-09 16:07:45.000000 rp2-1.4.2/docs/images/rp2_full_report_output_summary.png
--rw-r--r--   0 marcoz     (501) staff       (20)   229926 2022-08-09 16:07:45.000000 rp2-1.4.2/docs/images/rp2_full_report_output_tax.png
--rw-r--r--   0 marcoz     (501) staff       (20)   156431 2022-08-09 16:07:45.000000 rp2-1.4.2/docs/images/rp2_header.png
--rw-r--r--   0 marcoz     (501) staff       (20)    61646 2022-08-09 16:07:45.000000 rp2-1.4.2/docs/images/tax_report_us_output_capital_gains.png
--rw-r--r--   0 marcoz     (501) staff       (20)    24446 2022-08-09 16:07:45.000000 rp2-1.4.2/docs/images/tax_report_us_output_interest.png
--rw-r--r--   0 marcoz     (501) staff       (20)    15575 2023-01-26 03:44:18.000000 rp2-1.4.2/docs/input_files.md
--rw-r--r--   0 marcoz     (501) staff       (20)     8053 2023-01-26 03:44:18.000000 rp2-1.4.2/docs/output_files.md
--rw-r--r--   0 marcoz     (501) staff       (20)    27046 2023-03-18 05:55:57.000000 rp2-1.4.2/docs/user_faq.md
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.514356 rp2-1.4.2/input/
--rw-r--r--   0 marcoz     (501) staff       (20)    18562 2022-08-09 16:07:45.000000 rp2-1.4.2/input/crypto_example.ods
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.534065 rp2-1.4.2/input/golden/
--rw-r--r--   0 marcoz     (501) staff       (20)    28227 2022-08-11 23:19:50.000000 rp2-1.4.2/input/golden/crypto_example_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    27598 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/crypto_example_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    28267 2022-08-11 23:19:50.000000 rp2-1.4.2/input/golden/crypto_example_hifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    27561 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/crypto_example_hifo_tax_report_us.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    12608 2023-01-26 03:44:18.000000 rp2-1.4.2/input/golden/crypto_example_jp_en_fifo_open_positions.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    46257 2023-01-26 03:44:18.000000 rp2-1.4.2/input/golden/crypto_example_jp_en_fifo_rp2_full_report.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    57435 2023-01-26 03:44:18.000000 rp2-1.4.2/input/golden/crypto_example_jp_en_fifo_tax_report_jp.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    28267 2022-08-11 23:19:50.000000 rp2-1.4.2/input/golden/crypto_example_lifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    27560 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/crypto_example_lifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    38189 2022-08-11 23:18:19.000000 rp2-1.4.2/input/golden/test_data2_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    29720 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_data2_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    37998 2022-08-24 21:18:51.000000 rp2-1.4.2/input/golden/test_data2_hifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    29513 2022-08-24 21:18:51.000000 rp2-1.4.2/input/golden/test_data2_hifo_tax_report_us.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    13044 2023-01-26 03:44:18.000000 rp2-1.4.2/input/golden/test_data2_jp_en_fifo_open_positions.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    56093 2023-01-26 03:44:18.000000 rp2-1.4.2/input/golden/test_data2_jp_en_fifo_rp2_full_report.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    76795 2023-01-26 03:44:18.000000 rp2-1.4.2/input/golden/test_data2_jp_en_fifo_tax_report_jp.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    38085 2022-08-11 23:18:19.000000 rp2-1.4.2/input/golden/test_data2_lifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    29748 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_data2_lifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    31353 2022-08-11 23:18:56.000000 rp2-1.4.2/input/golden/test_data3_2019-12-01_2020-04-01_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    23272 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_data3_2019-12-01_2020-04-01_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    31002 2022-08-11 23:18:56.000000 rp2-1.4.2/input/golden/test_data3_2019-12-01_2020-04-01_hifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    23181 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_data3_2019-12-01_2020-04-01_hifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    30871 2022-08-11 23:18:56.000000 rp2-1.4.2/input/golden/test_data3_2019-12-01_2020-04-01_lifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    23125 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_data3_2019-12-01_2020-04-01_lifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    32272 2022-08-11 23:18:56.000000 rp2-1.4.2/input/golden/test_data3_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    23558 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_data3_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    31831 2022-08-11 23:18:56.000000 rp2-1.4.2/input/golden/test_data3_hifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    23324 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_data3_hifo_tax_report_us.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    12780 2023-01-26 03:44:18.000000 rp2-1.4.2/input/golden/test_data3_jp_en_fifo_open_positions.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    50213 2023-01-26 03:44:18.000000 rp2-1.4.2/input/golden/test_data3_jp_en_fifo_rp2_full_report.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    70575 2023-01-26 03:44:18.000000 rp2-1.4.2/input/golden/test_data3_jp_en_fifo_tax_report_jp.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    31703 2022-08-11 23:18:56.000000 rp2-1.4.2/input/golden/test_data3_lifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    23268 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_data3_lifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    31106 2022-10-16 20:35:40.000000 rp2-1.4.2/input/golden/test_data4_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    20872 2022-10-16 20:35:56.000000 rp2-1.4.2/input/golden/test_data4_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    30959 2022-10-16 20:35:40.000000 rp2-1.4.2/input/golden/test_data4_hifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    20807 2022-10-16 20:35:56.000000 rp2-1.4.2/input/golden/test_data4_hifo_tax_report_us.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    12317 2023-01-26 03:44:18.000000 rp2-1.4.2/input/golden/test_data4_jp_en_fifo_open_positions.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    49159 2023-01-26 03:44:18.000000 rp2-1.4.2/input/golden/test_data4_jp_en_fifo_rp2_full_report.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    59596 2023-01-26 03:44:18.000000 rp2-1.4.2/input/golden/test_data4_jp_en_fifo_tax_report_jp.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    30917 2022-10-16 20:35:40.000000 rp2-1.4.2/input/golden/test_data4_lifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    20784 2022-10-16 20:35:56.000000 rp2-1.4.2/input/golden/test_data4_lifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    35766 2022-08-11 23:19:05.000000 rp2-1.4.2/input/golden/test_data_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    29160 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_data_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    35784 2022-08-11 23:19:05.000000 rp2-1.4.2/input/golden/test_data_hifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    28958 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_data_hifo_tax_report_us.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    13247 2023-01-26 03:44:18.000000 rp2-1.4.2/input/golden/test_data_jp_en_fifo_open_positions.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    53767 2023-01-26 03:44:18.000000 rp2-1.4.2/input/golden/test_data_jp_en_fifo_rp2_full_report.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    73415 2023-01-26 03:44:18.000000 rp2-1.4.2/input/golden/test_data_jp_en_fifo_tax_report_jp.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    13272 2023-01-26 03:44:18.000000 rp2-1.4.2/input/golden/test_data_jp_kl_fifo_open_positions.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    35898 2023-01-26 03:44:18.000000 rp2-1.4.2/input/golden/test_data_jp_kl_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    35784 2022-08-11 23:19:05.000000 rp2-1.4.2/input/golden/test_data_lifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    28957 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_data_lifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    44766 2022-08-29 15:38:01.000000 rp2-1.4.2/input/golden/test_data_multi_method_mixed_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    23648 2022-08-29 15:38:23.000000 rp2-1.4.2/input/golden/test_data_multi_method_mixed_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    31746 2022-08-24 21:18:51.000000 rp2-1.4.2/input/golden/test_hifo2_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    18147 2022-08-24 21:18:51.000000 rp2-1.4.2/input/golden/test_hifo2_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    32073 2022-08-24 21:18:51.000000 rp2-1.4.2/input/golden/test_hifo2_hifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    18258 2022-08-24 21:18:51.000000 rp2-1.4.2/input/golden/test_hifo2_hifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    32296 2022-08-24 21:18:51.000000 rp2-1.4.2/input/golden/test_hifo2_lifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    18266 2022-08-24 21:18:51.000000 rp2-1.4.2/input/golden/test_hifo2_lifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    36717 2022-08-11 23:19:55.000000 rp2-1.4.2/input/golden/test_hifo_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    29719 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_hifo_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    36742 2022-08-11 23:19:55.000000 rp2-1.4.2/input/golden/test_hifo_hifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    29722 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_hifo_hifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    36422 2022-08-11 23:19:55.000000 rp2-1.4.2/input/golden/test_hifo_lifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    29521 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_hifo_lifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    63483 2022-08-11 23:20:16.000000 rp2-1.4.2/input/golden/test_large_input_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    31061 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_large_input_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    61078 2022-08-24 21:18:51.000000 rp2-1.4.2/input/golden/test_large_input_hifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    29914 2022-08-24 21:18:51.000000 rp2-1.4.2/input/golden/test_large_input_hifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    62257 2022-08-11 23:20:16.000000 rp2-1.4.2/input/golden/test_large_input_lifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    30873 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_large_input_lifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    29407 2022-08-11 23:19:40.000000 rp2-1.4.2/input/golden/test_many_year_data_0_2016-12-31_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    20139 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_many_year_data_0_2016-12-31_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    31894 2022-08-11 23:19:40.000000 rp2-1.4.2/input/golden/test_many_year_data_0_2017-12-31_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    28051 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_many_year_data_0_2017-12-31_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    32967 2022-08-11 23:19:40.000000 rp2-1.4.2/input/golden/test_many_year_data_0_2018-12-31_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    35588 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_many_year_data_0_2018-12-31_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    34926 2022-08-11 23:19:40.000000 rp2-1.4.2/input/golden/test_many_year_data_0_2019-12-31_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    41201 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_many_year_data_0_2019-12-31_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    36006 2022-08-11 23:19:40.000000 rp2-1.4.2/input/golden/test_many_year_data_0_2020-12-31_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    41330 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_many_year_data_0_2020-12-31_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    33576 2022-08-11 23:19:40.000000 rp2-1.4.2/input/golden/test_many_year_data_2017-01-01_2019-12-31_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    38267 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_many_year_data_2017-01-01_2019-12-31_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    36146 2022-08-11 23:19:40.000000 rp2-1.4.2/input/golden/test_many_year_data_2017-01-01_infinity_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    41378 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_many_year_data_2017-01-01_infinity_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    31327 2022-08-11 23:19:40.000000 rp2-1.4.2/input/golden/test_many_year_data_2018-01-01_2019-12-31_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    27939 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_many_year_data_2018-01-01_2019-12-31_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    34044 2022-08-11 23:19:40.000000 rp2-1.4.2/input/golden/test_many_year_data_2018-01-01_infinity_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    33598 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_many_year_data_2018-01-01_infinity_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    29968 2022-08-11 23:19:40.000000 rp2-1.4.2/input/golden/test_many_year_data_2019-01-01_2019-12-31_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    20351 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_many_year_data_2019-01-01_2019-12-31_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    33128 2022-08-11 23:19:40.000000 rp2-1.4.2/input/golden/test_many_year_data_2019-01-01_infinity_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    26109 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_many_year_data_2019-01-01_infinity_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    30811 2022-08-11 23:19:40.000000 rp2-1.4.2/input/golden/test_many_year_data_2020-01-01_infinity_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    20491 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_many_year_data_2020-01-01_infinity_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    29617 2022-08-11 23:19:40.000000 rp2-1.4.2/input/golden/test_many_year_data_2021-01-01_infinity_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    20378 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_many_year_data_2021-01-01_infinity_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    37403 2022-08-11 23:19:40.000000 rp2-1.4.2/input/golden/test_many_year_data_fifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    41639 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_many_year_data_fifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    37172 2022-08-11 23:19:40.000000 rp2-1.4.2/input/golden/test_many_year_data_hifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    41412 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_many_year_data_hifo_tax_report_us.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    13247 2023-01-26 03:44:18.000000 rp2-1.4.2/input/golden/test_many_year_data_jp_en_fifo_open_positions.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    55100 2023-01-26 03:44:18.000000 rp2-1.4.2/input/golden/test_many_year_data_jp_en_fifo_rp2_full_report.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)   140328 2023-01-26 03:44:18.000000 rp2-1.4.2/input/golden/test_many_year_data_jp_en_fifo_tax_report_jp.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    37171 2022-08-11 23:19:40.000000 rp2-1.4.2/input/golden/test_many_year_data_lifo_rp2_full_report.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    41409 2022-08-09 16:07:45.000000 rp2-1.4.2/input/golden/test_many_year_data_lifo_tax_report_us.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    14261 2022-08-09 16:07:45.000000 rp2-1.4.2/input/test_bad_data.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    19489 2022-08-09 16:07:45.000000 rp2-1.4.2/input/test_data.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    16939 2022-08-11 07:44:08.000000 rp2-1.4.2/input/test_data2.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    13203 2022-08-09 16:07:45.000000 rp2-1.4.2/input/test_data3.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    17177 2022-10-16 20:30:25.000000 rp2-1.4.2/input/test_data4.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    22355 2022-08-28 18:26:57.000000 rp2-1.4.2/input/test_data_multi_method.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    34398 2022-08-09 16:07:45.000000 rp2-1.4.2/input/test_hifo.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    22517 2022-08-24 21:18:51.000000 rp2-1.4.2/input/test_hifo2.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    19469 2022-08-09 16:07:45.000000 rp2-1.4.2/input/test_many_year_data.ods
--rw-r--r--   0 marcoz     (501) staff       (20)      276 2022-08-09 16:07:45.000000 rp2-1.4.2/pyproject.toml
--rw-r--r--   0 marcoz     (501) staff       (20)     2397 2023-04-01 22:40:25.564901 rp2-1.4.2/setup.cfg
--rw-r--r--   0 marcoz     (501) staff       (20)       92 2022-08-09 16:07:45.000000 rp2-1.4.2/setup.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.505356 rp2-1.4.2/src/
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.538430 rp2-1.4.2/src/rp2/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2022-08-09 16:07:45.000000 rp2-1.4.2/src/rp2/__init__.py
--rw-r--r--   0 marcoz     (501) staff       (20)     4220 2023-02-05 15:27:07.000000 rp2-1.4.2/src/rp2/abstract_accounting_method.py
--rw-r--r--   0 marcoz     (501) staff       (20)     3563 2022-08-16 22:08:07.000000 rp2-1.4.2/src/rp2/abstract_country.py
--rw-r--r--   0 marcoz     (501) staff       (20)     3497 2022-08-21 05:49:15.000000 rp2-1.4.2/src/rp2/abstract_entry.py
--rw-r--r--   0 marcoz     (501) staff       (20)     7808 2022-08-09 16:07:45.000000 rp2-1.4.2/src/rp2/abstract_entry_set.py
--rw-r--r--   0 marcoz     (501) staff       (20)     1287 2022-08-28 06:04:46.000000 rp2-1.4.2/src/rp2/abstract_report_generator.py
--rw-r--r--   0 marcoz     (501) staff       (20)     5123 2022-08-09 16:07:45.000000 rp2-1.4.2/src/rp2/abstract_transaction.py
--rw-r--r--   0 marcoz     (501) staff       (20)     9504 2023-02-05 15:27:07.000000 rp2-1.4.2/src/rp2/accounting_engine.py
--rw-r--r--   0 marcoz     (501) staff       (20)     9018 2022-08-21 05:49:57.000000 rp2-1.4.2/src/rp2/balance.py
--rw-r--r--   0 marcoz     (501) staff       (20)    18064 2022-08-09 16:07:45.000000 rp2-1.4.2/src/rp2/computed_data.py
--rw-r--r--   0 marcoz     (501) staff       (20)    22917 2023-01-26 03:44:18.000000 rp2-1.4.2/src/rp2/configuration.py
--rw-r--r--   0 marcoz     (501) staff       (20)     7696 2022-08-28 04:49:33.000000 rp2-1.4.2/src/rp2/configuration_schema.py
--rw-r--r--   0 marcoz     (501) staff       (20)     4018 2022-08-09 16:07:45.000000 rp2-1.4.2/src/rp2/entry_types.py
--rw-r--r--   0 marcoz     (501) staff       (20)    10703 2023-02-05 15:27:07.000000 rp2-1.4.2/src/rp2/gain_loss.py
--rw-r--r--   0 marcoz     (501) staff       (20)    15603 2023-02-05 15:27:07.000000 rp2-1.4.2/src/rp2/gain_loss_set.py
--rw-r--r--   0 marcoz     (501) staff       (20)     8760 2022-08-09 16:07:45.000000 rp2-1.4.2/src/rp2/in_transaction.py
--rw-r--r--   0 marcoz     (501) staff       (20)     3799 2022-08-09 16:07:45.000000 rp2-1.4.2/src/rp2/input_data.py
--rw-r--r--   0 marcoz     (501) staff       (20)     6384 2022-08-09 16:07:45.000000 rp2-1.4.2/src/rp2/intra_transaction.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.549592 rp2-1.4.2/src/rp2/locales/
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.505628 rp2-1.4.2/src/rp2/locales/en/
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.549911 rp2-1.4.2/src/rp2/locales/en/LC_MESSAGES/
--rw-r--r--   0 marcoz     (501) staff       (20)      439 2022-08-17 07:16:50.000000 rp2-1.4.2/src/rp2/locales/en/LC_MESSAGES/messages.mo
--rw-r--r--   0 marcoz     (501) staff       (20)    13303 2023-01-26 03:44:18.000000 rp2-1.4.2/src/rp2/locales/en/LC_MESSAGES/messages.po
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.505821 rp2-1.4.2/src/rp2/locales/ja/
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.550219 rp2-1.4.2/src/rp2/locales/ja/LC_MESSAGES/
--rw-r--r--   0 marcoz     (501) staff       (20)      432 2022-08-17 07:16:50.000000 rp2-1.4.2/src/rp2/locales/ja/LC_MESSAGES/messages.mo
--rw-r--r--   0 marcoz     (501) staff       (20)    12932 2023-01-26 03:44:18.000000 rp2-1.4.2/src/rp2/locales/ja/LC_MESSAGES/messages.po
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.506043 rp2-1.4.2/src/rp2/locales/kl/
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.550555 rp2-1.4.2/src/rp2/locales/kl/LC_MESSAGES/
--rw-r--r--   0 marcoz     (501) staff       (20)    21586 2022-08-17 07:16:50.000000 rp2-1.4.2/src/rp2/locales/kl/LC_MESSAGES/messages.mo
--rw-r--r--   0 marcoz     (501) staff       (20)    22439 2023-01-26 03:44:18.000000 rp2-1.4.2/src/rp2/locales/kl/LC_MESSAGES/messages.po
--rw-r--r--   0 marcoz     (501) staff       (20)    12890 2023-01-26 03:44:18.000000 rp2-1.4.2/src/rp2/locales/messages.pot
--rw-r--r--   0 marcoz     (501) staff       (20)     1582 2022-08-16 04:35:48.000000 rp2-1.4.2/src/rp2/localization.py
--rw-r--r--   0 marcoz     (501) staff       (20)     1749 2022-08-18 07:00:53.000000 rp2-1.4.2/src/rp2/logger.py
--rw-r--r--   0 marcoz     (501) staff       (20)    16316 2023-02-05 15:27:07.000000 rp2-1.4.2/src/rp2/ods_parser.py
--rw-r--r--   0 marcoz     (501) staff       (20)     9463 2023-04-01 21:05:33.000000 rp2-1.4.2/src/rp2/out_transaction.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.550737 rp2-1.4.2/src/rp2/plugin/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2022-08-09 16:07:45.000000 rp2-1.4.2/src/rp2/plugin/__init__.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.551310 rp2-1.4.2/src/rp2/plugin/accounting_method/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2022-08-09 16:07:45.000000 rp2-1.4.2/src/rp2/plugin/accounting_method/__init__.py
--rw-r--r--   0 marcoz     (501) staff       (20)     2719 2023-01-26 03:44:18.000000 rp2-1.4.2/src/rp2/plugin/accounting_method/fifo.py
--rw-r--r--   0 marcoz     (501) staff       (20)     2817 2023-01-26 03:44:18.000000 rp2-1.4.2/src/rp2/plugin/accounting_method/hifo.py
--rw-r--r--   0 marcoz     (501) staff       (20)     2989 2023-01-26 03:44:18.000000 rp2-1.4.2/src/rp2/plugin/accounting_method/lifo.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.551755 rp2-1.4.2/src/rp2/plugin/country/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2022-08-09 16:07:45.000000 rp2-1.4.2/src/rp2/plugin/country/__init__.py
--rwxr-xr-x   0 marcoz     (501) staff       (20)     1964 2023-01-26 03:44:18.000000 rp2-1.4.2/src/rp2/plugin/country/jp.py
--rw-r--r--   0 marcoz     (501) staff       (20)     1820 2022-11-25 21:27:34.000000 rp2-1.4.2/src/rp2/plugin/country/us.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.552379 rp2-1.4.2/src/rp2/plugin/report/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2022-08-09 16:07:45.000000 rp2-1.4.2/src/rp2/plugin/report/__init__.py
--rw-r--r--   0 marcoz     (501) staff       (20)    11255 2023-02-05 15:27:07.000000 rp2-1.4.2/src/rp2/plugin/report/abstract_ods_generator.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.552711 rp2-1.4.2/src/rp2/plugin/report/data/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2022-08-09 16:07:45.000000 rp2-1.4.2/src/rp2/plugin/report/data/__init__.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.553500 rp2-1.4.2/src/rp2/plugin/report/data/jp/
--rwxr-xr-x   0 marcoz     (501) staff       (20)    38159 2023-01-26 03:44:18.000000 rp2-1.4.2/src/rp2/plugin/report/data/jp/template_rp2_full_report_en.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    38159 2023-01-26 03:44:18.000000 rp2-1.4.2/src/rp2/plugin/report/data/jp/template_rp2_full_report_kl.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    47091 2023-01-26 03:44:18.000000 rp2-1.4.2/src/rp2/plugin/report/data/jp/template_tax_report_jp_en.ods
--rwxr-xr-x   0 marcoz     (501) staff       (20)    47104 2023-01-26 03:44:18.000000 rp2-1.4.2/src/rp2/plugin/report/data/jp/template_tax_report_jp_kl.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    11390 2022-08-11 05:19:23.000000 rp2-1.4.2/src/rp2/plugin/report/data/template_open_positions.ods
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.553903 rp2-1.4.2/src/rp2/plugin/report/data/us/
--rw-r--r--   0 marcoz     (501) staff       (20)    19993 2023-01-26 03:44:18.000000 rp2-1.4.2/src/rp2/plugin/report/data/us/template_rp2_full_report_en.ods
--rw-r--r--   0 marcoz     (501) staff       (20)    34429 2022-08-11 22:14:20.000000 rp2-1.4.2/src/rp2/plugin/report/data/us/template_tax_report_us_en.ods
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.554283 rp2-1.4.2/src/rp2/plugin/report/jp/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-01-26 03:44:18.000000 rp2-1.4.2/src/rp2/plugin/report/jp/__init__.py
--rw-r--r--   0 marcoz     (501) staff       (20)    21841 2023-02-05 15:27:07.000000 rp2-1.4.2/src/rp2/plugin/report/jp/tax_report_jp.py
--rw-r--r--   0 marcoz     (501) staff       (20)    29447 2022-08-28 22:26:16.000000 rp2-1.4.2/src/rp2/plugin/report/open_positions.py
--rw-r--r--   0 marcoz     (501) staff       (20)    52316 2023-04-01 21:01:02.000000 rp2-1.4.2/src/rp2/plugin/report/rp2_full_report.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.554622 rp2-1.4.2/src/rp2/plugin/report/us/
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2022-08-09 16:07:45.000000 rp2-1.4.2/src/rp2/plugin/report/us/__init__.py
--rw-r--r--   0 marcoz     (501) staff       (20)     9717 2023-01-26 03:44:18.000000 rp2-1.4.2/src/rp2/plugin/report/us/tax_report_us.py
--rw-r--r--   0 marcoz     (501) staff       (20)        0 2022-08-09 16:07:45.000000 rp2-1.4.2/src/rp2/py.typed
--rw-r--r--   0 marcoz     (501) staff       (20)     4451 2023-01-26 03:44:18.000000 rp2-1.4.2/src/rp2/rp2_configuration_translator.py
--rw-r--r--   0 marcoz     (501) staff       (20)     5726 2022-08-09 16:07:45.000000 rp2-1.4.2/src/rp2/rp2_decimal.py
--rw-r--r--   0 marcoz     (501) staff       (20)     1236 2023-02-05 15:27:07.000000 rp2-1.4.2/src/rp2/rp2_error.py
--rw-r--r--   0 marcoz     (501) staff       (20)    14338 2023-04-01 22:28:32.000000 rp2-1.4.2/src/rp2/rp2_main.py
--rw-r--r--   0 marcoz     (501) staff       (20)     9893 2023-02-05 15:27:07.000000 rp2-1.4.2/src/rp2/tax_engine.py
--rw-r--r--   0 marcoz     (501) staff       (20)     1993 2022-08-09 16:07:45.000000 rp2-1.4.2/src/rp2/transaction_set.py
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.549419 rp2-1.4.2/src/rp2.egg-info/
--rw-r--r--   0 marcoz     (501) staff       (20)    33726 2023-04-01 22:40:25.000000 rp2-1.4.2/src/rp2.egg-info/PKG-INFO
--rw-r--r--   0 marcoz     (501) staff       (20)    10060 2023-04-01 22:40:25.000000 rp2-1.4.2/src/rp2.egg-info/SOURCES.txt
--rw-r--r--   0 marcoz     (501) staff       (20)        1 2023-04-01 22:40:25.000000 rp2-1.4.2/src/rp2.egg-info/dependency_links.txt
--rw-r--r--   0 marcoz     (501) staff       (20)      175 2023-04-01 22:40:25.000000 rp2-1.4.2/src/rp2.egg-info/entry_points.txt
--rw-r--r--   0 marcoz     (501) staff       (20)      239 2023-04-01 22:40:25.000000 rp2-1.4.2/src/rp2.egg-info/requires.txt
--rw-r--r--   0 marcoz     (501) staff       (20)        4 2023-04-01 22:40:25.000000 rp2-1.4.2/src/rp2.egg-info/top_level.txt
-drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-04-01 22:40:25.557791 rp2-1.4.2/tests/
--rw-r--r--   0 marcoz     (501) staff       (20)     4194 2023-01-26 03:44:18.000000 rp2-1.4.2/tests/abstract_test_ods_output_diff.py
--rw-r--r--   0 marcoz     (501) staff       (20)     4794 2023-01-26 03:44:18.000000 rp2-1.4.2/tests/ods_diff.py
--rw-r--r--   0 marcoz     (501) staff       (20)    38722 2022-09-03 21:19:18.000000 rp2-1.4.2/tests/rp2_test_output.py
--rw-r--r--   0 marcoz     (501) staff       (20)    37707 2023-01-26 03:44:18.000000 rp2-1.4.2/tests/test_configuration.py
--rw-r--r--   0 marcoz     (501) staff       (20)    14527 2022-09-03 21:21:38.000000 rp2-1.4.2/tests/test_gain_loss.py
--rw-r--r--   0 marcoz     (501) staff       (20)    19000 2023-01-26 03:44:18.000000 rp2-1.4.2/tests/test_gain_loss_set.py
--rw-r--r--   0 marcoz     (501) staff       (20)    34051 2022-09-03 21:21:03.000000 rp2-1.4.2/tests/test_in_transaction.py
--rw-r--r--   0 marcoz     (501) staff       (20)    16953 2023-02-05 15:27:07.000000 rp2-1.4.2/tests/test_input_parser.py
--rw-r--r--   0 marcoz     (501) staff       (20)    27920 2022-09-03 21:21:00.000000 rp2-1.4.2/tests/test_intra_transaction.py
--rw-r--r--   0 marcoz     (501) staff       (20)     5655 2023-02-05 15:27:07.000000 rp2-1.4.2/tests/test_large_input.py
--rw-r--r--   0 marcoz     (501) staff       (20)     2400 2023-01-26 03:44:18.000000 rp2-1.4.2/tests/test_localized_output.py
--rw-r--r--   0 marcoz     (501) staff       (20)    17380 2022-08-28 18:57:55.000000 rp2-1.4.2/tests/test_ods_output_diff.py
--rwxr-xr-x   0 marcoz     (501) staff       (20)     6036 2023-01-26 03:44:18.000000 rp2-1.4.2/tests/test_ods_output_diff_jp.py
--rw-r--r--   0 marcoz     (501) staff       (20)    25709 2022-09-03 21:20:44.000000 rp2-1.4.2/tests/test_out_transaction.py
--rw-r--r--   0 marcoz     (501) staff       (20)     7230 2022-08-09 16:07:45.000000 rp2-1.4.2/tests/test_rp2_decimal.py
--rw-r--r--   0 marcoz     (501) staff       (20)     5464 2023-01-26 03:44:18.000000 rp2-1.4.2/tests/test_tax_engine.py
--rw-r--r--   0 marcoz     (501) staff       (20)    14675 2022-09-03 21:20:12.000000 rp2-1.4.2/tests/test_transaction_set.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.338540 rp2-1.5.0/
+-rw-r--r--   0 marcoz     (501) staff       (20)    13978 2023-06-19 10:26:47.000000 rp2-1.5.0/CHANGELOG.md
+-rw-r--r--   0 marcoz     (501) staff       (20)     2761 2023-06-19 10:26:47.000000 rp2-1.5.0/CONTRIBUTING.md
+-rw-r--r--   0 marcoz     (501) staff       (20)    11357 2023-06-19 10:26:47.000000 rp2-1.5.0/LICENSE
+-rw-r--r--   0 marcoz     (501) staff       (20)      263 2023-06-19 10:26:47.000000 rp2-1.5.0/MANIFEST.in
+-rw-r--r--   0 marcoz     (501) staff       (20)    33890 2023-06-19 10:31:02.338637 rp2-1.5.0/PKG-INFO
+-rw-r--r--   0 marcoz     (501) staff       (20)    22251 2023-06-19 10:26:47.000000 rp2-1.5.0/README.dev.md
+-rw-r--r--   0 marcoz     (501) staff       (20)    18215 2023-06-19 10:26:47.000000 rp2-1.5.0/README.md
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.253499 rp2-1.5.0/config/
+-rw-r--r--   0 marcoz     (501) staff       (20)      636 2023-06-19 10:26:47.000000 rp2-1.5.0/config/crypto_example.ini
+-rw-r--r--   0 marcoz     (501) staff       (20)      762 2023-06-19 10:26:47.000000 rp2-1.5.0/config/test_bad_data.ini
+-rw-r--r--   0 marcoz     (501) staff       (20)      597 2023-06-19 10:26:47.000000 rp2-1.5.0/config/test_data.ini
+-rw-r--r--   0 marcoz     (501) staff       (20)      556 2023-06-19 10:26:47.000000 rp2-1.5.0/config/test_data4.ini
+-rw-r--r--   0 marcoz     (501) staff       (20)      675 2023-06-19 10:26:47.000000 rp2-1.5.0/config/test_data_multi_method.ini
+-rw-r--r--   0 marcoz     (501) staff       (20)      516 2023-06-19 10:26:47.000000 rp2-1.5.0/config/test_large_input.ini
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.254120 rp2-1.5.0/docs/
+-rw-r--r--   0 marcoz     (501) staff       (20)     2893 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/developer_faq.md
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.256130 rp2-1.5.0/docs/images/
+-rw-r--r--   0 marcoz     (501) staff       (20)    94354 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/images/input_spreadsheet.png
+-rw-r--r--   0 marcoz     (501) staff       (20)    66768 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/images/open_positions_asset.png
+-rw-r--r--   0 marcoz     (501) staff       (20)    87502 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/images/open_positions_asset_exchange.png
+-rw-r--r--   0 marcoz     (501) staff       (20)    16751 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/images/open_positions_input.png
+-rw-r--r--   0 marcoz     (501) staff       (20)   126454 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/images/rp2_full_report_output_in_out.png
+-rw-r--r--   0 marcoz     (501) staff       (20)    43264 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/images/rp2_full_report_output_summary.png
+-rw-r--r--   0 marcoz     (501) staff       (20)   229926 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/images/rp2_full_report_output_tax.png
+-rw-r--r--   0 marcoz     (501) staff       (20)   156431 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/images/rp2_header.png
+-rw-r--r--   0 marcoz     (501) staff       (20)    61646 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/images/tax_report_us_output_capital_gains.png
+-rw-r--r--   0 marcoz     (501) staff       (20)    24446 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/images/tax_report_us_output_interest.png
+-rw-r--r--   0 marcoz     (501) staff       (20)    15575 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/input_files.md
+-rw-r--r--   0 marcoz     (501) staff       (20)     8402 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/output_files.md
+-rw-r--r--   0 marcoz     (501) staff       (20)    27064 2023-06-19 10:26:47.000000 rp2-1.5.0/docs/user_faq.md
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.257687 rp2-1.5.0/input/
+-rw-r--r--   0 marcoz     (501) staff       (20)    18562 2023-06-19 10:26:47.000000 rp2-1.5.0/input/crypto_example.ods
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.277056 rp2-1.5.0/input/golden/
+-rw-r--r--   0 marcoz     (501) staff       (20)    39476 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/crypto_example_es_es_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    28227 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/crypto_example_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    27598 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/crypto_example_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    28267 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/crypto_example_hifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    27561 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/crypto_example_hifo_tax_report_us.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    12608 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/crypto_example_jp_en_fifo_open_positions.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    46257 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/crypto_example_jp_en_fifo_rp2_full_report.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    57435 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/crypto_example_jp_en_fifo_tax_report_jp.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    28267 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/crypto_example_lifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    27560 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/crypto_example_lifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    49835 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data2_es_es_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    38189 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data2_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    29720 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data2_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    37998 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data2_hifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    29513 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data2_hifo_tax_report_us.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    13044 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data2_jp_en_fifo_open_positions.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    56093 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data2_jp_en_fifo_rp2_full_report.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    76795 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data2_jp_en_fifo_tax_report_jp.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    38085 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data2_lifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    29748 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data2_lifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    31353 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_2019-12-01_2020-04-01_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    23272 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_2019-12-01_2020-04-01_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    31002 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_2019-12-01_2020-04-01_hifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    23181 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_2019-12-01_2020-04-01_hifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    30871 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_2019-12-01_2020-04-01_lifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    23125 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_2019-12-01_2020-04-01_lifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    43773 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_es_es_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    32272 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    23558 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    31831 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_hifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    23324 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_hifo_tax_report_us.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    12780 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_jp_en_fifo_open_positions.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    50213 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_jp_en_fifo_rp2_full_report.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    70575 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_jp_en_fifo_tax_report_jp.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    31703 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_lifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    23268 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data3_lifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    42672 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data4_es_es_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    31106 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data4_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    20872 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data4_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    30959 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data4_hifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    20807 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data4_hifo_tax_report_us.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    12317 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data4_jp_en_fifo_open_positions.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    49159 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data4_jp_en_fifo_rp2_full_report.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    59596 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data4_jp_en_fifo_tax_report_jp.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    30917 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data4_lifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    20784 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data4_lifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    47327 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_es_es_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    35766 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    29160 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    35784 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_hifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    28958 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_hifo_tax_report_us.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    13247 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_jp_en_fifo_open_positions.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    53767 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_jp_en_fifo_rp2_full_report.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    73415 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_jp_en_fifo_tax_report_jp.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    13272 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_jp_kl_fifo_open_positions.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    35898 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_jp_kl_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    35784 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_lifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    28957 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_lifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    44766 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_multi_method_mixed_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    23648 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_data_multi_method_mixed_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    31746 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_hifo2_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    18147 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_hifo2_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    32073 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_hifo2_hifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    18258 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_hifo2_hifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    32296 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_hifo2_lifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    18266 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_hifo2_lifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    36717 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_hifo_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    29719 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_hifo_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    36742 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_hifo_hifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    29722 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_hifo_hifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    36422 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_hifo_lifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    29521 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_hifo_lifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    63483 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_large_input_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    31061 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_large_input_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    61078 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_large_input_hifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    29914 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_large_input_hifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    62257 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_large_input_lifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    30873 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_large_input_lifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    29407 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_0_2016-12-31_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    20139 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_0_2016-12-31_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    31894 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_0_2017-12-31_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    28051 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_0_2017-12-31_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    32967 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_0_2018-12-31_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    35588 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_0_2018-12-31_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    34926 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_0_2019-12-31_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    41201 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_0_2019-12-31_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    36006 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_0_2020-12-31_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    41330 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_0_2020-12-31_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    33576 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2017-01-01_2019-12-31_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    38267 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2017-01-01_2019-12-31_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    36146 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2017-01-01_infinity_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    41378 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2017-01-01_infinity_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    31327 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2018-01-01_2019-12-31_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    27939 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2018-01-01_2019-12-31_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    34044 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2018-01-01_infinity_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    33598 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2018-01-01_infinity_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    29968 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2019-01-01_2019-12-31_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    20351 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2019-01-01_2019-12-31_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    33128 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2019-01-01_infinity_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    26109 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2019-01-01_infinity_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    30811 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2020-01-01_infinity_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    20491 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2020-01-01_infinity_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    29617 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2021-01-01_infinity_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    20378 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_2021-01-01_infinity_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    49022 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_es_es_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    37403 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_fifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    41639 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_fifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    37172 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_hifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    41412 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_hifo_tax_report_us.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    13247 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_jp_en_fifo_open_positions.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    55100 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_jp_en_fifo_rp2_full_report.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)   140328 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_jp_en_fifo_tax_report_jp.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    37171 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_lifo_rp2_full_report.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    41409 2023-06-19 10:26:47.000000 rp2-1.5.0/input/golden/test_many_year_data_lifo_tax_report_us.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    14261 2023-06-19 10:26:47.000000 rp2-1.5.0/input/test_bad_data.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    19489 2023-06-19 10:26:47.000000 rp2-1.5.0/input/test_data.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    16939 2023-06-19 10:26:47.000000 rp2-1.5.0/input/test_data2.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    13203 2023-06-19 10:26:47.000000 rp2-1.5.0/input/test_data3.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    17177 2023-06-19 10:26:47.000000 rp2-1.5.0/input/test_data4.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    22355 2023-06-19 10:26:47.000000 rp2-1.5.0/input/test_data_multi_method.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    34398 2023-06-19 10:26:47.000000 rp2-1.5.0/input/test_hifo.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    22517 2023-06-19 10:26:47.000000 rp2-1.5.0/input/test_hifo2.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    19469 2023-06-19 10:26:47.000000 rp2-1.5.0/input/test_many_year_data.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)      276 2023-06-19 10:26:47.000000 rp2-1.5.0/pyproject.toml
+-rw-r--r--   0 marcoz     (501) staff       (20)     2445 2023-06-19 10:31:02.340252 rp2-1.5.0/setup.cfg
+-rw-r--r--   0 marcoz     (501) staff       (20)       92 2023-06-19 10:26:47.000000 rp2-1.5.0/setup.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.243163 rp2-1.5.0/src/
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.281322 rp2-1.5.0/src/rp2/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/__init__.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     4220 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/abstract_accounting_method.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     3562 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/abstract_country.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     3497 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/abstract_entry.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     7808 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/abstract_entry_set.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     1287 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/abstract_report_generator.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     5123 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/abstract_transaction.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     9503 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/accounting_engine.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     9017 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/balance.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    18062 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/computed_data.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    22917 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/configuration.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     7696 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/configuration_schema.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     4748 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/entry_types.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    10702 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/gain_loss.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    15603 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/gain_loss_set.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     8760 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/in_transaction.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     3799 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/input_data.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     6384 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/intra_transaction.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.302824 rp2-1.5.0/src/rp2/locales/
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.243630 rp2-1.5.0/src/rp2/locales/en/
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.303293 rp2-1.5.0/src/rp2/locales/en/LC_MESSAGES/
+-rw-r--r--   0 marcoz     (501) staff       (20)      439 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/locales/en/LC_MESSAGES/messages.mo
+-rw-r--r--   0 marcoz     (501) staff       (20)    13689 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/locales/en/LC_MESSAGES/messages.po
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.243916 rp2-1.5.0/src/rp2/locales/es/
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.305827 rp2-1.5.0/src/rp2/locales/es/LC_MESSAGES/
+-rw-r--r--   0 marcoz     (501) staff       (20)    22319 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/locales/es/LC_MESSAGES/messages.mo
+-rw-r--r--   0 marcoz     (501) staff       (20)    23003 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/locales/es/LC_MESSAGES/messages.po
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.244196 rp2-1.5.0/src/rp2/locales/ja/
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.306506 rp2-1.5.0/src/rp2/locales/ja/LC_MESSAGES/
+-rw-r--r--   0 marcoz     (501) staff       (20)      432 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/locales/ja/LC_MESSAGES/messages.mo
+-rw-r--r--   0 marcoz     (501) staff       (20)    13318 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/locales/ja/LC_MESSAGES/messages.po
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.245072 rp2-1.5.0/src/rp2/locales/kl/
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.307057 rp2-1.5.0/src/rp2/locales/kl/LC_MESSAGES/
+-rw-r--r--   0 marcoz     (501) staff       (20)    22133 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/locales/kl/LC_MESSAGES/messages.mo
+-rw-r--r--   0 marcoz     (501) staff       (20)    23016 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/locales/kl/LC_MESSAGES/messages.po
+-rw-r--r--   0 marcoz     (501) staff       (20)    13276 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/locales/messages.pot
+-rw-r--r--   0 marcoz     (501) staff       (20)     1582 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/localization.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     1749 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/logger.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    16314 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/ods_parser.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     9463 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/out_transaction.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.311374 rp2-1.5.0/src/rp2/plugin/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/__init__.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.312372 rp2-1.5.0/src/rp2/plugin/accounting_method/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/accounting_method/__init__.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     2719 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/accounting_method/fifo.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     2817 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/accounting_method/hifo.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     2989 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/accounting_method/lifo.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.326641 rp2-1.5.0/src/rp2/plugin/country/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/country/__init__.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     1697 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/country/es.py
+-rwxr-xr-x   0 marcoz     (501) staff       (20)     1964 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/country/jp.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     1820 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/country/us.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.327924 rp2-1.5.0/src/rp2/plugin/report/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/__init__.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    11252 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/abstract_ods_generator.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.328144 rp2-1.5.0/src/rp2/plugin/report/data/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/data/__init__.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.330290 rp2-1.5.0/src/rp2/plugin/report/data/es/
+-rw-r--r--   0 marcoz     (501) staff       (20)    31636 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/data/es/template_open_positions_es.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    30525 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/data/es/template_rp2_full_report_es.ods
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.333893 rp2-1.5.0/src/rp2/plugin/report/data/jp/
+-rw-r--r--   0 marcoz     (501) staff       (20)    11390 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/data/jp/template_open_positions_en.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    11390 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/data/jp/template_open_positions_kl.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    38159 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/data/jp/template_rp2_full_report_en.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    38159 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/data/jp/template_rp2_full_report_kl.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    47091 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/data/jp/template_tax_report_jp_en.ods
+-rwxr-xr-x   0 marcoz     (501) staff       (20)    47104 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/data/jp/template_tax_report_jp_kl.ods
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.334420 rp2-1.5.0/src/rp2/plugin/report/data/us/
+-rw-r--r--   0 marcoz     (501) staff       (20)    11390 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/data/us/template_open_positions_en.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    19993 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/data/us/template_rp2_full_report_en.ods
+-rw-r--r--   0 marcoz     (501) staff       (20)    34429 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/data/us/template_tax_report_us_en.ods
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.334626 rp2-1.5.0/src/rp2/plugin/report/es/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/es/__init__.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.334893 rp2-1.5.0/src/rp2/plugin/report/jp/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/jp/__init__.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    21833 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/jp/tax_report_jp.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    29443 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/open_positions.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    52465 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/rp2_full_report.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.335273 rp2-1.5.0/src/rp2/plugin/report/us/
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/us/__init__.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     9714 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/plugin/report/us/tax_report_us.py
+-rw-r--r--   0 marcoz     (501) staff       (20)        0 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/py.typed
+-rw-r--r--   0 marcoz     (501) staff       (20)     4450 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/rp2_configuration_translator.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     5725 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/rp2_decimal.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     1236 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/rp2_error.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    14337 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/rp2_main.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     9893 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/tax_engine.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     1993 2023-06-19 10:26:47.000000 rp2-1.5.0/src/rp2/transaction_set.py
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.302432 rp2-1.5.0/src/rp2.egg-info/
+-rw-r--r--   0 marcoz     (501) staff       (20)    33890 2023-06-19 10:31:02.000000 rp2-1.5.0/src/rp2.egg-info/PKG-INFO
+-rw-r--r--   0 marcoz     (501) staff       (20)    10838 2023-06-19 10:31:02.000000 rp2-1.5.0/src/rp2.egg-info/SOURCES.txt
+-rw-r--r--   0 marcoz     (501) staff       (20)        1 2023-06-19 10:31:02.000000 rp2-1.5.0/src/rp2.egg-info/dependency_links.txt
+-rw-r--r--   0 marcoz     (501) staff       (20)      216 2023-06-19 10:31:02.000000 rp2-1.5.0/src/rp2.egg-info/entry_points.txt
+-rw-r--r--   0 marcoz     (501) staff       (20)      239 2023-06-19 10:31:02.000000 rp2-1.5.0/src/rp2.egg-info/requires.txt
+-rw-r--r--   0 marcoz     (501) staff       (20)        4 2023-06-19 10:31:02.000000 rp2-1.5.0/src/rp2.egg-info/top_level.txt
+drwxr-xr-x   0 marcoz     (501) staff       (20)        0 2023-06-19 10:31:02.338407 rp2-1.5.0/tests/
+-rw-r--r--   0 marcoz     (501) staff       (20)     4193 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/abstract_test_ods_output_diff.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     4792 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/ods_diff.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    38722 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/rp2_test_output.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    37707 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_configuration.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    14527 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_gain_loss.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    19000 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_gain_loss_set.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    34051 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_in_transaction.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    16951 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_input_parser.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    27920 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_intra_transaction.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     5653 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_large_input.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     2399 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_localized_output.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    17379 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_ods_output_diff.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     4150 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_ods_output_diff_es.py
+-rwxr-xr-x   0 marcoz     (501) staff       (20)     6035 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_ods_output_diff_jp.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    25709 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_out_transaction.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     7230 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_rp2_decimal.py
+-rw-r--r--   0 marcoz     (501) staff       (20)     5464 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_tax_engine.py
+-rw-r--r--   0 marcoz     (501) staff       (20)    14675 2023-06-19 10:26:47.000000 rp2-1.5.0/tests/test_transaction_set.py
```

### Comparing `rp2-1.4.2/CHANGELOG.md` & `rp2-1.5.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,17 @@
 <!--- distributed under the License is distributed on an "AS IS" BASIS, --->
 <!--- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. --->
 <!--- See the License for the specific language governing permissions and --->
 <!--- limitations under the License. --->
 
 # RP2 Change Log
 
+## 1.5.0
+* added support for Spain (see #97)
+
 ## 1.4.2
 * fixed small bug in rp2_full_report generator: OUT transactions had slightly incorrect fiat_out field. The displayed value was fiat_out_no_fee - fiat fee, instead of fiat_out_no_fee. This bug didn't affect actual tax computation or the tax_report output: it only affected the fiat_out field in the OUT table of rp2_full_report.
 
 ## 1.4.1
 * added new RP2RuntimeError to handle non-recoverable problems without using Exception
 
 ## 1.4.0
```

### Comparing `rp2-1.4.2/CONTRIBUTING.md` & `rp2-1.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/LICENSE` & `rp2-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/PKG-INFO` & `rp2-1.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: rp2
-Version: 1.4.2
+Version: 1.5.0
 Summary: Privacy-focused, free, non-commercial, open-source, community-driven cryptocurrency tax calculator: it handles multiple coins/exchanges and computes long/short-term capital gains, cost bases, in/out lot relationships/fractioning, and account balances. It supports the FIFO accounting method, it features transparent computation for easy result verification, and it generates reports that tax accountants can understand, even if they are not cryptocurrency experts (e.g. form 8949).
 Home-page: https://github.com/eprbell/rp2
 Author: eprbell
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/eprbell/rp2
 Project-URL: Developer Documentation, https://github.com/eprbell/rp2/blob/main/README.dev.md
 Project-URL: User Documentation, https://github.com/eprbell/rp2/blob/main/README.md
 Project-URL: Contact, https://eprbell.github.io/eprbell/about.html
-Keywords: accounting,altcoin,bitcoin,BTC,capital gains,cost basis,crypto,cryptocurrency,ETH,ethereum,finance,form 8949,NFT,privacy,wallet,tax
+Keywords: accounting,altcoin,bitcoin,BTC,capital gains,cost basis,crypto,cryptocurrency,DeFi,ETH,ethereum,finance,form 8949,NFT,privacy,wallet,tax
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -37,25 +37,25 @@
 <!--- distributed under the License is distributed on an "AS IS" BASIS, --->
 <!--- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. --->
 <!--- See the License for the specific language governing permissions and --->
 <!--- limitations under the License. --->
 
 ![RP2 Logo](https://raw.githubusercontent.com/eprbell/rp2/main/docs/images/rp2_header.png)
 
-# RP2 v1.4.2
+# RP2 v1.5.0
 Privacy-focused, free, powerful crypto tax calculator
 
 [![Static Analysis / Main Branch](https://github.com/eprbell/rp2/actions/workflows/static_analysis.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/static_analysis.yml)
 [![Documentation Check / Main Branch](https://github.com/eprbell/rp2/actions/workflows/documentation_check.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/documentation_check.yml)
 [![Unix Unit Tests / Main Branch](https://github.com/eprbell/rp2/actions/workflows/unix_unit_tests.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/unix_unit_tests.yml)
 [![Windows Unit Tests / Main Branch](https://github.com/eprbell/rp2/actions/workflows/windows_unit_tests.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/windows_unit_tests.yml)
 [![CodeQL/Main Branch](https://github.com/eprbell/rp2/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/codeql-analysis.yml)
-
+<!-- markdown-link-check-disable -->
 [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=I%20use%20RP2,%20the%20privacy-focused,%20open%20source,%20free,%20non-commercial%20crypto%20tax%20calculator&url=https://github.com/eprbell/rp2/?anything)
-
+<!-- markdown-link-check-enable -->
 ## Table of Contents
 * **[Introduction](https://github.com/eprbell/rp2/blob/main/README.md#introduction)**
   * [How RP2 Operates](https://github.com/eprbell/rp2/blob/main/README.md#how-rp2-operates)
 * **[License](https://github.com/eprbell/rp2/blob/main/README.md#license)**
 * **[Download](https://github.com/eprbell/rp2/blob/main/README.md#download)**
 * **[Installation](https://github.com/eprbell/rp2/blob/main/README.md#installation)**
   * [Ubuntu Linux](https://github.com/eprbell/rp2/blob/main/README.md#installation-on-ubuntu-linux)
@@ -69,30 +69,30 @@
 * **[Reporting Bugs](https://github.com/eprbell/rp2/blob/main/README.md#reporting-bugs)**
 * **[Contributing](https://github.com/eprbell/rp2/blob/main/README.md#contributing)**
 * **[Developer Documentation](https://github.com/eprbell/rp2/blob/main/README.md#developer-documentation)**
 * **[Frequently Asked Questions](https://github.com/eprbell/rp2/blob/main/README.md#frequently-asked-questions)**
 * **[Change Log](https://github.com/eprbell/rp2/blob/main/README.md#change-log)**
 
 ## Introduction
-[RP2](https://github.com/eprbell/rp2) is a privacy-focused, free, non-commercial, open-source, community-driven cryptocurrency tax calculator. Preparing crypto taxes can be a daunting and error-prone task, especially if multiple transactions, coins, exchanges and wallets are involved. This task could be delegated to a crypto tax preparation service, but many crypto users value their privacy and prefer not to send their transaction information to third parties unnecessarily. Additionally, many of these services cost money. RP2 solves all of these problems:
+[RP2](https://github.com/eprbell/rp2) is a privacy-focused, free, non-commercial, open-source, community-driven cryptocurrency tax calculator for multiple countries (currently US, Japan and Spain are supported). Preparing crypto taxes can be a daunting and error-prone task, especially if multiple transactions, coins, exchanges and wallets are involved. This task could be delegated to a crypto tax preparation service, but many crypto users value their privacy and prefer not to send their transaction information to third parties unnecessarily. Additionally, many of these services cost money. RP2 solves all of these problems:
 * it manages the complexity related to coin flows and tax calculation and it generates [reports that accountants can understand](https://github.com/eprbell/rp2/blob/main/docs/output_files.md#advisor-friendly-report-tax-report-us-output) (in the format of form 8949, for the US case), even if they are not cryptocurrency experts;
 * it prioritizes user privacy by storing crypto transactions and tax results on the user's computer and not sending them anywhere else;
 * it's 100% free, open-source and non-commercial.
 
 This means that with RP2 there are no transaction limits, no premium versions, no payment requests, no personal data sent to a server (at risk of being hacked), no account creation, no unauditable source code.
 
 Another unique advantage of RP2 is [transparent computation](https://github.com/eprbell/rp2/blob/main/docs/output_files.md#transparent-computation-rp2-full-report-output): RP2 generates full computation details for every lot fraction, so that it's possible to:
 * verify step-by-step how RP2 reaches the final result;
 * track down every lot fraction and its accounting details, in case of an audit.
 
-RP2 currently supports the [FIFO](https://www.investopedia.com/terms/f/fifo.asp) accounting method for US taxes and the Total Average Method for Japanese taxes.
+RP2 currently supports the [FIFO](https://www.investopedia.com/terms/f/fifo.asp) accounting method for US and Spanish taxes and the Total Average Method for Japanese taxes.
 
 RP2 reads a configuration file and an input spreadsheet containing crypto transactions. These [input files](https://github.com/eprbell/rp2/blob/main/docs/input_files.md) can be generated either manually or automatically using [DaLI](https://github.com/eprbell/dali-rp2), a RP2 data loader and input generator (which is also privacy-focused, free, non-commercial, open-source and community-driven). After parsing the input, RP2 uses high-precision math to calculate long/short term capital gains, cost bases, balances, average price, in/out lot relationships/fractions, and finally it generates [output files](https://github.com/eprbell/rp2/blob/main/docs/output_files.md).
 
-RP2 has a programmable plugin architecture for [output generators](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-a-new-report-generator), [accounting methods](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-a-new-accounting-method) and [countries](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-support-for-a-new-country) (currently US and Japan are supported). The builtin output generator plugins are in part generic and in part country-specific, but RP2's architecture makes it possible to contribute additional generators for different countries or for different country-based cases. The builtin output generator plugins are:
+RP2 has a programmable plugin architecture for [output generators](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-a-new-report-generator), [accounting methods](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-a-new-accounting-method) and [countries](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-support-for-a-new-country). The builtin output generator plugins are in part generic and in part country-specific, but RP2's architecture makes it possible to contribute additional generators for different countries or for different country-based cases. The builtin output generator plugins are:
 * tax_report_us: generates a US-specific tax report meant to be read by tax preparers (in the format of form 8949);
 * tax_report_jp: generates a Japan-specific tax report meant to be read by tax preparers;
 * rp2_full_report: generates a comprehensive report (valid for any country), with complete transaction history, lot relationships/fractions and computation details;
 * open_positions: geterates a report (valid for any country) on assets with non-zero crypto balance: unrealized gains / losses, portfolio weighting, and more.
 
 RP2 has extensive [unit test](https://github.com/eprbell/rp2/tree/main/tests/) coverage to reduce the risk of regression.
 
@@ -252,14 +252,17 @@
 <!--- distributed under the License is distributed on an "AS IS" BASIS, --->
 <!--- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. --->
 <!--- See the License for the specific language governing permissions and --->
 <!--- limitations under the License. --->
 
 # RP2 Change Log
 
+## 1.5.0
+* added support for Spain (see #97)
+
 ## 1.4.2
 * fixed small bug in rp2_full_report generator: OUT transactions had slightly incorrect fiat_out field. The displayed value was fiat_out_no_fee - fiat fee, instead of fiat_out_no_fee. This bug didn't affect actual tax computation or the tax_report output: it only affected the fiat_out field in the OUT table of rp2_full_report.
 
 ## 1.4.1
 * added new RP2RuntimeError to handle non-recoverable problems without using Exception
 
 ## 1.4.0
```

### Comparing `rp2-1.4.2/README.dev.md` & `rp2-1.5.0/README.dev.md`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 <!--- Unless required by applicable law or agreed to in writing, software --->
 <!--- distributed under the License is distributed on an "AS IS" BASIS, --->
 <!--- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. --->
 <!--- See the License for the specific language governing permissions and --->
 <!--- limitations under the License. --->
 
-# RP2 v1.4.2 Developer Guide
+# RP2 v1.5.0 Developer Guide
 [![Static Analysis / Main Branch](https://github.com/eprbell/rp2/actions/workflows/static_analysis.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/static_analysis.yml)
 [![Documentation Check / Main Branch](https://github.com/eprbell/rp2/actions/workflows/documentation_check.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/documentation_check.yml)
 [![Unix Unit Tests / Main Branch](https://github.com/eprbell/rp2/actions/workflows/unix_unit_tests.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/unix_unit_tests.yml)
 [![Windows Unit Tests / Main Branch](https://github.com/eprbell/rp2/actions/workflows/windows_unit_tests.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/windows_unit_tests.yml)
 [![CodeQL/Main Branch](https://github.com/eprbell/rp2/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/codeql-analysis.yml)
 
 ## Table of Contents
@@ -178,15 +178,15 @@
 * security check: `bandit -r src`
 * reformat code: `black src tests`
 * sort imports: `isort .`
 * run pre-commit tests without committing: `pre-commit run --all-files`
 
 Logs are stored in the `log` directory. To generate debug logs, prepend the command line with `LOG_LEVEL=DEBUG`, e.g.:
 ```
-LOG_LEVEL=DEBUG bin/rp2_us -o output -p crypto_example_ config/crypto_example.ini input/crypto_example.ods
+LOG_LEVEL=DEBUG rp2_us -o output -p crypto_example_ config/crypto_example.ini input/crypto_example.ods
 ```
 
 ### Unit Tests
 RP2 has considerable unit test coverage to reduce the risk of regression. Unit tests are in the [tests](tests) directory. Please add unit tests for any new code.
 
 ## Creating a Release
 This section is for project maintainers.
```

### Comparing `rp2-1.4.2/README.md` & `rp2-1.5.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -10,25 +10,25 @@
 <!--- distributed under the License is distributed on an "AS IS" BASIS, --->
 <!--- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. --->
 <!--- See the License for the specific language governing permissions and --->
 <!--- limitations under the License. --->
 
 ![RP2 Logo](https://raw.githubusercontent.com/eprbell/rp2/main/docs/images/rp2_header.png)
 
-# RP2 v1.4.2
+# RP2 v1.5.0
 Privacy-focused, free, powerful crypto tax calculator
 
 [![Static Analysis / Main Branch](https://github.com/eprbell/rp2/actions/workflows/static_analysis.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/static_analysis.yml)
 [![Documentation Check / Main Branch](https://github.com/eprbell/rp2/actions/workflows/documentation_check.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/documentation_check.yml)
 [![Unix Unit Tests / Main Branch](https://github.com/eprbell/rp2/actions/workflows/unix_unit_tests.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/unix_unit_tests.yml)
 [![Windows Unit Tests / Main Branch](https://github.com/eprbell/rp2/actions/workflows/windows_unit_tests.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/windows_unit_tests.yml)
 [![CodeQL/Main Branch](https://github.com/eprbell/rp2/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/codeql-analysis.yml)
-
+<!-- markdown-link-check-disable -->
 [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=I%20use%20RP2,%20the%20privacy-focused,%20open%20source,%20free,%20non-commercial%20crypto%20tax%20calculator&url=https://github.com/eprbell/rp2/?anything)
-
+<!-- markdown-link-check-enable -->
 ## Table of Contents
 * **[Introduction](https://github.com/eprbell/rp2/blob/main/README.md#introduction)**
   * [How RP2 Operates](https://github.com/eprbell/rp2/blob/main/README.md#how-rp2-operates)
 * **[License](https://github.com/eprbell/rp2/blob/main/README.md#license)**
 * **[Download](https://github.com/eprbell/rp2/blob/main/README.md#download)**
 * **[Installation](https://github.com/eprbell/rp2/blob/main/README.md#installation)**
   * [Ubuntu Linux](https://github.com/eprbell/rp2/blob/main/README.md#installation-on-ubuntu-linux)
@@ -42,30 +42,30 @@
 * **[Reporting Bugs](https://github.com/eprbell/rp2/blob/main/README.md#reporting-bugs)**
 * **[Contributing](https://github.com/eprbell/rp2/blob/main/README.md#contributing)**
 * **[Developer Documentation](https://github.com/eprbell/rp2/blob/main/README.md#developer-documentation)**
 * **[Frequently Asked Questions](https://github.com/eprbell/rp2/blob/main/README.md#frequently-asked-questions)**
 * **[Change Log](https://github.com/eprbell/rp2/blob/main/README.md#change-log)**
 
 ## Introduction
-[RP2](https://github.com/eprbell/rp2) is a privacy-focused, free, non-commercial, open-source, community-driven cryptocurrency tax calculator. Preparing crypto taxes can be a daunting and error-prone task, especially if multiple transactions, coins, exchanges and wallets are involved. This task could be delegated to a crypto tax preparation service, but many crypto users value their privacy and prefer not to send their transaction information to third parties unnecessarily. Additionally, many of these services cost money. RP2 solves all of these problems:
+[RP2](https://github.com/eprbell/rp2) is a privacy-focused, free, non-commercial, open-source, community-driven cryptocurrency tax calculator for multiple countries (currently US, Japan and Spain are supported). Preparing crypto taxes can be a daunting and error-prone task, especially if multiple transactions, coins, exchanges and wallets are involved. This task could be delegated to a crypto tax preparation service, but many crypto users value their privacy and prefer not to send their transaction information to third parties unnecessarily. Additionally, many of these services cost money. RP2 solves all of these problems:
 * it manages the complexity related to coin flows and tax calculation and it generates [reports that accountants can understand](https://github.com/eprbell/rp2/blob/main/docs/output_files.md#advisor-friendly-report-tax-report-us-output) (in the format of form 8949, for the US case), even if they are not cryptocurrency experts;
 * it prioritizes user privacy by storing crypto transactions and tax results on the user's computer and not sending them anywhere else;
 * it's 100% free, open-source and non-commercial.
 
 This means that with RP2 there are no transaction limits, no premium versions, no payment requests, no personal data sent to a server (at risk of being hacked), no account creation, no unauditable source code.
 
 Another unique advantage of RP2 is [transparent computation](https://github.com/eprbell/rp2/blob/main/docs/output_files.md#transparent-computation-rp2-full-report-output): RP2 generates full computation details for every lot fraction, so that it's possible to:
 * verify step-by-step how RP2 reaches the final result;
 * track down every lot fraction and its accounting details, in case of an audit.
 
-RP2 currently supports the [FIFO](https://www.investopedia.com/terms/f/fifo.asp) accounting method for US taxes and the Total Average Method for Japanese taxes.
+RP2 currently supports the [FIFO](https://www.investopedia.com/terms/f/fifo.asp) accounting method for US and Spanish taxes and the Total Average Method for Japanese taxes.
 
 RP2 reads a configuration file and an input spreadsheet containing crypto transactions. These [input files](https://github.com/eprbell/rp2/blob/main/docs/input_files.md) can be generated either manually or automatically using [DaLI](https://github.com/eprbell/dali-rp2), a RP2 data loader and input generator (which is also privacy-focused, free, non-commercial, open-source and community-driven). After parsing the input, RP2 uses high-precision math to calculate long/short term capital gains, cost bases, balances, average price, in/out lot relationships/fractions, and finally it generates [output files](https://github.com/eprbell/rp2/blob/main/docs/output_files.md).
 
-RP2 has a programmable plugin architecture for [output generators](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-a-new-report-generator), [accounting methods](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-a-new-accounting-method) and [countries](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-support-for-a-new-country) (currently US and Japan are supported). The builtin output generator plugins are in part generic and in part country-specific, but RP2's architecture makes it possible to contribute additional generators for different countries or for different country-based cases. The builtin output generator plugins are:
+RP2 has a programmable plugin architecture for [output generators](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-a-new-report-generator), [accounting methods](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-a-new-accounting-method) and [countries](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-support-for-a-new-country). The builtin output generator plugins are in part generic and in part country-specific, but RP2's architecture makes it possible to contribute additional generators for different countries or for different country-based cases. The builtin output generator plugins are:
 * tax_report_us: generates a US-specific tax report meant to be read by tax preparers (in the format of form 8949);
 * tax_report_jp: generates a Japan-specific tax report meant to be read by tax preparers;
 * rp2_full_report: generates a comprehensive report (valid for any country), with complete transaction history, lot relationships/fractions and computation details;
 * open_positions: geterates a report (valid for any country) on assets with non-zero crypto balance: unrealized gains / losses, portfolio weighting, and more.
 
 RP2 has extensive [unit test](https://github.com/eprbell/rp2/tree/main/tests/) coverage to reduce the risk of regression.
```

### Comparing `rp2-1.4.2/config/crypto_example.ini` & `rp2-1.5.0/config/crypto_example.ini`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/config/test_bad_data.ini` & `rp2-1.5.0/config/test_bad_data.ini`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/config/test_data.ini` & `rp2-1.5.0/config/test_data.ini`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/config/test_data4.ini` & `rp2-1.5.0/config/test_data4.ini`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/config/test_data_multi_method.ini` & `rp2-1.5.0/config/test_data_multi_method.ini`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/config/test_large_input.ini` & `rp2-1.5.0/config/test_large_input.ini`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/docs/developer_faq.md` & `rp2-1.5.0/docs/developer_faq.md`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/docs/images/input_spreadsheet.png` & `rp2-1.5.0/docs/images/input_spreadsheet.png`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/docs/images/open_positions_asset.png` & `rp2-1.5.0/docs/images/open_positions_asset.png`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/docs/images/open_positions_asset_exchange.png` & `rp2-1.5.0/docs/images/open_positions_asset_exchange.png`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/docs/images/open_positions_input.png` & `rp2-1.5.0/docs/images/open_positions_input.png`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/docs/images/rp2_full_report_output_in_out.png` & `rp2-1.5.0/docs/images/rp2_full_report_output_in_out.png`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/docs/images/rp2_full_report_output_summary.png` & `rp2-1.5.0/docs/images/rp2_full_report_output_summary.png`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/docs/images/rp2_full_report_output_tax.png` & `rp2-1.5.0/docs/images/rp2_full_report_output_tax.png`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/docs/images/rp2_header.png` & `rp2-1.5.0/docs/images/rp2_header.png`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/docs/images/tax_report_us_output_capital_gains.png` & `rp2-1.5.0/docs/images/tax_report_us_output_capital_gains.png`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/docs/images/tax_report_us_output_interest.png` & `rp2-1.5.0/docs/images/tax_report_us_output_interest.png`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/docs/input_files.md` & `rp2-1.5.0/docs/input_files.md`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/docs/output_files.md` & `rp2-1.5.0/docs/output_files.md`

 * *Files 4% similar despite different names*

```diff
@@ -19,17 +19,18 @@
 * **[Transparent Computation (RP2 Full Output Report)](#transparent-computation-rp2-full-report-output)**
   * [Hyperlinks](#hyperlinks)
 * **[Advisor-Friendly Report (Tax Report US Output)](#advisor-friendly-report-tax-report-us-output)**
 * **[NTA-Friendly Report (Tax Report Japan Output)](#nta-friendly-report-tax-report-japan-output)**
 * **[Unrealized Gains (Open Positions Report Output)](#unrealized-gains-open-positions-report-output)**
 
 ## Introduction
-RP2 generates output files by running the report plugins. It comes with two builtin plugins for US taxes:
-* *rp2_full_report*: a comprehensive report containing full transaction history with hyperlinks, long/short capital gains, cost bases, balances, average price, in/out lot relationships and fractions. See [crypto_example_fifo_rp2_full_report.ods](../input/golden/crypto_example_fifo_rp2_full_report.ods) (an example of this output for input file [crypto_example.ods](../input/crypto_example.ods)) and screenshots further down in this document.
-* *tax_report_us*: a US-specific report that can be used to fill form 8949, etc. See [crypto_example_fifo_tax_report_us.ods](../input/golden/crypto_example_fifo_tax_report_us.ods) (an example of this output for input file [crypto_example.ods](../input/crypto_example.ods)) and screenshots further down in this document.
+RP2 generates output files by running the report plugins:
+* *tax_report_\** (US and Japan only). This is a tax-advisor-friendly report that can be given to a tax professional (not necessarily one that specializes in crypto).
+* *rp2_full_report* (all countries): a comprehensive report containing full transaction history with hyperlinks, long/short capital gains, cost bases, balances, average price, in/out lot relationships and fractions. This report can be useful in case of audit because it contains the complete history of coin movements and fractioning. See [crypto_example_fifo_rp2_full_report.ods](../input/golden/crypto_example_fifo_rp2_full_report.ods) (an example of this output for input file [crypto_example.ods](../input/crypto_example.ods)) and screenshots further down in this document.
+* *open_positions* (all countries): a report on assets with non-zero crypto balance: unrealized gains / losses, portfolio weighting, and more.
 
 After running RP2, the output files can be found in the `output` directory or in the directory specified with the -o command line option.
 
 ## Transparent Computation (RP2 Full Report Output)
 The rp2_full_report.ods output file is a comprehensive, ODS-format report containing full details about the computed taxes: it can be used to follow step-by-step the process RP2 uses to produce results and verify them. It contains:
 * a Legend sheet containing accounting method information and the meaning of each column and keyword
 * a Summary sheet containing total short/long term capital gains per year, per cryptocurrency. Here follows an example of this sheet: ![RP2 full report summary example](images/rp2_full_report_output_summary.png)
@@ -39,14 +40,16 @@
 
 ### Hyperlinks
 The RP2 Full Report contains hyperlinks to facilitate navigation: in LibreOffice, CTRL-click (on Mac, Command-click) on a cell to jump to the target. The following content is hyperlinked:
   * taxable events and acquired lots in *cryptocurrency* Tax sheet are hyperlinked to their definition line in the cryptocurrency* In-Out sheet;
   * summary lines in the Summary sheet are now hyperlinked to the first line of the given year in the *cryptocurrency* Tax sheet.
 
 ## Advisor-Friendly Report (Tax Report US Output)
+This report can be used to fill form 8949, etc: see [crypto_example_fifo_tax_report_us.ods](../input/golden/crypto_example_fifo_tax_report_us.ods) (an example of this output for input file [crypto_example.ods](../input/crypto_example.ods)) and screenshots further down.
+
 The tax_report_us.ods output file contains a legend sheet and a sheet per taxable event type (if there are no taxable events for a given event type, its respective sheet is not generated):
 * Airdrops;
 * Capital Gains (triggered by cryptocurrency sales);
 * Donations (cryptocurrency given to a qualified charity);
 * Gifts (cryptocurrency gifted to a friends or family);
 * Hard Forks;
 * Income;
@@ -64,22 +67,22 @@
 
 ![tax report us output capital gains](images/tax_report_us_output_capital_gains.png)
 
 And an example of the Interest sheet:
 
 ![tax report us output interest](images/tax_report_us_output_interest.png)
 
-## NTA-friendly Report (Tax Report Japan Ouput)
+## NTA-friendly Report (Tax Report Japan Output)
 The tax_report_jp.ods output file contains a legend sheet, a summary sheet for every year, and a calculation sheet per asset and year.
 
 The NTA (National Tax Agency) provides an excel spreadsheet for calculating the total average of each crypto asset per year. This report generates a similar report and can be optionally submitted with an individual's taxes or provided to the NTA if requested.
 
 The summary sheet contains the total for the tax year. This is what is normally reported as "miscellaneous income" (雑所得). However, it may be reported as business income in certain circumstances. Please do your own research.
 
 ## Unrealized Gains (Open Positions Report Output)
-The open_positions_us.ods output file is an ODS-format spreadsheet designed to provide information on assets with non-zero crypto balances including gains and losses.
+The open_positions_\*.ods output file is an ODS-format spreadsheet designed to provide information on assets with non-zero crypto balances including gains and losses.
 
 The report contains:
 * a Legend sheet containing the accounting method and the meaning of each column and keyword
 * the Input sheet for entering current asset values (or asset values on a given date to be used for the calculations per user requirements). ![Open Positions input tab example](images/open_positions_input.png)
 * the Asset sheet which among other things shows the crypto balance, cost basis information (by unit and in whole) and portfolio weighting of each asset as well as the unrealized / market value and the gains / loss data in fiat and percentage terms in addition to further breakdowns. This tab summarizes the information by asset and holder. ![Open Positions asset tab example](images/open_positions_asset.png)
 * The Asset - Exchange sheet provides the same information as the asset tab, but further breaks the information down by exchange. ![Open Positions asset exchange tab example](images/open_positions_asset_exchange.png)
```

### Comparing `rp2-1.4.2/docs/user_faq.md` & `rp2-1.5.0/docs/user_faq.md`

 * *Files 0% similar despite different names*

```diff
@@ -81,21 +81,21 @@
 ### What if I Don't Have the Spot Price for Some Transactions?
 In some cases exchange reports miss spot price information. In such situations you can retrieve historical price data from [Yahoo](https://finance.yahoo.com/quote/BTC-USD/history/), [CoinMarketCap](https://coinmarketcap.com/currencies/bitcoin/historical-data/) and others.
 
 ### What Tokens Does RP2 Support?
 The user adds the tokens to the `assets` field of the [config file](input_files.md#the-config-file): RP2 accepts as valid all the tokens present in this field. See also the question on [writing a config file from scratch](#can-i-avoid-writing-a-config-file-from-scratch).
 
 ### What Accounting Methods Are Supported?
-Currently only the [FIFO](https://www.investopedia.com/terms/f/fifo.asp) accounting method is supported for US taxes. Only the Total Average Method is supported for Japanese taxes. 
+Currently only the [FIFO](https://www.investopedia.com/terms/f/fifo.asp) accounting method is supported for US and Spanish taxes. Only the Total Average Method is supported for Japanese taxes.
 
 ### Can I Change Accounting Method?
 No, currently RP2 only supports FIFO for US taxes and the Total Average Method for JP taxes.
 
 ### What Countries Are Supported?
-Currently the US and Japan are supported, but more countries are being added. As new countries are added this FAQ will be updated.
+Currently the US, Japan and Spain are supported, but more countries are being added. As new countries are added this FAQ will be updated.
 
 ### How to Switch from Another Tax Software to RP2?
 In other words, how does RP2 handle transactions that were managed by other software in previous years? In this case the user can just leave out from the RP2 input spreadsheet the transactions/lots that were already sold in previous years.
 
 E.g. suppose the user's first year of trading BTC was 2020 and these were their transactions:
 
 <ol type="a">
```

### Comparing `rp2-1.4.2/input/crypto_example.ods` & `rp2-1.5.0/input/crypto_example.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/crypto_example_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/crypto_example_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/crypto_example_fifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/crypto_example_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/crypto_example_hifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/crypto_example_hifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/crypto_example_hifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/crypto_example_hifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/crypto_example_jp_en_fifo_open_positions.ods` & `rp2-1.5.0/input/golden/crypto_example_jp_en_fifo_open_positions.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/crypto_example_jp_en_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/crypto_example_jp_en_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/crypto_example_jp_en_fifo_tax_report_jp.ods` & `rp2-1.5.0/input/golden/crypto_example_jp_en_fifo_tax_report_jp.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/crypto_example_lifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/crypto_example_lifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/crypto_example_lifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/crypto_example_lifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data2_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_data2_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data2_fifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_data2_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data2_hifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_data2_hifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data2_hifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_data2_hifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data2_jp_en_fifo_open_positions.ods` & `rp2-1.5.0/input/golden/test_data2_jp_en_fifo_open_positions.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data2_jp_en_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_data2_jp_en_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data2_jp_en_fifo_tax_report_jp.ods` & `rp2-1.5.0/input/golden/test_data2_jp_en_fifo_tax_report_jp.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data2_lifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_data2_lifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data2_lifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_data2_lifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data3_2019-12-01_2020-04-01_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_data3_2019-12-01_2020-04-01_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data3_2019-12-01_2020-04-01_fifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_data3_2019-12-01_2020-04-01_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data3_2019-12-01_2020-04-01_hifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_data3_2019-12-01_2020-04-01_hifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data3_2019-12-01_2020-04-01_hifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_data3_2019-12-01_2020-04-01_hifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data3_2019-12-01_2020-04-01_lifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_data3_2019-12-01_2020-04-01_lifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data3_2019-12-01_2020-04-01_lifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_data3_2019-12-01_2020-04-01_lifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data3_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_data3_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data3_fifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_data3_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data3_hifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_data3_hifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data3_hifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_data3_hifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data3_jp_en_fifo_open_positions.ods` & `rp2-1.5.0/input/golden/test_data3_jp_en_fifo_open_positions.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data3_jp_en_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_data3_jp_en_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data3_jp_en_fifo_tax_report_jp.ods` & `rp2-1.5.0/input/golden/test_data3_jp_en_fifo_tax_report_jp.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data3_lifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_data3_lifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data3_lifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_data3_lifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data4_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_data4_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data4_fifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_data4_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data4_hifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_data4_hifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data4_hifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_data4_hifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data4_jp_en_fifo_open_positions.ods` & `rp2-1.5.0/input/golden/test_data4_jp_en_fifo_open_positions.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data4_jp_en_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_data4_jp_en_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data4_jp_en_fifo_tax_report_jp.ods` & `rp2-1.5.0/input/golden/test_data4_jp_en_fifo_tax_report_jp.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data4_lifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_data4_lifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data4_lifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_data4_lifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_data_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data_fifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_data_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data_hifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_data_hifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data_hifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_data_hifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data_jp_en_fifo_open_positions.ods` & `rp2-1.5.0/input/golden/test_data_jp_en_fifo_open_positions.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data_jp_en_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_data_jp_en_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data_jp_en_fifo_tax_report_jp.ods` & `rp2-1.5.0/input/golden/test_data_jp_en_fifo_tax_report_jp.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data_jp_kl_fifo_open_positions.ods` & `rp2-1.5.0/input/golden/test_data_jp_kl_fifo_open_positions.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data_jp_kl_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_data_jp_kl_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data_lifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_data_lifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data_lifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_data_lifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data_multi_method_mixed_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_data_multi_method_mixed_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_data_multi_method_mixed_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_data_multi_method_mixed_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_hifo2_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_hifo2_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_hifo2_fifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_hifo2_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_hifo2_hifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_hifo2_hifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_hifo2_hifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_hifo2_hifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_hifo2_lifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_hifo2_lifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_hifo2_lifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_hifo2_lifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_hifo_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_hifo_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_hifo_fifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_hifo_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_hifo_hifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_hifo_hifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_hifo_hifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_hifo_hifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_hifo_lifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_hifo_lifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_hifo_lifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_hifo_lifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_large_input_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_large_input_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_large_input_fifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_large_input_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_large_input_hifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_large_input_hifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_large_input_hifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_large_input_hifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_large_input_lifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_large_input_lifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_large_input_lifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_large_input_lifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_0_2016-12-31_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_many_year_data_0_2016-12-31_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_0_2016-12-31_fifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_many_year_data_0_2016-12-31_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_0_2017-12-31_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_many_year_data_0_2017-12-31_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_0_2017-12-31_fifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_many_year_data_0_2017-12-31_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_0_2018-12-31_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_many_year_data_0_2018-12-31_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_0_2018-12-31_fifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_many_year_data_0_2018-12-31_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_0_2019-12-31_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_many_year_data_0_2019-12-31_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_0_2019-12-31_fifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_many_year_data_0_2019-12-31_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_0_2020-12-31_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_many_year_data_0_2020-12-31_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_0_2020-12-31_fifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_many_year_data_0_2020-12-31_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_2017-01-01_2019-12-31_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_many_year_data_2017-01-01_2019-12-31_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_2017-01-01_2019-12-31_fifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_many_year_data_2017-01-01_2019-12-31_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_2017-01-01_infinity_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_many_year_data_2017-01-01_infinity_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_2017-01-01_infinity_fifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_many_year_data_2017-01-01_infinity_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_2018-01-01_2019-12-31_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_many_year_data_2018-01-01_2019-12-31_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_2018-01-01_2019-12-31_fifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_many_year_data_2018-01-01_2019-12-31_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_2018-01-01_infinity_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_many_year_data_2018-01-01_infinity_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_2018-01-01_infinity_fifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_many_year_data_2018-01-01_infinity_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_2019-01-01_2019-12-31_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_many_year_data_2019-01-01_2019-12-31_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_2019-01-01_2019-12-31_fifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_many_year_data_2019-01-01_2019-12-31_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_2019-01-01_infinity_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_many_year_data_2019-01-01_infinity_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_2019-01-01_infinity_fifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_many_year_data_2019-01-01_infinity_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_2020-01-01_infinity_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_many_year_data_2020-01-01_infinity_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_2020-01-01_infinity_fifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_many_year_data_2020-01-01_infinity_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_2021-01-01_infinity_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_many_year_data_2021-01-01_infinity_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_2021-01-01_infinity_fifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_many_year_data_2021-01-01_infinity_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_many_year_data_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_fifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_many_year_data_fifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_hifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_many_year_data_hifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_hifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_many_year_data_hifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_jp_en_fifo_open_positions.ods` & `rp2-1.5.0/input/golden/test_many_year_data_jp_en_fifo_open_positions.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_jp_en_fifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_many_year_data_jp_en_fifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_jp_en_fifo_tax_report_jp.ods` & `rp2-1.5.0/input/golden/test_many_year_data_jp_en_fifo_tax_report_jp.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_lifo_rp2_full_report.ods` & `rp2-1.5.0/input/golden/test_many_year_data_lifo_rp2_full_report.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/golden/test_many_year_data_lifo_tax_report_us.ods` & `rp2-1.5.0/input/golden/test_many_year_data_lifo_tax_report_us.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/test_bad_data.ods` & `rp2-1.5.0/input/test_bad_data.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/test_data.ods` & `rp2-1.5.0/input/test_data.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/test_data2.ods` & `rp2-1.5.0/input/test_data2.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/test_data3.ods` & `rp2-1.5.0/input/test_data3.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/test_data4.ods` & `rp2-1.5.0/input/test_data4.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/test_data_multi_method.ods` & `rp2-1.5.0/input/test_data_multi_method.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/test_hifo.ods` & `rp2-1.5.0/input/test_hifo.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/test_hifo2.ods` & `rp2-1.5.0/input/test_hifo2.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/input/test_many_year_data.ods` & `rp2-1.5.0/input/test_many_year_data.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/setup.cfg` & `rp2-1.5.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [metadata]
 name = rp2
-version = 1.4.2
+version = 1.5.0
 description = Privacy-focused, free, non-commercial, open-source, community-driven cryptocurrency tax calculator: it handles multiple coins/exchanges and computes long/short-term capital gains, cost bases, in/out lot relationships/fractioning, and account balances. It supports the FIFO accounting method, it features transparent computation for easy result verification, and it generates reports that tax accountants can understand, even if they are not cryptocurrency experts (e.g. form 8949).
 long_description_content_type = text/markdown
 long_description = file: README.md, CHANGELOG.md
-keywords = accounting, altcoin, bitcoin, BTC, capital gains, cost basis, crypto, cryptocurrency, ETH, ethereum, finance, form 8949, NFT, privacy, wallet, tax
+keywords = accounting, altcoin, bitcoin, BTC, capital gains, cost basis, crypto, cryptocurrency, DeFi, ETH, ethereum, finance, form 8949, NFT, privacy, wallet, tax
 license = Apache License 2.0
 author = eprbell
 url = https://github.com/eprbell/rp2
 classifiers = 
 	Development Status :: 5 - Production/Stable
 	Intended Audience :: End Users/Desktop
 	License :: OSI Approved :: Apache Software License
@@ -65,13 +65,14 @@
 rp2 = py.typed, locales/*/*/*.mo
 rp2.plugin.report = data/*.ods, data/*/*.ods, data/*/*.txt
 
 [options.entry_points]
 console_scripts = 
 	rp2_us = rp2.plugin.country.us:rp2_entry
 	rp2_jp = rp2.plugin.country.jp:rp2_entry
+	rp2_es = rp2.plugin.country.es:rp2_entry
 	rp2_config = rp2.rp2_configuration_translator:rp2_configuration_translator
 
 [egg_info]
 tag_build = 
 tag_date = 0
```

### Comparing `rp2-1.4.2/src/rp2/abstract_accounting_method.py` & `rp2-1.5.0/src/rp2/abstract_accounting_method.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/abstract_country.py` & `rp2-1.5.0/src/rp2/abstract_country.py`

 * *Files 0% similar despite different names*

```diff
@@ -28,15 +28,14 @@
         return instance
 
     def __init__(
         self,
         country_iso_code: str,  # ISO 3166-1 alpha-2
         currency_iso_code: str,  # ISO 4217
     ) -> None:
-
         if not isinstance(country_iso_code, str):
             raise RP2TypeError(f"Parameter 'country_iso_code' has non-string value {repr(country_iso_code)}")
         if not isinstance(currency_iso_code, str):
             raise RP2TypeError(f"Parameter 'currency_iso_code' has non-string value {repr(currency_iso_code)}")
 
         self.__country_iso_code = country_iso_code
         self.__currency_iso_code = currency_iso_code
```

### Comparing `rp2-1.4.2/src/rp2/abstract_entry.py` & `rp2-1.5.0/src/rp2/abstract_entry.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/abstract_entry_set.py` & `rp2-1.5.0/src/rp2/abstract_entry_set.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/abstract_report_generator.py` & `rp2-1.5.0/src/rp2/abstract_report_generator.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/abstract_transaction.py` & `rp2-1.5.0/src/rp2/abstract_transaction.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/accounting_engine.py` & `rp2-1.5.0/src/rp2/accounting_engine.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,14 @@
 
 
 class AcquiredLotsExhaustedException(_LotExhaustedException):
     pass
 
 
 class AccountingEngine:
-
     __taxable_event_iterator: Iterator[AbstractTransaction]
     __acquired_lot_list: List[InTransaction]
     __acquired_lot_avl: AVLTree[str, _AcquiredLotAndIndex]
     __acquired_lot_2_partial_amount: Dict[InTransaction, RP2Decimal]
 
     # Disambiguation is needed for transactions that have the same timestamp, because the avl tree class expects unique keys: 12 decimal digits express
     # 1 quadrillion, which should be enough to capture the maximum number of same-timestamp transactions in all reasonable cases.
```

### Comparing `rp2-1.4.2/src/rp2/balance.py` & `rp2-1.5.0/src/rp2/balance.py`

 * *Files 0% similar despite different names*

```diff
@@ -97,15 +97,14 @@
     # from_date is not used when computing average price per unit: only to_date is relevant.
     def __init__(
         self,
         configuration: Configuration,
         input_data: InputData,
         to_date: date,
     ) -> None:
-
         Configuration.type_check("configuration", configuration)
         self.__input_data = InputData.type_check("input_data", input_data)
 
         self.__asset: str = configuration.type_check_asset("in_transaction_set.asset", input_data.asset)
         self._balances: List[Balance] = []
 
         acquired_balances: Dict[Account, RP2Decimal] = {}
```

### Comparing `rp2-1.4.2/src/rp2/computed_data.py` & `rp2-1.5.0/src/rp2/computed_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -165,15 +165,15 @@
             )
 
         yearly_gain_loss_set: Set[YearlyGainLoss] = set()
         crypto_taxable_amount_total: RP2Decimal = ZERO
         fiat_taxable_amount_total: RP2Decimal = ZERO
         cost_basis_total: RP2Decimal = ZERO
         gain_loss_total: RP2Decimal = ZERO
-        for (key, value) in summaries.items():
+        for key, value in summaries.items():
             yearly_gain_loss: YearlyGainLoss = YearlyGainLoss(
                 year=key.year,
                 asset=key.asset,
                 transaction_type=key.transaction_type,
                 is_long_term_capital_gains=key.is_long_term_capital_gains,
                 crypto_amount=value.crypto_amount,
                 fiat_amount=value.fiat_amount,
```

### Comparing `rp2-1.4.2/src/rp2/configuration.py` & `rp2-1.5.0/src/rp2/configuration.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/configuration_schema.py` & `rp2-1.5.0/src/rp2/configuration_schema.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/gain_loss.py` & `rp2-1.5.0/src/rp2/gain_loss.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,14 @@
     def __init__(
         self,
         configuration: Configuration,
         crypto_amount: RP2Decimal,
         taxable_event: AbstractTransaction,
         acquired_lot: Optional[InTransaction],
     ) -> None:
-
         self.__taxable_event: AbstractTransaction = cast(AbstractTransaction, AbstractTransaction.type_check("taxable_event", taxable_event))
         if not taxable_event.is_taxable():
             raise RP2ValueError(f"Parameter 'taxable_event' of class {taxable_event.__class__.__name__} is not taxable: {taxable_event}")
 
         super().__init__(configuration, taxable_event.asset)
 
         self.__crypto_amount: RP2Decimal = configuration.type_check_positive_decimal("crypto_amount", crypto_amount, non_zero=True)
```

### Comparing `rp2-1.4.2/src/rp2/gain_loss_set.py` & `rp2-1.5.0/src/rp2/gain_loss_set.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/in_transaction.py` & `rp2-1.5.0/src/rp2/in_transaction.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/input_data.py` & `rp2-1.5.0/src/rp2/input_data.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/intra_transaction.py` & `rp2-1.5.0/src/rp2/intra_transaction.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/locales/en/LC_MESSAGES/messages.po` & `rp2-1.5.0/src/rp2/locales/en/LC_MESSAGES/messages.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the rp2 project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: rp2 1.0.6\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-08-17 00:13-0700\n"
+"POT-Creation-Date: 2023-05-22 14:31+0200\n"
 "PO-Revision-Date: 2022-08-10 12:38-0700\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: en\n"
 "Language-Team: en <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "<Crypto> In-Out"
 msgstr ""
 
 msgid "<Crypto> Tax"
 msgstr ""
 
@@ -626,14 +626,53 @@
 
 msgid "Yearly Gain / Loss Summary"
 msgstr ""
 
 msgid "Yellow"
 msgstr ""
 
+msgid "airdrop"
+msgstr ""
+
+msgid "buy"
+msgstr ""
+
+msgid "donate"
+msgstr ""
+
+msgid "fee"
+msgstr ""
+
+msgid "gift"
+msgstr ""
+
+msgid "hardfork"
+msgstr ""
+
+msgid "income"
+msgstr ""
+
+msgid "interest"
+msgstr ""
+
+msgid "mining"
+msgstr ""
+
+msgid "move"
+msgstr ""
+
+msgid "sell"
+msgstr ""
+
+msgid "staking"
+msgstr ""
+
+msgid "wages"
+msgstr ""
+
 msgid "{}"
 msgstr ""
 
 msgid "{} Fee"
 msgstr ""
 
 msgid "{} In"
@@ -707,14 +746,20 @@
 
 msgid "{} value of the transaction with fees"
 msgstr ""
 
 msgid "{} value of the transaction without fees"
 msgstr ""
 
+msgid "{}_Summary"
+msgstr ""
+
+msgid "{}_{}"
+msgstr ""
+
 #~ msgid "Asset - Exchange"
 #~ msgstr ""
 
 #~ msgid "Input"
 #~ msgstr ""
 
 #~ msgid "US dollar value of the fees"
```

### Comparing `rp2-1.4.2/src/rp2/locales/ja/LC_MESSAGES/messages.po` & `rp2-1.5.0/src/rp2/locales/ja/LC_MESSAGES/messages.po`

 * *Files 5% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the rp2 project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: rp2 1.0.6\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-08-17 00:13-0700\n"
+"POT-Creation-Date: 2023-05-22 14:31+0200\n"
 "PO-Revision-Date: 2022-08-11 21:50-0700\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: ja\n"
 "Language-Team: ja <LL@li.org>\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "<Crypto> In-Out"
 msgstr ""
 
 msgid "<Crypto> Tax"
 msgstr ""
 
@@ -626,14 +626,53 @@
 
 msgid "Yearly Gain / Loss Summary"
 msgstr ""
 
 msgid "Yellow"
 msgstr ""
 
+msgid "airdrop"
+msgstr ""
+
+msgid "buy"
+msgstr ""
+
+msgid "donate"
+msgstr ""
+
+msgid "fee"
+msgstr ""
+
+msgid "gift"
+msgstr ""
+
+msgid "hardfork"
+msgstr ""
+
+msgid "income"
+msgstr ""
+
+msgid "interest"
+msgstr ""
+
+msgid "mining"
+msgstr ""
+
+msgid "move"
+msgstr ""
+
+msgid "sell"
+msgstr ""
+
+msgid "staking"
+msgstr ""
+
+msgid "wages"
+msgstr ""
+
 msgid "{}"
 msgstr ""
 
 msgid "{} Fee"
 msgstr ""
 
 msgid "{} In"
@@ -706,7 +745,13 @@
 msgstr ""
 
 msgid "{} value of the transaction with fees"
 msgstr ""
 
 msgid "{} value of the transaction without fees"
 msgstr ""
+
+msgid "{}_Summary"
+msgstr ""
+
+msgid "{}_{}"
+msgstr ""
```

### Comparing `rp2-1.4.2/src/rp2/locales/kl/LC_MESSAGES/messages.mo` & `rp2-1.5.0/src/rp2/locales/kl/LC_MESSAGES/messages.mo`

 * *Files 3% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: rp2 1.0.6\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-08-17 00:13-0700\n"
+"POT-Creation-Date: 2023-05-22 14:31+0200\n"
 "PO-Revision-Date: 2022-08-10 19:04-0700\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: kl\n"
 "Language-Team: kl <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "<Crypto> In-Out"
 msgstr "__test_<Crypto> In-Out"
 
 msgid "<Crypto> Tax"
 msgstr "__test_<Crypto> Tax"
 
@@ -764,14 +764,53 @@
 
 msgid "Yearly Gain / Loss Summary"
 msgstr "__test_Yearly Gain / Loss Summary"
 
 msgid "Yellow"
 msgstr "__test_Yellow"
 
+msgid "airdrop"
+msgstr "__test_airdrop"
+
+msgid "buy"
+msgstr "__test_buy"
+
+msgid "donate"
+msgstr "__test_donate"
+
+msgid "fee"
+msgstr "__test_fee"
+
+msgid "gift"
+msgstr "__test_gift"
+
+msgid "hardfork"
+msgstr "__test_hardfork"
+
+msgid "income"
+msgstr "__test_income"
+
+msgid "interest"
+msgstr "__test_interest"
+
+msgid "mining"
+msgstr "__test_mining"
+
+msgid "move"
+msgstr "__test_move"
+
+msgid "sell"
+msgstr "__test_sell"
+
+msgid "staking"
+msgstr "__test_staking"
+
+msgid "wages"
+msgstr "__test_wages"
+
 msgid "{}"
 msgstr "__test_{}"
 
 msgid "{} Fee"
 msgstr "__test_{} Fee"
 
 msgid "{} In"
@@ -844,7 +883,13 @@
 msgstr "__test_{} value of the fees"
 
 msgid "{} value of the transaction with fees"
 msgstr "__test_{} value of the transaction with fees"
 
 msgid "{} value of the transaction without fees"
 msgstr "__test_{} value of the transaction without fees"
+
+msgid "{}_Summary"
+msgstr "__test_{}_Summary"
+
+msgid "{}_{}"
+msgstr "__test_{}_{}"
```

### Comparing `rp2-1.4.2/src/rp2/locales/kl/LC_MESSAGES/messages.po` & `rp2-1.5.0/src/rp2/locales/kl/LC_MESSAGES/messages.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,24 +3,24 @@
 # This file is distributed under the same license as the rp2 project.
 # FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: rp2 1.0.6\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-08-17 00:13-0700\n"
+"POT-Creation-Date: 2023-05-22 14:31+0200\n"
 "PO-Revision-Date: 2022-08-10 19:04-0700\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: kl\n"
 "Language-Team: kl <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "<Crypto> In-Out"
 msgstr "__test_<Crypto> In-Out"
 
 msgid "<Crypto> Tax"
 msgstr "__test_<Crypto> Tax"
 
@@ -626,14 +626,53 @@
 
 msgid "Yearly Gain / Loss Summary"
 msgstr "__test_Yearly Gain / Loss Summary"
 
 msgid "Yellow"
 msgstr "__test_Yellow"
 
+msgid "airdrop"
+msgstr "__test_airdrop"
+
+msgid "buy"
+msgstr "__test_buy"
+
+msgid "donate"
+msgstr "__test_donate"
+
+msgid "fee"
+msgstr "__test_fee"
+
+msgid "gift"
+msgstr "__test_gift"
+
+msgid "hardfork"
+msgstr "__test_hardfork"
+
+msgid "income"
+msgstr "__test_income"
+
+msgid "interest"
+msgstr "__test_interest"
+
+msgid "mining"
+msgstr "__test_mining"
+
+msgid "move"
+msgstr "__test_move"
+
+msgid "sell"
+msgstr "__test_sell"
+
+msgid "staking"
+msgstr "__test_staking"
+
+msgid "wages"
+msgstr "__test_wages"
+
 msgid "{}"
 msgstr "__test_{}"
 
 msgid "{} Fee"
 msgstr "__test_{} Fee"
 
 msgid "{} In"
@@ -707,14 +746,20 @@
 
 msgid "{} value of the transaction with fees"
 msgstr "__test_{} value of the transaction with fees"
 
 msgid "{} value of the transaction without fees"
 msgstr "__test_{} value of the transaction without fees"
 
+msgid "{}_Summary"
+msgstr "__test_{}_Summary"
+
+msgid "{}_{}"
+msgstr "__test_{}_{}"
+
 #~ msgid "Asset - Exchange"
 #~ msgstr "__test_Asset - Exchange"
 
 #~ msgid "Input"
 #~ msgstr "__test_Input"
 
 #~ msgid "US dollar value of the fees"
```

### Comparing `rp2-1.4.2/src/rp2/locales/messages.pot` & `rp2-1.5.0/src/rp2/locales/messages.pot`

 * *Files 7% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # Translations template for rp2.
-# Copyright (C) 2022 eprbell
+# Copyright (C) 2023 eprbell
 # This file is distributed under the same license as the rp2 project.
-# FIRST AUTHOR <EMAIL@ADDRESS>, 2022.
+# FIRST AUTHOR <EMAIL@ADDRESS>, 2023.
 #
 #, fuzzy
 msgid ""
 msgstr ""
-"Project-Id-Version: rp2 1.0.8\n"
+"Project-Id-Version: rp2 1.4.2\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-08-17 00:13-0700\n"
+"POT-Creation-Date: 2023-05-22 14:31+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid "<Crypto> In-Out"
 msgstr ""
 
 msgid "<Crypto> Tax"
 msgstr ""
 
@@ -625,14 +625,53 @@
 
 msgid "Yearly Gain / Loss Summary"
 msgstr ""
 
 msgid "Yellow"
 msgstr ""
 
+msgid "airdrop"
+msgstr ""
+
+msgid "buy"
+msgstr ""
+
+msgid "donate"
+msgstr ""
+
+msgid "fee"
+msgstr ""
+
+msgid "gift"
+msgstr ""
+
+msgid "hardfork"
+msgstr ""
+
+msgid "income"
+msgstr ""
+
+msgid "interest"
+msgstr ""
+
+msgid "mining"
+msgstr ""
+
+msgid "move"
+msgstr ""
+
+msgid "sell"
+msgstr ""
+
+msgid "staking"
+msgstr ""
+
+msgid "wages"
+msgstr ""
+
 msgid "{}"
 msgstr ""
 
 msgid "{} Fee"
 msgstr ""
 
 msgid "{} In"
@@ -705,7 +744,13 @@
 msgstr ""
 
 msgid "{} value of the transaction with fees"
 msgstr ""
 
 msgid "{} value of the transaction without fees"
 msgstr ""
+
+msgid "{}_Summary"
+msgstr ""
+
+msgid "{}_{}"
+msgstr ""
```

### Comparing `rp2-1.4.2/src/rp2/localization.py` & `rp2-1.5.0/src/rp2/localization.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/logger.py` & `rp2-1.5.0/src/rp2/logger.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/ods_parser.py` & `rp2-1.5.0/src/rp2/ods_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,14 @@
     if not Path(input_file_path).exists():
         raise RP2ValueError(f"Error: {input_file_path} does not exist")
 
     return ezodf.opendoc(input_file_path)
 
 
 def parse_ods(configuration: Configuration, asset: str, input_file_handle: Any) -> InputData:  # pylint: disable=too-many-branches
-
     Configuration.type_check("configuration", configuration)
     configuration.type_check_asset("asset", asset)
 
     if asset not in input_file_handle.sheets.names():
         raise RP2ValueError(f"Error: sheet {asset} does not exist in {Path(input_file_handle.docname).resolve()}")
     input_sheet: Any = input_file_handle.sheets[asset]
 
@@ -160,15 +159,14 @@
     row_values: List[Any],
     current_table_type: EntrySetType,
     internal_id: int,
     artificial_internal_id: int,
     unfiltered_transaction_sets: Dict[EntrySetType, TransactionSet],
     artificial_transaction_list: List[AbstractTransaction],
 ) -> None:
-
     transaction: AbstractTransaction = _create_transaction(configuration, current_table_type, internal_id, row_values)
 
     if isinstance(transaction, InTransaction) and transaction.is_crypto_fee_defined:
         # If an InTransaction has crypto fee defined it is split into two transactions:
         # - InTransaction with crypto_fee set to 0, but fiat_fee left as-is (the fiat-converted value of crypto_fee),
         # - fee-typed OutTransaction, modeling the crypto_fee.
         # These two transactions correctly model the coin flow of a InTransaction with crypto fee > 0: their notes
```

### Comparing `rp2-1.4.2/src/rp2/out_transaction.py` & `rp2-1.5.0/src/rp2/out_transaction.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/plugin/accounting_method/fifo.py` & `rp2-1.5.0/src/rp2/plugin/accounting_method/fifo.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/plugin/accounting_method/hifo.py` & `rp2-1.5.0/src/rp2/plugin/accounting_method/hifo.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/plugin/accounting_method/lifo.py` & `rp2-1.5.0/src/rp2/plugin/accounting_method/lifo.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/plugin/country/jp.py` & `rp2-1.5.0/src/rp2/plugin/country/jp.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/plugin/country/us.py` & `rp2-1.5.0/src/rp2/plugin/country/us.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/plugin/report/abstract_ods_generator.py` & `rp2-1.5.0/src/rp2/plugin/report/abstract_ods_generator.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,14 @@
         output_file_prefix: str,
         output_file_name: str,
         template_path: str,
         template_sheets_to_keep: Set[str],
         from_date: date,
         to_date: date,
     ) -> Any:
-
         Configuration.type_check_string("output_dir_path", output_dir_path)
         Configuration.type_check_string("output_file_prefix", output_file_prefix)
         Configuration.type_check_string("output_file_name", output_file_name)
         if not isinstance(template_sheets_to_keep, Set):
             raise RP2TypeError(f"Parameter 'template_sheets_to_keep' is not a Set: {template_sheets_to_keep}")
 
         accounting_method: str = years_2_accounting_method_names[MIN_DATE.year] if len(years_2_accounting_method_names) == 1 else "mixed"
@@ -164,15 +163,14 @@
         row_index: int,
         column_index: int,
         value: Any,
         visual_style: str = "transparent",
         data_style: str = "default",
         apply_style: bool = True,
     ) -> None:
-
         Configuration.type_check_string("visual_style", visual_style)
         Configuration.type_check_string("data_style", data_style)
 
         is_formula: bool = False
         if isinstance(value, str) and value and value[0] == "=":
             # If the value starts with '=' it is assumed to be a formula
             is_formula = True
@@ -187,15 +185,14 @@
             sheet[row_index, column_index].set_value(value)
         if apply_style:
             cls._apply_style_to_cell(sheet=sheet, row_index=row_index, column_index=column_index, style_name=style_name)
 
     def _fill_header(
         self, title: str, header_row_1: List[str], header_row_2: List[str], sheet: Any, row_index: int, column_index: int, apply_style: bool = True
     ) -> int:
-
         Configuration.type_check_string("title", title)
         if not isinstance(header_row_1, List):
             raise RP2TypeError("Parameter 'header_row_1' is not a List")
         if not isinstance(header_row_2, List):
             raise RP2TypeError("Parameter 'header_row_2' is not a List")
 
         self._fill_cell(sheet, row_index, 0, title, visual_style="title", apply_style=apply_style)
```

### Comparing `rp2-1.4.2/src/rp2/plugin/report/data/jp/template_rp2_full_report_en.ods` & `rp2-1.5.0/src/rp2/plugin/report/data/jp/template_rp2_full_report_en.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/plugin/report/data/jp/template_rp2_full_report_kl.ods` & `rp2-1.5.0/src/rp2/plugin/report/data/jp/template_rp2_full_report_kl.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/plugin/report/data/jp/template_tax_report_jp_en.ods` & `rp2-1.5.0/src/rp2/plugin/report/data/jp/template_tax_report_jp_en.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/plugin/report/data/jp/template_tax_report_jp_kl.ods` & `rp2-1.5.0/src/rp2/plugin/report/data/jp/template_tax_report_jp_kl.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/plugin/report/data/template_open_positions.ods` & `rp2-1.5.0/src/rp2/plugin/report/data/jp/template_open_positions_en.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/plugin/report/data/us/template_rp2_full_report_en.ods` & `rp2-1.5.0/src/rp2/plugin/report/data/us/template_rp2_full_report_en.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/plugin/report/data/us/template_tax_report_us_en.ods` & `rp2-1.5.0/src/rp2/plugin/report/data/us/template_tax_report_us_en.ods`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/plugin/report/jp/tax_report_jp.py` & `rp2-1.5.0/src/rp2/plugin/report/jp/tax_report_jp.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,27 +66,25 @@
     TransactionType.MINING: None,
     TransactionType.STAKING: None,
     TransactionType.WAGES: None,
 }
 
 
 class Generator(AbstractODSGenerator):
-
     MIN_ROWS: int = 20
     MAX_COLUMNS: int = 20
     OUTPUT_FILE: str = "tax_report_jp.ods"
 
     ASSET_TEMPLATE_SHEET: str = "Asset"
     SUMMARY_TEMPLATE_SHEET: str = "Summary"
     TRANSACTION_ROW_START: int = 22
 
     TRANSFER: str = "Transfer"
 
     def __init__(self) -> None:
-
         super().__init__()
         self.__year_row_offset: Dict[int, int] = {}
         self.__number_of_summaries: int = 0
 
     def generate(
         self,
         country: AbstractCountry,
@@ -94,15 +92,14 @@
         asset_to_computed_data: Dict[str, ComputedData],
         output_dir_path: str,
         output_file_prefix: str,
         from_date: date,
         to_date: date,
         generation_language: str,
     ) -> None:
-
         if from_date != MIN_DATE and to_date != MAX_DATE:
             raise RP2RuntimeError("To and From Dates can not be specified for the JP tax report.")
 
         if not isinstance(asset_to_computed_data, Dict):
             raise RP2TypeError(f"Parameter 'asset_to_computed_data' has non-Dict value {asset_to_computed_data}")
 
         template_path: str = self._get_template_path("tax_report_jp", country, generation_language)
@@ -201,15 +198,14 @@
             self._fill_cell(summary_sheet, self.__year_row_offset[year] + 2, 2, f"=SUM(C8:C{self.__year_row_offset[year] + 2})", apply_style=False)
             # Total Amount in yen
             self._fill_cell(summary_sheet, self.__year_row_offset[year] + 2, 5, f"=SUM(F8:F{self.__year_row_offset[year] + 2})", apply_style=False)
             # Net Income Amt
             self._fill_cell(summary_sheet, self.__year_row_offset[year] + 2, 6, f"=SUM(G8:G{self.__year_row_offset[year] + 2})", apply_style=False)
 
     def __process_in_transaction(self, transaction: InTransaction) -> _TransactionRow:
-
         purchase_amount_in_yen: RP2Decimal = transaction.crypto_in * transaction.spot_price
 
         # Find the fee in yen
         fee_in_yen: RP2Decimal = ZERO
         if RP2Decimal(transaction.crypto_fee) > ZERO:
             fee_in_yen = transaction.crypto_fee * transaction.spot_price
         elif RP2Decimal(transaction.fiat_fee) > ZERO:
@@ -237,15 +233,14 @@
             sales_crypto_amount=sales_crypto_amount,
             sales_amount_in_yen=sales_amount_in_yen,
             fee_in_yen=fee_in_yen,
             gift=gift,
         )
 
     def __process_intra_transaction(self, transaction: IntraTransaction) -> _TransactionRow:
-
         transaction_fee_in_crypto: Optional[RP2Decimal] = None
         transaction_fee_in_yen: Optional[RP2Decimal] = None
 
         transaction_fee_in_crypto = transaction.crypto_sent - transaction.crypto_received
         transaction_fee_in_yen = transaction_fee_in_crypto * transaction.spot_price
 
         return _TransactionRow(
@@ -256,15 +251,14 @@
             sales_crypto_amount=transaction_fee_in_crypto if transaction_fee_in_crypto > ZERO else None,
             sales_amount_in_yen=transaction_fee_in_yen if transaction_fee_in_yen > ZERO else None,
             fee_in_yen=ZERO,
             gift=ZERO,
         )
 
     def __process_out_transaction(self, transaction: OutTransaction) -> _TransactionRow:
-
         # Find the fee in yen
         fee_in_yen: RP2Decimal = ZERO
         if RP2Decimal(transaction.crypto_fee) > ZERO:
             fee_in_yen = transaction.crypto_fee * transaction.spot_price
         elif RP2Decimal(transaction.fiat_fee) > ZERO:
             fee_in_yen = transaction.fiat_fee
 
@@ -285,28 +279,26 @@
             sales_crypto_amount=transaction.crypto_out_with_fee,
             sales_amount_in_yen=sales_amount_in_yen,
             fee_in_yen=fee_in_yen,
             donated_amount_in_yen=donated_amount_in_yen,
         )
 
     def __generate_asset_year(self, asset: str, year: int, transaction_list: List[AbstractTransaction], output_file: Any, previous_year_row_offset: int) -> int:
-
         asset_year_sheet: Any = output_file.sheets[self.ASSET_TEMPLATE_SHEET].copy(newname=self.get_tax_sheet_name(asset, year))
         output_file.sheets += asset_year_sheet
 
         # Label the asset at the top of the page
         self._fill_cell(asset_year_sheet, 1, 7, asset, apply_style=False)
         row_index: int = 21
         total_donations: RP2Decimal = ZERO
         total_gifts: RP2Decimal = ZERO
         formatted_donation_amount: Optional[str] = None
         transaction_row: _TransactionRow
 
         for entry in transaction_list:
-
             if isinstance(entry, InTransaction):
                 transaction_row = self.__process_in_transaction(entry)
                 total_gifts += transaction_row.gift
 
             elif isinstance(entry, OutTransaction):
                 transaction_row = self.__process_out_transaction(entry)
                 if transaction_row.donated_amount_in_yen is not None:
```

### Comparing `rp2-1.4.2/src/rp2/plugin/report/open_positions.py` & `rp2-1.5.0/src/rp2/plugin/report/open_positions.py`

 * *Files 0% similar despite different names*

```diff
@@ -37,29 +37,27 @@
 _ASSET_EXCHANGE: str = "Asset - Exchange"
 _INPUT: str = "Input"
 _INPUT_VALUE_STRING: str = "Enter asset value"
 _REPORT_INPUT_VALUE_STRING: str = "See Input tab"
 
 
 class Generator(AbstractODSGenerator):
-
     OUTPUT_FILE: str = "open_positions.ods"
     HEADER_ROWS = 3
 
     __legend: List[List[str]] = []
     __asset_header_names_row_1: List[str] = []
     __asset_header_names_row_2: List[str] = []
     __asset_exchange_header_names_row_1: List[str] = []
     __asset_exchange_header_names_row_2: List[str] = []
     __input_header_names_row_1: List[str] = []
     __input_header_names_row_2: List[str] = []
 
     # pylint: disable=line-too-long
     def _setup_text_data(self, country: AbstractCountry) -> None:
-
         currency_code: str = country.currency_iso_code.upper()
 
         self.__legend: List[List[str]] = [
             # fmt: off
             [_("Open Positions / Unrealized Gains")],
             [_("Fill in Asset Prices in the Input Tab for calculations")],
             [_("This report leverages the details of your transactions to give you a snapshot of the value of your unsold holdings")],
@@ -170,23 +168,22 @@
         asset_to_computed_data: Dict[str, ComputedData],
         output_dir_path: str,
         output_file_prefix: str,
         from_date: date,
         to_date: date,
         generation_language: str,
     ) -> None:
-
         # pylint: disable=too-many-branches
 
         if not isinstance(asset_to_computed_data, Dict):
             raise RP2TypeError(f"Parameter 'asset_to_computed_data' has non-Dict value {asset_to_computed_data}")
 
         self._setup_text_data(country)
 
-        template_path: str = self._get_template_path("open_positions", None, generation_language)
+        template_path: str = self._get_template_path("open_positions", country, generation_language)
 
         output_file: Any
         output_file = self._initialize_output_file(
             country=country,
             legend_data=self.__legend,
             years_2_accounting_method_names=years_2_accounting_method_names,
             output_dir_path=output_dir_path,
@@ -251,17 +248,15 @@
                     value += transaction_cost_basis
                     asset_cost_bases[asset] = value
 
                     total_cost_basis += transaction_cost_basis
 
             # process balance set data for the asset to collect holder and crypto balance data.
             for balance_set in computed_data.balance_set:
-
                 if balance_set.final_balance > ZERO:
-
                     if balance_set.holder not in holders:
                         holders.append(balance_set.holder)
 
                     if asset not in asset_crypto_balance_holder:
                         asset_crypto_balance_holder[asset] = {}
                         asset_crypto_balance_holder_exchange[asset] = {}
 
@@ -272,15 +267,14 @@
                     asset_crypto_balance_holder[asset][balance_set.holder] += balance_set.final_balance
 
                     if balance_set.exchange not in asset_crypto_balance_holder_exchange[asset][balance_set.holder]:
                         asset_crypto_balance_holder_exchange[asset][balance_set.holder][balance_set.exchange] = balance_set.final_balance
 
         # Now looping through the assets to do the reporting.
         for asset, asset_cost_basis in asset_cost_bases.items():
-
             total_crypto_balance = ZERO
             for crypto_balance in asset_crypto_balance_holder[asset].values():
                 total_crypto_balance += crypto_balance
 
             unit_cost_basis: RP2Decimal = asset_cost_basis / total_crypto_balance
 
             # For report clarity, change how much precision is displayed in the output based on the unit price. The raw value is
@@ -322,15 +316,14 @@
                 self._fill_cell(asset_sheet, asset_row_index, 7, f"=C{asset_row_index+1}*G{asset_row_index+1}", data_style="fiat")
                 self._fill_cell(asset_sheet, asset_row_index, 8, f"=H{asset_row_index+1}-E{asset_row_index+1}", data_style="fiat")
                 self._fill_cell(asset_sheet, asset_row_index, 9, f"=(H{asset_row_index+1}-E{asset_row_index+1})/E{asset_row_index+1}", data_style="percent")
                 row_indexes[_ASSET] = asset_row_index + 1
 
             # Generate the Asset/Exchange table which will calc vals that will feed the asset table.
             for holder, exchanges in asset_crypto_balance_holder_exchange[asset].items():
-
                 for exchange, crypto_exchange_balance in exchanges.items():
                     exchange_cost_basis: RP2Decimal = crypto_exchange_balance * unit_cost_basis
 
                     asset_exchange_sheet.append_rows(1)
                     asset_exchange_row_index: int = row_indexes[_ASSET_EXCHANGE]
                     _vlookup_formula = f"VLOOKUP(A{asset_exchange_row_index+1};${_('Input')}.A:B;2;0)"
                     _lookup_field = f'=IF({_vlookup_formula}="{_INPUT_VALUE_STRING}";"{_REPORT_INPUT_VALUE_STRING}";{_vlookup_formula}'
```

### Comparing `rp2-1.4.2/src/rp2/plugin/report/rp2_full_report.py` & `rp2-1.5.0/src/rp2/plugin/report/rp2_full_report.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,14 @@
     year: int
 
 
 _ZERO: RP2Decimal = RP2Decimal(0)
 
 
 class Generator(AbstractODSGenerator):
-
     MIN_ROWS: int = 40
     MAX_COLUMNS: int = 40
     OUTPUT_FILE: str = "rp2_full_report.ods"
 
     TEMPLATE_SHEETS_TO_KEEP: Set[str] = {"__Summary"}
 
     __in_out_sheet_transaction_2_row: Dict[AbstractTransaction, int] = {}
@@ -85,15 +84,14 @@
     __gain_loss_summary_header_names_row_1: List[str] = []
     __gain_loss_summary_header_names_row_2: List[str] = []
     __gain_loss_detail_header_names_row_1: List[str] = []
     __gain_loss_detail_header_names_row_2: List[str] = []
 
     # pylint: disable=line-too-long
     def _setup_text_data(self, country: AbstractCountry) -> None:
-
         currency_code: str = country.currency_iso_code.upper()
 
         self.__legend: List[List[str]] = [
             # fmt: off
             [_("General")],
             [_("Accounting Method")],
             [_("From Date Filter")],
@@ -434,15 +432,14 @@
         asset_to_computed_data: Dict[str, ComputedData],
         output_dir_path: str,
         output_file_prefix: str,
         from_date: date,
         to_date: date,
         generation_language: str,
     ) -> None:
-
         if not isinstance(asset_to_computed_data, Dict):
             raise RP2TypeError(f"Parameter 'asset_to_computed_data' has non-Dict value {asset_to_computed_data}")
 
         self._setup_text_data(country)
 
         template_path: str = self._get_template_path("rp2_full_report", country, generation_language)
 
@@ -585,15 +582,15 @@
                 data_style="percent",
                 visual_style="acquired_lot" + border_suffix if in_lot_sold_percentage is not None else "transparent",
             )
             self._fill_cell(sheet, row_index, 1, transaction.timestamp, visual_style=visual_style)
             self._fill_cell(sheet, row_index, 2, transaction.asset, visual_style=visual_style)
             self._fill_cell(sheet, row_index, 3, transaction.exchange, visual_style=visual_style)
             self._fill_cell(sheet, row_index, 4, transaction.holder, visual_style=visual_style)
-            self._fill_cell(sheet, row_index, 5, transaction.transaction_type.value.upper(), visual_style=visual_style)
+            self._fill_cell(sheet, row_index, 5, transaction.transaction_type.get_translation().upper(), visual_style=visual_style)
             self._fill_cell(sheet, row_index, 6, transaction.spot_price, data_style="fiat", visual_style=visual_style)
             self._fill_cell(sheet, row_index, 7, transaction.crypto_in, data_style="crypto", visual_style=visual_style)
             self._fill_cell(sheet, row_index, 8, computed_data.get_crypto_in_running_sum(transaction), data_style="crypto", visual_style=visual_style)
             self._fill_cell(sheet, row_index, 9, transaction.fiat_fee, data_style="fiat", visual_style=visual_style)
             self._fill_cell(sheet, row_index, 10, transaction.fiat_in_no_fee, data_style="fiat", visual_style=visual_style)
             self._fill_cell(sheet, row_index, 11, transaction.fiat_in_with_fee, data_style="fiat", visual_style=highlighted_style)
             self._fill_cell(sheet, row_index, 12, _("YES") if transaction.is_taxable() else _("NO"), data_style="fiat", visual_style=visual_style)
@@ -624,15 +621,15 @@
             visual_style = transaction_visual_style.visual_style
             highlighted_style = transaction_visual_style.highlighted_style
             self._fill_cell(sheet, row_index, 0, "", visual_style="transparent")
             self._fill_cell(sheet, row_index, 1, transaction.timestamp, visual_style=visual_style)
             self._fill_cell(sheet, row_index, 2, transaction.asset, visual_style=visual_style)
             self._fill_cell(sheet, row_index, 3, transaction.exchange, visual_style=visual_style)
             self._fill_cell(sheet, row_index, 4, transaction.holder, visual_style=visual_style)
-            self._fill_cell(sheet, row_index, 5, transaction.transaction_type.value.upper(), visual_style=visual_style)
+            self._fill_cell(sheet, row_index, 5, transaction.transaction_type.get_translation().upper(), visual_style=visual_style)
             self._fill_cell(sheet, row_index, 6, transaction.spot_price, visual_style=visual_style, data_style="fiat")
             self._fill_cell(sheet, row_index, 7, transaction.crypto_out_no_fee, visual_style=visual_style, data_style="crypto")
             self._fill_cell(sheet, row_index, 8, transaction.crypto_fee, visual_style=visual_style, data_style="crypto")
             self._fill_cell(sheet, row_index, 9, computed_data.get_crypto_out_running_sum(transaction), data_style="crypto", visual_style=visual_style)
             self._fill_cell(sheet, row_index, 10, computed_data.get_crypto_out_fee_running_sum(transaction), data_style="crypto", visual_style=visual_style)
             self._fill_cell(
                 sheet,
@@ -710,15 +707,17 @@
             border_style: _BorderStyle = self.__get_border_style(yearly_gain_loss.year, year)
             year = border_style.year
             border_suffix = border_style.border_suffix
             self._fill_cell(sheet, row_index, 0, yearly_gain_loss.year, visual_style="transparent" + border_suffix, data_style="default")
             self._fill_cell(sheet, row_index, 1, yearly_gain_loss.asset, visual_style="transparent" + border_suffix, data_style="default")
             self._fill_cell(sheet, row_index, 2, yearly_gain_loss.fiat_gain_loss, visual_style="bold" + border_suffix, data_style="fiat")
             self._fill_cell(sheet, row_index, 3, capital_gains_type, visual_style="bold" + border_suffix, data_style="default")
-            self._fill_cell(sheet, row_index, 4, yearly_gain_loss.transaction_type.value.upper(), visual_style="bold" + border_suffix, data_style="default")
+            self._fill_cell(
+                sheet, row_index, 4, yearly_gain_loss.transaction_type.get_translation().upper(), visual_style="bold" + border_suffix, data_style="default"
+            )
             self._fill_cell(sheet, row_index, 5, yearly_gain_loss.crypto_amount, visual_style="transparent" + border_suffix, data_style="crypto")
             self._fill_cell(
                 sheet,
                 row_index,
                 6,
                 yearly_gain_loss.fiat_amount,
                 visual_style="taxable_event" + border_suffix,
@@ -752,15 +751,15 @@
             value = totals.setdefault(balance.holder, _ZERO)
             value += balance.final_balance
             totals[balance.holder] = value
             row_index += 1
 
         holder: str
         border_drawn: bool = False
-        for (holder, value) in sorted(totals.items()):
+        for holder, value in sorted(totals.items()):
             border_suffix: str = ""
             if not border_drawn:
                 border_suffix = "_border"
                 border_drawn = True
             self._fill_cell(sheet, row_index, 0, _("Total"), visual_style="bold" + border_suffix, data_style="default")
             self._fill_cell(sheet, row_index, 1, holder, visual_style="bold" + border_suffix, data_style="default")
             self._fill_cell(sheet, row_index, 2, "", visual_style="transparent" + border_suffix, data_style="default")
@@ -797,15 +796,14 @@
 
     def __get_in_out_sheet_row(self, transaction: AbstractTransaction) -> Optional[int]:
         if transaction not in self.__in_out_sheet_transaction_2_row:
             return None
         return self.__in_out_sheet_transaction_2_row[transaction]
 
     def __generate_gain_loss_detail(self, sheet: Any, asset: str, computed_data: ComputedData, row_index: int) -> int:
-
         row_index = self._fill_header(
             _("Gain / Loss Detail"), self.__gain_loss_detail_header_names_row_1, self.__gain_loss_detail_header_names_row_2, sheet, row_index, 0
         )
 
         gain_loss_set: GainLossSet = computed_data.gain_loss_set
 
         taxable_event_style_modifier: str = ""
@@ -824,15 +822,15 @@
             border_suffix = border_style.border_suffix
             transparent_style: str = f"transparent{border_suffix}"
             taxable_event_style: str = f"taxable_event{taxable_event_style_modifier}{border_suffix}"
             highlighted_style: str = f"highlighted{border_suffix}"
             current_taxable_event_fraction: int = gain_loss_set.get_taxable_event_fraction(gain_loss) + 1
             total_taxable_event_fractions: int = gain_loss_set.get_taxable_event_number_of_fractions(gain_loss.taxable_event)
             transaction_type: str = (
-                f"{self._get_table_type_from_transaction(gain_loss.taxable_event)} / " f"{gain_loss.taxable_event.transaction_type.value.upper()}"
+                f"{self._get_table_type_from_transaction(gain_loss.taxable_event)} / " f"{gain_loss.taxable_event.transaction_type.get_translation().upper()}"
             )
             taxable_event_note: str = (
                 f"{current_taxable_event_fraction}/"
                 f"{total_taxable_event_fractions}: "
                 f"{gain_loss.crypto_amount:.8f} of "
                 f"{gain_loss.taxable_event.crypto_balance_change:.8f} "
                 f"{asset}"
@@ -998,15 +996,19 @@
                 2,
                 self.__get_hyperlinked_summary_value(asset, gain_loss.fiat_gain_loss, year),
                 visual_style=visual_style,
                 data_style="fiat",
             )
             self._fill_cell(sheet, row_index, 3, self.__get_hyperlinked_summary_value(asset, capital_gains_type, year), visual_style=visual_style)
             self._fill_cell(
-                sheet, row_index, 4, self.__get_hyperlinked_summary_value(asset, gain_loss.transaction_type.value.upper(), year), visual_style=visual_style
+                sheet,
+                row_index,
+                4,
+                self.__get_hyperlinked_summary_value(asset, gain_loss.transaction_type.get_translation().upper(), year),
+                visual_style=visual_style,
             )
             self._fill_cell(
                 sheet, row_index, 5, self.__get_hyperlinked_summary_value(asset, gain_loss.crypto_amount, year), visual_style=visual_style, data_style="crypto"
             )
             self._fill_cell(
                 sheet,
                 row_index,
```

### Comparing `rp2-1.4.2/src/rp2/plugin/report/us/tax_report_us.py` & `rp2-1.5.0/src/rp2/plugin/report/us/tax_report_us.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,14 @@
 
 _TYPE_TO_SHEET: Dict[TransactionType, str] = {
     transaction_type: sheet_name for sheet_name, transaction_types in _SHEET_TO_TYPES.items() for transaction_type in transaction_types
 }
 
 
 class Generator(AbstractODSGenerator):
-
     MIN_ROWS: int = 20
     MAX_COLUMNS: int = 20
     OUTPUT_FILE: str = "tax_report_us.ods"
 
     HEADER_ROWS = 7
 
     def generate(
@@ -83,15 +82,14 @@
         asset_to_computed_data: Dict[str, ComputedData],
         output_dir_path: str,
         output_file_prefix: str,
         from_date: date,
         to_date: date,
         generation_language: str,
     ) -> None:
-
         row_indexes: Dict[str, int] = {sheet_name.value: self.HEADER_ROWS for sheet_name in SheetNames}
 
         if not isinstance(asset_to_computed_data, Dict):
             raise RP2TypeError(f"Parameter 'asset_to_computed_data' has non-Dict value {asset_to_computed_data}")
 
         template_path: str = self._get_template_path("tax_report_us", country, generation_language)
 
@@ -130,15 +128,14 @@
         for index in reversed(sheet_indexes_to_remove):
             del output_file.sheets[index]
 
         output_file.save()
         LOGGER.info("Plugin '%s' output: %s", __name__, Path(output_file.docname).resolve())
 
     def __generate(self, output_file: Any, asset: str, gain_loss_set: GainLossSet, row_indexes: Dict[str, int]) -> None:
-
         sheet: Any
         for sheet in output_file.sheets:
             if sheet.name == "Legend":
                 continue
             sheet_types: Tuple[TransactionType, ...] = _SHEET_TO_TYPES[sheet.name]
             for sheet_type in sheet_types:
                 sheet.append_rows(self.MIN_ROWS + gain_loss_set.get_transaction_type_count(sheet_type) + 1)
```

### Comparing `rp2-1.4.2/src/rp2/rp2_configuration_translator.py` & `rp2-1.5.0/src/rp2/rp2_configuration_translator.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,14 @@
 
     LOGGER.info("Input JSON configuration file: %s", json_file_name)
     LOGGER.info("Output INI configuration file: %s", ini_file_name)
     LOGGER.info("Done")
 
 
 def _setup_argument_parser() -> ArgumentParser:
-
     parser: ArgumentParser = ArgumentParser(
         description=("Convert a JSON-format RP2 configuration file to INI format"),
         formatter_class=RawTextHelpFormatter,
     )
 
     parser.add_argument(
         "-f",
```

### Comparing `rp2-1.4.2/src/rp2/rp2_decimal.py` & `rp2-1.5.0/src/rp2/rp2_decimal.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 CRYPTO_DECIMAL_MASK: Decimal = Decimal("1." + "0" * int(CRYPTO_DECIMALS))
 
 FIAT_DECIMALS: int = 2
 FIAT_DECIMAL_MASK: Decimal = Decimal("1." + "0" * int(FIAT_DECIMALS))
 
 
 class RP2Decimal(Decimal):
-
     # RP2Decimal initialization code. In Python there is no static constructor: the closest alternative is to add static initialization code
     # directly inside the class. Use arbitrarily high precision (quintillion + CRYPTO_DECIMALS digits)
     getcontext().prec = CRYPTO_DECIMALS + 18
     getcontext().traps[FloatOperation] = True
 
     @classmethod
     def is_equal_within_precision(cls, first: "RP2Decimal", second: "RP2Decimal", precision_mask: Decimal) -> bool:
```

### Comparing `rp2-1.4.2/src/rp2/rp2_error.py` & `rp2-1.5.0/src/rp2/rp2_error.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/rp2_main.py` & `rp2-1.5.0/src/rp2/rp2_main.py`

 * *Files 0% similar despite different names*

```diff
@@ -38,15 +38,15 @@
 )
 from rp2.input_data import InputData
 from rp2.localization import set_generation_language
 from rp2.logger import LOG_FILE, LOGGER
 from rp2.ods_parser import open_ods, parse_ods
 from rp2.tax_engine import compute_tax
 
-_VERSION: str = "1.4.2"
+_VERSION: str = "1.5.0"
 
 _ACCOUNTING_METHOD_PACKAGE = "rp2.plugin.accounting_method"
 
 
 def rp2_main(country: AbstractCountry) -> None:
     if "RP2_ENABLE_PROFILER" in os.environ:
         cProfile.runctx("_rp2_main_internal(country)", globals(), locals())
@@ -245,15 +245,14 @@
         LOGGER.error("No accounting method plugins found. Exiting...")
         sys.exit(1)
 
     return sorted(result)
 
 
 def _setup_argument_parser(country: AbstractCountry) -> ArgumentParser:
-
     accounting_methods = _validate_accounting_methods(country)
 
     parser: ArgumentParser = ArgumentParser(
         description=(
             "Generate capital gain/loss report and balances for crypto holdings. Links:\n"
             "- documentation: https://github.com/eprbell/rp2/blob/main/README.md\n"
             "- FAQ: https://github.com/eprbell/rp2/blob/main/docs/user_faq.md\n"
```

### Comparing `rp2-1.4.2/src/rp2/tax_engine.py` & `rp2-1.5.0/src/rp2/tax_engine.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2/transaction_set.py` & `rp2-1.5.0/src/rp2/transaction_set.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/src/rp2.egg-info/PKG-INFO` & `rp2-1.5.0/src/rp2.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: rp2
-Version: 1.4.2
+Version: 1.5.0
 Summary: Privacy-focused, free, non-commercial, open-source, community-driven cryptocurrency tax calculator: it handles multiple coins/exchanges and computes long/short-term capital gains, cost bases, in/out lot relationships/fractioning, and account balances. It supports the FIFO accounting method, it features transparent computation for easy result verification, and it generates reports that tax accountants can understand, even if they are not cryptocurrency experts (e.g. form 8949).
 Home-page: https://github.com/eprbell/rp2
 Author: eprbell
 License: Apache License 2.0
 Project-URL: Source Code, https://github.com/eprbell/rp2
 Project-URL: Developer Documentation, https://github.com/eprbell/rp2/blob/main/README.dev.md
 Project-URL: User Documentation, https://github.com/eprbell/rp2/blob/main/README.md
 Project-URL: Contact, https://eprbell.github.io/eprbell/about.html
-Keywords: accounting,altcoin,bitcoin,BTC,capital gains,cost basis,crypto,cryptocurrency,ETH,ethereum,finance,form 8949,NFT,privacy,wallet,tax
+Keywords: accounting,altcoin,bitcoin,BTC,capital gains,cost basis,crypto,cryptocurrency,DeFi,ETH,ethereum,finance,form 8949,NFT,privacy,wallet,tax
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
@@ -37,25 +37,25 @@
 <!--- distributed under the License is distributed on an "AS IS" BASIS, --->
 <!--- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. --->
 <!--- See the License for the specific language governing permissions and --->
 <!--- limitations under the License. --->
 
 ![RP2 Logo](https://raw.githubusercontent.com/eprbell/rp2/main/docs/images/rp2_header.png)
 
-# RP2 v1.4.2
+# RP2 v1.5.0
 Privacy-focused, free, powerful crypto tax calculator
 
 [![Static Analysis / Main Branch](https://github.com/eprbell/rp2/actions/workflows/static_analysis.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/static_analysis.yml)
 [![Documentation Check / Main Branch](https://github.com/eprbell/rp2/actions/workflows/documentation_check.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/documentation_check.yml)
 [![Unix Unit Tests / Main Branch](https://github.com/eprbell/rp2/actions/workflows/unix_unit_tests.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/unix_unit_tests.yml)
 [![Windows Unit Tests / Main Branch](https://github.com/eprbell/rp2/actions/workflows/windows_unit_tests.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/windows_unit_tests.yml)
 [![CodeQL/Main Branch](https://github.com/eprbell/rp2/actions/workflows/codeql-analysis.yml/badge.svg)](https://github.com/eprbell/rp2/actions/workflows/codeql-analysis.yml)
-
+<!-- markdown-link-check-disable -->
 [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=I%20use%20RP2,%20the%20privacy-focused,%20open%20source,%20free,%20non-commercial%20crypto%20tax%20calculator&url=https://github.com/eprbell/rp2/?anything)
-
+<!-- markdown-link-check-enable -->
 ## Table of Contents
 * **[Introduction](https://github.com/eprbell/rp2/blob/main/README.md#introduction)**
   * [How RP2 Operates](https://github.com/eprbell/rp2/blob/main/README.md#how-rp2-operates)
 * **[License](https://github.com/eprbell/rp2/blob/main/README.md#license)**
 * **[Download](https://github.com/eprbell/rp2/blob/main/README.md#download)**
 * **[Installation](https://github.com/eprbell/rp2/blob/main/README.md#installation)**
   * [Ubuntu Linux](https://github.com/eprbell/rp2/blob/main/README.md#installation-on-ubuntu-linux)
@@ -69,30 +69,30 @@
 * **[Reporting Bugs](https://github.com/eprbell/rp2/blob/main/README.md#reporting-bugs)**
 * **[Contributing](https://github.com/eprbell/rp2/blob/main/README.md#contributing)**
 * **[Developer Documentation](https://github.com/eprbell/rp2/blob/main/README.md#developer-documentation)**
 * **[Frequently Asked Questions](https://github.com/eprbell/rp2/blob/main/README.md#frequently-asked-questions)**
 * **[Change Log](https://github.com/eprbell/rp2/blob/main/README.md#change-log)**
 
 ## Introduction
-[RP2](https://github.com/eprbell/rp2) is a privacy-focused, free, non-commercial, open-source, community-driven cryptocurrency tax calculator. Preparing crypto taxes can be a daunting and error-prone task, especially if multiple transactions, coins, exchanges and wallets are involved. This task could be delegated to a crypto tax preparation service, but many crypto users value their privacy and prefer not to send their transaction information to third parties unnecessarily. Additionally, many of these services cost money. RP2 solves all of these problems:
+[RP2](https://github.com/eprbell/rp2) is a privacy-focused, free, non-commercial, open-source, community-driven cryptocurrency tax calculator for multiple countries (currently US, Japan and Spain are supported). Preparing crypto taxes can be a daunting and error-prone task, especially if multiple transactions, coins, exchanges and wallets are involved. This task could be delegated to a crypto tax preparation service, but many crypto users value their privacy and prefer not to send their transaction information to third parties unnecessarily. Additionally, many of these services cost money. RP2 solves all of these problems:
 * it manages the complexity related to coin flows and tax calculation and it generates [reports that accountants can understand](https://github.com/eprbell/rp2/blob/main/docs/output_files.md#advisor-friendly-report-tax-report-us-output) (in the format of form 8949, for the US case), even if they are not cryptocurrency experts;
 * it prioritizes user privacy by storing crypto transactions and tax results on the user's computer and not sending them anywhere else;
 * it's 100% free, open-source and non-commercial.
 
 This means that with RP2 there are no transaction limits, no premium versions, no payment requests, no personal data sent to a server (at risk of being hacked), no account creation, no unauditable source code.
 
 Another unique advantage of RP2 is [transparent computation](https://github.com/eprbell/rp2/blob/main/docs/output_files.md#transparent-computation-rp2-full-report-output): RP2 generates full computation details for every lot fraction, so that it's possible to:
 * verify step-by-step how RP2 reaches the final result;
 * track down every lot fraction and its accounting details, in case of an audit.
 
-RP2 currently supports the [FIFO](https://www.investopedia.com/terms/f/fifo.asp) accounting method for US taxes and the Total Average Method for Japanese taxes.
+RP2 currently supports the [FIFO](https://www.investopedia.com/terms/f/fifo.asp) accounting method for US and Spanish taxes and the Total Average Method for Japanese taxes.
 
 RP2 reads a configuration file and an input spreadsheet containing crypto transactions. These [input files](https://github.com/eprbell/rp2/blob/main/docs/input_files.md) can be generated either manually or automatically using [DaLI](https://github.com/eprbell/dali-rp2), a RP2 data loader and input generator (which is also privacy-focused, free, non-commercial, open-source and community-driven). After parsing the input, RP2 uses high-precision math to calculate long/short term capital gains, cost bases, balances, average price, in/out lot relationships/fractions, and finally it generates [output files](https://github.com/eprbell/rp2/blob/main/docs/output_files.md).
 
-RP2 has a programmable plugin architecture for [output generators](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-a-new-report-generator), [accounting methods](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-a-new-accounting-method) and [countries](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-support-for-a-new-country) (currently US and Japan are supported). The builtin output generator plugins are in part generic and in part country-specific, but RP2's architecture makes it possible to contribute additional generators for different countries or for different country-based cases. The builtin output generator plugins are:
+RP2 has a programmable plugin architecture for [output generators](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-a-new-report-generator), [accounting methods](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-a-new-accounting-method) and [countries](https://github.com/eprbell/rp2/tree/main/README.dev.md#adding-support-for-a-new-country). The builtin output generator plugins are in part generic and in part country-specific, but RP2's architecture makes it possible to contribute additional generators for different countries or for different country-based cases. The builtin output generator plugins are:
 * tax_report_us: generates a US-specific tax report meant to be read by tax preparers (in the format of form 8949);
 * tax_report_jp: generates a Japan-specific tax report meant to be read by tax preparers;
 * rp2_full_report: generates a comprehensive report (valid for any country), with complete transaction history, lot relationships/fractions and computation details;
 * open_positions: geterates a report (valid for any country) on assets with non-zero crypto balance: unrealized gains / losses, portfolio weighting, and more.
 
 RP2 has extensive [unit test](https://github.com/eprbell/rp2/tree/main/tests/) coverage to reduce the risk of regression.
 
@@ -252,14 +252,17 @@
 <!--- distributed under the License is distributed on an "AS IS" BASIS, --->
 <!--- WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. --->
 <!--- See the License for the specific language governing permissions and --->
 <!--- limitations under the License. --->
 
 # RP2 Change Log
 
+## 1.5.0
+* added support for Spain (see #97)
+
 ## 1.4.2
 * fixed small bug in rp2_full_report generator: OUT transactions had slightly incorrect fiat_out field. The displayed value was fiat_out_no_fee - fiat fee, instead of fiat_out_no_fee. This bug didn't affect actual tax computation or the tax_report output: it only affected the fiat_out field in the OUT table of rp2_full_report.
 
 ## 1.4.1
 * added new RP2RuntimeError to handle non-recoverable problems without using Exception
 
 ## 1.4.0
```

### Comparing `rp2-1.4.2/src/rp2.egg-info/SOURCES.txt` & `rp2-1.5.0/src/rp2.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -33,23 +33,25 @@
 input/test_data2.ods
 input/test_data3.ods
 input/test_data4.ods
 input/test_data_multi_method.ods
 input/test_hifo.ods
 input/test_hifo2.ods
 input/test_many_year_data.ods
+input/golden/crypto_example_es_es_fifo_rp2_full_report.ods
 input/golden/crypto_example_fifo_rp2_full_report.ods
 input/golden/crypto_example_fifo_tax_report_us.ods
 input/golden/crypto_example_hifo_rp2_full_report.ods
 input/golden/crypto_example_hifo_tax_report_us.ods
 input/golden/crypto_example_jp_en_fifo_open_positions.ods
 input/golden/crypto_example_jp_en_fifo_rp2_full_report.ods
 input/golden/crypto_example_jp_en_fifo_tax_report_jp.ods
 input/golden/crypto_example_lifo_rp2_full_report.ods
 input/golden/crypto_example_lifo_tax_report_us.ods
+input/golden/test_data2_es_es_fifo_rp2_full_report.ods
 input/golden/test_data2_fifo_rp2_full_report.ods
 input/golden/test_data2_fifo_tax_report_us.ods
 input/golden/test_data2_hifo_rp2_full_report.ods
 input/golden/test_data2_hifo_tax_report_us.ods
 input/golden/test_data2_jp_en_fifo_open_positions.ods
 input/golden/test_data2_jp_en_fifo_rp2_full_report.ods
 input/golden/test_data2_jp_en_fifo_tax_report_jp.ods
@@ -57,32 +59,35 @@
 input/golden/test_data2_lifo_tax_report_us.ods
 input/golden/test_data3_2019-12-01_2020-04-01_fifo_rp2_full_report.ods
 input/golden/test_data3_2019-12-01_2020-04-01_fifo_tax_report_us.ods
 input/golden/test_data3_2019-12-01_2020-04-01_hifo_rp2_full_report.ods
 input/golden/test_data3_2019-12-01_2020-04-01_hifo_tax_report_us.ods
 input/golden/test_data3_2019-12-01_2020-04-01_lifo_rp2_full_report.ods
 input/golden/test_data3_2019-12-01_2020-04-01_lifo_tax_report_us.ods
+input/golden/test_data3_es_es_fifo_rp2_full_report.ods
 input/golden/test_data3_fifo_rp2_full_report.ods
 input/golden/test_data3_fifo_tax_report_us.ods
 input/golden/test_data3_hifo_rp2_full_report.ods
 input/golden/test_data3_hifo_tax_report_us.ods
 input/golden/test_data3_jp_en_fifo_open_positions.ods
 input/golden/test_data3_jp_en_fifo_rp2_full_report.ods
 input/golden/test_data3_jp_en_fifo_tax_report_jp.ods
 input/golden/test_data3_lifo_rp2_full_report.ods
 input/golden/test_data3_lifo_tax_report_us.ods
+input/golden/test_data4_es_es_fifo_rp2_full_report.ods
 input/golden/test_data4_fifo_rp2_full_report.ods
 input/golden/test_data4_fifo_tax_report_us.ods
 input/golden/test_data4_hifo_rp2_full_report.ods
 input/golden/test_data4_hifo_tax_report_us.ods
 input/golden/test_data4_jp_en_fifo_open_positions.ods
 input/golden/test_data4_jp_en_fifo_rp2_full_report.ods
 input/golden/test_data4_jp_en_fifo_tax_report_jp.ods
 input/golden/test_data4_lifo_rp2_full_report.ods
 input/golden/test_data4_lifo_tax_report_us.ods
+input/golden/test_data_es_es_fifo_rp2_full_report.ods
 input/golden/test_data_fifo_rp2_full_report.ods
 input/golden/test_data_fifo_tax_report_us.ods
 input/golden/test_data_hifo_rp2_full_report.ods
 input/golden/test_data_hifo_tax_report_us.ods
 input/golden/test_data_jp_en_fifo_open_positions.ods
 input/golden/test_data_jp_en_fifo_rp2_full_report.ods
 input/golden/test_data_jp_en_fifo_tax_report_jp.ods
@@ -132,14 +137,15 @@
 input/golden/test_many_year_data_2019-01-01_2019-12-31_fifo_tax_report_us.ods
 input/golden/test_many_year_data_2019-01-01_infinity_fifo_rp2_full_report.ods
 input/golden/test_many_year_data_2019-01-01_infinity_fifo_tax_report_us.ods
 input/golden/test_many_year_data_2020-01-01_infinity_fifo_rp2_full_report.ods
 input/golden/test_many_year_data_2020-01-01_infinity_fifo_tax_report_us.ods
 input/golden/test_many_year_data_2021-01-01_infinity_fifo_rp2_full_report.ods
 input/golden/test_many_year_data_2021-01-01_infinity_fifo_tax_report_us.ods
+input/golden/test_many_year_data_es_es_fifo_rp2_full_report.ods
 input/golden/test_many_year_data_fifo_rp2_full_report.ods
 input/golden/test_many_year_data_fifo_tax_report_us.ods
 input/golden/test_many_year_data_hifo_rp2_full_report.ods
 input/golden/test_many_year_data_hifo_tax_report_us.ods
 input/golden/test_many_year_data_jp_en_fifo_open_positions.ods
 input/golden/test_many_year_data_jp_en_fifo_rp2_full_report.ods
 input/golden/test_many_year_data_jp_en_fifo_tax_report_jp.ods
@@ -179,38 +185,46 @@
 src/rp2.egg-info/dependency_links.txt
 src/rp2.egg-info/entry_points.txt
 src/rp2.egg-info/requires.txt
 src/rp2.egg-info/top_level.txt
 src/rp2/locales/messages.pot
 src/rp2/locales/en/LC_MESSAGES/messages.mo
 src/rp2/locales/en/LC_MESSAGES/messages.po
+src/rp2/locales/es/LC_MESSAGES/messages.mo
+src/rp2/locales/es/LC_MESSAGES/messages.po
 src/rp2/locales/ja/LC_MESSAGES/messages.mo
 src/rp2/locales/ja/LC_MESSAGES/messages.po
 src/rp2/locales/kl/LC_MESSAGES/messages.mo
 src/rp2/locales/kl/LC_MESSAGES/messages.po
 src/rp2/plugin/__init__.py
 src/rp2/plugin/accounting_method/__init__.py
 src/rp2/plugin/accounting_method/fifo.py
 src/rp2/plugin/accounting_method/hifo.py
 src/rp2/plugin/accounting_method/lifo.py
 src/rp2/plugin/country/__init__.py
+src/rp2/plugin/country/es.py
 src/rp2/plugin/country/jp.py
 src/rp2/plugin/country/us.py
 src/rp2/plugin/report/__init__.py
 src/rp2/plugin/report/abstract_ods_generator.py
 src/rp2/plugin/report/open_positions.py
 src/rp2/plugin/report/rp2_full_report.py
 src/rp2/plugin/report/data/__init__.py
-src/rp2/plugin/report/data/template_open_positions.ods
+src/rp2/plugin/report/data/es/template_open_positions_es.ods
+src/rp2/plugin/report/data/es/template_rp2_full_report_es.ods
+src/rp2/plugin/report/data/jp/template_open_positions_en.ods
+src/rp2/plugin/report/data/jp/template_open_positions_kl.ods
 src/rp2/plugin/report/data/jp/template_rp2_full_report_en.ods
 src/rp2/plugin/report/data/jp/template_rp2_full_report_kl.ods
 src/rp2/plugin/report/data/jp/template_tax_report_jp_en.ods
 src/rp2/plugin/report/data/jp/template_tax_report_jp_kl.ods
+src/rp2/plugin/report/data/us/template_open_positions_en.ods
 src/rp2/plugin/report/data/us/template_rp2_full_report_en.ods
 src/rp2/plugin/report/data/us/template_tax_report_us_en.ods
+src/rp2/plugin/report/es/__init__.py
 src/rp2/plugin/report/jp/__init__.py
 src/rp2/plugin/report/jp/tax_report_jp.py
 src/rp2/plugin/report/us/__init__.py
 src/rp2/plugin/report/us/tax_report_us.py
 tests/abstract_test_ods_output_diff.py
 tests/ods_diff.py
 tests/rp2_test_output.py
@@ -219,12 +233,13 @@
 tests/test_gain_loss_set.py
 tests/test_in_transaction.py
 tests/test_input_parser.py
 tests/test_intra_transaction.py
 tests/test_large_input.py
 tests/test_localized_output.py
 tests/test_ods_output_diff.py
+tests/test_ods_output_diff_es.py
 tests/test_ods_output_diff_jp.py
 tests/test_out_transaction.py
 tests/test_rp2_decimal.py
 tests/test_tax_engine.py
 tests/test_transaction_set.py
```

### Comparing `rp2-1.4.2/tests/abstract_test_ods_output_diff.py` & `rp2-1.5.0/tests/abstract_test_ods_output_diff.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
     OPEN_POSITIONS = "open_positions"
     RP2_FULL_REPORT = "rp2_full_report"
     TAX_REPORT_JP = "tax_report_jp"
     TAX_REPORT_US = "tax_report_us"
 
 
 class AbstractTestODSOutputDiff(unittest.TestCase):
-
     # Temporarily removed lifo and hifo due to https://github.com/eprbell/rp2/issues/79
     METHODS: List[str] = ["fifo"]
 
     def setUp(self) -> None:
         self.maxDiff = None  # pylint: disable=invalid-name
 
     @staticmethod
```

### Comparing `rp2-1.4.2/tests/ods_diff.py` & `rp2-1.5.0/tests/ods_diff.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,14 @@
     if value is None:
         value = ""
 
     return value
 
 
 def ods_diff(file1_path: Path, file2_path: Path, generate_ascii_representation: bool) -> str:  # pylint: disable=too-many-branches
-
     if not file1_path.exists():
         return f"Error: {file1_path} does not exist"
     if not file2_path.exists():
         return f"Error: {file2_path} does not exist"
 
     file1: Any = ezodf.opendoc(str(file1_path))
     file2: Any = ezodf.opendoc(str(file2_path))
@@ -120,15 +119,14 @@
                 temp_file.flush()
                 print(f"ASCII representation of {file_path}: {temp_file.name}")
 
     return "\n".join(unified_diff(contents1, contents2, lineterm=""))
 
 
 def main() -> None:
-
     parser: ArgumentParser = ArgumentParser(description="Generate yearly capital gain/loss report and account balances for crypto holdings.")
     parser.add_argument(
         "-a",
         "--ascii-representation",
         action="store_true",
         help="Save ASCII representation of ODS files in temporary directory",
     )
```

### Comparing `rp2-1.4.2/tests/rp2_test_output.py` & `rp2-1.5.0/tests/rp2_test_output.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/tests/test_configuration.py` & `rp2-1.5.0/tests/test_configuration.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/tests/test_gain_loss.py` & `rp2-1.5.0/tests/test_gain_loss.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/tests/test_gain_loss_set.py` & `rp2-1.5.0/tests/test_gain_loss_set.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/tests/test_in_transaction.py` & `rp2-1.5.0/tests/test_in_transaction.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/tests/test_input_parser.py` & `rp2-1.5.0/tests/test_input_parser.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
     def test_good_input(self) -> None:
         self._verify_good_sheet("B1", out_empty=True, intra_empty=True)
         self._verify_good_sheet("B2", out_empty=False, intra_empty=True)
         self._verify_good_sheet("B3", out_empty=True, intra_empty=False)
         self._verify_good_sheet("B4", out_empty=False, intra_empty=False)
 
     def _verify_good_sheet(self, sheet_name: str, out_empty: bool, intra_empty: bool) -> None:
-
         asset = sheet_name
         input_file_handle: object = open_ods(configuration=self._good_input_configuration, input_file_path="./input/test_data.ods")
         input_data: InputData = parse_ods(self._good_input_configuration, asset, input_file_handle)
 
         # In table is always present
         self._verify_non_empty_in_table(input_data.unfiltered_in_transaction_set, asset)
         if out_empty:
@@ -282,15 +281,14 @@
             self.assertEqual(transaction.fiat_balance_change, fiat_balance_change)
             self.assertEqual(transaction.is_taxable(), is_taxable)
             previous_transaction = transaction
             count += 1
         self.assertEqual(count, 4)
 
     def test_bad_input(self) -> None:
-
         sheets_to_expected_messages: Dict[str, ErrorAndMessage] = {
             "B1": ErrorAndMessage(RP2ValueError, "IN table not found"),
             "B2": ErrorAndMessage(RP2ValueError, 'Found an invalid cell "foo" while looking for a table-begin token'),
             "B3": ErrorAndMessage(RP2ValueError, 'Found an invalid cell "bar" while looking for a table-begin token'),
             "B4": ErrorAndMessage(RP2ValueError, "Found end-table keyword without having found a table-begin keyword first"),
             "B5": ErrorAndMessage(RP2ValueError, "Found end-table keyword without having found a table-begin keyword first"),
             "B6": ErrorAndMessage(RP2ValueError, "TABLE END not found for EntrySetType.IN table"),
```

### Comparing `rp2-1.4.2/tests/test_intra_transaction.py` & `rp2-1.5.0/tests/test_intra_transaction.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/tests/test_large_input.py` & `rp2-1.5.0/tests/test_large_input.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,15 +25,14 @@
 
 from rp2.rp2_error import RP2RuntimeError
 
 ROOT_PATH: Path = Path(os.path.dirname(__file__)).parent.absolute()
 
 
 class TestLargeInput(AbstractTestODSOutputDiff):
-
     output_dir: Path
 
     @classmethod
     def setUpClass(cls) -> None:
         cls.output_dir = ROOT_PATH / Path("output") / Path(cls.__module__)
 
         shutil.rmtree(cls.output_dir, ignore_errors=True)
@@ -45,15 +44,14 @@
             )
 
     def setUp(self) -> None:
         self.maxDiff = None  # pylint: disable=invalid-name
 
     @staticmethod
     def _fill_row(sheet: Any, row_index: int, row: List[Any]) -> int:
-
         for col_index, element in enumerate(row):
             sheet[row_index, col_index].set_value(element)
         return row_index + 1
 
     @classmethod
     def _generate_large_input(cls, output_dir: Path) -> None:
         output_file_path: Path = output_dir / Path("test_large_input.ods")
```

### Comparing `rp2-1.4.2/tests/test_localized_output.py` & `rp2-1.5.0/tests/test_localized_output.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 from abstract_test_ods_output_diff import AbstractTestODSOutputDiff, OutputPlugins
 
 ROOT_PATH: Path = Path(os.path.dirname(__file__)).parent.absolute()
 
 
 class TestLocalizedOutput(AbstractTestODSOutputDiff):  # pylint: disable=too-many-public-methods
-
     output_dir: Path
 
     @classmethod
     def setUpClass(cls) -> None:
         cls.output_dir = ROOT_PATH / Path("output") / Path(cls.__module__)
 
         shutil.rmtree(cls.output_dir, ignore_errors=True)
```

### Comparing `rp2-1.4.2/tests/test_ods_output_diff.py` & `rp2-1.5.0/tests/test_ods_output_diff.py`

 * *Files 0% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 
 from abstract_test_ods_output_diff import AbstractTestODSOutputDiff, OutputPlugins
 
 ROOT_PATH: Path = Path(os.path.dirname(__file__)).parent.absolute()
 
 
 class TestODSOutputDiff(AbstractTestODSOutputDiff):  # pylint: disable=too-many-public-methods
-
     output_dir: Path
 
     @classmethod
     def setUpClass(cls) -> None:
         cls.output_dir = ROOT_PATH / Path("output") / Path(cls.__module__)
 
         shutil.rmtree(cls.output_dir, ignore_errors=True)
```

### Comparing `rp2-1.4.2/tests/test_ods_output_diff_jp.py` & `rp2-1.5.0/tests/test_ods_output_diff_jp.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,14 @@
 
 from abstract_test_ods_output_diff import AbstractTestODSOutputDiff, OutputPlugins
 
 ROOT_PATH: Path = Path(os.path.dirname(__file__)).parent.absolute()
 
 
 class TestODSOutputDiff(AbstractTestODSOutputDiff):  # pylint: disable=too-many-public-methods
-
     output_dir: Path
 
     @classmethod
     def setUpClass(cls) -> None:
         cls.output_dir = ROOT_PATH / Path("output") / Path(cls.__module__)
 
         shutil.rmtree(cls.output_dir, ignore_errors=True)
```

### Comparing `rp2-1.4.2/tests/test_out_transaction.py` & `rp2-1.5.0/tests/test_out_transaction.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/tests/test_rp2_decimal.py` & `rp2-1.5.0/tests/test_rp2_decimal.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/tests/test_tax_engine.py` & `rp2-1.5.0/tests/test_tax_engine.py`

 * *Files identical despite different names*

### Comparing `rp2-1.4.2/tests/test_transaction_set.py` & `rp2-1.5.0/tests/test_transaction_set.py`

 * *Files identical despite different names*

