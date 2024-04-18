# Comparing `tmp/tensorpc-0.10.1.tar.gz` & `tmp/tensorpc-0.10.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tensorpc-0.10.1.tar", last modified: Mon Apr  8 06:19:37 2024, max compression
+gzip compressed data, was "tensorpc-0.10.2.tar", last modified: Thu Apr 18 06:07:23 2024, max compression
```

## Comparing `tensorpc-0.10.1.tar` & `tensorpc-0.10.2.tar`

### file list

```diff
@@ -1,360 +1,360 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.154681 tensorpc-0.10.1/
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-08 06:19:06.000000 tensorpc-0.10.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-08 06:19:06.000000 tensorpc-0.10.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-08 06:19:37.154681 tensorpc-0.10.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-08 06:19:06.000000 tensorpc-0.10.1/README.md
--rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-08 06:19:06.000000 tensorpc-0.10.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-08 06:19:37.154681 tensorpc-0.10.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-08 06:19:06.000000 tensorpc-0.10.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.102681 tensorpc-0.10.1/tensorpc/
--rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-08 06:19:36.000000 tensorpc-0.10.1/tensorpc/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.102681 tensorpc-0.10.1/tensorpc/apps/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/apps/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.102681 tensorpc-0.10.1/tensorpc/apps/cbvc/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/apps/cbvc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.102681 tensorpc-0.10.1/tensorpc/apps/file/
--rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/apps/file/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.102681 tensorpc-0.10.1/tensorpc/autossh/
--rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/autossh/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/autossh/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    52830 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/autossh/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/autossh/coretypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.106681 tensorpc-0.10.1/tensorpc/autossh/media/
--rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/autossh/media/hooks-bash-legacy.sh
--rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/autossh/media/hooks-bash.sh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.106681 tensorpc-0.10.1/tensorpc/autossh/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/autossh/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/autossh/scheduler/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/autossh/scheduler/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/autossh/scheduler/core.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.106681 tensorpc-0.10.1/tensorpc/autossh/scheduler/init_scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/autossh/scheduler/init_scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/autossh/scheduler/init_scheduler/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.106681 tensorpc-0.10.1/tensorpc/autossh/scheduler/runtask/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/autossh/scheduler/runtask/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/autossh/scheduler/runtask/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/autossh/scheduler/task_client.py
--rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/autossh/scheduler/test_data.py
--rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/autossh/scheduler/tmux.py
--rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/autossh/serv_names.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.106681 tensorpc-0.10.1/tensorpc/autossh/services/
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/autossh/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    12832 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/autossh/services/scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.106681 tensorpc-0.10.1/tensorpc/cli/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.106681 tensorpc-0.10.1/tensorpc/cli/cppls/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/cppls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/cppls/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.106681 tensorpc-0.10.1/tensorpc/cli/cpuusage/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/cpuusage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/cpuusage/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.106681 tensorpc-0.10.1/tensorpc/cli/createmsg/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/createmsg/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/createmsg/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.106681 tensorpc-0.10.1/tensorpc/cli/download_file/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/download_file/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/download_file/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.110681 tensorpc-0.10.1/tensorpc/cli/free_port/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/free_port/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/free_port/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.110681 tensorpc-0.10.1/tensorpc/cli/gpuusage/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/gpuusage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/gpuusage/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.110681 tensorpc-0.10.1/tensorpc/cli/iperf/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/iperf/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/iperf/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.110681 tensorpc-0.10.1/tensorpc/cli/ping/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/ping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/ping/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.110681 tensorpc-0.10.1/tensorpc/cli/proto_files/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/proto_files/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/proto_files/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.110681 tensorpc-0.10.1/tensorpc/cli/proto_root/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/proto_root/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/proto_root/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.110681 tensorpc-0.10.1/tensorpc/cli/pyls/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/pyls/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/pyls/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.110681 tensorpc-0.10.1/tensorpc/cli/pyright_launch/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/pyright_launch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/pyright_launch/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.110681 tensorpc-0.10.1/tensorpc/cli/start_worker/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/start_worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/cli/start_worker/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/compat.py
--rw-r--r--   0 runner    (1001) docker     (127)      670 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.114681 tensorpc-0.10.1/tensorpc/core/
--rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17225 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/asyncclient.py
--rw-r--r--   0 runner    (1001) docker     (127)    14211 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/asyncserver.py
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/asynctools.py
--rw-r--r--   0 runner    (1001) docker     (127)    16973 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/client.py
--rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)    35660 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/core_io.py
--rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/dataclass_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/defs.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.114681 tensorpc-0.10.1/tensorpc/core/event_emitter/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/event_emitter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/event_emitter/aio.py
--rw-r--r--   0 runner    (1001) docker     (127)    12964 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/event_emitter/base.py
--rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/funcid.py
--rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/httpclient.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.118681 tensorpc-0.10.1/tensorpc/core/httpservers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/httpservers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/httpservers/aiohttp_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/httpservers/all.py
--rw-r--r--   0 runner    (1001) docker     (127)    10199 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/httpservers/blacksheep_impl.py
--rw-r--r--   0 runner    (1001) docker     (127)    35233 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/httpservers/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/inspecttools.py
--rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/marker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/moduleid.py
--rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/prim.py
--rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/rprint_dispatch.py
--rw-r--r--   0 runner    (1001) docker     (127)     8397 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/server.py
--rw-r--r--   0 runner    (1001) docker     (127)    28937 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/server_core.py
--rw-r--r--   0 runner    (1001) docker     (127)    53083 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/serviceunit.py
--rw-r--r--   0 runner    (1001) docker     (127)    10312 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/tracer.py
--rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/core/tree_id.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.118681 tensorpc-0.10.1/tensorpc/examples/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.118681 tensorpc-0.10.1/tensorpc/examples/ai/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/ai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/ai/engine.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.098681 tensorpc-0.10.1/tensorpc/examples/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.118681 tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.1-Hello World.md
--rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.10-Template Component.md
--rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.11-Inheritance.md
--rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.12-App Context.md
--rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.13-Component Context.md
--rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.14-Host Resource.md
--rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.2-App Basic Architecture.md
--rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.3-Flex Box Basic.md
--rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.4-Containers.md
--rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.5-Advanced Events.md
--rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.6-Composite Component.md
--rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.7-Advanced UI Methods.md
--rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.8-Drag And Drop.md
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.9-Reload System.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.126681 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/
--rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.0-Common Props.md
--rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.1-Button.md
--rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.10-Slider.md
--rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.11-Tab.md
--rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.12-Drawer.md
--rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.13-Dialog.md
--rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.14-Collapse.md
--rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.15-Chip.md
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.16-Progress.md
--rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.17-MenuList.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.18-JsonLikeTree.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.19-DynamicControl.md
--rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.2-Typography.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.20-VirtualizedBox.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.21-DataFlexBox.md
--rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.22-DataGrid.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.23-Special.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.24-Editor.md
--rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.25-Plotly.md
--rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.26-Map.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.27-Allotment.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.28-JsonViewer.md
--rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.3-Markdown.md
--rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.4-TextField.md
--rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.5-List.md
--rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.6-Select.md
--rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.7-AutoComplete.md
--rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.8-ToggleButton.md
--rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.9-Image.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.126681 tensorpc-0.10.1/tensorpc/examples/tutorials/03-3d basic/
--rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/03-3d basic/3.1-Hello 3D World.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/03-3d basic/3.2-3D Events.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/03-3d basic/3.3-Controls.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/03-3d basic/3.4-Selection.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/03-3d basic/3.5-Views.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/03-3d basic/3.6-Resources.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/03-3d basic/3.7-Custom Shaders.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.126681 tensorpc-0.10.1/tensorpc/examples/tutorials/04-3d components/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/04-3d components/4.1-Canvas.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/04-3d components/4.2-Mesh.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/04-3d components/4.3-Points.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/04-3d components/4.4-Lines.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.126681 tensorpc-0.10.1/tensorpc/examples/tutorials/05-advanced/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/05-advanced/5.1-Inspector.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/05-advanced/5.2-SimpleCanvas.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.126681 tensorpc-0.10.1/tensorpc/examples/tutorials/06-sample apps/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/06-sample apps/6.1-Chat App.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/06-sample apps/6.2-Deep Learning.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.126681 tensorpc-0.10.1/tensorpc/examples/tutorials/07-V Api/
--rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/07-V Api/7.1-Basic.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/07-V Api/7.2-Events.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/07-V Api/7.3-Lines.md
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/07-V Api/7.4-Image.md
--rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials/07-V Api/7.5-Points.md
--rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/examples/tutorials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.130681 tensorpc-0.10.1/tensorpc/flow/
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    17924 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/client.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.130681 tensorpc-0.10.1/tensorpc/flow/close_langserv/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/close_langserv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/close_langserv/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/constants.py
--rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/coretypes.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.130681 tensorpc-0.10.1/tensorpc/flow/flowapp/
--rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    76779 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/appcore.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.130681 tensorpc-0.10.1/tensorpc/flow/flowapp/appctx/
--rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/appctx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/appctx/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/appctx/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6783 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/appctx/inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/colors.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.134681 tensorpc-0.10.1/tensorpc/flow/flowapp/components/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/annocore.py
--rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    13130 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/leaflet.py
--rw-r--r--   0 runner    (1001) docker     (127)   178760 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/mui.py
--rw-r--r--   0 runner    (1001) docker     (127)    15273 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plotly.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.138681 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/
--rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/arraycommon.py
--rw-r--r--   0 runner    (1001) docker     (127)    22472 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/arraygrid.py
--rw-r--r--   0 runner    (1001) docker     (127)    32169 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/common.py
--rw-r--r--   0 runner    (1001) docker     (127)    26537 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/config.py
--rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/figure.py
--rw-r--r--   0 runner    (1001) docker     (127)    16189 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/grid_preview_layout.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.138681 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/handlers/
--rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/handlers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/handlers/common.py
--rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/handlers/gv_common.py
--rw-r--r--   0 runner    (1001) docker     (127)     6902 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/monitor.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.138681 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/objinspect/
--rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/objinspect/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    18878 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/objinspect/analysis.py
--rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/objinspect/controllers.py
--rw-r--r--   0 runner    (1001) docker     (127)    24091 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/objinspect/inspector.py
--rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/objinspect/inspectpanel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/objinspect/layout.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/objinspect/reload.py
--rw-r--r--   0 runner    (1001) docker     (127)    44644 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/objinspect/tree.py
--rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/objinspect/treeitems.py
--rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/options.py
--rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/reload_utils.py
--rw-r--r--   0 runner    (1001) docker     (127)    16020 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (127)    13938 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/scriptmgr.py
--rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/sliders.py
--rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/tutorials.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.142681 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/vis/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/vis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    56801 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/vis/canvas.py
--rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/vis/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/vis/treeview.py
--rw-r--r--   0 runner    (1001) docker     (127)    27521 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/vis/vapi_core.py
--rw-r--r--   0 runner    (1001) docker     (127)   144462 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/three.py
--rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/threecore.py
--rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/components/typemetas.py
--rw-r--r--   0 runner    (1001) docker     (127)    79929 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/core.py
--rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/coretypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     9629 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/objtree.py
--rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/flowapp/reload.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.142681 tensorpc-0.10.1/tensorpc/flow/init_langserv/
--rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/init_langserv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/init_langserv/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)    24656 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/jsonlike.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.142681 tensorpc-0.10.1/tensorpc/flow/langserv/
--rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/langserv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/langserv/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/langserv/pyls.py
--rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/langserv/pyrightcfg.py
--rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/marker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.142681 tensorpc-0.10.1/tensorpc/flow/runapp/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/runapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/runapp/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.146681 tensorpc-0.10.1/tensorpc/flow/sampleapp/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/sampleapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)    59344 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/sampleapp/app.py
--rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/sampleapp/arraygrid.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/sampleapp/collection.py
--rw-r--r--   0 runner    (1001) docker     (127)    41653 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/sampleapp/d3.py
--rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/sampleapp/file.py
--rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/sampleapp/sample_preview.py
--rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/sampleapp/sample_reload_fn.py
--rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/sampleapp/v_nextgen.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.146681 tensorpc-0.10.1/tensorpc/flow/serv/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/serv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)   105758 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/serv/core.py
--rw-r--r--   0 runner    (1001) docker     (127)    18787 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/serv/flowapp.py
--rw-r--r--   0 runner    (1001) docker     (127)    29044 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/serv/worker.py
--rw-r--r--   0 runner    (1001) docker     (127)     8826 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/flow/serv_names.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/marker.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.146681 tensorpc-0.10.1/tensorpc/protos/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/protos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/protos/arraybuf_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/protos/arraybuf_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/protos/arraybuf_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/protos/remote_object_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/protos/remote_object_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)    21852 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/protos/remote_object_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/protos/rpc_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/protos/rpc_message_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/protos/wsdef_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/protos/wsdef_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/protos_export.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.150681 tensorpc-0.10.1/tensorpc/protos_legacy/
--rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/protos_legacy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/protos_legacy/arraybuf_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/protos_legacy/arraybuf_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/protos_legacy/remote_object_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)    11472 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/protos_legacy/remote_object_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (127)    25985 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/protos_legacy/rpc_message_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/protos_legacy/rpc_message_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/protos_legacy/wsdef_pb2.py
--rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/protos_legacy/wsdef_pb2.pyi
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.150681 tensorpc-0.10.1/tensorpc/scheduler/
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/scheduler/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.150681 tensorpc-0.10.1/tensorpc/serve/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/serve/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/serve/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.150681 tensorpc-0.10.1/tensorpc/serve/flowapp_script/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/serve/flowapp_script/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/serve/flowapp_script/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.150681 tensorpc-0.10.1/tensorpc/serve_sync/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/serve_sync/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/serve_sync/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.150681 tensorpc-0.10.1/tensorpc/services/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/services/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/services/collection.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.150681 tensorpc-0.10.1/tensorpc/services/flow/
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/services/flow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/services/flow/core.py
--rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/services/for_test.py
--rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/services/vis.py
--rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.154681 tensorpc-0.10.1/tensorpc/utils/
--rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/utils/address.py
--rw-r--r--   0 runner    (1001) docker     (127)     9344 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/utils/df_logging.py
--rw-r--r--   0 runner    (1001) docker     (127)     1653 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/utils/gpuusage.py
--rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/utils/registry.py
--rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/utils/reload.py
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/utils/subproc.py
--rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/utils/typeutils.py
--rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/utils/uniquename.py
--rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-08 06:19:06.000000 tensorpc-0.10.1/tensorpc/utils/wait_tools.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.154681 tensorpc-0.10.1/tensorpc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-08 06:19:37.000000 tensorpc-0.10.1/tensorpc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-04-08 06:19:37.000000 tensorpc-0.10.1/tensorpc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-08 06:19:37.000000 tensorpc-0.10.1/tensorpc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-08 06:19:37.000000 tensorpc-0.10.1/tensorpc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-08 06:19:37.000000 tensorpc-0.10.1/tensorpc.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-08 06:19:37.154681 tensorpc-0.10.1/test/
--rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-08 06:19:06.000000 tensorpc-0.10.1/test/test_tmux_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.623057 tensorpc-0.10.2/
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-18 06:06:51.000000 tensorpc-0.10.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)       87 2024-04-18 06:06:51.000000 tensorpc-0.10.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-18 06:07:23.623057 tensorpc-0.10.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)      642 2024-04-18 06:06:51.000000 tensorpc-0.10.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (127)      225 2024-04-18 06:06:51.000000 tensorpc-0.10.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-18 06:07:23.623057 tensorpc-0.10.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (127)     4406 2024-04-18 06:06:51.000000 tensorpc-0.10.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.567057 tensorpc-0.10.2/tensorpc/
+-rw-r--r--   0 runner    (1001) docker     (127)      701 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       23 2024-04-18 06:07:23.000000 tensorpc-0.10.2/tensorpc/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.571057 tensorpc-0.10.2/tensorpc/apps/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/apps/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.571057 tensorpc-0.10.2/tensorpc/apps/cbvc/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/apps/cbvc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.571057 tensorpc-0.10.2/tensorpc/apps/file/
+-rw-r--r--   0 runner    (1001) docker     (127)     2013 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/apps/file/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.571057 tensorpc-0.10.2/tensorpc/autossh/
+-rw-r--r--   0 runner    (1001) docker     (127)      600 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/autossh/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      656 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/autossh/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    52830 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/autossh/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      818 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/autossh/coretypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.571057 tensorpc-0.10.2/tensorpc/autossh/media/
+-rw-r--r--   0 runner    (1001) docker     (127)     5929 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/autossh/media/hooks-bash-legacy.sh
+-rw-r--r--   0 runner    (1001) docker     (127)     8475 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/autossh/media/hooks-bash.sh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.571057 tensorpc-0.10.2/tensorpc/autossh/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)      139 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/autossh/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7446 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/autossh/scheduler/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      764 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/autossh/scheduler/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3209 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/autossh/scheduler/core.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.571057 tensorpc-0.10.2/tensorpc/autossh/scheduler/init_scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/autossh/scheduler/init_scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      210 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/autossh/scheduler/init_scheduler/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.571057 tensorpc-0.10.2/tensorpc/autossh/scheduler/runtask/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/autossh/scheduler/runtask/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2788 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/autossh/scheduler/runtask/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2609 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/autossh/scheduler/task_client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      492 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/autossh/scheduler/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5518 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/autossh/scheduler/tmux.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3571 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/autossh/serv_names.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.575057 tensorpc-0.10.2/tensorpc/autossh/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/autossh/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12832 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/autossh/services/scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.575057 tensorpc-0.10.2/tensorpc/cli/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.575057 tensorpc-0.10.2/tensorpc/cli/cppls/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/cppls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      207 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/cppls/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.575057 tensorpc-0.10.2/tensorpc/cli/cpuusage/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/cpuusage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1085 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/cpuusage/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.575057 tensorpc-0.10.2/tensorpc/cli/createmsg/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/createmsg/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1318 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/createmsg/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.575057 tensorpc-0.10.2/tensorpc/cli/download_file/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/download_file/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      296 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/download_file/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.575057 tensorpc-0.10.2/tensorpc/cli/free_port/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/free_port/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      216 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/free_port/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.575057 tensorpc-0.10.2/tensorpc/cli/gpuusage/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/gpuusage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1426 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/gpuusage/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.575057 tensorpc-0.10.2/tensorpc/cli/iperf/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/iperf/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      908 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/iperf/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.575057 tensorpc-0.10.2/tensorpc/cli/ping/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/ping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      373 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/ping/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.575057 tensorpc-0.10.2/tensorpc/cli/proto_files/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/proto_files/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/proto_files/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.579057 tensorpc-0.10.2/tensorpc/cli/proto_root/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/proto_root/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      788 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/proto_root/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.579057 tensorpc-0.10.2/tensorpc/cli/pyls/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/pyls/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      243 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/pyls/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.579057 tensorpc-0.10.2/tensorpc/cli/pyright_launch/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/pyright_launch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      138 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/pyright_launch/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.579057 tensorpc-0.10.2/tensorpc/cli/start_worker/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/start_worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1462 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/cli/start_worker/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1725 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/compat.py
+-rw-r--r--   0 runner    (1001) docker     (127)      696 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.583057 tensorpc-0.10.2/tensorpc/core/
+-rw-r--r--   0 runner    (1001) docker     (127)     1393 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17225 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/asyncclient.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14880 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/asyncserver.py
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/asynctools.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16973 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/client.py
+-rw-r--r--   0 runner    (1001) docker     (127)      147 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35660 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/core_io.py
+-rw-r--r--   0 runner    (1001) docker     (127)      283 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/dataclass_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1792 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/defs.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.583057 tensorpc-0.10.2/tensorpc/core/event_emitter/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/event_emitter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3724 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/event_emitter/aio.py
+-rw-r--r--   0 runner    (1001) docker     (127)    12964 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/event_emitter/base.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7113 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/funcid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    14601 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/httpclient.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.583057 tensorpc-0.10.2/tensorpc/core/httpservers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/httpservers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13273 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/httpservers/aiohttp_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/httpservers/all.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10199 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/httpservers/blacksheep_impl.py
+-rw-r--r--   0 runner    (1001) docker     (127)    35233 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/httpservers/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4511 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/inspecttools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2339 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/marker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8940 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/moduleid.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1884 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/prim.py
+-rw-r--r--   0 runner    (1001) docker     (127)      336 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/rprint_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9055 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/server.py
+-rw-r--r--   0 runner    (1001) docker     (127)    28937 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/server_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    53083 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/serviceunit.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10714 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/tracer.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4755 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/core/tree_id.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.583057 tensorpc-0.10.2/tensorpc/examples/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.583057 tensorpc-0.10.2/tensorpc/examples/ai/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/ai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/ai/engine.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.563057 tensorpc-0.10.2/tensorpc/examples/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.587057 tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.1-Hello World.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7599 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.10-Template Component.md
+-rw-r--r--   0 runner    (1001) docker     (127)      958 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.11-Inheritance.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3465 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.12-App Context.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1350 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.13-Component Context.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2230 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.14-Host Resource.md
+-rw-r--r--   0 runner    (1001) docker     (127)     5957 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.2-App Basic Architecture.md
+-rw-r--r--   0 runner    (1001) docker     (127)     9827 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.3-Flex Box Basic.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1869 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.4-Containers.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3592 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.5-Advanced Events.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1655 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.6-Composite Component.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3370 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.7-Advanced UI Methods.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4209 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.8-Drag And Drop.md
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.9-Reload System.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.591057 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/
+-rw-r--r--   0 runner    (1001) docker     (127)     1623 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.0-Common Props.md
+-rw-r--r--   0 runner    (1001) docker     (127)     7521 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.1-Button.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1544 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.10-Slider.md
+-rw-r--r--   0 runner    (1001) docker     (127)    11336 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.11-Tab.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2069 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.12-Drawer.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1301 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.13-Dialog.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3956 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.14-Collapse.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2741 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.15-Chip.md
+-rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.16-Progress.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2805 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.17-MenuList.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.18-JsonLikeTree.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.19-DynamicControl.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1669 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.2-Typography.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.20-VirtualizedBox.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.21-DataFlexBox.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2776 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.22-DataGrid.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.23-Special.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.24-Editor.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3350 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.25-Plotly.md
+-rw-r--r--   0 runner    (1001) docker     (127)      783 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.26-Map.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.27-Allotment.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.28-JsonViewer.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2666 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.3-Markdown.md
+-rw-r--r--   0 runner    (1001) docker     (127)     6342 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.4-TextField.md
+-rw-r--r--   0 runner    (1001) docker     (127)     2665 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.5-List.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3132 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.6-Select.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3738 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.7-AutoComplete.md
+-rw-r--r--   0 runner    (1001) docker     (127)     3633 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.8-ToggleButton.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1521 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.9-Image.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.595057 tensorpc-0.10.2/tensorpc/examples/tutorials/03-3d basic/
+-rw-r--r--   0 runner    (1001) docker     (127)     2405 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/03-3d basic/3.1-Hello 3D World.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/03-3d basic/3.2-3D Events.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/03-3d basic/3.3-Controls.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/03-3d basic/3.4-Selection.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/03-3d basic/3.5-Views.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/03-3d basic/3.6-Resources.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/03-3d basic/3.7-Custom Shaders.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.595057 tensorpc-0.10.2/tensorpc/examples/tutorials/04-3d components/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/04-3d components/4.1-Canvas.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/04-3d components/4.2-Mesh.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/04-3d components/4.3-Points.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/04-3d components/4.4-Lines.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.595057 tensorpc-0.10.2/tensorpc/examples/tutorials/05-advanced/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/05-advanced/5.1-Inspector.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/05-advanced/5.2-SimpleCanvas.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.595057 tensorpc-0.10.2/tensorpc/examples/tutorials/06-sample apps/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/06-sample apps/6.1-Chat App.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/06-sample apps/6.2-Deep Learning.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.595057 tensorpc-0.10.2/tensorpc/examples/tutorials/07-V Api/
+-rw-r--r--   0 runner    (1001) docker     (127)     1843 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/07-V Api/7.1-Basic.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/07-V Api/7.2-Events.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/07-V Api/7.3-Lines.md
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/07-V Api/7.4-Image.md
+-rw-r--r--   0 runner    (1001) docker     (127)      244 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials/07-V Api/7.5-Points.md
+-rw-r--r--   0 runner    (1001) docker     (127)     1929 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/examples/tutorials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.595057 tensorpc-0.10.2/tensorpc/flow/
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    17924 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/client.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.599057 tensorpc-0.10.2/tensorpc/flow/close_langserv/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/close_langserv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      773 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/close_langserv/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2281 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/constants.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7240 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/coretypes.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.599057 tensorpc-0.10.2/tensorpc/flow/flowapp/
+-rw-r--r--   0 runner    (1001) docker     (127)      849 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    76779 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8905 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/appcore.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.599057 tensorpc-0.10.2/tensorpc/flow/flowapp/appctx/
+-rw-r--r--   0 runner    (1001) docker     (127)      154 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/appctx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2897 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/appctx/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5762 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/appctx/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7068 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/appctx/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6172 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/colors.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.603057 tensorpc-0.10.2/tensorpc/flow/flowapp/components/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      234 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/annocore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7405 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2584 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13130 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/leaflet.py
+-rw-r--r--   0 runner    (1001) docker     (127)   178760 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/mui.py
+-rw-r--r--   0 runner    (1001) docker     (127)    15273 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plotly.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.607056 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/
+-rw-r--r--   0 runner    (1001) docker     (127)     1490 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      793 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/arraycommon.py
+-rw-r--r--   0 runner    (1001) docker     (127)    22472 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/arraygrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)    32169 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3628 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)       51 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)    26537 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/config.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3908 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5028 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/figure.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16189 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/grid_preview_layout.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.607056 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/handlers/
+-rw-r--r--   0 runner    (1001) docker     (127)       45 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/handlers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    10741 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/handlers/common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5494 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/handlers/gv_common.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6902 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/monitor.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.607056 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/objinspect/
+-rw-r--r--   0 runner    (1001) docker     (127)      497 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/objinspect/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18922 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/objinspect/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5348 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/objinspect/controllers.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24337 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/objinspect/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (127)      970 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/objinspect/inspectpanel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8363 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/objinspect/layout.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/objinspect/reload.py
+-rw-r--r--   0 runner    (1001) docker     (127)    44599 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/objinspect/tree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8058 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/objinspect/treeitems.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1106 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/options.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1719 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/reload_utils.py
+-rw-r--r--   0 runner    (1001) docker     (127)    16020 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (127)    13938 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/scriptmgr.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3422 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/sliders.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8583 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/tutorials.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.611056 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/vis/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/vis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    56801 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/vis/canvas.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6316 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/vis/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4713 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/vis/treeview.py
+-rw-r--r--   0 runner    (1001) docker     (127)    27521 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/vis/vapi_core.py
+-rw-r--r--   0 runner    (1001) docker     (127)   144462 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/three.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1239 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/threecore.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1906 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/components/typemetas.py
+-rw-r--r--   0 runner    (1001) docker     (127)    79929 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)      305 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/coretypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9629 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/objtree.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8238 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/flowapp/reload.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.611056 tensorpc-0.10.2/tensorpc/flow/init_langserv/
+-rw-r--r--   0 runner    (1001) docker     (127)      575 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/init_langserv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      266 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/init_langserv/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    24688 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/jsonlike.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.611056 tensorpc-0.10.2/tensorpc/flow/langserv/
+-rw-r--r--   0 runner    (1001) docker     (127)       78 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/langserv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3843 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/langserv/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6845 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/langserv/pyls.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1781 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/langserv/pyrightcfg.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2956 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/marker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.611056 tensorpc-0.10.2/tensorpc/flow/runapp/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/runapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1105 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/runapp/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.611056 tensorpc-0.10.2/tensorpc/flow/sampleapp/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/sampleapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)    59344 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/sampleapp/app.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5225 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/sampleapp/arraygrid.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/sampleapp/collection.py
+-rw-r--r--   0 runner    (1001) docker     (127)    41653 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/sampleapp/d3.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2402 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/sampleapp/file.py
+-rw-r--r--   0 runner    (1001) docker     (127)      470 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/sampleapp/sample_preview.py
+-rw-r--r--   0 runner    (1001) docker     (127)      994 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/sampleapp/sample_reload_fn.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5279 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/sampleapp/v_nextgen.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.615056 tensorpc-0.10.2/tensorpc/flow/serv/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/serv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)   105758 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/serv/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)    18787 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/serv/flowapp.py
+-rw-r--r--   0 runner    (1001) docker     (127)    29044 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/serv/worker.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8826 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/flow/serv_names.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/marker.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.615056 tensorpc-0.10.2/tensorpc/protos/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/protos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2196 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/protos/arraybuf_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/protos/arraybuf_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      158 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/protos/arraybuf_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2595 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/protos/remote_object_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      215 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/protos/remote_object_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)    21852 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/protos/remote_object_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3906 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/protos/rpc_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/protos/rpc_message_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     1157 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/protos/wsdef_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/protos/wsdef_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)      334 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/protos_export.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.615056 tensorpc-0.10.2/tensorpc/protos_legacy/
+-rw-r--r--   0 runner    (1001) docker     (127)      101 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/protos_legacy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9604 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/protos_legacy/arraybuf_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2242 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/protos_legacy/arraybuf_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     6759 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/protos_legacy/remote_object_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)    11472 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/protos_legacy/remote_object_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (127)    25985 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/protos_legacy/rpc_message_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5647 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/protos_legacy/rpc_message_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (127)     3888 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/protos_legacy/wsdef_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (127)      936 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/protos_legacy/wsdef_pb2.pyi
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.619057 tensorpc-0.10.2/tensorpc/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)       63 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/scheduler/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.619057 tensorpc-0.10.2/tensorpc/serve/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/serve/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1923 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/serve/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.619057 tensorpc-0.10.2/tensorpc/serve/flowapp_script/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/serve/flowapp_script/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1009 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/serve/flowapp_script/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.619057 tensorpc-0.10.2/tensorpc/serve_sync/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/serve_sync/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1819 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/serve_sync/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.619057 tensorpc-0.10.2/tensorpc/services/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/services/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3559 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/services/collection.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.619057 tensorpc-0.10.2/tensorpc/services/flow/
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/services/flow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      571 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/services/flow/core.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1880 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/services/for_test.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1671 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/services/vis.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4581 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.623057 tensorpc-0.10.2/tensorpc/utils/
+-rw-r--r--   0 runner    (1001) docker     (127)     1131 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/utils/address.py
+-rw-r--r--   0 runner    (1001) docker     (127)     9344 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/utils/df_logging.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1704 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/utils/gpuusage.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3215 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/utils/registry.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2447 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/utils/reload.py
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/utils/subproc.py
+-rw-r--r--   0 runner    (1001) docker     (127)      491 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/utils/typeutils.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1403 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/utils/uniquename.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2599 2024-04-18 06:06:51.000000 tensorpc-0.10.2/tensorpc/utils/wait_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.623057 tensorpc-0.10.2/tensorpc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     2105 2024-04-18 06:07:23.000000 tensorpc-0.10.2/tensorpc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)    12013 2024-04-18 06:07:23.000000 tensorpc-0.10.2/tensorpc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-18 06:07:23.000000 tensorpc-0.10.2/tensorpc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      381 2024-04-18 06:07:23.000000 tensorpc-0.10.2/tensorpc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-18 06:07:23.000000 tensorpc-0.10.2/tensorpc.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-18 06:07:23.623057 tensorpc-0.10.2/test/
+-rw-r--r--   0 runner    (1001) docker     (127)     4898 2024-04-18 06:06:51.000000 tensorpc-0.10.2/test/test_tmux_scheduler.py
```

### Comparing `tensorpc-0.10.1/LICENSE` & `tensorpc-0.10.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/PKG-INFO` & `tensorpc-0.10.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorpc
-Version: 0.10.1
+Version: 0.10.2
 Summary: Backend for devflow.
 Home-page: https://github.com/FindDefinition/tensorpc
 Author: Yan Yan
 Author-email: yanyan.sub@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `tensorpc-0.10.1/README.md` & `tensorpc-0.10.2/README.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/setup.py` & `tensorpc-0.10.2/setup.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/__init__.py` & `tensorpc-0.10.2/tensorpc/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/__main__.py` & `tensorpc-0.10.2/tensorpc/__main__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/apps/__init__.py` & `tensorpc-0.10.2/tensorpc/apps/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/apps/cbvc/__init__.py` & `tensorpc-0.10.2/tensorpc/apps/cbvc/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/apps/file/__init__.py` & `tensorpc-0.10.2/tensorpc/apps/file/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/autossh/__init__.py` & `tensorpc-0.10.2/tensorpc/autossh/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/autossh/constants.py` & `tensorpc-0.10.2/tensorpc/autossh/constants.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/autossh/core.py` & `tensorpc-0.10.2/tensorpc/autossh/core.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/autossh/coretypes.py` & `tensorpc-0.10.2/tensorpc/autossh/coretypes.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/autossh/media/hooks-bash-legacy.sh` & `tensorpc-0.10.2/tensorpc/autossh/media/hooks-bash-legacy.sh`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/autossh/media/hooks-bash.sh` & `tensorpc-0.10.2/tensorpc/autossh/media/hooks-bash.sh`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/autossh/scheduler/client.py` & `tensorpc-0.10.2/tensorpc/autossh/scheduler/client.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/autossh/scheduler/constants.py` & `tensorpc-0.10.2/tensorpc/autossh/scheduler/constants.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/autossh/scheduler/core.py` & `tensorpc-0.10.2/tensorpc/autossh/scheduler/core.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/autossh/scheduler/runtask/__main__.py` & `tensorpc-0.10.2/tensorpc/autossh/scheduler/runtask/__main__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/autossh/scheduler/task_client.py` & `tensorpc-0.10.2/tensorpc/autossh/scheduler/task_client.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/autossh/scheduler/tmux.py` & `tensorpc-0.10.2/tensorpc/autossh/scheduler/tmux.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/autossh/serv_names.py` & `tensorpc-0.10.2/tensorpc/autossh/serv_names.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/autossh/services/__init__.py` & `tensorpc-0.10.2/tensorpc/autossh/services/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/autossh/services/scheduler.py` & `tensorpc-0.10.2/tensorpc/autossh/services/scheduler.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/cli/cpuusage/__init__.py` & `tensorpc-0.10.2/tensorpc/cli/cpuusage/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/cli/cpuusage/__main__.py` & `tensorpc-0.10.2/tensorpc/cli/cpuusage/__main__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/cli/createmsg/__init__.py` & `tensorpc-0.10.2/tensorpc/cli/createmsg/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/cli/createmsg/__main__.py` & `tensorpc-0.10.2/tensorpc/cli/createmsg/__main__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/cli/free_port/__init__.py` & `tensorpc-0.10.2/tensorpc/cli/free_port/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/cli/gpuusage/__init__.py` & `tensorpc-0.10.2/tensorpc/cli/gpuusage/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/cli/gpuusage/__main__.py` & `tensorpc-0.10.2/tensorpc/cli/gpuusage/__main__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/cli/iperf/__main__.py` & `tensorpc-0.10.2/tensorpc/cli/iperf/__main__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/cli/ping/__init__.py` & `tensorpc-0.10.2/tensorpc/cli/ping/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/cli/proto_files/__init__.py` & `tensorpc-0.10.2/tensorpc/cli/proto_files/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/cli/proto_files/__main__.py` & `tensorpc-0.10.2/tensorpc/cli/proto_files/__main__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/cli/proto_root/__init__.py` & `tensorpc-0.10.2/tensorpc/cli/proto_root/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/cli/proto_root/__main__.py` & `tensorpc-0.10.2/tensorpc/cli/proto_root/__main__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/cli/pyls/__init__.py` & `tensorpc-0.10.2/tensorpc/cli/pyls/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/cli/pyright_launch/__init__.py` & `tensorpc-0.10.2/tensorpc/cli/pyright_launch/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/cli/start_worker/__init__.py` & `tensorpc-0.10.2/tensorpc/cli/start_worker/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/cli/start_worker/__main__.py` & `tensorpc-0.10.2/tensorpc/cli/start_worker/__main__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/compat.py` & `tensorpc-0.10.2/tensorpc/compat.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/constants.py` & `tensorpc-0.10.2/tensorpc/constants.py`

 * *Files 14% similar despite different names*

