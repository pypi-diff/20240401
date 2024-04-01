# Comparing `tmp/mteb-1.3.4.tar.gz` & `tmp/mteb-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mteb-1.3.4.tar", last modified: Mon Apr  1 08:50:58 2024, max compression
+gzip compressed data, was "mteb-1.4.0.tar", last modified: Mon Apr  1 12:08:00 2024, max compression
```

## Comparing `mteb-1.3.4.tar` & `mteb-1.4.0.tar`

### file list

```diff
@@ -1,370 +1,370 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.290385 mteb-1.3.4/
--rw-r--r--   0 root         (0) root         (0)    11357 2024-04-01 08:50:54.000000 mteb-1.3.4/LICENSE
--rw-r--r--   0 root         (0) root         (0)    23566 2024-04-01 08:50:58.286385 mteb-1.3.4/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     9190 2024-04-01 08:50:54.000000 mteb-1.3.4/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.230385 mteb-1.3.4/mteb/
--rw-r--r--   0 root         (0) root         (0)     1917 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.234385 mteb-1.3.4/mteb/abstasks/
--rw-r--r--   0 root         (0) root         (0)     1592 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/abstasks/AbsTask.py
--rw-r--r--   0 root         (0) root         (0)     3063 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/abstasks/AbsTaskBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5881 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/abstasks/AbsTaskClassification.py
--rw-r--r--   0 root         (0) root         (0)     2389 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/abstasks/AbsTaskClustering.py
--rw-r--r--   0 root         (0) root         (0)     2542 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/abstasks/AbsTaskPairClassification.py
--rw-r--r--   0 root         (0) root         (0)     1120 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/abstasks/AbsTaskReranking.py
--rw-r--r--   0 root         (0) root         (0)    11832 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/abstasks/AbsTaskRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2007 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/abstasks/AbsTaskSTS.py
--rw-r--r--   0 root         (0) root         (0)     2296 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/abstasks/AbsTaskSummarization.py
--rw-r--r--   0 root         (0) root         (0)      961 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/abstasks/CrosslingualTask.py
--rw-r--r--   0 root         (0) root         (0)     2831 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/abstasks/LangMapping.py
--rw-r--r--   0 root         (0) root         (0)     1052 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/abstasks/MultilingualTask.py
--rw-r--r--   0 root         (0) root         (0)     5356 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/abstasks/TaskMetadata.py
--rw-r--r--   0 root         (0) root         (0)      422 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/abstasks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5296 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/cmd.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.234385 mteb-1.3.4/mteb/evaluation/
--rw-r--r--   0 root         (0) root         (0)    13067 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/evaluation/MTEB.py
--rw-r--r--   0 root         (0) root         (0)       56 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/evaluation/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.238385 mteb-1.3.4/mteb/evaluation/evaluators/
--rw-r--r--   0 root         (0) root         (0)     5849 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/evaluation/evaluators/BitextMiningEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     8942 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/evaluation/evaluators/ClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1463 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/evaluation/evaluators/ClusteringEvaluator.py
--rw-r--r--   0 root         (0) root         (0)      744 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/evaluation/evaluators/Evaluator.py
--rw-r--r--   0 root         (0) root         (0)     7140 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/evaluation/evaluators/PairClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     9613 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/evaluation/evaluators/RerankingEvaluator.py
--rw-r--r--   0 root         (0) root         (0)    12487 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/evaluation/evaluators/RetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     2394 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/evaluation/evaluators/STSEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     4841 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/evaluation/evaluators/SummarizationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)      324 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/evaluation/evaluators/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5482 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/evaluation/evaluators/utils.py
--rw-r--r--   0 root         (0) root         (0)      835 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/logging.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.238385 mteb-1.3.4/mteb/tasks/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.238385 mteb-1.3.4/mteb/tasks/BitextMining/
--rw-r--r--   0 root         (0) root         (0)      369 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/BitextMining/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.238385 mteb-1.3.4/mteb/tasks/BitextMining/da/
--rw-r--r--   0 root         (0) root         (0)     1800 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/BitextMining/da/BornholmskBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/BitextMining/da/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.238385 mteb-1.3.4/mteb/tasks/BitextMining/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1040 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     2257 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     5808 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     1813 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py
--rw-r--r--   0 root         (0) root         (0)     2761 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/BitextMining/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.242385 mteb-1.3.4/mteb/tasks/BitextMining/nb/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/BitextMining/nb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1806 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/BitextMining/nb/norwegian_courts_bitext_mining.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.242385 mteb-1.3.4/mteb/tasks/Classification/
--rw-r--r--   0 root         (0) root         (0)     1232 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.242385 mteb-1.3.4/mteb/tasks/Classification/da/
--rw-r--r--   0 root         (0) root         (0)     1278 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/da/AngryTweetsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1978 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/da/DKHateClassification.py
--rw-r--r--   0 root         (0) root         (0)     2881 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/da/DalajClassification.py
--rw-r--r--   0 root         (0) root         (0)     1967 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/da/DanishPoliticalCommentsClassification.py
--rw-r--r--   0 root         (0) root         (0)     3303 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/da/DdiscoCohesionClassification.py
--rw-r--r--   0 root         (0) root         (0)     1217 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/da/LccSentimentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/da/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.242385 mteb-1.3.4/mteb/tasks/Classification/en/
--rw-r--r--   0 root         (0) root         (0)      999 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/en/AmazonPolarityClassification.py
--rw-r--r--   0 root         (0) root         (0)     1012 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/en/Banking77Classification.py
--rw-r--r--   0 root         (0) root         (0)     1330 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/en/EmotionClassification.py
--rw-r--r--   0 root         (0) root         (0)      948 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/en/ImdbClassification.py
--rw-r--r--   0 root         (0) root         (0)     1368 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/en/ToxicConversationsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1239 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/en/TweetSentimentExtractionClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.246385 mteb-1.3.4/mteb/tasks/Classification/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1447 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
--rw-r--r--   0 root         (0) root         (0)     1199 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
--rw-r--r--   0 root         (0) root         (0)     1128 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
--rw-r--r--   0 root         (0) root         (0)     1128 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1367 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py
--rw-r--r--   0 root         (0) root         (0)     1787 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py
--rw-r--r--   0 root         (0) root         (0)     1793 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py
--rw-r--r--   0 root         (0) root         (0)     1841 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/multilingual/NordicLangClassification.py
--rw-r--r--   0 root         (0) root         (0)     7434 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/multilingual/ScalaClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.246385 mteb-1.3.4/mteb/tasks/Classification/nb/
--rw-r--r--   0 root         (0) root         (0)     1063 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/nb/NoRecClassification.py
--rw-r--r--   0 root         (0) root         (0)     1124 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/nb/NorwegianParliamentClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/nb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.246385 mteb-1.3.4/mteb/tasks/Classification/pl/
--rw-r--r--   0 root         (0) root         (0)     4712 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/pl/PolishClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.246385 mteb-1.3.4/mteb/tasks/Classification/sv/
--rw-r--r--   0 root         (0) root         (0)      995 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/sv/SweRecClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/sv/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.246385 mteb-1.3.4/mteb/tasks/Classification/zh/
--rw-r--r--   0 root         (0) root         (0)     6307 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/zh/CMTEBClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Classification/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.246385 mteb-1.3.4/mteb/tasks/Clustering/
--rw-r--r--   0 root         (0) root         (0)     1249 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.250385 mteb-1.3.4/mteb/tasks/Clustering/de/
--rw-r--r--   0 root         (0) root         (0)     1090 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/de/BlurbsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1073 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/de/BlurbsClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1058 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/de/TenKGnadClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1038 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/de/TenKGnadClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/de/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.250385 mteb-1.3.4/mteb/tasks/Clustering/en/
--rw-r--r--   0 root         (0) root         (0)     1059 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/en/ArxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1045 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/en/ArxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1086 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/en/BigPatentClustering.py
--rw-r--r--   0 root         (0) root         (0)     1029 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/en/BiorxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1019 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/en/BiorxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1030 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/en/MedrxivClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1020 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/en/MedrxivClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1060 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/en/RedditClustering.py
--rw-r--r--   0 root         (0) root         (0)     1049 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/en/RedditClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1085 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/en/StackExchangeClustering.py
--rw-r--r--   0 root         (0) root         (0)     1073 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/en/StackExchangeClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     1042 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/en/TwentyNewsgroupsClustering.py
--rw-r--r--   0 root         (0) root         (0)     1028 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/en/WikiCitiesClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.254385 mteb-1.3.4/mteb/tasks/Clustering/es/
--rw-r--r--   0 root         (0) root         (0)      987 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/es/FloresClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1016 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/es/SpanishNewsClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/es/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.254385 mteb-1.3.4/mteb/tasks/Clustering/fr/
--rw-r--r--   0 root         (0) root         (0)     2278 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/fr/AlloProfClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     2123 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/fr/AlloProfClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     1985 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/fr/HALClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)     2334 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/fr/MLSUMClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     2149 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/fr/MLSUMClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/fr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.254385 mteb-1.3.4/mteb/tasks/Clustering/multilingual/
--rw-r--r--   0 root         (0) root         (0)     2522 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py
--rw-r--r--   0 root         (0) root         (0)     2541 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.254385 mteb-1.3.4/mteb/tasks/Clustering/nb/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/nb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3837 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/nb/snl_clustering.py
--rw-r--r--   0 root         (0) root         (0)     3991 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/nb/vg_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.254385 mteb-1.3.4/mteb/tasks/Clustering/pl/
--rw-r--r--   0 root         (0) root         (0)     1093 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/pl/PolishClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.254385 mteb-1.3.4/mteb/tasks/Clustering/sv/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/sv/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4342 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/sv/swedn_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.254385 mteb-1.3.4/mteb/tasks/Clustering/zh/
--rw-r--r--   0 root         (0) root         (0)     3441 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/zh/CMTEBClustering.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Clustering/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.258385 mteb-1.3.4/mteb/tasks/PairClassification/
--rw-r--r--   0 root         (0) root         (0)      301 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/PairClassification/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.258385 mteb-1.3.4/mteb/tasks/PairClassification/en/
--rw-r--r--   0 root         (0) root         (0)     1110 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/PairClassification/en/SprintDuplicateQuestionsPC.py
--rw-r--r--   0 root         (0) root         (0)     1044 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/PairClassification/en/TwitterSemEval2015PC.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/PairClassification/en/TwitterURLCorpusPC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/PairClassification/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.258385 mteb-1.3.4/mteb/tasks/PairClassification/multilingual/
--rw-r--r--   0 root         (0) root         (0)     2720 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py
--rw-r--r--   0 root         (0) root         (0)     1930 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/PairClassification/multilingual/PawsX.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/PairClassification/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.258385 mteb-1.3.4/mteb/tasks/PairClassification/pl/
--rw-r--r--   0 root         (0) root         (0)     3298 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/PairClassification/pl/PolishPC.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/PairClassification/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.258385 mteb-1.3.4/mteb/tasks/PairClassification/zh/
--rw-r--r--   0 root         (0) root         (0)     1765 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/PairClassification/zh/CMTEBPairClassification.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/PairClassification/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.258385 mteb-1.3.4/mteb/tasks/Reranking/
--rw-r--r--   0 root         (0) root         (0)      339 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Reranking/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.258385 mteb-1.3.4/mteb/tasks/Reranking/en/
--rw-r--r--   0 root         (0) root         (0)     1076 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Reranking/en/AskUbuntuDupQuestions.py
--rw-r--r--   0 root         (0) root         (0)     1022 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Reranking/en/MindSmallReranking.py
--rw-r--r--   0 root         (0) root         (0)     2974 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Reranking/en/SciDocsReranking.py
--rw-r--r--   0 root         (0) root         (0)     1095 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Reranking/en/StackOverflowDupQuestions.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Reranking/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.258385 mteb-1.3.4/mteb/tasks/Reranking/fr/
--rw-r--r--   0 root         (0) root         (0)     1137 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Reranking/fr/AlloprofReranking.py
--rw-r--r--   0 root         (0) root         (0)     1023 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Reranking/fr/SyntecReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Reranking/fr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.262385 mteb-1.3.4/mteb/tasks/Reranking/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1170 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Reranking/multilingual/MIRACLReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Reranking/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.262385 mteb-1.3.4/mteb/tasks/Reranking/zh/
--rw-r--r--   0 root         (0) root         (0)     3360 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Reranking/zh/CMTEBReranking.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Reranking/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.262385 mteb-1.3.4/mteb/tasks/Retrieval/
--rw-r--r--   0 root         (0) root         (0)     2462 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.262385 mteb-1.3.4/mteb/tasks/Retrieval/da/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/da/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4206 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/da/dan_fever.py
--rw-r--r--   0 root         (0) root         (0)     2978 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/da/t2nord_retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3543 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/da/twitterhjerne.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.262385 mteb-1.3.4/mteb/tasks/Retrieval/de/
--rw-r--r--   0 root         (0) root         (0)     2186 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/de/GerDaLIRRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2925 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/de/GermanDPRRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2067 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/de/GermanQuADRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/de/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.270385 mteb-1.3.4/mteb/tasks/Retrieval/en/
--rw-r--r--   0 root         (0) root         (0)      969 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/ArguAnaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1023 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/CQADupstackAndroidRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1023 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/CQADupstackEnglishRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1020 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/CQADupstackGamingRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1011 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/CQADupstackGisRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1035 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/CQADupstackMathematicaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1023 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/CQADupstackPhysicsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1035 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/CQADupstackProgrammersRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1017 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/CQADupstackStatsRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1011 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/CQADupstackTexRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1014 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/CQADupstackUnixRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1032 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/CQADupstackWebmastersRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1029 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/CQADupstackWordpressRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1053 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/ClimateFEVERRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      989 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/DBPediaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1133 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/FEVERRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      941 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/FiQA2018Retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3652 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/HagridRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1109 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/HotpotQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)      967 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/MSMARCORetrieval.py
--rw-r--r--   0 root         (0) root         (0)      997 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/MSMARCOv2Retrieval.py
--rw-r--r--   0 root         (0) root         (0)      982 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/NFCorpusRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      957 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/NQRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1938 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/NarrativeQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1113 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/QuoraRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1072 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/SCIDOCSRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1004 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/SciFactRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1027 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/TRECCOVIDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      967 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/Touche2020Retrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.270385 mteb-1.3.4/mteb/tasks/Retrieval/es/
--rw-r--r--   0 root         (0) root         (0)     2074 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2P.py
--rw-r--r--   0 root         (0) root         (0)     2074 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2S.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/es/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.270385 mteb-1.3.4/mteb/tasks/Retrieval/fr/
--rw-r--r--   0 root         (0) root         (0)     2067 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/fr/AlloprofRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2540 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/fr/BSARDRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2053 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/fr/SyntecRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/fr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.270385 mteb-1.3.4/mteb/tasks/Retrieval/ko/
--rw-r--r--   0 root         (0) root         (0)      864 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/ko/KoMiracl.py
--rw-r--r--   0 root         (0) root         (0)      864 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/ko/KoMrtydi.py
--rw-r--r--   0 root         (0) root         (0)      880 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/ko/KoStrategyQA.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/ko/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.270385 mteb-1.3.4/mteb/tasks/Retrieval/multilingual/
--rw-r--r--   0 root         (0) root         (0)     3197 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2854 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     3083 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2870 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     2874 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.270385 mteb-1.3.4/mteb/tasks/Retrieval/nb/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/nb/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4347 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/nb/norquad.py
--rw-r--r--   0 root         (0) root         (0)     3103 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/nb/snl_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.274385 mteb-1.3.4/mteb/tasks/Retrieval/pl/
--rw-r--r--   0 root         (0) root         (0)      925 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/pl/ArguAnaPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/pl/DBPediaPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      942 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/pl/FiQAPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1070 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/pl/HotpotQAPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      967 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/pl/MSMARCOPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      998 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/pl/NFCorpusPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)      955 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/pl/NQPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1121 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/pl/QuoraPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1049 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/pl/SCIDOCSPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1011 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/pl/SciFactPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)     1043 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/pl/TRECCOVIDPLRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.274385 mteb-1.3.4/mteb/tasks/Retrieval/sv/
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/sv/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3635 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/sv/swedn_retrieval.py
--rw-r--r--   0 root         (0) root         (0)     3035 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/sv/swefaq_retrieval.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.274385 mteb-1.3.4/mteb/tasks/Retrieval/zh/
--rw-r--r--   0 root         (0) root         (0)     9421 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/zh/CMTEBRetrieval.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Retrieval/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.274385 mteb-1.3.4/mteb/tasks/STS/
--rw-r--r--   0 root         (0) root         (0)      562 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/STS/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.274385 mteb-1.3.4/mteb/tasks/STS/de/
--rw-r--r--   0 root         (0) root         (0)     1326 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/STS/de/GermanSTSBenchmarkSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/STS/de/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.278385 mteb-1.3.4/mteb/tasks/STS/en/
--rw-r--r--   0 root         (0) root         (0)     1140 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/STS/en/BiossesSTS.py
--rw-r--r--   0 root         (0) root         (0)     1109 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/STS/en/STS12STS.py
--rw-r--r--   0 root         (0) root         (0)     1106 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/STS/en/STS13STS.py
--rw-r--r--   0 root         (0) root         (0)     1140 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/STS/en/STS14STS.py
--rw-r--r--   0 root         (0) root         (0)     1104 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/STS/en/STS15STS.py
--rw-r--r--   0 root         (0) root         (0)     1104 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/STS/en/STS16STS.py
--rw-r--r--   0 root         (0) root         (0)     1164 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/STS/en/STSBenchmarkSTS.py
--rw-r--r--   0 root         (0) root         (0)     1149 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/STS/en/SickrSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/STS/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.278385 mteb-1.3.4/mteb/tasks/STS/es/
--rw-r--r--   0 root         (0) root         (0)     1686 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/STS/es/STSES.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/STS/es/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.278385 mteb-1.3.4/mteb/tasks/STS/fr/
--rw-r--r--   0 root         (0) root         (0)     1804 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/STS/fr/SickFrSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/STS/fr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.278385 mteb-1.3.4/mteb/tasks/STS/multilingual/
--rw-r--r--   0 root         (0) root         (0)     1324 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     1446 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py
--rw-r--r--   0 root         (0) root         (0)     2556 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/STS/multilingual/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.278385 mteb-1.3.4/mteb/tasks/STS/pl/
--rw-r--r--   0 root         (0) root         (0)     2180 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/STS/pl/PolishSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/STS/pl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.278385 mteb-1.3.4/mteb/tasks/STS/zh/
--rw-r--r--   0 root         (0) root         (0)     6816 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/STS/zh/CMTEBSTS.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/STS/zh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.278385 mteb-1.3.4/mteb/tasks/Summarization/
--rw-r--r--   0 root         (0) root         (0)      122 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Summarization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.282385 mteb-1.3.4/mteb/tasks/Summarization/en/
--rw-r--r--   0 root         (0) root         (0)     1199 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Summarization/en/SummEvalSummarization.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Summarization/en/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.282385 mteb-1.3.4/mteb/tasks/Summarization/fr/
--rw-r--r--   0 root         (0) root         (0)     1239 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Summarization/fr/SummEvalFrSummarization.py
--rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/Summarization/fr/__init__.py
--rw-r--r--   0 root         (0) root         (0)      252 2024-04-01 08:50:54.000000 mteb-1.3.4/mteb/tasks/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.286385 mteb-1.3.4/mteb.egg-info/
--rw-r--r--   0 root         (0) root         (0)    23566 2024-04-01 08:50:58.000000 mteb-1.3.4/mteb.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    12552 2024-04-01 08:50:58.000000 mteb-1.3.4/mteb.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 08:50:58.000000 mteb-1.3.4/mteb.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       39 2024-04-01 08:50:58.000000 mteb-1.3.4/mteb.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      219 2024-04-01 08:50:58.000000 mteb-1.3.4/mteb.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       31 2024-04-01 08:50:58.000000 mteb-1.3.4/mteb.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)     2105 2024-04-01 08:50:55.000000 mteb-1.3.4/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.282385 mteb-1.3.4/scripts/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.282385 mteb-1.3.4/scripts/data/
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.282385 mteb-1.3.4/scripts/data/amazon_polarity/
--rw-r--r--   0 root         (0) root         (0)      842 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/data/amazon_polarity/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.282385 mteb-1.3.4/scripts/data/amazon_reviews_multi/
--rw-r--r--   0 root         (0) root         (0)     1379 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/data/amazon_reviews_multi/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.282385 mteb-1.3.4/scripts/data/arxiv/
--rw-r--r--   0 root         (0) root         (0)     3146 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/data/arxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1451 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/data/arxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.282385 mteb-1.3.4/scripts/data/biorxiv/
--rw-r--r--   0 root         (0) root         (0)     1781 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/data/biorxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1674 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/data/biorxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.282385 mteb-1.3.4/scripts/data/bucc/
--rw-r--r--   0 root         (0) root         (0)     1171 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/data/bucc/create_data.py
--rw-r--r--   0 root         (0) root         (0)     5933 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/data/create_task_table.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.282385 mteb-1.3.4/scripts/data/germanquad/
--rw-r--r--   0 root         (0) root         (0)     2132 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/data/germanquad/process_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.282385 mteb-1.3.4/scripts/data/hal/
--rw-r--r--   0 root         (0) root         (0)     1512 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/data/hal/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.286385 mteb-1.3.4/scripts/data/imdb/
--rw-r--r--   0 root         (0) root         (0)      682 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/data/imdb/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.286385 mteb-1.3.4/scripts/data/medrxiv/
--rw-r--r--   0 root         (0) root         (0)     1780 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/data/medrxiv/script_clustering.py
--rw-r--r--   0 root         (0) root         (0)     1617 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/data/medrxiv/script_raw.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.286385 mteb-1.3.4/scripts/data/mind/
--rw-r--r--   0 root         (0) root         (0)     1377 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/data/mind/prepare_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.286385 mteb-1.3.4/scripts/data/redditp2p/
--rw-r--r--   0 root         (0) root         (0)     1880 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/data/redditp2p/script_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.286385 mteb-1.3.4/scripts/data/stackexchangep2p/
--rw-r--r--   0 root         (0) root         (0)     1627 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/data/stackexchangep2p/script_clustering.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.286385 mteb-1.3.4/scripts/data/sts22-crosslingual-sts/
--rw-r--r--   0 root         (0) root         (0)     2436 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/data/sts22-crosslingual-sts/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.286385 mteb-1.3.4/scripts/data/summeval_fr/
--rw-r--r--   0 root         (0) root         (0)     1692 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/data/summeval_fr/create_data.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.286385 mteb-1.3.4/scripts/data/toxic_conversations_50k/
--rw-r--r--   0 root         (0) root         (0)     1151 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/data/toxic_conversations_50k/create_data.py
--rw-r--r--   0 root         (0) root         (0)     2516 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/merge_cqadupstack.py
--rw-r--r--   0 root         (0) root         (0)     5155 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/mteb_meta.py
--rw-r--r--   0 root         (0) root         (0)      673 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/run_mteb_chinese.py
--rw-r--r--   0 root         (0) root         (0)     2819 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/run_mteb_english.py
--rw-r--r--   0 root         (0) root         (0)     1852 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/run_mteb_french.py
--rw-r--r--   0 root         (0) root         (0)     1305 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/run_mteb_german.py
--rw-r--r--   0 root         (0) root         (0)     1033 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/run_mteb_korean.py
--rw-r--r--   0 root         (0) root         (0)      975 2024-04-01 08:50:54.000000 mteb-1.3.4/scripts/run_mteb_polish.py
--rw-r--r--   0 root         (0) root         (0)       38 2024-04-01 08:50:58.290385 mteb-1.3.4/setup.cfg
-drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 08:50:58.286385 mteb-1.3.4/tests/
--rw-r--r--   0 root         (0) root         (0)      632 2024-04-01 08:50:54.000000 mteb-1.3.4/tests/test_ClusteringEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1560 2024-04-01 08:50:54.000000 mteb-1.3.4/tests/test_PairClassificationEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1130 2024-04-01 08:50:54.000000 mteb-1.3.4/tests/test_RerankingEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1113 2024-04-01 08:50:54.000000 mteb-1.3.4/tests/test_RetrievalEvaluator.py
--rw-r--r--   0 root         (0) root         (0)     1419 2024-04-01 08:50:54.000000 mteb-1.3.4/tests/test_all_abstasks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.516563 mteb-1.4.0/
+-rw-r--r--   0 root         (0) root         (0)    11357 2024-04-01 12:07:56.000000 mteb-1.4.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)    23581 2024-04-01 12:08:00.516563 mteb-1.4.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     9190 2024-04-01 12:07:56.000000 mteb-1.4.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.460563 mteb-1.4.0/mteb/
+-rw-r--r--   0 root         (0) root         (0)     1917 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.464563 mteb-1.4.0/mteb/abstasks/
+-rw-r--r--   0 root         (0) root         (0)     1592 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/abstasks/AbsTask.py
+-rw-r--r--   0 root         (0) root         (0)     3063 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/abstasks/AbsTaskBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5881 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/abstasks/AbsTaskClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2389 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/abstasks/AbsTaskClustering.py
+-rw-r--r--   0 root         (0) root         (0)     2542 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/abstasks/AbsTaskPairClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1120 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/abstasks/AbsTaskReranking.py
+-rw-r--r--   0 root         (0) root         (0)    11832 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/abstasks/AbsTaskRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/abstasks/AbsTaskSTS.py
+-rw-r--r--   0 root         (0) root         (0)     2296 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/abstasks/AbsTaskSummarization.py
+-rw-r--r--   0 root         (0) root         (0)      961 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/abstasks/CrosslingualTask.py
+-rw-r--r--   0 root         (0) root         (0)     2831 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/abstasks/LangMapping.py
+-rw-r--r--   0 root         (0) root         (0)     1052 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/abstasks/MultilingualTask.py
+-rw-r--r--   0 root         (0) root         (0)     5356 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/abstasks/TaskMetadata.py
+-rw-r--r--   0 root         (0) root         (0)      422 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/abstasks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5296 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/cmd.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.464563 mteb-1.4.0/mteb/evaluation/
+-rw-r--r--   0 root         (0) root         (0)    13067 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/evaluation/MTEB.py
+-rw-r--r--   0 root         (0) root         (0)       56 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/evaluation/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.464563 mteb-1.4.0/mteb/evaluation/evaluators/
+-rw-r--r--   0 root         (0) root         (0)     5849 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/evaluation/evaluators/BitextMiningEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     8942 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/evaluation/evaluators/ClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1463 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/evaluation/evaluators/ClusteringEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)      744 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/evaluation/evaluators/Evaluator.py
+-rw-r--r--   0 root         (0) root         (0)     7140 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/evaluation/evaluators/PairClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     9613 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/evaluation/evaluators/RerankingEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)    12487 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/evaluation/evaluators/RetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     2394 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/evaluation/evaluators/STSEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     4841 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/evaluation/evaluators/SummarizationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)      324 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/evaluation/evaluators/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5482 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/evaluation/evaluators/utils.py
+-rw-r--r--   0 root         (0) root         (0)      835 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/logging.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.468563 mteb-1.4.0/mteb/tasks/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.468563 mteb-1.4.0/mteb/tasks/BitextMining/
+-rw-r--r--   0 root         (0) root         (0)      369 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/BitextMining/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.468563 mteb-1.4.0/mteb/tasks/BitextMining/da/
+-rw-r--r--   0 root         (0) root         (0)     1800 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/BitextMining/da/BornholmskBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/BitextMining/da/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.468563 mteb-1.4.0/mteb/tasks/BitextMining/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1040 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     2257 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     5808 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     1813 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)     2761 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/BitextMining/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.468563 mteb-1.4.0/mteb/tasks/BitextMining/nb/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/BitextMining/nb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1806 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/BitextMining/nb/norwegian_courts_bitext_mining.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.468563 mteb-1.4.0/mteb/tasks/Classification/
+-rw-r--r--   0 root         (0) root         (0)     1232 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.468563 mteb-1.4.0/mteb/tasks/Classification/da/
+-rw-r--r--   0 root         (0) root         (0)     1278 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/da/AngryTweetsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1978 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/da/DKHateClassification.py
+-rw-r--r--   0 root         (0) root         (0)     2881 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/da/DalajClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1967 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/da/DanishPoliticalCommentsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     3303 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/da/DdiscoCohesionClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1217 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/da/LccSentimentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/da/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.472563 mteb-1.4.0/mteb/tasks/Classification/en/
+-rw-r--r--   0 root         (0) root         (0)      999 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/en/AmazonPolarityClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1012 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/en/Banking77Classification.py
+-rw-r--r--   0 root         (0) root         (0)     1330 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/en/EmotionClassification.py
+-rw-r--r--   0 root         (0) root         (0)      948 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/en/ImdbClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1368 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/en/ToxicConversationsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/en/TweetSentimentExtractionClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.472563 mteb-1.4.0/mteb/tasks/Classification/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1447 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1199 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1128 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1367 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1787 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1793 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1841 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/multilingual/NordicLangClassification.py
+-rw-r--r--   0 root         (0) root         (0)     7434 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/multilingual/ScalaClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.472563 mteb-1.4.0/mteb/tasks/Classification/nb/
+-rw-r--r--   0 root         (0) root         (0)     1063 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/nb/NoRecClassification.py
+-rw-r--r--   0 root         (0) root         (0)     1124 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/nb/NorwegianParliamentClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/nb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.476563 mteb-1.4.0/mteb/tasks/Classification/pl/
+-rw-r--r--   0 root         (0) root         (0)     4712 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/pl/PolishClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.476563 mteb-1.4.0/mteb/tasks/Classification/sv/
+-rw-r--r--   0 root         (0) root         (0)      995 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/sv/SweRecClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/sv/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.476563 mteb-1.4.0/mteb/tasks/Classification/zh/
+-rw-r--r--   0 root         (0) root         (0)     6307 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/zh/CMTEBClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Classification/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.476563 mteb-1.4.0/mteb/tasks/Clustering/
+-rw-r--r--   0 root         (0) root         (0)     1249 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.476563 mteb-1.4.0/mteb/tasks/Clustering/de/
+-rw-r--r--   0 root         (0) root         (0)     1090 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/de/BlurbsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/de/BlurbsClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1058 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/de/TenKGnadClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1038 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/de/TenKGnadClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/de/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.480563 mteb-1.4.0/mteb/tasks/Clustering/en/
+-rw-r--r--   0 root         (0) root         (0)     1059 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/en/ArxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1045 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/en/ArxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1086 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/en/BigPatentClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/en/BiorxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1019 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/en/BiorxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1030 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/en/MedrxivClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/en/MedrxivClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1060 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/en/RedditClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1049 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/en/RedditClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1085 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/en/StackExchangeClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1073 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/en/StackExchangeClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     1042 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/en/TwentyNewsgroupsClustering.py
+-rw-r--r--   0 root         (0) root         (0)     1028 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/en/WikiCitiesClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.480563 mteb-1.4.0/mteb/tasks/Clustering/es/
+-rw-r--r--   0 root         (0) root         (0)      987 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/es/FloresClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1016 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/es/SpanishNewsClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/es/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.480563 mteb-1.4.0/mteb/tasks/Clustering/fr/
+-rw-r--r--   0 root         (0) root         (0)     2278 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/fr/AlloProfClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     2123 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/fr/AlloProfClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     1985 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/fr/HALClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)     2334 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/fr/MLSUMClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     2149 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/fr/MLSUMClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/fr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.480563 mteb-1.4.0/mteb/tasks/Clustering/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     2522 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py
+-rw-r--r--   0 root         (0) root         (0)     2541 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.480563 mteb-1.4.0/mteb/tasks/Clustering/nb/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/nb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3837 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/nb/snl_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     3991 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/nb/vg_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.484563 mteb-1.4.0/mteb/tasks/Clustering/pl/
+-rw-r--r--   0 root         (0) root         (0)     1093 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/pl/PolishClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.484563 mteb-1.4.0/mteb/tasks/Clustering/sv/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/sv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4342 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/sv/swedn_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.484563 mteb-1.4.0/mteb/tasks/Clustering/zh/
+-rw-r--r--   0 root         (0) root         (0)     3441 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/zh/CMTEBClustering.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Clustering/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.484563 mteb-1.4.0/mteb/tasks/PairClassification/
+-rw-r--r--   0 root         (0) root         (0)      301 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/PairClassification/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.484563 mteb-1.4.0/mteb/tasks/PairClassification/en/
+-rw-r--r--   0 root         (0) root         (0)     1110 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/PairClassification/en/SprintDuplicateQuestionsPC.py
+-rw-r--r--   0 root         (0) root         (0)     1044 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/PairClassification/en/TwitterSemEval2015PC.py
+-rw-r--r--   0 root         (0) root         (0)      998 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/PairClassification/en/TwitterURLCorpusPC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/PairClassification/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.484563 mteb-1.4.0/mteb/tasks/PairClassification/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     2720 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py
+-rw-r--r--   0 root         (0) root         (0)     1930 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/PairClassification/multilingual/PawsX.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/PairClassification/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.484563 mteb-1.4.0/mteb/tasks/PairClassification/pl/
+-rw-r--r--   0 root         (0) root         (0)     3298 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/PairClassification/pl/PolishPC.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/PairClassification/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.484563 mteb-1.4.0/mteb/tasks/PairClassification/zh/
+-rw-r--r--   0 root         (0) root         (0)     1765 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/PairClassification/zh/CMTEBPairClassification.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/PairClassification/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.484563 mteb-1.4.0/mteb/tasks/Reranking/
+-rw-r--r--   0 root         (0) root         (0)      339 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Reranking/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.488563 mteb-1.4.0/mteb/tasks/Reranking/en/
+-rw-r--r--   0 root         (0) root         (0)     1076 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Reranking/en/AskUbuntuDupQuestions.py
+-rw-r--r--   0 root         (0) root         (0)     1022 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Reranking/en/MindSmallReranking.py
+-rw-r--r--   0 root         (0) root         (0)     2974 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Reranking/en/SciDocsReranking.py
+-rw-r--r--   0 root         (0) root         (0)     1095 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Reranking/en/StackOverflowDupQuestions.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Reranking/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.488563 mteb-1.4.0/mteb/tasks/Reranking/fr/
+-rw-r--r--   0 root         (0) root         (0)     1137 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Reranking/fr/AlloprofReranking.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Reranking/fr/SyntecReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Reranking/fr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.488563 mteb-1.4.0/mteb/tasks/Reranking/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1170 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Reranking/multilingual/MIRACLReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Reranking/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.488563 mteb-1.4.0/mteb/tasks/Reranking/zh/
+-rw-r--r--   0 root         (0) root         (0)     3360 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Reranking/zh/CMTEBReranking.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Reranking/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.488563 mteb-1.4.0/mteb/tasks/Retrieval/
+-rw-r--r--   0 root         (0) root         (0)     2462 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.488563 mteb-1.4.0/mteb/tasks/Retrieval/da/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/da/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4206 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/da/dan_fever.py
+-rw-r--r--   0 root         (0) root         (0)     2978 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/da/t2nord_retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3543 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/da/twitterhjerne.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.488563 mteb-1.4.0/mteb/tasks/Retrieval/de/
+-rw-r--r--   0 root         (0) root         (0)     2186 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/de/GerDaLIRRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2925 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/de/GermanDPRRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2067 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/de/GermanQuADRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/de/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.496563 mteb-1.4.0/mteb/tasks/Retrieval/en/
+-rw-r--r--   0 root         (0) root         (0)      969 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/ArguAnaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/CQADupstackAndroidRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/CQADupstackEnglishRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/CQADupstackGamingRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/CQADupstackGisRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1035 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/CQADupstackMathematicaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1023 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/CQADupstackPhysicsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1035 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/CQADupstackProgrammersRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1017 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/CQADupstackStatsRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/CQADupstackTexRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1014 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/CQADupstackUnixRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1032 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/CQADupstackWebmastersRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1029 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/CQADupstackWordpressRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1053 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/ClimateFEVERRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      989 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/DBPediaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1133 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/FEVERRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      941 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/FiQA2018Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3652 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/HagridRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1109 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/HotpotQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      967 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/MSMARCORetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      997 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/MSMARCOv2Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)      982 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/NFCorpusRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      957 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/NQRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1938 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/NarrativeQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/QuoraRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1072 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/SCIDOCSRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1004 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/SciFactRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1027 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/TRECCOVIDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      967 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/Touche2020Retrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.496563 mteb-1.4.0/mteb/tasks/Retrieval/es/
+-rw-r--r--   0 root         (0) root         (0)     2074 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2P.py
+-rw-r--r--   0 root         (0) root         (0)     2074 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2S.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/es/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.496563 mteb-1.4.0/mteb/tasks/Retrieval/fr/
+-rw-r--r--   0 root         (0) root         (0)     2067 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/fr/AlloprofRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2540 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/fr/BSARDRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2053 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/fr/SyntecRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/fr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.496563 mteb-1.4.0/mteb/tasks/Retrieval/ko/
+-rw-r--r--   0 root         (0) root         (0)      864 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/ko/KoMiracl.py
+-rw-r--r--   0 root         (0) root         (0)      864 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/ko/KoMrtydi.py
+-rw-r--r--   0 root         (0) root         (0)      880 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/ko/KoStrategyQA.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/ko/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.500563 mteb-1.4.0/mteb/tasks/Retrieval/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     3197 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2854 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3083 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2870 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     2874 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.500563 mteb-1.4.0/mteb/tasks/Retrieval/nb/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/nb/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4347 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/nb/norquad.py
+-rw-r--r--   0 root         (0) root         (0)     3103 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/nb/snl_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.500563 mteb-1.4.0/mteb/tasks/Retrieval/pl/
+-rw-r--r--   0 root         (0) root         (0)      925 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/pl/ArguAnaPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      998 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/pl/DBPediaPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      942 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/pl/FiQAPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1070 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/pl/HotpotQAPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      967 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/pl/MSMARCOPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      998 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/pl/NFCorpusPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)      955 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/pl/NQPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1121 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/pl/QuoraPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1049 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/pl/SCIDOCSPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1011 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/pl/SciFactPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)     1043 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/pl/TRECCOVIDPLRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.504563 mteb-1.4.0/mteb/tasks/Retrieval/sv/
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/sv/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3635 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/sv/swedn_retrieval.py
+-rw-r--r--   0 root         (0) root         (0)     3035 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/sv/swefaq_retrieval.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.504563 mteb-1.4.0/mteb/tasks/Retrieval/zh/
+-rw-r--r--   0 root         (0) root         (0)     9421 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/zh/CMTEBRetrieval.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Retrieval/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.504563 mteb-1.4.0/mteb/tasks/STS/
+-rw-r--r--   0 root         (0) root         (0)      562 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/STS/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.504563 mteb-1.4.0/mteb/tasks/STS/de/
+-rw-r--r--   0 root         (0) root         (0)     1326 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/STS/de/GermanSTSBenchmarkSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/STS/de/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.504563 mteb-1.4.0/mteb/tasks/STS/en/
+-rw-r--r--   0 root         (0) root         (0)     1140 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/STS/en/BiossesSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1109 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/STS/en/STS12STS.py
+-rw-r--r--   0 root         (0) root         (0)     1106 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/STS/en/STS13STS.py
+-rw-r--r--   0 root         (0) root         (0)     1140 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/STS/en/STS14STS.py
+-rw-r--r--   0 root         (0) root         (0)     1104 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/STS/en/STS15STS.py
+-rw-r--r--   0 root         (0) root         (0)     1104 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/STS/en/STS16STS.py
+-rw-r--r--   0 root         (0) root         (0)     1164 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/STS/en/STSBenchmarkSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1149 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/STS/en/SickrSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/STS/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.504563 mteb-1.4.0/mteb/tasks/STS/es/
+-rw-r--r--   0 root         (0) root         (0)     1686 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/STS/es/STSES.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/STS/es/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.504563 mteb-1.4.0/mteb/tasks/STS/fr/
+-rw-r--r--   0 root         (0) root         (0)     1804 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/STS/fr/SickFrSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/STS/fr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.508563 mteb-1.4.0/mteb/tasks/STS/multilingual/
+-rw-r--r--   0 root         (0) root         (0)     1324 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     1446 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)     2556 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/STS/multilingual/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.508563 mteb-1.4.0/mteb/tasks/STS/pl/
+-rw-r--r--   0 root         (0) root         (0)     2180 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/STS/pl/PolishSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/STS/pl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.508563 mteb-1.4.0/mteb/tasks/STS/zh/
+-rw-r--r--   0 root         (0) root         (0)     6816 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/STS/zh/CMTEBSTS.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/STS/zh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.508563 mteb-1.4.0/mteb/tasks/Summarization/
+-rw-r--r--   0 root         (0) root         (0)      122 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Summarization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.508563 mteb-1.4.0/mteb/tasks/Summarization/en/
+-rw-r--r--   0 root         (0) root         (0)     1199 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Summarization/en/SummEvalSummarization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Summarization/en/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.508563 mteb-1.4.0/mteb/tasks/Summarization/fr/
+-rw-r--r--   0 root         (0) root         (0)     1239 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Summarization/fr/SummEvalFrSummarization.py
+-rw-r--r--   0 root         (0) root         (0)        0 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/Summarization/fr/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      252 2024-04-01 12:07:56.000000 mteb-1.4.0/mteb/tasks/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.516563 mteb-1.4.0/mteb.egg-info/
+-rw-r--r--   0 root         (0) root         (0)    23581 2024-04-01 12:08:00.000000 mteb-1.4.0/mteb.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    12552 2024-04-01 12:08:00.000000 mteb-1.4.0/mteb.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2024-04-01 12:08:00.000000 mteb-1.4.0/mteb.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2024-04-01 12:08:00.000000 mteb-1.4.0/mteb.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      234 2024-04-01 12:08:00.000000 mteb-1.4.0/mteb.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       31 2024-04-01 12:08:00.000000 mteb-1.4.0/mteb.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)     2120 2024-04-01 12:07:57.000000 mteb-1.4.0/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.508563 mteb-1.4.0/scripts/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.508563 mteb-1.4.0/scripts/data/
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.512563 mteb-1.4.0/scripts/data/amazon_polarity/
+-rw-r--r--   0 root         (0) root         (0)      842 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/data/amazon_polarity/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.512563 mteb-1.4.0/scripts/data/amazon_reviews_multi/
+-rw-r--r--   0 root         (0) root         (0)     1379 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/data/amazon_reviews_multi/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.512563 mteb-1.4.0/scripts/data/arxiv/
+-rw-r--r--   0 root         (0) root         (0)     3146 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/data/arxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1451 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/data/arxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.512563 mteb-1.4.0/scripts/data/biorxiv/
+-rw-r--r--   0 root         (0) root         (0)     1781 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/data/biorxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1674 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/data/biorxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.512563 mteb-1.4.0/scripts/data/bucc/
+-rw-r--r--   0 root         (0) root         (0)     1171 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/data/bucc/create_data.py
+-rw-r--r--   0 root         (0) root         (0)     5933 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/data/create_task_table.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.512563 mteb-1.4.0/scripts/data/germanquad/
+-rw-r--r--   0 root         (0) root         (0)     2132 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/data/germanquad/process_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.512563 mteb-1.4.0/scripts/data/hal/
+-rw-r--r--   0 root         (0) root         (0)     1512 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/data/hal/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.512563 mteb-1.4.0/scripts/data/imdb/
+-rw-r--r--   0 root         (0) root         (0)      682 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/data/imdb/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.512563 mteb-1.4.0/scripts/data/medrxiv/
+-rw-r--r--   0 root         (0) root         (0)     1780 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/data/medrxiv/script_clustering.py
+-rw-r--r--   0 root         (0) root         (0)     1617 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/data/medrxiv/script_raw.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.512563 mteb-1.4.0/scripts/data/mind/
+-rw-r--r--   0 root         (0) root         (0)     1377 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/data/mind/prepare_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.512563 mteb-1.4.0/scripts/data/redditp2p/
+-rw-r--r--   0 root         (0) root         (0)     1880 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/data/redditp2p/script_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.512563 mteb-1.4.0/scripts/data/stackexchangep2p/
+-rw-r--r--   0 root         (0) root         (0)     1627 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/data/stackexchangep2p/script_clustering.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.512563 mteb-1.4.0/scripts/data/sts22-crosslingual-sts/
+-rw-r--r--   0 root         (0) root         (0)     2436 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/data/sts22-crosslingual-sts/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.512563 mteb-1.4.0/scripts/data/summeval_fr/
+-rw-r--r--   0 root         (0) root         (0)     1692 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/data/summeval_fr/create_data.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.512563 mteb-1.4.0/scripts/data/toxic_conversations_50k/
+-rw-r--r--   0 root         (0) root         (0)     1151 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/data/toxic_conversations_50k/create_data.py
+-rw-r--r--   0 root         (0) root         (0)     2516 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/merge_cqadupstack.py
+-rw-r--r--   0 root         (0) root         (0)     5155 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/mteb_meta.py
+-rw-r--r--   0 root         (0) root         (0)      673 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/run_mteb_chinese.py
+-rw-r--r--   0 root         (0) root         (0)     2819 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/run_mteb_english.py
+-rw-r--r--   0 root         (0) root         (0)     1852 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/run_mteb_french.py
+-rw-r--r--   0 root         (0) root         (0)     1305 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/run_mteb_german.py
+-rw-r--r--   0 root         (0) root         (0)     1033 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/run_mteb_korean.py
+-rw-r--r--   0 root         (0) root         (0)      975 2024-04-01 12:07:56.000000 mteb-1.4.0/scripts/run_mteb_polish.py
+-rw-r--r--   0 root         (0) root         (0)       38 2024-04-01 12:08:00.516563 mteb-1.4.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2024-04-01 12:08:00.516563 mteb-1.4.0/tests/
+-rw-r--r--   0 root         (0) root         (0)      632 2024-04-01 12:07:56.000000 mteb-1.4.0/tests/test_ClusteringEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1560 2024-04-01 12:07:56.000000 mteb-1.4.0/tests/test_PairClassificationEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1130 2024-04-01 12:07:56.000000 mteb-1.4.0/tests/test_RerankingEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2024-04-01 12:07:56.000000 mteb-1.4.0/tests/test_RetrievalEvaluator.py
+-rw-r--r--   0 root         (0) root         (0)     1419 2024-04-01 12:07:56.000000 mteb-1.4.0/tests/test_all_abstasks.py
```

### Comparing `mteb-1.3.4/LICENSE` & `mteb-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/PKG-INFO` & `mteb-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mteb
-Version: 1.3.4
+Version: 1.4.0
 Summary: Massive Text Embedding Benchmark
 Author-email: MTEB Contributors <niklas@huggingface.co>, nouamane@huggingface.co, info@nils-reimers.de
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -225,15 +225,15 @@
 Requires-Dist: requests>=2.26.0
 Requires-Dist: scikit_learn>=1.0.2
 Requires-Dist: scipy
 Requires-Dist: sentence_transformers>=2.2.0
 Requires-Dist: torch
 Requires-Dist: tqdm
 Requires-Dist: rich
