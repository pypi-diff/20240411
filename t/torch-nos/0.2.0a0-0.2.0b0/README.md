# Comparing `tmp/torch_nos-0.2.0a0-py3-none-any.whl.zip` & `tmp/torch_nos-0.2.0b0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,33 +1,33 @@
-Zip file size: 1760034 bytes, number of entries: 102
+Zip file size: 1752491 bytes, number of entries: 91
 -rw-r--r--  2.0 unx      424 b- defN 23-Dec-19 22:33 nos/__init__.py
 -rw-r--r--  2.0 unx     1951 b- defN 24-Feb-20 17:08 nos/constants.py
 -rw-r--r--  2.0 unx      750 b- defN 24-Jan-02 20:35 nos/exceptions.py
 -rw-r--r--  2.0 unx     2295 b- defN 23-Dec-19 22:33 nos/logging.py
 -rw-r--r--  2.0 unx     3199 b- defN 24-Jan-02 20:35 nos/protoc.py
 -rw-r--r--  2.0 unx     1436 b- defN 23-Dec-19 22:33 nos/telemetry.py
--rw-r--r--  2.0 unx       23 b- defN 24-Feb-21 20:57 nos/version.py
+-rw-r--r--  2.0 unx       23 b- defN 24-Apr-11 19:14 nos/version.py
 -rw-r--r--  2.0 unx     1898 b- defN 24-Feb-20 17:08 nos/catalogs/model_profile_catalog.json
 -rw-r--r--  2.0 unx      858 b- defN 24-Jan-16 08:09 nos/cli/cli.py
 -rw-r--r--  2.0 unx     1417 b- defN 24-Jan-02 20:35 nos/cli/hub.py
 -rw-r--r--  2.0 unx     7330 b- defN 24-Jan-02 20:35 nos/cli/predict.py
--rw-r--r--  2.0 unx    19039 b- defN 24-Feb-21 20:57 nos/cli/profile.py
--rw-r--r--  2.0 unx    19109 b- defN 24-Feb-20 22:08 nos/cli/serve.py
+-rw-r--r--  2.0 unx    13556 b- defN 24-Apr-11 19:08 nos/cli/profile.py
+-rw-r--r--  2.0 unx    19110 b- defN 24-Apr-11 00:42 nos/cli/serve.py
 -rw-r--r--  2.0 unx     1838 b- defN 23-Dec-19 22:33 nos/cli/system.py
 -rw-r--r--  2.0 unx      425 b- defN 23-May-05 01:05 nos/cli/utils.py
--rw-r--r--  2.0 unx     1979 b- defN 24-Feb-20 22:08 nos/cli/templates/docker-compose.serve.yml.j2
+-rw-r--r--  2.0 unx     1836 b- defN 24-Apr-11 19:08 nos/cli/templates/docker-compose.serve.yml.j2
 -rw-r--r--  2.0 unx      398 b- defN 24-Jan-02 20:35 nos/client/__init__.py
 -rw-r--r--  2.0 unx    30281 b- defN 24-Feb-20 22:10 nos/client/grpc.py
 -rw-r--r--  2.0 unx     3094 b- defN 24-Feb-20 17:08 nos/common/__init__.py
 -rw-r--r--  2.0 unx      204 b- defN 23-Jun-13 21:50 nos/common/cloudpickle.py
 -rw-r--r--  2.0 unx      906 b- defN 24-Jan-02 20:35 nos/common/exceptions.py
 -rw-r--r--  2.0 unx     5154 b- defN 23-Sep-02 01:00 nos/common/git.py
 -rw-r--r--  2.0 unx     1028 b- defN 24-Jan-02 20:35 nos/common/helpers.py
 -rw-r--r--  2.0 unx      499 b- defN 23-Sep-02 01:00 nos/common/metaclass.py
--rw-r--r--  2.0 unx    20848 b- defN 24-Feb-21 01:22 nos/common/profiler.py
+-rw-r--r--  2.0 unx    20811 b- defN 24-Apr-11 19:08 nos/common/profiler.py
 -rw-r--r--  2.0 unx      805 b- defN 24-Feb-20 17:08 nos/common/runtime.py
 -rw-r--r--  2.0 unx    11842 b- defN 23-Dec-19 22:33 nos/common/shm.py
 -rw-r--r--  2.0 unx    31844 b- defN 24-Feb-20 17:08 nos/common/spec.py
 -rw-r--r--  2.0 unx     7930 b- defN 24-Jan-02 20:35 nos/common/system.py
 -rw-r--r--  2.0 unx      830 b- defN 24-Jan-02 20:35 nos/common/tasks.py
 -rw-r--r--  2.0 unx     6117 b- defN 24-Feb-20 17:08 nos/common/types.py
 -rw-r--r--  2.0 unx     1465 b- defN 24-Feb-20 17:08 nos/common/io/__init__.py
@@ -67,38 +67,27 @@
 -rw-r--r--  2.0 unx     1284 b- defN 24-Feb-20 17:08 nos/neuron/device.py
 -rw-r--r--  2.0 unx     1895 b- defN 24-Jan-02 20:35 nos/proto/nos_service.proto
 -rw-r--r--  2.0 unx    10483 b- defN 23-Dec-19 22:33 nos/server/__init__.py
 -rw-r--r--  2.0 unx     7341 b- defN 24-Jan-02 20:35 nos/server/_docker.py
 -rw-r--r--  2.0 unx     9632 b- defN 24-Feb-20 17:08 nos/server/_runtime.py
 -rw-r--r--  2.0 unx    20201 b- defN 24-Feb-20 17:08 nos/server/_service.py
 -rw-r--r--  2.0 unx       83 b- defN 23-Oct-24 05:52 nos/server/http/__init__.py
