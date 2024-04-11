# Comparing `tmp/kombu-5.3.6.tar.gz` & `tmp/kombu-5.3.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kombu-5.3.6.tar", last modified: Wed Mar 27 13:06:01 2024, max compression
+gzip compressed data, was "kombu-5.3.7.tar", last modified: Thu Apr 11 12:14:51 2024, max compression
```

## Comparing `kombu-5.3.6.tar` & `kombu-5.3.7.tar`

### file list

```diff
@@ -1,346 +1,346 @@
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.328217 kombu-5.3.6/
--rw-r--r--   0 nusnus     (501) staff       (20)     5599 2022-10-19 10:47:33.000000 kombu-5.3.6/AUTHORS
--rw-r--r--   0 nusnus     (501) staff       (20)      436 2022-09-28 15:48:06.000000 kombu-5.3.6/FAQ
--rw-r--r--   0 nusnus     (501) staff       (20)      387 2022-09-28 15:48:06.000000 kombu-5.3.6/INSTALL
--rw-r--r--   0 nusnus     (501) staff       (20)     1664 2022-09-28 15:48:06.000000 kombu-5.3.6/LICENSE
--rw-r--r--   0 nusnus     (501) staff       (20)      515 2022-09-28 15:48:06.000000 kombu-5.3.6/MANIFEST.in
--rw-r--r--   0 nusnus     (501) staff       (20)     3027 2024-03-27 13:06:01.328128 kombu-5.3.6/PKG-INFO
--rw-r--r--   0 nusnus     (501) staff       (20)    13222 2024-03-27 13:05:32.000000 kombu-5.3.6/README.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      980 2022-09-28 15:48:06.000000 kombu-5.3.6/THANKS
--rw-r--r--   0 nusnus     (501) staff       (20)       82 2022-09-28 15:48:06.000000 kombu-5.3.6/TODO
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.280844 kombu-5.3.6/docs/
--rw-r--r--   0 nusnus     (501) staff       (20)     8009 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/Makefile
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.281110 kombu-5.3.6/docs/_ext/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/_ext/.keep
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.281250 kombu-5.3.6/docs/_static/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/_static/.keep
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.281371 kombu-5.3.6/docs/_templates/
--rw-r--r--   0 nusnus     (501) staff       (20)     3082 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/_templates/sidebardonations.html
--rw-r--r--   0 nusnus     (501) staff       (20)       30 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/changelog.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      938 2024-01-12 19:32:25.000000 kombu-5.3.6/docs/conf.py
--rw-r--r--   0 nusnus     (501) staff       (20)       20 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/faq.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.282017 kombu-5.3.6/docs/images/
--rw-r--r--   0 nusnus     (501) staff       (20)     5393 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/images/favicon.ico
--rw-r--r--   0 nusnus     (501) staff       (20)   115481 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/images/kombu.jpg
--rw-r--r--   0 nusnus     (501) staff       (20)    24746 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/images/kombusmall.jpg
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.282470 kombu-5.3.6/docs/includes/
--rw-r--r--   0 nusnus     (501) staff       (20)      453 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/includes/installation.txt
--rw-r--r--   0 nusnus     (501) staff       (20)    10596 2024-03-27 13:05:32.000000 kombu-5.3.6/docs/includes/introduction.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      726 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/includes/resources.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      303 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/index.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      216 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/introduction.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     7476 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/make.bat
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.291759 kombu-5.3.6/docs/reference/
--rw-r--r--   0 nusnus     (501) staff       (20)     2078 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/index.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      301 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.abstract.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      354 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.asynchronous.aws.connection.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      315 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.asynchronous.aws.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      353 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.asynchronous.aws.sqs.connection.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      340 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.asynchronous.aws.sqs.message.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      332 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.asynchronous.aws.sqs.queue.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      327 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.asynchronous.aws.sqs.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      324 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.asynchronous.debug.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      347 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.asynchronous.http.base.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      338 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.asynchronous.http.curl.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      312 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.asynchronous.http.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      317 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.asynchronous.hub.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      290 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.asynchronous.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      320 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.asynchronous.semaphore.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      303 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.asynchronous.timer.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      296 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.clocks.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      278 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.common.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      745 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.compat.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      513 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.compression.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      884 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.connection.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      461 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.exceptions.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      260 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.log.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      266 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.matcher.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      280 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.message.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      275 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.mixins.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     2335 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.pidbox.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      284 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.pools.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      287 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.resource.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     6031 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     1118 2022-10-19 10:47:33.000000 kombu-5.3.6/docs/reference/kombu.serialization.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     2045 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.simple.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      446 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.transport.SLMQ.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     2736 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.transport.SQS.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      533 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.transport.azureservicebus.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      557 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.transport.azurestoragequeues.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     1883 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.transport.base.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      605 2022-10-19 10:47:33.000000 kombu-5.3.6/docs/reference/kombu.transport.confluentkafka.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      459 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.transport.consul.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      451 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.transport.etcd.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      493 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.transport.filesystem.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      741 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.transport.librabbitmq.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      466 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.transport.memory.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      465 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.transport.mongodb.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      715 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.transport.pyamqp.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      535 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.transport.pyro.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      664 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.transport.qpid.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      576 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.transport.redis.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      543 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.transport.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     1152 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.transport.sqlalchemy.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      772 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.transport.virtual.exchange.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     2271 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.transport.virtual.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      484 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.transport.zookeeper.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      315 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.utils.amq_manager.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      313 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.utils.collections.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      300 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.utils.compat.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      296 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.utils.debug.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      284 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.utils.div.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      311 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.utils.encoding.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      302 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.utils.eventio.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      318 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.utils.functional.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      309 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.utils.imports.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      288 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.utils.json.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      293 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.utils.limits.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      308 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.utils.objects.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      293 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.utils.scheduling.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      289 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.utils.text.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      288 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.utils.time.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      260 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.utils.url.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      288 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/reference/kombu.utils.uuid.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.291894 kombu-5.3.6/docs/templates/
--rw-r--r--   0 nusnus     (501) staff       (20)     1262 2023-01-11 16:24:23.000000 kombu-5.3.6/docs/templates/readme.txt
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.293660 kombu-5.3.6/docs/userguide/
--rw-r--r--   0 nusnus     (501) staff       (20)     7817 2023-08-31 08:47:11.000000 kombu-5.3.6/docs/userguide/connections.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     7298 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/userguide/consumers.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     1047 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/userguide/examples.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     6726 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/userguide/failover.rst
--rw-r--r--   0 nusnus     (501) staff       (20)      232 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/userguide/index.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     3247 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/userguide/introduction.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     5458 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/userguide/pools.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     3635 2022-09-28 15:48:06.000000 kombu-5.3.6/docs/userguide/producers.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     6997 2023-04-14 11:55:19.000000 kombu-5.3.6/docs/userguide/serialization.rst
--rw-r--r--   0 nusnus     (501) staff       (20)     3916 2023-08-02 16:39:12.000000 kombu-5.3.6/docs/userguide/simple.rst
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.294778 kombu-5.3.6/examples/
--rw-r--r--   0 nusnus     (501) staff       (20)     1550 2022-10-19 10:47:33.000000 kombu-5.3.6/examples/complete_receive.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1174 2023-12-05 14:39:35.000000 kombu-5.3.6/examples/complete_send.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.294887 kombu-5.3.6/examples/experimental/
--rw-r--r--   0 nusnus     (501) staff       (20)      746 2023-05-25 11:07:02.000000 kombu-5.3.6/examples/experimental/async_consume.py
--rw-r--r--   0 nusnus     (501) staff       (20)      321 2022-10-19 10:47:33.000000 kombu-5.3.6/examples/hello_consumer.py
--rw-r--r--   0 nusnus     (501) staff       (20)      349 2022-10-19 10:47:33.000000 kombu-5.3.6/examples/hello_publisher.py
--rw-r--r--   0 nusnus     (501) staff       (20)      755 2022-10-19 10:47:33.000000 kombu-5.3.6/examples/memory_transport.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.295111 kombu-5.3.6/examples/rpc-tut6/
--rw-r--r--   0 nusnus     (501) staff       (20)     1447 2023-05-25 11:07:02.000000 kombu-5.3.6/examples/rpc-tut6/rpc_client.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1332 2023-05-25 11:07:02.000000 kombu-5.3.6/examples/rpc-tut6/rpc_server.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1225 2022-10-19 10:47:33.000000 kombu-5.3.6/examples/simple_eventlet_receive.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1181 2022-10-19 10:47:33.000000 kombu-5.3.6/examples/simple_eventlet_send.py
--rw-r--r--   0 nusnus     (501) staff       (20)      938 2022-10-19 10:47:33.000000 kombu-5.3.6/examples/simple_receive.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1001 2022-10-19 10:47:33.000000 kombu-5.3.6/examples/simple_send.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.295689 kombu-5.3.6/examples/simple_task_queue/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.6/examples/simple_task_queue/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)      994 2022-10-19 10:47:33.000000 kombu-5.3.6/examples/simple_task_queue/client.py
--rw-r--r--   0 nusnus     (501) staff       (20)      323 2022-10-19 10:47:33.000000 kombu-5.3.6/examples/simple_task_queue/queues.py
--rw-r--r--   0 nusnus     (501) staff       (20)       92 2022-10-19 10:47:33.000000 kombu-5.3.6/examples/simple_task_queue/tasks.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1276 2022-10-19 10:47:33.000000 kombu-5.3.6/examples/simple_task_queue/worker.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.299460 kombu-5.3.6/kombu/
--rw-r--r--   0 nusnus     (501) staff       (20)     3899 2024-03-27 13:05:32.000000 kombu-5.3.6/kombu/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4426 2023-05-15 03:09:16.000000 kombu-5.3.6/kombu/abstract.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.301063 kombu-5.3.6/kombu/asynchronous/
--rw-r--r--   0 nusnus     (501) staff       (20)      237 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/asynchronous/__init__.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.301587 kombu-5.3.6/kombu/asynchronous/aws/
--rw-r--r--   0 nusnus     (501) staff       (20)      475 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/asynchronous/aws/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8539 2023-11-28 12:45:32.000000 kombu-5.3.6/kombu/asynchronous/aws/connection.py
--rw-r--r--   0 nusnus     (501) staff       (20)      522 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/asynchronous/aws/ext.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.302268 kombu-5.3.6/kombu/asynchronous/aws/sqs/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.6/kombu/asynchronous/aws/sqs/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     9644 2023-11-28 12:45:32.000000 kombu-5.3.6/kombu/asynchronous/aws/sqs/connection.py
--rw-r--r--   0 nusnus     (501) staff       (20)      131 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/asynchronous/aws/sqs/ext.py
--rw-r--r--   0 nusnus     (501) staff       (20)      892 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/asynchronous/aws/sqs/message.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4402 2023-10-13 17:12:35.000000 kombu-5.3.6/kombu/asynchronous/aws/sqs/queue.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1773 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/asynchronous/debug.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.302770 kombu-5.3.6/kombu/asynchronous/http/
--rw-r--r--   0 nusnus     (501) staff       (20)      863 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/asynchronous/http/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     9592 2023-05-15 03:09:16.000000 kombu-5.3.6/kombu/asynchronous/http/base.py
--rw-r--r--   0 nusnus     (501) staff       (20)     9752 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/asynchronous/http/curl.py
--rw-r--r--   0 nusnus     (501) staff       (20)    11948 2024-01-08 15:56:44.000000 kombu-5.3.6/kombu/asynchronous/hub.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3521 2023-05-15 03:09:16.000000 kombu-5.3.6/kombu/asynchronous/semaphore.py
--rw-r--r--   0 nusnus     (501) staff       (20)     6922 2024-03-05 10:08:52.000000 kombu-5.3.6/kombu/asynchronous/timer.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4825 2023-05-15 03:09:16.000000 kombu-5.3.6/kombu/clocks.py
--rw-r--r--   0 nusnus     (501) staff       (20)    13529 2023-05-15 03:09:16.000000 kombu-5.3.6/kombu/common.py
--rw-r--r--   0 nusnus     (501) staff       (20)     6752 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/compat.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2984 2023-05-15 03:09:16.000000 kombu-5.3.6/kombu/compression.py
--rw-r--r--   0 nusnus     (501) staff       (20)    40494 2023-11-28 13:02:03.000000 kombu-5.3.6/kombu/connection.py
--rw-r--r--   0 nusnus     (501) staff       (20)    33201 2024-03-09 08:49:45.000000 kombu-5.3.6/kombu/entity.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2838 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/exceptions.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4066 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/log.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4269 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/matcher.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8151 2023-05-15 03:09:16.000000 kombu-5.3.6/kombu/message.py
--rw-r--r--   0 nusnus     (501) staff       (20)    24268 2023-08-31 08:47:11.000000 kombu-5.3.6/kombu/messaging.py
--rw-r--r--   0 nusnus     (501) staff       (20)     9701 2023-05-15 03:09:16.000000 kombu-5.3.6/kombu/mixins.py
--rw-r--r--   0 nusnus     (501) staff       (20)    14789 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/pidbox.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3975 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/pools.py
--rw-r--r--   0 nusnus     (501) staff       (20)     7735 2023-05-15 03:09:16.000000 kombu-5.3.6/kombu/resource.py
--rw-r--r--   0 nusnus     (501) staff       (20)    15446 2023-08-31 08:47:11.000000 kombu-5.3.6/kombu/serialization.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5302 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/simple.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.305849 kombu-5.3.6/kombu/transport/
--rw-r--r--   0 nusnus     (501) staff       (20)     6215 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/transport/SLMQ.py
--rw-r--r--   0 nusnus     (501) staff       (20)    34576 2023-10-13 17:12:35.000000 kombu-5.3.6/kombu/transport/SQS.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3342 2023-05-15 03:09:16.000000 kombu-5.3.6/kombu/transport/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    18174 2024-03-05 10:08:52.000000 kombu-5.3.6/kombu/transport/azureservicebus.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8894 2023-01-11 16:24:23.000000 kombu-5.3.6/kombu/transport/azurestoragequeues.py
--rw-r--r--   0 nusnus     (501) staff       (20)     7687 2023-05-15 03:09:16.000000 kombu-5.3.6/kombu/transport/base.py
--rw-r--r--   0 nusnus     (501) staff       (20)    12141 2023-11-28 12:45:32.000000 kombu-5.3.6/kombu/transport/confluentkafka.py
--rw-r--r--   0 nusnus     (501) staff       (20)     9424 2023-05-15 03:09:16.000000 kombu-5.3.6/kombu/transport/consul.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8644 2023-05-15 03:09:16.000000 kombu-5.3.6/kombu/transport/etcd.py
--rw-r--r--   0 nusnus     (501) staff       (20)    10416 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/transport/filesystem.py
--rw-r--r--   0 nusnus     (501) staff       (20)     6022 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/transport/librabbitmq.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2404 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/transport/memory.py
--rw-r--r--   0 nusnus     (501) staff       (20)    15446 2023-10-13 17:12:35.000000 kombu-5.3.6/kombu/transport/mongodb.py
--rw-r--r--   0 nusnus     (501) staff       (20)     7752 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/transport/pyamqp.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5844 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/transport/pyro.py
--rw-r--r--   0 nusnus     (501) staff       (20)    71681 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/transport/qpid.py
--rw-r--r--   0 nusnus     (501) staff       (20)    48720 2024-01-12 19:11:22.000000 kombu-5.3.6/kombu/transport/redis.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.306248 kombu-5.3.6/kombu/transport/sqlalchemy/
--rw-r--r--   0 nusnus     (501) staff       (20)     7448 2023-05-15 03:09:16.000000 kombu-5.3.6/kombu/transport/sqlalchemy/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2302 2023-02-14 14:21:21.000000 kombu-5.3.6/kombu/transport/sqlalchemy/models.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.306657 kombu-5.3.6/kombu/transport/virtual/
--rw-r--r--   0 nusnus     (501) staff       (20)      476 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/transport/virtual/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    34230 2024-01-08 15:56:44.000000 kombu-5.3.6/kombu/transport/virtual/base.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4894 2023-05-15 03:09:16.000000 kombu-5.3.6/kombu/transport/virtual/exchange.py
--rw-r--r--   0 nusnus     (501) staff       (20)     6339 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/transport/zookeeper.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.309477 kombu-5.3.6/kombu/utils/
--rw-r--r--   0 nusnus     (501) staff       (20)      698 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/utils/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)      716 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/utils/amq_manager.py
--rw-r--r--   0 nusnus     (501) staff       (20)      942 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/utils/collections.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3444 2023-05-25 11:07:02.000000 kombu-5.3.6/kombu/utils/compat.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1673 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/utils/debug.py
--rw-r--r--   0 nusnus     (501) staff       (20)      941 2024-01-08 15:56:44.000000 kombu-5.3.6/kombu/utils/div.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2297 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/utils/encoding.py
--rw-r--r--   0 nusnus     (501) staff       (20)    10159 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/utils/eventio.py
--rw-r--r--   0 nusnus     (501) staff       (20)    10699 2023-05-15 03:09:16.000000 kombu-5.3.6/kombu/utils/functional.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2089 2023-05-15 03:09:16.000000 kombu-5.3.6/kombu/utils/imports.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4088 2024-03-27 12:05:07.000000 kombu-5.3.6/kombu/utils/json.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2551 2023-05-15 03:09:16.000000 kombu-5.3.6/kombu/utils/limits.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2043 2023-11-28 12:45:32.000000 kombu-5.3.6/kombu/utils/objects.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2928 2023-05-15 03:09:16.000000 kombu-5.3.6/kombu/utils/scheduling.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2200 2023-05-15 03:09:16.000000 kombu-5.3.6/kombu/utils/text.py
--rw-r--r--   0 nusnus     (501) staff       (20)      272 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/utils/time.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3804 2022-10-19 10:47:33.000000 kombu-5.3.6/kombu/utils/url.py
--rw-r--r--   0 nusnus     (501) staff       (20)      327 2023-05-15 03:09:16.000000 kombu-5.3.6/kombu/utils/uuid.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.326396 kombu-5.3.6/kombu.egg-info/
--rw-r--r--   0 nusnus     (501) staff       (20)     3027 2024-03-27 13:06:01.000000 kombu-5.3.6/kombu.egg-info/PKG-INFO
--rw-r--r--   0 nusnus     (501) staff       (20)     9284 2024-03-27 13:06:01.000000 kombu-5.3.6/kombu.egg-info/SOURCES.txt
--rw-r--r--   0 nusnus     (501) staff       (20)        1 2024-03-27 13:06:01.000000 kombu-5.3.6/kombu.egg-info/dependency_links.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      783 2024-03-27 13:06:01.000000 kombu-5.3.6/kombu.egg-info/requires.txt
--rw-r--r--   0 nusnus     (501) staff       (20)        6 2024-03-27 13:06:01.000000 kombu-5.3.6/kombu.egg-info/top_level.txt
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.310515 kombu-5.3.6/requirements/
--rw-r--r--   0 nusnus     (501) staff       (20)      123 2023-06-18 20:37:05.000000 kombu-5.3.6/requirements/default.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       93 2023-01-11 16:24:23.000000 kombu-5.3.6/requirements/dev.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      243 2023-06-18 20:37:05.000000 kombu-5.3.6/requirements/docs.txt
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.313310 kombu-5.3.6/requirements/extras/
--rw-r--r--   0 nusnus     (501) staff       (20)       25 2023-05-15 03:09:16.000000 kombu-5.3.6/requirements/extras/azureservicebus.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       51 2023-04-14 11:55:19.000000 kombu-5.3.6/requirements/extras/azurestoragequeues.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      111 2023-04-14 11:55:19.000000 kombu-5.3.6/requirements/extras/brotli.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       23 2023-11-28 12:45:32.000000 kombu-5.3.6/requirements/extras/confluentkafka.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       15 2022-10-19 10:47:33.000000 kombu-5.3.6/requirements/extras/consul.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       10 2022-09-28 15:48:06.000000 kombu-5.3.6/requirements/extras/couchdb.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       19 2022-09-28 15:48:06.000000 kombu-5.3.6/requirements/extras/etcd.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       44 2023-06-18 20:37:05.000000 kombu-5.3.6/requirements/extras/librabbitmq.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       99 2023-06-18 20:37:05.000000 kombu-5.3.6/requirements/extras/lzma.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       15 2022-10-19 10:47:33.000000 kombu-5.3.6/requirements/extras/mongodb.txt
--rw-r--r--   0 nusnus     (501) staff       (20)        8 2022-09-28 15:48:06.000000 kombu-5.3.6/requirements/extras/msgpack.txt
--rw-r--r--   0 nusnus     (501) staff       (20)        6 2023-05-25 11:07:02.000000 kombu-5.3.6/requirements/extras/pyro.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       35 2022-09-28 15:48:06.000000 kombu-5.3.6/requirements/extras/qpid.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       29 2024-03-11 09:58:36.000000 kombu-5.3.6/requirements/extras/redis.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       27 2022-09-28 15:48:06.000000 kombu-5.3.6/requirements/extras/slmq.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       24 2023-05-15 03:09:16.000000 kombu-5.3.6/requirements/extras/sqlalchemy.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      121 2023-06-18 20:37:05.000000 kombu-5.3.6/requirements/extras/sqs.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       13 2022-09-28 15:48:06.000000 kombu-5.3.6/requirements/extras/yaml.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       13 2022-10-19 10:47:33.000000 kombu-5.3.6/requirements/extras/zookeeper.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       10 2022-09-28 15:48:06.000000 kombu-5.3.6/requirements/extras/zstd.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      191 2024-03-11 09:58:36.000000 kombu-5.3.6/requirements/funtest.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      116 2024-03-09 08:54:36.000000 kombu-5.3.6/requirements/pkgutils.txt
--rw-r--r--   0 nusnus     (501) staff       (20)      540 2024-03-27 12:05:07.000000 kombu-5.3.6/requirements/test-ci.txt
--rw-r--r--   0 nusnus     (501) staff       (20)       68 2024-03-11 09:37:32.000000 kombu-5.3.6/requirements/test.txt
--rw-r--r--   0 nusnus     (501) staff       (20)     1172 2024-03-27 13:06:01.328599 kombu-5.3.6/setup.cfg
--rw-r--r--   0 nusnus     (501) staff       (20)     3937 2023-11-28 12:45:32.000000 kombu-5.3.6/setup.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.313756 kombu-5.3.6/t/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.6/t/__init__.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.314598 kombu-5.3.6/t/integration/
--rw-r--r--   0 nusnus     (501) staff       (20)      120 2022-10-19 10:47:33.000000 kombu-5.3.6/t/integration/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    17367 2022-10-19 10:47:33.000000 kombu-5.3.6/t/integration/common.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1464 2022-10-19 10:47:33.000000 kombu-5.3.6/t/integration/test_kafka.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3675 2022-10-19 10:47:33.000000 kombu-5.3.6/t/integration/test_mongodb.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1970 2022-10-19 10:47:33.000000 kombu-5.3.6/t/integration/test_py_amqp.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4996 2023-06-18 20:37:05.000000 kombu-5.3.6/t/integration/test_redis.py
--rw-r--r--   0 nusnus     (501) staff       (20)     6008 2022-10-19 10:47:33.000000 kombu-5.3.6/t/mocks.py
--rw-r--r--   0 nusnus     (501) staff       (20)      283 2022-10-19 10:47:33.000000 kombu-5.3.6/t/skip.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.317515 kombu-5.3.6/t/unit/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.6/t/unit/__init__.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.318164 kombu-5.3.6/t/unit/asynchronous/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.6/t/unit/asynchronous/__init__.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.318849 kombu-5.3.6/t/unit/asynchronous/aws/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.6/t/unit/asynchronous/aws/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)      199 2022-10-19 10:47:33.000000 kombu-5.3.6/t/unit/asynchronous/aws/case.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.319339 kombu-5.3.6/t/unit/asynchronous/aws/sqs/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.6/t/unit/asynchronous/aws/sqs/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    16807 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/asynchronous/aws/sqs/test_connection.py
--rw-r--r--   0 nusnus     (501) staff       (20)     7147 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/asynchronous/aws/sqs/test_queue.py
--rw-r--r--   0 nusnus     (501) staff       (20)      318 2022-10-19 10:47:33.000000 kombu-5.3.6/t/unit/asynchronous/aws/test_aws.py
--rw-r--r--   0 nusnus     (501) staff       (20)     9284 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/asynchronous/aws/test_connection.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.319879 kombu-5.3.6/t/unit/asynchronous/http/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.6/t/unit/asynchronous/http/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5728 2022-10-19 10:47:33.000000 kombu-5.3.6/t/unit/asynchronous/http/test_curl.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4221 2022-10-19 10:47:33.000000 kombu-5.3.6/t/unit/asynchronous/http/test_http.py
--rw-r--r--   0 nusnus     (501) staff       (20)    17688 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/asynchronous/test_hub.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1141 2022-10-19 10:47:33.000000 kombu-5.3.6/t/unit/asynchronous/test_semaphore.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4247 2022-10-19 10:47:33.000000 kombu-5.3.6/t/unit/asynchronous/test_timer.py
--rw-r--r--   0 nusnus     (501) staff       (20)     9493 2022-10-19 10:47:33.000000 kombu-5.3.6/t/unit/conftest.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2359 2022-10-19 10:47:33.000000 kombu-5.3.6/t/unit/test_clocks.py
--rw-r--r--   0 nusnus     (501) staff       (20)    17580 2022-10-19 10:47:33.000000 kombu-5.3.6/t/unit/test_common.py
--rw-r--r--   0 nusnus     (501) staff       (20)    11202 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/test_compat.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2858 2022-10-19 10:47:33.000000 kombu-5.3.6/t/unit/test_compression.py
--rw-r--r--   0 nusnus     (501) staff       (20)    32471 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/test_connection.py
--rw-r--r--   0 nusnus     (501) staff       (20)    14216 2024-03-09 08:49:45.000000 kombu-5.3.6/t/unit/test_entity.py
--rw-r--r--   0 nusnus     (501) staff       (20)      229 2022-10-19 10:47:33.000000 kombu-5.3.6/t/unit/test_exceptions.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4803 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/test_log.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1133 2022-10-19 10:47:33.000000 kombu-5.3.6/t/unit/test_matcher.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1285 2022-10-19 10:47:33.000000 kombu-5.3.6/t/unit/test_message.py
--rw-r--r--   0 nusnus     (501) staff       (20)    24495 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/test_messaging.py
--rw-r--r--   0 nusnus     (501) staff       (20)     7882 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/test_mixins.py
--rw-r--r--   0 nusnus     (501) staff       (20)    12550 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/test_pidbox.py
--rw-r--r--   0 nusnus     (501) staff       (20)     7245 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/test_pools.py
--rw-r--r--   0 nusnus     (501) staff       (20)    11162 2022-10-19 10:47:33.000000 kombu-5.3.6/t/unit/test_serialization.py
--rw-r--r--   0 nusnus     (501) staff       (20)     6718 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/test_simple.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.323229 kombu-5.3.6/t/unit/transport/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.6/t/unit/transport/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    36583 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/transport/test_SQS.py
--rw-r--r--   0 nusnus     (501) staff       (20)    15613 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/transport/test_azureservicebus.py
--rw-r--r--   0 nusnus     (501) staff       (20)     3455 2023-01-11 16:24:23.000000 kombu-5.3.6/t/unit/transport/test_azurestoragequeues.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5631 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/transport/test_base.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2681 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/transport/test_consul.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2204 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/transport/test_etcd.py
--rw-r--r--   0 nusnus     (501) staff       (20)    10636 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/transport/test_filesystem.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4898 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/transport/test_librabbitmq.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5650 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/transport/test_memory.py
--rw-r--r--   0 nusnus     (501) staff       (20)    19745 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/transport/test_mongodb.py
--rw-r--r--   0 nusnus     (501) staff       (20)     7300 2024-03-09 08:49:45.000000 kombu-5.3.6/t/unit/transport/test_pyamqp.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2899 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/transport/test_pyro.py
--rw-r--r--   0 nusnus     (501) staff       (20)    71136 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/transport/test_qpid.py
--rw-r--r--   0 nusnus     (501) staff       (20)    62182 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/transport/test_redis.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1538 2022-10-19 10:47:33.000000 kombu-5.3.6/t/unit/transport/test_sqlalchemy.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1014 2022-10-19 10:47:33.000000 kombu-5.3.6/t/unit/transport/test_transport.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1071 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/transport/test_zookeeper.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.323595 kombu-5.3.6/t/unit/transport/virtual/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.6/t/unit/transport/virtual/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)    21287 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/transport/virtual/test_base.py
--rw-r--r--   0 nusnus     (501) staff       (20)     5565 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/transport/virtual/test_exchange.py
-drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-03-27 13:06:01.326108 kombu-5.3.6/t/unit/utils/
--rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.6/t/unit/utils/__init__.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1281 2022-10-19 10:47:33.000000 kombu-5.3.6/t/unit/utils/test_amq_manager.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2806 2023-04-14 11:55:19.000000 kombu-5.3.6/t/unit/utils/test_compat.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1630 2022-10-19 10:47:33.000000 kombu-5.3.6/t/unit/utils/test_debug.py
--rw-r--r--   0 nusnus     (501) staff       (20)     1132 2022-10-19 10:47:33.000000 kombu-5.3.6/t/unit/utils/test_div.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2969 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/utils/test_encoding.py
--rw-r--r--   0 nusnus     (501) staff       (20)     8807 2024-03-05 10:08:52.000000 kombu-5.3.6/t/unit/utils/test_functional.py
--rw-r--r--   0 nusnus     (501) staff       (20)      967 2022-10-19 10:47:33.000000 kombu-5.3.6/t/unit/utils/test_imports.py
--rw-r--r--   0 nusnus     (501) staff       (20)     4698 2024-03-27 12:05:07.000000 kombu-5.3.6/t/unit/utils/test_json.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2091 2023-11-28 12:45:32.000000 kombu-5.3.6/t/unit/utils/test_objects.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2769 2022-10-19 10:47:33.000000 kombu-5.3.6/t/unit/utils/test_scheduling.py
--rw-r--r--   0 nusnus     (501) staff       (20)      459 2022-10-19 10:47:33.000000 kombu-5.3.6/t/unit/utils/test_time.py
--rw-r--r--   0 nusnus     (501) staff       (20)     2964 2022-10-19 10:47:33.000000 kombu-5.3.6/t/unit/utils/test_url.py
--rw-r--r--   0 nusnus     (501) staff       (20)      609 2022-10-19 10:47:33.000000 kombu-5.3.6/t/unit/utils/test_utils.py
--rw-r--r--   0 nusnus     (501) staff       (20)      289 2022-10-19 10:47:33.000000 kombu-5.3.6/t/unit/utils/test_uuid.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.600473 kombu-5.3.7/
+-rw-r--r--   0 nusnus     (501) staff       (20)     5599 2022-10-19 10:47:33.000000 kombu-5.3.7/AUTHORS
+-rw-r--r--   0 nusnus     (501) staff       (20)      436 2022-09-28 15:48:06.000000 kombu-5.3.7/FAQ
+-rw-r--r--   0 nusnus     (501) staff       (20)      387 2022-09-28 15:48:06.000000 kombu-5.3.7/INSTALL
+-rw-r--r--   0 nusnus     (501) staff       (20)     1664 2022-09-28 15:48:06.000000 kombu-5.3.7/LICENSE
+-rw-r--r--   0 nusnus     (501) staff       (20)      515 2022-09-28 15:48:06.000000 kombu-5.3.7/MANIFEST.in
+-rw-r--r--   0 nusnus     (501) staff       (20)     3027 2024-04-11 12:14:51.600339 kombu-5.3.7/PKG-INFO
+-rw-r--r--   0 nusnus     (501) staff       (20)    13222 2024-04-11 12:08:57.000000 kombu-5.3.7/README.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      980 2022-09-28 15:48:06.000000 kombu-5.3.7/THANKS
+-rw-r--r--   0 nusnus     (501) staff       (20)       82 2022-09-28 15:48:06.000000 kombu-5.3.7/TODO
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.551510 kombu-5.3.7/docs/
+-rw-r--r--   0 nusnus     (501) staff       (20)     8009 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/Makefile
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.551655 kombu-5.3.7/docs/_ext/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/_ext/.keep
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.551766 kombu-5.3.7/docs/_static/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/_static/.keep
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.551868 kombu-5.3.7/docs/_templates/
+-rw-r--r--   0 nusnus     (501) staff       (20)     3082 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/_templates/sidebardonations.html
+-rw-r--r--   0 nusnus     (501) staff       (20)       30 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/changelog.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      938 2024-01-12 19:32:25.000000 kombu-5.3.7/docs/conf.py
+-rw-r--r--   0 nusnus     (501) staff       (20)       20 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/faq.rst
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.552355 kombu-5.3.7/docs/images/
+-rw-r--r--   0 nusnus     (501) staff       (20)     5393 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/images/favicon.ico
+-rw-r--r--   0 nusnus     (501) staff       (20)   115481 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/images/kombu.jpg
+-rw-r--r--   0 nusnus     (501) staff       (20)    24746 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/images/kombusmall.jpg
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.552846 kombu-5.3.7/docs/includes/
+-rw-r--r--   0 nusnus     (501) staff       (20)      453 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/includes/installation.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)    10596 2024-04-11 12:08:57.000000 kombu-5.3.7/docs/includes/introduction.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)      726 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/includes/resources.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)      303 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/index.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      216 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/introduction.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     7476 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/make.bat
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.563267 kombu-5.3.7/docs/reference/
+-rw-r--r--   0 nusnus     (501) staff       (20)     2078 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/index.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      301 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.abstract.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      354 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.asynchronous.aws.connection.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      315 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.asynchronous.aws.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      353 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.asynchronous.aws.sqs.connection.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      340 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.asynchronous.aws.sqs.message.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      332 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.asynchronous.aws.sqs.queue.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      327 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.asynchronous.aws.sqs.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      324 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.asynchronous.debug.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      347 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.asynchronous.http.base.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      338 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.asynchronous.http.curl.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      312 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.asynchronous.http.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      317 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.asynchronous.hub.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      290 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.asynchronous.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      320 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.asynchronous.semaphore.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      303 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.asynchronous.timer.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      296 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.clocks.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      278 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.common.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      745 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.compat.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      513 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.compression.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      884 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.connection.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      461 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.exceptions.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      260 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.log.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      266 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.matcher.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      280 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.message.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      275 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.mixins.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     2335 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.pidbox.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      284 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.pools.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      287 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.resource.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     6031 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     1118 2022-10-19 10:47:33.000000 kombu-5.3.7/docs/reference/kombu.serialization.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     2045 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.simple.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      446 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.transport.SLMQ.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     2736 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.transport.SQS.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      533 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.transport.azureservicebus.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      557 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.transport.azurestoragequeues.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     1883 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.transport.base.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      605 2022-10-19 10:47:33.000000 kombu-5.3.7/docs/reference/kombu.transport.confluentkafka.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      459 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.transport.consul.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      451 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.transport.etcd.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      493 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.transport.filesystem.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      741 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.transport.librabbitmq.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      466 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.transport.memory.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      465 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.transport.mongodb.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      715 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.transport.pyamqp.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      535 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.transport.pyro.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      664 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.transport.qpid.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      576 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.transport.redis.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      543 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.transport.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     1152 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.transport.sqlalchemy.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      772 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.transport.virtual.exchange.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     2271 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.transport.virtual.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      484 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.transport.zookeeper.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      315 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.utils.amq_manager.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      313 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.utils.collections.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      300 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.utils.compat.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      296 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.utils.debug.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      284 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.utils.div.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      311 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.utils.encoding.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      302 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.utils.eventio.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      318 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.utils.functional.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      309 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.utils.imports.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      288 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.utils.json.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      293 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.utils.limits.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      308 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.utils.objects.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      293 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.utils.scheduling.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      289 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.utils.text.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      288 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.utils.time.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      260 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.utils.url.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      288 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/reference/kombu.utils.uuid.rst
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.563416 kombu-5.3.7/docs/templates/
+-rw-r--r--   0 nusnus     (501) staff       (20)     1262 2023-01-11 16:24:23.000000 kombu-5.3.7/docs/templates/readme.txt
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.564981 kombu-5.3.7/docs/userguide/
+-rw-r--r--   0 nusnus     (501) staff       (20)     7817 2023-08-31 08:47:11.000000 kombu-5.3.7/docs/userguide/connections.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     7298 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/userguide/consumers.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     1047 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/userguide/examples.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     6726 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/userguide/failover.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)      232 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/userguide/index.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     3247 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/userguide/introduction.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     5458 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/userguide/pools.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     3635 2022-09-28 15:48:06.000000 kombu-5.3.7/docs/userguide/producers.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     6997 2023-04-14 11:55:19.000000 kombu-5.3.7/docs/userguide/serialization.rst
+-rw-r--r--   0 nusnus     (501) staff       (20)     3916 2023-08-02 16:39:12.000000 kombu-5.3.7/docs/userguide/simple.rst
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.566257 kombu-5.3.7/examples/
+-rw-r--r--   0 nusnus     (501) staff       (20)     1550 2022-10-19 10:47:33.000000 kombu-5.3.7/examples/complete_receive.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1174 2023-12-05 14:39:35.000000 kombu-5.3.7/examples/complete_send.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.566420 kombu-5.3.7/examples/experimental/
+-rw-r--r--   0 nusnus     (501) staff       (20)      746 2023-05-25 11:07:02.000000 kombu-5.3.7/examples/experimental/async_consume.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      321 2022-10-19 10:47:33.000000 kombu-5.3.7/examples/hello_consumer.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      349 2022-10-19 10:47:33.000000 kombu-5.3.7/examples/hello_publisher.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      755 2022-10-19 10:47:33.000000 kombu-5.3.7/examples/memory_transport.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.566711 kombu-5.3.7/examples/rpc-tut6/
+-rw-r--r--   0 nusnus     (501) staff       (20)     1447 2023-05-25 11:07:02.000000 kombu-5.3.7/examples/rpc-tut6/rpc_client.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1332 2023-05-25 11:07:02.000000 kombu-5.3.7/examples/rpc-tut6/rpc_server.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1225 2022-10-19 10:47:33.000000 kombu-5.3.7/examples/simple_eventlet_receive.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1181 2022-10-19 10:47:33.000000 kombu-5.3.7/examples/simple_eventlet_send.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      938 2022-10-19 10:47:33.000000 kombu-5.3.7/examples/simple_receive.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1001 2022-10-19 10:47:33.000000 kombu-5.3.7/examples/simple_send.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.567359 kombu-5.3.7/examples/simple_task_queue/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.7/examples/simple_task_queue/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      994 2022-10-19 10:47:33.000000 kombu-5.3.7/examples/simple_task_queue/client.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      323 2022-10-19 10:47:33.000000 kombu-5.3.7/examples/simple_task_queue/queues.py
+-rw-r--r--   0 nusnus     (501) staff       (20)       92 2022-10-19 10:47:33.000000 kombu-5.3.7/examples/simple_task_queue/tasks.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1276 2022-10-19 10:47:33.000000 kombu-5.3.7/examples/simple_task_queue/worker.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.571351 kombu-5.3.7/kombu/
+-rw-r--r--   0 nusnus     (501) staff       (20)     3899 2024-04-11 12:08:57.000000 kombu-5.3.7/kombu/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4426 2023-05-15 03:09:16.000000 kombu-5.3.7/kombu/abstract.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.572742 kombu-5.3.7/kombu/asynchronous/
+-rw-r--r--   0 nusnus     (501) staff       (20)      237 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/asynchronous/__init__.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.573200 kombu-5.3.7/kombu/asynchronous/aws/
+-rw-r--r--   0 nusnus     (501) staff       (20)      475 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/asynchronous/aws/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     8539 2023-11-28 12:45:32.000000 kombu-5.3.7/kombu/asynchronous/aws/connection.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      522 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/asynchronous/aws/ext.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.573850 kombu-5.3.7/kombu/asynchronous/aws/sqs/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.7/kombu/asynchronous/aws/sqs/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     9644 2023-11-28 12:45:32.000000 kombu-5.3.7/kombu/asynchronous/aws/sqs/connection.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      131 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/asynchronous/aws/sqs/ext.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      892 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/asynchronous/aws/sqs/message.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4402 2023-10-13 17:12:35.000000 kombu-5.3.7/kombu/asynchronous/aws/sqs/queue.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1773 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/asynchronous/debug.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.574276 kombu-5.3.7/kombu/asynchronous/http/
+-rw-r--r--   0 nusnus     (501) staff       (20)      863 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/asynchronous/http/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     9592 2023-05-15 03:09:16.000000 kombu-5.3.7/kombu/asynchronous/http/base.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     9752 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/asynchronous/http/curl.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    11948 2024-01-08 15:56:44.000000 kombu-5.3.7/kombu/asynchronous/hub.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3521 2023-05-15 03:09:16.000000 kombu-5.3.7/kombu/asynchronous/semaphore.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     6922 2024-03-05 10:08:52.000000 kombu-5.3.7/kombu/asynchronous/timer.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4825 2023-05-15 03:09:16.000000 kombu-5.3.7/kombu/clocks.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    13529 2023-05-15 03:09:16.000000 kombu-5.3.7/kombu/common.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     6752 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/compat.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2984 2023-05-15 03:09:16.000000 kombu-5.3.7/kombu/compression.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    40494 2023-11-28 13:02:03.000000 kombu-5.3.7/kombu/connection.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    33201 2024-03-09 08:49:45.000000 kombu-5.3.7/kombu/entity.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2838 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/exceptions.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4066 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/log.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4269 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/matcher.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     8151 2023-05-15 03:09:16.000000 kombu-5.3.7/kombu/message.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    24268 2023-08-31 08:47:11.000000 kombu-5.3.7/kombu/messaging.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     9701 2023-05-15 03:09:16.000000 kombu-5.3.7/kombu/mixins.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    14789 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/pidbox.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3975 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/pools.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     7735 2023-05-15 03:09:16.000000 kombu-5.3.7/kombu/resource.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    15446 2023-08-31 08:47:11.000000 kombu-5.3.7/kombu/serialization.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     5302 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/simple.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.577125 kombu-5.3.7/kombu/transport/
+-rw-r--r--   0 nusnus     (501) staff       (20)     6215 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/transport/SLMQ.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    34576 2023-10-13 17:12:35.000000 kombu-5.3.7/kombu/transport/SQS.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3342 2023-05-15 03:09:16.000000 kombu-5.3.7/kombu/transport/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    18174 2024-03-05 10:08:52.000000 kombu-5.3.7/kombu/transport/azureservicebus.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     8894 2023-01-11 16:24:23.000000 kombu-5.3.7/kombu/transport/azurestoragequeues.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     7687 2023-05-15 03:09:16.000000 kombu-5.3.7/kombu/transport/base.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    12141 2023-11-28 12:45:32.000000 kombu-5.3.7/kombu/transport/confluentkafka.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     9424 2023-05-15 03:09:16.000000 kombu-5.3.7/kombu/transport/consul.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     8644 2023-05-15 03:09:16.000000 kombu-5.3.7/kombu/transport/etcd.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    10416 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/transport/filesystem.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     6022 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/transport/librabbitmq.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2404 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/transport/memory.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    15446 2023-10-13 17:12:35.000000 kombu-5.3.7/kombu/transport/mongodb.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     7752 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/transport/pyamqp.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     5844 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/transport/pyro.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    71681 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/transport/qpid.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    48720 2024-01-12 19:11:22.000000 kombu-5.3.7/kombu/transport/redis.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.577599 kombu-5.3.7/kombu/transport/sqlalchemy/
+-rw-r--r--   0 nusnus     (501) staff       (20)     7448 2023-05-15 03:09:16.000000 kombu-5.3.7/kombu/transport/sqlalchemy/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2302 2023-02-14 14:21:21.000000 kombu-5.3.7/kombu/transport/sqlalchemy/models.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.578078 kombu-5.3.7/kombu/transport/virtual/
+-rw-r--r--   0 nusnus     (501) staff       (20)      476 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/transport/virtual/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    34230 2024-01-08 15:56:44.000000 kombu-5.3.7/kombu/transport/virtual/base.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4894 2023-05-15 03:09:16.000000 kombu-5.3.7/kombu/transport/virtual/exchange.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     6339 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/transport/zookeeper.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.580739 kombu-5.3.7/kombu/utils/
+-rw-r--r--   0 nusnus     (501) staff       (20)      698 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/utils/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      716 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/utils/amq_manager.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      942 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/utils/collections.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3444 2023-05-25 11:07:02.000000 kombu-5.3.7/kombu/utils/compat.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1673 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/utils/debug.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      941 2024-01-08 15:56:44.000000 kombu-5.3.7/kombu/utils/div.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2297 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/utils/encoding.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    10159 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/utils/eventio.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    10699 2023-05-15 03:09:16.000000 kombu-5.3.7/kombu/utils/functional.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2089 2023-05-15 03:09:16.000000 kombu-5.3.7/kombu/utils/imports.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4088 2024-03-27 12:05:07.000000 kombu-5.3.7/kombu/utils/json.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2551 2023-05-15 03:09:16.000000 kombu-5.3.7/kombu/utils/limits.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2043 2023-11-28 12:45:32.000000 kombu-5.3.7/kombu/utils/objects.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2928 2023-05-15 03:09:16.000000 kombu-5.3.7/kombu/utils/scheduling.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2200 2023-05-15 03:09:16.000000 kombu-5.3.7/kombu/utils/text.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      272 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/utils/time.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3804 2022-10-19 10:47:33.000000 kombu-5.3.7/kombu/utils/url.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      327 2023-05-15 03:09:16.000000 kombu-5.3.7/kombu/utils/uuid.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.598451 kombu-5.3.7/kombu.egg-info/
+-rw-r--r--   0 nusnus     (501) staff       (20)     3027 2024-04-11 12:14:51.000000 kombu-5.3.7/kombu.egg-info/PKG-INFO
+-rw-r--r--   0 nusnus     (501) staff       (20)     9284 2024-04-11 12:14:51.000000 kombu-5.3.7/kombu.egg-info/SOURCES.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)        1 2024-04-11 12:14:51.000000 kombu-5.3.7/kombu.egg-info/dependency_links.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)      783 2024-04-11 12:14:51.000000 kombu-5.3.7/kombu.egg-info/requires.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)        6 2024-04-11 12:14:51.000000 kombu-5.3.7/kombu.egg-info/top_level.txt
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.581634 kombu-5.3.7/requirements/
+-rw-r--r--   0 nusnus     (501) staff       (20)      123 2023-06-18 20:37:05.000000 kombu-5.3.7/requirements/default.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       93 2023-01-11 16:24:23.000000 kombu-5.3.7/requirements/dev.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)      243 2023-06-18 20:37:05.000000 kombu-5.3.7/requirements/docs.txt
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.584437 kombu-5.3.7/requirements/extras/
+-rw-r--r--   0 nusnus     (501) staff       (20)       25 2023-05-15 03:09:16.000000 kombu-5.3.7/requirements/extras/azureservicebus.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       51 2023-04-14 11:55:19.000000 kombu-5.3.7/requirements/extras/azurestoragequeues.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)      111 2023-04-14 11:55:19.000000 kombu-5.3.7/requirements/extras/brotli.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       23 2023-11-28 12:45:32.000000 kombu-5.3.7/requirements/extras/confluentkafka.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       15 2022-10-19 10:47:33.000000 kombu-5.3.7/requirements/extras/consul.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       10 2022-09-28 15:48:06.000000 kombu-5.3.7/requirements/extras/couchdb.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       19 2022-09-28 15:48:06.000000 kombu-5.3.7/requirements/extras/etcd.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       44 2023-06-18 20:37:05.000000 kombu-5.3.7/requirements/extras/librabbitmq.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       99 2023-06-18 20:37:05.000000 kombu-5.3.7/requirements/extras/lzma.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       15 2022-10-19 10:47:33.000000 kombu-5.3.7/requirements/extras/mongodb.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)        8 2022-09-28 15:48:06.000000 kombu-5.3.7/requirements/extras/msgpack.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)        6 2023-05-25 11:07:02.000000 kombu-5.3.7/requirements/extras/pyro.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       35 2022-09-28 15:48:06.000000 kombu-5.3.7/requirements/extras/qpid.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       29 2024-03-11 09:58:36.000000 kombu-5.3.7/requirements/extras/redis.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       27 2022-09-28 15:48:06.000000 kombu-5.3.7/requirements/extras/slmq.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       24 2023-05-15 03:09:16.000000 kombu-5.3.7/requirements/extras/sqlalchemy.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)      121 2023-06-18 20:37:05.000000 kombu-5.3.7/requirements/extras/sqs.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       13 2022-09-28 15:48:06.000000 kombu-5.3.7/requirements/extras/yaml.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       13 2022-10-19 10:47:33.000000 kombu-5.3.7/requirements/extras/zookeeper.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       10 2022-09-28 15:48:06.000000 kombu-5.3.7/requirements/extras/zstd.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)      191 2024-03-11 09:58:36.000000 kombu-5.3.7/requirements/funtest.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)      116 2024-03-09 08:54:36.000000 kombu-5.3.7/requirements/pkgutils.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)      540 2024-03-27 12:05:07.000000 kombu-5.3.7/requirements/test-ci.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)       68 2024-03-11 09:37:32.000000 kombu-5.3.7/requirements/test.txt
+-rw-r--r--   0 nusnus     (501) staff       (20)     1172 2024-04-11 12:14:51.600866 kombu-5.3.7/setup.cfg
+-rw-r--r--   0 nusnus     (501) staff       (20)     3937 2023-11-28 12:45:32.000000 kombu-5.3.7/setup.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.584794 kombu-5.3.7/t/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.7/t/__init__.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.586262 kombu-5.3.7/t/integration/
+-rw-r--r--   0 nusnus     (501) staff       (20)      120 2022-10-19 10:47:33.000000 kombu-5.3.7/t/integration/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    17367 2022-10-19 10:47:33.000000 kombu-5.3.7/t/integration/common.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1464 2022-10-19 10:47:33.000000 kombu-5.3.7/t/integration/test_kafka.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3675 2022-10-19 10:47:33.000000 kombu-5.3.7/t/integration/test_mongodb.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1970 2022-10-19 10:47:33.000000 kombu-5.3.7/t/integration/test_py_amqp.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4996 2023-06-18 20:37:05.000000 kombu-5.3.7/t/integration/test_redis.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     6008 2022-10-19 10:47:33.000000 kombu-5.3.7/t/mocks.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      283 2022-10-19 10:47:33.000000 kombu-5.3.7/t/skip.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.589577 kombu-5.3.7/t/unit/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.7/t/unit/__init__.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.590088 kombu-5.3.7/t/unit/asynchronous/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.7/t/unit/asynchronous/__init__.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.590874 kombu-5.3.7/t/unit/asynchronous/aws/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.7/t/unit/asynchronous/aws/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      199 2022-10-19 10:47:33.000000 kombu-5.3.7/t/unit/asynchronous/aws/case.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.591387 kombu-5.3.7/t/unit/asynchronous/aws/sqs/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.7/t/unit/asynchronous/aws/sqs/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    16807 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/asynchronous/aws/sqs/test_connection.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     7147 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/asynchronous/aws/sqs/test_queue.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      318 2022-10-19 10:47:33.000000 kombu-5.3.7/t/unit/asynchronous/aws/test_aws.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     9284 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/asynchronous/aws/test_connection.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.591810 kombu-5.3.7/t/unit/asynchronous/http/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.7/t/unit/asynchronous/http/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     5728 2022-10-19 10:47:33.000000 kombu-5.3.7/t/unit/asynchronous/http/test_curl.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4221 2022-10-19 10:47:33.000000 kombu-5.3.7/t/unit/asynchronous/http/test_http.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    17688 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/asynchronous/test_hub.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1141 2022-10-19 10:47:33.000000 kombu-5.3.7/t/unit/asynchronous/test_semaphore.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4247 2022-10-19 10:47:33.000000 kombu-5.3.7/t/unit/asynchronous/test_timer.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     9493 2022-10-19 10:47:33.000000 kombu-5.3.7/t/unit/conftest.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2359 2022-10-19 10:47:33.000000 kombu-5.3.7/t/unit/test_clocks.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    17580 2022-10-19 10:47:33.000000 kombu-5.3.7/t/unit/test_common.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    11202 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/test_compat.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2858 2022-10-19 10:47:33.000000 kombu-5.3.7/t/unit/test_compression.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    32471 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/test_connection.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    14216 2024-03-09 08:49:45.000000 kombu-5.3.7/t/unit/test_entity.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      229 2022-10-19 10:47:33.000000 kombu-5.3.7/t/unit/test_exceptions.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4803 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/test_log.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1133 2022-10-19 10:47:33.000000 kombu-5.3.7/t/unit/test_matcher.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1285 2022-10-19 10:47:33.000000 kombu-5.3.7/t/unit/test_message.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    24495 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/test_messaging.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     7882 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/test_mixins.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    12550 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/test_pidbox.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     7245 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/test_pools.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    11162 2022-10-19 10:47:33.000000 kombu-5.3.7/t/unit/test_serialization.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     6718 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/test_simple.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.595540 kombu-5.3.7/t/unit/transport/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.7/t/unit/transport/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    36583 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/transport/test_SQS.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    15613 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/transport/test_azureservicebus.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     3455 2023-01-11 16:24:23.000000 kombu-5.3.7/t/unit/transport/test_azurestoragequeues.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     5631 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/transport/test_base.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2681 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/transport/test_consul.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2204 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/transport/test_etcd.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    10636 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/transport/test_filesystem.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4898 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/transport/test_librabbitmq.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     5650 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/transport/test_memory.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    19745 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/transport/test_mongodb.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     7300 2024-03-09 08:49:45.000000 kombu-5.3.7/t/unit/transport/test_pyamqp.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2899 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/transport/test_pyro.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    71136 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/transport/test_qpid.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    62182 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/transport/test_redis.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1538 2022-10-19 10:47:33.000000 kombu-5.3.7/t/unit/transport/test_sqlalchemy.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1014 2022-10-19 10:47:33.000000 kombu-5.3.7/t/unit/transport/test_transport.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1071 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/transport/test_zookeeper.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.596057 kombu-5.3.7/t/unit/transport/virtual/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.7/t/unit/transport/virtual/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)    21287 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/transport/virtual/test_base.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     5565 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/transport/virtual/test_exchange.py
+drwxr-xr-x   0 nusnus     (501) staff       (20)        0 2024-04-11 12:14:51.598262 kombu-5.3.7/t/unit/utils/
+-rw-r--r--   0 nusnus     (501) staff       (20)        0 2022-09-28 15:48:06.000000 kombu-5.3.7/t/unit/utils/__init__.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1281 2022-10-19 10:47:33.000000 kombu-5.3.7/t/unit/utils/test_amq_manager.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2806 2023-04-14 11:55:19.000000 kombu-5.3.7/t/unit/utils/test_compat.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1630 2022-10-19 10:47:33.000000 kombu-5.3.7/t/unit/utils/test_debug.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     1132 2022-10-19 10:47:33.000000 kombu-5.3.7/t/unit/utils/test_div.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2969 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/utils/test_encoding.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     8807 2024-03-05 10:08:52.000000 kombu-5.3.7/t/unit/utils/test_functional.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      967 2022-10-19 10:47:33.000000 kombu-5.3.7/t/unit/utils/test_imports.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     4698 2024-03-27 12:05:07.000000 kombu-5.3.7/t/unit/utils/test_json.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2091 2023-11-28 12:45:32.000000 kombu-5.3.7/t/unit/utils/test_objects.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2769 2022-10-19 10:47:33.000000 kombu-5.3.7/t/unit/utils/test_scheduling.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      459 2022-10-19 10:47:33.000000 kombu-5.3.7/t/unit/utils/test_time.py
+-rw-r--r--   0 nusnus     (501) staff       (20)     2964 2022-10-19 10:47:33.000000 kombu-5.3.7/t/unit/utils/test_url.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      609 2022-10-19 10:47:33.000000 kombu-5.3.7/t/unit/utils/test_utils.py
+-rw-r--r--   0 nusnus     (501) staff       (20)      289 2022-10-19 10:47:33.000000 kombu-5.3.7/t/unit/utils/test_uuid.py
```

### Comparing `kombu-5.3.6/AUTHORS` & `kombu-5.3.7/AUTHORS`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/LICENSE` & `kombu-5.3.7/LICENSE`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/MANIFEST.in` & `kombu-5.3.7/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/PKG-INFO` & `kombu-5.3.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kombu
-Version: 5.3.6
+Version: 5.3.7
 Summary: Messaging library for Python.
 Home-page: https://kombu.readthedocs.io
 Author: Ask Solem
 Author-email: auvipy@gmail.com
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/celery/kombu
 Keywords: messaging message amqp rabbitmq redis actor producer consumer
