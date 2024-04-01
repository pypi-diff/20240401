# Comparing `tmp/tencentcloud-sdk-python-3.0.998.tar.gz` & `tmp/tencentcloud-sdk-python-3.0.999.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/data/__qci/root-workspaces/__qci-pipeline-732314-1/python_sdk/tencentcloud-sdk-python/dist/tmp5mwrndf1/tencentcloud-sdk-python", last modified: Fri Oct 13 00:18:45 2023, max compression
+gzip compressed data, was "/data/__qci/root-workspaces/__qci-pipeline-732314-1/python_sdk/tencentcloud-sdk-python/dist/tmpnaggkeg8/tencentcloud-sdk-python", last modified: Mon Oct 16 00:17:37 2023, max compression
```

## Comparing `tencentcloud-sdk-python-3.0.998.tar` & `tencentcloud-sdk-python-3.0.999.tar`

### file list

```diff
@@ -1,1921 +1,1921 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/
--rw-r--r--   0 root         (0) root         (0)      683 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/tdsql.py
--rw-r--r--   0 root         (0) root         (0)      687 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/scaling.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/live.py
--rw-r--r--   0 root         (0) root         (0)      787 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/ccr.py
--rw-r--r--   0 root         (0) root         (0)      683 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/redis.py
--rw-r--r--   0 root         (0) root         (0)      785 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/tmt.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/bill.py
--rw-r--r--   0 root         (0) root         (0)      811 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/dc.py
--rw-r--r--   0 root         (0) root         (0)      685 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/yunsou.py
--rw-r--r--   0 root         (0) root         (0)      780 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/sts.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/__init__.py
--rw-r--r--   0 root         (0) root         (0)      683 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/bmeip.py
--rw-r--r--   0 root         (0) root         (0)      776 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/emr.py
--rw-r--r--   0 root         (0) root         (0)      685 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/wenzhi.py
--rw-r--r--   0 root         (0) root         (0)      677 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/bm.py
--rw-r--r--   0 root         (0) root         (0)      683 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/trade.py
--rw-r--r--   0 root         (0) root         (0)      679 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/cbs.py
--rw-r--r--   0 root         (0) root         (0)      717 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/scf.py
--rw-r--r--   0 root         (0) root         (0)      679 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/dfw.py
--rw-r--r--   0 root         (0) root         (0)      680 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/sec.py
--rw-r--r--   0 root         (0) root         (0)      679 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/cns.py
--rw-r--r--   0 root         (0) root         (0)      683 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/image.py
--rw-r--r--   0 root         (0) root         (0)      679 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/eip.py
--rw-r--r--   0 root         (0) root         (0)      679 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/ccs.py
--rw-r--r--   0 root         (0) root         (0)      691 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/feecenter.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/cmem.py
--rw-r--r--   0 root         (0) root         (0)      802 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/athena.py
--rw-r--r--   0 root         (0) root         (0)      693 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/cloudaudit.py
--rw-r--r--   0 root         (0) root         (0)      683 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/bmvpc.py
--rw-r--r--   0 root         (0) root         (0)      679 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/vpc.py
--rw-r--r--   0 root         (0) root         (0)      793 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/tbaas.py
--rw-r--r--   0 root         (0) root         (0)      679 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/vod.py
--rw-r--r--   0 root         (0) root         (0)      693 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/apigateway.py
--rw-r--r--   0 root         (0) root         (0)      677 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/lb.py
--rw-r--r--   0 root         (0) root         (0)      685 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/market.py
--rw-r--r--   0 root         (0) root         (0)      683 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/bgpip.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/partners.py
--rw-r--r--   0 root         (0) root         (0)      687 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/monitor.py
--rw-r--r--   0 root         (0) root         (0)      681 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/bmlb.py
--rw-r--r--   0 root         (0) root         (0)      689 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/snapshot.py
--rw-r--r--   0 root         (0) root         (0)     1346 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/cdn.py
--rw-r--r--   0 root         (0) root         (0)      687 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/account.py
--rw-r--r--   0 root         (0) root         (0)      683 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/batch.py
--rw-r--r--   0 root         (0) root         (0)     5487 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/base.py
--rw-r--r--   0 root         (0) root         (0)      679 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/cdb.py
--rw-r--r--   0 root         (0) root         (0)      679 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/modules/cvm.py
--rw-r--r--   0 root         (0) root         (0)       23 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/common/
--rw-r--r--   0 root         (0) root         (0)     1378 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/common/api_exception.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/common/sign.py
--rw-r--r--   0 root         (0) root         (0)     5077 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/common/request.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/common/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6751 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/QcloudApi/qcloudapi.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud_sdk_python.egg-info/
--rw-r--r--   0 root         (0) root         (0)       23 2023-10-13 00:18:44.000000 tencentcloud-sdk-python-3.0.998/tencentcloud_sdk_python.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-10-13 00:18:44.000000 tencentcloud-sdk-python-3.0.998/tencentcloud_sdk_python.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)     1475 2023-10-13 00:18:44.000000 tencentcloud-sdk-python-3.0.998/tencentcloud_sdk_python.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)    54224 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud_sdk_python.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-10-13 00:18:44.000000 tencentcloud-sdk-python-3.0.998/tencentcloud_sdk_python.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)    11351 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/LICENSE
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/asr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/asr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/asr/v20190614/
--rw-r--r--   0 root         (0) root         (0)    30288 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/asr/v20190614/asr_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/asr/v20190614/__init__.py
--rw-r--r--   0 root         (0) root         (0)   119460 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/asr/v20190614/models.py
--rw-r--r--   0 root         (0) root         (0)     7627 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/asr/v20190614/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/oceanus/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/oceanus/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/oceanus/v20190422/
--rw-r--r--   0 root         (0) root         (0)    25417 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/oceanus/v20190422/oceanus_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/oceanus/v20190422/__init__.py
--rw-r--r--   0 root         (0) root         (0)   247703 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/oceanus/v20190422/models.py
--rw-r--r--   0 root         (0) root         (0)     9664 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/oceanus/v20190422/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bma/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bma/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bma/v20221115/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bma/v20221115/__init__.py
--rw-r--r--   0 root         (0) root         (0)    66446 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bma/v20221115/models.py
--rw-r--r--   0 root         (0) root         (0)     3348 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bma/v20221115/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    10571 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bma/v20221115/bma_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bma/v20210624/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bma/v20210624/__init__.py
--rw-r--r--   0 root         (0) root         (0)   146139 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bma/v20210624/models.py
--rw-r--r--   0 root         (0) root         (0)     1829 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bma/v20210624/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    25903 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bma/v20210624/bma_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bm/v20180423/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bm/v20180423/__init__.py
--rw-r--r--   0 root         (0) root         (0)   274077 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bm/v20180423/models.py
--rw-r--r--   0 root         (0) root         (0)    50710 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bm/v20180423/bm_client.py
--rw-r--r--   0 root         (0) root         (0)     1896 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bm/v20180423/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/v20230321/
--rw-r--r--   0 root         (0) root         (0)    17767 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/v20230321/thpc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/v20230321/__init__.py
--rw-r--r--   0 root         (0) root         (0)   167264 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/v20230321/models.py
--rw-r--r--   0 root         (0) root         (0)     4560 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/v20230321/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/v20220401/
--rw-r--r--   0 root         (0) root         (0)    16797 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/v20220401/thpc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/v20220401/__init__.py
--rw-r--r--   0 root         (0) root         (0)   142732 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/v20220401/models.py
--rw-r--r--   0 root         (0) root         (0)     4733 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/v20220401/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/v20211109/
--rw-r--r--   0 root         (0) root         (0)     4628 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/v20211109/thpc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/v20211109/__init__.py
--rw-r--r--   0 root         (0) root         (0)    63030 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/v20211109/models.py
--rw-r--r--   0 root         (0) root         (0)     2035 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/v20211109/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/market/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/market/v20191010/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/market/v20191010/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7313 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/market/v20191010/models.py
--rw-r--r--   0 root         (0) root         (0)      941 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/market/v20191010/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     2922 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/market/v20191010/market_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/market/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/antiddos/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/antiddos/v20200309/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/antiddos/v20200309/__init__.py
--rw-r--r--   0 root         (0) root         (0)   507080 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/antiddos/v20200309/models.py
--rw-r--r--   0 root         (0) root         (0)    89530 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/antiddos/v20200309/antiddos_client.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/antiddos/v20200309/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/antiddos/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vms/v20200902/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vms/v20200902/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10184 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vms/v20200902/models.py
--rw-r--r--   0 root         (0) root         (0)     2741 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vms/v20200902/vms_client.py
--rw-r--r--   0 root         (0) root         (0)     4848 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vms/v20200902/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdc/v20201214/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdc/v20201214/__init__.py
--rw-r--r--   0 root         (0) root         (0)   144909 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdc/v20201214/models.py
--rw-r--r--   0 root         (0) root         (0)     2972 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdc/v20201214/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    19439 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdc/v20201214/cdc_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/asw/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/asw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/asw/v20200722/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/asw/v20200722/__init__.py
--rw-r--r--   0 root         (0) root         (0)    44296 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/asw/v20200722/models.py
--rw-r--r--   0 root         (0) root         (0)      950 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/asw/v20200722/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     9134 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/asw/v20200722/asw_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/pts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/pts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/pts/v20210728/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/pts/v20210728/__init__.py
--rw-r--r--   0 root         (0) root         (0)   310158 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/pts/v20210728/models.py
--rw-r--r--   0 root         (0) root         (0)     2118 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/pts/v20210728/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    39385 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/pts/v20210728/pts_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/wedata/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/wedata/v20210820/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/wedata/v20210820/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1976966 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/wedata/v20210820/models.py
--rw-r--r--   0 root         (0) root         (0)     3640 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/wedata/v20210820/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   276930 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/wedata/v20210820/wedata_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/wedata/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/partners/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/partners/v20180321/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/partners/v20180321/__init__.py
--rw-r--r--   0 root         (0) root         (0)   109523 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/partners/v20180321/models.py
--rw-r--r--   0 root         (0) root         (0)      885 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/partners/v20180321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    19410 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/partners/v20180321/partners_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/partners/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bsca/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bsca/v20210811/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bsca/v20210811/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49093 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bsca/v20210811/models.py
--rw-r--r--   0 root         (0) root         (0)     5975 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bsca/v20210811/bsca_client.py
--rw-r--r--   0 root         (0) root         (0)     1057 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bsca/v20210811/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bsca/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ds/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ds/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ds/v20180523/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ds/v20180523/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49948 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ds/v20180523/models.py
--rw-r--r--   0 root         (0) root         (0)    10034 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ds/v20180523/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    13758 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ds/v20180523/ds_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcex/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcex/v20200727/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcex/v20200727/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8678 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcex/v20200727/models.py
--rw-r--r--   0 root         (0) root         (0)     1712 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcex/v20200727/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     3127 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcex/v20200727/tcex_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcex/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ess/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ess/v20201111/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ess/v20201111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   601905 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ess/v20201111/models.py
--rw-r--r--   0 root         (0) root         (0)   116342 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ess/v20201111/ess_client.py
--rw-r--r--   0 root         (0) root         (0)    24653 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ess/v20201111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ess/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ims/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ims/v20201229/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ims/v20201229/__init__.py
--rw-r--r--   0 root         (0) root         (0)    65090 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ims/v20201229/models.py
--rw-r--r--   0 root         (0) root         (0)     3639 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ims/v20201229/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     8527 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ims/v20201229/ims_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ims/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ims/v20200713/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ims/v20200713/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47064 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ims/v20200713/models.py
--rw-r--r--   0 root         (0) root         (0)     3528 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ims/v20200713/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     3228 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ims/v20200713/ims_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tts/v20190823/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tts/v20190823/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25951 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tts/v20190823/models.py
--rw-r--r--   0 root         (0) root         (0)     5608 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tts/v20190823/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     5886 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tts/v20190823/tts_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mvj/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mvj/v20190926/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mvj/v20190926/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6014 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mvj/v20190926/models.py
--rw-r--r--   0 root         (0) root         (0)     1105 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mvj/v20190926/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     2103 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mvj/v20190926/mvj_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mvj/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ssa/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ssa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ssa/v20180608/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ssa/v20180608/__init__.py
--rw-r--r--   0 root         (0) root         (0)   292973 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ssa/v20180608/models.py
--rw-r--r--   0 root         (0) root         (0)     2265 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ssa/v20180608/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    24532 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ssa/v20180608/ssa_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ssl/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ssl/v20191205/
--rw-r--r--   0 root         (0) root         (0)    55603 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ssl/v20191205/ssl_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ssl/v20191205/__init__.py
--rw-r--r--   0 root         (0) root         (0)   433897 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ssl/v20191205/models.py
--rw-r--r--   0 root         (0) root         (0)    10029 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ssl/v20191205/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ssl/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iecp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iecp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iecp/v20210914/
--rw-r--r--   0 root         (0) root         (0)    94049 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iecp/v20210914/iecp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iecp/v20210914/__init__.py
--rw-r--r--   0 root         (0) root         (0)   489786 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iecp/v20210914/models.py
--rw-r--r--   0 root         (0) root         (0)     2001 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iecp/v20210914/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ccc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ccc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ccc/v20200210/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ccc/v20200210/__init__.py
--rw-r--r--   0 root         (0) root         (0)   246207 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ccc/v20200210/models.py
--rw-r--r--   0 root         (0) root         (0)     4155 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ccc/v20200210/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    38339 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ccc/v20200210/ccc_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcss/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcss/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcss/v20201101/
--rw-r--r--   0 root         (0) root         (0)   320238 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcss/v20201101/tcss_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcss/v20201101/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1759454 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcss/v20201101/models.py
--rw-r--r--   0 root         (0) root         (0)     3916 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcss/v20201101/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ump/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ump/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ump/v20200918/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ump/v20200918/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89302 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ump/v20200918/models.py
--rw-r--r--   0 root         (0) root         (0)     1536 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ump/v20200918/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    16091 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ump/v20200918/ump_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cam/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cam/v20190116/
--rw-r--r--   0 root         (0) root         (0)    79374 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cam/v20190116/cam_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cam/v20190116/__init__.py
--rw-r--r--   0 root         (0) root         (0)   297923 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cam/v20190116/models.py
--rw-r--r--   0 root         (0) root         (0)    11646 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cam/v20190116/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cam/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yinsuda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yinsuda/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yinsuda/v20220527/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yinsuda/v20220527/__init__.py
--rw-r--r--   0 root         (0) root         (0)   119498 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yinsuda/v20220527/models.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yinsuda/v20220527/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    16968 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yinsuda/v20220527/yinsuda_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dcdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dcdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dcdb/v20180411/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dcdb/v20180411/__init__.py
--rw-r--r--   0 root         (0) root         (0)   396114 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dcdb/v20180411/models.py
--rw-r--r--   0 root         (0) root         (0)    13937 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dcdb/v20180411/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    72486 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dcdb/v20180411/dcdb_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/autoscaling/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/autoscaling/v20180419/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/autoscaling/v20180419/__init__.py
--rw-r--r--   0 root         (0) root         (0)   428851 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/autoscaling/v20180419/models.py
--rw-r--r--   0 root         (0) root         (0)    21614 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/autoscaling/v20180419/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    69676 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/autoscaling/v20180419/autoscaling_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/autoscaling/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cat/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cat/v20180409/
--rw-r--r--   0 root         (0) root         (0)    10939 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cat/v20180409/cat_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cat/v20180409/__init__.py
--rw-r--r--   0 root         (0) root         (0)    67446 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cat/v20180409/models.py
--rw-r--r--   0 root         (0) root         (0)     2879 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cat/v20180409/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tag/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tag/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tag/v20180813/
--rw-r--r--   0 root         (0) root         (0)    28668 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tag/v20180813/tag_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tag/v20180813/__init__.py
--rw-r--r--   0 root         (0) root         (0)   125754 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tag/v20180813/models.py
--rw-r--r--   0 root         (0) root         (0)     5579 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tag/v20180813/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/car/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/car/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/car/v20220110/
--rw-r--r--   0 root         (0) root         (0)     6298 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/car/v20220110/car_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/car/v20220110/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16317 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/car/v20220110/models.py
--rw-r--r--   0 root         (0) root         (0)     1965 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/car/v20220110/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mrs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mrs/v20200910/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mrs/v20200910/__init__.py
--rw-r--r--   0 root         (0) root         (0)   702042 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mrs/v20200910/models.py
--rw-r--r--   0 root         (0) root         (0)     3011 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mrs/v20200910/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     5798 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mrs/v20200910/mrs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mrs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rp/v20200224/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rp/v20200224/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16086 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rp/v20200224/models.py
--rw-r--r--   0 root         (0) root         (0)     2431 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rp/v20200224/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     2224 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rp/v20200224/rp_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ic/v20190307/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ic/v20190307/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46716 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ic/v20190307/models.py
--rw-r--r--   0 root         (0) root         (0)     8987 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ic/v20190307/ic_client.py
--rw-r--r--   0 root         (0) root         (0)      983 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ic/v20190307/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tem/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tem/v20201221/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tem/v20201221/__init__.py
--rw-r--r--   0 root         (0) root         (0)   117434 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tem/v20201221/models.py
--rw-r--r--   0 root         (0) root         (0)    15824 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tem/v20201221/tem_client.py
--rw-r--r--   0 root         (0) root         (0)      747 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tem/v20201221/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tem/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tem/v20210701/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tem/v20210701/__init__.py
--rw-r--r--   0 root         (0) root         (0)   379345 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tem/v20210701/models.py
--rw-r--r--   0 root         (0) root         (0)    46073 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tem/v20210701/tem_client.py
--rw-r--r--   0 root         (0) root         (0)    17128 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tem/v20210701/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gs/v20191118/
--rw-r--r--   0 root         (0) root         (0)     7857 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gs/v20191118/gs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gs/v20191118/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25245 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gs/v20191118/models.py
--rw-r--r--   0 root         (0) root         (0)     2065 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gs/v20191118/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trp/v20210515/
--rw-r--r--   0 root         (0) root         (0)    46794 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trp/v20210515/trp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trp/v20210515/__init__.py
--rw-r--r--   0 root         (0) root         (0)   253223 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trp/v20210515/models.py
--rw-r--r--   0 root         (0) root         (0)     1083 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trp/v20210515/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/goosefs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/goosefs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/goosefs/v20220519/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/goosefs/v20220519/__init__.py
--rw-r--r--   0 root         (0) root         (0)    74135 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/goosefs/v20220519/models.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/goosefs/v20220519/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    19861 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/goosefs/v20220519/goosefs_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bmvpc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bmvpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bmvpc/v20180625/
--rw-r--r--   0 root         (0) root         (0)    58956 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bmvpc/v20180625/bmvpc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bmvpc/v20180625/__init__.py
--rw-r--r--   0 root         (0) root         (0)   250943 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bmvpc/v20180625/models.py
--rw-r--r--   0 root         (0) root         (0)     3260 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bmvpc/v20180625/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dbbrain/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dbbrain/v20210527/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dbbrain/v20210527/__init__.py
--rw-r--r--   0 root         (0) root         (0)   379052 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dbbrain/v20210527/models.py
--rw-r--r--   0 root         (0) root         (0)     2143 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dbbrain/v20210527/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    60108 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dbbrain/v20210527/dbbrain_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dbbrain/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dbbrain/v20191016/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dbbrain/v20191016/__init__.py
--rw-r--r--   0 root         (0) root         (0)   183920 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dbbrain/v20191016/models.py
--rw-r--r--   0 root         (0) root         (0)     1652 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dbbrain/v20191016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    27767 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dbbrain/v20191016/dbbrain_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cpdp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cpdp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cpdp/v20190820/
--rw-r--r--   0 root         (0) root         (0)   210468 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cpdp/v20190820/cpdp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cpdp/v20190820/__init__.py
--rw-r--r--   0 root         (0) root         (0)  2033620 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cpdp/v20190820/models.py
--rw-r--r--   0 root         (0) root         (0)    19183 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cpdp/v20190820/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/domain/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/domain/v20180808/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/domain/v20180808/__init__.py
--rw-r--r--   0 root         (0) root         (0)   122825 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/domain/v20180808/models.py
--rw-r--r--   0 root         (0) root         (0)     9007 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/domain/v20180808/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    26115 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/domain/v20180808/domain_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/domain/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mariadb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mariadb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mariadb/v20170312/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mariadb/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   355011 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mariadb/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)    72060 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mariadb/v20170312/mariadb_client.py
--rw-r--r--   0 root         (0) root         (0)    14932 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mariadb/v20170312/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tmt/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tmt/v20180321/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tmt/v20180321/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46724 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tmt/v20180321/models.py
--rw-r--r--   0 root         (0) root         (0)     9450 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tmt/v20180321/tmt_client.py
--rw-r--r--   0 root         (0) root         (0)     3623 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tmt/v20180321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tmt/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotexplorer/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotexplorer/v20190423/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotexplorer/v20190423/__init__.py
--rw-r--r--   0 root         (0) root         (0)   368411 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotexplorer/v20190423/models.py
--rw-r--r--   0 root         (0) root         (0)    20522 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotexplorer/v20190423/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    84131 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotexplorer/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ses/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ses/v20201002/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ses/v20201002/__init__.py
--rw-r--r--   0 root         (0) root         (0)   115869 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ses/v20201002/models.py
--rw-r--r--   0 root         (0) root         (0)    11535 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ses/v20201002/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    29406 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ses/v20201002/ses_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ses/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/casb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/casb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/casb/v20200507/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/casb/v20200507/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5624 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/casb/v20200507/models.py
--rw-r--r--   0 root         (0) root         (0)      944 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/casb/v20200507/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     2216 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/casb/v20200507/casb_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ticm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ticm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ticm/v20181127/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ticm/v20181127/__init__.py
--rw-r--r--   0 root         (0) root         (0)    80377 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ticm/v20181127/models.py
--rw-r--r--   0 root         (0) root         (0)     1329 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ticm/v20181127/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     4025 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ticm/v20181127/ticm_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cbs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cbs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cbs/v20170312/
--rw-r--r--   0 root         (0) root         (0)    51017 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cbs/v20170312/cbs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cbs/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   227628 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cbs/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)     7755 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cbs/v20170312/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tic/v20201117/
--rw-r--r--   0 root         (0) root         (0)    14464 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tic/v20201117/tic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tic/v20201117/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43811 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tic/v20201117/models.py
--rw-r--r--   0 root         (0) root         (0)     1450 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tic/v20201117/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tat/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tat/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tat/v20201028/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tat/v20201028/__init__.py
--rw-r--r--   0 root         (0) root         (0)   159502 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tat/v20201028/models.py
--rw-r--r--   0 root         (0) root         (0)     8096 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tat/v20201028/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    27476 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tat/v20201028/tat_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/advisor/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/advisor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/advisor/v20200721/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/advisor/v20200721/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17632 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/advisor/v20200721/models.py
--rw-r--r--   0 root         (0) root         (0)     2848 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/advisor/v20200721/advisor_client.py
--rw-r--r--   0 root         (0) root         (0)     1113 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/advisor/v20200721/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/facefusion/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/facefusion/v20181201/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/facefusion/v20181201/__init__.py
--rw-r--r--   0 root         (0) root         (0)    39231 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/facefusion/v20181201/models.py
--rw-r--r--   0 root         (0) root         (0)     6831 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/facefusion/v20181201/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     5813 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/facefusion/v20181201/facefusion_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/facefusion/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/facefusion/v20220927/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/facefusion/v20220927/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25364 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/facefusion/v20220927/models.py
--rw-r--r--   0 root         (0) root         (0)     5623 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/facefusion/v20220927/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     3394 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/facefusion/v20220927/facefusion_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcr/v20190924/
--rw-r--r--   0 root         (0) root         (0)   105482 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcr/v20190924/tcr_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcr/v20190924/__init__.py
--rw-r--r--   0 root         (0) root         (0)   448531 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcr/v20190924/models.py
--rw-r--r--   0 root         (0) root         (0)     8622 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcr/v20190924/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbaas/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbaas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbaas/v20180416/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbaas/v20180416/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112703 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbaas/v20180416/models.py
--rw-r--r--   0 root         (0) root         (0)    10664 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbaas/v20180416/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    20172 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbaas/v20180416/tbaas_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cvm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cvm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cvm/v20170312/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cvm/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   626747 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cvm/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)    45566 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cvm/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   120056 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cvm/v20170312/cvm_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/anicloud/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/anicloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/anicloud/v20220923/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/anicloud/v20220923/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19109 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/anicloud/v20220923/models.py
--rw-r--r--   0 root         (0) root         (0)      709 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/anicloud/v20220923/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     3623 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/anicloud/v20220923/anicloud_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/hasim/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/hasim/v20210716/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/hasim/v20210716/__init__.py
--rw-r--r--   0 root         (0) root         (0)   123000 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/hasim/v20210716/models.py
--rw-r--r--   0 root         (0) root         (0)     1393 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/hasim/v20210716/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    19722 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/hasim/v20210716/hasim_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/hasim/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cme/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cme/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cme/v20191029/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cme/v20191029/__init__.py
--rw-r--r--   0 root         (0) root         (0)   445345 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cme/v20191029/models.py
--rw-r--r--   0 root         (0) root         (0)    55451 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cme/v20191029/cme_client.py
--rw-r--r--   0 root         (0) root         (0)     8415 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cme/v20191029/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/clb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/clb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/clb/v20180317/
--rw-r--r--   0 root         (0) root         (0)    95722 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/clb/v20180317/clb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/clb/v20180317/__init__.py
--rw-r--r--   0 root         (0) root         (0)   531752 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/clb/v20180317/models.py
--rw-r--r--   0 root         (0) root         (0)     3269 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/clb/v20180317/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tse/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tse/v20201207/
--rw-r--r--   0 root         (0) root         (0)    49343 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tse/v20201207/tse_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tse/v20201207/__init__.py
--rw-r--r--   0 root         (0) root         (0)   350755 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tse/v20201207/models.py
--rw-r--r--   0 root         (0) root         (0)     5600 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tse/v20201207/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ie/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ie/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ie/v20200304/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ie/v20200304/__init__.py
--rw-r--r--   0 root         (0) root         (0)   233379 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ie/v20200304/models.py
--rw-r--r--   0 root         (0) root         (0)     4235 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ie/v20200304/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    11025 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ie/v20200304/ie_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/smop/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/smop/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/smop/v20201203/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/smop/v20201203/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11024 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/smop/v20201203/models.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/smop/v20201203/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     1866 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/smop/v20201203/smop_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdb/v20170320/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdb/v20170320/__init__.py
--rw-r--r--   0 root         (0) root         (0)   803999 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdb/v20170320/models.py
--rw-r--r--   0 root         (0) root         (0)    20514 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdb/v20170320/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   148592 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdb/v20170320/cdb_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/redis/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/redis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/redis/v20180412/
--rw-r--r--   0 root         (0) root         (0)    87874 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/redis/v20180412/redis_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/redis/v20180412/__init__.py
--rw-r--r--   0 root         (0) root         (0)   467296 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/redis/v20180412/models.py
--rw-r--r--   0 root         (0) root         (0)    12423 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/redis/v20180412/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tms/v20201229/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tms/v20201229/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28735 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tms/v20201229/models.py
--rw-r--r--   0 root         (0) root         (0)     1723 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tms/v20201229/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     3551 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tms/v20201229/tms_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tms/v20200713/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tms/v20200713/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40163 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tms/v20200713/models.py
--rw-r--r--   0 root         (0) root         (0)     3027 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tms/v20200713/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     4674 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tms/v20200713/tms_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/region/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/region/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/region/v20220627/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/region/v20220627/__init__.py
--rw-r--r--   0 root         (0) root         (0)    18296 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/region/v20220627/models.py
--rw-r--r--   0 root         (0) root         (0)     3756 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/region/v20220627/region_client.py
--rw-r--r--   0 root         (0) root         (0)      866 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/region/v20220627/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tke/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tke/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tke/v20180525/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tke/v20180525/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1119118 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tke/v20180525/models.py
--rw-r--r--   0 root         (0) root         (0)    19924 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tke/v20180525/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   199717 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tke/v20180525/tke_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cr/v20180321/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cr/v20180321/__init__.py
--rw-r--r--   0 root         (0) root         (0)   136120 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cr/v20180321/models.py
--rw-r--r--   0 root         (0) root         (0)    26131 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cr/v20180321/cr_client.py
--rw-r--r--   0 root         (0) root         (0)     4158 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cr/v20180321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/btoe/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/btoe/v20210514/
--rw-r--r--   0 root         (0) root         (0)    14662 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/btoe/v20210514/btoe_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/btoe/v20210514/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43354 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/btoe/v20210514/models.py
--rw-r--r--   0 root         (0) root         (0)     3235 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/btoe/v20210514/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/btoe/v20210303/
--rw-r--r--   0 root         (0) root         (0)    14684 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/btoe/v20210303/btoe_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/btoe/v20210303/__init__.py
--rw-r--r--   0 root         (0) root         (0)    47728 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/btoe/v20210303/models.py
--rw-r--r--   0 root         (0) root         (0)     3211 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/btoe/v20210303/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/btoe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dsgc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dsgc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dsgc/v20190723/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dsgc/v20190723/__init__.py
--rw-r--r--   0 root         (0) root         (0)   797805 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dsgc/v20190723/models.py
--rw-r--r--   0 root         (0) root         (0)   145268 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dsgc/v20190723/dsgc_client.py
--rw-r--r--   0 root         (0) root         (0)     1791 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dsgc/v20190723/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cynosdb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cynosdb/v20190107/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cynosdb/v20190107/__init__.py
--rw-r--r--   0 root         (0) root         (0)   712502 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cynosdb/v20190107/models.py
--rw-r--r--   0 root         (0) root         (0)    11512 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cynosdb/v20190107/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   120044 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cynosdb/v20190107/cynosdb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cynosdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/af/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/af/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/af/v20200226/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/af/v20200226/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54195 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/af/v20200226/models.py
--rw-r--r--   0 root         (0) root         (0)     4164 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/af/v20200226/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     4131 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/af/v20200226/af_client.py
--rw-r--r--   0 root         (0) root         (0)      630 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ft/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ft/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ft/v20200304/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ft/v20200304/__init__.py
--rw-r--r--   0 root         (0) root         (0)    29493 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ft/v20200304/models.py
--rw-r--r--   0 root         (0) root         (0)     5649 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ft/v20200304/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     6827 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ft/v20200304/ft_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/acp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/acp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/acp/v20220105/
--rw-r--r--   0 root         (0) root         (0)     8408 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/acp/v20220105/acp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/acp/v20220105/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53725 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/acp/v20220105/models.py
--rw-r--r--   0 root         (0) root         (0)      832 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/acp/v20220105/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sms/v20210111/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sms/v20210111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   104906 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sms/v20210111/models.py
--rw-r--r--   0 root         (0) root         (0)    19344 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sms/v20210111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    28405 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sms/v20210111/sms_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sms/v20190711/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sms/v20190711/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93677 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sms/v20190711/models.py
--rw-r--r--   0 root         (0) root         (0)    18522 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sms/v20190711/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    26631 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sms/v20190711/sms_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lcic/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lcic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lcic/v20220817/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lcic/v20220817/__init__.py
--rw-r--r--   0 root         (0) root         (0)   248641 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lcic/v20220817/models.py
--rw-r--r--   0 root         (0) root         (0)     4699 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lcic/v20220817/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    50664 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lcic/v20220817/lcic_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/fmu/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/fmu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/fmu/v20191213/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/fmu/v20191213/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45807 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/fmu/v20191213/models.py
--rw-r--r--   0 root         (0) root         (0)     6925 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/fmu/v20191213/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    10618 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/fmu/v20191213/fmu_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/teo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/teo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/teo/v20220106/
--rw-r--r--   0 root         (0) root         (0)     5399 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/teo/v20220106/teo_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/teo/v20220106/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38737 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/teo/v20220106/models.py
--rw-r--r--   0 root         (0) root         (0)     2192 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/teo/v20220106/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/teo/v20220901/
--rw-r--r--   0 root         (0) root         (0)    61993 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/teo/v20220901/teo_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/teo/v20220901/__init__.py
--rw-r--r--   0 root         (0) root         (0)   625407 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/teo/v20220901/models.py
--rw-r--r--   0 root         (0) root         (0)    28390 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/teo/v20220901/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ciam/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ciam/v20220331/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ciam/v20220331/__init__.py
--rw-r--r--   0 root         (0) root         (0)   139059 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ciam/v20220331/models.py
--rw-r--r--   0 root         (0) root         (0)     8558 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ciam/v20220331/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    20721 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ciam/v20220331/ciam_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ciam/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/monitor/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/monitor/v20180724/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/monitor/v20180724/__init__.py
--rw-r--r--   0 root         (0) root         (0)   871012 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/monitor/v20180724/models.py
--rw-r--r--   0 root         (0) root         (0)    10348 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/monitor/v20180724/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   145293 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/monitor/v20180724/monitor_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/monitor/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ecc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ecc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ecc/v20181213/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ecc/v20181213/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40735 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ecc/v20181213/models.py
--rw-r--r--   0 root         (0) root         (0)     3889 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ecc/v20181213/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     4497 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ecc/v20181213/ecc_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bizlive/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bizlive/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bizlive/v20190313/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bizlive/v20190313/__init__.py
--rw-r--r--   0 root         (0) root         (0)    19225 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bizlive/v20190313/models.py
--rw-r--r--   0 root         (0) root         (0)     2083 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bizlive/v20190313/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     6329 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bizlive/v20190313/bizlive_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/irp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/irp/v20220324/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/irp/v20220324/__init__.py
--rw-r--r--   0 root         (0) root         (0)    54088 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/irp/v20220324/models.py
--rw-r--r--   0 root         (0) root         (0)      961 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/irp/v20220324/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     4389 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/irp/v20220324/irp_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/irp/v20220805/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/irp/v20220805/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81404 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/irp/v20220805/models.py
--rw-r--r--   0 root         (0) root         (0)     1018 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/irp/v20220805/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     7365 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/irp/v20220805/irp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/irp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/faceid/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/faceid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/faceid/v20180301/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/faceid/v20180301/__init__.py
--rw-r--r--   0 root         (0) root         (0)   222483 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/faceid/v20180301/models.py
--rw-r--r--   0 root         (0) root         (0)     9370 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/faceid/v20180301/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    34162 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/faceid/v20180301/faceid_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tics/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tics/v20181115/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tics/v20181115/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28834 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tics/v20181115/models.py
--rw-r--r--   0 root         (0) root         (0)     1037 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tics/v20181115/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     4917 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tics/v20181115/tics_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/nlp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/nlp/v20190408/
--rw-r--r--   0 root         (0) root         (0)    13476 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/nlp/v20190408/nlp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/nlp/v20190408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    52142 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/nlp/v20190408/models.py
--rw-r--r--   0 root         (0) root         (0)     4521 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/nlp/v20190408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/nlp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/waf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/waf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/waf/v20180125/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/waf/v20180125/__init__.py
--rw-r--r--   0 root         (0) root         (0)   618583 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/waf/v20180125/models.py
--rw-r--r--   0 root         (0) root         (0)     5741 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/waf/v20180125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   112925 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/waf/v20180125/waf_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gaap/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gaap/v20180529/
--rw-r--r--   0 root         (0) root         (0)   101614 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gaap/v20180529/gaap_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gaap/v20180529/__init__.py
--rw-r--r--   0 root         (0) root         (0)   516159 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gaap/v20180529/models.py
--rw-r--r--   0 root         (0) root         (0)    11791 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gaap/v20180529/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gaap/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tan/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tan/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tan/v20220420/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tan/v20220420/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2967 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tan/v20220420/models.py
--rw-r--r--   0 root         (0) root         (0)     2281 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tan/v20220420/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     1896 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tan/v20220420/tan_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vod/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vod/v20180717/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vod/v20180717/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1876797 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vod/v20180717/models.py
--rw-r--r--   0 root         (0) root         (0)    25211 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vod/v20180717/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   185303 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vod/v20180717/vod_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ecm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ecm/v20190719/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ecm/v20190719/__init__.py
--rw-r--r--   0 root         (0) root         (0)   733514 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ecm/v20190719/models.py
--rw-r--r--   0 root         (0) root         (0)    23498 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ecm/v20190719/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   136183 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ecm/v20190719/ecm_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ecm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lowcode/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lowcode/v20210108/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lowcode/v20210108/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26092 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lowcode/v20210108/models.py
--rw-r--r--   0 root         (0) root         (0)     1929 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lowcode/v20210108/lowcode_client.py
--rw-r--r--   0 root         (0) root         (0)      948 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lowcode/v20210108/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lowcode/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ms/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ms/v20180408/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ms/v20180408/__init__.py
--rw-r--r--   0 root         (0) root         (0)   180152 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ms/v20180408/models.py
--rw-r--r--   0 root         (0) root         (0)     5911 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ms/v20180408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    23945 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ms/v20180408/ms_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vrs/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vrs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vrs/v20200824/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vrs/v20200824/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28696 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vrs/v20200824/models.py
--rw-r--r--   0 root         (0) root         (0)     2156 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vrs/v20200824/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     7458 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vrs/v20200824/vrs_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bri/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bri/v20190328/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bri/v20190328/__init__.py
--rw-r--r--   0 root         (0) root         (0)    11308 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bri/v20190328/models.py
--rw-r--r--   0 root         (0) root         (0)     2407 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bri/v20190328/bri_client.py
--rw-r--r--   0 root         (0) root         (0)     2171 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bri/v20190328/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bri/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cis/v20180408/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cis/v20180408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    38589 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cis/v20180408/models.py
--rw-r--r--   0 root         (0) root         (0)      760 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cis/v20180408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     7726 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cis/v20180408/cis_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gse/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gse/v20191112/
--rw-r--r--   0 root         (0) root         (0)    89371 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gse/v20191112/gse_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gse/v20191112/__init__.py
--rw-r--r--   0 root         (0) root         (0)   387109 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gse/v20191112/models.py
--rw-r--r--   0 root         (0) root         (0)     2578 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gse/v20191112/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tourism/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tourism/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tourism/v20230215/
--rw-r--r--   0 root         (0) root         (0)     1959 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tourism/v20230215/tourism_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tourism/v20230215/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8749 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tourism/v20230215/models.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tourism/v20230215/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/apigateway/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/apigateway/v20180808/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/apigateway/v20180808/__init__.py
--rw-r--r--   0 root         (0) root         (0)   648978 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/apigateway/v20180808/models.py
--rw-r--r--   0 root         (0) root         (0)    22090 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/apigateway/v20180808/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    95541 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/apigateway/v20180808/apigateway_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/apigateway/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iai/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iai/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iai/v20180301/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iai/v20180301/__init__.py
--rw-r--r--   0 root         (0) root         (0)   236091 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iai/v20180301/models.py
--rw-r--r--   0 root         (0) root         (0)    11999 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iai/v20180301/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    46290 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iai/v20180301/iai_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iai/v20200303/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iai/v20200303/__init__.py
--rw-r--r--   0 root         (0) root         (0)   251563 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iai/v20200303/models.py
--rw-r--r--   0 root         (0) root         (0)    12105 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iai/v20200303/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    49515 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iai/v20200303/iai_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/es/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/es/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/es/v20180416/
--rw-r--r--   0 root         (0) root         (0)    36126 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/es/v20180416/es_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/es/v20180416/__init__.py
--rw-r--r--   0 root         (0) root         (0)   298586 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/es/v20180416/models.py
--rw-r--r--   0 root         (0) root         (0)    21311 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/es/v20180416/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eb/v20210416/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eb/v20210416/__init__.py
--rw-r--r--   0 root         (0) root         (0)   152636 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eb/v20210416/models.py
--rw-r--r--   0 root         (0) root         (0)    14675 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eb/v20210416/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    28438 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eb/v20210416/eb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bda/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bda/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bda/v20200324/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bda/v20200324/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112857 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bda/v20200324/models.py
--rw-r--r--   0 root         (0) root         (0)     8576 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bda/v20200324/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    20667 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bda/v20200324/bda_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dasb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dasb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dasb/v20191018/
--rw-r--r--   0 root         (0) root         (0)    48361 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dasb/v20191018/dasb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dasb/v20191018/__init__.py
--rw-r--r--   0 root         (0) root         (0)   279575 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dasb/v20191018/models.py
--rw-r--r--   0 root         (0) root         (0)     2500 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dasb/v20191018/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ecdn/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ecdn/v20191012/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ecdn/v20191012/__init__.py
--rw-r--r--   0 root         (0) root         (0)   120841 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ecdn/v20191012/models.py
--rw-r--r--   0 root         (0) root         (0)     9228 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ecdn/v20191012/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    20324 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ecdn/v20191012/ecdn_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ecdn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/postgres/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/postgres/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/postgres/v20170312/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/postgres/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   475358 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/postgres/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)    21166 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/postgres/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    91035 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/postgres/v20170312/postgres_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/youmall/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/youmall/v20180228/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/youmall/v20180228/__init__.py
--rw-r--r--   0 root         (0) root         (0)   184858 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/youmall/v20180228/models.py
--rw-r--r--   0 root         (0) root         (0)     2828 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/youmall/v20180228/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    31517 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/youmall/v20180228/youmall_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/youmall/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dts/v20180330/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dts/v20180330/__init__.py
--rw-r--r--   0 root         (0) root         (0)   124284 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dts/v20180330/models.py
--rw-r--r--   0 root         (0) root         (0)     5619 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dts/v20180330/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    24853 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dts/v20180330/dts_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dts/v20211206/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dts/v20211206/__init__.py
--rw-r--r--   0 root         (0) root         (0)   353467 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dts/v20211206/models.py
--rw-r--r--   0 root         (0) root         (0)     6952 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dts/v20211206/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    49338 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dts/v20211206/dts_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/common/
--rw-r--r--   0 root         (0) root         (0)    21860 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/common/abstract_client.py
--rw-r--r--   0 root         (0) root         (0)     1568 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/common/sign.py
--rw-r--r--   0 root         (0) root         (0)     2335 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/common/abstract_model.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/common/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/common/exception/
--rw-r--r--   0 root         (0) root         (0)      735 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/common/exception/__init__.py
--rw-r--r--   0 root         (0) root         (0)      760 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
--rw-r--r--   0 root         (0) root         (0)     1958 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/common/common_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/common/http/
--rw-r--r--   0 root         (0) root         (0)     4456 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/common/http/request.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/common/http/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/common/profile/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/common/profile/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1893 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/common/profile/http_profile.py
--rw-r--r--   0 root         (0) root         (0)     4534 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/common/profile/client_profile.py
--rw-r--r--   0 root         (0) root         (0)     4301 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/common/circuit_breaker.py
--rw-r--r--   0 root         (0) root         (0)    15945 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/common/credential.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ba/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ba/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ba/v20200720/
--rw-r--r--   0 root         (0) root         (0)     3804 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ba/v20200720/ba_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ba/v20200720/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7466 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ba/v20200720/models.py
--rw-r--r--   0 root         (0) root         (0)     1047 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ba/v20200720/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tia/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tia/v20180226/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tia/v20180226/__init__.py
--rw-r--r--   0 root         (0) root         (0)    49879 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tia/v20180226/models.py
--rw-r--r--   0 root         (0) root         (0)     2747 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tia/v20180226/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    10682 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tia/v20180226/tia_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tia/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/taf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/taf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/taf/v20200210/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/taf/v20200210/__init__.py
--rw-r--r--   0 root         (0) root         (0)    25951 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/taf/v20200210/models.py
--rw-r--r--   0 root         (0) root         (0)     4808 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/taf/v20200210/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     3826 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/taf/v20200210/taf_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ame/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ame/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ame/v20190916/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ame/v20190916/__init__.py
--rw-r--r--   0 root         (0) root         (0)   193152 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ame/v20190916/models.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ame/v20190916/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    29579 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ame/v20190916/ame_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcbr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcbr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcbr/v20220217/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcbr/v20220217/__init__.py
--rw-r--r--   0 root         (0) root         (0)    88962 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcbr/v20220217/models.py
--rw-r--r--   0 root         (0) root         (0)     1182 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcbr/v20220217/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    10074 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcbr/v20220217/tcbr_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/csxg/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/csxg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/csxg/v20230303/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/csxg/v20230303/__init__.py
--rw-r--r--   0 root         (0) root         (0)     4254 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/csxg/v20230303/models.py
--rw-r--r--   0 root         (0) root         (0)     5397 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/csxg/v20230303/csxg_client.py
--rw-r--r--   0 root         (0) root         (0)      769 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/csxg/v20230303/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/smpn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/smpn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/smpn/v20190822/
--rw-r--r--   0 root         (0) root         (0)     5314 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/smpn/v20190822/smpn_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/smpn/v20190822/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24181 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/smpn/v20190822/models.py
--rw-r--r--   0 root         (0) root         (0)     1008 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/smpn/v20190822/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cii/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cii/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cii/v20210408/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cii/v20210408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    87370 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cii/v20210408/models.py
--rw-r--r--   0 root         (0) root         (0)    13689 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cii/v20210408/cii_client.py
--rw-r--r--   0 root         (0) root         (0)     1358 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cii/v20210408/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cii/v20201210/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cii/v20201210/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16873 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cii/v20201210/models.py
--rw-r--r--   0 root         (0) root         (0)     3891 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cii/v20201210/cii_client.py
--rw-r--r--   0 root         (0) root         (0)     1065 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cii/v20201210/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cds/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cds/v20180420/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cds/v20180420/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24914 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cds/v20180420/models.py
--rw-r--r--   0 root         (0) root         (0)     6824 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cds/v20180420/cds_client.py
--rw-r--r--   0 root         (0) root         (0)      966 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cds/v20180420/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cds/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/afc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/afc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/afc/v20200226/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/afc/v20200226/__init__.py
--rw-r--r--   0 root         (0) root         (0)    40384 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/afc/v20200226/models.py
--rw-r--r--   0 root         (0) root         (0)     3863 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/afc/v20200226/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     3940 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/afc/v20200226/afc_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/aai/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/aai/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/aai/v20180522/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/aai/v20180522/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20548 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/aai/v20180522/models.py
--rw-r--r--   0 root         (0) root         (0)     4705 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/aai/v20180522/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     5497 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/aai/v20180522/aai_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/csip/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/csip/v20221121/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/csip/v20221121/__init__.py
--rw-r--r--   0 root         (0) root         (0)   341879 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/csip/v20221121/models.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/csip/v20221121/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    28721 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/csip/v20221121/csip_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/csip/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dataintegration/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dataintegration/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dataintegration/v20220613/
--rw-r--r--   0 root         (0) root         (0)     1914 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dataintegration/v20220613/dataintegration_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dataintegration/v20220613/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3967 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dataintegration/v20220613/models.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dataintegration/v20220613/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/npp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/npp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/npp/v20190823/
--rw-r--r--   0 root         (0) root         (0)     7974 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/npp/v20190823/npp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/npp/v20190823/__init__.py
--rw-r--r--   0 root         (0) root         (0)    60419 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/npp/v20190823/models.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/npp/v20190823/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iss/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iss/v20230517/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iss/v20230517/__init__.py
--rw-r--r--   0 root         (0) root         (0)   436666 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iss/v20230517/models.py
--rw-r--r--   0 root         (0) root         (0)    18801 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iss/v20230517/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    75806 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iss/v20230517/iss_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iss/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/captcha/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/captcha/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/captcha/v20190722/
--rw-r--r--   0 root         (0) root         (0)    17853 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/captcha/v20190722/captcha_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/captcha/v20190722/__init__.py
--rw-r--r--   0 root         (0) root         (0)   117646 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/captcha/v20190722/models.py
--rw-r--r--   0 root         (0) root         (0)     1037 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/captcha/v20190722/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trdp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trdp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trdp/v20220726/
--rw-r--r--   0 root         (0) root         (0)     1872 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trdp/v20220726/trdp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trdp/v20220726/__init__.py
--rw-r--r--   0 root         (0) root         (0)    37532 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trdp/v20220726/models.py
--rw-r--r--   0 root         (0) root         (0)     1158 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trdp/v20220726/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/chdfs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/chdfs/v20190718/
--rw-r--r--   0 root         (0) root         (0)    28126 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/chdfs/v20190718/chdfs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/chdfs/v20190718/__init__.py
--rw-r--r--   0 root         (0) root         (0)    78138 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/chdfs/v20190718/models.py
--rw-r--r--   0 root         (0) root         (0)     3280 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/chdfs/v20190718/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/chdfs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/chdfs/v20201112/
--rw-r--r--   0 root         (0) root         (0)    27402 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/chdfs/v20201112/chdfs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/chdfs/v20201112/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92834 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/chdfs/v20201112/models.py
--rw-r--r--   0 root         (0) root         (0)     3600 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/chdfs/v20201112/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mmps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mmps/v20200710/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mmps/v20200710/__init__.py
--rw-r--r--   0 root         (0) root         (0)    83019 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mmps/v20200710/models.py
--rw-r--r--   0 root         (0) root         (0)      775 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mmps/v20200710/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    15527 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mmps/v20200710/mmps_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mmps/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/api/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/api/v20201106/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/api/v20201106/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17428 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/api/v20201106/models.py
--rw-r--r--   0 root         (0) root         (0)     3726 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/api/v20201106/api_client.py
--rw-r--r--   0 root         (0) root         (0)      866 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/api/v20201106/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/api/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/organization/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/organization/v20181225/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/organization/v20181225/__init__.py
--rw-r--r--   0 root         (0) root         (0)    46488 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/organization/v20181225/models.py
--rw-r--r--   0 root         (0) root         (0)    19700 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/organization/v20181225/organization_client.py
--rw-r--r--   0 root         (0) root         (0)     3243 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/organization/v20181225/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/organization/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/organization/v20210331/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/organization/v20210331/__init__.py
--rw-r--r--   0 root         (0) root         (0)   130314 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/organization/v20210331/models.py
--rw-r--r--   0 root         (0) root         (0)    30181 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/organization/v20210331/organization_client.py
--rw-r--r--   0 root         (0) root         (0)    12433 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/organization/v20210331/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tci/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tci/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tci/v20190318/
--rw-r--r--   0 root         (0) root         (0)    44187 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tci/v20190318/tci_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tci/v20190318/__init__.py
--rw-r--r--   0 root         (0) root         (0)   285108 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tci/v20190318/models.py
--rw-r--r--   0 root         (0) root         (0)     8913 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tci/v20190318/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ckafka/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ckafka/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ckafka/v20190819/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ckafka/v20190819/__init__.py
--rw-r--r--   0 root         (0) root         (0)   785875 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ckafka/v20190819/models.py
--rw-r--r--   0 root         (0) root         (0)     3315 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ckafka/v20190819/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    73707 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ckafka/v20190819/ckafka_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tds/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tds/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tds/v20220801/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tds/v20220801/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27293 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tds/v20220801/models.py
--rw-r--r--   0 root         (0) root         (0)     4548 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tds/v20220801/tds_client.py
--rw-r--r--   0 root         (0) root         (0)      772 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tds/v20220801/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dbdc/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dbdc/v20201029/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dbdc/v20201029/__init__.py
--rw-r--r--   0 root         (0) root         (0)    72272 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dbdc/v20201029/models.py
--rw-r--r--   0 root         (0) root         (0)     2111 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dbdc/v20201029/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     6439 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dbdc/v20201029/dbdc_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dbdc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudhsm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudhsm/v20191112/
--rw-r--r--   0 root         (0) root         (0)    13347 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudhsm/v20191112/cloudhsm_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudhsm/v20191112/__init__.py
--rw-r--r--   0 root         (0) root         (0)    81651 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudhsm/v20191112/models.py
--rw-r--r--   0 root         (0) root         (0)     1020 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudhsm/v20191112/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudhsm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tiems/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tiems/v20190416/
--rw-r--r--   0 root         (0) root         (0)    28234 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tiems/v20190416/tiems_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tiems/v20190416/__init__.py
--rw-r--r--   0 root         (0) root         (0)   151851 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tiems/v20190416/models.py
--rw-r--r--   0 root         (0) root         (0)     1108 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tiems/v20190416/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tiems/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bmeip/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bmeip/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bmeip/v20180625/
--rw-r--r--   0 root         (0) root         (0)    18032 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bmeip/v20180625/bmeip_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bmeip/v20180625/__init__.py
--rw-r--r--   0 root         (0) root         (0)    69899 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bmeip/v20180625/models.py
--rw-r--r--   0 root         (0) root         (0)      820 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bmeip/v20180625/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ssm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ssm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ssm/v20190923/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ssm/v20190923/__init__.py
--rw-r--r--   0 root         (0) root         (0)   100023 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ssm/v20190923/models.py
--rw-r--r--   0 root         (0) root         (0)     3474 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ssm/v20190923/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    24609 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ssm/v20190923/ssm_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cfs/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cfs/v20190719/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cfs/v20190719/__init__.py
--rw-r--r--   0 root         (0) root         (0)   195707 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cfs/v20190719/models.py
--rw-r--r--   0 root         (0) root         (0)    15890 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cfs/v20190719/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    40047 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cfs/v20190719/cfs_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cfs/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tsw/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tsw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tsw/v20200924/
--rw-r--r--   0 root         (0) root         (0)     1878 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tsw/v20200924/tsw_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tsw/v20200924/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5590 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tsw/v20200924/models.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tsw/v20200924/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tsw/v20210412/
--rw-r--r--   0 root         (0) root         (0)     3722 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tsw/v20210412/tsw_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tsw/v20210412/__init__.py
--rw-r--r--   0 root         (0) root         (0)     3911 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tsw/v20210412/models.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tsw/v20210412/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yunjing/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yunjing/v20180228/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yunjing/v20180228/__init__.py
--rw-r--r--   0 root         (0) root         (0)   379701 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yunjing/v20180228/models.py
--rw-r--r--   0 root         (0) root         (0)    94372 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yunjing/v20180228/yunjing_client.py
--rw-r--r--   0 root         (0) root         (0)     3960 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yunjing/v20180228/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yunjing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gpm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gpm/v20200820/
--rw-r--r--   0 root         (0) root         (0)    18269 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gpm/v20200820/gpm_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gpm/v20200820/__init__.py
--rw-r--r--   0 root         (0) root         (0)   100825 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gpm/v20200820/models.py
--rw-r--r--   0 root         (0) root         (0)     5641 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gpm/v20200820/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gpm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tdid/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tdid/v20210519/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tdid/v20210519/__init__.py
--rw-r--r--   0 root         (0) root         (0)    43358 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tdid/v20210519/models.py
--rw-r--r--   0 root         (0) root         (0)    12712 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tdid/v20210519/tdid_client.py
--rw-r--r--   0 root         (0) root         (0)     1775 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tdid/v20210519/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tdid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/apm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/apm/v20210622/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/apm/v20210622/__init__.py
--rw-r--r--   0 root         (0) root         (0)    85514 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/apm/v20210622/models.py
--rw-r--r--   0 root         (0) root         (0)     3646 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/apm/v20210622/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     9241 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/apm/v20210622/apm_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/apm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/solar/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/solar/v20181011/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/solar/v20181011/__init__.py
--rw-r--r--   0 root         (0) root         (0)    88391 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/solar/v20181011/models.py
--rw-r--r--   0 root         (0) root         (0)     1500 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/solar/v20181011/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    15882 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/solar/v20181011/solar_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/solar/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gme/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gme/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gme/v20180711/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gme/v20180711/__init__.py
--rw-r--r--   0 root         (0) root         (0)   159505 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gme/v20180711/models.py
--rw-r--r--   0 root         (0) root         (0)     4026 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gme/v20180711/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    34890 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/gme/v20180711/gme_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/icr/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/icr/v20211014/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/icr/v20211014/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26493 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/icr/v20211014/models.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/icr/v20211014/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     1914 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/icr/v20211014/icr_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/icr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rkp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rkp/v20191209/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rkp/v20191209/__init__.py
--rw-r--r--   0 root         (0) root         (0)    21607 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rkp/v20191209/models.py
--rw-r--r--   0 root         (0) root         (0)     3783 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rkp/v20191209/rkp_client.py
--rw-r--r--   0 root         (0) root         (0)     3080 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rkp/v20191209/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rkp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/hcm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/hcm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/hcm/v20181106/
--rw-r--r--   0 root         (0) root         (0)     1947 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/hcm/v20181106/hcm_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/hcm/v20181106/__init__.py
--rw-r--r--   0 root         (0) root         (0)    14772 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/hcm/v20181106/models.py
--rw-r--r--   0 root         (0) root         (0)     2630 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/hcm/v20181106/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mna/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mna/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mna/v20210119/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mna/v20210119/__init__.py
--rw-r--r--   0 root         (0) root         (0)    67068 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mna/v20210119/models.py
--rw-r--r--   0 root         (0) root         (0)     2902 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mna/v20210119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    12133 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mna/v20210119/mna_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdwpg/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdwpg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdwpg/v20201230/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdwpg/v20201230/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48854 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdwpg/v20201230/models.py
--rw-r--r--   0 root         (0) root         (0)      737 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdwpg/v20201230/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     6392 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdwpg/v20201230/cdwpg_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/v20201215/
--rw-r--r--   0 root         (0) root         (0)    72567 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/v20201215/iotvideo_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/v20201215/__init__.py
--rw-r--r--   0 root         (0) root         (0)   304127 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/v20201215/models.py
--rw-r--r--   0 root         (0) root         (0)     1977 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/v20201215/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/v20191126/
--rw-r--r--   0 root         (0) root         (0)    64723 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/v20191126/iotvideo_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/v20191126/__init__.py
--rw-r--r--   0 root         (0) root         (0)   229605 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/v20191126/models.py
--rw-r--r--   0 root         (0) root         (0)     3098 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/v20191126/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/v20211125/
--rw-r--r--   0 root         (0) root         (0)    91083 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/v20211125/iotvideo_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/v20211125/__init__.py
--rw-r--r--   0 root         (0) root         (0)   381639 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/v20211125/models.py
--rw-r--r--   0 root         (0) root         (0)     2198 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/v20211125/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mongodb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mongodb/v20180408/
--rw-r--r--   0 root         (0) root         (0)    13623 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mongodb/v20180408/mongodb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mongodb/v20180408/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76740 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mongodb/v20180408/models.py
--rw-r--r--   0 root         (0) root         (0)     3903 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mongodb/v20180408/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mongodb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mongodb/v20190725/
--rw-r--r--   0 root         (0) root         (0)    36587 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mongodb/v20190725/mongodb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mongodb/v20190725/__init__.py
--rw-r--r--   0 root         (0) root         (0)   234826 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mongodb/v20190725/models.py
--rw-r--r--   0 root         (0) root         (0)     7304 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mongodb/v20190725/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iot/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iot/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iot/v20180123/
--rw-r--r--   0 root         (0) root         (0)    40904 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iot/v20180123/iot_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iot/v20180123/__init__.py
--rw-r--r--   0 root         (0) root         (0)   171391 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iot/v20180123/models.py
--rw-r--r--   0 root         (0) root         (0)     6163 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iot/v20180123/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vm/v20201229/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vm/v20201229/__init__.py
--rw-r--r--   0 root         (0) root         (0)    95121 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vm/v20201229/models.py
--rw-r--r--   0 root         (0) root         (0)     9185 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vm/v20201229/vm_client.py
--rw-r--r--   0 root         (0) root         (0)     1967 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vm/v20201229/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vm/v20210922/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vm/v20210922/__init__.py
--rw-r--r--   0 root         (0) root         (0)    84771 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vm/v20210922/models.py
--rw-r--r--   0 root         (0) root         (0)     5305 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vm/v20210922/vm_client.py
--rw-r--r--   0 root         (0) root         (0)     1967 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vm/v20210922/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vm/v20200709/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vm/v20200709/__init__.py
--rw-r--r--   0 root         (0) root         (0)    76744 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vm/v20200709/models.py
--rw-r--r--   0 root         (0) root         (0)     5863 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vm/v20200709/vm_client.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vm/v20200709/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ams/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ams/v20201229/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ams/v20201229/__init__.py
--rw-r--r--   0 root         (0) root         (0)    93055 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ams/v20201229/models.py
--rw-r--r--   0 root         (0) root         (0)     3347 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ams/v20201229/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    10675 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ams/v20201229/ams_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ams/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ams/v20200608/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ams/v20200608/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89744 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ams/v20200608/models.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ams/v20200608/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     9160 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ams/v20200608/ams_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcm/v20210413/
--rw-r--r--   0 root         (0) root         (0)    11262 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcm/v20210413/tcm_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcm/v20210413/__init__.py
--rw-r--r--   0 root         (0) root         (0)   130072 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcm/v20210413/models.py
--rw-r--r--   0 root         (0) root         (0)     1334 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcm/v20210413/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tav/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tav/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tav/v20190118/
--rw-r--r--   0 root         (0) root         (0)     4395 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tav/v20190118/tav_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tav/v20190118/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12546 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tav/v20190118/models.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tav/v20190118/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sslpod/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sslpod/v20190605/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sslpod/v20190605/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41178 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sslpod/v20190605/models.py
--rw-r--r--   0 root         (0) root         (0)     2079 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sslpod/v20190605/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     9749 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sslpod/v20190605/sslpod_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sslpod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bmlb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bmlb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bmlb/v20180625/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bmlb/v20180625/__init__.py
--rw-r--r--   0 root         (0) root         (0)   327109 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bmlb/v20180625/models.py
--rw-r--r--   0 root         (0) root         (0)    47282 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bmlb/v20180625/bmlb_client.py
--rw-r--r--   0 root         (0) root         (0)      929 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bmlb/v20180625/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/wss/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/wss/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/wss/v20180426/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/wss/v20180426/__init__.py
--rw-r--r--   0 root         (0) root         (0)    24432 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/wss/v20180426/models.py
--rw-r--r--   0 root         (0) root         (0)     1239 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/wss/v20180426/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     3606 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/wss/v20180426/wss_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cfg/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cfg/v20210820/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cfg/v20210820/__init__.py
--rw-r--r--   0 root         (0) root         (0)   123448 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cfg/v20210820/models.py
--rw-r--r--   0 root         (0) root         (0)     1933 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cfg/v20210820/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     9735 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cfg/v20210820/cfg_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cfg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/aa/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/aa/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/aa/v20200224/
--rw-r--r--   0 root         (0) root         (0)     2184 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/aa/v20200224/aa_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/aa/v20200224/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17163 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/aa/v20200224/models.py
--rw-r--r--   0 root         (0) root         (0)     2430 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/aa/v20200224/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vpc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vpc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vpc/v20170312/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vpc/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1365413 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vpc/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)    45216 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vpc/v20170312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   342735 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/vpc/v20170312/vpc_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideoindustry/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideoindustry/v20201201/
--rw-r--r--   0 root         (0) root         (0)   100347 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideoindustry/v20201201/iotvideoindustry_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideoindustry/v20201201/__init__.py
--rw-r--r--   0 root         (0) root         (0)   369812 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideoindustry/v20201201/models.py
--rw-r--r--   0 root         (0) root         (0)     8583 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideoindustry/v20201201/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideoindustry/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mps/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mps/v20190612/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mps/v20190612/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1333652 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mps/v20190612/models.py
--rw-r--r--   0 root         (0) root         (0)    13604 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mps/v20190612/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   100285 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mps/v20190612/mps_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mps/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ape/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ape/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ape/v20200513/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ape/v20200513/__init__.py
--rw-r--r--   0 root         (0) root         (0)    42775 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ape/v20200513/models.py
--rw-r--r--   0 root         (0) root         (0)     1570 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ape/v20200513/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     8191 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ape/v20200513/ape_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcaplusdb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcaplusdb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcaplusdb/v20190823/
--rw-r--r--   0 root         (0) root         (0)    49200 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcaplusdb/v20190823/tcaplusdb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcaplusdb/v20190823/__init__.py
--rw-r--r--   0 root         (0) root         (0)   309127 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcaplusdb/v20190823/models.py
--rw-r--r--   0 root         (0) root         (0)     3614 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcaplusdb/v20190823/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dayu/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dayu/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dayu/v20180709/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dayu/v20180709/__init__.py
--rw-r--r--   0 root         (0) root         (0)   545180 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dayu/v20180709/models.py
--rw-r--r--   0 root         (0) root         (0)     1440 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dayu/v20180709/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   103066 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dayu/v20180709/dayu_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/weilingwith/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/weilingwith/v20230427/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/weilingwith/v20230427/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13098 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/weilingwith/v20230427/models.py
--rw-r--r--   0 root         (0) root         (0)     1405 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/weilingwith/v20230427/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     5703 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/weilingwith/v20230427/weilingwith_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/weilingwith/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/scf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/scf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/scf/v20180416/
--rw-r--r--   0 root         (0) root         (0)    44580 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/scf/v20180416/scf_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/scf/v20180416/__init__.py
--rw-r--r--   0 root         (0) root         (0)   322466 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/scf/v20180416/models.py
--rw-r--r--   0 root         (0) root         (0)    32699 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/scf/v20180416/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lp/v20200224/
--rw-r--r--   0 root         (0) root         (0)     2098 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lp/v20200224/lp_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lp/v20200224/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17582 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lp/v20200224/models.py
--rw-r--r--   0 root         (0) root         (0)     2430 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lp/v20200224/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cim/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cim/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cim/v20190318/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cim/v20190318/__init__.py
--rw-r--r--   0 root         (0) root         (0)     1779 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cim/v20190318/models.py
--rw-r--r--   0 root         (0) root         (0)      827 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cim/v20190318/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     1894 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cim/v20190318/cim_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lighthouse/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lighthouse/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lighthouse/v20200324/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lighthouse/v20200324/__init__.py
--rw-r--r--   0 root         (0) root         (0)   449067 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lighthouse/v20200324/models.py
--rw-r--r--   0 root         (0) root         (0)    28428 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lighthouse/v20200324/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   117975 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/lighthouse/v20200324/lighthouse_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/keewidb/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/keewidb/v20220308/
--rw-r--r--   0 root         (0) root         (0)    37435 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/keewidb/v20220308/keewidb_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/keewidb/v20220308/__init__.py
--rw-r--r--   0 root         (0) root         (0)   219041 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/keewidb/v20220308/models.py
--rw-r--r--   0 root         (0) root         (0)     5660 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/keewidb/v20220308/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/keewidb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tdcpg/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tdcpg/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tdcpg/v20211118/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tdcpg/v20211118/__init__.py
--rw-r--r--   0 root         (0) root         (0)   102873 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tdcpg/v20211118/models.py
--rw-r--r--   0 root         (0) root         (0)     6249 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tdcpg/v20211118/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    24877 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tdcpg/v20211118/tdcpg_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdwch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdwch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdwch/v20200915/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdwch/v20200915/__init__.py
--rw-r--r--   0 root         (0) root         (0)   158461 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdwch/v20200915/models.py
--rw-r--r--   0 root         (0) root         (0)      703 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdwch/v20200915/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    24533 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdwch/v20200915/cdwch_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudstudio/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudstudio/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudstudio/v20210524/
--rw-r--r--   0 root         (0) root         (0)    21897 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudstudio/v20210524/cloudstudio_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudstudio/v20210524/__init__.py
--rw-r--r--   0 root         (0) root         (0)   112109 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudstudio/v20210524/models.py
--rw-r--r--   0 root         (0) root         (0)      828 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudstudio/v20210524/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudstudio/v20230508/
--rw-r--r--   0 root         (0) root         (0)     8992 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudstudio/v20230508/cloudstudio_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudstudio/v20230508/__init__.py
--rw-r--r--   0 root         (0) root         (0)    33829 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudstudio/v20230508/models.py
--rw-r--r--   0 root         (0) root         (0)      979 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudstudio/v20230508/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/msp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/msp/v20180319/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/msp/v20180319/__init__.py
--rw-r--r--   0 root         (0) root         (0)    30960 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/msp/v20180319/models.py
--rw-r--r--   0 root         (0) root         (0)     7386 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/msp/v20180319/msp_client.py
--rw-r--r--   0 root         (0) root         (0)      791 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/msp/v20180319/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/msp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/memcached/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/memcached/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/memcached/v20190318/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/memcached/v20190318/__init__.py
--rw-r--r--   0 root         (0) root         (0)    16280 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/memcached/v20190318/models.py
--rw-r--r--   0 root         (0) root         (0)     1378 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/memcached/v20190318/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     1906 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/memcached/v20190318/memcached_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bpaas/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bpaas/v20181217/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bpaas/v20181217/__init__.py
--rw-r--r--   0 root         (0) root         (0)    27503 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bpaas/v20181217/models.py
--rw-r--r--   0 root         (0) root         (0)     1297 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bpaas/v20181217/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     2832 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bpaas/v20181217/bpaas_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bpaas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbm/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbm/v20180129/
--rw-r--r--   0 root         (0) root         (0)    10459 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbm/v20180129/tbm_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbm/v20180129/__init__.py
--rw-r--r--   0 root         (0) root         (0)    53389 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbm/v20180129/models.py
--rw-r--r--   0 root         (0) root         (0)     1235 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbm/v20180129/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trro/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trro/v20220325/
--rw-r--r--   0 root         (0) root         (0)    21373 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trro/v20220325/trro_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trro/v20220325/__init__.py
--rw-r--r--   0 root         (0) root         (0)   103053 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trro/v20220325/models.py
--rw-r--r--   0 root         (0) root         (0)     1069 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trro/v20220325/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trro/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/smh/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/smh/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/smh/v20210712/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/smh/v20210712/__init__.py
--rw-r--r--   0 root         (0) root         (0)    55893 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/smh/v20210712/models.py
--rw-r--r--   0 root         (0) root         (0)     9912 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/smh/v20210712/smh_client.py
--rw-r--r--   0 root         (0) root         (0)     3851 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/smh/v20210712/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/kms/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/kms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/kms/v20190118/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/kms/v20190118/__init__.py
--rw-r--r--   0 root         (0) root         (0)   156339 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/kms/v20190118/models.py
--rw-r--r--   0 root         (0) root         (0)     5342 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/kms/v20190118/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    51055 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/kms/v20190118/kms_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/habo/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/habo/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/habo/v20181203/
--rw-r--r--   0 root         (0) root         (0)     2800 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/habo/v20181203/habo_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/habo/v20181203/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6216 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/habo/v20181203/models.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/habo/v20181203/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/omics/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/omics/v20221128/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/omics/v20221128/__init__.py
--rw-r--r--   0 root         (0) root         (0)    89719 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/omics/v20221128/models.py
--rw-r--r--   0 root         (0) root         (0)     4545 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/omics/v20221128/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    11346 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/omics/v20221128/omics_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/omics/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tkgdq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tkgdq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tkgdq/v20190411/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tkgdq/v20190411/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13153 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tkgdq/v20190411/models.py
--rw-r--r--   0 root         (0) root         (0)     1685 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tkgdq/v20190411/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     4193 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tkgdq/v20190411/tkgdq_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eiam/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eiam/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eiam/v20210420/
--rw-r--r--   0 root         (0) root         (0)    39100 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eiam/v20210420/eiam_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eiam/v20210420/__init__.py
--rw-r--r--   0 root         (0) root         (0)   218794 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eiam/v20210420/models.py
--rw-r--r--   0 root         (0) root         (0)     9938 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eiam/v20210420/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rce/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rce/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rce/v20201103/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rce/v20201103/__init__.py
--rw-r--r--   0 root         (0) root         (0)    48344 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rce/v20201103/models.py
--rw-r--r--   0 root         (0) root         (0)     4151 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rce/v20201103/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     4013 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rce/v20201103/rce_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/privatedns/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/privatedns/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/privatedns/v20201028/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/privatedns/v20201028/__init__.py
--rw-r--r--   0 root         (0) root         (0)    98914 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/privatedns/v20201028/models.py
--rw-r--r--   0 root         (0) root         (0)    23057 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/privatedns/v20201028/privatedns_client.py
--rw-r--r--   0 root         (0) root         (0)     7631 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/privatedns/v20201028/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tsf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tsf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tsf/v20180326/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tsf/v20180326/__init__.py
--rw-r--r--   0 root         (0) root         (0)  1295816 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tsf/v20180326/models.py
--rw-r--r--   0 root         (0) root         (0)    50530 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tsf/v20180326/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   197191 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tsf/v20180326/tsf_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iottid/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iottid/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iottid/v20190411/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iottid/v20190411/__init__.py
--rw-r--r--   0 root         (0) root         (0)    23421 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iottid/v20190411/models.py
--rw-r--r--   0 root         (0) root         (0)     1707 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iottid/v20190411/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     9166 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iottid/v20190411/iottid_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dc/v20180410/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dc/v20180410/__init__.py
--rw-r--r--   0 root         (0) root         (0)   148313 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dc/v20180410/models.py
--rw-r--r--   0 root         (0) root         (0)     2973 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dc/v20180410/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    21006 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dc/v20180410/dc_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/wav/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/wav/v20210129/
--rw-r--r--   0 root         (0) root         (0)    26012 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/wav/v20210129/wav_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/wav/v20210129/__init__.py
--rw-r--r--   0 root         (0) root         (0)   229425 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/wav/v20210129/models.py
--rw-r--r--   0 root         (0) root         (0)     1771 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/wav/v20210129/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/wav/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudaudit/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudaudit/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudaudit/v20190319/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudaudit/v20190319/__init__.py
--rw-r--r--   0 root         (0) root         (0)    90257 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudaudit/v20190319/models.py
--rw-r--r--   0 root         (0) root         (0)    18578 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudaudit/v20190319/cloudaudit_client.py
--rw-r--r--   0 root         (0) root         (0)     6753 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cloudaudit/v20190319/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rum/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rum/v20210622/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rum/v20210622/__init__.py
--rw-r--r--   0 root         (0) root         (0)   295365 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rum/v20210622/models.py
--rw-r--r--   0 root         (0) root         (0)    60037 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rum/v20210622/rum_client.py
--rw-r--r--   0 root         (0) root         (0)     2530 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rum/v20210622/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/rum/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tdmq/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tdmq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tdmq/v20200217/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tdmq/v20200217/__init__.py
--rw-r--r--   0 root         (0) root         (0)   641891 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tdmq/v20200217/models.py
--rw-r--r--   0 root         (0) root         (0)    10126 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tdmq/v20200217/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   101215 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tdmq/v20200217/tdmq_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dnspod/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dnspod/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dnspod/v20210323/
--rw-r--r--   0 root         (0) root         (0)    61922 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dnspod/v20210323/dnspod_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dnspod/v20210323/__init__.py
--rw-r--r--   0 root         (0) root         (0)   352399 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dnspod/v20210323/models.py
--rw-r--r--   0 root         (0) root         (0)    24241 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dnspod/v20210323/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eis/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eis/v20200715/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eis/v20200715/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17929 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eis/v20200715/models.py
--rw-r--r--   0 root         (0) root         (0)     3727 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eis/v20200715/eis_client.py
--rw-r--r--   0 root         (0) root         (0)     1197 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eis/v20200715/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eis/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eis/v20210601/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eis/v20210601/__init__.py
--rw-r--r--   0 root         (0) root         (0)    41837 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eis/v20210601/models.py
--rw-r--r--   0 root         (0) root         (0)     5866 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eis/v20210601/eis_client.py
--rw-r--r--   0 root         (0) root         (0)     3329 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/eis/v20210601/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbp/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbp/v20190627/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbp/v20190627/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20731 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbp/v20190627/models.py
--rw-r--r--   0 root         (0) root         (0)     1189 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbp/v20190627/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     2690 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbp/v20190627/tbp_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbp/v20190311/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbp/v20190311/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26651 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbp/v20190311/models.py
--rw-r--r--   0 root         (0) root         (0)     1554 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbp/v20190311/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     4436 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tbp/v20190311/tbp_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/live/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/live/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/live/v20180801/
--rw-r--r--   0 root         (0) root         (0)   157870 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/live/v20180801/live_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/live/v20180801/__init__.py
--rw-r--r--   0 root         (0) root         (0)   769438 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/live/v20180801/models.py
--rw-r--r--   0 root         (0) root         (0)    20164 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/live/v20180801/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mall/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mall/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mall/v20230518/
--rw-r--r--   0 root         (0) root         (0)     1941 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mall/v20230518/mall_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mall/v20230518/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8749 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mall/v20230518/models.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mall/v20230518/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cmq/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cmq/v20190304/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cmq/v20190304/__init__.py
--rw-r--r--   0 root         (0) root         (0)    98147 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cmq/v20190304/models.py
--rw-r--r--   0 root         (0) root         (0)    15822 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cmq/v20190304/cmq_client.py
--rw-r--r--   0 root         (0) root         (0)     1312 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cmq/v20190304/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cmq/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcb/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcb/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcb/v20180608/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcb/v20180608/__init__.py
--rw-r--r--   0 root         (0) root         (0)   553921 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcb/v20180608/models.py
--rw-r--r--   0 root         (0) root         (0)     4156 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcb/v20180608/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    84257 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tcb/v20180608/tcb_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cws/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cws/v20180312/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cws/v20180312/__init__.py
--rw-r--r--   0 root         (0) root         (0)    92049 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cws/v20180312/models.py
--rw-r--r--   0 root         (0) root         (0)     1228 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cws/v20180312/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    18593 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cws/v20180312/cws_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cws/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/billing/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/billing/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/billing/v20180709/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/billing/v20180709/__init__.py
--rw-r--r--   0 root         (0) root         (0)   342394 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/billing/v20180709/models.py
--rw-r--r--   0 root         (0) root         (0)     2984 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/billing/v20180709/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    28340 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/billing/v20180709/billing_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tchd/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tchd/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tchd/v20230306/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tchd/v20230306/__init__.py
--rw-r--r--   0 root         (0) root         (0)     7653 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tchd/v20230306/models.py
--rw-r--r--   0 root         (0) root         (0)      833 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tchd/v20230306/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     1986 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tchd/v20230306/tchd_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dtf/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dtf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dtf/v20200506/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dtf/v20200506/__init__.py
--rw-r--r--   0 root         (0) root         (0)    13921 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dtf/v20200506/models.py
--rw-r--r--   0 root         (0) root         (0)      849 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dtf/v20200506/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     1887 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dtf/v20200506/dtf_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cfw/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cfw/v20190904/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cfw/v20190904/__init__.py
--rw-r--r--   0 root         (0) root         (0)   529438 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cfw/v20190904/models.py
--rw-r--r--   0 root         (0) root         (0)     1836 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cfw/v20190904/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    96688 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cfw/v20190904/cfw_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cfw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/emr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/emr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/emr/v20190103/
--rw-r--r--   0 root         (0) root         (0)    31934 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/emr/v20190103/emr_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/emr/v20190103/__init__.py
--rw-r--r--   0 root         (0) root         (0)   467608 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/emr/v20190103/models.py
--rw-r--r--   0 root         (0) root         (0)    14648 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/emr/v20190103/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trocket/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trocket/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trocket/v20230308/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trocket/v20230308/__init__.py
--rw-r--r--   0 root         (0) root         (0)    96204 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trocket/v20230308/models.py
--rw-r--r--   0 root         (0) root         (0)    18157 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trocket/v20230308/trocket_client.py
--rw-r--r--   0 root         (0) root         (0)     1567 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trocket/v20230308/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sqlserver/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sqlserver/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sqlserver/v20180328/
--rw-r--r--   0 root         (0) root         (0)   111899 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sqlserver/v20180328/sqlserver_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sqlserver/v20180328/__init__.py
--rw-r--r--   0 root         (0) root         (0)   586240 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sqlserver/v20180328/models.py
--rw-r--r--   0 root         (0) root         (0)     9722 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sqlserver/v20180328/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mgobe/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mgobe/v20201014/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mgobe/v20201014/__init__.py
--rw-r--r--   0 root         (0) root         (0)    32095 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mgobe/v20201014/models.py
--rw-r--r--   0 root         (0) root         (0)    34111 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mgobe/v20201014/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     8272 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mgobe/v20201014/mgobe_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mgobe/v20190929/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mgobe/v20190929/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2464 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mgobe/v20190929/models.py
--rw-r--r--   0 root         (0) root         (0)    34005 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mgobe/v20190929/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     1859 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mgobe/v20190929/mgobe_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/mgobe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/essbasic/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/essbasic/v20201222/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/essbasic/v20201222/__init__.py
--rw-r--r--   0 root         (0) root         (0)   270905 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/essbasic/v20201222/models.py
--rw-r--r--   0 root         (0) root         (0)     5392 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/essbasic/v20201222/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    54057 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/essbasic/v20201222/essbasic_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/essbasic/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/essbasic/v20210526/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/essbasic/v20210526/__init__.py
--rw-r--r--   0 root         (0) root         (0)   505009 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/essbasic/v20210526/models.py
--rw-r--r--   0 root         (0) root         (0)    17658 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/essbasic/v20210526/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    78004 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/essbasic/v20210526/essbasic_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cms/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cms/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cms/v20190321/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cms/v20190321/__init__.py
--rw-r--r--   0 root         (0) root         (0)    97349 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cms/v20190321/models.py
--rw-r--r--   0 root         (0) root         (0)     4152 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cms/v20190321/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     6597 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cms/v20190321/cms_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cwp/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cwp/v20180228/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cwp/v20180228/__init__.py
--rw-r--r--   0 root         (0) root         (0)   478685 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cwp/v20180228/cwp_client.py
--rw-r--r--   0 root         (0) root         (0)  2448233 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cwp/v20180228/models.py
--rw-r--r--   0 root         (0) root         (0)     4402 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cwp/v20180228/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cwp/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tione/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tione/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tione/v20191022/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tione/v20191022/__init__.py
--rw-r--r--   0 root         (0) root         (0)   144266 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tione/v20191022/models.py
--rw-r--r--   0 root         (0) root         (0)     4465 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tione/v20191022/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    22102 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tione/v20191022/tione_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tione/v20211111/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tione/v20211111/__init__.py
--rw-r--r--   0 root         (0) root         (0)   649190 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tione/v20211111/models.py
--rw-r--r--   0 root         (0) root         (0)    15712 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tione/v20211111/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    64588 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tione/v20211111/tione_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdn/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdn/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdn/v20180606/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdn/v20180606/__init__.py
--rw-r--r--   0 root         (0) root         (0)   854187 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdn/v20180606/models.py
--rw-r--r--   0 root         (0) root         (0)    82459 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdn/v20180606/cdn_client.py
--rw-r--r--   0 root         (0) root         (0)    22415 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cdn/v20180606/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ivld/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ivld/v20210903/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ivld/v20210903/__init__.py
--rw-r--r--   0 root         (0) root         (0)   158264 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ivld/v20210903/models.py
--rw-r--r--   0 root         (0) root         (0)     9364 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ivld/v20210903/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    29555 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ivld/v20210903/ivld_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ivld/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/drm/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/drm/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/drm/v20181115/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/drm/v20181115/__init__.py
--rw-r--r--   0 root         (0) root         (0)    45281 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/drm/v20181115/models.py
--rw-r--r--   0 root         (0) root         (0)     1093 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/drm/v20181115/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     9944 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/drm/v20181115/drm_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tiia/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tiia/v20190529/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tiia/v20190529/__init__.py
--rw-r--r--   0 root         (0) root         (0)   146178 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tiia/v20190529/models.py
--rw-r--r--   0 root         (0) root         (0)    32719 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tiia/v20190529/tiia_client.py
--rw-r--r--   0 root         (0) root         (0)     7539 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tiia/v20190529/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tiia/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ocr/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ocr/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ocr/v20181119/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ocr/v20181119/__init__.py
--rw-r--r--   0 root         (0) root         (0)   780644 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ocr/v20181119/models.py
--rw-r--r--   0 root         (0) root         (0)     5927 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ocr/v20181119/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   110470 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/ocr/v20181119/ocr_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trtc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trtc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trtc/v20190722/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trtc/v20190722/__init__.py
--rw-r--r--   0 root         (0) root         (0)   306532 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trtc/v20190722/models.py
--rw-r--r--   0 root         (0) root         (0)     9778 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trtc/v20190722/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    72465 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/trtc/v20190722/trtc_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotcloud/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotcloud/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotcloud/v20210408/
--rw-r--r--   0 root         (0) root         (0)    67173 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotcloud/v20210408/iotcloud_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotcloud/v20210408/__init__.py
--rw-r--r--   0 root         (0) root         (0)   280299 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotcloud/v20210408/models.py
--rw-r--r--   0 root         (0) root         (0)    12818 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotcloud/v20210408/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotcloud/v20180614/
--rw-r--r--   0 root         (0) root         (0)    64562 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotcloud/v20180614/iotcloud_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotcloud/v20180614/__init__.py
--rw-r--r--   0 root         (0) root         (0)   281180 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotcloud/v20180614/models.py
--rw-r--r--   0 root         (0) root         (0)    12668 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iotcloud/v20180614/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/soe/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/soe/v20180724/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/soe/v20180724/__init__.py
--rw-r--r--   0 root         (0) root         (0)    67959 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/soe/v20180724/models.py
--rw-r--r--   0 root         (0) root         (0)     5919 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/soe/v20180724/soe_client.py
--rw-r--r--   0 root         (0) root         (0)    14811 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/soe/v20180724/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/soe/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/aiart/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/aiart/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/aiart/v20221229/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/aiart/v20221229/__init__.py
--rw-r--r--   0 root         (0) root         (0)    17082 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/aiart/v20221229/models.py
--rw-r--r--   0 root         (0) root         (0)     3806 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/aiart/v20221229/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     3676 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/aiart/v20221229/aiart_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yunsou/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yunsou/v20191115/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yunsou/v20191115/__init__.py
--rw-r--r--   0 root         (0) root         (0)    22913 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yunsou/v20191115/models.py
--rw-r--r--   0 root         (0) root         (0)     1301 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yunsou/v20191115/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     2741 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yunsou/v20191115/yunsou_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yunsou/v20180504/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yunsou/v20180504/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12751 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yunsou/v20180504/models.py
--rw-r--r--   0 root         (0) root         (0)      652 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yunsou/v20180504/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     2735 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yunsou/v20180504/yunsou_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/yunsou/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/apcas/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/apcas/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/apcas/v20201127/
--rw-r--r--   0 root         (0) root         (0)     7214 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/apcas/v20201127/apcas_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/apcas/v20201127/__init__.py
--rw-r--r--   0 root         (0) root         (0)    35285 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/apcas/v20201127/models.py
--rw-r--r--   0 root         (0) root         (0)     1430 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/apcas/v20201127/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bi/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bi/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bi/v20220105/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bi/v20220105/__init__.py
--rw-r--r--   0 root         (0) root         (0)   163392 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bi/v20220105/models.py
--rw-r--r--   0 root         (0) root         (0)    19358 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bi/v20220105/bi_client.py
--rw-r--r--   0 root         (0) root         (0)     2007 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/bi/v20220105/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tiw/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tiw/v20190919/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tiw/v20190919/__init__.py
--rw-r--r--   0 root         (0) root         (0)   284696 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tiw/v20190919/models.py
--rw-r--r--   0 root         (0) root         (0)    61603 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tiw/v20190919/tiw_client.py
--rw-r--r--   0 root         (0) root         (0)     6092 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tiw/v20190919/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/tiw/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dlc/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dlc/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dlc/v20210125/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dlc/v20210125/__init__.py
--rw-r--r--   0 root         (0) root         (0)   726055 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dlc/v20210125/models.py
--rw-r--r--   0 root         (0) root         (0)    17887 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dlc/v20210125/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)   106851 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/dlc/v20210125/dlc_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iir/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iir/v20200417/
--rw-r--r--   0 root         (0) root         (0)     2952 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iir/v20200417/iir_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iir/v20200417/__init__.py
--rw-r--r--   0 root         (0) root         (0)    12048 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iir/v20200417/models.py
--rw-r--r--   0 root         (0) root         (0)     1737 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iir/v20200417/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/iir/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cls/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cls/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cls/v20201016/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cls/v20201016/__init__.py
--rw-r--r--   0 root         (0) root         (0)   543823 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cls/v20201016/models.py
--rw-r--r--   0 root         (0) root         (0)     9633 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cls/v20201016/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)    87362 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/cls/v20201016/cls_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sts/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sts/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sts/v20180813/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sts/v20180813/__init__.py
--rw-r--r--   0 root         (0) root         (0)    28050 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sts/v20180813/models.py
--rw-r--r--   0 root         (0) root         (0)     3086 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sts/v20180813/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     7324 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/sts/v20180813/sts_client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/batch/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/batch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/batch/v20170312/
--rw-r--r--   0 root         (0) root         (0)    31661 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/batch/v20170312/batch_client.py
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/batch/v20170312/__init__.py
--rw-r--r--   0 root         (0) root         (0)   301995 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/batch/v20170312/models.py
--rw-r--r--   0 root         (0) root         (0)     8635 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/batch/v20170312/errorcodes.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/pds/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/pds/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/pds/v20210701/
--rw-r--r--   0 root         (0) root         (0)        0 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/pds/v20210701/__init__.py
--rw-r--r--   0 root         (0) root         (0)     8332 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/pds/v20210701/models.py
--rw-r--r--   0 root         (0) root         (0)     1395 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/pds/v20210701/errorcodes.py
--rw-r--r--   0 root         (0) root         (0)     2837 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/tencentcloud/pds/v20210701/pds_client.py
--rw-r--r--   0 root         (0) root         (0)       65 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1475 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      661 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/README.rst
--rw-r--r--   0 root         (0) root         (0)       67 2023-10-13 00:18:45.000000 tencentcloud-sdk-python-3.0.998/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1186 2023-10-13 00:07:49.000000 tencentcloud-sdk-python-3.0.998/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/
+-rw-r--r--   0 root         (0) root         (0)      683 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/tdsql.py
+-rw-r--r--   0 root         (0) root         (0)      687 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/scaling.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/live.py
+-rw-r--r--   0 root         (0) root         (0)      787 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/ccr.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/redis.py
+-rw-r--r--   0 root         (0) root         (0)      785 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/tmt.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/bill.py
+-rw-r--r--   0 root         (0) root         (0)      811 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/dc.py
+-rw-r--r--   0 root         (0) root         (0)      685 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/yunsou.py
+-rw-r--r--   0 root         (0) root         (0)      780 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/sts.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/bmeip.py
+-rw-r--r--   0 root         (0) root         (0)      776 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/emr.py
+-rw-r--r--   0 root         (0) root         (0)      685 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/wenzhi.py
+-rw-r--r--   0 root         (0) root         (0)      677 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/bm.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/trade.py
+-rw-r--r--   0 root         (0) root         (0)      679 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/cbs.py
+-rw-r--r--   0 root         (0) root         (0)      717 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/scf.py
+-rw-r--r--   0 root         (0) root         (0)      679 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/dfw.py
+-rw-r--r--   0 root         (0) root         (0)      680 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/sec.py
+-rw-r--r--   0 root         (0) root         (0)      679 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/cns.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/image.py
+-rw-r--r--   0 root         (0) root         (0)      679 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/eip.py
+-rw-r--r--   0 root         (0) root         (0)      679 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/ccs.py
+-rw-r--r--   0 root         (0) root         (0)      691 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/feecenter.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/cmem.py
+-rw-r--r--   0 root         (0) root         (0)      802 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/athena.py
+-rw-r--r--   0 root         (0) root         (0)      693 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/cloudaudit.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/bmvpc.py
+-rw-r--r--   0 root         (0) root         (0)      679 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/vpc.py
+-rw-r--r--   0 root         (0) root         (0)      793 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/tbaas.py
+-rw-r--r--   0 root         (0) root         (0)      679 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/vod.py
+-rw-r--r--   0 root         (0) root         (0)      693 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/apigateway.py
+-rw-r--r--   0 root         (0) root         (0)      677 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/lb.py
+-rw-r--r--   0 root         (0) root         (0)      685 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/market.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/bgpip.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/partners.py
+-rw-r--r--   0 root         (0) root         (0)      687 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/monitor.py
+-rw-r--r--   0 root         (0) root         (0)      681 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/bmlb.py
+-rw-r--r--   0 root         (0) root         (0)      689 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/snapshot.py
+-rw-r--r--   0 root         (0) root         (0)     1346 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/cdn.py
+-rw-r--r--   0 root         (0) root         (0)      687 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/account.py
+-rw-r--r--   0 root         (0) root         (0)      683 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/batch.py
+-rw-r--r--   0 root         (0) root         (0)     5487 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/base.py
+-rw-r--r--   0 root         (0) root         (0)      679 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/cdb.py
+-rw-r--r--   0 root         (0) root         (0)      679 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/modules/cvm.py
+-rw-r--r--   0 root         (0) root         (0)       23 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/common/
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/common/api_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/common/sign.py
+-rw-r--r--   0 root         (0) root         (0)     5077 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/common/request.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/common/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6751 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/QcloudApi/qcloudapi.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud_sdk_python.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       23 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud_sdk_python.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud_sdk_python.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)     1475 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud_sdk_python.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)    54224 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud_sdk_python.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud_sdk_python.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)    11351 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/LICENSE
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/asr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/asr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/asr/v20190614/
+-rw-r--r--   0 root         (0) root         (0)    30288 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/asr/v20190614/asr_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/asr/v20190614/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   119460 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/asr/v20190614/models.py
+-rw-r--r--   0 root         (0) root         (0)     7627 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/asr/v20190614/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/oceanus/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/oceanus/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/oceanus/v20190422/
+-rw-r--r--   0 root         (0) root         (0)    25417 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/oceanus/v20190422/oceanus_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/oceanus/v20190422/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   247703 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/oceanus/v20190422/models.py
+-rw-r--r--   0 root         (0) root         (0)     9664 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/oceanus/v20190422/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bma/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bma/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bma/v20221115/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bma/v20221115/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    66446 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bma/v20221115/models.py
+-rw-r--r--   0 root         (0) root         (0)     3348 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bma/v20221115/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    10571 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bma/v20221115/bma_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bma/v20210624/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bma/v20210624/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   146139 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bma/v20210624/models.py
+-rw-r--r--   0 root         (0) root         (0)     1829 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bma/v20210624/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    25903 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bma/v20210624/bma_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bm/v20180423/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bm/v20180423/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   274077 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bm/v20180423/models.py
+-rw-r--r--   0 root         (0) root         (0)    50710 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bm/v20180423/bm_client.py
+-rw-r--r--   0 root         (0) root         (0)     1896 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bm/v20180423/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/v20230321/
+-rw-r--r--   0 root         (0) root         (0)    17767 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/v20230321/thpc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/v20230321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   167264 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/v20230321/models.py
+-rw-r--r--   0 root         (0) root         (0)     4560 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/v20230321/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/v20220401/
+-rw-r--r--   0 root         (0) root         (0)    16797 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/v20220401/thpc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/v20220401/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   142732 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/v20220401/models.py
+-rw-r--r--   0 root         (0) root         (0)     4733 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/v20220401/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/v20211109/
+-rw-r--r--   0 root         (0) root         (0)     4628 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/v20211109/thpc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/v20211109/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    63030 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/v20211109/models.py
+-rw-r--r--   0 root         (0) root         (0)     2035 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/v20211109/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/market/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/market/v20191010/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/market/v20191010/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7313 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/market/v20191010/models.py
+-rw-r--r--   0 root         (0) root         (0)      941 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/market/v20191010/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     2922 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/market/v20191010/market_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/market/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/antiddos/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/antiddos/v20200309/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/antiddos/v20200309/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   507080 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/antiddos/v20200309/models.py
+-rw-r--r--   0 root         (0) root         (0)    89530 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/antiddos/v20200309/antiddos_client.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/antiddos/v20200309/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/antiddos/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vms/v20200902/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vms/v20200902/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10184 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vms/v20200902/models.py
+-rw-r--r--   0 root         (0) root         (0)     2741 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vms/v20200902/vms_client.py
+-rw-r--r--   0 root         (0) root         (0)     4848 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vms/v20200902/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdc/v20201214/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdc/v20201214/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   144909 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdc/v20201214/models.py
+-rw-r--r--   0 root         (0) root         (0)     2972 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdc/v20201214/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    19439 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdc/v20201214/cdc_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/asw/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/asw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/asw/v20200722/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/asw/v20200722/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    44296 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/asw/v20200722/models.py
+-rw-r--r--   0 root         (0) root         (0)      950 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/asw/v20200722/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     9134 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/asw/v20200722/asw_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/pts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/pts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/pts/v20210728/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/pts/v20210728/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   310158 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/pts/v20210728/models.py
+-rw-r--r--   0 root         (0) root         (0)     2118 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/pts/v20210728/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    39385 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/pts/v20210728/pts_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/wedata/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/wedata/v20210820/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/wedata/v20210820/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  2024031 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/wedata/v20210820/models.py
+-rw-r--r--   0 root         (0) root         (0)     3640 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/wedata/v20210820/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   284129 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/wedata/v20210820/wedata_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/wedata/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/partners/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/partners/v20180321/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/partners/v20180321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   109523 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/partners/v20180321/models.py
+-rw-r--r--   0 root         (0) root         (0)      885 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/partners/v20180321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    19410 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/partners/v20180321/partners_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/partners/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bsca/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bsca/v20210811/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bsca/v20210811/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49093 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bsca/v20210811/models.py
+-rw-r--r--   0 root         (0) root         (0)     5975 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bsca/v20210811/bsca_client.py
+-rw-r--r--   0 root         (0) root         (0)     1057 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bsca/v20210811/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bsca/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ds/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ds/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ds/v20180523/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ds/v20180523/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49948 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ds/v20180523/models.py
+-rw-r--r--   0 root         (0) root         (0)    10034 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ds/v20180523/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    13758 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ds/v20180523/ds_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcex/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcex/v20200727/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcex/v20200727/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8678 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcex/v20200727/models.py
+-rw-r--r--   0 root         (0) root         (0)     1712 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcex/v20200727/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     3127 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcex/v20200727/tcex_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcex/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ess/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ess/v20201111/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ess/v20201111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   602461 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ess/v20201111/models.py
+-rw-r--r--   0 root         (0) root         (0)   116342 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ess/v20201111/ess_client.py
+-rw-r--r--   0 root         (0) root         (0)    24792 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ess/v20201111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ess/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ims/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ims/v20201229/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ims/v20201229/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    65090 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ims/v20201229/models.py
+-rw-r--r--   0 root         (0) root         (0)     3639 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ims/v20201229/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     8527 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ims/v20201229/ims_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ims/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ims/v20200713/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ims/v20200713/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47064 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ims/v20200713/models.py
+-rw-r--r--   0 root         (0) root         (0)     3528 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ims/v20200713/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     3228 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ims/v20200713/ims_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tts/v20190823/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tts/v20190823/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25951 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tts/v20190823/models.py
+-rw-r--r--   0 root         (0) root         (0)     5608 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tts/v20190823/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     5886 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tts/v20190823/tts_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mvj/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mvj/v20190926/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mvj/v20190926/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6014 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mvj/v20190926/models.py
+-rw-r--r--   0 root         (0) root         (0)     1105 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mvj/v20190926/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     2103 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mvj/v20190926/mvj_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mvj/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ssa/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ssa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ssa/v20180608/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ssa/v20180608/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   292973 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ssa/v20180608/models.py
+-rw-r--r--   0 root         (0) root         (0)     2265 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ssa/v20180608/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    24532 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ssa/v20180608/ssa_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ssl/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ssl/v20191205/
+-rw-r--r--   0 root         (0) root         (0)    55603 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ssl/v20191205/ssl_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ssl/v20191205/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   433897 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ssl/v20191205/models.py
+-rw-r--r--   0 root         (0) root         (0)    10029 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ssl/v20191205/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ssl/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iecp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iecp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iecp/v20210914/
+-rw-r--r--   0 root         (0) root         (0)    94049 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iecp/v20210914/iecp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iecp/v20210914/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   489786 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iecp/v20210914/models.py
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iecp/v20210914/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ccc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ccc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ccc/v20200210/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ccc/v20200210/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   246183 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ccc/v20200210/models.py
+-rw-r--r--   0 root         (0) root         (0)     4155 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ccc/v20200210/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    38339 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ccc/v20200210/ccc_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcss/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcss/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcss/v20201101/
+-rw-r--r--   0 root         (0) root         (0)   320238 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcss/v20201101/tcss_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcss/v20201101/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1759454 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcss/v20201101/models.py
+-rw-r--r--   0 root         (0) root         (0)     3916 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcss/v20201101/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ump/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ump/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ump/v20200918/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ump/v20200918/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89302 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ump/v20200918/models.py
+-rw-r--r--   0 root         (0) root         (0)     1536 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ump/v20200918/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    16091 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ump/v20200918/ump_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cam/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cam/v20190116/
+-rw-r--r--   0 root         (0) root         (0)    79374 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cam/v20190116/cam_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cam/v20190116/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   297923 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cam/v20190116/models.py
+-rw-r--r--   0 root         (0) root         (0)    11646 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cam/v20190116/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cam/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yinsuda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yinsuda/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yinsuda/v20220527/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yinsuda/v20220527/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   119498 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yinsuda/v20220527/models.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yinsuda/v20220527/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    16968 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yinsuda/v20220527/yinsuda_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dcdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dcdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dcdb/v20180411/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dcdb/v20180411/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   396114 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dcdb/v20180411/models.py
+-rw-r--r--   0 root         (0) root         (0)    13937 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dcdb/v20180411/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    72486 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dcdb/v20180411/dcdb_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/autoscaling/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/autoscaling/v20180419/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/autoscaling/v20180419/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   428851 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/autoscaling/v20180419/models.py
+-rw-r--r--   0 root         (0) root         (0)    21614 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/autoscaling/v20180419/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    69676 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/autoscaling/v20180419/autoscaling_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/autoscaling/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cat/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cat/v20180409/
+-rw-r--r--   0 root         (0) root         (0)    10939 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cat/v20180409/cat_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cat/v20180409/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    67446 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cat/v20180409/models.py
+-rw-r--r--   0 root         (0) root         (0)     2879 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cat/v20180409/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tag/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tag/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tag/v20180813/
+-rw-r--r--   0 root         (0) root         (0)    28668 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tag/v20180813/tag_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tag/v20180813/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   125754 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tag/v20180813/models.py
+-rw-r--r--   0 root         (0) root         (0)     5579 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tag/v20180813/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/car/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/car/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/car/v20220110/
+-rw-r--r--   0 root         (0) root         (0)     6298 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/car/v20220110/car_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/car/v20220110/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16317 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/car/v20220110/models.py
+-rw-r--r--   0 root         (0) root         (0)     1965 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/car/v20220110/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mrs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mrs/v20200910/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mrs/v20200910/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   702042 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mrs/v20200910/models.py
+-rw-r--r--   0 root         (0) root         (0)     3011 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mrs/v20200910/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     5798 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mrs/v20200910/mrs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mrs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rp/v20200224/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rp/v20200224/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16086 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rp/v20200224/models.py
+-rw-r--r--   0 root         (0) root         (0)     2431 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rp/v20200224/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     2224 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rp/v20200224/rp_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ic/v20190307/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ic/v20190307/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46716 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ic/v20190307/models.py
+-rw-r--r--   0 root         (0) root         (0)     8987 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ic/v20190307/ic_client.py
+-rw-r--r--   0 root         (0) root         (0)      983 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ic/v20190307/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tem/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tem/v20201221/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tem/v20201221/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   117434 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tem/v20201221/models.py
+-rw-r--r--   0 root         (0) root         (0)    15824 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tem/v20201221/tem_client.py
+-rw-r--r--   0 root         (0) root         (0)      747 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tem/v20201221/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tem/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tem/v20210701/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tem/v20210701/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   379345 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tem/v20210701/models.py
+-rw-r--r--   0 root         (0) root         (0)    46073 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tem/v20210701/tem_client.py
+-rw-r--r--   0 root         (0) root         (0)    17128 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tem/v20210701/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gs/v20191118/
+-rw-r--r--   0 root         (0) root         (0)     7857 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gs/v20191118/gs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gs/v20191118/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25245 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gs/v20191118/models.py
+-rw-r--r--   0 root         (0) root         (0)     2065 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gs/v20191118/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trp/v20210515/
+-rw-r--r--   0 root         (0) root         (0)    46794 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trp/v20210515/trp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trp/v20210515/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   253223 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trp/v20210515/models.py
+-rw-r--r--   0 root         (0) root         (0)     1083 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trp/v20210515/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/goosefs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/goosefs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/goosefs/v20220519/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/goosefs/v20220519/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    74135 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/goosefs/v20220519/models.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/goosefs/v20220519/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    19861 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/goosefs/v20220519/goosefs_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bmvpc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bmvpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bmvpc/v20180625/
+-rw-r--r--   0 root         (0) root         (0)    58956 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bmvpc/v20180625/bmvpc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bmvpc/v20180625/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   250943 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bmvpc/v20180625/models.py
+-rw-r--r--   0 root         (0) root         (0)     3260 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bmvpc/v20180625/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dbbrain/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dbbrain/v20210527/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dbbrain/v20210527/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   379052 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dbbrain/v20210527/models.py
+-rw-r--r--   0 root         (0) root         (0)     2143 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dbbrain/v20210527/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    60108 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dbbrain/v20210527/dbbrain_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dbbrain/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dbbrain/v20191016/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dbbrain/v20191016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   183920 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dbbrain/v20191016/models.py
+-rw-r--r--   0 root         (0) root         (0)     1652 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dbbrain/v20191016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    27767 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dbbrain/v20191016/dbbrain_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cpdp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cpdp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cpdp/v20190820/
+-rw-r--r--   0 root         (0) root         (0)   210468 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cpdp/v20190820/cpdp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cpdp/v20190820/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  2033620 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cpdp/v20190820/models.py
+-rw-r--r--   0 root         (0) root         (0)    19183 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cpdp/v20190820/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/domain/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/domain/v20180808/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/domain/v20180808/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   122825 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/domain/v20180808/models.py
+-rw-r--r--   0 root         (0) root         (0)     9007 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/domain/v20180808/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    26115 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/domain/v20180808/domain_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/domain/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mariadb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mariadb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mariadb/v20170312/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mariadb/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   355011 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mariadb/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)    72060 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mariadb/v20170312/mariadb_client.py
+-rw-r--r--   0 root         (0) root         (0)    14932 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mariadb/v20170312/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tmt/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tmt/v20180321/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tmt/v20180321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46724 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tmt/v20180321/models.py
+-rw-r--r--   0 root         (0) root         (0)     9450 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tmt/v20180321/tmt_client.py
+-rw-r--r--   0 root         (0) root         (0)     3623 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tmt/v20180321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tmt/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotexplorer/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotexplorer/v20190423/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotexplorer/v20190423/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   373823 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotexplorer/v20190423/models.py
+-rw-r--r--   0 root         (0) root         (0)    20522 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotexplorer/v20190423/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    85058 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotexplorer/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ses/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ses/v20201002/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ses/v20201002/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   115869 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ses/v20201002/models.py
+-rw-r--r--   0 root         (0) root         (0)    11535 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ses/v20201002/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    29406 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ses/v20201002/ses_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ses/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/casb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/casb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/casb/v20200507/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/casb/v20200507/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5624 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/casb/v20200507/models.py
+-rw-r--r--   0 root         (0) root         (0)      944 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/casb/v20200507/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     2216 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/casb/v20200507/casb_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ticm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ticm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ticm/v20181127/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ticm/v20181127/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    80377 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ticm/v20181127/models.py
+-rw-r--r--   0 root         (0) root         (0)     1329 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ticm/v20181127/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     4025 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ticm/v20181127/ticm_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cbs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cbs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cbs/v20170312/
+-rw-r--r--   0 root         (0) root         (0)    51017 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cbs/v20170312/cbs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cbs/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   227628 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cbs/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)     7755 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cbs/v20170312/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tic/v20201117/
+-rw-r--r--   0 root         (0) root         (0)    14464 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tic/v20201117/tic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tic/v20201117/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43811 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tic/v20201117/models.py
+-rw-r--r--   0 root         (0) root         (0)     1450 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tic/v20201117/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tat/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tat/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tat/v20201028/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tat/v20201028/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   159502 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tat/v20201028/models.py
+-rw-r--r--   0 root         (0) root         (0)     8096 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tat/v20201028/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    27476 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tat/v20201028/tat_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/advisor/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/advisor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/advisor/v20200721/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/advisor/v20200721/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17632 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/advisor/v20200721/models.py
+-rw-r--r--   0 root         (0) root         (0)     2848 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/advisor/v20200721/advisor_client.py
+-rw-r--r--   0 root         (0) root         (0)     1113 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/advisor/v20200721/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/facefusion/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/facefusion/v20181201/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/facefusion/v20181201/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    39231 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/facefusion/v20181201/models.py
+-rw-r--r--   0 root         (0) root         (0)     6831 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/facefusion/v20181201/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     5813 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/facefusion/v20181201/facefusion_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/facefusion/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/facefusion/v20220927/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/facefusion/v20220927/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25364 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/facefusion/v20220927/models.py
+-rw-r--r--   0 root         (0) root         (0)     5623 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/facefusion/v20220927/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     3394 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/facefusion/v20220927/facefusion_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcr/v20190924/
+-rw-r--r--   0 root         (0) root         (0)   105482 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcr/v20190924/tcr_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcr/v20190924/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   448531 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcr/v20190924/models.py
+-rw-r--r--   0 root         (0) root         (0)     8622 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcr/v20190924/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbaas/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbaas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbaas/v20180416/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbaas/v20180416/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112703 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbaas/v20180416/models.py
+-rw-r--r--   0 root         (0) root         (0)    10664 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbaas/v20180416/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    20172 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbaas/v20180416/tbaas_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cvm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cvm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cvm/v20170312/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cvm/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   626813 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cvm/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)    45566 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cvm/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   120056 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cvm/v20170312/cvm_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/anicloud/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/anicloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/anicloud/v20220923/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/anicloud/v20220923/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19109 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/anicloud/v20220923/models.py
+-rw-r--r--   0 root         (0) root         (0)      709 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/anicloud/v20220923/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     3623 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/anicloud/v20220923/anicloud_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/hasim/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/hasim/v20210716/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/hasim/v20210716/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   123000 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/hasim/v20210716/models.py
+-rw-r--r--   0 root         (0) root         (0)     1393 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/hasim/v20210716/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    19722 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/hasim/v20210716/hasim_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/hasim/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cme/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cme/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cme/v20191029/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cme/v20191029/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   445345 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cme/v20191029/models.py
+-rw-r--r--   0 root         (0) root         (0)    55451 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cme/v20191029/cme_client.py
+-rw-r--r--   0 root         (0) root         (0)     8415 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cme/v20191029/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/clb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/clb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/clb/v20180317/
+-rw-r--r--   0 root         (0) root         (0)    95722 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/clb/v20180317/clb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/clb/v20180317/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   531752 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/clb/v20180317/models.py
+-rw-r--r--   0 root         (0) root         (0)     3269 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/clb/v20180317/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tse/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tse/v20201207/
+-rw-r--r--   0 root         (0) root         (0)    49343 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tse/v20201207/tse_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tse/v20201207/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   350755 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tse/v20201207/models.py
+-rw-r--r--   0 root         (0) root         (0)     5600 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tse/v20201207/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ie/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ie/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ie/v20200304/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ie/v20200304/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   233379 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ie/v20200304/models.py
+-rw-r--r--   0 root         (0) root         (0)     4235 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ie/v20200304/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    11025 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ie/v20200304/ie_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/smop/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/smop/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/smop/v20201203/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/smop/v20201203/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11024 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/smop/v20201203/models.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/smop/v20201203/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     1866 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/smop/v20201203/smop_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdb/v20170320/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdb/v20170320/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   803999 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdb/v20170320/models.py
+-rw-r--r--   0 root         (0) root         (0)    20514 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdb/v20170320/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   148592 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdb/v20170320/cdb_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/redis/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/redis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/redis/v20180412/
+-rw-r--r--   0 root         (0) root         (0)    87874 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/redis/v20180412/redis_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/redis/v20180412/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   467296 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/redis/v20180412/models.py
+-rw-r--r--   0 root         (0) root         (0)    12423 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/redis/v20180412/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tms/v20201229/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tms/v20201229/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28735 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tms/v20201229/models.py
+-rw-r--r--   0 root         (0) root         (0)     1723 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tms/v20201229/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     3551 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tms/v20201229/tms_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tms/v20200713/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tms/v20200713/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40163 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tms/v20200713/models.py
+-rw-r--r--   0 root         (0) root         (0)     3027 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tms/v20200713/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     4674 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tms/v20200713/tms_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/region/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/region/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/region/v20220627/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/region/v20220627/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    18296 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/region/v20220627/models.py
+-rw-r--r--   0 root         (0) root         (0)     3756 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/region/v20220627/region_client.py
+-rw-r--r--   0 root         (0) root         (0)      866 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/region/v20220627/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tke/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tke/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tke/v20180525/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tke/v20180525/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1119184 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tke/v20180525/models.py
+-rw-r--r--   0 root         (0) root         (0)    19924 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tke/v20180525/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   199717 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tke/v20180525/tke_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cr/v20180321/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cr/v20180321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   136120 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cr/v20180321/models.py
+-rw-r--r--   0 root         (0) root         (0)    26131 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cr/v20180321/cr_client.py
+-rw-r--r--   0 root         (0) root         (0)     4158 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cr/v20180321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/btoe/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/btoe/v20210514/
+-rw-r--r--   0 root         (0) root         (0)    14662 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/btoe/v20210514/btoe_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/btoe/v20210514/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43354 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/btoe/v20210514/models.py
+-rw-r--r--   0 root         (0) root         (0)     3235 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/btoe/v20210514/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/btoe/v20210303/
+-rw-r--r--   0 root         (0) root         (0)    14684 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/btoe/v20210303/btoe_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/btoe/v20210303/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    47728 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/btoe/v20210303/models.py
+-rw-r--r--   0 root         (0) root         (0)     3211 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/btoe/v20210303/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/btoe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dsgc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dsgc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dsgc/v20190723/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dsgc/v20190723/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   797805 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dsgc/v20190723/models.py
+-rw-r--r--   0 root         (0) root         (0)   145268 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dsgc/v20190723/dsgc_client.py
+-rw-r--r--   0 root         (0) root         (0)     1791 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dsgc/v20190723/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cynosdb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cynosdb/v20190107/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cynosdb/v20190107/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   712502 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cynosdb/v20190107/models.py
+-rw-r--r--   0 root         (0) root         (0)    11512 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cynosdb/v20190107/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   120044 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cynosdb/v20190107/cynosdb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cynosdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/af/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/af/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/af/v20200226/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/af/v20200226/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54195 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/af/v20200226/models.py
+-rw-r--r--   0 root         (0) root         (0)     4164 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/af/v20200226/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     4131 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/af/v20200226/af_client.py
+-rw-r--r--   0 root         (0) root         (0)      630 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ft/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ft/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ft/v20200304/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ft/v20200304/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    29493 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ft/v20200304/models.py
+-rw-r--r--   0 root         (0) root         (0)     5649 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ft/v20200304/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     6827 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ft/v20200304/ft_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/acp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/acp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/acp/v20220105/
+-rw-r--r--   0 root         (0) root         (0)     8408 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/acp/v20220105/acp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/acp/v20220105/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53725 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/acp/v20220105/models.py
+-rw-r--r--   0 root         (0) root         (0)      832 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/acp/v20220105/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sms/v20210111/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sms/v20210111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   104906 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sms/v20210111/models.py
+-rw-r--r--   0 root         (0) root         (0)    19344 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sms/v20210111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    28405 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sms/v20210111/sms_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sms/v20190711/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sms/v20190711/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93677 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sms/v20190711/models.py
+-rw-r--r--   0 root         (0) root         (0)    18522 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sms/v20190711/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    26631 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sms/v20190711/sms_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lcic/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lcic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lcic/v20220817/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lcic/v20220817/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   248641 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lcic/v20220817/models.py
+-rw-r--r--   0 root         (0) root         (0)     4699 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lcic/v20220817/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    50664 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lcic/v20220817/lcic_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/fmu/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/fmu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/fmu/v20191213/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/fmu/v20191213/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45807 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/fmu/v20191213/models.py
+-rw-r--r--   0 root         (0) root         (0)     6925 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/fmu/v20191213/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    10618 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/fmu/v20191213/fmu_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/teo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/teo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/teo/v20220106/
+-rw-r--r--   0 root         (0) root         (0)     5399 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/teo/v20220106/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/teo/v20220106/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38737 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/teo/v20220106/models.py
+-rw-r--r--   0 root         (0) root         (0)     2192 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/teo/v20220106/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/teo/v20220901/
+-rw-r--r--   0 root         (0) root         (0)    61993 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/teo/v20220901/teo_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/teo/v20220901/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   625407 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/teo/v20220901/models.py
+-rw-r--r--   0 root         (0) root         (0)    28390 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/teo/v20220901/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ciam/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ciam/v20220331/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ciam/v20220331/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   139059 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ciam/v20220331/models.py
+-rw-r--r--   0 root         (0) root         (0)     8558 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ciam/v20220331/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    20721 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ciam/v20220331/ciam_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ciam/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/monitor/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/monitor/v20180724/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/monitor/v20180724/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   871012 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/monitor/v20180724/models.py
+-rw-r--r--   0 root         (0) root         (0)    10348 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/monitor/v20180724/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   145293 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/monitor/v20180724/monitor_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/monitor/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ecc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ecc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ecc/v20181213/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ecc/v20181213/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40735 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ecc/v20181213/models.py
+-rw-r--r--   0 root         (0) root         (0)     3889 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ecc/v20181213/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     4497 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ecc/v20181213/ecc_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bizlive/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bizlive/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bizlive/v20190313/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bizlive/v20190313/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    19225 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bizlive/v20190313/models.py
+-rw-r--r--   0 root         (0) root         (0)     2083 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bizlive/v20190313/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     6329 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bizlive/v20190313/bizlive_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/irp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/irp/v20220324/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/irp/v20220324/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    54088 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/irp/v20220324/models.py
+-rw-r--r--   0 root         (0) root         (0)      961 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/irp/v20220324/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     4389 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/irp/v20220324/irp_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/irp/v20220805/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/irp/v20220805/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81404 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/irp/v20220805/models.py
+-rw-r--r--   0 root         (0) root         (0)     1018 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/irp/v20220805/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     7365 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/irp/v20220805/irp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/irp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/faceid/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/faceid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/faceid/v20180301/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/faceid/v20180301/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   222483 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/faceid/v20180301/models.py
+-rw-r--r--   0 root         (0) root         (0)     9370 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/faceid/v20180301/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    34162 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/faceid/v20180301/faceid_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tics/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tics/v20181115/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tics/v20181115/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28834 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tics/v20181115/models.py
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tics/v20181115/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     4917 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tics/v20181115/tics_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/nlp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/nlp/v20190408/
+-rw-r--r--   0 root         (0) root         (0)    13476 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/nlp/v20190408/nlp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/nlp/v20190408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    52142 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/nlp/v20190408/models.py
+-rw-r--r--   0 root         (0) root         (0)     4521 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/nlp/v20190408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/nlp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/waf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/waf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/waf/v20180125/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/waf/v20180125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   618583 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/waf/v20180125/models.py
+-rw-r--r--   0 root         (0) root         (0)     5741 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/waf/v20180125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   112925 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/waf/v20180125/waf_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gaap/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gaap/v20180529/
+-rw-r--r--   0 root         (0) root         (0)   101614 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gaap/v20180529/gaap_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gaap/v20180529/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   516159 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gaap/v20180529/models.py
+-rw-r--r--   0 root         (0) root         (0)    11791 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gaap/v20180529/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gaap/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tan/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tan/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tan/v20220420/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tan/v20220420/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2967 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tan/v20220420/models.py
+-rw-r--r--   0 root         (0) root         (0)     2281 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tan/v20220420/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     1896 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tan/v20220420/tan_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vod/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vod/v20180717/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vod/v20180717/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1876797 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vod/v20180717/models.py
+-rw-r--r--   0 root         (0) root         (0)    25211 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vod/v20180717/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   185303 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vod/v20180717/vod_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ecm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ecm/v20190719/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ecm/v20190719/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   733514 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ecm/v20190719/models.py
+-rw-r--r--   0 root         (0) root         (0)    23498 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ecm/v20190719/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   136183 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ecm/v20190719/ecm_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ecm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lowcode/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lowcode/v20210108/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lowcode/v20210108/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26092 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lowcode/v20210108/models.py
+-rw-r--r--   0 root         (0) root         (0)     1929 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lowcode/v20210108/lowcode_client.py
+-rw-r--r--   0 root         (0) root         (0)      948 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lowcode/v20210108/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lowcode/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ms/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ms/v20180408/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ms/v20180408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   180152 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ms/v20180408/models.py
+-rw-r--r--   0 root         (0) root         (0)     5911 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ms/v20180408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    23945 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ms/v20180408/ms_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vrs/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vrs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vrs/v20200824/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vrs/v20200824/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28696 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vrs/v20200824/models.py
+-rw-r--r--   0 root         (0) root         (0)     2156 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vrs/v20200824/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     7458 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vrs/v20200824/vrs_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bri/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bri/v20190328/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bri/v20190328/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    11308 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bri/v20190328/models.py
+-rw-r--r--   0 root         (0) root         (0)     2407 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bri/v20190328/bri_client.py
+-rw-r--r--   0 root         (0) root         (0)     2171 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bri/v20190328/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bri/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cis/v20180408/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cis/v20180408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    38589 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cis/v20180408/models.py
+-rw-r--r--   0 root         (0) root         (0)      760 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cis/v20180408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     7726 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cis/v20180408/cis_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gse/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gse/v20191112/
+-rw-r--r--   0 root         (0) root         (0)    89371 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gse/v20191112/gse_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gse/v20191112/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   387109 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gse/v20191112/models.py
+-rw-r--r--   0 root         (0) root         (0)     2578 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gse/v20191112/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tourism/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tourism/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tourism/v20230215/
+-rw-r--r--   0 root         (0) root         (0)     1959 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tourism/v20230215/tourism_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tourism/v20230215/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8749 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tourism/v20230215/models.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tourism/v20230215/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/apigateway/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/apigateway/v20180808/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/apigateway/v20180808/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   648978 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/apigateway/v20180808/models.py
+-rw-r--r--   0 root         (0) root         (0)    22090 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/apigateway/v20180808/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    95541 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/apigateway/v20180808/apigateway_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/apigateway/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iai/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iai/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iai/v20180301/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iai/v20180301/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   236091 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iai/v20180301/models.py
+-rw-r--r--   0 root         (0) root         (0)    11999 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iai/v20180301/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    46290 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iai/v20180301/iai_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iai/v20200303/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iai/v20200303/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   251563 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iai/v20200303/models.py
+-rw-r--r--   0 root         (0) root         (0)    12105 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iai/v20200303/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    49515 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iai/v20200303/iai_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/es/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/es/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/es/v20180416/
+-rw-r--r--   0 root         (0) root         (0)    36126 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/es/v20180416/es_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/es/v20180416/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   298586 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/es/v20180416/models.py
+-rw-r--r--   0 root         (0) root         (0)    21311 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/es/v20180416/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eb/v20210416/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eb/v20210416/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   152636 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eb/v20210416/models.py
+-rw-r--r--   0 root         (0) root         (0)    14675 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eb/v20210416/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    28438 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eb/v20210416/eb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bda/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bda/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bda/v20200324/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bda/v20200324/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112857 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bda/v20200324/models.py
+-rw-r--r--   0 root         (0) root         (0)     8576 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bda/v20200324/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    20667 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bda/v20200324/bda_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dasb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dasb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dasb/v20191018/
+-rw-r--r--   0 root         (0) root         (0)    48361 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dasb/v20191018/dasb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dasb/v20191018/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   279575 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dasb/v20191018/models.py
+-rw-r--r--   0 root         (0) root         (0)     2500 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dasb/v20191018/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ecdn/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ecdn/v20191012/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ecdn/v20191012/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   120841 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ecdn/v20191012/models.py
+-rw-r--r--   0 root         (0) root         (0)     9228 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ecdn/v20191012/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    20324 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ecdn/v20191012/ecdn_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ecdn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/postgres/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/postgres/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/postgres/v20170312/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/postgres/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   475358 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/postgres/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)    21166 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/postgres/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    91035 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/postgres/v20170312/postgres_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/youmall/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/youmall/v20180228/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/youmall/v20180228/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   184858 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/youmall/v20180228/models.py
+-rw-r--r--   0 root         (0) root         (0)     2828 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/youmall/v20180228/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    31517 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/youmall/v20180228/youmall_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/youmall/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dts/v20180330/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dts/v20180330/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   124284 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dts/v20180330/models.py
+-rw-r--r--   0 root         (0) root         (0)     5619 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dts/v20180330/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    24853 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dts/v20180330/dts_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dts/v20211206/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dts/v20211206/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   353467 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dts/v20211206/models.py
+-rw-r--r--   0 root         (0) root         (0)     6952 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dts/v20211206/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    49338 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dts/v20211206/dts_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/common/
+-rw-r--r--   0 root         (0) root         (0)    21860 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/common/abstract_client.py
+-rw-r--r--   0 root         (0) root         (0)     1568 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/common/sign.py
+-rw-r--r--   0 root         (0) root         (0)     2335 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/common/abstract_model.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/common/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/common/exception/
+-rw-r--r--   0 root         (0) root         (0)      735 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/common/exception/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      760 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/common/exception/tencent_cloud_sdk_exception.py
+-rw-r--r--   0 root         (0) root         (0)     1958 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/common/common_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/common/http/
+-rw-r--r--   0 root         (0) root         (0)     4456 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/common/http/request.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/common/http/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/common/profile/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/common/profile/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1893 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/common/profile/http_profile.py
+-rw-r--r--   0 root         (0) root         (0)     4534 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/common/profile/client_profile.py
+-rw-r--r--   0 root         (0) root         (0)     4301 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/common/circuit_breaker.py
+-rw-r--r--   0 root         (0) root         (0)    15945 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/common/credential.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ba/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ba/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ba/v20200720/
+-rw-r--r--   0 root         (0) root         (0)     3804 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ba/v20200720/ba_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ba/v20200720/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7466 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ba/v20200720/models.py
+-rw-r--r--   0 root         (0) root         (0)     1047 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ba/v20200720/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tia/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tia/v20180226/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tia/v20180226/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    49879 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tia/v20180226/models.py
+-rw-r--r--   0 root         (0) root         (0)     2747 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tia/v20180226/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    10682 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tia/v20180226/tia_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tia/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/taf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/taf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/taf/v20200210/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/taf/v20200210/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    25951 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/taf/v20200210/models.py
+-rw-r--r--   0 root         (0) root         (0)     4808 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/taf/v20200210/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     3826 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/taf/v20200210/taf_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ame/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ame/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ame/v20190916/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ame/v20190916/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   193152 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ame/v20190916/models.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ame/v20190916/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    29579 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ame/v20190916/ame_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcbr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcbr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcbr/v20220217/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcbr/v20220217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    88962 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcbr/v20220217/models.py
+-rw-r--r--   0 root         (0) root         (0)     1182 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcbr/v20220217/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    10074 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcbr/v20220217/tcbr_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/csxg/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/csxg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/csxg/v20230303/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/csxg/v20230303/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     4254 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/csxg/v20230303/models.py
+-rw-r--r--   0 root         (0) root         (0)     5397 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/csxg/v20230303/csxg_client.py
+-rw-r--r--   0 root         (0) root         (0)      769 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/csxg/v20230303/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/smpn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/smpn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/smpn/v20190822/
+-rw-r--r--   0 root         (0) root         (0)     5314 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/smpn/v20190822/smpn_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/smpn/v20190822/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24181 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/smpn/v20190822/models.py
+-rw-r--r--   0 root         (0) root         (0)     1008 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/smpn/v20190822/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cii/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cii/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cii/v20210408/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cii/v20210408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    87370 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cii/v20210408/models.py
+-rw-r--r--   0 root         (0) root         (0)    13689 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cii/v20210408/cii_client.py
+-rw-r--r--   0 root         (0) root         (0)     1358 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cii/v20210408/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cii/v20201210/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cii/v20201210/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16873 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cii/v20201210/models.py
+-rw-r--r--   0 root         (0) root         (0)     3891 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cii/v20201210/cii_client.py
+-rw-r--r--   0 root         (0) root         (0)     1065 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cii/v20201210/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cds/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cds/v20180420/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cds/v20180420/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24914 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cds/v20180420/models.py
+-rw-r--r--   0 root         (0) root         (0)     6824 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cds/v20180420/cds_client.py
+-rw-r--r--   0 root         (0) root         (0)      966 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cds/v20180420/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cds/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/afc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/afc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/afc/v20200226/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/afc/v20200226/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    40384 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/afc/v20200226/models.py
+-rw-r--r--   0 root         (0) root         (0)     3863 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/afc/v20200226/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     3940 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/afc/v20200226/afc_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/aai/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/aai/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/aai/v20180522/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/aai/v20180522/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20548 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/aai/v20180522/models.py
+-rw-r--r--   0 root         (0) root         (0)     4705 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/aai/v20180522/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     5497 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/aai/v20180522/aai_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/csip/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/csip/v20221121/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/csip/v20221121/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   342265 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/csip/v20221121/models.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/csip/v20221121/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    28721 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/csip/v20221121/csip_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/csip/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dataintegration/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dataintegration/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dataintegration/v20220613/
+-rw-r--r--   0 root         (0) root         (0)     1914 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dataintegration/v20220613/dataintegration_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dataintegration/v20220613/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3967 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dataintegration/v20220613/models.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dataintegration/v20220613/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/npp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/npp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/npp/v20190823/
+-rw-r--r--   0 root         (0) root         (0)     7974 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/npp/v20190823/npp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/npp/v20190823/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    60419 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/npp/v20190823/models.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/npp/v20190823/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iss/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iss/v20230517/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iss/v20230517/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   436666 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iss/v20230517/models.py
+-rw-r--r--   0 root         (0) root         (0)    18801 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iss/v20230517/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    75806 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iss/v20230517/iss_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iss/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/captcha/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/captcha/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/captcha/v20190722/
+-rw-r--r--   0 root         (0) root         (0)    17853 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/captcha/v20190722/captcha_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/captcha/v20190722/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   117646 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/captcha/v20190722/models.py
+-rw-r--r--   0 root         (0) root         (0)     1037 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/captcha/v20190722/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trdp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trdp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trdp/v20220726/
+-rw-r--r--   0 root         (0) root         (0)     1872 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trdp/v20220726/trdp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trdp/v20220726/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    37532 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trdp/v20220726/models.py
+-rw-r--r--   0 root         (0) root         (0)     1158 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trdp/v20220726/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/chdfs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/chdfs/v20190718/
+-rw-r--r--   0 root         (0) root         (0)    28126 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/chdfs/v20190718/chdfs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/chdfs/v20190718/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    78138 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/chdfs/v20190718/models.py
+-rw-r--r--   0 root         (0) root         (0)     3280 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/chdfs/v20190718/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/chdfs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/chdfs/v20201112/
+-rw-r--r--   0 root         (0) root         (0)    27402 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/chdfs/v20201112/chdfs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/chdfs/v20201112/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92834 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/chdfs/v20201112/models.py
+-rw-r--r--   0 root         (0) root         (0)     3600 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/chdfs/v20201112/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mmps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mmps/v20200710/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mmps/v20200710/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    83019 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mmps/v20200710/models.py
+-rw-r--r--   0 root         (0) root         (0)      775 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mmps/v20200710/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    15527 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mmps/v20200710/mmps_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mmps/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/api/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/api/v20201106/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/api/v20201106/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17428 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/api/v20201106/models.py
+-rw-r--r--   0 root         (0) root         (0)     3726 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/api/v20201106/api_client.py
+-rw-r--r--   0 root         (0) root         (0)      866 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/api/v20201106/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/api/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/organization/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/organization/v20181225/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/organization/v20181225/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    46488 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/organization/v20181225/models.py
+-rw-r--r--   0 root         (0) root         (0)    19700 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/organization/v20181225/organization_client.py
+-rw-r--r--   0 root         (0) root         (0)     3243 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/organization/v20181225/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/organization/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/organization/v20210331/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/organization/v20210331/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   130314 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/organization/v20210331/models.py
+-rw-r--r--   0 root         (0) root         (0)    30181 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/organization/v20210331/organization_client.py
+-rw-r--r--   0 root         (0) root         (0)    12433 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/organization/v20210331/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tci/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tci/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tci/v20190318/
+-rw-r--r--   0 root         (0) root         (0)    44187 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tci/v20190318/tci_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tci/v20190318/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   285108 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tci/v20190318/models.py
+-rw-r--r--   0 root         (0) root         (0)     8913 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tci/v20190318/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ckafka/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ckafka/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ckafka/v20190819/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ckafka/v20190819/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   785875 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ckafka/v20190819/models.py
+-rw-r--r--   0 root         (0) root         (0)     3315 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ckafka/v20190819/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    73707 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ckafka/v20190819/ckafka_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tds/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tds/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tds/v20220801/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tds/v20220801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27293 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tds/v20220801/models.py
+-rw-r--r--   0 root         (0) root         (0)     4548 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tds/v20220801/tds_client.py
+-rw-r--r--   0 root         (0) root         (0)      772 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tds/v20220801/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dbdc/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dbdc/v20201029/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dbdc/v20201029/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    72272 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dbdc/v20201029/models.py
+-rw-r--r--   0 root         (0) root         (0)     2111 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dbdc/v20201029/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     6439 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dbdc/v20201029/dbdc_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dbdc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudhsm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudhsm/v20191112/
+-rw-r--r--   0 root         (0) root         (0)    13347 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudhsm/v20191112/cloudhsm_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudhsm/v20191112/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    81651 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudhsm/v20191112/models.py
+-rw-r--r--   0 root         (0) root         (0)     1020 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudhsm/v20191112/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudhsm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tiems/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tiems/v20190416/
+-rw-r--r--   0 root         (0) root         (0)    28234 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tiems/v20190416/tiems_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tiems/v20190416/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   151851 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tiems/v20190416/models.py
+-rw-r--r--   0 root         (0) root         (0)     1108 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tiems/v20190416/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tiems/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bmeip/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bmeip/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bmeip/v20180625/
+-rw-r--r--   0 root         (0) root         (0)    18032 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bmeip/v20180625/bmeip_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bmeip/v20180625/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    69899 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bmeip/v20180625/models.py
+-rw-r--r--   0 root         (0) root         (0)      820 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bmeip/v20180625/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ssm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ssm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ssm/v20190923/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ssm/v20190923/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   100023 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ssm/v20190923/models.py
+-rw-r--r--   0 root         (0) root         (0)     3474 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ssm/v20190923/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    24609 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ssm/v20190923/ssm_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cfs/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cfs/v20190719/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cfs/v20190719/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   195707 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cfs/v20190719/models.py
+-rw-r--r--   0 root         (0) root         (0)    15890 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cfs/v20190719/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    40047 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cfs/v20190719/cfs_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cfs/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tsw/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tsw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tsw/v20200924/
+-rw-r--r--   0 root         (0) root         (0)     1878 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tsw/v20200924/tsw_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tsw/v20200924/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5590 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tsw/v20200924/models.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tsw/v20200924/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tsw/v20210412/
+-rw-r--r--   0 root         (0) root         (0)     3722 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tsw/v20210412/tsw_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tsw/v20210412/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     3911 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tsw/v20210412/models.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tsw/v20210412/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yunjing/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yunjing/v20180228/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yunjing/v20180228/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   379701 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yunjing/v20180228/models.py
+-rw-r--r--   0 root         (0) root         (0)    94372 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yunjing/v20180228/yunjing_client.py
+-rw-r--r--   0 root         (0) root         (0)     3960 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yunjing/v20180228/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yunjing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gpm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gpm/v20200820/
+-rw-r--r--   0 root         (0) root         (0)    18269 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gpm/v20200820/gpm_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gpm/v20200820/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   100825 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gpm/v20200820/models.py
+-rw-r--r--   0 root         (0) root         (0)     5641 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gpm/v20200820/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gpm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tdid/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tdid/v20210519/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tdid/v20210519/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    43358 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tdid/v20210519/models.py
+-rw-r--r--   0 root         (0) root         (0)    12712 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tdid/v20210519/tdid_client.py
+-rw-r--r--   0 root         (0) root         (0)     1775 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tdid/v20210519/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tdid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/apm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/apm/v20210622/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/apm/v20210622/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    85514 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/apm/v20210622/models.py
+-rw-r--r--   0 root         (0) root         (0)     3646 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/apm/v20210622/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     9241 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/apm/v20210622/apm_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/apm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/solar/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/solar/v20181011/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/solar/v20181011/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    88391 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/solar/v20181011/models.py
+-rw-r--r--   0 root         (0) root         (0)     1500 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/solar/v20181011/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    15882 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/solar/v20181011/solar_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/solar/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gme/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gme/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gme/v20180711/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gme/v20180711/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   159505 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gme/v20180711/models.py
+-rw-r--r--   0 root         (0) root         (0)     4026 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gme/v20180711/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    34890 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/gme/v20180711/gme_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/icr/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/icr/v20211014/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/icr/v20211014/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26493 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/icr/v20211014/models.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/icr/v20211014/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     1914 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/icr/v20211014/icr_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/icr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rkp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rkp/v20191209/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rkp/v20191209/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    21607 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rkp/v20191209/models.py
+-rw-r--r--   0 root         (0) root         (0)     3783 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rkp/v20191209/rkp_client.py
+-rw-r--r--   0 root         (0) root         (0)     3080 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rkp/v20191209/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rkp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/hcm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/hcm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/hcm/v20181106/
+-rw-r--r--   0 root         (0) root         (0)     1947 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/hcm/v20181106/hcm_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/hcm/v20181106/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    14772 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/hcm/v20181106/models.py
+-rw-r--r--   0 root         (0) root         (0)     2630 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/hcm/v20181106/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mna/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mna/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mna/v20210119/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mna/v20210119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    67068 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mna/v20210119/models.py
+-rw-r--r--   0 root         (0) root         (0)     2902 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mna/v20210119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    12133 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mna/v20210119/mna_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdwpg/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdwpg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdwpg/v20201230/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdwpg/v20201230/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48854 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdwpg/v20201230/models.py
+-rw-r--r--   0 root         (0) root         (0)      737 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdwpg/v20201230/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     6392 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdwpg/v20201230/cdwpg_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/v20201215/
+-rw-r--r--   0 root         (0) root         (0)    72567 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/v20201215/iotvideo_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/v20201215/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   304127 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/v20201215/models.py
+-rw-r--r--   0 root         (0) root         (0)     1977 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/v20201215/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/v20191126/
+-rw-r--r--   0 root         (0) root         (0)    64723 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/v20191126/iotvideo_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/v20191126/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   229605 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/v20191126/models.py
+-rw-r--r--   0 root         (0) root         (0)     3098 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/v20191126/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/v20211125/
+-rw-r--r--   0 root         (0) root         (0)    91083 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/v20211125/iotvideo_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/v20211125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   381639 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/v20211125/models.py
+-rw-r--r--   0 root         (0) root         (0)     2198 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/v20211125/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mongodb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mongodb/v20180408/
+-rw-r--r--   0 root         (0) root         (0)    13623 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mongodb/v20180408/mongodb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mongodb/v20180408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76740 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mongodb/v20180408/models.py
+-rw-r--r--   0 root         (0) root         (0)     3903 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mongodb/v20180408/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mongodb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mongodb/v20190725/
+-rw-r--r--   0 root         (0) root         (0)    36587 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mongodb/v20190725/mongodb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mongodb/v20190725/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   234826 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mongodb/v20190725/models.py
+-rw-r--r--   0 root         (0) root         (0)     7304 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mongodb/v20190725/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iot/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iot/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iot/v20180123/
+-rw-r--r--   0 root         (0) root         (0)    40904 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iot/v20180123/iot_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iot/v20180123/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   171391 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iot/v20180123/models.py
+-rw-r--r--   0 root         (0) root         (0)     6163 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iot/v20180123/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vm/v20201229/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vm/v20201229/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    95121 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vm/v20201229/models.py
+-rw-r--r--   0 root         (0) root         (0)     9185 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vm/v20201229/vm_client.py
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vm/v20201229/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vm/v20210922/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vm/v20210922/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    84771 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vm/v20210922/models.py
+-rw-r--r--   0 root         (0) root         (0)     5305 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vm/v20210922/vm_client.py
+-rw-r--r--   0 root         (0) root         (0)     1967 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vm/v20210922/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vm/v20200709/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vm/v20200709/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    76744 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vm/v20200709/models.py
+-rw-r--r--   0 root         (0) root         (0)     5863 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vm/v20200709/vm_client.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vm/v20200709/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ams/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ams/v20201229/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ams/v20201229/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    93055 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ams/v20201229/models.py
+-rw-r--r--   0 root         (0) root         (0)     3347 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ams/v20201229/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    10675 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ams/v20201229/ams_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ams/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ams/v20200608/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ams/v20200608/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89744 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ams/v20200608/models.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ams/v20200608/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     9160 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ams/v20200608/ams_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcm/v20210413/
+-rw-r--r--   0 root         (0) root         (0)    11262 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcm/v20210413/tcm_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcm/v20210413/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   130072 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcm/v20210413/models.py
+-rw-r--r--   0 root         (0) root         (0)     1334 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcm/v20210413/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tav/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tav/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tav/v20190118/
+-rw-r--r--   0 root         (0) root         (0)     4395 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tav/v20190118/tav_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tav/v20190118/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12546 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tav/v20190118/models.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tav/v20190118/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sslpod/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sslpod/v20190605/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sslpod/v20190605/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41178 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sslpod/v20190605/models.py
+-rw-r--r--   0 root         (0) root         (0)     2079 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sslpod/v20190605/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     9749 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sslpod/v20190605/sslpod_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sslpod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bmlb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bmlb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bmlb/v20180625/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bmlb/v20180625/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   327109 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bmlb/v20180625/models.py
+-rw-r--r--   0 root         (0) root         (0)    47282 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bmlb/v20180625/bmlb_client.py
+-rw-r--r--   0 root         (0) root         (0)      929 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bmlb/v20180625/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/wss/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/wss/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/wss/v20180426/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/wss/v20180426/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    24432 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/wss/v20180426/models.py
+-rw-r--r--   0 root         (0) root         (0)     1239 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/wss/v20180426/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     3606 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/wss/v20180426/wss_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cfg/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cfg/v20210820/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cfg/v20210820/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   123448 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cfg/v20210820/models.py
+-rw-r--r--   0 root         (0) root         (0)     1933 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cfg/v20210820/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     9735 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cfg/v20210820/cfg_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cfg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/aa/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/aa/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/aa/v20200224/
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/aa/v20200224/aa_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/aa/v20200224/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17163 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/aa/v20200224/models.py
+-rw-r--r--   0 root         (0) root         (0)     2430 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/aa/v20200224/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vpc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vpc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vpc/v20170312/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vpc/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1365413 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vpc/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)    45216 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vpc/v20170312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   342735 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/vpc/v20170312/vpc_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideoindustry/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideoindustry/v20201201/
+-rw-r--r--   0 root         (0) root         (0)   100347 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideoindustry/v20201201/iotvideoindustry_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideoindustry/v20201201/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   369812 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideoindustry/v20201201/models.py
+-rw-r--r--   0 root         (0) root         (0)     8583 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideoindustry/v20201201/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideoindustry/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mps/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mps/v20190612/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mps/v20190612/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1333652 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mps/v20190612/models.py
+-rw-r--r--   0 root         (0) root         (0)    13604 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mps/v20190612/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   100285 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mps/v20190612/mps_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mps/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ape/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ape/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ape/v20200513/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ape/v20200513/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    42775 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ape/v20200513/models.py
+-rw-r--r--   0 root         (0) root         (0)     1570 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ape/v20200513/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     8191 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ape/v20200513/ape_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcaplusdb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcaplusdb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcaplusdb/v20190823/
+-rw-r--r--   0 root         (0) root         (0)    49200 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcaplusdb/v20190823/tcaplusdb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcaplusdb/v20190823/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   309127 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcaplusdb/v20190823/models.py
+-rw-r--r--   0 root         (0) root         (0)     3614 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcaplusdb/v20190823/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dayu/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dayu/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dayu/v20180709/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dayu/v20180709/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   545180 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dayu/v20180709/models.py
+-rw-r--r--   0 root         (0) root         (0)     1440 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dayu/v20180709/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   103066 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dayu/v20180709/dayu_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/weilingwith/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/weilingwith/v20230427/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/weilingwith/v20230427/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13098 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/weilingwith/v20230427/models.py
+-rw-r--r--   0 root         (0) root         (0)     1405 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/weilingwith/v20230427/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     5703 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/weilingwith/v20230427/weilingwith_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/weilingwith/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/scf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/scf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/scf/v20180416/
+-rw-r--r--   0 root         (0) root         (0)    44580 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/scf/v20180416/scf_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/scf/v20180416/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   322505 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/scf/v20180416/models.py
+-rw-r--r--   0 root         (0) root         (0)    32699 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/scf/v20180416/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lp/v20200224/
+-rw-r--r--   0 root         (0) root         (0)     2098 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lp/v20200224/lp_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lp/v20200224/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17582 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lp/v20200224/models.py
+-rw-r--r--   0 root         (0) root         (0)     2430 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lp/v20200224/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cim/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cim/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cim/v20190318/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cim/v20190318/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     1779 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cim/v20190318/models.py
+-rw-r--r--   0 root         (0) root         (0)      827 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cim/v20190318/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     1894 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cim/v20190318/cim_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lighthouse/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lighthouse/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lighthouse/v20200324/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lighthouse/v20200324/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   449067 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lighthouse/v20200324/models.py
+-rw-r--r--   0 root         (0) root         (0)    28428 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lighthouse/v20200324/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   117975 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/lighthouse/v20200324/lighthouse_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/keewidb/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/keewidb/v20220308/
+-rw-r--r--   0 root         (0) root         (0)    37435 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/keewidb/v20220308/keewidb_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/keewidb/v20220308/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   219041 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/keewidb/v20220308/models.py
+-rw-r--r--   0 root         (0) root         (0)     5660 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/keewidb/v20220308/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/keewidb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tdcpg/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tdcpg/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tdcpg/v20211118/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tdcpg/v20211118/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   102873 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tdcpg/v20211118/models.py
+-rw-r--r--   0 root         (0) root         (0)     6249 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tdcpg/v20211118/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    24877 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tdcpg/v20211118/tdcpg_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdwch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdwch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdwch/v20200915/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdwch/v20200915/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   158461 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdwch/v20200915/models.py
+-rw-r--r--   0 root         (0) root         (0)      703 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdwch/v20200915/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    24533 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdwch/v20200915/cdwch_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudstudio/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudstudio/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudstudio/v20210524/
+-rw-r--r--   0 root         (0) root         (0)    21897 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudstudio/v20210524/cloudstudio_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudstudio/v20210524/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   112109 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudstudio/v20210524/models.py
+-rw-r--r--   0 root         (0) root         (0)      828 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudstudio/v20210524/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudstudio/v20230508/
+-rw-r--r--   0 root         (0) root         (0)     8992 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudstudio/v20230508/cloudstudio_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudstudio/v20230508/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    33829 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudstudio/v20230508/models.py
+-rw-r--r--   0 root         (0) root         (0)      979 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudstudio/v20230508/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/msp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/msp/v20180319/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/msp/v20180319/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    30960 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/msp/v20180319/models.py
+-rw-r--r--   0 root         (0) root         (0)     7386 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/msp/v20180319/msp_client.py
+-rw-r--r--   0 root         (0) root         (0)      791 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/msp/v20180319/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/msp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/memcached/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/memcached/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/memcached/v20190318/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/memcached/v20190318/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    16280 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/memcached/v20190318/models.py
+-rw-r--r--   0 root         (0) root         (0)     1378 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/memcached/v20190318/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     1906 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/memcached/v20190318/memcached_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bpaas/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bpaas/v20181217/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bpaas/v20181217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    27503 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bpaas/v20181217/models.py
+-rw-r--r--   0 root         (0) root         (0)     1297 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bpaas/v20181217/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     2832 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bpaas/v20181217/bpaas_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bpaas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbm/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbm/v20180129/
+-rw-r--r--   0 root         (0) root         (0)    10459 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbm/v20180129/tbm_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbm/v20180129/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    53389 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbm/v20180129/models.py
+-rw-r--r--   0 root         (0) root         (0)     1235 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbm/v20180129/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trro/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trro/v20220325/
+-rw-r--r--   0 root         (0) root         (0)    21373 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trro/v20220325/trro_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trro/v20220325/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   103053 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trro/v20220325/models.py
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trro/v20220325/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trro/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/smh/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/smh/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/smh/v20210712/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/smh/v20210712/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    55893 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/smh/v20210712/models.py
+-rw-r--r--   0 root         (0) root         (0)     9912 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/smh/v20210712/smh_client.py
+-rw-r--r--   0 root         (0) root         (0)     3851 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/smh/v20210712/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/kms/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/kms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/kms/v20190118/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/kms/v20190118/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   156339 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/kms/v20190118/models.py
+-rw-r--r--   0 root         (0) root         (0)     5342 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/kms/v20190118/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    51055 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/kms/v20190118/kms_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/habo/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/habo/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/habo/v20181203/
+-rw-r--r--   0 root         (0) root         (0)     2800 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/habo/v20181203/habo_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/habo/v20181203/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6216 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/habo/v20181203/models.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/habo/v20181203/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/omics/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/omics/v20221128/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/omics/v20221128/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    89719 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/omics/v20221128/models.py
+-rw-r--r--   0 root         (0) root         (0)     4545 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/omics/v20221128/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    11346 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/omics/v20221128/omics_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/omics/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tkgdq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tkgdq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tkgdq/v20190411/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tkgdq/v20190411/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13153 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tkgdq/v20190411/models.py
+-rw-r--r--   0 root         (0) root         (0)     1685 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tkgdq/v20190411/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     4193 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tkgdq/v20190411/tkgdq_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eiam/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eiam/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eiam/v20210420/
+-rw-r--r--   0 root         (0) root         (0)    39100 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eiam/v20210420/eiam_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eiam/v20210420/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   218794 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eiam/v20210420/models.py
+-rw-r--r--   0 root         (0) root         (0)     9938 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eiam/v20210420/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rce/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rce/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rce/v20201103/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rce/v20201103/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    48344 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rce/v20201103/models.py
+-rw-r--r--   0 root         (0) root         (0)     4151 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rce/v20201103/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     4013 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rce/v20201103/rce_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/privatedns/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/privatedns/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/privatedns/v20201028/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/privatedns/v20201028/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    98914 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/privatedns/v20201028/models.py
+-rw-r--r--   0 root         (0) root         (0)    23057 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/privatedns/v20201028/privatedns_client.py
+-rw-r--r--   0 root         (0) root         (0)     7631 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/privatedns/v20201028/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tsf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tsf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tsf/v20180326/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tsf/v20180326/__init__.py
+-rw-r--r--   0 root         (0) root         (0)  1295816 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tsf/v20180326/models.py
+-rw-r--r--   0 root         (0) root         (0)    50530 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tsf/v20180326/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   197191 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tsf/v20180326/tsf_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iottid/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iottid/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iottid/v20190411/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iottid/v20190411/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    23421 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iottid/v20190411/models.py
+-rw-r--r--   0 root         (0) root         (0)     1707 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iottid/v20190411/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     9166 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iottid/v20190411/iottid_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dc/v20180410/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dc/v20180410/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   148313 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dc/v20180410/models.py
+-rw-r--r--   0 root         (0) root         (0)     2973 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dc/v20180410/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    21006 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dc/v20180410/dc_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/wav/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/wav/v20210129/
+-rw-r--r--   0 root         (0) root         (0)    26012 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/wav/v20210129/wav_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/wav/v20210129/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   229425 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/wav/v20210129/models.py
+-rw-r--r--   0 root         (0) root         (0)     1771 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/wav/v20210129/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/wav/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudaudit/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudaudit/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudaudit/v20190319/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudaudit/v20190319/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    90257 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudaudit/v20190319/models.py
+-rw-r--r--   0 root         (0) root         (0)    18578 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudaudit/v20190319/cloudaudit_client.py
+-rw-r--r--   0 root         (0) root         (0)     6753 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cloudaudit/v20190319/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rum/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rum/v20210622/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rum/v20210622/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   295365 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rum/v20210622/models.py
+-rw-r--r--   0 root         (0) root         (0)    60037 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rum/v20210622/rum_client.py
+-rw-r--r--   0 root         (0) root         (0)     2530 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rum/v20210622/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/rum/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tdmq/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tdmq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tdmq/v20200217/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tdmq/v20200217/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   641891 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tdmq/v20200217/models.py
+-rw-r--r--   0 root         (0) root         (0)    10126 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tdmq/v20200217/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   101215 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tdmq/v20200217/tdmq_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dnspod/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dnspod/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dnspod/v20210323/
+-rw-r--r--   0 root         (0) root         (0)    61922 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dnspod/v20210323/dnspod_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dnspod/v20210323/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   352399 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dnspod/v20210323/models.py
+-rw-r--r--   0 root         (0) root         (0)    24241 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dnspod/v20210323/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eis/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eis/v20200715/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eis/v20200715/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17929 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eis/v20200715/models.py
+-rw-r--r--   0 root         (0) root         (0)     3727 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eis/v20200715/eis_client.py
+-rw-r--r--   0 root         (0) root         (0)     1197 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eis/v20200715/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eis/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eis/v20210601/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eis/v20210601/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    41837 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eis/v20210601/models.py
+-rw-r--r--   0 root         (0) root         (0)     5866 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eis/v20210601/eis_client.py
+-rw-r--r--   0 root         (0) root         (0)     3329 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/eis/v20210601/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbp/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbp/v20190627/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbp/v20190627/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20731 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbp/v20190627/models.py
+-rw-r--r--   0 root         (0) root         (0)     1189 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbp/v20190627/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     2690 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbp/v20190627/tbp_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbp/v20190311/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbp/v20190311/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26651 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbp/v20190311/models.py
+-rw-r--r--   0 root         (0) root         (0)     1554 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbp/v20190311/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     4436 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tbp/v20190311/tbp_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/live/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/live/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/live/v20180801/
+-rw-r--r--   0 root         (0) root         (0)   157870 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/live/v20180801/live_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/live/v20180801/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   769438 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/live/v20180801/models.py
+-rw-r--r--   0 root         (0) root         (0)    20164 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/live/v20180801/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mall/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mall/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mall/v20230518/
+-rw-r--r--   0 root         (0) root         (0)     1941 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mall/v20230518/mall_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mall/v20230518/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8749 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mall/v20230518/models.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mall/v20230518/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cmq/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cmq/v20190304/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cmq/v20190304/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    98147 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cmq/v20190304/models.py
+-rw-r--r--   0 root         (0) root         (0)    15822 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cmq/v20190304/cmq_client.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cmq/v20190304/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cmq/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcb/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcb/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcb/v20180608/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcb/v20180608/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   553921 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcb/v20180608/models.py
+-rw-r--r--   0 root         (0) root         (0)     4156 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcb/v20180608/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    84257 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tcb/v20180608/tcb_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cws/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cws/v20180312/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cws/v20180312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    92049 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cws/v20180312/models.py
+-rw-r--r--   0 root         (0) root         (0)     1228 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cws/v20180312/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    18593 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cws/v20180312/cws_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cws/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/billing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/billing/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/billing/v20180709/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/billing/v20180709/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   342394 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/billing/v20180709/models.py
+-rw-r--r--   0 root         (0) root         (0)     2984 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/billing/v20180709/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    28340 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/billing/v20180709/billing_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tchd/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tchd/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tchd/v20230306/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tchd/v20230306/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     7653 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tchd/v20230306/models.py
+-rw-r--r--   0 root         (0) root         (0)      833 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tchd/v20230306/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     1986 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tchd/v20230306/tchd_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dtf/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dtf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dtf/v20200506/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dtf/v20200506/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    13921 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dtf/v20200506/models.py
+-rw-r--r--   0 root         (0) root         (0)      849 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dtf/v20200506/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     1887 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dtf/v20200506/dtf_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cfw/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cfw/v20190904/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cfw/v20190904/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   529438 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cfw/v20190904/models.py
+-rw-r--r--   0 root         (0) root         (0)     1836 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cfw/v20190904/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    96688 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cfw/v20190904/cfw_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cfw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/emr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/emr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/emr/v20190103/
+-rw-r--r--   0 root         (0) root         (0)    32872 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/emr/v20190103/emr_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/emr/v20190103/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   477110 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/emr/v20190103/models.py
+-rw-r--r--   0 root         (0) root         (0)    14890 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/emr/v20190103/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trocket/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trocket/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trocket/v20230308/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trocket/v20230308/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    96204 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trocket/v20230308/models.py
+-rw-r--r--   0 root         (0) root         (0)    18157 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trocket/v20230308/trocket_client.py
+-rw-r--r--   0 root         (0) root         (0)     1567 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trocket/v20230308/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sqlserver/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sqlserver/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sqlserver/v20180328/
+-rw-r--r--   0 root         (0) root         (0)   111899 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sqlserver/v20180328/sqlserver_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sqlserver/v20180328/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   586240 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sqlserver/v20180328/models.py
+-rw-r--r--   0 root         (0) root         (0)     9722 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sqlserver/v20180328/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mgobe/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mgobe/v20201014/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mgobe/v20201014/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    32095 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mgobe/v20201014/models.py
+-rw-r--r--   0 root         (0) root         (0)    34111 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mgobe/v20201014/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     8272 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mgobe/v20201014/mgobe_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mgobe/v20190929/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mgobe/v20190929/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2464 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mgobe/v20190929/models.py
+-rw-r--r--   0 root         (0) root         (0)    34005 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mgobe/v20190929/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     1859 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mgobe/v20190929/mgobe_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/mgobe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/essbasic/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/essbasic/v20201222/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/essbasic/v20201222/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   270905 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/essbasic/v20201222/models.py
+-rw-r--r--   0 root         (0) root         (0)     5392 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/essbasic/v20201222/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    54057 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/essbasic/v20201222/essbasic_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/essbasic/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/essbasic/v20210526/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/essbasic/v20210526/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   505344 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/essbasic/v20210526/models.py
+-rw-r--r--   0 root         (0) root         (0)    17658 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/essbasic/v20210526/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    78004 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/essbasic/v20210526/essbasic_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cms/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cms/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cms/v20190321/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cms/v20190321/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    97349 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cms/v20190321/models.py
+-rw-r--r--   0 root         (0) root         (0)     4152 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cms/v20190321/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     6597 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cms/v20190321/cms_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cwp/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cwp/v20180228/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cwp/v20180228/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   478685 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cwp/v20180228/cwp_client.py
+-rw-r--r--   0 root         (0) root         (0)  2448233 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cwp/v20180228/models.py
+-rw-r--r--   0 root         (0) root         (0)     4402 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cwp/v20180228/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cwp/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tione/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tione/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tione/v20191022/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tione/v20191022/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   144266 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tione/v20191022/models.py
+-rw-r--r--   0 root         (0) root         (0)     4465 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tione/v20191022/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    22102 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tione/v20191022/tione_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tione/v20211111/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tione/v20211111/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   649190 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tione/v20211111/models.py
+-rw-r--r--   0 root         (0) root         (0)    15712 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tione/v20211111/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    64588 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tione/v20211111/tione_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdn/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdn/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdn/v20180606/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdn/v20180606/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   854187 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdn/v20180606/models.py
+-rw-r--r--   0 root         (0) root         (0)    82459 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdn/v20180606/cdn_client.py
+-rw-r--r--   0 root         (0) root         (0)    22415 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cdn/v20180606/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ivld/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ivld/v20210903/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ivld/v20210903/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   158264 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ivld/v20210903/models.py
+-rw-r--r--   0 root         (0) root         (0)     9364 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ivld/v20210903/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    29555 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ivld/v20210903/ivld_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ivld/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/drm/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/drm/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/drm/v20181115/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/drm/v20181115/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    45281 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/drm/v20181115/models.py
+-rw-r--r--   0 root         (0) root         (0)     1093 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/drm/v20181115/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     9944 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/drm/v20181115/drm_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tiia/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tiia/v20190529/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tiia/v20190529/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   146178 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tiia/v20190529/models.py
+-rw-r--r--   0 root         (0) root         (0)    32719 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tiia/v20190529/tiia_client.py
+-rw-r--r--   0 root         (0) root         (0)     7539 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tiia/v20190529/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tiia/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ocr/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ocr/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ocr/v20181119/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ocr/v20181119/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   780644 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ocr/v20181119/models.py
+-rw-r--r--   0 root         (0) root         (0)     5927 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ocr/v20181119/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   110470 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/ocr/v20181119/ocr_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trtc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trtc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trtc/v20190722/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trtc/v20190722/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   306532 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trtc/v20190722/models.py
+-rw-r--r--   0 root         (0) root         (0)     9778 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trtc/v20190722/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    72465 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/trtc/v20190722/trtc_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotcloud/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotcloud/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotcloud/v20210408/
+-rw-r--r--   0 root         (0) root         (0)    67173 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotcloud/v20210408/iotcloud_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotcloud/v20210408/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   280299 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotcloud/v20210408/models.py
+-rw-r--r--   0 root         (0) root         (0)    12818 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotcloud/v20210408/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotcloud/v20180614/
+-rw-r--r--   0 root         (0) root         (0)    64562 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotcloud/v20180614/iotcloud_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotcloud/v20180614/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   281180 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotcloud/v20180614/models.py
+-rw-r--r--   0 root         (0) root         (0)    12668 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iotcloud/v20180614/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/soe/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/soe/v20180724/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/soe/v20180724/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    68696 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/soe/v20180724/models.py
+-rw-r--r--   0 root         (0) root         (0)     5919 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/soe/v20180724/soe_client.py
+-rw-r--r--   0 root         (0) root         (0)    14811 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/soe/v20180724/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/soe/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/aiart/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/aiart/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/aiart/v20221229/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/aiart/v20221229/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    17082 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/aiart/v20221229/models.py
+-rw-r--r--   0 root         (0) root         (0)     3806 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/aiart/v20221229/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     3676 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/aiart/v20221229/aiart_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yunsou/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yunsou/v20191115/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yunsou/v20191115/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    22913 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yunsou/v20191115/models.py
+-rw-r--r--   0 root         (0) root         (0)     1301 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yunsou/v20191115/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     2741 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yunsou/v20191115/yunsou_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yunsou/v20180504/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yunsou/v20180504/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12751 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yunsou/v20180504/models.py
+-rw-r--r--   0 root         (0) root         (0)      652 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yunsou/v20180504/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     2735 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yunsou/v20180504/yunsou_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/yunsou/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/apcas/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/apcas/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/apcas/v20201127/
+-rw-r--r--   0 root         (0) root         (0)     7214 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/apcas/v20201127/apcas_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/apcas/v20201127/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    35285 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/apcas/v20201127/models.py
+-rw-r--r--   0 root         (0) root         (0)     1430 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/apcas/v20201127/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bi/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bi/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bi/v20220105/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bi/v20220105/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   163392 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bi/v20220105/models.py
+-rw-r--r--   0 root         (0) root         (0)    19358 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bi/v20220105/bi_client.py
+-rw-r--r--   0 root         (0) root         (0)     2007 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/bi/v20220105/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tiw/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tiw/v20190919/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tiw/v20190919/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   284696 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tiw/v20190919/models.py
+-rw-r--r--   0 root         (0) root         (0)    61603 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tiw/v20190919/tiw_client.py
+-rw-r--r--   0 root         (0) root         (0)     6092 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tiw/v20190919/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/tiw/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dlc/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dlc/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dlc/v20210125/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dlc/v20210125/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   726055 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dlc/v20210125/models.py
+-rw-r--r--   0 root         (0) root         (0)    17887 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dlc/v20210125/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)   106851 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/dlc/v20210125/dlc_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iir/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iir/v20200417/
+-rw-r--r--   0 root         (0) root         (0)     2952 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iir/v20200417/iir_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iir/v20200417/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    12048 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iir/v20200417/models.py
+-rw-r--r--   0 root         (0) root         (0)     1737 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iir/v20200417/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/iir/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cls/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cls/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cls/v20201016/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cls/v20201016/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   543823 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cls/v20201016/models.py
+-rw-r--r--   0 root         (0) root         (0)     9633 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cls/v20201016/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)    87362 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/cls/v20201016/cls_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sts/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sts/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sts/v20180813/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sts/v20180813/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    28050 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sts/v20180813/models.py
+-rw-r--r--   0 root         (0) root         (0)     3086 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sts/v20180813/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     7324 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/sts/v20180813/sts_client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/batch/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/batch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/batch/v20170312/
+-rw-r--r--   0 root         (0) root         (0)    31661 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/batch/v20170312/batch_client.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/batch/v20170312/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   302061 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/batch/v20170312/models.py
+-rw-r--r--   0 root         (0) root         (0)     8635 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/batch/v20170312/errorcodes.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/pds/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/pds/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/pds/v20210701/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/pds/v20210701/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     8332 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/pds/v20210701/models.py
+-rw-r--r--   0 root         (0) root         (0)     1395 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/pds/v20210701/errorcodes.py
+-rw-r--r--   0 root         (0) root         (0)     2837 2023-10-16 00:08:02.000000 tencentcloud-sdk-python-3.0.999/tencentcloud/pds/v20210701/pds_client.py
+-rw-r--r--   0 root         (0) root         (0)       65 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1475 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      661 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/README.rst
+-rw-r--r--   0 root         (0) root         (0)       67 2023-10-16 00:17:37.000000 tencentcloud-sdk-python-3.0.999/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1186 2023-10-16 00:08:01.000000 tencentcloud-sdk-python-3.0.999/setup.py
```

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/tdsql.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/tdsql.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/scaling.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/scaling.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/live.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/live.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/ccr.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/ccr.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/redis.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/redis.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/tmt.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/tmt.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/bill.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/bill.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/dc.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/dc.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/yunsou.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/yunsou.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/sts.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/sts.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/bmeip.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/bmeip.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/emr.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/emr.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/wenzhi.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/wenzhi.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/bm.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/bm.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/trade.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/trade.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/cbs.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/cbs.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/scf.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/scf.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/dfw.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/dfw.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/sec.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/sec.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/cns.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/cns.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/image.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/image.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/eip.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/eip.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/ccs.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/ccs.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/feecenter.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/feecenter.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/cmem.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/cmem.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/athena.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/athena.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/cloudaudit.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/cloudaudit.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/bmvpc.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/bmvpc.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/vpc.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/vpc.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/tbaas.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/tbaas.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/vod.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/vod.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/apigateway.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/apigateway.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/lb.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/lb.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/market.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/market.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/bgpip.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/bgpip.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/partners.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/partners.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/monitor.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/monitor.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/bmlb.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/bmlb.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/snapshot.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/snapshot.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/cdn.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/cdn.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/account.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/account.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/batch.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/batch.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/base.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/base.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/cdb.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/cdb.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/modules/cvm.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/modules/cvm.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/common/api_exception.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/common/api_exception.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/common/sign.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/common/sign.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/common/request.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/common/request.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/QcloudApi/qcloudapi.py` & `tencentcloud-sdk-python-3.0.999/QcloudApi/qcloudapi.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud_sdk_python.egg-info/PKG-INFO` & `tencentcloud-sdk-python-3.0.999/tencentcloud_sdk_python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tencentcloud-sdk-python
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Maintainer-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud_sdk_python.egg-info/SOURCES.txt` & `tencentcloud-sdk-python-3.0.999/tencentcloud_sdk_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/LICENSE` & `tencentcloud-sdk-python-3.0.999/LICENSE`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/asr/v20190614/asr_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/asr/v20190614/asr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/asr/v20190614/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/asr/v20190614/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/asr/v20190614/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/asr/v20190614/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/oceanus/v20190422/oceanus_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/oceanus/v20190422/oceanus_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/oceanus/v20190422/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/oceanus/v20190422/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/oceanus/v20190422/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/oceanus/v20190422/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bma/v20221115/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bma/v20221115/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bma/v20221115/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bma/v20221115/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bma/v20221115/bma_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bma/v20221115/bma_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bma/v20210624/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bma/v20210624/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bma/v20210624/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bma/v20210624/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bma/v20210624/bma_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bma/v20210624/bma_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bm/v20180423/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bm/v20180423/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bm/v20180423/bm_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bm/v20180423/bm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bm/v20180423/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bm/v20180423/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/v20230321/thpc_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/v20230321/thpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/v20230321/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/v20230321/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/v20230321/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/v20230321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/v20220401/thpc_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/v20220401/thpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/v20220401/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/v20220401/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/v20220401/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/v20220401/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/v20211109/thpc_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/v20211109/thpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/v20211109/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/v20211109/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/thpc/v20211109/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/thpc/v20211109/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/market/v20191010/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/market/v20191010/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/market/v20191010/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/market/v20191010/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/market/v20191010/market_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/market/v20191010/market_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/antiddos/v20200309/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/antiddos/v20200309/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/antiddos/v20200309/antiddos_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/antiddos/v20200309/antiddos_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/antiddos/v20200309/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/antiddos/v20200309/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/vms/v20200902/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/vms/v20200902/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/vms/v20200902/vms_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/vms/v20200902/vms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/vms/v20200902/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/vms/v20200902/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cdc/v20201214/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cdc/v20201214/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cdc/v20201214/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cdc/v20201214/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cdc/v20201214/cdc_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cdc/v20201214/cdc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/asw/v20200722/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/asw/v20200722/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/asw/v20200722/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/asw/v20200722/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/asw/v20200722/asw_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/asw/v20200722/asw_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/pts/v20210728/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/pts/v20210728/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/pts/v20210728/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/pts/v20210728/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/pts/v20210728/pts_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/pts/v20210728/pts_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/wedata/v20210820/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/wedata/v20210820/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,14 +307,23 @@
         :type MessageId: str
         :param _Operator: 阈值计算算子，1 : 大于 2 ：小于
 注意：此字段可能返回 null，表示取不到有效值。
         :type Operator: int
         :param _RegularId: 告警规则ID
 注意：此字段可能返回 null，表示取不到有效值。
         :type RegularId: str
