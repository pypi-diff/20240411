# Comparing `tmp/pop_cli-2.0.1.tar.gz` & `tmp/pop_cli-2.0.2.tar.gz`

## Comparing `pop_cli-2.0.1.tar` & `pop_cli-2.0.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 pop_cli-2.0.1/.pre-commit-config.yaml
--rwxr-xr-x   0        0        0      602 2020-02-02 00:00:00.000000 pop_cli-2.0.1/src/__main__.py
--rw-r--r--   0        0        0     1196 2020-02-02 00:00:00.000000 pop_cli-2.0.1/src/config.yaml
--rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 pop_cli-2.0.1/src/hub/cli.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pop_cli-2.0.1/src/hub/config.py
--rw-r--r--   0        0        0     6475 2020-02-02 00:00:00.000000 pop_cli-2.0.1/src/hub/console.py
--rw-r--r--   0        0        0     1647 2020-02-02 00:00:00.000000 pop_cli-2.0.1/src/hub/init.py
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 pop_cli-2.0.1/src/hub/ref.py
--rw-r--r--   0        0        0     1507 2020-02-02 00:00:00.000000 pop_cli-2.0.1/src/hub/state.py
--rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 pop_cli-2.0.1/tests/conftest.py
--rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 pop_cli-2.0.1/tests/integration/test_cli.py
--rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pop_cli-2.0.1/tests/integration/test_config.py
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pop_cli-2.0.1/tests/integration/test_console.py
--rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pop_cli-2.0.1/tests/integration/test_init.py
--rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 pop_cli-2.0.1/tests/integration/test_ref.py
--rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 pop_cli-2.0.1/tests/integration/test_state.py
--rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pop_cli-2.0.1/tests/tpath/plugin/config.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pop_cli-2.0.1/tests/tpath/plugin/src/init.py
--rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pop_cli-2.0.1/tests/tpath/plugin/src/mod.py
--rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pop_cli-2.0.1/.gitignore
--rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pop_cli-2.0.1/README.rst
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 pop_cli-2.0.1/pyproject.toml
--rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 pop_cli-2.0.1/PKG-INFO
+-rw-r--r--   0        0        0     3870 2020-02-02 00:00:00.000000 pop_cli-2.0.2/.pre-commit-config.yaml
+-rwxr-xr-x   0        0        0      602 2020-02-02 00:00:00.000000 pop_cli-2.0.2/src/__main__.py
+-rw-r--r--   0        0        0     1219 2020-02-02 00:00:00.000000 pop_cli-2.0.2/src/config.yaml
+-rw-r--r--   0        0        0     4249 2020-02-02 00:00:00.000000 pop_cli-2.0.2/src/hub/cli.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 pop_cli-2.0.2/src/hub/config.py
+-rw-r--r--   0        0        0     6690 2020-02-02 00:00:00.000000 pop_cli-2.0.2/src/hub/console.py
+-rw-r--r--   0        0        0     1968 2020-02-02 00:00:00.000000 pop_cli-2.0.2/src/hub/init.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 pop_cli-2.0.2/src/hub/ref.py
+-rw-r--r--   0        0        0     1575 2020-02-02 00:00:00.000000 pop_cli-2.0.2/src/hub/state.py
+-rw-r--r--   0        0        0      596 2020-02-02 00:00:00.000000 pop_cli-2.0.2/tests/conftest.py
+-rw-r--r--   0        0        0     3218 2020-02-02 00:00:00.000000 pop_cli-2.0.2/tests/integration/test_cli.py
+-rw-r--r--   0        0        0     2165 2020-02-02 00:00:00.000000 pop_cli-2.0.2/tests/integration/test_config.py
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pop_cli-2.0.2/tests/integration/test_console.py
+-rw-r--r--   0        0        0     1009 2020-02-02 00:00:00.000000 pop_cli-2.0.2/tests/integration/test_init.py
+-rw-r--r--   0        0        0     1448 2020-02-02 00:00:00.000000 pop_cli-2.0.2/tests/integration/test_ref.py
+-rw-r--r--   0        0        0      879 2020-02-02 00:00:00.000000 pop_cli-2.0.2/tests/integration/test_state.py
+-rw-r--r--   0        0        0      342 2020-02-02 00:00:00.000000 pop_cli-2.0.2/tests/tpath/plugin/config.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 pop_cli-2.0.2/tests/tpath/plugin/src/init.py
+-rw-r--r--   0        0        0      101 2020-02-02 00:00:00.000000 pop_cli-2.0.2/tests/tpath/plugin/src/mod.py
+-rw-r--r--   0        0        0     2474 2020-02-02 00:00:00.000000 pop_cli-2.0.2/.gitignore
+-rw-r--r--   0        0        0     1711 2020-02-02 00:00:00.000000 pop_cli-2.0.2/README.rst
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 pop_cli-2.0.2/pyproject.toml
+-rw-r--r--   0        0        0     2501 2020-02-02 00:00:00.000000 pop_cli-2.0.2/PKG-INFO
```

### Comparing `pop_cli-2.0.1/.pre-commit-config.yaml` & `pop_cli-2.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.1/src/__main__.py` & `pop_cli-2.0.2/src/__main__.py`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.1/src/config.yaml` & `pop_cli-2.0.2/src/config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -21,14 +21,15 @@
       positional: True
       nargs: "?"
     cli:
       help: The namespace to use as the authoritative CLI
       choices: _dynamic.config.cli_config
     args:
       help: Any additional arguments to forward to the next cli
+      positional: True
       nargs: "..."
     interactive:
       help: Start a python console that contains a hub and can await functions
       action: store_true
       options:
         - -i
     hub_state:
```

