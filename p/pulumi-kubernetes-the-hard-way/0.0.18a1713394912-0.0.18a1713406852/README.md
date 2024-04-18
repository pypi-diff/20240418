# Comparing `tmp/pulumi_kubernetes_the_hard_way-0.0.18a1713394912.tar.gz` & `tmp/pulumi_kubernetes_the_hard_way-0.0.18a1713406852.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.18a1713394912.tar", last modified: Wed Apr 17 23:04:23 2024, max compression
+gzip compressed data, was "pulumi_kubernetes_the_hard_way-0.0.18a1713406852.tar", last modified: Thu Apr 18 02:23:42 2024, max compression
```

## Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912.tar` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852.tar`

### file list

```diff
@@ -1,75 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:04:23.407535 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-17 23:04:23.407535 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:04:23.395535 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/
--rw-------   0 runner    (1001) docker     (127)     4080 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/__init__.py
--rw-------   0 runner    (1001) docker     (127)     9268 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:04:23.395535 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/config/
--rw-------   0 runner    (1001) docker     (127)      418 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/config/__init__.py
--rw-------   0 runner    (1001) docker     (127)      427 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/config/_enums.py
--rw-------   0 runner    (1001) docker     (127)    21101 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/config/_inputs.py
--rw-------   0 runner    (1001) docker     (127)     8728 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)     3426 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
--rw-------   0 runner    (1001) docker     (127)    23922 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
--rw-------   0 runner    (1001) docker     (127)    29159 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/config/outputs.py
--rw-------   0 runner    (1001) docker     (127)     2783 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/provider.py
--rw-------   0 runner    (1001) docker     (127)      116 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
--rw-------   0 runner    (1001) docker     (127)        0 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:04:23.403535 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/
--rw-------   0 runner    (1001) docker     (127)      940 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1095 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/_enums.py
--rw-------   0 runner    (1001) docker     (127)    15965 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    19229 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
--rw-------   0 runner    (1001) docker     (127)    10255 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
--rw-------   0 runner    (1001) docker     (127)    10159 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
--rw-------   0 runner    (1001) docker     (127)     8426 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/download.py
--rw-------   0 runner    (1001) docker     (127)    12377 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
--rw-------   0 runner    (1001) docker     (127)    14905 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
--rw-------   0 runner    (1001) docker     (127)    10651 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
--rw-------   0 runner    (1001) docker     (127)    14696 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
--rw-------   0 runner    (1001) docker     (127)     7339 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/file.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
--rw-------   0 runner    (1001) docker     (127)     9822 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
--rw-------   0 runner    (1001) docker     (127)     9652 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
--rw-------   0 runner    (1001) docker     (127)     9708 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
--rw-------   0 runner    (1001) docker     (127)     9622 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
--rw-------   0 runner    (1001) docker     (127)    15536 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/outputs.py
--rw-------   0 runner    (1001) docker     (127)    13390 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
--rw-------   0 runner    (1001) docker     (127)     9580 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/runc_install.py
--rw-------   0 runner    (1001) docker     (127)     5113 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
--rw-------   0 runner    (1001) docker     (127)     7429 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/static_pod.py
--rw-------   0 runner    (1001) docker     (127)     9915 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:04:23.403535 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tls/
--rw-------   0 runner    (1001) docker     (127)      425 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tls/__init__.py
--rw-------   0 runner    (1001) docker     (127)     1000 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tls/_enums.py
--rw-------   0 runner    (1001) docker     (127)     3157 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tls/_inputs.py
--rw-------   0 runner    (1001) docker     (127)    31109 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tls/certificate.py
--rw-------   0 runner    (1001) docker     (127)    15919 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
--rw-------   0 runner    (1001) docker     (127)     4450 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
--rw-------   0 runner    (1001) docker     (127)     3101 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tls/outputs.py
--rw-------   0 runner    (1001) docker     (127)    27642 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tls/root_ca.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:04:23.407535 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/
--rw-------   0 runner    (1001) docker     (127)      545 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/__init__.py
--rw-------   0 runner    (1001) docker     (127)     3142 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/_enums.py
--rw-------   0 runner    (1001) docker     (127)    22577 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/chmod.py
--rw-------   0 runner    (1001) docker     (127)    97822 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/curl.py
--rw-------   0 runner    (1001) docker     (127)    15129 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
--rw-------   0 runner    (1001) docker     (127)    24623 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
--rw-------   0 runner    (1001) docker     (127)    14032 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/mkdir.py
--rw-------   0 runner    (1001) docker     (127)    16572 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/mktemp.py
--rw-------   0 runner    (1001) docker     (127)    25981 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/mv.py
--rw-------   0 runner    (1001) docker     (127)    16828 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/rm.py
--rw-------   0 runner    (1001) docker     (127)    30857 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/sed.py
--rw-------   0 runner    (1001) docker     (127)    13649 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/systemctl.py
--rw-------   0 runner    (1001) docker     (127)    19232 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/tar.py
--rw-------   0 runner    (1001) docker     (127)    17062 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/tee.py
--rw-------   0 runner    (1001) docker     (127)    19599 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/wget.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-17 23:04:23.407535 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-17 23:04:23.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-17 23:04:23.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-17 23:04:23.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-17 23:04:23.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-17 23:04:23.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
--rw-------   0 runner    (1001) docker     (127)      899 2024-04-17 23:04:16.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-17 23:04:23.407535 pulumi_kubernetes_the_hard_way-0.0.18a1713394912/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:23:42.554564 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-18 02:23:42.554564 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     1165 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:23:42.538564 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/
+-rw-------   0 runner    (1001) docker     (127)     4080 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     9268 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:23:42.542564 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/config/
+-rw-------   0 runner    (1001) docker     (127)      418 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/config/__init__.py
+-rw-------   0 runner    (1001) docker     (127)      427 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/config/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    21101 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/config/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)     8728 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)     3426 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py
+-rw-------   0 runner    (1001) docker     (127)    23922 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py
+-rw-------   0 runner    (1001) docker     (127)    29159 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/config/outputs.py
+-rw-------   0 runner    (1001) docker     (127)     2783 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/provider.py
+-rw-------   0 runner    (1001) docker     (127)      116 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/pulumi-plugin.json
+-rw-------   0 runner    (1001) docker     (127)        0 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:23:42.546564 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/
+-rw-------   0 runner    (1001) docker     (127)      940 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1095 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    15965 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    19229 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py
+-rw-------   0 runner    (1001) docker     (127)    10255 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/containerd_install.py
+-rw-------   0 runner    (1001) docker     (127)    10159 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/crictl_install.py
+-rw-------   0 runner    (1001) docker     (127)     8426 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/download.py
+-rw-------   0 runner    (1001) docker     (127)    12377 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py
+-rw-------   0 runner    (1001) docker     (127)    14905 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py
+-rw-------   0 runner    (1001) docker     (127)    10651 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/etcd_install.py
+-rw-------   0 runner    (1001) docker     (127)    14696 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/etcd_service.py
+-rw-------   0 runner    (1001) docker     (127)     7339 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/file.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py
+-rw-------   0 runner    (1001) docker     (127)     9822 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py
+-rw-------   0 runner    (1001) docker     (127)     9652 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py
+-rw-------   0 runner    (1001) docker     (127)     9708 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py
+-rw-------   0 runner    (1001) docker     (127)     9622 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py
+-rw-------   0 runner    (1001) docker     (127)    15536 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    13390 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     9580 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/runc_install.py
+-rw-------   0 runner    (1001) docker     (127)     5113 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/start_etcd.py
+-rw-------   0 runner    (1001) docker     (127)     7429 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/static_pod.py
+-rw-------   0 runner    (1001) docker     (127)     9915 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/systemd_service.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:23:42.550564 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tls/
+-rw-------   0 runner    (1001) docker     (127)      425 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tls/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     1000 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tls/_enums.py
+-rw-------   0 runner    (1001) docker     (127)     3157 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tls/_inputs.py
+-rw-------   0 runner    (1001) docker     (127)    30597 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tls/certificate.py
+-rw-------   0 runner    (1001) docker     (127)    15919 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py
+-rw-------   0 runner    (1001) docker     (127)     4450 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tls/encryption_key.py
+-rw-------   0 runner    (1001) docker     (127)     3101 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tls/outputs.py
+-rw-------   0 runner    (1001) docker     (127)    27130 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tls/root_ca.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:23:42.550564 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/
+-rw-------   0 runner    (1001) docker     (127)      545 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/__init__.py
+-rw-------   0 runner    (1001) docker     (127)     3142 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/_enums.py
+-rw-------   0 runner    (1001) docker     (127)    22577 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/chmod.py
+-rw-------   0 runner    (1001) docker     (127)    97822 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/curl.py
+-rw-------   0 runner    (1001) docker     (127)    15129 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/etcdctl.py
+-rw-------   0 runner    (1001) docker     (127)    24623 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py
+-rw-------   0 runner    (1001) docker     (127)    14032 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/mkdir.py
+-rw-------   0 runner    (1001) docker     (127)    16572 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/mktemp.py
+-rw-------   0 runner    (1001) docker     (127)    25981 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/mv.py
+-rw-------   0 runner    (1001) docker     (127)    16828 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/rm.py
+-rw-------   0 runner    (1001) docker     (127)    30857 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/sed.py
+-rw-------   0 runner    (1001) docker     (127)    13649 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/systemctl.py
+-rw-------   0 runner    (1001) docker     (127)    19232 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/tar.py
+-rw-------   0 runner    (1001) docker     (127)    17062 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/tee.py
+-rw-------   0 runner    (1001) docker     (127)    19599 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/wget.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 02:23:42.550564 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     1850 2024-04-18 02:23:42.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     3302 2024-04-18 02:23:42.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 02:23:42.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      167 2024-04-18 02:23:42.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       31 2024-04-18 02:23:42.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way.egg-info/top_level.txt
+-rw-------   0 runner    (1001) docker     (127)      899 2024-04-18 02:23:35.000000 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 02:23:42.554564 pulumi_kubernetes_the_hard_way-0.0.18a1713406852/setup.cfg
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.18a1713394912
+Version: 0.0.18a1713406852
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/README.md` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/_utilities.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/config/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/config/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/config/get_kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/config/get_kubeconfig.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/config/kube_vip_manifest.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/config/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/provider.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/cni_plugins_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/containerd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/containerd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/crictl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/crictl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/download.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/download.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/etcd_cluster.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/etcd_configuration.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/etcd_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/etcd_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/etcd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/etcd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/file.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/file.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/kube_api_server_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/kube_controller_manager_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/kube_proxy_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/kube_scheduler_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/kubectl_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/kubelet_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/provision_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/runc_install.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/runc_install.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/start_etcd.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/start_etcd.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/static_pod.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/static_pod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/remote/systemd_service.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/remote/systemd_service.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tls/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tls/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tls/_inputs.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tls/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tls/certificate.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tls/certificate.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
                  algorithm: pulumi.Input['Algorithm'],
                  allowed_uses: pulumi.Input[Sequence[pulumi.Input['AllowedUsage']]],
                  ca_cert_pem: pulumi.Input[str],
                  ca_private_key_pem: pulumi.Input[str],
                  validity_period_hours: pulumi.Input[int],
                  dns_names: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  early_renewal_hours: Optional[pulumi.Input[int]] = None,
-                 ecdsa_curve: Optional[pulumi.Input[str]] = None,
+                 ecdsa_curve: Optional[pulumi.Input['EcdsaCurve']] = None,
                  ip_addresses: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  is_ca_certificate: Optional[pulumi.Input[bool]] = None,
                  rsa_bits: Optional[pulumi.Input[int]] = None,
                  set_subject_key_id: Optional[pulumi.Input[bool]] = None,
                  subject: Optional[pulumi.Input['pulumi_tls.CertRequestSubjectArgs']] = None,
                  uris: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
@@ -39,15 +39,15 @@
         :param pulumi.Input[int] validity_period_hours: Number of hours, after initial issuing, that the certificate will remain valid for.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] dns_names: List of DNS names for which a certificate is being requested (i.e. certificate subjects).
         :param pulumi.Input[int] early_renewal_hours: The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This
                can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old
                certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate
                revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the
                early renewal period. (default: `0`)
-        :param pulumi.Input[str] ecdsa_curve: When `algorithm` is `ECDSA`, the name of the elliptic curve to use. Currently-supported values are: `P224`, `P256`, `P384`, `P521`. (default: `P224`).
+        :param pulumi.Input['EcdsaCurve'] ecdsa_curve: TODO
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_addresses: List of IP addresses for which a certificate is being requested (i.e. certificate subjects).
         :param pulumi.Input[bool] is_ca_certificate: Is the generated certificate representing a Certificate Authority (CA) (default: `false`).
         :param pulumi.Input[int] rsa_bits: When `algorithm` is `RSA`, the size of the generated RSA key, in bits (default: `2048`).
         :param pulumi.Input[bool] set_subject_key_id: Should the generated certificate include a [subject key identifier](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2) (default: `false`).
         :param pulumi.Input['pulumi_tls.CertRequestSubjectArgs'] subject: TODO
         :param pulumi.Input[Sequence[pulumi.Input[str]]] uris: List of URIs for which a certificate is being requested (i.e. certificate subjects).
         """
@@ -161,22 +161,22 @@
 
     @early_renewal_hours.setter
     def early_renewal_hours(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "early_renewal_hours", value)
 
     @property
     @pulumi.getter(name="ecdsaCurve")
-    def ecdsa_curve(self) -> Optional[pulumi.Input[str]]:
+    def ecdsa_curve(self) -> Optional[pulumi.Input['EcdsaCurve']]:
         """
-        When `algorithm` is `ECDSA`, the name of the elliptic curve to use. Currently-supported values are: `P224`, `P256`, `P384`, `P521`. (default: `P224`).
+        TODO
         """
         return pulumi.get(self, "ecdsa_curve")
 
     @ecdsa_curve.setter
-    def ecdsa_curve(self, value: Optional[pulumi.Input[str]]):
+    def ecdsa_curve(self, value: Optional[pulumi.Input['EcdsaCurve']]):
         pulumi.set(self, "ecdsa_curve", value)
 
     @property
     @pulumi.getter(name="ipAddresses")
     def ip_addresses(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         List of IP addresses for which a certificate is being requested (i.e. certificate subjects).
@@ -255,15 +255,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  algorithm: Optional[pulumi.Input['Algorithm']] = None,
                  allowed_uses: Optional[pulumi.Input[Sequence[pulumi.Input['AllowedUsage']]]] = None,
                  ca_cert_pem: Optional[pulumi.Input[str]] = None,
                  ca_private_key_pem: Optional[pulumi.Input[str]] = None,
                  dns_names: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  early_renewal_hours: Optional[pulumi.Input[int]] = None,
-                 ecdsa_curve: Optional[pulumi.Input[str]] = None,
+                 ecdsa_curve: Optional[pulumi.Input['EcdsaCurve']] = None,
                  ip_addresses: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  is_ca_certificate: Optional[pulumi.Input[bool]] = None,
                  rsa_bits: Optional[pulumi.Input[int]] = None,
                  set_subject_key_id: Optional[pulumi.Input[bool]] = None,
                  subject: Optional[pulumi.Input[pulumi.InputType['pulumi_tls.CertRequestSubjectArgs']]] = None,
                  uris: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  validity_period_hours: Optional[pulumi.Input[int]] = None,
@@ -279,15 +279,15 @@
         :param pulumi.Input[str] ca_private_key_pem: Private key of the Certificate Authority (CA) used to sign the certificate, in [PEM (RFC 1421)](https://datatracker.ietf.org/doc/html/rfc1421) format.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] dns_names: List of DNS names for which a certificate is being requested (i.e. certificate subjects).
         :param pulumi.Input[int] early_renewal_hours: The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This
                can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old
                certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate
                revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the
                early renewal period. (default: `0`)
-        :param pulumi.Input[str] ecdsa_curve: When `algorithm` is `ECDSA`, the name of the elliptic curve to use. Currently-supported values are: `P224`, `P256`, `P384`, `P521`. (default: `P224`).
+        :param pulumi.Input['EcdsaCurve'] ecdsa_curve: TODO
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_addresses: List of IP addresses for which a certificate is being requested (i.e. certificate subjects).
         :param pulumi.Input[bool] is_ca_certificate: Is the generated certificate representing a Certificate Authority (CA) (default: `false`).
         :param pulumi.Input[int] rsa_bits: When `algorithm` is `RSA`, the size of the generated RSA key, in bits (default: `2048`).
         :param pulumi.Input[bool] set_subject_key_id: Should the generated certificate include a [subject key identifier](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2) (default: `false`).
         :param pulumi.Input[pulumi.InputType['pulumi_tls.CertRequestSubjectArgs']] subject: TODO
         :param pulumi.Input[Sequence[pulumi.Input[str]]] uris: List of URIs for which a certificate is being requested (i.e. certificate subjects).
         :param pulumi.Input[int] validity_period_hours: Number of hours, after initial issuing, that the certificate will remain valid for.
@@ -318,15 +318,15 @@
                  opts: Optional[pulumi.ResourceOptions] = None,
                  algorithm: Optional[pulumi.Input['Algorithm']] = None,
                  allowed_uses: Optional[pulumi.Input[Sequence[pulumi.Input['AllowedUsage']]]] = None,
                  ca_cert_pem: Optional[pulumi.Input[str]] = None,
                  ca_private_key_pem: Optional[pulumi.Input[str]] = None,
                  dns_names: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  early_renewal_hours: Optional[pulumi.Input[int]] = None,
-                 ecdsa_curve: Optional[pulumi.Input[str]] = None,
+                 ecdsa_curve: Optional[pulumi.Input['EcdsaCurve']] = None,
                  ip_addresses: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  is_ca_certificate: Optional[pulumi.Input[bool]] = None,
                  rsa_bits: Optional[pulumi.Input[int]] = None,
                  set_subject_key_id: Optional[pulumi.Input[bool]] = None,
                  subject: Optional[pulumi.Input[pulumi.InputType['pulumi_tls.CertRequestSubjectArgs']]] = None,
                  uris: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  validity_period_hours: Optional[pulumi.Input[int]] = None,
@@ -479,17 +479,17 @@
         revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the
         early renewal period. (default: `0`)
         """
         return pulumi.get(self, "early_renewal_hours")
 
     @property
     @pulumi.getter(name="ecdsaCurve")
-    def ecdsa_curve(self) -> pulumi.Output[str]:
+    def ecdsa_curve(self) -> pulumi.Output['EcdsaCurve']:
         """
-        When `algorithm` is `ECDSA`, the name of the elliptic curve to use. Currently-supported values are: `P224`, `P256`, `P384`, `P521`. (default: `P224`).
+        TODO
         """
         return pulumi.get(self, "ecdsa_curve")
 
     @property
     @pulumi.getter(name="ipAddresses")
     def ip_addresses(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tls/cluster_pki.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tls/encryption_key.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tls/encryption_key.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tls/outputs.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tls/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tls/root_ca.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tls/root_ca.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 @pulumi.input_type
 class RootCaArgs:
     def __init__(__self__, *,
                  validity_period_hours: pulumi.Input[int],
                  algorithm: Optional[pulumi.Input['Algorithm']] = None,
                  dns_names: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  early_renewal_hours: Optional[pulumi.Input[int]] = None,
-                 ecdsa_curve: Optional[pulumi.Input[str]] = None,
+                 ecdsa_curve: Optional[pulumi.Input['EcdsaCurve']] = None,
                  ip_addresses: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  rsa_bits: Optional[pulumi.Input[int]] = None,
                  set_authority_key_id: Optional[pulumi.Input[bool]] = None,
                  set_subject_key_id: Optional[pulumi.Input[bool]] = None,
                  subject: Optional[pulumi.Input['pulumi_tls.SelfSignedCertSubjectArgs']] = None,
                  uris: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None):
         """
@@ -33,15 +33,15 @@
         :param pulumi.Input['Algorithm'] algorithm: Name of the algorithm to use when generating the private key.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] dns_names: List of DNS names for which a certificate is being requested (i.e. certificate subjects).
         :param pulumi.Input[int] early_renewal_hours: The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This
                can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old
                certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate
                revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the
                early renewal period. (default: `0`)
-        :param pulumi.Input[str] ecdsa_curve: When `algorithm` is `ECDSA`, the name of the elliptic curve to use. Currently-supported values are: `P224`, `P256`, `P384`, `P521`. (default: `P224`).
+        :param pulumi.Input['EcdsaCurve'] ecdsa_curve: TODO
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_addresses: List of IP addresses for which a certificate is being requested (i.e. certificate subjects).
         :param pulumi.Input[int] rsa_bits: When `algorithm` is `RSA`, the size of the generated RSA key, in bits (default: `2048`).
         :param pulumi.Input[bool] set_authority_key_id: Should the generated certificate include an [authority key identifier](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.1): for self-signed certificates this is the same value as the [subject key identifier](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2) (default: `false`).
         :param pulumi.Input[bool] set_subject_key_id: Should the generated certificate include a [subject key identifier](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2) (default: `false`).
         :param pulumi.Input['pulumi_tls.SelfSignedCertSubjectArgs'] subject: TODO
         :param pulumi.Input[Sequence[pulumi.Input[str]]] uris: List of URIs for which a certificate is being requested (i.e. certificate subjects).
         """
@@ -117,22 +117,22 @@
 
     @early_renewal_hours.setter
     def early_renewal_hours(self, value: Optional[pulumi.Input[int]]):
         pulumi.set(self, "early_renewal_hours", value)
 
     @property
     @pulumi.getter(name="ecdsaCurve")
-    def ecdsa_curve(self) -> Optional[pulumi.Input[str]]:
+    def ecdsa_curve(self) -> Optional[pulumi.Input['EcdsaCurve']]:
         """
-        When `algorithm` is `ECDSA`, the name of the elliptic curve to use. Currently-supported values are: `P224`, `P256`, `P384`, `P521`. (default: `P224`).
+        TODO
         """
         return pulumi.get(self, "ecdsa_curve")
 
     @ecdsa_curve.setter
-    def ecdsa_curve(self, value: Optional[pulumi.Input[str]]):
+    def ecdsa_curve(self, value: Optional[pulumi.Input['EcdsaCurve']]):
         pulumi.set(self, "ecdsa_curve", value)
 
     @property
     @pulumi.getter(name="ipAddresses")
     def ip_addresses(self) -> Optional[pulumi.Input[Sequence[pulumi.Input[str]]]]:
         """
         List of IP addresses for which a certificate is being requested (i.e. certificate subjects).
@@ -208,15 +208,15 @@
     @overload
     def __init__(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  algorithm: Optional[pulumi.Input['Algorithm']] = None,
                  dns_names: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  early_renewal_hours: Optional[pulumi.Input[int]] = None,
-                 ecdsa_curve: Optional[pulumi.Input[str]] = None,
+                 ecdsa_curve: Optional[pulumi.Input['EcdsaCurve']] = None,
                  ip_addresses: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  rsa_bits: Optional[pulumi.Input[int]] = None,
                  set_authority_key_id: Optional[pulumi.Input[bool]] = None,
                  set_subject_key_id: Optional[pulumi.Input[bool]] = None,
                  subject: Optional[pulumi.Input[pulumi.InputType['pulumi_tls.SelfSignedCertSubjectArgs']]] = None,
                  uris: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  validity_period_hours: Optional[pulumi.Input[int]] = None,
@@ -229,15 +229,15 @@
         :param pulumi.Input['Algorithm'] algorithm: Name of the algorithm to use when generating the private key.
         :param pulumi.Input[Sequence[pulumi.Input[str]]] dns_names: List of DNS names for which a certificate is being requested (i.e. certificate subjects).
         :param pulumi.Input[int] early_renewal_hours: The resource will consider the certificate to have expired the given number of hours before its actual expiry time. This
                can be useful to deploy an updated certificate in advance of the expiration of the current certificate. However, the old
                certificate remains valid until its true expiration time, since this resource does not (and cannot) support certificate
                revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the
                early renewal period. (default: `0`)
-        :param pulumi.Input[str] ecdsa_curve: When `algorithm` is `ECDSA`, the name of the elliptic curve to use. Currently-supported values are: `P224`, `P256`, `P384`, `P521`. (default: `P224`).
+        :param pulumi.Input['EcdsaCurve'] ecdsa_curve: TODO
         :param pulumi.Input[Sequence[pulumi.Input[str]]] ip_addresses: List of IP addresses for which a certificate is being requested (i.e. certificate subjects).
         :param pulumi.Input[int] rsa_bits: When `algorithm` is `RSA`, the size of the generated RSA key, in bits (default: `2048`).
         :param pulumi.Input[bool] set_authority_key_id: Should the generated certificate include an [authority key identifier](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.1): for self-signed certificates this is the same value as the [subject key identifier](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2) (default: `false`).
         :param pulumi.Input[bool] set_subject_key_id: Should the generated certificate include a [subject key identifier](https://datatracker.ietf.org/doc/html/rfc5280#section-4.2.1.2) (default: `false`).
         :param pulumi.Input[pulumi.InputType['pulumi_tls.SelfSignedCertSubjectArgs']] subject: TODO
         :param pulumi.Input[Sequence[pulumi.Input[str]]] uris: List of URIs for which a certificate is being requested (i.e. certificate subjects).
         :param pulumi.Input[int] validity_period_hours: Number of hours, after initial issuing, that the certificate will remain valid for.
@@ -265,15 +265,15 @@
 
     def _internal_init(__self__,
                  resource_name: str,
                  opts: Optional[pulumi.ResourceOptions] = None,
                  algorithm: Optional[pulumi.Input['Algorithm']] = None,
                  dns_names: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  early_renewal_hours: Optional[pulumi.Input[int]] = None,
-                 ecdsa_curve: Optional[pulumi.Input[str]] = None,
+                 ecdsa_curve: Optional[pulumi.Input['EcdsaCurve']] = None,
                  ip_addresses: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  rsa_bits: Optional[pulumi.Input[int]] = None,
                  set_authority_key_id: Optional[pulumi.Input[bool]] = None,
                  set_subject_key_id: Optional[pulumi.Input[bool]] = None,
                  subject: Optional[pulumi.Input[pulumi.InputType['pulumi_tls.SelfSignedCertSubjectArgs']]] = None,
                  uris: Optional[pulumi.Input[Sequence[pulumi.Input[str]]]] = None,
                  validity_period_hours: Optional[pulumi.Input[int]] = None,
@@ -374,17 +374,17 @@
         revocation. Also, this advance update can only be performed should the Terraform configuration be applied during the
         early renewal period. (default: `0`)
         """
         return pulumi.get(self, "early_renewal_hours")
 
     @property
     @pulumi.getter(name="ecdsaCurve")
-    def ecdsa_curve(self) -> pulumi.Output[str]:
+    def ecdsa_curve(self) -> pulumi.Output['EcdsaCurve']:
         """
-        When `algorithm` is `ECDSA`, the name of the elliptic curve to use. Currently-supported values are: `P224`, `P256`, `P384`, `P521`. (default: `P224`).
+        TODO
         """
         return pulumi.get(self, "ecdsa_curve")
 
     @property
     @pulumi.getter(name="ipAddresses")
     def ip_addresses(self) -> pulumi.Output[Optional[Sequence[str]]]:
         """
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/__init__.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/_enums.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/chmod.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/chmod.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/curl.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/curl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/etcdctl.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/etcdctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/hostnamectl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/mkdir.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/mkdir.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/mktemp.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/mktemp.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/mv.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/mv.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/rm.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/rm.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/sed.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/sed.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/systemctl.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/systemctl.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/tar.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/tar.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/tee.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/tee.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way/tools/wget.py` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way/tools/wget.py`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_kubernetes_the_hard_way
-Version: 0.0.18a1713394912
+Version: 0.0.18a1713406852
 Summary: A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way
 License: Apache-2.0
 Project-URL: Repository, https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way
 Keywords: pulumi,command,tls,kubernetes,category/utility,kind/component
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Requires-Dist: parver>=0.2.1
```

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pulumi_kubernetes_the_hard_way.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_kubernetes_the_hard_way-0.0.18a1713394912/pyproject.toml` & `pulumi_kubernetes_the_hard_way-0.0.18a1713406852/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [project]
   name = "pulumi_kubernetes_the_hard_way"
   description = "A Pulumi implementation of Kelsey Hightower's Kubernetes the Hard Way"
   dependencies = ["parver>=0.2.1", "pulumi>=3.91.1,<4.0.0", "pulumi-command>=0.10.0,<1.0.0", "pulumi-kubernetes>=4.10.0,<5.0.0", "pulumi-random>=4.16.1,<5.0.0", "pulumi-tls>=5.0.2,<6.0.0", "semver>=2.8.1"]
   keywords = ["pulumi", "command", "tls", "kubernetes", "category/utility", "kind/component"]
   readme = "README.md"
   requires-python = ">=3.8"
-  version = "0.0.18a1713394912"
+  version = "0.0.18a1713406852"
   [project.license]
     text = "Apache-2.0"
   [project.urls]
     Repository = "https://github.com/UnstoppableMango/pulumi-kubernetes-the-hard-way"
 
 [build-system]
   requires = ["setuptools>=61.0"]
```

