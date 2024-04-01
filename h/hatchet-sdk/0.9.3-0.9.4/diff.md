# Comparing `tmp/hatchet_sdk-0.9.3.tar.gz` & `tmp/hatchet_sdk-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hatchet_sdk-0.9.3.tar", max compression
+gzip compressed data, was "hatchet_sdk-0.9.4.tar", max compression
```

## Comparing `hatchet_sdk-0.9.3.tar` & `hatchet_sdk-0.9.4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
--rw-r--r--   0        0        0      141 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/README.md
--rw-r--r--   0        0        0      116 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/hatchet_sdk/__init__.py
--rw-r--r--   0        0        0     3225 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/hatchet_sdk/client.py
--rw-r--r--   0        0        0     2010 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/hatchet_sdk/clients/admin.py
--rw-r--r--   0        0        0     7756 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/hatchet_sdk/clients/dispatcher.py
--rw-r--r--   0        0        0     1104 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/hatchet_sdk/clients/events.py
--rw-r--r--   0        0        0     4303 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/hatchet_sdk/clients/listener.py
--rw-r--r--   0        0        0      946 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/hatchet_sdk/context.py
--rw-r--r--   0        0        0     7175 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/hatchet_sdk/dispatcher_pb2.py
--rw-r--r--   0        0        0     9692 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/hatchet_sdk/dispatcher_pb2.pyi
--rw-r--r--   0        0        0    11518 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/hatchet_sdk/dispatcher_pb2_grpc.py
--rw-r--r--   0        0        0     2716 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/hatchet_sdk/events_pb2.py
--rw-r--r--   0        0        0     2266 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/hatchet_sdk/events_pb2.pyi
--rw-r--r--   0        0        0     5699 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/hatchet_sdk/events_pb2_grpc.py
--rw-r--r--   0        0        0     1608 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/hatchet_sdk/hatchet.py
--rw-r--r--   0        0        0     3170 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/hatchet_sdk/loader.py
--rw-r--r--   0        0        0      203 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/hatchet_sdk/logger.py
--rw-r--r--   0        0        0       79 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/hatchet_sdk/metadata.py
--rw-r--r--   0        0        0      997 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/hatchet_sdk/semver.py
--rw-r--r--   0        0        0      572 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/hatchet_sdk/token.py
--rw-r--r--   0        0        0    14142 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/hatchet_sdk/worker.py
--rw-r--r--   0        0        0     3117 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/hatchet_sdk/workflow.py
--rw-r--r--   0        0        0     8988 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/hatchet_sdk/workflows_pb2.py
--rw-r--r--   0        0        0    13249 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/hatchet_sdk/workflows_pb2.pyi
--rw-r--r--   0        0        0    11975 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/hatchet_sdk/workflows_pb2_grpc.py
--rw-r--r--   0        0        0      404 2024-02-06 12:18:17.941423 hatchet_sdk-0.9.3/pyproject.toml
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 hatchet_sdk-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0      141 2024-02-09 16:36:12.333369 hatchet_sdk-0.9.4/README.md
+-rw-r--r--   0        0        0      163 2024-02-09 16:36:12.333369 hatchet_sdk-0.9.4/hatchet_sdk/__init__.py
+-rw-r--r--   0        0        0     3225 2024-02-09 16:36:12.333369 hatchet_sdk-0.9.4/hatchet_sdk/client.py
+-rw-r--r--   0        0        0     2010 2024-02-09 16:36:12.333369 hatchet_sdk-0.9.4/hatchet_sdk/clients/admin.py
+-rw-r--r--   0        0        0     7756 2024-02-09 16:36:12.333369 hatchet_sdk-0.9.4/hatchet_sdk/clients/dispatcher.py
+-rw-r--r--   0        0        0     1104 2024-02-09 16:36:12.333369 hatchet_sdk-0.9.4/hatchet_sdk/clients/events.py
+-rw-r--r--   0        0        0     6846 2024-02-09 16:36:12.333369 hatchet_sdk-0.9.4/hatchet_sdk/clients/listener.py
+-rw-r--r--   0        0        0      946 2024-02-09 16:36:12.333369 hatchet_sdk-0.9.4/hatchet_sdk/context.py
+-rw-r--r--   0        0        0     7213 2024-02-09 16:36:12.333369 hatchet_sdk-0.9.4/hatchet_sdk/dispatcher_pb2.py
+-rw-r--r--   0        0        0     9779 2024-02-09 16:36:12.333369 hatchet_sdk-0.9.4/hatchet_sdk/dispatcher_pb2.pyi
+-rw-r--r--   0        0        0    10367 2024-02-09 16:36:12.333369 hatchet_sdk-0.9.4/hatchet_sdk/dispatcher_pb2_grpc.py
+-rw-r--r--   0        0        0     2716 2024-02-09 16:36:12.337369 hatchet_sdk-0.9.4/hatchet_sdk/events_pb2.py
+-rw-r--r--   0        0        0     2266 2024-02-09 16:36:12.337369 hatchet_sdk-0.9.4/hatchet_sdk/events_pb2.pyi
+-rw-r--r--   0        0        0     5318 2024-02-09 16:36:12.337369 hatchet_sdk-0.9.4/hatchet_sdk/events_pb2_grpc.py
+-rw-r--r--   0        0        0     1608 2024-02-09 16:36:12.337369 hatchet_sdk-0.9.4/hatchet_sdk/hatchet.py
+-rw-r--r--   0        0        0     3170 2024-02-09 16:36:12.337369 hatchet_sdk-0.9.4/hatchet_sdk/loader.py
+-rw-r--r--   0        0        0      203 2024-02-09 16:36:12.337369 hatchet_sdk-0.9.4/hatchet_sdk/logger.py
+-rw-r--r--   0        0        0       79 2024-02-09 16:36:12.337369 hatchet_sdk-0.9.4/hatchet_sdk/metadata.py
+-rw-r--r--   0        0        0      997 2024-02-09 16:36:12.337369 hatchet_sdk-0.9.4/hatchet_sdk/semver.py
+-rw-r--r--   0        0        0      572 2024-02-09 16:36:12.337369 hatchet_sdk-0.9.4/hatchet_sdk/token.py
+-rw-r--r--   0        0        0    14142 2024-02-09 16:36:12.337369 hatchet_sdk-0.9.4/hatchet_sdk/worker.py
+-rw-r--r--   0        0        0     3117 2024-02-09 16:36:12.337369 hatchet_sdk-0.9.4/hatchet_sdk/workflow.py
+-rw-r--r--   0        0        0     9033 2024-02-09 16:36:12.337369 hatchet_sdk-0.9.4/hatchet_sdk/workflows_pb2.py
+-rw-r--r--   0        0        0    13357 2024-02-09 16:36:12.337369 hatchet_sdk-0.9.4/hatchet_sdk/workflows_pb2.pyi
+-rw-r--r--   0        0        0    11975 2024-02-09 16:36:12.337369 hatchet_sdk-0.9.4/hatchet_sdk/workflows_pb2_grpc.py
+-rw-r--r--   0        0        0      404 2024-02-09 16:36:12.337369 hatchet_sdk-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 hatchet_sdk-0.9.4/PKG-INFO
```

### Comparing `hatchet_sdk-0.9.3/hatchet_sdk/client.py` & `hatchet_sdk-0.9.4/hatchet_sdk/client.py`

 * *Files identical despite different names*

### Comparing `hatchet_sdk-0.9.3/hatchet_sdk/clients/admin.py` & `hatchet_sdk-0.9.4/hatchet_sdk/clients/admin.py`

 * *Files identical despite different names*

### Comparing `hatchet_sdk-0.9.3/hatchet_sdk/clients/dispatcher.py` & `hatchet_sdk-0.9.4/hatchet_sdk/clients/dispatcher.py`

 * *Files identical despite different names*

### Comparing `hatchet_sdk-0.9.3/hatchet_sdk/clients/events.py` & `hatchet_sdk-0.9.4/hatchet_sdk/clients/events.py`

 * *Files identical despite different names*

### Comparing `hatchet_sdk-0.9.3/hatchet_sdk/clients/listener.py` & `hatchet_sdk-0.9.4/hatchet_sdk/clients/listener.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List
 import grpc
 from ..dispatcher_pb2_grpc import DispatcherStub
 
-from ..dispatcher_pb2 import SubscribeToWorkflowEventsRequest, ResourceEventType
+from ..dispatcher_pb2 import SubscribeToWorkflowEventsRequest, ResourceEventType, WorkflowEvent, RESOURCE_TYPE_STEP_RUN, RESOURCE_TYPE_WORKFLOW_RUN
 from ..loader import ClientConfig
 from ..metadata import get_metadata
 import json
 import time
 
 
 DEFAULT_ACTION_LISTENER_RETRY_INTERVAL = 5  # seconds
@@ -16,98 +16,146 @@
 class StepRunEventType:
     STEP_RUN_EVENT_TYPE_STARTED = 'STEP_RUN_EVENT_TYPE_STARTED'
     STEP_RUN_EVENT_TYPE_COMPLETED = 'STEP_RUN_EVENT_TYPE_COMPLETED'
     STEP_RUN_EVENT_TYPE_FAILED = 'STEP_RUN_EVENT_TYPE_FAILED'
     STEP_RUN_EVENT_TYPE_CANCELLED = 'STEP_RUN_EVENT_TYPE_CANCELLED'
     STEP_RUN_EVENT_TYPE_TIMED_OUT = 'STEP_RUN_EVENT_TYPE_TIMED_OUT'
 
+class WorkflowRunEventType:
+    WORKFLOW_RUN_EVENT_TYPE_STARTED = 'WORKFLOW_RUN_EVENT_TYPE_STARTED'
+    WORKFLOW_RUN_EVENT_TYPE_COMPLETED = 'WORKFLOW_RUN_EVENT_TYPE_COMPLETED'
+    WORKFLOW_RUN_EVENT_TYPE_FAILED = 'WORKFLOW_RUN_EVENT_TYPE_FAILED'
+    WORKFLOW_RUN_EVENT_TYPE_CANCELLED = 'WORKFLOW_RUN_EVENT_TYPE_CANCELLED'
+    WORKFLOW_RUN_EVENT_TYPE_TIMED_OUT = 'WORKFLOW_RUN_EVENT_TYPE_TIMED_OUT'
 
