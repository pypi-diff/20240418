# Comparing `tmp/packstack-23.0.0.0rc1.tar.gz` & `tmp/packstack-24.0.0.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "packstack-23.0.0.0rc1.tar", last modified: Tue Oct 17 15:26:12 2023, max compression
+gzip compressed data, was "packstack-24.0.0.0rc1.tar", last modified: Thu Apr 18 12:00:14 2024, max compression
```

## Comparing `packstack-23.0.0.0rc1.tar` & `packstack-24.0.0.0rc1.tar`

### file list

```diff
@@ -1,371 +1,368 @@
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.825910 packstack-23.0.0.0rc1/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/.stestr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/.testr.conf
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     9469 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/.zuul.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5530 2023-10-17 15:26:12.000000 packstack-23.0.0.0rc1/AUTHORS
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    74611 2023-10-17 15:26:12.000000 packstack-23.0.0.0rc1/ChangeLog
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      650 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/Gemfile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/MANIFEST.in
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11345 2023-10-17 15:26:12.825910 packstack-23.0.0.0rc1/PKG-INFO
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3783 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/Puppetfile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8303 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/README.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      913 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/Rakefile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/bindep.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.777910 packstack-23.0.0.0rc1/docs/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5576 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/docs/Makefile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8548 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/docs/conf.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    54829 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/docs/packstack.rst
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.777910 packstack-23.0.0.0rc1/packstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.781911 packstack-23.0.0.0rc1/packstack/installer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/installer/LICENSE
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/installer/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3649 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/installer/basedefs.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.781911 packstack-23.0.0.0rc1/packstack/installer/core/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/installer/core/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1189 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/installer/core/arch.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15319 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/installer/core/drones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2170 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/installer/core/parameters.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3650 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/installer/core/sequences.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2167 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/installer/exceptions.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5765 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/installer/output_messages.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5264 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/installer/processors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40967 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/installer/run_setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5347 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/installer/setup_controller.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.781911 packstack-23.0.0.0rc1/packstack/installer/utils/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1517 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/installer/utils/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4379 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/installer/utils/datastructures.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1382 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/installer/utils/decorators.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4447 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/installer/utils/network.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5734 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/installer/utils/shell.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1694 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/installer/utils/shortcuts.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2439 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/installer/utils/strings.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11910 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/installer/validators.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.781911 packstack-23.0.0.0rc1/packstack/modules/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/modules/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3767 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/modules/common.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2816 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/modules/documentation.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6529 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/modules/ospluginutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4733 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/modules/puppet.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.785910 packstack-23.0.0.0rc1/packstack/plugins/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/plugins/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7546 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/plugins/amqp_002.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4082 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/plugins/aodh_810.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7677 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/plugins/ceilometer_800.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    28691 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/plugins/cinder_250.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7836 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/plugins/dashboard_500.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4612 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/plugins/glance_200.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3495 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/plugins/gnocchi_790.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6709 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/plugins/heat_650.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3805 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/plugins/ironic_275.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    26987 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/plugins/keystone_100.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4040 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/plugins/magnum_920.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    24727 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/plugins/manila_355.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4171 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/plugins/mariadb_003.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    40818 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/plugins/neutron_350.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    20087 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/plugins/nova_300.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2602 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/plugins/openstack_client_400.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2295 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/plugins/postscript_951.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    54002 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/plugins/prescript_000.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    17382 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/plugins/provision_700.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    11822 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/plugins/puppet_950.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3845 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/plugins/sahara_900.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11565 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/plugins/ssl_001.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11752 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/plugins/swift_600.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5575 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/plugins/trove_850.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.773910 packstack-23.0.0.0rc1/packstack/puppet/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.769910 packstack-23.0.0.0rc1/packstack/puppet/modules/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.785910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/Gemfile
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/Rakefile
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.769910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/lib/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.789910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/default_hypervisor.rb
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/home_dir.rb
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/mariadb.rb
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8175 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/netns.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/netns_support.rb
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/network.rb
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.769910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.769910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.789910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/functions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/functions/choose_my_ip.rb
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1277 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/functions/force_interface.rb
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      393 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/functions/force_ip.rb
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.793910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.793910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/amqp/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2219 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/amqp/enable_rabbitmq.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/amqp.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.793910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/aodh/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1556 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/aodh/rabbitmq.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1362 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/aodh.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      665 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/apache.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.793910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ceilometer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ceilometer/nova_disabled.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1457 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ceilometer/rabbitmq.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1340 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ceilometer.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2155 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/chrony.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.793910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.793910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3425 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/lvm.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8184 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/netapp.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/nfs.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      764 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/solidfire.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      408 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/vmdk.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backup.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1681 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/rabbitmq.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2251 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1132 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/firewall.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.793910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.793910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/backend/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/backend/file.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      736 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/backend/swift.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1376 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/ceilometer.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1472 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1764 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/gnocchi.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.793910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat/cfn.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2374 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat/rabbitmq.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2678 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/horizon.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.793910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ironic/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1639 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ironic/rabbitmq.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ironic.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.797911 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/aodh.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/ceilometer.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/cinder.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      488 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/glance.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/gnocchi.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      613 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/heat.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      491 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/ironic.pp
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      586 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/magnum.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/manila.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/neutron.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      461 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/nova.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/placement.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/sahara.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/swift.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/trove.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     6766 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.797911 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/magnum/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1313 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/magnum/rabbitmq.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1613 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/magnum.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.797911 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.801910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1661 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/generic.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/glusternative.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/glusternfs.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/netapp.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1218 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/network.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1470 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/rabbitmq.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      832 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.801910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3685 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb/services.pp
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    18244 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb/services_remote.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2436 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/memcached.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/netns.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.805910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1692 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/api.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1475 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/bridge.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/dhcp.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/l3.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1006 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/lb_agent.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/metadata.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/metering.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1715 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ml2.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/notifications.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2128 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovn_agent.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovn_metadata.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovn_northd.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2248 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovs_agent.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovs_bridge.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1717 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/rabbitmq.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/sriov.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/vpnaas.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.805910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3790 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/api.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.805910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/ceilometer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1731 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/ceilometer/rabbitmq.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/ceilometer.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/common.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.805910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      504 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute/ironic.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2819 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute/libvirt.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      463 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute/vmware.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4234 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/conductor.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/metadata.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/neutron.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/nfs.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.809910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/sched/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/sched/ironic.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/sched.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/vncproxy.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3093 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2963 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/openstackclient.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      835 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/placement.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/prereqs.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.809910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1995 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/bridge.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      596 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/glance.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7480 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/tempest.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3940 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/redis.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.809910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/sahara/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/sahara/ceilometer.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2099 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/sahara/rabbitmq.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      267 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/sahara.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.809910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/ceilometer.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/fs.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3447 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/proxy.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1171 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/ringbuilder.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1298 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/storage.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.809910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/trove/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1634 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/trove/rabbitmq.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1236 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/trove.pp
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.809910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/spec/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      381 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/spec/spec_helper.rb
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.773910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/spec/unit/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.773910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/spec/unit/puppet/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.773910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/spec/unit/puppet/parser/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.809910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/spec/unit/puppet/parser/functions/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      948 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/spec/unit/puppet/parser/functions/choose_my_ip_spec.rb
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.809910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/templates/openstack-neutron.modules.erb
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.809910 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/templates/ssl/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1753 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/templates/ssl/generate_ssl_certs.sh.erb
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.809910 packstack-23.0.0.0rc1/packstack/puppet/templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1863 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/templates/compute.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5787 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/templates/controller.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/templates/controller_post.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1387 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/puppet/templates/network.pp
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/packstack/version.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.777910 packstack-23.0.0.0rc1/packstack.egg-info/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    11345 2023-10-17 15:26:12.000000 packstack-23.0.0.0rc1/packstack.egg-info/PKG-INFO
--rw-rw-r--   0 zuul      (1000) zuul      (1000)    15446 2023-10-17 15:26:12.000000 packstack-23.0.0.0rc1/packstack.egg-info/SOURCES.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-10-17 15:26:12.000000 packstack-23.0.0.0rc1/packstack.egg-info/dependency_links.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2023-10-17 15:26:12.000000 packstack-23.0.0.0rc1/packstack.egg-info/entry_points.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2023-10-17 15:26:12.000000 packstack-23.0.0.0rc1/packstack.egg-info/not-zip-safe
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2023-10-17 15:26:12.000000 packstack-23.0.0.0rc1/packstack.egg-info/pbr.json
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2023-10-17 15:26:12.000000 packstack-23.0.0.0rc1/packstack.egg-info/requires.txt
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       10 2023-10-17 15:26:12.000000 packstack-23.0.0.0rc1/packstack.egg-info/top_level.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.809910 packstack-23.0.0.0rc1/playbooks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1019 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/playbooks/packstack-centos9-pre.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/playbooks/packstack-integration-tempest.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2480 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/playbooks/packstack-multinode.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      462 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/playbooks/packstack-post-compute.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/playbooks/upload-logs.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.773910 packstack-23.0.0.0rc1/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.821910 packstack-23.0.0.0rc1/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/Add-Panko-service-63a8a966013abeaa.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/Panko-has-been-removed-fb234a047231d84f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/Remove-CONFIG_NEUTRON_ML2_SUPPORTED_PCI_VENDOR_DEVS-param-926649e4eef08b44.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/Remove-FWaaS-deployment-41cfa0b709cd9a3f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/Remove-Heat-Cloudwatch-07e55f1c35a16ee4.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/Remove-PKI-and-UUID-Keystone-token-formats-618f4b0dc4cf782f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/Remove-deprecated-keystone-ldap-params-848d0eaf7a24273e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/Replace-keystone-token-flush-cron-job-with-fernet-rotation-5b1fccf2bc6add91.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/Support-for-extracted-placement-service-8ae75efbb1ad25b5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1018 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/add-parameter-messages-47d9cf6996f58230.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/add-skip-tempest-tests-option-86cf59ec5a61d349.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/add-support-to-ovn-networking-ae6e0176270265c6.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/add_cinder_solidfire-9b62f78b86a52a09.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/admin-token-removed-64ae39c4ecd28f15.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/aodh-move-to-mariadb-9e36b7cfdbbd2aa5.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/bp-add-magnum-support-74d88638fe4b2c6c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/ceilometer-with-wsgi-a46d2ff0ceabaaf8.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/change-default-nagios-b190de0737165bf9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/check-unexpected-options-2f2d26ebe54da6c9.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/create-uec-image-70073744430d1538.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/custom-tempest-flavors-baa5cf02235f78dd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/demo-allocation-pools-c535e4235c7edcb2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/demo-image-properties-9994f2981a8c00a1.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/disable-rabbitmq-repositories-d5cb9dc8f1246a39.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/drop-mongodb-a9771fb4f0430a4c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/gnocchi-and-aodh-00da52a4c45588fd.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/install-tempest-from-rpm-fd59c072011f372b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/integration-tests-d5f86a29cc037329.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/keystone-evenlet-dropped-6f85670db62f7b91.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/keystone-v3-note-065b6302b49285f3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      548 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/l3-agent-multiple-networks-9d1837c4187055be.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/manifest-execution-refactor-418c27bbc03df064.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/move-to-pymysql-b5f1a40ededa8fb2.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/neutron-ovs-bridges-compute-0aec0e39c1b1b84b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/nova-cert-86fb2f0ddc53b032.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/nova-cpu-manager-8440f026c4a0165e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/nova-migration-improvements-85b208c2b45a3fbe.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/nova-placement-api-acf32977978da6fb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/ovs-bridges-on-network-nodes-890c51cbbddf8f1c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/ovs-tunnel-subnets-8955593d3004852e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/packstack-moved-from-stackforge-766c35141b5480c3.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/qpid-removal-f754f589e335ae0c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/register-satellite6-server-796a5f89b39386a4.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.773910 packstack-23.0.0.0rc1/releasenotes/notes/releasenotes/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.821910 packstack-23.0.0.0rc1/releasenotes/notes/releasenotes/notes/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/releasenotes/notes/add-custom-lvm-name-090af5002950706d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      294 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/remove-cinder-gluster-6c54d9f440424259.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/remove-collector-api-5b494f09593197f0.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/remove-config-gnocchi-install-ecfe10ce59f1d0da.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/remove-epel-support-3732f53a2e45d64c.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/remove-glance-registry-6076539ab6ce1a8b.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/remove-lbaas-0054d83972c5afcf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/remove-legacy-nova-filters-d6e21a5e8f5c31a7.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/remove-nagios-deployment-21362a84a3ac446f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      866 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/remove-nova-network-8fe352ac6eb22ecb.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/remove-retry-filter-nova-05e84f3fd020d8ed.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/remove-uec-images-d876bd8c805d9633.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1429 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/renamed-ssl-subject-parameters-c2a52d17c349a59f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/reno-for-release-notes-66c17b84c946591f.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/service-workers-and-mariadb-c2a6ba903f36b57e.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/swift-s3-removal-ee3ddc2ee21a56cf.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/switch-default-neutron-driver-to-ovn-0eb7053b81c7794d.yaml
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/notes/update-puppet-module-usage-4ed869e87e67caaf.yaml
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.821910 packstack-23.0.0.0rc1/releasenotes/source/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.821910 packstack-23.0.0.0rc1/releasenotes/source/_static/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/source/_static/.placeholder
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.821910 packstack-23.0.0.0rc1/releasenotes/source/_templates/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/source/_templates/.placeholder
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     8804 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/source/conf.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/source/index.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/releasenotes/source/unreleased.rst
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.773910 packstack-23.0.0.0rc1/roles/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.773910 packstack-23.0.0.0rc1/roles/packstack-integration-tempest/
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.821910 packstack-23.0.0.0rc1/roles/packstack-integration-tempest/tasks/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/roles/packstack-integration-tempest/tasks/main.yaml
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)    11311 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/run_tests.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1017 2023-10-17 15:26:12.825910 packstack-23.0.0.0rc1/setup.cfg
--rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/test-requirements.txt
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.821910 packstack-23.0.0.0rc1/tests/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/tests/__init__.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.825910 packstack-23.0.0.0rc1/tests/installer/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/tests/installer/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1691 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/tests/installer/test_arch.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     7721 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/tests/installer/test_drones.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1535 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/tests/installer/test_processors.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5203 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/tests/installer/test_run_setup.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3226 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/tests/installer/test_sequences.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3425 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/tests/installer/test_setup_params.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4187 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/tests/installer/test_utils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     4300 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/tests/installer/test_validators.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.825910 packstack-23.0.0.0rc1/tests/modules/
--rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/tests/modules/__init__.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1111 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/tests/modules/test_ospluginutils.py
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     2543 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/tests/modules/test_puppet.py
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1297 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/tests/scenario-py3.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)      265 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/tests/scenario000.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1396 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/tests/scenario001.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1497 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/tests/scenario002.sh
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1269 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/tests/scenario003.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     5552 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/tests/test_base.py
-drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2023-10-17 15:26:12.825910 packstack-23.0.0.0rc1/tools/
--rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5250 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/tools/copy-logs.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     3711 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/tools/fix_disk_layout.sh
--rw-rw-r--   0 zuul      (1000) zuul      (1000)     1221 2023-10-17 15:25:26.000000 packstack-23.0.0.0rc1/tox.ini
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.612075 packstack-24.0.0.0rc1/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       39 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/.stestr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      157 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/.testr.conf
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     9395 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/.zuul.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5575 2024-04-18 12:00:14.000000 packstack-24.0.0.0rc1/AUTHORS
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    75112 2024-04-18 12:00:14.000000 packstack-24.0.0.0rc1/ChangeLog
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      650 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/Gemfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      237 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/MANIFEST.in
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11655 2024-04-18 12:00:14.612075 packstack-24.0.0.0rc1/PKG-INFO
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3546 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/Puppetfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8574 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/README.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      913 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/Rakefile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      112 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/bindep.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.572075 packstack-24.0.0.0rc1/docs/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5576 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/docs/Makefile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8548 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/docs/conf.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    54222 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/docs/packstack.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      549 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/external_modules.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      154 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/openstack_modules.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.572075 packstack-24.0.0.0rc1/packstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.576075 packstack-24.0.0.0rc1/packstack/installer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11358 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/installer/LICENSE
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/installer/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3649 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/installer/basedefs.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.576075 packstack-24.0.0.0rc1/packstack/installer/core/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/installer/core/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1189 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/installer/core/arch.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15319 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/installer/core/drones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2170 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/installer/core/parameters.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3650 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/installer/core/sequences.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2167 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/installer/exceptions.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5765 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/installer/output_messages.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5197 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/installer/processors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40967 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/installer/run_setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5347 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/installer/setup_controller.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.576075 packstack-24.0.0.0rc1/packstack/installer/utils/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1517 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/installer/utils/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4379 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/installer/utils/datastructures.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1382 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/installer/utils/decorators.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4447 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/installer/utils/network.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5734 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/installer/utils/shell.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1694 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/installer/utils/shortcuts.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2439 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/installer/utils/strings.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11910 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/installer/validators.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.576075 packstack-24.0.0.0rc1/packstack/modules/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/modules/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3767 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/modules/common.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2816 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/modules/documentation.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6529 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/modules/ospluginutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4733 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/modules/puppet.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.580075 packstack-24.0.0.0rc1/packstack/plugins/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/plugins/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7546 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/plugins/amqp_002.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4082 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/plugins/aodh_810.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7677 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/plugins/ceilometer_800.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    28691 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/plugins/cinder_250.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7836 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/plugins/dashboard_500.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4612 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/plugins/glance_200.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3495 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/plugins/gnocchi_790.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6709 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/plugins/heat_650.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3805 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/plugins/ironic_275.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    26987 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/plugins/keystone_100.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     4040 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/plugins/magnum_920.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    24727 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/plugins/manila_355.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4171 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/plugins/mariadb_003.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    40786 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/plugins/neutron_350.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    20087 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/plugins/nova_300.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2602 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/plugins/openstack_client_400.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2295 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/plugins/postscript_951.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    52951 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/plugins/prescript_000.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    17382 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/plugins/provision_700.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    11772 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/plugins/puppet_950.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11565 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/plugins/ssl_001.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11752 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/plugins/swift_600.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5575 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/plugins/trove_850.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.568076 packstack-24.0.0.0rc1/packstack/puppet/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.564075 packstack-24.0.0.0rc1/packstack/puppet/modules/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.580075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/Gemfile
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      249 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/Rakefile
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.564075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/lib/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.580075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      406 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/default_hypervisor.rb
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      135 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/home_dir.rb
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/mariadb.rb
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8175 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/netns.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      357 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/netns_support.rb
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      152 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/network.rb
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.564075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.564075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.584075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/functions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      766 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/functions/choose_my_ip.rb
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1277 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/functions/force_interface.rb
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      393 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/functions/force_ip.rb
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.584075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.584075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/amqp/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2219 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/amqp/enable_rabbitmq.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      558 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/amqp.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.588075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/aodh/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1556 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/aodh/rabbitmq.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1362 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/aodh.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       56 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/apache.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.588075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ceilometer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ceilometer/nova_disabled.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1457 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ceilometer/rabbitmq.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1340 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ceilometer.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2155 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/chrony.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.588075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.588075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3425 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/lvm.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8184 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/netapp.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      536 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/nfs.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      764 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/solidfire.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      408 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/vmdk.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      323 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backup.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1681 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/rabbitmq.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2251 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1132 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/firewall.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.588075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.588075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/backend/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      161 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/backend/file.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      736 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/backend/swift.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1376 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/ceilometer.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1472 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1764 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/gnocchi.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.588075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      578 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat/cfn.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2374 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat/rabbitmq.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      905 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2551 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/horizon.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.588075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ironic/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1639 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ironic/rabbitmq.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      500 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ironic.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.588075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      423 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/aodh.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      206 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/ceilometer.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      516 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/cinder.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      488 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/glance.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      464 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/gnocchi.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      613 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/heat.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      491 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/ironic.pp
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      586 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/magnum.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      654 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/manila.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      494 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/neutron.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/nova.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      800 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/placement.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      648 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/swift.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/trove.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     6766 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.592075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/magnum/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1313 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/magnum/rabbitmq.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1613 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/magnum.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.592075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.592075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1661 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/generic.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      459 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/glusternative.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      636 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/glusternfs.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1235 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/netapp.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1218 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/network.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1470 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/rabbitmq.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      832 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.592075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     3460 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb/services.pp
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    17070 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb/services_remote.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2436 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      314 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/memcached.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      487 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/netns.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.592075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1692 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/api.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1475 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/bridge.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      414 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/dhcp.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      475 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/l3.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1006 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/lb_agent.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      340 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/metadata.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/metering.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1715 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ml2.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/notifications.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2187 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovn_agent.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      537 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovn_metadata.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       68 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovn_northd.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2248 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovs_agent.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      270 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovs_bridge.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1717 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/rabbitmq.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      201 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/sriov.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      190 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/vpnaas.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      457 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.596075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3790 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/api.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.596075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/ceilometer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1731 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/ceilometer/rabbitmq.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      483 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/ceilometer.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      359 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/common.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.596075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      504 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute/ironic.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2819 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute/libvirt.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      463 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute/vmware.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4234 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/conductor.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      263 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/metadata.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      526 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/neutron.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       92 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/nfs.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.596075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/sched/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/sched/ironic.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      246 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/sched.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      430 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/vncproxy.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3354 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2963 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/openstackclient.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      835 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/placement.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      285 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/prereqs.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.596075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1995 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/bridge.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      596 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/glance.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7356 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/tempest.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3940 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      450 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/redis.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.596075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      797 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/ceilometer.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      275 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/fs.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3447 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/proxy.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1171 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/ringbuilder.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1298 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/storage.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      257 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.596075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/trove/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1634 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/trove/rabbitmq.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1236 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/trove.pp
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.596075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/spec/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      381 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/spec/spec_helper.rb
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.568076 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/spec/unit/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.568076 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/spec/unit/puppet/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.568076 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/spec/unit/puppet/parser/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.596075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/spec/unit/puppet/parser/functions/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      948 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/spec/unit/puppet/parser/functions/choose_my_ip_spec.rb
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.596075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       93 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/templates/openstack-neutron.modules.erb
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.596075 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/templates/ssl/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1753 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/templates/ssl/generate_ssl_certs.sh.erb
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.596075 packstack-24.0.0.0rc1/packstack/puppet/templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1863 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/templates/compute.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5532 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/templates/controller.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/templates/controller_post.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1387 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/puppet/templates/network.pp
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      642 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/packstack/version.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.572075 packstack-24.0.0.0rc1/packstack.egg-info/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    11655 2024-04-18 12:00:14.000000 packstack-24.0.0.0rc1/packstack.egg-info/PKG-INFO
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)    15263 2024-04-18 12:00:14.000000 packstack-24.0.0.0rc1/packstack.egg-info/SOURCES.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-18 12:00:14.000000 packstack-24.0.0.0rc1/packstack.egg-info/dependency_links.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2024-04-18 12:00:14.000000 packstack-24.0.0.0rc1/packstack.egg-info/entry_points.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        1 2024-04-18 12:00:14.000000 packstack-24.0.0.0rc1/packstack.egg-info/not-zip-safe
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       47 2024-04-18 12:00:14.000000 packstack-24.0.0.0rc1/packstack.egg-info/pbr.json
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       87 2024-04-18 12:00:14.000000 packstack-24.0.0.0rc1/packstack.egg-info/requires.txt
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       10 2024-04-18 12:00:14.000000 packstack-24.0.0.0rc1/packstack.egg-info/top_level.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.600075 packstack-24.0.0.0rc1/playbooks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1322 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/playbooks/packstack-centos9-pre.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       58 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/playbooks/packstack-integration-tempest.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2480 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/playbooks/packstack-multinode.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      462 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/playbooks/packstack-post-compute.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      337 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/playbooks/upload-logs.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.568076 packstack-24.0.0.0rc1/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.608075 packstack-24.0.0.0rc1/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       61 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/Add-Panko-service-63a8a966013abeaa.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      333 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/Panko-has-been-removed-fb234a047231d84f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      228 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/Remove-CONFIG_NEUTRON_ML2_SUPPORTED_PCI_VENDOR_DEVS-param-926649e4eef08b44.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      243 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/Remove-FWaaS-deployment-41cfa0b709cd9a3f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      183 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/Remove-Heat-Cloudwatch-07e55f1c35a16ee4.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      212 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/Remove-PKI-and-UUID-Keystone-token-formats-618f4b0dc4cf782f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      310 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/Remove-deprecated-keystone-ldap-params-848d0eaf7a24273e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      425 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/Replace-keystone-token-flush-cron-job-with-fernet-rotation-5b1fccf2bc6add91.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      168 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/Support-for-extracted-placement-service-8ae75efbb1ad25b5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1018 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/add-parameter-messages-47d9cf6996f58230.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      182 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/add-skip-tempest-tests-option-86cf59ec5a61d349.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      858 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/add-support-to-ovn-networking-ae6e0176270265c6.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      358 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/add_cinder_solidfire-9b62f78b86a52a09.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      179 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/admin-token-removed-64ae39c4ecd28f15.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      313 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/aodh-move-to-mariadb-9e36b7cfdbbd2aa5.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/bp-add-magnum-support-74d88638fe4b2c6c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       86 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/ceilometer-with-wsgi-a46d2ff0ceabaaf8.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      302 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/change-default-nagios-b190de0737165bf9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      124 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/check-unexpected-options-2f2d26ebe54da6c9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      505 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/create-uec-image-70073744430d1538.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      137 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/custom-tempest-flavors-baa5cf02235f78dd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      122 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/demo-allocation-pools-c535e4235c7edcb2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      140 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/demo-image-properties-9994f2981a8c00a1.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      129 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/disable-rabbitmq-repositories-d5cb9dc8f1246a39.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/drop-mongodb-a9771fb4f0430a4c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      355 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/gnocchi-and-aodh-00da52a4c45588fd.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/install-tempest-from-rpm-fd59c072011f372b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      627 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/integration-tests-d5f86a29cc037329.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      245 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/keystone-evenlet-dropped-6f85670db62f7b91.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      150 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/keystone-v3-note-065b6302b49285f3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      548 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/l3-agent-multiple-networks-9d1837c4187055be.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1036 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/manifest-execution-refactor-418c27bbc03df064.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       82 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/move-to-pymysql-b5f1a40ededa8fb2.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      407 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/neutron-ovs-bridges-compute-0aec0e39c1b1b84b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       97 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/nova-cert-86fb2f0ddc53b032.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       88 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/nova-cpu-manager-8440f026c4a0165e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      172 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/nova-migration-improvements-85b208c2b45a3fbe.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      120 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/nova-placement-api-acf32977978da6fb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      123 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/ovs-bridges-on-network-nodes-890c51cbbddf8f1c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      217 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/ovs-tunnel-subnets-8955593d3004852e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      155 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/packstack-moved-from-stackforge-766c35141b5480c3.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      143 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/qpid-removal-f754f589e335ae0c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       66 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/register-satellite6-server-796a5f89b39386a4.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.568076 packstack-24.0.0.0rc1/releasenotes/notes/releasenotes/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.608075 packstack-24.0.0.0rc1/releasenotes/notes/releasenotes/notes/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      160 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/releasenotes/notes/add-custom-lvm-name-090af5002950706d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      294 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/remove-cinder-gluster-6c54d9f440424259.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       76 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/remove-collector-api-5b494f09593197f0.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      241 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/remove-config-gnocchi-install-ecfe10ce59f1d0da.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      178 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/remove-epel-support-3732f53a2e45d64c.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      184 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/remove-glance-registry-6076539ab6ce1a8b.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      103 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/remove-lbaas-0054d83972c5afcf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      163 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/remove-legacy-nova-filters-d6e21a5e8f5c31a7.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      396 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/remove-nagios-deployment-21362a84a3ac446f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      866 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/remove-nova-network-8fe352ac6eb22ecb.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      153 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/remove-retry-filter-nova-05e84f3fd020d8ed.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      111 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/remove-sahara-79e02a209c7128e9.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      385 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/remove-uec-images-d876bd8c805d9633.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1429 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/renamed-ssl-subject-parameters-c2a52d17c349a59f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      117 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/reno-for-release-notes-66c17b84c946591f.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      387 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/service-workers-and-mariadb-c2a6ba903f36b57e.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      128 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/swift-s3-removal-ee3ddc2ee21a56cf.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      501 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/switch-default-neutron-driver-to-ovn-0eb7053b81c7794d.yaml
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      159 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/notes/update-puppet-module-usage-4ed869e87e67caaf.yaml
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.608075 packstack-24.0.0.0rc1/releasenotes/source/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.608075 packstack-24.0.0.0rc1/releasenotes/source/_static/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/source/_static/.placeholder
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.608075 packstack-24.0.0.0rc1/releasenotes/source/_templates/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/source/_templates/.placeholder
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     8804 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/source/conf.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      209 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/source/index.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       77 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/releasenotes/source/unreleased.rst
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      100 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.568076 packstack-24.0.0.0rc1/roles/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.568076 packstack-24.0.0.0rc1/roles/packstack-integration-tempest/
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.608075 packstack-24.0.0.0rc1/roles/packstack-integration-tempest/tasks/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      465 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/roles/packstack-integration-tempest/tasks/main.yaml
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)    10665 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/run_tests.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1017 2024-04-18 12:00:14.612075 packstack-24.0.0.0rc1/setup.cfg
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)       84 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)      171 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/test-requirements.txt
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.608075 packstack-24.0.0.0rc1/tests/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/tests/__init__.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.608075 packstack-24.0.0.0rc1/tests/installer/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/tests/installer/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1691 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/tests/installer/test_arch.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     7721 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/tests/installer/test_drones.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1535 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/tests/installer/test_processors.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5203 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/tests/installer/test_run_setup.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3226 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/tests/installer/test_sequences.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3425 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/tests/installer/test_setup_params.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4187 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/tests/installer/test_utils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     4300 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/tests/installer/test_validators.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.612075 packstack-24.0.0.0rc1/tests/modules/
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)        0 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/tests/modules/__init__.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1111 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/tests/modules/test_ospluginutils.py
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     2543 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/tests/modules/test_puppet.py
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1297 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/tests/scenario-py3.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)      265 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/tests/scenario000.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1396 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/tests/scenario001.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1454 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/tests/scenario002.sh
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     1269 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/tests/scenario003.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     5552 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/tests/test_base.py
+drwxrwxr-x   0 zuul      (1000) zuul      (1000)        0 2024-04-18 12:00:14.612075 packstack-24.0.0.0rc1/tools/
+-rwxrwxr-x   0 zuul      (1000) zuul      (1000)     5250 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/tools/copy-logs.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     3711 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/tools/fix_disk_layout.sh
+-rw-rw-r--   0 zuul      (1000) zuul      (1000)     1221 2024-04-18 11:59:31.000000 packstack-24.0.0.0rc1/tox.ini
```

### Comparing `packstack-23.0.0.0rc1/.zuul.yaml` & `packstack-24.0.0.0rc1/.zuul.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -17,20 +17,18 @@
       - openstack/puppet-magnum
       - openstack/puppet-horizon
       - openstack/puppet-ironic
       - openstack/puppet-keystone
       - openstack/puppet-manila
       - openstack/puppet-neutron
       - openstack/puppet-nova
