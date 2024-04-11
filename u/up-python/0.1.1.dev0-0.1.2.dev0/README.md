# Comparing `tmp/up_python-0.1.1.dev0.tar.gz` & `tmp/up_python-0.1.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "up_python-0.1.1.dev0.tar", max compression
+gzip compressed data, was "up_python-0.1.2.dev0.tar", max compression
```

## Comparing `up_python-0.1.1.dev0.tar` & `up_python-0.1.2.dev0.tar`

### file list

```diff
@@ -1,122 +1,129 @@
--rw-r--r--   0        0        0    11357 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/LICENSE
--rw-r--r--   0        0        0     1007 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/NOTICE.adoc
--rw-r--r--   0        0        0     4477 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/README.adoc
--rw-r--r--   0        0        0      690 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/scripts/__init__.py
--rw-r--r--   0        0        0     4995 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/scripts/pull_and_compile_protos.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_cloudevent/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_cloudevent/test_datamodel/__init__.py
--rw-r--r--   0        0        0    16040 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_cloudevent/test_datamodel/test_ucloudevent.py
--rw-r--r--   0        0        0     4112 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_cloudevent/test_datamodel/test_ucloudeventattributes.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_cloudevent/test_factory/__init__.py
--rw-r--r--   0        0        0     6759 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_cloudevent/test_factory/cloudevent.json
--rw-r--r--   0        0        0    19308 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_cloudevent/test_factory/test_cloudeventfactory.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_cloudevent/test_serialize/__init__.py
--rw-r--r--   0        0        0     5544 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_cloudevent/test_serialize/cloudevent_to_protobuf.json
--rw-r--r--   0        0        0     3505 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_cloudevent/test_serialize/test_base64protobufserializer.py
--rw-r--r--   0        0        0     6961 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_cloudevent/test_serialize/test_cloudeventtojsonserializer.py
--rw-r--r--   0        0        0     7999 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_cloudevent/test_serialize/test_cloudeventtoprotobufserializer.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_cloudevent/test_validator/__init__.py
--rw-r--r--   0        0        0    25384 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_cloudevent/test_validator/test_cloudeventvalidator.py
--rw-r--r--   0        0        0     2698 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_cloudevent/test_validator/test_validationresult.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_rpc/__init__.py
--rw-r--r--   0        0        0     3760 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_rpc/test_calloptions.py
--rw-r--r--   0        0        0    10821 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_rpc/test_rpc.py
--rw-r--r--   0        0        0     8808 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_rpc/test_rpcresult.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_transport/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_transport/test_builder/__init__.py
--rw-r--r--   0        0        0     5001 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_transport/test_builder/test_uattributesbuilder.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_transport/test_validate/__init__.py
--rw-r--r--   0        0        0    26723 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_transport/test_validate/test_uattributesvalidator.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_uri/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_uri/test_serializer/__init__.py
--rw-r--r--   0        0        0    37043 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_uri/test_serializer/test_longuriserializer.py
--rw-r--r--   0        0        0     7326 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_uri/test_serializer/test_microuriserializer.py
--rw-r--r--   0        0        0     3291 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_uri/test_serializer/test_uriserializer.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_uri/test_validator/__init__.py
--rw-r--r--   0        0        0    16629 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_uri/test_validator/test_urivalidator.py
--rw-r--r--   0        0        0     2878 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_uri/test_validator/uris.json
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_uuid/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.719023 up_python-0.1.1.dev0/tests/test_uuid/test_factory/__init__.py
--rw-r--r--   0        0        0    11506 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/tests/test_uuid/test_factory/test_uuidfactory.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/tests/test_uuid/test_validator/__init__.py
--rw-r--r--   0        0        0     5536 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/tests/test_uuid/test_validator/test_uuidvalidator.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/__init__.py
--rw-r--r--   0        0        0     2160 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/cloudevent/README.adoc
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/cloudevent/__init__.py
--rw-r--r--   0        0        0     3277 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/cloudevent/cloudevents_pb2.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/cloudevent/datamodel/__init__.py
--rw-r--r--   0        0        0     7749 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/cloudevent/datamodel/ucloudeventattributes.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/cloudevent/factory/__init__.py
--rw-r--r--   0        0        0    11840 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/cloudevent/factory/cloudeventfactory.py
--rw-r--r--   0        0        0    23251 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/cloudevent/factory/ucloudevent.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/cloudevent/serialize/__init__.py
--rw-r--r--   0        0        0     2186 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/cloudevent/serialize/base64protobufserializer.py
--rw-r--r--   0        0        0     1370 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/cloudevent/serialize/cloudeventserializer.py
--rw-r--r--   0        0        0     1586 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/cloudevent/serialize/cloudeventserializers.py
--rw-r--r--   0        0        0     1615 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/cloudevent/serialize/cloudeventtojsonserializer.py
--rw-r--r--   0        0        0     4170 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/cloudevent/serialize/cloudeventtoprotobufserializer.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/cloudevent/validate/__init__.py
--rw-r--r--   0        0        0    15685 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/cloudevent/validate/cloudeventvalidator.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:32.235251 up_python-0.1.1.dev0/uprotocol/proto/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:32.251251 up_python-0.1.1.dev0/uprotocol/proto/core/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:32.251251 up_python-0.1.1.dev0/uprotocol/proto/core/udiscovery/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:32.251251 up_python-0.1.1.dev0/uprotocol/proto/core/udiscovery/v3/__init__.py
--rw-r--r--   0        0        0    11175 2024-03-05 19:46:32.251251 up_python-0.1.1.dev0/uprotocol/proto/core/udiscovery/v3/udiscovery_pb2.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:32.251251 up_python-0.1.1.dev0/uprotocol/proto/core/usubscription/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:32.251251 up_python-0.1.1.dev0/uprotocol/proto/core/usubscription/v3/__init__.py
--rw-r--r--   0        0        0    12375 2024-03-05 19:46:32.255252 up_python-0.1.1.dev0/uprotocol/proto/core/usubscription/v3/usubscription_pb2.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:32.255252 up_python-0.1.1.dev0/uprotocol/proto/core/utwin/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:32.255252 up_python-0.1.1.dev0/uprotocol/proto/core/utwin/v1/__init__.py
--rw-r--r--   0        0        0     2690 2024-03-05 19:46:32.255252 up_python-0.1.1.dev0/uprotocol/proto/core/utwin/v1/utwin_pb2.py
--rw-r--r--   0        0        0     1755 2024-03-05 19:46:32.239251 up_python-0.1.1.dev0/uprotocol/proto/file_pb2.py
--rw-r--r--   0        0        0     4596 2024-03-05 19:46:32.243251 up_python-0.1.1.dev0/uprotocol/proto/uattributes_pb2.py
--rw-r--r--   0        0        0     1359 2024-03-05 19:46:32.243251 up_python-0.1.1.dev0/uprotocol/proto/umessage_pb2.py
--rw-r--r--   0        0        0     3609 2024-03-05 19:46:32.247251 up_python-0.1.1.dev0/uprotocol/proto/upayload_pb2.py
--rw-r--r--   0        0        0     3218 2024-03-05 19:46:32.247251 up_python-0.1.1.dev0/uprotocol/proto/uprotocol_options_pb2.py
--rw-r--r--   0        0        0     2313 2024-03-05 19:46:32.251251 up_python-0.1.1.dev0/uprotocol/proto/uri_pb2.py
--rw-r--r--   0        0        0     2033 2024-03-05 19:46:32.239251 up_python-0.1.1.dev0/uprotocol/proto/ustatus_pb2.py
--rw-r--r--   0        0        0     1102 2024-03-05 19:46:32.247251 up_python-0.1.1.dev0/uprotocol/proto/uuid_pb2.py
--rw-r--r--   0        0        0      324 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/rpc/README.adoc
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/rpc/__init__.py
--rw-r--r--   0        0        0     3145 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/rpc/calloptions.py
--rw-r--r--   0        0        0     2764 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/rpc/rpcclient.py
--rw-r--r--   0        0        0     6810 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/rpc/rpcmapper.py
--rw-r--r--   0        0        0     5077 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/rpc/rpcresult.py
--rw-r--r--   0        0        0     2517 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/rpc/rpcserver.py
--rw-r--r--   0        0        0     1813 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/rpc/urpclistener.py
--rw-r--r--   0        0        0      526 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/transport/README.adoc
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/transport/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/transport/builder/__init__.py
--rw-r--r--   0        0        0     8375 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/transport/builder/uattributesbuilder.py
--rw-r--r--   0        0        0     3061 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/transport/builder/upayloadbuilder.py
--rw-r--r--   0        0        0     1565 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/transport/ulistener.py
--rw-r--r--   0        0        0     3218 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/transport/utransport.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/transport/validate/__init__.py
--rw-r--r--   0        0        0    13639 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/transport/validate/uattributesvalidator.py
--rw-r--r--   0        0        0     1915 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/uri/README.adoc
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/uri/__init__.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/uri/factory/__init__.py
--rw-r--r--   0        0        0     2251 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/uri/factory/uentity_factory.py
--rw-r--r--   0        0        0     2250 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/uri/factory/uresource_builder.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/uri/serializer/__init__.py
--rw-r--r--   0        0        0     7712 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/uri/serializer/longuriserializer.py
--rw-r--r--   0        0        0     6475 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/uri/serializer/microuriserializer.py
--rw-r--r--   0        0        0     3634 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/uri/serializer/uriserializer.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/uri/validator/__init__.py
--rw-r--r--   0        0        0     8062 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/uri/validator/urivalidator.py
--rw-r--r--   0        0        0      963 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/uuid/README.adoc
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/uuid/__init__.py
--rw-r--r--   0        0        0     5098 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/uuid/factory/__init__.py
--rw-r--r--   0        0        0     2429 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/uuid/factory/uuidfactory.py
--rw-r--r--   0        0        0     5860 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/uuid/factory/uuidutils.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/uuid/serializer/__init__.py
--rw-r--r--   0        0        0     2591 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/uuid/serializer/longuuidserializer.py
--rw-r--r--   0        0        0     2472 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/uuid/serializer/microuuidserializer.py
--rw-r--r--   0        0        0     2069 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/uuid/serializer/uuidserializer.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/uuid/validate/__init__.py
--rw-r--r--   0        0        0     4531 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/uuid/validate/uuidvalidator.py
--rw-r--r--   0        0        0        0 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/validation/__init__.py
--rw-r--r--   0        0        0     2922 2024-03-05 19:46:06.723023 up_python-0.1.1.dev0/uprotocol/validation/validationresult.py
--rw-r--r--   0        0        0     5443 1970-01-01 00:00:00.000000 up_python-0.1.1.dev0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2024-04-11 00:40:39.659589 up_python-0.1.2.dev0/LICENSE
+-rw-r--r--   0        0        0     1007 2024-04-11 00:40:39.659589 up_python-0.1.2.dev0/NOTICE.adoc
+-rw-r--r--   0        0        0     4476 2024-04-11 00:40:39.659589 up_python-0.1.2.dev0/README.adoc
+-rw-r--r--   0        0        0      767 2024-04-11 00:40:39.659589 up_python-0.1.2.dev0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.659589 up_python-0.1.2.dev0/scripts/__init__.py
+-rw-r--r--   0        0        0     4980 2024-04-11 00:40:39.659589 up_python-0.1.2.dev0/scripts/pull_and_compile_protos.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.659589 up_python-0.1.2.dev0/tests/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.659589 up_python-0.1.2.dev0/tests/test_cloudevent/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.659589 up_python-0.1.2.dev0/tests/test_cloudevent/test_datamodel/__init__.py
+-rw-r--r--   0        0        0    22624 2024-04-11 00:40:39.659589 up_python-0.1.2.dev0/tests/test_cloudevent/test_datamodel/test_ucloudevent.py
+-rw-r--r--   0        0        0     6818 2024-04-11 00:40:39.659589 up_python-0.1.2.dev0/tests/test_cloudevent/test_datamodel/test_ucloudeventattributes.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.659589 up_python-0.1.2.dev0/tests/test_cloudevent/test_factory/__init__.py
+-rw-r--r--   0        0        0     6759 2024-04-11 00:40:39.659589 up_python-0.1.2.dev0/tests/test_cloudevent/test_factory/cloudevent.json
+-rw-r--r--   0        0        0    21104 2024-04-11 00:40:39.659589 up_python-0.1.2.dev0/tests/test_cloudevent/test_factory/test_cloudeventfactory.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.659589 up_python-0.1.2.dev0/tests/test_cloudevent/test_serialize/__init__.py
+-rw-r--r--   0        0        0     5544 2024-04-11 00:40:39.659589 up_python-0.1.2.dev0/tests/test_cloudevent/test_serialize/cloudevent_to_protobuf.json
+-rw-r--r--   0        0        0     3641 2024-04-11 00:40:39.659589 up_python-0.1.2.dev0/tests/test_cloudevent/test_serialize/test_base64protobufserializer.py
+-rw-r--r--   0        0        0     6552 2024-04-11 00:40:39.659589 up_python-0.1.2.dev0/tests/test_cloudevent/test_serialize/test_cloudeventtojsonserializer.py
+-rw-r--r--   0        0        0     8549 2024-04-11 00:40:39.659589 up_python-0.1.2.dev0/tests/test_cloudevent/test_serialize/test_cloudeventtoprotobufserializer.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.659589 up_python-0.1.2.dev0/tests/test_cloudevent/test_validator/__init__.py
+-rw-r--r--   0        0        0    28104 2024-04-11 00:40:39.659589 up_python-0.1.2.dev0/tests/test_cloudevent/test_validator/test_cloudeventvalidator.py
+-rw-r--r--   0        0        0     2698 2024-04-11 00:40:39.659589 up_python-0.1.2.dev0/tests/test_cloudevent/test_validator/test_validationresult.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.659589 up_python-0.1.2.dev0/tests/test_rpc/__init__.py
+-rw-r--r--   0        0        0     2575 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_rpc/test_calloptions.py
+-rw-r--r--   0        0        0    12757 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_rpc/test_rpc.py
+-rw-r--r--   0        0        0     8808 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_rpc/test_rpcresult.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_transport/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_transport/test_builder/__init__.py
+-rw-r--r--   0        0        0     9708 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_transport/test_builder/test_uattributesbuilder.py
+-rw-r--r--   0        0        0     9259 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_transport/test_builder/test_upayloadbuilder.py
+-rw-r--r--   0        0        0     3163 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_transport/test_utransport.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_transport/test_validate/__init__.py
+-rw-r--r--   0        0        0    27824 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_transport/test_validate/test_uattributesvalidator.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_uri/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_uri/test_factory/__init__.py
+-rw-r--r--   0        0        0     5105 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_uri/test_factory/test_uentity_factory.py
+-rw-r--r--   0        0        0     2392 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_uri/test_factory/test_uresource_builder.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_uri/test_serializer/__init__.py
+-rw-r--r--   0        0        0     5066 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_uri/test_serializer/test_ipaddress.py
+-rw-r--r--   0        0        0    37218 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_uri/test_serializer/test_longuriserializer.py
+-rw-r--r--   0        0        0     6637 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_uri/test_serializer/test_microuriserializer.py
+-rw-r--r--   0        0        0    10369 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_uri/test_serializer/test_shorturiserializer.py
+-rw-r--r--   0        0        0    10177 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_uri/test_serializer/test_uriserializer.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_uri/test_validator/__init__.py
+-rw-r--r--   0        0        0    21826 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_uri/test_validator/test_urivalidator.py
+-rw-r--r--   0        0        0     2878 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_uri/test_validator/uris.json
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_uuid/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_uuid/test_factory/__init__.py
+-rw-r--r--   0        0        0    11600 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_uuid/test_factory/test_uuidfactory.py
+-rw-r--r--   0        0        0     4399 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_uuid/test_factory/test_uuidutils.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_uuid/test_validator/__init__.py
+-rw-r--r--   0        0        0     5522 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/tests/test_uuid/test_validator/test_uuidvalidator.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/__init__.py
+-rw-r--r--   0        0        0     2160 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/cloudevent/README.adoc
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/cloudevent/__init__.py
+-rw-r--r--   0        0        0     3277 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/cloudevent/cloudevents_pb2.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/cloudevent/datamodel/__init__.py
+-rw-r--r--   0        0        0     7956 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/cloudevent/datamodel/ucloudeventattributes.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/cloudevent/factory/__init__.py
+-rw-r--r--   0        0        0    11254 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/cloudevent/factory/cloudeventfactory.py
+-rw-r--r--   0        0        0    26264 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/cloudevent/factory/ucloudevent.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/cloudevent/serialize/__init__.py
+-rw-r--r--   0        0        0     2186 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/cloudevent/serialize/base64protobufserializer.py
+-rw-r--r--   0        0        0     1370 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/cloudevent/serialize/cloudeventserializer.py
+-rw-r--r--   0        0        0     1586 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/cloudevent/serialize/cloudeventserializers.py
+-rw-r--r--   0        0        0     1615 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/cloudevent/serialize/cloudeventtojsonserializer.py
+-rw-r--r--   0        0        0     4207 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/cloudevent/serialize/cloudeventtoprotobufserializer.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/cloudevent/validate/__init__.py
+-rw-r--r--   0        0        0    17695 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/cloudevent/validate/cloudeventvalidator.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:41:49.255353 up_python-0.1.2.dev0/uprotocol/proto/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:41:49.267353 up_python-0.1.2.dev0/uprotocol/proto/core/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:41:49.271353 up_python-0.1.2.dev0/uprotocol/proto/core/udiscovery/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:41:49.271353 up_python-0.1.2.dev0/uprotocol/proto/core/udiscovery/v3/__init__.py
+-rw-r--r--   0        0        0    11308 2024-04-11 00:41:49.275353 up_python-0.1.2.dev0/uprotocol/proto/core/udiscovery/v3/udiscovery_pb2.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:41:49.271353 up_python-0.1.2.dev0/uprotocol/proto/core/usubscription/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:41:49.271353 up_python-0.1.2.dev0/uprotocol/proto/core/usubscription/v3/__init__.py
+-rw-r--r--   0        0        0    11994 2024-04-11 00:41:49.271353 up_python-0.1.2.dev0/uprotocol/proto/core/usubscription/v3/usubscription_pb2.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:41:49.267353 up_python-0.1.2.dev0/uprotocol/proto/core/utwin/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:41:49.267353 up_python-0.1.2.dev0/uprotocol/proto/core/utwin/v2/__init__.py
+-rw-r--r--   0        0        0     2690 2024-04-11 00:41:49.271353 up_python-0.1.2.dev0/uprotocol/proto/core/utwin/v2/utwin_pb2.py
+-rw-r--r--   0        0        0     1755 2024-04-11 00:41:49.263352 up_python-0.1.2.dev0/uprotocol/proto/file_pb2.py
+-rw-r--r--   0        0        0     5217 2024-04-11 00:41:49.263352 up_python-0.1.2.dev0/uprotocol/proto/uattributes_pb2.py
+-rw-r--r--   0        0        0     1359 2024-04-11 00:41:49.267353 up_python-0.1.2.dev0/uprotocol/proto/umessage_pb2.py
+-rw-r--r--   0        0        0     3609 2024-04-11 00:41:49.255353 up_python-0.1.2.dev0/uprotocol/proto/upayload_pb2.py
+-rw-r--r--   0        0        0     3838 2024-04-11 00:41:49.259353 up_python-0.1.2.dev0/uprotocol/proto/uprotocol_options_pb2.py
+-rw-r--r--   0        0        0     2313 2024-04-11 00:41:49.259353 up_python-0.1.2.dev0/uprotocol/proto/uri_pb2.py
+-rw-r--r--   0        0        0     2033 2024-04-11 00:41:49.263352 up_python-0.1.2.dev0/uprotocol/proto/ustatus_pb2.py
+-rw-r--r--   0        0        0     1102 2024-04-11 00:41:49.267353 up_python-0.1.2.dev0/uprotocol/proto/uuid_pb2.py
+-rw-r--r--   0        0        0      324 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/rpc/README.adoc
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/rpc/__init__.py
+-rw-r--r--   0        0        0     2642 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/rpc/rpcclient.py
+-rw-r--r--   0        0        0     7308 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/rpc/rpcmapper.py
+-rw-r--r--   0        0        0     5281 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/rpc/rpcresult.py
+-rw-r--r--   0        0        0      526 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/transport/README.adoc
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/transport/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/transport/builder/__init__.py
+-rw-r--r--   0        0        0     9264 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/transport/builder/uattributesbuilder.py
+-rw-r--r--   0        0        0     3217 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/transport/builder/upayloadbuilder.py
+-rw-r--r--   0        0        0     1565 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/transport/ulistener.py
+-rw-r--r--   0        0        0     3218 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/transport/utransport.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/transport/validate/__init__.py
+-rw-r--r--   0        0        0    15993 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/transport/validate/uattributesvalidator.py
+-rw-r--r--   0        0        0     1519 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/uri/README.adoc
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/uri/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/uri/factory/__init__.py
+-rw-r--r--   0        0        0     2416 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/uri/factory/uentity_factory.py
+-rw-r--r--   0        0        0     3136 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/uri/factory/uresource_builder.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/uri/serializer/__init__.py
+-rw-r--r--   0        0        0     2645 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/uri/serializer/ipaddress.py
+-rw-r--r--   0        0        0     7318 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/uri/serializer/longuriserializer.py
+-rw-r--r--   0        0        0     6823 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/uri/serializer/microuriserializer.py
+-rw-r--r--   0        0        0     7471 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/uri/serializer/shorturiserializer.py
+-rw-r--r--   0        0        0     1961 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/uri/serializer/uriserializer.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.663589 up_python-0.1.2.dev0/uprotocol/uri/validator/__init__.py
+-rw-r--r--   0        0        0     9310 2024-04-11 00:40:39.667590 up_python-0.1.2.dev0/uprotocol/uri/validator/urivalidator.py
+-rw-r--r--   0        0        0      963 2024-04-11 00:40:39.667590 up_python-0.1.2.dev0/uprotocol/uuid/README.adoc
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.667590 up_python-0.1.2.dev0/uprotocol/uuid/__init__.py
+-rw-r--r--   0        0        0     5098 2024-04-11 00:40:39.667590 up_python-0.1.2.dev0/uprotocol/uuid/factory/__init__.py
+-rw-r--r--   0        0        0     2429 2024-04-11 00:40:39.667590 up_python-0.1.2.dev0/uprotocol/uuid/factory/uuidfactory.py
+-rw-r--r--   0        0        0     9106 2024-04-11 00:40:39.667590 up_python-0.1.2.dev0/uprotocol/uuid/factory/uuidutils.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.667590 up_python-0.1.2.dev0/uprotocol/uuid/serializer/__init__.py
+-rw-r--r--   0        0        0     2689 2024-04-11 00:40:39.667590 up_python-0.1.2.dev0/uprotocol/uuid/serializer/longuuidserializer.py
+-rw-r--r--   0        0        0     2536 2024-04-11 00:40:39.667590 up_python-0.1.2.dev0/uprotocol/uuid/serializer/microuuidserializer.py
+-rw-r--r--   0        0        0     2081 2024-04-11 00:40:39.667590 up_python-0.1.2.dev0/uprotocol/uuid/serializer/uuidserializer.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.667590 up_python-0.1.2.dev0/uprotocol/uuid/validate/__init__.py
+-rw-r--r--   0        0        0     4715 2024-04-11 00:40:39.667590 up_python-0.1.2.dev0/uprotocol/uuid/validate/uuidvalidator.py
+-rw-r--r--   0        0        0        0 2024-04-11 00:40:39.667590 up_python-0.1.2.dev0/uprotocol/validation/__init__.py
+-rw-r--r--   0        0        0     2925 2024-04-11 00:40:39.667590 up_python-0.1.2.dev0/uprotocol/validation/validationresult.py
+-rw-r--r--   0        0        0     5472 1970-01-01 00:00:00.000000 up_python-0.1.2.dev0/PKG-INFO
```

### Comparing `up_python-0.1.1.dev0/LICENSE` & `up_python-0.1.2.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `up_python-0.1.1.dev0/NOTICE.adoc` & `up_python-0.1.2.dev0/NOTICE.adoc`

 * *Files identical despite different names*

### Comparing `up_python-0.1.1.dev0/README.adoc` & `up_python-0.1.2.dev0/README.adoc`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -108,8 +108,8 @@
 `python clean_project.py`
 
 === Running the Tests
 
 Requires coverage to be installed first, that can be done by running `pip install coverage`
 
 then you run:
-`python -m coverage run --source tests/ -m unittest discover`
+`python -m coverage run --source tests/ -m unittest discover`
```

### Comparing `up_python-0.1.1.dev0/pyproject.toml` & `up_python-0.1.2.dev0/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,27 +1,29 @@
 [tool.poetry]
 name = "up-python"
-version = "0.1.1-dev"
+version = "0.1.2-dev"
 description = "Language specific uProtocol library for building and using UUri, UUID, UAttributes, UTransport, and more."
 authors = ["Neelam Kushwah <neelam.kushwah@gm.com>"]
 license = "The Apache License, Version 2.0"
 readme = "README.adoc"
 repository = "https://github.com/eclipse-uprotocol/up-python"
 packages = [{ include = "uprotocol" },
     { include = "tests" },
     { include = "scripts" }
 
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8"
 cloudevents = "*"
-multipledispatch = "*"
+multimethod = "*"
 gitpython = ">=3.1.41"
 googleapis-common-protos = ">=1.56.4"
+protobuf = "4.24.2"
+
+[tool.poetry.dev-dependencies]
+pytest = "^6.2"
+coverage = "^5.5"
 
 [build-system]
 requires = ["poetry-core"]
-build-backend = "poetry.core.masonry.api"
-
-
-
+build-backend = "poetry.core.masonry.api"
```

### Comparing `up_python-0.1.1.dev0/scripts/pull_and_compile_protos.py` & `up_python-0.1.2.dev0/scripts/pull_and_compile_protos.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,25 +30,25 @@
 import subprocess
 
 import git
 from git import Repo
 
 REPO_URL = "https://github.com/eclipse-uprotocol/up-core-api.git"
 PROTO_REPO_DIR = os.path.abspath("../target")
-TAG_NAME = "uprotocol-core-api-1.5.6"
+TAG_NAME = "uprotocol-core-api-1.5.7"
 PROTO_OUTPUT_DIR = os.path.abspath("../uprotocol/proto")
 
 
 def clone_or_pull(repo_url, PROTO_REPO_DIR):
     try:
         repo = Repo.clone_from(repo_url, PROTO_REPO_DIR)
         print(f"Repository cloned successfully from {repo_url} to {PROTO_REPO_DIR}")
         # Checkout the specific tag
         repo.git.checkout(TAG_NAME)
-    except git.exc.GitCommandError as clone_error:
+    except git.exc.GitCommandError:
         try:
             git_pull_command = ["git", "pull", "origin", TAG_NAME]
             subprocess.run(git_pull_command, cwd=PROTO_REPO_DIR, check=True)
             print("Git pull successful after clone failure.")
         except subprocess.CalledProcessError as pull_error:
             print(f"Error during Git pull: {pull_error}")
```

### Comparing `up_python-0.1.1.dev0/tests/test_cloudevent/test_datamodel/test_ucloudevent.py` & `up_python-0.1.2.dev0/tests/test_cloudevent/test_datamodel/test_ucloudevent.py`

 * *Files 23% similar despite different names*

```diff
@@ -20,58 +20,105 @@
 # under the License.
 # SPDX-FileType: SOURCE
 # SPDX-FileCopyrightText: 2023 General Motors GTO LLC
 # SPDX-License-Identifier: Apache-2.0
 #
 # -------------------------------------------------------------------------
 
+from datetime import datetime, timezone, timedelta
+
 from uprotocol.proto.uri_pb2 import UUri, UEntity, UResource
 from uprotocol.uri.serializer.longuriserializer import LongUriSerializer
 from uprotocol.cloudevent.cloudevents_pb2 import CloudEvent
 from uprotocol.proto.uattributes_pb2 import UMessageType, UPriority
+from uprotocol.proto.upayload_pb2 import UPayloadFormat 
 from uprotocol.cloudevent.factory.cloudeventfactory import CloudEventFactory
 from uprotocol.proto.ustatus_pb2 import UCode
 from uprotocol.uuid.factory.uuidfactory import Factories
 from uprotocol.uuid.serializer.longuuidserializer import LongUuidSerializer
 import time
 import unittest
 
 from google.protobuf import any_pb2
 
-from uprotocol.cloudevent.datamodel.ucloudeventattributes import UCloudEventAttributesBuilder
+from uprotocol.cloudevent.datamodel.ucloudeventattributes import (
+    UCloudEventAttributesBuilder,
+)
 from uprotocol.cloudevent.factory.ucloudevent import UCloudEvent
 
+
 def build_uri_for_test():
-    uri = UUri(entity=UEntity(name="body.access"),
-               resource=UResource(name="door", instance="front_left", message="Door"))
+    uri = UUri(
+        entity=UEntity(name="body.access"),
+        resource=UResource(name="door", instance="front_left", message="Door"),
+    )
     return LongUriSerializer().serialize(uri)
 
 
 def build_proto_payload_for_test():
-    ce_proto = CloudEvent(spec_version="1.0", source="//VCU.MY_CAR_VIN/body.access//door.front_left#Door", id="hello",
-                          type="example.demo",
-                          proto_data=any_pb2.Any())
+    ce_proto = CloudEvent(
+        spec_version="1.0",
+        source="//VCU.MY_CAR_VIN/body.access//door.front_left#Door",
+        id="hello",
+        type="example.demo",
+        proto_data=any_pb2.Any(),
+    )
 
     any_obj = any_pb2.Any()
     any_obj.Pack(ce_proto)
     return any_obj
 
 
 def build_cloud_event_for_test():
     source = build_uri_for_test()
     proto_payload = build_proto_payload_for_test()
     # additional attributes
-    u_cloud_event_attributes = UCloudEventAttributesBuilder().with_hash("somehash").with_priority(
-        UPriority.UPRIORITY_CS1).with_ttl(3).with_token("someOAuthToken").build()
+    u_cloud_event_attributes = (
+        UCloudEventAttributesBuilder()
+        .with_hash("somehash")
+        .with_priority(UPriority.UPRIORITY_CS1)
+        .with_ttl(3)
+        .with_token("someOAuthToken")
+        .build()
+    )
 
     # build the cloud event
-    cloud_event = CloudEventFactory.build_base_cloud_event("testme", source, proto_payload.SerializeToString(),
-                                                           proto_payload.type_url, u_cloud_event_attributes,
-                                                           UCloudEvent.get_event_type(
-                                                               UMessageType.UMESSAGE_TYPE_PUBLISH))
+    cloud_event = CloudEventFactory.build_base_cloud_event(
+        "testme",
+        source,
+        proto_payload.SerializeToString(),
+        proto_payload.type_url,
+        u_cloud_event_attributes,
+        UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_PUBLISH),
+    )
+    return cloud_event
+
+
+def build_cloud_event_for_test_with_id(id):
+    source = build_uri_for_test()
+    proto_payload = build_proto_payload_for_test()
+    # additional attributes
+    u_cloud_event_attributes = (
+        UCloudEventAttributesBuilder()
+        .with_hash("somehash")
+        .with_priority(UPriority.UPRIORITY_CS1)
+        .with_ttl(3)
+        .with_token("someOAuthToken")
+        .build()
+    )
+
+    # build the cloud event
+    cloud_event = CloudEventFactory.build_base_cloud_event(
+        id,
+        source,
+        proto_payload.SerializeToString(),
+        proto_payload.type_url,
+        u_cloud_event_attributes,
+        UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_PUBLISH),
+    )
     return cloud_event
 
 
 class TestUCloudEvent(unittest.TestCase):
     DATA_CONTENT_TYPE = "application/x-protobuf"
 
     def test_extract_source_from_cloudevent(self):
@@ -79,30 +126,35 @@
         source = UCloudEvent.get_source(cloud_event)
         self.assertEqual("/body.access//door.front_left#Door", source)
 
     def test_extract_sink_from_cloudevent_when_sink_exists(self):
         sink = "//bo.cloud/petapp/1/rpc.response"
         cloud_event = build_cloud_event_for_test()
         cloud_event.__setitem__("sink", sink)
+        cloud_event.__setitem__("plevel", 4)
         self.assertEqual(sink, UCloudEvent.get_sink(cloud_event))
 
     def test_extract_sink_from_cloudevent_when_sink_does_not_exist(self):
         cloud_event = build_cloud_event_for_test()
         self.assertEqual(None, UCloudEvent.get_sink(cloud_event))
 
     def test_extract_requestId_from_cloudevent_when_requestId_exists(self):
         cloud_event = build_cloud_event_for_test()
         cloud_event.__setitem__("reqid", "somereqid")
         self.assertEqual("somereqid", UCloudEvent.get_request_id(cloud_event))
 
-    def test_extract_requestId_from_cloudevent_when_requestId_does_not_exist(self):
+    def test_extract_requestId_from_cloudevent_when_requestId_does_not_exist(
+        self,
+    ):
         cloud_event = build_cloud_event_for_test()
         self.assertEqual(None, UCloudEvent.get_request_id(cloud_event))
 
-    def test_extract_requestId_from_cloudevent_when_requestId_value_is_null(self):
+    def test_extract_requestId_from_cloudevent_when_requestId_value_is_null(
+        self,
+    ):
         cloud_event = build_cloud_event_for_test()
         cloud_event.__setitem__("reqid", None)
         self.assertEqual(None, UCloudEvent.get_request_id(cloud_event))
 
     def test_extract_hash_from_cloudevent_when_hash_exists(self):
         cloud_event = build_cloud_event_for_test()
         self.assertEqual("somehash", UCloudEvent.get_hash(cloud_event))
@@ -110,24 +162,31 @@
     def test_extract_hash_from_cloudevent_when_hash_does_not_exist(self):
         cloud_event = build_cloud_event_for_test()
         cloud_event.__delitem__("hash")
         self.assertEqual(None, UCloudEvent.get_hash(cloud_event))
 
     def test_extract_priority_from_cloudevent_when_priority_exists(self):
         cloud_event = build_cloud_event_for_test()
-        self.assertEqual(UPriority.Name(UPriority.UPRIORITY_CS1), UCloudEvent.get_priority(cloud_event))
-
-    def test_extract_priority_from_cloudevent_when_priority_does_not_exist(self):
+        self.assertEqual(
+            UPriority.Name(UPriority.UPRIORITY_CS1),
+            UCloudEvent.get_priority(cloud_event),
+        )
+
+    def test_extract_priority_from_cloudevent_when_priority_does_not_exist(
+        self,
+    ):
         cloud_event = build_cloud_event_for_test()
         cloud_event.__delitem__("priority")
         self.assertEqual(None, UCloudEvent.get_priority(cloud_event))
 
     def test_extract_ttl_from_cloudevent_when_ttl_exists(self):
         cloud_event = build_cloud_event_for_test()
-        self.assertEqual(3, UCloudEvent.get_ttl(cloud_event))
+        self.assertEqual(
+            UCode.INVALID_ARGUMENT, UCloudEvent.get_ttl(cloud_event)
+        )
 
     def test_extract_ttl_from_cloudevent_when_ttl_does_not_exists(self):
         cloud_event = build_cloud_event_for_test()
         cloud_event.__delitem__("ttl")
         self.assertEqual(None, UCloudEvent.get_ttl(cloud_event))
 
     def test_extract_token_from_cloudevent_when_token_exists(self):
@@ -138,162 +197,417 @@
         cloud_event = build_cloud_event_for_test()
         cloud_event.__delitem__("token")
         self.assertEqual(None, UCloudEvent.get_token(cloud_event))
 
     def test_cloudevent_has_platform_error_when_platform_error_exists(self):
         cloud_event = build_cloud_event_for_test()
         cloud_event.__setitem__("commstatus", UCode.ABORTED)
-        self.assertEqual(10, UCloudEvent.get_communication_status(cloud_event))
-
-    def test_cloudevent_has_platform_error_when_platform_error_does_not_exist(self):
-        cloud_event = build_cloud_event_for_test()
-        self.assertEqual(UCode.OK, UCloudEvent.get_communication_status(cloud_event))
-
-    def test_extract_platform_error_from_cloudevent_when_platform_error_exists_in_wrong_format(self):
+        self.assertEqual(
+            UCode.ABORTED, UCloudEvent.get_communication_status(cloud_event)
+        )
+
+    def test_cloudevent_has_platform_error_when_platform_error_does_not_exist(
+        self,
+    ):
+        cloud_event = build_cloud_event_for_test()
+        self.assertEqual(
+            UCode.OK, UCloudEvent.get_communication_status(cloud_event)
+        )
+
+    def test_extract_platform_error_from_cloudevent_when_platform_error_exists_in_wrong_format(
+        self,
+    ):
         cloud_event = build_cloud_event_for_test()
         cloud_event.__setitem__("commstatus", "boom")
-        self.assertEqual(UCode.OK, UCloudEvent.get_communication_status(cloud_event))
+        self.assertEqual(
+            UCode.OK, UCloudEvent.get_communication_status(cloud_event)
+        )
+
+    def test_extract_platform_error_from_cloudevent_when_platform_error_exists(
+        self,
+    ):
+        cloud_event = build_cloud_event_for_test()
+        cloud_event.__setitem__("commstatus", UCode.INVALID_ARGUMENT)
+        self.assertEqual(
+            UCode.INVALID_ARGUMENT,
+            UCloudEvent.get_communication_status(cloud_event),
+        )
+
+    def test_extract_platform_error_from_cloudevent_when_platform_error_does_not_exist(
+        self,
+    ):
+        cloud_event = build_cloud_event_for_test()
+        self.assertEqual(
+            UCode.OK, UCloudEvent.get_communication_status(cloud_event)
+        )
+
+    def test_adding_platform_error_to_existing_cloudevent(
+        self,
+    ):
+        cloud_event = build_cloud_event_for_test()
+        self.assertEqual(
+            UCode.OK, UCloudEvent.get_communication_status(cloud_event)
+        )
+
+        cloud_event_1 = UCloudEvent.add_communication_status(
+            cloud_event, UCode.DEADLINE_EXCEEDED
+        )
+
+        self.assertEqual(
+            UCode.OK, UCloudEvent.get_communication_status(cloud_event)
+        )
+
+        self.assertEqual(
+            UCode.DEADLINE_EXCEEDED,
+            UCloudEvent.get_communication_status(cloud_event_1),
+        )
+
+    def test_adding_empty_platform_error_to_existing_cloudevent(
+        self,
+    ):
+        cloud_event = build_cloud_event_for_test()
+        self.assertEqual(
+            UCode.OK, UCloudEvent.get_communication_status(cloud_event)
+        )
+
+        cloud_event_1 = UCloudEvent.add_communication_status(cloud_event, None)
+
+        self.assertEqual(
+            UCode.OK, UCloudEvent.get_communication_status(cloud_event)
+        )
+
+        self.assertEqual(cloud_event, cloud_event_1)
+
+    def test_extract_creation_timestamp_from_cloudevent_UUID_Id_when_not_a_UUIDV8_id(
+        self,
+    ):
+        cloud_event = build_cloud_event_for_test()
+        self.assertEqual(None, UCloudEvent.get_creation_timestamp(cloud_event))
+
+    def test_extract_creation_timestamp_from_cloudevent_UUIDV8_Id_when_UUIDV8_id_is_valid(
+        self,
+    ):
+        uuid = Factories.UPROTOCOL.create()
+        str_uuid = LongUuidSerializer.instance().serialize(uuid)
+        cloud_event = build_cloud_event_for_test_with_id(str_uuid)
+        maybe_creation_timestamp = UCloudEvent.get_creation_timestamp(
+            cloud_event
+        )
+        self.assertIsNotNone(maybe_creation_timestamp)
+        creation_timestamp = maybe_creation_timestamp / 1000
+
+        now_timestamp = datetime.now(timezone.utc).timestamp()
+        self.assertAlmostEqual(creation_timestamp, now_timestamp, delta=1)
 
     def test_cloudevent_is_not_expired_cd_when_no_ttl_configured(self):
         cloud_event = build_cloud_event_for_test()
         cloud_event.__delitem__("ttl")
-        self.assertFalse(UCloudEvent.is_expired_by_cloud_event_creation_date(cloud_event))
+        self.assertFalse(
+            UCloudEvent.is_expired_by_cloud_event_creation_date(cloud_event)
+        )
 
     def test_cloudevent_is_not_expired_cd_when_ttl_is_zero(self):
         cloud_event = build_cloud_event_for_test()
         cloud_event.__setitem__("ttl", 0)
-        self.assertFalse(UCloudEvent.is_expired_by_cloud_event_creation_date(cloud_event))
+        self.assertFalse(
+            UCloudEvent.is_expired_by_cloud_event_creation_date(cloud_event)
+        )
 
     def test_cloudevent_is_not_expired_cd_when_ttl_is_minus_one(self):
         cloud_event = build_cloud_event_for_test()
         cloud_event.__setitem__("ttl", -1)
-        self.assertFalse(UCloudEvent.is_expired_by_cloud_event_creation_date(cloud_event))
+        self.assertFalse(
+            UCloudEvent.is_expired_by_cloud_event_creation_date(cloud_event)
+        )
+
+    def test_cloudevent_is_expired_cd_when_ttl_is_one(self):
+        cloud_event = build_cloud_event_for_test()
+        cloud_event.__setitem__("ttl", 1)
+        time.sleep(0.002)
+        self.assertTrue(
+            UCloudEvent.is_expired_by_cloud_event_creation_date(cloud_event)
+        )
 
     def test_cloudevent_is_expired_when_ttl_1_mili(self):
         uuid = Factories.UPROTOCOL.create()
         str_uuid = LongUuidSerializer.instance().serialize(uuid)
         cloud_event = build_cloud_event_for_test()
         cloud_event.__setitem__("ttl", 1)
-        cloud_event.__setitem__('id', str_uuid)
+        cloud_event.__setitem__("id", str_uuid)
         time.sleep(8)
         self.assertTrue(UCloudEvent.is_expired(cloud_event))
 
     def test_cloudevent_is_expired_for_invalid_uuid(self):
-        uuid = Factories.UPROTOCOL.create()
         cloud_event = build_cloud_event_for_test()
         cloud_event.__setitem__("ttl", 50000)
-        cloud_event.__setitem__('id', "")
+        cloud_event.__setitem__("id", "")
         self.assertFalse(UCloudEvent.is_expired(cloud_event))
 
     def test_cloudevent_has_a_UUIDV8_id(self):
         uuid = Factories.UPROTOCOL.create()
         str_uuid = LongUuidSerializer.instance().serialize(uuid)
         cloud_event = build_cloud_event_for_test()
-        cloud_event.__setitem__('id', str_uuid)
+        cloud_event.__setitem__("id", str_uuid)
         self.assertTrue(UCloudEvent.is_cloud_event_id(cloud_event))
 
     def test_to_message_with_valid_event(self):
         # additional attributes
-        u_cloud_event_attributes = UCloudEventAttributesBuilder().with_priority(
-            UPriority.UPRIORITY_CS2).with_ttl(3).build()
-        cloud_event = CloudEventFactory.publish(build_uri_for_test(), build_proto_payload_for_test(),
-                                                u_cloud_event_attributes)
+        u_cloud_event_attributes = (
+            UCloudEventAttributesBuilder()
+            .with_priority(UPriority.UPRIORITY_CS2)
+            .with_ttl(3)
+            .build()
+        )
+        cloud_event = CloudEventFactory.publish(
+            build_uri_for_test(),
+            build_proto_payload_for_test(),
+            u_cloud_event_attributes,
+        )
         u_message = UCloudEvent.toMessage(cloud_event)
         self.assertIsNotNone(u_message)
 
     def test_from_message_with_valid_message(self):
         # additional attributes
-        u_cloud_event_attributes = UCloudEventAttributesBuilder().with_priority(
-            UPriority.UPRIORITY_CS2).with_ttl(3).build()
-        cloud_event = CloudEventFactory.publish(build_uri_for_test(), build_proto_payload_for_test(),
-                                                u_cloud_event_attributes)
+        u_cloud_event_attributes = (
+            UCloudEventAttributesBuilder()
+            .with_priority(UPriority.UPRIORITY_CS2)
+            .with_ttl(3)
+            .with_traceparent("someParent")
+            .build()
+        )
+        cloud_event = CloudEventFactory.publish(
+            build_uri_for_test(),
+            build_proto_payload_for_test(),
+            u_cloud_event_attributes,
+        )
         u_message = UCloudEvent.toMessage(cloud_event)
         self.assertIsNotNone(u_message)
         cloud_event1 = UCloudEvent.fromMessage(u_message)
         self.assertIsNotNone(cloud_event1)
         cloud_event.__delitem__("time")
         cloud_event1.__delitem__("time")
         self.assertEqual(cloud_event, cloud_event1)
         self.assertEqual(cloud_event.get_data(), cloud_event1.get_data())
-        self.assertEqual(UCloudEvent.get_source(cloud_event), UCloudEvent.get_source(cloud_event1))
-        self.assertEqual(UCloudEvent.get_specversion(cloud_event), UCloudEvent.get_specversion(cloud_event1))
-        self.assertEqual(UCloudEvent.get_priority(cloud_event), UCloudEvent.get_priority(cloud_event1))
-        self.assertEqual(UCloudEvent.get_id(cloud_event), UCloudEvent.get_id(cloud_event1))
-        self.assertEqual(UCloudEvent.get_type(cloud_event), UCloudEvent.get_type(cloud_event1))
+        self.assertEqual(
+            UCloudEvent.get_source(cloud_event),
+            UCloudEvent.get_source(cloud_event1),
+        )
+        self.assertEqual(
+            UCloudEvent.get_specversion(cloud_event),
+            UCloudEvent.get_specversion(cloud_event1),
+        )
+        self.assertEqual(
+            UCloudEvent.get_priority(cloud_event),
+            UCloudEvent.get_priority(cloud_event1),
+        )
+        self.assertEqual(
+            UCloudEvent.get_id(cloud_event), UCloudEvent.get_id(cloud_event1)
+        )
+        self.assertEqual(
+            UCloudEvent.get_type(cloud_event),
+            UCloudEvent.get_type(cloud_event1),
+        )
+
+
 
     def test_to_from_message_from_request_cloudevent(self):
         # additional attributes
-        u_cloud_event_attributes = UCloudEventAttributesBuilder().with_priority(
-            UPriority.UPRIORITY_CS2).with_ttl(3).with_token("someOAuthToken").build()
-
-        cloud_event = CloudEventFactory.request(build_uri_for_test(), "//bo.cloud/petapp/1/rpc.response",
-                                                CloudEventFactory.generate_cloud_event_id(),
-                                                build_proto_payload_for_test(),
-                                                u_cloud_event_attributes)
+        u_cloud_event_attributes = (
+            UCloudEventAttributesBuilder()
+            .with_priority(UPriority.UPRIORITY_CS2)
+            .with_ttl(3)
+            .with_token("someOAuthToken")
+            .build()
+        )
+
+        cloud_event = CloudEventFactory.request(
+            build_uri_for_test(),
+            "//bo.cloud/petapp/1/rpc.response",
+            CloudEventFactory.generate_cloud_event_id(),
+            build_proto_payload_for_test(),
+            u_cloud_event_attributes,
+        )
         result = UCloudEvent.toMessage(cloud_event)
         self.assertIsNotNone(result)
-        self.assertEqual(UCloudEvent.get_ttl(cloud_event), result.attributes.ttl)
-        self.assertEqual(UCloudEvent.get_token(cloud_event), result.attributes.token)
-        self.assertEqual(UCloudEvent.get_sink(cloud_event),
-                          LongUriSerializer().serialize(result.attributes.sink))
-        self.assertEqual(UCloudEvent.get_payload(cloud_event).SerializeToString(), result.payload.value)
-        self.assertEqual(UCloudEvent.get_source(cloud_event),
-                          LongUriSerializer().serialize(result.attributes.source))
-        self.assertEqual(UCloudEvent.get_priority(cloud_event),
-                          UPriority.Name(result.attributes.priority))
+        self.assertEqual(
+            UCloudEvent.get_ttl(cloud_event), result.attributes.ttl
+        )
+        self.assertEqual(
+            UCloudEvent.get_token(cloud_event), result.attributes.token
+        )
+        self.assertEqual(
+            UCloudEvent.get_sink(cloud_event),
+            LongUriSerializer().serialize(result.attributes.sink),
+        )
+        self.assertEqual(
+            UCloudEvent.get_payload(cloud_event).SerializeToString(),
+            result.payload.value,
+        )
+        self.assertEqual(
+            UCloudEvent.get_source(cloud_event),
+            LongUriSerializer().serialize(result.attributes.source),
+        )
+        self.assertEqual(
+            UCloudEvent.get_priority(cloud_event),
+            UPriority.Name(result.attributes.priority),
+        )
 
         cloud_event1 = UCloudEvent.fromMessage(result)
         cloud_event.__delitem__("time")
         cloud_event1.__delitem__("time")
         self.assertEqual(cloud_event, cloud_event1)
         self.assertEqual(cloud_event.get_data(), cloud_event1.get_data())
-        self.assertEqual(UCloudEvent.get_source(cloud_event), UCloudEvent.get_source(cloud_event1))
-        self.assertEqual(UCloudEvent.get_sink(cloud_event), UCloudEvent.get_sink(cloud_event1))
-        self.assertEqual(UCloudEvent.get_specversion(cloud_event), UCloudEvent.get_specversion(cloud_event1))
-        self.assertEqual(UCloudEvent.get_priority(cloud_event), UCloudEvent.get_priority(cloud_event1))
-        self.assertEqual(UCloudEvent.get_id(cloud_event), UCloudEvent.get_id(cloud_event1))
-        self.assertEqual(UCloudEvent.get_type(cloud_event), UCloudEvent.get_type(cloud_event1))
-        self.assertEqual(UCloudEvent.get_request_id(cloud_event), UCloudEvent.get_request_id(cloud_event1))
+        self.assertEqual(
+            UCloudEvent.get_source(cloud_event),
+            UCloudEvent.get_source(cloud_event1),
+        )
+        self.assertEqual(
+            UCloudEvent.get_sink(cloud_event),
+            UCloudEvent.get_sink(cloud_event1),
+        )
+        self.assertEqual(
+            UCloudEvent.get_specversion(cloud_event),
+            UCloudEvent.get_specversion(cloud_event1),
+        )
+        self.assertEqual(
+            UCloudEvent.get_priority(cloud_event),
+            UCloudEvent.get_priority(cloud_event1),
+        )
+        self.assertEqual(
+            UCloudEvent.get_id(cloud_event), UCloudEvent.get_id(cloud_event1)
+        )
+        self.assertEqual(
+            UCloudEvent.get_type(cloud_event),
+            UCloudEvent.get_type(cloud_event1),
+        )
+        self.assertEqual(
+            UCloudEvent.get_request_id(cloud_event),
+            UCloudEvent.get_request_id(cloud_event1),
+        )
 
     def test_to_from_message_from_request_cloudevent_without_attributes(self):
         # additional attributes
         u_cloud_event_attributes = UCloudEventAttributesBuilder().build()
 
-        cloud_event = CloudEventFactory.request(build_uri_for_test(), "//bo.cloud/petapp/1/rpc.response",
-                                                CloudEventFactory.generate_cloud_event_id(),
-                                                build_proto_payload_for_test(),
-                                                u_cloud_event_attributes)
+        cloud_event = CloudEventFactory.request(
+            build_uri_for_test(),
+            "//bo.cloud/petapp/1/rpc.response",
+            CloudEventFactory.generate_cloud_event_id(),
+            build_proto_payload_for_test(),
+            u_cloud_event_attributes,
+        )
         result = UCloudEvent.toMessage(cloud_event)
         self.assertIsNotNone(result)
-        self.assertFalse(result.attributes.HasField('ttl'))
-        self.assertEqual(UCloudEvent.get_sink(cloud_event),
-                     LongUriSerializer().serialize(result.attributes.sink))
-        self.assertEqual(UCloudEvent.get_payload(cloud_event).SerializeToString(), result.payload.value)
-        self.assertEqual(UCloudEvent.get_source(cloud_event), LongUriSerializer().serialize(result.attributes.source))
+        self.assertFalse(result.attributes.HasField("ttl"))
+        self.assertEqual(
+            UCloudEvent.get_sink(cloud_event),
+            LongUriSerializer().serialize(result.attributes.sink),
+        )
+        self.assertEqual(
+            UCloudEvent.get_payload(cloud_event).SerializeToString(),
+            result.payload.value,
+        )
+        self.assertEqual(
+            UCloudEvent.get_source(cloud_event),
+            LongUriSerializer().serialize(result.attributes.source),
+        )
         self.assertEqual(result.attributes.priority, 0)
 
         cloud_event1 = UCloudEvent.fromMessage(result)
         self.assertEqual(cloud_event.get_data(), cloud_event1.get_data())
-        self.assertEqual(UCloudEvent.get_source(cloud_event),UCloudEvent.get_source(cloud_event1))
-        self.assertEqual(UCloudEvent.get_sink(cloud_event),UCloudEvent.get_sink(cloud_event1))
-        self.assertEqual(UCloudEvent.get_specversion(cloud_event),UCloudEvent.get_specversion(cloud_event1))
-        self.assertEqual(UCloudEvent.get_priority(cloud_event),UCloudEvent.get_priority(cloud_event1))
-        self.assertEqual(UCloudEvent.get_id(cloud_event),UCloudEvent.get_id(cloud_event1))
-        self.assertEqual(UCloudEvent.get_type(cloud_event),UCloudEvent.get_type(cloud_event1))
-        self.assertEqual(UCloudEvent.get_request_id(cloud_event),UCloudEvent.get_request_id(cloud_event1))
+        self.assertEqual(
+            UCloudEvent.get_source(cloud_event),
+            UCloudEvent.get_source(cloud_event1),
+        )
+        self.assertEqual(
+            UCloudEvent.get_sink(cloud_event),
+            UCloudEvent.get_sink(cloud_event1),
+        )
+        self.assertEqual(
+            UCloudEvent.get_specversion(cloud_event),
+            UCloudEvent.get_specversion(cloud_event1),
+        )
+        self.assertEqual(
+            UCloudEvent.get_priority(cloud_event),
+            UCloudEvent.get_priority(cloud_event1),
+        )
+        self.assertEqual(
+            UCloudEvent.get_id(cloud_event), UCloudEvent.get_id(cloud_event1)
+        )
+        self.assertEqual(
+            UCloudEvent.get_type(cloud_event),
+            UCloudEvent.get_type(cloud_event1),
+        )
+        self.assertEqual(
+            UCloudEvent.get_request_id(cloud_event),
+            UCloudEvent.get_request_id(cloud_event1),
+        )
 
     def test_to_from_message_from_UCP_cloudevent(self):
         # additional attributes
-        u_cloud_event_attributes = UCloudEventAttributesBuilder().with_ttl(3).with_token("someOAuthToken").build()
-
-        cloud_event = CloudEventFactory.request(build_uri_for_test(), "//bo.cloud/petapp/1/rpc.response",
-                                                CloudEventFactory.generate_cloud_event_id(),
-                                                build_proto_payload_for_test(),
-                                                u_cloud_event_attributes)
+        u_cloud_event_attributes = (
+            UCloudEventAttributesBuilder()
+            .with_ttl(3)
+            .with_token("someOAuthToken")
+            .build()
+        )
+
+        cloud_event = CloudEventFactory.request(
+            build_uri_for_test(),
+            "//bo.cloud/petapp/1/rpc.response",
+            CloudEventFactory.generate_cloud_event_id(),
+            build_proto_payload_for_test(),
+            u_cloud_event_attributes,
+        )
         cloud_event.__setitem__("priority", "CS4")
+        cloud_event.__setitem__("commstatus", 16)
+        cloud_event.__setitem__("permission_level", 4)
 
         result = UCloudEvent.toMessage(cloud_event)
         self.assertIsNotNone(result)
-        self.assertEqual(UPriority.UPRIORITY_CS4,result.attributes.priority)
+        self.assertEqual(UPriority.UPRIORITY_CS4, result.attributes.priority)
         cloud_event1 = UCloudEvent.fromMessage(result)
-        self.assertEqual(UCloudEvent.get_priority(cloud_event1),UPriority.Name(result.attributes.priority))
-
+        self.assertEqual(
+            UCloudEvent.get_priority(cloud_event1),
+            UPriority.Name(result.attributes.priority),
+        )
+
+    def test_from_message_with_null_message(self):
+        with self.assertRaises(ValueError) as context:
+            UCloudEvent.fromMessage(None)
+            self.assertTrue("message cannot be null." in context.exception)
+
+    def test_cloud_event_to_string(self):
+        u_cloud_event_attributes = (
+            UCloudEventAttributesBuilder()
+            .with_ttl(3)
+            .with_token("someOAuthToken")
+            .build()
+        )
+
+        cloud_event = CloudEventFactory.request(
+            build_uri_for_test(),
+            "//bo.cloud/petapp/1/rpc.response",
+            CloudEventFactory.generate_cloud_event_id(),
+            build_proto_payload_for_test(),
+            u_cloud_event_attributes,
+        )
+        cloud_event_string = UCloudEvent.to_string(cloud_event)
+        self.assertTrue(
+            "source='/body.access//door.front_left#Door', sink='//bo.cloud/petapp/1/rpc.response', type='req.v1'}"
+            in cloud_event_string
+        )
+
+    def test_cloud_event_to_string_none(self):
+        cloud_event_string = UCloudEvent.to_string(None)
+        self.assertEqual(
+            cloud_event_string, "null"
+        )
+
+    def test_get_upayload_format_from_content_type(self):
+        new_format = UCloudEvent().get_upayload_format_from_content_type("application/json")
+        self.assertEqual(new_format, UPayloadFormat.UPAYLOAD_FORMAT_JSON)
+
+    def test_to_message_none_entry(self):
+        with self.assertRaises(ValueError) as context:
+            UCloudEvent().toMessage(None)
+            self.assertTrue("Cloud Event can't be None" in context.exception)
```

### Comparing `up_python-0.1.1.dev0/tests/test_cloudevent/test_datamodel/test_ucloudeventattributes.py` & `up_python-0.1.2.dev0/tests/test_cloudevent/test_datamodel/test_ucloudeventattributes.py`

 * *Files 26% similar despite different names*

```diff
@@ -37,14 +37,31 @@
     def test_to_string(self):
         u_cloud_event_attributes = UCloudEventAttributesBuilder().with_hash("somehash").with_priority(
             UPriority.UPRIORITY_CS1).with_ttl(3).with_token("someOAuthToken").build()
 
         expected = "UCloudEventAttributes{hash='somehash', priority=UPRIORITY_CS1, ttl=3, token='someOAuthToken'}"
         self.assertEqual(expected, str(u_cloud_event_attributes))
 
+    def test_create_valid_with_blank_traceparent(self):
+        u_cloud_event_attributes = UCloudEventAttributesBuilder().with_hash("somehash").with_priority(
+            UPriority.UPRIORITY_CS1).with_ttl(3).with_token("someOAuthToken").with_traceparent(" ").build()
+        self.assertTrue(u_cloud_event_attributes.get_hash() is not None)
+        self.assertEqual("somehash", u_cloud_event_attributes.get_hash())
+        self.assertFalse(u_cloud_event_attributes.get_traceparent() is not None)
+
+    def test_create_empty_with_only_traceparent(self):
+        u_cloud_event_attributes = UCloudEventAttributesBuilder().with_traceparent("someTraceParent").build()
+        self.assertFalse(u_cloud_event_attributes.get_hash() is not None)
+        self.assertFalse(u_cloud_event_attributes.get_priority() is not None)
+        self.assertFalse(u_cloud_event_attributes.get_token() is not None)
+        self.assertFalse(u_cloud_event_attributes.get_ttl() is not None)
+        self.assertTrue(u_cloud_event_attributes.get_traceparent() is not None)
+        self.assertFalse(u_cloud_event_attributes.is_empty())
+        self.assertEqual("someTraceParent", u_cloud_event_attributes.get_traceparent())
+
     def test_create_valid(self):
         u_cloud_event_attributes = UCloudEventAttributesBuilder().with_hash("somehash").with_priority(
             UPriority.UPRIORITY_CS6).with_ttl(3).with_token("someOAuthToken").build()
 
         self.assertEqual("somehash", u_cloud_event_attributes.get_hash())
         self.assertEqual(UPriority.Name(UPriority.UPRIORITY_CS6), u_cloud_event_attributes.get_priority())
         self.assertEqual(3, u_cloud_event_attributes.get_ttl())
@@ -77,10 +94,33 @@
 
         u_cloud_event_attributes4 = UCloudEventAttributesBuilder().with_priority(UPriority.UPRIORITY_CS0).build()
         self.assertFalse(u_cloud_event_attributes4.is_empty())
 
         u_cloud_event_attributes5 = UCloudEventAttributesBuilder().with_ttl(8).build()
         self.assertFalse(u_cloud_event_attributes5.is_empty())
 
+    def test__eq__is_same(self):
+        u_cloud_event_attributes = UCloudEventAttributesBuilder().with_hash("  ").with_token("  ").build()
+        self.assertTrue(u_cloud_event_attributes.__eq__(u_cloud_event_attributes))
+
+    def test__eq__is_equal(self):
+        u_cloud_event_attributes_1 = UCloudEventAttributesBuilder().with_hash("  ").with_token("  ").build()
+        u_cloud_event_attributes_2 = UCloudEventAttributesBuilder().with_hash("  ").with_token("  ").build()
+        self.assertTrue(u_cloud_event_attributes_1.__eq__(u_cloud_event_attributes_2))
+    
+    def test__eq__is_not_equal(self):
+        u_cloud_event_attributes_1 = UCloudEventAttributesBuilder().with_hash("  ").with_token("  ").build()
+        u_cloud_event_attributes_2 = UCloudEventAttributesBuilder().with_hash("  ").with_token("12345").build()
+        self.assertFalse(u_cloud_event_attributes_1.__eq__(u_cloud_event_attributes_2))
+
+    def test__hash__same(self):
+        u_cloud_event_attributes_1 = UCloudEventAttributesBuilder().with_hash("  ").with_token("  ").build()
+        self.assertEqual(hash(u_cloud_event_attributes_1), hash(u_cloud_event_attributes_1))
+    
+    def test__hash__different(self):
+        u_cloud_event_attributes_1 = UCloudEventAttributesBuilder().with_hash("  ").with_token("  ").build()
+        u_cloud_event_attributes_2 = UCloudEventAttributesBuilder().with_hash("  ").with_token("12345").build()
+        self.assertNotEqual(hash(u_cloud_event_attributes_1), hash(u_cloud_event_attributes_2))
+    
 
 if __name__ == '__main__':
     unittest.main()
```

### Comparing `up_python-0.1.1.dev0/tests/test_cloudevent/test_factory/cloudevent.json` & `up_python-0.1.2.dev0/tests/test_cloudevent/test_factory/cloudevent.json`

 * *Files identical despite different names*

### Comparing `up_python-0.1.1.dev0/tests/test_cloudevent/test_factory/test_cloudeventfactory.py` & `up_python-0.1.2.dev0/tests/test_cloudevent/test_factory/test_cloudeventfactory.py`

 * *Files 7% similar despite different names*

```diff
@@ -25,365 +25,576 @@
 # -------------------------------------------------------------------------
 
 
 import unittest
 import json
 import os
 from google.protobuf import any_pb2
-from uprotocol.cloudevent.datamodel.ucloudeventattributes import UCloudEventAttributesBuilder, \
-    UCloudEventAttributes
+from uprotocol.cloudevent.datamodel.ucloudeventattributes import (
+    UCloudEventAttributesBuilder,
+    UCloudEventAttributes,
+)
 from uprotocol.cloudevent.factory.cloudeventfactory import CloudEventFactory
 from uprotocol.cloudevent.factory.ucloudevent import UCloudEvent
-from uprotocol.cloudevent.serialize.base64protobufserializer import Base64ProtobufSerializer
-from uprotocol.cloudevent.serialize.cloudeventtojsonserializer import CloudEventToJsonSerializer
+from uprotocol.cloudevent.serialize.base64protobufserializer import (
+    Base64ProtobufSerializer,
+)
+from uprotocol.cloudevent.serialize.cloudeventtojsonserializer import (
+    CloudEventToJsonSerializer,
+)
 from uprotocol.cloudevent.cloudevents_pb2 import CloudEvent
 from uprotocol.proto.uattributes_pb2 import UMessageType, UPriority
 from uprotocol.proto.uri_pb2 import UUri, UEntity, UResource
 from uprotocol.proto.ustatus_pb2 import UCode
 
 from uprotocol.uri.serializer.longuriserializer import LongUriSerializer
 
 
 def get_json_object():
     current_directory = os.getcwd()
-    json_file_path = os.path.join(current_directory, "tests","test_cloudevent","test_factory","cloudevent.json")
+    json_file_path = os.path.join(
+        current_directory,
+        "tests",
+        "test_cloudevent",
+        "test_factory",
+        "cloudevent.json",
+    )
 
-    with open(json_file_path, 'r') as json_file:
+    with open(json_file_path, "r") as json_file:
         json_data = json.load(json_file)
 
     return json_data
 
 
 def build_uri_for_test():
-    uri = UUri(entity=UEntity(name="body.access"),
-               resource=UResource(name="door", instance="front_left", message="Door"))
+    uri = UUri(
+        entity=UEntity(name="body.access"),
+        resource=UResource(name="door", instance="front_left", message="Door"),
+    )
     return LongUriSerializer().serialize(uri)
 
 
 def build_proto_payload_for_test():
-    ce_proto = CloudEvent(spec_version="1.0", source="https://example.com", id="hello", type="example.demo",
-                          proto_data=any_pb2.Any())
+    ce_proto = CloudEvent(
+        spec_version="1.0",
+        source="https://example.com",
+        id="hello",
+        type="example.demo",
+        proto_data=any_pb2.Any(),
+    )
 
     any_obj = any_pb2.Any()
     any_obj.Pack(ce_proto)
     return any_obj
 
 
 class TestCloudEventFactory(unittest.TestCase):
     DATA_CONTENT_TYPE = CloudEventFactory.PROTOBUF_CONTENT_TYPE
 
     def test_all_cloud_events_from_json(self):
         cloudevents = get_json_object()
         for ce_json in cloudevents:
-            bytes_ce = Base64ProtobufSerializer().serialize(ce_json['serialized_ce'])
+            bytes_ce = Base64ProtobufSerializer().serialize(
+                ce_json["serialized_ce"]
+            )
             cloudevent = CloudEventToJsonSerializer().deserialize(bytes_ce)
-            self.assertEqual(UCloudEvent.get_id(cloudevent), ce_json['id'])
-            self.assertEqual(UCloudEvent.get_specversion(cloudevent), ce_json['specversion'])
-            if 'source' in ce_json:
-                self.assertEqual(UCloudEvent.get_source(cloudevent), ce_json['source'])
-            if 'sink' in ce_json:
-                self.assertEqual(UCloudEvent.get_sink(cloudevent), ce_json['sink'])
-            if 'type' in ce_json:
-                self.assertEqual(UCloudEvent.get_type(cloudevent), ce_json['type'])
-            if 'priority' in ce_json:
-                self.assertEqual(UCloudEvent.get_priority(cloudevent), ce_json['priority'])
-            if 'ttl' in ce_json:
-                self.assertEqual(UCloudEvent.get_ttl(cloudevent), ce_json['ttl'])
-            if 'hash' in ce_json:
-                self.assertEqual(UCloudEvent.get_hash(cloudevent), ce_json['hash'])
-            if 'token' in ce_json:
-                self.assertEqual(UCloudEvent.get_token(cloudevent), ce_json['token'])
-            if 'dataschema' in ce_json:
-                self.assertEqual(UCloudEvent.get_data_schema(cloudevent), ce_json['dataschema'])
-            if 'datacontenttype' in ce_json:
-                self.assertEqual(UCloudEvent.get_data_content_type(cloudevent), ce_json['datacontenttype'])
-            if 'commstatus' in ce_json:
-                self.assertEqual(UCloudEvent.get_communication_status(cloudevent), ce_json['commstatus'])
+            self.assertEqual(UCloudEvent.get_id(cloudevent), ce_json["id"])
+            self.assertEqual(
+                UCloudEvent.get_specversion(cloudevent), ce_json["specversion"]
+            )
+            if "source" in ce_json:
+                self.assertEqual(
+                    UCloudEvent.get_source(cloudevent), ce_json["source"]
+                )
+            if "sink" in ce_json:
+                self.assertEqual(
+                    UCloudEvent.get_sink(cloudevent), ce_json["sink"]
+                )
+            if "type" in ce_json:
+                self.assertEqual(
+                    UCloudEvent.get_type(cloudevent), ce_json["type"]
+                )
+            if "priority" in ce_json:
+                self.assertEqual(
+                    UCloudEvent.get_priority(cloudevent), ce_json["priority"]
+                )
+            if "ttl" in ce_json:
+                self.assertEqual(
+                    UCloudEvent.get_ttl(cloudevent), ce_json["ttl"]
+                )
+            if "hash" in ce_json:
+                self.assertEqual(
+                    UCloudEvent.get_hash(cloudevent), ce_json["hash"]
+                )
+            if "token" in ce_json:
+                self.assertEqual(
+                    UCloudEvent.get_token(cloudevent), ce_json["token"]
+                )
+            if "dataschema" in ce_json:
+                self.assertEqual(
+                    UCloudEvent.get_data_schema(cloudevent),
+                    ce_json["dataschema"],
+                )
+            if "datacontenttype" in ce_json:
+                self.assertEqual(
+                    UCloudEvent.get_data_content_type(cloudevent),
+                    ce_json["datacontenttype"],
+                )
+            if "commstatus" in ce_json:
+                self.assertEqual(
+                    UCloudEvent.get_communication_status(cloudevent),
+                    ce_json["commstatus"],
+                )
 
     def test_create_base_cloud_event(self):
         source = build_uri_for_test()
 
         # fake payload
         proto_payload = build_proto_payload_for_test()
 
         # additional attributes
-        u_cloud_event_attributes = UCloudEventAttributesBuilder().with_hash("somehash").with_priority(
-            UPriority.UPRIORITY_CS1).with_ttl(3).with_token("someOAuthToken").build()
+        u_cloud_event_attributes = (
+            UCloudEventAttributesBuilder()
+            .with_hash("somehash")
+            .with_priority(UPriority.UPRIORITY_CS1)
+            .with_ttl(3)
+            .with_token("someOAuthToken")
+            .with_traceparent("sometraceparent")
+            .build()
+        )
 
         # build the cloud event
-        cloud_event = CloudEventFactory.build_base_cloud_event("testme", source, proto_payload.SerializeToString(),
-                                                               proto_payload.type_url, u_cloud_event_attributes,
-                                                               UCloudEvent.get_event_type(
-                                                                   UMessageType.UMESSAGE_TYPE_PUBLISH))
+        cloud_event = CloudEventFactory.build_base_cloud_event(
+            "testme",
+            source,
+            proto_payload.SerializeToString(),
+            proto_payload.type_url,
+            u_cloud_event_attributes,
+            UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_PUBLISH),
+        )
 
         self.assertEqual("1.0", UCloudEvent.get_specversion(cloud_event))
         self.assertEqual("testme", UCloudEvent.get_id(cloud_event))
         self.assertEqual(source, UCloudEvent.get_source(cloud_event))
-        self.assertEqual('pub.v1', UCloudEvent.get_type(cloud_event))
+        self.assertEqual("pub.v1", UCloudEvent.get_type(cloud_event))
         self.assertNotIn("sink", cloud_event.get_attributes())
         self.assertEqual("somehash", UCloudEvent.get_hash(cloud_event))
-        self.assertEqual(UPriority.Name(UPriority.UPRIORITY_CS1), UCloudEvent.get_priority(cloud_event))
+        self.assertEqual(
+            UPriority.Name(UPriority.UPRIORITY_CS1),
+            UCloudEvent.get_priority(cloud_event),
+        )
         self.assertEqual(3, UCloudEvent.get_ttl(cloud_event))
         self.assertEqual("someOAuthToken", UCloudEvent.get_token(cloud_event))
-        self.assertEqual(proto_payload.SerializeToString(), cloud_event.get_data())
+        self.assertEqual(
+            "sometraceparent", UCloudEvent.get_traceparent(cloud_event)
+        )
+        self.assertEqual(
+            proto_payload.SerializeToString(), cloud_event.get_data()
+        )
 
     def test_create_base_cloud_event_with_datacontenttype_and_schema(self):
         source = build_uri_for_test()
 
         # fake payload
         proto_payload = build_proto_payload_for_test()
 
         # additional attributes
-        u_cloud_event_attributes = UCloudEventAttributesBuilder().with_hash("somehash").with_priority(
-            UPriority.UPRIORITY_CS1).with_ttl(3).with_token("someOAuthToken").build()
+        u_cloud_event_attributes = (
+            UCloudEventAttributesBuilder()
+            .with_hash("somehash")
+            .with_priority(UPriority.UPRIORITY_CS1)
+            .with_ttl(3)
+            .with_token("someOAuthToken")
+            .build()
+        )
 
         # build the cloud event
-        cloud_event = CloudEventFactory.build_base_cloud_event("testme", source, proto_payload.SerializeToString(),
-                                                               proto_payload.type_url, u_cloud_event_attributes,
-                                                               UCloudEvent.get_event_type(
-                                                                   UMessageType.UMESSAGE_TYPE_PUBLISH))
-
-        cloud_event.__setitem__('datacontenttype', CloudEventFactory.PROTOBUF_CONTENT_TYPE)
-        cloud_event.__setitem__('dataschema', proto_payload.type_url)
+        cloud_event = CloudEventFactory.build_base_cloud_event(
+            "testme",
+            source,
+            proto_payload.SerializeToString(),
+            proto_payload.type_url,
+            u_cloud_event_attributes,
+            UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_PUBLISH),
+        )
+
+        cloud_event.__setitem__(
+            "datacontenttype", CloudEventFactory.PROTOBUF_CONTENT_TYPE
+        )
+        cloud_event.__setitem__("dataschema", proto_payload.type_url)
 
         # test all attributes
         self.assertEqual("1.0", UCloudEvent.get_specversion(cloud_event))
         self.assertEqual("testme", UCloudEvent.get_id(cloud_event))
         self.assertEqual(source, UCloudEvent.get_source(cloud_event))
-        self.assertEqual(UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_PUBLISH),
-                         UCloudEvent.get_type(cloud_event))
-        self.assertEqual(self.DATA_CONTENT_TYPE, UCloudEvent.get_data_content_type(cloud_event))
-        self.assertEqual(proto_payload.type_url, UCloudEvent.get_data_schema(cloud_event))
+        self.assertEqual(
+            UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_PUBLISH),
+            UCloudEvent.get_type(cloud_event),
+        )
+        self.assertEqual(
+            self.DATA_CONTENT_TYPE,
+            UCloudEvent.get_data_content_type(cloud_event),
+        )
+        self.assertEqual(
+            proto_payload.type_url, UCloudEvent.get_data_schema(cloud_event)
+        )
         self.assertNotIn("sink", cloud_event.get_attributes())
         self.assertEqual("somehash", UCloudEvent.get_hash(cloud_event))
-        self.assertEqual(UPriority.Name(UPriority.UPRIORITY_CS1), UCloudEvent.get_priority(cloud_event))
+        self.assertEqual(
+            UPriority.Name(UPriority.UPRIORITY_CS1),
+            UCloudEvent.get_priority(cloud_event),
+        )
         self.assertEqual(3, UCloudEvent.get_ttl(cloud_event))
         self.assertEqual("someOAuthToken", UCloudEvent.get_token(cloud_event))
-        self.assertEqual(proto_payload.SerializeToString(), cloud_event.get_data())
+        self.assertEqual(
+            proto_payload.SerializeToString(), cloud_event.get_data()
+        )
 
     def test_create_base_cloud_event_without_attributes(self):
         source = build_uri_for_test()
 
         # fake payload
         proto_payload = build_proto_payload_for_test()
 
         # no additional attributes
         u_cloud_event_attributes = UCloudEventAttributes.empty()
 
         # build the cloud event
         # build the cloud event
-        cloud_event = CloudEventFactory.build_base_cloud_event("testme", source, proto_payload.SerializeToString(),
-                                                               proto_payload.type_url, u_cloud_event_attributes,
-                                                               UCloudEvent.get_event_type(
-                                                                   UMessageType.UMESSAGE_TYPE_PUBLISH))
+        cloud_event = CloudEventFactory.build_base_cloud_event(
+            "testme",
+            source,
+            proto_payload.SerializeToString(),
+            proto_payload.type_url,
+            u_cloud_event_attributes,
+            UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_PUBLISH),
+        )
 
         # test all attributes
         self.assertEqual("1.0", UCloudEvent.get_specversion(cloud_event))
         self.assertEqual("testme", UCloudEvent.get_id(cloud_event))
         self.assertEqual(source, UCloudEvent.get_source(cloud_event))
-        self.assertEqual(UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_PUBLISH),
-                         UCloudEvent.get_type(cloud_event))
+        self.assertEqual(
+            UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_PUBLISH),
+            UCloudEvent.get_type(cloud_event),
+        )
         self.assertNotIn("sink", cloud_event.get_attributes())
         self.assertNotIn("hash", cloud_event.get_attributes())
         self.assertNotIn("priority", cloud_event.get_attributes())
         self.assertNotIn("ttl", cloud_event.get_attributes())
-        self.assertEqual(proto_payload.SerializeToString(), cloud_event.get_data())
+        self.assertEqual(
+            proto_payload.SerializeToString(), cloud_event.get_data()
+        )
 
     def test_create_publish_cloud_event(self):
         # source
         source = build_uri_for_test()
 
         # fake payload
         proto_payload = build_proto_payload_for_test()
 
         # additional attributes
-        u_cloud_event_attributes = UCloudEventAttributesBuilder().with_hash("somehash").with_priority(
-            UPriority.UPRIORITY_CS1).with_ttl(3).build()
-
-        cloud_event = CloudEventFactory.publish(source, proto_payload, u_cloud_event_attributes)
+        u_cloud_event_attributes = (
+            UCloudEventAttributesBuilder()
+            .with_hash("somehash")
+            .with_priority(UPriority.UPRIORITY_CS1)
+            .with_ttl(3)
+            .build()
+        )
+
+        cloud_event = CloudEventFactory.publish(
+            source, proto_payload, u_cloud_event_attributes
+        )
 
         # test all attributes
         self.assertEqual("1.0", UCloudEvent.get_specversion(cloud_event))
         self.assertIsNotNone(UCloudEvent.get_id(cloud_event))
         self.assertEqual(source, UCloudEvent.get_source(cloud_event))
-        self.assertEqual(UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_PUBLISH),
-                         UCloudEvent.get_type(cloud_event))
+        self.assertEqual(
+            UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_PUBLISH),
+            UCloudEvent.get_type(cloud_event),
+        )
         self.assertNotIn("sink", cloud_event.get_attributes())
         self.assertEqual("somehash", UCloudEvent.get_hash(cloud_event))
-        self.assertEqual(UPriority.Name(UPriority.UPRIORITY_CS1), UCloudEvent.get_priority(cloud_event))
+        self.assertEqual(
+            UPriority.Name(UPriority.UPRIORITY_CS1),
+            UCloudEvent.get_priority(cloud_event),
+        )
         self.assertEqual(3, UCloudEvent.get_ttl(cloud_event))
 
-        self.assertEqual(proto_payload.SerializeToString(), cloud_event.get_data())
+        self.assertEqual(
+            proto_payload.SerializeToString(), cloud_event.get_data()
+        )
 
     def test_create_notification_cloud_event(self):
         # source
         source = build_uri_for_test()
 
         # sink
         sink = build_uri_for_test()
 
         # fake payload
         proto_payload = build_proto_payload_for_test()
 
         # additional attributes
 
-        u_cloud_event_attributes = UCloudEventAttributesBuilder().with_hash("somehash").with_priority(
-            UPriority.UPRIORITY_CS2).with_ttl(3).build()
+        u_cloud_event_attributes = (
+            UCloudEventAttributesBuilder()
+            .with_hash("somehash")
+            .with_priority(UPriority.UPRIORITY_CS2)
+            .with_ttl(3)
+            .build()
+        )
 
         # build the cloud event of type publish with destination - a notification
-        cloud_event = CloudEventFactory.notification(source, sink, proto_payload, u_cloud_event_attributes)
+        cloud_event = CloudEventFactory.notification(
+            source, sink, proto_payload, u_cloud_event_attributes
+        )
 
         # test all attributes
         self.assertEqual("1.0", UCloudEvent.get_specversion(cloud_event))
         self.assertIsNotNone(UCloudEvent.get_id(cloud_event))
         self.assertEqual(source, UCloudEvent.get_source(cloud_event))
 
         self.assertIn("sink", cloud_event.get_attributes())
         self.assertEqual(sink, UCloudEvent.get_sink(cloud_event))
 
-        self.assertEqual(UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_PUBLISH),
-                         UCloudEvent.get_type(cloud_event))
+        self.assertEqual(
+            UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_PUBLISH),
+            UCloudEvent.get_type(cloud_event),
+        )
         self.assertEqual("somehash", UCloudEvent.get_hash(cloud_event))
-        self.assertEqual(UPriority.Name(UPriority.UPRIORITY_CS2), UCloudEvent.get_priority(cloud_event))
+        self.assertEqual(
+            UPriority.Name(UPriority.UPRIORITY_CS2),
+            UCloudEvent.get_priority(cloud_event),
+        )
         self.assertEqual(3, UCloudEvent.get_ttl(cloud_event))
 
-        self.assertEqual(proto_payload.SerializeToString(), cloud_event.get_data())
+        self.assertEqual(
+            proto_payload.SerializeToString(), cloud_event.get_data()
+        )
 
     def test_create_request_cloud_event_from_local_use(self):
         # UriPart for the application requesting the RPC
         application_uri_for_rpc = build_uri_for_test()
 
         # service Method UriPart
         service_method_uri = build_uri_for_test()
 
         # fake payload
         proto_payload = build_proto_payload_for_test()
 
         # additional attributes
 
-        u_cloud_event_attributes = UCloudEventAttributesBuilder().with_hash("somehash").with_priority(
-            UPriority.UPRIORITY_CS2).with_ttl(3).with_token("someOAuthToken").build()
-
-        cloud_event = CloudEventFactory.request(application_uri_for_rpc, service_method_uri,
-                                                CloudEventFactory.generate_cloud_event_id(), proto_payload,
-                                                u_cloud_event_attributes)
+        u_cloud_event_attributes = (
+            UCloudEventAttributesBuilder()
+            .with_hash("somehash")
+            .with_priority(UPriority.UPRIORITY_CS2)
+            .with_ttl(3)
+            .with_token("someOAuthToken")
+            .build()
+        )
+
+        cloud_event = CloudEventFactory.request(
+            application_uri_for_rpc,
+            service_method_uri,
+            CloudEventFactory.generate_cloud_event_id(),
+            proto_payload,
+            u_cloud_event_attributes,
+        )
 
         # test all attributes
         self.assertEqual("1.0", UCloudEvent.get_specversion(cloud_event))
         self.assertIsNotNone(UCloudEvent.get_id(cloud_event))
-        self.assertEqual(application_uri_for_rpc, UCloudEvent.get_source(cloud_event))
+        self.assertEqual(
+            application_uri_for_rpc, UCloudEvent.get_source(cloud_event)
+        )
 
         self.assertIn("sink", cloud_event.get_attributes())
         self.assertEqual(service_method_uri, UCloudEvent.get_sink(cloud_event))
 
         self.assertEqual("req.v1", UCloudEvent.get_type(cloud_event))
         self.assertEqual("somehash", UCloudEvent.get_hash(cloud_event))
-        self.assertEqual(UPriority.Name(UPriority.UPRIORITY_CS2), UCloudEvent.get_priority(cloud_event))
+        self.assertEqual(
+            UPriority.Name(UPriority.UPRIORITY_CS2),
+            UCloudEvent.get_priority(cloud_event),
+        )
         self.assertEqual(3, UCloudEvent.get_ttl(cloud_event))
         self.assertEqual("someOAuthToken", UCloudEvent.get_token(cloud_event))
 
-        self.assertEqual(proto_payload.SerializeToString(), cloud_event.get_data())
+        self.assertEqual(
+            proto_payload.SerializeToString(), cloud_event.get_data()
+        )
 
     def test_create_response_cloud_event_originating_from_local_use(self):
         # UriPart for the application requesting the RPC
         application_uri_for_rpc = build_uri_for_test()
 
         # service Method UriPart
         service_method_uri = build_uri_for_test()
 
         # fake payload
         proto_payload = build_proto_payload_for_test()
 
         # additional attributes
 
-        u_cloud_event_attributes = UCloudEventAttributesBuilder().with_hash("somehash").with_priority(
-            UPriority.UPRIORITY_CS2).with_ttl(3).build()
-
-        cloud_event = CloudEventFactory.response(application_uri_for_rpc, service_method_uri,
-                                                 "requestIdFromRequestCloudEvent", proto_payload,
-                                                 u_cloud_event_attributes)
+        u_cloud_event_attributes = (
+            UCloudEventAttributesBuilder()
+            .with_hash("somehash")
+            .with_priority(UPriority.UPRIORITY_CS2)
+            .with_ttl(3)
+            .build()
+        )
+
+        cloud_event = CloudEventFactory.response(
+            application_uri_for_rpc,
+            service_method_uri,
+            "requestIdFromRequestCloudEvent",
+            proto_payload,
+            u_cloud_event_attributes,
+        )
 
         # test all attributes
         self.assertEqual("1.0", UCloudEvent.get_specversion(cloud_event))
         self.assertIsNotNone(UCloudEvent.get_id(cloud_event))
-        self.assertEqual(service_method_uri, UCloudEvent.get_source(cloud_event))
+        self.assertEqual(
+            service_method_uri, UCloudEvent.get_source(cloud_event)
+        )
 
         self.assertIn("sink", cloud_event.get_attributes())
-        self.assertEqual(application_uri_for_rpc, UCloudEvent.get_sink(cloud_event))
+        self.assertEqual(
+            application_uri_for_rpc, UCloudEvent.get_sink(cloud_event)
+        )
 
         self.assertEqual("res.v1", UCloudEvent.get_type(cloud_event))
         self.assertEqual("somehash", UCloudEvent.get_hash(cloud_event))
-        self.assertEqual(UPriority.Name(UPriority.UPRIORITY_CS2), UCloudEvent.get_priority(cloud_event))
+        self.assertEqual(
+            UPriority.Name(UPriority.UPRIORITY_CS2),
+            UCloudEvent.get_priority(cloud_event),
+        )
         self.assertEqual(3, UCloudEvent.get_ttl(cloud_event))
 
-        self.assertEqual("requestIdFromRequestCloudEvent", UCloudEvent.get_request_id(cloud_event))
+        self.assertEqual(
+            "requestIdFromRequestCloudEvent",
+            UCloudEvent.get_request_id(cloud_event),
+        )
 
         # Use assertEqual to compare byte arrays
-        self.assertEqual(proto_payload.SerializeToString(), cloud_event.get_data())
-
-    def test_create_failed_response_cloud_event_originating_from_local_use(self):
+        self.assertEqual(
+            proto_payload.SerializeToString(), cloud_event.get_data()
+        )
+
+    def test_create_failed_response_cloud_event_originating_from_local_use(
+        self,
+    ):
         # UriPart for the application requesting the RPC
         application_uri_for_rpc = build_uri_for_test()
 
         # service Method UriPart
         service_method_uri = build_uri_for_test()
 
         # additional attributes
 
-        u_cloud_event_attributes = UCloudEventAttributesBuilder().with_hash("somehash").with_priority(
-            UPriority.UPRIORITY_CS2).with_ttl(3).build()
-
-        cloud_event = CloudEventFactory.failed_response(application_uri_for_rpc, service_method_uri,
-                                                        "requestIdFromRequestCloudEvent", UCode.INVALID_ARGUMENT,
-                                                        u_cloud_event_attributes)
+        u_cloud_event_attributes = (
+            UCloudEventAttributesBuilder()
+            .with_hash("somehash")
+            .with_priority(UPriority.UPRIORITY_CS2)
+            .with_ttl(3)
+            .build()
+        )
+
+        cloud_event = CloudEventFactory.failed_response(
+            application_uri_for_rpc,
+            service_method_uri,
+            "requestIdFromRequestCloudEvent",
+            UCode.INVALID_ARGUMENT,
+            u_cloud_event_attributes,
+        )
 
         # test all attributes
         self.assertEqual("1.0", UCloudEvent.get_specversion(cloud_event))
         self.assertIsNotNone(UCloudEvent.get_id(cloud_event))
-        self.assertEqual(service_method_uri, UCloudEvent.get_source(cloud_event))
+        self.assertEqual(
+            service_method_uri, UCloudEvent.get_source(cloud_event)
+        )
 
         self.assertIn("sink", cloud_event.get_attributes())
-        self.assertEqual(application_uri_for_rpc, UCloudEvent.get_sink(cloud_event))
+        self.assertEqual(
+            application_uri_for_rpc, UCloudEvent.get_sink(cloud_event)
+        )
 
         self.assertEqual("res.v1", UCloudEvent.get_type(cloud_event))
         self.assertEqual("somehash", UCloudEvent.get_hash(cloud_event))
-        self.assertEqual(UPriority.Name(UPriority.UPRIORITY_CS2), UCloudEvent.get_priority(cloud_event))
+        self.assertEqual(
+            UPriority.Name(UPriority.UPRIORITY_CS2),
+            UCloudEvent.get_priority(cloud_event),
+        )
         self.assertEqual(3, UCloudEvent.get_ttl(cloud_event))
-        self.assertEqual(UCode.INVALID_ARGUMENT, UCloudEvent.get_communication_status(cloud_event))
-
-        self.assertEqual("requestIdFromRequestCloudEvent", UCloudEvent.get_request_id(cloud_event))
-
-    def test_create_failed_response_cloud_event_originating_from_remote_use(self):
+        self.assertEqual(
+            UCode.INVALID_ARGUMENT,
+            UCloudEvent.get_communication_status(cloud_event),
+        )
+
+        self.assertEqual(
+            "requestIdFromRequestCloudEvent",
+            UCloudEvent.get_request_id(cloud_event),
+        )
+
+    def test_create_failed_response_cloud_event_originating_from_remote_use(
+        self,
+    ):
         # UriPart for the application requesting the RPC
         application_uri_for_rpc = build_uri_for_test()
 
         # service Method UriPart
         service_method_uri = build_uri_for_test()
 
         # additional attributes
 
-        u_cloud_event_attributes = UCloudEventAttributesBuilder().with_hash("somehash").with_priority(
-            UPriority.UPRIORITY_CS2).with_ttl(3).build()
-
-        cloud_event = CloudEventFactory.failed_response(application_uri_for_rpc, service_method_uri,
-                                                        "requestIdFromRequestCloudEvent", UCode.INVALID_ARGUMENT,
-                                                        u_cloud_event_attributes)
+        u_cloud_event_attributes = (
+            UCloudEventAttributesBuilder()
+            .with_hash("somehash")
+            .with_priority(UPriority.UPRIORITY_CS2)
+            .with_ttl(3)
+            .build()
+        )
+
+        cloud_event = CloudEventFactory.failed_response(
+            application_uri_for_rpc,
+            service_method_uri,
+            "requestIdFromRequestCloudEvent",
+            UCode.INVALID_ARGUMENT,
+            u_cloud_event_attributes,
+        )
 
         # test all attributes
         self.assertEqual("1.0", UCloudEvent.get_specversion(cloud_event))
         self.assertIsNotNone(UCloudEvent.get_id(cloud_event))
-        self.assertEqual(service_method_uri, UCloudEvent.get_source(cloud_event))
+        self.assertEqual(
+            service_method_uri, UCloudEvent.get_source(cloud_event)
+        )
 
         self.assertIn("sink", cloud_event.get_attributes())
-        self.assertEqual(application_uri_for_rpc, UCloudEvent.get_sink(cloud_event))
+        self.assertEqual(
+            application_uri_for_rpc, UCloudEvent.get_sink(cloud_event)
+        )
 
         self.assertEqual("res.v1", UCloudEvent.get_type(cloud_event))
         self.assertEqual("somehash", UCloudEvent.get_hash(cloud_event))
-        self.assertEqual(UPriority.Name(UPriority.UPRIORITY_CS2), UCloudEvent.get_priority(cloud_event))
+        self.assertEqual(
+            UPriority.Name(UPriority.UPRIORITY_CS2),
+            UCloudEvent.get_priority(cloud_event),
+        )
         self.assertEqual(3, UCloudEvent.get_ttl(cloud_event))
-        self.assertEqual(UCode.INVALID_ARGUMENT, UCloudEvent.get_communication_status(cloud_event))
-
-        self.assertEqual("requestIdFromRequestCloudEvent", UCloudEvent.get_request_id(cloud_event))
+        self.assertEqual(
+            UCode.INVALID_ARGUMENT,
+            UCloudEvent.get_communication_status(cloud_event),
+        )
+
+        self.assertEqual(
+            "requestIdFromRequestCloudEvent",
+            UCloudEvent.get_request_id(cloud_event),
+        )
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `up_python-0.1.1.dev0/tests/test_cloudevent/test_serialize/cloudevent_to_protobuf.json` & `up_python-0.1.2.dev0/tests/test_cloudevent/test_serialize/cloudevent_to_protobuf.json`

 * *Files identical despite different names*

### Comparing `up_python-0.1.1.dev0/tests/test_cloudevent/test_serialize/test_base64protobufserializer.py` & `up_python-0.1.2.dev0/tests/test_cloudevent/test_serialize/test_base64protobufserializer.py`

 * *Files 14% similar despite different names*

```diff
@@ -23,55 +23,77 @@
 # SPDX-License-Identifier: Apache-2.0
 
 # -------------------------------------------------------------------------
 
 
 import unittest
 
-from uprotocol.cloudevent.datamodel.ucloudeventattributes import UCloudEventAttributesBuilder
+from uprotocol.cloudevent.datamodel.ucloudeventattributes import (
+    UCloudEventAttributesBuilder,
+)
 from uprotocol.cloudevent.factory.cloudeventfactory import CloudEventFactory
-from uprotocol.cloudevent.serialize.base64protobufserializer import Base64ProtobufSerializer
-from uprotocol.cloudevent.serialize.cloudeventserializers import CloudEventSerializers
+from uprotocol.cloudevent.serialize.base64protobufserializer import (
+    Base64ProtobufSerializer,
+)
+from uprotocol.cloudevent.serialize.cloudeventserializers import (
+    CloudEventSerializers,
+)
 
 
 class TestBase64ProtobufSerializer(unittest.TestCase):
 
     def test_deserialize_bytes_to_string(self):
-        ce = CloudEventFactory.build_base_cloud_event("hello", "http://localhost", bytearray(), "",
-                                                      UCloudEventAttributesBuilder().build(), "example.vertx")
+        ce = CloudEventFactory.build_base_cloud_event(
+            "hello",
+            "http://localhost",
+            bytearray(),
+            "",
+            UCloudEventAttributesBuilder().build(),
+            "example.vertx",
+        )
         ce.__delitem__("time")
         bytes_data = CloudEventSerializers.PROTOBUF.serializer().serialize(ce)
         payload = Base64ProtobufSerializer().deserialize(bytes_data)
         self.assertEqual(
             "CgVoZWxsbxIQaHR0cDovL2xvY2FsaG9zdBoDMS4wIg1leGFtcGxlLnZlcnR4",
-            payload)
+            payload,
+        )
 
     def test_deserialize_bytes_to_string_when_bytes_is_null(self):
         payload = Base64ProtobufSerializer().deserialize(None)
         self.assertEqual("", payload)
 
     def test_deserialize_bytes_to_string_when_bytes_is_empty(self):
         payload = Base64ProtobufSerializer().deserialize(bytearray())
         self.assertEqual("", payload)
 
     def test_serialize_string_into_bytes(self):
-        json_str = "eyJzcGVjdmVyc2lvbiI6ICIxLjAiLCAiaWQiOiAiaGVsbG8iLCAic291cmNlIjogImh0dHA6Ly9sb2NhbGhvc3QiLCAidHlwZSI6ICJleGFtcGxlLnZlcnR4IiwgImRhdGFfYmFzZTY0IjogIiJ9"
+        json_str = (
+            "eyJzcGVjdmVyc2lvbiI6ICIxLjAiLCAiaWQiOiAiaGVsbG8iLCAic2"
+            + "91cmNlIjogImh0dHA6Ly9sb2NhbGhvc3QiLCAidHlwZSI6ICJleGFtcGxlLnZlcnR4IiwgImRhdGFfYmFzZTY0IjogIiJ9"
+        )
         bytes_json = Base64ProtobufSerializer().serialize(json_str)
 
-        ce = CloudEventFactory.build_base_cloud_event("hello", "http://localhost", bytearray(), "",
-                                                      UCloudEventAttributesBuilder().build(), "example.vertx")
+        ce = CloudEventFactory.build_base_cloud_event(
+            "hello",
+            "http://localhost",
+            bytearray(),
+            "",
+            UCloudEventAttributesBuilder().build(),
+            "example.vertx",
+        )
         ce.__delitem__("time")
 
         bytes_data = CloudEventSerializers.JSON.serializer().serialize(ce)
         self.assertEqual(bytes_json, bytes_data)
 
     def test_serialize_string_into_bytes_when_string_is_null(self):
         bytes_data = Base64ProtobufSerializer().serialize(None)
         self.assertEqual(bytearray(), bytes_data)
 
     def test_serialize_string_into_bytes_when_string_is_empty(self):
-        bytes_data = Base64ProtobufSerializer().serialize('')
+        bytes_data = Base64ProtobufSerializer().serialize("")
         self.assertEqual(bytearray(), bytes_data)
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `up_python-0.1.1.dev0/tests/test_cloudevent/test_serialize/test_cloudeventtojsonserializer.py` & `up_python-0.1.2.dev0/tests/test_cloudevent/test_serialize/test_cloudeventtojsonserializer.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,96 +25,131 @@
 # -------------------------------------------------------------------------
 
 
 import unittest
 
 from google.protobuf import any_pb2
 
-from uprotocol.cloudevent.datamodel.ucloudeventattributes import UCloudEventAttributesBuilder
+from uprotocol.cloudevent.datamodel.ucloudeventattributes import (
+    UCloudEventAttributesBuilder,
+)
 from uprotocol.cloudevent.factory.cloudeventfactory import CloudEventFactory
 from uprotocol.cloudevent.factory.ucloudevent import UCloudEvent
-from uprotocol.cloudevent.serialize.cloudeventserializers import CloudEventSerializers
-from uprotocol.cloudevent.serialize.cloudeventtojsonserializer import CloudEventToJsonSerializer
+from uprotocol.cloudevent.serialize.cloudeventserializers import (
+    CloudEventSerializers,
+)
 from uprotocol.cloudevent.cloudevents_pb2 import CloudEvent
 from uprotocol.proto.uattributes_pb2 import UPriority, UMessageType
 
 protoContentType = CloudEventFactory.PROTOBUF_CONTENT_TYPE
 serializer = CloudEventSerializers.JSON.serializer()
 
 
 def build_proto_payload_for_test():
-    ce_proto = CloudEvent(spec_version="1.0", source="https://example.com", id="hello", type="example.demo",
-                          proto_data=any_pb2.Any(),
-                          attributes={"ttl": CloudEvent.CloudEventAttributeValue(ce_string="3")})
+    ce_proto = CloudEvent(
+        spec_version="1.0",
+        source="https://example.com",
+        id="hello",
+        type="example.demo",
+        proto_data=any_pb2.Any(),
+        attributes={"ttl": CloudEvent.CloudEventAttributeValue(ce_string="3")},
+    )
 
     any_obj = any_pb2.Any()
     any_obj.Pack(ce_proto)
     return any_obj
 
 
 class TestCloudEventToJsonSerializer(unittest.TestCase):
 
     def test_serialize_cloud_event_to_json(self):
         proto_payload = build_proto_payload_for_test()
         # additional attributes
-        u_cloud_event_attributes = UCloudEventAttributesBuilder().with_priority(
-            UPriority.UPRIORITY_CS1).with_ttl(3).build()
+        u_cloud_event_attributes = (
+            UCloudEventAttributesBuilder()
+            .with_priority(UPriority.UPRIORITY_CS1)
+            .with_ttl(3)
+            .build()
+        )
 
         # build the cloud event
-        cloud_event = CloudEventFactory.build_base_cloud_event("hello", "/body.access/1/door.front_left",
-                                                               proto_payload.SerializeToString(),
-                                                               proto_payload.type_url, u_cloud_event_attributes,
-                                                               UCloudEvent.get_event_type(
-                                                                   UMessageType.UMESSAGE_TYPE_PUBLISH))
-        cloud_event.__setitem__('datacontenttype', protoContentType)
-        cloud_event.__setitem__('dataschema', proto_payload.type_url)
+        cloud_event = CloudEventFactory.build_base_cloud_event(
+            "hello",
+            "/body.access/1/door.front_left",
+            proto_payload.SerializeToString(),
+            proto_payload.type_url,
+            u_cloud_event_attributes,
+            UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_PUBLISH),
+        )
+        cloud_event.__setitem__("datacontenttype", protoContentType)
+        cloud_event.__setitem__("dataschema", proto_payload.type_url)
         cloud_event.__delitem__("time")
         bytes_data = serializer.serialize(cloud_event)
-        json_str = bytes_data.decode('utf-8')
-        expected = ('{"specversion": "1.0", "id": "hello", "source": "/body.access/1/door.front_left", '
-                    '"type": "pub.v1", "datacontenttype": "application/x-protobuf", "dataschema": '
-                    '"type.googleapis.com/io.cloudevents.v1.CloudEvent", "data_base64": '
-                    '"CjB0eXBlLmdvb2dsZWFwaXMuY29tL2lvLmNsb3VkZXZlbnRzLnYxLkNsb3VkRXZlbnQSPQoFaGVsbG8SE2h0dHBzOi8vZXhhbXBsZS5jb20aAzEuMCIMZXhhbXBsZS5kZW1vKgoKA3R0bBIDGgEzQgA=", "ttl": 3, "priority": "UPRIORITY_CS1"}')
+        json_str = bytes_data.decode("utf-8")
+        expected = (
+            '{"specversion": "1.0", "id": "hello", "source": "/body.access/1/door.front_left", '
+            '"type": "pub.v1", "datacontenttype": "application/x-protobuf", "dataschema": '
+            '"type.googleapis.com/io.cloudevents.v1.CloudEvent", "data_base64": '
+            '"CjB0eXBlLmdvb2dsZWFwaXMuY29tL2lvLmNsb3VkZXZlbnRzLnYxLkNsb3VkRXZlbnQSPQoFaGVs'
+            'bG8SE2h0dHBzOi8vZXhhbXBsZS5jb20aAzEuMCIMZXhhbXBsZS5kZW1vKgoKA3R0bBIDGgEzQgA=", '
+            '"ttl": 3, "priority": "UPRIORITY_CS1"}'
+        )
         self.assertEqual(expected, json_str)
 
     def test_serialize_and_deserialize_cloud_event_to_json(self):
         proto_payload = build_proto_payload_for_test()
         # additional attributes
-        u_cloud_event_attributes = UCloudEventAttributesBuilder().with_priority(
-            UPriority.UPRIORITY_CS1).with_ttl(3).build()
+        u_cloud_event_attributes = (
+            UCloudEventAttributesBuilder()
+            .with_priority(UPriority.UPRIORITY_CS1)
+            .with_ttl(3)
+            .build()
+        )
 
         # build the cloud event
-        cloud_event = CloudEventFactory.build_base_cloud_event("hello", "/body.access/1/door.front_left",
-                                                               proto_payload.SerializeToString(),
-                                                               proto_payload.type_url, u_cloud_event_attributes,
-                                                               UCloudEvent.get_event_type(
-                                                                   UMessageType.UMESSAGE_TYPE_PUBLISH))
-        cloud_event.__setitem__('datacontenttype', protoContentType)
-        cloud_event.__setitem__('dataschema', proto_payload.type_url)
+        cloud_event = CloudEventFactory.build_base_cloud_event(
+            "hello",
+            "/body.access/1/door.front_left",
+            proto_payload.SerializeToString(),
+            proto_payload.type_url,
+            u_cloud_event_attributes,
+            UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_PUBLISH),
+        )
+        cloud_event.__setitem__("datacontenttype", protoContentType)
+        cloud_event.__setitem__("dataschema", proto_payload.type_url)
         cloud_event.__delitem__("time")
         serialized_data = serializer.serialize(cloud_event)
         deserialized_data = serializer.deserialize(serialized_data)
         deserialized_data.__delitem__("time")
 
         self.assertEqual(cloud_event, deserialized_data)
 
-    def test_double_serialization_protobuf_when_creating_cloud_event_with_factory_methods(self):
+    def test_double_serialization_protobuf_when_creating_cloud_event_with_factory_methods(
+        self,
+    ):
         proto_payload = build_proto_payload_for_test()
         # additional attributes
-        u_cloud_event_attributes = UCloudEventAttributesBuilder().with_priority(
-            UPriority.UPRIORITY_CS1).with_ttl(3).build()
+        u_cloud_event_attributes = (
+            UCloudEventAttributesBuilder()
+            .with_priority(UPriority.UPRIORITY_CS1)
+            .with_ttl(3)
+            .build()
+        )
 
         # build the cloud event
-        cloud_event1 = CloudEventFactory.build_base_cloud_event("hello", "/body.access/1/door.front_left",
-                                                                proto_payload.SerializeToString(),
-                                                                proto_payload.type_url, u_cloud_event_attributes,
-                                                                UCloudEvent.get_event_type(
-                                                                    UMessageType.UMESSAGE_TYPE_PUBLISH))
-        cloud_event1.__setitem__('datacontenttype', protoContentType)
-        cloud_event1.__setitem__('dataschema', proto_payload.type_url)
+        cloud_event1 = CloudEventFactory.build_base_cloud_event(
+            "hello",
+            "/body.access/1/door.front_left",
+            proto_payload.SerializeToString(),
+            proto_payload.type_url,
+            u_cloud_event_attributes,
+            UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_PUBLISH),
+        )
+        cloud_event1.__setitem__("datacontenttype", protoContentType)
+        cloud_event1.__setitem__("dataschema", proto_payload.type_url)
         cloud_event1.__delitem__("time")
         serialized_data1 = serializer.serialize(cloud_event1)
         cloud_event2 = serializer.deserialize(serialized_data1)
         cloud_event2.__delitem__("time")
         self.assertEqual(cloud_event2, cloud_event1)
         serialized_data2 = serializer.serialize(cloud_event2)
         self.assertEqual(serialized_data1, serialized_data2)
```

### Comparing `up_python-0.1.1.dev0/tests/test_cloudevent/test_serialize/test_cloudeventtoprotobufserializer.py` & `up_python-0.1.2.dev0/tests/test_cloudevent/test_serialize/test_cloudeventtoprotobufserializer.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,132 +26,208 @@
 import json
 import os
 import unittest
 
 from cloudevents.http import CloudEvent as ApacheCloudEvent
 from google.protobuf import any_pb2
 
-from uprotocol.cloudevent.datamodel.ucloudeventattributes import UCloudEventAttributesBuilder
+from uprotocol.cloudevent.datamodel.ucloudeventattributes import (
+    UCloudEventAttributesBuilder,
+)
 from uprotocol.cloudevent.factory.cloudeventfactory import CloudEventFactory
 from uprotocol.cloudevent.factory.ucloudevent import UCloudEvent
-from uprotocol.cloudevent.serialize.base64protobufserializer import Base64ProtobufSerializer
-from uprotocol.cloudevent.serialize.cloudeventserializers import CloudEventSerializers
-from uprotocol.cloudevent.serialize.cloudeventtoprotobufserializer import CloudEventToProtobufSerializer
+from uprotocol.cloudevent.serialize.base64protobufserializer import (
+    Base64ProtobufSerializer,
+)
+from uprotocol.cloudevent.serialize.cloudeventserializers import (
+    CloudEventSerializers,
+)
+from uprotocol.cloudevent.serialize.cloudeventtoprotobufserializer import (
+    CloudEventToProtobufSerializer,
+)
 from uprotocol.cloudevent.cloudevents_pb2 import CloudEvent
 from uprotocol.proto.uattributes_pb2 import UPriority, UMessageType
 from uprotocol.proto.uri_pb2 import UUri, UEntity, UResource
 from uprotocol.uri.serializer.longuriserializer import LongUriSerializer
 
 serializer = CloudEventSerializers.PROTOBUF.serializer()
 
 
 def build_uuri_for_test():
-    uri = UUri(entity=UEntity(name="body.access"),
-               resource=UResource(name="door", instance="front_left", message="Door"))
+    uri = UUri(
+        entity=UEntity(name="body.access"),
+        resource=UResource(name="door", instance="front_left", message="Door"),
+    )
     return LongUriSerializer().serialize(uri)
 
 
 def build_proto_payload_for_test():
-    ce_proto = CloudEvent(spec_version="1.0", source="https://example.com", id="hello", type="example.demo",
-                          proto_data=any_pb2.Any(),
-                          attributes={"ttl": CloudEvent.CloudEventAttributeValue(ce_string="3")})
+    ce_proto = CloudEvent(
+        spec_version="1.0",
+        source="https://example.com",
+        id="hello",
+        type="example.demo",
+        proto_data=any_pb2.Any(),
+        attributes={"ttl": CloudEvent.CloudEventAttributeValue(ce_string="3")},
+    )
 
     any_obj = any_pb2.Any()
     any_obj.Pack(ce_proto)
     return any_obj
 
 
 def get_json_object():
     current_directory = os.getcwd()
-    json_file_path = os.path.join(current_directory, "tests","test_cloudevent",
-    "test_serialize","cloudevent_to_protobuf.json")
-    with open(json_file_path, 'r') as json_file:
+    json_file_path = os.path.join(
+        current_directory,
+        "tests",
+        "test_cloudevent",
+        "test_serialize",
+        "cloudevent_to_protobuf.json",
+    )
+    with open(json_file_path, "r") as json_file:
         json_data = json.load(json_file)
 
     return json_data
 
 
 class TestCloudEventToProtobufSerializer(unittest.TestCase):
 
     def test_all_cloud_events_from_json(self):
         cloudevents = get_json_object()
         for ce_json in cloudevents:
-            bytes_ce = Base64ProtobufSerializer().serialize(ce_json['serialized_ce'])
+            bytes_ce = Base64ProtobufSerializer().serialize(
+                ce_json["serialized_ce"]
+            )
             cloudevent = CloudEventToProtobufSerializer().deserialize(bytes_ce)
-            self.assertEqual(UCloudEvent.get_id(cloudevent), ce_json['id'])
-            self.assertEqual(UCloudEvent.get_specversion(cloudevent), ce_json['specversion'])
-            if 'source' in ce_json:
-                self.assertEqual(UCloudEvent.get_source(cloudevent), ce_json['source'])
-            if 'sink' in ce_json:
-                self.assertEqual(UCloudEvent.get_sink(cloudevent), ce_json['sink'])
-            if 'type' in ce_json:
-                self.assertEqual(UCloudEvent.get_type(cloudevent), ce_json['type'])
-            if 'priority' in ce_json:
-                self.assertEqual(UCloudEvent.get_priority(cloudevent), ce_json['priority'])
-            if 'ttl' in ce_json:
-                self.assertEqual(UCloudEvent.get_ttl(cloudevent), ce_json['ttl'])
-            if 'hash' in ce_json:
-                self.assertEqual(UCloudEvent.get_hash(cloudevent), ce_json['hash'])
-            if 'token' in ce_json:
-                self.assertEqual(UCloudEvent.get_token(cloudevent), ce_json['token'])
-            if 'dataschema' in ce_json:
-                self.assertEqual(UCloudEvent.get_data_schema(cloudevent), ce_json['dataschema'])
-            if 'datacontenttype' in ce_json:
-                self.assertEqual(UCloudEvent.get_data_content_type(cloudevent), ce_json['datacontenttype'])
-            if 'commstatus' in ce_json:
-                self.assertEqual(UCloudEvent.get_communication_status(cloudevent), ce_json['commstatus'])
+            self.assertEqual(UCloudEvent.get_id(cloudevent), ce_json["id"])
+            self.assertEqual(
+                UCloudEvent.get_specversion(cloudevent), ce_json["specversion"]
+            )
+            if "source" in ce_json:
+                self.assertEqual(
+                    UCloudEvent.get_source(cloudevent), ce_json["source"]
+                )
+            if "sink" in ce_json:
+                self.assertEqual(
+                    UCloudEvent.get_sink(cloudevent), ce_json["sink"]
+                )
+            if "type" in ce_json:
+                self.assertEqual(
+                    UCloudEvent.get_type(cloudevent), ce_json["type"]
+                )
+            if "priority" in ce_json:
+                self.assertEqual(
+                    UCloudEvent.get_priority(cloudevent), ce_json["priority"]
+                )
+            if "ttl" in ce_json:
+                self.assertEqual(
+                    UCloudEvent.get_ttl(cloudevent), ce_json["ttl"]
+                )
+            if "hash" in ce_json:
+                self.assertEqual(
+                    UCloudEvent.get_hash(cloudevent), ce_json["hash"]
+                )
+            if "token" in ce_json:
+                self.assertEqual(
+                    UCloudEvent.get_token(cloudevent), ce_json["token"]
+                )
+            if "dataschema" in ce_json:
+                self.assertEqual(
+                    UCloudEvent.get_data_schema(cloudevent),
+                    ce_json["dataschema"],
+                )
+            if "datacontenttype" in ce_json:
+                self.assertEqual(
+                    UCloudEvent.get_data_content_type(cloudevent),
+                    ce_json["datacontenttype"],
+                )
+            if "commstatus" in ce_json:
+                self.assertEqual(
+                    UCloudEvent.get_communication_status(cloudevent),
+                    ce_json["commstatus"],
+                )
 
     def test_serialize_and_deserialize_cloud_event_to_protobuf(self):
-        source = build_uuri_for_test()
         proto_payload = build_proto_payload_for_test()
         # additional attributes
-        u_cloud_event_attributes = UCloudEventAttributesBuilder().with_hash("somehash").with_priority(
-            UPriority.UPRIORITY_CS0).with_ttl(3).build()
+        u_cloud_event_attributes = (
+            UCloudEventAttributesBuilder()
+            .with_hash("somehash")
+            .with_priority(UPriority.UPRIORITY_CS0)
+            .with_ttl(3)
+            .build()
+        )
 
         # build the cloud event
-        cloud_event = CloudEventFactory.build_base_cloud_event("hello", "/body.access/1/door.front_left",
-                                                               proto_payload.SerializeToString(),
-                                                               proto_payload.type_url, u_cloud_event_attributes,
-                                                               UCloudEvent.get_event_type(
-                                                                   UMessageType.UMESSAGE_TYPE_PUBLISH))
+        cloud_event = CloudEventFactory.build_base_cloud_event(
+            "hello",
+            "/body.access/1/door.front_left",
+            proto_payload.SerializeToString(),
+            proto_payload.type_url,
+            u_cloud_event_attributes,
+            UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_PUBLISH),
+        )
 
         cloud_event.__delitem__("time")
         serialized_data = serializer.serialize(cloud_event)
 
         deserialized_data = serializer.deserialize(serialized_data)
         deserialized_data.__delitem__("time")
         self.assertEqual(cloud_event, deserialized_data)
 
     def test_serialize_two_different_cloud_event_are_not_the_same(self):
         proto_payload = build_proto_payload_for_test()
-        json_attributes1 = {"id": "hello", "source": "/body.access/1/door.front_left", "type": "pub.v1"}
-        cloud_event1 = ApacheCloudEvent(json_attributes1, proto_payload.SerializeToString())
-        cloud_event1.__setitem__('datacontenttype', 'application/protobuf')
-        cloud_event1.__setitem__('dataschema', proto_payload.type_url)
+        json_attributes1 = {
+            "id": "hello",
+            "source": "/body.access/1/door.front_left",
+            "type": "pub.v1",
+        }
+        cloud_event1 = ApacheCloudEvent(
+            json_attributes1, proto_payload.SerializeToString()
+        )
+        cloud_event1.__setitem__("datacontenttype", "application/protobuf")
+        cloud_event1.__setitem__("dataschema", proto_payload.type_url)
         cloud_event1.__delitem__("time")
 
-        json_attributes2 = {"source": "/body.access/1/door.front_left", "type": "file.v1"}
-        cloud_event2 = ApacheCloudEvent(json_attributes2, proto_payload.SerializeToString())
+        json_attributes2 = {
+            "source": "/body.access/1/door.front_left",
+            "type": "file.v1",
+        }
+        cloud_event2 = ApacheCloudEvent(
+            json_attributes2, proto_payload.SerializeToString()
+        )
         cloud_event2.__delitem__("time")
         serialized1 = serializer.serialize(cloud_event1)
         serialized2 = serializer.serialize(cloud_event2)
         self.assertNotEqual(serialized1, serialized2)
 
-    def test_double_serialization_protobuf_when_creating_cloud_event_with_factory_methods(self):
+    def test_double_serialization_protobuf_when_creating_cloud_event_with_factory_methods(
+        self,
+    ):
         proto_payload = build_proto_payload_for_test()
         source = build_uuri_for_test()
         # additional attributes
-        u_cloud_event_attributes = UCloudEventAttributesBuilder().with_hash("somehash").with_priority(
-            UPriority.UPRIORITY_CS1).with_ttl(3).with_token("someOAuthToken").build()
+        u_cloud_event_attributes = (
+            UCloudEventAttributesBuilder()
+            .with_hash("somehash")
+            .with_priority(UPriority.UPRIORITY_CS1)
+            .with_ttl(3)
+            .with_token("someOAuthToken")
+            .build()
+        )
 
         # build the cloud event
-        cloud_event = CloudEventFactory.build_base_cloud_event("testme", source, proto_payload.SerializeToString(),
-                                                               proto_payload.type_url, u_cloud_event_attributes,
-                                                               UCloudEvent.get_event_type(
-                                                                   UMessageType.UMESSAGE_TYPE_PUBLISH))
+        cloud_event = CloudEventFactory.build_base_cloud_event(
+            "testme",
+            source,
+            proto_payload.SerializeToString(),
+            proto_payload.type_url,
+            u_cloud_event_attributes,
+            UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_PUBLISH),
+        )
         cloud_event.__delitem__("time")
 
         serialized_data = serializer.serialize(cloud_event)
         deserialized_data = serializer.deserialize(serialized_data)
         deserialized_data.__delitem__("time")
         self.assertEqual(cloud_event, deserialized_data)
-
```

### Comparing `up_python-0.1.1.dev0/tests/test_cloudevent/test_validator/test_cloudeventvalidator.py` & `up_python-0.1.2.dev0/tests/test_cloudevent/test_validator/test_cloudeventvalidator.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,450 +21,623 @@
 # SPDX-FileType: SOURCE
 # SPDX-FileCopyrightText: 2023 General Motors GTO LLC
 # SPDX-License-Identifier: Apache-2.0
 
 # -------------------------------------------------------------------------
 
 
-
 import unittest
 
 from google.protobuf import any_pb2
 
-from uprotocol.cloudevent.datamodel.ucloudeventattributes import UCloudEventAttributesBuilder
+from uprotocol.cloudevent.datamodel.ucloudeventattributes import (
+    UCloudEventAttributesBuilder,
+)
 from uprotocol.cloudevent.factory.cloudeventfactory import CloudEventFactory
 from uprotocol.cloudevent.factory.ucloudevent import UCloudEvent
-from uprotocol.cloudevent.validate.cloudeventvalidator import CloudEventValidator, Validators
+from uprotocol.cloudevent.validate.cloudeventvalidator import (
+    CloudEventValidator,
+    Validators,
+)
 from uprotocol.cloudevent.cloudevents_pb2 import CloudEvent
 from uprotocol.proto.uattributes_pb2 import UPriority, UMessageType
 from uprotocol.proto.uri_pb2 import UUri, UEntity, UResource
 from uprotocol.proto.ustatus_pb2 import UCode
 from uprotocol.uri.serializer.longuriserializer import LongUriSerializer
 from uprotocol.uuid.factory.uuidfactory import Factories
 from uprotocol.uuid.serializer.longuuidserializer import LongUuidSerializer
 from uprotocol.validation.validationresult import ValidationResult
 
 
-def build_base_cloud_event_for_test():
+def build_base_publish_cloud_event_for_test():
     # uri
     source = build_long_uri_for_test()
 
     # fake payload
     proto_payload = build_proto_payload_for_test()
     # additional attributes
-    u_cloud_event_attributes = UCloudEventAttributesBuilder().with_hash("somehash").with_priority(
-        UPriority.UPRIORITY_CS1).with_ttl(3).with_token("someOAuthToken").build()
+    u_cloud_event_attributes = (
+        UCloudEventAttributesBuilder()
+        .with_hash("somehash")
+        .with_priority(UPriority.UPRIORITY_CS1)
+        .with_ttl(3)
+        .with_token("someOAuthToken")
+        .build()
+    )
     # build the cloud event
-    cloud_event = CloudEventFactory.build_base_cloud_event("testme", source, proto_payload.SerializeToString(),
-                                                           proto_payload.type_url, u_cloud_event_attributes,
-                                                           UCloudEvent.get_event_type(
-                                                               UMessageType.UMESSAGE_TYPE_PUBLISH))
+    cloud_event = CloudEventFactory.build_base_cloud_event(
+        "testme",
+        source,
+        proto_payload.SerializeToString(),
+        proto_payload.type_url,
+        u_cloud_event_attributes,
+        UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_PUBLISH),
+    )
+    return cloud_event
+
+    pass
+
+
+def build_base_notification_cloud_event_for_test():
+    # uri
+    source = build_long_uri_for_test()
+
+    # fake payload
+    proto_payload = build_proto_payload_for_test()
+    # additional attributes
+    u_cloud_event_attributes = (
+        UCloudEventAttributesBuilder()
+        .with_hash("somehash")
+        .with_priority(UPriority.UPRIORITY_CS1)
+        .with_ttl(3)
+        .with_token("someOAuthToken")
+        .build()
+    )
+    # build the cloud event
+    cloud_event = CloudEventFactory.build_base_cloud_event(
+        "testme",
+        source,
+        proto_payload.SerializeToString(),
+        proto_payload.type_url,
+        u_cloud_event_attributes,
+        UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_NOTIFICATION),
+    )
     return cloud_event
 
     pass
 
 
 def build_proto_payload_for_test():
-    ce_proto = CloudEvent(spec_version="1.0", source="https://example.com", id="hello", type="example.demo",
-                          proto_data=any_pb2.Any())
+    ce_proto = CloudEvent(
+        spec_version="1.0",
+        source="https://example.com",
+        id="hello",
+        type="example.demo",
+        proto_data=any_pb2.Any(),
+    )
 
     any_obj = any_pb2.Any()
     any_obj.Pack(ce_proto)
     return any_obj
 
 
 def build_uuri_for_test():
-    return UUri(entity=UEntity(name="body.access"),
-                resource=UResource(name="door", instance="front_left", message="Door"))
+    return UUri(
+        entity=UEntity(name="body.access"),
+        resource=UResource(name="door", instance="front_left", message="Door"),
+    )
 
 
 def build_long_uri_for_test():
     return LongUriSerializer().serialize(build_uuri_for_test())
 
 
 class TestCloudEventValidator(unittest.TestCase):
 
     def test_get_a_publish_cloud_event_validator(self):
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         validator = CloudEventValidator.get_validator(cloud_event)
         status = validator.validate_type(cloud_event).to_status()
         self.assertEqual(status, ValidationResult.STATUS_SUCCESS)
         self.assertEqual("CloudEventValidator.Publish", str(validator))
 
     def test_get_a_notification_cloud_event_validator(self):
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_notification_cloud_event_for_test()
         cloud_event.__setitem__("sink", "//bo.cloud/petapp")
         validator = Validators.NOTIFICATION.validator()
         status = validator.validate_type(cloud_event).to_status()
         self.assertEqual(status, ValidationResult.STATUS_SUCCESS)
         self.assertEqual("CloudEventValidator.Notification", str(validator))
 
     def test_publish_cloud_event_type(self):
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("type", "res.v1")
         validator = Validators.PUBLISH.validator()
         status = validator.validate_type(cloud_event).to_status()
         self.assertEqual(UCode.INVALID_ARGUMENT, status.code)
-        self.assertEqual("Invalid CloudEvent type [res.v1]. CloudEvent of type Publish must have a type of 'pub.v1'",
-                          status.message)
+        self.assertEqual(
+            "Invalid CloudEvent type [res.v1]. CloudEvent of type Publish must have a type of 'pub.v1'",
+            status.message,
+        )
 
     def test_notification_cloud_event_type(self):
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("type", "res.v1")
         validator = Validators.NOTIFICATION.validator()
         status = validator.validate_type(cloud_event).to_status()
         self.assertEqual(UCode.INVALID_ARGUMENT, status.code)
-        self.assertEqual("Invalid CloudEvent type [res.v1]. CloudEvent of type Publish must have a type of 'pub.v1'",
-                          status.message)
+        self.assertEqual(
+            "Invalid CloudEvent type [res.v1]. CloudEvent of type Notification must have a type of 'not.v1'",
+            status.message,
+        )
 
     def test_get_a_request_cloud_event_validator(self):
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("type", "req.v1")
         validator = CloudEventValidator.get_validator(cloud_event)
         status = validator.validate_type(cloud_event).to_status()
         self.assertEqual(status, ValidationResult.STATUS_SUCCESS)
         self.assertEqual("CloudEventValidator.Request", str(validator))
 
     def test_request_cloud_event_type(self):
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("type", "pub.v1")
         validator = Validators.REQUEST.validator()
         status = validator.validate_type(cloud_event).to_status()
         self.assertEqual(UCode.INVALID_ARGUMENT, status.code)
-        self.assertEqual("Invalid CloudEvent type [pub.v1]. CloudEvent of type Request must have a type of 'req.v1'",
-                          status.message)
+        self.assertEqual(
+            "Invalid CloudEvent type [pub.v1]. CloudEvent of type Request must have a type of 'req.v1'",
+            status.message,
+        )
 
     def test_get_a_response_cloud_event_validator(self):
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("type", "res.v1")
         validator = CloudEventValidator.get_validator(cloud_event)
         status = validator.validate_type(cloud_event).to_status()
         self.assertEqual(status, ValidationResult.STATUS_SUCCESS)
         self.assertEqual("CloudEventValidator.Response", str(validator))
 
     def test_response_cloud_event_type(self):
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("type", "pub.v1")
         validator = Validators.RESPONSE.validator()
         status = validator.validate_type(cloud_event).to_status()
         self.assertEqual(UCode.INVALID_ARGUMENT, status.code)
-        self.assertEqual("Invalid CloudEvent type [pub.v1]. CloudEvent of type Response must have a type of 'res.v1'",
-                          status.message)
-
-    def test_get_a_publish_cloud_event_validator_when_cloud_event_type_is_unknown(self):
-        cloud_event = build_base_cloud_event_for_test()
+        self.assertEqual(
+            "Invalid CloudEvent type [pub.v1]. CloudEvent of type Response must have a type of 'res.v1'",
+            status.message,
+        )
+
+    def test_get_a_publish_cloud_event_validator_when_cloud_event_type_is_unknown(
+        self,
+    ):
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("type", "lala.v1")
         validator = CloudEventValidator.get_validator(cloud_event)
-        status = validator.validate_type(cloud_event).to_status()
         self.assertEqual("CloudEventValidator.Publish", str(validator))
 
     def test_validate_cloud_event_version_when_valid(self):
         uuid = Factories.UPROTOCOL.create()
         str_uuid = LongUuidSerializer.instance().serialize(uuid)
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("type", "pub.v1")
         cloud_event.__setitem__("id", str_uuid)
         status = CloudEventValidator.validate_version(cloud_event).to_status()
         self.assertEqual(status, ValidationResult.STATUS_SUCCESS)
 
     def test_validate_cloud_event_version_when_not_valid(self):
         uuid = Factories.UPROTOCOL.create()
         str_uuid = LongUuidSerializer.instance().serialize(uuid)
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("specversion", "0.3")
         cloud_event.__setitem__("id", str_uuid)
         status = CloudEventValidator.validate_version(cloud_event).to_status()
         self.assertEqual(UCode.INVALID_ARGUMENT, status.code)
-        self.assertEqual("Invalid CloudEvent version [0.3]. CloudEvent version must be 1.0.", status.message)
+        self.assertEqual(
+            "Invalid CloudEvent version [0.3]. CloudEvent version must be 1.0.",
+            status.message,
+        )
 
     def test_validate_cloud_event_id_when_valid(self):
         uuid = Factories.UPROTOCOL.create()
         str_uuid = LongUuidSerializer.instance().serialize(uuid)
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("id", str_uuid)
         cloud_event.__setitem__("type", "pub.v1")
         status = CloudEventValidator.validate_version(cloud_event).to_status()
         self.assertEqual(status, ValidationResult.STATUS_SUCCESS)
 
     def test_validate_cloud_event_id_when_not_uuidv8_type_id(self):
         str_uuid = "1dd9200c-d41b-4658-8102-3101f0b91378"
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("id", str_uuid)
         cloud_event.__setitem__("type", "pub.v1")
         status = CloudEventValidator.validate_id(cloud_event).to_status()
         self.assertEqual(UCode.INVALID_ARGUMENT, status.code)
-        self.assertEqual("Invalid CloudEvent Id [" + str_uuid + "]. CloudEvent Id must be of type UUIDv8.",
-                          status.message)
+        self.assertEqual(
+            "Invalid CloudEvent Id ["
+            + str_uuid
+            + "]. CloudEvent Id must be of type UUIDv8.",
+            status.message,
+        )
 
     def test_validate_cloud_event_id_when_not_valid(self):
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("id", "testme")
         cloud_event.__setitem__("type", "pub.v1")
         status = CloudEventValidator.validate_id(cloud_event).to_status()
         self.assertEqual(UCode.INVALID_ARGUMENT, status.code)
-        self.assertEqual("Invalid CloudEvent Id [testme]. CloudEvent Id must be of type UUIDv8.", status.message)
+        self.assertEqual(
+            "Invalid CloudEvent Id [testme]. CloudEvent Id must be of type UUIDv8.",
+            status.message,
+        )
 
-    def test_publish_type_cloudevent_is_valid_when_everything_is_valid_local(self):
+    def test_publish_type_cloudevent_is_valid_when_everything_is_valid_local(
+        self,
+    ):
         uuid = Factories.UPROTOCOL.create()
         str_uuid = LongUuidSerializer.instance().serialize(uuid)
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("id", str_uuid)
         cloud_event.__setitem__("type", "pub.v1")
-        cloud_event.__setitem__("source", "/body.access/1/door.front_left#Door")
+        cloud_event.__setitem__(
+            "source", "/body.access/1/door.front_left#Door"
+        )
         validator = Validators.PUBLISH.validator()
         result = validator.validate(cloud_event)
         self.assertEqual(ValidationResult.success(), result)
 
-    def test_publish_type_cloudevent_is_valid_when_everything_is_valid_remote(self):
+    def test_publish_type_cloudevent_is_valid_when_everything_is_valid_remote(
+        self,
+    ):
         uuid = Factories.UPROTOCOL.create()
         str_uuid = LongUuidSerializer.instance().serialize(uuid)
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("id", str_uuid)
         cloud_event.__setitem__("type", "pub.v1")
-        cloud_event.__setitem__("source", "//VCU.myvin/body.access/1/door.front_left#Door")
+        cloud_event.__setitem__(
+            "source", "//VCU.myvin/body.access/1/door.front_left#Door"
+        )
         validator = Validators.PUBLISH.validator()
         result = validator.validate(cloud_event)
         self.assertEqual(ValidationResult.success(), result)
 
-    def test_publish_type_cloudevent_is_valid_when_everything_is_valid_remote_with_a_sink(self):
+    def test_publish_type_cloudevent_is_valid_when_everything_is_valid_remote_with_a_sink(
+        self,
+    ):
         uuid = Factories.UPROTOCOL.create()
         str_uuid = LongUuidSerializer.instance().serialize(uuid)
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("id", str_uuid)
         cloud_event.__setitem__("type", "pub.v1")
-        cloud_event.__setitem__("source", "//VCU.myvin/body.access/1/door.front_left#Door")
+        cloud_event.__setitem__(
+            "source", "//VCU.myvin/body.access/1/door.front_left#Door"
+        )
         cloud_event.__setitem__("sink", "//bo.cloud/petapp")
         validator = Validators.PUBLISH.validator()
         result = validator.validate(cloud_event)
         self.assertEqual(ValidationResult.success(), result)
 
-    def test_publish_type_cloudevent_is_not_valid_when_remote_with_invalid_sink(self):
+    def test_publish_type_cloudevent_is_not_valid_when_remote_with_invalid_sink(
+        self,
+    ):
         uuid = Factories.UPROTOCOL.create()
         str_uuid = LongUuidSerializer.instance().serialize(uuid)
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("id", str_uuid)
         cloud_event.__setitem__("type", "pub.v1")
-        cloud_event.__setitem__("source", "//VCU.myvin/body.access/1/door.front_left#Door")
+        cloud_event.__setitem__(
+            "source", "//VCU.myvin/body.access/1/door.front_left#Door"
+        )
         cloud_event.__setitem__("sink", "//bo.cloud")
         validator = Validators.PUBLISH.validator()
         result = validator.validate(cloud_event)
-        self.assertEqual("Invalid CloudEvent sink [//bo.cloud]. Uri is missing uSoftware Entity name.",
-                          result.get_message())
+        self.assertEqual(
+            "Invalid CloudEvent sink [//bo.cloud]. Uri is missing uSoftware Entity name.",
+            result.get_message(),
+        )
 
     def test_publish_type_cloudevent_is_not_valid_when_source_is_empty(self):
         uuid = Factories.UPROTOCOL.create()
         str_uuid = LongUuidSerializer.instance().serialize(uuid)
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("id", str_uuid)
         cloud_event.__setitem__("source", "/")
         validator = Validators.PUBLISH.validator()
         result = validator.validate(cloud_event)
-        self.assertEqual("Invalid Publish type CloudEvent source [/]. Uri is empty.", result.get_message())
+        self.assertEqual(
+            "Invalid Publish type CloudEvent source [/]. Uri is empty.",
+            result.get_message(),
+        )
 
-    def test_publish_type_cloudevent_is_not_valid_when_source_is_missing_authority(self):
-        cloud_event = build_base_cloud_event_for_test()
+    def test_notification_type_cloudevent_is_not_valid_when_source_is_empty(
+        self,
+    ):
+        uuid = Factories.UPROTOCOL.create()
+        str_uuid = LongUuidSerializer.instance().serialize(uuid)
+        cloud_event = build_base_notification_cloud_event_for_test()
+        cloud_event.__setitem__("id", str_uuid)
+        cloud_event.__setitem__("source", "/")
+        validator = Validators.NOTIFICATION.validator()
+        result = validator.validate(cloud_event)
+        self.assertEqual(
+            "Invalid Notification type CloudEvent source [/], Uri is empty.,"
+            + "Invalid CloudEvent sink. Notification CloudEvent sink must be an  uri.",
+            result.get_message(),
+        )
+
+    def test_publish_type_cloudevent_is_not_valid_when_source_is_missing_authority(
+        self,
+    ):
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("id", "testme")
         cloud_event.__setitem__("type", "pub.v1")
         cloud_event.__setitem__("source", "/body.access")
         validator = Validators.PUBLISH.validator()
         result = validator.validate(cloud_event)
         self.assertEqual(
-            "Invalid CloudEvent Id [testme]. CloudEvent Id must be of type UUIDv8.," + "Invalid Publish type " +
-            "CloudEvent source [/body.access]. UriPart is missing uResource name.",
-            result.get_message())
-
-    def test_publish_type_cloudevent_is_not_valid_when_source_is_missing_message_info(self):
-        cloud_event = build_base_cloud_event_for_test()
+            "Invalid CloudEvent Id [testme]. CloudEvent Id must be of type UUIDv8.,"
+            + "Invalid Publish type "
+            + "CloudEvent source [/body.access]. UriPart is missing uResource name.",
+            result.get_message(),
+        )
+
+    def test_publish_type_cloudevent_is_not_valid_when_source_is_missing_message_info(
+        self,
+    ):
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("id", "testme")
         cloud_event.__setitem__("type", "pub.v1")
         cloud_event.__setitem__("source", "/body.access/1/door.front_left")
         validator = Validators.PUBLISH.validator()
         result = validator.validate(cloud_event)
         self.assertEqual(
-            "Invalid CloudEvent Id [testme]. CloudEvent Id must be of type UUIDv8.," + "Invalid Publish type " +
-            "CloudEvent source [/body.access/1/door.front_left]. UriPart is missing Message information.",
-            result.get_message())
-
-    def test_notification_type_cloudevent_is_valid_when_everything_is_valid(self):
-        uuid = Factories.UPROTOCOL.create()
-        str_uuid = LongUuidSerializer.instance().serialize(uuid)
-        cloud_event = build_base_cloud_event_for_test()
-        cloud_event.__setitem__("id", str_uuid)
-        cloud_event.__setitem__("type", "pub.v1")
-        cloud_event.__setitem__("source", "/body.access/1/door.front_left#Door")
+            "Invalid CloudEvent Id [testme]. CloudEvent Id must be of type UUIDv8.,"
+            + "Invalid Publish type "
+            + "CloudEvent source [/body.access/1/door.front_left]. UriPart is missing Message information.",
+            result.get_message(),
+        )
+
+    def test_notification_type_cloudevent_is_valid_when_everything_is_valid(
+        self,
+    ):
+        uuid = Factories.UPROTOCOL.create()
+        str_uuid = LongUuidSerializer.instance().serialize(uuid)
+        cloud_event = build_base_notification_cloud_event_for_test()
+        cloud_event.__setitem__("id", str_uuid)
+        cloud_event.__setitem__("type", "not.v1")
+        cloud_event.__setitem__(
+            "source", "/body.access/1/door.front_left#Door"
+        )
         cloud_event.__setitem__("sink", "//bo.cloud/petapp")
         validator = Validators.NOTIFICATION.validator()
         result = validator.validate(cloud_event)
         self.assertEqual(ValidationResult.success(), result)
 
     def test_notification_type_cloudevent_is_not_valid_missing_sink(self):
         uuid = Factories.UPROTOCOL.create()
         str_uuid = LongUuidSerializer.instance().serialize(uuid)
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_notification_cloud_event_for_test()
         cloud_event.__setitem__("id", str_uuid)
-        cloud_event.__setitem__("type", "pub.v1")
-        cloud_event.__setitem__("source", "/body.access/1/door.front_left#Door")
+        cloud_event.__setitem__("type", "not.v1")
+        cloud_event.__setitem__(
+            "source", "/body.access/1/door.front_left#Door"
+        )
         validator = Validators.NOTIFICATION.validator()
         result = validator.validate(cloud_event)
-        self.assertEqual("Invalid CloudEvent sink. Notification CloudEvent sink must be an  uri.",
-                          result.get_message())
+        self.assertEqual(
+            "Invalid CloudEvent sink. Notification CloudEvent sink must be an  uri.",
+            result.get_message(),
+        )
 
     def test_notification_type_cloudevent_is_not_valid_invalid_sink(self):
         uuid = Factories.UPROTOCOL.create()
         str_uuid = LongUuidSerializer.instance().serialize(uuid)
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_notification_cloud_event_for_test()
         cloud_event.__setitem__("id", str_uuid)
-        cloud_event.__setitem__("type", "pub.v1")
+        cloud_event.__setitem__("type", "not.v1")
         cloud_event.__setitem__("sink", "//bo.cloud")
-        cloud_event.__setitem__("source", "/body.access/1/door.front_left#Door")
+        cloud_event.__setitem__(
+            "source", "/body.access/1/door.front_left#Door"
+        )
         validator = Validators.NOTIFICATION.validator()
         result = validator.validate(cloud_event)
         self.assertEqual(
             "Invalid Notification type CloudEvent sink [//bo.cloud]. Uri is missing uSoftware Entity name.",
-            result.get_message())
+            result.get_message(),
+        )
 
     def test_request_type_cloudevent_is_valid_when_everything_is_valid(self):
         uuid = Factories.UPROTOCOL.create()
         str_uuid = LongUuidSerializer.instance().serialize(uuid)
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("id", str_uuid)
         cloud_event.__setitem__("type", "req.v1")
-        cloud_event.__setitem__("sink", "//VCU.myvin/body.access/1/rpc.UpdateDoor")
+        cloud_event.__setitem__(
+            "sink", "//VCU.myvin/body.access/1/rpc.UpdateDoor"
+        )
         cloud_event.__setitem__("source", "//bo.cloud/petapp//rpc.response")
         validator = Validators.REQUEST.validator()
         result = validator.validate(cloud_event)
         self.assertEqual(ValidationResult.success(), result)
 
     def test_request_type_cloudevent_is_not_valid_invalid_source(self):
         uuid = Factories.UPROTOCOL.create()
         str_uuid = LongUuidSerializer.instance().serialize(uuid)
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("id", str_uuid)
         cloud_event.__setitem__("type", "req.v1")
-        cloud_event.__setitem__("sink", "//VCU.myvin/body.access/1/rpc.UpdateDoor")
+        cloud_event.__setitem__(
+            "sink", "//VCU.myvin/body.access/1/rpc.UpdateDoor"
+        )
         cloud_event.__setitem__("source", "//bo.cloud/petapp//dog")
         validator = Validators.REQUEST.validator()
         result = validator.validate(cloud_event)
         self.assertEqual(
-            "Invalid RPC Request CloudEvent source [//bo.cloud/petapp//dog]. " + "Invalid RPC uri application " +
-            "response topic. UriPart is missing rpc.response.",
-            result.get_message())
+            "Invalid RPC Request CloudEvent source [//bo.cloud/petapp//dog]. "
+            + "Invalid RPC uri application "
+            + "response topic. UriPart is missing rpc.response.",
+            result.get_message(),
+        )
 
     def test_request_type_cloudevent_is_not_valid_missing_sink(self):
         uuid = Factories.UPROTOCOL.create()
         str_uuid = LongUuidSerializer.instance().serialize(uuid)
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("id", str_uuid)
         cloud_event.__setitem__("type", "req.v1")
         cloud_event.__setitem__("source", "//bo.cloud/petapp//rpc.response")
         validator = Validators.REQUEST.validator()
         result = validator.validate(cloud_event)
         self.assertEqual(
             "Invalid RPC Request CloudEvent sink. Request CloudEvent sink must be uri for the method to be called.",
-            result.get_message())
+            result.get_message(),
+        )
 
-    def test_request_type_cloudevent_is_not_valid_invalid_sink_not_rpc_command(self):
+    def test_request_type_cloudevent_is_not_valid_invalid_sink_not_rpc_command(
+        self,
+    ):
         uuid = Factories.UPROTOCOL.create()
         str_uuid = LongUuidSerializer.instance().serialize(uuid)
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("id", str_uuid)
         cloud_event.__setitem__("type", "req.v1")
         cloud_event.__setitem__("source", "//bo.cloud/petapp//rpc.response")
         cloud_event.__setitem__("sink", "//VCU.myvin/body.access/1/UpdateDoor")
         validator = Validators.REQUEST.validator()
         result = validator.validate(cloud_event)
         self.assertEqual(
-            "Invalid RPC Request CloudEvent sink [//VCU.myvin/body.access/1/UpdateDoor]. " + "Invalid RPC method " +
-            "uri. UriPart should be the method to be called, or method from response.",
-            result.get_message())
+            "Invalid RPC Request CloudEvent sink [//VCU.myvin/body.access/1/UpdateDoor]. "
+            + "Invalid RPC method "
+            + "uri. UriPart should be the method to be called, or method from response.",
+            result.get_message(),
+        )
 
     def test_response_type_cloudevent_is_valid_when_everything_is_valid(self):
         uuid = Factories.UPROTOCOL.create()
         str_uuid = LongUuidSerializer.instance().serialize(uuid)
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("id", str_uuid)
         cloud_event.__setitem__("type", "res.v1")
         cloud_event.__setitem__("sink", "//bo.cloud/petapp//rpc.response")
-        cloud_event.__setitem__("source", "//VCU.myvin/body.access/1/rpc.UpdateDoor")
+        cloud_event.__setitem__(
+            "source", "//VCU.myvin/body.access/1/rpc.UpdateDoor"
+        )
         validator = Validators.RESPONSE.validator()
         result = validator.validate(cloud_event)
         self.assertEqual(ValidationResult.success(), result)
 
     def test_response_type_cloudevent_is_not_valid_invalid_source(self):
         uuid = Factories.UPROTOCOL.create()
         str_uuid = LongUuidSerializer.instance().serialize(uuid)
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("id", str_uuid)
         cloud_event.__setitem__("type", "res.v1")
         cloud_event.__setitem__("sink", "//bo.cloud/petapp//rpc.response")
-        cloud_event.__setitem__("source", "//VCU.myvin/body.access/1/UpdateDoor")
+        cloud_event.__setitem__(
+            "source", "//VCU.myvin/body.access/1/UpdateDoor"
+        )
         validator = Validators.RESPONSE.validator()
         result = validator.validate(cloud_event)
         self.assertEqual(
-            "Invalid RPC Response CloudEvent source [//VCU.myvin/body.access/1/UpdateDoor]. " + "Invalid RPC " +
-            "method uri. UriPart should be the method to be called, or method from response.",
-            result.get_message())
-
-    def test_response_type_cloudevent_is_not_valid_missing_sink_and_invalid_source(self):
+            "Invalid RPC Response CloudEvent source [//VCU.myvin/body.access/1/UpdateDoor]. "
+            + "Invalid RPC "
+            + "method uri. UriPart should be the method to be called, or method from response.",
+            result.get_message(),
+        )
+
+    def test_response_type_cloudevent_is_not_valid_missing_sink_and_invalid_source(
+        self,
+    ):
         uuid = Factories.UPROTOCOL.create()
         str_uuid = LongUuidSerializer.instance().serialize(uuid)
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("id", str_uuid)
         cloud_event.__setitem__("type", "res.v1")
-        cloud_event.__setitem__("source", "//VCU.myvin/body.access/1/UpdateDoor")
+        cloud_event.__setitem__(
+            "source", "//VCU.myvin/body.access/1/UpdateDoor"
+        )
         validator = Validators.RESPONSE.validator()
         result = validator.validate(cloud_event)
         self.assertEqual(
-            "Invalid RPC Response CloudEvent source [//VCU.myvin/body.access/1/UpdateDoor]. " + "Invalid RPC " +
-            "method uri. UriPart should be the method to be called, or method from response.," + "Invalid" + " CloudEvent sink. Response CloudEvent sink must be uri the destination of the response.",
-            result.get_message())
+            "Invalid RPC Response CloudEvent source [//VCU.myvin/body.access/1/UpdateDoor]. "
+            + "Invalid RPC "
+            + "method uri. UriPart should be the method to be called, or method from response.,"
+            + "Invalid"
+            + " CloudEvent sink. Response CloudEvent sink must be uri the destination of the response.",
+            result.get_message(),
+        )
 
     def test_response_type_cloudevent_is_not_valid_invalid_sink(self):
         uuid = Factories.UPROTOCOL.create()
         str_uuid = LongUuidSerializer.instance().serialize(uuid)
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("id", str_uuid)
         cloud_event.__setitem__("type", "res.v1")
         cloud_event.__setitem__("sink", "//bo.cloud")
         cloud_event.__setitem__("source", "//VCU.myvin")
         validator = Validators.RESPONSE.validator()
         result = validator.validate(cloud_event)
         self.assertEqual(
-            "Invalid RPC Response CloudEvent source [//VCU.myvin]. Invalid RPC method uri. Uri is missing " +
-            "uSoftware Entity name.,Invalid RPC Response CloudEvent sink [//bo.cloud]. Invalid RPC uri " +
-            "application response topic. Uri is missing uSoftware Entity name.",
-            result.get_message())
-
-    def test_response_type_cloudevent_is_not_valid_invalid_source_not_rpc_command(self):
+            "Invalid RPC Response CloudEvent source [//VCU.myvin]. Invalid RPC method uri. Uri is missing "
+            + "uSoftware Entity name.,Invalid RPC Response CloudEvent sink [//bo.cloud]. Invalid RPC uri "
+            + "application response topic. Uri is missing uSoftware Entity name.",
+            result.get_message(),
+        )
+
+    def test_response_type_cloudevent_is_not_valid_invalid_source_not_rpc_command(
+        self,
+    ):
         uuid = Factories.UPROTOCOL.create()
         str_uuid = LongUuidSerializer.instance().serialize(uuid)
-        cloud_event = build_base_cloud_event_for_test()
+        cloud_event = build_base_publish_cloud_event_for_test()
         cloud_event.__setitem__("id", str_uuid)
         cloud_event.__setitem__("type", "res.v1")
         cloud_event.__setitem__("source", "//bo.cloud/petapp/1/dog")
         cloud_event.__setitem__("sink", "//VCU.myvin/body.access/1/UpdateDoor")
         validator = Validators.RESPONSE.validator()
         result = validator.validate(cloud_event)
         self.assertEqual(
-            "Invalid RPC Response CloudEvent source [//bo.cloud/petapp/1/dog]. Invalid RPC method uri. UriPart " +
-            "should be the method to be called, or method from response.," + "Invalid RPC Response " + "CloudEvent "
-                                                                                                       "sink ["
-                                                                                                       "//VCU.myvin/body.access/1/UpdateDoor]. " + "Invalid RPC uri application " + "response topic. UriPart is missing rpc.response.",
-            result.get_message())
+            "Invalid RPC Response CloudEvent source [//bo.cloud/petapp/1/dog]. Invalid RPC method uri. UriPart "
+            + "should be the method to be called, or method from response.,"
+            + "Invalid RPC Response "
+            + "CloudEvent "
+            "sink ["
+            "//VCU.myvin/body.access/1/UpdateDoor]. "
+            + "Invalid RPC uri application "
+            + "response topic. UriPart is missing rpc.response.",
+            result.get_message(),
+        )
 
     def test_create_a_v6_cloudevent_and_validate_it_against_sdk(self):
         source = build_long_uri_for_test()
         uuid = Factories.UUIDV6.create()
         id = LongUuidSerializer.instance().serialize(uuid)
-        proto_payload=build_proto_payload_for_test()
+        proto_payload = build_proto_payload_for_test()
         # additional attributes
-        u_cloud_event_attributes = UCloudEventAttributesBuilder().with_priority(
-            UPriority.UPRIORITY_CS0).with_ttl(1000).build()
+        u_cloud_event_attributes = (
+            UCloudEventAttributesBuilder()
+            .with_priority(UPriority.UPRIORITY_CS0)
+            .with_ttl(1000)
+            .build()
+        )
         # build the cloud event
-        cloud_event = CloudEventFactory.build_base_cloud_event(id, source, proto_payload.SerializeToString(),
-                                                               proto_payload.type_url, u_cloud_event_attributes,
-                                                               UCloudEvent.get_event_type(
-                                                                   UMessageType.UMESSAGE_TYPE_PUBLISH))
+        cloud_event = CloudEventFactory.build_base_cloud_event(
+            id,
+            source,
+            proto_payload.SerializeToString(),
+            proto_payload.type_url,
+            u_cloud_event_attributes,
+            UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_PUBLISH),
+        )
         validator = Validators.PUBLISH.validator()
         result = validator.validate(cloud_event)
         self.assertTrue(result.is_success())
         self.assertFalse(UCloudEvent.is_expired(cloud_event))
+
+    def fetching_the_notification_validator(self):
+        cloud_event = build_base_notification_cloud_event_for_test()
+        validator = CloudEventValidator.get_validator(cloud_event)
+        status = validator.validate_type(cloud_event).to_status()
+        self.assertEqual(status, ValidationResult.STATUS_SUCCESS)
+        self.assertEqual("CloudEventValidator.Notification", str(validator))
```

### Comparing `up_python-0.1.1.dev0/tests/test_cloudevent/test_validator/test_validationresult.py` & `up_python-0.1.2.dev0/tests/test_cloudevent/test_validator/test_validationresult.py`

 * *Files identical despite different names*

### Comparing `up_python-0.1.1.dev0/tests/test_rpc/test_rpc.py` & `up_python-0.1.2.dev0/tests/test_rpc/test_rpc.py`

 * *Files 22% similar despite different names*

```diff
@@ -25,121 +25,166 @@
 # -------------------------------------------------------------------------
 
 
 import unittest
 from concurrent.futures import Future
 from google.protobuf.any_pb2 import Any
 from google.protobuf.wrappers_pb2 import Int32Value
-from uprotocol.rpc.calloptions import CallOptions
+from uprotocol.proto.uattributes_pb2 import CallOptions
 
 from uprotocol.cloudevent.cloudevents_pb2 import CloudEvent
-from uprotocol.proto.uattributes_pb2 import UPriority
 from uprotocol.proto.upayload_pb2 import UPayload, UPayloadFormat
 from uprotocol.proto.uri_pb2 import UUri, UEntity, UAuthority
 from uprotocol.proto.ustatus_pb2 import UStatus, UCode
 from uprotocol.rpc.rpcclient import RpcClient
 from uprotocol.rpc.rpcmapper import RpcMapper
-from uprotocol.rpc.rpcresult import RpcResult
-from uprotocol.transport.builder.uattributesbuilder import UAttributesBuilder
 from uprotocol.uri.serializer.longuriserializer import LongUriSerializer
 from uprotocol.uri.factory.uresource_builder import UResourceBuilder
 from uprotocol.proto.umessage_pb2 import UMessage
 
 
 def build_source():
-    return UUri(authority=UAuthority(name="vcu.someVin.veh.ultifi.gm.com"),
-                entity=UEntity(name="petapp.ultifi.gm.com", version_major=1),
-                resource=UResourceBuilder.for_rpc_request(None))
+    return UUri(
+        authority=UAuthority(name="vcu.someVin.veh.ultifi.gm.com"),
+        entity=UEntity(name="petapp.ultifi.gm.com", version_major=1),
+        resource=UResourceBuilder.for_rpc_request(None),
+    )
 
 
 def build_cloud_event():
-    return CloudEvent(spec_version="1.0", source="https://example.com", id="HARTLEY IS THE BEST")
+    return CloudEvent(
+        spec_version="1.0",
+        source="https://example.com",
+        id="HARTLEY IS THE BEST",
+    )
 
 
 def build_upayload():
     any_obj = Any()
     any_obj.Pack(build_cloud_event())
-    return UPayload(format=UPayloadFormat.UPAYLOAD_FORMAT_PROTOBUF, value=any_obj.SerializeToString())
+    return UPayload(
+        format=UPayloadFormat.UPAYLOAD_FORMAT_PROTOBUF,
+        value=any_obj.SerializeToString(),
+    )
 
 
 def build_topic():
     return LongUriSerializer().deserialize("//vcu.vin/hartley/1/rpc.Raise")
 
 
 def build_calloptions():
-    return CallOptions()
+    return CallOptions(ttl=1000)
 
 
 class ReturnsNumber3(RpcClient):
-    def invoke_method(self, topic: UUri, payload: UPayload, options: CallOptions):
+    def invoke_method(
+        self, topic: UUri, payload: UPayload, options: CallOptions
+    ):
         future = Future()
         any_obj = Any()
         any_obj.Pack(Int32Value(value=3))
-        data = UPayload(format=UPayloadFormat.UPAYLOAD_FORMAT_PROTOBUF, value=any_obj.SerializeToString())
+        data = UPayload(
+            format=UPayloadFormat.UPAYLOAD_FORMAT_PROTOBUF,
+            value=any_obj.SerializeToString(),
+        )
         future.set_result(UMessage(payload=data))
         return future
 
 
 class HappyPath(RpcClient):
-    def invoke_method(self, topic: UUri, payload: UPayload, options: CallOptions):
+    def invoke_method(
+        self, topic: UUri, payload: UPayload, options: CallOptions
+    ):
         future = Future()
         data = build_upayload()
         future.set_result(UMessage(payload=data))
         return future
 
 
 class WithUStatusCodeInsteadOfHappyPath(RpcClient):
-    def invoke_method(self, topic: UUri, payload: UPayload, options: CallOptions):
+    def invoke_method(
+        self, topic: UUri, payload: UPayload, options: CallOptions
+    ):
         future = Future()
         status = UStatus(code=UCode.INVALID_ARGUMENT, message="boom")
         any_value = Any()
         any_value.Pack(status)
-        data = UPayload(format=UPayloadFormat.UPAYLOAD_FORMAT_PROTOBUF, value=any_value.SerializeToString())
+        data = UPayload(
+            format=UPayloadFormat.UPAYLOAD_FORMAT_PROTOBUF,
+            value=any_value.SerializeToString(),
+        )
         future.set_result(UMessage(payload=data))
         return future
 
 
 class WithUStatusCodeHappyPath(RpcClient):
-    def invoke_method(self, topic: UUri, payload: UPayload, options: CallOptions):
+    def invoke_method(
+        self, topic: UUri, payload: UPayload, options: CallOptions
+    ):
         future = Future()
         status = UStatus(code=UCode.OK, message="all good")
         any_value = Any()
         any_value.Pack(status)
-        data = UPayload(format=UPayloadFormat.UPAYLOAD_FORMAT_PROTOBUF, value=any_value.SerializeToString())
+        data = UPayload(
+            format=UPayloadFormat.UPAYLOAD_FORMAT_PROTOBUF,
+            value=any_value.SerializeToString(),
+        )
         future.set_result(UMessage(payload=data))
         return future
 
 
 class ThatBarfsCrapyPayload(RpcClient):
-    def invoke_method(self, topic: UUri, payload: UPayload, options: CallOptions):
+    def invoke_method(
+        self, topic: UUri, payload: UPayload, options: CallOptions
+    ):
         future = Future()
-        response = UPayload(format=UPayloadFormat.UPAYLOAD_FORMAT_RAW, value=bytes([0]))
+        response = UPayload(
+            format=UPayloadFormat.UPAYLOAD_FORMAT_RAW, value=bytes([0])
+        )
         future.set_result(UMessage(payload=response))
         return future
 
 
 class ThatCompletesWithAnException(RpcClient):
-    def invoke_method(self, topic: UUri, payload: UPayload, options: CallOptions):
+    def invoke_method(
+        self, topic: UUri, payload: UPayload, options: CallOptions
+    ):
         future = Future()
         future.set_exception(RuntimeError("Boom"))
         return future
 
 
 class ThatReturnsTheWrongProto(RpcClient):
-    def invoke_method(self, topic: UUri, payload: UPayload, options: CallOptions):
+    def invoke_method(
+        self, topic: UUri, payload: UPayload, options: CallOptions
+    ):
         future = Future()
         any_value = Any()
         any_value.Pack(Int32Value(value=42))
-        data = UPayload(format=UPayloadFormat.UPAYLOAD_FORMAT_PROTOBUF, value=any_value.SerializeToString())
+        data = UPayload(
+            format=UPayloadFormat.UPAYLOAD_FORMAT_PROTOBUF,
+            value=any_value.SerializeToString(),
+        )
         future.set_result(UMessage(payload=data))
         return future
 
 
+class WithNullMessage(RpcClient):
+    def invoke_method(
+        self, topic: UUri, payload: UPayload, options: CallOptions
+    ):
+        future = Future()
+        future.set_result(UMessage())
+        return future
+
+
 class WithNullInPayload(RpcClient):
-    def invoke_method(self, topic: UUri, payload: UPayload, options: CallOptions):
+    def invoke_method(
+        self, topic: UUri, payload: UPayload, options: CallOptions
+    ):
         future = Future()
         future.set_result(None)
         return future
 
 
 def rpc_response(invoke_method_response: Future):
     payload, exception = invoke_method_response.result()
@@ -165,88 +210,159 @@
 
     # this will be called only if the expected return type is not status, but status was returned to
     # indicate a problem.
     if any_value.Is(UStatus.DESCRIPTOR):
         try:
             status = UStatus()
             any_value.Unpack(status)
-            raise RuntimeError(f"Error returned, status code: [{status.code}], message: [{status.message}]")
+            raise RuntimeError(
+                f"Error returned, status code: [{status.code}], message: [{status.message}]"
+            )
         except Exception as e:
             raise RuntimeError(f"{str(e)} [com.google.grpc.UStatus]") from e
 
     raise RuntimeError(f"Unknown payload type [{any_value.type_url}]")
 
 
 class TestRpc(unittest.TestCase):
 
     def test_compose_happy_path(self):
         rpc_response = RpcMapper.map_response_to_result(
-            ReturnsNumber3().invoke_method(build_topic(), build_upayload(), build_calloptions()), Int32Value)
+            ReturnsNumber3().invoke_method(
+                build_topic(), build_upayload(), build_calloptions()
+            ),
+            Int32Value,
+        )
         mapped = rpc_response.map(lambda x: x.value + 5)
         self.assertTrue(rpc_response.isSuccess())
         self.assertEqual(8, mapped.successValue())
 
     def test_compose_that_returns_status(self):
         rpc_response = RpcMapper.map_response_to_result(
-            WithUStatusCodeInsteadOfHappyPath().invoke_method(build_topic(), build_upayload(), build_calloptions()),
-            Int32Value)
+            WithUStatusCodeInsteadOfHappyPath().invoke_method(
+                build_topic(), build_upayload(), build_calloptions()
+            ),
+            Int32Value,
+        )
         mapped = rpc_response.map(lambda x: x.value + 5)
         self.assertTrue(rpc_response.isFailure())
         self.assertEqual(UCode.INVALID_ARGUMENT, mapped.failureValue().code)
         self.assertEqual("boom", mapped.failureValue().message)
 
     def test_compose_with_failure(self):
         rpc_response = RpcMapper.map_response_to_result(
-            ThatCompletesWithAnException().invoke_method(build_topic(), build_upayload(), build_calloptions()),
-            Int32Value)
+            ThatCompletesWithAnException().invoke_method(
+                build_topic(), build_upayload(), build_calloptions()
+            ),
+            Int32Value,
+        )
         mapped = rpc_response.map(lambda x: x.value + 5)
         self.assertTrue(rpc_response.isFailure())
         status = UStatus(code=UCode.UNKNOWN, message="Boom")
         self.assertEqual(status, mapped.failureValue())
 
-    def test_success_invoke_method_happy_flow_using_mapResponseToRpcResponse(self):
+    def test_map_response_with_payload_is_null(self):
         rpc_response = RpcMapper.map_response_to_result(
-            HappyPath().invoke_method(build_topic(), build_upayload(), build_calloptions()),
-            CloudEvent)
+            WithNullInPayload().invoke_method(
+                build_topic(), None, build_calloptions()
+            ),
+            UStatus,
+        )
+        mapped = rpc_response.map(lambda x: x.value + 5)
+        self.assertTrue(rpc_response.isFailure())
+        self.assertEqual(UCode.UNKNOWN, mapped.failureValue().code)
+        self.assertEqual(
+            "Server returned a null payload. Expected UStatus",
+            mapped.failureValue().message,
+        )
+
+    def test_success_invoke_method_happy_flow_using_mapResponseToRpcResponse(
+        self,
+    ):
+        rpc_response = RpcMapper.map_response_to_result(
+            HappyPath().invoke_method(
+                build_topic(), build_upayload(), build_calloptions()
+            ),
+            CloudEvent,
+        )
         self.assertTrue(rpc_response.isSuccess())
         self.assertEqual(build_cloud_event(), rpc_response.successValue())
 
-    def test_fail_invoke_method_when_invoke_method_returns_a_status_using_mapResponseToRpcResponse(self):
+    def test_fail_invoke_method_when_invoke_method_returns_a_status_using_mapResponseToRpcResponse(
+        self,
+    ):
         rpc_response = RpcMapper.map_response_to_result(
-            WithUStatusCodeInsteadOfHappyPath().invoke_method(build_topic(), build_upayload(), build_calloptions()),
-            CloudEvent)
+            WithUStatusCodeInsteadOfHappyPath().invoke_method(
+                build_topic(), build_upayload(), build_calloptions()
+            ),
+            CloudEvent,
+        )
         self.assertTrue(rpc_response.isFailure())
-        self.assertEqual(UCode.INVALID_ARGUMENT, rpc_response.failureValue().code)
+        self.assertEqual(
+            UCode.INVALID_ARGUMENT, rpc_response.failureValue().code
+        )
         self.assertEqual("boom", rpc_response.failureValue().message)
 
-    def test_fail_invoke_method_when_invoke_method_threw_an_exception_using_mapResponseToRpcResponse(self):
+    def test_fail_invoke_method_when_invoke_method_threw_an_exception_using_mapResponseToRpcResponse(
+        self,
+    ):
         rpc_response = RpcMapper.map_response_to_result(
-            ThatCompletesWithAnException().invoke_method(build_topic(), build_upayload(), build_calloptions()),
-            CloudEvent)
+            ThatCompletesWithAnException().invoke_method(
+                build_topic(), build_upayload(), build_calloptions()
+            ),
+            CloudEvent,
+        )
         self.assertTrue(rpc_response.isFailure())
         self.assertEqual(UCode.UNKNOWN, rpc_response.failureValue().code)
         self.assertEqual("Boom", rpc_response.failureValue().message)
 
-    def test_fail_invoke_method_when_invoke_method_returns_a_bad_proto_using_mapResponseToRpcResponse(self):
+    def test_fail_invoke_method_when_invoke_method_returns_a_bad_proto_using_mapResponseToRpcResponse(
+        self,
+    ):
         rpc_response = RpcMapper.map_response_to_result(
-            ThatReturnsTheWrongProto().invoke_method(build_topic(), build_upayload(), build_calloptions()),
-            CloudEvent)
+            ThatReturnsTheWrongProto().invoke_method(
+                build_topic(), build_upayload(), build_calloptions()
+            ),
+            CloudEvent,
+        )
         self.assertTrue(rpc_response.isFailure())
         self.assertEqual(UCode.UNKNOWN, rpc_response.failureValue().code)
         self.assertEqual(
             "Unknown payload type [type.googleapis.com/google.protobuf.Int32Value]. Expected ["
             "io.cloudevents.v1.CloudEvent]",
-            rpc_response.failureValue().message)
+            rpc_response.failureValue().message,
+        )
 
     def test_success_invoke_method_happy_flow_using_mapResponse(self):
         rpc_response = RpcMapper.map_response(
-            HappyPath().invoke_method(build_topic(), build_upayload(), build_calloptions()),
-            CloudEvent)
+            HappyPath().invoke_method(
+                build_topic(), build_upayload(), build_calloptions()
+            ),
+            CloudEvent,
+        )
         self.assertEqual(build_cloud_event(), rpc_response.result())
 
-    def test_fail_invoke_method_when_invoke_method_returns_a_status_using_mapResponse(self):
+    def test_fail_invoke_method_when_invoke_method_returns_a_status_using_mapResponse(
+        self,
+    ):
+        rpc_response = RpcMapper.map_response(
+            WithUStatusCodeInsteadOfHappyPath().invoke_method(
+                build_topic(), build_upayload(), build_calloptions()
+            ),
+            CloudEvent,
+        )
+        exception = RuntimeError(
+            "Unknown payload type [type.googleapis.com/uprotocol.v1.UStatus]. Expected [CloudEvent]"
+        )
+        self.assertEqual(str(exception), str(rpc_response.exception()))
+
+    def test_map_response_when_response_message_is_null(self):
         rpc_response = RpcMapper.map_response(
-            WithUStatusCodeInsteadOfHappyPath().invoke_method(build_topic(), build_upayload(), build_calloptions()),
-            CloudEvent)
+            WithNullMessage().invoke_method(
+                build_topic(), build_upayload(), build_calloptions()
+            ),
+            CloudEvent,
+        )
         exception = RuntimeError(
-            "Unknown payload type [type.googleapis.com/uprotocol.v1.UStatus]. Expected [CloudEvent]")
+            "Server returned a null payload. Expected CloudEvent"
+        )
         self.assertEqual(str(exception), str(rpc_response.exception()))
```

### Comparing `up_python-0.1.1.dev0/tests/test_rpc/test_rpcresult.py` & `up_python-0.1.2.dev0/tests/test_rpc/test_rpcresult.py`

 * *Files identical despite different names*

### Comparing `up_python-0.1.1.dev0/tests/test_transport/test_validate/test_uattributesvalidator.py` & `up_python-0.1.2.dev0/tests/test_transport/test_validate/test_uattributesvalidator.py`

 * *Files 10% similar despite different names*

```diff
@@ -22,248 +22,350 @@
 # SPDX-FileCopyrightText: 2023 General Motors GTO LLC
 # SPDX-License-Identifier: Apache-2.0
 #
 # -------------------------------------------------------------------------
 
 import time
 import unittest
+import uuid
 
 from uprotocol.proto.uattributes_pb2 import UPriority
 from uprotocol.proto.uri_pb2 import UUri, UAuthority, UEntity
-from uprotocol.proto.ustatus_pb2 import UCode
 from uprotocol.proto.uuid_pb2 import UUID
+from uprotocol.proto.uattributes_pb2 import UAttributes
 from uprotocol.transport.builder.uattributesbuilder import UAttributesBuilder
-from uprotocol.transport.validate.uattributesvalidator import UAttributesValidator, Validators
+from uprotocol.transport.validate.uattributesvalidator import (
+    UAttributesValidator,
+    Validators,
+)
 from uprotocol.uri.factory.uresource_builder import UResourceBuilder
 from uprotocol.uri.serializer.longuriserializer import LongUriSerializer
 from uprotocol.uuid.factory.uuidfactory import Factories
 from uprotocol.validation.validationresult import ValidationResult
 
 
 def build_sink():
-    return UUri(authority=UAuthority(name="vcu.someVin.veh.ultifi.gm.com"),
-                entity=UEntity(name="petapp.ultifi.gm.com", version_major=1),
-                resource=UResourceBuilder.for_rpc_response())
+    return UUri(
+        authority=UAuthority(name="vcu.someVin.veh.ultifi.gm.com"),
+        entity=UEntity(name="petapp.ultifi.gm.com", version_major=1),
+        resource=UResourceBuilder.for_rpc_response(),
+    )
+
 
 def build_source():
-    return UUri(authority=UAuthority(name="vcu.someVin.veh.ultifi.gm.com"),
-                entity=UEntity(name="petapp.ultifi.gm.com", version_major=1),
-                resource=UResourceBuilder.for_rpc_request(None))
+    return UUri(
+        authority=UAuthority(name="vcu.someVin.veh.ultifi.gm.com"),
+        entity=UEntity(name="petapp.ultifi.gm.com", version_major=1),
+        resource=UResourceBuilder.for_rpc_request(None),
+    )
+
 
 class TestUAttributesValidator(unittest.TestCase):
 
-    def test_fetching_validator_for_valid_types(self):
-        publish = UAttributesValidator.get_validator(UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0).build())
+    def test_fetching_validator_for_publish_type(self):
+        publish = UAttributesValidator.get_validator(
+            UAttributesBuilder.publish(
+                build_source(), UPriority.UPRIORITY_CS0
+            ).build()
+        )
         self.assertEqual("UAttributesValidator.Publish", str(publish))
 
+    def test_fetching_validator_for_request_type(self):
         request = UAttributesValidator.get_validator(
-            UAttributesBuilder.request(build_source(), UUri(), UPriority.UPRIORITY_CS4, 1000).build())
+            UAttributesBuilder.request(
+                build_source(), UUri(), UPriority.UPRIORITY_CS4, 1000
+            ).build()
+        )
         self.assertEqual("UAttributesValidator.Request", str(request))
 
+    def test_fetching_validator_for_response_type(self):
         response = UAttributesValidator.get_validator(
-            UAttributesBuilder.response(build_source(), UUri(), UPriority.UPRIORITY_CS4, Factories.UPROTOCOL.create()).build())
+            UAttributesBuilder.response(
+                build_source(),
+                UUri(),
+                UPriority.UPRIORITY_CS4,
+                Factories.UPROTOCOL.create(),
+            ).build()
+        )
         self.assertEqual("UAttributesValidator.Response", str(response))
 
+    def test_fetching_validator_for_notification_type(self):
+        response = UAttributesValidator.get_validator(
+            UAttributesBuilder.notification(
+                build_source(), UUri(), UPriority.UPRIORITY_CS4
+            ).build()
+        )
+        self.assertEqual("UAttributesValidator.Notification", str(response))
+
+    def test_fetching_validator_for_no_type(self):
+        response = UAttributesValidator.get_validator(UAttributes())
+        self.assertEqual("UAttributesValidator.Publish", str(response))
+
     def test_validate_uAttributes_for_publish_message_payload(self):
-        attributes = UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0).build()
+        attributes = UAttributesBuilder.publish(
+            build_source(), UPriority.UPRIORITY_CS0
+        ).build()
         validator = Validators.PUBLISH.validator()
         status = validator.validate(attributes)
         self.assertTrue(status.is_success())
         self.assertEqual("", status.get_message())
 
     def test_validate_uAttributes_for_publish_message_payload_alls(self):
-        attributes = UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0).withTtl(1000).withSink(
-            build_sink()).withPermissionLevel(2).withCommStatus(3).withReqId(Factories.UPROTOCOL.create()).build()
+        attributes = (
+            UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0)
+            .withTtl(1000)
+            .withSink(build_sink())
+            .withPermissionLevel(2)
+            .withCommStatus(3)
+            .withReqId(Factories.UPROTOCOL.create())
+            .build()
+        )
 
         validator = Validators.PUBLISH.validator()
         status = validator.validate(attributes)
         self.assertTrue(status.is_success())
         self.assertEqual("", status.get_message())
 
-    def test_validate_uAttributes_for_publish_message_payload_invalid_type(self):
-        attributes = UAttributesBuilder.response(build_source(), build_sink(), UPriority.UPRIORITY_CS0,
-                                                 Factories.UPROTOCOL.create()).build()
+    def test_validate_uAttributes_for_publish_message_payload_invalid_type(
+        self,
+    ):
+        attributes = UAttributesBuilder.response(
+            build_source(),
+            build_sink(),
+            UPriority.UPRIORITY_CS0,
+            Factories.UPROTOCOL.create(),
+        ).build()
         validator = Validators.PUBLISH.validator()
         status = validator.validate(attributes)
         self.assertTrue(status.is_failure())
-        self.assertEqual("Wrong Attribute Type [UMESSAGE_TYPE_RESPONSE]", status.get_message())
-
-    def test_validate_uAttributes_for_publish_message_payload_invalid_ttl(self):
-        attributes = UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0).withTtl(-1).build()
-
-        validator = Validators.PUBLISH.validator()
-        status = validator.validate(attributes)
-        self.assertTrue(status.is_failure())
-        self.assertEqual("Invalid TTL [-1]", status.get_message())
-
-    def test_validate_uAttributes_for_publish_message_payload_invalid_sink(self):
-        attributes = UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0).withSink(UUri()).build()
+        self.assertEqual(
+            "Wrong Attribute Type [UMESSAGE_TYPE_RESPONSE]",
+            status.get_message(),
+        )
+
+    def test_validate_uAttributes_for_publish_message_payload_invalid_ttl(
+        self,
+    ):
+        with self.assertRaises(ValueError) as context:
+            UAttributesBuilder.publish(
+                build_source(), UPriority.UPRIORITY_CS0
+            ).withTtl(-1).build()
+            self.assertTrue("Value out of range: -1" in context.exception)
+
+    def test_validate_uAttributes_for_publish_message_payload_invalid_sink(
+        self,
+    ):
+        attributes = (
+            UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0)
+            .withSink(UUri())
+            .build()
+        )
         validator = Validators.PUBLISH.validator()
         status = validator.validate(attributes)
         self.assertTrue(status.is_failure())
         self.assertEqual("Uri is empty.", status.get_message())
 
-    def test_validate_uAttributes_for_publish_message_payload_invalid_permission_level(self):
-        attributes = UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0).withPermissionLevel(-42).build()
-        validator = Validators.PUBLISH.validator()
-        status = validator.validate(attributes)
-        self.assertTrue(status.is_failure())
-        self.assertEqual("Invalid Permission Level", status.get_message())
-
-    def test_validate_uAttributes_for_publish_message_payload_invalid_communication_status(self):
-        attributes = UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0).withCommStatus(-42).build()
-        validator = Validators.PUBLISH.validator()
-        status = validator.validate(attributes)
-        self.assertTrue(status.is_failure())
-        self.assertEqual("Invalid Communication Status Code", status.get_message())
+    def test_validate_uAttributes_for_publish_message_payload_invalid_permission_level(
+        self,
+    ):
+        with self.assertRaises(ValueError) as context:
+            UAttributesBuilder.publish(
+                build_source(), UPriority.UPRIORITY_CS0
+            ).withPermissionLevel(-42).build()
+            self.assertTrue("Value out of range: -42" in context.exception)
 
     # def test_validate_uAttributes_for_publish_message_payload_invalid_request_id(self):
     #     uuid = java.util.UUID.randomUUID()
     #     attributes = UAttributesBuilder.publish(UPriority.UPRIORITY_CS0).withReqId(
     #         UUID.newBuilder().setMsb(uuid_java.getMostSignificantBits()).setLsb(uuid_java.getLeastSignificantBits())
     #         .build()).build()
     #
     #     validator = Validators.PUBLISH.validator()
     #     status = validator.validate(attributes)
     #     self.assertTrue(status.is_failure())
     #     self.assertEqual("Invalid UUID", status.get_message())
 
     def test_validate_uAttributes_for_rpc_request_message_payload(self):
-        attributes = UAttributesBuilder.request(build_source(), build_sink(), UPriority.UPRIORITY_CS4, 1000).build()
+        attributes = UAttributesBuilder.request(
+            build_source(), build_sink(), UPriority.UPRIORITY_CS4, 1000
+        ).build()
         validator = Validators.REQUEST.validator()
         status = validator.validate(attributes)
         self.assertTrue(status.is_success())
         self.assertEqual("", status.get_message())
 
     def test_validate_uAttributes_for_rpc_request_message_payload_alls(self):
-        attributes = UAttributesBuilder.request(build_source(), build_sink(), UPriority.UPRIORITY_CS4, 1000).withPermissionLevel(
-            2).withCommStatus(3).withReqId(Factories.UPROTOCOL.create()).build()
+        attributes = (
+            UAttributesBuilder.request(
+                build_source(), build_sink(), UPriority.UPRIORITY_CS4, 1000
+            )
+            .withPermissionLevel(2)
+            .withCommStatus(3)
+            .withReqId(Factories.UPROTOCOL.create())
+            .build()
+        )
 
         validator = Validators.REQUEST.validator()
         status = validator.validate(attributes)
         self.assertTrue(status.is_success())
         self.assertEqual("", status.get_message())
 
-    def test_validate_uAttributes_for_rpc_request_message_payload_invalid_type(self):
-        attributes = UAttributesBuilder.response(build_source(), build_sink(), UPriority.UPRIORITY_CS4,
-                                                 Factories.UPROTOCOL.create()).withTtl(1000).build()
+    def test_validate_uAttributes_for_rpc_request_message_payload_invalid_type(
+        self,
+    ):
+        attributes = (
+            UAttributesBuilder.response(
+                build_source(),
+                build_sink(),
+                UPriority.UPRIORITY_CS4,
+                Factories.UPROTOCOL.create(),
+            )
+            .withTtl(1000)
+            .build()
+        )
 
         validator = Validators.REQUEST.validator()
         status = validator.validate(attributes)
         self.assertTrue(status.is_failure())
-        self.assertEqual("Wrong Attribute Type [UMESSAGE_TYPE_RESPONSE]", status.get_message())
-
-    def test_validate_uAttributes_for_rpc_request_message_payload_invalid_ttl(self):
-        attributes = UAttributesBuilder.request(build_source(), build_sink(), UPriority.UPRIORITY_CS4, -1).build()
-
-        validator = Validators.REQUEST.validator()
-        status = validator.validate(attributes)
-        self.assertTrue(status.is_failure())
-        self.assertEqual("Invalid TTL [-1]", status.get_message())
-
-    def test_validate_uAttributes_for_rpc_request_message_payload_invalid_sink(self):
-        attributes = UAttributesBuilder.request(build_source(), UUri(), UPriority.UPRIORITY_CS4, 1000).build()
+        self.assertEqual(
+            "Wrong Attribute Type [UMESSAGE_TYPE_RESPONSE]",
+            status.get_message(),
+        )
+
+    def test_validate_uAttributes_for_rpc_request_message_payload_invalid_ttl(
+        self,
+    ):
+        with self.assertRaises(ValueError) as context:
+            UAttributesBuilder.request(
+                build_source(), build_sink(), UPriority.UPRIORITY_CS4, -1
+            ).build()
+            self.assertTrue("Value out of range: -1" in context.exception)
+
+    def test_validate_uAttributes_for_rpc_request_message_payload_invalid_sink(
+        self,
+    ):
+        attributes = UAttributesBuilder.request(
+            build_source(), UUri(), UPriority.UPRIORITY_CS4, 1000
+        ).build()
 
         validator = Validators.REQUEST.validator()
         status = validator.validate(attributes)
         self.assertTrue(status.is_failure())
         self.assertEqual("Uri is empty.", status.get_message())
 
-    def test_validate_uAttributes_for_rpc_request_message_payload_invalid_permission_level(self):
-        attributes = UAttributesBuilder.request(build_source(), build_sink(), UPriority.UPRIORITY_CS4, 1000).withPermissionLevel(
-            -42).build()
-
-        validator = Validators.REQUEST.validator()
-        status = validator.validate(attributes)
-        self.assertTrue(status.is_failure())
-        self.assertEqual("Invalid Permission Level", status.get_message())
-
-    def test_validate_uAttributes_for_rpc_request_message_payload_invalid_communication_status(self):
-        attributes = UAttributesBuilder.request(build_source(), build_sink(), UPriority.UPRIORITY_CS4, 1000).withCommStatus(-42).build()
-
-        validator = Validators.REQUEST.validator()
-        status = validator.validate(attributes)
-        self.assertTrue(status.is_failure())
-        self.assertEqual("Invalid Communication Status Code", status.get_message())
+    def test_validate_uAttributes_for_rpc_request_message_payload_invalid_permission_level(
+        self,
+    ):
+        with self.assertRaises(ValueError) as context:
+            UAttributesBuilder.request(
+                build_source(), build_sink(), UPriority.UPRIORITY_CS4, 1000
+            ).withPermissionLevel(-42).build()
+            self.assertTrue("Value out of range: -42" in context.exception)
 
     # def test_validate_uAttributes_for_rpc_request_message_payload_invalid_request_id(self):
     #     uuid_java = java.util.UUID.randomUUID()
     #     attributes = UAttributesBuilder.request(UPriority.UPRIORITY_CS4, build_sink(), 1000).withReqId(
     #         UUID.newBuilder().setMsb(uuid_java.getMostSignificantBits()).setLsb(uuid_java.getLeastSignificantBits())
     #         .build()).build()
     #
     #     validator = Validators.REQUEST.validator()
     #     status = validator.validate(attributes)
     #     self.assertTrue(status.is_failure())
     #     self.assertEqual("Invalid UUID", status.get_message())
 
     def test_validate_uAttributes_for_rpc_response_message_payload(self):
-        attributes = UAttributesBuilder.response(build_source(), build_sink(), UPriority.UPRIORITY_CS4,
-                                                 Factories.UPROTOCOL.create()).build()
+        attributes = UAttributesBuilder.response(
+            build_source(),
+            build_sink(),
+            UPriority.UPRIORITY_CS4,
+            Factories.UPROTOCOL.create(),
+        ).build()
 
         validator = Validators.RESPONSE.validator()
         status = validator.validate(attributes)
         self.assertTrue(status.is_success())
         self.assertEqual("", status.get_message())
 
     def test_validate_uAttributes_for_rpc_response_message_payload_alls(self):
-        attributes = UAttributesBuilder.response(build_source(), build_sink(), UPriority.UPRIORITY_CS4, 
-                                                 Factories.UPROTOCOL.create()).withPermissionLevel(2).withCommStatus(
-            3).build()
+        attributes = (
+            UAttributesBuilder.response(
+                build_source(),
+                build_sink(),
+                UPriority.UPRIORITY_CS4,
+                Factories.UPROTOCOL.create(),
+            )
+            .withPermissionLevel(2)
+            .withCommStatus(3)
+            .build()
+        )
 
         validator = Validators.RESPONSE.validator()
         status = validator.validate(attributes)
         self.assertTrue(status.is_success())
         self.assertEqual("", status.get_message())
 
-    def test_validate_uAttributes_for_rpc_response_message_payload_invalid_type(self):
-        attributes = UAttributesBuilder.notification(build_source(), build_sink(), UPriority.UPRIORITY_CS4).build()
-
-        validator = Validators.RESPONSE.validator()
-        status = validator.validate(attributes)
-        self.assertTrue(status.is_failure())
-        self.assertEqual("Wrong Attribute Type [UMESSAGE_TYPE_PUBLISH],Missing correlationId", status.get_message())
-
-    def test_validate_uAttributes_for_rpc_response_message_payload_invalid_ttl(self):
-        attributes = UAttributesBuilder.response(build_source(), build_sink(), UPriority.UPRIORITY_CS4,
-                                                 Factories.UPROTOCOL.create()).withTtl(-1).build()
+    def test_validate_uAttributes_for_rpc_response_message_payload_invalid_type(
+        self,
+    ):
+        attributes = UAttributesBuilder.notification(
+            build_source(), build_sink(), UPriority.UPRIORITY_CS4
+        ).build()
 
         validator = Validators.RESPONSE.validator()
         status = validator.validate(attributes)
         self.assertTrue(status.is_failure())
-        self.assertEqual("Invalid TTL [-1]", status.get_message())
-
-    def test_validate_uAttributes_for_rpc_response_message_payload_missing_sink_and_missing_requestId(self):
-        attributes = UAttributesBuilder.response(build_source(), UUri(), UPriority.UPRIORITY_CS4, UUID()).build()
+        self.assertEqual(
+            "Wrong Attribute Type [UMESSAGE_TYPE_NOTIFICATION],Missing correlationId",
+            status.get_message(),
+        )
+
+    def test_validate_uAttributes_for_rpc_response_message_payload_invalid_ttl(
+        self,
+    ):
+        with self.assertRaises(ValueError) as context:
+            UAttributesBuilder.response(
+                build_source(),
+                build_sink(),
+                UPriority.UPRIORITY_CS4,
+                Factories.UPROTOCOL.create(),
+            ).withTtl(-1).build()
+            self.assertTrue("Value out of range: -1" in context.exception)
+
+    def test_validate_uAttributes_for_rpc_response_message_payload_missing_sink_and_missing_requestId(
+        self,
+    ):
+        attributes = UAttributesBuilder.response(
+            build_source(), UUri(), UPriority.UPRIORITY_CS4, UUID()
+        ).build()
 
         validator = Validators.RESPONSE.validator()
         status = validator.validate(attributes)
         self.assertTrue(status.is_failure())
-        self.assertEqual("Missing Sink,Missing correlationId", status.get_message())
-
-    def test_validate_uAttributes_for_rpc_response_message_payload_invalid_permission_level(self):
-        attributes = UAttributesBuilder.response(build_source(), build_sink(), UPriority.UPRIORITY_CS4,
-                                                 Factories.UPROTOCOL.create()).withPermissionLevel(-42).build()
-
-        validator = Validators.RESPONSE.validator()
-        status = validator.validate(attributes)
-        self.assertTrue(status.is_failure())
-        self.assertEqual("Invalid Permission Level", status.get_message())
-
-    def test_validate_uAttributes_for_rpc_response_message_payload_invalid_communication_status(self):
-        attributes = UAttributesBuilder.response(build_source(), build_sink(), UPriority.UPRIORITY_CS4, 
-                                                 Factories.UPROTOCOL.create()).withCommStatus(-42).build()
-
-        validator = Validators.RESPONSE.validator()
-        status = validator.validate(attributes)
-        self.assertTrue(status.is_failure())
-        self.assertEqual("Invalid Communication Status Code", status.get_message())
-
-    def test_validate_uAttributes_for_rpc_response_message_payload_missing_request_id(self):
-        attributes = UAttributesBuilder.response(build_source(), build_sink(), UPriority.UPRIORITY_CS4, UUID()).build()
+        self.assertEqual(
+            "Missing Sink,Missing correlationId", status.get_message()
+        )
+
+    def test_validate_uAttributes_for_rpc_response_message_payload_invalid_permission_level(
+        self,
+    ):
+        with self.assertRaises(ValueError) as context:
+            UAttributesBuilder.response(
+                build_source(),
+                build_sink(),
+                UPriority.UPRIORITY_CS4,
+                Factories.UPROTOCOL.create(),
+            ).withPermissionLevel(-42).build()
+            self.assertTrue("Value out of range: -42" in context.exception)
+
+    def test_validate_uAttributes_for_rpc_response_message_payload_missing_request_id(
+        self,
+    ):
+        attributes = UAttributesBuilder.response(
+            build_source(), build_sink(), UPriority.UPRIORITY_CS4, UUID()
+        ).build()
 
         validator = Validators.RESPONSE.validator()
         status = validator.validate(attributes)
         self.assertTrue(status.is_failure())
         self.assertEqual("Missing correlationId", status.get_message())
 
     # def test_validate_uAttributes_for_rpc_response_message_payload_invalid_request_id(self):
@@ -274,226 +376,335 @@
     #
     #     validator = Validators.RESPONSE.validator()
     #     status = validator.validate(attributes)
     #     self.assertTrue(status.is_failure())
     #     self.assertEqual(f"Invalid correlationId [{reqid}]", status.get_message())
 
     # ----
-    def test_validate_uAttributes_for_publish_message_payload_not_expired(self):
-        attributes = UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0).build()
+    def test_validate_uAttributes_for_publish_message_payload_not_expired(
+        self,
+    ):
+        attributes = UAttributesBuilder.publish(
+            build_source(), UPriority.UPRIORITY_CS0
+        ).build()
 
         validator = Validators.PUBLISH.validator()
         self.assertFalse(validator.is_expired(attributes))
 
-    def test_validate_uAttributes_for_publish_message_payload_not_expired_withTtl_zero(self):
-        attributes = UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0).withTtl(0).build()
+    def test_validate_uAttributes_for_publish_message_payload_not_expired_withTtl_zero(
+        self,
+    ):
+        attributes = (
+            UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0)
+            .withTtl(0)
+            .build()
+        )
 
         validator = Validators.PUBLISH.validator()
         self.assertFalse(validator.is_expired(attributes))
 
-    def test_validate_uAttributes_for_publish_message_payload_not_expired_withTtl(self):
-        attributes = UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0).withTtl(10000).build()
+    def test_validate_uAttributes_for_publish_message_payload_not_expired_withTtl(
+        self,
+    ):
+        attributes = (
+            UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0)
+            .withTtl(10000)
+            .build()
+        )
 
         validator = Validators.PUBLISH.validator()
         self.assertFalse(validator.is_expired(attributes))
 
-    def test_validate_uAttributes_for_publish_message_payload_expired_withTtl(self):
-        attributes = UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0).withTtl(1).build()
+    def test_validate_uAttributes_for_publish_message_payload_expired_withTtl(
+        self,
+    ):
+        attributes = (
+            UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0)
+            .withTtl(1)
+            .build()
+        )
 
         time.sleep(0.8)
 
         validator = Validators.PUBLISH.validator()
         self.assertTrue(validator.is_expired(attributes))
 
     # ----
 
     def test_validating_publish_invalid_ttl_attribute(self):
-        attributes = UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0).withTtl(-1).build()
-
-        validator = Validators.PUBLISH.validator()
-        status = validator.validate_ttl(attributes)
-        self.assertTrue(status.is_failure())
-        self.assertEqual("Invalid TTL [-1]", status.get_message())
+        with self.assertRaises(ValueError) as context:
+            UAttributesBuilder.publish(
+                build_source(), UPriority.UPRIORITY_CS0
+            ).withTtl(-1).build()
+            self.assertTrue("Value out of range: -1" in context.exception)
 
     def test_validating_valid_ttl_attribute(self):
-        attributes = UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0).withTtl(100).build()
+        attributes = (
+            UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0)
+            .withTtl(100)
+            .build()
+        )
 
         validator = Validators.PUBLISH.validator()
         status = validator.validate_ttl(attributes)
         self.assertEqual(ValidationResult.success(), status)
 
     def test_validating_invalid_sink_attribute(self):
         uri = LongUriSerializer().deserialize("//")
-        attributes = UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0).withSink(uri).build()
+        attributes = (
+            UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0)
+            .withSink(uri)
+            .build()
+        )
         validator = Validators.PUBLISH.validator()
         status = validator.validate_sink(attributes)
         self.assertTrue(status.is_failure())
         self.assertEqual("Uri is empty.", status.get_message())
 
     def test_validating_valid_sink_attribute(self):
-        uri = UUri(authority=UAuthority(name="vcu.someVin.veh.ultifi.gm.com"),
-                   entity=UEntity(name="petapp.ultifi.gm.com", version_major=1),
-                   resource=UResourceBuilder.for_rpc_response())
-        attributes = UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0).withSink(uri).build()
+        uri = UUri(
+            authority=UAuthority(name="vcu.someVin.veh.ultifi.gm.com"),
+            entity=UEntity(name="petapp.ultifi.gm.com", version_major=1),
+            resource=UResourceBuilder.for_rpc_response(),
+        )
+        attributes = (
+            UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0)
+            .withSink(uri)
+            .build()
+        )
 
         validator = Validators.PUBLISH.validator()
         status = validator.validate_sink(attributes)
         self.assertEqual(ValidationResult.success(), status)
 
     # def test_validating_invalid_ReqId_attribute(self):
-    #     uuid_java = java.util.UUID.randomUUID()
-    #
-    #     attributes = UAttributesBuilder.publish(UPriority.UPRIORITY_CS0).with_req_id(
-    #         UUID.newBuilder().setMsb(uuid_java.getMostSignificantBits()).setLsb(uuid_java.getLeastSignificantBits())
-    #         .build()).build()
-    #
+    #     uuid_python = uuid.UUID('12345678123456781234567812345678')
+
+    #     attributes = (
+    #         UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0)
+    #         .withReqId(None)
+    #         .build()
+    #     )
+
     #     validator = Validators.PUBLISH.validator()
     #     status = validator.validate_req_id(attributes)
     #     self.assertTrue(status.is_failure())
     #     self.assertEqual("Invalid UUID", status.get_message())
 
     def test_validating_valid_ReqId_attribute(self):
-        attributes = UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0).withReqId(
-            Factories.UPROTOCOL.create()).build()
+        attributes = (
+            UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0)
+            .withReqId(Factories.UPROTOCOL.create())
+            .build()
+        )
 
         validator = Validators.PUBLISH.validator()
         status = validator.validate_req_id(attributes)
         self.assertEqual(ValidationResult.success(), status)
 
-    def test_validating_invalid_PermissionLevel_attribute(self):
-        attributes = UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0).withPermissionLevel(-1).build()
+    def test_validating_valid_type_attribute(self):
+        attributes = (
+            UAttributesBuilder.notification(build_source(), build_sink(), UPriority.UPRIORITY_CS0)
+            .withReqId(Factories.UPROTOCOL.create())
+            .build()
+        )
 
-        validator = Validators.PUBLISH.validator()
-        status = validator.validate_permission_level(attributes)
-        self.assertTrue(status.is_failure())
-        self.assertEqual("Invalid Permission Level", status.get_message())
+        validator = Validators.NOTIFICATION.validator()
+        status = validator.validate_type(attributes)
+        self.assertEqual(ValidationResult.success(), status)
+
+    def test_validating_valid_sink_attribute(self):
+        attributes = (
+            UAttributesBuilder.notification(build_source(), build_sink(), UPriority.UPRIORITY_CS0)
+            .withReqId(Factories.UPROTOCOL.create())
+            .build()
+        )
+
+        validator = Validators.NOTIFICATION.validator()
+        status = validator.validate_sink(attributes)
+        self.assertEqual(ValidationResult.success(), status)
+
+    def test_validating_none_attribute(self):
+        attributes = None
+
+        validator = Validators.NOTIFICATION.validator()
+        status = validator.validate_sink(attributes)
+        self.assertEqual("UAttributes cannot be null.", status.get_message())
+
+    def test_validating_invalid_sink_attribute(self):
+        attributes = (
+            UAttributesBuilder.notification(build_source(), UUri(), UPriority.UPRIORITY_CS0)
+            .withReqId(Factories.UPROTOCOL.create())
+            .build()
+        )
+
+        validator = Validators.NOTIFICATION.validator()
+        status = validator.validate_sink(attributes)
+        self.assertEqual("Missing Sink", status.get_message())
+
+
+    def test_validating_invalid_PermissionLevel_attribute(self):
+        with self.assertRaises(ValueError) as context:
+            UAttributesBuilder.publish(
+                build_source(), UPriority.UPRIORITY_CS0
+            ).withPermissionLevel(-1).build()
+            self.assertTrue("Value out of range: -1" in context.exception)
 
     def test_validating_valid_PermissionLevel_attribute(self):
-        attributes = UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0).withPermissionLevel(3).build()
+        attributes = (
+            UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0)
+            .withPermissionLevel(3)
+            .build()
+        )
 
         validator = Validators.PUBLISH.validator()
         status = validator.validate_permission_level(attributes)
         self.assertEqual(ValidationResult.success(), status)
 
     def test_validating_valid_PermissionLevel_attribute_invalid(self):
-        attributes = UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0).withPermissionLevel(0).build()
+        attributes = (
+            UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0)
+            .withPermissionLevel(0)
+            .build()
+        )
 
         validator = Validators.PUBLISH.validator()
         status = validator.validate_permission_level(attributes)
         self.assertTrue(status.is_failure())
         self.assertEqual("Invalid Permission Level", status.get_message())
 
-    def test_validating_invalid_commstatus_attribute(self):
-        attributes = UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0).withCommStatus(100).build()
-
-        validator = Validators.PUBLISH.validator()
-        status = validator.validate_comm_status(attributes)
-        self.assertTrue(status.is_failure())
-        self.assertEqual("Invalid Communication Status Code", status.get_message())
-
-    def test_validating_valid_commstatus_attribute(self):
-        attributes = UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0).withCommStatus(UCode.ABORTED).build()
-
-        validator = Validators.PUBLISH.validator()
-        status = validator.validate_comm_status(attributes)
-        self.assertEqual(ValidationResult.success(), status)
-
     def test_validating_request_message_types(self):
-        attributes = UAttributesBuilder.request(build_source(), build_sink(), UPriority.UPRIORITY_CS6, 100).build()
+        attributes = UAttributesBuilder.request(
+            build_source(), build_sink(), UPriority.UPRIORITY_CS6, 100
+        ).build()
 
         validator = UAttributesValidator.get_validator(attributes)
         self.assertEqual("UAttributesValidator.Request", str(validator))
         status = validator.validate(attributes)
         self.assertTrue(status.is_success())
         self.assertEqual("", status.get_message())
 
     def test_validating_request_validator_with_wrong_messagetype(self):
-        attributes = UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS6).build()
+        attributes = UAttributesBuilder.publish(
+            build_source(), UPriority.UPRIORITY_CS6
+        ).build()
 
         validator = Validators.REQUEST.validator()
         self.assertEqual("UAttributesValidator.Request", str(validator))
         status = validator.validate(attributes)
         self.assertTrue(status.is_failure())
-        self.assertEqual("Wrong Attribute Type [UMESSAGE_TYPE_PUBLISH],Missing TTL,Missing Sink", status.get_message())
+        self.assertEqual(
+            "Wrong Attribute Type [UMESSAGE_TYPE_PUBLISH],Missing TTL,Missing Sink",
+            status.get_message(),
+        )
 
     def test_validating_request_validator_with_wrong_bad_ttl(self):
-        attributes = UAttributesBuilder.request(build_source(), LongUriSerializer().deserialize("/hartley/1/rpc.response"), 
-                                                UPriority.UPRIORITY_CS6, -1).build()
-
-        validator = Validators.REQUEST.validator()
-        self.assertEqual("UAttributesValidator.Request", str(validator))
-        status = validator.validate(attributes)
-        self.assertTrue(status.is_failure())
-        self.assertEqual("Invalid TTL [-1]", status.get_message())
+        with self.assertRaises(ValueError) as context:
+            UAttributesBuilder.request(
+                build_source(),
+                LongUriSerializer().deserialize("/hartley/1/rpc.response"),
+                UPriority.UPRIORITY_CS6,
+                -1,
+            ).build()
+            self.assertTrue("Value out of range: -1" in context.exception)
 
     def test_validating_response_validator_with_wrong_bad_ttl(self):
-        attributes = UAttributesBuilder.response(build_source(), LongUriSerializer().deserialize("/hartley/1/rpc.response"), 
-                                                 UPriority.UPRIORITY_CS6, Factories.UPROTOCOL.create()).withTtl(-1).build()
-
-        validator = Validators.RESPONSE.validator()
-        self.assertEqual("UAttributesValidator.Response", str(validator))
-        status = validator.validate(attributes)
-        self.assertTrue(status.is_failure())
-        self.assertEqual("Invalid TTL [-1]", status.get_message())
+        with self.assertRaises(ValueError) as context:
+            UAttributesBuilder.response(
+                build_source(),
+                LongUriSerializer().deserialize("/hartley/1/rpc.response"),
+                UPriority.UPRIORITY_CS6,
+                Factories.UPROTOCOL.create(),
+            ).withTtl(-1).build()
+            self.assertTrue("Value out of range: -1" in context.exception)
 
     def test_validating_publish_validator_with_wrong_messagetype(self):
-        attributes = UAttributesBuilder.request(build_source(), build_sink(), UPriority.UPRIORITY_CS6, 1000).build()
+        attributes = UAttributesBuilder.request(
+            build_source(), build_sink(), UPriority.UPRIORITY_CS6, 1000
+        ).build()
         validator = Validators.PUBLISH.validator()
         self.assertEqual("UAttributesValidator.Publish", str(validator))
         status = validator.validate(attributes)
         self.assertTrue(status.is_failure())
-        self.assertEqual("Wrong Attribute Type [UMESSAGE_TYPE_REQUEST]", status.get_message())
+        self.assertEqual(
+            "Wrong Attribute Type [UMESSAGE_TYPE_REQUEST]",
+            status.get_message(),
+        )
 
     def test_validating_response_validator_with_wrong_messagetype(self):
-        attributes = UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS6).build()
+        attributes = UAttributesBuilder.publish(
+            build_source(), UPriority.UPRIORITY_CS6
+        ).build()
 
         validator = Validators.RESPONSE.validator()
         self.assertEqual("UAttributesValidator.Response", str(validator))
         status = validator.validate(attributes)
         self.assertTrue(status.is_failure())
-        self.assertEqual("Wrong Attribute Type [UMESSAGE_TYPE_PUBLISH],Missing Sink,Missing correlationId",
-                         status.get_message())
+        self.assertEqual(
+            "Wrong Attribute Type [UMESSAGE_TYPE_PUBLISH],Missing Sink,Missing correlationId",
+            status.get_message(),
+        )
 
     def test_validating_request_containing_token(self):
-        attributes = UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0).withToken("null").build()
+        attributes = (
+            UAttributesBuilder.publish(build_source(), UPriority.UPRIORITY_CS0)
+            .withToken("null")
+            .build()
+        )
 
         validator = UAttributesValidator.get_validator(attributes)
         self.assertEqual("UAttributesValidator.Publish", str(validator))
         status = validator.validate(attributes)
         self.assertEqual(ValidationResult.success(), status)
 
     def test_valid_request_methoduri_in_sink(self):
         sink = LongUriSerializer().deserialize("/test.service/1/rpc.method")
-        attributes = UAttributesBuilder.request(build_source(), sink, UPriority.UPRIORITY_CS0, 3000).build()
+        attributes = UAttributesBuilder.request(
+            build_source(), sink, UPriority.UPRIORITY_CS0, 3000
+        ).build()
         validator = UAttributesValidator.get_validator(attributes)
         self.assertEqual("UAttributesValidator.Request", str(validator))
         status = validator.validate(attributes)
         self.assertEqual(ValidationResult.success(), status)
 
     def test_invalid_request_methoduri_in_sink(self):
         sink = LongUriSerializer().deserialize("/test.client/1/test.response")
-        attributes = UAttributesBuilder.request(build_source(),  sink, UPriority.UPRIORITY_CS0, 3000).build()
+        attributes = UAttributesBuilder.request(
+            build_source(), sink, UPriority.UPRIORITY_CS0, 3000
+        ).build()
         validator = UAttributesValidator.get_validator(attributes)
         self.assertEqual("UAttributesValidator.Request", str(validator))
         status = validator.validate(attributes)
-        self.assertEqual("Invalid RPC method uri. Uri should be the method to be called, or method from response.", status.get_message())
+        self.assertEqual(
+            "Invalid RPC method uri. Uri should be the method to be called, or method from response.",
+            status.get_message(),
+        )
 
     def test_valid_response_uri_in_sink(self):
         sink = LongUriSerializer().deserialize("/test.client/1/rpc.response")
-        attributes = UAttributesBuilder.response(build_source(), sink, UPriority.UPRIORITY_CS0, Factories.UPROTOCOL.create()).build()
+        attributes = UAttributesBuilder.response(
+            build_source(),
+            sink,
+            UPriority.UPRIORITY_CS0,
+            Factories.UPROTOCOL.create(),
+        ).build()
         validator = UAttributesValidator.get_validator(attributes)
         self.assertEqual("UAttributesValidator.Response", str(validator))
         status = validator.validate(attributes)
         self.assertEqual(ValidationResult.success(), status)
 
     def test_invalid_response_uri_in_sink(self):
         sink = LongUriSerializer().deserialize("/test.client/1/rpc.method")
-        attributes = UAttributesBuilder.response(build_source(), sink, UPriority.UPRIORITY_CS0, Factories.UPROTOCOL.create()).build()
+        attributes = UAttributesBuilder.response(
+            build_source(),
+            sink,
+            UPriority.UPRIORITY_CS0,
+            Factories.UPROTOCOL.create(),
+        ).build()
         validator = UAttributesValidator.get_validator(attributes)
         self.assertEqual("UAttributesValidator.Response", str(validator))
         status = validator.validate(attributes)
         self.assertEqual("Invalid RPC response type.", status.get_message())
 
 
-
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `up_python-0.1.1.dev0/tests/test_uri/test_serializer/test_longuriserializer.py` & `up_python-0.1.2.dev0/tests/test_uri/test_serializer/test_longuriserializer.py`

 * *Files 7% similar despite different names*

```diff
@@ -32,78 +32,81 @@
 from uprotocol.uri.serializer.longuriserializer import LongUriSerializer
 from uprotocol.uri.validator.urivalidator import UriValidator
 
 
 class TestLongUriSerializer(unittest.TestCase):
 
     def test_using_the_serializers(self):
-        uri = UUri(entity=UEntity(name="hartley"), resource=UResourceBuilder.for_rpc_request("raise"))
+        uri = UUri(
+            entity=UEntity(name="hartley"),
+            resource=UResourceBuilder.for_rpc_request("raise"),
+        )
 
         str_uri = LongUriSerializer().serialize(uri)
         self.assertEqual("/hartley//rpc.raise", str_uri)
         uri2 = LongUriSerializer().deserialize(str_uri)
         self.assertEqual(uri, uri2)
 
     def test_parse_protocol_uri_when_is_null(self):
         uri = LongUriSerializer().deserialize(None)
         self.assertTrue(UriValidator.is_empty(uri))
         self.assertFalse(UriValidator.is_resolved(uri))
         self.assertFalse(UriValidator.is_long_form(uri))
 
     def test_parse_protocol_uri_when_is_empty_string(self):
-        uri = ''
+        uri = ""
         uuri = LongUriSerializer().deserialize(uri)
         self.assertTrue(UriValidator.is_empty(uuri))
         uri2 = LongUriSerializer().serialize(None)
         self.assertTrue(len(uri2) == 0)
 
     def test_parse_protocol_uri_with_schema_and_slash(self):
         uri = "/"
         uuri = LongUriSerializer().deserialize(uri)
-        self.assertFalse(uuri.HasField('authority'))
+        self.assertFalse(uuri.HasField("authority"))
         self.assertTrue(UriValidator.is_empty(uuri))
-        self.assertFalse(uuri.HasField('resource'))
-        self.assertFalse(uuri.HasField('entity'))
+        self.assertFalse(uuri.HasField("resource"))
+        self.assertFalse(uuri.HasField("entity"))
         uri2 = LongUriSerializer().serialize(UUri())
         self.assertTrue(len(uri2) == 0)
 
     def test_parse_protocol_uri_with_schema_and_double_slash(self):
         uri = "//"
         uuri = LongUriSerializer().deserialize(uri)
-        self.assertFalse(uuri.HasField('authority'))
-        self.assertFalse(uuri.HasField('resource'))
-        self.assertFalse(uuri.HasField('entity'))
+        self.assertFalse(uuri.HasField("authority"))
+        self.assertFalse(uuri.HasField("resource"))
+        self.assertFalse(uuri.HasField("entity"))
         self.assertTrue(UriValidator.is_empty(uuri))
 
     def test_parse_protocol_uri_with_schema_and_3_slash_and_something(self):
         uri = "///body.access"
         uuri = LongUriSerializer().deserialize(uri)
-        self.assertFalse(uuri.HasField('authority'))
-        self.assertFalse(uuri.HasField('resource'))
-        self.assertFalse(uuri.HasField('entity'))
+        self.assertFalse(uuri.HasField("authority"))
+        self.assertFalse(uuri.HasField("resource"))
+        self.assertFalse(uuri.HasField("entity"))
         self.assertTrue(UriValidator.is_empty(uuri))
         self.assertNotEqual("body.access", uuri.entity.name)
         self.assertEqual(0, uuri.entity.version_major)
 
     def test_parse_protocol_uri_with_schema_and_4_slash_and_something(self):
         uri = "////body.access"
         uuri = LongUriSerializer().deserialize(uri)
 
         self.assertFalse(UriValidator.is_remote(uuri.authority))
-        self.assertFalse(uuri.HasField('resource'))
-        self.assertFalse(uuri.HasField('entity'))
+        self.assertFalse(uuri.HasField("resource"))
+        self.assertFalse(uuri.HasField("entity"))
         self.assertTrue(len(uuri.entity.name) == 0)
         self.assertEqual(0, uuri.entity.version_major)
 
     def test_parse_protocol_uri_with_schema_and_5_slash_and_something(self):
         uri = "/////body.access"
         uuri = LongUriSerializer().deserialize(uri)
         self.assertFalse(UriValidator.is_remote(uuri.authority))
-        self.assertFalse(uuri.HasField('resource'))
-        self.assertFalse(uuri.HasField('entity'))
+        self.assertFalse(uuri.HasField("resource"))
+        self.assertFalse(uuri.HasField("entity"))
         self.assertTrue(UriValidator.is_empty(uuri))
 
     def test_parse_protocol_uri_with_schema_and_6_slash_and_something(self):
         uri = "//////body.access"
         uuri = LongUriSerializer().deserialize(uri)
 
         self.assertFalse(UriValidator.is_remote(uuri.authority))
@@ -113,83 +116,95 @@
         uri = "/body.access"
         uuri = LongUriSerializer().deserialize(uri)
 
         self.assertFalse(UriValidator.is_remote(uuri.authority))
         self.assertEqual("body.access", uuri.entity.name)
         self.assertEqual(0, uuri.entity.version_major)
         self.assertEqual(0, uuri.entity.version_minor)
-        self.assertFalse(uuri.HasField('resource'))
+        self.assertFalse(uuri.HasField("resource"))
 
     def test_parse_protocol_uri_with_local_service_with_version(self):
         uri = "/body.access/1"
         uuri = LongUriSerializer().deserialize(uri)
 
         self.assertFalse(UriValidator.is_remote(uuri.authority))
         self.assertEqual("body.access", uuri.entity.name)
         self.assertEqual(1, uuri.entity.version_major)
-        self.assertFalse(uuri.HasField('resource'))
+        self.assertFalse(uuri.HasField("resource"))
 
-    def test_parse_protocol_uri_with_local_service_no_version_with_resource_name_only(self):
+    def test_parse_protocol_uri_with_local_service_no_version_with_resource_name_only(
+        self,
+    ):
         uri = "/body.access//door"
         uuri = LongUriSerializer().deserialize(uri)
 
         self.assertFalse(UriValidator.is_remote(uuri.authority))
         self.assertEqual("body.access", uuri.entity.name)
         self.assertEqual(0, uuri.entity.version_major)
         self.assertEqual(0, uuri.entity.version_minor)
         self.assertEqual("door", uuri.resource.name)
         self.assertTrue(len(uuri.resource.instance) == 0)
         self.assertTrue(len(uuri.resource.message) == 0)
 
-    def test_parse_protocol_uri_with_local_service_with_version_with_resource_name_only(self):
+    def test_parse_protocol_uri_with_local_service_with_version_with_resource_name_only(
+        self,
+    ):
         uri = "/body.access/1/door"
         uuri = LongUriSerializer().deserialize(uri)
         self.assertFalse(UriValidator.is_remote(uuri.authority))
         self.assertEqual("body.access", uuri.entity.name)
         self.assertEqual(1, uuri.entity.version_major)
         self.assertEqual("door", uuri.resource.name)
         self.assertTrue(len(uuri.resource.instance) == 0)
         self.assertTrue(len(uuri.resource.message) == 0)
 
-    def test_parse_protocol_uri_with_local_service_no_version_with_resource_with_instance(self):
+    def test_parse_protocol_uri_with_local_service_no_version_with_resource_with_instance(
+        self,
+    ):
         uri = "/body.access//door.front_left"
         uuri = LongUriSerializer().deserialize(uri)
         self.assertFalse(UriValidator.is_remote(uuri.authority))
         self.assertEqual("body.access", uuri.entity.name)
         self.assertEqual(0, uuri.entity.version_major)
         self.assertEqual("door", uuri.resource.name)
         self.assertFalse(len(uuri.resource.instance) == 0)
         self.assertEqual("front_left", uuri.resource.instance)
         self.assertTrue(len(uuri.resource.message) == 0)
 
-    def test_parse_protocol_uri_with_local_service_with_version_with_resource_with_getMessage(self):
+    def test_parse_protocol_uri_with_local_service_with_version_with_resource_with_getMessage(
+        self,
+    ):
         uri = "/body.access/1/door.front_left"
         uuri = LongUriSerializer().deserialize(uri)
         self.assertFalse(UriValidator.is_remote(uuri.authority))
         self.assertEqual("body.access", uuri.entity.name)
         self.assertNotEqual(0, uuri.entity.version_major)
         self.assertEqual(1, uuri.entity.version_major)
         self.assertEqual("door", uuri.resource.name)
         self.assertFalse(len(uuri.resource.instance) == 0)
         self.assertEqual("front_left", uuri.resource.instance)
         self.assertTrue(len(uuri.resource.message) == 0)
 
-    def test_parse_protocol_uri_with_local_service_no_version_with_resource_with_instance_and_getMessage(self):
+    def test_parse_protocol_uri_with_local_service_no_version_with_resource_with_instance_and_getMessage(
+        self,
+    ):
         uri = "/body.access//door.front_left#Door"
         uuri = LongUriSerializer().deserialize(uri)
         self.assertFalse(UriValidator.is_remote(uuri.authority))
         self.assertEqual("body.access", uuri.entity.name)
         self.assertEqual(0, uuri.entity.version_major)
         self.assertEqual("door", uuri.resource.name)
         self.assertFalse(len(uuri.resource.instance) == 0)
         self.assertEqual("front_left", uuri.resource.instance)
         self.assertFalse(len(uuri.resource.message) == 0)
         self.assertEqual("Door", uuri.resource.message)
 
-    def test_parse_protocol_uri_with_local_service_with_version_with_resource_with_instance_and_getMessage(self):
+    def test_parse_protocol_uri_with_local_service_with_version_with_resource_with_instance_and_getMessage(
+        self,
+    ):
         uri = "/body.access/1/door.front_left#Door"
         uuri = LongUriSerializer().deserialize(uri)
         self.assertFalse(UriValidator.is_remote(uuri.authority))
         self.assertEqual("body.access", uuri.entity.name)
         self.assertNotEqual(0, uuri.entity.version_major)
         self.assertEqual(1, uuri.entity.version_major)
         self.assertEqual("door", uuri.resource.name)
@@ -217,190 +232,212 @@
         self.assertNotEqual(0, uuri.entity.version_major)
         self.assertEqual(1, uuri.entity.version_major)
         self.assertEqual("rpc", uuri.resource.name)
         self.assertFalse(len(uuri.resource.instance) == 0)
         self.assertEqual("response", uuri.resource.instance)
         self.assertTrue(len(uuri.resource.message) == 0)
 
-    def test_parse_protocol_uri_with_remote_service_only_device_and_domain(self):
+    def test_parse_protocol_uri_with_remote_service_only_device_and_domain(
+        self,
+    ):
         uri = "//VCU.MY_CAR_VIN"
         uuri = LongUriSerializer().deserialize(uri)
         self.assertTrue(UriValidator.is_remote(uuri.authority))
         self.assertFalse(len(uuri.authority.name) == 0)
         self.assertEqual("VCU.MY_CAR_VIN", uuri.authority.name)
 
-    def test_parse_protocol_uri_with_remote_service_only_device_and_cloud_domain(self):
+    def test_parse_protocol_uri_with_remote_service_only_device_and_cloud_domain(
+        self,
+    ):
         uri = "//cloud.uprotocol.example.com"
         uuri = LongUriSerializer().deserialize(uri)
         self.assertTrue(UriValidator.is_remote(uuri.authority))
         self.assertFalse(len(uuri.authority.name) == 0)
         self.assertEqual("cloud.uprotocol.example.com", uuri.authority.name)
-        self.assertFalse(uuri.HasField('entity'))
-        self.assertFalse(uuri.HasField('resource'))
+        self.assertFalse(uuri.HasField("entity"))
+        self.assertFalse(uuri.HasField("resource"))
 
     def test_parse_protocol_uri_with_remote_service_no_version(self):
         uri = "//VCU.MY_CAR_VIN/body.access"
         uuri = LongUriSerializer().deserialize(uri)
         self.assertTrue(UriValidator.is_remote(uuri.authority))
         self.assertFalse(len(uuri.authority.name) == 0)
         self.assertEqual("VCU.MY_CAR_VIN", uuri.authority.name)
         self.assertFalse(len(uuri.entity.name) == 0)
         self.assertEqual("body.access", uuri.entity.name)
         self.assertEqual(0, uuri.entity.version_major)
-        self.assertFalse(uuri.HasField('resource'))
+        self.assertFalse(uuri.HasField("resource"))
 
     def test_parse_protocol_uri_with_remote_cloud_service_no_version(self):
         uri = "//cloud.uprotocol.example.com/body.access"
         uuri = LongUriSerializer().deserialize(uri)
         self.assertTrue(UriValidator.is_remote(uuri.authority))
         self.assertFalse(len(uuri.authority.name) == 0)
         self.assertEqual("cloud.uprotocol.example.com", uuri.authority.name)
         self.assertFalse(len(uuri.entity.name) == 0)
         self.assertEqual("body.access", uuri.entity.name)
         self.assertEqual(0, uuri.entity.version_major)
-        self.assertFalse(uuri.HasField('resource'))
+        self.assertFalse(uuri.HasField("resource"))
 
     def test_parse_protocol_uri_with_remote_service_with_version(self):
         uri = "//VCU.MY_CAR_VIN/body.access/1"
         uuri = LongUriSerializer().deserialize(uri)
         self.assertTrue(UriValidator.is_remote(uuri.authority))
         self.assertFalse(len(uuri.authority.name) == 0)
         self.assertEqual("VCU.MY_CAR_VIN", uuri.authority.name)
         self.assertFalse(len(uuri.entity.name) == 0)
         self.assertEqual("body.access", uuri.entity.name)
         self.assertNotEqual(0, uuri.entity.version_major)
         self.assertEqual(1, uuri.entity.version_major)
-        self.assertFalse(uuri.HasField('resource'))
+        self.assertFalse(uuri.HasField("resource"))
 
     def test_parse_protocol_uri_with_remote_cloud_service_with_version(self):
         uri = "//cloud.uprotocol.example.com/body.access/1"
         uuri = LongUriSerializer().deserialize(uri)
         self.assertTrue(UriValidator.is_remote(uuri.authority))
         self.assertFalse(len(uuri.authority.name) == 0)
         self.assertEqual("cloud.uprotocol.example.com", uuri.authority.name)
         self.assertFalse(len(uuri.entity.name) == 0)
         self.assertEqual("body.access", uuri.entity.name)
         self.assertNotEqual(0, uuri.entity.version_major)
         self.assertEqual(1, uuri.entity.version_major)
-        self.assertFalse(uuri.HasField('resource'))
+        self.assertFalse(uuri.HasField("resource"))
 
-    def test_parse_protocol_uri_with_remote_service_no_version_with_resource_name_only(self):
+    def test_parse_protocol_uri_with_remote_service_no_version_with_resource_name_only(
+        self,
+    ):
         uri = "//VCU.MY_CAR_VIN/body.access//door"
         uuri = LongUriSerializer().deserialize(uri)
         self.assertTrue(UriValidator.is_remote(uuri.authority))
         self.assertFalse(len(uuri.authority.name) == 0)
         self.assertEqual("VCU.MY_CAR_VIN", uuri.authority.name)
         self.assertFalse(len(uuri.entity.name) == 0)
         self.assertEqual("body.access", uuri.entity.name)
         self.assertEqual(0, uuri.entity.version_major)
         self.assertEqual("door", uuri.resource.name)
         self.assertTrue(len(uuri.resource.instance) == 0)
         self.assertTrue(len(uuri.resource.message) == 0)
 
-    def test_parse_protocol_uri_with_remote_cloud_service_no_version_with_resource_name_only(self):
+    def test_parse_protocol_uri_with_remote_cloud_service_no_version_with_resource_name_only(
+        self,
+    ):
         uri = "//cloud.uprotocol.example.com/body.access//door"
         uuri = LongUriSerializer().deserialize(uri)
         self.assertTrue(UriValidator.is_remote(uuri.authority))
         self.assertFalse(len(uuri.authority.name) == 0)
         self.assertEqual("cloud.uprotocol.example.com", uuri.authority.name)
         self.assertFalse(len(uuri.entity.name) == 0)
         self.assertEqual("body.access", uuri.entity.name)
         self.assertEqual(0, uuri.entity.version_major)
         self.assertEqual("door", uuri.resource.name)
         self.assertTrue(len(uuri.resource.instance) == 0)
         self.assertTrue(len(uuri.resource.message) == 0)
 
-    def test_parse_protocol_uri_with_remote_service_with_version_with_resource_name_only(self):
+    def test_parse_protocol_uri_with_remote_service_with_version_with_resource_name_only(
+        self,
+    ):
         uri = "//VCU.MY_CAR_VIN/body.access/1/door"
         uuri = LongUriSerializer().deserialize(uri)
         self.assertTrue(UriValidator.is_remote(uuri.authority))
         self.assertFalse(len(uuri.authority.name) == 0)
         self.assertEqual("VCU.MY_CAR_VIN", uuri.authority.name)
         self.assertFalse(len(uuri.entity.name) == 0)
         self.assertEqual("body.access", uuri.entity.name)
         self.assertNotEqual(0, uuri.entity.version_major)
         self.assertEqual(1, uuri.entity.version_major)
         self.assertEqual("door", uuri.resource.name)
         self.assertTrue(len(uuri.resource.instance) == 0)
         self.assertTrue(len(uuri.resource.message) == 0)
 
-    def test_parse_protocol_uri_with_remote_service_cloud_with_version_with_resource_name_only(self):
+    def test_parse_protocol_uri_with_remote_service_cloud_with_version_with_resource_name_only(
+        self,
+    ):
         uri = "//cloud.uprotocol.example.com/body.access/1/door"
         uuri = LongUriSerializer().deserialize(uri)
         self.assertTrue(UriValidator.is_remote(uuri.authority))
         self.assertFalse(len(uuri.authority.name) == 0)
         self.assertEqual("cloud.uprotocol.example.com", uuri.authority.name)
         self.assertFalse(len(uuri.entity.name) == 0)
         self.assertEqual("body.access", uuri.entity.name)
         self.assertNotEqual(0, uuri.entity.version_major)
         self.assertEqual(1, uuri.entity.version_major)
         self.assertEqual("door", uuri.resource.name)
         self.assertTrue(len(uuri.resource.instance) == 0)
         self.assertTrue(len(uuri.resource.message) == 0)
 
-    def test_parse_protocol_uri_with_remote_service_no_version_with_resource_and_instance_no_getMessage(self):
+    def test_parse_protocol_uri_with_remote_service_no_version_with_resource_and_instance_no_getMessage(
+        self,
+    ):
         uri = "//VCU.MY_CAR_VIN/body.access//door.front_left"
         uuri = LongUriSerializer().deserialize(uri)
         self.assertTrue(UriValidator.is_remote(uuri.authority))
         self.assertFalse(len(uuri.authority.name) == 0)
         self.assertEqual("VCU.MY_CAR_VIN", uuri.authority.name)
         self.assertFalse(len(uuri.entity.name) == 0)
         self.assertEqual("body.access", uuri.entity.name)
         self.assertEqual(0, uuri.entity.version_major)
         self.assertEqual("door", uuri.resource.name)
         self.assertFalse(len(uuri.resource.instance) == 0)
         self.assertEqual("front_left", uuri.resource.instance)
         self.assertTrue(len(uuri.resource.message) == 0)
 
-    def test_parse_protocol_uri_with_remote_service_with_version_with_resource_and_instance_no_getMessage(self):
+    def test_parse_protocol_uri_with_remote_service_with_version_with_resource_and_instance_no_getMessage(
+        self,
+    ):
         uri = "//VCU.MY_CAR_VIN/body.access/1/door.front_left"
         uuri = LongUriSerializer().deserialize(uri)
         self.assertTrue(UriValidator.is_remote(uuri.authority))
         self.assertFalse(len(uuri.authority.name) == 0)
         self.assertEqual("VCU.MY_CAR_VIN", uuri.authority.name)
         self.assertFalse(len(uuri.entity.name) == 0)
         self.assertEqual("body.access", uuri.entity.name)
         self.assertNotEqual(0, uuri.entity.version_major)
         self.assertEqual(1, uuri.entity.version_major)
         self.assertEqual("door", uuri.resource.name)
         self.assertFalse(len(uuri.resource.instance) == 0)
         self.assertEqual("front_left", uuri.resource.instance)
         self.assertTrue(len(uuri.resource.message) == 0)
 
-    def test_parse_protocol_uri_with_remote_service_no_version_with_resource_and_instance_and_getMessage(self):
+    def test_parse_protocol_uri_with_remote_service_no_version_with_resource_and_instance_and_getMessage(
+        self,
+    ):
         uri = "//VCU.MY_CAR_VIN/body.access//door.front_left#Door"
         uuri = LongUriSerializer().deserialize(uri)
         self.assertTrue(UriValidator.is_remote(uuri.authority))
         self.assertFalse(len(uuri.authority.name) == 0)
         self.assertEqual("VCU.MY_CAR_VIN", uuri.authority.name)
         self.assertFalse(len(uuri.entity.name) == 0)
         self.assertEqual("body.access", uuri.entity.name)
         self.assertEqual(0, uuri.entity.version_major)
         self.assertEqual("door", uuri.resource.name)
         self.assertFalse(len(uuri.resource.instance) == 0)
         self.assertEqual("front_left", uuri.resource.instance)
         self.assertFalse(len(uuri.resource.message) == 0)
         self.assertEqual("Door", uuri.resource.message)
 
-    def test_parse_protocol_uri_with_remote_cloud_service_no_version_with_resource_and_instance_and_getMessage(self):
+    def test_parse_protocol_uri_with_remote_cloud_service_no_version_with_resource_and_instance_and_getMessage(
+        self,
+    ):
         uri = "//cloud.uprotocol.example.com/body.access//door.front_left#Door"
         uuri = LongUriSerializer().deserialize(uri)
         self.assertTrue(UriValidator.is_remote(uuri.authority))
         self.assertFalse(len(uuri.authority.name) == 0)
         self.assertEqual("cloud.uprotocol.example.com", uuri.authority.name)
         self.assertFalse(len(uuri.entity.name) == 0)
         self.assertEqual("body.access", uuri.entity.name)
         self.assertEqual(0, uuri.entity.version_major)
         self.assertEqual("door", uuri.resource.name)
         self.assertFalse(len(uuri.resource.instance) == 0)
         self.assertEqual("front_left", uuri.resource.instance)
         self.assertFalse(len(uuri.resource.message) == 0)
         self.assertEqual("Door", uuri.resource.message)
 
-    def test_parse_protocol_uri_with_remote_service_with_version_with_resource_and_instance_and_getMessage(self):
+    def test_parse_protocol_uri_with_remote_service_with_version_with_resource_and_instance_and_getMessage(
+        self,
+    ):
         uri = "//VCU.MY_CAR_VIN/body.access/1/door.front_left#Door"
         uuri = LongUriSerializer().deserialize(uri)
         self.assertTrue(UriValidator.is_remote(uuri.authority))
         self.assertFalse(len(uuri.authority.name) == 0)
         self.assertEqual("VCU.MY_CAR_VIN", uuri.authority.name)
         self.assertFalse(len(uuri.entity.name) == 0)
         self.assertEqual("body.access", uuri.entity.name)
@@ -408,31 +445,37 @@
         self.assertEqual(1, uuri.entity.version_major)
         self.assertEqual("door", uuri.resource.name)
         self.assertFalse(len(uuri.resource.instance) == 0)
         self.assertEqual("front_left", uuri.resource.instance)
         self.assertFalse(len(uuri.resource.message) == 0)
         self.assertEqual("Door", uuri.resource.message)
 
-    def test_parse_protocol_uri_with_remote_cloud_service_with_version_with_resource_and_instance_and_getMessage(self):
-        uri = "//cloud.uprotocol.example.com/body.access/1/door.front_left#Door"
+    def test_parse_protocol_uri_with_remote_cloud_service_with_version_with_resource_and_instance_and_getMessage(
+        self,
+    ):
+        uri = (
+            "//cloud.uprotocol.example.com/body.access/1/door.front_left#Door"
+        )
         uuri = LongUriSerializer().deserialize(uri)
         self.assertTrue(UriValidator.is_remote(uuri.authority))
         self.assertFalse(len(uuri.authority.name) == 0)
         self.assertEqual("cloud.uprotocol.example.com", uuri.authority.name)
         self.assertFalse(len(uuri.entity.name) == 0)
         self.assertEqual("body.access", uuri.entity.name)
         self.assertNotEqual(0, uuri.entity.version_major)
         self.assertEqual(1, uuri.entity.version_major)
         self.assertEqual("door", uuri.resource.name)
         self.assertFalse(len(uuri.resource.instance) == 0)
         self.assertEqual("front_left", uuri.resource.instance)
         self.assertFalse(len(uuri.resource.message) == 0)
         self.assertEqual("Door", uuri.resource.message)
 
-    def test_parse_protocol_uri_with_remote_service_with_version_with_resource_with_message_device_no_domain(self):
+    def test_parse_protocol_uri_with_remote_service_with_version_with_resource_with_message_device_no_domain(
+        self,
+    ):
         uri = "//VCU/body.access/1/door.front_left"
         uuri = LongUriSerializer().deserialize(uri)
         self.assertTrue(UriValidator.is_remote(uuri.authority))
         self.assertFalse(len(uuri.authority.name) == 0)
         self.assertEqual("VCU", uuri.authority.name)
         self.assertFalse(len(uuri.entity.name) == 0)
         self.assertEqual("body.access", uuri.entity.name)
@@ -470,174 +513,277 @@
         self.assertEqual("rpc", uuri.resource.name)
         self.assertFalse(len(uuri.resource.instance) == 0)
         self.assertEqual("response", uuri.resource.instance)
         self.assertTrue(len(uuri.resource.message) == 0)
 
     def test_build_protocol_uri_from__uri_when__uri_isnull(self):
         uprotocol_uri = LongUriSerializer().serialize(None)
-        self.assertEqual('', uprotocol_uri)
+        self.assertEqual("", uprotocol_uri)
 
     def test_build_protocol_uri_from__uri_when__uri_isEmpty(self):
         uuri = UUri()
         uprotocol_uri = LongUriSerializer().serialize(uuri)
-        self.assertEqual('', uprotocol_uri)
+        self.assertEqual("", uprotocol_uri)
 
     def test_build_protocol_uri_from__uri_when__uri_has_empty_use(self):
         use = UEntity()
-        uuri = UUri(authority=UAuthority(), entity=use, resource=UResource(name="door"))
+        uuri = UUri(
+            authority=UAuthority(), entity=use, resource=UResource(name="door")
+        )
         uprotocol_uri = LongUriSerializer().serialize(uuri)
         self.assertEqual("/////door", uprotocol_uri)
 
-    def test_build_protocol_uri_from__uri_when__uri_has_local_authority_service_no_version(self):
+    def test_build_protocol_uri_from__uri_when__uri_has_local_authority_service_no_version(
+        self,
+    ):
         uuri = UUri(entity=UEntity(name="body.access"))
         uprotocol_uri = LongUriSerializer().serialize(uuri)
         self.assertEqual("/body.access", uprotocol_uri)
 
-    def test_build_protocol_uri_from__uri_when__uri_has_local_authority_service_and_version(self):
+    def test_build_protocol_uri_from__uri_when__uri_has_local_authority_service_and_version(
+        self,
+    ):
         use = UEntity(name="body.access", version_major=1)
         uuri = UUri(entity=use, resource=UResource())
         uprotocol_uri = LongUriSerializer().serialize(uuri)
         self.assertEqual("/body.access/1", uprotocol_uri)
 
-    def test_build_protocol_uri_from__uri_when__uri_has_local_authority_service_no_version_with_resource(self):
+    def test_build_protocol_uri_from__uri_when__uri_has_local_authority_service_no_version_with_resource(
+        self,
+    ):
         use = UEntity(name="body.access")
         uuri = UUri(entity=use, resource=UResource(name="door"))
         uprotocol_uri = LongUriSerializer().serialize(uuri)
         self.assertEqual("/body.access//door", uprotocol_uri)
 
-    def test_build_protocol_uri_from__uri_when__uri_has_local_authority_service_and_version_with_resource(self):
+    def test_build_protocol_uri_from__uri_when__uri_has_local_authority_service_and_version_with_resource(
+        self,
+    ):
         use = UEntity(name="body.access", version_major=1)
         uuri = UUri(entity=use, resource=UResource(name="door"))
         uprotocol_uri = LongUriSerializer().serialize(uuri)
         self.assertEqual("/body.access/1/door", uprotocol_uri)
 
-    def test_build_protocol_uri_from_uri_when_uri_has_local_authority_service_no_version_with_resource_with_instance_no_getMessage(
-            self):
+    def test_build_protocol_uri_from_uri_when_uri_has_l_authority_service_n_vsn_with_rsrc_with_instance_n_getMessage(
+        self,
+    ):
         use = UEntity(name="body.access")
-        uuri = UUri(entity=use, resource=UResource(name="door", instance="front_left"))
+        uuri = UUri(
+            entity=use, resource=UResource(name="door", instance="front_left")
+        )
         uprotocol_uri = LongUriSerializer().serialize(uuri)
         self.assertEqual("/body.access//door.front_left", uprotocol_uri)
 
-    def test_build_protocol_uri_from_uri_when_uri_has_local_authority_service_and_version_with_resource_with_instance_no_getMessage(
-            self):
-        use = UEntity(name="body.access", version_major=1)
-        uuri = UUri(entity=use, resource=UResource(name="door", instance="front_left"))
+    def test_build_protocol_uri_from_uri_when_uri_has_l_authority_service_and_vsn_with_rsrc_with_instance_n_getMessage(
+        self,
+    ):
+        use = UEntity(name="body.access", version_major=1)
+        uuri = UUri(
+            entity=use, resource=UResource(name="door", instance="front_left")
+        )
         uprotocol_uri = LongUriSerializer().serialize(uuri)
         self.assertEqual("/body.access/1/door.front_left", uprotocol_uri)
 
-    def test_build_protocol_uri_from_uri_when_uri_has_local_authority_service_no_version_with_resource_with_instance_with_getMessage(
-            self):
+    def test_build_protocol_uri_from_uri_when_uri_has_l_authority_svc_no_vsn_with_rsrc_with_instance_with_getMessage(
+        self,
+    ):
         use = UEntity(name="body.access")
-        uuri = UUri(entity=use, resource=UResource(name="door", instance="front_left", message="Door"))
+        uuri = UUri(
+            entity=use,
+            resource=UResource(
+                name="door", instance="front_left", message="Door"
+            ),
+        )
         uprotocol_uri = LongUriSerializer().serialize(uuri)
         self.assertEqual("/body.access//door.front_left#Door", uprotocol_uri)
 
-    def test_build_protocol_uri_from_uri_when_uri_has_local_authority_service_and_version_with_resource_with_instance_with_getMessage(
-            self):
-        use = UEntity(name="body.access", version_major=1)
-        uuri = UUri(entity=use, resource=UResource(name="door", instance="front_left", message="Door"))
+    def test_build_protocol_uri_from_uri_when_uri_has_l_authority_svc_and_vsn_with_rsrc_with_instance_with_getMessage(
+        self,
+    ):
+        use = UEntity(name="body.access", version_major=1)
+        uuri = UUri(
+            entity=use,
+            resource=UResource(
+                name="door", instance="front_left", message="Door"
+            ),
+        )
         uprotocol_uri = LongUriSerializer().serialize(uuri)
         self.assertEqual("/body.access/1/door.front_left#Door", uprotocol_uri)
 
-    def test_build_protocol_uri_from_uri_when_uri_has_remote_authority_service_no_version(self):
+    def test_build_protocol_uri_from_uri_when_uri_has_remote_authority_service_no_version(
+        self,
+    ):
         use = UEntity(name="body.access")
         uuri = UUri(authority=UAuthority(name="vcu.my_car_vin"), entity=use)
         uprotocol_uri = LongUriSerializer().serialize(uuri)
         self.assertEqual("//vcu.my_car_vin/body.access", uprotocol_uri)
 
-    def test_build_protocol_uri_from_uri_when_uri_has_remote_authority_service_and_version(self):
+    def test_build_protocol_uri_from_uri_when_uri_has_remote_authority_service_and_version(
+        self,
+    ):
         use = UEntity(name="body.access", version_major=1)
         uuri = UUri(authority=UAuthority(name="vcu.my_car_vin"), entity=use)
         uprotocol_uri = LongUriSerializer().serialize(uuri)
         self.assertEqual("//vcu.my_car_vin/body.access/1", uprotocol_uri)
 
-    def test_build_protocol_uri_from_uri_when_uri_has_remote_cloud_authority_service_and_version(self):
-        use = UEntity(name="body.access", version_major=1)
-        uuri = UUri(authority=UAuthority(name="cloud.uprotocol.example.com"), entity=use)
-        uprotocol_uri = LongUriSerializer().serialize(uuri)
-        self.assertEqual("//cloud.uprotocol.example.com/body.access/1", uprotocol_uri)
-
-    def test_build_protocol_uri_from_uri_when_uri_has_remote_authority_service_and_version_with_resource(self):
-        use = UEntity(name="body.access", version_major=1)
-        uuri = UUri(authority=UAuthority(name="vcu.my_car_vin"), entity=use, resource=UResource(name="door"))
+    def test_build_protocol_uri_from_uri_when_uri_has_remote_cloud_authority_service_and_version(
+        self,
+    ):
+        use = UEntity(name="body.access", version_major=1)
+        uuri = UUri(
+            authority=UAuthority(name="cloud.uprotocol.example.com"),
+            entity=use,
+        )
+        uprotocol_uri = LongUriSerializer().serialize(uuri)
+        self.assertEqual(
+            "//cloud.uprotocol.example.com/body.access/1", uprotocol_uri
+        )
+
+    def test_build_protocol_uri_from_uri_when_uri_has_remote_authority_service_and_version_with_resource(
+        self,
+    ):
+        use = UEntity(name="body.access", version_major=1)
+        uuri = UUri(
+            authority=UAuthority(name="vcu.my_car_vin"),
+            entity=use,
+            resource=UResource(name="door"),
+        )
         uprotocol_uri = LongUriSerializer().serialize(uuri)
         self.assertEqual("//vcu.my_car_vin/body.access/1/door", uprotocol_uri)
 
-    def test_build_protocol_uri_from_uri_when_uri_has_remote_authority_service_no_version_with_resource(self):
+    def test_build_protocol_uri_from_uri_when_uri_has_remote_authority_service_no_version_with_resource(
+        self,
+    ):
         use = UEntity(name="body.access")
-        uuri = UUri(authority=UAuthority(name="vcu.my_car_vin"), entity=use, resource=UResource(name="door"))
+        uuri = UUri(
+            authority=UAuthority(name="vcu.my_car_vin"),
+            entity=use,
+            resource=UResource(name="door"),
+        )
         uprotocol_uri = LongUriSerializer().serialize(uuri)
         self.assertEqual("//vcu.my_car_vin/body.access//door", uprotocol_uri)
 
-    def test_build_protocol_uri_from_uri_when_uri_has_remote_authority_service_and_version_with_resource_with_instance_no_getMessage(
-            self):
-        use = UEntity(name="body.access", version_major=1)
-        uuri = UUri(authority=UAuthority(name="vcu.my_car_vin"), entity=use,
-                    resource=UResource(name="door", instance="front_left"))
-        uprotocol_uri = LongUriSerializer().serialize(uuri)
-        self.assertEqual("//vcu.my_car_vin/body.access/1/door.front_left", uprotocol_uri)
-
-    def test_build_protocol_uri_from_uri_when_uri_has_remote_cloud_authority_service_and_version_with_resource_with_instance_no_getMessage(
-            self):
-        use = UEntity(name="body.access", version_major=1)
-        uuri = UUri(authority=UAuthority(name="cloud.uprotocol.example.com"), entity=use,
-                    resource=UResource(name="door", instance="front_left"))
-        uprotocol_uri = LongUriSerializer().serialize(uuri)
-        self.assertEqual("//cloud.uprotocol.example.com/body.access/1/door.front_left", uprotocol_uri)
-
-    def test_build_protocol_uri_from_uri_when_uri_has_remote_authority_service_no_version_with_resource_with_instance_no_getMessage(
-            self):
+    def test_build_protocol_uri_from_uri_when_uri_has_r_authority_svc_and_vsn_with_rsrc_with_instance_no_getMessage(
+        self,
+    ):
+        use = UEntity(name="body.access", version_major=1)
+        uuri = UUri(
+            authority=UAuthority(name="vcu.my_car_vin"),
+            entity=use,
+            resource=UResource(name="door", instance="front_left"),
+        )
+        uprotocol_uri = LongUriSerializer().serialize(uuri)
+        self.assertEqual(
+            "//vcu.my_car_vin/body.access/1/door.front_left", uprotocol_uri
+        )
+
+    def test_build_protocol_uri_from_uri_when_uri_has_r_cld_authority_svc_and_vsn_with_rsrc_with_instance_n_getMessage(
+        self,
+    ):
+        use = UEntity(name="body.access", version_major=1)
+        uuri = UUri(
+            authority=UAuthority(name="cloud.uprotocol.example.com"),
+            entity=use,
+            resource=UResource(name="door", instance="front_left"),
+        )
+        uprotocol_uri = LongUriSerializer().serialize(uuri)
+        self.assertEqual(
+            "//cloud.uprotocol.example.com/body.access/1/door.front_left",
+            uprotocol_uri,
+        )
+
+    def test_build_protocol_uri_from_uri_when_uri_has_r_authority_svc_no_vsn_with_resource_with_instance_n_getMessage(
+        self,
+    ):
         use = UEntity(name="body.access")
-        uuri = UUri(authority=UAuthority(name="vcu.my_car_vin"), entity=use,
-                    resource=UResource(name="door", instance="front_left"))
-        uprotocol_uri = LongUriSerializer().serialize(uuri)
-        self.assertEqual("//vcu.my_car_vin/body.access//door.front_left", uprotocol_uri)
-
-    def test_build_protocol_uri_from_uri_when_uri_has_remote_authority_service_and_version_with_resource_with_instance_and_getMessage(
-            self):
-        use = UEntity(name="body.access", version_major=1)
-        uuri = UUri(authority=UAuthority(name="vcu.my_car_vin"), entity=use,
-                    resource=UResource(name="door", instance="front_left", message="Door"))
-        uprotocol_uri = LongUriSerializer().serialize(uuri)
-        self.assertEqual("//vcu.my_car_vin/body.access/1/door.front_left#Door", uprotocol_uri)
-
-    def test_build_protocol_uri_from_uri_when_uri_has_remote_authority_service_no_version_with_resource_with_instance_and_getMessage(
-            self):
+        uuri = UUri(
+            authority=UAuthority(name="vcu.my_car_vin"),
+            entity=use,
+            resource=UResource(name="door", instance="front_left"),
+        )
+        uprotocol_uri = LongUriSerializer().serialize(uuri)
+        self.assertEqual(
+            "//vcu.my_car_vin/body.access//door.front_left", uprotocol_uri
+        )
+
+    def test_build_protocol_uri_from_uri_when_uri_has_r_authority_svc_and_version_with_rsrc_with_i_and_getMessage(
+        self,
+    ):
+        use = UEntity(name="body.access", version_major=1)
+        uuri = UUri(
+            authority=UAuthority(name="vcu.my_car_vin"),
+            entity=use,
+            resource=UResource(
+                name="door", instance="front_left", message="Door"
+            ),
+        )
+        uprotocol_uri = LongUriSerializer().serialize(uuri)
+        self.assertEqual(
+            "//vcu.my_car_vin/body.access/1/door.front_left#Door",
+            uprotocol_uri,
+        )
+
+    def test_build_protocol_uri_from_uri_when_uri_has_r_authority_svc_no_version_with_rsrc_with_i_and_getMessage(
+        self,
+    ):
         use = UEntity(name="body.access")
-        uuri = UUri(authority=UAuthority(name="vcu.my_car_vin"), entity=use,
-                    resource=UResource(name="door", instance="front_left", message="Door"))
-        uprotocol_uri = LongUriSerializer().serialize(uuri)
-        self.assertEqual("//vcu.my_car_vin/body.access//door.front_left#Door", uprotocol_uri)
-
-    def test_build_protocol_uri_for_source_part_of_rpc_request_where_source_is_local(self):
+        uuri = UUri(
+            authority=UAuthority(name="vcu.my_car_vin"),
+            entity=use,
+            resource=UResource(
+                name="door", instance="front_left", message="Door"
+            ),
+        )
+        uprotocol_uri = LongUriSerializer().serialize(uuri)
+        self.assertEqual(
+            "//vcu.my_car_vin/body.access//door.front_left#Door", uprotocol_uri
+        )
+
+    def test_build_protocol_uri_for_source_part_of_rpc_request_where_source_is_local(
+        self,
+    ):
         use = UEntity(name="petapp", version_major=1)
         resource = UResource(name="rpc", instance="response")
-        uprotocol_uri = LongUriSerializer().serialize(UUri(entity=use, resource=resource))
+        uprotocol_uri = LongUriSerializer().serialize(
+            UUri(entity=use, resource=resource)
+        )
         self.assertEqual("/petapp/1/rpc.response", uprotocol_uri)
 
-    def test_build_protocol_uri_for_source_part_of_rpc_request_where_source_is_remote(self):
+    def test_build_protocol_uri_for_source_part_of_rpc_request_where_source_is_remote(
+        self,
+    ):
         uAuthority = UAuthority(name="cloud.uprotocol.example.com")
         use = UEntity(name="petapp")
         resource = UResource(name="rpc", instance="response")
 
-        uprotocol_uri = LongUriSerializer().serialize(UUri(authority=uAuthority, entity=use, resource=resource))
-        self.assertEqual("//cloud.uprotocol.example.com/petapp//rpc.response", uprotocol_uri)
-
-    def test_build_protocol_uri_from_uri_parts_when_uri_has_remote_authority_service_and_version_with_resource(self):
+        uprotocol_uri = LongUriSerializer().serialize(
+            UUri(authority=uAuthority, entity=use, resource=resource)
+        )
+        self.assertEqual(
+            "//cloud.uprotocol.example.com/petapp//rpc.response", uprotocol_uri
+        )
+
+    def test_build_protocol_uri_from_uri_parts_when_uri_has_remote_authority_service_and_version_with_resource(
+        self,
+    ):
         u_authority = UAuthority(name="vcu.my_car_vin")
         use = UEntity(name="body.access", version_major=1)
         resource = UResource(name="door")
-        uprotocol_uri = LongUriSerializer().serialize(UUri(authority=u_authority, entity=use, resource=resource))
+        uprotocol_uri = LongUriSerializer().serialize(
+            UUri(authority=u_authority, entity=use, resource=resource)
+        )
         self.assertEqual("//vcu.my_car_vin/body.access/1/door", uprotocol_uri)
 
     def test_custom_scheme_no_scheme(self):
         u_authority = UAuthority(name="vcu.my_car_vin")
         use = UEntity(name="body.access", version_major=1)
         resource = UResource(name="door")
-        ucustom_uri = LongUriSerializer().serialize(UUri(authority=u_authority, entity=use, resource=resource))
+        ucustom_uri = LongUriSerializer().serialize(
+            UUri(authority=u_authority, entity=use, resource=resource)
+        )
         self.assertEqual("//vcu.my_car_vin/body.access/1/door", ucustom_uri)
 
     def test_parse_local_protocol_uri_with_custom_scheme(self):
         uri = "custom:/body.access//door.front_left#Door"
         uuri = LongUriSerializer().deserialize(uri)
         self.assertFalse(UriValidator.is_remote(uuri.authority))
         self.assertEqual("body.access", uuri.entity.name)
@@ -657,30 +803,10 @@
         self.assertEqual("body.access", uuri.entity.name)
         self.assertEqual(0, uuri.entity.version_major)
         self.assertEqual("door", uuri.resource.name)
         self.assertEqual("front_left", uuri.resource.instance)
         self.assertEqual("Door", uuri.resource.message)
         self.assertEqual(uri2, LongUriSerializer().serialize(uuri))
 
-    def test_deserialize_long_and_micro_passing_null(self):
-        uri = LongUriSerializer().build_resolved(None, None)
-        self.assertTrue(uri is not None)
-        self.assertEqual("", LongUriSerializer().serialize(uri))
-
-    def test_deserialize_long_and_micro_passing_null_long_uri_empty_byte_array(self):
-        uri = LongUriSerializer().build_resolved(None, bytearray())
-        self.assertTrue(uri is not None)
-        self.assertEqual("", LongUriSerializer().serialize(uri))
-
-    def test_deserialize_long_and_micro_passing_nullempty_long_uri_null_byte_array(self):
-        uri = LongUriSerializer().build_resolved("", None)
-        self.assertTrue(uri is not None)
-        self.assertEqual("", LongUriSerializer().serialize(uri))
-
-    def test_deserialize_long_and_micro_passing_empty_long_uri_empty_byte_array(self):
-        uri = LongUriSerializer().build_resolved("", bytearray())
-        self.assertTrue(uri is not None)
-        self.assertEqual("", LongUriSerializer().serialize(uri))
-
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `up_python-0.1.1.dev0/tests/test_uri/test_serializer/test_microuriserializer.py` & `up_python-0.1.2.dev0/tests/test_uri/test_serializer/test_microuriserializer.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,33 +1,7 @@
-# -------------------------------------------------------------------------
-#
-# Copyright (c) 2023 General Motors GTO LLC
-#
-# Licensed to the Apache Software Foundation (ASF) under one
-# or more contributor license agreements.  See the NOTICE file
-# distributed with this work for additional information
-# regarding copyright ownership.  The ASF licenses this file
-# to you under the Apache License, Version 2.0 (the
-# "License"); you may not use this file except in compliance
-# with the License.  You may obtain a copy of the License at
-#
-#   http://www.apache.org/licenses/LICENSE-2.0
-#
-# Unless required by applicable law or agreed to in writing,
-# software distributed under the License is distributed on an
-# "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
-# KIND, either express or implied.  See the License for the
-# specific language governing permissions and limitations
-# under the License.
-# SPDX-FileType: SOURCE
-# SPDX-FileCopyrightText: 2023 General Motors GTO LLC
-# SPDX-License-Identifier: Apache-2.0
-#
-# -------------------------------------------------------------------------
-
 import socket
 import unittest
 
 from uprotocol.proto.uri_pb2 import UEntity, UUri, UAuthority, UResource
 from uprotocol.uri.factory.uresource_builder import UResourceBuilder
 from uprotocol.uri.serializer.microuriserializer import MicroUriSerializer
 from uprotocol.uri.validator.urivalidator import UriValidator
@@ -44,17 +18,19 @@
     def test_null(self):
         bytes_uuri = MicroUriSerializer().serialize(None)
         self.assertEqual(len(bytes_uuri), 0)
         uri2 = MicroUriSerializer().deserialize(None)
         self.assertTrue(UriValidator.is_empty(uri2))
 
     def test_serialize_uri(self):
-        uri = UUri(entity=UEntity(id=29999, version_major=254), resource=UResource(id=19999))
+        uri = UUri(entity=UEntity(id=29999, version_major=254), resource=UResourceBuilder.from_id(19999))
         bytes_uuri = MicroUriSerializer().serialize(uri)
         uri2 = MicroUriSerializer().deserialize(bytes_uuri)
+        self.assertTrue(UriValidator.is_micro_form(uri))
+        self.assertTrue(len(bytes_uuri) > 0)
         self.assertEqual(uri, uri2)
 
     def test_serialize_remote_uri_without_address(self):
         uri = UUri(authority=UAuthority(name="vcu.vin"), entity=UEntity(id=29999, version_major=254),
                    resource=UResourceBuilder.for_rpc_response())
         bytes_uuri = MicroUriSerializer().serialize(uri)
         self.assertTrue(len(bytes_uuri) == 0)
@@ -98,57 +74,63 @@
         self.assertTrue(UriValidator.is_empty(uuri))
 
         badMicroUUri = bytes([0x1, 0x2, 0x0, 0x0, 0x0, 0x0, 0x0, 0x0, 0x0, 0x0])
         uuri = MicroUriSerializer().deserialize(badMicroUUri)
         self.assertTrue(UriValidator.is_empty(uuri))
 
     def test_serialize_good_ipv4_based_authority(self):
-        uri = UUri(authority=UAuthority(ip=bytes(socket.inet_pton(socket.AF_INET, "10.0.3.3"))),
-                   entity=UEntity(id=29999, version_major=254), resource=UResourceBuilder.for_rpc_request_with_id(99))
+        uri = UUri(authority=UAuthority(ip=socket.inet_pton(socket.AF_INET, "10.0.3.3")),
+                   entity=UEntity(id=29999, version_major=254), resource=UResourceBuilder.for_rpc_request(99))
         bytes_uuri = MicroUriSerializer().serialize(uri)
         uri2 = MicroUriSerializer().deserialize(bytes_uuri)
         self.assertTrue(len(bytes_uuri) > 0)
         self.assertTrue(UriValidator.is_micro_form(uri))
         self.assertTrue(UriValidator.is_micro_form(uri2))
         self.assertEqual(str(uri), str(uri2))
         self.assertTrue(uri == uri2)
 
+    def test_serialize_bad_authority(self):
+        uri = UUri(authority=UAuthority(ip=b"123456789"),
+                   entity=UEntity(id=29999, version_major=254), resource=UResourceBuilder.for_rpc_request(99))
+        bytes_uuri = MicroUriSerializer().serialize(uri)
+        self.assertEqual(bytes_uuri, bytearray())
+
     def test_serialize_good_ipv6_based_authority(self):
         uri = UUri(authority=UAuthority(
-            ip=bytes(socket.inet_pton(socket.AF_INET6, "2001:0db8:85a3:0000:0000:8a2e:0370:7334"))),
-            entity=UEntity(id=29999, version_major=254), resource=UResource(id=19999))
+            ip=socket.inet_pton(socket.AF_INET6, "2001:0db8:85a3:0000:0000:8a2e:0370:7334")),
+            entity=UEntity(id=29999, version_major=254), resource=UResource(id=19999, name="rpc"))
         bytes_uuri = MicroUriSerializer().serialize(uri)
         uri2 = MicroUriSerializer().deserialize(bytes_uuri)
         self.assertTrue(UriValidator.is_micro_form(uri))
         self.assertTrue(len(bytes_uuri) > 0)
         self.assertTrue(uri == uri2)
 
     def test_serialize_id_based_authority(self):
         size = 13
         byteArray = bytearray(i for i in range(size))
         uri = UUri(authority=UAuthority(id=bytes(byteArray)), entity=UEntity(id=29999, version_major=254),
-                   resource=UResource(id=19999))
+                   resource=UResource(id=19999, name="rpc"))
         bytes_uuri = MicroUriSerializer().serialize(uri)
         uri2 = MicroUriSerializer().deserialize(bytes_uuri)
         self.assertTrue(UriValidator.is_micro_form(uri))
         self.assertTrue(len(bytes_uuri) > 0)
         self.assertTrue(uri == uri2)
 
     def test_serialize_bad_length_ip_based_authority(self):
         byteArray = bytes([127, 1, 23, 123, 12, 6])
-        uri = UUri(authority=UAuthority(ip=bytes(byteArray)), entity=UEntity(id=29999, version_major=254),
+        uri = UUri(authority=UAuthority(ip=byteArray), entity=UEntity(id=29999, version_major=254),
                    resource=UResource(id=19999))
         bytes_uuri = MicroUriSerializer().serialize(uri)
         self.assertTrue(len(bytes_uuri) == 0)
 
     def test_serialize_id_size_255_based_authority(self):
         size = 129
         byteArray = bytes(i for i in range(size))
-        uri = UUri(authority=UAuthority(id=bytes(byteArray)), entity=UEntity(id=29999, version_major=254),
-                   resource=UResourceBuilder.for_rpc_request_with_id(99))
+        uri = UUri(authority=UAuthority(id=byteArray), entity=UEntity(id=29999, version_major=254),
+                   resource=UResourceBuilder.for_rpc_request(99))
         bytes_uuri = MicroUriSerializer().serialize(uri)
         self.assertEqual(len(bytes_uuri), 9 + size)
         uri2 = MicroUriSerializer().deserialize(bytes_uuri)
         self.assertTrue(UriValidator.is_micro_form(uri))
         self.assertTrue(uri == uri2)
```

### Comparing `up_python-0.1.1.dev0/tests/test_uri/test_validator/test_urivalidator.py` & `up_python-0.1.2.dev0/tests/test_uri/test_validator/test_urivalidator.py`

 * *Files 17% similar despite different names*

```diff
@@ -21,21 +21,21 @@
 # SPDX-FileType: SOURCE
 # SPDX-FileCopyrightText: 2023 General Motors GTO LLC
 # SPDX-License-Identifier: Apache-2.0
 #
 # -------------------------------------------------------------------------
 
 
-
 import json
 import os
 import unittest
 
 from uprotocol.uri.serializer.longuriserializer import LongUriSerializer
 from uprotocol.uri.validator.urivalidator import UriValidator
+from uprotocol.uri.factory.uresource_builder import UResourceBuilder
 from uprotocol.validation.validationresult import ValidationResult
 from uprotocol.proto.uri_pb2 import UUri, UEntity, UResource, UAuthority
 
 
 class TestUriValidator(unittest.TestCase):
 
     def test_validate_blank_uri(self):
@@ -51,15 +51,14 @@
         self.assertEqual("Uri is empty.", status.get_message())
 
     def test_validate_uri_with_getEntity(self):
         uri = LongUriSerializer().deserialize("/neelam")
         status = UriValidator.validate(uri)
         self.assertTrue(ValidationResult.success().__eq__(status))
 
-
     def test_validate_with_malformed_uri(self):
         uri = LongUriSerializer().deserialize("neelam")
         status = UriValidator.validate(uri)
         self.assertTrue(UriValidator.is_empty(uri))
         self.assertEqual("Uri is empty.", status.get_message())
 
     def test_validate_with_blank_uentity_name_uri(self):
@@ -85,15 +84,14 @@
         self.assertEqual("Uri is empty.", status.get_message())
 
     def test_validateRpcResponse_with_valid_uri(self):
         uri = LongUriSerializer().deserialize("/neelam//rpc.response")
         status = UriValidator.validate_rpc_response(uri)
         self.assertTrue(ValidationResult.success().__eq__(status))
 
-
     def test_validateRpcResponse_with_malformed_uri(self):
         uri = LongUriSerializer().deserialize("neelam")
         status = UriValidator.validate_rpc_response(uri)
         self.assertTrue(UriValidator.is_empty(uri))
         self.assertEqual("Uri is empty.", status.get_message())
 
     def test_validateRpcResponse_with_rpc_type(self):
@@ -161,139 +159,200 @@
     def test_topic_uri_invalid_when_uri_is_missing_use_name_local(self):
         uri = "//VCU.myvin//1"
         status = UriValidator.validate(LongUriSerializer().deserialize(uri))
         self.assertTrue(status.is_failure())
 
     def test_rpc_topic_uri_with_version_when_it_is_valid_remote(self):
         uri = "//bo.cloud/petapp/1/rpc.response"
-        status = UriValidator.validate_rpc_method(LongUriSerializer().deserialize(uri))
+        status = UriValidator.validate_rpc_method(
+            LongUriSerializer().deserialize(uri)
+        )
         self.assertTrue(status.is_success)
 
     def test_rpc_topic_uri_no_version_when_it_is_valid_remote(self):
         uri = "//bo.cloud/petapp//rpc.response"
-        status = UriValidator.validate_rpc_method(LongUriSerializer().deserialize(uri))
+        status = UriValidator.validate_rpc_method(
+            LongUriSerializer().deserialize(uri)
+        )
         self.assertTrue(status.is_success)
 
     def test_rpc_topic_uri_with_version_when_it_is_valid_local(self):
         uri = "/petapp/1/rpc.response"
-        status = UriValidator.validate_rpc_method(LongUriSerializer().deserialize(uri))
+        status = UriValidator.validate_rpc_method(
+            LongUriSerializer().deserialize(uri)
+        )
         self.assertTrue(status.is_success)
 
     def test_rpc_topic_uri_no_version_when_it_is_valid_local(self):
         uri = "/petapp//rpc.response"
-        status = UriValidator.validate_rpc_method(LongUriSerializer().deserialize(uri))
+        status = UriValidator.validate_rpc_method(
+            LongUriSerializer().deserialize(uri)
+        )
         self.assertTrue(status.is_success)
 
     def test_rpc_topic_uri_invalid_when_uri_has_schema_only(self):
         uri = ":"
-        status = UriValidator.validate_rpc_method(LongUriSerializer().deserialize(uri))
+        status = UriValidator.validate_rpc_method(
+            LongUriSerializer().deserialize(uri)
+        )
         self.assertTrue(status.is_failure())
 
     def test_rpc_topic_uri_with_version_when_it_is_not_valid_missing_rpc_response_local(self):
         uri = "/petapp/1/dog"
         status = UriValidator.validate_rpc_method(LongUriSerializer().deserialize(uri))
         self.assertTrue(status.is_failure())
 
-    def test_rpc_topic_uri_with_version_when_it_is_not_valid_missing_rpc_response_remote(self):
+    def test_rpc_topic_uri_with_version_when_it_is_not_valid_missing_rpc_response_remote(
+        self,
+    ):
         uri = "//petapp/1/dog"
-        status = UriValidator.validate_rpc_method(LongUriSerializer().deserialize(uri))
+        status = UriValidator.validate_rpc_method(
+            LongUriSerializer().deserialize(uri)
+        )
         self.assertTrue(status.is_failure())
 
     def test_rpc_topic_uri_invalid_when_uri_is_remote_no_authority(self):
         uri = "//"
-        status = UriValidator.validate_rpc_method(LongUriSerializer().deserialize(uri))
+        status = UriValidator.validate_rpc_method(
+            LongUriSerializer().deserialize(uri)
+        )
         self.assertTrue(status.is_failure())
 
-    def test_rpc_topic_uri_invalid_when_uri_is_remote_no_authority_with_use(self):
+    def test_rpc_topic_uri_invalid_when_uri_is_remote_no_authority_with_use(
+        self,
+    ):
         uri = "///body.access/1"
-        status = UriValidator.validate_rpc_method(LongUriSerializer().deserialize(uri))
+        status = UriValidator.validate_rpc_method(
+            LongUriSerializer().deserialize(uri)
+        )
         self.assertTrue(status.is_failure())
 
     def test_rpc_topic_uri_invalid_when_uri_is_missing_use(self):
         uri = "//VCU.myvin"
-        status = UriValidator.validate_rpc_method(LongUriSerializer().deserialize(uri))
+        status = UriValidator.validate_rpc_method(
+            LongUriSerializer().deserialize(uri)
+        )
         self.assertTrue(status.is_failure())
 
     def test_rpc_topic_uri_invalid_when_uri_is_missing_use_name_remote(self):
         uri = "/1"
-        status = UriValidator.validate_rpc_method(LongUriSerializer().deserialize(uri))
+        status = UriValidator.validate_rpc_method(
+            LongUriSerializer().deserialize(uri)
+        )
         self.assertTrue(status.is_failure())
 
     def test_rpc_topic_uri_invalid_when_uri_is_missing_use_name_local(self):
         uri = "//VCU.myvin//1"
-        status = UriValidator.validate_rpc_method(LongUriSerializer().deserialize(uri))
+        status = UriValidator.validate_rpc_method(
+            LongUriSerializer().deserialize(uri)
+        )
         self.assertTrue(status.is_failure())
 
     def test_rpc_method_uri_with_version_when_it_is_valid_remote(self):
         uri = "//VCU.myvin/body.access/1/rpc.UpdateDoor"
-        status = UriValidator.validate_rpc_method(LongUriSerializer().deserialize(uri))
+        status = UriValidator.validate_rpc_method(
+            LongUriSerializer().deserialize(uri)
+        )
         self.assertTrue(status.is_success)
 
     def test_rpc_method_uri_no_version_when_it_is_valid_remote(self):
         uri = "//VCU.myvin/body.access//rpc.UpdateDoor"
-        status = UriValidator.validate_rpc_method(LongUriSerializer().deserialize(uri))
+        status = UriValidator.validate_rpc_method(
+            LongUriSerializer().deserialize(uri)
+        )
         self.assertTrue(status.is_success)
 
     def test_rpc_method_uri_with_version_when_it_is_valid_local(self):
         uri = "/body.access/1/rpc.UpdateDoor"
-        status = UriValidator.validate_rpc_method(LongUriSerializer().deserialize(uri))
+        status = UriValidator.validate_rpc_method(
+            LongUriSerializer().deserialize(uri)
+        )
         self.assertTrue(status.is_success)
 
     def test_rpc_method_uri_no_version_when_it_is_valid_local(self):
         uri = "/body.access//rpc.UpdateDoor"
-        status = UriValidator.validate_rpc_method(LongUriSerializer().deserialize(uri))
+        status = UriValidator.validate_rpc_method(
+            LongUriSerializer().deserialize(uri)
+        )
         self.assertTrue(status.is_success)
 
     def test_rpc_method_uri_invalid_when_uri_has_schema_only(self):
         uri = ":"
-        status = UriValidator.validate_rpc_method(LongUriSerializer().deserialize(uri))
+        status = UriValidator.validate_rpc_method(
+            LongUriSerializer().deserialize(uri)
+        )
         self.assertTrue(status.is_failure())
 
-    def test_rpc_method_uri_with_version_when_it_is_not_valid_not_rpc_method_local(self):
+    def test_rpc_method_uri_with_version_when_it_is_not_valid_not_rpc_method_local(
+        self,
+    ):
         uri = "/body.access//UpdateDoor"
-        status = UriValidator.validate_rpc_method(LongUriSerializer().deserialize(uri))
+        status = UriValidator.validate_rpc_method(
+            LongUriSerializer().deserialize(uri)
+        )
         self.assertTrue(status.is_failure())
 
-    def test_rpc_method_uri_with_version_when_it_is_not_valid_not_rpc_method_remote(self):
+    def test_rpc_method_uri_with_version_when_it_is_not_valid_not_rpc_method_remote(
+        self,
+    ):
         uri = "//body.access/1/UpdateDoor"
-        status = UriValidator.validate_rpc_method(LongUriSerializer().deserialize(uri))
+        status = UriValidator.validate_rpc_method(
+            LongUriSerializer().deserialize(uri)
+        )
         self.assertTrue(status.is_failure())
 
     def test_rpc_method_uri_invalid_when_uri_is_remote_no_authority(self):
         uri = "//"
-        status = UriValidator.validate_rpc_method(LongUriSerializer().deserialize(uri))
+        status = UriValidator.validate_rpc_method(
+            LongUriSerializer().deserialize(uri)
+        )
         self.assertTrue(status.is_failure())
 
-    def test_rpc_method_uri_invalid_when_uri_is_remote_no_authority_with_use(self):
+    def test_rpc_method_uri_invalid_when_uri_is_remote_no_authority_with_use(
+        self,
+    ):
         uri = "///body.access/1/rpc.UpdateDoor"
         uuri = LongUriSerializer().deserialize(uri)
         status = UriValidator.validate_rpc_method(uuri)
         self.assertEqual("", str(uuri))
         self.assertTrue(status.is_failure())
 
-    def test_rpc_method_uri_invalid_when_uri_is_remote_missing_authority_remotecase(self):
-        uuri = UUri(entity=UEntity(name="body.access"),resource=UResource(name="rpc",instance="UpdateDoor"),authority=
-            UAuthority())
+    def test_rpc_method_uri_invalid_when_uri_is_remote_missing_authority_remotecase(
+        self,
+    ):
+        uuri = UUri(
+            entity=UEntity(name="body.access"),
+            resource=UResource(name="rpc", instance="UpdateDoor"),
+            authority=UAuthority(),
+        )
         status = UriValidator.validate_rpc_method(uuri)
         self.assertTrue(status.is_failure())
-        self.assertEqual("Uri is remote missing uAuthority.", status.get_message())
+        self.assertEqual(
+            "Uri is remote missing uAuthority.", status.get_message()
+        )
 
     def test_rpc_method_uri_invalid_when_uri_is_missing_use(self):
         uri = "//VCU.myvin"
-        status = UriValidator.validate_rpc_method(LongUriSerializer().deserialize(uri))
+        status = UriValidator.validate_rpc_method(
+            LongUriSerializer().deserialize(uri)
+        )
         self.assertTrue(status.is_failure())
 
     def test_rpc_method_uri_invalid_when_uri_is_missing_use_name_local(self):
         uri = "/1/rpc.UpdateDoor"
-        status = UriValidator.validate_rpc_method(LongUriSerializer().deserialize(uri))
+        status = UriValidator.validate_rpc_method(
+            LongUriSerializer().deserialize(uri)
+        )
         self.assertTrue(status.is_failure())
 
     def test_rpc_method_uri_invalid_when_uri_is_missing_use_name_remote(self):
         uri = "//VCU.myvin//1/rpc.UpdateDoor"
-        status = UriValidator.validate_rpc_method(LongUriSerializer().deserialize(uri))
+        status = UriValidator.validate_rpc_method(
+            LongUriSerializer().deserialize(uri)
+        )
         self.assertTrue(status.is_failure())
 
     def test_all_valid_uris(self):
         # Access the "validUris" array
         valid_uris = self.get_json_object()["validUris"]
         for valid_uri in valid_uris:
             uuri = LongUriSerializer().deserialize(valid_uri)
@@ -303,58 +362,178 @@
     def test_all_invalid_uris(self):
         # Access the "invalidUris" array
         invalid_uris = self.get_json_object()["invalidUris"]
         for invalid_uri in invalid_uris:
             uuri = LongUriSerializer().deserialize(invalid_uri["uri"])
             status = UriValidator.validate(uuri)
             self.assertTrue(status.is_failure())
-            self.assertEqual(status.get_message(), invalid_uri["status_message"])
+            self.assertEqual(
+                status.get_message(), invalid_uri["status_message"]
+            )
 
     def test_all_valid_rpc_uris(self):
         valid_rpc_uris = self.get_json_object()["validRpcUris"]
         for valid_rpc_uri in valid_rpc_uris:
             uuri = LongUriSerializer().deserialize(valid_rpc_uri)
             status = UriValidator.validate_rpc_method(uuri)
             self.assertTrue(status.is_success)
 
     def test_all_invalid_rpc_uris(self):
         invalid_rpc_uris = self.get_json_object()["invalidRpcUris"]
         for invalid_rpc_uri in invalid_rpc_uris:
             uuri = LongUriSerializer().deserialize(invalid_rpc_uri["uri"])
             status = UriValidator.validate_rpc_method(uuri)
             self.assertTrue(status.is_failure())
-            self.assertEqual(status.get_message(), invalid_rpc_uri["status_message"])
+            self.assertEqual(
+                status.get_message(), invalid_rpc_uri["status_message"]
+            )
 
     def test_all_valid_rpc_response_uris(self):
-        valid_rpc_response_uris = self.get_json_object()["validRpcResponseUris"]
+        valid_rpc_response_uris = self.get_json_object()[
+            "validRpcResponseUris"
+        ]
         for valid_rpc_response_uri in valid_rpc_response_uris:
             uuri = LongUriSerializer().deserialize(valid_rpc_response_uri)
             status = UriValidator.validate_rpc_response(uuri)
             self.assertTrue(UriValidator.is_rpc_response(uuri))
             self.assertTrue(status.is_success)
 
     def test_valid_rpc_response_uri(self):
-        uuri = UUri(entity=UEntity(name="neelam"),resource=UResource(name="rpc",id=0,instance="response"))
+        uuri = UUri(
+            entity=UEntity(name="neelam"),
+            resource=UResource(name="rpc", id=0, instance="response"),
+        )
         status = UriValidator.validate_rpc_response(uuri)
         self.assertTrue(UriValidator.is_rpc_response(uuri))
         self.assertTrue(status.is_success)
 
     def test_all_invalid_rpc_response_uris(self):
-        invalid_rpc_response_uris = self.get_json_object()["invalidRpcResponseUris"]
+        invalid_rpc_response_uris = self.get_json_object()[
+            "invalidRpcResponseUris"
+        ]
         for invalid_rpc_response_uri in invalid_rpc_response_uris:
             uuri = LongUriSerializer().deserialize(invalid_rpc_response_uri)
             status = UriValidator.validate_rpc_response(uuri)
             self.assertTrue(status.is_failure())
 
+    def test_invalid_rpc_method_uri(self):
+        uuri: UUri = UUri(
+            entity=UEntity(name="hello.world"),
+            resource=UResource(name="testrpc", instance="SayHello"),
+        )
+        status = UriValidator.validate_rpc_method(uuri)
+        self.assertFalse(UriValidator.is_rpc_method(uuri))
+        self.assertFalse(status.is_success())
+
+    def test_invalid_rpc_response_uri(self):
+        uuri: UUri = UUri(
+            entity=UEntity(name="hartley"),
+            resource=UResource(name="rpc", id=19999),
+        )
+        status = UriValidator.validate_rpc_response(uuri)
+        self.assertFalse(UriValidator.is_rpc_response(uuri))
+        self.assertFalse(status.is_success())
+
+        uuri: UUri = UUri(
+            entity=UEntity(name="hartley"),
+            resource=UResource(name="testrpc", instance="response"),
+        )
+        status = UriValidator.validate_rpc_response(uuri)
+        self.assertFalse(UriValidator.is_rpc_response(uuri))
+        self.assertFalse(status.is_success())
+
+        uuri: UUri = UUri(
+            entity=UEntity(name="hartley"),
+            resource=UResource(name="testrpc", instance="response"),
+        )
+        status = UriValidator.validate_rpc_response(uuri)
+        self.assertFalse(UriValidator.is_rpc_response(uuri))
+        self.assertFalse(status.is_success())
+
     @staticmethod
     def get_json_object():
         current_directory = os.getcwd()
-        json_file_path = os.path.join(current_directory,"tests","test_uri","test_validator", "uris.json")
+        json_file_path = os.path.join(
+            current_directory,
+            "tests",
+            "test_uri",
+            "test_validator",
+            "uris.json",
+        )
 
-        with open(json_file_path, 'r') as json_file:
+        with open(json_file_path, "r") as json_file:
             json_data = json.load(json_file)
 
         return json_data
 
+    def test_is_rpc_method_with_uresource_and_no_uauthority(self):
+        self.assertFalse(UriValidator.is_rpc_method(UUri()))
+
+        uri = UUri(
+            entity=UEntity(name="hartley"),
+            resource=UResourceBuilder.from_id(0x8000),
+        )
+        self.assertFalse(UriValidator.is_rpc_method(uri))
+
+    def test_is_rpc_method_passing_null_for_uri(self):
+        self.assertFalse(UriValidator.is_rpc_method(None))
+
+    def test_is_rpc_method_passing_null_for_resource(self):
+        self.assertFalse(UriValidator.is_rpc_method(None))
+
+    def test_is_rpc_method_for_uresource_without_an_instance(self):
+        resource = UResource(name="rpc")
+        self.assertFalse(UriValidator.is_rpc_method(resource))
+
+    def test_is_rpc_method_for_uresource_with_an_empty_instance(self):
+        resource = UResource(name="rpc", instance="")
+        self.assertFalse(UriValidator.is_rpc_method(resource))
+
+    def test_is_rpc_method_for_uresource_with_id_that_is_less_than_min_topic(
+        self,
+    ):
+        resource = UResource(name="rpc", id=0)
+        self.assertTrue(UriValidator.is_rpc_method(resource))
+
+    def test_is_rpc_method_for_uresource_with_id_that_is_greater_than_min_topic(
+        self,
+    ):
+        resource = UResource(name="rpc", id=0x8000)
+        self.assertFalse(UriValidator.is_rpc_method(resource))
+
+    def test_is_empty_with_null_uri(self):
+        self.assertTrue(UriValidator.is_empty(None))
+
+    def test_is_resolved_when_uri_is_long_form_only(self):
+        uri = UUri(
+            entity=UEntity(name="hartley", version_major=23),
+            resource=UResource(name="rpc", instance="echo"),
+        )
+        self.assertFalse(UriValidator.is_resolved(uri))
+
+    def test_is_local_when_authority_is_null(self):
+        self.assertFalse(UriValidator.is_local(None))
+
+    def test_is_remote_when_authority_is_null(self):
+        self.assertFalse(UriValidator.is_remote(None))
+
+    # def test_is_remote_when_authority_does_not_have_a_name_but_does_have_a_number_set(self):
+    #     authority = UAuthority(id=b"hello Jello")
+    #     self.assertTrue(UriValidator.is_remote(authority))
+    #     self.assertFalse(authority.name is not None)
+    #     self.assertEqual(authority.number_case(), UAuthority.NumberCase.ID)
+
+    # def test_is_remote_when_authority_has_name_and_number_set(self):
+    #     authority = UAuthority(name="vcu.veh.gm.com", id=b"hello Jello")
+    #     self.assertTrue(UriValidator.is_remote(authority))
+    #     self.assertTrue(authority.name is not None)
+    #     self.assertEqual(authority.number_case(), UAuthority.NumberCase.ID)
+
+    # def test_is_remote_when_authority_has_name_and_number_is_not_set(self):
+    #     authority = UAuthority(name="vcu.veh.gm.com")
+    #     self.assertTrue(UriValidator.is_remote(authority))
+    #     self.assertTrue(authority.name is not None)
+    #     self.assertEqual(authority.number_case(), UAuthority.NumberCase.NUMBER_NOT_SET)
+
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
```

### Comparing `up_python-0.1.1.dev0/tests/test_uri/test_validator/uris.json` & `up_python-0.1.2.dev0/tests/test_uri/test_validator/uris.json`

 * *Files identical despite different names*

### Comparing `up_python-0.1.1.dev0/tests/test_uuid/test_factory/test_uuidfactory.py` & `up_python-0.1.2.dev0/tests/test_uuid/test_factory/test_uuidfactory.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -------------------------------------------------------------------------
 #
-# Copyright (c) 2023 General Motors GTO LLC
+# Copyright (c) 2024 General Motors GTO LLC
 #
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
@@ -15,44 +15,43 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 # SPDX-FileType: SOURCE
-# SPDX-FileCopyrightText: 2023 General Motors GTO LLC
+# SPDX-FileCopyrightText: 2024 General Motors GTO LLC
 # SPDX-License-Identifier: Apache-2.0
 #
 # -------------------------------------------------------------------------
 
 
-from datetime import datetime, timedelta
+from datetime import datetime, timedelta, timezone
 import unittest
 from uprotocol.uuid.serializer.longuuidserializer import LongUuidSerializer
 from uprotocol.uuid.serializer.microuuidserializer import MicroUuidSerializer
-from uprotocol.uuid.factory.uuidfactory import UUIDFactory, Factories
+from uprotocol.uuid.factory.uuidfactory import Factories
 from uprotocol.uuid.factory.uuidutils import UUIDUtils, Version
 from uprotocol.proto.uuid_pb2 import UUID
 
 
-
 class TestUUIDFactory(unittest.TestCase):
 
     def test_uuidv8_creation(self):
         now = datetime.now()
         uuid = Factories.UPROTOCOL.create(now)
-        version = UUIDUtils.getVersion(uuid)
-        time = UUIDUtils.getTime(uuid)
+        version = UUIDUtils.get_version(uuid)
+        time = UUIDUtils.get_time(uuid)
         bytes_data = MicroUuidSerializer.instance().serialize(uuid)
         uuid_string = LongUuidSerializer.instance().serialize(uuid)
 
         self.assertIsNotNone(uuid)
-        self.assertTrue(UUIDUtils.isUProtocol(uuid))
-        self.assertTrue(UUIDUtils.isuuid(uuid))
-        self.assertFalse(UUIDUtils.isUuidv6(uuid))
+        self.assertTrue(UUIDUtils.is_uprotocol(uuid))
+        self.assertTrue(UUIDUtils.is_uuid(uuid))
+        self.assertFalse(UUIDUtils.is_uuidv6(uuid))
         self.assertTrue(version)
         self.assertTrue(time)
         self.assertEqual(time, int(now.timestamp() * 1000))
 
         self.assertGreater(len(bytes_data), 0)
         self.assertFalse(uuid_string.isspace())
 
@@ -62,23 +61,23 @@
         self.assertNotEqual(uuid1, UUID())
         self.assertNotEqual(uuid2, UUID())
         self.assertEqual(uuid, uuid1)
         self.assertEqual(uuid, uuid2)
 
     def test_uuidv8_creation_with_null_instant(self):
         uuid = Factories.UPROTOCOL.create(None)
-        version = UUIDUtils.getVersion(uuid)
-        time = UUIDUtils.getTime(uuid)
+        version = UUIDUtils.get_version(uuid)
+        time = UUIDUtils.get_time(uuid)
         bytes_data = MicroUuidSerializer.instance().serialize(uuid)
         uuid_string = LongUuidSerializer.instance().serialize(uuid)
 
         self.assertIsNotNone(uuid)
-        self.assertTrue(UUIDUtils.isUProtocol(uuid))
-        self.assertTrue(UUIDUtils.isuuid(uuid))
-        self.assertFalse(UUIDUtils.isUuidv6(uuid))
+        self.assertTrue(UUIDUtils.is_uprotocol(uuid))
+        self.assertTrue(UUIDUtils.is_uuid(uuid))
+        self.assertFalse(UUIDUtils.is_uuidv6(uuid))
         self.assertTrue(version)
         self.assertTrue(time)
         self.assertGreater(len(bytes_data), 0)
         self.assertFalse(uuid_string.isspace())
 
         uuid1 = MicroUuidSerializer.instance().deserialize(bytes_data)
         uuid2 = LongUuidSerializer.instance().deserialize(uuid_string)
@@ -92,31 +91,34 @@
         uuid_list = []
         max_count = 4095
 
         now = datetime.now()
         for i in range(max_count * 2):
             uuid_list.append(Factories.UPROTOCOL.create(now))
 
-            self.assertEqual(UUIDUtils.getTime(uuid_list[0]), UUIDUtils.getTime(uuid_list[i]))
+            self.assertEqual(
+                UUIDUtils.get_time(uuid_list[0]),
+                UUIDUtils.get_time(uuid_list[i]),
+            )
             self.assertEqual(uuid_list[0].lsb, uuid_list[i].lsb)
             if i > max_count:
                 self.assertEqual(uuid_list[max_count].msb, uuid_list[i].msb)
 
     def test_uuidv6_creation_with_instant(self):
         now = datetime.now()
         uuid = Factories.UUIDV6.create(now)
-        version = UUIDUtils.getVersion(uuid)
+        version = UUIDUtils.get_version(uuid)
         # time = UUIDUtils.getTime(uuid)
         bytes_data = MicroUuidSerializer.instance().serialize(uuid)
         uuid_string = LongUuidSerializer.instance().serialize(uuid)
 
         self.assertIsNotNone(uuid)
-        self.assertTrue(UUIDUtils.isUuidv6(uuid))
-        self.assertTrue(UUIDUtils.isuuid(uuid))
-        self.assertFalse(UUIDUtils.isUProtocol(uuid))
+        self.assertTrue(UUIDUtils.is_uuidv6(uuid))
+        self.assertTrue(UUIDUtils.is_uuid(uuid))
+        self.assertFalse(UUIDUtils.is_uprotocol(uuid))
         self.assertTrue(version)
         # self.assertTrue(time)
         # self.assertEqual(time, int(17007094616498160 * 1000))
         self.assertGreater(len(bytes_data), 0)
         self.assertFalse(uuid_string.isspace())
 
         uuid1 = MicroUuidSerializer.instance().deserialize(bytes_data)
@@ -125,47 +127,49 @@
         self.assertNotEqual(uuid1, UUID())
         self.assertNotEqual(uuid2, UUID())
         self.assertEqual(uuid, uuid1)
         self.assertEqual(uuid, uuid2)
 
     def test_uuidv6_creation_with_null_instant(self):
         uuid = Factories.UUIDV6.create(None)
-        version = UUIDUtils.getVersion(uuid)
-        time = UUIDUtils.getTime(uuid)
+        version = UUIDUtils.get_version(uuid)
+        time = UUIDUtils.get_time(uuid)
         bytes_data = MicroUuidSerializer.instance().serialize(uuid)
         uuid_string = LongUuidSerializer.instance().serialize(uuid)
 
         self.assertIsNotNone(uuid)
-        self.assertTrue(UUIDUtils.isUuidv6(uuid))
-        self.assertFalse(UUIDUtils.isUProtocol(uuid))
-        self.assertTrue(UUIDUtils.isuuid(uuid))
+        self.assertTrue(UUIDUtils.is_uuidv6(uuid))
+        self.assertFalse(UUIDUtils.is_uprotocol(uuid))
+        self.assertTrue(UUIDUtils.is_uuid(uuid))
         self.assertTrue(version)
         self.assertTrue(time)
         self.assertGreater(len(bytes_data), 0)
         self.assertFalse(uuid_string.isspace())
 
         uuid1 = MicroUuidSerializer.instance().deserialize(bytes_data)
         uuid2 = LongUuidSerializer.instance().deserialize(uuid_string)
 
         self.assertNotEqual(uuid1, UUID())
         self.assertNotEqual(uuid2, UUID())
         self.assertEqual(uuid, uuid1)
         self.assertEqual(uuid, uuid2)
 
     def test_UUIDUtils_for_random_uuid(self):
-        uuid = LongUuidSerializer.instance().deserialize("195f9bd1-526d-4c28-91b1-ff34c8e3632d")
-        version = UUIDUtils.getVersion(uuid)
-        time = UUIDUtils.getTime(uuid)
+        uuid = LongUuidSerializer.instance().deserialize(
+            "195f9bd1-526d-4c28-91b1-ff34c8e3632d"
+        )
+        version = UUIDUtils.get_version(uuid)
+        time = UUIDUtils.get_time(uuid)
         bytes_data = MicroUuidSerializer.instance().serialize(uuid)
         uuid_string = LongUuidSerializer.instance().serialize(uuid)
 
         self.assertIsNotNone(uuid)
-        self.assertFalse(UUIDUtils.isUuidv6(uuid))
-        self.assertFalse(UUIDUtils.isUProtocol(uuid))
-        self.assertFalse(UUIDUtils.isuuid(uuid))
+        self.assertFalse(UUIDUtils.is_uuidv6(uuid))
+        self.assertFalse(UUIDUtils.is_uprotocol(uuid))
+        self.assertFalse(UUIDUtils.is_uuid(uuid))
         self.assertTrue(version)
         self.assertFalse(time)
         self.assertGreater(len(bytes_data), 0)
         self.assertFalse(uuid_string.isspace())
 
         uuid1 = MicroUuidSerializer.instance().deserialize(bytes_data)
         uuid2 = LongUuidSerializer.instance().deserialize(uuid_string)
@@ -173,112 +177,116 @@
         self.assertNotEqual(uuid1, UUID())
         self.assertNotEqual(uuid2, UUID())
         self.assertEqual(uuid, uuid1)
         self.assertEqual(uuid, uuid2)
 
     def test_UUIDUtils_for_empty_uuid(self):
         uuid = UUID()
-        version = UUIDUtils.getVersion(uuid)
-        time = UUIDUtils.getTime(uuid)
+        version = UUIDUtils.get_version(uuid)
+        time = UUIDUtils.get_time(uuid)
         bytes_data = MicroUuidSerializer.instance().serialize(uuid)
         uuid_string = LongUuidSerializer.instance().serialize(uuid)
 
         self.assertIsNotNone(uuid)
-        self.assertFalse(UUIDUtils.isUuidv6(uuid))
-        self.assertFalse(UUIDUtils.isUProtocol(uuid))
+        self.assertFalse(UUIDUtils.is_uuidv6(uuid))
+        self.assertFalse(UUIDUtils.is_uprotocol(uuid))
         self.assertTrue(version)
         self.assertEqual(version, Version.VERSION_UNKNOWN)
         self.assertFalse(time)
         self.assertGreater(len(bytes_data), 0)
         self.assertFalse(uuid_string.isspace())
-        self.assertFalse(UUIDUtils.isUuidv6(None))
-        self.assertFalse(UUIDUtils.isUProtocol(None))
-        self.assertFalse(UUIDUtils.isuuid(None))
+        self.assertFalse(UUIDUtils.is_uuidv6(None))
+        self.assertFalse(UUIDUtils.is_uprotocol(None))
+        self.assertFalse(UUIDUtils.is_uuid(None))
 
         uuid1 = MicroUuidSerializer.instance().deserialize(bytes_data)
 
         self.assertTrue(uuid1, UUID())
         self.assertEqual(uuid, uuid1)
 
         uuid2 = LongUuidSerializer.instance().deserialize(uuid_string)
         self.assertTrue(uuid2, UUID())
         self.assertEqual(uuid, uuid2)
 
     def test_UUIDUtils_for_null_uuid(self):
-        self.assertFalse(UUIDUtils.getVersion(None))
-        self.assertEqual(len(MicroUuidSerializer.instance().serialize(None)), 0)
-        self.assertEqual(len(LongUuidSerializer.instance().serialize(None)),0)
-        self.assertFalse(UUIDUtils.isUuidv6(None))
-        self.assertFalse(UUIDUtils.isUProtocol(None))
-        self.assertFalse(UUIDUtils.isuuid(None))
-        self.assertFalse(UUIDUtils.getTime(None))
+        self.assertFalse(UUIDUtils.get_version(None))
+        self.assertEqual(
+            len(MicroUuidSerializer.instance().serialize(None)), 0
+        )
+        self.assertEqual(len(LongUuidSerializer.instance().serialize(None)), 0)
+        self.assertFalse(UUIDUtils.is_uuidv6(None))
+        self.assertFalse(UUIDUtils.is_uprotocol(None))
+        self.assertFalse(UUIDUtils.is_uuid(None))
+        self.assertFalse(UUIDUtils.get_time(None))
 
     def test_uuidutils_from_invalid_uuid(self):
         uuid = UUID(msb=9 << 12, lsb=0)  # Invalid UUID type
-        self.assertFalse(UUIDUtils.getVersion(uuid))
-        self.assertFalse(UUIDUtils.getTime(uuid))
-        self.assertTrue(len(MicroUuidSerializer.instance().serialize(uuid)) > 0)
-        self.assertFalse(LongUuidSerializer.instance().serialize(uuid).isspace())
-        self.assertFalse(UUIDUtils.isUuidv6(uuid))
-        self.assertFalse(UUIDUtils.isUProtocol(uuid))
-        self.assertFalse(UUIDUtils.isuuid(uuid))
-        self.assertFalse(UUIDUtils.getTime(uuid))
+        self.assertFalse(UUIDUtils.get_version(uuid))
+        self.assertFalse(UUIDUtils.get_time(uuid))
+        self.assertTrue(
+            len(MicroUuidSerializer.instance().serialize(uuid)) > 0
+        )
+        self.assertFalse(
+            LongUuidSerializer.instance().serialize(uuid).isspace()
+        )
+        self.assertFalse(UUIDUtils.is_uuidv6(uuid))
+        self.assertFalse(UUIDUtils.is_uprotocol(uuid))
+        self.assertFalse(UUIDUtils.is_uuid(uuid))
+        self.assertFalse(UUIDUtils.get_time(uuid))
 
     def test_uuidutils_fromstring_with_invalid_string(self):
         uuid = LongUuidSerializer.instance().deserialize(None)
         self.assertTrue(uuid == UUID())
         uuid1 = LongUuidSerializer.instance().deserialize("")
         self.assertTrue(uuid1 == UUID())
 
     def test_uuidutils_frombytes_with_invalid_bytes(self):
         uuid = MicroUuidSerializer.instance().deserialize(None)
         self.assertTrue(uuid == UUID())
         uuid1 = MicroUuidSerializer.instance().deserialize(bytearray())
         self.assertTrue(uuid1 == UUID())
 
     def test_create_uprotocol_uuid_in_the_past(self):
-        past = datetime.utcnow() - timedelta(seconds=10)
+        now = datetime.now()
+        past = now - timedelta(seconds=10)
+        past = past.replace(tzinfo=timezone.utc)
         uuid = Factories.UPROTOCOL.create(past)
-        time = UUIDUtils.getTime(uuid)
-        self.assertTrue(UUIDUtils.isUProtocol(uuid))
-        self.assertTrue(UUIDUtils.isuuid(uuid))
+        time = UUIDUtils.get_time(uuid)
+        self.assertTrue(UUIDUtils.is_uprotocol(uuid))
+        self.assertTrue(UUIDUtils.is_uuid(uuid))
         self.assertTrue(time is not None)
         self.assertEqual(time, int(past.timestamp() * 1000))
 
     def test_create_uprotocol_uuid_with_different_time_values(self):
         uuid = Factories.UPROTOCOL.create()
         import time
-        time.sleep(0.01) # Sleep for 10 milliseconds
+
+        time.sleep(0.01)  # Sleep for 10 milliseconds
         uuid1 = Factories.UPROTOCOL.create()
-        time = UUIDUtils.getTime(uuid)
-        time1 = UUIDUtils.getTime(uuid1)
+        time = UUIDUtils.get_time(uuid)
+        time1 = UUIDUtils.get_time(uuid1)
 
-        self.assertTrue(UUIDUtils.isUProtocol(uuid))
-        self.assertTrue(UUIDUtils.isuuid(uuid))
-        self.assertTrue(UUIDUtils.isUProtocol(uuid1))
-        self.assertTrue(UUIDUtils.isuuid(uuid1))
+        self.assertTrue(UUIDUtils.is_uprotocol(uuid))
+        self.assertTrue(UUIDUtils.is_uuid(uuid))
+        self.assertTrue(UUIDUtils.is_uprotocol(uuid1))
+        self.assertTrue(UUIDUtils.is_uuid(uuid1))
 
         self.assertTrue(time is not None)
         self.assertTrue(time1 is not None)
         self.assertNotEqual(time, time1)
 
     def test_create_both_uuidv6_and_v8_to_compare_performance(self):
         uuidv6_list = []
         uuidv8_list = []
         max_count = 10000
 
-        start = datetime.utcnow()
         for _ in range(max_count):
             uuidv8_list.append(Factories.UPROTOCOL.create())
-        v8_diff = datetime.utcnow() - start
 
-        start = datetime.utcnow()
         for _ in range(max_count):
             uuidv6_list.append(Factories.UUIDV6.create())
-        v6_diff = datetime.utcnow() - start
         # print(
         #     f"UUIDv8: [{v8_diff.total_seconds() / max_count}s] UUIDv6: [{v6_diff.total_seconds() / max_count}s]")
 
 
-if __name__ == '__main__':
+if __name__ == "__main__":
     unittest.main()
-
```

### Comparing `up_python-0.1.1.dev0/tests/test_uuid/test_validator/test_uuidvalidator.py` & `up_python-0.1.2.dev0/tests/test_uuid/test_validator/test_uuidvalidator.py`

 * *Files 0% similar despite different names*

```diff
@@ -57,15 +57,15 @@
         self.assertEqual(UCode.INVALID_ARGUMENT, status.code)
         self.assertEqual(
             "Invalid UUID Version,Invalid UUID Variant,Invalid UUID Time",
             status.message,
         )
 
     def test_invalid_time_uuid(self):
-        epoch_time = datetime.utcfromtimestamp(0).replace(tzinfo=timezone.utc)
+        epoch_time = datetime.fromtimestamp(0, tz=timezone.utc)
 
         uuid = Factories.UPROTOCOL.create(
             epoch_time
         )
         status = Validators.UPROTOCOL.validator().validate(uuid)
         self.assertEqual(UCode.INVALID_ARGUMENT, status.code)
         self.assertEqual("Invalid UUID Time", status.message)
@@ -98,15 +98,15 @@
         self.assertEqual("Invalid UUIDv8 Version,Invalid UUID Time", status2.message)
 
     def test_good_uuidv6(self):
         uuid = Factories.UUIDV6.create()
 
         validator = UuidValidator.get_validator(uuid)
         self.assertIsNotNone(validator)
-        self.assertTrue(UUIDUtils.isUuidv6(uuid))
+        self.assertTrue(UUIDUtils.is_uuidv6(uuid))
         self.assertEqual(UCode.OK, validator.validate(uuid).code)
 
     def test_uuidv6_with_invalid_uuid(self):
         uuid = UUID(msb=9 << 12, lsb=0)
         validator = Validators.UUIDV6.validator()
         self.assertIsNotNone(validator)
         status = validator.validate(uuid)
```

### Comparing `up_python-0.1.1.dev0/uprotocol/cloudevent/README.adoc` & `up_python-0.1.2.dev0/uprotocol/cloudevent/README.adoc`

 * *Files identical despite different names*

### Comparing `up_python-0.1.1.dev0/uprotocol/cloudevent/cloudevents_pb2.py` & `up_python-0.1.2.dev0/uprotocol/cloudevent/cloudevents_pb2.py`

 * *Files identical despite different names*

### Comparing `up_python-0.1.1.dev0/uprotocol/cloudevent/datamodel/ucloudeventattributes.py` & `up_python-0.1.2.dev0/uprotocol/cloudevent/datamodel/ucloudeventattributes.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,39 +20,44 @@
 # under the License.
 # SPDX-FileType: SOURCE
 # SPDX-FileCopyrightText: 2023 General Motors GTO LLC
 # SPDX-License-Identifier: Apache-2.0
 
 # -------------------------------------------------------------------------
 
-from typing import Optional
 
 from uprotocol.proto.uattributes_pb2 import UPriority
-from uprotocol.proto.uattributes_pb2 import UPriority
 
 
 class UCloudEventAttributes:
     """
     Specifies the properties that can configure the UCloudEvent.
     """
 
-    def __init__(self, priority: UPriority, hash_value: str = None, ttl: int = None, token: str = None):
+    def __init__(
+        self,
+        priority: UPriority,
+        hash_value: str = None,
+        ttl: int = None,
+        token: str = None,
+        traceparent: str = None,
+    ):
         """
         Construct the properties object.<br><br>
         @param hash_value: an HMAC generated on the data portion of the CloudEvent message using the device key.
         @param priority: uProtocol Prioritization classifications.
         @param ttl: How long this event should live for after it was generated (in milliseconds). Events without this
         attribute (or value is 0) MUST NOT timeout.
         @param token: Oauth2 access token to perform the access request defined in the request message.
         """
         self.hash = hash_value
         self.priority = priority
         self.ttl = ttl
         self.token = token
-        self.traceparent = None
+        self.traceparent = traceparent
 
     @staticmethod
     def empty():
         """
         Static factory method for creating an empty  cloud event attributes object, to avoid working with null<br><br>
         @return: Returns an empty  cloud event attributes that indicates that there are no added additional
         attributes to configure.
@@ -61,17 +66,21 @@
 
     def is_empty(self):
         """
         Indicates that there are no added additional attributes to configure when building a CloudEvent.<br><br>
         @return: Returns true if this attributes container is an empty container and has no valuable information in
         building a CloudEvent.
         """
-        return (self.hash is None or self.hash.isspace()) and (self.ttl is None) and (
-                    self.token is None or self.token.isspace()) and (self.priority is None or self.priority.isspace()) and (
-                           self.traceparent is None or self.traceparent.isspace())
+        return (
+            (self.hash is None or self.hash.isspace())
+            and (self.ttl is None)
+            and (self.token is None or self.token.isspace())
+            and (self.priority is None or self.priority.isspace())
+            and (self.traceparent is None or self.traceparent.isspace())
+        )
 
     def get_hash(self) -> str:
         """
         An HMAC generated on the data portion of the CloudEvent message using the device key.<br><br>
         @return: Returns an Optional hash attribute.
         """
         return self.hash if self.hash and self.hash.strip() else None
@@ -93,30 +102,51 @@
     def get_token(self) -> str:
         """
         Oauth2 access token to perform the access request defined in the request message.<br><br>
         @return: Returns an Optional OAuth token attribute.
         """
         return self.token if self.token and self.token.strip() else None
 
+    def get_traceparent(self) -> str:
+        """
+        Traceparent of the event.
+        @return: Returns an optional traceparent attribute.
+        """
+        return (
+            self.traceparent
+            if self.traceparent and self.traceparent.strip()
+            else None
+        )
+
     def __eq__(self, other):
         if self is other:
             return True
         if not isinstance(other, UCloudEventAttributes):
             return False
         return (
-                self.hash == other.hash and self.priority == other.priority and self.ttl == other.ttl and self.token
-                == other.token and self.traceparent == other.traceparent)
+            self.hash == other.hash
+            and self.priority == other.priority
+            and self.ttl == other.ttl
+            and self.token == other.token
+            and self.traceparent == other.traceparent
+        )
 
     def __hash__(self):
-        return hash((self.hash, self.priority, self.ttl, self.token, self.traceparent))
+        return hash(
+            (self.hash, self.priority, self.ttl, self.token, self.traceparent)
+        )
 
     def __str__(self):
-        traceparent_string = f", traceparent='{self.traceparent}'" if self.traceparent else ""
-        return f"UCloudEventAttributes{{hash='{self.hash}', priority={self.priority}," \
-               f" ttl={self.ttl}, token='{self.token}'{traceparent_string}}}"
+        traceparent_string = (
+            f", traceparent='{self.traceparent}'" if self.traceparent else ""
+        )
+        return (
+            f"UCloudEventAttributes{{hash='{self.hash}', priority={self.priority},"
+            f" ttl={self.ttl}, token='{self.token}'{traceparent_string}}}"
+        )
 
 
 class UCloudEventAttributesBuilder:
     """
     Builder for constructing the UCloudEventAttributes.
     """
 
@@ -161,30 +191,25 @@
         Add an Oauth2 access token to perform the access request defined in the request message.<br><br>
         @param token: An Oauth2 access token to perform the access request defined in the request message.
         @return: Returns the UCloudEventAttributesBuilder with the configured OAuth token.
         """
         self.token = token
         return self
 
-
     def with_traceparent(self, traceparent: str):
         """
         An identifier used to correlate observability across related events.
         @param traceparent: identifier
         @return Returns a traceparent attribute.
         """
         self.traceparent = traceparent
         return self
 
     def build(self):
         """
         Construct the UCloudEventAttributes from the builder.<br><br>
         @return: Returns a constructed UProperty.
         """
-        return UCloudEventAttributes(self.priority, self.hash, self.ttl, self.token)
-
+        return UCloudEventAttributes(
+            self.priority, self.hash, self.ttl, self.token, self.traceparent
+        )
 
-if __name__ == "__main__":
-    # Example usage:
-    attributes = UCloudEventAttributesBuilder().with_hash("abc123").with_priority(UPriority.UPRIORITY_CS0).with_ttl(
-        1000).with_token("xyz456").with_traceparent("123456").build()
-    print(attributes)
```

### Comparing `up_python-0.1.1.dev0/uprotocol/cloudevent/factory/cloudeventfactory.py` & `up_python-0.1.2.dev0/uprotocol/cloudevent/factory/cloudeventfactory.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,83 +25,103 @@
 # -------------------------------------------------------------------------
 
 
 from cloudevents.http import CloudEvent
 from google.protobuf import empty_pb2
 from google.protobuf.any_pb2 import Any
 
-from uprotocol.cloudevent.datamodel.ucloudeventattributes import UCloudEventAttributes
+from uprotocol.cloudevent.datamodel.ucloudeventattributes import (
+    UCloudEventAttributes,
+)
 from uprotocol.cloudevent.factory.ucloudevent import UCloudEvent
 from uprotocol.proto.uattributes_pb2 import UMessageType
 from uprotocol.uuid.factory.uuidfactory import Factories
 from uprotocol.uuid.serializer.longuuidserializer import LongUuidSerializer
 
 
 # A factory is a part of the software has methods to generate concrete objects, usually of the same type or
 # interface. CloudEvents is a specification for describing events in a common way. We will use CloudEvents to
 # formulate all kinds of  events (messages) that will be sent to and from devices. The CloudEvent factory knows how
 # to generate CloudEvents of the 4 core types: req.v1, res.v1 and pub.v1
 class CloudEventFactory:
     PROTOBUF_CONTENT_TYPE = "application/x-protobuf"
 
     @staticmethod
-    def request(application_uri_for_rpc: str, service_method_uri: str, request_id: str, proto_payload: Any,
-                attributes: UCloudEventAttributes) -> CloudEvent:
+    def request(
+        application_uri_for_rpc: str,
+        service_method_uri: str,
+        request_id: str,
+        proto_payload: Any,
+        attributes: UCloudEventAttributes,
+    ) -> CloudEvent:
         """
         Create a CloudEvent for an event for the use case of: RPC Request message.
         @param application_uri_for_rpc: The uri for the application requesting the RPC.
         @param service_method_uri: The uri for the method to be called on the service Ex. :/body.access/1/rpc.UpdateDoor
         @param request_id:The attribute id from the original request
         @param proto_payload:Protobuf Any object with the Message command to be executed on the sink service.
         @param attributes: Additional attributes such as ttl, hash, priority and token.
         @return: Returns an  request CloudEvent.
         """
         event_id = CloudEventFactory.generate_cloud_event_id()
-        cloud_event = CloudEventFactory.build_base_cloud_event(event_id, application_uri_for_rpc,
-
-                                                               proto_payload.SerializeToString(),
-                                                               proto_payload.DESCRIPTOR.full_name, attributes,
-                                                               UCloudEvent.get_event_type(
-                                                                   UMessageType.UMESSAGE_TYPE_REQUEST)
-                                                               )
+        cloud_event = CloudEventFactory.build_base_cloud_event(
+            event_id,
+            application_uri_for_rpc,
+            proto_payload.SerializeToString(),
+            proto_payload.DESCRIPTOR.full_name,
+            attributes,
+            UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_REQUEST),
+        )
         cloud_event.__setitem__("sink", service_method_uri)
         cloud_event.__setitem__("reqid", request_id)
 
         return cloud_event
 
     @staticmethod
-    def response(application_uri_for_rpc: str, service_method_uri: str, request_id: str, proto_payload: Any,
-                 attributes: UCloudEventAttributes) -> CloudEvent:
+    def response(
+        application_uri_for_rpc: str,
+        service_method_uri: str,
+        request_id: str,
+        proto_payload: Any,
+        attributes: UCloudEventAttributes,
+    ) -> CloudEvent:
         """
         Create a CloudEvent for an event for the use case of: RPC Response message.
         @param application_uri_for_rpc: The destination of the response. The uri for the original application that
         requested the RPC and this response is for.
         @param service_method_uri: The uri for the method that was called on the service Ex.
         :/body.access/1/rpc.UpdateDoor
         @param request_id:The cloud event id from the original request cloud event that this response if for.
         @param proto_payload: The protobuf serialized response message as defined by the application interface or the
         UStatus message containing the details of an error.
         @param attributes: Additional attributes such as ttl, hash and priority.
         @return: Returns an  response CloudEvent.
         """
         event_id = CloudEventFactory.generate_cloud_event_id()
-        cloud_event = CloudEventFactory.build_base_cloud_event(event_id, service_method_uri,
-
-                                                               proto_payload.SerializeToString(),
-                                                               proto_payload.DESCRIPTOR.full_name, attributes,
-                                                               UCloudEvent.get_event_type(
-                                                                   UMessageType.UMESSAGE_TYPE_RESPONSE))
+        cloud_event = CloudEventFactory.build_base_cloud_event(
+            event_id,
+            service_method_uri,
+            proto_payload.SerializeToString(),
+            proto_payload.DESCRIPTOR.full_name,
+            attributes,
+            UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_RESPONSE),
+        )
         cloud_event.__setitem__("sink", application_uri_for_rpc)
         cloud_event.__setitem__("reqid", request_id)
 
         return cloud_event
 
     @staticmethod
-    def failed_response(application_uri_for_rpc: str, service_method_uri: str, request_id: str,
-                        communication_status: int, attributes: UCloudEventAttributes) -> CloudEvent:
+    def failed_response(
+        application_uri_for_rpc: str,
+        service_method_uri: str,
+        request_id: str,
+        communication_status: int,
+        attributes: UCloudEventAttributes,
+    ) -> CloudEvent:
         """
         Create a CloudEvent for an event for the use case of: RPC Response message that failed.
         @param application_uri_for_rpc: The destination of the response. The uri for the original application that
         requested the RPC and this response is for.
         @param service_method_uri: The uri for the method that was called on the service Ex.
         :/body.access/1/rpc.UpdateDoor
         @param request_id:The cloud event id from the original request cloud event that this response if for.
@@ -110,98 +130,122 @@
         @param attributes:Additional attributes such as ttl, hash and priority.
         @return:Returns an  response CloudEvent Response for the use case of RPC Response message that failed.
         """
         event_id = CloudEventFactory.generate_cloud_event_id()
         # Create an Any message packing an Empty message
         empty_proto_payload = Any()
         empty_proto_payload.Pack(empty_pb2.Empty())
-        cloud_event = CloudEventFactory.build_base_cloud_event(event_id, service_method_uri,
-
-                                                               empty_proto_payload.SerializeToString(),  # Empty payload
-                                                               "google.protobuf.Empty", attributes,
-                                                               UCloudEvent.get_event_type(
-                                                                   UMessageType.UMESSAGE_TYPE_RESPONSE)
-                                                               )
+        cloud_event = CloudEventFactory.build_base_cloud_event(
+            event_id,
+            service_method_uri,
+            empty_proto_payload.SerializeToString(),  # Empty payload
+            "google.protobuf.Empty",
+            attributes,
+            UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_RESPONSE),
+        )
         cloud_event.__setitem__("sink", application_uri_for_rpc)
         cloud_event.__setitem__("reqid", request_id)
         cloud_event.__setitem__("commstatus", communication_status)
 
         return cloud_event
 
     @staticmethod
-    def publish(source: str, proto_payload: Any, attributes: UCloudEventAttributes) -> CloudEvent:
+    def publish(
+        source: str, proto_payload: Any, attributes: UCloudEventAttributes
+    ) -> CloudEvent:
         """
         Create a CloudEvent for an event for the use case of: Publish generic message.
         @param source:The  uri of the topic being published.
         @param proto_payload:protobuf Any object with the Message to be published.
         @param attributes:Additional attributes such as ttl, hash and priority.
         @return:Returns a publish CloudEvent.
         """
         event_id = CloudEventFactory.generate_cloud_event_id()
-        cloud_event = CloudEventFactory.build_base_cloud_event(event_id, source, proto_payload.SerializeToString(),
-                                                               proto_payload.DESCRIPTOR.full_name, attributes,
-                                                               UCloudEvent.get_event_type(
-                                                                   UMessageType.UMESSAGE_TYPE_PUBLISH))
+        cloud_event = CloudEventFactory.build_base_cloud_event(
+            event_id,
+            source,
+            proto_payload.SerializeToString(),
+            proto_payload.DESCRIPTOR.full_name,
+            attributes,
+            UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_PUBLISH),
+        )
 
         return cloud_event
 
     @staticmethod
-    def notification(source: str, sink: str, proto_payload: Any, attributes: UCloudEventAttributes) -> CloudEvent:
+    def notification(
+        source: str,
+        sink: str,
+        proto_payload: Any,
+        attributes: UCloudEventAttributes,
+    ) -> CloudEvent:
         """
         Create a CloudEvent for an event for the use case of: Publish a notification message. A published event
         containing the sink (destination) is often referred to as a notification, it is an event sent to a specific
         consumer.
         @param source: The  uri of the topic being published.
         @param sink:  The  uri of the destination of this notification.
         @param proto_payload: protobuf Any object with the Message to be published.
         @param attributes:  Additional attributes such as ttl, hash and priority.
         @return: Returns a publish CloudEvent.
         """
         event_id = CloudEventFactory.generate_cloud_event_id()
-        cloud_event = CloudEventFactory.build_base_cloud_event(event_id, source, proto_payload.SerializeToString(),
-                                                               proto_payload.DESCRIPTOR.full_name, attributes,
-                                                               UCloudEvent.get_event_type(
-                                                                   UMessageType.UMESSAGE_TYPE_PUBLISH))
+        cloud_event = CloudEventFactory.build_base_cloud_event(
+            event_id,
+            source,
+            proto_payload.SerializeToString(),
+            proto_payload.DESCRIPTOR.full_name,
+            attributes,
+            UCloudEvent.get_event_type(UMessageType.UMESSAGE_TYPE_PUBLISH),
+        )
         cloud_event.__setitem__("sink", sink)
 
         return cloud_event
 
     @staticmethod
     def generate_cloud_event_id() -> str:
         """
         Generate a UUIDv8
         @return:  Returns a UUIDv8 id.
         """
         uuid_inst = Factories.UPROTOCOL.create()
         return LongUuidSerializer.instance().serialize(uuid_inst)
 
     @staticmethod
-    def build_base_cloud_event(id: str, source: str, proto_payload_bytes: bytes, proto_payload_schema: str,
-                               attributes: UCloudEventAttributes, type) -> CloudEvent:
+    def build_base_cloud_event(
+        id: str,
+        source: str,
+        proto_payload_bytes: bytes,
+        proto_payload_schema: str,
+        attributes: UCloudEventAttributes,
+        type,
+    ) -> CloudEvent:
         """
         Base CloudEvent builder that is the same for all CloudEvent types.
-        
+
         @param id:Event unique identifier.
         @param source: Identifies who is sending this event in the format of a uProtocol URI that can be built from a
         UUri object.
         @param proto_payload_bytes:The serialized Event data with the content type of "application/x-protobuf".
         @param proto_payload_schema:The schema of the proto payload bytes, for example you can use
         <code>protoPayload.getTypeUrl()</code> on your service/app object.
         @param attributes:Additional cloud event attributes that can be passed in. All attributes are optional and
         will be added only if they were configured.
         @param type: Type of the cloud event
         @return:Returns a CloudEventBuilder that can be additionally configured and then by calling .build()
         construct a CloudEvent ready to be serialized and sent to the transport layer.
         """
         json_attributes = {"id": id, "source": source, "type": type}
         if attributes.get_hash() is not None:
-            json_attributes['hash'] = attributes.get_hash()
+            json_attributes["hash"] = attributes.get_hash()
         if attributes.get_ttl() is not None:
-            json_attributes['ttl'] = attributes.get_ttl()
+            json_attributes["ttl"] = attributes.get_ttl()
         if attributes.get_priority() is not None:
-            json_attributes['priority'] = attributes.get_priority()
+            json_attributes["priority"] = attributes.get_priority()
         if attributes.get_token() is not None:
-            json_attributes['token'] = attributes.get_token()
+            json_attributes["token"] = attributes.get_token()
+        if attributes.get_traceparent() is not None:
+            json_attributes["traceparent"] = attributes.get_traceparent()
 
         cloud_event = CloudEvent(json_attributes, proto_payload_bytes)
 
         return cloud_event
```

### Comparing `up_python-0.1.1.dev0/uprotocol/cloudevent/factory/ucloudevent.py` & `up_python-0.1.2.dev0/uprotocol/cloudevent/factory/ucloudevent.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 # -------------------------------------------------------------------------
-import time
 # Copyright (c) 2023 General Motors GTO LLC
 #
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
@@ -21,462 +20,629 @@
 # SPDX-FileType: SOURCE
 # SPDX-FileCopyrightText: 2023 General Motors GTO LLC
 # SPDX-License-Identifier: Apache-2.0
 
 # -------------------------------------------------------------------------
 
 
-from datetime import datetime, timedelta
+import time
+from datetime import datetime, timedelta, timezone
+import copy
 
 from cloudevents.http import CloudEvent
 from google.protobuf import any_pb2
 from google.protobuf.message import DecodeError
 
 from uprotocol.proto.ustatus_pb2 import UCode
-from uprotocol.proto.uattributes_pb2 import UMessageType, UPriority, UAttributes
+from uprotocol.proto.uattributes_pb2 import (
+    UMessageType,
+    UPriority,
+    UAttributes,
+)
 from uprotocol.proto.upayload_pb2 import UPayload
-from uprotocol.proto.uri_pb2 import UUri
 from uprotocol.uri.serializer.longuriserializer import LongUriSerializer
 from uprotocol.uuid.factory.uuidutils import UUIDUtils
 from uprotocol.uuid.serializer.longuuidserializer import LongUuidSerializer
-from uprotocol.proto.upayload_pb2 import UPayloadFormat, UPayload
+from uprotocol.proto.upayload_pb2 import UPayloadFormat
 from uprotocol.proto.umessage_pb2 import UMessage
 from uprotocol.proto.uuid_pb2 import UUID
 
 
 class UCloudEvent:
     """
     Class to extract  information from a CloudEvent.
     """
 
     @staticmethod
     def get_source(ce: CloudEvent) -> str:
         """
-        Extract the source from a cloud event. The source is a mandatory attribute. The CloudEvent constructor does
-        not allow creating a cloud event without a source.<br><br>
-        @param ce:CloudEvent with source to be extracted.
-        @return:Returns the String value of a CloudEvent source attribute.
+        Extract the source from a cloud event. The source is a mandatory
+        attribute. The CloudEvent constructor does not allow creating a cloud
+        event without a source.<br><br>
+        @param ce:CloudEvent with source to be
+        extracted.
+        @return:Returns the String value of a CloudEvent source
+        attribute.
         """
         return UCloudEvent.extract_string_value_from_attributes("source", ce)
 
     @staticmethod
     def get_data_content_type(ce: CloudEvent) -> str:
         """
-        Extract the source from a cloud event. The source is a mandatory attribute. The CloudEvent constructor does
-        not allow creating a cloud event without a source.<br><br>
-        @param ce:CloudEvent with source to be extracted.
-        @return:Returns the String value of a CloudEvent source attribute.
-        """
-        return UCloudEvent.extract_string_value_from_attributes("datacontenttype", ce)
+        Extract the source from a cloud event. The source is a mandatory
+        attribute. The CloudEvent constructor does not allow creating a cloud
+        event without a source.<br><br>
+        @param ce:CloudEvent with source to be
+        extracted.
+        @return:Returns the String value of a CloudEvent source
+        attribute.
+        """
+        return UCloudEvent.extract_string_value_from_attributes(
+            "datacontenttype", ce
+        )
 
     @staticmethod
     def get_data_schema(ce: CloudEvent) -> str:
         """
-        Extract the source from a cloud event. The source is a mandatory attribute. The CloudEvent constructor does
-        not allow creating a cloud event without a source.<br><br>
-        @param ce:CloudEvent with source to be extracted.
-        @return:Returns the String value of a CloudEvent source attribute.
-        """
-        return UCloudEvent.extract_string_value_from_attributes("dataschema", ce)
+        Extract the source from a cloud event. The source is a mandatory
+        attribute. The CloudEvent constructor does not allow creating a cloud
+        event without a source.<br><br>
+        @param ce:CloudEvent with source to be
+        extracted.
+        @return:Returns the String value of a CloudEvent source
+        attribute.
+        """
+        return UCloudEvent.extract_string_value_from_attributes(
+            "dataschema", ce
+        )
 
     @staticmethod
     def get_type(ce: CloudEvent) -> str:
         """
-        Extract the type from a cloud event. The source is a mandatory attribute. The CloudEvent constructor does
-        not allow creating a cloud event without a type.<br><br>
-        @param ce:CloudEvent with source to be extracted.
-        @return:Returns the String value of a CloudEvent type attribute.
+        Extract the type from a cloud event. The source is a mandatory
+        attribute. The CloudEvent constructor does not allow creating a cloud
+        event without a type.<br><br>
+        @param ce:CloudEvent with source to be
+        extracted.
+        @return:Returns the String value of a CloudEvent type
+        attribute.
         """
         return UCloudEvent.extract_string_value_from_attributes("type", ce)
 
     @staticmethod
     def get_id(ce: CloudEvent) -> str:
         """
-        Extract the id from a cloud event. The id is a mandatory attribute. The CloudEvent constructor does
-        not allow creating a cloud event without an id.<br><br>
+        Extract the id from a cloud event. The id is a mandatory attribute. The
+        CloudEvent constructor does not allow creating a cloud event without an
+        id.<br><br>
         @param ce:CloudEvent with source to be extracted.
         @return:Returns the String value of a CloudEvent id attribute.
         """
         return UCloudEvent.extract_string_value_from_attributes("id", ce)
 
     @staticmethod
     def get_specversion(ce: CloudEvent) -> str:
         """
         Extract the specversion from a cloud event. <br><br>
-        @param ce:CloudEvent with source to be extracted.
-        @return:Returns the String value of a CloudEvent spec version attribute.
-        """
-        return UCloudEvent.extract_string_value_from_attributes("specversion", ce)
+        @param
+        ce:CloudEvent with source to be extracted.
+        @return:Returns the String
+        value of a CloudEvent spec version attribute.
+        """
+        return UCloudEvent.extract_string_value_from_attributes(
+            "specversion", ce
+        )
 
     @staticmethod
     def get_sink(ce: CloudEvent) -> str:
         """
-        Extract the sink from a cloud event. The sink attribute is optional.<br><br>
+        Extract the sink from a cloud event. The sink attribute is
+        optional.<br><br>
         @param ce:CloudEvent with sink to be extracted.
-        @return:Returns an Optional String value of a CloudEvent sink attribute if it exists, otherwise an
-        Optional.empty() is returned.
+        @return:Returns an Optional String value of a CloudEvent sink attribute
+        if it exists, otherwise an Optional.empty() is returned.
         """
         return UCloudEvent.extract_string_value_from_attributes("sink", ce)
 
     @staticmethod
     def get_request_id(ce: CloudEvent) -> str:
         """
-        Extract the request id from a cloud event that is a response RPC CloudEvent. The attribute is optional.<br><br>
-        @param ce: the response RPC CloudEvent with request id to be extracted.
-        @return: Returns an Optional String value of a response RPC CloudEvent request id attribute if it exists,
-        otherwise an Optional.empty() is returned.
+        Extract the request id from a cloud event that is a response RPC
+        CloudEvent. The attribute is optional.<br><br>
+        @param ce: the response
+        RPC CloudEvent with request id to be extracted.
+        @return: Returns an
+        Optional String value of a response RPC CloudEvent request id attribute
+        if it exists, otherwise an Optional.empty() is returned.
         """
         return UCloudEvent.extract_string_value_from_attributes("reqid", ce)
 
     @staticmethod
     def get_hash(ce: CloudEvent) -> str:
         """
-        Extract the hash attribute from a cloud event. The hash attribute is optional.<br><br>
+        Extract the hash attribute from a cloud event. The hash attribute is
+        optional.<br><br>
         @param ce: CloudEvent with hash to be extracted.
-        @return:Returns an Optional String value of a CloudEvent hash attribute if it exists, otherwise an
-        Optional.empty() is returned.
+        @return:Returns an Optional String value of a CloudEvent hash attribute
+        if it exists, otherwise an Optional.empty() is returned.
         """
         return UCloudEvent.extract_string_value_from_attributes("hash", ce)
 
     @staticmethod
     def get_priority(ce: CloudEvent) -> str:
         """
-        Extract the string value of the priority attribute from a cloud event. The priority attribute is
-        optional.<br><br>
-        @param ce:CloudEvent with priority to be extracted.
-        @return:Returns an Optional String value of a CloudEvent priority attribute if it exists,  otherwise an
+        Extract the string value of the priority attribute from a cloud event.
+        The priority attribute is optional.<br><br>
+        @param ce:CloudEvent with
+        priority to be extracted.
+        @return:Returns an Optional String value of a
+        CloudEvent priority attribute if it exists,  otherwise an
         Optional.empty() is returned.
         """
         return UCloudEvent.extract_string_value_from_attributes("priority", ce)
 
     @staticmethod
     def get_ttl(ce: CloudEvent) -> int:
         """
-        Extract the integer value of the ttl attribute from a cloud event. The ttl attribute is optional.<br><br>
-        @param ce:CloudEvent with ttl to be extracted.
-        @return: Returns an Optional String value of a CloudEvent ttl attribute if it exists,otherwise an
-        Optional.empty() is returned.
+        Extract the integer value of the ttl attribute from a cloud event. The
+        ttl attribute is optional.<br><br>
+        @param ce:CloudEvent with ttl to be
+        extracted.
+        @return: Returns an Optional String value of a CloudEvent
+        ttl attribute if it exists,otherwise an Optional.empty() is returned.
         """
         ttl_str = UCloudEvent.extract_string_value_from_attributes("ttl", ce)
         return int(ttl_str) if ttl_str is not None else None
 
     @staticmethod
     def get_token(ce: CloudEvent) -> str:
         """
-        Extract the string value of the token attribute from a cloud event. The token attribute is optional.<br><br>
-        @param ce: CloudEvent with token to be extracted.
-        @return:Returns an Optional String value of a CloudEvent priority token if it exists, otherwise an
-        Optional.empty() is returned.
+        Extract the string value of the token attribute from a cloud event. The
+        token attribute is optional.<br><br>
+        @param ce: CloudEvent with token
+        to be extracted.
+        @return:Returns an Optional String value of a
+        CloudEvent priority token if it exists, otherwise an Optional.empty()
+        is returned.
         """
         return UCloudEvent.extract_string_value_from_attributes("token", ce)
 
     @staticmethod
-    def get_communication_status(ce: CloudEvent) -> int:
+    def get_communication_status(ce: CloudEvent) -> UCode:
         """
-        Extract the integer value of the communication status attribute from a cloud event. The communication status
-        attribute is optional. If there was a platform communication error that occurred while delivering this
-        cloudEvent, it will be indicated in this attribute. If the attribute does not exist, it is assumed that
-        everything was UCode.OK_VALUE.<br><br>
-        @param ce: CloudEvent with the platformError to be extracted.
-        @return: Returns a UCode value that indicates of a platform communication error while delivering this
-        CloudEvent or UCode.OK_VALUE.
+        Extract the integer value of the communication status attribute from a
+        cloud event. The communication status attribute is optional. If there
+        was a platform communication error that occurred while delivering this
+        cloudEvent, it will be indicated in this attribute. If the attribute
+        does not exist, it is assumed that everything was
+        UCode.OK_VALUE.<br><br>
+        @param ce: CloudEvent with the platformError to
+        be extracted.
+        @return: Returns a UCode value that indicates of a
+        platform communication error while delivering this CloudEvent or
+        UCode.OK_VALUE.
         """
         try:
-            comm_status = UCloudEvent.extract_string_value_from_attributes("commstatus", ce)
+            comm_status = UCloudEvent.extract_string_value_from_attributes(
+                "commstatus", ce
+            )
             return int(comm_status) if comm_status is not None else UCode.OK
-        except:
+        except Exception:
             return UCode.OK
 
     @staticmethod
+    def get_traceparent(ce: CloudEvent) -> str:
+        """
+        Extract the string value of the traceparent attribute from a cloud
+        event. The traceparent attribute is optional.
+        @param ce: CloudEvent
+        with traceparent to be extracted.
+        @return: Returns the string value of
+        the traceparent if it exists, else returns None.
+        """
+        return UCloudEvent.extract_string_value_from_attributes(
+            "traceparent", ce
+        )
+
+    @staticmethod
     def has_communication_status_problem(ce: CloudEvent) -> bool:
         """
-        Indication of a platform communication error that occurred while trying to deliver the CloudEvent.<br><br>
-        @param ce:CloudEvent to be queried for a platform delivery error.
-        @return:returns true if the provided CloudEvent is marked with having a platform delivery problem.
+        Indication of a platform communication error that occurred while trying
+        to deliver the CloudEvent.<br><br>
+        @param ce:CloudEvent to be queried
+        for a platform delivery error.
+        @return:returns true if the provided
+        CloudEvent is marked with having a platform delivery problem.
         """
         return UCloudEvent.get_communication_status(ce) != UCode.OK
 
     @staticmethod
-    def add_communication_status(ce: CloudEvent, communication_status) -> CloudEvent:
-        """
-        Returns a new CloudEvent from the supplied CloudEvent, with the platform communication added.<br><br>
-        @param ce:CloudEvent that the platform delivery error will be added.
-        @param communication_status:the platform delivery error UCode to add to the CloudEvent.
-        @return:Returns a new CloudEvent from the supplied CloudEvent, with the platform communication added.
+    def add_communication_status(
+        ce: CloudEvent, communication_status
+    ) -> CloudEvent:
+        """
+        Returns a new CloudEvent from the supplied CloudEvent, with the
+        platform communication added.<br><br>
+        @param ce:CloudEvent that the
+        platform delivery error will be added.
+        @param communication_status:the
+        platform delivery error UCode to add to the CloudEvent.
+        @return:Returns
+        a new CloudEvent from the supplied CloudEvent, with the platform
+        communication added.
         """
         if communication_status is None:
             return ce
-        ce.__setitem__("commstatus", communication_status)
-        return ce
+        ce_new = copy.deepcopy(ce)
+        ce_new.__setitem__("commstatus", communication_status)
+        return ce_new
 
     @staticmethod
     def get_creation_timestamp(ce: CloudEvent) -> int:
         """
         Extract the timestamp from the UUIDV8 CloudEvent Id.<br><br>
-        @param ce:The CloudEvent with the timestamp to extract.
-        @return:Return the timestamp from the UUIDV8 CloudEvent Id or an empty Optional if timestamp can't be extracted.
-        """
-        cloud_event_id = UCloudEvent.extract_string_value_from_attributes("id", ce)
+        @param
+        ce:The CloudEvent with the timestamp to extract.
+        @return:Return the
+        timestamp from the UUIDV8 CloudEvent Id or an empty Optional if
+        timestamp can't be extracted.
+        """
+        cloud_event_id = UCloudEvent.extract_string_value_from_attributes(
+            "id", ce
+        )
         uuid = LongUuidSerializer.instance().deserialize(cloud_event_id)
 
-        return UUIDUtils.getTime(uuid) if uuid is not None else None
+        return UUIDUtils.get_time(uuid) if uuid is not None else None
 
     @staticmethod
     def is_expired_by_cloud_event_creation_date(ce: CloudEvent) -> bool:
         """
-        Calculate if a CloudEvent configured with a creation time and a ttl attribute is expired. The ttl attribute
-        is a configuration of how long this event should live for after it was generated (in milliseconds)<br><br>
-        @param ce:The CloudEvent to inspect for being expired.
-        @return:Returns true if the CloudEvent was configured with a ttl &gt; 0 and a creation time to compare for
-        expiration.
+        Calculate if a CloudEvent configured with a creation time and a ttl
+        attribute is expired. The ttl attribute is a configuration of how long
+        this event should live for after it was generated (in
+        milliseconds)<br><br>
+        @param ce:The CloudEvent to inspect for being
+        expired.
+        @return:Returns true if the CloudEvent was configured with a
+        ttl &gt; 0 and a creation time to compare for expiration.
         """
         maybe_ttl = UCloudEvent.get_ttl(ce)
         if not maybe_ttl or maybe_ttl <= 0:
             return False
 
-        cloud_event_creation_time = UCloudEvent.extract_string_value_from_attributes("time", ce)
+        cloud_event_creation_time = (
+            UCloudEvent.extract_string_value_from_attributes("time", ce)
+        )
         if cloud_event_creation_time is None:
             return False
 
-        now = datetime.now()
-        creation_time_plus_ttl = cloud_event_creation_time + timedelta(milliseconds=maybe_ttl)
+        now = datetime.now(timezone.utc)
+        creation_time_plus_ttl = datetime.fromisoformat(cloud_event_creation_time) + timedelta(
+            milliseconds=maybe_ttl
+        )
 
         return now > creation_time_plus_ttl
 
     @staticmethod
     def is_expired(ce: CloudEvent) -> bool:
         """
-        Calculate if a CloudEvent configured with UUIDv8 id and a ttl attribute is expired. The ttl attribute is a
-        configuration of how long this event should live for after it was generated (in milliseconds).<br><br>
+        Calculate if a CloudEvent configured with UUIDv8 id and a ttl attribute
+        is expired. The ttl attribute is a configuration of how long this event
+        should live for after it was generated (in milliseconds).<br><br>
         @param ce:The CloudEvent to inspect for being expired.
-        @return:Returns true if the CloudEvent was configured with a ttl &gt; 0 and UUIDv8 id to compare for expiration.
+        @return:Returns
+        true if the CloudEvent was configured with a ttl &gt; 0 and UUIDv8 id
+        to compare for expiration.
         """
         maybe_ttl = UCloudEvent.get_ttl(ce)
         if not maybe_ttl or maybe_ttl <= 0:
             return False
-        cloud_event_id = UCloudEvent.extract_string_value_from_attributes("id", ce)
+        cloud_event_id = UCloudEvent.extract_string_value_from_attributes(
+            "id", ce
+        )
 
         try:
             uuid = LongUuidSerializer.instance().deserialize(cloud_event_id)
             if uuid is None or uuid == UUID():
                 return False
-            delta =  int(round(time.time() * 1000)) - UUIDUtils.getTime(uuid)
+            delta = int(round(time.time() * 1000)) - UUIDUtils.get_time(uuid)
         except ValueError:
             # Invalid UUID, handle accordingly
             delta = 0
         return delta >= maybe_ttl
 
     @staticmethod
     def is_cloud_event_id(ce: CloudEvent) -> bool:
         """
         Check if a CloudEvent is a valid UUIDv6 or v8 .<br><br>
         @param ce:The CloudEvent with the id to inspect.
         @return: Returns true if the CloudEvent is valid.
         """
-        cloud_event_id = UCloudEvent.extract_string_value_from_attributes("id", ce)
+        cloud_event_id = UCloudEvent.extract_string_value_from_attributes(
+            "id", ce
+        )
         uuid = LongUuidSerializer.instance().deserialize(cloud_event_id)
 
-        return uuid is not None and UUIDUtils.isuuid(uuid)
+        return uuid is not None and UUIDUtils.is_uuid(uuid)
 
     @staticmethod
     def get_payload(ce: CloudEvent) -> any_pb2.Any:
         """
-        Extract the payload from the CloudEvent as a protobuf Any object. <br>An all or nothing error handling
-        strategy is implemented. If anything goes wrong, an Any.getDefaultInstance() will be returned.<br><br>
-        @param ce:CloudEvent containing the payload to extract.
-        @return:Extracts the payload from a CloudEvent as a Protobuf Any object.
+        Extract the payload from the CloudEvent as a protobuf Any object.
+        <br>An all or nothing error handling strategy is implemented. If
+        anything goes wrong, an Any.getDefaultInstance() will be
+        returned.<br><br>
+        @param ce:CloudEvent containing the payload to
+        extract.
+        @return:Extracts the payload from a CloudEvent as a Protobuf
+        Any object.
         """
         data = ce.get_data()
         if data is None:
             return any_pb2.Any()
         try:
             return any_pb2.Any().FromString(data)
         except DecodeError:
             return any_pb2.Any()
 
     @staticmethod
     def unpack(ce: CloudEvent, clazz):
         """
-        Extract the payload from the CloudEvent as a protobuf Message of the provided class. The protobuf of this
-        message class must be loaded on the client for this to work. <br>  An all or nothing error handling strategy
-        is implemented. If anything goes wrong, an empty optional will be returned. <br><br> Example: <br>
-        <pre>Optional&lt;SomeMessage&gt; unpacked = UCloudEvent.unpack(cloudEvent, SomeMessage.class);</pre><br><br>
-        @param ce:CloudEvent containing the payload to extract.
-        @param clazz:The class that extends Message that the payload is extracted into.
-        @return:  Returns a Message payload of the class type that is provided.
+        Extract the payload from the CloudEvent as a protobuf Message of the
+        provided class. The protobuf of this message class must be loaded on
+        the client for this to work. <br>  An all or nothing error handling
+        strategy is implemented. If anything goes wrong, an empty optional will
+        be returned. <br><br> Example: <br> <pre>Optional&lt;SomeMessage&gt;
+        unpacked = UCloudEvent.unpack(cloudEvent,
+        SomeMessage.class);</pre><br><br>
+        @param ce:CloudEvent containing the
+        payload to extract.
+        @param clazz:The class that extends Message that
+        the payload is extracted into.
+        @return:  Returns a Message payload of
+        the class type that is provided.
         """
         try:
             any_obj = UCloudEvent.get_payload(ce)
             value = clazz()
             value.ParseFromString(any_obj.value)
             return value
         except DecodeError:
             return None
 
     @staticmethod
     def to_string(ce: CloudEvent) -> str:
         """
-        Function used to pretty print a CloudEvent containing only the id, source, type and maybe a sink. Used mainly
-        for logging.<br><br>
-        @param ce:The CloudEvent we want to pretty print.
-        @return:returns the String representation of the CloudEvent containing only the id, source, type and maybe a
-        sink.
+        Function used to pretty print a CloudEvent containing only the id,
+        source, type and maybe a sink. Used mainly for logging.<br><br>
+        @param
+        ce:The CloudEvent we want to pretty print.
+        @return:returns the String
+        representation of the CloudEvent containing only the id, source, type
+        and maybe a sink.
         """
         if ce is not None:
             sink_str = UCloudEvent.get_sink(ce)
             sink_str = f", sink='{sink_str}'" if sink_str is not None else ""
             id = UCloudEvent.extract_string_value_from_attributes("id", ce)
-            source = UCloudEvent.extract_string_value_from_attributes("source", ce)
+            source = UCloudEvent.extract_string_value_from_attributes(
+                "source", ce
+            )
             type = UCloudEvent.extract_string_value_from_attributes("type", ce)
             return f"CloudEvent{{id='{id}', source='{source}'{sink_str}, type='{type}'}}"
         else:
             return "null"
 
     @staticmethod
     def extract_string_value_from_attributes(attr_name, ce: CloudEvent) -> str:
         """
         Utility for extracting the String value of an attribute.<br><br>
-        @param attr_name:The name of the CloudEvent attribute.
-        @param ce:The CloudEvent containing the data.
-        @return:the Optional String value of an attribute matching the attribute name, or an Optional.empty() is the
+        @param
+        attr_name:The name of the CloudEvent attribute.
+        @param ce:The
+        CloudEvent containing the data.
+        @return:the Optional String value of an
+        attribute matching the attribute name, or an Optional.empty() is the
         value does not exist.
         """
 
         return ce.get_attributes().get(attr_name)
 
     @staticmethod
-    def extract_integer_value_from_attributes(attr_name, ce: CloudEvent) -> int:
+    def extract_integer_value_from_attributes(
+        attr_name, ce: CloudEvent
+    ) -> int:
         """
 
         Utility for extracting the Integer value of an attribute.<br><br>
         @param attr_name:The name of the CloudEvent attribute.
-        @param ce:The CloudEvent containing the data.
-        @return:returns the Optional Integer value of an attribute matching the attribute name,or an Optional.empty()
-        is the value does not exist.
+        @param ce:The
+        CloudEvent containing the data.
+        @return:returns the Optional Integer
+        value of an attribute matching the attribute name,or an
+        Optional.empty() is the value does not exist.
         """
         value = UCloudEvent.extract_string_value_from_attributes(attr_name, ce)
         return int(value) if value is not None else None
 
     @staticmethod
     def get_event_type(type):
-        return {UMessageType.UMESSAGE_TYPE_PUBLISH: "pub.v1", UMessageType.UMESSAGE_TYPE_REQUEST: "req.v1",
-                UMessageType.UMESSAGE_TYPE_RESPONSE: "res.v1"}.get(type, "")
+        """
+        Get the string representation of the UMessageType. Note: The
+        UMessageType is determined by the type of the CloudEvent. If the
+        UMessageType is UMESSAGE_TYPE_NOTIFICATION, we assume the CloudEvent
+        type is "pub.v1" and the sink is present.
+        @param type The UMessageType
+        @return returns the string representation of the UMessageType
+        """
+        return {
+            UMessageType.UMESSAGE_TYPE_PUBLISH: "pub.v1",
+            UMessageType.UMESSAGE_TYPE_REQUEST: "req.v1",
+            UMessageType.UMESSAGE_TYPE_RESPONSE: "res.v1",
+            UMessageType.UMESSAGE_TYPE_NOTIFICATION: "not.v1",
+        }.get(type, "")
 
     @staticmethod
     def get_message_type(ce_type):
-        return {"pub.v1": UMessageType.UMESSAGE_TYPE_PUBLISH, "req.v1": UMessageType.UMESSAGE_TYPE_REQUEST,
-                "res.v1": UMessageType.UMESSAGE_TYPE_RESPONSE}.get(ce_type, UMessageType.UMESSAGE_TYPE_UNSPECIFIED)
+        """
+        Get the UMessageType from the string representation. Note: The
+        UMessageType is determined by the type of the CloudEvent. If the
+        CloudEvent type is "pub.v1" and the sink is present, the UMessageType
+        is assumed to be UMESSAGE_TYPE_NOTIFICATION, this is because uProtocol
+        CloudEvent definition did not have an explicit notification type.
+        @param cloudEvent The CloudEvent containing the data.
+        @return returns
+        the UMessageType
+        """
+        return {
+            "pub.v1": UMessageType.UMESSAGE_TYPE_PUBLISH,
+            "req.v1": UMessageType.UMESSAGE_TYPE_REQUEST,
+            "res.v1": UMessageType.UMESSAGE_TYPE_RESPONSE,
+        }.get(ce_type, UMessageType.UMESSAGE_TYPE_UNSPECIFIED)
 
     @staticmethod
     def get_content_type_from_upayload_format(payload_format: UPayloadFormat):
         """
-        Retrieves the string representation of the data content type based on the provided UPayloadFormat. <BR>
-        This method uses the uProtocol mimeType custom options declared in upayload.proto.
-        @param payload_format The UPayloadFormat enumeration representing the payload format.
-        @return The corresponding content type string based on the payload format.
+        Retrieves the string representation of the data content type based on
+        the provided UPayloadFormat. <BR> This method uses the uProtocol
+        mimeType custom options declared in upayload.proto.
+        @param
+        payload_format The UPayloadFormat enumeration representing the payload
+        format.
+        @return The corresponding content type string based on the
+        payload format.
         """
         return {
             UPayloadFormat.UPAYLOAD_FORMAT_JSON: "application/json",
             UPayloadFormat.UPAYLOAD_FORMAT_RAW: "application/octet-stream",
             UPayloadFormat.UPAYLOAD_FORMAT_TEXT: "text/plain",
             UPayloadFormat.UPAYLOAD_FORMAT_SOMEIP: "application/x-someip",
             UPayloadFormat.UPAYLOAD_FORMAT_SOMEIP_TLV: "application/x-someip_tlv",
         }.get(payload_format, "")
 
     @staticmethod
     def get_upayload_format_from_content_type(contenttype: str):
         """
-        Retrieves the payload format enumeration based on the provided string representation of the data content type <br>
-        This method uses the uProtocol mimeType custom options declared in upayload.proto.
-        @param contentType The content type string representing the format of the payload.
-        @return The corresponding UPayloadFormat enumeration based on the content type.
+        Retrieves the payload format enumeration based on the provided string
+        representation of the data content type <br> This method uses the
+        uProtocol mimeType custom options declared in upayload.proto.
+        @param
+        contentType The content type string representing the format of the
+        payload.
+        @return The corresponding UPayloadFormat enumeration based on
+        the content type.
         """
         if contenttype is None:
             return UPayloadFormat.UPAYLOAD_FORMAT_PROTOBUF_WRAPPED_IN_ANY
 
         content_type_mapping = {
             "application/json": UPayloadFormat.UPAYLOAD_FORMAT_JSON,
             "application/octet-stream": UPayloadFormat.UPAYLOAD_FORMAT_RAW,
             "text/plain": UPayloadFormat.UPAYLOAD_FORMAT_TEXT,
             "application/x-someip": UPayloadFormat.UPAYLOAD_FORMAT_SOMEIP,
             "application/x-someip_tlv": UPayloadFormat.UPAYLOAD_FORMAT_SOMEIP_TLV,
         }
-        return content_type_mapping.get(contenttype, UPayloadFormat.UPAYLOAD_FORMAT_PROTOBUF)
+        return content_type_mapping.get(
+            contenttype, UPayloadFormat.UPAYLOAD_FORMAT_PROTOBUF
+        )
 
     @staticmethod
     def fromMessage(message: UMessage) -> CloudEvent:
         """
         Get the Cloudevent from the UMessage<br>
-        <b>Note: For now, only the value format of UPayload is supported in the SDK.If the UPayload has a reference, it
+        <b>Note: For now, only the value format of
+        UPayload is supported in the SDK.If the UPayload has a reference, it
         needs to be copied to CloudEvent.</b>
         @param message The UMessage protobuf containing the data
         @return returns the cloud event
         """
 
+        if message is None:
+            raise ValueError("message cannot be null.")
+
         attributes = message.attributes
         payload = message.payload
 
         if attributes is None:
             attributes = UAttributes()
         if payload is None:
             payload = UPayload()
 
         data = bytearray()
-        json_attributes = {"id": LongUuidSerializer.instance().serialize(attributes.id),
-                           "source": LongUriSerializer().serialize(message.attributes.source),
-                           "type": UCloudEvent.get_event_type(attributes.type)}
-        contenttype = UCloudEvent.get_content_type_from_upayload_format(payload.format)
+        json_attributes = {
+            "id": LongUuidSerializer.instance().serialize(attributes.id),
+            "source": LongUriSerializer().serialize(message.attributes.source),
+            "type": UCloudEvent.get_event_type(attributes.type),
+        }
+        contenttype = UCloudEvent.get_content_type_from_upayload_format(
+            payload.format
+        )
 
         if contenttype:
-            json_attributes['datacontenttype'] = "application/x-protobuf"
+            json_attributes["datacontenttype"] = "application/x-protobuf"
 
         # IMPORTANT: Currently, ONLY the VALUE format is supported in the SDK!
-        if payload.HasField('value'):
+        if payload.HasField("value"):
             data = payload.value
-        if attributes.HasField('ttl'):
-            json_attributes['ttl'] = attributes.ttl
+        if attributes.HasField("ttl"):
+            json_attributes["ttl"] = attributes.ttl
         if attributes.priority > 0:
-            json_attributes['priority'] = UPriority.Name(attributes.priority)
-        if attributes.HasField('token'):
-            json_attributes['token'] = attributes.token
-        if attributes.HasField('sink'):
-            json_attributes['sink'] = LongUriSerializer().serialize(attributes.sink)
-        if attributes.HasField('commstatus'):
-            json_attributes['commstatus'] = attributes.commstatus
-        if attributes.HasField('reqid'):
-            json_attributes['reqid'] = LongUuidSerializer.instance().serialize(attributes.reqid)
-        if attributes.HasField('permission_level'):
-            json_attributes['plevel'] = attributes.permission_level
+            json_attributes["priority"] = UPriority.Name(attributes.priority)
+        if attributes.HasField("token"):
+            json_attributes["token"] = attributes.token
+        if attributes.HasField("sink"):
+            json_attributes["sink"] = LongUriSerializer().serialize(
+                attributes.sink
+            )
+        if attributes.HasField("commstatus"):
+            json_attributes["commstatus"] = attributes.commstatus
+        if attributes.HasField("reqid"):
+            json_attributes["reqid"] = LongUuidSerializer.instance().serialize(
+                attributes.reqid
+            )
+        if attributes.HasField("permission_level"):
+            json_attributes["plevel"] = attributes.permission_level
+        if attributes.HasField("traceparent"):
+            json_attributes["traceparent"] = attributes.traceparent
 
         cloud_event = CloudEvent(json_attributes, data)
         return cloud_event
 
     @staticmethod
     def toMessage(event: CloudEvent) -> UMessage:
         """
 
-         Get the UMessage from the cloud event
-         @param event The CloudEvent containing the data.
-         @return returns the UMessage
+        Get the UMessage from the cloud event
+        @param event The CloudEvent containing the data.
+        @return returns the UMessage
         """
         if event is None:
             raise ValueError("Cloud Event can't be None")
 
         payload = UPayload(
-            format=UCloudEvent.get_upayload_format_from_content_type(UCloudEvent.get_data_content_type(event)),
-            value=UCloudEvent.get_payload(event).SerializeToString())
-        attributes = UAttributes(id=LongUuidSerializer.instance().deserialize(UCloudEvent.get_id(event)),
-                                 type=UCloudEvent.get_message_type(UCloudEvent.get_type(event)),
-                                 source=LongUriSerializer().deserialize(UCloudEvent.get_source(event)))
+            format=UCloudEvent.get_upayload_format_from_content_type(
+                UCloudEvent.get_data_content_type(event)
+            ),
+            value=UCloudEvent.get_payload(event).SerializeToString(),
+        )
+        attributes = UAttributes(
+            id=LongUuidSerializer.instance().deserialize(
+                UCloudEvent.get_id(event)
+            ),
+            type=UCloudEvent.get_message_type(UCloudEvent.get_type(event)),
+            source=LongUriSerializer().deserialize(
+                UCloudEvent.get_source(event)
+            ),
+        )
         if UCloudEvent.has_communication_status_problem(event):
             attributes.commstatus = UCloudEvent.get_communication_status(event)
         priority = UCloudEvent.get_priority(event)
 
-        if priority and 'UPRIORITY_' not in priority:
-            priority = 'UPRIORITY_' + priority
+        if priority and "UPRIORITY_" not in priority:
+            priority = "UPRIORITY_" + priority
 
         if priority is not None:
             attributes.priority = priority
 
         sink = UCloudEvent.get_sink(event)
         if sink is not None:
             attributes.sink.CopyFrom(LongUriSerializer().deserialize(sink))
@@ -489,12 +655,18 @@
         if ttl is not None:
             attributes.ttl = ttl
 
         token = UCloudEvent.get_token(event)
         if token is not None:
             attributes.token = token
 
-        plevel = UCloudEvent.extract_integer_value_from_attributes("plevel", event)
+        traceparent = UCloudEvent.get_traceparent(event)
+        if traceparent is not None:
+            attributes.traceparent = traceparent
+
+        plevel = UCloudEvent.extract_integer_value_from_attributes(
+            "plevel", event
+        )
         if plevel is not None:
             attributes.permission_level = plevel
 
         return UMessage(attributes=attributes, payload=payload)
```

### Comparing `up_python-0.1.1.dev0/uprotocol/cloudevent/serialize/base64protobufserializer.py` & `up_python-0.1.2.dev0/uprotocol/cloudevent/serialize/base64protobufserializer.py`

 * *Files identical despite different names*

### Comparing `up_python-0.1.1.dev0/uprotocol/cloudevent/serialize/cloudeventserializer.py` & `up_python-0.1.2.dev0/uprotocol/cloudevent/serialize/cloudeventserializer.py`

 * *Files identical despite different names*

### Comparing `up_python-0.1.1.dev0/uprotocol/cloudevent/serialize/cloudeventserializers.py` & `up_python-0.1.2.dev0/uprotocol/cloudevent/serialize/cloudeventserializers.py`

 * *Files identical despite different names*

### Comparing `up_python-0.1.1.dev0/uprotocol/cloudevent/serialize/cloudeventtojsonserializer.py` & `up_python-0.1.2.dev0/uprotocol/cloudevent/serialize/cloudeventtojsonserializer.py`

 * *Files identical despite different names*

### Comparing `up_python-0.1.1.dev0/uprotocol/cloudevent/serialize/cloudeventtoprotobufserializer.py` & `up_python-0.1.2.dev0/uprotocol/cloudevent/serialize/cloudeventtoprotobufserializer.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,15 +22,17 @@
 # SPDX-License-Identifier: Apache-2.0
 #
 # -------------------------------------------------------------------------
 
 
 from cloudevents.http import CloudEvent
 
-from uprotocol.cloudevent.serialize.cloudeventserializer import CloudEventSerializer
+from uprotocol.cloudevent.serialize.cloudeventserializer import (
+    CloudEventSerializer,
+)
 from uprotocol.cloudevent import cloudevents_pb2
 
 
 # ToDo- convert cloud event to cloudevent proto
 class CloudEventToProtobufSerializer(CloudEventSerializer):
     """
     CloudEventSerializer to serialize and deserialize CloudEvents to protobuf format.
@@ -38,23 +40,22 @@
 
     def __init__(self):
         pass
 
     def serialize(self, http_event: CloudEvent) -> bytes:
         proto_event = cloudevents_pb2.CloudEvent()
         # Set required attributes
-        proto_event.id = http_event['id']
-        proto_event.source = http_event['source']
-        proto_event.spec_version = http_event['specversion']
-        proto_event.type = http_event['type']
-
+        proto_event.id = http_event["id"]
+        proto_event.source = http_event["source"]
+        proto_event.spec_version = http_event["specversion"]
+        proto_event.type = http_event["type"]
 
         # Set optional & extension attributes
         for key, value in http_event.get_attributes().items():
-            if key not in ['specversion', 'id', 'source', 'type',  'data']:
+            if key not in ["specversion", "id", "source", "type", "data"]:
                 attribute_value = proto_event.attributes[key]
                 if isinstance(value, bool):
                     attribute_value.ce_boolean = value
                 elif isinstance(value, int):
                     attribute_value.ce_integer = value
                 elif isinstance(value, str):
                     attribute_value.ce_string = value
@@ -70,35 +71,37 @@
 
         return proto_event.SerializeToString()
 
     def deserialize(self, bytes_data: bytes) -> CloudEvent:
         proto_event = cloudevents_pb2.CloudEvent()
         proto_event.ParseFromString(bytes_data)
 
-        json_attributes = {"id": proto_event.id, "source": proto_event.source, "type": proto_event.type,
-                           "specversion": proto_event.spec_version}
-
-
+        json_attributes = {
+            "id": proto_event.id,
+            "source": proto_event.source,
+            "type": proto_event.type,
+            "specversion": proto_event.spec_version,
+        }
 
         # Set optional & extension attributes
         for key in proto_event.attributes:
-            if key not in ['specversion', 'id', 'source', 'type', 'data']:
+            if key not in ["specversion", "id", "source", "type", "data"]:
                 attribute_value = proto_event.attributes[key]
-                if attribute_value.HasField('ce_boolean'):
+                if attribute_value.HasField("ce_boolean"):
                     json_attributes[key] = attribute_value.ce_boolean
-                elif attribute_value.HasField('ce_integer'):
+                elif attribute_value.HasField("ce_integer"):
                     json_attributes[key] = attribute_value.ce_integer
-                elif attribute_value.HasField('ce_string'):
+                elif attribute_value.HasField("ce_string"):
                     json_attributes[key] = attribute_value.ce_string
-                elif attribute_value.HasField('ce_bytes'):
+                elif attribute_value.HasField("ce_bytes"):
                     json_attributes[key] = attribute_value.ce_bytes
 
         # Set data
         data = bytearray()
-        if proto_event.HasField('binary_data'):
+        if proto_event.HasField("binary_data"):
             data = proto_event.binary_data
-        elif proto_event.HasField('text_data'):
+        elif proto_event.HasField("text_data"):
             data = proto_event.text_data
 
         cloud_event = CloudEvent(json_attributes, data)
 
         return cloud_event
```

### Comparing `up_python-0.1.1.dev0/uprotocol/cloudevent/validate/cloudeventvalidator.py` & `up_python-0.1.2.dev0/uprotocol/cloudevent/validate/cloudeventvalidator.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,277 +39,379 @@
 
 
 class CloudEventValidator(ABC):
 
     @staticmethod
     def get_validator(ce: CloudEvent):
         """
-        Obtain a CloudEventValidator according to the type attribute in the CloudEvent.<br><br>
+        Obtain a CloudEventValidator according to the type
+        attribute in the CloudEvent.<br><br>
         @param ce:The CloudEvent with the type attribute.
-        @return:Returns a CloudEventValidator according to the type attribute in the CloudEvent.
+        @return:Returns a CloudEventValidator according to the
+        type attribute in the CloudEvent.
         """
         cloud_event_type = ce.get_attributes().get("type")
 
-        if cloud_event_type is None or not cloud_event_type:
+        if cloud_event_type is None:
             return Validators.PUBLISH.validator()
 
         message_type = UCloudEvent.get_message_type(cloud_event_type)
 
         if message_type == UMessageType.UMESSAGE_TYPE_RESPONSE:
             return Validators.RESPONSE.validator()
         elif message_type == UMessageType.UMESSAGE_TYPE_REQUEST:
             return Validators.REQUEST.validator()
+        elif message_type == UMessageType.UMESSAGE_TYPE_NOTIFICATION:
+            return Validators.NOTIFICATION.validator()
         else:
             return Validators.PUBLISH.validator()
 
     def validate(self, ce: CloudEvent) -> ValidationResult:
         """
-        Validate the CloudEvent. A CloudEventValidator instance is obtained according to the type attribute on the
-        CloudEvent.<br><br>
-        @param ce:The CloudEvent to validate.
-        @return:Returns a ValidationResult with success or a ValidationResult with failure containing all the
-        errors that were found.
-        """
-        validation_results = [self.validate_version(ce), self.validate_id(ce), self.validate_source(ce),
-                              self.validate_type(ce), self.validate_sink(ce)]
-
-        error_messages = [result.get_message() for result in validation_results if not result.is_success()]
+        Validate the CloudEvent. A CloudEventValidator instance is obtained
+        according to the type attribute on the CloudEvent.<br><br> @param
+        ce:The CloudEvent to validate. @return:Returns a ValidationResult with
+        success or a ValidationResult with failure containing all the errors
+        that were found.
+        """
+        self.validate_source(ce)
+        validation_results = [
+            self.validate_version(ce),
+            self.validate_id(ce),
+            self.validate_source(ce),
+            self.validate_type(ce),
+            self.validate_sink(ce),
+        ]
+
+        error_messages = [
+            result.get_message()
+            for result in validation_results
+            if not result.is_success()
+        ]
         error_message = ",".join(error_messages)
 
         if not error_message:
             return ValidationResult.success()
         else:
             return ValidationResult.failure(",".join(error_messages))
 
     @staticmethod
     def validate_version(ce: CloudEvent) -> ValidationResult:
-        return CloudEventValidator.validate_version_spec(ce.get_attributes().get("specversion"))
+        return CloudEventValidator.validate_version_spec(
+            ce.get_attributes().get("specversion")
+        )
 
     @staticmethod
     def validate_version_spec(version) -> ValidationResult:
         if version == "1.0":
             return ValidationResult.success()
         else:
-            return ValidationResult.failure(f"Invalid CloudEvent version [{version}]. CloudEvent version must be 1.0.")
+            return ValidationResult.failure(
+                f"Invalid CloudEvent version [{version}]. CloudEvent version must be 1.0."
+            )
 
     @staticmethod
     def validate_id(ce: CloudEvent) -> ValidationResult:
         id = UCloudEvent.extract_string_value_from_attributes("id", ce)
-        return (ValidationResult.success() if UCloudEvent.is_cloud_event_id(ce) else ValidationResult.failure(
-            f"Invalid CloudEvent Id [{id}]. CloudEvent Id must be of type UUIDv8."))
+        return (
+            ValidationResult.success()
+            if UCloudEvent.is_cloud_event_id(ce)
+            else ValidationResult.failure(
+                f"Invalid CloudEvent Id [{id}]. CloudEvent Id must be of type UUIDv8."
+            )
+        )
 
     @abstractmethod
     def validate_source(self, ce: CloudEvent):
         """
         Validate the source value of a cloud event.<br><br>
-        @param ce:The cloud event containing the source to validate.
-        @return:Returns the ValidationResult containing a success or a failure with the error message.
+        @param ce:The cloud
+        event containing the source to validate.
+        @return:Returns the
+        ValidationResult containing a success or a failure with the error
+        message.
         """
         raise NotImplementedError("Subclasses must implement this method")
 
     @abstractmethod
     def validate_type(self, ce: CloudEvent):
         """
         Validate the type value of a cloud event.<br><br>
-        @param ce:The cloud event containing the type to validate.
-        @return:Returns the ValidationResult containing a success or a failure with the error message.
+        @param ce:The cloud
+        event containing the type to validate.
+        @return:Returns the
+        ValidationResult containing a success or a failure with the error
+        message.
         """
         raise NotImplementedError("Subclasses must implement this method")
 
     def validate_sink(self, ce: CloudEvent) -> ValidationResult:
         """
-        Validate the sink value of a cloud event in the default scenario where the sink attribute is optional.<br><br>
-        @param ce:The cloud event containing the sink to validate.
-        @return:Returns the ValidationResult containing a success or a failure with the error message.
+        Validate the sink value of a cloud event in the default scenario where
+        the sink attribute is optional.<br><br>
+        @param ce:The cloud event
+        containing the sink to validate.
+        @return:Returns the ValidationResult
+        containing a success or a failure with the error message.
         """
         maybe_sink = UCloudEvent.get_sink(ce)
         if maybe_sink:
             sink = maybe_sink
             check_sink = self.validate_u_entity_uri(sink)
             if check_sink.is_failure():
-                return ValidationResult.failure(f"Invalid CloudEvent sink [{sink}]. {check_sink.get_message()}")
+                return ValidationResult.failure(
+                    f"Invalid CloudEvent sink [{sink}]. {check_sink.get_message()}"
+                )
 
         return ValidationResult.success()
 
     @staticmethod
     def validate_u_entity_uri(uri: str) -> ValidationResult:
         """
-        Validate an  UriPart for an  Software Entity must have an authority in the case of a microRemote uri,
-        and must contain the name of the USE.<br><br>
+        Validate an  UriPart for an  Software Entity must have an authority in
+        the case of a microRemote uri, and must contain the name of the
+        USE.<br><br>
         @param uri:uri string to validate.
-        @return:Returns the ValidationResult containing a success or a failure with the error message.
+        @return:Returns the
+        ValidationResult containing a success or a failure with the error
+        message.
         """
         uri = LongUriSerializer().deserialize(uri)
         return CloudEventValidator.validate_u_entity_uri_from_UURI(uri)
 
     @staticmethod
     def validate_u_entity_uri_from_UURI(uri: UUri) -> ValidationResult:
         return UriValidator.validate(uri)
 
-
     @staticmethod
     def validate_topic_uri(uri: str) -> ValidationResult:
         """
-         Validate a UriPart that is to be used as a topic in publish scenarios for events such as publish,
-         file and notification.<br><br>
+        Validate a UriPart that is to be used as a topic in publish scenarios
+        for events such as publish, file and notification.<br><br>
         @param uri:String UriPart to validate
-        @return:Returns the ValidationResult containing a success or a failure with the error message.
+        @return:Returns the
+        ValidationResult containing a success or a failure with the error
+        message.
         """
         Uri = LongUriSerializer().deserialize(uri)
         return CloudEventValidator.validate_topic_uri_from_UURI(Uri)
 
     @staticmethod
     def validate_topic_uri_from_UURI(uri: UUri) -> ValidationResult:
         """
-        Validate a UriPart that is to be used as a topic in publish scenarios for events such as publish,
-        file and notification.<br><br>
-        @param uri: UriPart to validate.
-        @return:Returns the ValidationResult containing a success or a failure with the error message.
-        """
-        validationResult = CloudEventValidator.validate_u_entity_uri_from_UURI(uri)
+        Validate a UriPart that is to be used as a topic in publish scenarios
+        for events such as publish, file and notification.<br><br>
+        @param uri:
+        UriPart to validate.
+        @return:Returns the ValidationResult containing a
+        success or a failure with the error message.
+        """
+        validationResult = CloudEventValidator.validate_u_entity_uri_from_UURI(
+            uri
+        )
         if validationResult.is_failure():
             return validationResult
 
         u_resource = uri.resource
         if not u_resource.name:
-            return ValidationResult.failure("UriPart is missing uResource name.")
+            return ValidationResult.failure(
+                "UriPart is missing uResource name."
+            )
 
         if not u_resource.message:
-            return ValidationResult.failure("UriPart is missing Message information.")
+            return ValidationResult.failure(
+                "UriPart is missing Message information."
+            )
 
         return ValidationResult.success()
 
     @staticmethod
     def validate_rpc_topic_uri(uri: str) -> ValidationResult:
         """
-        Validate a UriPart that is meant to be used as the application response topic for rpc calls. <br>Used in
-        Request source values and Response sink values.<br><br>
+        Validate a UriPart that is meant to be used as the application response
+        topic for rpc calls. <br>Used in Request source values and Response
+        sink values.<br><br>
         @param uri:String UriPart to validate.
-        @return:Returns the ValidationResult containing a success or a failure with the error message.
+        @return:Returns the ValidationResult containing a success or a failure
+        with the error message.
         """
         Uri = LongUriSerializer().deserialize(uri)
         return CloudEventValidator.validate_rpc_topic_uri_from_uuri(Uri)
 
     @staticmethod
     def validate_rpc_topic_uri_from_uuri(uri: UUri) -> ValidationResult:
         """
-        Validate a UriPart that is meant to be used as the application response topic for rpc calls. <br>Used in
-        Request source values and Response sink values.<br><br>
+        Validate a UriPart that is meant to be used as the application response
+        topic for rpc calls. <br>Used in Request source values and Response
+        sink values.<br><br>
         @param uri:UriPart to validate.
-        @return:Returns the ValidationResult containing a success or a failure with the error message.
-        """
-        validationResult = CloudEventValidator.validate_u_entity_uri_from_UURI(uri)
+        @return:Returns
+        the ValidationResult containing a success or a failure with the error
+        message.
+        """
+        validationResult = CloudEventValidator.validate_u_entity_uri_from_UURI(
+            uri
+        )
         if validationResult.is_failure():
             return ValidationResult.failure(
-                f"Invalid RPC uri application response topic. {validationResult.get_message()}")
+                f"Invalid RPC uri application response topic. {validationResult.get_message()}",
+            )
 
         u_resource = uri.resource
-        topic = f"{u_resource.name}.{u_resource.instance}" if u_resource.instance else f"{u_resource.name}"
+        topic = (
+            f"{u_resource.name}.{u_resource.instance}"
+            if u_resource.instance
+            else f"{u_resource.name}"
+        )
         if topic != "rpc.response":
-            return ValidationResult.failure("Invalid RPC uri application response topic. UriPart is missing rpc.response.")
+            return ValidationResult.failure(
+                "Invalid RPC uri application response topic. UriPart is missing rpc.response.",
+            )
 
         return ValidationResult.success()
 
     @staticmethod
     def validate_rpc_method(uri: str) -> ValidationResult:
         """
         Validate a UriPart that is meant to be used as an RPC method URI. Used in Request sink values and Response
         source values.<br><br>
         @param uri: String UriPart to validate
         @return:Returns the ValidationResult containing a success or a failure with the error message.
         """
         uuri = LongUriSerializer().deserialize(uri)
-        validationResult = CloudEventValidator.validate_u_entity_uri_from_UURI(uuri)
+        validationResult = CloudEventValidator.validate_u_entity_uri_from_UURI(
+            uuri
+        )
         if validationResult.is_failure():
-            return ValidationResult.failure(f"Invalid RPC method uri. {validationResult.get_message()}")
+            return ValidationResult.failure(
+                f"Invalid RPC method uri. {validationResult.get_message()}"
+            )
 
         if not UriValidator.is_rpc_method(uuri):
             return ValidationResult.failure(
-                "Invalid RPC method uri. UriPart should be the method to be called, or method from response.")
+                "Invalid RPC method uri. UriPart should be the method to be called, or method from response.",
+            )
 
         return ValidationResult.success()
 
 
 class Publish(CloudEventValidator):
     """
     Implements Validations for a CloudEvent of type Publish.
     """
 
     def validate_source(self, cl_event: CloudEvent) -> ValidationResult:
         source = cl_event.get_attributes().get("source")
         check_source = self.validate_topic_uri(source)
         if check_source.is_failure():
             return ValidationResult.failure(
-                f"Invalid Publish type CloudEvent source [{source}]. {check_source.get_message()}")
+                f"Invalid Publish type CloudEvent source [{source}]. {check_source.get_message()}",
+            )
 
         return ValidationResult.success()
 
     def validate_type(self, cl_event: CloudEvent) -> ValidationResult:
         type = cl_event.get_attributes().get("type")
-        return (ValidationResult.success() if type == "pub.v1" else ValidationResult.failure(
-            f"Invalid CloudEvent type [{type}]. CloudEvent of type Publish must have a type of 'pub.v1'"))
+        return (
+            ValidationResult.success()
+            if type == "pub.v1"
+            else ValidationResult.failure(
+                f"Invalid CloudEvent type [{type}]. CloudEvent of type Publish must have a type of 'pub.v1'",
+            )
+        )
 
     def __str__(self) -> str:
         return "CloudEventValidator.Publish"
 
 
 class Notification(Publish):
     """
-    Implements Validations for a CloudEvent of type Publish that behaves as a Notification, meaning it must have a sink.
+    Implements Validations for a CloudEvent of type Publish that behaves as a
+    Notification, meaning it must have a sink.
     """
 
     def validate_sink(self, cl_event: CloudEvent) -> ValidationResult:
         maybe_sink = UCloudEvent.get_sink(cl_event)
         if not maybe_sink:
-            return ValidationResult.failure("Invalid CloudEvent sink. Notification CloudEvent sink must be an  uri.")
+            return ValidationResult.failure(
+                "Invalid CloudEvent sink. Notification CloudEvent sink must be an  uri.",
+            )
         else:
             sink = maybe_sink
             check_sink = self.validate_u_entity_uri(sink)
             if check_sink.is_failure():
                 return ValidationResult.failure(
-                    f"Invalid Notification type CloudEvent sink [{sink}]. {check_sink.get_message()}")
+                    f"Invalid Notification type CloudEvent sink [{sink}]. {check_sink.get_message()}",
+                )
+
+        return ValidationResult.success()
 
+    def validate_source(self, cl_event: CloudEvent) -> ValidationResult:
+        source = UCloudEvent.get_source(cl_event)
+        check_source = self.validate_topic_uri(source)
+        if check_source.is_failure():
+            return ValidationResult.failure(
+                f"Invalid Notification type CloudEvent source [{source}], {check_source.get_message()}",
+            )
         return ValidationResult.success()
 
+    def validate_type(self, cl_event: CloudEvent) -> ValidationResult:
+        return (
+            ValidationResult.success()
+            if UCloudEvent.get_type(cl_event) == "not.v1"
+            else ValidationResult.failure(
+                f"Invalid CloudEvent type [{UCloudEvent.get_type(cl_event)}]. " +
+                "CloudEvent of type Notification must have a type of 'not.v1'",
+            )
+        )
+
     def __str__(self):
         return "CloudEventValidator.Notification"
 
 
 class Request(CloudEventValidator):
     """
     Implements Validations for a CloudEvent for RPC Request.
     """
 
     def validate_source(self, cl_event: CloudEvent) -> ValidationResult:
         source = cl_event.get_attributes().get("source")
         check_source = self.validate_rpc_topic_uri(source)
         if check_source.is_failure():
             return ValidationResult.failure(
-                f"Invalid RPC Request CloudEvent source [{source}]. {check_source.get_message()}")
+                f"Invalid RPC Request CloudEvent source [{source}]. {check_source.get_message()}",
+            )
         return ValidationResult.success()
 
     def validate_sink(self, cl_event: CloudEvent) -> ValidationResult:
         maybe_sink = UCloudEvent.get_sink(cl_event)
         if not maybe_sink:
             return ValidationResult.failure(
-                "Invalid RPC Request CloudEvent sink. Request CloudEvent sink must be uri for the method to be called.")
+                "Invalid RPC Request CloudEvent sink. Request CloudEvent sink must be uri for the method to be called."
+            )
         else:
             sink = maybe_sink
             check_sink = self.validate_rpc_method(sink)
             if check_sink.is_failure():
                 return ValidationResult.failure(
-                    f"Invalid RPC Request CloudEvent sink [{sink}]. {check_sink.get_message()}")
+                    f"Invalid RPC Request CloudEvent sink [{sink}]. {check_sink.get_message()}",
+                )
 
         return ValidationResult.success()
 
     def validate_type(self, cl_event: CloudEvent) -> ValidationResult:
         type = cl_event.get_attributes().get("type")
 
-        return (ValidationResult.success() if type == "req.v1" else ValidationResult.failure(
-            f"Invalid CloudEvent type [{type}]. CloudEvent of type Request must have a type of 'req.v1'"))
+        return (
+            ValidationResult.success()
+            if type == "req.v1"
+            else ValidationResult.failure(
+                f"Invalid CloudEvent type [{type}]. CloudEvent of type Request must have a type of 'req.v1'",
+            )
+        )
 
     def __str__(self):
         return "CloudEventValidator.Request"
 
 
 class Response(CloudEventValidator):
     """
@@ -317,46 +419,56 @@
     """
 
     def validate_source(self, cl_event: CloudEvent) -> ValidationResult:
         source = cl_event.get_attributes().get("source")
         check_source = self.validate_rpc_method(source)
         if check_source.is_failure():
             return ValidationResult.failure(
-                f"Invalid RPC Response CloudEvent source [{source}]. {check_source.get_message()}")
+                f"Invalid RPC Response CloudEvent source [{source}]. {check_source.get_message()}",
+            )
 
         return ValidationResult.success()
 
     def validate_sink(self, cl_event) -> ValidationResult:
         maybe_sink = UCloudEvent.get_sink(cl_event)
         if not maybe_sink:
             return ValidationResult.failure(
-                "Invalid CloudEvent sink. Response CloudEvent sink must be uri the destination of the response.")
+                "Invalid CloudEvent sink. Response CloudEvent sink must be uri the destination of the response.",
+            )
         else:
             sink = maybe_sink
             check_sink = self.validate_rpc_topic_uri(sink)
             if check_sink.is_failure():
                 return ValidationResult.failure(
-                    f"Invalid RPC Response CloudEvent sink [{sink}]. {check_sink.get_message()}")
+                    f"Invalid RPC Response CloudEvent sink [{sink}]. {check_sink.get_message()}",
+                )
 
         return ValidationResult.success()
 
     def validate_type(self, cl_event: CloudEvent) -> ValidationResult:
         type = cl_event.get_attributes().get("type")
 
-        return (ValidationResult.success() if type == "res.v1" else ValidationResult.failure(
-            f"Invalid CloudEvent type [{type}]. CloudEvent of type Response must have a type of 'res.v1'"))
+        return (
+            ValidationResult.success()
+            if type == "res.v1"
+            else ValidationResult.failure(
+                f"Invalid CloudEvent type [{type}]. CloudEvent of type Response must have a type of 'res.v1'",
+            )
+        )
 
     def __str__(self):
         return "CloudEventValidator.Response"
 
 
 class Validators(Enum):
     """
-     Enum that hold the implementations of CloudEventValidator according to type.
+    Enum that hold the implementations of CloudEventValidator according to
+    type.
     """
+
     PUBLISH = Publish()
     NOTIFICATION = Notification()
     REQUEST = Request()
     RESPONSE = Response()
 
     def __init__(self, cloud_event_validator: CloudEventValidator):
         self.cloud_event_validator = cloud_event_validator
```

### Comparing `up_python-0.1.1.dev0/uprotocol/proto/core/udiscovery/v3/udiscovery_pb2.py` & `up_python-0.1.2.dev0/uprotocol/proto/core/udiscovery/v3/udiscovery_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,52 +13,52 @@
 
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 import uprotocol.proto.uprotocol_options_pb2 as uprotocol__options__pb2
 import uprotocol.proto.uri_pb2 as uri__pb2
 import uprotocol.proto.ustatus_pb2 as ustatus__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#core/udiscovery/v3/udiscovery.proto\x12\x1cuprotocol.core.udiscovery.v3\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17uprotocol_options.proto\x1a\turi.proto\x1a\rustatus.proto\"\xd8\x01\n\rPropertyValue\x12\x13\n\tu_boolean\x18\x01 \x01(\x08H\x00\x12\x13\n\tu_integer\x18\x02 \x01(\x05H\x00\x12\x12\n\x08u_string\x18\x03 \x01(\tH\x00\x12\x11\n\x07u_bytes\x18\x04 \x01(\x0cH\x00\x12\x0f\n\x05u_uri\x18\x05 \x01(\tH\x00\x12\x31\n\x0bu_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x12\x12\n\x08u_double\x18\x07 \x01(\x01H\x00\x12\x16\n\x0cu_integer_64\x18\x08 \x01(\x03H\x00\x42\x06\n\x04\x61ttr\"\xac\x03\n\x04Node\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x31\n\x05nodes\x18\x02 \x03(\x0b\x32\".uprotocol.core.udiscovery.v3.Node\x12\x46\n\nproperties\x18\x03 \x03(\x0b\x32\x32.uprotocol.core.udiscovery.v3.Node.PropertiesEntry\x12\x35\n\x04type\x18\x04 \x01(\x0e\x32\'.uprotocol.core.udiscovery.v3.Node.Type\x1a^\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12:\n\x05value\x18\x02 \x01(\x0b\x32+.uprotocol.core.udiscovery.v3.PropertyValue:\x02\x38\x01\"\x84\x01\n\x04Type\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x44OMAIN\x10\x01\x12\n\n\x06\x44\x45VICE\x10\x02\x12\n\n\x06\x45NTITY\x10\x03\x12\x0b\n\x07VERSION\x10\t\x12\t\n\x05TOPIC\x10\x04\x12\n\n\x06METHOD\x10\x05\x12\x0b\n\x07MESSAGE\x10\x06\x12\x0c\n\x08RESOURCE\x10\x07\x12\x08\n\x04USER\x10\x08\"_\n\x11UpdateNodeRequest\x12\x30\n\x04node\x18\x01 \x01(\x0b\x32\".uprotocol.core.udiscovery.v3.Node\x12\x10\n\x03ttl\x18\x03 \x01(\x05H\x00\x88\x01\x01\x42\x06\n\x04_ttl\"\"\n\x12\x44\x65leteNodesRequest\x12\x0c\n\x04uris\x18\x01 \x03(\t\"=\n\x10\x46indNodesRequest\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x12\n\x05\x64\x65pth\x18\x02 \x01(\x05H\x00\x88\x01\x01\x42\x08\n\x06_depth\"\x87\x01\n\x11\x46indNodesResponse\x12\x31\n\x05nodes\x18\x01 \x03(\x0b\x32\".uprotocol.core.udiscovery.v3.Node\x12%\n\x06status\x18\x02 \x01(\x0b\x32\x15.uprotocol.v1.UStatus\x12\x10\n\x03ttl\x18\x03 \x01(\x05H\x00\x88\x01\x01\x42\x06\n\x04_ttl\"<\n\x19\x46indNodePropertiesRequest\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x12\n\nproperties\x18\x02 \x03(\t\"\x81\x02\n\x1a\x46indNodePropertiesResponse\x12\\\n\nproperties\x18\x01 \x03(\x0b\x32H.uprotocol.core.udiscovery.v3.FindNodePropertiesResponse.PropertiesEntry\x12%\n\x06status\x18\x02 \x01(\x0b\x32\x15.uprotocol.v1.UStatus\x1a^\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12:\n\x05value\x18\x02 \x01(\x0b\x32+.uprotocol.core.udiscovery.v3.PropertyValue:\x02\x38\x01\"X\n\x0f\x41\x64\x64NodesRequest\x12\x12\n\nparent_uri\x18\x01 \x01(\t\x12\x31\n\x05nodes\x18\x02 \x03(\x0b\x32\".uprotocol.core.udiscovery.v3.Node\"r\n\x15UpdatePropertyRequest\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x10\n\x08property\x18\x02 \x01(\t\x12:\n\x05value\x18\x03 \x01(\x0b\x32+.uprotocol.core.udiscovery.v3.PropertyValue\"\xf9\x01\n\x0cNotification\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x17\n\nparent_uri\x18\x02 \x01(\tH\x00\x88\x01\x01\x12G\n\toperation\x18\x03 \x01(\x0e\x32\x34.uprotocol.core.udiscovery.v3.Notification.Operation\x12\x10\n\x03ttl\x18\x04 \x01(\x05H\x01\x88\x01\x01\"9\n\tOperation\x12\x0b\n\x07INVALID\x10\x00\x12\n\n\x06UPDATE\x10\x01\x12\x07\n\x03\x41\x44\x44\x10\x02\x12\n\n\x06REMOVE\x10\x03\"\x16\n\tResources\x12\t\n\x05nodes\x10\x00\x42\r\n\x0b_parent_uriB\x06\n\x04_ttl\"\x1b\n\x0cObserverInfo\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\x80\x01\n\x14NotificationsRequest\x12\x0c\n\x04uris\x18\x01 \x03(\t\x12<\n\x08observer\x18\x02 \x01(\x0b\x32*.uprotocol.core.udiscovery.v3.ObserverInfo\x12\x12\n\x05\x64\x65pth\x18\x03 \x01(\x05H\x00\x88\x01\x01\x42\x08\n\x06_depth\"4\n\x11ResolveUriRequest\x12\x1f\n\x03uri\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUri\"\\\n\x12ResolveUriResponse\x12\x1f\n\x03uri\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUri\x12%\n\x06status\x18\x03 \x01(\x0b\x32\x15.uprotocol.v1.UStatus\"a\n\x11LookupUriResponse\x12%\n\x04uris\x18\x01 \x01(\x0b\x32\x17.uprotocol.v1.UUriBatch\x12%\n\x06status\x18\x02 \x01(\x0b\x32\x15.uprotocol.v1.UStatus\"r\n\x15NodeNotificationTopic\x12R\n\rresource_name\x18\x01 \x01(\x0e\x32\x34.uprotocol.core.udiscovery.v3.Notification.ResourcesB\x05\x82\xce\x18\x01*:\x05\xe0\xc7\x18\xe8\x07\x32\xd2\x08\n\nuDiscovery\x12V\n\tLookupUri\x12\x12.uprotocol.v1.UUri\x1a/.uprotocol.core.udiscovery.v3.LookupUriResponse\"\x04\xc0\xc1\x18\x01\x12Z\n\nUpdateNode\x12/.uprotocol.core.udiscovery.v3.UpdateNodeRequest\x1a\x15.uprotocol.v1.UStatus\"\x04\xc0\xc1\x18\x02\x12r\n\tFindNodes\x12..uprotocol.core.udiscovery.v3.FindNodesRequest\x1a/.uprotocol.core.udiscovery.v3.FindNodesResponse\"\x04\xc0\xc1\x18\x03\x12\x8d\x01\n\x12\x46indNodeProperties\x12\x37.uprotocol.core.udiscovery.v3.FindNodePropertiesRequest\x1a\x38.uprotocol.core.udiscovery.v3.FindNodePropertiesResponse\"\x04\xc0\xc1\x18\x04\x12\\\n\x0b\x44\x65leteNodes\x12\x30.uprotocol.core.udiscovery.v3.DeleteNodesRequest\x1a\x15.uprotocol.v1.UStatus\"\x04\xc0\xc1\x18\x05\x12V\n\x08\x41\x64\x64Nodes\x12-.uprotocol.core.udiscovery.v3.AddNodesRequest\x1a\x15.uprotocol.v1.UStatus\"\x04\xc0\xc1\x18\x06\x12\x62\n\x0eUpdateProperty\x12\x33.uprotocol.core.udiscovery.v3.UpdatePropertyRequest\x1a\x15.uprotocol.v1.UStatus\"\x04\xc0\xc1\x18\x07\x12k\n\x18RegisterForNotifications\x12\x32.uprotocol.core.udiscovery.v3.NotificationsRequest\x1a\x15.uprotocol.v1.UStatus\"\x04\xc0\xc1\x18\x08\x12m\n\x1aUnregisterForNotifications\x12\x32.uprotocol.core.udiscovery.v3.NotificationsRequest\x1a\x15.uprotocol.v1.UStatus\"\x04\xc0\xc1\x18\t\x12u\n\nResolveUri\x12/.uprotocol.core.udiscovery.v3.ResolveUriRequest\x1a\x30.uprotocol.core.udiscovery.v3.ResolveUriResponse\"\x04\xc0\xc1\x18\n\x1a\x1f\xa2\xbb\x18\x0f\x63ore.udiscovery\xa8\xbb\x18\x03\xb0\xbb\x18\x00\xb8\xbb\x18\x01\x42=\n(org.eclipse.uprotocol.core.udiscovery.v3B\x0fUDiscoveryProtoP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n#core/udiscovery/v3/udiscovery.proto\x12\x1cuprotocol.core.udiscovery.v3\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\x17uprotocol_options.proto\x1a\turi.proto\x1a\rustatus.proto\"\xd8\x01\n\rPropertyValue\x12\x13\n\tu_boolean\x18\x01 \x01(\x08H\x00\x12\x13\n\tu_integer\x18\x02 \x01(\x05H\x00\x12\x12\n\x08u_string\x18\x03 \x01(\tH\x00\x12\x11\n\x07u_bytes\x18\x04 \x01(\x0cH\x00\x12\x0f\n\x05u_uri\x18\x05 \x01(\tH\x00\x12\x31\n\x0bu_timestamp\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x00\x12\x12\n\x08u_double\x18\x07 \x01(\x01H\x00\x12\x16\n\x0cu_integer_64\x18\x08 \x01(\x03H\x00\x42\x06\n\x04\x61ttr\"\xac\x03\n\x04Node\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x31\n\x05nodes\x18\x02 \x03(\x0b\x32\".uprotocol.core.udiscovery.v3.Node\x12\x46\n\nproperties\x18\x03 \x03(\x0b\x32\x32.uprotocol.core.udiscovery.v3.Node.PropertiesEntry\x12\x35\n\x04type\x18\x04 \x01(\x0e\x32\'.uprotocol.core.udiscovery.v3.Node.Type\x1a^\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12:\n\x05value\x18\x02 \x01(\x0b\x32+.uprotocol.core.udiscovery.v3.PropertyValue:\x02\x38\x01\"\x84\x01\n\x04Type\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\n\n\x06\x44OMAIN\x10\x01\x12\n\n\x06\x44\x45VICE\x10\x02\x12\n\n\x06\x45NTITY\x10\x03\x12\x0b\n\x07VERSION\x10\t\x12\t\n\x05TOPIC\x10\x04\x12\n\n\x06METHOD\x10\x05\x12\x0b\n\x07MESSAGE\x10\x06\x12\x0c\n\x08RESOURCE\x10\x07\x12\x08\n\x04USER\x10\x08\"_\n\x11UpdateNodeRequest\x12\x30\n\x04node\x18\x01 \x01(\x0b\x32\".uprotocol.core.udiscovery.v3.Node\x12\x10\n\x03ttl\x18\x03 \x01(\x05H\x00\x88\x01\x01\x42\x06\n\x04_ttl\"\"\n\x12\x44\x65leteNodesRequest\x12\x0c\n\x04uris\x18\x01 \x03(\t\"=\n\x10\x46indNodesRequest\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x12\n\x05\x64\x65pth\x18\x02 \x01(\x05H\x00\x88\x01\x01\x42\x08\n\x06_depth\"\x87\x01\n\x11\x46indNodesResponse\x12\x31\n\x05nodes\x18\x01 \x03(\x0b\x32\".uprotocol.core.udiscovery.v3.Node\x12%\n\x06status\x18\x02 \x01(\x0b\x32\x15.uprotocol.v1.UStatus\x12\x10\n\x03ttl\x18\x03 \x01(\x05H\x00\x88\x01\x01\x42\x06\n\x04_ttl\"<\n\x19\x46indNodePropertiesRequest\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x12\n\nproperties\x18\x02 \x03(\t\"\x81\x02\n\x1a\x46indNodePropertiesResponse\x12\\\n\nproperties\x18\x01 \x03(\x0b\x32H.uprotocol.core.udiscovery.v3.FindNodePropertiesResponse.PropertiesEntry\x12%\n\x06status\x18\x02 \x01(\x0b\x32\x15.uprotocol.v1.UStatus\x1a^\n\x0fPropertiesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12:\n\x05value\x18\x02 \x01(\x0b\x32+.uprotocol.core.udiscovery.v3.PropertyValue:\x02\x38\x01\"X\n\x0f\x41\x64\x64NodesRequest\x12\x12\n\nparent_uri\x18\x01 \x01(\t\x12\x31\n\x05nodes\x18\x02 \x03(\x0b\x32\".uprotocol.core.udiscovery.v3.Node\"r\n\x15UpdatePropertyRequest\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x10\n\x08property\x18\x02 \x01(\t\x12:\n\x05value\x18\x03 \x01(\x0b\x32+.uprotocol.core.udiscovery.v3.PropertyValue\"\xf9\x01\n\x0cNotification\x12\x0b\n\x03uri\x18\x01 \x01(\t\x12\x17\n\nparent_uri\x18\x02 \x01(\tH\x00\x88\x01\x01\x12G\n\toperation\x18\x03 \x01(\x0e\x32\x34.uprotocol.core.udiscovery.v3.Notification.Operation\x12\x10\n\x03ttl\x18\x04 \x01(\x05H\x01\x88\x01\x01\"9\n\tOperation\x12\x0b\n\x07INVALID\x10\x00\x12\n\n\x06UPDATE\x10\x01\x12\x07\n\x03\x41\x44\x44\x10\x02\x12\n\n\x06REMOVE\x10\x03\"\x16\n\tResources\x12\t\n\x05nodes\x10\x00\x42\r\n\x0b_parent_uriB\x06\n\x04_ttl\"\x1b\n\x0cObserverInfo\x12\x0b\n\x03uri\x18\x01 \x01(\t\"\x80\x01\n\x14NotificationsRequest\x12\x0c\n\x04uris\x18\x01 \x03(\t\x12<\n\x08observer\x18\x02 \x01(\x0b\x32*.uprotocol.core.udiscovery.v3.ObserverInfo\x12\x12\n\x05\x64\x65pth\x18\x03 \x01(\x05H\x00\x88\x01\x01\x42\x08\n\x06_depth\"4\n\x11ResolveUriRequest\x12\x1f\n\x03uri\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUri\"\\\n\x12ResolveUriResponse\x12\x1f\n\x03uri\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUri\x12%\n\x06status\x18\x03 \x01(\x0b\x32\x15.uprotocol.v1.UStatus\"a\n\x11LookupUriResponse\x12%\n\x04uris\x18\x01 \x01(\x0b\x32\x17.uprotocol.v1.UUriBatch\x12%\n\x06status\x18\x02 \x01(\x0b\x32\x15.uprotocol.v1.UStatus\"r\n\x15NodeNotificationTopic\x12R\n\rresource_name\x18\x01 \x01(\x0e\x32\x34.uprotocol.core.udiscovery.v3.Notification.ResourcesB\x05\xc2\x8c\x19\x01*:\x05\xa0\x86\x19\xe8\x07\x32\xf4\x08\n\nuDiscovery\x12V\n\tLookupUri\x12\x12.uprotocol.v1.UUri\x1a/.uprotocol.core.udiscovery.v3.LookupUriResponse\"\x04\x80\x80\x19\x01\x12Z\n\nUpdateNode\x12/.uprotocol.core.udiscovery.v3.UpdateNodeRequest\x1a\x15.uprotocol.v1.UStatus\"\x04\x80\x80\x19\x02\x12r\n\tFindNodes\x12..uprotocol.core.udiscovery.v3.FindNodesRequest\x1a/.uprotocol.core.udiscovery.v3.FindNodesResponse\"\x04\x80\x80\x19\x03\x12\x8d\x01\n\x12\x46indNodeProperties\x12\x37.uprotocol.core.udiscovery.v3.FindNodePropertiesRequest\x1a\x38.uprotocol.core.udiscovery.v3.FindNodePropertiesResponse\"\x04\x80\x80\x19\x04\x12\\\n\x0b\x44\x65leteNodes\x12\x30.uprotocol.core.udiscovery.v3.DeleteNodesRequest\x1a\x15.uprotocol.v1.UStatus\"\x04\x80\x80\x19\x05\x12V\n\x08\x41\x64\x64Nodes\x12-.uprotocol.core.udiscovery.v3.AddNodesRequest\x1a\x15.uprotocol.v1.UStatus\"\x04\x80\x80\x19\x06\x12\x62\n\x0eUpdateProperty\x12\x33.uprotocol.core.udiscovery.v3.UpdatePropertyRequest\x1a\x15.uprotocol.v1.UStatus\"\x04\x80\x80\x19\x07\x12k\n\x18RegisterForNotifications\x12\x32.uprotocol.core.udiscovery.v3.NotificationsRequest\x1a\x15.uprotocol.v1.UStatus\"\x04\x80\x80\x19\x08\x12m\n\x1aUnregisterForNotifications\x12\x32.uprotocol.core.udiscovery.v3.NotificationsRequest\x1a\x15.uprotocol.v1.UStatus\"\x04\x80\x80\x19\t\x12u\n\nResolveUri\x12/.uprotocol.core.udiscovery.v3.ResolveUriRequest\x1a\x30.uprotocol.core.udiscovery.v3.ResolveUriResponse\"\x04\x80\x80\x19\n\x1a\x41\xe2\xf9\x18\x0f\x63ore.udiscovery\xe8\xf9\x18\x03\xf0\xf9\x18\x00\xf8\xf9\x18\x01\x92\xfa\x18\x1e\x08\x80\x80\x02\x12\nNodeChange\x1a\x0cNotificationB=\n(org.eclipse.uprotocol.core.udiscovery.v3B\x0fUDiscoveryProtoP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'core.udiscovery.v3.udiscovery_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n(org.eclipse.uprotocol.core.udiscovery.v3B\017UDiscoveryProtoP\001'
   _NODE_PROPERTIESENTRY._options = None
   _NODE_PROPERTIESENTRY._serialized_options = b'8\001'
   _FINDNODEPROPERTIESRESPONSE_PROPERTIESENTRY._options = None
   _FINDNODEPROPERTIESRESPONSE_PROPERTIESENTRY._serialized_options = b'8\001'
   _NODENOTIFICATIONTOPIC.fields_by_name['resource_name']._options = None
-  _NODENOTIFICATIONTOPIC.fields_by_name['resource_name']._serialized_options = b'\202\316\030\001*'
+  _NODENOTIFICATIONTOPIC.fields_by_name['resource_name']._serialized_options = b'\302\214\031\001*'
   _NODENOTIFICATIONTOPIC._options = None
-  _NODENOTIFICATIONTOPIC._serialized_options = b'\340\307\030\350\007'
+  _NODENOTIFICATIONTOPIC._serialized_options = b'\240\206\031\350\007'
   _UDISCOVERY._options = None
-  _UDISCOVERY._serialized_options = b'\242\273\030\017core.udiscovery\250\273\030\003\260\273\030\000\270\273\030\001'
+  _UDISCOVERY._serialized_options = b'\342\371\030\017core.udiscovery\350\371\030\003\360\371\030\000\370\371\030\001\222\372\030\036\010\200\200\002\022\nNodeChange\032\014Notification'
   _UDISCOVERY.methods_by_name['LookupUri']._options = None
-  _UDISCOVERY.methods_by_name['LookupUri']._serialized_options = b'\300\301\030\001'
+  _UDISCOVERY.methods_by_name['LookupUri']._serialized_options = b'\200\200\031\001'
   _UDISCOVERY.methods_by_name['UpdateNode']._options = None
-  _UDISCOVERY.methods_by_name['UpdateNode']._serialized_options = b'\300\301\030\002'
+  _UDISCOVERY.methods_by_name['UpdateNode']._serialized_options = b'\200\200\031\002'
   _UDISCOVERY.methods_by_name['FindNodes']._options = None
-  _UDISCOVERY.methods_by_name['FindNodes']._serialized_options = b'\300\301\030\003'
+  _UDISCOVERY.methods_by_name['FindNodes']._serialized_options = b'\200\200\031\003'
   _UDISCOVERY.methods_by_name['FindNodeProperties']._options = None
-  _UDISCOVERY.methods_by_name['FindNodeProperties']._serialized_options = b'\300\301\030\004'
+  _UDISCOVERY.methods_by_name['FindNodeProperties']._serialized_options = b'\200\200\031\004'
   _UDISCOVERY.methods_by_name['DeleteNodes']._options = None
-  _UDISCOVERY.methods_by_name['DeleteNodes']._serialized_options = b'\300\301\030\005'
+  _UDISCOVERY.methods_by_name['DeleteNodes']._serialized_options = b'\200\200\031\005'
   _UDISCOVERY.methods_by_name['AddNodes']._options = None
-  _UDISCOVERY.methods_by_name['AddNodes']._serialized_options = b'\300\301\030\006'
+  _UDISCOVERY.methods_by_name['AddNodes']._serialized_options = b'\200\200\031\006'
   _UDISCOVERY.methods_by_name['UpdateProperty']._options = None
-  _UDISCOVERY.methods_by_name['UpdateProperty']._serialized_options = b'\300\301\030\007'
+  _UDISCOVERY.methods_by_name['UpdateProperty']._serialized_options = b'\200\200\031\007'
   _UDISCOVERY.methods_by_name['RegisterForNotifications']._options = None
-  _UDISCOVERY.methods_by_name['RegisterForNotifications']._serialized_options = b'\300\301\030\010'
+  _UDISCOVERY.methods_by_name['RegisterForNotifications']._serialized_options = b'\200\200\031\010'
   _UDISCOVERY.methods_by_name['UnregisterForNotifications']._options = None
-  _UDISCOVERY.methods_by_name['UnregisterForNotifications']._serialized_options = b'\300\301\030\t'
+  _UDISCOVERY.methods_by_name['UnregisterForNotifications']._serialized_options = b'\200\200\031\t'
   _UDISCOVERY.methods_by_name['ResolveUri']._options = None
-  _UDISCOVERY.methods_by_name['ResolveUri']._serialized_options = b'\300\301\030\n'
+  _UDISCOVERY.methods_by_name['ResolveUri']._serialized_options = b'\200\200\031\n'
   _PROPERTYVALUE._serialized_start=154
   _PROPERTYVALUE._serialized_end=370
   _NODE._serialized_start=373
   _NODE._serialized_end=801
   _NODE_PROPERTIESENTRY._serialized_start=572
   _NODE_PROPERTIESENTRY._serialized_end=666
   _NODE_TYPE._serialized_start=669
@@ -96,9 +96,9 @@
   _RESOLVEURIRESPONSE._serialized_start=2131
   _RESOLVEURIRESPONSE._serialized_end=2223
   _LOOKUPURIRESPONSE._serialized_start=2225
   _LOOKUPURIRESPONSE._serialized_end=2322
   _NODENOTIFICATIONTOPIC._serialized_start=2324
   _NODENOTIFICATIONTOPIC._serialized_end=2438
   _UDISCOVERY._serialized_start=2441
-  _UDISCOVERY._serialized_end=3547
+  _UDISCOVERY._serialized_end=3581
 # @@protoc_insertion_point(module_scope)
```

### Comparing `up_python-0.1.1.dev0/uprotocol/proto/core/usubscription/v3/usubscription_pb2.py` & `up_python-0.1.2.dev0/uprotocol/proto/core/usubscription/v3/usubscription_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -14,92 +14,86 @@
 from google.protobuf import any_pb2 as google_dot_protobuf_dot_any__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 import uprotocol.proto.ustatus_pb2 as ustatus__pb2
 import uprotocol.proto.uri_pb2 as uri__pb2
 import uprotocol.proto.uprotocol_options_pb2 as uprotocol__options__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)core/usubscription/v3/usubscription.proto\x12\x1fuprotocol.core.usubscription.v3\x1a\x19google/protobuf/any.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\rustatus.proto\x1a\turi.proto\x1a\x17uprotocol_options.proto\"h\n\x13SubscribeAttributes\x12*\n\x06\x65xpire\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12%\n\x07\x64\x65tails\x18\x02 \x03(\x0b\x32\x14.google.protobuf.Any\"X\n\x0eSubscriberInfo\x12\x1f\n\x03uri\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUri\x12%\n\x07\x64\x65tails\x18\x02 \x03(\x0b\x32\x14.google.protobuf.Any\"\xed\x01\n\x12SubscriptionStatus\x12H\n\x05state\x18\x01 \x01(\x0e\x32\x39.uprotocol.core.usubscription.v3.SubscriptionStatus.State\x12!\n\x04\x63ode\x18\x02 \x01(\x0e\x32\x13.uprotocol.v1.UCode\x12\x0f\n\x07message\x18\x03 \x01(\t\"Y\n\x05State\x12\x10\n\x0cUNSUBSCRIBED\x10\x00\x12\x15\n\x11SUBSCRIBE_PENDING\x10\x01\x12\x0e\n\nSUBSCRIBED\x10\x02\x12\x17\n\x13UNSUBSCRIBE_PENDING\x10\x03\"\xd2\x01\n\x13\x45ventDeliveryConfig\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12X\n\nattributes\x18\x03 \x03(\x0b\x32\x44.uprotocol.core.usubscription.v3.EventDeliveryConfig.AttributesEntry\x1aG\n\x0f\x41ttributesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.google.protobuf.Any:\x02\x38\x01\"\xc7\x01\n\x13SubscriptionRequest\x12!\n\x05topic\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUri\x12\x43\n\nsubscriber\x18\x02 \x01(\x0b\x32/.uprotocol.core.usubscription.v3.SubscriberInfo\x12H\n\nattributes\x18\x03 \x01(\x0b\x32\x34.uprotocol.core.usubscription.v3.SubscribeAttributes\"\xc4\x01\n\x14SubscriptionResponse\x12\x43\n\x06status\x18\x01 \x01(\x0b\x32\x33.uprotocol.core.usubscription.v3.SubscriptionStatus\x12\x44\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x34.uprotocol.core.usubscription.v3.EventDeliveryConfig\x12!\n\x05topic\x18\x03 \x01(\x0b\x32\x12.uprotocol.v1.UUri\"|\n\x12UnsubscribeRequest\x12!\n\x05topic\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUri\x12\x43\n\nsubscriber\x18\x02 \x01(\x0b\x32/.uprotocol.core.usubscription.v3.SubscriberInfo\"\\\n\x17\x46\x65tchSubscribersRequest\x12!\n\x05topic\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUri\x12\x13\n\x06offset\x18\x02 \x01(\rH\x00\x88\x01\x01\x42\t\n\x07_offset\"\xbb\x01\n\x18\x46\x65tchSubscribersResponse\x12\x44\n\x0bsubscribers\x18\x01 \x03(\x0b\x32/.uprotocol.core.usubscription.v3.SubscriberInfo\x12\x1d\n\x10has_more_records\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12%\n\x06status\x18\x03 \x01(\x0b\x32\x15.uprotocol.v1.UStatusB\x13\n\x11_has_more_records\"\xcb\x02\n\x0cSubscription\x12!\n\x05topic\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUri\x12\x43\n\nsubscriber\x18\x02 \x01(\x0b\x32/.uprotocol.core.usubscription.v3.SubscriberInfo\x12\x43\n\x06status\x18\x03 \x01(\x0b\x32\x33.uprotocol.core.usubscription.v3.SubscriptionStatus\x12H\n\nattributes\x18\x04 \x01(\x0b\x32\x34.uprotocol.core.usubscription.v3.SubscribeAttributes\x12\x44\n\x06\x63onfig\x18\x05 \x01(\x0b\x32\x34.uprotocol.core.usubscription.v3.EventDeliveryConfig\"\xb2\x01\n\x19\x46\x65tchSubscriptionsRequest\x12#\n\x05topic\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUriH\x00\x12\x45\n\nsubscriber\x18\x02 \x01(\x0b\x32/.uprotocol.core.usubscription.v3.SubscriberInfoH\x00\x12\x13\n\x06offset\x18\x03 \x01(\rH\x01\x88\x01\x01\x42\t\n\x07requestB\t\n\x07_offset\"\xbd\x01\n\x1a\x46\x65tchSubscriptionsResponse\x12\x44\n\rsubscriptions\x18\x01 \x03(\x0b\x32-.uprotocol.core.usubscription.v3.Subscription\x12\x1d\n\x10has_more_records\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12%\n\x06status\x18\x03 \x01(\x0b\x32\x15.uprotocol.v1.UStatusB\x13\n\x11_has_more_records\"~\n\x14NotificationsRequest\x12!\n\x05topic\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUri\x12\x43\n\nsubscriber\x18\x02 \x01(\x0b\x32/.uprotocol.core.usubscription.v3.SubscriberInfo\"7\n\x12\x43reateTopicRequest\x12!\n\x05topic\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUri\":\n\x15\x44\x65precateTopicRequest\x12!\n\x05topic\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUri\"\x9f\x02\n\x06Update\x12!\n\x05topic\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUri\x12\x43\n\nsubscriber\x18\x02 \x01(\x0b\x32/.uprotocol.core.usubscription.v3.SubscriberInfo\x12\x43\n\x06status\x18\x03 \x01(\x0b\x32\x33.uprotocol.core.usubscription.v3.SubscriptionStatus\x12H\n\nattributes\x18\x04 \x01(\x0b\x32\x34.uprotocol.core.usubscription.v3.SubscribeAttributes\"\x1e\n\tResources\x12\x11\n\rsubscriptions\x10\x00\"x\n\x1eSubscriptionChangeNotification\x12O\n\rresource_name\x18\x01 \x01(\x0e\x32\x31.uprotocol.core.usubscription.v3.Update.ResourcesB\x05\x82\xce\x18\x01*:\x05\xe0\xc7\x18\xe8\x07\"\x1d\n\x0bPassiveMode\x12\x0e\n\x06\x65nable\x18\x01 \x01(\x08\"\xd6\x02\n\x0cResetRequest\x12I\n\x06reason\x18\x01 \x01(\x0b\x32\x34.uprotocol.core.usubscription.v3.ResetRequest.ReasonH\x00\x88\x01\x01\x12/\n\x06\x62\x65\x66ore\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x01\x88\x01\x01\x1a\xb3\x01\n\x06Reason\x12G\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x39.uprotocol.core.usubscription.v3.ResetRequest.Reason.Code\x12\x14\n\x07message\x18\x02 \x01(\tH\x00\x88\x01\x01\">\n\x04\x43ode\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x11\n\rFACTORY_RESET\x10\x01\x12\x12\n\x0e\x43ORRUPTED_DATA\x10\x02\x42\n\n\x08_messageB\t\n\x07_reasonB\t\n\x07_before2\xb9\x08\n\ruSubscription\x12~\n\tSubscribe\x12\x34.uprotocol.core.usubscription.v3.SubscriptionRequest\x1a\x35.uprotocol.core.usubscription.v3.SubscriptionResponse\"\x04\xc0\xc1\x18\x01\x12_\n\x0bUnsubscribe\x12\x33.uprotocol.core.usubscription.v3.UnsubscribeRequest\x1a\x15.uprotocol.v1.UStatus\"\x04\xc0\xc1\x18\x02\x12\x93\x01\n\x12\x46\x65tchSubscriptions\x12:.uprotocol.core.usubscription.v3.FetchSubscriptionsRequest\x1a;.uprotocol.core.usubscription.v3.FetchSubscriptionsResponse\"\x04\xc0\xc1\x18\x03\x12_\n\x0b\x43reateTopic\x12\x33.uprotocol.core.usubscription.v3.CreateTopicRequest\x1a\x15.uprotocol.v1.UStatus\"\x04\xc0\xc1\x18\x04\x12\x65\n\x0e\x44\x65precateTopic\x12\x36.uprotocol.core.usubscription.v3.DeprecateTopicRequest\x1a\x15.uprotocol.v1.UStatus\"\x04\xc0\xc1\x18\x05\x12n\n\x18RegisterForNotifications\x12\x35.uprotocol.core.usubscription.v3.NotificationsRequest\x1a\x15.uprotocol.v1.UStatus\"\x04\xc0\xc1\x18\x06\x12p\n\x1aUnregisterForNotifications\x12\x35.uprotocol.core.usubscription.v3.NotificationsRequest\x1a\x15.uprotocol.v1.UStatus\"\x04\xc0\xc1\x18\x07\x12\x8d\x01\n\x10\x46\x65tchSubscribers\x12\x38.uprotocol.core.usubscription.v3.FetchSubscribersRequest\x1a\x39.uprotocol.core.usubscription.v3.FetchSubscribersResponse\"\x04\xc0\xc1\x18\x08\x12S\n\x05Reset\x12-.uprotocol.core.usubscription.v3.ResetRequest\x1a\x15.uprotocol.v1.UStatus\"\x04\xc0\xc1\x18\t\x1a\"\xa2\xbb\x18\x12\x63ore.usubscription\xa8\xbb\x18\x03\xb0\xbb\x18\x00\xb8\xbb\x18\x00\x42\x43\n+org.eclipse.uprotocol.core.usubscription.v3B\x12USubscriptionProtoP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n)core/usubscription/v3/usubscription.proto\x12\x1fuprotocol.core.usubscription.v3\x1a\x19google/protobuf/any.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\rustatus.proto\x1a\turi.proto\x1a\x17uprotocol_options.proto\"\x9c\x01\n\x13SubscribeAttributes\x12*\n\x06\x65xpire\x18\x01 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12%\n\x07\x64\x65tails\x18\x02 \x03(\x0b\x32\x14.google.protobuf.Any\x12\x1d\n\x10sample_period_ms\x18\x03 \x01(\rH\x00\x88\x01\x01\x42\x13\n\x11_sample_period_ms\"X\n\x0eSubscriberInfo\x12\x1f\n\x03uri\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUri\x12%\n\x07\x64\x65tails\x18\x02 \x03(\x0b\x32\x14.google.protobuf.Any\"\xed\x01\n\x12SubscriptionStatus\x12H\n\x05state\x18\x01 \x01(\x0e\x32\x39.uprotocol.core.usubscription.v3.SubscriptionStatus.State\x12!\n\x04\x63ode\x18\x02 \x01(\x0e\x32\x13.uprotocol.v1.UCode\x12\x0f\n\x07message\x18\x03 \x01(\t\"Y\n\x05State\x12\x10\n\x0cUNSUBSCRIBED\x10\x00\x12\x15\n\x11SUBSCRIBE_PENDING\x10\x01\x12\x0e\n\nSUBSCRIBED\x10\x02\x12\x17\n\x13UNSUBSCRIBE_PENDING\x10\x03\"\xd2\x01\n\x13\x45ventDeliveryConfig\x12\n\n\x02id\x18\x01 \x01(\t\x12\x0c\n\x04type\x18\x02 \x01(\t\x12X\n\nattributes\x18\x03 \x03(\x0b\x32\x44.uprotocol.core.usubscription.v3.EventDeliveryConfig.AttributesEntry\x1aG\n\x0f\x41ttributesEntry\x12\x0b\n\x03key\x18\x01 \x01(\t\x12#\n\x05value\x18\x02 \x01(\x0b\x32\x14.google.protobuf.Any:\x02\x38\x01\"\xc7\x01\n\x13SubscriptionRequest\x12!\n\x05topic\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUri\x12\x43\n\nsubscriber\x18\x02 \x01(\x0b\x32/.uprotocol.core.usubscription.v3.SubscriberInfo\x12H\n\nattributes\x18\x03 \x01(\x0b\x32\x34.uprotocol.core.usubscription.v3.SubscribeAttributes\"\xc4\x01\n\x14SubscriptionResponse\x12\x43\n\x06status\x18\x01 \x01(\x0b\x32\x33.uprotocol.core.usubscription.v3.SubscriptionStatus\x12\x44\n\x06\x63onfig\x18\x02 \x01(\x0b\x32\x34.uprotocol.core.usubscription.v3.EventDeliveryConfig\x12!\n\x05topic\x18\x03 \x01(\x0b\x32\x12.uprotocol.v1.UUri\"|\n\x12UnsubscribeRequest\x12!\n\x05topic\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUri\x12\x43\n\nsubscriber\x18\x02 \x01(\x0b\x32/.uprotocol.core.usubscription.v3.SubscriberInfo\"\\\n\x17\x46\x65tchSubscribersRequest\x12!\n\x05topic\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUri\x12\x13\n\x06offset\x18\x02 \x01(\rH\x00\x88\x01\x01\x42\t\n\x07_offset\"\xbb\x01\n\x18\x46\x65tchSubscribersResponse\x12\x44\n\x0bsubscribers\x18\x01 \x03(\x0b\x32/.uprotocol.core.usubscription.v3.SubscriberInfo\x12\x1d\n\x10has_more_records\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12%\n\x06status\x18\x03 \x01(\x0b\x32\x15.uprotocol.v1.UStatusB\x13\n\x11_has_more_records\"\xcb\x02\n\x0cSubscription\x12!\n\x05topic\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUri\x12\x43\n\nsubscriber\x18\x02 \x01(\x0b\x32/.uprotocol.core.usubscription.v3.SubscriberInfo\x12\x43\n\x06status\x18\x03 \x01(\x0b\x32\x33.uprotocol.core.usubscription.v3.SubscriptionStatus\x12H\n\nattributes\x18\x04 \x01(\x0b\x32\x34.uprotocol.core.usubscription.v3.SubscribeAttributes\x12\x44\n\x06\x63onfig\x18\x05 \x01(\x0b\x32\x34.uprotocol.core.usubscription.v3.EventDeliveryConfig\"\xb2\x01\n\x19\x46\x65tchSubscriptionsRequest\x12#\n\x05topic\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUriH\x00\x12\x45\n\nsubscriber\x18\x02 \x01(\x0b\x32/.uprotocol.core.usubscription.v3.SubscriberInfoH\x00\x12\x13\n\x06offset\x18\x03 \x01(\rH\x01\x88\x01\x01\x42\t\n\x07requestB\t\n\x07_offset\"\xbd\x01\n\x1a\x46\x65tchSubscriptionsResponse\x12\x44\n\rsubscriptions\x18\x01 \x03(\x0b\x32-.uprotocol.core.usubscription.v3.Subscription\x12\x1d\n\x10has_more_records\x18\x02 \x01(\x08H\x00\x88\x01\x01\x12%\n\x06status\x18\x03 \x01(\x0b\x32\x15.uprotocol.v1.UStatusB\x13\n\x11_has_more_records\"~\n\x14NotificationsRequest\x12!\n\x05topic\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUri\x12\x43\n\nsubscriber\x18\x02 \x01(\x0b\x32/.uprotocol.core.usubscription.v3.SubscriberInfo\"7\n\x12\x43reateTopicRequest\x12!\n\x05topic\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUri\":\n\x15\x44\x65precateTopicRequest\x12!\n\x05topic\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUri\"\x9f\x02\n\x06Update\x12!\n\x05topic\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUri\x12\x43\n\nsubscriber\x18\x02 \x01(\x0b\x32/.uprotocol.core.usubscription.v3.SubscriberInfo\x12\x43\n\x06status\x18\x03 \x01(\x0b\x32\x33.uprotocol.core.usubscription.v3.SubscriptionStatus\x12H\n\nattributes\x18\x04 \x01(\x0b\x32\x34.uprotocol.core.usubscription.v3.SubscribeAttributes\"\x1e\n\tResources\x12\x11\n\rsubscriptions\x10\x00\"\x1d\n\x0bPassiveMode\x12\x0e\n\x06\x65nable\x18\x01 \x01(\x08\"\xd6\x02\n\x0cResetRequest\x12I\n\x06reason\x18\x01 \x01(\x0b\x32\x34.uprotocol.core.usubscription.v3.ResetRequest.ReasonH\x00\x88\x01\x01\x12/\n\x06\x62\x65\x66ore\x18\x02 \x01(\x0b\x32\x1a.google.protobuf.TimestampH\x01\x88\x01\x01\x1a\xb3\x01\n\x06Reason\x12G\n\x04\x63ode\x18\x01 \x01(\x0e\x32\x39.uprotocol.core.usubscription.v3.ResetRequest.Reason.Code\x12\x14\n\x07message\x18\x02 \x01(\tH\x00\x88\x01\x01\">\n\x04\x43ode\x12\x0f\n\x0bUNSPECIFIED\x10\x00\x12\x11\n\rFACTORY_RESET\x10\x01\x12\x12\n\x0e\x43ORRUPTED_DATA\x10\x02\x42\n\n\x08_messageB\t\n\x07_reasonB\t\n\x07_before2\xdd\x08\n\ruSubscription\x12~\n\tSubscribe\x12\x34.uprotocol.core.usubscription.v3.SubscriptionRequest\x1a\x35.uprotocol.core.usubscription.v3.SubscriptionResponse\"\x04\x80\x80\x19\x01\x12_\n\x0bUnsubscribe\x12\x33.uprotocol.core.usubscription.v3.UnsubscribeRequest\x1a\x15.uprotocol.v1.UStatus\"\x04\x80\x80\x19\x02\x12\x93\x01\n\x12\x46\x65tchSubscriptions\x12:.uprotocol.core.usubscription.v3.FetchSubscriptionsRequest\x1a;.uprotocol.core.usubscription.v3.FetchSubscriptionsResponse\"\x04\x80\x80\x19\x03\x12_\n\x0b\x43reateTopic\x12\x33.uprotocol.core.usubscription.v3.CreateTopicRequest\x1a\x15.uprotocol.v1.UStatus\"\x04\x80\x80\x19\x04\x12\x65\n\x0e\x44\x65precateTopic\x12\x36.uprotocol.core.usubscription.v3.DeprecateTopicRequest\x1a\x15.uprotocol.v1.UStatus\"\x04\x80\x80\x19\x05\x12n\n\x18RegisterForNotifications\x12\x35.uprotocol.core.usubscription.v3.NotificationsRequest\x1a\x15.uprotocol.v1.UStatus\"\x04\x80\x80\x19\x06\x12p\n\x1aUnregisterForNotifications\x12\x35.uprotocol.core.usubscription.v3.NotificationsRequest\x1a\x15.uprotocol.v1.UStatus\"\x04\x80\x80\x19\x07\x12\x8d\x01\n\x10\x46\x65tchSubscribers\x12\x38.uprotocol.core.usubscription.v3.FetchSubscribersRequest\x1a\x39.uprotocol.core.usubscription.v3.FetchSubscribersResponse\"\x04\x80\x80\x19\x08\x12S\n\x05Reset\x12-.uprotocol.core.usubscription.v3.ResetRequest\x1a\x15.uprotocol.v1.UStatus\"\x04\x80\x80\x19\t\x1a\x46\xe2\xf9\x18\x12\x63ore.usubscription\xe8\xf9\x18\x03\xf0\xf9\x18\x00\xf8\xf9\x18\x00\x92\xfa\x18 \x08\x80\x80\x02\x12\x12SubscriptionChange\x1a\x06UpdateBC\n+org.eclipse.uprotocol.core.usubscription.v3B\x12USubscriptionProtoP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'core.usubscription.v3.usubscription_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n+org.eclipse.uprotocol.core.usubscription.v3B\022USubscriptionProtoP\001'
   _EVENTDELIVERYCONFIG_ATTRIBUTESENTRY._options = None
   _EVENTDELIVERYCONFIG_ATTRIBUTESENTRY._serialized_options = b'8\001'
-  _SUBSCRIPTIONCHANGENOTIFICATION.fields_by_name['resource_name']._options = None
-  _SUBSCRIPTIONCHANGENOTIFICATION.fields_by_name['resource_name']._serialized_options = b'\202\316\030\001*'
-  _SUBSCRIPTIONCHANGENOTIFICATION._options = None
-  _SUBSCRIPTIONCHANGENOTIFICATION._serialized_options = b'\340\307\030\350\007'
   _USUBSCRIPTION._options = None
-  _USUBSCRIPTION._serialized_options = b'\242\273\030\022core.usubscription\250\273\030\003\260\273\030\000\270\273\030\000'
+  _USUBSCRIPTION._serialized_options = b'\342\371\030\022core.usubscription\350\371\030\003\360\371\030\000\370\371\030\000\222\372\030 \010\200\200\002\022\022SubscriptionChange\032\006Update'
   _USUBSCRIPTION.methods_by_name['Subscribe']._options = None
-  _USUBSCRIPTION.methods_by_name['Subscribe']._serialized_options = b'\300\301\030\001'
+  _USUBSCRIPTION.methods_by_name['Subscribe']._serialized_options = b'\200\200\031\001'
   _USUBSCRIPTION.methods_by_name['Unsubscribe']._options = None
-  _USUBSCRIPTION.methods_by_name['Unsubscribe']._serialized_options = b'\300\301\030\002'
+  _USUBSCRIPTION.methods_by_name['Unsubscribe']._serialized_options = b'\200\200\031\002'
   _USUBSCRIPTION.methods_by_name['FetchSubscriptions']._options = None
-  _USUBSCRIPTION.methods_by_name['FetchSubscriptions']._serialized_options = b'\300\301\030\003'
+  _USUBSCRIPTION.methods_by_name['FetchSubscriptions']._serialized_options = b'\200\200\031\003'
   _USUBSCRIPTION.methods_by_name['CreateTopic']._options = None
-  _USUBSCRIPTION.methods_by_name['CreateTopic']._serialized_options = b'\300\301\030\004'
+  _USUBSCRIPTION.methods_by_name['CreateTopic']._serialized_options = b'\200\200\031\004'
   _USUBSCRIPTION.methods_by_name['DeprecateTopic']._options = None
-  _USUBSCRIPTION.methods_by_name['DeprecateTopic']._serialized_options = b'\300\301\030\005'
+  _USUBSCRIPTION.methods_by_name['DeprecateTopic']._serialized_options = b'\200\200\031\005'
   _USUBSCRIPTION.methods_by_name['RegisterForNotifications']._options = None
-  _USUBSCRIPTION.methods_by_name['RegisterForNotifications']._serialized_options = b'\300\301\030\006'
+  _USUBSCRIPTION.methods_by_name['RegisterForNotifications']._serialized_options = b'\200\200\031\006'
   _USUBSCRIPTION.methods_by_name['UnregisterForNotifications']._options = None
-  _USUBSCRIPTION.methods_by_name['UnregisterForNotifications']._serialized_options = b'\300\301\030\007'
+  _USUBSCRIPTION.methods_by_name['UnregisterForNotifications']._serialized_options = b'\200\200\031\007'
   _USUBSCRIPTION.methods_by_name['FetchSubscribers']._options = None
-  _USUBSCRIPTION.methods_by_name['FetchSubscribers']._serialized_options = b'\300\301\030\010'
+  _USUBSCRIPTION.methods_by_name['FetchSubscribers']._serialized_options = b'\200\200\031\010'
   _USUBSCRIPTION.methods_by_name['Reset']._options = None
-  _USUBSCRIPTION.methods_by_name['Reset']._serialized_options = b'\300\301\030\t'
-  _SUBSCRIBEATTRIBUTES._serialized_start=189
-  _SUBSCRIBEATTRIBUTES._serialized_end=293
-  _SUBSCRIBERINFO._serialized_start=295
-  _SUBSCRIBERINFO._serialized_end=383
-  _SUBSCRIPTIONSTATUS._serialized_start=386
-  _SUBSCRIPTIONSTATUS._serialized_end=623
-  _SUBSCRIPTIONSTATUS_STATE._serialized_start=534
-  _SUBSCRIPTIONSTATUS_STATE._serialized_end=623
-  _EVENTDELIVERYCONFIG._serialized_start=626
-  _EVENTDELIVERYCONFIG._serialized_end=836
-  _EVENTDELIVERYCONFIG_ATTRIBUTESENTRY._serialized_start=765
-  _EVENTDELIVERYCONFIG_ATTRIBUTESENTRY._serialized_end=836
-  _SUBSCRIPTIONREQUEST._serialized_start=839
-  _SUBSCRIPTIONREQUEST._serialized_end=1038
-  _SUBSCRIPTIONRESPONSE._serialized_start=1041
-  _SUBSCRIPTIONRESPONSE._serialized_end=1237
-  _UNSUBSCRIBEREQUEST._serialized_start=1239
-  _UNSUBSCRIBEREQUEST._serialized_end=1363
-  _FETCHSUBSCRIBERSREQUEST._serialized_start=1365
-  _FETCHSUBSCRIBERSREQUEST._serialized_end=1457
-  _FETCHSUBSCRIBERSRESPONSE._serialized_start=1460
-  _FETCHSUBSCRIBERSRESPONSE._serialized_end=1647
-  _SUBSCRIPTION._serialized_start=1650
-  _SUBSCRIPTION._serialized_end=1981
-  _FETCHSUBSCRIPTIONSREQUEST._serialized_start=1984
-  _FETCHSUBSCRIPTIONSREQUEST._serialized_end=2162
-  _FETCHSUBSCRIPTIONSRESPONSE._serialized_start=2165
-  _FETCHSUBSCRIPTIONSRESPONSE._serialized_end=2354
-  _NOTIFICATIONSREQUEST._serialized_start=2356
-  _NOTIFICATIONSREQUEST._serialized_end=2482
-  _CREATETOPICREQUEST._serialized_start=2484
-  _CREATETOPICREQUEST._serialized_end=2539
-  _DEPRECATETOPICREQUEST._serialized_start=2541
-  _DEPRECATETOPICREQUEST._serialized_end=2599
-  _UPDATE._serialized_start=2602
-  _UPDATE._serialized_end=2889
-  _UPDATE_RESOURCES._serialized_start=2859
-  _UPDATE_RESOURCES._serialized_end=2889
-  _SUBSCRIPTIONCHANGENOTIFICATION._serialized_start=2891
-  _SUBSCRIPTIONCHANGENOTIFICATION._serialized_end=3011
-  _PASSIVEMODE._serialized_start=3013
-  _PASSIVEMODE._serialized_end=3042
-  _RESETREQUEST._serialized_start=3045
-  _RESETREQUEST._serialized_end=3387
-  _RESETREQUEST_REASON._serialized_start=3186
-  _RESETREQUEST_REASON._serialized_end=3365
-  _RESETREQUEST_REASON_CODE._serialized_start=3291
-  _RESETREQUEST_REASON_CODE._serialized_end=3353
-  _USUBSCRIPTION._serialized_start=3390
-  _USUBSCRIPTION._serialized_end=4471
+  _USUBSCRIPTION.methods_by_name['Reset']._serialized_options = b'\200\200\031\t'
+  _SUBSCRIBEATTRIBUTES._serialized_start=190
+  _SUBSCRIBEATTRIBUTES._serialized_end=346
+  _SUBSCRIBERINFO._serialized_start=348
+  _SUBSCRIBERINFO._serialized_end=436
+  _SUBSCRIPTIONSTATUS._serialized_start=439
+  _SUBSCRIPTIONSTATUS._serialized_end=676
+  _SUBSCRIPTIONSTATUS_STATE._serialized_start=587
+  _SUBSCRIPTIONSTATUS_STATE._serialized_end=676
+  _EVENTDELIVERYCONFIG._serialized_start=679
+  _EVENTDELIVERYCONFIG._serialized_end=889
+  _EVENTDELIVERYCONFIG_ATTRIBUTESENTRY._serialized_start=818
+  _EVENTDELIVERYCONFIG_ATTRIBUTESENTRY._serialized_end=889
+  _SUBSCRIPTIONREQUEST._serialized_start=892
+  _SUBSCRIPTIONREQUEST._serialized_end=1091
+  _SUBSCRIPTIONRESPONSE._serialized_start=1094
+  _SUBSCRIPTIONRESPONSE._serialized_end=1290
+  _UNSUBSCRIBEREQUEST._serialized_start=1292
+  _UNSUBSCRIBEREQUEST._serialized_end=1416
+  _FETCHSUBSCRIBERSREQUEST._serialized_start=1418
+  _FETCHSUBSCRIBERSREQUEST._serialized_end=1510
+  _FETCHSUBSCRIBERSRESPONSE._serialized_start=1513
+  _FETCHSUBSCRIBERSRESPONSE._serialized_end=1700
+  _SUBSCRIPTION._serialized_start=1703
+  _SUBSCRIPTION._serialized_end=2034
+  _FETCHSUBSCRIPTIONSREQUEST._serialized_start=2037
+  _FETCHSUBSCRIPTIONSREQUEST._serialized_end=2215
+  _FETCHSUBSCRIPTIONSRESPONSE._serialized_start=2218
+  _FETCHSUBSCRIPTIONSRESPONSE._serialized_end=2407
+  _NOTIFICATIONSREQUEST._serialized_start=2409
+  _NOTIFICATIONSREQUEST._serialized_end=2535
+  _CREATETOPICREQUEST._serialized_start=2537
+  _CREATETOPICREQUEST._serialized_end=2592
+  _DEPRECATETOPICREQUEST._serialized_start=2594
+  _DEPRECATETOPICREQUEST._serialized_end=2652
+  _UPDATE._serialized_start=2655
+  _UPDATE._serialized_end=2942
+  _UPDATE_RESOURCES._serialized_start=2912
+  _UPDATE_RESOURCES._serialized_end=2942
+  _PASSIVEMODE._serialized_start=2944
+  _PASSIVEMODE._serialized_end=2973
+  _RESETREQUEST._serialized_start=2976
+  _RESETREQUEST._serialized_end=3318
+  _RESETREQUEST_REASON._serialized_start=3117
+  _RESETREQUEST_REASON._serialized_end=3296
+  _RESETREQUEST_REASON_CODE._serialized_start=3222
+  _RESETREQUEST_REASON_CODE._serialized_end=3284
+  _USUBSCRIPTION._serialized_start=3321
+  _USUBSCRIPTION._serialized_end=4438
 # @@protoc_insertion_point(module_scope)
```

### Comparing `up_python-0.1.1.dev0/uprotocol/proto/core/utwin/v1/utwin_pb2.py` & `up_python-0.1.2.dev0/uprotocol/proto/core/utwin/v2/utwin_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # -*- coding: utf-8 -*-
 # Generated by the protocol buffer compiler.  DO NOT EDIT!
-# source: core/utwin/v1/utwin.proto
+# source: core/utwin/v2/utwin.proto
 """Generated protocol buffer code."""
 from google.protobuf.internal import builder as _builder
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
@@ -13,28 +13,28 @@
 
 import uprotocol.proto.uprotocol_options_pb2 as uprotocol__options__pb2
 import uprotocol.proto.ustatus_pb2 as ustatus__pb2
 import uprotocol.proto.uri_pb2 as uri__pb2
 import uprotocol.proto.umessage_pb2 as umessage__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19\x63ore/utwin/v1/utwin.proto\x12\x17uprotocol.core.utwin.v1\x1a\x17uprotocol_options.proto\x1a\rustatus.proto\x1a\turi.proto\x1a\x0eumessage.proto\"\x84\x01\n\x0fMessageResponse\x12!\n\x05topic\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUri\x12%\n\x06status\x18\x02 \x01(\x0b\x32\x15.uprotocol.v1.UStatus\x12\'\n\x07message\x18\x03 \x01(\x0b\x32\x16.uprotocol.v1.UMessage\"V\n\x17GetLastMessagesResponse\x12;\n\tresponses\x18\x02 \x03(\x0b\x32(.uprotocol.core.utwin.v1.MessageResponse2\xce\x01\n\x05uTwin\x12\x62\n\x0fGetLastMessages\x12\x17.uprotocol.v1.UUriBatch\x1a\x30.uprotocol.core.utwin.v1.GetLastMessagesResponse\"\x04\xc0\xc1\x18\x01\x12\x45\n\x0eSetLastMessage\x12\x16.uprotocol.v1.UMessage\x1a\x15.uprotocol.v1.UStatus\"\x04\xc0\xc1\x18\x02\x1a\x1a\xa2\xbb\x18\ncore.utwin\xa8\xbb\x18\x01\xb0\xbb\x18\x00\xb8\xbb\x18\x1a\x42\x33\n#org.eclipse.uprotocol.core.utwin.v1B\nUTwinProtoP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x19\x63ore/utwin/v2/utwin.proto\x12\x17uprotocol.core.utwin.v2\x1a\x17uprotocol_options.proto\x1a\rustatus.proto\x1a\turi.proto\x1a\x0eumessage.proto\"\x84\x01\n\x0fMessageResponse\x12!\n\x05topic\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUri\x12%\n\x06status\x18\x02 \x01(\x0b\x32\x15.uprotocol.v1.UStatus\x12\'\n\x07message\x18\x03 \x01(\x0b\x32\x16.uprotocol.v1.UMessage\"V\n\x17GetLastMessagesResponse\x12;\n\tresponses\x18\x02 \x03(\x0b\x32(.uprotocol.core.utwin.v2.MessageResponse2\xce\x01\n\x05uTwin\x12\x62\n\x0fGetLastMessages\x12\x17.uprotocol.v1.UUriBatch\x1a\x30.uprotocol.core.utwin.v2.GetLastMessagesResponse\"\x04\x80\x80\x19\x01\x12\x45\n\x0eSetLastMessage\x12\x16.uprotocol.v1.UMessage\x1a\x15.uprotocol.v1.UStatus\"\x04\x80\x80\x19\x02\x1a\x1a\xe2\xf9\x18\ncore.utwin\xe8\xf9\x18\x02\xf0\xf9\x18\x00\xf8\xf9\x18\x1a\x42\x33\n#org.eclipse.uprotocol.core.utwin.v2B\nUTwinProtoP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
-_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'core.utwin.v1.utwin_pb2', globals())
+_builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'core.utwin.v2.utwin_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
-  DESCRIPTOR._serialized_options = b'\n#org.eclipse.uprotocol.core.utwin.v1B\nUTwinProtoP\001'
+  DESCRIPTOR._serialized_options = b'\n#org.eclipse.uprotocol.core.utwin.v2B\nUTwinProtoP\001'
   _UTWIN._options = None
-  _UTWIN._serialized_options = b'\242\273\030\ncore.utwin\250\273\030\001\260\273\030\000\270\273\030\032'
+  _UTWIN._serialized_options = b'\342\371\030\ncore.utwin\350\371\030\002\360\371\030\000\370\371\030\032'
   _UTWIN.methods_by_name['GetLastMessages']._options = None
-  _UTWIN.methods_by_name['GetLastMessages']._serialized_options = b'\300\301\030\001'
+  _UTWIN.methods_by_name['GetLastMessages']._serialized_options = b'\200\200\031\001'
   _UTWIN.methods_by_name['SetLastMessage']._options = None
-  _UTWIN.methods_by_name['SetLastMessage']._serialized_options = b'\300\301\030\002'
+  _UTWIN.methods_by_name['SetLastMessage']._serialized_options = b'\200\200\031\002'
   _MESSAGERESPONSE._serialized_start=122
   _MESSAGERESPONSE._serialized_end=254
   _GETLASTMESSAGESRESPONSE._serialized_start=256
   _GETLASTMESSAGESRESPONSE._serialized_end=342
   _UTWIN._serialized_start=345
   _UTWIN._serialized_end=551
 # @@protoc_insertion_point(module_scope)
```

### Comparing `up_python-0.1.1.dev0/uprotocol/proto/file_pb2.py` & `up_python-0.1.2.dev0/uprotocol/proto/file_pb2.py`

 * *Files identical despite different names*

### Comparing `up_python-0.1.1.dev0/uprotocol/proto/uattributes_pb2.py` & `up_python-0.1.2.dev0/uprotocol/proto/uattributes_pb2.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,45 +9,50 @@
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
 import uprotocol.proto.uri_pb2 as uri__pb2
 import uprotocol.proto.uuid_pb2 as uuid__pb2
+import uprotocol.proto.ustatus_pb2 as ustatus__pb2
 import uprotocol.proto.uprotocol_options_pb2 as uprotocol__options__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11uattributes.proto\x12\x0cuprotocol.v1\x1a\turi.proto\x1a\nuuid.proto\x1a\x17uprotocol_options.proto\"\xa9\x03\n\x0bUAttributes\x12\x1e\n\x02id\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUID\x12(\n\x04type\x18\x02 \x01(\x0e\x32\x1a.uprotocol.v1.UMessageType\x12\"\n\x06source\x18\x03 \x01(\x0b\x32\x12.uprotocol.v1.UUri\x12 \n\x04sink\x18\x04 \x01(\x0b\x32\x12.uprotocol.v1.UUri\x12)\n\x08priority\x18\x05 \x01(\x0e\x32\x17.uprotocol.v1.UPriority\x12\x10\n\x03ttl\x18\x06 \x01(\x05H\x00\x88\x01\x01\x12\x1d\n\x10permission_level\x18\x07 \x01(\x05H\x01\x88\x01\x01\x12\x17\n\ncommstatus\x18\x08 \x01(\x05H\x02\x88\x01\x01\x12!\n\x05reqid\x18\t \x01(\x0b\x32\x12.uprotocol.v1.UUID\x12\x12\n\x05token\x18\n \x01(\tH\x03\x88\x01\x01\x12\x18\n\x0btraceparent\x18\x0b \x01(\tH\x04\x88\x01\x01\x42\x06\n\x04_ttlB\x13\n\x11_permission_levelB\r\n\x0b_commstatusB\x08\n\x06_tokenB\x0e\n\x0c_traceparent*\xa3\x01\n\x0cUMessageType\x12\x1d\n\x19UMESSAGE_TYPE_UNSPECIFIED\x10\x00\x12%\n\x15UMESSAGE_TYPE_PUBLISH\x10\x01\x1a\n\xaa\xd4\x18\x06pub.v1\x12%\n\x15UMESSAGE_TYPE_REQUEST\x10\x02\x1a\n\xaa\xd4\x18\x06req.v1\x12&\n\x16UMESSAGE_TYPE_RESPONSE\x10\x03\x1a\n\xaa\xd4\x18\x06res.v1*\xea\x01\n\tUPriority\x12\x19\n\x15UPRIORITY_UNSPECIFIED\x10\x00\x12\x1a\n\rUPRIORITY_CS0\x10\x01\x1a\x07\xaa\xd4\x18\x03\x43S0\x12\x1a\n\rUPRIORITY_CS1\x10\x02\x1a\x07\xaa\xd4\x18\x03\x43S1\x12\x1a\n\rUPRIORITY_CS2\x10\x03\x1a\x07\xaa\xd4\x18\x03\x43S2\x12\x1a\n\rUPRIORITY_CS3\x10\x04\x1a\x07\xaa\xd4\x18\x03\x43S3\x12\x1a\n\rUPRIORITY_CS4\x10\x05\x1a\x07\xaa\xd4\x18\x03\x43S4\x12\x1a\n\rUPRIORITY_CS5\x10\x06\x1a\x07\xaa\xd4\x18\x03\x43S5\x12\x1a\n\rUPRIORITY_CS6\x10\x07\x1a\x07\xaa\xd4\x18\x03\x43S6B.\n\x18org.eclipse.uprotocol.v1B\x10UAttributesProtoP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x11uattributes.proto\x12\x0cuprotocol.v1\x1a\turi.proto\x1a\nuuid.proto\x1a\rustatus.proto\x1a\x17uprotocol_options.proto\"\xbe\x03\n\x0bUAttributes\x12\x1e\n\x02id\x18\x01 \x01(\x0b\x32\x12.uprotocol.v1.UUID\x12(\n\x04type\x18\x02 \x01(\x0e\x32\x1a.uprotocol.v1.UMessageType\x12\"\n\x06source\x18\x03 \x01(\x0b\x32\x12.uprotocol.v1.UUri\x12 \n\x04sink\x18\x04 \x01(\x0b\x32\x12.uprotocol.v1.UUri\x12)\n\x08priority\x18\x05 \x01(\x0e\x32\x17.uprotocol.v1.UPriority\x12\x10\n\x03ttl\x18\x06 \x01(\rH\x00\x88\x01\x01\x12\x1d\n\x10permission_level\x18\x07 \x01(\rH\x01\x88\x01\x01\x12,\n\ncommstatus\x18\x08 \x01(\x0e\x32\x13.uprotocol.v1.UCodeH\x02\x88\x01\x01\x12!\n\x05reqid\x18\t \x01(\x0b\x32\x12.uprotocol.v1.UUID\x12\x12\n\x05token\x18\n \x01(\tH\x03\x88\x01\x01\x12\x18\n\x0btraceparent\x18\x0b \x01(\tH\x04\x88\x01\x01\x42\x06\n\x04_ttlB\x13\n\x11_permission_levelB\r\n\x0b_commstatusB\x08\n\x06_tokenB\x0e\n\x0c_traceparent\"c\n\x0b\x43\x61llOptions\x12)\n\x08priority\x18\x01 \x01(\x0e\x32\x17.uprotocol.v1.UPriority\x12\x0b\n\x03ttl\x18\x02 \x01(\r\x12\x12\n\x05token\x18\x03 \x01(\tH\x00\x88\x01\x01\x42\x08\n\x06_token*\xcf\x01\n\x0cUMessageType\x12\x1d\n\x19UMESSAGE_TYPE_UNSPECIFIED\x10\x00\x12%\n\x15UMESSAGE_TYPE_PUBLISH\x10\x01\x1a\n\xea\x92\x19\x06pub.v1\x12%\n\x15UMESSAGE_TYPE_REQUEST\x10\x02\x1a\n\xea\x92\x19\x06req.v1\x12&\n\x16UMESSAGE_TYPE_RESPONSE\x10\x03\x1a\n\xea\x92\x19\x06res.v1\x12*\n\x1aUMESSAGE_TYPE_NOTIFICATION\x10\x04\x1a\n\xea\x92\x19\x06not.v1*\xea\x01\n\tUPriority\x12\x19\n\x15UPRIORITY_UNSPECIFIED\x10\x00\x12\x1a\n\rUPRIORITY_CS0\x10\x01\x1a\x07\xea\x92\x19\x03\x43S0\x12\x1a\n\rUPRIORITY_CS1\x10\x02\x1a\x07\xea\x92\x19\x03\x43S1\x12\x1a\n\rUPRIORITY_CS2\x10\x03\x1a\x07\xea\x92\x19\x03\x43S2\x12\x1a\n\rUPRIORITY_CS3\x10\x04\x1a\x07\xea\x92\x19\x03\x43S3\x12\x1a\n\rUPRIORITY_CS4\x10\x05\x1a\x07\xea\x92\x19\x03\x43S4\x12\x1a\n\rUPRIORITY_CS5\x10\x06\x1a\x07\xea\x92\x19\x03\x43S5\x12\x1a\n\rUPRIORITY_CS6\x10\x07\x1a\x07\xea\x92\x19\x03\x43S6B.\n\x18org.eclipse.uprotocol.v1B\x10UAttributesProtoP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'uattributes_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\030org.eclipse.uprotocol.v1B\020UAttributesProtoP\001'
   _UMESSAGETYPE.values_by_name["UMESSAGE_TYPE_PUBLISH"]._options = None
-  _UMESSAGETYPE.values_by_name["UMESSAGE_TYPE_PUBLISH"]._serialized_options = b'\252\324\030\006pub.v1'
+  _UMESSAGETYPE.values_by_name["UMESSAGE_TYPE_PUBLISH"]._serialized_options = b'\352\222\031\006pub.v1'
   _UMESSAGETYPE.values_by_name["UMESSAGE_TYPE_REQUEST"]._options = None
-  _UMESSAGETYPE.values_by_name["UMESSAGE_TYPE_REQUEST"]._serialized_options = b'\252\324\030\006req.v1'
+  _UMESSAGETYPE.values_by_name["UMESSAGE_TYPE_REQUEST"]._serialized_options = b'\352\222\031\006req.v1'
   _UMESSAGETYPE.values_by_name["UMESSAGE_TYPE_RESPONSE"]._options = None
-  _UMESSAGETYPE.values_by_name["UMESSAGE_TYPE_RESPONSE"]._serialized_options = b'\252\324\030\006res.v1'
+  _UMESSAGETYPE.values_by_name["UMESSAGE_TYPE_RESPONSE"]._serialized_options = b'\352\222\031\006res.v1'
+  _UMESSAGETYPE.values_by_name["UMESSAGE_TYPE_NOTIFICATION"]._options = None
+  _UMESSAGETYPE.values_by_name["UMESSAGE_TYPE_NOTIFICATION"]._serialized_options = b'\352\222\031\006not.v1'
   _UPRIORITY.values_by_name["UPRIORITY_CS0"]._options = None
-  _UPRIORITY.values_by_name["UPRIORITY_CS0"]._serialized_options = b'\252\324\030\003CS0'
+  _UPRIORITY.values_by_name["UPRIORITY_CS0"]._serialized_options = b'\352\222\031\003CS0'
   _UPRIORITY.values_by_name["UPRIORITY_CS1"]._options = None
-  _UPRIORITY.values_by_name["UPRIORITY_CS1"]._serialized_options = b'\252\324\030\003CS1'
+  _UPRIORITY.values_by_name["UPRIORITY_CS1"]._serialized_options = b'\352\222\031\003CS1'
   _UPRIORITY.values_by_name["UPRIORITY_CS2"]._options = None
-  _UPRIORITY.values_by_name["UPRIORITY_CS2"]._serialized_options = b'\252\324\030\003CS2'
+  _UPRIORITY.values_by_name["UPRIORITY_CS2"]._serialized_options = b'\352\222\031\003CS2'
   _UPRIORITY.values_by_name["UPRIORITY_CS3"]._options = None
-  _UPRIORITY.values_by_name["UPRIORITY_CS3"]._serialized_options = b'\252\324\030\003CS3'
+  _UPRIORITY.values_by_name["UPRIORITY_CS3"]._serialized_options = b'\352\222\031\003CS3'
   _UPRIORITY.values_by_name["UPRIORITY_CS4"]._options = None
-  _UPRIORITY.values_by_name["UPRIORITY_CS4"]._serialized_options = b'\252\324\030\003CS4'
+  _UPRIORITY.values_by_name["UPRIORITY_CS4"]._serialized_options = b'\352\222\031\003CS4'
   _UPRIORITY.values_by_name["UPRIORITY_CS5"]._options = None
-  _UPRIORITY.values_by_name["UPRIORITY_CS5"]._serialized_options = b'\252\324\030\003CS5'
+  _UPRIORITY.values_by_name["UPRIORITY_CS5"]._serialized_options = b'\352\222\031\003CS5'
   _UPRIORITY.values_by_name["UPRIORITY_CS6"]._options = None
-  _UPRIORITY.values_by_name["UPRIORITY_CS6"]._serialized_options = b'\252\324\030\003CS6'
-  _UMESSAGETYPE._serialized_start=512
-  _UMESSAGETYPE._serialized_end=675
-  _UPRIORITY._serialized_start=678
-  _UPRIORITY._serialized_end=912
-  _UATTRIBUTES._serialized_start=84
-  _UATTRIBUTES._serialized_end=509
+  _UPRIORITY.values_by_name["UPRIORITY_CS6"]._serialized_options = b'\352\222\031\003CS6'
+  _UMESSAGETYPE._serialized_start=649
+  _UMESSAGETYPE._serialized_end=856
+  _UPRIORITY._serialized_start=859
+  _UPRIORITY._serialized_end=1093
+  _UATTRIBUTES._serialized_start=99
+  _UATTRIBUTES._serialized_end=545
+  _CALLOPTIONS._serialized_start=547
+  _CALLOPTIONS._serialized_end=646
 # @@protoc_insertion_point(module_scope)
```

### Comparing `up_python-0.1.1.dev0/uprotocol/proto/umessage_pb2.py` & `up_python-0.1.2.dev0/uprotocol/proto/umessage_pb2.py`

 * *Files identical despite different names*

### Comparing `up_python-0.1.1.dev0/uprotocol/proto/upayload_pb2.py` & `up_python-0.1.2.dev0/uprotocol/proto/upayload_pb2.py`

 * *Files 11% similar despite different names*

```diff
@@ -10,34 +10,34 @@
 
 _sym_db = _symbol_database.Default()
 
 
 import uprotocol.proto.uprotocol_options_pb2 as uprotocol__options__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0eupayload.proto\x12\x0cuprotocol.v1\x1a\x17uprotocol_options.proto\"\x86\x01\n\x08UPayload\x12\x13\n\treference\x18\x01 \x01(\x06H\x00\x12\x0f\n\x05value\x18\x02 \x01(\x0cH\x00\x12\x13\n\x06length\x18\x03 \x01(\x05H\x01\x88\x01\x01\x12,\n\x06\x66ormat\x18\x04 \x01(\x0e\x32\x1c.uprotocol.v1.UPayloadFormatB\x06\n\x04\x64\x61taB\t\n\x07_length*\xb7\x03\n\x0eUPayloadFormat\x12\x1f\n\x1bUPAYLOAD_FORMAT_UNSPECIFIED\x10\x00\x12G\n\'UPAYLOAD_FORMAT_PROTOBUF_WRAPPED_IN_ANY\x10\x01\x1a\x1a\xa2\xd4\x18\x16\x61pplication/x-protobuf\x12\x36\n\x18UPAYLOAD_FORMAT_PROTOBUF\x10\x02\x1a\x18\xa2\xd4\x18\x14\x61pplication/protobuf\x12.\n\x14UPAYLOAD_FORMAT_JSON\x10\x03\x1a\x14\xa2\xd4\x18\x10\x61pplication/json\x12\x34\n\x16UPAYLOAD_FORMAT_SOMEIP\x10\x04\x1a\x18\xa2\xd4\x18\x14\x61pplication/x-someip\x12<\n\x1aUPAYLOAD_FORMAT_SOMEIP_TLV\x10\x05\x1a\x1c\xa2\xd4\x18\x18\x61pplication/x-someip_tlv\x12\x35\n\x13UPAYLOAD_FORMAT_RAW\x10\x06\x1a\x1c\xa2\xd4\x18\x18\x61pplication/octet-stream\x12(\n\x14UPAYLOAD_FORMAT_TEXT\x10\x07\x1a\x0e\xa2\xd4\x18\ntext/plainB+\n\x18org.eclipse.uprotocol.v1B\rUPayloadProtoP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x0eupayload.proto\x12\x0cuprotocol.v1\x1a\x17uprotocol_options.proto\"\x86\x01\n\x08UPayload\x12\x13\n\treference\x18\x01 \x01(\x06H\x00\x12\x0f\n\x05value\x18\x02 \x01(\x0cH\x00\x12\x13\n\x06length\x18\x03 \x01(\x05H\x01\x88\x01\x01\x12,\n\x06\x66ormat\x18\x04 \x01(\x0e\x32\x1c.uprotocol.v1.UPayloadFormatB\x06\n\x04\x64\x61taB\t\n\x07_length*\xb7\x03\n\x0eUPayloadFormat\x12\x1f\n\x1bUPAYLOAD_FORMAT_UNSPECIFIED\x10\x00\x12G\n\'UPAYLOAD_FORMAT_PROTOBUF_WRAPPED_IN_ANY\x10\x01\x1a\x1a\xe2\x92\x19\x16\x61pplication/x-protobuf\x12\x36\n\x18UPAYLOAD_FORMAT_PROTOBUF\x10\x02\x1a\x18\xe2\x92\x19\x14\x61pplication/protobuf\x12.\n\x14UPAYLOAD_FORMAT_JSON\x10\x03\x1a\x14\xe2\x92\x19\x10\x61pplication/json\x12\x34\n\x16UPAYLOAD_FORMAT_SOMEIP\x10\x04\x1a\x18\xe2\x92\x19\x14\x61pplication/x-someip\x12<\n\x1aUPAYLOAD_FORMAT_SOMEIP_TLV\x10\x05\x1a\x1c\xe2\x92\x19\x18\x61pplication/x-someip_tlv\x12\x35\n\x13UPAYLOAD_FORMAT_RAW\x10\x06\x1a\x1c\xe2\x92\x19\x18\x61pplication/octet-stream\x12(\n\x14UPAYLOAD_FORMAT_TEXT\x10\x07\x1a\x0e\xe2\x92\x19\ntext/plainB+\n\x18org.eclipse.uprotocol.v1B\rUPayloadProtoP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'upayload_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\030org.eclipse.uprotocol.v1B\rUPayloadProtoP\001'
   _UPAYLOADFORMAT.values_by_name["UPAYLOAD_FORMAT_PROTOBUF_WRAPPED_IN_ANY"]._options = None
-  _UPAYLOADFORMAT.values_by_name["UPAYLOAD_FORMAT_PROTOBUF_WRAPPED_IN_ANY"]._serialized_options = b'\242\324\030\026application/x-protobuf'
+  _UPAYLOADFORMAT.values_by_name["UPAYLOAD_FORMAT_PROTOBUF_WRAPPED_IN_ANY"]._serialized_options = b'\342\222\031\026application/x-protobuf'
   _UPAYLOADFORMAT.values_by_name["UPAYLOAD_FORMAT_PROTOBUF"]._options = None
-  _UPAYLOADFORMAT.values_by_name["UPAYLOAD_FORMAT_PROTOBUF"]._serialized_options = b'\242\324\030\024application/protobuf'
+  _UPAYLOADFORMAT.values_by_name["UPAYLOAD_FORMAT_PROTOBUF"]._serialized_options = b'\342\222\031\024application/protobuf'
   _UPAYLOADFORMAT.values_by_name["UPAYLOAD_FORMAT_JSON"]._options = None
-  _UPAYLOADFORMAT.values_by_name["UPAYLOAD_FORMAT_JSON"]._serialized_options = b'\242\324\030\020application/json'
+  _UPAYLOADFORMAT.values_by_name["UPAYLOAD_FORMAT_JSON"]._serialized_options = b'\342\222\031\020application/json'
   _UPAYLOADFORMAT.values_by_name["UPAYLOAD_FORMAT_SOMEIP"]._options = None
-  _UPAYLOADFORMAT.values_by_name["UPAYLOAD_FORMAT_SOMEIP"]._serialized_options = b'\242\324\030\024application/x-someip'
+  _UPAYLOADFORMAT.values_by_name["UPAYLOAD_FORMAT_SOMEIP"]._serialized_options = b'\342\222\031\024application/x-someip'
   _UPAYLOADFORMAT.values_by_name["UPAYLOAD_FORMAT_SOMEIP_TLV"]._options = None
-  _UPAYLOADFORMAT.values_by_name["UPAYLOAD_FORMAT_SOMEIP_TLV"]._serialized_options = b'\242\324\030\030application/x-someip_tlv'
+  _UPAYLOADFORMAT.values_by_name["UPAYLOAD_FORMAT_SOMEIP_TLV"]._serialized_options = b'\342\222\031\030application/x-someip_tlv'
   _UPAYLOADFORMAT.values_by_name["UPAYLOAD_FORMAT_RAW"]._options = None
-  _UPAYLOADFORMAT.values_by_name["UPAYLOAD_FORMAT_RAW"]._serialized_options = b'\242\324\030\030application/octet-stream'
+  _UPAYLOADFORMAT.values_by_name["UPAYLOAD_FORMAT_RAW"]._serialized_options = b'\342\222\031\030application/octet-stream'
   _UPAYLOADFORMAT.values_by_name["UPAYLOAD_FORMAT_TEXT"]._options = None
-  _UPAYLOADFORMAT.values_by_name["UPAYLOAD_FORMAT_TEXT"]._serialized_options = b'\242\324\030\ntext/plain'
+  _UPAYLOADFORMAT.values_by_name["UPAYLOAD_FORMAT_TEXT"]._serialized_options = b'\342\222\031\ntext/plain'
   _UPAYLOADFORMAT._serialized_start=195
   _UPAYLOADFORMAT._serialized_end=634
   _UPAYLOAD._serialized_start=58
   _UPAYLOAD._serialized_end=192
 # @@protoc_insertion_point(module_scope)
```

### Comparing `up_python-0.1.1.dev0/uprotocol/proto/uprotocol_options_pb2.py` & `up_python-0.1.2.dev0/uprotocol/proto/uprotocol_options_pb2.py`

 * *Files 12% similar despite different names*

```diff
@@ -10,28 +10,32 @@
 
 _sym_db = _symbol_database.Default()
 
 
 from google.protobuf import descriptor_pb2 as google_dot_protobuf_dot_descriptor__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17uprotocol_options.proto\x12\tuprotocol\x1a google/protobuf/descriptor.proto:/\n\x04name\x12\x1f.google.protobuf.ServiceOptions\x18\xb4\x87\x03 \x01(\t:8\n\rversion_major\x12\x1f.google.protobuf.ServiceOptions\x18\xb5\x87\x03 \x01(\r:8\n\rversion_minor\x12\x1f.google.protobuf.ServiceOptions\x18\xb6\x87\x03 \x01(\r:-\n\x02id\x12\x1f.google.protobuf.ServiceOptions\x18\xb7\x87\x03 \x01(\r:;\n\x10permission_level\x12\x1f.google.protobuf.ServiceOptions\x18\xb8\x87\x03 \x01(\r:6\n\tmethod_id\x12\x1e.google.protobuf.MethodOptions\x18\x98\x88\x03 \x01(\r\x88\x01\x01:A\n\x17method_permission_level\x12\x1e.google.protobuf.MethodOptions\x18\x99\x88\x03 \x01(\r:;\n\rbase_topic_id\x12\x1f.google.protobuf.MessageOptions\x18\xfc\x88\x03 \x01(\r\x88\x01\x01:A\n\x16topic_permission_level\x12\x1f.google.protobuf.MessageOptions\x18\xfd\x88\x03 \x01(\r:>\n\x12resource_name_mask\x12\x1d.google.protobuf.FieldOptions\x18\xe0\x89\x03 \x01(\t\x88\x01\x01:9\n\tmime_type\x12!.google.protobuf.EnumValueOptions\x18\xc4\x8a\x03 \x01(\t\x88\x01\x01:7\n\x07\x63\x65_name\x12!.google.protobuf.EnumValueOptions\x18\xc5\x8a\x03 \x01(\t\x88\x01\x01\x42\x19\n\x15org.eclipse.uprotocolP\x01\x62\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x17uprotocol_options.proto\x12\tuprotocol\x1a google/protobuf/descriptor.proto\":\n\rUServiceTopic\x12\n\n\x02id\x18\x01 \x01(\r\x12\x0c\n\x04name\x18\x02 \x01(\t\x12\x0f\n\x07message\x18\x03 \x01(\t:/\n\x04name\x12\x1f.google.protobuf.ServiceOptions\x18\x9c\x8f\x03 \x01(\t:8\n\rversion_major\x12\x1f.google.protobuf.ServiceOptions\x18\x9d\x8f\x03 \x01(\r:8\n\rversion_minor\x12\x1f.google.protobuf.ServiceOptions\x18\x9e\x8f\x03 \x01(\r:-\n\x02id\x12\x1f.google.protobuf.ServiceOptions\x18\x9f\x8f\x03 \x01(\r:;\n\x10permission_level\x12\x1f.google.protobuf.ServiceOptions\x18\xa0\x8f\x03 \x01(\r:R\n\rpublish_topic\x12\x1f.google.protobuf.ServiceOptions\x18\xa1\x8f\x03 \x03(\x0b\x32\x18.uprotocol.UServiceTopic:W\n\x12notification_topic\x12\x1f.google.protobuf.ServiceOptions\x18\xa2\x8f\x03 \x03(\x0b\x32\x18.uprotocol.UServiceTopic:6\n\tmethod_id\x12\x1e.google.protobuf.MethodOptions\x18\x80\x90\x03 \x01(\r\x88\x01\x01:A\n\x17method_permission_level\x12\x1e.google.protobuf.MethodOptions\x18\x81\x90\x03 \x01(\r:;\n\rbase_topic_id\x12\x1f.google.protobuf.MessageOptions\x18\xe4\x90\x03 \x01(\r\x88\x01\x01:A\n\x16topic_permission_level\x12\x1f.google.protobuf.MessageOptions\x18\xe5\x90\x03 \x01(\r:>\n\x12resource_name_mask\x12\x1d.google.protobuf.FieldOptions\x18\xc8\x91\x03 \x01(\t\x88\x01\x01:9\n\tmime_type\x12!.google.protobuf.EnumValueOptions\x18\xac\x92\x03 \x01(\t\x88\x01\x01:7\n\x07\x63\x65_name\x12!.google.protobuf.EnumValueOptions\x18\xad\x92\x03 \x01(\t\x88\x01\x01\x42\x19\n\x15org.eclipse.uprotocolP\x01\x62\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'uprotocol_options_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
   google_dot_protobuf_dot_descriptor__pb2.ServiceOptions.RegisterExtension(name)
   google_dot_protobuf_dot_descriptor__pb2.ServiceOptions.RegisterExtension(version_major)
   google_dot_protobuf_dot_descriptor__pb2.ServiceOptions.RegisterExtension(version_minor)
   google_dot_protobuf_dot_descriptor__pb2.ServiceOptions.RegisterExtension(id)
   google_dot_protobuf_dot_descriptor__pb2.ServiceOptions.RegisterExtension(permission_level)
+  google_dot_protobuf_dot_descriptor__pb2.ServiceOptions.RegisterExtension(publish_topic)
+  google_dot_protobuf_dot_descriptor__pb2.ServiceOptions.RegisterExtension(notification_topic)
   google_dot_protobuf_dot_descriptor__pb2.MethodOptions.RegisterExtension(method_id)
   google_dot_protobuf_dot_descriptor__pb2.MethodOptions.RegisterExtension(method_permission_level)
   google_dot_protobuf_dot_descriptor__pb2.MessageOptions.RegisterExtension(base_topic_id)
   google_dot_protobuf_dot_descriptor__pb2.MessageOptions.RegisterExtension(topic_permission_level)
   google_dot_protobuf_dot_descriptor__pb2.FieldOptions.RegisterExtension(resource_name_mask)
   google_dot_protobuf_dot_descriptor__pb2.EnumValueOptions.RegisterExtension(mime_type)
   google_dot_protobuf_dot_descriptor__pb2.EnumValueOptions.RegisterExtension(ce_name)
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\n\025org.eclipse.uprotocolP\001'
+  _USERVICETOPIC._serialized_start=72
+  _USERVICETOPIC._serialized_end=130
 # @@protoc_insertion_point(module_scope)
```

### Comparing `up_python-0.1.1.dev0/uprotocol/proto/uri_pb2.py` & `up_python-0.1.2.dev0/uprotocol/proto/uri_pb2.py`

 * *Files identical despite different names*

### Comparing `up_python-0.1.1.dev0/uprotocol/proto/ustatus_pb2.py` & `up_python-0.1.2.dev0/uprotocol/proto/ustatus_pb2.py`

 * *Files identical despite different names*

### Comparing `up_python-0.1.1.dev0/uprotocol/proto/uuid_pb2.py` & `up_python-0.1.2.dev0/uprotocol/proto/uuid_pb2.py`

 * *Files identical despite different names*

### Comparing `up_python-0.1.1.dev0/uprotocol/rpc/calloptions.py` & `up_python-0.1.2.dev0/uprotocol/uri/serializer/uriserializer.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 # -------------------------------------------------------------------------
-#
+
 # Copyright (c) 2023 General Motors GTO LLC
 #
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
@@ -17,86 +17,40 @@
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 # SPDX-FileType: SOURCE
 # SPDX-FileCopyrightText: 2023 General Motors GTO LLC
 # SPDX-License-Identifier: Apache-2.0
-#
-# -------------------------------------------------------------------------
-
-
-class CallOptions:
-    """
-    This class is used when making uRPC calls to pass additional options.
-    """
-    TIMEOUT_DEFAULT = 10000
-    """
-    Default timeout of a call in milliseconds.
-    """
-
-
-    def __init__(self, timeout=TIMEOUT_DEFAULT, token=""):
-        self.mTimeout = timeout
-        self.mToken = token if token else ""
 
+# -------------------------------------------------------------------------
 
-    def get_timeout(self):
-        """
-        Get a timeout.<br><br>
-        @return:  A timeout in milliseconds.
-        """
-        return self.mTimeout
-
-    def get_token(self):
-        """
-        Get an OAuth2 access token.<br><br>
-        @return: An Optional OAuth2 access token.
-        """
-        return self.mToken if self.mToken else None
-
-    def __eq__(self, other):
-        if not isinstance(other, CallOptions):
-            return False
-        return self.mTimeout == other.mTimeout and self.mToken == other.mToken
-
-    def __hash__(self):
-        return hash((self.mTimeout, self.mToken))
 
-    def __str__(self):
-        return f"CallOptions{{mTimeout={self.mTimeout}, mToken='{self.mToken}'}}"
+from abc import ABC, abstractmethod
+from re import T
+from uprotocol.proto.uri_pb2 import UUri
 
 
-class CallOptionsBuilder:
+class UriSerializer(ABC):
     """
-    Builder for constructing <code>CallOptions</code>.
+    UUris are used in transport layers and hence need to be serialized.<br>
+    Each transport supports different
+    serialization formats.
     """
-    TIMEOUT_DEFAULT = 10000
-    DEFAULT= CallOptions(TIMEOUT_DEFAULT,'')
-    def __init__(self):
-        self.mTimeout = self.TIMEOUT_DEFAULT
-        self.mToken = ""
-
-    def with_timeout(self, timeout):
-        """
-        Add a timeout.<br><br>
-        @param timeout:A timeout in milliseconds.
-        @return:This builder.
-        """
-        self.mTimeout = timeout if timeout > 0 else self.TIMEOUT_DEFAULT
-        return self
 
-    def with_token(self, token):
+    @abstractmethod
+    def deserialize(self, uri: T) -> UUri:
         """
-        Add an OAuth2 access token.<br><br>
-        @param token:An OAuth2 access token.
-        @return:This builder.
+        Deserialize from the format to a UUri.<br><br>
+        @param uri:serialized UUri.
+        @return:Returns a UUri object from the serialized format from the wire.
         """
-        self.mToken = token
-        return self
+        pass
 
-    def build(self):
+    @abstractmethod
+    def serialize(self, uri: UUri) -> T:
         """
-        Construct a <code>CallOptions</code> from this builder.<br><br>
-        @return:A constructed <code>CallOptions</code>.
+        Serialize from a UUri to a specific serialization format.<br><br>
+        @param uri:UUri object to be serialized to the format T.
+        @return:Returns the UUri in the transport serialized format.
         """
-        return CallOptions(self.mTimeout, self.mToken)
+        pass
```

### Comparing `up_python-0.1.1.dev0/uprotocol/rpc/rpcclient.py` & `up_python-0.1.2.dev0/uprotocol/rpc/rpcclient.py`

 * *Files 8% similar despite different names*

```diff
@@ -26,35 +26,39 @@
 
 
 from abc import ABC, abstractmethod
 from concurrent.futures import Future
 
 from uprotocol.proto.uri_pb2 import UUri
 from uprotocol.proto.upayload_pb2 import UPayload
-from uprotocol.rpc.calloptions import CallOptions
+from uprotocol.proto.uattributes_pb2 import CallOptions
 
 
 class RpcClient(ABC):
     """
-    RpcClient is an interface used by code generators for uProtocol services defined in proto files such as the core
-    uProtocol services found in <a href=https://github.com/eclipse-uprotocol/uprotocol-core-api>here</a>.<br> The
-    interface provides a
-    clean contract for all transports to implement to be able to support RPC on their platform.<br> Each platform MUST
-    implement this interface.<br> For more details please refer to<br>
-    <a href=https://github.com/eclipse-uprotocol/uprotocol-spec/blob/main/up-l2/README.adoc>[RpcClient
-    Specifications]</a>
+    RpcClient is an interface used by code generators for uProtocol services
+    defined in proto files such as the core
+    uProtocol services found in
+    <a href=https://github.com/eclipse-uprotocol/uprotocol-core-api>here
+    </a>.<br> The interface provides a clean contract for all transports
+    to implement to be able to support RPC on their platform.<br>
+    Each platform MUST implement this interface.<br>
     """
 
     @abstractmethod
-    def invoke_method(self, methodUri: UUri, request_payload: UPayload, options: CallOptions) -> Future:
+    def invoke_method(
+        self, methodUri: UUri, request_payload: UPayload, options: CallOptions
+    ) -> Future:
         """
-        API for clients to invoke a method (send an RPC request) and receive the response (the returned 
-        Future UMessage. <br>
-        Client will set method to be the URI of the method they want to invoke, 
-        payload to the request message, and attributes with the various metadata for the 
-        method invocation.
-        @param methodUri The method URI to be invoked, ex (long form): /example.hello_world/1/rpc.SayHello.
-        @param requestPayload The request message to be sent to the server.
+        API for clients to invoke a method (send an RPC request) and
+        receive the response (the returned Future UMessage. <br>
+        Client will set method to be the URI of the method they want to invoke,
+        payload to the request message, and attributes
+        with the various metadata for the method invocation.
+        @param methodUri The method URI to be invoked,
+        ex (long form): /example.hello_world/1/rpc.SayHello.
+        @param requestPayload The request
+        message to be sent to the server.
         @param options RPC method invocation call options, see CallOptions
         @return: Returns the CompletableFuture with the result or exception.
         """
         pass
```

### Comparing `up_python-0.1.1.dev0/uprotocol/rpc/rpcmapper.py` & `up_python-0.1.2.dev0/uprotocol/rpc/rpcmapper.py`

 * *Files 4% similar despite different names*

```diff
@@ -28,55 +28,70 @@
 from concurrent.futures import Future
 
 from google.protobuf import any_pb2
 from uprotocol.proto.ustatus_pb2 import UCode
 from uprotocol.proto.ustatus_pb2 import UStatus
 
 from uprotocol.rpc.rpcresult import RpcResult
-from uprotocol.proto.upayload_pb2 import UPayload
 
 
 class RpcMapper:
     """
-    RPC Wrapper is an interface that provides static methods to be able to wrap an RPC request with an RPC Response (
-    uP-L2). APIs that return Message assumes that the message is protobuf serialized com.google.protobuf.Any (
+    RPC Wrapper is an interface that provides static methods to be able to
+    wrap an RPC request with an RPC Response (
+    uP-L2). APIs that return Message assumes that the message is
+    protobuf serialized com.google.protobuf.Any (
     UMessageFormat.PROTOBUF) and will barf if anything else is passed
     """
 
     @staticmethod
     def map_response(message_future: Future, expected_cls):
         """
-         Map a response of CompletableFuture&lt;UMessage&gt; from Link into a CompletableFuture containing the
-         declared expected return type of the RPC method or an exception.<br><br>
-        @param response_future:CompletableFuture&lt;UMessage&gt; response from uTransport.
-        @param expected_cls:The class name of the declared expected return type of the RPC method.
-        @return:Returns a CompletableFuture containing the declared expected return type of the RPC method or an
+         Map a response of CompletableFuture&lt;UMessage&gt; from Link
+         into a CompletableFuture containing the
+         declared expected return type of the RPC method or an
+         exception.<br><br>
+        @param response_future:CompletableFuture&lt;UMessage&gt;
+        response from uTransport.
+        @param expected_cls:The class name of the declared expected
+        return type of the RPC method.
+        @return:Returns a CompletableFuture containing the declared
+        expected return type of the RPC method or an
         exception.
         """
         response_future: Future = Future()
 
         def handle_response(message):
             nonlocal response_future
             message = message.result()
-            if not message or not message.HasField('payload'):
+            if not message or not message.HasField("payload"):
                 response_future.set_exception(
-                    RuntimeError(f"Server returned a null payload. Expected {expected_cls.__name__}"))
-
+                    RuntimeError(
+                        f"Server returned a null payload. Expected {expected_cls.__name__}"
+                    )
+                )
+                return response_future
             try:
                 any_message = any_pb2.Any()
                 any_message.ParseFromString(message.payload.value)
                 if any_message.Is(expected_cls.DESCRIPTOR):
-                    response_future.set_result(RpcMapper.unpack_payload(any_message, expected_cls))
+                    response_future.set_result(
+                        RpcMapper.unpack_payload(any_message, expected_cls)
+                    )
                 else:
                     response_future.set_exception(
                         RuntimeError(
-                            f"Unknown payload type [{any_message.type_url}]. Expected [{expected_cls.__name__}]"))
+                            f"Unknown payload type [{any_message.type_url}]. Expected [{expected_cls.__name__}]"
+                        )
+                    )
 
             except Exception as e:
-                response_future.set_exception(RuntimeError(f"{str(e)} [{UStatus.__name__}]"))
+                response_future.set_exception(
+                    RuntimeError(f"{str(e)} [{UStatus.__name__}]")
+                )
 
         message_future.add_done_callback(handle_response)
 
         return response_future
 
     @staticmethod
     def map_response_to_result(response_future: Future, expected_cls):
@@ -88,54 +103,69 @@
         @return:Returns a CompletableFuture containing an RpcResult containing the declared expected return type T,
         or a UStatus containing any errors.
         """
 
         def handle_response(message):
             if message.exception():
                 exception = message.exception()
-                return RpcResult.failure(value=exception, message=str(exception))
+                return RpcResult.failure(
+                    value=exception, message=str(exception)
+                )
 
             message = message.result()
-            if not message or not message.HasField('payload'):
-                exception = RuntimeError(f"Server returned a null payload. Expected {expected_cls.__name__}")
-                return RpcResult.failure(value=exception, message=str(exception))
+            if not message or not message.HasField("payload"):
+                exception = RuntimeError(
+                    f"Server returned a null payload. Expected {expected_cls.__name__}"
+                )
+                return RpcResult.failure(
+                    value=exception, message=str(exception)
+                )
 
             try:
                 any_message = any_pb2.Any()
                 any_message.ParseFromString(message.payload.value)
 
                 if any_message.Is(expected_cls.DESCRIPTOR):
                     if expected_cls == UStatus:
                         return RpcMapper.calculate_status_result(any_message)
                     else:
-                        return RpcResult.success(RpcMapper.unpack_payload(any_message, expected_cls))
+                        return RpcResult.success(
+                            RpcMapper.unpack_payload(any_message, expected_cls)
+                        )
 
                 if any_message.Is(UStatus.DESCRIPTOR):
                     return RpcMapper.calculate_status_result(any_message)
             except Exception as e:
                 exception = RuntimeError(f"{str(e)} [{UStatus.__name__}]")
-                return RpcResult.failure(value=exception, message=str(exception))
+                return RpcResult.failure(
+                    value=exception, message=str(exception)
+                )
 
             exception = RuntimeError(
-                f"Unknown payload type [{any_message.type_url}]. Expected [{expected_cls.DESCRIPTOR.full_name}]")
+                f"Unknown payload type [{any_message.type_url}]. Expected [{expected_cls.DESCRIPTOR.full_name}]"
+            )
             return RpcResult.failure(value=exception, message=str(exception))
 
         result = None  # Initialize result
 
         def callback_wrapper(payload):
             nonlocal result
             result = handle_response(payload)
 
         response_future.add_done_callback(callback_wrapper)
         return result
 
     @staticmethod
     def calculate_status_result(payload):
         status = RpcMapper.unpack_payload(payload, UStatus)
-        return RpcResult.success(status) if status.code == UCode.OK else RpcResult.failure(status)
+        return (
+            RpcResult.success(status)
+            if status.code == UCode.OK
+            else RpcResult.failure(status)
+        )
 
     @staticmethod
     def unpack_payload(payload, expected_cls):
         """
         Unpack a payload of type Any into an object of type T, which is what was packing into the Any
         object.<br><br>
         @param payload:an Any message containing a type of expectedClazz.
```

### Comparing `up_python-0.1.1.dev0/uprotocol/rpc/rpcresult.py` & `up_python-0.1.2.dev0/uprotocol/rpc/rpcresult.py`

 * *Files 4% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 
 from abc import ABC, abstractmethod
 from typing import Callable, TypeVar, Union
 
 from uprotocol.proto.ustatus_pb2 import UCode
 from uprotocol.proto.ustatus_pb2 import UStatus
 
-T = TypeVar('T')
+T = TypeVar("T")
 
 
 class RpcResult(ABC):
     """
     Wrapper class for RPC Stub calls. It contains a Success with the type of the RPC call, or a failure with the
     UStatus returned by the failed call.
     """
@@ -49,44 +49,51 @@
         pass
 
     @abstractmethod
     def getOrElse(self, default_value: Callable[[], T]) -> T:
         pass
 
     @abstractmethod
-    def map(self, f: Callable[[T], T]) -> 'RpcResult':
+    def map(self, f: Callable[[T], T]) -> "RpcResult":
         pass
 
     @abstractmethod
-    def flatMap(self, f: Callable[[T], 'RpcResult']) -> 'RpcResult':
+    def flatMap(self, f: Callable[[T], "RpcResult"]) -> "RpcResult":
         pass
 
     @abstractmethod
-    def filter(self, f: Callable[[T], bool]) -> 'RpcResult':
+    def filter(self, f: Callable[[T], bool]) -> "RpcResult":
         pass
 
     @abstractmethod
     def failureValue(self) -> UStatus:
         pass
 
     @abstractmethod
     def successValue(self) -> T:
         pass
 
     @staticmethod
-    def success(value: T) -> 'RpcResult':
+    def success(value: T) -> "RpcResult":
         return Success(value)
 
     @staticmethod
-    def failure(value: Union[UStatus,'Failure', Exception,] = None, code: UCode = UCode.UNKNOWN,
-                message: str = '') -> 'RpcResult':
+    def failure(
+        value: Union[
+            UStatus,
+            "Failure",
+            Exception,
+        ] = None,
+        code: UCode = UCode.UNKNOWN,
+        message: str = "",
+    ) -> "RpcResult":
         return Failure(value, code, message)
 
     @staticmethod
-    def flatten(result: 'RpcResult') -> 'RpcResult':
+    def flatten(result: "RpcResult") -> "RpcResult":
         return result.flatMap(lambda x: x)
 
 
 class Success(RpcResult):
 
     def __init__(self, value: T):
         self.value = value
@@ -111,15 +118,21 @@
         try:
             return f(self.successValue())
         except Exception as e:
             return self.failure(e)
 
     def filter(self, f: Callable[[T], bool]) -> RpcResult:
         try:
-            return self if f(self.successValue()) else self.failure(code=UCode.FAILED_PRECONDITION, message="filtered out")
+            return (
+                self
+                if f(self.successValue())
+                else self.failure(
+                    code=UCode.FAILED_PRECONDITION, message="filtered out"
+                )
+            )
         except Exception as e:
             return self.failure(e)
 
     def failureValue(self) -> UStatus:
         raise ValueError("Method failureValue() called on a Success instance")
 
     def successValue(self) -> T:
@@ -127,15 +140,20 @@
 
     def __str__(self) -> str:
         return f"Success({self.successValue()})"
 
 
 class Failure(RpcResult):
 
-    def __init__(self, value: Union[UStatus,'Failure', Exception, None] = None, code: UCode = UCode.UNKNOWN, message: str = ''):
+    def __init__(
+        self,
+        value: Union[UStatus, "Failure", Exception, None] = None,
+        code: UCode = UCode.UNKNOWN,
+        message: str = "",
+    ):
         if isinstance(value, UStatus):
             self.value = value
         elif isinstance(value, Exception):
             self.value = UStatus(code=code, message=str(value))
         elif isinstance(value, Failure):
             self.value = value.failureValue()
         else:
```

### Comparing `up_python-0.1.1.dev0/uprotocol/rpc/urpclistener.py` & `up_python-0.1.2.dev0/uprotocol/transport/ulistener.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,27 +20,26 @@
 # under the License.
 # SPDX-FileType: SOURCE
 # SPDX-FileCopyrightText: 2023 General Motors GTO LLC
 # SPDX-License-Identifier: Apache-2.0
 
 # -------------------------------------------------------------------------
 
+
 from abc import ABC, abstractmethod
-from concurrent.futures import Future
 
 from uprotocol.proto.umessage_pb2 import UMessage
 
-class URpcListener(ABC):
-    '''
-    uService (servers) implement this to receive requests messages from clients. <br>
-    The service must implement the onReceive(UMessage, CompletableFuture) method to handle
-    the request and then complete the future passed to the method that triggers the uLink library to
-    send (over the transport) the response.
-    '''
-    
+
+class UListener(ABC):
+    """
+    For any implementation that defines some kind of callback or function that will be called to handle incoming
+    messages.
+    """
+
     @abstractmethod
-    def on_receive(message: UMessage, response_future: Future) -> None:
-        '''
-        Method called to handle/process events.
-        @param message Message received.
-        '''
-        pass
+    def on_receive(self, umsg: UMessage) -> None:
+        """
+        Method called to handle/process messages.<br><br>
+        @param umsg: UMessage to be sent.
+        """
+        pass
```

### Comparing `up_python-0.1.1.dev0/uprotocol/transport/README.adoc` & `up_python-0.1.2.dev0/uprotocol/transport/README.adoc`

 * *Files identical despite different names*

### Comparing `up_python-0.1.1.dev0/uprotocol/transport/builder/uattributesbuilder.py` & `up_python-0.1.2.dev0/uprotocol/transport/builder/uattributesbuilder.py`

 * *Files 13% similar despite different names*

```diff
@@ -20,31 +20,42 @@
 # under the License.
 # SPDX-FileType: SOURCE
 # SPDX-FileCopyrightText: 2023 General Motors GTO LLC
 # SPDX-License-Identifier: Apache-2.0
 
 # -------------------------------------------------------------------------
 
+from multimethod import multimethod
+from typing import Union
 
-from uprotocol.proto.uattributes_pb2 import UAttributes, UPriority, UMessageType
+from uprotocol.proto.uattributes_pb2 import (
+    UAttributes,
+    UPriority,
+    UMessageType,
+)
 from uprotocol.proto.uri_pb2 import UUri
+from uprotocol.proto.ustatus_pb2 import UCode
 from uprotocol.proto.uuid_pb2 import UUID
-from uprotocol.uuid.factory.uuidfactory import *
+from uprotocol.uuid.factory.uuidfactory import Factories
 
 
 class UAttributesBuilder:
     """
-    Construct the UAttributesBuilder with the configurations that are required for every payload transport.
+    Construct the UAttributesBuilder with the configurations that are
+    required for every payload transport.
 
     @param id       Unique identifier for the message.
-    @param type     Message type such as Publish a state change, RPC request or RPC response.
+    @param type     Message type such as Publish a state change,
+    RPC request or RPC response.
     @param priority uProtocol Prioritization classifications.
     """
 
-    def __init__(self, source: UUri, id: UUID, type: UMessageType, priority: UPriority):
+    def __init__(
+        self, source: UUri, id: UUID, type: UMessageType, priority: UPriority
+    ):
         self.source = source
         self.id = id
         self.type = UMessageType.Name(type)
         self.priority = priority
         self.ttl = None
         self.token = None
         self.sink = None
@@ -61,75 +72,117 @@
         @param priority The priority of the message.
         @return Returns the UAttributesBuilder with the configured priority.
         """
         if source is None:
             raise ValueError("Source cannot be None.")
         if priority is None:
             raise ValueError("UPriority cannot be None.")
-        return UAttributesBuilder(source, Factories.UPROTOCOL.create(), UMessageType.UMESSAGE_TYPE_PUBLISH, priority)
+        return UAttributesBuilder(
+            source,
+            Factories.UPROTOCOL.create(),
+            UMessageType.UMESSAGE_TYPE_PUBLISH,
+            priority,
+        )
 
     @staticmethod
     def notification(source: UUri, sink: UUri, priority: UPriority):
         """
         Construct a UAttributesBuilder for a notification message.
         @param source   Source address of the message.
         @param sink     The destination URI.
         @param priority The priority of the message.
-        @return Returns the UAttributesBuilder with the configured source, priority and sink.
+        @return Returns the UAttributesBuilder with the configured source,
+        priority and sink.
         """
         if source is None:
             raise ValueError("Source cannot be None.")
         if priority is None:
             raise ValueError("UPriority cannot be null.")
         if sink is None:
             raise ValueError("sink cannot be null.")
-        return UAttributesBuilder(source, Factories.UPROTOCOL.create(), UMessageType.UMESSAGE_TYPE_PUBLISH, priority
-                                  ).withSink(sink)
+        return UAttributesBuilder(
+            source,
+            Factories.UPROTOCOL.create(),
+            UMessageType.UMESSAGE_TYPE_NOTIFICATION,
+            priority,
+        ).withSink(sink)
 
     @staticmethod
     def request(source: UUri, sink: UUri, priority: UPriority, ttl: int):
         """
         Construct a UAttributesBuilder for a request message.
         @param source   Source address of the message.
         @param sink     The destination URI.
         @param priority The priority of the message.
         @param ttl      The time to live in milliseconds.
-        @return Returns the UAttributesBuilder with the configured priority, sink and ttl.
+        @return Returns the UAttributesBuilder with the configured
+        priority, sink and ttl.
         """
         if source is None:
             raise ValueError("Source cannot be None.")
         if priority is None:
             raise ValueError("UPriority cannot be null.")
         if sink is None:
             raise ValueError("sink cannot be null.")
         if ttl is None:
             raise ValueError("ttl cannot be null.")
 
-        return UAttributesBuilder(source, Factories.UPROTOCOL.create(), UMessageType.UMESSAGE_TYPE_REQUEST, priority
-                                  ).withTtl(ttl).withSink(sink)
-
-    @staticmethod
-    def response(source: UUri,  sink: UUri, priority: UPriority, reqid: UUID):
+        return (
+            UAttributesBuilder(
+                source,
+                Factories.UPROTOCOL.create(),
+                UMessageType.UMESSAGE_TYPE_REQUEST,
+                priority,
+            )
+            .withTtl(ttl)
+            .withSink(sink)
+        )
+
+    @multimethod
+    def response(
+        source: Union[UUri, None],
+        sink: Union[UUri, None],
+        priority: Union[int, None],
+        reqid: Union[UUID, None],
+    ):
         """
         Construct a UAttributesBuilder for a response message.
         @param source   Source address of the message.
         @param sink     The destination URI.
         @param priority The priority of the message.
-        @param reqid    The original request UUID used to correlate the response to the request.
-        @return Returns the UAttributesBuilder with the configured priority, sink and reqid.
+        @param reqid    The original request UUID used to correlate the
+        response to the request.
+        @return Returns the UAttributesBuilder with the configured priority,
+        sink and reqid.
         """
         if priority is None:
             raise ValueError("UPriority cannot be null.")
         if sink is None:
             raise ValueError("sink cannot be null.")
         if reqid is None:
             raise ValueError("reqid cannot be null.")
 
-        return UAttributesBuilder(source, Factories.UPROTOCOL.create(), UMessageType.UMESSAGE_TYPE_RESPONSE, priority
-                                  ).withSink(sink).withReqId(reqid)
+        return (
+            UAttributesBuilder(
+                source,
+                Factories.UPROTOCOL.create(),
+                UMessageType.UMESSAGE_TYPE_RESPONSE,
+                priority,
+            )
+            .withSink(sink)
+            .withReqId(reqid)
+        )
+
+    @multimethod
+    def response(request: Union[UAttributes, None]):
+        if request is None:
+            raise ValueError("request cannot be null.")
+        return UAttributesBuilder.response(
+            request.sink, request.source, request.priority, request.id
+        )
 
     def withTtl(self, ttl: int):
         """
         Add the time to live in milliseconds.
 
         @param ttl the time to live in milliseconds.
         @return Returns the UAttributesBuilder with the configured ttl.
@@ -142,15 +195,15 @@
         dd the authorization token used for TAP.
 
         @param token the authorization token used for TAP.
         @return Returns the UAttributesBuilder with the configured token.
         """
         self.token = token
         return self
-    
+
     def withSink(self, sink: UUri):
         """
         Add the explicit destination URI.
 
         @param sink the explicit destination URI.
         @return Returns the UAttributesBuilder with the configured sink.
         """
@@ -163,15 +216,15 @@
 
         @param plevel the permission level of the message.
         @return Returns the UAttributesBuilder with the configured plevel.
         """
         self.plevel = plevel
         return self
 
-    def withCommStatus(self, commstatus: int):
+    def withCommStatus(self, commstatus: UCode):
         """
         Add the communication status of the message.
 
         @param commstatus the communication status of the message.
         @return Returns the UAttributesBuilder with the configured commstatus.
         """
         self.commstatus = commstatus
@@ -182,41 +235,46 @@
         Add the request ID.
 
         @param reqid the request ID.
         @return Returns the UAttributesBuilder with the configured reqid.
         """
         self.reqid = reqid
         return self
-    
+
     def withTraceparent(self, traceparent: str):
         """
         Add the traceparent.
 
         @param reqid    the traceparent.
-        @return Returns the UAttributesBuilder with the configured traceparent.
+        @return Returns the UAttributesBuilder with the configured
+        traceparent.
         """
         self.traceparent = traceparent
         return self
 
-
     def build(self):
         """
         Construct the UAttributes from the builder.
 
         @return Returns a constructed
         """
-        attributes = UAttributes(source=self.source, id=self.id, type=self.type, priority=self.priority)
+        attributes = UAttributes(
+            source=self.source,
+            id=self.id,
+            type=self.type,
+            priority=self.priority,
+        )
         if self.sink is not None:
             attributes.sink.CopyFrom(self.sink)
         if self.ttl is not None:
             attributes.ttl = self.ttl
         if self.plevel is not None:
             attributes.permission_level = self.plevel
         if self.commstatus is not None:
             attributes.commstatus = self.commstatus
         if self.reqid is not None:
             attributes.reqid.CopyFrom(self.reqid)
         if self.traceparent is not None:
             attributes.traceparent = self.traceparent
-        if self.token != None:
+        if self.token is not None:
             attributes.token = self.token
         return attributes
```

### Comparing `up_python-0.1.1.dev0/uprotocol/transport/builder/upayloadbuilder.py` & `up_python-0.1.2.dev0/uprotocol/transport/builder/upayloadbuilder.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,59 +20,70 @@
 # under the License.
 # SPDX-FileType: SOURCE
 # SPDX-FileCopyrightText: 2023 General Motors GTO LLC
 # SPDX-License-Identifier: Apache-2.0
 
 # -------------------------------------------------------------------------
 
-import typing
+from typing import Optional, Type
 
 from uprotocol.proto.upayload_pb2 import UPayload, UPayloadFormat
 from google.protobuf.any_pb2 import Any
-from google.protobuf import message
+from google.protobuf.message import Message
+
 
 class UPayloadBuilder:
-    
-    def pack_to_any(message: message) -> UPayload:
-        '''
-        Build a uPayload from google.protobuf.Message by stuffing the message into an Any. 
+
+    @staticmethod
+    def pack_to_any(message: Message) -> UPayload:
+        """
+        Build a uPayload from google.protobuf.Message by stuffing the message into an Any.
         @param message the message to pack
-        @return the UPayload 
-        '''
+        @return the UPayload
+        """
         any_message = Any()
         any_message.Pack(message)
-        return UPayload(format=UPayloadFormat.UPAYLOAD_FORMAT_PROTOBUF_WRAPPED_IN_ANY,
-                           value=any_message.SerializeToString())
-    
-    def pack(message: message) -> UPayload:
-        '''
+        return UPayload(
+            format=UPayloadFormat.UPAYLOAD_FORMAT_PROTOBUF_WRAPPED_IN_ANY,
+            value=any_message.SerializeToString(),
+        )
+
+    @staticmethod
+    def pack(message: Message) -> UPayload:
+        """
         Build a uPayload from google.protobuf.Message using protobuf PayloadFormat.
         @param message the message to pack
         @return the UPayload
-        '''
-        return UPayload(format=UPayloadFormat.UPAYLOAD_FORMAT_PROTOBUF,
-                           value=message.SerializeToString())
+        """
+        return UPayload(
+            format=UPayloadFormat.UPAYLOAD_FORMAT_PROTOBUF,
+            value=message.SerializeToString(),
+        )
 
-    def unpack(payload: UPayload, clazz: typing.Type) -> typing.Type:
-        '''
+    @staticmethod
+    def unpack(payload: UPayload, clazz: Type[Message]) -> Optional[Message]:
+        """
         Unpack a uPayload into a google.protobuf.Message.
         @param payload the payload to unpack
         @param clazz the class of the message to unpack
         @return the unpacked message
-        '''
+        """
         if payload is None or payload.value is None:
             return None
         try:
             if payload.format == UPayloadFormat.UPAYLOAD_FORMAT_PROTOBUF:
                 message = clazz()
                 message.ParseFromString(payload.value)
                 return message
-            elif payload.format == UPayloadFormat.UPAYLOAD_FORMAT_PROTOBUF_WRAPPED_IN_ANY:
+            elif (
+                payload.format
+                == UPayloadFormat.UPAYLOAD_FORMAT_PROTOBUF_WRAPPED_IN_ANY
+            ):
                 any_message = Any()
                 any_message.ParseFromString(payload.value)
                 message = clazz()
                 any_message.Unpack(message)
                 return message
             else:
                 return None
-        except:
-            return None
+        except Exception:
+            return None
```

### Comparing `up_python-0.1.1.dev0/uprotocol/transport/utransport.py` & `up_python-0.1.2.dev0/uprotocol/transport/utransport.py`

 * *Files 1% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from abc import ABC, abstractmethod
 
 from uprotocol.proto.uri_pb2 import UUri
 from uprotocol.transport.ulistener import UListener
 from uprotocol.proto.ustatus_pb2 import UStatus
 from uprotocol.proto.umessage_pb2 import UMessage
 
+
 class UTransport(ABC):
     """
     UTransport is the  uP-L1 interface that provides a common API for uE developers to send and receive
     messages.<br>UTransport implementations contain the details for connecting to the underlying transport technology
     and sending UMessage using the configured technology.<br>For more information please refer to
     <a href =https://github.com/eclipse-uprotocol/uprotocol-spec/blob/main/up-l1/README.adoc>link</a>
     """
@@ -50,15 +51,15 @@
         pass
 
     @abstractmethod
     def register_listener(self, topic: UUri, listener: UListener) -> UStatus:
         """
         Register UListener for UUri topic to be called when a message is received.
         @param topic UUri to listen for messages from.
-        @param listener The UListener that will be execute when the message is 
+        @param listener The UListener that will be execute when the message is
         received on the given UUri.
         @return Returns UStatus with UCode.OK if the listener is registered
         correctly, otherwise it returns with the appropriate failure.
         """
         pass
 
     @abstractmethod
```

### Comparing `up_python-0.1.1.dev0/uprotocol/transport/validate/uattributesvalidator.py` & `up_python-0.1.2.dev0/uprotocol/transport/validate/uattributesvalidator.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -------------------------------------------------------------------------
 import time
+
 # Copyright (c) 2023 General Motors GTO LLC
 #
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
@@ -24,271 +25,409 @@
 
 # -------------------------------------------------------------------------
 
 
 from abc import abstractmethod
 from enum import Enum
 from uprotocol.proto.uri_pb2 import UUri
-from uprotocol.proto.uattributes_pb2 import UAttributes, UMessageType
-from uprotocol.proto.ustatus_pb2 import UCode
+from uprotocol.proto.uattributes_pb2 import (
+    UAttributes,
+    UMessageType,
+    UPriority,
+)
 from uprotocol.uri.validator.urivalidator import UriValidator
 from uprotocol.uuid.factory.uuidutils import UUIDUtils
 from uprotocol.validation.validationresult import ValidationResult
 
 
 class UAttributesValidator:
     """
-    UAttributes is the class that defines the Payload. It is the place for configuring time to live, priority,
+    UAttributes is the class that defines the Payload. It is the place
+    for configuring time to live, priority,
     security tokens and more.<br><br>
-    Each UAttributes class defines a different type of message payload. The payload can represent a simple published
-    payload with some state change,Payload representing an RPC request or Payload representing an RPC response.<br><br>
-    UAttributesValidator is a base class for all UAttribute validators, that can help validate that the
+    Each UAttributes class defines a different type of message payload.
+    The payload can represent a simple published
+    payload with some state change,Payload representing an RPC
+    request or Payload representing an RPC response.<br><br>
+    UAttributesValidator is a base class for all UAttribute
+    validators, that can help validate that the
     UAttributes object is correctly defined to define the Payload correctly.
 
     """
 
     @staticmethod
     def get_validator(attribute: UAttributes):
         """
-        Static factory method for getting a validator according to the UMessageType defined in the
+        Static factory method for getting a validator according to the
+        UMessageType defined in the
         UAttributes.<br>
         @param attribute: UAttributes containing the UMessageType.
-        @return: returns a UAttributesValidator according to the UMessageType defined in the
+        @return: returns a UAttributesValidator according to the
+        UMessageType defined in the
         UAttributes.
         """
         if attribute.type is None:
             return Validators.PUBLISH.validator()
         elif attribute.type == UMessageType.UMESSAGE_TYPE_RESPONSE:
             return Validators.RESPONSE.validator()
         elif attribute.type == UMessageType.UMESSAGE_TYPE_REQUEST:
             return Validators.REQUEST.validator()
+        elif attribute.type == UMessageType.UMESSAGE_TYPE_NOTIFICATION:
+            return Validators.NOTIFICATION.validator()
         else:
             return Validators.PUBLISH.validator()
 
     def validate(self, attributes: UAttributes) -> ValidationResult:
         """
         Take a UAttributes object and run validations.<br><br>
         @param attributes:The UAttriubes to validate.
-        @return:Returns a ValidationResult that is success or failed with a message containing all validation errors
+        @return:Returns a ValidationResult that is success or failed
+        with a message containing all validation errors
         for invalid configurations.
         """
-        error_messages = [self.validate_type(attributes),
-                          self.validate_ttl(attributes),
-                          self.validate_sink(attributes), self.validate_comm_status(attributes),
-                          self.validate_permission_level(attributes), self.validate_req_id(attributes)]
-
-        error_messages = [status.get_message() for status in error_messages if
-                          status.is_failure()]
+        error_messages = [
+            self.validate_type(attributes),
+            self.validate_ttl(attributes),
+            self.validate_sink(attributes),
+            self.validate_priority(attributes),
+            self.validate_permission_level(attributes),
+            self.validate_req_id(attributes),
+        ]
+
+        error_messages = [
+            status.get_message()
+            for status in error_messages
+            if status.is_failure()
+        ]
 
         if error_messages:
             return ValidationResult.failure(",".join(error_messages))
         else:
             return ValidationResult.success()
 
     @staticmethod
     def is_expired(u_attributes: UAttributes) -> bool:
-        '''
+        """
         Check the time-to-live attribute to see if it has expired. <br>
-        The message has expired when the current time is greater than the original UUID time
+        The message has expired when the current time is greater
+        than the original UUID time
         plus the ttl attribute.
         @param uAttributes UAttributes with time to live value.
-        @return Returns a true if the original time plus the ttl is less than the current time
-        '''
+        @return Returns a true if the original time plus the ttl
+        is less than the current time
+        """
         ttl = u_attributes.ttl
-        maybe_time = UUIDUtils.getTime(u_attributes.id)
+        maybe_time = UUIDUtils.get_time(u_attributes.id)
 
-        if not u_attributes.HasField('ttl') or maybe_time is None or ttl <=0:
+        if maybe_time is None or ttl <= 0:
             return False
-    
+
         return (maybe_time + ttl) < int(time.time() * 1000)
 
     @staticmethod
     def validate_ttl(attr: UAttributes) -> ValidationResult:
         """
-        Validate the time to live configuration. If the UAttributes does not contain a time to live then the
+        Validate the time to live configuration. If the UAttributes
+        does not contain a time to live then the
         ValidationResult
         is ok.<br><br>
-        @param attr:UAttributes object containing the message time to live configuration to validate.
-        @return:Returns a  ValidationResult that is success or failed with a failure message.
+        @param attr:UAttributes object containing the message time
+        to live configuration to validate.
+        @return:Returns a  ValidationResult that is success or
+        failed with a failure message.
         """
-        if attr.HasField('ttl') and attr.ttl <= 0:
-            return ValidationResult.failure(f"Invalid TTL [{attr.ttl}]")
-        else:
-            return ValidationResult.success()
+        return ValidationResult.success()
 
     @staticmethod
     def validate_sink(attr: UAttributes) -> ValidationResult:
         """
-        Validate the sink UriPart for the default case. If the UAttributes does not contain a sink then the
+        Validate the sink UriPart for the default case. If the
+        UAttributes does not contain a sink then the
         ValidationResult
         is ok.<br><br>
         @param attr:UAttributes object containing the sink to validate.
-        @return:Returns a  ValidationResult that is success or failed with a failure message.
+        @return:Returns a  ValidationResult that is success or
+        failed with a failure message.
         """
-        return UriValidator.validate(attr.sink) if attr.HasField('sink') else ValidationResult.success()
+        return (
+            UriValidator.validate(attr.sink)
+            if attr.HasField("sink")
+            else ValidationResult.success()
+        )
+
+    @staticmethod
+    def validate_priority(attr: UAttributes):
+        """
+        Validate the priority value to ensure it is one of the known CS values
+
+        @param attributes Attributes object containing the
+        Priority to validate.
+        @return Returns a ValidationResult that is success or
+        failed with a failure message.
+        """
+        return (
+            ValidationResult.success()
+            if attr.priority >= UPriority.UPRIORITY_CS0
+            else ValidationResult.failure(
+                f"Invalid UPriority [{UPriority.Name(attr.priority)}]"
+            )
+        )
 
     @staticmethod
     def validate_permission_level(attr: UAttributes) -> ValidationResult:
         """
-        Validate the permissionLevel for the default case. If the UAttributes does not contain a permission level
+        Validate the permissionLevel for the default case. If the
+        UAttributes does not contain a permission level
         then the  ValidationResult is ok.<br><br>
-        @param attr:UAttributes object containing the permission level to validate.
-        @return:Returns a  ValidationResult indicating if the permissionLevel is valid or not.
+        @param attr:UAttributes object containing the permission
+        level to validate.
+        @return:Returns a  ValidationResult indicating if the
+        permissionLevel is valid or not.
         """
-        if attr.HasField('permission_level') and attr.permission_level <= 0:
+        if attr.HasField("permission_level") and attr.permission_level <= 0:
             return ValidationResult.failure("Invalid Permission Level")
         else:
             return ValidationResult.success()
 
     @staticmethod
-    def validate_comm_status(attr: UAttributes) -> ValidationResult:
-        """
-        Validate the commStatus for the default case. If the UAttributes does not contain a comm status then the
-         ValidationResult is ok.<br><br>
-        @param attr:UAttributes object containing the comm status to validate.
-        @return:Returns a  ValidationResult that is success or failed with a failure message.
-        """
-        if attr.HasField('commstatus'):
-            try:
-                UCode.Name(attr.commstatus)
-            except ValueError:
-                return ValidationResult.failure("Invalid Communication Status Code")
-
-        return ValidationResult.success()
-
-    @staticmethod
     def validate_req_id(attr: UAttributes) -> ValidationResult:
         """
-        Validate the correlationId for the default case. If the UAttributes does not contain a request id then the
-         ValidationResult is ok.<br><br>
+        Validate the correlationId for the default case. If the
+        UAttributes does not contain a request id then the
+        ValidationResult is ok.<br><br>
         @param attr:Attributes object containing the request id to validate.
-        @return:Returns a  ValidationResult that is success or failed with a failure message.
+        @return:Returns a  ValidationResult that is
+        success or failed with a failure message.
         """
 
-        if attr.HasField('reqid') and not UUIDUtils.isuuid(attr.reqid):
+        if attr.HasField("reqid") and not UUIDUtils.is_uuid(attr.reqid):
             return ValidationResult.failure("Invalid UUID")
         else:
             return ValidationResult.success()
 
     @abstractmethod
     def validate_type(self, attr: UAttributes):
         """
         Validate the UMessageType attribute, it is required.<br><br>
-        @param attr:UAttributes object containing the message type to validate.
-        @return:Returns a  ValidationResult that is success or failed with a failure message.
+        @param attr:UAttributes object containing the
+        message type to validate.
+        @return:Returns a  ValidationResult that is success
+        or failed with a failure message.
         """
         raise NotImplementedError("Subclasses must implement this method.")
 
 
 class Publish(UAttributesValidator):
     """
-     Implements validations for UAttributes that define a message that is meant for publishing state changes.
+    Implements validations for UAttributes that define a message
+    that is meant for publishing state changes.
     """
 
     def validate_type(self, attributes_value: UAttributes) -> ValidationResult:
         """
-        Validates that attributes for a message meant to publish state changes has the correct type.<br><br>
-        @param attributes_value:UAttributes object containing the message type to validate.
-        @return:Returns a  ValidationResult that is success or failed with a failure message.
-        """
-        return ValidationResult.success() if attributes_value.type == UMessageType.UMESSAGE_TYPE_PUBLISH else (
-            ValidationResult.failure(
-                f"Wrong Attribute Type [{UMessageType.Name(attributes_value.type)}]"))
+        Validates that attributes for a message meant to publish
+        state changes has the correct type.<br><br>
+        @param attributes_value:UAttributes object containing
+        the message type to validate.
+        @return:Returns a  ValidationResult that is success or
+        failed with a failure message.
+        """
+        return (
+            ValidationResult.success()
+            if attributes_value.type == UMessageType.UMESSAGE_TYPE_PUBLISH
+            else (
+                ValidationResult.failure(
+                    f"Wrong Attribute Type [{UMessageType.Name(attributes_value.type)}]"
+                )
+            )
+        )
 
     def __str__(self):
         return "UAttributesValidator.Publish"
 
 
 class Request(UAttributesValidator):
     """
-    Implements validations for UAttributes that define a message that is meant for an RPC request.
+    Implements validations for UAttributes that define a message
+    that is meant for an RPC request.
     """
 
     def validate_type(self, attributes_value: UAttributes) -> ValidationResult:
         """
-        Validates that attributes for a message meant for an RPC request has the correct type.<br><br>
-        @param attributes_value:UAttributes object containing the message type to validate.
-        @return:Returns a  ValidationResult that is success or failed with a failure message.
-        """
-        return ValidationResult.success() if attributes_value.type == UMessageType.UMESSAGE_TYPE_REQUEST else (
-            ValidationResult.failure(
-                f"Wrong Attribute Type [{UMessageType.Name(attributes_value.type)}]"))
+        Validates that attributes for a message meant for an
+        RPC request has the correct type.<br><br>
+        @param attributes_value:UAttributes object containing
+        the message type to validate.
+        @return:Returns a  ValidationResult that is success
+        or failed with a failure message.
+        """
+        return (
+            ValidationResult.success()
+            if attributes_value.type == UMessageType.UMESSAGE_TYPE_REQUEST
+            else (
+                ValidationResult.failure(
+                    f"Wrong Attribute Type [{UMessageType.Name(attributes_value.type)}]"
+                )
+            )
+        )
 
     def validate_sink(self, attributes_value: UAttributes) -> ValidationResult:
         """
-        Validates that attributes for a message meant for an RPC request has a destination sink.<br><br> In the case
+        Validates that attributes for a message meant for an RPC
+        request has a destination sink.<br><br> In the case
         of an RPC request, the sink is required.
-        @param attributes_value:UAttributes object containing the sink to validate.
-        @return:Returns a  ValidationResult that is success or failed with a failure message.
-        """
-        return UriValidator.validate_rpc_method(
-            attributes_value.sink) if attributes_value.HasField('sink') else ValidationResult.failure("Missing Sink")
+        @param attributes_value:UAttributes object containing
+        the sink to validate.
+        @return:Returns a  ValidationResult that is success or
+        failed with a failure message.
+        """
+        return (
+            UriValidator.validate_rpc_method(attributes_value.sink)
+            if attributes_value.HasField("sink")
+            else ValidationResult.failure("Missing Sink")
+        )
 
     def validate_ttl(self, attributes_value: UAttributes) -> ValidationResult:
         """
-        Validate the time to live configuration.<br>In the case of an RPC request, the time to live is required.<br><br>
-        @param attributes_value:UAttributes object containing the time to live to validate.
-        @return:Returns a  ValidationResult that is success or failed with a failure message.
+        Validate the time to live configuration.<br>In the case of an RPC
+        request, the time to live is required.<br><br>
+        @param attributes_value:UAttributes object containing the
+        time to live to validate.
+        @return:Returns a  ValidationResult that is success or
+        failed with a failure message.
         """
-        if not attributes_value.HasField('ttl'):
+        if not attributes_value.HasField("ttl"):
             return ValidationResult.failure("Missing TTL")
-        if attributes_value.ttl <= 0:
-            return ValidationResult.failure(f"Invalid TTL [{attributes_value.ttl}]")
 
         return ValidationResult.success()
 
     def __str__(self):
         return "UAttributesValidator.Request"
 
 
 class Response(UAttributesValidator):
     """
-    Implements validations for UAttributes that define a message that is meant for an RPC response.
+    Implements validations for UAttributes that define a message that is
+    meant for an RPC response.
     """
 
     def validate_type(self, attributes_value: UAttributes) -> ValidationResult:
         """
-        Validates that attributes for a message meant for an RPC response has the correct type.<br><br>
-        @param attributes_value:UAttributes object containing the message type to validate.
-        @return:Returns a  ValidationResult that is success or failed with a failure message.
-        """
-        return ValidationResult.success() if attributes_value.type == UMessageType.UMESSAGE_TYPE_RESPONSE else (
-            ValidationResult.failure(
-                f"Wrong Attribute Type [{UMessageType.Name(attributes_value.type)}]"))
+        Validates that attributes for a message meant for an RPC
+        response has the correct type.<br><br>
+        @param attributes_value:UAttributes object containing the
+        message type to validate.
+        @return:Returns a  ValidationResult that is success or
+        failed with a failure message.
+        """
+        return (
+            ValidationResult.success()
+            if attributes_value.type == UMessageType.UMESSAGE_TYPE_RESPONSE
+            else (
+                ValidationResult.failure(
+                    f"Wrong Attribute Type [{UMessageType.Name(attributes_value.type)}]"
+                )
+            )
+        )
 
     def validate_sink(self, attributes_value: UAttributes) -> ValidationResult:
         """
-        Validates that attributes for a message meant for an RPC response has a destination sink.<br>In the case of
+        Validates that attributes for a message meant for an RPC response
+        has a destination sink.<br>In the case of
         an RPC response, the sink is required.<br><br>
-        @param attributes_value:UAttributes object containing the sink to validate.
-        @return:Returns a  ValidationResult that is success or failed with a failure message.
-        """
-        if not attributes_value.HasField('sink') or attributes_value.sink == UUri():
+        @param attributes_value:UAttributes object containing the sink
+        to validate.
+        @return:Returns a  ValidationResult that is success or failed
+        with a failure message.
+        """
+        if (
+            not attributes_value.HasField("sink")
+            or attributes_value.sink == UUri()
+        ):
             return ValidationResult.failure("Missing Sink")
         result = UriValidator.validate_rpc_response(attributes_value.sink)
         return result
 
+    def validate_req_id(
+        self, attributes_value: UAttributes
+    ) -> ValidationResult:
+        """
+        Validate the correlationId. n the case of an RPC response, the
+        correlation id is required.<br><br>
+        @param attributes_value:UAttributes object containing the
+        correlation id to validate.
+        @return:Returns a  ValidationResult that is success or
+        failed with a failure message.
+        """
+        return (
+            ValidationResult.success()
+            if attributes_value.reqid
+            and UUIDUtils.is_uuid(attributes_value.reqid)
+            else ValidationResult.failure("Missing correlationId")
+        )
+
+    def __str__(self):
+        return "UAttributesValidator.Response"
+
+
+class Notification(UAttributesValidator):
+    """
+    Implements validations for UAttributes that define a message that is
+    meant for notifications.
+    """
 
-    def validate_req_id(self, attributes_value: UAttributes) -> ValidationResult:
+    def validate_type(self, attributes_value: UAttributes) -> ValidationResult:
         """
-        Validate the correlationId. n the case of an RPC response, the correlation id is required.<br><br>
-        @param attributes_value:UAttributes object containing the correlation id to validate.
-        @return:Returns a  ValidationResult that is success or failed with a failure message.
+        Validates that attributes for a message meant for Notification
+        state changes has the correct type.<br><br>
+        @param attributes_value:UAttributes object containing the message
+        type to validate.
+        @return:Returns a ValidationResult that is success or failed with
+        a failure message.
+        """
+        return (
+            ValidationResult.success()
+            if attributes_value.type == UMessageType.UMESSAGE_TYPE_NOTIFICATION
+            else (
+                ValidationResult.failure(
+                    f"Wrong Attribute Type [{UMessageType.Name(attributes_value.type)}]"
+                )
+            )
+        )
+
+    def validate_sink(self, attributes_value: UAttributes) -> ValidationResult:
         """
-        return ValidationResult.success() if attributes_value.reqid and UUIDUtils.isuuid(
-            attributes_value.reqid) else ValidationResult.failure("Missing correlationId")
+        Validates that attributes for a message meant for an RPC response
+        has a destination sink.<br>In the case of
+        an RPC response, the sink is required.<br><br>
+        @param attributes_value:UAttributes object containing the
+        sink to validate.
+        @return:Returns a  ValidationResult that is success or
+        failed with a failure message.
+        """
+        if attributes_value is None:
+            return ValidationResult.failure("UAttributes cannot be null.")
+        if (
+            not attributes_value.HasField("sink")
+            or attributes_value.sink == UUri()
+        ):
+            return ValidationResult.failure("Missing Sink")
+        return ValidationResult.success()
 
     def __str__(self):
-        return "UAttributesValidator.Response"
+        return "UAttributesValidator.Notification"
 
 
 class Validators(Enum):
     """
-    Validators Factory. <br>Example: UAttributesValidator validateForPublishMessageType =
+    Validators Factory. <br>Example: UAttributesValidator
+    validateForPublishMessageType =
     UAttributesValidator.Validators.PUBLISH.validator()
     """
+
     PUBLISH = Publish()
     REQUEST = Request()
     RESPONSE = Response()
+    NOTIFICATION = Notification()
 
     def validator(self):
         return self.value
```

### Comparing `up_python-0.1.1.dev0/uprotocol/uri/README.adoc` & `up_python-0.1.2.dev0/uprotocol/uri/README.adoc`

 * *Files 26% similar despite different names*

```diff
@@ -27,19 +27,7 @@
 
 === Validating
 [,python]
 ----
 status : ValidationResult = UriValidator.validate_rpc_method(uuri)
 assertTrue(status.is_success());
 ----
-
-=== Serializing & Deserializing
-[,python]
-----
-        uri = .../* UUri example above */
-        micro = MicroUriSerializer().serialize(uri)
-        long = LongUriSerializer().serialize(uri)
-        deserialized_micro_uuri = MicroUriSerializer().deserialize(uri)
-        deserialized_long_uuri = LongUriSerializer().deserialize(uri)
-        uri2 = UriSerializer.build_resolved(long, micro)
-
-----
```

### Comparing `up_python-0.1.1.dev0/uprotocol/uri/factory/uentity_factory.py` & `up_python-0.1.2.dev0/uprotocol/uri/factory/uentity_factory.py`

 * *Files 15% similar despite different names*

```diff
@@ -19,44 +19,49 @@
 # specific language governing permissions and limitations
 # under the License.
 # SPDX-FileType: SOURCE
 # SPDX-FileCopyrightText: 2023 General Motors GTO LLC
 # SPDX-License-Identifier: Apache-2.0
 
 # -------------------------------------------------------------------------
+from google.protobuf.descriptor import ServiceDescriptor
+from google.protobuf.descriptor_pb2 import ServiceOptions
 
 from uprotocol.proto.uri_pb2 import UEntity
-from uprotocol.proto.uprotocol_options_pb2 import UProtocolOptions
-from google.protobuf.descriptor_pb2 import ServiceDescriptorProto
+from uprotocol.proto.uprotocol_options_pb2 import name as Name
+from uprotocol.proto.uprotocol_options_pb2 import (
+    version_major as Version_Major,
+)
+from uprotocol.proto.uprotocol_options_pb2 import (
+    version_minor as Version_Minor,
+)
+from uprotocol.proto.uprotocol_options_pb2 import id as Id
+
 
 class UEntityFactory:
     """
     Factory for creating UEntity objects.
     """
 
     @staticmethod
-    def from_proto(descriptor: ServiceDescriptorProto) -> UEntity:
-        '''
-        Builds a UEntity for an protobuf generated code Service Descriptor.
-        @param descriptor The protobuf generated code Service Descriptor.
-        @return Returns a UEntity for an protobuf generated code Service Descriptor.
-        '''
-
-        if descriptor is None:
+    def from_proto(service_descriptor: ServiceDescriptor):
+        if service_descriptor is None:
             return UEntity()
-        
-        options = descriptor.options
 
-        uentity = UEntity()
+        options: ServiceOptions = service_descriptor.GetOptions()
 
-        name = options.getExtension(UProtocolOptions.name)
-        id = options.getExtension(UProtocolOptions.id)
-        version = options.getExtension(UProtocolOptions.version_major)
-        
+        name: str = options.Extensions[Name]
+        version_major: int = options.Extensions[Version_Major]
+        version_minor: int = options.Extensions[Version_Minor]
+        id: int = options.Extensions[Id]
+
+        uentity = UEntity()
         if name is not None:
             uentity.name = name
+        if version_major is not None:
+            uentity.version_major = version_major
+        if version_minor is not None:
+            uentity.version_minor = version_minor
         if id is not None:
             uentity.id = id
-        if version is not None:
-            uentity.version_major = version
 
-        return uentity
+        return uentity
```

### Comparing `up_python-0.1.1.dev0/uprotocol/uri/factory/uresource_builder.py` & `up_python-0.1.2.dev0/uprotocol/uri/factory/uresource_builder.py`

 * *Files 20% similar despite different names*

```diff
@@ -21,47 +21,77 @@
 # SPDX-FileType: SOURCE
 # SPDX-FileCopyrightText: 2023 General Motors GTO LLC
 # SPDX-License-Identifier: Apache-2.0
 
 # -------------------------------------------------------------------------
 
 
+import re
 from uprotocol.proto.uri_pb2 import UResource
+from multimethod import multimethod
+from typing import Union
 
 
 class UResourceBuilder:
     MAX_RPC_ID = 1000
 
+    # The minimum topic ID, below this value are methods.
+    MIN_TOPIC_ID = 0x8000
+
     @staticmethod
     def for_rpc_response():
         return UResource(name="rpc", instance="response", id=0)
 
-    @staticmethod
-    def for_rpc_request(method, id=None):
+    @multimethod
+    def for_rpc_request(method: Union[str, None], id: int = None):
         uresource = UResource(name="rpc")
         if method is not None:
             uresource.instance = method
         if id is not None:
             uresource.id = id
 
         return uresource
 
-    @staticmethod
-    def for_rpc_request_with_id(id):
+    @multimethod
+    def for_rpc_request(id: int):
         return UResourceBuilder.for_rpc_request(None, id)
 
     @staticmethod
     def from_id(id):
         if id is None:
             raise ValueError("id cannot be None")
 
-        return UResourceBuilder.for_rpc_request_with_id(id) if id < UResourceBuilder.MAX_RPC_ID else UResource(id=id)
+        return (
+            UResourceBuilder.for_rpc_response()
+            if id == 0
+            else (
+                UResourceBuilder.for_rpc_request(id)
+                if id < UResourceBuilder.MIN_TOPIC_ID
+                else UResource(id=id)
+            )
+        )
 
     @staticmethod
-    def from_proto(instance):
-        '''
-        Build a UResource from a protobuf message. This method will determine if
-        the message is a RPC or topic message based on the message type
-        @param message The protobuf message.
+    def from_uservice_topic(topic):
+        """
+        Build a UResource from a UServiceTopic that is defined in protos and
+        available from generated stubs.
+        @param topic The UServiceTopic to build the UResource from.
         @return Returns a UResource for an RPC request.
-        '''
-        pass
+        """
+        if topic is None:
+            raise ValueError("topic cannot be None.")
+        name_and_instance_parts = re.split(r"[\\.]", topic.name)
+        resource_name = name_and_instance_parts[0]
+        resource_instance = (
+            None
+            if len(name_and_instance_parts) <= 1
+            else name_and_instance_parts[1]
+        )
+
+        resource = UResource(
+            name=resource_name, id=topic.id, message=topic.message
+        )
+        if resource_instance is not None:
+            resource.instance = resource_instance
+
+        return resource
```

### Comparing `up_python-0.1.1.dev0/uprotocol/uri/serializer/longuriserializer.py` & `up_python-0.1.2.dev0/uprotocol/uri/serializer/longuriserializer.py`

 * *Files 12% similar despite different names*

```diff
@@ -42,36 +42,38 @@
     https://github.com/eclipse-uprotocol/uprotocol-spec/blob/main/basics/uri.adoc</a>
     """
 
     def serialize(self, uri: UUri) -> str:
         """
         Support for serializing UUri objects into their String format.<br><br>
         @param uri: UUri object to be serialized to the String format.
-        @return:Returns the String format of the supplied UUri that can be used as a sink or a source in a
+        @return:Returns the String format of the supplied UUri that can be
+        used as a sink or a source in a
         uProtocol publish communication.
         """
         if uri is None or UriValidator.is_empty(uri):
             return ""
 
         sb = []
 
-        if uri.HasField('authority'):
-            sb.append(self.build_authority_part_of_uri(uri.authority))
+        if uri.HasField("authority"):
+            sb.append("//")
+            sb.append(uri.authority.name)
 
         sb.append("/")
 
         sb.append(self.build_software_entity_part_of_uri(uri.entity))
         sb.append(self.build_resource_part_of_uri(uri))
 
-        return re.sub('/+$', '', "".join(sb))
+        return re.sub("/+$", "", "".join(sb))
 
     @staticmethod
     def build_resource_part_of_uri(uuri: UUri) -> str:
 
-        if not uuri.HasField('resource'):
+        if not uuri.HasField("resource"):
             return ""
         u_resource = uuri.resource
 
         sb = "/" + u_resource.name
 
         if u_resource.instance:
             sb += "." + u_resource.instance
@@ -79,52 +81,42 @@
             sb += "#" + u_resource.message
 
         return sb
 
     @staticmethod
     def build_software_entity_part_of_uri(entity: UEntity) -> str:
         """
-        Create the service part of the uProtocol URI from an UEntity object.<br><br>
-        @param entity:Software Entity representing a service or an application.
-        @return: Returns the String representation of the UEntity in the uProtocol URI.
+        Create the service part of the uProtocol URI from an
+        UEntity object.<br><br>
+        @param entity:Software Entity representing a service
+        or an application.
+        @return: Returns the String representation of the UEntity
+        in the uProtocol URI.
         """
         sb = str(entity.name.strip())
         sb += "/"
 
         if entity.version_major > 0:
             sb += str(entity.version_major)
 
         return sb
 
-    @staticmethod
-    def build_authority_part_of_uri(authority: UAuthority) -> str:
-        """
-        Create the authority part of the uProtocol URI from an UAuthority object.<br><br>
-        @param authority:represents the deployment location of a specific  Software Entity in the Ultiverse.
-        @return:Returns the String representation of the  Authority in the uProtocol URI.
-        """
-
-        partial_uri = "//"
-        maybe_name = authority.name
-
-        if maybe_name is not None or maybe_name != "":
-            partial_uri += maybe_name
-
-        return partial_uri
-
     def deserialize(self, u_protocol_uri: str) -> UUri:
         """
         Deserialize a String into a UUri object.<br><br>
         @param u_protocol_uri:A long format uProtocol URI.
         @return:Returns an UUri data object.
         """
         if u_protocol_uri is None or u_protocol_uri.strip() == "":
             return UUri()
-        uri = u_protocol_uri[u_protocol_uri.index(":") + 1:] \
-            if ":" in u_protocol_uri else u_protocol_uri.replace('\\', '/')
+        uri = (
+            u_protocol_uri[u_protocol_uri.index(":") + 1:]
+            if ":" in u_protocol_uri
+            else u_protocol_uri.replace("\\", "/")
+        )
 
         is_local = not uri.startswith("//")
         uri_parts = LongUriSerializer.remove_empty(uri.split("/"))
         number_of_parts_in_uri = len(uri_parts)
 
         if number_of_parts_in_uri == 0 or number_of_parts_in_uri == 1:
             return UUri()
@@ -173,41 +165,52 @@
             new_uri.resource.CopyFrom(u_resource)
 
         return new_uri
 
     @staticmethod
     def parse_from_string(resource_string: str) -> UResource:
         """
-        Static builder method for creating a UResource using a string that contains name + instance + message.<br><br>
+        Static builder method for creating a UResource using a string
+        that contains name + instance + message.<br><br>
         @param resource_string:String that contains the UResource information.
         @return:Returns a UResource object.
         """
         if resource_string is None or resource_string.strip() == "":
             raise ValueError("Resource must have a command name.")
 
         parts = LongUriSerializer.remove_empty(resource_string.split("#"))
         name_and_instance = parts[0]
 
-        name_and_instance_parts = LongUriSerializer.remove_empty(name_and_instance.split("."))
+        name_and_instance_parts = LongUriSerializer.remove_empty(
+            name_and_instance.split(".")
+        )
         resource_name = name_and_instance_parts[0]
-        resource_instance = name_and_instance_parts[1] if len(name_and_instance_parts) > 1 else None
+        resource_instance = (
+            name_and_instance_parts[1]
+            if len(name_and_instance_parts) > 1
+            else None
+        )
         resource_message = parts[1] if len(parts) > 1 else None
 
         u_resource = UResource(name=resource_name)
         if resource_instance is not None:
             u_resource.instance = resource_instance
         if resource_message is not None:
             u_resource.message = resource_message
-        if "rpc" in resource_name and resource_instance is not None and "response" in resource_instance:
+        if (
+            "rpc" in resource_name
+            and resource_instance is not None
+            and "response" in resource_instance
+        ):
             u_resource.id = 0
 
         return u_resource
 
     @staticmethod
     def remove_empty(parts):
         result = parts[:]
 
         # Iterate through the list in reverse and remove empty strings
-        while result and result[-1] == '':
+        while result and result[-1] == "":
             result.pop()
 
         return result
```

### Comparing `up_python-0.1.1.dev0/uprotocol/uri/serializer/microuriserializer.py` & `up_python-0.1.2.dev0/uprotocol/uri/serializer/microuriserializer.py`

 * *Files 13% similar despite different names*

```diff
@@ -21,127 +21,135 @@
 # SPDX-FileType: SOURCE
 # SPDX-FileCopyrightText: 2023 General Motors GTO LLC
 # SPDX-License-Identifier: Apache-2.0
 
 # -------------------------------------------------------------------------
 
 
-import io
-import struct
 from enum import Enum
 
 from uprotocol.proto.uri_pb2 import UAuthority
 from uprotocol.proto.uri_pb2 import UEntity
 from uprotocol.proto.uri_pb2 import UUri
 from uprotocol.uri.factory.uresource_builder import UResourceBuilder
 from uprotocol.uri.serializer.uriserializer import UriSerializer
 from uprotocol.uri.validator.urivalidator import UriValidator
 
 
 class AddressType(Enum):
     """
     The type of address used for Micro URI.
     """
+
     LOCAL = 0
     IPv4 = 1
     IPv6 = 2
     ID = 3
 
-    def getValue(self):
-        return bytes(self.value)
+    # def getValue(self):
+    #     return bytes(self.value)
 
     @classmethod
     def from_value(cls, value):
         for addr_type in cls:
             if addr_type.value == value:
                 return addr_type
         return None  # Return None if no matching enum value is found
 
 
+def keep_8_least_significant_bits(n: int):
+    # by default, python is little endian
+    return n & 0xFF
+
+
 class MicroUriSerializer(UriSerializer):
     """
     UUri Serializer that serializes a UUri to a byte[] (micro format) per <a
     href="https://github.com/eclipse-uprotocol/uprotocol-spec/blob/main/basics/uri.adoc">
     https://github.com/eclipse-uprotocol/uprotocol-spec/blob/main/basics/uri.adoc</a>
     """
+
     LOCAL_MICRO_URI_LENGTH = 8
     IPV4_MICRO_URI_LENGTH = 12
     IPV6_MICRO_URI_LENGTH = 24
     UP_VERSION = 0x1
 
     def serialize(self, uri: UUri) -> bytes:
         """
-        Serialize a UUri into a byte[] following the Micro-URI specifications.<br><br>
+        Serialize a UUri into a byte[] following the Micro-URI specifications
+        for python, bits are unsigned integers [0, 255)
         @param uri:The UUri data object.
         @return:Returns a byte[] representing the serialized UUri.
         """
 
-        if uri is None or UriValidator.is_empty(uri) or not UriValidator.is_micro_form(uri):
+        if (
+            uri is None
+            or UriValidator.is_empty(uri)
+            or not UriValidator.is_micro_form(uri)
+        ):
             return bytearray()
 
-        maybe_ue_id = uri.entity.id
-        maybe_uresource_id = uri.resource.id
+        maybe_ue_id: int = uri.entity.id
+        maybe_uresource_id: int = uri.resource.id
+
+        byte_arr: bytearray = bytearray()
 
-        os = io.BytesIO()
-        os.write(bytes([self.UP_VERSION]))
+        byte_arr.append(self.UP_VERSION)
 
-        if uri.authority.HasField('ip'):
+        address_type: AddressType = AddressType.LOCAL
+        if uri.authority.HasField("ip"):
             length: int = len(uri.authority.ip)
             if length == 4:
                 address_type = AddressType.IPv4
             elif length == 16:
                 address_type = AddressType.IPv6
             else:
                 return bytearray()
-        elif uri.authority.HasField('id'):
+        elif uri.authority.HasField("id"):
             address_type = AddressType.ID
-        else:
-            address_type = AddressType.LOCAL
 
-        os.write(address_type.value.to_bytes(1, 'big'))
+        byte_arr.append(address_type.value)
 
         # URESOURCE_ID
-        os.write((maybe_uresource_id >> 8).to_bytes(1, 'big'))
-        os.write((maybe_uresource_id & 0xFF).to_bytes(1, 'big'))
+        byte_arr.append(keep_8_least_significant_bits(maybe_uresource_id >> 8))
+        byte_arr.append(keep_8_least_significant_bits(maybe_uresource_id))
 
         # UENTITY_ID
-        os.write((maybe_ue_id >> 8).to_bytes(1, 'big'))
-        os.write((maybe_ue_id & 0xFF).to_bytes(1, 'big'))
+        byte_arr.append(keep_8_least_significant_bits(maybe_ue_id >> 8))
+        byte_arr.append(keep_8_least_significant_bits(maybe_ue_id))
 
         # UE_VERSION
-        unsigned_value = uri.entity.version_major
-        if unsigned_value > 127:
-            signed_byte = unsigned_value - 256
-        else:
-            signed_byte = unsigned_value
-        os.write(struct.pack('b', signed_byte))
+        unsigned_value: int = uri.entity.version_major
+        byte_arr.append(keep_8_least_significant_bits(unsigned_value))
+
         # UNUSED
-        os.write(bytes([0]))
+        byte_arr.append(0x0)
 
         # Populating the UAuthority
         if address_type != AddressType.LOCAL:
             # Write the ID length if the type is ID
             if address_type == AddressType.ID:
-                os.write(len(uri.authority.id).to_bytes(1, 'big'))
-
+                byte_arr.append(
+                    keep_8_least_significant_bits(len(uri.authority.id))
+                )
             try:
                 if uri.authority.HasField("ip"):
-                    os.write(uri.authority.ip)
+                    byte_arr.extend(bytearray(uri.authority.ip))
                 elif uri.authority.HasField("id"):
-                    os.write(uri.authority.id)
-            except Exception as e:
-                print(e)  # Handle the exception as needed
-
-        return os.getvalue()
+                    byte_arr.extend(bytearray(uri.authority.id))
+            except Exception:
+                return bytearray()
+        return byte_arr
 
     def deserialize(self, micro_uri: bytes) -> UUri:
         """
         Deserialize a byte[] into a UUri object.<br><br>
         @param micro_uri:A byte[] uProtocol micro URI.
-        @return:Returns an UUri data object from the serialized format of a microUri.
+        @return:Returns an UUri data object from the serialized
+        format of a microUri.
         """
         if micro_uri is None or len(micro_uri) < self.LOCAL_MICRO_URI_LENGTH:
             return UUri()
 
         if micro_uri[0] != self.UP_VERSION:
             return UUri()
 
@@ -150,19 +158,28 @@
 
         # Validate Type is found
         if addresstype is None:
             return UUri()
 
         # Validate that the micro_uri is the correct length for the type
         address_type = addresstype
-        if address_type == AddressType.LOCAL and len(micro_uri) != self.LOCAL_MICRO_URI_LENGTH:
-            return UUri()
-        elif address_type == AddressType.IPv4 and len(micro_uri) != self.IPV4_MICRO_URI_LENGTH:
-            return UUri()
-        elif address_type == AddressType.IPv6 and len(micro_uri) != self.IPV6_MICRO_URI_LENGTH:
+        if (
+            address_type == AddressType.LOCAL
+            and len(micro_uri) != self.LOCAL_MICRO_URI_LENGTH
+        ):
+            return UUri()
+        elif (
+            address_type == AddressType.IPv4
+            and len(micro_uri) != self.IPV4_MICRO_URI_LENGTH
+        ):
+            return UUri()
+        elif (
+            address_type == AddressType.IPv6
+            and len(micro_uri) != self.IPV6_MICRO_URI_LENGTH
+        ):
             return UUri()
 
         # UENTITY_ID
         ue_id = ((micro_uri[4] & 0xFF) << 8) | (micro_uri[5] & 0xFF)
 
         # UE_VERSION
         ui_version = micro_uri[6]
@@ -172,13 +189,16 @@
             length = 4 if address_type == AddressType.IPv4 else 16
             data = micro_uri[8:8 + length]
             u_authority = UAuthority(ip=bytes(data))
         elif address_type == AddressType.ID:
             length = micro_uri[8]
             u_authority = UAuthority(id=bytes(micro_uri[9:9 + length]))
 
-        uri = UUri(entity=UEntity(id=ue_id, version_major=ui_version), resource=UResourceBuilder.from_id(u_resource_id))
+        uri = UUri(
+            entity=UEntity(id=ue_id, version_major=ui_version),
+            resource=UResourceBuilder.from_id(u_resource_id),
+        )
 
         if u_authority is not None:
             uri.authority.CopyFrom(u_authority)
 
         return uri
```

### Comparing `up_python-0.1.1.dev0/uprotocol/uri/serializer/uriserializer.py` & `up_python-0.1.2.dev0/uprotocol/uuid/serializer/longuuidserializer.py`

 * *Files 25% similar despite different names*

```diff
@@ -21,69 +21,55 @@
 # SPDX-FileType: SOURCE
 # SPDX-FileCopyrightText: 2023 General Motors GTO LLC
 # SPDX-License-Identifier: Apache-2.0
 
 # -------------------------------------------------------------------------
 
 
-from abc import ABC, abstractmethod
-from re import T
-from typing import Optional
-from uprotocol.proto.uri_pb2 import UUri,UAuthority,UEntity,UResource
-from uprotocol.uri.validator.urivalidator import UriValidator
+from uprotocol.proto.uuid_pb2 import UUID
+from uprotocol.uuid.factory import PythonUUID
+from uprotocol.uuid.factory.uuidutils import UUIDUtils
+from uprotocol.uuid.serializer.uuidserializer import UuidSerializer
 
 
-class UriSerializer(ABC):
+class LongUuidSerializer(UuidSerializer):
     """
-    UUris are used in transport layers and hence need to be serialized.<br>Each transport supports different
-    serialization formats.<br>For more information, please refer to <a
-    href="https://github.com/eclipse-uprotocol/uprotocol-spec/blob/main/basics/uri.adoc">
-    https://github.com/eclipse-uprotocol/uprotocol-spec/blob/main/basics/uri.adoc</a>
+    UUID Serializer implementation used to serialize/deserialize UUIDs to/from
+    a string
     """
 
-    @abstractmethod
-    def deserialize(self, uri: T) -> UUri:
-        """
-        Deserialize from the format to a UUri.<br><br>
-        @param uri:serialized UUri.
-        @return:Returns a UUri object from the serialized format from the wire.
-        """
-        pass
-
-    @abstractmethod
-    def serialize(self, uri: UUri) -> T:
-        """
-        Serialize from a UUri to a specific serialization format.<br><br>
-        @param uri:UUri object to be serialized to the format T.
-        @return:Returns the UUri in the transport serialized format.
-        """
-        pass
-
-    def build_resolved(self, long_uri: str, micro_uri: bytes) -> UUri:
-        """
-        Build a fully resolved UUri from the serialized long format and the serializes micro format.<br><br>
-        @param long_uri:UUri serialized as a Sting.
-        @param micro_uri:UUri serialized as a byte[].
-        @return:Returns a UUri object serialized from one of the forms.
-        """
-        if (not long_uri or long_uri.isspace()) and (not micro_uri or len(micro_uri) == 0):
-            return UUri()
-        from uprotocol.uri.serializer.longuriserializer import LongUriSerializer
-        from uprotocol.uri.serializer.microuriserializer import MicroUriSerializer
-        long_u_uri = LongUriSerializer().deserialize(long_uri)
-        micro_u_uri = MicroUriSerializer().deserialize(micro_uri)
-        u_authority = UAuthority()
-        u_authority.CopyFrom(micro_u_uri.authority)
-
-        u_authority.name = long_u_uri.authority.name
-
-        u_entity = UEntity()
-        u_entity.CopyFrom(micro_u_uri.entity)
-
-        u_entity.name = long_u_uri.entity.name
-
-        u_resource = UResource()
-        u_resource.CopyFrom(long_u_uri.resource)
-        u_resource.id = micro_u_uri.resource.id
-
-        u_uri = UUri(authority=u_authority, entity=u_entity, resource=u_resource)
-        return u_uri if UriValidator.is_resolved(u_uri) else None
+    @staticmethod
+    def instance():
+        return LongUuidSerializer()
+
+    def deserialize(self, string_uuid: str) -> UUID:
+        """
+        Deserialize from the string format to a UUID.
+        :param string_uuid: Serialized UUID in string format.
+        :return: Returns a UUID object from the serialized format from the
+        wire.
+        """
+        if not string_uuid or string_uuid.isspace():
+            return (
+                UUID()
+            )  # Return default UUID if string is empty or whitespace
+        try:
+            msb, lsb = UUIDUtils.get_msb_lsb(PythonUUID(string_uuid))
+            return UUID(msb=msb, lsb=lsb)
+        except ValueError:
+            return (
+                UUID()
+            )  # Return default UUID in case of parsing failure
+
+    def serialize(self, uuid: UUID) -> str:
+        """
+        Serialize from a UUID to a string format.
+        :param uuid: UUID object to be serialized to a string.
+        :return: Returns the UUID in the string serialized format.
+        """
+        if uuid is None:
+            return ""
+
+        pythonuuid = UUIDUtils.create_pythonuuid_from_eclipseuuid(
+            uuid
+        )
+        return str(pythonuuid) if uuid else ""
```

### Comparing `up_python-0.1.1.dev0/uprotocol/uri/validator/urivalidator.py` & `up_python-0.1.2.dev0/uprotocol/uri/validator/urivalidator.py`

 * *Files 18% similar despite different names*

```diff
@@ -20,174 +20,250 @@
 # under the License.
 # SPDX-FileType: SOURCE
 # SPDX-FileCopyrightText: 2023 General Motors GTO LLC
 # SPDX-License-Identifier: Apache-2.0
 
 # -------------------------------------------------------------------------
 
+from multimethod import multimethod
 
 from uprotocol.proto.uri_pb2 import UAuthority
-from uprotocol.proto.uri_pb2 import UEntity
 from uprotocol.proto.uri_pb2 import UResource
 from uprotocol.proto.uri_pb2 import UUri
+from uprotocol.uri.factory.uresource_builder import UResourceBuilder
 from uprotocol.validation.validationresult import ValidationResult
-from multipledispatch import dispatch
+
 
 class UriValidator:
     """
     Class for validating Uris.
     """
 
     @staticmethod
     def validate(uri: UUri) -> ValidationResult:
         """
-        Validate a UUri to ensure that it has at least a name for the uEntity.<br><br>
+        Validate a UUri to ensure that it has at least a name
+        for the uEntity.<br><br>
         @param uri:UUri to validate.
-        @return:Returns UStatus containing a success or a failure with the error message.
+        @return:Returns UStatus containing a success or a failure
+        with the error message.
         """
         if UriValidator.is_empty(uri):
             return ValidationResult.failure("Uri is empty.")
 
-        if uri.HasField('authority') and not UriValidator.is_remote(uri.authority):
-            return ValidationResult.failure("Uri is remote missing uAuthority.")
+        if uri.HasField("authority") and not UriValidator.is_remote(
+            uri.authority
+        ):
+            return ValidationResult.failure(
+                "Uri is remote missing uAuthority."
+            )
 
         if uri.entity.name.strip() == "":
-            return ValidationResult.failure("Uri is missing uSoftware Entity name.")
+            return ValidationResult.failure(
+                "Uri is missing uSoftware Entity name."
+            )
 
         return ValidationResult.success()
 
     @staticmethod
     def validate_rpc_method(uri: UUri) -> ValidationResult:
         """
-        Validate a UUri that is meant to be used as an RPC method URI. Used in Request sink values and Response
+        Validate a UUri that is meant to be used as an RPC method URI.
+        Used in Request sink values and Response
         source values.<br><br>
         @param uri:UUri to validate.
-        @return:Returns UStatus containing a success or a failure with the error message.
+        @return:Returns UStatus containing a success or a failure
+        with the error message.
         """
         status = UriValidator.validate(uri)
         if status.is_failure():
             return status
 
         if not UriValidator.is_rpc_method(uri):
             return ValidationResult.failure(
-                "Invalid RPC method uri. Uri should be the method to be called, or method from response.")
+                "Invalid RPC method uri. Uri should be the method to be called, or method from response."
+            )
 
         return ValidationResult.success()
 
     @staticmethod
     def validate_rpc_response(uri: UUri) -> ValidationResult:
         """
-        Validate a UUri that is meant to be used as an RPC response URI. Used in Request source values and
+        Validate a UUri that is meant to be used as an RPC response URI.
+        Used in Request source values and
         Response sink values.<br><br>
         @param uri:UUri to validate.
-        @return:Returns UStatus containing a success or a failure with the error message.
+        @return:Returns UStatus containing a success or a failure with
+        the error message.
         """
         status = UriValidator.validate(uri)
         if status.is_failure():
             return status
 
         if not UriValidator.is_rpc_response(uri):
             return ValidationResult.failure("Invalid RPC response type.")
 
         return ValidationResult.success()
 
     @staticmethod
     def is_empty(uri: UUri) -> bool:
-        '''
-        Indicates that this  URI is an empty as it does not contain authority, entity, and resource.
+        """
+        Indicates that this  URI is an empty as it does not contain
+        authority, entity, and resource.
         @param uri UUri to check if it is empty
-        @return Returns true if this  URI is an empty container and has no valuable information in building uProtocol sinks or sources.
-        '''
-        return uri is not None and not uri.HasField('authority') and not uri.HasField('entity') and not uri.HasField('resource')
-
+        @return Returns true if this  URI is an empty container and has
+        no valuable information in building uProtocol sinks or sources.
+        """
+        return uri is None or uri == UUri()
 
-    @staticmethod
+    @multimethod
     def is_rpc_method(uri: UUri) -> bool:
         """
-        Returns true if this resource specifies an RPC method call or RPC response.<br><br>
-        @param uri:
-        @return:Returns true if this resource specifies an RPC method call or RPC response.
-        """
-        return not UriValidator.is_empty(uri) and uri.resource.name == "rpc" and (
-                uri.resource.HasField('instance') and uri.resource.instance.strip() != "" or (
-                uri.resource.HasField('id') and uri.resource.id != 0))
+        Returns true if URI is of type RPC. A UUri is of type RPC if it
+        contains the word rpc in the resource name
+        and has an instance name and/or the id is less than MIN_TOPIC_ID.
+        @param uri: UUri to check if it is of type RPC
+        @return: Returns true if this resource specifies an RPC method
+        call or RPC response.
+        """
+        return uri is not None and UriValidator.is_rpc_method(uri.resource)
+
+    @multimethod
+    def is_rpc_method(uri: None) -> bool:
+        """
+        Returns false if input is None.
+        @param uri: None
+        @return Returns false.
+        """
+        return False
+
+    @multimethod
+    def is_rpc_method(resource: UResource) -> bool:
+        """
+        Returns true if Uresource is of type RPC.
+        @param resource: UResource to check if it is of type RPC method
+        @return Returns true if URI is of type RPC.
+        """
+        return (
+            resource is not None
+            and resource.name == "rpc"
+            and (
+                resource.HasField("instance")
+                and resource.instance.strip() != ""
+                or (
+                    resource.HasField("id")
+                    and resource.id < UResourceBuilder.MIN_TOPIC_ID
+                )
+            )
+        )
 
     @staticmethod
     def is_resolved(uri: UUri) -> bool:
 
-        return uri is not None and not UriValidator.is_empty(uri) and \
-            UriValidator.is_long_form(uri) and UriValidator.is_micro_form(uri)
+        return UriValidator.is_long_form(uri) and UriValidator.is_micro_form(
+            uri
+        )
 
     @staticmethod
     def is_rpc_response(uri: UUri) -> bool:
-        if uri is None:
-            return False
-        
-        resource = uri.resource
+        return (
+            uri is not None
+            and uri.resource == UResourceBuilder.for_rpc_response()
+        )
 
-        return "rpc" in resource.name and uri.HasField("resource") and "response" in resource.instance and resource.HasField("id") and resource.id == 0
-
-    @staticmethod
-    @dispatch(UUri)
+    @multimethod
     def is_micro_form(uri: UUri) -> bool:
         """
-        Determines if this UUri can be serialized into a micro form UUri.<br><br>
+        Determines if this UUri can be serialized into
+        a micro form UUri.<br><br>
         @param uuri: An UUri proto message object
-        @return:Returns true if this UUri can be serialized into a micro form UUri.
+        @return:Returns true if this UUri can be serialized into
+        a micro form UUri.
         """
 
-        return uri is not None and not UriValidator.is_empty(uri) and uri.entity.HasField('id') \
-            and uri.resource.HasField('id') and UriValidator.is_micro_form(uri.authority)
-            
-    @staticmethod
-    @dispatch(UAuthority)
+        return (
+            uri is not None
+            and not UriValidator.is_empty(uri)
+            and uri.entity.HasField("id")
+            and uri.resource.HasField("id")
+            and UriValidator.is_micro_form(uri.authority)
+        )
+
+    @multimethod
     def is_micro_form(authority: UAuthority) -> bool:
-        '''
-        check if UAuthority can be represented in micro format. Micro UAuthorities are local or ones 
+        """
+        check if UAuthority can be represented in micro format.
+        Micro UAuthorities are local or ones
         that contain IP address or IDs.
         @param authority UAuthority to check
         @return Returns true if UAuthority can be represented in micro format
-        '''
-
+        """
 
-        return UriValidator.is_local(authority) or (authority.HasField('ip') or (authority.HasField('id')))
+        return UriValidator.is_local(authority) or (
+            authority.HasField("ip") or (authority.HasField("id"))
+        )
 
-    @staticmethod
-    @dispatch(UUri)
+    @multimethod
     def is_long_form(uri: UUri) -> bool:
         """
-        Determines if this UUri can be serialized into a long form UUri.<br><br>
+        Determines if this UUri can be serialized into
+        a long form UUri.<br><br>
         @param uuri: An UUri proto message object
-        @return:Returns true if this UUri can be serialized into a long form UUri.
+        @return:Returns true if this UUri can be serialized into
+        a long form UUri.
         """
 
-        return uri is not None and not UriValidator.is_empty(uri) and UriValidator.is_long_form(uri.authority) and \
-            uri.entity.name.strip() != "" and uri.resource.name.strip() != ""
-            
-    @staticmethod
-    @dispatch(UAuthority)
+        return (
+            uri is not None
+            and not UriValidator.is_empty(uri)
+            and UriValidator.is_long_form(uri.authority)
+            and uri.entity.name.strip() != ""
+            and uri.resource.name.strip() != ""
+        )
+
+    @multimethod
     def is_long_form(authority: UAuthority) -> bool:
-        '''
-        Returns true if UAuthority contains names so that it can be serialized into long format.
+        """
+        Returns true if UAuthority is local contains names so
+        that it can be serialized into long format.
         @param authority UAuthority to check
-        @return Returns true if URI contains names so that it can be serialized into long format.
-        '''
-        return authority is not None and authority.HasField('name') and authority.name.strip() != ""
-    
+        @return Returns true if URI contains names so that
+        it can be serialized into long format.
+        """
+        return authority is not None and (
+            UriValidator.is_local(authority)
+            or (authority.HasField("name") and authority.name.strip() != "")
+        )
+
     @staticmethod
     def is_local(authority: UAuthority) -> bool:
-        '''
-        Returns true if UAuthority is local meaning there is no name/ip/id set.
+        """
+        Returns true if UAuthority is local meaning there
+        is no name/ip/id set.
         @param authority UAuthority to check if it is local or not
-        @return Returns true if UAuthority is local meaning the Authority is not populated with name, ip and id
-        '''
-        return (authority is None) or (authority == UAuthority())
+        @return Returns true if UAuthority is local meaning the
+        Authority is not populated with name, ip and id
+        """
+        return (authority is not None) and (authority == UAuthority())
 
     @staticmethod
     def is_remote(authority: UAuthority) -> bool:
-        '''
-        Returns true if UAuthority is remote meaning the name and/or ip/id is populated.
+        """
+        Returns true if UAuthority is remote meaning
+        the name and/or ip/id is populated.
         @param authority UAuthority to check if it is remote or not
-        @return Returns true if UAuthority is remote meaning the name and/or ip/id is populated.
-        '''
-        return (authority is not None) and (not authority == UAuthority()) and \
-            (UriValidator.is_long_form(authority) or UriValidator.is_micro_form(authority))
+        @return Returns true if UAuthority is remote meaning
+        the name and/or ip/id is populated.
+        """
+        return (authority is not None) and (not authority == UAuthority())
+
+    @staticmethod
+    def is_short_form(uri: UUri) -> bool:
+        """
+        Return True of the UUri is Short form. A UUri that
+        is micro form (contains numbers) can
+        also be a Short form Uri.
+        @param uri {@link UUri} to check
+        @return Returns true if contains ids can can
+        be serialized to short format.
+        """
+        return UriValidator.is_micro_form(uri)
```

### Comparing `up_python-0.1.1.dev0/uprotocol/uuid/README.adoc` & `up_python-0.1.2.dev0/uprotocol/uuid/README.adoc`

 * *Files identical despite different names*

### Comparing `up_python-0.1.1.dev0/uprotocol/uuid/factory/__init__.py` & `up_python-0.1.2.dev0/uprotocol/uuid/factory/__init__.py`

 * *Files identical despite different names*

### Comparing `up_python-0.1.1.dev0/uprotocol/uuid/factory/uuidfactory.py` & `up_python-0.1.2.dev0/uprotocol/uuid/factory/uuidfactory.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,9 @@
 # -------------------------------------------------------------------------
-import hashlib
-import random
-import struct
-from datetime import datetime
-# Copyright (c) 2023 General Motors GTO LLC
+# Copyright (c) 2024 General Motors GTO LLC
 #
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
 # "License"); you may not use this file except in compliance
@@ -18,24 +14,25 @@
 # Unless required by applicable law or agreed to in writing,
 # software distributed under the License is distributed on an
 # "AS IS" BASIS, WITHOUT WARRANTIES OR CONDITIONS OF ANY
 # KIND, either express or implied.  See the License for the
 # specific language governing permissions and limitations
 # under the License.
 # SPDX-FileType: SOURCE
-# SPDX-FileCopyrightText: 2023 General Motors GTO LLC
+# SPDX-FileCopyrightText: 2024 General Motors GTO LLC
 # SPDX-License-Identifier: Apache-2.0
 
 # -------------------------------------------------------------------------
 
 
-from enum import Enum
+import random
+from datetime import datetime
 
 from uprotocol.proto.uuid_pb2 import UUID
-from uprotocol.uuid.factory import *
+from uprotocol.uuid.factory import uuid6
 from uprotocol.uuid.factory.uuidutils import UUIDUtils
 
 
 class UUIDFactory:
     def create(self, instant=None):
         if instant is None:
             instant = datetime.now()
@@ -51,27 +48,32 @@
 
         python_uuid = uuid6()
         msb, lsb = UUIDUtils.get_msb_lsb(python_uuid)
         return UUID(msb=msb, lsb=lsb)
 
 
 class UUIDv8Factory(UUIDFactory):
-    MAX_COUNT = 0xfff
-    _lsb = (random.getrandbits(63) & 0x3fffffffffffffff) | 0x8000000000000000
+    MAX_COUNT = 0xFFF
+    _lsb = (random.getrandbits(63) & 0x3FFFFFFFFFFFFFFF) | 0x8000000000000000
     UUIDV8_VERSION = 8
     _msb = UUIDV8_VERSION << 12
+
     def _create(self, instant) -> UUID:
-        time = int(instant.timestamp() * 1000) if instant else int(datetime.now().timestamp() * 1000)
+        time = (
+            int(instant.timestamp() * 1000)
+            if instant
+            else int(datetime.now().timestamp() * 1000)
+        )
 
         if time == (self._msb >> 16):
             if (self._msb & 0xFFF) < self.MAX_COUNT:
                 self._msb += 1
         else:
             self._msb = (time << 16) | (8 << 12)
 
         return UUID(msb=self._msb, lsb=self._lsb)
         # return UUID(msb=msb, lsb=lsb)
 
 
-class Factories():
+class Factories:
     UUIDV6 = UUIDv6Factory()
     UPROTOCOL = UUIDv8Factory()
```

### Comparing `up_python-0.1.1.dev0/uprotocol/uuid/serializer/longuuidserializer.py` & `up_python-0.1.2.dev0/uprotocol/uuid/serializer/uuidserializer.py`

 * *Files 16% similar despite different names*

```diff
@@ -21,47 +21,39 @@
 # SPDX-FileType: SOURCE
 # SPDX-FileCopyrightText: 2023 General Motors GTO LLC
 # SPDX-License-Identifier: Apache-2.0
 
 # -------------------------------------------------------------------------
 
 
+from abc import ABC, abstractmethod
+from typing import TypeVar, Generic
+
 from uprotocol.proto.uuid_pb2 import UUID
-from uprotocol.uuid.factory import PythonUUID
-from uprotocol.uuid.factory.uuidutils import UUIDUtils
-from uprotocol.uuid.serializer.uuidserializer import UuidSerializer
+
+T = TypeVar("T")
 
 
-class LongUuidSerializer(UuidSerializer):
+class UuidSerializer(ABC, Generic[T]):
     """
-    UUID Serializer implementation used to serialize/deserialize UUIDs to/from a string
+    UUID Serializer interface used to serialize/deserialize UUIDs
+    to/from either Long (string) or micro (bytes) form
     """
 
-    @staticmethod
-    def instance():
-        return LongUuidSerializer()
-
-    def deserialize(self, string_uuid: str) -> UUID:
+    @abstractmethod
+    def deserialize(self, uuid: T) -> UUID:
         """
-        Deserialize from the string format to a UUID.
-        :param string_uuid: Serialized UUID in string format.
-        :return: Returns a UUID object from the serialized format from the wire.
+        Deserialize from the format to a UUID.
+        :param uuid: Serialized UUID.
+        :return: Returns a UUID object from the
+        serialized format from the wire.
         """
-        if not string_uuid or string_uuid.isspace():
-            return UUID()  # Return default UUID if string is empty or whitespace
-        try:
-            msb, lsb = UUIDUtils.get_msb_lsb(PythonUUID(string_uuid))
-            return UUID(msb=msb, lsb=lsb)
-        except ValueError:
-            return UUID()  # Return default UUID in case of parsing failure
+        pass  # Implement your deserialization logic here
 
-    def serialize(self, uuid: UUID) -> str:
+    @abstractmethod
+    def serialize(self, uuid: UUID) -> T:
         """
-        Serialize from a UUID to a string format.
-        :param uuid: UUID object to be serialized to a string.
-        :return: Returns the UUID in the string serialized format.
+        Serialize from a UUID to a specific serialization format.
+        :param uuid: UUID object to be serialized to the format T.
+        :return: Returns the UUID in the transport serialized format.
         """
-        if uuid is None:
-            return ''
-
-        pythonuuid = UUIDUtils.create_pythonuuid_from_eclipseuuid(uuid)
-        return str(pythonuuid) if uuid else ''
+        pass  # Implement your serialization logic here
```

### Comparing `up_python-0.1.1.dev0/uprotocol/uuid/serializer/microuuidserializer.py` & `up_python-0.1.2.dev0/uprotocol/uuid/serializer/microuuidserializer.py`

 * *Files 4% similar despite different names*

```diff
@@ -30,37 +30,43 @@
 from uprotocol.proto.uuid_pb2 import UUID
 from uprotocol.uuid.factory.uuidutils import UUIDUtils
 from uprotocol.uuid.serializer.uuidserializer import UuidSerializer
 
 
 class MicroUuidSerializer(UuidSerializer):
     """
-    UUID Serializer implementation used to serialize/deserialize UUIDs to/from bytes
+    UUID Serializer implementation used to serialize/deserialize UUIDs to/from
+    bytes
     """
 
     @staticmethod
     def instance():
         return MicroUuidSerializer()
 
     def deserialize(self, uuid_bytes: bytes) -> UUID:
         """
         Deserialize from the bytes format to a UUID.
         :param uuid_bytes: Serialized UUID in bytes format.
-        :return: Returns a UUID object from the serialized format from the wire.
+        :return: Returns a UUID object from the serialized format from the
+        wire.
         """
         if not uuid_bytes or len(uuid_bytes) != 16:
-            return UUID()  # Return default UUID if bytes are empty or not 16 bytes
+            return (
+                UUID()
+            )  # Return default UUID if bytes are empty or not 16 bytes
 
-        msb, lsb = struct.unpack('>QQ', uuid_bytes)
+        msb, lsb = struct.unpack(">QQ", uuid_bytes)
         return UUID(msb=msb, lsb=lsb)
 
     def serialize(self, uuid: UUID) -> bytes:
         """
         Serialize from a UUID to bytes format.
         :param uuid: UUID object to be serialized to bytes.
         :return: Returns the UUID in the bytes serialized format.
         """
         if uuid is None:
             return bytearray()
-        pythonuuid = UUIDUtils.create_pythonuuid_from_eclipseuuid(uuid)
-        msb, lsb = divmod(pythonuuid.int, 2 ** 64)
-        return struct.pack('>QQ', msb, lsb)
+        pythonuuid = UUIDUtils.create_pythonuuid_from_eclipseuuid(
+            uuid
+        )
+        msb, lsb = divmod(pythonuuid.int, 2**64)
+        return struct.pack(">QQ", msb, lsb)
```

### Comparing `up_python-0.1.1.dev0/uprotocol/uuid/validate/uuidvalidator.py` & `up_python-0.1.2.dev0/uprotocol/uuid/validate/uuidvalidator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 # -------------------------------------------------------------------------
 from abc import ABC, abstractmethod
+
 # Copyright (c) 2023 General Motors GTO LLC
 #
 # Licensed to the Apache Software Foundation (ASF) under one
 # or more contributor license agreements.  See the NOTICE file
 # distributed with this work for additional information
 # regarding copyright ownership.  The ASF licenses this file
 # to you under the Apache License, Version 2.0 (the
@@ -21,15 +22,14 @@
 # SPDX-FileType: SOURCE
 # SPDX-FileCopyrightText: 2023 General Motors GTO LLC
 # SPDX-License-Identifier: Apache-2.0
 
 # -------------------------------------------------------------------------
 
 
-from collections import namedtuple
 from enum import Enum
 
 from uprotocol.proto.uuid_pb2 import UUID
 from uprotocol.uuid.factory.uuidutils import UUIDUtils, Version
 from uprotocol.validation.validationresult import ValidationResult
 from uprotocol.proto.ustatus_pb2 import UStatus, UCode
 
@@ -41,36 +41,48 @@
 class UuidValidator(ABC):
     """
     UUID Validator class that validates UUIDs
     """
 
     @staticmethod
     def get_validator(uuid: UUID):
-        if UUIDUtils.isUuidv6(uuid):
+        if UUIDUtils.is_uuidv6(uuid):
             return Validators.UUIDV6.validator()
-        elif UUIDUtils.isUProtocol(uuid):
+        elif UUIDUtils.is_uprotocol(uuid):
             return Validators.UPROTOCOL.validator()
         else:
             return Validators.UNKNOWN.validator()
 
     def validate(self, uuid: UUID) -> UStatus:
-        error_messages = [self.validate_version(uuid), self.validate_variant(uuid), self.validate_time(uuid)]
-        error_messages = [result.get_message() for result in error_messages if result.is_failure()]
+        error_messages = [
+            self.validate_version(uuid),
+            self.validate_variant(uuid),
+            self.validate_time(uuid),
+        ]
+        error_messages = [
+            result.get_message()
+            for result in error_messages
+            if result.is_failure()
+        ]
         error_message = ",".join(error_messages)
         if not error_message:
             return ValidationResult.success().to_status()
         return UStatus(code=UCode.INVALID_ARGUMENT, message=error_message)
 
     @abstractmethod
     def validate_version(self, uuid: UUID) -> ValidationResult:
         raise NotImplementedError
 
     def validate_time(self, uuid: UUID) -> ValidationResult:
-        time = UUIDUtils.getTime(uuid)
-        return ValidationResult.success() if (time is not None and time > 0 )else ValidationResult.failure("Invalid UUID Time")
+        time = UUIDUtils.get_time(uuid)
+        return (
+            ValidationResult.success()
+            if (time is not None and time > 0)
+            else ValidationResult.failure("Invalid UUID Time")
+        )
 
     @abstractmethod
     def validate_variant(self, uuid: UUID) -> ValidationResult:
         raise NotImplementedError
 
 
 class InvalidValidator(UuidValidator):
@@ -79,31 +91,38 @@
 
     def validate_variant(self, uuid: UUID) -> ValidationResult:
         return ValidationResult.failure("Invalid UUID Variant")
 
 
 class UUIDv6Validator(UuidValidator):
     def validate_version(self, uuid: UUID) -> ValidationResult:
-        version = UUIDUtils.getVersion(uuid)
-        return ValidationResult.success() if version and version == Version.VERSION_TIME_ORDERED else (
-            ValidationResult.failure(
-                "Not a UUIDv6 Version"))
+        version = UUIDUtils.get_version(uuid)
+        return (
+            ValidationResult.success()
+            if version and version == Version.VERSION_TIME_ORDERED
+            else (ValidationResult.failure("Not a UUIDv6 Version"))
+        )
 
     def validate_variant(self, uuid: UUID) -> ValidationResult:
-        variant = UUIDUtils.getVariant(uuid)
-        return ValidationResult.success() if variant and "RFC 4122" in variant else ValidationResult.failure(
-            "Invalid UUIDv6 variant")
+        variant = UUIDUtils.get_variant(uuid)
+        return (
+            ValidationResult.success()
+            if variant and "RFC 4122" in variant
+            else ValidationResult.failure("Invalid UUIDv6 variant")
+        )
 
 
 class UUIDv8Validator(UuidValidator):
     def validate_version(self, uuid: UUID) -> ValidationResult:
-        version = UUIDUtils.getVersion(uuid)
-        return ValidationResult.success() if version and version == Version.VERSION_UPROTOCOL else (
-            ValidationResult.failure(
-                "Invalid UUIDv8 Version"))
+        version = UUIDUtils.get_version(uuid)
+        return (
+            ValidationResult.success()
+            if version and version == Version.VERSION_UPROTOCOL
+            else (ValidationResult.failure("Invalid UUIDv8 Version"))
+        )
 
     def validate_variant(self, uuid: UUID) -> ValidationResult:
         return ValidationResult.success()
 
 
 class Validators(Enum):
     UNKNOWN = InvalidValidator()  # Use a default validator instance
```

### Comparing `up_python-0.1.1.dev0/uprotocol/validation/validationresult.py` & `up_python-0.1.2.dev0/uprotocol/validation/validationresult.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,18 +26,18 @@
 
 
 from abc import ABC, abstractmethod
 
 from uprotocol.proto.ustatus_pb2 import UCode, UStatus
 
 
-
 class ValidationResult(ABC):
     """
-    Class wrapping a ValidationResult of success or failure wrapping the value of a UStatus.
+    Class wrapping a ValidationResult of success or failure wrapping the value
+    of a UStatus.
     """
     STATUS_SUCCESS = UStatus(code=UCode.OK, message="OK")
 
     def __init__(self):
         pass
 
     @abstractmethod
```

### Comparing `up_python-0.1.1.dev0/PKG-INFO` & `up_python-0.1.2.dev0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: up-python
-Version: 0.1.1.dev0
+Version: 0.1.2.dev0
 Summary: Language specific uProtocol library for building and using UUri, UUID, UAttributes, UTransport, and more.
 Home-page: https://github.com/eclipse-uprotocol/up-python
 License: The Apache License, Version 2.0
 Author: Neelam Kushwah
 Author-email: neelam.kushwah@gm.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
@@ -13,15 +13,16 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: cloudevents
 Requires-Dist: gitpython (>=3.1.41)
 Requires-Dist: googleapis-common-protos (>=1.56.4)
-Requires-Dist: multipledispatch
+Requires-Dist: multimethod
+Requires-Dist: protobuf (==4.24.2)
 Project-URL: Repository, https://github.com/eclipse-uprotocol/up-python
 Description-Content-Type: text/plain
 
 = Eclipse uProtocol Python Library
 :toc:
 
 == Overview
@@ -132,8 +133,7 @@
 
 === Running the Tests
 
 Requires coverage to be installed first, that can be done by running `pip install coverage`
 
 then you run:
 `python -m coverage run --source tests/ -m unittest discover`
-
```

