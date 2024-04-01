# Comparing `tmp/FanFicFare-4.8.0.tar.gz` & `tmp/FanFicFare-4.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FanFicFare-4.8.0.tar", last modified: Thu Dec  2 15:36:51 2021, max compression
+gzip compressed data, was "FanFicFare-4.9.0.tar", last modified: Tue Jan 11 22:02:21 2022, max compression
```

## Comparing `FanFicFare-4.8.0.tar` & `FanFicFare-4.9.0.tar`

### file list

```diff
@@ -1,199 +1,199 @@
-drwxrwxrwx   0        0        0        0 2021-12-02 15:36:51.488760 FanFicFare-4.8.0/
--rw-rw-rw-   0        0        0      498 2019-05-01 14:05:45.000000 FanFicFare-4.8.0/DESCRIPTION.rst
-drwxrwxrwx   0        0        0        0 2021-12-02 15:36:51.272605 FanFicFare-4.8.0/FanFicFare.egg-info/
--rw-rw-rw-   0        0        0     1195 2021-12-02 15:36:50.000000 FanFicFare-4.8.0/FanFicFare.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     8120 2021-12-02 15:36:51.000000 FanFicFare-4.8.0/FanFicFare.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-12-02 15:36:50.000000 FanFicFare-4.8.0/FanFicFare.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2021-12-02 15:36:50.000000 FanFicFare-4.8.0/FanFicFare.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      177 2021-12-02 15:36:50.000000 FanFicFare-4.8.0/FanFicFare.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2021-12-02 15:36:50.000000 FanFicFare-4.8.0/FanFicFare.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    46701 2019-05-01 14:05:45.000000 FanFicFare-4.8.0/LICENSE
--rw-rw-rw-   0        0        0       58 2019-05-01 14:05:45.000000 FanFicFare-4.8.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1195 2021-12-02 15:36:51.488760 FanFicFare-4.8.0/PKG-INFO
--rw-rw-rw-   0        0        0     2972 2021-09-23 15:30:39.000000 FanFicFare-4.8.0/README.md
-drwxrwxrwx   0        0        0        0 2021-12-02 15:36:51.303859 FanFicFare-4.8.0/fanficfare/
--rw-rw-rw-   0        0        0     1773 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/HtmlTagStack.py
--rw-rw-rw-   0        0        0     1455 2021-09-17 02:51:53.000000 FanFicFare-4.8.0/fanficfare/__init__.py
-drwxrwxrwx   0        0        0        0 2021-12-02 15:36:51.457509 FanFicFare-4.8.0/fanficfare/adapters/
--rw-rw-rw-   0        0        0    12282 2021-11-20 21:50:25.000000 FanFicFare-4.8.0/fanficfare/adapters/__init__.py
--rw-rw-rw-   0        0        0     8619 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_adastrafanficcom.py
--rw-rw-rw-   0        0        0    20915 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_adultfanfictionorg.py
--rw-rw-rw-   0        0        0     1582 2021-09-17 02:51:53.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_alternatehistorycom.py
--rw-rw-rw-   0        0        0    11518 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_andromedawebcom.py
--rw-rw-rw-   0        0        0    29117 2021-09-23 15:57:25.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_archiveofourownorg.py
--rw-rw-rw-   0        0        0     6882 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_archiveskyehawkecom.py
--rw-rw-rw-   0        0        0     6132 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_asexstoriescom.py
--rw-rw-rw-   0        0        0     9331 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_ashwindersycophanthexcom.py
--rw-rw-rw-   0        0        0    10613 2021-09-23 15:15:22.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_asianfanficscom.py
--rw-rw-rw-   0        0        0     8554 2021-09-17 02:51:53.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_bdsmlibrarycom.py
--rw-rw-rw-   0        0        0     7849 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_bloodshedversecom.py
--rw-rw-rw-   0        0        0    13000 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_bloodtiesfancom.py
--rw-rw-rw-   0        0        0    11404 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_buffygilescom.py
--rw-rw-rw-   0        0        0     8756 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_chaossycophanthexcom.py
--rw-rw-rw-   0        0        0     3855 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_chireadscom.py
--rw-rw-rw-   0        0        0     9557 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_chosentwofanficcom.py
--rw-rw-rw-   0        0        0     8847 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_csiforensicscom.py
--rw-rw-rw-   0        0        0     1954 2021-02-03 15:44:28.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_darksolaceorg.py
--rw-rw-rw-   0        0        0     8967 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_destinysgatewaycom.py
--rw-rw-rw-   0        0        0     6949 2021-11-19 16:12:35.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_deviantartcom.py
--rw-rw-rw-   0        0        0    10426 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_dokugacom.py
--rw-rw-rw-   0        0        0    11384 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_dracoandginnycom.py
--rw-rw-rw-   0        0        0    12348 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_efpfanficnet.py
--rw-rw-rw-   0        0        0     9377 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_erosnsapphosycophanthexcom.py
--rw-rw-rw-   0        0        0    12401 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_fanficauthorsnet.py
--rw-rw-rw-   0        0        0     7024 2021-09-28 17:51:47.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_fanfichu.py
--rw-rw-rw-   0        0        0    14662 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_fanficsme.py
--rw-rw-rw-   0        0        0     9371 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_fanfictalkcom.py
--rw-rw-rw-   0        0        0    17458 2021-09-19 17:49:46.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_fanfictionnet.py
--rw-rw-rw-   0        0        0     8894 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_fanfiktionde.py
--rw-rw-rw-   0        0        0     5078 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_fastnovelnet.py
--rw-rw-rw-   0        0        0     9418 2021-11-09 14:53:20.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_ficbooknet.py
--rw-rw-rw-   0        0        0     9280 2021-10-27 18:34:30.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_fictionalleyarchiveorg.py
--rw-rw-rw-   0        0        0     9301 2021-10-11 01:33:24.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_fictionhuntcom.py
--rw-rw-rw-   0        0        0    25264 2021-09-17 02:51:53.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_fictionlive.py
--rw-rw-rw-   0        0        0     7883 2021-09-17 02:51:53.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_fictionmaniatv.py
--rw-rw-rw-   0        0        0     1768 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_fictionpresscom.py
--rw-rw-rw-   0        0        0     9080 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_ficwadcom.py
--rw-rw-rw-   0        0        0    20025 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_fimfictionnet.py
--rw-rw-rw-   0        0        0     2237 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_finestoriescom.py
--rw-rw-rw-   0        0        0     7515 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_fireflyfansnet.py
--rw-rw-rw-   0        0        0     1735 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_forumquestionablequestingcom.py
--rw-rw-rw-   0        0        0     1726 2021-02-03 15:44:28.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_forumsspacebattlescom.py
--rw-rw-rw-   0        0        0     1894 2021-02-03 15:44:28.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_forumssufficientvelocitycom.py
--rw-rw-rw-   0        0        0     1874 2021-02-03 15:44:28.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_gluttonyfictioncom.py
--rw-rw-rw-   0        0        0     7237 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_hentaifoundrycom.py
--rw-rw-rw-   0        0        0     8526 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_hlfictionnet.py
--rw-rw-rw-   0        0        0     9052 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_hpfanficarchivecom.py
--rw-rw-rw-   0        0        0    10642 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_iketernalnet.py
--rw-rw-rw-   0        0        0    10909 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_imagineeficcom.py
--rw-rw-rw-   0        0        0     7925 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_inkbunnynet.py
--rw-rw-rw-   0        0        0    13928 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_ksarchivecom.py
--rw-rw-rw-   0        0        0     7548 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_lcfanficcom.py
--rw-rw-rw-   0        0        0     1196 2021-02-03 15:44:28.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_libraryofmoriacom.py
--rw-rw-rw-   0        0        0    19048 2021-09-17 02:51:53.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_literotica.py
--rw-rw-rw-   0        0        0     1865 2021-06-27 15:03:30.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_looselugscom.py
--rw-rw-rw-   0        0        0    14950 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_lotrgficcom.py
--rw-rw-rw-   0        0        0     8756 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_lumossycophanthexcom.py
--rw-rw-rw-   0        0        0    28595 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_masseffect2in.py
--rw-rw-rw-   0        0        0     6456 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_mcstoriescom.py
--rw-rw-rw-   0        0        0     8576 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_mediaminerorg.py
--rw-rw-rw-   0        0        0    11146 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_merlinficdtwinscouk.py
--rw-rw-rw-   0        0        0    11916 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_midnightwhispers.py
--rw-rw-rw-   0        0        0     1205 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_mttjustoncenet.py
--rw-rw-rw-   0        0        0     1179 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_mugglenetfanfictioncom.py
--rw-rw-rw-   0        0        0     1084 2021-02-03 15:44:28.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_naiceanilmenet.py
--rw-rw-rw-   0        0        0     1114 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_narutoficorg.py
--rw-rw-rw-   0        0        0     1344 2021-02-03 15:44:28.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_ncisfictioncom.py
--rw-rw-rw-   0        0        0     1754 2021-02-03 15:44:28.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_ninelivesarchivecom.py
--rw-rw-rw-   0        0        0     3421 2021-11-20 21:21:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_novelfull.py
--rw-rw-rw-   0        0        0     8115 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_novelonlinefullcom.py
--rw-rw-rw-   0        0        0     6204 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_noveltrovecom.py
--rw-rw-rw-   0        0        0     1512 2021-02-03 15:44:28.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_novelupdatescc.py
--rw-rw-rw-   0        0        0     9436 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_occlumencysycophanthexcom.py
--rw-rw-rw-   0        0        0     8827 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_phoenixsongnet.py
--rw-rw-rw-   0        0        0    10124 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_ponyfictionarchivenet.py
--rw-rw-rw-   0        0        0     8868 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_potionsandsnitches.py
--rw-rw-rw-   0        0        0    11273 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_potterheadsanonymouscom.py
--rw-rw-rw-   0        0        0     9461 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_pretendercentrecom.py
--rw-rw-rw-   0        0        0     8461 2021-11-14 18:00:24.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_psychficcom.py
--rw-rw-rw-   0        0        0     9924 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_qafficcom.py
--rw-rw-rw-   0        0        0     5716 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_quotevcom.py
--rw-rw-rw-   0        0        0     9685 2021-11-02 01:00:56.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_royalroadcom.py
--rw-rw-rw-   0        0        0    13567 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_samandjacknet.py
--rw-rw-rw-   0        0        0    10039 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_scarvesandcoffeenet.py
--rw-rw-rw-   0        0        0     1324 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_scifistoriescom.py
--rw-rw-rw-   0        0        0    15533 2021-11-28 18:27:20.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_scribblehubcom.py
--rw-rw-rw-   0        0        0    12713 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_sheppardweircom.py
--rw-rw-rw-   0        0        0    11378 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_shriftweborgbfa.py
--rw-rw-rw-   0        0        0    12041 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_silmarillionwritersguildorg.py
--rw-rw-rw-   0        0        0     1401 2021-02-03 15:44:29.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_sinfuldreamscomunicornfic.py
--rw-rw-rw-   0        0        0     1410 2021-02-03 15:44:29.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_sinfuldreamscomwhisperedmuse.py
--rw-rw-rw-   0        0        0     1419 2021-02-03 15:44:29.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_sinfuldreamscomwickedtemptation.py
--rw-rw-rw-   0        0        0     9945 2021-09-17 02:51:53.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_siyecouk.py
--rw-rw-rw-   0        0        0     1375 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_spikeluvercom.py
--rw-rw-rw-   0        0        0     1712 2021-02-03 15:44:29.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_squidgeworldorg.py
--rw-rw-rw-   0        0        0     1145 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_starskyhutcharchivenet.py
--rw-rw-rw-   0        0        0     1892 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_starslibrarynet.py
--rw-rw-rw-   0        0        0     6120 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_storiesofardacom.py
--rw-rw-rw-   0        0        0    27163 2021-11-13 01:21:10.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_storiesonlinenet.py
--rw-rw-rw-   0        0        0     7710 2021-09-17 02:51:53.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_sugarquillnet.py
--rw-rw-rw-   0        0        0     5695 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_swiorgru.py
--rw-rw-rw-   0        0        0     1118 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_swordborderlineangelcom.py
--rw-rw-rw-   0        0        0     1266 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_tasteofpoisoninkubationnet.py
--rw-rw-rw-   0        0        0     9210 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_tenhawkpresents.py
--rw-rw-rw-   0        0        0    24101 2021-09-17 02:52:14.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_test1.py
--rw-rw-rw-   0        0        0     1082 2021-02-03 15:44:29.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_tgstorytimecom.py
--rw-rw-rw-   0        0        0     1481 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_thedelphicexpansecom.py
--rw-rw-rw-   0        0        0     1363 2021-02-03 15:44:29.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_thehookupzonenet.py
--rw-rw-rw-   0        0        0     1222 2021-02-03 15:44:29.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_themaplebookshelf.py
--rw-rw-rw-   0        0        0    10243 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_themasquenet.py
--rw-rw-rw-   0        0        0     1984 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_thesietchcom.py
--rw-rw-rw-   0        0        0     7869 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_tomparisdormcom.py
--rw-rw-rw-   0        0        0     8908 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_trekfanfictionnet.py
--rw-rw-rw-   0        0        0    12841 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_trekiverseorg.py
--rw-rw-rw-   0        0        0    17176 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_tthfanficorg.py
--rw-rw-rw-   0        0        0     9255 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_twilightednet.py
--rw-rw-rw-   0        0        0     2017 2021-06-27 15:03:40.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_valentchambercom.py
--rw-rw-rw-   0        0        0     9278 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_voracity2eficcom.py
--rw-rw-rw-   0        0        0     8748 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_walkingtheplankorg.py
--rw-rw-rw-   0        0        0     6795 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_wattpadcom.py
--rw-rw-rw-   0        0        0     9329 2021-11-19 16:22:20.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_webnovelcom.py
--rw-rw-rw-   0        0        0    10615 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_whoficcom.py
--rw-rw-rw-   0        0        0     8176 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_wolverineandroguecom.py
--rw-rw-rw-   0        0        0     2097 2021-09-17 02:51:53.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_worldofxde.py
--rw-rw-rw-   0        0        0     8787 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_wraithbaitcom.py
--rw-rw-rw-   0        0        0     5499 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_wuxiaworldco.py
--rw-rw-rw-   0        0        0     4842 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_wuxiaworldcom.py
--rw-rw-rw-   0        0        0     6313 2021-11-28 18:31:14.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_wuxiaworldsite.py
--rw-rw-rw-   0        0        0     5534 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_wwwaneroticstorycom.py
--rw-rw-rw-   0        0        0     1319 2021-02-03 15:44:29.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_wwwgiantessworldnet.py
--rw-rw-rw-   0        0        0    11650 2021-09-28 17:35:34.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_wwwlushstoriescom.py
--rw-rw-rw-   0        0        0    11455 2021-09-17 02:51:53.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_wwwnovelallcom.py
--rw-rw-rw-   0        0        0     9265 2021-10-24 14:39:42.000000 FanFicFare-4.8.0/fanficfare/adapters/adapter_wwwutopiastoriescom.py
--rw-rw-rw-   0        0        0    37988 2021-11-28 18:31:26.000000 FanFicFare-4.8.0/fanficfare/adapters/base_adapter.py
--rw-rw-rw-   0        0        0    19046 2021-09-17 02:51:53.000000 FanFicFare-4.8.0/fanficfare/adapters/base_efiction_adapter.py
--rw-rw-rw-   0        0        0    13510 2021-09-17 02:51:53.000000 FanFicFare-4.8.0/fanficfare/adapters/base_xenforo2forum_adapter.py
--rw-rw-rw-   0        0        0    38672 2021-09-17 02:51:53.000000 FanFicFare-4.8.0/fanficfare/adapters/base_xenforoforum_adapter.py
-drwxrwxrwx   0        0        0        0 2021-12-02 15:36:51.473136 FanFicFare-4.8.0/fanficfare/browsercache/
--rw-rw-rw-   0        0        0     1460 2021-07-12 17:23:33.000000 FanFicFare-4.8.0/fanficfare/browsercache/__init__.py
--rw-rw-rw-   0        0        0     8965 2021-11-20 21:50:25.000000 FanFicFare-4.8.0/fanficfare/browsercache/basebrowsercache.py
--rw-rw-rw-   0        0        0     5294 2021-09-17 02:51:53.000000 FanFicFare-4.8.0/fanficfare/browsercache/blockfilecache.py
-drwxrwxrwx   0        0        0        0 2021-12-02 15:36:51.473136 FanFicFare-4.8.0/fanficfare/browsercache/chromagnon/
--rw-rw-rw-   0        0        0     3357 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/browsercache/chromagnon/SuperFastHash.py
--rw-rw-rw-   0        0        0        0 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/browsercache/chromagnon/__init__.py
--rw-rw-rw-   0        0        0     3797 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/browsercache/chromagnon/cacheAddress.py
--rw-rw-rw-   0        0        0     3117 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/browsercache/chromagnon/cacheAddressTest.py
--rw-rw-rw-   0        0        0     4094 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/browsercache/chromagnon/cacheBlock.py
--rw-rw-rw-   0        0        0     5398 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/browsercache/chromagnon/cacheData.py
--rw-rw-rw-   0        0        0     7093 2021-09-17 02:51:53.000000 FanFicFare-4.8.0/fanficfare/browsercache/chromagnon/cacheEntry.py
--rw-rw-rw-   0        0        0     9165 2021-09-17 02:51:53.000000 FanFicFare-4.8.0/fanficfare/browsercache/firefoxcache2.py
--rw-rw-rw-   0        0        0     2672 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/browsercache/share_open.py
--rw-rw-rw-   0        0        0     8997 2021-09-17 02:51:53.000000 FanFicFare-4.8.0/fanficfare/browsercache/simplecache.py
--rw-rw-rw-   0        0        0    31519 2021-12-02 15:33:00.000000 FanFicFare-4.8.0/fanficfare/cli.py
--rw-rw-rw-   0        0        0    48777 2021-11-28 18:29:38.000000 FanFicFare-4.8.0/fanficfare/configurable.py
--rw-rw-rw-   0        0        0     3541 2021-09-17 02:51:53.000000 FanFicFare-4.8.0/fanficfare/dateutils.py
--rw-rw-rw-   0        0        0   148081 2021-11-28 18:30:28.000000 FanFicFare-4.8.0/fanficfare/defaults.ini
--rw-rw-rw-   0        0        0    21658 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/epubutils.py
--rw-rw-rw-   0        0        0     2924 2021-09-17 02:51:53.000000 FanFicFare-4.8.0/fanficfare/example.ini
--rw-rw-rw-   0        0        0     4032 2021-07-08 22:31:58.000000 FanFicFare-4.8.0/fanficfare/exceptions.py
--rw-rw-rw-   0        0        0    22287 2021-10-03 01:53:00.000000 FanFicFare-4.8.0/fanficfare/fetcher.py
--rw-rw-rw-   0        0        0    10452 2021-11-03 19:55:14.000000 FanFicFare-4.8.0/fanficfare/flaresolverr_proxy.py
--rw-rw-rw-   0        0        0    14105 2021-10-16 20:29:16.000000 FanFicFare-4.8.0/fanficfare/geturls.py
--rw-rw-rw-   0        0        0    17240 2021-02-03 15:44:30.000000 FanFicFare-4.8.0/fanficfare/htmlcleanup.py
--rw-rw-rw-   0        0        0    15618 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/htmlheuristics.py
--rw-rw-rw-   0        0        0    13565 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/mobi.py
--rw-rw-rw-   0        0        0     5735 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/mobihtml.py
--rw-rw-rw-   0        0        0     6978 2021-09-17 02:51:53.000000 FanFicFare-4.8.0/fanficfare/nsapa_proxy.py
--rw-rw-rw-   0        0        0     5130 2021-10-16 19:41:28.000000 FanFicFare-4.8.0/fanficfare/requestable.py
--rw-rw-rw-   0        0        0    35181 2021-02-03 15:44:30.000000 FanFicFare-4.8.0/fanficfare/six.py
--rw-rw-rw-   0        0        0    64175 2021-11-20 02:17:12.000000 FanFicFare-4.8.0/fanficfare/story.py
--rw-rw-rw-   0        0        0     2914 2021-02-03 15:44:30.000000 FanFicFare-4.8.0/fanficfare/translit.py
-drwxrwxrwx   0        0        0        0 2021-12-02 15:36:51.488760 FanFicFare-4.8.0/fanficfare/writers/
--rw-rw-rw-   0        0        0     1381 2021-02-03 15:44:30.000000 FanFicFare-4.8.0/fanficfare/writers/__init__.py
--rw-rw-rw-   0        0        0    10348 2021-07-05 01:10:06.000000 FanFicFare-4.8.0/fanficfare/writers/base_writer.py
--rw-rw-rw-   0        0        0    40425 2021-09-17 02:51:53.000000 FanFicFare-4.8.0/fanficfare/writers/writer_epub.py
--rw-rw-rw-   0        0        0     5925 2021-09-17 02:51:53.000000 FanFicFare-4.8.0/fanficfare/writers/writer_html.py
--rw-rw-rw-   0        0        0     6673 2021-09-17 02:51:53.000000 FanFicFare-4.8.0/fanficfare/writers/writer_mobi.py
--rw-rw-rw-   0        0        0     5897 2021-09-17 02:51:53.000000 FanFicFare-4.8.0/fanficfare/writers/writer_txt.py
--rw-rw-rw-   0        0        0       42 2021-12-02 15:36:51.488760 FanFicFare-4.8.0/setup.cfg
--rw-rw-rw-   0        0        0     4622 2021-12-02 15:33:00.000000 FanFicFare-4.8.0/setup.py
+drwxrwxrwx   0        0        0        0 2022-01-11 22:02:21.945605 FanFicFare-4.9.0/
+-rw-rw-rw-   0        0        0      498 2019-05-01 14:05:45.000000 FanFicFare-4.9.0/DESCRIPTION.rst
+drwxrwxrwx   0        0        0        0 2022-01-11 22:02:21.698187 FanFicFare-4.9.0/FanFicFare.egg-info/
+-rw-rw-rw-   0        0        0     1195 2022-01-11 22:02:21.000000 FanFicFare-4.9.0/FanFicFare.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     8120 2022-01-11 22:02:21.000000 FanFicFare-4.9.0/FanFicFare.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-01-11 22:02:21.000000 FanFicFare-4.9.0/FanFicFare.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2022-01-11 22:02:21.000000 FanFicFare-4.9.0/FanFicFare.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      177 2022-01-11 22:02:21.000000 FanFicFare-4.9.0/FanFicFare.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2022-01-11 22:02:21.000000 FanFicFare-4.9.0/FanFicFare.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    46701 2019-05-01 14:05:45.000000 FanFicFare-4.9.0/LICENSE
+-rw-rw-rw-   0        0        0       58 2019-05-01 14:05:45.000000 FanFicFare-4.9.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     1195 2022-01-11 22:02:21.945605 FanFicFare-4.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2972 2021-09-23 15:30:39.000000 FanFicFare-4.9.0/README.md
+drwxrwxrwx   0        0        0        0 2022-01-11 22:02:21.713812 FanFicFare-4.9.0/fanficfare/
+-rw-rw-rw-   0        0        0     1773 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/HtmlTagStack.py
+-rw-rw-rw-   0        0        0     1455 2021-09-17 02:51:53.000000 FanFicFare-4.9.0/fanficfare/__init__.py
+drwxrwxrwx   0        0        0        0 2022-01-11 22:02:21.914352 FanFicFare-4.9.0/fanficfare/adapters/
+-rw-rw-rw-   0        0        0    12282 2021-11-20 21:50:25.000000 FanFicFare-4.9.0/fanficfare/adapters/__init__.py
+-rw-rw-rw-   0        0        0     8619 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_adastrafanficcom.py
+-rw-rw-rw-   0        0        0    20915 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_adultfanfictionorg.py
+-rw-rw-rw-   0        0        0     1582 2021-09-17 02:51:53.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_alternatehistorycom.py
+-rw-rw-rw-   0        0        0    11518 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_andromedawebcom.py
+-rw-rw-rw-   0        0        0    29205 2021-12-15 01:33:36.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_archiveofourownorg.py
+-rw-rw-rw-   0        0        0     6882 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_archiveskyehawkecom.py
+-rw-rw-rw-   0        0        0     6132 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_asexstoriescom.py
+-rw-rw-rw-   0        0        0     9331 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_ashwindersycophanthexcom.py
+-rw-rw-rw-   0        0        0    10613 2021-09-23 15:15:22.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_asianfanficscom.py
+-rw-rw-rw-   0        0        0     8554 2021-09-17 02:51:53.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_bdsmlibrarycom.py
+-rw-rw-rw-   0        0        0     7849 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_bloodshedversecom.py
+-rw-rw-rw-   0        0        0    13000 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_bloodtiesfancom.py
+-rw-rw-rw-   0        0        0    11404 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_buffygilescom.py
+-rw-rw-rw-   0        0        0     8756 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_chaossycophanthexcom.py
+-rw-rw-rw-   0        0        0     3855 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_chireadscom.py
+-rw-rw-rw-   0        0        0     9557 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_chosentwofanficcom.py
+-rw-rw-rw-   0        0        0     8847 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_csiforensicscom.py
+-rw-rw-rw-   0        0        0     1954 2021-02-03 15:44:28.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_darksolaceorg.py
+-rw-rw-rw-   0        0        0     8967 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_destinysgatewaycom.py
+-rw-rw-rw-   0        0        0     6949 2021-11-19 16:12:35.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_deviantartcom.py
+-rw-rw-rw-   0        0        0    10426 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_dokugacom.py
+-rw-rw-rw-   0        0        0    11384 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_dracoandginnycom.py
+-rw-rw-rw-   0        0        0    12348 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_efpfanficnet.py
+-rw-rw-rw-   0        0        0     9377 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_erosnsapphosycophanthexcom.py
+-rw-rw-rw-   0        0        0    12401 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_fanficauthorsnet.py
+-rw-rw-rw-   0        0        0     7024 2021-09-28 17:51:47.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_fanfichu.py
+-rw-rw-rw-   0        0        0    14662 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_fanficsme.py
+-rw-rw-rw-   0        0        0     9371 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_fanfictalkcom.py
+-rw-rw-rw-   0        0        0    17458 2021-09-19 17:49:46.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_fanfictionnet.py
+-rw-rw-rw-   0        0        0     8894 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_fanfiktionde.py
+-rw-rw-rw-   0        0        0     5078 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_fastnovelnet.py
+-rw-rw-rw-   0        0        0     9418 2021-11-09 14:53:20.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_ficbooknet.py
+-rw-rw-rw-   0        0        0     9280 2021-10-27 18:34:30.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_fictionalleyarchiveorg.py
+-rw-rw-rw-   0        0        0     9437 2022-01-04 15:49:10.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_fictionhuntcom.py
+-rw-rw-rw-   0        0        0    25264 2021-09-17 02:51:53.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_fictionlive.py
+-rw-rw-rw-   0        0        0     7883 2021-09-17 02:51:53.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_fictionmaniatv.py
+-rw-rw-rw-   0        0        0     1768 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_fictionpresscom.py
+-rw-rw-rw-   0        0        0     9080 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_ficwadcom.py
+-rw-rw-rw-   0        0        0    20025 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_fimfictionnet.py
+-rw-rw-rw-   0        0        0     2237 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_finestoriescom.py
+-rw-rw-rw-   0        0        0     7515 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_fireflyfansnet.py
+-rw-rw-rw-   0        0        0     1735 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_forumquestionablequestingcom.py
+-rw-rw-rw-   0        0        0     1726 2021-02-03 15:44:28.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_forumsspacebattlescom.py
+-rw-rw-rw-   0        0        0     1894 2021-02-03 15:44:28.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_forumssufficientvelocitycom.py
+-rw-rw-rw-   0        0        0     1874 2021-02-03 15:44:28.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_gluttonyfictioncom.py
+-rw-rw-rw-   0        0        0     7237 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_hentaifoundrycom.py
+-rw-rw-rw-   0        0        0     8526 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_hlfictionnet.py
+-rw-rw-rw-   0        0        0     9052 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_hpfanficarchivecom.py
+-rw-rw-rw-   0        0        0    10642 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_iketernalnet.py
+-rw-rw-rw-   0        0        0    10909 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_imagineeficcom.py
+-rw-rw-rw-   0        0        0     7925 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_inkbunnynet.py
+-rw-rw-rw-   0        0        0    13928 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_ksarchivecom.py
+-rw-rw-rw-   0        0        0     7548 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_lcfanficcom.py
+-rw-rw-rw-   0        0        0     1196 2021-02-03 15:44:28.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_libraryofmoriacom.py
+-rw-rw-rw-   0        0        0    19048 2021-09-17 02:51:53.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_literotica.py
+-rw-rw-rw-   0        0        0     1865 2021-06-27 15:03:30.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_looselugscom.py
+-rw-rw-rw-   0        0        0    14950 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_lotrgficcom.py
+-rw-rw-rw-   0        0        0     8756 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_lumossycophanthexcom.py
+-rw-rw-rw-   0        0        0    28595 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_masseffect2in.py
+-rw-rw-rw-   0        0        0     6456 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_mcstoriescom.py
+-rw-rw-rw-   0        0        0     8576 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_mediaminerorg.py
+-rw-rw-rw-   0        0        0    11146 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_merlinficdtwinscouk.py
+-rw-rw-rw-   0        0        0    11916 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_midnightwhispers.py
+-rw-rw-rw-   0        0        0     1205 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_mttjustoncenet.py
+-rw-rw-rw-   0        0        0     1179 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_mugglenetfanfictioncom.py
+-rw-rw-rw-   0        0        0     1084 2021-02-03 15:44:28.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_naiceanilmenet.py
+-rw-rw-rw-   0        0        0     1114 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_narutoficorg.py
+-rw-rw-rw-   0        0        0     1344 2021-02-03 15:44:28.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_ncisfictioncom.py
+-rw-rw-rw-   0        0        0     1754 2021-02-03 15:44:28.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_ninelivesarchivecom.py
+-rw-rw-rw-   0        0        0     3421 2021-11-20 21:21:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_novelfull.py
+-rw-rw-rw-   0        0        0     8115 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_novelonlinefullcom.py
+-rw-rw-rw-   0        0        0     6204 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_noveltrovecom.py
+-rw-rw-rw-   0        0        0     1512 2021-02-03 15:44:28.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_novelupdatescc.py
+-rw-rw-rw-   0        0        0     9436 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_occlumencysycophanthexcom.py
+-rw-rw-rw-   0        0        0     8827 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_phoenixsongnet.py
+-rw-rw-rw-   0        0        0    10124 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_ponyfictionarchivenet.py
+-rw-rw-rw-   0        0        0     8868 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_potionsandsnitches.py
+-rw-rw-rw-   0        0        0    11273 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_potterheadsanonymouscom.py
+-rw-rw-rw-   0        0        0     9461 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_pretendercentrecom.py
+-rw-rw-rw-   0        0        0     8461 2021-11-14 18:00:24.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_psychficcom.py
+-rw-rw-rw-   0        0        0     9924 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_qafficcom.py
+-rw-rw-rw-   0        0        0     5716 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_quotevcom.py
+-rw-rw-rw-   0        0        0     9685 2021-11-02 01:00:56.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_royalroadcom.py
+-rw-rw-rw-   0        0        0    13567 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_samandjacknet.py
+-rw-rw-rw-   0        0        0    10039 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_scarvesandcoffeenet.py
+-rw-rw-rw-   0        0        0     1324 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_scifistoriescom.py
+-rw-rw-rw-   0        0        0    15632 2021-12-10 16:11:39.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_scribblehubcom.py
+-rw-rw-rw-   0        0        0    12713 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_sheppardweircom.py
+-rw-rw-rw-   0        0        0    11378 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_shriftweborgbfa.py
+-rw-rw-rw-   0        0        0    12041 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_silmarillionwritersguildorg.py
+-rw-rw-rw-   0        0        0     1401 2021-02-03 15:44:29.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_sinfuldreamscomunicornfic.py
+-rw-rw-rw-   0        0        0     1410 2021-02-03 15:44:29.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_sinfuldreamscomwhisperedmuse.py
+-rw-rw-rw-   0        0        0     1419 2021-02-03 15:44:29.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_sinfuldreamscomwickedtemptation.py
+-rw-rw-rw-   0        0        0     9945 2021-09-17 02:51:53.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_siyecouk.py
+-rw-rw-rw-   0        0        0     1375 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_spikeluvercom.py
+-rw-rw-rw-   0        0        0     1712 2021-02-03 15:44:29.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_squidgeworldorg.py
+-rw-rw-rw-   0        0        0     1145 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_starskyhutcharchivenet.py
+-rw-rw-rw-   0        0        0     1892 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_starslibrarynet.py
+-rw-rw-rw-   0        0        0     6120 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_storiesofardacom.py
+-rw-rw-rw-   0        0        0    27163 2021-11-13 01:21:10.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_storiesonlinenet.py
+-rw-rw-rw-   0        0        0     7710 2021-09-17 02:51:53.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_sugarquillnet.py
+-rw-rw-rw-   0        0        0     5695 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_swiorgru.py
+-rw-rw-rw-   0        0        0     1118 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_swordborderlineangelcom.py
+-rw-rw-rw-   0        0        0     1266 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_tasteofpoisoninkubationnet.py
+-rw-rw-rw-   0        0        0     9210 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_tenhawkpresents.py
+-rw-rw-rw-   0        0        0    24138 2021-12-11 23:49:24.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_test1.py
+-rw-rw-rw-   0        0        0     1082 2021-02-03 15:44:29.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_tgstorytimecom.py
+-rw-rw-rw-   0        0        0     1481 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_thedelphicexpansecom.py
+-rw-rw-rw-   0        0        0     1363 2021-02-03 15:44:29.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_thehookupzonenet.py
+-rw-rw-rw-   0        0        0     1222 2021-02-03 15:44:29.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_themaplebookshelf.py
+-rw-rw-rw-   0        0        0    10243 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_themasquenet.py
+-rw-rw-rw-   0        0        0     1984 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_thesietchcom.py
+-rw-rw-rw-   0        0        0     7869 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_tomparisdormcom.py
+-rw-rw-rw-   0        0        0     8908 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_trekfanfictionnet.py
+-rw-rw-rw-   0        0        0    12841 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_trekiverseorg.py
+-rw-rw-rw-   0        0        0    17176 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_tthfanficorg.py
+-rw-rw-rw-   0        0        0     9255 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_twilightednet.py
+-rw-rw-rw-   0        0        0     2017 2021-06-27 15:03:40.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_valentchambercom.py
+-rw-rw-rw-   0        0        0     9278 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_voracity2eficcom.py
+-rw-rw-rw-   0        0        0     8748 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_walkingtheplankorg.py
+-rw-rw-rw-   0        0        0     6795 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_wattpadcom.py
+-rw-rw-rw-   0        0        0     9329 2021-11-19 16:22:20.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_webnovelcom.py
+-rw-rw-rw-   0        0        0    10615 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_whoficcom.py
+-rw-rw-rw-   0        0        0     8176 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_wolverineandroguecom.py
+-rw-rw-rw-   0        0        0     2097 2021-09-17 02:51:53.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_worldofxde.py
+-rw-rw-rw-   0        0        0     8787 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_wraithbaitcom.py
+-rw-rw-rw-   0        0        0     5499 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_wuxiaworldco.py
+-rw-rw-rw-   0        0        0     4842 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_wuxiaworldcom.py
+-rw-rw-rw-   0        0        0     6313 2021-11-28 18:31:14.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_wuxiaworldsite.py
+-rw-rw-rw-   0        0        0     5534 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_wwwaneroticstorycom.py
+-rw-rw-rw-   0        0        0     1319 2021-02-03 15:44:29.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_wwwgiantessworldnet.py
+-rw-rw-rw-   0        0        0    11650 2021-09-28 17:35:34.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_wwwlushstoriescom.py
+-rw-rw-rw-   0        0        0    11732 2021-12-03 16:56:37.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_wwwnovelallcom.py
+-rw-rw-rw-   0        0        0     9265 2021-10-24 14:39:42.000000 FanFicFare-4.9.0/fanficfare/adapters/adapter_wwwutopiastoriescom.py
+-rw-rw-rw-   0        0        0    38877 2021-12-12 01:31:37.000000 FanFicFare-4.9.0/fanficfare/adapters/base_adapter.py
+-rw-rw-rw-   0        0        0    19046 2021-12-12 01:27:29.000000 FanFicFare-4.9.0/fanficfare/adapters/base_efiction_adapter.py
+-rw-rw-rw-   0        0        0    13510 2021-09-17 02:51:53.000000 FanFicFare-4.9.0/fanficfare/adapters/base_xenforo2forum_adapter.py
+-rw-rw-rw-   0        0        0    38672 2021-09-17 02:51:53.000000 FanFicFare-4.9.0/fanficfare/adapters/base_xenforoforum_adapter.py
+drwxrwxrwx   0        0        0        0 2022-01-11 22:02:21.914352 FanFicFare-4.9.0/fanficfare/browsercache/
+-rw-rw-rw-   0        0        0     1460 2021-07-12 17:23:33.000000 FanFicFare-4.9.0/fanficfare/browsercache/__init__.py
+-rw-rw-rw-   0        0        0     8965 2021-11-20 21:50:25.000000 FanFicFare-4.9.0/fanficfare/browsercache/basebrowsercache.py
+-rw-rw-rw-   0        0        0     5294 2021-09-17 02:51:53.000000 FanFicFare-4.9.0/fanficfare/browsercache/blockfilecache.py
+drwxrwxrwx   0        0        0        0 2022-01-11 22:02:21.929978 FanFicFare-4.9.0/fanficfare/browsercache/chromagnon/
+-rw-rw-rw-   0        0        0     3357 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/browsercache/chromagnon/SuperFastHash.py
+-rw-rw-rw-   0        0        0        0 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/browsercache/chromagnon/__init__.py
+-rw-rw-rw-   0        0        0     3797 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/browsercache/chromagnon/cacheAddress.py
+-rw-rw-rw-   0        0        0     3117 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/browsercache/chromagnon/cacheAddressTest.py
+-rw-rw-rw-   0        0        0     4094 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/browsercache/chromagnon/cacheBlock.py
+-rw-rw-rw-   0        0        0     5398 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/browsercache/chromagnon/cacheData.py
+-rw-rw-rw-   0        0        0     7093 2021-09-17 02:51:53.000000 FanFicFare-4.9.0/fanficfare/browsercache/chromagnon/cacheEntry.py
+-rw-rw-rw-   0        0        0     9165 2021-09-17 02:51:53.000000 FanFicFare-4.9.0/fanficfare/browsercache/firefoxcache2.py
+-rw-rw-rw-   0        0        0     2672 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/browsercache/share_open.py
+-rw-rw-rw-   0        0        0     8997 2021-09-17 02:51:53.000000 FanFicFare-4.9.0/fanficfare/browsercache/simplecache.py
+-rw-rw-rw-   0        0        0    32103 2022-01-11 21:58:16.000000 FanFicFare-4.9.0/fanficfare/cli.py
+-rw-rw-rw-   0        0        0    48849 2021-12-12 01:26:20.000000 FanFicFare-4.9.0/fanficfare/configurable.py
+-rw-rw-rw-   0        0        0     3541 2021-09-17 02:51:53.000000 FanFicFare-4.9.0/fanficfare/dateutils.py
+-rw-rw-rw-   0        0        0   148738 2022-01-10 15:06:57.000000 FanFicFare-4.9.0/fanficfare/defaults.ini
+-rw-rw-rw-   0        0        0    21658 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/epubutils.py
+-rw-rw-rw-   0        0        0     2924 2021-09-17 02:51:53.000000 FanFicFare-4.9.0/fanficfare/example.ini
+-rw-rw-rw-   0        0        0     4032 2021-07-08 22:31:58.000000 FanFicFare-4.9.0/fanficfare/exceptions.py
+-rw-rw-rw-   0        0        0    22287 2021-10-03 01:53:00.000000 FanFicFare-4.9.0/fanficfare/fetcher.py
+-rw-rw-rw-   0        0        0    10452 2021-11-03 19:55:14.000000 FanFicFare-4.9.0/fanficfare/flaresolverr_proxy.py
+-rw-rw-rw-   0        0        0    14105 2021-10-16 20:29:16.000000 FanFicFare-4.9.0/fanficfare/geturls.py
+-rw-rw-rw-   0        0        0    17240 2021-02-03 15:44:30.000000 FanFicFare-4.9.0/fanficfare/htmlcleanup.py
+-rw-rw-rw-   0        0        0    15618 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/htmlheuristics.py
+-rw-rw-rw-   0        0        0    13565 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/mobi.py
+-rw-rw-rw-   0        0        0     5735 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/mobihtml.py
+-rw-rw-rw-   0        0        0     6978 2021-09-17 02:51:53.000000 FanFicFare-4.9.0/fanficfare/nsapa_proxy.py
+-rw-rw-rw-   0        0        0     5130 2021-10-16 19:41:28.000000 FanFicFare-4.9.0/fanficfare/requestable.py
+-rw-rw-rw-   0        0        0    35181 2021-02-03 15:44:30.000000 FanFicFare-4.9.0/fanficfare/six.py
+-rw-rw-rw-   0        0        0    64175 2021-11-20 02:17:12.000000 FanFicFare-4.9.0/fanficfare/story.py
+-rw-rw-rw-   0        0        0     2914 2021-02-03 15:44:30.000000 FanFicFare-4.9.0/fanficfare/translit.py
+drwxrwxrwx   0        0        0        0 2022-01-11 22:02:21.945605 FanFicFare-4.9.0/fanficfare/writers/
+-rw-rw-rw-   0        0        0     1381 2021-02-03 15:44:30.000000 FanFicFare-4.9.0/fanficfare/writers/__init__.py
+-rw-rw-rw-   0        0        0    10348 2021-07-05 01:10:06.000000 FanFicFare-4.9.0/fanficfare/writers/base_writer.py
+-rw-rw-rw-   0        0        0    40425 2021-09-17 02:51:53.000000 FanFicFare-4.9.0/fanficfare/writers/writer_epub.py
+-rw-rw-rw-   0        0        0     5925 2021-09-17 02:51:53.000000 FanFicFare-4.9.0/fanficfare/writers/writer_html.py
+-rw-rw-rw-   0        0        0     6673 2021-09-17 02:51:53.000000 FanFicFare-4.9.0/fanficfare/writers/writer_mobi.py
+-rw-rw-rw-   0        0        0     5897 2021-09-17 02:51:53.000000 FanFicFare-4.9.0/fanficfare/writers/writer_txt.py
+-rw-rw-rw-   0        0        0       42 2022-01-11 22:02:21.945605 FanFicFare-4.9.0/setup.cfg
+-rw-rw-rw-   0        0        0     4622 2022-01-11 21:58:16.000000 FanFicFare-4.9.0/setup.py
```

### Comparing `FanFicFare-4.8.0/FanFicFare.egg-info/PKG-INFO` & `FanFicFare-4.9.0/FanFicFare.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FanFicFare
-Version: 4.8.0
+Version: 4.9.0
 Summary: A tool for downloading fanfiction to eBook formats
 Home-page: https://github.com/JimmXinu/FanFicFare
 Author: Jim Miller
 Author-email: retiefjimm@gmail.com
 License: Apache License
 Keywords: fanfiction download ebook epub html
 Platform: UNKNOWN
