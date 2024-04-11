# Comparing `tmp/q1simulator-0.9.1.tar.gz` & `tmp/q1simulator-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\q1simulator-0.9.1.tar", last modified: Mon Jul 10 09:36:19 2023, max compression
+gzip compressed data, was "dist\q1simulator-0.9.4.tar", last modified: Thu Aug  3 11:26:54 2023, max compression
```

## Comparing `q1simulator-0.9.1.tar` & `q1simulator-0.9.4.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxrwxrwx   0        0        0        0 2023-07-10 09:36:19.000000 q1simulator-0.9.1/
--rw-rw-rw-   0        0        0     1092 2021-12-09 11:11:44.000000 q1simulator-0.9.1/LICENSE
--rw-rw-rw-   0        0        0      209 2023-07-10 09:36:19.000000 q1simulator-0.9.1/PKG-INFO
--rw-rw-rw-   0        0        0     8162 2023-07-10 09:33:00.000000 q1simulator-0.9.1/README.md
-drwxrwxrwx   0        0        0        0 2023-07-10 09:36:19.000000 q1simulator-0.9.1/q1simulator/
--rw-rw-rw-   0        0        0      178 2023-07-10 09:35:50.000000 q1simulator-0.9.1/q1simulator/__init__.py
--rw-rw-rw-   0        0        0     4843 2023-03-13 17:18:47.000000 q1simulator-0.9.1/q1simulator/cluster.py
--rw-rw-rw-   0        0        0    11391 2023-05-02 14:09:38.000000 q1simulator-0.9.1/q1simulator/q1core.py
--rw-rw-rw-   0        0        0     6365 2023-06-30 08:34:39.000000 q1simulator-0.9.1/q1simulator/q1parser.py
--rw-rw-rw-   0        0        0    15504 2023-04-28 13:04:44.000000 q1simulator-0.9.1/q1simulator/q1sequencer.py
--rw-rw-rw-   0        0        0     9060 2023-07-10 09:20:17.000000 q1simulator-0.9.1/q1simulator/q1simulator.py
--rw-rw-rw-   0        0        0     2102 2023-03-13 17:18:47.000000 q1simulator-0.9.1/q1simulator/q1viewer.py
--rw-rw-rw-   0        0        0      613 2023-03-13 17:18:47.000000 q1simulator-0.9.1/q1simulator/qblox_version.py
--rw-rw-rw-   0        0        0    20159 2023-07-10 09:26:54.000000 q1simulator-0.9.1/q1simulator/rt_renderer.py
--rw-rw-rw-   0        0        0     2004 2023-03-13 17:18:47.000000 q1simulator-0.9.1/q1simulator/trigger_sorting.py
--rw-rw-rw-   0        0        0     1213 2023-03-13 17:18:47.000000 q1simulator-0.9.1/q1simulator/triggers.py
-drwxrwxrwx   0        0        0        0 2023-07-10 09:36:19.000000 q1simulator-0.9.1/q1simulator.egg-info/
--rw-rw-rw-   0        0        0      209 2023-07-10 09:36:18.000000 q1simulator-0.9.1/q1simulator.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      517 2023-07-10 09:36:19.000000 q1simulator-0.9.1/q1simulator.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-07-10 09:36:18.000000 q1simulator-0.9.1/q1simulator.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       25 2023-07-10 09:36:19.000000 q1simulator-0.9.1/q1simulator.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-07-10 09:36:19.000000 q1simulator-0.9.1/q1simulator.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       74 2023-07-10 09:36:19.000000 q1simulator-0.9.1/setup.cfg
--rw-rw-rw-   0        0        0      377 2023-07-10 09:35:50.000000 q1simulator-0.9.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-07-10 09:36:19.000000 q1simulator-0.9.1/test/
--rw-rw-rw-   0        0        0     4585 2023-03-13 17:18:47.000000 q1simulator-0.9.1/test/test_conditional.py
+drwxrwxrwx   0        0        0        0 2023-08-03 11:26:54.000000 q1simulator-0.9.4/
+-rw-rw-rw-   0        0        0     1092 2021-12-09 11:11:44.000000 q1simulator-0.9.4/LICENSE
+-rw-rw-rw-   0        0        0      209 2023-08-03 11:26:54.000000 q1simulator-0.9.4/PKG-INFO
+-rw-rw-rw-   0        0        0     8162 2023-07-10 09:37:22.000000 q1simulator-0.9.4/README.md
+drwxrwxrwx   0        0        0        0 2023-08-03 11:26:54.000000 q1simulator-0.9.4/q1simulator/
+-rw-rw-rw-   0        0        0      178 2023-08-03 11:26:42.000000 q1simulator-0.9.4/q1simulator/__init__.py
+-rw-rw-rw-   0        0        0     5280 2023-07-28 07:46:46.000000 q1simulator-0.9.4/q1simulator/cluster.py
+-rw-rw-rw-   0        0        0    11735 2023-08-03 07:34:50.000000 q1simulator-0.9.4/q1simulator/q1core.py
+-rw-rw-rw-   0        0        0     6783 2023-08-03 07:28:19.000000 q1simulator-0.9.4/q1simulator/q1parser.py
+-rw-rw-rw-   0        0        0    15597 2023-08-03 10:25:33.000000 q1simulator-0.9.4/q1simulator/q1sequencer.py
+-rw-rw-rw-   0        0        0     9383 2023-07-28 07:46:13.000000 q1simulator-0.9.4/q1simulator/q1simulator.py
+-rw-rw-rw-   0        0        0     2102 2023-03-13 17:18:47.000000 q1simulator-0.9.4/q1simulator/q1viewer.py
+-rw-rw-rw-   0        0        0      613 2023-07-21 14:11:55.000000 q1simulator-0.9.4/q1simulator/qblox_version.py
+-rw-rw-rw-   0        0        0    20731 2023-08-03 10:27:31.000000 q1simulator-0.9.4/q1simulator/rt_renderer.py
+-rw-rw-rw-   0        0        0     2004 2023-07-20 07:51:46.000000 q1simulator-0.9.4/q1simulator/trigger_sorting.py
+-rw-rw-rw-   0        0        0     1286 2023-07-17 14:16:36.000000 q1simulator-0.9.4/q1simulator/triggers.py
+drwxrwxrwx   0        0        0        0 2023-08-03 11:26:54.000000 q1simulator-0.9.4/q1simulator.egg-info/
+-rw-rw-rw-   0        0        0      209 2023-08-03 11:26:53.000000 q1simulator-0.9.4/q1simulator.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      543 2023-08-03 11:26:53.000000 q1simulator-0.9.4/q1simulator.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-08-03 11:26:53.000000 q1simulator-0.9.4/q1simulator.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       25 2023-08-03 11:26:53.000000 q1simulator-0.9.4/q1simulator.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-08-03 11:26:53.000000 q1simulator-0.9.4/q1simulator.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2023-08-03 11:26:54.000000 q1simulator-0.9.4/setup.cfg
+-rw-rw-rw-   0        0        0      377 2023-08-03 11:26:42.000000 q1simulator-0.9.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-08-03 11:26:54.000000 q1simulator-0.9.4/test/
+-rw-rw-rw-   0        0        0     4589 2023-07-17 14:16:36.000000 q1simulator-0.9.4/test/test_conditional.py
+-rw-rw-rw-   0        0        0     6669 2023-07-21 14:11:55.000000 q1simulator-0.9.4/test/test_conditional2.py
```

### Comparing `q1simulator-0.9.1/LICENSE` & `q1simulator-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `q1simulator-0.9.1/README.md` & `q1simulator-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `q1simulator-0.9.1/q1simulator/cluster.py` & `q1simulator-0.9.4/q1simulator/cluster.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import qcodes as qc
 
 from qblox_instruments import (
         SystemStatus, SystemState, SystemStatusSlotFlags,
         InstrumentClass, InstrumentType,
         )
 
