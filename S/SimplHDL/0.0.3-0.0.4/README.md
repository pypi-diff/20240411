# Comparing `tmp/SimplHDL-0.0.3.tar.gz` & `tmp/SimplHDL-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "SimplHDL-0.0.3.tar", last modified: Fri Apr  5 12:19:54 2024, max compression
+gzip compressed data, was "SimplHDL-0.0.4.tar", last modified: Thu Apr 11 13:40:01 2024, max compression
```

## Comparing `SimplHDL-0.0.3.tar` & `SimplHDL-0.0.4.tar`

### file list

```diff
@@ -1,228 +1,228 @@
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.261170 SimplHDL-0.0.3/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.225170 SimplHDL-0.0.3/.github/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.233170 SimplHDL-0.0.3/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/.gitignore
--rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/.readthedocs.yaml
--rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-05 12:19:54.261170 SimplHDL-0.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.233170 SimplHDL-0.0.3/docs/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.233170 SimplHDL-0.0.3/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (127)    50717 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/_static/simplhdl_dark.png
--rw-r--r--   0 runner    (1001) docker     (127)   111558 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/_static/simplhdl_light.png
--rw-r--r--   0 runner    (1001) docker     (127)    38948 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/_static/simplhdl_light_1.png
--rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (127)    20233 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/drawing.svg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.237170 SimplHDL-0.0.3/docs/flows/
--rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/flows/ghdl.rst
--rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/flows/icarus.rst
--rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/flows/quartus.rst
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/flows/questasim.rst
--rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/flows/vcs.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/flows/vivado.rst
--rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/flows/xsim.rst
--rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/flows.rst
--rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/intel-ips.md
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/introduction.rst
--rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/plugins.rst
--rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/docs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.229170 SimplHDL-0.0.3/examples/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.229170 SimplHDL-0.0.3/examples/hdl/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.237170 SimplHDL-0.0.3/examples/hdl/adder/
--rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/adder/adder.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.237170 SimplHDL-0.0.3/examples/hdl/adder/hdl/
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/adder/hdl/adder.sv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.237170 SimplHDL-0.0.3/examples/hdl/adder/sim/
--rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/adder/sim/testbench.sv
--rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/adder/sim/testbench.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.237170 SimplHDL-0.0.3/examples/hdl/adder/syn/
--rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/adder/syn/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/adder/syn/placement.xdc
--rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/adder/syn/timing.xdc
--rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/adder/syn/top.sv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.237170 SimplHDL-0.0.3/examples/hdl/alu/
--rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/alu.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.237170 SimplHDL-0.0.3/examples/hdl/alu/hdl/
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/hdl/add.sv
--rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/hdl/alu.sv
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/hdl/mul.sv
--rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/hdl/sub.sv
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.225170 SimplHDL-0.0.3/examples/hdl/alu/sim/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.237170 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.241170 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/alu_vip/
--rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/alu_vip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/alu_vip/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/alu_vip/aluif.py
--rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/alu_vip/driver.py
--rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/alu_vip/monitor.py
--rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/alu_vip/sequenceitem.py
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/alu_vip/sequencer.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.241170 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/clock_vip/
--rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/clock_vip/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/clock_vip/agent.py
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/clock_vip/clockif.py
--rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/pyuvm.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.241170 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/test/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/test/env.py
--rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/test/seq_lib.py
--rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/test/test.py
--rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/testbench.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.225170 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.241170 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/alu_vip/
--rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/alu_vip/agent.svh
--rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/alu_vip/alu_vip.sv
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/alu_vip/alu_vip.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/alu_vip/driver.svh
--rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/alu_vip/env.svh
--rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/alu_vip/monitor.svh
--rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/alu_vip/sequence_item.svh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.241170 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/tb_env/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.241170 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/tb_env/seq_lib/
--rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/tb_env/seq_lib/add_seq.svh
--rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/tb_env/seq_lib/base_seq.svh
--rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/tb_env/tb_env.sv
--rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/tb_env/tb_env.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.241170 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/tb_env/test/
--rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/tb_env/test/base_test.svh
--rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/tb_env/test/test_add.svh
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.245170 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/testbench/
--rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/testbench/alu_if.sv
--rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/testbench/testbench.sv
--rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/testbench/testbench.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.229170 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/testcases/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.245170 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/testcases/test_add/
--rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/testcases/test_add/test_add.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.245170 SimplHDL-0.0.3/examples/hdl/alu/syn/
--rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/syn/build.yml
--rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/syn/placement.xdc
--rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/alu/syn/timing.xdc
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.245170 SimplHDL-0.0.3/examples/hdl/hello/
--rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/hello/build.sbt
--rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/hello/hello.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.229170 SimplHDL-0.0.3/examples/hdl/hello/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.229170 SimplHDL-0.0.3/examples/hdl/hello/src/main/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.245170 SimplHDL-0.0.3/examples/hdl/hello/src/main/scala/
--rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/hello/src/main/scala/Hello.scala
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.245170 SimplHDL-0.0.3/examples/hdl/hello/syn/
--rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/hdl/hello/syn/build.yml
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.229170 SimplHDL-0.0.3/examples/plugins/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.245170 SimplHDL-0.0.3/examples/plugins/simple_parser/
--rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/plugins/simple_parser/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.229170 SimplHDL-0.0.3/examples/plugins/simple_parser/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.245170 SimplHDL-0.0.3/examples/plugins/simple_parser/src/simple_parser/
--rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/plugins/simple_parser/src/simple_parser/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/examples/plugins/simple_parser/src/simple_parser/simple_parser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-05 12:19:54.261170 SimplHDL-0.0.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.229170 SimplHDL-0.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.261170 SimplHDL-0.0.3/src/SimplHDL.egg-info/
--rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-05 12:19:54.000000 SimplHDL-0.0.3/src/SimplHDL.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (127)     6470 2024-04-05 12:19:54.000000 SimplHDL-0.0.3/src/SimplHDL.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-05 12:19:54.000000 SimplHDL-0.0.3/src/SimplHDL.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-05 12:19:54.000000 SimplHDL-0.0.3/src/SimplHDL.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-05 12:19:54.000000 SimplHDL-0.0.3/src/SimplHDL.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-05 12:19:54.000000 SimplHDL-0.0.3/src/SimplHDL.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.249170 SimplHDL-0.0.3/src/simplhdl/
--rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/__main__.py
--rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/cocotb.py
--rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.249170 SimplHDL-0.0.3/src/simplhdl/flows/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/implementationflow.py
--rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/modelsimflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     4468 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/quartusflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.249170 SimplHDL-0.0.3/src/simplhdl/flows/questasim/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/questasim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/questasim/questasimflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.249170 SimplHDL-0.0.3/src/simplhdl/flows/rivierapro/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/rivierapro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     8975 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/rivierapro/rivieraproflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/simulationflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.249170 SimplHDL-0.0.3/src/simplhdl/flows/vcs/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/vcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/vcs/vcsflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/vivadoflow.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.249170 SimplHDL-0.0.3/src/simplhdl/flows/xsim/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/xsim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/flows/xsim/xsimflow.py
--rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.253170 SimplHDL-0.0.3/src/simplhdl/generators/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/generators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/generators/chisel.py
--rw-r--r--   0 runner    (1001) docker     (127)     8484 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/generators/ipxact.py
--rw-r--r--   0 runner    (1001) docker     (127)     6153 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/generators/spd.py
--rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/generators/systemrdl.py
--rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/info.py
--rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/parser.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.253170 SimplHDL-0.0.3/src/simplhdl/parsers/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/parsers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/parsers/fusesocparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/parsers/simplhdlparser.py
--rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.253170 SimplHDL-0.0.3/src/simplhdl/pyedaa/
--rw-r--r--   0 runner    (1001) docker     (127)     3430 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/pyedaa/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/pyedaa/attributes.py
--rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/pyedaa/design.py
--rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/pyedaa/fileset.py
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/pyedaa/filetypes.py
--rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/pyedaa/project.py
--rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/pyedaa/vhdllibrary.py
--rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/repo.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.253170 SimplHDL-0.0.3/src/simplhdl/resources/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.253170 SimplHDL-0.0.3/src/simplhdl/resources/templates/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.253170 SimplHDL-0.0.3/src/simplhdl/resources/templates/quartus/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/quartus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)     2250 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/quartus/project.tcl.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/quartus/run.tcl.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.257170 SimplHDL-0.0.3/src/simplhdl/resources/templates/questasim/
--rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/questasim/Makefile.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/questasim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/questasim/cocotb.mk.j2
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/questasim/dependencies.mk.j2
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/questasim/files.j2
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/questasim/fileset.j2
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/questasim/project.mk.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.257170 SimplHDL-0.0.3/src/simplhdl/resources/templates/rivierapro/
--rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/rivierapro/Makefile.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/rivierapro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/rivierapro/cocotb.mk.j2
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/rivierapro/dependencies.mk.j2
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/rivierapro/files.j2
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/rivierapro/fileset.j2
--rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/rivierapro/project.mk.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.257170 SimplHDL-0.0.3/src/simplhdl/resources/templates/vcs/
--rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vcs/Makefile.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vcs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vcs/cocotb.mk.j2
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vcs/dependencies.mk.j2
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vcs/files.j2
--rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vcs/fileset.j2
--rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vcs/pli.tab.j2
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vcs/project.mk.j2
--rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vcs/synopsys_sim.setup.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.257170 SimplHDL-0.0.3/src/simplhdl/resources/templates/vivado/
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vivado/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vivado/launch_run.sh.j2
--rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vivado/project.tcl.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vivado/run.tcl.j2
--rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/vivado/steps.tcl.j2
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.261170 SimplHDL-0.0.3/src/simplhdl/resources/templates/xsim/
--rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/xsim/Makefile.j2
--rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/xsim/__init__.py
--rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/xsim/cocotb.mk.j2
--rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/xsim/dependencies.mk.j2
--rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/xsim/files.j2
--rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/xsim/fileset.j2
--rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/resources/templates/xsim/project.mk.j2
--rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/simplhdl.py
--rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/tools.py
--rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/src/simplhdl/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-05 12:19:54.261170 SimplHDL-0.0.3/tests/
--rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/tests/test_dummy.py
--rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-05 12:19:49.000000 SimplHDL-0.0.3/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.225458 SimplHDL-0.0.4/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.193458 SimplHDL-0.0.4/.github/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.201458 SimplHDL-0.0.4/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (127)     1185 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1092 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (127)      704 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/.readthedocs.yaml
+-rw-r--r--   0 runner    (1001) docker     (127)     1065 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-11 13:40:01.225458 SimplHDL-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     2664 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.201458 SimplHDL-0.0.4/docs/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.201458 SimplHDL-0.0.4/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (127)    50717 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/_static/simplhdl_dark.png
+-rw-r--r--   0 runner    (1001) docker     (127)   111558 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/_static/simplhdl_light.png
+-rw-r--r--   0 runner    (1001) docker     (127)    38948 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/_static/simplhdl_light_1.png
+-rw-r--r--   0 runner    (1001) docker     (127)     2099 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (127)    20233 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/drawing.svg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.205458 SimplHDL-0.0.4/docs/flows/
+-rw-r--r--   0 runner    (1001) docker     (127)       10 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/flows/ghdl.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       14 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/flows/icarus.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       48 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/flows/quartus.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/flows/questasim.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       26 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/flows/vcs.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1168 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/flows/vivado.rst
+-rw-r--r--   0 runner    (1001) docker     (127)       24 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/flows/xsim.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      187 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/flows.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      541 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      976 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/intel-ips.md
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/introduction.rst
+-rw-r--r--   0 runner    (1001) docker     (127)     1493 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/plugins.rst
+-rw-r--r--   0 runner    (1001) docker     (127)      681 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/docs/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.197458 SimplHDL-0.0.4/examples/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.197458 SimplHDL-0.0.4/examples/hdl/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.205458 SimplHDL-0.0.4/examples/hdl/adder/
+-rw-r--r--   0 runner    (1001) docker     (127)       39 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/adder/adder.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.205458 SimplHDL-0.0.4/examples/hdl/adder/hdl/
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/adder/hdl/adder.sv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.205458 SimplHDL-0.0.4/examples/hdl/adder/sim/
+-rw-r--r--   0 runner    (1001) docker     (127)      134 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/adder/sim/testbench.sv
+-rw-r--r--   0 runner    (1001) docker     (127)      102 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/adder/sim/testbench.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.205458 SimplHDL-0.0.4/examples/hdl/adder/syn/
+-rw-r--r--   0 runner    (1001) docker     (127)      200 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/adder/syn/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)      968 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/adder/syn/placement.xdc
+-rw-r--r--   0 runner    (1001) docker     (127)       58 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/adder/syn/timing.xdc
+-rw-r--r--   0 runner    (1001) docker     (127)      425 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/adder/syn/top.sv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.205458 SimplHDL-0.0.4/examples/hdl/alu/
+-rw-r--r--   0 runner    (1001) docker     (127)       82 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/alu.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.205458 SimplHDL-0.0.4/examples/hdl/alu/hdl/
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/hdl/add.sv
+-rw-r--r--   0 runner    (1001) docker     (127)     2449 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/hdl/alu.sv
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/hdl/mul.sv
+-rw-r--r--   0 runner    (1001) docker     (127)      191 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/hdl/sub.sv
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.197458 SimplHDL-0.0.4/examples/hdl/alu/sim/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.205458 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.205458 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/alu_vip/
+-rw-r--r--   0 runner    (1001) docker     (127)      155 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/alu_vip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      840 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/alu_vip/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      268 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/alu_vip/aluif.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1249 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/alu_vip/driver.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1058 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/alu_vip/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (127)      982 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/alu_vip/sequenceitem.py
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/alu_vip/sequencer.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.209458 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/clock_vip/
+-rw-r--r--   0 runner    (1001) docker     (127)       59 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/clock_vip/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      737 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/clock_vip/agent.py
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/clock_vip/clockif.py
+-rw-r--r--   0 runner    (1001) docker     (127)       93 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/pyuvm.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.209458 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/test/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      359 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/test/env.py
+-rw-r--r--   0 runner    (1001) docker     (127)      829 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/test/seq_lib.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1328 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/test/test.py
+-rw-r--r--   0 runner    (1001) docker     (127)      169 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/testbench.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.197458 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.209458 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/alu_vip/
+-rw-r--r--   0 runner    (1001) docker     (127)     1440 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/alu_vip/agent.svh
+-rw-r--r--   0 runner    (1001) docker     (127)      446 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/alu_vip/alu_vip.sv
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/alu_vip/alu_vip.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1640 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/alu_vip/driver.svh
+-rw-r--r--   0 runner    (1001) docker     (127)       43 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/alu_vip/env.svh
+-rw-r--r--   0 runner    (1001) docker     (127)     4458 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/alu_vip/monitor.svh
+-rw-r--r--   0 runner    (1001) docker     (127)      812 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/alu_vip/sequence_item.svh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.209458 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/tb_env/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.209458 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/tb_env/seq_lib/
+-rw-r--r--   0 runner    (1001) docker     (127)      477 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/tb_env/seq_lib/add_seq.svh
+-rw-r--r--   0 runner    (1001) docker     (127)     1044 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/tb_env/seq_lib/base_seq.svh
+-rw-r--r--   0 runner    (1001) docker     (127)      256 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/tb_env/tb_env.sv
+-rw-r--r--   0 runner    (1001) docker     (127)      212 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/tb_env/tb_env.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.209458 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/tb_env/test/
+-rw-r--r--   0 runner    (1001) docker     (127)      691 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/tb_env/test/base_test.svh
+-rw-r--r--   0 runner    (1001) docker     (127)      854 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/tb_env/test/test_add.svh
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.209458 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/testbench/
+-rw-r--r--   0 runner    (1001) docker     (127)     2257 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/testbench/alu_if.sv
+-rw-r--r--   0 runner    (1001) docker     (127)      964 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/testbench/testbench.sv
+-rw-r--r--   0 runner    (1001) docker     (127)      115 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/testbench/testbench.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.197458 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/testcases/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.209458 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/testcases/test_add/
+-rw-r--r--   0 runner    (1001) docker     (127)      124 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/testcases/test_add/test_add.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.213458 SimplHDL-0.0.4/examples/hdl/alu/syn/
+-rw-r--r--   0 runner    (1001) docker     (127)      132 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/syn/build.yml
+-rw-r--r--   0 runner    (1001) docker     (127)     1689 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/syn/placement.xdc
+-rw-r--r--   0 runner    (1001) docker     (127)      192 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/alu/syn/timing.xdc
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.213458 SimplHDL-0.0.4/examples/hdl/hello/
+-rw-r--r--   0 runner    (1001) docker     (127)      333 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/hello/build.sbt
+-rw-r--r--   0 runner    (1001) docker     (127)       36 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/hello/hello.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.197458 SimplHDL-0.0.4/examples/hdl/hello/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.197458 SimplHDL-0.0.4/examples/hdl/hello/src/main/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.213458 SimplHDL-0.0.4/examples/hdl/hello/src/main/scala/
+-rw-r--r--   0 runner    (1001) docker     (127)      588 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/hello/src/main/scala/Hello.scala
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.213458 SimplHDL-0.0.4/examples/hdl/hello/syn/
+-rw-r--r--   0 runner    (1001) docker     (127)       97 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/hdl/hello/syn/build.yml
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.197458 SimplHDL-0.0.4/examples/plugins/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.213458 SimplHDL-0.0.4/examples/plugins/simple_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)      418 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/plugins/simple_parser/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.197458 SimplHDL-0.0.4/examples/plugins/simple_parser/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.213458 SimplHDL-0.0.4/examples/plugins/simple_parser/src/simple_parser/
+-rw-r--r--   0 runner    (1001) docker     (127)       80 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/plugins/simple_parser/src/simple_parser/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1552 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/examples/plugins/simple_parser/src/simple_parser/simple_parser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1496 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (127)       38 2024-04-11 13:40:01.225458 SimplHDL-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.197458 SimplHDL-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.225458 SimplHDL-0.0.4/src/SimplHDL.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (127)     5226 2024-04-11 13:40:01.000000 SimplHDL-0.0.4/src/SimplHDL.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (127)     6470 2024-04-11 13:40:01.000000 SimplHDL-0.0.4/src/SimplHDL.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        1 2024-04-11 13:40:01.000000 SimplHDL-0.0.4/src/SimplHDL.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (127)       49 2024-04-11 13:40:01.000000 SimplHDL-0.0.4/src/SimplHDL.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (127)      140 2024-04-11 13:40:01.000000 SimplHDL-0.0.4/src/SimplHDL.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (127)        9 2024-04-11 13:40:01.000000 SimplHDL-0.0.4/src/SimplHDL.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.217458 SimplHDL-0.0.4/src/simplhdl/
+-rw-r--r--   0 runner    (1001) docker     (127)       22 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2044 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1610 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/cocotb.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1986 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.217458 SimplHDL-0.0.4/src/simplhdl/flows/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      495 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/implementationflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)      909 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/modelsimflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4748 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/quartusflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.217458 SimplHDL-0.0.4/src/simplhdl/flows/questasim/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/questasim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8485 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/questasim/questasimflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.217458 SimplHDL-0.0.4/src/simplhdl/flows/rivierapro/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/rivierapro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8975 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/rivierapro/rivieraproflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7447 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/simulationflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.217458 SimplHDL-0.0.4/src/simplhdl/flows/vcs/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/vcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7216 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/vcs/vcsflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5422 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/vivadoflow.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.217458 SimplHDL-0.0.4/src/simplhdl/flows/xsim/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/xsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     7319 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/flows/xsim/xsimflow.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1727 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.217458 SimplHDL-0.0.4/src/simplhdl/generators/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/generators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2172 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/generators/chisel.py
+-rw-r--r--   0 runner    (1001) docker     (127)     8484 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/generators/ipxact.py
+-rw-r--r--   0 runner    (1001) docker     (127)     6493 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/generators/spd.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1141 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/generators/systemrdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4117 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/info.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1485 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/parser.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.217458 SimplHDL-0.0.4/src/simplhdl/parsers/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/parsers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      996 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/parsers/fusesocparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     4993 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/parsers/simplhdlparser.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1599 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.221458 SimplHDL-0.0.4/src/simplhdl/pyedaa/
+-rw-r--r--   0 runner    (1001) docker     (127)     3851 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/pyedaa/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      131 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/pyedaa/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2071 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/pyedaa/design.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1989 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/pyedaa/fileset.py
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/pyedaa/filetypes.py
+-rw-r--r--   0 runner    (1001) docker     (127)     5281 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/pyedaa/project.py
+-rw-r--r--   0 runner    (1001) docker     (127)      707 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/pyedaa/vhdllibrary.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1912 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/repo.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.221458 SimplHDL-0.0.4/src/simplhdl/resources/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.221458 SimplHDL-0.0.4/src/simplhdl/resources/templates/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.221458 SimplHDL-0.0.4/src/simplhdl/resources/templates/quartus/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/quartus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)     2160 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/quartus/project.tcl.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1235 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/quartus/run.tcl.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.221458 SimplHDL-0.0.4/src/simplhdl/resources/templates/questasim/
+-rw-r--r--   0 runner    (1001) docker     (127)     1118 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/questasim/Makefile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/questasim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      717 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/questasim/cocotb.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/questasim/dependencies.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/questasim/files.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/questasim/fileset.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/questasim/project.mk.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.221458 SimplHDL-0.0.4/src/simplhdl/resources/templates/rivierapro/
+-rw-r--r--   0 runner    (1001) docker     (127)     1142 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/rivierapro/Makefile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/rivierapro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      741 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/rivierapro/cocotb.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/rivierapro/dependencies.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/rivierapro/files.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/rivierapro/fileset.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      576 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/rivierapro/project.mk.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.225458 SimplHDL-0.0.4/src/simplhdl/resources/templates/vcs/
+-rw-r--r--   0 runner    (1001) docker     (127)     1217 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vcs/Makefile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vcs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      407 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vcs/cocotb.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vcs/dependencies.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vcs/files.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      122 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vcs/fileset.j2
+-rw-r--r--   0 runner    (1001) docker     (127)       13 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vcs/pli.tab.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vcs/project.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      189 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vcs/synopsys_sim.setup.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.225458 SimplHDL-0.0.4/src/simplhdl/resources/templates/vivado/
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vivado/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      149 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vivado/launch_run.sh.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     5140 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vivado/project.tcl.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1292 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vivado/run.tcl.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      397 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/vivado/steps.tcl.j2
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.225458 SimplHDL-0.0.4/src/simplhdl/resources/templates/xsim/
+-rw-r--r--   0 runner    (1001) docker     (127)      947 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/xsim/Makefile.j2
+-rw-r--r--   0 runner    (1001) docker     (127)        0 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/xsim/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (127)      447 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/xsim/cocotb.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      178 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/xsim/dependencies.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      100 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/xsim/files.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      117 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/xsim/fileset.j2
+-rw-r--r--   0 runner    (1001) docker     (127)      205 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/resources/templates/xsim/project.mk.j2
+-rw-r--r--   0 runner    (1001) docker     (127)     1661 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/simplhdl.py
+-rw-r--r--   0 runner    (1001) docker     (127)      322 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/tools.py
+-rw-r--r--   0 runner    (1001) docker     (127)     3553 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/src/simplhdl/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (127)        0 2024-04-11 13:40:01.225458 SimplHDL-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (127)       28 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/tests/test_dummy.py
+-rw-r--r--   0 runner    (1001) docker     (127)     1182 2024-04-11 13:39:56.000000 SimplHDL-0.0.4/tox.ini
```

### Comparing `SimplHDL-0.0.3/.github/workflows/publish.yml` & `SimplHDL-0.0.4/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/.gitignore` & `SimplHDL-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/.readthedocs.yaml` & `SimplHDL-0.0.4/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/LICENSE` & `SimplHDL-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/PKG-INFO` & `SimplHDL-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimplHDL
-Version: 0.0.3
+Version: 0.0.4
 Summary: A framework for simulating and implementing HDL designs
 Author-email: Rasmus Grøndahl Olsen <simplhdl@gmail.com>
 Maintainer-email: Rasmus Grøndahl Olsen <simplhdl@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 SimplHDL
