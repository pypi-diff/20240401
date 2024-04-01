# Comparing `tmp/antchain_riskplus-1.9.3.tar.gz` & `tmp/antchain_riskplus-1.9.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/antchain_riskplus-1.9.3.tar", last modified: Mon Mar 28 07:37:27 2022, max compression
+gzip compressed data, was "dist/antchain_riskplus-1.9.5.tar", last modified: Fri Apr 15 08:37:40 2022, max compression
```

## Comparing `antchain_riskplus-1.9.3.tar` & `antchain_riskplus-1.9.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-28 07:37:27.000000 antchain_riskplus-1.9.3/
--rw-r--r--   0 root         (0) root         (0)      600 2022-03-28 07:37:25.000000 antchain_riskplus-1.9.3/LICENSE
--rw-r--r--   0 root         (0) root         (0)       29 2022-03-28 07:37:25.000000 antchain_riskplus-1.9.3/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     2200 2022-03-28 07:37:27.000000 antchain_riskplus-1.9.3/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      827 2022-03-28 07:37:25.000000 antchain_riskplus-1.9.3/README-CN.md
--rw-r--r--   0 root         (0) root         (0)     1013 2022-03-28 07:37:25.000000 antchain_riskplus-1.9.3/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-28 07:37:27.000000 antchain_riskplus-1.9.3/antchain_riskplus.egg-info/
--rw-r--r--   0 root         (0) root         (0)     2200 2022-03-28 07:37:26.000000 antchain_riskplus-1.9.3/antchain_riskplus.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      363 2022-03-28 07:37:26.000000 antchain_riskplus-1.9.3/antchain_riskplus.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2022-03-28 07:37:26.000000 antchain_riskplus-1.9.3/antchain_riskplus.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      107 2022-03-28 07:37:26.000000 antchain_riskplus-1.9.3/antchain_riskplus.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       22 2022-03-28 07:37:26.000000 antchain_riskplus-1.9.3/antchain_riskplus.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2022-03-28 07:37:27.000000 antchain_riskplus-1.9.3/antchain_sdk_riskplus/
--rw-r--r--   0 root         (0) root         (0)       21 2022-03-28 07:37:25.000000 antchain_riskplus-1.9.3/antchain_sdk_riskplus/__init__.py
--rw-r--r--   0 root         (0) root         (0)   208657 2022-03-28 07:37:25.000000 antchain_riskplus-1.9.3/antchain_sdk_riskplus/client.py
--rw-r--r--   0 root         (0) root         (0)   567907 2022-03-28 07:37:25.000000 antchain_riskplus-1.9.3/antchain_sdk_riskplus/models.py
--rw-r--r--   0 root         (0) root         (0)       73 2022-03-28 07:37:27.000000 antchain_riskplus-1.9.3/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     2513 2022-03-28 07:37:25.000000 antchain_riskplus-1.9.3/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-15 08:37:40.000000 antchain_riskplus-1.9.5/
+-rw-r--r--   0 root         (0) root         (0)      600 2022-04-15 08:37:39.000000 antchain_riskplus-1.9.5/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       29 2022-04-15 08:37:39.000000 antchain_riskplus-1.9.5/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     2200 2022-04-15 08:37:40.000000 antchain_riskplus-1.9.5/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      827 2022-04-15 08:37:39.000000 antchain_riskplus-1.9.5/README-CN.md
+-rw-r--r--   0 root         (0) root         (0)     1013 2022-04-15 08:37:39.000000 antchain_riskplus-1.9.5/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-15 08:37:40.000000 antchain_riskplus-1.9.5/antchain_riskplus.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     2200 2022-04-15 08:37:39.000000 antchain_riskplus-1.9.5/antchain_riskplus.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      363 2022-04-15 08:37:40.000000 antchain_riskplus-1.9.5/antchain_riskplus.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2022-04-15 08:37:39.000000 antchain_riskplus-1.9.5/antchain_riskplus.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      107 2022-04-15 08:37:39.000000 antchain_riskplus-1.9.5/antchain_riskplus.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       22 2022-04-15 08:37:39.000000 antchain_riskplus-1.9.5/antchain_riskplus.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2022-04-15 08:37:40.000000 antchain_riskplus-1.9.5/antchain_sdk_riskplus/
+-rw-r--r--   0 root         (0) root         (0)       21 2022-04-15 08:37:39.000000 antchain_riskplus-1.9.5/antchain_sdk_riskplus/__init__.py
+-rw-r--r--   0 root         (0) root         (0)   221413 2022-04-15 08:37:39.000000 antchain_riskplus-1.9.5/antchain_sdk_riskplus/client.py
+-rw-r--r--   0 root         (0) root         (0)   585931 2022-04-15 08:37:39.000000 antchain_riskplus-1.9.5/antchain_sdk_riskplus/models.py
+-rw-r--r--   0 root         (0) root         (0)       73 2022-04-15 08:37:40.000000 antchain_riskplus-1.9.5/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     2513 2022-04-15 08:37:39.000000 antchain_riskplus-1.9.5/setup.py
```

### Comparing `antchain_riskplus-1.9.3/LICENSE` & `antchain_riskplus-1.9.5/LICENSE`

 * *Files identical despite different names*

### Comparing `antchain_riskplus-1.9.3/PKG-INFO` & `antchain_riskplus-1.9.5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain_riskplus
-Version: 1.9.3
+Version: 1.9.5
 Summary: Ant Chain RISKPLUS SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_riskplus-1.9.3/README-CN.md` & `antchain_riskplus-1.9.5/README-CN.md`

 * *Files identical despite different names*

### Comparing `antchain_riskplus-1.9.3/README.md` & `antchain_riskplus-1.9.5/README.md`

 * *Files identical despite different names*

### Comparing `antchain_riskplus-1.9.3/antchain_riskplus.egg-info/PKG-INFO` & `antchain_riskplus-1.9.5/antchain_riskplus.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: antchain-riskplus
-Version: 1.9.3
+Version: 1.9.5
 Summary: Ant Chain RISKPLUS SDK Library for Python
 Home-page: https://github.com/alipay/antchain-openapi-prod-sdk
 Author: Ant Chain SDK
 Author-email: sdk-team@alibabacloud.com
 License: Apache License 2.0
 Description: English | [简体中文](README-CN.md)
