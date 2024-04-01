# Comparing `tmp/testcontainers-4.2.0rc2.tar.gz` & `tmp/testcontainers-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testcontainers-4.2.0rc2.tar", max compression
+gzip compressed data, was "testcontainers-4.3.0.tar", max compression
```

## Comparing `testcontainers-4.2.0rc2.tar` & `testcontainers-4.3.0.tar`

### file list

```diff
@@ -1,40 +1,48 @@
--rw-r--r--   0        0        0    11328 2024-03-24 02:15:30.163467 testcontainers-4.2.0rc2/LICENSE.txt
--rw-r--r--   0        0        0     1655 2024-03-24 02:22:15.776216 testcontainers-4.2.0rc2/README.md
--rw-r--r--   0        0        0      172 2024-03-24 02:22:15.776216 testcontainers-4.2.0rc2/core/testcontainers/compose/__init__.py
--rw-r--r--   0        0        0    13022 2024-03-24 02:22:15.776216 testcontainers-4.2.0rc2/core/testcontainers/compose/compose.py
--rw-r--r--   0        0        0        0 2024-03-24 02:15:30.163467 testcontainers-4.2.0rc2/core/testcontainers/core/__init__.py
--rw-r--r--   0        0        0      524 2024-03-24 02:22:15.776216 testcontainers-4.2.0rc2/core/testcontainers/core/config.py
--rw-r--r--   0        0        0     7857 2024-03-24 02:22:15.780216 testcontainers-4.2.0rc2/core/testcontainers/core/container.py
--rw-r--r--   0        0        0     7128 2024-03-24 02:22:15.780216 testcontainers-4.2.0rc2/core/testcontainers/core/docker_client.py
--rw-r--r--   0        0        0      734 2024-03-24 02:22:15.780216 testcontainers-4.2.0rc2/core/testcontainers/core/exceptions.py
--rw-r--r--   0        0        0     2418 2024-03-24 02:22:15.780216 testcontainers-4.2.0rc2/core/testcontainers/core/generic.py
--rw-r--r--   0        0        0      498 2024-03-24 02:22:15.780216 testcontainers-4.2.0rc2/core/testcontainers/core/labels.py
--rw-r--r--   0        0        0     2088 2024-03-24 02:15:30.163467 testcontainers-4.2.0rc2/core/testcontainers/core/utils.py
--rw-r--r--   0        0        0     4059 2024-03-24 02:15:30.163467 testcontainers-4.2.0rc2/core/testcontainers/core/waiting_utils.py
--rw-r--r--   0        0        0     3760 2024-03-24 02:22:15.780216 testcontainers-4.2.0rc2/modules/arangodb/testcontainers/arangodb/__init__.py
--rw-r--r--   0        0        0     4385 2024-03-24 02:15:30.163467 testcontainers-4.2.0rc2/modules/azurite/testcontainers/azurite/__init__.py
--rw-r--r--   0        0        0     3030 2024-03-24 02:22:15.780216 testcontainers-4.2.0rc2/modules/clickhouse/testcontainers/clickhouse/__init__.py
--rw-r--r--   0        0        0     3886 2024-03-24 02:15:30.163467 testcontainers-4.2.0rc2/modules/elasticsearch/testcontainers/elasticsearch/__init__.py
--rw-r--r--   0        0        0       50 2024-03-24 02:15:30.163467 testcontainers-4.2.0rc2/modules/google/testcontainers/google/__init__.py
--rw-r--r--   0        0        0     2558 2024-03-24 02:15:30.163467 testcontainers-4.2.0rc2/modules/google/testcontainers/google/pubsub.py
--rw-r--r--   0        0        0     3759 2024-03-24 02:22:15.780216 testcontainers-4.2.0rc2/modules/influxdb/testcontainers/influxdb.py
--rw-r--r--   0        0        0     2387 2024-03-24 02:22:15.780216 testcontainers-4.2.0rc2/modules/influxdb/testcontainers/influxdb1/__init__.py
--rw-r--r--   0        0        0     4464 2024-03-24 02:22:15.780216 testcontainers-4.2.0rc2/modules/influxdb/testcontainers/influxdb2/__init__.py
--rw-r--r--   0        0        0     2662 2024-03-24 02:15:30.163467 testcontainers-4.2.0rc2/modules/k3s/testcontainers/k3s/__init__.py
--rw-r--r--   0        0        0     3917 2024-03-24 02:15:30.163467 testcontainers-4.2.0rc2/modules/kafka/testcontainers/kafka/__init__.py
--rw-r--r--   0        0        0     2633 2024-03-24 02:22:15.780216 testcontainers-4.2.0rc2/modules/keycloak/testcontainers/keycloak/__init__.py
--rw-r--r--   0        0        0     3222 2024-03-24 02:15:30.163467 testcontainers-4.2.0rc2/modules/localstack/testcontainers/localstack/__init__.py
--rw-r--r--   0        0        0     4116 2024-03-24 02:15:30.163467 testcontainers-4.2.0rc2/modules/minio/testcontainers/minio/__init__.py
--rw-r--r--   0        0        0     3260 2024-03-24 02:22:15.780216 testcontainers-4.2.0rc2/modules/mongodb/testcontainers/mongodb/__init__.py
--rw-r--r--   0        0        0     1808 2024-03-24 02:15:30.167467 testcontainers-4.2.0rc2/modules/mssql/testcontainers/mssql/__init__.py
--rw-r--r--   0        0        0     3261 2024-03-24 02:15:30.167467 testcontainers-4.2.0rc2/modules/mysql/testcontainers/mysql/__init__.py
--rw-r--r--   0        0        0     2761 2024-03-24 02:15:30.167467 testcontainers-4.2.0rc2/modules/neo4j/testcontainers/neo4j/__init__.py
--rw-r--r--   0        0        0     1596 2024-03-24 02:15:30.167467 testcontainers-4.2.0rc2/modules/nginx/testcontainers/nginx/__init__.py
--rw-r--r--   0        0        0     4108 2024-03-24 02:15:30.167467 testcontainers-4.2.0rc2/modules/opensearch/testcontainers/opensearch/__init__.py
--rw-r--r--   0        0        0     1103 2024-03-24 02:15:30.167467 testcontainers-4.2.0rc2/modules/oracle/testcontainers/oracle/__init__.py
--rw-r--r--   0        0        0     4027 2024-03-24 02:22:15.780216 testcontainers-4.2.0rc2/modules/postgres/testcontainers/postgres/__init__.py
--rw-r--r--   0        0        0     2966 2024-03-24 02:22:15.780216 testcontainers-4.2.0rc2/modules/rabbitmq/testcontainers/rabbitmq/__init__.py
--rw-r--r--   0        0        0     3144 2024-03-24 02:22:15.780216 testcontainers-4.2.0rc2/modules/redis/testcontainers/redis/__init__.py
--rw-r--r--   0        0        0     2722 2024-03-24 02:15:30.167467 testcontainers-4.2.0rc2/modules/selenium/testcontainers/selenium/__init__.py
--rw-r--r--   0        0        0     7621 2024-03-24 03:03:24.678870 testcontainers-4.2.0rc2/pyproject.toml
--rw-r--r--   0        0        0     4595 1970-01-01 00:00:00.000000 testcontainers-4.2.0rc2/PKG-INFO
+-rw-r--r--   0        0        0    11328 2024-04-01 11:51:45.518006 testcontainers-4.3.0/LICENSE.txt
+-rw-r--r--   0        0        0     2042 2024-04-01 11:51:45.518006 testcontainers-4.3.0/README.md
+-rw-r--r--   0        0        0      172 2024-04-01 11:51:45.518006 testcontainers-4.3.0/core/testcontainers/compose/__init__.py
+-rw-r--r--   0        0        0    13096 2024-04-01 11:51:45.518006 testcontainers-4.3.0/core/testcontainers/compose/compose.py
+-rw-r--r--   0        0        0        0 2024-04-01 11:51:45.518006 testcontainers-4.3.0/core/testcontainers/core/__init__.py
+-rw-r--r--   0        0        0      605 2024-04-01 11:51:45.518006 testcontainers-4.3.0/core/testcontainers/core/config.py
+-rw-r--r--   0        0        0     7687 2024-04-01 11:51:45.518006 testcontainers-4.3.0/core/testcontainers/core/container.py
+-rw-r--r--   0        0        0     7262 2024-04-01 11:51:45.518006 testcontainers-4.3.0/core/testcontainers/core/docker_client.py
+-rw-r--r--   0        0        0      734 2024-04-01 11:51:45.518006 testcontainers-4.3.0/core/testcontainers/core/exceptions.py
+-rw-r--r--   0        0        0     2418 2024-04-01 11:51:45.518006 testcontainers-4.3.0/core/testcontainers/core/generic.py
+-rw-r--r--   0        0        0      498 2024-04-01 11:51:45.518006 testcontainers-4.3.0/core/testcontainers/core/labels.py
+-rw-r--r--   0        0        0     2088 2024-04-01 11:51:45.518006 testcontainers-4.3.0/core/testcontainers/core/utils.py
+-rw-r--r--   0        0        0     4059 2024-04-01 11:51:45.518006 testcontainers-4.3.0/core/testcontainers/core/waiting_utils.py
+-rw-r--r--   0        0        0     3760 2024-04-01 11:51:45.518006 testcontainers-4.3.0/modules/arangodb/testcontainers/arangodb/__init__.py
+-rw-r--r--   0        0        0     4385 2024-04-01 11:51:45.518006 testcontainers-4.3.0/modules/azurite/testcontainers/azurite/__init__.py
+-rw-r--r--   0        0        0     2492 2024-04-01 11:51:45.518006 testcontainers-4.3.0/modules/cassandra/testcontainers/cassandra/__init__.py
+-rw-r--r--   0        0        0     2736 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/chroma/testcontainers/chroma/__init__.py
+-rw-r--r--   0        0        0     3030 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/clickhouse/testcontainers/clickhouse/__init__.py
+-rw-r--r--   0        0        0     3886 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/elasticsearch/testcontainers/elasticsearch/__init__.py
+-rw-r--r--   0        0        0      106 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/google/testcontainers/google/__init__.py
+-rw-r--r--   0        0        0     2709 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/google/testcontainers/google/datastore.py
+-rw-r--r--   0        0        0     2952 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/google/testcontainers/google/pubsub.py
+-rw-r--r--   0        0        0     3759 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/influxdb/testcontainers/influxdb.py
+-rw-r--r--   0        0        0     2387 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/influxdb/testcontainers/influxdb1/__init__.py
+-rw-r--r--   0        0        0     4464 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/influxdb/testcontainers/influxdb2/__init__.py
+-rw-r--r--   0        0        0     2662 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/k3s/testcontainers/k3s/__init__.py
+-rw-r--r--   0        0        0     3592 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/kafka/testcontainers/kafka/__init__.py
+-rw-r--r--   0        0        0     2727 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/kafka/testcontainers/kafka/_redpanda.py
+-rw-r--r--   0        0        0     3313 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/keycloak/testcontainers/keycloak/__init__.py
+-rw-r--r--   0        0        0     3222 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/localstack/testcontainers/localstack/__init__.py
+-rw-r--r--   0        0        0     4116 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/minio/testcontainers/minio/__init__.py
+-rw-r--r--   0        0        0     3260 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/mongodb/testcontainers/mongodb/__init__.py
+-rw-r--r--   0        0        0     1808 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/mssql/testcontainers/mssql/__init__.py
+-rw-r--r--   0        0        0     3261 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/mysql/testcontainers/mysql/__init__.py
+-rw-r--r--   0        0        0     2811 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/nats/testcontainers/nats/__init__.py
+-rw-r--r--   0        0        0     2761 2024-04-01 11:51:45.522006 testcontainers-4.3.0/modules/neo4j/testcontainers/neo4j/__init__.py
+-rw-r--r--   0        0        0     1596 2024-04-01 11:51:45.526006 testcontainers-4.3.0/modules/nginx/testcontainers/nginx/__init__.py
+-rw-r--r--   0        0        0     4108 2024-04-01 11:51:45.526006 testcontainers-4.3.0/modules/opensearch/testcontainers/opensearch/__init__.py
+-rw-r--r--   0        0        0     2809 2024-04-01 11:51:45.526006 testcontainers-4.3.0/modules/oracle-free/testcontainers/oracle/__init__.py
+-rw-r--r--   0        0        0     3971 2024-04-01 11:51:45.526006 testcontainers-4.3.0/modules/postgres/testcontainers/postgres/__init__.py
+-rw-r--r--   0        0        0     5188 2024-04-01 11:51:45.526006 testcontainers-4.3.0/modules/qdrant/testcontainers/qdrant/__init__.py
+-rw-r--r--   0        0        0     2966 2024-04-01 11:51:45.526006 testcontainers-4.3.0/modules/rabbitmq/testcontainers/rabbitmq/__init__.py
+-rw-r--r--   0        0        0     3144 2024-04-01 11:51:45.526006 testcontainers-4.3.0/modules/redis/testcontainers/redis/__init__.py
+-rw-r--r--   0        0        0     2761 2024-04-01 11:51:45.526006 testcontainers-4.3.0/modules/registry/testcontainers/registry/__init__.py
+-rw-r--r--   0        0        0     2722 2024-04-01 11:51:45.526006 testcontainers-4.3.0/modules/selenium/testcontainers/selenium/__init__.py
+-rw-r--r--   0        0        0     5588 2024-04-01 11:51:45.526006 testcontainers-4.3.0/modules/weaviate/testcontainers/weaviate/__init__.py
+-rw-r--r--   0        0        0     8628 2024-04-01 11:51:45.526006 testcontainers-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0     5473 1970-01-01 00:00:00.000000 testcontainers-4.3.0/PKG-INFO
```

### Comparing `testcontainers-4.2.0rc2/LICENSE.txt` & `testcontainers-4.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `testcontainers-4.2.0rc2/README.md` & `testcontainers-4.3.0/README.md`

 * *Files 9% similar despite different names*

