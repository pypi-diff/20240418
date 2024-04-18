# Comparing `tmp/socket.d-2.4.10.4.tar.gz` & `tmp/socket.d-2.4.10.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "socket.d-2.4.10.4.tar", last modified: Thu Apr 18 05:21:32 2024, max compression
+gzip compressed data, was "socket.d-2.4.10.5.tar", last modified: Thu Apr 18 09:25:08 2024, max compression
```

## Comparing `socket.d-2.4.10.4.tar` & `socket.d-2.4.10.5.tar`

### file list

```diff
@@ -1,149 +1,149 @@
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.790752 socket.d-2.4.10.4/
--rw-r--r--   0 noear      (501) staff       (20)      555 2024-04-18 05:21:32.789998 socket.d-2.4.10.4/PKG-INFO
--rw-r--r--   0 noear      (501) staff       (20)     1713 2024-04-18 04:06:21.000000 socket.d-2.4.10.4/README.md
--rw-r--r--   0 noear      (501) staff       (20)       38 2024-04-18 05:21:32.790934 socket.d-2.4.10.4/setup.cfg
--rw-r--r--   0 noear      (501) staff       (20)      875 2024-04-18 05:21:09.000000 socket.d-2.4.10.4/setup.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.788745 socket.d-2.4.10.4/socket.d.egg-info/
--rw-r--r--   0 noear      (501) staff       (20)      555 2024-04-18 05:21:32.000000 socket.d-2.4.10.4/socket.d.egg-info/PKG-INFO
--rw-r--r--   0 noear      (501) staff       (20)     4922 2024-04-18 05:21:32.000000 socket.d-2.4.10.4/socket.d.egg-info/SOURCES.txt
--rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-18 05:21:32.000000 socket.d-2.4.10.4/socket.d.egg-info/dependency_links.txt
--rw-r--r--   0 noear      (501) staff       (20)       18 2024-04-18 05:21:32.000000 socket.d-2.4.10.4/socket.d.egg-info/requires.txt
--rw-r--r--   0 noear      (501) staff       (20)       42 2024-04-18 05:21:32.000000 socket.d-2.4.10.4/socket.d.egg-info/top_level.txt
--rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-18 05:21:32.000000 socket.d-2.4.10.4/socket.d.egg-info/zip-safe
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.669407 socket.d-2.4.10.4/socketd/
--rw-r--r--   0 noear      (501) staff       (20)     4162 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/SocketD.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.672968 socket.d-2.4.10.4/socketd/broker/
--rw-r--r--   0 noear      (501) staff       (20)      243 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/broker/BrokerFragmentHandler.py
--rw-r--r--   0 noear      (501) staff       (20)     3571 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/broker/BrokerListener.py
--rw-r--r--   0 noear      (501) staff       (20)     3128 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/broker/BrokerListenerBase.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/broker/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.677217 socket.d-2.4.10.4/socketd/cluster/
--rw-r--r--   0 noear      (501) staff       (20)     2757 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/cluster/ClusterClient.py
--rw-r--r--   0 noear      (501) staff       (20)     2697 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/cluster/ClusterClientSession.py
--rw-r--r--   0 noear      (501) staff       (20)     2002 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/cluster/LoadBalancer.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/cluster/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.678622 socket.d-2.4.10.4/socketd/exception/
--rw-r--r--   0 noear      (501) staff       (20)      654 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/exception/SocketDExecption.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/exception/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.679786 socket.d-2.4.10.4/socketd/transport/
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.711281 socket.d-2.4.10.4/socketd/transport/client/
--rw-r--r--   0 noear      (501) staff       (20)     1720 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/Client.py
--rw-r--r--   0 noear      (501) staff       (20)     3585 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/ClientBase.py
--rw-r--r--   0 noear      (501) staff       (20)     6510 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/ClientChannel.py
--rw-r--r--   0 noear      (501) staff       (20)     2843 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/ClientConfig.py
--rw-r--r--   0 noear      (501) staff       (20)      144 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/ClientConfigHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      384 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/ClientConnectHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      483 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/ClientConnector.py
--rw-r--r--   0 noear      (501) staff       (20)      462 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/ClientConnectorBase.py
--rw-r--r--   0 noear      (501) staff       (20)      373 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/ClientHandshakeResult.py
--rw-r--r--   0 noear      (501) staff       (20)      224 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/ClientHeartbeatHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      303 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/ClientProvider.py
--rw-r--r--   0 noear      (501) staff       (20)     1126 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/ClientSession.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/client/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.729392 socket.d-2.4.10.4/socketd/transport/core/
--rw-r--r--   0 noear      (501) staff       (20)     1426 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Asserts.py
--rw-r--r--   0 noear      (501) staff       (20)     2476 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Channel.py
--rw-r--r--   0 noear      (501) staff       (20)      688 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/ChannelAssistant.py
--rw-r--r--   0 noear      (501) staff       (20)      625 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/ChannelInternal.py
--rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/ChannelSupporter.py
--rw-r--r--   0 noear      (501) staff       (20)     1294 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Codec.py
--rw-r--r--   0 noear      (501) staff       (20)     2978 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Config.py
--rw-r--r--   0 noear      (501) staff       (20)     1262 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Costants.py
--rw-r--r--   0 noear      (501) staff       (20)     1148 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Entity.py
--rw-r--r--   0 noear      (501) staff       (20)      697 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/EntityMetas.py
--rw-r--r--   0 noear      (501) staff       (20)     1717 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Flags.py
--rw-r--r--   0 noear      (501) staff       (20)     1154 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/FragmentAggregator.py
--rw-r--r--   0 noear      (501) staff       (20)      838 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/FragmentHandler.py
--rw-r--r--   0 noear      (501) staff       (20)      419 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Frame.py
--rw-r--r--   0 noear      (501) staff       (20)     2290 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Frames.py
--rw-r--r--   0 noear      (501) staff       (20)     2531 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/HandshakeDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      167 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/IdGenerator.py
--rw-r--r--   0 noear      (501) staff       (20)      504 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Listener.py
--rw-r--r--   0 noear      (501) staff       (20)      735 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Message.py
--rw-r--r--   0 noear      (501) staff       (20)      801 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Processor.py
--rw-r--r--   0 noear      (501) staff       (20)     1953 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/Session.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.735278 socket.d-2.4.10.4/socketd/transport/core/codec/
--rw-r--r--   0 noear      (501) staff       (20)     1164 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/codec/Buffer.py
--rw-r--r--   0 noear      (501) staff       (20)      780 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/codec/ByteBufferCodecReader.py
--rw-r--r--   0 noear      (501) staff       (20)      642 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/codec/ByteBufferCodecWriter.py
--rw-r--r--   0 noear      (501) staff       (20)     4514 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/codec/CodecDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      200 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/codec/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.741684 socket.d-2.4.10.4/socketd/transport/core/entity/
--rw-r--r--   0 noear      (501) staff       (20)     3783 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/entity/EntityDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      839 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/entity/FileEntity.py
--rw-r--r--   0 noear      (501) staff       (20)      885 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/entity/MessageBuilder.py
--rw-r--r--   0 noear      (501) staff       (20)     2045 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/entity/MessageDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      215 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/entity/StringEntity.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/entity/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.743664 socket.d-2.4.10.4/socketd/transport/core/fragment/
--rw-r--r--   0 noear      (501) staff       (20)     2007 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/fragment/FragmentAggregatorDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     3377 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/fragment/FragmentHandlerBase.py
--rw-r--r--   0 noear      (501) staff       (20)      502 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/fragment/FragmentHandlerDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      188 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/fragment/FragmentHolder.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/fragment/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.747256 socket.d-2.4.10.4/socketd/transport/core/impl/
--rw-r--r--   0 noear      (501) staff       (20)     2358 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/impl/ChannelBase.py
--rw-r--r--   0 noear      (501) staff       (20)     6906 2024-04-18 04:06:21.000000 socket.d-2.4.10.4/socketd/transport/core/impl/ChannelDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     6579 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/impl/ConfigBase.py
--rw-r--r--   0 noear      (501) staff       (20)      282 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/impl/LogConfig.py
--rw-r--r--   0 noear      (501) staff       (20)     7748 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/impl/ProcessorDefault.py
--rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/impl/SessionBase.py
--rw-r--r--   0 noear      (501) staff       (20)     4288 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/impl/SessionDefault.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/impl/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.751400 socket.d-2.4.10.4/socketd/transport/core/listener/
--rw-r--r--   0 noear      (501) staff       (20)     2323 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/listener/EventListener.py
--rw-r--r--   0 noear      (501) staff       (20)     1043 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/listener/PathListener.py
--rw-r--r--   0 noear      (501) staff       (20)      176 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/listener/PathMapper.py
--rw-r--r--   0 noear      (501) staff       (20)      457 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/listener/PipelineListener.py
--rw-r--r--   0 noear      (501) staff       (20)      457 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/listener/SimpleListener.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/core/listener/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.754205 socket.d-2.4.10.4/socketd/transport/server/
--rw-r--r--   0 noear      (501) staff       (20)      608 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/server/Server.py
--rw-r--r--   0 noear      (501) staff       (20)     2437 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/server/ServerBase.py
--rw-r--r--   0 noear      (501) staff       (20)     1645 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/server/ServerConfig.py
--rw-r--r--   0 noear      (501) staff       (20)      250 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/server/ServerProvider.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/server/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.763024 socket.d-2.4.10.4/socketd/transport/stream/
--rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/stream/RequestStream.py
--rw-r--r--   0 noear      (501) staff       (20)      332 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/stream/SendStream.py
--rw-r--r--   0 noear      (501) staff       (20)      690 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/stream/Stream.py
--rw-r--r--   0 noear      (501) staff       (20)     2100 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/stream/StreamBase.py
--rw-r--r--   0 noear      (501) staff       (20)      907 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/stream/StreamManger.py
--rw-r--r--   0 noear      (501) staff       (20)     1025 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/stream/StreamMangerDefault.py
--rw-r--r--   0 noear      (501) staff       (20)      843 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/stream/SubscribeStream.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/stream/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.766704 socket.d-2.4.10.4/socketd/transport/utils/
--rw-r--r--   0 noear      (501) staff       (20)     3488 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/utils/AsyncUtil.py
--rw-r--r--   0 noear      (501) staff       (20)     1989 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/utils/CompletableFuture.py
--rw-r--r--   0 noear      (501) staff       (20)      662 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/utils/StrUtil.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/utils/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.767745 socket.d-2.4.10.4/socketd/transport/utils/async_api/
--rw-r--r--   0 noear      (501) staff       (20)      787 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/utils/async_api/AtomicRefer.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/utils/async_api/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.768935 socket.d-2.4.10.4/socketd/transport/utils/sync_api/
--rw-r--r--   0 noear      (501) staff       (20)      747 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/utils/sync_api/AtomicRefer.py
--rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd/transport/utils/sync_api/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.775990 socket.d-2.4.10.4/socketd_aio_tcp/
--rw-r--r--   0 noear      (501) staff       (20)     4144 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_aio_tcp/TCPAIOServer.py
--rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_aio_tcp/TCPStreamIO.py
--rw-r--r--   0 noear      (501) staff       (20)     2331 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_aio_tcp/TcpAIOChannelAssistant.py
--rw-r--r--   0 noear      (501) staff       (20)      645 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_aio_tcp/TcpAioClient.py
--rw-r--r--   0 noear      (501) staff       (20)     6614 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_aio_tcp/TcpAioClientConnector.py
--rw-r--r--   0 noear      (501) staff       (20)      776 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_aio_tcp/TcpAioProvider.py
--rw-r--r--   0 noear      (501) staff       (20)      183 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_aio_tcp/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.779747 socket.d-2.4.10.4/socketd_websocket/
--rw-r--r--   0 noear      (501) staff       (20)     2471 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_websocket/WsAioChannelAssistant.py
--rw-r--r--   0 noear      (501) staff       (20)      574 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_websocket/WsAioClient.py
--rw-r--r--   0 noear      (501) staff       (20)     3630 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_websocket/WsAioClientConnector.py
--rw-r--r--   0 noear      (501) staff       (20)      830 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_websocket/WsAioProvider.py
--rw-r--r--   0 noear      (501) staff       (20)     2289 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_websocket/WsAioServer.py
--rw-r--r--   0 noear      (501) staff       (20)      117 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_websocket/__init__.py
-drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 05:21:32.786897 socket.d-2.4.10.4/socketd_websocket/impl/
--rw-r--r--   0 noear      (501) staff       (20)     4784 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_websocket/impl/AIOConnect.py
--rw-r--r--   0 noear      (501) staff       (20)     6180 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_websocket/impl/AIOServe.py
--rw-r--r--   0 noear      (501) staff       (20)     5946 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_websocket/impl/AIOWebSocketClientImpl.py
--rw-r--r--   0 noear      (501) staff       (20)     4602 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_websocket/impl/AIOWebSocketServerImpl.py
--rw-r--r--   0 noear      (501) staff       (20)      274 2024-04-18 02:59:52.000000 socket.d-2.4.10.4/socketd_websocket/impl/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 09:25:08.482503 socket.d-2.4.10.5/
+-rw-r--r--   0 noear      (501) staff       (20)      555 2024-04-18 09:25:08.481778 socket.d-2.4.10.5/PKG-INFO
+-rw-r--r--   0 noear      (501) staff       (20)     1713 2024-04-18 04:06:21.000000 socket.d-2.4.10.5/README.md
+-rw-r--r--   0 noear      (501) staff       (20)       38 2024-04-18 09:25:08.482777 socket.d-2.4.10.5/setup.cfg
+-rw-r--r--   0 noear      (501) staff       (20)      875 2024-04-18 09:25:05.000000 socket.d-2.4.10.5/setup.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 09:25:08.480873 socket.d-2.4.10.5/socket.d.egg-info/
+-rw-r--r--   0 noear      (501) staff       (20)      555 2024-04-18 09:25:08.000000 socket.d-2.4.10.5/socket.d.egg-info/PKG-INFO
+-rw-r--r--   0 noear      (501) staff       (20)     4922 2024-04-18 09:25:08.000000 socket.d-2.4.10.5/socket.d.egg-info/SOURCES.txt
+-rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-18 09:25:08.000000 socket.d-2.4.10.5/socket.d.egg-info/dependency_links.txt
+-rw-r--r--   0 noear      (501) staff       (20)       18 2024-04-18 09:25:08.000000 socket.d-2.4.10.5/socket.d.egg-info/requires.txt
+-rw-r--r--   0 noear      (501) staff       (20)       42 2024-04-18 09:25:08.000000 socket.d-2.4.10.5/socket.d.egg-info/top_level.txt
+-rw-r--r--   0 noear      (501) staff       (20)        1 2024-04-18 09:25:08.000000 socket.d-2.4.10.5/socket.d.egg-info/zip-safe
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 09:25:08.405101 socket.d-2.4.10.5/socketd/
+-rw-r--r--   0 noear      (501) staff       (20)     4162 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/SocketD.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 09:25:08.407577 socket.d-2.4.10.5/socketd/broker/
+-rw-r--r--   0 noear      (501) staff       (20)      243 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/broker/BrokerFragmentHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)     3571 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/broker/BrokerListener.py
+-rw-r--r--   0 noear      (501) staff       (20)     3128 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/broker/BrokerListenerBase.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/broker/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 09:25:08.410111 socket.d-2.4.10.5/socketd/cluster/
+-rw-r--r--   0 noear      (501) staff       (20)     2757 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/cluster/ClusterClient.py
+-rw-r--r--   0 noear      (501) staff       (20)     2697 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/cluster/ClusterClientSession.py
+-rw-r--r--   0 noear      (501) staff       (20)     2002 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/cluster/LoadBalancer.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/cluster/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 09:25:08.411260 socket.d-2.4.10.5/socketd/exception/
+-rw-r--r--   0 noear      (501) staff       (20)      654 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/exception/SocketDExecption.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/exception/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 09:25:08.411922 socket.d-2.4.10.5/socketd/transport/
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 09:25:08.419616 socket.d-2.4.10.5/socketd/transport/client/
+-rw-r--r--   0 noear      (501) staff       (20)     1720 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/client/Client.py
+-rw-r--r--   0 noear      (501) staff       (20)     3607 2024-04-18 09:13:43.000000 socket.d-2.4.10.5/socketd/transport/client/ClientBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     6520 2024-04-18 09:13:43.000000 socket.d-2.4.10.5/socketd/transport/client/ClientChannel.py
+-rw-r--r--   0 noear      (501) staff       (20)     2843 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/client/ClientConfig.py
+-rw-r--r--   0 noear      (501) staff       (20)      144 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/client/ClientConfigHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      384 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/client/ClientConnectHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      483 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/client/ClientConnector.py
+-rw-r--r--   0 noear      (501) staff       (20)      462 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/client/ClientConnectorBase.py
+-rw-r--r--   0 noear      (501) staff       (20)      373 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/client/ClientHandshakeResult.py
+-rw-r--r--   0 noear      (501) staff       (20)      224 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/client/ClientHeartbeatHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      303 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/client/ClientProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)     1126 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/client/ClientSession.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/client/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 09:25:08.433071 socket.d-2.4.10.5/socketd/transport/core/
+-rw-r--r--   0 noear      (501) staff       (20)     1426 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/Asserts.py
+-rw-r--r--   0 noear      (501) staff       (20)     2482 2024-04-18 09:13:43.000000 socket.d-2.4.10.5/socketd/transport/core/Channel.py
+-rw-r--r--   0 noear      (501) staff       (20)      688 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/ChannelAssistant.py
+-rw-r--r--   0 noear      (501) staff       (20)      625 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/ChannelInternal.py
+-rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/ChannelSupporter.py
+-rw-r--r--   0 noear      (501) staff       (20)     1294 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/Codec.py
+-rw-r--r--   0 noear      (501) staff       (20)     2978 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/Config.py
+-rw-r--r--   0 noear      (501) staff       (20)     1262 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/Costants.py
+-rw-r--r--   0 noear      (501) staff       (20)     1148 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/Entity.py
+-rw-r--r--   0 noear      (501) staff       (20)      697 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/EntityMetas.py
+-rw-r--r--   0 noear      (501) staff       (20)     1717 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/Flags.py
+-rw-r--r--   0 noear      (501) staff       (20)     1154 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/FragmentAggregator.py
+-rw-r--r--   0 noear      (501) staff       (20)      838 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/FragmentHandler.py
+-rw-r--r--   0 noear      (501) staff       (20)      419 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/Frame.py
+-rw-r--r--   0 noear      (501) staff       (20)     2290 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/Frames.py
+-rw-r--r--   0 noear      (501) staff       (20)     2531 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/HandshakeDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      167 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/IdGenerator.py
+-rw-r--r--   0 noear      (501) staff       (20)      504 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/Listener.py
+-rw-r--r--   0 noear      (501) staff       (20)      735 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/Message.py
+-rw-r--r--   0 noear      (501) staff       (20)      801 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/Processor.py
+-rw-r--r--   0 noear      (501) staff       (20)     1953 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/Session.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 09:25:08.436350 socket.d-2.4.10.5/socketd/transport/core/codec/
+-rw-r--r--   0 noear      (501) staff       (20)     1164 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/codec/Buffer.py
+-rw-r--r--   0 noear      (501) staff       (20)      780 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/codec/ByteBufferCodecReader.py
+-rw-r--r--   0 noear      (501) staff       (20)      642 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/codec/ByteBufferCodecWriter.py
+-rw-r--r--   0 noear      (501) staff       (20)     4514 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/codec/CodecDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      200 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/codec/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 09:25:08.439447 socket.d-2.4.10.5/socketd/transport/core/entity/
+-rw-r--r--   0 noear      (501) staff       (20)     3783 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/entity/EntityDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      839 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/entity/FileEntity.py
+-rw-r--r--   0 noear      (501) staff       (20)      885 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/entity/MessageBuilder.py
+-rw-r--r--   0 noear      (501) staff       (20)     2045 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/entity/MessageDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      215 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/entity/StringEntity.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/entity/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 09:25:08.441851 socket.d-2.4.10.5/socketd/transport/core/fragment/
+-rw-r--r--   0 noear      (501) staff       (20)     2007 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/fragment/FragmentAggregatorDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     3377 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/fragment/FragmentHandlerBase.py
+-rw-r--r--   0 noear      (501) staff       (20)      502 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/fragment/FragmentHandlerDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      188 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/fragment/FragmentHolder.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/fragment/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 09:25:08.447618 socket.d-2.4.10.5/socketd/transport/core/impl/
+-rw-r--r--   0 noear      (501) staff       (20)     2358 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/impl/ChannelBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     6927 2024-04-18 09:13:43.000000 socket.d-2.4.10.5/socketd/transport/core/impl/ChannelDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     6579 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/impl/ConfigBase.py
+-rw-r--r--   0 noear      (501) staff       (20)      338 2024-04-18 09:13:43.000000 socket.d-2.4.10.5/socketd/transport/core/impl/LogConfig.py
+-rw-r--r--   0 noear      (501) staff       (20)     7672 2024-04-18 09:13:43.000000 socket.d-2.4.10.5/socketd/transport/core/impl/ProcessorDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/impl/SessionBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     4288 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/impl/SessionDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/impl/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 09:25:08.452101 socket.d-2.4.10.5/socketd/transport/core/listener/
+-rw-r--r--   0 noear      (501) staff       (20)     2323 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/listener/EventListener.py
+-rw-r--r--   0 noear      (501) staff       (20)     1043 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/listener/PathListener.py
+-rw-r--r--   0 noear      (501) staff       (20)      176 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/listener/PathMapper.py
+-rw-r--r--   0 noear      (501) staff       (20)      457 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/listener/PipelineListener.py
+-rw-r--r--   0 noear      (501) staff       (20)      457 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/listener/SimpleListener.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/core/listener/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 09:25:08.455830 socket.d-2.4.10.5/socketd/transport/server/
+-rw-r--r--   0 noear      (501) staff       (20)      723 2024-04-18 05:45:29.000000 socket.d-2.4.10.5/socketd/transport/server/Server.py
+-rw-r--r--   0 noear      (501) staff       (20)     2437 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/server/ServerBase.py
+-rw-r--r--   0 noear      (501) staff       (20)     1645 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/server/ServerConfig.py
+-rw-r--r--   0 noear      (501) staff       (20)      250 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/server/ServerProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/server/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 09:25:08.462201 socket.d-2.4.10.5/socketd/transport/stream/
+-rw-r--r--   0 noear      (501) staff       (20)     1355 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/stream/RequestStream.py
+-rw-r--r--   0 noear      (501) staff       (20)      332 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/stream/SendStream.py
+-rw-r--r--   0 noear      (501) staff       (20)      690 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/stream/Stream.py
+-rw-r--r--   0 noear      (501) staff       (20)     2100 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/stream/StreamBase.py
+-rw-r--r--   0 noear      (501) staff       (20)      907 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/stream/StreamManger.py
+-rw-r--r--   0 noear      (501) staff       (20)     1025 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/stream/StreamMangerDefault.py
+-rw-r--r--   0 noear      (501) staff       (20)      843 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/stream/SubscribeStream.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/stream/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 09:25:08.464386 socket.d-2.4.10.5/socketd/transport/utils/
+-rw-r--r--   0 noear      (501) staff       (20)     3488 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/utils/AsyncUtil.py
+-rw-r--r--   0 noear      (501) staff       (20)     1989 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/utils/CompletableFuture.py
+-rw-r--r--   0 noear      (501) staff       (20)      662 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/utils/StrUtil.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/utils/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 09:25:08.465111 socket.d-2.4.10.5/socketd/transport/utils/async_api/
+-rw-r--r--   0 noear      (501) staff       (20)      787 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/utils/async_api/AtomicRefer.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/utils/async_api/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 09:25:08.466019 socket.d-2.4.10.5/socketd/transport/utils/sync_api/
+-rw-r--r--   0 noear      (501) staff       (20)      747 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/utils/sync_api/AtomicRefer.py
+-rw-r--r--   0 noear      (501) staff       (20)        0 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd/transport/utils/sync_api/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 09:25:08.471094 socket.d-2.4.10.5/socketd_aio_tcp/
+-rw-r--r--   0 noear      (501) staff       (20)     4144 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd_aio_tcp/TCPAIOServer.py
+-rw-r--r--   0 noear      (501) staff       (20)      517 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd_aio_tcp/TCPStreamIO.py
+-rw-r--r--   0 noear      (501) staff       (20)     2331 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd_aio_tcp/TcpAIOChannelAssistant.py
+-rw-r--r--   0 noear      (501) staff       (20)      645 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd_aio_tcp/TcpAioClient.py
+-rw-r--r--   0 noear      (501) staff       (20)     6594 2024-04-18 09:13:43.000000 socket.d-2.4.10.5/socketd_aio_tcp/TcpAioClientConnector.py
+-rw-r--r--   0 noear      (501) staff       (20)      776 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd_aio_tcp/TcpAioProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)      183 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd_aio_tcp/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 09:25:08.476071 socket.d-2.4.10.5/socketd_websocket/
+-rw-r--r--   0 noear      (501) staff       (20)     2471 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd_websocket/WsAioChannelAssistant.py
+-rw-r--r--   0 noear      (501) staff       (20)      574 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd_websocket/WsAioClient.py
+-rw-r--r--   0 noear      (501) staff       (20)     3636 2024-04-18 09:13:43.000000 socket.d-2.4.10.5/socketd_websocket/WsAioClientConnector.py
+-rw-r--r--   0 noear      (501) staff       (20)      830 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd_websocket/WsAioProvider.py
+-rw-r--r--   0 noear      (501) staff       (20)     2289 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd_websocket/WsAioServer.py
+-rw-r--r--   0 noear      (501) staff       (20)      117 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd_websocket/__init__.py
+drwxr-xr-x   0 noear      (501) staff       (20)        0 2024-04-18 09:25:08.480219 socket.d-2.4.10.5/socketd_websocket/impl/
+-rw-r--r--   0 noear      (501) staff       (20)     4784 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd_websocket/impl/AIOConnect.py
+-rw-r--r--   0 noear      (501) staff       (20)     6180 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd_websocket/impl/AIOServe.py
+-rw-r--r--   0 noear      (501) staff       (20)     5990 2024-04-18 09:13:43.000000 socket.d-2.4.10.5/socketd_websocket/impl/AIOWebSocketClientImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)     4602 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd_websocket/impl/AIOWebSocketServerImpl.py
+-rw-r--r--   0 noear      (501) staff       (20)      274 2024-04-18 02:59:52.000000 socket.d-2.4.10.5/socketd_websocket/impl/__init__.py
```

### Comparing `socket.d-2.4.10.4/PKG-INFO` & `socket.d-2.4.10.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socket.d
-Version: 2.4.10.4
+Version: 2.4.10.5
 Summary: @noear/socket.d python project
 Home-page: https://socketd.noear.org/
 Author: noear,bai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
