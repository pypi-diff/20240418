# Comparing `tmp/sbcli_dev-2.2.3.zip` & `tmp/sbcli_dev-2.2.4.zip`

## zipinfo {}

```diff
@@ -1,146 +1,146 @@
-Zip file size: 178315 bytes, number of entries: 144
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 13:18 sbcli_dev-2.2.3/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_cli/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 13:18 sbcli_dev-2.2.3/sbcli_dev.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/
--rw-r--r--  2.0 unx     2251 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/setup.py
--rw-r--r--  2.0 unx      730 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/README.md
--rw-r--r--  2.0 unx      148 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/env_var
--rw-r--r--  2.0 unx       84 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/pyproject.toml
--rw-r--r--  2.0 unx       38 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/setup.cfg
--rw-r--r--  2.0 unx     1129 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/PKG-INFO
--rw-r--r--  2.0 unx    76437 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_cli/cli.py
--rw-r--r--  2.0 unx      357 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_cli/main.py
--rw-r--r--  2.0 unx        1 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/sbcli_dev.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     5073 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/sbcli_dev.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       49 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/sbcli_dev.egg-info/top_level.txt
--rw-r--r--  2.0 unx     1129 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/sbcli_dev.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       66 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/sbcli_dev.egg-info/requires.txt
--rw-r--r--  2.0 unx       55 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/sbcli_dev.egg-info/entry_points.txt
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/services/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/scripts/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/controllers/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/models/
--rw-r--r--  2.0 unx    62031 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/storage_node_ops.py
--rw-r--r--  2.0 unx     1440 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/constants.py
--rw-r--r--  2.0 unx     3153 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/mgmt_node_ops.py
--rw-r--r--  2.0 unx     3444 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/cnode_client.py
--rw-r--r--  2.0 unx      279 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/shell_utils.py
--rw-r--r--  2.0 unx      938 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/pci_utils.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/__init__.py
--rw-r--r--  2.0 unx     3193 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/snode_client.py
--rw-r--r--  2.0 unx     8189 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/kv_store.py
--rw-r--r--  2.0 unx     7640 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/utils.py
--rw-r--r--  2.0 unx    23335 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/cluster_ops.py
--rw-r--r--  2.0 unx     5112 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/compute_node_ops.py
--rw-r--r--  2.0 unx    21428 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/rpc_client.py
--rw-r--r--  2.0 unx     7387 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/distr_controller.py
--rw-r--r--  2.0 unx     2189 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/services/lvol_monitor.py
--rw-r--r--  2.0 unx     3203 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/services/caching_node_monitor.py
--rw-r--r--  2.0 unx     5443 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/services/capacity_collector.py
--rw-r--r--  2.0 unx     5462 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/services/health_check_service.py
--rw-r--r--  2.0 unx      229 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/services/service_template.service
--rw-r--r--  2.0 unx     4817 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/services/lvol_stat_collector.py
--rw-r--r--  2.0 unx      173 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/services/remove_service.sh
--rw-r--r--  2.0 unx     2410 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/services/log_agg_service.py
--rw-r--r--  2.0 unx     5034 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/services/distr_event_collector.py
--rw-r--r--  2.0 unx     7439 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/services/capacity_and_stats_collector.py
--rw-r--r--  2.0 unx     2423 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/services/port_stat_collector.py
--rw-r--r--  2.0 unx     2490 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/services/device_monitor.py
--rw-r--r--  2.0 unx     4118 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/services/__init__.py
--rw-r--r--  2.0 unx      837 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/services/install_service.sh
--rw-r--r--  2.0 unx     3003 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/services/mgmt_node_monitor.py
--rw-r--r--  2.0 unx     2671 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/services/cap_monitor.py
--rw-r--r--  2.0 unx     6577 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/services/storage_node_monitor.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/scripts/alerting/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/scripts/dashboards/
--rw-r--r--  2.0 unx      694 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/scripts/deploy_stack.sh
--rw-r--r--  2.0 unx      152 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/scripts/set_db_config.sh
--rw-r--r--  2.0 unx     1163 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/scripts/haproxy.cfg
--rw-r--r--  2.0 unx     8081 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/scripts/docker-compose-swarm.yml
--rw-r--r--  2.0 unx       54 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/scripts/db_config_single.sh
--rw-r--r--  2.0 unx     5305 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/scripts/stack_deploy_wait.sh
--rw-r--r--  2.0 unx      453 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/scripts/config_docker.sh
--rw-r--r--  2.0 unx     1694 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/scripts/__init__.py
--rw-r--r--  2.0 unx      311 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/scripts/clean_local_storage_deploy.sh
--rw-r--r--  2.0 unx      118 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/scripts/db_config_double.sh
--rw-r--r--  2.0 unx      360 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/scripts/datasource.yml
--rw-r--r--  2.0 unx       43 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/scripts/run_ssh.sh
--rw-r--r--  2.0 unx     1420 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/scripts/install_deps.sh
--rw-r--r--  2.0 unx      187 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/scripts/prometheus.yml
--rwxr-xr-x  2.0 unx      595 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/scripts/apply_dashboard.sh
--rw-r--r--  2.0 unx     5860 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/scripts/alerting/alert_rules.yaml
--rw-r--r--  2.0 unx     1853 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/scripts/alerting/alert_resources.yaml
--rw-r--r--  2.0 unx    98143 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/scripts/dashboards/devices.json
--rw-r--r--  2.0 unx    98086 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/scripts/dashboards/nodes.json
--rw-r--r--  2.0 unx    98031 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/scripts/dashboards/lvols.json
--rw-r--r--  2.0 unx    98198 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/scripts/dashboards/cluster.json
--rw-r--r--  2.0 unx    13535 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/controllers/device_controller.py
--rw-r--r--  2.0 unx     1120 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/controllers/mgmt_events.py
--rw-r--r--  2.0 unx     1961 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/controllers/events_controller.py
--rw-r--r--  2.0 unx     1521 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/controllers/storage_events.py
--rw-r--r--  2.0 unx     1427 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/controllers/lvol_events.py
--rw-r--r--  2.0 unx    10557 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/controllers/snapshot_controller.py
--rw-r--r--  2.0 unx     1568 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/controllers/device_events.py
--rw-r--r--  2.0 unx    10375 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/controllers/pool_controller.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/controllers/__init__.py
--rw-r--r--  2.0 unx     1900 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/controllers/cluster_events.py
--rw-r--r--  2.0 unx    22847 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/controllers/caching_node_controller.py
--rw-r--r--  2.0 unx     1122 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/controllers/snapshot_events.py
--rw-r--r--  2.0 unx    46084 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/controllers/lvol_controller.py
--rw-r--r--  2.0 unx    11294 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/controllers/health_controller.py
--rw-r--r--  2.0 unx      695 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/controllers/pool_events.py
--rw-r--r--  2.0 unx     1500 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/models/events.py
--rw-r--r--  2.0 unx      806 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/models/iface.py
--rw-r--r--  2.0 unx     4846 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/models/base_model.py
--rw-r--r--  2.0 unx     2579 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/models/lvol_model.py
--rw-r--r--  2.0 unx      917 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/models/compute_node.py
--rw-r--r--  2.0 unx      736 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/models/snapshot.py
--rw-r--r--  2.0 unx     1602 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/models/pool.py
--rw-r--r--  2.0 unx     1228 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/models/global_settings.py
--rw-r--r--  2.0 unx     1020 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/models/port_stat.py
--rw-r--r--  2.0 unx     3252 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/models/storage_node.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/models/__init__.py
--rw-r--r--  2.0 unx     4242 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/models/stats.py
--rw-r--r--  2.0 unx     2565 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/models/cluster.py
--rw-r--r--  2.0 unx     1466 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/models/mgmt_node.py
--rw-r--r--  2.0 unx     3766 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/models/caching_node.py
--rw-r--r--  2.0 unx     2071 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_core/models/nvme_device.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/static/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/templates/
-drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/blueprints/
--rw-r--r--  2.0 unx      725 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/caching_node_app_k8s.py
--rw-r--r--  2.0 unx     5098 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/node_utils.py
--rw-r--r--  2.0 unx      703 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/snode_app.py
--rw-r--r--  2.0 unx     1263 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/app.py
--rw-r--r--  2.0 unx     1638 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/auth_middleware.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/__init__.py
--rw-r--r--  2.0 unx      717 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/caching_node_app.py
--rw-r--r--  2.0 unx     2508 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/utils.py
--rw-r--r--  2.0 unx     1434 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/node_webapp.py
--rw-r--r--  2.0 unx      507 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/static/deploy_cnode.yaml
--rw-r--r--  2.0 unx      322 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/static/tst.py
--rw-r--r--  2.0 unx      434 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/static/is_up.py
--rw-r--r--  2.0 unx      827 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/static/delete.py
--rw-r--r--  2.0 unx     1302 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/static/deploy.py
--rw-r--r--  2.0 unx     1466 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/static/deploy_spdk.yaml
--rw-r--r--  2.0 unx      463 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/static/rpac.yaml
--rw-r--r--  2.0 unx      417 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/static/list_deps.py
--rw-r--r--  2.0 unx     2876 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/templates/deploy_spdk.yaml.j2
--rw-r--r--  2.0 unx     5547 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/blueprints/node_api_caching_docker.py
--rw-r--r--  2.0 unx     4795 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/blueprints/node_api_caching_ks.py
--rw-r--r--  2.0 unx     5317 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/blueprints/web_api_caching_node.py
--rw-r--r--  2.0 unx     8654 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/blueprints/snode_ops.py
--rw-r--r--  2.0 unx     8169 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/blueprints/web_api_lvol.py
--rw-r--r--  2.0 unx    11244 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/blueprints/csi.py
--rw-r--r--  2.0 unx    12198 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/blueprints/caching_node_ops.py
--rw-r--r--  2.0 unx      975 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/blueprints/web_api_mgmt_node.py
--rw-r--r--  2.0 unx     6326 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/blueprints/web_api_storage_node.py
--rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/blueprints/__init__.py
--rw-r--r--  2.0 unx     7846 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/blueprints/caching_node_ops_k8s.py
--rw-r--r--  2.0 unx     2940 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/blueprints/web_api_device.py
--rw-r--r--  2.0 unx     5274 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/blueprints/web_api_cluster.py
--rw-r--r--  2.0 unx     3103 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/blueprints/node_api_basic.py
--rw-r--r--  2.0 unx     6206 b- defN 24-Apr-18 13:18 sbcli_dev-2.2.3/simplyblock_web/blueprints/web_api_pool.py
-144 files, 984331 bytes uncompressed, 152179 bytes compressed:  84.5%
+Zip file size: 178923 bytes, number of entries: 144
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 16:22 sbcli_dev-2.2.4/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_cli/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 16:22 sbcli_dev-2.2.4/sbcli_dev.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/
+-rw-r--r--  2.0 unx     2251 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/setup.py
+-rw-r--r--  2.0 unx      740 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/README.md
+-rw-r--r--  2.0 unx      148 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/env_var
+-rw-r--r--  2.0 unx       84 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/pyproject.toml
+-rw-r--r--  2.0 unx       38 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/setup.cfg
+-rw-r--r--  2.0 unx     1139 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/PKG-INFO
+-rw-r--r--  2.0 unx    76893 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_cli/cli.py
+-rw-r--r--  2.0 unx      357 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_cli/main.py
+-rw-r--r--  2.0 unx        1 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/sbcli_dev.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     5073 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/sbcli_dev.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       49 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/sbcli_dev.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     1139 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/sbcli_dev.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       66 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/sbcli_dev.egg-info/requires.txt
+-rw-r--r--  2.0 unx       55 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/sbcli_dev.egg-info/entry_points.txt
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/services/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/scripts/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/controllers/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/models/
+-rw-r--r--  2.0 unx    62388 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/storage_node_ops.py
+-rw-r--r--  2.0 unx     1440 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/constants.py
+-rw-r--r--  2.0 unx     3153 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/mgmt_node_ops.py
+-rw-r--r--  2.0 unx     3444 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/cnode_client.py
+-rw-r--r--  2.0 unx      279 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/shell_utils.py
+-rw-r--r--  2.0 unx      938 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/pci_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/__init__.py
+-rw-r--r--  2.0 unx     3193 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/snode_client.py
+-rw-r--r--  2.0 unx     8189 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/kv_store.py
+-rw-r--r--  2.0 unx     7640 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/utils.py
+-rw-r--r--  2.0 unx    23335 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/cluster_ops.py
+-rw-r--r--  2.0 unx     5112 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/compute_node_ops.py
+-rw-r--r--  2.0 unx    21493 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/rpc_client.py
+-rw-r--r--  2.0 unx     7387 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/distr_controller.py
+-rw-r--r--  2.0 unx     2189 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/services/lvol_monitor.py
+-rw-r--r--  2.0 unx     3203 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/services/caching_node_monitor.py
+-rw-r--r--  2.0 unx     5443 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/services/capacity_collector.py
+-rw-r--r--  2.0 unx     5462 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/services/health_check_service.py
+-rw-r--r--  2.0 unx      229 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/services/service_template.service
+-rw-r--r--  2.0 unx     4817 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/services/lvol_stat_collector.py
+-rw-r--r--  2.0 unx      173 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/services/remove_service.sh
+-rw-r--r--  2.0 unx     2410 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/services/log_agg_service.py
+-rw-r--r--  2.0 unx     5034 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/services/distr_event_collector.py
+-rw-r--r--  2.0 unx     7439 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/services/capacity_and_stats_collector.py
+-rw-r--r--  2.0 unx     2423 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/services/port_stat_collector.py
+-rw-r--r--  2.0 unx     2490 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/services/device_monitor.py
+-rw-r--r--  2.0 unx     4118 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/services/__init__.py
+-rw-r--r--  2.0 unx      837 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/services/install_service.sh
+-rw-r--r--  2.0 unx     3003 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/services/mgmt_node_monitor.py
+-rw-r--r--  2.0 unx     2671 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/services/cap_monitor.py
+-rw-r--r--  2.0 unx     6577 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/services/storage_node_monitor.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/scripts/alerting/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/scripts/dashboards/
+-rw-r--r--  2.0 unx      694 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/scripts/deploy_stack.sh
+-rw-r--r--  2.0 unx      152 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/scripts/set_db_config.sh
+-rw-r--r--  2.0 unx     1163 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/scripts/haproxy.cfg
+-rw-r--r--  2.0 unx     8081 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/scripts/docker-compose-swarm.yml
+-rw-r--r--  2.0 unx       54 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/scripts/db_config_single.sh
+-rw-r--r--  2.0 unx     5305 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/scripts/stack_deploy_wait.sh
+-rw-r--r--  2.0 unx      453 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/scripts/config_docker.sh
+-rw-r--r--  2.0 unx     1694 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/scripts/__init__.py
+-rw-r--r--  2.0 unx      311 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/scripts/clean_local_storage_deploy.sh
+-rw-r--r--  2.0 unx      118 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/scripts/db_config_double.sh
+-rw-r--r--  2.0 unx      360 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/scripts/datasource.yml
+-rw-r--r--  2.0 unx       43 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/scripts/run_ssh.sh
+-rw-r--r--  2.0 unx     1420 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/scripts/install_deps.sh
+-rw-r--r--  2.0 unx      187 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/scripts/prometheus.yml
+-rwxr-xr-x  2.0 unx      595 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/scripts/apply_dashboard.sh
+-rw-r--r--  2.0 unx     5860 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/scripts/alerting/alert_rules.yaml
+-rw-r--r--  2.0 unx     1853 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/scripts/alerting/alert_resources.yaml
+-rw-r--r--  2.0 unx    98143 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/scripts/dashboards/devices.json
+-rw-r--r--  2.0 unx    98086 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/scripts/dashboards/nodes.json
+-rw-r--r--  2.0 unx    98031 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/scripts/dashboards/lvols.json
+-rw-r--r--  2.0 unx    98198 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/scripts/dashboards/cluster.json
+-rw-r--r--  2.0 unx    13535 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/controllers/device_controller.py
+-rw-r--r--  2.0 unx     1120 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/controllers/mgmt_events.py
+-rw-r--r--  2.0 unx     1961 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/controllers/events_controller.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/controllers/storage_events.py
+-rw-r--r--  2.0 unx     1427 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/controllers/lvol_events.py
+-rw-r--r--  2.0 unx    10557 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/controllers/snapshot_controller.py
+-rw-r--r--  2.0 unx     1568 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/controllers/device_events.py
+-rw-r--r--  2.0 unx    10375 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/controllers/pool_controller.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/controllers/__init__.py
+-rw-r--r--  2.0 unx     1900 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/controllers/cluster_events.py
+-rw-r--r--  2.0 unx    22847 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/controllers/caching_node_controller.py
+-rw-r--r--  2.0 unx     1122 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/controllers/snapshot_events.py
+-rw-r--r--  2.0 unx    47314 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/controllers/lvol_controller.py
+-rw-r--r--  2.0 unx    11294 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/controllers/health_controller.py
+-rw-r--r--  2.0 unx      695 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/controllers/pool_events.py
+-rw-r--r--  2.0 unx     1500 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/models/events.py
+-rw-r--r--  2.0 unx      806 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/models/iface.py
+-rw-r--r--  2.0 unx     4846 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/models/base_model.py
+-rw-r--r--  2.0 unx     2579 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/models/lvol_model.py
+-rw-r--r--  2.0 unx      917 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/models/compute_node.py
+-rw-r--r--  2.0 unx      736 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/models/snapshot.py
+-rw-r--r--  2.0 unx     1602 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/models/pool.py
+-rw-r--r--  2.0 unx     1228 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/models/global_settings.py
+-rw-r--r--  2.0 unx     1020 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/models/port_stat.py
+-rw-r--r--  2.0 unx     3252 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/models/storage_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/models/__init__.py
+-rw-r--r--  2.0 unx     4242 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/models/stats.py
+-rw-r--r--  2.0 unx     2565 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/models/cluster.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/models/mgmt_node.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/models/caching_node.py
+-rw-r--r--  2.0 unx     2071 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_core/models/nvme_device.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/static/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/templates/
+drwxr-xr-x  2.0 unx        0 b- stor 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/blueprints/
+-rw-r--r--  2.0 unx      725 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/caching_node_app_k8s.py
+-rw-r--r--  2.0 unx     5098 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/node_utils.py
+-rw-r--r--  2.0 unx      703 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/snode_app.py
+-rw-r--r--  2.0 unx     1263 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/app.py
+-rw-r--r--  2.0 unx     1638 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/auth_middleware.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/__init__.py
+-rw-r--r--  2.0 unx      717 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/caching_node_app.py
+-rw-r--r--  2.0 unx     2508 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/utils.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/node_webapp.py
+-rw-r--r--  2.0 unx      507 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/static/deploy_cnode.yaml
+-rw-r--r--  2.0 unx      322 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/static/tst.py
+-rw-r--r--  2.0 unx      434 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/static/is_up.py
+-rw-r--r--  2.0 unx      827 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/static/delete.py
+-rw-r--r--  2.0 unx     1302 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/static/deploy.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/static/deploy_spdk.yaml
+-rw-r--r--  2.0 unx      463 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/static/rpac.yaml
+-rw-r--r--  2.0 unx      417 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/static/list_deps.py
+-rw-r--r--  2.0 unx     2876 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/templates/deploy_spdk.yaml.j2
+-rw-r--r--  2.0 unx     5547 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/blueprints/node_api_caching_docker.py
+-rw-r--r--  2.0 unx     4795 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/blueprints/node_api_caching_ks.py
+-rw-r--r--  2.0 unx     5317 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/blueprints/web_api_caching_node.py
+-rw-r--r--  2.0 unx     8654 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/blueprints/snode_ops.py
+-rw-r--r--  2.0 unx     8547 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/blueprints/web_api_lvol.py
+-rw-r--r--  2.0 unx    11244 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/blueprints/csi.py
+-rw-r--r--  2.0 unx    12198 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/blueprints/caching_node_ops.py
+-rw-r--r--  2.0 unx      975 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/blueprints/web_api_mgmt_node.py
+-rw-r--r--  2.0 unx     6326 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/blueprints/web_api_storage_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/blueprints/__init__.py
+-rw-r--r--  2.0 unx     7846 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/blueprints/caching_node_ops_k8s.py
+-rw-r--r--  2.0 unx     2940 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/blueprints/web_api_device.py
+-rw-r--r--  2.0 unx     5274 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/blueprints/web_api_cluster.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/blueprints/node_api_basic.py
+-rw-r--r--  2.0 unx     6206 b- defN 24-Apr-18 16:22 sbcli_dev-2.2.4/simplyblock_web/blueprints/web_api_pool.py
+144 files, 986847 bytes uncompressed, 152787 bytes compressed:  84.5%
```

