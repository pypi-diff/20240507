# Comparing `tmp/sbcli_release-1.1.0.zip` & `tmp/sbcli_release-1.1.2.zip`

## zipinfo {}

```diff
@@ -1,148 +1,148 @@
-Zip file size: 215504 bytes, number of entries: 146
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_cli/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/sbcli_release.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/
--rw-r--r--  2.0 unx     2269 b- defN 24-May-02 16:27 sbcli_release-1.1.0/setup.py
--rw-r--r--  2.0 unx     1068 b- defN 24-May-02 16:27 sbcli_release-1.1.0/README.md
--rw-r--r--  2.0 unx      158 b- defN 24-May-02 16:27 sbcli_release-1.1.0/env_var
--rw-r--r--  2.0 unx       84 b- defN 24-May-02 16:27 sbcli_release-1.1.0/pyproject.toml
--rw-r--r--  2.0 unx       38 b- defN 24-May-02 16:27 sbcli_release-1.1.0/setup.cfg
--rw-r--r--  2.0 unx     1493 b- defN 24-May-02 16:27 sbcli_release-1.1.0/PKG-INFO
--rw-r--r--  2.0 unx    77592 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_cli/cli.py
--rw-r--r--  2.0 unx      357 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_cli/main.py
--rw-r--r--  2.0 unx        1 b- defN 24-May-02 16:27 sbcli_release-1.1.0/sbcli_release.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     5212 b- defN 24-May-02 16:27 sbcli_release-1.1.0/sbcli_release.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx       49 b- defN 24-May-02 16:27 sbcli_release-1.1.0/sbcli_release.egg-info/top_level.txt
--rw-r--r--  2.0 unx     1493 b- defN 24-May-02 16:27 sbcli_release-1.1.0/sbcli_release.egg-info/PKG-INFO
--rw-r--r--  2.0 unx       73 b- defN 24-May-02 16:27 sbcli_release-1.1.0/sbcli_release.egg-info/requires.txt
--rw-r--r--  2.0 unx       59 b- defN 24-May-02 16:27 sbcli_release-1.1.0/sbcli_release.egg-info/entry_points.txt
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/
--rw-r--r--  2.0 unx    69747 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/storage_node_ops.py
--rw-r--r--  2.0 unx     1485 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/constants.py
--rw-r--r--  2.0 unx     3153 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/mgmt_node_ops.py
--rw-r--r--  2.0 unx     3444 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/cnode_client.py
--rw-r--r--  2.0 unx      279 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/shell_utils.py
--rw-r--r--  2.0 unx      938 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/pci_utils.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/__init__.py
--rw-r--r--  2.0 unx     3416 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/snode_client.py
--rw-r--r--  2.0 unx     8189 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/kv_store.py
--rw-r--r--  2.0 unx     7640 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/utils.py
--rw-r--r--  2.0 unx    23423 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/cluster_ops.py
--rw-r--r--  2.0 unx     5112 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/compute_node_ops.py
--rw-r--r--  2.0 unx    21980 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/rpc_client.py
--rw-r--r--  2.0 unx     7504 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/distr_controller.py
--rw-r--r--  2.0 unx     2189 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/lvol_monitor.py
--rw-r--r--  2.0 unx     3203 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/caching_node_monitor.py
--rw-r--r--  2.0 unx     5462 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/health_check_service.py
--rw-r--r--  2.0 unx      229 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/service_template.service
--rw-r--r--  2.0 unx     5268 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/lvol_stat_collector.py
--rw-r--r--  2.0 unx      173 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/remove_service.sh
--rw-r--r--  2.0 unx     2410 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/log_agg_service.py
--rw-r--r--  2.0 unx     5140 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/distr_event_collector.py
--rw-r--r--  2.0 unx     7438 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/capacity_and_stats_collector.py
--rw-r--r--  2.0 unx     2423 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/port_stat_collector.py
--rw-r--r--  2.0 unx     2499 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/device_monitor.py
--rw-r--r--  2.0 unx     4118 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/__init__.py
--rw-r--r--  2.0 unx      837 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/install_service.sh
--rw-r--r--  2.0 unx     3003 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/mgmt_node_monitor.py
--rw-r--r--  2.0 unx     2671 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/cap_monitor.py
--rw-r--r--  2.0 unx     6577 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/services/storage_node_monitor.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/alerting/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/
--rw-r--r--  2.0 unx      930 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/deploy_stack.sh
--rw-r--r--  2.0 unx      152 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/set_db_config.sh
--rw-r--r--  2.0 unx     1163 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/haproxy.cfg
--rw-r--r--  2.0 unx     4977 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/docker-compose-swarm.yml
--rw-r--r--  2.0 unx       54 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/db_config_single.sh
--rw-r--r--  2.0 unx     5305 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/stack_deploy_wait.sh
--rw-r--r--  2.0 unx     4470 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
--rw-r--r--  2.0 unx      453 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/config_docker.sh
--rw-r--r--  2.0 unx     1782 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/__init__.py
--rw-r--r--  2.0 unx      311 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/clean_local_storage_deploy.sh
--rw-r--r--  2.0 unx      118 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/db_config_double.sh
--rw-r--r--  2.0 unx      360 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/datasource.yml
--rw-r--r--  2.0 unx       43 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/run_ssh.sh
--rw-r--r--  2.0 unx     1438 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/install_deps.sh
--rw-r--r--  2.0 unx      311 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/prometheus.yml
--rwxr-xr-x  2.0 unx      657 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/apply_dashboard.sh
--rw-r--r--  2.0 unx    25433 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/alerting/alert_rules.yaml
--rw-r--r--  2.0 unx     1856 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/alerting/alert_resources.yaml
--rw-r--r--  2.0 unx   106705 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/devices.json
--rw-r--r--  2.0 unx   799409 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/node-exporter.json
--rw-r--r--  2.0 unx    99758 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/nodes.json
--rw-r--r--  2.0 unx    99707 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/lvols.json
--rw-r--r--  2.0 unx    99862 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/cluster.json
--rw-r--r--  2.0 unx    99707 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/pools.json
--rw-r--r--  2.0 unx    13127 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/device_controller.py
--rw-r--r--  2.0 unx     1120 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/mgmt_events.py
--rw-r--r--  2.0 unx     3191 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/events_controller.py
--rw-r--r--  2.0 unx     1521 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/storage_events.py
--rw-r--r--  2.0 unx     1630 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/lvol_events.py
--rw-r--r--  2.0 unx    10557 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/snapshot_controller.py
--rw-r--r--  2.0 unx     1568 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/device_events.py
--rw-r--r--  2.0 unx    10375 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/pool_controller.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/__init__.py
--rw-r--r--  2.0 unx     1900 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/cluster_events.py
--rw-r--r--  2.0 unx    22802 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/caching_node_controller.py
--rw-r--r--  2.0 unx     1122 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/snapshot_events.py
--rw-r--r--  2.0 unx    47366 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/lvol_controller.py
--rw-r--r--  2.0 unx    11298 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/health_controller.py
--rw-r--r--  2.0 unx      695 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/controllers/pool_events.py
--rw-r--r--  2.0 unx     1500 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/events.py
--rw-r--r--  2.0 unx      806 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/iface.py
--rw-r--r--  2.0 unx     4846 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/base_model.py
--rw-r--r--  2.0 unx     2579 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/lvol_model.py
--rw-r--r--  2.0 unx      917 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/compute_node.py
--rw-r--r--  2.0 unx      736 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/snapshot.py
--rw-r--r--  2.0 unx     1602 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/pool.py
--rw-r--r--  2.0 unx     1228 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/global_settings.py
--rw-r--r--  2.0 unx     1020 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/port_stat.py
--rw-r--r--  2.0 unx     3765 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/storage_node.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/__init__.py
--rw-r--r--  2.0 unx     4242 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/stats.py
--rw-r--r--  2.0 unx     2565 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/cluster.py
--rw-r--r--  2.0 unx     1466 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/mgmt_node.py
--rw-r--r--  2.0 unx     3766 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/caching_node.py
--rw-r--r--  2.0 unx     3136 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_core/models/nvme_device.py
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/static/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/templates/
-drwxr-xr-x  2.0 unx        0 b- stor 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/
--rw-r--r--  2.0 unx      725 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/caching_node_app_k8s.py
--rw-r--r--  2.0 unx     5098 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/node_utils.py
--rw-r--r--  2.0 unx      703 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/snode_app.py
--rw-r--r--  2.0 unx     1263 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/app.py
--rw-r--r--  2.0 unx     1638 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/auth_middleware.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/__init__.py
--rw-r--r--  2.0 unx      717 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/caching_node_app.py
--rw-r--r--  2.0 unx     2513 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/utils.py
--rw-r--r--  2.0 unx     1434 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/node_webapp.py
--rw-r--r--  2.0 unx      507 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/static/deploy_cnode.yaml
--rw-r--r--  2.0 unx      322 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/static/tst.py
--rw-r--r--  2.0 unx      434 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/static/is_up.py
--rw-r--r--  2.0 unx      827 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/static/delete.py
--rw-r--r--  2.0 unx     1302 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/static/deploy.py
--rw-r--r--  2.0 unx     1466 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/static/deploy_spdk.yaml
--rw-r--r--  2.0 unx      463 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/static/rpac.yaml
--rw-r--r--  2.0 unx      417 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/static/list_deps.py
--rw-r--r--  2.0 unx     2876 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/templates/deploy_spdk.yaml.j2
--rw-r--r--  2.0 unx     5547 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/node_api_caching_docker.py
--rw-r--r--  2.0 unx     4795 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/node_api_caching_ks.py
--rw-r--r--  2.0 unx     5392 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_caching_node.py
--rw-r--r--  2.0 unx    10879 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/snode_ops.py
--rw-r--r--  2.0 unx     8547 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_lvol.py
--rw-r--r--  2.0 unx    11244 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/csi.py
--rw-r--r--  2.0 unx    12198 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/caching_node_ops.py
--rw-r--r--  2.0 unx      975 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_mgmt_node.py
--rw-r--r--  2.0 unx     6326 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_storage_node.py
--rw-r--r--  2.0 unx        0 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/__init__.py
--rw-r--r--  2.0 unx     7846 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/caching_node_ops_k8s.py
--rw-r--r--  2.0 unx     2940 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_device.py
--rw-r--r--  2.0 unx     5274 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_cluster.py
--rw-r--r--  2.0 unx     3103 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/node_api_basic.py
--rw-r--r--  2.0 unx     6206 b- defN 24-May-02 16:27 sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_pool.py
-146 files, 1931280 bytes uncompressed, 187702 bytes compressed:  90.3%
+Zip file size: 215995 bytes, number of entries: 146
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-07 10:52 sbcli_release-1.1.2/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_cli/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-07 10:52 sbcli_release-1.1.2/sbcli_release.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/
+-rw-r--r--  2.0 unx     2269 b- defN 24-May-07 10:52 sbcli_release-1.1.2/setup.py
+-rw-r--r--  2.0 unx     1068 b- defN 24-May-07 10:52 sbcli_release-1.1.2/README.md
+-rw-r--r--  2.0 unx      158 b- defN 24-May-07 10:52 sbcli_release-1.1.2/env_var
+-rw-r--r--  2.0 unx       84 b- defN 24-May-07 10:52 sbcli_release-1.1.2/pyproject.toml
+-rw-r--r--  2.0 unx       38 b- defN 24-May-07 10:52 sbcli_release-1.1.2/setup.cfg
+-rw-r--r--  2.0 unx     1493 b- defN 24-May-07 10:52 sbcli_release-1.1.2/PKG-INFO
+-rw-r--r--  2.0 unx    77728 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_cli/cli.py
+-rw-r--r--  2.0 unx      357 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_cli/main.py
+-rw-r--r--  2.0 unx        1 b- defN 24-May-07 10:52 sbcli_release-1.1.2/sbcli_release.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     5212 b- defN 24-May-07 10:52 sbcli_release-1.1.2/sbcli_release.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx       49 b- defN 24-May-07 10:52 sbcli_release-1.1.2/sbcli_release.egg-info/top_level.txt
+-rw-r--r--  2.0 unx     1493 b- defN 24-May-07 10:52 sbcli_release-1.1.2/sbcli_release.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx       73 b- defN 24-May-07 10:52 sbcli_release-1.1.2/sbcli_release.egg-info/requires.txt
+-rw-r--r--  2.0 unx       59 b- defN 24-May-07 10:52 sbcli_release-1.1.2/sbcli_release.egg-info/entry_points.txt
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/services/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/controllers/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/models/
+-rw-r--r--  2.0 unx    69747 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/storage_node_ops.py
+-rw-r--r--  2.0 unx     1514 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/constants.py
+-rw-r--r--  2.0 unx     3153 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/mgmt_node_ops.py
+-rw-r--r--  2.0 unx     3638 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/cnode_client.py
+-rw-r--r--  2.0 unx      279 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/shell_utils.py
+-rw-r--r--  2.0 unx      938 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/pci_utils.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/__init__.py
+-rw-r--r--  2.0 unx     3416 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/snode_client.py
+-rw-r--r--  2.0 unx     8343 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/kv_store.py
+-rw-r--r--  2.0 unx     7640 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/utils.py
+-rw-r--r--  2.0 unx    23423 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/cluster_ops.py
+-rw-r--r--  2.0 unx     5112 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/compute_node_ops.py
+-rw-r--r--  2.0 unx    21980 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/rpc_client.py
+-rw-r--r--  2.0 unx     7504 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/distr_controller.py
+-rw-r--r--  2.0 unx     2189 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/services/lvol_monitor.py
+-rw-r--r--  2.0 unx     3203 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/services/caching_node_monitor.py
+-rw-r--r--  2.0 unx     5462 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/services/health_check_service.py
+-rw-r--r--  2.0 unx      229 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/services/service_template.service
+-rw-r--r--  2.0 unx     5268 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/services/lvol_stat_collector.py
+-rw-r--r--  2.0 unx      173 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/services/remove_service.sh
+-rw-r--r--  2.0 unx     2410 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/services/log_agg_service.py
+-rw-r--r--  2.0 unx     5140 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/services/distr_event_collector.py
+-rw-r--r--  2.0 unx     7438 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/services/capacity_and_stats_collector.py
+-rw-r--r--  2.0 unx     2423 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/services/port_stat_collector.py
+-rw-r--r--  2.0 unx     2499 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/services/device_monitor.py
+-rw-r--r--  2.0 unx     4118 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/services/__init__.py
+-rw-r--r--  2.0 unx      837 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/services/install_service.sh
+-rw-r--r--  2.0 unx     3003 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/services/mgmt_node_monitor.py
+-rw-r--r--  2.0 unx     2671 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/services/cap_monitor.py
+-rw-r--r--  2.0 unx     6577 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/services/storage_node_monitor.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/alerting/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/dashboards/
+-rw-r--r--  2.0 unx      930 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/deploy_stack.sh
+-rw-r--r--  2.0 unx      152 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/set_db_config.sh
+-rw-r--r--  2.0 unx     1163 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/haproxy.cfg
+-rw-r--r--  2.0 unx     5333 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/docker-compose-swarm.yml
+-rw-r--r--  2.0 unx       54 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/db_config_single.sh
+-rw-r--r--  2.0 unx     5305 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/stack_deploy_wait.sh
+-rw-r--r--  2.0 unx     4409 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
+-rw-r--r--  2.0 unx      453 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/config_docker.sh
+-rw-r--r--  2.0 unx     1782 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/__init__.py
+-rw-r--r--  2.0 unx      311 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/clean_local_storage_deploy.sh
+-rw-r--r--  2.0 unx      118 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/db_config_double.sh
+-rw-r--r--  2.0 unx      360 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/datasource.yml
+-rw-r--r--  2.0 unx       43 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/run_ssh.sh
+-rw-r--r--  2.0 unx     1438 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/install_deps.sh
+-rw-r--r--  2.0 unx      311 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/prometheus.yml
+-rwxr-xr-x  2.0 unx      657 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/apply_dashboard.sh
+-rw-r--r--  2.0 unx    25433 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/alerting/alert_rules.yaml
+-rw-r--r--  2.0 unx     1856 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/alerting/alert_resources.yaml
+-rw-r--r--  2.0 unx   106705 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/dashboards/devices.json
+-rw-r--r--  2.0 unx   799409 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/dashboards/node-exporter.json
+-rw-r--r--  2.0 unx    99758 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/dashboards/nodes.json
+-rw-r--r--  2.0 unx    99707 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/dashboards/lvols.json
+-rw-r--r--  2.0 unx    99862 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/dashboards/cluster.json
+-rw-r--r--  2.0 unx    99707 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/scripts/dashboards/pools.json
+-rw-r--r--  2.0 unx    13127 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/controllers/device_controller.py
+-rw-r--r--  2.0 unx     1120 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/controllers/mgmt_events.py
+-rw-r--r--  2.0 unx     3191 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/controllers/events_controller.py
+-rw-r--r--  2.0 unx     1521 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/controllers/storage_events.py
+-rw-r--r--  2.0 unx     1630 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/controllers/lvol_events.py
+-rw-r--r--  2.0 unx    10557 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/controllers/snapshot_controller.py
+-rw-r--r--  2.0 unx     1568 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/controllers/device_events.py
+-rw-r--r--  2.0 unx    10375 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/controllers/pool_controller.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/controllers/__init__.py
+-rw-r--r--  2.0 unx     1900 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/controllers/cluster_events.py
+-rw-r--r--  2.0 unx    23200 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/controllers/caching_node_controller.py
+-rw-r--r--  2.0 unx     1122 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/controllers/snapshot_events.py
+-rw-r--r--  2.0 unx    47498 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/controllers/lvol_controller.py
+-rw-r--r--  2.0 unx    11298 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/controllers/health_controller.py
+-rw-r--r--  2.0 unx      695 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/controllers/pool_events.py
+-rw-r--r--  2.0 unx     1500 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/models/events.py
+-rw-r--r--  2.0 unx      806 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/models/iface.py
+-rw-r--r--  2.0 unx     4846 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/models/base_model.py
+-rw-r--r--  2.0 unx     2579 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/models/lvol_model.py
+-rw-r--r--  2.0 unx      917 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/models/compute_node.py
+-rw-r--r--  2.0 unx      736 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/models/snapshot.py
+-rw-r--r--  2.0 unx     1602 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/models/pool.py
+-rw-r--r--  2.0 unx     1228 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/models/global_settings.py
+-rw-r--r--  2.0 unx     1020 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/models/port_stat.py
+-rw-r--r--  2.0 unx     3765 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/models/storage_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/models/__init__.py
+-rw-r--r--  2.0 unx     4242 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/models/stats.py
+-rw-r--r--  2.0 unx     2565 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/models/cluster.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/models/mgmt_node.py
+-rw-r--r--  2.0 unx     3766 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/models/caching_node.py
+-rw-r--r--  2.0 unx     3136 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_core/models/nvme_device.py
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/static/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/templates/
+drwxr-xr-x  2.0 unx        0 b- stor 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/blueprints/
+-rw-r--r--  2.0 unx      725 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/caching_node_app_k8s.py
+-rw-r--r--  2.0 unx     5098 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/node_utils.py
+-rw-r--r--  2.0 unx      703 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/snode_app.py
+-rw-r--r--  2.0 unx     1263 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/app.py
+-rw-r--r--  2.0 unx     1638 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/auth_middleware.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/__init__.py
+-rw-r--r--  2.0 unx      717 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/caching_node_app.py
+-rw-r--r--  2.0 unx     2513 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/utils.py
+-rw-r--r--  2.0 unx     1434 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/node_webapp.py
+-rw-r--r--  2.0 unx      507 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/static/deploy_cnode.yaml
+-rw-r--r--  2.0 unx      322 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/static/tst.py
+-rw-r--r--  2.0 unx      434 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/static/is_up.py
+-rw-r--r--  2.0 unx      827 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/static/delete.py
+-rw-r--r--  2.0 unx     1302 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/static/deploy.py
+-rw-r--r--  2.0 unx     1466 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/static/deploy_spdk.yaml
+-rw-r--r--  2.0 unx      463 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/static/rpac.yaml
+-rw-r--r--  2.0 unx      417 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/static/list_deps.py
+-rw-r--r--  2.0 unx     2905 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/templates/deploy_spdk.yaml.j2
+-rw-r--r--  2.0 unx     5547 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/blueprints/node_api_caching_docker.py
+-rw-r--r--  2.0 unx     4883 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/blueprints/node_api_caching_ks.py
+-rw-r--r--  2.0 unx     5491 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/blueprints/web_api_caching_node.py
+-rw-r--r--  2.0 unx    10879 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/blueprints/snode_ops.py
+-rw-r--r--  2.0 unx     8547 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/blueprints/web_api_lvol.py
+-rw-r--r--  2.0 unx    11244 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/blueprints/csi.py
+-rw-r--r--  2.0 unx    12198 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/blueprints/caching_node_ops.py
+-rw-r--r--  2.0 unx      975 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/blueprints/web_api_mgmt_node.py
+-rw-r--r--  2.0 unx     6326 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/blueprints/web_api_storage_node.py
+-rw-r--r--  2.0 unx        0 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/blueprints/__init__.py
+-rw-r--r--  2.0 unx     8075 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/blueprints/caching_node_ops_k8s.py
+-rw-r--r--  2.0 unx     2940 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/blueprints/web_api_device.py
+-rw-r--r--  2.0 unx     5274 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/blueprints/web_api_cluster.py
+-rw-r--r--  2.0 unx     3103 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/blueprints/node_api_basic.py
+-rw-r--r--  2.0 unx     6206 b- defN 24-May-07 10:52 sbcli_release-1.1.2/simplyblock_web/blueprints/web_api_pool.py
+146 files, 1933063 bytes uncompressed, 188193 bytes compressed:  90.3%
```

