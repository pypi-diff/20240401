# Comparing `tmp/eptr2-0.2.3.tar.gz` & `tmp/eptr2-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eptr2-0.2.3.tar", max compression
+gzip compressed data, was "eptr2-0.3.0.tar", max compression
```

## Comparing `eptr2-0.2.3.tar` & `eptr2-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,21 @@
--rw-r--r--   0        0        0    11357 2023-11-15 12:19:13.028669 eptr2-0.2.3/LICENSE
--rw-r--r--   0        0        0     4371 2024-01-31 13:55:19.157264 eptr2-0.2.3/README.md
--rw-r--r--   0        0        0       48 2023-11-24 09:44:59.967784 eptr2-0.2.3/eptr2/__init__.py
--rw-r--r--   0        0        0     5478 2024-02-23 09:41:05.037172 eptr2-0.2.3/eptr2/main.py
--rw-r--r--   0        0        0      248 2023-12-16 08:05:15.039389 eptr2-0.2.3/eptr2/mapping/__init__.py
--rw-r--r--   0        0        0    63289 2024-01-31 13:55:19.160996 eptr2-0.2.3/eptr2/mapping/help.py
--rw-r--r--   0        0        0     7420 2024-02-23 09:41:05.037386 eptr2-0.2.3/eptr2/mapping/parameters.py
--rw-r--r--   0        0        0    23239 2024-02-16 13:25:59.575358 eptr2-0.2.3/eptr2/mapping/path.py
--rw-r--r--   0        0        0     3105 2024-02-16 13:25:59.575681 eptr2-0.2.3/eptr2/mapping/processing.py
--rw-r--r--   0        0        0      183 2023-12-08 13:25:19.644848 eptr2-0.2.3/eptr2/processing/__init__.py
--rw-r--r--   0        0        0        0 2023-12-08 13:25:19.644898 eptr2-0.2.3/eptr2/processing/postprocess/__init__.py
--rw-r--r--   0        0        0      829 2024-01-31 13:55:19.162404 eptr2-0.2.3/eptr2/processing/postprocess/items.py
--rw-r--r--   0        0        0        0 2023-11-24 09:44:59.970042 eptr2-0.2.3/eptr2/processing/preprocess/__init__.py
--rw-r--r--   0        0        0     1502 2024-02-23 09:41:05.037560 eptr2-0.2.3/eptr2/processing/preprocess/params.py
--rw-r--r--   0        0        0        0 2023-11-24 09:44:59.970736 eptr2-0.2.3/eptr2/util/__init__.py
--rw-r--r--   0        0        0     3161 2023-12-05 12:02:08.460583 eptr2-0.2.3/eptr2/util/certificate.py
--rw-r--r--   0        0        0     6527 2024-03-21 10:11:19.451330 eptr2-0.2.3/eptr2/util/costs.py
--rw-r--r--   0        0        0     1207 2024-01-10 14:14:00.769596 eptr2-0.2.3/eptr2/util/evaluation.py
--rw-r--r--   0        0        0     3759 2023-11-27 07:59:15.415246 eptr2-0.2.3/eptr2/util/time.py
--rw-r--r--   0        0        0      434 2024-03-21 10:11:19.452909 eptr2-0.2.3/pyproject.toml
--rw-r--r--   0        0        0     4931 1970-01-01 00:00:00.000000 eptr2-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-11-15 12:19:13.028669 eptr2-0.3.0/LICENSE
+-rw-r--r--   0        0        0     3132 2024-04-01 16:49:22.653196 eptr2-0.3.0/README.md
+-rw-r--r--   0        0        0       48 2023-11-24 09:44:59.967784 eptr2-0.3.0/eptr2/__init__.py
+-rw-r--r--   0        0        0     5846 2024-04-01 16:46:11.719108 eptr2-0.3.0/eptr2/main.py
+-rw-r--r--   0        0        0      248 2024-04-01 16:47:02.813358 eptr2-0.3.0/eptr2/mapping/__init__.py
+-rw-r--r--   0        0        0    74878 2024-04-01 16:19:34.773267 eptr2-0.3.0/eptr2/mapping/help.py
+-rw-r--r--   0        0        0     7683 2024-04-01 16:36:27.545931 eptr2-0.3.0/eptr2/mapping/parameters.py
+-rw-r--r--   0        0        0    24542 2024-04-01 16:41:59.019233 eptr2-0.3.0/eptr2/mapping/path.py
+-rw-r--r--   0        0        0     3240 2024-04-01 16:35:34.003858 eptr2-0.3.0/eptr2/mapping/processing.py
+-rw-r--r--   0        0        0      183 2024-04-01 16:47:13.041852 eptr2-0.3.0/eptr2/processing/__init__.py
+-rw-r--r--   0        0        0        0 2023-12-08 13:25:19.644898 eptr2-0.3.0/eptr2/processing/postprocess/__init__.py
+-rw-r--r--   0        0        0      829 2024-01-31 13:55:19.162404 eptr2-0.3.0/eptr2/processing/postprocess/items.py
+-rw-r--r--   0        0        0        0 2023-11-24 09:44:59.970042 eptr2-0.3.0/eptr2/processing/preprocess/__init__.py
+-rw-r--r--   0        0        0     1502 2024-02-23 09:41:05.037560 eptr2-0.3.0/eptr2/processing/preprocess/params.py
+-rw-r--r--   0        0        0        0 2023-11-24 09:44:59.970736 eptr2-0.3.0/eptr2/util/__init__.py
+-rw-r--r--   0        0        0     3161 2023-12-05 12:02:08.460583 eptr2-0.3.0/eptr2/util/certificate.py
+-rw-r--r--   0        0        0     6527 2024-03-21 10:11:19.451330 eptr2-0.3.0/eptr2/util/costs.py
+-rw-r--r--   0        0        0     1207 2024-01-10 14:14:00.769596 eptr2-0.3.0/eptr2/util/evaluation.py
+-rw-r--r--   0        0        0     3759 2023-11-27 07:59:15.415246 eptr2-0.3.0/eptr2/util/time.py
+-rw-r--r--   0        0        0      513 2024-04-01 16:50:03.100488 eptr2-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3770 1970-01-01 00:00:00.000000 eptr2-0.3.0/PKG-INFO
```

### Comparing `eptr2-0.2.3/LICENSE` & `eptr2-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `eptr2-0.2.3/eptr2/main.py` & `eptr2-0.3.0/eptr2/main.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,38 +1,48 @@
-import os
 from typing import Any
-import pandas as pd
-import json
 import requests
 import re
 from urllib.parse import urljoin
 import copy
 from eptr2.mapping import (
     get_total_path,
     get_call_method,
     get_required_parameters,
     get_param_label,
     get_path_map,
     get_optional_parameters,
 )
 from warnings import warn
-from eptr2.processing import preprocess_parameter, postprocess_items_to_df
+from eptr2.processing import preprocess_parameter
 from eptr2.mapping import get_postprocess_function
 
 
 class EPTR2:
     def __init__(self, **kwargs) -> None:
         ## kwargs are
         ### map_param_labels: bool
         ### secure: bool
         ### query_parameters: dict
         ### just_call_phrase: bool
         self.ssl_verify = kwargs.get("ssl_verify", True)
         self.postprocess = kwargs.get("postprocess", True)
 
+        # try:
+        #     import pandas as pd
+        # except ImportError:
+        #     warn(
+        #         "pandas is not installed. Some functionalities may not work properly. Postprocessing is disabled.",
+        #         ImportWarning,
+        #         stacklevel=2,
+        #     )
+        #     self.postprocess = False
+
+        # if self.postprocess:
+        #     from eptr2.mapping import get_postprocess_function
+
     ## Ref: https://stackoverflow.com/a/62303969/3608936
     def __getattr__(self, __name: str) -> Any:
         def method(*args, **kwargs):
             key_raw = __name
             key = re.sub("_", "-", key_raw)
             if key not in get_path_map(just_call_keys=True):
                 raise Exception(
```