```

### Comparing `FanFicFare-4.8.0/FanFicFare.egg-info/SOURCES.txt` & `FanFicFare-4.9.0/FanFicFare.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/LICENSE` & `FanFicFare-4.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/PKG-INFO` & `FanFicFare-4.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FanFicFare
-Version: 4.8.0
+Version: 4.9.0
 Summary: A tool for downloading fanfiction to eBook formats
 Home-page: https://github.com/JimmXinu/FanFicFare
 Author: Jim Miller
 Author-email: retiefjimm@gmail.com
 License: Apache License
 Keywords: fanfiction download ebook epub html
 Platform: UNKNOWN
```

### Comparing `FanFicFare-4.8.0/README.md` & `FanFicFare-4.9.0/README.md`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/HtmlTagStack.py` & `FanFicFare-4.9.0/fanficfare/HtmlTagStack.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/__init__.py` & `FanFicFare-4.9.0/fanficfare/__init__.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/__init__.py` & `FanFicFare-4.9.0/fanficfare/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_adastrafanficcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_adastrafanficcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_adultfanfictionorg.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_adultfanfictionorg.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_alternatehistorycom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_alternatehistorycom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_andromedawebcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_andromedawebcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_archiveofourownorg.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_archiveofourownorg.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,16 @@
 
     @classmethod
     def get_section_url(cls,url):
         ## minimal URL used for section names in INI and reject list
         ## for comparison
         # logger.debug("pre--url:%s"%url)
         ## https://archiveofourown.org/works/19334905/chapters/71697933
-        url = re.sub(r'^(.*/works/\d+).*$',r'\1',url)
+        # http://archiveofourown.org/works/34686793/chapters/89043733
+        url = re.sub(r'^https?://(.*/works/\d+).*$',r'https://\1',url)
         # logger.debug("post-url:%s"%url)
         return url
 
     ## Login
     def needToLoginCheck(self, data):
         if 'This work is only available to registered users of the Archive.' in data \
                 or "The password or user name you entered doesn't match our records" in data:
```

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_archiveskyehawkecom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_archiveskyehawkecom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_asexstoriescom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_asexstoriescom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_ashwindersycophanthexcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_ashwindersycophanthexcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_asianfanficscom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_asianfanficscom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_bdsmlibrarycom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_bdsmlibrarycom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_bloodshedversecom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_bloodshedversecom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_bloodtiesfancom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_bloodtiesfancom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_buffygilescom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_buffygilescom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_chaossycophanthexcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_chaossycophanthexcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_chireadscom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_chireadscom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_chosentwofanficcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_chosentwofanficcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_csiforensicscom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_csiforensicscom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_darksolaceorg.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_darksolaceorg.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_destinysgatewaycom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_destinysgatewaycom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_deviantartcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_deviantartcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_dokugacom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_dokugacom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_dracoandginnycom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_dracoandginnycom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_efpfanficnet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_efpfanficnet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_erosnsapphosycophanthexcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_erosnsapphosycophanthexcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_fanficauthorsnet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_fanficauthorsnet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_fanfichu.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_fanfichu.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_fanficsme.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_fanficsme.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_fanfictalkcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_fanfictalkcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_fanfictionnet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_fanfictionnet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_fanfiktionde.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_fanfiktionde.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_fastnovelnet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_fastnovelnet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_ficbooknet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_ficbooknet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_fictionalleyarchiveorg.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_fictionalleyarchiveorg.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_fictionhuntcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_fictionhuntcom.py`

 * *Files 0% similar despite different names*

```diff
@@ -119,17 +119,19 @@
 
         # fetch the chapter.  From that we will get almost all the
         # metadata and chapter list
 
         url = self.url
         data = self.get_request(url)
 
