# Comparing `tmp/opentakserver-1.1.1.tar.gz` & `tmp/opentakserver-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "opentakserver-1.1.1.tar", max compression
+gzip compressed data, was "opentakserver-1.1.2.tar", max compression
```

## Comparing `opentakserver-1.1.1.tar` & `opentakserver-1.1.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
--rw-r--r--   0        0        0    35803 2023-11-29 17:24:22.234248 opentakserver-1.1.1/LICENSE
--rw-r--r--   0        0        0      128 2024-04-04 21:44:21.774113 opentakserver-1.1.1/opentakserver/__init__.py
--rw-r--r--   0        0        0    10612 2024-04-03 23:02:30.004021 opentakserver-1.1.1/opentakserver/app.py
--rw-r--r--   0        0        0        0 2023-12-13 18:19:32.000000 opentakserver-1.1.1/opentakserver/blueprints/__init__.py
--rw-r--r--   0        0        0    41916 2024-04-04 21:36:33.553055 opentakserver-1.1.1/opentakserver/blueprints/api.py
--rw-r--r--   0        0        0     5061 2024-02-08 04:58:11.564334 opentakserver-1.1.1/opentakserver/blueprints/config.py
--rw-r--r--   0        0        0    26182 2024-04-04 14:24:20.109147 opentakserver-1.1.1/opentakserver/blueprints/marti.py
--rw-r--r--   0        0        0      935 2024-01-19 16:14:22.948256 opentakserver-1.1.1/opentakserver/blueprints/ots_socketio.py
--rw-r--r--   0        0        0     4588 2024-02-29 22:51:03.042964 opentakserver-1.1.1/opentakserver/blueprints/scheduled_jobs.py
--rw-r--r--   0        0        0     3709 2024-02-07 20:21:41.027299 opentakserver-1.1.1/opentakserver/blueprints/scheduler_api.py
--rw-r--r--   0        0        0     3378 2024-01-03 04:37:35.139149 opentakserver-1.1.1/opentakserver/ca_config.py
--rw-r--r--   0        0        0    22887 2024-04-04 13:23:59.284952 opentakserver-1.1.1/opentakserver/certificate_authority.py
--rw-r--r--   0        0        0        0 2023-11-30 13:57:03.000000 opentakserver-1.1.1/opentakserver/controllers/__init__.py
--rw-r--r--   0        0        0    10565 2024-04-03 18:07:25.951570 opentakserver-1.1.1/opentakserver/controllers/client_controller.py
--rw-r--r--   0        0        0    34898 2024-04-03 23:05:12.049517 opentakserver-1.1.1/opentakserver/controllers/cot_controller.py
--rw-r--r--   0        0        0     3983 2024-03-22 03:19:30.991223 opentakserver-1.1.1/opentakserver/defaultconfig.py
--rw-r--r--   0        0        0     1719 2024-03-29 15:46:06.381933 opentakserver-1.1.1/opentakserver/EmailValidator.py
--rw-r--r--   0        0        0      430 2024-03-22 02:45:11.460029 opentakserver-1.1.1/opentakserver/extensions.py
--rw-r--r--   0        0        0        0 2024-01-12 18:16:59.724301 opentakserver-1.1.1/opentakserver/forms/__init__.py
--rw-r--r--   0        0        0     2538 2024-01-12 19:32:55.799523 opentakserver-1.1.1/opentakserver/forms/MediaMTXGlobalConfig.py
--rw-r--r--   0        0        0     3237 2024-02-08 20:10:17.606065 opentakserver-1.1.1/opentakserver/forms/MediaMTXPathConfig.py
--rw-r--r--   0        0        0      498 2024-01-25 04:20:43.892847 opentakserver-1.1.1/opentakserver/functions.py
--rw-r--r--   0        0        0        0 2023-11-30 04:49:58.000000 opentakserver-1.1.1/opentakserver/models/__init__.py
--rw-r--r--   0        0        0     1926 2024-01-25 04:33:33.722411 opentakserver-1.1.1/opentakserver/models/Alert.py
--rw-r--r--   0        0        0       88 2023-12-12 03:59:25.000000 opentakserver-1.1.1/opentakserver/models/Base.py
--rw-r--r--   0        0        0     8027 2024-03-27 16:18:27.050188 opentakserver-1.1.1/opentakserver/models/CasEvac.py
--rw-r--r--   0        0        0     2551 2024-04-03 18:26:30.129258 opentakserver-1.1.1/opentakserver/models/Certificate.py
--rw-r--r--   0        0        0     1075 2024-01-25 16:53:37.654426 opentakserver-1.1.1/opentakserver/models/Chatrooms.py
--rw-r--r--   0        0        0      534 2024-01-25 04:24:24.905475 opentakserver-1.1.1/opentakserver/models/ChatroomsUids.py
--rw-r--r--   0        0        0      356 2024-02-07 04:30:20.062715 opentakserver-1.1.1/opentakserver/models/Config.py
--rw-r--r--   0        0        0     2812 2024-01-30 17:15:18.630584 opentakserver-1.1.1/opentakserver/models/CoT.py
--rw-r--r--   0        0        0     2378 2024-03-20 14:43:29.949183 opentakserver-1.1.1/opentakserver/models/DataPackage.py
--rw-r--r--   0        0        0     3716 2024-04-02 22:43:21.454953 opentakserver-1.1.1/opentakserver/models/EUD.py
--rw-r--r--   0        0        0     1422 2024-01-25 16:58:20.832045 opentakserver-1.1.1/opentakserver/models/GeoChat.py
--rw-r--r--   0        0        0     1462 2024-01-25 03:55:46.133780 opentakserver-1.1.1/opentakserver/models/Icon.py
--rw-r--r--   0        0        0     4050 2024-01-30 17:15:19.234690 opentakserver-1.1.1/opentakserver/models/Marker.py
--rw-r--r--   0        0        0     3193 2024-03-07 14:42:01.426952 opentakserver-1.1.1/opentakserver/models/Point.py
--rw-r--r--   0        0        0     4637 2024-02-03 20:36:12.354511 opentakserver-1.1.1/opentakserver/models/RBLine.py
--rw-r--r--   0        0        0      416 2024-01-15 18:18:51.545174 opentakserver-1.1.1/opentakserver/models/role.py
--rw-r--r--   0        0        0     1394 2024-01-25 18:50:18.903032 opentakserver-1.1.1/opentakserver/models/Team.py
--rw-r--r--   0        0        0     1227 2024-04-03 18:26:30.115290 opentakserver-1.1.1/opentakserver/models/user.py
--rw-r--r--   0        0        0     2626 2024-01-31 03:55:59.748405 opentakserver-1.1.1/opentakserver/models/VideoRecording.py
--rw-r--r--   0        0        0     5476 2024-03-08 05:21:32.683056 opentakserver-1.1.1/opentakserver/models/VideoStream.py
--rw-r--r--   0        0        0      158 2024-03-22 03:00:06.153840 opentakserver-1.1.1/opentakserver/models/WebAuthn.py
--rw-r--r--   0        0        0     1146 2024-01-25 03:55:46.149750 opentakserver-1.1.1/opentakserver/models/ZMIST.py
--rw-r--r--   0        0        0        0 2024-02-02 04:47:28.610655 opentakserver-1.1.1/opentakserver/mumble/__init__.py
--rw-r--r--   0        0        0     3207 2024-02-29 18:19:41.795118 opentakserver-1.1.1/opentakserver/mumble/mumble_authenticator.py
--rw-r--r--   0        0        0     6448 2024-02-29 18:19:41.787175 opentakserver-1.1.1/opentakserver/mumble/mumble_ice_app.py
--rw-r--r--   0        0        0    39926 2024-02-02 04:47:28.610655 opentakserver-1.1.1/opentakserver/mumble/Murmur.ice
--rw-r--r--   0        0        0     3444 2024-03-21 14:16:06.218434 opentakserver-1.1.1/opentakserver/SocketServer.py
--rw-r--r--   0        0        0     1739 2024-04-04 21:44:21.765184 opentakserver-1.1.1/pyproject.toml
--rw-r--r--   0        0        0     1647 2024-02-02 04:47:28.605667 opentakserver-1.1.1/README.md
--rw-r--r--   0        0        0     3506 1970-01-01 00:00:00.000000 opentakserver-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0    35803 2023-11-29 17:24:22.234248 opentakserver-1.1.2/LICENSE
+-rw-r--r--   0        0        0      128 2024-04-11 18:09:49.558470 opentakserver-1.1.2/opentakserver/__init__.py
+-rw-r--r--   0        0        0    10612 2024-04-11 02:48:47.117926 opentakserver-1.1.2/opentakserver/app.py
+-rw-r--r--   0        0        0        0 2023-12-13 18:19:32.000000 opentakserver-1.1.2/opentakserver/blueprints/__init__.py
+-rw-r--r--   0        0        0    46717 2024-04-11 18:07:13.514520 opentakserver-1.1.2/opentakserver/blueprints/api.py
+-rw-r--r--   0        0        0     5061 2024-02-08 04:58:11.564334 opentakserver-1.1.2/opentakserver/blueprints/config.py
+-rw-r--r--   0        0        0    26182 2024-04-04 14:24:20.109147 opentakserver-1.1.2/opentakserver/blueprints/marti.py
+-rw-r--r--   0        0        0      935 2024-01-19 16:14:22.948256 opentakserver-1.1.2/opentakserver/blueprints/ots_socketio.py
+-rw-r--r--   0        0        0     4588 2024-04-11 02:49:02.199161 opentakserver-1.1.2/opentakserver/blueprints/scheduled_jobs.py
+-rw-r--r--   0        0        0     3709 2024-02-07 20:21:41.027299 opentakserver-1.1.2/opentakserver/blueprints/scheduler_api.py
+-rw-r--r--   0        0        0     3378 2024-01-03 04:37:35.139149 opentakserver-1.1.2/opentakserver/ca_config.py
+-rw-r--r--   0        0        0    22887 2024-04-04 13:23:59.284952 opentakserver-1.1.2/opentakserver/certificate_authority.py
+-rw-r--r--   0        0        0        0 2023-11-30 13:57:03.000000 opentakserver-1.1.2/opentakserver/controllers/__init__.py
+-rw-r--r--   0        0        0    10712 2024-04-11 02:48:20.040469 opentakserver-1.1.2/opentakserver/controllers/client_controller.py
+-rw-r--r--   0        0        0    34898 2024-04-11 02:48:54.783881 opentakserver-1.1.2/opentakserver/controllers/cot_controller.py
+-rw-r--r--   0        0        0     3983 2024-03-22 03:19:30.991223 opentakserver-1.1.2/opentakserver/defaultconfig.py
+-rw-r--r--   0        0        0     1719 2024-03-29 15:46:06.381933 opentakserver-1.1.2/opentakserver/EmailValidator.py
+-rw-r--r--   0        0        0      430 2024-03-22 02:45:11.460029 opentakserver-1.1.2/opentakserver/extensions.py
+-rw-r--r--   0        0        0        0 2024-01-12 18:16:59.724301 opentakserver-1.1.2/opentakserver/forms/__init__.py
+-rw-r--r--   0        0        0     2538 2024-01-12 19:32:55.799523 opentakserver-1.1.2/opentakserver/forms/MediaMTXGlobalConfig.py
+-rw-r--r--   0        0        0     3237 2024-02-08 20:10:17.606065 opentakserver-1.1.2/opentakserver/forms/MediaMTXPathConfig.py
+-rw-r--r--   0        0        0      498 2024-01-25 04:20:43.892847 opentakserver-1.1.2/opentakserver/functions.py
+-rw-r--r--   0        0        0        0 2023-11-30 04:49:58.000000 opentakserver-1.1.2/opentakserver/models/__init__.py
+-rw-r--r--   0        0        0     1926 2024-01-25 04:33:33.722411 opentakserver-1.1.2/opentakserver/models/Alert.py
+-rw-r--r--   0        0        0       88 2023-12-12 03:59:25.000000 opentakserver-1.1.2/opentakserver/models/Base.py
+-rw-r--r--   0        0        0     8027 2024-03-27 16:18:27.050188 opentakserver-1.1.2/opentakserver/models/CasEvac.py
+-rw-r--r--   0        0        0     2551 2024-04-03 18:26:30.129258 opentakserver-1.1.2/opentakserver/models/Certificate.py
+-rw-r--r--   0        0        0     1075 2024-01-25 16:53:37.654426 opentakserver-1.1.2/opentakserver/models/Chatrooms.py
+-rw-r--r--   0        0        0      534 2024-01-25 04:24:24.905475 opentakserver-1.1.2/opentakserver/models/ChatroomsUids.py
+-rw-r--r--   0        0        0      356 2024-02-07 04:30:20.062715 opentakserver-1.1.2/opentakserver/models/Config.py
+-rw-r--r--   0        0        0     2812 2024-01-30 17:15:18.630584 opentakserver-1.1.2/opentakserver/models/CoT.py
+-rw-r--r--   0        0        0     2378 2024-03-20 14:43:29.949183 opentakserver-1.1.2/opentakserver/models/DataPackage.py
+-rw-r--r--   0        0        0     3716 2024-04-02 22:43:21.454953 opentakserver-1.1.2/opentakserver/models/EUD.py
+-rw-r--r--   0        0        0     1422 2024-01-25 16:58:20.832045 opentakserver-1.1.2/opentakserver/models/GeoChat.py
+-rw-r--r--   0        0        0     1462 2024-01-25 03:55:46.133780 opentakserver-1.1.2/opentakserver/models/Icon.py
+-rw-r--r--   0        0        0     4050 2024-01-30 17:15:19.234690 opentakserver-1.1.2/opentakserver/models/Marker.py
+-rw-r--r--   0        0        0     3193 2024-03-07 14:42:01.426952 opentakserver-1.1.2/opentakserver/models/Point.py
+-rw-r--r--   0        0        0     4637 2024-02-03 20:36:12.354511 opentakserver-1.1.2/opentakserver/models/RBLine.py
+-rw-r--r--   0        0        0      416 2024-01-15 18:18:51.545174 opentakserver-1.1.2/opentakserver/models/role.py
+-rw-r--r--   0        0        0     1394 2024-01-25 18:50:18.903032 opentakserver-1.1.2/opentakserver/models/Team.py
+-rw-r--r--   0        0        0     1227 2024-04-03 18:26:30.115290 opentakserver-1.1.2/opentakserver/models/user.py
+-rw-r--r--   0        0        0     2626 2024-01-31 03:55:59.748405 opentakserver-1.1.2/opentakserver/models/VideoRecording.py
+-rw-r--r--   0        0        0     5476 2024-03-08 05:21:32.683056 opentakserver-1.1.2/opentakserver/models/VideoStream.py
+-rw-r--r--   0        0        0      158 2024-03-22 03:00:06.153840 opentakserver-1.1.2/opentakserver/models/WebAuthn.py
+-rw-r--r--   0        0        0     1146 2024-01-25 03:55:46.149750 opentakserver-1.1.2/opentakserver/models/ZMIST.py
+-rw-r--r--   0        0        0        0 2024-02-02 04:47:28.610655 opentakserver-1.1.2/opentakserver/mumble/__init__.py
+-rw-r--r--   0        0        0     3207 2024-02-29 18:19:41.795118 opentakserver-1.1.2/opentakserver/mumble/mumble_authenticator.py
+-rw-r--r--   0        0        0     6448 2024-02-29 18:19:41.787175 opentakserver-1.1.2/opentakserver/mumble/mumble_ice_app.py
+-rw-r--r--   0        0        0    39926 2024-02-02 04:47:28.610655 opentakserver-1.1.2/opentakserver/mumble/Murmur.ice
+-rw-r--r--   0        0        0     3527 2024-04-10 20:27:14.987143 opentakserver-1.1.2/opentakserver/SocketServer.py
+-rw-r--r--   0        0        0     1739 2024-04-11 18:09:49.548458 opentakserver-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1647 2024-02-02 04:47:28.605667 opentakserver-1.1.2/README.md
+-rw-r--r--   0        0        0     3506 1970-01-01 00:00:00.000000 opentakserver-1.1.2/PKG-INFO
```

### Comparing `opentakserver-1.1.1/LICENSE` & `opentakserver-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/app.py` & `opentakserver-1.1.2/opentakserver/app.py`

 * *Files 1% similar despite different names*

```diff
@@ -78,15 +78,15 @@
 
     cors = CORS(app, resources={r"/api/*": {"origins": "*"}, r"/Marti/*": {"origins": "*"}, r"/*": {"origins": "*"}},
                 supports_credentials=True)
     flask_wtf.CSRFProtect(app)
 
     socketio.init_app(app, logger=logger)
 
