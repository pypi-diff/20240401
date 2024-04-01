# Comparing `tmp/neon-llm-core-0.1.1a2.tar.gz` & `tmp/neon-llm-core-0.1.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "neon-llm-core-0.1.1a2.tar", last modified: Fri Mar 22 18:08:31 2024, max compression
+gzip compressed data, was "neon-llm-core-0.1.1a3.tar", last modified: Mon Apr  1 18:35:27 2024, max compression
```

## Comparing `neon-llm-core-0.1.1a2.tar` & `neon-llm-core-0.1.1a3.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:08:31.366122 neon-llm-core-0.1.1a2/
--rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-03-22 18:08:24.000000 neon-llm-core-0.1.1a2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-03-22 18:08:31.366122 neon-llm-core-0.1.1a2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-03-22 18:08:24.000000 neon-llm-core-0.1.1a2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:08:31.366122 neon-llm-core-0.1.1a2/neon_llm_core/
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-03-22 18:08:24.000000 neon-llm-core-0.1.1a2/neon_llm_core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-03-22 18:08:24.000000 neon-llm-core-0.1.1a2/neon_llm_core/chatbot.py
--rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-03-22 18:08:24.000000 neon-llm-core-0.1.1a2/neon_llm_core/llm.py
--rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-03-22 18:08:24.000000 neon-llm-core-0.1.1a2/neon_llm_core/rmq.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:08:31.366122 neon-llm-core-0.1.1a2/neon_llm_core/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-03-22 18:08:24.000000 neon-llm-core-0.1.1a2/neon_llm_core/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-03-22 18:08:24.000000 neon-llm-core-0.1.1a2/neon_llm_core/utils/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-03-22 18:08:24.000000 neon-llm-core-0.1.1a2/neon_llm_core/utils/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:08:31.366122 neon-llm-core-0.1.1a2/neon_llm_core/utils/personas/
--rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-03-22 18:08:24.000000 neon-llm-core-0.1.1a2/neon_llm_core/utils/personas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-03-22 18:08:24.000000 neon-llm-core-0.1.1a2/neon_llm_core/utils/personas/models.py
--rw-r--r--   0 runner    (1001) docker     (127)     4783 2024-03-22 18:08:24.000000 neon-llm-core-0.1.1a2/neon_llm_core/utils/personas/provider.py
--rw-r--r--   0 runner    (1001) docker     (127)     4623 2024-03-22 18:08:24.000000 neon-llm-core-0.1.1a2/neon_llm_core/utils/personas/state.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-03-22 18:08:31.366122 neon-llm-core-0.1.1a2/neon_llm_core.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-03-22 18:08:31.000000 neon-llm-core-0.1.1a2/neon_llm_core.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      592 2024-03-22 18:08:31.000000 neon-llm-core-0.1.1a2/neon_llm_core.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 18:08:31.000000 neon-llm-core-0.1.1a2/neon_llm_core.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      112 2024-03-22 18:08:31.000000 neon-llm-core-0.1.1a2/neon_llm_core.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-03-22 18:08:31.000000 neon-llm-core-0.1.1a2/neon_llm_core.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-03-22 18:08:31.000000 neon-llm-core-0.1.1a2/neon_llm_core.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-03-22 18:08:31.366122 neon-llm-core-0.1.1a2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-03-22 18:08:24.000000 neon-llm-core-0.1.1a2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:35:27.767654 neon-llm-core-0.1.1a3/
+-rw-r--r--   0 runner    (1001) docker     (127)     1635 2024-04-01 18:35:21.000000 neon-llm-core-0.1.1a3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-01 18:35:27.767654 neon-llm-core-0.1.1a3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1546 2024-04-01 18:35:21.000000 neon-llm-core-0.1.1a3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:35:27.763654 neon-llm-core-0.1.1a3/neon_llm_core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-01 18:35:21.000000 neon-llm-core-0.1.1a3/neon_llm_core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7860 2024-04-01 18:35:21.000000 neon-llm-core-0.1.1a3/neon_llm_core/chatbot.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4544 2024-04-01 18:35:21.000000 neon-llm-core-0.1.1a3/neon_llm_core/llm.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9842 2024-04-01 18:35:21.000000 neon-llm-core-0.1.1a3/neon_llm_core/rmq.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:35:27.763654 neon-llm-core-0.1.1a3/neon_llm_core/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-01 18:35:21.000000 neon-llm-core-0.1.1a3/neon_llm_core/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3286 2024-04-01 18:35:21.000000 neon-llm-core-0.1.1a3/neon_llm_core/utils/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1705 2024-04-01 18:35:21.000000 neon-llm-core-0.1.1a3/neon_llm_core/utils/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:35:27.767654 neon-llm-core-0.1.1a3/neon_llm_core/utils/personas/
+-rw-r--r--   0 runner    (1001) docker     (127)     1685 2024-04-01 18:35:21.000000 neon-llm-core-0.1.1a3/neon_llm_core/utils/personas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2075 2024-04-01 18:35:21.000000 neon-llm-core-0.1.1a3/neon_llm_core/utils/personas/models.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4989 2024-04-01 18:35:21.000000 neon-llm-core-0.1.1a3/neon_llm_core/utils/personas/provider.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4728 2024-04-01 18:35:21.000000 neon-llm-core-0.1.1a3/neon_llm_core/utils/personas/state.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-01 18:35:27.763654 neon-llm-core-0.1.1a3/neon_llm_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1946 2024-04-01 18:35:27.000000 neon-llm-core-0.1.1a3/neon_llm_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      592 2024-04-01 18:35:27.000000 neon-llm-core-0.1.1a3/neon_llm_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 18:35:27.000000 neon-llm-core-0.1.1a3/neon_llm_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      112 2024-04-01 18:35:27.000000 neon-llm-core-0.1.1a3/neon_llm_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-01 18:35:27.000000 neon-llm-core-0.1.1a3/neon_llm_core.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-01 18:35:27.000000 neon-llm-core-0.1.1a3/neon_llm_core.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-01 18:35:27.767654 neon-llm-core-0.1.1a3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     3840 2024-04-01 18:35:21.000000 neon-llm-core-0.1.1a3/setup.py
```

### Comparing `neon-llm-core-0.1.1a2/LICENSE.md` & `neon-llm-core-0.1.1a3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `neon-llm-core-0.1.1a2/PKG-INFO` & `neon-llm-core-0.1.1a3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-llm-core
-Version: 0.1.1a2
+Version: 0.1.1a3
 Summary: Core Neon LLM service
 Home-page: https://github.com/NeonGeckoCom/neon-llm-core
 Author: NeonGecko
 Author-email: developers@neon.ai
 License: BSD-3.0
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `neon-llm-core-0.1.1a2/README.md` & `neon-llm-core-0.1.1a3/README.md`

 * *Files identical despite different names*

### Comparing `neon-llm-core-0.1.1a2/neon_llm_core/__init__.py` & `neon-llm-core-0.1.1a3/neon_llm_core/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-llm-core-0.1.1a2/neon_llm_core/chatbot.py` & `neon-llm-core-0.1.1a3/neon_llm_core/chatbot.py`

 * *Files identical despite different names*

### Comparing `neon-llm-core-0.1.1a2/neon_llm_core/llm.py` & `neon-llm-core-0.1.1a3/neon_llm_core/llm.py`

 * *Files identical despite different names*

### Comparing `neon-llm-core-0.1.1a2/neon_llm_core/rmq.py` & `neon-llm-core-0.1.1a3/neon_llm_core/rmq.py`

 * *Files identical despite different names*

### Comparing `neon-llm-core-0.1.1a2/neon_llm_core/utils/__init__.py` & `neon-llm-core-0.1.1a3/neon_llm_core/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-llm-core-0.1.1a2/neon_llm_core/utils/config.py` & `neon-llm-core-0.1.1a3/neon_llm_core/utils/config.py`

 * *Files identical despite different names*

### Comparing `neon-llm-core-0.1.1a2/neon_llm_core/utils/constants.py` & `neon-llm-core-0.1.1a3/neon_llm_core/utils/constants.py`

 * *Files identical despite different names*

### Comparing `neon-llm-core-0.1.1a2/neon_llm_core/utils/personas/__init__.py` & `neon-llm-core-0.1.1a3/neon_llm_core/utils/personas/__init__.py`

 * *Files identical despite different names*

### Comparing `neon-llm-core-0.1.1a2/neon_llm_core/utils/personas/models.py` & `neon-llm-core-0.1.1a3/neon_llm_core/utils/personas/models.py`

 * *Files identical despite different names*

### Comparing `neon-llm-core-0.1.1a2/neon_llm_core/utils/personas/provider.py` & `neon-llm-core-0.1.1a3/neon_llm_core/utils/personas/provider.py`

 * *Files 5% similar despite different names*

```diff
@@ -61,29 +61,34 @@
 
     @property
     def personas(self):
         return self._personas
 
     @personas.setter
     def personas(self, data):