-      - openstack/puppet-openstack_extras
       - openstack/puppet-openstacklib
       - openstack/puppet-oslo
       - openstack/puppet-ovn
       - openstack/puppet-placement
-      - openstack/puppet-sahara
       - openstack/puppet-swift
       - openstack/puppet-tempest
       - openstack/puppet-trove
       - openstack/puppet-vswitch
 
 - job:
     name: packstack-centos9
```

### Comparing `packstack-23.0.0.0rc1/AUTHORS` & `packstack-24.0.0.0rc1/AUTHORS`

 * *Files 1% similar despite different names*

```diff
@@ -125,14 +125,15 @@
 Shahar Havivi <shavivi@redhat.com>
 Sofer Athlan-Guyot <chem@sathlan.org>
 Solly Ross <sross@redhat.com>
 Steven Hardy <shardy@redhat.com>
 Summer Long <slong@redhat.com>
 Suraj Narwade <hackersvilla123@gmail.com>
 Swapnil Kulkarni (coolsvap) <me@coolsvap.net>
+Takashi Kajinami <kajinamit@oss.nttdata.com>
 Takashi Kajinami <tkajinam@redhat.com>
 Takeshi Kusune <kusune@bridgehead.group.gr.jp>
 Terry Wilson <twilson@redhat.com>
 Tobias Urdin <tobias.urdin@binero.se>
 Tony Breeds <tony@bakeyournoodle.com>
 Vieri <15050873171@163.com>
 Vladan Popovic <vpopovic@redhat.com>