--rw-r--r--  2.0 unx    21273 b- defN 24-Feb-21 01:29 nos/server/http/_service.py
+-rw-r--r--  2.0 unx    20019 b- defN 24-Apr-11 19:08 nos/server/http/_service.py
 -rw-r--r--  2.0 unx     2865 b- defN 23-Dec-19 22:33 nos/server/http/_utils.py
 -rw-r--r--  2.0 unx     4223 b- defN 24-Jan-02 20:35 nos/server/http/integrations/openai/models.py
 -rw-r--r--  2.0 unx      373 b- defN 23-Apr-23 00:49 nos/test/benchmark.py
 -rw-r--r--  2.0 unx    10761 b- defN 24-Jan-02 20:35 nos/test/conftest.py
 -rw-r--r--  2.0 unx     2749 b- defN 24-Jan-02 20:35 nos/test/utils.py
 -rw-r--r--  2.0 unx   259865 b- defN 23-Sep-21 19:18 nos/test/test_data/test.jpg
 -rw-r--r--  2.0 unx   300601 b- defN 23-Sep-21 19:18 nos/test/test_data/test.mp4
 -rw-r--r--  2.0 unx  1152693 b- defN 23-Sep-21 19:18 nos/test/test_data/test_speech.flac
--rw-rw-r--  2.0 unx     1163 b- defN 23-Nov-07 23:24 nos/test/test_data/hub/custom_model/Dockerfile.custom_model
--rw-r--r--  2.0 unx      185 b- defN 24-Jan-02 20:35 nos/test/test_data/hub/custom_model/config-alternate-init-kwargs.yaml
--rw-r--r--  2.0 unx      159 b- defN 24-Feb-20 17:08 nos/test/test_data/hub/custom_model/config-malformed-model-cls.yaml
--rw-r--r--  2.0 unx      162 b- defN 24-Feb-20 17:08 nos/test/test_data/hub/custom_model/config-malformed-model-method.yaml
--rw-r--r--  2.0 unx      160 b- defN 24-Feb-20 17:08 nos/test/test_data/hub/custom_model/config-malformed-model-path.yaml
--rw-r--r--  2.0 unx      430 b- defN 24-Feb-20 17:08 nos/test/test_data/hub/custom_model/config-with-existing-model-id.yaml
--rw-r--r--  2.0 unx      654 b- defN 24-Feb-20 17:08 nos/test/test_data/hub/custom_model/config-with-replicas.yaml
--rw-r--r--  2.0 unx      353 b- defN 24-Jan-02 20:35 nos/test/test_data/hub/custom_model/config.yaml
--rw-rw-r--  2.0 unx      900 b- defN 23-Oct-31 21:34 nos/test/test_data/hub/custom_model/docker-compose.animatediff.yml
--rw-rw-r--  2.0 unx      993 b- defN 23-Nov-01 02:54 nos/test/test_data/hub/custom_model/docker-compose.custom_model.yml
 -rw-r--r--  2.0 unx      178 b- defN 24-Jan-02 20:35 nos/test/test_data/hub/custom_model/models/model.py
--rwxrwxr-x  2.0 unx      332 b- defN 23-Oct-27 23:27 nos/test/test_data/hub/custom_model/scripts/entrypoint.sh
 -rw-r--r--  2.0 unx     2101 b- defN 24-Jan-22 21:22 nos-profiling-catalogs/nos-profile--0-1-4a--20240122--nvidia-geforce-rtx-2080.json
 -rw-rw-r--  2.0 unx     2086 b- defN 24-Jan-23 21:49 nos-profiling-catalogs/nos-profile--0-1-5--20240123--nvidia-geforce-rtx-2080.json
 -rw-r--r--  2.0 unx     3006 b- defN 23-Aug-29 22:59 scripts/nos_bot.py
--rw-rw-r--  2.0 unx    11355 b- defN 24-Feb-21 21:15 torch_nos-0.2.0a0.dist-info/LICENSE
--rw-r--r--  2.0 unx    27187 b- defN 24-Feb-21 21:15 torch_nos-0.2.0a0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 24-Feb-21 21:15 torch_nos-0.2.0a0.dist-info/WHEEL
--rw-r--r--  2.0 unx      135 b- defN 24-Feb-21 21:15 torch_nos-0.2.0a0.dist-info/entry_points.txt
--rw-r--r--  2.0 unx       35 b- defN 24-Feb-21 21:15 torch_nos-0.2.0a0.dist-info/top_level.txt
--rw-rw-r--  2.0 unx     8749 b- defN 24-Feb-21 21:15 torch_nos-0.2.0a0.dist-info/RECORD
-102 files, 2196247 bytes uncompressed, 1746242 bytes compressed:  20.5%
+-rw-rw-r--  2.0 unx    11355 b- defN 24-Apr-11 19:15 torch_nos-0.2.0b0.dist-info/LICENSE
+-rw-r--r--  2.0 unx    26900 b- defN 24-Apr-11 19:15 torch_nos-0.2.0b0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 24-Apr-11 19:15 torch_nos-0.2.0b0.dist-info/WHEEL
+-rw-r--r--  2.0 unx      135 b- defN 24-Apr-11 19:15 torch_nos-0.2.0b0.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx       74 b- defN 24-Apr-11 19:15 torch_nos-0.2.0b0.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx     7431 b- defN 24-Apr-11 19:15 torch_nos-0.2.0b0.dist-info/RECORD
+91 files, 2182274 bytes uncompressed, 1740937 bytes compressed:  20.2%
```

## zipnote {}

```diff
@@ -237,71 +237,38 @@
 
 Filename: nos/test/test_data/test.mp4
 Comment: 
 
 Filename: nos/test/test_data/test_speech.flac
 Comment: 
 