+from .qblox_version import check_qblox_instrument_version
 from .q1simulator import Q1Module
 from .triggers import TriggerDistributor
 from .trigger_sorting import get_seq_trigger_info, sort_sequencers
 
 logger = logging.getLogger(__name__)
 
 
@@ -21,14 +22,15 @@
         super().__init__(root_instrument, name)
         self._slot = slot
         super().init_module(n_sequencers, sim_type)
 
     def present(self):
         return True
 
+    @property
     def slot_idx(self):
         return self._slot
 
 
 class EmptySlot(qc.InstrumentChannel):
     def __init__(self, root_instrument, name):
         super().__init__(root_instrument, name)
@@ -37,25 +39,33 @@
         return False
 
 
 class Cluster(qc.Instrument):
     _cluster_parameters = [
         'trigger_monitor_latest',
         ]
+    _log_only_params = [
+        'led_brightness',
+        ]
 
     def __init__(self, name, modules={}):
+        check_qblox_instrument_version()
         super().__init__(name)
 
         # TODO return trigger count
         for par_name in self._cluster_parameters:
             self.add_parameter(par_name, set_cmd=partial(self._set, par_name))
         for i in range(1,16):
             par_name = f'trigger{i}_monitor_count'
             self.add_parameter(par_name, set_cmd=partial(self._set, par_name))
 