## zipnote {}

```diff
@@ -1,433 +1,433 @@
-Filename: sbcli_dev-2.2.3/
+Filename: sbcli_dev-2.2.4/
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_cli/
+Filename: sbcli_dev-2.2.4/simplyblock_cli/
 Comment: 
 
-Filename: sbcli_dev-2.2.3/sbcli_dev.egg-info/
+Filename: sbcli_dev-2.2.4/sbcli_dev.egg-info/
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/
+Filename: sbcli_dev-2.2.4/simplyblock_core/
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/
+Filename: sbcli_dev-2.2.4/simplyblock_web/
 Comment: 
 
-Filename: sbcli_dev-2.2.3/setup.py
+Filename: sbcli_dev-2.2.4/setup.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/README.md
+Filename: sbcli_dev-2.2.4/README.md
 Comment: 
 
-Filename: sbcli_dev-2.2.3/env_var
+Filename: sbcli_dev-2.2.4/env_var
 Comment: 
 
-Filename: sbcli_dev-2.2.3/pyproject.toml
+Filename: sbcli_dev-2.2.4/pyproject.toml
 Comment: 
 
-Filename: sbcli_dev-2.2.3/setup.cfg
+Filename: sbcli_dev-2.2.4/setup.cfg
 Comment: 
 
-Filename: sbcli_dev-2.2.3/PKG-INFO
+Filename: sbcli_dev-2.2.4/PKG-INFO
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_cli/cli.py
+Filename: sbcli_dev-2.2.4/simplyblock_cli/cli.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_cli/main.py
+Filename: sbcli_dev-2.2.4/simplyblock_cli/main.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/sbcli_dev.egg-info/dependency_links.txt
+Filename: sbcli_dev-2.2.4/sbcli_dev.egg-info/dependency_links.txt
 Comment: 
 
-Filename: sbcli_dev-2.2.3/sbcli_dev.egg-info/SOURCES.txt
+Filename: sbcli_dev-2.2.4/sbcli_dev.egg-info/SOURCES.txt
 Comment: 
 
-Filename: sbcli_dev-2.2.3/sbcli_dev.egg-info/top_level.txt
+Filename: sbcli_dev-2.2.4/sbcli_dev.egg-info/top_level.txt
 Comment: 
 
-Filename: sbcli_dev-2.2.3/sbcli_dev.egg-info/PKG-INFO
+Filename: sbcli_dev-2.2.4/sbcli_dev.egg-info/PKG-INFO
 Comment: 
 
-Filename: sbcli_dev-2.2.3/sbcli_dev.egg-info/requires.txt
+Filename: sbcli_dev-2.2.4/sbcli_dev.egg-info/requires.txt
 Comment: 
 
-Filename: sbcli_dev-2.2.3/sbcli_dev.egg-info/entry_points.txt
+Filename: sbcli_dev-2.2.4/sbcli_dev.egg-info/entry_points.txt
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/services/
+Filename: sbcli_dev-2.2.4/simplyblock_core/services/
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/scripts/
+Filename: sbcli_dev-2.2.4/simplyblock_core/scripts/
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/controllers/
+Filename: sbcli_dev-2.2.4/simplyblock_core/controllers/
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/models/
+Filename: sbcli_dev-2.2.4/simplyblock_core/models/
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/storage_node_ops.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/storage_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/constants.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/constants.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/mgmt_node_ops.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/mgmt_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/cnode_client.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/cnode_client.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/shell_utils.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/shell_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/pci_utils.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/pci_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/__init__.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/snode_client.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/snode_client.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/kv_store.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/kv_store.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/utils.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/utils.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/cluster_ops.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/cluster_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/compute_node_ops.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/compute_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/rpc_client.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/rpc_client.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/distr_controller.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/distr_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/services/lvol_monitor.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/services/lvol_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/services/caching_node_monitor.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/services/caching_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/services/capacity_collector.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/services/capacity_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/services/health_check_service.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/services/health_check_service.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/services/service_template.service
+Filename: sbcli_dev-2.2.4/simplyblock_core/services/service_template.service
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/services/lvol_stat_collector.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/services/lvol_stat_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/services/remove_service.sh
+Filename: sbcli_dev-2.2.4/simplyblock_core/services/remove_service.sh
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/services/log_agg_service.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/services/log_agg_service.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/services/distr_event_collector.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/services/distr_event_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/services/capacity_and_stats_collector.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/services/capacity_and_stats_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/services/port_stat_collector.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/services/port_stat_collector.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/services/device_monitor.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/services/device_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/services/__init__.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/services/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/services/install_service.sh
+Filename: sbcli_dev-2.2.4/simplyblock_core/services/install_service.sh
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/services/mgmt_node_monitor.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/services/mgmt_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/services/cap_monitor.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/services/cap_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/services/storage_node_monitor.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/services/storage_node_monitor.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/scripts/alerting/
+Filename: sbcli_dev-2.2.4/simplyblock_core/scripts/alerting/
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/scripts/dashboards/
+Filename: sbcli_dev-2.2.4/simplyblock_core/scripts/dashboards/
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/scripts/deploy_stack.sh
+Filename: sbcli_dev-2.2.4/simplyblock_core/scripts/deploy_stack.sh
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/scripts/set_db_config.sh
+Filename: sbcli_dev-2.2.4/simplyblock_core/scripts/set_db_config.sh
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/scripts/haproxy.cfg
+Filename: sbcli_dev-2.2.4/simplyblock_core/scripts/haproxy.cfg
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/scripts/docker-compose-swarm.yml
+Filename: sbcli_dev-2.2.4/simplyblock_core/scripts/docker-compose-swarm.yml
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/scripts/db_config_single.sh
+Filename: sbcli_dev-2.2.4/simplyblock_core/scripts/db_config_single.sh
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/scripts/stack_deploy_wait.sh
+Filename: sbcli_dev-2.2.4/simplyblock_core/scripts/stack_deploy_wait.sh
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/scripts/config_docker.sh
+Filename: sbcli_dev-2.2.4/simplyblock_core/scripts/config_docker.sh
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/scripts/__init__.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/scripts/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/scripts/clean_local_storage_deploy.sh
+Filename: sbcli_dev-2.2.4/simplyblock_core/scripts/clean_local_storage_deploy.sh
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/scripts/db_config_double.sh
+Filename: sbcli_dev-2.2.4/simplyblock_core/scripts/db_config_double.sh
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/scripts/datasource.yml
+Filename: sbcli_dev-2.2.4/simplyblock_core/scripts/datasource.yml
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/scripts/run_ssh.sh
+Filename: sbcli_dev-2.2.4/simplyblock_core/scripts/run_ssh.sh
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/scripts/install_deps.sh
+Filename: sbcli_dev-2.2.4/simplyblock_core/scripts/install_deps.sh
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/scripts/prometheus.yml
+Filename: sbcli_dev-2.2.4/simplyblock_core/scripts/prometheus.yml
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/scripts/apply_dashboard.sh
+Filename: sbcli_dev-2.2.4/simplyblock_core/scripts/apply_dashboard.sh
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/scripts/alerting/alert_rules.yaml
+Filename: sbcli_dev-2.2.4/simplyblock_core/scripts/alerting/alert_rules.yaml
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/scripts/alerting/alert_resources.yaml
+Filename: sbcli_dev-2.2.4/simplyblock_core/scripts/alerting/alert_resources.yaml
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/scripts/dashboards/devices.json
+Filename: sbcli_dev-2.2.4/simplyblock_core/scripts/dashboards/devices.json
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/scripts/dashboards/nodes.json
+Filename: sbcli_dev-2.2.4/simplyblock_core/scripts/dashboards/nodes.json
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/scripts/dashboards/lvols.json
+Filename: sbcli_dev-2.2.4/simplyblock_core/scripts/dashboards/lvols.json
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/scripts/dashboards/cluster.json
+Filename: sbcli_dev-2.2.4/simplyblock_core/scripts/dashboards/cluster.json
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/controllers/device_controller.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/controllers/device_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/controllers/mgmt_events.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/controllers/mgmt_events.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/controllers/events_controller.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/controllers/events_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/controllers/storage_events.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/controllers/storage_events.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/controllers/lvol_events.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/controllers/lvol_events.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/controllers/snapshot_controller.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/controllers/snapshot_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/controllers/device_events.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/controllers/device_events.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/controllers/pool_controller.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/controllers/pool_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/controllers/__init__.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/controllers/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/controllers/cluster_events.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/controllers/cluster_events.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/controllers/caching_node_controller.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/controllers/caching_node_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/controllers/snapshot_events.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/controllers/snapshot_events.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/controllers/lvol_controller.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/controllers/lvol_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/controllers/health_controller.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/controllers/health_controller.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/controllers/pool_events.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/controllers/pool_events.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/models/events.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/models/events.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/models/iface.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/models/iface.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/models/base_model.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/models/base_model.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/models/lvol_model.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/models/lvol_model.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/models/compute_node.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/models/compute_node.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/models/snapshot.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/models/snapshot.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/models/pool.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/models/pool.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/models/global_settings.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/models/global_settings.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/models/port_stat.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/models/port_stat.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/models/storage_node.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/models/storage_node.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/models/__init__.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/models/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/models/stats.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/models/stats.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/models/cluster.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/models/cluster.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/models/mgmt_node.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/models/mgmt_node.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/models/caching_node.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/models/caching_node.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_core/models/nvme_device.py
+Filename: sbcli_dev-2.2.4/simplyblock_core/models/nvme_device.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/static/
+Filename: sbcli_dev-2.2.4/simplyblock_web/static/
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/templates/
+Filename: sbcli_dev-2.2.4/simplyblock_web/templates/
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/blueprints/
+Filename: sbcli_dev-2.2.4/simplyblock_web/blueprints/
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/caching_node_app_k8s.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/caching_node_app_k8s.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/node_utils.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/node_utils.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/snode_app.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/snode_app.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/app.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/app.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/auth_middleware.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/auth_middleware.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/__init__.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/caching_node_app.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/caching_node_app.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/utils.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/utils.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/node_webapp.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/node_webapp.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/static/deploy_cnode.yaml
+Filename: sbcli_dev-2.2.4/simplyblock_web/static/deploy_cnode.yaml
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/static/tst.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/static/tst.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/static/is_up.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/static/is_up.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/static/delete.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/static/delete.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/static/deploy.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/static/deploy.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/static/deploy_spdk.yaml
+Filename: sbcli_dev-2.2.4/simplyblock_web/static/deploy_spdk.yaml
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/static/rpac.yaml
+Filename: sbcli_dev-2.2.4/simplyblock_web/static/rpac.yaml
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/static/list_deps.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/static/list_deps.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/templates/deploy_spdk.yaml.j2
+Filename: sbcli_dev-2.2.4/simplyblock_web/templates/deploy_spdk.yaml.j2
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/blueprints/node_api_caching_docker.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/blueprints/node_api_caching_docker.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/blueprints/node_api_caching_ks.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/blueprints/node_api_caching_ks.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/blueprints/web_api_caching_node.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/blueprints/web_api_caching_node.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/blueprints/snode_ops.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/blueprints/snode_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/blueprints/web_api_lvol.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/blueprints/web_api_lvol.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/blueprints/csi.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/blueprints/csi.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/blueprints/caching_node_ops.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/blueprints/caching_node_ops.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/blueprints/web_api_mgmt_node.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/blueprints/web_api_mgmt_node.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/blueprints/web_api_storage_node.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/blueprints/web_api_storage_node.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/blueprints/__init__.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/blueprints/__init__.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/blueprints/caching_node_ops_k8s.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/blueprints/caching_node_ops_k8s.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/blueprints/web_api_device.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/blueprints/web_api_device.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/blueprints/web_api_cluster.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/blueprints/web_api_cluster.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/blueprints/node_api_basic.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/blueprints/node_api_basic.py
 Comment: 
 
-Filename: sbcli_dev-2.2.3/simplyblock_web/blueprints/web_api_pool.py
+Filename: sbcli_dev-2.2.4/simplyblock_web/blueprints/web_api_pool.py
 Comment: 
 
 Zip file comment:
```