## zipnote {}

```diff
@@ -1,439 +1,439 @@
-Filename: sbcli_release-1.1.0/
+Filename: sbcli_release-1.1.2/
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_cli/
+Filename: sbcli_release-1.1.2/simplyblock_cli/
 Comment: 
 
-Filename: sbcli_release-1.1.0/sbcli_release.egg-info/
+Filename: sbcli_release-1.1.2/sbcli_release.egg-info/
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/
+Filename: sbcli_release-1.1.2/simplyblock_core/
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/
+Filename: sbcli_release-1.1.2/simplyblock_web/
 Comment: 
 
-Filename: sbcli_release-1.1.0/setup.py
+Filename: sbcli_release-1.1.2/setup.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/README.md
+Filename: sbcli_release-1.1.2/README.md
 Comment: 
 
-Filename: sbcli_release-1.1.0/env_var
+Filename: sbcli_release-1.1.2/env_var
 Comment: 
 
-Filename: sbcli_release-1.1.0/pyproject.toml
+Filename: sbcli_release-1.1.2/pyproject.toml
 Comment: 
 
-Filename: sbcli_release-1.1.0/setup.cfg
+Filename: sbcli_release-1.1.2/setup.cfg
 Comment: 
 
-Filename: sbcli_release-1.1.0/PKG-INFO
+Filename: sbcli_release-1.1.2/PKG-INFO
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_cli/cli.py
+Filename: sbcli_release-1.1.2/simplyblock_cli/cli.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_cli/main.py
+Filename: sbcli_release-1.1.2/simplyblock_cli/main.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/sbcli_release.egg-info/dependency_links.txt
+Filename: sbcli_release-1.1.2/sbcli_release.egg-info/dependency_links.txt
 Comment: 
 
-Filename: sbcli_release-1.1.0/sbcli_release.egg-info/SOURCES.txt
+Filename: sbcli_release-1.1.2/sbcli_release.egg-info/SOURCES.txt
 Comment: 
 
-Filename: sbcli_release-1.1.0/sbcli_release.egg-info/top_level.txt
+Filename: sbcli_release-1.1.2/sbcli_release.egg-info/top_level.txt
 Comment: 
 
-Filename: sbcli_release-1.1.0/sbcli_release.egg-info/PKG-INFO
+Filename: sbcli_release-1.1.2/sbcli_release.egg-info/PKG-INFO
 Comment: 
 
-Filename: sbcli_release-1.1.0/sbcli_release.egg-info/requires.txt
+Filename: sbcli_release-1.1.2/sbcli_release.egg-info/requires.txt
 Comment: 
 
-Filename: sbcli_release-1.1.0/sbcli_release.egg-info/entry_points.txt
+Filename: sbcli_release-1.1.2/sbcli_release.egg-info/entry_points.txt
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/services/
+Filename: sbcli_release-1.1.2/simplyblock_core/services/
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/controllers/
+Filename: sbcli_release-1.1.2/simplyblock_core/controllers/
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/models/
+Filename: sbcli_release-1.1.2/simplyblock_core/models/
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/storage_node_ops.py
+Filename: sbcli_release-1.1.2/simplyblock_core/storage_node_ops.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/constants.py
+Filename: sbcli_release-1.1.2/simplyblock_core/constants.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/mgmt_node_ops.py
+Filename: sbcli_release-1.1.2/simplyblock_core/mgmt_node_ops.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/cnode_client.py
+Filename: sbcli_release-1.1.2/simplyblock_core/cnode_client.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/shell_utils.py
+Filename: sbcli_release-1.1.2/simplyblock_core/shell_utils.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/pci_utils.py
+Filename: sbcli_release-1.1.2/simplyblock_core/pci_utils.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/__init__.py
+Filename: sbcli_release-1.1.2/simplyblock_core/__init__.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/snode_client.py
+Filename: sbcli_release-1.1.2/simplyblock_core/snode_client.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/kv_store.py
+Filename: sbcli_release-1.1.2/simplyblock_core/kv_store.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/utils.py
+Filename: sbcli_release-1.1.2/simplyblock_core/utils.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/cluster_ops.py
+Filename: sbcli_release-1.1.2/simplyblock_core/cluster_ops.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/compute_node_ops.py
+Filename: sbcli_release-1.1.2/simplyblock_core/compute_node_ops.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/rpc_client.py
+Filename: sbcli_release-1.1.2/simplyblock_core/rpc_client.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/distr_controller.py
+Filename: sbcli_release-1.1.2/simplyblock_core/distr_controller.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/services/lvol_monitor.py
+Filename: sbcli_release-1.1.2/simplyblock_core/services/lvol_monitor.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/services/caching_node_monitor.py
+Filename: sbcli_release-1.1.2/simplyblock_core/services/caching_node_monitor.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/services/health_check_service.py
+Filename: sbcli_release-1.1.2/simplyblock_core/services/health_check_service.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/services/service_template.service
+Filename: sbcli_release-1.1.2/simplyblock_core/services/service_template.service
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/services/lvol_stat_collector.py
+Filename: sbcli_release-1.1.2/simplyblock_core/services/lvol_stat_collector.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/services/remove_service.sh
+Filename: sbcli_release-1.1.2/simplyblock_core/services/remove_service.sh
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/services/log_agg_service.py
+Filename: sbcli_release-1.1.2/simplyblock_core/services/log_agg_service.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/services/distr_event_collector.py
+Filename: sbcli_release-1.1.2/simplyblock_core/services/distr_event_collector.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/services/capacity_and_stats_collector.py
+Filename: sbcli_release-1.1.2/simplyblock_core/services/capacity_and_stats_collector.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/services/port_stat_collector.py
+Filename: sbcli_release-1.1.2/simplyblock_core/services/port_stat_collector.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/services/device_monitor.py
+Filename: sbcli_release-1.1.2/simplyblock_core/services/device_monitor.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/services/__init__.py
+Filename: sbcli_release-1.1.2/simplyblock_core/services/__init__.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/services/install_service.sh
+Filename: sbcli_release-1.1.2/simplyblock_core/services/install_service.sh
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/services/mgmt_node_monitor.py
+Filename: sbcli_release-1.1.2/simplyblock_core/services/mgmt_node_monitor.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/services/cap_monitor.py
+Filename: sbcli_release-1.1.2/simplyblock_core/services/cap_monitor.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/services/storage_node_monitor.py
+Filename: sbcli_release-1.1.2/simplyblock_core/services/storage_node_monitor.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/alerting/
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/alerting/
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/dashboards/
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/deploy_stack.sh
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/deploy_stack.sh
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/set_db_config.sh
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/set_db_config.sh
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/haproxy.cfg
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/haproxy.cfg
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/docker-compose-swarm.yml
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/docker-compose-swarm.yml
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/db_config_single.sh
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/db_config_single.sh
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/stack_deploy_wait.sh
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/stack_deploy_wait.sh
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/config_docker.sh
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/config_docker.sh
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/__init__.py
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/__init__.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/clean_local_storage_deploy.sh
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/clean_local_storage_deploy.sh
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/db_config_double.sh
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/db_config_double.sh
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/datasource.yml
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/datasource.yml
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/run_ssh.sh
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/run_ssh.sh
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/install_deps.sh
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/install_deps.sh
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/prometheus.yml
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/prometheus.yml
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/apply_dashboard.sh
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/apply_dashboard.sh
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/alerting/alert_rules.yaml
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/alerting/alert_rules.yaml
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/alerting/alert_resources.yaml
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/alerting/alert_resources.yaml
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/devices.json
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/dashboards/devices.json
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/node-exporter.json
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/dashboards/node-exporter.json
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/nodes.json
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/dashboards/nodes.json
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/lvols.json
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/dashboards/lvols.json
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/cluster.json
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/dashboards/cluster.json
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/pools.json
+Filename: sbcli_release-1.1.2/simplyblock_core/scripts/dashboards/pools.json
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/controllers/device_controller.py
+Filename: sbcli_release-1.1.2/simplyblock_core/controllers/device_controller.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/controllers/mgmt_events.py
+Filename: sbcli_release-1.1.2/simplyblock_core/controllers/mgmt_events.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/controllers/events_controller.py
+Filename: sbcli_release-1.1.2/simplyblock_core/controllers/events_controller.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/controllers/storage_events.py
+Filename: sbcli_release-1.1.2/simplyblock_core/controllers/storage_events.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/controllers/lvol_events.py
+Filename: sbcli_release-1.1.2/simplyblock_core/controllers/lvol_events.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/controllers/snapshot_controller.py
+Filename: sbcli_release-1.1.2/simplyblock_core/controllers/snapshot_controller.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/controllers/device_events.py
+Filename: sbcli_release-1.1.2/simplyblock_core/controllers/device_events.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/controllers/pool_controller.py
+Filename: sbcli_release-1.1.2/simplyblock_core/controllers/pool_controller.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/controllers/__init__.py
+Filename: sbcli_release-1.1.2/simplyblock_core/controllers/__init__.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/controllers/cluster_events.py
+Filename: sbcli_release-1.1.2/simplyblock_core/controllers/cluster_events.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/controllers/caching_node_controller.py
+Filename: sbcli_release-1.1.2/simplyblock_core/controllers/caching_node_controller.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/controllers/snapshot_events.py
+Filename: sbcli_release-1.1.2/simplyblock_core/controllers/snapshot_events.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/controllers/lvol_controller.py
+Filename: sbcli_release-1.1.2/simplyblock_core/controllers/lvol_controller.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/controllers/health_controller.py
+Filename: sbcli_release-1.1.2/simplyblock_core/controllers/health_controller.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/controllers/pool_events.py
+Filename: sbcli_release-1.1.2/simplyblock_core/controllers/pool_events.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/models/events.py
+Filename: sbcli_release-1.1.2/simplyblock_core/models/events.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/models/iface.py
+Filename: sbcli_release-1.1.2/simplyblock_core/models/iface.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/models/base_model.py
+Filename: sbcli_release-1.1.2/simplyblock_core/models/base_model.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/models/lvol_model.py
+Filename: sbcli_release-1.1.2/simplyblock_core/models/lvol_model.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/models/compute_node.py
+Filename: sbcli_release-1.1.2/simplyblock_core/models/compute_node.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/models/snapshot.py
+Filename: sbcli_release-1.1.2/simplyblock_core/models/snapshot.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/models/pool.py
+Filename: sbcli_release-1.1.2/simplyblock_core/models/pool.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/models/global_settings.py
+Filename: sbcli_release-1.1.2/simplyblock_core/models/global_settings.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/models/port_stat.py
+Filename: sbcli_release-1.1.2/simplyblock_core/models/port_stat.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/models/storage_node.py
+Filename: sbcli_release-1.1.2/simplyblock_core/models/storage_node.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/models/__init__.py
+Filename: sbcli_release-1.1.2/simplyblock_core/models/__init__.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/models/stats.py
+Filename: sbcli_release-1.1.2/simplyblock_core/models/stats.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/models/cluster.py
+Filename: sbcli_release-1.1.2/simplyblock_core/models/cluster.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/models/mgmt_node.py
+Filename: sbcli_release-1.1.2/simplyblock_core/models/mgmt_node.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/models/caching_node.py
+Filename: sbcli_release-1.1.2/simplyblock_core/models/caching_node.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_core/models/nvme_device.py
+Filename: sbcli_release-1.1.2/simplyblock_core/models/nvme_device.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/static/
+Filename: sbcli_release-1.1.2/simplyblock_web/static/
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/templates/
+Filename: sbcli_release-1.1.2/simplyblock_web/templates/
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/
+Filename: sbcli_release-1.1.2/simplyblock_web/blueprints/
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/caching_node_app_k8s.py
+Filename: sbcli_release-1.1.2/simplyblock_web/caching_node_app_k8s.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/node_utils.py
+Filename: sbcli_release-1.1.2/simplyblock_web/node_utils.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/snode_app.py
+Filename: sbcli_release-1.1.2/simplyblock_web/snode_app.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/app.py
+Filename: sbcli_release-1.1.2/simplyblock_web/app.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/auth_middleware.py
+Filename: sbcli_release-1.1.2/simplyblock_web/auth_middleware.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/__init__.py
+Filename: sbcli_release-1.1.2/simplyblock_web/__init__.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/caching_node_app.py
+Filename: sbcli_release-1.1.2/simplyblock_web/caching_node_app.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/utils.py
+Filename: sbcli_release-1.1.2/simplyblock_web/utils.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/node_webapp.py
+Filename: sbcli_release-1.1.2/simplyblock_web/node_webapp.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/static/deploy_cnode.yaml
+Filename: sbcli_release-1.1.2/simplyblock_web/static/deploy_cnode.yaml
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/static/tst.py
+Filename: sbcli_release-1.1.2/simplyblock_web/static/tst.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/static/is_up.py
+Filename: sbcli_release-1.1.2/simplyblock_web/static/is_up.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/static/delete.py
+Filename: sbcli_release-1.1.2/simplyblock_web/static/delete.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/static/deploy.py
+Filename: sbcli_release-1.1.2/simplyblock_web/static/deploy.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/static/deploy_spdk.yaml
+Filename: sbcli_release-1.1.2/simplyblock_web/static/deploy_spdk.yaml
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/static/rpac.yaml
+Filename: sbcli_release-1.1.2/simplyblock_web/static/rpac.yaml
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/static/list_deps.py
+Filename: sbcli_release-1.1.2/simplyblock_web/static/list_deps.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/templates/deploy_spdk.yaml.j2
+Filename: sbcli_release-1.1.2/simplyblock_web/templates/deploy_spdk.yaml.j2
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/node_api_caching_docker.py
+Filename: sbcli_release-1.1.2/simplyblock_web/blueprints/node_api_caching_docker.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/node_api_caching_ks.py
+Filename: sbcli_release-1.1.2/simplyblock_web/blueprints/node_api_caching_ks.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_caching_node.py
+Filename: sbcli_release-1.1.2/simplyblock_web/blueprints/web_api_caching_node.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/snode_ops.py
+Filename: sbcli_release-1.1.2/simplyblock_web/blueprints/snode_ops.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_lvol.py
+Filename: sbcli_release-1.1.2/simplyblock_web/blueprints/web_api_lvol.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/csi.py
+Filename: sbcli_release-1.1.2/simplyblock_web/blueprints/csi.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/caching_node_ops.py
+Filename: sbcli_release-1.1.2/simplyblock_web/blueprints/caching_node_ops.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_mgmt_node.py
+Filename: sbcli_release-1.1.2/simplyblock_web/blueprints/web_api_mgmt_node.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_storage_node.py
+Filename: sbcli_release-1.1.2/simplyblock_web/blueprints/web_api_storage_node.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/__init__.py
+Filename: sbcli_release-1.1.2/simplyblock_web/blueprints/__init__.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/caching_node_ops_k8s.py
+Filename: sbcli_release-1.1.2/simplyblock_web/blueprints/caching_node_ops_k8s.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_device.py
+Filename: sbcli_release-1.1.2/simplyblock_web/blueprints/web_api_device.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_cluster.py
+Filename: sbcli_release-1.1.2/simplyblock_web/blueprints/web_api_cluster.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/node_api_basic.py
+Filename: sbcli_release-1.1.2/simplyblock_web/blueprints/node_api_basic.py
 Comment: 
 
-Filename: sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_pool.py
+Filename: sbcli_release-1.1.2/simplyblock_web/blueprints/web_api_pool.py
 Comment: 
 
 Zip file comment:
```