```diff
@@ -19,7 +19,8 @@
 
 TENSORPC_READUNTIL = "__tensorpc_readuntil_string"
 
 TENSORPC_FILE_NAME_PREFIX = "__tensorpc_inmemory_fname"
 
 TENSORPC_OBSERVED_FUNCTION_ATTR = "__tensorpc_observed_function__"
 
+TENSORPC_PORT_MAX_TRY = 15
```

### Comparing `tensorpc-0.10.1/tensorpc/core/__init__.py` & `tensorpc-0.10.2/tensorpc/core/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/core/asyncclient.py` & `tensorpc-0.10.2/tensorpc/core/asyncclient.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/core/asyncserver.py` & `tensorpc-0.10.2/tensorpc/core/asyncserver.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,32 +14,35 @@
 """The Python implementation of the GRPC RemoteCall.RemoteObject server."""
 
 import asyncio
 import json
 import os
 import time
 from functools import partial
-from typing import Callable, Dict, List, Mapping, Optional, Sequence, Union
+from typing import Callable, Dict, List, Mapping, Optional, Sequence, Tuple, Union
 
 import grpc
 import grpc.aio
 import numpy as np
 
 from tensorpc import compat
+from tensorpc.constants import TENSORPC_PORT_MAX_TRY
 from tensorpc.core.defs import ServiceDef
 from tensorpc.core.server_core import ProtobufServiceCore, ServerMeta
 from tensorpc.protos_export import remote_object_pb2 as remote_object_pb2
 from tensorpc.protos_export import rpc_message_pb2
 from tensorpc.protos_export import \
     remote_object_pb2_grpc as remote_object_pb2_grpc
 from tensorpc.utils.df_logging import get_logger
 from tensorpc.core.httpservers import aiohttp_impl as httpserver
 # from tensorpc.core.httpservers import blacksheep_impl as httpserver
 import aiohttp
 