+        :param _AlarmRecipientName: 告警接收人昵称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AlarmRecipientName: str
+        :param _TaskType: 告警任务类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TaskType: int
+        :param _SendResult: 发送结果
+注意：此字段可能返回 null，表示取不到有效值。
+        :type SendResult: str
         """
         self._AlarmId = None
         self._AlarmTime = None
         self._TaskId = None
         self._RegularName = None
         self._AlarmLevel = None
         self._AlarmWay = None
@@ -326,14 +335,17 @@
         self._EstimatedTime = None
         self._InstanceId = None
         self._TaskName = None
         self._IsSendSuccess = None
         self._MessageId = None
         self._Operator = None
         self._RegularId = None
+        self._AlarmRecipientName = None
+        self._TaskType = None
+        self._SendResult = None
 
     @property
     def AlarmId(self):
         return self._AlarmId
 
     @AlarmId.setter
     def AlarmId(self, AlarmId):
@@ -471,14 +483,38 @@
     def RegularId(self):
         return self._RegularId
 
     @RegularId.setter
     def RegularId(self, RegularId):
         self._RegularId = RegularId
 
+    @property
+    def AlarmRecipientName(self):
+        return self._AlarmRecipientName
+
+    @AlarmRecipientName.setter
+    def AlarmRecipientName(self, AlarmRecipientName):
+        self._AlarmRecipientName = AlarmRecipientName
+
+    @property
+    def TaskType(self):
+        return self._TaskType
+
+    @TaskType.setter
+    def TaskType(self, TaskType):
+        self._TaskType = TaskType
+
+    @property
+    def SendResult(self):
+        return self._SendResult
+
+    @SendResult.setter
+    def SendResult(self, SendResult):
+        self._SendResult = SendResult
+
 
     def _deserialize(self, params):
         self._AlarmId = params.get("AlarmId")
         self._AlarmTime = params.get("AlarmTime")
         self._TaskId = params.get("TaskId")
         self._RegularName = params.get("RegularName")
         self._AlarmLevel = params.get("AlarmLevel")
@@ -491,14 +527,17 @@
         self._EstimatedTime = params.get("EstimatedTime")
         self._InstanceId = params.get("InstanceId")
         self._TaskName = params.get("TaskName")
         self._IsSendSuccess = params.get("IsSendSuccess")
         self._MessageId = params.get("MessageId")
         self._Operator = params.get("Operator")
         self._RegularId = params.get("RegularId")
+        self._AlarmRecipientName = params.get("AlarmRecipientName")
+        self._TaskType = params.get("TaskType")
+        self._SendResult = params.get("SendResult")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -7942,17 +7981,17 @@
 class CreateCustomFunctionRequest(AbstractModel):
     """CreateCustomFunction请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _Type: 类型：HIVE、SPARK
