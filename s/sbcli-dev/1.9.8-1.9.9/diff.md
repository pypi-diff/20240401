# Comparing `tmp/sbcli-dev-1.9.8.zip` & `tmp/sbcli-dev-1.9.9.zip`

## zipinfo {}

```diff
@@ -1,135 +1,135 @@
 Zip file size: 161194 bytes, number of entries: 133
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 00:04 sbcli-dev-1.9.8/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_cli/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 00:04 sbcli-dev-1.9.8/sbcli_dev.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/
--rw-r--r--  2.0 unx      149 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/env_var
--rw-r--r--  2.0 unx     2159 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/setup.py
--rw-r--r--  2.0 unx       38 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/setup.cfg
--rw-r--r--  2.0 unx      730 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/README.md
--rw-r--r--  2.0 unx       84 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/pyproject.toml
--rw-r--r--  2.0 unx     1129 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/PKG-INFO
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/static/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/templates/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/blueprints/
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/__init__.py
--rw-r--r--  2.0 unx      717 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/caching_node_app.py
--rw-r--r--  2.0 unx     2508 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/utils.py
--rw-r--r--  2.0 unx     1638 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/auth_middleware.py
--rw-r--r--  2.0 unx      725 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/caching_node_app_k8s.py
--rw-r--r--  2.0 unx     1263 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/app.py
--rw-r--r--  2.0 unx     5078 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/node_utils.py
--rw-r--r--  2.0 unx     1434 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/node_webapp.py
--rw-r--r--  2.0 unx      703 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/snode_app.py
--rw-r--r--  2.0 unx     1466 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/static/deploy_spdk.yaml
--rw-r--r--  2.0 unx      417 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/static/list_deps.py
--rw-r--r--  2.0 unx      463 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/static/rpac.yaml
--rw-r--r--  2.0 unx      827 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/static/delete.py
--rw-r--r--  2.0 unx      507 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/static/deploy_cnode.yaml
--rw-r--r--  2.0 unx     1302 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/static/deploy.py
--rw-r--r--  2.0 unx      434 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/static/is_up.py
--rw-r--r--  2.0 unx      322 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/static/tst.py
--rw-r--r--  2.0 unx     1890 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/templates/deploy_spdk.yaml.j2
--rw-r--r--  2.0 unx     4795 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/blueprints/node_api_caching_ks.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/blueprints/__init__.py
--rw-r--r--  2.0 unx    12129 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/blueprints/caching_node_ops.py
--rw-r--r--  2.0 unx     6206 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/blueprints/web_api_pool.py
--rw-r--r--  2.0 unx     3103 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/blueprints/node_api_basic.py
--rw-r--r--  2.0 unx      975 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/blueprints/web_api_mgmt_node.py
--rw-r--r--  2.0 unx     5274 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/blueprints/web_api_cluster.py
--rw-r--r--  2.0 unx     5317 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/blueprints/web_api_caching_node.py
--rw-r--r--  2.0 unx     2940 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/blueprints/web_api_device.py
--rw-r--r--  2.0 unx     6326 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/blueprints/web_api_storage_node.py
--rw-r--r--  2.0 unx     7846 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/blueprints/caching_node_ops_k8s.py
--rw-r--r--  2.0 unx     5547 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/blueprints/node_api_caching_docker.py
--rw-r--r--  2.0 unx    11244 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/blueprints/csi.py
--rw-r--r--  2.0 unx     8585 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/blueprints/snode_ops.py
--rw-r--r--  2.0 unx     8169 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_web/blueprints/web_api_lvol.py
--rw-r--r--  2.0 unx      357 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_cli/main.py
--rw-r--r--  2.0 unx    76175 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_cli/cli.py
--rw-r--r--  2.0 unx       55 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/sbcli_dev.egg-info/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/sbcli_dev.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx       66 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/sbcli_dev.egg-info/requires.txt
--rw-r--r--  2.0 unx       49 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/sbcli_dev.egg-info/top_level.txt
--rw-r--r--  2.0 unx     4651 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/sbcli_dev.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx     1129 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/sbcli_dev.egg-info/PKG-INFO
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/scripts/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/services/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/models/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/controllers/
--rw-r--r--  2.0 unx     3193 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/snode_client.py
--rw-r--r--  2.0 unx     1426 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/constants.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/__init__.py
--rw-r--r--  2.0 unx     3444 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/cnode_client.py
--rw-r--r--  2.0 unx     3153 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/mgmt_node_ops.py
--rw-r--r--  2.0 unx     7626 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/utils.py
--rw-r--r--  2.0 unx    62998 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/storage_node_ops.py
--rw-r--r--  2.0 unx      279 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/shell_utils.py
--rw-r--r--  2.0 unx    23186 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/cluster_ops.py
--rw-r--r--  2.0 unx      938 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/pci_utils.py
--rw-r--r--  2.0 unx     6262 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/distr_controller.py
--rw-r--r--  2.0 unx    21361 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/rpc_client.py
--rw-r--r--  2.0 unx     8189 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/kv_store.py
--rw-r--r--  2.0 unx     5112 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/compute_node_ops.py
--rw-r--r--  2.0 unx      118 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/scripts/db_config_double.sh
--rw-r--r--  2.0 unx     1163 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/scripts/haproxy.cfg
--rw-r--r--  2.0 unx      648 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/scripts/deploy_stack.sh
--rw-r--r--  2.0 unx       43 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/scripts/run_ssh.sh
--rw-r--r--  2.0 unx     1493 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/scripts/__init__.py
--rw-r--r--  2.0 unx       54 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/scripts/db_config_single.sh
--rw-r--r--  2.0 unx     1420 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/scripts/install_deps.sh
--rw-r--r--  2.0 unx      152 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/scripts/set_db_config.sh
--rw-r--r--  2.0 unx     6716 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/scripts/docker-compose-swarm.yml
--rw-r--r--  2.0 unx     5305 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/scripts/stack_deploy_wait.sh
--rw-r--r--  2.0 unx      453 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/scripts/config_docker.sh
--rw-r--r--  2.0 unx      311 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/scripts/clean_local_storage_deploy.sh
--rw-r--r--  2.0 unx     3203 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/services/caching_node_monitor.py
--rw-r--r--  2.0 unx     4118 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/services/__init__.py
--rw-r--r--  2.0 unx     2423 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/services/port_stat_collector.py
--rw-r--r--  2.0 unx     2189 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/services/lvol_monitor.py
--rw-r--r--  2.0 unx      173 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/services/remove_service.sh
--rw-r--r--  2.0 unx     4637 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/services/distr_event_collector.py
--rw-r--r--  2.0 unx     3003 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/services/mgmt_node_monitor.py
--rw-r--r--  2.0 unx     2410 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/services/log_agg_service.py
--rw-r--r--  2.0 unx      229 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/services/service_template.service
--rw-r--r--  2.0 unx     7218 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/services/capacity_and_stats_collector.py
--rw-r--r--  2.0 unx     2612 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/services/cap_monitor.py
--rw-r--r--  2.0 unx     6360 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/services/storage_node_monitor.py
--rw-r--r--  2.0 unx      837 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/services/install_service.sh
--rw-r--r--  2.0 unx     5462 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/services/health_check_service.py
--rw-r--r--  2.0 unx     2490 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/services/device_monitor.py
--rw-r--r--  2.0 unx     5443 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/services/capacity_collector.py
--rw-r--r--  2.0 unx     4817 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/services/lvol_stat_collector.py
--rw-r--r--  2.0 unx     1500 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/models/events.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/models/__init__.py
--rw-r--r--  2.0 unx     2193 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/models/nvme_device.py
--rw-r--r--  2.0 unx     1228 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/models/global_settings.py
--rw-r--r--  2.0 unx     3766 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/models/caching_node.py
--rw-r--r--  2.0 unx     1020 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/models/port_stat.py
--rw-r--r--  2.0 unx      736 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/models/snapshot.py
--rw-r--r--  2.0 unx      806 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/models/iface.py
--rw-r--r--  2.0 unx     4242 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/models/stats.py
--rw-r--r--  2.0 unx     3222 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/models/storage_node.py
--rw-r--r--  2.0 unx      917 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/models/compute_node.py
--rw-r--r--  2.0 unx     1466 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/models/mgmt_node.py
--rw-r--r--  2.0 unx     1602 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/models/pool.py
--rw-r--r--  2.0 unx     2565 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/models/cluster.py
--rw-r--r--  2.0 unx     4846 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/models/base_model.py
--rw-r--r--  2.0 unx     2579 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/models/lvol_model.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/controllers/__init__.py
--rw-r--r--  2.0 unx     1521 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/controllers/storage_events.py
--rw-r--r--  2.0 unx     1900 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/controllers/cluster_events.py
--rw-r--r--  2.0 unx     1961 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/controllers/events_controller.py
--rw-r--r--  2.0 unx    46469 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/controllers/lvol_controller.py
--rw-r--r--  2.0 unx      695 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/controllers/pool_events.py
--rw-r--r--  2.0 unx    22847 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/controllers/caching_node_controller.py
--rw-r--r--  2.0 unx    10781 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/controllers/snapshot_controller.py
--rw-r--r--  2.0 unx     1120 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/controllers/mgmt_events.py
--rw-r--r--  2.0 unx    13528 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/controllers/device_controller.py
--rw-r--r--  2.0 unx     1425 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/controllers/lvol_events.py
--rw-r--r--  2.0 unx     1568 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/controllers/device_events.py
--rw-r--r--  2.0 unx     1122 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/controllers/snapshot_events.py
--rw-r--r--  2.0 unx    11300 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/controllers/health_controller.py
--rw-r--r--  2.0 unx    10375 b- defN 24-Mar-30 00:04 sbcli-dev-1.9.8/simplyblock_core/controllers/pool_controller.py
-133 files, 578889 bytes uncompressed, 137212 bytes compressed:  76.3%
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 17:21 sbcli-dev-1.9.9/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_cli/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 17:21 sbcli-dev-1.9.9/sbcli_dev.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/
+-rw-r--r--  2.0 unx      149 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/env_var
+-rw-r--r--  2.0 unx     2159 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/setup.py
+-rw-r--r--  2.0 unx       38 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/setup.cfg
+-rw-r--r--  2.0 unx      730 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/README.md
+-rw-r--r--  2.0 unx       84 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/pyproject.toml
+-rw-r--r--  2.0 unx     1129 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/PKG-INFO
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/static/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/templates/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/blueprints/
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/__init__.py
+-rw-r--r--  2.0 unx      717 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/caching_node_app.py
+-rw-r--r--  2.0 unx     2508 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/utils.py
+-rw-r--r--  2.0 unx     1638 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/auth_middleware.py
+-rw-r--r--  2.0 unx      725 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/caching_node_app_k8s.py
+-rw-r--r--  2.0 unx     1263 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/app.py
+-rw-r--r--  2.0 unx     5078 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/node_utils.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/node_webapp.py
+-rw-r--r--  2.0 unx      703 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/snode_app.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/static/deploy_spdk.yaml
+-rw-r--r--  2.0 unx      417 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/static/list_deps.py
+-rw-r--r--  2.0 unx      463 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/static/rpac.yaml
+-rw-r--r--  2.0 unx      827 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/static/delete.py
+-rw-r--r--  2.0 unx      507 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/static/deploy_cnode.yaml
+-rw-r--r--  2.0 unx     1302 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/static/deploy.py
+-rw-r--r--  2.0 unx      434 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/static/is_up.py
+-rw-r--r--  2.0 unx      322 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/static/tst.py
+-rw-r--r--  2.0 unx     1890 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/templates/deploy_spdk.yaml.j2
+-rw-r--r--  2.0 unx     4795 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/blueprints/node_api_caching_ks.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/blueprints/__init__.py
+-rw-r--r--  2.0 unx    12129 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/blueprints/caching_node_ops.py
+-rw-r--r--  2.0 unx     6206 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/blueprints/web_api_pool.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/blueprints/node_api_basic.py
+-rw-r--r--  2.0 unx      975 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/blueprints/web_api_mgmt_node.py
+-rw-r--r--  2.0 unx     5274 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/blueprints/web_api_cluster.py
+-rw-r--r--  2.0 unx     5317 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/blueprints/web_api_caching_node.py
+-rw-r--r--  2.0 unx     2940 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/blueprints/web_api_device.py
+-rw-r--r--  2.0 unx     6326 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/blueprints/web_api_storage_node.py
+-rw-r--r--  2.0 unx     7846 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/blueprints/caching_node_ops_k8s.py
+-rw-r--r--  2.0 unx     5547 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/blueprints/node_api_caching_docker.py
+-rw-r--r--  2.0 unx    11244 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/blueprints/csi.py
+-rw-r--r--  2.0 unx     8585 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/blueprints/snode_ops.py
+-rw-r--r--  2.0 unx     8169 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_web/blueprints/web_api_lvol.py
+-rw-r--r--  2.0 unx      357 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_cli/main.py
+-rw-r--r--  2.0 unx    76175 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_cli/cli.py
+-rw-r--r--  2.0 unx       55 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/sbcli_dev.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/sbcli_dev.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx       66 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/sbcli_dev.egg-info/requires.txt
+-rw-r--r--  2.0 unx       49 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/sbcli_dev.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     4651 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/sbcli_dev.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx     1129 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/sbcli_dev.egg-info/PKG-INFO
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/scripts/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/services/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/models/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/controllers/
+-rw-r--r--  2.0 unx     3193 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/snode_client.py
+-rw-r--r--  2.0 unx     1426 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/constants.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/__init__.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/cnode_client.py
+-rw-r--r--  2.0 unx     3153 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/mgmt_node_ops.py
+-rw-r--r--  2.0 unx     7626 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/utils.py
+-rw-r--r--  2.0 unx    62998 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/storage_node_ops.py
+-rw-r--r--  2.0 unx      279 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/shell_utils.py
+-rw-r--r--  2.0 unx    23186 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/cluster_ops.py
+-rw-r--r--  2.0 unx      938 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/pci_utils.py
+-rw-r--r--  2.0 unx     6262 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/distr_controller.py
+-rw-r--r--  2.0 unx    21362 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/rpc_client.py
+-rw-r--r--  2.0 unx     8189 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/kv_store.py
+-rw-r--r--  2.0 unx     5112 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/compute_node_ops.py
+-rw-r--r--  2.0 unx      118 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/scripts/db_config_double.sh
+-rw-r--r--  2.0 unx     1163 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/scripts/haproxy.cfg
+-rw-r--r--  2.0 unx      648 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/scripts/deploy_stack.sh
+-rw-r--r--  2.0 unx       43 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/scripts/run_ssh.sh
+-rw-r--r--  2.0 unx     1493 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/scripts/__init__.py
+-rw-r--r--  2.0 unx       54 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/scripts/db_config_single.sh
+-rw-r--r--  2.0 unx     1420 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/scripts/install_deps.sh
+-rw-r--r--  2.0 unx      152 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/scripts/set_db_config.sh
+-rw-r--r--  2.0 unx     6716 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/scripts/docker-compose-swarm.yml
+-rw-r--r--  2.0 unx     5305 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/scripts/stack_deploy_wait.sh
+-rw-r--r--  2.0 unx      453 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/scripts/config_docker.sh
+-rw-r--r--  2.0 unx      311 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/scripts/clean_local_storage_deploy.sh
+-rw-r--r--  2.0 unx     3203 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/services/caching_node_monitor.py
+-rw-r--r--  2.0 unx     4118 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/services/__init__.py
+-rw-r--r--  2.0 unx     2423 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/services/port_stat_collector.py
+-rw-r--r--  2.0 unx     2189 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/services/lvol_monitor.py
+-rw-r--r--  2.0 unx      173 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/services/remove_service.sh
+-rw-r--r--  2.0 unx     4637 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/services/distr_event_collector.py
+-rw-r--r--  2.0 unx     3003 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/services/mgmt_node_monitor.py
+-rw-r--r--  2.0 unx     2410 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/services/log_agg_service.py
+-rw-r--r--  2.0 unx      229 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/services/service_template.service
+-rw-r--r--  2.0 unx     7218 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/services/capacity_and_stats_collector.py
+-rw-r--r--  2.0 unx     2612 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/services/cap_monitor.py
+-rw-r--r--  2.0 unx     6360 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/services/storage_node_monitor.py
+-rw-r--r--  2.0 unx      837 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/services/install_service.sh
+-rw-r--r--  2.0 unx     5462 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/services/health_check_service.py
+-rw-r--r--  2.0 unx     2490 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/services/device_monitor.py
+-rw-r--r--  2.0 unx     5443 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/services/capacity_collector.py
+-rw-r--r--  2.0 unx     4817 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/services/lvol_stat_collector.py
+-rw-r--r--  2.0 unx     1500 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/models/events.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/models/__init__.py
+-rw-r--r--  2.0 unx     2193 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/models/nvme_device.py
+-rw-r--r--  2.0 unx     1228 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/models/global_settings.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/models/caching_node.py
+-rw-r--r--  2.0 unx     1020 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/models/port_stat.py
+-rw-r--r--  2.0 unx      736 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/models/snapshot.py
+-rw-r--r--  2.0 unx      806 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/models/iface.py
+-rw-r--r--  2.0 unx     4242 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/models/stats.py
+-rw-r--r--  2.0 unx     3222 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/models/storage_node.py
+-rw-r--r--  2.0 unx      917 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/models/compute_node.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/models/mgmt_node.py
+-rw-r--r--  2.0 unx     1602 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/models/pool.py
+-rw-r--r--  2.0 unx     2565 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/models/cluster.py
+-rw-r--r--  2.0 unx     4846 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/models/base_model.py
+-rw-r--r--  2.0 unx     2579 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/models/lvol_model.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/controllers/__init__.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/controllers/storage_events.py
+-rw-r--r--  2.0 unx     1900 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/controllers/cluster_events.py
+-rw-r--r--  2.0 unx     1961 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/controllers/events_controller.py
+-rw-r--r--  2.0 unx    46469 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/controllers/lvol_controller.py
+-rw-r--r--  2.0 unx      695 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/controllers/pool_events.py
+-rw-r--r--  2.0 unx    22847 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/controllers/caching_node_controller.py
+-rw-r--r--  2.0 unx    10781 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/controllers/snapshot_controller.py
+-rw-r--r--  2.0 unx     1120 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/controllers/mgmt_events.py
+-rw-r--r--  2.0 unx    13549 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/controllers/device_controller.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/controllers/lvol_events.py
+-rw-r--r--  2.0 unx     1568 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/controllers/device_events.py
+-rw-r--r--  2.0 unx     1122 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/controllers/snapshot_events.py
+-rw-r--r--  2.0 unx    11300 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/controllers/health_controller.py
+-rw-r--r--  2.0 unx    10375 b- defN 24-Apr-01 17:21 sbcli-dev-1.9.9/simplyblock_core/controllers/pool_controller.py
+133 files, 578911 bytes uncompressed, 137212 bytes compressed:  76.3%
```