+from tensorpc.utils.wait_tools import get_free_ports
+
 LOGGER = get_logger()
 
 _ONE_DAY_IN_SECONDS = 60 * 60 * 24
 
 
 class AsyncRemoteObjectService(remote_object_pb2_grpc.RemoteObjectServicer):
     """Main service of codeai.distributed. Arbitrary python code execute service.
@@ -126,44 +129,59 @@
                         wait_time=-1,
                         port=50051,
                         length=-1,
                         is_local=False,
                         max_threads=10,
                         process_id=-1,
                         ssl_key_path: str = "",
-                        ssl_crt_path: str = ""):
+                        ssl_crt_path: str = "",
+                        grpc_options: Optional[List[Tuple[str, Union[str, int]]]] = None):
     assert isinstance(service, AsyncRemoteObjectService)
     if is_local and process_id >= 0:
         if hasattr(os, "sched_setaffinity"):
             # lock process to cpu to increase performance.
             LOGGER.info("lock worker {} to core {}".format(
                 process_id, process_id))
             os.sched_setaffinity(0, [process_id])
     wait_interval = _ONE_DAY_IN_SECONDS
     if wait_time > 0:
         wait_interval = wait_time
-    options = None
+    options = []
     if length > 0:
         options = [('grpc.max_send_message_length', length * 1024 * 1024),
                    ('grpc.max_receive_message_length', length * 1024 * 1024)]
+    options.append(('grpc.so_reuseport', 0))
+    if grpc_options is not None:
+        options = grpc_options # override
     server = grpc.aio.server(options=options)
     remote_object_pb2_grpc.add_RemoteObjectServicer_to_server(service, server)
-    url = '[::]:{}'.format(port)
     credentials = None
     if ssl_key_path != "" and ssl_key_path != "":
         with open(ssl_key_path, "rb") as f:
             private_key = f.read()
         with open(ssl_crt_path, "rb") as f:
             certificate_chain = f.read()
         credentials = grpc.ssl_server_credentials([(private_key,
                                                     certificate_chain)])
-    if credentials is not None:
-        server.add_secure_port(url, credentials)
-    else:
-        server.add_insecure_port(url)
+    
+    for i in range(TENSORPC_PORT_MAX_TRY):
+        if port == -1:
+            port = get_free_ports(1)[0]
+        url = '[::]:{}'.format(port)
+        try:
+            if credentials is not None:
+                server.add_secure_port(url, credentials)
+            else:
+                server.add_insecure_port(url)
+            LOGGER.info("server started at {}".format(url))
+            break
+        except:
+            port = -1
+    if port == -1:
+        raise RuntimeError("Cannot find free port")
 
     await server.start()
     loop = asyncio.get_running_loop()
     server_core = service.server_core
 
     async def server_graceful_shutdown():
         # Shuts down the server with 5 seconds of grace period. During the
```

### Comparing `tensorpc-0.10.1/tensorpc/core/client.py` & `tensorpc-0.10.2/tensorpc/core/client.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/core/core_io.py` & `tensorpc-0.10.2/tensorpc/core/core_io.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/core/defs.py` & `tensorpc-0.10.2/tensorpc/core/defs.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/core/event_emitter/aio.py` & `tensorpc-0.10.2/tensorpc/core/event_emitter/aio.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/core/event_emitter/base.py` & `tensorpc-0.10.2/tensorpc/core/event_emitter/base.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/core/funcid.py` & `tensorpc-0.10.2/tensorpc/core/funcid.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/core/httpclient.py` & `tensorpc-0.10.2/tensorpc/core/httpclient.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/core/httpservers/aiohttp_impl.py` & `tensorpc-0.10.2/tensorpc/core/httpservers/aiohttp_impl.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/core/httpservers/all.py` & `tensorpc-0.10.2/tensorpc/core/httpservers/all.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/core/httpservers/blacksheep_impl.py` & `tensorpc-0.10.2/tensorpc/core/httpservers/blacksheep_impl.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/core/httpservers/core.py` & `tensorpc-0.10.2/tensorpc/core/httpservers/core.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/core/inspecttools.py` & `tensorpc-0.10.2/tensorpc/core/inspecttools.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/core/marker.py` & `tensorpc-0.10.2/tensorpc/core/marker.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/core/moduleid.py` & `tensorpc-0.10.2/tensorpc/core/moduleid.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/core/prim.py` & `tensorpc-0.10.2/tensorpc/core/prim.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/core/server.py` & `tensorpc-0.10.2/tensorpc/core/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -16,28 +16,30 @@
 import asyncio
 import json
 import os
 import threading
 import time
 import traceback
 from concurrent import futures
-from typing import Callable, Dict, List, Mapping, Optional, Sequence, Union
+from typing import Callable, Dict, List, Mapping, Optional, Sequence, Tuple, Union
 
 import grpc
 import numpy as np
+from tensorpc.constants import TENSORPC_PORT_MAX_TRY
 from tensorpc.core.defs import ServiceDef
 
 from tensorpc.core.server_core import ProtobufServiceCore, ServerMeta
 
 from tensorpc.protos_export import remote_object_pb2 as remote_object_pb2
 from tensorpc.protos_export import rpc_message_pb2
 
 from tensorpc.protos_export import \
     remote_object_pb2_grpc as remote_object_pb2_grpc
 from tensorpc.utils.df_logging import get_logger
+from tensorpc.utils.wait_tools import get_free_ports
 
 LOGGER = get_logger()
 
 _ONE_DAY_IN_SECONDS = 60 * 60 * 24
 
 
 class RemoteObjectService(remote_object_pb2_grpc.RemoteObjectServicer):
@@ -126,37 +128,52 @@
 def serve_service(service: RemoteObjectService,
                   wait_time=-1,
                   port=50051,
                   length=-1,
                   is_local=False,
                   max_threads=10,
                   process_id=-1,
-                  credentials=None):
+                  credentials=None,
+                  grpc_options: Optional[List[Tuple[str, Union[str, int]]]] = None):
     assert isinstance(service, RemoteObjectService)
     if is_local and process_id >= 0:
         if hasattr(os, "sched_setaffinity"):
             # lock process to cpu to increase performance.
             LOGGER.info("lock worker {} to core {}".format(
                 process_id, process_id))
             os.sched_setaffinity(0, [process_id])
     wait_interval = _ONE_DAY_IN_SECONDS
     if wait_time > 0:
         wait_interval = wait_time
-    options = None
+    options = []
     if length > 0:
         options = [('grpc.max_send_message_length', length * 1024 * 1024),
                    ('grpc.max_receive_message_length', length * 1024 * 1024)]
+    options.append(('grpc.so_reuseport', 0))
+    if grpc_options is not None:
+        options = grpc_options # override
     server = grpc.server(futures.ThreadPoolExecutor(max_workers=max_threads),
                          options=options)
-    url = '[::]:{}'.format(port)
     remote_object_pb2_grpc.add_RemoteObjectServicer_to_server(service, server)
-    if credentials is not None:
-        server.add_secure_port(url, credentials)
-    else:
-        server.add_insecure_port(url)
+    for i in range(TENSORPC_PORT_MAX_TRY):
+        if port == -1:
+            port = get_free_ports(1)[0]
+        url = '[::]:{}'.format(port)
+        try:
+            if credentials is not None:
+                server.add_secure_port(url, credentials)
+            else:
+                server.add_insecure_port(url)
+            LOGGER.info("server started at {}".format(url))
+            break
+        except:
+            port = -1
+    if port == -1:
+        raise RuntimeError("Cannot find free port")
+
     server.start()
     server_core = service.server_core
     try:
         while True:
             # looks like event return false instead of raise timeouterror
             if server_core.shutdown_event.wait(wait_interval):
                 break
```

### Comparing `tensorpc-0.10.1/tensorpc/core/server_core.py` & `tensorpc-0.10.2/tensorpc/core/server_core.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/core/serviceunit.py` & `tensorpc-0.10.2/tensorpc/core/serviceunit.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/core/tracer.py` & `tensorpc-0.10.2/tensorpc/core/tracer.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,14 +25,15 @@
     filename: str
     lineno: int
     local_vars: Mapping[str, Any]
     # depth only available when trace return (slower mode).
     depth: int = -1
     module_qname: str = ""
     timestamp: int = -1
+    c_call_obj: Optional[object] = None
 
     def get_unique_id(self):
         return f"{self.filename}@:{self.lineno}{self.qualname}"
 
 
 class Tracer(object):
     """A simple tracer for python functions.