-Filename: nos/test/test_data/hub/custom_model/Dockerfile.custom_model
-Comment: 
-
-Filename: nos/test/test_data/hub/custom_model/config-alternate-init-kwargs.yaml
-Comment: 
-
-Filename: nos/test/test_data/hub/custom_model/config-malformed-model-cls.yaml
-Comment: 
-
-Filename: nos/test/test_data/hub/custom_model/config-malformed-model-method.yaml
-Comment: 
-
-Filename: nos/test/test_data/hub/custom_model/config-malformed-model-path.yaml
-Comment: 
-
-Filename: nos/test/test_data/hub/custom_model/config-with-existing-model-id.yaml
-Comment: 
-
-Filename: nos/test/test_data/hub/custom_model/config-with-replicas.yaml
-Comment: 
-
-Filename: nos/test/test_data/hub/custom_model/config.yaml
-Comment: 
-
-Filename: nos/test/test_data/hub/custom_model/docker-compose.animatediff.yml
-Comment: 
-
-Filename: nos/test/test_data/hub/custom_model/docker-compose.custom_model.yml
-Comment: 
-
 Filename: nos/test/test_data/hub/custom_model/models/model.py
 Comment: 
 
-Filename: nos/test/test_data/hub/custom_model/scripts/entrypoint.sh
-Comment: 
-
 Filename: nos-profiling-catalogs/nos-profile--0-1-4a--20240122--nvidia-geforce-rtx-2080.json
 Comment: 
 
 Filename: nos-profiling-catalogs/nos-profile--0-1-5--20240123--nvidia-geforce-rtx-2080.json
 Comment: 
 
 Filename: scripts/nos_bot.py
 Comment: 
 
-Filename: torch_nos-0.2.0a0.dist-info/LICENSE
+Filename: torch_nos-0.2.0b0.dist-info/LICENSE
 Comment: 
 
-Filename: torch_nos-0.2.0a0.dist-info/METADATA
+Filename: torch_nos-0.2.0b0.dist-info/METADATA
 Comment: 
 
-Filename: torch_nos-0.2.0a0.dist-info/WHEEL
+Filename: torch_nos-0.2.0b0.dist-info/WHEEL
 Comment: 
 
-Filename: torch_nos-0.2.0a0.dist-info/entry_points.txt
+Filename: torch_nos-0.2.0b0.dist-info/entry_points.txt
 Comment: 
 
-Filename: torch_nos-0.2.0a0.dist-info/top_level.txt
+Filename: torch_nos-0.2.0b0.dist-info/top_level.txt
 Comment: 
 
-Filename: torch_nos-0.2.0a0.dist-info/RECORD
+Filename: torch_nos-0.2.0b0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## nos/version.py

```diff
@@ -1 +1 @@
-__version__ = "0.2.0a"
+__version__ = "0.2.0b"
```

## nos/cli/profile.py