```

### Comparing `antchain_riskplus-1.9.3/antchain_sdk_riskplus/client.py` & `antchain_riskplus-1.9.5/antchain_sdk_riskplus/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -131,15 +131,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.9.3'
+                    'sdk_version': '1.9.5'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
                     'user-agent': UtilClient.get_user_agent(self._user_agent)
                 }, headers)
@@ -233,15 +233,15 @@
                     'method': action,
                     'version': version,
                     'sign_type': 'HmacSHA1',
                     'req_time': AntchainUtils.get_timestamp(),
                     'req_msg_id': AntchainUtils.get_nonce(),
                     'access_key': self._access_key_id,
                     'base_sdk_version': 'TeaSDK-2.0',
-                    'sdk_version': '1.9.3'
+                    'sdk_version': '1.9.5'
                 }
                 if not UtilClient.empty(self._security_token):
                     _request.query['security_token'] = self._security_token
                 _request.headers = TeaCore.merge({
                     'host': UtilClient.default_string(self._endpoint, 'openapi.antchain.antgroup.com'),
                     'user-agent': UtilClient.get_user_agent(self._user_agent)
                 }, headers)
@@ -2245,14 +2245,68 @@
         Summary: 调额申请
         """
         UtilClient.validate_model(request)
         return riskplus_models.UpdateDubbridgeInstitutionCreditResponse().from_map(
             await self.do_request_async('1.0', 'riskplus.dubbridge.institution.credit.update', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def query_dubbridge_riskinfo_businessinfo(
+        self,
+        request: riskplus_models.QueryDubbridgeRiskinfoBusinessinfoRequest,
+    ) -> riskplus_models.QueryDubbridgeRiskinfoBusinessinfoResponse:
+        """
+        Description: 天枢企业经营数据查询
+        Summary: 天枢企业经营数据查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_dubbridge_riskinfo_businessinfo_ex(request, headers, runtime)
+
+    async def query_dubbridge_riskinfo_businessinfo_async(
+        self,
+        request: riskplus_models.QueryDubbridgeRiskinfoBusinessinfoRequest,
+    ) -> riskplus_models.QueryDubbridgeRiskinfoBusinessinfoResponse:
+        """
+        Description: 天枢企业经营数据查询
+        Summary: 天枢企业经营数据查询
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_dubbridge_riskinfo_businessinfo_ex_async(request, headers, runtime)
+
+    def query_dubbridge_riskinfo_businessinfo_ex(
+        self,
+        request: riskplus_models.QueryDubbridgeRiskinfoBusinessinfoRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> riskplus_models.QueryDubbridgeRiskinfoBusinessinfoResponse:
+        """
+        Description: 天枢企业经营数据查询
+        Summary: 天枢企业经营数据查询
+        """
+        UtilClient.validate_model(request)
+        return riskplus_models.QueryDubbridgeRiskinfoBusinessinfoResponse().from_map(
+            self.do_request('1.0', 'riskplus.dubbridge.riskinfo.businessinfo.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_dubbridge_riskinfo_businessinfo_ex_async(
+        self,
+        request: riskplus_models.QueryDubbridgeRiskinfoBusinessinfoRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> riskplus_models.QueryDubbridgeRiskinfoBusinessinfoResponse:
+        """
+        Description: 天枢企业经营数据查询
+        Summary: 天枢企业经营数据查询
+        """
+        UtilClient.validate_model(request)
+        return riskplus_models.QueryDubbridgeRiskinfoBusinessinfoResponse().from_map(
+            await self.do_request_async('1.0', 'riskplus.dubbridge.riskinfo.businessinfo.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def verify_finservice_zhima_identify(
         self,
         request: riskplus_models.VerifyFinserviceZhimaIdentifyRequest,
     ) -> riskplus_models.VerifyFinserviceZhimaIdentifyResponse:
         """
         Description: 四要素认证首先调用此接口
         Summary: 芝麻四要素接口