-    rabbit_connection = pika.BlockingConnection(pika.ConnectionParameters('localhost'))
+    rabbit_connection = pika.BlockingConnection(pika.ConnectionParameters('127.0.0.1'))
     channel = rabbit_connection.channel()
     channel.exchange_declare('cot', durable=True, exchange_type='fanout')
     channel.exchange_declare('dms', durable=True, exchange_type='direct')
     channel.exchange_declare('chatrooms', durable=True, exchange_type='direct')
     channel.queue_declare(queue='cot_controller')
     channel.exchange_declare(exchange='cot_controller', exchange_type='fanout')
```

### Comparing `opentakserver-1.1.1/opentakserver/blueprints/api.py` & `opentakserver-1.1.2/opentakserver/blueprints/api.py`

 * *Files 4% similar despite different names*

```diff
@@ -214,38 +214,41 @@
 
 @api_blueprint.route("/api/certificate", methods=['GET', 'POST'])
 @auth_required()
 def certificate():
     if request.method == 'POST' and 'username' in request.json.keys():
         try:
             username = bleach.clean(request.json.get('username'))
-            truststore_filename = os.path.join(app.config.get("OTS_CA_FOLDER"), 'certs', "opentakserver", "truststore-root.p12")
+            truststore_filename = os.path.join(app.config.get("OTS_CA_FOLDER"), 'certs', "opentakserver",
+                                               "truststore-root.p12")
             user_filename = os.path.join(app.config.get("OTS_CA_FOLDER"), 'certs', username,
                                          "{}.p12".format(username))
 
             user = app.security.datastore.find_user(username=username)
 
             if not user:
                 return ({'success': False, 'error': 'Invalid username: {}'.format(username)}, 400,
                         {'Content-Type': 'application/json'})
 
             ca = CertificateAuthority(logger, app)
             filenames = ca.issue_certificate(username, False)
 
             for filename in filenames:
                 file_hash = hashlib.sha256(
-                    open(os.path.join(app.config.get("OTS_CA_FOLDER"), 'certs', username, filename),'rb').read()).hexdigest()
+                    open(os.path.join(app.config.get("OTS_CA_FOLDER"), 'certs', username, filename),
+                         'rb').read()).hexdigest()
 
                 data_package = DataPackage()
                 data_package.filename = filename
                 data_package.keywords = "public"
                 data_package.creator_uid = request.json['uid'] if 'uid' in request.json.keys() else str(uuid.uuid4())
                 data_package.submission_time = datetime.datetime.now()
                 data_package.mime_type = "application/x-zip-compressed"
