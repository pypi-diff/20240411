# Comparing `tmp/uhppoted-0.8.8.tar.gz` & `tmp/uhppoted-0.8.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uhppoted-0.8.8.tar", last modified: Tue Mar 26 20:09:53 2024, max compression
+gzip compressed data, was "uhppoted-0.8.8.1.tar", last modified: Thu Apr 11 18:22:01 2024, max compression
```

## Comparing `uhppoted-0.8.8.tar` & `uhppoted-0.8.8.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 tonyseebregts   (501) staff       (20)        0 2024-03-26 20:09:53.805251 uhppoted-0.8.8/
--rw-r--r--   0 tonyseebregts   (501) staff       (20)     1065 2023-08-08 17:29:06.000000 uhppoted-0.8.8/LICENSE
--rw-r--r--   0 tonyseebregts   (501) staff       (20)    29899 2024-03-26 20:09:53.804299 uhppoted-0.8.8/PKG-INFO
--rw-r--r--   0 tonyseebregts   (501) staff       (20)    29224 2024-02-29 17:11:16.000000 uhppoted-0.8.8/README.md
--rw-r--r--   0 tonyseebregts   (501) staff       (20)      779 2024-02-29 17:06:58.000000 uhppoted-0.8.8/pyproject.toml
--rw-r--r--   0 tonyseebregts   (501) staff       (20)       38 2024-03-26 20:09:53.805405 uhppoted-0.8.8/setup.cfg
-drwxr-xr-x   0 tonyseebregts   (501) staff       (20)        0 2024-03-26 20:09:53.795784 uhppoted-0.8.8/src/
-drwxr-xr-x   0 tonyseebregts   (501) staff       (20)        0 2024-03-26 20:09:53.799098 uhppoted-0.8.8/src/uhppoted/
--rw-r--r--   0 tonyseebregts   (501) staff       (20)    41438 2024-02-29 17:06:58.000000 uhppoted-0.8.8/src/uhppoted/decode.py
--rw-r--r--   0 tonyseebregts   (501) staff       (20)    24308 2024-02-29 17:06:58.000000 uhppoted-0.8.8/src/uhppoted/encode.py
--rw-r--r--   0 tonyseebregts   (501) staff       (20)    18458 2024-02-29 17:06:58.000000 uhppoted-0.8.8/src/uhppoted/structs.py
--rw-r--r--   0 tonyseebregts   (501) staff       (20)     7573 2023-08-11 16:43:19.000000 uhppoted-0.8.8/src/uhppoted/udp.py
--rw-r--r--   0 tonyseebregts   (501) staff       (20)    31690 2024-02-29 17:06:58.000000 uhppoted-0.8.8/src/uhppoted/uhppote.py
-drwxr-xr-x   0 tonyseebregts   (501) staff       (20)        0 2024-03-26 20:09:53.802682 uhppoted-0.8.8/src/uhppoted.egg-info/
--rw-r--r--   0 tonyseebregts   (501) staff       (20)    29899 2024-03-26 20:09:53.000000 uhppoted-0.8.8/src/uhppoted.egg-info/PKG-INFO
--rw-r--r--   0 tonyseebregts   (501) staff       (20)      325 2024-03-26 20:09:53.000000 uhppoted-0.8.8/src/uhppoted.egg-info/SOURCES.txt
--rw-r--r--   0 tonyseebregts   (501) staff       (20)        1 2024-03-26 20:09:53.000000 uhppoted-0.8.8/src/uhppoted.egg-info/dependency_links.txt
--rw-r--r--   0 tonyseebregts   (501) staff       (20)       41 2024-03-26 20:09:53.000000 uhppoted-0.8.8/src/uhppoted.egg-info/requires.txt
--rw-r--r--   0 tonyseebregts   (501) staff       (20)        9 2024-03-26 20:09:53.000000 uhppoted-0.8.8/src/uhppoted.egg-info/top_level.txt
+drwxr-xr-x   0 tonyseebregts   (501) staff       (20)        0 2024-04-11 18:22:01.557420 uhppoted-0.8.8.1/
+-rw-r--r--   0 tonyseebregts   (501) staff       (20)     1065 2023-08-08 17:29:06.000000 uhppoted-0.8.8.1/LICENSE
+-rw-r--r--   0 tonyseebregts   (501) staff       (20)    30812 2024-04-11 18:22:01.556491 uhppoted-0.8.8.1/PKG-INFO
+-rw-r--r--   0 tonyseebregts   (501) staff       (20)    30135 2024-04-11 03:11:25.000000 uhppoted-0.8.8.1/README.md
+-rw-r--r--   0 tonyseebregts   (501) staff       (20)      781 2024-04-01 16:16:26.000000 uhppoted-0.8.8.1/pyproject.toml
+-rw-r--r--   0 tonyseebregts   (501) staff       (20)       38 2024-04-11 18:22:01.557577 uhppoted-0.8.8.1/setup.cfg
+drwxr-xr-x   0 tonyseebregts   (501) staff       (20)        0 2024-04-11 18:22:01.549283 uhppoted-0.8.8.1/src/
+drwxr-xr-x   0 tonyseebregts   (501) staff       (20)        0 2024-04-11 18:22:01.552695 uhppoted-0.8.8.1/src/uhppoted/
+-rw-r--r--   0 tonyseebregts   (501) staff       (20)    41438 2024-02-29 17:06:58.000000 uhppoted-0.8.8.1/src/uhppoted/decode.py
+-rw-r--r--   0 tonyseebregts   (501) staff       (20)    24907 2024-04-08 17:41:56.000000 uhppoted-0.8.8.1/src/uhppoted/encode.py
+-rw-r--r--   0 tonyseebregts   (501) staff       (20)    18458 2024-02-29 17:06:58.000000 uhppoted-0.8.8.1/src/uhppoted/structs.py
+-rw-r--r--   0 tonyseebregts   (501) staff       (20)     9087 2024-04-10 17:57:03.000000 uhppoted-0.8.8.1/src/uhppoted/udp.py
+-rw-r--r--   0 tonyseebregts   (501) staff       (20)    41760 2024-04-08 17:35:31.000000 uhppoted-0.8.8.1/src/uhppoted/uhppote.py
+drwxr-xr-x   0 tonyseebregts   (501) staff       (20)        0 2024-04-11 18:22:01.555296 uhppoted-0.8.8.1/src/uhppoted.egg-info/
+-rw-r--r--   0 tonyseebregts   (501) staff       (20)    30812 2024-04-11 18:22:01.000000 uhppoted-0.8.8.1/src/uhppoted.egg-info/PKG-INFO
+-rw-r--r--   0 tonyseebregts   (501) staff       (20)      325 2024-04-11 18:22:01.000000 uhppoted-0.8.8.1/src/uhppoted.egg-info/SOURCES.txt
+-rw-r--r--   0 tonyseebregts   (501) staff       (20)        1 2024-04-11 18:22:01.000000 uhppoted-0.8.8.1/src/uhppoted.egg-info/dependency_links.txt
+-rw-r--r--   0 tonyseebregts   (501) staff       (20)       41 2024-04-11 18:22:01.000000 uhppoted-0.8.8.1/src/uhppoted.egg-info/requires.txt
+-rw-r--r--   0 tonyseebregts   (501) staff       (20)        9 2024-04-11 18:22:01.000000 uhppoted-0.8.8.1/src/uhppoted.egg-info/top_level.txt
```

### Comparing `uhppoted-0.8.8/LICENSE` & `uhppoted-0.8.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `uhppoted-0.8.8/PKG-INFO` & `uhppoted-0.8.8.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uhppoted
-Version: 0.8.8
+Version: 0.8.8.1
 Summary: Python API for the UHPPOTE TCP/IP access controllers
 Author-email: uhppoted <uhppoted.development@gmail.com>
 Project-URL: Homepage, https://github.com/uhppoted/uhppoted-python
 Project-URL: Bug Tracker, https://github.com/uhppoted/uhppoted-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -97,15 +97,26 @@
   'gateway': IPv4Address('192.168.1.1'),
   'ip_address': IPv4Address('192.168.1.100'),
   'mac_address': '00:12:23:34::45:56',
   'subnet_mask': IPv4Address('255.255.255.0'),
   'version': 'v8.92'}
 ```
 
