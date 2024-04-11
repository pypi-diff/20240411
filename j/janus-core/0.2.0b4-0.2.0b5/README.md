# Comparing `tmp/janus_core-0.2.0b4.tar.gz` & `tmp/janus_core-0.2.0b5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "janus_core-0.2.0b4.tar", max compression
+gzip compressed data, was "janus_core-0.2.0b5.tar", max compression
```

## Comparing `janus_core-0.2.0b4.tar` & `janus_core-0.2.0b5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     1533 2024-04-09 07:25:35.263221 janus_core-0.2.0b4/LICENSE
--rw-r--r--   0        0        0     8011 2024-04-09 07:25:35.263221 janus_core-0.2.0b4/README.md
--rw-r--r--   0        0        0       80 2024-04-09 07:25:35.263221 janus_core-0.2.0b4/janus_core/__init__.py
--rw-r--r--   0        0        0    28807 2024-04-09 07:25:35.263221 janus_core-0.2.0b4/janus_core/cli.py
--rw-r--r--   0        0        0     4790 2024-04-09 07:25:35.263221 janus_core-0.2.0b4/janus_core/geom_opt.py
--rw-r--r--   0        0        0     1664 2024-04-09 07:25:35.263221 janus_core-0.2.0b4/janus_core/janus_types.py
--rw-r--r--   0        0        0     4045 2024-04-09 07:25:35.263221 janus_core-0.2.0b4/janus_core/log.py
--rw-r--r--   0        0        0    29064 2024-04-09 07:25:35.263221 janus_core-0.2.0b4/janus_core/md.py
--rw-r--r--   0        0        0     3514 2024-04-09 07:25:35.263221 janus_core-0.2.0b4/janus_core/mlip_calculators.py
--rw-r--r--   0        0        0    12111 2024-04-09 07:25:35.263221 janus_core-0.2.0b4/janus_core/single_point.py
--rw-r--r--   0        0        0     3293 2024-04-09 07:25:35.263221 janus_core-0.2.0b4/janus_core/stats.py
--rw-r--r--   0        0        0      545 2024-04-09 07:25:35.263221 janus_core-0.2.0b4/janus_core/utils.py
--rw-r--r--   0        0        0     2553 2024-04-09 07:25:35.263221 janus_core-0.2.0b4/pyproject.toml
--rw-r--r--   0        0        0     9072 1970-01-01 00:00:00.000000 janus_core-0.2.0b4/PKG-INFO
+-rw-r--r--   0        0        0     1533 2024-04-11 11:04:09.575169 janus_core-0.2.0b5/LICENSE
+-rw-r--r--   0        0        0     8784 2024-04-11 11:04:09.575169 janus_core-0.2.0b5/README.md
+-rw-r--r--   0        0        0       80 2024-04-11 11:04:09.579169 janus_core-0.2.0b5/janus_core/__init__.py
+-rw-r--r--   0        0        0    29979 2024-04-11 11:04:09.579169 janus_core-0.2.0b5/janus_core/cli.py
+-rw-r--r--   0        0        0     4790 2024-04-11 11:04:09.579169 janus_core-0.2.0b5/janus_core/geom_opt.py
+-rw-r--r--   0        0        0     1664 2024-04-11 11:04:09.579169 janus_core-0.2.0b5/janus_core/janus_types.py
+-rw-r--r--   0        0        0     4045 2024-04-11 11:04:09.579169 janus_core-0.2.0b5/janus_core/log.py
+-rw-r--r--   0        0        0    32211 2024-04-11 11:04:09.579169 janus_core-0.2.0b5/janus_core/md.py
+-rw-r--r--   0        0        0     3514 2024-04-11 11:04:09.579169 janus_core-0.2.0b5/janus_core/mlip_calculators.py
+-rw-r--r--   0        0        0    12111 2024-04-11 11:04:09.579169 janus_core-0.2.0b5/janus_core/single_point.py
+-rw-r--r--   0        0        0     3293 2024-04-11 11:04:09.579169 janus_core-0.2.0b5/janus_core/stats.py
+-rw-r--r--   0        0        0      545 2024-04-11 11:04:09.579169 janus_core-0.2.0b5/janus_core/utils.py
+-rw-r--r--   0        0        0     2553 2024-04-11 11:04:09.579169 janus_core-0.2.0b5/pyproject.toml
+-rw-r--r--   0        0        0     9845 1970-01-01 00:00:00.000000 janus_core-0.2.0b5/PKG-INFO
```

### Comparing `janus_core-0.2.0b4/LICENSE` & `janus_core-0.2.0b5/LICENSE`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b4/README.md` & `janus_core-0.2.0b5/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 [![Docs status][docs-badge]][docs-link]
 [![PyPI version][pypi-badge]][pypi-link]
 [![License][license-badge]][license-link]
 [![DOI][doi-badge]][doi-link]
 
 # janus-core
 
+![logo][logo]
+
 Tools for machine learnt interatomic potentials
 
 ## Features in development
 
 - [x] Support for multiple MLIPs
   - MACE
   - M3GNET
@@ -136,14 +138,33 @@
 
 This performs an NVE molecular dynamics simulation at 300K for 200 steps (0.2 ps), saving the trajectory every 10 steps after the first 100, and the thermodynamical statistics every 10 steps, as well as changing the output file names for both.
 
 
 For all options, run `janus md --help`.
 
 
+### Heating
+
+Run an NVT heating simultation from 20K to 300K in steps of 20K, with 10fs at each temperature:
+
+```shell
+janus md --ensemble nvt --struct tests/data/NaCl.cif --temp-start 20 --temp-end 300 --temp-step 20 --temp-time 10
+```
+
+This produces the same output files as an MD simulation.
+
+MD can also be carried out after heating using the same options as described in #molecular-dynamics. For example:
+
+```shell
+janus md --ensemble nvt --struct tests/data/NaCl.cif --temp-start 20 --temp-end 300 --temp-step 20 --temp-time 10 --steps 1000 --temp 300
+```
+
+This performs the same initial heating, before running a further 1000 steps (1 ps) at 300K.
+
+
 ### Using configuration files
 
 Default values for all command line options may be specifed through a Yaml 1.1 formatted configuration file by adding the `--config` option. If an option is present in both the command line and configuration file, the command line value takes precedence.
 
 For example, with the following configuration file and command:
 
 ```yaml