### Comparing `eptr2-0.2.3/eptr2/mapping/help.py` & `eptr2-0.3.0/eptr2/mapping/help.py`

 * *Files 8% similar despite different names*

```diff
@@ -451,26 +451,206 @@
             },
             "desc": {
                 "tr": "(Açıklama Yok)",
                 "en": "(No description)",
             },
             "url": "https://seffaflik.epias.com.tr/electricity/electricity-market-reports/mcp-smp-and-imbalance-price-listing",
         },
+        "idm-summary": {
+            "category": "Elektrik Piyasası Raporları",
+            "title": {
+                "tr": "GİP Kontrat Özeti",
+                "en": "IDM Contract Summary",
+            },
+            "desc": {
+                "tr": "(Açıklama Yok)",
+                "en": "(No description)",
+            },
+            "url": "https://seffaflik.epias.com.tr/electricity/electricity-market-reports/idm-contract-summary",
+        },
+        "idm-contract-list": {
+            "category": "Elektrik Piyasası Raporları",
+            "title": {
+                "tr": "GİP Kontrat Listesi",
+                "en": "IDM Contract List",
+            },
+            "desc": {
+                "tr": "(Açıklama Yok)",
+                "en": "(No description)",
+            },
+            "url": "https://seffaflik.epias.com.tr/electricity/electricity-market-reports/idm-order-list",
+        },
+        "idm-contract-list": {
+            "category": "Elektrik Piyasası Raporları",
+            "title": {
+                "tr": "GİP Teklif Listesi",
+                "en": "IDM Order List",
+            },
+            "desc": {
+                "tr": "(Açıklama Yok)",
+                "en": "(No description)",
+            },
+            "url": "https://seffaflik.epias.com.tr/electricity/electricity-market-reports/idm-order-list",
+        },
+        "electricity-market-quantity": {
+            "category": "Elektrik Piyasası Raporları",
+            "title": {
+                "tr": "Elektrik Piyasa Hacimleri Fiziksel",
+                "en": "Electricity Market Volume Physically",
+            },
+            "desc": {
+                "tr": "(Açıklama Yok)",
+                "en": "(No description)",
+            },
+            "url": "https://seffaflik.epias.com.tr/electricity/electricity-market-reports/electricity-market-volume-physically",
+        },
         "bpm-orders-w-avg": {
             "category": "Elektrik Piyasası Raporları",
             "title": {
                 "tr": "DGP Talimatları (Ağırlıklı Ortalama)",
                 "en": "BPM Instructions (Weighted Average)",
             },
             "desc": {
                 "tr": "(Açıklama Yok)",
                 "en": "(No description)",
             },
             "url": "https://seffaflik.epias.com.tr/electricity/electricity-market-reports/bpm-instructions-weighted-average",
         },
+        "dams-daily-level": {
+            "category": "Barajlar",
+            "title": {
+                "tr": "Günlük Kot",
+                "en": "Daily Kot",
+            },
+            "desc": {
+                "tr": "Barajın ilgili gündeki su yüksekliğini belirtir. Veriler saat 17:00 itibariyle nihai halini almaktadır.",
+                "en": "Indicates the water height of the dam on the relevant day. The data is finalized as of 5 pm.",
+            },
+            "url": "https://seffaflik.epias.com.tr/electricity/dams/daily-kot",
+        },
+        "dams-daily-volume": {
+            "category": "Barajlar",
+            "title": {
+                "tr": "Günlük Hacim",
+                "en": "Daily Volume",
+            },
+            "desc": {
+                "tr": "Bir barajın ilgili tarihteki seviyesine karşılık gelen hacimdir. Veriler saat 17:00 itibariyle nihai halini almaktadır.",
+                "en": "The volume corresponding to the level of a dam at the relevant date. Data is finalized at 17:00.",
+            },
+            "url": "https://seffaflik.epias.com.tr/electricity/dams/daily-volume",
+        },
+        "dams-active-fullness": {
+            "category": "Barajlar",
+            "title": {
+                "tr": "Aktif Doluluk",
+                "en": "Active Fullness",
+            },
+            "desc": {
+                "tr": "Bir barajın maksimum ve minimum işletme seviyeleri arasındaki hacimin yüzdesidir. Formül: Aktif Doluluk= [( İlgili Tarihteki Seviyeye Karşılık Gelen Hacim – Minimum Hacim ) / ( Maksimum Hacim – Minimum Hacim )] * 100. Veriler saat 17:00 itibariyle nihai halini almaktadır.",
+                "en": "The percentage of volume between the maximum and minimum operating levels of a dam. Formula: Active Occupancy= [( Volume Corresponding to the Level on the Relevant Date - Minimum Volume ) / ( Maximum Volume - Minimum Volume )] *100. Data is finalized as of 17:00.",
+            },
+            "url": "https://seffaflik.epias.com.tr/electricity/dams/active-fullness",
+        },
+        "dams-active-volume": {
+            "category": "Barajlar",
+            "title": {
+                "tr": "Aktif Hacim",
+                "en": "Active Volume",
+            },
+            "desc": {
+                "tr": "Bir barajın ilgili tarihteki seviyeye karşılık gelen hacmi ve minimum işletme seviyeleri arasındaki hacimdir. Veriler saat 17:00 itibariyle nihai halini almaktadır.",
+                "en": "The volume between the minimum volume and minimum operating levels of a dam at the relevant date. Data is finalized at 17:00.",
+            },
+            "url": "https://seffaflik.epias.com.tr/electricity/dams/active-volume",
+        },
+        "dams-water-energy-provision": {
+            "category": "Barajlar",
+            "title": {
+                "tr": "Suyun Enerji Karşılığı",
+                "en": "Water Energy Provision",
+            },
+            "desc": {
+                "tr": "Barajda yer alan suyun hesaplanan MWh cinsinden enerji karşılığıdır. Veriler saat 17:00 itibariyle nihai halini almaktadır.",
+                "en": "The energy equivalent of Mwh in the dam. Data is finalized at 17:00.",
+            },
+            "url": "https://seffaflik.epias.com.tr/electricity/dams/water-energy-provision",
+        },
+        "dams-level-minmax": {
+            "category": "Barajlar",
+            "title": {
+                "tr": "Kot",
+                "en": "Kot",
+            },
+            "desc": {
+                "tr": "İlgili barajın maximum ve minumum seviyesini gösterir.",
+                "en": "Indicates the minimum and maximum water level of the dam.",
+            },
+            "url": "https://seffaflik.epias.com.tr/electricity/dams/dam-info/kot",
+        },
+        "dams-volume-minmax": {
+            "category": "Barajlar",
+            "title": {
+                "tr": "Hacim",
+                "en": "Volume",
+            },
+            "desc": {
+                "tr": "İlgili barajın maksimum ve minumum hacim seviyesini gösterir.",
+                "en": "It shows the maximum and minimum volume level of the relevant dam.",
+            },
+            "url": "https://seffaflik.epias.com.tr/electricity/dams/dam-info/volume",
+        },
+        "dams-info": {
+            "category": "Barajlar",
+            "title": {
+                "tr": "Debi ve Kurulu Güç",
+                "en": "Flow Rate and Installed Power",
+            },
+            "desc": {
+                "tr": "İlgili barajda üniteden geçen suyun miktarını ve barajın kurulu gücünü gösterir.",
+                "en": "It shows the amount of water passing through the unit in the relevant dam and the installed power of the dam.",
+            },
+            "url": "https://seffaflik.epias.com.tr/electricity/dams/dam-info/volume",
+        },
+        "dam-list": {
+            "category": "Barajlar",
+            "title": {
+                "tr": "Baraj Listesi",
+                "en": "Dam List",
+            },
+            "desc": {
+                "tr": "Barajların listesini döner.",
+                "en": "Returns the list of dams.",
+            },
+            "url": "https://seffaflik.epias.com.tr/electricity/dams/daily-kot",
+        },
+        "basin-list": {
+            "category": "Barajlar",
+            "title": {
+                "tr": "Havza Listesi",
+                "en": "Basin List",
+            },
+            "desc": {
+                "tr": "Havzaların listesini döner.",
+                "en": "Returns the list of basins.",
+            },
+            "url": "https://seffaflik.epias.com.tr/electricity/dams/daily-kot",
+        },
+        "bpm-orders": {
+            "category": "Elektrik Piyasası Raporları",
+            "title": {
+                "tr": "DGP Talimatları",
+                "en": "BPM Instructions",
+            },
+            "desc": {
+                "tr": "(Açıklama Yok)",
+                "en": "(No description)",
+            },
+            "url": "https://seffaflik.epias.com.tr/electricity/electricity-market-reports/bpm-instructions",
+        },
         "kgup": {
             "category": "Üretim Planlama",
             "title": {
                 "tr": "Kesinleşmiş Günlük Üretim Planı (KGÜP)",
                 "en": "Final Daily Production Program (FDPP)",
             },
             "desc": {
@@ -667,14 +847,62 @@
             },
             "desc": {
                 "tr": "Uzlaştırmaya esas çekiş birimlerinin, tedarik yükümlülüğü kapsamında sistemden aldığı enerji miktarlarının toplam değerine ilişkin veri seti",
                 "en": "The data set regarding total energy withdrawal quantity under supply liability of withdrawal units.",
             },
             "url": "https://seffaflik.epias.com.tr/electricity/electricity-consumption/ex-post-consumption/withdrawal-quantity-under-supply-liability",
         },
+        "anc-pf-qty": {
+            "category": "Yan Hizmetler",
+            "title": {
+                "tr": "Primer Frekans Rezerv Miktarı",
+                "en": "Primary Frequency Capacity Amount",
+            },
+            "desc": {
+                "tr": "Katılımcıların gerçek zamanlı frekans dengeleme için ayırması gereken saatlik toplam birincil frekans kapasite hacimleridir.",
+                "en": "It displays hourly total primary frequency capacity volume that the participants need to reserve for the real time frequency balancing.",
+            },
+            "url": "https://seffaflik.epias.com.tr/electricity/electricity-markets/ancillary-services/primary-frequency-capacity-amount",
+        },
+        "anc-pfk": {
+            "category": "Yan Hizmetler",
+            "title": {
+                "tr": "Primer Frekans Kontrolü (PFK) Fiyat",
+                "en": "Primary Frequency Capacity Price (PFCP)",
+            },
+            "desc": {
+                "tr": "Saatlik bazda ihale ile belirlenen PFK kapasite bedelidir.",
+                "en": "It displays Primary Frequency Capacity Price determined by the tender on an hourly basis. Tenders are held by Transmission System Operator.",
+            },
+            "url": "https://seffaflik.epias.com.tr/electricity/electricity-markets/ancillary-services/primary-frequency-capacity-price-pfcp",
+        },
+        "anc-sf-qty": {
+            "category": "Yan Hizmetler",
+            "title": {
+                "tr": "Sekonder Frekans Rezerv Miktarı",
+                "en": "Secondary Frequency Capacity Amount",
+            },
+            "desc": {
+                "tr": "Saatlik toplam belirlenen rezerv miktarlarıdır.",
+                "en": "It displays hourly total secondary frequency capacity volume that the participants need to reserve for the real time frequency balancing.",
+            },
+            "url": "https://seffaflik.epias.com.tr/electricity/electricity-markets/ancillary-services/secondary-frequency-capacity-amount",
+        },
+        "anc-sfk": {
+            "category": "Yan Hizmetler",
+            "title": {
+                "tr": "Sekonder Frekans Kontrolü (SFK) Fiyat",
+                "en": "Secondary Frequency Capacity Price (SFCP)",
+            },
+            "desc": {
+                "tr": "Saatlik bazda ihale ile belirlenen SFK kapasite bedelidir.",
+                "en": "It displays Secondary Frequency Capacity Price determined by the tender on an hourly basis. Tenders are held by Transmission System Operator.",
+            },
+            "url": "https://seffaflik.epias.com.tr/electricity/electricity-markets/ancillary-services/secondary-frequency-capacity-price-sfcp",
+        },
         "wind-forecast": {
             "category": "Üretim",
             "title": {
                 "tr": "RES Üretim ve Tahmin",
                 "en": "WPP Generation and Forecast",
             },
             "desc": {
@@ -1057,14 +1285,26 @@
             },
             "desc": {
                 "tr": "Piyasa Katılımcıları’nın organizasyon listesi.",
                 "en": "Market Participants organization list.",
             },
             "url": "https://seffaflik.epias.com.tr/electricity/electricity-markets/general-data/market-participants",
         },
+        "participant-count-based-upon-license-type": {
+            "category": "Listeleme",
+            "title": {
+                "tr": "Lisans Türüne Göre Katılımcı Sayısı",
+                "en": "Participant Count Based Upon License Type",
+            },
+            "desc": {
+                "tr": "Kamu ve Özel Sektör piyasa katılımcılarının Üretim, Tedarik, Dağıtım, OSB Üretim, İletim ve Görevli Tedaril lisansları türlerine göre toplam sayılarını gösterir. Görevli tedarik şirketleri tüketici grupları için K1 (21), K2 (21) ve K3 (21) olacak şekilde kategorize edilmiştir.",
+                "en": "It indicates the number of market participants by the licence types.",
+            },
+            "url": "https://seffaflik.epias.com.tr/electricity/electricity-markets/general-data/participant-count-based-upon-license-type",
+        },
         "dams-active-fullness": {
             "category": "Barajlar",
             "title": {
                 "tr": "Aktif Doluluk",
                 "en": "Active Fullness",
             },
             "desc": {
```