## Comparing `sbcli_dev-2.2.3/setup.py` & `sbcli_dev-2.2.4/setup.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/README.md` & `sbcli_dev-2.2.4/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -13,16 +13,16 @@
 # Components 
 
 ## Simply Block Core
 Contains core logic and controllers for the simplyblock cluster
 
 ## Simply Block CLI
 Please see this document 
-[README.md](../simplyblock_cli/README.md)
+[README.md](../main/simplyblock_cli/README.md)
 
 
 ## Simply Block Web API
 Please see this document 
-[README.md](../simplyblock_web/README.md)
+[README.md](../main/simplyblock_web/README.md)
```

## Comparing `sbcli_dev-2.2.3/PKG-INFO` & `sbcli_dev-2.2.4/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-dev
-Version: 2.2.3
+Version: 2.2.4
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
@@ -29,16 +29,16 @@
 # Components 
 
 ## Simply Block Core
 Contains core logic and controllers for the simplyblock cluster
 
 ## Simply Block CLI
 Please see this document 
-[README.md](../simplyblock_cli/README.md)
+[README.md](../main/simplyblock_cli/README.md)
 
 
 ## Simply Block Web API
 Please see this document 
-[README.md](../simplyblock_web/README.md)
+[README.md](../main/simplyblock_web/README.md)
```

## Comparing `sbcli_dev-2.2.3/simplyblock_cli/cli.py` & `sbcli_dev-2.2.4/simplyblock_cli/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -443,14 +443,18 @@
                                  dest='ha_type', choices=["single", "ha", "default"], default='default')
 
         sub_command.add_argument("--compress",
                                  help='Use inline data compression and de-compression on the logical volume',
                                  required=False, action='store_true')
         sub_command.add_argument("--encrypt", help='Use inline data encryption and de-cryption on the logical volume',
                                  required=False, action='store_true')