+        :param _Type: 枚举值：HIVE、SPARK、DLC
         :type Type: str
-        :param _Kind: 分类：窗口函数、聚合函数、日期函数......
+        :param _Kind: 枚举值：ANALYSIS(函数)、ENCRYPTION(加密函数)、AGGREGATE(聚合函数)、LOGIC(逻辑函数)、DATE_AND_TIME(日期与时间函数)、MATH(数学函数)、CONVERSION(转换函数)、STRING(字符串函数)、IP_AND_DOMAIN(IP和域名函数)、WINDOW(窗口函数)、OTHER(其他函数)
         :type Kind: str
         :param _Name: 函数名称
         :type Name: str
         :param _ClusterIdentifier: 集群实例引擎 ID
         :type ClusterIdentifier: str
         :param _DbName: 数据库名称
         :type DbName: str
@@ -8342,14 +8381,109 @@
 
 
     def _deserialize(self, params):
         self._Data = params.get("Data")
         self._RequestId = params.get("RequestId")
 
 
+class CreateDsFolderRequest(AbstractModel):
+    """CreateDsFolder请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ProjectId: 项目Id
+        :type ProjectId: str
+        :param _FolderName: 文件夹名称
+        :type FolderName: str
+        :param _ParentsFolderId: 父文件夹ID
+        :type ParentsFolderId: str
+        """
+        self._ProjectId = None
+        self._FolderName = None
+        self._ParentsFolderId = None
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def FolderName(self):
+        return self._FolderName
+
+    @FolderName.setter
+    def FolderName(self, FolderName):
+        self._FolderName = FolderName
+
+    @property
+    def ParentsFolderId(self):
+        return self._ParentsFolderId
+
+    @ParentsFolderId.setter
+    def ParentsFolderId(self, ParentsFolderId):
+        self._ParentsFolderId = ParentsFolderId
+
+
+    def _deserialize(self, params):
+        self._ProjectId = params.get("ProjectId")
+        self._FolderName = params.get("FolderName")
+        self._ParentsFolderId = params.get("ParentsFolderId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class CreateDsFolderResponse(AbstractModel):
+    """CreateDsFolder返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 文件夹Id，null则创建失败
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Data: str
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._Data = params.get("Data")
+        self._RequestId = params.get("RequestId")
+
+
 class CreateFolderRequest(AbstractModel):
     """CreateFolder请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -8852,15 +8986,15 @@
 
     def __init__(self):
         r"""
         :param _NodeInfo: 集成节点信息
         :type NodeInfo: :class:`tencentcloud.wedata.v20210820.models.IntegrationNodeInfo`
         :param _ProjectId: 项目id
         :type ProjectId: str
-        :param _TaskType: 任务类型
+        :param _TaskType: 任务类型，201为实时任务，202为离线任务
         :type TaskType: int
         """
         self._NodeInfo = None
         self._ProjectId = None
         self._TaskType = None
 
     @property
@@ -12301,14 +12435,96 @@
 
 
     def _deserialize(self, params):
         self._Data = params.get("Data")
         self._RequestId = params.get("RequestId")
 
 
+class DeleteDsFolderRequest(AbstractModel):
+    """DeleteDsFolder请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ProjectId: 项目Id
+        :type ProjectId: str
+        :param _FolderId: 文件夹ID
+        :type FolderId: str
+        """
+        self._ProjectId = None
+        self._FolderId = None
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def FolderId(self):
+        return self._FolderId
+
+    @FolderId.setter
+    def FolderId(self, FolderId):
+        self._FolderId = FolderId
+
+
+    def _deserialize(self, params):
+        self._ProjectId = params.get("ProjectId")
+        self._FolderId = params.get("FolderId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DeleteDsFolderResponse(AbstractModel):
+    """DeleteDsFolder返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: true代表删除成功，false代表删除失败
+        :type Data: bool
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._Data = params.get("Data")
+        self._RequestId = params.get("RequestId")
+
+
 class DeleteFilePathRequest(AbstractModel):
     """DeleteFilePath请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -18500,14 +18716,272 @@
             for item in params.get("Data"):
                 obj = DrInstanceOpsDto()
                 obj._deserialize(item)
                 self._Data.append(obj)
         self._RequestId = params.get("RequestId")
 
 
+class DescribeDsFolderTreeRequest(AbstractModel):
+    """DescribeDsFolderTree请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ProjectId: 项目id
+        :type ProjectId: str
+        :param _FirstLevelPull: 是否一级拉取
+        :type FirstLevelPull: bool
+        :param _FolderId: 文件夹ID
+        :type FolderId: str
+        :param _WorkflowId: 工作流ID
+        :type WorkflowId: str
+        :param _Keyword: 关键字搜索
+        :type Keyword: str
+        :param _IncludeWorkflow: 是否包含工作流
+        :type IncludeWorkflow: bool
+        :param _IncludeTask: 是否包含任务
+        :type IncludeTask: bool
+        """
+        self._ProjectId = None
+        self._FirstLevelPull = None
+        self._FolderId = None
+        self._WorkflowId = None
+        self._Keyword = None
+        self._IncludeWorkflow = None
+        self._IncludeTask = None
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def FirstLevelPull(self):
+        return self._FirstLevelPull
+
+    @FirstLevelPull.setter
+    def FirstLevelPull(self, FirstLevelPull):
+        self._FirstLevelPull = FirstLevelPull
+
+    @property
+    def FolderId(self):
+        return self._FolderId
+
+    @FolderId.setter
+    def FolderId(self, FolderId):
+        self._FolderId = FolderId
+
+    @property
+    def WorkflowId(self):
+        return self._WorkflowId
+
+    @WorkflowId.setter
+    def WorkflowId(self, WorkflowId):
+        self._WorkflowId = WorkflowId
+
+    @property
+    def Keyword(self):
+        return self._Keyword
+
+    @Keyword.setter
+    def Keyword(self, Keyword):
+        self._Keyword = Keyword
+
+    @property
+    def IncludeWorkflow(self):
+        return self._IncludeWorkflow
+
+    @IncludeWorkflow.setter
+    def IncludeWorkflow(self, IncludeWorkflow):
+        self._IncludeWorkflow = IncludeWorkflow
+
+    @property
+    def IncludeTask(self):
+        return self._IncludeTask
+
+    @IncludeTask.setter
+    def IncludeTask(self, IncludeTask):
+        self._IncludeTask = IncludeTask
+
+
+    def _deserialize(self, params):
+        self._ProjectId = params.get("ProjectId")
+        self._FirstLevelPull = params.get("FirstLevelPull")
+        self._FolderId = params.get("FolderId")
+        self._WorkflowId = params.get("WorkflowId")
+        self._Keyword = params.get("Keyword")
+        self._IncludeWorkflow = params.get("IncludeWorkflow")
+        self._IncludeTask = params.get("IncludeTask")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeDsFolderTreeResponse(AbstractModel):
+    """DescribeDsFolderTree返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 统一树结构返回属性列表
+        :type Data: list of PathNodeDsVO
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = []
+            for item in params.get("Data"):
+                obj = PathNodeDsVO()
+                obj._deserialize(item)
+                self._Data.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
+class DescribeDsParentFolderTreeRequest(AbstractModel):
+    """DescribeDsParentFolderTree请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ProjectId: 项目id
+        :type ProjectId: str
+        :param _FolderId: 文件夹ID
+        :type FolderId: str
+        :param _WorkflowId: 工作流ID
+        :type WorkflowId: str
+        :param _TaskId: 任务id
+        :type TaskId: str
+        """
+        self._ProjectId = None
+        self._FolderId = None
+        self._WorkflowId = None
+        self._TaskId = None
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def FolderId(self):
+        return self._FolderId
+
+    @FolderId.setter
+    def FolderId(self, FolderId):
+        self._FolderId = FolderId
+
+    @property
+    def WorkflowId(self):
+        return self._WorkflowId
+
+    @WorkflowId.setter
+    def WorkflowId(self, WorkflowId):
+        self._WorkflowId = WorkflowId
+
+    @property
+    def TaskId(self):
+        return self._TaskId
+
+    @TaskId.setter
+    def TaskId(self, TaskId):
+        self._TaskId = TaskId
+
+
+    def _deserialize(self, params):
+        self._ProjectId = params.get("ProjectId")
+        self._FolderId = params.get("FolderId")
+        self._WorkflowId = params.get("WorkflowId")
+        self._TaskId = params.get("TaskId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeDsParentFolderTreeResponse(AbstractModel):
+    """DescribeDsParentFolderTree返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 统一树结构返回属性列表
+        :type Data: list of PathNodeDsVO
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = []
+            for item in params.get("Data"):
+                obj = PathNodeDsVO()
+                obj._deserialize(item)
+                self._Data.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeEventCasesRequest(AbstractModel):
     """DescribeEventCases请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -24046,14 +24520,16 @@
         :type SourceServiceType: str
         :param _TargetServiceId: （仅针对离线同步任务）目标数据源id
         :type TargetServiceId: str
         :param _TargetServiceType: （仅针对离线同步任务）目标数据源类型
         :type TargetServiceType: str
         :param _AlarmType: 告警类型，多个类型以逗号分隔
         :type AlarmType: str
+        :param _ExecutorGroupIdList: 资源组id,多个资源组id之间以英文字符逗号分隔
+        :type ExecutorGroupIdList: str
         """
         self._ProjectId = None
         self._FolderIdList = None
         self._WorkFlowIdList = None
         self._WorkFlowNameList = None
         self._TaskNameList = None
         self._TaskIdList = None
@@ -24067,14 +24543,15 @@
         self._TaskCycleUnitList = None
         self._ProductNameList = None
         self._SourceServiceId = None
         self._SourceServiceType = None
         self._TargetServiceId = None
         self._TargetServiceType = None
         self._AlarmType = None
+        self._ExecutorGroupIdList = None
 
     @property
     def ProjectId(self):
         return self._ProjectId
 
     @ProjectId.setter
     def ProjectId(self, ProjectId):
@@ -24228,14 +24705,22 @@
     def AlarmType(self):
         return self._AlarmType
 
     @AlarmType.setter
     def AlarmType(self, AlarmType):
         self._AlarmType = AlarmType
 
+    @property
+    def ExecutorGroupIdList(self):
+        return self._ExecutorGroupIdList
+
+    @ExecutorGroupIdList.setter
+    def ExecutorGroupIdList(self, ExecutorGroupIdList):
+        self._ExecutorGroupIdList = ExecutorGroupIdList
+
 
     def _deserialize(self, params):
         self._ProjectId = params.get("ProjectId")
         self._FolderIdList = params.get("FolderIdList")
         self._WorkFlowIdList = params.get("WorkFlowIdList")
         self._WorkFlowNameList = params.get("WorkFlowNameList")
         self._TaskNameList = params.get("TaskNameList")
@@ -24250,14 +24735,15 @@
         self._TaskCycleUnitList = params.get("TaskCycleUnitList")
         self._ProductNameList = params.get("ProductNameList")
         self._SourceServiceId = params.get("SourceServiceId")
         self._SourceServiceType = params.get("SourceServiceType")
         self._TargetServiceId = params.get("TargetServiceId")
         self._TargetServiceType = params.get("TargetServiceType")
         self._AlarmType = params.get("AlarmType")
+        self._ExecutorGroupIdList = params.get("ExecutorGroupIdList")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -26043,17 +26529,17 @@
 class DescribeRealTimeTaskMetricOverviewRequest(AbstractModel):
     """DescribeRealTimeTaskMetricOverview请求参数结构体
 
     """
 
     def __init__(self):
         r"""
-        :param _TaskId: 要查看的实时任务的任务Id
+        :param _TaskId: 要查看的实时任务的任务ID，可在任务列表页面中获得
         :type TaskId: str
-        :param _ProjectId: 无
+        :param _ProjectId: 要查看的项目ID
         :type ProjectId: str
         :param _StartTime: 开始时间
         :type StartTime: int
         :param _EndTime: 结束时间
         :type EndTime: int
         """
         self._TaskId = None
@@ -30516,24 +31002,27 @@
         :type Container: str
         :param _Limit: 条数
         :type Limit: int
         :param _OrderType: 排序类型 desc asc
         :type OrderType: str
         :param _RunningOrderId: 作业运行的实例ID
         :type RunningOrderId: int
+        :param _Keyword: 关键字
+        :type Keyword: str
         """
         self._ProjectId = None
         self._TaskId = None
         self._JobId = None
         self._EndTime = None
         self._StartTime = None
         self._Container = None
         self._Limit = None
         self._OrderType = None
         self._RunningOrderId = None
+        self._Keyword = None
 
     @property
     def ProjectId(self):
         return self._ProjectId
 
     @ProjectId.setter
     def ProjectId(self, ProjectId):
@@ -30599,25 +31088,34 @@
     def RunningOrderId(self):
         return self._RunningOrderId
 
     @RunningOrderId.setter
     def RunningOrderId(self, RunningOrderId):
         self._RunningOrderId = RunningOrderId
 
+    @property
+    def Keyword(self):
+        return self._Keyword
+
+    @Keyword.setter
+    def Keyword(self, Keyword):
+        self._Keyword = Keyword
+
 
     def _deserialize(self, params):
         self._ProjectId = params.get("ProjectId")
         self._TaskId = params.get("TaskId")
         self._JobId = params.get("JobId")
         self._EndTime = params.get("EndTime")
         self._StartTime = params.get("StartTime")
         self._Container = params.get("Container")
         self._Limit = params.get("Limit")
         self._OrderType = params.get("OrderType")
         self._RunningOrderId = params.get("RunningOrderId")
+        self._Keyword = params.get("Keyword")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -37451,14 +37949,90 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class FindAllFolderRequest(AbstractModel):
+    """FindAllFolder请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ProjectId: 项目ID
+        :type ProjectId: str
+        """
+        self._ProjectId = None
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+
+    def _deserialize(self, params):
+        self._ProjectId = params.get("ProjectId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class FindAllFolderResponse(AbstractModel):
+    """FindAllFolder返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _FolderList: 文件夹列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FolderList: list of FolderDsDto
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._FolderList = None
+        self._RequestId = None
+
+    @property
+    def FolderList(self):
+        return self._FolderList
+
+    @FolderList.setter
+    def FolderList(self, FolderList):
+        self._FolderList = FolderList
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("FolderList") is not None:
+            self._FolderList = []
+            for item in params.get("FolderList"):
+                obj = FolderDsDto()
+                obj._deserialize(item)
+                self._FolderList.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
 class Folder(AbstractModel):
     """文件夹信息
 
     """
 
     def __init__(self):
         r"""
@@ -37532,14 +38106,188 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class FolderDsDto(AbstractModel):
+    """文件夹属性
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Id: 文件夹id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Id: str
+        :param _CreateTime: 创建时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CreateTime: str
+        :param _Name: 文件夹名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Name: str
+        :param _ProjectId: 所属项目id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ProjectId: str
+        :param _UpdateTime: 更新时间
+注意：此字段可能返回 null，表示取不到有效值。
+        :type UpdateTime: str
+        :param _ParentsFolderId: 父文件夹id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ParentsFolderId: str
+        :param _Total: 工作流总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Total: int
+        :param _Workflows: 工作流列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Workflows: list of WorkflowCanvasOpsDto
+        :param _TotalFolders: 子文件夹总数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type TotalFolders: int
+        :param _Folders: 子文件夹列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Folders: list of FolderDsDto
+        :param _FindType: 搜索类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type FindType: str
+        """
+        self._Id = None
+        self._CreateTime = None
+        self._Name = None
+        self._ProjectId = None
+        self._UpdateTime = None
+        self._ParentsFolderId = None
+        self._Total = None
+        self._Workflows = None
+        self._TotalFolders = None
+        self._Folders = None
+        self._FindType = None
+
+    @property
+    def Id(self):
+        return self._Id
+
+    @Id.setter
+    def Id(self, Id):
+        self._Id = Id
+
+    @property
+    def CreateTime(self):
+        return self._CreateTime
+
+    @CreateTime.setter
+    def CreateTime(self, CreateTime):
+        self._CreateTime = CreateTime
+
+    @property
+    def Name(self):
+        return self._Name
+
+    @Name.setter
+    def Name(self, Name):
+        self._Name = Name
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def UpdateTime(self):
+        return self._UpdateTime
+
+    @UpdateTime.setter
+    def UpdateTime(self, UpdateTime):
+        self._UpdateTime = UpdateTime
+
+    @property
+    def ParentsFolderId(self):
+        return self._ParentsFolderId
+
+    @ParentsFolderId.setter
+    def ParentsFolderId(self, ParentsFolderId):
+        self._ParentsFolderId = ParentsFolderId
+
+    @property
+    def Total(self):
+        return self._Total
+
+    @Total.setter
+    def Total(self, Total):
+        self._Total = Total
+
+    @property
+    def Workflows(self):
+        return self._Workflows
+
+    @Workflows.setter
+    def Workflows(self, Workflows):
+        self._Workflows = Workflows
+
+    @property
+    def TotalFolders(self):
+        return self._TotalFolders
+
+    @TotalFolders.setter
+    def TotalFolders(self, TotalFolders):
+        self._TotalFolders = TotalFolders
+
+    @property
+    def Folders(self):
+        return self._Folders
+
+    @Folders.setter
+    def Folders(self, Folders):
+        self._Folders = Folders
+
+    @property
+    def FindType(self):
+        return self._FindType
+
+    @FindType.setter
+    def FindType(self, FindType):
+        self._FindType = FindType
+
+
+    def _deserialize(self, params):
+        self._Id = params.get("Id")
+        self._CreateTime = params.get("CreateTime")
+        self._Name = params.get("Name")
+        self._ProjectId = params.get("ProjectId")
+        self._UpdateTime = params.get("UpdateTime")
+        self._ParentsFolderId = params.get("ParentsFolderId")
+        self._Total = params.get("Total")
+        if params.get("Workflows") is not None:
+            self._Workflows = []
+            for item in params.get("Workflows"):
+                obj = WorkflowCanvasOpsDto()
+                obj._deserialize(item)
+                self._Workflows.append(obj)
+        self._TotalFolders = params.get("TotalFolders")
+        if params.get("Folders") is not None:
+            self._Folders = []
+            for item in params.get("Folders"):
+                obj = FolderDsDto()
+                obj._deserialize(item)
+                self._Folders.append(obj)
+        self._FindType = params.get("FindType")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class FolderOpsDto(AbstractModel):
     """文件夹属性
 
     """
 
     def __init__(self):
         r"""
@@ -39445,14 +40193,20 @@
         :type CvmAgentStatusList: list of CvmAgentStatus
         :param _AgentTotal: agent数量
 注意：此字段可能返回 null，表示取不到有效值。
         :type AgentTotal: int
         :param _LifeDays: 生命周期
 注意：此字段可能返回 null，表示取不到有效值。
         :type LifeDays: int
+        :param _ClusterId: 集群ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ClusterId: str
+        :param _AgentRegion: agent地域
+注意：此字段可能返回 null，表示取不到有效值。
+        :type AgentRegion: str
         """
         self._AgentId = None
         self._AgentName = None
         self._Status = None
         self._StatusDesc = None
         self._AgentType = None
         self._Source = None
@@ -39460,14 +40214,16 @@
         self._ExecutorGroupId = None
         self._ExecutorGroupName = None
         self._TaskCount = None
         self._AgentGroupId = None
         self._CvmAgentStatusList = None
         self._AgentTotal = None
         self._LifeDays = None
+        self._ClusterId = None
+        self._AgentRegion = None
 
     @property
     def AgentId(self):
         return self._AgentId
 
     @AgentId.setter
     def AgentId(self, AgentId):
@@ -39573,14 +40329,30 @@
     def LifeDays(self):
         return self._LifeDays
 
     @LifeDays.setter
     def LifeDays(self, LifeDays):
         self._LifeDays = LifeDays
 
+    @property
+    def ClusterId(self):
+        return self._ClusterId
+
+    @ClusterId.setter
+    def ClusterId(self, ClusterId):
+        self._ClusterId = ClusterId
+
+    @property
+    def AgentRegion(self):
+        return self._AgentRegion
+
+    @AgentRegion.setter
+    def AgentRegion(self, AgentRegion):
+        self._AgentRegion = AgentRegion
+
 
     def _deserialize(self, params):
         self._AgentId = params.get("AgentId")
         self._AgentName = params.get("AgentName")
         self._Status = params.get("Status")
         self._StatusDesc = params.get("StatusDesc")
         self._AgentType = params.get("AgentType")
@@ -39594,14 +40366,16 @@
             self._CvmAgentStatusList = []
             for item in params.get("CvmAgentStatusList"):
                 obj = CvmAgentStatus()
                 obj._deserialize(item)
                 self._CvmAgentStatusList.append(obj)
         self._AgentTotal = params.get("AgentTotal")
         self._LifeDays = params.get("LifeDays")
+        self._ClusterId = params.get("ClusterId")
+        self._AgentRegion = params.get("AgentRegion")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -39846,14 +40620,16 @@
         :type DagDependent: str
         :param _DagDepth: dag深度 默认为1，取值 1-6
         :type DagDepth: int
         :param _TenantId: 租户id
         :type TenantId: str
         :param _DataTimeCycle: 根据当前数据时间或者是下一个数据时间查询, 默认当前数据时间
         :type DataTimeCycle: str
+        :param _ExecutorGroupIdList: 资源组id,多个资源组id用英文逗号分隔
+        :type ExecutorGroupIdList: list of str
         """
         self._Instance = None
         self._SortCol = None
         self._TaskIdList = None
         self._TaskNameList = None
         self._FolderList = None
         self._Sort = None
@@ -39877,14 +40653,15 @@
         self._InstanceType = None
         self._DagDeal = None
         self._DagType = None
         self._DagDependent = None
         self._DagDepth = None
         self._TenantId = None
         self._DataTimeCycle = None
+        self._ExecutorGroupIdList = None
 
     @property
     def Instance(self):
         return self._Instance
 
     @Instance.setter
     def Instance(self, Instance):
@@ -40118,14 +40895,22 @@
     def DataTimeCycle(self):
         return self._DataTimeCycle
 
     @DataTimeCycle.setter
     def DataTimeCycle(self, DataTimeCycle):
         self._DataTimeCycle = DataTimeCycle
 
+    @property
+    def ExecutorGroupIdList(self):
+        return self._ExecutorGroupIdList
+
+    @ExecutorGroupIdList.setter
+    def ExecutorGroupIdList(self, ExecutorGroupIdList):
+        self._ExecutorGroupIdList = ExecutorGroupIdList
+
 
     def _deserialize(self, params):
         if params.get("Instance") is not None:
             self._Instance = InstanceOpsDto()
             self._Instance._deserialize(params.get("Instance"))
         self._SortCol = params.get("SortCol")
         self._TaskIdList = params.get("TaskIdList")
@@ -40157,14 +40942,15 @@
         self._InstanceType = params.get("InstanceType")
         self._DagDeal = params.get("DagDeal")
         self._DagType = params.get("DagType")
         self._DagDependent = params.get("DagDependent")
         self._DagDepth = params.get("DagDepth")
         self._TenantId = params.get("TenantId")
         self._DataTimeCycle = params.get("DataTimeCycle")
+        self._ExecutorGroupIdList = params.get("ExecutorGroupIdList")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -41262,14 +42048,20 @@
         :type ProjectName: str
         :param _TenantId: 租户id
 注意：此字段可能返回 null，表示取不到有效值。
         :type TenantId: str
         :param _InstanceKey: 实例标识
 注意：此字段可能返回 null，表示取不到有效值。
         :type InstanceKey: str
+        :param _ExecutorGroupId: 资源组id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecutorGroupId: str
+        :param _ExecutorGroupName: 资源组名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecutorGroupName: str
         """
         self._TaskId = None
         self._TaskName = None
         self._WorkflowId = None
         self._WorkflowName = None
         self._InCharge = None
         self._CycleType = None
@@ -41315,14 +42107,16 @@
         self._FirstSubmitTime = None
         self._FirstRunTime = None
         self._ProjectId = None
         self._ProjectIdent = None
         self._ProjectName = None
         self._TenantId = None
         self._InstanceKey = None
+        self._ExecutorGroupId = None
+        self._ExecutorGroupName = None
 
     @property
     def TaskId(self):
         return self._TaskId
 
     @TaskId.setter
     def TaskId(self, TaskId):
@@ -41732,14 +42526,30 @@
     def InstanceKey(self):
         return self._InstanceKey
 
     @InstanceKey.setter
     def InstanceKey(self, InstanceKey):
         self._InstanceKey = InstanceKey
 
+    @property
+    def ExecutorGroupId(self):
+        return self._ExecutorGroupId
+
+    @ExecutorGroupId.setter
+    def ExecutorGroupId(self, ExecutorGroupId):
+        self._ExecutorGroupId = ExecutorGroupId
+
+    @property
+    def ExecutorGroupName(self):
+        return self._ExecutorGroupName
+
+    @ExecutorGroupName.setter
+    def ExecutorGroupName(self, ExecutorGroupName):
+        self._ExecutorGroupName = ExecutorGroupName
+
 
     def _deserialize(self, params):
         self._TaskId = params.get("TaskId")
         self._TaskName = params.get("TaskName")
         self._WorkflowId = params.get("WorkflowId")
         self._WorkflowName = params.get("WorkflowName")
         self._InCharge = params.get("InCharge")
@@ -41788,14 +42598,16 @@
         self._FirstSubmitTime = params.get("FirstSubmitTime")
         self._FirstRunTime = params.get("FirstRunTime")
         self._ProjectId = params.get("ProjectId")
         self._ProjectIdent = params.get("ProjectIdent")
         self._ProjectName = params.get("ProjectName")
         self._TenantId = params.get("TenantId")
         self._InstanceKey = params.get("InstanceKey")
+        self._ExecutorGroupId = params.get("ExecutorGroupId")
+        self._ExecutorGroupName = params.get("ExecutorGroupName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -46727,14 +47539,120 @@
 
 
     def _deserialize(self, params):
         self._Data = params.get("Data")
         self._RequestId = params.get("RequestId")
 
 
+class ModifyDsFolderRequest(AbstractModel):
+    """ModifyDsFolder请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ProjectId: 项目Id
+        :type ProjectId: str
+        :param _FolderName: 文件夹名称
+        :type FolderName: str
+        :param _FolderId: 文件夹Id
+        :type FolderId: str
+        :param _ParentsFolderId: 父文件夹ID
+        :type ParentsFolderId: str
+        """
+        self._ProjectId = None
+        self._FolderName = None
+        self._FolderId = None
+        self._ParentsFolderId = None
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def FolderName(self):
+        return self._FolderName
+
+    @FolderName.setter
+    def FolderName(self, FolderName):
+        self._FolderName = FolderName
+
+    @property
+    def FolderId(self):
+        return self._FolderId
+
+    @FolderId.setter
+    def FolderId(self, FolderId):
+        self._FolderId = FolderId
+
+    @property
+    def ParentsFolderId(self):
+        return self._ParentsFolderId
+
+    @ParentsFolderId.setter
+    def ParentsFolderId(self, ParentsFolderId):
+        self._ParentsFolderId = ParentsFolderId
+
+
+    def _deserialize(self, params):
+        self._ProjectId = params.get("ProjectId")
+        self._FolderName = params.get("FolderName")
+        self._FolderId = params.get("FolderId")
+        self._ParentsFolderId = params.get("ParentsFolderId")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class ModifyDsFolderResponse(AbstractModel):
+    """ModifyDsFolder返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: true代表成功，false代表失败
+        :type Data: bool
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._Data = params.get("Data")
+        self._RequestId = params.get("RequestId")
+
+
 class ModifyExecStrategyRequest(AbstractModel):
     """ModifyExecStrategy请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -51252,14 +52170,131 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class PathNodeDsVO(AbstractModel):
+    """数据开发-统一树结构返回属性
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Id: PathNode ID
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Id: str
+        :param _Title: PathNode 名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Title: str
+        :param _Type: PathNode 类型
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Type: str
+        :param _ParentId: 父节点唯一标识
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ParentId: str
+        :param _IsLeaf: 是否叶子节点
+注意：此字段可能返回 null，表示取不到有效值。
+        :type IsLeaf: bool
+        :param _Children: 子节点列表
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Children: list of PathNodeDsVO
+        :param _Params: 业务参数 ,base64编译的json串，获取具体参数需要base64反编译
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Params: str
+        """
+        self._Id = None
+        self._Title = None
+        self._Type = None
+        self._ParentId = None
+        self._IsLeaf = None
+        self._Children = None
+        self._Params = None
+
+    @property
+    def Id(self):
+        return self._Id
+
+    @Id.setter
+    def Id(self, Id):
+        self._Id = Id
+
+    @property
+    def Title(self):
+        return self._Title
+
+    @Title.setter
+    def Title(self, Title):
+        self._Title = Title
+
+    @property
+    def Type(self):
+        return self._Type
+
+    @Type.setter
+    def Type(self, Type):
+        self._Type = Type
+
+    @property
+    def ParentId(self):
+        return self._ParentId
+
+    @ParentId.setter
+    def ParentId(self, ParentId):
+        self._ParentId = ParentId
+
+    @property
+    def IsLeaf(self):
+        return self._IsLeaf
+
+    @IsLeaf.setter
+    def IsLeaf(self, IsLeaf):
+        self._IsLeaf = IsLeaf
+
+    @property
+    def Children(self):
+        return self._Children
+
+    @Children.setter
+    def Children(self, Children):
+        self._Children = Children
+
+    @property
+    def Params(self):
+        return self._Params
+
+    @Params.setter
+    def Params(self, Params):
+        self._Params = Params
+
+
+    def _deserialize(self, params):
+        self._Id = params.get("Id")
+        self._Title = params.get("Title")
+        self._Type = params.get("Type")
+        self._ParentId = params.get("ParentId")
+        self._IsLeaf = params.get("IsLeaf")
+        if params.get("Children") is not None:
+            self._Children = []
+            for item in params.get("Children"):
+                obj = PathNodeDsVO()
+                obj._deserialize(item)
+                self._Children.append(obj)
+        self._Params = params.get("Params")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class ProdSchedulerTask(AbstractModel):
     """数据质量生产调度任务业务实体
 
     """
 
     def __init__(self):
         r"""
@@ -56977,14 +58012,584 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class RunForceSucScheduleInstancesRequest(AbstractModel):
+    """RunForceSucScheduleInstances请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Instances: 实例列表
+        :type Instances: list of InstanceOpsDto
+        :param _CheckFather: 检查父任务类型, true: 检查父任务; false: 不检查父任务 
+        :type CheckFather: bool
+        :param _RerunType: 重跑类型, 1: 自身; 3: 孩子; 2: 自身以及孩子 
+        :type RerunType: str
+        :param _DependentWay: 实例依赖方式, 1: 自依赖; 2: 任务依赖; 3: 自依赖及父子依赖 
+        :type DependentWay: str
+        :param _SkipEventListening: 重跑忽略事件监听与否 
+        :type SkipEventListening: bool
+        :param _SonInstanceType: 下游实例范围 1: 所在工作流 2: 所在项目 3: 所有跨工作流依赖的项目
+        :type SonInstanceType: str
+        :param _SearchCondition: 查询条件
+        :type SearchCondition: :class:`tencentcloud.wedata.v20210820.models.InstanceApiOpsRequest`
+        :param _OptType: 访问类型
+        :type OptType: str
+        :param _OperatorName: 操作者名称
+        :type OperatorName: str
+        :param _OperatorId: 操作者id
+        :type OperatorId: str
+        :param _ProjectId: 项目id
+        :type ProjectId: str
+        :param _ProjectIdent: 项目标志
+        :type ProjectIdent: str
+        :param _ProjectName: 项目名称
+        :type ProjectName: str
+        :param _PageIndex: 索引页码
+        :type PageIndex: int
+        :param _PageSize: 页面大小
+        :type PageSize: int
+        :param _Count: 数据总数
+        :type Count: int
+        :param _RequestBaseInfo: 基础请求信息
+        :type RequestBaseInfo: :class:`tencentcloud.wedata.v20210820.models.ProjectBaseInfoOpsRequest`
+        :param _IsCount: 是否计算总数
+        :type IsCount: bool
+        """
+        self._Instances = None
+        self._CheckFather = None
+        self._RerunType = None
+        self._DependentWay = None
+        self._SkipEventListening = None
+        self._SonInstanceType = None
+        self._SearchCondition = None
+        self._OptType = None
+        self._OperatorName = None
+        self._OperatorId = None
+        self._ProjectId = None
+        self._ProjectIdent = None
+        self._ProjectName = None
+        self._PageIndex = None
+        self._PageSize = None
+        self._Count = None
+        self._RequestBaseInfo = None
+        self._IsCount = None
+
+    @property
+    def Instances(self):
+        return self._Instances
+
+    @Instances.setter
+    def Instances(self, Instances):
+        self._Instances = Instances
+
+    @property
+    def CheckFather(self):
+        return self._CheckFather
+
+    @CheckFather.setter
+    def CheckFather(self, CheckFather):
+        self._CheckFather = CheckFather
+
+    @property
+    def RerunType(self):
+        return self._RerunType
+
+    @RerunType.setter
+    def RerunType(self, RerunType):
+        self._RerunType = RerunType
+
+    @property
+    def DependentWay(self):
+        return self._DependentWay
+
+    @DependentWay.setter
+    def DependentWay(self, DependentWay):
+        self._DependentWay = DependentWay
+
+    @property
+    def SkipEventListening(self):
+        return self._SkipEventListening
+
+    @SkipEventListening.setter
+    def SkipEventListening(self, SkipEventListening):
+        self._SkipEventListening = SkipEventListening
+
+    @property
+    def SonInstanceType(self):
+        return self._SonInstanceType
+
+    @SonInstanceType.setter
+    def SonInstanceType(self, SonInstanceType):
+        self._SonInstanceType = SonInstanceType
+
+    @property
+    def SearchCondition(self):
+        return self._SearchCondition
+
+    @SearchCondition.setter
+    def SearchCondition(self, SearchCondition):
+        self._SearchCondition = SearchCondition
+
+    @property
+    def OptType(self):
+        return self._OptType
+
+    @OptType.setter
+    def OptType(self, OptType):
+        self._OptType = OptType
+
+    @property
+    def OperatorName(self):
+        return self._OperatorName
+
+    @OperatorName.setter
+    def OperatorName(self, OperatorName):
+        self._OperatorName = OperatorName
+
+    @property
+    def OperatorId(self):
+        return self._OperatorId
+
+    @OperatorId.setter
+    def OperatorId(self, OperatorId):
+        self._OperatorId = OperatorId
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def ProjectIdent(self):
+        return self._ProjectIdent
+
+    @ProjectIdent.setter
+    def ProjectIdent(self, ProjectIdent):
+        self._ProjectIdent = ProjectIdent
+
+    @property
+    def ProjectName(self):
+        return self._ProjectName
+
+    @ProjectName.setter
+    def ProjectName(self, ProjectName):
+        self._ProjectName = ProjectName
+
+    @property
+    def PageIndex(self):
+        return self._PageIndex
+
+    @PageIndex.setter
+    def PageIndex(self, PageIndex):
+        self._PageIndex = PageIndex
+
+    @property
+    def PageSize(self):
+        return self._PageSize
+
+    @PageSize.setter
+    def PageSize(self, PageSize):
+        self._PageSize = PageSize
+
+    @property
+    def Count(self):
+        return self._Count
+
+    @Count.setter
+    def Count(self, Count):
+        self._Count = Count
+
+    @property
+    def RequestBaseInfo(self):
+        return self._RequestBaseInfo
+
+    @RequestBaseInfo.setter
+    def RequestBaseInfo(self, RequestBaseInfo):
+        self._RequestBaseInfo = RequestBaseInfo
+
+    @property
+    def IsCount(self):
+        return self._IsCount
+
+    @IsCount.setter
+    def IsCount(self, IsCount):
+        self._IsCount = IsCount
+
+
+    def _deserialize(self, params):
+        if params.get("Instances") is not None:
+            self._Instances = []
+            for item in params.get("Instances"):
+                obj = InstanceOpsDto()
+                obj._deserialize(item)
+                self._Instances.append(obj)
+        self._CheckFather = params.get("CheckFather")
+        self._RerunType = params.get("RerunType")
+        self._DependentWay = params.get("DependentWay")
+        self._SkipEventListening = params.get("SkipEventListening")
+        self._SonInstanceType = params.get("SonInstanceType")
+        if params.get("SearchCondition") is not None:
+            self._SearchCondition = InstanceApiOpsRequest()
+            self._SearchCondition._deserialize(params.get("SearchCondition"))
+        self._OptType = params.get("OptType")
+        self._OperatorName = params.get("OperatorName")
+        self._OperatorId = params.get("OperatorId")
+        self._ProjectId = params.get("ProjectId")
+        self._ProjectIdent = params.get("ProjectIdent")
+        self._ProjectName = params.get("ProjectName")
+        self._PageIndex = params.get("PageIndex")
+        self._PageSize = params.get("PageSize")
+        self._Count = params.get("Count")
+        if params.get("RequestBaseInfo") is not None:
+            self._RequestBaseInfo = ProjectBaseInfoOpsRequest()
+            self._RequestBaseInfo._deserialize(params.get("RequestBaseInfo"))
+        self._IsCount = params.get("IsCount")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class RunForceSucScheduleInstancesResponse(AbstractModel):
+    """RunForceSucScheduleInstances返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 结果
+        :type Data: :class:`tencentcloud.wedata.v20210820.models.BatchOperateResultOpsDto`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = BatchOperateResultOpsDto()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
+
+
+class RunRerunScheduleInstancesRequest(AbstractModel):
+    """RunRerunScheduleInstances请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Instances: 实例列表
+        :type Instances: list of InstanceOpsDto
+        :param _CheckFather: 检查父任务类型, true: 检查父任务; false: 不检查父任务 
+        :type CheckFather: bool
+        :param _RerunType: 重跑类型, 1: 自身; 3: 孩子; 2: 自身以及孩子 
+        :type RerunType: str
+        :param _DependentWay: 实例依赖方式, 1: 自依赖; 2: 任务依赖; 3: 自依赖及父子依赖 
+        :type DependentWay: str
+        :param _SkipEventListening: 重跑忽略事件监听与否 
+        :type SkipEventListening: bool
+        :param _SonInstanceType: 下游实例范围 1: 所在工作流 2: 所在项目 3: 所有跨工作流依赖的项目
+        :type SonInstanceType: str
+        :param _SearchCondition: 查询条件
+        :type SearchCondition: :class:`tencentcloud.wedata.v20210820.models.InstanceApiOpsRequest`
+        :param _OptType: 访问类型
+        :type OptType: str
+        :param _OperatorName: 操作者名称
+        :type OperatorName: str
+        :param _OperatorId: 操作者id
+        :type OperatorId: str
+        :param _ProjectId: 项目id
+        :type ProjectId: str
+        :param _ProjectIdent: 项目标志
+        :type ProjectIdent: str
+        :param _ProjectName: 项目名称
+        :type ProjectName: str
+        :param _PageIndex: 索引页码
+        :type PageIndex: int
+        :param _PageSize: 页面大小
+        :type PageSize: int
+        :param _Count: 数据总数
+        :type Count: int
+        :param _RequestBaseInfo: 基础请求信息
+        :type RequestBaseInfo: :class:`tencentcloud.wedata.v20210820.models.ProjectBaseInfoOpsRequest`
+        :param _IsCount: 是否计算总数
+        :type IsCount: bool
+        """
+        self._Instances = None
+        self._CheckFather = None
+        self._RerunType = None
+        self._DependentWay = None
+        self._SkipEventListening = None
+        self._SonInstanceType = None
+        self._SearchCondition = None
+        self._OptType = None
+        self._OperatorName = None
+        self._OperatorId = None
+        self._ProjectId = None
+        self._ProjectIdent = None
+        self._ProjectName = None
+        self._PageIndex = None
+        self._PageSize = None
+        self._Count = None
+        self._RequestBaseInfo = None
+        self._IsCount = None
+
+    @property
+    def Instances(self):
+        return self._Instances
+
+    @Instances.setter
+    def Instances(self, Instances):
+        self._Instances = Instances
+
+    @property
+    def CheckFather(self):
+        return self._CheckFather
+
+    @CheckFather.setter
+    def CheckFather(self, CheckFather):
+        self._CheckFather = CheckFather
+
+    @property
+    def RerunType(self):
+        return self._RerunType
+
+    @RerunType.setter
+    def RerunType(self, RerunType):
+        self._RerunType = RerunType
+
+    @property
+    def DependentWay(self):
+        return self._DependentWay
+
+    @DependentWay.setter
+    def DependentWay(self, DependentWay):
+        self._DependentWay = DependentWay
+
+    @property
+    def SkipEventListening(self):
+        return self._SkipEventListening
+
+    @SkipEventListening.setter
+    def SkipEventListening(self, SkipEventListening):
+        self._SkipEventListening = SkipEventListening
+
+    @property
+    def SonInstanceType(self):
+        return self._SonInstanceType
+
+    @SonInstanceType.setter
+    def SonInstanceType(self, SonInstanceType):
+        self._SonInstanceType = SonInstanceType
+
+    @property
+    def SearchCondition(self):
+        return self._SearchCondition
+
+    @SearchCondition.setter
+    def SearchCondition(self, SearchCondition):
+        self._SearchCondition = SearchCondition
+
+    @property
+    def OptType(self):
+        return self._OptType
+
+    @OptType.setter
+    def OptType(self, OptType):
+        self._OptType = OptType
+
+    @property
+    def OperatorName(self):
+        return self._OperatorName
+
+    @OperatorName.setter
+    def OperatorName(self, OperatorName):
+        self._OperatorName = OperatorName
+
+    @property
+    def OperatorId(self):
+        return self._OperatorId
+
+    @OperatorId.setter
+    def OperatorId(self, OperatorId):
+        self._OperatorId = OperatorId
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def ProjectIdent(self):
+        return self._ProjectIdent
+
+    @ProjectIdent.setter
+    def ProjectIdent(self, ProjectIdent):
+        self._ProjectIdent = ProjectIdent
+
+    @property
+    def ProjectName(self):
+        return self._ProjectName
+
+    @ProjectName.setter
+    def ProjectName(self, ProjectName):
+        self._ProjectName = ProjectName
+
+    @property
+    def PageIndex(self):
+        return self._PageIndex
+
+    @PageIndex.setter
+    def PageIndex(self, PageIndex):
+        self._PageIndex = PageIndex
+
+    @property
+    def PageSize(self):
+        return self._PageSize
+
+    @PageSize.setter
+    def PageSize(self, PageSize):
+        self._PageSize = PageSize
+
+    @property
+    def Count(self):
+        return self._Count
+
+    @Count.setter
+    def Count(self, Count):
+        self._Count = Count
+
+    @property
+    def RequestBaseInfo(self):
+        return self._RequestBaseInfo
+
+    @RequestBaseInfo.setter
+    def RequestBaseInfo(self, RequestBaseInfo):
+        self._RequestBaseInfo = RequestBaseInfo
+
+    @property
+    def IsCount(self):
+        return self._IsCount
+
+    @IsCount.setter
+    def IsCount(self, IsCount):
+        self._IsCount = IsCount
+
+
+    def _deserialize(self, params):
+        if params.get("Instances") is not None:
+            self._Instances = []
+            for item in params.get("Instances"):
+                obj = InstanceOpsDto()
+                obj._deserialize(item)
+                self._Instances.append(obj)
+        self._CheckFather = params.get("CheckFather")
+        self._RerunType = params.get("RerunType")
+        self._DependentWay = params.get("DependentWay")
+        self._SkipEventListening = params.get("SkipEventListening")
+        self._SonInstanceType = params.get("SonInstanceType")
+        if params.get("SearchCondition") is not None:
+            self._SearchCondition = InstanceApiOpsRequest()
+            self._SearchCondition._deserialize(params.get("SearchCondition"))
+        self._OptType = params.get("OptType")
+        self._OperatorName = params.get("OperatorName")
+        self._OperatorId = params.get("OperatorId")
+        self._ProjectId = params.get("ProjectId")
+        self._ProjectIdent = params.get("ProjectIdent")
+        self._ProjectName = params.get("ProjectName")
+        self._PageIndex = params.get("PageIndex")
+        self._PageSize = params.get("PageSize")
+        self._Count = params.get("Count")
+        if params.get("RequestBaseInfo") is not None:
+            self._RequestBaseInfo = ProjectBaseInfoOpsRequest()
+            self._RequestBaseInfo._deserialize(params.get("RequestBaseInfo"))
+        self._IsCount = params.get("IsCount")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class RunRerunScheduleInstancesResponse(AbstractModel):
+    """RunRerunScheduleInstances返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Data: 结果
+        :type Data: :class:`tencentcloud.wedata.v20210820.models.BatchOperateResultOpsDto`
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._Data = None
+        self._RequestId = None
+
+    @property
+    def Data(self):
+        return self._Data
+
+    @Data.setter
+    def Data(self, Data):
+        self._Data = Data
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        if params.get("Data") is not None:
+            self._Data = BatchOperateResultOpsDto()
+            self._Data._deserialize(params.get("Data"))
+        self._RequestId = params.get("RequestId")
+
+
 class RunTaskRequest(AbstractModel):
     """RunTask请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -65366,14 +66971,20 @@
         :type TargetServiceType: str
         :param _TasksStr: 子任务列表
 注意：此字段可能返回 null，表示取不到有效值。
         :type TasksStr: str
         :param _Submit: 任务版本是否已提交
 注意：此字段可能返回 null，表示取不到有效值。
         :type Submit: bool
+        :param _ExecutorGroupId: 资源组id
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecutorGroupId: str
+        :param _ExecutorGroupName: 资源组名称
+注意：此字段可能返回 null，表示取不到有效值。
+        :type ExecutorGroupName: str
         """
         self._TaskId = None
         self._VirtualTaskId = None
         self._VirtualFlag = None
         self._TaskName = None
         self._WorkflowId = None
         self._RealWorkflowId = None
@@ -65447,14 +67058,16 @@
         self._Layer = None
         self._SourceServiceId = None
         self._SourceServiceType = None
         self._TargetServiceId = None
         self._TargetServiceType = None
         self._TasksStr = None
         self._Submit = None
+        self._ExecutorGroupId = None
+        self._ExecutorGroupName = None
 
     @property
     def TaskId(self):
         return self._TaskId
 
     @TaskId.setter
     def TaskId(self, TaskId):
@@ -66088,14 +67701,30 @@
     def Submit(self):
         return self._Submit
 
     @Submit.setter
     def Submit(self, Submit):
         self._Submit = Submit
 
+    @property
+    def ExecutorGroupId(self):
+        return self._ExecutorGroupId
+
+    @ExecutorGroupId.setter
+    def ExecutorGroupId(self, ExecutorGroupId):
+        self._ExecutorGroupId = ExecutorGroupId
+
+    @property
+    def ExecutorGroupName(self):
+        return self._ExecutorGroupName
+
+    @ExecutorGroupName.setter
+    def ExecutorGroupName(self, ExecutorGroupName):
+        self._ExecutorGroupName = ExecutorGroupName
+
 
     def _deserialize(self, params):
         self._TaskId = params.get("TaskId")
         self._VirtualTaskId = params.get("VirtualTaskId")
         self._VirtualFlag = params.get("VirtualFlag")
         self._TaskName = params.get("TaskName")
         self._WorkflowId = params.get("WorkflowId")
@@ -66174,14 +67803,16 @@
         self._Layer = params.get("Layer")
         self._SourceServiceId = params.get("SourceServiceId")
         self._SourceServiceType = params.get("SourceServiceType")
         self._TargetServiceId = params.get("TargetServiceId")
         self._TargetServiceType = params.get("TargetServiceType")
         self._TasksStr = params.get("TasksStr")
         self._Submit = params.get("Submit")
+        self._ExecutorGroupId = params.get("ExecutorGroupId")
+        self._ExecutorGroupName = params.get("ExecutorGroupName")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
```

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/wedata/v20210820/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/wedata/v20210820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/wedata/v20210820/wedata_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/wedata/v20210820/wedata_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -808,14 +808,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def CreateDsFolder(self, request):
+        """编排空间-创建文件夹
+
+        :param request: Request instance for CreateDsFolder.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.CreateDsFolderRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.CreateDsFolderResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("CreateDsFolder", params, headers=headers)
+            response = json.loads(body)
+            model = models.CreateDsFolderResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def CreateFolder(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         创建文件夹
 
         :param request: Request instance for CreateFolder.
         :type request: :class:`tencentcloud.wedata.v20210820.models.CreateFolderRequest`
         :rtype: :class:`tencentcloud.wedata.v20210820.models.CreateFolderResponse`
@@ -1249,14 +1272,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def DeleteDsFolder(self, request):
+        """编排空间-删除文件夹
+
+        :param request: Request instance for DeleteDsFolder.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.DeleteDsFolderRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.DeleteDsFolderResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DeleteDsFolder", params, headers=headers)
+            response = json.loads(body)
+            model = models.DeleteDsFolderResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def DeleteFile(self, request):
         """删除文件
 
         :param request: Request instance for DeleteFile.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DeleteFileRequest`
         :rtype: :class:`tencentcloud.wedata.v20210820.models.DeleteFileResponse`
 
@@ -2405,14 +2451,60 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def DescribeDsFolderTree(self, request):
+        """查询目录树
+
+        :param request: Request instance for DescribeDsFolderTree.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeDsFolderTreeRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.DescribeDsFolderTreeResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDsFolderTree", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDsFolderTreeResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def DescribeDsParentFolderTree(self, request):
+        """查询父目录树，用于工作流、任务定位
+
+        :param request: Request instance for DescribeDsParentFolderTree.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeDsParentFolderTreeRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.DescribeDsParentFolderTreeResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeDsParentFolderTree", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeDsParentFolderTreeResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def DescribeEvent(self, request):
         """根据项目ID和事件名称查看事件详情
 
         :param request: Request instance for DescribeEvent.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeEventRequest`
         :rtype: :class:`tencentcloud.wedata.v20210820.models.DescribeEventResponse`
 
@@ -3283,15 +3375,17 @@
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def DescribeKafkaTopicInfo(self, request):
-        """获取kafka的topic信息
+        """没用到
+
+        获取kafka的topic信息
 
         :param request: Request instance for DescribeKafkaTopicInfo.
         :type request: :class:`tencentcloud.wedata.v20210820.models.DescribeKafkaTopicInfoRequest`
         :rtype: :class:`tencentcloud.wedata.v20210820.models.DescribeKafkaTopicInfoResponse`
 
         """
         try:
@@ -5335,14 +5429,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def FindAllFolder(self, request):
+        """查找全部的文件夹
+
+        :param request: Request instance for FindAllFolder.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.FindAllFolderRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.FindAllFolderResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("FindAllFolder", params, headers=headers)
+            response = json.loads(body)
+            model = models.FindAllFolderResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def ForceSucInstances(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         实例批量置成功
 
         :param request: Request instance for ForceSucInstances.
         :type request: :class:`tencentcloud.wedata.v20210820.models.ForceSucInstancesRequest`
         :rtype: :class:`tencentcloud.wedata.v20210820.models.ForceSucInstancesResponse`
@@ -5850,14 +5967,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def ModifyDsFolder(self, request):
+        """数据开发模块-文件夹更新
+
+        :param request: Request instance for ModifyDsFolder.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.ModifyDsFolderRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.ModifyDsFolderResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("ModifyDsFolder", params, headers=headers)
+            response = json.loads(body)
+            model = models.ModifyDsFolderResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def ModifyExecStrategy(self, request):
         """更新规则组执行策略
 
         :param request: Request instance for ModifyExecStrategy.
         :type request: :class:`tencentcloud.wedata.v20210820.models.ModifyExecStrategyRequest`
         :rtype: :class:`tencentcloud.wedata.v20210820.models.ModifyExecStrategyResponse`
 
@@ -6409,14 +6549,60 @@
             model._deserialize(response["Response"])
             return model
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def RunForceSucScheduleInstances(self, request):
+        """实例强制成功
+
+        :param request: Request instance for RunForceSucScheduleInstances.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.RunForceSucScheduleInstancesRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.RunForceSucScheduleInstancesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("RunForceSucScheduleInstances", params, headers=headers)
+            response = json.loads(body)
+            model = models.RunForceSucScheduleInstancesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
+    def RunRerunScheduleInstances(self, request):
+        """实例批量重跑
+
+        :param request: Request instance for RunRerunScheduleInstances.
+        :type request: :class:`tencentcloud.wedata.v20210820.models.RunRerunScheduleInstancesRequest`
+        :rtype: :class:`tencentcloud.wedata.v20210820.models.RunRerunScheduleInstancesResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("RunRerunScheduleInstances", params, headers=headers)
+            response = json.loads(body)
+            model = models.RunRerunScheduleInstancesResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
     def RunTask(self, request):
         """<p style="color:red;">[注意：该Beta版本只满足广州区部分白名单客户使用]</p>
         运行任务
 
         :param request: Request instance for RunTask.
```

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/partners/v20180321/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/partners/v20180321/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/partners/v20180321/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/partners/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/partners/v20180321/partners_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/partners/v20180321/partners_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bsca/v20210811/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bsca/v20210811/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bsca/v20210811/bsca_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bsca/v20210811/bsca_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bsca/v20210811/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bsca/v20210811/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ds/v20180523/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ds/v20180523/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ds/v20180523/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ds/v20180523/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ds/v20180523/ds_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ds/v20180523/ds_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tcex/v20200727/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tcex/v20200727/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tcex/v20200727/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tcex/v20200727/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tcex/v20200727/tcex_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tcex/v20200727/tcex_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ess/v20201111/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ess/v20201111/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1609,14 +1609,28 @@
         :type ComponentName: str
         :param _ComponentRequired: 是否必选，默认为false-非必选
         :type ComponentRequired: bool
         :param _ComponentRecipientId: 控件关联的参与方ID，对应Recipient结构体中的RecipientId
         :type ComponentRecipientId: str
         :param _ComponentExtra: 扩展参数：
 为JSON格式。
+不同类型的控件会有部分非通用参数
+
+ComponentType为TEXT、MULTI_LINE_TEXT时，支持以下参数：
+1 Font：目前只支持黑体、宋体
+2 FontSize： 范围12-72
+3 FontAlign： Left/Right/Center，左对齐/居中/右对齐
+4 FontColor：字符串类型，格式为RGB颜色数字
+参数样例：    "ComponentExtra": "{\"FontColor\":\"255,0,0\",\"FontSize\":12}"
+
+TEXT/MULTI_LINE_TEXT控件可以指定
+1 Font：目前只支持黑体、宋体
+2 FontSize： 范围12-72
+3 FontAlign： Left/Right/Center，左对齐/居中/右对齐
+例如：{"FontSize":12}
 
 ComponentType为FILL_IMAGE时，支持以下参数：
 NotMakeImageCenter：bool。是否设置图片居中。false：居中（默认）。 true: 不居中
 FillMethod: int. 填充方式。0-铺满（默认）；1-等比例缩放
 
 ComponentType为SIGN_SIGNATURE类型可以控制签署方式
 {“ComponentTypeLimit”: [“xxx”]}
@@ -1631,19 +1645,19 @@
 1 Font：字符串类型目前只支持"黑体"、"宋体"，如果不填默认为"黑体"
 2 FontSize： 数字类型，范围6-72，默认值为12
 3 FontAlign： 字符串类型，可取Left/Right/Center，对应左对齐/居中/右对齐
 4 Format： 字符串类型，日期格式，必须是以下五种之一 “yyyy m d”，”yyyy年m月d日”，”yyyy/m/d”，”yyyy-m-d”，”yyyy.m.d”。
 5 Gaps:： 字符串类型，仅在Format为“yyyy m d”时起作用，格式为用逗号分开的两个整数，例如”2,2”，两个数字分别是日期格式的前后两个空隙中的空格个数
 如果extra参数为空，默认为”yyyy年m月d日”格式的居中日期
 特别地，如果extra中Format字段为空或无法被识别，则extra参数会被当作默认值处理（Font，FontSize，Gaps和FontAlign都不会起效）
-参数样例：    "ComponentExtra": "{\"Format\":“yyyy m d”,\"FontSize\":12,\"Gaps\":\"2,2\", \"FontAlign\":\"Right\"}"
+参数样例： "ComponentExtra": "{"Format":“yyyy m d”,"FontSize":12,"Gaps":"2,2", "FontAlign":"Right"}"
 
 ComponentType为SIGN_SEAL类型时，支持以下参数：
 1.PageRanges：PageRange的数组，通过PageRanges属性设置该印章在PDF所有页面上盖章（适用于标书在所有页面盖章的情况）
-参数样例："ComponentExtra":"{\"PageRanges\":[{\"BeginPage\":1,\"EndPage\":-1}]}"
+参数样例： "ComponentExtra":"{"PageRange":[{"BeginPage":1,"EndPage":-1}]}"
         :type ComponentExtra: str
         :param _IsFormType: 是否是表单域类型，默认false-不是
 注意：此字段可能返回 null，表示取不到有效值。
         :type IsFormType: bool
         :param _ComponentValue: 控件填充vaule，ComponentType和传入值类型对应关系：
 TEXT - 文本内容
 MULTI_LINE_TEXT - 文本内容
```

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ess/v20201111/ess_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ess/v20201111/ess_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ess/v20201111/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ess/v20201111/errorcodes.py`

 * *Files 0% similar despite different names*

```diff
@@ -25,14 +25,17 @@
 
 # 签署流程已有关联文档，请检查参数修改后重试。
 FAILEDOPERATION_FLOWHASDOCUMENT = 'FailedOperation.FlowHasDocument'
 
 # 流程未找到关联的电子文件信息，请检查操作步骤，检查参数，并在修改后重试。
 FAILEDOPERATION_FLOWHASNODOCUMENT = 'FailedOperation.FlowHasNoDocument'
 
+# 身份信息校验不通过，请确认后重试。
+FAILEDOPERATION_IDCARDNUMBERCHECKFAILED = 'FailedOperation.IdCardNumberCheckFailed'
+
 # 当前无可用的许可
 FAILEDOPERATION_LICENSENOQUOTA = 'FailedOperation.LicenseNoQuota'
 
 # 签署审核未通过，请先完成审核。
 FAILEDOPERATION_NOSIGNREVIEWPASS = 'FailedOperation.NoSignReviewPass'
 
 # 此合同流程不支持审批
```

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ims/v20201229/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ims/v20201229/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ims/v20201229/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ims/v20201229/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ims/v20201229/ims_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ims/v20201229/ims_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ims/v20200713/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ims/v20200713/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ims/v20200713/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ims/v20200713/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ims/v20200713/ims_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ims/v20200713/ims_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tts/v20190823/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tts/v20190823/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tts/v20190823/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tts/v20190823/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tts/v20190823/tts_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tts/v20190823/tts_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mvj/v20190926/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mvj/v20190926/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mvj/v20190926/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mvj/v20190926/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mvj/v20190926/mvj_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mvj/v20190926/mvj_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ssa/v20180608/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ssa/v20180608/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ssa/v20180608/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ssa/v20180608/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ssa/v20180608/ssa_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ssa/v20180608/ssa_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ssl/v20191205/ssl_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ssl/v20191205/ssl_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ssl/v20191205/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ssl/v20191205/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ssl/v20191205/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ssl/v20191205/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iecp/v20210914/iecp_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iecp/v20210914/iecp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iecp/v20210914/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iecp/v20210914/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iecp/v20210914/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iecp/v20210914/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ccc/v20200210/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ccc/v20200210/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7985,15 +7985,15 @@
 
 电话呼入	             105	        noSeatOnline	       无坐席在线
 
 电话呼入              106	       notWorkTime	       非工作时间   
 
 电话呼入	            107	       ivrEnd	               IVR 后直接结束
 
-电话呼入	            100	      CallinBlockedContact  呼入黑名单 
+电话呼入	            100	      blackList 呼入黑名单 
 
 电话呼出               2	              unconnected	未接通
                          
 电话呼出             201            unknown	未知状态
 
 电话呼出            203	    userReject	拒接挂断
 
@@ -8056,15 +8056,15 @@
 
 电话呼入	             105	        noSeatOnline	       无坐席在线
 
 电话呼入              106	       notWorkTime	       非工作时间   
 
 电话呼入	            107	       ivrEnd	               IVR 后直接结束
 
-电话呼入	            100	      CallinBlockedContact  呼入黑名单 
+电话呼入	            100	      blackList 呼入黑名单 
 
 电话呼出               2	              unconnected	未接通
                          
 电话呼出             201            unknown	未知状态
 听
 电话呼出            203	    userReject	拒接挂断
```

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ccc/v20200210/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ccc/v20200210/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ccc/v20200210/ccc_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ccc/v20200210/ccc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tcss/v20201101/tcss_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tcss/v20201101/tcss_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tcss/v20201101/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tcss/v20201101/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tcss/v20201101/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tcss/v20201101/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ump/v20200918/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ump/v20200918/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ump/v20200918/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ump/v20200918/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ump/v20200918/ump_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ump/v20200918/ump_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cam/v20190116/cam_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cam/v20190116/cam_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cam/v20190116/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cam/v20190116/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cam/v20190116/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cam/v20190116/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/yinsuda/v20220527/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/yinsuda/v20220527/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/yinsuda/v20220527/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/yinsuda/v20220527/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/yinsuda/v20220527/yinsuda_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/yinsuda/v20220527/yinsuda_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dcdb/v20180411/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dcdb/v20180411/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dcdb/v20180411/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dcdb/v20180411/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dcdb/v20180411/dcdb_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dcdb/v20180411/dcdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/autoscaling/v20180419/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/autoscaling/v20180419/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/autoscaling/v20180419/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/autoscaling/v20180419/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/autoscaling/v20180419/autoscaling_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/autoscaling/v20180419/autoscaling_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cat/v20180409/cat_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cat/v20180409/cat_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cat/v20180409/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cat/v20180409/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cat/v20180409/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cat/v20180409/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tag/v20180813/tag_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tag/v20180813/tag_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tag/v20180813/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tag/v20180813/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tag/v20180813/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tag/v20180813/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/car/v20220110/car_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/car/v20220110/car_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/car/v20220110/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/car/v20220110/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/car/v20220110/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/car/v20220110/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mrs/v20200910/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mrs/v20200910/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mrs/v20200910/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mrs/v20200910/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mrs/v20200910/mrs_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mrs/v20200910/mrs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/rp/v20200224/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/rp/v20200224/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/rp/v20200224/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/rp/v20200224/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/rp/v20200224/rp_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/rp/v20200224/rp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ic/v20190307/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ic/v20190307/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ic/v20190307/ic_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ic/v20190307/ic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ic/v20190307/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ic/v20190307/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tem/v20201221/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tem/v20201221/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tem/v20201221/tem_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tem/v20201221/tem_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tem/v20201221/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tem/v20201221/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tem/v20210701/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tem/v20210701/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tem/v20210701/tem_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tem/v20210701/tem_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tem/v20210701/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tem/v20210701/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/gs/v20191118/gs_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/gs/v20191118/gs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/gs/v20191118/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/gs/v20191118/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/gs/v20191118/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/gs/v20191118/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/trp/v20210515/trp_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/trp/v20210515/trp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/trp/v20210515/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/trp/v20210515/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/trp/v20210515/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/trp/v20210515/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/goosefs/v20220519/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/goosefs/v20220519/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/goosefs/v20220519/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/goosefs/v20220519/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/goosefs/v20220519/goosefs_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/goosefs/v20220519/goosefs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bmvpc/v20180625/bmvpc_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bmvpc/v20180625/bmvpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bmvpc/v20180625/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bmvpc/v20180625/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bmvpc/v20180625/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bmvpc/v20180625/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dbbrain/v20210527/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dbbrain/v20210527/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dbbrain/v20210527/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dbbrain/v20210527/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dbbrain/v20210527/dbbrain_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dbbrain/v20210527/dbbrain_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dbbrain/v20191016/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dbbrain/v20191016/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dbbrain/v20191016/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dbbrain/v20191016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dbbrain/v20191016/dbbrain_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dbbrain/v20191016/dbbrain_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cpdp/v20190820/cpdp_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cpdp/v20190820/cpdp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cpdp/v20190820/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cpdp/v20190820/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cpdp/v20190820/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cpdp/v20190820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/domain/v20180808/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/domain/v20180808/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/domain/v20180808/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/domain/v20180808/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/domain/v20180808/domain_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/domain/v20180808/domain_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mariadb/v20170312/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mariadb/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mariadb/v20170312/mariadb_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mariadb/v20170312/mariadb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mariadb/v20170312/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mariadb/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tmt/v20180321/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tmt/v20180321/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tmt/v20180321/tmt_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tmt/v20180321/tmt_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tmt/v20180321/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tmt/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iotexplorer/v20190423/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iotexplorer/v20190423/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -7965,14 +7965,180 @@
             for item in params.get("Positions"):
                 obj = PositionItem()
                 obj._deserialize(item)
                 self._Positions.append(obj)
         self._RequestId = params.get("RequestId")
 
 
+class GetDeviceSumStatisticsRequest(AbstractModel):
+    """GetDeviceSumStatistics请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ProjectId: 项目id
+        :type ProjectId: str
+        :param _ProductIds: 产品id列表，长度为0则拉取项目内全部产品
+        :type ProductIds: list of str
+        """
+        self._ProjectId = None
+        self._ProductIds = None
+
+    @property
+    def ProjectId(self):
+        return self._ProjectId
+
+    @ProjectId.setter
+    def ProjectId(self, ProjectId):
+        self._ProjectId = ProjectId
+
+    @property
+    def ProductIds(self):
+        return self._ProductIds
+
+    @ProductIds.setter
+    def ProductIds(self, ProductIds):
+        self._ProductIds = ProductIds
+
+
+    def _deserialize(self, params):
+        self._ProjectId = params.get("ProjectId")
+        self._ProductIds = params.get("ProductIds")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class GetDeviceSumStatisticsResponse(AbstractModel):
+    """GetDeviceSumStatistics返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _ActivationCount: 激活设备总数
+        :type ActivationCount: int
+        :param _OnlineCount: 在线设备总数
+        :type OnlineCount: int
+        :param _ActivationBeforeDay: 前一天激活设备数
+        :type ActivationBeforeDay: int
+        :param _ActiveBeforeDay: 前一天活跃设备数
+        :type ActiveBeforeDay: int
+        :param _ActivationWeekDayCount: 前一周激活设备数
+        :type ActivationWeekDayCount: int
+        :param _ActiveWeekDayCount: 前一周活跃设备数
+        :type ActiveWeekDayCount: int
+        :param _ActivationBeforeWeekDayCount: 上一周激活设备数
+        :type ActivationBeforeWeekDayCount: int
+        :param _ActiveBeforeWeekDayCount: 上一周活跃设备数
+        :type ActiveBeforeWeekDayCount: int
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._ActivationCount = None
+        self._OnlineCount = None
+        self._ActivationBeforeDay = None
+        self._ActiveBeforeDay = None
+        self._ActivationWeekDayCount = None
+        self._ActiveWeekDayCount = None
+        self._ActivationBeforeWeekDayCount = None
+        self._ActiveBeforeWeekDayCount = None
+        self._RequestId = None
+
+    @property
+    def ActivationCount(self):
+        return self._ActivationCount
+
+    @ActivationCount.setter
+    def ActivationCount(self, ActivationCount):
+        self._ActivationCount = ActivationCount
+
+    @property
+    def OnlineCount(self):
+        return self._OnlineCount
+
+    @OnlineCount.setter
+    def OnlineCount(self, OnlineCount):
+        self._OnlineCount = OnlineCount
+
+    @property
+    def ActivationBeforeDay(self):
+        return self._ActivationBeforeDay
+
+    @ActivationBeforeDay.setter
+    def ActivationBeforeDay(self, ActivationBeforeDay):
+        self._ActivationBeforeDay = ActivationBeforeDay
+
+    @property
+    def ActiveBeforeDay(self):
+        return self._ActiveBeforeDay
+
+    @ActiveBeforeDay.setter
+    def ActiveBeforeDay(self, ActiveBeforeDay):
+        self._ActiveBeforeDay = ActiveBeforeDay
+
+    @property
+    def ActivationWeekDayCount(self):
+        return self._ActivationWeekDayCount
+
+    @ActivationWeekDayCount.setter
+    def ActivationWeekDayCount(self, ActivationWeekDayCount):
+        self._ActivationWeekDayCount = ActivationWeekDayCount
+
+    @property
+    def ActiveWeekDayCount(self):
+        return self._ActiveWeekDayCount
+
+    @ActiveWeekDayCount.setter
+    def ActiveWeekDayCount(self, ActiveWeekDayCount):
+        self._ActiveWeekDayCount = ActiveWeekDayCount
+
+    @property
+    def ActivationBeforeWeekDayCount(self):
+        return self._ActivationBeforeWeekDayCount
+
+    @ActivationBeforeWeekDayCount.setter
+    def ActivationBeforeWeekDayCount(self, ActivationBeforeWeekDayCount):
+        self._ActivationBeforeWeekDayCount = ActivationBeforeWeekDayCount
+
+    @property
+    def ActiveBeforeWeekDayCount(self):
+        return self._ActiveBeforeWeekDayCount
+
+    @ActiveBeforeWeekDayCount.setter
+    def ActiveBeforeWeekDayCount(self, ActiveBeforeWeekDayCount):
+        self._ActiveBeforeWeekDayCount = ActiveBeforeWeekDayCount
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._ActivationCount = params.get("ActivationCount")
+        self._OnlineCount = params.get("OnlineCount")
+        self._ActivationBeforeDay = params.get("ActivationBeforeDay")
+        self._ActiveBeforeDay = params.get("ActiveBeforeDay")
+        self._ActivationWeekDayCount = params.get("ActivationWeekDayCount")
+        self._ActiveWeekDayCount = params.get("ActiveWeekDayCount")
+        self._ActivationBeforeWeekDayCount = params.get("ActivationBeforeWeekDayCount")
+        self._ActiveBeforeWeekDayCount = params.get("ActiveBeforeWeekDayCount")
+        self._RequestId = params.get("RequestId")
+
+
 class GetFamilyDeviceUserListRequest(AbstractModel):
     """GetFamilyDeviceUserList请求参数结构体
 
     """
 
     def __init__(self):
         r"""
```

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iotexplorer/v20190423/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iotexplorer/v20190423/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iotexplorer/v20190423/iotexplorer_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -1356,14 +1356,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def GetDeviceSumStatistics(self, request):
+        """拉取设备统计汇总数据
+
+        :param request: Request instance for GetDeviceSumStatistics.
+        :type request: :class:`tencentcloud.iotexplorer.v20190423.models.GetDeviceSumStatisticsRequest`
+        :rtype: :class:`tencentcloud.iotexplorer.v20190423.models.GetDeviceSumStatisticsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("GetDeviceSumStatistics", params, headers=headers)
+            response = json.loads(body)
+            model = models.GetDeviceSumStatisticsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def GetFamilyDeviceUserList(self, request):
         """用于获取设备绑定的用户列表
 
         :param request: Request instance for GetFamilyDeviceUserList.
         :type request: :class:`tencentcloud.iotexplorer.v20190423.models.GetFamilyDeviceUserListRequest`
         :rtype: :class:`tencentcloud.iotexplorer.v20190423.models.GetFamilyDeviceUserListResponse`
```

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ses/v20201002/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ses/v20201002/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ses/v20201002/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ses/v20201002/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ses/v20201002/ses_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ses/v20201002/ses_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/casb/v20200507/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/casb/v20200507/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/casb/v20200507/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/casb/v20200507/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/casb/v20200507/casb_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/casb/v20200507/casb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ticm/v20181127/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ticm/v20181127/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ticm/v20181127/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ticm/v20181127/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ticm/v20181127/ticm_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ticm/v20181127/ticm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cbs/v20170312/cbs_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cbs/v20170312/cbs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cbs/v20170312/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cbs/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cbs/v20170312/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cbs/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tic/v20201117/tic_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tic/v20201117/tic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tic/v20201117/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tic/v20201117/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tic/v20201117/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tic/v20201117/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tat/v20201028/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tat/v20201028/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tat/v20201028/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tat/v20201028/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tat/v20201028/tat_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tat/v20201028/tat_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/advisor/v20200721/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/advisor/v20200721/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/advisor/v20200721/advisor_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/advisor/v20200721/advisor_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/advisor/v20200721/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/advisor/v20200721/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/facefusion/v20181201/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/facefusion/v20181201/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/facefusion/v20181201/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/facefusion/v20181201/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/facefusion/v20181201/facefusion_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/facefusion/v20181201/facefusion_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/facefusion/v20220927/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/facefusion/v20220927/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/facefusion/v20220927/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/facefusion/v20220927/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/facefusion/v20220927/facefusion_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/facefusion/v20220927/facefusion_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tcr/v20190924/tcr_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tcr/v20190924/tcr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tcr/v20190924/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tcr/v20190924/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tcr/v20190924/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tcr/v20190924/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tbaas/v20180416/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tbaas/v20180416/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tbaas/v20180416/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tbaas/v20180416/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tbaas/v20180416/tbaas_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tbaas/v20180416/tbaas_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cvm/v20170312/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cvm/v20170312/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -2554,17 +2554,17 @@
 该参数目前仅用于 `RunInstances` 接口。
 注意：此字段可能返回 null，表示取不到有效值。
         :type DeleteWithInstance: bool
         :param _SnapshotId: 数据盘快照ID。选择的数据盘快照大小需小于数据盘大小。
 注意：此字段可能返回 null，表示取不到有效值。
         :type SnapshotId: str
         :param _Encrypt: 数据盘是加密。取值范围：
-<li>TRUE：加密
-<li>FALSE：不加密<br>
-默认取值：FALSE<br>
+<li>true：加密
+<li>false：不加密<br>
+默认取值：false<br>
 该参数目前仅用于 `RunInstances` 接口。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Encrypt: bool
         :param _KmsKeyId: 自定义CMK对应的ID，取值为UUID或者类似kms-abcd1234。用于加密云盘。
 
 该参数目前仅用于 `RunInstances` 接口。
 注意：此字段可能返回 null，表示取不到有效值。
@@ -16128,15 +16128,15 @@
 class RunAutomationServiceEnabled(AbstractModel):
     """描述了 “云自动化助手” 服务相关的信息
 
     """
 
     def __init__(self):
         r"""
-        :param _Enabled: 是否开启云自动化助手。取值范围：<br><li>TRUE：表示开启云自动化助手服务<br><li>FALSE：表示不开启云自动化助手服务<br><br>默认取值：FALSE。
+        :param _Enabled: 是否开启云自动化助手。取值范围：<br><li>true：表示开启云自动化助手服务<br><li>false：表示不开启云自动化助手服务<br><br>默认取值：false。
         :type Enabled: bool
         """
         self._Enabled = None
 
     @property
     def Enabled(self):
         return self._Enabled
@@ -16592,15 +16592,16 @@
 class RunMonitorServiceEnabled(AbstractModel):
     """描述了 “云监控” 服务相关的信息
 
     """
 
     def __init__(self):
         r"""
-        :param _Enabled: 是否开启[云监控](/document/product/248)服务。取值范围：<br><li>TRUE：表示开启云监控服务<br><li>FALSE：表示不开启云监控服务<br><br>默认取值：TRUE。
+        :param _Enabled: 是否开启[云监控](/document/product/248)服务。取值范围：<br><li>true：表示开启云监控服务<br><li>false：表示不开启云监控服务<br><br>默认取值：true。
+注意：此字段可能返回 null，表示取不到有效值。
         :type Enabled: bool
         """
         self._Enabled = None
 
     @property
     def Enabled(self):
         return self._Enabled
@@ -17500,15 +17501,15 @@
 
     def __init__(self):
         r"""
         :param _VpcId: 私有网络ID，形如`vpc-xxx`。有效的VpcId可通过登录[控制台](https://console.cloud.tencent.com/vpc/vpc?rid=1)查询；也可以调用接口 [DescribeVpcEx](/document/api/215/1372) ，从接口返回中的`unVpcId`字段获取。若在创建子机时VpcId与SubnetId同时传入`DEFAULT`，则强制使用默认vpc网络。
         :type VpcId: str
         :param _SubnetId: 私有网络子网ID，形如`subnet-xxx`。有效的私有网络子网ID可通过登录[控制台](https://console.cloud.tencent.com/vpc/subnet?rid=1)查询；也可以调用接口  [DescribeSubnets](/document/api/215/15784) ，从接口返回中的`unSubnetId`字段获取。若在创建子机时SubnetId与VpcId同时传入`DEFAULT`，则强制使用默认vpc网络。
         :type SubnetId: str
-        :param _AsVpcGateway: 是否用作公网网关。公网网关只有在实例拥有公网IP以及处于私有网络下时才能正常使用。取值范围：<br><li>TRUE：表示用作公网网关<br><li>FALSE：表示不作为公网网关<br><br>默认取值：FALSE。
+        :param _AsVpcGateway: 是否用作公网网关。公网网关只有在实例拥有公网IP以及处于私有网络下时才能正常使用。取值范围：<br><li>true：表示用作公网网关<br><li>false：表示不作为公网网关<br><br>默认取值：false。
         :type AsVpcGateway: bool
         :param _PrivateIpAddresses: 私有网络子网 IP 数组，在创建实例、修改实例vpc属性操作中可使用此参数。当前仅批量创建多台实例时支持传入相同子网的多个 IP。
         :type PrivateIpAddresses: list of str
         :param _Ipv6AddressCount: 为弹性网卡指定随机生成的 IPv6 地址数量。
         :type Ipv6AddressCount: int
         """
         self._VpcId = None
```

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cvm/v20170312/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cvm/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cvm/v20170312/cvm_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cvm/v20170312/cvm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/anicloud/v20220923/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/anicloud/v20220923/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/anicloud/v20220923/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/anicloud/v20220923/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/anicloud/v20220923/anicloud_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/anicloud/v20220923/anicloud_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/hasim/v20210716/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/hasim/v20210716/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/hasim/v20210716/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/hasim/v20210716/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/hasim/v20210716/hasim_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/hasim/v20210716/hasim_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cme/v20191029/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cme/v20191029/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cme/v20191029/cme_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cme/v20191029/cme_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cme/v20191029/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cme/v20191029/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/clb/v20180317/clb_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/clb/v20180317/clb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/clb/v20180317/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/clb/v20180317/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/clb/v20180317/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/clb/v20180317/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tse/v20201207/tse_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tse/v20201207/tse_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tse/v20201207/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tse/v20201207/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tse/v20201207/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tse/v20201207/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ie/v20200304/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ie/v20200304/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ie/v20200304/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ie/v20200304/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ie/v20200304/ie_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ie/v20200304/ie_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/smop/v20201203/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/smop/v20201203/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/smop/v20201203/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/smop/v20201203/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/smop/v20201203/smop_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/smop/v20201203/smop_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cdb/v20170320/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cdb/v20170320/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cdb/v20170320/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cdb/v20170320/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cdb/v20170320/cdb_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cdb/v20170320/cdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/redis/v20180412/redis_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/redis/v20180412/redis_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/redis/v20180412/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/redis/v20180412/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/redis/v20180412/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/redis/v20180412/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tms/v20201229/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tms/v20201229/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tms/v20201229/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tms/v20201229/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tms/v20201229/tms_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tms/v20201229/tms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tms/v20200713/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tms/v20200713/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tms/v20200713/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tms/v20200713/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tms/v20200713/tms_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tms/v20200713/tms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/region/v20220627/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/region/v20220627/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/region/v20220627/region_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/region/v20220627/region_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/region/v20220627/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/region/v20220627/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tke/v20180525/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tke/v20180525/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -34414,15 +34414,15 @@
 class RunAutomationServiceEnabled(AbstractModel):
     """描述了 “云自动化助手” 服务相关的信息
 
     """
 
     def __init__(self):
         r"""
-        :param _Enabled: 是否开启云自动化助手。取值范围：<br><li>TRUE：表示开启云自动化助手服务<br><li>FALSE：表示不开启云自动化助手服务<br><br>默认取值：FALSE。
+        :param _Enabled: 是否开启云自动化助手。取值范围：<br><li>true：表示开启云自动化助手服务<br><li>false：表示不开启云自动化助手服务<br><br>默认取值：false。
         :type Enabled: bool
         """
         self._Enabled = None
 
     @property
     def Enabled(self):
         return self._Enabled
@@ -34509,15 +34509,16 @@
 class RunMonitorServiceEnabled(AbstractModel):
     """描述了 “云监控” 服务相关的信息
 
     """
 
     def __init__(self):
         r"""
-        :param _Enabled: 是否开启[云监控](/document/product/248)服务。取值范围：<br><li>TRUE：表示开启云监控服务<br><li>FALSE：表示不开启云监控服务<br><br>默认取值：TRUE。
+        :param _Enabled: 是否开启[云监控](/document/product/248)服务。取值范围：<br><li>true：表示开启云监控服务<br><li>false：表示不开启云监控服务<br><br>默认取值：true。
+注意：此字段可能返回 null，表示取不到有效值。
         :type Enabled: bool
         """
         self._Enabled = None
 
     @property
     def Enabled(self):
         return self._Enabled
```

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tke/v20180525/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tke/v20180525/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tke/v20180525/tke_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tke/v20180525/tke_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cr/v20180321/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cr/v20180321/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cr/v20180321/cr_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cr/v20180321/cr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cr/v20180321/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cr/v20180321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/btoe/v20210514/btoe_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/btoe/v20210514/btoe_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/btoe/v20210514/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/btoe/v20210514/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/btoe/v20210514/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/btoe/v20210514/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/btoe/v20210303/btoe_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/btoe/v20210303/btoe_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/btoe/v20210303/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/btoe/v20210303/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/btoe/v20210303/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/btoe/v20210303/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dsgc/v20190723/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dsgc/v20190723/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dsgc/v20190723/dsgc_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dsgc/v20190723/dsgc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dsgc/v20190723/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dsgc/v20190723/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cynosdb/v20190107/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cynosdb/v20190107/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cynosdb/v20190107/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cynosdb/v20190107/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cynosdb/v20190107/cynosdb_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cynosdb/v20190107/cynosdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/af/v20200226/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/af/v20200226/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/af/v20200226/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/af/v20200226/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/af/v20200226/af_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/af/v20200226/af_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/__init__.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,8 +10,8 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-__version__ = '3.0.998'
+__version__ = '3.0.999'
```

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ft/v20200304/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ft/v20200304/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ft/v20200304/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ft/v20200304/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ft/v20200304/ft_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ft/v20200304/ft_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/acp/v20220105/acp_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/acp/v20220105/acp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/acp/v20220105/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/acp/v20220105/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/acp/v20220105/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/acp/v20220105/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/sms/v20210111/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/sms/v20210111/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/sms/v20210111/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/sms/v20210111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/sms/v20210111/sms_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/sms/v20210111/sms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/sms/v20190711/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/sms/v20190711/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/sms/v20190711/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/sms/v20190711/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/sms/v20190711/sms_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/sms/v20190711/sms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/lcic/v20220817/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/lcic/v20220817/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/lcic/v20220817/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/lcic/v20220817/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/lcic/v20220817/lcic_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/lcic/v20220817/lcic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/fmu/v20191213/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/fmu/v20191213/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/fmu/v20191213/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/fmu/v20191213/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/fmu/v20191213/fmu_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/fmu/v20191213/fmu_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/teo/v20220106/teo_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/teo/v20220106/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/teo/v20220106/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/teo/v20220106/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/teo/v20220106/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/teo/v20220106/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/teo/v20220901/teo_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/teo/v20220901/teo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/teo/v20220901/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/teo/v20220901/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/teo/v20220901/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/teo/v20220901/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ciam/v20220331/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ciam/v20220331/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ciam/v20220331/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ciam/v20220331/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ciam/v20220331/ciam_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ciam/v20220331/ciam_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/monitor/v20180724/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/monitor/v20180724/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/monitor/v20180724/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/monitor/v20180724/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/monitor/v20180724/monitor_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/monitor/v20180724/monitor_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ecc/v20181213/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ecc/v20181213/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ecc/v20181213/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ecc/v20181213/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ecc/v20181213/ecc_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ecc/v20181213/ecc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bizlive/v20190313/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bizlive/v20190313/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bizlive/v20190313/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bizlive/v20190313/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bizlive/v20190313/bizlive_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bizlive/v20190313/bizlive_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/irp/v20220324/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/irp/v20220324/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/irp/v20220324/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/irp/v20220324/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/irp/v20220324/irp_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/irp/v20220324/irp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/irp/v20220805/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/irp/v20220805/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/irp/v20220805/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/irp/v20220805/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/irp/v20220805/irp_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/irp/v20220805/irp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/faceid/v20180301/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/faceid/v20180301/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/faceid/v20180301/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/faceid/v20180301/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/faceid/v20180301/faceid_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/faceid/v20180301/faceid_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tics/v20181115/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tics/v20181115/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tics/v20181115/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tics/v20181115/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tics/v20181115/tics_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tics/v20181115/tics_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/nlp/v20190408/nlp_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/nlp/v20190408/nlp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/nlp/v20190408/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/nlp/v20190408/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/nlp/v20190408/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/nlp/v20190408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/waf/v20180125/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/waf/v20180125/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/waf/v20180125/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/waf/v20180125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/waf/v20180125/waf_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/waf/v20180125/waf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/gaap/v20180529/gaap_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/gaap/v20180529/gaap_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/gaap/v20180529/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/gaap/v20180529/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/gaap/v20180529/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/gaap/v20180529/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tan/v20220420/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tan/v20220420/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tan/v20220420/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tan/v20220420/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tan/v20220420/tan_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tan/v20220420/tan_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/vod/v20180717/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/vod/v20180717/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/vod/v20180717/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/vod/v20180717/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/vod/v20180717/vod_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/vod/v20180717/vod_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ecm/v20190719/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ecm/v20190719/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ecm/v20190719/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ecm/v20190719/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ecm/v20190719/ecm_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ecm/v20190719/ecm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/lowcode/v20210108/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/lowcode/v20210108/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/lowcode/v20210108/lowcode_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/lowcode/v20210108/lowcode_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/lowcode/v20210108/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/lowcode/v20210108/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ms/v20180408/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ms/v20180408/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ms/v20180408/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ms/v20180408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ms/v20180408/ms_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ms/v20180408/ms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/vrs/v20200824/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/vrs/v20200824/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/vrs/v20200824/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/vrs/v20200824/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/vrs/v20200824/vrs_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/vrs/v20200824/vrs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bri/v20190328/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bri/v20190328/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bri/v20190328/bri_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bri/v20190328/bri_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bri/v20190328/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bri/v20190328/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cis/v20180408/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cis/v20180408/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cis/v20180408/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cis/v20180408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cis/v20180408/cis_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cis/v20180408/cis_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/gse/v20191112/gse_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/gse/v20191112/gse_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/gse/v20191112/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/gse/v20191112/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/gse/v20191112/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/gse/v20191112/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tourism/v20230215/tourism_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tourism/v20230215/tourism_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tourism/v20230215/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tourism/v20230215/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tourism/v20230215/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tourism/v20230215/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/apigateway/v20180808/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/apigateway/v20180808/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/apigateway/v20180808/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/apigateway/v20180808/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/apigateway/v20180808/apigateway_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/apigateway/v20180808/apigateway_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iai/v20180301/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iai/v20180301/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iai/v20180301/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iai/v20180301/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iai/v20180301/iai_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iai/v20180301/iai_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iai/v20200303/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iai/v20200303/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iai/v20200303/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iai/v20200303/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iai/v20200303/iai_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iai/v20200303/iai_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/es/v20180416/es_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/es/v20180416/es_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/es/v20180416/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/es/v20180416/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/es/v20180416/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/es/v20180416/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/eb/v20210416/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/eb/v20210416/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/eb/v20210416/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/eb/v20210416/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/eb/v20210416/eb_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/eb/v20210416/eb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bda/v20200324/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bda/v20200324/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bda/v20200324/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bda/v20200324/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bda/v20200324/bda_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bda/v20200324/bda_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dasb/v20191018/dasb_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dasb/v20191018/dasb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dasb/v20191018/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dasb/v20191018/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dasb/v20191018/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dasb/v20191018/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ecdn/v20191012/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ecdn/v20191012/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ecdn/v20191012/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ecdn/v20191012/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ecdn/v20191012/ecdn_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ecdn/v20191012/ecdn_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/postgres/v20170312/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/postgres/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/postgres/v20170312/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/postgres/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/postgres/v20170312/postgres_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/postgres/v20170312/postgres_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/youmall/v20180228/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/youmall/v20180228/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/youmall/v20180228/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/youmall/v20180228/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/youmall/v20180228/youmall_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/youmall/v20180228/youmall_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dts/v20180330/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dts/v20180330/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dts/v20180330/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dts/v20180330/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dts/v20180330/dts_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dts/v20180330/dts_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dts/v20211206/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dts/v20211206/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dts/v20211206/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dts/v20211206/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dts/v20211206/dts_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dts/v20211206/dts_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/common/abstract_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/common/abstract_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/common/sign.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/common/sign.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/common/abstract_model.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/common/abstract_model.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/common/exception/__init__.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/common/exception/__init__.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/common/exception/tencent_cloud_sdk_exception.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/common/exception/tencent_cloud_sdk_exception.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/common/common_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/common/common_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/common/http/request.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/common/http/request.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/common/profile/http_profile.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/common/profile/http_profile.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/common/profile/client_profile.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/common/profile/client_profile.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/common/circuit_breaker.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/common/circuit_breaker.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/common/credential.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/common/credential.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ba/v20200720/ba_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ba/v20200720/ba_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ba/v20200720/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ba/v20200720/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ba/v20200720/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ba/v20200720/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tia/v20180226/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tia/v20180226/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tia/v20180226/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tia/v20180226/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tia/v20180226/tia_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tia/v20180226/tia_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/taf/v20200210/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/taf/v20200210/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/taf/v20200210/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/taf/v20200210/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/taf/v20200210/taf_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/taf/v20200210/taf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ame/v20190916/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ame/v20190916/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ame/v20190916/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ame/v20190916/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ame/v20190916/ame_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ame/v20190916/ame_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tcbr/v20220217/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tcbr/v20220217/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tcbr/v20220217/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tcbr/v20220217/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tcbr/v20220217/tcbr_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tcbr/v20220217/tcbr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/csxg/v20230303/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/csxg/v20230303/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/csxg/v20230303/csxg_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/csxg/v20230303/csxg_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/csxg/v20230303/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/csxg/v20230303/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/smpn/v20190822/smpn_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/smpn/v20190822/smpn_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/smpn/v20190822/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/smpn/v20190822/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/smpn/v20190822/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/smpn/v20190822/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cii/v20210408/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cii/v20210408/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cii/v20210408/cii_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cii/v20210408/cii_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cii/v20210408/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cii/v20210408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cii/v20201210/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cii/v20201210/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cii/v20201210/cii_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cii/v20201210/cii_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cii/v20201210/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cii/v20201210/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cds/v20180420/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cds/v20180420/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cds/v20180420/cds_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cds/v20180420/cds_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cds/v20180420/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cds/v20180420/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/afc/v20200226/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/afc/v20200226/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/afc/v20200226/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/afc/v20200226/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/afc/v20200226/afc_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/afc/v20200226/afc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/aai/v20180522/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/aai/v20180522/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/aai/v20180522/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/aai/v20180522/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/aai/v20180522/aai_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/aai/v20180522/aai_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/csip/v20221121/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/csip/v20221121/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -3347,26 +3347,29 @@
         :type ScanPlanType: int
         :param _Assets: 扫描资产信息列表
         :type Assets: list of TaskAssetObject
         :param _ScanPlanContent: 扫描计划详情
         :type ScanPlanContent: str
         :param _SelfDefiningAssets: ip/域名/url数组
         :type SelfDefiningAssets: list of str
+        :param _ScanFrom: 请求发起源，默认为vss表示漏洞扫描服务，云安全中心的用户请填充csip
+        :type ScanFrom: str
         :param _TaskAdvanceCFG: 高级配置
         :type TaskAdvanceCFG: :class:`tencentcloud.csip.v20221121.models.TaskAdvanceCFG`
         :param _TaskMode: 体检模式，0-标准模式，1-快速模式，2-高级模式，默认标准模式
         :type TaskMode: int
         """
         self._TaskName = None
         self._ScanAssetType = None
         self._ScanItem = None
         self._ScanPlanType = None
         self._Assets = None
         self._ScanPlanContent = None
         self._SelfDefiningAssets = None
+        self._ScanFrom = None
         self._TaskAdvanceCFG = None
         self._TaskMode = None
 
     @property
     def TaskName(self):
         return self._TaskName
 
@@ -3419,14 +3422,22 @@
         return self._SelfDefiningAssets
 
     @SelfDefiningAssets.setter
     def SelfDefiningAssets(self, SelfDefiningAssets):
         self._SelfDefiningAssets = SelfDefiningAssets
 
     @property
+    def ScanFrom(self):
+        return self._ScanFrom
+
+    @ScanFrom.setter
+    def ScanFrom(self, ScanFrom):
+        self._ScanFrom = ScanFrom
+
+    @property
     def TaskAdvanceCFG(self):
         return self._TaskAdvanceCFG
 
     @TaskAdvanceCFG.setter
     def TaskAdvanceCFG(self, TaskAdvanceCFG):
         self._TaskAdvanceCFG = TaskAdvanceCFG
 
@@ -3448,14 +3459,15 @@
             self._Assets = []
             for item in params.get("Assets"):
                 obj = TaskAssetObject()
                 obj._deserialize(item)
                 self._Assets.append(obj)
         self._ScanPlanContent = params.get("ScanPlanContent")
         self._SelfDefiningAssets = params.get("SelfDefiningAssets")
+        self._ScanFrom = params.get("ScanFrom")
         if params.get("TaskAdvanceCFG") is not None:
             self._TaskAdvanceCFG = TaskAdvanceCFG()
             self._TaskAdvanceCFG._deserialize(params.get("TaskAdvanceCFG"))
         self._TaskMode = params.get("TaskMode")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
```

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/csip/v20221121/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/csip/v20221121/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/csip/v20221121/csip_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/csip/v20221121/csip_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dataintegration/v20220613/dataintegration_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dataintegration/v20220613/dataintegration_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dataintegration/v20220613/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dataintegration/v20220613/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dataintegration/v20220613/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dataintegration/v20220613/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/npp/v20190823/npp_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/npp/v20190823/npp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/npp/v20190823/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/npp/v20190823/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/npp/v20190823/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/npp/v20190823/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iss/v20230517/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iss/v20230517/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iss/v20230517/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iss/v20230517/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iss/v20230517/iss_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iss/v20230517/iss_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/captcha/v20190722/captcha_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/captcha/v20190722/captcha_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/captcha/v20190722/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/captcha/v20190722/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/captcha/v20190722/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/captcha/v20190722/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/trdp/v20220726/trdp_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/trdp/v20220726/trdp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/trdp/v20220726/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/trdp/v20220726/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/trdp/v20220726/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/trdp/v20220726/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/chdfs/v20190718/chdfs_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/chdfs/v20190718/chdfs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/chdfs/v20190718/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/chdfs/v20190718/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/chdfs/v20190718/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/chdfs/v20190718/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/chdfs/v20201112/chdfs_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/chdfs/v20201112/chdfs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/chdfs/v20201112/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/chdfs/v20201112/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/chdfs/v20201112/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/chdfs/v20201112/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mmps/v20200710/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mmps/v20200710/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mmps/v20200710/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mmps/v20200710/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mmps/v20200710/mmps_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mmps/v20200710/mmps_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/api/v20201106/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/api/v20201106/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/api/v20201106/api_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/api/v20201106/api_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/api/v20201106/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/api/v20201106/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/organization/v20181225/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/organization/v20181225/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/organization/v20181225/organization_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/organization/v20181225/organization_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/organization/v20181225/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/organization/v20181225/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/organization/v20210331/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/organization/v20210331/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/organization/v20210331/organization_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/organization/v20210331/organization_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/organization/v20210331/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/organization/v20210331/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tci/v20190318/tci_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tci/v20190318/tci_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tci/v20190318/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tci/v20190318/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tci/v20190318/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tci/v20190318/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ckafka/v20190819/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ckafka/v20190819/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ckafka/v20190819/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ckafka/v20190819/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ckafka/v20190819/ckafka_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ckafka/v20190819/ckafka_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tds/v20220801/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tds/v20220801/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tds/v20220801/tds_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tds/v20220801/tds_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tds/v20220801/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tds/v20220801/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dbdc/v20201029/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dbdc/v20201029/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dbdc/v20201029/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dbdc/v20201029/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dbdc/v20201029/dbdc_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dbdc/v20201029/dbdc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cloudhsm/v20191112/cloudhsm_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cloudhsm/v20191112/cloudhsm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cloudhsm/v20191112/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cloudhsm/v20191112/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cloudhsm/v20191112/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cloudhsm/v20191112/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tiems/v20190416/tiems_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tiems/v20190416/tiems_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tiems/v20190416/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tiems/v20190416/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tiems/v20190416/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tiems/v20190416/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bmeip/v20180625/bmeip_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bmeip/v20180625/bmeip_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bmeip/v20180625/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bmeip/v20180625/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bmeip/v20180625/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bmeip/v20180625/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ssm/v20190923/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ssm/v20190923/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ssm/v20190923/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ssm/v20190923/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ssm/v20190923/ssm_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ssm/v20190923/ssm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cfs/v20190719/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cfs/v20190719/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cfs/v20190719/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cfs/v20190719/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cfs/v20190719/cfs_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cfs/v20190719/cfs_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tsw/v20200924/tsw_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tsw/v20200924/tsw_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tsw/v20200924/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tsw/v20200924/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tsw/v20200924/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tsw/v20200924/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tsw/v20210412/tsw_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tsw/v20210412/tsw_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tsw/v20210412/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tsw/v20210412/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tsw/v20210412/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tsw/v20210412/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/yunjing/v20180228/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/yunjing/v20180228/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/yunjing/v20180228/yunjing_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/yunjing/v20180228/yunjing_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/yunjing/v20180228/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/yunjing/v20180228/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/gpm/v20200820/gpm_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/gpm/v20200820/gpm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/gpm/v20200820/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/gpm/v20200820/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/gpm/v20200820/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/gpm/v20200820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tdid/v20210519/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tdid/v20210519/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tdid/v20210519/tdid_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tdid/v20210519/tdid_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tdid/v20210519/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tdid/v20210519/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/apm/v20210622/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/apm/v20210622/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/apm/v20210622/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/apm/v20210622/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/apm/v20210622/apm_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/apm/v20210622/apm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/solar/v20181011/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/solar/v20181011/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/solar/v20181011/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/solar/v20181011/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/solar/v20181011/solar_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/solar/v20181011/solar_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/gme/v20180711/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/gme/v20180711/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/gme/v20180711/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/gme/v20180711/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/gme/v20180711/gme_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/gme/v20180711/gme_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/icr/v20211014/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/icr/v20211014/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/icr/v20211014/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/icr/v20211014/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/icr/v20211014/icr_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/icr/v20211014/icr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/rkp/v20191209/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/rkp/v20191209/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/rkp/v20191209/rkp_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/rkp/v20191209/rkp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/rkp/v20191209/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/rkp/v20191209/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/hcm/v20181106/hcm_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/hcm/v20181106/hcm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/hcm/v20181106/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/hcm/v20181106/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/hcm/v20181106/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/hcm/v20181106/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mna/v20210119/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mna/v20210119/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mna/v20210119/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mna/v20210119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mna/v20210119/mna_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mna/v20210119/mna_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cdwpg/v20201230/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cdwpg/v20201230/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cdwpg/v20201230/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cdwpg/v20201230/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cdwpg/v20201230/cdwpg_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cdwpg/v20201230/cdwpg_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/v20201215/iotvideo_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/v20201215/iotvideo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/v20201215/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/v20201215/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/v20201215/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/v20201215/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/v20191126/iotvideo_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/v20191126/iotvideo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/v20191126/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/v20191126/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/v20191126/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/v20191126/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/v20211125/iotvideo_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/v20211125/iotvideo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/v20211125/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/v20211125/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideo/v20211125/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideo/v20211125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mongodb/v20180408/mongodb_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mongodb/v20180408/mongodb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mongodb/v20180408/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mongodb/v20180408/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mongodb/v20180408/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mongodb/v20180408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mongodb/v20190725/mongodb_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mongodb/v20190725/mongodb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mongodb/v20190725/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mongodb/v20190725/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mongodb/v20190725/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mongodb/v20190725/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iot/v20180123/iot_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iot/v20180123/iot_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iot/v20180123/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iot/v20180123/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iot/v20180123/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iot/v20180123/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/vm/v20201229/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/vm/v20201229/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/vm/v20201229/vm_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/vm/v20201229/vm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/vm/v20201229/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/vm/v20201229/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/vm/v20210922/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/vm/v20210922/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/vm/v20210922/vm_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/vm/v20210922/vm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/vm/v20210922/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/vm/v20210922/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/vm/v20200709/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/vm/v20200709/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/vm/v20200709/vm_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/vm/v20200709/vm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/vm/v20200709/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/vm/v20200709/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ams/v20201229/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ams/v20201229/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ams/v20201229/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ams/v20201229/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ams/v20201229/ams_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ams/v20201229/ams_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ams/v20200608/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ams/v20200608/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ams/v20200608/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ams/v20200608/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ams/v20200608/ams_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ams/v20200608/ams_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tcm/v20210413/tcm_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tcm/v20210413/tcm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tcm/v20210413/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tcm/v20210413/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tcm/v20210413/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tcm/v20210413/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tav/v20190118/tav_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tav/v20190118/tav_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tav/v20190118/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tav/v20190118/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tav/v20190118/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tav/v20190118/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/sslpod/v20190605/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/sslpod/v20190605/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/sslpod/v20190605/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/sslpod/v20190605/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/sslpod/v20190605/sslpod_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/sslpod/v20190605/sslpod_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bmlb/v20180625/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bmlb/v20180625/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bmlb/v20180625/bmlb_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bmlb/v20180625/bmlb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bmlb/v20180625/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bmlb/v20180625/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/wss/v20180426/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/wss/v20180426/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/wss/v20180426/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/wss/v20180426/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/wss/v20180426/wss_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/wss/v20180426/wss_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cfg/v20210820/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cfg/v20210820/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cfg/v20210820/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cfg/v20210820/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cfg/v20210820/cfg_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cfg/v20210820/cfg_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/aa/v20200224/aa_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/aa/v20200224/aa_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/aa/v20200224/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/aa/v20200224/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/aa/v20200224/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/aa/v20200224/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/vpc/v20170312/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/vpc/v20170312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/vpc/v20170312/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/vpc/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/vpc/v20170312/vpc_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/vpc/v20170312/vpc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideoindustry/v20201201/iotvideoindustry_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideoindustry/v20201201/iotvideoindustry_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideoindustry/v20201201/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideoindustry/v20201201/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iotvideoindustry/v20201201/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iotvideoindustry/v20201201/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mps/v20190612/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mps/v20190612/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mps/v20190612/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mps/v20190612/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mps/v20190612/mps_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mps/v20190612/mps_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ape/v20200513/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ape/v20200513/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ape/v20200513/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ape/v20200513/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ape/v20200513/ape_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ape/v20200513/ape_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tcaplusdb/v20190823/tcaplusdb_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tcaplusdb/v20190823/tcaplusdb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tcaplusdb/v20190823/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tcaplusdb/v20190823/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tcaplusdb/v20190823/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tcaplusdb/v20190823/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dayu/v20180709/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dayu/v20180709/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dayu/v20180709/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dayu/v20180709/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dayu/v20180709/dayu_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dayu/v20180709/dayu_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/weilingwith/v20230427/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/weilingwith/v20230427/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/weilingwith/v20230427/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/weilingwith/v20230427/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/weilingwith/v20230427/weilingwith_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/weilingwith/v20230427/weilingwith_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/scf/v20180416/scf_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/scf/v20180416/scf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/scf/v20180416/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/scf/v20180416/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -1516,15 +1516,15 @@
 
     def __init__(self):
         r"""
         :param _FunctionName: 新建触发器绑定的函数名称
         :type FunctionName: str
         :param _TriggerName: 新建触发器名称。如果是定时触发器，名称支持英文字母、数字、连接符和下划线，最长100个字符；如果是cos触发器，需要是对应cos存储桶适用于XML API的访问域名(例如:5401-5ff414-12345.cos.ap-shanghai.myqcloud.com);如果是其他触发器，见具体触发器绑定参数的说明
         :type TriggerName: str
-        :param _Type: 触发器类型，目前支持 cos 、cmq、 timer、 ckafka、apigw类型。创建 cls 触发器请参考[CLS 创建投递 SCF 任务](https://cloud.tencent.com/document/product/614/61096)。
+        :param _Type: 触发器类型，目前支持 cos 、cmq、 timer、 ckafka、apigw类型。创建函数URL请在此填写 http 。创建 cls 触发器请参考[CLS 创建投递 SCF 任务](https://cloud.tencent.com/document/product/614/61096)。
         :type Type: str
         :param _TriggerDesc: 触发器对应的参数，可见具体[触发器描述说明](https://cloud.tencent.com/document/product/583/39901)
         :type TriggerDesc: str
         :param _Namespace: 函数的命名空间
         :type Namespace: str
         :param _Qualifier: 函数的版本，默认为 $LATEST，建议填写 [$DEFAULT](https://cloud.tencent.com/document/product/583/36149#.E9.BB.98.E8.AE.A4.E5.88.AB.E5.90.8D)方便后续进行版本的灰度发布。
         :type Qualifier: str
```

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/scf/v20180416/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/scf/v20180416/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/lp/v20200224/lp_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/lp/v20200224/lp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/lp/v20200224/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/lp/v20200224/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/lp/v20200224/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/lp/v20200224/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cim/v20190318/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cim/v20190318/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cim/v20190318/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cim/v20190318/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cim/v20190318/cim_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cim/v20190318/cim_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/lighthouse/v20200324/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/lighthouse/v20200324/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/lighthouse/v20200324/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/lighthouse/v20200324/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/lighthouse/v20200324/lighthouse_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/lighthouse/v20200324/lighthouse_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/keewidb/v20220308/keewidb_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/keewidb/v20220308/keewidb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/keewidb/v20220308/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/keewidb/v20220308/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/keewidb/v20220308/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/keewidb/v20220308/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tdcpg/v20211118/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tdcpg/v20211118/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tdcpg/v20211118/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tdcpg/v20211118/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tdcpg/v20211118/tdcpg_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tdcpg/v20211118/tdcpg_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cdwch/v20200915/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cdwch/v20200915/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cdwch/v20200915/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cdwch/v20200915/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cdwch/v20200915/cdwch_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cdwch/v20200915/cdwch_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cloudstudio/v20210524/cloudstudio_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cloudstudio/v20210524/cloudstudio_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cloudstudio/v20210524/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cloudstudio/v20210524/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cloudstudio/v20210524/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cloudstudio/v20210524/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cloudstudio/v20230508/cloudstudio_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cloudstudio/v20230508/cloudstudio_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cloudstudio/v20230508/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cloudstudio/v20230508/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cloudstudio/v20230508/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cloudstudio/v20230508/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/msp/v20180319/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/msp/v20180319/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/msp/v20180319/msp_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/msp/v20180319/msp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/msp/v20180319/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/msp/v20180319/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/memcached/v20190318/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/memcached/v20190318/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/memcached/v20190318/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/memcached/v20190318/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/memcached/v20190318/memcached_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/memcached/v20190318/memcached_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bpaas/v20181217/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bpaas/v20181217/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bpaas/v20181217/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bpaas/v20181217/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bpaas/v20181217/bpaas_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bpaas/v20181217/bpaas_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tbm/v20180129/tbm_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tbm/v20180129/tbm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tbm/v20180129/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tbm/v20180129/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tbm/v20180129/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tbm/v20180129/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/trro/v20220325/trro_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/trro/v20220325/trro_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/trro/v20220325/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/trro/v20220325/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/trro/v20220325/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/trro/v20220325/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/smh/v20210712/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/smh/v20210712/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/smh/v20210712/smh_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/smh/v20210712/smh_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/smh/v20210712/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/smh/v20210712/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/kms/v20190118/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/kms/v20190118/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/kms/v20190118/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/kms/v20190118/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/kms/v20190118/kms_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/kms/v20190118/kms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/habo/v20181203/habo_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/habo/v20181203/habo_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/habo/v20181203/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/habo/v20181203/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/habo/v20181203/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/habo/v20181203/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/omics/v20221128/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/omics/v20221128/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/omics/v20221128/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/omics/v20221128/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/omics/v20221128/omics_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/omics/v20221128/omics_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tkgdq/v20190411/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tkgdq/v20190411/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tkgdq/v20190411/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tkgdq/v20190411/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tkgdq/v20190411/tkgdq_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tkgdq/v20190411/tkgdq_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/eiam/v20210420/eiam_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/eiam/v20210420/eiam_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/eiam/v20210420/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/eiam/v20210420/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/eiam/v20210420/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/eiam/v20210420/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/rce/v20201103/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/rce/v20201103/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/rce/v20201103/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/rce/v20201103/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/rce/v20201103/rce_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/rce/v20201103/rce_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/privatedns/v20201028/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/privatedns/v20201028/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/privatedns/v20201028/privatedns_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/privatedns/v20201028/privatedns_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/privatedns/v20201028/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/privatedns/v20201028/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tsf/v20180326/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tsf/v20180326/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tsf/v20180326/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tsf/v20180326/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tsf/v20180326/tsf_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tsf/v20180326/tsf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iottid/v20190411/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iottid/v20190411/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iottid/v20190411/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iottid/v20190411/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iottid/v20190411/iottid_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iottid/v20190411/iottid_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dc/v20180410/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dc/v20180410/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dc/v20180410/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dc/v20180410/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dc/v20180410/dc_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dc/v20180410/dc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/wav/v20210129/wav_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/wav/v20210129/wav_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/wav/v20210129/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/wav/v20210129/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/wav/v20210129/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/wav/v20210129/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cloudaudit/v20190319/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cloudaudit/v20190319/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cloudaudit/v20190319/cloudaudit_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cloudaudit/v20190319/cloudaudit_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cloudaudit/v20190319/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cloudaudit/v20190319/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/rum/v20210622/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/rum/v20210622/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/rum/v20210622/rum_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/rum/v20210622/rum_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/rum/v20210622/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/rum/v20210622/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tdmq/v20200217/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tdmq/v20200217/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tdmq/v20200217/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tdmq/v20200217/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tdmq/v20200217/tdmq_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tdmq/v20200217/tdmq_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dnspod/v20210323/dnspod_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dnspod/v20210323/dnspod_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dnspod/v20210323/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dnspod/v20210323/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dnspod/v20210323/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dnspod/v20210323/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/eis/v20200715/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/eis/v20200715/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/eis/v20200715/eis_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/eis/v20200715/eis_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/eis/v20200715/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/eis/v20200715/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/eis/v20210601/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/eis/v20210601/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/eis/v20210601/eis_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/eis/v20210601/eis_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/eis/v20210601/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/eis/v20210601/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tbp/v20190627/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tbp/v20190627/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tbp/v20190627/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tbp/v20190627/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tbp/v20190627/tbp_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tbp/v20190627/tbp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tbp/v20190311/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tbp/v20190311/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tbp/v20190311/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tbp/v20190311/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tbp/v20190311/tbp_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tbp/v20190311/tbp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/live/v20180801/live_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/live/v20180801/live_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/live/v20180801/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/live/v20180801/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/live/v20180801/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/live/v20180801/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mall/v20230518/mall_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mall/v20230518/mall_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mall/v20230518/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mall/v20230518/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mall/v20230518/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mall/v20230518/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cmq/v20190304/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cmq/v20190304/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cmq/v20190304/cmq_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cmq/v20190304/cmq_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cmq/v20190304/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cmq/v20190304/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tcb/v20180608/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tcb/v20180608/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tcb/v20180608/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tcb/v20180608/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tcb/v20180608/tcb_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tcb/v20180608/tcb_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cws/v20180312/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cws/v20180312/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cws/v20180312/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cws/v20180312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cws/v20180312/cws_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cws/v20180312/cws_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/billing/v20180709/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/billing/v20180709/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/billing/v20180709/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/billing/v20180709/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/billing/v20180709/billing_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/billing/v20180709/billing_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tchd/v20230306/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tchd/v20230306/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tchd/v20230306/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tchd/v20230306/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tchd/v20230306/tchd_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tchd/v20230306/tchd_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dtf/v20200506/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dtf/v20200506/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dtf/v20200506/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dtf/v20200506/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dtf/v20200506/dtf_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dtf/v20200506/dtf_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cfw/v20190904/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cfw/v20190904/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cfw/v20190904/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cfw/v20190904/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cfw/v20190904/cfw_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cfw/v20190904/cfw_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/emr/v20190103/emr_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/emr/v20190103/emr_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -115,14 +115,37 @@
         except Exception as e:
             if isinstance(e, TencentCloudSDKException):
                 raise
             else:
                 raise TencentCloudSDKException(type(e).__name__, str(e))
 
 
+    def DescribeAutoScaleRecords(self, request):
+        """获取集群的自动扩缩容的详细记录
+
+        :param request: Request instance for DescribeAutoScaleRecords.
+        :type request: :class:`tencentcloud.emr.v20190103.models.DescribeAutoScaleRecordsRequest`
+        :rtype: :class:`tencentcloud.emr.v20190103.models.DescribeAutoScaleRecordsResponse`
+
+        """
+        try:
+            params = request._serialize()
+            headers = request.headers
+            body = self.call("DescribeAutoScaleRecords", params, headers=headers)
+            response = json.loads(body)
+            model = models.DescribeAutoScaleRecordsResponse()
+            model._deserialize(response["Response"])
+            return model
+        except Exception as e:
+            if isinstance(e, TencentCloudSDKException):
+                raise
+            else:
+                raise TencentCloudSDKException(type(e).__name__, str(e))
+
+
     def DescribeClusterNodes(self, request):
         """查询集群节点信息
 
         :param request: Request instance for DescribeClusterNodes.
         :type request: :class:`tencentcloud.emr.v20190103.models.DescribeClusterNodesRequest`
         :rtype: :class:`tencentcloud.emr.v20190103.models.DescribeClusterNodesResponse`
```

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/emr/v20190103/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/emr/v20190103/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -365,14 +365,169 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class AutoScaleRecord(AbstractModel):
+    """弹性扩缩容记录
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _StrategyName: 扩缩容规则名。
+        :type StrategyName: str
+        :param _ScaleAction: "SCALE_OUT"和"SCALE_IN"，分别表示扩容和缩容。
+        :type ScaleAction: str
+        :param _ActionStatus: 取值为"SUCCESS","FAILED","PART_SUCCESS","IN_PROCESS"，分别表示成功、失败、部分成功和流程中。
+        :type ActionStatus: str
+        :param _ActionTime: 流程触发时间。
+        :type ActionTime: str
+        :param _ScaleInfo: 扩缩容相关描述信息。
+        :type ScaleInfo: str
+        :param _ExpectScaleNum: 只在ScaleAction为SCALE_OUT时有效。
+        :type ExpectScaleNum: int
+        :param _EndTime: 流程结束时间。
+        :type EndTime: str
+        :param _StrategyType: 策略类型，按负载或者按时间，1表示负载伸缩，2表示时间伸缩
+        :type StrategyType: int
+        :param _SpecInfo: 扩容时所使用规格信息。
+        :type SpecInfo: str
+        :param _CompensateFlag: 补偿扩容，0表示不开启，1表示开启
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CompensateFlag: int
+        :param _CompensateCount: 补偿次数
+注意：此字段可能返回 null，表示取不到有效值。
+        :type CompensateCount: int
+        """
+        self._StrategyName = None
+        self._ScaleAction = None
+        self._ActionStatus = None
+        self._ActionTime = None
+        self._ScaleInfo = None
+        self._ExpectScaleNum = None
+        self._EndTime = None
+        self._StrategyType = None
+        self._SpecInfo = None
+        self._CompensateFlag = None
+        self._CompensateCount = None
+
+    @property
+    def StrategyName(self):
+        return self._StrategyName
+
+    @StrategyName.setter
+    def StrategyName(self, StrategyName):
+        self._StrategyName = StrategyName
+
+    @property
+    def ScaleAction(self):
+        return self._ScaleAction
+
+    @ScaleAction.setter
+    def ScaleAction(self, ScaleAction):
+        self._ScaleAction = ScaleAction
+
+    @property
+    def ActionStatus(self):
+        return self._ActionStatus
+
+    @ActionStatus.setter
+    def ActionStatus(self, ActionStatus):
+        self._ActionStatus = ActionStatus
+
+    @property
+    def ActionTime(self):
+        return self._ActionTime
+
+    @ActionTime.setter
+    def ActionTime(self, ActionTime):
+        self._ActionTime = ActionTime
+
+    @property
+    def ScaleInfo(self):
+        return self._ScaleInfo
+
+    @ScaleInfo.setter
+    def ScaleInfo(self, ScaleInfo):
+        self._ScaleInfo = ScaleInfo
+
+    @property
+    def ExpectScaleNum(self):
+        return self._ExpectScaleNum
+
+    @ExpectScaleNum.setter
+    def ExpectScaleNum(self, ExpectScaleNum):
+        self._ExpectScaleNum = ExpectScaleNum
+
+    @property
+    def EndTime(self):
+        return self._EndTime
+
+    @EndTime.setter
+    def EndTime(self, EndTime):
+        self._EndTime = EndTime
+
+    @property
+    def StrategyType(self):
+        return self._StrategyType
+
+    @StrategyType.setter
+    def StrategyType(self, StrategyType):
+        self._StrategyType = StrategyType
+
+    @property
+    def SpecInfo(self):
+        return self._SpecInfo
+
+    @SpecInfo.setter
+    def SpecInfo(self, SpecInfo):
+        self._SpecInfo = SpecInfo
+
+    @property
+    def CompensateFlag(self):
+        return self._CompensateFlag
+
+    @CompensateFlag.setter
+    def CompensateFlag(self, CompensateFlag):
+        self._CompensateFlag = CompensateFlag
+
+    @property
+    def CompensateCount(self):
+        return self._CompensateCount
+
+    @CompensateCount.setter
+    def CompensateCount(self, CompensateCount):
+        self._CompensateCount = CompensateCount
+
+
+    def _deserialize(self, params):
+        self._StrategyName = params.get("StrategyName")
+        self._ScaleAction = params.get("ScaleAction")
+        self._ActionStatus = params.get("ActionStatus")
+        self._ActionTime = params.get("ActionTime")
+        self._ScaleInfo = params.get("ScaleInfo")
+        self._ExpectScaleNum = params.get("ExpectScaleNum")
+        self._EndTime = params.get("EndTime")
+        self._StrategyType = params.get("StrategyType")
+        self._SpecInfo = params.get("SpecInfo")
+        self._CompensateFlag = params.get("CompensateFlag")
+        self._CompensateCount = params.get("CompensateCount")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
 class BootstrapAction(AbstractModel):
     """引导脚本
 
     """
 
     def __init__(self):
         r"""
@@ -2924,14 +3079,142 @@
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
+class DescribeAutoScaleRecordsRequest(AbstractModel):
+    """DescribeAutoScaleRecords请求参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _InstanceId: 实例ID。
+        :type InstanceId: str
+        :param _Filters: 记录过滤参数，目前仅能为“StartTime”,“EndTime”和“StrategyName”。StartTime和EndTime支持2006-01-02 15:04:05 或者2006/01/02 15:04:05的时间格式
+        :type Filters: list of KeyValue
+        :param _Offset: 分页参数。
+        :type Offset: int
+        :param _Limit: 分页参数。最大支持100
+        :type Limit: int
+        """
+        self._InstanceId = None
+        self._Filters = None
+        self._Offset = None
+        self._Limit = None
+
+    @property
+    def InstanceId(self):
+        return self._InstanceId
+
+    @InstanceId.setter
+    def InstanceId(self, InstanceId):
+        self._InstanceId = InstanceId
+
+    @property
+    def Filters(self):
+        return self._Filters
+
+    @Filters.setter
+    def Filters(self, Filters):
+        self._Filters = Filters
+
+    @property
+    def Offset(self):
+        return self._Offset
+
+    @Offset.setter
+    def Offset(self, Offset):
+        self._Offset = Offset
+
+    @property
+    def Limit(self):
+        return self._Limit
+
+    @Limit.setter
+    def Limit(self, Limit):
+        self._Limit = Limit
+
+
+    def _deserialize(self, params):
+        self._InstanceId = params.get("InstanceId")
+        if params.get("Filters") is not None:
+            self._Filters = []
+            for item in params.get("Filters"):
+                obj = KeyValue()
+                obj._deserialize(item)
+                self._Filters.append(obj)
+        self._Offset = params.get("Offset")
+        self._Limit = params.get("Limit")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class DescribeAutoScaleRecordsResponse(AbstractModel):
+    """DescribeAutoScaleRecords返回参数结构体
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _TotalCount: 总扩缩容记录数。
+        :type TotalCount: int
+        :param _RecordList: 记录列表。
+        :type RecordList: list of AutoScaleRecord
+        :param _RequestId: 唯一请求 ID，每次请求都会返回。定位问题时需要提供该次请求的 RequestId。
+        :type RequestId: str
+        """
+        self._TotalCount = None
+        self._RecordList = None
+        self._RequestId = None
+
+    @property
+    def TotalCount(self):
+        return self._TotalCount
+
+    @TotalCount.setter
+    def TotalCount(self, TotalCount):
+        self._TotalCount = TotalCount
+
+    @property
+    def RecordList(self):
+        return self._RecordList
+
+    @RecordList.setter
+    def RecordList(self, RecordList):
+        self._RecordList = RecordList
+
+    @property
+    def RequestId(self):
+        return self._RequestId
+
+    @RequestId.setter
+    def RequestId(self, RequestId):
+        self._RequestId = RequestId
+
+
+    def _deserialize(self, params):
+        self._TotalCount = params.get("TotalCount")
+        if params.get("RecordList") is not None:
+            self._RecordList = []
+            for item in params.get("RecordList"):
+                obj = AutoScaleRecord()
+                obj._deserialize(item)
+                self._RecordList.append(obj)
+        self._RequestId = params.get("RequestId")
+
+
 class DescribeClusterNodesRequest(AbstractModel):
     """DescribeClusterNodes请求参数结构体
 
     """
 
     def __init__(self):
         r"""
@@ -7861,14 +8144,61 @@
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
+        
+
+
+class KeyValue(AbstractModel):
+    """键值对，主要用来做Filter
+
+    """
+
+    def __init__(self):
+        r"""
+        :param _Key: 键
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Key: str
+        :param _Value: 值
+注意：此字段可能返回 null，表示取不到有效值。
+        :type Value: str
+        """
+        self._Key = None
+        self._Value = None
+
+    @property
+    def Key(self):
+        return self._Key
+
+    @Key.setter
+    def Key(self, Key):
+        self._Key = Key
+
+    @property
+    def Value(self):
+        return self._Value
+
+    @Value.setter
+    def Value(self, Value):
+        self._Value = Value
+
+
+    def _deserialize(self, params):
+        self._Key = params.get("Key")
+        self._Value = params.get("Value")
+        memeber_set = set(params.keys())
+        for name, value in vars(self).items():
+            property_name = name[1:]
+            if property_name in memeber_set:
+                memeber_set.remove(property_name)
+        if len(memeber_set) > 0:
+            warnings.warn("%s fileds are useless." % ",".join(memeber_set))
         
 
 
 class LoginSettings(AbstractModel):
     """登录设置
 
     """
```

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/emr/v20190103/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/emr/v20190103/errorcodes.py`

 * *Files 1% similar despite different names*

```diff
@@ -181,14 +181,17 @@
 
 # CustomConfig参数值无效。
 INVALIDPARAMETER_INVALIDEXTENDFIELD = 'InvalidParameter.InvalidExtendField'
 
 # 无效的任务失败处理策略。
 INVALIDPARAMETER_INVALIDFAILUREPOLICY = 'InvalidParameter.InvalidFailurePolicy'
 
+# 无效过滤参数。
+INVALIDPARAMETER_INVALIDFILTERKEY = 'InvalidParameter.InvalidFilterKey'
+
 # 无效参数，EMR实例不符合要求。
 INVALIDPARAMETER_INVALIDINSTANCE = 'InvalidParameter.InvalidInstance'
 
 # 不合法的实例计费模式。
 INVALIDPARAMETER_INVALIDINSTANCECHARGETYPE = 'InvalidParameter.InvalidInstanceChargeType'
 
 # 无效的集群名称。
@@ -283,14 +286,17 @@
 
 # 软件名无效。
 INVALIDPARAMETER_INVALIDSOFTWARENAME = 'InvalidParameter.InvalidSoftWareName'
 
 # 软件版本无效。
 INVALIDPARAMETER_INVALIDSOFTWAREVERSION = 'InvalidParameter.InvalidSoftWareVersion'
 
+# invalid Parameter StartTime or EndTime.参数无效
+INVALIDPARAMETER_INVALIDSTARTTIMEORENDTIME = 'InvalidParameter.InvalidStartTimeOrEndTime'
+
 # 无效的子网ID。
 INVALIDPARAMETER_INVALIDSUBNETID = 'InvalidParameter.InvalidSubnetId'
 
 # 无效的高可用参数。
 INVALIDPARAMETER_INVALIDSUPPORTHA = 'InvalidParameter.InvalidSupportHA'
 
 # 参数错误。
```

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/trocket/v20230308/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/trocket/v20230308/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/trocket/v20230308/trocket_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/trocket/v20230308/trocket_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/trocket/v20230308/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/trocket/v20230308/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/sqlserver/v20180328/sqlserver_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/sqlserver/v20180328/sqlserver_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/sqlserver/v20180328/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/sqlserver/v20180328/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/sqlserver/v20180328/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/sqlserver/v20180328/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mgobe/v20201014/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mgobe/v20201014/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mgobe/v20201014/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mgobe/v20201014/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mgobe/v20201014/mgobe_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mgobe/v20201014/mgobe_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mgobe/v20190929/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mgobe/v20190929/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mgobe/v20190929/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mgobe/v20190929/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/mgobe/v20190929/mgobe_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/mgobe/v20190929/mgobe_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/essbasic/v20201222/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/essbasic/v20201222/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/essbasic/v20201222/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/essbasic/v20201222/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/essbasic/v20201222/essbasic_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/essbasic/v20201222/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/essbasic/v20210526/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/essbasic/v20210526/models.py`

 * *Files 0% similar despite different names*

```diff
@@ -7147,14 +7147,21 @@
         :type ComponentPosX: float
         :param _ComponentPosY: 参数控件Y位置，单位px
         :type ComponentPosY: float
         :param _ComponentExtra: 扩展参数：
 为JSON格式。
 不同类型的控件会有部分非通用参数
 
+ComponentType为TEXT、MULTI_LINE_TEXT时，支持以下参数：
+1 Font：目前只支持黑体、宋体
+2 FontSize： 范围12-72
+3 FontAlign： Left/Right/Center，左对齐/居中/右对齐
+4 FontColor：字符串类型，格式为RGB颜色数字
+参数样例：    "ComponentExtra": "{\"FontColor\":\"255,0,0\",\"FontSize\":12}"
+
 TEXT/MULTI_LINE_TEXT控件可以指定
 1 Font：目前只支持黑体、宋体
 2 FontSize： 范围12-72
 3 FontAlign： Left/Right/Center，左对齐/居中/右对齐
 例如：{"FontSize":12}
 
 ComponentType为FILL_IMAGE时，支持以下参数：
```

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/essbasic/v20210526/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/essbasic/v20210526/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/essbasic/v20210526/essbasic_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/essbasic/v20210526/essbasic_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cms/v20190321/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cms/v20190321/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cms/v20190321/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cms/v20190321/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cms/v20190321/cms_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cms/v20190321/cms_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cwp/v20180228/cwp_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cwp/v20180228/cwp_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cwp/v20180228/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cwp/v20180228/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cwp/v20180228/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cwp/v20180228/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tione/v20191022/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tione/v20191022/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tione/v20191022/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tione/v20191022/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tione/v20191022/tione_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tione/v20191022/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tione/v20211111/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tione/v20211111/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tione/v20211111/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tione/v20211111/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tione/v20211111/tione_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tione/v20211111/tione_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cdn/v20180606/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cdn/v20180606/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cdn/v20180606/cdn_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cdn/v20180606/cdn_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cdn/v20180606/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cdn/v20180606/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ivld/v20210903/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ivld/v20210903/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ivld/v20210903/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ivld/v20210903/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ivld/v20210903/ivld_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ivld/v20210903/ivld_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/drm/v20181115/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/drm/v20181115/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/drm/v20181115/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/drm/v20181115/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/drm/v20181115/drm_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/drm/v20181115/drm_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tiia/v20190529/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tiia/v20190529/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tiia/v20190529/tiia_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tiia/v20190529/tiia_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tiia/v20190529/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tiia/v20190529/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ocr/v20181119/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ocr/v20181119/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ocr/v20181119/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ocr/v20181119/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/ocr/v20181119/ocr_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/ocr/v20181119/ocr_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/trtc/v20190722/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/trtc/v20190722/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/trtc/v20190722/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/trtc/v20190722/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/trtc/v20190722/trtc_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/trtc/v20190722/trtc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iotcloud/v20210408/iotcloud_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iotcloud/v20210408/iotcloud_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iotcloud/v20210408/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iotcloud/v20210408/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iotcloud/v20210408/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iotcloud/v20210408/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iotcloud/v20180614/iotcloud_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iotcloud/v20180614/iotcloud_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iotcloud/v20180614/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iotcloud/v20180614/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iotcloud/v20180614/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iotcloud/v20180614/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/soe/v20180724/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/soe/v20180724/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -1363,14 +1363,16 @@
         :type IsQuery: int
         :param _TextMode: 输入文本模式
 0: 普通文本（默认）
 1：[音素结构](https://cloud.tencent.com/document/product/884/33698)文本
         :type TextMode: int
         :param _Keyword: 主题词和关键词
         :type Keyword: str
+        :param _COSBucketURL: 音频存储路径，支持通过子路径指定文件夹名称
+        :type COSBucketURL: str
         """
         self._SeqId = None
         self._IsEnd = None
         self._VoiceFileType = None
         self._VoiceEncodeType = None
         self._UserVoiceData = None
         self._SessionId = None
@@ -1382,14 +1384,15 @@
         self._StorageMode = None
         self._SentenceInfoEnabled = None
         self._ServerType = None
         self._IsAsync = None
         self._IsQuery = None
         self._TextMode = None
         self._Keyword = None
+        self._COSBucketURL = None
 
     @property
     def SeqId(self):
         return self._SeqId
 
     @SeqId.setter
     def SeqId(self, SeqId):
@@ -1473,18 +1476,22 @@
 
     @SoeAppId.setter
     def SoeAppId(self, SoeAppId):
         self._SoeAppId = SoeAppId
 
     @property
     def StorageMode(self):
+        warnings.warn("parameter `StorageMode` is deprecated", DeprecationWarning) 
+
         return self._StorageMode
 
     @StorageMode.setter
     def StorageMode(self, StorageMode):
+        warnings.warn("parameter `StorageMode` is deprecated", DeprecationWarning) 
+
         self._StorageMode = StorageMode
 
     @property
     def SentenceInfoEnabled(self):
         return self._SentenceInfoEnabled
 
     @SentenceInfoEnabled.setter
@@ -1527,14 +1534,22 @@
     def Keyword(self):
         return self._Keyword
 
     @Keyword.setter
     def Keyword(self, Keyword):
         self._Keyword = Keyword
 
+    @property
+    def COSBucketURL(self):
+        return self._COSBucketURL
+
+    @COSBucketURL.setter
+    def COSBucketURL(self, COSBucketURL):
+        self._COSBucketURL = COSBucketURL
+
 
     def _deserialize(self, params):
         self._SeqId = params.get("SeqId")
         self._IsEnd = params.get("IsEnd")
         self._VoiceFileType = params.get("VoiceFileType")
         self._VoiceEncodeType = params.get("VoiceEncodeType")
         self._UserVoiceData = params.get("UserVoiceData")
@@ -1547,14 +1562,15 @@
         self._StorageMode = params.get("StorageMode")
         self._SentenceInfoEnabled = params.get("SentenceInfoEnabled")
         self._ServerType = params.get("ServerType")
         self._IsAsync = params.get("IsAsync")
         self._IsQuery = params.get("IsQuery")
         self._TextMode = params.get("TextMode")
         self._Keyword = params.get("Keyword")
+        self._COSBucketURL = params.get("COSBucketURL")
         memeber_set = set(params.keys())
         for name, value in vars(self).items():
             property_name = name[1:]
             if property_name in memeber_set:
                 memeber_set.remove(property_name)
         if len(memeber_set) > 0:
             warnings.warn("%s fileds are useless." % ",".join(memeber_set))
@@ -1650,18 +1666,22 @@
 
     @SessionId.setter
     def SessionId(self, SessionId):
         self._SessionId = SessionId
 
     @property
     def AudioUrl(self):
+        warnings.warn("parameter `AudioUrl` is deprecated", DeprecationWarning) 
+
         return self._AudioUrl
 
     @AudioUrl.setter
     def AudioUrl(self, AudioUrl):
+        warnings.warn("parameter `AudioUrl` is deprecated", DeprecationWarning) 
+
         self._AudioUrl = AudioUrl
 
     @property
     def SentenceInfoSet(self):
         return self._SentenceInfoSet
 
     @SentenceInfoSet.setter
```

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/soe/v20180724/soe_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/soe/v20180724/soe_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/soe/v20180724/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/soe/v20180724/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/aiart/v20221229/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/aiart/v20221229/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/aiart/v20221229/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/aiart/v20221229/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/aiart/v20221229/aiart_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/aiart/v20221229/aiart_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/yunsou/v20191115/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/yunsou/v20191115/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/yunsou/v20191115/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/yunsou/v20191115/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/yunsou/v20191115/yunsou_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/yunsou/v20191115/yunsou_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/yunsou/v20180504/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/yunsou/v20180504/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/yunsou/v20180504/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/yunsou/v20180504/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/yunsou/v20180504/yunsou_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/yunsou/v20180504/yunsou_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/apcas/v20201127/apcas_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/apcas/v20201127/apcas_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/apcas/v20201127/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/apcas/v20201127/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/apcas/v20201127/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/apcas/v20201127/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bi/v20220105/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bi/v20220105/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bi/v20220105/bi_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bi/v20220105/bi_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/bi/v20220105/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/bi/v20220105/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tiw/v20190919/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tiw/v20190919/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tiw/v20190919/tiw_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tiw/v20190919/tiw_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/tiw/v20190919/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/tiw/v20190919/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dlc/v20210125/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dlc/v20210125/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dlc/v20210125/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dlc/v20210125/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/dlc/v20210125/dlc_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/dlc/v20210125/dlc_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iir/v20200417/iir_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iir/v20200417/iir_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iir/v20200417/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iir/v20200417/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/iir/v20200417/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/iir/v20200417/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cls/v20201016/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cls/v20201016/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cls/v20201016/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cls/v20201016/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/cls/v20201016/cls_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/cls/v20201016/cls_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/sts/v20180813/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/sts/v20180813/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/sts/v20180813/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/sts/v20180813/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/sts/v20180813/sts_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/sts/v20180813/sts_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/batch/v20170312/batch_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/batch/v20170312/batch_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/batch/v20170312/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/batch/v20170312/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -1584,17 +1584,17 @@
 该参数目前仅用于 `RunInstances` 接口。
 注意：此字段可能返回 null，表示取不到有效值。
         :type DeleteWithInstance: bool
         :param _SnapshotId: 数据盘快照ID。选择的数据盘快照大小需小于数据盘大小。
 注意：此字段可能返回 null，表示取不到有效值。
         :type SnapshotId: str
         :param _Encrypt: 数据盘是加密。取值范围：
-<li>TRUE：加密
-<li>FALSE：不加密<br>
-默认取值：FALSE<br>
+<li>true：加密
+<li>false：不加密<br>
+默认取值：false<br>
 该参数目前仅用于 `RunInstances` 接口。
 注意：此字段可能返回 null，表示取不到有效值。
         :type Encrypt: bool
         :param _KmsKeyId: 自定义CMK对应的ID，取值为UUID或者类似kms-abcd1234。用于加密云盘。
 
 该参数目前仅用于 `RunInstances` 接口。
 注意：此字段可能返回 null，表示取不到有效值。
@@ -7762,15 +7762,15 @@
 class RunAutomationServiceEnabled(AbstractModel):
     """描述了 “云自动化助手” 服务相关的信息
 
     """
 
     def __init__(self):
         r"""
-        :param _Enabled: 是否开启云自动化助手。取值范围：<br><li>TRUE：表示开启云自动化助手服务<br><li>FALSE：表示不开启云自动化助手服务<br><br>默认取值：FALSE。
+        :param _Enabled: 是否开启云自动化助手。取值范围：<br><li>true：表示开启云自动化助手服务<br><li>false：表示不开启云自动化助手服务<br><br>默认取值：false。
         :type Enabled: bool
         """
         self._Enabled = None
 
     @property
     def Enabled(self):
         return self._Enabled
@@ -7795,15 +7795,16 @@
 class RunMonitorServiceEnabled(AbstractModel):
     """描述了 “云监控” 服务相关的信息
 
     """
 
     def __init__(self):
         r"""
-        :param _Enabled: 是否开启[云监控](/document/product/248)服务。取值范围：<br><li>TRUE：表示开启云监控服务<br><li>FALSE：表示不开启云监控服务<br><br>默认取值：TRUE。
+        :param _Enabled: 是否开启[云监控](/document/product/248)服务。取值范围：<br><li>true：表示开启云监控服务<br><li>false：表示不开启云监控服务<br><br>默认取值：true。
+注意：此字段可能返回 null，表示取不到有效值。
         :type Enabled: bool
         """
         self._Enabled = None
 
     @property
     def Enabled(self):
         return self._Enabled
@@ -9412,15 +9413,15 @@
 
     def __init__(self):
         r"""
         :param _VpcId: 私有网络ID，形如`vpc-xxx`。有效的VpcId可通过登录[控制台](https://console.cloud.tencent.com/vpc/vpc?rid=1)查询；也可以调用接口 [DescribeVpcEx](/document/api/215/1372) ，从接口返回中的`unVpcId`字段获取。若在创建子机时VpcId与SubnetId同时传入`DEFAULT`，则强制使用默认vpc网络。
         :type VpcId: str
         :param _SubnetId: 私有网络子网ID，形如`subnet-xxx`。有效的私有网络子网ID可通过登录[控制台](https://console.cloud.tencent.com/vpc/subnet?rid=1)查询；也可以调用接口  [DescribeSubnets](/document/api/215/15784) ，从接口返回中的`unSubnetId`字段获取。若在创建子机时SubnetId与VpcId同时传入`DEFAULT`，则强制使用默认vpc网络。
         :type SubnetId: str
-        :param _AsVpcGateway: 是否用作公网网关。公网网关只有在实例拥有公网IP以及处于私有网络下时才能正常使用。取值范围：<br><li>TRUE：表示用作公网网关<br><li>FALSE：表示不作为公网网关<br><br>默认取值：FALSE。
+        :param _AsVpcGateway: 是否用作公网网关。公网网关只有在实例拥有公网IP以及处于私有网络下时才能正常使用。取值范围：<br><li>true：表示用作公网网关<br><li>false：表示不作为公网网关<br><br>默认取值：false。
         :type AsVpcGateway: bool
         :param _PrivateIpAddresses: 私有网络子网 IP 数组，在创建实例、修改实例vpc属性操作中可使用此参数。当前仅批量创建多台实例时支持传入相同子网的多个 IP。
         :type PrivateIpAddresses: list of str
         :param _Ipv6AddressCount: 为弹性网卡指定随机生成的 IPv6 地址数量。
         :type Ipv6AddressCount: int
         """
         self._VpcId = None
```

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/batch/v20170312/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/batch/v20170312/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/pds/v20210701/models.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/pds/v20210701/models.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/pds/v20210701/errorcodes.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/pds/v20210701/errorcodes.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/tencentcloud/pds/v20210701/pds_client.py` & `tencentcloud-sdk-python-3.0.999/tencentcloud/pds/v20210701/pds_client.py`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/PKG-INFO` & `tencentcloud-sdk-python-3.0.999/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tencentcloud-sdk-python
-Version: 3.0.998
+Version: 3.0.999
 Summary: Tencent Cloud SDK for Python
 Home-page: https://github.com/TencentCloud/tencentcloud-sdk-python
 Author: Tencent Cloud
 Maintainer-email: tencentcloudapi@tencent.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `tencentcloud-sdk-python-3.0.998/README.rst` & `tencentcloud-sdk-python-3.0.999/README.rst`

 * *Files identical despite different names*

### Comparing `tencentcloud-sdk-python-3.0.998/setup.py` & `tencentcloud-sdk-python-3.0.999/setup.py`

 * *Files identical despite different names*