@@ -46,14 +47,15 @@
                  callback: Callable[[FrameResult], Any],
                  traced_types: Optional[Tuple[Type]] = None,
                  traced_names: Optional[Set[str]] = None,
                  traced_folders: Optional[Set[str]] = None,
                  trace_return: bool = True,
                  depth: int = 5,
                  ignored_names: Optional[Set[str]] = None,
+                 use_profile: bool = False,
                  *,
                  _frame_cnt: int = 1):
         self.target_frames: Set[FrameType] = set()
         self.thread_local = threading.local()
         self.depth = depth
         self.traced_types = traced_types
         self.traced_names = traced_names
@@ -65,14 +67,15 @@
         self.traced_folders: Optional[Set[Path]] = None
         self.trace_return = trace_return
         self.callback = callback
         if traced_folders is not None and len(traced_folders) > 0:
             self.traced_folders = set(
                 Path(folder) for folder in traced_folders)
         self._frame_cnt = _frame_cnt
+        self.use_profile = use_profile
 
         self._inner_frame_fnames: Set[str] = set([Tracer.__enter__.__code__.co_filename])
 
     def _filter_frame(self, frame: FrameType):
         if frame.f_code in self.code_res:
             return self.code_res[frame.f_code][0]
         is_traced_types = True
@@ -141,20 +144,26 @@
         if not self._is_internal_frame(calling_frame):
             calling_frame.f_trace = trace_fn
             self.target_frames.add(calling_frame)
 
         stack = self.thread_local.__dict__.setdefault(
             'original_trace_functions', [])
         stack.append(sys.gettrace())