-All API functions raise an `Exception` if the call fails for any reason whatsoever.
+### Notes
+1. All API functions raise an `Exception` if the call fails for any reason whatsoever.
+2. All API functions (other than `get_controllers` and `listen`) take an optional `dest_addr` kwarg that sets the
+   IP address to which to send the request, e.g.:
+```
+   get_controller(controller, dest_addr='192.168.1.100:60000')
+```
+3. All API functions (other than `listen`) take an optional `timeout` kwarg that sets the time limit for the 
+   request (in seconds), e.g.:
+```
+   get_controller(controller, dest_addr='192.168.1.100:60000', timeout=0.75)
+```
 
 ### `get_controllers`
 ```
 get_controllers()
 
 Returns an array of `GetControllerResponse`.
 
@@ -459,14 +470,35 @@
 
 ID  uint32  controller serial number 
 
 
 Raises an Exception if the call failed for any reason.
 ```
 
+### `listen`
+```
+listen(handler)
+
+handler  event handling callback function of the form
+         def on_event(event):
+              ...
+
+Raises an Exception if the call failed for any reason.
+```
+
+`listen` is a blocking call that will invoke the `handler` function for each received event, e.g.:
+```
+    ...
+    u.listen(on_event)
+
+def on_event(event):
+    if event != None:
+        pprint(event.__dict__, indent=2, width=1)
+    ...
+```
 
 ## Types
 
 ### `GetControllerResponse`
 
 Container class for the decoded response from a get-controller request.
```

### Comparing `uhppoted-0.8.8/README.md` & `uhppoted-0.8.8.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -79,15 +79,26 @@
   'gateway': IPv4Address('192.168.1.1'),
   'ip_address': IPv4Address('192.168.1.100'),
   'mac_address': '00:12:23:34::45:56',
   'subnet_mask': IPv4Address('255.255.255.0'),
   'version': 'v8.92'}
 ```
 
-All API functions raise an `Exception` if the call fails for any reason whatsoever.
+### Notes
+1. All API functions raise an `Exception` if the call fails for any reason whatsoever.
+2. All API functions (other than `get_controllers` and `listen`) take an optional `dest_addr` kwarg that sets the
+   IP address to which to send the request, e.g.:
+```
+   get_controller(controller, dest_addr='192.168.1.100:60000')
+```
+3. All API functions (other than `listen`) take an optional `timeout` kwarg that sets the time limit for the 
+   request (in seconds), e.g.:
+```
+   get_controller(controller, dest_addr='192.168.1.100:60000', timeout=0.75)
+```
 
 ### `get_controllers`
 ```
 get_controllers()
 
 Returns an array of `GetControllerResponse`.
 
@@ -441,14 +452,35 @@
 
 ID  uint32  controller serial number 
 
 
 Raises an Exception if the call failed for any reason.
 ```
 
+### `listen`
+```
+listen(handler)
+
+handler  event handling callback function of the form
+         def on_event(event):
+              ...
+
+Raises an Exception if the call failed for any reason.
+```
+
+`listen` is a blocking call that will invoke the `handler` function for each received event, e.g.:
+```
+    ...
+    u.listen(on_event)
+
+def on_event(event):
+    if event != None:
+        pprint(event.__dict__, indent=2, width=1)
+    ...
+```
 
 ## Types
 
 ### `GetControllerResponse`
 
 Container class for the decoded response from a get-controller request.
```