```diff
@@ -11,20 +11,14 @@
 
 import humanize
 import numpy as np
 import typer
 from PIL import Image
 from rich import print
 
-import sky
-from sky.backends.cloud_vm_ray_backend import CloudVmRayResourceHandle
-import requests
-from nos.client import Client
-import time
-
 from nos import hub
 from nos.common.profiler import ModelProfiler, ModelProfileRequest, Profiler
 from nos.common.spec import ModelSpec
 from nos.common.tasks import TaskType
 from nos.logging import logger
 from nos.server._runtime import InferenceServiceRuntime
 from nos.test.utils import NOS_TEST_IMAGE
@@ -69,161 +63,18 @@
         if model_id is not None and model_id != _model_id:
             continue
         spec: ModelSpec = hub.load_spec(_model_id)
         for method in spec.signature:
             yield _model_id, method, spec
 
 
-def launch_profiling_cluster_with_resource(resource_name: str, cluster_name: str = None) -> CloudVmRayResourceHandle:
-    # Launch a cluster with the specified resource
-    if cluster_name is None:
-        cluster_name = f"nos-profile-{resource_name}"
-
-    # Check if the cluster already exists
-    status = sky.status(cluster_name)
-    if len(status) > 0:
-        print(f"Cluster {cluster_name} already exists")
-        status = sky.status(cluster_name)
-        return status[0]['handle']
-
-    # HACK: for now we've just added gpu and server resources to 
-    # the http gateway so we can run the full profiling flow, but 
-    # ideally this should be serialized out of the server.
-    # Below will only work with the profiling rest endpoint exposed.
-    # Only supports single model profiling for now. 
-    # TODO: are we using the right nos version for this?
-    nos_task = sky.Task(setup='pip install torch-nos',
-            run='nos serve up --http')
-            # workdir='~/.nosd/remote') 
-    
-    nos_task.set_resources(sky.Resources(accelerators=resource_name, ports=['50051']))
-    
-    try:
-        print('launching cluster...')
-        id, handle = sky.launch( 
-            task=nos_task,
-            cluster_name=cluster_name,
-            retry_until_up=True,
-            idle_minutes_to_autostop=30, # Kill the cluster after 30 mins of inactivity
-            down=False, # Keep it running until then
-            dryrun=False, # Turn this off when it works
-            stream_logs=False,
-            # detach_run=True,
-        )
-    except Exception as e:
-        print(f"Failed to launch cluster {cluster_name} with resource {resource_name}")
-        print(e)
-        raise e
-
-    print(f"Launched cluster {cluster_name} with resource {resource_name}" )
-
-    return handle
-
-
-def profile_cluster_model_id(resource_handle: CloudVmRayResourceHandle, model_id: str):
-    active_ports = resource_handle.launched_resources.ports
-    # We always use 50051 for consistency, uncler if this causes 
-    # issues for multiple nos instances on one cluster?
-    assert '50051' in active_ports
-    client = Client(f"{resource_handle.head_ip}:50051")
-    print(f"Connecting to {resource_handle.head_ip}:50051...")
-    try:
-        client.WaitForServer()
-    except:
-        print(f"Failed to connect to {resource_handle.head_ip}:50051")
-        return
-    
-    if not client.IsHealthy():
-        print(f"Failed to connect to {resource_handle.head_ip}:50051")
-        return
-
-    assert model_id is not None
-    models: List[str] = client.ListModels()
-    assert model_id in models
-
-    """
-        $ curl -X POST \
-            'http://localhost:8000/v1/profile \
-            -H 'accept: application/json' \
-            -H 'Content-Type: multipart/form-data' \
-            -F 'model_id=yolox/small' \
-            -F '
-    """
-
-    print(f"Profiling {model_id}...")
-
-    res = requests.post(
-        f"http://{resource_handle.head_ip}:8000/v1/profile",
-        headers={"accept": "application/json", "Content-Type": "multipart/form-data"},
-        data={"model_id": model_id},
-    )
-
-    if res.status_code != 200:
-        print(f"Failed to profile {model_id}")
-        return
-    
-    catalog_path = res.json()["catalog_path"]
-    print("Catalog path: ", catalog_path)
-
-
-    # Old flow: just pings /infer
-    """
-    model = client.Module(model_id)
-    assert model is not None
-    assert model.GetModelInfo() is not None
-    print(f"Test [model={model_id}]")
-
-    url = "http://images.cocodataset.org/val2017/000000039769.jpg"
-    image = Image.open(requests.get(url, stream=True).raw)
-
-    # exclude model loading time
-    response = model(prompts=['astronaut on the moon'])
-
-    total_runs = 3
-    runs = []
-
-    for i in range(total_runs):
-        start_time = time.time()
-        response = model(prompts=['astronaut on the moon'])
-        end_time = time.time()
-        assert isinstance(response, dict)
-        print(f"Time taken: {end_time - start_time} seconds")
-        runs.append(end_time - start_time)
-
-    print(f"Average time taken: {sum(runs) / total_runs} seconds") 
-    """
-
-
-def profile_remote(
-    model_id: str = None, resource: str = None
-) -> Profiler:
-    """Entrypoint for profiling remote models."""
-
-    # Launch a profiling service on the appropriate resource if it doesn't already exist
-    try:
-        resource_handle = launch_profiling_cluster_with_resource(resource)
-    except Exception as e:
-        print(f"Failed to launch cluster with resource {resource}")
-        print(e)
-        return
-
-    print("got resource handle: ", resource_handle)
-    print('profiling: ', model_id)
-    profile_cluster_model_id(resource_handle, model_id)
-    return
-
-
 def profile_models(
-    model_id: str = None, device_id: int = 0, save: bool = False, verbose: bool = False, remote: str = None, catalog_path: str = None
-):
+    model_id: str = None, device_id: int = 0, save: bool = False, verbose: bool = False, catalog_path: str = None
+) -> Profiler:
     """Main entrypoint for profiling all models."""
-
-    if remote is not None:
-        # Requested remote profiling on a specific resource
-        resource_handle = launch_profiling_cluster_with_resource(remote)
     import torch
 
     # TODO (spillai): Pytorch cuda.devices are reported in the descending order of memory,
     # so we need to force them to match the `nvidia-smi` order. Setting CUDA_DEVICE_ORDER=PCI_BUS_ID
     # allows us to keep the order consistent with `nvidia-smi`.
     assert torch.cuda.device_count() > 0, "No CUDA devices found, profiling is only supported on NVIDIA currently."
     # assert os.getenv("CUDA_DEVICE_ORDER", "") == "PCI_BUS_ID", "CUDA_DEVICE_ORDER must be PCI_BUS_ID."
@@ -345,44 +196,34 @@
             logger.warning(f"Unsupported task: {task}, skipping.")
             continue
 
     # Run the profiler, and optionally save the catalog
     profiler.run()
     if save:
         profiler.save(catalog_path=catalog_path)
-    return profiler, catalog_path
+    return profiler
 
 
 def profile_models_with_method(
     method_name: str, device_id: int = 0, save: bool = False, verbose: bool = False, catalog_path: str = None
 ) -> Profiler:
     for model_id, method, _spec in _model_methods(None):
         if method == method_name:
             profile_models(model_id, device_id, save, verbose, catalog_path)
 
 
-@profile_cli.command(name="remote")
-def _profile_remote(
-    model_id: str = typer.Option(..., "-m", "--model-id", help="Model identifier."),
-    resource: str = typer.Option(False, "--resource", "-r", help="Remote profiling on the given resource."),
-):
-    """Profile model on remote cluster."""
-    profile_remote(model_id=model_id, resource=resource)
-
-
 @profile_cli.command(name="model")
 def _profile_model(
     model_id: str = typer.Option(..., "-m", "--model-id", help="Model identifier."),
     device_id: int = typer.Option(0, "--device-id", "-d", help="Device ID to use."),
     verbose: bool = typer.Option(False, "--verbose", "-v", help="Verbose profiling."),
-    remote: str = typer.Option(False, "--remote", "-r", help="Remote profiling on the given resource."),
     catalog_path: str = typer.Option(None, "--catalog-path", "-e", help="Export path for the catalog json."),
 ):
     """Profile a specific model by its identifier."""
-    profile_models(model_id, device_id=device_id, save=True, verbose=verbose, remote=remote, catalog_path=catalog_path)
+    profile_models(model_id, device_id=device_id, save=True, verbose=verbose, catalog_path=catalog_path)
 
 
 @profile_cli.command(name="method")
 def _profile_method(
     method_name: str = typer.Option(..., "-m", "--method-name", help="Method name."),
     device_id: int = typer.Option(0, "--device-id", "-d", help="Device ID to use."),
     verbose: bool = typer.Option(False, "--verbose", "-v", help="Verbose profiling."),
```

