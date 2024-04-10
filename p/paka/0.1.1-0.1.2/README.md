# Comparing `tmp/paka-0.1.1.tar.gz` & `tmp/paka-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paka-0.1.1.tar", max compression
+gzip compressed data, was "paka-0.1.2.tar", max compression
```

## Comparing `paka-0.1.1.tar` & `paka-0.1.2.tar`

### file list

```diff
@@ -1,55 +1,56 @@
--rw-r--r--   0        0        0     1072 2024-04-03 04:57:05.293202 paka-0.1.1/LICENSE
--rw-r--r--   0        0        0     4445 2024-04-03 04:57:05.293202 paka-0.1.1/README.md
--rw-r--r--   0        0        0       22 2024-04-03 04:57:05.293202 paka-0.1.1/paka/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cli/__init__.py
--rw-r--r--   0        0        0     1608 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cli/__main__.py
--rw-r--r--   0        0        0     1141 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cli/build.py
--rw-r--r--   0        0        0     2793 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cli/cluster.py
--rw-r--r--   0        0        0     6690 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cli/function.py
--rw-r--r--   0        0        0     5874 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cli/job.py
--rw-r--r--   0        0        0      427 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cli/kubeconfig.py
--rw-r--r--   0        0        0     2197 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cli/model_group.py
--rw-r--r--   0        0        0     3188 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cli/run.py
--rw-r--r--   0        0        0     8779 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cli/utils.py
--rw-r--r--   0        0        0        0 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/__init__.py
--rw-r--r--   0        0        0        0 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/aws/__init__.py
--rw-r--r--   0        0        0     1037 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/aws/cloudwatch.py
--rw-r--r--   0        0        0     3113 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/aws/cluster_autoscaler.py
--rw-r--r--   0        0        0      722 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/aws/container_registry.py
--rw-r--r--   0        0        0     2521 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/aws/ebs_csi_driver.py
--rw-r--r--   0        0        0    11885 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/aws/eks.py
--rw-r--r--   0        0        0     1432 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/aws/elb.py
--rw-r--r--   0        0        0      725 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/aws/object_store.py
--rw-r--r--   0        0        0     4078 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/aws/service_account.py
--rw-r--r--   0        0        0     1874 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/aws/utils.py
--rw-r--r--   0        0        0     4643 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/fluentbit.py
--rw-r--r--   0        0        0     1228 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/keda.py
--rw-r--r--   0        0        0     4920 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/knative.py
--rw-r--r--   0        0        0        0 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/manager/__init__.py
--rw-r--r--   0        0        0     1210 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/manager/aws.py
--rw-r--r--   0        0        0     2737 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/manager/base.py
--rw-r--r--   0        0        0      879 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/namespace.py
--rw-r--r--   0        0        0     4237 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/prometheus.py
--rw-r--r--   0        0        0     4000 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/qdrant.py
--rw-r--r--   0        0        0     2325 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/redis.py
--rw-r--r--   0        0        0      935 2024-04-03 04:57:05.293202 paka-0.1.1/paka/cluster/zipkin.py
--rw-r--r--   0        0        0    13265 2024-04-03 04:57:05.293202 paka-0.1.1/paka/config.py
--rw-r--r--   0        0        0      115 2024-04-03 04:57:05.293202 paka-0.1.1/paka/constants.py
--rw-r--r--   0        0        0     3015 2024-04-03 04:57:05.293202 paka-0.1.1/paka/container/ecr.py
--rw-r--r--   0        0        0     2374 2024-04-03 04:57:05.293202 paka-0.1.1/paka/container/pack.py
--rw-r--r--   0        0        0    18963 2024-04-03 04:57:05.293202 paka-0.1.1/paka/k8s.py
--rw-r--r--   0        0        0        0 2024-04-03 04:57:05.293202 paka-0.1.1/paka/kube_resources/function/__init__.py
--rw-r--r--   0        0        0     5706 2024-04-03 04:57:05.293202 paka-0.1.1/paka/kube_resources/function/service.py
--rw-r--r--   0        0        0        0 2024-04-03 04:57:05.293202 paka-0.1.1/paka/kube_resources/job/__init__.py
--rw-r--r--   0        0        0     2342 2024-04-03 04:57:05.293202 paka-0.1.1/paka/kube_resources/job/autoscaler.py
--rw-r--r--   0        0        0     4142 2024-04-03 04:57:05.293202 paka-0.1.1/paka/kube_resources/job/worker.py
--rw-r--r--   0        0        0        0 2024-04-03 04:57:05.293202 paka-0.1.1/paka/kube_resources/model_group/__init__.py
--rw-r--r--   0        0        0     2012 2024-04-03 04:57:05.293202 paka-0.1.1/paka/kube_resources/model_group/ingress.py
--rw-r--r--   0        0        0      131 2024-04-03 04:57:05.293202 paka-0.1.1/paka/kube_resources/model_group/manifest.py
--rw-r--r--   0        0        0     9969 2024-04-03 04:57:05.293202 paka-0.1.1/paka/kube_resources/model_group/model.py
--rw-r--r--   0        0        0    16598 2024-04-03 04:57:05.293202 paka-0.1.1/paka/kube_resources/model_group/service.py
--rw-r--r--   0        0        0     1105 2024-04-03 04:57:05.293202 paka-0.1.1/paka/kube_resources/model_group/supported_models.py
--rw-r--r--   0        0        0      761 2024-04-03 04:57:05.293202 paka-0.1.1/paka/logger.py
--rw-r--r--   0        0        0     9750 2024-04-03 04:57:05.293202 paka-0.1.1/paka/utils.py
--rw-r--r--   0        0        0     1262 2024-04-03 04:57:05.293202 paka-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5410 1970-01-01 00:00:00.000000 paka-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1072 2024-04-10 23:12:18.012434 paka-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4429 2024-04-10 23:12:18.012434 paka-0.1.2/README.md
+-rw-r--r--   0        0        0      153 2024-04-10 23:12:18.016434 paka-0.1.2/paka/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cli/__init__.py
+-rw-r--r--   0        0        0     1608 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cli/__main__.py
+-rw-r--r--   0        0        0     1141 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cli/build.py
+-rw-r--r--   0        0        0     3227 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cli/cluster.py
+-rw-r--r--   0        0        0     6690 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cli/function.py
+-rw-r--r--   0        0        0     5874 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cli/job.py
+-rw-r--r--   0        0        0      427 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cli/kubeconfig.py
+-rw-r--r--   0        0        0     2197 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cli/model_group.py
+-rw-r--r--   0        0        0     3188 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cli/run.py
+-rw-r--r--   0        0        0     8779 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cli/utils.py
+-rw-r--r--   0        0        0        0 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/aws/__init__.py
+-rw-r--r--   0        0        0     1037 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/aws/cloudwatch.py
+-rw-r--r--   0        0        0     3113 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/aws/cluster_autoscaler.py
+-rw-r--r--   0        0        0      722 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/aws/container_registry.py
+-rw-r--r--   0        0        0     2521 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/aws/ebs_csi_driver.py
+-rw-r--r--   0        0        0    12118 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/aws/eks.py
+-rw-r--r--   0        0        0     1432 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/aws/elb.py
+-rw-r--r--   0        0        0      725 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/aws/object_store.py
+-rw-r--r--   0        0        0     4078 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/aws/service_account.py
+-rw-r--r--   0        0        0     1874 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/aws/utils.py
+-rw-r--r--   0        0        0     4643 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/fluentbit.py
+-rw-r--r--   0        0        0     1228 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/keda.py
+-rw-r--r--   0        0        0     4920 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/knative.py
+-rw-r--r--   0        0        0        0 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/manager/__init__.py
+-rw-r--r--   0        0        0     1210 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/manager/aws.py
+-rw-r--r--   0        0        0     2737 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/manager/base.py
+-rw-r--r--   0        0        0      879 2024-04-10 23:12:18.016434 paka-0.1.2/paka/cluster/namespace.py
+-rw-r--r--   0        0        0     3414 2024-04-10 23:12:18.020434 paka-0.1.2/paka/cluster/nvidia_device_plugin.py
+-rw-r--r--   0        0        0     4237 2024-04-10 23:12:18.020434 paka-0.1.2/paka/cluster/prometheus.py
+-rw-r--r--   0        0        0     4000 2024-04-10 23:12:18.020434 paka-0.1.2/paka/cluster/qdrant.py
+-rw-r--r--   0        0        0     2325 2024-04-10 23:12:18.020434 paka-0.1.2/paka/cluster/redis.py
+-rw-r--r--   0        0        0      935 2024-04-10 23:12:18.020434 paka-0.1.2/paka/cluster/zipkin.py
+-rw-r--r--   0        0        0    15359 2024-04-10 23:12:18.020434 paka-0.1.2/paka/config.py
+-rw-r--r--   0        0        0      115 2024-04-10 23:12:18.020434 paka-0.1.2/paka/constants.py
+-rw-r--r--   0        0        0     3015 2024-04-10 23:12:18.020434 paka-0.1.2/paka/container/ecr.py
+-rw-r--r--   0        0        0     2374 2024-04-10 23:12:18.020434 paka-0.1.2/paka/container/pack.py
+-rw-r--r--   0        0        0    19164 2024-04-10 23:12:18.020434 paka-0.1.2/paka/k8s.py
+-rw-r--r--   0        0        0        0 2024-04-10 23:12:18.020434 paka-0.1.2/paka/kube_resources/function/__init__.py
+-rw-r--r--   0        0        0     5706 2024-04-10 23:12:18.020434 paka-0.1.2/paka/kube_resources/function/service.py
+-rw-r--r--   0        0        0        0 2024-04-10 23:12:18.020434 paka-0.1.2/paka/kube_resources/job/__init__.py
+-rw-r--r--   0        0        0     2342 2024-04-10 23:12:18.020434 paka-0.1.2/paka/kube_resources/job/autoscaler.py
+-rw-r--r--   0        0        0     4142 2024-04-10 23:12:18.020434 paka-0.1.2/paka/kube_resources/job/worker.py
+-rw-r--r--   0        0        0        0 2024-04-10 23:12:18.020434 paka-0.1.2/paka/kube_resources/model_group/__init__.py
+-rw-r--r--   0        0        0     2012 2024-04-10 23:12:18.020434 paka-0.1.2/paka/kube_resources/model_group/ingress.py
+-rw-r--r--   0        0        0      131 2024-04-10 23:12:18.020434 paka-0.1.2/paka/kube_resources/model_group/manifest.py
+-rw-r--r--   0        0        0     9969 2024-04-10 23:12:18.020434 paka-0.1.2/paka/kube_resources/model_group/model.py
+-rw-r--r--   0        0        0    17462 2024-04-10 23:12:18.020434 paka-0.1.2/paka/kube_resources/model_group/service.py
+-rw-r--r--   0        0        0     1105 2024-04-10 23:12:18.020434 paka-0.1.2/paka/kube_resources/model_group/supported_models.py
+-rw-r--r--   0        0        0      761 2024-04-10 23:12:18.020434 paka-0.1.2/paka/logger.py
+-rw-r--r--   0        0        0     9750 2024-04-10 23:12:18.020434 paka-0.1.2/paka/utils.py
+-rw-r--r--   0        0        0     1262 2024-04-10 23:12:18.020434 paka-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5394 1970-01-01 00:00:00.000000 paka-0.1.2/PKG-INFO
```

### Comparing `paka-0.1.1/LICENSE` & `paka-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/README.md` & `paka-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 <img src="docs/img/paka.svg" alt="paka.svg" width="200" height="200">
 
 **paka** is a versatile LLMOps tool that simplifies the deployment and management of large language model (LLM) apps with a single command.
 
 ## Paka Highlights
 
 - **Cloud-Agnostic Resource Provisioning**: paka starts by breaking down the barriers of cloud vendor lock-in, currently supporting EKS with plans to expand to more cloud services.