-Requires-Dist: pytrec_eval
+Requires-Dist: pytrec-eval-terrier>=0.5.6
 Requires-Dist: pydantic
 Requires-Dist: typing_extensions
 Requires-Dist: eval_type_backport
 Provides-Extra: dev
 Requires-Dist: ruff>=0.0.254; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
```

### Comparing `mteb-1.3.4/README.md` & `mteb-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/__init__.py` & `mteb-1.4.0/mteb/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/abstasks/AbsTask.py` & `mteb-1.4.0/mteb/abstasks/AbsTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/abstasks/AbsTaskBitextMining.py` & `mteb-1.4.0/mteb/abstasks/AbsTaskBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/abstasks/AbsTaskClassification.py` & `mteb-1.4.0/mteb/abstasks/AbsTaskClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/abstasks/AbsTaskClustering.py` & `mteb-1.4.0/mteb/abstasks/AbsTaskClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/abstasks/AbsTaskPairClassification.py` & `mteb-1.4.0/mteb/abstasks/AbsTaskPairClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/abstasks/AbsTaskReranking.py` & `mteb-1.4.0/mteb/abstasks/AbsTaskReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/abstasks/AbsTaskRetrieval.py` & `mteb-1.4.0/mteb/abstasks/AbsTaskRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/abstasks/AbsTaskSTS.py` & `mteb-1.4.0/mteb/abstasks/AbsTaskSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/abstasks/AbsTaskSummarization.py` & `mteb-1.4.0/mteb/abstasks/AbsTaskSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/abstasks/CrosslingualTask.py` & `mteb-1.4.0/mteb/abstasks/CrosslingualTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/abstasks/LangMapping.py` & `mteb-1.4.0/mteb/abstasks/LangMapping.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/abstasks/MultilingualTask.py` & `mteb-1.4.0/mteb/abstasks/MultilingualTask.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/abstasks/TaskMetadata.py` & `mteb-1.4.0/mteb/abstasks/TaskMetadata.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/cmd.py` & `mteb-1.4.0/mteb/cmd.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/evaluation/MTEB.py` & `mteb-1.4.0/mteb/evaluation/MTEB.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/evaluation/evaluators/BitextMiningEvaluator.py` & `mteb-1.4.0/mteb/evaluation/evaluators/BitextMiningEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/evaluation/evaluators/ClassificationEvaluator.py` & `mteb-1.4.0/mteb/evaluation/evaluators/ClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/evaluation/evaluators/ClusteringEvaluator.py` & `mteb-1.4.0/mteb/evaluation/evaluators/ClusteringEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/evaluation/evaluators/Evaluator.py` & `mteb-1.4.0/mteb/evaluation/evaluators/Evaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/evaluation/evaluators/PairClassificationEvaluator.py` & `mteb-1.4.0/mteb/evaluation/evaluators/PairClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/evaluation/evaluators/RerankingEvaluator.py` & `mteb-1.4.0/mteb/evaluation/evaluators/RerankingEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/evaluation/evaluators/RetrievalEvaluator.py` & `mteb-1.4.0/mteb/evaluation/evaluators/RetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/evaluation/evaluators/STSEvaluator.py` & `mteb-1.4.0/mteb/evaluation/evaluators/STSEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/evaluation/evaluators/SummarizationEvaluator.py` & `mteb-1.4.0/mteb/evaluation/evaluators/SummarizationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/evaluation/evaluators/utils.py` & `mteb-1.4.0/mteb/evaluation/evaluators/utils.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/logging.py` & `mteb-1.4.0/mteb/logging.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/BitextMining/da/BornholmskBitextMining.py` & `mteb-1.4.0/mteb/tasks/BitextMining/da/BornholmskBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py` & `mteb-1.4.0/mteb/tasks/BitextMining/multilingual/BUCCBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py` & `mteb-1.4.0/mteb/tasks/BitextMining/multilingual/DiaBLaBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py` & `mteb-1.4.0/mteb/tasks/BitextMining/multilingual/FloresBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py` & `mteb-1.4.0/mteb/tasks/BitextMining/multilingual/NorwegianCourtsBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py` & `mteb-1.4.0/mteb/tasks/BitextMining/multilingual/TatoebaBitextMining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/BitextMining/nb/norwegian_courts_bitext_mining.py` & `mteb-1.4.0/mteb/tasks/BitextMining/nb/norwegian_courts_bitext_mining.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/__init__.py` & `mteb-1.4.0/mteb/tasks/Classification/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/da/AngryTweetsClassification.py` & `mteb-1.4.0/mteb/tasks/Classification/da/AngryTweetsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/da/DKHateClassification.py` & `mteb-1.4.0/mteb/tasks/Classification/da/DKHateClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/da/DalajClassification.py` & `mteb-1.4.0/mteb/tasks/Classification/da/DalajClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/da/DanishPoliticalCommentsClassification.py` & `mteb-1.4.0/mteb/tasks/Classification/da/DanishPoliticalCommentsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/da/DdiscoCohesionClassification.py` & `mteb-1.4.0/mteb/tasks/Classification/da/DdiscoCohesionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/da/LccSentimentClassification.py` & `mteb-1.4.0/mteb/tasks/Classification/da/LccSentimentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/en/AmazonPolarityClassification.py` & `mteb-1.4.0/mteb/tasks/Classification/en/AmazonPolarityClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/en/Banking77Classification.py` & `mteb-1.4.0/mteb/tasks/Classification/en/Banking77Classification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/en/EmotionClassification.py` & `mteb-1.4.0/mteb/tasks/Classification/en/EmotionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/en/ImdbClassification.py` & `mteb-1.4.0/mteb/tasks/Classification/en/ImdbClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/en/ToxicConversationsClassification.py` & `mteb-1.4.0/mteb/tasks/Classification/en/ToxicConversationsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/en/TweetSentimentExtractionClassification.py` & `mteb-1.4.0/mteb/tasks/Classification/en/TweetSentimentExtractionClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py` & `mteb-1.4.0/mteb/tasks/Classification/multilingual/AmazonCounterfactualClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py` & `mteb-1.4.0/mteb/tasks/Classification/multilingual/AmazonReviewsClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py` & `mteb-1.4.0/mteb/tasks/Classification/multilingual/MTOPDomainClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py` & `mteb-1.4.0/mteb/tasks/Classification/multilingual/MTOPIntentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py` & `mteb-1.4.0/mteb/tasks/Classification/multilingual/MasakhaNEWSClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py` & `mteb-1.4.0/mteb/tasks/Classification/multilingual/MassiveIntentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py` & `mteb-1.4.0/mteb/tasks/Classification/multilingual/MassiveScenarioClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/multilingual/NordicLangClassification.py` & `mteb-1.4.0/mteb/tasks/Classification/multilingual/NordicLangClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/multilingual/ScalaClassification.py` & `mteb-1.4.0/mteb/tasks/Classification/multilingual/ScalaClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/nb/NoRecClassification.py` & `mteb-1.4.0/mteb/tasks/Classification/nb/NoRecClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/nb/NorwegianParliamentClassification.py` & `mteb-1.4.0/mteb/tasks/Classification/nb/NorwegianParliamentClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/pl/PolishClassification.py` & `mteb-1.4.0/mteb/tasks/Classification/pl/PolishClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/sv/SweRecClassification.py` & `mteb-1.4.0/mteb/tasks/Classification/sv/SweRecClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Classification/zh/CMTEBClassification.py` & `mteb-1.4.0/mteb/tasks/Classification/zh/CMTEBClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/__init__.py` & `mteb-1.4.0/mteb/tasks/Clustering/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/de/BlurbsClusteringP2P.py` & `mteb-1.4.0/mteb/tasks/Clustering/de/BlurbsClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/de/BlurbsClusteringS2S.py` & `mteb-1.4.0/mteb/tasks/Clustering/de/BlurbsClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/de/TenKGnadClusteringP2P.py` & `mteb-1.4.0/mteb/tasks/Clustering/de/TenKGnadClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/de/TenKGnadClusteringS2S.py` & `mteb-1.4.0/mteb/tasks/Clustering/de/TenKGnadClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/en/ArxivClusteringP2P.py` & `mteb-1.4.0/mteb/tasks/Clustering/en/ArxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/en/ArxivClusteringS2S.py` & `mteb-1.4.0/mteb/tasks/Clustering/en/ArxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/en/BigPatentClustering.py` & `mteb-1.4.0/mteb/tasks/Clustering/en/BigPatentClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/en/BiorxivClusteringP2P.py` & `mteb-1.4.0/mteb/tasks/Clustering/en/BiorxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/en/BiorxivClusteringS2S.py` & `mteb-1.4.0/mteb/tasks/Clustering/en/BiorxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/en/MedrxivClusteringP2P.py` & `mteb-1.4.0/mteb/tasks/Clustering/en/MedrxivClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/en/MedrxivClusteringS2S.py` & `mteb-1.4.0/mteb/tasks/Clustering/en/MedrxivClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/en/RedditClustering.py` & `mteb-1.4.0/mteb/tasks/Clustering/en/RedditClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/en/RedditClusteringP2P.py` & `mteb-1.4.0/mteb/tasks/Clustering/en/RedditClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/en/StackExchangeClustering.py` & `mteb-1.4.0/mteb/tasks/Clustering/en/StackExchangeClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/en/StackExchangeClusteringP2P.py` & `mteb-1.4.0/mteb/tasks/Clustering/en/StackExchangeClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/en/TwentyNewsgroupsClustering.py` & `mteb-1.4.0/mteb/tasks/Clustering/en/TwentyNewsgroupsClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/en/WikiCitiesClustering.py` & `mteb-1.4.0/mteb/tasks/Clustering/en/WikiCitiesClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/es/FloresClusteringS2S.py` & `mteb-1.4.0/mteb/tasks/Clustering/es/FloresClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/es/SpanishNewsClusteringP2P.py` & `mteb-1.4.0/mteb/tasks/Clustering/es/SpanishNewsClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/fr/AlloProfClusteringP2P.py` & `mteb-1.4.0/mteb/tasks/Clustering/fr/AlloProfClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/fr/AlloProfClusteringS2S.py` & `mteb-1.4.0/mteb/tasks/Clustering/fr/AlloProfClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/fr/HALClusteringS2S.py` & `mteb-1.4.0/mteb/tasks/Clustering/fr/HALClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/fr/MLSUMClusteringP2P.py` & `mteb-1.4.0/mteb/tasks/Clustering/fr/MLSUMClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/fr/MLSUMClusteringS2S.py` & `mteb-1.4.0/mteb/tasks/Clustering/fr/MLSUMClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py` & `mteb-1.4.0/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringP2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py` & `mteb-1.4.0/mteb/tasks/Clustering/multilingual/MasakhaNEWSClusteringS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/nb/snl_clustering.py` & `mteb-1.4.0/mteb/tasks/Clustering/nb/snl_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/nb/vg_clustering.py` & `mteb-1.4.0/mteb/tasks/Clustering/nb/vg_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/pl/PolishClustering.py` & `mteb-1.4.0/mteb/tasks/Clustering/pl/PolishClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/sv/swedn_clustering.py` & `mteb-1.4.0/mteb/tasks/Clustering/sv/swedn_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Clustering/zh/CMTEBClustering.py` & `mteb-1.4.0/mteb/tasks/Clustering/zh/CMTEBClustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/PairClassification/en/SprintDuplicateQuestionsPC.py` & `mteb-1.4.0/mteb/tasks/PairClassification/en/SprintDuplicateQuestionsPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/PairClassification/en/TwitterSemEval2015PC.py` & `mteb-1.4.0/mteb/tasks/PairClassification/en/TwitterSemEval2015PC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/PairClassification/en/TwitterURLCorpusPC.py` & `mteb-1.4.0/mteb/tasks/PairClassification/en/TwitterURLCorpusPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py` & `mteb-1.4.0/mteb/tasks/PairClassification/multilingual/OpusparcusPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/PairClassification/multilingual/PawsX.py` & `mteb-1.4.0/mteb/tasks/PairClassification/multilingual/PawsX.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/PairClassification/pl/PolishPC.py` & `mteb-1.4.0/mteb/tasks/PairClassification/pl/PolishPC.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/PairClassification/zh/CMTEBPairClassification.py` & `mteb-1.4.0/mteb/tasks/PairClassification/zh/CMTEBPairClassification.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Reranking/en/AskUbuntuDupQuestions.py` & `mteb-1.4.0/mteb/tasks/Reranking/en/AskUbuntuDupQuestions.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Reranking/en/MindSmallReranking.py` & `mteb-1.4.0/mteb/tasks/Reranking/en/MindSmallReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Reranking/en/SciDocsReranking.py` & `mteb-1.4.0/mteb/tasks/Reranking/en/SciDocsReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Reranking/en/StackOverflowDupQuestions.py` & `mteb-1.4.0/mteb/tasks/Reranking/en/StackOverflowDupQuestions.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Reranking/fr/AlloprofReranking.py` & `mteb-1.4.0/mteb/tasks/Reranking/fr/AlloprofReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Reranking/fr/SyntecReranking.py` & `mteb-1.4.0/mteb/tasks/Reranking/fr/SyntecReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Reranking/multilingual/MIRACLReranking.py` & `mteb-1.4.0/mteb/tasks/Reranking/multilingual/MIRACLReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Reranking/zh/CMTEBReranking.py` & `mteb-1.4.0/mteb/tasks/Reranking/zh/CMTEBReranking.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/__init__.py` & `mteb-1.4.0/mteb/tasks/Retrieval/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/da/dan_fever.py` & `mteb-1.4.0/mteb/tasks/Retrieval/da/dan_fever.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/da/t2nord_retrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/da/t2nord_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/da/twitterhjerne.py` & `mteb-1.4.0/mteb/tasks/Retrieval/da/twitterhjerne.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/de/GerDaLIRRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/de/GerDaLIRRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/de/GermanDPRRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/de/GermanDPRRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/de/GermanQuADRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/de/GermanQuADRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/ArguAnaRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/ArguAnaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/CQADupstackAndroidRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/CQADupstackAndroidRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/CQADupstackEnglishRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/CQADupstackEnglishRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/CQADupstackGamingRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/CQADupstackGamingRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/CQADupstackGisRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/CQADupstackGisRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/CQADupstackMathematicaRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/CQADupstackMathematicaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/CQADupstackPhysicsRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/CQADupstackPhysicsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/CQADupstackProgrammersRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/CQADupstackProgrammersRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/CQADupstackStatsRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/CQADupstackStatsRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/CQADupstackTexRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/CQADupstackTexRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/CQADupstackUnixRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/CQADupstackUnixRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/CQADupstackWebmastersRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/CQADupstackWebmastersRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/CQADupstackWordpressRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/CQADupstackWordpressRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/ClimateFEVERRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/ClimateFEVERRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/DBPediaRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/DBPediaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/FEVERRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/FEVERRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/FiQA2018Retrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/FiQA2018Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/HagridRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/HagridRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/HotpotQARetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/HotpotQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/MSMARCORetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/MSMARCORetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/MSMARCOv2Retrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/MSMARCOv2Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/NFCorpusRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/NFCorpusRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/NQRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/NQRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/NarrativeQARetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/NarrativeQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/QuoraRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/QuoraRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/SCIDOCSRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/SCIDOCSRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/SciFactRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/SciFactRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/TRECCOVIDRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/TRECCOVIDRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/en/Touche2020Retrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/en/Touche2020Retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2P.py` & `mteb-1.4.0/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2P.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2S.py` & `mteb-1.4.0/mteb/tasks/Retrieval/es/SpanishPassageRetrievalS2S.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/fr/AlloprofRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/fr/AlloprofRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/fr/BSARDRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/fr/BSARDRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/fr/SyntecRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/fr/SyntecRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/ko/KoMiracl.py` & `mteb-1.4.0/mteb/tasks/Retrieval/ko/KoMiracl.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/ko/KoMrtydi.py` & `mteb-1.4.0/mteb/tasks/Retrieval/ko/KoMrtydi.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/ko/KoStrategyQA.py` & `mteb-1.4.0/mteb/tasks/Retrieval/ko/KoStrategyQA.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/multilingual/MIRACLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/multilingual/MintakaRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/multilingual/MultiLongDocRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/multilingual/XMarketRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/multilingual/XPQARetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/nb/norquad.py` & `mteb-1.4.0/mteb/tasks/Retrieval/nb/norquad.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/nb/snl_retrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/nb/snl_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/pl/ArguAnaPLRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/pl/ArguAnaPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/pl/DBPediaPLRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/pl/DBPediaPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/pl/FiQAPLRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/pl/FiQAPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/pl/HotpotQAPLRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/pl/HotpotQAPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/pl/MSMARCOPLRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/pl/MSMARCOPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/pl/NFCorpusPLRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/pl/NFCorpusPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/pl/NQPLRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/pl/NQPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/pl/QuoraPLRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/pl/QuoraPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/pl/SCIDOCSPLRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/pl/SCIDOCSPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/pl/SciFactPLRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/pl/SciFactPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/pl/TRECCOVIDPLRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/pl/TRECCOVIDPLRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/sv/swedn_retrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/sv/swedn_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/sv/swefaq_retrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/sv/swefaq_retrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Retrieval/zh/CMTEBRetrieval.py` & `mteb-1.4.0/mteb/tasks/Retrieval/zh/CMTEBRetrieval.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/STS/__init__.py` & `mteb-1.4.0/mteb/tasks/STS/__init__.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/STS/de/GermanSTSBenchmarkSTS.py` & `mteb-1.4.0/mteb/tasks/STS/de/GermanSTSBenchmarkSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/STS/en/BiossesSTS.py` & `mteb-1.4.0/mteb/tasks/STS/en/BiossesSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/STS/en/STS12STS.py` & `mteb-1.4.0/mteb/tasks/STS/en/STS12STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/STS/en/STS13STS.py` & `mteb-1.4.0/mteb/tasks/STS/en/STS13STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/STS/en/STS14STS.py` & `mteb-1.4.0/mteb/tasks/STS/en/STS14STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/STS/en/STS15STS.py` & `mteb-1.4.0/mteb/tasks/STS/en/STS15STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/STS/en/STS16STS.py` & `mteb-1.4.0/mteb/tasks/STS/en/STS16STS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/STS/en/STSBenchmarkSTS.py` & `mteb-1.4.0/mteb/tasks/STS/en/STSBenchmarkSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/STS/en/SickrSTS.py` & `mteb-1.4.0/mteb/tasks/STS/en/SickrSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/STS/es/STSES.py` & `mteb-1.4.0/mteb/tasks/STS/es/STSES.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/STS/fr/SickFrSTS.py` & `mteb-1.4.0/mteb/tasks/STS/fr/SickFrSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py` & `mteb-1.4.0/mteb/tasks/STS/multilingual/STS17CrosslingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py` & `mteb-1.4.0/mteb/tasks/STS/multilingual/STS22CrosslingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py` & `mteb-1.4.0/mteb/tasks/STS/multilingual/STSBenchmarkMultilingualSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/STS/pl/PolishSTS.py` & `mteb-1.4.0/mteb/tasks/STS/pl/PolishSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/STS/zh/CMTEBSTS.py` & `mteb-1.4.0/mteb/tasks/STS/zh/CMTEBSTS.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Summarization/en/SummEvalSummarization.py` & `mteb-1.4.0/mteb/tasks/Summarization/en/SummEvalSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb/tasks/Summarization/fr/SummEvalFrSummarization.py` & `mteb-1.4.0/mteb/tasks/Summarization/fr/SummEvalFrSummarization.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/mteb.egg-info/PKG-INFO` & `mteb-1.4.0/mteb.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mteb
-Version: 1.3.4
+Version: 1.4.0
 Summary: Massive Text Embedding Benchmark
 Author-email: MTEB Contributors <niklas@huggingface.co>, nouamane@huggingface.co, info@nils-reimers.de
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
@@ -225,15 +225,15 @@
 Requires-Dist: requests>=2.26.0
 Requires-Dist: scikit_learn>=1.0.2
 Requires-Dist: scipy
 Requires-Dist: sentence_transformers>=2.2.0
 Requires-Dist: torch
 Requires-Dist: tqdm
 Requires-Dist: rich
