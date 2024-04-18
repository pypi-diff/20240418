# Comparing `tmp/aerleon-1.7.0.tar.gz` & `tmp/aerleon-1.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aerleon-1.7.0.tar", max compression
+gzip compressed data, was "aerleon-1.9.0.tar", max compression
```

## Comparing `aerleon-1.7.0.tar` & `aerleon-1.9.0.tar`

### file list

```diff
@@ -1,68 +1,70 @@
--rw-r--r--   0        0        0    11358 2023-08-17 04:48:56.610003 aerleon-1.7.0/LICENSE
--rw-r--r--   0        0        0     6934 2023-08-17 04:48:56.610003 aerleon-1.7.0/README.md
--rw-r--r--   0        0        0       15 2023-08-17 04:48:56.610003 aerleon-1.7.0/aerleon/__init__.py
--rw-r--r--   0        0        0      167 2023-08-17 04:48:56.610003 aerleon-1.7.0/aerleon/__main__.py
--rw-r--r--   0        0        0     4399 2023-08-17 04:48:56.610003 aerleon-1.7.0/aerleon/aclcheck_cmdline.py
--rw-r--r--   0        0        0    17930 2023-08-17 04:48:56.610003 aerleon-1.7.0/aerleon/aclgen.py
--rw-r--r--   0        0        0    13124 2023-08-17 04:48:56.610003 aerleon-1.7.0/aerleon/api.py
--rw-r--r--   0        0        0    11358 2023-08-17 04:48:56.610003 aerleon-1.7.0/aerleon/lib/COPYING
--rw-r--r--   0        0        0       29 2023-08-17 04:48:56.610003 aerleon-1.7.0/aerleon/lib/__init__.py
--rwxr-xr-x   0        0        0    11008 2023-08-17 04:48:56.610003 aerleon-1.7.0/aerleon/lib/aclcheck.py
--rw-r--r--   0        0        0    24716 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/aclgenerator.py
--rw-r--r--   0        0        0     7802 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/addressbook.py
--rw-r--r--   0        0        0     2792 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/arista.py
--rw-r--r--   0        0        0    36487 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/arista_tp.py
--rw-r--r--   0        0        0    10035 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/aruba.py
--rw-r--r--   0        0        0     1116 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/brocade.py
--rw-r--r--   0        0        0    40084 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/cisco.py
--rw-r--r--   0        0        0    14390 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/ciscoasa.py
--rw-r--r--   0        0        0     2754 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/cisconx.py
--rw-r--r--   0        0        0     2428 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/ciscoxr.py
--rw-r--r--   0        0        0     9968 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/cloudarmor.py
--rw-r--r--   0        0        0     7737 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/demo.py
--rw-r--r--   0        0        0      691 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/fqdn.py
--rw-r--r--   0        0        0    24978 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/gce.py
--rw-r--r--   0        0        0     4759 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/gcp.py
--rw-r--r--   0        0        0    24295 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/gcp_hf.py
--rw-r--r--   0        0        0     9076 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/ipset.py
--rw-r--r--   0        0        0    38752 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/iptables.py
--rw-r--r--   0        0        0    45434 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/juniper.py
--rw-r--r--   0        0        0     5090 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/juniperevo.py
--rw-r--r--   0        0        0    32101 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/junipermsmpc.py
--rw-r--r--   0        0        0    37939 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/junipersrx.py
--rw-r--r--   0        0        0    14344 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/k8s.py
--rw-r--r--   0        0        0    17897 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/nacaddr.py
--rw-r--r--   0        0        0    39850 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/naming.py
--rw-r--r--   0        0        0    33371 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/nftables.py
--rw-r--r--   0        0        0     8158 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/nokiasrl.py
--rw-r--r--   0        0        0    12419 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/nsxt.py
--rw-r--r--   0        0        0    24865 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/nsxv.py
--rw-r--r--   0        0        0    12537 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/openconfig.py
--rw-r--r--   0        0        0    23397 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/packetfilter.py
--rw-r--r--   0        0        0    48254 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/paloaltofw.py
--rw-r--r--   0        0        0    17225 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/pcap.py
--rw-r--r--   0        0        0     3411 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/plugin.py
--rw-r--r--   0        0        0    13514 2023-08-17 04:48:56.614003 aerleon-1.7.0/aerleon/lib/plugin_supervisor.py
--rw-r--r--   0        0        0    97865 2023-08-17 04:48:56.618003 aerleon-1.7.0/aerleon/lib/policy.py
--rw-r--r--   0        0        0    39619 2023-08-17 04:48:56.618003 aerleon-1.7.0/aerleon/lib/policy_builder.py
--rw-r--r--   0        0        0    21391 2023-08-17 04:48:56.618003 aerleon-1.7.0/aerleon/lib/policy_simple.py
--rw-r--r--   0        0        0     9162 2023-08-17 04:48:56.618003 aerleon-1.7.0/aerleon/lib/policyreader.py
--rw-r--r--   0        0        0     4948 2023-08-17 04:48:56.618003 aerleon-1.7.0/aerleon/lib/port.py
--rw-r--r--   0        0        0    14617 2023-08-17 04:48:56.618003 aerleon-1.7.0/aerleon/lib/recognizers.py
--rw-r--r--   0        0        0      697 2023-08-17 04:48:56.618003 aerleon-1.7.0/aerleon/lib/sonic.py
--rw-r--r--   0        0        0     1322 2023-08-17 04:48:56.618003 aerleon-1.7.0/aerleon/lib/speedway.py
--rw-r--r--   0        0        0     2405 2023-08-17 04:48:56.618003 aerleon-1.7.0/aerleon/lib/srxlo.py
--rw-r--r--   0        0        0     9069 2023-08-17 04:48:56.618003 aerleon-1.7.0/aerleon/lib/summarizer.py
--rw-r--r--   0        0        0    14092 2023-08-17 04:48:56.618003 aerleon-1.7.0/aerleon/lib/windows.py
--rw-r--r--   0        0        0     6118 2023-08-17 04:48:56.618003 aerleon-1.7.0/aerleon/lib/windows_advfirewall.py
--rw-r--r--   0        0        0     9096 2023-08-17 04:48:56.618003 aerleon-1.7.0/aerleon/lib/windows_ipsec.py
--rw-r--r--   0        0        0    16148 2023-08-17 04:48:56.618003 aerleon-1.7.0/aerleon/lib/yaml.py
--rw-r--r--   0        0        0     1140 2023-08-17 04:48:56.618003 aerleon-1.7.0/aerleon/lib/yaml_loader.py
--rw-r--r--   0        0        0        0 2023-08-17 04:48:56.618003 aerleon-1.7.0/aerleon/utils/__init__.py
--rw-r--r--   0        0        0     3240 2023-08-17 04:48:56.618003 aerleon-1.7.0/aerleon/utils/config.py
--rw-r--r--   0        0        0     3592 2023-08-17 04:48:56.618003 aerleon-1.7.0/aerleon/utils/iputils.py
--rw-r--r--   0        0        0     2712 2023-08-17 04:48:56.622003 aerleon-1.7.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-08-17 04:48:56.666003 aerleon-1.7.0/tools/__init__.py
--rw-r--r--   0        0        0    16269 2023-08-17 04:48:56.666003 aerleon-1.7.0/tools/cgrep.py
--rw-r--r--   0        0        0     1794 2023-08-17 04:48:56.666003 aerleon-1.7.0/tools/iputilstools.py
--rw-r--r--   0        0        0     8090 1970-01-01 00:00:00.000000 aerleon-1.7.0/PKG-INFO
+-rw-r--r--   0        0        0      337 2024-04-18 07:41:26.492712 aerleon-1.9.0/AUTHORS
+-rw-r--r--   0        0        0    11358 2024-04-18 07:41:26.492712 aerleon-1.9.0/LICENSE
+-rw-r--r--   0        0        0     7011 2024-04-18 07:41:26.496712 aerleon-1.9.0/README.md
+-rw-r--r--   0        0        0       15 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/__init__.py
+-rw-r--r--   0        0        0      167 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/__main__.py
+-rw-r--r--   0        0        0     4399 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/aclcheck_cmdline.py
+-rw-r--r--   0        0        0    17930 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/aclgen.py
+-rw-r--r--   0        0        0    13123 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/api.py
+-rw-r--r--   0        0        0    11358 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/COPYING
+-rw-r--r--   0        0        0       29 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/__init__.py
+-rwxr-xr-x   0        0        0    11008 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/aclcheck.py
+-rw-r--r--   0        0        0    24716 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/aclgenerator.py
+-rw-r--r--   0        0        0     7802 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/addressbook.py
+-rw-r--r--   0        0        0     2792 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/arista.py
+-rw-r--r--   0        0        0    36487 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/arista_tp.py
+-rw-r--r--   0        0        0    10035 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/aruba.py
+-rw-r--r--   0        0        0     1116 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/brocade.py
+-rw-r--r--   0        0        0    40080 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/cisco.py
+-rw-r--r--   0        0        0    14387 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/ciscoasa.py
+-rw-r--r--   0        0        0     2754 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/cisconx.py
+-rw-r--r--   0        0        0     2428 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/ciscoxr.py
+-rw-r--r--   0        0        0     9967 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/cloudarmor.py
+-rw-r--r--   0        0        0     7735 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/demo.py
+-rw-r--r--   0        0        0      691 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/fqdn.py
+-rw-r--r--   0        0        0    24978 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/gce.py
+-rw-r--r--   0        0        0     4759 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/gcp.py
+-rw-r--r--   0        0        0    24294 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/gcp_hf.py
+-rw-r--r--   0        0        0     9074 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/ipset.py
+-rw-r--r--   0        0        0    39248 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/iptables.py
+-rw-r--r--   0        0        0    45430 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/juniper.py
+-rw-r--r--   0        0        0     5090 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/juniperevo.py
+-rw-r--r--   0        0        0    32101 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/junipermsmpc.py
+-rw-r--r--   0        0        0    37936 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/junipersrx.py
+-rw-r--r--   0        0        0    14343 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/k8s.py
+-rw-r--r--   0        0        0    17897 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/nacaddr.py
+-rw-r--r--   0        0        0    39849 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/naming.py
+-rw-r--r--   0        0        0    33371 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/nftables.py
+-rw-r--r--   0        0        0     9031 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/nokiasrl.py
+-rw-r--r--   0        0        0    12417 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/nsxt.py
+-rw-r--r--   0        0        0    24862 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/nsxv.py
+-rw-r--r--   0        0        0    12745 2024-04-18 07:41:26.496712 aerleon-1.9.0/aerleon/lib/openconfig.py
+-rw-r--r--   0        0        0    23395 2024-04-18 07:41:26.500712 aerleon-1.9.0/aerleon/lib/packetfilter.py
+-rw-r--r--   0        0        0    48251 2024-04-18 07:41:26.500712 aerleon-1.9.0/aerleon/lib/paloaltofw.py
+-rw-r--r--   0        0        0    17224 2024-04-18 07:41:26.500712 aerleon-1.9.0/aerleon/lib/pcap.py
+-rw-r--r--   0        0        0     3411 2024-04-18 07:41:26.500712 aerleon-1.9.0/aerleon/lib/plugin.py
+-rw-r--r--   0        0        0    13513 2024-04-18 07:41:26.500712 aerleon-1.9.0/aerleon/lib/plugin_supervisor.py
+-rw-r--r--   0        0        0    97864 2024-04-18 07:41:26.500712 aerleon-1.9.0/aerleon/lib/policy.py
+-rw-r--r--   0        0        0    39619 2024-04-18 07:41:26.500712 aerleon-1.9.0/aerleon/lib/policy_builder.py
+-rw-r--r--   0        0        0    21391 2024-04-18 07:41:26.500712 aerleon-1.9.0/aerleon/lib/policy_simple.py
+-rw-r--r--   0        0        0     9162 2024-04-18 07:41:26.500712 aerleon-1.9.0/aerleon/lib/policyreader.py
+-rw-r--r--   0        0        0     4948 2024-04-18 07:41:26.500712 aerleon-1.9.0/aerleon/lib/port.py
+-rw-r--r--   0        0        0    14617 2024-04-18 07:41:26.500712 aerleon-1.9.0/aerleon/lib/recognizers.py
+-rw-r--r--   0        0        0      697 2024-04-18 07:41:26.500712 aerleon-1.9.0/aerleon/lib/sonic.py
+-rw-r--r--   0        0        0     1322 2024-04-18 07:41:26.500712 aerleon-1.9.0/aerleon/lib/speedway.py
+-rw-r--r--   0        0        0     2405 2024-04-18 07:41:26.500712 aerleon-1.9.0/aerleon/lib/srxlo.py
+-rw-r--r--   0        0        0     9069 2024-04-18 07:41:26.500712 aerleon-1.9.0/aerleon/lib/summarizer.py
+-rw-r--r--   0        0        0    14092 2024-04-18 07:41:26.500712 aerleon-1.9.0/aerleon/lib/windows.py
+-rw-r--r--   0        0        0     6116 2024-04-18 07:41:26.500712 aerleon-1.9.0/aerleon/lib/windows_advfirewall.py
+-rw-r--r--   0        0        0     9096 2024-04-18 07:41:26.500712 aerleon-1.9.0/aerleon/lib/windows_ipsec.py
+-rw-r--r--   0        0        0    16147 2024-04-18 07:41:26.500712 aerleon-1.9.0/aerleon/lib/yaml.py
+-rw-r--r--   0        0        0     1140 2024-04-18 07:41:26.500712 aerleon-1.9.0/aerleon/lib/yaml_loader.py
+-rw-r--r--   0        0        0        0 2024-04-18 07:41:26.500712 aerleon-1.9.0/aerleon/py.typed
+-rw-r--r--   0        0        0        0 2024-04-18 07:41:26.500712 aerleon-1.9.0/aerleon/utils/__init__.py
+-rw-r--r--   0        0        0     3240 2024-04-18 07:41:26.500712 aerleon-1.9.0/aerleon/utils/config.py
+-rw-r--r--   0        0        0     3592 2024-04-18 07:41:26.500712 aerleon-1.9.0/aerleon/utils/iputils.py
+-rw-r--r--   0        0        0     2667 2024-04-18 07:41:26.504712 aerleon-1.9.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-18 07:41:26.552712 aerleon-1.9.0/tools/__init__.py
+-rw-r--r--   0        0        0    16269 2024-04-18 07:41:26.552712 aerleon-1.9.0/tools/cgrep.py
+-rw-r--r--   0        0        0     1794 2024-04-18 07:41:26.552712 aerleon-1.9.0/tools/iputilstools.py
+-rw-r--r--   0        0        0     8168 1970-01-01 00:00:00.000000 aerleon-1.9.0/PKG-INFO
```

### Comparing `aerleon-1.7.0/LICENSE` & `aerleon-1.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/README.md` & `aerleon-1.9.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -14,20 +14,26 @@
 - Typed Python APIs for ACL generation and aclcheck queries.
 - A [SLSA-compatible verifiable release process](https://aerleon.readthedocs.io/en/latest/install/#verifying-installation).
 - A detailed regression test suite.
 - Many bug fixes and performance enhancements.
 
 ## Install
 
-Aerleon requires Python 3.7 or higher.
+Aerleon requires Python 3.8 or higher.
 
 ```bash
 pip install aerleon
 ```
 
+To install via [`brew`](https://brew.sh):
+
+```bash
+brew install aerleon
+```
+
 ## Overview
 
 Aerleon provides a command line tool and a Python API that will generate configs for multiple firewall platforms from a single platform-agnostic configuration language. It can generate configs for Cisco, Juniper, Palo Alto Networks and [many other firewall vendors](https://aerleon.readthedocs.io/en/latest/#core-supported-generators).
 
 A [getting started guide](https://aerleon.readthedocs.io/en/latest/getting_started/) walking through the basics of using Aerleon is available on the docs website.
 
 ## Documentation
```

### Comparing `aerleon-1.7.0/aerleon/aclcheck_cmdline.py` & `aerleon-1.9.0/aerleon/aclcheck_cmdline.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/aclgen.py` & `aerleon-1.9.0/aerleon/aclgen.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/api.py` & `aerleon-1.9.0/aerleon/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -276,15 +276,14 @@
     context: multiprocessing.context.BaseContext,
     output_directory: pathlib.Path = None,
     optimize: bool = False,
     shade_check: bool = False,
     exp_info: int = 2,
     max_renderers: int = 1,
 ) -> "dict[str, str]":
-
     # thead-safe list for storing files to write
     manager: multiprocessing.managers.SyncManager = context.Manager()
     write_files: WriteList = manager.list()
     errors: list = manager.list()
     generated_configs: dict = manager.dict()
 
     if max_renderers == 1:
```

### Comparing `aerleon-1.7.0/aerleon/lib/COPYING` & `aerleon-1.9.0/aerleon/lib/COPYING`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/aclcheck.py` & `aerleon-1.9.0/aerleon/lib/aclcheck.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/aclgenerator.py` & `aerleon-1.9.0/aerleon/lib/aclgenerator.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/addressbook.py` & `aerleon-1.9.0/aerleon/lib/addressbook.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/arista.py` & `aerleon-1.9.0/aerleon/lib/arista.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/arista_tp.py` & `aerleon-1.9.0/aerleon/lib/arista_tp.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/aruba.py` & `aerleon-1.9.0/aerleon/lib/aruba.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/brocade.py` & `aerleon-1.9.0/aerleon/lib/brocade.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/cisco.py` & `aerleon-1.9.0/aerleon/lib/cisco.py`

 * *Files 0% similar despite different names*

```diff
@@ -208,15 +208,14 @@
         # for using cisco, which has decided to implement its own meta language.
 
         # Create network object-groups
         for zone, name, ips, _ in self.addressbook.Walk():
             for version in (4, 6):
                 vips = [i for i in ips if i.version == version]
                 if vips:
-
                     ret_str.append(f'object-group network ipv{version} {name}')
                     for ip in vips:
                         ret_str.append(f' {ip.network_address}/{ip.prefixlen}')
                     ret_str.append('exit\n')
 
             # Create port object-groups
         for term in self.terms:
@@ -491,15 +490,14 @@
             elif self.platform == 'ciscoxr':
                 protocol = ['ipv4']
             else:
                 protocol = ['ip']
         elif self.term.protocol == ['hopopt'] or self.term.protocol == self.PROTO_MAP['hopopt']:
             protocol = ['hbh']
         elif self.proto_int:
-
             protocol = [
                 proto
                 if proto in self.ALLOWED_PROTO_STRINGS or proto.isnumeric()
                 else self.PROTO_MAP.get(proto)
                 for proto in self.term.protocol
             ]
         else:
@@ -1057,15 +1055,15 @@
 
     def __str__(self) -> str:
         target_header = []
         target = []
         # add the p4 tags
         target.extend(aclgenerator.AddRepositoryTags('! '))
 
-        for (header, filter_name, filter_list, terms, obj_target) in self.cisco_policies:
+        for header, filter_name, filter_list, terms, obj_target in self.cisco_policies:
             for filter_type in filter_list:
                 target.extend(self._AppendTargetByFilterType(filter_name, filter_type))
                 if filter_type == 'object-group':
                     obj_target.AddName(filter_name)
 
                 # Add the Perforce Id/Date tags, these must come after
                 # remove/re-create of the filter, otherwise config mode doesn't
```

### Comparing `aerleon-1.7.0/aerleon/lib/ciscoasa.py` & `aerleon-1.9.0/aerleon/lib/ciscoasa.py`

 * *Files 1% similar despite different names*

```diff
@@ -350,16 +350,15 @@
                 new_terms.append(str(Term(term, filter_name, enable_dsmo=enable_dsmo)))
 
             self.ciscoasa_policies.append((header, filter_name, new_terms))
 
     def __str__(self) -> str:
         target = []
 
-        for (header, filter_name, terms) in self.ciscoasa_policies:
-
+        for header, filter_name, terms in self.ciscoasa_policies:
             target.append('clear configure access-list %s' % filter_name)
 
             # add the p4 tags
             target.extend(aclgenerator.AddRepositoryTags('access-list %s remark ' % filter_name))
 
             # add a header comment if one exists
             for comment in header.comment:
```

### Comparing `aerleon-1.7.0/aerleon/lib/cisconx.py` & `aerleon-1.9.0/aerleon/lib/cisconx.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/ciscoxr.py` & `aerleon-1.9.0/aerleon/lib/ciscoxr.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/cloudarmor.py` & `aerleon-1.9.0/aerleon/lib/cloudarmor.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from aerleon.lib import aclgenerator, policy
 
 if sys.version_info < (3, 8):
     from typing_extensions import TypedDict
 else:
     from typing import TypedDict
 
+
 # Generic error class
 class Error(aclgenerator.Error):
     """Generic error class."""
 
 
 class ExceededMaxTermsError(Error):
     """Raised when number of terms in a policy exceed _MAX_RULES_PER_POLICY."""
@@ -239,29 +240,27 @@
                     raise UnsupportedFilterTypeError(
                         "'%s' is not a valid filter type" % filter_type
                     )
 
             counter = 1
 
             for term in terms:
-
                 json_rule_list = Term(
                     term, address_family=filter_type, verbose=verbose
                 ).ConvertToDict(priority_index=counter)
                 # count number of rules generated after split (if any)
                 split_rule_count = len(json_rule_list)
 
                 self.cloudarmor_policies.extend(json_rule_list)
 
                 counter = counter + split_rule_count
 
                 total_rule_count = len(self.cloudarmor_policies)
 
                 if total_rule_count > self._RULECOUNT_WARN_THRESHOLD:
-
                     if total_rule_count > self._MAX_RULES_PER_POLICY:
                         raise ExceededMaxTermsError(
                             'Exceeded maximum number of rules in '
                             ' a single policy | MAX = %d' % self._MAX_RULES_PER_POLICY
                         )
                     else:
                         logging.warning(
```

### Comparing `aerleon-1.7.0/aerleon/lib/demo.py` & `aerleon-1.9.0/aerleon/lib/demo.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,15 @@
                 new_terms.append(Term(term, filter_type))
             self.demo_policies.append(
                 (header, filter_name, filter_type, interface_specific, new_terms)
             )
 
     def __str__(self):
         target = []
-        for (header, filter_name, filter_type, interface_specific, terms) in self.demo_policies:
+        for header, filter_name, filter_type, interface_specific, terms in self.demo_policies:
             target.append('Header {')
             target.append(' ' * 4 + 'Name: %s {' % filter_name)
             target.append(' ' * 8 + 'Type: %s ' % filter_type)
             for comment in header.comment:
                 for line in comment.split('\n'):
                     target.append(' ' * 8 + 'Comment: %s' % line)
             target.append(' ' * 8 + 'Family type: %s' % interface_specific)
```

### Comparing `aerleon-1.7.0/aerleon/lib/fqdn.py` & `aerleon-1.9.0/aerleon/lib/fqdn.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/gce.py` & `aerleon-1.9.0/aerleon/lib/gce.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/gcp.py` & `aerleon-1.9.0/aerleon/lib/gcp.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/gcp_hf.py` & `aerleon-1.9.0/aerleon/lib/gcp_hf.py`

 * *Files 0% similar despite different names*

```diff
@@ -425,15 +425,14 @@
         policy = {'rules': [], 'type': 'FIREWALL'}
         is_policy_modified = False
         counter = 1
         total_cost = 0
         policies_max_cost = self._DEFAULT_MAXIMUM_COST
         previous_max_cost = -1
         for header, terms in pol.filters:
-
             filter_options = header.FilterOptions(self._PLATFORM)
 
             is_policy_modified = True
 
             # Get term direction if set.
             direction = 'INGRESS'
             for i in self._GOOD_DIRECTION:
```

### Comparing `aerleon-1.7.0/aerleon/lib/ipset.py` & `aerleon-1.9.0/aerleon/lib/ipset.py`

 * *Files 0% similar despite different names*

```diff
@@ -196,15 +196,15 @@
 
     def __str__(self) -> str:
         # Actual rendering happens in __str__, so it has to be called
         # before we do set specific part.
         iptables_output = super().__str__()
         output = []
         output.append(self._MARKER_BEGIN)
-        for (_, _, _, _, terms) in self.iptables_policies:
+        for _, _, _, _, terms in self.iptables_policies:
             for term in terms:
                 output.extend(self._GenerateSetConfig(term))
         output.append(self._MARKER_END)
         output.append(iptables_output)
         return '\n'.join(output)
 
     def _GenerateSetConfig(self, term: Term) -> List[str]:
```

### Comparing `aerleon-1.7.0/aerleon/lib/iptables.py` & `aerleon-1.9.0/aerleon/lib/iptables.py`

 * *Files 2% similar despite different names*

```diff
@@ -72,14 +72,15 @@
         self,
         term: Term,
         filter_name: str,
         trackstate: bool,
         filter_action: Optional[str],
         af: str = 'inet',
         verbose: bool = True,
+        chained_terms: bool = True,
     ) -> None:
         """Setup a new term.
 
         Args:
           term: A policy.Term object to represent in iptables.
           filter_name: The name of the filter chan to attach the term to.
           trackstate: Specifies if conntrack should be used for new connections.
@@ -101,22 +102,25 @@
         self.trackstate = trackstate
         self.term = term  # term object
         self.filter = filter_name  # actual name of filter
         self.default_action = filter_action
         self.options = []
         self.af = af
         self.verbose = verbose
+        self.chained_terms = chained_terms
         if af == 'inet6':
             self._all_ips = nacaddr.IPv6('::/0')
             self._action_table['reject'] = '-j REJECT --reject-with ' 'icmp6-adm-prohibited'
         else:
             self._all_ips = nacaddr.IPv4('0.0.0.0/0')
             self._action_table['reject'] = '-j REJECT --reject-with ' 'icmp-host-prohibited'
-
-        self.term_name = '%s_%s' % (self.filter[:1], self.term.name)
+        if self.chained_terms:
+            self.term_name = '%s_%s' % (self.filter[:1], self.term.name)
+        else:
+            self.term_name = self.filter
 
     def __str__(self) -> str:
         ret_str = []
 
         # Don't render icmpv6 protocol terms under inet, or icmp under inet6
         if (self.af == 'inet6' and 'icmp' in self.term.protocol) or (
             self.af == 'inet' and 'icmpv6' in self.term.protocol
@@ -134,18 +138,18 @@
             for next_verbatim in self.term.verbatim:
                 if next_verbatim[0] == self._PLATFORM:
                     ret_str.append(str(next_verbatim[1]))
             return '\n'.join(ret_str)
 
         # Create a new term
         self._SetDefaultAction()
-        if self._TERM_FORMAT:
-            ret_str.append(self._TERM_FORMAT.substitute(term=self.term_name))
 
-        if self._PREJUMP_FORMAT:
+        if self.chained_terms and self._TERM_FORMAT:
+            ret_str.append(self._TERM_FORMAT.substitute(term=self.term_name))
+        if self.chained_terms and self._PREJUMP_FORMAT:
             ret_str.append(
                 self._PREJUMP_FORMAT.substitute(filter=self.filter, term=self.term_name)
             )
 
         if self.verbose:
             if self.term.owner:
                 self.term.comment.append('Owner: %s' % self.term.owner)
@@ -228,15 +232,14 @@
             source_port = self.term.source_port
         if self.term.destination_port:
             destination_port = self.term.destination_port
 
         # icmp-types
         icmp_types = ['']
         if self.term.icmp_type:
-
             icmp_types = self.NormalizeIcmpTypes(self.term.icmp_type, protocol, self.af)
 
         source_interface = ''
         if self.term.source_interface:
             source_interface = self.term.source_interface
 
         destination_interface = ''
@@ -361,15 +364,15 @@
                                         source_interface,
                                         destination_interface,
                                         log_hits,
                                         self._action_table.get(str(self.term.action[0])),
                                     )
                                 )
 
-        if self._POSTJUMP_FORMAT:
+        if self._POSTJUMP_FORMAT and self.chained_terms:
             ret_str.append(
                 self._POSTJUMP_FORMAT.substitute(filter=self.filter, term=self.term_name)
             )
 
         return '\n'.join(str(v) for v in ret_str if v)
 
     def _CalculateAddresses(
@@ -735,15 +738,15 @@
     _RENDER_SUFFIX = None
     _DEFAULTACTION_FORMAT = '-P %s %s'
     _DEFAULTACTION_FORMAT_CUSTOM_CHAIN = '-N %s'
     _DEFAULT_ACTION = 'DROP'
     _TERM = Term
     _TERM_MAX_LENGTH = 24
     _GOOD_FILTERS = ['INPUT', 'OUTPUT', 'FORWARD']
-    _GOOD_OPTIONS = ['nostate', 'abbreviateterms', 'truncateterms', 'noverbose']
+    _GOOD_OPTIONS = ['nostate', 'abbreviateterms', 'truncateterms', 'noverbose', 'nochainedterms']
 
     def __init__(self, pol: Policy, exp_info: int) -> None:
         self.iptables_policies = []
         super().__init__(pol, exp_info)
 
     def _BuildTokens(self) -> Tuple[Set[str], Dict[str, Set[str]]]:
         """Build supported tokens for platform.
@@ -801,14 +804,15 @@
             )
 
     def _TranslatePolicy(self, pol: Policy, exp_info: int) -> None:
         """Translate a policy from objects into strings."""
         default_action = None
         good_default_actions = ['ACCEPT', 'DROP']
         good_afs = ['inet', 'inet6']
+        chained_terms = True
         all_protocols_stateful = True
         self.verbose = True
 
         for header, terms in pol.filters:
             filter_type = None
             self.filter_options = header.FilterOptions(self._PLATFORM)[1:]
             filter_name = header.FilterName(self._PLATFORM)
@@ -829,14 +833,16 @@
                     )
 
             # disable stateful?
             if 'nostate' in self.filter_options:
                 all_protocols_stateful = False
             if 'noverbose' in self.filter_options:
                 self.verbose = False
+            if 'nochainedterms' in self.filter_options:
+                chained_terms = False
 
             # Check for matching af
             for address_family in good_afs:
                 if address_family in self.filter_options:
                     # should not specify more than one AF in options
                     if filter_type is not None:
                         raise UnsupportedFilterError(
@@ -888,14 +894,16 @@
                         'You have a duplicate term: %s' % term.name
                     )
                 term_names.add(term.name)
                 if not term.logging and term.log_limit:
                     raise LimitButNoLogError(
                         'Term %s: Cannoy use log-limit without logging' % term.name
                     )
+                if not chained_terms:
+                    term.name = filter_name
 
                 term = self.FixHighPorts(
                     term, af=filter_type, all_protocols_stateful=all_protocols_stateful
                 )
                 if not term:
                     continue
 
@@ -903,14 +911,15 @@
                     self._TERM(
                         term,
                         filter_name,
                         all_protocols_stateful,
                         default_action,
                         filter_type,
                         self.verbose,
+                        chained_terms,
                     )
                 )
 
             self.iptables_policies.append(
                 (header, filter_name, filter_type, default_action, new_terms)
             )
 