-                data_package.size = os.path.getsize(os.path.join(app.config.get("OTS_CA_FOLDER"), 'certs', username, filename))
+                data_package.size = os.path.getsize(
+                    os.path.join(app.config.get("OTS_CA_FOLDER"), 'certs', username, filename))
                 data_package.hash = file_hash
                 data_package.submission_user = current_user.id
 
                 try:
                     db.session.add(data_package)
                     db.session.commit()
                 except sqlalchemy.exc.IntegrityError as e:
@@ -256,15 +259,16 @@
 
                 copyfile(os.path.join(app.config.get("OTS_CA_FOLDER"), 'certs', username, "{}".format(filename)),
                          os.path.join(app.config.get("UPLOAD_FOLDER"), "{}.zip".format(file_hash)))
 
                 cert = Certificate()
                 cert.common_name = username
                 cert.username = username
-                cert.expiration_date = datetime.datetime.today() + datetime.timedelta(days=app.config.get("OTS_CA_EXPIRATION_TIME"))
+                cert.expiration_date = datetime.datetime.today() + datetime.timedelta(
+                    days=app.config.get("OTS_CA_EXPIRATION_TIME"))
                 cert.server_address = urlparse(request.url_root).hostname
                 cert.server_port = app.config.get("OTS_SSL_STREAMING_PORT")
                 cert.truststore_filename = truststore_filename
                 cert.user_cert_filename = user_filename
                 cert.cert_password = app.config.get("OTS_CA_PASSWORD")
                 cert.data_package_id = data_package.id if data_package else None
 