```

### Comparing `socket.d-2.4.10.4/README.md` & `socket.d-2.4.10.5/README.md`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/setup.py` & `socket.d-2.4.10.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 #! /usr/bin/env python
 # -*- coding: utf-8 -*_
 from setuptools import setup,find_packages
 
 setup(
     name='socket.d',
-    version='2.4.10.4',
+    version='2.4.10.5',
     description='@noear/socket.d python project',
     author='noear,bai',
     url='https://socketd.noear.org/',
     packages=find_packages(exclude=['*test*']),   # 包内不需要引用的文件夹
     install_requires=[                          # 依赖包
         'loguru',
         'websockets'
```

### Comparing `socket.d-2.4.10.4/socket.d.egg-info/PKG-INFO` & `socket.d-2.4.10.5/socket.d.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: socket.d
-Version: 2.4.10.4
+Version: 2.4.10.5
 Summary: @noear/socket.d python project
 Home-page: https://socketd.noear.org/
 Author: noear,bai
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved
 Classifier: Operating System :: OS Independent
```

### Comparing `socket.d-2.4.10.4/socket.d.egg-info/SOURCES.txt` & `socket.d-2.4.10.5/socket.d.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/SocketD.py` & `socket.d-2.4.10.5/socketd/SocketD.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/broker/BrokerListener.py` & `socket.d-2.4.10.5/socketd/broker/BrokerListener.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/broker/BrokerListenerBase.py` & `socket.d-2.4.10.5/socketd/broker/BrokerListenerBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/cluster/ClusterClient.py` & `socket.d-2.4.10.5/socketd/cluster/ClusterClient.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/cluster/ClusterClientSession.py` & `socket.d-2.4.10.5/socketd/cluster/ClusterClientSession.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/cluster/LoadBalancer.py` & `socket.d-2.4.10.5/socketd/cluster/LoadBalancer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/exception/SocketDExecption.py` & `socket.d-2.4.10.5/socketd/exception/SocketDExecption.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/client/Client.py` & `socket.d-2.4.10.5/socketd/transport/client/Client.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/client/ClientBase.py` & `socket.d-2.4.10.5/socketd/transport/client/ClientBase.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,18 +7,18 @@
 from socketd.transport.client.ClientConfigHandler import ClientConfigHandler
 from socketd.transport.client.ClientConnectHandler import ClientConnectHandler, ClientConnectHandlerDefault
 from socketd.transport.client.ClientConnector import ClientConnector
 from socketd.transport.core.ChannelAssistant import ChannelAssistant
 from socketd.transport.core.Costants import Constants
 from socketd.transport.core.Session import Session
 from socketd.transport.client.ClientHeartbeatHandler import ClientHeartbeatHandler