```

### Comparing `packstack-23.0.0.0rc1/ChangeLog` & `packstack-24.0.0.0rc1/ChangeLog`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,26 @@
 CHANGES
 =======
 
+24.0.0.0rc1
+-----------
+
+* Nova: Enable service token
+* Generate Puppetfile
+* Follow puppet-systemd master again
+* Clean up unnecessary workaround related to puppetlabs-apache
+* Fix branch to pull puppetlabs-xinetd
+* Add info about bug tracking tool for packstack
+* Add enable-chassis-as-gw option for OVN CMS cluster
+* Bump cirros version
+* Remove script logic for CentOS/RHEL < 7
+* Prohibit retired/unmaintained network plugins
+* Remove sahara support
+* Remove reference to monolithic puppet-openstack
+
 23.0.0.0rc1
 -----------
 
 * The \`action\` attribute within the \`firewall\` type has been removed
 
 22.0.0.0rc1
 -----------
@@ -509,16 +525,16 @@
 * Add release notes for the Mitaka cycle
 * Try setting the tuned profile more than once
 * Fix mode for rabbitmq.config
 * Start managing release notes in Packstack with Reno
 * Configure gnocchi statsd service
 * Make ceilometer metering backend configurable
 
-8.0.0.0rc1
-----------
+8.0.0rc1
+--------
 
 * Deploy ceilometer api as wsgi
 * Add libyaml-devel to list of dependencies
 * Add a switch to install from source or binary
 * Allow arbitrary amount of lines between Subscription Name and Pool ID
 * Do not enable RabbitMQ repo during installation
 * Replacing keystone user-list with openstack user list
```