## zipnote {}

```diff
@@ -1,400 +1,400 @@
-Filename: sbcli-dev-1.9.8/
+Filename: sbcli-dev-1.9.9/
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/
+Filename: sbcli-dev-1.9.9/simplyblock_web/
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_cli/
+Filename: sbcli-dev-1.9.9/simplyblock_cli/
 Comment: 
 
-Filename: sbcli-dev-1.9.8/sbcli_dev.egg-info/
+Filename: sbcli-dev-1.9.9/sbcli_dev.egg-info/
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/
+Filename: sbcli-dev-1.9.9/simplyblock_core/
 Comment: 
 
-Filename: sbcli-dev-1.9.8/env_var
+Filename: sbcli-dev-1.9.9/env_var
 Comment: 
 
-Filename: sbcli-dev-1.9.8/setup.py
+Filename: sbcli-dev-1.9.9/setup.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/setup.cfg
+Filename: sbcli-dev-1.9.9/setup.cfg
 Comment: 
 
-Filename: sbcli-dev-1.9.8/README.md
+Filename: sbcli-dev-1.9.9/README.md
 Comment: 
 
-Filename: sbcli-dev-1.9.8/pyproject.toml
+Filename: sbcli-dev-1.9.9/pyproject.toml
 Comment: 
 
-Filename: sbcli-dev-1.9.8/PKG-INFO
+Filename: sbcli-dev-1.9.9/PKG-INFO
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/static/
+Filename: sbcli-dev-1.9.9/simplyblock_web/static/
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/templates/
+Filename: sbcli-dev-1.9.9/simplyblock_web/templates/
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/blueprints/
+Filename: sbcli-dev-1.9.9/simplyblock_web/blueprints/
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/__init__.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/__init__.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/caching_node_app.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/caching_node_app.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/utils.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/utils.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/auth_middleware.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/auth_middleware.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/caching_node_app_k8s.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/caching_node_app_k8s.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/app.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/app.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/node_utils.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/node_utils.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/node_webapp.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/node_webapp.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/snode_app.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/snode_app.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/static/deploy_spdk.yaml
+Filename: sbcli-dev-1.9.9/simplyblock_web/static/deploy_spdk.yaml
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/static/list_deps.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/static/list_deps.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/static/rpac.yaml
+Filename: sbcli-dev-1.9.9/simplyblock_web/static/rpac.yaml
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/static/delete.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/static/delete.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/static/deploy_cnode.yaml
+Filename: sbcli-dev-1.9.9/simplyblock_web/static/deploy_cnode.yaml
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/static/deploy.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/static/deploy.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/static/is_up.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/static/is_up.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/static/tst.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/static/tst.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/templates/deploy_spdk.yaml.j2
+Filename: sbcli-dev-1.9.9/simplyblock_web/templates/deploy_spdk.yaml.j2
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/blueprints/node_api_caching_ks.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/blueprints/node_api_caching_ks.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/blueprints/__init__.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/blueprints/__init__.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/blueprints/caching_node_ops.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/blueprints/caching_node_ops.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/blueprints/web_api_pool.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/blueprints/web_api_pool.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/blueprints/node_api_basic.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/blueprints/node_api_basic.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/blueprints/web_api_mgmt_node.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/blueprints/web_api_mgmt_node.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/blueprints/web_api_cluster.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/blueprints/web_api_cluster.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/blueprints/web_api_caching_node.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/blueprints/web_api_caching_node.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/blueprints/web_api_device.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/blueprints/web_api_device.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/blueprints/web_api_storage_node.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/blueprints/web_api_storage_node.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/blueprints/caching_node_ops_k8s.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/blueprints/caching_node_ops_k8s.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/blueprints/node_api_caching_docker.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/blueprints/node_api_caching_docker.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/blueprints/csi.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/blueprints/csi.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/blueprints/snode_ops.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/blueprints/snode_ops.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_web/blueprints/web_api_lvol.py
+Filename: sbcli-dev-1.9.9/simplyblock_web/blueprints/web_api_lvol.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_cli/main.py
+Filename: sbcli-dev-1.9.9/simplyblock_cli/main.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_cli/cli.py
+Filename: sbcli-dev-1.9.9/simplyblock_cli/cli.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/sbcli_dev.egg-info/entry_points.txt
+Filename: sbcli-dev-1.9.9/sbcli_dev.egg-info/entry_points.txt
 Comment: 
 
-Filename: sbcli-dev-1.9.8/sbcli_dev.egg-info/dependency_links.txt
+Filename: sbcli-dev-1.9.9/sbcli_dev.egg-info/dependency_links.txt
 Comment: 
 
-Filename: sbcli-dev-1.9.8/sbcli_dev.egg-info/requires.txt
+Filename: sbcli-dev-1.9.9/sbcli_dev.egg-info/requires.txt
 Comment: 
 
-Filename: sbcli-dev-1.9.8/sbcli_dev.egg-info/top_level.txt
+Filename: sbcli-dev-1.9.9/sbcli_dev.egg-info/top_level.txt
 Comment: 
 
-Filename: sbcli-dev-1.9.8/sbcli_dev.egg-info/SOURCES.txt
+Filename: sbcli-dev-1.9.9/sbcli_dev.egg-info/SOURCES.txt
 Comment: 
 
-Filename: sbcli-dev-1.9.8/sbcli_dev.egg-info/PKG-INFO
+Filename: sbcli-dev-1.9.9/sbcli_dev.egg-info/PKG-INFO
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/scripts/
+Filename: sbcli-dev-1.9.9/simplyblock_core/scripts/
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/services/
+Filename: sbcli-dev-1.9.9/simplyblock_core/services/
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/models/
+Filename: sbcli-dev-1.9.9/simplyblock_core/models/
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/controllers/
+Filename: sbcli-dev-1.9.9/simplyblock_core/controllers/
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/snode_client.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/snode_client.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/constants.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/constants.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/__init__.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/__init__.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/cnode_client.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/cnode_client.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/mgmt_node_ops.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/mgmt_node_ops.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/utils.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/utils.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/storage_node_ops.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/storage_node_ops.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/shell_utils.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/shell_utils.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/cluster_ops.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/cluster_ops.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/pci_utils.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/pci_utils.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/distr_controller.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/distr_controller.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/rpc_client.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/rpc_client.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/kv_store.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/kv_store.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/compute_node_ops.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/compute_node_ops.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/scripts/db_config_double.sh
+Filename: sbcli-dev-1.9.9/simplyblock_core/scripts/db_config_double.sh
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/scripts/haproxy.cfg
+Filename: sbcli-dev-1.9.9/simplyblock_core/scripts/haproxy.cfg
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/scripts/deploy_stack.sh
+Filename: sbcli-dev-1.9.9/simplyblock_core/scripts/deploy_stack.sh
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/scripts/run_ssh.sh
+Filename: sbcli-dev-1.9.9/simplyblock_core/scripts/run_ssh.sh
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/scripts/__init__.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/scripts/__init__.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/scripts/db_config_single.sh
+Filename: sbcli-dev-1.9.9/simplyblock_core/scripts/db_config_single.sh
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/scripts/install_deps.sh
+Filename: sbcli-dev-1.9.9/simplyblock_core/scripts/install_deps.sh
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/scripts/set_db_config.sh
+Filename: sbcli-dev-1.9.9/simplyblock_core/scripts/set_db_config.sh
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/scripts/docker-compose-swarm.yml
+Filename: sbcli-dev-1.9.9/simplyblock_core/scripts/docker-compose-swarm.yml
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/scripts/stack_deploy_wait.sh
+Filename: sbcli-dev-1.9.9/simplyblock_core/scripts/stack_deploy_wait.sh
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/scripts/config_docker.sh
+Filename: sbcli-dev-1.9.9/simplyblock_core/scripts/config_docker.sh
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/scripts/clean_local_storage_deploy.sh
+Filename: sbcli-dev-1.9.9/simplyblock_core/scripts/clean_local_storage_deploy.sh
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/services/caching_node_monitor.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/services/caching_node_monitor.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/services/__init__.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/services/__init__.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/services/port_stat_collector.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/services/port_stat_collector.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/services/lvol_monitor.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/services/lvol_monitor.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/services/remove_service.sh
+Filename: sbcli-dev-1.9.9/simplyblock_core/services/remove_service.sh
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/services/distr_event_collector.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/services/distr_event_collector.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/services/mgmt_node_monitor.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/services/mgmt_node_monitor.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/services/log_agg_service.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/services/log_agg_service.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/services/service_template.service
+Filename: sbcli-dev-1.9.9/simplyblock_core/services/service_template.service
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/services/capacity_and_stats_collector.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/services/capacity_and_stats_collector.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/services/cap_monitor.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/services/cap_monitor.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/services/storage_node_monitor.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/services/storage_node_monitor.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/services/install_service.sh
+Filename: sbcli-dev-1.9.9/simplyblock_core/services/install_service.sh
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/services/health_check_service.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/services/health_check_service.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/services/device_monitor.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/services/device_monitor.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/services/capacity_collector.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/services/capacity_collector.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/services/lvol_stat_collector.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/services/lvol_stat_collector.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/models/events.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/models/events.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/models/__init__.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/models/__init__.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/models/nvme_device.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/models/nvme_device.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/models/global_settings.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/models/global_settings.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/models/caching_node.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/models/caching_node.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/models/port_stat.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/models/port_stat.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/models/snapshot.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/models/snapshot.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/models/iface.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/models/iface.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/models/stats.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/models/stats.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/models/storage_node.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/models/storage_node.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/models/compute_node.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/models/compute_node.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/models/mgmt_node.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/models/mgmt_node.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/models/pool.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/models/pool.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/models/cluster.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/models/cluster.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/models/base_model.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/models/base_model.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/models/lvol_model.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/models/lvol_model.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/controllers/__init__.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/controllers/__init__.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/controllers/storage_events.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/controllers/storage_events.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/controllers/cluster_events.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/controllers/cluster_events.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/controllers/events_controller.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/controllers/events_controller.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/controllers/lvol_controller.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/controllers/lvol_controller.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/controllers/pool_events.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/controllers/pool_events.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/controllers/caching_node_controller.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/controllers/caching_node_controller.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/controllers/snapshot_controller.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/controllers/snapshot_controller.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/controllers/mgmt_events.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/controllers/mgmt_events.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/controllers/device_controller.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/controllers/device_controller.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/controllers/lvol_events.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/controllers/lvol_events.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/controllers/device_events.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/controllers/device_events.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/controllers/snapshot_events.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/controllers/snapshot_events.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/controllers/health_controller.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/controllers/health_controller.py
 Comment: 
 
-Filename: sbcli-dev-1.9.8/simplyblock_core/controllers/pool_controller.py
+Filename: sbcli-dev-1.9.9/simplyblock_core/controllers/pool_controller.py
 Comment: 
 
 Zip file comment:
```