-        if self.needToLoginCheck(data):
-            self.performLogin(url)
-            data = self.get_request(url,usecache=False)
+        ## As per #784, site isn't requiring login anymore.
+        ## Login check commented since we've seen it toggle before.
+        # if self.needToLoginCheck(data):
+        #     self.performLogin(url)
+        #     data = self.get_request(url,usecache=False)
 
         soup = self.make_soup(data)
         ## detect old storyUrl, switch to new storyUrl:
         canonlink = soup.find('link',rel='canonical')
         if canonlink:
             # logger.debug(canonlink)
             canonlink = re.sub(r"/chapters/\d+","",canonlink['href'])
```

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_fictionlive.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_fictionlive.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_fictionmaniatv.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_fictionmaniatv.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_fictionpresscom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_fictionpresscom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_ficwadcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_ficwadcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_fimfictionnet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_fimfictionnet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_finestoriescom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_finestoriescom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_fireflyfansnet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_fireflyfansnet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_forumquestionablequestingcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_forumquestionablequestingcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_forumsspacebattlescom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_forumsspacebattlescom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_forumssufficientvelocitycom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_forumssufficientvelocitycom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_gluttonyfictioncom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_gluttonyfictioncom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_hentaifoundrycom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_hentaifoundrycom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_hlfictionnet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_hlfictionnet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_hpfanficarchivecom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_hpfanficarchivecom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_iketernalnet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_iketernalnet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_imagineeficcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_imagineeficcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_inkbunnynet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_inkbunnynet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_ksarchivecom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_ksarchivecom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_lcfanficcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_lcfanficcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_libraryofmoriacom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_libraryofmoriacom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_literotica.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_literotica.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_looselugscom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_looselugscom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_lotrgficcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_lotrgficcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_lumossycophanthexcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_lumossycophanthexcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_masseffect2in.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_masseffect2in.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_mcstoriescom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_mcstoriescom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_mediaminerorg.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_mediaminerorg.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_merlinficdtwinscouk.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_merlinficdtwinscouk.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_midnightwhispers.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_midnightwhispers.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_mttjustoncenet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_mttjustoncenet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_mugglenetfanfictioncom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_mugglenetfanfictioncom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_naiceanilmenet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_naiceanilmenet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_narutoficorg.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_narutoficorg.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_ncisfictioncom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_ncisfictioncom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_ninelivesarchivecom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_ninelivesarchivecom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_novelfull.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_novelfull.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_novelonlinefullcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_novelonlinefullcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_noveltrovecom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_noveltrovecom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_novelupdatescc.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_novelupdatescc.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_occlumencysycophanthexcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_occlumencysycophanthexcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_phoenixsongnet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_phoenixsongnet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_ponyfictionarchivenet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_ponyfictionarchivenet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_potionsandsnitches.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_potionsandsnitches.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_potterheadsanonymouscom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_potterheadsanonymouscom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_pretendercentrecom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_pretendercentrecom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_psychficcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_psychficcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_qafficcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_qafficcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_quotevcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_quotevcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_royalroadcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_royalroadcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_samandjacknet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_samandjacknet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_scarvesandcoffeenet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_scarvesandcoffeenet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_scifistoriescom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_scifistoriescom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_scribblehubcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_scribblehubcom.py`

 * *Files 1% similar despite different names*