## Comparing `sbcli_release-1.1.0/setup.py` & `sbcli_release-1.1.2/setup.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/README.md` & `sbcli_release-1.1.2/README.md`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/PKG-INFO` & `sbcli_release-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-release
-Version: 1.1.0
+Version: 1.1.2
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_release-1.1.0/simplyblock_cli/cli.py` & `sbcli_release-1.1.2/simplyblock_cli/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -307,16 +307,16 @@
         sub_command.add_argument("--cap-crit", help='Capacity critical level in percent, default=90',
                                  type=int, required=False, dest="cap_crit")
         sub_command.add_argument("--prov-cap-warn", help='Capacity warning level in percent, default=180',
                                  type=int, required=False, dest="prov_cap_warn")
         sub_command.add_argument("--prov-cap-crit", help='Capacity critical level in percent, default=190',
                                  type=int, required=False, dest="prov_cap_crit")
         sub_command.add_argument("--ifname", help='Management interface name, default: eth0')
-        sub_command.add_argument("--log-del-interval", help='graylog deletion interval, default: 24h',
-                                 dest='log_del_interval', default='24h')
+        sub_command.add_argument("--log-del-interval", help='graylog deletion interval, default: 7d',
+                                 dest='log_del_interval', default='7d')
         sub_command.add_argument("--metrics-retention-period", help='retention period for prometheus metrics, default: 7d',
                                  dest='metrics_retention_period', default='7d')
 
         # show cluster list
         sub_command = self.add_sub_command(subparser, 'list', 'Show clusters list')
 
         # # join cluster