@@ -2947,14 +3001,176 @@
         Summary: 企业授信结果查询
         """
         UtilClient.validate_model(request)
         return riskplus_models.QueryRbbCompanyCreditResponse().from_map(
             await self.do_request_async('1.0', 'riskplus.rbb.company.credit.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def query_rbb_regdatasync_prepared(
+        self,
+        request: riskplus_models.QueryRbbRegdatasyncPreparedRequest,
+    ) -> riskplus_models.QueryRbbRegdatasyncPreparedResponse:
+        """
+        Description: 风险大脑-上交所数据离线同步数据准备状态，上交所本地部署鹰眼项目需要获取离线数据是否准备好的信息
+        Summary: 风险大脑-上交所数据离线同步数据准备状态
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.query_rbb_regdatasync_prepared_ex(request, headers, runtime)
+
+    async def query_rbb_regdatasync_prepared_async(
+        self,
+        request: riskplus_models.QueryRbbRegdatasyncPreparedRequest,
+    ) -> riskplus_models.QueryRbbRegdatasyncPreparedResponse:
+        """
+        Description: 风险大脑-上交所数据离线同步数据准备状态，上交所本地部署鹰眼项目需要获取离线数据是否准备好的信息
+        Summary: 风险大脑-上交所数据离线同步数据准备状态
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.query_rbb_regdatasync_prepared_ex_async(request, headers, runtime)
+
+    def query_rbb_regdatasync_prepared_ex(
+        self,
+        request: riskplus_models.QueryRbbRegdatasyncPreparedRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> riskplus_models.QueryRbbRegdatasyncPreparedResponse:
+        """
+        Description: 风险大脑-上交所数据离线同步数据准备状态，上交所本地部署鹰眼项目需要获取离线数据是否准备好的信息
+        Summary: 风险大脑-上交所数据离线同步数据准备状态
+        """
+        UtilClient.validate_model(request)
+        return riskplus_models.QueryRbbRegdatasyncPreparedResponse().from_map(
+            self.do_request('1.0', 'riskplus.rbb.regdatasync.prepared.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def query_rbb_regdatasync_prepared_ex_async(
+        self,
+        request: riskplus_models.QueryRbbRegdatasyncPreparedRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> riskplus_models.QueryRbbRegdatasyncPreparedResponse:
+        """
+        Description: 风险大脑-上交所数据离线同步数据准备状态，上交所本地部署鹰眼项目需要获取离线数据是否准备好的信息
+        Summary: 风险大脑-上交所数据离线同步数据准备状态
+        """
+        UtilClient.validate_model(request)
+        return riskplus_models.QueryRbbRegdatasyncPreparedResponse().from_map(
+            await self.do_request_async('1.0', 'riskplus.rbb.regdatasync.prepared.query', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def start_rbb_regdatasync_schedule(
+        self,
+        request: riskplus_models.StartRbbRegdatasyncScheduleRequest,
+    ) -> riskplus_models.StartRbbRegdatasyncScheduleResponse:
+        """
+        Description: 风险大脑-上交所数据离线同步数据开始通知标识
+        Summary: 风险大脑-上交所数据离线同步数据开始通知
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.start_rbb_regdatasync_schedule_ex(request, headers, runtime)
+
+    async def start_rbb_regdatasync_schedule_async(
+        self,
+        request: riskplus_models.StartRbbRegdatasyncScheduleRequest,
+    ) -> riskplus_models.StartRbbRegdatasyncScheduleResponse:
+        """
+        Description: 风险大脑-上交所数据离线同步数据开始通知标识
+        Summary: 风险大脑-上交所数据离线同步数据开始通知
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.start_rbb_regdatasync_schedule_ex_async(request, headers, runtime)
+
+    def start_rbb_regdatasync_schedule_ex(
+        self,
+        request: riskplus_models.StartRbbRegdatasyncScheduleRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> riskplus_models.StartRbbRegdatasyncScheduleResponse:
+        """
+        Description: 风险大脑-上交所数据离线同步数据开始通知标识
+        Summary: 风险大脑-上交所数据离线同步数据开始通知
+        """
+        UtilClient.validate_model(request)
+        return riskplus_models.StartRbbRegdatasyncScheduleResponse().from_map(
+            self.do_request('1.0', 'riskplus.rbb.regdatasync.schedule.start', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def start_rbb_regdatasync_schedule_ex_async(
+        self,
+        request: riskplus_models.StartRbbRegdatasyncScheduleRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> riskplus_models.StartRbbRegdatasyncScheduleResponse:
+        """
+        Description: 风险大脑-上交所数据离线同步数据开始通知标识
+        Summary: 风险大脑-上交所数据离线同步数据开始通知
+        """
+        UtilClient.validate_model(request)
+        return riskplus_models.StartRbbRegdatasyncScheduleResponse().from_map(
+            await self.do_request_async('1.0', 'riskplus.rbb.regdatasync.schedule.start', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    def finish_rbb_regdatasync_schedule(
+        self,
+        request: riskplus_models.FinishRbbRegdatasyncScheduleRequest,
+    ) -> riskplus_models.FinishRbbRegdatasyncScheduleResponse:
+        """
+        Description: 风险大脑-上交所数据离线同步数据完成记录 记录完成的状态
+        Summary: 风险大脑-上交所数据离线同步数据完成记录
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.finish_rbb_regdatasync_schedule_ex(request, headers, runtime)
+
+    async def finish_rbb_regdatasync_schedule_async(
+        self,
+        request: riskplus_models.FinishRbbRegdatasyncScheduleRequest,
+    ) -> riskplus_models.FinishRbbRegdatasyncScheduleResponse:
+        """
+        Description: 风险大脑-上交所数据离线同步数据完成记录 记录完成的状态
+        Summary: 风险大脑-上交所数据离线同步数据完成记录
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.finish_rbb_regdatasync_schedule_ex_async(request, headers, runtime)
+
+    def finish_rbb_regdatasync_schedule_ex(
+        self,
+        request: riskplus_models.FinishRbbRegdatasyncScheduleRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> riskplus_models.FinishRbbRegdatasyncScheduleResponse:
+        """
+        Description: 风险大脑-上交所数据离线同步数据完成记录 记录完成的状态
+        Summary: 风险大脑-上交所数据离线同步数据完成记录
+        """
+        UtilClient.validate_model(request)
+        return riskplus_models.FinishRbbRegdatasyncScheduleResponse().from_map(
+            self.do_request('1.0', 'riskplus.rbb.regdatasync.schedule.finish', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def finish_rbb_regdatasync_schedule_ex_async(
+        self,
+        request: riskplus_models.FinishRbbRegdatasyncScheduleRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> riskplus_models.FinishRbbRegdatasyncScheduleResponse:
+        """
+        Description: 风险大脑-上交所数据离线同步数据完成记录 记录完成的状态
+        Summary: 风险大脑-上交所数据离线同步数据完成记录
+        """
+        UtilClient.validate_model(request)
+        return riskplus_models.FinishRbbRegdatasyncScheduleResponse().from_map(
+            await self.do_request_async('1.0', 'riskplus.rbb.regdatasync.schedule.finish', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def query_rpgw_sign_url(
         self,
         request: riskplus_models.QueryRpgwSignUrlRequest,
     ) -> riskplus_models.QueryRpgwSignUrlResponse:
         """
         Description: 获取签约接口
         Summary: 获取签约接口