```diff
@@ -329,15 +329,17 @@
                     new_tag = soup.new_tag('b')
                     new_tag.string = spoiler_title.get_text()
                     spoiler_div.append(new_tag)
 
                 spoiler_body = spoiler.find('div', {'class' : 'sp-body'})
                 if spoiler_body:
                     # Remove [collapse] text
-                    spoiler_body.find('div', {'class' : 'spdiv'}).decompose()
+                    spdiv = spoiler_body.find('div', {'class' : 'spdiv'})
+                    if spdiv: # saw one with no spdiv tag.
+                        spdiv.decompose()
 
                     new_tag = soup.new_tag('blockquote')
                     new_tag.append(spoiler_body)
                     spoiler_div.append(new_tag)
 
                 # Clear old children from the spoiler box, then add this
                 spoiler.clear()
```

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_sheppardweircom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_sheppardweircom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_shriftweborgbfa.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_shriftweborgbfa.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_silmarillionwritersguildorg.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_silmarillionwritersguildorg.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_sinfuldreamscomunicornfic.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_sinfuldreamscomunicornfic.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_sinfuldreamscomwhisperedmuse.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_sinfuldreamscomwhisperedmuse.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_sinfuldreamscomwickedtemptation.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_sinfuldreamscomwickedtemptation.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_siyecouk.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_siyecouk.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_spikeluvercom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_spikeluvercom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_squidgeworldorg.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_squidgeworldorg.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_starskyhutcharchivenet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_starskyhutcharchivenet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_starslibrarynet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_starslibrarynet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_storiesofardacom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_storiesofardacom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_storiesonlinenet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_storiesonlinenet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_sugarquillnet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_sugarquillnet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_swiorgru.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_swiorgru.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_swordborderlineangelcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_swordborderlineangelcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_tasteofpoisoninkubationnet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_tasteofpoisoninkubationnet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_tenhawkpresents.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_tenhawkpresents.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_test1.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_test1.py`

 * *Files 0% similar despite different names*

```diff
@@ -391,23 +391,23 @@
             for tag in bq.find_all('div', class_="bbCodeBlock-expandContent"):
                 tag.name='blockquote'
 
             return self.utf8FromSoup(url[:url.index('/',8)+1],bq)
 
         else:
             text=u'''
-<div>
+<div class='chapter'>
 <h3 extra="value">Chapter title from site</h3>
 <style>
  p { color: red; }
  body { color:blue; margin: 5%; }
 </style>
 <p>chapter URL:'''+url+'''</p>
 <p style="color:blue;">Timestamp:'''+datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")+'''</p>
