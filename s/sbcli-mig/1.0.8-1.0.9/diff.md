# Comparing `tmp/sbcli-mig-1.0.8.zip` & `tmp/sbcli-mig-1.0.9.zip`

## zipinfo {}

```diff
@@ -1,146 +1,146 @@
-Zip file size: 175996 bytes, number of entries: 144
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 16:50 sbcli-mig-1.0.8/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 16:50 sbcli-mig-1.0.8/simplyblock_web/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 16:50 sbcli-mig-1.0.8/simplyblock_cli/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 16:50 sbcli-mig-1.0.8/sbcli_mig.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 16:50 sbcli-mig-1.0.8/simplyblock_core/
--rw-r--r--  2.0 unx      149 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/env_var
--rw-r--r--  2.0 unx     2251 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/setup.py
--rw-r--r--  2.0 unx       38 b- defN 24-Mar-30 16:50 sbcli-mig-1.0.8/setup.cfg
--rw-r--r--  2.0 unx      730 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/README.md
--rw-r--r--  2.0 unx       84 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/pyproject.toml
--rw-r--r--  2.0 unx     1129 b- defN 24-Mar-30 16:50 sbcli-mig-1.0.8/PKG-INFO
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 16:50 sbcli-mig-1.0.8/simplyblock_web/static/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 16:50 sbcli-mig-1.0.8/simplyblock_web/templates/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 16:50 sbcli-mig-1.0.8/simplyblock_web/blueprints/
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/__init__.py
--rw-r--r--  2.0 unx      717 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/caching_node_app.py
--rw-r--r--  2.0 unx     2508 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/utils.py
--rw-r--r--  2.0 unx     1638 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/auth_middleware.py
--rw-r--r--  2.0 unx      725 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/caching_node_app_k8s.py
--rw-r--r--  2.0 unx     1263 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/app.py
--rw-r--r--  2.0 unx     5078 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/node_utils.py
--rw-r--r--  2.0 unx     1434 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/node_webapp.py
--rw-r--r--  2.0 unx      703 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/snode_app.py
--rw-r--r--  2.0 unx     1466 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/static/deploy_spdk.yaml
--rw-r--r--  2.0 unx      417 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/static/list_deps.py
--rw-r--r--  2.0 unx      463 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/static/rpac.yaml
--rw-r--r--  2.0 unx      827 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/static/delete.py
--rw-r--r--  2.0 unx      507 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/static/deploy_cnode.yaml
--rw-r--r--  2.0 unx     1302 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/static/deploy.py
--rw-r--r--  2.0 unx      434 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/static/is_up.py
--rw-r--r--  2.0 unx      322 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/static/tst.py
--rw-r--r--  2.0 unx     1890 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/templates/deploy_spdk.yaml.j2
--rw-r--r--  2.0 unx     4795 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/blueprints/node_api_caching_ks.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/blueprints/__init__.py
--rw-r--r--  2.0 unx    12129 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/blueprints/caching_node_ops.py
--rw-r--r--  2.0 unx     6206 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/blueprints/web_api_pool.py
--rw-r--r--  2.0 unx     3103 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/blueprints/node_api_basic.py
--rw-r--r--  2.0 unx      975 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/blueprints/web_api_mgmt_node.py
--rw-r--r--  2.0 unx     5274 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/blueprints/web_api_cluster.py
--rw-r--r--  2.0 unx     5317 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/blueprints/web_api_caching_node.py
--rw-r--r--  2.0 unx     2940 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/blueprints/web_api_device.py
--rw-r--r--  2.0 unx     6326 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/blueprints/web_api_storage_node.py
--rw-r--r--  2.0 unx     7846 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/blueprints/caching_node_ops_k8s.py
--rw-r--r--  2.0 unx     5547 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/blueprints/node_api_caching_docker.py
--rw-r--r--  2.0 unx    11244 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/blueprints/csi.py
--rw-r--r--  2.0 unx     8585 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/blueprints/snode_ops.py
--rw-r--r--  2.0 unx     8169 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_web/blueprints/web_api_lvol.py
--rw-r--r--  2.0 unx      357 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_cli/main.py
--rw-r--r--  2.0 unx    75229 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_cli/cli.py
--rw-r--r--  2.0 unx       55 b- defN 24-Mar-30 16:50 sbcli-mig-1.0.8/sbcli_mig.egg-info/entry_points.txt
--rw-r--r--  2.0 unx        1 b- defN 24-Mar-30 16:50 sbcli-mig-1.0.8/sbcli_mig.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx       66 b- defN 24-Mar-30 16:50 sbcli-mig-1.0.8/sbcli_mig.egg-info/requires.txt
--rw-r--r--  2.0 unx       49 b- defN 24-Mar-30 16:50 sbcli-mig-1.0.8/sbcli_mig.egg-info/top_level.txt
--rw-r--r--  2.0 unx     5073 b- defN 24-Mar-30 16:50 sbcli-mig-1.0.8/sbcli_mig.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx     1129 b- defN 24-Mar-30 16:50 sbcli-mig-1.0.8/sbcli_mig.egg-info/PKG-INFO
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 16:50 sbcli-mig-1.0.8/simplyblock_core/scripts/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 16:50 sbcli-mig-1.0.8/simplyblock_core/services/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 16:50 sbcli-mig-1.0.8/simplyblock_core/models/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 16:50 sbcli-mig-1.0.8/simplyblock_core/controllers/
--rw-r--r--  2.0 unx     3193 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/snode_client.py
--rw-r--r--  2.0 unx     1426 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/constants.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/__init__.py
--rw-r--r--  2.0 unx     3444 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/cnode_client.py
--rw-r--r--  2.0 unx     3153 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/mgmt_node_ops.py
--rw-r--r--  2.0 unx     7557 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/utils.py
--rw-r--r--  2.0 unx    63003 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/storage_node_ops.py
--rw-r--r--  2.0 unx      279 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/shell_utils.py
--rw-r--r--  2.0 unx    23325 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/cluster_ops.py
--rw-r--r--  2.0 unx      938 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/pci_utils.py
--rw-r--r--  2.0 unx     6262 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/distr_controller.py
--rw-r--r--  2.0 unx    20877 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/rpc_client.py
--rw-r--r--  2.0 unx     8189 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/kv_store.py
--rw-r--r--  2.0 unx     5112 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/compute_node_ops.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 16:50 sbcli-mig-1.0.8/simplyblock_core/scripts/alerting/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Mar-30 16:50 sbcli-mig-1.0.8/simplyblock_core/scripts/dashboards/
--rw-r--r--  2.0 unx      118 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/scripts/db_config_double.sh
--rw-r--r--  2.0 unx     1163 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/scripts/haproxy.cfg
--rw-r--r--  2.0 unx      694 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/scripts/deploy_stack.sh
--rw-r--r--  2.0 unx       43 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/scripts/run_ssh.sh
--rw-r--r--  2.0 unx     1694 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/scripts/__init__.py
--rw-r--r--  2.0 unx       54 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/scripts/db_config_single.sh
--rw-r--r--  2.0 unx     1420 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/scripts/install_deps.sh
--rw-r--r--  2.0 unx      152 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/scripts/set_db_config.sh
--rw-r--r--  2.0 unx     8081 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/scripts/docker-compose-swarm.yml
--rw-r--r--  2.0 unx      187 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/scripts/prometheus.yml
--rw-r--r--  2.0 unx     5305 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/scripts/stack_deploy_wait.sh
--rwxr-xr-x  2.0 unx      595 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/scripts/apply_dashboard.sh
--rw-r--r--  2.0 unx      453 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/scripts/config_docker.sh
--rw-r--r--  2.0 unx      311 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/scripts/clean_local_storage_deploy.sh
--rw-r--r--  2.0 unx      360 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/scripts/datasource.yml
--rw-r--r--  2.0 unx     1853 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/scripts/alerting/alert_resources.yaml
--rw-r--r--  2.0 unx     5860 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/scripts/alerting/alert_rules.yaml
--rw-r--r--  2.0 unx    98031 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/scripts/dashboards/lvols.json
--rw-r--r--  2.0 unx    98198 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/scripts/dashboards/cluster.json
--rw-r--r--  2.0 unx    98086 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/scripts/dashboards/nodes.json
--rw-r--r--  2.0 unx    98143 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/scripts/dashboards/devices.json
--rw-r--r--  2.0 unx     3203 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/services/caching_node_monitor.py
--rw-r--r--  2.0 unx     4118 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/services/__init__.py
--rw-r--r--  2.0 unx     2423 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/services/port_stat_collector.py
--rw-r--r--  2.0 unx     2189 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/services/lvol_monitor.py
--rw-r--r--  2.0 unx      173 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/services/remove_service.sh
--rw-r--r--  2.0 unx     4637 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/services/distr_event_collector.py
--rw-r--r--  2.0 unx     3003 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/services/mgmt_node_monitor.py
--rw-r--r--  2.0 unx     2410 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/services/log_agg_service.py
--rw-r--r--  2.0 unx      229 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/services/service_template.service
--rw-r--r--  2.0 unx     7218 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/services/capacity_and_stats_collector.py
--rw-r--r--  2.0 unx     2612 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/services/cap_monitor.py
--rw-r--r--  2.0 unx     6360 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/services/storage_node_monitor.py
--rw-r--r--  2.0 unx      837 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/services/install_service.sh
--rw-r--r--  2.0 unx     5462 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/services/health_check_service.py
--rw-r--r--  2.0 unx     2490 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/services/device_monitor.py
--rw-r--r--  2.0 unx     5443 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/services/capacity_collector.py
--rw-r--r--  2.0 unx     4817 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/services/lvol_stat_collector.py
--rw-r--r--  2.0 unx     1500 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/models/events.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/models/__init__.py
--rw-r--r--  2.0 unx     2193 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/models/nvme_device.py
--rw-r--r--  2.0 unx     1228 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/models/global_settings.py
--rw-r--r--  2.0 unx     3766 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/models/caching_node.py
--rw-r--r--  2.0 unx     1020 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/models/port_stat.py
--rw-r--r--  2.0 unx      632 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/models/snapshot.py
--rw-r--r--  2.0 unx      806 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/models/iface.py
--rw-r--r--  2.0 unx     4242 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/models/stats.py
--rw-r--r--  2.0 unx     3222 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/models/storage_node.py
--rw-r--r--  2.0 unx      917 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/models/compute_node.py
--rw-r--r--  2.0 unx     1466 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/models/mgmt_node.py
--rw-r--r--  2.0 unx     1602 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/models/pool.py
--rw-r--r--  2.0 unx     2565 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/models/cluster.py
--rw-r--r--  2.0 unx     4846 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/models/base_model.py
--rw-r--r--  2.0 unx     2479 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/models/lvol_model.py
--rw-r--r--  2.0 unx        0 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/controllers/__init__.py
--rw-r--r--  2.0 unx     1521 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/controllers/storage_events.py
--rw-r--r--  2.0 unx     1900 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/controllers/cluster_events.py
--rw-r--r--  2.0 unx     1961 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/controllers/events_controller.py
--rw-r--r--  2.0 unx    43386 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/controllers/lvol_controller.py
--rw-r--r--  2.0 unx      695 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/controllers/pool_events.py
--rw-r--r--  2.0 unx    22847 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/controllers/caching_node_controller.py
--rw-r--r--  2.0 unx     6389 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/controllers/snapshot_controller.py
--rw-r--r--  2.0 unx     1120 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/controllers/mgmt_events.py
--rw-r--r--  2.0 unx    13528 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/controllers/device_controller.py
--rw-r--r--  2.0 unx     1425 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/controllers/lvol_events.py
--rw-r--r--  2.0 unx     1568 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/controllers/device_events.py
--rw-r--r--  2.0 unx     1123 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/controllers/snapshot_events.py
--rw-r--r--  2.0 unx    11300 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/controllers/health_controller.py
--rw-r--r--  2.0 unx    10375 b- defN 24-Mar-30 16:49 sbcli-mig-1.0.8/simplyblock_core/controllers/pool_controller.py
-144 files, 973295 bytes uncompressed, 149860 bytes compressed:  84.6%
+Zip file size: 177586 bytes, number of entries: 144
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_cli/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/sbcli_mig.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/
+-rw-r--r--  2.0 unx      149 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/env_var
+-rw-r--r--  2.0 unx     2251 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/setup.py
+-rw-r--r--  2.0 unx       38 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/setup.cfg
+-rw-r--r--  2.0 unx      730 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/README.md
+-rw-r--r--  2.0 unx       84 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/pyproject.toml
+-rw-r--r--  2.0 unx     1129 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/PKG-INFO
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/static/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/templates/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/__init__.py
+-rw-r--r--  2.0 unx      717 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/caching_node_app.py
+-rw-r--r--  2.0 unx     2508 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/utils.py
+-rw-r--r--  2.0 unx     1638 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/auth_middleware.py
+-rw-r--r--  2.0 unx      725 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/caching_node_app_k8s.py
+-rw-r--r--  2.0 unx     1263 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/app.py
+-rw-r--r--  2.0 unx     5078 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/node_utils.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/node_webapp.py
+-rw-r--r--  2.0 unx      703 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/snode_app.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/static/deploy_spdk.yaml
+-rw-r--r--  2.0 unx      417 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/static/list_deps.py
+-rw-r--r--  2.0 unx      463 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/static/rpac.yaml
+-rw-r--r--  2.0 unx      827 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/static/delete.py
+-rw-r--r--  2.0 unx      507 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/static/deploy_cnode.yaml
+-rw-r--r--  2.0 unx     1302 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/static/deploy.py
+-rw-r--r--  2.0 unx      434 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/static/is_up.py
+-rw-r--r--  2.0 unx      322 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/static/tst.py
+-rw-r--r--  2.0 unx     1890 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/templates/deploy_spdk.yaml.j2
+-rw-r--r--  2.0 unx     4795 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/node_api_caching_ks.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/__init__.py
+-rw-r--r--  2.0 unx    12129 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/caching_node_ops.py
+-rw-r--r--  2.0 unx     6206 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_pool.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/node_api_basic.py
+-rw-r--r--  2.0 unx      975 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_mgmt_node.py
+-rw-r--r--  2.0 unx     5274 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_cluster.py
+-rw-r--r--  2.0 unx     5317 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_caching_node.py
+-rw-r--r--  2.0 unx     2940 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_device.py
+-rw-r--r--  2.0 unx     6326 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_storage_node.py
+-rw-r--r--  2.0 unx     7846 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/caching_node_ops_k8s.py
+-rw-r--r--  2.0 unx     5547 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/node_api_caching_docker.py
+-rw-r--r--  2.0 unx    11244 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/csi.py
+-rw-r--r--  2.0 unx     8585 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/snode_ops.py
+-rw-r--r--  2.0 unx     8169 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_lvol.py
+-rw-r--r--  2.0 unx      357 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_cli/main.py
+-rw-r--r--  2.0 unx    76175 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_cli/cli.py
+-rw-r--r--  2.0 unx       55 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/sbcli_mig.egg-info/entry_points.txt
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/sbcli_mig.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx       66 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/sbcli_mig.egg-info/requires.txt
+-rw-r--r--  2.0 unx       49 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/sbcli_mig.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     5073 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/sbcli_mig.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx     1129 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/sbcli_mig.egg-info/PKG-INFO
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/
+-rw-r--r--  2.0 unx     3193 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/snode_client.py
+-rw-r--r--  2.0 unx     1426 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/constants.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/__init__.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/cnode_client.py
+-rw-r--r--  2.0 unx     3153 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/mgmt_node_ops.py
+-rw-r--r--  2.0 unx     7626 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/utils.py
+-rw-r--r--  2.0 unx    62998 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/storage_node_ops.py
+-rw-r--r--  2.0 unx      279 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/shell_utils.py
+-rw-r--r--  2.0 unx    24246 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/cluster_ops.py
+-rw-r--r--  2.0 unx      938 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/pci_utils.py
+-rw-r--r--  2.0 unx     6262 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/distr_controller.py
+-rw-r--r--  2.0 unx    21361 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/rpc_client.py
+-rw-r--r--  2.0 unx     8189 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/kv_store.py
+-rw-r--r--  2.0 unx     5112 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/compute_node_ops.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/alerting/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/
+-rw-r--r--  2.0 unx      118 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/db_config_double.sh
+-rw-r--r--  2.0 unx     1163 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/haproxy.cfg
+-rw-r--r--  2.0 unx      694 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/deploy_stack.sh
+-rw-r--r--  2.0 unx       43 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/run_ssh.sh
+-rw-r--r--  2.0 unx     1694 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/__init__.py
+-rw-r--r--  2.0 unx       54 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/db_config_single.sh
+-rw-r--r--  2.0 unx     1420 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/install_deps.sh
+-rw-r--r--  2.0 unx      152 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/set_db_config.sh
+-rw-r--r--  2.0 unx     8081 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/docker-compose-swarm.yml
+-rw-r--r--  2.0 unx      187 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/prometheus.yml
+-rw-r--r--  2.0 unx     5305 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/stack_deploy_wait.sh
+-rwxr-xr-x  2.0 unx      595 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/apply_dashboard.sh
+-rw-r--r--  2.0 unx      453 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/config_docker.sh
+-rw-r--r--  2.0 unx      311 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/clean_local_storage_deploy.sh
+-rw-r--r--  2.0 unx      360 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/datasource.yml
+-rw-r--r--  2.0 unx     1853 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/alerting/alert_resources.yaml
+-rw-r--r--  2.0 unx     5860 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/alerting/alert_rules.yaml
+-rw-r--r--  2.0 unx    98031 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/lvols.json
+-rw-r--r--  2.0 unx    98198 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/cluster.json
+-rw-r--r--  2.0 unx    98086 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/nodes.json
+-rw-r--r--  2.0 unx    98143 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/devices.json
+-rw-r--r--  2.0 unx     3203 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/caching_node_monitor.py
+-rw-r--r--  2.0 unx     4118 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/__init__.py
+-rw-r--r--  2.0 unx     2423 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/port_stat_collector.py
+-rw-r--r--  2.0 unx     2189 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/lvol_monitor.py
+-rw-r--r--  2.0 unx      173 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/remove_service.sh
+-rw-r--r--  2.0 unx     4637 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/distr_event_collector.py
+-rw-r--r--  2.0 unx     3003 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/mgmt_node_monitor.py
+-rw-r--r--  2.0 unx     2410 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/log_agg_service.py
+-rw-r--r--  2.0 unx      229 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/service_template.service
+-rw-r--r--  2.0 unx     7218 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/capacity_and_stats_collector.py
+-rw-r--r--  2.0 unx     2612 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/cap_monitor.py
+-rw-r--r--  2.0 unx     6360 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/storage_node_monitor.py
+-rw-r--r--  2.0 unx      837 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/install_service.sh
+-rw-r--r--  2.0 unx     5462 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/health_check_service.py
+-rw-r--r--  2.0 unx     2490 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/device_monitor.py
+-rw-r--r--  2.0 unx     5443 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/capacity_collector.py
+-rw-r--r--  2.0 unx     4817 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/services/lvol_stat_collector.py
+-rw-r--r--  2.0 unx     1500 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/events.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/__init__.py
+-rw-r--r--  2.0 unx     2193 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/nvme_device.py
+-rw-r--r--  2.0 unx     1228 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/global_settings.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/caching_node.py
+-rw-r--r--  2.0 unx     1020 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/port_stat.py
+-rw-r--r--  2.0 unx      736 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/snapshot.py
+-rw-r--r--  2.0 unx      806 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/iface.py
+-rw-r--r--  2.0 unx     4242 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/stats.py
+-rw-r--r--  2.0 unx     3222 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/storage_node.py
+-rw-r--r--  2.0 unx      917 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/compute_node.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/mgmt_node.py
+-rw-r--r--  2.0 unx     1602 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/pool.py
+-rw-r--r--  2.0 unx     2565 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/cluster.py
+-rw-r--r--  2.0 unx     4846 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/base_model.py
+-rw-r--r--  2.0 unx     2579 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/models/lvol_model.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/__init__.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/storage_events.py
+-rw-r--r--  2.0 unx     1900 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/cluster_events.py
+-rw-r--r--  2.0 unx     1961 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/events_controller.py
+-rw-r--r--  2.0 unx    46469 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/lvol_controller.py
+-rw-r--r--  2.0 unx      695 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/pool_events.py
+-rw-r--r--  2.0 unx    22847 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/caching_node_controller.py
+-rw-r--r--  2.0 unx    10781 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/snapshot_controller.py
+-rw-r--r--  2.0 unx     1120 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/mgmt_events.py
+-rw-r--r--  2.0 unx    13528 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/device_controller.py
+-rw-r--r--  2.0 unx     1425 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/lvol_events.py
+-rw-r--r--  2.0 unx     1568 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/device_events.py
+-rw-r--r--  2.0 unx     1122 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/snapshot_events.py
+-rw-r--r--  2.0 unx    11300 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/health_controller.py
+-rw-r--r--  2.0 unx    10375 b- defN 24-Apr-01 11:58 sbcli-mig-1.0.9/simplyblock_core/controllers/pool_controller.py
+144 files, 983388 bytes uncompressed, 151450 bytes compressed:  84.6%
```