```

### Comparing `kombu-5.3.6/README.rst` & `kombu-5.3.7/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 ========================================
  kombu - Messaging library for Python
 ========================================
 
 |build-status| |coverage| |license| |wheel| |pyversion| |pyimp| |downloads|
 
-:Version: 5.3.6
+:Version: 5.3.7
 :Documentation: https://kombu.readthedocs.io/
 :Download: https://pypi.org/project/kombu/
 :Source: https://github.com/celery/kombu/
 :Keywords: messaging, amqp, rabbitmq, redis, mongodb, python, queue
 
 About
 =====
```

### Comparing `kombu-5.3.6/THANKS` & `kombu-5.3.7/THANKS`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/Makefile` & `kombu-5.3.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/_templates/sidebardonations.html` & `kombu-5.3.7/docs/_templates/sidebardonations.html`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/conf.py` & `kombu-5.3.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/images/favicon.ico` & `kombu-5.3.7/docs/images/favicon.ico`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/images/kombu.jpg` & `kombu-5.3.7/docs/images/kombu.jpg`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/images/kombusmall.jpg` & `kombu-5.3.7/docs/images/kombusmall.jpg`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/includes/introduction.txt` & `kombu-5.3.7/docs/includes/introduction.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-:Version: 5.3.6
+:Version: 5.3.7
 :Web: https://kombu.readthedocs.io/
 :Download: https://pypi.org/project/kombu/
 :Source: https://github.com/celery/kombu/
 :Keywords: messaging, amqp, rabbitmq, redis, mongodb, python, queue
 
 About
 =====
```