### Comparing `eptr2-0.2.3/eptr2/mapping/parameters.py` & `eptr2-0.3.0/eptr2/mapping/parameters.py`

 * *Files 1% similar despite different names*

```diff
@@ -134,14 +134,19 @@
         "dams-volume-minmax": [],
         "dams-info": [],
         "dams-water-energy-provision": [],
         "idm-summary": ["start_date", "end_date"],
         "electricity-market-quantity": ["start_date", "end_date"],
         "idm-contract-list": ["se_date"],
         "idm-order-history": ["se_date", "idm_contract_id"],
+        "participant-count-based-upon-license-type": ["start_date"],
+        "anc-pf-qty": ["start_date", "end_date"],
+        "anc-pfk": ["start_date", "end_date"],
+        "anc-sf-qty": ["start_date", "end_date"],
+        "anc-sfk": ["start_date", "end_date"],
     }
     ## UPDATE: As a precaution every call should have an input parameter
     return d[key]
 
 
 def get_optional_parameters(key):
     d = {
```

### Comparing `eptr2-0.2.3/eptr2/mapping/path.py` & `eptr2-0.3.0/eptr2/mapping/path.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,14 +312,38 @@
             },
             ## Tedarik Yükümlülüğü Kapsamındaki UEÇM
             "su-uecm": {
                 "prefix": "data",
                 "prev": "consumption",
                 "label": "withdrawal-quantity-under-supply-liability",
             },
