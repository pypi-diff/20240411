# Comparing `tmp/cpop-32.0.3.tar.gz` & `tmp/cpop-32.0.4.tar.gz`

## Comparing `cpop-32.0.3.tar` & `cpop-32.0.4.tar`

### file list

```diff
@@ -1,174 +1,153 @@
--rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 cpop-32.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     8448 2020-02-02 00:00:00.000000 cpop-32.0.3/src/cpop/contract.pyx
--rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 cpop-32.0.3/src/cpop/data.pyx
--rw-r--r--   0        0        0     1929 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/config.yaml
--rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/dirs.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/exc.py
--rw-r--r--   0        0        0    24876 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/hub.py
--rw-r--r--   0        0        0    11428 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/loader.py
--rw-r--r--   0        0        0      493 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/ref.py
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/scanner.py
--rw-r--r--   0        0        0     7642 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/verify.py
--rw-r--r--   0        0        0     5221 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/log/async.py
--rw-r--r--   0        0        0     9482 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/mods/config.py
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/mods/contract.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/mods/dyne.py
--rw-r--r--   0        0        0     6941 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/mods/sub.py
--rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/mods/task.py
--rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cpop-32.0.3/src/pop/mods/test.py
--rw-r--r--   0        0        0      578 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/conftest.py
--rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/alias/init.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/cmods/ctest.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/cmods/contracts/ctest.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/contracts/ctx.py
--rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/contracts/ctx_args.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/contracts/ctx_update.py
--rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/contracts/many.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/contracts/priv.py
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/contracts/test.py
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/contracts/testing.py
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/coro/test.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/coro/contracts/test.py
--rw-r--r--   0        0        0      353 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/csigs/sigs.py
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/csigs/contracts/sigs.py
--rw-r--r--   0        0        0      265 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/external_module/api.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/__init__.py
--rw-r--r--   0        0        0     7459 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/test_basic.py
--rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/test_bench.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/test_cli.py
--rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/test_contract_ctx.py
--rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/test_coro.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/test_cpop.py
--rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/test_fail.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/test_hub.py
--rw-r--r--   0        0        0     1221 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/test_no_raise_on_pre_failure.py
--rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/test_raise_on_pre_failure.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/test_serial.py
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/func/test_sub.py
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/contract_ordering/single_module/thing.py
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/contract_ordering/single_module/contracts/default.py
--rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/contract_ordering/single_module/contracts/dunder.py
--rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/contract_ordering/single_module/contracts/init.py
--rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/contract_ordering/single_module/contracts/thing.py
--rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/contract_ordering/single_module/recursive_contracts/default.py
--rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py
--rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/contract_ordering/single_module/recursive_contracts/init.py
--rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/contracted/test_contracted_access.py
--rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/contracted/mods/contracted_access.py
--rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/contracted/mods/contracts/contracted_access.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/recursive_contract/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/recursive_contract/test_sub.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/recursive_contract/rc_sub1/rc_sub2/thing.py
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/fnord.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/contracts/init.py
--rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py
--rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/bad.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/falias_dict.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/falias_func.py
--rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/foo.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/fork.py
--rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/many.py
--rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/priv.py
--rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/proc.py
--rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/test.py
--rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/testing.py
--rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/vbad.py
--rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/virt.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/vtrue.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/bad_import/bad_import.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/contract_ctx/ctx.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/contract_ctx/ctx_args.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/contract_ctx/ctx_update.py
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/contract_sig/fail_sigs.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/contract_sig/pass_sigs.py
--rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/contract_sig/contracts/init.py
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/coro/coro.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/iter/bar.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/iter/foo.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/iter/init.py
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/nest/basic.py
--rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/same_vname/will_load.py
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/same_vname/will_not_load.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/subinit/init.py
--rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/mods/subinit/subinit.py
--rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/regression/contract_masking/test_contract_masking.py
--rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/regression/contract_masking/test_duplicate_contracts.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/regression/contract_masking/contract1/init.py
--rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/regression/contract_masking/contract2/init.py
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/regression/contract_masking/sub/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/sdirs/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/sdirs/l11/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/sdirs/l11/l2/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/sdirs/l12/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/sdirs/l12/l2/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/sdirs/l13/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/sdirs/l13/l2/test.py
--rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/README.rst
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/cn/config.yaml
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/cn/contract/test.py
--rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/cn/contract/contracts/test.py
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/config.yaml
--rw-r--r--   0        0        0      577 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/init.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/clash.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/dup1.py
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/dup2.py
--rw-r--r--   0        0        0      222 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/float.py
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/init.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/invalid.py
--rw-r--r--   0        0        0      248 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/neg.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/neg_last.py
--rw-r--r--   0        0        0      241 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/pos.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/pos_first.py
--rw-r--r--   0        0        0      245 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/pos_first_tie.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/unordered_1.py
--rw-r--r--   0        0        0      185 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/unordered_2.py
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/verify_fail.py
--rw-r--r--   0        0        0      213 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/verify_pass.py
--rw-r--r--   0        0        0      225 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/verify_raise.py
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/contracts/zero.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/nest/init.py
--rw-r--r--   0        0        0      233 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/recursive_contracts/clash.py
--rw-r--r--   0        0        0      247 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/recursive_contracts/init.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/recursive_contracts/unordered_3.py
--rw-r--r--   0        0        0      195 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/co1/contract_ordering/recursive_contracts/unordered_4.py
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/config/config.yaml
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dn1/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dn1/dn1/nest/dn1.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dn1/dn1/nest/over.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dn2/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dn2/dn1/nest/dn2.py
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dn2/dn1/nest/over.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dn3/config.yaml
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dn3/dn1/nest/dn3.py
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dn3/dn1/nest/over.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dn3/dn1/nest/next/test.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dn3/dn1/nest/next/last/test.py
--rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne1/config.yaml
--rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne1/dyne1/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne1/dyne1/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne1/nest/dyne/nest.py
--rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne2/config.yaml
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne2/dyne2/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne2/dyne2/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne2/nest/dyne/nest.py
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne3/config.yaml
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne3/dyne3/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne3/dyne3/test.py
--rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne3/nest/dyne/nest.py
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne4/config.yaml
--rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne4/dyne4/nest/init.py
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/dyne4/dyne4/nest/subvert.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/fork/config.yaml
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/fork/fork/rsub.py
--rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/fork/fork/nest/init.py
--rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/v1/config.yaml
--rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/tpath/v1/v1/load.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/unit/__init__.py
--rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/unit/test_contract.py
--rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 cpop-32.0.3/tests/unit/test_sigs.py
--rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-32.0.3/.gitignore
--rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 cpop-32.0.3/README.rst
--rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 cpop-32.0.3/pyproject.toml
--rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 cpop-32.0.3/PKG-INFO
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 cpop-32.0.4/.coveragerc
+-rw-r--r--   0        0        0     3816 2020-02-02 00:00:00.000000 cpop-32.0.4/.pre-commit-config.yaml
+-rw-r--r--   0        0        0     8448 2020-02-02 00:00:00.000000 cpop-32.0.4/src/cpop/contract.pyx
+-rw-r--r--   0        0        0     6101 2020-02-02 00:00:00.000000 cpop-32.0.4/src/cpop/data.pyx
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 cpop-32.0.4/src/pop/config.yaml
+-rw-r--r--   0        0        0     4472 2020-02-02 00:00:00.000000 cpop-32.0.4/src/pop/dirs.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 cpop-32.0.4/src/pop/exc.py
+-rw-r--r--   0        0        0    24999 2020-02-02 00:00:00.000000 cpop-32.0.4/src/pop/hub.py
+-rw-r--r--   0        0        0    11174 2020-02-02 00:00:00.000000 cpop-32.0.4/src/pop/loader.py
+-rw-r--r--   0        0        0     1691 2020-02-02 00:00:00.000000 cpop-32.0.4/src/pop/ref.py
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 cpop-32.0.4/src/pop/scanner.py
+-rw-r--r--   0        0        0     7642 2020-02-02 00:00:00.000000 cpop-32.0.4/src/pop/verify.py
+-rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 cpop-32.0.4/src/pop/log/basic.py
+-rw-r--r--   0        0        0     3786 2020-02-02 00:00:00.000000 cpop-32.0.4/src/pop/log/init.py
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 cpop-32.0.4/src/pop/log/timed_rolling.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-32.0.4/src/pop/log/contracts/init.py
+-rw-r--r--   0        0        0     9560 2020-02-02 00:00:00.000000 cpop-32.0.4/src/pop/mods/config.py
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 cpop-32.0.4/src/pop/mods/contract.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 cpop-32.0.4/src/pop/mods/dyne.py
+-rw-r--r--   0        0        0     6947 2020-02-02 00:00:00.000000 cpop-32.0.4/src/pop/mods/sub.py
+-rw-r--r--   0        0        0     2115 2020-02-02 00:00:00.000000 cpop-32.0.4/src/pop/mods/task.py
+-rw-r--r--   0        0        0      861 2020-02-02 00:00:00.000000 cpop-32.0.4/src/pop/mods/test.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/conftest.py
+-rw-r--r--   0        0        0       80 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/alias/init.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/cmods/ctest.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/cmods/contracts/ctest.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/contracts/ctx.py
+-rw-r--r--   0        0        0      150 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/contracts/ctx_args.py
+-rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/contracts/ctx_update.py
+-rw-r--r--   0        0        0      512 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/contracts/many.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/contracts/priv.py
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/contracts/test.py
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/coro/test.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/coro/contracts/test.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/func/__init__.py
+-rw-r--r--   0        0        0     7665 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/func/test_basic.py
+-rw-r--r--   0        0        0      451 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/func/test_bench.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/func/test_cli.py
+-rw-r--r--   0        0        0     4080 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/func/test_config.py
+-rw-r--r--   0        0        0     1230 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/func/test_contract_ctx.py
+-rw-r--r--   0        0        0      304 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/func/test_coro.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/func/test_cpop.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/func/test_dyne.py
+-rw-r--r--   0        0        0     1156 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/func/test_fail.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/func/test_hub.py
+-rw-r--r--   0        0        0     2202 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/func/test_log.py
+-rw-r--r--   0        0        0     1159 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/func/test_no_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      755 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/func/test_raise_on_pre_failure.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/func/test_ref.py
+-rw-r--r--   0        0        0      667 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/func/test_serial.py
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/func/test_sub.py
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/integration/contract_ordering/single_module/thing.py
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/integration/contract_ordering/single_module/contracts/default.py
+-rw-r--r--   0        0        0      952 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/integration/contract_ordering/single_module/contracts/dunder.py
+-rw-r--r--   0        0        0      889 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/integration/contract_ordering/single_module/contracts/init.py
+-rw-r--r--   0        0        0      905 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/integration/contract_ordering/single_module/contracts/thing.py
+-rw-r--r--   0        0        0     1128 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/integration/contract_ordering/single_module/recursive_contracts/default.py
+-rw-r--r--   0        0        0     1112 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py
+-rw-r--r--   0        0        0     1080 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/integration/contract_ordering/single_module/recursive_contracts/init.py
+-rw-r--r--   0        0        0     1096 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/integration/contracted/test_contracted_access.py
+-rw-r--r--   0        0        0      474 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/integration/contracted/mods/contracted_access.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/integration/contracted/mods/contracts/contracted_access.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/integration/recursive_contract/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/integration/recursive_contract/test_sub.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/integration/recursive_contract/rc_sub1/rc_sub2/thing.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/fnord.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/integration/recursive_contract/rc_sub1/rc_sub2/nested_sub/contracts/init.py
+-rw-r--r--   0        0        0      539 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py
+-rw-r--r--   0        0        0      169 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/bad.py
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/falias_dict.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/falias_func.py
+-rw-r--r--   0        0        0       96 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/foo.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/fork.py
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/many.py
+-rw-r--r--   0        0        0      139 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/priv.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/proc.py
+-rw-r--r--   0        0        0      917 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/test.py
+-rw-r--r--   0        0        0      386 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/testing.py
+-rw-r--r--   0        0        0      250 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/vbad.py
+-rw-r--r--   0        0        0      237 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/virt.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/vtrue.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/bad_import/bad_import.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/contract_ctx/ctx.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/contract_ctx/ctx_args.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/contract_ctx/ctx_update.py
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/contract_sig/fail_sigs.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/contract_sig/pass_sigs.py
+-rw-r--r--   0        0        0      171 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/contract_sig/contracts/init.py
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/coro/coro.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/iter/bar.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/iter/foo.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/iter/init.py
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/nest/basic.py
+-rw-r--r--   0        0        0      118 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/same_vname/will_load.py
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/same_vname/will_not_load.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/subinit/init.py
+-rw-r--r--   0        0        0      159 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/mods/subinit/subinit.py
+-rw-r--r--   0        0        0      801 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/regression/contract_masking/test_contract_masking.py
+-rw-r--r--   0        0        0      711 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/regression/contract_masking/test_duplicate_contracts.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/regression/contract_masking/contract1/init.py
+-rw-r--r--   0        0        0       58 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/regression/contract_masking/contract2/init.py
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/regression/contract_masking/sub/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/sdirs/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/sdirs/l11/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/sdirs/l11/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/sdirs/l12/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/sdirs/l12/l2/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/sdirs/l13/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/sdirs/l13/l2/test.py
+-rw-r--r--   0        0        0      259 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/README.rst
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/cn/config.yaml
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/cn/contract/test.py
+-rw-r--r--   0        0        0      470 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/cn/contract/contracts/test.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dn1/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dn1/dn1/nest/dn1.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dn1/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dn2/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dn2/dn1/nest/dn2.py
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dn2/dn1/nest/over.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dn3/config.yaml
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dn3/dn1/nest/dn3.py
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dn3/dn1/nest/over.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dn3/dn1/nest/next/test.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dn3/dn1/nest/next/last/test.py
+-rw-r--r--   0        0        0       38 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dyne1/config.yaml
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dyne1/dyne1/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dyne1/dyne1/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dyne1/nest/dyne/nest.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dyne2/config.yaml
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dyne2/dyne2/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dyne2/dyne2/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dyne2/nest/dyne/nest.py
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dyne3/config.yaml
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dyne3/dyne3/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dyne3/dyne3/test.py
+-rw-r--r--   0        0        0       47 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dyne3/nest/dyne/nest.py
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dyne4/config.yaml
+-rw-r--r--   0        0        0       85 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dyne4/dyne4/nest/init.py
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/dyne4/dyne4/nest/subvert.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/fork/config.yaml
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/fork/fork/rsub.py
+-rw-r--r--   0        0        0      164 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/fork/fork/nest/init.py
+-rw-r--r--   0        0        0       92 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/v1/config.yaml
+-rw-r--r--   0        0        0      132 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/tpath/v1/v1/load.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/unit/__init__.py
+-rw-r--r--   0        0        0      652 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/unit/test_contract.py
+-rw-r--r--   0        0        0     1382 2020-02-02 00:00:00.000000 cpop-32.0.4/tests/unit/test_sigs.py
+-rw-r--r--   0        0        0     5689 2020-02-02 00:00:00.000000 cpop-32.0.4/.gitignore
+-rw-r--r--   0        0        0     3901 2020-02-02 00:00:00.000000 cpop-32.0.4/README.rst
+-rw-r--r--   0        0        0     1628 2020-02-02 00:00:00.000000 cpop-32.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4898 2020-02-02 00:00:00.000000 cpop-32.0.4/PKG-INFO
```