+        sub_command.add_argument("--crypto-key1", help='the hex value of key1 to be used for lvol encryption',
+                                 dest='crypto_key1', default=None)
+        sub_command.add_argument("--crypto-key2", help='the hex value of key2 to be used for lvol encryption',
+                                 dest='crypto_key2', default=None)
         sub_command.add_argument("--thick", help='Deactivate thin provisioning', required=False, action='store_true')
         sub_command.add_argument("--node-ha",
                                  help='The maximum amount of concurrent node failures accepted without interruption of operations',
                                  required=False, default=1, type=int, choices=[0, 1, 2])
         sub_command.add_argument("--dev-redundancy",
                                  help='{1,2} supported minimal concurrent device failures without data loss',
                                  required=False, action='store_true')
@@ -1070,15 +1074,17 @@
                     args.max_rw_iops,
                     args.max_rw_mbytes,
                     args.max_r_mbytes,
                     args.max_w_mbytes,
                     distr_bs,
                     distr_chunk_bs,
                     with_snapshot=with_snapshot,
-                    max_size=max_size)
+                    max_size=max_size,
+                    crypto_key1=args.crypto_key1,
+                    crypto_key2=args.crypto_key2)
                 if results:
                     ret = results
                 else:
                     ret = error
             elif sub_command == "add-distr":
                 pass
             elif sub_command == "qos-set":