### Comparing `uhppoted-0.8.8/pyproject.toml` & `uhppoted-0.8.8.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "uhppoted"
-version = "0.8.8"
+version = "0.8.8.1"
 authors = [
   { name="uhppoted", email="uhppoted.development@gmail.com" },
 ]
 description = "Python API for the UHPPOTE TCP/IP access controllers"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `uhppoted-0.8.8/src/uhppoted/decode.py` & `uhppoted-0.8.8.1/src/uhppoted/decode.py`

 * *Files identical despite different names*

### Comparing `uhppoted-0.8.8/src/uhppoted/encode.py` & `uhppoted-0.8.8.1/src/uhppoted/encode.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 Encodes a UHPPOTE access controller request as a 64 byte UDP packet:
 
 - uint8, uint16, uint24 and uint32 values are encoded as little endian unsigned integers
 - datetime, date and time values are encoded as BCD
 - boolean values are encoded as 0 (False) or 1 (True)
 '''
 
+import datetime
 import struct
 
 
 def get_controller_request(controller):
     '''
     Encodes a get-controller request.
 
@@ -527,20 +528,45 @@
     pack_bool(monday, packet, 17)
     pack_bool(tuesday, packet, 18)
     pack_bool(wednesday, packet, 19)
     pack_bool(thursday, packet, 20)
     pack_bool(friday, packet, 21)
     pack_bool(saturday, packet, 22)
     pack_bool(sunday, packet, 23)
-    pack_HHmm(segment_1_start, packet, 24)
-    pack_HHmm(segment_1_end, packet, 26)
-    pack_HHmm(segment_2_start, packet, 28)
-    pack_HHmm(segment_2_end, packet, 30)
-    pack_HHmm(segment_3_start, packet, 32)
-    pack_HHmm(segment_3_end, packet, 34)
+
+    if segment_1_start == None:
+        pack_HHmm(datetime.time(0, 0), packet, 24)
+    else:
+        pack_HHmm(segment_1_start, packet, 24)
+
+    if segment_1_end == None:
+        pack_HHmm(datetime.time(0, 0), packet, 26)
+    else:
+        pack_HHmm(segment_1_end, packet, 26)
+
+    if segment_2_start == None:
+        pack_HHmm(datetime.time(0, 0), packet, 28)
+    else:
+        pack_HHmm(segment_2_start, packet, 28)
+
+    if segment_2_end == None:
+        pack_HHmm(datetime.time(0, 0), packet, 30)
+    else:
+        pack_HHmm(segment_2_end, packet, 30)
+
+    if segment_3_start == None:
+        pack_HHmm(datetime.time(0, 0), packet, 32)
+    else:
+        pack_HHmm(segment_3_start, packet, 32)
+
+    if segment_3_end == None:
+        pack_HHmm(datetime.time(0, 0), packet, 34)
+    else:
+        pack_HHmm(segment_3_end, packet, 34)
+
     pack_uint8(linked_profile_id, packet, 36)
 
     return packet
 
 
 def delete_all_time_profiles_request(controller):
     '''
```

### Comparing `uhppoted-0.8.8/src/uhppoted/structs.py` & `uhppoted-0.8.8.1/src/uhppoted/structs.py`

 * *Files identical despite different names*

### Comparing `uhppoted-0.8.8/src/uhppoted/udp.py` & `uhppoted-0.8.8.1/src/uhppoted/udp.py`

 * *Files 21% similar despite different names*

```diff
@@ -37,22 +37,23 @@
                           address:port combination.
         '''
         self._bind = (bind, 0)
         self._broadcast = resolve(broadcast)
         self._listen = resolve(listen)
         self._debug = debug
 
-    def broadcast(self, request):
+    def broadcast(self, request, timeout=2.5):
         '''
         Binds to the bind address from the constructor and then broadcasts a UDP request to the broadcast
         address from the constructor and then waits 5 seconds for the replies from any reponding access 
         controllers.
 
             Parameters:
                request  (bytearray)  64 byte request packet.
+                timeout (float)      Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                List of received response packets (may be empty).
 
             Raises:
                Error  For any socket related errors.
         '''
@@ -64,25 +65,28 @@
             sock.bind(self._bind)
             sock.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
             sock.setsockopt(socket.SOL_SOCKET, socket.SO_SNDTIMEO, WRITE_TIMEOUT)
             sock.setsockopt(socket.SOL_SOCKET, socket.SO_RCVTIMEO, READ_TIMEOUT)
 
             sock.sendto(request, self._broadcast)
 
-            return read_all(sock, self._debug)
+            return _read_all(sock, timeout=timeout, debug=self._debug)
         finally:
             sock.close()
 
-    def send(self, request):
+    def send(self, request, dest_addr=None, timeout=2.5):
         '''
         Binds to the bind address from the constructor and then broadcasts a UDP request to the broadcast,
         and then waits 5 seconds for a reply from the destination access controllers.
 
             Parameters:
-               request  (bytearray)  64 byte request packet.
+               request   (bytearray)  64 byte request packet.
+               dest_addr (string)     Optional IPv4 address:port of the controller. Defaults to port 60000
+                                      if dest_addr does not include a port.
+              timeout (float)         Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                Received response packet (if any) or None (for set-ip request).
 
             Raises:
                Error  For any socket related errors.
         '''
@@ -93,20 +97,24 @@
 
         try:
             sock.bind(self._bind)
             sock.setsockopt(socket.SOL_SOCKET, socket.SO_BROADCAST, 1)
             sock.setsockopt(socket.SOL_SOCKET, socket.SO_SNDTIMEO, WRITE_TIMEOUT)
             sock.setsockopt(socket.SOL_SOCKET, socket.SO_RCVTIMEO, READ_TIMEOUT)
 