### Comparing `cpop-32.0.3/.pre-commit-config.yaml` & `cpop-32.0.4/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/src/cpop/contract.pyx` & `cpop-32.0.4/src/cpop/contract.pyx`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/src/cpop/data.pyx` & `cpop-32.0.4/src/cpop/data.pyx`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/src/pop/config.yaml` & `cpop-32.0.4/src/pop/config.yaml`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 config:
   pop:
     config:
       default: ~/.pop/config.yaml
       os: POP_CONFIG
   log:
     log_plugin:
-      default: async
+      default: basic
       os: POP_LOG_PLUGIN
     log_file:
       default: ~/.pop/pop.log
       os: POP_LOG_FILE
     log_level:
       os: POP_LOG_LEVEL
       default: "warning"
@@ -31,15 +31,15 @@
       options:
         - -c
       subcommands:
         - __global__
   log:
     log_plugin:
       help: The log plugin to use
-      choices: log
+      choices: log._loaded
       group: Logging Options
       subcommands:
         - __global__
     log_file:
       help: The location of the log file
       group: Logging Options
       subcommands:
@@ -73,14 +73,15 @@
 import:
   - aiologger.handlers.files
   - argparse
   - asyncio
   - collections
   - importlib
   - importlib.resources
+  - logging
   - os
   - pathlib
   - pop.exc
   - cpop.contract
   - cpop.data
   - pop.hub
   - signal