```

### Comparing `SimplHDL-0.0.3/README.md` & `SimplHDL-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/docs/_static/simplhdl_dark.png` & `SimplHDL-0.0.4/docs/_static/simplhdl_dark.png`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/docs/_static/simplhdl_light.png` & `SimplHDL-0.0.4/docs/_static/simplhdl_light.png`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/docs/_static/simplhdl_light_1.png` & `SimplHDL-0.0.4/docs/_static/simplhdl_light_1.png`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/docs/conf.py` & `SimplHDL-0.0.4/docs/conf.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/docs/drawing.svg` & `SimplHDL-0.0.4/docs/drawing.svg`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/docs/flows/vivado.rst` & `SimplHDL-0.0.4/docs/flows/vivado.rst`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/docs/index.rst` & `SimplHDL-0.0.4/docs/index.rst`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/docs/intel-ips.md` & `SimplHDL-0.0.4/docs/intel-ips.md`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/docs/plugins.rst` & `SimplHDL-0.0.4/docs/plugins.rst`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/docs/requirements.txt` & `SimplHDL-0.0.4/docs/requirements.txt`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/examples/hdl/adder/syn/placement.xdc` & `SimplHDL-0.0.4/examples/hdl/adder/syn/placement.xdc`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/examples/hdl/alu/hdl/alu.sv` & `SimplHDL-0.0.4/examples/hdl/alu/hdl/alu.sv`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/alu_vip/agent.py` & `SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/alu_vip/agent.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/alu_vip/driver.py` & `SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/alu_vip/driver.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/alu_vip/monitor.py` & `SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/alu_vip/monitor.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/alu_vip/sequenceitem.py` & `SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/alu_vip/sequenceitem.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/clock_vip/agent.py` & `SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/clock_vip/agent.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/test/seq_lib.py` & `SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/test/seq_lib.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/examples/hdl/alu/sim/pyuvm/test/test.py` & `SimplHDL-0.0.4/examples/hdl/alu/sim/pyuvm/test/test.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/alu_vip/agent.svh` & `SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/alu_vip/agent.svh`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/alu_vip/driver.svh` & `SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/alu_vip/driver.svh`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/alu_vip/monitor.svh` & `SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/alu_vip/monitor.svh`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/alu_vip/sequence_item.svh` & `SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/alu_vip/sequence_item.svh`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/tb_env/seq_lib/base_seq.svh` & `SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/tb_env/seq_lib/base_seq.svh`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/tb_env/test/base_test.svh` & `SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/tb_env/test/base_test.svh`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/tb_env/test/test_add.svh` & `SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/tb_env/test/test_add.svh`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/testbench/alu_if.sv` & `SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/testbench/alu_if.sv`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/examples/hdl/alu/sim/uvm/testbench/testbench.sv` & `SimplHDL-0.0.4/examples/hdl/alu/sim/uvm/testbench/testbench.sv`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/examples/hdl/alu/syn/placement.xdc` & `SimplHDL-0.0.4/examples/hdl/alu/syn/placement.xdc`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/examples/hdl/hello/src/main/scala/Hello.scala` & `SimplHDL-0.0.4/examples/hdl/hello/src/main/scala/Hello.scala`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/examples/plugins/simple_parser/src/simple_parser/simple_parser.py` & `SimplHDL-0.0.4/examples/plugins/simple_parser/src/simple_parser/simple_parser.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/pyproject.toml` & `SimplHDL-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/SimplHDL.egg-info/PKG-INFO` & `SimplHDL-0.0.4/src/SimplHDL.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: SimplHDL
-Version: 0.0.3
+Version: 0.0.4
 Summary: A framework for simulating and implementing HDL designs
 Author-email: Rasmus Grøndahl Olsen <simplhdl@gmail.com>
 Maintainer-email: Rasmus Grøndahl Olsen <simplhdl@gmail.com>
 License: MIT License
         
         Copyright (c) 2024 SimplHDL
