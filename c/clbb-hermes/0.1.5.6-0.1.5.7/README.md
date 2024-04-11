# Comparing `tmp/clbb-hermes-0.1.5.6.tar.gz` & `tmp/clbb-hermes-0.1.5.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clbb-hermes-0.1.5.6.tar", last modified: Tue Mar 12 14:56:09 2024, max compression
+gzip compressed data, was "clbb-hermes-0.1.5.7.tar", last modified: Thu Apr 11 20:31:52 2024, max compression
```

## Comparing `clbb-hermes-0.1.5.6.tar` & `clbb-hermes-0.1.5.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-03-12 14:56:09.847054 clbb-hermes-0.1.5.6/
--rw-r--r--   0 diego     (1000) diego     (1000)      307 2024-03-12 14:56:09.847054 clbb-hermes-0.1.5.6/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)       14 2024-03-07 13:43:35.000000 clbb-hermes-0.1.5.6/README.md
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-03-12 14:56:09.847054 clbb-hermes-0.1.5.6/clbb_hermes.egg-info/
--rw-r--r--   0 diego     (1000) diego     (1000)      307 2024-03-12 14:56:09.000000 clbb-hermes-0.1.5.6/clbb_hermes.egg-info/PKG-INFO
--rw-rw-r--   0 diego     (1000) diego     (1000)      249 2024-03-12 14:56:09.000000 clbb-hermes-0.1.5.6/clbb_hermes.egg-info/SOURCES.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        1 2024-03-12 14:56:09.000000 clbb-hermes-0.1.5.6/clbb_hermes.egg-info/dependency_links.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)       85 2024-03-12 14:56:09.000000 clbb-hermes-0.1.5.6/clbb_hermes.egg-info/requires.txt
--rw-rw-r--   0 diego     (1000) diego     (1000)        7 2024-03-12 14:56:09.000000 clbb-hermes-0.1.5.6/clbb_hermes.egg-info/top_level.txt
-drwxrwxr-x   0 diego     (1000) diego     (1000)        0 2024-03-12 14:56:09.847054 clbb-hermes-0.1.5.6/hermes/
--rw-rw-r--   0 diego     (1000) diego     (1000)       48 2024-03-08 14:31:46.000000 clbb-hermes-0.1.5.6/hermes/__init__.py
--rw-rw-r--   0 diego     (1000) diego     (1000)        0 2024-03-06 20:27:32.000000 clbb-hermes-0.1.5.6/hermes/functions.py
--rw-rw-r--   0 diego     (1000) diego     (1000)     4267 2024-03-12 14:56:01.000000 clbb-hermes-0.1.5.6/hermes/handler.py
--rw-rw-r--   0 diego     (1000) diego     (1000)       38 2024-03-12 14:56:09.847054 clbb-hermes-0.1.5.6/setup.cfg
--rw-rw-r--   0 diego     (1000) diego     (1000)      384 2024-03-12 14:56:07.000000 clbb-hermes-0.1.5.6/setup.py
+drwxrwxrwx   0        0        0        0 2024-04-11 20:31:52.243672 clbb-hermes-0.1.5.7/
+-rw-rw-rw-   0        0        0      321 2024-04-11 20:31:52.241671 clbb-hermes-0.1.5.7/PKG-INFO
+-rw-rw-rw-   0        0        0       14 2024-03-07 13:43:35.000000 clbb-hermes-0.1.5.7/README.md
+drwxrwxrwx   0        0        0        0 2024-04-11 20:31:52.239673 clbb-hermes-0.1.5.7/clbb_hermes.egg-info/
+-rw-rw-rw-   0        0        0      321 2024-04-11 20:31:52.000000 clbb-hermes-0.1.5.7/clbb_hermes.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      249 2024-04-11 20:31:52.000000 clbb-hermes-0.1.5.7/clbb_hermes.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2024-04-11 20:31:52.000000 clbb-hermes-0.1.5.7/clbb_hermes.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       85 2024-04-11 20:31:52.000000 clbb-hermes-0.1.5.7/clbb_hermes.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2024-04-11 20:31:52.000000 clbb-hermes-0.1.5.7/clbb_hermes.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2024-04-11 20:31:52.237671 clbb-hermes-0.1.5.7/hermes/
+-rw-rw-rw-   0        0        0       48 2024-03-08 14:31:46.000000 clbb-hermes-0.1.5.7/hermes/__init__.py
+-rw-rw-rw-   0        0        0        0 2024-03-06 20:27:32.000000 clbb-hermes-0.1.5.7/hermes/functions.py
+-rw-rw-rw-   0        0        0     4372 2024-04-11 16:38:51.000000 clbb-hermes-0.1.5.7/hermes/handler.py
+-rw-rw-rw-   0        0        0       42 2024-04-11 20:31:52.244322 clbb-hermes-0.1.5.7/setup.cfg
+-rw-rw-rw-   0        0        0      384 2024-04-11 20:23:30.000000 clbb-hermes-0.1.5.7/setup.py
```

### Comparing `clbb-hermes-0.1.5.6/hermes/handler.py` & `clbb-hermes-0.1.5.7/hermes/handler.py`

 * *Files 8% similar despite different names*

```diff
@@ -77,30 +77,32 @@
             geometries.append(wkt.loads(feature['geometry'].split(';')[-1]))
             properties.append(feature['properties'])
 
         amenities = gpd.GeoDataFrame(properties, geometry=geometries)
         amenities.drop(columns=['tags'], inplace=True)
         return amenities
 
-    def load_area_of_interest(self, id=2):
+    def load_area_of_interest(self, id=1):
         area_of_interest = None
         endpoint = f'{self.server_address}/{self.request_data_endpoint}/areaofinterest/{id}/'
         response = requests.get(endpoint)
         data = response.json()
         geometries= [wkt.loads(data['geometry'].split(';')[-1])]
         properties= [data['properties']]
 
         area_of_interest = gpd.GeoDataFrame(properties, geometry=geometries)
         area_of_interest = area_of_interest.set_crs(4326)
         return area_of_interest
 
     def load_network(self, id_network=None):
         if id_network is None:
             id_network = self.id_network
-        filename = f'/app/tmp/net_{id_network}.h5'
+        download_path = '/app/tmp'
+        os.makedirs(download_path, exist_ok=True)
+        filename = os.path.join(download_path, f'net_{id_network}.h5')
         if not os.path.exists(filename):
             endpoint = f'{self.server_address}/{self.request_data_endpoint}/roadnetwork/{id_network}/serve_h5_file/'
             print(endpoint)
             response = requests.get(endpoint)
             if response.status_code == 200:
                 with open(filename, 'wb') as f:
                     f.write(response.content)
```