@@ -719,14 +719,15 @@
         sub_command.add_argument("cluster_id", help='UUID of the cluster to which the node will belong')
         sub_command.add_argument("node_ip", help='IP of caching node to add')
         sub_command.add_argument("ifname", help='Management interface name')
         sub_command.add_argument("--cpu-mask", help='SPDK app CPU mask, default is all cores found',
                                  dest='spdk_cpu_mask')
         sub_command.add_argument("--memory", help='SPDK huge memory allocation, default is Max hugepages available', dest='spdk_mem')
         sub_command.add_argument("--spdk-image", help='SPDK image uri', dest='spdk_image')
+        sub_command.add_argument("--namespace", help='k8s namespace to deploy on',)
 
         sub_command = self.add_sub_command(subparser, 'list', 'List Caching nodes')
 
         sub_command = self.add_sub_command(subparser, 'list-lvols', 'List connected lvols')
         sub_command.add_argument("id", help='Caching Node UUID')
 
         sub_command = self.add_sub_command(subparser, 'remove', 'Remove Caching node from the cluster')
@@ -1254,14 +1255,15 @@
 
             if sub_command == "add-node":
                 cluster_id = args.cluster_id
                 node_ip = args.node_ip
                 ifname = args.ifname
                 data_nics = []
                 spdk_image = args.spdk_image
