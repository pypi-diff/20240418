# Comparing `tmp/socket.d-2.4.10.3.tar.gz` & `tmp/socket.d-2.4.10.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socket.d-2.4.10.3.tar", last modified: Thu Apr 18 05:14:10 2024, max compression
+gzip compressed data, was "socket.d-2.4.10.4.tar", last modified: Thu Apr 18 05:21:32 2024, max compression
```

## Comparing `socket.d-2.4.10.3.tar` & `socket.d-2.4.10.4.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:14:10.051449 socket.d-2.4.10.3/
--rw-r--r--   0 noear      (501) staff       (20)      582 2024-04-18 05:14:10.050717 socket.d-2.4.10.3/PKG-INFO
--rw-r--r--   0 noear      (501) staff       (20)     1713 2024-04-18 04:06:21.000000 socket.d-2.4.10.3/README.md
--rw-r--r--   0 noear      (501) staff       (20)       38 2024-04-18 05:14:10.051659 socket.d-2.4.10.3/setup.cfg
--rw-r--r--   0 noear      (501) staff       (20)      946 2024-04-18 05:14:03.000000 socket.d-2.4.10.3/setup.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:14:10.049718 socket.d-2.4.10.3/socket.d.egg-info/
--rw-r--r--   0 noear      (501) staff       (20)      582 2024-04-18 05:14:09.000000 socket.d-2.4.10.3/socket.d.egg-info/PKG-INFO
--rw-r--r--   0 noear      (501) staff       (20)     4922 2024-04-18 05:14:09.000000 socket.d-2.4.10.3/socket.d.egg-info/SOURCES.txt
--rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-18 05:14:09.000000 socket.d-2.4.10.3/socket.d.egg-info/dependency_links.txt
--rw-r--r--   0 noear      (501) staff       (20)       18 2024-04-18 05:14:09.000000 socket.d-2.4.10.3/socket.d.egg-info/requires.txt
--rw-r--r--   0 noear      (501) staff       (20)       42 2024-04-18 05:14:09.000000 socket.d-2.4.10.3/socket.d.egg-info/top_level.txt
--rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-18 05:14:09.000000 socket.d-2.4.10.3/socket.d.egg-info/zip-safe
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:14:09.982936 socket.d-2.4.10.3/socketd/
--rw-r--r--   0 noear      (501) staff       (20)     4162 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/SocketD.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:14:09.984654 socket.d-2.4.10.3/socketd/broker/
--rw-r--r--   0 noear      (501) staff       (20)      243 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/broker/BrokerFragmentHandler.py
--rw-r--r--   0 noear      (501) staff       (20)     3571 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/broker/BrokerListener.py
--rw-r--r--   0 noear      (501) staff       (20)     3128 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/broker/BrokerListenerBase.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/broker/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:14:09.986018 socket.d-2.4.10.3/socketd/cluster/
--rw-r--r--   0 noear      (501) staff       (20)     2757 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/cluster/ClusterClient.py
--rw-r--r--   0 noear      (501) staff       (20)     2697 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/cluster/ClusterClientSession.py
--rw-r--r--   0 noear      (501) staff       (20)     2002 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/cluster/LoadBalancer.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/cluster/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:14:09.986568 socket.d-2.4.10.3/socketd/exception/
--rw-r--r--   0 noear      (501) staff       (20)      654 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/exception/SocketDExecption.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/exception/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:14:09.986815 socket.d-2.4.10.3/socketd/transport/
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:14:09.992881 socket.d-2.4.10.3/socketd/transport/client/
--rw-r--r--   0 noear      (501) staff       (20)     1720 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/client/Client.py
--rw-r--r--   0 noear      (501) staff       (20)     3585 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/client/ClientBase.py
--rw-r--r--   0 noear      (501) staff       (20)     6510 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/client/ClientChannel.py
--rw-r--r--   0 noear      (501) staff       (20)     2843 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/client/ClientConfig.py
--rw-r--r--   0 noear      (501) staff       (20)      144 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/client/ClientConfigHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      384 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/client/ClientConnectHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      483 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/client/ClientConnector.py
--rw-r--r--   0 noear      (501) staff       (20)      462 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/client/ClientConnectorBase.py
--rw-r--r--   0 noear      (501) staff       (20)      373 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/client/ClientHandshakeResult.py
--rw-r--r--   0 noear      (501) staff       (20)      224 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/client/ClientHeartbeatHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      303 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/client/ClientProvider.py
--rw-r--r--   0 noear      (501) staff       (20)     1126 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/client/ClientSession.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/client/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:14:10.006200 socket.d-2.4.10.3/socketd/transport/core/
--rw-r--r--   0 noear      (501) staff       (20)     1426 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/Asserts.py
--rw-r--r--   0 noear      (501) staff       (20)     2476 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/Channel.py
--rw-r--r--   0 noear      (501) staff       (20)      688 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/ChannelAssistant.py
--rw-r--r--   0 noear      (501) staff       (20)      625 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/ChannelInternal.py
--rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/ChannelSupporter.py
--rw-r--r--   0 noear      (501) staff       (20)     1294 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/Codec.py
--rw-r--r--   0 noear      (501) staff       (20)     2978 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/Config.py
--rw-r--r--   0 noear      (501) staff       (20)     1262 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/Costants.py
--rw-r--r--   0 noear      (501) staff       (20)     1148 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/Entity.py
--rw-r--r--   0 noear      (501) staff       (20)      697 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/EntityMetas.py
--rw-r--r--   0 noear      (501) staff       (20)     1717 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/Flags.py
--rw-r--r--   0 noear      (501) staff       (20)     1154 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/FragmentAggregator.py
--rw-r--r--   0 noear      (501) staff       (20)      838 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/FragmentHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      419 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/Frame.py
--rw-r--r--   0 noear      (501) staff       (20)     2290 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/Frames.py
--rw-r--r--   0 noear      (501) staff       (20)     2531 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/HandshakeDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      167 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/IdGenerator.py
--rw-r--r--   0 noear      (501) staff       (20)      504 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/Listener.py
--rw-r--r--   0 noear      (501) staff       (20)      735 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/Message.py
--rw-r--r--   0 noear      (501) staff       (20)      801 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/Processor.py
--rw-r--r--   0 noear      (501) staff       (20)     1953 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/Session.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:14:10.010362 socket.d-2.4.10.3/socketd/transport/core/codec/
--rw-r--r--   0 noear      (501) staff       (20)     1164 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/codec/Buffer.py
--rw-r--r--   0 noear      (501) staff       (20)      780 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/codec/ByteBufferCodecReader.py
--rw-r--r--   0 noear      (501) staff       (20)      642 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/codec/ByteBufferCodecWriter.py
--rw-r--r--   0 noear      (501) staff       (20)     4514 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/codec/CodecDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      200 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/codec/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:14:10.014491 socket.d-2.4.10.3/socketd/transport/core/entity/
--rw-r--r--   0 noear      (501) staff       (20)     3783 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/entity/EntityDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      839 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/entity/FileEntity.py
--rw-r--r--   0 noear      (501) staff       (20)      885 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/entity/MessageBuilder.py
--rw-r--r--   0 noear      (501) staff       (20)     2045 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/entity/MessageDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      215 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/entity/StringEntity.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/entity/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:14:10.019260 socket.d-2.4.10.3/socketd/transport/core/fragment/
--rw-r--r--   0 noear      (501) staff       (20)     2007 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/fragment/FragmentAggregatorDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     3377 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/fragment/FragmentHandlerBase.py
--rw-r--r--   0 noear      (501) staff       (20)      502 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/fragment/FragmentHandlerDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      188 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/fragment/FragmentHolder.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/fragment/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:14:10.023444 socket.d-2.4.10.3/socketd/transport/core/impl/
--rw-r--r--   0 noear      (501) staff       (20)     2358 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/impl/ChannelBase.py
--rw-r--r--   0 noear      (501) staff       (20)     6906 2024-04-18 04:06:21.000000 socket.d-2.4.10.3/socketd/transport/core/impl/ChannelDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     6579 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/impl/ConfigBase.py
--rw-r--r--   0 noear      (501) staff       (20)      282 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/impl/LogConfig.py
--rw-r--r--   0 noear      (501) staff       (20)     7748 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/impl/ProcessorDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/impl/SessionBase.py
--rw-r--r--   0 noear      (501) staff       (20)     4288 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/impl/SessionDefault.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/impl/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:14:10.027449 socket.d-2.4.10.3/socketd/transport/core/listener/
--rw-r--r--   0 noear      (501) staff       (20)     2323 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/listener/EventListener.py
--rw-r--r--   0 noear      (501) staff       (20)     1043 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/listener/PathListener.py
--rw-r--r--   0 noear      (501) staff       (20)      176 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/listener/PathMapper.py
--rw-r--r--   0 noear      (501) staff       (20)      457 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/listener/PipelineListener.py
--rw-r--r--   0 noear      (501) staff       (20)      457 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/listener/SimpleListener.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/core/listener/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:14:10.030231 socket.d-2.4.10.3/socketd/transport/server/
--rw-r--r--   0 noear      (501) staff       (20)      608 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/server/Server.py
--rw-r--r--   0 noear      (501) staff       (20)     2437 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/server/ServerBase.py
--rw-r--r--   0 noear      (501) staff       (20)     1645 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/server/ServerConfig.py
--rw-r--r--   0 noear      (501) staff       (20)      250 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/server/ServerProvider.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/server/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:14:10.033843 socket.d-2.4.10.3/socketd/transport/stream/
--rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/stream/RequestStream.py
--rw-r--r--   0 noear      (501) staff       (20)      332 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/stream/SendStream.py
--rw-r--r--   0 noear      (501) staff       (20)      690 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/stream/Stream.py
--rw-r--r--   0 noear      (501) staff       (20)     2100 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/stream/StreamBase.py
--rw-r--r--   0 noear      (501) staff       (20)      907 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/stream/StreamManger.py
--rw-r--r--   0 noear      (501) staff       (20)     1025 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/stream/StreamMangerDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      843 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/stream/SubscribeStream.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/stream/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:14:10.035600 socket.d-2.4.10.3/socketd/transport/utils/
--rw-r--r--   0 noear      (501) staff       (20)     3488 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/utils/AsyncUtil.py
--rw-r--r--   0 noear      (501) staff       (20)     1989 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/utils/CompletableFuture.py
--rw-r--r--   0 noear      (501) staff       (20)      662 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/utils/StrUtil.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/utils/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:14:10.036171 socket.d-2.4.10.3/socketd/transport/utils/async_api/
--rw-r--r--   0 noear      (501) staff       (20)      787 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/utils/async_api/AtomicRefer.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/utils/async_api/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:14:10.037067 socket.d-2.4.10.3/socketd/transport/utils/sync_api/
--rw-r--r--   0 noear      (501) staff       (20)      747 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/utils/sync_api/AtomicRefer.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd/transport/utils/sync_api/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:14:10.041587 socket.d-2.4.10.3/socketd_aio_tcp/
--rw-r--r--   0 noear      (501) staff       (20)     4144 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd_aio_tcp/TCPAIOServer.py
--rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd_aio_tcp/TCPStreamIO.py
--rw-r--r--   0 noear      (501) staff       (20)     2331 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd_aio_tcp/TcpAIOChannelAssistant.py
--rw-r--r--   0 noear      (501) staff       (20)      645 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd_aio_tcp/TcpAioClient.py
--rw-r--r--   0 noear      (501) staff       (20)     6614 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd_aio_tcp/TcpAioClientConnector.py
--rw-r--r--   0 noear      (501) staff       (20)      776 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd_aio_tcp/TcpAioProvider.py
--rw-r--r--   0 noear      (501) staff       (20)      183 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd_aio_tcp/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:14:10.045249 socket.d-2.4.10.3/socketd_websocket/
--rw-r--r--   0 noear      (501) staff       (20)     2471 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd_websocket/WsAioChannelAssistant.py
--rw-r--r--   0 noear      (501) staff       (20)      574 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd_websocket/WsAioClient.py
--rw-r--r--   0 noear      (501) staff       (20)     3630 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd_websocket/WsAioClientConnector.py
--rw-r--r--   0 noear      (501) staff       (20)      830 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd_websocket/WsAioProvider.py
--rw-r--r--   0 noear      (501) staff       (20)     2289 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd_websocket/WsAioServer.py
--rw-r--r--   0 noear      (501) staff       (20)      117 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd_websocket/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:14:10.048897 socket.d-2.4.10.3/socketd_websocket/impl/
--rw-r--r--   0 noear      (501) staff       (20)     4784 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd_websocket/impl/AIOConnect.py
--rw-r--r--   0 noear      (501) staff       (20)     6180 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd_websocket/impl/AIOServe.py
--rw-r--r--   0 noear      (501) staff       (20)     5946 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd_websocket/impl/AIOWebSocketClientImpl.py
--rw-r--r--   0 noear      (501) staff       (20)     4602 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd_websocket/impl/AIOWebSocketServerImpl.py
--rw-r--r--   0 noear      (501) staff       (20)      274 2024-04-18 02:59:52.000000 socket.d-2.4.10.3/socketd_websocket/impl/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.790752 socket.d-2.4.10.4/
+-rw-r--r--   0 noear      (501) staff       (20)      555 2024-04-18 05:21:32.789998 socket.d-2.4.10.4/PKG-INFO
+-rw-r--r--   0 noear      (501) staff       (20)     1713 2024-04-18 04:06:21.000000 socket.d-2.4.10.4/README.md
+-rw-r--r--   0 noear      (501) staff       (20)       38 2024-04-18 05:21:32.790934 socket.d-2.4.10.4/setup.cfg
+-rw-r--r--   0 noear      (501) staff       (20)      875 2024-04-18 05:21:09.000000 socket.d-2.4.10.4/setup.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.788745 socket.d-2.4.10.4/socket.d.egg-info/
+-rw-r--r--   0 noear      (501) staff       (20)      555 2024-04-18 05:21:32.000000 socket.d-2.4.10.4/socket.d.egg-info/PKG-INFO
+-rw-r--r--   0 noear      (501) staff       (20)     4922 2024-04-18 05:21:32.000000 socket.d-2.4.10.4/socket.d.egg-info/SOURCES.txt
+-rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-18 05:21:32.000000 socket.d-2.4.10.4/socket.d.egg-info/dependency_links.txt
+-rw-r--r--   0 noear      (501) staff       (20)       18 2024-04-18 05:21:32.000000 socket.d-2.4.10.4/socket.d.egg-info/requires.txt
+-rw-r--r--   0 noear      (501) staff       (20)       42 2024-04-18 05:21:32.000000 socket.d-2.4.10.4/socket.d.egg-info/top_level.txt
+-rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-18 05:21:32.000000 socket.d-2.4.10.4/socket.d.egg-info/zip-safe
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.669407 socket.d-2.4.10.4/socketd/
+-rw-r--r--   0 noear      (501) staff       (20)     4162 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/SocketD.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.672968 socket.d-2.4.10.4/socketd/broker/
+-rw-r--r--   0 noear      (501) staff       (20)      243 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/broker/BrokerFragmentHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)     3571 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/broker/BrokerListener.py
+-rw-r--r--   0 noear      (501) staff       (20)     3128 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/broker/BrokerListenerBase.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/broker/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.677217 socket.d-2.4.10.4/socketd/cluster/
+-rw-r--r--   0 noear      (501) staff       (20)     2757 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/cluster/ClusterClient.py
+-rw-r--r--   0 noear      (501) staff       (20)     2697 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/cluster/ClusterClientSession.py
+-rw-r--r--   0 noear      (501) staff       (20)     2002 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/cluster/LoadBalancer.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/cluster/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.678622 socket.d-2.4.10.4/socketd/exception/
+-rw-r--r--   0 noear      (501) staff       (20)      654 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/exception/SocketDExecption.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/exception/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.679786 socket.d-2.4.10.4/socketd/transport/
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.711281 socket.d-2.4.10.4/socketd/transport/client/
+-rw-r--r--   0 noear      (501) staff       (20)     1720 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/Client.py
+-rw-r--r--   0 noear      (501) staff       (20)     3585 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/ClientBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     6510 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/ClientChannel.py
+-rw-r--r--   0 noear      (501) staff       (20)     2843 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/ClientConfig.py
+-rw-r--r--   0 noear      (501) staff       (20)      144 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/ClientConfigHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      384 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/ClientConnectHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      483 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/ClientConnector.py
+-rw-r--r--   0 noear      (501) staff       (20)      462 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/ClientConnectorBase.py
+-rw-r--r--   0 noear      (501) staff       (20)      373 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/ClientHandshakeResult.py
+-rw-r--r--   0 noear      (501) staff       (20)      224 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/ClientHeartbeatHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      303 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/ClientProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)     1126 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/ClientSession.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.729392 socket.d-2.4.10.4/socketd/transport/core/
+-rw-r--r--   0 noear      (501) staff       (20)     1426 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Asserts.py
+-rw-r--r--   0 noear      (501) staff       (20)     2476 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Channel.py
+-rw-r--r--   0 noear      (501) staff       (20)      688 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/ChannelAssistant.py
+-rw-r--r--   0 noear      (501) staff       (20)      625 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/ChannelInternal.py
+-rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/ChannelSupporter.py
+-rw-r--r--   0 noear      (501) staff       (20)     1294 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Codec.py
+-rw-r--r--   0 noear      (501) staff       (20)     2978 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Config.py
+-rw-r--r--   0 noear      (501) staff       (20)     1262 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Costants.py
+-rw-r--r--   0 noear      (501) staff       (20)     1148 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Entity.py
+-rw-r--r--   0 noear      (501) staff       (20)      697 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/EntityMetas.py
+-rw-r--r--   0 noear      (501) staff       (20)     1717 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Flags.py
+-rw-r--r--   0 noear      (501) staff       (20)     1154 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/FragmentAggregator.py
+-rw-r--r--   0 noear      (501) staff       (20)      838 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/FragmentHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      419 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Frame.py
+-rw-r--r--   0 noear      (501) staff       (20)     2290 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Frames.py
+-rw-r--r--   0 noear      (501) staff       (20)     2531 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/HandshakeDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      167 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/IdGenerator.py
+-rw-r--r--   0 noear      (501) staff       (20)      504 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Listener.py
+-rw-r--r--   0 noear      (501) staff       (20)      735 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Message.py
+-rw-r--r--   0 noear      (501) staff       (20)      801 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Processor.py
+-rw-r--r--   0 noear      (501) staff       (20)     1953 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Session.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.735278 socket.d-2.4.10.4/socketd/transport/core/codec/
+-rw-r--r--   0 noear      (501) staff       (20)     1164 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/codec/Buffer.py
+-rw-r--r--   0 noear      (501) staff       (20)      780 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/codec/ByteBufferCodecReader.py
+-rw-r--r--   0 noear      (501) staff       (20)      642 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/codec/ByteBufferCodecWriter.py
+-rw-r--r--   0 noear      (501) staff       (20)     4514 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/codec/CodecDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      200 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/codec/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.741684 socket.d-2.4.10.4/socketd/transport/core/entity/
+-rw-r--r--   0 noear      (501) staff       (20)     3783 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/entity/EntityDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      839 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/entity/FileEntity.py
+-rw-r--r--   0 noear      (501) staff       (20)      885 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/entity/MessageBuilder.py
+-rw-r--r--   0 noear      (501) staff       (20)     2045 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/entity/MessageDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      215 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/entity/StringEntity.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/entity/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.743664 socket.d-2.4.10.4/socketd/transport/core/fragment/
+-rw-r--r--   0 noear      (501) staff       (20)     2007 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/fragment/FragmentAggregatorDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     3377 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/fragment/FragmentHandlerBase.py
+-rw-r--r--   0 noear      (501) staff       (20)      502 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/fragment/FragmentHandlerDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      188 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/fragment/FragmentHolder.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/fragment/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.747256 socket.d-2.4.10.4/socketd/transport/core/impl/
+-rw-r--r--   0 noear      (501) staff       (20)     2358 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/impl/ChannelBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     6906 2024-04-18 04:06:21.000000 socket.d-2.4.10.4/socketd/transport/core/impl/ChannelDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     6579 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/impl/ConfigBase.py
+-rw-r--r--   0 noear      (501) staff       (20)      282 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/impl/LogConfig.py
+-rw-r--r--   0 noear      (501) staff       (20)     7748 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/impl/ProcessorDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/impl/SessionBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     4288 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/impl/SessionDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/impl/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.751400 socket.d-2.4.10.4/socketd/transport/core/listener/
+-rw-r--r--   0 noear      (501) staff       (20)     2323 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/listener/EventListener.py
+-rw-r--r--   0 noear      (501) staff       (20)     1043 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/listener/PathListener.py
+-rw-r--r--   0 noear      (501) staff       (20)      176 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/listener/PathMapper.py
+-rw-r--r--   0 noear      (501) staff       (20)      457 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/listener/PipelineListener.py
+-rw-r--r--   0 noear      (501) staff       (20)      457 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/listener/SimpleListener.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/listener/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.754205 socket.d-2.4.10.4/socketd/transport/server/
+-rw-r--r--   0 noear      (501) staff       (20)      608 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/server/Server.py
+-rw-r--r--   0 noear      (501) staff       (20)     2437 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/server/ServerBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     1645 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/server/ServerConfig.py
+-rw-r--r--   0 noear      (501) staff       (20)      250 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/server/ServerProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/server/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.763024 socket.d-2.4.10.4/socketd/transport/stream/
+-rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/stream/RequestStream.py
+-rw-r--r--   0 noear      (501) staff       (20)      332 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/stream/SendStream.py
+-rw-r--r--   0 noear      (501) staff       (20)      690 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/stream/Stream.py
+-rw-r--r--   0 noear      (501) staff       (20)     2100 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/stream/StreamBase.py
+-rw-r--r--   0 noear      (501) staff       (20)      907 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/stream/StreamManger.py
+-rw-r--r--   0 noear      (501) staff       (20)     1025 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/stream/StreamMangerDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      843 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/stream/SubscribeStream.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/stream/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.766704 socket.d-2.4.10.4/socketd/transport/utils/
+-rw-r--r--   0 noear      (501) staff       (20)     3488 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/utils/AsyncUtil.py
+-rw-r--r--   0 noear      (501) staff       (20)     1989 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/utils/CompletableFuture.py
+-rw-r--r--   0 noear      (501) staff       (20)      662 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/utils/StrUtil.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/utils/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.767745 socket.d-2.4.10.4/socketd/transport/utils/async_api/
+-rw-r--r--   0 noear      (501) staff       (20)      787 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/utils/async_api/AtomicRefer.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/utils/async_api/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.768935 socket.d-2.4.10.4/socketd/transport/utils/sync_api/
+-rw-r--r--   0 noear      (501) staff       (20)      747 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/utils/sync_api/AtomicRefer.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/utils/sync_api/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.775990 socket.d-2.4.10.4/socketd_aio_tcp/
+-rw-r--r--   0 noear      (501) staff       (20)     4144 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_aio_tcp/TCPAIOServer.py
+-rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_aio_tcp/TCPStreamIO.py
+-rw-r--r--   0 noear      (501) staff       (20)     2331 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_aio_tcp/TcpAIOChannelAssistant.py
+-rw-r--r--   0 noear      (501) staff       (20)      645 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_aio_tcp/TcpAioClient.py
+-rw-r--r--   0 noear      (501) staff       (20)     6614 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_aio_tcp/TcpAioClientConnector.py
+-rw-r--r--   0 noear      (501) staff       (20)      776 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_aio_tcp/TcpAioProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)      183 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_aio_tcp/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.779747 socket.d-2.4.10.4/socketd_websocket/
+-rw-r--r--   0 noear      (501) staff       (20)     2471 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_websocket/WsAioChannelAssistant.py
+-rw-r--r--   0 noear      (501) staff       (20)      574 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_websocket/WsAioClient.py
+-rw-r--r--   0 noear      (501) staff       (20)     3630 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_websocket/WsAioClientConnector.py
+-rw-r--r--   0 noear      (501) staff       (20)      830 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_websocket/WsAioProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)     2289 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_websocket/WsAioServer.py
+-rw-r--r--   0 noear      (501) staff       (20)      117 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_websocket/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.786897 socket.d-2.4.10.4/socketd_websocket/impl/
+-rw-r--r--   0 noear      (501) staff       (20)     4784 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_websocket/impl/AIOConnect.py
+-rw-r--r--   0 noear      (501) staff       (20)     6180 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_websocket/impl/AIOServe.py
+-rw-r--r--   0 noear      (501) staff       (20)     5946 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_websocket/impl/AIOWebSocketClientImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)     4602 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_websocket/impl/AIOWebSocketServerImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)      274 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_websocket/impl/__init__.py
```

### Comparing `socket.d-2.4.10.3/PKG-INFO` & `socket.d-2.4.10.4/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: socket.d
-Version: 2.4.10.3
-Summary: 基于事件和语义消息流的网络应用层协议。
+Version: 2.4.10.4
+Summary: @noear/socket.d python project
 Home-page: https://socketd.noear.org/
 Author: noear,bai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `socket.d-2.4.10.3/README.md` & `socket.d-2.4.10.4/README.md`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socket.d.egg-info/PKG-INFO` & `socket.d-2.4.10.4/socket.d.egg-info/PKG-INFO`

 * *Files 19% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: socket.d
-Version: 2.4.10.3
-Summary: 基于事件和语义消息流的网络应用层协议。
+Version: 2.4.10.4
+Summary: @noear/socket.d python project
 Home-page: https://socketd.noear.org/
 Author: noear,bai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `socket.d-2.4.10.3/socket.d.egg-info/SOURCES.txt` & `socket.d-2.4.10.4/socket.d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/SocketD.py` & `socket.d-2.4.10.4/socketd/SocketD.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/broker/BrokerListener.py` & `socket.d-2.4.10.4/socketd/broker/BrokerListener.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/broker/BrokerListenerBase.py` & `socket.d-2.4.10.4/socketd/broker/BrokerListenerBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/cluster/ClusterClient.py` & `socket.d-2.4.10.4/socketd/cluster/ClusterClient.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/cluster/ClusterClientSession.py` & `socket.d-2.4.10.4/socketd/cluster/ClusterClientSession.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/cluster/LoadBalancer.py` & `socket.d-2.4.10.4/socketd/cluster/LoadBalancer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/exception/SocketDExecption.py` & `socket.d-2.4.10.4/socketd/exception/SocketDExecption.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/client/Client.py` & `socket.d-2.4.10.4/socketd/transport/client/Client.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/client/ClientBase.py` & `socket.d-2.4.10.4/socketd/transport/client/ClientBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/client/ClientChannel.py` & `socket.d-2.4.10.4/socketd/transport/client/ClientChannel.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/client/ClientConfig.py` & `socket.d-2.4.10.4/socketd/transport/client/ClientConfig.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/client/ClientSession.py` & `socket.d-2.4.10.4/socketd/transport/client/ClientSession.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/Asserts.py` & `socket.d-2.4.10.4/socketd/transport/core/Asserts.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/Channel.py` & `socket.d-2.4.10.4/socketd/transport/core/Channel.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/ChannelAssistant.py` & `socket.d-2.4.10.4/socketd/transport/core/ChannelAssistant.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/ChannelInternal.py` & `socket.d-2.4.10.4/socketd/transport/core/ChannelInternal.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/ChannelSupporter.py` & `socket.d-2.4.10.4/socketd/transport/core/ChannelSupporter.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/Codec.py` & `socket.d-2.4.10.4/socketd/transport/core/Codec.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/Config.py` & `socket.d-2.4.10.4/socketd/transport/core/Config.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/Costants.py` & `socket.d-2.4.10.4/socketd/transport/core/Costants.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/Entity.py` & `socket.d-2.4.10.4/socketd/transport/core/Entity.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/EntityMetas.py` & `socket.d-2.4.10.4/socketd/transport/core/EntityMetas.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/Flags.py` & `socket.d-2.4.10.4/socketd/transport/core/Flags.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/FragmentAggregator.py` & `socket.d-2.4.10.4/socketd/transport/core/FragmentAggregator.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/FragmentHandler.py` & `socket.d-2.4.10.4/socketd/transport/core/FragmentHandler.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/Frames.py` & `socket.d-2.4.10.4/socketd/transport/core/Frames.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/HandshakeDefault.py` & `socket.d-2.4.10.4/socketd/transport/core/HandshakeDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/Message.py` & `socket.d-2.4.10.4/socketd/transport/core/Message.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/Processor.py` & `socket.d-2.4.10.4/socketd/transport/core/Processor.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/Session.py` & `socket.d-2.4.10.4/socketd/transport/core/Session.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/codec/Buffer.py` & `socket.d-2.4.10.4/socketd/transport/core/codec/Buffer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/codec/ByteBufferCodecReader.py` & `socket.d-2.4.10.4/socketd/transport/core/codec/ByteBufferCodecReader.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/codec/ByteBufferCodecWriter.py` & `socket.d-2.4.10.4/socketd/transport/core/codec/ByteBufferCodecWriter.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/codec/CodecDefault.py` & `socket.d-2.4.10.4/socketd/transport/core/codec/CodecDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/entity/EntityDefault.py` & `socket.d-2.4.10.4/socketd/transport/core/entity/EntityDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/entity/FileEntity.py` & `socket.d-2.4.10.4/socketd/transport/core/entity/FileEntity.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/entity/MessageBuilder.py` & `socket.d-2.4.10.4/socketd/transport/core/entity/MessageBuilder.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/entity/MessageDefault.py` & `socket.d-2.4.10.4/socketd/transport/core/entity/MessageDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/fragment/FragmentAggregatorDefault.py` & `socket.d-2.4.10.4/socketd/transport/core/fragment/FragmentAggregatorDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/fragment/FragmentHandlerBase.py` & `socket.d-2.4.10.4/socketd/transport/core/fragment/FragmentHandlerBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/impl/ChannelBase.py` & `socket.d-2.4.10.4/socketd/transport/core/impl/ChannelBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/impl/ChannelDefault.py` & `socket.d-2.4.10.4/socketd/transport/core/impl/ChannelDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/impl/ConfigBase.py` & `socket.d-2.4.10.4/socketd/transport/core/impl/ConfigBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/impl/ProcessorDefault.py` & `socket.d-2.4.10.4/socketd/transport/core/impl/ProcessorDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/impl/SessionBase.py` & `socket.d-2.4.10.4/socketd/transport/core/impl/SessionBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/impl/SessionDefault.py` & `socket.d-2.4.10.4/socketd/transport/core/impl/SessionDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/listener/EventListener.py` & `socket.d-2.4.10.4/socketd/transport/core/listener/EventListener.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/core/listener/PathListener.py` & `socket.d-2.4.10.4/socketd/transport/core/listener/PathListener.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/server/Server.py` & `socket.d-2.4.10.4/socketd/transport/server/Server.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/server/ServerBase.py` & `socket.d-2.4.10.4/socketd/transport/server/ServerBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/server/ServerConfig.py` & `socket.d-2.4.10.4/socketd/transport/server/ServerConfig.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/stream/RequestStream.py` & `socket.d-2.4.10.4/socketd/transport/stream/RequestStream.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/stream/Stream.py` & `socket.d-2.4.10.4/socketd/transport/stream/Stream.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/stream/StreamBase.py` & `socket.d-2.4.10.4/socketd/transport/stream/StreamBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/stream/StreamManger.py` & `socket.d-2.4.10.4/socketd/transport/stream/StreamManger.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/stream/StreamMangerDefault.py` & `socket.d-2.4.10.4/socketd/transport/stream/StreamMangerDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/stream/SubscribeStream.py` & `socket.d-2.4.10.4/socketd/transport/stream/SubscribeStream.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/utils/AsyncUtil.py` & `socket.d-2.4.10.4/socketd/transport/utils/AsyncUtil.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/utils/CompletableFuture.py` & `socket.d-2.4.10.4/socketd/transport/utils/CompletableFuture.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/utils/StrUtil.py` & `socket.d-2.4.10.4/socketd/transport/utils/StrUtil.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/utils/async_api/AtomicRefer.py` & `socket.d-2.4.10.4/socketd/transport/utils/async_api/AtomicRefer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd/transport/utils/sync_api/AtomicRefer.py` & `socket.d-2.4.10.4/socketd/transport/utils/sync_api/AtomicRefer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd_aio_tcp/TCPAIOServer.py` & `socket.d-2.4.10.4/socketd_aio_tcp/TCPAIOServer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd_aio_tcp/TCPStreamIO.py` & `socket.d-2.4.10.4/socketd_aio_tcp/TCPStreamIO.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd_aio_tcp/TcpAIOChannelAssistant.py` & `socket.d-2.4.10.4/socketd_aio_tcp/TcpAIOChannelAssistant.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd_aio_tcp/TcpAioClient.py` & `socket.d-2.4.10.4/socketd_aio_tcp/TcpAioClient.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd_aio_tcp/TcpAioClientConnector.py` & `socket.d-2.4.10.4/socketd_aio_tcp/TcpAioClientConnector.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd_aio_tcp/TcpAioProvider.py` & `socket.d-2.4.10.4/socketd_aio_tcp/TcpAioProvider.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd_websocket/WsAioChannelAssistant.py` & `socket.d-2.4.10.4/socketd_websocket/WsAioChannelAssistant.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd_websocket/WsAioClient.py` & `socket.d-2.4.10.4/socketd_websocket/WsAioClient.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd_websocket/WsAioClientConnector.py` & `socket.d-2.4.10.4/socketd_websocket/WsAioClientConnector.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd_websocket/WsAioProvider.py` & `socket.d-2.4.10.4/socketd_websocket/WsAioProvider.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd_websocket/WsAioServer.py` & `socket.d-2.4.10.4/socketd_websocket/WsAioServer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd_websocket/impl/AIOConnect.py` & `socket.d-2.4.10.4/socketd_websocket/impl/AIOConnect.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd_websocket/impl/AIOServe.py` & `socket.d-2.4.10.4/socketd_websocket/impl/AIOServe.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd_websocket/impl/AIOWebSocketClientImpl.py` & `socket.d-2.4.10.4/socketd_websocket/impl/AIOWebSocketClientImpl.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.3/socketd_websocket/impl/AIOWebSocketServerImpl.py` & `socket.d-2.4.10.4/socketd_websocket/impl/AIOWebSocketServerImpl.py`

 * *Files identical despite different names*

