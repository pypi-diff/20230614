# Comparing `tmp/paasta-tools-0.92.0.tar.gz` & `tmp/paasta-tools-0.92.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/paasta-tools-0.92.0.tar", last modified: Thu Jan  2 21:29:45 2020, max compression
+gzip compressed data, was "dist/paasta-tools-0.92.1.tar", last modified: Fri Jan  3 01:32:14 2020, max compression
```

## Comparing `paasta-tools-0.92.0.tar` & `paasta-tools-0.92.1.tar`

### file list

```diff
@@ -1,254 +1,254 @@
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1043 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/requirements-minimal.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      194 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/MANIFEST.in
--rw-rw-r--   0 travis    (2000) travis    (2000)      248 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)     4990 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/README.md
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1550 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/check_kubernetes_api.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2748 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/hacheck.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5710 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/marathon_dashboard.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      248 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/generate_all_deployments
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1697 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/autoscale_all_services.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6614 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/check_oom_events.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5169 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/secret_tools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16184 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/firewall.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6411 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/list_marathon_service_instances.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    72590 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/kubernetes_tools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4765 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/remote_git.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7754 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cassandracluster_tools.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    25316 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/paasta_remote_run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3855 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/spark_tools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    19754 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/long_running_service_tools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5335 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/setup_kubernetes_crd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12175 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/setup_kubernetes_cr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2962 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cleanup_tron_namespaces.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1100 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/am_i_mesos_leader.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    19511 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/paasta_metastatus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35579 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/mesos_tools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4613 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cleanup_kubernetes_cr.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      870 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/paasta_native_serviceinit.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6773 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/flink_tools.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1140 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/check_cassandracluster_services_replication.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools/autoscaling/
--rw-rw-r--   0 travis    (2000) travis    (2000)     4159 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/autoscaling/forecasting.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7807 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/autoscaling/load_boost.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1088 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/autoscaling/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1916 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/autoscaling/ec2_fitness.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/autoscaling/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2333 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/autoscaling/pause_service_autoscaler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    63346 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/autoscaling/autoscaling_cluster_lib.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    38259 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/autoscaling/autoscaling_service_lib.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools/monitoring/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2128 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/monitoring/kill_orphaned_docker_containers.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     6026 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/monitoring/check_capacity.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     5574 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/monitoring/check_synapse_replication.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1494 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/monitoring/check_marathon_has_apps.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      995 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/monitoring/check_mesos_quorum.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1785 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/monitoring/check_mesos_duplicate_frameworks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5455 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/monitoring/check_mesos_outdated_tasks.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1813 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/monitoring/check_mesos_active_frameworks.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      578 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/monitoring/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      106 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/paasta_deploy_tron_jobs
--rw-rw-r--   0 travis    (2000) travis    (2000)     7352 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/paasta_service_config_loader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5348 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/firewall_update.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     9448 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/paasta_maintenance.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4668 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/check_kubernetes_services_replication.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5708 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/oom_logger.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     5758 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/native_mesos_scheduler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6475 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cleanup_kubernetes_jobs.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools/contrib/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2575 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/contrib/mock_patch_checker.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1575 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/contrib/mass-deploy-tag.sh
--rw-rw-r--   0 travis    (2000) travis    (2000)     1884 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/contrib/emit_allocated_cpu_metrics.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     5803 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/contrib/graceful_container_drain.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2342 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/contrib/bounce_log_latency_parser.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1181 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/contrib/create_dynamodb_table.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3155 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/contrib/delete_old_marathon_deployments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      138 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/contrib/README.md
--rwxrwxr-x   0 travis    (2000) travis    (2000)      525 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/contrib/check_deployd_leader_election.sh
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2108 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/contrib/utilization_check.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/contrib/check_registered_slaves_aws.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2317 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/contrib/get_running_task_allocation.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2480 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/contrib/shared_ip_check.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7036 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/contrib/check_orphans.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3861 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/contrib/kill_bad_containers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1315 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/contrib/is_pod_healthy_in_smartstack.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     9948 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/contrib/paasta_update_soa_memcpu.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      715 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/contrib/paasta_get_num_deployments.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4190 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cleanup_kubernetes_crd.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4994 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/paasta_cluster_boost.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools/mesos/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2199 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/mesos/util.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1453 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/mesos/cfg.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2985 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/mesos/task.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1355 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/mesos/exceptions.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1949 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/mesos/parallel.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1158 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/mesos/zookeeper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2029 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/mesos/framework.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10338 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/mesos/master.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/mesos/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3993 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/mesos/slave.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5366 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/mesos/mesos_file.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2201 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/mesos/cluster.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1488 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/mesos/log.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4054 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/paasta_execute_docker_command.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools/api/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools/api/views/
--rw-rw-r--   0 travis    (2000) travis    (2000)     1204 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/api/views/marathon_dashboard.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1367 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/api/views/service.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    39896 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/api/views/instance.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2755 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/api/views/resources.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1457 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/api/views/exception.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3944 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/api/views/autoscaler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      841 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/api/views/version.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      578 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/api/views/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2278 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/api/views/pause_autoscaler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      975 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/api/views/metastatus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4975 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/api/auth_decorator.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools/api/api_docs/
--rw-rw-r--   0 travis    (2000) travis    (2000)    52273 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/api/api_docs/swagger.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     6780 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/api/api.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      578 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/api/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1348 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/api/settings.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4796 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/api/client.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      886 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/get_mesos_leader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)   115069 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    25198 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/tron_tools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1331 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/mac_address.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4593 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/generate_services_file.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1448 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/synapse_srv_namespaces_fact.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1927 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/dump_locally_running_services.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      896 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/generate_services_yaml.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1586 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/run-paasta-api-in-dev-mode.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    30677 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/mesos_maintenance.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     3946 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cleanup_maintenance.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools/deployd/
--rwxrwxr-x   0 travis    (2000) travis    (2000)    17046 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/deployd/watchers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8619 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/deployd/queue.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8316 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/deployd/common.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4472 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/deployd/metrics.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2591 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/deployd/leader.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6655 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/deployd/workers.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    10497 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/deployd/master.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/deployd/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     8573 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/check_services_replication_tools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15942 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/bounce_lib.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    20156 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/monitoring_tools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3484 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/async_utils.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools/tron/
--rw-rw-r--   0 travis    (2000) travis    (2000)     5385 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/tron/tron_command_context.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/tron/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3063 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/tron/tron_timeutils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3960 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/tron/client.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools/frameworks/
--rw-rw-r--   0 travis    (2000) travis    (2000)     9731 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/frameworks/native_service_config.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24434 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/frameworks/native_scheduler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2821 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/frameworks/adhoc_scheduler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/frameworks/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8537 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/frameworks/task_store.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3035 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/frameworks/constraints.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4813 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/check_marathon_services_replication.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools/cli/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/
--rw-rw-r--   0 travis    (2000) travis    (2000)    31767 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/spark_run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2435 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/security_check.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    40152 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/local_run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    13130 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/check.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2526 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/get_latest_deployment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2972 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/performance_check.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3931 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/cook_image.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    16268 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/validate.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    10202 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/remote_run.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7186 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/push_to_registry.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8776 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/secret.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    12007 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/start_stop_restart.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    48361 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/logs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1964 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/list.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7879 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/wait_for_deployment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1601 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/list_clusters.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    53227 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/mark_for_deployment.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     9300 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/rollback.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3188 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/autoscale.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      578 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3733 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/itest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     3558 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/pause_service_autoscaler.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2735 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/get_docker_image.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5945 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/info.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4549 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/sysdig.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    52952 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/status.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4644 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/boost.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     8274 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cmds/metastatus.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      929 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/paasta_tabcomplete.sh
--rwxrwxr-x   0 travis    (2000) travis    (2000)     5623 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/cli.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    35926 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/utils.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4249 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/fsm_cmd.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      578 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools/cli/schemas/
--rw-rw-r--   0 travis    (2000) travis    (2000)    12744 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/schemas/marathon_schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     3271 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/schemas/adhoc_schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)    19818 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/schemas/kubernetes_schema.json
--rw-rw-r--   0 travis    (2000) travis    (2000)     9907 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/schemas/tron_schema.json
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools/cli/fsm/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2757 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/fsm/autosuggest.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      578 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/fsm/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools/cli/fsm/template/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/
--rw-rw-r--   0 travis    (2000) travis    (2000)      739 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/monitoring.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)     4069 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/marathon-PROD.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      319 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/service.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)       52 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/smartstack.yaml
--rw-rw-r--   0 travis    (2000) travis    (2000)      277 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/fsm/template/README.md
--rw-rw-r--   0 travis    (2000) travis    (2000)      144 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cli/fsm/template/cookiecutter.json
--rwxrwxr-x   0 travis    (2000) travis    (2000)    10833 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/docker_wrapper.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1201 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/deployment_utils.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)      108 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/deploy_marathon_services
--rwxrwxr-x   0 travis    (2000) travis    (2000)    10357 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/generate_deployments_for_service.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       66 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/py.typed
--rw-rw-r--   0 travis    (2000) travis    (2000)    63073 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/marathon_tools.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools/secret_providers/
--rw-rw-r--   0 travis    (2000) travis    (2000)     6205 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/secret_providers/vault.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     1531 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/secret_providers/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      865 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     5542 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/kafkacluster_tools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     2700 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/slack.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6571 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/setup_kubernetes_job.py
--rw-rw-r--   0 travis    (2000) travis    (2000)      690 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/clusterman.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     7519 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/cleanup_marathon_jobs.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)    40479 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/setup_marathon_job.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7518 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/iptables.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4909 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/adhoc_tools.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2191 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/autoscale_cluster.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools/kubernetes/
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools/kubernetes/application/
--rw-rw-r--   0 travis    (2000) travis    (2000)     2783 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/kubernetes/application/tools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    15783 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/kubernetes/application/controller_wrappers.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/kubernetes/application/__init__.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools/kubernetes/bin/
--rwxrwxr-x   0 travis    (2000) travis    (2000)     7219 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/kubernetes/bin/paasta_secrets_sync.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/kubernetes/bin/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     5259 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/kubernetes/bin/kubernetes_remove_evicted_pods.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     6310 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/kubernetes/bin/paasta_cleanup_stale_nodes.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/kubernetes/__init__.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    24963 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/smartstack_tools.py
--rw-rw-r--   0 travis    (2000) travis    (2000)    12724 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/drain_lib.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     7250 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/check_spark_jobs.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4183 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/firewall_logging.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     2399 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/list_kubernetes_service_instances.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools/metrics/
--rwxrwxr-x   0 travis    (2000) travis    (2000)    38811 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/metrics/metastatus_lib.py
--rw-rw-r--   0 travis    (2000) travis    (2000)     4063 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/metrics/metrics_lib.py
--rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/metrics/__init__.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4690 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/setup_tron_namespace.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     1450 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/list_tron_namespaces.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     4355 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/graceful_app_drain.py
--rwxrwxr-x   0 travis    (2000) travis    (2000)     5835 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/paasta_tools/check_flink_services_health.py
--rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/setup.cfg
--rw-rw-r--   0 travis    (2000) travis    (2000)      315 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/pyproject.toml
--rw-rw-r--   0 travis    (2000) travis    (2000)     5084 2020-01-02 21:07:37.000000 paasta-tools-0.92.0/setup.py
-drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools.egg-info/
--rw-rw-r--   0 travis    (2000) travis    (2000)      248 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools.egg-info/PKG-INFO
--rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)       13 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools.egg-info/top_level.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     8635 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)      864 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools.egg-info/requires.txt
--rw-rw-r--   0 travis    (2000) travis    (2000)     1110 2020-01-02 21:29:45.000000 paasta-tools-0.92.0/paasta_tools.egg-info/entry_points.txt
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1043 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/requirements-minimal.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      194 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/MANIFEST.in
+-rw-rw-r--   0 travis    (2000) travis    (2000)      248 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4990 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/README.md
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1550 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/check_kubernetes_api.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2748 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/hacheck.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5710 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/marathon_dashboard.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      248 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/generate_all_deployments
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1697 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/autoscale_all_services.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6614 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/check_oom_events.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5169 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/secret_tools.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16184 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/firewall.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     6411 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/list_marathon_service_instances.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    72590 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/kubernetes_tools.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4765 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/remote_git.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7754 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cassandracluster_tools.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    25316 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/paasta_remote_run.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3855 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/spark_tools.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19754 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/long_running_service_tools.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5335 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/setup_kubernetes_crd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12175 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/setup_kubernetes_cr.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2962 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cleanup_tron_namespaces.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1100 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/am_i_mesos_leader.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    19511 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/paasta_metastatus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35579 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/mesos_tools.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4613 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cleanup_kubernetes_cr.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      870 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/paasta_native_serviceinit.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6773 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/flink_tools.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1140 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/check_cassandracluster_services_replication.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools/autoscaling/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4159 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/autoscaling/forecasting.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7807 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/autoscaling/load_boost.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1088 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/autoscaling/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1916 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/autoscaling/ec2_fitness.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/autoscaling/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2333 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/autoscaling/pause_service_autoscaler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    63346 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/autoscaling/autoscaling_cluster_lib.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    38259 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/autoscaling/autoscaling_service_lib.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools/monitoring/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2128 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/monitoring/kill_orphaned_docker_containers.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     6026 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/monitoring/check_capacity.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     5574 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/monitoring/check_synapse_replication.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1494 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/monitoring/check_marathon_has_apps.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      995 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/monitoring/check_mesos_quorum.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1785 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/monitoring/check_mesos_duplicate_frameworks.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5455 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/monitoring/check_mesos_outdated_tasks.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1813 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/monitoring/check_mesos_active_frameworks.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      578 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/monitoring/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      106 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/paasta_deploy_tron_jobs
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7352 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/paasta_service_config_loader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5348 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/firewall_update.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     9448 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/paasta_maintenance.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4668 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/check_kubernetes_services_replication.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5708 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/oom_logger.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     5758 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/native_mesos_scheduler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6475 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cleanup_kubernetes_jobs.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools/contrib/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2575 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/contrib/mock_patch_checker.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1575 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/contrib/mass-deploy-tag.sh
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1884 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/contrib/emit_allocated_cpu_metrics.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     5803 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/contrib/graceful_container_drain.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2342 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/contrib/bounce_log_latency_parser.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1181 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/contrib/create_dynamodb_table.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3155 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/contrib/delete_old_marathon_deployments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      138 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/contrib/README.md
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      525 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/contrib/check_deployd_leader_election.sh
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2108 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/contrib/utilization_check.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2941 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/contrib/check_registered_slaves_aws.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2317 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/contrib/get_running_task_allocation.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2480 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/contrib/shared_ip_check.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7036 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/contrib/check_orphans.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3861 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/contrib/kill_bad_containers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1315 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/contrib/is_pod_healthy_in_smartstack.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     9948 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/contrib/paasta_update_soa_memcpu.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      715 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/contrib/paasta_get_num_deployments.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4190 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cleanup_kubernetes_crd.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4994 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/paasta_cluster_boost.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools/mesos/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2199 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/mesos/util.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1453 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/mesos/cfg.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2985 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/mesos/task.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1355 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/mesos/exceptions.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1949 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/mesos/parallel.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1158 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/mesos/zookeeper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2029 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/mesos/framework.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10338 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/mesos/master.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/mesos/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3993 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/mesos/slave.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5366 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/mesos/mesos_file.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2201 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/mesos/cluster.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1488 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/mesos/log.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4054 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/paasta_execute_docker_command.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools/api/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools/api/views/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1204 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/api/views/marathon_dashboard.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1367 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/api/views/service.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    39896 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/api/views/instance.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2755 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/api/views/resources.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1457 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/api/views/exception.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3944 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/api/views/autoscaler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      841 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/api/views/version.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      578 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/api/views/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2278 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/api/views/pause_autoscaler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      975 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/api/views/metastatus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4975 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/api/auth_decorator.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools/api/api_docs/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    52273 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/api/api_docs/swagger.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6780 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/api/api.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      578 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/api/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1348 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/api/settings.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4796 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/api/client.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      886 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/get_mesos_leader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)   115069 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    25198 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/tron_tools.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1331 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/mac_address.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4593 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/generate_services_file.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1448 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/synapse_srv_namespaces_fact.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1927 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/dump_locally_running_services.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      896 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/generate_services_yaml.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1586 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/run-paasta-api-in-dev-mode.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    30677 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/mesos_maintenance.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     3946 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cleanup_maintenance.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools/deployd/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    17046 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/deployd/watchers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8619 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/deployd/queue.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8316 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/deployd/common.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4472 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/deployd/metrics.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2591 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/deployd/leader.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6655 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/deployd/workers.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    10497 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/deployd/master.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/deployd/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     8573 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/check_services_replication_tools.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15942 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/bounce_lib.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    20156 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/monitoring_tools.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3484 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/async_utils.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools/tron/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5385 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/tron/tron_command_context.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/tron/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3063 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/tron/tron_timeutils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3960 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/tron/client.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools/frameworks/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9731 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/frameworks/native_service_config.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24434 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/frameworks/native_scheduler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2821 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/frameworks/adhoc_scheduler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/frameworks/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8537 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/frameworks/task_store.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3035 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/frameworks/constraints.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4813 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/check_marathon_services_replication.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools/cli/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    32079 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/spark_run.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2435 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/security_check.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    40152 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/local_run.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    13130 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/check.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2526 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/get_latest_deployment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2972 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/performance_check.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3931 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/cook_image.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    16268 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/validate.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    10202 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/remote_run.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7186 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/push_to_registry.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8776 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/secret.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    12007 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/start_stop_restart.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    48361 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/logs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1964 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/list.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7879 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/wait_for_deployment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1601 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/list_clusters.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    53227 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/mark_for_deployment.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9300 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/rollback.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3188 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/autoscale.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      578 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3733 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/itest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3558 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/pause_service_autoscaler.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2735 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/get_docker_image.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5945 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/info.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4549 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/sysdig.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    52952 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/status.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4644 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/boost.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8274 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cmds/metastatus.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      929 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/paasta_tabcomplete.sh
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     5623 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/cli.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    35926 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/utils.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4249 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/fsm_cmd.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      578 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools/cli/schemas/
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12744 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/schemas/marathon_schema.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     3271 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/schemas/adhoc_schema.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)    19818 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/schemas/kubernetes_schema.json
+-rw-rw-r--   0 travis    (2000) travis    (2000)     9907 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/schemas/tron_schema.json
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools/cli/fsm/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2757 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/fsm/autosuggest.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      578 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/fsm/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools/cli/fsm/template/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      739 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/monitoring.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4069 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/marathon-PROD.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      319 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/service.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)       52 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/smartstack.yaml
+-rw-rw-r--   0 travis    (2000) travis    (2000)      277 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/fsm/template/README.md
+-rw-rw-r--   0 travis    (2000) travis    (2000)      144 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cli/fsm/template/cookiecutter.json
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    10833 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/docker_wrapper.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1201 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/deployment_utils.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)      108 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/deploy_marathon_services
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    10357 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/generate_deployments_for_service.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       66 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/py.typed
+-rw-rw-r--   0 travis    (2000) travis    (2000)    63073 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/marathon_tools.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools/secret_providers/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6205 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/secret_providers/vault.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1531 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/secret_providers/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      865 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5542 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/kafkacluster_tools.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2700 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/slack.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6571 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/setup_kubernetes_job.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)      690 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/clusterman.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     7519 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/cleanup_marathon_jobs.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    40479 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/setup_marathon_job.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7518 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/iptables.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4909 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/adhoc_tools.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2191 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/autoscale_cluster.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools/kubernetes/
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools/kubernetes/application/
+-rw-rw-r--   0 travis    (2000) travis    (2000)     2783 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/kubernetes/application/tools.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    15783 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/kubernetes/application/controller_wrappers.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/kubernetes/application/__init__.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools/kubernetes/bin/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     7219 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/kubernetes/bin/paasta_secrets_sync.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/kubernetes/bin/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     5259 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/kubernetes/bin/kubernetes_remove_evicted_pods.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     6310 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/kubernetes/bin/paasta_cleanup_stale_nodes.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/kubernetes/__init__.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    24963 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/smartstack_tools.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)    12724 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/drain_lib.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     7250 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/check_spark_jobs.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4183 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/firewall_logging.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     2399 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/list_kubernetes_service_instances.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools/metrics/
+-rwxrwxr-x   0 travis    (2000) travis    (2000)    38811 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/metrics/metastatus_lib.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)     4063 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/metrics/metrics_lib.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)        0 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/metrics/__init__.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4690 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/setup_tron_namespace.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     1450 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/list_tron_namespaces.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     4355 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/graceful_app_drain.py
+-rwxrwxr-x   0 travis    (2000) travis    (2000)     5835 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/paasta_tools/check_flink_services_health.py
+-rw-rw-r--   0 travis    (2000) travis    (2000)       38 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/setup.cfg
+-rw-rw-r--   0 travis    (2000) travis    (2000)      315 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/pyproject.toml
+-rw-rw-r--   0 travis    (2000) travis    (2000)     5084 2020-01-03 01:10:29.000000 paasta-tools-0.92.1/setup.py
+drwxrwxr-x   0 travis    (2000) travis    (2000)        0 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools.egg-info/
+-rw-rw-r--   0 travis    (2000) travis    (2000)      248 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 travis    (2000) travis    (2000)        1 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)       13 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools.egg-info/top_level.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     8635 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)      864 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools.egg-info/requires.txt
+-rw-rw-r--   0 travis    (2000) travis    (2000)     1110 2020-01-03 01:32:14.000000 paasta-tools-0.92.1/paasta_tools.egg-info/entry_points.txt
```

### Comparing `paasta-tools-0.92.0/requirements-minimal.txt` & `paasta-tools-0.92.1/requirements-minimal.txt`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/README.md` & `paasta-tools-0.92.1/README.md`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/check_kubernetes_api.py` & `paasta-tools-0.92.1/paasta_tools/check_kubernetes_api.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/hacheck.py` & `paasta-tools-0.92.1/paasta_tools/hacheck.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/marathon_dashboard.py` & `paasta-tools-0.92.1/paasta_tools/marathon_dashboard.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/autoscale_all_services.py` & `paasta-tools-0.92.1/paasta_tools/autoscale_all_services.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/check_oom_events.py` & `paasta-tools-0.92.1/paasta_tools/check_oom_events.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/secret_tools.py` & `paasta-tools-0.92.1/paasta_tools/secret_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/firewall.py` & `paasta-tools-0.92.1/paasta_tools/firewall.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/list_marathon_service_instances.py` & `paasta-tools-0.92.1/paasta_tools/list_marathon_service_instances.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/kubernetes_tools.py` & `paasta-tools-0.92.1/paasta_tools/kubernetes_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/remote_git.py` & `paasta-tools-0.92.1/paasta_tools/remote_git.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cassandracluster_tools.py` & `paasta-tools-0.92.1/paasta_tools/cassandracluster_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/paasta_remote_run.py` & `paasta-tools-0.92.1/paasta_tools/paasta_remote_run.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/spark_tools.py` & `paasta-tools-0.92.1/paasta_tools/spark_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/long_running_service_tools.py` & `paasta-tools-0.92.1/paasta_tools/long_running_service_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/setup_kubernetes_crd.py` & `paasta-tools-0.92.1/paasta_tools/setup_kubernetes_crd.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/setup_kubernetes_cr.py` & `paasta-tools-0.92.1/paasta_tools/setup_kubernetes_cr.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cleanup_tron_namespaces.py` & `paasta-tools-0.92.1/paasta_tools/cleanup_tron_namespaces.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/am_i_mesos_leader.py` & `paasta-tools-0.92.1/paasta_tools/am_i_mesos_leader.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/paasta_metastatus.py` & `paasta-tools-0.92.1/paasta_tools/paasta_metastatus.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/mesos_tools.py` & `paasta-tools-0.92.1/paasta_tools/mesos_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cleanup_kubernetes_cr.py` & `paasta-tools-0.92.1/paasta_tools/cleanup_kubernetes_cr.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/paasta_native_serviceinit.py` & `paasta-tools-0.92.1/paasta_tools/paasta_native_serviceinit.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/flink_tools.py` & `paasta-tools-0.92.1/paasta_tools/flink_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/check_cassandracluster_services_replication.py` & `paasta-tools-0.92.1/paasta_tools/check_cassandracluster_services_replication.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/autoscaling/forecasting.py` & `paasta-tools-0.92.1/paasta_tools/autoscaling/forecasting.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/autoscaling/load_boost.py` & `paasta-tools-0.92.1/paasta_tools/autoscaling/load_boost.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/autoscaling/utils.py` & `paasta-tools-0.92.1/paasta_tools/autoscaling/utils.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/autoscaling/ec2_fitness.py` & `paasta-tools-0.92.1/paasta_tools/autoscaling/ec2_fitness.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/autoscaling/pause_service_autoscaler.py` & `paasta-tools-0.92.1/paasta_tools/autoscaling/pause_service_autoscaler.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/autoscaling/autoscaling_cluster_lib.py` & `paasta-tools-0.92.1/paasta_tools/autoscaling/autoscaling_cluster_lib.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/autoscaling/autoscaling_service_lib.py` & `paasta-tools-0.92.1/paasta_tools/autoscaling/autoscaling_service_lib.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/monitoring/kill_orphaned_docker_containers.py` & `paasta-tools-0.92.1/paasta_tools/monitoring/kill_orphaned_docker_containers.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/monitoring/check_capacity.py` & `paasta-tools-0.92.1/paasta_tools/monitoring/check_capacity.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/monitoring/check_synapse_replication.py` & `paasta-tools-0.92.1/paasta_tools/monitoring/check_synapse_replication.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/monitoring/check_marathon_has_apps.py` & `paasta-tools-0.92.1/paasta_tools/monitoring/check_marathon_has_apps.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/monitoring/check_mesos_quorum.py` & `paasta-tools-0.92.1/paasta_tools/monitoring/check_mesos_quorum.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/monitoring/check_mesos_duplicate_frameworks.py` & `paasta-tools-0.92.1/paasta_tools/monitoring/check_mesos_duplicate_frameworks.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/monitoring/check_mesos_outdated_tasks.py` & `paasta-tools-0.92.1/paasta_tools/monitoring/check_mesos_outdated_tasks.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/monitoring/check_mesos_active_frameworks.py` & `paasta-tools-0.92.1/paasta_tools/monitoring/check_mesos_active_frameworks.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/monitoring/__init__.py` & `paasta-tools-0.92.1/paasta_tools/monitoring/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/paasta_service_config_loader.py` & `paasta-tools-0.92.1/paasta_tools/paasta_service_config_loader.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/firewall_update.py` & `paasta-tools-0.92.1/paasta_tools/firewall_update.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/paasta_maintenance.py` & `paasta-tools-0.92.1/paasta_tools/paasta_maintenance.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/check_kubernetes_services_replication.py` & `paasta-tools-0.92.1/paasta_tools/check_kubernetes_services_replication.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/oom_logger.py` & `paasta-tools-0.92.1/paasta_tools/oom_logger.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/native_mesos_scheduler.py` & `paasta-tools-0.92.1/paasta_tools/native_mesos_scheduler.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cleanup_kubernetes_jobs.py` & `paasta-tools-0.92.1/paasta_tools/cleanup_kubernetes_jobs.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/contrib/mock_patch_checker.py` & `paasta-tools-0.92.1/paasta_tools/contrib/mock_patch_checker.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/contrib/mass-deploy-tag.sh` & `paasta-tools-0.92.1/paasta_tools/contrib/mass-deploy-tag.sh`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/contrib/emit_allocated_cpu_metrics.py` & `paasta-tools-0.92.1/paasta_tools/contrib/emit_allocated_cpu_metrics.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/contrib/graceful_container_drain.py` & `paasta-tools-0.92.1/paasta_tools/contrib/graceful_container_drain.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/contrib/bounce_log_latency_parser.py` & `paasta-tools-0.92.1/paasta_tools/contrib/bounce_log_latency_parser.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/contrib/create_dynamodb_table.py` & `paasta-tools-0.92.1/paasta_tools/contrib/create_dynamodb_table.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/contrib/delete_old_marathon_deployments.py` & `paasta-tools-0.92.1/paasta_tools/contrib/delete_old_marathon_deployments.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/contrib/check_deployd_leader_election.sh` & `paasta-tools-0.92.1/paasta_tools/contrib/check_deployd_leader_election.sh`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/contrib/utilization_check.py` & `paasta-tools-0.92.1/paasta_tools/contrib/utilization_check.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/contrib/check_registered_slaves_aws.py` & `paasta-tools-0.92.1/paasta_tools/contrib/check_registered_slaves_aws.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/contrib/get_running_task_allocation.py` & `paasta-tools-0.92.1/paasta_tools/contrib/get_running_task_allocation.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/contrib/shared_ip_check.py` & `paasta-tools-0.92.1/paasta_tools/contrib/shared_ip_check.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/contrib/check_orphans.py` & `paasta-tools-0.92.1/paasta_tools/contrib/check_orphans.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/contrib/kill_bad_containers.py` & `paasta-tools-0.92.1/paasta_tools/contrib/kill_bad_containers.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/contrib/is_pod_healthy_in_smartstack.py` & `paasta-tools-0.92.1/paasta_tools/contrib/is_pod_healthy_in_smartstack.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/contrib/paasta_update_soa_memcpu.py` & `paasta-tools-0.92.1/paasta_tools/contrib/paasta_update_soa_memcpu.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/contrib/paasta_get_num_deployments.py` & `paasta-tools-0.92.1/paasta_tools/contrib/paasta_get_num_deployments.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cleanup_kubernetes_crd.py` & `paasta-tools-0.92.1/paasta_tools/cleanup_kubernetes_crd.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/paasta_cluster_boost.py` & `paasta-tools-0.92.1/paasta_tools/paasta_cluster_boost.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/mesos/util.py` & `paasta-tools-0.92.1/paasta_tools/mesos/util.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/mesos/cfg.py` & `paasta-tools-0.92.1/paasta_tools/mesos/cfg.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/mesos/task.py` & `paasta-tools-0.92.1/paasta_tools/mesos/task.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/mesos/exceptions.py` & `paasta-tools-0.92.1/paasta_tools/mesos/exceptions.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/mesos/parallel.py` & `paasta-tools-0.92.1/paasta_tools/mesos/parallel.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/mesos/zookeeper.py` & `paasta-tools-0.92.1/paasta_tools/mesos/zookeeper.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/mesos/framework.py` & `paasta-tools-0.92.1/paasta_tools/mesos/framework.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/mesos/master.py` & `paasta-tools-0.92.1/paasta_tools/mesos/master.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/mesos/slave.py` & `paasta-tools-0.92.1/paasta_tools/mesos/slave.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/mesos/mesos_file.py` & `paasta-tools-0.92.1/paasta_tools/mesos/mesos_file.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/mesos/cluster.py` & `paasta-tools-0.92.1/paasta_tools/mesos/cluster.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/mesos/log.py` & `paasta-tools-0.92.1/paasta_tools/mesos/log.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/paasta_execute_docker_command.py` & `paasta-tools-0.92.1/paasta_tools/paasta_execute_docker_command.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/api/views/marathon_dashboard.py` & `paasta-tools-0.92.1/paasta_tools/api/views/marathon_dashboard.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/api/views/service.py` & `paasta-tools-0.92.1/paasta_tools/api/views/service.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/api/views/instance.py` & `paasta-tools-0.92.1/paasta_tools/api/views/instance.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/api/views/resources.py` & `paasta-tools-0.92.1/paasta_tools/api/views/resources.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/api/views/exception.py` & `paasta-tools-0.92.1/paasta_tools/api/views/exception.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/api/views/autoscaler.py` & `paasta-tools-0.92.1/paasta_tools/api/views/autoscaler.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/api/views/version.py` & `paasta-tools-0.92.1/paasta_tools/api/views/version.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/api/views/__init__.py` & `paasta-tools-0.92.1/paasta_tools/api/views/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/api/views/pause_autoscaler.py` & `paasta-tools-0.92.1/paasta_tools/api/views/pause_autoscaler.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/api/views/metastatus.py` & `paasta-tools-0.92.1/paasta_tools/api/views/metastatus.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/api/auth_decorator.py` & `paasta-tools-0.92.1/paasta_tools/api/auth_decorator.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/api/api_docs/swagger.json` & `paasta-tools-0.92.1/paasta_tools/api/api_docs/swagger.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/api/api.py` & `paasta-tools-0.92.1/paasta_tools/api/api.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/api/__init__.py` & `paasta-tools-0.92.1/paasta_tools/api/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/api/settings.py` & `paasta-tools-0.92.1/paasta_tools/api/settings.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/api/client.py` & `paasta-tools-0.92.1/paasta_tools/api/client.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/get_mesos_leader.py` & `paasta-tools-0.92.1/paasta_tools/get_mesos_leader.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/utils.py` & `paasta-tools-0.92.1/paasta_tools/utils.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/tron_tools.py` & `paasta-tools-0.92.1/paasta_tools/tron_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/mac_address.py` & `paasta-tools-0.92.1/paasta_tools/mac_address.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/generate_services_file.py` & `paasta-tools-0.92.1/paasta_tools/generate_services_file.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/synapse_srv_namespaces_fact.py` & `paasta-tools-0.92.1/paasta_tools/synapse_srv_namespaces_fact.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/dump_locally_running_services.py` & `paasta-tools-0.92.1/paasta_tools/dump_locally_running_services.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/generate_services_yaml.py` & `paasta-tools-0.92.1/paasta_tools/generate_services_yaml.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/run-paasta-api-in-dev-mode.py` & `paasta-tools-0.92.1/paasta_tools/run-paasta-api-in-dev-mode.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/mesos_maintenance.py` & `paasta-tools-0.92.1/paasta_tools/mesos_maintenance.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cleanup_maintenance.py` & `paasta-tools-0.92.1/paasta_tools/cleanup_maintenance.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/deployd/watchers.py` & `paasta-tools-0.92.1/paasta_tools/deployd/watchers.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/deployd/queue.py` & `paasta-tools-0.92.1/paasta_tools/deployd/queue.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/deployd/common.py` & `paasta-tools-0.92.1/paasta_tools/deployd/common.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/deployd/metrics.py` & `paasta-tools-0.92.1/paasta_tools/deployd/metrics.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/deployd/leader.py` & `paasta-tools-0.92.1/paasta_tools/deployd/leader.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/deployd/workers.py` & `paasta-tools-0.92.1/paasta_tools/deployd/workers.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/deployd/master.py` & `paasta-tools-0.92.1/paasta_tools/deployd/master.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/check_services_replication_tools.py` & `paasta-tools-0.92.1/paasta_tools/check_services_replication_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/bounce_lib.py` & `paasta-tools-0.92.1/paasta_tools/bounce_lib.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/monitoring_tools.py` & `paasta-tools-0.92.1/paasta_tools/monitoring_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/async_utils.py` & `paasta-tools-0.92.1/paasta_tools/async_utils.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/tron/tron_command_context.py` & `paasta-tools-0.92.1/paasta_tools/tron/tron_command_context.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/tron/tron_timeutils.py` & `paasta-tools-0.92.1/paasta_tools/tron/tron_timeutils.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/tron/client.py` & `paasta-tools-0.92.1/paasta_tools/tron/client.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/frameworks/native_service_config.py` & `paasta-tools-0.92.1/paasta_tools/frameworks/native_service_config.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/frameworks/native_scheduler.py` & `paasta-tools-0.92.1/paasta_tools/frameworks/native_scheduler.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/frameworks/adhoc_scheduler.py` & `paasta-tools-0.92.1/paasta_tools/frameworks/adhoc_scheduler.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/frameworks/task_store.py` & `paasta-tools-0.92.1/paasta_tools/frameworks/task_store.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/frameworks/constraints.py` & `paasta-tools-0.92.1/paasta_tools/frameworks/constraints.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/check_marathon_services_replication.py` & `paasta-tools-0.92.1/paasta_tools/check_marathon_services_replication.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/spark_run.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/spark_run.py`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,15 @@
 from paasta_tools.spark_tools import get_aws_credentials
 from paasta_tools.spark_tools import get_default_event_log_dir
 from paasta_tools.spark_tools import load_mesos_secret_for_spark
 from paasta_tools.utils import _run
 from paasta_tools.utils import DEFAULT_SOA_DIR
 from paasta_tools.utils import get_possible_launched_by_user_variable_from_env
 from paasta_tools.utils import get_username
+from paasta_tools.utils import InstanceConfig
 from paasta_tools.utils import list_services
 from paasta_tools.utils import load_system_paasta_config
 from paasta_tools.utils import NoConfigurationForServiceError
 from paasta_tools.utils import NoDeploymentsAvailable
 from paasta_tools.utils import NoDockerImageError
 from paasta_tools.utils import paasta_print
 from paasta_tools.utils import PaastaColors
@@ -603,15 +604,15 @@
         constraints[k] = v
 
     return constraints
 
 
 def run_docker_container(
     container_name, volumes, environment, docker_img, docker_cmd, dry_run, nvidia
-):
+) -> int:
     docker_run_args = dict(
         container_name=container_name,
         volumes=volumes,
         env=environment,
         docker_img=docker_img,
         docker_cmd=docker_cmd,
         nvidia=nvidia,
@@ -623,16 +624,19 @@
         return 0
 
     os.execlpe("paasta_docker_wrapper", *docker_run_cmd)
     return 0
 
 
 def configure_and_run_docker_container(
-    args, docker_img, instance_config, system_paasta_config
-):
+    args: argparse.Namespace,
+    docker_img: str,
+    instance_config: InstanceConfig,
+    system_paasta_config: SystemPaastaConfig,
+) -> int:
     volumes = list()
     for volume in instance_config.get_volumes(system_paasta_config.get_volumes()):
         if os.path.exists(volume["hostPath"]):
             volumes.append(
                 "{}:{}:{}".format(
                     volume["hostPath"], volume["containerPath"], volume["mode"].lower()
                 )
@@ -649,15 +653,20 @@
     spark_ui_port = pick_random_port(args.service + str(os.getpid()))
     spark_app_name = "paasta_spark_run_{}".format(get_username())
     container_name = spark_app_name + "_" + str(spark_ui_port)
     original_docker_cmd = args.cmd or instance_config.get_cmd()
     if "jupyter" not in original_docker_cmd:
         spark_app_name = container_name
 
-    access_key, secret_key = get_aws_credentials(args)
+    access_key, secret_key = get_aws_credentials(
+        service=args.service,
+        no_aws_credentials=args.no_aws_credentials,
+        aws_credentials_yaml=args.aws_credentials_yaml,
+        profile_name=args.aws_profile,
+    )
     spark_config_dict = get_spark_config(
         args=args,
         spark_app_name=spark_app_name,
         spark_ui_port=spark_ui_port,
         docker_img=docker_img,
         system_paasta_config=system_paasta_config,
         volumes=volumes,
```

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/security_check.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/security_check.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/local_run.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/local_run.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/check.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/check.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/get_latest_deployment.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/get_latest_deployment.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/performance_check.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/performance_check.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/cook_image.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/cook_image.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/validate.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/validate.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/remote_run.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/remote_run.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/push_to_registry.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/push_to_registry.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/secret.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/secret.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/start_stop_restart.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/start_stop_restart.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/logs.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/logs.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/list.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/list.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/wait_for_deployment.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/wait_for_deployment.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/list_clusters.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/list_clusters.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/mark_for_deployment.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/mark_for_deployment.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/rollback.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/rollback.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/autoscale.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/autoscale.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/__init__.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/itest.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/itest.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/pause_service_autoscaler.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/pause_service_autoscaler.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/get_docker_image.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/get_docker_image.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/info.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/info.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/sysdig.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/sysdig.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/status.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/status.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/boost.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/boost.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cmds/metastatus.py` & `paasta-tools-0.92.1/paasta_tools/cli/cmds/metastatus.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/paasta_tabcomplete.sh` & `paasta-tools-0.92.1/paasta_tools/cli/paasta_tabcomplete.sh`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/cli.py` & `paasta-tools-0.92.1/paasta_tools/cli/cli.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/utils.py` & `paasta-tools-0.92.1/paasta_tools/cli/utils.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/fsm_cmd.py` & `paasta-tools-0.92.1/paasta_tools/cli/fsm_cmd.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/__init__.py` & `paasta-tools-0.92.1/paasta_tools/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/schemas/marathon_schema.json` & `paasta-tools-0.92.1/paasta_tools/cli/schemas/marathon_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/schemas/adhoc_schema.json` & `paasta-tools-0.92.1/paasta_tools/cli/schemas/adhoc_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/schemas/kubernetes_schema.json` & `paasta-tools-0.92.1/paasta_tools/cli/schemas/kubernetes_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/schemas/tron_schema.json` & `paasta-tools-0.92.1/paasta_tools/cli/schemas/tron_schema.json`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/fsm/autosuggest.py` & `paasta-tools-0.92.1/paasta_tools/cli/fsm/autosuggest.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/fsm/__init__.py` & `paasta-tools-0.92.1/paasta_tools/cli/fsm/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/monitoring.yaml` & `paasta-tools-0.92.1/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/monitoring.yaml`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/marathon-PROD.yaml` & `paasta-tools-0.92.1/paasta_tools/cli/fsm/template/{{cookiecutter.service}}/marathon-PROD.yaml`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/docker_wrapper.py` & `paasta-tools-0.92.1/paasta_tools/docker_wrapper.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/deployment_utils.py` & `paasta-tools-0.92.1/paasta_tools/deployment_utils.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/generate_deployments_for_service.py` & `paasta-tools-0.92.1/paasta_tools/generate_deployments_for_service.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/marathon_tools.py` & `paasta-tools-0.92.1/paasta_tools/marathon_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/secret_providers/vault.py` & `paasta-tools-0.92.1/paasta_tools/secret_providers/vault.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/secret_providers/__init__.py` & `paasta-tools-0.92.1/paasta_tools/secret_providers/__init__.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/__init__.py` & `paasta-tools-0.92.1/paasta_tools/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -13,8 +13,8 @@
 # limitations under the License.
 #
 # It is imperative that this file not contain any imports from our
 # dependencies. Since this file is imported from setup.py in the
 # setup phase, the dependencies may not exist on disk yet.
 #
 # Don't bump version manually. See `make release` docs in ./Makefile