-        sys.settrace(trace_fn)
+        if self.use_profile:
+            sys.setprofile(trace_fn)
+        else:
+            sys.settrace(trace_fn)
 
     def __exit__(self, exc_type, exc_value, exc_traceback):
         # print("EXIT", self._frame_cnt, self._inner_frame_fnames, self.target_frames)
         stack = self.thread_local.original_trace_functions
-        sys.settrace(stack.pop())
+        if self.use_profile:
+            sys.setprofile(stack.pop())
+        else:
+            sys.settrace(stack.pop())
         cur_frame = inspect.currentframe()
         assert cur_frame is not None
         frame = cur_frame
         _frame_cnt = self._frame_cnt
         while _frame_cnt > 0:
             frame = cur_frame.f_back
             assert frame is not None
@@ -164,22 +173,21 @@
         assert calling_frame is not None
         self.target_frames.discard(calling_frame)
 
     def _is_internal_frame(self, frame: FrameType):
         return frame.f_code.co_filename in self._inner_frame_fnames
 
     def trace_lite(self, frame: FrameType, event, arg):
-        # print(frame.f_code.co_name, event, frame.f_lineno)
         if event == 'return':
             THREAD_GLOBALS.depth -= 1
             # print(event, frame.f_code.co_name, "THREAD_GLOBALS.depth", THREAD_GLOBALS.depth)
             self.callback(self.get_frame_result(TraceType.Return, frame, THREAD_GLOBALS.depth))
 
     @staticmethod
