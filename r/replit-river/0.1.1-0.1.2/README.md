# Comparing `tmp/replit_river-0.1.1.tar.gz` & `tmp/replit_river-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "replit_river-0.1.1.tar", max compression
+gzip compressed data, was "replit_river-0.1.2.tar", max compression
```

## Comparing `replit_river-0.1.1.tar` & `replit_river-0.1.2.tar`

### file list

```diff
@@ -1,16 +1,18 @@
--rw-r--r--   0        0        0     1064 2024-03-26 21:03:19.806548 replit_river-0.1.1/LICENSE
--rw-r--r--   0        0        0     1628 2024-03-26 20:33:50.343232 replit_river-0.1.1/README.md
--rw-r--r--   0        0        0     1732 2024-03-26 21:32:35.827238 replit_river-0.1.1/pyproject.toml
--rw-r--r--   0        0        0      432 2024-03-26 20:33:50.345071 replit_river-0.1.1/replit_river/__init__.py
--rw-r--r--   0        0        0    16455 2024-03-26 21:09:45.631342 replit_river-0.1.1/replit_river/client.py
--rw-r--r--   0        0        0        0 2024-03-26 20:33:50.348071 replit_river-0.1.1/replit_river/codegen/__init__.py
--rwxr-xr-x   0        0        0      153 2024-03-26 20:33:50.348249 replit_river-0.1.1/replit_river/codegen/__main__.py
--rw-r--r--   0        0        0    13340 2024-03-26 20:34:45.102365 replit_river-0.1.1/replit_river/codegen/client.py
--rw-r--r--   0        0        0     1903 2024-03-26 20:33:50.350608 replit_river-0.1.1/replit_river/codegen/run.py
--rw-r--r--   0        0        0     5354 2024-03-26 20:33:50.350781 replit_river-0.1.1/replit_river/codegen/schema.py
--rw-r--r--   0        0        0    12604 2024-03-26 20:33:50.350933 replit_river-0.1.1/replit_river/codegen/server.py
--rw-r--r--   0        0        0      434 2024-03-26 20:33:50.351114 replit_river-0.1.1/replit_river/error_schema.py
--rw-r--r--   0        0        0        0 2024-03-26 20:33:50.351248 replit_river-0.1.1/replit_river/py.typed
--rw-r--r--   0        0        0    11535 2024-03-26 21:09:45.629077 replit_river-0.1.1/replit_river/rpc.py
--rw-r--r--   0        0        0     9843 2024-03-26 20:33:50.351597 replit_river-0.1.1/replit_river/server.py
--rw-r--r--   0        0        0     2450 1970-01-01 00:00:00.000000 replit_river-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1064 2024-04-02 22:20:09.999604 replit_river-0.1.2/LICENSE
+-rw-r--r--   0        0        0     1628 2024-03-26 20:33:50.343232 replit_river-0.1.2/README.md
+-rw-r--r--   0        0        0     1732 2024-04-11 21:07:11.137264 replit_river-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0      487 2024-04-11 21:05:27.020432 replit_river-0.1.2/replit_river/__init__.py
+-rw-r--r--   0        0        0    18569 2024-04-11 21:02:04.035350 replit_river-0.1.2/replit_river/client.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:24:00.533020 replit_river-0.1.2/replit_river/codegen/__init__.py
+-rwxr-xr-x   0        0        0      153 2024-04-11 18:24:00.533220 replit_river-0.1.2/replit_river/codegen/__main__.py
+-rw-r--r--   0        0        0    13340 2024-04-11 18:24:00.535474 replit_river-0.1.2/replit_river/codegen/client.py
+-rw-r--r--   0        0        0     1903 2024-04-11 18:24:00.535693 replit_river-0.1.2/replit_river/codegen/run.py
+-rw-r--r--   0        0        0     5354 2024-04-11 18:24:00.535865 replit_river-0.1.2/replit_river/codegen/schema.py
+-rw-r--r--   0        0        0    12604 2024-04-11 18:24:00.536045 replit_river-0.1.2/replit_river/codegen/server.py
+-rw-r--r--   0        0        0      478 2024-04-11 18:33:34.741591 replit_river-0.1.2/replit_river/error_schema.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:24:00.536395 replit_river-0.1.2/replit_river/py.typed
+-rw-r--r--   0        0        0    11973 2024-04-11 18:34:41.139263 replit_river-0.1.2/replit_river/rpc.py
+-rw-r--r--   0        0        0     2152 2024-04-11 21:05:41.429562 replit_river-0.1.2/replit_river/seq_manager.py
+-rw-r--r--   0        0        0     1340 2024-04-11 21:05:27.021060 replit_river-0.1.2/replit_river/server.py
+-rw-r--r--   0        0        0    15581 2024-04-11 21:05:49.017905 replit_river-0.1.2/replit_river/transport.py
+-rw-r--r--   0        0        0     2450 1970-01-01 00:00:00.000000 replit_river-0.1.2/PKG-INFO
```

### Comparing `replit_river-0.1.1/LICENSE` & `replit_river-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.1/README.md` & `replit_river-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.1/pyproject.toml` & `replit_river-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name="replit-river"
-version="0.1.1"
+version="0.1.2"
 description="Replit river toolkit for Python"
 authors = ["Replit <eng@replit.com>"]
 license = "LICENSE"
 keywords = ["rpc", "websockets"]
 readme = "README.md"
 
 [tool.poetry.scripts]