```

### Comparing `SimplHDL-0.0.3/src/SimplHDL.egg-info/SOURCES.txt` & `SimplHDL-0.0.4/src/SimplHDL.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/__main__.py` & `SimplHDL-0.0.4/src/simplhdl/__main__.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/cocotb.py` & `SimplHDL-0.0.4/src/simplhdl/cocotb.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/flow.py` & `SimplHDL-0.0.4/src/simplhdl/flow.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/flows/modelsimflow.py` & `SimplHDL-0.0.4/src/simplhdl/flows/modelsimflow.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/flows/quartusflow.py` & `SimplHDL-0.0.4/src/simplhdl/flows/quartusflow.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,15 +12,16 @@
 
 from ..flow import FlowFactory, FlowTools
 from .implementationflow import ImplementationFlow
 from ..resources.templates import quartus as templates
 from ..utils import sh, generate_from_template
 from ..pyedaa import (QuartusIPSpecificationFile, VerilogIncludeFile, VerilogSourceFile,
                       SystemVerilogSourceFile, VHDLSourceFile, ConstraintFile,
-                      EDIFNetlistFile, NetlistFile, SettingFile, QuartusSignalTapFile)
+                      EDIFNetlistFile, NetlistFile, SettingFile, QuartusSignalTapFile,
+                      QuartusIniFile, QuartusQIPSpecificationFile, QuartusQSYSSpecificationFile)
 from ..pyedaa.project import Project
 from ..pyedaa.attributes import UsedIn
 
 logger = logging.getLogger(__name__)
 
 
 @FlowFactory.register('quartus')