## nos/cli/serve.py

```diff
@@ -297,15 +297,15 @@
         # Render the dockerfiles
         # agipack is responsible for the "images" sections
         # which are rendered into Dockerfiles and docker-compose files.
         builder = AGIPack(config)
         dockerfiles: Dict[str, Path] = builder.render(
             filename=str(NOS_SERVE_TMP_DIR / f"Dockerfile.{sandbox_name}"),
             env="prod" if prod else "dev",
-            skip_base_builds=True,
+            skip_base_builds=False,
         )
 
         # Check if several targets are defined, if so, expect the user
         # to specify which one to build / serve
         if len(dockerfiles) > 1 and target is None:
             raise ValueError(
                 f"Several targets defined in the config, please specify which one to "
```

## nos/cli/templates/docker-compose.serve.yml.j2

```diff
@@ -27,21 +27,14 @@
         {%- endfor %}
       {%- endif %}
     ports:
       - {{ http_port }}:{{ http_port }}
     ipc: host
     depends_on:
       - nos-server
-{%- if runtime == 'gpu' %}
-    deploy:
-      resources:
-        reservations:
-          devices:
-            - capabilities: [gpu]
-{% endif %}
 {% endif %}
   nos-server:
     image: {{ image }}
     {%- if config %}
     command: nos-grpc-server -c {{ config }}
     {%- endif %}
     environment:
```

## nos/common/profiler.py

```diff
@@ -506,17 +506,17 @@
         )
         self.profiling_data.save(profile_path)
 
         # Still need to copy to the default catalog path for now
         from nos.constants import NOS_PROFILE_CATALOG_PATH
 
         shutil.copyfile(str(profile_path), str(NOS_PROFILE_CATALOG_PATH))
- 
+
         # This is a WIP to allow us to map the profiling catalog to a
         # filemount when running in GCP etc.
-        if catalog_path is not None and not Path(catalog_path).exists():
+        if catalog_path is not None:
             # Copy the profile to the metadata catalog
             Path(catalog_path).mkdir(parents=True, exist_ok=True)
             full_catalog_path = Path(catalog_path) / profile_path.name
             shutil.copyfile(str(profile_path), str(Path(full_catalog_path)))
 
         return str(profile_path)
```

## nos/server/http/_service.py

```diff
@@ -17,15 +17,14 @@
 
 from nos.client import Client
 from nos.common.tasks import TaskType
 from nos.constants import DEFAULT_GRPC_ADDRESS
 from nos.logging import logger
 from nos.protoc import import_module
 from nos.version import __version__
-from nos.cli.profile import profile_models
 
 from ._utils import decode_item, encode_item
 from .integrations.openai.models import (
     ChatCompletionsRequest,
     ChatModel,
     Choice,
     Completion,
@@ -209,15 +208,15 @@
             raise HTTPException(status_code=400, detail=f"Invalid model {model}")
 
     @app.post(f"/{version}/chat/completions", status_code=status.HTTP_201_CREATED)
     def chat(
         request: ChatCompletionsRequest,
         client: Client = Depends(get_client),
     ) -> StreamingResponse:
-        # Perform chat completion on the given input data.
+        """Perform chat completion on the given input data."""
         logger.debug(f"Received chat request [model={request.model}, messages={request.messages}]")
         _model_table = build_model_table(client)
         model_id: str = unnormalize_id(request.model)
         try:
             _ = _model_table[model_id]
         except KeyError:
             raise HTTPException(status_code=400, detail=f"Invalid model {request.model}")
@@ -230,15 +229,15 @@
             raise HTTPException(status_code=400, detail="Invalid chat request, last message must be from the user")
 
         # Perform chat completion (streaming)
         messages = [message.dict() for message in request.messages]
         if request.stream:
 
             def openai_streaming_generator():
-                # Streaming generator for OpenAI chat completion.
+                """Streaming generator for OpenAI chat completion."""
                 # Add responses incrementally to the chat
                 choices = [DeltaChoice(delta=DeltaRole(content="", role="assistant"), index=0, finish_reason=None)]
                 yield f"data: {Completion(id=request.id, object='chat.completion.chunk', model=request.model, choices=choices).json()}\n\n"
                 for response in model.chat(
                     messages=messages,
                     max_new_tokens=request.max_tokens,
                     _stream=True,
@@ -456,50 +455,17 @@
         else:
             try:
                 return JSONResponse(content=encode_item(response), status_code=status.HTTP_201_CREATED)
             except Exception as e:
                 logger.exception(f"Failed to encode response [type={type(response)}, e={e}]")
                 raise HTTPException(status_code=500, detail="Image generation failed")
 
-
-    @app.post(f"/{version}/profile", status_code=status.HTTP_201_CREATED)
-    def profile(
-        model_id: str = Form(...),
-        # method: Optional[str] = Form(None),
-        # file: Optional[UploadFile] = File(None),
-        # url: Optional[str] = Form(None),
-        # client: Client = Depends(get_client),
-    ) -> JSONResponse:
-        """Profile the given input data using multipart/form-data.
-
-        $ curl -X POST \
-            'http://localhost:8000/v1/profile \
-            -H 'accept: application/json' \
-            -H 'Content-Type: multipart/form-data' \
-            -F 'model_id=yolox/small' \
-            -F '
-        """
-
-        # Construct a profiling request and send it to the nos profiler:
-
-        # check the number of cuda devices with torch:
-        import torch
-        if torch.cuda.is_available():
-            print(torch.cuda.device_count())
-        else:
-            print("No cuda devices available")
-
-        from nos.constants import NOS_PROFILE_CATALOG_PATH
-
-        _, catlog_path = profile_models(model_id=model_id, save=True, catalog_path=NOS_PROFILE_CATALOG_PATH)
-
-        return JSONResponse(content={"catlog_path": str(catlog_path)}, status_code=status.HTTP_201_CREATED)
-
     return app
 
+
 def main():
     """Main entrypoint for the NOS REST API service / gateway."""
     import argparse
 
     import uvicorn
 
     from nos.constants import DEFAULT_HTTP_HOST, DEFAULT_HTTP_PORT
```