```

### Comparing `replit_river-0.1.1/replit_river/client.py` & `replit_river-0.1.2/replit_river/client.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,40 +3,60 @@
 from collections.abc import AsyncIterable, AsyncIterator
 from typing import Any, Callable, Dict, Optional, Union
 
 import msgpack  # type: ignore
 import nanoid  # type: ignore
 from aiochannel import Channel
 from pydantic import ValidationError
-from river.error_schema import RiverException
 from websockets import Data
 from websockets.client import WebSocketClientProtocol
 from websockets.exceptions import ConnectionClosed
 
+from replit_river.error_schema import ERROR_CODE_STREAM_CLOSED, RiverException
+from replit_river.seq_manager import (
+    IgnoreTransportMessageException,
+    InvalidTransportMessageException,
+    SeqManager,
+)
+from replit_river.transport import FailedSendingMessageException
+
 from .rpc import (
+    ACK_BIT,
     STREAM_CLOSED_BIT,
     STREAM_OPEN_BIT,
     ControlMessageHandshakeRequest,
     ControlMessageHandshakeResponse,
     ErrorType,
     InitType,
     RequestType,
     ResponseType,
     TransportMessage,
 )
 
+CROSIS_PREFIX_BYTES = b"\x00\x00"
+PID2_PREFIX_BYTES = b"\xff\xff"
+
 
 class Client:
-    def __init__(self, websockets: WebSocketClientProtocol) -> None:
+    def __init__(
+        self,
+        websockets: WebSocketClientProtocol,
+        use_prefix_bytes: bool = True,
+        client_id: Optional[str] = None,
+        server_id: Optional[str] = None,
+    ) -> None:
         self.ws = websockets
         self._tasks = set()
         self._from = nanoid.generate()
         self._streams: Dict[str, Channel[Dict[str, Any]]] = {}
-        self._seq = 0
-        self._ack = 0
+        self._seq_manager = SeqManager()
+        self._is_handshaked = False
+        self._use_prefix_bytes = use_prefix_bytes
+        self._instance_id = client_id or "python-client-" + self.generate_nanoid()
+        self._server_id = server_id or "SERVER"
 
         task = asyncio.create_task(self._handle_messages())
         self._tasks.add(task)
 
         def _handle_messages_callback(task: asyncio.Task) -> None:
             self._tasks.remove(task)
             if task.exception():
@@ -46,132 +66,160 @@
 
         task.add_done_callback(_handle_messages_callback)
 
     async def send_close_stream(
         self, service_name: str, procedure_name: str, stream_id: str
     ) -> None:
         # close stream