@@ -317,15 +321,17 @@
         db.session.delete(data_package[0])
         db.session.commit()
         os.remove(os.path.join(app.config.get("UPLOAD_FOLDER"), "{}.zip".format(data_package[0].hash)))
 
         if data_package[0].certificate:
             Certificate.query.filter_by(id=data_package[0].certificate.id).delete()
             db.session.commit()
-            shutil.rmtree(os.path.join(app.config.get("OTS_CA_FOLDER"), "certs", data_package[0].certificate.common_name), ignore_errors=True)
+            shutil.rmtree(
+                os.path.join(app.config.get("OTS_CA_FOLDER"), "certs", data_package[0].certificate.common_name),
+                ignore_errors=True)
     except BaseException as e:
         logger.error("Failed to delete data package")
         logger.error(traceback.format_exc())
         return jsonify({'success': False, 'error': str(e)}), 500
 
     return jsonify({'success': True})
 
@@ -573,14 +579,15 @@
 
 # This is mainly for mediamtx authentication
 @api_blueprint.route('/api/external_auth', methods=['POST'])
 def external_auth():
     username = bleach.clean(request.json.get('user'))
     password = bleach.clean(request.json.get('password'))
     action = bleach.clean(request.json.get('action'))
+    query = bleach.clean(request.json.get('query'))
 
     user = app.security.datastore.find_user(username=username)
     if user and verify_password(password, user.password):
         if action == 'publish':
             logger.debug("Publish {}".format(request.json.get('path')))
             v = VideoStream()
             v.uid = bleach.clean(request.json.get('id')) if request.json.get('id') else None