+            ## Yan Hizmetler - Primer Frekans Rezerv Miktarı
+            "anc-pf-qty": {
+                "prefix": "data",
+                "prev": "ancillary-services",
+                "label": "primary-frequency-capacity-amount",
+            },
+            ## Yan Hizmetler - Primer Frekans Kapasite fiyatı (PFK)
+            "anc-pfk": {
+                "prefix": "data",
+                "prev": "ancillary-services",
+                "label": "primary-frequency-capacity-price",
+            },
+            ## Yan Hizmetler - Sekonder Frekans Rezerv Miktarı
+            "anc-sf-qty": {
+                "prefix": "data",
+                "prev": "ancillary-services",
+                "label": "secondary-frequency-capacity-amount",
+            },
+            ## Yan Hizmetler - Sekonder Frekans Kapasite fiyatı (SFK)
+            "anc-sfk": {
+                "prefix": "data",
+                "prev": "ancillary-services",
+                "label": "secondary-frequency-capacity-price",
+            },
             ## YEKDEM RES Üretim ve Tahmin Listeleme
             "wind-forecast": {
                 "prefix": "data",
                 "prev": "renewables",
                 "label": "res-generation-and-forecast",
             },
             ## YEKDEM Santral Listesi
@@ -404,15 +428,14 @@
             ## Kısıt Maliyeti
             "congestion-cost": {
                 "prefix": "data",
                 "prev": "transmission",
                 "label": "congestion-cost",
             },
             ##ENTSO-E (X) Kodları