@@ -196,7 +217,8 @@
 [docs-link]: https://stfc.github.io/janus-core/
 [pypi-badge]: https://badge.fury.io/py/janus-core.svg
 [pypi-link]: https://badge.fury.io/py/janus-core
 [license-badge]: https://img.shields.io/badge/License-BSD_3--Clause-blue.svg
 [license-link]: https://opensource.org/licenses/BSD-3-Clause
 [doi-link]: https://zenodo.org/badge/latestdoi/754081470
 [doi-badge]: https://zenodo.org/badge/754081470.svg
+[logo]: https://raw.githubusercontent.com/stfc/janus-core/main/docs/source/images/janus-core-100.png
```

### Comparing `janus_core-0.2.0b4/janus_core/cli.py` & `janus_core-0.2.0b5/janus_core/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -663,14 +663,28 @@
     ] = False,
     traj_start: Annotated[
         int, typer.Option(help="Step to start saving trajectory.")
     ] = 0,
     traj_every: Annotated[
         int, typer.Option(help="Frequency of steps to save trajectory.")
     ] = 100,
+    temp_start: Annotated[
+        Optional[float],
+        typer.Option(help="Temperature to start heating, in K.  [default: None]"),
+    ] = None,
+    temp_end: Annotated[
+        Optional[float],
+        typer.Option(help="Maximum temperature for heating, in K.  [default: None]"),
+    ] = None,
+    temp_step: Annotated[
+        float, typer.Option(help="Size of temperature steps when heating, in K.")
+    ] = None,
+    temp_time: Annotated[
+        float, typer.Option(help="Time between heating steps, in fs.")
+    ] = None,
     log: LogPath = "md.log",
     seed: Annotated[
         Optional[int],
         typer.Option(help="Random seed for numpy.random and random functions."),
     ] = None,
     summary: Summary = "md_summary.yml",
 ):