+                namespace = args.namespace
 
                 spdk_cpu_mask = None
                 if args.spdk_cpu_mask:
                     if self.validate_cpu_mask(args.spdk_cpu_mask):
                         spdk_cpu_mask = args.spdk_cpu_mask
                     else:
                         return f"Invalid cpu mask value: {args.spdk_cpu_mask}"
@@ -1269,15 +1271,15 @@
                 spdk_mem = None
                 if args.spdk_mem:
                     spdk_mem = self.parse_size(args.spdk_mem)
                     if spdk_mem < 1 * 1024 * 1024:
                         return f"SPDK memory:{args.spdk_mem} must be larger than 1G"
 
                 ret = caching_node_controller.add_node(
-                    cluster_id, node_ip, ifname, data_nics, spdk_cpu_mask, spdk_mem, spdk_image)
+                    cluster_id, node_ip, ifname, data_nics, spdk_cpu_mask, spdk_mem, spdk_image, namespace)
 
             if sub_command == "list":
                 #cluster_id
                 ret = caching_node_controller.list_nodes()
             if sub_command == "list-lvols":
                 ret = caching_node_controller.list_lvols(args.id)
             if sub_command == "remove":
```

## Comparing `sbcli_release-1.1.0/sbcli_release.egg-info/SOURCES.txt` & `sbcli_release-1.1.2/sbcli_release.egg-info/SOURCES.txt`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/sbcli_release.egg-info/PKG-INFO` & `sbcli_release-1.1.2/sbcli_release.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbcli-release
-Version: 1.1.0
+Version: 1.1.2
 Summary: CLI for managing SimplyBlock cluster
 Home-page: https://www.simplyblock.io/
 Author: Hamdy
 Author-email: hamdy@simplyblock.io
 Description-Content-Type: text/markdown
 Requires-Dist: foundationdb
 Requires-Dist: requests
```

## Comparing `sbcli_release-1.1.0/simplyblock_core/storage_node_ops.py` & `sbcli_release-1.1.2/simplyblock_core/storage_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/constants.py` & `sbcli_release-1.1.2/simplyblock_core/constants.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,12 +47,14 @@
 # To use 75% of hugepages to calculate ssd size to use for the ocf bdev
 CACHING_NODE_MEMORY_FACTOR = 0.75
 
 HEALTH_CHECK_INTERVAL_SEC = 60
 
 GRAYLOG_CHECK_INTERVAL_SEC = 60
 
+FDB_CHECK_INTERVAL_SEC = 60
+
 SIMPLY_BLOCK_DOCKER_IMAGE = "simplyblock/simplyblock:release_v1"
 SIMPLY_BLOCK_SPDK_CORE_IMAGE = "simplyblock/spdk-core:latest"
 SIMPLY_BLOCK_SPDK_ULTRA_IMAGE = "simplyblock/spdk:release_v1-latest"
 
 GELF_PORT = 12201
```

## Comparing `sbcli_release-1.1.0/simplyblock_core/mgmt_node_ops.py` & `sbcli_release-1.1.2/simplyblock_core/mgmt_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/cnode_client.py` & `sbcli_release-1.1.2/simplyblock_core/cnode_client.py`

 * *Files 6% similar despite different names*

```diff
@@ -65,33 +65,39 @@
 
     def is_live(self):
         return self._request("GET", "")
 
     def info(self):
         return self._request("GET", "cnode/info")
 
-    def spdk_process_start(self, spdk_cpu_mask, spdk_mem, spdk_image, server_ip, rpc_port, rpc_username, rpc_password):
+    def spdk_process_start(
+            self, spdk_cpu_mask, spdk_mem, spdk_image, server_ip, rpc_port, rpc_username, rpc_password, namespace=None):
         params = {
             "spdk_cpu_mask": spdk_cpu_mask,
             "spdk_mem": spdk_mem,
             "spdk_image": spdk_image,
             "server_ip": server_ip,
             "rpc_port": rpc_port,
             "rpc_username": rpc_username,
             "rpc_password": rpc_password,
         }
+        if namespace:
+            params["namespace"] = namespace
         return self._request("POST", "cnode/spdk_process_start", params)
 
     def join_db(self, db_connection):
         params = {"db_connection": db_connection}
         return self._request("POST", "cnode/join_db", params)
 
     def spdk_process_kill(self):
         return self._request("GET", "cnode/spdk_process_kill")
 
+    def spdk_process_is_up(self):
+        return self._request("GET", "cnode/spdk_process_is_up")
+
     def connect_nvme(self, ip, port, nqn):
         params = {
             "ip": ip,
             "port": port,
             "nqn": nqn}
         return self._request("POST", "cnode/nvme_connect", params)
```

## Comparing `sbcli_release-1.1.0/simplyblock_core/pci_utils.py` & `sbcli_release-1.1.2/simplyblock_core/pci_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/snode_client.py` & `sbcli_release-1.1.2/simplyblock_core/snode_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/kv_store.py` & `sbcli_release-1.1.2/simplyblock_core/kv_store.py`

 * *Files 2% similar despite different names*

```diff
@@ -177,14 +177,19 @@
             return ret[0]
 
     def get_lvol_by_id(self, id):
         ret = LVol().read_from_db(self.kv_store, id)
         if ret:
             return ret[0]
 
+    def get_lvol_by_name(self, lvol_name):
+        for lvol in self.get_lvols():
+            if lvol.lvol_name == lvol_name:
+                return lvol
+
     def get_mgmt_node_by_id(self, id):
         ret = MgmtNode().read_from_db(self.kv_store, id)
         if ret:
             return ret[0]
 
     def get_mgmt_nodes(self, cluster_id=None):
         return MgmtNode().read_from_db(self.kv_store)