@@ -90,14 +91,17 @@
             VHDLSourceFile=VHDLSourceFile,
             ConstraintFile=ConstraintFile,
             QuartusIPSpecificationFile=QuartusIPSpecificationFile,
             EDIFNetlistFile=EDIFNetlistFile,
             NetlistFile=NetlistFile,
             SettingFile=SettingFile,
             QuartusSignalTapFile=QuartusSignalTapFile,
+            QuartusQIPSpecificationFile=QuartusQIPSpecificationFile,
+            QuartusQSYSSpecificationFile=QuartusQSYSSpecificationFile,
+            QuartusIniFile=QuartusIniFile,
             project=self.project,
             UsedIn=UsedIn)
         template = environment.get_template('run.tcl.j2')
         generate_from_template(template, self.builddir,
                                project=self.project)
         command = "quartus_sh -t project.tcl".split()
         self.is_tool_setup()
```

### Comparing `SimplHDL-0.0.3/src/simplhdl/flows/questasim/questasimflow.py` & `SimplHDL-0.0.4/src/simplhdl/flows/questasim/questasimflow.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/flows/rivierapro/rivieraproflow.py` & `SimplHDL-0.0.4/src/simplhdl/flows/rivierapro/rivieraproflow.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/flows/simulationflow.py` & `SimplHDL-0.0.4/src/simplhdl/flows/simulationflow.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/flows/vcs/vcsflow.py` & `SimplHDL-0.0.4/src/simplhdl/flows/vcs/vcsflow.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/flows/vivadoflow.py` & `SimplHDL-0.0.4/src/simplhdl/flows/vivadoflow.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/flows/xsim/xsimflow.py` & `SimplHDL-0.0.4/src/simplhdl/flows/xsim/xsimflow.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/generator.py` & `SimplHDL-0.0.4/src/simplhdl/generator.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/generators/chisel.py` & `SimplHDL-0.0.4/src/simplhdl/generators/chisel.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/generators/ipxact.py` & `SimplHDL-0.0.4/src/simplhdl/generators/ipxact.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/generators/spd.py` & `SimplHDL-0.0.4/src/simplhdl/generators/spd.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 from pathlib import Path
 from xml.etree.ElementTree import Element, parse
 from zipfile import ZipFile
 from shutil import copy, copytree
 
 from ..pyedaa import (
     File, SystemVerilogSourceFile, VHDLSourceFile, VerilogSourceFile,
-    QuartusIPSpecificationFile, HDLLibrary, ConstraintFile, HDLSourceFile
+    QuartusIPSpecificationFile, HDLLibrary, ConstraintFile, HDLSourceFile,
+    QuartusIPCompressedSpecificationFile, QuartusQSYSSpecificationFile
 )
 from ..pyedaa.fileset import FileSet
 from ..flow import FlowBase, FlowCategory, FlowTools
 from ..generator import GeneratorFactory, GeneratorBase, GeneratorError
 from ..utils import md5write, md5check
 
 logger = logging.getLogger(__name__)