+from socketd.transport.core.impl.LogConfig import log
 from socketd.transport.core.impl.ProcessorDefault import ProcessorDefault
 from socketd.transport.client.ClientConfig import ClientConfig
 
-from loguru import logger
 
 
 class ClientBase(ClientInternal, ABC):
 
     def __init__(self, client_config: ClientConfig, assistant: ChannelAssistant):
         self.__config: ClientConfig = client_config
         self.__assistant: ChannelAssistant = assistant
@@ -72,21 +72,21 @@
 
     async def _open_do(self, isThrow):
         connector: ClientConnector = self.create_connector()
         clientChannel: ClientChannel = ClientChannel(self, connector)
 
         try:
             await clientChannel.connect()
-            logger.info(f"Socket.D client successfully connected: link={self.get_config().get_link_url()}")
+            log.info(f"Socket.D client successfully connected: link={self.get_config().get_link_url()}")
         except Exception as e:
             if isThrow:
                 await clientChannel.close(code=Constants.CLOSE2008_OPEN_FAIL)
                 raise SocketDException(f"Socket.D client Connection failed {e}")
             else:
-                logger.info(f"Socket.D client Connection failed: link={self.get_config().get_link_url()}")
+                log.info(f"Socket.D client Connection failed: link={self.get_config().get_link_url()}")
 
         return clientChannel.get_session()
 
     def open(self) -> Awaitable[Session]:
         return self._open_do(False)
 
     def open_or_throw(self) -> Awaitable[Session]:
```

### Comparing `socket.d-2.4.10.4/socketd/transport/client/ClientChannel.py` & `socket.d-2.4.10.5/socketd/transport/client/ClientChannel.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,19 +2,19 @@
 from asyncio import Future
 
 from socketd.exception.SocketDExecption import SocketDException, SocketDChannelException
 from socketd.transport.client.Client import ClientInternal
 from socketd.transport.core.Asserts import Asserts
 from socketd.transport.core.ChannelInternal import ChannelInternal
 from socketd.transport.core.Costants import Constants
+from socketd.transport.core.impl.LogConfig import log
 from socketd.transport.core.impl.SessionDefault import SessionDefault
 from socketd.transport.stream.StreamManger import StreamInternal
 from socketd.transport.core.impl.ChannelBase import ChannelBase
 from socketd.transport.client.ClientConnector import ClientConnector
-from loguru import logger
 
 from socketd.transport.client.ClientHeartbeatHandler import ClientHeartbeatHandlerDefault
 from socketd.transport.utils.sync_api.AtomicRefer import AtomicRefer
 
 
 class ClientChannel(ChannelBase):
     def __init__(self, client: ClientInternal, connector: ClientConnector):
@@ -36,15 +36,15 @@
         self.init_heartbeat()
 
     def __del__(self):
         try:
             if not self.__heartbeatScheduledFuture.done():
                 self.__heartbeatScheduledFuture.cancel()
         except Exception as e:
-            logger.warning(e)
+            log.warning(e)
 
     async def __heartbeatScheduled(self) -> None:
         while True:
             await asyncio.sleep(self.__client.get_heartbeat_interval() / 1000)
             await self.heartbeat_handle()
 
     def init_heartbeat(self):
@@ -56,15 +56,15 @@
 
     async def heartbeat_handle(self):
         if self.__real:
             if self.__real.get_handshake() is None:
                 return
 
             if Asserts.is_closed_and_end(self.__real):
-                logger.debug("Client channel is closed (pause heartbeat), sessionId=" + self.get_session().session_id())
+                log.debug("Client channel is closed (pause heartbeat), sessionId=" + self.get_session().session_id())
                 await self.close(self.__real.is_closed())
                 return
 
             if self.__real.is_closing():
                 return
 
         with self:
@@ -132,29 +132,29 @@
 
             if self.__connector:
                 await self.__connector.close()
 
             if self.__real:
                 await self.__real.close(code)
         except Exception as e:
-            logger.error(e)
+            log.error(e)
         finally:
             await super().close(code)
 
     def get_session(self):
         return self.__sessionShell
 
     def on_error(self, error: Exception):
         self.__real.on_error(error)
 
     async def reconnect(self):
         self.init_heartbeat()
         await self.internalCheck()
 