### Comparing `kombu-5.3.6/docs/includes/resources.txt` & `kombu-5.3.7/docs/includes/resources.txt`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/make.bat` & `kombu-5.3.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/reference/index.rst` & `kombu-5.3.7/docs/reference/index.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/reference/kombu.compat.rst` & `kombu-5.3.7/docs/reference/kombu.compat.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/reference/kombu.compression.rst` & `kombu-5.3.7/docs/reference/kombu.compression.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/reference/kombu.connection.rst` & `kombu-5.3.7/docs/reference/kombu.connection.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/reference/kombu.pidbox.rst` & `kombu-5.3.7/docs/reference/kombu.pidbox.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/reference/kombu.rst` & `kombu-5.3.7/docs/reference/kombu.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/reference/kombu.serialization.rst` & `kombu-5.3.7/docs/reference/kombu.serialization.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/reference/kombu.simple.rst` & `kombu-5.3.7/docs/reference/kombu.simple.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/reference/kombu.transport.SQS.rst` & `kombu-5.3.7/docs/reference/kombu.transport.SQS.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/reference/kombu.transport.azureservicebus.rst` & `kombu-5.3.7/docs/reference/kombu.transport.azureservicebus.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/reference/kombu.transport.azurestoragequeues.rst` & `kombu-5.3.7/docs/reference/kombu.transport.azurestoragequeues.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/reference/kombu.transport.base.rst` & `kombu-5.3.7/docs/reference/kombu.transport.base.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/reference/kombu.transport.confluentkafka.rst` & `kombu-5.3.7/docs/reference/kombu.transport.confluentkafka.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/reference/kombu.transport.librabbitmq.rst` & `kombu-5.3.7/docs/reference/kombu.transport.librabbitmq.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/reference/kombu.transport.pyamqp.rst` & `kombu-5.3.7/docs/reference/kombu.transport.pyamqp.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/reference/kombu.transport.pyro.rst` & `kombu-5.3.7/docs/reference/kombu.transport.pyro.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/reference/kombu.transport.qpid.rst` & `kombu-5.3.7/docs/reference/kombu.transport.qpid.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/reference/kombu.transport.redis.rst` & `kombu-5.3.7/docs/reference/kombu.transport.redis.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/reference/kombu.transport.rst` & `kombu-5.3.7/docs/reference/kombu.transport.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/reference/kombu.transport.sqlalchemy.rst` & `kombu-5.3.7/docs/reference/kombu.transport.sqlalchemy.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/reference/kombu.transport.virtual.exchange.rst` & `kombu-5.3.7/docs/reference/kombu.transport.virtual.exchange.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/reference/kombu.transport.virtual.rst` & `kombu-5.3.7/docs/reference/kombu.transport.virtual.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/templates/readme.txt` & `kombu-5.3.7/docs/templates/readme.txt`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/userguide/connections.rst` & `kombu-5.3.7/docs/userguide/connections.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/userguide/consumers.rst` & `kombu-5.3.7/docs/userguide/consumers.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/userguide/examples.rst` & `kombu-5.3.7/docs/userguide/examples.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/userguide/failover.rst` & `kombu-5.3.7/docs/userguide/failover.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/userguide/introduction.rst` & `kombu-5.3.7/docs/userguide/introduction.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/userguide/pools.rst` & `kombu-5.3.7/docs/userguide/pools.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/userguide/producers.rst` & `kombu-5.3.7/docs/userguide/producers.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/userguide/serialization.rst` & `kombu-5.3.7/docs/userguide/serialization.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/docs/userguide/simple.rst` & `kombu-5.3.7/docs/userguide/simple.rst`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/examples/complete_receive.py` & `kombu-5.3.7/examples/complete_receive.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/examples/complete_send.py` & `kombu-5.3.7/examples/complete_send.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/examples/experimental/async_consume.py` & `kombu-5.3.7/examples/experimental/async_consume.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/examples/memory_transport.py` & `kombu-5.3.7/examples/memory_transport.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/examples/rpc-tut6/rpc_client.py` & `kombu-5.3.7/examples/rpc-tut6/rpc_client.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/examples/rpc-tut6/rpc_server.py` & `kombu-5.3.7/examples/rpc-tut6/rpc_server.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/examples/simple_eventlet_receive.py` & `kombu-5.3.7/examples/simple_eventlet_receive.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/examples/simple_eventlet_send.py` & `kombu-5.3.7/examples/simple_eventlet_send.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/examples/simple_receive.py` & `kombu-5.3.7/examples/simple_receive.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/examples/simple_send.py` & `kombu-5.3.7/examples/simple_send.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/examples/simple_task_queue/client.py` & `kombu-5.3.7/examples/simple_task_queue/client.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/examples/simple_task_queue/worker.py` & `kombu-5.3.7/examples/simple_task_queue/worker.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/__init__.py` & `kombu-5.3.7/kombu/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 import os
 import re
 import sys
 from collections import namedtuple
 from typing import Any, cast
 