## Comparing `torch_nos-0.2.0a0.dist-info/LICENSE` & `torch_nos-0.2.0b0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `torch_nos-0.2.0a0.dist-info/METADATA` & `torch_nos-0.2.0b0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch-nos
-Version: 0.2.0a0
+Version: 0.2.0b0
 Summary: Nitrous Oxide for your AI Infrastructure.
 License: Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
         
            TERMS AND CONDITIONS FOR USE, REPRODUCTION, AND DISTRIBUTION
         
@@ -253,16 +253,14 @@
 Requires-Dist: huggingface-hub >=0.17.3 ; extra == 'all'
 Requires-Dist: pyarrow >=12.0.0 ; extra == 'all'
 Requires-Dist: ray[default] >=2.9.1 ; extra == 'all'
 Requires-Dist: safetensors >=0.3.0 ; extra == 'all'
 Requires-Dist: tabulate ; extra == 'all'
 Requires-Dist: timm >=0.9.2 ; extra == 'all'
 Requires-Dist: transformers >=4.35.0 ; extra == 'all'
-Requires-Dist: skypilot-nightly[gcp] ; extra == 'all'
-Requires-Dist: pytest ; extra == 'all'
 Requires-Dist: torch >=2.0.1 ; extra == 'all'
 Requires-Dist: torchaudio ; extra == 'all'
 Requires-Dist: torchvision ; extra == 'all'
 Requires-Dist: fastapi ; extra == 'all'
 Requires-Dist: uvicorn[standard] ; extra == 'all'
 Provides-Extra: cpu
 Provides-Extra: dev
@@ -287,27 +285,23 @@
 Requires-Dist: mkdocstrings ; extra == 'docs'
 Requires-Dist: mkdocstrings-python ; extra == 'docs'
 Requires-Dist: mkdocstrings[python] ; extra == 'docs'
 Provides-Extra: gpu
 Provides-Extra: http
 Requires-Dist: fastapi ; extra == 'http'
 Requires-Dist: uvicorn[standard] ; extra == 'http'
-Requires-Dist: skypilot-nightly[gcp] ; extra == 'http'
-Requires-Dist: pytest ; extra == 'http'
 Provides-Extra: server
 Requires-Dist: diffusers >=0.17.1 ; extra == 'server'
 Requires-Dist: huggingface-hub >=0.17.3 ; extra == 'server'
 Requires-Dist: pyarrow >=12.0.0 ; extra == 'server'
 Requires-Dist: ray[default] >=2.9.1 ; extra == 'server'
 Requires-Dist: safetensors >=0.3.0 ; extra == 'server'
 Requires-Dist: tabulate ; extra == 'server'
 Requires-Dist: timm >=0.9.2 ; extra == 'server'
 Requires-Dist: transformers >=4.35.0 ; extra == 'server'
-Requires-Dist: skypilot-nightly[gcp] ; extra == 'server'
-Requires-Dist: pytest ; extra == 'server'
 Requires-Dist: torch >=2.0.1 ; extra == 'server'
 Requires-Dist: torchaudio ; extra == 'server'
 Requires-Dist: torchvision ; extra == 'server'
 Provides-Extra: test
 Requires-Dist: httpx ; extra == 'test'
 Requires-Dist: pytest ; extra == 'test'
 Requires-Dist: pytest-asyncio ; extra == 'test'
```

## Comparing `torch_nos-0.2.0a0.dist-info/RECORD` & `torch_nos-0.2.0b0.dist-info/RECORD`

 * *Files 25% similar despite different names*

```diff
@@ -1,32 +1,32 @@
 nos/__init__.py,sha256=qNlh5FXCaooUrODrcPiHY_yK9NwtRFLCTsN4FLGRVFQ,424
 nos/constants.py,sha256=ZWv5a3CP0IqZljnPnElohGJqmvQXIDxvlfpNqlSQgQo,1951
 nos/exceptions.py,sha256=i3SD26SIgCIpDq2hSJ3Tt_ECgwbK-5p3ZbjGY0lcOQw,750
 nos/logging.py,sha256=IkkbLtVKUFg6hbECKOBUUzozDdlwJ2MpmlRn6NxzbIQ,2295
 nos/protoc.py,sha256=_VoBlDRZozu1vmhnJ65SsEHOfedbHW0_SlB6NWUgI9Q,3199
 nos/telemetry.py,sha256=KclGHUUBC7x1aviM-62dUMT5SrA9IhlqY9j4Bdvw6t8,1436
-nos/version.py,sha256=XjyJiDibDV_Z51ez3mi17tJbHaMxh3JTg26NJv2NY80,23
+nos/version.py,sha256=jaXChwfIgwjM8CGVXQS3V5mfoUdkBU_6vPxsrLg-QJc,23
 nos/catalogs/model_profile_catalog.json,sha256=fp2ec-MwGFNXoHhc4Vws1pY87TrTWr2eNypeGXLfU60,1898
 nos/cli/cli.py,sha256=H-X2g7g1qtFGHTnsmUNE-9ZnO3sC8Ys3QrI-Hty3SLc,858
 nos/cli/hub.py,sha256=apjVHOka3ltxdTZC31HSCZK47a6Ou2O5TlpzQNY_gz8,1417
 nos/cli/predict.py,sha256=acD1ZDOC-phJIKSuBzyOw8TEaNlcFT-Gq92NUozyca0,7330