```

## Comparing `sbcli_release-1.1.0/simplyblock_core/utils.py` & `sbcli_release-1.1.2/simplyblock_core/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/cluster_ops.py` & `sbcli_release-1.1.2/simplyblock_core/cluster_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/compute_node_ops.py` & `sbcli_release-1.1.2/simplyblock_core/compute_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/rpc_client.py` & `sbcli_release-1.1.2/simplyblock_core/rpc_client.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/distr_controller.py` & `sbcli_release-1.1.2/simplyblock_core/distr_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/services/lvol_monitor.py` & `sbcli_release-1.1.2/simplyblock_core/services/lvol_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/services/caching_node_monitor.py` & `sbcli_release-1.1.2/simplyblock_core/services/caching_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/services/health_check_service.py` & `sbcli_release-1.1.2/simplyblock_core/services/health_check_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/services/lvol_stat_collector.py` & `sbcli_release-1.1.2/simplyblock_core/services/lvol_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/services/log_agg_service.py` & `sbcli_release-1.1.2/simplyblock_core/services/log_agg_service.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/services/distr_event_collector.py` & `sbcli_release-1.1.2/simplyblock_core/services/distr_event_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/services/capacity_and_stats_collector.py` & `sbcli_release-1.1.2/simplyblock_core/services/capacity_and_stats_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/services/port_stat_collector.py` & `sbcli_release-1.1.2/simplyblock_core/services/port_stat_collector.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/services/device_monitor.py` & `sbcli_release-1.1.2/simplyblock_core/services/device_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/services/__init__.py` & `sbcli_release-1.1.2/simplyblock_core/services/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/services/install_service.sh` & `sbcli_release-1.1.2/simplyblock_core/services/install_service.sh`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/services/mgmt_node_monitor.py` & `sbcli_release-1.1.2/simplyblock_core/services/mgmt_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/services/cap_monitor.py` & `sbcli_release-1.1.2/simplyblock_core/services/cap_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/services/storage_node_monitor.py` & `sbcli_release-1.1.2/simplyblock_core/services/storage_node_monitor.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/scripts/deploy_stack.sh` & `sbcli_release-1.1.2/simplyblock_core/scripts/deploy_stack.sh`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/scripts/haproxy.cfg` & `sbcli_release-1.1.2/simplyblock_core/scripts/haproxy.cfg`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/scripts/docker-compose-swarm.yml` & `sbcli_release-1.1.2/simplyblock_core/scripts/docker-compose-swarm.yml`

 * *Files 2% similar despite different names*

```diff
@@ -185,15 +185,26 @@
     deploy:
       placement:
         constraints: [node.role == manager]
     volumes:
       - "/etc/foundationdb:/etc/foundationdb"
     networks:
       - hostnet
-
+  CleanupFDB:
+    image: $SIMPLYBLOCK_DOCKER_IMAGE
+    environment:
+      LOG_DELETION_INTERVAL: "${LOG_DELETION_INTERVAL}"
+    command: "python simplyblock_core/workers/cleanup_foundationdb.py"
+    deploy:
+      placement:
+        constraints: [node.role == manager]
+    volumes:
+      - "/etc/foundationdb:/etc/foundationdb"
+    networks:
+      - hostnet
 volumes:
   os_data:
 
 networks:
   hostnet:
     external: true
     name: host
```

## Comparing `sbcli_release-1.1.0/simplyblock_core/scripts/stack_deploy_wait.sh` & `sbcli_release-1.1.2/simplyblock_core/scripts/stack_deploy_wait.sh`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml` & `sbcli_release-1.1.2/simplyblock_core/scripts/docker-compose-swarm-monitoring.yml`

 * *Files 2% similar despite different names*

```diff
@@ -93,15 +93,14 @@
       - /proc:/host/proc:ro
       - /sys:/host/sys:ro
       - /:/rootfs:ro
     command:
       - '--path.procfs=/host/proc'
       - '--path.sysfs=/host/sys'
       - '--path.rootfs=/host'
-      - '--collector.textfile.directory=/etc/node-exporter/'
       - '--collector.filesystem.ignored-mount-points="^(/rootfs|/host|)/(sys|proc|dev|host|etc)($$|/)"'
       - '--collector.filesystem.ignored-fs-types="^(sys|proc|auto|cgroup|devpts|ns|au|fuse\.lxc|mqueue)(fs|)$$"'
       - '--no-collector.ipvs'
     restart: "always"
     deploy:
       mode: global
       placement:
```

## Comparing `sbcli_release-1.1.0/simplyblock_core/scripts/__init__.py` & `sbcli_release-1.1.2/simplyblock_core/scripts/__init__.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/scripts/install_deps.sh` & `sbcli_release-1.1.2/simplyblock_core/scripts/install_deps.sh`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/scripts/apply_dashboard.sh` & `sbcli_release-1.1.2/simplyblock_core/scripts/apply_dashboard.sh`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/scripts/alerting/alert_rules.yaml` & `sbcli_release-1.1.2/simplyblock_core/scripts/alerting/alert_rules.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/scripts/alerting/alert_resources.yaml` & `sbcli_release-1.1.2/simplyblock_core/scripts/alerting/alert_resources.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/devices.json` & `sbcli_release-1.1.2/simplyblock_core/scripts/dashboards/devices.json`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/node-exporter.json` & `sbcli_release-1.1.2/simplyblock_core/scripts/dashboards/node-exporter.json`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/nodes.json` & `sbcli_release-1.1.2/simplyblock_core/scripts/dashboards/nodes.json`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/lvols.json` & `sbcli_release-1.1.2/simplyblock_core/scripts/dashboards/lvols.json`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/cluster.json` & `sbcli_release-1.1.2/simplyblock_core/scripts/dashboards/cluster.json`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/scripts/dashboards/pools.json` & `sbcli_release-1.1.2/simplyblock_core/scripts/dashboards/pools.json`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/controllers/device_controller.py` & `sbcli_release-1.1.2/simplyblock_core/controllers/device_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/controllers/mgmt_events.py` & `sbcli_release-1.1.2/simplyblock_core/controllers/mgmt_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/controllers/events_controller.py` & `sbcli_release-1.1.2/simplyblock_core/controllers/events_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/controllers/storage_events.py` & `sbcli_release-1.1.2/simplyblock_core/controllers/storage_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/controllers/lvol_events.py` & `sbcli_release-1.1.2/simplyblock_core/controllers/lvol_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/controllers/snapshot_controller.py` & `sbcli_release-1.1.2/simplyblock_core/controllers/snapshot_controller.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -133,22 +133,22 @@
     # creating RPCClient instance
     rpc_client = RPCClient(
         snode.mgmt_ip,
         snode.rpc_port,
         snode.rpc_username,
         snode.rpc_password)
 
-    ret = rpc_client.bdev_distrib_delete(snap.base_bdev)
+    ret = rpc_client.ultra21_lvol_dismount(snap.snap_bdev)
     if not ret:
-        logger.error(f"Failed to delete BDev {snap.base_bdev}")
+        logger.error(f"Failed to delete BDev {snap.snap_bdev}")
         return False
 
-    ret = rpc_client.ultra21_lvol_dismount(snap.snap_bdev)
+    ret = rpc_client.bdev_distrib_delete(snap.base_bdev)
     if not ret:
-        logger.error(f"Failed to delete BDev {snap.snap_bdev}")
+        logger.error(f"Failed to delete BDev {snap.base_bdev}")
         return False
 
     snap.remove(db_controller.kv_store)
 
     base_lvol = db_controller.get_lvol_by_id(snap.lvol.get_id())
     if base_lvol.deleted is True:
         lvol_controller.delete_lvol(base_lvol.get_id())
```

## Comparing `sbcli_release-1.1.0/simplyblock_core/controllers/device_events.py` & `sbcli_release-1.1.2/simplyblock_core/controllers/device_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/controllers/pool_controller.py` & `sbcli_release-1.1.2/simplyblock_core/controllers/pool_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/controllers/cluster_events.py` & `sbcli_release-1.1.2/simplyblock_core/controllers/cluster_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/controllers/caching_node_controller.py` & `sbcli_release-1.1.2/simplyblock_core/controllers/caching_node_controller.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,15 +70,15 @@
                     'cluster_id': snode.cluster_id,
                     'status': 'online'
                 }))
             sequential_number += device_partitions_count
     return devices
 
 
-def add_node(cluster_id, node_ip, iface_name, data_nics_list, spdk_cpu_mask, spdk_mem, spdk_image=None):
+def add_node(cluster_id, node_ip, iface_name, data_nics_list, spdk_cpu_mask, spdk_mem, spdk_image=None, namespace=None):
     db_controller = DBController()
     kv_store = db_controller.kv_store
 
     cluster = db_controller.get_cluster_by_id(cluster_id)
     if not cluster:
         logger.error("Cluster not found: %s", cluster_id)
         return False
@@ -150,19 +150,34 @@
         #     logger.warning(f"Free hugepages are less than 1G: {utils.humanbytes(huge_free)}")
         if not spdk_mem:
             spdk_mem = memory_details['free']
 
     logger.info(f"Trying to set hugepages for: {utils.humanbytes(spdk_mem)}")
     logger.info("Deploying SPDK")
     results, err = snode_api.spdk_process_start(
-        spdk_cpu_mask, spdk_mem, spdk_image, snode.mgmt_ip, snode.rpc_port, snode.rpc_username, snode.rpc_password)
+        spdk_cpu_mask, spdk_mem, spdk_image, snode.mgmt_ip,
+        snode.rpc_port, snode.rpc_username, snode.rpc_password, namespace)
     if not results:
         logger.error(f"Failed to start spdk: {err}")
         return False