-Requires-Dist: pytrec_eval
+Requires-Dist: pytrec-eval-terrier>=0.5.6
 Requires-Dist: pydantic
 Requires-Dist: typing_extensions
 Requires-Dist: eval_type_backport
 Provides-Extra: dev
 Requires-Dist: ruff>=0.0.254; extra == "dev"
 Requires-Dist: pytest; extra == "dev"
 Requires-Dist: pytest-xdist; extra == "dev"
```

### Comparing `mteb-1.3.4/mteb.egg-info/SOURCES.txt` & `mteb-1.4.0/mteb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/pyproject.toml` & `mteb-1.4.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=42", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mteb"
-version = "1.3.4"
+version = "1.4.0"
 description = "Massive Text Embedding Benchmark"
 readme = "README.md"
 authors = [
     { name = "MTEB Contributors", email = "niklas@huggingface.co" },
     { email = "nouamane@huggingface.co" },
     { email = "info@nils-reimers.de" },
 ]
@@ -31,15 +31,15 @@
     "requests>=2.26.0",
     "scikit_learn>=1.0.2",
     "scipy",
     "sentence_transformers>=2.2.0",
     "torch",
     "tqdm",
     "rich",
-    "pytrec_eval",
+    "pytrec-eval-terrier>=0.5.6",
     "pydantic",
     "typing_extensions",
     "eval_type_backport",
 ]
 
 
 [project.urls]