-- **Optimized Model Execution**: Designed for efficiency, paka runs LLM models on CPUs, with imminent support for GPUs, ensuring optimal performance. Auto-scaling of model replicas based on CPU usage, request rate, and latency.
+- **Optimized Model Execution**: Designed for efficiency, paka runs LLM models on CPUs and Nvidia GPUs, ensuring optimal performance. Auto-scaling of model replicas based on CPU usage, request rate, and latency.
 - **Scalable Batch Job Management**: paka excels in managing batch jobs that dynamically scale out and in, catering to varying workload demands without manual intervention.
 - **Seamless Application Deployment**: With support for running Langchain and LlamaIndex applications as functions, paka offers scalability to zero and back up, along with rolling updates to ensure no downtime.
 - **Comprehensive Monitoring and Tracing**: Embedded with built-in support for metrics collection via Prometheus and Grafana, along with tracing through Zipkin.
```

### Comparing `paka-0.1.1/paka/cli/__main__.py` & `paka-0.1.2/paka/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/cli/build.py` & `paka-0.1.2/paka/cli/build.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/cli/cluster.py` & `paka-0.1.2/paka/cli/cluster.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 from typing import List
 
 import click
 import typer
 
 from paka.cli.utils import load_cluster_manager
+from paka.k8s import remove_crd_finalizers
 from paka.k8s import update_kubeconfig as merge_update_kubeconfig
 from paka.logger import logger
 
 cluster_app = typer.Typer()
 
 
 @cluster_app.command()