```

## Comparing `sbcli_dev-2.2.3/sbcli_dev.egg-info/SOURCES.txt` & `sbcli_dev-2.2.4/sbcli_dev.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/sbcli_dev.egg-info/PKG-INFO` & `sbcli_dev-2.2.4/sbcli_dev.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-dev
-Version: 2.2.3
+Version: 2.2.4
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
@@ -29,16 +29,16 @@
 # Components 
 
 ## Simply Block Core
 Contains core logic and controllers for the simplyblock cluster
 
 ## Simply Block CLI
 Please see this document 
-[README.md](../simplyblock_cli/README.md)
+[README.md](../main/simplyblock_cli/README.md)
 
 
 ## Simply Block Web API
 Please see this document 
-[README.md](../simplyblock_web/README.md)
+[README.md](../main/simplyblock_web/README.md)
```

## Comparing `sbcli_dev-2.2.3/simplyblock_core/storage_node_ops.py` & `sbcli_dev-2.2.4/simplyblock_core/storage_node_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -739,16 +739,19 @@
         else:
             logger.error("Snapshots found on the storage node, use --force-remove or --force-migrate")
             return False
 
     if snode.nvme_devices:
         for dev in snode.nvme_devices:
             if dev.status == 'online':
-                distr_controller.send_dev_status_event(dev.cluster_device_order, "unavailable")
-            distr_controller.disconnect_device(dev)
+                distr_controller.disconnect_device(dev)
+            old_status = dev.status
+            dev.status = NVMeDevice.STATUS_FAILED
+            distr_controller.send_dev_status_event(dev.cluster_device_order, NVMeDevice.STATUS_FAILED)
+            device_events.device_status_change(dev, NVMeDevice.STATUS_FAILED, old_status)
 
     for lvol in db_controller.get_lvols():
         lvol_controller.send_cluster_map(lvol.get_id())
 
     logger.info("Removing storage node")
 
     logger.debug("Leaving swarm...")