-<p>Lorem '''+self.crazystring+u''' <i>italics</i>, <b>bold</b>, <u>underline</u>, <s>Strike through</s> consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
+<p class='chapter ptag'>Lorem '''+self.crazystring+u''' <i>italics</i>, <b>bold</b>, <u>underline</u>, <s>Strike through</s> consectetur adipisicing elit, sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip ex ea commodo consequat. Duis aute irure dolor in reprehenderit in voluptate velit esse cillum dolore eu fugiat nulla pariatur. Excepteur sint occaecat cupidatat non proident, sunt in culpa qui officia deserunt mollit anim id est laborum.</p>
 br breaks<br><br>
 Puella Magi Madoka Magica/魔法少女まどか★マギカ
 <!-- a href="http://code.google.com/p/fanficdownloader/wiki/FanFictionDownLoaderPluginWithReadingList" title="Tilt-a-Whirl by Jim &amp; Sarah, on Flickr"><img src="http://i.imgur.com/bo8eD.png"></a --><br/>
 br breaks<br><br>
 Don't&#8212e;ver&#8212d;o&#8212;that&#8212a;gain, &#27861; &#xE9;
 <hr>
 horizontal rules
```

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_tgstorytimecom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_tgstorytimecom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_thedelphicexpansecom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_thedelphicexpansecom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_thehookupzonenet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_thehookupzonenet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_themaplebookshelf.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_themaplebookshelf.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_themasquenet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_themasquenet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_thesietchcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_thesietchcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_tomparisdormcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_tomparisdormcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_trekfanfictionnet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_trekfanfictionnet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_trekiverseorg.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_trekiverseorg.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_tthfanficorg.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_tthfanficorg.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_twilightednet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_twilightednet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_valentchambercom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_valentchambercom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_voracity2eficcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_voracity2eficcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_walkingtheplankorg.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_walkingtheplankorg.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_wattpadcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_wattpadcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_webnovelcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_webnovelcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_whoficcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_whoficcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_wolverineandroguecom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_wolverineandroguecom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_worldofxde.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_worldofxde.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_wraithbaitcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_wraithbaitcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_wuxiaworldco.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_wuxiaworldco.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_wuxiaworldcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_wuxiaworldcom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_wuxiaworldsite.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_wuxiaworldsite.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_wwwaneroticstorycom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_wwwaneroticstorycom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_wwwgiantessworldnet.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_wwwgiantessworldnet.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_wwwlushstoriescom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_wwwlushstoriescom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_wwwnovelallcom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_wwwnovelallcom.py`

 * *Files 2% similar despite different names*