## Comparing `sbcli-dev-1.9.8/setup.py` & `sbcli-dev-1.9.9/setup.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/README.md` & `sbcli-dev-1.9.9/README.md`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/PKG-INFO` & `sbcli-dev-1.9.9/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-dev
-Version: 1.9.8
+Version: 1.9.9
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli-dev-1.9.8/simplyblock_web/caching_node_app.py` & `sbcli-dev-1.9.9/simplyblock_web/caching_node_app.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_web/utils.py` & `sbcli-dev-1.9.9/simplyblock_web/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_web/auth_middleware.py` & `sbcli-dev-1.9.9/simplyblock_web/auth_middleware.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_web/caching_node_app_k8s.py` & `sbcli-dev-1.9.9/simplyblock_web/caching_node_app_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_web/app.py` & `sbcli-dev-1.9.9/simplyblock_web/app.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_web/node_utils.py` & `sbcli-dev-1.9.9/simplyblock_web/node_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_web/node_webapp.py` & `sbcli-dev-1.9.9/simplyblock_web/node_webapp.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_web/snode_app.py` & `sbcli-dev-1.9.9/simplyblock_web/snode_app.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_web/static/deploy_spdk.yaml` & `sbcli-dev-1.9.9/simplyblock_web/static/deploy_spdk.yaml`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_web/static/delete.py` & `sbcli-dev-1.9.9/simplyblock_web/static/delete.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_web/static/deploy.py` & `sbcli-dev-1.9.9/simplyblock_web/static/deploy.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_web/templates/deploy_spdk.yaml.j2` & `sbcli-dev-1.9.9/simplyblock_web/templates/deploy_spdk.yaml.j2`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_web/blueprints/node_api_caching_ks.py` & `sbcli-dev-1.9.9/simplyblock_web/blueprints/node_api_caching_ks.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_web/blueprints/caching_node_ops.py` & `sbcli-dev-1.9.9/simplyblock_web/blueprints/caching_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_web/blueprints/web_api_pool.py` & `sbcli-dev-1.9.9/simplyblock_web/blueprints/web_api_pool.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_web/blueprints/node_api_basic.py` & `sbcli-dev-1.9.9/simplyblock_web/blueprints/node_api_basic.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_web/blueprints/web_api_mgmt_node.py` & `sbcli-dev-1.9.9/simplyblock_web/blueprints/web_api_mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_web/blueprints/web_api_cluster.py` & `sbcli-dev-1.9.9/simplyblock_web/blueprints/web_api_cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_web/blueprints/web_api_caching_node.py` & `sbcli-dev-1.9.9/simplyblock_web/blueprints/web_api_caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_web/blueprints/web_api_device.py` & `sbcli-dev-1.9.9/simplyblock_web/blueprints/web_api_device.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_web/blueprints/web_api_storage_node.py` & `sbcli-dev-1.9.9/simplyblock_web/blueprints/web_api_storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_web/blueprints/caching_node_ops_k8s.py` & `sbcli-dev-1.9.9/simplyblock_web/blueprints/caching_node_ops_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_web/blueprints/node_api_caching_docker.py` & `sbcli-dev-1.9.9/simplyblock_web/blueprints/node_api_caching_docker.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_web/blueprints/csi.py` & `sbcli-dev-1.9.9/simplyblock_web/blueprints/csi.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_web/blueprints/snode_ops.py` & `sbcli-dev-1.9.9/simplyblock_web/blueprints/snode_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_web/blueprints/web_api_lvol.py` & `sbcli-dev-1.9.9/simplyblock_web/blueprints/web_api_lvol.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_cli/cli.py` & `sbcli-dev-1.9.9/simplyblock_cli/cli.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/sbcli_dev.egg-info/SOURCES.txt` & `sbcli-dev-1.9.9/sbcli_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/sbcli_dev.egg-info/PKG-INFO` & `sbcli-dev-1.9.9/sbcli_dev.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-dev
-Version: 1.9.8
+Version: 1.9.9
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli-dev-1.9.8/simplyblock_core/snode_client.py` & `sbcli-dev-1.9.9/simplyblock_core/snode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/constants.py` & `sbcli-dev-1.9.9/simplyblock_core/constants.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/cnode_client.py` & `sbcli-dev-1.9.9/simplyblock_core/cnode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/mgmt_node_ops.py` & `sbcli-dev-1.9.9/simplyblock_core/mgmt_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/utils.py` & `sbcli-dev-1.9.9/simplyblock_core/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/storage_node_ops.py` & `sbcli-dev-1.9.9/simplyblock_core/storage_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/cluster_ops.py` & `sbcli-dev-1.9.9/simplyblock_core/cluster_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/pci_utils.py` & `sbcli-dev-1.9.9/simplyblock_core/pci_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/distr_controller.py` & `sbcli-dev-1.9.9/simplyblock_core/distr_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/rpc_client.py` & `sbcli-dev-1.9.9/simplyblock_core/rpc_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -505,15 +505,15 @@
             "pt_name": name
         }
         return self._request("bdev_passtest_delete", params)
 
     def bdev_nvme_set_options(self):
         params = {
             "action_on_timeout": "abort",
-            "timeout_us": 25000,
+            "timeout_us": 250000,
             "ctrlr_loss_timeout_sec": -1,
             "reconnect_delay_sec": 15,
             "transport_retry_count": 1,
             "bdev_retry_count": 1}
         return self._request("bdev_nvme_set_options", params)
 
     def bdev_set_options(self, bdev_io_pool_size, bdev_io_cache_size, iobuf_small_cache_size, iobuf_large_cache_size):