+        for par_name in self._log_only_params:
+            self.add_parameter(par_name,
+                               set_cmd=partial(self._log_set, par_name))
+
         self._modules = {}
         for slot in range(1,21):
             name = f'module{slot}'
             if slot in modules:
                 module = ClusterModule(self, name, slot, sim_type=modules[slot])
             else:
                 module = EmptySlot(self, name)
@@ -141,7 +151,9 @@
     @property
     def modules(self):
         return list(self.submodules.values())
 
     def reset(self):
         pass
 
+    def _log_set(self, name, value):
+        logger.info(f'{self.name}: {name}={value}')
```

### Comparing `q1simulator-0.9.1/q1simulator/q1core.py` & `q1simulator-0.9.4/q1simulator/q1core.py`

 * *Files 18% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 
 class Abort(Exception):
     pass
 
 class Illegal(Exception):
     pass
 
+
 class Q1Core:
     def __init__(self, name, renderer, is_qrm):
         self.name = name
         self.renderer = renderer
         self._is_qrm = is_qrm
         self.max_core_cycles= 10_000_000
         self.render_repetitions = True
@@ -57,31 +58,36 @@
 
         if len(self.instructions) == 0:
             print(f'*** No instructions loaded')
             self._error('SEQUENCE PROCESSOR Q1 ILLEGAL INSTRUCTION')
             return
 
         for instr in self.instructions:
-            instr.func = getattr(self, instr.func_name)
+            try:
+                instr.func = getattr(self, instr.func_name)
+            except AttributeError as ex:
+                msg = f'Illegal instruction at line {instr.text_line_nr}: {ex}'
+                self._print_error_msg(msg, instr, 0)
+                self._error('SEQUENCE PROCESSOR Q1 ILLEGAL INSTRUCTION')
+                return
 
         start = time.perf_counter()
         try:
             cntr = 0
             while(True):
                 cntr += 1
                 instr = self.instructions[self.iptr]
                 self.iptr += 1
                 if instr.reg_args is not None:
                     args = instr.args.copy()
                     for i in instr.reg_args:
                         args[i] = self.R[args[i]]
-                        # add 1 clock tick for every register access
-                        self.clock.add_ticks(1)
                 else:
                     args = instr.args
+                self.clock.add_ticks(instr.clock_ticks)
                 instr.func(*args)
                 if self.iptr >= len(self.instructions):
                     raise Illegal(f'No instruction at {self.iptr:04}')
                 if cntr >= self.max_core_cycles:
                     raise Abort('Core cycle limited exceeded',
                                 'FORCED STOP')
         except Halt:
@@ -131,143 +137,146 @@
     def _illegal(self):
         raise Illegal('illegal instruction')
 
     def _stop(self):
         raise Halt('stop instruction')
 
     def _nop(self):
-        self.clock.add_ticks(1)
+        pass
 
     def _jmp(self, label):
-        self.clock.add_ticks(4)
+        # 3 cycles for jump
+        self.clock.add_ticks(3)
         self.iptr = label
 
     def _jlt(self, value, n, label):
-        self.clock.add_ticks(4)
+        # 2 cycles for arithmetic
+        self.clock.add_ticks(2)
         if value < n:
+            # 3 cycles for jump
+            self.clock.add_ticks(3)
             self.iptr = label
 
     def _jge(self, value, n, label):
-        self.clock.add_ticks(4)
+        # 2 cycles for arithmetic
+        self.clock.add_ticks(2)
         if value >= n:
+            # 3 cycles for jump
+            self.clock.add_ticks(3)
             self.iptr = label
 
     def _loop(self, register, label):
-        self.clock.add_ticks(5)
+        # 2 cycles for arithmetic
+        self.clock.add_ticks(2)
         self._set_register(register, self.R[register] - 1)
         instr = self.instructions[self.iptr-1]
         if not self.render_repetitions and instr.arglist[1] == '@_start':
             logger.info('Skipping repetitions')
             return
         if self.R[register] != 0:
+            # 3 cycles for jump
+            self.clock.add_ticks(3)
             self.iptr = label
 
     def _move(self, source, destination):
-        self.clock.add_ticks(1)
         self._set_register(destination, source)
 
     def _not(self, source, destination):
+        # 2 cycles for arithmetic
         self.clock.add_ticks(2)
         self._set_register(destination, ~source)
 
     def _add(self, lhs, rhs, destination):
+        # 2 cycles for arithmetic
         self.clock.add_ticks(2)
         self._set_register(destination, lhs + rhs)
 
     def _sub(self, lhs, rhs, destination):
+        # 2 cycles for arithmetic
         self.clock.add_ticks(2)
         self._set_register(destination, lhs - rhs)
 
     def _and(self, lhs, rhs, destination):
+        # 2 cycles for arithmetic
         self.clock.add_ticks(2)
         self._set_register(destination, lhs & rhs)
 
     def _or(self, lhs, rhs, destination):
+        # 2 cycles for arithmetic
         self.clock.add_ticks(2)
         self._set_register(destination, lhs | rhs)
 
     def _xor(self, lhs, rhs, destination):
+        # 2 cycles for arithmetic
         self.clock.add_ticks(2)
         self._set_register(destination, lhs ^ rhs)
 
     def _asl(self, lhs, rhs, destination):
+        # 2 cycles for arithmetic
         self.clock.add_ticks(2)
         self._set_register(destination, lhs << rhs)
 
     def _asr(self, lhs, rhs, destination):
+        # 2 cycles for arithmetic
         self.clock.add_ticks(2)
         self._set_register(destination, lhs >> rhs)
 
     def _set_mrk(self, value):
-        self.clock.add_ticks(1)
         self.renderer.set_mrk(value)
 
     def _set_freq(self, freq):
-        self.clock.add_ticks(1)
         self.renderer.set_freq(freq)
 
     def _reset_ph(self):
-        self.clock.add_ticks(1)
         self.renderer.reset_ph()
 
     def _set_ph(self, phase):
-        self.clock.add_ticks(1)
         self.renderer.set_ph(phase)
 
     def _set_ph_delta(self, phase_delta):
-        self.clock.add_ticks(1)
         self.renderer.set_ph_delta(phase_delta)
 
     def _set_awg_gain(self, gain0, gain1):
-        self.clock.add_ticks(1)
         self.renderer.set_awg_gain(gain0, gain1)
 
     def _set_awg_offs(self, offset0, offset1):
-        self.clock.add_ticks(1)
         self.renderer.set_awg_offs(offset0, offset1)
 
     def _set_cond(self, enable, mask, op, else_wait):
         self.renderer.set_cond(enable, mask, op, else_wait)
 
     def _upd_param(self, wait_after):
-        self.clock.add_ticks(1)
         self.clock.schedule_rt(self.renderer.time)
         self.renderer.upd_param(wait_after)
 
     def _play(self, wave0, wave1, wait_after):
-        self.clock.add_ticks(1)
         self.clock.schedule_rt(self.renderer.time)
         self.renderer.play(wave0, wave1, wait_after)
 
     def _acquire(self, bins, bin_index, wait_after):
         if not self._is_qrm:
             raise NotImplementedError('instrument type is not QRM')
-        self.clock.add_ticks(1)
         self.clock.schedule_rt(self.renderer.time)
         self.renderer.acquire(bins, bin_index, wait_after)
 
     def _acquire_weighed(self, bins, bin_index, weight0, weight1, wait_after):
         if not self._is_qrm:
             raise NotImplementedError('instrument type is not QRM')
-        self.clock.add_ticks(1)
         self.clock.schedule_rt(self.renderer.time)
         self.renderer.acquire_weighed(bins, bin_index, weight0, weight1, wait_after)
 
-    def _latch_en(self, enable, wait_after):
-        self.clock.add_ticks(1)
+    def _set_latch_en(self, enable, wait_after):
         self.clock.schedule_rt(self.renderer.time)
-        self.renderer.latch_en(enable, wait_after)
+        self.renderer.set_latch_en(enable, wait_after)
 
     def _latch_rst(self, wait):
-        self.clock.add_ticks(1)
         self.clock.schedule_rt(self.renderer.time)
         self.renderer.latch_rst(wait)
 
     def _wait(self, time):
-        self.clock.add_ticks(1)
         self.clock.schedule_rt(self.renderer.time)
         self.renderer.wait(time)
 
     def _wait_sync(self, wait_after):
         # assume wait_sync pauses the RT exec for at least 200 ns = 50 ticks
         self.clock.add_ticks(-50)
         self.renderer.wait_sync(wait_after)
@@ -297,14 +306,15 @@
         if 'T' in options:
             time_str = f' q1:{self.clock.core_time:6} rt:{self.renderer.time:6} ns'
         print(f'{msg}: {value_str}{time_str}')
 
     def _sim_trigger(self, addr, value):
         self.renderer.sim_trigger(addr, value)
 
+
 class CoreClock:
     def __init__(self):
         self.rt_buffer = deque()
         self.core_time = 0
 
     def add_ticks(self, value):
         self.core_time += value * 4
@@ -327,8 +337,8 @@
         # q1core halts when buffer is full
         if len(b) >= 16:
             # q1core will continue when an instruction is read from buffer.
             # When q1core continues the time advantage is `time` - popped time.
             # So, core time will be equal to popped time
             self.core_time = b.popleft()
 
-        self.rt_buffer.append(time)
+        b.append(time)
```