```diff
@@ -200,26 +200,33 @@
         ## getting tags
         tags = soup.find('span', string='Tag(s):')
         if tags:
             for a in tags.find_next_siblings("a"):
                 self.story.addToList('sitetags', a.string)
 
         ## getting description
-        self.setDescription(url, soup.select_one('#show').string.strip())
+        descdiv = soup.select_one('#show')
+        if descdiv:
+            # remove style="display: none"
+            del descdiv['style']
+            self.setDescription(url, descdiv)
 
         ## getting cover
         img = soup.find('img', class_='detail-cover')
         if img:
             self.setCoverImage(url,img['src'])
 
         ## getting chapters
         cdata = soup.select('.detail-chlist li')
         cdata.reverse()
-        cdates = []
+        if not cdata: # user found a story with no chapters.
+            raise exceptions.FailedToDownload(
+                "Story has no chapters: %s" % url)
 
+        cdates = []
         for li in cdata:
             # <span class="time">31 minutes ago</span>s
             # <span class="time">Jul 15, 2017</span>
             dt = li.select_one('.time').string
             if "ago" in dt:
                 cdates.append(parse_relative_date_string(dt))
             else:
```

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/adapter_wwwutopiastoriescom.py` & `FanFicFare-4.9.0/fanficfare/adapters/adapter_wwwutopiastoriescom.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/base_adapter.py` & `FanFicFare-4.9.0/fanficfare/adapters/base_adapter.py`

 * *Files 1% similar despite different names*

```diff
@@ -588,14 +588,26 @@
         self.times.add("utf8FromSoup->copy", datetime.now() - start)
         ## _do_utf8FromSoup broken out to separate copy & timing and
         ## allow for inherit override.
         retval = self._do_utf8FromSoup(url,soup,fetch,allow_replace_br_with_p)
         self.times.add("utf8FromSoup", datetime.now() - start)
         return retval
 
+    def remove_class_chapter(self,soup):
+        def rm_chp_cls(t):
+            t['class'].remove('chapter')
+            if not t['class']: # remove if list empty now.
+                del t['class']
+        for t in soup.select('.chapter'):
+            rm_chp_cls(t)
+        # if soup is itself a tag with class='chapter', select doesn't
+        # find it.
+        if soup.has_attr('class') and 'chapter' in soup['class']:
+            rm_chp_cls(soup)
+
     def _do_utf8FromSoup(self,url,soup,fetch=None,allow_replace_br_with_p=True):
         if not fetch:
             fetch=self.get_request_raw
 
         acceptable_attributes = self.getConfigList('keep_html_attrs',['href','name','class','id','data-orighref'])
 
         if self.getConfig("keep_style_attr"):
@@ -620,14 +632,21 @@
             for img in soup.find_all('img'):
                 img.decompose()
 
         for attr in self.get_attr_keys(soup):
             if attr not in acceptable_attributes:
                 del soup[attr] ## strip all tag attributes except configured
 
+        ## some tags, notable chapter div from Base eFiction have
+        ## class='chapter', which causes calibre convert to id it as a
+        ## chapter and 'pagebreak' - AKA split the file.  Remove by
+        ## default, but only if class otherwise allowed (minor perf opt).
+        if 'class' in acceptable_attributes and self.getConfig('remove_class_chapter',True):
+            self.remove_class_chapter(soup)
+
         ## Make relative links in text into absolute links using page
         ## URL.
         if self.getConfig('fix_relative_text_links'):
             for alink in soup.find_all('a'):
                 if alink.has_attr('href'):
                     toppath=""
                     href = alink['href']