### Comparing `packstack-23.0.0.0rc1/Gemfile` & `packstack-24.0.0.0rc1/Gemfile`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/LICENSE` & `packstack-24.0.0.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/PKG-INFO` & `packstack-24.0.0.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packstack
-Version: 23.0.0.0rc1
+Version: 24.0.0.0rc1
 Summary: A utility to install OpenStack
 Home-page: http://www.rdoproject.org/
 Author: RDO
 Author-email: rdo-list@redhat.com
 License: UNKNOWN
 Description: Packstack
         =========
@@ -254,15 +254,14 @@
         vpnaas                                            
         cinder         X           X                      
         ceilometer     X                                   X
         aodh           X                                   X
         gnocchi        X                                   X
         heat                                               X
         swift          X                       X          
-        sahara                                 X          
         trove                                  X          
         horizon                    X                      
         manila                     X                      
         SSL                        X                      
         ============== =========== =========== =========== ===========
         
         To run these tests:
@@ -290,14 +289,20 @@
         
         ::
         
            <setup your own custom repositories here>
            export MANAGE_REPOS="false"
            ./run_tests.sh
         
+        Reporting Bugs
+        --------------
+        
+        Bugs for packstack are tracked in the "packstack" component of the [RDO Jira board](https://issues.redhat.com/issues/?jql=project+%3D+RDO+AND+component+%3D+packstack).
+        If you find issues, you can create an issue on that board and provide the relevant information to describe your problem.
+        
         
 Platform: UNKNOWN
 Classifier: Environment :: OpenStack
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `packstack-23.0.0.0rc1/Puppetfile` & `packstack-24.0.0.0rc1/Puppetfile`

 * *Files 0% similar despite different names*

```diff
@@ -50,18 +50,14 @@
   :git => 'https://github.com/openstack/puppet-neutron',
   :ref => 'master'
 
 mod 'nova',
   :git => 'https://github.com/openstack/puppet-nova',
   :ref => 'master'
 
-mod 'openstack_extras',
-  :git => 'https://github.com/openstack/puppet-openstack_extras',
-  :ref => 'master'
-
 mod 'openstacklib',
   :git => 'https://github.com/openstack/puppet-openstacklib',
   :ref => 'master'
 
 mod 'oslo',
   :git => 'https://github.com/openstack/puppet-oslo',
   :ref => 'master'
@@ -70,18 +66,14 @@
   :git => 'https://github.com/openstack/puppet-ovn',
   :ref => 'master'
 
 mod 'placement',
   :git => 'https://github.com/openstack/puppet-placement',
   :ref => 'master'
 
-mod 'sahara',
-  :git => 'https://github.com/openstack/puppet-sahara',
-  :ref => 'master'
-
 mod 'swift',
   :git => 'https://github.com/openstack/puppet-swift',
   :ref => 'master'
 
 mod 'tempest',
   :git => 'https://github.com/openstack/puppet-tempest',
   :ref => 'master'
@@ -149,18 +141,18 @@
   :ref => 'main'
 
 mod 'sysctl',
   :git => 'https://github.com/duritong/puppet-sysctl',
   :ref => 'master'
 
 mod 'systemd',
-  :git => 'https://github.com/camptocamp/puppet-systemd',
-  :ref => '8f68b0dcf3bbbafc60c025879a28004fc9815aab'
+  :git => 'https://github.com/voxpupuli/puppet-systemd',
+  :ref => 'master'
 
 mod 'vcsrepo',
   :git => 'https://github.com/puppetlabs/puppetlabs-vcsrepo',
   :ref => 'main'
 
 mod 'xinetd',
   :git => 'https://github.com/puppetlabs/puppetlabs-xinetd',
-  :ref => 'master'
+  :ref => 'main'
```

### Comparing `packstack-23.0.0.0rc1/README.rst` & `packstack-24.0.0.0rc1/README.rst`

 * *Files 12% similar despite different names*

```diff
@@ -246,15 +246,14 @@
 vpnaas                                            
 cinder         X           X                      
 ceilometer     X                                   X
 aodh           X                                   X
 gnocchi        X                                   X
 heat                                               X
 swift          X                       X          
-sahara                                 X          
 trove                                  X          
 horizon                    X                      
 manila                     X                      
 SSL                        X                      
 ============== =========== =========== =========== ===========
 
 To run these tests:
@@ -281,7 +280,14 @@
 You can also choose to disable repository management entirely:
 
 ::
 
    <setup your own custom repositories here>
    export MANAGE_REPOS="false"
    ./run_tests.sh
+
+Reporting Bugs
+--------------
+
+Bugs for packstack are tracked in the "packstack" component of the [RDO Jira board](https://issues.redhat.com/issues/?jql=project+%3D+RDO+AND+component+%3D+packstack).
+If you find issues, you can create an issue on that board and provide the relevant information to describe your problem.
+
```

### Comparing `packstack-23.0.0.0rc1/Rakefile` & `packstack-24.0.0.0rc1/Rakefile`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/docs/Makefile` & `packstack-24.0.0.0rc1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/docs/conf.py` & `packstack-24.0.0.0rc1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/docs/packstack.rst` & `packstack-24.0.0.0rc1/docs/packstack.rst`

 * *Files 2% similar despite different names*

```diff
@@ -68,17 +68,14 @@
 
 **CONFIG_HEAT_INSTALL**
     Specify 'y' to install OpenStack Orchestration (heat). ['y', 'n']
 
 **CONFIG_MAGNUM_INSTALL**
     Specify 'y' to install OpenStack Container Infrastructure Management Service (magnum). ['y', 'n']
 
-**CONFIG_SAHARA_INSTALL**
-    Specify 'y' to install OpenStack Data Processing (sahara). In case of sahara installation packstack also installs heat.['y', 'n']
-
 **CONFIG_TROVE_INSTALL**
     Specify 'y' to install OpenStack Database (trove) ['y', 'n']
 
 **CONFIG_IRONIC_INSTALL**
     Specify 'y' to install OpenStack Bare Metal Provisioning (ironic). ['y', 'n']
 
 **CONFIG_CLIENT_INSTALL**
@@ -166,17 +163,14 @@
 
 Global unsupported options
 --------------------------
 
 **CONFIG_STORAGE_HOST**
     (Unsupported!) Server on which to install OpenStack services specific to storage servers such as Image or Block Storage services.
 
-**CONFIG_SAHARA_HOST**
-    (Unsupported!) Server on which to install OpenStack services specific to OpenStack Data Processing (sahara).
-
 Server Prepare Configs
 -----------------------
 
 **CONFIG_REPO**
     Comma-separated list of URLs for any additional yum repositories, to use for installation.
 
 **CONFIG_ENABLE_RDO_TESTING**
@@ -766,15 +760,15 @@
 **CONFIG_NEUTRON_ML2_TYPE_DRIVERS**
     Comma-separated list of network-type driver entry points to be loaded from the neutron.ml2.type_drivers namespace. ['local', 'flat', 'vlan', 'gre', 'vxlan', 'geneve']
 
 **CONFIG_NEUTRON_ML2_TENANT_NETWORK_TYPES**
     Comma-separated, ordered list of network types to allocate as tenant networks. The 'local' value is only useful for single-box testing and provides no connectivity between hosts. ['local', 'vlan', 'gre', 'vxlan', 'geneve']
 
 **CONFIG_NEUTRON_ML2_MECHANISM_DRIVERS**
-    Comma-separated ordered list of networking mechanism driver entry points to be loaded from the neutron.ml2.mechanism_drivers namespace. ['logger', 'test', 'linuxbridge', 'openvswitch', 'hyperv', 'ncs', 'arista', 'cisco_nexus', 'mlnx', 'l2population', 'sriovnicswitch', 'ovn']
+    Comma-separated ordered list of networking mechanism driver entry points to be loaded from the neutron.ml2.mechanism_drivers namespace. ['logger', 'test', 'linuxbridge', 'openvswitch', 'arista', 'mlnx', 'l2population', 'sriovnicswitch', 'ovn']
 
 **CONFIG_NEUTRON_ML2_FLAT_NETWORKS**
     Comma-separated list of physical_network names with which flat networks can be created. Use * to allow flat networks with arbitrary physical_network names.
 
 **CONFIG_NEUTRON_ML2_VLAN_RANGES**
     Comma-separated list of <physical_network>:<vlan_min>:<vlan_max> or <physical_network> specifying physical_network names usable for VLAN provider and tenant networks, as well as ranges of VLAN tags on each available for allocation to tenant networks.
 
@@ -1067,23 +1061,14 @@
 **CONFIG_GNOCCHI_DB_PW**
     Password to use for Gnocchi to access the database.
 
 **CONFIG_GNOCCHI_KS_PW**
     Password to use for Gnocchi to authenticate with the Identity service.
 
 
-Sahara Config parameters
-------------------------
-
-**CONFIG_SAHARA_DB_PW**
-    Password to use for OpenStack Data Processing (sahara) to access the database.
-
-**CONFIG_SAHARA_KS_PW**
-    Password to use for OpenStack Data Processing to authenticate with the Identity service.
-
 Trove config parameters
 -----------------------
 
 **CONFIG_TROVE_DB_PW**
     Password to use for OpenStack Database-as-a-Service (trove) to access the database.
 
 **CONFIG_TROVE_KS_PW**
```

### Comparing `packstack-23.0.0.0rc1/packstack/installer/LICENSE` & `packstack-24.0.0.0rc1/packstack/installer/LICENSE`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/installer/basedefs.py` & `packstack-24.0.0.0rc1/packstack/installer/basedefs.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/installer/core/arch.py` & `packstack-24.0.0.0rc1/packstack/installer/core/arch.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/installer/core/drones.py` & `packstack-24.0.0.0rc1/packstack/installer/core/drones.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/installer/core/parameters.py` & `packstack-24.0.0.0rc1/packstack/installer/core/parameters.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/installer/core/sequences.py` & `packstack-24.0.0.0rc1/packstack/installer/core/sequences.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/installer/exceptions.py` & `packstack-24.0.0.0rc1/packstack/installer/exceptions.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/installer/output_messages.py` & `packstack-24.0.0.0rc1/packstack/installer/output_messages.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/installer/processors.py` & `packstack-24.0.0.0rc1/packstack/installer/processors.py`

 * *Files 2% similar despite different names*

```diff
@@ -121,16 +121,14 @@
                 process_password.pw_dict[param_name] = param
             else:
                 param = process_password.pw_dict[param_name]
     return param
 
 
 def process_heat(param, param_name, config=None):
-    if config["CONFIG_SAHARA_INSTALL"] == 'y':
-        param = 'y'
     return param
 
 
 def process_string_nofloat(param, param_name, config=None):
     """
     Process a string, making sure it is *not* convertible into a float
     If it is, change it into a random 16 char string, and check again
```

### Comparing `packstack-23.0.0.0rc1/packstack/installer/run_setup.py` & `packstack-24.0.0.0rc1/packstack/installer/run_setup.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/installer/setup_controller.py` & `packstack-24.0.0.0rc1/packstack/installer/setup_controller.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/installer/utils/__init__.py` & `packstack-24.0.0.0rc1/packstack/installer/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/installer/utils/datastructures.py` & `packstack-24.0.0.0rc1/packstack/installer/utils/datastructures.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/installer/utils/decorators.py` & `packstack-24.0.0.0rc1/packstack/installer/utils/decorators.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/installer/utils/network.py` & `packstack-24.0.0.0rc1/packstack/installer/utils/network.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/installer/utils/shell.py` & `packstack-24.0.0.0rc1/packstack/installer/utils/shell.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/installer/utils/shortcuts.py` & `packstack-24.0.0.0rc1/packstack/installer/utils/shortcuts.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/installer/utils/strings.py` & `packstack-24.0.0.0rc1/packstack/installer/utils/strings.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/installer/validators.py` & `packstack-24.0.0.0rc1/packstack/installer/validators.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/modules/common.py` & `packstack-24.0.0.0rc1/packstack/modules/common.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/modules/documentation.py` & `packstack-24.0.0.0rc1/packstack/modules/documentation.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/modules/ospluginutils.py` & `packstack-24.0.0.0rc1/packstack/modules/ospluginutils.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/modules/puppet.py` & `packstack-24.0.0.0rc1/packstack/modules/puppet.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/plugins/amqp_002.py` & `packstack-24.0.0.0rc1/packstack/plugins/amqp_002.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/plugins/aodh_810.py` & `packstack-24.0.0.0rc1/packstack/plugins/aodh_810.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/plugins/ceilometer_800.py` & `packstack-24.0.0.0rc1/packstack/plugins/ceilometer_800.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/plugins/cinder_250.py` & `packstack-24.0.0.0rc1/packstack/plugins/cinder_250.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/plugins/dashboard_500.py` & `packstack-24.0.0.0rc1/packstack/plugins/dashboard_500.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/plugins/glance_200.py` & `packstack-24.0.0.0rc1/packstack/plugins/glance_200.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/plugins/gnocchi_790.py` & `packstack-24.0.0.0rc1/packstack/plugins/gnocchi_790.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/plugins/heat_650.py` & `packstack-24.0.0.0rc1/packstack/plugins/heat_650.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/plugins/ironic_275.py` & `packstack-24.0.0.0rc1/packstack/plugins/ironic_275.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/plugins/keystone_100.py` & `packstack-24.0.0.0rc1/packstack/plugins/keystone_100.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/plugins/magnum_920.py` & `packstack-24.0.0.0rc1/packstack/plugins/magnum_920.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/plugins/manila_355.py` & `packstack-24.0.0.0rc1/packstack/plugins/manila_355.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/plugins/mariadb_003.py` & `packstack-24.0.0.0rc1/packstack/plugins/mariadb_003.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/plugins/neutron_350.py` & `packstack-24.0.0.0rc1/packstack/plugins/neutron_350.py`

 * *Files 1% similar despite different names*

```diff
@@ -340,16 +340,16 @@
              "CONDITION": False},
 
             {"CMD_OPTION": "os-neutron-ml2-mechanism-drivers",
              "CONF_NAME": "CONFIG_NEUTRON_ML2_MECHANISM_DRIVERS",
              "PROMPT": ("Enter a comma separated ordered list of networking "
                         "mechanism driver entrypoints"),
              "OPTION_LIST": ["logger", "test", "linuxbridge", "openvswitch",
-                             "hyperv", "ncs", "arista", "cisco_nexus",
-                             "mlnx", "l2population", "sriovnicswitch", "ovn"],
+                             "arista", "mlnx", "l2population",
+                             "sriovnicswitch", "ovn"],
              "VALIDATORS": [validators.validate_multi_options],
              "DEFAULT_VALUE": "ovn",
              "MASK_INPUT": False,
              "LOOSE_VALIDATION": False,
              "USE_DEFAULT": False,
              "NEED_CONFIRM": False,
              "CONDITION": False},
```

### Comparing `packstack-23.0.0.0rc1/packstack/plugins/nova_300.py` & `packstack-24.0.0.0rc1/packstack/plugins/nova_300.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/plugins/openstack_client_400.py` & `packstack-24.0.0.0rc1/packstack/plugins/openstack_client_400.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/plugins/postscript_951.py` & `packstack-24.0.0.0rc1/packstack/plugins/postscript_951.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/plugins/prescript_000.py` & `packstack-24.0.0.0rc1/packstack/plugins/prescript_000.py`

 * *Files 1% similar despite different names*

```diff
@@ -227,29 +227,14 @@
              "MASK_INPUT": False,
              "LOOSE_VALIDATION": False,
              "CONF_NAME": "CONFIG_AODH_INSTALL",
              "USE_DEFAULT": False,
              "NEED_CONFIRM": False,
              "CONDITION": False},
 
-            {"CMD_OPTION": "os-sahara-install",
-             "PROMPT": (
-                 "Should Packstack install OpenStack Clustering (Sahara)."
-                 " If yes it'll also install Heat."
-             ),
-             "OPTION_LIST": ["y", "n"],
-             "VALIDATORS": [validators.validate_options],
-             "DEFAULT_VALUE": "n",
-             "MASK_INPUT": False,
-             "LOOSE_VALIDATION": False,
-             "CONF_NAME": "CONFIG_SAHARA_INSTALL",
-             "USE_DEFAULT": False,
-             "NEED_CONFIRM": False,
-             "CONDITION": False},
-
             {"CMD_OPTION": "os-heat-install",
              "PROMPT": (
                  "Should Packstack install OpenStack Orchestration (Heat)"
              ),
              "OPTION_LIST": ["y", "n"],
              "VALIDATORS": [validators.validate_options],
              "PROCESSORS": [processors.process_heat],
@@ -513,26 +498,14 @@
              "OPTION_LIST": [],
              "VALIDATORS": [validators.validate_ssh],
              "DEFAULT_VALUE": utils.get_localhost_ip(),
              "MASK_INPUT": False,
              "LOOSE_VALIDATION": False,
              "USE_DEFAULT": False,
              "NEED_CONFIRM": False,
-             "CONDITION": False},
-
-            {"CONF_NAME": "CONFIG_SAHARA_HOST",
-             "CMD_OPTION": "os-sahara-host",
-             "PROMPT": "Enter the host for the Sahara",
-             "OPTION_LIST": [],
-             "VALIDATORS": [validators.validate_ssh],
-             "DEFAULT_VALUE": utils.get_localhost_ip(),
-             "MASK_INPUT": False,
-             "LOOSE_VALIDATION": False,
-             "USE_DEFAULT": False,
-             "NEED_CONFIRM": False,
              "CONDITION": False},
         ],
 
         "SERVERPREPARE": [
             {"CMD_OPTION": "additional-repo",
              "PROMPT": ("Enter a comma separated list of URLs to any "
                         "additional yum repositories to install"),
```

### Comparing `packstack-23.0.0.0rc1/packstack/plugins/provision_700.py` & `packstack-24.0.0.0rc1/packstack/plugins/provision_700.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/plugins/puppet_950.py` & `packstack-24.0.0.0rc1/packstack/plugins/puppet_950.py`

 * *Files 2% similar despite different names*

```diff
@@ -145,19 +145,18 @@
 
 
 def copy_puppet_modules(config, messages):
     os_modules = ' '.join(('aodh', 'apache', 'ceilometer', 'cinder', 'concat',
                            'firewall', 'glance', 'gnocchi', 'heat', 'horizon',
                            'inifile', 'ironic', 'keystone', 'magnum', 'manila',
                            'memcached', 'mysql', 'neutron', 'nova', 'nssdb',
-                           'openstack', 'openstacklib', 'oslo', 'ovn',
-                           'packstack', 'placement', 'rabbitmq', 'redis',
-                           'remote', 'rsync', 'sahara', 'ssh', 'stdlib',
-                           'swift', 'sysctl', 'systemd', 'tempest', 'trove',
-                           'vcsrepo', 'vswitch', 'xinetd'))
+                           'openstacklib', 'oslo', 'ovn', 'packstack',
+                           'placement', 'rabbitmq', 'redis', 'remote', 'rsync',
+                           'ssh', 'stdlib', 'swift', 'sysctl', 'systemd',
+                           'tempest', 'trove', 'vcsrepo', 'vswitch', 'xinetd'))
 
     # write puppet manifest to disk
     manifestfiles.writeManifests()
     # write hieradata file to disk
     generateHieraDataFile()
 
     server = utils.ScriptRunner()
```

### Comparing `packstack-23.0.0.0rc1/packstack/plugins/sahara_900.py` & `packstack-24.0.0.0rc1/packstack/plugins/trove_850.py`

 * *Files 25% similar despite different names*

```diff
@@ -9,100 +9,150 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or
 # implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 """
-Installs and configures Sahara
+Installs and configures Trove
 """
 
 from packstack.installer import basedefs
 from packstack.installer import utils
 from packstack.installer import validators
 from packstack.installer import processors
 
 from packstack.modules.documentation import update_params_usage
 from packstack.modules.ospluginutils import generate_ssl_cert
 
-# ------------------ Sahara installer initialization ------------------
+# ------------------ Trove Packstack Plugin initialization ------------------
 
-PLUGIN_NAME = "OS-Sahara"
-PLUGIN_NAME_COLORED = utils.color_text(PLUGIN_NAME, "blue")
+PLUGIN_NAME = "OS-Trove"
+PLUGIN_NAME_COLORED = utils.color_text(PLUGIN_NAME, 'blue')
+
+
+# NOVA_USER, NOVA_TENANT, NOVA_PW
+
+def process_trove_nova_pw(param, param_name, config=None):
+    if (param == 'PW_PLACEHOLDER' and
+            config['CONFIG_TROVE_NOVA_USER'] == 'trove'):
+        return config['CONFIG_TROVE_KS_PW']
+    else:
+        return param
 
 
 def initConfig(controller):
-    params = [
-        {"CONF_NAME": "CONFIG_SAHARA_DB_PW",
-         "CMD_OPTION": "sahara-db-passwd",
-         "PROMPT": "Enter the password to use for Sahara to access the DB",
+    parameters = [
+        {"CONF_NAME": "CONFIG_TROVE_DB_PW",
+         "CMD_OPTION": "trove-db-passwd",
+         "PROMPT": "Enter the password to use for Trove to access the DB",
          "OPTION_LIST": [],
          "VALIDATORS": [validators.validate_not_empty],
          "DEFAULT_VALUE": "PW_PLACEHOLDER",
          "PROCESSORS": [processors.process_password],
          "MASK_INPUT": True,
          "LOOSE_VALIDATION": False,
          "USE_DEFAULT": False,
          "NEED_CONFIRM": True,
          "CONDITION": False},
 
-        {"CONF_NAME": "CONFIG_SAHARA_KS_PW",
-         "CMD_OPTION": "sahara-ks-passwd",
-         "PROMPT": "Enter the password for Sahara Keystone access",
+        {"CONF_NAME": "CONFIG_TROVE_KS_PW",
+         "CMD_OPTION": "trove-ks-passwd",
+         "PROMPT": "Enter the password for Trove Keystone access",
          "OPTION_LIST": [],
          "VALIDATORS": [validators.validate_not_empty],
          "DEFAULT_VALUE": "PW_PLACEHOLDER",
          "PROCESSORS": [processors.process_password],
          "MASK_INPUT": True,
          "LOOSE_VALIDATION": False,
          "USE_DEFAULT": False,
          "NEED_CONFIRM": True,
          "CONDITION": False},
+
+        {"CONF_NAME": "CONFIG_TROVE_NOVA_USER",
+         "CMD_OPTION": "trove-nova-user",
+         "PROMPT": "Enter the user for Trove to use to connect to Nova",
+         "OPTION_LIST": [],
+         "VALIDATORS": [validators.validate_not_empty],
+         "DEFAULT_VALUE": "trove",
+         "MASK_INPUT": False,
+         "LOOSE_VALIDATION": False,
+         "USE_DEFAULT": True,
+         "NEED_CONFIRM": True,
+         "CONDITION": False},
+
+        {"CONF_NAME": "CONFIG_TROVE_NOVA_TENANT",
+         "CMD_OPTION": "trove-nova-tenant",
+         "PROMPT": "Enter the tenant for Trove to use to connect to Nova",
+         "OPTION_LIST": [],
+         "VALIDATORS": [validators.validate_not_empty],
+         "DEFAULT_VALUE": "services",
+         "MASK_INPUT": False,
+         "LOOSE_VALIDATION": False,
+         "USE_DEFAULT": True,
+         "NEED_CONFIRM": True,
+         "CONDITION": False},
+
+        {"CONF_NAME": "CONFIG_TROVE_NOVA_PW",
+         "CMD_OPTION": "trove-nova-passwd",
+         "PROMPT": "Enter the password for Trove to use to connect to Nova",
+         "OPTION_LIST": [],
+         "VALIDATORS": [validators.validate_not_empty],
+         "DEFAULT_VALUE": "PW_PLACEHOLDER",  # default is trove pass
+         "PROCESSORS": [process_trove_nova_pw],
+         "MASK_INPUT": True,
+         "LOOSE_VALIDATION": False,
+         "USE_DEFAULT": False,
+         "NEED_CONFIRM": True,
+         "CONDITION": False},
     ]
-    update_params_usage(basedefs.PACKSTACK_DOC, params, sectioned=False)
-    group = {"GROUP_NAME": "SAHARA",
-             "DESCRIPTION": "Sahara Config parameters",
-             "PRE_CONDITION": "CONFIG_SAHARA_INSTALL",
+    update_params_usage(basedefs.PACKSTACK_DOC, parameters, sectioned=False)
+    group = {"GROUP_NAME": "Trove",
+             "DESCRIPTION": "Trove config parameters",
+             "PRE_CONDITION": "CONFIG_TROVE_INSTALL",
              "PRE_CONDITION_MATCH": "y",
              "POST_CONDITION": False,
              "POST_CONDITION_MATCH": True}
-    controller.addGroup(group, params)
+
+    controller.addGroup(group, parameters)
 
 
 def initSequences(controller):
-    conf = controller.CONF
-    if conf["CONFIG_SAHARA_INSTALL"] != 'y':
+    config = controller.CONF
+    if config['CONFIG_TROVE_INSTALL'] != 'y':
         return
 
-    saharasteps = [
-        {"title": "Preparing Sahara entries",
-         "functions": [create_manifest]},
+    steps = [
+        {'title': 'Preparing Trove entries',
+         'functions': [create_manifest]}
     ]
-    controller.addSequence("Installing Sahara", [], [], saharasteps)
 
+    controller.addSequence("Installing Trove", [], [], steps)
 
-# -------------------------- step functions --------------------------
-def create_manifest(config, messages):
-    if config['CONFIG_UNSUPPORTED'] != 'y':
-        config['CONFIG_SAHARA_HOST'] = config['CONFIG_CONTROLLER_HOST']
 
+# ------------------------ step functions --------------------------
+def create_manifest(config, messages):
     if config['CONFIG_AMQP_ENABLE_SSL'] == 'y':
-        ssl_host = config['CONFIG_SAHARA_HOST']
-        ssl_cert_file = config['CONFIG_SAHARA_SSL_CERT'] = (
-            '/etc/pki/tls/certs/ssl_amqp_sahara.crt'
+        ssl_cert_file = config['CONFIG_TROVE_SSL_CERT'] = (
+            '/etc/pki/tls/certs/ssl_amqp_trove.crt'
         )
-        ssl_key_file = config['CONFIG_SAHARA_SSL_KEY'] = (
-            '/etc/pki/tls/private/ssl_amqp_sahara.key'
+        ssl_key_file = config['CONFIG_TROVE_SSL_KEY'] = (
+            '/etc/pki/tls/private/ssl_amqp_trove.key'
         )
-        service = 'sahara'
+        ssl_host = config['CONFIG_CONTROLLER_HOST']
+        service = 'trove'
         generate_ssl_cert(config, ssl_host, service, ssl_key_file,
                           ssl_cert_file)
 
+    if (config['CONFIG_TROVE_NOVA_USER'] == 'trove' and
+            config['CONFIG_TROVE_NOVA_PW'] == ''):
+        config['CONFIG_TROVE_NOVA_PW'] = config['CONFIG_TROVE_KS_PW']
+
     fw_details = dict()
-    key = "sahara-api"
+    key = "trove"
     fw_details.setdefault(key, {})
-    fw_details[key]["host"] = "ALL"
-    fw_details[key]["service_name"] = "sahara api"
-    fw_details[key]["chain"] = "INPUT"
-    fw_details[key]["ports"] = ["8386"]
-    fw_details[key]["proto"] = "tcp"
-    config["FIREWALL_SAHARA_CFN_RULES"] = fw_details
+    fw_details[key]['host'] = "ALL"
+    fw_details[key]['service_name'] = "trove api"
+    fw_details[key]['chain'] = "INPUT"
+    fw_details[key]['ports'] = ['8779']
+    fw_details[key]['proto'] = "tcp"
+    config['FIREWALL_TROVE_API_RULES'] = fw_details
```

### Comparing `packstack-23.0.0.0rc1/packstack/plugins/ssl_001.py` & `packstack-24.0.0.0rc1/packstack/plugins/ssl_001.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/plugins/swift_600.py` & `packstack-24.0.0.0rc1/packstack/plugins/swift_600.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/netns.py` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/lib/facter/netns.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/functions/choose_my_ip.rb` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/functions/choose_my_ip.rb`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/functions/force_interface.rb` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/lib/puppet/parser/functions/force_interface.rb`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/amqp/enable_rabbitmq.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/amqp/enable_rabbitmq.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/amqp.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/amqp.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/aodh/rabbitmq.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/aodh/rabbitmq.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/aodh.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/aodh.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ceilometer/rabbitmq.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ceilometer/rabbitmq.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ceilometer.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ceilometer.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/chrony.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/chrony.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/lvm.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/lvm.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/netapp.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/netapp.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/nfs.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/nfs.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/solidfire.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/backend/solidfire.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/rabbitmq.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder/rabbitmq.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/cinder.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/firewall.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/firewall.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/backend/swift.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/backend/swift.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/ceilometer.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance/ceilometer.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/glance.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/gnocchi.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/gnocchi.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat/cfn.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat/cfn.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat/rabbitmq.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat/rabbitmq.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/heat.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/horizon.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/horizon.pp`

 * *Files 9% similar despite different names*

```diff
@@ -48,18 +48,14 @@
       ensure_packages(['openstack-ironic-ui'], {'ensure' => 'present'})
     }
 
     if lookup('CONFIG_TROVE_INSTALL') == 'y' {
       ensure_packages(['openstack-trove-ui'], {'ensure' => 'present'})
     }
 
-    if lookup('CONFIG_SAHARA_INSTALL') == 'y' {
-      ensure_packages(['openstack-sahara-ui'], {'ensure' => 'present'})
-    }
-
     if lookup('CONFIG_HEAT_INSTALL') == 'y' {
       ensure_packages(['openstack-heat-ui'], {'ensure' => 'present'})
     }
 
     include packstack::memcached
 
     $firewall_port = lookup('CONFIG_HORIZON_PORT')
```

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ironic/rabbitmq.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/ironic/rabbitmq.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/cinder.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/cinder.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/heat.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/heat.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/magnum.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/magnum.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/manila.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/manila.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/placement.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/placement.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/swift.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone/swift.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/keystone.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/magnum/rabbitmq.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/magnum/rabbitmq.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/magnum.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/magnum.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/generic.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/generic.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/glusternfs.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/glusternfs.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/netapp.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/backend/netapp.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/network.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/network.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/rabbitmq.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila/rabbitmq.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/manila.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb/services.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb/services.pp`

 * *Files 1% similar despite different names*

```diff
@@ -104,23 +104,14 @@
           password      => lookup('CONFIG_NOVA_DB_PW'),
           host          => '%',
           allowed_hosts => '%',
           charset       => 'utf8',
         }
     }
 