## zipnote {}

```diff
@@ -1,433 +1,433 @@
-Filename: sbcli-mig-1.0.8/
+Filename: sbcli-mig-1.0.9/
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/
+Filename: sbcli-mig-1.0.9/simplyblock_web/
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_cli/
+Filename: sbcli-mig-1.0.9/simplyblock_cli/
 Comment: 
 
-Filename: sbcli-mig-1.0.8/sbcli_mig.egg-info/
+Filename: sbcli-mig-1.0.9/sbcli_mig.egg-info/
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/
+Filename: sbcli-mig-1.0.9/simplyblock_core/
 Comment: 
 
-Filename: sbcli-mig-1.0.8/env_var
+Filename: sbcli-mig-1.0.9/env_var
 Comment: 
 
-Filename: sbcli-mig-1.0.8/setup.py
+Filename: sbcli-mig-1.0.9/setup.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/setup.cfg
+Filename: sbcli-mig-1.0.9/setup.cfg
 Comment: 
 
-Filename: sbcli-mig-1.0.8/README.md
+Filename: sbcli-mig-1.0.9/README.md
 Comment: 
 
-Filename: sbcli-mig-1.0.8/pyproject.toml
+Filename: sbcli-mig-1.0.9/pyproject.toml
 Comment: 
 
-Filename: sbcli-mig-1.0.8/PKG-INFO
+Filename: sbcli-mig-1.0.9/PKG-INFO
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/static/
+Filename: sbcli-mig-1.0.9/simplyblock_web/static/
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/templates/
+Filename: sbcli-mig-1.0.9/simplyblock_web/templates/
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/blueprints/
+Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/__init__.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/__init__.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/caching_node_app.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/caching_node_app.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/utils.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/utils.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/auth_middleware.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/auth_middleware.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/caching_node_app_k8s.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/caching_node_app_k8s.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/app.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/app.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/node_utils.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/node_utils.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/node_webapp.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/node_webapp.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/snode_app.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/snode_app.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/static/deploy_spdk.yaml
+Filename: sbcli-mig-1.0.9/simplyblock_web/static/deploy_spdk.yaml
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/static/list_deps.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/static/list_deps.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/static/rpac.yaml
+Filename: sbcli-mig-1.0.9/simplyblock_web/static/rpac.yaml
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/static/delete.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/static/delete.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/static/deploy_cnode.yaml
+Filename: sbcli-mig-1.0.9/simplyblock_web/static/deploy_cnode.yaml
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/static/deploy.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/static/deploy.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/static/is_up.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/static/is_up.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/static/tst.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/static/tst.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/templates/deploy_spdk.yaml.j2
+Filename: sbcli-mig-1.0.9/simplyblock_web/templates/deploy_spdk.yaml.j2
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/blueprints/node_api_caching_ks.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/node_api_caching_ks.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/blueprints/__init__.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/__init__.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/blueprints/caching_node_ops.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/caching_node_ops.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/blueprints/web_api_pool.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_pool.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/blueprints/node_api_basic.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/node_api_basic.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/blueprints/web_api_mgmt_node.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_mgmt_node.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/blueprints/web_api_cluster.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_cluster.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/blueprints/web_api_caching_node.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_caching_node.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/blueprints/web_api_device.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_device.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/blueprints/web_api_storage_node.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_storage_node.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/blueprints/caching_node_ops_k8s.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/caching_node_ops_k8s.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/blueprints/node_api_caching_docker.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/node_api_caching_docker.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/blueprints/csi.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/csi.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/blueprints/snode_ops.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/snode_ops.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_web/blueprints/web_api_lvol.py
+Filename: sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_lvol.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_cli/main.py
+Filename: sbcli-mig-1.0.9/simplyblock_cli/main.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_cli/cli.py
+Filename: sbcli-mig-1.0.9/simplyblock_cli/cli.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/sbcli_mig.egg-info/entry_points.txt
+Filename: sbcli-mig-1.0.9/sbcli_mig.egg-info/entry_points.txt
 Comment: 
 
-Filename: sbcli-mig-1.0.8/sbcli_mig.egg-info/dependency_links.txt
+Filename: sbcli-mig-1.0.9/sbcli_mig.egg-info/dependency_links.txt
 Comment: 
 
-Filename: sbcli-mig-1.0.8/sbcli_mig.egg-info/requires.txt
+Filename: sbcli-mig-1.0.9/sbcli_mig.egg-info/requires.txt
 Comment: 
 
-Filename: sbcli-mig-1.0.8/sbcli_mig.egg-info/top_level.txt
+Filename: sbcli-mig-1.0.9/sbcli_mig.egg-info/top_level.txt
 Comment: 
 
-Filename: sbcli-mig-1.0.8/sbcli_mig.egg-info/SOURCES.txt
+Filename: sbcli-mig-1.0.9/sbcli_mig.egg-info/SOURCES.txt
 Comment: 
 
-Filename: sbcli-mig-1.0.8/sbcli_mig.egg-info/PKG-INFO
+Filename: sbcli-mig-1.0.9/sbcli_mig.egg-info/PKG-INFO
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/scripts/
+Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/services/
+Filename: sbcli-mig-1.0.9/simplyblock_core/services/
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/models/
+Filename: sbcli-mig-1.0.9/simplyblock_core/models/
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/controllers/
+Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/snode_client.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/snode_client.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/constants.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/constants.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/__init__.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/__init__.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/cnode_client.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/cnode_client.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/mgmt_node_ops.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/mgmt_node_ops.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/utils.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/utils.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/storage_node_ops.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/storage_node_ops.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/shell_utils.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/shell_utils.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/cluster_ops.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/cluster_ops.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/pci_utils.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/pci_utils.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/distr_controller.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/distr_controller.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/rpc_client.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/rpc_client.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/kv_store.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/kv_store.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/compute_node_ops.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/compute_node_ops.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/scripts/alerting/
+Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/alerting/
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/scripts/dashboards/
+Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/scripts/db_config_double.sh
+Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/db_config_double.sh
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/scripts/haproxy.cfg
+Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/haproxy.cfg
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/scripts/deploy_stack.sh
+Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/deploy_stack.sh
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/scripts/run_ssh.sh
+Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/run_ssh.sh
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/scripts/__init__.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/__init__.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/scripts/db_config_single.sh
+Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/db_config_single.sh
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/scripts/install_deps.sh
+Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/install_deps.sh
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/scripts/set_db_config.sh
+Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/set_db_config.sh
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/scripts/docker-compose-swarm.yml
+Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/docker-compose-swarm.yml
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/scripts/prometheus.yml
+Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/prometheus.yml
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/scripts/stack_deploy_wait.sh
+Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/stack_deploy_wait.sh
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/scripts/apply_dashboard.sh
+Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/apply_dashboard.sh
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/scripts/config_docker.sh
+Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/config_docker.sh
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/scripts/clean_local_storage_deploy.sh
+Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/clean_local_storage_deploy.sh
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/scripts/datasource.yml
+Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/datasource.yml
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/scripts/alerting/alert_resources.yaml
+Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/alerting/alert_resources.yaml
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/scripts/alerting/alert_rules.yaml
+Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/alerting/alert_rules.yaml
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/scripts/dashboards/lvols.json
+Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/lvols.json
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/scripts/dashboards/cluster.json
+Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/cluster.json
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/scripts/dashboards/nodes.json
+Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/nodes.json
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/scripts/dashboards/devices.json
+Filename: sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/devices.json
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/services/caching_node_monitor.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/services/caching_node_monitor.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/services/__init__.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/services/__init__.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/services/port_stat_collector.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/services/port_stat_collector.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/services/lvol_monitor.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/services/lvol_monitor.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/services/remove_service.sh
+Filename: sbcli-mig-1.0.9/simplyblock_core/services/remove_service.sh
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/services/distr_event_collector.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/services/distr_event_collector.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/services/mgmt_node_monitor.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/services/mgmt_node_monitor.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/services/log_agg_service.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/services/log_agg_service.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/services/service_template.service
+Filename: sbcli-mig-1.0.9/simplyblock_core/services/service_template.service
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/services/capacity_and_stats_collector.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/services/capacity_and_stats_collector.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/services/cap_monitor.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/services/cap_monitor.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/services/storage_node_monitor.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/services/storage_node_monitor.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/services/install_service.sh
+Filename: sbcli-mig-1.0.9/simplyblock_core/services/install_service.sh
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/services/health_check_service.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/services/health_check_service.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/services/device_monitor.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/services/device_monitor.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/services/capacity_collector.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/services/capacity_collector.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/services/lvol_stat_collector.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/services/lvol_stat_collector.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/models/events.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/models/events.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/models/__init__.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/models/__init__.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/models/nvme_device.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/models/nvme_device.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/models/global_settings.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/models/global_settings.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/models/caching_node.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/models/caching_node.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/models/port_stat.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/models/port_stat.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/models/snapshot.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/models/snapshot.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/models/iface.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/models/iface.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/models/stats.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/models/stats.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/models/storage_node.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/models/storage_node.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/models/compute_node.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/models/compute_node.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/models/mgmt_node.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/models/mgmt_node.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/models/pool.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/models/pool.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/models/cluster.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/models/cluster.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/models/base_model.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/models/base_model.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/models/lvol_model.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/models/lvol_model.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/controllers/__init__.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/__init__.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/controllers/storage_events.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/storage_events.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/controllers/cluster_events.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/cluster_events.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/controllers/events_controller.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/events_controller.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/controllers/lvol_controller.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/lvol_controller.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/controllers/pool_events.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/pool_events.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/controllers/caching_node_controller.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/caching_node_controller.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/controllers/snapshot_controller.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/snapshot_controller.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/controllers/mgmt_events.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/mgmt_events.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/controllers/device_controller.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/device_controller.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/controllers/lvol_events.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/lvol_events.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/controllers/device_events.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/device_events.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/controllers/snapshot_events.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/snapshot_events.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/controllers/health_controller.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/health_controller.py
 Comment: 
 
-Filename: sbcli-mig-1.0.8/simplyblock_core/controllers/pool_controller.py
+Filename: sbcli-mig-1.0.9/simplyblock_core/controllers/pool_controller.py
 Comment: 
 
 Zip file comment:
```