@@ -634,45 +641,72 @@
                                 "Failed to add path {} to mediamtx. Status code {} {}".format(v.path, r.status_code,
                                                                                               r.text))
                     except:
                         logger.error(traceback.format_exc())
 
         logger.debug("external_auth returning 200")
         return '', 200
+    elif query:
+        for arg in query.split("&"):
+            key, value = arg.split("=")
+            if key == 'token' and value == app.config.get("OTS_MEDIAMTX_TOKEN"):
+                return '', 200
     else:
         logger.debug("external_auth returning 401")
         return '', 401
 
 
+@api_blueprint.route('/api/videos/thumbnail', methods=['GET'])
+@auth_required()
+def thumbnail():
+    path = request.args.get("path")
+    recording = request.args.get("recording")
+    if not path:
+        return jsonify({"success": False, "error": "Please specify a path"}), 400
+
+    if recording and os.path.exists(os.path.join(app.config.get("OTS_DATA_FOLDER"), "mediamtx", "recordings", path, recording + ".png")):
+        logger.warning(os.path.join(app.config.get("OTS_DATA_FOLDER"), "mediamtx", "recordings", path, recording + ".png"))
+        return send_from_directory(os.path.join(app.config.get("OTS_DATA_FOLDER"), "mediamtx", "recordings", path), recording + ".png")
+
+    elif os.path.exists(os.path.join(app.config.get("OTS_DATA_FOLDER"), "mediamtx", "recordings", path)):
+        return send_from_directory(os.path.join(app.config.get("OTS_DATA_FOLDER"), "mediamtx", "recordings", path), "thumbnail.png")
+
+    return jsonify({"success": False, "error": "Please specify a valid path"}), 400
+
+
 @api_blueprint.route('/api/videos/recordings')
 @auth_required()
 def video_recordings():
     query = db.session.query(VideoRecording)
     query = search(query, VideoRecording, 'path')
 
     return paginate(query)
 
 
-@api_blueprint.route('/api/videos/recording', methods=['GET', 'DELETE'])
+@api_blueprint.route('/api/videos/recording', methods=['GET', 'DELETE', 'HEAD'])
 @auth_required()
 def download_recording():
     if not request.args.get("id"):
         return jsonify({'success': False, 'error': 'Please specify a recording ID'}), 400
     recording_id = bleach.clean(request.args.get('id'))
 
     try:
-        recording = db.session.execute(db.session.query(VideoRecording).filter(VideoRecording.id == recording_id)).first()[0]
+        recording = \
+            db.session.execute(db.session.query(VideoRecording).filter(VideoRecording.id == recording_id)).first()[0]
 
         if request.method == 'GET':
             filename = pathlib.Path(recording.segment_path)
             return send_from_directory(filename.parent, filename.name)
         elif request.method == 'DELETE':
+            os.remove(recording.segment_path)
             db.session.delete(recording)
             db.session.commit()
             return jsonify({'success': True})
+        elif request.method == 'HEAD':
+            return '', 200
     except:
         logger.error(traceback.format_exc())
         return jsonify({'success': False, 'error': 'Recording not found'}), 404
 
 
 @api_blueprint.route('/api/user/assign_eud', methods=['POST'])
 @auth_required()