-__version__ = "0.92.0"
+__version__ = "0.92.1"
```

### Comparing `paasta-tools-0.92.0/paasta_tools/kafkacluster_tools.py` & `paasta-tools-0.92.1/paasta_tools/kafkacluster_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/slack.py` & `paasta-tools-0.92.1/paasta_tools/slack.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/setup_kubernetes_job.py` & `paasta-tools-0.92.1/paasta_tools/setup_kubernetes_job.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/clusterman.py` & `paasta-tools-0.92.1/paasta_tools/clusterman.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/cleanup_marathon_jobs.py` & `paasta-tools-0.92.1/paasta_tools/cleanup_marathon_jobs.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/setup_marathon_job.py` & `paasta-tools-0.92.1/paasta_tools/setup_marathon_job.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/iptables.py` & `paasta-tools-0.92.1/paasta_tools/iptables.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/adhoc_tools.py` & `paasta-tools-0.92.1/paasta_tools/adhoc_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/autoscale_cluster.py` & `paasta-tools-0.92.1/paasta_tools/autoscale_cluster.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/kubernetes/application/tools.py` & `paasta-tools-0.92.1/paasta_tools/kubernetes/application/tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/kubernetes/application/controller_wrappers.py` & `paasta-tools-0.92.1/paasta_tools/kubernetes/application/controller_wrappers.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/kubernetes/bin/paasta_secrets_sync.py` & `paasta-tools-0.92.1/paasta_tools/kubernetes/bin/paasta_secrets_sync.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/kubernetes/bin/kubernetes_remove_evicted_pods.py` & `paasta-tools-0.92.1/paasta_tools/kubernetes/bin/kubernetes_remove_evicted_pods.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/kubernetes/bin/paasta_cleanup_stale_nodes.py` & `paasta-tools-0.92.1/paasta_tools/kubernetes/bin/paasta_cleanup_stale_nodes.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/smartstack_tools.py` & `paasta-tools-0.92.1/paasta_tools/smartstack_tools.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/drain_lib.py` & `paasta-tools-0.92.1/paasta_tools/drain_lib.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/check_spark_jobs.py` & `paasta-tools-0.92.1/paasta_tools/check_spark_jobs.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/firewall_logging.py` & `paasta-tools-0.92.1/paasta_tools/firewall_logging.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/list_kubernetes_service_instances.py` & `paasta-tools-0.92.1/paasta_tools/list_kubernetes_service_instances.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/metrics/metastatus_lib.py` & `paasta-tools-0.92.1/paasta_tools/metrics/metastatus_lib.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/metrics/metrics_lib.py` & `paasta-tools-0.92.1/paasta_tools/metrics/metrics_lib.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/setup_tron_namespace.py` & `paasta-tools-0.92.1/paasta_tools/setup_tron_namespace.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/list_tron_namespaces.py` & `paasta-tools-0.92.1/paasta_tools/list_tron_namespaces.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/graceful_app_drain.py` & `paasta-tools-0.92.1/paasta_tools/graceful_app_drain.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools/check_flink_services_health.py` & `paasta-tools-0.92.1/paasta_tools/check_flink_services_health.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/setup.py` & `paasta-tools-0.92.1/setup.py`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools.egg-info/SOURCES.txt` & `paasta-tools-0.92.1/paasta_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools.egg-info/requires.txt` & `paasta-tools-0.92.1/paasta_tools.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `paasta-tools-0.92.0/paasta_tools.egg-info/entry_points.txt` & `paasta-tools-0.92.1/paasta_tools.egg-info/entry_points.txt`

 * *Files identical despite different names*