@@ -60,14 +61,26 @@
     Tears down the Kubernetes cluster, removing all associated resources and data.
     """
     if yes or click.confirm(
         f"Are you sure you want to proceed with the operation? Please note that "
         "all resources and data will be permanently deleted.",
         default=False,
     ):
+        # Sometime finalizers might block CRD deletion, so we need to force delete those
+        # TODO: better way to handle this
+        remove_crd_finalizers(
+            "scaledobjects.keda.sh",
+        )
+        remove_crd_finalizers(
+            "routes.serving.knative.dev",
+        )
+        remove_crd_finalizers(
+            "ingresses.networking.internal.knative.dev",
+        )
+
         cluster_manager = load_cluster_manager(cluster_config)
         cluster_manager.destroy()
 
 
 @cluster_app.command()
 def preview(
     cluster_config: str = typer.Option(
```

### Comparing `paka-0.1.1/paka/cli/function.py` & `paka-0.1.2/paka/cli/function.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/cli/job.py` & `paka-0.1.2/paka/cli/job.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/cli/model_group.py` & `paka-0.1.2/paka/cli/model_group.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/cli/run.py` & `paka-0.1.2/paka/cli/run.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/cli/utils.py` & `paka-0.1.2/paka/cli/utils.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/cluster/aws/cloudwatch.py` & `paka-0.1.2/paka/cluster/aws/cloudwatch.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/cluster/aws/cluster_autoscaler.py` & `paka-0.1.2/paka/cluster/aws/cluster_autoscaler.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/cluster/aws/container_registry.py` & `paka-0.1.2/paka/cluster/aws/container_registry.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/cluster/aws/ebs_csi_driver.py` & `paka-0.1.2/paka/cluster/aws/ebs_csi_driver.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/cluster/aws/eks.py` & `paka-0.1.2/paka/cluster/aws/eks.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 from paka.cluster.aws.cluster_autoscaler import create_cluster_autoscaler
 from paka.cluster.aws.ebs_csi_driver import create_ebs_csi_driver
 from paka.cluster.aws.elb import update_elb_idle_timeout
 from paka.cluster.aws.service_account import create_service_accounts
 from paka.cluster.keda import create_keda
 from paka.cluster.knative import create_knative_and_istio
 from paka.cluster.namespace import create_namespace
+from paka.cluster.nvidia_device_plugin import install_nvidia_device_plugin
 from paka.cluster.prometheus import create_prometheus
 from paka.cluster.qdrant import create_qdrant
 from paka.cluster.redis import create_redis
 from paka.cluster.zipkin import create_zipkin
 from paka.config import CloudConfig
 from paka.utils import kubify_name, save_kubeconfig
 
@@ -75,40 +76,41 @@
     for model_group in config.modelGroups:
         # Create a managed node group for our cluster
         eks.ManagedNodeGroup(
             f"{project}-{kubify_name(model_group.name)}-group",
             node_group_name=f"{project}-{kubify_name(model_group.name)}-group",
             cluster=cluster,
             instance_types=[model_group.nodeType],
-            # Set the desired size of the node group to the minimum number of instances
-            # specified for the model group.
-            # Note: Scaling down to 0 is not supported, since cold starting time is
-            # too long for model group services.
             scaling_config=aws.eks.NodeGroupScalingConfigArgs(
                 desired_size=model_group.minInstances,
                 min_size=model_group.minInstances,
                 max_size=model_group.maxInstances,
             ),
             labels={
                 "size": model_group.nodeType,
                 "app": "model-group",
                 "model": model_group.name,
             },
             node_role_arn=worker_role.arn,
             subnet_ids=vpc.private_subnet_ids,
-            # Apply taints to ensure that only pods belonging to the same model group
-            # can be scheduled on this node group.
             taints=[
                 aws.eks.NodeGroupTaintArgs(
                     effect="NO_SCHEDULE", key="app", value="model-group"
                 ),
                 aws.eks.NodeGroupTaintArgs(
                     effect="NO_SCHEDULE", key="model", value=model_group.name
                 ),
             ],
+            # Supported AMI types https://docs.aws.amazon.com/eks/latest/APIReference/API_Nodegroup.html#AmazonEKS-Type-Nodegroup-amiType
+            ami_type=("AL2_x86_64_GPU" if model_group.awsGpu else None),
+            disk_size=(
+                model_group.awsGpu.diskSize
+                if model_group.awsGpu
+                else model_group.diskSize
+            ),
         )
 
 
 def create_node_group_for_qdrant(
     config: CloudConfig,
     cluster: eks.Cluster,
     vpc: awsx.ec2.Vpc,
@@ -297,14 +299,17 @@
         create_keda(config, k8s_provider)
         create_qdrant(config, k8s_provider)
 
         create_service_accounts(config, cluster, k8s_provider)
         enable_cloudwatch(config, k8s_provider)
         create_prometheus(config, k8s_provider)
         create_zipkin(config, k8s_provider)
+        # Install the NVIDIA device plugin for GPU support
+        # Even if the cluster doesn't have GPUs, this won't cause any issues
+        install_nvidia_device_plugin(k8s_provider)
 
         # TODO: Set timeout to be the one used by knative
         update_elb_idle_timeout(kubeconfig_json, 300)
 
     # Save the kubeconfig to a file
     cluster.kubeconfig_json.apply(create_eks_resources)
```

### Comparing `paka-0.1.1/paka/cluster/aws/elb.py` & `paka-0.1.2/paka/cluster/aws/elb.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/cluster/aws/object_store.py` & `paka-0.1.2/paka/cluster/aws/object_store.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/cluster/aws/service_account.py` & `paka-0.1.2/paka/cluster/aws/service_account.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/cluster/aws/utils.py` & `paka-0.1.2/paka/cluster/aws/utils.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/cluster/fluentbit.py` & `paka-0.1.2/paka/cluster/fluentbit.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/cluster/keda.py` & `paka-0.1.2/paka/cluster/keda.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/cluster/knative.py` & `paka-0.1.2/paka/cluster/knative.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/cluster/manager/aws.py` & `paka-0.1.2/paka/cluster/manager/aws.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/cluster/manager/base.py` & `paka-0.1.2/paka/cluster/manager/base.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/cluster/namespace.py` & `paka-0.1.2/paka/cluster/namespace.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/cluster/prometheus.py` & `paka-0.1.2/paka/cluster/prometheus.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/cluster/qdrant.py` & `paka-0.1.2/paka/cluster/qdrant.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/cluster/redis.py` & `paka-0.1.2/paka/cluster/redis.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/cluster/zipkin.py` & `paka-0.1.2/paka/cluster/zipkin.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/config.py` & `paka-0.1.2/paka/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 import re
-from typing import Any, Dict, List, Optional
+from typing import Any, Dict, List, Optional, Union
 
 from pydantic import BaseModel, field_validator, model_validator
 from ruamel.yaml import YAML
 
 from paka.utils import to_yaml
 
 
@@ -29,18 +29,20 @@
 class ResourceRequest(BaseModel):
     """
     Represents the resource request for a container.
 
     Attributes:
         cpu (str): The amount of CPU to request.
         memory (str): The amount of memory to request.