-    @logger.catch
+    @log.catch
     async def connect(self):
         with self.__isConnecting as isConnected:
             if isConnected:
                 return
             else:
                 self.__isConnecting.set(True)
 
@@ -162,17 +162,17 @@
             if self.__real:
                 await self.__real.close(Constants.CLOSE2002_RECONNECT)
 
             self.__real = await self.__client.get_connect_handler()(self.__connector)
             self.__real.set_session(self.__sessionShell)
             self.set_handshake(self.__real.get_handshake())
         except TimeoutError as t:
-            logger.error(f"socketD connect timed out: {t}")
+            log.error(f"socketD connect timed out: {t}")
         except Exception as e:
-            logger.error(e)
+            log.error(e)
             raise SocketDChannelException(f"socketD connect")
         finally:
             self.__isConnecting.set(False)
 
     async def internalCloseIfError(self):
         if self.__real:
             await self.__real.close(Constants.CLOSE2001_ERROR)
```

### Comparing `socket.d-2.4.10.4/socketd/transport/client/ClientConfig.py` & `socket.d-2.4.10.5/socketd/transport/client/ClientConfig.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/client/ClientSession.py` & `socket.d-2.4.10.5/socketd/transport/client/ClientSession.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/Asserts.py` & `socket.d-2.4.10.5/socketd/transport/core/Asserts.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/Channel.py` & `socket.d-2.4.10.5/socketd/transport/core/Channel.py`

 * *Files 2% similar despite different names*

```diff
@@ -83,15 +83,15 @@
         ...
 
     @abstractmethod
     async def send(self, frame: 'Frame', stream: Optional[StreamInternal]) -> None:
         ...
 
     @abstractmethod
-    def retrieve(self, frame: Frame, stream: StreamInternal) -> None:
+    async def retrieve(self, frame: Frame, stream: StreamInternal) -> None:
         ...
 
     @abstractmethod
     def get_session(self) -> Session:
         ...
 
     @abstractmethod
```

### Comparing `socket.d-2.4.10.4/socketd/transport/core/ChannelAssistant.py` & `socket.d-2.4.10.5/socketd/transport/core/ChannelAssistant.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/ChannelInternal.py` & `socket.d-2.4.10.5/socketd/transport/core/ChannelInternal.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/ChannelSupporter.py` & `socket.d-2.4.10.5/socketd/transport/core/ChannelSupporter.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/Codec.py` & `socket.d-2.4.10.5/socketd/transport/core/Codec.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/Config.py` & `socket.d-2.4.10.5/socketd/transport/core/Config.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/Costants.py` & `socket.d-2.4.10.5/socketd/transport/core/Costants.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/Entity.py` & `socket.d-2.4.10.5/socketd/transport/core/Entity.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/EntityMetas.py` & `socket.d-2.4.10.5/socketd/transport/core/EntityMetas.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/Flags.py` & `socket.d-2.4.10.5/socketd/transport/core/Flags.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/FragmentAggregator.py` & `socket.d-2.4.10.5/socketd/transport/core/FragmentAggregator.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/FragmentHandler.py` & `socket.d-2.4.10.5/socketd/transport/core/FragmentHandler.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/Frames.py` & `socket.d-2.4.10.5/socketd/transport/core/Frames.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/HandshakeDefault.py` & `socket.d-2.4.10.5/socketd/transport/core/HandshakeDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/Message.py` & `socket.d-2.4.10.5/socketd/transport/core/Message.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/Processor.py` & `socket.d-2.4.10.5/socketd/transport/core/Processor.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/Session.py` & `socket.d-2.4.10.5/socketd/transport/core/Session.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/codec/Buffer.py` & `socket.d-2.4.10.5/socketd/transport/core/codec/Buffer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/codec/ByteBufferCodecReader.py` & `socket.d-2.4.10.5/socketd/transport/core/codec/ByteBufferCodecReader.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/codec/ByteBufferCodecWriter.py` & `socket.d-2.4.10.5/socketd/transport/core/codec/ByteBufferCodecWriter.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/codec/CodecDefault.py` & `socket.d-2.4.10.5/socketd/transport/core/codec/CodecDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/entity/EntityDefault.py` & `socket.d-2.4.10.5/socketd/transport/core/entity/EntityDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/entity/FileEntity.py` & `socket.d-2.4.10.5/socketd/transport/core/entity/FileEntity.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/entity/MessageBuilder.py` & `socket.d-2.4.10.5/socketd/transport/core/entity/MessageBuilder.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/entity/MessageDefault.py` & `socket.d-2.4.10.5/socketd/transport/core/entity/MessageDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/fragment/FragmentAggregatorDefault.py` & `socket.d-2.4.10.5/socketd/transport/core/fragment/FragmentAggregatorDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/fragment/FragmentHandlerBase.py` & `socket.d-2.4.10.5/socketd/transport/core/fragment/FragmentHandlerBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/impl/ChannelBase.py` & `socket.d-2.4.10.5/socketd/transport/core/impl/ChannelBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/impl/ChannelDefault.py` & `socket.d-2.4.10.5/socketd/transport/core/impl/ChannelDefault.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,28 +102,28 @@
                 await self.get_config().get_fragment_handler().split_fragment(self, stream, message, __consumer)
             return
 
         await self._assistant.write(self._source, frame)
         if stream is not None:
             stream.on_progress(True, 1, 1)
 
-    def retrieve(self, frame: Frame, stream: StreamInternal) -> None:
+    async def retrieve(self, frame: Frame, stream: StreamInternal) -> None:
         """接收（接收答复帧）"""
         if stream is not None:
             if stream.demands() < Constants.DEMANDS_MULTIPLE or frame.flag() == Flags.ReplyEnd:
                 # 如果是单收或者答复结束，则移除流接收器
                 self._streamManger.remove_stream(frame.message().sid())
 
             if stream.demands() < Constants.DEMANDS_MULTIPLE:
                 # 单收时，内部已经是异步机制
-                stream.on_reply(frame.message())
+                await stream.on_reply(frame.message())
             else:
-                #stream.on_reply(frame.message())
                 # 改为异步处理，避免卡死Io线程