@@ -107,47 +108,53 @@
             filesets.append(fileset)
         return filesets
 
 
 @GeneratorFactory.register('QuartusIP')
 class QuartusIP(GeneratorBase):
 
-    def unpack_ip(self, filename: QuartusIPSpecificationFile) -> QuartusIPSpecificationFile:
+    def unpack_ip(self, filename: QuartusIPSpecificationFile) -> QuartusIPSpecificationFile:  # noqa: C901
         ipdir = self.builddir.joinpath('ips')
         dest = ipdir.joinpath(filename.Path.name).with_suffix('')
         md5file = dest.with_suffix('.md5')
         ipdir.mkdir(exist_ok=True)
-        if filename.Path.suffix == '.qsys':
-            return
-        elif filename.Path.suffix == '.zip':
+        if filename.FileType == QuartusQSYSSpecificationFile:
+            pass
+
+        elif filename.FileType == QuartusIPCompressedSpecificationFile:
             update = True
             if md5file.exists():
                 update = not md5check(filename.Path, filename=md5file)
             if update:
                 with ZipFile(filename.Path, 'r') as zip:
                     zip.extractall(ipdir)
                 md5write(filename.Path, filename=md5file)
                 logger.debug(f"Copy {filename.Path} to {dest}")
-        elif filename.Path.suffix == '.ip':
+
+            if filename.Path.suffix == '.zip':
+                filename._path = dest.absolute()
+            else:
+                filename._path = dest.with_suffix('.ip').absolute()
+            filename._fileType = QuartusIPSpecificationFile
+
+        elif filename.FileType == QuartusIPSpecificationFile:
             update = True
             dir = filename.Path.with_suffix('')
             if dir.exists():
                 if md5file.exists():
                     update = not md5check(filename.Path, dir, filename=md5file)
             if update:
                 copy(str(filename.Path), str(dest.with_suffix('.ip')))
                 md5write(filename.Path, filename=md5file)
                 if dir.exists():
                     copytree(str(dir), str(dest.with_suffix('')), dirs_exist_ok=True)
                     md5write(filename.Path, dir, filename=md5file)
                     logger.debug(f"Copy {filename.Path} to {dest}")