```

### Comparing `cpop-32.0.3/src/pop/dirs.py` & `cpop-32.0.4/src/pop/dirs.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/src/pop/exc.py` & `cpop-32.0.4/src/pop/exc.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/src/pop/hub.py` & `cpop-32.0.4/src/pop/hub.py`

 * *Files 1% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 
             if load_config:
                 # Overwrite opt with config data
                 self._opt = await self.pop.config.load(cli=cli, **self._dynamic.config)
 
         # Set up a logger
         if "log" in self._subs and logs:
-            await self.log[self._opt.log.log_plugin].setup(self._opt.log.copy())
+            await self.log.init.setup(**self._opt.log.copy())
 
     @property
     def OPT(self):
         return self._opt
 
     async def _load_all(self):
         for base, imp in self._dynamic.imports.items():
@@ -235,14 +235,17 @@
             aliases=self._sub_alias,
             OPT=cpop.data.unfreeze(self._opt),
             imports={subname: mod.__name__ for subname, mod in self._imports.items()},
             attrs=attrs,
         )
         return state
 
+    def __reduce__(self):
+        return Hub, (), self.__getstate__()
+
     def __setstate__(self, state: dict):
         subs = state["subs"]
         opt = state["OPT"]
         aliases = state["aliases"]
 
         for subname, modname in state["imports"].items():
             try:
@@ -489,14 +492,17 @@
             },
             subs={name: sub.__getstate__() for name, sub in self._subs.items()},
             aliases=self._sub_alias,
             imports={subname: mod.__name__ for subname, mod in self._imports.items()},
             attrs=attrs,
         )
 
+    def __reduce__(self):
+        return Sub, (), self.__getstate__()
+
     def __setstate__(self, state: dict):
         """
         Only a hub can truly restore a sub because of their interdependency
         """
         subs = state["subs"]
         aliases = state["aliases"]
         imports = state["imports"]
```