-                asyncio.get_running_loop().run_in_executor(self.get_config().get_exchange_executor(), lambda _m: asyncio.run(stream.on_reply(_m)), frame.message())
+                asyncio.get_running_loop().run_in_executor(self.get_config().get_exchange_executor(),
+                                                           lambda _m: asyncio.run(stream.on_reply(_m)), frame.message())
         else:
             log.debug(
                 f"{self.get_config().get_role_name()} stream not found, sid={frame.message().sid()}, sessionId={self.get_session().session_id()}")
 
     def reconnect(self):
         ...
```

### Comparing `socket.d-2.4.10.4/socketd/transport/core/impl/ConfigBase.py` & `socket.d-2.4.10.5/socketd/transport/core/impl/ConfigBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/impl/ProcessorDefault.py` & `socket.d-2.4.10.5/socketd/transport/core/impl/ProcessorDefault.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,52 +1,48 @@
 import asyncio
 from abc import ABC
-from typing import Optional, Union
-
-from loguru import logger
+from typing import Optional
 
 from socketd.exception.SocketDExecption import SocketDAlarmException, SocketDConnectionException
 from socketd.transport.core.ChannelInternal import ChannelInternal
 from socketd.transport.core.HandshakeDefault import HandshakeDefault
 from socketd.transport.core.Message import Message
 from socketd.transport.core.Processor import Processor
 from socketd.transport.core.Costants import Constants
 from socketd.transport.core.Flags import Flags
 from socketd.transport.core.EntityMetas import EntityMetas
 from socketd.transport.core.Frame import Frame
+from socketd.transport.core.impl.LogConfig import log
 from socketd.transport.core.listener.SimpleListener import SimpleListener
-from socketd.transport.stream.Stream import Stream
 from socketd.transport.stream.StreamManger import StreamInternal
-from socketd.transport.utils.AsyncUtil import AsyncUtil
 
 
 class ProcessorDefault(Processor, ABC):
 
     def __init__(self):
         self.listener = SimpleListener()
-        self.log = logger.opt()
 
     def set_listener(self, listener):
         if listener is not None:
             self.listener = listener
 
     async def on_receive(self, channel: ChannelInternal, frame):
         if channel.get_config().client_mode():
-            logger.debug(f"C-REV:{frame}")
+            log.debug(f"C-REV:{frame}")
         else:
-            logger.debug(f"S-REV:{frame}")
+            log.debug(f"S-REV:{frame}")
 
         if frame.flag() == Flags.Connect:
             # if server
             connectMessage = frame.message()
             channel.set_handshake(HandshakeDefault(connectMessage))
 
             async def _future(r: bool, e: Exception):
                 if r:
-                    #如果无异常
+                    # 如果无异常
                     if channel.is_valid():
                         try:
                             await channel.send_connack(connectMessage)
                         except Exception as _e:
                             self.on_error(channel, _e)
                 else:
                     # 如果有异常
@@ -63,29 +59,30 @@
         else:
             if channel.get_handshake() is None:
                 await channel.close(Constants.CLOSE1002_PROTOCOL_ILLEGAL)
 
                 if frame.flag() == Flags.Close:
                     raise SocketDConnectionException("Connection request was rejected")
 
-                self.log.warning("{} channel handshake is None, sessionId={}", channel.get_config().get_role_name(), channel.get_session().session_id())
+                log.warning("{} channel handshake is None, sessionId={}", channel.get_config().get_role_name(),
+                                 channel.get_session().session_id())
                 return
 
             # 更新最后活动时间
             channel.set_live_time_as_now()
 
             try:
                 if frame.flag() == Flags.Ping:
                     await channel.send_pong()
                 elif frame.flag() == Flags.Pong:
                     pass
                 elif frame.flag() == Flags.Close:
-                    code:int = 0
+                    code: int = 0
 
-                    if frame.message()  is not None:
+                    if frame.message() is not None:
                         code = frame.message().meta_as_int("code")
 
                     if code == 0:
                         code = Constants.CLOSE1001_PROTOCOL_CLOSE
 
                     await self.on_close_internal(channel, code)
                 elif frame.flag() == Flags.Alarm:
@@ -137,45 +134,44 @@
                 else:
                     del frame
                     frame = frameNew
 
         if isReply:
             if stream:
                 stream.on_progress(False, streamIndex, streamTotal)
-            channel.retrieve(frame, stream)
+            await channel.retrieve(frame, stream)
         else:
             self.on_message(channel, frame.message())
 
     def on_open(self, channel: ChannelInternal):
         asyncio.create_task(self.on_open_do(channel))
 
     async def on_open_do(self, channel: ChannelInternal):
         try:
             await self.listener.on_open(channel.get_session())
             channel.do_open_future(True, None)
         except Exception as e:
-            logger.warning("{} channel listener onOpen error", channel.get_config().get_role_name(), e)
+            log.warning("{} channel listener onOpen error", channel.get_config().get_role_name(), e)
             channel.do_open_future(False, e)
 
     def on_message(self, channel: ChannelInternal, message: Message):
         asyncio.create_task(self.on_message_do(channel, message))
 
     async def on_message_do(self, channel: ChannelInternal, message: Message):
         try:
             await self.listener.on_message(channel.get_session(), message)
         except Exception as e:
-            logger.warning("{} channel listener onMessage error", channel.get_config().get_role_name(), e)
+            log.warning("{} channel listener onMessage error", channel.get_config().get_role_name(), e)
             self.on_error(channel, e)
 
     def on_close(self, channel: ChannelInternal):
         if channel.is_closed() <= Constants.CLOSE1000_PROTOCOL_CLOSE_STARTING:
-            self.on_close_internal(channel, Constants.CLOSE2003_DISCONNECTION)
+            asyncio.create_task(self.on_close_internal(channel, Constants.CLOSE2003_DISCONNECTION))
 
     async def on_close_internal(self, channel: ChannelInternal, code: int):
         await channel.close(code)
 
         if code > Constants.CLOSE1000_PROTOCOL_CLOSE_STARTING:
             await self.listener.on_close(channel.get_session())
 
     def on_error(self, channel: ChannelInternal, error):
         self.listener.on_error(channel.get_session(), error)
-
```

### Comparing `socket.d-2.4.10.4/socketd/transport/core/impl/SessionBase.py` & `socket.d-2.4.10.5/socketd/transport/core/impl/SessionBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/impl/SessionDefault.py` & `socket.d-2.4.10.5/socketd/transport/core/impl/SessionDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/listener/EventListener.py` & `socket.d-2.4.10.5/socketd/transport/core/listener/EventListener.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/core/listener/PathListener.py` & `socket.d-2.4.10.5/socketd/transport/core/listener/PathListener.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/server/Server.py` & `socket.d-2.4.10.5/socketd/transport/server/Server.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,22 +3,29 @@
 from typing import Callable, Coroutine
 
 from websockets.sync.server import WebSocketServer
 
 from socketd.transport.server.ServerConfig import ServerConfig
 from socketd.transport.core.Listener import Listener
 