## Comparing `sbcli-mig-1.0.8/setup.py` & `sbcli-mig-1.0.9/setup.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/README.md` & `sbcli-mig-1.0.9/README.md`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/PKG-INFO` & `sbcli-mig-1.0.9/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-mig
-Version: 1.0.8
+Version: 1.0.9
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli-mig-1.0.8/simplyblock_web/caching_node_app.py` & `sbcli-mig-1.0.9/simplyblock_web/caching_node_app.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_web/utils.py` & `sbcli-mig-1.0.9/simplyblock_web/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_web/auth_middleware.py` & `sbcli-mig-1.0.9/simplyblock_web/auth_middleware.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_web/caching_node_app_k8s.py` & `sbcli-mig-1.0.9/simplyblock_web/caching_node_app_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_web/app.py` & `sbcli-mig-1.0.9/simplyblock_web/app.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_web/node_utils.py` & `sbcli-mig-1.0.9/simplyblock_web/node_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_web/node_webapp.py` & `sbcli-mig-1.0.9/simplyblock_web/node_webapp.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_web/snode_app.py` & `sbcli-mig-1.0.9/simplyblock_web/snode_app.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_web/static/deploy_spdk.yaml` & `sbcli-mig-1.0.9/simplyblock_web/static/deploy_spdk.yaml`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_web/static/delete.py` & `sbcli-mig-1.0.9/simplyblock_web/static/delete.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_web/static/deploy.py` & `sbcli-mig-1.0.9/simplyblock_web/static/deploy.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_web/templates/deploy_spdk.yaml.j2` & `sbcli-mig-1.0.9/simplyblock_web/templates/deploy_spdk.yaml.j2`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_web/blueprints/node_api_caching_ks.py` & `sbcli-mig-1.0.9/simplyblock_web/blueprints/node_api_caching_ks.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_web/blueprints/caching_node_ops.py` & `sbcli-mig-1.0.9/simplyblock_web/blueprints/caching_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_web/blueprints/web_api_pool.py` & `sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_pool.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_web/blueprints/node_api_basic.py` & `sbcli-mig-1.0.9/simplyblock_web/blueprints/node_api_basic.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_web/blueprints/web_api_mgmt_node.py` & `sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_web/blueprints/web_api_cluster.py` & `sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_web/blueprints/web_api_caching_node.py` & `sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_web/blueprints/web_api_device.py` & `sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_device.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_web/blueprints/web_api_storage_node.py` & `sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_web/blueprints/caching_node_ops_k8s.py` & `sbcli-mig-1.0.9/simplyblock_web/blueprints/caching_node_ops_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_web/blueprints/node_api_caching_docker.py` & `sbcli-mig-1.0.9/simplyblock_web/blueprints/node_api_caching_docker.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_web/blueprints/csi.py` & `sbcli-mig-1.0.9/simplyblock_web/blueprints/csi.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_web/blueprints/snode_ops.py` & `sbcli-mig-1.0.9/simplyblock_web/blueprints/snode_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_web/blueprints/web_api_lvol.py` & `sbcli-mig-1.0.9/simplyblock_web/blueprints/web_api_lvol.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_cli/cli.py` & `sbcli-mig-1.0.9/simplyblock_cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -429,15 +429,18 @@
         # lvol ops
         subparser = self.add_command('lvol', 'LVol commands')
         # add lvol
         sub_command = self.add_sub_command(subparser, 'add', 'Add a new logical volume')
         sub_command.add_argument("name", help='LVol name or id')
         sub_command.add_argument("size", help='LVol size: 10M, 10G, 10(bytes)')
         sub_command.add_argument("pool", help='Pool UUID or name')