-    time.sleep(5)
+
+    retries = 20
+    while retries > 0:
+        resp, _ = snode_api.spdk_process_is_up()
+        if resp:
+            logger.info(f"Pod is up")
+            break
+        else:
+            logger.info("Pod is not running, waiting...")
+            time.sleep(3)
+            retries -= 1
+
+    if retries == 0:
+        logger.error("Pod is not running, exiting")
+        return False
 
     # creating RPCClient instance
     rpc_client = RPCClient(
         snode.mgmt_ip, snode.rpc_port,
         snode.rpc_username, snode.rpc_password,
         timeout=60*5, retry=5)
```

## Comparing `sbcli_release-1.1.0/simplyblock_core/controllers/snapshot_events.py` & `sbcli_release-1.1.2/simplyblock_core/controllers/snapshot_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/controllers/lvol_controller.py` & `sbcli_release-1.1.2/simplyblock_core/controllers/lvol_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -933,19 +933,21 @@
     # ret = rpc_client.alceml_unmap_vuid(name, lvol.vuid)
     # lvol.deletion_status = 'jm_unmapped'
     lvol.write_to_db(db_controller.kv_store)
 
     return True
 
 
-def delete_lvol(uuid, force_delete=False):
-    lvol = db_controller.get_lvol_by_id(uuid)
+def delete_lvol(id_or_name, force_delete=False):
+    lvol = db_controller.get_lvol_by_id(id_or_name)
     if not lvol:
-        logger.error(f"lvol not found: {uuid}")
-        return False
+        lvol = db_controller.get_lvol_by_name(id_or_name)
+        if not lvol:
+            logger.error(f"lvol not found: {id_or_name}")
+            return False
 
     pool = db_controller.get_pool_by_id(lvol.pool_uuid)
     if pool.status == Pool.STATUS_INACTIVE:
         logger.error(f"Pool is disabled")
         return False
 
     logger.debug(lvol)
@@ -956,15 +958,15 @@
         snode.rpc_port,
         snode.rpc_username,
         snode.rpc_password)
 
     # soft delete LVol if it has snapshots
     snaps = db_controller.get_snapshots()
     for snap in snaps:
-        if snap.lvol.get_id() == uuid:
+        if snap.lvol.get_id() == lvol.get_id():
             logger.warning(f"Soft delete LVol that has snapshots. Snapshot:{snap.get_id()}")
             ret = rpc_client.subsystem_delete(lvol.nqn)
             logger.debug(ret)
             lvol.deleted = True
             lvol.write_to_db(db_controller.kv_store)
             return True
 
@@ -979,19 +981,19 @@
     elif lvol.ha_type == "ha":
         for nodes_id in lvol.nodes:
             ret = delete_lvol_from_node(lvol.get_id(), nodes_id)
             if not ret:
                 return False
 
     # remove from storage node
-    snode.lvols.remove(uuid)
+    snode.lvols.remove(lvol.get_id())
     snode.write_to_db(db_controller.kv_store)
 
     # remove from pool
-    pool.lvols.remove(uuid)
+    pool.lvols.remove(lvol.get_id())
     pool.write_to_db(db_controller.kv_store)
 
     lvol.remove(db_controller.kv_store)
 
     # if lvol is clone and snapshot is deleted, then delete snapshot
     if lvol.cloned_from_snap:
         snap = db_controller.get_snapshot_by_id(lvol.cloned_from_snap)
```

## Comparing `sbcli_release-1.1.0/simplyblock_core/controllers/health_controller.py` & `sbcli_release-1.1.2/simplyblock_core/controllers/health_controller.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/controllers/pool_events.py` & `sbcli_release-1.1.2/simplyblock_core/controllers/pool_events.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/models/events.py` & `sbcli_release-1.1.2/simplyblock_core/models/events.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/models/iface.py` & `sbcli_release-1.1.2/simplyblock_core/models/iface.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/models/base_model.py` & `sbcli_release-1.1.2/simplyblock_core/models/base_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/models/lvol_model.py` & `sbcli_release-1.1.2/simplyblock_core/models/lvol_model.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/models/compute_node.py` & `sbcli_release-1.1.2/simplyblock_core/models/compute_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/models/snapshot.py` & `sbcli_release-1.1.2/simplyblock_core/models/snapshot.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/models/pool.py` & `sbcli_release-1.1.2/simplyblock_core/models/pool.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/models/global_settings.py` & `sbcli_release-1.1.2/simplyblock_core/models/global_settings.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/models/port_stat.py` & `sbcli_release-1.1.2/simplyblock_core/models/port_stat.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/models/storage_node.py` & `sbcli_release-1.1.2/simplyblock_core/models/storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/models/stats.py` & `sbcli_release-1.1.2/simplyblock_core/models/stats.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/models/cluster.py` & `sbcli_release-1.1.2/simplyblock_core/models/cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/models/mgmt_node.py` & `sbcli_release-1.1.2/simplyblock_core/models/mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/models/caching_node.py` & `sbcli_release-1.1.2/simplyblock_core/models/caching_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_core/models/nvme_device.py` & `sbcli_release-1.1.2/simplyblock_core/models/nvme_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_web/caching_node_app_k8s.py` & `sbcli_release-1.1.2/simplyblock_web/caching_node_app_k8s.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_web/node_utils.py` & `sbcli_release-1.1.2/simplyblock_web/node_utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_web/snode_app.py` & `sbcli_release-1.1.2/simplyblock_web/snode_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_web/app.py` & `sbcli_release-1.1.2/simplyblock_web/app.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_web/auth_middleware.py` & `sbcli_release-1.1.2/simplyblock_web/auth_middleware.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_web/caching_node_app.py` & `sbcli_release-1.1.2/simplyblock_web/caching_node_app.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_web/utils.py` & `sbcli_release-1.1.2/simplyblock_web/utils.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_web/node_webapp.py` & `sbcli_release-1.1.2/simplyblock_web/node_webapp.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_web/static/delete.py` & `sbcli_release-1.1.2/simplyblock_web/static/delete.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_web/static/deploy.py` & `sbcli_release-1.1.2/simplyblock_web/static/deploy.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_web/static/deploy_spdk.yaml` & `sbcli_release-1.1.2/simplyblock_web/static/deploy_spdk.yaml`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_web/templates/deploy_spdk.yaml.j2` & `sbcli_release-1.1.2/simplyblock_web/templates/deploy_spdk.yaml.j2`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 apiVersion: apps/v1
 kind: Deployment
 metadata:
   name: spdk-deployment-{{ HOSTNAME }}
+  namespace: {{ NAMESPACE }}
 spec:
   replicas: 1
   selector:
     matchLabels:
       app: spdk-app-{{ HOSTNAME }}
   template:
     metadata:
```

## Comparing `sbcli_release-1.1.0/simplyblock_web/blueprints/node_api_caching_docker.py` & `sbcli_release-1.1.2/simplyblock_web/blueprints/node_api_caching_docker.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_web/blueprints/node_api_caching_ks.py` & `sbcli_release-1.1.2/simplyblock_web/blueprints/node_api_caching_ks.py`

 * *Files 2% similar despite different names*

```diff
@@ -40,14 +40,18 @@
     if 'spdk_cpu_mask' in data:
         spdk_cpu_mask = data['spdk_cpu_mask']
     spdk_mem = None
     if 'spdk_mem' in data:
         spdk_mem = data['spdk_mem']
     node_cpu_count = os.cpu_count()
 
+    global namespace
+    if 'namespace' in data:
+        namespace = data['namespace']
+
     if spdk_cpu_mask:
         requested_cpu_count = len(format(int(spdk_cpu_mask, 16), 'b'))
         if requested_cpu_count > node_cpu_count:
             return utils.get_response(
                 False,
                 f"The requested cpu count: {requested_cpu_count} "
                 f"is larger than the node's cpu count: {node_cpu_count}")
```

## Comparing `sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_caching_node.py` & `sbcli_release-1.1.2/simplyblock_web/blueprints/web_api_caching_node.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 #!/usr/bin/env python
 # encoding: utf-8
 
 import logging
+import threading
 
 from flask import Blueprint, request
 
 
 from simplyblock_web import utils
 from simplyblock_core import kv_store
 from simplyblock_core.controllers import caching_node_controller
@@ -30,34 +31,37 @@
     node_ip = cl_data['node_ip']
     iface_name = cl_data['iface_name']
 
     data_nics_list = []
     spdk_cpu_mask = None
     spdk_mem = None
     spdk_image = None
+    namespace = None
 
     if 'spdk_cpu_mask' in cl_data:
         spdk_cpu_mask = cl_data['spdk_cpu_mask']
 
     if 'spdk_mem' in cl_data:
         mem = cl_data['spdk_mem']
         spdk_mem = utils.parse_size(mem)
         if spdk_mem < 1 * 1024 * 1024:
             return utils.get_response_error(f"SPDK memory:{mem} must be larger than 1G", 400)
 
     if 'spdk_image' in cl_data:
         spdk_image = cl_data['spdk_image']
 