-    if lookup('CONFIG_SAHARA_INSTALL') == 'y' {
-        class { 'sahara::db::mysql':
-          password      => lookup('CONFIG_SAHARA_DB_PW'),
-          host          => '%',
-          allowed_hosts => '%',
-        }
-
-    }
-
     if lookup('CONFIG_TROVE_INSTALL') == 'y' {
         class { 'trove::db::mysql':
             password      => lookup('CONFIG_TROVE_DB_PW'),
             host          => '%',
             allowed_hosts => '%',
             charset       => 'utf8',
         }
```

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb/services_remote.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb/services_remote.pp`

 * *Files 2% similar despite different names*

```diff
@@ -409,45 +409,14 @@
           provider    => 'mysql',
           require     => [ Remote_database_user['nova@%'],
                           Remote_database['nova_cell0'] ],
         }
 
     }
 
-    if lookup('CONFIG_SAHARA_INSTALL') == 'y' {
-        remote_database { 'sahara':
-          ensure      => 'present',
-          charset     => 'utf8',
-          db_host     => lookup('CONFIG_MARIADB_HOST'),
-          db_user     => lookup('CONFIG_MARIADB_USER'),
-          db_password => lookup('CONFIG_MARIADB_PW'),
-          provider    => 'mysql',
-        }
-
-        $sahara_cfg_sahara_db_pw = lookup('CONFIG_SAHARA_DB_PW')
-
-        remote_database_user { 'sahara@%':
-          password_hash => mysql_password($sahara_cfg_sahara_db_pw),
-          db_host       => lookup('CONFIG_MARIADB_HOST'),
-          db_user       => lookup('CONFIG_MARIADB_USER'),
-          db_password   => lookup('CONFIG_MARIADB_PW'),
-          provider      => 'mysql',
-          require       => Remote_database['sahara'],
-        }
-
-        remote_database_grant { 'sahara@%/sahara':
-          privileges  => 'all',
-          db_host     => lookup('CONFIG_MARIADB_HOST'),
-          db_user     => lookup('CONFIG_MARIADB_USER'),
-          db_password => lookup('CONFIG_MARIADB_PW'),
-          provider    => 'mysql',
-          require     => Remote_database_user['sahara@%'],
-        }
-    }
-
     if lookup('CONFIG_TROVE_INSTALL') == 'y' {
         remote_database { 'trove':
           ensure      => 'present',
           charset     => 'utf8',
           db_host     => lookup('CONFIG_MARIADB_HOST'),
           db_user     => lookup('CONFIG_MARIADB_USER'),
           db_password => lookup('CONFIG_MARIADB_PW'),
```

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/mariadb.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/api.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/api.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/bridge.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/bridge.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/lb_agent.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/lb_agent.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ml2.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ml2.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovn_agent.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovn_agent.pp`

 * *Files 6% similar despite different names*

```diff
@@ -47,9 +47,10 @@
 
     class { 'ovn::controller':
       ovn_remote                => $ovn_southd,
       ovn_bridge_mappings       => $bridge_mappings,
       bridge_interface_mappings => $bridge_uplinks,
       ovn_encap_ip              => force_ip($localip),
       hostname                  => $::fqdn,
+      ovn_cms_options           => 'enable-chassis-as-gw',
     }
 }