@@ -932,15 +941,15 @@
     def __str__(self) -> str:
         target = []
         pretty_platform = '%s%s' % (self._PLATFORM[0].upper(), self._PLATFORM[1:])
 
         if self._RENDER_PREFIX:
             target.append(self._RENDER_PREFIX)
 
-        for (header, filter_name, filter_type, default_action, terms) in self.iptables_policies:
+        for header, filter_name, filter_type, default_action, terms in self.iptables_policies:
             # Add comments for this filter
             target.append('# %s %s Policy' % (pretty_platform, header.FilterName(self._PLATFORM)))
 
             # reformat long text comments, if needed
             comments = aclgenerator.WrapWords(header.comment, 70)
             if comments and comments[0]:
                 for line in comments:
```

### Comparing `aerleon-1.7.0/aerleon/lib/juniper.py` & `aerleon-1.9.0/aerleon/lib/juniper.py`

 * *Files 1% similar despite different names*

```diff
@@ -844,25 +844,23 @@
         # length_eol is the width of the line; b/c of the addition of the space
         # and the /* characters, it needs to be a little less than the actual width
         # to keep from wrapping
         length_eol = 77 - indentation
 
         if isinstance(addr, (nacaddr.IPv4, nacaddr.IPv6, summarizer.DSMNet)):
             if addr.text:
-
                 if line_length == 0:
                     # line_length of 0 means that we don't want to truncate the comment.
                     line_length = len(addr.text)
 
                 # There should never be a /* or */, but be safe and ignore those
                 # comments
                 if addr.text.find('/*') >= 0 or addr.text.find('*/') >= 0:
                     logging.warning('Malformed comment [%s] ignoring', addr.text)
                 else:
-
                     text = addr.text[:line_length]
 
                     comment = ' /*'
                     while text:
                         # split the line
                         if len(text) > length_eol:
                             new_length_eol = text[:length_eol].rfind(' ')
@@ -1046,27 +1044,25 @@
 
             if filter_type == 'mixed':
                 filter_types_to_process = ['inet', 'inet6']
             else:
                 filter_types_to_process = [filter_type]
 
             for term_filter_type in filter_types_to_process:
-
                 filter_name_suffix = ''
                 # If mixed filter_type, will append 4 or 6 to the filter name
                 if len(filter_types_to_process) > 1:
                     if term_filter_type == 'inet':
                         filter_name_suffix = '4'
                     if term_filter_type == 'inet6':
                         filter_name_suffix = '6'
 
                 term_names = set()
                 new_terms = []
                 for term in terms:
-
                     # Ignore if the term is for a different AF
                     if (
                         term.restrict_address_family
                         and term.restrict_address_family != term_filter_type
                     ):
                         continue