-            sock.sendto(request, self._broadcast)
+            if dest_addr == None:
+                sock.sendto(request, self._broadcast)
+            else:
+                addr = resolve(f'{dest_addr}')
+                sock.sendto(request, addr)
 
             if request[1] == 0x96:
                 return None
 
-            return read(sock, self._debug)
+            return _read(sock, timeout=timeout, debug=self._debug)
         finally:
             sock.close()
 
     def listen(self, onEvent):
         '''
         Binds to the listen address from the constructor and invokes the events handler for
         any received 64 byte UDP packets. Invalid'ish packets are silently discarded.
@@ -148,52 +156,58 @@
                None.
         '''
         if self._debug:
             dump(packet)
 
 
 # TODO convert to asyncio
-def read(sock, debug):
+def _read(sock, timeout=2.5, debug=False):
     '''
     Waits 2.5 seconds for a single 64 byte packet to be received on the socket. Prints the packet to the console
     if debug is True.
 
         Parameters:
-            sock  (socket)  Initialised and open UDP socket.
-            debug (bool)    Enables dumping the received packet to the console.
+            sock    (socket)  Initialised and open UDP socket.
+            timeout (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
+            debug   (bool)    Enables dumping the received packet to the console.
 
         Returns:
             Received 64 byte UDP packet (or None).
     '''
-    sock.settimeout(2.5)
+    time_limit = timeout_to_seconds(timeout)
+
+    sock.settimeout(time_limit)
 
     while True:
         reply = sock.recv(1024)
         if len(reply) == 64:
             if debug:
                 dump(reply)
             return reply
 
     return None
 
 
 # TODO convert to asyncio
-def read_all(sock, debug):
+def _read_all(sock, timeout=2.5, debug=False):
     '''
     Accumulates received 64 byte UDP packets, waiting up to 2.5 seconds for an incoming packet. Prints the 
     packet to the console if debug is True.
 
         Parameters:
-            sock  (socket)  Initialised and open UDP socket.
-            debug (bool)    Enables dumping the received packet to the console.
+            sock    (socket) Initialised and open UDP socket.
+            timeout (float)  Optional operation timeout (in seconds). Defaults to 2.5s.
+            debug   (bool)   Enables dumping the received packet to the console.
 
         Returns:
             List of received 64 byte UDP packets (may be empty).
     '''
-    sock.settimeout(2.5)
+    time_limit = timeout_to_seconds(timeout)
+
+    sock.settimeout(time_limit)
 
     replies = []
     while True:
         try:
             reply = sock.recv(1024)
             if len(reply) == 64:
                 replies.append(reply)
@@ -220,14 +234,37 @@
     if match:
         return (match.group(1), int(match.group(2)))
     else:
         address = ipaddress.IPv4Address(addr)
         return (str(address), 60000)
 
 
+def timeout_to_seconds(val, defval=2.5):
+    '''
+    Converts a timeout value to seconds, returning the default value if the supplied value
+    is None, cannot be converted, or is out of the range [50ms..30s]
+
+        Parameters:
+            val    (float)  Timeout in seconds
+            defval (float)  Optional default values.
+
+        Returns:
+            timeout in seconds as a float
+    '''
+    try:
+        if val != None:
+            v = float(f'{val}')
+            if v >= 0.05 and v <= 30:
+                return v
+    except:
+        pass
+
+    return defval
+
+
 def dump(packet):
     '''
     Prints a packet to the console as a formatted hexadecimal string.
 
         Parameters:
            packet  (bytearray)  64 byte UDP packet.
```

### Comparing `uhppoted-0.8.8/src/uhppoted/uhppote.py` & `uhppoted-0.8.8.1/src/uhppoted/uhppote.py`

 * *Files 24% similar despite different names*

```diff
@@ -25,502 +25,576 @@
 
             Raises:
                ValueError  If any of the supplied IPv4 values cannot be translated to a valid IPv4 
                            address:port combination.
         '''
         self._udp = udp.UDP(bind, broadcast, listen, debug)
 
-    def get_all_controllers(self):
+    def get_all_controllers(self, timeout=2.5):
         '''
         Retrieves a list of all controllers accessible on the local LAN segment.
 
+            Parameters:
+              timeout (float)  Optional operation timeout (in seconds). Defaults to 2.5s.
+
             Returns:
                []GetControllerResponse  List of get_controller_responses from access controllers 
                                        on the local LAN segment.
 
             Raises:
                Exception  If any of the responses from the access controllers cannot be decoded.
         '''
         request = encode.get_controller_request(0)
-        replies = self._udp.broadcast(request)
+        replies = self._udp.broadcast(request, timeout=timeout)
 
         list = []
         for reply in replies:
             list.append(decode.get_controller_response(reply))
 
         return list
 
-    def get_controller(self, controller):
+    def get_controller(self, controller, dest_addr=None, timeout=2.5):
         '''
         Retrieves the controller information for an access controller.
 
             Parameters:
                controller (uint32)  Controller serial number (expected to be greater than 0).
+               dest_addr  (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout    (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                GetControllerResponse  Response from access controller to the get-controller request.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.get_controller_request(controller)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.get_controller_response(reply)
 
         return None
 
-    def set_ip(self, controller, address, netmask, gateway):
+    def set_ip(self, controller, address, netmask, gateway, dest_addr=None, timeout=2.5):
         '''
         Sets the controller IPv4 address, netmask and gateway address.
 
             Parameters:
                controller (uint32)       Controller serial number (expected to be greater than 0).
                address    (IPv4Address)  Controller IPv4 address.
                netmask    (IPv4Address)  Controller IPv4 subnet mask.
                gateway    (IPv4Address)  Controller IPv4 gateway address.