-        sub_command.add_argument("--host_id", help='Primary storage node UUID or Hostname')
+        sub_command.add_argument("--snapshot", "-s", help='Make LVol with snapshot capability, default is False',
+                                 required=False, action='store_true')
+        sub_command.add_argument("--max-size", help='LVol max size', dest='max_size', default="0")
+        sub_command.add_argument("--host-id", help='Primary storage node UUID or Hostname', dest='host_id')
         sub_command.add_argument("--ha-type", help='LVol HA type (single, ha), default is cluster HA type',
                                  dest='ha_type', choices=["single", "ha", "default"], default='default')
 
         sub_command.add_argument("--compress",
                                  help='Use inline data compression and de-compression on the logical volume',
                                  required=False, action='store_true')
         sub_command.add_argument("--encrypt", help='Use inline data encryption and de-cryption on the logical volume',
@@ -471,14 +474,18 @@
         sub_command.add_argument("--max-r-mbytes", help='Maximum Read Mega Bytes Per Second', type=int)
         sub_command.add_argument("--max-w-mbytes", help='Maximum Write Mega Bytes Per Second', type=int)
 
         # list lvols
         sub_command = self.add_sub_command(subparser, 'list', 'List all LVols')
         sub_command.add_argument("--cluster-id", help='List LVols in particular cluster')
         sub_command.add_argument("--json", help='Print outputs in json format', required=False, action='store_true')
+        # list lvols
+        sub_command = self.add_sub_command(subparser, 'list-mem', 'List all LVols')
+        sub_command.add_argument("--json", help='Print outputs in json format', required=False, action='store_true')
+        sub_command.add_argument("--csv", help='Print outputs in csv format', required=False, action='store_true')
         # get lvol
         sub_command = self.add_sub_command(subparser, 'get', 'Get LVol details')
         sub_command.add_argument("id", help='LVol id or name')
         sub_command.add_argument("--json", help='Print outputs in json format', required=False, action='store_true')
         # delete lvol
         sub_command = self.add_sub_command(
             subparser, 'delete', 'Delete LVol. This is only possible, if no more snapshots and non-inflated clones '
@@ -1038,45 +1045,51 @@
                 self.parser.print_help()
 
         elif args.command == 'lvol':
             sub_command = args_dict[args.command]
             if sub_command == "add":
                 name = args.name
                 size = self.parse_size(args.size)
+                max_size = self.parse_size(args.max_size)
                 host_id = args.host_id
                 ha_type = args.ha_type
                 pool = args.pool
                 comp = args.compress
                 crypto = args.encrypt
                 distr_vuid = args.distr_vuid
                 distr_ndcs = args.distr_ndcs
                 distr_npcs = args.distr_npcs
                 distr_bs = args.distr_bs
                 distr_chunk_bs = args.distr_chunk_bs
+                with_snapshot = args.snapshot
                 results, error = lvol_controller.add_lvol_ha(
                     name, size, host_id, ha_type, pool, comp, crypto,
                     distr_vuid, distr_ndcs, distr_npcs,
                     args.max_rw_iops,
                     args.max_rw_mbytes,
                     args.max_r_mbytes,
                     args.max_w_mbytes,
                     distr_bs,
-                    distr_chunk_bs)
+                    distr_chunk_bs,
+                    with_snapshot=with_snapshot,
+                    max_size=max_size)
                 if results:
                     ret = results
                 else:
                     ret = error
             elif sub_command == "add-distr":
                 pass
             elif sub_command == "qos-set":
                 ret = lvol_controller.set_lvol(
                     args.id, args.max_rw_iops, args.max_rw_mbytes,
                     args.max_r_mbytes, args.max_w_mbytes)
             elif sub_command == "list":
                 ret = lvol_controller.list_lvols(args.json)
+            elif sub_command == "list-mem":
+                ret = lvol_controller.list_lvols_mem(args.json, args.csv)
             elif sub_command == "get":
                 ret = lvol_controller.get_lvol(args.id, args.json)
             elif sub_command == "delete":
                 for id in args.id:
                     force = args.force
                     ret = lvol_controller.delete_lvol(id, force)
             elif sub_command == "connect":
```

## Comparing `sbcli-mig-1.0.8/sbcli_mig.egg-info/SOURCES.txt` & `sbcli-mig-1.0.9/sbcli_mig.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/sbcli_mig.egg-info/PKG-INFO` & `sbcli-mig-1.0.9/sbcli_mig.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-mig
-Version: 1.0.8
+Version: 1.0.9
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli-mig-1.0.8/simplyblock_core/snode_client.py` & `sbcli-mig-1.0.9/simplyblock_core/snode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/constants.py` & `sbcli-mig-1.0.9/simplyblock_core/constants.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/cnode_client.py` & `sbcli-mig-1.0.9/simplyblock_core/cnode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/mgmt_node_ops.py` & `sbcli-mig-1.0.9/simplyblock_core/mgmt_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/utils.py` & `sbcli-mig-1.0.9/simplyblock_core/utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,7 +272,11 @@
     elif len(records) == 1:
         return records[0]
     else:
         total = records[0]
         for rec in records[1:]:
             total += rec
         return total
+
+
+def get_random_vuid():
+    return 1 + int(random.random() * 10000)
```

## Comparing `sbcli-mig-1.0.8/simplyblock_core/storage_node_ops.py` & `sbcli-mig-1.0.9/simplyblock_core/storage_node_ops.py`

 * *Files 0% similar despite different names*

```diff
@@ -267,15 +267,15 @@
         ret = rpc_client.nvmf_subsystem_add_ns(subsystem_nqn, pt_name)
         if not ret:
             logger.error(f"Failed to add: {pt_name} to the subsystem: {subsystem_nqn}")
             return False
 
         # create jm
         if nvme.jm_bdev:
-            ret = rpc_client.bdev_jm_create(nvme.jm_bdev, nvme.alceml_bdev)
+            ret = rpc_client.bdev_jm_create(nvme.jm_bdev, alceml_name)
             if not ret:
                 logger.error(f"Failed to create JM bdev: {snode.nvme_devices[0].jm_bdev}")
                 return False
 
         nvme.testing_bdev = test_name
         nvme.alceml_bdev = alceml_name
         nvme.pt_bdev = pt_name
```

## Comparing `sbcli-mig-1.0.8/simplyblock_core/cluster_ops.py` & `sbcli-mig-1.0.9/simplyblock_core/cluster_ops.py`

 * *Files 5% similar despite different names*

```diff
@@ -41,14 +41,39 @@
     }
     session = requests.session()
     session.auth = ("admin", password)
     response = session.request("POST", url, headers=headers, data=payload)
     logger.debug(response.text)
     return response.status_code == 201
 