-    if 'spdk_image' in cl_data:
-        spdk_image = cl_data['spdk_image']
+    if 'namespace' in cl_data:
+        namespace = cl_data['namespace']
 
-    ret = caching_node_controller.add_node(
-        cluster_id, node_ip, iface_name, data_nics_list, spdk_cpu_mask, spdk_mem, spdk_image)
+    t = threading.Thread(
+        target=caching_node_controller.add_node,
+        args=(cluster_id, node_ip, iface_name, data_nics_list, spdk_cpu_mask, spdk_mem, spdk_image, namespace))
+    t.start()
 
-    return utils.get_response(ret)
+    return utils.get_response(True)
 
 
 @bp.route('/cachingnode', methods=['GET'], defaults={'uuid': None})
 @bp.route('/cachingnode/<string:uuid>', methods=['GET'])
 def list_caching_nodes(uuid):
     if uuid:
         node = db_controller.get_caching_node_by_id(uuid)
```

## Comparing `sbcli_release-1.1.0/simplyblock_web/blueprints/snode_ops.py` & `sbcli_release-1.1.2/simplyblock_web/blueprints/snode_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_lvol.py` & `sbcli_release-1.1.2/simplyblock_web/blueprints/web_api_lvol.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_web/blueprints/csi.py` & `sbcli_release-1.1.2/simplyblock_web/blueprints/csi.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_web/blueprints/caching_node_ops.py` & `sbcli_release-1.1.2/simplyblock_web/blueprints/caching_node_ops.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_mgmt_node.py` & `sbcli_release-1.1.2/simplyblock_web/blueprints/web_api_mgmt_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_storage_node.py` & `sbcli_release-1.1.2/simplyblock_web/blueprints/web_api_storage_node.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_web/blueprints/caching_node_ops_k8s.py` & `sbcli_release-1.1.2/simplyblock_web/blueprints/caching_node_ops_k8s.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 #!/usr/bin/env python
 # encoding: utf-8
 import logging
 import math
 import os
 import time
+import traceback
 
 import cpuinfo
 import yaml
 from kubernetes import client, config
 from flask import Blueprint
 from flask import request
 from kubernetes.client import ApiException
@@ -20,15 +21,16 @@
 logger = logging.getLogger(__name__)
 logger.setLevel(logging.DEBUG)
 bp = Blueprint("caching_node_k", __name__, url_prefix="/cnode")
 
 
 node_name = os.environ.get("HOSTNAME")
 deployment_name = f"spdk-deployment-{node_name}"
-namespace = 'default'
+default_namespace = 'default'
+namespace_id_file = '/etc/simplyblock/namespace'
 pod_name = 'spdk-deployment'
 
 
 config.load_incluster_config()
 k8s_apps_v1 = client.AppsV1Api()
 k8s_core_v1 = client.CoreV1Api()
 
@@ -41,14 +43,34 @@
 system_id = ""
 try:
     system_id, _, _ = node_utils.run_command("dmidecode -s system-uuid")
 except:
     pass
 
 
+def get_namespace():
+    if os.path.exists(namespace_id_file):
+        with open(namespace_id_file, 'r') as f:
+            out = f.read()
+            return out
+    return default_namespace
+
+
+def set_namespace(namespace):
+    if not os.path.exists(namespace_id_file):
+        try:
+            os.makedirs(os.path.dirname(namespace_id_file), exist_ok=True)
+        except:
+            logger.error(traceback.format_exc())
+            return False
+    with open(namespace_id_file, "w+") as f:
+        f.write(namespace)
+    return True
+
+
 @bp.route('/scan_devices', methods=['GET'])
 def scan_devices():
     run_health_check = request.args.get('run_health_check', default=False, type=bool)
     out = {
         "nvme_devices": node_utils._get_nvme_devices(),
         "nvme_pcie_list": node_utils._get_nvme_pcie_list(),
         "spdk_devices": node_utils._get_spdk_devices(),
@@ -65,14 +87,19 @@
     if 'spdk_cpu_mask' in data:
         spdk_cpu_mask = data['spdk_cpu_mask']
     spdk_mem = None
     if 'spdk_mem' in data:
         spdk_mem = data['spdk_mem']
     node_cpu_count = os.cpu_count()
 
+    namespace = get_namespace()
+    if 'namespace' in data:
+        namespace = data['namespace']
+        set_namespace(namespace)
+
     if spdk_cpu_mask:
         requested_cpu_count = len(format(int(spdk_cpu_mask, 16), 'b'))
         if requested_cpu_count > node_cpu_count:
             return utils.get_response(
                 False,
                 f"The requested cpu count: {requested_cpu_count} "
                 f"is larger than the node's cpu count: {node_cpu_count}")
@@ -91,66 +118,45 @@
     if _is_pod_up():
         logger.info("SPDK deployment found, removing...")
         spdk_process_kill()
 
     node_name = os.environ.get("HOSTNAME")
     logger.debug(f"deploying caching node spdk on worker: {node_name}")
 
-    env = Environment(loader=FileSystemLoader(os.path.join(TOP_DIR, 'templates')), trim_blocks=True, lstrip_blocks=True)
-    template = env.get_template('deploy_spdk.yaml.j2')
-    values = {
-        'SPDK_IMAGE': spdk_image,
-        'SPDK_CPU_MASK': spdk_cpu_mask,
-        'SPDK_MEM': spdk_mem,
-        'SERVER_IP': data['server_ip'],
-        'RPC_PORT': data['rpc_port'],
-        'RPC_USERNAME': data['rpc_username'],
-        'RPC_PASSWORD': data['rpc_password'],
-        'HOSTNAME': node_name,
-    }
-    dep = yaml.safe_load(template.render(values))
-    resp = k8s_apps_v1.create_namespaced_deployment(body=dep, namespace=namespace)
-    logger.info(f"Deployment created: '{resp.metadata.name}'")
-
-    retries = 20
-    while retries > 0:
-        resp = k8s_core_v1.list_namespaced_pod(namespace)
-        new_pod = None
-        for pod in resp.items:
-            if pod.metadata.name.startswith(pod_name):
-                new_pod = pod
-                break
-
-        if not new_pod:
-            logger.info("Container is not running, waiting...")
-            time.sleep(3)
-            retries -= 1
-            continue
-
-        status = new_pod.status.phase
-        logger.info(f"pod: {pod_name} status: {status}")
-
-        if status == "Running":
-            logger.info(f"Container status: {status}")
-            return utils.get_response(True)
-        else:
-            logger.info("Container is not running, waiting...")
-            time.sleep(3)
-            retries -= 1
+    try:
+        env = Environment(loader=FileSystemLoader(os.path.join(TOP_DIR, 'templates')), trim_blocks=True, lstrip_blocks=True)
+        template = env.get_template('deploy_spdk.yaml.j2')
+        values = {
+            'SPDK_IMAGE': spdk_image,
+            'SPDK_CPU_MASK': spdk_cpu_mask,
+            'SPDK_MEM': spdk_mem,
+            'SERVER_IP': data['server_ip'],
+            'RPC_PORT': data['rpc_port'],
+            'RPC_USERNAME': data['rpc_username'],
+            'RPC_PASSWORD': data['rpc_password'],
+            'HOSTNAME': node_name,
+            'NAMESPACE': namespace,
+        }
+        dep = yaml.safe_load(template.render(values))
+        logger.debug(dep)
+        resp = k8s_apps_v1.create_namespaced_deployment(body=dep, namespace=namespace)
+        msg = f"Deployment created: '{resp.metadata.name}' in namespace '{namespace}"
+        logger.info(msg)
+    except:
+        return utils.get_response(False, f"Deployment failed:\n{traceback.format_exc()}")
 
-    return utils.get_response(
-        False, f"Deployment create max retries reached")
+    return utils.get_response(msg)
 
 
 @bp.route('/spdk_process_kill', methods=['GET'])
 def spdk_process_kill():
 
     try:
+        namespace = get_namespace()
         resp = k8s_apps_v1.delete_namespaced_deployment(deployment_name, namespace)
-
         retries = 20
         while retries > 0:
             resp = k8s_core_v1.list_namespaced_pod(namespace)
             found = False
             for pod in resp.items:
                 if pod.metadata.name.startswith(pod_name):
                     found = True
@@ -165,15 +171,15 @@
     except ApiException as e:
         logger.info(e.body)
 
     return utils.get_response(True)
 
 
 def _is_pod_up():
-    resp = k8s_core_v1.list_namespaced_pod(namespace)
+    resp = k8s_core_v1.list_namespaced_pod(get_namespace())
     for pod in resp.items:
         if pod.metadata.name.startswith(pod_name):
             status = pod.status.phase
             if status == "Running":
                 return True
             else:
                 return False
```

## Comparing `sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_device.py` & `sbcli_release-1.1.2/simplyblock_web/blueprints/web_api_device.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_cluster.py` & `sbcli_release-1.1.2/simplyblock_web/blueprints/web_api_cluster.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_web/blueprints/node_api_basic.py` & `sbcli_release-1.1.2/simplyblock_web/blueprints/node_api_basic.py`

 * *Files identical despite different names*

## Comparing `sbcli_release-1.1.0/simplyblock_web/blueprints/web_api_pool.py` & `sbcli_release-1.1.2/simplyblock_web/blueprints/web_api_pool.py`

 * *Files identical despite different names*

