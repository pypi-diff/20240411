# Comparing `tmp/synrbl-0.0.1.tar.gz` & `tmp/synrbl-0.0.2.tar.gz`

## Comparing `synrbl-0.0.1.tar` & `synrbl-0.0.2.tar`

### file list

```diff
@@ -1,185 +1,142 @@
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 synrbl-0.0.1/.coveragerc
--rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 synrbl-0.0.1/.gitattributes
--rwxr-xr-x   0        0        0      228 2020-02-02 00:00:00.000000 synrbl-0.0.1/lint_check.sh
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 synrbl-0.0.1/reaction.json.gz
--rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 synrbl-0.0.1/requirements.txt
--rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 synrbl-0.0.1/setup.py
--rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 synrbl-0.0.1/synrbl.py
--rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 synrbl-0.0.1/synrbl_pilot.py
--rw-r--r--   0        0        0   815176 2020-02-02 00:00:00.000000 synrbl-0.0.1/Data/Raw_data/Golden/Golden.csv
--rw-r--r--   0        0        0    44593 2020-02-02 00:00:00.000000 synrbl-0.0.1/Data/Raw_data/Jaworski/complex.csv
--rw-r--r--   0        0        0   128945 2020-02-02 00:00:00.000000 synrbl-0.0.1/Data/Raw_data/Jaworski/patent.csv
--rw-r--r--   0        0        0    91588 2020-02-02 00:00:00.000000 synrbl-0.0.1/Data/Raw_data/Jaworski/typical.csv
--rw-r--r--   0        0        0  5788436 2020-02-02 00:00:00.000000 synrbl-0.0.1/Data/Raw_data/USPTO/USPTO_50K.csv
--rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 synrbl-0.0.1/Data/Rules/automated_rules.json.gz
--rw-r--r--   0        0        0    63599 2020-02-02 00:00:00.000000 synrbl-0.0.1/Data/Validation_set/Jaworski.csv
--rw-r--r--   0        0        0  5788436 2020-02-02 00:00:00.000000 synrbl-0.0.1/Data/Validation_set/USPTO_50K.csv
--rw-r--r--   0        0        0   188656 2020-02-02 00:00:00.000000 synrbl-0.0.1/Data/Validation_set/USPTO_diff.csv
--rw-r--r--   0        0        0    89839 2020-02-02 00:00:00.000000 synrbl-0.0.1/Data/Validation_set/USPTO_random_class.csv
--rw-r--r--   0        0        0    64959 2020-02-02 00:00:00.000000 synrbl-0.0.1/Data/Validation_set/USPTO_unbalance_class.csv
--rw-r--r--   0        0        0   677196 2020-02-02 00:00:00.000000 synrbl-0.0.1/Data/Validation_set/golden_dataset.csv
--rw-r--r--   0        0        0  1955873 2020-02-02 00:00:00.000000 synrbl-0.0.1/Data/Validation_set/validation_set.csv
--rw-r--r--   0        0        0  2769281 2020-02-02 00:00:00.000000 synrbl-0.0.1/Data/Validation_set/validation_set.json
--rw-r--r--   0        0        0    22209 2020-02-02 00:00:00.000000 synrbl-0.0.1/Docs/Examples/notebook.ipynb
--rw-r--r--   0        0        0    86666 2020-02-02 00:00:00.000000 synrbl-0.0.1/Docs/Images/Flowchart.png
--rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 synrbl-0.0.1/Docs/Paper_fig/figures.py
--rw-r--r--   0        0        0    55850 2020-02-02 00:00:00.000000 synrbl-0.0.1/Pipeline/Validation/Analysis/Analysis_vis.ipynb
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 synrbl-0.0.1/Pipeline/Validation/Analysis/SynRBL - Jaworski.csv
--rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 synrbl-0.0.1/Pipeline/Validation/Analysis/SynRBL - USPTO_diff.csv
--rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 synrbl-0.0.1/Pipeline/Validation/Analysis/SynRBL - USPTO_random_class.csv
--rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 synrbl-0.0.1/Pipeline/Validation/Analysis/SynRBL - USPTO_unbalance_class.csv
--rw-r--r--   0        0        0    13301 2020-02-02 00:00:00.000000 synrbl-0.0.1/Pipeline/Validation/Analysis/SynRBL - golden_dataset.csv
--rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 synrbl-0.0.1/Scripts/result_evaluation.py
--rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 synrbl-0.0.1/Scripts/validation_set_interface.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/__init__.py
--rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/confidence_prediction.py
--rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/main.py
--rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/mcs.py
--rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/postprocess.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/preprocess.py
--rw-r--r--   0        0        0    14738 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/rsmi_utils.py
--rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/rule_based.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynAnalysis/__init__.py
--rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynAnalysis/analysis_process.py
--rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynAnalysis/analysis_utils.py
--rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynAnalysis/eda_analysis.py
--rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynAnalysis/feature_analysis.py
--rw-r--r--   0        0        0   278926 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynAnalysis/scoring_function.dump
--rw-r--r--   0        0        0    16405 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynAnalysis/visualizer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynChemImputer/__init__.py
--rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynChemImputer/appel_reaction.py
--rw-r--r--   0        0        0     7786 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynChemImputer/functional_group_checker.py
--rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynChemImputer/peroxide_imputer.py
--rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynCmd/__init__.py
--rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynCmd/cmd_benchmark.py
--rw-r--r--   0        0        0     4243 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynCmd/cmd_run.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynCmd/logging.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynMCSImputer/__init__.py
--rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynMCSImputer/compound_rules.json
--rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynMCSImputer/expand_rules.json
--rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynMCSImputer/merge.py
--rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynMCSImputer/merge_rules.json
--rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynMCSImputer/merge_rules_example.json
--rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynMCSImputer/model.py
--rw-r--r--   0        0        0    29044 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynMCSImputer/rules.py
--rw-r--r--   0        0        0     6768 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynMCSImputer/structure.py
--rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynMCSImputer/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynMCSImputer/MissingGraph/__init__.py
--rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynMCSImputer/MissingGraph/find_graph_dict.py
--rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynMCSImputer/MissingGraph/find_missing_graphs.py
--rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynMCSImputer/MissingGraph/molcurator.py
--rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynMCSImputer/MissingGraph/refinement_uncertainty.py
--rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynMCSImputer/MissingGraph/uncertainty_graph.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynMCSImputer/SubStructure/__init__.py
--rw-r--r--   0        0        0    11814 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynMCSImputer/SubStructure/extract_common_mcs.py
--rw-r--r--   0        0        0     9958 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynMCSImputer/SubStructure/mcs_graph_detector.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynMCSImputer/SubStructure/mcs_process.py
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynMCSImputer/SubStructure/substructure_analyzer.py
--rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynProcessor/__init__.py
--rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynProcessor/check_carbon_balance.py
--rw-r--r--   0        0        0     5245 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynProcessor/rsmi_both_side_process.py
--rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynProcessor/rsmi_comparator.py
--rw-r--r--   0        0        0     7320 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynProcessor/rsmi_decomposer.py
--rw-r--r--   0        0        0     7209 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynProcessor/rsmi_processing.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynRuleImputer/__init__.py
--rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynRuleImputer/auto_extract_rules.py
--rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynRuleImputer/auto_extract_smiles.py
--rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynRuleImputer/rule_data_manager.py
--rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynRuleImputer/rules_manager.json.gz
--rw-r--r--   0        0        0     9182 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynRuleImputer/synthetic_rule_constraint.py
--rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynRuleImputer/synthetic_rule_imputer.py
--rw-r--r--   0        0        0     8858 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynRuleImputer/synthetic_rule_matcher.py
--rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynUtils/__init__.py
--rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynUtils/chem_utils.py
--rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynUtils/common.py
--rw-r--r--   0        0        0    11925 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynUtils/data_utils.py
--rw-r--r--   0        0        0     9444 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynUtils/functional_group_utils.py
--rw-r--r--   0        0        0    14679 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynUtils/rsmi_utils.py
--rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynVis/__init__.py
--rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynVis/mcs_visualizer.py
--rw-r--r--   0        0        0     9300 2020-02-02 00:00:00.000000 synrbl-0.0.1/SynRBL/SynVis/reaction_visualizer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/__init__.py
--rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynChemImputer/test_appeal_reaction.py
--rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynChemImputer/test_peroxide_imputer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynMCSImputer/__init__.py
--rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynMCSImputer/test_merge.py
--rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynMCSImputer/test_model.py
--rw-r--r--   0        0        0    11025 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynMCSImputer/test_rules.py
--rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynMCSImputer/test_structure.py
--rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynMCSImputer/test_utils.py
--rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynMCSImputer/MissingGraph/test_find_graph_dict.py
--rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynMCSImputer/MissingGraph/test_find_missing_graphs.py
--rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynMCSImputer/MissingGraph/test_molcurator.py
--rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynMCSImputer/MissingGraph/test_uncertainty_graph.py
--rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynMCSImputer/SubStructure/test_extract_common_mcs.py
--rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynMCSImputer/SubStructure/test_mcs_graph_detector.py
--rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynMCSImputer/SubStructure/test_mcs_process.py
--rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynMCSImputer/SubStructure/test_substructure_analyzer.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynProcessor/__init__.py
--rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynProcessor/test_check_carbon_balance.py
--rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynProcessor/test_rmsi_comparator.py
--rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynProcessor/test_rmsi_decomposer.py
--rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynProcessor/test_rmsi_processing.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynRuleImputer/__init__.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynRuleImputer/test_auto_extract_rules.py
--rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynRuleImputer/test_auto_extract_smiles.py
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynRuleImputer/test_rule_constraint.py
--rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynRuleImputer/test_rule_data_manager.py
--rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynRuleImputer/test_synthetic_rule_imputer.py
--rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynRuleImputer/test_synthetic_rule_matcher.py
--rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynUtils/test_chem_utils.py
--rw-r--r--   0        0        0     8918 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynUtils/test_functional_group_utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynVis/__init__.py
--rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 synrbl-0.0.1/Test/SynVis/test_reaction_visualizer.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/.gitignore
--rw-r--r--   0        0        0    21865 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/coverage_html.js
--rw-r--r--   0        0        0    37998 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_09022e60b285fc03_merge_py.html
--rw-r--r--   0        0        0    43561 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_09022e60b285fc03_model_py.html
--rw-r--r--   0        0        0   242275 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_09022e60b285fc03_rules_py.html
--rw-r--r--   0        0        0    66554 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_09022e60b285fc03_structure_py.html
--rw-r--r--   0        0        0    43543 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_09022e60b285fc03_utils_py.html
--rw-r--r--   0        0        0    72307 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_14cc0e59e8251033_chem_utils_py.html
--rw-r--r--   0        0        0     7729 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_14cc0e59e8251033_common_py.html
--rw-r--r--   0        0        0    89824 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_14cc0e59e8251033_data_utils_py.html
--rw-r--r--   0        0        0    87842 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_14cc0e59e8251033_functional_group_utils_py.html
--rw-r--r--   0        0        0    35300 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_2aa998d7320c3ea5_analysis_utils_py.html
--rw-r--r--   0        0        0    26309 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_2fa482a02b84ec6a_auto_extract_rules_py.html
--rw-r--r--   0        0        0    43367 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_2fa482a02b84ec6a_auto_extract_smiles_py.html
--rw-r--r--   0        0        0    43882 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_2fa482a02b84ec6a_rule_data_manager_py.html
--rw-r--r--   0        0        0    69288 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_2fa482a02b84ec6a_synthetic_rule_constraint_py.html
--rw-r--r--   0        0        0    41163 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_2fa482a02b84ec6a_synthetic_rule_imputer_py.html
--rw-r--r--   0        0        0    67515 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_2fa482a02b84ec6a_synthetic_rule_matcher_py.html
--rw-r--r--   0        0        0    48572 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_454370984969b610_find_graph_dict_py.html
--rw-r--r--   0        0        0    62568 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_454370984969b610_find_missing_graphs_py.html
--rw-r--r--   0        0        0    30203 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_454370984969b610_molcurator_py.html
--rw-r--r--   0        0        0    27990 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_454370984969b610_uncertainty_graph_py.html
--rw-r--r--   0        0        0    68630 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_631933eb2c7348e4_reaction_visualizer_py.html
--rw-r--r--   0        0        0    24557 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_85ac37c667340548_confidence_prediction_py.html
--rw-r--r--   0        0        0    33625 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_85ac37c667340548_main_py.html
--rw-r--r--   0        0        0    28320 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_85ac37c667340548_mcs_py.html
--rw-r--r--   0        0        0    23318 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_85ac37c667340548_postprocess_py.html
--rw-r--r--   0        0        0    12046 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_85ac37c667340548_preprocess_py.html
--rw-r--r--   0        0        0   109336 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_85ac37c667340548_rsmi_utils_py.html
--rw-r--r--   0        0        0    44391 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_85ac37c667340548_rule_based_py.html
--rw-r--r--   0        0        0    36972 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_8f1918bee0e3b2c1_check_carbon_balance_py.html
--rw-r--r--   0        0        0    38659 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_8f1918bee0e3b2c1_rsmi_both_side_process_py.html
--rw-r--r--   0        0        0    49394 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_8f1918bee0e3b2c1_rsmi_comparator_py.html
--rw-r--r--   0        0        0    65048 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_8f1918bee0e3b2c1_rsmi_decomposer_py.html
--rw-r--r--   0        0        0    51142 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_8f1918bee0e3b2c1_rsmi_processing_py.html
--rw-r--r--   0        0        0    30496 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_b943f5a2ccfc8bc3_appel_reaction_py.html
--rw-r--r--   0        0        0    27887 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_b943f5a2ccfc8bc3_peroxide_imputer_py.html
--rw-r--r--   0        0        0    81363 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_eb6e41804575f727_extract_common_mcs_py.html
--rw-r--r--   0        0        0    71849 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_eb6e41804575f727_mcs_graph_detector_py.html
--rw-r--r--   0        0        0    30348 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_eb6e41804575f727_mcs_process_py.html
--rw-r--r--   0        0        0    26917 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/d_eb6e41804575f727_substructure_analyzer_py.html
--rw-r--r--   0        0        0     1732 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/favicon_32.png
--rw-r--r--   0        0        0    16497 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/index.html
--rw-r--r--   0        0        0     9004 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/keybd_closed.png
--rw-r--r--   0        0        0     9003 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/keybd_open.png
--rw-r--r--   0        0        0     9672 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/status.json
--rw-r--r--   0        0        0    12406 2020-02-02 00:00:00.000000 synrbl-0.0.1/htmlcov/style.css
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 synrbl-0.0.1/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 synrbl-0.0.1/LICENSE
--rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 synrbl-0.0.1/README.md
--rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 synrbl-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4390 2020-02-02 00:00:00.000000 synrbl-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 synrbl-0.0.2/.coveragerc
+-rw-r--r--   0        0        0       66 2020-02-02 00:00:00.000000 synrbl-0.0.2/.gitattributes
+-rwxr-xr-x   0        0        0      216 2020-02-02 00:00:00.000000 synrbl-0.0.2/lint_check.sh
+-rw-r--r--   0        0        0      129 2020-02-02 00:00:00.000000 synrbl-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 synrbl-0.0.2/setup.py
+-rw-r--r--   0        0        0      473 2020-02-02 00:00:00.000000 synrbl-0.0.2/synrbl.py
+-rw-r--r--   0        0        0     3242 2020-02-02 00:00:00.000000 synrbl-0.0.2/synrbl_pilot.py
+-rw-r--r--   0        0        0     1108 2020-02-02 00:00:00.000000 synrbl-0.0.2/.github/workflows/publish-package.yml
+-rw-r--r--   0        0        0     1041 2020-02-02 00:00:00.000000 synrbl-0.0.2/.github/workflows/test-and-lint.yml
+-rw-r--r--   0        0        0   815176 2020-02-02 00:00:00.000000 synrbl-0.0.2/Data/Raw_data/Golden/Golden.csv
+-rw-r--r--   0        0        0    44593 2020-02-02 00:00:00.000000 synrbl-0.0.2/Data/Raw_data/Jaworski/complex.csv
+-rw-r--r--   0        0        0   128945 2020-02-02 00:00:00.000000 synrbl-0.0.2/Data/Raw_data/Jaworski/patent.csv
+-rw-r--r--   0        0        0    91588 2020-02-02 00:00:00.000000 synrbl-0.0.2/Data/Raw_data/Jaworski/typical.csv
+-rw-r--r--   0        0        0  5788436 2020-02-02 00:00:00.000000 synrbl-0.0.2/Data/Raw_data/USPTO/USPTO_50K.csv
+-rw-r--r--   0        0        0     1480 2020-02-02 00:00:00.000000 synrbl-0.0.2/Data/Rules/automated_rules.json.gz
+-rw-r--r--   0        0        0    63599 2020-02-02 00:00:00.000000 synrbl-0.0.2/Data/Validation_set/Jaworski.csv
+-rw-r--r--   0        0        0  5788436 2020-02-02 00:00:00.000000 synrbl-0.0.2/Data/Validation_set/USPTO_50K.csv
+-rw-r--r--   0        0        0   188656 2020-02-02 00:00:00.000000 synrbl-0.0.2/Data/Validation_set/USPTO_diff.csv
+-rw-r--r--   0        0        0    89839 2020-02-02 00:00:00.000000 synrbl-0.0.2/Data/Validation_set/USPTO_random_class.csv
+-rw-r--r--   0        0        0    64959 2020-02-02 00:00:00.000000 synrbl-0.0.2/Data/Validation_set/USPTO_unbalance_class.csv
+-rw-r--r--   0        0        0   677196 2020-02-02 00:00:00.000000 synrbl-0.0.2/Data/Validation_set/golden_dataset.csv
+-rw-r--r--   0        0        0  1955873 2020-02-02 00:00:00.000000 synrbl-0.0.2/Data/Validation_set/validation_set.csv
+-rw-r--r--   0        0        0  2769281 2020-02-02 00:00:00.000000 synrbl-0.0.2/Data/Validation_set/validation_set.json
+-rw-r--r--   0        0        0    22209 2020-02-02 00:00:00.000000 synrbl-0.0.2/Docs/Examples/notebook.ipynb
+-rw-r--r--   0        0        0    86666 2020-02-02 00:00:00.000000 synrbl-0.0.2/Docs/Images/Flowchart.png
+-rw-r--r--   0        0        0     3756 2020-02-02 00:00:00.000000 synrbl-0.0.2/Docs/Paper_fig/figures.py
+-rw-r--r--   0        0        0    55850 2020-02-02 00:00:00.000000 synrbl-0.0.2/Pipeline/Validation/Analysis/Analysis_vis.ipynb
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 synrbl-0.0.2/Pipeline/Validation/Analysis/SynRBL - Jaworski.csv
+-rw-r--r--   0        0        0     5678 2020-02-02 00:00:00.000000 synrbl-0.0.2/Pipeline/Validation/Analysis/SynRBL - USPTO_diff.csv
+-rw-r--r--   0        0        0     5671 2020-02-02 00:00:00.000000 synrbl-0.0.2/Pipeline/Validation/Analysis/SynRBL - USPTO_random_class.csv
+-rw-r--r--   0        0        0     3014 2020-02-02 00:00:00.000000 synrbl-0.0.2/Pipeline/Validation/Analysis/SynRBL - USPTO_unbalance_class.csv
+-rw-r--r--   0        0        0    13301 2020-02-02 00:00:00.000000 synrbl-0.0.2/Pipeline/Validation/Analysis/SynRBL - golden_dataset.csv
+-rw-r--r--   0        0        0     4845 2020-02-02 00:00:00.000000 synrbl-0.0.2/Scripts/result_evaluation.py
+-rw-r--r--   0        0        0     1638 2020-02-02 00:00:00.000000 synrbl-0.0.2/Scripts/validation_set_interface.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/__init__.py
+-rw-r--r--   0        0        0     2454 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/confidence_prediction.py
+-rw-r--r--   0        0        0     3327 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/main.py
+-rw-r--r--   0        0        0     2966 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/mcs.py
+-rw-r--r--   0        0        0     2315 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/postprocess.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/preprocess.py
+-rw-r--r--   0        0        0    14738 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/rsmi_utils.py
+-rw-r--r--   0        0        0     4690 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/rule_based.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynAnalysis/__init__.py
+-rw-r--r--   0        0        0     4061 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynAnalysis/analysis_process.py
+-rw-r--r--   0        0        0     4104 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynAnalysis/analysis_utils.py
+-rw-r--r--   0        0        0    10195 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynAnalysis/eda_analysis.py
+-rw-r--r--   0        0        0     3740 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynAnalysis/feature_analysis.py
+-rw-r--r--   0        0        0   278926 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynAnalysis/scoring_function.dump
+-rw-r--r--   0        0        0    16405 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynAnalysis/visualizer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynChemImputer/__init__.py
+-rw-r--r--   0        0        0     3657 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynChemImputer/appel_reaction.py
+-rw-r--r--   0        0        0     7786 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynChemImputer/functional_group_checker.py
+-rw-r--r--   0        0        0     3397 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynChemImputer/peroxide_imputer.py
+-rw-r--r--   0        0        0      537 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynCmd/__init__.py
+-rw-r--r--   0        0        0     4820 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynCmd/cmd_benchmark.py
+-rw-r--r--   0        0        0     4243 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynCmd/cmd_run.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynCmd/logging.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynMCSImputer/__init__.py
+-rw-r--r--   0        0        0      516 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynMCSImputer/compound_rules.json
+-rw-r--r--   0        0        0     1611 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynMCSImputer/expand_rules.json
+-rw-r--r--   0        0        0     4192 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynMCSImputer/merge.py
+-rw-r--r--   0        0        0     1264 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynMCSImputer/merge_rules.json
+-rw-r--r--   0        0        0      425 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynMCSImputer/merge_rules_example.json
+-rw-r--r--   0        0        0     5037 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynMCSImputer/model.py
+-rw-r--r--   0        0        0    29044 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynMCSImputer/rules.py
+-rw-r--r--   0        0        0     6768 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynMCSImputer/structure.py
+-rw-r--r--   0        0        0     5169 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynMCSImputer/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynMCSImputer/MissingGraph/__init__.py
+-rw-r--r--   0        0        0     6700 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynMCSImputer/MissingGraph/find_graph_dict.py
+-rw-r--r--   0        0        0     9205 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynMCSImputer/MissingGraph/find_missing_graphs.py
+-rw-r--r--   0        0        0     3564 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynMCSImputer/MissingGraph/molcurator.py
+-rw-r--r--   0        0        0     3720 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynMCSImputer/MissingGraph/refinement_uncertainty.py
+-rw-r--r--   0        0        0     3563 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynMCSImputer/MissingGraph/uncertainty_graph.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynMCSImputer/SubStructure/__init__.py
+-rw-r--r--   0        0        0    11814 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynMCSImputer/SubStructure/extract_common_mcs.py
+-rw-r--r--   0        0        0     9958 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynMCSImputer/SubStructure/mcs_graph_detector.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynMCSImputer/SubStructure/mcs_process.py
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynMCSImputer/SubStructure/substructure_analyzer.py
+-rw-r--r--   0        0        0      235 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynProcessor/__init__.py
+-rw-r--r--   0        0        0     4253 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynProcessor/check_carbon_balance.py
+-rw-r--r--   0        0        0     5245 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynProcessor/rsmi_both_side_process.py
+-rw-r--r--   0        0        0     6541 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynProcessor/rsmi_comparator.py
+-rw-r--r--   0        0        0     7320 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynProcessor/rsmi_decomposer.py
+-rw-r--r--   0        0        0     7210 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynProcessor/rsmi_processing.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynRuleImputer/__init__.py
+-rw-r--r--   0        0        0     3125 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynRuleImputer/auto_extract_rules.py
+-rw-r--r--   0        0        0     5396 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynRuleImputer/auto_extract_smiles.py
+-rw-r--r--   0        0        0     5471 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynRuleImputer/rule_data_manager.py
+-rw-r--r--   0        0        0     4176 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynRuleImputer/rules_manager.json.gz
+-rw-r--r--   0        0        0     9182 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynRuleImputer/synthetic_rule_constraint.py
+-rw-r--r--   0        0        0     5405 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynRuleImputer/synthetic_rule_imputer.py
+-rw-r--r--   0        0        0     8858 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynRuleImputer/synthetic_rule_matcher.py
+-rw-r--r--   0        0        0      435 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynUtils/__init__.py
+-rw-r--r--   0        0        0     8875 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynUtils/chem_utils.py
+-rw-r--r--   0        0        0      321 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynUtils/common.py
+-rw-r--r--   0        0        0    11925 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynUtils/data_utils.py
+-rw-r--r--   0        0        0     9444 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynUtils/functional_group_utils.py
+-rw-r--r--   0        0        0    14679 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynUtils/rsmi_utils.py
+-rw-r--r--   0        0        0       52 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynVis/__init__.py
+-rw-r--r--   0        0        0     4241 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynVis/mcs_visualizer.py
+-rw-r--r--   0        0        0     9300 2020-02-02 00:00:00.000000 synrbl-0.0.2/SynRBL/SynVis/reaction_visualizer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynChemImputer/__init__.py
+-rw-r--r--   0        0        0     3864 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynChemImputer/test_appeal_reaction.py
+-rw-r--r--   0        0        0     1822 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynChemImputer/test_peroxide_imputer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynMCSImputer/__init__.py
+-rw-r--r--   0        0        0    12934 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynMCSImputer/test_merge.py
+-rw-r--r--   0        0        0     5575 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynMCSImputer/test_model.py
+-rw-r--r--   0        0        0    11025 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynMCSImputer/test_rules.py
+-rw-r--r--   0        0        0     2769 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynMCSImputer/test_structure.py
+-rw-r--r--   0        0        0      524 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynMCSImputer/test_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynMCSImputer/MissingGraph/__init__.py
+-rw-r--r--   0        0        0     2032 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynMCSImputer/MissingGraph/test_find_graph_dict.py
+-rw-r--r--   0        0        0     2609 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynMCSImputer/MissingGraph/test_find_missing_graphs.py
+-rw-r--r--   0        0        0     1010 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynMCSImputer/MissingGraph/test_molcurator.py
+-rw-r--r--   0        0        0     1649 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynMCSImputer/MissingGraph/test_uncertainty_graph.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynMCSImputer/SubStructure/__init__.py
+-rw-r--r--   0        0        0     2942 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynMCSImputer/SubStructure/test_extract_common_mcs.py
+-rw-r--r--   0        0        0     4692 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynMCSImputer/SubStructure/test_mcs_graph_detector.py
+-rw-r--r--   0        0        0     1307 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynMCSImputer/SubStructure/test_mcs_process.py
+-rw-r--r--   0        0        0     2184 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynMCSImputer/SubStructure/test_substructure_analyzer.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynProcessor/__init__.py
+-rw-r--r--   0        0        0     1902 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynProcessor/test_check_carbon_balance.py
+-rw-r--r--   0        0        0     2410 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynProcessor/test_rmsi_comparator.py
+-rw-r--r--   0        0        0     1660 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynProcessor/test_rmsi_decomposer.py
+-rw-r--r--   0        0        0     3648 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynProcessor/test_rmsi_processing.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynRuleImputer/__init__.py
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynRuleImputer/test_auto_extract_rules.py
+-rw-r--r--   0        0        0     1428 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynRuleImputer/test_auto_extract_smiles.py
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynRuleImputer/test_rule_constraint.py
+-rw-r--r--   0        0        0     2308 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynRuleImputer/test_rule_data_manager.py
+-rw-r--r--   0        0        0     2161 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynRuleImputer/test_synthetic_rule_imputer.py
+-rw-r--r--   0        0        0     2183 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynRuleImputer/test_synthetic_rule_matcher.py
+-rw-r--r--   0        0        0     2755 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynUtils/test_chem_utils.py
+-rw-r--r--   0        0        0     8918 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynUtils/test_functional_group_utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynVis/__init__.py
+-rw-r--r--   0        0        0      531 2020-02-02 00:00:00.000000 synrbl-0.0.2/Test/SynVis/test_reaction_visualizer.py
+-rw-r--r--   0        0        0      141 2020-02-02 00:00:00.000000 synrbl-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 synrbl-0.0.2/LICENSE
+-rw-r--r--   0        0        0     3508 2020-02-02 00:00:00.000000 synrbl-0.0.2/README.md
+-rw-r--r--   0        0        0      877 2020-02-02 00:00:00.000000 synrbl-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0     4390 2020-02-02 00:00:00.000000 synrbl-0.0.2/PKG-INFO
```