```

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/base_efiction_adapter.py` & `FanFicFare-4.9.0/fanficfare/adapters/base_efiction_adapter.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/base_xenforo2forum_adapter.py` & `FanFicFare-4.9.0/fanficfare/adapters/base_xenforo2forum_adapter.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/adapters/base_xenforoforum_adapter.py` & `FanFicFare-4.9.0/fanficfare/adapters/base_xenforoforum_adapter.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/browsercache/__init__.py` & `FanFicFare-4.9.0/fanficfare/browsercache/__init__.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/browsercache/basebrowsercache.py` & `FanFicFare-4.9.0/fanficfare/browsercache/basebrowsercache.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/browsercache/blockfilecache.py` & `FanFicFare-4.9.0/fanficfare/browsercache/blockfilecache.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/browsercache/chromagnon/SuperFastHash.py` & `FanFicFare-4.9.0/fanficfare/browsercache/chromagnon/SuperFastHash.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/browsercache/chromagnon/cacheAddress.py` & `FanFicFare-4.9.0/fanficfare/browsercache/chromagnon/cacheAddress.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/browsercache/chromagnon/cacheAddressTest.py` & `FanFicFare-4.9.0/fanficfare/browsercache/chromagnon/cacheAddressTest.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/browsercache/chromagnon/cacheBlock.py` & `FanFicFare-4.9.0/fanficfare/browsercache/chromagnon/cacheBlock.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/browsercache/chromagnon/cacheData.py` & `FanFicFare-4.9.0/fanficfare/browsercache/chromagnon/cacheData.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/browsercache/chromagnon/cacheEntry.py` & `FanFicFare-4.9.0/fanficfare/browsercache/chromagnon/cacheEntry.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/browsercache/firefoxcache2.py` & `FanFicFare-4.9.0/fanficfare/browsercache/firefoxcache2.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/browsercache/share_open.py` & `FanFicFare-4.9.0/fanficfare/browsercache/share_open.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/browsercache/simplecache.py` & `FanFicFare-4.9.0/fanficfare/browsercache/simplecache.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/cli.py` & `FanFicFare-4.9.0/fanficfare/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 import getpass
 import logging
 import pprint
 import string
 import os, sys, platform
 
 
-version="4.8.0"
+version="4.9.0"
 os.environ['CURRENT_VERSION_ID']=version
 
 global_cache = 'global_cache'
 global_cookies = 'global_cookies'
 
 if sys.version_info >= (2, 7):
     # suppresses default logger.  Logging is setup in fanficfare/__init__.py so it works in calibre, too.
@@ -60,26 +60,21 @@
         logger.info("Output suppressed by --no-output")
     else:
         writer.writeStory(outstream=outstream, metaonly=metaonly)
         logger.debug("Successfully wrote '%s'"%output_filename)
     del writer
     return output_filename
 
-def main(argv=None,
-         parser=None,
-         passed_defaultsini=None,
-         passed_personalini=None):
-    if argv is None:
-        argv = sys.argv[1:]
+def mkParser(calibre, parser=None):
     # read in args, anything starting with -- will be treated as --<varible>=<value>
     if not parser:
         parser = OptionParser('usage: %prog [options] [STORYURL]...')
     parser.add_option('-f', '--format', dest='format', default='epub',
                       help='Write story as FORMAT, epub(default), mobi, txt or html.', metavar='FORMAT')
-    if passed_defaultsini:
+    if calibre:
         config_help = 'calibre plugin defaults.ini, calibre plugin personal.ini'
     else:
         config_help = '~/.fanficfare/defaults.ini, $XDG_CONFIG_HOME/fanficfare/defaults.ini, ./defaults.ini'
     parser.add_option('-c', '--config',
                       action='append', dest='configfile', default=None,
                       help=('Read config from specified file(s) in addition to (ordered lowest to highest priority): '
                             +config_help
@@ -142,117 +137,122 @@
                       action='store_true', dest='imaplist',
                       help='Get list of valid story URLs from unread email from IMAP account configured in ini.', )
 
     parser.add_option('--download-imap',
                       action='store_true', dest='downloadimap',
                       help='Download valid story URLs from unread email from IMAP account configured in ini.  Update existing EPUBs if used with --update-epub.', )
 
+    def sitesList(*args):
+        for site, examples in adapters.getSiteExamples():
+            print('\n#### %s\nExample URLs:' % site)
+            for u in examples:
+                print('  * %s' % u)
+        sys.exit()
+
     parser.add_option('-s', '--sites-list',
-                      action='store_true', dest='siteslist', default=False,
+                      action='callback', callback=sitesList,
                       help='Get list of valid story URLs examples.', )
     parser.add_option('--non-interactive',
                       action='store_false', dest='interactive', default=sys.stdin.isatty() and sys.stdout.isatty(),
                       help='Prevent interactive prompts (for scripting).', )
     parser.add_option('-d', '--debug',
                       action='store_true', dest='debug',
                       help='Show debug and notice output.', )
     parser.add_option('-p', '--progressbar',
                       action='store_true', dest='progressbar',
                       help='Display a simple progress bar while downloading--one dot(.) per network fetch.', )
     parser.add_option('--color',
                       action='store_true', dest='color',
                       help='Display a errors and warnings in a contrasting color.  Requires package colorama on Windows.', )
+
+    def printVersion(*args):
+        print("Version: %s" % version)
+        sys.exit()
+
     parser.add_option('-v', '--version',
-                      action='store_true', dest='version',
+                      action='callback', callback=printVersion,
                       help='Display version and quit.', )
 
     ## undocumented feature for development use.  Save page cache and
     ## cookies between runs.  Saves in PWD as files global_cache and
     ## global_cookies
     parser.add_option('--save-cache', '--save_cache',
                       action='store_true', dest='save_cache',
                       help=SUPPRESS_HELP, )
     ## 'undocumented' feature to allow expired/unverified SSL certs pass.
     ## removed in favor of use_ssl_unverified_context ini setting.
     parser.add_option('--unverified_ssl',
                       action='store_true', dest='unverified_ssl',
                       help=SUPPRESS_HELP, )
 
-    options, args = parser.parse_args(argv)
+    return parser
+
+def expandOptions(options):
+    options.list_only = any((options.imaplist,
+                             options.list,
+                             options.normalize,
+                             ))
 
+    # options.updatealways should also invoke most options.update logic.
+    if options.updatealways:
+        options.update = True
+
+def validateOptions(parser, options, args):
     if options.unverified_ssl:
-        print("Option --unverified_ssl removed.\nSet use_ssl_unverified_context:true in ini file or --option instead.")
-        return
+        parser.error("Option --unverified_ssl removed.\nSet use_ssl_unverified_context:true in ini file or --option instead.")
+
+    if options.list_only and (args or any((options.downloadimap,
+                                           options.downloadlist))):
+        parser.error('Incorrect arguments: Cannot download and list URLs at the same time.')
+
+    if options.update and options.format != 'epub':
+        parser.error('-u/--update-epub/-U/--update-epub-always only work with epub')
+
+    if options.unnew and options.format != 'epub':
+        parser.error('--unnew only works with epub')
+
+    if not options.list_only and not (args or any((options.infile,
+                                                   options.downloadimap,
+                                                   options.downloadlist))):
+        parser.print_help()
+        sys.exit()
 
+def setup(options):
     if not options.debug:
         logger.setLevel(logging.WARNING)
     else:
         logger.debug("    OS Version:%s"%platform.platform())
         logger.debug("Python Version:%s"%sys.version)
         logger.debug("   FFF Version:%s"%version)
 
-    if options.version:
-        print("Version: %s" % version)
-        return
-
     if options.color:
         if 'Windows' in platform.platform():
             try:
                 from colorama import init as colorama_init
                 colorama_init()
             except ImportError:
                 print("Option --color will not work on Windows without installing Python package colorama.\nContinue? (y/n)?")
                 if options.interactive:
                     if not sys.stdin.readline().strip().lower().startswith('y'):
-                        return
+                        sys.exit()
                     else:
                         # for non-interactive, default the response to yes and continue processing
                         print('y')
         def warn(t):
             print("\033[{}m{}\033[0m".format(34, t)) # blue
         def fail(t):
             print("\033[{}m{}\033[0m".format(31, t)) # red
     else:
         warn = fail = print
 
-    list_only = any((options.imaplist,
-                     options.siteslist,
-                     options.list,
-                     options.normalize,
-                     ))
-
-    if list_only and (args or any((options.downloadimap,
-                                   options.downloadlist))):
-        parser.error('Incorrect arguments: Cannot download and list URLs at the same time.')
-
-    if options.siteslist:
-        for site, examples in adapters.getSiteExamples():
-            print('\n#### %s\nExample URLs:' % site)
-            for u in examples:
-                print('  * %s' % u)
-        return
-
-    # options.updatealways should also invoke most options.update logic.
-    if options.updatealways:
-        options.update = True
-
-    if options.update and options.format != 'epub':
-        parser.error('-u/--update-epub/-U/--update-epub-always only work with epub')
-
-    if options.unnew and options.format != 'epub':
-        parser.error('--unnew only works with epub')
-
-    urls=args
-
-    if not list_only and not (args or any((options.infile,
-                                           options.downloadimap,
-                                           options.downloadlist))):
-        parser.print_help();
-        return
+    return warn, fail
 
+def dispatch(options, urls,
+             passed_defaultsini=None, passed_personalini=None,
+             warn=print, fail=print):
     if options.list:
         configuration = get_configuration(options.list,
                                           passed_defaultsini,
                                           passed_personalini,options)
         frompage = get_urls_from_page(options.list, configuration)
         if options.jsonmeta:
             import json
@@ -300,15 +300,15 @@
                 if '#' in url:
                     url = url[:url.find('#')].strip()
                 url = url.strip()
                 if len(url) > 0:
                     #print("url: (%s)"%url)
                     urls.append(url)
 
-    if not list_only:
+    if not options.list_only:
         if len(urls) < 1:
             print("No valid story URLs found")
         else:
             for url in urls:
                 try:
                     do_download(url,
                                 options,
@@ -317,14 +317,29 @@
                                 warn,
                                 fail)
                 except Exception as e:
                     if len(urls) == 1:
                         raise
                     fail("URL(%s) Failed: Exception (%s). Run URL individually for more detail."%(url,e))
 
+def main(argv=None,
+         parser=None,
+         passed_defaultsini=None,
+         passed_personalini=None):
+    if argv is None:
+        argv = sys.argv[1:]
+
+    parser = mkParser(bool(passed_defaultsini), parser)
+    options, args = parser.parse_args(argv)
+    expandOptions(options)
+    validateOptions(parser, options, args)
+    warn, fail = setup(options)
+    urls=args
+    dispatch(options, urls, passed_defaultsini, passed_personalini, warn, fail)
+
 # make rest a function and loop on it.
 def do_download(arg,
                 options,
                 passed_defaultsini,
                 passed_personalini,
                 warn=print,
                 fail=print):
```

### Comparing `FanFicFare-4.8.0/fanficfare/configurable.py` & `FanFicFare-4.9.0/fanficfare/configurable.py`

 * *Files 0% similar despite different names*

```diff
@@ -264,14 +264,15 @@
                'grayscale_images':(None,['epub','html'],boollist),
                'no_image_processing':(None,['epub','html'],boollist),
                'dedup_img_files':(None,['epub','html'],boollist),
                'convert_inline_images':(None,['epub','html'],boollist),
                'fix_relative_text_links':(None,['epub','html'],boollist),
                'normalize_text_links':(None,['epub','html'],boollist),
                'internalize_text_links':(None,['epub','html'],boollist),
+               'remove_class_chapter':(None,['epub','html'],boollist),
 
                'capitalize_forumtags':(base_xenforo_list,None,boollist),
                'minimum_threadmarks':(base_xenforo_list,None,None),
                'first_post_title':(base_xenforo_list,None,None),
                'always_include_first_post':(base_xenforo_list,None,boollist),
                'always_reload_first_chapter':(base_xenforo_list,None,boollist),
                'always_use_forumtags':(base_xenforo_list,None,boollist),
```

### Comparing `FanFicFare-4.8.0/fanficfare/dateutils.py` & `FanFicFare-4.9.0/fanficfare/dateutils.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/defaults.ini` & `FanFicFare-4.9.0/fanficfare/defaults.ini`

 * *Files 2% similar despite different names*