+def _add_graylog_input_tcp(cluster_ip, password):
+    url = f"http://{cluster_ip}:9000/api/system/inputs"
+    payload = json.dumps({
+        "title": "spdk log input",
+        "type": "org.graylog2.inputs.gelf.tcp.GELFTCPInput",
+        "configuration": {
+            "bind_address": "0.0.0.0",
+            "port": 12201,
+            "recv_buffer_size": 262144,
+            "number_worker_threads": 2,
+            "override_source": None,
+            "charset_name": "UTF-8",
+            "decompress_size_limit": 8388608
+        },
+        "global": True
+    })
+    headers = {
+        'X-Requested-By': '',
+        'Content-Type': 'application/json',
+    }
+    session = requests.session()
+    session.auth = ("admin", password)
+    response = session.request("POST", url, headers=headers, data=payload)
+    logger.debug(response.text)
+    return response.status_code == 201
 
 def create_cluster(blk_size, page_size_in_blocks, ha_type, tls,
                    auth_hosts_only, cli_pass, model_ids,
                    cap_warn, cap_crit, prov_cap_warn, prov_cap_crit, ifname):
     logger.info("Installing dependencies...")
     ret = scripts.install_deps()
     logger.info("Installing dependencies > Done")
@@ -112,14 +137,15 @@
     logger.info("Deploying swarm stack > Done")
 
     logger.info("Configuring DB...")
     out = scripts.set_db_config_single()
     logger.info("Configuring DB > Done")
 
     _add_graylog_input(DEV_IP, c.secret)
+    _add_graylog_input_tcp(DEV_IP, c.secret)
 
     c.status = Cluster.STATUS_ACTIVE
     if ha_type == 'ha':
         c.status = Cluster.STATUS_SUSPENDED
     c.updated_at = int(time.time())
     c.write_to_db(db_controller.kv_store)
```

## Comparing `sbcli-mig-1.0.8/simplyblock_core/pci_utils.py` & `sbcli-mig-1.0.9/simplyblock_core/pci_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/distr_controller.py` & `sbcli-mig-1.0.9/simplyblock_core/distr_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/rpc_client.py` & `sbcli-mig-1.0.9/simplyblock_core/rpc_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -594,19 +594,25 @@
         return self._request("ultra21_lvol_mount", params)
 
     def ultra21_lvol_mount_lvol(self, lvol_name, base_bdev, label, desc):
         params = {
             "modus": "BASE",
             "lvol_bdev": lvol_name,
             "base_bdev": base_bdev,
-            "label": label,
-            "desc": desc
+            # "label": label,
+            # "desc": desc
         }
         return self._request("ultra21_lvol_mount", params)
 
+    def ultra21_lvol_dismount(self, lvol_name):
+        params = {
+            "lvol_bdev": lvol_name
+        }
+        return self._request("ultra21_lvol_dismount", params)
+
     def bdev_jm_create(self, name, name_storage1, block_size=4096):
         params = {
             "name": name,
             "name_storage1": name_storage1,
             "block_size": block_size
         }
         return self._request("bdev_jm_create", params)
@@ -615,14 +621,23 @@
         params = {"name": name}
         return self._request("bdev_jm_delete", params)
 
     def ultra21_util_get_malloc_stats(self):
         params = {"socket_id": 0}
         return self._request("ultra21_util_get_malloc_stats", params)
 
+    def ultra21_lvol_mount_clone(self, clone_name, snap_bdev, base_bdev):
+        params = {
+            "modus": "CLONE",
+            "lvol_bdev": clone_name,
+            "base_bdev": base_bdev,
+            "snapshot_bdev": snap_bdev
+        }
+        return self._request("ultra21_lvol_mount", params)
+
     def alceml_unmap_vuid(self, name, vuid):
         params = {"name": name, "vuid": vuid}
         return self._request("alceml_unmap_vuid", params)
 
     def jm_delete(self):
         params = {"name": 0, "vuid": 0}
         return self._request("jm_delete", params)
```

## Comparing `sbcli-mig-1.0.8/simplyblock_core/kv_store.py` & `sbcli-mig-1.0.9/simplyblock_core/kv_store.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/compute_node_ops.py` & `sbcli-mig-1.0.9/simplyblock_core/compute_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/scripts/haproxy.cfg` & `sbcli-mig-1.0.9/simplyblock_core/scripts/haproxy.cfg`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/scripts/deploy_stack.sh` & `sbcli-mig-1.0.9/simplyblock_core/scripts/deploy_stack.sh`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/scripts/__init__.py` & `sbcli-mig-1.0.9/simplyblock_core/scripts/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/scripts/install_deps.sh` & `sbcli-mig-1.0.9/simplyblock_core/scripts/install_deps.sh`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/scripts/docker-compose-swarm.yml` & `sbcli-mig-1.0.9/simplyblock_core/scripts/docker-compose-swarm.yml`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/scripts/stack_deploy_wait.sh` & `sbcli-mig-1.0.9/simplyblock_core/scripts/stack_deploy_wait.sh`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/scripts/apply_dashboard.sh` & `sbcli-mig-1.0.9/simplyblock_core/scripts/apply_dashboard.sh`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/scripts/alerting/alert_resources.yaml` & `sbcli-mig-1.0.9/simplyblock_core/scripts/alerting/alert_resources.yaml`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/scripts/alerting/alert_rules.yaml` & `sbcli-mig-1.0.9/simplyblock_core/scripts/alerting/alert_rules.yaml`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/scripts/dashboards/lvols.json` & `sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/lvols.json`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/scripts/dashboards/cluster.json` & `sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/cluster.json`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/scripts/dashboards/nodes.json` & `sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/nodes.json`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/scripts/dashboards/devices.json` & `sbcli-mig-1.0.9/simplyblock_core/scripts/dashboards/devices.json`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/services/caching_node_monitor.py` & `sbcli-mig-1.0.9/simplyblock_core/services/caching_node_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 
 
 from simplyblock_core import constants, kv_store
 from simplyblock_core.rpc_client import RPCClient
 from simplyblock_core.models.caching_node import CachingNode
 
 # Import the GELF logger