### Comparing `q1simulator-0.9.1/q1simulator/q1parser.py` & `q1simulator-0.9.4/q1simulator/q1parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     mnemonic: str
     arglist: Optional[Tuple[str]] = None
     label: Optional[str] = None
     args: List[Union[int,str]] = None
     reg_args: List[int] = None
     func_name: Optional[str] = None
     func: Any = None
+    clock_ticks: int = 1
 
 
 class AsmSyntaxError(Exception):
     pass
 
 # I = immediate, R = register, L = label, D = destination register
 mnemonic_args = {
@@ -44,15 +45,15 @@
     'set_awg_gain': 'IR,IR',
     'set_awg_offs': 'IR,IR',
     'set_cond': 'IR,IR,IR,I',
     'upd_param': 'I',
     'play': 'IR,IR,I',
     'acquire': 'I,IR,I',
     'acquire_weighed': 'I,IR,IR,IR,I',
-    'latch_en': 'IR,I',
+    'set_latch_en': 'IR,I',
     'latch_rst': 'IR',
     'wait': 'IR',
     'wait_sync': 'IR',
     'wait_trigger': 'IR',
     'sw_req': 'IR',
     }
 
@@ -85,14 +86,20 @@
             func_name = '_' + mnemonic
             instr.func_name = func_name
             if mnemonic in mnemonic_args:
                 try:
                     args,reg_args = self._evaluate_args(mnemonic_args[mnemonic], instr.arglist)
                     instr.args = args
                     instr.reg_args = reg_args
