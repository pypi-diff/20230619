# Comparing `tmp/funasr-0.6.1.tar.gz` & `tmp/funasr-0.6.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "funasr-0.6.1.tar", last modified: Tue Jun 13 03:14:17 2023, max compression
+gzip compressed data, was "funasr-0.6.2.tar", last modified: Mon Jun 19 11:14:29 2023, max compression
```

## Comparing `funasr-0.6.1.tar` & `funasr-0.6.2.tar`

### file list

```diff
@@ -1,424 +1,424 @@
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.938001 funasr-0.6.1/
--rw-r--r--   0 zhifu      (502) staff       (20)     8368 2023-06-13 03:14:17.936643 funasr-0.6.1/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)     7368 2023-06-05 05:14:38.000000 funasr-0.6.1/README.md
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:16.302715 funasr-0.6.1/funasr/
--rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:16.375554 funasr-0.6.1/funasr/bin/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/bin/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/bin/aggregate_stats_dirs.py
--rw-r--r--   0 zhifu      (502) staff       (20)    69576 2023-06-12 13:47:19.000000 funasr-0.6.1/funasr/bin/asr_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    72856 2023-06-12 10:51:43.000000 funasr-0.6.1/funasr/bin/asr_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1715 2023-05-24 02:58:26.000000 funasr-0.6.1/funasr/bin/asr_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5416 2023-06-06 13:50:59.000000 funasr-0.6.1/funasr/bin/build_trainer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/bin/data2vec_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    12198 2023-05-25 08:06:43.000000 funasr-0.6.1/funasr/bin/diar_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    18753 2023-05-22 05:06:44.000000 funasr-0.6.1/funasr/bin/diar_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1180 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/bin/diar_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15054 2023-05-23 08:26:46.000000 funasr-0.6.1/funasr/bin/lm_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1189 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/bin/lm_train.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12512 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/bin/punc_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     8675 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/bin/punc_inference_launch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      999 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/bin/punc_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     1241 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/bin/sa_asr_train.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5299 2023-05-22 05:06:44.000000 funasr-0.6.1/funasr/bin/sv_infer.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    10573 2023-05-22 05:06:44.000000 funasr-0.6.1/funasr/bin/sv_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     8449 2023-02-11 09:29:33.000000 funasr-0.6.1/funasr/bin/tokenize_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3999 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/bin/tp_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10220 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/bin/tp_inference_launch.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    17699 2023-05-25 08:06:43.000000 funasr-0.6.1/funasr/bin/train.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7276 2023-06-06 13:50:59.000000 funasr-0.6.1/funasr/bin/vad_infer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13448 2023-05-22 05:06:44.000000 funasr-0.6.1/funasr/bin/vad_inference_launch.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:16.422916 funasr-0.6.1/funasr/build_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-05-18 12:04:14.000000 funasr-0.6.1/funasr/build_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3425 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/build_utils/build_args.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14060 2023-06-06 13:50:59.000000 funasr-0.6.1/funasr/build_utils/build_asr_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)      672 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/build_utils/build_dataloader.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9592 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/build_utils/build_diar_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1552 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/build_utils/build_distributed.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1418 2023-05-22 05:06:44.000000 funasr-0.6.1/funasr/build_utils/build_lm_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)      968 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/build_utils/build_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)      810 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/build_utils/build_optimizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2993 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/build_utils/build_pretrain_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2211 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/build_utils/build_punc_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1531 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/build_utils/build_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)    35626 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/build_utils/build_trainer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2196 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/build_utils/build_vad_model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:16.459792 funasr-0.6.1/funasr/datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4338 2023-02-09 08:39:15.000000 funasr-0.6.1/funasr/datasets/collate_fn.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15174 2023-04-17 03:36:48.000000 funasr-0.6.1/funasr/datasets/dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15562 2023-03-29 08:06:18.000000 funasr-0.6.1/funasr/datasets/iterable_dataset.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:16.548697 funasr-0.6.1/funasr/datasets/large_datasets/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/datasets/large_datasets/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3794 2023-06-06 13:50:59.000000 funasr-0.6.1/funasr/datasets/large_datasets/build_dataloader.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:16.581320 funasr-0.6.1/funasr/datasets/large_datasets/datapipes/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/datasets/large_datasets/datapipes/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.6.1/funasr/datasets/large_datasets/datapipes/batch.py
--rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/datasets/large_datasets/datapipes/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/datasets/large_datasets/datapipes/map.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10367 2023-06-06 13:50:59.000000 funasr-0.6.1/funasr/datasets/large_datasets/dataset.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:16.613612 funasr-0.6.1/funasr/datasets/large_datasets/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/datasets/large_datasets/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.6.1/funasr/datasets/large_datasets/utils/clipping.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.6.1/funasr/datasets/large_datasets/utils/filter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1566 2023-05-07 09:22:42.000000 funasr-0.6.1/funasr/datasets/large_datasets/utils/hotword_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/datasets/large_datasets/utils/low_frame_rate.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3303 2023-05-07 09:22:42.000000 funasr-0.6.1/funasr/datasets/large_datasets/utils/padding.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2582 2023-05-25 08:06:43.000000 funasr-0.6.1/funasr/datasets/large_datasets/utils/tokenize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/datasets/ms_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31032 2023-04-27 08:40:56.000000 funasr-0.6.1/funasr/datasets/preprocessor.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:16.617278 funasr-0.6.1/funasr/export/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.1/funasr/export/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10699 2023-05-12 02:41:22.000000 funasr-0.6.1/funasr/export/export_model.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:16.626290 funasr-0.6.1/funasr/export/models/
--rw-r--r--   0 zhifu      (502) staff       (20)     5127 2023-05-07 09:22:42.000000 funasr-0.6.1/funasr/export/models/CT_Transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1540 2023-04-17 03:36:48.000000 funasr-0.6.1/funasr/export/models/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:16.633599 funasr-0.6.1/funasr/export/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.1/funasr/export/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.6.1/funasr/export/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.6.1/funasr/export/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.6.1/funasr/export/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.6.1/funasr/export/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:16.637422 funasr-0.6.1/funasr/export/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.1/funasr/export/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.6.1/funasr/export/models/encoder/conformer_encoder.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.6.1/funasr/export/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-05-05 07:04:25.000000 funasr-0.6.1/funasr/export/models/encoder/sanm_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:16.656486 funasr-0.6.1/funasr/export/models/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.1/funasr/export/models/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.6.1/funasr/export/models/modules/decoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.6.1/funasr/export/models/modules/encoder_layer.py
--rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.6.1/funasr/export/models/modules/feedforward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.6.1/funasr/export/models/modules/multihead_att.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:16.658882 funasr-0.6.1/funasr/export/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.1/funasr/export/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.6.1/funasr/export/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:16.680888 funasr-0.6.1/funasr/export/test/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.6.1/funasr/export/test/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.6.1/funasr/export/test/test_onnx.py
--rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.6.1/funasr/export/test/test_onnx_punc.py
--rw-r--r--   0 zhifu      (502) staff       (20)      927 2023-05-22 05:06:44.000000 funasr-0.6.1/funasr/export/test/test_onnx_punc_vadrealtime.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.6.1/funasr/export/test/test_onnx_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-05-24 08:36:46.000000 funasr-0.6.1/funasr/export/test/test_torchscripts.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:16.682087 funasr-0.6.1/funasr/export/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.1/funasr/export/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.6.1/funasr/export/utils/torch_function.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:16.707720 funasr-0.6.1/funasr/fileio/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/fileio/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2383 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/fileio/datadir_writer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2357 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/fileio/npy_scp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2361 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/fileio/rand_gen_dataset.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2273 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/fileio/read_text.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4050 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/fileio/sound_scp.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:16.726802 funasr-0.6.1/funasr/iterators/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/iterators/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/iterators/abs_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7808 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/iterators/chunk_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1140 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/iterators/multiple_iter_factory.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5236 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/iterators/sequence_iter_factory.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:16.741567 funasr-0.6.1/funasr/layers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/layers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      358 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/layers/abs_normalize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/layers/complex_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3499 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/layers/global_mvn.py
--rw-r--r--   0 zhifu      (502) staff       (20)      348 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/layers/inversible_interface.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2539 2023-03-10 07:21:13.000000 funasr-0.6.1/funasr/layers/label_aggregation.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/layers/log_mel.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10488 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/layers/mask_along_axis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9033 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/layers/sinc_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8436 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/layers/stft.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/layers/time_warp.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2309 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/layers/utterance_mvn.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:16.743390 funasr-0.6.1/funasr/losses/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/losses/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4320 2023-05-09 03:02:42.000000 funasr-0.6.1/funasr/losses/label_smoothing_loss.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:16.746118 funasr-0.6.1/funasr/main_funcs/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/main_funcs/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4687 2023-04-12 07:23:40.000000 funasr-0.6.1/funasr/main_funcs/average_nbest_models.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/main_funcs/calculate_all_attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5018 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/main_funcs/collect_stats.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.6.1/funasr/main_funcs/pack_funcs.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.684727 funasr-0.6.1/funasr/models/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/models/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      319 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/models/base_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6541 2023-02-11 09:29:22.000000 funasr-0.6.1/funasr/models/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5285 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/models/data2vec.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.729051 funasr-0.6.1/funasr/models/decoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/models/decoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/models/decoder/abs_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    40834 2023-04-17 03:36:48.000000 funasr-0.6.1/funasr/models/decoder/contextual_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12133 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/models/decoder/rnn_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8355 2023-05-09 09:17:41.000000 funasr-0.6.1/funasr/models/decoder/rnnt_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    75478 2023-06-06 13:50:59.000000 funasr-0.6.1/funasr/models/decoder/sanm_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/models/decoder/sv_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    43192 2023-05-09 03:02:42.000000 funasr-0.6.1/funasr/models/decoder/transformer_decoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16699 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/models/e2e_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/models/e2e_asr_common.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15709 2023-05-07 09:22:42.000000 funasr-0.6.1/funasr/models/e2e_asr_contextual_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11838 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/models/e2e_asr_mfcca.py
--rw-r--r--   0 zhifu      (502) staff       (20)   100491 2023-06-06 13:50:59.000000 funasr-0.6.1/funasr/models/e2e_asr_paraformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    35111 2023-06-06 13:50:59.000000 funasr-0.6.1/funasr/models/e2e_asr_transducer.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10226 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/models/e2e_diar_eend_ola.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20567 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/models/e2e_diar_sond.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19490 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/models/e2e_sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10084 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/models/e2e_sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6682 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/models/e2e_tp.py
--rw-r--r--   0 zhifu      (502) staff       (20)    51719 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/models/e2e_uni_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    31858 2023-06-13 03:13:40.000000 funasr-0.6.1/funasr/models/e2e_vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.734247 funasr-0.6.1/funasr/models/encoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/models/encoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      502 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/models/encoder/abs_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    43621 2023-05-22 05:06:44.000000 funasr-0.6.1/funasr/models/encoder/conformer_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20992 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/models/encoder/data2vec_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.6.1/funasr/models/encoder/ecapa_tdnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.6.1/funasr/models/encoder/encoder_layer_mfcca.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.6.1/funasr/models/encoder/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17681 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/models/encoder/mfcca_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.736006 funasr-0.6.1/funasr/models/encoder/opennmt_encoders/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.6.1/funasr/models/encoder/opennmt_encoders/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.6.1/funasr/models/encoder/opennmt_encoders/ci_scorers.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11046 2023-04-17 03:36:48.000000 funasr-0.6.1/funasr/models/encoder/opennmt_encoders/conv_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13971 2023-02-11 09:30:01.000000 funasr-0.6.1/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21170 2023-04-17 03:36:48.000000 funasr-0.6.1/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    41076 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/models/encoder/resnet34_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3633 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/models/encoder/rnn_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    56364 2023-06-06 13:50:59.000000 funasr-0.6.1/funasr/models/encoder/sanm_encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26890 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/models/encoder/transformer_encoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.741085 funasr-0.6.1/funasr/models/frontend/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/models/frontend/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      399 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/models/frontend/abs_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9122 2023-05-22 05:06:44.000000 funasr-0.6.1/funasr/models/frontend/default.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.6.1/funasr/models/frontend/eend_ola_feature.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5758 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/models/frontend/fused.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4989 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/models/frontend/s3prl.py
--rw-r--r--   0 zhifu      (502) staff       (20)    20537 2023-06-06 13:50:59.000000 funasr-0.6.1/funasr/models/frontend/wav_frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2321 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/models/frontend/wav_frontend_kaldifeat.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2811 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/models/frontend/windowing.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.744335 funasr-0.6.1/funasr/models/joint_net/
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.6.1/funasr/models/joint_net/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.6.1/funasr/models/joint_net/joint_network.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.745113 funasr-0.6.1/funasr/models/pooling/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/models/pooling/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3550 2023-05-09 03:02:42.000000 funasr-0.6.1/funasr/models/pooling/statistic_pooling.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.774489 funasr-0.6.1/funasr/models/postencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/models/postencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/models/postencoder/abs_postencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3626 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/models/postencoder/hugging_face_transformers_postencoder.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.775157 funasr-0.6.1/funasr/models/predictor/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/models/predictor/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    35747 2023-05-22 05:06:44.000000 funasr-0.6.1/funasr/models/predictor/cif.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.776676 funasr-0.6.1/funasr/models/preencoder/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/models/preencoder/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/models/preencoder/abs_preencoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1042 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/models/preencoder/linear.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10296 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/models/preencoder/sinc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5906 2023-05-22 05:06:44.000000 funasr-0.6.1/funasr/models/seq_rnn_lm.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.777315 funasr-0.6.1/funasr/models/specaug/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/models/specaug/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      424 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/models/specaug/abs_specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/models/specaug/specaug.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4476 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/models/target_delay_transformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4246 2023-05-22 05:06:44.000000 funasr-0.6.1/funasr/models/transformer_lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4666 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/models/vad_realtime_transformer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.827462 funasr-0.6.1/funasr/modules/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/add_sos_eos.py
--rw-r--r--   0 zhifu      (502) staff       (20)    38235 2023-05-09 03:02:42.000000 funasr-0.6.1/funasr/modules/attention.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.829667 funasr-0.6.1/funasr/modules/beam_search/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/beam_search/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/beam_search/batch_beam_search.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/beam_search/batch_beam_search_online_sim.py
--rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/beam_search/beam_search.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)    20115 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/modules/beam_search/beam_search_sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.6.1/funasr/modules/beam_search/beam_search_transducer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.861100 funasr-0.6.1/funasr/modules/data2vec/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/data2vec/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5831 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/data2vec/data_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/data2vec/ema_module.py
--rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/data2vec/grad_multiply.py
--rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/data2vec/multihead_attention.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/data2vec/quant_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/data2vec/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/data2vec/wav2vec2.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/dynamic_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/dynamic_conv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.6.1/funasr/modules/e2e_asr_common.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.862034 funasr-0.6.1/funasr/modules/eend_ola/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.6.1/funasr/modules/eend_ola/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.6.1/funasr/modules/eend_ola/encoder.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.6.1/funasr/modules/eend_ola/encoder_decoder_attractor.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17767 2023-04-27 09:38:10.000000 funasr-0.6.1/funasr/modules/embedding.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.864262 funasr-0.6.1/funasr/modules/frontends/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/frontends/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/frontends/beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/frontends/dnn_beamformer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/frontends/dnn_wpe.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/frontends/feature_transform.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/frontends/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2648 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/frontends/mask_estimator.py
--rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/layer_norm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/lightconv.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/lightconv2d.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.6.1/funasr/modules/mask.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.6.1/funasr/modules/multi_layer_conv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    22963 2023-05-09 09:17:41.000000 funasr-0.6.1/funasr/modules/nets_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/positionwise_feed_forward.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3687 2023-05-09 09:17:41.000000 funasr-0.6.1/funasr/modules/repeat.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.867729 funasr-0.6.1/funasr/modules/rnn/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/rnn/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/rnn/argument.py
--rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/rnn/attentions.py
--rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/rnn/decoders.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/rnn/encoders.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.869225 funasr-0.6.1/funasr/modules/scorers/
--rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/scorers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/scorers/ctc.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/scorers/ctc_prefix_score.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/scorers/length_bonus.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/scorers/scorer_interface.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.871378 funasr-0.6.1/funasr/modules/streaming_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/streaming_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.6.1/funasr/modules/streaming_utils/chunk_utilis.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/streaming_utils/load_fr_tf.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/streaming_utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21445 2023-05-25 08:06:43.000000 funasr-0.6.1/funasr/modules/subsampling.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/modules/subsampling_without_posenc.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.872485 funasr-0.6.1/funasr/optimizers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/optimizers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.6.1/funasr/optimizers/fairseq_adam.py
--rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/optimizers/sgd.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.872751 funasr-0.6.1/funasr/runtime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.1/funasr/runtime/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.872909 funasr-0.6.1/funasr/runtime/python/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.1/funasr/runtime/python/__init__.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.873900 funasr-0.6.1/funasr/runtime/python/libtorch/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.6.1/funasr/runtime/python/libtorch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.6.1/funasr/runtime/python/libtorch/demo.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.876393 funasr-0.6.1/funasr/runtime/python/libtorch/funasr_torch/
--rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.6.1/funasr/runtime/python/libtorch/funasr_torch/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.6.1/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.879466 funasr-0.6.1/funasr/runtime/python/libtorch/funasr_torch/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.6.1/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.6.1/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7040 2023-04-12 07:23:40.000000 funasr-0.6.1/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.6.1/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.6.1/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4845 2023-04-17 03:36:48.000000 funasr-0.6.1/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1443 2023-04-17 03:36:48.000000 funasr-0.6.1/funasr/runtime/python/libtorch/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.881944 funasr-0.6.1/funasr/runtime/python/onnxruntime/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.1/funasr/runtime/python/onnxruntime/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      679 2023-05-12 03:37:01.000000 funasr-0.6.1/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      724 2023-05-12 03:39:34.000000 funasr-0.6.1/funasr/runtime/python/onnxruntime/demo_punc_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      916 2023-05-12 03:39:34.000000 funasr-0.6.1/funasr/runtime/python/onnxruntime/demo_punc_online.py
--rw-r--r--   0 zhifu      (502) staff       (20)      316 2023-05-12 03:39:34.000000 funasr-0.6.1/funasr/runtime/python/onnxruntime/demo_vad_offline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      930 2023-05-12 03:39:34.000000 funasr-0.6.1/funasr/runtime/python/onnxruntime/demo_vad_online.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.883976 funasr-0.6.1/funasr/runtime/python/onnxruntime/funasr_onnx/
--rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.6.1/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr-0.6.1/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13034 2023-05-22 05:06:44.000000 funasr-0.6.1/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.887275 funasr-0.6.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.6.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr-0.6.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
--rw-r--r--   0 zhifu      (502) staff       (20)    15848 2023-04-23 09:14:56.000000 funasr-0.6.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.6.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.6.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     9221 2023-05-12 02:56:06.000000 funasr-0.6.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-05-12 03:03:13.000000 funasr-0.6.1/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1580 2023-05-12 03:39:34.000000 funasr-0.6.1/funasr/runtime/python/onnxruntime/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.891439 funasr-0.6.1/funasr/samplers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/samplers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/samplers/abs_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6231 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/samplers/build_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5716 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/samplers/folded_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5168 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/samplers/length_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5680 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/samplers/num_elements_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3144 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/samplers/sorted_batch_sampler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2940 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/samplers/unsorted_batch_sampler.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.893759 funasr-0.6.1/funasr/schedulers/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/schedulers/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/schedulers/abs_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2067 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/schedulers/noam_lr.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3658 2023-02-09 08:39:15.000000 funasr-0.6.1/funasr/schedulers/tri_stage_scheduler.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1494 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/schedulers/warmup_lr.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.898279 funasr-0.6.1/funasr/tasks/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/tasks/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    73166 2023-05-24 02:58:26.000000 funasr-0.6.1/funasr/tasks/abs_task.py
--rw-r--r--   0 zhifu      (502) staff       (20)    53365 2023-05-24 02:58:26.000000 funasr-0.6.1/funasr/tasks/asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    12089 2023-02-09 08:39:15.000000 funasr-0.6.1/funasr/tasks/data2vec.py
--rw-r--r--   0 zhifu      (502) staff       (20)    32440 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/tasks/diar.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6755 2023-05-22 05:06:44.000000 funasr-0.6.1/funasr/tasks/lm.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7948 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/tasks/punctuation.py
--rw-r--r--   0 zhifu      (502) staff       (20)    21367 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/tasks/sa_asr.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18791 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/tasks/sv.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10644 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/tasks/vad.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.904063 funasr-0.6.1/funasr/text/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/text/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/text/abs_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2205 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/text/build_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2230 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/text/char_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1479 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/text/cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/text/korean_cleaner.py
--rw-r--r--   0 zhifu      (502) staff       (20)    16601 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/text/phoneme_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1294 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/text/sentencepiece_tokenizer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2100 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/text/token_id_converter.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2074 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/text/word_tokenizer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.906979 funasr-0.6.1/funasr/torch_utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/torch_utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/torch_utils/add_gradient_noise.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/torch_utils/device_funcs.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1052 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/torch_utils/forward_adaptor.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3788 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/torch_utils/initialize.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3817 2023-05-07 09:22:42.000000 funasr-0.6.1/funasr/torch_utils/load_pretrained_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/torch_utils/model_summary.py
--rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/torch_utils/pytorch_version.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/torch_utils/recursive_op.py
--rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/torch_utils/set_all_random_seed.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.910559 funasr-0.6.1/funasr/train/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/train/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11513 2023-05-22 05:06:44.000000 funasr-0.6.1/funasr/train/abs_model.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3017 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/train/class_choices.py
--rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.6.1/funasr/train/distributed_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    18344 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/train/reporter.py
--rw-r--r--   0 zhifu      (502) staff       (20)    38665 2023-06-06 13:50:59.000000 funasr-0.6.1/funasr/train/trainer.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.930511 funasr-0.6.1/funasr/utils/
--rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/utils/__init__.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/utils/asr_env_checking.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11612 2023-03-29 08:06:19.000000 funasr-0.6.1/funasr/utils/asr_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      582 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/utils/build_dataclass.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/utils/cli_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/utils/compute_eer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/utils/compute_min_dcf.py
--rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.6.1/funasr/utils/compute_wer.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/utils/config_argparse.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/utils/get_default_kwargs.py
--rw-r--r--   0 zhifu      (502) staff       (20)     5632 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/utils/griffin_lim.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.6.1/funasr/utils/job_runner.py
--rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-06-06 13:50:59.000000 funasr-0.6.1/funasr/utils/kwargs2args.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1607 2023-02-11 09:30:01.000000 funasr-0.6.1/funasr/utils/misc.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.6.1/funasr/utils/modelscope_param.py
--rw-r--r--   0 zhifu      (502) staff       (20)      571 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/utils/modelscope_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/utils/nested_dict_action.py
--rw-r--r--   0 zhifu      (502) staff       (20)     7734 2023-05-09 03:02:42.000000 funasr-0.6.1/funasr/utils/postprocess_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    10094 2023-06-06 13:50:59.000000 funasr-0.6.1/funasr/utils/prepare_data.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/utils/sized_dict.py
--rw-r--r--   0 zhifu      (502) staff       (20)    13380 2023-05-10 06:41:10.000000 funasr-0.6.1/funasr/utils/timestamp_tools.py
--rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/utils/types.py
--rw-r--r--   0 zhifu      (502) staff       (20)      638 2023-05-22 05:05:02.000000 funasr-0.6.1/funasr/utils/vad_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)    11760 2023-04-25 03:22:30.000000 funasr-0.6.1/funasr/utils/wav_utils.py
--rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.6.1/funasr/utils/yaml_no_alias_safe_dump.py
--rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-06-13 03:13:55.000000 funasr-0.6.1/funasr/version.txt
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:16.319008 funasr-0.6.1/funasr.egg-info/
--rw-r--r--   0 zhifu      (502) staff       (20)     8368 2023-06-13 03:14:16.000000 funasr-0.6.1/funasr.egg-info/PKG-INFO
--rw-r--r--   0 zhifu      (502) staff       (20)    13363 2023-06-13 03:14:16.000000 funasr-0.6.1/funasr.egg-info/SOURCES.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-06-13 03:14:16.000000 funasr-0.6.1/funasr.egg-info/dependency_links.txt
--rw-r--r--   0 zhifu      (502) staff       (20)      857 2023-06-13 03:14:16.000000 funasr-0.6.1/funasr.egg-info/requires.txt
--rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-06-13 03:14:16.000000 funasr-0.6.1/funasr.egg-info/top_level.txt
--rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-06-13 03:14:17.938097 funasr-0.6.1/setup.cfg
--rw-r--r--   0 zhifu      (502) staff       (20)     4626 2023-06-06 13:50:59.000000 funasr-0.6.1/setup.py
-drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-13 03:14:17.935120 funasr-0.6.1/tests/
--rw-r--r--   0 zhifu      (502) staff       (20)    26162 2023-05-08 08:26:24.000000 funasr-0.6.1/tests/test_asr_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1210 2023-03-29 08:06:19.000000 funasr-0.6.1/tests/test_asr_vad_punc_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.6.1/tests/test_lm_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.6.1/tests/test_punctuation_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     1949 2023-04-12 07:23:40.000000 funasr-0.6.1/tests/test_sv_inference_pipeline.py
--rw-r--r--   0 zhifu      (502) staff       (20)     2298 2023-04-25 05:58:46.000000 funasr-0.6.1/tests/test_vad_inference_pipeline.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.239728 funasr-0.6.2/
+-rw-r--r--   0 zhifu      (502) staff       (20)     8149 2023-06-19 11:14:29.239490 funasr-0.6.2/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)     7149 2023-06-19 09:03:43.000000 funasr-0.6.2/README.md
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.562972 funasr-0.6.2/funasr/
+-rw-r--r--   0 zhifu      (502) staff       (20)      203 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.634647 funasr-0.6.2/funasr/bin/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/bin/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     3798 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/bin/aggregate_stats_dirs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    69792 2023-06-19 09:03:43.000000 funasr-0.6.2/funasr/bin/asr_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    73057 2023-06-19 11:11:09.000000 funasr-0.6.2/funasr/bin/asr_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1715 2023-05-24 02:58:26.000000 funasr-0.6.2/funasr/bin/asr_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5416 2023-06-06 13:50:59.000000 funasr-0.6.2/funasr/bin/build_trainer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1012 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/bin/data2vec_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    12198 2023-05-25 08:06:43.000000 funasr-0.6.2/funasr/bin/diar_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    18753 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/bin/diar_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1180 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/bin/diar_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15054 2023-05-23 08:26:46.000000 funasr-0.6.2/funasr/bin/lm_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1189 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/bin/lm_train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12512 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/bin/punc_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     8675 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/bin/punc_inference_launch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      999 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/bin/punc_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     1241 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/bin/sa_asr_train.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5299 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/bin/sv_infer.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    10573 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/bin/sv_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     8449 2023-02-11 09:29:33.000000 funasr-0.6.2/funasr/bin/tokenize_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3999 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/bin/tp_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10220 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/bin/tp_inference_launch.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    17705 2023-06-19 09:03:43.000000 funasr-0.6.2/funasr/bin/train.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7276 2023-06-06 13:50:59.000000 funasr-0.6.2/funasr/bin/vad_infer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13448 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/bin/vad_inference_launch.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.729439 funasr-0.6.2/funasr/build_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-05-18 12:04:14.000000 funasr-0.6.2/funasr/build_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3425 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/build_utils/build_args.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16062 2023-06-19 09:03:43.000000 funasr-0.6.2/funasr/build_utils/build_asr_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      672 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/build_utils/build_dataloader.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9592 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/build_utils/build_diar_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1552 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/build_utils/build_distributed.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1418 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/build_utils/build_lm_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      968 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/build_utils/build_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      810 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/build_utils/build_optimizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2993 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/build_utils/build_pretrain_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2211 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/build_utils/build_punc_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1531 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/build_utils/build_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    35626 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/build_utils/build_trainer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2196 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/build_utils/build_vad_model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.774909 funasr-0.6.2/funasr/datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4338 2023-02-09 08:39:15.000000 funasr-0.6.2/funasr/datasets/collate_fn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15174 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/datasets/dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15562 2023-03-29 08:06:18.000000 funasr-0.6.2/funasr/datasets/iterable_dataset.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.776569 funasr-0.6.2/funasr/datasets/large_datasets/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/datasets/large_datasets/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3794 2023-06-06 13:50:59.000000 funasr-0.6.2/funasr/datasets/large_datasets/build_dataloader.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.803885 funasr-0.6.2/funasr/datasets/large_datasets/datapipes/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/datasets/large_datasets/datapipes/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8298 2023-02-09 08:39:15.000000 funasr-0.6.2/funasr/datasets/large_datasets/datapipes/batch.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      519 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/datasets/large_datasets/datapipes/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      453 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/datasets/large_datasets/datapipes/map.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10367 2023-06-06 13:50:59.000000 funasr-0.6.2/funasr/datasets/large_datasets/dataset.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.813982 funasr-0.6.2/funasr/datasets/large_datasets/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/datasets/large_datasets/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1382 2023-02-09 08:39:15.000000 funasr-0.6.2/funasr/datasets/large_datasets/utils/clipping.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1013 2023-02-09 08:39:15.000000 funasr-0.6.2/funasr/datasets/large_datasets/utils/filter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1566 2023-05-07 09:22:42.000000 funasr-0.6.2/funasr/datasets/large_datasets/utils/hotword_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      948 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/datasets/large_datasets/utils/low_frame_rate.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3303 2023-05-07 09:22:42.000000 funasr-0.6.2/funasr/datasets/large_datasets/utils/padding.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2582 2023-05-25 08:06:43.000000 funasr-0.6.2/funasr/datasets/large_datasets/utils/tokenize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1281 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/datasets/ms_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31032 2023-04-27 08:40:56.000000 funasr-0.6.2/funasr/datasets/preprocessor.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.814843 funasr-0.6.2/funasr/export/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.2/funasr/export/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10699 2023-05-12 02:41:22.000000 funasr-0.6.2/funasr/export/export_model.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.817185 funasr-0.6.2/funasr/export/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)     5127 2023-05-07 09:22:42.000000 funasr-0.6.2/funasr/export/models/CT_Transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1540 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/export/models/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.818917 funasr-0.6.2/funasr/export/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.2/funasr/export/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6326 2023-04-14 02:11:18.000000 funasr-0.6.2/funasr/export/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5470 2023-03-10 07:21:13.000000 funasr-0.6.2/funasr/export/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8441 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/export/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2047 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/export/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.843602 funasr-0.6.2/funasr/export/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.2/funasr/export/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3881 2023-03-29 08:06:18.000000 funasr-0.6.2/funasr/export/models/encoder/conformer_encoder.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9141 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/export/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7524 2023-05-05 07:04:25.000000 funasr-0.6.2/funasr/export/models/encoder/sanm_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.860967 funasr-0.6.2/funasr/export/models/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.2/funasr/export/models/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1931 2023-03-29 08:06:18.000000 funasr-0.6.2/funasr/export/models/modules/decoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2354 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/export/models/modules/encoder_layer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      658 2023-02-08 11:34:59.000000 funasr-0.6.2/funasr/export/models/modules/feedforward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8644 2023-04-14 02:11:18.000000 funasr-0.6.2/funasr/export/models/modules/multihead_att.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.862253 funasr-0.6.2/funasr/export/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.2/funasr/export/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9917 2023-04-14 02:11:18.000000 funasr-0.6.2/funasr/export/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.890828 funasr-0.6.2/funasr/export/test/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/export/test/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      785 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/export/test/test_onnx.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      702 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/export/test/test_onnx_punc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      927 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/export/test/test_onnx_punc_vadrealtime.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1046 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/export/test/test_onnx_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      477 2023-05-24 08:36:46.000000 funasr-0.6.2/funasr/export/test/test_torchscripts.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.892775 funasr-0.6.2/funasr/export/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-08 11:34:59.000000 funasr-0.6.2/funasr/export/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2620 2023-02-08 11:34:59.000000 funasr-0.6.2/funasr/export/utils/torch_function.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.895767 funasr-0.6.2/funasr/fileio/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/fileio/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2383 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/fileio/datadir_writer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2357 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/fileio/npy_scp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2361 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/fileio/rand_gen_dataset.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2273 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/fileio/read_text.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4050 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/fileio/sound_scp.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.914662 funasr-0.6.2/funasr/iterators/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/iterators/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      234 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/iterators/abs_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7808 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/iterators/chunk_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1140 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/iterators/multiple_iter_factory.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5236 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/iterators/sequence_iter_factory.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.918457 funasr-0.6.2/funasr/layers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/layers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      358 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/layers/abs_normalize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6717 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/layers/complex_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3499 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/layers/global_mvn.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      348 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/layers/inversible_interface.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2539 2023-03-10 07:21:13.000000 funasr-0.6.2/funasr/layers/label_aggregation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2564 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/layers/log_mel.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10488 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/layers/mask_along_axis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9033 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/layers/sinc_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8436 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/layers/stft.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2513 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/layers/time_warp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2309 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/layers/utterance_mvn.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.918801 funasr-0.6.2/funasr/losses/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/losses/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4320 2023-05-09 03:02:42.000000 funasr-0.6.2/funasr/losses/label_smoothing_loss.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.921191 funasr-0.6.2/funasr/main_funcs/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/main_funcs/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4687 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/main_funcs/average_nbest_models.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5599 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/main_funcs/calculate_all_attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5018 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/main_funcs/collect_stats.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9906 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/main_funcs/pack_funcs.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.960179 funasr-0.6.2/funasr/models/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      319 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/base_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6541 2023-02-11 09:29:22.000000 funasr-0.6.2/funasr/models/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5285 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/data2vec.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.963818 funasr-0.6.2/funasr/models/decoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/decoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      473 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/decoder/abs_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    40834 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/models/decoder/contextual_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12133 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/decoder/rnn_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8355 2023-05-09 09:17:41.000000 funasr-0.6.2/funasr/models/decoder/rnnt_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    75478 2023-06-06 13:50:59.000000 funasr-0.6.2/funasr/models/decoder/sanm_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1389 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/decoder/sv_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    43192 2023-05-09 03:02:42.000000 funasr-0.6.2/funasr/models/decoder/transformer_decoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16699 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/e2e_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8572 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/e2e_asr_common.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15709 2023-05-07 09:22:42.000000 funasr-0.6.2/funasr/models/e2e_asr_contextual_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11838 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/e2e_asr_mfcca.py
+-rw-r--r--   0 zhifu      (502) staff       (20)   100491 2023-06-06 13:50:59.000000 funasr-0.6.2/funasr/models/e2e_asr_paraformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    35111 2023-06-06 13:50:59.000000 funasr-0.6.2/funasr/models/e2e_asr_transducer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10226 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/e2e_diar_eend_ola.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20567 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/e2e_diar_sond.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18965 2023-06-19 09:03:43.000000 funasr-0.6.2/funasr/models/e2e_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10084 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/e2e_sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6682 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/e2e_tp.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    51719 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/e2e_uni_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    31858 2023-06-13 03:13:40.000000 funasr-0.6.2/funasr/models/e2e_vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.970556 funasr-0.6.2/funasr/models/encoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/encoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      502 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/encoder/abs_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    43621 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/models/encoder/conformer_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20992 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/encoder/data2vec_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    19855 2023-03-10 07:21:13.000000 funasr-0.6.2/funasr/models/encoder/ecapa_tdnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10164 2023-02-16 09:30:51.000000 funasr-0.6.2/funasr/models/encoder/encoder_layer_mfcca.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     9281 2023-03-10 07:21:13.000000 funasr-0.6.2/funasr/models/encoder/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17681 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/encoder/mfcca_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.973388 funasr-0.6.2/funasr/models/encoder/opennmt_encoders/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-11 09:30:01.000000 funasr-0.6.2/funasr/models/encoder/opennmt_encoders/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      909 2023-02-11 09:30:01.000000 funasr-0.6.2/funasr/models/encoder/opennmt_encoders/ci_scorers.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11046 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/models/encoder/opennmt_encoders/conv_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13971 2023-02-11 09:30:01.000000 funasr-0.6.2/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21170 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    41076 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/encoder/resnet34_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3633 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/encoder/rnn_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    56364 2023-06-06 13:50:59.000000 funasr-0.6.2/funasr/models/encoder/sanm_encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26890 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/encoder/transformer_encoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.979316 funasr-0.6.2/funasr/models/frontend/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/frontend/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      399 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/frontend/abs_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11467 2023-06-19 09:03:43.000000 funasr-0.6.2/funasr/models/frontend/default.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1405 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/models/frontend/eend_ola_feature.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5758 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/frontend/fused.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4989 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/frontend/s3prl.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    20537 2023-06-06 13:50:59.000000 funasr-0.6.2/funasr/models/frontend/wav_frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2321 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/frontend/wav_frontend_kaldifeat.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2811 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/frontend/windowing.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.980319 funasr-0.6.2/funasr/models/joint_net/
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-04-25 03:22:30.000000 funasr-0.6.2/funasr/models/joint_net/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1855 2023-04-25 03:22:30.000000 funasr-0.6.2/funasr/models/joint_net/joint_network.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.981100 funasr-0.6.2/funasr/models/pooling/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/pooling/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3550 2023-05-09 03:02:42.000000 funasr-0.6.2/funasr/models/pooling/statistic_pooling.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.986016 funasr-0.6.2/funasr/models/postencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/postencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      403 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/postencoder/abs_postencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3626 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/postencoder/hugging_face_transformers_postencoder.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.987214 funasr-0.6.2/funasr/models/predictor/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/predictor/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    35747 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/models/predictor/cif.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.988886 funasr-0.6.2/funasr/models/preencoder/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/preencoder/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      402 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/preencoder/abs_preencoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1042 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/preencoder/linear.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10296 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/preencoder/sinc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5906 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/models/seq_rnn_lm.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.989583 funasr-0.6.2/funasr/models/specaug/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/specaug/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      424 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/specaug/abs_specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6607 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/models/specaug/specaug.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4476 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/target_delay_transformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4246 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/models/transformer_lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4666 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/models/vad_realtime_transformer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.000054 funasr-0.6.2/funasr/modules/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      940 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/add_sos_eos.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    38235 2023-05-09 03:02:42.000000 funasr-0.6.2/funasr/modules/attention.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.034597 funasr-0.6.2/funasr/modules/beam_search/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/beam_search/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13305 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/beam_search/batch_beam_search.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10175 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/beam_search/batch_beam_search_online_sim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    53592 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/beam_search/beam_search.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)    20115 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/modules/beam_search/beam_search_sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    23002 2023-04-25 03:22:30.000000 funasr-0.6.2/funasr/modules/beam_search/beam_search_transducer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.036570 funasr-0.6.2/funasr/modules/data2vec/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/data2vec/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5831 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/data2vec/data_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4474 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/data2vec/ema_module.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      442 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/data2vec/grad_multiply.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    26458 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/data2vec/multihead_attention.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4021 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/data2vec/quant_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4858 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/data2vec/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12734 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/data2vec/wav2vec2.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4244 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/dynamic_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4863 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/dynamic_conv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13662 2023-04-27 08:40:56.000000 funasr-0.6.2/funasr/modules/e2e_asr_common.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.069542 funasr-0.6.2/funasr/modules/eend_ola/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:18.000000 funasr-0.6.2/funasr/modules/eend_ola/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5287 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/modules/eend_ola/encoder.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2768 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/modules/eend_ola/encoder_decoder_attractor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17767 2023-04-27 09:38:10.000000 funasr-0.6.2/funasr/modules/embedding.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.076223 funasr-0.6.2/funasr/modules/frontends/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/frontends/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2731 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/frontends/beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5540 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/frontends/dnn_beamformer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2825 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/frontends/dnn_wpe.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7958 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/frontends/feature_transform.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4585 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/frontends/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2648 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/frontends/mask_estimator.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      958 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/layer_norm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3590 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/lightconv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4230 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/lightconv2d.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1654 2023-03-28 05:50:14.000000 funasr-0.6.2/funasr/modules/mask.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4800 2023-02-11 09:30:01.000000 funasr-0.6.2/funasr/modules/multi_layer_conv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    22963 2023-05-09 09:17:41.000000 funasr-0.6.2/funasr/modules/nets_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1936 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/positionwise_feed_forward.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3687 2023-05-09 09:17:41.000000 funasr-0.6.2/funasr/modules/repeat.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.079243 funasr-0.6.2/funasr/modules/rnn/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/rnn/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4080 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/rnn/argument.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    66987 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/rnn/attentions.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    49387 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/rnn/decoders.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14180 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/rnn/encoders.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.081119 funasr-0.6.2/funasr/modules/scorers/
+-rw-r--r--   0 zhifu      (502) staff       (20)       30 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/scorers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5026 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/scorers/ctc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13951 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/scorers/ctc_prefix_score.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1787 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/scorers/length_bonus.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5938 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/scorers/scorer_interface.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.082875 funasr-0.6.2/funasr/modules/streaming_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/streaming_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    17409 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/modules/streaming_utils/chunk_utilis.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1809 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/streaming_utils/load_fr_tf.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2399 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/streaming_utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21445 2023-05-25 08:06:43.000000 funasr-0.6.2/funasr/modules/subsampling.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1898 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/modules/subsampling_without_posenc.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.084210 funasr-0.6.2/funasr/optimizers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/optimizers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5643 2023-02-09 08:39:15.000000 funasr-0.6.2/funasr/optimizers/fairseq_adam.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      828 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/optimizers/sgd.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.084564 funasr-0.6.2/funasr/runtime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.2/funasr/runtime/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.084891 funasr-0.6.2/funasr/runtime/python/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.2/funasr/runtime/python/__init__.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.086040 funasr-0.6.2/funasr/runtime/python/libtorch/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-03-29 08:06:19.000000 funasr-0.6.2/funasr/runtime/python/libtorch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      544 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/runtime/python/libtorch/demo.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.087466 funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/
+-rw-r--r--   0 zhifu      (502) staff       (20)       65 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8172 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.090309 funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/utils/__init__.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5123 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7040 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7566 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2762 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4845 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1443 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/runtime/python/libtorch/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.093303 funasr-0.6.2/funasr/runtime/python/onnxruntime/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-16 09:30:51.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      679 2023-05-12 03:37:01.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      724 2023-05-12 03:39:34.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/demo_punc_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      916 2023-05-12 03:39:34.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/demo_punc_online.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      316 2023-05-12 03:39:34.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/demo_vad_offline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      930 2023-05-12 03:39:34.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/demo_vad_online.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.096006 funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/
+-rw-r--r--   0 zhifu      (502) staff       (20)      218 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     8855 2023-05-12 03:03:13.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13034 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.098650 funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-04-12 07:23:40.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    29216 2023-05-07 09:22:42.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    15848 2023-04-23 09:14:56.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7686 2023-04-25 07:21:40.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2933 2023-04-25 07:21:40.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     9221 2023-05-12 02:56:06.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10950 2023-05-12 03:03:13.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1580 2023-05-12 03:39:34.000000 funasr-0.6.2/funasr/runtime/python/onnxruntime/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.101498 funasr-0.6.2/funasr/samplers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/samplers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      425 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/samplers/abs_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6231 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/samplers/build_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5716 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/samplers/folded_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5168 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/samplers/length_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5680 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/samplers/num_elements_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3144 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/samplers/sorted_batch_sampler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2940 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/samplers/unsorted_batch_sampler.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.103063 funasr-0.6.2/funasr/schedulers/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/schedulers/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1679 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/schedulers/abs_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2067 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/schedulers/noam_lr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3658 2023-02-09 08:39:15.000000 funasr-0.6.2/funasr/schedulers/tri_stage_scheduler.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1494 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/schedulers/warmup_lr.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.108033 funasr-0.6.2/funasr/tasks/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/tasks/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    73166 2023-05-24 02:58:26.000000 funasr-0.6.2/funasr/tasks/abs_task.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    58550 2023-06-19 09:03:43.000000 funasr-0.6.2/funasr/tasks/asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    12089 2023-02-09 08:39:15.000000 funasr-0.6.2/funasr/tasks/data2vec.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    32440 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/tasks/diar.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6755 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/tasks/lm.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7948 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/tasks/punctuation.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    21358 2023-06-19 09:03:43.000000 funasr-0.6.2/funasr/tasks/sa_asr.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18791 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/tasks/sv.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10644 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/tasks/vad.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.111063 funasr-0.6.2/funasr/text/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/text/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      347 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/text/abs_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2205 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/text/build_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2230 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/text/char_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1479 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/text/cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1968 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/text/korean_cleaner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    16601 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/text/phoneme_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1294 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/text/sentencepiece_tokenizer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2100 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/text/token_id_converter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2074 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/text/word_tokenizer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.125732 funasr-0.6.2/funasr/torch_utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/torch_utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      987 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/torch_utils/add_gradient_noise.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2681 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/torch_utils/device_funcs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1052 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/torch_utils/forward_adaptor.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3788 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/torch_utils/initialize.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3817 2023-05-07 09:22:42.000000 funasr-0.6.2/funasr/torch_utils/load_pretrained_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2498 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/torch_utils/model_summary.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      468 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/torch_utils/pytorch_version.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1615 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/torch_utils/recursive_op.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      167 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/torch_utils/set_all_random_seed.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.129411 funasr-0.6.2/funasr/train/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/train/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11513 2023-05-22 05:06:44.000000 funasr-0.6.2/funasr/train/abs_model.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3017 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/train/class_choices.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    14493 2023-03-29 08:06:19.000000 funasr-0.6.2/funasr/train/distributed_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    18344 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/train/reporter.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    38665 2023-06-06 13:50:59.000000 funasr-0.6.2/funasr/train/trainer.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.236653 funasr-0.6.2/funasr/utils/
+-rw-r--r--   0 zhifu      (502) staff       (20)        0 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/__init__.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2664 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/asr_env_checking.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11612 2023-03-29 08:06:19.000000 funasr-0.6.2/funasr/utils/asr_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      582 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/build_dataclass.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1380 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/cli_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2078 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/compute_eer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     6714 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/compute_min_dcf.py
+-rwxr-xr-x   0 zhifu      (502) staff       (20)     5189 2023-04-17 03:36:48.000000 funasr-0.6.2/funasr/utils/compute_wer.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1760 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/config_argparse.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1830 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/get_default_kwargs.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     5632 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/griffin_lim.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4001 2023-02-11 09:30:01.000000 funasr-0.6.2/funasr/utils/job_runner.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      426 2023-06-06 13:50:59.000000 funasr-0.6.2/funasr/utils/kwargs2args.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1607 2023-02-11 09:30:01.000000 funasr-0.6.2/funasr/utils/misc.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1357 2023-02-09 08:39:15.000000 funasr-0.6.2/funasr/utils/modelscope_param.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      571 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/utils/modelscope_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     3598 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/nested_dict_action.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     7734 2023-05-09 03:02:42.000000 funasr-0.6.2/funasr/utils/postprocess_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    10094 2023-06-06 13:50:59.000000 funasr-0.6.2/funasr/utils/prepare_data.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2027 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/sized_dict.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    13380 2023-05-10 06:41:10.000000 funasr-0.6.2/funasr/utils/timestamp_tools.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     4185 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/types.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      638 2023-05-22 05:05:02.000000 funasr-0.6.2/funasr/utils/vad_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)    11760 2023-04-25 03:22:30.000000 funasr-0.6.2/funasr/utils/wav_utils.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      380 2023-02-07 07:13:39.000000 funasr-0.6.2/funasr/utils/yaml_no_alias_safe_dump.py
+-rw-r--r--   0 zhifu      (502) staff       (20)        6 2023-06-19 11:13:21.000000 funasr-0.6.2/funasr/version.txt
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:28.578277 funasr-0.6.2/funasr.egg-info/
+-rw-r--r--   0 zhifu      (502) staff       (20)     8149 2023-06-19 11:14:28.000000 funasr-0.6.2/funasr.egg-info/PKG-INFO
+-rw-r--r--   0 zhifu      (502) staff       (20)    13363 2023-06-19 11:14:28.000000 funasr-0.6.2/funasr.egg-info/SOURCES.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        1 2023-06-19 11:14:28.000000 funasr-0.6.2/funasr.egg-info/dependency_links.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)      857 2023-06-19 11:14:28.000000 funasr-0.6.2/funasr.egg-info/requires.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)        7 2023-06-19 11:14:28.000000 funasr-0.6.2/funasr.egg-info/top_level.txt
+-rw-r--r--   0 zhifu      (502) staff       (20)       38 2023-06-19 11:14:29.239788 funasr-0.6.2/setup.cfg
+-rw-r--r--   0 zhifu      (502) staff       (20)     4626 2023-06-06 13:50:59.000000 funasr-0.6.2/setup.py
+drwxr-xr-x   0 zhifu      (502) staff       (20)        0 2023-06-19 11:14:29.238808 funasr-0.6.2/tests/
+-rw-r--r--   0 zhifu      (502) staff       (20)    26773 2023-06-15 09:10:12.000000 funasr-0.6.2/tests/test_asr_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1310 2023-06-15 09:10:12.000000 funasr-0.6.2/tests/test_asr_vad_punc_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)      804 2023-03-29 08:06:19.000000 funasr-0.6.2/tests/test_lm_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2055 2023-04-17 03:36:48.000000 funasr-0.6.2/tests/test_punctuation_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     1584 2023-06-19 09:03:43.000000 funasr-0.6.2/tests/test_sv_inference_pipeline.py
+-rw-r--r--   0 zhifu      (502) staff       (20)     2298 2023-04-25 05:58:46.000000 funasr-0.6.2/tests/test_vad_inference_pipeline.py
```

### Comparing `funasr-0.6.1/PKG-INFO` & `funasr-0.6.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.6.1
+Version: 0.6.2
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -94,25 +94,24 @@
 
 |Dingding group |                     Wechat group                      |
 |:---:|:-----------------------------------------------------:|
 |<div align="left"><img src="docs/images/dingding.jpg" width="250"/> | <img src="docs/images/wechat.png" width="232"/></div> |
 
 ## Contributors
 