-from graypy import GELFUDPHandler
+from graypy import GELFTCPHandler
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
-gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
+gelf_handler = GELFTCPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 
 # get DB controller
```

## Comparing `sbcli-mig-1.0.8/simplyblock_core/services/__init__.py` & `sbcli-mig-1.0.9/simplyblock_core/services/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/services/port_stat_collector.py` & `sbcli-mig-1.0.9/simplyblock_core/services/port_stat_collector.py`

 * *Files 4% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 import psutil
 
 
 from simplyblock_core import constants, kv_store, utils
 from simplyblock_core.models.port_stat import PortStat
 
 # Import the GELF logger
-from graypy import GELFUDPHandler
+from graypy import GELFTCPHandler
 
 def update_port_stats(snode, nic, stats):
     now = int(time.time())
     data = {
         "uuid": nic.get_id(),
         "node_id": snode.get_id(),
         "date": now,
@@ -39,15 +39,15 @@
     stat_obj.write_to_db(db_controller.kv_store)
     return
 
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
-gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
+gelf_handler = GELFTCPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_controller = kv_store.DBController()
```

## Comparing `sbcli-mig-1.0.8/simplyblock_core/services/lvol_monitor.py` & `sbcli-mig-1.0.9/simplyblock_core/services/lvol_monitor.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 from datetime import datetime
 
 from simplyblock_core import constants, kv_store
 from simplyblock_core.models.lvol_model import LVol
 from simplyblock_core.controllers import health_controller, lvol_events
 
 # Import the GELF logger
-from graypy import GELFUDPHandler
+from graypy import GELFTCPHandler
 
 def set_lvol_status(lvol, status):
     if lvol.status != status:
         lvol = db_controller.get_lvol_by_id(lvol.get_id())
         old_status = lvol.status
         lvol.status = status
         lvol.write_to_db(db_store)
@@ -32,15 +32,15 @@
     lvol.write_to_db(db_store)
     lvol_events.lvol_health_check_change(lvol, lvol.health_check, old_status, caused_by="monitor")
 
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
-gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
+gelf_handler = GELFTCPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_store = kv_store.KVStore()
```

## Comparing `sbcli-mig-1.0.8/simplyblock_core/services/distr_event_collector.py` & `sbcli-mig-1.0.9/simplyblock_core/services/distr_event_collector.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 
 
 from simplyblock_core import constants, kv_store, utils, rpc_client
 from simplyblock_core.controllers import events_controller, device_controller, lvol_events
 from simplyblock_core.models.lvol_model import LVol
 
 # Import the GELF logger
-from graypy import GELFUDPHandler
+from graypy import GELFTCPHandler
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
-gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
+gelf_handler = GELFTCPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_controller = kv_store.DBController()
```

## Comparing `sbcli-mig-1.0.8/simplyblock_core/services/mgmt_node_monitor.py` & `sbcli-mig-1.0.9/simplyblock_core/services/mgmt_node_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,20 +8,20 @@
 
 
 from simplyblock_core import constants, kv_store, utils
 from simplyblock_core.controllers import mgmt_events
 from simplyblock_core.models.mgmt_node import MgmtNode
 
 # Import the GELF logger
-from graypy import GELFUDPHandler
+from graypy import GELFTCPHandler
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
-gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
+gelf_handler = GELFTCPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 
 # get DB controller
```

## Comparing `sbcli-mig-1.0.8/simplyblock_core/services/log_agg_service.py` & `sbcli-mig-1.0.9/simplyblock_core/services/log_agg_service.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,20 +5,20 @@
 import time
 import sys
 
 from simplyblock_core import constants, kv_store, utils
 from simplyblock_core.models.stats import DeviceStatObject, NodeStatObject, ClusterStatObject
 
 # Import the GELF logger
-from graypy import GELFUDPHandler
+from graypy import GELFTCPHandler
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
-gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
+gelf_handler = GELFTCPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_controller = kv_store.DBController()
```

## Comparing `sbcli-mig-1.0.8/simplyblock_core/services/capacity_and_stats_collector.py` & `sbcli-mig-1.0.9/simplyblock_core/services/capacity_and_stats_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 import sys
 
 from simplyblock_core import constants, kv_store, utils
 from simplyblock_core.rpc_client import RPCClient
 from simplyblock_core.models.stats import DeviceStatObject, NodeStatObject, ClusterStatObject
 
 # Import the GELF logger