+                    if reg_args and mnemonic not in ['jmp', 'jge', 'jlt', 'loop']:
+                        # 1 cycle for every register. instr and 1st register are loaded in 1 cycle
+                        instr.clock_ticks = len(reg_args)
+                    else:
+                        # 1 cycle to load instruction
+                        instr.clock_ticks = 1
                 except AsmSyntaxError as ex:
                     print(ex)
                     print(lines[instr.text_line_nr])
                     raise
             else:
                 instr.args = instr.arglist
 
@@ -122,15 +129,15 @@
         match = re.fullmatch(instr_pattern, line)
         if match:
             label = match.group(1)
             if label:
                 label = label[:-1]
             args = match.group(3).strip()
             if args:
-                arglist = args.split(',')
+                arglist = args.replace(' ','').split(',')
             else:
                 arglist = []
             return [label, match.group(2), arglist]
         raise Exception(f'{self.name}: Parse error on line: {org_line}')
 
     def _parse_simcmd(self, command):
         command = command.strip()
```

### Comparing `q1simulator-0.9.1/q1simulator/q1sequencer.py` & `q1simulator-0.9.4/q1simulator/q1sequencer.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,14 +107,16 @@
         elif name == 'max_core_cycles':
             self.q1core.max_core_cycles = value
         elif name == 'trace':
             self._trace = value
             self.rt_renderer.trace_enabled = value
         elif name == 'render_repetitions':
             self.q1core.render_repetitions = value