@@ -744,14 +778,36 @@
 
 
 @api_blueprint.route('/api/truststore')
 def get_truststore():
     return send_from_directory(app.config.get("OTS_CA_FOLDER"), 'truststore-root.p12', as_attachment=True)
 
 
+def get_stream_protocol(source_type):
+    protocol = "rtsp"
+    if source_type.startswith('rtsps'):
+        protocol = 'rtsps'
+    if source_type.startswith('rtsp'):
+        protocol = "rtsp"
+    elif source_type == 'hlsSource':
+        protocol = "hls"
+    elif source_type == 'rpiCameraSource':
+        protocol = "rpi_camera"
+    elif source_type.startswith('rtmp'):
+        protocol = 'rtmp'
+    elif source_type.startswith('srt'):
+        protocol = 'srt'
+    elif source_type.startswith('udp'):
+        protocol = 'udp'
+    elif source_type.startswith('webRTC'):
+        protocol = 'webrtc'
+
+    return protocol
+
+
 @api_blueprint.route('/api/mediamtx/webhook')
 def mediamtx_webhook():
     token = request.args.get('token')
     if not token or bleach.clean(token) != app.config.get("OTS_MEDIAMTX_TOKEN"):
         logger.error('Invalid token')
         return jsonify({'success': False, 'error': 'Invalid token'}), 401
 
@@ -763,14 +819,45 @@
         if path == 'startup':
             paths = VideoStream.query.all()
             for path in paths:
                 r = requests.post("http://localhost:9997/v3/config/paths/add/{}".format(path.path),
                                   json=json.loads(path.mediamtx_settings))
                 logger.debug("Init added {} {}".format(path, r.status_code))
 
+            # Get all paths from MediaMTX and make sure they're in OTS's database
+            r = requests.get("http://localhost:9997/v3/paths/list")
+            paths = r.json()
+            for path in paths['items']:
+                video_stream = db.session.query(VideoStream).where(VideoStream.path == path['name']).first()
+                if not video_stream:
+                    if not path['source']:
+                        continue
+                    video_stream = VideoStream()
+                    video_stream.protocol = get_stream_protocol(path['source']['type'])
+
+                    r = requests.get("http://localhost:9997/v3/config/global/get")
+                    video_stream.port = r.json()['rtspAddress'].replace(":", "")
+
+                    r = requests.get("http://localhost:9997/v3/config/paths/get/{}".format(path['name']))
+                    video_stream.mediamtx_settings = json.dumps(r.json())
+
+                    video_stream.path = path['name']
+                    video_stream.alias = path['name']
+                    video_stream.rtsp_reliable = 1
+                    video_stream.ready = event == 'ready'
+                    video_stream.rover_port = -1
+                    video_stream.ignore_embedded_klv = False
+                    video_stream.buffer_time = None
+                    video_stream.network_timeout = 10000
+                    video_stream.uid = str(uuid.uuid4())
+                    video_stream.generate_xml(urlparse(request.url_root).hostname)
+
+                    db.session.add(video_stream)
+                    db.session.commit()
+
     elif event == 'connect':
         connection_type = bleach.clean(request.args.get("connection_type"))
         connection_id = bleach.clean(request.args.get("connection_id"))
         rtsp_port = bleach.clean(request.args.get("rtsp_port"))
     elif event == 'ready' or event == 'notready':
         rtsp_port = bleach.clean(request.args.get("rtsp_port"))
         path = bleach.clean(request.args.get("path"))
@@ -801,34 +888,42 @@
             elif source_type.startswith('srt'):
                 video_stream.protocol = 'srt'
             elif source_type.startswith('udp'):
                 video_stream.protocol = 'udp'
             elif source_type.startswith('webRTC'):
                 video_stream.protocol = 'webrtc'
 
-            video_stream.query = query
+            # video_stream.query = query
             video_stream.port = rtsp_port
             video_stream.path = path
             video_stream.alias = path
             video_stream.rtsp_reliable = 1
             video_stream.ready = event == 'ready'
             video_stream.rover_port = -1
             video_stream.ignore_embedded_klv = False
             video_stream.buffer_time = None
             video_stream.network_timeout = 10000
             video_stream.uid = str(uuid.uuid4())
             video_stream.generate_xml(urlparse(request.url_root).hostname)
             mediamtx_settings = MediaMTXPathConfig(None)
-            mediamtx_settings.sourceOnDemand.data = False
+            mediamtx_settings.sourceOnDemand.data = source_id is not None
             mediamtx_settings.record.data = False
             video_stream.mediamtx_settings = json.dumps(mediamtx_settings.serialize())
 
             db.session.add(video_stream)
             db.session.commit()
 