@@ -745,14 +759,26 @@
         Trajectory file to save. Default inferred from `file_prefix`.
     traj_append : bool
         Whether to append trajectory. Default is False.
     traj_start : int
         Step to start saving trajectory. Default is 0.
     traj_every : int
         Frequency of steps to save trajectory. Default is 100.
+    temp_start : Optional[float]
+        Temperature to start heating, in K. Default is None, which disables
+        heating.
+    temp_end : Optional[float]
+        Maximum temperature for heating, in K. Default is None, which disables
+        heating.
+    temp_step : Optional[float]
+        Size of temperature steps when heating, in K. Default is None, which disables
+        heating.
+    temp_time : Optional[float]
+        Time between heating steps, in fs. Default is None, which disables
+        heating.
     log : Optional[Path]
         Path to write logs to. Default is "md.log".
     seed : Optional[int]
         Random seed used by numpy.random and random functions, such as in Langevin.
         Default is None.
     summary : Path
         Path to save summary of inputs and start/end time. Default is md_summary.yml.
@@ -804,14 +830,18 @@
         "restarts_to_keep": restarts_to_keep,
         "stats_file": stats_file,
         "stats_every": stats_every,
         "traj_file": traj_file,
         "traj_append": traj_append,
         "traj_start": traj_start,
         "traj_every": traj_every,
+        "temp_start": temp_start,
+        "temp_end": temp_end,
+        "temp_step": temp_step,
+        "temp_time": temp_time,
         "log_kwargs": log_kwargs,
         "seed": seed,
     }
 
     # Instantiate MD ensemble
     if ensemble == "nvt":
         for key in ["thermostat_time", "barostat_time", "bulk_modulus", "pressure"]:
```

### Comparing `janus_core-0.2.0b4/janus_core/geom_opt.py` & `janus_core-0.2.0b5/janus_core/geom_opt.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b4/janus_core/janus_types.py` & `janus_core-0.2.0b5/janus_core/janus_types.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b4/janus_core/log.py` & `janus_core-0.2.0b5/janus_core/log.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b4/janus_core/md.py` & `janus_core-0.2.0b5/janus_core/md.py`

 * *Files 8% similar despite different names*

```diff
@@ -81,14 +81,23 @@
         Trajectory file to save. Default inferred from `file_prefix`.
     traj_append : bool
         Whether to append trajectory. Default is False.
     traj_start : int
         Step to start saving trajectory. Default is 0.
     traj_every : int
         Frequency of steps to save trajectory. Default is 100.
+    temp_start : Optional[float]
+        Temperature to start heating, in K. Default is None, which disables heating.
+    temp_end : Optional[float]
+        Maximum temperature for heating, in K. Default is None, which disables heating.
+    temp_step : Optional[float]
+        Size of temperature steps when heating, in K. Default is None, which disables
+        heating.
+    temp_time : Optional[float]
+        Time between heating steps, in fs. Default is None, which disables heating.
     log_kwargs : Optional[dict[str, Any]]
         Keyword arguments to pass to log config. Default is None.
     seed : Optional[int]
         Random seed used by numpy.random and random functions, such as in Langevin.
         Default is None.
 
     Attributes
@@ -102,28 +111,16 @@
     restart_files : list[PathLike]
         List of files saved to restart dynamics.
     offset : int
         Number of previous steps if restarting simulation.
 
     Methods
     -------
-    optimize_structure()
-        Perform geometry optimization.
-    reset_velocities()
-        Reset velocities and (optionally) rotation of system.
-    rotate_restart_files()
-        Rotate restart files.
     run()