+        elif name == 'skip_wait_sync':
+            self.rt_renderer.skip_wait_sync = value
 
     def reset(self):
         self.waveforms = {}
         self.weights = {}
         self.acquisition_bins = {}
         self._mock_data = {}
         self._trigger_events = []
```

### Comparing `q1simulator-0.9.1/q1simulator/q1simulator.py` & `q1simulator-0.9.4/q1simulator/q1simulator.py`

 * *Files 1% similar despite different names*

```diff
@@ -70,15 +70,14 @@
         'scope_acq_avg_mode_en_path1',
         ]
 
     # NOTE: No __init__() !!!
     # This class is used as a mixin. Although quite heavy mixin.
 
     def init_module(self, n_sequencers=6, sim_type=None):
-        check_qblox_instrument_version()
         self._sim_type = sim_type
         if sim_type is None:
             raise Exception('sim_type must be specified')
 
         self._is_qcm = sim_type in ['QCM', 'QCM-RF', 'Viewer']
         self._is_qrm = sim_type in ['QRM', 'QRM-RF', 'Viewer']
         self._is_rf = sim_type in ['QCM-RF', 'QRM-RF']
@@ -224,22 +223,30 @@
         self.sequencers[seq_nr].print_registers(reg_nrs)
 
 
 class Q1Simulator(qc.Instrument, Q1Module):
     _pulsar_parameters = [
         'reference_source',
         ]
+    _log_only_params = [
+        'led_brightness',
+        ]
 
     def __init__(self, name, n_sequencers=6, sim_type=None):
+        check_qblox_instrument_version()
         super().__init__(name)
         super().init_module(n_sequencers, sim_type)
 
         for par_name in self._pulsar_parameters:
             self.add_parameter(par_name, set_cmd=partial(self._set, par_name))
 
+        for par_name in self._log_only_params:
+            self.add_parameter(par_name,
+                               set_cmd=partial(self._log_set, par_name))
+
     def get_idn(self):
         return dict(vendor='Q1Simulator', model=self._sim_type, serial='', firmware='')
 
     @property
     def instrument_class(self):
         return InstrumentClass.PULSAR
 
@@ -263,7 +270,10 @@
         trigger_dist = TriggerDistributor()
         seq_infos = sort_sequencers(seq_infos)
         for seq_info in seq_infos:
             seq = seq_info.module.sequencers[seq_info.seq_number]
             seq.set_trigger_events(trigger_dist.get_trigger_events())
             seq.run()
             trigger_dist.add_emitted_triggers(seq.get_acq_trigger_events())
+
+    def _log_set(self, name, value):
+        logger.info(f'{self.name}: {name}={value}')
```

### Comparing `q1simulator-0.9.1/q1simulator/q1viewer.py` & `q1simulator-0.9.4/q1simulator/q1viewer.py`

 * *Files identical despite different names*

### Comparing `q1simulator-0.9.1/q1simulator/qblox_version.py` & `q1simulator-0.9.4/q1simulator/qblox_version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 from qblox_instruments import __version__ as qblox_version_str
 from packaging.version import Version
 from q1simulator import __version__ as q1simulator_version
 
 def check_qblox_instrument_version():
     if qblox_version >= Version('0.10'):
-        print(f'WARNING Q1Simulator {q1simulator_version} simulates qblox_instruments v0.8.x, '
+        print(f'WARNING Q1Simulator {q1simulator_version} simulates qblox_instruments v0.9.x, '
               f'but qblox_instruments version {qblox_version} is installed')
     elif qblox_version < Version('0.8'):
         raise Exception('Q1Simulator {q1simulator_version} expects qblox_instruments version v0.8+')
 
 qblox_version = Version(qblox_version_str)
```

### Comparing `q1simulator-0.9.1/q1simulator/rt_renderer.py` & `q1simulator-0.9.4/q1simulator/rt_renderer.py`

 * *Files 3% similar despite different names*

```diff
@@ -88,14 +88,15 @@
         self.nco_frequency = 0.0
         self.mod_en_awg = False
         self.mixer_gain_ratio = 1.0
         self.mixer_phase_offset_degree = 0.0
         self.delete_acquisition_data_all()
         self.reset()
         self.trace_enabled = False
+        self.skip_wait_sync = True
         self.threshold_count = np.full(15, 2^16-1, dtype=np.uint16)
         self.threshold_invert = np.zeros(15, dtype=bool)
         self.acq_conf = AcqConf()
 
     def reset(self):
         self.settings = Settings()
         self.next_settings = Settings()
@@ -215,15 +216,15 @@
                               self.time + len(self.waves[1]))
         self._render(wait_after)
 
     @check_conditional
     def acquire(self, bins, bin_index, wait_after):
         self._update_settings()
         if self.trace_enabled:
-            self._trace(f'Acquire {bins} {bin_index}')
+            self._trace(f'Acquire {bins} {bin_index} ({self.acq_conf.length} ns)')
         self._add_acquisition(bins, bin_index, self.acq_conf.length)
         self._render(wait_after)
 
     @check_conditional
     def acquire_weighed(self, bins, bin_index, weight0, weight1, wait_after):
         self._update_settings()
         if self.trace_enabled:
@@ -243,14 +244,16 @@
     @check_conditional
     def wait(self, time):
         if self.trace_enabled:
             self._trace(f'Wait {time}')
         self._render(time)
 
     def wait_sync(self, wait_after):
+        if self.skip_wait_sync:
+            return
         self._render(wait_after)
 
     def set_cond(self, enable, mask, op, else_wait):
         if not enable:
             self._trace(f'Cond disabled')
             self.skip_rt = False
             return
@@ -270,27 +273,27 @@
             match = bits_set != bits_mask
         elif op == 4: # XOR
             match = (bits_set%2) == 1
         elif op == 5: # XNOR
             match = (bits_set%2) == 0
         else:
             raise Exception(f'Unknown operator {op}')
-        logger.info(f'set_cond 1, {mask}, {op}, {else_wait}')
-        logger.info(f'latches: {self.latch_regs}')
-        logger.info(f'mask:    {mask_ar}')
-        logger.info(f'state:   {state}')
-        logger.info(f'cond:    {match}')
-        self._trace(f'Cond {match}')
+        logger.debug(f'set_cond 1, {mask}, {op}, {else_wait}')
+        logger.debug(f'latches: {self.latch_regs}')
+        logger.debug(f'mask:    {mask_ar}')
+        logger.debug(f'state:   {state}')
+        logger.debug(f'cond:    {match}')
+        self._trace(f'Cond {match} {state}')
         self.skip_rt = not match
         self.else_wait = else_wait
 
     def _else_wait(self, *args, **kwargs):
         self._render(self.else_wait)
 
-    def latch_en(self, enable, wait_after):
+    def set_latch_en(self, enable, wait_after):
         if self.trace_enabled:
             self._trace(f'Latch {"on" if enable else "off"}')
         self._process_triggers()
         self.latch_enabled = enable
         self._render(wait_after)
 
     def latch_rst(self, wait):
@@ -351,25 +354,29 @@
             self._render_marker(old.marker, new.marker)
         # copy marker, offset and gain
         self.settings = copy(self.next_settings)
 
     def _render_marker(self, old_marker, new_marker):
         for i in range(4):
             m = 1 << i
-            m_old = old_marker & m
-            m_new = new_marker & m
+            m_old = (old_marker & m) != 0
+            m_new = (new_marker & m) != 0
             if m_new != m_old:
                 l = self.marker_out[i]
                 if self.time < self.max_render_time:
                     l += [[self.time, m_old], [self.time, m_new]]
                 elif l[-1][0] < self.max_render_time:
                     # add final marker step
                     l += [[self.max_render_time, m_old], [self.max_render_time, 0]]
 
     def _render(self, time):
+        if time < 4:
+            logger.error(f'{self.name}: wait_time ({time} ns) must be >= 4 ns')
+            self._error('WAIT TIME < 4 ns')
+
         if time & 0x0003:
             logger.error(f'{self.name}: wait time not aligned on '
                           f'4 ns boundary: {time} ns (offset={time&0x03} ns)')
             self._error('TIME NOT ALIGNED')
 
         # 16 bits, 4 ns resolution
         time &= 0xFFFC
@@ -430,14 +437,15 @@
         t = self.time
         # TODO Refactor trigger distribution. Request triggers for interval.
         while len(self.trigger_events) > 0 and self.trigger_events[0].time <= t:
             trigger = self.trigger_events.pop(0)
             if self.latch_enabled:
                 index = trigger.addr-1
                 self.latch_regs[index] += trigger.state
