# Comparing `tmp/relationalai-0.2.1.tar.gz` & `tmp/relationalai-0.2.2.tar.gz`

## Comparing `relationalai-0.2.1.tar` & `relationalai-0.2.2.tar`

### file list

```diff
@@ -1,360 +1,361 @@
--rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 relationalai-0.2.1/README.md
--rw-r--r--   0        0        0     1543 2020-02-02 00:00:00.000000 relationalai-0.2.1/.github/workflows/end-to-end.yml
--rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 relationalai-0.2.1/.github/workflows/publish-to-pypi.yml
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 relationalai-0.2.1/.github/workflows/ruff.yml
--rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/README.md
--rw-r--r--   0        0        0    17337 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/getting_started.md
--rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/_old/OLD_pyrel_quickstart.md
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/_old/metamodel.md
--rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/_old/python_dsl.md
--rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/_old/quickstart.md
--rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/README.md
--rw-r--r--   0        0        0    13703 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/cli/README.md
--rw-r--r--   0        0        0     7009 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/configuration/README.md
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Expression.md
--rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Property.md
--rw-r--r--   0        0        0     6050 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/README.md
--rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Context/README.md
--rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Context/enter__.md
--rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Context/exit__.md
--rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Context/iter__.md
--rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Context/model.md
--rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Context/results.md
--rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/ContextSelect/README.md
--rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/ContextSelect/add.md
--rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/ContextSelect/call__.md
--rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/ContextSelect/getattribute__.md
--rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Instance/README.md
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Instance/persist.md
--rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Instance/set.md
--rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Instance/unpersist.md
--rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/InstanceProperty/README.md
--rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/InstanceProperty/or_.md
--rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Model/README.md
--rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Model/Type.md
--rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Model/found.md
--rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Model/name.md
--rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Model/not_found.md
--rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Model/ordered_choice.md
--rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Model/query.md
--rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Model/read.md
--rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Model/rule.md
--rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Model/scope.md
--rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Model/union.md
--rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Producer/README.md
--rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Producer/add__.md
--rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Producer/enter__.md
--rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Producer/eq__.md
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Producer/exit__.md
--rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Producer/ge__.md
--rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Producer/getattribute__.md
--rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Producer/gt__.md
--rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Producer/le__.md
--rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Producer/lt__.md
--rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Producer/mul__.md
--rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Producer/ne__.md
--rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Producer/pow__.md
--rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Producer/radd__.md
--rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Producer/rmul__.md
--rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Producer/rpow__.md
--rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Producer/rsub__.md
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Producer/rtruediv__.md
--rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Producer/sub__.md
--rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Producer/truediv__.md
--rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Type/README.md
--rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Type/add.md
--rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Type/call__.md
--rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Type/model.md
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Type/name.md
--rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/Type/or__.md
--rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/clients/README.md
--rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/clients/snowflake/PrimaryKey.md
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/clients/snowflake/README.md
--rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/clients/snowflake/Snowflake.md
--rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md
--rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md
--rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md
--rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md
--rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/README.md
--rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/Vars.md
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/alias.md
--rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/aggregates/README.md
--rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/aggregates/avg.md
--rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/aggregates/count.md
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/aggregates/max.md
--rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/aggregates/min.md
--rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/aggregates/rank_asc.md
--rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/aggregates/rank_desc.md
--rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/aggregates/sum.md
--rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/README.md
--rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/README.md
--rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md
--rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md
--rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/degree.md
--rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/degree_centrality.md
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md
--rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/indegree.md
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/infomap.md
--rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md
--rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/label_propagation.md
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/louvain.md
--rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/outdegree.md
--rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/pagerank.md
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md
--rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Edges/README.md
--rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Edges/add.md
--rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Edges/extend.md
--rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Graph/README.md
--rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Graph/compute.md
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Graph/edges.md
--rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Graph/fetch.md
--rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Graph/id.md
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Graph/model.md
--rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Graph/nodes.md
--rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Graph/undirected.md
--rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Graph/visualize.md
--rw-r--r--   0        0        0    20679 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png
--rw-r--r--   0        0        0    15558 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png
--rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png
--rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Nodes/README.md
--rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Nodes/add.md
--rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/python/std/graphs/Nodes/extend.md
--rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/api_reference/sql/README.md
--rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/README.md
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/cdc.py
--rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/emit_playground.py
--rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/found.py
--rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/fraud.ipynb
--rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/fraud.py
--rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/graph_algos.py
--rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/load_raw.py
--rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/nested.py
--rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/or_types.py
--rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/remote_load_csv.py
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/requirements.txt
--rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/simple.py
--rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/simple_recursion.py
--rw-r--r--   0        0        0      722 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/simple_streamlit.py
--rw-r--r--   0        0        0     2383 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/solver.py
--rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/weighted_graph_algos.py
--rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/data/people.csv
--rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/data/transactions.csv
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/ev_penetration/ev_penetration.py
--rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/ev_penetration/ev_penetration_csv.py
--rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/ev_penetration/state_stats.csv
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/imdb/README.md
--rw-r--r--   0        0        0   787694 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/imdb/imdb.csv
--rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/imdb/imdb.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/rel/bar.rel
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/rel/foo.rel
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/rel/solver.rel
--rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/social-money-network/SF_pagerank.ipynb
--rw-r--r--   0        0        0  2419367 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/social-money-network/Simulation-and-SF-Upload.ipynb
--rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 relationalai-0.2.1/examples/social-money-network/snowflake_pagerank.py
--rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/.gitignore
--rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/README.md
--rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/index.html
--rw-r--r--   0        0        0   454881 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/package-lock.json
--rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/package.json
--rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/tsconfig.json
--rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/vite.config.ts
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/.storybook/main.ts
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/.storybook/preview-body.html
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/.storybook/preview-head.html
--rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/.storybook/preview.ts
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/App.tsx
--rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/app.styl
--rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/debugger_client.ts
--rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/index.css
--rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/index.tsx
--rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/logo.svg
--rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/util.styl
--rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/ws.ts
--rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/assets/favicon.ico
--rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Button.styl
--rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Button.tsx
--rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Field.stories.tsx
--rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Field.styl
--rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Field.tsx
--rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Modal.stories.tsx
--rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Modal.styl
--rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Modal.tsx
--rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Sidebar.styl
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Sidebar.tsx
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Tooltip.stories.tsx
--rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Tooltip.styl
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Tooltip.tsx
--rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx
--rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Schematic/ScopeProvider.tsx
--rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Schematic/index.stories.tsx
--rw-r--r--   0        0        0     4724 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Schematic/index.styl
--rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Schematic/index.tsx
--rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Schematic/nodes/ComputeNode.tsx
--rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Schematic/nodes/FilterNode.tsx
--rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx
--rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx
--rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx
--rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx
--rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Schematic/nodes/UnknownNode.tsx
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Schematic/nodes/base.styl
--rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Schematic/nodes/base.tsx
--rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/components/Schematic/nodes/index.tsx
--rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/fixtures/branch-improved.json
--rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/fixtures/branch.json
--rw-r--r--   0        0        0    67308 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/fixtures/fraud.json
--rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/fixtures/index.ts
--rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/fixtures/not_found.json
--rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/fixtures/simple.json
--rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/fixtures/union.json
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/types/json.d.ts
--rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/types/jsx.d.ts
--rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 relationalai-0.2.1/frontend/debugger/src/types/mech.d.ts
--rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/__init__.py
--rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/emit.py
--rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/exec.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/fixtures.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/patch.py
--rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/util.py
--rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/cli/__main__.py
--rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/cli/collect_failures.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/cli/collect_tests.py
--rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/cli/repro.py
--rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/cli/run_tests.py
--rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/cli/watch.py
--rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/gen/action.py
--rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/gen/context.py
--rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/gen/document.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/gen/error.py
--rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/gen/group_limited.py
--rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/gen/ir.py
--rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/gen/scope.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/gen/staged.py
--rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/gen/task.py
--rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/gen/test.py
--rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/harness/database.py
--rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/harness/vendor_types.py
--rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/validate/diff.py
--rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/validate/errors.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/validate/mapping.py
--rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/gentest/validate/roundtrip.py
--rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/__init__.py
--rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/compiler.py
--rw-r--r--   0        0        0     9991 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/debugging.py
--rw-r--r--   0        0        0    44676 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/dsl.py
--rw-r--r--   0        0        0    12279 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/errors.py
--rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/metagen.py
--rw-r--r--   0        0        0    27821 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/metamodel.py
--rw-r--r--   0        0        0    18690 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/rel.py
--rw-r--r--   0        0        0    20453 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/rel2.py
--rw-r--r--   0        0        0    12236 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/rel_emitter.py
--rw-r--r--   0        0        0     3440 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/rel_utils.py
--rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/analysis/mechanistic.py
--rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/analysis/whynot.py
--rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/clients/__init__.py
--rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/clients/azure.py
--rw-r--r--   0        0        0    10135 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/clients/client.py
--rw-r--r--   0        0        0    17646 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/clients/config.py
--rw-r--r--   0        0        0    32550 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/clients/snowflake.py
--rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/clients/test.py
--rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/clients/types.py
--rw-r--r--   0        0        0     7343 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/loaders/csv.py
--rw-r--r--   0        0        0     7130 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/loaders/loader.py
--rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/loaders/types.py
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/std/__init__.py
--rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/std/aggregates.py
--rw-r--r--   0        0        0    13684 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/std/graphs.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/tools/__init__.py
--rw-r--r--   0        0        0    50480 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/tools/cli.py
--rw-r--r--   0        0        0    10318 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/tools/cli_controls.py
--rw-r--r--   0        0        0     6804 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/tools/debugger.py
--rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/tools/debugger_server.py
--rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/tools/dev.py
--rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 relationalai-0.2.1/src/relationalai/tools/notes
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/__init__.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/conftest.py
--rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/README.md
--rw-r--r--   0        0        0     1546 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/conftest.py
--rw-r--r--   0        0        0     7974 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/test_graph_visualize.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/test_snapshots.py
--rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query0.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query1.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/bottom/query0.txt
--rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/cosine_similarity/query0.txt
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/eigenvector_centrality/query0.txt
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/first/query0.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/indegree/query0.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/indegree/query1.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/infomap/query0.txt
--rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/jaccard_similarity/query0.txt
--rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/jaccard_similarity/query1.txt
--rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/louvain/query0.txt
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query0.txt
--rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query1.txt
--rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt
--rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query3.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query4.txt
--rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query0.txt
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query1.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/outdegree/query0.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/outdegree/query1.txt
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/page_rank/query0.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query0.txt
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query1.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query2.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query3.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query0.txt
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query1.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/top/query0.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query0.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query1.txt
--rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query2.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query3.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query4.txt
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query5.txt
--rw-r--r--   0        0        0      379 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/test_cases/agg_ordering.py
--rw-r--r--   0        0        0      700 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/test_cases/bool.py
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/test_cases/bottom.py
--rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/test_cases/cosine_similarity.py
--rw-r--r--   0        0        0      772 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/test_cases/eigenvector_centrality.py
--rw-r--r--   0        0        0      651 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/test_cases/export.py
--rw-r--r--   0        0        0      406 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/test_cases/first.py
--rw-r--r--   0        0        0     1046 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/test_cases/indegree.py
--rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/test_cases/infomap.py
--rw-r--r--   0        0        0      963 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/test_cases/jaccard_similarity.py
--rw-r--r--   0        0        0      985 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/test_cases/louvain.py
--rw-r--r--   0        0        0     1447 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/test_cases/multi_valued.py
--rw-r--r--   0        0        0      837 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/test_cases/not_found.py
--rw-r--r--   0        0        0     1002 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/test_cases/outdegree.py
--rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/test_cases/page_rank.py
--rw-r--r--   0        0        0      647 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/test_cases/persist.py
--rw-r--r--   0        0        0      645 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/test_cases/smoke.py
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/test_cases/top.py
--rw-r--r--   0        0        0     1716 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/end2end/test_cases/weighted_graphs.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/execution/test_core.py
--rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/execution/test_examples.py
--rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/execution/basic/smoketest.py
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/execution/snapshots/test_core/test_basic/smoketest/query0.txt
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/execution/snapshots/test_examples/test_example/emit_playground/query0.txt
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/execution/snapshots/test_examples/test_example/found/query0.txt
--rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/execution/snapshots/test_examples/test_example/graph/query0.txt
--rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/execution/snapshots/test_examples/test_example/graph/query1.txt
--rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/execution/snapshots/test_examples/test_example/load_raw/query0.txt
--rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/execution/snapshots/test_examples/test_example/or_types/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/execution/snapshots/test_examples/test_example/simple/query0.txt
--rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/execution/snapshots/test_examples/test_example/simple_recursion/query0.txt
--rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/execution/snapshots/test_examples/test_example/simple_streamlit/query0.txt
--rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/execution/snapshots/test_examples/test_example/test/query0.txt
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/init-cli/__init__.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/init-cli/azure_basic.py
--rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/init-cli/common.py
--rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/roundtrip/test_document.py
--rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 relationalai-0.2.1/tests/roundtrip/test_task.py
--rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 relationalai-0.2.1/.gitignore
--rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 relationalai-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 relationalai-0.2.1/docs/pypi/README.md
--rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 relationalai-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     5378 2020-02-02 00:00:00.000000 relationalai-0.2.2/README.md
+-rw-r--r--   0        0        0     2394 2020-02-02 00:00:00.000000 relationalai-0.2.2/.github/actions/end-to-end/action.yml
+-rw-r--r--   0        0        0     2388 2020-02-02 00:00:00.000000 relationalai-0.2.2/.github/workflows/end-to-end.yml
+-rw-r--r--   0        0        0      582 2020-02-02 00:00:00.000000 relationalai-0.2.2/.github/workflows/publish-to-pypi.yml
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 relationalai-0.2.2/.github/workflows/ruff.yml
+-rw-r--r--   0        0        0      252 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/README.md
+-rw-r--r--   0        0        0    17337 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/getting_started.md
+-rw-r--r--   0        0        0     9875 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/_old/OLD_pyrel_quickstart.md
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/_old/metamodel.md
+-rw-r--r--   0        0        0     5935 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/_old/python_dsl.md
+-rw-r--r--   0        0        0     9371 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/_old/quickstart.md
+-rw-r--r--   0        0        0      220 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/README.md
+-rw-r--r--   0        0        0    13377 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/cli/README.md
+-rw-r--r--   0        0        0     7100 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/configuration/README.md
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Expression.md
+-rw-r--r--   0        0        0     1874 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Property.md
+-rw-r--r--   0        0        0     6050 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/README.md
+-rw-r--r--   0        0        0     2199 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Context/README.md
+-rw-r--r--   0        0        0     2214 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Context/enter__.md
+-rw-r--r--   0        0        0     1640 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Context/exit__.md
+-rw-r--r--   0        0        0      961 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Context/iter__.md
+-rw-r--r--   0        0        0      800 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Context/model.md
+-rw-r--r--   0        0        0     1834 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Context/results.md
+-rw-r--r--   0        0        0     3094 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/ContextSelect/README.md
+-rw-r--r--   0        0        0     3419 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/ContextSelect/add.md
+-rw-r--r--   0        0        0     1435 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/ContextSelect/call__.md
+-rw-r--r--   0        0        0     1847 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/ContextSelect/getattribute__.md
+-rw-r--r--   0        0        0     1656 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Instance/README.md
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Instance/persist.md
+-rw-r--r--   0        0        0     1508 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Instance/set.md
+-rw-r--r--   0        0        0     1132 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Instance/unpersist.md
+-rw-r--r--   0        0        0     1642 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/InstanceProperty/README.md
+-rw-r--r--   0        0        0     1414 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/InstanceProperty/or_.md
+-rw-r--r--   0        0        0     1258 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Model/README.md
+-rw-r--r--   0        0        0      600 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Model/Type.md
+-rw-r--r--   0        0        0     3427 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Model/found.md
+-rw-r--r--   0        0        0      316 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Model/name.md
+-rw-r--r--   0        0        0     1599 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Model/not_found.md
+-rw-r--r--   0        0        0     5008 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Model/ordered_choice.md
+-rw-r--r--   0        0        0     3040 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Model/query.md
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Model/read.md
+-rw-r--r--   0        0        0     2050 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Model/rule.md
+-rw-r--r--   0        0        0     2978 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Model/scope.md
+-rw-r--r--   0        0        0     3411 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Model/union.md
+-rw-r--r--   0        0        0     2400 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/README.md
+-rw-r--r--   0        0        0     1789 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/add__.md
+-rw-r--r--   0        0        0     2193 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/enter__.md
+-rw-r--r--   0        0        0     1418 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/eq__.md
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/exit__.md
+-rw-r--r--   0        0        0     1518 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/ge__.md
+-rw-r--r--   0        0        0     1395 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/getattribute__.md
+-rw-r--r--   0        0        0     1548 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/gt__.md
+-rw-r--r--   0        0        0     1517 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/le__.md
+-rw-r--r--   0        0        0     1488 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/lt__.md
+-rw-r--r--   0        0        0     1734 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/mul__.md
+-rw-r--r--   0        0        0     1446 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/ne__.md
+-rw-r--r--   0        0        0     1664 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/pow__.md
+-rw-r--r--   0        0        0      372 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/radd__.md
+-rw-r--r--   0        0        0      374 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/rmul__.md
+-rw-r--r--   0        0        0      404 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/rpow__.md
+-rw-r--r--   0        0        0      384 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/rsub__.md
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/rtruediv__.md
+-rw-r--r--   0        0        0     1823 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/sub__.md
+-rw-r--r--   0        0        0     1857 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Producer/truediv__.md
+-rw-r--r--   0        0        0     1004 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Type/README.md
+-rw-r--r--   0        0        0     1608 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Type/add.md
+-rw-r--r--   0        0        0     2561 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Type/call__.md
+-rw-r--r--   0        0        0      346 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Type/model.md
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Type/name.md
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/Type/or__.md
+-rw-r--r--   0        0        0      692 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/clients/README.md
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/clients/snowflake/PrimaryKey.md
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/clients/snowflake/README.md
+-rw-r--r--   0        0        0     2678 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/clients/snowflake/Snowflake.md
+-rw-r--r--   0        0        0     2588 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md
+-rw-r--r--   0        0        0     1936 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md
+-rw-r--r--   0        0        0      695 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md
+-rw-r--r--   0        0        0      743 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md
+-rw-r--r--   0        0        0     2428 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/README.md
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/Vars.md
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/alias.md
+-rw-r--r--   0        0        0      973 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/aggregates/README.md
+-rw-r--r--   0        0        0     3105 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/aggregates/avg.md
+-rw-r--r--   0        0        0     2994 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/aggregates/count.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/aggregates/max.md
+-rw-r--r--   0        0        0     2083 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/aggregates/min.md
+-rw-r--r--   0        0        0     3303 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/aggregates/rank_asc.md
+-rw-r--r--   0        0        0     3335 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/aggregates/rank_desc.md
+-rw-r--r--   0        0        0     3031 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/aggregates/sum.md
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/README.md
+-rw-r--r--   0        0        0     2228 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/README.md
+-rw-r--r--   0        0        0     1916 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md
+-rw-r--r--   0        0        0     2138 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md
+-rw-r--r--   0        0        0     2349 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/degree.md
+-rw-r--r--   0        0        0     1909 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/degree_centrality.md
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md
+-rw-r--r--   0        0        0     2344 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/indegree.md
+-rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/infomap.md
+-rw-r--r--   0        0        0     2140 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md
+-rw-r--r--   0        0        0     1886 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/label_propagation.md
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/louvain.md
+-rw-r--r--   0        0        0     2354 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/outdegree.md
+-rw-r--r--   0        0        0     2295 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/pagerank.md
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md
+-rw-r--r--   0        0        0     1407 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Edges/README.md
+-rw-r--r--   0        0        0     1760 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Edges/add.md
+-rw-r--r--   0        0        0     1388 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Edges/extend.md
+-rw-r--r--   0        0        0     1420 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/README.md
+-rw-r--r--   0        0        0     1177 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/compute.md
+-rw-r--r--   0        0        0      874 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/edges.md
+-rw-r--r--   0        0        0     1241 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/fetch.md
+-rw-r--r--   0        0        0      703 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/id.md
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/model.md
+-rw-r--r--   0        0        0      790 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/nodes.md
+-rw-r--r--   0        0        0     1020 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/undirected.md
+-rw-r--r--   0        0        0     4167 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/visualize.md
+-rw-r--r--   0        0        0    20679 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png
+-rw-r--r--   0        0        0    15558 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png
+-rw-r--r--   0        0        0    14921 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png
+-rw-r--r--   0        0        0     1326 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Nodes/README.md
+-rw-r--r--   0        0        0     1215 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Nodes/add.md
+-rw-r--r--   0        0        0     1218 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/python/std/graphs/Nodes/extend.md
+-rw-r--r--   0        0        0      238 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/api_reference/sql/README.md
+-rw-r--r--   0        0        0     1355 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/README.md
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/cdc.py
+-rw-r--r--   0        0        0      935 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/emit_playground.py
+-rw-r--r--   0        0        0      589 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/found.py
+-rw-r--r--   0        0        0     6699 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/fraud.ipynb
+-rw-r--r--   0        0        0     3028 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/fraud.py
+-rw-r--r--   0        0        0     1952 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/graph_algos.py
+-rw-r--r--   0        0        0      333 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/load_raw.py
+-rw-r--r--   0        0        0      559 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/nested.py
+-rw-r--r--   0        0        0      627 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/or_types.py
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/remote_load_csv.py
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/requirements.txt
+-rw-r--r--   0        0        0      481 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/simple.py
+-rw-r--r--   0        0        0      653 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/simple_recursion.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/simple_streamlit.py
+-rw-r--r--   0        0        0     2416 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/solver.py
+-rw-r--r--   0        0        0     1562 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/weighted_graph_algos.py
+-rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/data/people.csv
+-rw-r--r--   0        0        0    10518 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/data/transactions.csv
+-rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/ev_penetration/ev_penetration.py
+-rw-r--r--   0        0        0     1321 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/ev_penetration/ev_penetration_csv.py
+-rw-r--r--   0        0        0     1525 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/ev_penetration/state_stats.csv
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/imdb/README.md
+-rw-r--r--   0        0        0   787694 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/imdb/imdb.csv
+-rw-r--r--   0        0        0      721 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/imdb/imdb.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/rel/bar.rel
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/rel/foo.rel
+-rw-r--r--   0        0        0      728 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/rel/solver.rel
+-rw-r--r--   0        0        0     6174 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/social-money-network/SF_pagerank.ipynb
+-rw-r--r--   0        0        0  2419367 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/social-money-network/Simulation-and-SF-Upload.ipynb
+-rw-r--r--   0        0        0     2831 2020-02-02 00:00:00.000000 relationalai-0.2.2/examples/social-money-network/snowflake_pagerank.py
+-rw-r--r--   0        0        0       32 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/.gitignore
+-rw-r--r--   0        0        0      229 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/README.md
+-rw-r--r--   0        0        0      499 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/index.html
+-rw-r--r--   0        0        0   454881 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/package-lock.json
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/package.json
+-rw-r--r--   0        0        0      500 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/tsconfig.json
+-rw-r--r--   0        0        0      576 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/vite.config.ts
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/.storybook/main.ts
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/.storybook/preview-body.html
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/.storybook/preview-head.html
+-rw-r--r--   0        0        0      189 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/.storybook/preview.ts
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/App.tsx
+-rw-r--r--   0        0        0     2280 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/app.styl
+-rw-r--r--   0        0        0     5496 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/debugger_client.ts
+-rw-r--r--   0        0        0      366 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/index.css
+-rw-r--r--   0        0        0      393 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/index.tsx
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/logo.svg
+-rw-r--r--   0        0        0     2112 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/util.styl
+-rw-r--r--   0        0        0      162 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/ws.ts
+-rw-r--r--   0        0        0    15086 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/assets/favicon.ico
+-rw-r--r--   0        0        0      156 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Button.styl
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Button.tsx
+-rw-r--r--   0        0        0     1290 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Field.stories.tsx
+-rw-r--r--   0        0        0      910 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Field.styl
+-rw-r--r--   0        0        0     3561 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Field.tsx
+-rw-r--r--   0        0        0     1062 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Modal.stories.tsx
+-rw-r--r--   0        0        0      813 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Modal.styl
+-rw-r--r--   0        0        0     1489 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Modal.tsx
+-rw-r--r--   0        0        0     2061 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Sidebar.styl
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Sidebar.tsx
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Tooltip.stories.tsx
+-rw-r--r--   0        0        0     1275 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Tooltip.styl
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Tooltip.tsx
+-rw-r--r--   0        0        0      634 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx
+-rw-r--r--   0        0        0     3228 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/ScopeProvider.tsx
+-rw-r--r--   0        0        0     1144 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/index.stories.tsx
+-rw-r--r--   0        0        0     4724 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/index.styl
+-rw-r--r--   0        0        0     2294 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/index.tsx
+-rw-r--r--   0        0        0     1505 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/ComputeNode.tsx
+-rw-r--r--   0        0        0     1416 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/FilterNode.tsx
+-rw-r--r--   0        0        0     1262 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx
+-rw-r--r--   0        0        0      614 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx
+-rw-r--r--   0        0        0      624 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx
+-rw-r--r--   0        0        0     1743 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx
+-rw-r--r--   0        0        0      339 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/UnknownNode.tsx
+-rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/base.styl
+-rw-r--r--   0        0        0     5326 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/base.tsx
+-rw-r--r--   0        0        0     1402 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/index.tsx
+-rw-r--r--   0        0        0     4529 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/fixtures/branch-improved.json
+-rw-r--r--   0        0        0     5229 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/fixtures/branch.json
+-rw-r--r--   0        0        0    67308 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/fixtures/fraud.json
+-rw-r--r--   0        0        0      308 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/fixtures/index.ts
+-rw-r--r--   0        0        0     9536 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/fixtures/not_found.json
+-rw-r--r--   0        0        0     6685 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/fixtures/simple.json
+-rw-r--r--   0        0        0     6271 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/fixtures/union.json
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/types/json.d.ts
+-rw-r--r--   0        0        0      179 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/types/jsx.d.ts
+-rw-r--r--   0        0        0     2845 2020-02-02 00:00:00.000000 relationalai-0.2.2/frontend/debugger/src/types/mech.d.ts
+-rw-r--r--   0        0        0     3709 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/__init__.py
+-rw-r--r--   0        0        0    12329 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/emit.py
+-rw-r--r--   0        0        0     2598 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/exec.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/fixtures.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/patch.py
+-rw-r--r--   0        0        0     7629 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/util.py
+-rwxr-xr-x   0        0        0     3521 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/cli/__main__.py
+-rw-r--r--   0        0        0     1299 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/cli/collect_failures.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/cli/collect_tests.py
+-rw-r--r--   0        0        0     5707 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/cli/repro.py
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/cli/run_tests.py
+-rw-r--r--   0        0        0    15710 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/cli/watch.py
+-rw-r--r--   0        0        0     3232 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/gen/action.py
+-rw-r--r--   0        0        0     5461 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/gen/context.py
+-rw-r--r--   0        0        0     1610 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/gen/document.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/gen/error.py
+-rw-r--r--   0        0        0     6095 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/gen/group_limited.py
+-rw-r--r--   0        0        0     4662 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/gen/ir.py
+-rw-r--r--   0        0        0    17029 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/gen/scope.py
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/gen/staged.py
+-rw-r--r--   0        0        0     2888 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/gen/task.py
+-rw-r--r--   0        0        0     2204 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/gen/test.py
+-rw-r--r--   0        0        0     2863 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/harness/database.py
+-rw-r--r--   0        0        0      228 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/harness/vendor_types.py
+-rw-r--r--   0        0        0     1709 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/validate/diff.py
+-rw-r--r--   0        0        0     5588 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/validate/errors.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/validate/mapping.py
+-rw-r--r--   0        0        0     5426 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/gentest/validate/roundtrip.py
+-rw-r--r--   0        0        0     2191 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/__init__.py
+-rw-r--r--   0        0        0     6310 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/compiler.py
+-rw-r--r--   0        0        0     9991 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/debugging.py
+-rw-r--r--   0        0        0    44677 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/dsl.py
+-rw-r--r--   0        0        0    12279 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/errors.py
+-rw-r--r--   0        0        0    26752 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/metagen.py
+-rw-r--r--   0        0        0    27821 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/metamodel.py
+-rw-r--r--   0        0        0    18690 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/rel.py
+-rw-r--r--   0        0        0    20453 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/rel2.py
+-rw-r--r--   0        0        0    12998 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/rel_emitter.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/rel_utils.py
+-rw-r--r--   0        0        0     8570 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/analysis/mechanistic.py
+-rw-r--r--   0        0        0      914 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/analysis/whynot.py
+-rw-r--r--   0        0        0      114 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/clients/__init__.py
+-rw-r--r--   0        0        0     8909 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/clients/azure.py
+-rw-r--r--   0        0        0    10135 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/clients/client.py
+-rw-r--r--   0        0        0    17646 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/clients/config.py
+-rw-r--r--   0        0        0    32470 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/clients/snowflake.py
+-rw-r--r--   0        0        0     5526 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/clients/test.py
+-rw-r--r--   0        0        0     1089 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/clients/types.py
+-rw-r--r--   0        0        0     7366 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/loaders/csv.py
+-rw-r--r--   0        0        0     7140 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/loaders/loader.py
+-rw-r--r--   0        0        0      584 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/loaders/types.py
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/std/__init__.py
+-rw-r--r--   0        0        0     1648 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/std/aggregates.py
+-rw-r--r--   0        0        0    13750 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/std/graphs.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/tools/__init__.py
+-rw-r--r--   0        0        0    51381 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/tools/cli.py
+-rw-r--r--   0        0        0    10318 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/tools/cli_controls.py
+-rw-r--r--   0        0        0     6804 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/tools/debugger.py
+-rw-r--r--   0        0        0     2610 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/tools/debugger_server.py
+-rw-r--r--   0        0        0     9121 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/tools/dev.py
+-rw-r--r--   0        0        0      263 2020-02-02 00:00:00.000000 relationalai-0.2.2/src/relationalai/tools/notes
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/__init__.py
+-rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/conftest.py
+-rw-r--r--   0        0        0     4972 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/README.md
+-rw-r--r--   0        0        0     3301 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/conftest.py
+-rw-r--r--   0        0        0     8024 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_graph_visualize.py
+-rw-r--r--   0        0        0     1164 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_snapshots.py
+-rw-r--r--   0        0        0        9 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/agg_ordering/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query0.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/bool/query1.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/bottom/query0.txt
+-rw-r--r--   0        0        0       41 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/cosine_similarity/query0.txt
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/eigenvector_centrality/query0.txt
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/first/query0.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/indegree/query0.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/indegree/query1.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/infomap/query0.txt
+-rw-r--r--   0        0        0       33 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/jaccard_similarity/query0.txt
+-rw-r--r--   0        0        0      329 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/jaccard_similarity/query1.txt
+-rw-r--r--   0        0        0       53 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/louvain/query0.txt
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query0.txt
+-rw-r--r--   0        0        0      142 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query1.txt
+-rw-r--r--   0        0        0     1007 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt
+-rw-r--r--   0        0        0       25 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query3.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query4.txt
+-rw-r--r--   0        0        0       95 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query0.txt
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/not_found/query1.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/outdegree/query0.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/outdegree/query1.txt
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/page_rank/query0.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query0.txt
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query1.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query2.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/persist/query3.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query0.txt
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/smoke/query1.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/top/query0.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query0.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query1.txt
+-rw-r--r--   0        0        0       62 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query2.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query3.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query4.txt
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/weighted_graphs/query5.txt
+-rw-r--r--   0        0        0      385 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/agg_ordering.py
+-rw-r--r--   0        0        0      714 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/bool.py
+-rw-r--r--   0        0        0      526 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/bottom.py
+-rw-r--r--   0        0        0      847 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/cosine_similarity.py
+-rw-r--r--   0        0        0      771 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/eigenvector_centrality.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/export.py
+-rw-r--r--   0        0        0      431 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/first.py
+-rw-r--r--   0        0        0     1053 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/indegree.py
+-rw-r--r--   0        0        0      850 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/infomap.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/jaccard_similarity.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/louvain.py
+-rw-r--r--   0        0        0     1466 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/multi_valued.py
+-rw-r--r--   0        0        0      849 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/not_found.py
+-rw-r--r--   0        0        0     1015 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/outdegree.py
+-rw-r--r--   0        0        0      887 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/page_rank.py
+-rw-r--r--   0        0        0      661 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/persist.py
+-rw-r--r--   0        0        0      664 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/smoke.py
+-rw-r--r--   0        0        0      523 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/top.py
+-rw-r--r--   0        0        0     1720 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/end2end/test_cases/weighted_graphs.py
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/test_core.py
+-rw-r--r--   0        0        0      462 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/test_examples.py
+-rw-r--r--   0        0        0      437 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/basic/smoketest.py
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/snapshots/test_core/test_basic/smoketest/query0.txt
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/snapshots/test_examples/test_example/emit_playground/query0.txt
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/snapshots/test_examples/test_example/found/query0.txt
+-rw-r--r--   0        0        0      199 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/snapshots/test_examples/test_example/graph/query0.txt
+-rw-r--r--   0        0        0      127 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/snapshots/test_examples/test_example/graph/query1.txt
+-rw-r--r--   0        0        0       69 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/snapshots/test_examples/test_example/load_raw/query0.txt
+-rw-r--r--   0        0        0      147 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/snapshots/test_examples/test_example/or_types/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/snapshots/test_examples/test_example/simple/query0.txt
+-rw-r--r--   0        0        0      327 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/snapshots/test_examples/test_example/simple_recursion/query0.txt
+-rw-r--r--   0        0        0      107 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/snapshots/test_examples/test_example/simple_streamlit/query0.txt
+-rw-r--r--   0        0        0       68 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/execution/snapshots/test_examples/test_example/test/query0.txt
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/init-cli/__init__.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/init-cli/azure_basic.py
+-rw-r--r--   0        0        0     2352 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/init-cli/common.py
+-rw-r--r--   0        0        0     3097 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/roundtrip/test_document.py
+-rw-r--r--   0        0        0     2956 2020-02-02 00:00:00.000000 relationalai-0.2.2/tests/roundtrip/test_task.py
+-rw-r--r--   0        0        0      266 2020-02-02 00:00:00.000000 relationalai-0.2.2/.gitignore
+-rw-r--r--   0        0        0     1133 2020-02-02 00:00:00.000000 relationalai-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      205 2020-02-02 00:00:00.000000 relationalai-0.2.2/docs/pypi/README.md
+-rw-r--r--   0        0        0     1405 2020-02-02 00:00:00.000000 relationalai-0.2.2/PKG-INFO
```