### Comparing `synrbl-0.0.1/setup.py` & `synrbl-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/synrbl_pilot.py` & `synrbl-0.0.2/synrbl_pilot.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Data/Raw_data/Golden/Golden.csv` & `synrbl-0.0.2/Data/Raw_data/Golden/Golden.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Data/Raw_data/Jaworski/complex.csv` & `synrbl-0.0.2/Data/Raw_data/Jaworski/complex.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Data/Raw_data/Jaworski/patent.csv` & `synrbl-0.0.2/Data/Raw_data/Jaworski/patent.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Data/Raw_data/Jaworski/typical.csv` & `synrbl-0.0.2/Data/Raw_data/Jaworski/typical.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Data/Raw_data/USPTO/USPTO_50K.csv` & `synrbl-0.0.2/Data/Raw_data/USPTO/USPTO_50K.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Data/Rules/automated_rules.json.gz` & `synrbl-0.0.2/Data/Rules/automated_rules.json.gz`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Data/Validation_set/Jaworski.csv` & `synrbl-0.0.2/Data/Validation_set/Jaworski.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Data/Validation_set/USPTO_50K.csv` & `synrbl-0.0.2/Data/Validation_set/USPTO_50K.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Data/Validation_set/USPTO_diff.csv` & `synrbl-0.0.2/Data/Validation_set/USPTO_diff.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Data/Validation_set/USPTO_random_class.csv` & `synrbl-0.0.2/Data/Validation_set/USPTO_random_class.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Data/Validation_set/USPTO_unbalance_class.csv` & `synrbl-0.0.2/Data/Validation_set/USPTO_unbalance_class.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Data/Validation_set/golden_dataset.csv` & `synrbl-0.0.2/Data/Validation_set/golden_dataset.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Data/Validation_set/validation_set.csv` & `synrbl-0.0.2/Data/Validation_set/validation_set.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Data/Validation_set/validation_set.json` & `synrbl-0.0.2/Data/Validation_set/validation_set.json`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Docs/Examples/notebook.ipynb` & `synrbl-0.0.2/Docs/Examples/notebook.ipynb`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Docs/Images/Flowchart.png` & `synrbl-0.0.2/Docs/Images/Flowchart.png`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Docs/Paper_fig/figures.py` & `synrbl-0.0.2/Docs/Paper_fig/figures.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Pipeline/Validation/Analysis/Analysis_vis.ipynb` & `synrbl-0.0.2/Pipeline/Validation/Analysis/Analysis_vis.ipynb`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Pipeline/Validation/Analysis/SynRBL - Jaworski.csv` & `synrbl-0.0.2/Pipeline/Validation/Analysis/SynRBL - Jaworski.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Pipeline/Validation/Analysis/SynRBL - USPTO_diff.csv` & `synrbl-0.0.2/Pipeline/Validation/Analysis/SynRBL - USPTO_diff.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Pipeline/Validation/Analysis/SynRBL - USPTO_random_class.csv` & `synrbl-0.0.2/Pipeline/Validation/Analysis/SynRBL - USPTO_random_class.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Pipeline/Validation/Analysis/SynRBL - USPTO_unbalance_class.csv` & `synrbl-0.0.2/Pipeline/Validation/Analysis/SynRBL - USPTO_unbalance_class.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Pipeline/Validation/Analysis/SynRBL - golden_dataset.csv` & `synrbl-0.0.2/Pipeline/Validation/Analysis/SynRBL - golden_dataset.csv`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Scripts/result_evaluation.py` & `synrbl-0.0.2/Scripts/result_evaluation.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Scripts/validation_set_interface.py` & `synrbl-0.0.2/Scripts/validation_set_interface.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/confidence_prediction.py` & `synrbl-0.0.2/SynRBL/confidence_prediction.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/main.py` & `synrbl-0.0.2/SynRBL/main.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/mcs.py` & `synrbl-0.0.2/SynRBL/mcs.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/postprocess.py` & `synrbl-0.0.2/SynRBL/postprocess.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/preprocess.py` & `synrbl-0.0.2/SynRBL/preprocess.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/rsmi_utils.py` & `synrbl-0.0.2/SynRBL/rsmi_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/rule_based.py` & `synrbl-0.0.2/SynRBL/rule_based.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynAnalysis/analysis_process.py` & `synrbl-0.0.2/SynRBL/SynAnalysis/analysis_process.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynAnalysis/analysis_utils.py` & `synrbl-0.0.2/SynRBL/SynAnalysis/analysis_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynAnalysis/eda_analysis.py` & `synrbl-0.0.2/SynRBL/SynAnalysis/eda_analysis.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynAnalysis/feature_analysis.py` & `synrbl-0.0.2/SynRBL/SynAnalysis/feature_analysis.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynAnalysis/scoring_function.dump` & `synrbl-0.0.2/SynRBL/SynAnalysis/scoring_function.dump`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynAnalysis/visualizer.py` & `synrbl-0.0.2/SynRBL/SynAnalysis/visualizer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynChemImputer/appel_reaction.py` & `synrbl-0.0.2/SynRBL/SynChemImputer/appel_reaction.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynChemImputer/functional_group_checker.py` & `synrbl-0.0.2/SynRBL/SynChemImputer/functional_group_checker.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynChemImputer/peroxide_imputer.py` & `synrbl-0.0.2/SynRBL/SynChemImputer/peroxide_imputer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynCmd/__init__.py` & `synrbl-0.0.2/SynRBL/SynCmd/__init__.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynCmd/cmd_benchmark.py` & `synrbl-0.0.2/SynRBL/SynCmd/cmd_benchmark.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynCmd/cmd_run.py` & `synrbl-0.0.2/SynRBL/SynCmd/cmd_run.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynMCSImputer/compound_rules.json` & `synrbl-0.0.2/SynRBL/SynMCSImputer/compound_rules.json`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynMCSImputer/expand_rules.json` & `synrbl-0.0.2/SynRBL/SynMCSImputer/expand_rules.json`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynMCSImputer/merge.py` & `synrbl-0.0.2/SynRBL/SynMCSImputer/merge.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynMCSImputer/merge_rules.json` & `synrbl-0.0.2/SynRBL/SynMCSImputer/merge_rules.json`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynMCSImputer/model.py` & `synrbl-0.0.2/SynRBL/SynMCSImputer/model.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynMCSImputer/rules.py` & `synrbl-0.0.2/SynRBL/SynMCSImputer/rules.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynMCSImputer/structure.py` & `synrbl-0.0.2/SynRBL/SynMCSImputer/structure.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynMCSImputer/utils.py` & `synrbl-0.0.2/SynRBL/SynMCSImputer/utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynMCSImputer/MissingGraph/find_graph_dict.py` & `synrbl-0.0.2/SynRBL/SynMCSImputer/MissingGraph/find_graph_dict.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynMCSImputer/MissingGraph/find_missing_graphs.py` & `synrbl-0.0.2/SynRBL/SynMCSImputer/MissingGraph/find_missing_graphs.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynMCSImputer/MissingGraph/molcurator.py` & `synrbl-0.0.2/SynRBL/SynMCSImputer/MissingGraph/molcurator.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynMCSImputer/MissingGraph/refinement_uncertainty.py` & `synrbl-0.0.2/SynRBL/SynMCSImputer/MissingGraph/refinement_uncertainty.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynMCSImputer/MissingGraph/uncertainty_graph.py` & `synrbl-0.0.2/SynRBL/SynMCSImputer/MissingGraph/uncertainty_graph.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynMCSImputer/SubStructure/extract_common_mcs.py` & `synrbl-0.0.2/SynRBL/SynMCSImputer/SubStructure/extract_common_mcs.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynMCSImputer/SubStructure/mcs_graph_detector.py` & `synrbl-0.0.2/SynRBL/SynMCSImputer/SubStructure/mcs_graph_detector.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynMCSImputer/SubStructure/mcs_process.py` & `synrbl-0.0.2/SynRBL/SynMCSImputer/SubStructure/mcs_process.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynMCSImputer/SubStructure/substructure_analyzer.py` & `synrbl-0.0.2/SynRBL/SynMCSImputer/SubStructure/substructure_analyzer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynProcessor/check_carbon_balance.py` & `synrbl-0.0.2/SynRBL/SynProcessor/check_carbon_balance.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynProcessor/rsmi_both_side_process.py` & `synrbl-0.0.2/SynRBL/SynProcessor/rsmi_both_side_process.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynProcessor/rsmi_comparator.py` & `synrbl-0.0.2/SynRBL/SynProcessor/rsmi_comparator.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynProcessor/rsmi_decomposer.py` & `synrbl-0.0.2/SynRBL/SynProcessor/rsmi_decomposer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynProcessor/rsmi_processing.py` & `synrbl-0.0.2/SynRBL/SynProcessor/rsmi_processing.py`

 * *Files 0% similar despite different names*