```diff
@@ -21,13 +21,14 @@
 'PostgreSQL 16...'
 ```
 
 The snippet above will spin up a postgres database in a container. The `get_connection_url()` convenience method returns a `sqlalchemy` compatible url we use to connect to the database and retrieve the database version.
 
 ## Configuration
 
-| Env Variable                              | Example                       | Description                              |
-| ----------------------------------------- | ----------------------------- | ---------------------------------------- |
-| `TESTCONTAINERS_DOCKER_SOCKET_OVERRIDE`   | `/var/run/docker.sock`        | Path to Docker's socket used by ryuk     |
-| `TESTCONTAINERS_RYUK_PRIVILEGED`          | `false`                       | Run ryuk as a privileged container       |
-| `TESTCONTAINERS_RYUK_DISABLED`            | `false`                       | Disable ryuk                             |
-| `RYUK_CONTAINER_IMAGE`                    | `testcontainers/ryuk:0.5.1`   | Custom image for ryuk                    |
+| Env Variable                            | Example                     | Description                                                                        |
+| --------------------------------------- | --------------------------- | ---------------------------------------------------------------------------------- |
+| `TESTCONTAINERS_DOCKER_SOCKET_OVERRIDE` | `/var/run/docker.sock`      | Path to Docker's socket used by ryuk                                               |
+| `TESTCONTAINERS_RYUK_PRIVILEGED`        | `false`                     | Run ryuk as a privileged container                                                 |
+| `TESTCONTAINERS_RYUK_DISABLED`          | `false`                     | Disable ryuk                                                                       |
+| `RYUK_CONTAINER_IMAGE`                  | `testcontainers/ryuk:0.7.0` | Custom image for ryuk                                                              |
+| `RYUK_RECONNECTION_TIMEOUT`             | `10s`                       | Reconnection timeout for Ryuk TCP socket before Ryuk reaps all dangling containers |
```

### Comparing `testcontainers-4.2.0rc2/core/testcontainers/compose/compose.py` & `testcontainers-4.3.0/core/testcontainers/compose/compose.py`

 * *Files 1% similar despite different names*

```diff
@@ -154,14 +154,15 @@
     context: Union[str, PathLike]
     compose_file_name: Optional[Union[str, list[str]]] = None
     pull: bool = False
     build: bool = False
     wait: bool = True
     env_file: Optional[str] = None
     services: Optional[list[str]] = None