-            ## TODO: Fix
             "eic-x-org-list": {
                 "prefix": "data",
                 "prev": "transmission",
                 "label": "organization-list",
             },
             ##ENTSO-E (W) Kodları
             "eic-w-org-list": {
@@ -506,14 +529,20 @@
             },
             ##Piyasa Katılımcıları Organizasyon
             "market-participants-organization-list": {
                 "prefix": "data",
                 "prev": "general-data",
                 "label": "market-participants-organization-filter-list",
             },
+            ##Lisans Türüne Göre Katılımcı Sayısı
+            "participant-count-based-upon-license-type": {
+                "prefix": "data",
+                "prev": "general-data",
+                "label": "participant-count-based-upon-license-type",
+            },
             ## Aktif Doluluk
             "dams-active-fullness": {
                 "prefix": "data",
                 "prev": "dams",
                 "label": "active-fullness",
             },
             ## Günlük Kot
@@ -602,14 +631,15 @@
         "bilateral-contracts": {"prev": "markets"},
         "general-data": {"prev": "markets"},
         "imbalance": {"prev": "markets"},
         "dams": {"prev": "electricity-service"},
         "markets": {"prev": "electricity-service"},
         "generation": {"prev": "electricity-service"},
         "consumption": {"prev": "electricity-service"},