+               dest_addr  (string)       Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout    (float)        Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                True  For (probably) internal reasons the access controller does not respond to this command.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.set_ip_request(controller, address, netmask, gateway)
-        self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         return True
 
-    def get_time(self, controller):
+    def get_time(self, controller, dest_addr=None, timeout=2.5):
         '''
         Retrieves the access controller current date/time.
 
             Parameters:
                controller (uint32)  Controller serial number (expected to be greater than 0).
+               dest_addr  (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout    (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                GetTimeResponse  Controller current date/time.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.get_time_request(controller)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.get_time_response(reply)
 
         return None
 
-    def set_time(self, controller, datetime):
+    def set_time(self, controller, datetime, dest_addr=None, timeout=2.5):
         '''
         Sets the access controller current date/time.
 
             Parameters:
                controller (uint32)   Controller serial number (expected to be greater than 0).
                datetime   (dateime)  Date/time to set.
+               dest_addr  (string)   Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout    (float)    Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                SetTimeResponse  Controller current date/time.
 
             Raises:
                Exception  If the datetime format cannot be encoded or the response from the 
                           access controller cannot be decoded.
         '''
         request = encode.set_time_request(controller, datetime)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.set_time_response(reply)
 
         return None
 
-    def get_status(self, controller):
+    def get_status(self, controller, dest_addr=None, timeout=2.5):
         '''
         Retrieves the current status of an access controller.
 
             Parameters:
                controller (uint32)  Controller serial number (expected to be greater than 0).
