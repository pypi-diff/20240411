# Comparing `tmp/gewu-2.3.2.tar.gz` & `tmp/gewu-2.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gewu-2.3.2.tar", last modified: Fri Mar 15 08:12:11 2024, max compression
+gzip compressed data, was "gewu-2.3.3.tar", last modified: Thu Apr 11 03:11:49 2024, max compression
```

## Comparing `gewu-2.3.2.tar` & `gewu-2.3.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2024-03-15 08:12:11.207428 gewu-2.3.2/
--rw-rw-rw-   0        0        0     1093 2024-01-17 07:33:18.000000 gewu-2.3.2/LICENSE
--rw-rw-rw-   0        0        0      500 2024-03-15 08:12:11.206467 gewu-2.3.2/PKG-INFO
--rw-rw-rw-   0        0        0      609 2024-03-15 08:07:15.000000 gewu-2.3.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2024-03-15 08:12:11.207428 gewu-2.3.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2024-03-15 08:12:11.171837 gewu-2.3.2/src/
-drwxrwxrwx   0        0        0        0 2024-03-15 08:12:11.184073 gewu-2.3.2/src/gewu/
--rw-rw-rw-   0        0        0       18 2024-01-19 06:39:27.000000 gewu-2.3.2/src/gewu/__init__.py
--rw-rw-rw-   0        0        0    31936 2024-03-15 08:01:23.000000 gewu-2.3.2/src/gewu/gewu.py
-drwxrwxrwx   0        0        0        0 2024-03-15 08:12:11.205432 gewu-2.3.2/src/gewu.egg-info/
--rw-rw-rw-   0        0        0      500 2024-03-15 08:12:11.000000 gewu-2.3.2/src/gewu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      188 2024-03-15 08:12:11.000000 gewu-2.3.2/src/gewu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2024-03-15 08:12:11.000000 gewu-2.3.2/src/gewu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        5 2024-03-15 08:12:11.000000 gewu-2.3.2/src/gewu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 03:11:49.017826 gewu-2.3.3/
+-rw-rw-rw-   0        0        0     1093 2024-01-17 07:33:18.000000 gewu-2.3.3/LICENSE
+-rw-rw-rw-   0        0        0      500 2024-04-11 03:11:49.017826 gewu-2.3.3/PKG-INFO
+-rw-rw-rw-   0        0        0      609 2024-04-11 03:10:33.000000 gewu-2.3.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2024-04-11 03:11:49.018865 gewu-2.3.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2024-04-11 03:11:48.991445 gewu-2.3.3/src/
+drwxrwxrwx   0        0        0        0 2024-04-11 03:11:49.000636 gewu-2.3.3/src/gewu/
+-rw-rw-rw-   0        0        0       18 2024-01-19 06:39:27.000000 gewu-2.3.3/src/gewu/__init__.py
+-rw-rw-rw-   0        0        0    35289 2024-04-11 03:07:56.000000 gewu-2.3.3/src/gewu/gewu.py
+drwxrwxrwx   0        0        0        0 2024-04-11 03:11:49.015766 gewu-2.3.3/src/gewu.egg-info/
+-rw-rw-rw-   0        0        0      500 2024-04-11 03:11:48.000000 gewu-2.3.3/src/gewu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      188 2024-04-11 03:11:48.000000 gewu-2.3.3/src/gewu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 03:11:48.000000 gewu-2.3.3/src/gewu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        5 2024-04-11 03:11:48.000000 gewu-2.3.3/src/gewu.egg-info/top_level.txt
```

### Comparing `gewu-2.3.2/LICENSE` & `gewu-2.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `gewu-2.3.2/pyproject.toml` & `gewu-2.3.3/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "gewu"
-version = "2.3.2"
+version = "2.3.3"
 authors = [
   { name = "xiaoheli", email = "1173324325@qq.com" },
 ]
 dependencies = []
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.8"
```