-        now = int(time())
         LOG.debug(f'Setting personas={data}')
-        if data and isinstance(data, list):
-            self._personas = data
-            self._persona_last_sync = now
-            self._persona_handlers_state.clean_up_personas(ignore_items=self._personas)
-        elif now - self._persona_last_sync > self.PERSONA_STATE_TTL:
+        if self._should_reset_personas(data=data):
             LOG.warning(f'Persona state TTL expired, resetting personas config')
             self._personas = []
             self._persona_handlers_state.init_default_handlers()
+        else:
+            self._personas = data
+        self._persona_handlers_state.clean_up_personas(ignore_items=self._personas)
+
+    def _should_reset_personas(self, data) -> bool:
+        return (not (self._persona_last_sync == 0 and data)
+                and int(time()) - self._persona_last_sync > self.PERSONA_STATE_TTL)
 
     def _fetch_persona_config(self):
         response = send_mq_request(vhost=LLM_VHOST,
                                    request_data={"service_name": self.service_name},
-                                   target_queue=PersonasProvider.GET_CONFIGURED_PERSONAS_QUEUE)
+                                   target_queue=PersonasProvider.GET_CONFIGURED_PERSONAS_QUEUE,
+                                   timeout=60)
+        if 'items' in response:
+            self._persona_last_sync = int(time())
         response_data = response.get('items', [])
         personas = []
         for item in response_data:
             item.setdefault('name', item.pop('persona_name', None))
             persona = PersonaModel.parse_obj(obj=item)
             self._persona_handlers_state.add_persona_handler(persona=persona)
             personas.append(persona)