### Comparing `relationalai-0.2.1/README.md` & `relationalai-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/.github/workflows/publish-to-pypi.yml` & `relationalai-0.2.2/.github/workflows/publish-to-pypi.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/.github/workflows/ruff.yml` & `relationalai-0.2.2/.github/workflows/ruff.yml`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/getting_started.md` & `relationalai-0.2.2/docs/getting_started.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/_old/OLD_pyrel_quickstart.md` & `relationalai-0.2.2/docs/_old/OLD_pyrel_quickstart.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/_old/metamodel.md` & `relationalai-0.2.2/docs/_old/metamodel.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/_old/python_dsl.md` & `relationalai-0.2.2/docs/_old/python_dsl.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/_old/quickstart.md` & `relationalai-0.2.2/docs/_old/quickstart.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/cli/README.md` & `relationalai-0.2.2/docs/api_reference/cli/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -207,79 +207,79 @@
 After you select the model to use and the file to upload, you are asked to provide a resource name,
 which defaults to the name of the file, and verify the file's schema:
 
 ```sh
 $ rai imports:snapshot
 
 ---------------------------------------------------
- 
-▰▰▰▰ Models fetched   
+
+▰▰▰▰ Models fetched
 
 ? Select a model: myModel
 
 ? Select a file: data/transactions.csv
 ? name: transactions.csv
-                                  
-  Field    Type     Ex.           
- ──────────────────────────────── 
-  id       String   TXN-00004052  
-  date     String   2023-10-12    
-  from     String   P-00013130    
-  to       String   P-00015417    
-  amount   Number   5214          
-                                  
+
+  Field    Type     Ex.
+ ────────────────────────────────
+  id       String   TXN-00004052
+  date     String   2023-10-12
+  from     String   P-00013130
+  to       String   P-00015417
+  amount   Number   5214
+
 ? Use this schema for transactions.csv: Yes
-▰▰▰▰ Snapshot for transactions.csv created   
+▰▰▰▰ Snapshot for transactions.csv created
 
 ---------------------------------------------------
 ```
 
 Use the `--source`, `--model`, and `--name` flags to load a file without interactively selecting the file, model, and resource name.
 You must still interactively confirm the schema of the file:
 
 ```sh
 $ rai imports:snapshot --source data/transactions.csv --model myModel --name transactions
 
 ---------------------------------------------------
-                                  
-  Field    Type     Ex.           
- ──────────────────────────────── 
-  id       String   TXN-00004052  
-  date     String   2023-10-12    
-  from     String   P-00013130    
-  to       String   P-00015417    
-  amount   Number   5214          
-                                  
+
+  Field    Type     Ex.
+ ────────────────────────────────
+  id       String   TXN-00004052
+  date     String   2023-10-12
+  from     String   P-00013130
+  to       String   P-00015417
+  amount   Number   5214
+
 ? Use this schema for transactions: Yes
-▰▰▰▰ Snapshot for transactions created   
+▰▰▰▰ Snapshot for transactions created
 
 ---------------------------------------------------
 ```
 
 To change the default schema, pass additional command-line arguments of the form `schema:<column_name>=<type>`.
 For example, to use `string` for the `amount` column, pass the arg `schema:amount=string`.
 As usual, you are asked to verify the schema before the snapshot is uploaded:
 
 ```sh
 $ rai imports:snapshot --source data/transactions.csv --model myModel --name transactions schema:amount=string
 
 ---------------------------------------------------
- 
+
 ? name: transactions.csv
-                                  
-  Field    Type     Ex.           
- ──────────────────────────────── 
-  id       String   TXN-00004052  
-  date     String   2023-10-12    
-  from     String   P-00013130    
-  to       String   P-00015417    
-  amount   String   5214          
-                                  
+
+  Field    Type     Ex.
+ ────────────────────────────────
+  id       String   TXN-00004052
+  date     String   2023-10-12
+  from     String   P-00013130
+  to       String   P-00015417
+  amount   String   5214
+
 ? Use this schema for transactions: Yes
-▰▰▰▰ Snapshot for transactions created   
+▰▰▰▰ Snapshot for transactions created
 
 ---------------------------------------------------
 ```
 
 You may provide multiple `schema:*` arguments to customize the schema as needed.
 
 Once you create the snapshot, you may add objects from the file to your model in
