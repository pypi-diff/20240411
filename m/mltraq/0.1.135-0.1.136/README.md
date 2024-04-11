# Comparing `tmp/mltraq-0.1.135.tar.gz` & `tmp/mltraq-0.1.136.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mltraq-0.1.135.tar", max compression
+gzip compressed data, was "mltraq-0.1.136.tar", max compression
```

## Comparing `mltraq-0.1.135.tar` & `mltraq-0.1.136.tar`

### file list

```diff
@@ -1,45 +1,45 @@
--rw-r--r--   0        0        0     1558 2024-02-01 14:57:55.062171 mltraq-0.1.135/LICENSE
--rw-r--r--   0        0        0     1438 2024-03-04 22:43:16.862910 mltraq-0.1.135/README.md
--rw-r--r--   0        0        0     2033 2024-04-04 06:53:40.893609 mltraq-0.1.135/pyproject.toml
--rw-r--r--   0        0        0      567 2024-03-19 10:23:28.870801 mltraq-0.1.135/src/mltraq/__init__.py
--rw-r--r--   0        0        0     5580 2024-04-03 13:54:50.228420 mltraq-0.1.135/src/mltraq/cli.py
--rw-r--r--   0        0        0    17976 2024-03-19 13:22:46.831343 mltraq-0.1.135/src/mltraq/experiment.py
--rw-r--r--   0        0        0     4460 2024-03-19 13:22:46.831924 mltraq-0.1.135/src/mltraq/job.py
--rw-r--r--   0        0        0     2594 2024-04-03 16:57:41.689028 mltraq-0.1.135/src/mltraq/opts.py
--rw-r--r--   0        0        0     8344 2024-04-03 13:54:50.228570 mltraq-0.1.135/src/mltraq/run.py
--rw-r--r--   0        0        0     6503 2024-03-14 14:37:15.386067 mltraq-0.1.135/src/mltraq/runs.py
--rw-r--r--   0        0        0     4445 2024-04-03 17:01:21.291897 mltraq-0.1.135/src/mltraq/session.py
--rw-r--r--   0        0        0        0 2024-03-04 22:43:16.892485 mltraq-0.1.135/src/mltraq/steps/__init__.py
--rw-r--r--   0        0        0      511 2024-03-08 14:51:09.434989 mltraq-0.1.135/src/mltraq/steps/chdir.py
--rw-r--r--   0        0        0     1947 2024-03-13 12:59:03.698950 mltraq-0.1.135/src/mltraq/steps/codelog.py
--rw-r--r--   0        0        0      434 2024-03-08 14:51:09.435116 mltraq-0.1.135/src/mltraq/steps/init_fields.py
--rw-r--r--   0        0        0      576 2024-03-05 21:43:24.694290 mltraq-0.1.135/src/mltraq/steps/init_sequences.py
--rw-r--r--   0        0        0      370 2024-03-08 14:51:09.435213 mltraq-0.1.135/src/mltraq/steps/sleep.py
--rw-r--r--   0        0        0        0 2023-01-27 08:07:24.094966 mltraq-0.1.135/src/mltraq/storage/__init__.py
--rw-r--r--   0        0        0     7359 2024-04-04 06:46:09.781812 mltraq-0.1.135/src/mltraq/storage/archivestore.py
--rw-r--r--   0        0        0    14550 2024-04-03 13:54:50.228977 mltraq-0.1.135/src/mltraq/storage/database.py
--rw-r--r--   0        0        0     4500 2024-03-19 13:22:46.832675 mltraq-0.1.135/src/mltraq/storage/datastore.py
--rw-r--r--   0        0        0    15501 2024-03-08 14:51:09.435415 mltraq-0.1.135/src/mltraq/storage/datastream.py
--rw-r--r--   0        0        0     1275 2024-02-26 17:08:44.448505 mltraq-0.1.135/src/mltraq/storage/models.py
--rw-r--r--   0        0        0     4325 2024-03-19 13:22:46.833013 mltraq-0.1.135/src/mltraq/storage/serialization.py
--rw-r--r--   0        0        0     8960 2024-04-03 17:01:21.292242 mltraq-0.1.135/src/mltraq/storage/serializers/datapak.py
--rw-r--r--   0        0        0     2265 2024-03-08 13:58:52.849470 mltraq-0.1.135/src/mltraq/storage/serializers/pickle.py
--rw-r--r--   0        0        0    28608 2024-03-20 19:54:19.798062 mltraq-0.1.135/src/mltraq/storage/serializers/pickle_opcodes_whitelist.py
--rw-r--r--   0        0        0     2896 2024-04-03 13:54:50.229150 mltraq-0.1.135/src/mltraq/storage/serializers/serializer.py
--rw-r--r--   0        0        0        0 2023-01-27 08:07:24.095322 mltraq-0.1.135/src/mltraq/utils/__init__.py
--rw-r--r--   0        0        0     5299 2024-03-05 21:43:24.695673 mltraq-0.1.135/src/mltraq/utils/base_options.py
--rw-r--r--   0        0        0     2150 2024-03-04 22:43:16.893745 mltraq-0.1.135/src/mltraq/utils/bunch.py
--rw-r--r--   0        0        0      699 2024-02-26 17:08:44.449361 mltraq-0.1.135/src/mltraq/utils/enums.py
--rw-r--r--   0        0        0     2989 2024-03-04 22:43:16.893912 mltraq-0.1.135/src/mltraq/utils/exceptions.py
--rw-r--r--   0        0        0      536 2024-02-01 14:57:55.098470 mltraq-0.1.135/src/mltraq/utils/frames.py
--rw-r--r--   0        0        0     2894 2024-04-04 06:44:01.272604 mltraq-0.1.135/src/mltraq/utils/fs.py
--rw-r--r--   0        0        0      542 2024-03-05 21:43:24.695923 mltraq-0.1.135/src/mltraq/utils/json.py
--rw-r--r--   0        0        0     1455 2024-03-08 14:51:09.435616 mltraq-0.1.135/src/mltraq/utils/logging.py
--rw-r--r--   0        0        0     4797 2024-04-03 13:54:50.229310 mltraq-0.1.135/src/mltraq/utils/plot.py
--rw-r--r--   0        0        0     4589 2024-04-03 17:01:21.292620 mltraq-0.1.135/src/mltraq/utils/sequence.py
--rw-r--r--   0        0        0     2518 2024-03-08 14:51:09.435721 mltraq-0.1.135/src/mltraq/utils/sysmon.py
--rw-r--r--   0        0        0      869 2024-02-01 14:57:55.098760 mltraq-0.1.135/src/mltraq/utils/text.py
--rw-r--r--   0        0        0     1605 2024-04-03 17:01:21.443726 mltraq-0.1.135/src/mltraq/utils/web.py
--rw-r--r--   0        0        0       24 2024-04-04 06:53:40.920140 mltraq-0.1.135/src/mltraq/version.py
--rw-r--r--   0        0        0     2504 1970-01-01 00:00:00.000000 mltraq-0.1.135/setup.py
--rw-r--r--   0        0        0     2370 1970-01-01 00:00:00.000000 mltraq-0.1.135/PKG-INFO
+-rw-r--r--   0        0        0     1558 2024-02-01 14:57:55.062171 mltraq-0.1.136/LICENSE
+-rw-r--r--   0        0        0     1391 2024-04-11 14:33:23.808388 mltraq-0.1.136/README.md
+-rw-r--r--   0        0        0     2141 2024-04-11 14:44:36.959409 mltraq-0.1.136/pyproject.toml
+-rw-r--r--   0        0        0      567 2024-03-19 10:23:28.870801 mltraq-0.1.136/src/mltraq/__init__.py
+-rw-r--r--   0        0        0     5613 2024-04-08 07:33:22.170029 mltraq-0.1.136/src/mltraq/cli.py
+-rw-r--r--   0        0        0    17976 2024-03-19 13:22:46.831343 mltraq-0.1.136/src/mltraq/experiment.py
+-rw-r--r--   0        0        0     4460 2024-03-19 13:22:46.831924 mltraq-0.1.136/src/mltraq/job.py
+-rw-r--r--   0        0        0     2594 2024-04-03 16:57:41.689028 mltraq-0.1.136/src/mltraq/opts.py
+-rw-r--r--   0        0        0     8344 2024-04-03 13:54:50.228570 mltraq-0.1.136/src/mltraq/run.py
+-rw-r--r--   0        0        0     6503 2024-03-14 14:37:15.386067 mltraq-0.1.136/src/mltraq/runs.py
+-rw-r--r--   0        0        0     4481 2024-04-08 07:34:41.095061 mltraq-0.1.136/src/mltraq/session.py
+-rw-r--r--   0        0        0        0 2024-03-04 22:43:16.892485 mltraq-0.1.136/src/mltraq/steps/__init__.py
+-rw-r--r--   0        0        0      511 2024-03-08 14:51:09.434989 mltraq-0.1.136/src/mltraq/steps/chdir.py
+-rw-r--r--   0        0        0     1947 2024-03-13 12:59:03.698950 mltraq-0.1.136/src/mltraq/steps/codelog.py
+-rw-r--r--   0        0        0      434 2024-03-08 14:51:09.435116 mltraq-0.1.136/src/mltraq/steps/init_fields.py
+-rw-r--r--   0        0        0      576 2024-03-05 21:43:24.694290 mltraq-0.1.136/src/mltraq/steps/init_sequences.py
+-rw-r--r--   0        0        0      370 2024-03-08 14:51:09.435213 mltraq-0.1.136/src/mltraq/steps/sleep.py
+-rw-r--r--   0        0        0        0 2023-01-27 08:07:24.094966 mltraq-0.1.136/src/mltraq/storage/__init__.py
+-rw-r--r--   0        0        0     7359 2024-04-04 07:00:04.317494 mltraq-0.1.136/src/mltraq/storage/archivestore.py
+-rw-r--r--   0        0        0    14550 2024-04-03 13:54:50.228977 mltraq-0.1.136/src/mltraq/storage/database.py
+-rw-r--r--   0        0        0     4500 2024-03-19 13:22:46.832675 mltraq-0.1.136/src/mltraq/storage/datastore.py
+-rw-r--r--   0        0        0    15512 2024-04-08 07:33:22.170214 mltraq-0.1.136/src/mltraq/storage/datastream.py
+-rw-r--r--   0        0        0     1275 2024-02-26 17:08:44.448505 mltraq-0.1.136/src/mltraq/storage/models.py
+-rw-r--r--   0        0        0     4325 2024-03-19 13:22:46.833013 mltraq-0.1.136/src/mltraq/storage/serialization.py
+-rw-r--r--   0        0        0     8960 2024-04-03 17:01:21.292242 mltraq-0.1.136/src/mltraq/storage/serializers/datapak.py
+-rw-r--r--   0        0        0     2265 2024-03-08 13:58:52.849470 mltraq-0.1.136/src/mltraq/storage/serializers/pickle.py
+-rw-r--r--   0        0        0    28608 2024-03-20 19:54:19.798062 mltraq-0.1.136/src/mltraq/storage/serializers/pickle_opcodes_whitelist.py
+-rw-r--r--   0        0        0     2896 2024-04-03 13:54:50.229150 mltraq-0.1.136/src/mltraq/storage/serializers/serializer.py
+-rw-r--r--   0        0        0        0 2023-01-27 08:07:24.095322 mltraq-0.1.136/src/mltraq/utils/__init__.py
+-rw-r--r--   0        0        0     5299 2024-03-05 21:43:24.695673 mltraq-0.1.136/src/mltraq/utils/base_options.py
+-rw-r--r--   0        0        0     2150 2024-03-04 22:43:16.893745 mltraq-0.1.136/src/mltraq/utils/bunch.py
+-rw-r--r--   0        0        0      699 2024-02-26 17:08:44.449361 mltraq-0.1.136/src/mltraq/utils/enums.py
+-rw-r--r--   0        0        0     2989 2024-03-04 22:43:16.893912 mltraq-0.1.136/src/mltraq/utils/exceptions.py
+-rw-r--r--   0        0        0      536 2024-02-01 14:57:55.098470 mltraq-0.1.136/src/mltraq/utils/frames.py
+-rw-r--r--   0        0        0     2894 2024-04-04 07:00:04.317678 mltraq-0.1.136/src/mltraq/utils/fs.py
+-rw-r--r--   0        0        0      542 2024-03-05 21:43:24.695923 mltraq-0.1.136/src/mltraq/utils/json.py
+-rw-r--r--   0        0        0     1455 2024-03-08 14:51:09.435616 mltraq-0.1.136/src/mltraq/utils/logging.py
+-rw-r--r--   0        0        0     4797 2024-04-03 13:54:50.229310 mltraq-0.1.136/src/mltraq/utils/plot.py
+-rw-r--r--   0        0        0     4589 2024-04-03 17:01:21.292620 mltraq-0.1.136/src/mltraq/utils/sequence.py
+-rw-r--r--   0        0        0     2518 2024-03-08 14:51:09.435721 mltraq-0.1.136/src/mltraq/utils/sysmon.py
+-rw-r--r--   0        0        0      869 2024-02-01 14:57:55.098760 mltraq-0.1.136/src/mltraq/utils/text.py
+-rw-r--r--   0        0        0     1605 2024-04-03 17:01:21.443726 mltraq-0.1.136/src/mltraq/utils/web.py
+-rw-r--r--   0        0        0       24 2024-04-11 14:44:36.982339 mltraq-0.1.136/src/mltraq/version.py
+-rw-r--r--   0        0        0     2457 1970-01-01 00:00:00.000000 mltraq-0.1.136/setup.py
+-rw-r--r--   0        0        0     2323 1970-01-01 00:00:00.000000 mltraq-0.1.136/PKG-INFO
```

### Comparing `mltraq-0.1.135/LICENSE` & `mltraq-0.1.136/LICENSE`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/README.md` & `mltraq-0.1.136/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -21,10 +21,10 @@
 Track anything, stream, reproduce, collaborate, and resume the computation state anywhere.
 
 ---
 
 * **Documentation**: [https://www.mltraq.com](https://www.mltraq.com/)
 * **Source code**: [https://github.com/elehcimd/mltraq](https://github.com/elehcimd/mltraq) (License: [BSD 3-Clause](https://mltraq.com/license/))
 * **Discussions**: [Ask questions, share ideas, engage](https://github.com/elehcimd/mltraq/discussions)
-* **Funding**: You can [sponsor](https://mltraq.com/sponsor/), [cite](https://mltraq.com/cite/), [star](https://github.com/elehcimd/mltraq) the project, and [hire me](https://www.linkedin.com/in/dallachiesa/) for DS/ML/AI work
+* **Funding**: You can [star](https://github.com/elehcimd/mltraq) the project on GitHub and [hire me](https://www.linkedin.com/in/dallachiesa/) to make your experiments run faster
 
 ---
```