-from graypy import GELFUDPHandler
+from graypy import GELFTCPHandler
 
 last_object_record = {}
 
 
 def add_device_stats(cl, device, capacity_dict, stats_dict):
     now = int(time.time())
     data = {
@@ -147,15 +147,15 @@
     stat_obj.write_to_db(db_controller.kv_store)
     return stat_obj
 
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
-gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
+gelf_handler = GELFTCPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_controller = kv_store.DBController()
```

## Comparing `sbcli-mig-1.0.8/simplyblock_core/services/cap_monitor.py` & `sbcli-mig-1.0.9/simplyblock_core/services/cap_monitor.py`

 * *Files 5% similar despite different names*

```diff
@@ -7,20 +7,20 @@
 
 
 from simplyblock_core import kv_store, constants, cluster_ops
 from simplyblock_core.controllers import cluster_events
 from simplyblock_core.models.cluster import Cluster
 
 # Import the GELF logger
-from graypy import GELFUDPHandler
+from graypy import GELFTCPHandler
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
-gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
+gelf_handler = GELFTCPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_controller = kv_store.DBController()
```

## Comparing `sbcli-mig-1.0.8/simplyblock_core/services/storage_node_monitor.py` & `sbcli-mig-1.0.9/simplyblock_core/services/storage_node_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,20 +10,20 @@
 from simplyblock_core import constants, kv_store, cluster_ops
 from simplyblock_core.controllers import storage_events, health_controller
 from simplyblock_core.models.cluster import Cluster
 from simplyblock_core.models.nvme_device import NVMeDevice
 from simplyblock_core.models.storage_node import StorageNode
 
 # Import the GELF logger
-from graypy import GELFUDPHandler
+from graypy import GELFTCPHandler
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
-gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
+gelf_handler = GELFTCPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 
 # get DB controller
```

## Comparing `sbcli-mig-1.0.8/simplyblock_core/services/install_service.sh` & `sbcli-mig-1.0.9/simplyblock_core/services/install_service.sh`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/services/health_check_service.py` & `sbcli-mig-1.0.9/simplyblock_core/services/health_check_service.py`

 * *Files 0% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from simplyblock_core.controllers import health_controller, storage_events, device_events
 from simplyblock_core.models.storage_node import StorageNode
 from simplyblock_core.rpc_client import RPCClient
 from simplyblock_core import constants, kv_store
 
 # Import the GELF logger
-from graypy import GELFUDPHandler
+from graypy import GELFTCPHandler
 
 def set_node_health_check(snode, health_check_status):
     snode = db_controller.get_storage_node_by_id(snode.get_id())
     if snode.health_check == health_check_status:
         return
     old_status = snode.health_check
     snode.health_check = health_check_status
@@ -39,15 +39,15 @@
                     device_events.device_health_check_change(
                         dev, dev.health_check, old_status, caused_by="monitor")
 
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
-gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
+gelf_handler = GELFTCPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_store = kv_store.KVStore()
```

## Comparing `sbcli-mig-1.0.8/simplyblock_core/services/device_monitor.py` & `sbcli-mig-1.0.9/simplyblock_core/services/device_monitor.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 from simplyblock_core import constants, kv_store, storage_node_ops
 from simplyblock_core.controllers import health_controller,  device_controller
 from simplyblock_core.models.nvme_device import NVMeDevice
 from simplyblock_core.models.storage_node import StorageNode
 
 # Import the GELF logger
-from graypy import GELFUDPHandler
+from graypy import GELFTCPHandler
 
 def set_dev_status(device, status):
     node = db_controller.get_storage_node_by_id(device.node_id)
     if node.status != StorageNode.STATUS_ONLINE:
         logger.error(f"Node is not online, {node.get_id()}, status: {node.status}, "
                      f"skipping device status change")
         return
@@ -28,15 +28,15 @@
             break
     return
 
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
-gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
+gelf_handler = GELFTCPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_store = kv_store.KVStore()
```

## Comparing `sbcli-mig-1.0.8/simplyblock_core/services/capacity_collector.py` & `sbcli-mig-1.0.9/simplyblock_core/services/capacity_collector.py`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import uuid
 
 from simplyblock_core import constants, kv_store
 from simplyblock_core.rpc_client import RPCClient
 from simplyblock_core.models.stats import CapacityStat
 
 # Import the GELF logger
-from graypy import GELFUDPHandler
+from graypy import GELFTCPHandler
 
 def add_cluster_stats(cl, records):
 
     if not records:
         return False
 
     size_total = 0
@@ -129,15 +129,15 @@
 
     return stat_obj
 
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
-gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
+gelf_handler = GELFTCPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_controller = kv_store.DBController()
```

## Comparing `sbcli-mig-1.0.8/simplyblock_core/services/lvol_stat_collector.py` & `sbcli-mig-1.0.9/simplyblock_core/services/lvol_stat_collector.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 
 from simplyblock_core import constants, kv_store, utils
 from simplyblock_core.models.stats import LVolStatObject, PoolStatObject
 from simplyblock_core.rpc_client import RPCClient
 
 # Import the GELF logger
-from graypy import GELFUDPHandler
+from graypy import GELFTCPHandler
 
 last_object_record = {}
 
 
 def add_lvol_stats(pool, lvol, stats_dict):
     now = int(time.time())
     data = {
@@ -88,15 +88,15 @@
     stat_obj.write_to_db(db_controller.kv_store)
     return stat_obj
 
 
 # configure logging
 logger_handler = logging.StreamHandler(stream=sys.stdout)
 logger_handler.setFormatter(logging.Formatter('%(asctime)s: %(levelname)s: %(message)s'))
-gelf_handler = GELFUDPHandler('0.0.0.0', constants.GELF_PORT)
+gelf_handler = GELFTCPHandler('0.0.0.0', constants.GELF_PORT)
 logger = logging.getLogger()
 logger.addHandler(gelf_handler)
 logger.addHandler(logger_handler)
 logger.setLevel(logging.DEBUG)
 
 # get DB controller
 db_store = kv_store.KVStore()
```

## Comparing `sbcli-mig-1.0.8/simplyblock_core/models/events.py` & `sbcli-mig-1.0.9/simplyblock_core/models/events.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/models/nvme_device.py` & `sbcli-mig-1.0.9/simplyblock_core/models/nvme_device.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/models/global_settings.py` & `sbcli-mig-1.0.9/simplyblock_core/models/global_settings.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/models/caching_node.py` & `sbcli-mig-1.0.9/simplyblock_core/models/caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/models/port_stat.py` & `sbcli-mig-1.0.9/simplyblock_core/models/port_stat.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/models/snapshot.py` & `sbcli-mig-1.0.9/simplyblock_core/models/snapshot.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,18 +3,20 @@
 from simplyblock_core.models.base_model import BaseModel
 from simplyblock_core.models.lvol_model import LVol
 
 
 class SnapShot(BaseModel):
     attributes = {
         "uuid": {"type": str, 'default': ""},
-        "snap_name": {"type": str, 'default': 0},
-        "snap_bdev": {"type": str, 'default': 0},
+        "snap_name": {"type": str, 'default': ""},
+        "base_bdev": {"type": str, 'default': ""},
+        "snap_bdev": {"type": str, 'default': ""},
         "lvol": {"type": LVol, 'default': None},
         "created_at": {"type": int, 'default': 0},
+        "mem_diff": {"type": dict, 'default': {}},
     }
 
     def __init__(self, data=None):
         super(SnapShot, self).__init__()
         self.set_attrs(self.attributes, data)
         self.object_type = "object"
```

## Comparing `sbcli-mig-1.0.8/simplyblock_core/models/iface.py` & `sbcli-mig-1.0.9/simplyblock_core/models/iface.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/models/stats.py` & `sbcli-mig-1.0.9/simplyblock_core/models/stats.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/models/storage_node.py` & `sbcli-mig-1.0.9/simplyblock_core/models/storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/models/compute_node.py` & `sbcli-mig-1.0.9/simplyblock_core/models/compute_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/models/mgmt_node.py` & `sbcli-mig-1.0.9/simplyblock_core/models/mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/models/pool.py` & `sbcli-mig-1.0.9/simplyblock_core/models/pool.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/models/cluster.py` & `sbcli-mig-1.0.9/simplyblock_core/models/cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/models/base_model.py` & `sbcli-mig-1.0.9/simplyblock_core/models/base_model.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/models/lvol_model.py` & `sbcli-mig-1.0.9/simplyblock_core/models/lvol_model.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
     STATUS_ONLINE = 'online'
     STATUS_OFFLINE = 'offline'
     STATUS_IN_DELETION = 'in_deletion'
 
     attributes = {
         "lvol_name": {"type": str, 'default': ""},
         "size": {"type": int, 'default': 0},
+        "max_size": {"type": int, 'default': 0},
         "uuid": {"type": str, 'default': ""},
         "guid": {"type": str, 'default': ""},
         "ha_type": {"type": str, 'default': ""},
         "status": {"type": str, 'default': ""},
 
         "base_bdev": {"type": str, 'default': ""},
         "lvol_bdev": {"type": str, 'default': ""},
@@ -53,14 +54,15 @@
         "distr_bs": {"type": int, 'default': 0},
         "distr_chunk_bs": {"type": int, 'default': 0},
         "distr_page_size": {"type": int, 'default': 0},
 
         "health_check": {"type": bool, "default": True},
 
         "snapshot_name": {"type": str, 'default': ""},
+        "mem_diff": {"type": dict, 'default': {}},
         "io_error": {"type": bool, 'default': False},
 
         "deletion_status": {"type": str, 'default': ""},
 
     }
 
     def __init__(self, data=None):
```

## Comparing `sbcli-mig-1.0.8/simplyblock_core/controllers/storage_events.py` & `sbcli-mig-1.0.9/simplyblock_core/controllers/storage_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/controllers/cluster_events.py` & `sbcli-mig-1.0.9/simplyblock_core/controllers/cluster_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/controllers/events_controller.py` & `sbcli-mig-1.0.9/simplyblock_core/controllers/events_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/controllers/lvol_controller.py` & `sbcli-mig-1.0.9/simplyblock_core/controllers/lvol_controller.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import sys
 import time
 import uuid
 
 from simplyblock_core import utils, constants, distr_controller
 from simplyblock_core.controllers import snapshot_controller, pool_controller, lvol_events
 from simplyblock_core.kv_store import DBController
+from simplyblock_core.models.cluster import Cluster
 from simplyblock_core.models.nvme_device import NVMeDevice
 from simplyblock_core.models.pool import Pool
 from simplyblock_core.models.lvol_model import LVol
 from simplyblock_core.models.storage_node import StorageNode
 from simplyblock_core.rpc_client import RPCClient
 
 
@@ -431,15 +432,15 @@
     else:
         return online_nodes
 
 
 def add_lvol_ha(name, size, host_id_or_name, ha_type, pool_id_or_name, use_comp, use_crypto,
                 distr_vuid, distr_ndcs, distr_npcs,
                 max_rw_iops, max_rw_mbytes, max_r_mbytes, max_w_mbytes,
-                distr_bs=None, distr_chunk_bs=None):
+                distr_bs=None, distr_chunk_bs=None, with_snapshot=False, max_size=0):
 
     logger.info(f"Adding LVol: {name}")
     host_node = None
     if host_id_or_name:
         host_node = db_controller.get_storage_node_by_id(host_id_or_name)
         if not host_node:
             host_node = db_controller.get_storage_node_by_hostname(host_id_or_name)
@@ -514,15 +515,15 @@
         logger.error(msg)
         return False, msg
 
     elif cl.prov_cap_warn and cl.prov_cap_warn < cluster_size_prov_util:
         logger.warning(f"Cluster provisioned cap warning, util: {cluster_size_prov_util}% of cluster util: {cl.prov_cap_warn}")
 
     if distr_vuid == 0:
-        vuid = 1 + int(random.random() * 10000)
+        vuid = utils.get_random_vuid()
     else:
         vuid = distr_vuid
 
     if distr_ndcs == 0 and distr_npcs == 0:
         if ha_type == "single":
             distr_ndcs = 4
             distr_npcs = 1
@@ -535,17 +536,29 @@
             elif dev_count >= 6:
                 distr_ndcs = 4
             distr_npcs = 1
     else:
         if distr_ndcs + distr_npcs >= dev_count:
             return False, f"ndcs+npcs: {distr_ndcs+distr_npcs} must be less than online devices count: {dev_count}"
 
+    if max_size:
+        if max_size < size:
+            return False, f"Max size:{max_size} must be larger than size {size}"
+    else:
+        records = db_controller.get_cluster_capacity(cl)
+        if records:
+            max_size = records[0]['size_total']
+        else:
+            max_size = size * 10
+
+    logger.info(f"Max size: {utils.humanbytes(max_size)}")
     lvol = LVol()
     lvol.lvol_name = name
     lvol.size = size
+    lvol.max_size = max_size
     lvol.status = LVol.STATUS_ONLINE
     lvol.ha_type = ha_type
     lvol.bdev_stack = []
     lvol.uuid = str(uuid.uuid4())
     lvol.guid = _generate_hex_string(16)
     lvol.vuid = vuid
     lvol.lvol_bdev = f"LVS_{vuid}/{name}"
@@ -564,28 +577,53 @@
     lvol.distr_chunk_bs = distr_chunk_bs
     lvol.distr_page_size = cl.page_size_in_blocks
 
     lvol.base_bdev = f"distr_{lvol.vuid}_{name}"
     lvol.top_bdev = lvol.base_bdev
 
     lvol.bdev_stack.append({
-        "type": "distr",
+        "type": "bdev_distr",
         "name": lvol.base_bdev,
         "params": {
             "name": lvol.base_bdev,
             "vuid": lvol.vuid,
             "ndcs": lvol.ndcs,
             "npcs": lvol.npcs,
             "num_blocks": int(lvol.size / lvol.distr_bs),
             "block_size": lvol.distr_bs,
             "chunk_size": lvol.distr_chunk_bs,
             "pba_page_size":  lvol.distr_page_size,
         }
     })
 
+    if with_snapshot:
+        lvol.bdev_stack.append({
+            "type": "bmap_init",
+            "name": lvol.base_bdev,
+            "params": {
+                "bdev_name": lvol.base_bdev,
+                "num_blocks": int(lvol.size / lvol.distr_bs),
+                "block_len": lvol.distr_bs,
+                "page_len": int(lvol.distr_page_size / lvol.distr_bs),
+                "max_num_blocks": int(lvol.max_size / lvol.distr_bs)
+            }
+        })
+        lvol.snapshot_name = f"snapshot_{lvol.vuid}_{name}"
+        lvol.top_bdev = f"lvol_{lvol.vuid}_{lvol.lvol_name}"
+        lvol.bdev_stack.append({
+            "type": "ultra_lvol",
+            "name": lvol.top_bdev,
+            "params": {
+                "lvol_name": lvol.top_bdev,
+                "base_bdev": lvol.base_bdev,
+                "label": "label",
+                "desc": "desc"
+            }
+        })
+
     if use_crypto is True:
         lvol.crypto_bdev = f"crypto_{lvol.lvol_name}"
         lvol.bdev_stack.append({
             "type": "crypto",
             "name": lvol.crypto_bdev,
             "params": {
                 "name": lvol.crypto_bdev,
@@ -655,30 +693,42 @@
     if max_rw_iops or max_rw_mbytes or max_r_mbytes or max_w_mbytes:
         set_lvol(lvol.uuid, max_rw_iops, max_rw_mbytes, max_r_mbytes, max_w_mbytes)
     return lvol.uuid, None
 
 
 def _create_bdev_stack(lvol, snode, ha_comm_addrs, ha_inode_self):
     rpc_client = RPCClient(snode.mgmt_ip, snode.rpc_port, snode.rpc_username, snode.rpc_password)
+
     created_bdevs = []
     for bdev in lvol.bdev_stack:
         # if 'status' in bdev and bdev['status'] == 'created':
         #     continue
 
         type = bdev['type']
         name = bdev['name']
         params = bdev['params']
         ret = None
 
-        if type == "distr":
+        if type == "bdev_distr":
             params['jm_names'] = get_jm_names(snode)
             params['ha_comm_addrs'] = ha_comm_addrs
             params['ha_inode_self'] = ha_inode_self
             ret = rpc_client.bdev_distrib_create(**params)
 
+            snodes = db_controller.get_storage_nodes()
+            cluster_map_data = distr_controller.get_distr_cluster_map(snodes, snode)
+            cluster_map_data['UUID_node_target'] = snode.get_id()
+            rpc_client.distr_send_cluster_map(cluster_map_data)
+
+        elif type == "bmap_init":
+            ret = rpc_client.ultra21_lvol_bmap_init(**params)
+
+        elif type == "ultra_lvol":
+            ret = rpc_client.ultra21_lvol_mount_lvol(**params)
+
         elif type == "crypto":
             ret = _create_crypto_lvol(rpc_client, **params)
 
         elif type == "comp":
             ret = _create_compress_lvol(rpc_client, **params)
 
         else:
@@ -694,20 +744,21 @@
                 _remove_bdev_stack(created_bdevs, rpc_client)
             return False, f"Failed to create BDev: {name}"
 
     return True, None
 
 
 def add_lvol_on_node(lvol, snode, ha_comm_addrs=None, ha_inode_self=None):
+    rpc_client = RPCClient(snode.mgmt_ip, snode.rpc_port, snode.rpc_username, snode.rpc_password)
+    spdk_mem_info_before = rpc_client.ultra21_util_get_malloc_stats()
 
     ret, msg = _create_bdev_stack(lvol, snode, ha_comm_addrs, ha_inode_self)
     if not ret:
         return False, msg
 
-    rpc_client = RPCClient(snode.mgmt_ip, snode.rpc_port, snode.rpc_username, snode.rpc_password)
     logger.info("creating subsystem %s", lvol.nqn)
     ret = rpc_client.subsystem_create(lvol.nqn, 'sbcli-cn', lvol.uuid)
     logger.debug(ret)
 
     # add listeners
     logger.info("adding listeners")
     for iface in snode.data_nics:
@@ -737,14 +788,26 @@
 
     logger.info("Sending cluster map to LVol")
     snodes = db_controller.get_storage_nodes()
     cluster_map_data = distr_controller.get_distr_cluster_map(snodes, snode)
     cluster_map_data['UUID_node_target'] = snode.get_id()
     ret = rpc_client.distr_send_cluster_map(cluster_map_data)
 
+    spdk_mem_info_after = rpc_client.ultra21_util_get_malloc_stats()
+    logger.debug("ultra21_util_get_malloc_stats:")
+    logger.debug(spdk_mem_info_after)
+
+    diff = {}
+    for key in spdk_mem_info_after.keys():
+        diff[key] = spdk_mem_info_after[key] - spdk_mem_info_before[key]
+
+    logger.info("spdk mem diff:")
+    logger.info(json.dumps(diff, indent=2))
+    lvol.mem_diff = diff
+
     return True, None
 
 
 def recreate_lvol(lvol_id, snode):
     lvol = db_controller.get_lvol_by_id(lvol_id)
     if not lvol:
         logger.error(f"lvol not found: {lvol_id}")
@@ -778,33 +841,37 @@
             continue
 
         type = bdev['type']
         name = bdev['name']
         ret = None
         # if type == "alceml":
         #     ret = rpc_client.bdev_alceml_delete(name)
-        if type == "distr":
+        if type == "bdev_distr":
             ret = rpc_client.bdev_distrib_delete(name)
         # elif type == "lvs":
         #     ret = rpc_client.bdev_lvol_delete_lvstore(name)
         # elif type == "lvol":
         #     ret = rpc_client.delete_lvol(name)
         # elif type == "ultra_pt":
         #     ret = rpc_client.ultra21_bdev_pass_delete(name)
+        elif type == "ultra_lvol":
+            ret = rpc_client.ultra21_lvol_dismount(name)
         elif type == "comp":
             ret = rpc_client.lvol_compress_delete(name)
         elif type == "crypto":
             ret = rpc_client.lvol_crypto_delete(name)
         else:
             logger.debug(f"Unknown BDev type: {type}")
+            continue
 
         if not ret:
             logger.error(f"Failed to delete BDev {name}")
 
         bdev['status'] = 'deleted'
+        time.sleep(1)
 
 
 def delete_lvol_from_node(lvol, node_id):
     snode = db_controller.get_storage_node_by_id(node_id)
     logger.debug(f"Deleting LVol:{lvol.get_id()} from node:{snode.get_id()}")
     rpc_client = RPCClient(snode.mgmt_ip, snode.rpc_port, snode.rpc_username, snode.rpc_password)
 
@@ -978,14 +1045,38 @@
 
     if is_json:
         return json.dumps(data, indent=2)
     else:
         return utils.print_table(data)
 
 
+def list_lvols_mem(is_json, is_csv):
+    lvols = db_controller.get_lvols()
+    data = []
+    for lvol in lvols:
+        if lvol.deleted is True:
+            continue
+        logger.debug(lvol)
+        data.append({
+            "id": lvol.uuid,
+            "size": utils.humanbytes(lvol.size),
+            "max_size": utils.humanbytes(lvol.max_size),
+            **lvol.mem_diff
+        })
+
+    if is_json:
+        return json.dumps(data, indent=2)
+    elif is_csv:
+        print(";".join(data[0].keys()))
+        for d in data:
+            print(";".join([str(v) for v in d.values()]))
+    else:
+        return utils.print_table(data)
+
+
 def get_lvol(lvol_id_or_name, is_json):
     lvol = None
     for lv in db_controller.get_lvols():
         if lv.get_id() == lvol_id_or_name or lv.lvol_name == lvol_id_or_name:
             lvol = lv
             break
```

## Comparing `sbcli-mig-1.0.8/simplyblock_core/controllers/pool_events.py` & `sbcli-mig-1.0.9/simplyblock_core/controllers/pool_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/controllers/caching_node_controller.py` & `sbcli-mig-1.0.9/simplyblock_core/controllers/caching_node_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/controllers/mgmt_events.py` & `sbcli-mig-1.0.9/simplyblock_core/controllers/mgmt_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/controllers/device_controller.py` & `sbcli-mig-1.0.9/simplyblock_core/controllers/device_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/controllers/lvol_events.py` & `sbcli-mig-1.0.9/simplyblock_core/controllers/lvol_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/controllers/device_events.py` & `sbcli-mig-1.0.9/simplyblock_core/controllers/device_events.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/controllers/snapshot_events.py` & `sbcli-mig-1.0.9/simplyblock_core/controllers/snapshot_events.py`

 * *Files 18% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 from simplyblock_core.kv_store import DBController
 
 logger = logging.getLogger()
 db_controller = DBController()
 
 
 def _snapshot_event(snapshot, message, caused_by, event):
-    snode = db_controller.get_storage_node_by_id(snapshot.lvol.hostname)
+    snode = db_controller.get_storage_node_by_id(snapshot.lvol.node_id)
     ec.log_event_cluster(
         cluster_id=snode.cluster_id,
         domain=ec.DOMAIN_CLUSTER,
         event=event,
         db_object=snapshot,
         caused_by=caused_by,
         message=message,
```

## Comparing `sbcli-mig-1.0.8/simplyblock_core/controllers/health_controller.py` & `sbcli-mig-1.0.9/simplyblock_core/controllers/health_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli-mig-1.0.8/simplyblock_core/controllers/pool_controller.py` & `sbcli-mig-1.0.9/simplyblock_core/controllers/pool_controller.py`

 * *Files identical despite different names*