@@ -328,15 +328,15 @@
 
 #### Example
 
 Stream the data from the Snowflake table `my_database.my_schema.my_table`
 to the RelationalAI model `myModel`:
 
 ```sh
-rai imports:stream --object my_database.my_schema.my_table --model myModel
+rai imports:stream --source my_database.my_schema.my_table --model myModel
 ```
 
 Once the stream is finished setting up,
 data from the table may be accessed using the `relationalai` Python package:
 
 ```python
 import relationalai as rai
```

### Comparing `relationalai-0.2.1/docs/api_reference/configuration/README.md` & `relationalai-0.2.2/docs/api_reference/configuration/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -97,15 +97,15 @@
 
 ### The `RAI_PROFILE` environment variable
 
 If the `RAI_PROFILE` environment variable is set and the `profile` and `config` parameters of `rai.Model` are not supplied, the `relationalai` package will use `RAI_PROFILE` to determine which `raiconfig.toml` profile to use.
 
 ## Where do I find my credentials?
 
-The `rai init` command will help you fill in many of the values you need. However, there are a few values you will need to find on your own.
+The `rai init` command will help you fill in many of the values you need. However, there are a few values you will need to find separately.
 
 ### Snowflake
 
 Your Snowflake `user` and `password` are the same values you use to log in to the Snowflake web interface. To find your account value, log into `https://app.snowflake.com` and then look at the part of the URL after `https://app.snowflake.com` and replace the slash with a dash. For example, if your URL were `https://app.snowflake.com/plvoura/client_solutions`, the value you should use for `account` in your credentials is `plvoura-client_solutions`.
 
 ### Azure
 