-        else:
-            # Non Qartus IP files
-            return filename
-        filename._path = dest.absolute()
+            filename._path = dest.with_suffix('.ip').absolute()
+
         return filename
 
     def run(self, flow: FlowBase):
         os.makedirs(self.builddir, exist_ok=True)
         for ipfile in self.project.DefaultDesign.DefaultFileSet.Files(fileType=QuartusIPSpecificationFile):
             newipfile = self.unpack_ip(ipfile)
             if flow.category == FlowCategory.SIMULATION:
```

### Comparing `SimplHDL-0.0.3/src/simplhdl/generators/systemrdl.py` & `SimplHDL-0.0.4/src/simplhdl/generators/systemrdl.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/info.py` & `SimplHDL-0.0.4/src/simplhdl/info.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/parser.py` & `SimplHDL-0.0.4/src/simplhdl/parser.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/parsers/fusesocparser.py` & `SimplHDL-0.0.4/src/simplhdl/parsers/fusesocparser.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/parsers/simplhdlparser.py` & `SimplHDL-0.0.4/src/simplhdl/parsers/simplhdlparser.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/plugins.py` & `SimplHDL-0.0.4/src/simplhdl/plugins.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/pyedaa/__init__.py` & `SimplHDL-0.0.4/src/simplhdl/pyedaa/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -124,14 +124,33 @@
         self[UsedIn] = {'implmentation'}
 
 
 class QuartusIPSpecificationFile(IPSpecificationFile):
     pass
 
 