+        "ancillary-services": {"prev": "markets"},
         "renewables": {"prev": "electricity-service"},
         "transmission": {"prev": "electricity-service"},
         #### services
         "electricity-service": {"next": "version"},
         "reporting-service": {"next": "version"},
         "version": {"label": "v1"},
     }
```

### Comparing `eptr2-0.2.3/eptr2/mapping/processing.py` & `eptr2-0.3.0/eptr2/mapping/processing.py`

 * *Files 10% similar despite different names*

```diff
@@ -45,14 +45,15 @@
         "imb-org-list",
         "interim-mcp",
         "mcp-smp-imb",
         "bpm-orders-w-avg",
         "bpm-orders",
         "market-participants",
         "market-participants-organization-list",
+        "participant-count-based-upon-license-type",
         "kgup",
         "kudup",
         "eak",
         "gen-org",
         "gen-uevcb",
         "rt-gen",
         "pp-list",
@@ -99,14 +100,18 @@
         "dams-volume-minmax",
         "dams-info",
         "dams-water-energy-provision",
         "idm-summary",
         "electricity-market-quantity",
         "idm-contract-list",
         "idm-order-history",
+        "anc-pf-qty",
+        "anc-sf-qty",
+        "anc-pfk",
+        "anc-sfk",
     ]:
         return postprocess_items_to_df
 
     elif key in ["interim-mcp-status"]:
         return postprocess_mcp_status
 
     elif key in [
```

### Comparing `eptr2-0.2.3/eptr2/processing/postprocess/items.py` & `eptr2-0.3.0/eptr2/processing/postprocess/items.py`

 * *Files identical despite different names*

### Comparing `eptr2-0.2.3/eptr2/processing/preprocess/params.py` & `eptr2-0.3.0/eptr2/processing/preprocess/params.py`

 * *Files identical despite different names*

### Comparing `eptr2-0.2.3/eptr2/util/certificate.py` & `eptr2-0.3.0/eptr2/util/certificate.py`

 * *Files identical despite different names*

### Comparing `eptr2-0.2.3/eptr2/util/costs.py` & `eptr2-0.3.0/eptr2/util/costs.py`

 * *Files identical despite different names*

### Comparing `eptr2-0.2.3/eptr2/util/evaluation.py` & `eptr2-0.3.0/eptr2/util/evaluation.py`

 * *Files identical despite different names*

### Comparing `eptr2-0.2.3/eptr2/util/time.py` & `eptr2-0.3.0/eptr2/util/time.py`

 * *Files identical despite different names*