@@ -146,14 +146,16 @@
 
 To use the configuration file from `~/.rai`, you can a save `raiconfig.toml` in your project directory that looks like this:
 
 ```toml
 active_profile = "field-team"
 ```
 
+> :bulb: You can change your active profile using the CLI subcommand `rai profile:switch`.
+
 The `relationalai` package will fill in the values from the `field-team` profile in `~/.rai/raiconfig.toml`.
 
 You can also override configuration keys from the parent configuration file by specifying them in the child configuration file. For example, if you wanted to use your `field-team` profile but with a different engine for a particular project, you could use a `raiconfig.toml` file like this:
 
 ```toml
 active_profile = "field-team"
 engine = "special_field_team_engine"
```

### Comparing `relationalai-0.2.1/docs/api_reference/python/Expression.md` & `relationalai-0.2.2/docs/api_reference/python/Expression.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Property.md` & `relationalai-0.2.2/docs/api_reference/python/Property.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/README.md` & `relationalai-0.2.2/docs/api_reference/python/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Context/README.md` & `relationalai-0.2.2/docs/api_reference/python/Context/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Context/enter__.md` & `relationalai-0.2.2/docs/api_reference/python/Context/enter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Context/exit__.md` & `relationalai-0.2.2/docs/api_reference/python/Context/exit__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Context/iter__.md` & `relationalai-0.2.2/docs/api_reference/python/Context/iter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Context/model.md` & `relationalai-0.2.2/docs/api_reference/python/Context/model.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Context/results.md` & `relationalai-0.2.2/docs/api_reference/python/Context/results.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/ContextSelect/README.md` & `relationalai-0.2.2/docs/api_reference/python/ContextSelect/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/ContextSelect/add.md` & `relationalai-0.2.2/docs/api_reference/python/ContextSelect/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/ContextSelect/call__.md` & `relationalai-0.2.2/docs/api_reference/python/ContextSelect/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/ContextSelect/getattribute__.md` & `relationalai-0.2.2/docs/api_reference/python/ContextSelect/getattribute__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Instance/README.md` & `relationalai-0.2.2/docs/api_reference/python/Instance/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Instance/persist.md` & `relationalai-0.2.2/docs/api_reference/python/Instance/persist.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Instance/set.md` & `relationalai-0.2.2/docs/api_reference/python/Instance/set.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Instance/unpersist.md` & `relationalai-0.2.2/docs/api_reference/python/Instance/unpersist.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/InstanceProperty/README.md` & `relationalai-0.2.2/docs/api_reference/python/InstanceProperty/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/InstanceProperty/or_.md` & `relationalai-0.2.2/docs/api_reference/python/InstanceProperty/or_.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Model/README.md` & `relationalai-0.2.2/docs/api_reference/python/Model/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Model/Type.md` & `relationalai-0.2.2/docs/api_reference/python/Model/Type.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Model/found.md` & `relationalai-0.2.2/docs/api_reference/python/Model/found.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Model/not_found.md` & `relationalai-0.2.2/docs/api_reference/python/Model/not_found.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Model/ordered_choice.md` & `relationalai-0.2.2/docs/api_reference/python/Model/ordered_choice.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Model/query.md` & `relationalai-0.2.2/docs/api_reference/python/Model/query.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Model/read.md` & `relationalai-0.2.2/docs/api_reference/python/Model/read.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Model/rule.md` & `relationalai-0.2.2/docs/api_reference/python/Model/rule.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Model/scope.md` & `relationalai-0.2.2/docs/api_reference/python/Model/scope.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Model/union.md` & `relationalai-0.2.2/docs/api_reference/python/Model/union.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Producer/README.md` & `relationalai-0.2.2/docs/api_reference/python/Producer/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Producer/add__.md` & `relationalai-0.2.2/docs/api_reference/python/Producer/add__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Producer/enter__.md` & `relationalai-0.2.2/docs/api_reference/python/Producer/enter__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Producer/eq__.md` & `relationalai-0.2.2/docs/api_reference/python/Producer/eq__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Producer/exit__.md` & `relationalai-0.2.2/docs/api_reference/python/Producer/exit__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Producer/ge__.md` & `relationalai-0.2.2/docs/api_reference/python/Producer/ge__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Producer/getattribute__.md` & `relationalai-0.2.2/docs/api_reference/python/Producer/getattribute__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Producer/gt__.md` & `relationalai-0.2.2/docs/api_reference/python/Producer/gt__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Producer/le__.md` & `relationalai-0.2.2/docs/api_reference/python/Producer/le__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Producer/lt__.md` & `relationalai-0.2.2/docs/api_reference/python/Producer/lt__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Producer/mul__.md` & `relationalai-0.2.2/docs/api_reference/python/Producer/mul__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Producer/ne__.md` & `relationalai-0.2.2/docs/api_reference/python/Producer/ne__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Producer/pow__.md` & `relationalai-0.2.2/docs/api_reference/python/Producer/pow__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Producer/sub__.md` & `relationalai-0.2.2/docs/api_reference/python/Producer/sub__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Producer/truediv__.md` & `relationalai-0.2.2/docs/api_reference/python/Producer/truediv__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Type/README.md` & `relationalai-0.2.2/docs/api_reference/python/Type/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Type/add.md` & `relationalai-0.2.2/docs/api_reference/python/Type/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Type/call__.md` & `relationalai-0.2.2/docs/api_reference/python/Type/call__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/Type/or__.md` & `relationalai-0.2.2/docs/api_reference/python/Type/or__.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/clients/README.md` & `relationalai-0.2.2/docs/api_reference/python/clients/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/clients/snowflake/PrimaryKey.md` & `relationalai-0.2.2/docs/api_reference/python/clients/snowflake/PrimaryKey.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/clients/snowflake/README.md` & `relationalai-0.2.2/docs/api_reference/python/clients/snowflake/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/clients/snowflake/Snowflake.md` & `relationalai-0.2.2/docs/api_reference/python/clients/snowflake/Snowflake.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md` & `relationalai-0.2.2/docs/api_reference/python/clients/snowflake/SnowflakeTable/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md` & `relationalai-0.2.2/docs/api_reference/python/clients/snowflake/SnowflakeTable/describe.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md` & `relationalai-0.2.2/docs/api_reference/python/clients/snowflake/SnowflakeTable/fqname.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md` & `relationalai-0.2.2/docs/api_reference/python/clients/snowflake/SnowflakeTable/namespace.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/README.md` & `relationalai-0.2.2/docs/api_reference/python/std/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/Vars.md` & `relationalai-0.2.2/docs/api_reference/python/std/Vars.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/alias.md` & `relationalai-0.2.2/docs/api_reference/python/std/alias.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/aggregates/README.md` & `relationalai-0.2.2/docs/api_reference/python/std/aggregates/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/aggregates/avg.md` & `relationalai-0.2.2/docs/api_reference/python/std/aggregates/avg.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/aggregates/count.md` & `relationalai-0.2.2/docs/api_reference/python/std/aggregates/count.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/aggregates/max.md` & `relationalai-0.2.2/docs/api_reference/python/std/aggregates/max.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/aggregates/min.md` & `relationalai-0.2.2/docs/api_reference/python/std/aggregates/min.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/aggregates/rank_asc.md` & `relationalai-0.2.2/docs/api_reference/python/std/aggregates/rank_asc.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/aggregates/rank_desc.md` & `relationalai-0.2.2/docs/api_reference/python/std/aggregates/rank_desc.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/aggregates/sum.md` & `relationalai-0.2.2/docs/api_reference/python/std/aggregates/sum.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/README.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/README.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/betweeness_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/cosine_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/degree.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/degree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/degree_centrality.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/degree_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/eigenvector_centrality.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/indegree.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/indegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/infomap.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/infomap.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/jaccard_similarity.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/label_propagation.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/label_propagation.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/louvain.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/louvain.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/outdegree.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/outdegree.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/pagerank.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/pagerank.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Compute/weakly_connected_component.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Edges/README.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Edges/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Edges/add.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Edges/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Edges/extend.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Edges/extend.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Graph/README.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Graph/compute.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/compute.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Graph/edges.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/edges.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Graph/fetch.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/fetch.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Graph/id.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/id.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Graph/model.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/model.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Graph/nodes.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/nodes.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Graph/undirected.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/undirected.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Graph/visualize.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/visualize.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/img/graph-viz-with-labels-and-colors.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/img/graph-viz.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Graph/img/simple-social-network.png`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Nodes/README.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Nodes/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Nodes/add.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Nodes/add.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/docs/api_reference/python/std/graphs/Nodes/extend.md` & `relationalai-0.2.2/docs/api_reference/python/std/graphs/Nodes/extend.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/examples/README.md` & `relationalai-0.2.2/examples/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/examples/cdc.py` & `relationalai-0.2.2/examples/cdc.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/examples/emit_playground.py` & `relationalai-0.2.2/examples/emit_playground.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/examples/found.py` & `relationalai-0.2.2/examples/found.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/examples/fraud.ipynb` & `relationalai-0.2.2/examples/fraud.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/examples/fraud.py` & `relationalai-0.2.2/examples/fraud.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/examples/graph_algos.py` & `relationalai-0.2.2/examples/graph_algos.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/examples/nested.py` & `relationalai-0.2.2/examples/nested.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/examples/or_types.py` & `relationalai-0.2.2/examples/or_types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/examples/remote_load_csv.py` & `relationalai-0.2.2/examples/remote_load_csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/examples/simple_recursion.py` & `relationalai-0.2.2/examples/simple_recursion.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/examples/simple_streamlit.py` & `relationalai-0.2.2/examples/simple_streamlit.py`

 * *Files 18% similar despite different names*

```diff
@@ -4,29 +4,30 @@
 import streamlit as st
 import pandas as pd
 
 model = rai.Model("MyCoolDatabase")
 Person = model.Type("Person")
 Adult = model.Type("Adult")
 
-Person.add(name="Joe", age=54)
-Person.add(name="Bob", age=40)
-Person.add(name="Jane", age=10)
+with model.rule():
+    Person.add(name="Joe", age=54)
+    Person.add(name="Bob", age=40)
+    Person.add(name="Jane", age=10)
 
 with model.rule():
     p = Person()
     p.age > 18
     p.set(Adult)
 
-st.header("Adults above a certain age")
 min_age = st.number_input("Age", min_value=0, max_value=100, value=18, step=1, key="age")
 
 with st.spinner("Running query..."):
     with model.query() as select:
         a = Adult()
         a.age > min_age
         z = select(a, a.name, a.age)
 
+st.header("Adults above a certain age", divider=True)
 st.table(pd.DataFrame(z.results, columns=["id", "name", "age"]))
```

### Comparing `relationalai-0.2.1/examples/solver.py` & `relationalai-0.2.2/examples/solver.py`

 * *Files 7% similar despite different names*

```diff
@@ -35,21 +35,21 @@
 pprint("Foo/Bar results", z)
 
 #--------------------------------------------------
 # Execute a raw string of rel
 #--------------------------------------------------
 
 res = model.exec_raw("""
-    def model2 = rel_primitive_solverapi_model[
-        :min, vars,  obj[vars:x, vars:y], cons[vars:x, vars:y]
-    ]
-    def solved2 = rel:solverapi:solve[model2, "HiGHS", {}]
-    def extracted2 = rel:solverapi:extract[model2, solved2]
-    def sol2 = extracted2:point
-    def output = extracted2:termination_status, sol2:x, sol2:y
+    def model2 { rel_primitive_solverapi_model[
+        :min, vars, obj[vars[:x], vars[:y]], cons[vars[:x], vars[:y]]
+    ] }
+    def solved2 { rel[:solverapi, :solve, model2, "HiGHS", {}] }
+    def extracted2 { rel[:solverapi, :extract, model2, solved2] }
+    def sol2 { extracted2[:point] }
+    def output {(extracted2[:termination_status], sol2[:x], sol2[:y])}
 """, raw_results=False)
 
 pprint("Exec raw results", res)
 
 #--------------------------------------------------
 # Query the solver relations
 #--------------------------------------------------
```

