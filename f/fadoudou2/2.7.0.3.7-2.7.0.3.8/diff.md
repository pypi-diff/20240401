# Comparing `tmp/fadoudou2-2.7.0.3.7.tar.gz` & `tmp/fadoudou2-2.7.0.3.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fadoudou2-2.7.0.3.7.tar", last modified: Wed Mar 27 06:28:17 2024, max compression
+gzip compressed data, was "fadoudou2-2.7.0.3.8.tar", last modified: Mon Apr  1 09:38:27 2024, max compression
```

## Comparing `fadoudou2-2.7.0.3.7.tar` & `fadoudou2-2.7.0.3.8.tar`

### file list

```diff
@@ -1,229 +1,229 @@
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.992903 fadoudou2-2.7.0.3.7/
--rw-rw-rw-   0        0        0    11641 2023-12-20 10:07:38.000000 fadoudou2-2.7.0.3.7/LICENSE
--rw-rw-rw-   0        0        0      303 2023-12-20 10:07:38.000000 fadoudou2-2.7.0.3.7/MANIFEST.in
--rw-rw-rw-   0        0        0    27414 2024-03-27 06:28:17.991903 fadoudou2-2.7.0.3.7/PKG-INFO
--rw-rw-rw-   0        0        0    20341 2023-12-26 16:06:52.000000 fadoudou2-2.7.0.3.7/README.md
--rw-rw-rw-   0        0        0      886 2023-12-20 10:07:38.000000 fadoudou2-2.7.0.3.7/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.888384 fadoudou2-2.7.0.3.7/fadoudou2.egg-info/
--rw-rw-rw-   0        0        0    27414 2024-03-27 06:28:17.000000 fadoudou2-2.7.0.3.7/fadoudou2.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     6835 2024-03-27 06:28:17.000000 fadoudou2-2.7.0.3.7/fadoudou2.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-27 06:28:17.000000 fadoudou2-2.7.0.3.7/fadoudou2.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       55 2024-03-27 06:28:17.000000 fadoudou2-2.7.0.3.7/fadoudou2.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      271 2024-03-27 06:28:17.000000 fadoudou2-2.7.0.3.7/fadoudou2.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2024-03-27 06:28:17.000000 fadoudou2-2.7.0.3.7/fadoudou2.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    37494 2024-03-27 06:28:12.000000 fadoudou2-2.7.0.3.7/paddleocr.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.869385 fadoudou2-2.7.0.3.7/ppocr/
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.892390 fadoudou2-2.7.0.3.7/ppocr/data/
--rw-rw-rw-   0        0        0     5319 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/data/__init__.py
--rw-rw-rw-   0        0        0     4052 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/collate_fn.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.904897 fadoudou2-2.7.0.3.7/ppocr/data/imaug/
--rw-rw-rw-   0        0        0     1053 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/ColorJitter.py
--rw-rw-rw-   0        0        0     2732 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/__init__.py
--rw-rw-rw-   0        0        0    16796 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/abinet_aug.py
--rw-rw-rw-   0        0        0     6805 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/copy_paste.py
--rw-rw-rw-   0        0        0    12056 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/ct_process.py
--rw-rw-rw-   0        0        0    30081 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/drrg_targets.py
--rw-rw-rw-   0        0        0    17677 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/east_process.py
--rw-rw-rw-   0        0        0    21486 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/fce_aug.py
--rw-rw-rw-   0        0        0    27258 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/fce_targets.py
--rw-rw-rw-   0        0        0     3529 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/iaa_augment.py
--rw-rw-rw-   0        0        0    56312 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/label_ops.py
--rw-rw-rw-   0        0        0     6824 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/make_border_map.py
--rw-rw-rw-   0        0        0     4008 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/make_pse_gt.py
--rw-rw-rw-   0        0        0     4970 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/make_shrink_map.py
--rw-rw-rw-   0        0        0    18017 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/operators.py
--rw-rw-rw-   0        0        0    42337 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/pg_process.py
--rw-rw-rw-   0        0        0     5591 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/randaugment.py
--rw-rw-rw-   0        0        0     8070 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/random_crop_data.py
--rw-rw-rw-   0        0        0    27968 2024-03-01 06:11:06.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/rec_img_aug.py
--rw-rw-rw-   0        0        0    30175 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/sast_process.py
--rw-rw-rw-   0        0        0     2217 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/ssl_img_aug.py
--rw-rw-rw-   0        0        0     9005 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/table_ops.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.905898 fadoudou2-2.7.0.3.7/ppocr/data/imaug/text_image_aug/
--rw-rw-rw-   0        0        0      750 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/text_image_aug/__init__.py
--rw-rw-rw-   0        0        0     3557 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/text_image_aug/augment.py
--rw-rw-rw-   0        0        0     6621 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/text_image_aug/warp_mls.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.906898 fadoudou2-2.7.0.3.7/ppocr/data/imaug/vqa/
--rw-rw-rw-   0        0        0      871 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/vqa/__init__.py
--rw-rw-rw-   0        0        0     1213 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/vqa/augment.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.909898 fadoudou2-2.7.0.3.7/ppocr/data/imaug/vqa/token/
--rw-rw-rw-   0        0        0      833 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/vqa/token/__init__.py
--rw-rw-rw-   0        0        0     2066 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/vqa/token/vqa_re_convert.py
--rw-rw-rw-   0        0        0     5130 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/vqa/token/vqa_token_chunk.py
--rw-rw-rw-   0        0        0     4863 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/vqa/token/vqa_token_pad.py
--rw-rw-rw-   0        0        0     2529 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/imaug/vqa/token/vqa_token_relation.py
--rw-rw-rw-   0        0        0    10793 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/data/lmdb_dataset.py
--rw-rw-rw-   0        0        0     6948 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/data/multi_scale_sampler.py
--rw-rw-rw-   0        0        0     4300 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/pgnet_dataset.py
--rw-rw-rw-   0        0        0     5234 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/data/pubtab_dataset.py
--rw-rw-rw-   0        0        0    11073 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/data/simple_dataset.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.918899 fadoudou2-2.7.0.3.7/ppocr/postprocess/
--rw-rw-rw-   0        0        0     3321 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/postprocess/__init__.py
--rw-rw-rw-   0        0        0     1570 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/postprocess/cls_postprocess.py
--rw-rw-rw-   0        0        0     5517 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/postprocess/ct_postprocess.py
--rw-rw-rw-   0        0        0    10175 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/postprocess/db_postprocess.py
--rw-rw-rw-   0        0        0    11893 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/postprocess/drrg_postprocess.py
--rw-rw-rw-   0        0        0     5335 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/postprocess/east_postprocess.py
--rw-rw-rw-   0        0        0     8888 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/postprocess/fce_postprocess.py
--rw-rw-rw-   0        0        0     5233 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/postprocess/locality_aware_nms.py
--rw-rw-rw-   0        0        0     2118 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/postprocess/pg_postprocess.py
--rw-rw-rw-   0        0        0    10024 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/postprocess/picodet_postprocess.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.919899 fadoudou2-2.7.0.3.7/ppocr/postprocess/pse_postprocess/
--rw-rw-rw-   0        0        0      668 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/postprocess/pse_postprocess/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.920898 fadoudou2-2.7.0.3.7/ppocr/postprocess/pse_postprocess/pse/
--rw-rw-rw-   0        0        0     1174 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/postprocess/pse_postprocess/pse/__init__.py
--rw-rw-rw-   0        0        0      340 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/postprocess/pse_postprocess/pse/setup.py
--rw-rw-rw-   0        0        0     4228 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/postprocess/pse_postprocess/pse_postprocess.py
--rw-rw-rw-   0        0        0    39934 2024-03-26 10:17:50.000000 fadoudou2-2.7.0.3.7/ppocr/postprocess/rec_postprocess.py
--rw-rw-rw-   0        0        0    14125 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/postprocess/sast_postprocess.py
--rw-rw-rw-   0        0        0     7015 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/postprocess/table_postprocess.py
--rw-rw-rw-   0        0        0     3862 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/postprocess/vqa_token_re_layoutlm_postprocess.py
--rw-rw-rw-   0        0        0     4682 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/postprocess/vqa_token_ser_layoutlm_postprocess.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.928897 fadoudou2-2.7.0.3.7/ppocr/utils/
--rw-rw-rw-   0        0        0      280 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/EN_symbol_dict.txt
--rw-rw-rw-   0        0        0      623 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.934899 fadoudou2-2.7.0.3.7/ppocr/utils/__pycache__/
--rw-rw-rw-   0        0        0      161 2023-12-26 10:07:15.000000 fadoudou2-2.7.0.3.7/ppocr/utils/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0     2027 2023-12-26 10:08:35.000000 fadoudou2-2.7.0.3.7/ppocr/utils/__pycache__/logging.cpython-310.pyc
--rw-rw-rw-   0        0        0     2700 2023-12-27 02:31:38.000000 fadoudou2-2.7.0.3.7/ppocr/utils/__pycache__/network.cpython-310.pyc
--rw-rw-rw-   0        0        0     3656 2023-12-26 10:08:40.000000 fadoudou2-2.7.0.3.7/ppocr/utils/__pycache__/poly_nms.cpython-310.pyc
--rw-rw-rw-   0        0        0     3552 2024-02-04 03:38:11.000000 fadoudou2-2.7.0.3.7/ppocr/utils/__pycache__/profiler.cpython-310.pyc
--rw-rw-rw-   0        0        0     5035 2024-02-04 03:38:10.000000 fadoudou2-2.7.0.3.7/ppocr/utils/__pycache__/save_load.cpython-310.pyc
--rw-rw-rw-   0        0        0     2445 2024-02-04 03:38:11.000000 fadoudou2-2.7.0.3.7/ppocr/utils/__pycache__/stats.cpython-310.pyc
--rw-rw-rw-   0        0        0     6406 2023-12-26 16:07:23.000000 fadoudou2-2.7.0.3.7/ppocr/utils/__pycache__/utility.cpython-310.pyc
--rw-rw-rw-   0        0        0     3650 2023-12-26 16:07:25.000000 fadoudou2-2.7.0.3.7/ppocr/utils/__pycache__/visual.cpython-310.pyc
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.935899 fadoudou2-2.7.0.3.7/ppocr/utils/corpus/
--rw-rw-rw-   0        0        0  1381583 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/utils/corpus/fi_corpus.txt
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.956899 fadoudou2-2.7.0.3.7/ppocr/utils/dict/
--rw-rw-rw-   0        0        0      390 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/ar_dict.txt
--rw-rw-rw-   0        0        0      566 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/arabic_dict.txt
--rw-rw-rw-   0        0        0      502 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/be_dict.txt
--rw-rw-rw-   0        0        0      481 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/bg_dict.txt
--rw-rw-rw-   0        0        0    41864 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/chinese_cht_dict.txt
--rw-rw-rw-   0        0        0    30912 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/confuse.pkl
--rw-rw-rw-   0        0        0      573 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/cyrillic_dict.txt
--rw-rw-rw-   0        0        0      675 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/devanagari_dict.txt
--rw-rw-rw-   0        0        0      189 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/en_dict.txt
--rw-rw-rw-   0        0        0      466 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/fa_dict.txt
--rw-rw-rw-   0        0        0      244 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/fi_dict.txt
--rw-rw-rw-   0        0        0      460 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/french_dict.txt
--rw-rw-rw-   0        0        0      489 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/german_dict.txt
--rw-rw-rw-   0        0        0      650 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/hi_dict.txt
--rw-rw-rw-   0        0        0      384 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/it_dict.txt
--rw-rw-rw-   0        0        0    21731 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/japan_dict.txt
--rw-rw-rw-   0        0        0      605 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/ka_dict.txt
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.957899 fadoudou2-2.7.0.3.7/ppocr/utils/dict/kie_dict/
--rw-rw-rw-   0        0        0       33 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/kie_dict/xfund_class_list.txt
--rw-rw-rw-   0        0        0    18168 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/korean_dict.txt
--rw-rw-rw-   0        0        0      475 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/latex_symbol_dict.txt
--rw-rw-rw-   0        0        0      653 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/latin_dict.txt
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.958897 fadoudou2-2.7.0.3.7/ppocr/utils/dict/layout_dict/
--rw-rw-rw-   0        0        0       94 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/layout_dict/layout_cdla_dict.txt
--rw-rw-rw-   0        0        0       32 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/layout_dict/layout_publaynet_dict.txt
--rw-rw-rw-   0        0        0        5 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/layout_dict/layout_table_dict.txt
--rw-rw-rw-   0        0        0      605 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/mr_dict.txt
--rw-rw-rw-   0        0        0      605 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/ne_dict.txt
--rw-rw-rw-   0        0        0      306 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/oc_dict.txt
--rw-rw-rw-   0        0        0      435 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/pu_dict.txt
--rw-rw-rw-   0        0        0      285 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/rs_dict.txt
--rw-rw-rw-   0        0        0      458 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/rsc_dict.txt
--rw-rw-rw-   0        0        0      438 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/ru_dict.txt
--rw-rw-rw-   0        0        0      202 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/spin_dict.txt
--rw-rw-rw-   0        0        0      480 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/ta_dict.txt
--rw-rw-rw-   0        0        0     1171 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/table_dict.txt
--rw-rw-rw-   0        0        0      474 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/table_master_structure_dict.txt
--rw-rw-rw-   0        0        0      324 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/table_structure_dict.txt
--rw-rw-rw-   0        0        0      626 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/table_structure_dict_ch.txt
--rw-rw-rw-   0        0        0      580 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/te_dict.txt
--rw-rw-rw-   0        0        0      377 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/ug_dict.txt
--rw-rw-rw-   0        0        0      490 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/uk_dict.txt
--rw-rw-rw-   0        0        0      469 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/ur_dict.txt
--rw-rw-rw-   0        0        0      360 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict/xi_dict.txt
--rw-rw-rw-   0        0        0      268 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/dict90.txt
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.959899 fadoudou2-2.7.0.3.7/ppocr/utils/e2e_metric/
--rw-rw-rw-   0        0        0    31477 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/utils/e2e_metric/Deteval.py
--rw-rw-rw-   0        0        0     2925 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/e2e_metric/polygon_fast.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.962898 fadoudou2-2.7.0.3.7/ppocr/utils/e2e_utils/
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.964898 fadoudou2-2.7.0.3.7/ppocr/utils/e2e_utils/__pycache__/
--rw-rw-rw-   0        0        0    12926 2023-12-26 10:09:26.000000 fadoudou2-2.7.0.3.7/ppocr/utils/e2e_utils/__pycache__/extract_textpoint_fast.cpython-310.pyc
--rw-rw-rw-   0        0        0    13650 2023-12-26 10:09:06.000000 fadoudou2-2.7.0.3.7/ppocr/utils/e2e_utils/__pycache__/extract_textpoint_slow.cpython-310.pyc
--rw-rw-rw-   0        0        0     3953 2023-12-26 10:09:06.000000 fadoudou2-2.7.0.3.7/ppocr/utils/e2e_utils/__pycache__/pgnet_pp_utils.cpython-310.pyc
--rw-rw-rw-   0        0        0     3373 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/e2e_utils/extract_batchsize.py
--rw-rw-rw-   0        0        0    19283 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/e2e_utils/extract_textpoint_fast.py
--rw-rw-rw-   0        0        0    22815 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/e2e_utils/extract_textpoint_slow.py
--rw-rw-rw-   0        0        0     6734 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/e2e_utils/pgnet_pp_utils.py
--rw-rw-rw-   0        0        0     5420 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/e2e_utils/visual.py
--rw-rw-rw-   0        0        0      285 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/en_dict.txt
--rw-rw-rw-   0        0        0     3067 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/utils/gen_label.py
--rw-rw-rw-   0        0        0      106 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/ic15_dict.txt
--rw-rw-rw-   0        0        0     1754 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/iou.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.967898 fadoudou2-2.7.0.3.7/ppocr/utils/loggers/
--rw-rw-rw-   0        0        0      104 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/loggers/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.971899 fadoudou2-2.7.0.3.7/ppocr/utils/loggers/__pycache__/
--rw-rw-rw-   0        0        0      300 2024-02-04 03:38:11.000000 fadoudou2-2.7.0.3.7/ppocr/utils/loggers/__pycache__/__init__.cpython-310.pyc
--rw-rw-rw-   0        0        0      866 2024-02-04 03:38:11.000000 fadoudou2-2.7.0.3.7/ppocr/utils/loggers/__pycache__/base_logger.cpython-310.pyc
--rw-rw-rw-   0        0        0     1107 2024-02-04 03:38:11.000000 fadoudou2-2.7.0.3.7/ppocr/utils/loggers/__pycache__/loggers.cpython-310.pyc
--rw-rw-rw-   0        0        0     1376 2024-02-04 03:38:11.000000 fadoudou2-2.7.0.3.7/ppocr/utils/loggers/__pycache__/vdl_logger.cpython-310.pyc
--rw-rw-rw-   0        0        0     2509 2024-02-04 03:38:11.000000 fadoudou2-2.7.0.3.7/ppocr/utils/loggers/__pycache__/wandb_logger.cpython-310.pyc
--rw-rw-rw-   0        0        0      338 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/loggers/base_logger.py
--rw-rw-rw-   0        0        0      599 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/loggers/loggers.py
--rw-rw-rw-   0        0        0      653 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/loggers/vdl_logger.py
--rw-rw-rw-   0        0        0     2452 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/loggers/wandb_logger.py
--rw-rw-rw-   0        0        0     2757 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/logging.py
--rw-rw-rw-   0        0        0     3680 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/utils/network.py
--rw-rw-rw-   0        0        0     4283 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/poly_nms.py
--rw-rw-rw-   0        0        0    32871 2024-03-01 07:07:48.000000 fadoudou2-2.7.0.3.7/ppocr/utils/ppocr_keys_v1.txt
--rw-rw-rw-   0        0        0     5388 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/utils/profiler.py
--rw-rw-rw-   0        0        0     9373 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/utils/save_load.py
--rw-rw-rw-   0        0        0     2304 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppocr/utils/stats.py
--rw-rw-rw-   0        0        0     6984 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/utils/utility.py
--rw-rw-rw-   0        0        0     4551 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppocr/utils/visual.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.973899 fadoudou2-2.7.0.3.7/ppstructure/
--rw-rw-rw-   0        0        0      621 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppstructure/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.974898 fadoudou2-2.7.0.3.7/ppstructure/kie/
--rw-rw-rw-   0        0        0     6004 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppstructure/kie/predict_kie_token_ser.py
--rw-rw-rw-   0        0        0     5014 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppstructure/kie/predict_kie_token_ser_re.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.975899 fadoudou2-2.7.0.3.7/ppstructure/kie/tools/
--rw-rw-rw-   0        0        0     8518 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppstructure/kie/tools/eval_with_label_end2end.py
--rw-rw-rw-   0        0        0     6202 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppstructure/kie/tools/trans_funsd_label.py
--rw-rw-rw-   0        0        0     2161 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppstructure/kie/tools/trans_xfun_data.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.976899 fadoudou2-2.7.0.3.7/ppstructure/layout/
--rw-rw-rw-   0        0        0      621 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppstructure/layout/__init__.py
--rw-rw-rw-   0        0        0     4285 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppstructure/layout/predict_layout.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.977898 fadoudou2-2.7.0.3.7/ppstructure/pdf2word/
--rw-rw-rw-   0        0        0    21178 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppstructure/pdf2word/pdf2word.py
--rw-rw-rw-   0        0        0    14074 2024-01-18 10:40:29.000000 fadoudou2-2.7.0.3.7/ppstructure/predict_system.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.978898 fadoudou2-2.7.0.3.7/ppstructure/recovery/
--rw-rw-rw-   0        0        0      621 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppstructure/recovery/__init__.py
--rw-rw-rw-   0        0        0     5537 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppstructure/recovery/recovery_to_doc.py
--rw-rw-rw-   0        0        0    11710 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppstructure/recovery/table_process.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.982898 fadoudou2-2.7.0.3.7/ppstructure/table/
--rw-rw-rw-   0        0        0      621 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppstructure/table/__init__.py
--rw-rw-rw-   0        0        0     3145 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppstructure/table/convert_label2html.py
--rw-rw-rw-   0        0        0     3581 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppstructure/table/eval_table.py
--rw-rw-rw-   0        0        0     8164 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppstructure/table/matcher.py
--rw-rw-rw-   0        0        0     7686 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppstructure/table/predict_structure.py
--rw-rw-rw-   0        0        0     8752 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.7/ppstructure/table/predict_table.py
--rw-rw-rw-   0        0        0    37580 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppstructure/table/table_master_match.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.984898 fadoudou2-2.7.0.3.7/ppstructure/table/table_metric/
--rw-rw-rw-   0        0        0      673 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppstructure/table/table_metric/__init__.py
--rw-rw-rw-   0        0        0     2198 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppstructure/table/table_metric/parallel.py
--rw-rw-rw-   0        0        0     8599 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppstructure/table/table_metric/table_metric.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.986900 fadoudou2-2.7.0.3.7/ppstructure/table/tablepyxl/
--rw-rw-rw-   0        0        0      619 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppstructure/table/tablepyxl/__init__.py
--rw-rw-rw-   0        0        0    10415 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppstructure/table/tablepyxl/style.py
--rw-rw-rw-   0        0        0     4217 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/ppstructure/table/tablepyxl/tablepyxl.py
--rw-rw-rw-   0        0        0    10495 2024-02-01 05:58:22.000000 fadoudou2-2.7.0.3.7/ppstructure/utility.py
--rw-rw-rw-   0        0        0       42 2024-03-27 06:28:17.992903 fadoudou2-2.7.0.3.7/setup.cfg
--rw-rw-rw-   0        0        0     2663 2024-02-01 08:24:19.000000 fadoudou2-2.7.0.3.7/setup.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.986900 fadoudou2-2.7.0.3.7/tools/
--rw-rw-rw-   0        0        0      708 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/tools/__init__.py
-drwxrwxrwx   0        0        0        0 2024-03-27 06:28:17.991903 fadoudou2-2.7.0.3.7/tools/infer/
--rw-rw-rw-   0        0        0    69313 2023-12-27 09:24:55.000000 fadoudou2-2.7.0.3.7/tools/infer/diff_match_patch.py
--rw-rw-rw-   0        0        0     5891 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/tools/infer/predict_cls.py
--rw-rw-rw-   0        0        0    14487 2024-03-26 08:51:22.000000 fadoudou2-2.7.0.3.7/tools/infer/predict_det.py
--rw-rw-rw-   0        0        0     6458 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/tools/infer/predict_e2e.py
--rw-rw-rw-   0        0        0    29985 2024-03-26 10:18:25.000000 fadoudou2-2.7.0.3.7/tools/infer/predict_rec.py
--rw-rw-rw-   0        0        0     5813 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.7/tools/infer/predict_sr.py
--rw-rw-rw-   0        0        0    12170 2024-03-01 06:07:23.000000 fadoudou2-2.7.0.3.7/tools/infer/predict_system.py
--rw-rw-rw-   0        0        0    26113 2024-03-01 06:26:55.000000 fadoudou2-2.7.0.3.7/tools/infer/utility.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.845539 fadoudou2-2.7.0.3.8/
+-rw-rw-rw-   0        0        0    11641 2023-12-20 10:07:38.000000 fadoudou2-2.7.0.3.8/LICENSE
+-rw-rw-rw-   0        0        0      303 2023-12-20 10:07:38.000000 fadoudou2-2.7.0.3.8/MANIFEST.in
+-rw-rw-rw-   0        0        0    27414 2024-04-01 09:38:27.844538 fadoudou2-2.7.0.3.8/PKG-INFO
+-rw-rw-rw-   0        0        0    20341 2023-12-26 16:06:52.000000 fadoudou2-2.7.0.3.8/README.md
+-rw-rw-rw-   0        0        0      886 2023-12-20 10:07:38.000000 fadoudou2-2.7.0.3.8/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.177737 fadoudou2-2.7.0.3.8/fadoudou2.egg-info/
+-rw-rw-rw-   0        0        0    27414 2024-04-01 09:38:27.000000 fadoudou2-2.7.0.3.8/fadoudou2.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     6835 2024-04-01 09:38:27.000000 fadoudou2-2.7.0.3.8/fadoudou2.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-01 09:38:27.000000 fadoudou2-2.7.0.3.8/fadoudou2.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       55 2024-04-01 09:38:27.000000 fadoudou2-2.7.0.3.8/fadoudou2.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      271 2024-04-01 09:38:27.000000 fadoudou2-2.7.0.3.8/fadoudou2.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2024-04-01 09:38:27.000000 fadoudou2-2.7.0.3.8/fadoudou2.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    37494 2024-04-01 09:38:13.000000 fadoudou2-2.7.0.3.8/paddleocr.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.141219 fadoudou2-2.7.0.3.8/ppocr/
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.207736 fadoudou2-2.7.0.3.8/ppocr/data/
+-rw-rw-rw-   0        0        0     5319 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/data/__init__.py
+-rw-rw-rw-   0        0        0     4052 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/collate_fn.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.310244 fadoudou2-2.7.0.3.8/ppocr/data/imaug/
+-rw-rw-rw-   0        0        0     1053 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/ColorJitter.py
+-rw-rw-rw-   0        0        0     2732 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/__init__.py
+-rw-rw-rw-   0        0        0    16796 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/abinet_aug.py
+-rw-rw-rw-   0        0        0     6805 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/copy_paste.py
+-rw-rw-rw-   0        0        0    12056 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/ct_process.py
+-rw-rw-rw-   0        0        0    30081 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/drrg_targets.py
+-rw-rw-rw-   0        0        0    17677 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/east_process.py
+-rw-rw-rw-   0        0        0    21486 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/fce_aug.py
+-rw-rw-rw-   0        0        0    27258 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/fce_targets.py
+-rw-rw-rw-   0        0        0     3529 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/iaa_augment.py
+-rw-rw-rw-   0        0        0    56312 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/label_ops.py
+-rw-rw-rw-   0        0        0     6824 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/make_border_map.py
+-rw-rw-rw-   0        0        0     4008 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/make_pse_gt.py
+-rw-rw-rw-   0        0        0     4970 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/make_shrink_map.py
+-rw-rw-rw-   0        0        0    18017 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/operators.py
+-rw-rw-rw-   0        0        0    42337 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/pg_process.py
+-rw-rw-rw-   0        0        0     5591 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/randaugment.py
+-rw-rw-rw-   0        0        0     8070 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/random_crop_data.py
+-rw-rw-rw-   0        0        0    27968 2024-03-01 06:11:06.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/rec_img_aug.py
+-rw-rw-rw-   0        0        0    30175 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/sast_process.py
+-rw-rw-rw-   0        0        0     2217 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/ssl_img_aug.py
+-rw-rw-rw-   0        0        0     9005 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/table_ops.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.322247 fadoudou2-2.7.0.3.8/ppocr/data/imaug/text_image_aug/
+-rw-rw-rw-   0        0        0      750 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/text_image_aug/__init__.py
+-rw-rw-rw-   0        0        0     3557 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/text_image_aug/augment.py
+-rw-rw-rw-   0        0        0     6621 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/text_image_aug/warp_mls.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.330248 fadoudou2-2.7.0.3.8/ppocr/data/imaug/vqa/
+-rw-rw-rw-   0        0        0      871 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/vqa/__init__.py
+-rw-rw-rw-   0        0        0     1213 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/vqa/augment.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.348835 fadoudou2-2.7.0.3.8/ppocr/data/imaug/vqa/token/
+-rw-rw-rw-   0        0        0      833 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/vqa/token/__init__.py
+-rw-rw-rw-   0        0        0     2066 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/vqa/token/vqa_re_convert.py
+-rw-rw-rw-   0        0        0     5130 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/vqa/token/vqa_token_chunk.py
+-rw-rw-rw-   0        0        0     4863 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/vqa/token/vqa_token_pad.py
+-rw-rw-rw-   0        0        0     2529 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/imaug/vqa/token/vqa_token_relation.py
+-rw-rw-rw-   0        0        0    10793 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/data/lmdb_dataset.py
+-rw-rw-rw-   0        0        0     6948 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/data/multi_scale_sampler.py
+-rw-rw-rw-   0        0        0     4300 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/pgnet_dataset.py
+-rw-rw-rw-   0        0        0     5234 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/data/pubtab_dataset.py
+-rw-rw-rw-   0        0        0    11073 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/data/simple_dataset.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.411350 fadoudou2-2.7.0.3.8/ppocr/postprocess/
+-rw-rw-rw-   0        0        0     3321 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/postprocess/__init__.py
+-rw-rw-rw-   0        0        0     1570 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/postprocess/cls_postprocess.py
+-rw-rw-rw-   0        0        0     5517 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/postprocess/ct_postprocess.py
+-rw-rw-rw-   0        0        0    10175 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/postprocess/db_postprocess.py
+-rw-rw-rw-   0        0        0    11893 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/postprocess/drrg_postprocess.py
+-rw-rw-rw-   0        0        0     5335 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/postprocess/east_postprocess.py
+-rw-rw-rw-   0        0        0     8888 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/postprocess/fce_postprocess.py
+-rw-rw-rw-   0        0        0     5233 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/postprocess/locality_aware_nms.py
+-rw-rw-rw-   0        0        0     2118 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/postprocess/pg_postprocess.py
+-rw-rw-rw-   0        0        0    10024 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/postprocess/picodet_postprocess.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.418347 fadoudou2-2.7.0.3.8/ppocr/postprocess/pse_postprocess/
+-rw-rw-rw-   0        0        0      668 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/postprocess/pse_postprocess/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.427350 fadoudou2-2.7.0.3.8/ppocr/postprocess/pse_postprocess/pse/
+-rw-rw-rw-   0        0        0     1174 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/postprocess/pse_postprocess/pse/__init__.py
+-rw-rw-rw-   0        0        0      340 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/postprocess/pse_postprocess/pse/setup.py
+-rw-rw-rw-   0        0        0     4228 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/postprocess/pse_postprocess/pse_postprocess.py
+-rw-rw-rw-   0        0        0    39934 2024-03-26 10:17:50.000000 fadoudou2-2.7.0.3.8/ppocr/postprocess/rec_postprocess.py
+-rw-rw-rw-   0        0        0    14125 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/postprocess/sast_postprocess.py
+-rw-rw-rw-   0        0        0     7015 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/postprocess/table_postprocess.py
+-rw-rw-rw-   0        0        0     3862 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/postprocess/vqa_token_re_layoutlm_postprocess.py
+-rw-rw-rw-   0        0        0     4682 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/postprocess/vqa_token_ser_layoutlm_postprocess.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.486858 fadoudou2-2.7.0.3.8/ppocr/utils/
+-rw-rw-rw-   0        0        0      280 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/EN_symbol_dict.txt
+-rw-rw-rw-   0        0        0      623 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.493860 fadoudou2-2.7.0.3.8/ppocr/utils/__pycache__/
+-rw-rw-rw-   0        0        0      161 2023-12-26 10:07:15.000000 fadoudou2-2.7.0.3.8/ppocr/utils/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2027 2023-12-26 10:08:35.000000 fadoudou2-2.7.0.3.8/ppocr/utils/__pycache__/logging.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2700 2023-12-27 02:31:38.000000 fadoudou2-2.7.0.3.8/ppocr/utils/__pycache__/network.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3656 2023-12-26 10:08:40.000000 fadoudou2-2.7.0.3.8/ppocr/utils/__pycache__/poly_nms.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3552 2024-02-04 03:38:11.000000 fadoudou2-2.7.0.3.8/ppocr/utils/__pycache__/profiler.cpython-310.pyc
+-rw-rw-rw-   0        0        0     5035 2024-02-04 03:38:10.000000 fadoudou2-2.7.0.3.8/ppocr/utils/__pycache__/save_load.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2445 2024-02-04 03:38:11.000000 fadoudou2-2.7.0.3.8/ppocr/utils/__pycache__/stats.cpython-310.pyc
+-rw-rw-rw-   0        0        0     6406 2023-12-26 16:07:23.000000 fadoudou2-2.7.0.3.8/ppocr/utils/__pycache__/utility.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3650 2023-12-26 16:07:25.000000 fadoudou2-2.7.0.3.8/ppocr/utils/__pycache__/visual.cpython-310.pyc
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.498862 fadoudou2-2.7.0.3.8/ppocr/utils/corpus/
+-rw-rw-rw-   0        0        0  1381583 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/utils/corpus/fi_corpus.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.644374 fadoudou2-2.7.0.3.8/ppocr/utils/dict/
+-rw-rw-rw-   0        0        0      390 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/ar_dict.txt
+-rw-rw-rw-   0        0        0      566 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/arabic_dict.txt
+-rw-rw-rw-   0        0        0      502 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/be_dict.txt
+-rw-rw-rw-   0        0        0      481 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/bg_dict.txt
+-rw-rw-rw-   0        0        0    41864 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/chinese_cht_dict.txt
+-rw-rw-rw-   0        0        0    30912 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/confuse.pkl
+-rw-rw-rw-   0        0        0      573 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/cyrillic_dict.txt
+-rw-rw-rw-   0        0        0      675 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/devanagari_dict.txt
+-rw-rw-rw-   0        0        0      189 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/en_dict.txt
+-rw-rw-rw-   0        0        0      466 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/fa_dict.txt
+-rw-rw-rw-   0        0        0      244 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/fi_dict.txt
+-rw-rw-rw-   0        0        0      460 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/french_dict.txt
+-rw-rw-rw-   0        0        0      489 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/german_dict.txt
+-rw-rw-rw-   0        0        0      650 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/hi_dict.txt
+-rw-rw-rw-   0        0        0      384 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/it_dict.txt
+-rw-rw-rw-   0        0        0    21731 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/japan_dict.txt
+-rw-rw-rw-   0        0        0      605 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/ka_dict.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.647374 fadoudou2-2.7.0.3.8/ppocr/utils/dict/kie_dict/
+-rw-rw-rw-   0        0        0       33 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/kie_dict/xfund_class_list.txt
+-rw-rw-rw-   0        0        0    18168 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/korean_dict.txt
+-rw-rw-rw-   0        0        0      475 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/latex_symbol_dict.txt
+-rw-rw-rw-   0        0        0      653 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/latin_dict.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.655370 fadoudou2-2.7.0.3.8/ppocr/utils/dict/layout_dict/
+-rw-rw-rw-   0        0        0       94 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/layout_dict/layout_cdla_dict.txt
+-rw-rw-rw-   0        0        0       32 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/layout_dict/layout_publaynet_dict.txt
+-rw-rw-rw-   0        0        0        5 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/layout_dict/layout_table_dict.txt
+-rw-rw-rw-   0        0        0      605 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/mr_dict.txt
+-rw-rw-rw-   0        0        0      605 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/ne_dict.txt
+-rw-rw-rw-   0        0        0      306 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/oc_dict.txt
+-rw-rw-rw-   0        0        0      435 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/pu_dict.txt
+-rw-rw-rw-   0        0        0      285 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/rs_dict.txt
+-rw-rw-rw-   0        0        0      458 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/rsc_dict.txt
+-rw-rw-rw-   0        0        0      438 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/ru_dict.txt
+-rw-rw-rw-   0        0        0      202 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/spin_dict.txt
+-rw-rw-rw-   0        0        0      480 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/ta_dict.txt
+-rw-rw-rw-   0        0        0     1171 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/table_dict.txt
+-rw-rw-rw-   0        0        0      474 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/table_master_structure_dict.txt
+-rw-rw-rw-   0        0        0      324 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/table_structure_dict.txt
+-rw-rw-rw-   0        0        0      626 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/table_structure_dict_ch.txt
+-rw-rw-rw-   0        0        0      580 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/te_dict.txt
+-rw-rw-rw-   0        0        0      377 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/ug_dict.txt
+-rw-rw-rw-   0        0        0      490 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/uk_dict.txt
+-rw-rw-rw-   0        0        0      469 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/ur_dict.txt
+-rw-rw-rw-   0        0        0      360 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict/xi_dict.txt
+-rw-rw-rw-   0        0        0      268 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/dict90.txt
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.665377 fadoudou2-2.7.0.3.8/ppocr/utils/e2e_metric/
+-rw-rw-rw-   0        0        0    31477 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/utils/e2e_metric/Deteval.py
+-rw-rw-rw-   0        0        0     2925 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/e2e_metric/polygon_fast.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.684887 fadoudou2-2.7.0.3.8/ppocr/utils/e2e_utils/
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.687888 fadoudou2-2.7.0.3.8/ppocr/utils/e2e_utils/__pycache__/
+-rw-rw-rw-   0        0        0    12926 2023-12-26 10:09:26.000000 fadoudou2-2.7.0.3.8/ppocr/utils/e2e_utils/__pycache__/extract_textpoint_fast.cpython-310.pyc
+-rw-rw-rw-   0        0        0    13650 2023-12-26 10:09:06.000000 fadoudou2-2.7.0.3.8/ppocr/utils/e2e_utils/__pycache__/extract_textpoint_slow.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3953 2023-12-26 10:09:06.000000 fadoudou2-2.7.0.3.8/ppocr/utils/e2e_utils/__pycache__/pgnet_pp_utils.cpython-310.pyc
+-rw-rw-rw-   0        0        0     3373 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/e2e_utils/extract_batchsize.py
+-rw-rw-rw-   0        0        0    19283 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/e2e_utils/extract_textpoint_fast.py
+-rw-rw-rw-   0        0        0    22815 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/e2e_utils/extract_textpoint_slow.py
+-rw-rw-rw-   0        0        0     6734 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/e2e_utils/pgnet_pp_utils.py
+-rw-rw-rw-   0        0        0     5420 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/e2e_utils/visual.py
+-rw-rw-rw-   0        0        0      285 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/en_dict.txt
+-rw-rw-rw-   0        0        0     3067 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/utils/gen_label.py
+-rw-rw-rw-   0        0        0      106 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/ic15_dict.txt
+-rw-rw-rw-   0        0        0     1754 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/iou.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.703892 fadoudou2-2.7.0.3.8/ppocr/utils/loggers/
+-rw-rw-rw-   0        0        0      104 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/loggers/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.706888 fadoudou2-2.7.0.3.8/ppocr/utils/loggers/__pycache__/
+-rw-rw-rw-   0        0        0      300 2024-02-04 03:38:11.000000 fadoudou2-2.7.0.3.8/ppocr/utils/loggers/__pycache__/__init__.cpython-310.pyc
+-rw-rw-rw-   0        0        0      866 2024-02-04 03:38:11.000000 fadoudou2-2.7.0.3.8/ppocr/utils/loggers/__pycache__/base_logger.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1107 2024-02-04 03:38:11.000000 fadoudou2-2.7.0.3.8/ppocr/utils/loggers/__pycache__/loggers.cpython-310.pyc
+-rw-rw-rw-   0        0        0     1376 2024-02-04 03:38:11.000000 fadoudou2-2.7.0.3.8/ppocr/utils/loggers/__pycache__/vdl_logger.cpython-310.pyc
+-rw-rw-rw-   0        0        0     2509 2024-02-04 03:38:11.000000 fadoudou2-2.7.0.3.8/ppocr/utils/loggers/__pycache__/wandb_logger.cpython-310.pyc
+-rw-rw-rw-   0        0        0      338 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/loggers/base_logger.py
+-rw-rw-rw-   0        0        0      599 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/loggers/loggers.py
+-rw-rw-rw-   0        0        0      653 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/loggers/vdl_logger.py
+-rw-rw-rw-   0        0        0     2452 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/loggers/wandb_logger.py
+-rw-rw-rw-   0        0        0     2757 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/logging.py
+-rw-rw-rw-   0        0        0     3680 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/utils/network.py
+-rw-rw-rw-   0        0        0     4283 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/poly_nms.py
+-rw-rw-rw-   0        0        0    32871 2024-03-01 07:07:48.000000 fadoudou2-2.7.0.3.8/ppocr/utils/ppocr_keys_v1.txt
+-rw-rw-rw-   0        0        0     5388 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/utils/profiler.py
+-rw-rw-rw-   0        0        0     9373 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/utils/save_load.py
+-rw-rw-rw-   0        0        0     2304 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppocr/utils/stats.py
+-rw-rw-rw-   0        0        0     6984 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/utils/utility.py
+-rw-rw-rw-   0        0        0     4551 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppocr/utils/visual.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.715889 fadoudou2-2.7.0.3.8/ppstructure/
+-rw-rw-rw-   0        0        0      621 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppstructure/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.723891 fadoudou2-2.7.0.3.8/ppstructure/kie/
+-rw-rw-rw-   0        0        0     6004 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppstructure/kie/predict_kie_token_ser.py
+-rw-rw-rw-   0        0        0     5014 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppstructure/kie/predict_kie_token_ser_re.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.734887 fadoudou2-2.7.0.3.8/ppstructure/kie/tools/
+-rw-rw-rw-   0        0        0     8518 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppstructure/kie/tools/eval_with_label_end2end.py
+-rw-rw-rw-   0        0        0     6202 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppstructure/kie/tools/trans_funsd_label.py
+-rw-rw-rw-   0        0        0     2161 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppstructure/kie/tools/trans_xfun_data.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.739887 fadoudou2-2.7.0.3.8/ppstructure/layout/
+-rw-rw-rw-   0        0        0      621 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppstructure/layout/__init__.py
+-rw-rw-rw-   0        0        0     4285 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppstructure/layout/predict_layout.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.744887 fadoudou2-2.7.0.3.8/ppstructure/pdf2word/
+-rw-rw-rw-   0        0        0    21178 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppstructure/pdf2word/pdf2word.py
+-rw-rw-rw-   0        0        0    14074 2024-01-18 10:40:29.000000 fadoudou2-2.7.0.3.8/ppstructure/predict_system.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.753892 fadoudou2-2.7.0.3.8/ppstructure/recovery/
+-rw-rw-rw-   0        0        0      621 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppstructure/recovery/__init__.py
+-rw-rw-rw-   0        0        0     5537 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppstructure/recovery/recovery_to_doc.py
+-rw-rw-rw-   0        0        0    11710 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppstructure/recovery/table_process.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.781537 fadoudou2-2.7.0.3.8/ppstructure/table/
+-rw-rw-rw-   0        0        0      621 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppstructure/table/__init__.py
+-rw-rw-rw-   0        0        0     3145 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppstructure/table/convert_label2html.py
+-rw-rw-rw-   0        0        0     3581 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppstructure/table/eval_table.py
+-rw-rw-rw-   0        0        0     8164 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppstructure/table/matcher.py
+-rw-rw-rw-   0        0        0     7686 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppstructure/table/predict_structure.py
+-rw-rw-rw-   0        0        0     8752 2023-12-26 16:06:53.000000 fadoudou2-2.7.0.3.8/ppstructure/table/predict_table.py
+-rw-rw-rw-   0        0        0    37580 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppstructure/table/table_master_match.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.793536 fadoudou2-2.7.0.3.8/ppstructure/table/table_metric/
+-rw-rw-rw-   0        0        0      673 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppstructure/table/table_metric/__init__.py
+-rw-rw-rw-   0        0        0     2198 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppstructure/table/table_metric/parallel.py
+-rw-rw-rw-   0        0        0     8599 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppstructure/table/table_metric/table_metric.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.803541 fadoudou2-2.7.0.3.8/ppstructure/table/tablepyxl/
+-rw-rw-rw-   0        0        0      619 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppstructure/table/tablepyxl/__init__.py
+-rw-rw-rw-   0        0        0    10415 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppstructure/table/tablepyxl/style.py
+-rw-rw-rw-   0        0        0     4217 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/ppstructure/table/tablepyxl/tablepyxl.py
+-rw-rw-rw-   0        0        0    12552 2024-03-29 02:19:19.000000 fadoudou2-2.7.0.3.8/ppstructure/utility.py
+-rw-rw-rw-   0        0        0       42 2024-04-01 09:38:27.845539 fadoudou2-2.7.0.3.8/setup.cfg
+-rw-rw-rw-   0        0        0     2663 2024-02-01 08:24:19.000000 fadoudou2-2.7.0.3.8/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.806536 fadoudou2-2.7.0.3.8/tools/
+-rw-rw-rw-   0        0        0      708 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/tools/__init__.py
+drwxrwxrwx   0        0        0        0 2024-04-01 09:38:27.843537 fadoudou2-2.7.0.3.8/tools/infer/
+-rw-rw-rw-   0        0        0    69313 2023-12-27 09:24:55.000000 fadoudou2-2.7.0.3.8/tools/infer/diff_match_patch.py
+-rw-rw-rw-   0        0        0     5891 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/tools/infer/predict_cls.py
+-rw-rw-rw-   0        0        0    14487 2024-03-26 08:51:22.000000 fadoudou2-2.7.0.3.8/tools/infer/predict_det.py
+-rw-rw-rw-   0        0        0     6458 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/tools/infer/predict_e2e.py
+-rw-rw-rw-   0        0        0    29985 2024-03-26 10:18:25.000000 fadoudou2-2.7.0.3.8/tools/infer/predict_rec.py
+-rw-rw-rw-   0        0        0     5813 2023-12-20 10:07:39.000000 fadoudou2-2.7.0.3.8/tools/infer/predict_sr.py
+-rw-rw-rw-   0        0        0    12170 2024-03-01 06:07:23.000000 fadoudou2-2.7.0.3.8/tools/infer/predict_system.py
+-rw-rw-rw-   0        0        0    26113 2024-03-01 06:26:55.000000 fadoudou2-2.7.0.3.8/tools/infer/utility.py
```

### Comparing `fadoudou2-2.7.0.3.7/LICENSE` & `fadoudou2-2.7.0.3.8/LICENSE`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/PKG-INFO` & `fadoudou2-2.7.0.3.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fadoudou2
-Version: 2.7.0.3.7
+Version: 2.7.0.3.8
 Summary: Awesome OCR toolkits based on PaddlePaddle (8.6M ultra-lightweight pre-trained model, support training and deployment among server, mobile, embeded and IoT devices)
 Home-page: https://github.com/PaddlePaddle/PaddleOCR
 Download-URL: https://github.com/PaddlePaddle/PaddleOCR.git
 License: Apache License 2.0
 Keywords: ocr textdetection textrecognition paddleocr crnn east star-net rosetta ocrlite db chineseocr chinesetextdetection chinesetextrecognition
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `fadoudou2-2.7.0.3.7/README.md` & `fadoudou2-2.7.0.3.8/README.md`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/__init__.py` & `fadoudou2-2.7.0.3.8/__init__.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/fadoudou2.egg-info/PKG-INFO` & `fadoudou2-2.7.0.3.8/fadoudou2.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fadoudou2
-Version: 2.7.0.3.7
+Version: 2.7.0.3.8
 Summary: Awesome OCR toolkits based on PaddlePaddle (8.6M ultra-lightweight pre-trained model, support training and deployment among server, mobile, embeded and IoT devices)
 Home-page: https://github.com/PaddlePaddle/PaddleOCR
 Download-URL: https://github.com/PaddlePaddle/PaddleOCR.git
 License: Apache License 2.0
 Keywords: ocr textdetection textrecognition paddleocr crnn east star-net rosetta ocrlite db chineseocr chinesetextdetection chinesetextrecognition
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `fadoudou2-2.7.0.3.7/fadoudou2.egg-info/SOURCES.txt` & `fadoudou2-2.7.0.3.8/fadoudou2.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/paddleocr.py` & `fadoudou2-2.7.0.3.8/paddleocr.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,15 +55,15 @@
 logger = get_logger()
 __all__ = [
     'PaddleOCR', 'PPStructure', 'draw_ocr', 'draw_structure_result',
     'save_structure_res', 'download_with_progressbar', 'to_excel'
 ]
 
 SUPPORT_DET_MODEL = ['DB']