-        Run molecular dynamics simulation.
-    write_md_log()
-        Write molecular dynamics log.
-    write_traj()
-        Write current structure to trajectory file.
-    write_restart()
-        Write restart file and (optionally) rotate files saved.
+        Run molecular dynamics simulation and/or heating ramp.
     get_log_stats()
         Get thermodynamical statistics to be written to molecular dynamics log.
     get_log_header()
         Get header string for molecular dynamics log.
     """
 
     def __init__(  # pylint: disable=too-many-arguments,too-many-locals,too-many-statements
@@ -149,14 +146,18 @@
         restarts_to_keep: int = 4,
         stats_file: Optional[PathLike] = None,
         stats_every: int = 100,
         traj_file: Optional[PathLike] = None,
         traj_append: bool = False,
         traj_start: int = 0,
         traj_every: int = 100,
+        temp_start: Optional[float] = None,
+        temp_end: Optional[float] = None,
+        temp_step: Optional[float] = None,
+        temp_time: Optional[float] = None,
         log_kwargs: Optional[dict[str, Any]] = None,
         seed: Optional[int] = None,
     ) -> None:
         """
         Initialise molecular dynamics simulation configuration.
 
         Parameters
@@ -212,14 +213,25 @@
             Trajectory file to save. Default inferred from `file_prefix`.
         traj_append : bool
             Whether to append trajectory. Default is False.
         traj_start : int
             Step to start saving trajectory. Default is 0.
         traj_every : int
             Frequency of steps to save trajectory. Default is 100.