```diff
@@ -371,14 +371,23 @@
 ## internalize_text_links to preserve links when chapters are
 ## inserted.)
 ## Example: To add 'style', 'title' and 'align' to the list to keep,
 ## in your personal.ini [defaults] put:
 ## add_to_keep_html_attrs:,style,title,align
 keep_html_attrs:href,name,class,id,colspan,rowspan,data-orighref
 
+## Some tags, notable chapter div tags from Base eFiction, have
+## class='chapter', which causes calibre convert to identify it as a
+## chapter and 'pagebreak' at that point, aka split the file, which
+## adds unexpected pagebreaks and breaks FFF update if an epub to epub
+## conversion is done.  Remove class='chapter' from all tags by
+## default.  Also affects previously downloaded chapters on epub
+## update.
+remove_class_chapter:true
+
 ## Tags listed here will be replaced with <span class="tagname">.
 ## For example: <u>underlined text</u> becomes
 ## <span class="u">underlined text</span>
 ## Note that the output_css should contain the class .u, .big, etc for
 ## the spans to be useful.
 ## This feature is for replacing old tags deprecated/removed in newer
 ## HTML and EPUB standards.
@@ -511,41 +520,43 @@
 ## Chromium-derived) or Firefox browser's cache.  Requires both
 ## use_browser_cache:true and browser_cache_path to be set.
 ##
 ## browser_cache_path needs to be set to the location of YOUR browser
 ## cache.  Here are a few examples for different OS.  Note that all
 ## have YOUR user name in them somewhere as well as a Profile name,
 ## frequently Default.  Make sure you have personalized (and
-## uncommented) ONE browser_cache_path setting.
+## uncommented) ONE browser_cache_path setting.  Also note that Chrome
+## browsers added an additional directory level, 'Cache_Data', in
+## early 2022.
 
 ## Note also that browser_cache_path goes under [defaults] because
 ## browser cache is read once and shared between all downloads for
 ## performance.
 
 ## Further note that there is a time cost to first reading the browser
 ## cache on each download session (not Calibre session)
 
 ## windows:
 ### Chrome:
-#browser_cache_path:C:\Users\YourUser\AppData\Local\Google\Chrome\User Data\Default\Cache
-#browser_cache_path:C:\Users\YourUser\AppData\Local\Google\Chrome\User Data\Profile 1\Cache
+#browser_cache_path:C:\Users\YourUser\AppData\Local\Google\Chrome\User Data\Default\Cache\Cache_Data
+#browser_cache_path:C:\Users\YourUser\AppData\Local\Google\Chrome\User Data\Profile 1\Cache\Cache_Data
 ### Firefox
 #browser_cache_path:C:\Users\YourUser\AppData\Local\Mozilla\Firefox\Profiles\ZjwI7Fo4.default\cache2
 
 ## mac:
 ### Chrome:
-#browser_cache_path:/Users/your.user/Library/Caches/Google/Chrome/Default/Cache
-#browser_cache_path:/Users/your.user/Library/Caches/Google/Chrome/Profile 2/Cache
+#browser_cache_path:/Users/your.user/Library/Caches/Google/Chrome/Default/Cache/Cache_Data
+#browser_cache_path:/Users/your.user/Library/Caches/Google/Chrome/Profile 2/Cache/Cache_Data
 ### Firefox
 #browser_cache_path:/Users/your.user/Library/Caches/Firefox/Profiles/43fkezvc.default-release/cache2
 
 ## linux:
 ### Chrome:
-#browser_cache_path:/home/youruser/.cache/google-chrome/Default/Cache
-#browser_cache_path:/home/youruser/.cache/google-chrome/Profile 1/Cache
+#browser_cache_path:/home/youruser/.cache/google-chrome/Default/Cache/Cache_Data
+#browser_cache_path:/home/youruser/.cache/google-chrome/Profile 1/Cache/Cache_Data
 ### Firefox
 #browser_cache_path:/home/youruser/.cache/mozilla/firefox/dk4o1y83.default-release/cache2
 
 ## It's common for browser cached files to be kept for several hours
 ## or more.  You can limit the age of cached files FFF will use from
 ## browser_cache_path with browser_cache_age_limit.  Only cached files
 ## that were downloaded within 'browser_cache_age_limit' hours will be
@@ -699,36 +710,36 @@
 
 add_to_replace_metadata:
 # 'detects' if there are 'tags'. That is, [( in title.  Replaces
 # previous version's include_metadata_pre Can't do on tagsfromtitle
 # because that's applied to each part after split.
  tagsfromtitledetect=>^[^\]\)]+$=>
 # for QuestionableQuesting NSFW subforum.
- tagsfromtitle=>^\[NSFW\].*?([\(\[]([^\]\)]+)[\)\]]).*?$=>NSFW,\2
+ tagsfromtitle=>^\[NSFW\].*?(\[([^\]]+)\]|\(([^\)]+)\)).*?$=>NSFW\,\2\,\3
 # remove anything outside () or []
- tagsfromtitle=>^.*?([\(\[]([^\]\)]+)[\)\]]).*?$=>\2
+ tagsfromtitle=>^.*?(\[([^\]]+)\]|\(([^\)]+)\)).*?$=>\2\,\3
 # remove () []
 # tagsfromtitle=>[\(\)\[\]]=>
 # shield these html entities from the ';' pattern below
  tagsfromtitle=>&(amp|lt|gt);=>&\1FFF_ENT_MARKER
-# change (spaces)slash(or semicolon)(spaces) to comma
- tagsfromtitle=> *[/;|] *=>,
+# change (spaces)slash(or semicolon, pipe or comma)(spaces) to comma
+ tagsfromtitle=> *[/;|,] *=>,
 # revert html entities
  tagsfromtitle=>&(amp|lt|gt)FFF_ENT_MARKER=>&\1;
  tagsfromtitle=> [xX] =>,
 # split commas into individual list items.
 # these will work on up to 14 splits, should be plenty.
  tagsfromtitle=>([^,]+),([^,]+),([^,]+),([^,]+),([^,]+),(.+)=>\1\,\2\,\3,\4\,\5\,\6
  tagsfromtitle=>([^,]+),([^,]+),([^,]+),([^,]+),(.+)=>\1\,\2\,\3,\4\,\5
  tagsfromtitle=>([^,]+),([^,]+),([^,]+),(.+)=>\1\,\2\,\3,\4
  tagsfromtitle=>([^,]+),([^,]+),(.+)=>\1\,\2\,\3
  tagsfromtitle=>([^,]+),(.+)=>\1\,\2
 
 # remove [] or () blocks and leading/trailing spaces/dashes/colons
- title=>[-: ]*[\(\[]([^\]\)]+)[\)\]][-: ]*=>
+ title=>[-: ]*(\[([^\]]+)\]|\(([^\)]+)\))[-: ]*=>
 # remove 'Thread' and the next word, usually "Thread 2", "Thread
 # four", "Thread iv", "Story Thread", etc
  title,tagsfromtitle=>[-: ,]*(Story *)?[Tt]hread [^ ]+[-: ]*=>
 
 # Normalize 'fanfiction/fanfic/fan-fiction' a little.
  forumtags=>[Ff]an-?[Ff]ic(tion)?=>FanFiction
 
@@ -949,15 +960,15 @@
 
 [base_xenforo2forum]
 ## [base_xenforoforum] also applied, but [base_xenforo2forum] takes
 ## precedence.
 
 ## Some additional 'thread' metadata entries.
 add_to_extra_valid_entries:,threadmarks_title,threadmarks_description,threadmarks_status,estimatedWords
-add_to_extra_titlepage_entries:,threadmarks_title,threadmarks_description,threadmarks_status,estimatedWords
+#add_to_extra_titlepage_entries:,threadmarks_title,threadmarks_description,threadmarks_status,estimatedWords
 
 # Just to remove '_'.
 threadmarks_title_label:Threadmarks Title
 threadmarks_description_label:Threadmarks Description
 threadmarks_status_label:Threadmarks Status
 estimatedWords_label:Estimated Word Count
```

### Comparing `FanFicFare-4.8.0/fanficfare/epubutils.py` & `FanFicFare-4.9.0/fanficfare/epubutils.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/example.ini` & `FanFicFare-4.9.0/fanficfare/example.ini`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/exceptions.py` & `FanFicFare-4.9.0/fanficfare/exceptions.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/fetcher.py` & `FanFicFare-4.9.0/fanficfare/fetcher.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/flaresolverr_proxy.py` & `FanFicFare-4.9.0/fanficfare/flaresolverr_proxy.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/geturls.py` & `FanFicFare-4.9.0/fanficfare/geturls.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/htmlcleanup.py` & `FanFicFare-4.9.0/fanficfare/htmlcleanup.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/htmlheuristics.py` & `FanFicFare-4.9.0/fanficfare/htmlheuristics.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/mobi.py` & `FanFicFare-4.9.0/fanficfare/mobi.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/mobihtml.py` & `FanFicFare-4.9.0/fanficfare/mobihtml.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/nsapa_proxy.py` & `FanFicFare-4.9.0/fanficfare/nsapa_proxy.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/requestable.py` & `FanFicFare-4.9.0/fanficfare/requestable.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/six.py` & `FanFicFare-4.9.0/fanficfare/six.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/story.py` & `FanFicFare-4.9.0/fanficfare/story.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/translit.py` & `FanFicFare-4.9.0/fanficfare/translit.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/writers/__init__.py` & `FanFicFare-4.9.0/fanficfare/writers/__init__.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/writers/base_writer.py` & `FanFicFare-4.9.0/fanficfare/writers/base_writer.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/writers/writer_epub.py` & `FanFicFare-4.9.0/fanficfare/writers/writer_epub.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/writers/writer_html.py` & `FanFicFare-4.9.0/fanficfare/writers/writer_html.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/writers/writer_mobi.py` & `FanFicFare-4.9.0/fanficfare/writers/writer_mobi.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/fanficfare/writers/writer_txt.py` & `FanFicFare-4.9.0/fanficfare/writers/writer_txt.py`

 * *Files identical despite different names*

### Comparing `FanFicFare-4.8.0/setup.py` & `FanFicFare-4.9.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 with codecs.open('DESCRIPTION.rst', encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name=package_name,
 
     # Versions should comply with PEP440.
-    version="4.8.0",
+    version="4.9.0",
 
     description='A tool for downloading fanfiction to eBook formats',
     long_description=long_description,
 
     # The project's main homepage.
     url='https://github.com/JimmXinu/FanFicFare',
```