+                self._trace(f'Latch reg {index} {trigger.state:+d} -> {self.latch_regs[index]}')
 
     def _get_acq_data(self, bins, default):
         mock_data_iter = self.mock_data.get(bins, None)
         if mock_data_iter is None:
             return (default, default)
         else:
             try:
@@ -475,32 +483,34 @@
         if bin_index >= self.acq_bins[bins]:
             self._error('ACQ BIN INDEX INVALID')
             return
         if not self.acq_buffer.add(t):
             self._error('ACQ BINNING FIFO ERROR')
             return
         acq_conf = self.acq_conf
-        value = self._get_acq_data(bins, t)
+        value = self._get_acq_data(bins, t/1e6)
         angle = acq_conf.rotation/180*np.pi
         rot_value = value[0]*np.cos(angle) + value[1]*np.sin(angle)
         state = rot_value >= acq_conf.threshold
+        self._trace(f'Acq result {state}, {rot_value}, {acq_conf.threshold}')
 
         if self.acq_count[bins][bin_index] == 0:
             self.acq_data[bins][bin_index] = value
             self.acq_thresholded[bins][bin_index] = state
         else:
             self.acq_data[bins][bin_index] += value
             self.acq_thresholded[bins][bin_index] += state
         self.acq_count[bins][bin_index] += 1
 
         if acq_conf.trigger_en:
             t_end = t + duration
             trigger_state = state ^ acq_conf.trigger_invert
             # TODO also add to trigger events. Part of TriggerDistributor redesign.
-            self.acq_trigger_events.append(TriggerEvent(acq_conf.addr, t_end, trigger_state))
+            self.acq_trigger_events.append(TriggerEvent(acq_conf.trigger_addr, t_end, trigger_state))
+            self._trace(f'Trigger {acq_conf.trigger_addr} {t_end} {trigger_state}')
 
     def _trace(self, msg):
         if self.trace_enabled:
             print(f'{self.time:-6} {msg}')
 
     def plot(self, v_max):
         scaling = v_max/2**15
```

### Comparing `q1simulator-0.9.1/q1simulator/trigger_sorting.py` & `q1simulator-0.9.4/q1simulator/trigger_sorting.py`

 * *Files identical despite different names*

### Comparing `q1simulator-0.9.1/q1simulator/triggers.py` & `q1simulator-0.9.4/q1simulator/triggers.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from copy import copy
 import math
 from dataclasses import dataclass
 from typing import List
 
 @dataclass
 class TriggerEvent:
     '''
@@ -10,20 +11,23 @@
         The simulator also sends events with state == 0.
         This allows worst case timing checks.
     '''
     addr: int
     time: int # time in ns
     state: bool
 
-    def with_delay(self, delay=200, alignment=20):
+    def with_delay(self, delay=220, alignment=28):
         res = self.copy()
         res.time = math.ceil(res.time / alignment) * alignment
         res.time += delay
         return res
 
+    def copy(self):
+        return copy(self)
+
 # TODO Refactor trigger distributor into runtime distributor
 # Run till sequencer calls set_cond. Block it and let others run.
 # Sequencer may resume when all other sequencers are at least at equal time.
 
 class TriggerDistributor:
     def __init__(self):
         self.trigger_events: List[TriggerEvent] = []
```

### Comparing `q1simulator-0.9.1/q1simulator.egg-info/SOURCES.txt` & `q1simulator-0.9.4/q1simulator.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -14,8 +14,9 @@
 q1simulator/trigger_sorting.py
 q1simulator/triggers.py
 q1simulator.egg-info/PKG-INFO
 q1simulator.egg-info/SOURCES.txt
 q1simulator.egg-info/dependency_links.txt
 q1simulator.egg-info/requires.txt
 q1simulator.egg-info/top_level.txt
-test/test_conditional.py
+test/test_conditional.py
+test/test_conditional2.py
```

### Comparing `q1simulator-0.9.1/test/test_conditional.py` & `q1simulator-0.9.4/test/test_conditional.py`

 * *Files 0% similar despite different names*

```diff
@@ -77,15 +77,15 @@
 
 sim = init()
 
 #%%
 sim.reset()
 program='''
 wait_sync 100
-latch_en 1,4
+set_latch_en 1,4
 #Q1Sim:sim_trigger 1, 1
 
 play 0,0,92 # subtract 8 for next conditional
 
 set_cond 1, 1, 0, 4
 wait 8 # 4ns * number of statements including this wait
 play 0,1,72 # subtract 8 ns for next conditional
```