+        gpu (Optional[int]): The number of GPUs to request. Defaults to None.
     """
 
     cpu: str
     memory: str
+    gpu: Optional[int] = None
 
     @field_validator("cpu", mode="before")
     def validate_cpu(cls, v: str) -> str:
         """
         Validates the format of the cpu field.
 
         Args:
@@ -68,25 +70,86 @@
             str: The input value if validation is successful.
 
         Raises:
             ValueError: If the format of the input value is invalid.
         """
         return validate_size(v, "Invalid memory format")
 
+    @field_validator("gpu")
+    def validate_gpu(cls, v: Optional[int]) -> Optional[int]:
+        """
+        Validates the value of the gpu field.
+
+        Args:
+            v (Optional[int]): The value of the gpu field.
+
+        Returns:
+            Optional[int]: The input value if validation is successful.
+
+        Raises:
+            ValueError: If the value is less than 0.
+        """
+        if v is not None and v < 0:
+            raise ValueError("GPU count cannot be less than 0")
+        return v
+
+
+class AwsGpuNode(BaseModel):
+    """
+    Represents a configuration for an AWS GPU node.
+
+    Attributes:
+        diskSize (int): The size of the disk for the GPU node in GB.
+    """
+
+    diskSize: int
+
+
+class GcpGpuNode(BaseModel):
+    """
+    Represents a Google Cloud Platform GPU node.
+
+    Attributes:
+        imageType (str): The type of image used for the GPU node.
+        acceleratorType (str): The type of accelerator used for the GPU node.
+        acceleratorCount (int): The number of accelerators attached to the GPU node.
+        diskType (str): The type of disk used for the GPU node.
+        diskSize (int): The size of the disk attached to the GPU node in GB.
+    """
+
+    imageType: str
+    acceleratorType: str
+    acceleratorCount: int
+    diskType: str
+    diskSize: int
+
 
 class CloudNode(BaseModel):
     """
     Represents a node in the cloud cluster.
 
     Attributes:
         nodeType (str): The type of the node.