-event_type_mapping = {
+step_run_event_type_mapping = {
     ResourceEventType.RESOURCE_EVENT_TYPE_STARTED: StepRunEventType.STEP_RUN_EVENT_TYPE_STARTED,
     ResourceEventType.RESOURCE_EVENT_TYPE_COMPLETED: StepRunEventType.STEP_RUN_EVENT_TYPE_COMPLETED,
     ResourceEventType.RESOURCE_EVENT_TYPE_FAILED: StepRunEventType.STEP_RUN_EVENT_TYPE_FAILED,
     ResourceEventType.RESOURCE_EVENT_TYPE_CANCELLED: StepRunEventType.STEP_RUN_EVENT_TYPE_CANCELLED,
     ResourceEventType.RESOURCE_EVENT_TYPE_TIMED_OUT: StepRunEventType.STEP_RUN_EVENT_TYPE_TIMED_OUT,
 }
 
+workflow_run_event_type_mapping = {
+    ResourceEventType.RESOURCE_EVENT_TYPE_STARTED: WorkflowRunEventType.WORKFLOW_RUN_EVENT_TYPE_STARTED,
+    ResourceEventType.RESOURCE_EVENT_TYPE_COMPLETED: WorkflowRunEventType.WORKFLOW_RUN_EVENT_TYPE_COMPLETED,
+    ResourceEventType.RESOURCE_EVENT_TYPE_FAILED: WorkflowRunEventType.WORKFLOW_RUN_EVENT_TYPE_FAILED,
+    ResourceEventType.RESOURCE_EVENT_TYPE_CANCELLED: WorkflowRunEventType.WORKFLOW_RUN_EVENT_TYPE_CANCELLED,
+    ResourceEventType.RESOURCE_EVENT_TYPE_TIMED_OUT: WorkflowRunEventType.WORKFLOW_RUN_EVENT_TYPE_TIMED_OUT,
+}
 
 class StepRunEvent:
     def __init__(self, type: StepRunEventType, payload: str):
         self.type = type
         self.payload = payload
 
 
 def new_listener(conn, config: ClientConfig):
     return ListenerClientImpl(
         client=DispatcherStub(conn),
         token=config.token,
     )
 
 
-class ListenerClientImpl:
-    def __init__(self, client: DispatcherStub, token):
+class HatchetListener:
+    def __init__(self, client: DispatcherStub, workflow_run_id: str, token: str):
         self.client = client
+        self.stop_signal = False
+        self.workflow_run_id = workflow_run_id
         self.token = token
 
-    async def generator(self, workflowRunId: str) -> List[StepRunEvent]:
-        listener = self.retry_subscribe(workflowRunId)
+    def __iter__(self):
+        return self._generator()
+
+    def abort(self):
+        self.stop_signal = True
+
+    def _generator(self, stop_step: str = None) -> List[StepRunEvent]:
+        listener = self.retry_subscribe()
+        while listener:
+            if self.stop_signal:
+                listener = None
+                break
 
-        while True:
             try:
                 for workflow_event in listener:
                     eventType = None
 
-                    if workflow_event.eventType in event_type_mapping:
-                        eventType = event_type_mapping[workflow_event.eventType]
-                    else:
-                        raise Exception(
-                            f"Unknown event type: {workflow_event.eventType}")
-
-                    payload = None
-                    if workflow_event.eventPayload:
-                        payload = json.loads(workflow_event.eventPayload)
-
-                    # call the handler
-                    event = StepRunEvent(type=eventType, payload=payload)
-                    yield event
+                    if workflow_event.resourceType == RESOURCE_TYPE_STEP_RUN:
+                        if workflow_event.eventType in step_run_event_type_mapping:
+                            eventType = step_run_event_type_mapping[workflow_event.eventType]
+                        else:
+                            raise Exception(
+                                f"Unknown event type: {workflow_event.eventType}")
+                        payload = None
+                        if workflow_event.eventPayload:
+                            payload = json.loads(workflow_event.eventPayload)
+
+                        # call the handler
+                        event = StepRunEvent(type=eventType, payload=payload)
+                        yield event
+                    elif workflow_event.resourceType == RESOURCE_TYPE_WORKFLOW_RUN:
+                        if workflow_event.eventType in workflow_run_event_type_mapping:
+                            eventType = workflow_run_event_type_mapping[workflow_event.eventType]
+                        else:
+                            raise Exception(
+                                f"Unknown event type: {workflow_event.eventType}")
+                        
+                        payload = None
+                        if workflow_event.eventPayload:
+                            payload = json.loads(workflow_event.eventPayload)
+                        
+                    if workflow_event.hangup:
+                        listener = None
+                        print('hangup stopping listener...')
+                        break
 
             except grpc.RpcError as e:
                 # Handle different types of errors
                 if e.code() == grpc.StatusCode.CANCELLED:
                     # Context cancelled, unsubscribe and close
                     break
                 elif e.code() == grpc.StatusCode.UNAVAILABLE:
                     # Retry logic
                     # logger.info("Could not connect to Hatchet, retrying...")
-                    listener = self.retry_subscribe(workflowRunId)
+                    listener = self.retry_subscribe()
                 elif e.code() == grpc.StatusCode.DEADLINE_EXCEEDED:
                     # logger.info("Deadline exceeded, retrying subscription")
                     continue
                 else:
                     # Unknown error, report and break
                     # logger.error(f"Failed to receive message: {e}")
                     break
 
-    def on(self, workflowRunId: str, handler: callable = None):
-        for event in self.generator(workflowRunId):
-            # call the handler if provided
-            if handler:
-                handler(event)
-
-    def retry_subscribe(self, workflowRunId: str):
+    def retry_subscribe(self):
         retries = 0
 
         while retries < DEFAULT_ACTION_LISTENER_RETRY_COUNT:
             try:
                 if retries > 0:
                     time.sleep(DEFAULT_ACTION_LISTENER_RETRY_INTERVAL)
 
                 listener = self.client.SubscribeToWorkflowEvents(
                     SubscribeToWorkflowEventsRequest(
-                        workflowRunId=workflowRunId,
+                        workflowRunId=self.workflow_run_id,
                     ), metadata=get_metadata(self.token))
                 return listener
             except grpc.RpcError as e:
                 if e.code() == grpc.StatusCode.UNAVAILABLE:
                     retries = retries + 1
                 else:
                     raise ValueError(f"gRPC error: {e}")
+
+
+class ListenerClientImpl:
+    def __init__(self, client: DispatcherStub, token: str):
+        self.client = client
+        self.token = token
+
+    def stream(self, workflow_run_id: str):
+        return HatchetListener(self.client, workflow_run_id, self.token)
+
+    def on(self, workflow_run_id: str, handler: callable = None):
+        for event in self.stream(workflow_run_id):
+            # call the handler if provided
+            if handler:
+                handler(event)
```

### Comparing `hatchet_sdk-0.9.3/hatchet_sdk/context.py` & `hatchet_sdk-0.9.4/hatchet_sdk/context.py`

 * *Files identical despite different names*

### Comparing `hatchet_sdk-0.9.3/hatchet_sdk/dispatcher_pb2.py` & `hatchet_sdk-0.9.4/hatchet_sdk/dispatcher_pb2.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,32 +11,32 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x64ispatcher.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"N\n\x15WorkerRegisterRequest\x12\x12\n\nworkerName\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x63tions\x18\x02 \x03(\t\x12\x10\n\x08services\x18\x03 \x03(\t\"P\n\x16WorkerRegisterResponse\x12\x10\n\x08tenantId\x18\x01 \x01(\t\x12\x10\n\x08workerId\x18\x02 \x01(\t\x12\x12\n\nworkerName\x18\x03 \x01(\t\"\xf2\x01\n\x0e\x41ssignedAction\x12\x10\n\x08tenantId\x18\x01 \x01(\t\x12\x15\n\rworkflowRunId\x18\x02 \x01(\t\x12\x18\n\x10getGroupKeyRunId\x18\x03 \x01(\t\x12\r\n\x05jobId\x18\x04 \x01(\t\x12\x0f\n\x07jobName\x18\x05 \x01(\t\x12\x10\n\x08jobRunId\x18\x06 \x01(\t\x12\x0e\n\x06stepId\x18\x07 \x01(\t\x12\x11\n\tstepRunId\x18\x08 \x01(\t\x12\x10\n\x08\x61\x63tionId\x18\t \x01(\t\x12\x1f\n\nactionType\x18\n \x01(\x0e\x32\x0b.ActionType\x12\x15\n\ractionPayload\x18\x0b \x01(\t\"\'\n\x13WorkerListenRequest\x12\x10\n\x08workerId\x18\x01 \x01(\t\",\n\x18WorkerUnsubscribeRequest\x12\x10\n\x08workerId\x18\x01 \x01(\t\"?\n\x19WorkerUnsubscribeResponse\x12\x10\n\x08tenantId\x18\x01 \x01(\t\x12\x10\n\x08workerId\x18\x02 \x01(\t\"\xe1\x01\n\x13GroupKeyActionEvent\x12\x10\n\x08workerId\x18\x01 \x01(\t\x12\x15\n\rworkflowRunId\x18\x02 \x01(\t\x12\x18\n\x10getGroupKeyRunId\x18\x03 \x01(\t\x12\x10\n\x08\x61\x63tionId\x18\x04 \x01(\t\x12\x32\n\x0e\x65ventTimestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\teventType\x18\x06 \x01(\x0e\x32\x18.GroupKeyActionEventType\x12\x14\n\x0c\x65ventPayload\x18\x07 \x01(\t\"\xec\x01\n\x0fStepActionEvent\x12\x10\n\x08workerId\x18\x01 \x01(\t\x12\r\n\x05jobId\x18\x02 \x01(\t\x12\x10\n\x08jobRunId\x18\x03 \x01(\t\x12\x0e\n\x06stepId\x18\x04 \x01(\t\x12\x11\n\tstepRunId\x18\x05 \x01(\t\x12\x10\n\x08\x61\x63tionId\x18\x06 \x01(\t\x12\x32\n\x0e\x65ventTimestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\teventType\x18\x08 \x01(\x0e\x32\x14.StepActionEventType\x12\x14\n\x0c\x65ventPayload\x18\t \x01(\t\"9\n\x13\x41\x63tionEventResponse\x12\x10\n\x08tenantId\x18\x01 \x01(\t\x12\x10\n\x08workerId\x18\x02 \x01(\t\"9\n SubscribeToWorkflowEventsRequest\x12\x15\n\rworkflowRunId\x18\x01 \x01(\t\"\xd0\x01\n\rWorkflowEvent\x12\x15\n\rworkflowRunId\x18\x01 \x01(\t\x12#\n\x0cresourceType\x18\x02 \x01(\x0e\x32\r.ResourceType\x12%\n\teventType\x18\x03 \x01(\x0e\x32\x12.ResourceEventType\x12\x12\n\nresourceId\x18\x04 \x01(\t\x12\x32\n\x0e\x65ventTimestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x0c\x65ventPayload\x18\x06 \x01(\t*N\n\nActionType\x12\x12\n\x0eSTART_STEP_RUN\x10\x00\x12\x13\n\x0f\x43\x41NCEL_STEP_RUN\x10\x01\x12\x17\n\x13START_GET_GROUP_KEY\x10\x02*\xa2\x01\n\x17GroupKeyActionEventType\x12 \n\x1cGROUP_KEY_EVENT_TYPE_UNKNOWN\x10\x00\x12 \n\x1cGROUP_KEY_EVENT_TYPE_STARTED\x10\x01\x12\"\n\x1eGROUP_KEY_EVENT_TYPE_COMPLETED\x10\x02\x12\x1f\n\x1bGROUP_KEY_EVENT_TYPE_FAILED\x10\x03*\x8a\x01\n\x13StepActionEventType\x12\x1b\n\x17STEP_EVENT_TYPE_UNKNOWN\x10\x00\x12\x1b\n\x17STEP_EVENT_TYPE_STARTED\x10\x01\x12\x1d\n\x19STEP_EVENT_TYPE_COMPLETED\x10\x02\x12\x1a\n\x16STEP_EVENT_TYPE_FAILED\x10\x03*e\n\x0cResourceType\x12\x19\n\x15RESOURCE_TYPE_UNKNOWN\x10\x00\x12\x1a\n\x16RESOURCE_TYPE_STEP_RUN\x10\x01\x12\x1e\n\x1aRESOURCE_TYPE_WORKFLOW_RUN\x10\x02*\xde\x01\n\x11ResourceEventType\x12\x1f\n\x1bRESOURCE_EVENT_TYPE_UNKNOWN\x10\x00\x12\x1f\n\x1bRESOURCE_EVENT_TYPE_STARTED\x10\x01\x12!\n\x1dRESOURCE_EVENT_TYPE_COMPLETED\x10\x02\x12\x1e\n\x1aRESOURCE_EVENT_TYPE_FAILED\x10\x03\x12!\n\x1dRESOURCE_EVENT_TYPE_CANCELLED\x10\x04\x12!\n\x1dRESOURCE_EVENT_TYPE_TIMED_OUT\x10\x05\x32\xa6\x03\n\nDispatcher\x12=\n\x08Register\x12\x16.WorkerRegisterRequest\x1a\x17.WorkerRegisterResponse\"\x00\x12\x33\n\x06Listen\x12\x14.WorkerListenRequest\x1a\x0f.AssignedAction\"\x00\x30\x01\x12R\n\x19SubscribeToWorkflowEvents\x12!.SubscribeToWorkflowEventsRequest\x1a\x0e.WorkflowEvent\"\x00\x30\x01\x12?\n\x13SendStepActionEvent\x12\x10.StepActionEvent\x1a\x14.ActionEventResponse\"\x00\x12G\n\x17SendGroupKeyActionEvent\x12\x14.GroupKeyActionEvent\x1a\x14.ActionEventResponse\"\x00\x12\x46\n\x0bUnsubscribe\x12\x19.WorkerUnsubscribeRequest\x1a\x1a.WorkerUnsubscribeResponse\"\x00\x42GZEgithub.com/hatchet-dev/hatchet/internal/services/dispatcher/contractsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x10\x64ispatcher.proto\x1a\x1fgoogle/protobuf/timestamp.proto\"N\n\x15WorkerRegisterRequest\x12\x12\n\nworkerName\x18\x01 \x01(\t\x12\x0f\n\x07\x61\x63tions\x18\x02 \x03(\t\x12\x10\n\x08services\x18\x03 \x03(\t\"P\n\x16WorkerRegisterResponse\x12\x10\n\x08tenantId\x18\x01 \x01(\t\x12\x10\n\x08workerId\x18\x02 \x01(\t\x12\x12\n\nworkerName\x18\x03 \x01(\t\"\xf2\x01\n\x0e\x41ssignedAction\x12\x10\n\x08tenantId\x18\x01 \x01(\t\x12\x15\n\rworkflowRunId\x18\x02 \x01(\t\x12\x18\n\x10getGroupKeyRunId\x18\x03 \x01(\t\x12\r\n\x05jobId\x18\x04 \x01(\t\x12\x0f\n\x07jobName\x18\x05 \x01(\t\x12\x10\n\x08jobRunId\x18\x06 \x01(\t\x12\x0e\n\x06stepId\x18\x07 \x01(\t\x12\x11\n\tstepRunId\x18\x08 \x01(\t\x12\x10\n\x08\x61\x63tionId\x18\t \x01(\t\x12\x1f\n\nactionType\x18\n \x01(\x0e\x32\x0b.ActionType\x12\x15\n\ractionPayload\x18\x0b \x01(\t\"\'\n\x13WorkerListenRequest\x12\x10\n\x08workerId\x18\x01 \x01(\t\",\n\x18WorkerUnsubscribeRequest\x12\x10\n\x08workerId\x18\x01 \x01(\t\"?\n\x19WorkerUnsubscribeResponse\x12\x10\n\x08tenantId\x18\x01 \x01(\t\x12\x10\n\x08workerId\x18\x02 \x01(\t\"\xe1\x01\n\x13GroupKeyActionEvent\x12\x10\n\x08workerId\x18\x01 \x01(\t\x12\x15\n\rworkflowRunId\x18\x02 \x01(\t\x12\x18\n\x10getGroupKeyRunId\x18\x03 \x01(\t\x12\x10\n\x08\x61\x63tionId\x18\x04 \x01(\t\x12\x32\n\x0e\x65ventTimestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\teventType\x18\x06 \x01(\x0e\x32\x18.GroupKeyActionEventType\x12\x14\n\x0c\x65ventPayload\x18\x07 \x01(\t\"\xec\x01\n\x0fStepActionEvent\x12\x10\n\x08workerId\x18\x01 \x01(\t\x12\r\n\x05jobId\x18\x02 \x01(\t\x12\x10\n\x08jobRunId\x18\x03 \x01(\t\x12\x0e\n\x06stepId\x18\x04 \x01(\t\x12\x11\n\tstepRunId\x18\x05 \x01(\t\x12\x10\n\x08\x61\x63tionId\x18\x06 \x01(\t\x12\x32\n\x0e\x65ventTimestamp\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\'\n\teventType\x18\x08 \x01(\x0e\x32\x14.StepActionEventType\x12\x14\n\x0c\x65ventPayload\x18\t \x01(\t\"9\n\x13\x41\x63tionEventResponse\x12\x10\n\x08tenantId\x18\x01 \x01(\t\x12\x10\n\x08workerId\x18\x02 \x01(\t\"9\n SubscribeToWorkflowEventsRequest\x12\x15\n\rworkflowRunId\x18\x01 \x01(\t\"\xe0\x01\n\rWorkflowEvent\x12\x15\n\rworkflowRunId\x18\x01 \x01(\t\x12#\n\x0cresourceType\x18\x02 \x01(\x0e\x32\r.ResourceType\x12%\n\teventType\x18\x03 \x01(\x0e\x32\x12.ResourceEventType\x12\x12\n\nresourceId\x18\x04 \x01(\t\x12\x32\n\x0e\x65ventTimestamp\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x14\n\x0c\x65ventPayload\x18\x06 \x01(\t\x12\x0e\n\x06hangup\x18\x07 \x01(\x08*N\n\nActionType\x12\x12\n\x0eSTART_STEP_RUN\x10\x00\x12\x13\n\x0f\x43\x41NCEL_STEP_RUN\x10\x01\x12\x17\n\x13START_GET_GROUP_KEY\x10\x02*\xa2\x01\n\x17GroupKeyActionEventType\x12 \n\x1cGROUP_KEY_EVENT_TYPE_UNKNOWN\x10\x00\x12 \n\x1cGROUP_KEY_EVENT_TYPE_STARTED\x10\x01\x12\"\n\x1eGROUP_KEY_EVENT_TYPE_COMPLETED\x10\x02\x12\x1f\n\x1bGROUP_KEY_EVENT_TYPE_FAILED\x10\x03*\x8a\x01\n\x13StepActionEventType\x12\x1b\n\x17STEP_EVENT_TYPE_UNKNOWN\x10\x00\x12\x1b\n\x17STEP_EVENT_TYPE_STARTED\x10\x01\x12\x1d\n\x19STEP_EVENT_TYPE_COMPLETED\x10\x02\x12\x1a\n\x16STEP_EVENT_TYPE_FAILED\x10\x03*e\n\x0cResourceType\x12\x19\n\x15RESOURCE_TYPE_UNKNOWN\x10\x00\x12\x1a\n\x16RESOURCE_TYPE_STEP_RUN\x10\x01\x12\x1e\n\x1aRESOURCE_TYPE_WORKFLOW_RUN\x10\x02*\xde\x01\n\x11ResourceEventType\x12\x1f\n\x1bRESOURCE_EVENT_TYPE_UNKNOWN\x10\x00\x12\x1f\n\x1bRESOURCE_EVENT_TYPE_STARTED\x10\x01\x12!\n\x1dRESOURCE_EVENT_TYPE_COMPLETED\x10\x02\x12\x1e\n\x1aRESOURCE_EVENT_TYPE_FAILED\x10\x03\x12!\n\x1dRESOURCE_EVENT_TYPE_CANCELLED\x10\x04\x12!\n\x1dRESOURCE_EVENT_TYPE_TIMED_OUT\x10\x05\x32\xa6\x03\n\nDispatcher\x12=\n\x08Register\x12\x16.WorkerRegisterRequest\x1a\x17.WorkerRegisterResponse\"\x00\x12\x33\n\x06Listen\x12\x14.WorkerListenRequest\x1a\x0f.AssignedAction\"\x00\x30\x01\x12R\n\x19SubscribeToWorkflowEvents\x12!.SubscribeToWorkflowEventsRequest\x1a\x0e.WorkflowEvent\"\x00\x30\x01\x12?\n\x13SendStepActionEvent\x12\x10.StepActionEvent\x1a\x14.ActionEventResponse\"\x00\x12G\n\x17SendGroupKeyActionEvent\x12\x14.GroupKeyActionEvent\x1a\x14.ActionEventResponse\"\x00\x12\x46\n\x0bUnsubscribe\x12\x19.WorkerUnsubscribeRequest\x1a\x1a.WorkerUnsubscribeResponse\"\x00\x42GZEgithub.com/hatchet-dev/hatchet/internal/services/dispatcher/contractsb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'dispatcher_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'ZEgithub.com/hatchet-dev/hatchet/internal/services/dispatcher/contracts'
-  _globals['_ACTIONTYPE']._serialized_start=1408
-  _globals['_ACTIONTYPE']._serialized_end=1486
-  _globals['_GROUPKEYACTIONEVENTTYPE']._serialized_start=1489
-  _globals['_GROUPKEYACTIONEVENTTYPE']._serialized_end=1651
-  _globals['_STEPACTIONEVENTTYPE']._serialized_start=1654
-  _globals['_STEPACTIONEVENTTYPE']._serialized_end=1792
-  _globals['_RESOURCETYPE']._serialized_start=1794
-  _globals['_RESOURCETYPE']._serialized_end=1895
-  _globals['_RESOURCEEVENTTYPE']._serialized_start=1898
-  _globals['_RESOURCEEVENTTYPE']._serialized_end=2120
+  _globals['_ACTIONTYPE']._serialized_start=1424
+  _globals['_ACTIONTYPE']._serialized_end=1502
+  _globals['_GROUPKEYACTIONEVENTTYPE']._serialized_start=1505
+  _globals['_GROUPKEYACTIONEVENTTYPE']._serialized_end=1667
+  _globals['_STEPACTIONEVENTTYPE']._serialized_start=1670
+  _globals['_STEPACTIONEVENTTYPE']._serialized_end=1808
+  _globals['_RESOURCETYPE']._serialized_start=1810
+  _globals['_RESOURCETYPE']._serialized_end=1911
+  _globals['_RESOURCEEVENTTYPE']._serialized_start=1914
+  _globals['_RESOURCEEVENTTYPE']._serialized_end=2136
   _globals['_WORKERREGISTERREQUEST']._serialized_start=53
   _globals['_WORKERREGISTERREQUEST']._serialized_end=131
   _globals['_WORKERREGISTERRESPONSE']._serialized_start=133
   _globals['_WORKERREGISTERRESPONSE']._serialized_end=213
   _globals['_ASSIGNEDACTION']._serialized_start=216
   _globals['_ASSIGNEDACTION']._serialized_end=458
   _globals['_WORKERLISTENREQUEST']._serialized_start=460
@@ -50,11 +50,11 @@
   _globals['_STEPACTIONEVENT']._serialized_start=841
   _globals['_STEPACTIONEVENT']._serialized_end=1077
   _globals['_ACTIONEVENTRESPONSE']._serialized_start=1079
   _globals['_ACTIONEVENTRESPONSE']._serialized_end=1136
   _globals['_SUBSCRIBETOWORKFLOWEVENTSREQUEST']._serialized_start=1138
   _globals['_SUBSCRIBETOWORKFLOWEVENTSREQUEST']._serialized_end=1195
   _globals['_WORKFLOWEVENT']._serialized_start=1198
-  _globals['_WORKFLOWEVENT']._serialized_end=1406
-  _globals['_DISPATCHER']._serialized_start=2123
-  _globals['_DISPATCHER']._serialized_end=2545
+  _globals['_WORKFLOWEVENT']._serialized_end=1422
+  _globals['_DISPATCHER']._serialized_start=2139
+  _globals['_DISPATCHER']._serialized_end=2561
 # @@protoc_insertion_point(module_scope)
```

### Comparing `hatchet_sdk-0.9.3/hatchet_sdk/dispatcher_pb2.pyi` & `hatchet_sdk-0.9.4/hatchet_sdk/dispatcher_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -179,21 +179,23 @@
 class SubscribeToWorkflowEventsRequest(_message.Message):
     __slots__ = ("workflowRunId",)
     WORKFLOWRUNID_FIELD_NUMBER: _ClassVar[int]
     workflowRunId: str
     def __init__(self, workflowRunId: _Optional[str] = ...) -> None: ...
 
 class WorkflowEvent(_message.Message):
-    __slots__ = ("workflowRunId", "resourceType", "eventType", "resourceId", "eventTimestamp", "eventPayload")
+    __slots__ = ("workflowRunId", "resourceType", "eventType", "resourceId", "eventTimestamp", "eventPayload", "hangup")
     WORKFLOWRUNID_FIELD_NUMBER: _ClassVar[int]
     RESOURCETYPE_FIELD_NUMBER: _ClassVar[int]
     EVENTTYPE_FIELD_NUMBER: _ClassVar[int]
     RESOURCEID_FIELD_NUMBER: _ClassVar[int]
     EVENTTIMESTAMP_FIELD_NUMBER: _ClassVar[int]
     EVENTPAYLOAD_FIELD_NUMBER: _ClassVar[int]
+    HANGUP_FIELD_NUMBER: _ClassVar[int]
     workflowRunId: str
     resourceType: ResourceType
     eventType: ResourceEventType
     resourceId: str
     eventTimestamp: _timestamp_pb2.Timestamp
     eventPayload: str
-    def __init__(self, workflowRunId: _Optional[str] = ..., resourceType: _Optional[_Union[ResourceType, str]] = ..., eventType: _Optional[_Union[ResourceEventType, str]] = ..., resourceId: _Optional[str] = ..., eventTimestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., eventPayload: _Optional[str] = ...) -> None: ...
+    hangup: bool
+    def __init__(self, workflowRunId: _Optional[str] = ..., resourceType: _Optional[_Union[ResourceType, str]] = ..., eventType: _Optional[_Union[ResourceEventType, str]] = ..., resourceId: _Optional[str] = ..., eventTimestamp: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., eventPayload: _Optional[str] = ..., hangup: bool = ...) -> None: ...
```

### Comparing `hatchet_sdk-0.9.3/hatchet_sdk/dispatcher_pb2_grpc.py` & `hatchet_sdk-0.9.4/hatchet_sdk/dispatcher_pb2_grpc.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,43 +11,43 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.Register = channel.unary_unary(
-            '/Dispatcher/Register',
-            request_serializer=dispatcher__pb2.WorkerRegisterRequest.SerializeToString,
-            response_deserializer=dispatcher__pb2.WorkerRegisterResponse.FromString,
-        )
+                '/Dispatcher/Register',
+                request_serializer=dispatcher__pb2.WorkerRegisterRequest.SerializeToString,
+                response_deserializer=dispatcher__pb2.WorkerRegisterResponse.FromString,
+                )
         self.Listen = channel.unary_stream(
-            '/Dispatcher/Listen',
-            request_serializer=dispatcher__pb2.WorkerListenRequest.SerializeToString,
-            response_deserializer=dispatcher__pb2.AssignedAction.FromString,
-        )
+                '/Dispatcher/Listen',
+                request_serializer=dispatcher__pb2.WorkerListenRequest.SerializeToString,
+                response_deserializer=dispatcher__pb2.AssignedAction.FromString,
+                )
         self.SubscribeToWorkflowEvents = channel.unary_stream(
-            '/Dispatcher/SubscribeToWorkflowEvents',
-            request_serializer=dispatcher__pb2.SubscribeToWorkflowEventsRequest.SerializeToString,
-            response_deserializer=dispatcher__pb2.WorkflowEvent.FromString,
-        )
+                '/Dispatcher/SubscribeToWorkflowEvents',
+                request_serializer=dispatcher__pb2.SubscribeToWorkflowEventsRequest.SerializeToString,
+                response_deserializer=dispatcher__pb2.WorkflowEvent.FromString,
+                )
         self.SendStepActionEvent = channel.unary_unary(
-            '/Dispatcher/SendStepActionEvent',
-            request_serializer=dispatcher__pb2.StepActionEvent.SerializeToString,
-            response_deserializer=dispatcher__pb2.ActionEventResponse.FromString,
-        )
+                '/Dispatcher/SendStepActionEvent',
+                request_serializer=dispatcher__pb2.StepActionEvent.SerializeToString,
+                response_deserializer=dispatcher__pb2.ActionEventResponse.FromString,
+                )
         self.SendGroupKeyActionEvent = channel.unary_unary(
-            '/Dispatcher/SendGroupKeyActionEvent',
-            request_serializer=dispatcher__pb2.GroupKeyActionEvent.SerializeToString,
-            response_deserializer=dispatcher__pb2.ActionEventResponse.FromString,
-        )
+                '/Dispatcher/SendGroupKeyActionEvent',
+                request_serializer=dispatcher__pb2.GroupKeyActionEvent.SerializeToString,
+                response_deserializer=dispatcher__pb2.ActionEventResponse.FromString,
+                )
         self.Unsubscribe = channel.unary_unary(
-            '/Dispatcher/Unsubscribe',
-            request_serializer=dispatcher__pb2.WorkerUnsubscribeRequest.SerializeToString,
-            response_deserializer=dispatcher__pb2.WorkerUnsubscribeResponse.FromString,
-        )
+                '/Dispatcher/Unsubscribe',
+                request_serializer=dispatcher__pb2.WorkerUnsubscribeRequest.SerializeToString,
+                response_deserializer=dispatcher__pb2.WorkerUnsubscribeResponse.FromString,
+                )
 
 
 class DispatcherServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def Register(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -84,149 +84,148 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_DispatcherServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        'Register': grpc.unary_unary_rpc_method_handler(
-            servicer.Register,
-            request_deserializer=dispatcher__pb2.WorkerRegisterRequest.FromString,
-            response_serializer=dispatcher__pb2.WorkerRegisterResponse.SerializeToString,
-        ),
-        'Listen': grpc.unary_stream_rpc_method_handler(
-            servicer.Listen,
-            request_deserializer=dispatcher__pb2.WorkerListenRequest.FromString,
-            response_serializer=dispatcher__pb2.AssignedAction.SerializeToString,
-        ),
-        'SubscribeToWorkflowEvents': grpc.unary_stream_rpc_method_handler(
-            servicer.SubscribeToWorkflowEvents,
-            request_deserializer=dispatcher__pb2.SubscribeToWorkflowEventsRequest.FromString,
-            response_serializer=dispatcher__pb2.WorkflowEvent.SerializeToString,
-        ),
-        'SendStepActionEvent': grpc.unary_unary_rpc_method_handler(
-            servicer.SendStepActionEvent,
-            request_deserializer=dispatcher__pb2.StepActionEvent.FromString,
-            response_serializer=dispatcher__pb2.ActionEventResponse.SerializeToString,
-        ),
-        'SendGroupKeyActionEvent': grpc.unary_unary_rpc_method_handler(
-            servicer.SendGroupKeyActionEvent,
-            request_deserializer=dispatcher__pb2.GroupKeyActionEvent.FromString,
-            response_serializer=dispatcher__pb2.ActionEventResponse.SerializeToString,
-        ),
-        'Unsubscribe': grpc.unary_unary_rpc_method_handler(
-            servicer.Unsubscribe,
-            request_deserializer=dispatcher__pb2.WorkerUnsubscribeRequest.FromString,
-            response_serializer=dispatcher__pb2.WorkerUnsubscribeResponse.SerializeToString,
-        ),
+            'Register': grpc.unary_unary_rpc_method_handler(
+                    servicer.Register,
+                    request_deserializer=dispatcher__pb2.WorkerRegisterRequest.FromString,
+                    response_serializer=dispatcher__pb2.WorkerRegisterResponse.SerializeToString,
+            ),
+            'Listen': grpc.unary_stream_rpc_method_handler(
+                    servicer.Listen,
+                    request_deserializer=dispatcher__pb2.WorkerListenRequest.FromString,
+                    response_serializer=dispatcher__pb2.AssignedAction.SerializeToString,
+            ),
+            'SubscribeToWorkflowEvents': grpc.unary_stream_rpc_method_handler(
+                    servicer.SubscribeToWorkflowEvents,
+                    request_deserializer=dispatcher__pb2.SubscribeToWorkflowEventsRequest.FromString,
+                    response_serializer=dispatcher__pb2.WorkflowEvent.SerializeToString,
+            ),
+            'SendStepActionEvent': grpc.unary_unary_rpc_method_handler(
+                    servicer.SendStepActionEvent,
+                    request_deserializer=dispatcher__pb2.StepActionEvent.FromString,
+                    response_serializer=dispatcher__pb2.ActionEventResponse.SerializeToString,
+            ),
+            'SendGroupKeyActionEvent': grpc.unary_unary_rpc_method_handler(
+                    servicer.SendGroupKeyActionEvent,
+                    request_deserializer=dispatcher__pb2.GroupKeyActionEvent.FromString,
+                    response_serializer=dispatcher__pb2.ActionEventResponse.SerializeToString,
+            ),
+            'Unsubscribe': grpc.unary_unary_rpc_method_handler(
+                    servicer.Unsubscribe,
+                    request_deserializer=dispatcher__pb2.WorkerUnsubscribeRequest.FromString,
+                    response_serializer=dispatcher__pb2.WorkerUnsubscribeResponse.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        'Dispatcher', rpc_method_handlers)
+            'Dispatcher', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
- # This class is part of an EXPERIMENTAL API.
-
 
+ # This class is part of an EXPERIMENTAL API.
 class Dispatcher(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
     def Register(request,
-                 target,
-                 options=(),
-                 channel_credentials=None,
-                 call_credentials=None,
-                 insecure=False,
-                 compression=None,
-                 wait_for_ready=None,
-                 timeout=None,
-                 metadata=None):
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
         return grpc.experimental.unary_unary(request, target, '/Dispatcher/Register',
-                                             dispatcher__pb2.WorkerRegisterRequest.SerializeToString,
-                                             dispatcher__pb2.WorkerRegisterResponse.FromString,
-                                             options, channel_credentials,
-                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            dispatcher__pb2.WorkerRegisterRequest.SerializeToString,
+            dispatcher__pb2.WorkerRegisterResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def Listen(request,
-               target,
-               options=(),
-               channel_credentials=None,
-               call_credentials=None,
-               insecure=False,
-               compression=None,
-               wait_for_ready=None,
-               timeout=None,
-               metadata=None):
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
         return grpc.experimental.unary_stream(request, target, '/Dispatcher/Listen',
-                                              dispatcher__pb2.WorkerListenRequest.SerializeToString,
-                                              dispatcher__pb2.AssignedAction.FromString,
-                                              options, channel_credentials,
-                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            dispatcher__pb2.WorkerListenRequest.SerializeToString,
+            dispatcher__pb2.AssignedAction.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def SubscribeToWorkflowEvents(request,
-                                  target,
-                                  options=(),
-                                  channel_credentials=None,
-                                  call_credentials=None,
-                                  insecure=False,
-                                  compression=None,
-                                  wait_for_ready=None,
-                                  timeout=None,
-                                  metadata=None):
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
         return grpc.experimental.unary_stream(request, target, '/Dispatcher/SubscribeToWorkflowEvents',
-                                              dispatcher__pb2.SubscribeToWorkflowEventsRequest.SerializeToString,
-                                              dispatcher__pb2.WorkflowEvent.FromString,
-                                              options, channel_credentials,
-                                              insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            dispatcher__pb2.SubscribeToWorkflowEventsRequest.SerializeToString,
+            dispatcher__pb2.WorkflowEvent.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def SendStepActionEvent(request,
-                            target,
-                            options=(),
-                            channel_credentials=None,
-                            call_credentials=None,
-                            insecure=False,
-                            compression=None,
-                            wait_for_ready=None,
-                            timeout=None,
-                            metadata=None):
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
         return grpc.experimental.unary_unary(request, target, '/Dispatcher/SendStepActionEvent',
-                                             dispatcher__pb2.StepActionEvent.SerializeToString,
-                                             dispatcher__pb2.ActionEventResponse.FromString,
-                                             options, channel_credentials,
-                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            dispatcher__pb2.StepActionEvent.SerializeToString,
+            dispatcher__pb2.ActionEventResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def SendGroupKeyActionEvent(request,
-                                target,
-                                options=(),
-                                channel_credentials=None,
-                                call_credentials=None,
-                                insecure=False,
-                                compression=None,
-                                wait_for_ready=None,
-                                timeout=None,
-                                metadata=None):
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
         return grpc.experimental.unary_unary(request, target, '/Dispatcher/SendGroupKeyActionEvent',
-                                             dispatcher__pb2.GroupKeyActionEvent.SerializeToString,
-                                             dispatcher__pb2.ActionEventResponse.FromString,
-                                             options, channel_credentials,
-                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            dispatcher__pb2.GroupKeyActionEvent.SerializeToString,
+            dispatcher__pb2.ActionEventResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def Unsubscribe(request,
-                    target,
-                    options=(),
-                    channel_credentials=None,
-                    call_credentials=None,
-                    insecure=False,
-                    compression=None,
-                    wait_for_ready=None,
-                    timeout=None,
-                    metadata=None):
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
         return grpc.experimental.unary_unary(request, target, '/Dispatcher/Unsubscribe',
-                                             dispatcher__pb2.WorkerUnsubscribeRequest.SerializeToString,
-                                             dispatcher__pb2.WorkerUnsubscribeResponse.FromString,
-                                             options, channel_credentials,
-                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            dispatcher__pb2.WorkerUnsubscribeRequest.SerializeToString,
+            dispatcher__pb2.WorkerUnsubscribeResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `hatchet_sdk-0.9.3/hatchet_sdk/events_pb2.py` & `hatchet_sdk-0.9.4/hatchet_sdk/events_pb2.py`

 * *Files identical despite different names*

### Comparing `hatchet_sdk-0.9.3/hatchet_sdk/events_pb2.pyi` & `hatchet_sdk-0.9.4/hatchet_sdk/events_pb2.pyi`

 * *Files identical despite different names*

### Comparing `hatchet_sdk-0.9.3/hatchet_sdk/events_pb2_grpc.py` & `hatchet_sdk-0.9.4/hatchet_sdk/events_pb2_grpc.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,28 +11,28 @@
     def __init__(self, channel):
         """Constructor.
 
         Args:
             channel: A grpc.Channel.
         """
         self.Push = channel.unary_unary(
-            '/EventsService/Push',
-            request_serializer=events__pb2.PushEventRequest.SerializeToString,
-            response_deserializer=events__pb2.Event.FromString,
-        )
+                '/EventsService/Push',
+                request_serializer=events__pb2.PushEventRequest.SerializeToString,
+                response_deserializer=events__pb2.Event.FromString,
+                )
         self.List = channel.unary_unary(
-            '/EventsService/List',
-            request_serializer=events__pb2.ListEventRequest.SerializeToString,
-            response_deserializer=events__pb2.ListEventResponse.FromString,
-        )
+                '/EventsService/List',
+                request_serializer=events__pb2.ListEventRequest.SerializeToString,
+                response_deserializer=events__pb2.ListEventResponse.FromString,
+                )
         self.ReplaySingleEvent = channel.unary_unary(
-            '/EventsService/ReplaySingleEvent',
-            request_serializer=events__pb2.ReplayEventRequest.SerializeToString,
-            response_deserializer=events__pb2.Event.FromString,
-        )
+                '/EventsService/ReplaySingleEvent',
+                request_serializer=events__pb2.ReplayEventRequest.SerializeToString,
+                response_deserializer=events__pb2.Event.FromString,
+                )
 
 
 class EventsServiceServicer(object):
     """Missing associated documentation comment in .proto file."""
 
     def Push(self, request, context):
         """Missing associated documentation comment in .proto file."""
@@ -51,83 +51,82 @@
         context.set_code(grpc.StatusCode.UNIMPLEMENTED)
         context.set_details('Method not implemented!')
         raise NotImplementedError('Method not implemented!')
 
 
 def add_EventsServiceServicer_to_server(servicer, server):
     rpc_method_handlers = {
-        'Push': grpc.unary_unary_rpc_method_handler(
-            servicer.Push,
-            request_deserializer=events__pb2.PushEventRequest.FromString,
-            response_serializer=events__pb2.Event.SerializeToString,
-        ),
-        'List': grpc.unary_unary_rpc_method_handler(
-            servicer.List,
-            request_deserializer=events__pb2.ListEventRequest.FromString,
-            response_serializer=events__pb2.ListEventResponse.SerializeToString,
-        ),
-        'ReplaySingleEvent': grpc.unary_unary_rpc_method_handler(
-            servicer.ReplaySingleEvent,
-            request_deserializer=events__pb2.ReplayEventRequest.FromString,
-            response_serializer=events__pb2.Event.SerializeToString,
-        ),
+            'Push': grpc.unary_unary_rpc_method_handler(
+                    servicer.Push,
+                    request_deserializer=events__pb2.PushEventRequest.FromString,
+                    response_serializer=events__pb2.Event.SerializeToString,
+            ),
+            'List': grpc.unary_unary_rpc_method_handler(
+                    servicer.List,
+                    request_deserializer=events__pb2.ListEventRequest.FromString,
+                    response_serializer=events__pb2.ListEventResponse.SerializeToString,
+            ),
+            'ReplaySingleEvent': grpc.unary_unary_rpc_method_handler(
+                    servicer.ReplaySingleEvent,
+                    request_deserializer=events__pb2.ReplayEventRequest.FromString,
+                    response_serializer=events__pb2.Event.SerializeToString,
+            ),
     }
     generic_handler = grpc.method_handlers_generic_handler(
-        'EventsService', rpc_method_handlers)
+            'EventsService', rpc_method_handlers)
     server.add_generic_rpc_handlers((generic_handler,))
 
- # This class is part of an EXPERIMENTAL API.
-
 
+ # This class is part of an EXPERIMENTAL API.
 class EventsService(object):
     """Missing associated documentation comment in .proto file."""
 
     @staticmethod
     def Push(request,
-             target,
-             options=(),
-             channel_credentials=None,
-             call_credentials=None,
-             insecure=False,
-             compression=None,
-             wait_for_ready=None,
-             timeout=None,
-             metadata=None):
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
         return grpc.experimental.unary_unary(request, target, '/EventsService/Push',
-                                             events__pb2.PushEventRequest.SerializeToString,
-                                             events__pb2.Event.FromString,
-                                             options, channel_credentials,
-                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            events__pb2.PushEventRequest.SerializeToString,
+            events__pb2.Event.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def List(request,
-             target,
-             options=(),
-             channel_credentials=None,
-             call_credentials=None,
-             insecure=False,
-             compression=None,
-             wait_for_ready=None,
-             timeout=None,
-             metadata=None):
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
         return grpc.experimental.unary_unary(request, target, '/EventsService/List',
-                                             events__pb2.ListEventRequest.SerializeToString,
-                                             events__pb2.ListEventResponse.FromString,
-                                             options, channel_credentials,
-                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            events__pb2.ListEventRequest.SerializeToString,
+            events__pb2.ListEventResponse.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
 
     @staticmethod
     def ReplaySingleEvent(request,
-                          target,
-                          options=(),
-                          channel_credentials=None,
-                          call_credentials=None,
-                          insecure=False,
-                          compression=None,
-                          wait_for_ready=None,
-                          timeout=None,
-                          metadata=None):
+            target,
+            options=(),
+            channel_credentials=None,
+            call_credentials=None,
+            insecure=False,
+            compression=None,
+            wait_for_ready=None,
+            timeout=None,
+            metadata=None):
         return grpc.experimental.unary_unary(request, target, '/EventsService/ReplaySingleEvent',
-                                             events__pb2.ReplayEventRequest.SerializeToString,
-                                             events__pb2.Event.FromString,
-                                             options, channel_credentials,
-                                             insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
+            events__pb2.ReplayEventRequest.SerializeToString,
+            events__pb2.Event.FromString,
+            options, channel_credentials,
+            insecure, call_credentials, compression, wait_for_ready, timeout, metadata)
```

### Comparing `hatchet_sdk-0.9.3/hatchet_sdk/hatchet.py` & `hatchet_sdk-0.9.4/hatchet_sdk/hatchet.py`

 * *Files identical despite different names*

### Comparing `hatchet_sdk-0.9.3/hatchet_sdk/loader.py` & `hatchet_sdk-0.9.4/hatchet_sdk/loader.py`

 * *Files identical despite different names*

### Comparing `hatchet_sdk-0.9.3/hatchet_sdk/semver.py` & `hatchet_sdk-0.9.4/hatchet_sdk/semver.py`

 * *Files identical despite different names*

### Comparing `hatchet_sdk-0.9.3/hatchet_sdk/token.py` & `hatchet_sdk-0.9.4/hatchet_sdk/token.py`

 * *Files identical despite different names*

### Comparing `hatchet_sdk-0.9.3/hatchet_sdk/worker.py` & `hatchet_sdk-0.9.4/hatchet_sdk/worker.py`

 * *Files identical despite different names*

### Comparing `hatchet_sdk-0.9.3/hatchet_sdk/workflow.py` & `hatchet_sdk-0.9.4/hatchet_sdk/workflow.py`

 * *Files identical despite different names*

### Comparing `hatchet_sdk-0.9.3/hatchet_sdk/workflows_pb2.py` & `hatchet_sdk-0.9.4/hatchet_sdk/workflows_pb2.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,60 +12,60 @@
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from google.protobuf import wrappers_pb2 as google_dot_protobuf_dot_wrappers__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fworkflows.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\">\n\x12PutWorkflowRequest\x12(\n\x04opts\x18\x01 \x01(\x0b\x32\x1a.CreateWorkflowVersionOpts\"\x8b\x02\n\x19\x43reateWorkflowVersionOpts\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x16\n\x0e\x65vent_triggers\x18\x04 \x03(\t\x12\x15\n\rcron_triggers\x18\x05 \x03(\t\x12\x36\n\x12scheduled_triggers\x18\x06 \x03(\x0b\x32\x1a.google.protobuf.Timestamp\x12$\n\x04jobs\x18\x07 \x03(\x0b\x32\x16.CreateWorkflowJobOpts\x12-\n\x0b\x63oncurrency\x18\x08 \x01(\x0b\x32\x18.WorkflowConcurrencyOpts\"n\n\x17WorkflowConcurrencyOpts\x12\x0e\n\x06\x61\x63tion\x18\x01 \x01(\t\x12\x10\n\x08max_runs\x18\x02 \x01(\x05\x12\x31\n\x0elimit_strategy\x18\x03 \x01(\x0e\x32\x19.ConcurrencyLimitStrategy\"s\n\x15\x43reateWorkflowJobOpts\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\t\x12&\n\x05steps\x18\x04 \x03(\x0b\x32\x17.CreateWorkflowStepOpts\"o\n\x16\x43reateWorkflowStepOpts\x12\x13\n\x0breadable_id\x18\x01 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\t\x12\x0e\n\x06inputs\x18\x04 \x01(\t\x12\x0f\n\x07parents\x18\x05 \x03(\t\"\x16\n\x14ListWorkflowsRequest\"l\n\x17ScheduleWorkflowRequest\x12\x13\n\x0bworkflow_id\x18\x01 \x01(\t\x12-\n\tschedules\x18\x02 \x03(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05input\x18\x03 \x01(\t\"5\n\x15ListWorkflowsResponse\x12\x1c\n\tworkflows\x18\x01 \x03(\x0b\x32\t.Workflow\"1\n\x1cListWorkflowsForEventRequest\x12\x11\n\tevent_key\x18\x01 \x01(\t\"\xee\x01\n\x08Workflow\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nupdated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\ttenant_id\x18\x05 \x01(\t\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\x31\n\x0b\x64\x65scription\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\"\n\x08versions\x18\x08 \x03(\x0b\x32\x10.WorkflowVersion\"\xeb\x01\n\x0fWorkflowVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nupdated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05order\x18\x06 \x01(\x05\x12\x13\n\x0bworkflow_id\x18\x07 \x01(\t\x12#\n\x08triggers\x18\x08 \x01(\x0b\x32\x11.WorkflowTriggers\x12\x12\n\x04jobs\x18\t \x03(\x0b\x32\x04.Job\"\x80\x02\n\x10WorkflowTriggers\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nupdated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x13workflow_version_id\x18\x05 \x01(\t\x12\x11\n\ttenant_id\x18\x06 \x01(\t\x12(\n\x06\x65vents\x18\x07 \x03(\x0b\x32\x18.WorkflowTriggerEventRef\x12&\n\x05\x63rons\x18\x08 \x03(\x0b\x32\x17.WorkflowTriggerCronRef\"?\n\x17WorkflowTriggerEventRef\x12\x11\n\tparent_id\x18\x01 \x01(\t\x12\x11\n\tevent_key\x18\x02 \x01(\t\"9\n\x16WorkflowTriggerCronRef\x12\x11\n\tparent_id\x18\x01 \x01(\t\x12\x0c\n\x04\x63ron\x18\x02 \x01(\t\"\xa7\x02\n\x03Job\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nupdated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\ttenant_id\x18\x05 \x01(\t\x12\x1b\n\x13workflow_version_id\x18\x06 \x01(\t\x12\x0c\n\x04name\x18\x07 \x01(\t\x12\x31\n\x0b\x64\x65scription\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x14\n\x05steps\x18\t \x03(\x0b\x32\x05.Step\x12-\n\x07timeout\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xaa\x02\n\x04Step\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nupdated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\x0breadable_id\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x11\n\ttenant_id\x18\x06 \x01(\t\x12\x0e\n\x06job_id\x18\x07 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x08 \x01(\t\x12-\n\x07timeout\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x0f\n\x07parents\x18\n \x03(\t\x12\x10\n\x08\x63hildren\x18\x0b \x03(\t\",\n\x15\x44\x65leteWorkflowRequest\x12\x13\n\x0bworkflow_id\x18\x01 \x01(\t\"(\n\x18GetWorkflowByNameRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"5\n\x16TriggerWorkflowRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05input\x18\x02 \x01(\t\"2\n\x17TriggerWorkflowResponse\x12\x17\n\x0fworkflow_run_id\x18\x01 \x01(\t*U\n\x18\x43oncurrencyLimitStrategy\x12\x16\n\x12\x43\x41NCEL_IN_PROGRESS\x10\x00\x12\x0f\n\x0b\x44ROP_NEWEST\x10\x01\x12\x10\n\x0cQUEUE_NEWEST\x10\x02\x32\xcd\x03\n\x0fWorkflowService\x12>\n\rListWorkflows\x12\x15.ListWorkflowsRequest\x1a\x16.ListWorkflowsResponse\x12\x34\n\x0bPutWorkflow\x12\x13.PutWorkflowRequest\x1a\x10.WorkflowVersion\x12>\n\x10ScheduleWorkflow\x12\x18.ScheduleWorkflowRequest\x1a\x10.WorkflowVersion\x12\x44\n\x0fTriggerWorkflow\x12\x17.TriggerWorkflowRequest\x1a\x18.TriggerWorkflowResponse\x12\x39\n\x11GetWorkflowByName\x12\x19.GetWorkflowByNameRequest\x1a\t.Workflow\x12N\n\x15ListWorkflowsForEvent\x12\x1d.ListWorkflowsForEventRequest\x1a\x16.ListWorkflowsResponse\x12\x33\n\x0e\x44\x65leteWorkflow\x12\x16.DeleteWorkflowRequest\x1a\t.WorkflowBBZ@github.com/hatchet-dev/hatchet/internal/services/admin/contractsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0fworkflows.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x1egoogle/protobuf/wrappers.proto\">\n\x12PutWorkflowRequest\x12(\n\x04opts\x18\x01 \x01(\x0b\x32\x1a.CreateWorkflowVersionOpts\"\x8b\x02\n\x19\x43reateWorkflowVersionOpts\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0f\n\x07version\x18\x03 \x01(\t\x12\x16\n\x0e\x65vent_triggers\x18\x04 \x03(\t\x12\x15\n\rcron_triggers\x18\x05 \x03(\t\x12\x36\n\x12scheduled_triggers\x18\x06 \x03(\x0b\x32\x1a.google.protobuf.Timestamp\x12$\n\x04jobs\x18\x07 \x03(\x0b\x32\x16.CreateWorkflowJobOpts\x12-\n\x0b\x63oncurrency\x18\x08 \x01(\x0b\x32\x18.WorkflowConcurrencyOpts\"n\n\x17WorkflowConcurrencyOpts\x12\x0e\n\x06\x61\x63tion\x18\x01 \x01(\t\x12\x10\n\x08max_runs\x18\x02 \x01(\x05\x12\x31\n\x0elimit_strategy\x18\x03 \x01(\x0e\x32\x19.ConcurrencyLimitStrategy\"s\n\x15\x43reateWorkflowJobOpts\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\x13\n\x0b\x64\x65scription\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\t\x12&\n\x05steps\x18\x04 \x03(\x0b\x32\x17.CreateWorkflowStepOpts\"\x82\x01\n\x16\x43reateWorkflowStepOpts\x12\x13\n\x0breadable_id\x18\x01 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x02 \x01(\t\x12\x0f\n\x07timeout\x18\x03 \x01(\t\x12\x0e\n\x06inputs\x18\x04 \x01(\t\x12\x0f\n\x07parents\x18\x05 \x03(\t\x12\x11\n\tuser_data\x18\x06 \x01(\t\"\x16\n\x14ListWorkflowsRequest\"l\n\x17ScheduleWorkflowRequest\x12\x13\n\x0bworkflow_id\x18\x01 \x01(\t\x12-\n\tschedules\x18\x02 \x03(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05input\x18\x03 \x01(\t\"5\n\x15ListWorkflowsResponse\x12\x1c\n\tworkflows\x18\x01 \x03(\x0b\x32\t.Workflow\"1\n\x1cListWorkflowsForEventRequest\x12\x11\n\tevent_key\x18\x01 \x01(\t\"\xee\x01\n\x08Workflow\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nupdated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\ttenant_id\x18\x05 \x01(\t\x12\x0c\n\x04name\x18\x06 \x01(\t\x12\x31\n\x0b\x64\x65scription\x18\x07 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\"\n\x08versions\x18\x08 \x03(\x0b\x32\x10.WorkflowVersion\"\xeb\x01\n\x0fWorkflowVersion\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nupdated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x0f\n\x07version\x18\x05 \x01(\t\x12\r\n\x05order\x18\x06 \x01(\x05\x12\x13\n\x0bworkflow_id\x18\x07 \x01(\t\x12#\n\x08triggers\x18\x08 \x01(\x0b\x32\x11.WorkflowTriggers\x12\x12\n\x04jobs\x18\t \x03(\x0b\x32\x04.Job\"\x80\x02\n\x10WorkflowTriggers\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nupdated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x1b\n\x13workflow_version_id\x18\x05 \x01(\t\x12\x11\n\ttenant_id\x18\x06 \x01(\t\x12(\n\x06\x65vents\x18\x07 \x03(\x0b\x32\x18.WorkflowTriggerEventRef\x12&\n\x05\x63rons\x18\x08 \x03(\x0b\x32\x17.WorkflowTriggerCronRef\"?\n\x17WorkflowTriggerEventRef\x12\x11\n\tparent_id\x18\x01 \x01(\t\x12\x11\n\tevent_key\x18\x02 \x01(\t\"9\n\x16WorkflowTriggerCronRef\x12\x11\n\tparent_id\x18\x01 \x01(\t\x12\x0c\n\x04\x63ron\x18\x02 \x01(\t\"\xa7\x02\n\x03Job\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nupdated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x11\n\ttenant_id\x18\x05 \x01(\t\x12\x1b\n\x13workflow_version_id\x18\x06 \x01(\t\x12\x0c\n\x04name\x18\x07 \x01(\t\x12\x31\n\x0b\x64\x65scription\x18\x08 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x14\n\x05steps\x18\t \x03(\x0b\x32\x05.Step\x12-\n\x07timeout\x18\n \x01(\x0b\x32\x1c.google.protobuf.StringValue\"\xaa\x02\n\x04Step\x12\n\n\x02id\x18\x01 \x01(\t\x12.\n\ncreated_at\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nupdated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\x0breadable_id\x18\x05 \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x11\n\ttenant_id\x18\x06 \x01(\t\x12\x0e\n\x06job_id\x18\x07 \x01(\t\x12\x0e\n\x06\x61\x63tion\x18\x08 \x01(\t\x12-\n\x07timeout\x18\t \x01(\x0b\x32\x1c.google.protobuf.StringValue\x12\x0f\n\x07parents\x18\n \x03(\t\x12\x10\n\x08\x63hildren\x18\x0b \x03(\t\",\n\x15\x44\x65leteWorkflowRequest\x12\x13\n\x0bworkflow_id\x18\x01 \x01(\t\"(\n\x18GetWorkflowByNameRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\"5\n\x16TriggerWorkflowRequest\x12\x0c\n\x04name\x18\x01 \x01(\t\x12\r\n\x05input\x18\x02 \x01(\t\"2\n\x17TriggerWorkflowResponse\x12\x17\n\x0fworkflow_run_id\x18\x01 \x01(\t*U\n\x18\x43oncurrencyLimitStrategy\x12\x16\n\x12\x43\x41NCEL_IN_PROGRESS\x10\x00\x12\x0f\n\x0b\x44ROP_NEWEST\x10\x01\x12\x10\n\x0cQUEUE_NEWEST\x10\x02\x32\xcd\x03\n\x0fWorkflowService\x12>\n\rListWorkflows\x12\x15.ListWorkflowsRequest\x1a\x16.ListWorkflowsResponse\x12\x34\n\x0bPutWorkflow\x12\x13.PutWorkflowRequest\x1a\x10.WorkflowVersion\x12>\n\x10ScheduleWorkflow\x12\x18.ScheduleWorkflowRequest\x1a\x10.WorkflowVersion\x12\x44\n\x0fTriggerWorkflow\x12\x17.TriggerWorkflowRequest\x1a\x18.TriggerWorkflowResponse\x12\x39\n\x11GetWorkflowByName\x12\x19.GetWorkflowByNameRequest\x1a\t.Workflow\x12N\n\x15ListWorkflowsForEvent\x12\x1d.ListWorkflowsForEventRequest\x1a\x16.ListWorkflowsResponse\x12\x33\n\x0e\x44\x65leteWorkflow\x12\x16.DeleteWorkflowRequest\x1a\t.WorkflowBBZ@github.com/hatchet-dev/hatchet/internal/services/admin/contractsb\x06proto3')
 
 _globals = globals()
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, _globals)
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'workflows_pb2', _globals)
 if _descriptor._USE_C_DESCRIPTORS == False:
   _globals['DESCRIPTOR']._options = None
   _globals['DESCRIPTOR']._serialized_options = b'Z@github.com/hatchet-dev/hatchet/internal/services/admin/contracts'
-  _globals['_CONCURRENCYLIMITSTRATEGY']._serialized_start=2656
-  _globals['_CONCURRENCYLIMITSTRATEGY']._serialized_end=2741
+  _globals['_CONCURRENCYLIMITSTRATEGY']._serialized_start=2676
+  _globals['_CONCURRENCYLIMITSTRATEGY']._serialized_end=2761
   _globals['_PUTWORKFLOWREQUEST']._serialized_start=84
   _globals['_PUTWORKFLOWREQUEST']._serialized_end=146
   _globals['_CREATEWORKFLOWVERSIONOPTS']._serialized_start=149
   _globals['_CREATEWORKFLOWVERSIONOPTS']._serialized_end=416
   _globals['_WORKFLOWCONCURRENCYOPTS']._serialized_start=418
   _globals['_WORKFLOWCONCURRENCYOPTS']._serialized_end=528
   _globals['_CREATEWORKFLOWJOBOPTS']._serialized_start=530
   _globals['_CREATEWORKFLOWJOBOPTS']._serialized_end=645
-  _globals['_CREATEWORKFLOWSTEPOPTS']._serialized_start=647
-  _globals['_CREATEWORKFLOWSTEPOPTS']._serialized_end=758
-  _globals['_LISTWORKFLOWSREQUEST']._serialized_start=760
-  _globals['_LISTWORKFLOWSREQUEST']._serialized_end=782
-  _globals['_SCHEDULEWORKFLOWREQUEST']._serialized_start=784
-  _globals['_SCHEDULEWORKFLOWREQUEST']._serialized_end=892
-  _globals['_LISTWORKFLOWSRESPONSE']._serialized_start=894
-  _globals['_LISTWORKFLOWSRESPONSE']._serialized_end=947
-  _globals['_LISTWORKFLOWSFOREVENTREQUEST']._serialized_start=949
-  _globals['_LISTWORKFLOWSFOREVENTREQUEST']._serialized_end=998
-  _globals['_WORKFLOW']._serialized_start=1001
-  _globals['_WORKFLOW']._serialized_end=1239
-  _globals['_WORKFLOWVERSION']._serialized_start=1242
-  _globals['_WORKFLOWVERSION']._serialized_end=1477
-  _globals['_WORKFLOWTRIGGERS']._serialized_start=1480
-  _globals['_WORKFLOWTRIGGERS']._serialized_end=1736
-  _globals['_WORKFLOWTRIGGEREVENTREF']._serialized_start=1738
-  _globals['_WORKFLOWTRIGGEREVENTREF']._serialized_end=1801
-  _globals['_WORKFLOWTRIGGERCRONREF']._serialized_start=1803
-  _globals['_WORKFLOWTRIGGERCRONREF']._serialized_end=1860
-  _globals['_JOB']._serialized_start=1863
-  _globals['_JOB']._serialized_end=2158
-  _globals['_STEP']._serialized_start=2161
-  _globals['_STEP']._serialized_end=2459
-  _globals['_DELETEWORKFLOWREQUEST']._serialized_start=2461
-  _globals['_DELETEWORKFLOWREQUEST']._serialized_end=2505
-  _globals['_GETWORKFLOWBYNAMEREQUEST']._serialized_start=2507
-  _globals['_GETWORKFLOWBYNAMEREQUEST']._serialized_end=2547
-  _globals['_TRIGGERWORKFLOWREQUEST']._serialized_start=2549
-  _globals['_TRIGGERWORKFLOWREQUEST']._serialized_end=2602
-  _globals['_TRIGGERWORKFLOWRESPONSE']._serialized_start=2604
-  _globals['_TRIGGERWORKFLOWRESPONSE']._serialized_end=2654
-  _globals['_WORKFLOWSERVICE']._serialized_start=2744
-  _globals['_WORKFLOWSERVICE']._serialized_end=3205
+  _globals['_CREATEWORKFLOWSTEPOPTS']._serialized_start=648
+  _globals['_CREATEWORKFLOWSTEPOPTS']._serialized_end=778
+  _globals['_LISTWORKFLOWSREQUEST']._serialized_start=780
+  _globals['_LISTWORKFLOWSREQUEST']._serialized_end=802
+  _globals['_SCHEDULEWORKFLOWREQUEST']._serialized_start=804
+  _globals['_SCHEDULEWORKFLOWREQUEST']._serialized_end=912
+  _globals['_LISTWORKFLOWSRESPONSE']._serialized_start=914
+  _globals['_LISTWORKFLOWSRESPONSE']._serialized_end=967
+  _globals['_LISTWORKFLOWSFOREVENTREQUEST']._serialized_start=969
+  _globals['_LISTWORKFLOWSFOREVENTREQUEST']._serialized_end=1018
+  _globals['_WORKFLOW']._serialized_start=1021
+  _globals['_WORKFLOW']._serialized_end=1259
+  _globals['_WORKFLOWVERSION']._serialized_start=1262
+  _globals['_WORKFLOWVERSION']._serialized_end=1497
+  _globals['_WORKFLOWTRIGGERS']._serialized_start=1500
+  _globals['_WORKFLOWTRIGGERS']._serialized_end=1756
+  _globals['_WORKFLOWTRIGGEREVENTREF']._serialized_start=1758
+  _globals['_WORKFLOWTRIGGEREVENTREF']._serialized_end=1821
+  _globals['_WORKFLOWTRIGGERCRONREF']._serialized_start=1823
+  _globals['_WORKFLOWTRIGGERCRONREF']._serialized_end=1880
+  _globals['_JOB']._serialized_start=1883
+  _globals['_JOB']._serialized_end=2178
+  _globals['_STEP']._serialized_start=2181
+  _globals['_STEP']._serialized_end=2479
+  _globals['_DELETEWORKFLOWREQUEST']._serialized_start=2481
+  _globals['_DELETEWORKFLOWREQUEST']._serialized_end=2525
+  _globals['_GETWORKFLOWBYNAMEREQUEST']._serialized_start=2527
+  _globals['_GETWORKFLOWBYNAMEREQUEST']._serialized_end=2567
+  _globals['_TRIGGERWORKFLOWREQUEST']._serialized_start=2569
+  _globals['_TRIGGERWORKFLOWREQUEST']._serialized_end=2622
+  _globals['_TRIGGERWORKFLOWRESPONSE']._serialized_start=2624
+  _globals['_TRIGGERWORKFLOWRESPONSE']._serialized_end=2674
+  _globals['_WORKFLOWSERVICE']._serialized_start=2764
+  _globals['_WORKFLOWSERVICE']._serialized_end=3225
 # @@protoc_insertion_point(module_scope)
```

### Comparing `hatchet_sdk-0.9.3/hatchet_sdk/workflows_pb2.pyi` & `hatchet_sdk-0.9.4/hatchet_sdk/workflows_pb2.pyi`

 * *Files 1% similar despite different names*

```diff
@@ -62,26 +62,28 @@
     name: str
     description: str
     timeout: str
     steps: _containers.RepeatedCompositeFieldContainer[CreateWorkflowStepOpts]
     def __init__(self, name: _Optional[str] = ..., description: _Optional[str] = ..., timeout: _Optional[str] = ..., steps: _Optional[_Iterable[_Union[CreateWorkflowStepOpts, _Mapping]]] = ...) -> None: ...
 
 class CreateWorkflowStepOpts(_message.Message):
-    __slots__ = ("readable_id", "action", "timeout", "inputs", "parents")
+    __slots__ = ("readable_id", "action", "timeout", "inputs", "parents", "user_data")
     READABLE_ID_FIELD_NUMBER: _ClassVar[int]
     ACTION_FIELD_NUMBER: _ClassVar[int]
     TIMEOUT_FIELD_NUMBER: _ClassVar[int]
     INPUTS_FIELD_NUMBER: _ClassVar[int]
     PARENTS_FIELD_NUMBER: _ClassVar[int]
+    USER_DATA_FIELD_NUMBER: _ClassVar[int]
     readable_id: str
     action: str
     timeout: str
     inputs: str
     parents: _containers.RepeatedScalarFieldContainer[str]
-    def __init__(self, readable_id: _Optional[str] = ..., action: _Optional[str] = ..., timeout: _Optional[str] = ..., inputs: _Optional[str] = ..., parents: _Optional[_Iterable[str]] = ...) -> None: ...
+    user_data: str
+    def __init__(self, readable_id: _Optional[str] = ..., action: _Optional[str] = ..., timeout: _Optional[str] = ..., inputs: _Optional[str] = ..., parents: _Optional[_Iterable[str]] = ..., user_data: _Optional[str] = ...) -> None: ...
 
 class ListWorkflowsRequest(_message.Message):
     __slots__ = ()
     def __init__(self) -> None: ...
 
 class ScheduleWorkflowRequest(_message.Message):
     __slots__ = ("workflow_id", "schedules", "input")
```

### Comparing `hatchet_sdk-0.9.3/hatchet_sdk/workflows_pb2_grpc.py` & `hatchet_sdk-0.9.4/hatchet_sdk/workflows_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `hatchet_sdk-0.9.3/PKG-INFO` & `hatchet_sdk-0.9.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hatchet-sdk
-Version: 0.9.3
+Version: 0.9.4
 Summary: 
 Author: Alexander Belanger
 Author-email: alexander@hatchet.run
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