```

### Comparing `neon-llm-core-0.1.1a2/neon_llm_core/utils/personas/state.py` & `neon-llm-core-0.1.1a3/neon_llm_core/utils/personas/state.py`

 * *Files 6% similar despite different names*

```diff
@@ -38,15 +38,14 @@
 class PersonaHandlersState:
 
     def __init__(self, service_name: str, ovos_config: dict):
         self._created_items: Dict[str, LLMBot] = {}
         self.service_name = service_name
         self.ovos_config = ovos_config
         self.mq_config = ovos_config.get('MQ', {})
-        self.init_default_handlers()
 
     def init_default_handlers(self):
         self._created_items = {}
         if self.ovos_config.get("llm_bots", {}).get(self.service_name):
             LOG.info(f"Chatbot(s) configured for: {self.service_name}")
             for persona in self.ovos_config['llm_bots'][self.service_name]:
                 self.add_persona_handler(persona=PersonaModel.parse_obj(obj=persona))
@@ -80,9 +79,13 @@
         return bot
 
     def clean_up_personas(self, ignore_items: List[PersonaModel] = None):
         connected_personas = set(self._created_items)
         ignored_persona_ids = set(persona.id for persona in ignore_items or [])
         personas_to_remove = connected_personas - ignored_persona_ids
         for persona_id in personas_to_remove:
-            LOG.info(f'Removing persona_id = {persona_id}')
-            self._created_items.pop(persona_id, None)
+            self.remove_persona(persona_id=persona_id)
+
+    def remove_persona(self, persona_id: str):
+        LOG.info(f'Removing persona_id = {persona_id}')
+        self._created_items[persona_id].stop()
+        self._created_items.pop(persona_id, None)
```

### Comparing `neon-llm-core-0.1.1a2/neon_llm_core.egg-info/PKG-INFO` & `neon-llm-core-0.1.1a3/neon_llm_core.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: neon-llm-core
-Version: 0.1.1a2
+Version: 0.1.1a3
 Summary: Core Neon LLM service
 Home-page: https://github.com/NeonGeckoCom/neon-llm-core
 Author: NeonGecko
 Author-email: developers@neon.ai
 License: BSD-3.0
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `neon-llm-core-0.1.1a2/neon_llm_core.egg-info/SOURCES.txt` & `neon-llm-core-0.1.1a3/neon_llm_core.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `neon-llm-core-0.1.1a2/setup.py` & `neon-llm-core-0.1.1a3/setup.py`

 * *Files identical despite different names*