-
+        diskSize (int): The size of the disk attached to the node in GB.
+        awsGpu (Optional[AwsGpuNode]): The AWS GPU node configuration, if applicable.
+        gcpGpu (Optional[GcpGpuNode]): The GCP GPU node configuration, if applicable.
     """
 
     nodeType: str
+    diskSize: int = 20
+    awsGpu: Optional[AwsGpuNode] = None
+    gcpGpu: Optional[GcpGpuNode] = None
+
+    @model_validator(mode="before")
+    def validate_gpu(
+        cls, values: Dict[str, Union[AwsGpuNode, GcpGpuNode]]
+    ) -> Dict[str, Union[AwsGpuNode, GcpGpuNode]]:
+        if values.get("awsGpu") and values.get("gcpGpu"):
+            raise ValueError("At most one of awsGpu or gcpGpu can exist")
+        return values
 
 
 class ModelGroup(BaseModel):
     """
     Represents a group of VMs that serve the inference for a specific type of model.
 
     Attributes:
```

### Comparing `paka-0.1.1/paka/container/ecr.py` & `paka-0.1.2/paka/container/ecr.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/container/pack.py` & `paka-0.1.2/paka/container/pack.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/k8s.py` & `paka-0.1.2/paka/k8s.py`

 * *Files 1% similar despite different names*

```diff
@@ -617,9 +617,15 @@
         namespace=namespace,
         name=pod_name,
         container=container_name,
     ):
         logger.info(event)
 
 