@@ -762,15 +765,18 @@
     try:
         snode_api = SNodeClient(snode.api_endpoint)
         snode_api.spdk_process_kill()
         snode_api.leave_swarm()
     except Exception as e:
         logger.warning(f"Failed to remove SPDK process: {e}")
 
-    snode.remove(db_controller.kv_store)
+    snode.status = StorageNode.STATUS_REMOVED
+    snode.write_to_db(db_controller.kv_store)
+    logger.info("Sending node event update")
+    distr_controller.send_node_status_event(snode.get_id(), snode.status)
     storage_events.snode_remove(snode)
     logger.info("done")
 
 
 def restart_storage_node(
         node_id,
         spdk_cpu_mask=None,
```

## Comparing `sbcli_dev-2.2.3/simplyblock_core/constants.py` & `sbcli_dev-2.2.4/simplyblock_core/constants.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/mgmt_node_ops.py` & `sbcli_dev-2.2.4/simplyblock_core/mgmt_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/cnode_client.py` & `sbcli_dev-2.2.4/simplyblock_core/cnode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/pci_utils.py` & `sbcli_dev-2.2.4/simplyblock_core/pci_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/snode_client.py` & `sbcli_dev-2.2.4/simplyblock_core/snode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/kv_store.py` & `sbcli_dev-2.2.4/simplyblock_core/kv_store.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/utils.py` & `sbcli_dev-2.2.4/simplyblock_core/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/cluster_ops.py` & `sbcli_dev-2.2.4/simplyblock_core/cluster_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/compute_node_ops.py` & `sbcli_dev-2.2.4/simplyblock_core/compute_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/rpc_client.py` & `sbcli_dev-2.2.4/simplyblock_core/rpc_client.py`

 * *Files 1% similar despite different names*

```diff
@@ -320,14 +320,15 @@
             "base_bdev_name": base_name,
             "name": name,
             "key_name": key_name,
         }
         return self._request("bdev_crypto_create", params)
 
     def lvol_crypto_key_create(self, name, key, key2):
+        # todo: mask the keys so that they don't show up in logs
         params = {
             "cipher": "AES_XTS",
             "key": key,
             "key2": key2,
             "name": name
         }
         return self._request("accel_crypto_key_create", params)
