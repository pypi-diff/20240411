# Comparing `tmp/python_sysinformer-1.5.0.tar.gz` & `tmp/python_sysinformer-1.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python_sysinformer-1.5.0.tar", max compression
+gzip compressed data, was "python_sysinformer-1.6.0.tar", max compression
```

## Comparing `python_sysinformer-1.5.0.tar` & `python_sysinformer-1.6.0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0    35149 2024-04-09 19:13:21.563897 python_sysinformer-1.5.0/LICENSE
--rw-r--r--   0        0        0     5341 2024-04-09 19:13:21.567897 python_sysinformer-1.5.0/README.md
--rw-r--r--   0        0        0     1593 2024-04-09 19:13:48.107782 python_sysinformer-1.5.0/pyproject.toml
--rw-r--r--   0        0        0        0 2024-04-09 19:13:21.567897 python_sysinformer-1.5.0/src/__init__.py
--rw-r--r--   0        0        0        0 2024-04-09 19:13:21.567897 python_sysinformer-1.5.0/src/config/__init__.py
--rw-r--r--   0        0        0     1102 2024-04-09 19:13:21.567897 python_sysinformer-1.5.0/src/config/config_parser.py
--rw-r--r--   0        0        0     1233 2024-04-09 19:13:21.567897 python_sysinformer-1.5.0/src/config/default_config.py
--rw-r--r--   0        0        0      221 2024-04-09 19:13:21.567897 python_sysinformer-1.5.0/src/constants.py
--rw-r--r--   0        0        0        0 2024-04-09 19:13:21.567897 python_sysinformer-1.5.0/src/core/__init__.py
--rw-r--r--   0        0        0     4448 2024-04-09 19:13:21.567897 python_sysinformer-1.5.0/src/core/containers.py
--rw-r--r--   0        0        0     5666 2024-04-09 19:13:21.567897 python_sysinformer-1.5.0/src/core/cpu.py
--rw-r--r--   0        0        0     2041 2024-04-09 19:13:21.571897 python_sysinformer-1.5.0/src/core/disks.py
--rw-r--r--   0        0        0     3745 2024-04-09 19:13:21.571897 python_sysinformer-1.5.0/src/core/latency.py
--rw-r--r--   0        0        0     4335 2024-04-09 19:13:21.571897 python_sysinformer-1.5.0/src/core/memory.py
--rw-r--r--   0        0        0     2597 2024-04-09 19:13:21.571897 python_sysinformer-1.5.0/src/core/networking.py
--rw-r--r--   0        0        0     2764 2024-04-09 19:13:21.571897 python_sysinformer-1.5.0/src/core/processes.py
--rw-r--r--   0        0        0     2605 2024-04-09 19:13:21.571897 python_sysinformer-1.5.0/src/core/services.py
--rw-r--r--   0        0        0     4035 2024-04-09 19:13:21.571897 python_sysinformer-1.5.0/src/core/system.py
--rw-r--r--   0        0        0     4417 2024-04-09 19:13:21.571897 python_sysinformer-1.5.0/src/main.py
--rw-r--r--   0        0        0        0 2024-04-09 19:13:21.571897 python_sysinformer-1.5.0/src/utilities/__init__.py
--rw-r--r--   0        0        0      442 2024-04-09 19:13:21.571897 python_sysinformer-1.5.0/src/utilities/exceptions.py
--rw-r--r--   0        0        0      560 2024-04-09 19:13:21.571897 python_sysinformer-1.5.0/src/utilities/utils.py
--rw-r--r--   0        0        0     6061 1970-01-01 00:00:00.000000 python_sysinformer-1.5.0/PKG-INFO
+-rw-r--r--   0        0        0    35149 2024-04-11 18:39:07.797460 python_sysinformer-1.6.0/LICENSE
+-rw-r--r--   0        0        0     5479 2024-04-11 18:39:07.797460 python_sysinformer-1.6.0/README.md
+-rw-r--r--   0        0        0     1593 2024-04-11 18:39:35.625689 python_sysinformer-1.6.0/pyproject.toml
+-rw-r--r--   0        0        0        0 2024-04-11 18:39:07.801460 python_sysinformer-1.6.0/src/__init__.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:39:07.801460 python_sysinformer-1.6.0/src/config/__init__.py
+-rw-r--r--   0        0        0     1102 2024-04-11 18:39:07.801460 python_sysinformer-1.6.0/src/config/config_parser.py
+-rw-r--r--   0        0        0     1233 2024-04-11 18:39:07.801460 python_sysinformer-1.6.0/src/config/default_config.py
+-rw-r--r--   0        0        0      221 2024-04-11 18:39:07.801460 python_sysinformer-1.6.0/src/constants.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:39:07.801460 python_sysinformer-1.6.0/src/core/__init__.py
+-rw-r--r--   0        0        0     4448 2024-04-11 18:39:07.801460 python_sysinformer-1.6.0/src/core/containers.py
+-rw-r--r--   0        0        0     6261 2024-04-11 18:39:07.801460 python_sysinformer-1.6.0/src/core/cpu.py
+-rw-r--r--   0        0        0     2041 2024-04-11 18:39:07.801460 python_sysinformer-1.6.0/src/core/disks.py
+-rw-r--r--   0        0        0     3745 2024-04-11 18:39:07.801460 python_sysinformer-1.6.0/src/core/latency.py
+-rw-r--r--   0        0        0     5730 2024-04-11 18:39:07.801460 python_sysinformer-1.6.0/src/core/memory.py
+-rw-r--r--   0        0        0     2597 2024-04-11 18:39:07.801460 python_sysinformer-1.6.0/src/core/networking.py
+-rw-r--r--   0        0        0     2764 2024-04-11 18:39:07.801460 python_sysinformer-1.6.0/src/core/processes.py
+-rw-r--r--   0        0        0     2605 2024-04-11 18:39:07.801460 python_sysinformer-1.6.0/src/core/services.py
+-rw-r--r--   0        0        0     4035 2024-04-11 18:39:07.801460 python_sysinformer-1.6.0/src/core/system.py
+-rw-r--r--   0        0        0     4417 2024-04-11 18:39:07.801460 python_sysinformer-1.6.0/src/main.py
+-rw-r--r--   0        0        0        0 2024-04-11 18:39:07.801460 python_sysinformer-1.6.0/src/utilities/__init__.py
+-rw-r--r--   0        0        0      442 2024-04-11 18:39:07.801460 python_sysinformer-1.6.0/src/utilities/exceptions.py
+-rw-r--r--   0        0        0      560 2024-04-11 18:39:07.801460 python_sysinformer-1.6.0/src/utilities/utils.py
+-rw-r--r--   0        0        0     6199 1970-01-01 00:00:00.000000 python_sysinformer-1.6.0/PKG-INFO
```

### Comparing `python_sysinformer-1.5.0/LICENSE` & `python_sysinformer-1.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.5.0/README.md` & `python_sysinformer-1.6.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -34,14 +34,17 @@
 
 ## Installation
 
 The easiest way to install the tool is with `pip`:
 
 ```bash
   pip install python-SysInformer
+
+  # if using pyenv - upgrade the tool with to avoid potential cache issues:
+  pip install --upgrade python-SysInformer --force-reinstall
 ```
 
 Additionaly, if you have [poetry](https://python-poetry.org/) installed you can install the tool with:
 
 ```bash
 git clone [this repo]
 poetry install
```

### Comparing `python_sysinformer-1.5.0/pyproject.toml` & `python_sysinformer-1.6.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-SysInformer"
-version = "1.5.0"
+version = "1.6.0"
 description = "A simple system information tool for Linux"
 authors = ["Timothy Bryant <timothybryant3@gmail.com>"]
 readme = "README.md"
 packages = [{include = "src", from = "."}]
 # classifiers = ["Private :: Do not Upload"]
 
 [tool.poetry.dependencies]
```

### Comparing `python_sysinformer-1.5.0/src/config/config_parser.py` & `python_sysinformer-1.6.0/src/config/config_parser.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.5.0/src/config/default_config.py` & `python_sysinformer-1.6.0/src/config/default_config.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.5.0/src/core/containers.py` & `python_sysinformer-1.6.0/src/core/containers.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.5.0/src/core/cpu.py` & `python_sysinformer-1.6.0/src/core/cpu.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,32 +48,54 @@
                 cpu_cache = f"{int(result.stdout.strip()) // 1024} KB"
         except subprocess.SubprocessError:
             cpu_cache = "UNKNOWN"
 
     return cpu_cache, cpu_bogomips
 
 
+def get_cpu_processor_info() -> str:
+    """
+    Gets the CPU processor information.
+
+    Returns:
+    str: The CPU processor information.
+    """
+    os_type = platform.system()
+    try:
+        if os_type == platform.system() == "Linux":
+            cpu_info = platform.processor() or "UNKNOWN"
+        elif os_type == "Darwin":
+            cpu_info = subprocess.run(
+                ["sysctl", "-n", "machdep.cpu.brand_string"],
+                capture_output=True,
+                check=True,
+                text=True,
+            ).stdout.strip() or "UNKNOWN"
+        else:
+            cpu_info = "UNKNOWN"
+    except (subprocess.SubprocessError, FileNotFoundError):
+        cpu_info = "UNKNOWN"
+    return cpu_info
+
+
 def get_cpu_info() -> tuple[int, str, Union[float, Literal["Unknown"]], str, str]:
+    # sourcery skip: extract-method
     """
     Gets CPU information.
 
     Returns:
     tuple: A tuple containing the number of CPUs, CPU info, frequency, cache size, and bogomips.
     """
     try:
+        cpu_info = get_cpu_processor_info()
         cpu_nb = psutil.cpu_count() or 0  # if psutil.cpu_count() is not None else 0
-        cpu_info = platform.processor() or "UNKNOWN"
         # cpu_freq = psutil.cpu_freq().max or 0  # if psutil.cpu_freq() is not None else 0
         cpu_freq_info = psutil.cpu_freq()
         cpu_freq = cpu_freq_info.max if cpu_freq_info is not None else 0
-
-        # cache size and bogomips are not available via psutil so we need to get them from files
         cpu_cache, cpu_bogomips = get_cpu_cache_and_bogomips()
-        # cpu_cache = 'UNKNOWN'
-        # cpu_bogomips = 'UNKNOWN'
 
         return cpu_nb, cpu_info, cpu_freq, cpu_cache, cpu_bogomips
     except psutil.Error:
         # print(f"Error reading CPU info: {exception}")
         return 0, "UNKNOWN", 0, "UNKNOWN", "UNKNOWN"
     except FileNotFoundError:
         # print(f"Error reading CPU info: {exception}")
@@ -150,15 +172,15 @@
 def print_cpu_info() -> None:
     """
     Prints the CPU information, CPU usage, load average, and system temperature.
     """
     os_type = platform.system()
     cpu_nb, cpu_info, cpu_freq, cpu_cache, cpu_bogomips = get_cpu_info()
     print_title("CPU Information")
-    print_bold_kv("Number", str(cpu_nb))
+    print_bold_kv("Number of cores", str(cpu_nb))
     print_bold_kv("Model", cpu_info)
     print_bold_kv("Frequency", f"{cpu_freq} MHz")
     print_bold_kv("Cache L2", cpu_cache)
     print_bold_kv("Bogomips", cpu_bogomips)
     print_bold_kv("CPU Usage", f"{get_cpu_usage()}%")
 
     if os_type == "Linux":
```

### Comparing `python_sysinformer-1.5.0/src/core/disks.py` & `python_sysinformer-1.6.0/src/core/disks.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.5.0/src/core/latency.py` & `python_sysinformer-1.6.0/src/core/latency.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.5.0/src/core/memory.py` & `python_sysinformer-1.6.0/src/core/memory.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import platform
 import re
 import subprocess
 
+from typing import Literal, Optional
 from tabulate import tabulate
 
 from src.utilities.utils import print_title
 
 
 def calculate_memory_usage(
     total: int, free: int, buffers: int, cached: int
@@ -25,99 +26,139 @@
     total //= 1024
     free = (free + buffers + cached) // 1024
     used_percentage = ((total - free) / total) * 100 if total != 0 else 0
 
     return total, free, used_percentage
 
 
-def get_memory_info() -> tuple[int, int, float, int, int, float]:
+def format_memory_value(value_in_mb: float) -> str:
+    """Formats memory values to display in MB or GB as appropriate."""
+    if value_in_mb > 1000:
+        return f"{value_in_mb / 1024:.2f}GB"
+    else:
+        return f"{value_in_mb}MB"
+
+
+def get_memory_info() -> (
+    tuple[str, str, float | Literal[0], str, str, float | Literal[0]]
+):
+    """Get memory information"""
     if platform.system() == "Darwin":
         return get_memory_info_macos()
     elif platform.system() == "Linux":
         try:
             mem_info = {
                 i.split()[0].rstrip(":"): int(i.split()[1])
                 for i in open("/proc/meminfo", encoding="UTF-8").readlines()
             }
         except (FileNotFoundError, PermissionError):
             # print(f"Error reading file '/proc/meminfo': {exception}")
-            return (0, 0, 0, 0, 0, 0)
+            return ("0MB", "0MB", 0, "0MB", "0MB", 0)
 
         keys = ["MemTotal", "MemFree", "Buffers", "Cached", "SwapTotal", "SwapFree"]
         if any(key not in mem_info for key in keys):
             print("Not all keys found in '/proc/meminfo'")
-            return (0, 0, 0, 0, 0, 0)
+            return ("0MB", "0MB", 0, "0MB", "0MB", 0)
 
-        mem_total, mem_free, mem_used_percentage = calculate_memory_usage(
+        total_memory, mem_free, mem_used_percentage = calculate_memory_usage(
             mem_info["MemTotal"],
             mem_info["MemFree"],
             mem_info["Buffers"],
             mem_info["Cached"],
         )
 
         swap_total, swap_free, swap_used_percentage = calculate_memory_usage(
             mem_info["SwapTotal"], mem_info["SwapFree"], 0, 0
         )
 
         return (
-            mem_total,
-            mem_free,
+            format_memory_value(total_memory),
+            format_memory_value(mem_free),
             mem_used_percentage,
-            swap_total,
-            swap_free,
+            format_memory_value(swap_total),
+            format_memory_value(swap_free),
             swap_used_percentage,
         )
     else:
-        return (0, 0, 0, 0, 0, 0)
+        return ("0MB", "0MB", 0, "0MB", "0MB", 0)
+
+
+def get_total_memory_of_all_processes() -> float:
+    """
+    Get the total memory usage of all processes on macOS.
+
+    Returns:
+        int: Total memory usage of all processes in MB.
+    """
+    # Get process info
+    ps = (
+        subprocess.Popen(["ps", "-caxm", "-orss,comm"], stdout=subprocess.PIPE)
+        .communicate()[0]
+        .decode()
+    )
+
+    # Iterate processes
+    process_lines = ps.split("\n")
+    sep = re.compile(r"[\s]+")
+    ps_total = 0  # kB
+    for row in range(1, len(process_lines)):
+        row_text = process_lines[row].strip()
+        row_elements = sep.split(row_text)
+        try:
+            rss = float(row_elements[0]) * 1024
+        except (ValueError, IndexError):
+            rss = 0  # ignore...
+        ps_total += rss
+    return ps_total / 1024 / 1024 or 0
 
 
-def get_memory_info_macos() -> tuple[int, int, float, int, int, float]:
+def get_memory_info_macos() -> (
+    tuple[str, str, float | Literal[0], str, str, float | Literal[0]]
+):
     """Get memory information on macOS"""
     try:
-        vm_stat_output = subprocess.check_output(["vm_stat"]).decode()
         sysctl_output = subprocess.check_output(["sysctl", "-n", "hw.memsize"]).decode()
     except (subprocess.CalledProcessError, PermissionError):
-        return (0, 0, 0, 0, 0, 0)
+        return ("0MB", "0MB", 0, "0MB", "0MB", 0)
 
-    vm_stats = parse_vm_stat_output(vm_stat_output)
     total_memory = int(sysctl_output.strip()) // (1024 * 1024)  # Convert bytes to MB
 
-    mem_free = vm_stats.get("Pages free", 0) // 256  # Convert pages to MB
+    mem_usage_process = get_total_memory_of_all_processes()
+    mem_free = round(total_memory - mem_usage_process)
     mem_used_percentage = (
         ((total_memory - mem_free) / total_memory) * 100 if total_memory != 0 else 0
     )
 
-    swap_total = vm_stats.get("Swapins", 0) // 256  # Convert pages to MB
-    swap_free = (
-        vm_stats.get("Swapins", 0) - vm_stats.get("Swapouts", 0)
-    ) // 256  # Convert pages to MB
+    swap_output = subprocess.check_output(["sysctl", "-n", "vm.swapusage"]).decode()
+    swap_stats = {
+        k: float(v.replace("M", ""))
+        for k, v in re.findall(r"(\w+) = (\d+\.?\d*)M", swap_output)
+    }
+    swap_total = swap_stats.get("total", 0)  # Already in MB
+    swap_free = swap_stats.get("free", 0)  # Already in MB
     swap_used_percentage = (
         ((swap_total - swap_free) / swap_total) * 100 if swap_total != 0 else 0
     )
 
     return (
-        total_memory,
-        mem_free,
+        format_memory_value(total_memory),
+        format_memory_value(mem_free),
         mem_used_percentage,
-        swap_total,
-        swap_free,
+        format_memory_value(swap_total),
+        format_memory_value(swap_free),
         swap_used_percentage,
     )
 
+def show_warning_msg() -> Optional[str]:
+    """
+    Print the macOS warning message
+    """
+    if platform.system() == "Darwin":
+        return "\033[1mWARNING\033[0m: memory usage of all processes used to calculate free memory on macOS"
 
-def parse_vm_stat_output(output: str) -> dict:
-    """Parse the output of the 'vm_stat' command on macOS."""
-    vm_stats = {}
-    lines = output.split("\n")
-    sep = re.compile(r":[\s]+")
-    for line in lines[1:-2]:
-        line = line.strip()
-        key, value = sep.split(line)
-        vm_stats[key] = int(value.strip("."))
-    return vm_stats
 
 
 def print_memory_info() -> None:
     """
     Print the memory information table
     """
     # Memory
@@ -127,15 +168,16 @@
         mem_used_percentage,
         swap_total,
         swap_free,
         swap_used_percentage,
     ) = get_memory_info()
 
     table = [
-        ["Memory", f"{mem_free}MB", f"{mem_total}MB", f"{mem_used_percentage:.2f}%"],
-        ["Swap", f"{swap_free}MB", f"{swap_total}MB", f"{swap_used_percentage:.2f}%"],
+        ["Memory", f"{mem_free}", f"{mem_total}", f"{mem_used_percentage:.2f}%"],
+        ["Swap", f"{swap_free}", f"{swap_total}", f"{swap_used_percentage:.2f}%"],
     ]
 
     headers = ["Type", "Free", "Total", "Usage"]
 
     print_title("Memory Information")
+    print(show_warning_msg())
     print(tabulate(table, headers, tablefmt="simple_grid"))
```

### Comparing `python_sysinformer-1.5.0/src/core/networking.py` & `python_sysinformer-1.6.0/src/core/networking.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.5.0/src/core/processes.py` & `python_sysinformer-1.6.0/src/core/processes.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.5.0/src/core/services.py` & `python_sysinformer-1.6.0/src/core/services.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.5.0/src/core/system.py` & `python_sysinformer-1.6.0/src/core/system.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.5.0/src/main.py` & `python_sysinformer-1.6.0/src/main.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.5.0/src/utilities/utils.py` & `python_sysinformer-1.6.0/src/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `python_sysinformer-1.5.0/PKG-INFO` & `python_sysinformer-1.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-sysinformer
-Version: 1.5.0
+Version: 1.6.0
 Summary: A simple system information tool for Linux
 Author: Timothy Bryant
 Author-email: timothybryant3@gmail.com
 Requires-Python: >=3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -54,14 +54,17 @@
 
 ## Installation
 
 The easiest way to install the tool is with `pip`:
 
 ```bash
   pip install python-SysInformer
+
+  # if using pyenv - upgrade the tool with to avoid potential cache issues:
+  pip install --upgrade python-SysInformer --force-reinstall
 ```
 
 Additionaly, if you have [poetry](https://python-poetry.org/) installed you can install the tool with:
 
 ```bash
 git clone [this repo]
 poetry install
```