-
+#服务端接口
 class Server:
+    #获取台头
     def get_title(self): ...
 
+    #获取配置
     def get_config(self) -> ServerConfig: ...
 
+    #配置
     def config(self, consumer: Callable[[ServerConfig], None]) -> Server: ...
 
+    #监听
     def listen(self, listener: Listener) -> Server: ...
 
+    #启动
     def start(self) -> WebSocketServer | Coroutine: ...
 
+    #预停止
     def prestop(self) -> Coroutine: ...
 
+    #停止
     def stop(self) -> Coroutine: ...
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `socket.d-2.4.10.4/socketd/transport/server/ServerBase.py` & `socket.d-2.4.10.5/socketd/transport/server/ServerBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/server/ServerConfig.py` & `socket.d-2.4.10.5/socketd/transport/server/ServerConfig.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/stream/RequestStream.py` & `socket.d-2.4.10.5/socketd/transport/stream/RequestStream.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/stream/Stream.py` & `socket.d-2.4.10.5/socketd/transport/stream/Stream.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/stream/StreamBase.py` & `socket.d-2.4.10.5/socketd/transport/stream/StreamBase.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/stream/StreamManger.py` & `socket.d-2.4.10.5/socketd/transport/stream/StreamManger.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/stream/StreamMangerDefault.py` & `socket.d-2.4.10.5/socketd/transport/stream/StreamMangerDefault.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/stream/SubscribeStream.py` & `socket.d-2.4.10.5/socketd/transport/stream/SubscribeStream.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/utils/AsyncUtil.py` & `socket.d-2.4.10.5/socketd/transport/utils/AsyncUtil.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/utils/CompletableFuture.py` & `socket.d-2.4.10.5/socketd/transport/utils/CompletableFuture.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/utils/StrUtil.py` & `socket.d-2.4.10.5/socketd/transport/utils/StrUtil.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/utils/async_api/AtomicRefer.py` & `socket.d-2.4.10.5/socketd/transport/utils/async_api/AtomicRefer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd/transport/utils/sync_api/AtomicRefer.py` & `socket.d-2.4.10.5/socketd/transport/utils/sync_api/AtomicRefer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd_aio_tcp/TCPAIOServer.py` & `socket.d-2.4.10.5/socketd_aio_tcp/TCPAIOServer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd_aio_tcp/TCPStreamIO.py` & `socket.d-2.4.10.5/socketd_aio_tcp/TCPStreamIO.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd_aio_tcp/TcpAIOChannelAssistant.py` & `socket.d-2.4.10.5/socketd_aio_tcp/TcpAIOChannelAssistant.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd_aio_tcp/TcpAioClient.py` & `socket.d-2.4.10.5/socketd_aio_tcp/TcpAioClient.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd_aio_tcp/TcpAioClientConnector.py` & `socket.d-2.4.10.5/socketd_aio_tcp/TcpAioClientConnector.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,15 @@
         self.transfer_dataTask: Optional[asyncio.Task] = None
         self._on_receive_tasks: List[asyncio.Task] = []
         self._loop: Optional[asyncio.AbstractEventLoop] = None
 
     async def connect(self):
         # 处理自定义架构的影响
         loop = asyncio.get_running_loop()
-        tcp_url = self.client.get_config().get_url().replace("std:", "").replace("-python", "")
+        tcp_url = self.client.get_config().get_url().replace("-python", "")
         _sch, _host, _port = tcp_url.replace("//", "").split(":")
         _port = int(_port.split("/")[0])
         if self.__top is None:
             self._loop = asyncio.new_event_loop()
             self.__top = AsyncUtil.run_forever(self._loop, daemon=True)
         try:
```

### Comparing `socket.d-2.4.10.4/socketd_aio_tcp/TcpAioProvider.py` & `socket.d-2.4.10.5/socketd_aio_tcp/TcpAioProvider.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd_websocket/WsAioChannelAssistant.py` & `socket.d-2.4.10.5/socketd_websocket/WsAioChannelAssistant.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd_websocket/WsAioClient.py` & `socket.d-2.4.10.5/socketd_websocket/WsAioClient.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd_websocket/WsAioClientConnector.py` & `socket.d-2.4.10.5/socketd_websocket/WsAioClientConnector.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
         self._loop: Optional[asyncio.AbstractEventLoop] = None
         self.__real: Optional[AIOWebSocketClientImpl] = None
         self.__con: Optional[AIOConnect] = None
         super().__init__(client)
 
     async def connect(self) -> Channel:
         # 关闭之前的资源
-        self.close()
+        await self.close()
 
         # 处理自定义架构的影响
         ws_url = self.client.get_config().get_url().replace("-python://", "://")
 
         # 支持 ssl
         if self.client.get_config().get_ssl_context() is not None:
             ws_url = ws_url.replace("ws", "wss")
```

### Comparing `socket.d-2.4.10.4/socketd_websocket/WsAioProvider.py` & `socket.d-2.4.10.5/socketd_websocket/WsAioProvider.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd_websocket/WsAioServer.py` & `socket.d-2.4.10.5/socketd_websocket/WsAioServer.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd_websocket/impl/AIOConnect.py` & `socket.d-2.4.10.5/socketd_websocket/impl/AIOConnect.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd_websocket/impl/AIOServe.py` & `socket.d-2.4.10.5/socketd_websocket/impl/AIOServe.py`

 * *Files identical despite different names*

### Comparing `socket.d-2.4.10.4/socketd_websocket/impl/AIOWebSocketClientImpl.py` & `socket.d-2.4.10.5/socketd_websocket/impl/AIOWebSocketClientImpl.py`

 * *Files 1% similar despite different names*

```diff
@@ -124,12 +124,13 @@
             logger.info(e)
         except Exception as e:
             self.on_error(e)
 
     async def on_close(self):
         await self.client.get_processor().on_close(self.channel)
         if self.handshake_future is not None:
-            await asyncio.wait(self.__on_receive_tasks, timeout=10)
+            if self.__on_receive_tasks:
+                await asyncio.wait(self.__on_receive_tasks, timeout=10)
             await asyncio.wait([self._handler_future], timeout=10)
 
     def on_error(self, e):
         self.client.get_processor().on_error(self.channel, e)
```

### Comparing `socket.d-2.4.10.4/socketd_websocket/impl/AIOWebSocketServerImpl.py` & `socket.d-2.4.10.5/socketd_websocket/impl/AIOWebSocketServerImpl.py`

 * *Files identical despite different names*