-    def get_frame_result(trace_type: TraceType, frame: FrameType, depth: int=-1):
+    def get_frame_result(trace_type: TraceType, frame: FrameType, depth: int=-1, c_call_obj: Optional[object]=None):
         qname = frame.f_code.co_name
         if sys.version_info[:2] >= (3, 11):
             qname = frame.f_code.co_qualname # type: ignore
         else:
             if "self" in frame.f_locals:
                 qname = type(frame.f_locals["self"]).__qualname__ + "." + qname                
         module = inspect.getmodule(frame)
@@ -191,14 +199,15 @@
             qualname=qname,
             filename=frame.f_code.co_filename,
             lineno=frame.f_lineno,
             local_vars=frame.f_locals.copy(),
             depth=depth,
             module_qname=module_qname,
             timestamp=time.time_ns(),
+            c_call_obj=c_call_obj,
         )
 
     def trace_call_func(self, frame: FrameType, event, arg):
         if not (frame in self.target_frames):
             if self.depth == 1:
                 # We did the most common and quickest check above, because the
                 # trace function runs so incredibly often, therefore it's
@@ -222,14 +231,16 @@
             return None
         if event == "call":
             self.callback(self.get_frame_result(TraceType.Call, frame))
         return None
 
     def trace_return_func(self, frame: FrameType, event, arg):
         # print(event, frame.f_code.co_name, self.target_frames, frame.f_code.co_filename, self._is_internal_frame(frame))
+        # if arg is not None and event == "c_call":
+        #     print(get_qualname_of_type(arg))
 
         if not (frame in self.target_frames):
             if self.depth == 1:
                 # We did the most common and quickest check above, because the
                 # trace function runs so incredibly often, therefore it's
                 # crucial to hyper-optimize it for the common case.
                 return None
```

### Comparing `tensorpc-0.10.1/tensorpc/core/tree_id.py` & `tensorpc-0.10.2/tensorpc/core/tree_id.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/__init__.py` & `tensorpc-0.10.2/tensorpc/examples/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/ai/__init__.py` & `tensorpc-0.10.2/tensorpc/examples/ai/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/ai/engine.py` & `tensorpc-0.10.2/tensorpc/examples/ai/engine.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.10-Template Component.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.10-Template Component.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.11-Inheritance.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.11-Inheritance.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.12-App Context.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.12-App Context.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.13-Component Context.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.13-Component Context.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.14-Host Resource.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.14-Host Resource.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.2-App Basic Architecture.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.2-App Basic Architecture.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.3-Flex Box Basic.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.3-Flex Box Basic.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.4-Containers.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.4-Containers.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.5-Advanced Events.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.5-Advanced Events.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.6-Composite Component.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.6-Composite Component.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.7-Advanced UI Methods.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.7-Advanced UI Methods.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.8-Drag And Drop.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.8-Drag And Drop.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/01-basic/1.9-Reload System.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/01-basic/1.9-Reload System.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.0-Common Props.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.0-Common Props.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.1-Button.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.1-Button.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.10-Slider.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.10-Slider.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.11-Tab.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.11-Tab.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.12-Drawer.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.12-Drawer.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.13-Dialog.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.13-Dialog.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.14-Collapse.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.14-Collapse.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.15-Chip.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.15-Chip.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.16-Progress.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.16-Progress.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.17-MenuList.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.17-MenuList.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.2-Typography.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.2-Typography.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.22-DataGrid.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.22-DataGrid.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.25-Plotly.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.25-Plotly.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.26-Map.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.26-Map.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.3-Markdown.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.3-Markdown.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.4-TextField.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.4-TextField.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.5-List.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.5-List.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.6-Select.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.6-Select.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.7-AutoComplete.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.7-AutoComplete.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.8-ToggleButton.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.8-ToggleButton.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/02-components/2.9-Image.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/02-components/2.9-Image.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/03-3d basic/3.1-Hello 3D World.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/03-3d basic/3.1-Hello 3D World.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials/07-V Api/7.1-Basic.md` & `tensorpc-0.10.2/tensorpc/examples/tutorials/07-V Api/7.1-Basic.md`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/examples/tutorials.py` & `tensorpc-0.10.2/tensorpc/examples/tutorials.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/__init__.py` & `tensorpc-0.10.2/tensorpc/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/client.py` & `tensorpc-0.10.2/tensorpc/flow/client.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/close_langserv/__main__.py` & `tensorpc-0.10.2/tensorpc/flow/close_langserv/__main__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/constants.py` & `tensorpc-0.10.2/tensorpc/flow/constants.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/coretypes.py` & `tensorpc-0.10.2/tensorpc/flow/coretypes.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/__init__.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/app.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/app.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/appcore.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/appcore.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/appctx/canvas.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/appctx/canvas.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/appctx/core.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/appctx/core.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/appctx/inspector.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/appctx/inspector.py`

 * *Files 7% similar despite different names*

```diff
@@ -56,14 +56,15 @@
                key: str = "trace",
                traced_types: Optional[Tuple[Type]] = None,
                traced_names: Optional[Set[str]] = None,
                traced_folders: Optional[Set[str]] = None,
                trace_return: bool = True,
                depth: int = 5,
                use_return_locals: bool = False,
+               use_profile: bool = False,
                *,
                _frame_cnt=5):
     """trace, store call vars, then write result to ObjectInspector.
     """
     comp = find_component(plus.ObjectInspector)
     if comp is None:
         yield
@@ -74,26 +75,28 @@
                          traced_types,
                          traced_names,
                          traced_folders,
                          trace_return,
                          depth,
                          use_return_locals,
                          _frame_cnt=_frame_cnt,
+                         use_profile=use_profile,
                          loop=get_app()._loop):
         yield
 
 
 @contextlib.contextmanager
 def trace_sync_return(traced_locs: List[Union[str, Path, types.ModuleType]],
                       key: str = "trace",
                       traced_types: Optional[Tuple[Type]] = None,
                       traced_names: Optional[Set[str]] = None,
                       traced_folders: Optional[Set[str]] = None,
                       trace_return: bool = True,
                       depth: int = 5,
+                      use_profile: bool = False,
                       *,
                       _frame_cnt=5):
     """trace, store local vars in return stmt, then write result to ObjectInspector.
     """
     comp = find_component(plus.ObjectInspector)
     if comp is None:
         yield
@@ -103,28 +106,30 @@
                          key,
                          traced_types,
                          traced_names,
                          traced_folders,
                          trace_return,
                          depth,
                          True,
+                         use_profile=use_profile,
                          _frame_cnt=_frame_cnt,
                          loop=get_app()._loop):
         yield
 
 
 @contextlib.asynccontextmanager
 async def trace(traced_locs: List[Union[str, Path, types.ModuleType]],
                 key: str = "trace",
                 traced_types: Optional[Tuple[Type]] = None,
                 traced_names: Optional[Set[str]] = None,
                 traced_folders: Optional[Set[str]] = None,
                 trace_return: bool = True,
                 depth: int = 5,
                 use_return_locals: bool = False,
+                use_profile: bool = False,
                 *,
                 _frame_cnt=5):
     """async trace, store local vars / args in return stmt, then write result to ObjectInspector.
     """
     comp = find_component(plus.ObjectInspector)
     if comp is None:
         yield
@@ -134,14 +139,15 @@
                           key,
                           traced_types,
                           traced_names,
                           traced_folders,
                           trace_return,
                           depth,
                           use_return_locals,
+                          use_profile=use_profile,
                           _frame_cnt=_frame_cnt):
         yield
 
 
 async def set_object(obj, key: str, expand_level: int = 0):
     comp = find_component(plus.ObjectInspector)
     if comp is None:
```

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/colors.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/colors.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/__init__.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/common.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/common.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/core.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/core.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/leaflet.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/leaflet.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/mui.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/mui.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plotly.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plotly.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/__init__.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/arraycommon.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/arraycommon.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/arraygrid.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/arraygrid.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/canvas.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/canvas.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/collection.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/collection.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/config.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/config.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/core.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/core.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/figure.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/figure.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/grid_preview_layout.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/grid_preview_layout.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/handlers/common.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/handlers/common.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/handlers/gv_common.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/handlers/gv_common.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/monitor.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/monitor.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/objinspect/analysis.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/objinspect/analysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -108,15 +108,15 @@
         elif isinstance(obj, dict):
             # return {k: v for k, v in obj.items() if not _is_obj_builtin_or_module(v)}
             return obj
         elif isinstance(obj, tuple(USER_OBJ_TREE_TYPES)):
             return obj.get_childs()
         elif isinstance(obj, TreeItem):
             # this is very special, we need to lazy access the child of a treeitem.
-            return await obj.get_child_desps() 
+            return await obj.get_child_desps(UniqueTreeIdForTree("")) 
         if self.custom_tree_item_handler is not None:
             res_tmp = await self.custom_tree_item_handler.get_childs(obj)
             if res_tmp is not None:
                 return res_tmp
         for k, v in self._custom_type_expanders.items():
             if isinstance(obj, k):
                 return v(obj)
@@ -131,19 +131,19 @@
     async def parse_obj_to_tree_node(self, obj, name: str, obj_meta_cache=None):
         obj_type = type(obj)
         try:
             isinst = isinstance(obj, TreeItem)
         except:
             print("???", type(obj))
             raise 