### Comparing `gewu-2.3.2/src/gewu/gewu.py` & `gewu-2.3.3/src/gewu/gewu.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,20 @@
 '''
+# 1.2.5
+* 优化串口模式STOP的时候停止码盘电机
+
+# 1.2.4
+* 修改串口的函数，防止混淆
+
+# 1.2.3
+* 优化蓝牙连接不显示的问题
+
+# 1.2.1
+* 增加CAR模式
+
 # 1.2.0
 * 优化蓝牙下的停止问题
 
 # 1.1.8
 * 修正电机的run函数
 
 # 1.1.7
@@ -115,22 +127,23 @@
 acc_y = 0
 acc_z = 0
 
 dist_result = bytearray(4) #存储4个端口的超声波数据
 color_result = bytearray(16) #[result,r,g,b]
 motor_result = [0] * 20 #[state,car,power,speed,count]
 motor_result_flag = 0
+car_status = 0
 
 ble_connect_flag = 0
 com_connect_flag = 0
 
 ble_Client = 0
-ble_queue = queue.Queue(256)
+ble_queue = queue.Queue(512)
 
-def get_serialport():
+def _get_serialport():
     # 获取所有串口设备实例。
     # 如果没找到串口设备，则输出：“无串口设备。”
     # 如果找到串口设备，则依次输出每个设备对应的串口号和描述信息。
     ports_list = list(serial.tools.list_ports.comports())
     gewu_port = ""
     if len(ports_list) <= 0:
         print("无串口设备")
@@ -148,16 +161,16 @@
                 gewu_port = list(comport)[0]
     if gewu_port !="":
         #print("Gewu Serial:" + gewu_port)
         return gewu_port
     else:
         return None
 
-def open_serial_port():
-    gewu_port = get_serialport()
+def _open_serial_port():
+    gewu_port = _get_serialport()
     if gewu_port == None:
         print("搜索串口设备失败")
         print("请检查usb线是否已经连接上设备。")
         return None
     try:
         ser = serial.Serial(gewu_port, 115200)    # 打开COM17，将波特率配置为115200，其余参数使用默认值
     except Exception as e:
@@ -231,15 +244,15 @@
             return True
         else:
             print('crc error')
     return False
 
 def recv_data_handler(data):
     global btn_a_state,btn_b_state,mic_value,pin_2_input,light_value,acc_x,acc_y,acc_z,pin_1_input,dist_result,color_result,motor_result
-    global motor_result_flag
+    global motor_result_flag,car_status
     for ch in data:
         if recv_parse(ch) == True:
             cmd = readCmd()
             if cmd == 0x01: #广播数据
                 [state] = readBytes(1, 0)
                 [btn] = readBytes(1, 1)
                 #print(btn)
@@ -266,14 +279,15 @@
                     color_result[4*p+1] = b
                     color_result[4*p+2] = c
                     color_result[4*p+3] = d
             elif cmd == 0x08: #电机参数
                     [p] = readBytes(1, 0) #端口
                     p = p - 0xE9
                     [motor_state] = readBytes(1, 1)
+                    [car_status] = readBytes(1, 2)
                     [deg1,deg2,deg3,deg4] = readBytes(4, 7)
                     deg = deg1 | (deg2<<8) |(deg3<<16)|(deg4<<24)
                     motor_result[5*p] = motor_state
                     if deg > 2147483647:
                         motor_result[5*p+4] = 4294967295 - deg
                     else:
                         motor_result[5*p+4] = deg
@@ -757,18 +771,117 @@
             time.sleep(0.01)
             count = count + 1
             if count > 500:
                 #print('error01 time out')
                 break
         return motor_result[5*(self.port -0xe0 - 9)+4]
 
+class CarMode:
+    def set_state(self,state_str):
+        _data = bytearray(3)
+        _data[0] = 8
+        state = 0
+        if state_str == "top":
+            state = 1
+        elif state_str == "bottom":
+            state = 2
+        elif state_str == "left":
+            state = 3
+        elif state_str == "right":
+            state = 4
+        elif state_str == "front":
+            state = 5   
+        elif state_str == "opposite":
+            state = 6
+        _data[1] = state
+        pack_send_data(0x0B, bytearray(_data), 2)
+        time.sleep(0.02)
+        
+    def set_port(self,left,right):
+        _data = bytearray(3)
+        _data[0] = 6
+        _data[1] = 0xE0+left
+        _data[2] = 0xE0+right
+        pack_send_data(0x0B, bytearray(_data), 3)
+        time.sleep(0.02)
+        
+    def run (self,speed):
+        _data = bytearray(5)
+        _data[0] = 0x0A
+        _data[1] = speed&0xff
+        _data[2] = (speed>>8)&0xff
+        _data[3] = speed&0xff
+        _data[4] = (speed>>8)&0xff
+        pack_send_data(0x0B, bytearray(_data), 5) 
+        time.sleep(0.02)
+        
+    def stop(self):
+        _data = bytearray(2)
+        _data[0] = 4
+        _data[1] = 0
+        pack_send_data(0x0B, bytearray(_data), 2)
+        time.sleep(0.02)
+    
+    def turn_left(self,degree):
+        global car_status
+        d=int(degree)*-1
+        print(d)
+        _data = bytearray(3)
+        _data[0] = 2
+        _data[1] = (d)&0xff
+        _data[2] = ((d)>>8)&0xff
+        print(_data[1])
+        print(_data[2])
+        pack_send_data(0x0B, bytearray(_data), 3)
+        time.sleep(0.02)
+        car_status = 1
+        while True:
+            print("### "+ str(car_status))
+            if car_status == 0:
+                self.stop()
+                break
+            self.getMotorStatus()
+            time.sleep(0.1)
+
+    def turn_right(self,degree):
+        global car_status
+        d=int(degree)
+        _data = bytearray(3)
+        _data[0] = 2
+        _data[1] = (d)&0xff
+        _data[2] = ((d)>>8)&0xff
+        pack_send_data(0x0B, bytearray(_data), 3)
+        time.sleep(0.02)
+        car_status = 1
+        while True:
+            print("### "+ str(car_status))
+            if car_status == 0:
+                self.stop()
+                break
+            self.getMotorStatus()
+            time.sleep(0.1)
+        
+    def getMotorStatus(self):
+        # _data = bytearray(1)
+        # _data[0] = 0x0E
+        # pack_send_data(0x0B, bytearray(_data), 1)
+        # time.sleep(0.1)
+        _data = bytearray(3)
+        _data[0] = 7
+        _data[1] = 0xE9
+        _data[2] = 0x00
+        pack_send_data(0x0A, bytearray(_data), 3)
+        time.sleep(0.1)
+        
 class Timer():
     def get_time(self):
         pass
 
+car_mode = CarMode()
+
 button = Button()
 lcd = OLED()
 
 p1 = Pin(1)
 p2 = Pin(2)
 
 class _ir_sensor:
@@ -832,15 +945,15 @@
 
 # print(hex2str(0x05))
 # print(hex2str(0x0F))
 port = 0
 port_th = 0
 def open_gewu_port():
     global port,ble_connect_flag,com_connect_flag,port_th
-    port = open_serial_port()
+    port = _open_serial_port()
     if port == 0  or port == None:
         print("退出")
         quit()
     port_th = Thread(target=recv_serial_handler,args=(port,))
     port_th.start()
     ble_connect_flag = 0
     com_connect_flag = 1
@@ -888,31 +1001,33 @@
             #print(f"Connected: {client.is_connected}")
             ble_Client = client
             # 是否配对
             # paired = await client.pair(protection_level=1)
             #print(f"Paired: {paired}")
             
             # if paired:
-            ble_connect_flag = 1
+            
             # 开启通知的接收
             #print('w')
             
             await client.start_notify(SERVICE_NOTIFY_UUID, notify_callback)
             #print('e')
             await client.write_gatt_char(SERVICE_WRITE_UUID, chr(0x03).encode("utf-8"))
-            await asyncio.sleep(0.01)
+            await asyncio.sleep(0.1)
             await client.write_gatt_char(SERVICE_WRITE_UUID, chr(0x06).encode("utf-8"))
-            await asyncio.sleep(0.01)
+            await asyncio.sleep(0.1)
             #ble_queue.put(0x03)
             #time.sleep_ms(1)
             #ble_queue.put(0x03)
             #time.sleep_ms(1)
             #ble_queue.put(0x06)
             #time.sleep_ms(1)
             print("蓝牙连接成功!")
+            await asyncio.sleep(0.1)
+            ble_connect_flag = 1
             # lcd.clear()
             # lcd.icon(0,0,"yeah")
             # lcd.show()
 
             # n = ble_queue.qsize()
             # watchData = []
             # openDoor_send = [0x68, 0x06, 0x01]
@@ -934,15 +1049,15 @@
                         for i in range(n):
                             watchData.append(ble_queue.get())
                         await client.write_gatt_char(SERVICE_WRITE_UUID,bytes(watchData),response=False)
                     except:
                         pass
                     finally:
                         pass
-                await asyncio.sleep(0.1)
+                await asyncio.sleep(0.02)
                 if ble_connect_flag == 0:
                     await client.write_gatt_char(SERVICE_WRITE_UUID, chr(0x03).encode("utf-8"))
                     await asyncio.sleep(0.01)
                     await client.write_gatt_char(SERVICE_WRITE_UUID, chr(0x06).encode("utf-8"))
                     await asyncio.sleep(0.01)
                     await client.unpair()
                     await client.disconnect()
@@ -1007,25 +1122,28 @@
     th = Thread(target=ble_service,args=(address,))
     th.start()
     com_connect_flag = 0
     #write_config(address)
     while True:
         time.sleep(0.1)
         if ble_connect_flag == 1:
+            time.sleep(0.1)
             break
         
 def open_gewu_ble_name(name):
     global com_connect_flag,ble_connect_flag
+    ble_connect_flag = 0
     th = Thread(target=ble_service,args=(name,))
     th.start()
     com_connect_flag = 0
     #write_config(address)
     while True:
         time.sleep(0.1)
         if ble_connect_flag == 1:
+            time.sleep(2)
             break
 
 def stop_gewu():#停止硬件运行，用于软件点击停止时调用
     global com_connect_flag,ble_connect_flag
     if ble_connect_flag == 0 and com_connect_flag == 0:
         #s = read_config()
         # if len(s) == 0:
@@ -1036,14 +1154,17 @@
         #     open_gewu_ble(s)
         return
     _data = bytearray(1)
     _data[0] = 2
     pack_send_data(0x00, bytearray(_data), 1)
     time.sleep(0.1)
     if com_connect_flag == 1:
+        port.write(chr(0x03).encode("utf-8"))
+        port.write(chr(0x06).encode("utf-8")) #进入在线模式
+        time.sleep(0.1)
         port.close()
         com_connect_flag = 0
         print('############################')
     if ble_connect_flag == 1:
         ble_connect_flag = 0
     time.sleep(1)
```