```

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovn_metadata.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovn_metadata.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovs_agent.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/ovs_agent.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/rabbitmq.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/neutron/rabbitmq.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/api.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/api.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/ceilometer/rabbitmq.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/ceilometer/rabbitmq.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute/libvirt.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute/libvirt.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/compute.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/neutron.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova/neutron.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/nova.pp`

 * *Files 4% similar despite different names*

```diff
@@ -80,8 +80,16 @@
       ram_allocation_ratio    => lookup('CONFIG_NOVA_SCHED_RAM_ALLOC_RATIO'),
       host                    => $novahost,
       ssl_only                => $ssl_only,
       cert                    => $cert,
       key                     => $key,
     }
 
+    $admin_password = lookup('CONFIG_NOVA_KS_PW')
+
+    class { 'nova::keystone::service_user':
+      send_service_user_token => true,
+      password                => $admin_password,
+      auth_url                => lookup('CONFIG_KEYSTONE_ADMIN_URL'),
+    }
+
 }
```

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/openstackclient.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/openstackclient.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/placement.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/placement.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/bridge.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/bridge.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/glance.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/glance.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/tempest.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision/tempest.pp`

 * *Files 5% similar despite different names*

```diff
@@ -85,15 +85,14 @@
     $glance_available     = str2bool(lookup('CONFIG_GLANCE_INSTALL'))
     $horizon_available    = str2bool(lookup('CONFIG_HORIZON_INSTALL'))
     $nova_available       = str2bool(lookup('CONFIG_NOVA_INSTALL'))
     $neutron_available    = str2bool(lookup('CONFIG_NEUTRON_INSTALL'))
     $ceilometer_available = str2bool(lookup('CONFIG_CEILOMETER_INSTALL'))
     $aodh_available       = str2bool(lookup('CONFIG_AODH_INSTALL'))
     $trove_available      = str2bool(lookup('CONFIG_TROVE_INSTALL'))