+    docker_command_path: Optional[str] = None
 
     def __post_init__(self):
         if isinstance(self.compose_file_name, str):
             self.compose_file_name = [self.compose_file_name]
 
     def __enter__(self) -> "DockerCompose":
         self.start()
@@ -177,15 +178,15 @@
         Returns:
             cmd: Docker compose command parts.
         """
         return self.compose_command_property
 
     @cached_property
     def compose_command_property(self) -> list[str]:
-        docker_compose_cmd = ["docker", "compose"]
+        docker_compose_cmd = [self.docker_command_path or "docker", "compose"]
         if self.compose_file_name:
             for file in self.compose_file_name:
                 docker_compose_cmd += ["-f", file]
         if self.env_file:
             docker_compose_cmd += ["--env-file", self.env_file]
         return docker_compose_cmd
```

### Comparing `testcontainers-4.2.0rc2/core/testcontainers/core/container.py` & `testcontainers-4.3.0/core/testcontainers/core/container.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,21 @@
-from atexit import register
-from contextlib import suppress
+import contextlib
 from platform import system
-from signal import SIGINT, SIGTERM, signal
 from socket import socket
 from typing import TYPE_CHECKING, Optional
 
-from docker.errors import NotFound
+import docker.errors
 
-from testcontainers.core.config import RYUK_DISABLED, RYUK_DOCKER_SOCKET, RYUK_IMAGE, RYUK_PRIVILEGED
+from testcontainers.core.config import (
+    RYUK_DISABLED,
+    RYUK_DOCKER_SOCKET,
+    RYUK_IMAGE,
+    RYUK_PRIVILEGED,
+    RYUK_RECONNECTION_TIMEOUT,
+)
 from testcontainers.core.docker_client import DockerClient
 from testcontainers.core.exceptions import ContainerStartException
 from testcontainers.core.labels import LABEL_SESSION_ID, SESSION_ID
 from testcontainers.core.utils import inside_container, is_arm, setup_logger
 from testcontainers.core.waiting_utils import wait_container_is_ready, wait_for_logs
 
 if TYPE_CHECKING:
@@ -40,15 +44,15 @@
         **kwargs,
     ) -> None:
         self.env = {}
         self.ports = {}
         self.volumes = {}
         self.image = image
         self._docker = DockerClient(**(docker_client_kw or {}))
-        self._container: Optional[Container] = None
+        self._container = None
         self._command = None
         self._name = None
         self._kwargs = kwargs
 
     def with_env(self, key: str, value: str) -> "DockerContainer":
         self.env[key] = value
         return self
@@ -149,15 +153,15 @@
 
     def get_wrapped_container(self) -> "Container":
         return self._container
 
     def get_docker_client(self) -> DockerClient:
         return self._docker
 
-    def get_logs(self) -> tuple[str, str]:
+    def get_logs(self) -> tuple[bytes, bytes]:
         if not self._container:
             raise ContainerStartException("Container should be started before getting logs")
         return self._container.logs(stderr=False), self._container.logs(stdout=False)
 
     def exec(self, command) -> tuple[int, str]:
         if not self._container:
             raise ContainerStartException("Container should be started before executing a command")
@@ -178,18 +182,17 @@
 
     @classmethod
     def delete_instance(cls) -> None:
         if Reaper._socket is not None:
             Reaper._socket.close()
             Reaper._socket = None
 
-        if Reaper._container is not None:
-            if Reaper._container._container is not None:
-                with suppress(NotFound):
-                    Reaper._container._container.stop()
+        if Reaper._container is not None and Reaper._container._container is not None:
+            with contextlib.suppress(docker.errors.NotFound):
+                Reaper._container.stop()
             Reaper._container = None
 
         if Reaper._instance is not None:
             Reaper._instance = None
 
     @classmethod
     def _create_instance(cls) -> "Reaper":
@@ -197,19 +200,17 @@
 
         Reaper._container = (
             DockerContainer(RYUK_IMAGE)
             .with_name(f"testcontainers-ryuk-{SESSION_ID}")
             .with_exposed_ports(8080)
             .with_volume_mapping(RYUK_DOCKER_SOCKET, "/var/run/docker.sock", "rw")
             .with_kwargs(privileged=RYUK_PRIVILEGED, auto_remove=True)
+            .with_env("RYUK_RECONNECTION_TIMEOUT", RYUK_RECONNECTION_TIMEOUT)
             .start()
         )
-        register(lambda: Reaper.delete_instance())
-        signal(SIGINT, lambda _, __: Reaper.delete_instance())
-        signal(SIGTERM, lambda _, __: Reaper.delete_instance())
         wait_for_logs(Reaper._container, r".* Started!")
 
         container_host = Reaper._container.get_container_host_ip()
         container_port = int(Reaper._container.get_exposed_port(8080))
 
         Reaper._socket = socket()
         Reaper._socket.connect((container_host, container_port))
```

### Comparing `testcontainers-4.2.0rc2/core/testcontainers/core/docker_client.py` & `testcontainers-4.3.0/core/testcontainers/core/docker_client.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 #
 #    Unless required by applicable law or agreed to in writing, software
 #    distributed under the License is distributed on an "AS IS" BASIS, WITHOUT
 #    WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied. See the
 #    License for the specific language governing permissions and limitations
 #    under the License.
 import functools as ft
+import importlib.metadata
 import ipaddress
 import os
 import urllib
 import urllib.parse
 from os.path import exists
 from pathlib import Path
 from typing import Optional, Union
@@ -40,14 +41,15 @@
 
         if docker_host:
             LOGGER.info(f"using host {docker_host}")
             self.client = docker.DockerClient(base_url=docker_host)
         else:
             self.client = docker.from_env(**kwargs)
         self.client.api.headers["x-tc-sid"] = SESSION_ID
+        self.client.api.headers["User-Agent"] = "tc-python/" + importlib.metadata.version("testcontainers")
 
     @ft.wraps(ContainerCollection.run)
     def run(
         self,
         image: str,
         command: Optional[Union[str, list[str]]] = None,
         environment: Optional[dict] = None,
```

### Comparing `testcontainers-4.2.0rc2/core/testcontainers/core/exceptions.py` & `testcontainers-4.3.0/core/testcontainers/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.2.0rc2/core/testcontainers/core/generic.py` & `testcontainers-4.3.0/core/testcontainers/core/generic.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.2.0rc2/core/testcontainers/core/utils.py` & `testcontainers-4.3.0/core/testcontainers/core/utils.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.2.0rc2/core/testcontainers/core/waiting_utils.py` & `testcontainers-4.3.0/core/testcontainers/core/waiting_utils.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.2.0rc2/modules/arangodb/testcontainers/arangodb/__init__.py` & `testcontainers-4.3.0/modules/arangodb/testcontainers/arangodb/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.2.0rc2/modules/azurite/testcontainers/azurite/__init__.py` & `testcontainers-4.3.0/modules/azurite/testcontainers/azurite/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.2.0rc2/modules/clickhouse/testcontainers/clickhouse/__init__.py` & `testcontainers-4.3.0/modules/clickhouse/testcontainers/clickhouse/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.2.0rc2/modules/elasticsearch/testcontainers/elasticsearch/__init__.py` & `testcontainers-4.3.0/modules/elasticsearch/testcontainers/elasticsearch/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.2.0rc2/modules/google/testcontainers/google/pubsub.py` & `testcontainers-4.3.0/modules/google/testcontainers/google/pubsub.py`

 * *Files 20% similar despite different names*

```diff
@@ -52,11 +52,19 @@
         return f"{self.get_container_host_ip()}:{self.get_exposed_port(self.port)}"
 
     def _get_client(self, cls: type, **kwargs) -> dict:
         with patch.dict(os.environ, PUBSUB_EMULATOR_HOST=self.get_pubsub_emulator_host()):
             return cls(**kwargs)
 
     def get_publisher_client(self, **kwargs) -> pubsub.PublisherClient:
+        from google.auth import credentials
+
+        kwargs["client_options"] = {"api_endpoint": self.get_pubsub_emulator_host()}
+        kwargs["credentials"] = credentials.AnonymousCredentials()
         return self._get_client(pubsub.PublisherClient, **kwargs)
 
     def get_subscriber_client(self, **kwargs) -> pubsub.SubscriberClient:
+        from google.auth import credentials
+
+        kwargs["client_options"] = {"api_endpoint": self.get_pubsub_emulator_host()}
+        kwargs["credentials"] = credentials.AnonymousCredentials()
         return self._get_client(pubsub.SubscriberClient, **kwargs)
```

### Comparing `testcontainers-4.2.0rc2/modules/influxdb/testcontainers/influxdb.py` & `testcontainers-4.3.0/modules/influxdb/testcontainers/influxdb.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.2.0rc2/modules/influxdb/testcontainers/influxdb1/__init__.py` & `testcontainers-4.3.0/modules/influxdb/testcontainers/influxdb1/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.2.0rc2/modules/influxdb/testcontainers/influxdb2/__init__.py` & `testcontainers-4.3.0/modules/influxdb/testcontainers/influxdb2/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.2.0rc2/modules/k3s/testcontainers/k3s/__init__.py` & `testcontainers-4.3.0/modules/k3s/testcontainers/k3s/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.2.0rc2/modules/kafka/testcontainers/kafka/__init__.py` & `testcontainers-4.3.0/modules/kafka/testcontainers/kafka/__init__.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 import tarfile
 import time
 from io import BytesIO
 from textwrap import dedent
 
-from kafka import KafkaConsumer
-from kafka.errors import KafkaError, NoBrokersAvailable, UnrecognizedBrokerVersion
 from testcontainers.core.container import DockerContainer
 from testcontainers.core.utils import raise_for_deprecated_parameter
-from testcontainers.core.waiting_utils import wait_container_is_ready
+from testcontainers.core.waiting_utils import wait_for_logs
+from testcontainers.kafka._redpanda import RedpandaContainer
+
+__all__ = [
+    "KafkaContainer",
+    "RedpandaContainer",
+]
 
 
 class KafkaContainer(DockerContainer):
     """
     Kafka container.
 
     Example:
@@ -43,21 +47,14 @@
         self.with_env("KAFKA_GROUP_INITIAL_REBALANCE_DELAY_MS", "0")
 
     def get_bootstrap_server(self) -> str:
         host = self.get_container_host_ip()
         port = self.get_exposed_port(self.port)
         return f"{host}:{port}"
 
-    @wait_container_is_ready(UnrecognizedBrokerVersion, NoBrokersAvailable, KafkaError, ValueError)
-    def _connect(self) -> None:
-        bootstrap_server = self.get_bootstrap_server()
-        consumer = KafkaConsumer(group_id="test", bootstrap_servers=[bootstrap_server])
-        if not consumer.bootstrap_connected():
-            raise KafkaError("Unable to connect with kafka container!")
-
     def tc_start(self) -> None:
         host = self.get_container_host_ip()
         port = self.get_exposed_port(self.port)
         listeners = f"PLAINTEXT://{host}:{port},BROKER://$(hostname -i):9092"
         data = (
             dedent(
                 f"""
@@ -74,21 +71,21 @@
                 """
             )
             .strip()
             .encode("utf-8")
         )
         self.create_file(data, KafkaContainer.TC_START_SCRIPT)
 
-    def start(self) -> "KafkaContainer":
+    def start(self, timeout=30) -> "KafkaContainer":
         script = KafkaContainer.TC_START_SCRIPT
         command = f'sh -c "while [ ! -f {script} ]; do sleep 0.1; done; sh {script}"'
         self.with_command(command)
         super().start()
         self.tc_start()