-        msg = TransportMessage(
-            id=nanoid.generate(),
+        await self.send_transport_message(
             from_=self._from,
-            to="SERVER",
+            to=self._server_id,
             serviceName=service_name,
             procedureName=procedure_name,
             streamId=stream_id,
             controlFlags=STREAM_CLOSED_BIT,
-            ack=self._ack,
-            seq=self._seq,
             payload={
                 "type": "CLOSE",
             },
         )
-        await self.ws.send(msgpack.packb(msg.model_dump(by_alias=True), datetime=True))
 
     def to_transport_message(self, message: Data) -> TransportMessage:
         unpacked = msgpack.unpackb(message, timestamp=3)
 
         return TransportMessage(**unpacked)
 
-    async def send_transport_message(self, message: TransportMessage) -> None:
-        await self.ws.send(
-            msgpack.packb(
-                message.model_dump(by_alias=True),
-                datetime=True,
-            )
-        )
-        self._seq += 1
-
-    def pack_transport_message(
+    async def send_transport_message(
         self,
         from_: str,
         to: str,
-        serviceName: str,
-        procedureName: str,
+        serviceName: Optional[str],
+        procedureName: Optional[str],
         streamId: str,
         controlFlags: int,
         payload: Dict[str, Any],
-    ) -> TransportMessage:
-        return TransportMessage(
+        is_handshake: bool = False,
+    ) -> None:
+        current_seq = 0
+        if not is_handshake:
+            while not self._is_handshaked:
+                await asyncio.sleep(0.01)
+        if is_handshake:
+            current_seq = await self._seq_manager.get_seq()
+        else:
+            current_seq = await self._seq_manager.get_seq_and_increment()
+        current_ack = await self._seq_manager.get_ack()
+        message = TransportMessage(
             id=nanoid.generate(),
             from_=from_,
             to=to,
             serviceName=serviceName,
             procedureName=procedureName,
             streamId=streamId,
             controlFlags=controlFlags,
             payload=payload,
-            seq=self._seq,
-            ack=self._ack,
+            seq=current_seq,
+            ack=current_ack,
         )
+        prefix = PID2_PREFIX_BYTES if self._use_prefix_bytes else b""
+        try:
+            await self.ws.send(
+                prefix
+                + msgpack.packb(
+                    message.model_dump(by_alias=True, exclude_none=True),
+                    datetime=True,
+                )
+            )
+        except ConnectionClosed:
+            raise FailedSendingMessageException(
+                "Connection closed while sending message"
+            )
 
     def generate_nanoid(self) -> str:
         return str(nanoid.generate())
 
+    async def _receive_pid2_message(self) -> Data:
+        data = await self.ws.recv()
+        if self._use_prefix_bytes:
+            while data[:2] == CROSIS_PREFIX_BYTES:
+                data = await self.ws.recv()
+            return data[2:]
+        return data
+
     async def _handle_messages(self) -> None:
         handshake_request = ControlMessageHandshakeRequest(
             type="HANDSHAKE_REQ",
-            protocol_version="v1",
-            instance_id="python-client-" + self.generate_nanoid(),
+            protocolVersion="v1",
+            instanceId=self._instance_id,
         )
-        await self.send_transport_message(
-            TransportMessage(
-                id=self.generate_nanoid(),
+        try:
+            await self.send_transport_message(
                 from_=self._from,
-                to="SERVER",
-                seq=0,
-                ack=0,
+                to=self._server_id,
                 serviceName=None,
                 procedureName=None,
                 streamId=self.generate_nanoid(),
                 controlFlags=0,
                 payload=handshake_request.model_dump(),
+                is_handshake=True,
             )
-        )
-        first_message = self.to_transport_message(await self.ws.recv())
+        except FailedSendingMessageException:
+            raise RiverException(
+                ERROR_CODE_STREAM_CLOSED, "Stream closed before response"
+            )
+        data = await self._receive_pid2_message()
+        first_message = self.to_transport_message(data)
         try:
             handshake_response = ControlMessageHandshakeResponse(
                 **first_message.payload
             )
         except ValidationError:
             logging.error("Failed to parse handshake response")
             # TODO: close the connection here
             return
-        if not handshake_response.status["ok"]:
-            logging.error(f"Handshake failed: {handshake_response.status['message']}")
+        if not handshake_response.status.ok:
+            logging.error(f"Handshake failed: {handshake_response.status.reason}")
             # TODO: close the connection here
             return
+        self._is_handshaked = True
 
         async for message in self.ws:
             if isinstance(message, str):
                 # Not something we will try to handle.
                 logging.debug(
                     "ignored a message beacuse it was a text frame: %r",
                     message,
                 )
                 continue
+            if self._use_prefix_bytes:
+                if message[:2] == CROSIS_PREFIX_BYTES:
+                    logging.debug("ignored a crosis message")
+                    continue
+                message = message[2:]
+
             try:
                 unpacked = msgpack.unpackb(message, timestamp=3)
-
                 msg = TransportMessage(**unpacked)
-                if msg.seq != self._ack:
-                    logging.debug(
-                        "Received out of order message: %d, expected %d",
-                        msg.seq,
-                        self._ack,
-                    )
+                try:
+                    await self._seq_manager.check_seq_and_update(msg)
+                except IgnoreTransportMessageException:
                     continue
-                self.ack = msg.seq + 1
+                except InvalidTransportMessageException:
+                    return
+                if msg.controlFlags == ACK_BIT:
+                    continue
+
             except ConnectionClosed:
                 logging.info("Connection closed")
                 break
 
             except (
                 ValidationError,
                 ValueError,
                 msgpack.UnpackException,
+                msgpack.exceptions.ExtraData,
             ):
                 logging.exception("failed to parse message")
                 return
             previous_output = self._streams.get(msg.streamId, None)
             if not previous_output:
                 logging.warning("no stream for %s", msg.streamId)
                 continue
@@ -194,31 +242,39 @@
 
         Expects the input and output be messages that will be msgpacked.
         """
 
         stream_id = nanoid.generate()
         output: Channel[Any] = Channel(1)
         self._streams[stream_id] = output
-
-        msg = self.pack_transport_message(
-            from_=self._from,
-            to="SERVER",
-            serviceName=service_name,
-            procedureName=procedure_name,
-            streamId=stream_id,
-            controlFlags=STREAM_OPEN_BIT | STREAM_CLOSED_BIT,
-            payload=request_serializer(request),
-        )
-        await self.send_transport_message(msg)
+        try:
+            await self.send_transport_message(
+                from_=self._from,
+                to=self._server_id,
+                serviceName=service_name,
+                procedureName=procedure_name,
+                streamId=stream_id,
+                controlFlags=STREAM_OPEN_BIT | STREAM_CLOSED_BIT,
+                payload=request_serializer(request),
+            )
+        except FailedSendingMessageException:
+            raise RiverException(
+                ERROR_CODE_STREAM_CLOSED, "Stream closed before response"
+            )
 
         # Handle potential errors during communication
         try:
-            response = await output.get()
-            if response.get("ack", None):
+            try:
                 response = await output.get()
+            except RuntimeError:
+                # if the stream is closed before we get a response, we will get a
+                # RuntimeError: RuntimeError: Event loop is closed
+                raise RiverException(
+                    ERROR_CODE_STREAM_CLOSED, "Stream closed before response"
+                )
             if not response.get("ok", False):
                 try:
                     error = error_deserializer(response["payload"])
                 except Exception as e:
                     raise RiverException("error_deserializer", str(e))
                 raise RiverException(error.code, error.message)
             return response_deserializer(response["payload"])
@@ -245,55 +301,57 @@
         Expects the input and output be messages that will be msgpacked.
         """
 
         stream_id = nanoid.generate()
         output: Channel[Any] = Channel(1024)
         self._streams[stream_id] = output
         first_message = True
-        num_sent_messages = 0
-        if init and init_serializer:
-            num_sent_messages += 1
-            msg = self.pack_transport_message(
-                from_=self._from,
-                to="SERVER",
-                serviceName=service_name,
-                procedureName=procedure_name,
-                streamId=stream_id,
-                controlFlags=STREAM_OPEN_BIT,
-                payload=init_serializer(init),
-            )
-            await self.send_transport_message(msg)
-            first_message = False
-
-        async for item in request:
-            control_flags = 0
-            if first_message:
-                control_flags = STREAM_OPEN_BIT
+        try:
+            if init and init_serializer:
+                await self.send_transport_message(
+                    from_=self._from,
+                    to=self._server_id,
+                    serviceName=service_name,
+                    procedureName=procedure_name,
+                    streamId=stream_id,
+                    controlFlags=STREAM_OPEN_BIT,
+                    payload=init_serializer(init),
+                )
                 first_message = False
-            num_sent_messages += 1
-            msg = self.pack_transport_message(
-                from_=self._from,
-                to="SERVER",
-                serviceName=service_name,
-                procedureName=procedure_name,
-                streamId=stream_id,
-                controlFlags=control_flags,
-                payload=request_serializer(item),
+
+            async for item in request:
+                control_flags = 0
+                if first_message:
+                    control_flags = STREAM_OPEN_BIT
+                    first_message = False
+                await self.send_transport_message(
+                    from_=self._from,
+                    to=self._server_id,
+                    serviceName=service_name,
+                    procedureName=procedure_name,
+                    streamId=stream_id,
+                    controlFlags=control_flags,
+                    payload=request_serializer(item),
+                )
+        except FailedSendingMessageException:
+            raise RiverException(
+                ERROR_CODE_STREAM_CLOSED, "Stream closed before response"
             )
-            await self.send_transport_message(msg)
-        num_sent_messages += 1
         await self.send_close_stream(service_name, procedure_name, stream_id)
 
         # Handle potential errors during communication
         try:
-            for _ in range(num_sent_messages):
-                ack_response = await output.get()
-                if not ack_response.get("ack", None):
-                    raise RiverException("ack error", "No ack received")
-            response = await output.get()
+            try:
+                response = await output.get()
+            except RuntimeError:
+                # if the stream is closed before we get a response, we will get a
+                # RuntimeError: RuntimeError: Event loop is closed
+                raise RiverException(
+                    ERROR_CODE_STREAM_CLOSED, "Stream closed before response"
+                )
             if not response.get("ok", False):
                 try:
                     error = error_deserializer(response["payload"])
                 except Exception as e:
                     raise RiverException("error_deserializer", str(e))
                 raise RiverException(error.code, error.message)
 
@@ -317,33 +375,33 @@
         """Sends a subscription request to the server.
 
         Expects the input and output be messages that will be msgpacked.
         """
         stream_id = nanoid.generate()
         output: Channel[Any] = Channel(1024)
         self._streams[stream_id] = output
-        msg = self.pack_transport_message(
-            from_=self._from,
-            to="SERVER",
-            serviceName=service_name,
-            procedureName=procedure_name,
-            streamId=stream_id,
-            controlFlags=STREAM_OPEN_BIT,
-            payload=request_serializer(request),
-        )
-        await self.send_transport_message(msg)
+        try:
+            await self.send_transport_message(
+                from_=self._from,
+                to=self._server_id,
+                serviceName=service_name,
+                procedureName=procedure_name,
+                streamId=stream_id,
+                controlFlags=STREAM_OPEN_BIT,
+                payload=request_serializer(request),
+            )
+        except FailedSendingMessageException:
+            raise RiverException(
+                ERROR_CODE_STREAM_CLOSED, "Stream closed before response"
+            )
 
         # Handle potential errors during communication
         try:
-            ack_response = await output.get()
-            if not ack_response.get("ack", None):
-                raise RiverException("ack error", "No ack received")
-
             async for item in output:
-                if "type" in item and item["type"] == "CLOSE":
+                if item.get("type", None) == "CLOSE":
                     break
                 if not item.get("ok", False):
                     try:
                         yield error_deserializer(item["payload"])
                     except Exception:
                         logging.exception(
                             f"Error during subscription error deserialization: {item}"
@@ -370,77 +428,68 @@
 
         Expects the input and output be messages that will be msgpacked.
         """
 
         stream_id = nanoid.generate()
         output: Channel[Any] = Channel(1024)
         self._streams[stream_id] = output
-        num_sent_messages = 0
+        try:
+            if init and init_serializer:
+                await self.send_transport_message(
+                    from_=self._from,
+                    to=self._server_id,
+                    serviceName=service_name,
+                    procedureName=procedure_name,
+                    streamId=stream_id,
+                    controlFlags=STREAM_OPEN_BIT,
+                    payload=init_serializer(init),
+                )
+            else:
+                # Get the very first message to open the stream
+                request_iter = aiter(request)
+                first = await anext(request_iter)
+                await self.send_transport_message(
+                    from_=self._from,
+                    to=self._server_id,
+                    serviceName=service_name,
+                    procedureName=procedure_name,
+                    streamId=stream_id,
+                    controlFlags=STREAM_OPEN_BIT,
+                    payload=request_serializer(first),
+                )
 
-        if init and init_serializer:
-            num_sent_messages += 1
-            msg = self.pack_transport_message(
-                from_=self._from,
-                to="SERVER",
-                serviceName=service_name,
-                procedureName=procedure_name,
-                streamId=stream_id,
-                controlFlags=STREAM_OPEN_BIT,
-                payload=init_serializer(init),
+        except FailedSendingMessageException:
+            raise RiverException(
+                ERROR_CODE_STREAM_CLOSED, "Stream closed before response"
             )
-            await self.send_transport_message(msg)
-        else:
-            num_sent_messages += 1
-            # Get the very first message to open the stream
-            request_iter = aiter(request)
-            first = await anext(request_iter)
-            msg = self.pack_transport_message(
-                from_=self._from,
-                to="SERVER",
-                serviceName=service_name,
-                procedureName=procedure_name,
-                streamId=stream_id,
-                controlFlags=STREAM_OPEN_BIT,
-                payload=request_serializer(first),
-            )
-            await self.send_transport_message(msg)
 
         # Create the encoder task
         async def _encode_stream() -> None:
             async for item in request:
-                nonlocal num_sent_messages
-                num_sent_messages += 1
-                msg = self.pack_transport_message(
+                if item is None:
+                    continue
+                await self.send_transport_message(
                     from_=self._from,
-                    to="SERVER",
+                    to=self._server_id,
                     serviceName=service_name,
                     procedureName=procedure_name,
                     streamId=stream_id,
                     controlFlags=0,
                     payload=request_serializer(item),
                 )
-                await self.send_transport_message(msg)
-            num_sent_messages += 1
             await self.send_close_stream(service_name, procedure_name, stream_id)
 
         task = asyncio.create_task(_encode_stream())
         self._tasks.add(task)
         task.add_done_callback(lambda _: self._tasks.remove(task))
 
-        for _ in range(num_sent_messages):
-            ack_response = await output.get()
-            if not ack_response.get("ack", None):
-                raise RiverException("ack error", "No ack received")
-
         # Handle potential errors during communication
         try:
             async for item in output:
                 if "type" in item and item["type"] == "CLOSE":
-                    # close the stream here
-                    self._streams[stream_id].close()
                     break
                 if not item.get("ok", False):
                     try:
                         yield error_deserializer(item["payload"])
                     except Exception:
                         logging.exception(
                             f"Error during subscription error deserialization: {item}"
```

### Comparing `replit_river-0.1.1/replit_river/codegen/client.py` & `replit_river-0.1.2/replit_river/codegen/client.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.1/replit_river/codegen/run.py` & `replit_river-0.1.2/replit_river/codegen/run.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.1/replit_river/codegen/schema.py` & `replit_river-0.1.2/replit_river/codegen/schema.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.1/replit_river/codegen/server.py` & `replit_river-0.1.2/replit_river/codegen/server.py`

 * *Files identical despite different names*

### Comparing `replit_river-0.1.1/replit_river/rpc.py` & `replit_river-0.1.2/replit_river/rpc.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,15 +17,16 @@
     TypeVar,
     Union,
 )
 
 import grpc
 from aiochannel import Channel
 from pydantic import BaseModel, ConfigDict, Field
-from river.error_schema import RiverError
+
+from replit_river.error_schema import RiverError
 
 InitType = TypeVar("InitType")
 RequestType = TypeVar("RequestType")
 ResponseType = TypeVar("ResponseType")
 ErrorType = TypeVar("ErrorType", bound=RiverError)
 
 _MetadataType = Union[grpc.aio.Metadata, Sequence[Tuple[str, Union[str, bytes]]]]
@@ -38,22 +39,30 @@
 STREAM_CLOSED_BIT = 0x0004
 
 
 # Equivalent of https://github.com/replit/river/blob/c1345f1ff6a17a841d4319fad5c153b5bda43827/transport/message.ts#L23-L33
 
 
 class ControlMessageHandshakeRequest(BaseModel):
-    type: Literal["HANDSHAKE_REQ"]
-    protocol_version: str
-    instance_id: str
+    type: Literal["HANDSHAKE_REQ"] = "HANDSHAKE_REQ"
+    protocolVersion: str
+    instanceId: str
+
+
+class HandShakeStatus(BaseModel):
+    ok: bool
+    # Instance id should be server level id, each server have one
+    instanceId: Optional[str] = None
+    # Reason for failure
+    reason: Optional[str] = None
 
 
 class ControlMessageHandshakeResponse(BaseModel):
-    type: Literal["HANDSHAKE_RESP"]
-    status: Dict
+    type: Literal["HANDSHAKE_RESP"] = "HANDSHAKE_RESP"
+    status: HandShakeStatus
 
 
 class TransportMessage(BaseModel):
     id: str
     from_: str = Field(..., alias="from")
     to: str
     seq: int
@@ -136,14 +145,32 @@
         pass
 
     async def write(self, message: ResponseType) -> None:
         # Normally this method should not be used.
         raise grpc.RpcError()
 
 
+def get_response_or_error_payload(
+    response: Any, response_serializer: Callable[[ResponseType], Any]
+) -> Dict:
+    if isinstance(response, RiverError):
+        return {
+            "ok": False,
+            "payload": {
+                "code": response.code,
+                "message": response.message,
+            },
+        }
+    else:
+        return {
+            "ok": True,
+            "payload": response_serializer(response),
+        }
+
+
 def rpc_method_handler(
     method: Callable[[RequestType, grpc.aio.ServicerContext], Awaitable[ResponseType]],
     request_deserializer: Callable[[str], RequestType],
     response_serializer: Callable[[ResponseType], Any],
 ) -> GenericRpcHandler:
     async def wrapped(
         peer: str,
@@ -151,18 +178,15 @@
         output: Channel[Any],
     ) -> None:
         try:
             context = GrpcContext(peer)
             request = request_deserializer(await input.get())
             response = await method(request, context)
             await output.put(
-                {
-                    "ok": True,
-                    "payload": response_serializer(response),
-                }
+                get_response_or_error_payload(response, response_serializer)
             )
         except grpc.RpcError:
             await output.put(
                 {
                     "ok": False,
                     "payload": {
                         "code": grpc.StatusCode(context._abort_code).name,
@@ -201,18 +225,15 @@
         output: Channel[Any],
     ) -> None:
         try:
             context = GrpcContext(peer)
             request = request_deserializer(await input.get())
             async for response in method(request, context):
                 await output.put(
-                    {
-                        "ok": True,
-                        "payload": response_serializer(response),
-                    }
+                    get_response_or_error_payload(response, response_serializer)
                 )
         except grpc.RpcError:
             await output.put(
                 {
                     "ok": False,
                     "payload": {
                         "code": grpc.StatusCode(context._abort_code).name,
@@ -260,20 +281,17 @@
                     async for item in input:
                         await request.put(request_deserializer(item))
                 finally:
                     request.close()
 
             async def _convert_outputs() -> None:
                 try:
-                    item = await method(request, context)
+                    response = await method(request, context)
                     await output.put(
-                        {
-                            "ok": True,
-                            "payload": response_serializer(item),
-                        }
+                        get_response_or_error_payload(response, response_serializer)
                     )
                 except Exception as e:
                     print("upload caught exception", e)
                     await output.put(
                         {
                             "ok": False,
                             "payload": {
@@ -331,18 +349,15 @@
 
             response = method(request, context)
 
             async def _convert_outputs() -> None:
                 try:
                     async for item in response:
                         await output.put(
-                            {
-                                "ok": True,
-                                "payload": response_serializer(item),
-                            }
+                            get_response_or_error_payload(item, response_serializer)
                         )
                 finally:
                     output.close()
 
             convert_inputs_task = asyncio.create_task(_convert_inputs())
             convert_outputs_task = asyncio.create_task(_convert_outputs())
             await asyncio.wait((convert_inputs_task, convert_outputs_task))
```

### Comparing `replit_river-0.1.1/PKG-INFO` & `replit_river-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: replit-river
-Version: 0.1.1
+Version: 0.1.2
 Summary: Replit river toolkit for Python
 License: LICENSE
 Keywords: rpc,websockets
 Author: Replit
 Author-email: eng@replit.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
```