### Comparing `pop_cli-2.0.1/src/hub/cli.py` & `pop_cli-2.0.2/src/hub/cli.py`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.1/src/hub/config.py` & `pop_cli-2.0.2/src/hub/config.py`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.1/src/hub/console.py` & `pop_cli-2.0.2/src/hub/console.py`

 * *Files 3% similar despite different names*

```diff
@@ -47,30 +47,34 @@
 
                 result = local_namespace.pop("__result__", None)
                 post = {k: v for k, v in local_namespace.items() if k != "hub"}
 
                 # The locals didn't change, this wasn't a variable assignment
                 if previous == post:
                     # If an async function was called without being assigned to a variable then await it
-                    if hub.lib.asyncio.iscoroutine(result):
+                    if (
+                        hub.lib.asyncio.iscoroutine(result)
+                        and result not in local_namespace.values()
+                    ):
                         result = await result
 
                     # If the result wasn't assigned to a variable then print it out
                     if result is not None:
                         print(result)
 
         except EOFError:
             # Exit handling...
             break
         except KeyboardInterrupt:
             # Keyboard interrupt handling...
-            break
+            continue
         except Exception:
             # Error handling...
             await hub.log.error(hub.lib.traceback.format_exc())
+            continue
 
 
 async def get_completer(hub, **kwargs):
     """
     Creates a completer for the interactive console that provides completion suggestions for the 'hub' namespace.
 
     Args:
@@ -111,17 +115,19 @@
                                     finder = tuple(finder).__getitem__(int(p))
                                 except Exception:
                                     # No completions if the path is invalid
                                     return
                             else:
                                 # No completions if the path is invalid
                                 return
-                        except KeyError:
-                            # No completions if the path is invalid
+                        except Exception:
                             return
+                    except Exception:
+                        # No completions if the path is invalid
+                        return
 
                 # Get the prefix of the current attribute being completed
                 current_attr_prefix = parts[-1]
                 attrs = []
                 try:
                     # Get all attributes and methods of the current object in the hub namespace
                     attrs += [_ for _ in finder]
@@ -139,15 +145,15 @@
                         if name.startswith(current_attr_prefix):
                             display = f"hub.{'.'.join(parts[:-1] + [name])}"
                             yield hub.lib.prompt_toolkit.completion.Completion(
                                 name,
                                 start_position=-len(current_attr_prefix),
                                 display=display,
                             )
-                    except:
+                    except Exception:
                         continue
 
     completer = HubCompleter()
     # Create a completer for local variables
     local_completer = hub.lib.prompt_toolkit.completion.WordCompleter(
         list(kwargs.keys()), ignore_case=True
     )
```