-        self._connect()
+        wait_for_logs(self, r".*\[KafkaServer id=\d+\] started.*", timeout=timeout)
         return self
 
     def create_file(self, content: bytes, path: str) -> None:
         with BytesIO() as archive, tarfile.TarFile(fileobj=archive, mode="w") as tar:
             tarinfo = tarfile.TarInfo(name=path)
             tarinfo.size = len(content)
             tarinfo.mtime = time.time()
```

### Comparing `testcontainers-4.2.0rc2/modules/keycloak/testcontainers/keycloak/__init__.py` & `testcontainers-4.3.0/modules/keycloak/testcontainers/keycloak/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -13,29 +13,32 @@
 import os
 from typing import Optional
 
 import requests
 
 from keycloak import KeycloakAdmin
 from testcontainers.core.container import DockerContainer
-from testcontainers.core.waiting_utils import wait_container_is_ready
+from testcontainers.core.waiting_utils import wait_container_is_ready, wait_for_logs
+
+_DEFAULT_DEV_COMMAND = "start-dev"
 
 
 class KeycloakContainer(DockerContainer):
     """
     Keycloak container.
 
     Example:
 
         .. doctest::
 
             >>> from testcontainers.keycloak import KeycloakContainer
 
-            >>> with KeycloakContainer() as kc:
-            ...    keycloak = kc.get_client()
+            >>> with KeycloakContainer(f"quay.io/keycloak/keycloak:24.0.1") as keycloak:
+            ...     keycloak.get_client().users_count()
+            1
     """
 
     def __init__(
         self,
         image="quay.io/keycloak/keycloak:latest",
         username: Optional[str] = None,
         password: Optional[str] = None,
@@ -46,30 +49,38 @@
         self.password = password or os.environ.get("KEYCLOAK_ADMIN_PASSWORD", "test")
         self.port = port
         self.with_exposed_ports(self.port)
 
     def _configure(self) -> None:
         self.with_env("KEYCLOAK_ADMIN", self.username)
         self.with_env("KEYCLOAK_ADMIN_PASSWORD", self.password)
-        self.with_command("start-dev")
+        # Enable health checks
+        # see: https://www.keycloak.org/server/health#_relevant_options
+        self.with_env("KC_HEALTH_ENABLED", "true")
+        # Starting Keycloak in development mode
+        # see: https://www.keycloak.org/server/configuration#_starting_keycloak_in_development_mode
+        self.with_command(_DEFAULT_DEV_COMMAND)
 
     def get_url(self) -> str:
         host = self.get_container_host_ip()
         port = self.get_exposed_port(self.port)
         return f"http://{host}:{port}"
 
     @wait_container_is_ready(requests.exceptions.ConnectionError, requests.exceptions.ReadTimeout)
-    def _connect(self) -> None:
-        response = requests.get(self.get_url(), timeout=1)
+    def _readiness_probe(self) -> None:
+        # Keycloak provides an REST API endpoints for health checks: https://www.keycloak.org/server/health
+        response = requests.get(f"{self.get_url()}/health/ready", timeout=1)
         response.raise_for_status()
+        if self._command == _DEFAULT_DEV_COMMAND:
+            wait_for_logs(self, "Added user .* to realm .*")
 
     def start(self) -> "KeycloakContainer":
         self._configure()
         super().start()
-        self._connect()
+        self._readiness_probe()
         return self
 
     def get_client(self, **kwargs) -> KeycloakAdmin:
         default_kwargs = {
             "server_url": self.get_url(),
             "username": self.username,
             "password": self.password,
```

### Comparing `testcontainers-4.2.0rc2/modules/localstack/testcontainers/localstack/__init__.py` & `testcontainers-4.3.0/modules/localstack/testcontainers/localstack/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.2.0rc2/modules/minio/testcontainers/minio/__init__.py` & `testcontainers-4.3.0/modules/minio/testcontainers/minio/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.2.0rc2/modules/mongodb/testcontainers/mongodb/__init__.py` & `testcontainers-4.3.0/modules/mongodb/testcontainers/mongodb/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.2.0rc2/modules/mssql/testcontainers/mssql/__init__.py` & `testcontainers-4.3.0/modules/mssql/testcontainers/mssql/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.2.0rc2/modules/mysql/testcontainers/mysql/__init__.py` & `testcontainers-4.3.0/modules/mysql/testcontainers/mysql/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.2.0rc2/modules/neo4j/testcontainers/neo4j/__init__.py` & `testcontainers-4.3.0/modules/neo4j/testcontainers/neo4j/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.2.0rc2/modules/nginx/testcontainers/nginx/__init__.py` & `testcontainers-4.3.0/modules/nginx/testcontainers/nginx/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.2.0rc2/modules/opensearch/testcontainers/opensearch/__init__.py` & `testcontainers-4.3.0/modules/opensearch/testcontainers/opensearch/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.2.0rc2/modules/postgres/testcontainers/postgres/__init__.py` & `testcontainers-4.3.0/modules/postgres/testcontainers/postgres/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -34,16 +34,15 @@
         driver.
 
         .. doctest::
 
             >>> from testcontainers.postgres import PostgresContainer
             >>> import sqlalchemy
 
-            >>> postgres_container = PostgresContainer("postgres:16")
-            >>> with postgres_container as postgres:
+            >>> with PostgresContainer("postgres:16") as postgres:
             ...     engine = sqlalchemy.create_engine(postgres.get_connection_url())
             ...     with engine.begin() as connection:
             ...         result = connection.execute(sqlalchemy.text("select version()"))
             ...         version, = result.fetchone()
             >>> version
             'PostgreSQL 16...'
     """
```

### Comparing `testcontainers-4.2.0rc2/modules/rabbitmq/testcontainers/rabbitmq/__init__.py` & `testcontainers-4.3.0/modules/rabbitmq/testcontainers/rabbitmq/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.2.0rc2/modules/redis/testcontainers/redis/__init__.py` & `testcontainers-4.3.0/modules/redis/testcontainers/redis/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.2.0rc2/modules/selenium/testcontainers/selenium/__init__.py` & `testcontainers-4.3.0/modules/selenium/testcontainers/selenium/__init__.py`

 * *Files identical despite different names*

### Comparing `testcontainers-4.2.0rc2/pyproject.toml` & `testcontainers-4.3.0/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 [tool.poetry]
 name = "testcontainers"
-version = "4.2.0rc2"  # auto-incremented by release-please
+version = "4.3.0"  # auto-incremented by release-please
 description = "Python library for throwaway instances of anything that can run in a Docker container"
 authors = ["Sergey Pirogov <automationremarks@gmail.com>"]
 maintainers = [
     "Balint Bartha <totallyzen@users.noreply.github.com>",
-    "David Ankin <daveankin@gmail.com>"
+    "David Ankin <daveankin@gmail.com>",
+    "Vemund Santi <vemund@santi.no>"
 ]
 readme = "README.md"
 keywords = ["testing", "logging", "docker", "test automation"]
 classifiers = [
     "License :: OSI Approved :: Apache Software License",
     "Intended Audience :: Information Technology",
     "Intended Audience :: Developers",
@@ -25,34 +26,40 @@
     "Operating System :: MacOS",
 ]
 # testcontainers-core is a proper package dependency - only modules needed here
 packages = [
     { include = "testcontainers", from = "core" },
     { include = "testcontainers", from = "modules/arangodb" },
     { include = "testcontainers", from = "modules/azurite" },
+    { include = "testcontainers", from = "modules/cassandra" },
+    { include = "testcontainers", from = "modules/chroma" },
     { include = "testcontainers", from = "modules/clickhouse" },
     { include = "testcontainers", from = "modules/elasticsearch" },
     { include = "testcontainers", from = "modules/google" },
     { include = "testcontainers", from = "modules/influxdb" },
     { include = "testcontainers", from = "modules/k3s" },
     { include = "testcontainers", from = "modules/kafka" },
     { include = "testcontainers", from = "modules/keycloak" },
     { include = "testcontainers", from = "modules/localstack" },
     { include = "testcontainers", from = "modules/minio" },
     { include = "testcontainers", from = "modules/mongodb" },
     { include = "testcontainers", from = "modules/mssql" },
     { include = "testcontainers", from = "modules/mysql" },
+    { include = "testcontainers", from = "modules/nats" },
     { include = "testcontainers", from = "modules/neo4j" },
     { include = "testcontainers", from = "modules/nginx" },
     { include = "testcontainers", from = "modules/opensearch" },
-    { include = "testcontainers", from = "modules/oracle" },
+    { include = "testcontainers", from = "modules/oracle-free" },
     { include = "testcontainers", from = "modules/postgres" },
+    { include = "testcontainers", from = "modules/qdrant" },
     { include = "testcontainers", from = "modules/rabbitmq" },
     { include = "testcontainers", from = "modules/redis" },
-    { include = "testcontainers", from = "modules/selenium" }
+    { include = "testcontainers", from = "modules/registry" },
+    { include = "testcontainers", from = "modules/selenium" },
+    { include = "testcontainers", from = "modules/weaviate" }
 ]
 
 [tool.poetry.urls]
 "GitHub" = "https://github.com/testcontainers/testcontainers-python"
 "Issue Tracker" = "https://github.com/testcontainers/testcontainers-python/issues"
 
 [tool.poetry.dependencies]
@@ -62,70 +69,85 @@
 wrapt = "*" # "^1.16.0"
 
 # community modules
 python-arango = { version = "^7.8", optional = true }
 azure-storage-blob = { version = "^12.19", optional = true }
 clickhouse-driver = { version = "*", optional = true }
 google-cloud-pubsub = { version = ">=2", optional = true }
+google-cloud-datastore = { version = ">=2", optional = true }
 influxdb = { version = "*", optional = true }
 influxdb-client = { version = "*", optional = true }
 kubernetes = { version = "*", optional = true }
 pyyaml = { version = "*", optional = true }
-kafka-python = { version = "*", optional = true }
 python-keycloak = { version = "*", optional = true }
 boto3 = { version = "*", optional = true }
 minio = { version = "*", optional = true }
+nats-py = { version = "*", optional = true }
 pymongo = { version = "*", optional = true }
 sqlalchemy = { version = "*", optional = true }
 pymssql = { version = "*", optional = true }
 pymysql = { version = "*", extras = ["rsa"], optional = true }
 neo4j = { version = "*", optional = true }
 opensearch-py = { version = "*", optional = true }
-cx_Oracle = { version = "*", optional = true }
+oracledb = { version = "*", optional = true }
 pika = { version = "*", optional = true }
 redis = { version = "*", optional = true }
 selenium = { version = "*", optional = true }
+weaviate-client = { version = "^4.5.4", optional = true }
+chromadb-client = { version = "*", optional = true }
+qdrant-client = { version = "*", optional = true }
+bcrypt = { version = "*", optional = true }
 
 [tool.poetry.extras]
 arangodb = ["python-arango"]
 azurite = ["azure-storage-blob"]
+cassandra = []
 clickhouse = ["clickhouse-driver"]
 elasticsearch = []
-google = ["google-cloud-pubsub"]
+google = ["google-cloud-pubsub", "google-cloud-datastore"]
 influxdb = ["influxdb", "influxdb-client"]
 k3s = ["kubernetes", "pyyaml"]
-kafka = ["kafka-python"]
+kafka = []
 keycloak = ["python-keycloak"]
 localstack = ["boto3"]
 minio = ["minio"]
 mongodb = ["pymongo"]
 mssql = ["sqlalchemy", "pymssql"]
 mysql = ["sqlalchemy", "pymysql"]
+nats = ["nats-py"]
 neo4j = ["neo4j"]
 nginx = []
 opensearch = ["opensearch-py"]
-oracle = ["sqlalchemy", "cx_Oracle"]
+oracle = ["sqlalchemy", "oracledb"]
+oracle-free = ["sqlalchemy", "oracledb"]
 postgres = []
+qdrant = ["qdrant-client"]
 rabbitmq = ["pika"]
 redis = ["redis"]
+registry = ["bcrypt"]
 selenium = ["selenium"]
+weaviate = ["weaviate-client"]
+chroma = ["chromadb-client"]
 
 [tool.poetry.group.dev.dependencies]
 mypy = "1.7.1"
 pre-commit = "^3.6"
 pytest = "7.4.3"
 pytest-cov = "4.1.0"
 sphinx = "^7.2.6"
 twine = "^4.0.2"
 anyio = "^4.3.0"
 # for tests only
 psycopg2-binary = "*"
 pg8000 = "*"
 sqlalchemy = "*"
-
+psycopg = "*"
+cassandra-driver = "*"
+pytest-asyncio = "0.23.5"
+kafka-python-ng = "^2.2.0"
 
 [[tool.poetry.source]]
 name = "PyPI"
 priority = "primary"
 
 [tool.black]
 line-length = 120
@@ -216,14 +238,15 @@
 strict = true
 fast_module_lookup = true
 modules = ["testcontainers.core"]
 mypy_path = [
     "core",
 #    "modules/arangodb",
 #    "modules/azurite",
+#    "modules/cassandra",
 #    "modules/clickhouse",
 #    "modules/elasticsearch",
 #    "modules/google",
 #    "modules/k3s",
 #    "modules/kafka",
 #    "modules/keycloak",
 #    "modules/localstack",
@@ -235,14 +258,15 @@
 #    "modules/nginx",
 #    "modules/opensearch",
 #    "modules/oracle",
 #    "modules/postgres",
 #    "modules/rabbitmq",
 #    "modules/redis",
 #    "modules/selenium"
+#    "modules/weaviate"
 ]
 enable_error_code = [
     "ignore-without-code",
     "redundant-expr",
     "truthy-bool",
 ]
```

### Comparing `testcontainers-4.2.0rc2/PKG-INFO` & `testcontainers-4.3.0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: testcontainers
-Version: 4.2.0rc2
+Version: 4.3.0
 Summary: Python library for throwaway instances of anything that can run in a Docker container
 Keywords: testing,logging,docker,test automation
 Author: Sergey Pirogov
 Author-email: automationremarks@gmail.com
 Maintainer: Balint Bartha
 Maintainer-email: totallyzen@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
@@ -19,58 +19,70 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Provides-Extra: arangodb
 Provides-Extra: azurite
+Provides-Extra: cassandra
+Provides-Extra: chroma
 Provides-Extra: clickhouse
 Provides-Extra: elasticsearch
 Provides-Extra: google
 Provides-Extra: influxdb
 Provides-Extra: k3s
 Provides-Extra: kafka
 Provides-Extra: keycloak
 Provides-Extra: localstack
 Provides-Extra: minio
 Provides-Extra: mongodb
 Provides-Extra: mssql
 Provides-Extra: mysql
+Provides-Extra: nats
 Provides-Extra: neo4j
 Provides-Extra: nginx
 Provides-Extra: opensearch
 Provides-Extra: oracle
+Provides-Extra: oracle-free
 Provides-Extra: postgres
+Provides-Extra: qdrant
 Provides-Extra: rabbitmq
 Provides-Extra: redis
+Provides-Extra: registry
 Provides-Extra: selenium
+Provides-Extra: weaviate
 Requires-Dist: azure-storage-blob (>=12.19,<13.0) ; extra == "azurite"
+Requires-Dist: bcrypt ; extra == "registry"
 Requires-Dist: boto3 ; extra == "localstack"
+Requires-Dist: chromadb-client ; extra == "chroma"
 Requires-Dist: clickhouse-driver ; extra == "clickhouse"
-Requires-Dist: cx_Oracle ; extra == "oracle"
 Requires-Dist: docker
+Requires-Dist: google-cloud-datastore (>=2) ; extra == "google"
 Requires-Dist: google-cloud-pubsub (>=2) ; extra == "google"
 Requires-Dist: influxdb ; extra == "influxdb"
 Requires-Dist: influxdb-client ; extra == "influxdb"
-Requires-Dist: kafka-python ; extra == "kafka"
 Requires-Dist: kubernetes ; extra == "k3s"
 Requires-Dist: minio ; extra == "minio"
+Requires-Dist: nats-py ; extra == "nats"
 Requires-Dist: neo4j ; extra == "neo4j"
 Requires-Dist: opensearch-py ; extra == "opensearch"
+Requires-Dist: oracledb ; extra == "oracle" or extra == "oracle-free"
 Requires-Dist: pika ; extra == "rabbitmq"
 Requires-Dist: pymongo ; extra == "mongodb"
 Requires-Dist: pymssql ; extra == "mssql"
 Requires-Dist: pymysql[rsa] ; extra == "mysql"
 Requires-Dist: python-arango (>=7.8,<8.0) ; extra == "arangodb"
 Requires-Dist: python-keycloak ; extra == "keycloak"
 Requires-Dist: pyyaml ; extra == "k3s"
+Requires-Dist: qdrant-client ; extra == "qdrant"
 Requires-Dist: redis ; extra == "redis"
 Requires-Dist: selenium ; extra == "selenium"
-Requires-Dist: sqlalchemy ; extra == "mssql" or extra == "mysql" or extra == "oracle"
+Requires-Dist: sqlalchemy ; extra == "mssql" or extra == "mysql" or extra == "oracle" or extra == "oracle-free"
 Requires-Dist: urllib3
+Requires-Dist: weaviate-client (>=4.5.4,<5.0.0) ; extra == "weaviate"
 Requires-Dist: wrapt
 Project-URL: GitHub, https://github.com/testcontainers/testcontainers-python
 Project-URL: Issue Tracker, https://github.com/testcontainers/testcontainers-python/issues
 Description-Content-Type: text/markdown
 
 # Testcontainers Python
 
@@ -95,14 +107,15 @@
 'PostgreSQL 16...'
 ```
 
 The snippet above will spin up a postgres database in a container. The `get_connection_url()` convenience method returns a `sqlalchemy` compatible url we use to connect to the database and retrieve the database version.
 
 ## Configuration
 
-| Env Variable                              | Example                       | Description                              |
-| ----------------------------------------- | ----------------------------- | ---------------------------------------- |
-| `TESTCONTAINERS_DOCKER_SOCKET_OVERRIDE`   | `/var/run/docker.sock`        | Path to Docker's socket used by ryuk     |
-| `TESTCONTAINERS_RYUK_PRIVILEGED`          | `false`                       | Run ryuk as a privileged container       |
-| `TESTCONTAINERS_RYUK_DISABLED`            | `false`                       | Disable ryuk                             |
-| `RYUK_CONTAINER_IMAGE`                    | `testcontainers/ryuk:0.5.1`   | Custom image for ryuk                    |
+| Env Variable                            | Example                     | Description                                                                        |
+| --------------------------------------- | --------------------------- | ---------------------------------------------------------------------------------- |
+| `TESTCONTAINERS_DOCKER_SOCKET_OVERRIDE` | `/var/run/docker.sock`      | Path to Docker's socket used by ryuk                                               |
+| `TESTCONTAINERS_RYUK_PRIVILEGED`        | `false`                     | Run ryuk as a privileged container                                                 |
+| `TESTCONTAINERS_RYUK_DISABLED`          | `false`                     | Disable ryuk                                                                       |
+| `RYUK_CONTAINER_IMAGE`                  | `testcontainers/ryuk:0.7.0` | Custom image for ryuk                                                              |
+| `RYUK_RECONNECTION_TIMEOUT`             | `10s`                       | Reconnection timeout for Ryuk TCP socket before Ryuk reaps all dangling containers |
```