-| <div align="left"><img src="docs/images/damo.png" width="180"/> | <div align="left"><img src="docs/images/nwpu.png" width="260"/> | <img src="docs/images/China_Telecom.png" width="200"/> </div>  | <img src="docs/images/RapidAI.png" width="200"/> </div> | <img src="docs/images/DeepScience.png" width="200"/> </div> | <img src="docs/images/aihealthx.png" width="200"/> </div> |
-|:---------------------------------------------------------------:|:---------------------------------------------------------------:|:--------------------------------------------------------------:|:-------------------------------------------------------:|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
+| <div align="left"><img src="docs/images/damo.png" width="180"/> | <div align="left"><img src="docs/images/nwpu.png" width="260"/> | <img src="docs/images/China_Telecom.png" width="200"/> </div>  | <img src="docs/images/RapidAI.png" width="200"/> </div> | <img src="docs/images/aihealthx.png" width="200"/> </div> |
+|:---------------------------------------------------------------:|:---------------------------------------------------------------:|:--------------------------------------------------------------:|:-------------------------------------------------------:|:-----------------------------------------------------------:|
 
 ## Acknowledge
 
 1. We borrowed a lot of code from [Kaldi](http://kaldi-asr.org/) for data preparation.
 2. We borrowed a lot of code from [ESPnet](https://github.com/espnet/espnet). FunASR follows up the training and finetuning pipelines of ESPnet.
 3. We referred [Wenet](https://github.com/wenet-e2e/wenet) for building dataloader for large scale data training.
 4. We acknowledge [ChinaTelecom](https://github.com/zhuzizyf/damo-fsmn-vad-infer-httpserver) for contributing the VAD runtime. 
 5. We acknowledge [RapidAI](https://github.com/RapidAI) for contributing the Paraformer and CT_Transformer-punc runtime.
-6. We acknowledge [DeepScience](https://www.deepscience.cn) for contributing the grpc service.
 6. We acknowledge [AiHealthx](http://www.aihealthx.com/) for contributing the websocket service and html5.
 
 ## License
 This project is licensed under the [The MIT License](https://opensource.org/licenses/MIT). FunASR also contains various third-party components and some code modified from other repos under other open source licenses.
 The use of pretraining model is subject to [model licencs](./MODEL_LICENSE)
 
 ## Citations
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.6.1 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.6.2 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
@@ -73,38 +73,36 @@
 inc.com) |Dingding group | Wechat group | |:---:|:-----------------------------
 ------------------------:| |
 [docs/images/dingding.jpg] | [docs/images/wechat.png]
 | ## Contributors |
 [docs/images/damo.png] |
 [docs/images/nwpu.png] | [docs/images/China_Telecom.png]
 | [docs/images/RapidAI.png]
-| [docs/images/DeepScience.png]
 | [docs/images/aihealthx.png]
 | |:---------------------------------------------------------------:|:---------
 ------------------------------------------------------:|:----------------------
 ----------------------------------------:|:------------------------------------
 -------------------:|:---------------------------------------------------------
---:|:-----------------------------------------------------------:| ##
-Acknowledge 1. We borrowed a lot of code from [Kaldi](http://kaldi-asr.org/
-) for data preparation. 2. We borrowed a lot of code from [ESPnet](https://
-github.com/espnet/espnet). FunASR follows up the training and finetuning
-pipelines of ESPnet. 3. We referred [Wenet](https://github.com/wenet-e2e/wenet)
-for building dataloader for large scale data training. 4. We acknowledge
-[ChinaTelecom](https://github.com/zhuzizyf/damo-fsmn-vad-infer-httpserver) for
-contributing the VAD runtime. 5. We acknowledge [RapidAI](https://github.com/
-RapidAI) for contributing the Paraformer and CT_Transformer-punc runtime. 6. We
-acknowledge [DeepScience](https://www.deepscience.cn) for contributing the grpc
-service. 6. We acknowledge [AiHealthx](http://www.aihealthx.com/) for
-contributing the websocket service and html5. ## License This project is
-licensed under the [The MIT License](https://opensource.org/licenses/MIT).
-FunASR also contains various third-party components and some code modified from
-other repos under other open source licenses. The use of pretraining model is
-subject to [model licencs](./MODEL_LICENSE) ## Citations ``` bibtex
-@inproceedings{gao2023funasr, author={Zhifu Gao and Zerui Li and Jiaming Wang
-and Haoneng Luo and Xian Shi and Mengzhe Chen and Yabin Li and Lingyun Zuo and
-Zhihao Du and Zhangyu Xiao and Shiliang Zhang}, title={FunASR: A Fundamental
-End-to-End Speech Recognition Toolkit}, year={2023}, booktitle={INTERSPEECH}, }
-@inproceedings{gao22b_interspeech, author={Zhifu Gao and ShiLiang Zhang and Ian
-McLoughlin and Zhijie Yan}, title={{Paraformer: Fast and Accurate Parallel
-Transformer for Non-autoregressive End-to-End Speech Recognition}}, year=2022,
-booktitle={Proc. Interspeech 2022}, pages={2063--2067}, doi={10.21437/
-Interspeech.2022-9996} } ```
+--:| ## Acknowledge 1. We borrowed a lot of code from [Kaldi](http://kaldi-
+asr.org/) for data preparation. 2. We borrowed a lot of code from [ESPnet]
+(https://github.com/espnet/espnet). FunASR follows up the training and
+finetuning pipelines of ESPnet. 3. We referred [Wenet](https://github.com/
+wenet-e2e/wenet) for building dataloader for large scale data training. 4. We
+acknowledge [ChinaTelecom](https://github.com/zhuzizyf/damo-fsmn-vad-infer-
+httpserver) for contributing the VAD runtime. 5. We acknowledge [RapidAI]
+(https://github.com/RapidAI) for contributing the Paraformer and
+CT_Transformer-punc runtime. 6. We acknowledge [AiHealthx](http://
+www.aihealthx.com/) for contributing the websocket service and html5. ##
+License This project is licensed under the [The MIT License](https://
+opensource.org/licenses/MIT). FunASR also contains various third-party
+components and some code modified from other repos under other open source
+licenses. The use of pretraining model is subject to [model licencs](./
+MODEL_LICENSE) ## Citations ``` bibtex @inproceedings{gao2023funasr, author=
+{Zhifu Gao and Zerui Li and Jiaming Wang and Haoneng Luo and Xian Shi and
+Mengzhe Chen and Yabin Li and Lingyun Zuo and Zhihao Du and Zhangyu Xiao and
+Shiliang Zhang}, title={FunASR: A Fundamental End-to-End Speech Recognition
+Toolkit}, year={2023}, booktitle={INTERSPEECH}, } @inproceedings
+{gao22b_interspeech, author={Zhifu Gao and ShiLiang Zhang and Ian McLoughlin
+and Zhijie Yan}, title={{Paraformer: Fast and Accurate Parallel Transformer for
+Non-autoregressive End-to-End Speech Recognition}}, year=2022, booktitle={Proc.
+Interspeech 2022}, pages={2063--2067}, doi={10.21437/Interspeech.2022-9996} }
+```
```

### Comparing `funasr-0.6.1/README.md` & `funasr-0.6.2/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -68,25 +68,24 @@
 
 |Dingding group |                     Wechat group                      |
 |:---:|:-----------------------------------------------------:|
 |<div align="left"><img src="docs/images/dingding.jpg" width="250"/> | <img src="docs/images/wechat.png" width="232"/></div> |
 
 ## Contributors
 
-| <div align="left"><img src="docs/images/damo.png" width="180"/> | <div align="left"><img src="docs/images/nwpu.png" width="260"/> | <img src="docs/images/China_Telecom.png" width="200"/> </div>  | <img src="docs/images/RapidAI.png" width="200"/> </div> | <img src="docs/images/DeepScience.png" width="200"/> </div> | <img src="docs/images/aihealthx.png" width="200"/> </div> |
-|:---------------------------------------------------------------:|:---------------------------------------------------------------:|:--------------------------------------------------------------:|:-------------------------------------------------------:|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
+| <div align="left"><img src="docs/images/damo.png" width="180"/> | <div align="left"><img src="docs/images/nwpu.png" width="260"/> | <img src="docs/images/China_Telecom.png" width="200"/> </div>  | <img src="docs/images/RapidAI.png" width="200"/> </div> | <img src="docs/images/aihealthx.png" width="200"/> </div> |
+|:---------------------------------------------------------------:|:---------------------------------------------------------------:|:--------------------------------------------------------------:|:-------------------------------------------------------:|:-----------------------------------------------------------:|
 
 ## Acknowledge
 
 1. We borrowed a lot of code from [Kaldi](http://kaldi-asr.org/) for data preparation.
 2. We borrowed a lot of code from [ESPnet](https://github.com/espnet/espnet). FunASR follows up the training and finetuning pipelines of ESPnet.
 3. We referred [Wenet](https://github.com/wenet-e2e/wenet) for building dataloader for large scale data training.
 4. We acknowledge [ChinaTelecom](https://github.com/zhuzizyf/damo-fsmn-vad-infer-httpserver) for contributing the VAD runtime. 
 5. We acknowledge [RapidAI](https://github.com/RapidAI) for contributing the Paraformer and CT_Transformer-punc runtime.
-6. We acknowledge [DeepScience](https://www.deepscience.cn) for contributing the grpc service.
 6. We acknowledge [AiHealthx](http://www.aihealthx.com/) for contributing the websocket service and html5.
 
 ## License
 This project is licensed under the [The MIT License](https://opensource.org/licenses/MIT). FunASR also contains various third-party components and some code modified from other repos under other open source licenses.
 The use of pretraining model is subject to [model licencs](./MODEL_LICENSE)
 
 ## Citations
```

#### html2text {}

```diff
@@ -60,38 +60,36 @@
 inc.com) |Dingding group | Wechat group | |:---:|:-----------------------------
 ------------------------:| |
 [docs/images/dingding.jpg] | [docs/images/wechat.png]
 | ## Contributors |
 [docs/images/damo.png] |
 [docs/images/nwpu.png] | [docs/images/China_Telecom.png]
 | [docs/images/RapidAI.png]
-| [docs/images/DeepScience.png]
 | [docs/images/aihealthx.png]
 | |:---------------------------------------------------------------:|:---------
 ------------------------------------------------------:|:----------------------
 ----------------------------------------:|:------------------------------------
 -------------------:|:---------------------------------------------------------
---:|:-----------------------------------------------------------:| ##
-Acknowledge 1. We borrowed a lot of code from [Kaldi](http://kaldi-asr.org/
-) for data preparation. 2. We borrowed a lot of code from [ESPnet](https://
-github.com/espnet/espnet). FunASR follows up the training and finetuning
-pipelines of ESPnet. 3. We referred [Wenet](https://github.com/wenet-e2e/wenet)
-for building dataloader for large scale data training. 4. We acknowledge
-[ChinaTelecom](https://github.com/zhuzizyf/damo-fsmn-vad-infer-httpserver) for
-contributing the VAD runtime. 5. We acknowledge [RapidAI](https://github.com/
-RapidAI) for contributing the Paraformer and CT_Transformer-punc runtime. 6. We
-acknowledge [DeepScience](https://www.deepscience.cn) for contributing the grpc
-service. 6. We acknowledge [AiHealthx](http://www.aihealthx.com/) for
-contributing the websocket service and html5. ## License This project is
-licensed under the [The MIT License](https://opensource.org/licenses/MIT).
-FunASR also contains various third-party components and some code modified from
-other repos under other open source licenses. The use of pretraining model is
-subject to [model licencs](./MODEL_LICENSE) ## Citations ``` bibtex
-@inproceedings{gao2023funasr, author={Zhifu Gao and Zerui Li and Jiaming Wang
-and Haoneng Luo and Xian Shi and Mengzhe Chen and Yabin Li and Lingyun Zuo and
-Zhihao Du and Zhangyu Xiao and Shiliang Zhang}, title={FunASR: A Fundamental
-End-to-End Speech Recognition Toolkit}, year={2023}, booktitle={INTERSPEECH}, }
-@inproceedings{gao22b_interspeech, author={Zhifu Gao and ShiLiang Zhang and Ian
-McLoughlin and Zhijie Yan}, title={{Paraformer: Fast and Accurate Parallel
-Transformer for Non-autoregressive End-to-End Speech Recognition}}, year=2022,
-booktitle={Proc. Interspeech 2022}, pages={2063--2067}, doi={10.21437/
-Interspeech.2022-9996} } ```
+--:| ## Acknowledge 1. We borrowed a lot of code from [Kaldi](http://kaldi-
+asr.org/) for data preparation. 2. We borrowed a lot of code from [ESPnet]
+(https://github.com/espnet/espnet). FunASR follows up the training and
+finetuning pipelines of ESPnet. 3. We referred [Wenet](https://github.com/
+wenet-e2e/wenet) for building dataloader for large scale data training. 4. We
+acknowledge [ChinaTelecom](https://github.com/zhuzizyf/damo-fsmn-vad-infer-
+httpserver) for contributing the VAD runtime. 5. We acknowledge [RapidAI]
+(https://github.com/RapidAI) for contributing the Paraformer and
+CT_Transformer-punc runtime. 6. We acknowledge [AiHealthx](http://
+www.aihealthx.com/) for contributing the websocket service and html5. ##
+License This project is licensed under the [The MIT License](https://
+opensource.org/licenses/MIT). FunASR also contains various third-party
+components and some code modified from other repos under other open source
+licenses. The use of pretraining model is subject to [model licencs](./
+MODEL_LICENSE) ## Citations ``` bibtex @inproceedings{gao2023funasr, author=
+{Zhifu Gao and Zerui Li and Jiaming Wang and Haoneng Luo and Xian Shi and
+Mengzhe Chen and Yabin Li and Lingyun Zuo and Zhihao Du and Zhangyu Xiao and
+Shiliang Zhang}, title={FunASR: A Fundamental End-to-End Speech Recognition
+Toolkit}, year={2023}, booktitle={INTERSPEECH}, } @inproceedings
+{gao22b_interspeech, author={Zhifu Gao and ShiLiang Zhang and Ian McLoughlin
+and Zhijie Yan}, title={{Paraformer: Fast and Accurate Parallel Transformer for
+Non-autoregressive End-to-End Speech Recognition}}, year=2022, booktitle={Proc.
+Interspeech 2022}, pages={2063--2067}, doi={10.21437/Interspeech.2022-9996} }
+```
```

### Comparing `funasr-0.6.1/funasr/bin/aggregate_stats_dirs.py` & `funasr-0.6.2/funasr/bin/aggregate_stats_dirs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/bin/asr_infer.py` & `funasr-0.6.2/funasr/bin/asr_infer.py`

 * *Files 0% similar despite different names*

```diff
@@ -1647,23 +1647,25 @@
         streaming: bool = False,
         frontend_conf: dict = None,
         **kwargs,
     ):
         assert check_argument_types()
         
         # 1. Build ASR model
-        from funasr.tasks.sa_asr import ASRTask
+        from funasr.tasks.asr import ASRTaskSAASR
         scorers = {}
-        asr_model, asr_train_args = ASRTask.build_model_from_file(
+        asr_model, asr_train_args = ASRTaskSAASR.build_model_from_file(
             asr_train_config, asr_model_file, cmvn_file, device
         )
         frontend = None
         if asr_train_args.frontend is not None and asr_train_args.frontend_conf is not None:
-            if asr_train_args.frontend == 'wav_frontend':
-                frontend = WavFrontend(cmvn_file=cmvn_file, **asr_train_args.frontend_conf)
+            from funasr.tasks.sa_asr import frontend_choices
+            if asr_train_args.frontend == 'wav_frontend' or asr_train_args.frontend == "multichannelfrontend":
+                frontend_class = frontend_choices.get_class(asr_train_args.frontend)
+                frontend = frontend_class(cmvn_file=cmvn_file, **asr_train_args.frontend_conf).eval()
             else:
                 frontend_class = frontend_choices.get_class(asr_train_args.frontend)
                 frontend = frontend_class(**asr_train_args.frontend_conf).eval()
         
         logging.info("asr_model: {}".format(asr_model))
         logging.info("asr_train_args: {}".format(asr_train_args))
         asr_model.to(dtype=getattr(torch, dtype)).eval()
```

### Comparing `funasr-0.6.1/funasr/bin/asr_inference_launch.py` & `funasr-0.6.2/funasr/bin/asr_inference_launch.py`

 * *Files 1% similar despite different names*

```diff
@@ -654,14 +654,18 @@
             speech, speech_lengths = batch["speech"], batch["speech_lengths"]
             
             n = len(vadsegments)
             data_with_index = [(vadsegments[i], i) for i in range(n)]
             sorted_data = sorted(data_with_index, key=lambda x: x[0][1] - x[0][0])
             results_sorted = []
             batch_size_token_ms = batch_size_token*60
+            if speech2text.device == "cpu":
+                batch_size_token_ms = 0
+            batch_size_token_ms = max(batch_size_token_ms, sorted_data[0][0][1] - sorted_data[0][0][0])
+            
             batch_size_token_ms_cum = 0
             beg_idx = 0
             for j, _ in enumerate(range(0, n)):
                 batch_size_token_ms_cum += (sorted_data[j][0][1] - sorted_data[j][0][0])
                 if j < n-1 and (batch_size_token_ms_cum + sorted_data[j+1][0][1] - sorted_data[j+1][0][0])<batch_size_token_ms:
                     continue
                 batch_size_token_ms_cum = 0
```

### Comparing `funasr-0.6.1/funasr/bin/asr_train.py` & `funasr-0.6.2/funasr/bin/asr_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/bin/build_trainer.py` & `funasr-0.6.2/funasr/bin/build_trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/bin/data2vec_train.py` & `funasr-0.6.2/funasr/bin/data2vec_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/bin/diar_infer.py` & `funasr-0.6.2/funasr/bin/diar_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/bin/diar_inference_launch.py` & `funasr-0.6.2/funasr/bin/diar_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/bin/diar_train.py` & `funasr-0.6.2/funasr/bin/diar_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/bin/lm_inference_launch.py` & `funasr-0.6.2/funasr/bin/lm_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/bin/lm_train.py` & `funasr-0.6.2/funasr/bin/lm_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/bin/punc_infer.py` & `funasr-0.6.2/funasr/bin/punc_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/bin/punc_inference_launch.py` & `funasr-0.6.2/funasr/bin/punc_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/bin/punc_train.py` & `funasr-0.6.2/funasr/bin/punc_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/bin/sa_asr_train.py` & `funasr-0.6.2/funasr/bin/sa_asr_train.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/bin/sv_infer.py` & `funasr-0.6.2/funasr/bin/sv_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/bin/sv_inference_launch.py` & `funasr-0.6.2/funasr/bin/sv_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/bin/tokenize_text.py` & `funasr-0.6.2/funasr/bin/tokenize_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/bin/tp_infer.py` & `funasr-0.6.2/funasr/bin/tp_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/bin/tp_inference_launch.py` & `funasr-0.6.2/funasr/bin/tp_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/bin/train.py` & `funasr-0.6.2/funasr/bin/train.py`

 * *Files 1% similar despite different names*

```diff
@@ -295,15 +295,15 @@
         default=False,
         help="Ignore size mismatch when loading pre-trained model",
     )
     parser.add_argument(
         "--freeze_param",
         type=str,
         default=[],
-        nargs="*",
+        action="append",
         help="Freeze parameters",
     )
 
     # dataset related
     parser.add_argument(
         "--dataset_type",
         type=str,
```

### Comparing `funasr-0.6.1/funasr/bin/vad_infer.py` & `funasr-0.6.2/funasr/bin/vad_infer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/bin/vad_inference_launch.py` & `funasr-0.6.2/funasr/bin/vad_inference_launch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/build_utils/build_args.py` & `funasr-0.6.2/funasr/build_utils/build_args.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/build_utils/build_asr_model.py` & `funasr-0.6.2/funasr/build_utils/build_asr_model.py`

 * *Files 10% similar despite different names*

```diff
@@ -17,23 +17,26 @@
 from funasr.models.decoder.transformer_decoder import (
     LightweightConvolutionTransformerDecoder,  # noqa: H301
 )
 from funasr.models.decoder.transformer_decoder import ParaformerDecoderSAN
 from funasr.models.decoder.transformer_decoder import TransformerDecoder
 from funasr.models.decoder.rnnt_decoder import RNNTDecoder
 from funasr.models.joint_net.joint_network import JointNetwork
+from funasr.models.decoder.transformer_decoder import SAAsrTransformerDecoder
 from funasr.models.e2e_asr import ASRModel
 from funasr.models.e2e_asr_mfcca import MFCCA
+from funasr.models.e2e_sa_asr import SAASRModel
 from funasr.models.e2e_asr_paraformer import Paraformer, ParaformerOnline, ParaformerBert, BiCifParaformer, ContextualParaformer
 from funasr.models.e2e_tp import TimestampPredictor
 from funasr.models.e2e_uni_asr import UniASR
 from funasr.models.e2e_asr_transducer import TransducerModel, UnifiedTransducerModel
 from funasr.models.encoder.conformer_encoder import ConformerEncoder, ConformerChunkEncoder
 from funasr.models.encoder.data2vec_encoder import Data2VecEncoder
 from funasr.models.encoder.mfcca_encoder import MFCCAEncoder
+from funasr.models.encoder.resnet34_encoder import ResNet34Diar
 from funasr.models.encoder.rnn_encoder import RNNEncoder
 from funasr.models.encoder.sanm_encoder import SANMEncoder, SANMEncoderChunkOpt
 from funasr.models.encoder.transformer_encoder import TransformerEncoder
 from funasr.models.frontend.default import DefaultFrontend
 from funasr.models.frontend.default import MultiChannelFrontend
 from funasr.models.frontend.fused import FusedFrontends
 from funasr.models.frontend.s3prl import S3prlFrontend
@@ -86,14 +89,16 @@
         paraformer_bert=ParaformerBert,
         bicif_paraformer=BiCifParaformer,
         contextual_paraformer=ContextualParaformer,
         mfcca=MFCCA,
         timestamp_prediction=TimestampPredictor,
         rnnt=TransducerModel,
         rnnt_unified=UnifiedTransducerModel,
+        sa_asr=SAASRModel,
+
     ),
     default="asr",
 )
 encoder_choices = ClassChoices(
     "encoder",
     classes=dict(
         conformer=ConformerEncoder,
@@ -103,14 +108,35 @@
         sanm_chunk_opt=SANMEncoderChunkOpt,
         data2vec_encoder=Data2VecEncoder,
         mfcca_enc=MFCCAEncoder,
         chunk_conformer=ConformerChunkEncoder,
     ),
     default="rnn",
 )
+asr_encoder_choices = ClassChoices(
+    "asr_encoder",
+    classes=dict(
+        conformer=ConformerEncoder,
+        transformer=TransformerEncoder,
+        rnn=RNNEncoder,
+        sanm=SANMEncoder,
+        sanm_chunk_opt=SANMEncoderChunkOpt,
+        data2vec_encoder=Data2VecEncoder,
+        mfcca_enc=MFCCAEncoder,
+    ),
+    default="rnn",
+)
+
+spk_encoder_choices = ClassChoices(
+    "spk_encoder",
+    classes=dict(
+        resnet34_diar=ResNet34Diar,
+    ),
+    default="resnet34_diar",
+)
 encoder_choices2 = ClassChoices(
     "encoder2",
     classes=dict(
         conformer=ConformerEncoder,
         transformer=TransformerEncoder,
         rnn=RNNEncoder,
         sanm=SANMEncoder,
@@ -127,14 +153,15 @@
         dynamic_conv=DynamicConvolutionTransformerDecoder,
         dynamic_conv2d=DynamicConvolution2DTransformerDecoder,
         rnn=RNNDecoder,
         fsmn_scama_opt=FsmnDecoderSCAMAOpt,
         paraformer_decoder_sanm=ParaformerSANMDecoder,
         paraformer_decoder_san=ParaformerDecoderSAN,
         contextual_paraformer_decoder=ContextualParaformerDecoder,
+        sa_decoder=SAAsrTransformerDecoder,
     ),
     default="rnn",
 )
 decoder_choices2 = ClassChoices(
     "decoder2",
     classes=dict(
         transformer=TransformerDecoder,
@@ -218,14 +245,18 @@
     predictor_choices2,
     # --stride_conv and --stride_conv_conf
     stride_conv_choices,
     # --rnnt_decoder and --rnnt_decoder_conf
     rnnt_decoder_choices,
     # --joint_network and --joint_network_conf
     joint_network_choices,
+    # --asr_encoder and --asr_encoder_conf
+    asr_encoder_choices,
+    # --spk_encoder and --spk_encoder_conf
+    spk_encoder_choices,
 ]
 
 
 def build_asr_model(args):
     # token_list
     if args.token_list is not None:
         with open(args.token_list) as f:
@@ -235,15 +266,15 @@
         logging.info(f"Vocabulary size: {vocab_size}")
     else:
         vocab_size = None
 
     # frontend
     if args.input_size is None:
         frontend_class = frontend_choices.get_class(args.frontend)
-        if args.frontend == 'wav_frontend':
+        if args.frontend == 'wav_frontend' or args.frontend == 'multichannelfrontend':
             frontend = frontend_class(cmvn_file=args.cmvn_file, **args.frontend_conf)
         else:
             frontend = frontend_class(**args.frontend_conf)
         input_size = frontend.output_size()
     else:
         args.frontend = None
         args.frontend_conf = {}
@@ -409,14 +440,41 @@
             normalize=normalize,
             encoder=encoder,
             decoder=decoder,
             att_decoder=att_decoder,
             joint_network=joint_network,
             **args.model_conf,
         )
+    elif args.model == "sa_asr":
+        asr_encoder_class = asr_encoder_choices.get_class(args.asr_encoder)
+        asr_encoder = asr_encoder_class(input_size=input_size, **args.asr_encoder_conf)
+        spk_encoder_class = spk_encoder_choices.get_class(args.spk_encoder)
+        spk_encoder = spk_encoder_class(input_size=input_size, **args.spk_encoder_conf)
+        decoder = decoder_class(
+            vocab_size=vocab_size,
+            encoder_output_size=asr_encoder.output_size(),
+            **args.decoder_conf,
+        )
+        ctc = CTC(
+            odim=vocab_size, encoder_output_size=asr_encoder.output_size(), **args.ctc_conf
+        )
+
+        model_class = model_choices.get_class(args.model)
+        model = model_class(
+            vocab_size=vocab_size,
+            frontend=frontend,
+            specaug=specaug,
+            normalize=normalize,
+            asr_encoder=asr_encoder,
+            spk_encoder=spk_encoder,
+            decoder=decoder,
+            ctc=ctc,
+            token_list=token_list,
+            **args.model_conf,
+        )
 
     else:
         raise NotImplementedError("Not supported model: {}".format(args.model))
 
     # initialize
     if args.init is not None:
         initialize(model, args.init)
```

### Comparing `funasr-0.6.1/funasr/build_utils/build_dataloader.py` & `funasr-0.6.2/funasr/build_utils/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/build_utils/build_diar_model.py` & `funasr-0.6.2/funasr/build_utils/build_diar_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/build_utils/build_distributed.py` & `funasr-0.6.2/funasr/build_utils/build_distributed.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/build_utils/build_lm_model.py` & `funasr-0.6.2/funasr/build_utils/build_lm_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/build_utils/build_model.py` & `funasr-0.6.2/funasr/build_utils/build_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/build_utils/build_optimizer.py` & `funasr-0.6.2/funasr/build_utils/build_optimizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/build_utils/build_pretrain_model.py` & `funasr-0.6.2/funasr/build_utils/build_pretrain_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/build_utils/build_punc_model.py` & `funasr-0.6.2/funasr/build_utils/build_punc_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/build_utils/build_scheduler.py` & `funasr-0.6.2/funasr/build_utils/build_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/build_utils/build_trainer.py` & `funasr-0.6.2/funasr/build_utils/build_trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/build_utils/build_vad_model.py` & `funasr-0.6.2/funasr/build_utils/build_vad_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/datasets/collate_fn.py` & `funasr-0.6.2/funasr/datasets/collate_fn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/datasets/dataset.py` & `funasr-0.6.2/funasr/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/datasets/iterable_dataset.py` & `funasr-0.6.2/funasr/datasets/iterable_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/datasets/large_datasets/build_dataloader.py` & `funasr-0.6.2/funasr/datasets/large_datasets/build_dataloader.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/datasets/large_datasets/datapipes/batch.py` & `funasr-0.6.2/funasr/datasets/large_datasets/datapipes/batch.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/datasets/large_datasets/datapipes/filter.py` & `funasr-0.6.2/funasr/datasets/large_datasets/datapipes/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/datasets/large_datasets/dataset.py` & `funasr-0.6.2/funasr/datasets/large_datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/datasets/large_datasets/utils/clipping.py` & `funasr-0.6.2/funasr/datasets/large_datasets/utils/clipping.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/datasets/large_datasets/utils/filter.py` & `funasr-0.6.2/funasr/datasets/large_datasets/utils/filter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/datasets/large_datasets/utils/hotword_utils.py` & `funasr-0.6.2/funasr/datasets/large_datasets/utils/hotword_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/datasets/large_datasets/utils/low_frame_rate.py` & `funasr-0.6.2/funasr/datasets/large_datasets/utils/low_frame_rate.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/datasets/large_datasets/utils/padding.py` & `funasr-0.6.2/funasr/datasets/large_datasets/utils/padding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/datasets/large_datasets/utils/tokenize.py` & `funasr-0.6.2/funasr/datasets/large_datasets/utils/tokenize.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/datasets/ms_dataset.py` & `funasr-0.6.2/funasr/datasets/ms_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/datasets/preprocessor.py` & `funasr-0.6.2/funasr/datasets/preprocessor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/export/export_model.py` & `funasr-0.6.2/funasr/export/export_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/export/models/CT_Transformer.py` & `funasr-0.6.2/funasr/export/models/CT_Transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/export/models/__init__.py` & `funasr-0.6.2/funasr/export/models/__init__.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/export/models/decoder/sanm_decoder.py` & `funasr-0.6.2/funasr/export/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/export/models/decoder/transformer_decoder.py` & `funasr-0.6.2/funasr/export/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/export/models/e2e_asr_paraformer.py` & `funasr-0.6.2/funasr/export/models/e2e_asr_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/export/models/e2e_vad.py` & `funasr-0.6.2/funasr/export/models/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/export/models/encoder/conformer_encoder.py` & `funasr-0.6.2/funasr/export/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/export/models/encoder/fsmn_encoder.py` & `funasr-0.6.2/funasr/export/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/export/models/encoder/sanm_encoder.py` & `funasr-0.6.2/funasr/export/models/encoder/sanm_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/export/models/modules/decoder_layer.py` & `funasr-0.6.2/funasr/export/models/modules/decoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/export/models/modules/encoder_layer.py` & `funasr-0.6.2/funasr/export/models/modules/encoder_layer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/export/models/modules/feedforward.py` & `funasr-0.6.2/funasr/export/models/modules/feedforward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/export/models/modules/multihead_att.py` & `funasr-0.6.2/funasr/export/models/modules/multihead_att.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/export/models/predictor/cif.py` & `funasr-0.6.2/funasr/export/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/export/test/test_onnx.py` & `funasr-0.6.2/funasr/export/test/test_onnx.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/export/test/test_onnx_punc.py` & `funasr-0.6.2/funasr/export/test/test_onnx_punc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/export/test/test_onnx_punc_vadrealtime.py` & `funasr-0.6.2/funasr/export/test/test_onnx_punc_vadrealtime.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/export/test/test_onnx_vad.py` & `funasr-0.6.2/funasr/export/test/test_onnx_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/export/utils/torch_function.py` & `funasr-0.6.2/funasr/export/utils/torch_function.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/fileio/datadir_writer.py` & `funasr-0.6.2/funasr/fileio/datadir_writer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/fileio/npy_scp.py` & `funasr-0.6.2/funasr/fileio/npy_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/fileio/rand_gen_dataset.py` & `funasr-0.6.2/funasr/fileio/rand_gen_dataset.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/fileio/read_text.py` & `funasr-0.6.2/funasr/fileio/read_text.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/fileio/sound_scp.py` & `funasr-0.6.2/funasr/fileio/sound_scp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/iterators/chunk_iter_factory.py` & `funasr-0.6.2/funasr/iterators/chunk_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/iterators/multiple_iter_factory.py` & `funasr-0.6.2/funasr/iterators/multiple_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/iterators/sequence_iter_factory.py` & `funasr-0.6.2/funasr/iterators/sequence_iter_factory.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/layers/complex_utils.py` & `funasr-0.6.2/funasr/layers/complex_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/layers/global_mvn.py` & `funasr-0.6.2/funasr/layers/global_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/layers/label_aggregation.py` & `funasr-0.6.2/funasr/layers/label_aggregation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/layers/log_mel.py` & `funasr-0.6.2/funasr/layers/log_mel.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/layers/mask_along_axis.py` & `funasr-0.6.2/funasr/layers/mask_along_axis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/layers/sinc_conv.py` & `funasr-0.6.2/funasr/layers/sinc_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/layers/stft.py` & `funasr-0.6.2/funasr/layers/stft.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/layers/time_warp.py` & `funasr-0.6.2/funasr/layers/time_warp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/layers/utterance_mvn.py` & `funasr-0.6.2/funasr/layers/utterance_mvn.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/losses/label_smoothing_loss.py` & `funasr-0.6.2/funasr/losses/label_smoothing_loss.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/main_funcs/average_nbest_models.py` & `funasr-0.6.2/funasr/main_funcs/average_nbest_models.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/main_funcs/calculate_all_attentions.py` & `funasr-0.6.2/funasr/main_funcs/calculate_all_attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/main_funcs/collect_stats.py` & `funasr-0.6.2/funasr/main_funcs/collect_stats.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/main_funcs/pack_funcs.py` & `funasr-0.6.2/funasr/main_funcs/pack_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/ctc.py` & `funasr-0.6.2/funasr/models/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/data2vec.py` & `funasr-0.6.2/funasr/models/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/decoder/contextual_decoder.py` & `funasr-0.6.2/funasr/models/decoder/contextual_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/decoder/rnn_decoder.py` & `funasr-0.6.2/funasr/models/decoder/rnn_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/decoder/rnnt_decoder.py` & `funasr-0.6.2/funasr/models/decoder/rnnt_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/decoder/sanm_decoder.py` & `funasr-0.6.2/funasr/models/decoder/sanm_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/decoder/sv_decoder.py` & `funasr-0.6.2/funasr/models/decoder/sv_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/decoder/transformer_decoder.py` & `funasr-0.6.2/funasr/models/decoder/transformer_decoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/e2e_asr.py` & `funasr-0.6.2/funasr/models/e2e_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/e2e_asr_common.py` & `funasr-0.6.2/funasr/models/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/e2e_asr_contextual_paraformer.py` & `funasr-0.6.2/funasr/models/e2e_asr_contextual_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/e2e_asr_mfcca.py` & `funasr-0.6.2/funasr/models/e2e_asr_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/e2e_asr_paraformer.py` & `funasr-0.6.2/funasr/models/e2e_asr_paraformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/e2e_asr_transducer.py` & `funasr-0.6.2/funasr/models/e2e_asr_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/e2e_diar_eend_ola.py` & `funasr-0.6.2/funasr/models/e2e_diar_eend_ola.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/e2e_diar_sond.py` & `funasr-0.6.2/funasr/models/e2e_diar_sond.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/e2e_sa_asr.py` & `funasr-0.6.2/funasr/models/e2e_sa_asr.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,29 +36,27 @@
 else:
     # Nothing to do if torch<1.6.0
     @contextmanager
     def autocast(enabled=True):
         yield
 
 
-class ESPnetASRModel(FunASRModel):
+class SAASRModel(FunASRModel):
     """CTC-attention hybrid Encoder-Decoder model"""
 
     def __init__(
             self,
             vocab_size: int,
             max_spk_num: int,
             token_list: Union[Tuple[str, ...], List[str]],
             frontend: Optional[AbsFrontend],
             specaug: Optional[AbsSpecAug],
             normalize: Optional[AbsNormalize],
-            preencoder: Optional[AbsPreEncoder],
             asr_encoder: AbsEncoder,
             spk_encoder: torch.nn.Module,
-            postencoder: Optional[AbsPostEncoder],
             decoder: AbsDecoder,
             ctc: CTC,
             spk_weight: float = 0.5,
             ctc_weight: float = 0.5,
             interctc_weight: float = 0.0,
             ignore_id: int = -1,
             lsm_weight: float = 0.0,
@@ -85,16 +83,14 @@
         self.ctc_weight = ctc_weight
         self.interctc_weight = interctc_weight
         self.token_list = token_list.copy()
 
         self.frontend = frontend
         self.specaug = specaug
         self.normalize = normalize
-        self.preencoder = preencoder
-        self.postencoder = postencoder
         self.asr_encoder = asr_encoder
         self.spk_encoder = spk_encoder
 
         if not hasattr(self.asr_encoder, "interctc_use_conditioning"):
             self.asr_encoder.interctc_use_conditioning = False
         if self.asr_encoder.interctc_use_conditioning:
             self.asr_encoder.conditioning_layer = torch.nn.Linear(
@@ -289,18 +285,14 @@
             if self.specaug is not None and self.training:
                 feats, feats_lengths = self.specaug(feats, feats_lengths)
 
             # 3. Normalization for feature: e.g. Global-CMVN, Utterance-CMVN
             if self.normalize is not None:
                 feats, feats_lengths = self.normalize(feats, feats_lengths)
 
-        # Pre-encoder, e.g. used for raw input data
-        if self.preencoder is not None:
-            feats, feats_lengths = self.preencoder(feats, feats_lengths)
-
         # 4. Forward encoder
         # feats: (Batch, Length, Dim)
         # -> encoder_out: (Batch, Length2, Dim2)
         if self.asr_encoder.interctc_use_conditioning:
             encoder_out, encoder_out_lens, _ = self.asr_encoder(
                 feats, feats_lengths, ctc=self.ctc
             )
@@ -313,19 +305,14 @@
 
         encoder_out_spk_ori = self.spk_encoder(feats_raw, feats_lengths)[0]
         # import ipdb;ipdb.set_trace()
         if encoder_out_spk_ori.size(1)!=encoder_out.size(1):
             encoder_out_spk=F.interpolate(encoder_out_spk_ori.transpose(-2,-1), size=(encoder_out.size(1)), mode='nearest').transpose(-2,-1)
         else:
             encoder_out_spk=encoder_out_spk_ori
-        # Post-encoder, e.g. NLU
-        if self.postencoder is not None:
-            encoder_out, encoder_out_lens = self.postencoder(
-                encoder_out, encoder_out_lens
-            )
 
         assert encoder_out.size(0) == speech.size(0), (
             encoder_out.size(),
             speech.size(0),
         )
         assert encoder_out.size(1) <= encoder_out_lens.max(), (
             encoder_out.size(),
@@ -333,15 +320,15 @@
         )
         assert encoder_out_spk.size(0) == speech.size(0), (
             encoder_out_spk.size(),
             speech.size(0),
         )
 
         if intermediate_outs is not None:
-            return (encoder_out, intermediate_outs), encoder_out_lens
+            return (encoder_out, intermediate_outs), encoder_out_lens, encoder_out_spk
 
         return encoder_out, encoder_out_lens, encoder_out_spk
 
     def _extract_feats(
             self, speech: torch.Tensor, speech_lengths: torch.Tensor
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         assert speech_lengths.dim() == 1, speech_lengths.shape
```

### Comparing `funasr-0.6.1/funasr/models/e2e_sv.py` & `funasr-0.6.2/funasr/models/e2e_sv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/e2e_tp.py` & `funasr-0.6.2/funasr/models/e2e_tp.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/e2e_uni_asr.py` & `funasr-0.6.2/funasr/models/e2e_uni_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/e2e_vad.py` & `funasr-0.6.2/funasr/models/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/encoder/conformer_encoder.py` & `funasr-0.6.2/funasr/models/encoder/conformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/encoder/data2vec_encoder.py` & `funasr-0.6.2/funasr/models/encoder/data2vec_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/encoder/ecapa_tdnn_encoder.py` & `funasr-0.6.2/funasr/models/encoder/ecapa_tdnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/encoder/encoder_layer_mfcca.py` & `funasr-0.6.2/funasr/models/encoder/encoder_layer_mfcca.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/encoder/fsmn_encoder.py` & `funasr-0.6.2/funasr/models/encoder/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/encoder/mfcca_encoder.py` & `funasr-0.6.2/funasr/models/encoder/mfcca_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/encoder/opennmt_encoders/ci_scorers.py` & `funasr-0.6.2/funasr/models/encoder/opennmt_encoders/ci_scorers.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/encoder/opennmt_encoders/conv_encoder.py` & `funasr-0.6.2/funasr/models/encoder/opennmt_encoders/conv_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py` & `funasr-0.6.2/funasr/models/encoder/opennmt_encoders/fsmn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py` & `funasr-0.6.2/funasr/models/encoder/opennmt_encoders/self_attention_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/encoder/resnet34_encoder.py` & `funasr-0.6.2/funasr/models/encoder/resnet34_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/encoder/rnn_encoder.py` & `funasr-0.6.2/funasr/models/encoder/rnn_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/encoder/sanm_encoder.py` & `funasr-0.6.2/funasr/models/encoder/sanm_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/encoder/transformer_encoder.py` & `funasr-0.6.2/funasr/models/encoder/transformer_encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/frontend/default.py` & `funasr-0.6.2/funasr/models/frontend/default.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 import copy
 from typing import Optional
 from typing import Tuple
 from typing import Union
-
+import logging
 import humanfriendly
 import numpy as np
 import torch
 from torch_complex.tensor import ComplexTensor
 from typeguard import check_argument_types
 
 from funasr.layers.log_mel import LogMel
 from funasr.layers.stft import Stft
 from funasr.models.frontend.abs_frontend import AbsFrontend
 from funasr.modules.frontends.frontend import Frontend
 from funasr.utils.get_default_kwargs import get_default_kwargs
+from funasr.modules.nets_utils import make_pad_mask
 
 
 class DefaultFrontend(AbsFrontend):
     """Conventional frontend structure for ASR.
     Stft -> WPE -> MVDR-Beamformer -> Power-spec -> Mel-Fbank -> CMVN
     """
 
@@ -133,56 +134,55 @@
 
         # Change torch.Tensor to ComplexTensor
         # input_stft: (..., F, 2) -> (..., F)
         input_stft = ComplexTensor(input_stft[..., 0], input_stft[..., 1])
         return input_stft, feats_lens
 
 
-
-
 class MultiChannelFrontend(AbsFrontend):
     """Conventional frontend structure for ASR.
     Stft -> WPE -> MVDR-Beamformer -> Power-spec -> Mel-Fbank -> CMVN
     """
 
     def __init__(
             self,
             fs: Union[int, str] = 16000,
-            n_fft: int = 512,
-            win_length: int = None,
-            hop_length: int = 128,
+            n_fft: int = 400,
+            frame_length: int = 25,
+            frame_shift: int = 10,
             window: Optional[str] = "hann",
             center: bool = True,
             normalized: bool = False,
             onesided: bool = True,
             n_mels: int = 80,
             fmin: int = None,
             fmax: int = None,
             htk: bool = False,
             frontend_conf: Optional[dict] = get_default_kwargs(Frontend),
             apply_stft: bool = True,
-            frame_length: int = None,
-            frame_shift: int = None,
-            lfr_m: int = None,
-            lfr_n: int = None,
+            use_channel: int = None,
+            lfr_m: int = 1,
+            lfr_n: int = 1,
+            cmvn_file: str = None
     ):
         assert check_argument_types()
         super().__init__()
         if isinstance(fs, str):
             fs = humanfriendly.parse_size(fs)
 
         # Deepcopy (In general, dict shouldn't be used as default arg)
         frontend_conf = copy.deepcopy(frontend_conf)
-        self.hop_length = hop_length
+        self.win_length = frame_length * 16
+        self.hop_length = frame_shift * 16
 
         if apply_stft:
             self.stft = Stft(
                 n_fft=n_fft,
-                win_length=win_length,
-                hop_length=hop_length,
+                win_length=self.win_length,
+                hop_length=self.hop_length,
                 center=center,
                 window=window,
                 normalized=normalized,
                 onesided=onesided,
             )
         else:
             self.stft = None
@@ -198,64 +198,119 @@
             n_fft=n_fft,
             n_mels=n_mels,
             fmin=fmin,
             fmax=fmax,
             htk=htk,
         )
         self.n_mels = n_mels
-        self.frontend_type = "multichannelfrontend"
+        self.frontend_type = "default"
+        self.use_channel = use_channel
+        if self.use_channel is not None:
+            logging.info("use the channel %d" % (self.use_channel))
+        else:
+            logging.info("random select channel")
+        self.cmvn_file = cmvn_file
+        if self.cmvn_file is not None:
+            mean, std = self._load_cmvn(self.cmvn_file)
+            self.register_buffer("mean", torch.from_numpy(mean))
+            self.register_buffer("std", torch.from_numpy(std))
 
     def output_size(self) -> int:
         return self.n_mels
 
     def forward(
             self, input: torch.Tensor, input_lengths: torch.Tensor
     ) -> Tuple[torch.Tensor, torch.Tensor]:
         # 1. Domain-conversion: e.g. Stft: time -> time-freq
         #import pdb;pdb.set_trace()
         if self.stft is not None:
             input_stft, feats_lens = self._compute_stft(input, input_lengths)
         else:
-            if isinstance(input, ComplexTensor):
-                input_stft = input
-            else:
-                input_stft = ComplexTensor(input[..., 0], input[..., 1])
+            input_stft = ComplexTensor(input[..., 0], input[..., 1])
             feats_lens = input_lengths
         # 2. [Option] Speech enhancement
         if self.frontend is not None:
             assert isinstance(input_stft, ComplexTensor), type(input_stft)
             # input_stft: (Batch, Length, [Channel], Freq)
             input_stft, _, mask = self.frontend(input_stft, feats_lens)
+
+        # 3. [Multi channel case]: Select a channel
+        if input_stft.dim() == 4:
+            # h: (B, T, C, F) -> h: (B, T, F)
+            if self.training:
+                if self.use_channel is not None:
+                    input_stft = input_stft[:, :, self.use_channel, :]
+                    
+                else:
+                    # Select 1ch randomly
+                    ch = np.random.randint(input_stft.size(2))
+                    input_stft = input_stft[:, :, ch, :]
+            else:
+                # Use the first channel
+                input_stft = input_stft[:, :, 0, :]
+
         # 4. STFT -> Power spectrum
         # h: ComplexTensor(B, T, F) -> torch.Tensor(B, T, F)
         input_power = input_stft.real ** 2 + input_stft.imag ** 2
 
         # 5. Feature transform e.g. Stft -> Log-Mel-Fbank
         # input_power: (Batch, [Channel,] Length, Freq)
         #       -> input_feats: (Batch, Length, Dim)
         input_feats, _ = self.logmel(input_power, feats_lens)
-        bt = input_feats.size(0)
-        if input_feats.dim() ==4:
-            channel_size = input_feats.size(2)
-            # batch * channel * T * D
-            #pdb.set_trace()
-            input_feats = input_feats.transpose(1,2).reshape(bt*channel_size,-1,80).contiguous()
-            # input_feats = input_feats.transpose(1,2)
-            # batch * channel
-            feats_lens = feats_lens.repeat(1,channel_size).squeeze()
-        else:
-            channel_size = 1
-        return input_feats, feats_lens, channel_size
+        
+        # 6. Apply CMVN
+        if self.cmvn_file is not None:
+            if feats_lens is None:
+                feats_lens = input_feats.new_full([input_feats.size(0)], input_feats.size(1))
+            self.mean = self.mean.to(input_feats.device, input_feats.dtype)
+            self.std = self.std.to(input_feats.device, input_feats.dtype)
+            mask = make_pad_mask(feats_lens, input_feats, 1)
+
+            if input_feats.requires_grad:
+                input_feats = input_feats + self.mean
+            else:
+                input_feats += self.mean
+            if input_feats.requires_grad:
+                input_feats = input_feats.masked_fill(mask, 0.0)
+            else:
+                input_feats.masked_fill_(mask, 0.0)
+
+            input_feats *= self.std
+
+        return input_feats, feats_lens
 
     def _compute_stft(
             self, input: torch.Tensor, input_lengths: torch.Tensor
     ) -> torch.Tensor:
         input_stft, feats_lens = self.stft(input, input_lengths)
 
         assert input_stft.dim() >= 4, input_stft.shape
         # "2" refers to the real/imag parts of Complex
         assert input_stft.shape[-1] == 2, input_stft.shape
 
         # Change torch.Tensor to ComplexTensor
         # input_stft: (..., F, 2) -> (..., F)
         input_stft = ComplexTensor(input_stft[..., 0], input_stft[..., 1])
-        return input_stft, feats_lens
+        return input_stft, feats_lens
+
+    def _load_cmvn(self, cmvn_file):
+        with open(cmvn_file, 'r', encoding='utf-8') as f:
+            lines = f.readlines()
+        means_list = []
+        vars_list = []
+        for i in range(len(lines)):
+            line_item = lines[i].split()
+            if line_item[0] == '<AddShift>':
+                line_item = lines[i + 1].split()
+                if line_item[0] == '<LearnRateCoef>':
+                    add_shift_line = line_item[3:(len(line_item) - 1)]
+                    means_list = list(add_shift_line)
+                    continue
+            elif line_item[0] == '<Rescale>':
+                line_item = lines[i + 1].split()
+                if line_item[0] == '<LearnRateCoef>':
+                    rescale_line = line_item[3:(len(line_item) - 1)]
+                    vars_list = list(rescale_line)
+                    continue
+        means = np.array(means_list).astype(np.float)
+        vars = np.array(vars_list).astype(np.float)
+        return means, vars
```

### Comparing `funasr-0.6.1/funasr/models/frontend/eend_ola_feature.py` & `funasr-0.6.2/funasr/models/frontend/eend_ola_feature.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/frontend/fused.py` & `funasr-0.6.2/funasr/models/frontend/fused.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/frontend/s3prl.py` & `funasr-0.6.2/funasr/models/frontend/s3prl.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/frontend/wav_frontend.py` & `funasr-0.6.2/funasr/models/frontend/wav_frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/frontend/wav_frontend_kaldifeat.py` & `funasr-0.6.2/funasr/models/frontend/wav_frontend_kaldifeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/frontend/windowing.py` & `funasr-0.6.2/funasr/models/frontend/windowing.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/joint_net/joint_network.py` & `funasr-0.6.2/funasr/models/joint_net/joint_network.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/pooling/statistic_pooling.py` & `funasr-0.6.2/funasr/models/pooling/statistic_pooling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/postencoder/hugging_face_transformers_postencoder.py` & `funasr-0.6.2/funasr/models/postencoder/hugging_face_transformers_postencoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/predictor/cif.py` & `funasr-0.6.2/funasr/models/predictor/cif.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/preencoder/linear.py` & `funasr-0.6.2/funasr/models/preencoder/linear.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/preencoder/sinc.py` & `funasr-0.6.2/funasr/models/preencoder/sinc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/seq_rnn_lm.py` & `funasr-0.6.2/funasr/models/seq_rnn_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/specaug/specaug.py` & `funasr-0.6.2/funasr/models/specaug/specaug.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/target_delay_transformer.py` & `funasr-0.6.2/funasr/models/target_delay_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/transformer_lm.py` & `funasr-0.6.2/funasr/models/transformer_lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/models/vad_realtime_transformer.py` & `funasr-0.6.2/funasr/models/vad_realtime_transformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/add_sos_eos.py` & `funasr-0.6.2/funasr/modules/add_sos_eos.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/attention.py` & `funasr-0.6.2/funasr/modules/attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/beam_search/batch_beam_search.py` & `funasr-0.6.2/funasr/modules/beam_search/batch_beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/beam_search/batch_beam_search_online_sim.py` & `funasr-0.6.2/funasr/modules/beam_search/batch_beam_search_online_sim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/beam_search/beam_search.py` & `funasr-0.6.2/funasr/modules/beam_search/beam_search.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/beam_search/beam_search_sa_asr.py` & `funasr-0.6.2/funasr/modules/beam_search/beam_search_sa_asr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/beam_search/beam_search_transducer.py` & `funasr-0.6.2/funasr/modules/beam_search/beam_search_transducer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/data2vec/data_utils.py` & `funasr-0.6.2/funasr/modules/data2vec/data_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/data2vec/ema_module.py` & `funasr-0.6.2/funasr/modules/data2vec/ema_module.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/data2vec/multihead_attention.py` & `funasr-0.6.2/funasr/modules/data2vec/multihead_attention.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/data2vec/quant_noise.py` & `funasr-0.6.2/funasr/modules/data2vec/quant_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/data2vec/utils.py` & `funasr-0.6.2/funasr/modules/data2vec/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/data2vec/wav2vec2.py` & `funasr-0.6.2/funasr/modules/data2vec/wav2vec2.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/dynamic_conv.py` & `funasr-0.6.2/funasr/modules/dynamic_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/dynamic_conv2d.py` & `funasr-0.6.2/funasr/modules/dynamic_conv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/e2e_asr_common.py` & `funasr-0.6.2/funasr/modules/e2e_asr_common.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/eend_ola/encoder.py` & `funasr-0.6.2/funasr/modules/eend_ola/encoder.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/eend_ola/encoder_decoder_attractor.py` & `funasr-0.6.2/funasr/modules/eend_ola/encoder_decoder_attractor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/embedding.py` & `funasr-0.6.2/funasr/modules/embedding.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/frontends/beamformer.py` & `funasr-0.6.2/funasr/modules/frontends/beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/frontends/dnn_beamformer.py` & `funasr-0.6.2/funasr/modules/frontends/dnn_beamformer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/frontends/dnn_wpe.py` & `funasr-0.6.2/funasr/modules/frontends/dnn_wpe.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/frontends/feature_transform.py` & `funasr-0.6.2/funasr/modules/frontends/feature_transform.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/frontends/frontend.py` & `funasr-0.6.2/funasr/modules/frontends/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/frontends/mask_estimator.py` & `funasr-0.6.2/funasr/modules/frontends/mask_estimator.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/layer_norm.py` & `funasr-0.6.2/funasr/modules/layer_norm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/lightconv.py` & `funasr-0.6.2/funasr/modules/lightconv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/lightconv2d.py` & `funasr-0.6.2/funasr/modules/lightconv2d.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/mask.py` & `funasr-0.6.2/funasr/modules/mask.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/multi_layer_conv.py` & `funasr-0.6.2/funasr/modules/multi_layer_conv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/nets_utils.py` & `funasr-0.6.2/funasr/modules/nets_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/positionwise_feed_forward.py` & `funasr-0.6.2/funasr/modules/positionwise_feed_forward.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/repeat.py` & `funasr-0.6.2/funasr/modules/repeat.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/rnn/argument.py` & `funasr-0.6.2/funasr/modules/rnn/argument.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/rnn/attentions.py` & `funasr-0.6.2/funasr/modules/rnn/attentions.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/rnn/decoders.py` & `funasr-0.6.2/funasr/modules/rnn/decoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/rnn/encoders.py` & `funasr-0.6.2/funasr/modules/rnn/encoders.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/scorers/ctc.py` & `funasr-0.6.2/funasr/modules/scorers/ctc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/scorers/ctc_prefix_score.py` & `funasr-0.6.2/funasr/modules/scorers/ctc_prefix_score.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/scorers/length_bonus.py` & `funasr-0.6.2/funasr/modules/scorers/length_bonus.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/scorers/scorer_interface.py` & `funasr-0.6.2/funasr/modules/scorers/scorer_interface.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/streaming_utils/chunk_utilis.py` & `funasr-0.6.2/funasr/modules/streaming_utils/chunk_utilis.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/streaming_utils/load_fr_tf.py` & `funasr-0.6.2/funasr/modules/streaming_utils/load_fr_tf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/streaming_utils/utils.py` & `funasr-0.6.2/funasr/modules/streaming_utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/subsampling.py` & `funasr-0.6.2/funasr/modules/subsampling.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/modules/subsampling_without_posenc.py` & `funasr-0.6.2/funasr/modules/subsampling_without_posenc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/optimizers/fairseq_adam.py` & `funasr-0.6.2/funasr/optimizers/fairseq_adam.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/optimizers/sgd.py` & `funasr-0.6.2/funasr/optimizers/sgd.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/runtime/python/libtorch/demo.py` & `funasr-0.6.2/funasr/runtime/python/libtorch/demo.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py` & `funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py` & `funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py` & `funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py` & `funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py` & `funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py` & `funasr-0.6.2/funasr/runtime/python/libtorch/funasr_torch/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/runtime/python/libtorch/setup.py` & `funasr-0.6.2/funasr/runtime/python/libtorch/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py` & `funasr-0.6.2/funasr/runtime/python/onnxruntime/demo_paraformer_offline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/runtime/python/onnxruntime/demo_punc_offline.py` & `funasr-0.6.2/funasr/runtime/python/onnxruntime/demo_punc_offline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/runtime/python/onnxruntime/demo_punc_online.py` & `funasr-0.6.2/funasr/runtime/python/onnxruntime/demo_punc_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/runtime/python/onnxruntime/demo_vad_online.py` & `funasr-0.6.2/funasr/runtime/python/onnxruntime/demo_vad_online.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py` & `funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/paraformer_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py` & `funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/punc_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py` & `funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/e2e_vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py` & `funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/frontend.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py` & `funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py` & `funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/timestamp_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py` & `funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/utils/utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py` & `funasr-0.6.2/funasr/runtime/python/onnxruntime/funasr_onnx/vad_bin.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/runtime/python/onnxruntime/setup.py` & `funasr-0.6.2/funasr/runtime/python/onnxruntime/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/samplers/build_batch_sampler.py` & `funasr-0.6.2/funasr/samplers/build_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/samplers/folded_batch_sampler.py` & `funasr-0.6.2/funasr/samplers/folded_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/samplers/length_batch_sampler.py` & `funasr-0.6.2/funasr/samplers/length_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/samplers/num_elements_batch_sampler.py` & `funasr-0.6.2/funasr/samplers/num_elements_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/samplers/sorted_batch_sampler.py` & `funasr-0.6.2/funasr/samplers/sorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/samplers/unsorted_batch_sampler.py` & `funasr-0.6.2/funasr/samplers/unsorted_batch_sampler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/schedulers/abs_scheduler.py` & `funasr-0.6.2/funasr/schedulers/abs_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/schedulers/noam_lr.py` & `funasr-0.6.2/funasr/schedulers/noam_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/schedulers/tri_stage_scheduler.py` & `funasr-0.6.2/funasr/schedulers/tri_stage_scheduler.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/schedulers/warmup_lr.py` & `funasr-0.6.2/funasr/schedulers/warmup_lr.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/tasks/abs_task.py` & `funasr-0.6.2/funasr/tasks/abs_task.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/tasks/asr.py` & `funasr-0.6.2/funasr/tasks/asr.py`

 * *Files 3% similar despite different names*

```diff
@@ -34,30 +34,33 @@
 )
 from funasr.models.decoder.transformer_decoder import (
     LightweightConvolutionTransformerDecoder,  # noqa: H301
 )
 from funasr.models.decoder.transformer_decoder import ParaformerDecoderSAN
 from funasr.models.decoder.transformer_decoder import TransformerDecoder
 from funasr.models.decoder.contextual_decoder import ContextualParaformerDecoder
+from funasr.models.decoder.transformer_decoder import SAAsrTransformerDecoder
 from funasr.models.e2e_asr import ASRModel
 from funasr.models.decoder.rnnt_decoder import RNNTDecoder
 from funasr.models.joint_net.joint_network import JointNetwork
 from funasr.models.e2e_asr_paraformer import Paraformer, ParaformerOnline, ParaformerBert, BiCifParaformer, ContextualParaformer
 from funasr.models.e2e_asr_contextual_paraformer import NeatContextualParaformer
 from funasr.models.e2e_tp import TimestampPredictor
 from funasr.models.e2e_asr_mfcca import MFCCA
+from funasr.models.e2e_sa_asr import SAASRModel
 from funasr.models.e2e_uni_asr import UniASR
 from funasr.models.e2e_asr_transducer import TransducerModel, UnifiedTransducerModel
 from funasr.models.encoder.abs_encoder import AbsEncoder
 from funasr.models.encoder.conformer_encoder import ConformerEncoder, ConformerChunkEncoder
 from funasr.models.encoder.data2vec_encoder import Data2VecEncoder
 from funasr.models.encoder.rnn_encoder import RNNEncoder
 from funasr.models.encoder.sanm_encoder import SANMEncoder, SANMEncoderChunkOpt
 from funasr.models.encoder.transformer_encoder import TransformerEncoder
 from funasr.models.encoder.mfcca_encoder import MFCCAEncoder
+from funasr.models.encoder.resnet34_encoder import ResNet34Diar
 from funasr.models.frontend.abs_frontend import AbsFrontend
 from funasr.models.frontend.default import DefaultFrontend
 from funasr.models.frontend.default import MultiChannelFrontend
 from funasr.models.frontend.fused import FusedFrontends
 from funasr.models.frontend.s3prl import S3prlFrontend
 from funasr.models.frontend.wav_frontend import WavFrontend
 from funasr.models.frontend.windowing import SlidingWindow
@@ -130,14 +133,15 @@
         bicif_paraformer=BiCifParaformer,
         contextual_paraformer=ContextualParaformer,
         neatcontextual_paraformer=NeatContextualParaformer,
         mfcca=MFCCA,
         timestamp_prediction=TimestampPredictor,
         rnnt=TransducerModel,
         rnnt_unified=UnifiedTransducerModel,
+        sa_asr=SAASRModel,
     ),
     type_check=FunASRModel,
     default="asr",
 )
 preencoder_choices = ClassChoices(
     name="preencoder",
     classes=dict(
@@ -171,14 +175,35 @@
         rnn=RNNEncoder,
         sanm=SANMEncoder,
         sanm_chunk_opt=SANMEncoderChunkOpt,
     ),
     type_check=AbsEncoder,
     default="rnn",
 )
+asr_encoder_choices = ClassChoices(
+    "asr_encoder",
+    classes=dict(
+        conformer=ConformerEncoder,
+        transformer=TransformerEncoder,
+        rnn=RNNEncoder,
+        sanm=SANMEncoder,
+        sanm_chunk_opt=SANMEncoderChunkOpt,
+        data2vec_encoder=Data2VecEncoder,
+        mfcca_enc=MFCCAEncoder,
+    ),
+    type_check=AbsEncoder,
+    default="rnn",
+)
+spk_encoder_choices = ClassChoices(
+    "spk_encoder",
+    classes=dict(
+        resnet34_diar=ResNet34Diar,
+    ),
+    default="resnet34_diar",
+)
 postencoder_choices = ClassChoices(
     name="postencoder",
     classes=dict(
         hugging_face_transformers=HuggingFaceTransformersPostEncoder,
     ),
     type_check=AbsPostEncoder,
     default=None,
@@ -193,14 +218,15 @@
         dynamic_conv=DynamicConvolutionTransformerDecoder,
         dynamic_conv2d=DynamicConvolution2DTransformerDecoder,
         rnn=RNNDecoder,
         fsmn_scama_opt=FsmnDecoderSCAMAOpt,
         paraformer_decoder_sanm=ParaformerSANMDecoder,
         paraformer_decoder_san=ParaformerDecoderSAN,
         contextual_paraformer_decoder=ContextualParaformerDecoder,
+        sa_decoder=SAAsrTransformerDecoder,
     ),
     type_check=AbsDecoder,
     default="rnn",
 )
 decoder_choices2 = ClassChoices(
     "decoder2",
     classes=dict(
@@ -326,14 +352,20 @@
         group.add_argument(
             "--split_with_space",
             type=str2bool,
             default=True,
             help="whether to split text using <space>",
         )
         group.add_argument(
+            "--max_spk_num",
+            type=int_or_none,
+            default=None,
+            help="A text mapping int-id to token",
+        )
+        group.add_argument(
             "--seg_dict_file",
             type=str,
             default=None,
             help="seg_dict_file for text processing",
         )
         group.add_argument(
             "--init",
@@ -1491,7 +1523,127 @@
                 "Currently not supported.",
                 "Initialization part will be reworked in a short future.",
             )
 
         #assert check_return_type(model)
 
         return model
+
+
+class ASRTaskSAASR(ASRTask):
+    # If you need more than one optimizers, change this value
+    num_optimizers: int = 1
+
+    # Add variable objects configurations
+    class_choices_list = [
+        # --frontend and --frontend_conf
+        frontend_choices,
+        # --specaug and --specaug_conf
+        specaug_choices,
+        # --normalize and --normalize_conf
+        normalize_choices,
+        # --model and --model_conf
+        model_choices,
+        # --preencoder and --preencoder_conf
+        preencoder_choices,
+        # --encoder and --encoder_conf
+        # --asr_encoder and --asr_encoder_conf
+        asr_encoder_choices,
+        # --spk_encoder and --spk_encoder_conf
+        spk_encoder_choices,
+        # --decoder and --decoder_conf
+        decoder_choices,
+    ]
+
+    # If you need to modify train() or eval() procedures, change Trainer class here
+    trainer = Trainer
+
+    @classmethod
+    def build_model(cls, args: argparse.Namespace):
+        assert check_argument_types()
+        if isinstance(args.token_list, str):
+            with open(args.token_list, encoding="utf-8") as f:
+                token_list = [line.rstrip() for line in f]
+
+            # Overwriting token_list to keep it as "portable".
+            args.token_list = list(token_list)
+        elif isinstance(args.token_list, (tuple, list)):
+            token_list = list(args.token_list)
+        else:
+            raise RuntimeError("token_list must be str or list")
+        vocab_size = len(token_list)
+        logging.info(f"Vocabulary size: {vocab_size}")
+
+        # 1. frontend
+        if args.input_size is None:
+            # Extract features in the model
+            frontend_class = frontend_choices.get_class(args.frontend)
+            if args.frontend == 'wav_frontend' or args.frontend == "multichannelfrontend":
+                frontend = frontend_class(cmvn_file=args.cmvn_file, **args.frontend_conf)
+            else:
+                frontend = frontend_class(**args.frontend_conf)
+            input_size = frontend.output_size()
+        else:
+            # Give features from data-loader
+            args.frontend = None
+            args.frontend_conf = {}
+            frontend = None
+            input_size = args.input_size
+
+        # 2. Data augmentation for spectrogram
+        if args.specaug is not None:
+            specaug_class = specaug_choices.get_class(args.specaug)
+            specaug = specaug_class(**args.specaug_conf)
+        else:
+            specaug = None
+
+        # 3. Normalization layer
+        if args.normalize is not None:
+            normalize_class = normalize_choices.get_class(args.normalize)
+            normalize = normalize_class(**args.normalize_conf)
+        else:
+            normalize = None
+
+        # 5. Encoder
+        asr_encoder_class = asr_encoder_choices.get_class(args.asr_encoder)
+        asr_encoder = asr_encoder_class(input_size=input_size, **args.asr_encoder_conf)
+        spk_encoder_class = spk_encoder_choices.get_class(args.spk_encoder)
+        spk_encoder = spk_encoder_class(input_size=input_size, **args.spk_encoder_conf)
+
+        # 7. Decoder
+        decoder_class = decoder_choices.get_class(args.decoder)
+        decoder = decoder_class(
+            vocab_size=vocab_size,
+            encoder_output_size=asr_encoder.output_size(),
+            **args.decoder_conf,
+        )
+
+        # 8. CTC
+        ctc = CTC(
+            odim=vocab_size, encoder_output_size=asr_encoder.output_size(), **args.ctc_conf
+        )
+
+        # import ipdb;ipdb.set_trace()
+        # 9. Build model
+        try:
+            model_class = model_choices.get_class(args.model)
+        except AttributeError:
+            model_class = model_choices.get_class("asr")
+        model = model_class(
+            vocab_size=vocab_size,
+            frontend=frontend,
+            specaug=specaug,
+            normalize=normalize,
+            asr_encoder=asr_encoder,
+            spk_encoder=spk_encoder,
+            decoder=decoder,
+            ctc=ctc,
+            token_list=token_list,
+            **args.model_conf,
+        )
+
+        # 10. Initialize
+        if args.init is not None:
+            initialize(model, args.init)
+
+        assert check_return_type(model)
+        return model
```

### Comparing `funasr-0.6.1/funasr/tasks/data2vec.py` & `funasr-0.6.2/funasr/tasks/data2vec.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/tasks/diar.py` & `funasr-0.6.2/funasr/tasks/diar.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/tasks/lm.py` & `funasr-0.6.2/funasr/tasks/lm.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/tasks/punctuation.py` & `funasr-0.6.2/funasr/tasks/punctuation.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/tasks/sa_asr.py` & `funasr-0.6.2/funasr/tasks/sa_asr.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,15 +35,15 @@
 )
 from funasr.models.decoder.transformer_decoder import (
     LightweightConvolutionTransformerDecoder,  # noqa: H301
 )
 from funasr.models.decoder.transformer_decoder import ParaformerDecoderSAN
 from funasr.models.decoder.transformer_decoder import TransformerDecoder
 from funasr.models.decoder.contextual_decoder import ContextualParaformerDecoder
-from funasr.models.e2e_sa_asr import ESPnetASRModel
+from funasr.models.e2e_sa_asr import SAASRModel
 from funasr.models.e2e_asr_paraformer import Paraformer, ParaformerBert, BiCifParaformer, ContextualParaformer
 from funasr.models.e2e_tp import TimestampPredictor
 from funasr.models.e2e_asr_mfcca import MFCCA
 from funasr.models.e2e_uni_asr import UniASR
 from funasr.models.encoder.abs_encoder import AbsEncoder
 from funasr.models.encoder.conformer_encoder import ConformerEncoder
 from funasr.models.encoder.data2vec_encoder import Data2VecEncoder
@@ -116,15 +116,15 @@
     type_check=AbsNormalize,
     default=None,
     optional=True,
 )
 model_choices = ClassChoices(
     "model",
     classes=dict(
-        asr=ESPnetASRModel,
+        asr=SAASRModel,
         uniasr=UniASR,
         paraformer=Paraformer,
         paraformer_bert=ParaformerBert,
         bicif_paraformer=BiCifParaformer,
         contextual_paraformer=ContextualParaformer,
         mfcca=MFCCA,
         timestamp_prediction=TimestampPredictor,
@@ -616,8 +616,8 @@
         )
 
         # 10. Initialize
         if args.init is not None:
             initialize(model, args.init)
 
         assert check_return_type(model)
-        return model
+        return model
```

### Comparing `funasr-0.6.1/funasr/tasks/sv.py` & `funasr-0.6.2/funasr/tasks/sv.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/tasks/vad.py` & `funasr-0.6.2/funasr/tasks/vad.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/text/build_tokenizer.py` & `funasr-0.6.2/funasr/text/build_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/text/char_tokenizer.py` & `funasr-0.6.2/funasr/text/char_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/text/cleaner.py` & `funasr-0.6.2/funasr/text/cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/text/korean_cleaner.py` & `funasr-0.6.2/funasr/text/korean_cleaner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/text/phoneme_tokenizer.py` & `funasr-0.6.2/funasr/text/phoneme_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/text/sentencepiece_tokenizer.py` & `funasr-0.6.2/funasr/text/sentencepiece_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/text/token_id_converter.py` & `funasr-0.6.2/funasr/text/token_id_converter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/text/word_tokenizer.py` & `funasr-0.6.2/funasr/text/word_tokenizer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/torch_utils/add_gradient_noise.py` & `funasr-0.6.2/funasr/torch_utils/add_gradient_noise.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/torch_utils/device_funcs.py` & `funasr-0.6.2/funasr/torch_utils/device_funcs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/torch_utils/forward_adaptor.py` & `funasr-0.6.2/funasr/torch_utils/forward_adaptor.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/torch_utils/initialize.py` & `funasr-0.6.2/funasr/torch_utils/initialize.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/torch_utils/load_pretrained_model.py` & `funasr-0.6.2/funasr/torch_utils/load_pretrained_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/torch_utils/model_summary.py` & `funasr-0.6.2/funasr/torch_utils/model_summary.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/torch_utils/recursive_op.py` & `funasr-0.6.2/funasr/torch_utils/recursive_op.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/train/abs_model.py` & `funasr-0.6.2/funasr/train/abs_model.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/train/class_choices.py` & `funasr-0.6.2/funasr/train/class_choices.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/train/distributed_utils.py` & `funasr-0.6.2/funasr/train/distributed_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/train/reporter.py` & `funasr-0.6.2/funasr/train/reporter.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/train/trainer.py` & `funasr-0.6.2/funasr/train/trainer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/utils/asr_env_checking.py` & `funasr-0.6.2/funasr/utils/asr_env_checking.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/utils/asr_utils.py` & `funasr-0.6.2/funasr/utils/asr_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/utils/build_dataclass.py` & `funasr-0.6.2/funasr/utils/build_dataclass.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/utils/cli_utils.py` & `funasr-0.6.2/funasr/utils/cli_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/utils/compute_eer.py` & `funasr-0.6.2/funasr/utils/compute_eer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/utils/compute_min_dcf.py` & `funasr-0.6.2/funasr/utils/compute_min_dcf.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/utils/compute_wer.py` & `funasr-0.6.2/funasr/utils/compute_wer.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/utils/config_argparse.py` & `funasr-0.6.2/funasr/utils/config_argparse.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/utils/get_default_kwargs.py` & `funasr-0.6.2/funasr/utils/get_default_kwargs.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/utils/griffin_lim.py` & `funasr-0.6.2/funasr/utils/griffin_lim.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/utils/job_runner.py` & `funasr-0.6.2/funasr/utils/job_runner.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/utils/misc.py` & `funasr-0.6.2/funasr/utils/misc.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/utils/modelscope_param.py` & `funasr-0.6.2/funasr/utils/modelscope_param.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/utils/modelscope_utils.py` & `funasr-0.6.2/funasr/utils/modelscope_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/utils/nested_dict_action.py` & `funasr-0.6.2/funasr/utils/nested_dict_action.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/utils/postprocess_utils.py` & `funasr-0.6.2/funasr/utils/postprocess_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/utils/prepare_data.py` & `funasr-0.6.2/funasr/utils/prepare_data.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/utils/sized_dict.py` & `funasr-0.6.2/funasr/utils/sized_dict.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/utils/timestamp_tools.py` & `funasr-0.6.2/funasr/utils/timestamp_tools.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/utils/types.py` & `funasr-0.6.2/funasr/utils/types.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/utils/vad_utils.py` & `funasr-0.6.2/funasr/utils/vad_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr/utils/wav_utils.py` & `funasr-0.6.2/funasr/utils/wav_utils.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr.egg-info/PKG-INFO` & `funasr-0.6.2/funasr.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: funasr
-Version: 0.6.1
+Version: 0.6.2
 Summary: FunASR: A Fundamental End-to-End Speech Recognition Toolkit
 Home-page: https://github.com/alibaba-damo-academy/FunASR.git
 Author: Speech Lab of DAMO Academy, Alibaba Group
 Author-email: funasr@list.alibaba-inc.com
 License: The MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
@@ -94,25 +94,24 @@
 
 |Dingding group |                     Wechat group                      |
 |:---:|:-----------------------------------------------------:|
 |<div align="left"><img src="docs/images/dingding.jpg" width="250"/> | <img src="docs/images/wechat.png" width="232"/></div> |
 
 ## Contributors
 
-| <div align="left"><img src="docs/images/damo.png" width="180"/> | <div align="left"><img src="docs/images/nwpu.png" width="260"/> | <img src="docs/images/China_Telecom.png" width="200"/> </div>  | <img src="docs/images/RapidAI.png" width="200"/> </div> | <img src="docs/images/DeepScience.png" width="200"/> </div> | <img src="docs/images/aihealthx.png" width="200"/> </div> |
-|:---------------------------------------------------------------:|:---------------------------------------------------------------:|:--------------------------------------------------------------:|:-------------------------------------------------------:|:-----------------------------------------------------------:|:-----------------------------------------------------------:|
+| <div align="left"><img src="docs/images/damo.png" width="180"/> | <div align="left"><img src="docs/images/nwpu.png" width="260"/> | <img src="docs/images/China_Telecom.png" width="200"/> </div>  | <img src="docs/images/RapidAI.png" width="200"/> </div> | <img src="docs/images/aihealthx.png" width="200"/> </div> |
+|:---------------------------------------------------------------:|:---------------------------------------------------------------:|:--------------------------------------------------------------:|:-------------------------------------------------------:|:-----------------------------------------------------------:|
 
 ## Acknowledge
 
 1. We borrowed a lot of code from [Kaldi](http://kaldi-asr.org/) for data preparation.
 2. We borrowed a lot of code from [ESPnet](https://github.com/espnet/espnet). FunASR follows up the training and finetuning pipelines of ESPnet.
 3. We referred [Wenet](https://github.com/wenet-e2e/wenet) for building dataloader for large scale data training.
 4. We acknowledge [ChinaTelecom](https://github.com/zhuzizyf/damo-fsmn-vad-infer-httpserver) for contributing the VAD runtime. 
 5. We acknowledge [RapidAI](https://github.com/RapidAI) for contributing the Paraformer and CT_Transformer-punc runtime.
-6. We acknowledge [DeepScience](https://www.deepscience.cn) for contributing the grpc service.
 6. We acknowledge [AiHealthx](http://www.aihealthx.com/) for contributing the websocket service and html5.
 
 ## License
 This project is licensed under the [The MIT License](https://opensource.org/licenses/MIT). FunASR also contains various third-party components and some code modified from other repos under other open source licenses.
 The use of pretraining model is subject to [model licencs](./MODEL_LICENSE)
 
 ## Citations
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: funasr Version: 0.6.1 Summary: FunASR: A
+Metadata-Version: 2.1 Name: funasr Version: 0.6.2 Summary: FunASR: A
 Fundamental End-to-End Speech Recognition Toolkit Home-page: https://
 github.com/alibaba-damo-academy/FunASR.git Author: Speech Lab of DAMO Academy,
 Alibaba Group Author-email: funasr@list.alibaba-inc.com License: The MIT
 License Classifier: Programming Language :: Python Classifier: Programming
 Language :: Python :: 3 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8 Classifier: Programming
 Language :: Python :: 3.9 Classifier: Development Status :: 5 - Production/
@@ -73,38 +73,36 @@
 inc.com) |Dingding group | Wechat group | |:---:|:-----------------------------
 ------------------------:| |
 [docs/images/dingding.jpg] | [docs/images/wechat.png]
 | ## Contributors |
 [docs/images/damo.png] |
 [docs/images/nwpu.png] | [docs/images/China_Telecom.png]
 | [docs/images/RapidAI.png]
-| [docs/images/DeepScience.png]
 | [docs/images/aihealthx.png]
 | |:---------------------------------------------------------------:|:---------
 ------------------------------------------------------:|:----------------------
 ----------------------------------------:|:------------------------------------
 -------------------:|:---------------------------------------------------------
---:|:-----------------------------------------------------------:| ##
-Acknowledge 1. We borrowed a lot of code from [Kaldi](http://kaldi-asr.org/
-) for data preparation. 2. We borrowed a lot of code from [ESPnet](https://
-github.com/espnet/espnet). FunASR follows up the training and finetuning
-pipelines of ESPnet. 3. We referred [Wenet](https://github.com/wenet-e2e/wenet)
-for building dataloader for large scale data training. 4. We acknowledge
-[ChinaTelecom](https://github.com/zhuzizyf/damo-fsmn-vad-infer-httpserver) for
-contributing the VAD runtime. 5. We acknowledge [RapidAI](https://github.com/
-RapidAI) for contributing the Paraformer and CT_Transformer-punc runtime. 6. We
-acknowledge [DeepScience](https://www.deepscience.cn) for contributing the grpc
-service. 6. We acknowledge [AiHealthx](http://www.aihealthx.com/) for
-contributing the websocket service and html5. ## License This project is
-licensed under the [The MIT License](https://opensource.org/licenses/MIT).
-FunASR also contains various third-party components and some code modified from
-other repos under other open source licenses. The use of pretraining model is
-subject to [model licencs](./MODEL_LICENSE) ## Citations ``` bibtex
-@inproceedings{gao2023funasr, author={Zhifu Gao and Zerui Li and Jiaming Wang
-and Haoneng Luo and Xian Shi and Mengzhe Chen and Yabin Li and Lingyun Zuo and
-Zhihao Du and Zhangyu Xiao and Shiliang Zhang}, title={FunASR: A Fundamental
-End-to-End Speech Recognition Toolkit}, year={2023}, booktitle={INTERSPEECH}, }
-@inproceedings{gao22b_interspeech, author={Zhifu Gao and ShiLiang Zhang and Ian
-McLoughlin and Zhijie Yan}, title={{Paraformer: Fast and Accurate Parallel
-Transformer for Non-autoregressive End-to-End Speech Recognition}}, year=2022,
-booktitle={Proc. Interspeech 2022}, pages={2063--2067}, doi={10.21437/
-Interspeech.2022-9996} } ```
+--:| ## Acknowledge 1. We borrowed a lot of code from [Kaldi](http://kaldi-
+asr.org/) for data preparation. 2. We borrowed a lot of code from [ESPnet]
+(https://github.com/espnet/espnet). FunASR follows up the training and
+finetuning pipelines of ESPnet. 3. We referred [Wenet](https://github.com/
+wenet-e2e/wenet) for building dataloader for large scale data training. 4. We
+acknowledge [ChinaTelecom](https://github.com/zhuzizyf/damo-fsmn-vad-infer-
+httpserver) for contributing the VAD runtime. 5. We acknowledge [RapidAI]
+(https://github.com/RapidAI) for contributing the Paraformer and
+CT_Transformer-punc runtime. 6. We acknowledge [AiHealthx](http://
+www.aihealthx.com/) for contributing the websocket service and html5. ##
+License This project is licensed under the [The MIT License](https://
+opensource.org/licenses/MIT). FunASR also contains various third-party
+components and some code modified from other repos under other open source
+licenses. The use of pretraining model is subject to [model licencs](./
+MODEL_LICENSE) ## Citations ``` bibtex @inproceedings{gao2023funasr, author=
+{Zhifu Gao and Zerui Li and Jiaming Wang and Haoneng Luo and Xian Shi and
+Mengzhe Chen and Yabin Li and Lingyun Zuo and Zhihao Du and Zhangyu Xiao and
+Shiliang Zhang}, title={FunASR: A Fundamental End-to-End Speech Recognition
+Toolkit}, year={2023}, booktitle={INTERSPEECH}, } @inproceedings
+{gao22b_interspeech, author={Zhifu Gao and ShiLiang Zhang and Ian McLoughlin
+and Zhijie Yan}, title={{Paraformer: Fast and Accurate Parallel Transformer for
+Non-autoregressive End-to-End Speech Recognition}}, year=2022, booktitle={Proc.
+Interspeech 2022}, pages={2063--2067}, doi={10.21437/Interspeech.2022-9996} }
+```
```

### Comparing `funasr-0.6.1/funasr.egg-info/SOURCES.txt` & `funasr-0.6.2/funasr.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/funasr.egg-info/requires.txt` & `funasr-0.6.2/funasr.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/setup.py` & `funasr-0.6.2/setup.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/tests/test_asr_inference_pipeline.py` & `funasr-0.6.2/tests/test_asr_inference_pipeline.py`

 * *Files 1% similar despite different names*

```diff
@@ -83,54 +83,60 @@
         inference_pipeline = pipeline(
             task=Tasks.auto_speech_recognition,
             model='damo/speech_paraformer-large-contextual_asr_nat-zh-cn-16k-common-vocab8404',
             param_dict=param_dict)
         rec_result = inference_pipeline(
             audio_in='https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/asr_example_hotword.wav')
         logger.info("asr inference result: {0}".format(rec_result))
+        assert rec_result["text"] == "国务院发展研究中心市场经济研究所副所长邓郁松认为"
 
     def test_paraformer_large_aishell1(self):
         inference_pipeline = pipeline(
             task=Tasks.auto_speech_recognition,
             model='damo/speech_paraformer-large_asr_nat-zh-cn-16k-aishell1-vocab8404-pytorch')
         rec_result = inference_pipeline(
             audio_in='https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/asr_example_zh.wav')
         logger.info("asr inference result: {0}".format(rec_result))
+        assert rec_result["text"] == "欢迎大家来体验达摩院推出的语音识别模型"
 
     def test_paraformer_large_aishell2(self):
         inference_pipeline = pipeline(
             task=Tasks.auto_speech_recognition,
             model='damo/speech_paraformer-large_asr_nat-zh-cn-16k-aishell2-vocab8404-pytorch')
         rec_result = inference_pipeline(
             audio_in='https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/asr_example_zh.wav')
         logger.info("asr inference result: {0}".format(rec_result))
+        assert rec_result["text"] == "欢迎大家来体验达摩院推出的语音识别模型"
 
     def test_paraformer_large_common(self):
         inference_pipeline = pipeline(
             task=Tasks.auto_speech_recognition,
             model='damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-pytorch')
         rec_result = inference_pipeline(
             audio_in='https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/asr_example_zh.wav')
         logger.info("asr inference result: {0}".format(rec_result))
+        assert rec_result["text"] == "欢迎大家来体验达摩院推出的语音识别模型"
 
     def test_paraformer_large_online_common(self):
         inference_pipeline = pipeline(
             task=Tasks.auto_speech_recognition,
             model='damo/speech_paraformer-large_asr_nat-zh-cn-16k-common-vocab8404-online')
         rec_result = inference_pipeline(
             audio_in='https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/asr_example_zh.wav')
         logger.info("asr inference result: {0}".format(rec_result))
+        assert rec_result["text"] == "欢迎大 家来 体验达 摩院推 出的 语音识 别模 型"
 
     def test_paraformer_online_common(self):
         inference_pipeline = pipeline(
             task=Tasks.auto_speech_recognition,
             model='damo/speech_paraformer_asr_nat-zh-cn-16k-common-vocab8404-online')
         rec_result = inference_pipeline(
             audio_in='https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/asr_example_zh.wav')
         logger.info("asr inference result: {0}".format(rec_result))
+        assert rec_result["text"] == "欢迎 大家来 体验达 摩院推 出的 语音识 别模 型"
 
     def test_paraformer_tiny_commandword(self):
         inference_pipeline = pipeline(
             task=Tasks.auto_speech_recognition,
             model='damo/speech_paraformer-tiny-commandword_asr_nat-zh-cn-16k-vocab544-pytorch')
         rec_result = inference_pipeline(
             audio_in='https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/asr_example_zh_command.wav')
```

### Comparing `funasr-0.6.1/tests/test_asr_vad_punc_inference_pipeline.py` & `funasr-0.6.2/tests/test_asr_vad_punc_inference_pipeline.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,11 +22,12 @@
             punc_model='damo/punc_ct-transformer_zh-cn-common-vocab272727-pytorch',
             punc_model_revision="v1.1.6",
             ngpu=1,
         )
         rec_result = inference_pipeline(
             audio_in='https://isv-data.oss-cn-hangzhou.aliyuncs.com/ics/MaaS/ASR/test_audio/asr_example_zh.wav')
         logger.info("asr_vad_punc inference result: {0}".format(rec_result))
+        assert rec_result["text"] == "欢迎大家来体验达摩院推出的语音识别模型。"
 
 
 if __name__ == '__main__':
     unittest.main()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `funasr-0.6.1/tests/test_lm_pipeline.py` & `funasr-0.6.2/tests/test_lm_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/tests/test_punctuation_pipeline.py` & `funasr-0.6.2/tests/test_punctuation_pipeline.py`

 * *Files identical despite different names*

### Comparing `funasr-0.6.1/tests/test_vad_inference_pipeline.py` & `funasr-0.6.2/tests/test_vad_inference_pipeline.py`

 * *Files identical despite different names*