+        temp_start : Optional[float]
+            Temperature to start heating, in K. Default is None, which disables
+            heating.
+        temp_end : Optional[float]
+            Maximum temperature for heating, in K. Default is None, which disables
+            heating.
+        temp_step : Optional[float]
+            Size of temperature steps when heating, in K. Default is None, which
+            disables heating.
+        temp_time : Optional[float]
+            Time between heating steps, in fs. Default is None, which disables heating.
         log_kwargs : Optional[dict[str, Any]]
             Keyword arguments to pass to log config. Default is None.
         seed : Optional[int]
             Random seed used by numpy.random and random functions, such as in Langevin.
             Default is None.
         """
         self.struct = struct
@@ -241,14 +253,18 @@
         self.restarts_to_keep = restarts_to_keep
         self.stats_file = stats_file
         self.stats_every = stats_every
         self.traj_file = traj_file
         self.traj_append = traj_append
         self.traj_start = traj_start
         self.traj_every = traj_every
+        self.temp_start = temp_start
+        self.temp_end = temp_end
+        self.temp_step = temp_step
+        self.temp_time = temp_time * units.fs if temp_time else None
         self.log_kwargs = log_kwargs
         self.ensemble = ensemble
         self.seed = seed
 
         self.log_kwargs = (
             log_kwargs if log_kwargs else {}
         )  # pylint: disable=duplicate-code
@@ -265,14 +281,30 @@
         if minimize and equil_steps < minimize_every:
             warn("Geometry will not be minimized during dynamics")
 
         # Warn if attempting to remove rotation without resetting velocities
         if remove_rot and not rescale_velocities:
             warn("Rotation will not be removed unless `rescale_velocities` is True")
 
+        # Check temperatures for heating differ
+        if self.temp_start is not None and self.temp_start == self.temp_end:
+            raise ValueError("Start and end temperatures must be different")
+
+        # Warn if mix of None and not None
+        self.ramp_temp = (
+            self.temp_start and self.temp_end and self.temp_step and self.temp_time
+        )
+        if (
+            self.temp_start or self.temp_end or self.temp_step or self.temp_time
+        ) and not self.ramp_temp:
+            warn(
+                "`temp_start`, `temp_end` and `temp_step` must all be specified for "
+                "heating to run"
+            )
+
         self.minimize_kwargs = minimize_kwargs if minimize_kwargs else {}
         self.restart_files = []
         self.dyn = None
         self.n_atoms = len(self.struct)
 
         # Infer names for structure and if not specified
         if not self.struct_name:
@@ -285,33 +317,42 @@
         if "masses" not in self.struct.arrays.keys():
             self.struct.set_masses()
 
         if self.seed:
             np.random.seed(seed)
             random.seed(seed)
 
-    def rotate_restart_files(self) -> None:
+    def _rotate_restart_files(self) -> None:
         """Rotate restart files."""
         if len(self.restart_files) > self.restarts_to_keep:
             path = Path(self.restart_files.pop(0))
             path.unlink(missing_ok=True)
 
-    def reset_velocities(self) -> None:
-        """Reset velocities and (optionally) rotation of system."""
-        if self.dyn.nsteps < self.equil_steps:
-            MaxwellBoltzmannDistribution(self.struct, temperature_K=self.temp)
-            Stationary(self.struct)
+    def _set_velocity_distribution(self) -> None:
+        """
+        Set velocities to current target temperature.
+
+        Sets Maxwell-Boltzmann velocity distribution, as well as removing
+        centre-of-mass momentum, and (optionally) total angular momentum.
+        """
+        MaxwellBoltzmannDistribution(self.struct, temperature_K=self.temp)
+        Stationary(self.struct)
+        if self.logger:
+            self.logger.info("Velocities reset at step %s", self.dyn.nsteps)
+        if self.remove_rot:
+            ZeroRotation(self.struct)
             if self.logger:
-                self.logger.info("Velocities reset at step %s", self.dyn.nsteps)
-            if self.remove_rot:
-                ZeroRotation(self.struct)
-                if self.logger:
-                    self.logger.info("Rotation reset at step %s", self.dyn.nsteps)
+                self.logger.info("Rotation reset at step %s", self.dyn.nsteps)
+
+    def _reset_velocities(self) -> None:
+        """Reset velocities and (optionally) rotation of system while equilibrating."""
+        if self.dyn.nsteps < self.equil_steps:
+            self._set_velocity_distribution()
 
-    def optimize_structure(self) -> None:
+    def _optimize_structure(self) -> None:
         """Perform geometry optimization."""
         if self.dyn.nsteps < self.equil_steps:
             if self.logger:
                 self.minimize_kwargs["log_kwargs"] = {
                     "filename": self.log_kwargs["filename"],
                     "name": self.logger.name,
                     "filemode": "a",
@@ -340,15 +381,15 @@
 
         Returns
         -------
         str
             Header for molecular dynamics log.
         """
         log_header = (
-            "Step | Real Time [s] | Time [fs] | Epot/N [eV] | Ekin/N [eV] | "
+            "# Step | Real Time [s] | Time [fs] | Epot/N [eV] | Ekin/N [eV] | "
             "T [K] | Etot/N [eV] | Density [g/cm^3] | Volume [A^3] | P [bar] | "
             "Pxx [bar] | Pyy [bar] | Pzz [bar] | Pyz [bar] | Pxz [bar] | Pxy [bar]"
         )
 
         return log_header
 
     def get_log_stats(self) -> str:
@@ -405,92 +446,121 @@
             f"{pressure_tensor[1]:.3e} {pressure_tensor[2]:.3e} "
             f"{pressure_tensor[3]:.3e} {pressure_tensor[4]:.3e} "
             f"{pressure_tensor[5]:.3e}"
         )
 
         return log_stats
 
-    def write_md_log(self) -> None:
+    def _write_stats_file(self) -> None:
         """Write molecular dynamics log."""
         log_stats = self.get_log_stats()
-        with open(self.stats_file, "a", encoding="utf8") as md_log:
-            print(log_stats, file=md_log)
+        with open(self.stats_file, "a", encoding="utf8") as stats_file:
+            print(log_stats, file=stats_file)
 
-    def write_traj(self) -> None:
+    def _write_traj(self) -> None:
         """Write current structure to trajectory file."""
         if self.dyn.nsteps >= self.traj_start:
             # Append if restarting or already started writing
             append = self.restart or (
                 self.dyn.nsteps > self.traj_start + self.traj_start % self.traj_every
             )
 
             self.dyn.atoms.write(
                 self.traj_file,
                 write_info=True,
                 columns=["symbols", "positions", "momenta", "masses"],
                 append=append,
             )
 