+               dest_addr  (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout    (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                GetStatusResponse  Current controller status.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.get_status_request(controller)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.get_status_response(reply)
 
         return None
 
-    def get_listener(self, controller):
+    def get_listener(self, controller, dest_addr=None, timeout=2.5):
         '''
         Retrieves the configured event listener address:port from an access controller.
 
             Parameters:
                controller (uint32)  Controller serial number (expected to be greater than 0).
+               dest_addr  (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout    (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                GetListenerResponse  Current controller event listener UDP address and port.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.get_listener_request(controller)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.get_listener_response(reply)
 
         return None
 
-    def set_listener(self, controller, address, port):
+    def set_listener(self, controller, address, port, dest_addr=None, timeout=2.5):
         '''
         Sets an access controller event listener IPv4 address and port.
 
             Parameters:
                controller (uint32)       Controller serial number (expected to be greater than 0).
                address    (IPv4Address)  IPv4 address of event listener.
                port       (uint16)       UDP port of event listener.
+               dest_addr  (string)       Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout    (float)        Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                SetListenerResponse  Success/fail response from controller.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.set_listener_request(controller, address, port)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.set_listener_response(reply)
 
         return None
 
-    def get_door_control(self, controller, door):
+    def get_door_control(self, controller, door, dest_addr=None, timeout=2.5):
         '''
         Gets the door delay and control mode for an access controller door.
 
             Parameters:
                controller (uint32)  Controller serial number (expected to be greater than 0).
                door       (uint8)   Door [1..4]
+               dest_addr  (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout    (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                GetDoorControlResponse  Door delay and control mode.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.get_door_control_request(controller, door)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.get_door_control_response(reply)
 
         return None
 
-    def set_door_control(self, controller, door, mode, delay):
+    def set_door_control(self, controller, door, mode, delay, dest_addr=None, timeout=2.5):
         '''
         Sets the door delay and control mode for an access controller door.
 
             Parameters:
                controller (uint32)  Controller serial number (expected to be greater than 0).
                door       (uint8)   Door [1..4]
                mode       (uint8)   Control mode (1: normally open, 2: normally closed, 3: controlled)
                delay      (uint8)   Door unlock duration (seconds)
+               dest_addr  (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout    (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                SetDoorControlResponse  Door delay and control mode.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.set_door_control_request(controller, door, mode, delay)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.set_door_control_response(reply)
 
         return None
 
-    def open_door(self, controller, door):
+    def open_door(self, controller, door, dest_addr=None, timeout=2.5):
         '''
         Remotely opens a door controlled by an access controller.
 
             Parameters:
                controller (uint32)  Controller serial number (expected to be greater than 0).
                door       (uint8)   Door [1..4]
+               dest_addr  (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout    (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                OpenDoorResponse  Door open success/fail response.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.open_door_request(controller, door)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.open_door_response(reply)
 
         return None
 
-    def get_cards(self, controller):
+    def get_cards(self, controller, dest_addr=None, timeout=2.5):
         '''
         Retrieves the number of cards stored in the access controller.
 
             Parameters:
                controller (uint32)  Controller serial number (expected to be greater than 0).
+               dest_addr  (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout    (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                GetCardsResponse  Number of cards stored locally in controller.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.get_cards_request(controller)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.get_cards_response(reply)
 
         return None
 
-    def get_card(self, controller, card_number):
+    def get_card(self, controller, card_number, dest_addr=None, timeout=2.5):
         '''
         Retrieves the card access record for a card number from the access controller.
             Parameters:
                controller  (uint32)  Controller serial number (expected to be greater than 0).
                card_number (uint32)  Access card number.
+               dest_addr   (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout     (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                GetCardResponse  Card information associated with the card number.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.get_card_request(controller, card_number)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.get_card_response(reply)
 
         return None
 
-    def get_card_by_index(self, controller, card_index):
+    def get_card_by_index(self, controller, card_index, dest_addr=None, timeout=2.5):
         '''
         Retrieves the card access record for a card record from the access controller.
             Parameters:
                controller  (uint32)  Controller serial number (expected to be greater than 0).
                index       (uint32)  Controller card list record number.
+               dest_addr   (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout     (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                GetCardByIndexResponse  Card information associated with the card number.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.get_card_by_index_request(controller, card_index)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.get_card_by_index_response(reply)
 
         return None
 
-    def put_card(self, controller, card_number, start_date, end_date, door_1, door_2, door_3, door_4, pin):
+    def put_card(self,
+                 controller,
+                 card_number,
+                 start_date,
+                 end_date,
+                 door_1,
+                 door_2,
+                 door_3,
+                 door_4,
+                 pin,
+                 dest_addr=None,
+                 timeout=2.5):
         '''
         Adds (or updates) a card record stored on the access controller.
             Parameters:
                controller  (uint32)  Controller serial number (expected to be greater than 0).
                card_number (uint32)  Access card number.
                start_date  (date)    Card 'valid from' date (YYYYMMDD).
                end_date    (date)    Card 'valid until' date (YYYYMMDD).
                door_1      (uint8)   Card access permissions for door 1 (0: none, 1: all, 2-254: time profile ID)
                door_2      (uint8)   Card access permissions for door 2 (0: none, 1: all, 2-254: time profile ID)
                door_3      (uint8)   Card access permissions for door 3 (0: none, 1: all, 2-254: time profile ID)
                door_4      (uint8)   Card access permissions for door 4 (0: none, 1: all, 2-254: time profile ID)
                pin         (uint24)  Card access keypad PIN code (0 for none)
+               dest_addr   (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout     (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                PutCardResponse  Card record add/update success/fail.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.put_card_request(controller, card_number, start_date, end_date, door_1, door_2, door_3, door_4,
                                           pin)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.put_card_response(reply)
 
         return None
 
-    def delete_card(self, controller, card_number):
+    def delete_card(self, controller, card_number, dest_addr=None, timeout=2.5):
         '''
         Deletes the card record from the access controller.
             Parameters:
                controller  (uint32)  Controller serial number (expected to be greater than 0).
                card_number (uint32)  Access card number to delete.
+               dest_addr   (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout     (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                DeleteCardResponse  Card record delete success/fail.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.delete_card_request(controller, card_number)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.delete_card_response(reply)
 
         return None
 
-    def delete_all_cards(self, controller):
+    def delete_all_cards(self, controller, dest_addr=None, timeout=2.5):
         '''
         Deletes all card records stored on the access controller.
             Parameters:
                controller  (uint32)  Controller serial number (expected to be greater than 0).
+               dest_addr   (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout     (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                DeleteAllCardsResponse  Clear card records success/fail.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.delete_cards_request(controller)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.delete_all_cards_response(reply)
 
         return None
 
-    def get_event(self, controller, event_index):
+    def get_event(self, controller, event_index, dest_addr=None, timeout=2.5):
         '''
         Retrieves a stored event from the access controller.
             Parameters:
                controller  (uint32)  Controller serial number (expected to be greater than 0).
                event_index (uint32)  Index of event in controller list.
+               dest_addr   (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout     (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                GetEventResponse  Event information.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.get_event_request(controller, event_index)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.get_event_response(reply)
 
         return None
 
-    def get_event_index(self, controller):
+    def get_event_index(self, controller, dest_addr=None, timeout=2.5):
         '''
         Retrieves the 'last downloaded event' index from the controller. The downloaded event index
         is a single utility register on the controller that is managed by an application (not by the
         controller).
 
             Parameters:
                controller  (uint32)  Controller serial number (expected to be greater than 0).
+               dest_addr   (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout     (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                GetEventIndexResponse  Current value of downloaded event index.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.get_event_index_request(controller)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.get_event_index_response(reply)
 
         return None
 
-    def set_event_index(self, controller, event_index):
+    def set_event_index(self, controller, event_index, dest_addr=None, timeout=2.5):
         '''
         Sets the 'last downloaded event' index on the controller. The downloaded event index is a 
         single utility register on the controller that is managed by an application (not by the
         controller).
 
             Parameters:
                controller  (uint32)  Controller serial number (expected to be greater than 0).
                event_index (uitn32)  Event index to which to set the 'downloaded event' index.
+               dest_addr   (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout     (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                SetEventIndexResponse  Set event index success/fail response.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.set_event_index_request(controller, event_index)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.set_event_index_response(reply)
 
         return None
 
-    def record_special_events(self, controller, enable):
+    def record_special_events(self, controller, enable, dest_addr=None, timeout=2.5):
         '''
         Enables or disables door open and close and pushbutton press events.
 
             Parameters:
                controller  (uint32)  Controller serial number (expected to be greater than 0).
                enable      (bool)    Includes door open and close and pushbutton events in the
                                      events stored and broadcast by the controller.
+               dest_addr   (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout     (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                RecordSpecialEventsResponse  Record special events success/fail response.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.record_special_events_request(controller, enable)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.record_special_events_response(reply)
 
         return None
 
-    def get_time_profile(self, controller, profile_id):
+    def get_time_profile(self, controller, profile_id, dest_addr=None, timeout=2.5):
         '''
         Retrieves a time profile from an access conntroller.
 
             Parameters:
                controller  (uint32)  Controller serial number (expected to be greater than 0).
                profile_id  (uint8)   Time profile ID [2..254] to retrieve.
+               dest_addr   (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout     (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                GetTimeProfileResponse  Time profile information for the profile ID.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.get_time_profile_request(controller, profile_id)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.get_time_profile_response(reply)
 
         return None
 
-    def set_time_profile(self, controller, profile_id, start_date, end_date, monday, tuesday, wednesday, thursday,
-                         friday, saturday, sunday, segment_1_start, segment_1_end, segment_2_start, segment_2_end,
-                         segment_3_start, segment_3_end, linked_profile_id):
+    def set_time_profile(self,
+                         controller,
+                         profile_id,
+                         start_date,
+                         end_date,
+                         monday,
+                         tuesday,
+                         wednesday,
+                         thursday,
+                         friday,
+                         saturday,
+                         sunday,
+                         segment_1_start,
+                         segment_1_end,
+                         segment_2_start,
+                         segment_2_end,
+                         segment_3_start,
+                         segment_3_end,
+                         linked_profile_id,
+                         dest_addr=None,
+                         timeout=2.5):
         '''
         Creates (or updates) a time profile on an access conntroller.
 
             Parameters:
                controller        (uint32)  Controller serial number (expected to be greater than 0).
                profile_id        (uint8)   Time profile ID [2..254] to retrieve.
                start_date        (date)    Time profile 'valid from' date.
@@ -535,55 +609,74 @@
                segment_1_start   (time)    Time profile segment 1 start time (HHmm).
                segment_1_end     (time)    Time profile segment 1 end time (HHmm).
                segment_2_start   (time)    Time profile segment 2 start time (HHmm).
                segment_2_end     (time)    Time profile segment 2 end time (HHmm).
                segment_3_start   (time)    Time profile segment 3 start time (HHmm).
                segment_3_end     (time)    Time profile segment 3 end time (HHmm).
                linked_profile_id (uint8)   Next profile ID in chain (0 if none).
- 
+               dest_addr         (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout           (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
+
             Returns:
                SetTimeProfileResponse  Set time profile success/fail response.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.set_time_profile_request(controller, profile_id, start_date, end_date, monday, tuesday,
                                                   wednesday, thursday, friday, saturday, sunday, segment_1_start,
                                                   segment_1_end, segment_2_start, segment_2_end, segment_3_start,
                                                   segment_3_end, linked_profile_id)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.set_time_profile_response(reply)
 
         return None
 
-    def delete_all_time_profiles(self, controller):
+    def delete_all_time_profiles(self, controller, dest_addr=None, timeout=2.5):
         '''
         Clears all time profiles from an access conntroller.
 
             Parameters:
                controller (uint32)  Controller serial number (expected to be greater than 0).
+               dest_addr  (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout    (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                DeleteAllTimeProfilesResponse  Clear time profiles success/fail response.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.delete_all_time_profiles_request(controller)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.delete_all_time_profiles_response(reply)
 
         return None
 
-    def add_task(self, controller, start_date, end_date, monday, tuesday, wednesday, thursday, friday, saturday, sunday,
-                 start_time, door, task_type, more_cards):
+    def add_task(self,
+                 controller,
+                 start_date,
+                 end_date,
+                 monday,
+                 tuesday,
+                 wednesday,
+                 thursday,
+                 friday,
+                 saturday,
+                 sunday,
+                 start_time,
+                 door,
+                 task_type,
+                 more_cards,
+                 dest_addr=None,
+                 timeout=2.5):
         '''
         Creates a scheduled task on an access conntroller.
 
             Parameters:
                controller  (uint32)    Controller serial number (expected to be greater than 0).
                start_date  (datetime)  Task 'valid from' date.
                end_date    (datetime)  Task 'valid until' date.
@@ -607,192 +700,216 @@
                                        7:  card, password
                                        8:  enable 'more cards'
                                        9:  disable 'more cards'
                                        10: trigger once
                                        11: disable pushbutton
                                        12: enable pushbutton
                more_cards  (uint8)     Number of cards for the 'more cards' task.
+               dest_addr   (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout     (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                AddTaskResponse  Add task success/fail response.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.add_task_request(controller, start_date, end_date, monday, tuesday, wednesday, thursday,
                                           friday, saturday, sunday, start_time, door, task_type, more_cards)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.add_task_response(reply)
 
         return None
 
-    def refresh_tasklist(self, controller):
+    def refresh_tasklist(self, controller, dest_addr=None, timeout=2.5):
         '''
         Updates the active tasklist to include tasks added by add_task.
 
             Parameters:
                controller  (uint32)  Controller serial number (expected to be greater than 0).
+               dest_addr   (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout     (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                RefreshTasklistResponse  Refresh tasklist success/fail response.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.refresh_tasklist_request(controller)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.refresh_tasklist_response(reply)
 
         return None
 
-    def clear_tasklist(self, controller):
+    def clear_tasklist(self, controller, dest_addr=None, timeout=2.5):
         '''
         Clears all active and pending tasks.
 
             Parameters:
                controller  (uint32)  Controller serial number (expected to be greater than 0).
+               dest_addr   (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout     (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                ClearTasklistResponse  Clear tasklist success/fail response.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.clear_tasklist_request(controller)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.clear_tasklist_response(reply)
 
         return None
 
-    def set_pc_control(self, controller, enable):
+    def set_pc_control(self, controller, enable, dest_addr=None, timeout=2.5):
         '''
         Defers access control decisions to a remote host. The remote host is expected to 
         interact with the controller at least once every 30 seconds (typically by enabling
         set_pc_control), failing which the access controller will fallback to the internal
         access control list.
 
             Parameters:
                controller  (uint32)  Controller serial number (expected to be greater than 0).
                enable      (bool)    Enables remote control of access.
+               dest_addr   (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout     (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                SetPcControlResponse  Enable PC control success/fail response.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.set_pc_control_request(controller, enable)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.set_pc_control_response(reply)
 
         return None
 
-    def set_interlock(self, controller, interlock):
+    def set_interlock(self, controller, interlock, dest_addr=None, timeout=2.5):
         '''
         Sets the door interlock mode for an access controller.
 
             Parameters:
                controller  (uint32)  Controller serial number (expected to be greater than 0).
                interlock   (uint8)   Door interlock mode:
                                      0:  none
                                      1:  doors 1 and 2 interlocked
                                      2:  doors 2 and 3 interlocked
                                      3:  doors 1 and 2 interlocked, doors 3 and 4 interlocked
                                      4:  doors 1 and 2 and 3 interlocked
                                      8:  doors 1 and 2 and 3 and 4 interlocked
+               dest_addr   (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout     (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                SetInterlockResponse  Set interlock success/fail response.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.set_interlock_request(controller, interlock)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.set_interlock_response(reply)
 
         return None
 
-    def activate_keypads(self, controller, reader1, reader2, reader3, reader4):
+    def activate_keypads(self, controller, reader1, reader2, reader3, reader4, dest_addr=None, timeout=2.5):
         '''
         Enables (or disables) the keypad associated with an access reader.
 
             Parameters:
                controller (uint32)  Controller serial number (expected to be greater than 0).
                reader1    (bool)    Enables/disable reader 1 access keypad
                reader2    (bool)    Enables/disable reader 2 access keypad
                reader3    (bool)    Enables/disable reader 3 access keypad
                reader4    (bool)    Enables/disable reader 4 access keypad
+               dest_addr  (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout    (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                ActivateKeypadsResponse  Activate keypads success/fail response.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.activate_keypads_request(controller, reader1, reader2, reader3, reader4)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.activate_keypads_response(reply)
 
         return None
 
-    def set_door_passcodes(self, controller, door, passcode1, passcode2, passcode3, passcode4):
+    def set_door_passcodes(self,
+                           controller,
+                           door,
+                           passcode1,
+                           passcode2,
+                           passcode3,
+                           passcode4,
+                           dest_addr=None,
+                           timeout=2.5):
         '''
         Sets up to four supervisor passcodes for a door. The passcodes override any other access 
         restrictions and a valid passcode is in the range [0..999999], with 0 corresponding to 
         'no code'.
 
             Parameters:
                controller (uint32)  Controller serial number (expected to be greater than 0).
                door       (uint8)   Door ID [1..4].
                passcode1  (uint32)  Passcode [0..999999].
                passcode2  (uint32)  Passcode [0..999999].
                passcode3  (uint32)  Passcode [0..999999].
                passcode4  (uint32)  Passcode [0..999999].
+               dest_addr  (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout    (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                SetDoorPasscodesResponse  Set door passcodes success/fail response.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.set_door_passcodes_request(controller, door, passcode1, passcode2, passcode3, passcode4)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.set_door_passcodes_response(reply)
 
         return None
 
-    def restore_default_parameters(self, controller):
+    def restore_default_parameters(self, controller, dest_addr=None, timeout=2.5):
         '''
         Resets a controller to the manufacturer default configuration.
             Parameters:
                controller  (uint32)  Controller serial number (expected to be greater than 0).
+               dest_addr   (string)  Optional controller IPv4 addess:port. Defaults to broadcast address and port 60000.
+               timeout     (float)   Optional operation timeout (in seconds). Defaults to 2.5s.
 
             Returns:
                RestoreDefaultParametersResponse  Reset success/fail.
 
             Raises:
                Exception  If the response from the access controller cannot be decoded.
         '''
         request = encode.restore_default_parameters_request(controller)
-        reply = self._udp.send(request)
+        reply = self._udp.send(request, dest_addr=dest_addr, timeout=timeout)
 
         if reply != None:
             return decode.restore_default_parameters_response(reply)
 
         return None
 
     def listen(self, onEvent):
```

### Comparing `uhppoted-0.8.8/src/uhppoted.egg-info/PKG-INFO` & `uhppoted-0.8.8.1/src/uhppoted.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uhppoted
-Version: 0.8.8
+Version: 0.8.8.1
 Summary: Python API for the UHPPOTE TCP/IP access controllers
 Author-email: uhppoted <uhppoted.development@gmail.com>
 Project-URL: Homepage, https://github.com/uhppoted/uhppoted-python
 Project-URL: Bug Tracker, https://github.com/uhppoted/uhppoted-python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -97,15 +97,26 @@
   'gateway': IPv4Address('192.168.1.1'),
   'ip_address': IPv4Address('192.168.1.100'),
   'mac_address': '00:12:23:34::45:56',
   'subnet_mask': IPv4Address('255.255.255.0'),
   'version': 'v8.92'}
 ```
 
-All API functions raise an `Exception` if the call fails for any reason whatsoever.
+### Notes
+1. All API functions raise an `Exception` if the call fails for any reason whatsoever.
+2. All API functions (other than `get_controllers` and `listen`) take an optional `dest_addr` kwarg that sets the
+   IP address to which to send the request, e.g.:
+```
+   get_controller(controller, dest_addr='192.168.1.100:60000')
+```
+3. All API functions (other than `listen`) take an optional `timeout` kwarg that sets the time limit for the 
+   request (in seconds), e.g.:
+```
+   get_controller(controller, dest_addr='192.168.1.100:60000', timeout=0.75)
+```
 
 ### `get_controllers`
 ```
 get_controllers()
 
 Returns an array of `GetControllerResponse`.
 
@@ -459,14 +470,35 @@
 
 ID  uint32  controller serial number 
 
 
 Raises an Exception if the call failed for any reason.
 ```
 
+### `listen`
+```
+listen(handler)
+
+handler  event handling callback function of the form
+         def on_event(event):
+              ...
+
+Raises an Exception if the call failed for any reason.
+```
+
+`listen` is a blocking call that will invoke the `handler` function for each received event, e.g.:
+```
+    ...
+    u.listen(on_event)
+
+def on_event(event):
+    if event != None:
+        pprint(event.__dict__, indent=2, width=1)
+    ...
+```
 
 ## Types
 
 ### `GetControllerResponse`
 
 Container class for the decoded response from a get-controller request.
```