+class QuartusIPCompressedSpecificationFile(QuartusIPSpecificationFile):
+    pass
+
+
+class QuartusQSYSSpecificationFile(QuartusIPSpecificationFile):
+    pass
+
+
+class QuartusQIPSpecificationFile(QuartusIPSpecificationFile):
+    pass
+
+
+class QuartusIniFile(File):
+    def _registerAttributes(self):
+        super()._registerAttributes()
+        FileMixIn._registerAttributes(self)
+        self[UsedIn] = {'implementation'}
+
+
 class VivadoIPSpecificationFile(IPSpecificationFile):
     pass
 
 
 class SystemRDLSourceFile(File):
     pass
```

### Comparing `SimplHDL-0.0.3/src/simplhdl/pyedaa/design.py` & `SimplHDL-0.0.4/src/simplhdl/pyedaa/design.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/pyedaa/fileset.py` & `SimplHDL-0.0.4/src/simplhdl/pyedaa/fileset.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/pyedaa/project.py` & `SimplHDL-0.0.4/src/simplhdl/pyedaa/project.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/pyedaa/vhdllibrary.py` & `SimplHDL-0.0.4/src/simplhdl/pyedaa/vhdllibrary.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/repo.py` & `SimplHDL-0.0.4/src/simplhdl/repo.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/resources/templates/quartus/project.tcl.j2` & `SimplHDL-0.0.4/src/simplhdl/resources/templates/quartus/project.tcl.j2`

 * *Files 18% similar despite different names*

```diff
@@ -10,41 +10,34 @@
 {% endfor %}
 {% for define, value in project.Defines.items() %}
 set_global_assignment -name VERILOG_MACRO "{{define}}={{value}}"
 {% endfor %}
 {% for file in project.DefaultDesign.Files() if 'implementation' in file[UsedIn] %}
 {% if file.FileType == VerilogIncludeFile %}
 set_global_assignment -name VERILOG_INCLUDE_FILE "{{file.Path}}"