```diff
@@ -56,15 +56,15 @@
         index_col: str = "R-id",
         rsmi_col: str = None,
         symbol: str = ">>",
         n_jobs: int = 4,
         drop_duplicates: bool = True,
         verbose: int = 1,
         parallel: bool = True,
-        save_json: bool = True,
+        save_json: bool = False,
         save_path_name: str = "reaction.json.gz",
         orient: str = "records",
         compression: str = "gzip",
     ) -> None:
         self.reaction_smiles = reaction_smiles
         self.symbol = symbol
         self.n_jobs = n_jobs
```

### Comparing `synrbl-0.0.1/SynRBL/SynRuleImputer/auto_extract_rules.py` & `synrbl-0.0.2/SynRBL/SynRuleImputer/auto_extract_rules.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynRuleImputer/auto_extract_smiles.py` & `synrbl-0.0.2/SynRBL/SynRuleImputer/auto_extract_smiles.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynRuleImputer/rule_data_manager.py` & `synrbl-0.0.2/SynRBL/SynRuleImputer/rule_data_manager.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynRuleImputer/rules_manager.json.gz` & `synrbl-0.0.2/SynRBL/SynRuleImputer/rules_manager.json.gz`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynRuleImputer/synthetic_rule_constraint.py` & `synrbl-0.0.2/SynRBL/SynRuleImputer/synthetic_rule_constraint.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynRuleImputer/synthetic_rule_imputer.py` & `synrbl-0.0.2/SynRBL/SynRuleImputer/synthetic_rule_imputer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynRuleImputer/synthetic_rule_matcher.py` & `synrbl-0.0.2/SynRBL/SynRuleImputer/synthetic_rule_matcher.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynUtils/chem_utils.py` & `synrbl-0.0.2/SynRBL/SynUtils/chem_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynUtils/data_utils.py` & `synrbl-0.0.2/SynRBL/SynUtils/data_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynUtils/functional_group_utils.py` & `synrbl-0.0.2/SynRBL/SynUtils/functional_group_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynUtils/rsmi_utils.py` & `synrbl-0.0.2/SynRBL/SynUtils/rsmi_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynVis/mcs_visualizer.py` & `synrbl-0.0.2/SynRBL/SynVis/mcs_visualizer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/SynRBL/SynVis/reaction_visualizer.py` & `synrbl-0.0.2/SynRBL/SynVis/reaction_visualizer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynChemImputer/test_appeal_reaction.py` & `synrbl-0.0.2/Test/SynChemImputer/test_appeal_reaction.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynChemImputer/test_peroxide_imputer.py` & `synrbl-0.0.2/Test/SynChemImputer/test_peroxide_imputer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynMCSImputer/test_merge.py` & `synrbl-0.0.2/Test/SynMCSImputer/test_merge.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynMCSImputer/test_model.py` & `synrbl-0.0.2/Test/SynMCSImputer/test_model.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynMCSImputer/test_rules.py` & `synrbl-0.0.2/Test/SynMCSImputer/test_rules.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynMCSImputer/test_structure.py` & `synrbl-0.0.2/Test/SynMCSImputer/test_structure.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynMCSImputer/test_utils.py` & `synrbl-0.0.2/Test/SynMCSImputer/test_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynMCSImputer/MissingGraph/test_find_graph_dict.py` & `synrbl-0.0.2/Test/SynMCSImputer/MissingGraph/test_find_graph_dict.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynMCSImputer/MissingGraph/test_find_missing_graphs.py` & `synrbl-0.0.2/Test/SynMCSImputer/MissingGraph/test_find_missing_graphs.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynMCSImputer/MissingGraph/test_molcurator.py` & `synrbl-0.0.2/Test/SynMCSImputer/MissingGraph/test_molcurator.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynMCSImputer/MissingGraph/test_uncertainty_graph.py` & `synrbl-0.0.2/Test/SynMCSImputer/MissingGraph/test_uncertainty_graph.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynMCSImputer/SubStructure/test_extract_common_mcs.py` & `synrbl-0.0.2/Test/SynMCSImputer/SubStructure/test_extract_common_mcs.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynMCSImputer/SubStructure/test_mcs_graph_detector.py` & `synrbl-0.0.2/Test/SynMCSImputer/SubStructure/test_mcs_graph_detector.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynMCSImputer/SubStructure/test_mcs_process.py` & `synrbl-0.0.2/Test/SynMCSImputer/SubStructure/test_mcs_process.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynMCSImputer/SubStructure/test_substructure_analyzer.py` & `synrbl-0.0.2/Test/SynMCSImputer/SubStructure/test_substructure_analyzer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynProcessor/test_check_carbon_balance.py` & `synrbl-0.0.2/Test/SynProcessor/test_check_carbon_balance.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynProcessor/test_rmsi_comparator.py` & `synrbl-0.0.2/Test/SynProcessor/test_rmsi_comparator.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynProcessor/test_rmsi_decomposer.py` & `synrbl-0.0.2/Test/SynProcessor/test_rmsi_decomposer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynProcessor/test_rmsi_processing.py` & `synrbl-0.0.2/Test/SynProcessor/test_rmsi_processing.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynRuleImputer/test_auto_extract_rules.py` & `synrbl-0.0.2/Test/SynRuleImputer/test_auto_extract_rules.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynRuleImputer/test_auto_extract_smiles.py` & `synrbl-0.0.2/Test/SynRuleImputer/test_auto_extract_smiles.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynRuleImputer/test_rule_constraint.py` & `synrbl-0.0.2/Test/SynRuleImputer/test_rule_constraint.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynRuleImputer/test_rule_data_manager.py` & `synrbl-0.0.2/Test/SynRuleImputer/test_rule_data_manager.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynRuleImputer/test_synthetic_rule_imputer.py` & `synrbl-0.0.2/Test/SynRuleImputer/test_synthetic_rule_imputer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynRuleImputer/test_synthetic_rule_matcher.py` & `synrbl-0.0.2/Test/SynRuleImputer/test_synthetic_rule_matcher.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynUtils/test_chem_utils.py` & `synrbl-0.0.2/Test/SynUtils/test_chem_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynUtils/test_functional_group_utils.py` & `synrbl-0.0.2/Test/SynUtils/test_functional_group_utils.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/Test/SynVis/test_reaction_visualizer.py` & `synrbl-0.0.2/Test/SynVis/test_reaction_visualizer.py`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/LICENSE` & `synrbl-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/README.md` & `synrbl-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `synrbl-0.0.1/pyproject.toml` & `synrbl-0.0.2/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "synrbl"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
 	{name="Tieu Long Phan", email="long.tieu_phan@uni-leipzig.de"}, 
 	{name="Klaus Weinbauer", email="klaus@bioinf.uni-leipzig.de"}
 	]
 description = "Synthesis Rebalancing Framework for Computational Chemistry"
 readme = "README.md"
 requires-python = ">=3.11"
```

### Comparing `synrbl-0.0.1/PKG-INFO` & `synrbl-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: synrbl
-Version: 0.0.1
+Version: 0.0.2
 Summary: Synthesis Rebalancing Framework for Computational Chemistry
 Project-URL: homepage, https://github.com/TieuLongPhan/SynRBL
 Project-URL: source, https://github.com/TieuLongPhan/SynRBL
 Project-URL: issues, https://github.com/TieuLongPhan/SynRBL/issues
 Author-email: Tieu Long Phan <long.tieu_phan@uni-leipzig.de>, Klaus Weinbauer <klaus@bioinf.uni-leipzig.de>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
```