-VERSION = '2.7.0.3.7'
+VERSION = '2.7.0.3.8'
 SUPPORT_REC_MODEL = ['CRNN', 'SVTR_LCNet','CTCLabelDecode']
 BASE_DIR = os.path.expanduser("~/.paddleocr/")
 
 DEFAULT_OCR_MODEL_VERSION = 'PP-OCRv4'
 SUPPORT_OCR_MODEL_VERSION = ['PP-OCR', 'PP-OCRv2', 'PP-OCRv3', 'PP-OCRv4']
 DEFAULT_STRUCTURE_MODEL_VERSION = 'PP-StructureV2'
 SUPPORT_STRUCTURE_MODEL_VERSION = ['PP-Structure', 'PP-StructureV2']
```

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/__init__.py` & `fadoudou2-2.7.0.3.8/ppocr/data/__init__.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/collate_fn.py` & `fadoudou2-2.7.0.3.8/ppocr/data/collate_fn.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/ColorJitter.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/ColorJitter.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/__init__.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/__init__.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/abinet_aug.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/abinet_aug.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/copy_paste.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/copy_paste.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/ct_process.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/ct_process.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/drrg_targets.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/drrg_targets.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/east_process.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/east_process.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/fce_aug.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/fce_aug.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/fce_targets.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/fce_targets.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/iaa_augment.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/iaa_augment.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/label_ops.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/label_ops.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/make_border_map.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/make_border_map.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/make_pse_gt.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/make_pse_gt.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/make_shrink_map.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/make_shrink_map.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/operators.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/operators.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/pg_process.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/pg_process.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/randaugment.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/randaugment.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/random_crop_data.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/random_crop_data.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/rec_img_aug.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/rec_img_aug.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/sast_process.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/sast_process.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/ssl_img_aug.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/ssl_img_aug.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/table_ops.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/table_ops.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/text_image_aug/__init__.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/text_image_aug/__init__.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/text_image_aug/augment.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/text_image_aug/augment.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/text_image_aug/warp_mls.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/text_image_aug/warp_mls.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/vqa/__init__.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/vqa/__init__.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/vqa/augment.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/vqa/augment.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/vqa/token/__init__.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/vqa/token/__init__.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/vqa/token/vqa_re_convert.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/vqa/token/vqa_re_convert.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/vqa/token/vqa_token_chunk.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/vqa/token/vqa_token_chunk.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/vqa/token/vqa_token_pad.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/vqa/token/vqa_token_pad.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/imaug/vqa/token/vqa_token_relation.py` & `fadoudou2-2.7.0.3.8/ppocr/data/imaug/vqa/token/vqa_token_relation.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/lmdb_dataset.py` & `fadoudou2-2.7.0.3.8/ppocr/data/lmdb_dataset.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/multi_scale_sampler.py` & `fadoudou2-2.7.0.3.8/ppocr/data/multi_scale_sampler.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/pgnet_dataset.py` & `fadoudou2-2.7.0.3.8/ppocr/data/pgnet_dataset.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/pubtab_dataset.py` & `fadoudou2-2.7.0.3.8/ppocr/data/pubtab_dataset.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/data/simple_dataset.py` & `fadoudou2-2.7.0.3.8/ppocr/data/simple_dataset.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/postprocess/__init__.py` & `fadoudou2-2.7.0.3.8/ppocr/postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/postprocess/cls_postprocess.py` & `fadoudou2-2.7.0.3.8/ppocr/postprocess/cls_postprocess.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/postprocess/ct_postprocess.py` & `fadoudou2-2.7.0.3.8/ppocr/postprocess/ct_postprocess.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/postprocess/db_postprocess.py` & `fadoudou2-2.7.0.3.8/ppocr/postprocess/db_postprocess.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/postprocess/drrg_postprocess.py` & `fadoudou2-2.7.0.3.8/ppocr/postprocess/drrg_postprocess.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/postprocess/east_postprocess.py` & `fadoudou2-2.7.0.3.8/ppocr/postprocess/east_postprocess.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/postprocess/fce_postprocess.py` & `fadoudou2-2.7.0.3.8/ppocr/postprocess/fce_postprocess.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/postprocess/locality_aware_nms.py` & `fadoudou2-2.7.0.3.8/ppocr/postprocess/locality_aware_nms.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/postprocess/pg_postprocess.py` & `fadoudou2-2.7.0.3.8/ppocr/postprocess/pg_postprocess.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/postprocess/picodet_postprocess.py` & `fadoudou2-2.7.0.3.8/ppocr/postprocess/picodet_postprocess.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/postprocess/pse_postprocess/__init__.py` & `fadoudou2-2.7.0.3.8/ppocr/postprocess/pse_postprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/postprocess/pse_postprocess/pse/__init__.py` & `fadoudou2-2.7.0.3.8/ppocr/postprocess/pse_postprocess/pse/__init__.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/postprocess/pse_postprocess/pse_postprocess.py` & `fadoudou2-2.7.0.3.8/ppocr/postprocess/pse_postprocess/pse_postprocess.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/postprocess/rec_postprocess.py` & `fadoudou2-2.7.0.3.8/ppocr/postprocess/rec_postprocess.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/postprocess/sast_postprocess.py` & `fadoudou2-2.7.0.3.8/ppocr/postprocess/sast_postprocess.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/postprocess/table_postprocess.py` & `fadoudou2-2.7.0.3.8/ppocr/postprocess/table_postprocess.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/postprocess/vqa_token_re_layoutlm_postprocess.py` & `fadoudou2-2.7.0.3.8/ppocr/postprocess/vqa_token_re_layoutlm_postprocess.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/postprocess/vqa_token_ser_layoutlm_postprocess.py` & `fadoudou2-2.7.0.3.8/ppocr/postprocess/vqa_token_ser_layoutlm_postprocess.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/__init__.py` & `fadoudou2-2.7.0.3.8/ppocr/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/__pycache__/logging.cpython-310.pyc` & `fadoudou2-2.7.0.3.8/ppocr/utils/__pycache__/logging.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/__pycache__/network.cpython-310.pyc` & `fadoudou2-2.7.0.3.8/ppocr/utils/__pycache__/network.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/__pycache__/poly_nms.cpython-310.pyc` & `fadoudou2-2.7.0.3.8/ppocr/utils/__pycache__/poly_nms.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/__pycache__/profiler.cpython-310.pyc` & `fadoudou2-2.7.0.3.8/ppocr/utils/__pycache__/profiler.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/__pycache__/save_load.cpython-310.pyc` & `fadoudou2-2.7.0.3.8/ppocr/utils/__pycache__/save_load.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/__pycache__/stats.cpython-310.pyc` & `fadoudou2-2.7.0.3.8/ppocr/utils/__pycache__/stats.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/__pycache__/utility.cpython-310.pyc` & `fadoudou2-2.7.0.3.8/ppocr/utils/__pycache__/utility.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/__pycache__/visual.cpython-310.pyc` & `fadoudou2-2.7.0.3.8/ppocr/utils/__pycache__/visual.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/corpus/fi_corpus.txt` & `fadoudou2-2.7.0.3.8/ppocr/utils/corpus/fi_corpus.txt`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/dict/arabic_dict.txt` & `fadoudou2-2.7.0.3.8/ppocr/utils/dict/arabic_dict.txt`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/dict/chinese_cht_dict.txt` & `fadoudou2-2.7.0.3.8/ppocr/utils/dict/chinese_cht_dict.txt`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/dict/confuse.pkl` & `fadoudou2-2.7.0.3.8/ppocr/utils/dict/confuse.pkl`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/dict/cyrillic_dict.txt` & `fadoudou2-2.7.0.3.8/ppocr/utils/dict/cyrillic_dict.txt`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/dict/devanagari_dict.txt` & `fadoudou2-2.7.0.3.8/ppocr/utils/dict/devanagari_dict.txt`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/dict/hi_dict.txt` & `fadoudou2-2.7.0.3.8/ppocr/utils/dict/hi_dict.txt`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/dict/japan_dict.txt` & `fadoudou2-2.7.0.3.8/ppocr/utils/dict/japan_dict.txt`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/dict/ka_dict.txt` & `fadoudou2-2.7.0.3.8/ppocr/utils/dict/ka_dict.txt`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/dict/korean_dict.txt` & `fadoudou2-2.7.0.3.8/ppocr/utils/dict/korean_dict.txt`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/dict/latin_dict.txt` & `fadoudou2-2.7.0.3.8/ppocr/utils/dict/latin_dict.txt`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/dict/mr_dict.txt` & `fadoudou2-2.7.0.3.8/ppocr/utils/dict/mr_dict.txt`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/dict/ne_dict.txt` & `fadoudou2-2.7.0.3.8/ppocr/utils/dict/ne_dict.txt`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/dict/table_dict.txt` & `fadoudou2-2.7.0.3.8/ppocr/utils/dict/table_dict.txt`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/dict/table_structure_dict_ch.txt` & `fadoudou2-2.7.0.3.8/ppocr/utils/dict/table_structure_dict_ch.txt`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/dict/te_dict.txt` & `fadoudou2-2.7.0.3.8/ppocr/utils/dict/te_dict.txt`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/e2e_metric/Deteval.py` & `fadoudou2-2.7.0.3.8/ppocr/utils/e2e_metric/Deteval.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/e2e_metric/polygon_fast.py` & `fadoudou2-2.7.0.3.8/ppocr/utils/e2e_metric/polygon_fast.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/e2e_utils/__pycache__/extract_textpoint_fast.cpython-310.pyc` & `fadoudou2-2.7.0.3.8/ppocr/utils/e2e_utils/__pycache__/extract_textpoint_fast.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/e2e_utils/__pycache__/extract_textpoint_slow.cpython-310.pyc` & `fadoudou2-2.7.0.3.8/ppocr/utils/e2e_utils/__pycache__/extract_textpoint_slow.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/e2e_utils/__pycache__/pgnet_pp_utils.cpython-310.pyc` & `fadoudou2-2.7.0.3.8/ppocr/utils/e2e_utils/__pycache__/pgnet_pp_utils.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/e2e_utils/extract_batchsize.py` & `fadoudou2-2.7.0.3.8/ppocr/utils/e2e_utils/extract_batchsize.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/e2e_utils/extract_textpoint_fast.py` & `fadoudou2-2.7.0.3.8/ppocr/utils/e2e_utils/extract_textpoint_fast.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/e2e_utils/extract_textpoint_slow.py` & `fadoudou2-2.7.0.3.8/ppocr/utils/e2e_utils/extract_textpoint_slow.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/e2e_utils/pgnet_pp_utils.py` & `fadoudou2-2.7.0.3.8/ppocr/utils/e2e_utils/pgnet_pp_utils.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/e2e_utils/visual.py` & `fadoudou2-2.7.0.3.8/ppocr/utils/e2e_utils/visual.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/gen_label.py` & `fadoudou2-2.7.0.3.8/ppocr/utils/gen_label.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/iou.py` & `fadoudou2-2.7.0.3.8/ppocr/utils/iou.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/loggers/__pycache__/base_logger.cpython-310.pyc` & `fadoudou2-2.7.0.3.8/ppocr/utils/loggers/__pycache__/base_logger.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/loggers/__pycache__/loggers.cpython-310.pyc` & `fadoudou2-2.7.0.3.8/ppocr/utils/loggers/__pycache__/loggers.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/loggers/__pycache__/vdl_logger.cpython-310.pyc` & `fadoudou2-2.7.0.3.8/ppocr/utils/loggers/__pycache__/vdl_logger.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/loggers/__pycache__/wandb_logger.cpython-310.pyc` & `fadoudou2-2.7.0.3.8/ppocr/utils/loggers/__pycache__/wandb_logger.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/loggers/loggers.py` & `fadoudou2-2.7.0.3.8/ppocr/utils/loggers/loggers.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/loggers/vdl_logger.py` & `fadoudou2-2.7.0.3.8/ppocr/utils/loggers/vdl_logger.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/loggers/wandb_logger.py` & `fadoudou2-2.7.0.3.8/ppocr/utils/loggers/wandb_logger.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/logging.py` & `fadoudou2-2.7.0.3.8/ppocr/utils/logging.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/network.py` & `fadoudou2-2.7.0.3.8/ppocr/utils/network.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/poly_nms.py` & `fadoudou2-2.7.0.3.8/ppocr/utils/poly_nms.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/ppocr_keys_v1.txt` & `fadoudou2-2.7.0.3.8/ppocr/utils/ppocr_keys_v1.txt`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/profiler.py` & `fadoudou2-2.7.0.3.8/ppocr/utils/profiler.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/save_load.py` & `fadoudou2-2.7.0.3.8/ppocr/utils/save_load.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/stats.py` & `fadoudou2-2.7.0.3.8/ppocr/utils/stats.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/utility.py` & `fadoudou2-2.7.0.3.8/ppocr/utils/utility.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppocr/utils/visual.py` & `fadoudou2-2.7.0.3.8/ppocr/utils/visual.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/__init__.py` & `fadoudou2-2.7.0.3.8/ppstructure/__init__.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/kie/predict_kie_token_ser.py` & `fadoudou2-2.7.0.3.8/ppstructure/kie/predict_kie_token_ser.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/kie/predict_kie_token_ser_re.py` & `fadoudou2-2.7.0.3.8/ppstructure/kie/predict_kie_token_ser_re.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/kie/tools/eval_with_label_end2end.py` & `fadoudou2-2.7.0.3.8/ppstructure/kie/tools/eval_with_label_end2end.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/kie/tools/trans_funsd_label.py` & `fadoudou2-2.7.0.3.8/ppstructure/kie/tools/trans_funsd_label.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/kie/tools/trans_xfun_data.py` & `fadoudou2-2.7.0.3.8/ppstructure/kie/tools/trans_xfun_data.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/layout/__init__.py` & `fadoudou2-2.7.0.3.8/ppstructure/layout/__init__.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/layout/predict_layout.py` & `fadoudou2-2.7.0.3.8/ppstructure/layout/predict_layout.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/pdf2word/pdf2word.py` & `fadoudou2-2.7.0.3.8/ppstructure/pdf2word/pdf2word.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/predict_system.py` & `fadoudou2-2.7.0.3.8/ppstructure/predict_system.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/recovery/__init__.py` & `fadoudou2-2.7.0.3.8/ppstructure/recovery/__init__.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/recovery/recovery_to_doc.py` & `fadoudou2-2.7.0.3.8/ppstructure/recovery/recovery_to_doc.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/recovery/table_process.py` & `fadoudou2-2.7.0.3.8/ppstructure/recovery/table_process.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/table/__init__.py` & `fadoudou2-2.7.0.3.8/ppstructure/table/__init__.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/table/convert_label2html.py` & `fadoudou2-2.7.0.3.8/ppstructure/table/convert_label2html.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/table/eval_table.py` & `fadoudou2-2.7.0.3.8/ppstructure/table/eval_table.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/table/matcher.py` & `fadoudou2-2.7.0.3.8/ppstructure/table/matcher.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/table/predict_structure.py` & `fadoudou2-2.7.0.3.8/ppstructure/table/predict_structure.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/table/predict_table.py` & `fadoudou2-2.7.0.3.8/ppstructure/table/predict_table.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/table/table_master_match.py` & `fadoudou2-2.7.0.3.8/ppstructure/table/table_master_match.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/table/table_metric/__init__.py` & `fadoudou2-2.7.0.3.8/ppstructure/table/table_metric/__init__.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/table/table_metric/parallel.py` & `fadoudou2-2.7.0.3.8/ppstructure/table/table_metric/parallel.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/table/table_metric/table_metric.py` & `fadoudou2-2.7.0.3.8/ppstructure/table/table_metric/table_metric.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/table/tablepyxl/__init__.py` & `fadoudou2-2.7.0.3.8/ppstructure/table/tablepyxl/__init__.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/table/tablepyxl/style.py` & `fadoudou2-2.7.0.3.8/ppstructure/table/tablepyxl/style.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/table/tablepyxl/tablepyxl.py` & `fadoudou2-2.7.0.3.8/ppstructure/table/tablepyxl/tablepyxl.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/ppstructure/utility.py` & `fadoudou2-2.7.0.3.8/ppstructure/utility.py`

 * *Files 12% similar despite different names*

```diff
@@ -267,7 +267,51 @@
             cell_x_start = max(int(center_x - avg_char_width / 2), 0) + bbox_x_start
             cell_x_end = min(int(center_x + avg_char_width / 2), bbox_x_end - bbox_x_start) + bbox_x_start
             cell = ((cell_x_start, bbox_y_start), (cell_x_end, bbox_y_start), (cell_x_end, bbox_y_end),
                     (cell_x_start, bbox_y_end))
             word_box_list.append(cell)
     return flatten_list(word_box_content_list), sort_word_box_list(word_box_list)
 