-__version__ = '5.3.6'
+__version__ = '5.3.7'
 __author__ = 'Ask Solem'
 __contact__ = 'auvipy@gmail.com'
 __homepage__ = 'https://kombu.readthedocs.io'
 __docformat__ = 'restructuredtext en'
 
 # -eof meta-
```

### Comparing `kombu-5.3.6/kombu/abstract.py` & `kombu-5.3.7/kombu/abstract.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/asynchronous/aws/connection.py` & `kombu-5.3.7/kombu/asynchronous/aws/connection.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/asynchronous/aws/ext.py` & `kombu-5.3.7/kombu/asynchronous/aws/ext.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/asynchronous/aws/sqs/connection.py` & `kombu-5.3.7/kombu/asynchronous/aws/sqs/connection.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/asynchronous/aws/sqs/message.py` & `kombu-5.3.7/kombu/asynchronous/aws/sqs/message.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/asynchronous/aws/sqs/queue.py` & `kombu-5.3.7/kombu/asynchronous/aws/sqs/queue.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/asynchronous/debug.py` & `kombu-5.3.7/kombu/asynchronous/debug.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/asynchronous/http/__init__.py` & `kombu-5.3.7/kombu/asynchronous/http/__init__.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/asynchronous/http/base.py` & `kombu-5.3.7/kombu/asynchronous/http/base.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/asynchronous/http/curl.py` & `kombu-5.3.7/kombu/asynchronous/http/curl.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/asynchronous/hub.py` & `kombu-5.3.7/kombu/asynchronous/hub.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/asynchronous/semaphore.py` & `kombu-5.3.7/kombu/asynchronous/semaphore.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/asynchronous/timer.py` & `kombu-5.3.7/kombu/asynchronous/timer.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/clocks.py` & `kombu-5.3.7/kombu/clocks.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/common.py` & `kombu-5.3.7/kombu/common.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/compat.py` & `kombu-5.3.7/kombu/compat.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/compression.py` & `kombu-5.3.7/kombu/compression.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/connection.py` & `kombu-5.3.7/kombu/connection.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/entity.py` & `kombu-5.3.7/kombu/entity.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/exceptions.py` & `kombu-5.3.7/kombu/exceptions.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/log.py` & `kombu-5.3.7/kombu/log.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/matcher.py` & `kombu-5.3.7/kombu/matcher.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/message.py` & `kombu-5.3.7/kombu/message.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/messaging.py` & `kombu-5.3.7/kombu/messaging.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/mixins.py` & `kombu-5.3.7/kombu/mixins.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/pidbox.py` & `kombu-5.3.7/kombu/pidbox.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/pools.py` & `kombu-5.3.7/kombu/pools.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/resource.py` & `kombu-5.3.7/kombu/resource.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/serialization.py` & `kombu-5.3.7/kombu/serialization.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/simple.py` & `kombu-5.3.7/kombu/simple.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/transport/SLMQ.py` & `kombu-5.3.7/kombu/transport/SLMQ.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/transport/SQS.py` & `kombu-5.3.7/kombu/transport/SQS.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/transport/__init__.py` & `kombu-5.3.7/kombu/transport/__init__.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/transport/azureservicebus.py` & `kombu-5.3.7/kombu/transport/azureservicebus.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/transport/azurestoragequeues.py` & `kombu-5.3.7/kombu/transport/azurestoragequeues.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/transport/base.py` & `kombu-5.3.7/kombu/transport/base.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/transport/confluentkafka.py` & `kombu-5.3.7/kombu/transport/confluentkafka.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/transport/consul.py` & `kombu-5.3.7/kombu/transport/consul.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/transport/etcd.py` & `kombu-5.3.7/kombu/transport/etcd.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/transport/filesystem.py` & `kombu-5.3.7/kombu/transport/filesystem.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/transport/librabbitmq.py` & `kombu-5.3.7/kombu/transport/librabbitmq.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/transport/memory.py` & `kombu-5.3.7/kombu/transport/memory.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/transport/mongodb.py` & `kombu-5.3.7/kombu/transport/mongodb.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/transport/pyamqp.py` & `kombu-5.3.7/kombu/transport/pyamqp.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/transport/pyro.py` & `kombu-5.3.7/kombu/transport/pyro.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/transport/qpid.py` & `kombu-5.3.7/kombu/transport/qpid.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/transport/redis.py` & `kombu-5.3.7/kombu/transport/redis.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/transport/sqlalchemy/__init__.py` & `kombu-5.3.7/kombu/transport/sqlalchemy/__init__.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/transport/sqlalchemy/models.py` & `kombu-5.3.7/kombu/transport/sqlalchemy/models.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/transport/virtual/base.py` & `kombu-5.3.7/kombu/transport/virtual/base.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/transport/virtual/exchange.py` & `kombu-5.3.7/kombu/transport/virtual/exchange.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/transport/zookeeper.py` & `kombu-5.3.7/kombu/transport/zookeeper.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/utils/__init__.py` & `kombu-5.3.7/kombu/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/utils/amq_manager.py` & `kombu-5.3.7/kombu/utils/amq_manager.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/utils/collections.py` & `kombu-5.3.7/kombu/utils/collections.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/utils/compat.py` & `kombu-5.3.7/kombu/utils/compat.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/utils/debug.py` & `kombu-5.3.7/kombu/utils/debug.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/utils/div.py` & `kombu-5.3.7/kombu/utils/div.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/utils/encoding.py` & `kombu-5.3.7/kombu/utils/encoding.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/utils/eventio.py` & `kombu-5.3.7/kombu/utils/eventio.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/utils/functional.py` & `kombu-5.3.7/kombu/utils/functional.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/utils/imports.py` & `kombu-5.3.7/kombu/utils/imports.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/utils/json.py` & `kombu-5.3.7/kombu/utils/json.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/utils/limits.py` & `kombu-5.3.7/kombu/utils/limits.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/utils/objects.py` & `kombu-5.3.7/kombu/utils/objects.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/utils/scheduling.py` & `kombu-5.3.7/kombu/utils/scheduling.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/utils/text.py` & `kombu-5.3.7/kombu/utils/text.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu/utils/url.py` & `kombu-5.3.7/kombu/utils/url.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu.egg-info/PKG-INFO` & `kombu-5.3.7/kombu.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kombu
-Version: 5.3.6
+Version: 5.3.7
 Summary: Messaging library for Python.
 Home-page: https://kombu.readthedocs.io
 Author: Ask Solem
 Author-email: auvipy@gmail.com
 License: BSD-3-Clause
 Project-URL: Source, https://github.com/celery/kombu
 Keywords: messaging message amqp rabbitmq redis actor producer consumer