```

## Comparing `sbcli_dev-2.2.3/simplyblock_core/distr_controller.py` & `sbcli_dev-2.2.4/simplyblock_core/distr_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/services/lvol_monitor.py` & `sbcli_dev-2.2.4/simplyblock_core/services/lvol_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/services/caching_node_monitor.py` & `sbcli_dev-2.2.4/simplyblock_core/services/caching_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/services/capacity_collector.py` & `sbcli_dev-2.2.4/simplyblock_core/services/capacity_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/services/health_check_service.py` & `sbcli_dev-2.2.4/simplyblock_core/services/health_check_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/services/lvol_stat_collector.py` & `sbcli_dev-2.2.4/simplyblock_core/services/lvol_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/services/log_agg_service.py` & `sbcli_dev-2.2.4/simplyblock_core/services/log_agg_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/services/distr_event_collector.py` & `sbcli_dev-2.2.4/simplyblock_core/services/distr_event_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/services/capacity_and_stats_collector.py` & `sbcli_dev-2.2.4/simplyblock_core/services/capacity_and_stats_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/services/port_stat_collector.py` & `sbcli_dev-2.2.4/simplyblock_core/services/port_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/services/device_monitor.py` & `sbcli_dev-2.2.4/simplyblock_core/services/device_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/services/__init__.py` & `sbcli_dev-2.2.4/simplyblock_core/services/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/services/install_service.sh` & `sbcli_dev-2.2.4/simplyblock_core/services/install_service.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/services/mgmt_node_monitor.py` & `sbcli_dev-2.2.4/simplyblock_core/services/mgmt_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/services/cap_monitor.py` & `sbcli_dev-2.2.4/simplyblock_core/services/cap_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/services/storage_node_monitor.py` & `sbcli_dev-2.2.4/simplyblock_core/services/storage_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/scripts/deploy_stack.sh` & `sbcli_dev-2.2.4/simplyblock_core/scripts/deploy_stack.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/scripts/haproxy.cfg` & `sbcli_dev-2.2.4/simplyblock_core/scripts/haproxy.cfg`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/scripts/docker-compose-swarm.yml` & `sbcli_dev-2.2.4/simplyblock_core/scripts/docker-compose-swarm.yml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/scripts/stack_deploy_wait.sh` & `sbcli_dev-2.2.4/simplyblock_core/scripts/stack_deploy_wait.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/scripts/__init__.py` & `sbcli_dev-2.2.4/simplyblock_core/scripts/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/scripts/install_deps.sh` & `sbcli_dev-2.2.4/simplyblock_core/scripts/install_deps.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/scripts/apply_dashboard.sh` & `sbcli_dev-2.2.4/simplyblock_core/scripts/apply_dashboard.sh`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/scripts/alerting/alert_rules.yaml` & `sbcli_dev-2.2.4/simplyblock_core/scripts/alerting/alert_rules.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/scripts/alerting/alert_resources.yaml` & `sbcli_dev-2.2.4/simplyblock_core/scripts/alerting/alert_resources.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/scripts/dashboards/devices.json` & `sbcli_dev-2.2.4/simplyblock_core/scripts/dashboards/devices.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/scripts/dashboards/nodes.json` & `sbcli_dev-2.2.4/simplyblock_core/scripts/dashboards/nodes.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/scripts/dashboards/lvols.json` & `sbcli_dev-2.2.4/simplyblock_core/scripts/dashboards/lvols.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/scripts/dashboards/cluster.json` & `sbcli_dev-2.2.4/simplyblock_core/scripts/dashboards/cluster.json`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/controllers/device_controller.py` & `sbcli_dev-2.2.4/simplyblock_core/controllers/device_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/controllers/mgmt_events.py` & `sbcli_dev-2.2.4/simplyblock_core/controllers/mgmt_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/controllers/events_controller.py` & `sbcli_dev-2.2.4/simplyblock_core/controllers/events_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/controllers/storage_events.py` & `sbcli_dev-2.2.4/simplyblock_core/controllers/storage_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/controllers/lvol_events.py` & `sbcli_dev-2.2.4/simplyblock_core/controllers/lvol_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/controllers/snapshot_controller.py` & `sbcli_dev-2.2.4/simplyblock_core/controllers/snapshot_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/controllers/device_events.py` & `sbcli_dev-2.2.4/simplyblock_core/controllers/device_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/controllers/pool_controller.py` & `sbcli_dev-2.2.4/simplyblock_core/controllers/pool_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/controllers/cluster_events.py` & `sbcli_dev-2.2.4/simplyblock_core/controllers/cluster_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/controllers/caching_node_controller.py` & `sbcli_dev-2.2.4/simplyblock_core/controllers/caching_node_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/controllers/snapshot_events.py` & `sbcli_dev-2.2.4/simplyblock_core/controllers/snapshot_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/controllers/lvol_controller.py` & `sbcli_dev-2.2.4/simplyblock_core/controllers/lvol_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -26,21 +26,20 @@
     def _generate_string(length):
         return ''.join(random.SystemRandom().choice(
             string.ascii_letters + string.digits) for _ in range(length))
 
     return _generate_string(length).encode('utf-8').hex()
 
 
-def _create_crypto_lvol(rpc_client, name, base_name):
+def _create_crypto_lvol(rpc_client, name, base_name, key1, key2):
     key_name = f'key_{name}'
-    key1 = _generate_hex_string(32)
-    key2 = _generate_hex_string(32)
     ret = rpc_client.lvol_crypto_key_create(key_name, key1, key2)
     if not ret:
-        logger.warning("failed to create crypto key")
+        logger.error("failed to create crypto key")
+        return False
     ret = rpc_client.lvol_crypto_create(name, base_name, key_name)
     if not ret:
         logger.error(f"failed to create crypto LVol {name}")
         return False
     return ret
 
 
@@ -290,15 +289,15 @@
 
     lvol_type = 'lvol'
     lvol_bdev = f"LVS_{vuid}/{name}"
     crypto_bdev = ''
     comp_bdev = ''
     top_bdev = lvol_bdev
     if use_crypto is True:
-        crypto_bdev = _create_crypto_lvol(rpc_client, name, lvol_bdev)
+        crypto_bdev = _create_crypto_lvol(rpc_client, name, lvol_bdev, "", "")
         bdev_stack.append({"type": "crypto", "name": crypto_bdev})
         if not crypto_bdev:
             return False, "Error creating crypto bdev"
         lvol_type += ',crypto'
         top_bdev = crypto_bdev
 
     if use_comp is True:
@@ -428,19 +427,48 @@
             node = db_controller.get_storage_node_by_id(node_id)
             print(f"Selected node: {node_id}, {node.hostname}")
             ret.append(node)
         return ret
     else:
         return online_nodes
 
+def is_hex(s: str) -> bool:
+    """
+    given an input checks if the value is hex encoded or not
+    """
+    try:
+        int(s, 16)
+        return True
+    except ValueError:
+        return False
+
+def validate_aes_xts_keys(key1: str, key2: str) -> tuple[bool, str]:
+    """
+    Key Length: each key should be either 128 or 256 bits long.
+    since hex values of the keys are expected, the key lengths should be either 32 or 64
+    """
+
+    if len(key1) != len(key2):
+        return False, "both the keys should be of the same length"
+
+    if len(key1) not in [32, 64] or len(key2) not in [32, 64]:
+        return False, "each key should be either 16 or 32 bytes long"
+
+    if not is_hex(key1):
+        return False, "please provide hex encoded value for crypto_key1"
+
+    if not is_hex(key2):
+        return False, "please provide hex encoded value for crypto_key2"
+
+    return True, ""
 
 def add_lvol_ha(name, size, host_id_or_name, ha_type, pool_id_or_name, use_comp, use_crypto,
                 distr_vuid, distr_ndcs, distr_npcs,
                 max_rw_iops, max_rw_mbytes, max_r_mbytes, max_w_mbytes,
-                distr_bs=None, distr_chunk_bs=None, with_snapshot=False, max_size=0):
+                distr_bs=None, distr_chunk_bs=None, with_snapshot=False, max_size=0, crypto_key1=None, crypto_key2=None):
 
     logger.info(f"Adding LVol: {name}")
     host_node = None
     if host_id_or_name:
         host_node = db_controller.get_storage_node_by_id(host_id_or_name)
         if not host_node:
             host_node = db_controller.get_storage_node_by_hostname(host_id_or_name)
@@ -524,15 +552,14 @@
         vuid = distr_vuid
 
     if distr_ndcs == 0 and distr_npcs == 0:
         if ha_type == "single":
             distr_ndcs = 4
             distr_npcs = 1
         else:
-
             if dev_count == 3:
                 distr_ndcs = 1
             elif dev_count in [4, 5]:
                 distr_ndcs = 2
             elif dev_count >= 6:
                 distr_ndcs = 4
             distr_npcs = 1
@@ -616,22 +643,31 @@
                 "lvol_name": lvol.top_bdev,
                 "base_bdev": lvol.base_bdev,
                 "label": "label",
                 "desc": "desc"
             }
         })
 
-    if use_crypto is True:
+    if use_crypto:
+        if crypto_key1 == None or crypto_key2 == None:
+            return False, "encryption keys for lvol not provided"
+        else:
+            success, err = validate_aes_xts_keys(crypto_key1, crypto_key2)
+            if not success:
+                return False, err
+
         lvol.crypto_bdev = f"crypto_{lvol.lvol_name}"
         lvol.bdev_stack.append({
             "type": "crypto",
             "name": lvol.crypto_bdev,
             "params": {
                 "name": lvol.crypto_bdev,
-                "base_name": lvol.lvol_bdev
+                "base_name": lvol.base_bdev,
+                "key1": crypto_key1,
+                "key2": crypto_key2,
             }
         })
         lvol.lvol_type += ',crypto'
         lvol.top_bdev = lvol.crypto_bdev
 
     if use_comp is True:
         base_bdev = lvol.lvol_bdev
```