+
+def en_cal_ocr_word_box(rec_str, box, rec_word_info):
+    ''' Calculate the detection frame for each word based on the results of recognition and detection of ocr'''
+
+    col_num, word_list, word_col_list, state_list = rec_word_info
+    box = box.tolist()
+    bbox_x_start = box[0][0]
+    bbox_x_end = box[1][0]
+    bbox_y_start = box[0][1]
+    bbox_y_end = box[2][1]
+
+    cell_width = (bbox_x_end - bbox_x_start)/col_num
+
+    word_box_list = []
+    word_box_content_list = []
+    cn_width_list = []
+    cn_col_list = []
+    for word, word_col, state in zip(word_list, word_col_list, state_list):
+        if state == 'cn':
+            if len(word_col) != 1:
+                char_seq_length = (word_col[-1] - word_col[0] + 1) * cell_width
+                char_width = char_seq_length/(len(word_col)-1)
+                cn_width_list.append(char_width)
+            cn_col_list += word_col
+            word_box_content_list += word
+        else:
+            cell_x_start = bbox_x_start + int(word_col[0] * cell_width)
+            cell_x_end = bbox_x_start + int((word_col[-1]+1) * cell_width)
+            cell = ((cell_x_start, bbox_y_start), (cell_x_end, bbox_y_start), (cell_x_end, bbox_y_end), (cell_x_start, bbox_y_end))
+            word_box_list.append(cell)
+            word_box_content_list.append("".join(word))
+    if len(cn_col_list) != 0:
+        if len(cn_width_list) != 0:
+            avg_char_width = np.mean(cn_width_list)
+        else:
+            avg_char_width = (bbox_x_end - bbox_x_start)/len(rec_str)
+        for center_idx in cn_col_list:
+            center_x = (center_idx+0.5)*cell_width
+            cell_x_start = max(int(center_x - avg_char_width/2), 0) + bbox_x_start
+            cell_x_end = min(int(center_x + avg_char_width/2), bbox_x_end-bbox_x_start) + bbox_x_start
+            cell = ((cell_x_start, bbox_y_start), (cell_x_end, bbox_y_start), (cell_x_end, bbox_y_end), (cell_x_start, bbox_y_end))
+            word_box_list.append(cell)
+
+    return word_box_content_list, word_box_list
```

### Comparing `fadoudou2-2.7.0.3.7/setup.py` & `fadoudou2-2.7.0.3.8/setup.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/tools/__init__.py` & `fadoudou2-2.7.0.3.8/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/tools/infer/diff_match_patch.py` & `fadoudou2-2.7.0.3.8/tools/infer/diff_match_patch.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/tools/infer/predict_cls.py` & `fadoudou2-2.7.0.3.8/tools/infer/predict_cls.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/tools/infer/predict_det.py` & `fadoudou2-2.7.0.3.8/tools/infer/predict_det.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/tools/infer/predict_e2e.py` & `fadoudou2-2.7.0.3.8/tools/infer/predict_e2e.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/tools/infer/predict_rec.py` & `fadoudou2-2.7.0.3.8/tools/infer/predict_rec.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/tools/infer/predict_sr.py` & `fadoudou2-2.7.0.3.8/tools/infer/predict_sr.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/tools/infer/predict_system.py` & `fadoudou2-2.7.0.3.8/tools/infer/predict_system.py`

 * *Files identical despite different names*

### Comparing `fadoudou2-2.7.0.3.7/tools/infer/utility.py` & `fadoudou2-2.7.0.3.8/tools/infer/utility.py`

 * *Files identical despite different names*