+        uid_name = UniqueTreeIdForTree.from_parts([name])
         if isinst:
-            node_candidate = obj.get_json_like_node()
+            node_candidate = obj.get_json_like_node(uid_name)
             if node_candidate is not None:
                 return node_candidate
-        uid_name = UniqueTreeIdForTree.from_parts([name])
         node = parse_obj_to_jsonlike(obj, name, uid_name)
         if isinstance(obj, mui.JsonLikeNode):
             return node
         if node.type == mui.JsonLikeType.Object.value:
             t = mui.JsonLikeType.Object
             value = mui.undefined
             count = 1  # make object expandable
@@ -214,18 +214,18 @@
 
     async def parse_obj_to_tree(self, obj, node: mui.JsonLikeNode, total_expand_level: int = 0):
         """parse object to json like tree.
         """
         if not self._should_expand_node(obj, node, total_expand_level):
             return 
         if isinstance(obj, TreeItem):
-            obj_dict = await obj.get_child_desps()
-            for k, v in obj_dict.items():
-                # v.id = f"{node.id}{GLOBAL_SPLIT}{v.id}"
-                v.id = node.id + v.id
+            obj_dict = await obj.get_child_desps(node.id)
+            # for k, v in obj_dict.items():
+            #     # v.id = f"{node.id}{GLOBAL_SPLIT}{v.id}"
+            #     v.id = node.id + v.id
             tree_children = list(obj_dict.values())
         else:
             obj_dict = await self.expand_object(obj)
             tree_children = await self.parse_obj_dict_to_nodes(obj_dict, node.id, self._obj_meta_cache)
         node.children = tree_children
         node.cnt = len(obj_dict)
         for (k, v), child_node in zip(obj_dict.items(), node.children):
```

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/objinspect/controllers.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/objinspect/controllers.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/objinspect/inspector.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/objinspect/inspector.py`

 * *Files 2% similar despite different names*

```diff
@@ -470,14 +470,15 @@
                    traced_types: Optional[Tuple[Type]] = None,
                    traced_names: Optional[Set[str]] = None,
                    traced_folders: Optional[Set[str]] = None,
                    trace_return: bool = True,
                    depth: int = 5,
                    use_return_locals: bool = False,
                    ignored_names: Optional[Set[str]] = None,
+                    use_profile: bool = False,
                    *,
                    _frame_cnt=3,
                    loop: Optional[asyncio.AbstractEventLoop] = None):
         if traced_folders is None:
             traced_folders = set()
         traced_folders.update(_parse_trace_modules(traced_locs))
         trace_res: List[FrameResult] = []
@@ -488,15 +489,16 @@
         tracer = Tracer(lambda x: trace_res.append(x),
                         traced_types,
                         traced_names,
                         traced_folders,
                         trace_return,
                         depth,
                         ignored_names,
-                        _frame_cnt=_frame_cnt)
+                        _frame_cnt=_frame_cnt,
+                        use_profile=use_profile)
         try:
             with tracer:
                 yield
         finally:
             tree_items = parse_frame_result_to_trace_item(
                 trace_res, use_return_locals)
             show_dict = {v.get_uid(): v for v in tree_items}
@@ -508,14 +510,15 @@
                           key: str = "trace",
                           traced_types: Optional[Tuple[Type]] = None,
                           traced_names: Optional[Set[str]] = None,
                           traced_folders: Optional[Set[str]] = None,
                           trace_return: bool = True,
                           depth: int = 5,
                           ignored_names: Optional[Set[str]] = None,
+                            use_profile: bool = False,
                           *,
                           _frame_cnt: int = 4,
                           loop: Optional[asyncio.AbstractEventLoop] = None):
         return self.trace_sync(traced_locs,
                                key,
                                traced_types,
                                traced_names,
@@ -534,30 +537,31 @@
                     traced_types: Optional[Tuple[Type]] = None,
                     traced_names: Optional[Set[str]] = None,
                     traced_folders: Optional[Set[str]] = None,
                     trace_return: bool = True,
                     depth: int = 5,
                     use_return_locals: bool = False,
                     ignored_names: Optional[Set[str]] = None,
+                    use_profile: bool = False,
                     *,
                     _frame_cnt: int = 3):
         if traced_folders is None:
             traced_folders = set()
         traced_folders.update(_parse_trace_modules(traced_locs))
         trace_res: List[FrameResult] = []
         tracer = Tracer(lambda x: trace_res.append(x),
                         traced_types,
                         traced_names,
                         traced_folders,
                         trace_return,
                         depth,
                         ignored_names,
+                        use_profile=use_profile,
                         _frame_cnt=_frame_cnt)
         try:
             with tracer:
-
                 yield
         finally:
             tree_items = parse_frame_result_to_trace_item(
                 trace_res, use_return_locals)
             show_dict = {v.get_uid(): v for v in tree_items}
             await self.set_object(show_dict, key)
```

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/objinspect/inspectpanel.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/objinspect/inspectpanel.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/objinspect/layout.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/objinspect/layout.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/objinspect/reload.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/objinspect/reload.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/objinspect/tree.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/objinspect/tree.py`

 * *Files 1% similar despite different names*

```diff
@@ -158,17 +158,18 @@
 class DataStorageTreeItem(TreeItem):
 
     def __init__(self, node_id: str, readable_id: str) -> None:
         super().__init__()
         self.node_id = node_id
         self.readable_id = readable_id
 
-    async def get_child_desps(self) -> Dict[str, mui.JsonLikeNode]:
+    async def get_child_desps(self, parent_ns: UniqueTreeIdForTree) -> Dict[str, mui.JsonLikeNode]:
         metas = await appctx.list_data_storage(self.node_id)
         for m in metas:
+            m.id = parent_ns + m.id
             userdata = {
                 "type": ContextMenuType.DataStorageItemDelete.value,
             }
             userdata_cpycmd = {
                 "type": ContextMenuType.DataStorageItemCommand.value,
             }
 
@@ -187,19 +188,19 @@
             #                         mui.IconType.Delete.value)]
         return {m.last_part(): m for m in metas}
 
     async def get_child(self, key: str) -> Any:
         res = await appctx.read_data_storage(key, self.node_id)
         return res
 
-    def get_json_like_node(self) -> Optional[mui.JsonLikeNode]:
+    def get_json_like_node(self, id: UniqueTreeIdForTree) -> Optional[mui.JsonLikeNode]:
         btns = [
             IconButtonData(ButtonType.Delete.value, mui.IconType.Delete.value)
         ]