+def remove_crd_finalizers(name: str) -> None:
+    api = client.ApiextensionsV1Api()
+    body = [{"op": "remove", "path": "/metadata/finalizers"}]
+    api.patch_custom_resource_definition(name, body)
+
+
 # Load the kubeconfig when this module is imported
 try_load_kubeconfig()
```

### Comparing `paka-0.1.1/paka/kube_resources/function/service.py` & `paka-0.1.2/paka/kube_resources/function/service.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/kube_resources/job/autoscaler.py` & `paka-0.1.2/paka/kube_resources/job/autoscaler.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/kube_resources/job/worker.py` & `paka-0.1.2/paka/kube_resources/job/worker.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/kube_resources/model_group/ingress.py` & `paka-0.1.2/paka/kube_resources/model_group/ingress.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/kube_resources/model_group/model.py` & `paka-0.1.2/paka/kube_resources/model_group/model.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/kube_resources/model_group/service.py` & `paka-0.1.2/paka/kube_resources/model_group/service.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,17 +4,20 @@
 
 from paka.config import CloudConfig, CloudModelGroup, Config
 from paka.constants import ACCESS_ALL_SA
 from paka.k8s import CustomResource, apply_resource, try_load_kubeconfig
 from paka.kube_resources.model_group.model import MODEL_PATH_PREFIX, download_model
 from paka.utils import kubify_name, read_cluster_data
 