### Comparing `relationalai-0.2.1/examples/weighted_graph_algos.py` & `relationalai-0.2.2/examples/weighted_graph_algos.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/examples/data/people.csv` & `relationalai-0.2.2/examples/data/people.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/examples/data/transactions.csv` & `relationalai-0.2.2/examples/data/transactions.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/examples/ev_penetration/ev_penetration.py` & `relationalai-0.2.2/examples/ev_penetration/ev_penetration.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/examples/ev_penetration/ev_penetration_csv.py` & `relationalai-0.2.2/examples/ev_penetration/ev_penetration_csv.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/examples/ev_penetration/state_stats.csv` & `relationalai-0.2.2/examples/ev_penetration/state_stats.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/examples/imdb/README.md` & `relationalai-0.2.2/examples/imdb/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/examples/imdb/imdb.csv` & `relationalai-0.2.2/examples/imdb/imdb.csv`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/examples/imdb/imdb.py` & `relationalai-0.2.2/examples/imdb/imdb.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/examples/social-money-network/SF_pagerank.ipynb` & `relationalai-0.2.2/examples/social-money-network/SF_pagerank.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/examples/social-money-network/Simulation-and-SF-Upload.ipynb` & `relationalai-0.2.2/examples/social-money-network/Simulation-and-SF-Upload.ipynb`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/examples/social-money-network/snowflake_pagerank.py` & `relationalai-0.2.2/examples/social-money-network/snowflake_pagerank.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/package-lock.json` & `relationalai-0.2.2/frontend/debugger/package-lock.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/package.json` & `relationalai-0.2.2/frontend/debugger/package.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/vite.config.ts` & `relationalai-0.2.2/frontend/debugger/vite.config.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/App.tsx` & `relationalai-0.2.2/frontend/debugger/src/App.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/app.styl` & `relationalai-0.2.2/frontend/debugger/src/app.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/debugger_client.ts` & `relationalai-0.2.2/frontend/debugger/src/debugger_client.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/logo.svg` & `relationalai-0.2.2/frontend/debugger/src/logo.svg`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/util.styl` & `relationalai-0.2.2/frontend/debugger/src/util.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/assets/favicon.ico` & `relationalai-0.2.2/frontend/debugger/src/assets/favicon.ico`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Button.tsx` & `relationalai-0.2.2/frontend/debugger/src/components/Button.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Field.stories.tsx` & `relationalai-0.2.2/frontend/debugger/src/components/Field.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Field.styl` & `relationalai-0.2.2/frontend/debugger/src/components/Field.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Field.tsx` & `relationalai-0.2.2/frontend/debugger/src/components/Field.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Modal.stories.tsx` & `relationalai-0.2.2/frontend/debugger/src/components/Modal.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Modal.styl` & `relationalai-0.2.2/frontend/debugger/src/components/Modal.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Modal.tsx` & `relationalai-0.2.2/frontend/debugger/src/components/Modal.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Sidebar.styl` & `relationalai-0.2.2/frontend/debugger/src/components/Sidebar.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Sidebar.tsx` & `relationalai-0.2.2/frontend/debugger/src/components/Sidebar.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Tooltip.stories.tsx` & `relationalai-0.2.2/frontend/debugger/src/components/Tooltip.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Tooltip.styl` & `relationalai-0.2.2/frontend/debugger/src/components/Tooltip.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Tooltip.tsx` & `relationalai-0.2.2/frontend/debugger/src/components/Tooltip.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx` & `relationalai-0.2.2/frontend/debugger/src/components/Schematic/NodeIcon.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Schematic/ScopeProvider.tsx` & `relationalai-0.2.2/frontend/debugger/src/components/Schematic/ScopeProvider.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Schematic/index.stories.tsx` & `relationalai-0.2.2/frontend/debugger/src/components/Schematic/index.stories.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Schematic/index.styl` & `relationalai-0.2.2/frontend/debugger/src/components/Schematic/index.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Schematic/index.tsx` & `relationalai-0.2.2/frontend/debugger/src/components/Schematic/index.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx` & `relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/CallNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx` & `relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/EffectNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx` & `relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/GetNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx` & `relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/QuantifyNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx` & `relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/ReturnNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx` & `relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/SequenceNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx` & `relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/UnionNode.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Schematic/nodes/base.styl` & `relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/base.styl`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Schematic/nodes/base.tsx` & `relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/base.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/components/Schematic/nodes/index.tsx` & `relationalai-0.2.2/frontend/debugger/src/components/Schematic/nodes/index.tsx`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/fixtures/branch-improved.json` & `relationalai-0.2.2/frontend/debugger/src/fixtures/branch-improved.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/fixtures/branch.json` & `relationalai-0.2.2/frontend/debugger/src/fixtures/branch.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/fixtures/fraud.json` & `relationalai-0.2.2/frontend/debugger/src/fixtures/fraud.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/fixtures/not_found.json` & `relationalai-0.2.2/frontend/debugger/src/fixtures/not_found.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/fixtures/simple.json` & `relationalai-0.2.2/frontend/debugger/src/fixtures/simple.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/fixtures/union.json` & `relationalai-0.2.2/frontend/debugger/src/fixtures/union.json`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/frontend/debugger/src/types/mech.d.ts` & `relationalai-0.2.2/frontend/debugger/src/types/mech.d.ts`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/gentest/README.md` & `relationalai-0.2.2/src/gentest/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/gentest/emit.py` & `relationalai-0.2.2/src/gentest/emit.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/gentest/exec.py` & `relationalai-0.2.2/src/gentest/exec.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/gentest/fixtures.py` & `relationalai-0.2.2/src/gentest/fixtures.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/gentest/patch.py` & `relationalai-0.2.2/src/gentest/patch.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/gentest/util.py` & `relationalai-0.2.2/src/gentest/util.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/gentest/cli/__main__.py` & `relationalai-0.2.2/src/gentest/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/gentest/cli/collect_failures.py` & `relationalai-0.2.2/src/gentest/cli/collect_failures.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/gentest/cli/collect_tests.py` & `relationalai-0.2.2/src/gentest/cli/collect_tests.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/gentest/cli/repro.py` & `relationalai-0.2.2/src/gentest/cli/repro.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/gentest/cli/watch.py` & `relationalai-0.2.2/src/gentest/cli/watch.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/gentest/gen/action.py` & `relationalai-0.2.2/src/gentest/gen/action.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/gentest/gen/context.py` & `relationalai-0.2.2/src/gentest/gen/context.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/gentest/gen/document.py` & `relationalai-0.2.2/src/gentest/gen/document.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/gentest/gen/group_limited.py` & `relationalai-0.2.2/src/gentest/gen/group_limited.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/gentest/gen/ir.py` & `relationalai-0.2.2/src/gentest/gen/ir.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/gentest/gen/scope.py` & `relationalai-0.2.2/src/gentest/gen/scope.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/gentest/gen/task.py` & `relationalai-0.2.2/src/gentest/gen/task.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/gentest/gen/test.py` & `relationalai-0.2.2/src/gentest/gen/test.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/gentest/harness/database.py` & `relationalai-0.2.2/src/gentest/harness/database.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/gentest/validate/diff.py` & `relationalai-0.2.2/src/gentest/validate/diff.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/gentest/validate/errors.py` & `relationalai-0.2.2/src/gentest/validate/errors.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/gentest/validate/mapping.py` & `relationalai-0.2.2/src/gentest/validate/mapping.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/gentest/validate/roundtrip.py` & `relationalai-0.2.2/src/gentest/validate/roundtrip.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/relationalai/__init__.py` & `relationalai-0.2.2/src/relationalai/__init__.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/relationalai/compiler.py` & `relationalai-0.2.2/src/relationalai/compiler.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/relationalai/debugging.py` & `relationalai-0.2.2/src/relationalai/debugging.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/relationalai/dsl.py` & `relationalai-0.2.2/src/relationalai/dsl.py`

 * *Files 1% similar despite different names*

```diff
@@ -515,18 +515,18 @@
 
             prop_var = to_var(val)
             if is_collection(prop_var.value):
                 raise Exception("Can't set a property to a collection")
 
             if not prop_var.name:
                 prop_var.name = prop.name
-            if prop_var.value is None:
-                self._graph._check_property(prop, unknown_cardinality=True)
-            else:
+            if action_type.is_effect():
                 self._graph._check_property(prop)
+            else:
+                self._graph._check_property(prop, unknown_cardinality=True)
             self._action.append(prop, prop_var)
 
         #--------------------------------------------------
         # Entities
         #--------------------------------------------------
         self._var = self._action.entity
         if self._var.type == Builtins.Unknown and len(self._action.types):
```

### Comparing `relationalai-0.2.1/src/relationalai/errors.py` & `relationalai-0.2.2/src/relationalai/errors.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/relationalai/metagen.py` & `relationalai-0.2.2/src/relationalai/metagen.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/relationalai/metamodel.py` & `relationalai-0.2.2/src/relationalai/metamodel.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/relationalai/rel.py` & `relationalai-0.2.2/src/relationalai/rel.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/relationalai/rel2.py` & `relationalai-0.2.2/src/relationalai/rel2.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/relationalai/rel_emitter.py` & `relationalai-0.2.2/src/relationalai/rel_emitter.py`

 * *Files 5% similar despite different names*

```diff
@@ -171,18 +171,27 @@
                 return f"{args[2]} = {args[0]} {rel_name} {args[1]}"
         rel_name = self.sanitize(rel_name, True)
         if isinstance(root, Task) and root.isa(Builtins.Quantifier):
             # TODO: handle quantifier grouping
             args = args[1:]
             rel_name = rel_name.lower()
         if action.action == ActionType.Persist:
-            rel_name = f"insert:{rel_name}"
+            rel_name = f"insert[:{rel_name}]"
         elif action.action == ActionType.Unpersist:
-            rel_name = f"delete:{rel_name}"
-        final = f"{rel_name}({', '.join(args)})"
+            rel_name = f"delete[:{rel_name}]"
+        partial_appl = rel_name.find('[')
+        if partial_appl >= 0:
+            final_rel_name = rel_name[:partial_appl]
+            if len(args):
+                final_args = f"{rel_name[partial_appl+1:-1]}, {', '.join(args)}"
+            else:
+                final_args = ', '.join(args)
+            final = f"{final_rel_name}({final_args})"
+        else:
+            final = f"{rel_name}({', '.join(args)})"
         return final
 
     def to_return(self, action: Action, vars: set, body:List[str]):
         args = []
         for var in action.bindings.values():
             emitted = self.emit_var(var)
             vars.add(var)
@@ -196,28 +205,38 @@
 
     def to_set(self, action: Action, vars: set):
         vals:Any = [v for v in action.bindings.values()]
         mid_point = len(vals) // 2
         vars_str = ", ".join([self.emit_var(i) for i in vals[mid_point:]])
         rows = []
         for ix in range(len(vals[0].value)):
-            rows.append(",".join([self.emit_var(col.value[ix]) for col in vals[:mid_point]]))
+            row_vals = vals[:mid_point]
+            product_str = ",".join([self.emit_var(col.value[ix]) for col in row_vals])
+            if len(row_vals) > 1:
+                rows.append(f"({product_str})")
+            else:
+                rows.append(product_str)
         row_str = "; ".join(rows)
         return f"{{{row_str}}}({vars_str})"
 
     def to_inline_set(self, action: Action, vars: set):
         vals:Any = [v for v in action.bindings.values()]
         rows = []
         for ix in range(len(vals[0].value)):
-            rows.append(",".join([self.emit_var(col.value[ix]) for col in vals[:-1]]))
+            row_vals = vals[:-1]
+            product_str = ",".join([self.emit_var(col.value[ix]) for col in row_vals])
+            if len(row_vals) > 1:
+                rows.append(f"({product_str})")
+            else:
+                rows.append(product_str)
         row_str = "; ".join(rows)
         return (vals[-1], f"{{{row_str}}}")
 
     def to_inline_relation(self, task:Task, existing_vars=set()):
-        return f"( {self.query(task, True)} )"
+        return f"{{{self.query(task, True)}}}"
 
     #--------------------------------------------------
     # Query
     #--------------------------------------------------
 
     def query(self, task: Task, inline = False):
         supporting_rules = []
@@ -235,68 +254,68 @@
                     body.append(self.to_set(i, body_vars))
                 elif i.entity.value == Builtins.InlineRawData:
                     (v, data) = self.to_inline_set(i, body_vars)
                     self.mapped[v] = data
                     head_vars.add(v)
                 elif i.entity.value == Builtins.Install:
                     (item,) = i.bindings.values()
-                    supporting_rules.append(f"bound {self.emit_var(item)}")
+                    supporting_rules.append(f"declare {self.emit_var(item)}")
                     if isinstance(item.value, Type) and item.value.isa(Builtins.ValueType):
                         vtype = self.sanitize(item.value.name).capitalize() + "Type"
-                        supporting_rules.append(f"value type {vtype} = UInt128")
+                        supporting_rules.append(f"value type {vtype} {{ UInt128 }}")
                         for op in ["<", ">"]:
-                            supporting_rules.append(f"def ::std::common::({op})[x in {vtype}, y in {vtype}] = ^{vtype}(a, x) and ^{vtype}(b, y) and a {op} b from a, b")
+                            supporting_rules.append(f"def ::std::common::({op})[x in {vtype}, y in {vtype}]: exists((a, b) | ^{vtype}(a, x) and ^{vtype}(b, y) and a {op} b)")
                 else:
                     body.append(self.to_relation(i, body_vars, body))
             elif i.action == ActionType.Bind and i.entity.value == Builtins.Return:
                 head_rel = self.to_return(i, head_vars, body)
-                head = f"def {head_rel} =\n    "
+                head = f"def {head_rel}:\n    "
             elif i.action in [ActionType.Bind, ActionType.Persist, ActionType.Unpersist]:
                 if not inline:
                     head_rel = self.to_relation(i, head_vars, body, True)
                     annotations = set()
                     ent = i.entity.value
                     if isinstance(ent, Type) or isinstance(ent, Property):
                         for parent in ent.parents:
                             if parent.isa(Builtins.Annotation):
                                 annotations.add(parent.name.lower())
                     if annotations:
                         annotation_str = " ".join([f"@{a}" for a in annotations])
-                        head = f"{annotation_str}\ndef {head_rel} =\n    "
+                        head = f"{annotation_str}\ndef {head_rel}:\n    "
                     else:
-                        head = f"def {head_rel} =\n    "
+                        head = f"def {head_rel}:\n    "
                 else:
                     props = list(i.bindings.values())
                     head_vars.update(props)
-                    head = ",".join([self.emit_var(v) for v in props]) + ": "
+                    head = f"({', '.join([self.emit_var(v) for v in props])}): "
             elif i.action == ActionType.Construct:
                 inputs = [*i.bindings.values()]
                 input_str =', '.join([self.emit_var(v) for v in inputs[:-1]])
                 output = self.emit_var(inputs[-1])
                 body_vars.update(inputs)
                 body.append(f"{output} = ^{self.sanitize(i.entity.value.name).capitalize()}Type[{input_str}]")
             else:
                 raise Exception(f"TODO: Rel emit for action type {i.action}")
         body_str = " and\n    ".join(body)
         existing_vars = set()
         for vars in self.stack[:-1]:
             existing_vars.update(vars)
         from_vars = [self.emit_var(v) for v in (body_vars - head_vars - existing_vars) if v.value is None]
         if len(from_vars) and not inline:
-            body_str += f"\n    from {', '.join(from_vars)}"
+            body_str = f"exists(({', '.join(from_vars)}) |\n    {body_str})"
         if head and len(from_vars) and inline:
-            body_str += f" from {', '.join(from_vars)}"
+            body_str = f"exists(({', '.join(from_vars)}) | {body_str})"
 
 
         self.stack.pop()
 
         if not head and inline:
             return body_str
         elif not head:
-            head = f"def T{task.id}() =\n    "
+            head = f"def T{task.id}():\n    "
 
         support_str = ""
         if len(supporting_rules):
             support_str = "\n\n".join(supporting_rules) + "\n\n"
 
         if support_str and not head_vars and not body_str:
             return support_str
```