### Comparing `cpop-32.0.3/src/pop/loader.py` & `cpop-32.0.4/src/pop/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -30,26 +30,14 @@
         self.edict = {
             "msg": msg,
             "exception": exception,
             "verror": verror,
         }
         self.traceback = traceback
 
-    def __call__(self):
-        """
-        Return the error cases
-        """
-        return self.edict
-
-    def __getattr__(self, attr):
-        """
-        Return a lambda that returns the edict
-        """
-        return self.__calling_load_error__
-
 
 def load_mod(modname: str, form: str, path: str) -> "LoadedMod":
     """
     Load a single module
     :param modname: The name of the module to get from the loader
     :param form: The name of the loader module
     :param path: The package to use as the anchor point from which to resolve the
```

### Comparing `cpop-32.0.3/src/pop/scanner.py` & `cpop-32.0.4/src/pop/scanner.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/src/pop/verify.py` & `cpop-32.0.4/src/pop/verify.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/src/pop/mods/config.py` & `cpop-32.0.4/src/pop/mods/config.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,7 @@
-import cpop.data
-
-
 async def load(
     hub,
     cli: str = None,
     cli_config: dict[str, object] = None,
     config: dict[str, object] = None,
     subcommands: dict[str, object] = None,
     global_clis: list[str] = None,
@@ -46,15 +43,15 @@
     )
 
     # Get the plain config data that will tell us about OS vars and defaults
     if config is None:
         config = hub._dynamic.config.get("config") or {}
 
     # Load the config file parameter in the proper order
-    pop_config = config.get("pop", {}).get("config")
+    pop_config = config.get("pop", {}).get("config") or {}
     config_file = (
         cli_opts.get("config")
         or hub.lib.os.environ.get("POP_CONFIG", pop_config.get("os"))
         or pop_config.get("default")
     )
     if config_file and hub.lib.os.path.exists(config_file):
         async with hub.lib.aiofiles.open(config_file, "r") as fh:
@@ -66,15 +63,15 @@
         cli=cli,
         cli_opts=cli_opts,
         config=config,
         config_file_data=config_data,
         global_clis=global_clis,
     )
 
-    return cpop.data.freeze(OPT)
+    return hub.lib.cpop.data.freeze(OPT)
 
 
 async def parse_cli(
     hub,
     cli: str,
     active_cli: dict[str, object],
     subcommands: dict[str, object],
@@ -102,17 +99,21 @@
     sparser = None
     subparsers = {}
 
     # Add subcommands to the parser
     for subcommand, opts in subcommands.items():
         if sparser is None:
             sparser = parser.add_subparsers(dest="SUBPARSER")
+        if "description" not in opts:
+            opts["description"] = (
+                f"{cli.title().replace('_', ' ')} {subcommand.title().replace('_', ' ')} CLI Parser"
+            )
+
         subparsers[subcommand] = sparser.add_parser(
             subcommand,
-            description=f"{cli.title().replace('_', ' ')} {subcommand.title().replace('_', ' ')} CLI Parser",
             **opts,
         )
 
     # Add CLI options to the parser
     groups = {}
     subparser_groups = {subcommand: {} for subcommand in subparsers}
 
@@ -161,28 +162,28 @@
                         subparsers[subcommand].add_argument_group(group_name),
                     )
                     if group_name
                     else subparsers[subcommand]
                 )
                 subparser_group.add_argument(cli_name, *options, **opts)
 
-    return cpop.data.NamespaceDict(parser.parse_args(args=parser_args).__dict__)
+    return hub.lib.cpop.data.NamespaceDict(parser.parse_args(args=parser_args).__dict__)
 
 
 PLACEHOLDER = object()
 
 
 async def prioritize(
     hub,
     cli: str,
     cli_opts: dict[str, any],
     config: dict[str, any],
     config_file_data: dict[str, any],
     global_clis: list[str],
-) -> cpop.data.ImmutableNamespaceDict:
+):
     """
     Prioritize configuration data from various sources.
 
     The order of priority is:
     1. CLI options (highest priority)
     2. Configuration file data
     3. OS environment variables