-nos/cli/profile.py,sha256=1dwXyJo_-N0svD-pAoOWbToD4nI638_MeOxN2tIZ39s,19039
-nos/cli/serve.py,sha256=el0FElTJ7RTSZwR34gJ65BoZWOgIKyZVMbNkdc5Mk2A,19109
+nos/cli/profile.py,sha256=ZYqprxKqDMtgsu1Mi0l9a7ovXFyOUPQ7D4ShLe-uqTI,13556
+nos/cli/serve.py,sha256=MBNbneaeFFLkI3Jwv8xNSkYVTSLDMJQgJXLLOpHhixc,19110
 nos/cli/system.py,sha256=oeAN6WA1IdhlIR89cnW1xFhd8HEAZLl15TcwucsojSI,1838
 nos/cli/utils.py,sha256=uR1lGZyyDEuflNvxKuAmVUP-DTE55PzZL5c0c3l2h4U,425
-nos/cli/templates/docker-compose.serve.yml.j2,sha256=JsRCd__VGfLo5HpmbH5oNn3MXc3Gk6a8WOUo_1P54I8,1979
+nos/cli/templates/docker-compose.serve.yml.j2,sha256=CnD0dlpLhV79En_aC0pMhC1_DaheiBg779Qj1CV0nwM,1836
 nos/client/__init__.py,sha256=cGqTR-ItKRYX-3FNxc7EL6ex0gAuvYLev8jSJrVZhOk,398
 nos/client/grpc.py,sha256=8hQgZ12ZZrhgv6t-XmHZ6ceK8LjaSxoeE2Ivbuuildk,30281
 nos/common/__init__.py,sha256=-GcgzkFF8jP5bGOK0Y8AANC2wtiRIbtY2EkcGS3ZcaM,3094
 nos/common/cloudpickle.py,sha256=2VBtGaLHbVtKg9ICT-xUITweHQCd6PxsFobDKwSYE2I,204
 nos/common/exceptions.py,sha256=zP8v9dm4gFTLoCr6bKHS1TuIm2CcF4h51hJmSrp7e3s,906
 nos/common/git.py,sha256=cd-m0WkUEhVDdqNdcUAg_hVbX4SuFkev0ONkPebLe1I,5154
 nos/common/helpers.py,sha256=6wb1I6XlY2cvWG_i5LHSRbrwpRwsX7rKaqgRhginTSE,1028
 nos/common/metaclass.py,sha256=Yhicnnff8uppLxjF63rqvSnS5AxMIfTDfOsqztJMiE8,499
-nos/common/profiler.py,sha256=QlHP4_NtKSuOrGMlzPKv3IiVcRgFnIQ4RW_h76dq7IY,20848
+nos/common/profiler.py,sha256=IBoK0fsiAo5HAEV3vdSEZxll83o4Bl_PQTnh3uuR1Uc,20811
 nos/common/runtime.py,sha256=yXPFjp4oeB-hno5Yuzkx-_B7gRER9xZRf3L32bpE-gA,805
 nos/common/shm.py,sha256=k5WLv4vUVifIRyhGQPT6LAI9IhmuU5W6Azukns0u_PE,11842
 nos/common/spec.py,sha256=ARJ-CyJY8Cv8khGen8OLrEUyYz53LbdTSVkcWULJ5s0,31844
 nos/common/system.py,sha256=KPPsH36RVZEMRZ9vbi0ty3927kfpnRDg8hzBQ2y6IR8,7930
 nos/common/tasks.py,sha256=b_7DMIV7rlhWOgNO1jx0_HSNTPX6MZsOCfASv8Laakw,830
 nos/common/types.py,sha256=kZYYI6b-u1xvOsiM0e02tENIQZwauCGcCcKwZXC7ZY8,6117
 nos/common/io/__init__.py,sha256=XLg1aKxI3GKObzvb437Ht0PId1mvrA9tmiyHFMg04Yk,1465
@@ -66,37 +66,26 @@
 nos/neuron/device.py,sha256=UhDtot6HG3B1z4oa780juuEWVUsnd2uKU6NMYLAv9Vo,1284
 nos/proto/nos_service.proto,sha256=eue7x4XWSEJCI7CQFVlmnwtmYGKoSyCnpo58rFkcths,1895
 nos/server/__init__.py,sha256=8o9wTyD4DvdntWHRedVGCoszjt7ON6-LgodlRcQXZSM,10483
 nos/server/_docker.py,sha256=hXRH1m_iI5v8z60n36cDdMbxs_I_uJ6517paFPwQJLw,7341
 nos/server/_runtime.py,sha256=lyIb9NS3ceYUxasvXwadU_43PyKNOIuSKz5KAcIhdzY,9632
 nos/server/_service.py,sha256=CELEBP110vyhwwqmjZAPD6iwA8i9LtT6JkjRRzv2OxA,20201
 nos/server/http/__init__.py,sha256=3HBNsYRdbgLgn6mug36-UxeMxtKa81ZDbqT_54ktng0,83
-nos/server/http/_service.py,sha256=r57pKqFJcOwpvTftLtXx9yy63ZEDj8z8fpttIHs6CzI,21273
+nos/server/http/_service.py,sha256=h1Puk1aAQDWE0VtWmtmafmBbIYu4FH6Dxv0AjtW3uT4,20019
 nos/server/http/_utils.py,sha256=x6ndk5ONVxuoC9GKQD25chXvHMa3hbe_qlyzjNaXMNo,2865
 nos/server/http/integrations/openai/models.py,sha256=FYCdFLDDL2DPKB6bz6ZzNCz_C4p6H3Geqr-6rjVeNgk,4223
 nos/test/benchmark.py,sha256=b_QMHfStY5iRjHGPZwaY7VrXzy_VeFKfjld9UEVbn-g,373
 nos/test/conftest.py,sha256=3eama-JQx3R92n3MltQA1FkO7KF2ih3IV7wog8jsSYU,10761
 nos/test/utils.py,sha256=Lal3t2U-B5YgGzvKynTMoWN9Z12Jok52tlAt_IG2T7E,2749
 nos/test/test_data/test.jpg,sha256=jpqxNdp-rKve7u4Rukt7zdG_rBKM-Sqd6cefmEBgrh4,259865
 nos/test/test_data/test.mp4,sha256=uDyQB1PSe7jQ1QvON3EReYUGtQYvh69w9RBzA5ILun8,300601
 nos/test/test_data/test_speech.flac,sha256=Y6Sx5MHcZVrHCWH_v1GKzSSd8jfloBUvqumkqDaUlxU,1152693