### Comparing `relationalai-0.2.1/src/relationalai/rel_utils.py` & `relationalai-0.2.2/src/relationalai/rel_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
 def emit_nested_relation(prefix: str, obj: dict|None = None, keys: Iterable[str]|None = None, raw = False) -> str:
     """Emit a set of defs encoding `obj` in GNF on `prefix`."""
     obj = obj or {}
     result = ""
     for k in keys or obj.keys():
         v = obj.get(k, None)
         if v is not None:
-            result += f"def {prefix}[{safe_symbol(k)}] = {emit_literal(v) if not raw else v}\n"
+            result += f"def {prefix}{safe_symbol(k)}]: {emit_literal(v) if not raw else v}\n"
     return result
 
 #-------------------------------------------------------------------------------
 # Result Handling
 #-------------------------------------------------------------------------------
 
 _known_problems: list[Any] = []
```

### Comparing `relationalai-0.2.1/src/relationalai/analysis/mechanistic.py` & `relationalai-0.2.2/src/relationalai/analysis/mechanistic.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/relationalai/analysis/whynot.py` & `relationalai-0.2.2/src/relationalai/analysis/whynot.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/relationalai/clients/azure.py` & `relationalai-0.2.2/src/relationalai/clients/azure.py`

 * *Files 2% similar despite different names*

```diff
@@ -95,16 +95,16 @@
     def create_models(self, database: str, engine: str, models:List[Tuple[str, str]]) -> List[Any]:
         lines = []
         for (name, code) in models:
             name = name.replace("\"", "\\\"")
             assert "\"\"\"\"\"\"\"" not in code, "Code literals must use fewer than 7 quotes."
 
             lines.append(textwrap.dedent(f"""
-            def delete:rel:catalog:model["{name}"] = rel:catalog:model["{name}"]
-            def insert:rel:catalog:model["{name}"] = raw\"\"\"\"\"\"\"{code}\"\"\"\"\"\"\"
+            def delete[:rel, :catalog, :model, "{name}"] = rel[:catalog, :model, "{name}"]
+            def insert[:rel, :catalog, :model, "{name}"] = raw\"\"\"\"\"\"\"{code}\"\"\"\"\"\"\"
             """))
         rel_code = "\n\n".join(lines)
         results = self.exec_raw(database, engine, rel_code, readonly=False)
         if results.problems:
             return results.problems
         return []
 
@@ -203,19 +203,18 @@
 # Graph
 #--------------------------------------------------
 
 def Graph(name, *, profile:str|None=None, config:Config, dry_run:bool=False):
     client = Client(Resources(profile, config), rel.Compiler(config), name, dry_run=dry_run)
     client.install("pyrel_base", dsl.build.raw_task("""
         @inline
-        def make_identity(x..., z) =
-            hash128({x...}, x..., u) and
-            hash_value_uint128_convert(u, z)
-            from u
+        def make_identity(x..., z):
+            exists((u) | hash128({x...}, x..., u) and
+            hash_value_uint128_convert(u, z))
 
         @inline
-        def pyrel_default[F, c](k..., v) =
+        def pyrel_default({F}, c, k..., v):
             F(k..., v) or (not F(k..., _) and v = c)
 
-        bound __resource
+        declare __resource
     """))
     return dsl.Graph(client, name)
```

### Comparing `relationalai-0.2.1/src/relationalai/clients/client.py` & `relationalai-0.2.2/src/relationalai/clients/client.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/relationalai/clients/config.py` & `relationalai-0.2.2/src/relationalai/clients/config.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/relationalai/clients/snowflake.py` & `relationalai-0.2.2/src/relationalai/clients/snowflake.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
     def create_engine(self, name:str, size:str, pool:str = ""):
         if not pool:
             raise ValueError("Pool is required")
         try:
             self._exec(f"call {APP_NAME}.api.create_engine('{name}', '{pool}', '{size}');")
         except Exception as e:
-            raise Exception("Failed to create engine") from e
+            raise Exception(f"Failed to create engine {name} using pool {pool} and size {size}") from e
 
     def delete_engine(self, name:str):
         self._exec(f"call {APP_NAME}.api.delete_engine('{name}');")
 
     def suspend_engine(self, name:str):
         raise Exception("Not implemented")
 
@@ -192,24 +192,24 @@
     def create_models(self, database: str, engine: str, models:List[Tuple[str, str]]) -> List[Any]:
         lines = []
         for (name, code) in models:
             name = name.replace("\"", "\\\"")
             assert "\"\"\"\"\"\"\"" not in code, "Code literals must use fewer than 7 quotes."
 
             lines.append(textwrap.dedent(f"""
-            def delete:rel:catalog:model["{name}"] = rel:catalog:model["{name}"]
-            def insert:rel:catalog:model["{name}"] = raw\"\"\"\"\"\"\"{code}\"\"\"\"\"\"\"
+            def delete[:rel, :catalog, :model, "{name}"] = rel[:catalog, :model, "{name}"]
+            def insert[:rel, :catalog, :model, "{name}"] = raw\"\"\"\"\"\"\"{code}\"\"\"\"\"\"\"
             """))
         rel_code = "\n\n".join(lines)
         self.exec_raw(database, engine, rel_code, readonly=False)
         # TODO: handle SPCS errors once they're figured out
         return []
 
     def delete_model(self, database:str, engine:str, name:str):
-        self.exec_raw(database, engine, f"def delete:rel:catalog:model[\"{name}\"] = rel:catalog:model[\"{name}\"]", readonly=False)
+        self.exec_raw(database, engine, f"def delete[:rel, :catalog, :model, \"{name}\"] = rel[:catalog, :model, \"{name}\"]", readonly=False)
 
     #--------------------------------------------------
     # Exports
     #--------------------------------------------------
 
     def list_exports(self, database: str, engine: str):
         return []
@@ -300,19 +300,14 @@
     def create_import_stream(self, source:ImportSource, model:str, rate = 1, options: dict|None = None):
         assert isinstance(source, ImportSourceTable), "Snowflake integration only supports loading from SF Tables right now. Try loading your data as a table via the snowflake interface first."
         object = source.fqn
 
         if object.lower() in [x["name"].lower() for x in self.list_imports(model)]:
             return
 
-        try:
-            self._exec(f"call {APP_NAME}.api.setup_cdc('{self.config.get('engine')}');")
-        except Exception:
-           pass
-
         info = self._exec(f"SHOW OBJECTS like %s in {source.database}.{source.schema}", [source.table])
         if not info:
             raise ValueError(f"Object {source.table} not found in {source.database}.{source.schema}")
         else:
             # (time, name, db_name, schema_name, kind, *rest)
             kind = info.fetchone()[4]
 
@@ -731,15 +726,15 @@
         if self._finalzed:
             return
 
         self._finalzed = True
         self._schema = self._parent._table_info[self._name]
         relation_name = self.fqname().replace(".", "_").lower()
         model:dsl.Graph = self._model
-        model.install_raw(f"bound {relation_name}")
+        model.install_raw(f"declare {relation_name}")
 
         with model.rule(dynamic=True):
             prop, id, val = std.Vars(3)
             if self._schema["pks"]:
                 getattr(getattr(std.rel, relation_name), self._schema["pks"][0].upper())(id, val)
             else:
                 getattr(std.rel, relation_name)(prop, id, val)
@@ -782,17 +777,16 @@
 # Graph
 #--------------------------------------------------
 
 def Graph(name, *, profile:str|None=None, config:Config, dry_run:bool=False):
     client = Client(Resources(profile, config), rel.Compiler(config), name, dry_run=dry_run)
     client.install("pyrel_base", dsl.build.raw_task("""
         @inline
-        def make_identity(x..., z) =
-            hash128({x...}, x..., u) and
-            hash_value_uint128_convert(u, z)
-            from u
+        def make_identity(x..., z):
+            exists((u) | hash128({x...}, x..., u) and
+            hash_value_uint128_convert(u, z))
 
         @inline
-        def pyrel_default[F, c](k..., v) =
+        def pyrel_default({F}, c, k..., v):
             F(k..., v) or (not F(k..., _) and v = c)
     """))
     return dsl.Graph(client, name)
```

### Comparing `relationalai-0.2.1/src/relationalai/clients/test.py` & `relationalai-0.2.2/src/relationalai/clients/test.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/relationalai/clients/types.py` & `relationalai-0.2.2/src/relationalai/clients/types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/relationalai/loaders/csv.py` & `relationalai-0.2.2/src/relationalai/loaders/csv.py`

 * *Files 4% similar despite different names*

```diff
@@ -90,47 +90,47 @@
     """Load CSV files and URLs in RAI DB using `load_csv`."""
     type = "csv"
 
     def load(self, provider: ResourceProvider, model: str, source: ImportSource, *, schema: Schema, syntax: Syntax):
         assert isinstance(source, ImportSourceFile), "CSV Loader can only load from files and URLs, not {type(source).__name__}"
 
         id = compute_str_hash(source.raw_path)
-        prefix = f"""def config:path = "{source.raw_path}" """
+        prefix = f"""def config[:path]: "{source.raw_path}" """
         inputs = None
 
         if not source.is_url():
             with open(source.raw_path, "r") as csv_file:
                 data = csv_file.read()
 
             id = compute_file_hash(source.raw_path)
-            prefix = "def config:data = data"
+            prefix = "def config[:data]: data"
             inputs = {"data": data}
 
         relation = sanitize(source.name)
         schema = schema or {}
 
         for key in ["delim", "quotechar", "escapechar"]:
             if syntax.get(key, None) and not isinstance(syntax[key], Char):
                 syntax[key] = Char(syntax[key])
 
         q = f"""
-        bound {relation}
-        def delete:{relation} = {relation}
-        def delete:__resource[k, "{relation}"] = __resource[k, "{relation}"]
+        declare {relation}
+        def delete[:{relation}]: {relation}
+        def delete[:__resource, k, "{relation}"]: __resource[k, "{relation}"]
 
         {prefix}
-        {emit_nested_relation("config:syntax", cast(dict, syntax), api._syntax_options)}
-        {emit_nested_relation("config:schema", {col: TYPE_TO_REL_SCHEMA.get(type, "string") for col, type in schema.items()})}
-        {emit_nested_relation("insert:__resource", {
+        {emit_nested_relation("config[:syntax, ", cast(dict, syntax), api._syntax_options)}
+        {emit_nested_relation("config[:schema, ", {col: TYPE_TO_REL_SCHEMA.get(type, "string") for col, type in schema.items()})}
+        {emit_nested_relation("insert[:__resource, ", {
         "id": (relation, id),
         "type": (relation, self.type),
         "name": (relation, source.name)
         })}
-        def insert:__resource:schema = "{relation}", config:schema
-        def insert:{relation} = load_csv[config]
+        def insert[:__resource, :schema]: ("{relation}", config[:schema])
+        def insert[:{relation}]: load_csv[config]
         """
         q = "\n".join(line.strip() for line in q.splitlines())
         print(q)
         res = provider.exec_raw(model, provider.get_default_engine_name(), q, readonly=False, inputs=inputs)
         assert_no_problems(res)
 
     SAMPLE_LINES_COUNT = 100