@@ -216,32 +217,32 @@
 
             # Skip malformed config
             if not isinstance(data, dict):
                 raise TypeError(f"Invalid data from config.yaml: {data}")
 
             # 3. Check OS environment variables if config file data is not set
             if value is PLACEHOLDER and "os" in data:
-                value = hub.lib.os.environ.get(arg, PLACEHOLDER)
+                value = hub.lib.os.environ.get(data["os"], PLACEHOLDER)
 
             # 4. Use default value if none of the above are set
             if value is PLACEHOLDER:
                 value = data.get("default")
             if arg == "root_dir":
                 root_dir = value
             # Set the value in the OPT dictionary
             OPT[namespace][arg] = value
     await hub.pop.config.manage_paths(cli, OPT, root_dir)
 
     OPT["pop"]["subparser"] = cli_opts.get("SUBPARSER", "")
     OPT["pop"]["global_clis"] = global_clis
 
-    return cpop.data.freeze(OPT)
+    return hub.lib.cpop.data.freeze(OPT)
 
 
-async def manage_paths(hub, cli, OPT, root_dir):
+async def manage_paths(hub, cli: str, OPT: dict, root_dir: str):
     """
     If a root_dir has been specified, then we support rewriting roots, find all of the options
     for _dir, _path, and _file and update them
     """
     reroot = True if root_dir else False
     if not root_dir:
         root_dir = hub.lib.pathlib.Path(hub.lib.os.sep)