```

## Comparing `sbcli-dev-1.9.8/simplyblock_core/kv_store.py` & `sbcli-dev-1.9.9/simplyblock_core/kv_store.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/compute_node_ops.py` & `sbcli-dev-1.9.9/simplyblock_core/compute_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/scripts/haproxy.cfg` & `sbcli-dev-1.9.9/simplyblock_core/scripts/haproxy.cfg`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/scripts/deploy_stack.sh` & `sbcli-dev-1.9.9/simplyblock_core/scripts/deploy_stack.sh`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/scripts/__init__.py` & `sbcli-dev-1.9.9/simplyblock_core/scripts/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/scripts/install_deps.sh` & `sbcli-dev-1.9.9/simplyblock_core/scripts/install_deps.sh`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/scripts/docker-compose-swarm.yml` & `sbcli-dev-1.9.9/simplyblock_core/scripts/docker-compose-swarm.yml`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/scripts/stack_deploy_wait.sh` & `sbcli-dev-1.9.9/simplyblock_core/scripts/stack_deploy_wait.sh`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/services/caching_node_monitor.py` & `sbcli-dev-1.9.9/simplyblock_core/services/caching_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/services/__init__.py` & `sbcli-dev-1.9.9/simplyblock_core/services/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/services/port_stat_collector.py` & `sbcli-dev-1.9.9/simplyblock_core/services/port_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/services/lvol_monitor.py` & `sbcli-dev-1.9.9/simplyblock_core/services/lvol_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/services/distr_event_collector.py` & `sbcli-dev-1.9.9/simplyblock_core/services/distr_event_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/services/mgmt_node_monitor.py` & `sbcli-dev-1.9.9/simplyblock_core/services/mgmt_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/services/log_agg_service.py` & `sbcli-dev-1.9.9/simplyblock_core/services/log_agg_service.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/services/capacity_and_stats_collector.py` & `sbcli-dev-1.9.9/simplyblock_core/services/capacity_and_stats_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/services/cap_monitor.py` & `sbcli-dev-1.9.9/simplyblock_core/services/cap_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/services/storage_node_monitor.py` & `sbcli-dev-1.9.9/simplyblock_core/services/storage_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/services/install_service.sh` & `sbcli-dev-1.9.9/simplyblock_core/services/install_service.sh`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/services/health_check_service.py` & `sbcli-dev-1.9.9/simplyblock_core/services/health_check_service.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/services/device_monitor.py` & `sbcli-dev-1.9.9/simplyblock_core/services/device_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/services/capacity_collector.py` & `sbcli-dev-1.9.9/simplyblock_core/services/capacity_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/services/lvol_stat_collector.py` & `sbcli-dev-1.9.9/simplyblock_core/services/lvol_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/models/events.py` & `sbcli-dev-1.9.9/simplyblock_core/models/events.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/models/nvme_device.py` & `sbcli-dev-1.9.9/simplyblock_core/models/nvme_device.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/models/global_settings.py` & `sbcli-dev-1.9.9/simplyblock_core/models/global_settings.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/models/caching_node.py` & `sbcli-dev-1.9.9/simplyblock_core/models/caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/models/port_stat.py` & `sbcli-dev-1.9.9/simplyblock_core/models/port_stat.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/models/snapshot.py` & `sbcli-dev-1.9.9/simplyblock_core/models/snapshot.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/models/iface.py` & `sbcli-dev-1.9.9/simplyblock_core/models/iface.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/models/stats.py` & `sbcli-dev-1.9.9/simplyblock_core/models/stats.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/models/storage_node.py` & `sbcli-dev-1.9.9/simplyblock_core/models/storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/models/compute_node.py` & `sbcli-dev-1.9.9/simplyblock_core/models/compute_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/models/mgmt_node.py` & `sbcli-dev-1.9.9/simplyblock_core/models/mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/models/pool.py` & `sbcli-dev-1.9.9/simplyblock_core/models/pool.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/models/cluster.py` & `sbcli-dev-1.9.9/simplyblock_core/models/cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/models/base_model.py` & `sbcli-dev-1.9.9/simplyblock_core/models/base_model.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/models/lvol_model.py` & `sbcli-dev-1.9.9/simplyblock_core/models/lvol_model.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/controllers/storage_events.py` & `sbcli-dev-1.9.9/simplyblock_core/controllers/storage_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/controllers/cluster_events.py` & `sbcli-dev-1.9.9/simplyblock_core/controllers/cluster_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/controllers/events_controller.py` & `sbcli-dev-1.9.9/simplyblock_core/controllers/events_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/controllers/lvol_controller.py` & `sbcli-dev-1.9.9/simplyblock_core/controllers/lvol_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/controllers/pool_events.py` & `sbcli-dev-1.9.9/simplyblock_core/controllers/pool_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/controllers/caching_node_controller.py` & `sbcli-dev-1.9.9/simplyblock_core/controllers/caching_node_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/controllers/snapshot_controller.py` & `sbcli-dev-1.9.9/simplyblock_core/controllers/snapshot_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/controllers/mgmt_events.py` & `sbcli-dev-1.9.9/simplyblock_core/controllers/mgmt_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/controllers/device_controller.py` & `sbcli-dev-1.9.9/simplyblock_core/controllers/device_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,14 +207,15 @@
 
 
 def set_device_testing_mode(device_id, mode):
     db_controller = DBController()
     device = db_controller.get_storage_devices(device_id)
     if not device:
         logger.error("device not found")
+        return False
 
     snode = db_controller.get_storage_node_by_id(device.node_id)
     if not snode:
         logger.error("node not found")
         return False
 
     logger.info(f"Set device:{device_id} Test mode:{mode}")
```

## Comparing `sbcli-dev-1.9.8/simplyblock_core/controllers/lvol_events.py` & `sbcli-dev-1.9.9/simplyblock_core/controllers/lvol_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/controllers/device_events.py` & `sbcli-dev-1.9.9/simplyblock_core/controllers/device_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/controllers/snapshot_events.py` & `sbcli-dev-1.9.9/simplyblock_core/controllers/snapshot_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/controllers/health_controller.py` & `sbcli-dev-1.9.9/simplyblock_core/controllers/health_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-dev-1.9.8/simplyblock_core/controllers/pool_controller.py` & `sbcli-dev-1.9.9/simplyblock_core/controllers/pool_controller.py`

 * *Files identical despite different names*