```

### Comparing `kombu-5.3.6/kombu.egg-info/SOURCES.txt` & `kombu-5.3.7/kombu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/kombu.egg-info/requires.txt` & `kombu-5.3.7/kombu.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/requirements/test-ci.txt` & `kombu-5.3.7/requirements/test-ci.txt`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/setup.cfg` & `kombu-5.3.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/setup.py` & `kombu-5.3.7/setup.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/integration/common.py` & `kombu-5.3.7/t/integration/common.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/integration/test_kafka.py` & `kombu-5.3.7/t/integration/test_kafka.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/integration/test_mongodb.py` & `kombu-5.3.7/t/integration/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/integration/test_py_amqp.py` & `kombu-5.3.7/t/integration/test_py_amqp.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/integration/test_redis.py` & `kombu-5.3.7/t/integration/test_redis.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/mocks.py` & `kombu-5.3.7/t/mocks.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/asynchronous/aws/sqs/test_connection.py` & `kombu-5.3.7/t/unit/asynchronous/aws/sqs/test_connection.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/asynchronous/aws/sqs/test_queue.py` & `kombu-5.3.7/t/unit/asynchronous/aws/sqs/test_queue.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/asynchronous/aws/test_connection.py` & `kombu-5.3.7/t/unit/asynchronous/aws/test_connection.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/asynchronous/http/test_curl.py` & `kombu-5.3.7/t/unit/asynchronous/http/test_curl.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/asynchronous/http/test_http.py` & `kombu-5.3.7/t/unit/asynchronous/http/test_http.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/asynchronous/test_hub.py` & `kombu-5.3.7/t/unit/asynchronous/test_hub.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/asynchronous/test_semaphore.py` & `kombu-5.3.7/t/unit/asynchronous/test_semaphore.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/asynchronous/test_timer.py` & `kombu-5.3.7/t/unit/asynchronous/test_timer.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/conftest.py` & `kombu-5.3.7/t/unit/conftest.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/test_clocks.py` & `kombu-5.3.7/t/unit/test_clocks.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/test_common.py` & `kombu-5.3.7/t/unit/test_common.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/test_compat.py` & `kombu-5.3.7/t/unit/test_compat.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/test_compression.py` & `kombu-5.3.7/t/unit/test_compression.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/test_connection.py` & `kombu-5.3.7/t/unit/test_connection.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/test_entity.py` & `kombu-5.3.7/t/unit/test_entity.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/test_log.py` & `kombu-5.3.7/t/unit/test_log.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/test_matcher.py` & `kombu-5.3.7/t/unit/test_matcher.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/test_message.py` & `kombu-5.3.7/t/unit/test_message.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/test_messaging.py` & `kombu-5.3.7/t/unit/test_messaging.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/test_mixins.py` & `kombu-5.3.7/t/unit/test_mixins.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/test_pidbox.py` & `kombu-5.3.7/t/unit/test_pidbox.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/test_pools.py` & `kombu-5.3.7/t/unit/test_pools.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/test_serialization.py` & `kombu-5.3.7/t/unit/test_serialization.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/test_simple.py` & `kombu-5.3.7/t/unit/test_simple.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/transport/test_SQS.py` & `kombu-5.3.7/t/unit/transport/test_SQS.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/transport/test_azureservicebus.py` & `kombu-5.3.7/t/unit/transport/test_azureservicebus.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/transport/test_azurestoragequeues.py` & `kombu-5.3.7/t/unit/transport/test_azurestoragequeues.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/transport/test_base.py` & `kombu-5.3.7/t/unit/transport/test_base.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/transport/test_consul.py` & `kombu-5.3.7/t/unit/transport/test_consul.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/transport/test_etcd.py` & `kombu-5.3.7/t/unit/transport/test_etcd.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/transport/test_filesystem.py` & `kombu-5.3.7/t/unit/transport/test_filesystem.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/transport/test_librabbitmq.py` & `kombu-5.3.7/t/unit/transport/test_librabbitmq.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/transport/test_memory.py` & `kombu-5.3.7/t/unit/transport/test_memory.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/transport/test_mongodb.py` & `kombu-5.3.7/t/unit/transport/test_mongodb.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/transport/test_pyamqp.py` & `kombu-5.3.7/t/unit/transport/test_pyamqp.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/transport/test_pyro.py` & `kombu-5.3.7/t/unit/transport/test_pyro.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/transport/test_qpid.py` & `kombu-5.3.7/t/unit/transport/test_qpid.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/transport/test_redis.py` & `kombu-5.3.7/t/unit/transport/test_redis.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/transport/test_sqlalchemy.py` & `kombu-5.3.7/t/unit/transport/test_sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/transport/test_transport.py` & `kombu-5.3.7/t/unit/transport/test_transport.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/transport/test_zookeeper.py` & `kombu-5.3.7/t/unit/transport/test_zookeeper.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/transport/virtual/test_base.py` & `kombu-5.3.7/t/unit/transport/virtual/test_base.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/transport/virtual/test_exchange.py` & `kombu-5.3.7/t/unit/transport/virtual/test_exchange.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/utils/test_amq_manager.py` & `kombu-5.3.7/t/unit/utils/test_amq_manager.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/utils/test_compat.py` & `kombu-5.3.7/t/unit/utils/test_compat.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/utils/test_debug.py` & `kombu-5.3.7/t/unit/utils/test_debug.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/utils/test_div.py` & `kombu-5.3.7/t/unit/utils/test_div.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/utils/test_encoding.py` & `kombu-5.3.7/t/unit/utils/test_encoding.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/utils/test_functional.py` & `kombu-5.3.7/t/unit/utils/test_functional.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/utils/test_imports.py` & `kombu-5.3.7/t/unit/utils/test_imports.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/utils/test_json.py` & `kombu-5.3.7/t/unit/utils/test_json.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/utils/test_objects.py` & `kombu-5.3.7/t/unit/utils/test_objects.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/utils/test_scheduling.py` & `kombu-5.3.7/t/unit/utils/test_scheduling.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/utils/test_url.py` & `kombu-5.3.7/t/unit/utils/test_url.py`

 * *Files identical despite different names*

### Comparing `kombu-5.3.6/t/unit/utils/test_utils.py` & `kombu-5.3.7/t/unit/utils/test_utils.py`

 * *Files identical despite different names*