```

### Comparing `aerleon-1.7.0/aerleon/lib/juniperevo.py` & `aerleon-1.9.0/aerleon/lib/juniperevo.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/junipermsmpc.py` & `aerleon-1.9.0/aerleon/lib/junipermsmpc.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/junipersrx.py` & `aerleon-1.9.0/aerleon/lib/junipersrx.py`

 * *Files 0% similar despite different names*

```diff
@@ -729,15 +729,14 @@
 
     def _GenerateAddressBook(self) -> IndentList:
         """Creates address book."""
         target = IndentList(self.INDENT)
 
         # create address books if address-book-type set to global
         if self._GLOBAL_ADDR_BOOK in self.addr_book_type:
-
             target.IndentAppend(1, 'replace: address-book {')
             target.IndentAppend(2, 'global {')
             global_addressbook = addressbook.Addressbook()
             for zone, _, ips, fqdns in self.addressbook.Walk():
                 global_addressbook.AddAddresses('global', ips)
                 global_addressbook.AddFQDNs('global', fqdns, suffix=FQDNSUFFIX)
             if 'global' in global_addressbook.GetZoneNames():
@@ -885,15 +884,15 @@
         # POLICIES
         target.IndentAppend(1, '/*')
         target.extend(aclgenerator.AddRepositoryTags(self.INDENT * 1))
         target.IndentAppend(1, '*/')
 
         target.IndentAppend(1, 'replace: policies {')
 