### Comparing `mltraq-0.1.135/pyproject.toml` & `mltraq-0.1.136/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mltraq"
-version = "0.1.135"
+version = "0.1.136"
 description = "Track and Collaborate on AI Experiments."
 authors = ["Michele Dallachiesa <michele.dallachiesa@sigforge.com>"]
 license = "BSD-3"
 readme = "README.md"
 homepage = "https://mltraq.com/"
 repository = "https://github.com/elehcimd/mltraq"
 classifiers = [
@@ -58,14 +58,15 @@
 # mlflow = "^2.10.2"
 # aim = "^3.18.1"
 # neptune = "^1.9.1"
 # comet-ml = "^3.38.0"
 # wandb = "^0.16.3"
 # fasttrackml = "0.5.0b2"
 
+# pip install wandb==0.16.3 mlflow==2.11.0 fasttrackml==0.5.0b2 neptune==1.9.1 aim==3.18.1 comet-ml==3.38.1
 
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.black]
```

### Comparing `mltraq-0.1.135/src/mltraq/__init__.py` & `mltraq-0.1.136/src/mltraq/__init__.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/cli.py` & `mltraq-0.1.136/src/mltraq/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,29 +76,29 @@
     if args.cmd == "dss":
         datastream_server()
     elif args.cmd == "ls":
         session = mltraq.create_session()
         print_df(session.ls())
     elif args.cmd == "exp":
         session = mltraq.create_session()