+        if event == 'ready':
+            os.makedirs(os.path.join(app.config.get('OTS_DATA_FOLDER'), "mediamtx", "recordings", video_stream.path), exist_ok=True)
+
+            (ffmpeg.input(video_stream.to_json()['rtsp_link'] + "?token={}".format(app.config.get("OTS_MEDIAMTX_TOKEN")))
+             .output(os.path.join(app.config.get('OTS_DATA_FOLDER'), "mediamtx", "recordings", video_stream.path,
+                                  "thumbnail.png"), vframes=1)
+             .overwrite_output().run(capture_stdout=True, capture_stderr=True, quiet=True))
+
     elif event == 'read':
         rtsp_port = bleach.clean(request.args.get("rtsp_port"))
         path = bleach.clean(request.args.get("path"))
         query = bleach.clean(request.args.get("query"))
         reader_type = bleach.clean(request.args.get("reader_type"))
         reader_id = bleach.clean(request.args.get("reader_id"))
     elif event == 'disconnect':
@@ -852,15 +947,15 @@
                                    .values(**recording.serialize()))
                 db.session.commit()
     elif event == 'segment_record_complete':
         segment_path = bleach.clean(request.args.get("segment_path"))
         with app.app_context():
             recording = db.session.execute(db.session.query(VideoRecording)
                                            .filter(VideoRecording.segment_path == segment_path)).first()
-            if recording.count:
+            if recording and recording.count:
                 recording = recording[0]
                 recording.in_progress = False
                 recording.stop_time = datetime.datetime.now()
                 recording.duration = (recording.stop_time - recording.start_time).seconds
             else:
                 recording = VideoRecording()
                 recording.segment_path = bleach.clean(request.args.get('segment_path'))
@@ -872,14 +967,18 @@
                 probe = ffmpeg.probe(recording.segment_path)
                 for stream in probe['streams']:
                     if stream['codec_type'].lower() == 'video':
                         recording.width = stream['width']
                         recording.height = stream['height']
                         recording.video_bitrate = stream['bit_rate']
                         recording.video_codec = stream['codec_name']
+                        ffmpeg.input(recording.segment_path, ss="00:00:01").filter('scale', stream['width'], -1).output(
+                            recording.segment_path + ".png", vframes=1).overwrite_output().run(capture_stdout=True,
+                                                                                               capture_stderr=True,
+                                                                                               quiet=True)
                     elif stream['codec_type'].lower() == 'audio':
                         recording.audio_codec = stream['codec_name']
                         recording.audio_samplerate = stream['sample_rate']
                         recording.audio_channels = stream['channels']
                         recording.audio_bitrate = stream['bit_rate']
                 if 'format' in probe and 'size' in probe['format']:
                     recording.file_size = probe['format']['size']
```

### Comparing `opentakserver-1.1.1/opentakserver/blueprints/config.py` & `opentakserver-1.1.2/opentakserver/blueprints/config.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/blueprints/marti.py` & `opentakserver-1.1.2/opentakserver/blueprints/marti.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/blueprints/ots_socketio.py` & `opentakserver-1.1.2/opentakserver/blueprints/ots_socketio.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/blueprints/scheduled_jobs.py` & `opentakserver-1.1.2/opentakserver/blueprints/scheduled_jobs.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     with apscheduler.app.app_context():
         try:
             r = requests.get('https://api.airplanes.live/v2/point/{}/{}/{}'
                              .format(app.config["OTS_AIRPLANES_LIVE_LAT"],
                                      app.config["OTS_AIRPLANES_LIVE_LON"],
                                      app.config["OTS_AIRPLANES_LIVE_RADIUS"]))
             if r.status_code == 200:
-                rabbit_connection = pika.BlockingConnection(pika.ConnectionParameters('localhost'))
+                rabbit_connection = pika.BlockingConnection(pika.ConnectionParameters('127.0.0.1'))
                 channel = rabbit_connection.channel()
 
                 for craft in r.json()['ac']:
                     try:
                         event = adsbxcot.adsbx_to_cot(craft, known_craft=None)
                     except ValueError:
                         continue
```

### Comparing `opentakserver-1.1.1/opentakserver/blueprints/scheduler_api.py` & `opentakserver-1.1.2/opentakserver/blueprints/scheduler_api.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/ca_config.py` & `opentakserver-1.1.2/opentakserver/ca_config.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/certificate_authority.py` & `opentakserver-1.1.2/opentakserver/certificate_authority.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/controllers/client_controller.py` & `opentakserver-1.1.2/opentakserver/controllers/client_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,23 +49,26 @@
         self.le = 0
         self.course = 0
         self.speed = 0
         self.location_source = None
         self.common_name = None
 
         if self.is_ssl:
-            self.sock.do_handshake()
-            for c in self.sock.getpeercert()['subject']:
-                if c[0][0] == 'commonName':
-                    self.common_name = c[0][1]
-                    self.logger.debug("Got common name {}".format(self.common_name))
+            try:
+                self.sock.do_handshake()
+                for c in self.sock.getpeercert()['subject']:
+                    if c[0][0] == 'commonName':
+                        self.common_name = c[0][1]
+                        self.logger.debug("Got common name {}".format(self.common_name))
+            except BaseException as e:
+                logger.warning("Failed to do handshake: {}".format(e))
 
         # RabbitMQ
         try:
-            self.rabbit_connection = pika.SelectConnection(pika.ConnectionParameters('localhost'),
+            self.rabbit_connection = pika.SelectConnection(pika.ConnectionParameters('127.0.0.1'),
                                                            self.on_connection_open)
             self.rabbit_channel = None
             self.iothread = Thread(target=self.rabbit_connection.ioloop.start)
             self.iothread.daemon = True
             self.iothread.start()
             self.is_consuming = False
         except BaseException as e:
```

### Comparing `opentakserver-1.1.1/opentakserver/controllers/cot_controller.py` & `opentakserver-1.1.2/opentakserver/controllers/cot_controller.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 
         self.online_euds = {}
         self.online_callsigns = {}
         self.exchanges = []
 
         # RabbitMQ
         try:
-            self.rabbit_connection = pika.SelectConnection(pika.ConnectionParameters('localhost'),
+            self.rabbit_connection = pika.SelectConnection(pika.ConnectionParameters('127.0.0.1'),
                                                            self.on_connection_open)
             self.rabbit_channel = None
             self.iothread = Thread(target=self.rabbit_connection.ioloop.start)
             self.iothread.daemon = True
             self.iothread.start()
             self.is_consuming = False
         except BaseException as e:
```

### Comparing `opentakserver-1.1.1/opentakserver/defaultconfig.py` & `opentakserver-1.1.2/opentakserver/defaultconfig.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/EmailValidator.py` & `opentakserver-1.1.2/opentakserver/EmailValidator.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/forms/MediaMTXGlobalConfig.py` & `opentakserver-1.1.2/opentakserver/forms/MediaMTXGlobalConfig.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/forms/MediaMTXPathConfig.py` & `opentakserver-1.1.2/opentakserver/forms/MediaMTXPathConfig.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/models/Alert.py` & `opentakserver-1.1.2/opentakserver/models/Alert.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/models/CasEvac.py` & `opentakserver-1.1.2/opentakserver/models/CasEvac.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/models/Certificate.py` & `opentakserver-1.1.2/opentakserver/models/Certificate.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/models/Chatrooms.py` & `opentakserver-1.1.2/opentakserver/models/Chatrooms.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/models/ChatroomsUids.py` & `opentakserver-1.1.2/opentakserver/models/ChatroomsUids.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/models/CoT.py` & `opentakserver-1.1.2/opentakserver/models/CoT.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/models/DataPackage.py` & `opentakserver-1.1.2/opentakserver/models/DataPackage.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/models/EUD.py` & `opentakserver-1.1.2/opentakserver/models/EUD.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/models/GeoChat.py` & `opentakserver-1.1.2/opentakserver/models/GeoChat.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/models/Icon.py` & `opentakserver-1.1.2/opentakserver/models/Icon.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/models/Marker.py` & `opentakserver-1.1.2/opentakserver/models/Marker.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/models/Point.py` & `opentakserver-1.1.2/opentakserver/models/Point.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/models/RBLine.py` & `opentakserver-1.1.2/opentakserver/models/RBLine.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/models/Team.py` & `opentakserver-1.1.2/opentakserver/models/Team.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/models/user.py` & `opentakserver-1.1.2/opentakserver/models/user.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/models/VideoRecording.py` & `opentakserver-1.1.2/opentakserver/models/VideoRecording.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/models/VideoStream.py` & `opentakserver-1.1.2/opentakserver/models/VideoStream.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/models/ZMIST.py` & `opentakserver-1.1.2/opentakserver/models/ZMIST.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/mumble/mumble_authenticator.py` & `opentakserver-1.1.2/opentakserver/mumble/mumble_authenticator.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/mumble/mumble_ice_app.py` & `opentakserver-1.1.2/opentakserver/mumble/mumble_ice_app.py`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/mumble/Murmur.ice` & `opentakserver-1.1.2/opentakserver/mumble/Murmur.ice`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/opentakserver/SocketServer.py` & `opentakserver-1.1.2/opentakserver/SocketServer.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,14 +44,16 @@
                 self.clients.append(new_thread)
             except KeyboardInterrupt:
                 break
             except TimeoutError:
                 if self.shutdown:
                     self.socket.shutdown(socket.SHUT_RDWR)
                     self.socket.close()
+            except BaseException as e:
+                self.logger.warning(str(e))
 
         if self.ssl:
             self.logger.info("SSL server has shut down")
         else:
             self.logger.info("TCP server has shut down")
 
     def launch_tcp_server(self):
```

### Comparing `opentakserver-1.1.1/pyproject.toml` & `opentakserver-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "opentakserver"
-version = "1.1.1"
+version = "1.1.2"
 description = "A server for ATAK, WinTAK, and iTAK"
 authors = ["OpenTAKServer <opentakserver@gmail.com>"]
 readme = "README.md"
 license = "GPL-3.0-or-later"
 repository = "https://github.com/brian7704/OpenTAKServer"
 documentation = "https://docs.opentakserver.io"
```

### Comparing `opentakserver-1.1.1/README.md` & `opentakserver-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `opentakserver-1.1.1/PKG-INFO` & `opentakserver-1.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: opentakserver
-Version: 1.1.1
+Version: 1.1.2
 Summary: A server for ATAK, WinTAK, and iTAK
 Home-page: https://github.com/brian7704/OpenTAKServer
 License: GPL-3.0-or-later
 Author: OpenTAKServer
 Author-email: opentakserver@gmail.com
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
```