-        for (header, terms, filter_options) in self.srx_policies:
+        for header, terms, filter_options in self.srx_policies:
             if self._NOVERBOSE not in filter_options[4:]:
                 target.IndentAppend(2, '/*')
                 target.extend(
                     [
                         self.INDENT * 2 + line
                         for line in aclgenerator.WrapWords(
                             header.comment, self._MAX_HEADER_COMMENT_LENGTH
```

### Comparing `aerleon-1.7.0/aerleon/lib/k8s.py` & `aerleon-1.9.0/aerleon/lib/k8s.py`

 * *Files 1% similar despite different names*

```diff
@@ -279,15 +279,14 @@
                 base_port_selector = {'port': start, 'endPort': end}
 
             base_port_selectors.append(base_port_selector)
 
         # Use the ports info to make one selector per port pair per proto
         port_selectors = []
         for proto in self.term.protocol:
-
             # If the list of ports is null, we still need to specify proto
             if not base_port_selectors:
                 port_selectors.append({'protocol': proto.upper()})
                 continue
 
             for base_selector in base_port_selectors:
                 current_selector = copy.deepcopy(base_selector)
```

### Comparing `aerleon-1.7.0/aerleon/lib/nacaddr.py` & `aerleon-1.9.0/aerleon/lib/nacaddr.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/naming.py` & `aerleon-1.9.0/aerleon/lib/naming.py`

 * *Files 0% similar despite different names*

```diff
@@ -658,15 +658,14 @@
             '.net': DEF_TYPE_NETWORKS,
             '.svc': DEF_TYPE_SERVICES,
             '.yaml': 'yaml',
             '.yml': 'yaml',
         }
 
         for path in Path(definitions_directory).iterdir():
-
             def_type = file_def_type.get(path.suffix)
 
             if not def_type:
                 continue
 
             try:
                 with open(path, 'r') as file:
```

### Comparing `aerleon-1.7.0/aerleon/lib/nftables.py` & `aerleon-1.9.0/aerleon/lib/nftables.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/nokiasrl.py` & `aerleon-1.9.0/aerleon/lib/nokiasrl.py`

 * *Files 19% similar despite different names*

```diff
@@ -46,18 +46,35 @@
         "source-port": Port,
         "destination-port": Port,
     },
 )
 Action = TypedDict("Action", {"accept": None, "drop": None})
 ACLEntry = TypedDict(
     "ACLEntry",
-    {"sequence-id": int, "action": Action, "match": Match},
+    {
+        "sequence-id": int,
+        "action": Action,
+        "match": Match,
+        "description": str,
+        "_annotate_description": str,
+    },
+)
+Entries = TypedDict(
+    "Entries",
+    {
+        "entry": List[ACLEntry],
+        "description": str,
+        "name": str,
+        "type": str,
+        "_annotate": str,
+        "statistics-per-entry": bool,
+    },
 )