-    def write_restart(self) -> None:
+    def _write_restart(self) -> None:
         """Write restart file and (optionally) rotate files saved."""
         step = self.offset + self.dyn.nsteps
         if step > 0:
             restart_file = f"{self.restart_stem}-{step}.xyz"
             write(
                 restart_file,
                 self.struct,
                 write_info=True,
                 columns=["symbols", "positions", "momenta", "masses"],
             )
             if self.rotate_restart:
                 self.restart_files.append(restart_file)
-                self.rotate_restart_files()
+                self._rotate_restart_files()
 
     def run(self) -> None:
-        """Run molecular dynamics simulation."""
-        if self.logger:
-            self.logger.info("Starting molecular dynamics simulation")
-
-        self.struct.info["real_time"] = datetime.datetime.now()
-
+        """Run molecular dynamics simulation and/or temperature ramp."""
+        # Check if restarting simulation
         if self.restart:
             try:
-                with open(self.stats_file, encoding="utf8") as md_log:
-                    last_line = md_log.readlines()[-1].split()
+                with open(self.stats_file, encoding="utf8") as stats_file:
+                    last_line = stats_file.readlines()[-1].split()
                 try:
                     self.offset = int(last_line[0])
                 except (IndexError, ValueError) as e:
                     raise ValueError("Unable to read restart file") from e
             except FileNotFoundError as e:
                 raise FileNotFoundError("Unable to read restart file") from e
 
         else:
             if self.minimize:
                 optimize(self.struct, **self.minimize_kwargs)
             if self.rescale_velocities:
-                self.reset_velocities()
+                self._reset_velocities()
 
             log_header = self.get_log_header()
-            with open(self.stats_file, "w", encoding="utf8") as md_log:
-                print(log_header, file=md_log)
+            with open(self.stats_file, "w", encoding="utf8") as stats_file:
+                print(log_header, file=stats_file)
 
-        self.dyn.attach(self.write_md_log, interval=self.stats_every)
-        self.dyn.attach(self.write_traj, interval=self.traj_every)
-        self.dyn.attach(self.write_restart, interval=self.restart_every)
+        self.dyn.attach(self._write_stats_file, interval=self.stats_every)
+        self.dyn.attach(self._write_traj, interval=self.traj_every)
+        self.dyn.attach(self._write_restart, interval=self.restart_every)
 
         if self.rescale_velocities:
-            self.dyn.attach(self.reset_velocities, interval=self.rescale_every)
+            self.dyn.attach(self._reset_velocities, interval=self.rescale_every)
 
         if self.minimize and self.minimize_every > 0:
-            self.dyn.attach(self.optimize_structure, interval=self.minimize_every)
+            self.dyn.attach(self._optimize_structure, interval=self.minimize_every)
+
+        # Note current time
+        self.struct.info["real_time"] = datetime.datetime.now()
+        self._run_dynamics()
 