-        return mui.JsonLikeNode(UniqueTreeIdForTree.from_parts([self.readable_id]),
+        return mui.JsonLikeNode(id + self.readable_id,
                                 self.readable_id,
                                 mui.JsonLikeType.Object.value,
                                 typeStr="DataStorageTreeItem",
                                 cnt=1,
                                 drag=False,
                                 iconBtns=btns)
 
@@ -237,18 +238,18 @@
 
     def __init__(self) -> None:
         super().__init__()
         self._watched_funcs: Set[str] = set()
 
     # async def get_childs(self):
 
-    async def get_child_desps(self) -> Dict[str, mui.JsonLikeNode]:
+    async def get_child_desps(self, parent_ns: UniqueTreeIdForTree) -> Dict[str, mui.JsonLikeNode]:
         metas: Dict[str, mui.JsonLikeNode] = {}
         for k, v in appctx.get_app().get_observed_func_registry().items():
-            node = mui.JsonLikeNode(UniqueTreeIdForTree.from_parts([k]), v.name,
+            node = mui.JsonLikeNode(parent_ns + k, v.name,
                                     mui.JsonLikeType.Function.value, alias=v.name)
             node.iconBtns = [
                 IconButtonData(ButtonType.Watch.value,
                                mui.IconType.Visibility.value, "Watch"),
                 IconButtonData(ButtonType.Record.value, mui.IconType.Mic.value,
                                "Record")
             ]
@@ -262,15 +263,15 @@
             node.value = value
             metas[k] = node
         return metas
 
     async def get_child(self, key: str) -> Any:
         return appctx.get_app().get_observed_func_registry()[key]
 
-    def get_json_like_node(self) -> Optional[mui.JsonLikeNode]:
+    def get_json_like_node(self, id: UniqueTreeIdForTree) -> Optional[mui.JsonLikeNode]:
         return mui.JsonLikeNode(UniqueTreeIdForTree.from_parts(["observedFunc"]),
                                 "observedFunc",
                                 mui.JsonLikeType.Object.value,
                                 typeStr="ObservedFunctions",
                                 cnt=1,
                                 drag=False)
 
@@ -536,18 +537,15 @@
                 node.children = node._get_divided_tree(self.limit, 0)
                 upd = self.tree.update_event(tree=self._objinspect_root)
                 return await self.tree.send_and_wait(upd)
             # if not found, we expand (update) the deepest valid object.
             # if the object is special (extend TreeItem), we use used-defined
             # function instead of analysis it.
             if isinstance(obj, TreeItem):
-                obj_dict_desp = await obj.get_child_desps()  
-                for k, v in obj_dict_desp.items():
-                    # v.id = f"{uid}{GLOBAL_SPLIT}{v.id}"
-                    v.id = uid + v.id
+                obj_dict_desp = await obj.get_child_desps(uid)  
                 obj_dict = {**obj_dict_desp}
                 tree = list(obj_dict_desp.values())
             else:
                 obj_dict = {**(await self._tree_parser.expand_object(obj))}
                 tree = await self._tree_parser.parse_obj_dict_to_nodes(obj_dict, node.id)
             node.children = tree
             upd = self.tree.update_event(tree=self._objinspect_root)
```

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/objinspect/treeitems.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/objinspect/treeitems.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/options.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/options.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/reload_utils.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/reload_utils.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/scheduler.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/scheduler.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/scriptmgr.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/scriptmgr.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/sliders.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/sliders.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/tutorials.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/tutorials.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/vis/canvas.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/vis/canvas.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/vis/core.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/vis/core.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/vis/treeview.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/vis/treeview.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/plus/vis/vapi_core.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/plus/vis/vapi_core.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/three.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/three.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/threecore.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/threecore.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/components/typemetas.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/components/typemetas.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/core.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/core.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/objtree.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/objtree.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/flowapp/reload.py` & `tensorpc-0.10.2/tensorpc/flow/flowapp/reload.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/init_langserv/__init__.py` & `tensorpc-0.10.2/tensorpc/flow/init_langserv/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/jsonlike.py` & `tensorpc-0.10.2/tensorpc/flow/jsonlike.py`

 * *Files 0% similar despite different names*

```diff
@@ -665,15 +665,15 @@
                             t.value,
                             value=value,
                             typeStr=obj_type.__qualname__)
 
 
 class TreeItem(abc.ABC):
     @abc.abstractmethod
-    async def get_child_desps(self) -> Dict[str, JsonLikeNode]:
+    async def get_child_desps(self, parent_ns: UniqueTreeIdForTree) -> Dict[str, JsonLikeNode]:
         raise NotImplementedError
 
     @abc.abstractmethod
     async def get_child(self, key: str) -> Any:
         raise NotImplementedError
 
     def get_json_like_node(self) -> Optional[JsonLikeNode]:
```

### Comparing `tensorpc-0.10.1/tensorpc/flow/langserv/core.py` & `tensorpc-0.10.2/tensorpc/flow/langserv/core.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/langserv/pyls.py` & `tensorpc-0.10.2/tensorpc/flow/langserv/pyls.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/langserv/pyrightcfg.py` & `tensorpc-0.10.2/tensorpc/flow/langserv/pyrightcfg.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/marker.py` & `tensorpc-0.10.2/tensorpc/flow/marker.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/runapp/__init__.py` & `tensorpc-0.10.2/tensorpc/flow/runapp/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/runapp/__main__.py` & `tensorpc-0.10.2/tensorpc/flow/runapp/__main__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/sampleapp/__init__.py` & `tensorpc-0.10.2/tensorpc/flow/sampleapp/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/sampleapp/app.py` & `tensorpc-0.10.2/tensorpc/flow/sampleapp/app.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/sampleapp/arraygrid.py` & `tensorpc-0.10.2/tensorpc/flow/sampleapp/arraygrid.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/sampleapp/collection.py` & `tensorpc-0.10.2/tensorpc/flow/sampleapp/collection.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/sampleapp/d3.py` & `tensorpc-0.10.2/tensorpc/flow/sampleapp/d3.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/sampleapp/file.py` & `tensorpc-0.10.2/tensorpc/flow/sampleapp/file.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/sampleapp/sample_reload_fn.py` & `tensorpc-0.10.2/tensorpc/flow/sampleapp/sample_reload_fn.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/sampleapp/v_nextgen.py` & `tensorpc-0.10.2/tensorpc/flow/sampleapp/v_nextgen.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/serv/__init__.py` & `tensorpc-0.10.2/tensorpc/flow/serv/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/serv/core.py` & `tensorpc-0.10.2/tensorpc/flow/serv/core.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/serv/flowapp.py` & `tensorpc-0.10.2/tensorpc/flow/serv/flowapp.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/serv/worker.py` & `tensorpc-0.10.2/tensorpc/flow/serv/worker.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/flow/serv_names.py` & `tensorpc-0.10.2/tensorpc/flow/serv_names.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/marker.py` & `tensorpc-0.10.2/tensorpc/marker.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/protos/arraybuf_pb2.py` & `tensorpc-0.10.2/tensorpc/protos/arraybuf_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/protos/arraybuf_pb2.pyi` & `tensorpc-0.10.2/tensorpc/protos/arraybuf_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/protos/remote_object_pb2.py` & `tensorpc-0.10.2/tensorpc/protos/remote_object_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/protos/remote_object_pb2_grpc.py` & `tensorpc-0.10.2/tensorpc/protos/remote_object_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/protos/rpc_message_pb2.py` & `tensorpc-0.10.2/tensorpc/protos/rpc_message_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/protos/rpc_message_pb2.pyi` & `tensorpc-0.10.2/tensorpc/protos/rpc_message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/protos/wsdef_pb2.py` & `tensorpc-0.10.2/tensorpc/protos/wsdef_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/protos/wsdef_pb2.pyi` & `tensorpc-0.10.2/tensorpc/protos/wsdef_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/protos_legacy/arraybuf_pb2.py` & `tensorpc-0.10.2/tensorpc/protos_legacy/arraybuf_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/protos_legacy/arraybuf_pb2.pyi` & `tensorpc-0.10.2/tensorpc/protos_legacy/arraybuf_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/protos_legacy/remote_object_pb2.py` & `tensorpc-0.10.2/tensorpc/protos_legacy/remote_object_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/protos_legacy/remote_object_pb2_grpc.py` & `tensorpc-0.10.2/tensorpc/protos_legacy/remote_object_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/protos_legacy/rpc_message_pb2.py` & `tensorpc-0.10.2/tensorpc/protos_legacy/rpc_message_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/protos_legacy/rpc_message_pb2.pyi` & `tensorpc-0.10.2/tensorpc/protos_legacy/rpc_message_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/protos_legacy/wsdef_pb2.py` & `tensorpc-0.10.2/tensorpc/protos_legacy/wsdef_pb2.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/protos_legacy/wsdef_pb2.pyi` & `tensorpc-0.10.2/tensorpc/protos_legacy/wsdef_pb2.pyi`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/serve/__init__.py` & `tensorpc-0.10.2/tensorpc/serve/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/serve/__main__.py` & `tensorpc-0.10.2/tensorpc/serve/__main__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/serve/flowapp_script/__main__.py` & `tensorpc-0.10.2/tensorpc/serve/flowapp_script/__main__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/serve_sync/__main__.py` & `tensorpc-0.10.2/tensorpc/serve_sync/__main__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/services/__init__.py` & `tensorpc-0.10.2/tensorpc/services/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/services/collection.py` & `tensorpc-0.10.2/tensorpc/services/collection.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/services/flow/__init__.py` & `tensorpc-0.10.2/tensorpc/services/flow/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/services/flow/core.py` & `tensorpc-0.10.2/tensorpc/services/flow/core.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/services/for_test.py` & `tensorpc-0.10.2/tensorpc/services/for_test.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/services/vis.py` & `tensorpc-0.10.2/tensorpc/services/vis.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/tools.py` & `tensorpc-0.10.2/tensorpc/tools.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/utils/__init__.py` & `tensorpc-0.10.2/tensorpc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/utils/df_logging.py` & `tensorpc-0.10.2/tensorpc/utils/df_logging.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/utils/gpuusage.py` & `tensorpc-0.10.2/tensorpc/utils/gpuusage.py`

 * *Files 6% similar despite different names*

```diff
@@ -28,25 +28,25 @@
         "temperature.gpu",
         "memory.used",
         "memory.total",
     ]
     try:
         output = subprocess.check_output(
             ["nvidia-smi", f"--query-gpu={','.join(querys)}", "--format=csv"])
+        output_str = output.decode("utf-8")
+        output_str_file = io.StringIO(output_str)
+        csv_data = csv.reader(output_str_file, delimiter=',', quotechar=',')
+        rows = list(csv_data)[1:]
+        rows = [[r.strip() for r in row] for row in rows]
+        for r in rows:
+            query = dict(zip(querys, r))
+            gpuusage = int(query["utilization.gpu"].split(" ")[0])
+            memusage = int(query["utilization.memory"].split(" ")[0])
+            memused = int(query["memory.used"].split(" ")[0])
+            memtotal = int(query["memory.total"].split(" ")[0])
+            temp = int(query["temperature.gpu"])
+            gpumeasure = GPUMeasure(query["gpu_name"], gpuusage, memusage,
+                                    temp, memused, memtotal)
+            gpumeasures.append(gpumeasure)
     except:
-        return gpumeasures
-    output_str = output.decode("utf-8")
-    output_str_file = io.StringIO(output_str)
-    csv_data = csv.reader(output_str_file, delimiter=',', quotechar=',')
-    rows = list(csv_data)[1:]
-    rows = [[r.strip() for r in row] for row in rows]
-    for r in rows:
-        query = dict(zip(querys, r))
-        gpuusage = int(query["utilization.gpu"].split(" ")[0])
-        memusage = int(query["utilization.memory"].split(" ")[0])
-        memused = int(query["memory.used"].split(" ")[0])
-        memtotal = int(query["memory.total"].split(" ")[0])
-        temp = int(query["temperature.gpu"])
-        gpumeasure = GPUMeasure(query["gpu_name"], gpuusage, memusage,
-                                temp, memused, memtotal)
-        gpumeasures.append(gpumeasure)
+        return []
     return gpumeasures
```

### Comparing `tensorpc-0.10.1/tensorpc/utils/registry.py` & `tensorpc-0.10.2/tensorpc/utils/registry.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/utils/reload.py` & `tensorpc-0.10.2/tensorpc/utils/reload.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/utils/subproc.py` & `tensorpc-0.10.2/tensorpc/utils/subproc.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/utils/uniquename.py` & `tensorpc-0.10.2/tensorpc/utils/uniquename.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc/utils/wait_tools.py` & `tensorpc-0.10.2/tensorpc/utils/wait_tools.py`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/tensorpc.egg-info/PKG-INFO` & `tensorpc-0.10.2/tensorpc.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tensorpc
-Version: 0.10.1
+Version: 0.10.2
 Summary: Backend for devflow.
 Home-page: https://github.com/FindDefinition/tensorpc
 Author: Yan Yan
 Author-email: yanyan.sub@outlook.com
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
```

### Comparing `tensorpc-0.10.1/tensorpc.egg-info/SOURCES.txt` & `tensorpc-0.10.2/tensorpc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `tensorpc-0.10.1/test/test_tmux_scheduler.py` & `tensorpc-0.10.2/test/test_tmux_scheduler.py`

 * *Files identical despite different names*