-        experiment = session.load(name=args.experiment_name, id_experiment=args.experiment_uuid)
+        experiment = session.load_experiment(name=args.experiment_name, id_experiment=args.experiment_uuid)
         print_df(experiment.df())
     elif args.cmd == "runs":
         session = mltraq.create_session()
-        experiment = session.load(name=args.experiment_name, id_experiment=args.experiment_uuid)
+        experiment = session.load_experiment(name=args.experiment_name, id_experiment=args.experiment_uuid)
         print_df(experiment.runs.df())
     elif args.cmd == "options":
         df = pd.Series(options().flatten(), name="Value").to_frame()
         df.index.name = "Name"
         if args.option_name:
             df = df[df.index == args.option_name]
         print_df(df)
     elif args.cmd == "stats":
         session = mltraq.create_session()
-        experiment = session.load(name=args.experiment_name, id_experiment=args.experiment_uuid)
+        experiment = session.load_experiment(name=args.experiment_name, id_experiment=args.experiment_uuid)
         df = experiment_stats(experiment)
         if args.stat_name:
             df = df[df.index == args.stat_name]
         print_df(df, showindex=True)
     else:
         raise InvalidInput(f"Unknown command '{args.cmd}'")
```

### Comparing `mltraq-0.1.135/src/mltraq/experiment.py` & `mltraq-0.1.136/src/mltraq/experiment.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/job.py` & `mltraq-0.1.136/src/mltraq/job.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/opts.py` & `mltraq-0.1.136/src/mltraq/opts.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/run.py` & `mltraq-0.1.136/src/mltraq/run.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/runs.py` & `mltraq-0.1.136/src/mltraq/runs.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/session.py` & `mltraq-0.1.136/src/mltraq/session.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,27 +71,29 @@
 
     def ls(self) -> pd.DataFrame:
         """
         Returns a Pandas dataframe with the list of persisted experiments.
         """
         return Experiment.ls(self.db)
 