```

### Comparing `cpop-32.0.3/src/pop/mods/contract.py` & `cpop-32.0.4/src/pop/mods/contract.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/src/pop/mods/sub.py` & `cpop-32.0.4/src/pop/mods/sub.py`

 * *Files 1% similar despite different names*

```diff
@@ -170,11 +170,11 @@
     when started.
     :param hub: The redistributed pop central hub
     :param subname: The name that the sub is going to take on the hub
         if nothing else is passed, it is used as the pypath
     """
     if hasattr(hub, subname):
         sub = getattr(hub, subname)
-        sub._prepare()
+        await sub._prepare()
         return True
     else:
         return False
```

### Comparing `cpop-32.0.3/src/pop/mods/task.py` & `cpop-32.0.4/src/pop/mods/task.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/src/pop/mods/test.py` & `cpop-32.0.4/src/pop/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/tests/conftest.py` & `cpop-32.0.4/tests/conftest.py`

 * *Files 26% similar despite different names*

```diff
@@ -4,15 +4,22 @@
 
 import pop.hub
 import pytest
 
 
 @pytest.fixture()
 async def hub():
-    yield await pop.hub.AsyncHub()
+    yield await pop.hub.AsyncHub(
+        # Let each test manually add their structure
+        load_all_dynes=False,
+        load_all_subdirs=False,
+        recurse_subdirs=False,
+        logs=False,
+        load_config=False,
+    )
 
 
 @pytest.fixture(autouse=True, scope="session")
 def tpath():
     code_dir = pathlib.Path(__file__).parent.parent.absolute()
     assert code_dir.exists()
```

### Comparing `cpop-32.0.3/tests/contracts/ctx.py` & `cpop-32.0.4/tests/contracts/ctx.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/tests/contracts/many.py` & `cpop-32.0.4/tests/contracts/many.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/tests/contracts/test.py` & `cpop-32.0.4/tests/contracts/test.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/tests/func/test_basic.py` & `cpop-32.0.4/tests/func/test_basic.py`

 * *Files 2% similar despite different names*

```diff
@@ -213,7 +213,16 @@
     assert "Signature Errors" in errs[0]
 
     filtered_errs = set({e for e in errs[1:-1] if "Enforcing signature" not in e})
     assert filtered_errs == {
         "args: **kwargs are not permitted as a parameter",
         "kwargs: *args are not permitted as a parameter",
     }
+
+
+async def test_reload(hub):
+    await hub.pop.sub.add(dyne_name="dn1")
+    assert await hub.pop.sub.reload("dn1")
+
+
+async def test_reload_fail(hub):
+    assert not await hub.pop.sub.reload("nonexistant")
```

### Comparing `cpop-32.0.3/tests/func/test_contract_ctx.py` & `cpop-32.0.4/tests/func/test_contract_ctx.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/tests/func/test_fail.py` & `cpop-32.0.4/tests/func/test_fail.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/tests/func/test_no_raise_on_pre_failure.py` & `cpop-32.0.4/tests/func/test_no_raise_on_pre_failure.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-import pop.exc
-import pop.hub
 import pytest
 
 
 @pytest.fixture(scope="function")
-async def hub():
-    hub = await pop.hub.AsyncHub()
+async def hub(hub):
     await hub.pop.sub.add(dyne_name="cn")
     yield hub
 
 
 async def test_pre_fail_sync(hub):
     with pytest.raises(
         Exception, match="Pre contract 'pre_func1' failed for function 'func1'"
```

### Comparing `cpop-32.0.3/tests/func/test_raise_on_pre_failure.py` & `cpop-32.0.4/tests/func/test_raise_on_pre_failure.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/tests/integration/contract_ordering/single_module/contracts/default.py` & `cpop-32.0.4/tests/integration/contract_ordering/single_module/contracts/default.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/tests/integration/contract_ordering/single_module/contracts/dunder.py` & `cpop-32.0.4/tests/integration/contract_ordering/single_module/contracts/dunder.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/tests/integration/contract_ordering/single_module/contracts/init.py` & `cpop-32.0.4/tests/integration/contract_ordering/single_module/contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/tests/integration/contract_ordering/single_module/contracts/thing.py` & `cpop-32.0.4/tests/integration/contract_ordering/single_module/contracts/thing.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/tests/integration/contract_ordering/single_module/recursive_contracts/default.py` & `cpop-32.0.4/tests/integration/contract_ordering/single_module/recursive_contracts/default.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py` & `cpop-32.0.4/tests/integration/contract_ordering/single_module/recursive_contracts/dunder.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/tests/integration/contract_ordering/single_module/recursive_contracts/init.py` & `cpop-32.0.4/tests/integration/contract_ordering/single_module/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py` & `cpop-32.0.4/tests/integration/contract_ordering/single_module/recursive_contracts/thing.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py` & `cpop-32.0.4/tests/integration/recursive_contract/rc_sub1/rc_sub2/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py` & `cpop-32.0.4/tests/integration/recursive_contract/rc_sub1/recursive_contracts/init.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/tests/mods/proc.py` & `cpop-32.0.4/tests/mods/proc.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/tests/mods/test.py` & `cpop-32.0.4/tests/mods/test.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/tests/regression/contract_masking/test_contract_masking.py` & `cpop-32.0.4/tests/regression/contract_masking/test_contract_masking.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/tests/regression/contract_masking/test_duplicate_contracts.py` & `cpop-32.0.4/tests/regression/contract_masking/test_duplicate_contracts.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/tests/tpath/cn/contract/test.py` & `cpop-32.0.4/tests/tpath/cn/contract/test.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/tests/unit/test_contract.py` & `cpop-32.0.4/tests/unit/test_contract.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/tests/unit/test_sigs.py` & `cpop-32.0.4/tests/unit/test_sigs.py`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/.gitignore` & `cpop-32.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/README.rst` & `cpop-32.0.4/README.rst`

 * *Files identical despite different names*

### Comparing `cpop-32.0.3/pyproject.toml` & `cpop-32.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-cython"]
 build-backend = "hatchling.build"
 
 [project]
 name = "cpop"
-version = "32.0.3"
+version = "32.0.4"
 description = "The Cython-Optimized Plugin Oriented Programming System"
 readme = "README.rst"
 authors = [
     {name = "Tyler Levy Conde", email = "yonstib@gmail.com"},
     {name = "Thomas Hatch", email = "thatch45@gmail.com"},
 ]
 classifiers = [
```

### Comparing `cpop-32.0.3/PKG-INFO` & `cpop-32.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cpop
-Version: 32.0.3
+Version: 32.0.4
 Summary: The Cython-Optimized Plugin Oriented Programming System
 Author-email: Tyler Levy Conde <yonstib@gmail.com>, Thomas Hatch <thatch45@gmail.com>
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