-nos/test/test_data/hub/custom_model/Dockerfile.custom_model,sha256=aGHNdp0C6zMqTO72FXaclMOg_LxcvxQrgsUhZxb14Sk,1163
-nos/test/test_data/hub/custom_model/config-alternate-init-kwargs.yaml,sha256=xQMi5_PxJNrBvf-b25KiDhXsBQnnRn1OEyamgADe5O8,185
-nos/test/test_data/hub/custom_model/config-malformed-model-cls.yaml,sha256=joElYOKjvJmmSisL8lf3h8uSRZ7bnJoYlf9NAqlL3Zk,159
-nos/test/test_data/hub/custom_model/config-malformed-model-method.yaml,sha256=L0pj0SoLSoQhC_WmCM28uguhtoTuVgqaohVLsk72Umg,162
-nos/test/test_data/hub/custom_model/config-malformed-model-path.yaml,sha256=gdVQ1QSwWaDHCDuuDEU6nKN_2YhI88qwKIilxszLR_Y,160
-nos/test/test_data/hub/custom_model/config-with-existing-model-id.yaml,sha256=KrJwwyUBwxbFZ6fYV8eWKOXdRl8ficH94gq5sRflRYk,430
-nos/test/test_data/hub/custom_model/config-with-replicas.yaml,sha256=d_gv7zkEQYDYLEFNJ6m9K8DMMDd5_ug6GVwIPA-dWrg,654
-nos/test/test_data/hub/custom_model/config.yaml,sha256=bwl8YZ7QkXQyWWP5sgxtx7CSrp1nFH33E2u6XD_Ca8o,353
-nos/test/test_data/hub/custom_model/docker-compose.animatediff.yml,sha256=NEyLHsG5Yu7YQtSbAXa1zX6xbCu-hgORr7Sr0GlPGHc,900
-nos/test/test_data/hub/custom_model/docker-compose.custom_model.yml,sha256=JDdJy8Na2qk8dpaw2mQzf8HwwS5604CQRlHTtBSMF8k,993
 nos/test/test_data/hub/custom_model/models/model.py,sha256=D4pGZtlMBN8mvbgyKSfmDgUcEmCnAsr95jGUfG9AtWY,178
-nos/test/test_data/hub/custom_model/scripts/entrypoint.sh,sha256=a0EAN9SENH4ybHxYkeiGA_K5dgMxuInrRv_S9ePN5xw,332
 nos-profiling-catalogs/nos-profile--0-1-4a--20240122--nvidia-geforce-rtx-2080.json,sha256=Aoe0GM0D4MY7mRmY_95qqJi6j4y4m5J_MRhMSAaW6RI,2101
 nos-profiling-catalogs/nos-profile--0-1-5--20240123--nvidia-geforce-rtx-2080.json,sha256=YeGfIx29NGhtuw6oJSvRgZTJq5Wo-Ig13LBipQzvmhU,2086
 scripts/nos_bot.py,sha256=JjbzNCT9caxk2wYnKEk1ZUehVO-enzdiwHPGqAeTYbg,3006
-torch_nos-0.2.0a0.dist-info/LICENSE,sha256=Sx_bJsho4SrloBQw1plyToriX8KcfYwQ2RCBVd_UAjs,11355
-torch_nos-0.2.0a0.dist-info/METADATA,sha256=koXL3bKvY_zLDDSJ-oSQ74ZPIfxNeA_b6J56IlSB15k,27187
-torch_nos-0.2.0a0.dist-info/WHEEL,sha256=oiQVh_5PnQM0E3gPdiz09WCNmwiHDMaGer_elqB3coM,92
-torch_nos-0.2.0a0.dist-info/entry_points.txt,sha256=m5LWTBk_24bET1ibsIwOn_g3YUEM1ZSjTGpNkECt3iI,135
-torch_nos-0.2.0a0.dist-info/top_level.txt,sha256=IS9ghqe2qZFvEB6T2r05Gm73sjL2DX62z9dSp4bd1-A,35
-torch_nos-0.2.0a0.dist-info/RECORD,,
+torch_nos-0.2.0b0.dist-info/LICENSE,sha256=Sx_bJsho4SrloBQw1plyToriX8KcfYwQ2RCBVd_UAjs,11355
+torch_nos-0.2.0b0.dist-info/METADATA,sha256=W-aVsDnMVlvkolaI5lguST160OZilxHs1r697CW4LWg,26900
+torch_nos-0.2.0b0.dist-info/WHEEL,sha256=GJ7t_kWBFywbagK5eo9IoUwLW6oyOeTKmQ-9iHFVNxQ,92
+torch_nos-0.2.0b0.dist-info/entry_points.txt,sha256=m5LWTBk_24bET1ibsIwOn_g3YUEM1ZSjTGpNkECt3iI,135
+torch_nos-0.2.0b0.dist-info/top_level.txt,sha256=1rEZQcaUw9uO6bbe6_8o_XGGTRnYsJeIeBhdfZen8po,74
+torch_nos-0.2.0b0.dist-info/RECORD,,
```