## Comparing `sbcli_dev-2.2.3/simplyblock_core/controllers/health_controller.py` & `sbcli_dev-2.2.4/simplyblock_core/controllers/health_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/controllers/pool_events.py` & `sbcli_dev-2.2.4/simplyblock_core/controllers/pool_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/models/events.py` & `sbcli_dev-2.2.4/simplyblock_core/models/events.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/models/iface.py` & `sbcli_dev-2.2.4/simplyblock_core/models/iface.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/models/base_model.py` & `sbcli_dev-2.2.4/simplyblock_core/models/base_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/models/lvol_model.py` & `sbcli_dev-2.2.4/simplyblock_core/models/lvol_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/models/compute_node.py` & `sbcli_dev-2.2.4/simplyblock_core/models/compute_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/models/snapshot.py` & `sbcli_dev-2.2.4/simplyblock_core/models/snapshot.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/models/pool.py` & `sbcli_dev-2.2.4/simplyblock_core/models/pool.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/models/global_settings.py` & `sbcli_dev-2.2.4/simplyblock_core/models/global_settings.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/models/port_stat.py` & `sbcli_dev-2.2.4/simplyblock_core/models/port_stat.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/models/storage_node.py` & `sbcli_dev-2.2.4/simplyblock_core/models/storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/models/stats.py` & `sbcli_dev-2.2.4/simplyblock_core/models/stats.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/models/cluster.py` & `sbcli_dev-2.2.4/simplyblock_core/models/cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/models/mgmt_node.py` & `sbcli_dev-2.2.4/simplyblock_core/models/mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/models/caching_node.py` & `sbcli_dev-2.2.4/simplyblock_core/models/caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_core/models/nvme_device.py` & `sbcli_dev-2.2.4/simplyblock_core/models/nvme_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_web/caching_node_app_k8s.py` & `sbcli_dev-2.2.4/simplyblock_web/caching_node_app_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_web/node_utils.py` & `sbcli_dev-2.2.4/simplyblock_web/node_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_web/snode_app.py` & `sbcli_dev-2.2.4/simplyblock_web/snode_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_web/app.py` & `sbcli_dev-2.2.4/simplyblock_web/app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_web/auth_middleware.py` & `sbcli_dev-2.2.4/simplyblock_web/auth_middleware.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_web/caching_node_app.py` & `sbcli_dev-2.2.4/simplyblock_web/caching_node_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_web/utils.py` & `sbcli_dev-2.2.4/simplyblock_web/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_web/node_webapp.py` & `sbcli_dev-2.2.4/simplyblock_web/node_webapp.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_web/static/delete.py` & `sbcli_dev-2.2.4/simplyblock_web/static/delete.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_web/static/deploy.py` & `sbcli_dev-2.2.4/simplyblock_web/static/deploy.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_web/static/deploy_spdk.yaml` & `sbcli_dev-2.2.4/simplyblock_web/static/deploy_spdk.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_web/templates/deploy_spdk.yaml.j2` & `sbcli_dev-2.2.4/simplyblock_web/templates/deploy_spdk.yaml.j2`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_web/blueprints/node_api_caching_docker.py` & `sbcli_dev-2.2.4/simplyblock_web/blueprints/node_api_caching_docker.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_web/blueprints/node_api_caching_ks.py` & `sbcli_dev-2.2.4/simplyblock_web/blueprints/node_api_caching_ks.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_web/blueprints/web_api_caching_node.py` & `sbcli_dev-2.2.4/simplyblock_web/blueprints/web_api_caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_web/blueprints/snode_ops.py` & `sbcli_dev-2.2.4/simplyblock_web/blueprints/snode_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_web/blueprints/web_api_lvol.py` & `sbcli_dev-2.2.4/simplyblock_web/blueprints/web_api_lvol.py`

 * *Files 6% similar despite different names*

```diff
@@ -90,15 +90,16 @@
         | max_w_mbytes    | Maximum Write Mega Bytes Per Second
         | ha_type         | LVol HA type, can be (single,ha,default=cluster's ha type), Default=default
         | distr_vuid      | Distr bdev virtual unique ID, Default=0 means random
         | distr_ndcs      | Distr bdev number of data chunks per stripe, Default=0 means auto set
         | distr_npcs      | Distr bdev number of parity chunks per stripe, Default=0 means auto set
         | distr_bs        | Distr bdev block size, Default=4096
         | distr_chunk_bs  | Distr bdev chunk block size, Default=4096
-
+        | crypto_key1     | the hex value of key1 to be used for lvol encryption
+        | crypto_key2     | the hex value of key2 to be used for lvol encryption
     """""
 
     cl_data = request.get_json()
     logger.debug(cl_data)
     if 'size' not in cl_data:
         return utils.get_csi_response(None, "missing required param: size", 400)
     if 'name' not in cl_data:
@@ -134,14 +135,16 @@
     ha_type = utils.get_value_or_default(cl_data, "ha_type", "default")
 
     distr_vuid = utils.get_int_value_or_default(cl_data, "distr_vuid", 0)
     distr_ndcs = utils.get_int_value_or_default(cl_data, "distr_ndcs", 0)
     distr_npcs = utils.get_int_value_or_default(cl_data, "distr_npcs", 0)
     distr_bs = utils.get_int_value_or_default(cl_data, "distr_ps", 4096)
     distr_chunk_bs = utils.get_int_value_or_default(cl_data, "distr_chunk_bs", 4096)
+    crypto_key1 = utils.get_value_or_default(cl_data, "crypto_key1", None)
+    crypto_key2 = utils.get_value_or_default(cl_data, "crypto_key2", None)
 
     ret, error = lvol_controller.add_lvol_ha(
         name=name,
         size=size,
         pool_id_or_name=pool.get_id(),
 
         use_comp=compression,
@@ -154,15 +157,17 @@
 
         host_id_or_name=None,
         ha_type=ha_type,
         distr_vuid=distr_vuid,
         distr_ndcs=distr_ndcs,
         distr_npcs=distr_npcs,
         distr_bs=distr_bs,
-        distr_chunk_bs=distr_chunk_bs
+        distr_chunk_bs=distr_chunk_bs,
+        crypto_key1=crypto_key1,
+        crypto_key2=crypto_key2,
     )
 
     return utils.get_csi_response(ret, error)
 
 
 @bp.route('/lvol/<string:uuid>', methods=['PUT'])
 def update_lvol(uuid):
```

## Comparing `sbcli_dev-2.2.3/simplyblock_web/blueprints/csi.py` & `sbcli_dev-2.2.4/simplyblock_web/blueprints/csi.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_web/blueprints/caching_node_ops.py` & `sbcli_dev-2.2.4/simplyblock_web/blueprints/caching_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_web/blueprints/web_api_mgmt_node.py` & `sbcli_dev-2.2.4/simplyblock_web/blueprints/web_api_mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_web/blueprints/web_api_storage_node.py` & `sbcli_dev-2.2.4/simplyblock_web/blueprints/web_api_storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_web/blueprints/caching_node_ops_k8s.py` & `sbcli_dev-2.2.4/simplyblock_web/blueprints/caching_node_ops_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_web/blueprints/web_api_device.py` & `sbcli_dev-2.2.4/simplyblock_web/blueprints/web_api_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_web/blueprints/web_api_cluster.py` & `sbcli_dev-2.2.4/simplyblock_web/blueprints/web_api_cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_web/blueprints/node_api_basic.py` & `sbcli_dev-2.2.4/simplyblock_web/blueprints/node_api_basic.py`

 * *Files identical despite different names*

## Comparing `sbcli_dev-2.2.3/simplyblock_web/blueprints/web_api_pool.py` & `sbcli_dev-2.2.4/simplyblock_web/blueprints/web_api_pool.py`

 * *Files identical despite different names*