-Entries = TypedDict("Entries", {"entry": List[ACLEntry], "description": str})
-IPFilters = TypedDict("IPFilters", {"ipv4-filter": Entries, "ipv6-filter": Entries})
+IPFilters = TypedDict("IPFilters", {"acl-filter": Entries})
+
 
 # generic error class
 class Error(aclgenerator.Error):
     pass
 
 
 class TcpEstablishedWithNonTcpError(Error):
@@ -77,28 +94,32 @@
 
 
 class SRLTerm(openconfig.Term):
     """Creates the term for the SR Linux ACL."""
 
     ACTION_MAP = {'accept': 'accept', 'deny': 'drop', 'reject': 'drop'}
 
+    def SetName(self, name: str) -> None:
+        # Put name in description field
+        self.term_dict['description'] = name
+
     def SetAction(self) -> None:
         action = self.ACTION_MAP[self.term.action[0]]
         log = {}
         if self.term.logging:
             if action == 'drop':
                 log = {"log": True}
             else:
                 raise UnsupportedLogging(
                     f'logging can only be used with deny in term {self.term.name}'
                 )
         self.term_dict['action'] = {action: log}
 
     def SetComments(self, comments: List[str]) -> None:
-        self.term_dict['description'] = "_".join(comments)[:255]
+        self.term_dict['_annotate_description'] = "_".join(comments)[:255]
 
     def SetOptions(self, family: str) -> None:
         # Handle various options
         opts = [str(x) for x in self.term.option]
         self.term_dict['match'] = {}
         if ('fragments' in opts) or ('is-fragment' in opts):
             self.term_dict['match']['fragment'] = True
@@ -198,35 +219,46 @@
         return supported_tokens, supported_sub_tokens
 
     def _InitACLSet(self) -> None:
         """Initialize self.acl_sets with proper Typing"""
         self.acl_sets: List[IPFilters] = []
 
     def _TranslateTerms(
-        self, terms: List[Term], address_family: str, filter_name: str, hdr_comments: List[str]
+        self,
+        terms: List[Term],
+        address_family: str,
+        filter_name: str,
+        hdr_comments: List[str],
+        filter_options: List[str],
     ) -> None:
-        srl_acl_entries: List[ACLEntry] = []
+        srl_acl_entries: Dict[str, List[ACLEntry]] = {'inet': [], 'inet6': []}
+        afs = ['inet', 'inet6'] if address_family == 'mixed' else [address_family]
         for term in terms:
-            # Handle mixed for each indvidual term as inet and inet6.
-            # inet/inet6 are treated the same.
-            term_address_families = []
-            if address_family == 'mixed':
-                term_address_families = ['inet', 'inet6']
-            else:
-                term_address_families = [address_family]
-            for term_af in term_address_families:
+            for term_af in afs:
                 t = SRLTerm(term, term_af)
                 for rule in t.ConvertToDict():
                     self.total_rule_count += 1
-                    rule['sequence-id'] = (len(srl_acl_entries) + 1) * 5
-                    srl_acl_entries.append(rule)
+                    rule['sequence-id'] = (len(srl_acl_entries[term_af]) + 1) * 5
+                    srl_acl_entries[term_af].append(rule)
         desc = "_".join(hdr_comments)[:255] if hdr_comments else ""
-        ip_filter = {
-            'ipv4-filter'
-            if address_family == 'inet'
-            else 'ipv6-filter': {
-                'description': desc,
-                'entry': srl_acl_entries,
-                'name': filter_name,
-            }
-        }
-        self.acl_sets.append(ip_filter)
+
+        for af in srl_acl_entries.keys():
+            if srl_acl_entries[af]:
+                # r24.3 changed the syntax for filters. For r24.3 or higher use the option `r24.3`.
+                if 'r24.3' in filter_options:
+                    key = "acl-filter"
+                else:
+                    key = "ipv4-filter" if af == 'inet' else "ipv6-filter"
+
+                ip_filter = {
+                    key: {
+                        '_annotate': " ".join(aclgenerator.AddRepositoryTags()),
+                        'name': filter_name,
+                        'description': desc,
+                        'entry': srl_acl_entries[af],
+                    }
+                }
+                if 'stats' in filter_options:
+                    ip_filter[key]['statistics-per-entry'] = True
+                if 'r24.3' in filter_options:
+                    ip_filter[key]['type'] = "ipv4" if af == 'inet' else "ipv6"
+                self.acl_sets.append(ip_filter)
```

### Comparing `aerleon-1.7.0/aerleon/lib/nsxt.py` & `aerleon-1.9.0/aerleon/lib/nsxt.py`

 * *Files 0% similar despite different names*

```diff
@@ -368,15 +368,15 @@
         self._FILTER_OPTIONS_DICT['section_id'] = section_id
         self._FILTER_OPTIONS_DICT['applied_to'] = applied_to
 
     def __str__(self):
         """Render the output of the nsxt policy."""
         if len(self.nsxt_policies) > 1:
             raise NsxtUnsupportedManyPoliciesError('Only one policy can be rendered')