```

### Comparing `mteb-1.3.4/scripts/data/amazon_polarity/create_data.py` & `mteb-1.4.0/scripts/data/amazon_polarity/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/data/amazon_reviews_multi/create_data.py` & `mteb-1.4.0/scripts/data/amazon_reviews_multi/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/data/arxiv/script_clustering.py` & `mteb-1.4.0/scripts/data/arxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/data/arxiv/script_raw.py` & `mteb-1.4.0/scripts/data/arxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/data/biorxiv/script_clustering.py` & `mteb-1.4.0/scripts/data/biorxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/data/biorxiv/script_raw.py` & `mteb-1.4.0/scripts/data/biorxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/data/bucc/create_data.py` & `mteb-1.4.0/scripts/data/bucc/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/data/create_task_table.py` & `mteb-1.4.0/scripts/data/create_task_table.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/data/germanquad/process_data.py` & `mteb-1.4.0/scripts/data/germanquad/process_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/data/hal/create_data.py` & `mteb-1.4.0/scripts/data/hal/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/data/imdb/create_data.py` & `mteb-1.4.0/scripts/data/imdb/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/data/medrxiv/script_clustering.py` & `mteb-1.4.0/scripts/data/medrxiv/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/data/medrxiv/script_raw.py` & `mteb-1.4.0/scripts/data/medrxiv/script_raw.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/data/mind/prepare_data.py` & `mteb-1.4.0/scripts/data/mind/prepare_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/data/redditp2p/script_clustering.py` & `mteb-1.4.0/scripts/data/redditp2p/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/data/stackexchangep2p/script_clustering.py` & `mteb-1.4.0/scripts/data/stackexchangep2p/script_clustering.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/data/sts22-crosslingual-sts/create_data.py` & `mteb-1.4.0/scripts/data/sts22-crosslingual-sts/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/data/summeval_fr/create_data.py` & `mteb-1.4.0/scripts/data/summeval_fr/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/data/toxic_conversations_50k/create_data.py` & `mteb-1.4.0/scripts/data/toxic_conversations_50k/create_data.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/merge_cqadupstack.py` & `mteb-1.4.0/scripts/merge_cqadupstack.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/mteb_meta.py` & `mteb-1.4.0/scripts/mteb_meta.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/run_mteb_chinese.py` & `mteb-1.4.0/scripts/run_mteb_chinese.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/run_mteb_english.py` & `mteb-1.4.0/scripts/run_mteb_english.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/run_mteb_french.py` & `mteb-1.4.0/scripts/run_mteb_french.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/run_mteb_german.py` & `mteb-1.4.0/scripts/run_mteb_german.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/run_mteb_korean.py` & `mteb-1.4.0/scripts/run_mteb_korean.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/scripts/run_mteb_polish.py` & `mteb-1.4.0/scripts/run_mteb_polish.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/tests/test_ClusteringEvaluator.py` & `mteb-1.4.0/tests/test_ClusteringEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/tests/test_PairClassificationEvaluator.py` & `mteb-1.4.0/tests/test_PairClassificationEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/tests/test_RerankingEvaluator.py` & `mteb-1.4.0/tests/test_RerankingEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/tests/test_RetrievalEvaluator.py` & `mteb-1.4.0/tests/test_RetrievalEvaluator.py`

 * *Files identical despite different names*

### Comparing `mteb-1.3.4/tests/test_all_abstasks.py` & `mteb-1.4.0/tests/test_all_abstasks.py`

 * *Files identical despite different names*