```

### Comparing `relationalai-0.2.1/src/relationalai/loaders/loader.py` & `relationalai-0.2.2/src/relationalai/loaders/loader.py`

 * *Files 2% similar despite different names*

```diff
@@ -140,29 +140,29 @@
 
     return Loader.get_loader_for_type(type)().load(provider, model, source, **metadata)
 
 def emit_delete_import(name: str) -> str:
     """Utility fn for emitting the rel to delete the specified import relation and all its metadata."""
     relation = sanitize(name)
     return f"""
-    bound {relation}
-    def delete:{relation} = {relation}
-    def delete:__resource[k] = "{name}", __resource[k, "{name}"]
+    declare {relation}
+    def delete[:{relation}]: {relation}
+    def delete[:__resource, k]: ("{name}", __resource[k, "{name}"])
     """
 
 #-------------------------------------------------------------------------------
 # Resource Management
 #-------------------------------------------------------------------------------
 
 available_resources:dict[str, dict] = {}
 
 def list_available_resources(provider: ResourceProvider, database: str, engine: str):
     res = provider.exec_raw(database, engine, """
-    bound __resource
-    def output = __resource
+    declare __resource
+    def output {{__resource}}
     """)
     assert_no_problems(res)
 
     available_resources = process_gnf_results(res.results, "name")
     return available_resources
 
 class MissingResourceError(Exception):
```

### Comparing `relationalai-0.2.1/src/relationalai/loaders/types.py` & `relationalai-0.2.2/src/relationalai/loaders/types.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/relationalai/std/aggregates.py` & `relationalai-0.2.2/src/relationalai/std/aggregates.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/relationalai/std/graphs.py` & `relationalai-0.2.2/src/relationalai/std/graphs.py`

 * *Files 5% similar despite different names*

```diff
@@ -209,20 +209,20 @@
         graph_type = "::graphlib::undirected_graph" if undirected else "::graphlib::directed_graph"
         if weighted:
             create_graph = f"""{graph_type}[{self.Edge._prop("weight")._name}]"""
         else:
             create_graph = f"{graph_type}[{self.Edge._type._name}]"
 
         self.model.install_raw(f"""
-        bound {self.Node._type.name}
-        bound {self.Edge._type._name}
-        {f"bound {self.Edge._prop('weight')._name}" if weighted else ""}
-        def {self._graph_ref()} = {create_graph}
+        declare {self.Node._type.name}
+        declare {self.Edge._type._name}
+        {f"declare {self.Edge._prop('weight')._name}" if weighted else ""}
+        def {self._graph_ref()} {{{create_graph}}}
         @inline
-        def {self._lib_ref()} = rel:graphlib[{self._graph_ref()}]
+        def {self._lib_ref()} {{rel[:graphlib, {self._graph_ref()}]}}
         """)
 
         # Add a rule that makes all nodes used in edges are also added to
         # the nodes relation
         with model.rule():
             a, b = dsl.Vars(2)
             self.Edge._type(a, b)
@@ -244,20 +244,21 @@
 
     #--------------------------------------------------
     # Fetch
     #--------------------------------------------------
 
     def fetch(self):
         code = []
-        code.append(f"def output:nodes(n) = {self.Node._type.name}(n)")
+        code.append(f"def output(:nodes, n): {self.Node._type.name}(n)")
         for prop in self.Node._type.properties:
-            code.append(f"def output:nodes:{prop.name.split('_')[-1]}(n, v) = {prop.name}(n, v)")
-        code.append(f"def output:edges(a,b) = {self.Edge._type._name}(a,b)")
+            scope = self.Node._scope
+            code.append(f"def output(:nodes, :{prop.name.removeprefix(scope)}, n, v): {prop.name}(n, v)")
+        code.append(f"def output(:edges, a,b): {self.Edge._type._name}(a,b)")
         for name, prop in self.Edge._props.items():
-            code.append(f"def output:edges:{name}(a,b,v) = {prop._name}(a,b,v)")
+            code.append(f"def output(:edges, :{name}, a, b, v): {prop._name}(a, b, v)")
 
         output = {"nodes": defaultdict(dict), "edges": defaultdict(dict)}
         results = self.model.exec_raw("\n".join(code), raw_results=True)
         for set_ in results.results:
             path = [v[1:] for v in set_["relationId"].split("/")[2:] if v[0] == ":"]
             if path[0] not in ["nodes", "edges"]:
                 continue
```

### Comparing `relationalai-0.2.1/src/relationalai/tools/cli.py` & `relationalai-0.2.2/src/relationalai/tools/cli.py`

 * *Files 1% similar despite different names*

```diff
@@ -545,14 +545,44 @@
             save_flow(cfg)
             gitignore_flow()
             rich.print(f"[yellow bold]✓ Saved partial raiconfig.toml ({os.path.abspath('raiconfig.toml')})")
 
         divider()
 
 #--------------------------------------------------
+# Profile switcher
+#--------------------------------------------------
+
+@cli.command(
+    name="profile:switch",
+    help="Switch to a different profile",
+)
+@click.option("--profile", help="Profile to switch to")
+def profile_switch(profile:str|None=None):
+    cfg = ensure_config()
+    profiles = list(cfg.get_profiles().keys())
+    divider()
+    if not profile:
+        if len(profiles) == 0:
+            rich.print("[yellow]No profiles found")
+            divider()
+            sys.exit(1)
+        profile = controls.fuzzy("Select a profile:", profiles)
+        divider()
+    else:
+        if profile not in profiles:
+            rich.print(f"[yellow]Profile '{profile}' not found")
+            divider()
+            sys.exit(1)
+    cfg.profile = profile
+    cfg.save()
+    rich.print(f"[green]✓ Switched to profile '{profile}'")
+    divider()
+
+#--------------------------------------------------
 # Explain config
 #--------------------------------------------------
 
 @cli.command(
     name="config:explain",
     help="Inspect config status",
 )
```

### Comparing `relationalai-0.2.1/src/relationalai/tools/cli_controls.py` & `relationalai-0.2.2/src/relationalai/tools/cli_controls.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/relationalai/tools/debugger.py` & `relationalai-0.2.2/src/relationalai/tools/debugger.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/relationalai/tools/debugger_server.py` & `relationalai-0.2.2/src/relationalai/tools/debugger_server.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/src/relationalai/tools/dev.py` & `relationalai-0.2.2/src/relationalai/tools/dev.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/tests/conftest.py` & `relationalai-0.2.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/tests/end2end/README.md` & `relationalai-0.2.2/tests/end2end/README.md`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/tests/end2end/test_graph_visualize.py` & `relationalai-0.2.2/tests/end2end/test_graph_visualize.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,58 +109,58 @@
         ),
         # Undirected graph with two data edges (but one graph edge), props, custom node and edge colors.
         # Shows property merge behavior for undirected graphs with multiple data edges for a single graph edge.
         # Compare to the directed graph case below.
         pytest.param(
             {
                 "adj_list": {1: [2]},
-                "node_props": {1: {'color': 'blue'}, 2: {'color': 'red'}},
+                "node_props": {1: {'node_color': 'blue'}, 2: {'node_color': 'red'}},
                 "edge_props": {
                     (1, 2): {'color': 'green'},
                     (2, 1): {'color': 'yellow'}
                 },
                 "undirected": True,
                 "style": {
-                    'nodes': {'color': lambda n: n['color']},
+                    'nodes': {'color': lambda n: n['node_color']},
                     'edges': {'color': lambda e: e['color']}
                 },
                 "kwargs": {},
             },
             {
                 'directed': False,
                 'nodes': {
-                    'jLWfdS5w49/Nqwx+mYthYw': {'metadata': {'color': 'red'}},
-                    'peH/vEX2TeRy3NL41/2Nag': {'metadata': {'color': 'blue'}},
+                    'jLWfdS5w49/Nqwx+mYthYw': {'metadata': {'node_color': 'red'}},
+                    'peH/vEX2TeRy3NL41/2Nag': {'metadata': {'node_color': 'blue'}},
                 },
                 'edges': [{'metadata': {'color': 'green'}, 'source': 'jLWfdS5w49/Nqwx+mYthYw', 'target': 'peH/vEX2TeRy3NL41/2Nag'}],
                 'metadata': DEFAULT_METADATA,
             },
             id="undirected_with_props_custom_style",
         ),
         # Directed graph with two data edges (and two graph edges), props, custom node and edge colors.
         pytest.param(
             {
                 "adj_list": {1: [2]},
-                "node_props": {1: {'color': 'blue'}, 2: {'color': 'red'}},
+                "node_props": {1: {'node_color': 'blue'}, 2: {'node_color': 'red'}},
                 "edge_props": {
                     (1, 2): {'color': 'green'},
                     (2, 1): {'color': 'yellow'}
                 },
                 "undirected": False,
                 "style": {
-                    'nodes': {'color': lambda n: n['color']},
+                    'nodes': {'color': lambda n: n['node_color']},
                     'edges': {'color': lambda e: e['color']}
                 },
                 "kwargs": {},
             },
             {
                 'directed': True,
                 'nodes': {
-                    'jLWfdS5w49/Nqwx+mYthYw': {'metadata': {'color': 'red'}},
-                    'peH/vEX2TeRy3NL41/2Nag': {'metadata': {'color': 'blue'}},
+                    'jLWfdS5w49/Nqwx+mYthYw': {'metadata': {'node_color': 'red'}},
+                    'peH/vEX2TeRy3NL41/2Nag': {'metadata': {'node_color': 'blue'}},
                 },
                 'edges': [
                     {'metadata': {'color': 'yellow'}, 'source': 'jLWfdS5w49/Nqwx+mYthYw', 'target': 'peH/vEX2TeRy3NL41/2Nag'},
                     {'metadata': {'color': 'green'}, 'source': 'peH/vEX2TeRy3NL41/2Nag', 'target': 'jLWfdS5w49/Nqwx+mYthYw'}
                 ],
                 'metadata': DEFAULT_METADATA,
             },
```

### Comparing `relationalai-0.2.1/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt` & `relationalai-0.2.2/tests/end2end/snapshots/test_snapshots/test_snapshots/multi_valued/query2.txt`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/tests/end2end/test_cases/bool.py` & `relationalai-0.2.2/tests/end2end/test_cases/smoke.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,34 +1,31 @@
-#pyright: reportUnusedExpression=false
+# pyright: reportUnusedExpression=false
 import relationalai as rai
 
-model = rai.Model("test_bool", config=globals().get("test_config"))
+
+model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
 Person = model.Type("Person")
 Adult = model.Type("Adult")
 
 with model.rule():
     Person.add(name="Joe", age=74)
     Person.add(name="Bob", age=40)
     Person.add(name="Jane", age=10)
 
 with model.rule():
     p = Person()
     p.age >= 18
-    p.set(Adult, cool=False)
+    p.set(Adult)
 
 with model.rule():
     p = Person()
-    p.age < 18
-    p.set(cool=True)
+    with p.age == 10:
+        p.set(coolness=100)
 
 with model.query() as select:
     a = Adult()
-    a.cool == False # noqa
-    z = select(a, a.name, a.age)
-
-print(z.results)
+    10 <= p.age <= 80
+    select(a, a.name, a.age)
 
 with model.query() as select:
-    p = Person(cool=True)
-    z = select(p, p.name)
-
-print(z.results)
+    p = Person()
+    select(p, p.coolness)
```

### Comparing `relationalai-0.2.1/tests/end2end/test_cases/cosine_similarity.py` & `relationalai-0.2.2/tests/end2end/test_cases/cosine_similarity.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,25 +1,24 @@
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-
 # Test case taken from:
 # https://github.com/RelationalAI/raicode/blob/8da410b949e8c47913a6faf4809234928fd8c238/test/RelLibraries/GraphAnalytics/graph_similarity_tests.jl#L238
 
-model = rai.Model("cosineSimilarityTest2", config=globals().get("test_config"))
+model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
 Node = model.Type("Node")
 
 edge_list = [(11, 12), (12, 13), (13, 13), (12, 14), (14, 13)]
 with model.rule(dynamic=True):
-    for (x, y) in edge_list:
+    for x, y in edge_list:
         node1 = Node.add(id=x)
         node2 = Node.add(id=y)
         node1.set(adjacent_to=node2)
 
 graph = Graph(model, undirected=True)
 graph.Edge.extend(Node.adjacent_to)
 
 with model.query() as select:
     node1 = Node(id=12)
     node2 = Node(id=14)
     similarity = graph.compute.cosine_similarity(node1, node2)