-    def load(
+    def load_experiment(
         self, name: str | None = None, id_experiment: uuid.UUID | None = None, unsafe_pickle: bool = False
     ) -> Experiment:
         """
         Loads a persisted experiment by `name` or `id_experiment`. If `pickle` is True, it will
         attempt to reload the pickled Experiment object from database.
         Unpickling Experiment objects is unsafe, but powerful.
         Whenever possible, prefer the safe persistence of experiment states.
         """
 
         return Experiment.load(self.db, name=name, id_experiment=id_experiment, unsafe_pickle=unsafe_pickle)
 
-    def persist(self, experiment: Experiment, name: str | None = None, if_exists: IfExists = "fail") -> Experiment:
+    def persist_experiment(
+        self, experiment: Experiment, name: str | None = None, if_exists: IfExists = "fail"
+    ) -> Experiment:
         """
         Persist the experiment on the database linked by the session (as a copy), and return it.
         The database considered is the one of the session, allowing us to copy experiments
         between datasets. The new experiment will have a different UUID and its name will be retained,
         if not specified otherwise via `name`.
 
         If `name` is passed, it is used as name of the experiment to persist.
```

### Comparing `mltraq-0.1.135/src/mltraq/steps/codelog.py` & `mltraq-0.1.136/src/mltraq/steps/codelog.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/steps/init_sequences.py` & `mltraq-0.1.136/src/mltraq/steps/init_sequences.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/storage/archivestore.py` & `mltraq-0.1.136/src/mltraq/storage/archivestore.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/storage/database.py` & `mltraq-0.1.136/src/mltraq/storage/database.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/storage/datastore.py` & `mltraq-0.1.136/src/mltraq/storage/datastore.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/storage/datastream.py` & `mltraq-0.1.136/src/mltraq/storage/datastream.py`

 * *Files 0% similar despite different names*

```diff
@@ -359,15 +359,15 @@
             return
 
         id_experiments = set()
         for message in self.batch:
             try:
                 # The experiment and run must already exist in the db.
                 if message["id_experiment"] not in self.experiments:
-                    self.experiments[message["id_experiment"]] = self.session.load(
+                    self.experiments[message["id_experiment"]] = self.session.load_experiment(
                         id_experiment=message["id_experiment"]
                     )
                 run = self.experiments[message["id_experiment"]].runs[message["id_run"]]
 
                 # If the sequence with field_name doesn't exist, add it.
                 if message["field_name"] not in run.fields:
                     run.fields[message["field_name"]] = Sequence()
```

### Comparing `mltraq-0.1.135/src/mltraq/storage/models.py` & `mltraq-0.1.136/src/mltraq/storage/models.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/storage/serialization.py` & `mltraq-0.1.136/src/mltraq/storage/serialization.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/storage/serializers/datapak.py` & `mltraq-0.1.136/src/mltraq/storage/serializers/datapak.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/storage/serializers/pickle.py` & `mltraq-0.1.136/src/mltraq/storage/serializers/pickle.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/storage/serializers/pickle_opcodes_whitelist.py` & `mltraq-0.1.136/src/mltraq/storage/serializers/pickle_opcodes_whitelist.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/storage/serializers/serializer.py` & `mltraq-0.1.136/src/mltraq/storage/serializers/serializer.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/utils/base_options.py` & `mltraq-0.1.136/src/mltraq/utils/base_options.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/utils/bunch.py` & `mltraq-0.1.136/src/mltraq/utils/bunch.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/utils/enums.py` & `mltraq-0.1.136/src/mltraq/utils/enums.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/utils/exceptions.py` & `mltraq-0.1.136/src/mltraq/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/utils/frames.py` & `mltraq-0.1.136/src/mltraq/utils/frames.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/utils/fs.py` & `mltraq-0.1.136/src/mltraq/utils/fs.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/utils/json.py` & `mltraq-0.1.136/src/mltraq/utils/json.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/utils/logging.py` & `mltraq-0.1.136/src/mltraq/utils/logging.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/utils/plot.py` & `mltraq-0.1.136/src/mltraq/utils/plot.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/utils/sequence.py` & `mltraq-0.1.136/src/mltraq/utils/sequence.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/utils/sysmon.py` & `mltraq-0.1.136/src/mltraq/utils/sysmon.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/utils/text.py` & `mltraq-0.1.136/src/mltraq/utils/text.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/src/mltraq/utils/web.py` & `mltraq-0.1.136/src/mltraq/utils/web.py`

 * *Files identical despite different names*

### Comparing `mltraq-0.1.135/setup.py` & `mltraq-0.1.136/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -24,17 +24,17 @@
  'tqdm>=4.64.1']
 
 entry_points = \
 {'console_scripts': ['mltraq = mltraq.cli:main']}
 
 setup_kwargs = {
     'name': 'mltraq',
-    'version': '0.1.135',
+    'version': '0.1.136',
     'description': 'Track and Collaborate on AI Experiments.',
-    'long_description': '<p align="center">\n<img width="75%" height="75%" src="https://mltraq.com/assets/img/logo-wide-black.svg" alt="MLtraq Logo">\n</p>\n\n<p align="center">\n<img src="https://www.mltraq.com/assets/img/badges/test.svg" alt="Test">\n<img src="https://www.mltraq.com/assets/img/badges/coverage.svg" alt="Coverage">\n<img src="https://www.mltraq.com/assets/img/badges/python.svg" alt="Python">\n<img src="https://www.mltraq.com/assets/img/badges/pypi.svg" alt="PyPi">\n<img src="https://www.mltraq.com/assets/img/badges/license.svg" alt="License">\n<img src="https://www.mltraq.com/assets/img/badges/code-style.svg" alt="Code style">\n</p>\n\n---\n\n<h1 align="center">\nTrack and Collaborate on AI Experiments.\n</h1>\n\nThe open-source Python library for AI developers to design, execute and share experiments.\nTrack anything, stream, reproduce, collaborate, and resume the computation state anywhere.\n\n---\n\n* **Documentation**: [https://www.mltraq.com](https://www.mltraq.com/)\n* **Source code**: [https://github.com/elehcimd/mltraq](https://github.com/elehcimd/mltraq) (License: [BSD 3-Clause](https://mltraq.com/license/))\n* **Discussions**: [Ask questions, share ideas, engage](https://github.com/elehcimd/mltraq/discussions)\n* **Funding**: You can [sponsor](https://mltraq.com/sponsor/), [cite](https://mltraq.com/cite/), [star](https://github.com/elehcimd/mltraq) the project, and [hire me](https://www.linkedin.com/in/dallachiesa/) for DS/ML/AI work\n\n---\n',
+    'long_description': '<p align="center">\n<img width="75%" height="75%" src="https://mltraq.com/assets/img/logo-wide-black.svg" alt="MLtraq Logo">\n</p>\n\n<p align="center">\n<img src="https://www.mltraq.com/assets/img/badges/test.svg" alt="Test">\n<img src="https://www.mltraq.com/assets/img/badges/coverage.svg" alt="Coverage">\n<img src="https://www.mltraq.com/assets/img/badges/python.svg" alt="Python">\n<img src="https://www.mltraq.com/assets/img/badges/pypi.svg" alt="PyPi">\n<img src="https://www.mltraq.com/assets/img/badges/license.svg" alt="License">\n<img src="https://www.mltraq.com/assets/img/badges/code-style.svg" alt="Code style">\n</p>\n\n---\n\n<h1 align="center">\nTrack and Collaborate on AI Experiments.\n</h1>\n\nThe open-source Python library for AI developers to design, execute and share experiments.\nTrack anything, stream, reproduce, collaborate, and resume the computation state anywhere.\n\n---\n\n* **Documentation**: [https://www.mltraq.com](https://www.mltraq.com/)\n* **Source code**: [https://github.com/elehcimd/mltraq](https://github.com/elehcimd/mltraq) (License: [BSD 3-Clause](https://mltraq.com/license/))\n* **Discussions**: [Ask questions, share ideas, engage](https://github.com/elehcimd/mltraq/discussions)\n* **Funding**: You can [star](https://github.com/elehcimd/mltraq) the project on GitHub and [hire me](https://www.linkedin.com/in/dallachiesa/) to make your experiments run faster\n\n---\n',
     'author': 'Michele Dallachiesa',
     'author_email': 'michele.dallachiesa@sigforge.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://mltraq.com/',
     'package_dir': package_dir,
     'packages': packages,
```

### Comparing `mltraq-0.1.135/PKG-INFO` & `mltraq-0.1.136/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mltraq
-Version: 0.1.135
+Version: 0.1.136
 Summary: Track and Collaborate on AI Experiments.
 Home-page: https://mltraq.com/
 License: BSD-3
 Author: Michele Dallachiesa
 Author-email: michele.dallachiesa@sigforge.com
 Requires-Python: >=3.10.0,<3.13.0
 Classifier: Development Status :: 3 - Alpha
@@ -47,11 +47,11 @@
 Track anything, stream, reproduce, collaborate, and resume the computation state anywhere.
 
 ---
 
 * **Documentation**: [https://www.mltraq.com](https://www.mltraq.com/)
 * **Source code**: [https://github.com/elehcimd/mltraq](https://github.com/elehcimd/mltraq) (License: [BSD 3-Clause](https://mltraq.com/license/))
 * **Discussions**: [Ask questions, share ideas, engage](https://github.com/elehcimd/mltraq/discussions)
-* **Funding**: You can [sponsor](https://mltraq.com/sponsor/), [cite](https://mltraq.com/cite/), [star](https://github.com/elehcimd/mltraq) the project, and [hire me](https://www.linkedin.com/in/dallachiesa/) for DS/ML/AI work
+* **Funding**: You can [star](https://github.com/elehcimd/mltraq) the project on GitHub and [hire me](https://www.linkedin.com/in/dallachiesa/) to make your experiments run faster
 
 ---
```