-{% endif %}
-{% if file.FileType == SystemVerilogSourceFile %}
+{% elif file.FileType == SystemVerilogSourceFile %}
 set_global_assignment -name SYSTEMVERILOG_FILE "{{file.Path}}"
-{% endif %}
-{% if file.FileType == VerilogSourceFile %}
+{% elif file.FileType == VerilogSourceFile %}
 set_global_assignment -name VERILOG_FILE "{{file.Path}}"
-{% endif %}
-{% if file.FileType == VHDLSourceFile %}
+{% elif file.FileType == VHDLSourceFile %}
 set_global_assignment -name VHDL_FILE "{{file.Path}}"
-{% endif %}
-{% if file.FileType == ConstraintFile %}
+{% elif file.FileType == ConstraintFile %}
 set_global_assignment -name SDC_FILE "{{file.Path}}"
-{% endif %}
-{% if file.FileType == TCLSourceFile %}
+{% elif file.FileType == TCLSourceFile %}
 set_global_assignment -name TCL_FILE "{{file.Path}}"
-{% endif %}
-{% if file.FileType == QuartusIPSpecificationFile and file.Path.suffix == '.ip' %}
+{% elif file.FileType == QuartusIPSpecificationFile %}
 set_global_assignment -name IP_FILE "{{file.Path}}"
-{% endif %}
-{% if file.FileType == QuartusIPSpecificationFile and file.Path.suffix == '.qip' %}
+{% elif file.FileType == QuartusQIPSpecificationFile %}
 set_global_assignment -name QIP_FILE "{{file.Path}}"
-{% endif %}
-{% if file.FileType == QuartusIPSpecificationFile and file.Path.suffix == '.qsys' %}
+{% elif file.FileType == QuartusQSYSSpecificationFile %}
 set_global_assignment -name QSYS_FILE "{{file.Path}}"
-{% endif %}
-{% if file.FileType == SettingFile and file.Path.suffix == '.qsf' %}
+{% elif file.FileType == SettingFile and file.Path.suffix == '.qsf' %}
 source "{{file.Path}}"
+{% elif file.FileType == QuartusIniFile %}
+file copy -force "{{file.Path}}" "quartus.ini"
 {% endif %}
 {% endfor %}
 
 {% for file in project.DefaultDesign.Files(QuartusSignalTapFile) %}
 set_global_assignment -name SIGNALTAP_FILE "{{file.Path}}"
 {% if loop.last %}
 set_global_assignment -name ENABLE_SIGNALTAP ON
```

### Comparing `SimplHDL-0.0.3/src/simplhdl/resources/templates/quartus/run.tcl.j2` & `SimplHDL-0.0.4/src/simplhdl/resources/templates/quartus/run.tcl.j2`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/resources/templates/questasim/Makefile.j2` & `SimplHDL-0.0.4/src/simplhdl/resources/templates/questasim/Makefile.j2`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/resources/templates/questasim/cocotb.mk.j2` & `SimplHDL-0.0.4/src/simplhdl/resources/templates/questasim/cocotb.mk.j2`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/resources/templates/questasim/project.mk.j2` & `SimplHDL-0.0.4/src/simplhdl/resources/templates/questasim/project.mk.j2`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/resources/templates/rivierapro/Makefile.j2` & `SimplHDL-0.0.4/src/simplhdl/resources/templates/rivierapro/Makefile.j2`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/resources/templates/rivierapro/cocotb.mk.j2` & `SimplHDL-0.0.4/src/simplhdl/resources/templates/rivierapro/cocotb.mk.j2`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/resources/templates/rivierapro/project.mk.j2` & `SimplHDL-0.0.4/src/simplhdl/resources/templates/rivierapro/project.mk.j2`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/resources/templates/vcs/Makefile.j2` & `SimplHDL-0.0.4/src/simplhdl/resources/templates/vcs/Makefile.j2`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/resources/templates/vivado/project.tcl.j2` & `SimplHDL-0.0.4/src/simplhdl/resources/templates/vivado/project.tcl.j2`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/resources/templates/vivado/run.tcl.j2` & `SimplHDL-0.0.4/src/simplhdl/resources/templates/vivado/run.tcl.j2`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/resources/templates/xsim/Makefile.j2` & `SimplHDL-0.0.4/src/simplhdl/resources/templates/xsim/Makefile.j2`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/simplhdl.py` & `SimplHDL-0.0.4/src/simplhdl/simplhdl.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/src/simplhdl/utils.py` & `SimplHDL-0.0.4/src/simplhdl/utils.py`

 * *Files identical despite different names*

### Comparing `SimplHDL-0.0.3/tox.ini` & `SimplHDL-0.0.4/tox.ini`

 * *Files identical despite different names*