-# We hardcode the image here for now
+# `latest` will be stale because of the `IfNotPresent` policy
+# We hardcode the image here for now, we can make it configurable later
 LLAMA_CPP_PYTHON_IMAGE = "ghcr.io/abetlen/llama-cpp-python:latest"
 
+LLAMA_CPP_PYTHON_CUDA = "jijunleng/llama-cpp-python-cuda:latest"
+
 try_load_kubeconfig()
 
 
 def init_aws(config: CloudConfig, model_group: CloudModelGroup) -> client.V1Container:
     """
     Initializes an AWS container for downloading a model from S3.
 
@@ -111,16 +114,17 @@
             client.V1VolumeMount(
                 name="model-data",
                 mount_path="/data",
             )
         ],
         "env": [
             client.V1EnvVar(
-                name="USE_MLOCK",  # Model weights are locked in RAM or not
-                value="0",
+                name="N_GPU_LAYERS",
+                # -1 means all layers are GPU layers, 0 means no GPU layers
+                value=("-1" if model_group.awsGpu else "0"),
             ),
             client.V1EnvVar(
                 name="MODEL",
                 value=f"/data/my_model.gguf",
             ),
             client.V1EnvVar(
                 name="PORT",
@@ -155,14 +159,25 @@
         container_args["resources"] = client.V1ResourceRequirements(
             requests={
                 "cpu": model_group.resourceRequest.cpu,
                 "memory": model_group.resourceRequest.memory,
             },
         )
 
+    if model_group.awsGpu:
+        if "resources" not in container_args:
+            container_args["resources"] = client.V1ResourceRequirements()
+        if container_args["resources"].limits is None:
+            container_args["resources"].limits = {}
+        gpu_count = 1
+        if model_group.resourceRequest and model_group.resourceRequest.gpu:
+            gpu_count = model_group.resourceRequest.gpu
+        # Ah, we only support nvidia GPUs for now
+        container_args["resources"].limits["nvidia.com/gpu"] = gpu_count
+
     return client.V1Pod(
         metadata=client.V1ObjectMeta(
             name=f"{kubify_name(model_group.name)}",
             namespace=namespace,
             labels={
                 "app": "model-group",
                 "model": model_group.name,
@@ -484,15 +499,21 @@
         raise ValueError("Only AWS is supported at this time")
 
     # Download the model to S3 first
     download_model(model_group.name)
 
     port = 8000
 
-    pod = create_pod(namespace, config, model_group, LLAMA_CPP_PYTHON_IMAGE, port)
+    pod = create_pod(
+        namespace,
+        config,
+        model_group,
+        (LLAMA_CPP_PYTHON_CUDA if model_group.awsGpu else LLAMA_CPP_PYTHON_IMAGE),
+        port,
+    )
 
     deployment = create_deployment(namespace, model_group, pod)
     apply_resource(deployment)
 
     svc = create_service(namespace, model_group, port)
     apply_resource(svc)
```

### Comparing `paka-0.1.1/paka/kube_resources/model_group/supported_models.py` & `paka-0.1.2/paka/kube_resources/model_group/supported_models.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/logger.py` & `paka-0.1.2/paka/logger.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/paka/utils.py` & `paka-0.1.2/paka/utils.py`

 * *Files identical despite different names*

### Comparing `paka-0.1.1/pyproject.toml` & `paka-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "paka"
-version = "0.1.1"
+version = "0.1.2"
 description = "LLMOps tool designed to simplify the deployment and management of large language model (LLM) applications"
 authors = ["Jijun Leng"]
 readme = "README.md"
 
 [tool.codespell]
 check-filenames = true
```

### Comparing `paka-0.1.1/PKG-INFO` & `paka-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paka
-Version: 0.1.1
+Version: 0.1.2
 Summary: LLMOps tool designed to simplify the deployment and management of large language model (LLM) applications
 Author: Jijun Leng
 Requires-Python: >=3.11,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.12
 Requires-Dist: boto3 (>=1.34.22,<2.0.0)
@@ -27,15 +27,15 @@
 <img src="docs/img/paka.svg" alt="paka.svg" width="200" height="200">
 
 **paka** is a versatile LLMOps tool that simplifies the deployment and management of large language model (LLM) apps with a single command.
 
 ## Paka Highlights
 
 - **Cloud-Agnostic Resource Provisioning**: paka starts by breaking down the barriers of cloud vendor lock-in, currently supporting EKS with plans to expand to more cloud services.
-- **Optimized Model Execution**: Designed for efficiency, paka runs LLM models on CPUs, with imminent support for GPUs, ensuring optimal performance. Auto-scaling of model replicas based on CPU usage, request rate, and latency.
+- **Optimized Model Execution**: Designed for efficiency, paka runs LLM models on CPUs and Nvidia GPUs, ensuring optimal performance. Auto-scaling of model replicas based on CPU usage, request rate, and latency.
 - **Scalable Batch Job Management**: paka excels in managing batch jobs that dynamically scale out and in, catering to varying workload demands without manual intervention.
 - **Seamless Application Deployment**: With support for running Langchain and LlamaIndex applications as functions, paka offers scalability to zero and back up, along with rolling updates to ensure no downtime.
 - **Comprehensive Monitoring and Tracing**: Embedded with built-in support for metrics collection via Prometheus and Grafana, along with tracing through Zipkin.
```