-    response = select(node1.id, node2.id, similarity)
+    response = select(node1.id, node2.id, similarity)
```

### Comparing `relationalai-0.2.1/tests/end2end/test_cases/eigenvector_centrality.py` & `relationalai-0.2.2/tests/end2end/test_cases/eigenvector_centrality.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-
 # Test case taken from:
 # https://github.com/RelationalAI/raicode/blob/8da410b949e8c47913a6faf4809234928fd8c238/test/RelLibraries/GraphAnalytics/centrality_tests.jl#L495
 
-model = rai.Model("eigenvectorCentralityTest2", config=globals()["test_config"])
+model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
 Node = model.Type("Node")
 
 edge_list = [(1, 2), (2, 3), (3, 4)]
 with model.rule(dynamic=True):
-    for (x, y) in edge_list:
+    for x, y in edge_list:
         node1 = Node.add(id=x)
         node2 = Node.add(id=y)
         node1.set(adjacent_to=node2)
 
 graph = Graph(model, undirected=True)
 graph.Edge.extend(Node.adjacent_to)
 
 with model.query() as select:
     node = Node()
     centrality = graph.compute.eigenvector_centrality(node)
-    response = select(node.id, centrality)
+    response = select(node.id, centrality)
```

### Comparing `relationalai-0.2.1/tests/end2end/test_cases/export.py` & `relationalai-0.2.2/tests/end2end/test_cases/export.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 #pyright: reportUnusedExpression=false
 from typing import Tuple
 import relationalai as rai
 
 # Since exports aren't supported in Azure, we'll do this as a dry run
 # to test just the bytecode generation
-model = rai.Model("test_export", dry_run=True, config=globals().get("test_config"))
+model = rai.Model(name=globals().get("name", ""), config=globals().get("config"), dry_run=True)
+
 Person = model.Type("Person")
 Adult = model.Type("Adult")
 
 with model.rule():
     Person.add(name="Joe", age=74)
     Person.add(name="Bob", age=40)
     Person.add(name="Jane", age=10)
```

### Comparing `relationalai-0.2.1/tests/end2end/test_cases/indegree.py` & `relationalai-0.2.2/tests/end2end/test_cases/indegree.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-
 # Test case taken from:
 # https://github.com/RelationalAI/raicode/blob/8da410b949e8c47913a6faf4809234928fd8c238/test/RelLibraries/GraphAnalytics/graph_similarity_tests.jl#L238
 
-model = rai.Model("indegreeTest2", config=globals().get("test_config"))
+model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
 Node = model.Type("Node")
 
 edge_list = [(11, 12), (12, 13), (13, 13), (13, 14)]
 with model.rule(dynamic=True):
-    for (x, y) in edge_list:
+    for x, y in edge_list:
         node1 = Node.add(id=x)
         node2 = Node.add(id=y)
         node1.set(adjacent_to=node2)
 
 # Undirected case
 undirected_graph = Graph(model, undirected=True)
 undirected_graph.Edge.extend(Node.adjacent_to)
```

### Comparing `relationalai-0.2.1/tests/end2end/test_cases/infomap.py` & `relationalai-0.2.2/tests/end2end/test_cases/infomap.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
 
 # Test case taken from:
 # https://github.com/RelationalAI/raicode/blob/a4b86f395ea1f4bbc0add40b3764aa17c1272110/src/rel/graphlib-infomap.rel#L37
 
-model = rai.Model("infomapTest", config=globals()["test_config"])
+model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
 Node = model.Type("Node")
 
 edge_list = [
     (1, 2), (1, 3), (2, 3),  # The first three-clique.
     (4, 5), (4, 6), (5, 6),  # The second three-clique.
     (1, 3),  # The connection between the three-cliques.
 ]
```

### Comparing `relationalai-0.2.1/tests/end2end/test_cases/jaccard_similarity.py` & `relationalai-0.2.2/tests/end2end/test_cases/jaccard_similarity.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,20 +1,19 @@
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-
 # Test case taken from:
 # https://docs.relational.ai/preview/graph-analytics/reference/graph-measures?rai-search#jaccard_similarity
 
-model = rai.Model("jaccardSimilarityTest2", config=globals()["test_config"])
+model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
 Node = model.Type("Node")
 
 edge_list = [(11, 12), (12, 13), (13, 13), (12, 14), (14, 13)]
 with model.rule(dynamic=True):
-    for (x, y) in edge_list:
+    for x, y in edge_list:
         node1 = Node.add(id=x)
         node2 = Node.add(id=y)
         node1.set(adjacent_to=node2)
 
 graph = Graph(model, undirected=True)
 graph.Edge.extend(Node.adjacent_to)
```

### Comparing `relationalai-0.2.1/tests/end2end/test_cases/louvain.py` & `relationalai-0.2.2/tests/end2end/test_cases/louvain.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,24 +4,24 @@
 
 # Test case taken from:
 # https://github.com/RelationalAI/raicode/blob/8da410b949e8c47913a6faf4809234928fd8c238/test/RelLibraries/GraphAnalytics/graph_community_detection_louvain_tests.jl#L17
 # Note that the expected output here differs from the expected output in the Rel test.
 # This is because the Rel uses the integer IDs for the node IDs in the graph,
 # while PyRel uses the hash as the node ID.
 
-model = rai.Model("louvainTest2", config=globals().get("test_config"))
+model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
 Node = model.Type("Node")
 
 edge_list = [(10, 10), (20, 20), (30, 30), (40, 40), (50, 50)]
 with model.rule(dynamic=True):
-    for (x, y) in edge_list:
+    for x, y in edge_list:
         node1 = Node.add(id=x)
         node2 = Node.add(id=y)
         node1.set(adjacent_to=node2)
 
 graph = Graph(model)
 graph.Edge.extend(Node.adjacent_to)
 
 with model.query() as select:
     node = Node()
     community = graph.compute.louvain(node)
-    response = select(node.id, community)
+    response = select(node.id, community)
```

### Comparing `relationalai-0.2.1/tests/end2end/test_cases/multi_valued.py` & `relationalai-0.2.2/tests/end2end/test_cases/multi_valued.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 #pyright: reportUnusedExpression=false
 import relationalai as rai
 
-model = rai.Model("test_collections", config=globals().get("test_config"))
+model = rai.Model(name=globals().get("name", "multi_valued"), config=globals().get("config"))
 model._config.set("compiler.use_multi_valued", True)
 
 Person = model.Type("Person")
 Adult = model.Type("Adult")
 
 Person.foos.has_many()
```

### Comparing `relationalai-0.2.1/tests/end2end/test_cases/not_found.py` & `relationalai-0.2.2/tests/end2end/test_cases/bool.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,34 +1,34 @@
+#pyright: reportUnusedExpression=false
 import relationalai as rai
 
-model = rai.Model("TestNotFound", config=globals().get("test_config"))
-Invited = model.Type("Invited")
-Invite = model.Type("Invite")
+model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
 Person = model.Type("Person")
+Adult = model.Type("Adult")
 
 with model.rule():
-    joe = Person.add(name="Joe", age=74)
-    bob = Person.add(name="Bob", age=40)
-    jane = Person.add(name="Jane", age=10)
-
-    joe.set(friend=jane).set(friend=bob)
-    jane.set(friend=joe)
-    bob.set(friend=jane)
-
-    Invited.add(person=joe)
+    Person.add(name="Joe", age=74)
+    Person.add(name="Bob", age=40)
+    Person.add(name="Jane", age=10)
 
 with model.rule():
     p = Person()
-    with model.not_found():
-        Invited(person=p)
+    p.age >= 18
+    p.set(Adult, cool=False)
 
-    Invite.add(person=p)
+with model.rule():
+    p = Person()
+    p.age < 18
+    p.set(cool=True)
 
 with model.query() as select:
-    p = Person()
-    p.friend.age > 10
-    with model.not_found():
-        p.friend.name == "Joe"
-    res = select(p, p.name, p.age, p.friend.name, p.friend.age)
+    a = Adult()
+    a.cool == False # noqa
+    z = select(a, a.name, a.age)
+
+print(z.results)
 
 with model.query() as select:
-    res = select(Invite().person.name)
+    p = Person(cool=True)
+    z = select(p, p.name)
+
+print(z.results)
```

### Comparing `relationalai-0.2.1/tests/end2end/test_cases/outdegree.py` & `relationalai-0.2.2/tests/end2end/test_cases/outdegree.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
+
 # Test case taken from:
 # https://github.com/RelationalAI/raicode/blob/8da410b949e8c47913a6faf4809234928fd8c238/src/rel/graph.rel#L537
 
-model = rai.Model("indegreeTest2", config=globals()["test_config"])
+model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
 Node = model.Type("Node")
 
 edge_list = [(11, 12), (12, 13), (13, 13), (12, 14)]
 with model.rule(dynamic=True):
-    for (x, y) in edge_list:
+    for x, y in edge_list:
         node1 = Node.add(id=x)
         node2 = Node.add(id=y)
         node1.set(adjacent_to=node2)
 
 # Undirected case
 undirected_graph = Graph(model, undirected=True)
 undirected_graph.Edge.extend(Node.adjacent_to)
```

### Comparing `relationalai-0.2.1/tests/end2end/test_cases/page_rank.py` & `relationalai-0.2.2/tests/end2end/test_cases/page_rank.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-model = rai.Model("socialNetwork2", config=globals()["test_config"])
+model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
 Person = model.Type("Person")
 
 # Add some people to the model and connect them with a `follows` property.
 with model.rule():
     alice = Person.add(name="Alice")
     bob = Person.add(name="Bob")
     carol = Person.add(name="Carol")
```

### Comparing `relationalai-0.2.1/tests/end2end/test_cases/smoke.py` & `relationalai-0.2.2/tests/end2end/test_cases/not_found.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,30 +1,35 @@
-#pyright: reportUnusedExpression=false
 import relationalai as rai
 
-model = rai.Model("test_smoke", config=globals()["test_config"])
+
+model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
+Invited = model.Type("Invited")
+Invite = model.Type("Invite")
 Person = model.Type("Person")
-Adult = model.Type("Adult")
 
 with model.rule():
-    Person.add(name="Joe", age=74)
-    Person.add(name="Bob", age=40)
-    Person.add(name="Jane", age=10)
+    joe = Person.add(name="Joe", age=74)
+    bob = Person.add(name="Bob", age=40)
+    jane = Person.add(name="Jane", age=10)
+
+    joe.set(friend=jane).set(friend=bob)
+    jane.set(friend=joe)
+    bob.set(friend=jane)
 
-with model.rule():
-    p = Person()
-    p.age >= 18
-    p.set(Adult)
+    Invited.add(person=joe)
 
 with model.rule():
     p = Person()
-    with p.age == 10:
-        p.set(coolness=100)
+    with model.not_found():
+        Invited(person=p)
 
-with model.query() as select:
-    a = Adult()
-    10 <= p.age <= 80
-    select(a, a.name, a.age)
+    Invite.add(person=p)
 
 with model.query() as select:
     p = Person()
-    select(p, p.coolness)
+    p.friend.age > 10
+    with model.not_found():
+        p.friend.name == "Joe"
+    res = select(p, p.name, p.age, p.friend.name, p.friend.age)
+
+with model.query() as select:
+    res = select(Invite().person.name)
```

### Comparing `relationalai-0.2.1/tests/end2end/test_cases/weighted_graphs.py` & `relationalai-0.2.2/tests/end2end/test_cases/weighted_graphs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import relationalai as rai
 from relationalai.std.graphs import Graph
 
-model = rai.Model("weightedGraphsTest2", config=globals().get("test_config"))
+model = rai.Model(name=globals().get("name", ""), config=globals().get("config"))
 
 
 def run_test(algo, ix: int, raw_edges):
     Node = model.Type(f"Node{ix}")
     graph = Graph(model, weighted=ix > 0)
 
     # Install graph data
```

### Comparing `relationalai-0.2.1/tests/init-cli/azure_basic.py` & `relationalai-0.2.2/tests/init-cli/azure_basic.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/tests/init-cli/common.py` & `relationalai-0.2.2/tests/init-cli/common.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/tests/roundtrip/test_document.py` & `relationalai-0.2.2/tests/roundtrip/test_document.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/tests/roundtrip/test_task.py` & `relationalai-0.2.2/tests/roundtrip/test_task.py`

 * *Files identical despite different names*

### Comparing `relationalai-0.2.1/pyproject.toml` & `relationalai-0.2.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = 'relationalai'
-version = '0.2.1'
+version = '0.2.2'
 description = 'RelationalAI Library and CLI'
 readme="docs/pypi/README.md"
 authors = [
     { name="RelationalAI", email="support@relational.ai" },
 ]
 requires-python = ">= 3.10"
 dependencies = [
```

### Comparing `relationalai-0.2.1/PKG-INFO` & `relationalai-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: relationalai
-Version: 0.2.1
+Version: 0.2.2
 Summary: RelationalAI Library and CLI
 Author-email: RelationalAI <support@relational.ai>
 Requires-Python: >=3.10
 Requires-Dist: bytecode
 Requires-Dist: click
 Requires-Dist: colorama
 Requires-Dist: gravis
```