### Comparing `pop_cli-2.0.1/src/hub/init.py` & `pop_cli-2.0.2/src/hub/init.py`

 * *Files 26% similar despite different names*

```diff
@@ -8,30 +8,37 @@
 
     Args:
         hub (pop.hub.Hub): The global namespace
     """
     # Grab OPT for cli, arguments it doesn't use will be passed onward to the next cli
     OPT = hub.lib.cpop.data.NamespaceDict(hub.OPT.copy())
     ref = OPT.cli.ref
+    await hub.log.debug(f"Using ref: hub.{ref}")
 
     # If no cli was defined, then use the first part of the passed ref as the authoritative cli
     cli = OPT.cli.cli or ref.split(".")[0]
+    await hub.log.debug(f"Using cli: {cli}")
 
     # Try to restore the hub state
     hub_state_file = await hub.cli.state.restore(OPT)
 
     if OPT.cli.cli or (
         (cli in hub._dynamic.config.cli_config)
         and (cli not in OPT.get("pop", {}).get("global_clis", ()))
     ):
+        await hub.log.debug(f"Loading cli: {cli}")
         # Reload hub.OPT with the cli arguments not consumed by the initial hub
         await hub.cli.config.override(cli, OPT)
-
-    # Treat all the extra args as parameters for the named ref
-    args, kwargs = await hub.cli.cli.parameters(OPT)
+        args = []
+        kwargs = {}
+    else:
+        # Treat all the extra args as parameters for the named ref
+        args, kwargs = await hub.cli.cli.parameters(OPT)
+        await hub.log.debug(f"Args: {' '.join(args)}")
+        await hub.log.debug(f"Kwargs: {' '.join(kwargs.keys())}")
 
     # Get the named reference from the hub
     finder = await hub.cli.ref.find(ref)
 
     if OPT.cli.interactive:
         # Start an asynchronous interactive console
         await hub.cli.console.run(OPT=OPT, ref=finder)
```

### Comparing `pop_cli-2.0.1/src/hub/ref.py` & `pop_cli-2.0.2/src/hub/ref.py`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.1/src/hub/state.py` & `pop_cli-2.0.2/src/hub/state.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 async def restore(hub, opts: dict) -> str:
     # Try to get a saved hub
     if opts.cli.hub_state:
         hub_state = await hub.cli.cli.parse_value(opts.cli.hub_state)
 
         # Load the saved state of the hub from a file in memory
         hub_state_file = hub.lib.pathlib.Path(hub_state).expanduser()
+        await hub.log.debug(f"Restoring hub from {hub_state_file}")
         await hub.cli.state.load(hub_state_file)
     else:
         hub_state_file = None
 
     return hub_state_file
```

### Comparing `pop_cli-2.0.1/tests/conftest.py` & `pop_cli-2.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.1/tests/integration/test_cli.py` & `pop_cli-2.0.2/tests/integration/test_cli.py`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.1/tests/integration/test_config.py` & `pop_cli-2.0.2/tests/integration/test_config.py`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.1/tests/integration/test_console.py` & `pop_cli-2.0.2/tests/integration/test_console.py`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.1/tests/integration/test_init.py` & `pop_cli-2.0.2/tests/integration/test_init.py`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.1/tests/integration/test_ref.py` & `pop_cli-2.0.2/tests/integration/test_ref.py`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.1/tests/integration/test_state.py` & `pop_cli-2.0.2/tests/integration/test_state.py`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.1/.gitignore` & `pop_cli-2.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.1/README.rst` & `pop_cli-2.0.2/README.rst`

 * *Files identical despite different names*

### Comparing `pop_cli-2.0.1/pyproject.toml` & `pop_cli-2.0.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "pop-cli"
-version = "2.0.1"
+version = "2.0.2"
 description = "A POP cli interface"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
 ]
 classifiers = [
     "Operating System :: OS Independent",
```

### Comparing `pop_cli-2.0.1/PKG-INFO` & `pop_cli-2.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: pop-cli
-Version: 2.0.1
+Version: 2.0.2
 Summary: A POP cli interface
 Author-email: Tyler Levy Conde <yonstib@gmail.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