-        for (_, _, _, terms) in self.nsxt_policies:
+        for _, _, _, terms in self.nsxt_policies:
             rules = [json.loads(str(term)) for term in terms]
 
         section_name = self._FILTER_OPTIONS_DICT['section_name']
         section_id = self._FILTER_OPTIONS_DICT['section_id']
         applied_to = self._FILTER_OPTIONS_DICT['applied_to']
 
         policy = {
```

### Comparing `aerleon-1.7.0/aerleon/lib/nsxv.py` & `aerleon-1.9.0/aerleon/lib/nsxv.py`

 * *Files 0% similar despite different names*

```diff
@@ -278,15 +278,14 @@
         if self.term.logging:
             log = 'true'
 
         sources = ''
         if source_addr:
             sources = '<sources excluded="false">'
             for saddr in source_addr:
-
                 # inet4
                 if isinstance(saddr, nacaddr.IPv4):
                     if saddr.num_addresses > 1:
                         saddr = '%s%s%s' % (
                             _XML_TABLE.get('srcIpv4Start'),
                             saddr.with_prefixlen,
                             _XML_TABLE.get('srcIpv4End'),
@@ -645,15 +644,15 @@
 
         # add the p4 tags
         target.append('<!--')
         target.extend(aclgenerator.AddRepositoryTags('\n'))
         target.append('\n')
         target.append('-->')
 
-        for (_, _, _, terms) in self.nsxv_policies:
+        for _, _, _, terms in self.nsxv_policies:
             section_name = self._FILTER_OPTIONS_DICT['section_name']
             # check section id value
             section_id = self._FILTER_OPTIONS_DICT['section_id']
             if not section_id or section_id == 0:
                 logging.warning(
                     'WARNING: Section-id is 0. A new Section is created '
                     'for %s. If there is any existing section, it '
```

### Comparing `aerleon-1.7.0/aerleon/lib/openconfig.py` & `aerleon-1.9.0/aerleon/lib/openconfig.py`

 * *Files 1% similar despite different names*

```diff
@@ -138,14 +138,16 @@
         # Rules will hold all exploded acl-entry dictionaries.
         rules = []
 
         # Convert the integer to the proper openconfig schema name str, ipv4/ipv6.
         term_af = self.AF_MAP.get(self.inet_version)
         family = self.AF_RENAME[term_af]
 
+        self.SetName(self.term.name)
+
         # Action
         self.SetAction()
 
         # Ballot fatigue handling for 'any'.
         saddrs = self.term.GetAddressOfVersion('flattened_saddr', term_af)
         if not saddrs:
             saddrs = ['any']
@@ -211,14 +213,17 @@
 
                             # This is the business end of ace explosion.
                             # A dict is a reference type, so deepcopy is actually required.
                             rules.append(copy.deepcopy(self.term_dict))
 
         return rules
 
+    def SetName(self, name: str) -> None:
+        pass
+
     def SetAction(self) -> None:
         action = self.ACTION_MAP[self.term.action[0]]
         self.term_dict['actions'] = {}
         self.term_dict['actions']['config'] = {}
         self.term_dict['actions']['config']['forwarding-action'] = action
 
     def SetComments(self, comments: List[str]) -> None:
@@ -312,20 +317,27 @@
 
             # Get the address family if set.
             address_family = 'inet'
             for i in self._SUPPORTED_AF:
                 if i in filter_options:
                     address_family = i
                     filter_options.remove(i)
-            self._TranslateTerms(terms, address_family, filter_name, header.comment)
+            self._TranslateTerms(
+                terms, address_family, filter_name, header.comment, filter_options
+            )
 
         logging.info('Total rule count of policy %s is: %d', filter_name, self.total_rule_count)
 
     def _TranslateTerms(
-        self, terms: List[Term], address_family: str, filter_name: str, hdr_comments: List[str]
+        self,
+        terms: List[Term],
+        address_family: str,
+        filter_name: str,
+        hdr_comments: List[str],
+        filter_options: List[str],
     ) -> None:
         """
         Factor out the translation of terms, such that it can be overridden by subclasses
         """
         oc_acl_entries: List[ACLEntry] = []
 
         for term in terms:
```

### Comparing `aerleon-1.7.0/aerleon/lib/packetfilter.py` & `aerleon-1.9.0/aerleon/lib/packetfilter.py`

 * *Files 0% similar despite different names*

```diff
@@ -605,15 +605,15 @@
         # Create address table.
         for name in sorted(self.address_book):
             v4 = sorted([x for x in self.address_book[name] if x.version == 4])
             v6 = sorted([x for x in self.address_book[name] if x.version == 6])
             entries = ',\\\n'.join(str(x) for x in v4 + v6)
             target.append('table <%s> {%s}' % (name, entries))
         # pylint: disable=unused-variable
-        for (header, filter_name, filter_type, terms) in self.pf_policies:
+        for header, filter_name, filter_type, terms in self.pf_policies:
             # Add comments for this filter
             target.append('# %s %s Policy' % (pretty_platform, header.FilterName(self._PLATFORM)))
 
             # reformat long text comments, if needed
             comments = aclgenerator.WrapWords(header.comment, 70)
             if comments and comments[0]:
                 for line in comments:
```

### Comparing `aerleon-1.7.0/aerleon/lib/paloaltofw.py` & `aerleon-1.9.0/aerleon/lib/paloaltofw.py`

 * *Files 0% similar despite different names*

```diff
@@ -928,15 +928,15 @@
         rules = etree.SubElement(security, "rules")
         tag = etree.Element("tag")
 
         tag_num = 0
 
         # pytype: disable=key-error
         # pylint: disable=unused-variable
-        for (header, pa_rules, filter_options) in self.pafw_policies:
+        for header, pa_rules, filter_options in self.pafw_policies:
             tag_name = None
             if header.comment:
                 comment = " ".join(header.comment).strip()
                 if comment:
                     tag_num += 1
                     # max tag len 127, max zone len 31
                     tag_name = self._TAG_NAME_FORMAT.format(
@@ -1115,15 +1115,14 @@
                     member = etree.SubElement(static, "member")
                     member.text = f'{ip.parent_token}_{count}'
                     count += 1
 
         vsys_entry.append(etree.Comment(" Addresses "))
         addr = etree.SubElement(vsys_entry, "address")
         if not no_addr_obj:
-
             for _, token, ips, _ in self.addressbook.Walk(''):
                 count = 0
                 for ip in ips:
                     entry = etree.SubElement(addr, "entry", {"name": f'{token}_{count}'})
                     desc = etree.SubElement(entry, "description")
                     desc.text = f'{token}_{count}'
                     elem = etree.SubElement(entry, "ip-netmask")
```

### Comparing `aerleon-1.7.0/aerleon/lib/pcap.py` & `aerleon-1.9.0/aerleon/lib/pcap.py`

 * *Files 0% similar despite different names*

```diff
@@ -449,15 +449,14 @@
         for (
             unused_header,
             unused_filter_name,
             unused_filter_type,
             accept_terms,
             deny_terms,
         ) in self.pcap_policies:
-
             accept = []
             for term in accept_terms:
                 term_str = str(term)
                 if term_str:
                     accept.append(str(term))
             accept_clause = Term.JoinConditionals(accept, 'and')
```

### Comparing `aerleon-1.7.0/aerleon/lib/plugin.py` & `aerleon-1.9.0/aerleon/lib/plugin.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/plugin_supervisor.py` & `aerleon-1.9.0/aerleon/lib/plugin_supervisor.py`

 * *Files 1% similar despite different names*

```diff
@@ -200,15 +200,14 @@
         if not self.disable_discovery:
             loaded_plugins.extend(self._CollectEntrypointPlugins())
         if self.include_path:
             loaded_plugins.extend(self._CollectPluginsByPath())
 
         # Attempt to load, initialize, interrogate, and register generators from each plugin
         for plugin_name, loaded_plugin in loaded_plugins:
-
             # Initialize entrypoint class or function and request metadata
             try:
                 plugin_instance: plugin.BasePlugin = loaded_plugin()
                 metadata = plugin_instance.RequestMetadata(SYSTEM_METADATA)
                 if not isinstance(metadata, plugin.PluginMetadata) or any(
                     filter(
                         lambda c: not isinstance(c, plugin.PluginCapability), metadata.capabilities
```

### Comparing `aerleon-1.7.0/aerleon/lib/policy.py` & `aerleon-1.9.0/aerleon/lib/policy.py`

 * *Files 0% similar despite different names*

```diff
@@ -1392,15 +1392,14 @@
                 if icmptype not in self.ICMP_TYPE[4] and icmptype not in self.ICMP_TYPE[6]:
                     raise TermInvalidIcmpType(
                         'Term %s contains an invalid icmp-type:' '%s' % (self.name, icmptype)
                     )
 
         if self.ttl:
             if not _MIN_TTL <= self.ttl <= _MAX_TTL:
-
                 raise InvalidTermTTLValue(
                     'Term %s contains invalid TTL: %s' % (self.name, self.ttl)
                 )
         for proto in self.protocol:
             if proto.isnumeric():
                 if int(proto) < 0 or 255 < int(proto):
                     raise InvalidNumericProtoValue(
```

### Comparing `aerleon-1.7.0/aerleon/lib/policy_builder.py` & `aerleon-1.9.0/aerleon/lib/policy_builder.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/policy_simple.py` & `aerleon-1.9.0/aerleon/lib/policy_simple.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/policyreader.py` & `aerleon-1.9.0/aerleon/lib/policyreader.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/port.py` & `aerleon-1.9.0/aerleon/lib/port.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/recognizers.py` & `aerleon-1.9.0/aerleon/lib/recognizers.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/sonic.py` & `aerleon-1.9.0/aerleon/lib/sonic.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/speedway.py` & `aerleon-1.9.0/aerleon/lib/speedway.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/srxlo.py` & `aerleon-1.9.0/aerleon/lib/srxlo.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/summarizer.py` & `aerleon-1.9.0/aerleon/lib/summarizer.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/windows.py` & `aerleon-1.9.0/aerleon/lib/windows.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/windows_advfirewall.py` & `aerleon-1.9.0/aerleon/lib/windows_advfirewall.py`

 * *Files 1% similar despite different names*

```diff
@@ -153,15 +153,15 @@
 
     def _ComposePortString(self, ports: List[Tuple[int, int]]) -> str:
         """Convert the list of ports tuples into a multiport range string."""
         if not ports:
             return ''
 
         multiports = []
-        for (start, end) in ports:
+        for start, end in ports:
             if start == end:
                 multiports.append(str(start))
             else:
                 multiports.append('-'.join([str(start), str(end)]))
         return ','.join(multiports)
```

### Comparing `aerleon-1.7.0/aerleon/lib/windows_ipsec.py` & `aerleon-1.9.0/aerleon/lib/windows_ipsec.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/lib/yaml.py` & `aerleon-1.9.0/aerleon/lib/yaml.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,14 @@
         policy_dict=policy_dict,
     )
 
 
 def _preprocessYAMLPolicyInner(
     depth: int, debug_stack: list, filename: str, base_dir: str, policy_dict: Optional[PolicyDict]
 ) -> Optional[Dict[str, List[Dict[str, Union[Dict[str, Dict[str, str]], List[Dict[str, str]]]]]]]:
-
     # Empty files are ignored with a warning
     if policy_dict is None or not policy_dict:
         logging.warning(UserMessage("Ignoring empty policy file.", filename=filename))
         return
 
     # Malformed policy files should generate a PolicyTypeError (unless this is an include file)
     if 'filters' in policy_dict and isinstance(policy_dict['filters'], list):
```

### Comparing `aerleon-1.7.0/aerleon/lib/yaml_loader.py` & `aerleon-1.9.0/aerleon/lib/yaml_loader.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/utils/config.py` & `aerleon-1.9.0/aerleon/utils/config.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/aerleon/utils/iputils.py` & `aerleon-1.9.0/aerleon/utils/iputils.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/pyproject.toml` & `aerleon-1.9.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,37 @@
 [tool.poetry]
 name = "aerleon"
-version = "1.7.0"
+version = "1.9.0"
 description = "A firewall generation tool"
 authors = ["Rob Ankeny <ankenyr@gmail.com>", "Jason Benterou <jason.benterou@gmail.com>"]
 license = "Apache-2.0"
 readme = "README.md"
 homepage = "https://github.com/aerleon/aerleon"
 repository = "https://github.com/aerleon/aerleon"
 keywords = ["firewall", "networking", "security"]
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Topic :: Security",
     "Topic :: System :: Networking :: Firewalls"
 ]
 include = [
     "LICENSE",
     "README.md",
     "tools",
 ]
 packages = [{include = "aerleon"}, {include = "aerleon/lib"}, {include = "tools"}]
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "^3.8"
 PyYAML = "^6.0"
 ply = "^3.11"
 absl-py = "^1.2.0"
 typing_extensions = "^4.4.0"
 importlib-metadata = { version = "^4.2", markers = "python_version <= '3.10'" }
 
 [tool.poetry.dev-dependencies]
```

### Comparing `aerleon-1.7.0/tools/cgrep.py` & `aerleon-1.9.0/tools/cgrep.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/tools/iputilstools.py` & `aerleon-1.9.0/tools/iputilstools.py`

 * *Files identical despite different names*

### Comparing `aerleon-1.7.0/PKG-INFO` & `aerleon-1.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 Metadata-Version: 2.1
 Name: aerleon
-Version: 1.7.0
+Version: 1.9.0
 Summary: A firewall generation tool
 Home-page: https://github.com/aerleon/aerleon
 License: Apache-2.0
 Keywords: firewall,networking,security
 Author: Rob Ankeny
 Author-email: ankenyr@gmail.com
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.12
 Classifier: Topic :: Security
 Classifier: Topic :: System :: Networking :: Firewalls
 Requires-Dist: PyYAML (>=6.0,<7.0)
 Requires-Dist: absl-py (>=1.2.0,<2.0.0)
 Requires-Dist: importlib-metadata (>=4.2,<5.0) ; python_version <= "3.10"
 Requires-Dist: ply (>=3.11,<4.0)
 Requires-Dist: typing_extensions (>=4.4.0,<5.0.0)
@@ -43,20 +43,26 @@
 - Typed Python APIs for ACL generation and aclcheck queries.
 - A [SLSA-compatible verifiable release process](https://aerleon.readthedocs.io/en/latest/install/#verifying-installation).
 - A detailed regression test suite.
 - Many bug fixes and performance enhancements.
 
 ## Install
 
-Aerleon requires Python 3.7 or higher.
+Aerleon requires Python 3.8 or higher.
 
 ```bash
 pip install aerleon
 ```
 
+To install via [`brew`](https://brew.sh):
+
+```bash
+brew install aerleon
+```
+
 ## Overview
 
 Aerleon provides a command line tool and a Python API that will generate configs for multiple firewall platforms from a single platform-agnostic configuration language. It can generate configs for Cisco, Juniper, Palo Alto Networks and [many other firewall vendors](https://aerleon.readthedocs.io/en/latest/#core-supported-generators).
 
 A [getting started guide](https://aerleon.readthedocs.io/en/latest/getting_started/) walking through the basics of using Aerleon is available on the docs website.
 
 ## Documentation
```