@@ -4875,14 +5091,68 @@
         Summary: 营销盾实时营销服务
         """
         UtilClient.validate_model(request)
         return riskplus_models.BatchqueryUmktRtMarketingResponse().from_map(
             await self.do_request_async('1.0', 'riskplus.umkt.rt.marketing.batchquery', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
         )
 
+    def sync_umkt_rt_eventresult(
+        self,
+        request: riskplus_models.SyncUmktRtEventresultRequest,
+    ) -> riskplus_models.SyncUmktRtEventresultResponse:
+        """
+        Description: 梦网富信投放事件通知
+        Summary: 梦网富信投放事件通知
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return self.sync_umkt_rt_eventresult_ex(request, headers, runtime)
+
+    async def sync_umkt_rt_eventresult_async(
+        self,
+        request: riskplus_models.SyncUmktRtEventresultRequest,
+    ) -> riskplus_models.SyncUmktRtEventresultResponse:
+        """
+        Description: 梦网富信投放事件通知
+        Summary: 梦网富信投放事件通知
+        """
+        runtime = util_models.RuntimeOptions()
+        headers = {}
+        return await self.sync_umkt_rt_eventresult_ex_async(request, headers, runtime)
+
+    def sync_umkt_rt_eventresult_ex(
+        self,
+        request: riskplus_models.SyncUmktRtEventresultRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> riskplus_models.SyncUmktRtEventresultResponse:
+        """
+        Description: 梦网富信投放事件通知
+        Summary: 梦网富信投放事件通知
+        """
+        UtilClient.validate_model(request)
+        return riskplus_models.SyncUmktRtEventresultResponse().from_map(
+            self.do_request('1.0', 'riskplus.umkt.rt.eventresult.sync', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
+    async def sync_umkt_rt_eventresult_ex_async(
+        self,
+        request: riskplus_models.SyncUmktRtEventresultRequest,
+        headers: Dict[str, str],
+        runtime: util_models.RuntimeOptions,
+    ) -> riskplus_models.SyncUmktRtEventresultResponse:
+        """
+        Description: 梦网富信投放事件通知
+        Summary: 梦网富信投放事件通知
+        """
+        UtilClient.validate_model(request)
+        return riskplus_models.SyncUmktRtEventresultResponse().from_map(
+            await self.do_request_async('1.0', 'riskplus.umkt.rt.eventresult.sync', 'HTTPS', 'POST', f'/gateway.do', TeaCore.to_map(request), headers, runtime)
+        )
+
     def create_antcloud_gatewayx_file_upload(
         self,
         request: riskplus_models.CreateAntcloudGatewayxFileUploadRequest,
     ) -> riskplus_models.CreateAntcloudGatewayxFileUploadResponse:
         """
         Description: 创建HTTP PUT提交的文件上传
         Summary: 文件上传创建
```

### Comparing `antchain_riskplus-1.9.3/antchain_sdk_riskplus/models.py` & `antchain_riskplus-1.9.5/antchain_sdk_riskplus/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -3175,14 +3175,110 @@
         if m.get('update_date') is not None:
             self.update_date = m.get('update_date')
         if m.get('platform') is not None:
             self.platform = m.get('platform')
         return self
 
 
+class EventResultSyncDetail(TeaModel):
+    def __init__(
+        self,
+        plan_owner_id: str = None,
+        event_id: str = None,
+        plan_id: str = None,
+        msg_id: str = None,
+        event_time: str = None,
+        event_type: int = None,
+        state: int = None,
+        key_type: str = None,
+        customer_key: str = None,
+        ext_data: str = None,
+    ):
+        # 广告主id
+        self.plan_owner_id = plan_owner_id
+        # 事件唯一id（单个租户全局唯一）
+        self.event_id = event_id
+        # 营销计划id
+        self.plan_id = plan_id
+        # 消息id
+        self.msg_id = msg_id
+        # 事件时间
+        self.event_time = event_time
+        # 事件类型：1为富信贴尾
+        self.event_type = event_type
+        # 1为成功 2为失败
+        self.state = state
+        # 用户key类型
+        self.key_type = key_type
+        # 手机号
+        self.customer_key = customer_key
+        # 扩展字段
+        self.ext_data = ext_data
+
+    def validate(self):
+        self.validate_required(self.plan_owner_id, 'plan_owner_id')
+        self.validate_required(self.event_id, 'event_id')
+        self.validate_required(self.plan_id, 'plan_id')
+        self.validate_required(self.msg_id, 'msg_id')
+        self.validate_required(self.event_time, 'event_time')
+        self.validate_required(self.event_type, 'event_type')
+        self.validate_required(self.state, 'state')
+        self.validate_required(self.key_type, 'key_type')
+        self.validate_required(self.customer_key, 'customer_key')
+        self.validate_required(self.ext_data, 'ext_data')
+
+    def to_map(self):
+        result = dict()
+        if self.plan_owner_id is not None:
+            result['plan_owner_id'] = self.plan_owner_id
+        if self.event_id is not None:
+            result['event_id'] = self.event_id
+        if self.plan_id is not None:
+            result['plan_id'] = self.plan_id
+        if self.msg_id is not None:
+            result['msg_id'] = self.msg_id
+        if self.event_time is not None:
+            result['event_time'] = self.event_time
+        if self.event_type is not None:
+            result['event_type'] = self.event_type
+        if self.state is not None:
+            result['state'] = self.state
+        if self.key_type is not None:
+            result['key_type'] = self.key_type
+        if self.customer_key is not None:
+            result['customer_key'] = self.customer_key
+        if self.ext_data is not None:
+            result['ext_data'] = self.ext_data
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('plan_owner_id') is not None:
+            self.plan_owner_id = m.get('plan_owner_id')
+        if m.get('event_id') is not None:
+            self.event_id = m.get('event_id')
+        if m.get('plan_id') is not None:
+            self.plan_id = m.get('plan_id')
+        if m.get('msg_id') is not None:
+            self.msg_id = m.get('msg_id')
+        if m.get('event_time') is not None:
+            self.event_time = m.get('event_time')
+        if m.get('event_type') is not None:
+            self.event_type = m.get('event_type')
+        if m.get('state') is not None:
+            self.state = m.get('state')
+        if m.get('key_type') is not None:
+            self.key_type = m.get('key_type')
+        if m.get('customer_key') is not None:
+            self.customer_key = m.get('customer_key')
+        if m.get('ext_data') is not None:
+            self.ext_data = m.get('ext_data')
+        return self
+
+
 class RtopCompanyAlarm(TeaModel):
     def __init__(
         self,
         company_id: str = None,
         alarm_type: str = None,
         alarm_idx: str = None,
         alarm_date: str = None,
@@ -8515,63 +8611,63 @@
 class QueryDubbridgeRiskinfoEnterprisescoreRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         social_credit_code: str = None,
         mobile_md_5: str = None,
-        open_id: str = None,
+        customer_no: str = None,
         channel_code: str = None,
     ):
         # OAuth模式下的授权token
         self.auth_token = auth_token
         self.product_instance_id = product_instance_id
         # 统一信用代码
         self.social_credit_code = social_credit_code
         # MD5
         self.mobile_md_5 = mobile_md_5
-        # 合作方用户id
-        self.open_id = open_id
+        # 客户号
+        self.customer_no = customer_no
         # 渠道号
         self.channel_code = channel_code
 
     def validate(self):
         self.validate_required(self.social_credit_code, 'social_credit_code')
         self.validate_required(self.mobile_md_5, 'mobile_md_5')
-        self.validate_required(self.open_id, 'open_id')
+        self.validate_required(self.customer_no, 'customer_no')
         self.validate_required(self.channel_code, 'channel_code')
 
     def to_map(self):
         result = dict()
         if self.auth_token is not None:
             result['auth_token'] = self.auth_token
         if self.product_instance_id is not None:
             result['product_instance_id'] = self.product_instance_id
         if self.social_credit_code is not None:
             result['social_credit_code'] = self.social_credit_code
         if self.mobile_md_5 is not None:
             result['mobile_md5'] = self.mobile_md_5
-        if self.open_id is not None:
-            result['open_id'] = self.open_id
+        if self.customer_no is not None:
+            result['customer_no'] = self.customer_no
         if self.channel_code is not None:
             result['channel_code'] = self.channel_code
         return result
 
     def from_map(self, m: dict = None):
         m = m or dict()
         if m.get('auth_token') is not None:
             self.auth_token = m.get('auth_token')
         if m.get('product_instance_id') is not None:
             self.product_instance_id = m.get('product_instance_id')
         if m.get('social_credit_code') is not None:
             self.social_credit_code = m.get('social_credit_code')
         if m.get('mobile_md5') is not None:
             self.mobile_md_5 = m.get('mobile_md5')
-        if m.get('open_id') is not None:
-            self.open_id = m.get('open_id')
+        if m.get('customer_no') is not None:
+            self.customer_no = m.get('customer_no')
         if m.get('channel_code') is not None:
             self.channel_code = m.get('channel_code')
         return self
 
 
 class QueryDubbridgeRiskinfoEnterprisescoreResponse(TeaModel):
     def __init__(
@@ -8901,14 +8997,112 @@
         if m.get('biz_code') is not None:
             self.biz_code = m.get('biz_code')
         if m.get('biz_msg') is not None:
             self.biz_msg = m.get('biz_msg')
         return self
 
 
+class QueryDubbridgeRiskinfoBusinessinfoRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        channel_code: str = None,
+        customer_no: str = None,
+        social_credit_code: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 渠道号
+        self.channel_code = channel_code
+        # 客户号
+        self.customer_no = customer_no
+        # 统一社会信用代码
+        self.social_credit_code = social_credit_code
+
+    def validate(self):
+        self.validate_required(self.channel_code, 'channel_code')
+        self.validate_required(self.customer_no, 'customer_no')
+        self.validate_required(self.social_credit_code, 'social_credit_code')
+
+    def to_map(self):
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.channel_code is not None:
+            result['channel_code'] = self.channel_code
+        if self.customer_no is not None:
+            result['customer_no'] = self.customer_no
+        if self.social_credit_code is not None:
+            result['social_credit_code'] = self.social_credit_code
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('channel_code') is not None:
+            self.channel_code = m.get('channel_code')
+        if m.get('customer_no') is not None:
+            self.customer_no = m.get('customer_no')
+        if m.get('social_credit_code') is not None:
+            self.social_credit_code = m.get('social_credit_code')
+        return self
+
+
+class QueryDubbridgeRiskinfoBusinessinfoResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        info: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 企业经营信息
+        self.info = info
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.info is not None:
+            result['info'] = self.info
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('info') is not None:
+            self.info = m.get('info')
+        return self
+
+
 class VerifyFinserviceZhimaIdentifyRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         legal_person_cert_name: str = None,
         legal_person_cert_no: str = None,
@@ -10185,14 +10379,258 @@
         if m.get('credit_amount') is not None:
             self.credit_amount = m.get('credit_amount')
         if m.get('extra') is not None:
             self.extra = m.get('extra')
         return self
 
 
+class QueryRbbRegdatasyncPreparedRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        biz_date: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 查询该bizDate数据分区的数据是否已经准备好
+        self.biz_date = biz_date
+
+    def validate(self):
+        self.validate_required(self.biz_date, 'biz_date')
+        if self.biz_date is not None:
+            self.validate_max_length(self.biz_date, 'biz_date', 8)
+
+    def to_map(self):
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.biz_date is not None:
+            result['biz_date'] = self.biz_date
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('biz_date') is not None:
+            self.biz_date = m.get('biz_date')
+        return self
+
+
+class QueryRbbRegdatasyncPreparedResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+        prepared: bool = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+        # 指定时间分区的数据是否已经准备完毕
+        self.prepared = prepared
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        if self.prepared is not None:
+            result['prepared'] = self.prepared
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        if m.get('prepared') is not None:
+            self.prepared = m.get('prepared')
+        return self
+
+
+class StartRbbRegdatasyncScheduleRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        biz_date: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 同步时间分区
+        self.biz_date = biz_date
+
+    def validate(self):
+        self.validate_required(self.biz_date, 'biz_date')
+
+    def to_map(self):
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.biz_date is not None:
+            result['biz_date'] = self.biz_date
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('biz_date') is not None:
+            self.biz_date = m.get('biz_date')
+        return self
+
+
+class StartRbbRegdatasyncScheduleResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
+class FinishRbbRegdatasyncScheduleRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        biz_date: str = None,
+        sync_info: str = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 时间分区
+        self.biz_date = biz_date
+        # 记录当前分区离线同步情况
+        self.sync_info = sync_info
+
+    def validate(self):
+        self.validate_required(self.biz_date, 'biz_date')
+        if self.biz_date is not None:
+            self.validate_max_length(self.biz_date, 'biz_date', 8)
+        self.validate_required(self.sync_info, 'sync_info')
+
+    def to_map(self):
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        if self.biz_date is not None:
+            result['biz_date'] = self.biz_date
+        if self.sync_info is not None:
+            result['sync_info'] = self.sync_info
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        if m.get('biz_date') is not None:
+            self.biz_date = m.get('biz_date')
+        if m.get('sync_info') is not None:
+            self.sync_info = m.get('sync_info')
+        return self
+
+
+class FinishRbbRegdatasyncScheduleResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
 class QueryRpgwSignUrlRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         product_instance_id: str = None,
         company_code: str = None,
         platform_user_identification: str = None,
@@ -14970,14 +15408,98 @@
         if m.get('query_result') is not None:
             for k in m.get('query_result'):
                 temp_model = CustomerUmktInfoModel()
                 self.query_result.append(temp_model.from_map(k))
         return self
 
 
+class SyncUmktRtEventresultRequest(TeaModel):
+    def __init__(
+        self,
+        auth_token: str = None,
+        product_instance_id: str = None,
+        detail: List[EventResultSyncDetail] = None,
+    ):
+        # OAuth模式下的授权token
+        self.auth_token = auth_token
+        self.product_instance_id = product_instance_id
+        # 详细事件明细
+        self.detail = detail
+
+    def validate(self):
+        self.validate_required(self.detail, 'detail')
+        if self.detail:
+            for k in self.detail:
+                if k:
+                    k.validate()
+
+    def to_map(self):
+        result = dict()
+        if self.auth_token is not None:
+            result['auth_token'] = self.auth_token
+        if self.product_instance_id is not None:
+            result['product_instance_id'] = self.product_instance_id
+        result['detail'] = []
+        if self.detail is not None:
+            for k in self.detail:
+                result['detail'].append(k.to_map() if k else None)
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('auth_token') is not None:
+            self.auth_token = m.get('auth_token')
+        if m.get('product_instance_id') is not None:
+            self.product_instance_id = m.get('product_instance_id')
+        self.detail = []
+        if m.get('detail') is not None:
+            for k in m.get('detail'):
+                temp_model = EventResultSyncDetail()
+                self.detail.append(temp_model.from_map(k))
+        return self
+
+
+class SyncUmktRtEventresultResponse(TeaModel):
+    def __init__(
+        self,
+        req_msg_id: str = None,
+        result_code: str = None,
+        result_msg: str = None,
+    ):
+        # 请求唯一ID，用于链路跟踪和问题排查
+        self.req_msg_id = req_msg_id
+        # 结果码，一般OK表示调用成功
+        self.result_code = result_code
+        # 异常信息的文本描述
+        self.result_msg = result_msg
+
+    def validate(self):
+        pass
+
+    def to_map(self):
+        result = dict()
+        if self.req_msg_id is not None:
+            result['req_msg_id'] = self.req_msg_id
+        if self.result_code is not None:
+            result['result_code'] = self.result_code
+        if self.result_msg is not None:
+            result['result_msg'] = self.result_msg
+        return result
+
+    def from_map(self, m: dict = None):
+        m = m or dict()
+        if m.get('req_msg_id') is not None:
+            self.req_msg_id = m.get('req_msg_id')
+        if m.get('result_code') is not None:
+            self.result_code = m.get('result_code')
+        if m.get('result_msg') is not None:
+            self.result_msg = m.get('result_msg')
+        return self
+
+
 class CreateAntcloudGatewayxFileUploadRequest(TeaModel):
     def __init__(
         self,
         auth_token: str = None,
         api_code: str = None,
         file_label: str = None,
         file_metadata: str = None,
```

### Comparing `antchain_riskplus-1.9.3/setup.py` & `antchain_riskplus-1.9.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 
 import os
 from setuptools import setup, find_packages
 
 """
 setup module for antchain_riskplus.
 
-Created on 28/03/2022
+Created on 15/04/2022
 
 @author: Ant Chain SDK
 """
 
 PACKAGE = "antchain_sdk_riskplus"
 NAME = "antchain_riskplus" or "alibabacloud-package"
 DESCRIPTION = "Ant Chain RISKPLUS SDK Library for Python"
```