-    $sahara_available     = str2bool(lookup('CONFIG_SAHARA_INSTALL'))
     $heat_available       = str2bool(lookup('CONFIG_HEAT_INSTALL'))
     $swift_available      = str2bool(lookup('CONFIG_SWIFT_INSTALL'))
     $configure_tempest    = str2bool(lookup('CONFIG_PROVISION_TEMPEST'))
 
     # Some API extensions as l3_agent_scheduler are not enabled by OVN plugin
     $l2_agent  = lookup('CONFIG_NEUTRON_L2_AGENT')
     if $l2_agent == 'ovn' {
@@ -139,15 +138,14 @@
       log_file                  => $log_file,
       neutron_available         => $neutron_available,
       nova_available            => $nova_available,
       password                  => $password,
       public_network_name       => $public_network_name,
       public_router_id          => $public_router_id,
       resize_available          => $resize_available,
-      sahara_available          => $sahara_available,
       ssh_key_type              => $ssh_key_type,
       swift_available           => $swift_available,
       tempest_workspace         => $tempest_workspace,
       install_from_source       => false,
       project_name              => $project_name,
       trove_available           => $trove_available,
       username                  => $username,
```

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/provision.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/ceilometer.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/ceilometer.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/proxy.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/proxy.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/ringbuilder.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/ringbuilder.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/storage.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/swift/storage.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/trove/rabbitmq.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/trove/rabbitmq.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/manifests/trove.pp` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/manifests/trove.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/spec/unit/puppet/parser/functions/choose_my_ip_spec.rb` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/spec/unit/puppet/parser/functions/choose_my_ip_spec.rb`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/modules/packstack/templates/ssl/generate_ssl_certs.sh.erb` & `packstack-24.0.0.0rc1/packstack/puppet/modules/packstack/templates/ssl/generate_ssl_certs.sh.erb`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/templates/compute.pp` & `packstack-24.0.0.0rc1/packstack/puppet/templates/compute.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/templates/controller.pp` & `packstack-24.0.0.0rc1/packstack/puppet/templates/controller.pp`

 * *Files 1% similar despite different names*

```diff
@@ -185,16 +185,7 @@
 }
 
 if lookup('CONFIG_TROVE_INSTALL') == 'y' {
   include 'packstack::keystone::trove'
   include 'packstack::trove::rabbitmq'
   include 'packstack::trove'
 }
-
-if lookup('CONFIG_SAHARA_INSTALL') == 'y' {
-  include 'packstack::keystone::sahara'
-  include 'packstack::sahara::rabbitmq'
-  include 'packstack::sahara'
-  if lookup('CONFIG_CEILOMETER_INSTALL') == 'y' {
-    include 'packstack::sahara::ceilometer'
-  }
-}
```

### Comparing `packstack-23.0.0.0rc1/packstack/puppet/templates/network.pp` & `packstack-24.0.0.0rc1/packstack/puppet/templates/network.pp`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack/version.py` & `packstack-24.0.0.0rc1/packstack/version.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/packstack.egg-info/PKG-INFO` & `packstack-24.0.0.0rc1/packstack.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packstack
-Version: 23.0.0.0rc1
+Version: 24.0.0.0rc1
 Summary: A utility to install OpenStack
 Home-page: http://www.rdoproject.org/
 Author: RDO
 Author-email: rdo-list@redhat.com
 License: UNKNOWN
 Description: Packstack
         =========
@@ -254,15 +254,14 @@
         vpnaas                                            
         cinder         X           X                      
         ceilometer     X                                   X
         aodh           X                                   X
         gnocchi        X                                   X
         heat                                               X
         swift          X                       X          
-        sahara                                 X          
         trove                                  X          
         horizon                    X                      
         manila                     X                      
         SSL                        X                      
         ============== =========== =========== =========== ===========
         
         To run these tests:
@@ -290,14 +289,20 @@
         
         ::
         
            <setup your own custom repositories here>
            export MANAGE_REPOS="false"
            ./run_tests.sh
         
+        Reporting Bugs
+        --------------
+        
+        Bugs for packstack are tracked in the "packstack" component of the [RDO Jira board](https://issues.redhat.com/issues/?jql=project+%3D+RDO+AND+component+%3D+packstack).
+        If you find issues, you can create an issue on that board and provide the relevant information to describe your problem.
+        
         
 Platform: UNKNOWN
 Classifier: Environment :: OpenStack
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `packstack-23.0.0.0rc1/packstack.egg-info/SOURCES.txt` & `packstack-24.0.0.0rc1/packstack.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -6,14 +6,16 @@
 Gemfile
 LICENSE
 MANIFEST.in
 Puppetfile
 README.rst
 Rakefile
 bindep.txt
+external_modules.txt
+openstack_modules.txt
 requirements.txt
 run_tests.sh
 setup.cfg
 setup.py
 test-requirements.txt
 tox.ini
 docs/Makefile
@@ -72,15 +74,14 @@
 packstack/plugins/neutron_350.py
 packstack/plugins/nova_300.py
 packstack/plugins/openstack_client_400.py
 packstack/plugins/postscript_951.py
 packstack/plugins/prescript_000.py
 packstack/plugins/provision_700.py
 packstack/plugins/puppet_950.py
-packstack/plugins/sahara_900.py
 packstack/plugins/ssl_001.py
 packstack/plugins/swift_600.py
 packstack/plugins/trove_850.py
 packstack/puppet/modules/packstack/Gemfile
 packstack/puppet/modules/packstack/Rakefile
 packstack/puppet/modules/packstack/lib/facter/default_hypervisor.rb
 packstack/puppet/modules/packstack/lib/facter/home_dir.rb
@@ -112,15 +113,14 @@
 packstack/puppet/modules/packstack/manifests/neutron.pp
 packstack/puppet/modules/packstack/manifests/nova.pp
 packstack/puppet/modules/packstack/manifests/openstackclient.pp
 packstack/puppet/modules/packstack/manifests/placement.pp
 packstack/puppet/modules/packstack/manifests/prereqs.pp
 packstack/puppet/modules/packstack/manifests/provision.pp
 packstack/puppet/modules/packstack/manifests/redis.pp
-packstack/puppet/modules/packstack/manifests/sahara.pp
 packstack/puppet/modules/packstack/manifests/swift.pp
 packstack/puppet/modules/packstack/manifests/trove.pp
 packstack/puppet/modules/packstack/manifests/amqp/enable_rabbitmq.pp
 packstack/puppet/modules/packstack/manifests/aodh/rabbitmq.pp
 packstack/puppet/modules/packstack/manifests/ceilometer/nova_disabled.pp
 packstack/puppet/modules/packstack/manifests/ceilometer/rabbitmq.pp
 packstack/puppet/modules/packstack/manifests/cinder/backup.pp
@@ -144,15 +144,14 @@
 packstack/puppet/modules/packstack/manifests/keystone/heat.pp
 packstack/puppet/modules/packstack/manifests/keystone/ironic.pp
 packstack/puppet/modules/packstack/manifests/keystone/magnum.pp
 packstack/puppet/modules/packstack/manifests/keystone/manila.pp
 packstack/puppet/modules/packstack/manifests/keystone/neutron.pp
 packstack/puppet/modules/packstack/manifests/keystone/nova.pp
 packstack/puppet/modules/packstack/manifests/keystone/placement.pp
-packstack/puppet/modules/packstack/manifests/keystone/sahara.pp
 packstack/puppet/modules/packstack/manifests/keystone/swift.pp
 packstack/puppet/modules/packstack/manifests/keystone/trove.pp
 packstack/puppet/modules/packstack/manifests/magnum/rabbitmq.pp
 packstack/puppet/modules/packstack/manifests/manila/network.pp
 packstack/puppet/modules/packstack/manifests/manila/rabbitmq.pp
 packstack/puppet/modules/packstack/manifests/manila/backend/generic.pp
 packstack/puppet/modules/packstack/manifests/manila/backend/glusternative.pp
@@ -191,16 +190,14 @@
 packstack/puppet/modules/packstack/manifests/nova/compute/ironic.pp
 packstack/puppet/modules/packstack/manifests/nova/compute/libvirt.pp
 packstack/puppet/modules/packstack/manifests/nova/compute/vmware.pp
 packstack/puppet/modules/packstack/manifests/nova/sched/ironic.pp
 packstack/puppet/modules/packstack/manifests/provision/bridge.pp
 packstack/puppet/modules/packstack/manifests/provision/glance.pp
 packstack/puppet/modules/packstack/manifests/provision/tempest.pp
-packstack/puppet/modules/packstack/manifests/sahara/ceilometer.pp
-packstack/puppet/modules/packstack/manifests/sahara/rabbitmq.pp
 packstack/puppet/modules/packstack/manifests/swift/ceilometer.pp
 packstack/puppet/modules/packstack/manifests/swift/fs.pp
 packstack/puppet/modules/packstack/manifests/swift/proxy.pp
 packstack/puppet/modules/packstack/manifests/swift/ringbuilder.pp
 packstack/puppet/modules/packstack/manifests/swift/storage.pp
 packstack/puppet/modules/packstack/manifests/trove/rabbitmq.pp
 packstack/puppet/modules/packstack/spec/spec_helper.rb
@@ -265,14 +262,15 @@
 releasenotes/notes/remove-epel-support-3732f53a2e45d64c.yaml
 releasenotes/notes/remove-glance-registry-6076539ab6ce1a8b.yaml
 releasenotes/notes/remove-lbaas-0054d83972c5afcf.yaml
 releasenotes/notes/remove-legacy-nova-filters-d6e21a5e8f5c31a7.yaml
 releasenotes/notes/remove-nagios-deployment-21362a84a3ac446f.yaml
 releasenotes/notes/remove-nova-network-8fe352ac6eb22ecb.yaml
 releasenotes/notes/remove-retry-filter-nova-05e84f3fd020d8ed.yaml
+releasenotes/notes/remove-sahara-79e02a209c7128e9.yaml
 releasenotes/notes/remove-uec-images-d876bd8c805d9633.yaml
 releasenotes/notes/renamed-ssl-subject-parameters-c2a52d17c349a59f.yaml
 releasenotes/notes/reno-for-release-notes-66c17b84c946591f.yaml
 releasenotes/notes/service-workers-and-mariadb-c2a6ba903f36b57e.yaml
 releasenotes/notes/swift-s3-removal-ee3ddc2ee21a56cf.yaml
 releasenotes/notes/switch-default-neutron-driver-to-ovn-0eb7053b81c7794d.yaml
 releasenotes/notes/update-puppet-module-usage-4ed869e87e67caaf.yaml
```

### Comparing `packstack-23.0.0.0rc1/playbooks/packstack-multinode.yaml` & `packstack-24.0.0.0rc1/playbooks/packstack-multinode.yaml`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/releasenotes/notes/add-parameter-messages-47d9cf6996f58230.yaml` & `packstack-24.0.0.0rc1/releasenotes/notes/add-parameter-messages-47d9cf6996f58230.yaml`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/releasenotes/notes/add-support-to-ovn-networking-ae6e0176270265c6.yaml` & `packstack-24.0.0.0rc1/releasenotes/notes/add-support-to-ovn-networking-ae6e0176270265c6.yaml`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/releasenotes/notes/integration-tests-d5f86a29cc037329.yaml` & `packstack-24.0.0.0rc1/releasenotes/notes/integration-tests-d5f86a29cc037329.yaml`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/releasenotes/notes/l3-agent-multiple-networks-9d1837c4187055be.yaml` & `packstack-24.0.0.0rc1/releasenotes/notes/l3-agent-multiple-networks-9d1837c4187055be.yaml`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/releasenotes/notes/manifest-execution-refactor-418c27bbc03df064.yaml` & `packstack-24.0.0.0rc1/releasenotes/notes/manifest-execution-refactor-418c27bbc03df064.yaml`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/releasenotes/notes/remove-nova-network-8fe352ac6eb22ecb.yaml` & `packstack-24.0.0.0rc1/releasenotes/notes/remove-nova-network-8fe352ac6eb22ecb.yaml`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/releasenotes/notes/renamed-ssl-subject-parameters-c2a52d17c349a59f.yaml` & `packstack-24.0.0.0rc1/releasenotes/notes/renamed-ssl-subject-parameters-c2a52d17c349a59f.yaml`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/releasenotes/source/conf.py` & `packstack-24.0.0.0rc1/releasenotes/source/conf.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/run_tests.sh` & `packstack-24.0.0.0rc1/run_tests.sh`

 * *Files 6% similar despite different names*

```diff
@@ -172,43 +172,32 @@
                      subversion \
                      systemtap
 
 # Some dependencies are not installed on RHEL/CentOS 8, or are renamed
 OS_NAME=$(facter operatingsystem)
 OS_VERSION=$(facter operatingsystemmajrelease)
 
-if ([ "$OS_NAME" = "RedHat" ] || [ "$OS_NAME" = "CentOS" ]) && [ $OS_VERSION -gt 7 ]; then
-    $SUDO $PKG_MGR -y install python3-setuptools \
-                              python3-devel \
-                              python3-wheel \
-                              python3-pyyaml
-else
-    $SUDO $PKG_MGR -y install python-setuptools \
-                              python-devel \
-                              yum-plugin-priorities
-fi
+$SUDO $PKG_MGR -y install python3-setuptools \
+                          python3-devel \
+                          python3-wheel \
+                          python3-pyyaml
 
 # Don't assume pip is installed
 which pip3 && PIP=pip3
 if [ -z $PIP ]; then
-    if ([ "$OS_NAME" = "RedHat" ] || [ "$OS_NAME" = "CentOS" ]) && [ $OS_VERSION -gt 7 ]; then
-        $SUDO $PKG_MGR -y install python3-pip python3-wheel
-        PIP=pip3
-    else
-        which pip || $SUDO easy_install pip
-        PIP=pip
-    fi
+    $SUDO $PKG_MGR -y install python3-pip python3-wheel
+    PIP=pip3
 fi
 
 # Try to use pre-cached cirros images, if available, otherwise download them
 rm -rf /tmp/cirros
 mkdir /tmp/cirros
 
 export CIRROS_ARCH="$(uname -p)"
-export CIRROS_VERSION="0.5.1"
+export CIRROS_VERSION=${CIRROS_VERSION:-"0.6.2"}
 
 if [ -f ~/cache/files/cirros-$CIRROS_VERSION-$CIRROS_ARCH-uec.tar.gz ]; then
     tar -xzvf ~/cache/files/cirros-$CIRROS_VERSION-$CIRROS_ARCH-uec.tar.gz -C /tmp/cirros/
 else
     echo "No pre-cached uec archive found, downloading..."
     curl -Lo /tmp/cirros/cirros-$CIRROS_VERSION-$CIRROS_ARCH-uec.tar.gz --retry 10 https://download.cirros-cloud.net/$CIRROS_VERSION/cirros-$CIRROS_VERSION-$CIRROS_ARCH-uec.tar.gz
     tar -xzvf /tmp/cirros/cirros-$CIRROS_VERSION-$CIRROS_ARCH-uec.tar.gz -C /tmp/cirros/
@@ -278,20 +267,15 @@
   if [ "${PKG_MGR}" = "dnf" ]; then
       export GEM_BIN_DIR=/usr/local/bin/
   else
       export GEM_BIN_DIR=/tmp/packstackgems/bin/
   fi
   export PUPPETFILE_DIR=/usr/share/openstack-puppet/modules
   export GEM_HOME=/tmp/packstackgems
-  if ([ "$OS_NAME" = "RedHat" ] || [ "$OS_NAME" = "CentOS" ]) && [ $OS_VERSION -gt 8 ]; then
-      $SUDO gem install r10k
-  else
-      $SUDO gem install gettext -v 3.2.9 --no-ri --no-rdoc
-      $SUDO gem install r10k -v 2.6.4 --no-ri --no-rdoc
-  fi
+  $SUDO gem install r10k
   # make sure there is no puppet module pre-installed
   $SUDO rm -rf "${PUPPETFILE_DIR:?}/"*
   install_modules
 else
   $SUDO $PKG_MGR -y install openstack-packstack
 fi
```

### Comparing `packstack-23.0.0.0rc1/setup.cfg` & `packstack-24.0.0.0rc1/setup.cfg`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/tests/installer/test_arch.py` & `packstack-24.0.0.0rc1/tests/installer/test_arch.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/tests/installer/test_drones.py` & `packstack-24.0.0.0rc1/tests/installer/test_drones.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/tests/installer/test_processors.py` & `packstack-24.0.0.0rc1/tests/installer/test_processors.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/tests/installer/test_run_setup.py` & `packstack-24.0.0.0rc1/tests/installer/test_run_setup.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/tests/installer/test_sequences.py` & `packstack-24.0.0.0rc1/tests/installer/test_sequences.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/tests/installer/test_setup_params.py` & `packstack-24.0.0.0rc1/tests/installer/test_setup_params.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/tests/installer/test_utils.py` & `packstack-24.0.0.0rc1/tests/installer/test_utils.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/tests/installer/test_validators.py` & `packstack-24.0.0.0rc1/tests/installer/test_validators.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/tests/modules/test_ospluginutils.py` & `packstack-24.0.0.0rc1/tests/modules/test_ospluginutils.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/tests/modules/test_puppet.py` & `packstack-24.0.0.0rc1/tests/modules/test_puppet.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/tests/scenario-py3.sh` & `packstack-24.0.0.0rc1/tests/scenario-py3.sh`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/tests/scenario001.sh` & `packstack-24.0.0.0rc1/tests/scenario001.sh`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/tests/scenario002.sh` & `packstack-24.0.0.0rc1/tests/scenario002.sh`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,14 @@
 
 echo -e "Generating packstack config for:
 - keystone
 - glance (swift backend)
 - nova
 - neutron (ovs+vxlan)
 - swift
-- sahara
 - trove
 - tempest (regex: 'smoke dashboard')"
 echo "tempest will run if packstack's installation completes successfully."
 echo
 
 if [ -z $COMPUTE_NODE ]; then
   NODE_FLAGS="--allinone"
@@ -35,15 +34,14 @@
           --os-cinder-install=n \
           --os-horizon-install=n \
           --glance-backend=swift \
           --os-neutron-l2-agent=openvswitch \
           --os-neutron-ml2-type-drivers="vxlan,flat" \
           --os-neutron-ml2-tenant-network-types="vxlan" \
           --os-neutron-vpnaas-install=n \
-          --os-sahara-install=y \
           --os-trove-install=y \
           --nova-libvirt-virt-type=qemu \
           --provision-image-url="/tmp/cirros/cirros-$CIRROS_VERSION-$CIRROS_ARCH-disk.img" \
           --provision-demo=y \
           --provision-tempest=y \
           --run-tempest=y \
           --run-tempest-tests="smoke" || export FAILURE=true
```

### Comparing `packstack-23.0.0.0rc1/tests/scenario003.sh` & `packstack-24.0.0.0rc1/tests/scenario003.sh`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/tests/test_base.py` & `packstack-24.0.0.0rc1/tests/test_base.py`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/tools/copy-logs.sh` & `packstack-24.0.0.0rc1/tools/copy-logs.sh`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/tools/fix_disk_layout.sh` & `packstack-24.0.0.0rc1/tools/fix_disk_layout.sh`

 * *Files identical despite different names*

### Comparing `packstack-23.0.0.0rc1/tox.ini` & `packstack-24.0.0.0rc1/tox.ini`

 * *Files identical despite different names*