-        self.dyn.run(self.steps)
+    def _run_dynamics(self) -> None:
+        """Run dynamics and/or temperature ramp."""
+        # Store temperature for final MD
+        md_temp = self.temp
+        if self.ramp_temp:
+            self.temp = self.temp_start
+
+        # Set velocities to match current temperature
+        self._set_velocity_distribution()
+
+        # Run temperature ramp
+        if self.ramp_temp:
+            heating_steps = int(self.temp_time // self.timestep)
 
-        if self.logger:
-            self.logger.info("Molecular dynamics simulation complete")
+            n_temps = int(1 + (self.temp_end - self.temp_start) // self.temp_step)
+            temps = [self.temp_start + i * self.temp_step for i in range(n_temps)]
+
+            if self.logger:
+                self.logger.info("Beginning temperature ramp at %sK", temps[0])
+            for temp in temps:
+                self.temp = temp
+                self.dyn.run(heating_steps)
+            if self.logger:
+                self.logger.info("Temperature ramp complete at %sK", temps[-1])
+
+        # Run MD
+        if self.steps > 0:
+            if self.logger:
+                self.logger.info("Starting molecular dynamics simulation")
+            self.temp = md_temp
+            self.dyn.run(self.steps)
+            if self.logger:
+                self.logger.info("Molecular dynamics simulation complete")
 
 
 class NPT(MolecularDynamics):
     """
     Configure NPT dynamics.
 
     Parameters
```

### Comparing `janus_core-0.2.0b4/janus_core/mlip_calculators.py` & `janus_core-0.2.0b5/janus_core/mlip_calculators.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b4/janus_core/single_point.py` & `janus_core-0.2.0b5/janus_core/single_point.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b4/janus_core/stats.py` & `janus_core-0.2.0b5/janus_core/stats.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b4/janus_core/utils.py` & `janus_core-0.2.0b5/janus_core/utils.py`

 * *Files identical despite different names*

### Comparing `janus_core-0.2.0b4/pyproject.toml` & `janus_core-0.2.0b5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "janus-core"
-version = "0.2.0b4"
+version = "0.2.0b5"
 description = "Tools for machine learnt interatomic potentials"
 authors = [
     "Elliott Kasoar",
     "Federica Zanca",
     "Patrick Austin",
     "David Mason",
     "Jacob Wilkins",
```

### Comparing `janus_core-0.2.0b4/PKG-INFO` & `janus_core-0.2.0b5/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: janus-core
-Version: 0.2.0b4
+Version: 0.2.0b5
 Summary: Tools for machine learnt interatomic potentials
 Home-page: https://github.com/stfc/janus-core/
 Author: Elliott Kasoar
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
@@ -29,14 +29,16 @@
 [![Docs status][docs-badge]][docs-link]
 [![PyPI version][pypi-badge]][pypi-link]
 [![License][license-badge]][license-link]
 [![DOI][doi-badge]][doi-link]
 
 # janus-core
 
+![logo][logo]
+
 Tools for machine learnt interatomic potentials
 
 ## Features in development
 
 - [x] Support for multiple MLIPs
   - MACE
   - M3GNET
@@ -162,14 +164,33 @@
 
 This performs an NVE molecular dynamics simulation at 300K for 200 steps (0.2 ps), saving the trajectory every 10 steps after the first 100, and the thermodynamical statistics every 10 steps, as well as changing the output file names for both.
 
 
 For all options, run `janus md --help`.
 
 
+### Heating
+
+Run an NVT heating simultation from 20K to 300K in steps of 20K, with 10fs at each temperature:
+
+```shell
+janus md --ensemble nvt --struct tests/data/NaCl.cif --temp-start 20 --temp-end 300 --temp-step 20 --temp-time 10
+```
+
+This produces the same output files as an MD simulation.
+
+MD can also be carried out after heating using the same options as described in #molecular-dynamics. For example:
+
+```shell
+janus md --ensemble nvt --struct tests/data/NaCl.cif --temp-start 20 --temp-end 300 --temp-step 20 --temp-time 10 --steps 1000 --temp 300
+```
+
+This performs the same initial heating, before running a further 1000 steps (1 ps) at 300K.
+
+
 ### Using configuration files
 
 Default values for all command line options may be specifed through a Yaml 1.1 formatted configuration file by adding the `--config` option. If an option is present in both the command line and configuration file, the command line value takes precedence.
 
 For example, with the following configuration file and command:
 
 ```yaml
@@ -222,8 +243,9 @@
 [docs-link]: https://stfc.github.io/janus-core/
 [pypi-badge]: https://badge.fury.io/py/janus-core.svg
 [pypi-link]: https://badge.fury.io/py/janus-core
 [license-badge]: https://img.shields.io/badge/License-BSD_3--Clause-blue.svg
 [license-link]: https://opensource.org/licenses/BSD-3-Clause
 [doi-link]: https://zenodo.org/badge/latestdoi/754081470
 [doi-badge]: https://zenodo.org/badge/754081470.svg
+[logo]: https://raw.githubusercontent.com/stfc/janus-core/main/docs/source/images/janus-core-100.png
```

