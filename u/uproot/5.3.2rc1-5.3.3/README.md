# Comparing `tmp/uproot-5.3.2rc1.tar.gz` & `tmp/uproot-5.3.3.tar.gz`

## Comparing `uproot-5.3.2rc1.tar` & `uproot-5.3.3.tar`

### file list

```diff
@@ -1,267 +1,274 @@
--rw-r--r--   0        0        0    15192 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/.all-contributorsrc
--rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/.readthedocs.yml
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/CITATION.cff
--rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/.github/dependabot.yml
--rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/.github/ISSUE_TEMPLATE/bug-report.md
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/.github/ISSUE_TEMPLATE/config.yml
--rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/.github/ISSUE_TEMPLATE/documentation.md
--rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/.github/ISSUE_TEMPLATE/feature-request.md
--rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/.github/workflows/build-distributions.yml
--rw-r--r--   0        0        0     2617 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/.github/workflows/build-test.yml
--rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/.github/workflows/deploy.yml
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/.github/workflows/semantic-pr-title.yml
--rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/.github/workflows/upload-nightly-wheels.yml
--rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/dev/example-objects.py
--rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/dev/make-models.py
--rw-r--r--   0        0        0    95009 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/docs-img/diagrams/abstraction-layers.png
--rw-r--r--   0        0        0    39940 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/docs-img/diagrams/abstraction-layers.svg
--rw-r--r--   0        0        0    49015 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/docs-img/diagrams/example-dask-graph.png
--rw-r--r--   0        0        0    70413 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/docs-img/diagrams/uproot-awkward-timeline.png
--rw-r--r--   0        0        0    28715 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/docs-img/diagrams/uproot-awkward-timeline.svg
--rw-r--r--   0        0        0     6794 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/docs-img/logo/logo-300px-white.png
--rw-r--r--   0        0        0     8489 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/docs-img/logo/logo-300px.png
--rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/docs-img/logo/logo-600px.png
--rw-r--r--   0        0        0     7695 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/docs-img/logo/logo.svg
--rw-r--r--   0        0        0   223219 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/docs-img/photos/switcheroo.jpg
--rw-r--r--   0        0        0    69268 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/docs-sphinx/basic.rst
--rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/docs-sphinx/conf.py
--rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/docs-sphinx/index.rst
--rw-r--r--   0        0        0     7841 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/docs-sphinx/make_changelog.py
--rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/docs-sphinx/prepare_docstrings.py
--rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/docs-sphinx/requirements.txt
--rw-r--r--   0        0        0    22209 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/docs-sphinx/uproot3-to-4.rst
--rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/docs-sphinx/_templates/breadcrumbs.html
--rw-r--r--   0        0        0     6925 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/__init__.py
--rw-r--r--   0        0        0     9180 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/_awkwardforth.py
--rw-r--r--   0        0        0    57409 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/_dask.py
--rw-r--r--   0        0        0    34627 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/_util.py
--rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/behavior.py
--rw-r--r--   0        0        0     7506 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/cache.py
--rw-r--r--   0        0        0    19349 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/compression.py
--rw-r--r--   0        0        0     4191 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/const.py
--rw-r--r--   0        0        0    60550 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/containers.py
--rw-r--r--   0        0        0    20781 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/deserialization.py
--rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/dynamic.py
--rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/exceptions.py
--rw-r--r--   0        0        0     8373 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/extras.py
--rw-r--r--   0        0        0    66238 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/model.py
--rw-r--r--   0        0        0     9625 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/pyroot.py
--rw-r--r--   0        0        0    97903 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/reading.py
--rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/serialization.py
--rw-r--r--   0        0        0    64332 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/streamers.py
--rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/version.py
--rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/behaviors/RooCurve.py
--rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/behaviors/RooHist.py
--rw-r--r--   0        0        0    10083 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/behaviors/TAxis.py
--rw-r--r--   0        0        0   130481 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/behaviors/TBranch.py
--rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/behaviors/TBranchElement.py
--rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/behaviors/TDatime.py
--rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/behaviors/TGraph.py
--rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/behaviors/TGraphAsymmErrors.py
--rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/behaviors/TGraphErrors.py
--rw-r--r--   0        0        0    12104 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/behaviors/TH1.py
--rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/behaviors/TH2.py
--rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/behaviors/TH2Poly.py
--rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/behaviors/TH3.py
--rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/behaviors/TParameter.py
--rw-r--r--   0        0        0    12480 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/behaviors/TProfile.py
--rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/behaviors/TProfile2D.py
--rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/behaviors/TProfile3D.py
--rw-r--r--   0        0        0     5407 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/behaviors/TTree.py
--rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/behaviors/__init__.py
--rw-r--r--   0        0        0     8305 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/interpretation/__init__.py
--rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/interpretation/grouped.py
--rw-r--r--   0        0        0    40596 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/interpretation/identify.py
--rw-r--r--   0        0        0    14929 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/interpretation/jagged.py
--rw-r--r--   0        0        0    38262 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/interpretation/library.py
--rw-r--r--   0        0        0    23102 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/interpretation/numerical.py
--rw-r--r--   0        0        0    37315 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/interpretation/objects.py
--rw-r--r--   0        0        0    18832 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/interpretation/strings.py
--rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/language/__init__.py
--rw-r--r--   0        0        0    16982 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/language/python.py
--rw-r--r--   0        0        0    30977 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/models/RNTuple.py
--rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/models/TArray.py
--rw-r--r--   0        0        0    25962 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/models/TAtt.py
--rw-r--r--   0        0        0    11306 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/models/TBasket.py
--rw-r--r--   0        0        0    37710 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/models/TBranch.py
--rw-r--r--   0        0        0     2721 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/models/TClonesArray.py
--rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/models/TDatime.py
--rw-r--r--   0        0        0    35986 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/models/TGraph.py
--rw-r--r--   0        0        0   215525 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/models/TH.py
--rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/models/THashList.py
--rw-r--r--   0        0        0    34985 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/models/TLeaf.py
--rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/models/TList.py
--rw-r--r--   0        0        0     2768 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/models/TMatrixT.py
--rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/models/TNamed.py
--rw-r--r--   0        0        0     5879 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/models/TObjArray.py
--rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/models/TObjString.py
--rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/models/TObject.py
--rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/models/TRef.py
--rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/models/TString.py
--rw-r--r--   0        0        0     7502 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/models/TTable.py
--rw-r--r--   0        0        0    47535 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/models/TTree.py
--rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/models/__init__.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/sink/__init__.py
--rw-r--r--   0        0        0     7279 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/sink/file.py
--rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/source/__init__.py
--rw-r--r--   0        0        0    17565 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/source/chunk.py
--rw-r--r--   0        0        0    24429 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/source/cursor.py
--rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/source/file.py
--rw-r--r--   0        0        0     8185 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/source/fsspec.py
--rw-r--r--   0        0        0    15114 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/source/futures.py
--rw-r--r--   0        0        0    28569 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/source/http.py
--rw-r--r--   0        0        0     4065 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/source/object.py
--rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/source/s3.py
--rw-r--r--   0        0        0    17188 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/source/xrootd.py
--rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/writing/__init__.py
--rw-r--r--   0        0        0    82513 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/writing/_cascade.py
--rw-r--r--   0        0        0    31821 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/writing/_cascadentuple.py
--rw-r--r--   0        0        0    62788 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/writing/_cascadetree.py
--rw-r--r--   0        0        0     6360 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/writing/_dask_write.py
--rw-r--r--   0        0        0    82208 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/writing/identify.py
--rw-r--r--   0        0        0    80878 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/src/uproot/writing/writable.py
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/__init__.py
--rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/conftest.py
--rw-r--r--   0        0        0    17012 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0001_source_class.py
--rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0006_notify_when_downloaded.py
--rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0007_single_chunk_interface.py
--rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0008_start_interpretation.py
--rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0009_nested_directories.py
--rw-r--r--   0        0        0    29196 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0010_start_streamers.py
--rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0011_generate_classes_from_streamers.py
--rw-r--r--   0        0        0     3530 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0013_rntuple_anchor.py
--rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0014_all_ttree_versions.py
--rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0016_interpretations.py
--rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0017_multi_basket_multi_branch_fetch.py
--rw-r--r--   0        0        0    33935 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0018_array_fetching_interface.py
--rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0022_number_of_branches.py
--rw-r--r--   0        0        0    13960 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0023_more_interpretations_1.py
--rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0023_ttree_versions.py
--rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0028_fallback_to_read_streamer.py
--rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0029_more_string_types.py
--rw-r--r--   0        0        0    23329 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0031_test_stl_containers.py
--rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0033_more_interpretations_2.py
--rw-r--r--   0        0        0    46572 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0034_generic_objects_in_ttrees.py
--rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0035_datatype_generality.py
--rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0038_memberwise_serialization.py
--rw-r--r--   0        0        0     8188 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0043_iterate_function.py
--rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0044_concatenate_function.py
--rw-r--r--   0        0        0    68981 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0046_histograms_bh_hist.py
--rw-r--r--   0        0        0     8605 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0053_parents_should_not_be_bases.py
--rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0058_detach_model_objects_from_files.py
--rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0066_fix_http_fallback_freeze.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0067_common_entry_offsets.py
--rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0081_dont_parse_colons.py
--rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0087_memberwise_splitting_not_implemented_messages.py
--rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0088_read_with_http.py
--rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0099_read_from_file_object.py
--rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0112_fix_pandas_with_cut.py
--rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0118_fix_name_fetch_again.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0123_atlas_issues.py
--rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0126_turn_unknown_emptyarrays_into_known_types.py
--rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0167_use_the_common_histogram_interface.py
--rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0172_allow_allocators_in_vector_typenames.py
--rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0173_empty_and_multiprocessing_bugs.py
--rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0182_complain_about_missing_files.py
--rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0194_fix_lost_cuts_in_iterate.py
--rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0220_contiguous_byte_ranges_in_http.py
--rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0228_read_TProfiles.py
--rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0240_read_TGraphAsymmErrors.py
--rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0278_specializations_for_TParameter.py
--rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0302_pickle.py
--rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0303_empty_jagged_array.py
--rw-r--r--   0        0        0    14234 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0320_start_working_on_ROOT_writing.py
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0322_writablefile_infrastructure.py
--rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0329_update_existing_root_files.py
--rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0335_empty_ttree_division_by_zero.py
--rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0341_manipulate_streamer_info.py
--rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0344_writabledirectory_can_read.py
--rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0345_bulk_copy_method.py
--rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0349_write_TObjString.py
--rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0350_read_RooCurve_RooHist.py
--rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0351_write_TList.py
--rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0352_write_THashList.py
--rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0384_move_behavior_of_and_fix_383.py
--rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0398_dimensions_in_leaflist.py
--rw-r--r--   0        0        0    26536 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0405_write_a_histogram.py
--rw-r--r--   0        0        0    11518 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0406_write_a_ttree.py
--rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0407_read_TDatime.py
--rw-r--r--   0        0        0    17062 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0412_write_multidimensional_numpy_to_ttree.py
--rw-r--r--   0        0        0    15363 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0414_write_jagged_arrays.py
--rw-r--r--   0        0        0    26104 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0416_writing_compressed_data.py
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0418_read_TTable.py
--rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0420_pyroot_uproot_interoperability.py
--rw-r--r--   0        0        0    17479 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0422_hist_integration.py
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0430_global_index_for_tuples_of_DataFrames.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0438_TClonesArray_is_not_AsGrouped.py
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0439_check_awkward_before_numpy.py
--rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0442_regular_TClonesArray.py
--rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0472_tstreamerinfo_for_ttree.py
--rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0475_remember_to_update_freesegments.py
--rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0484_manually_add_model_for_TMatrixTSym_double_.py
--rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0487_implement_asdtypeinplace.py
--rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0498_create_leaf_branch_in_extend.py
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0519_remove_memmap_copy.py
--rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0520_dynamic_classes_cant_be_abc_subclasses.py
--rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0569_fBits_is_4_bytes.py
--rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0576_unicode_in_names.py
--rw-r--r--   0        0        0    25906 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0578_dask_for_numpy.py
--rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0580_round_trip_for_no_flow_histograms.py
--rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0589_explicitly_interpret_RVec_type.py
--rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0603_dask_delayed_open.py
--rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0609_num_enteries_func.py
--rw-r--r--   0        0        0    18214 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0610_awkward_form.py
--rw-r--r--   0        0        0     1613 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0630_rntuple_basics.py
--rw-r--r--   0        0        0   132838 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0637_setup_tests_for_AwkwardForth.py
--rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0643_reading_vector_pair_TLorentzVector_int.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0651_implement_transformed_axis.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0652_dask_for_awkward.py
--rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0662_rntuple_stl_containers.py
--rw-r--r--   0        0        0    16170 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0692_fsspec_reading.py
--rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0692_fsspec_writing.py
--rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0700_dask_empty_arrays.py
--rw-r--r--   0        0        0     2612 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0705_rntuple_writing_metadata.py
--rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0750_avoid_empty_TBasket_issue.py
--rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0755_dask_awkward_column_projection.py
--rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0791_protect_uproot_project_columns_from_dask_node_names.py
--rw-r--r--   0        0        0     4885 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0798_DAOD_PHYSLITE.py
--rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0808_fix_awkward_form_for_AsStridedObjects.py
--rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0816_separate_AwkwardForth_machines_by_TBranch.py
--rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0832_ak_add_doc_should_also_add_to_typetracer.py
--rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0840_support_tleafG.py
--rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0841_fix_814.py
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0844_fix_delete_hist_from_root.py
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0852_fix_strided_interp_extra_offsets.py
--rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0870_writing_arrays_of_type_unknown_fix_822.py
--rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0876_uproot_dask_blind_steps.py
--rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0886_fix_awkward_form_breadcrumbs.py
--rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0910_fix_906_members_non_numerical_branches.py
--rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0911_fix_interp_array_non_numerical_objs_issue_880.py
--rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0912_fix_pandas_and_double_nested_vectors_issue_885.py
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0916_read_from_s3.py
--rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0927_dont_assume_uproot_in_global_scope_in_TPython_Eval.py
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0930_expressions_in_pandas.py
--rw-r--r--   0        0        0     7233 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0940_feat_add_TLeafC_string_support.py
--rw-r--r--   0        0        0     2118 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0962_RNTuple_update.py
--rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0965_inverted_axes_variances_hist_888.py
--rw-r--r--   0        0        0     7389 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_0976_path_object_split.py
--rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_1000-write-TProfiles.py
--rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_1043_const_std_string.py
--rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_1058_dask_awkward_report.py
--rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_1063_dask_distributed.py
--rw-r--r--   0        0        0      362 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_1070_pandas_dataframe_building_performance_fix.py
--rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_1085_dask_write.py
--rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_1102_any_locks_in_models_must_be_transient.py
--rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_1114_fix_attempt_to_concatenate_numpy_with_awkward.py
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_1120_check_decompression_executor_pass_for_dask.py
--rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_1127_fix_allow_colon_in_key_names.py
--rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_1146_split_ranges_for_large_files_over_http.py
--rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_1154_classof_using_relative_path.py
--rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/test_1160_std_string_in_TDirectory.py
--rw-r--r--   0        0        0   128147 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/tests/samples/h_dynamic.pkl
--rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/.gitignore
--rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/LICENSE
--rw-r--r--   0        0        0    28804 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/README.md
--rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/pyproject.toml
--rw-r--r--   0        0        0    31581 2020-02-02 00:00:00.000000 uproot-5.3.2rc1/PKG-INFO
+-rw-r--r--   0        0        0    15427 2020-02-02 00:00:00.000000 uproot-5.3.3/.all-contributorsrc
+-rw-r--r--   0        0        0     1127 2020-02-02 00:00:00.000000 uproot-5.3.3/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      212 2020-02-02 00:00:00.000000 uproot-5.3.3/.readthedocs.yml
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 uproot-5.3.3/CITATION.cff
+-rw-r--r--   0        0        0      218 2020-02-02 00:00:00.000000 uproot-5.3.3/.github/dependabot.yml
+-rw-r--r--   0        0        0      968 2020-02-02 00:00:00.000000 uproot-5.3.3/.github/ISSUE_TEMPLATE/bug-report.md
+-rw-r--r--   0        0        0      414 2020-02-02 00:00:00.000000 uproot-5.3.3/.github/ISSUE_TEMPLATE/config.yml
+-rw-r--r--   0        0        0      279 2020-02-02 00:00:00.000000 uproot-5.3.3/.github/ISSUE_TEMPLATE/documentation.md
+-rw-r--r--   0        0        0      606 2020-02-02 00:00:00.000000 uproot-5.3.3/.github/ISSUE_TEMPLATE/feature-request.md
+-rw-r--r--   0        0        0      720 2020-02-02 00:00:00.000000 uproot-5.3.3/.github/workflows/build-distributions.yml
+-rw-r--r--   0        0        0     3266 2020-02-02 00:00:00.000000 uproot-5.3.3/.github/workflows/build-test.yml
+-rw-r--r--   0        0        0      806 2020-02-02 00:00:00.000000 uproot-5.3.3/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 uproot-5.3.3/.github/workflows/semantic-pr-title.yml
+-rw-r--r--   0        0        0     1039 2020-02-02 00:00:00.000000 uproot-5.3.3/.github/workflows/upload-nightly-wheels.yml
+-rw-r--r--   0        0        0     4297 2020-02-02 00:00:00.000000 uproot-5.3.3/dev/example-objects.py
+-rw-r--r--   0        0        0     4133 2020-02-02 00:00:00.000000 uproot-5.3.3/dev/make-models.py
+-rw-r--r--   0        0        0    95009 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-img/diagrams/abstraction-layers.png
+-rw-r--r--   0        0        0    39940 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-img/diagrams/abstraction-layers.svg
+-rw-r--r--   0        0        0    49015 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-img/diagrams/example-dask-graph.png
+-rw-r--r--   0        0        0    70413 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-img/diagrams/uproot-awkward-timeline.png
+-rw-r--r--   0        0        0    28715 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-img/diagrams/uproot-awkward-timeline.svg
+-rw-r--r--   0        0        0     6794 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-img/logo/logo-300px-white.png
+-rw-r--r--   0        0        0     8489 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-img/logo/logo-300px.png
+-rw-r--r--   0        0        0    17651 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-img/logo/logo-600px.png
+-rw-r--r--   0        0        0     7695 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-img/logo/logo.svg
+-rw-r--r--   0        0        0   223219 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-img/photos/switcheroo.jpg
+-rw-r--r--   0        0        0    69268 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-sphinx/basic.rst
+-rw-r--r--   0        0        0     2219 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-sphinx/conf.py
+-rw-r--r--   0        0        0     5622 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-sphinx/index.rst
+-rw-r--r--   0        0        0     7841 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-sphinx/make_changelog.py
+-rw-r--r--   0        0        0    10456 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-sphinx/prepare_docstrings.py
+-rw-r--r--   0        0        0       31 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-sphinx/requirements.txt
+-rw-r--r--   0        0        0    22209 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-sphinx/uproot3-to-4.rst
+-rw-r--r--   0        0        0       97 2020-02-02 00:00:00.000000 uproot-5.3.3/docs-sphinx/_templates/breadcrumbs.html
+-rw-r--r--   0        0        0     6952 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/__init__.py
+-rw-r--r--   0        0        0     9180 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/_awkwardforth.py
+-rw-r--r--   0        0        0    57024 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/_dask.py
+-rw-r--r--   0        0        0    34679 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/_util.py
+-rw-r--r--   0        0        0     2999 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behavior.py
+-rw-r--r--   0        0        0     7506 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/cache.py
+-rw-r--r--   0        0        0    19158 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/compression.py
+-rw-r--r--   0        0        0     4215 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/const.py
+-rw-r--r--   0        0        0    64522 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/containers.py
+-rw-r--r--   0        0        0    20731 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/deserialization.py
+-rw-r--r--   0        0        0      896 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/dynamic.py
+-rw-r--r--   0        0        0     3019 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/exceptions.py
+-rw-r--r--   0        0        0     8297 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/extras.py
+-rw-r--r--   0        0        0    66033 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/model.py
+-rw-r--r--   0        0        0     9625 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/pyroot.py
+-rw-r--r--   0        0        0    98111 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/reading.py
+-rw-r--r--   0        0        0     3171 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/serialization.py
+-rw-r--r--   0        0        0    64326 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/streamers.py
+-rw-r--r--   0        0        0      411 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/version.py
+-rw-r--r--   0        0        0     5649 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/RooCurve.py
+-rw-r--r--   0        0        0     3614 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/RooHist.py
+-rw-r--r--   0        0        0    10083 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TAxis.py
+-rw-r--r--   0        0        0   129662 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TBranch.py
+-rw-r--r--   0        0        0      839 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TBranchElement.py
+-rw-r--r--   0        0        0      398 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TDatime.py
+-rw-r--r--   0        0        0     1358 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TGraph.py
+-rw-r--r--   0        0        0     3485 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TGraphAsymmErrors.py
+-rw-r--r--   0        0        0      306 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TGraphErrors.py
+-rw-r--r--   0        0        0    12104 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TH1.py
+-rw-r--r--   0        0        0     3511 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TH2.py
+-rw-r--r--   0        0        0      783 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TH2Poly.py
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TH3.py
+-rw-r--r--   0        0        0     1892 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TParameter.py
+-rw-r--r--   0        0        0    12480 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TProfile.py
+-rw-r--r--   0        0        0     3950 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TProfile2D.py
+-rw-r--r--   0        0        0     4412 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TProfile3D.py
+-rw-r--r--   0        0        0     5361 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/TTree.py
+-rw-r--r--   0        0        0     1078 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/behaviors/__init__.py
+-rw-r--r--   0        0        0     8305 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/interpretation/__init__.py
+-rw-r--r--   0        0        0     4461 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/interpretation/grouped.py
+-rw-r--r--   0        0        0    41203 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/interpretation/identify.py
+-rw-r--r--   0        0        0    14929 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/interpretation/jagged.py
+-rw-r--r--   0        0        0    38158 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/interpretation/library.py
+-rw-r--r--   0        0        0    22691 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/interpretation/numerical.py
+-rw-r--r--   0        0        0    37080 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/interpretation/objects.py
+-rw-r--r--   0        0        0    18832 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/interpretation/strings.py
+-rw-r--r--   0        0        0      655 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/language/__init__.py
+-rw-r--r--   0        0        0    16942 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/language/python.py
+-rw-r--r--   0        0        0    31247 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/RNTuple.py
+-rw-r--r--   0        0        0     4903 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TArray.py
+-rw-r--r--   0        0        0    25962 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TAtt.py
+-rw-r--r--   0        0        0    11268 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TBasket.py
+-rw-r--r--   0        0        0    37710 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TBranch.py
+-rw-r--r--   0        0        0     2673 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TClonesArray.py
+-rw-r--r--   0        0        0     2974 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TDatime.py
+-rw-r--r--   0        0        0    35842 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TGraph.py
+-rw-r--r--   0        0        0   215525 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TH.py
+-rw-r--r--   0        0        0     1749 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/THashList.py
+-rw-r--r--   0        0        0    34985 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TLeaf.py
+-rw-r--r--   0        0        0     3462 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TList.py
+-rw-r--r--   0        0        0     2720 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TMatrixT.py
+-rw-r--r--   0        0        0     3164 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TNamed.py
+-rw-r--r--   0        0        0     5879 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TObjArray.py
+-rw-r--r--   0        0        0     3948 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TObjString.py
+-rw-r--r--   0        0        0     4278 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TObject.py
+-rw-r--r--   0        0        0     8575 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TRef.py
+-rw-r--r--   0        0        0     3617 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TString.py
+-rw-r--r--   0        0        0     7502 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TTable.py
+-rw-r--r--   0        0        0     3989 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TTime.py
+-rw-r--r--   0        0        0    47535 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/TTree.py
+-rw-r--r--   0        0        0     1821 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/models/__init__.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/sink/__init__.py
+-rw-r--r--   0        0        0     7081 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/sink/file.py
+-rw-r--r--   0        0        0      907 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/source/__init__.py
+-rw-r--r--   0        0        0    17529 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/source/chunk.py
+-rw-r--r--   0        0        0    24376 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/source/cursor.py
+-rw-r--r--   0        0        0     8752 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/source/file.py
+-rw-r--r--   0        0        0     8185 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/source/fsspec.py
+-rw-r--r--   0        0        0    15114 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/source/futures.py
+-rw-r--r--   0        0        0    28139 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/source/http.py
+-rw-r--r--   0        0        0     4065 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/source/object.py
+-rw-r--r--   0        0        0     2851 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/source/s3.py
+-rw-r--r--   0        0        0    17188 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/source/xrootd.py
+-rw-r--r--   0        0        0     1287 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/writing/__init__.py
+-rw-r--r--   0        0        0    81089 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/writing/_cascade.py
+-rw-r--r--   0        0        0    31428 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/writing/_cascadentuple.py
+-rw-r--r--   0        0        0    62285 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/writing/_cascadetree.py
+-rw-r--r--   0        0        0     6360 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/writing/_dask_write.py
+-rw-r--r--   0        0        0    82120 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/writing/identify.py
+-rw-r--r--   0        0        0    80822 2020-02-02 00:00:00.000000 uproot-5.3.3/src/uproot/writing/writable.py
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/__init__.py
+-rw-r--r--   0        0        0     2686 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/conftest.py
+-rw-r--r--   0        0        0    17012 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0001_source_class.py
+-rw-r--r--   0        0        0     7141 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0006_notify_when_downloaded.py
+-rw-r--r--   0        0        0     5467 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0007_single_chunk_interface.py
+-rw-r--r--   0        0        0     1962 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0008_start_interpretation.py
+-rw-r--r--   0        0        0      906 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0009_nested_directories.py
+-rw-r--r--   0        0        0    29196 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0010_start_streamers.py
+-rw-r--r--   0        0        0     4207 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0011_generate_classes_from_streamers.py
+-rw-r--r--   0        0        0     3679 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0013_rntuple_anchor.py
+-rw-r--r--   0        0        0     9305 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0014_all_ttree_versions.py
+-rw-r--r--   0        0        0     3760 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0016_interpretations.py
+-rw-r--r--   0        0        0     9651 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0017_multi_basket_multi_branch_fetch.py
+-rw-r--r--   0        0        0    33935 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0018_array_fetching_interface.py
+-rw-r--r--   0        0        0     8813 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0022_number_of_branches.py
+-rw-r--r--   0        0        0    13960 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0023_more_interpretations_1.py
+-rw-r--r--   0        0        0    24165 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0023_ttree_versions.py
+-rw-r--r--   0        0        0      360 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0028_fallback_to_read_streamer.py
+-rw-r--r--   0        0        0     7606 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0029_more_string_types.py
+-rw-r--r--   0        0        0    23329 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0031_test_stl_containers.py
+-rw-r--r--   0        0        0     4534 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0033_more_interpretations_2.py
+-rw-r--r--   0        0        0    46572 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0034_generic_objects_in_ttrees.py
+-rw-r--r--   0        0        0     1766 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0035_datatype_generality.py
+-rw-r--r--   0        0        0     1220 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0038_memberwise_serialization.py
+-rw-r--r--   0        0        0     8188 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0043_iterate_function.py
+-rw-r--r--   0        0        0     1263 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0044_concatenate_function.py
+-rw-r--r--   0        0        0    68981 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0046_histograms_bh_hist.py
+-rw-r--r--   0        0        0     8605 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0053_parents_should_not_be_bases.py
+-rw-r--r--   0        0        0     2336 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0058_detach_model_objects_from_files.py
+-rw-r--r--   0        0        0      368 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0066_fix_http_fallback_freeze.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0067_common_entry_offsets.py
+-rw-r--r--   0        0        0     2682 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0081_dont_parse_colons.py
+-rw-r--r--   0        0        0      876 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0087_memberwise_splitting_not_implemented_messages.py
+-rw-r--r--   0        0        0      969 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0088_read_with_http.py
+-rw-r--r--   0        0        0      814 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0099_read_from_file_object.py
+-rw-r--r--   0        0        0      529 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0112_fix_pandas_with_cut.py
+-rw-r--r--   0        0        0     7914 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0118_fix_name_fetch_again.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0123_atlas_issues.py
+-rw-r--r--   0        0        0      409 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0126_turn_unknown_emptyarrays_into_known_types.py
+-rw-r--r--   0        0        0     6118 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0167_use_the_common_histogram_interface.py
+-rw-r--r--   0        0        0      442 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0172_allow_allocators_in_vector_typenames.py
+-rw-r--r--   0        0        0      995 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0173_empty_and_multiprocessing_bugs.py
+-rw-r--r--   0        0        0      746 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0182_complain_about_missing_files.py
+-rw-r--r--   0        0        0      402 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0194_fix_lost_cuts_in_iterate.py
+-rw-r--r--   0        0        0      648 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0220_contiguous_byte_ranges_in_http.py
+-rw-r--r--   0        0        0     1331 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0228_read_TProfiles.py
+-rw-r--r--   0        0        0     1986 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0240_read_TGraphAsymmErrors.py
+-rw-r--r--   0        0        0      607 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0278_specializations_for_TParameter.py
+-rw-r--r--   0        0        0     2343 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0302_pickle.py
+-rw-r--r--   0        0        0      719 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0303_empty_jagged_array.py
+-rw-r--r--   0        0        0    14234 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0320_start_working_on_ROOT_writing.py
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0322_writablefile_infrastructure.py
+-rw-r--r--   0        0        0      987 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0329_update_existing_root_files.py
+-rw-r--r--   0        0        0      336 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0335_empty_ttree_division_by_zero.py
+-rw-r--r--   0        0        0     7555 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0341_manipulate_streamer_info.py
+-rw-r--r--   0        0        0     2821 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0344_writabledirectory_can_read.py
+-rw-r--r--   0        0        0     1591 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0345_bulk_copy_method.py
+-rw-r--r--   0        0        0     2951 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0349_write_TObjString.py
+-rw-r--r--   0        0        0     6943 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0350_read_RooCurve_RooHist.py
+-rw-r--r--   0        0        0     1858 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0351_write_TList.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0352_write_THashList.py
+-rw-r--r--   0        0        0      696 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0384_move_behavior_of_and_fix_383.py
+-rw-r--r--   0        0        0     1527 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0398_dimensions_in_leaflist.py
+-rw-r--r--   0        0        0    26536 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0405_write_a_histogram.py
+-rw-r--r--   0        0        0    11518 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0406_write_a_ttree.py
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0407_read_TDatime.py
+-rw-r--r--   0        0        0    17062 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0412_write_multidimensional_numpy_to_ttree.py
+-rw-r--r--   0        0        0    15363 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0414_write_jagged_arrays.py
+-rw-r--r--   0        0        0    26104 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0416_writing_compressed_data.py
+-rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0418_read_TTable.py
+-rw-r--r--   0        0        0     3568 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0420_pyroot_uproot_interoperability.py
+-rw-r--r--   0        0        0    17479 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0422_hist_integration.py
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0430_global_index_for_tuples_of_DataFrames.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0438_TClonesArray_is_not_AsGrouped.py
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0439_check_awkward_before_numpy.py
+-rw-r--r--   0        0        0     1222 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0442_regular_TClonesArray.py
+-rw-r--r--   0        0        0      742 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0472_tstreamerinfo_for_ttree.py
+-rw-r--r--   0        0        0     1074 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0475_remember_to_update_freesegments.py
+-rw-r--r--   0        0        0      460 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0484_manually_add_model_for_TMatrixTSym_double_.py
+-rw-r--r--   0        0        0     1741 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0487_implement_asdtypeinplace.py
+-rw-r--r--   0        0        0     4527 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0498_create_leaf_branch_in_extend.py
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0519_remove_memmap_copy.py
+-rw-r--r--   0        0        0      458 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0520_dynamic_classes_cant_be_abc_subclasses.py
+-rw-r--r--   0        0        0      371 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0569_fBits_is_4_bytes.py
+-rw-r--r--   0        0        0      550 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0576_unicode_in_names.py
+-rw-r--r--   0        0        0    25906 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0578_dask_for_numpy.py
+-rw-r--r--   0        0        0     1231 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0580_round_trip_for_no_flow_histograms.py
+-rw-r--r--   0        0        0      747 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0589_explicitly_interpret_RVec_type.py
+-rw-r--r--   0        0        0     2930 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0603_dask_delayed_open.py
+-rw-r--r--   0        0        0     1839 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0609_num_enteries_func.py
+-rw-r--r--   0        0        0    18214 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0610_awkward_form.py
+-rw-r--r--   0        0        0     1535 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0630_rntuple_basics.py
+-rw-r--r--   0        0        0   132838 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0637_setup_tests_for_AwkwardForth.py
+-rw-r--r--   0        0        0      792 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0643_reading_vector_pair_TLorentzVector_int.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0651_implement_transformed_axis.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0652_dask_for_awkward.py
+-rw-r--r--   0        0        0     3379 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0662_rntuple_stl_containers.py
+-rw-r--r--   0        0        0    16181 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0692_fsspec_reading.py
+-rw-r--r--   0        0        0     6369 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0692_fsspec_writing.py
+-rw-r--r--   0        0        0     2447 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0700_dask_empty_arrays.py
+-rw-r--r--   0        0        0     2728 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0705_rntuple_writing_metadata.py
+-rw-r--r--   0        0        0      340 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0750_avoid_empty_TBasket_issue.py
+-rw-r--r--   0        0        0      660 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0755_dask_awkward_column_projection.py
+-rw-r--r--   0        0        0      546 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0791_protect_uproot_project_columns_from_dask_node_names.py
+-rw-r--r--   0        0        0     4885 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0798_DAOD_PHYSLITE.py
+-rw-r--r--   0        0        0     2365 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0808_fix_awkward_form_for_AsStridedObjects.py
+-rw-r--r--   0        0        0     1807 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0816_separate_AwkwardForth_machines_by_TBranch.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0832_ak_add_doc_should_also_add_to_typetracer.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0840_support_tleafG.py
+-rw-r--r--   0        0        0      947 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0841_fix_814.py
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0844_fix_delete_hist_from_root.py
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0852_fix_strided_interp_extra_offsets.py
+-rw-r--r--   0        0        0      494 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0870_writing_arrays_of_type_unknown_fix_822.py
+-rw-r--r--   0        0        0     2322 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0876_uproot_dask_blind_steps.py
+-rw-r--r--   0        0        0      294 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0886_fix_awkward_form_breadcrumbs.py
+-rw-r--r--   0        0        0      457 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0910_fix_906_members_non_numerical_branches.py
+-rw-r--r--   0        0        0      643 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0911_fix_interp_array_non_numerical_objs_issue_880.py
+-rw-r--r--   0        0        0     1943 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0912_fix_pandas_and_double_nested_vectors_issue_885.py
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0916_read_from_s3.py
+-rw-r--r--   0        0        0      344 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0927_dont_assume_uproot_in_global_scope_in_TPython_Eval.py
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0930_expressions_in_pandas.py
+-rw-r--r--   0        0        0     7233 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0940_feat_add_TLeafC_string_support.py
+-rw-r--r--   0        0        0     1979 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0962_RNTuple_update.py
+-rw-r--r--   0        0        0     1561 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0965_inverted_axes_variances_hist_888.py
+-rw-r--r--   0        0        0     7389 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_0976_path_object_split.py
+-rw-r--r--   0        0        0     2868 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1000-write-TProfiles.py
+-rw-r--r--   0        0        0      312 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1043_const_std_string.py
+-rw-r--r--   0        0        0     1573 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1058_dask_awkward_report.py
+-rw-r--r--   0        0        0      639 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1063_dask_distributed.py
+-rw-r--r--   0        0        0      394 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1070_pandas_dataframe_building_performance_fix.py
+-rw-r--r--   0        0        0     3527 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1085_dask_write.py
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1102_any_locks_in_models_must_be_transient.py
+-rw-r--r--   0        0        0      770 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1114_fix_attempt_to_concatenate_numpy_with_awkward.py
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1120_check_decompression_executor_pass_for_dask.py
+-rw-r--r--   0        0        0      767 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1127_fix_allow_colon_in_key_names.py
+-rw-r--r--   0        0        0      766 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1146_split_ranges_for_large_files_over_http.py
+-rw-r--r--   0        0        0     1073 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1154_classof_using_relative_path.py
+-rw-r--r--   0        0        0      517 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1160_std_string_in_TDirectory.py
+-rw-r--r--   0        0        0      776 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1180_read_free_floating_vector_issue_1179.py
+-rw-r--r--   0        0        0     2145 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1181_support_for_stl_list.py
+-rw-r--r--   0        0        0     1106 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1182_add_support_for_bitset.py
+-rw-r--r--   0        0        0      571 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1183_ttime_custom.py
+-rw-r--r--   0        0        0      631 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1186_dtype_might_raise_ValueError.py
+-rw-r--r--   0        0        0      644 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/test_1189_dask_failing_on_duplicate_keys.py
+-rw-r--r--   0        0        0   128147 2020-02-02 00:00:00.000000 uproot-5.3.3/tests/samples/h_dynamic.pkl
+-rw-r--r--   0        0        0     1949 2020-02-02 00:00:00.000000 uproot-5.3.3/.gitignore
+-rw-r--r--   0        0        0     1526 2020-02-02 00:00:00.000000 uproot-5.3.3/LICENSE
+-rw-r--r--   0        0        0    29133 2020-02-02 00:00:00.000000 uproot-5.3.3/README.md
+-rw-r--r--   0        0        0     3941 2020-02-02 00:00:00.000000 uproot-5.3.3/pyproject.toml
+-rw-r--r--   0        0        0    31907 2020-02-02 00:00:00.000000 uproot-5.3.3/PKG-INFO
```

### Comparing `uproot-5.3.2rc1/.all-contributorsrc` & `uproot-5.3.3/.all-contributorsrc`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9993169398907105%*

 * *Differences: {"'contributors'": "{insert: [(60, OrderedDict([('login', 'djw9497'), ('name', 'djw9497'), "*

 * *                   "('avatar_url', 'https://avatars.githubusercontent.com/u/51672890?v=4'), "*

 * *                   "('profile', 'https://github.com/djw9497'), ('contributions', ['code'])]))]}"}*

```diff
@@ -554,14 +554,23 @@
             "avatar_url": "https://avatars.githubusercontent.com/u/13764397?v=4",
             "contributions": [
                 "code"
             ],
             "login": "milesgranger",
             "name": "Miles",
             "profile": "https://github.com/milesgranger"
+        },
+        {
+            "avatar_url": "https://avatars.githubusercontent.com/u/51672890?v=4",
+            "contributions": [
+                "code"
+            ],
+            "login": "djw9497",
+            "name": "djw9497",
+            "profile": "https://github.com/djw9497"
         }
     ],
     "contributorsPerLine": 7,
     "files": [
         "README.md"
     ],
     "imageSize": 100,
```

### Comparing `uproot-5.3.2rc1/.pre-commit-config.yaml` & `uproot-5.3.3/.pre-commit-config.yaml`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,44 @@
 ci:
   autoupdate_commit_msg: 'chore: update pre-commit hooks'
   autofix_commit_msg: 'style: pre-commit fixes'
 
 repos:
   - repo: https://github.com/pre-commit/pre-commit-hooks
-    rev: v4.5.0
+    rev: v4.6.0
     hooks:
       - id: check-added-large-files
       - id: check-case-conflict
       - id: check-merge-conflict
       - id: check-symlinks
       - id: check-yaml
       - id: debug-statements
       - id: end-of-file-fixer
       - id: mixed-line-ending
       - id: requirements-txt-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/psf/black-pre-commit-mirror
-    rev: 24.2.0
+    rev: 24.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/astral-sh/ruff-pre-commit
-    rev: v0.2.2
+    rev: v0.3.5
     hooks:
       - id: ruff
         args: [--fix, --show-fixes]
 
 
   - repo: https://github.com/asottile/pyupgrade
-    rev: v3.15.1
+    rev: v3.15.2
     hooks:
       - id: pyupgrade
         args: [--py38-plus]
 
   - repo: https://github.com/macisamuele/language-formatters-pre-commit-hooks
-    rev: v2.12.0
+    rev: v2.13.0
     hooks:
       - id: pretty-format-toml
         args: [--autofix]
       - id: pretty-format-yaml
         args: [--autofix, --indent, '2', --offset, '2']
```

### Comparing `uproot-5.3.2rc1/CITATION.cff` & `uproot-5.3.3/CITATION.cff`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/.github/ISSUE_TEMPLATE/bug-report.md` & `uproot-5.3.3/.github/ISSUE_TEMPLATE/bug-report.md`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/.github/ISSUE_TEMPLATE/feature-request.md` & `uproot-5.3.3/.github/ISSUE_TEMPLATE/feature-request.md`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/.github/workflows/build-distributions.yml` & `uproot-5.3.3/.github/workflows/build-distributions.yml`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/.github/workflows/build-test.yml` & `uproot-5.3.3/.github/workflows/build-test.yml`

 * *Files 7% similar despite different names*

```diff
@@ -88,7 +88,31 @@
 
       - name: Pip install the package
         run: python -m pip install .[test,dev]
 
       - name: Run pytest
         run: |
           python -m pytest -vv tests --reruns 10 --reruns-delay 30 --only-rerun "(?i)http|ssl|timeout|expired|connection|socket"
+
+  numpy2-build:
+    strategy:
+      fail-fast: false
+      matrix:
+        platform: [windows-latest, ubuntu-latest, macos-latest]
+        python-version: ['3.11']
+
+    runs-on: ${{ matrix.platform }}
+    timeout-minutes: 30
+
+    steps:
+      - uses: actions/checkout@v4
+
+      - uses: actions/setup-python@v5
+        with:
+          python-version: ${{ matrix.python-version }}
+
+      - name: Pip install the package
+        run: python -m pip install 'numpy>=2.0.0b1' .[test]
+
+      - name: Run pytest
+        run: |
+          python -m pytest -vv tests --reruns 10 --reruns-delay 30 --only-rerun "(?i)http|ssl|timeout|expired|connection|socket"
```

### Comparing `uproot-5.3.2rc1/.github/workflows/deploy.yml` & `uproot-5.3.3/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/.github/workflows/upload-nightly-wheels.yml` & `uproot-5.3.3/.github/workflows/upload-nightly-wheels.yml`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/dev/example-objects.py` & `uproot-5.3.3/dev/example-objects.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/dev/make-models.py` & `uproot-5.3.3/dev/make-models.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/docs-img/diagrams/abstraction-layers.png` & `uproot-5.3.3/docs-img/diagrams/abstraction-layers.png`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/docs-img/diagrams/abstraction-layers.svg` & `uproot-5.3.3/docs-img/diagrams/abstraction-layers.svg`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/docs-img/diagrams/example-dask-graph.png` & `uproot-5.3.3/docs-img/diagrams/example-dask-graph.png`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/docs-img/diagrams/uproot-awkward-timeline.png` & `uproot-5.3.3/docs-img/diagrams/uproot-awkward-timeline.png`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/docs-img/diagrams/uproot-awkward-timeline.svg` & `uproot-5.3.3/docs-img/diagrams/uproot-awkward-timeline.svg`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/docs-img/logo/logo-300px-white.png` & `uproot-5.3.3/docs-img/logo/logo-300px-white.png`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/docs-img/logo/logo-300px.png` & `uproot-5.3.3/docs-img/logo/logo-300px.png`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/docs-img/logo/logo-600px.png` & `uproot-5.3.3/docs-img/logo/logo-600px.png`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/docs-img/logo/logo.svg` & `uproot-5.3.3/docs-img/logo/logo.svg`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/docs-img/photos/switcheroo.jpg` & `uproot-5.3.3/docs-img/photos/switcheroo.jpg`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/docs-sphinx/basic.rst` & `uproot-5.3.3/docs-sphinx/basic.rst`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/docs-sphinx/conf.py` & `uproot-5.3.3/docs-sphinx/conf.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/docs-sphinx/index.rst` & `uproot-5.3.3/docs-sphinx/index.rst`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/docs-sphinx/make_changelog.py` & `uproot-5.3.3/docs-sphinx/make_changelog.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/docs-sphinx/prepare_docstrings.py` & `uproot-5.3.3/docs-sphinx/prepare_docstrings.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/docs-sphinx/uproot3-to-4.rst` & `uproot-5.3.3/docs-sphinx/uproot3-to-4.rst`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/__init__.py` & `uproot-5.3.3/src/uproot/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -143,14 +143,15 @@
 import uproot.models.TBranch
 import uproot.models.TLeaf
 import uproot.models.TBasket
 import uproot.models.RNTuple
 import uproot.models.TH
 import uproot.models.TGraph
 import uproot.models.TMatrixT
+import uproot.models.TTime
 
 from uproot.models.TTree import num_entries
 
 from uproot.containers import STLVector
 from uproot.containers import STLSet
 from uproot.containers import STLMap
```

### Comparing `uproot-5.3.2rc1/src/uproot/_awkwardforth.py` & `uproot-5.3.3/src/uproot/_awkwardforth.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/_dask.py` & `uproot-5.3.3/src/uproot/_dask.py`

 * *Files 2% similar despite different names*

```diff
@@ -602,14 +602,15 @@
 
             new_keys = obj.keys(
                 recursive=recursive,
                 filter_name=filter_name,
                 filter_typename=filter_typename,
                 filter_branch=real_filter_branch,
                 full_paths=full_paths,
+                ignore_duplicates=True,
             )
 
             if common_keys is None:
                 common_keys = new_keys
             else:
                 new_keys = set(new_keys)
                 common_keys = [key for key in common_keys if key in new_keys]
@@ -623,35 +624,25 @@
             1, int(math.ceil(total_entries / (total_files * steps_per_file)))
         )
 
     if count == 0:
         raise ValueError(
             "allow_missing=True and no TTrees found in\n\n    {}".format(
                 "\n    ".join(
-                    "{"
-                    + "{}: {}".format(
-                        repr(f.file_path if isinstance(f, HasBranches) else f),
-                        repr(f.object_path if isinstance(f, HasBranches) else o),
-                    )
-                    + "}"
+                    f"{{{f.file_path if isinstance(f, HasBranches) else f!r}: {f.object_path if isinstance(f, HasBranches) else o!r}}}"
                     for f, o in files
                 )
             )
         )
 
     if len(common_keys) == 0 or not (all(is_self) or not any(is_self)):
         raise ValueError(
             "TTrees in\n\n    {}\n\nhave no TBranches in common".format(
                 "\n    ".join(
-                    "{"
-                    + "{}: {}".format(
-                        repr(f.file_path if isinstance(f, HasBranches) else f),
-                        repr(f.object_path if isinstance(f, HasBranches) else o),
-                    )
-                    + "}"
+                    f"{{{f.file_path if isinstance(f, HasBranches) else f!r}: {f.object_path if isinstance(f, HasBranches) else o!r}}}"
                     for f, o in files
                 )
             )
         )
 
     dask_dict = {}
 
@@ -753,14 +744,15 @@
     )
     common_keys = obj.keys(
         recursive=recursive,
         filter_name=filter_name,
         filter_typename=filter_typename,
         filter_branch=filter_branch,
         full_paths=full_paths,
+        ignore_duplicates=True,
     )
 
     dask_dict = {}
 
     for key in common_keys:
         dt = obj[key].interpretation.numpy_dtype
         if dt.subdtype is None:
@@ -1447,14 +1439,15 @@
 
             new_keys = obj.keys(
                 recursive=recursive,
                 filter_name=filter_name,
                 filter_typename=filter_typename,
                 filter_branch=real_filter_branch,
                 full_paths=full_paths,
+                ignore_duplicates=True,
             )
 
             if common_keys is None:
                 common_keys = new_keys
             else:
                 new_keys = set(new_keys)
                 common_keys = [key for key in common_keys if key in new_keys]
@@ -1468,35 +1461,25 @@
             1, int(math.ceil(total_entries / (total_files * steps_per_file)))
         )
 
     if count == 0:
         raise ValueError(
             "allow_missing=True and no TTrees found in\n\n    {}".format(
                 "\n    ".join(
-                    "{"
-                    + "{}: {}".format(
-                        repr(f.file_path if isinstance(f, HasBranches) else f),
-                        repr(f.object_path if isinstance(f, HasBranches) else o),
-                    )
-                    + "}"
+                    f"{{{f.file_path if isinstance(f, HasBranches) else f!r}: {f.object_path if isinstance(f, HasBranches) else o!r}}}"
                     for f, o in files
                 )
             )
         )
 
     if len(common_keys) == 0 or not (all(is_self) or not any(is_self)):
         raise ValueError(
             "TTrees in\n\n    {}\n\nhave no TBranches in common".format(
                 "\n    ".join(
-                    "{"
-                    + "{}: {}".format(
-                        repr(f.file_path if isinstance(f, HasBranches) else f),
-                        repr(f.object_path if isinstance(f, HasBranches) else o),
-                    )
-                    + "}"
+                    f"{{{f.file_path if isinstance(f, HasBranches) else f!r}: {f.object_path if isinstance(f, HasBranches) else o!r}}}"
                     for f, o in files
                 )
             )
         )
 
     step_sum = 0
     for ttree in ttrees:
@@ -1602,26 +1585,27 @@
 ):
     dask_awkward = uproot.extras.dask_awkward()
     awkward = uproot.extras.awkward()
 
     ffile_path, fobject_path = files[0][0:2]
 
     if known_base_form is not None:
-        common_keys = list(known_base_form.fields)
+        common_keys = list(dict.fromkeys(known_base_form.fields))
         base_form = known_base_form
     else:
         obj = uproot._util.regularize_object_path(
             ffile_path, fobject_path, custom_classes, allow_missing, real_options
         )
         common_keys = obj.keys(
             recursive=recursive,
             filter_name=filter_name,
             filter_typename=filter_typename,
             filter_branch=filter_branch,
             full_paths=full_paths,
+            ignore_duplicates=True,
         )
         base_form = _get_ttree_form(
             awkward, obj, common_keys, interp_options.get("ak_add_doc")
         )
 
     divisions = [0]
     partition_args = []
```

### Comparing `uproot-5.3.2rc1/src/uproot/_util.py` & `uproot-5.3.3/src/uproot/_util.py`

 * *Files 0% similar despite different names*

```diff
@@ -76,15 +76,17 @@
     Returns an ``np.ndarray`` if ``array`` can be converted to an array of the
     desired type and raises TypeError if it cannot.
     """
     import uproot
 
     awkward = uproot.extras.awkward()
     with warnings.catch_warnings():
-        warnings.simplefilter("error", numpy.VisibleDeprecationWarning)
+        warnings.simplefilter(
+            "error", getattr(numpy, "exceptions", numpy).VisibleDeprecationWarning
+        )
         if isinstance(array, awkward.contents.Content):
             out = awkward.to_numpy(array)
         else:
             try:
                 out = numpy.asarray(array)
             except (ValueError, numpy.VisibleDeprecationWarning) as err:
                 raise TypeError("cannot be converted to a NumPy array") from err
```

### Comparing `uproot-5.3.2rc1/src/uproot/behavior.py` & `uproot-5.3.3/src/uproot/behavior.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/cache.py` & `uproot-5.3.3/src/uproot/cache.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/compression.py` & `uproot-5.3.3/src/uproot/compression.py`

 * *Files 2% similar despite different names*

```diff
@@ -430,18 +430,16 @@
             )
             data = cursor.bytes(chunk, block_compressed_bytes, context)
 
             xxhash = uproot.extras.xxhash()
             computed_checksum = xxhash.xxh64(data).intdigest()
             if computed_checksum != expected_checksum:
                 raise ValueError(
-                    """computed checksum {} didn't match expected checksum {}
-in file {}""".format(
-                        computed_checksum, expected_checksum, chunk.source.file_path
-                    )
+                    f"""computed checksum {computed_checksum} didn't match expected checksum {expected_checksum}
+in file {chunk.source.file_path}"""
                 )
 
         elif algo == _decompress_ZSTD._2byte:
             decompressor = _decompress_ZSTD
             data = cursor.bytes(chunk, block_compressed_bytes, context)
 
         elif algo == b"CS":
@@ -464,24 +462,18 @@
 
         uncompressed_bytestring = decompressor.decompress(
             data, block_uncompressed_bytes
         )
 
         if len(uncompressed_bytestring) != block_uncompressed_bytes:
             raise ValueError(
-                """after successfully decompressing {} blocks, a block of """
-                """compressed size {} decompressed to {} bytes, but the """
-                """block header expects {} bytes.
-in file {}""".format(
-                    num_blocks,
-                    block_compressed_bytes,
-                    len(uncompressed_bytestring),
-                    block_uncompressed_bytes,
-                    chunk.source.file_path,
-                )
+                f"""after successfully decompressing {num_blocks} blocks, a block of """
+                f"""compressed size {block_compressed_bytes} decompressed to {len(uncompressed_bytestring)} bytes, but the """
+                f"""block header expects {block_uncompressed_bytes} bytes.
+in file {chunk.source.file_path}"""
             )
 
         uncompressed_array = numpy.frombuffer(
             uncompressed_bytestring, dtype=uproot.source.chunk.Chunk._dtype
         )
 
         if num_blocks == 0:
```

### Comparing `uproot-5.3.2rc1/src/uproot/const.py` & `uproot-5.3.3/src/uproot/const.py`

 * *Files 2% similar despite different names*

```diff
@@ -114,20 +114,20 @@
 kGenerateOffsetMap = numpy.uint8(1)
 
 ############# other
 
 kStreamedMemberWise = numpy.uint16(1 << 14)
 
 ############ RNTuple https://github.com/root-project/root/blob/master/tree/ntuple/v7/doc/specifications.md
-_rntuple_frame_format = struct.Struct("<HH")
-rntuple_env_header = _rntuple_frame_format.pack(1, 1)
+_rntuple_frame_format = struct.Struct("<Q")
+rntuple_env_header = _rntuple_frame_format.pack(0)  # TODO: need to check this
 rntuple_col_num_to_dtype_dict = {
     1: "uint64",
     2: "uint32",
-    3: "uint64",  # Switch
+    3: "switch",  # Switch
     4: "uint8",
     5: "uint8",  # char
     6: "bit",
     7: "float64",
     8: "float32",
     9: "float16",
     10: "uint64",
@@ -149,15 +149,15 @@
     26: "int64",  # split + zigzag encoding
     27: "int32",  # split + zigzag encoding
     28: "int16",  # split + zigzag encoding
 }
 rntuple_col_num_to_size_dict = {
     1: 64,
     2: 32,
-    3: 64,  # Switch
+    3: 96,  # Switch
     4: 8,
     5: 8,  # char
     6: 1,
     7: 64,
     8: 32,
     9: 16,
     10: 64,
```

### Comparing `uproot-5.3.2rc1/src/uproot/containers.py` & `uproot-5.3.3/src/uproot/containers.py`

 * *Files 2% similar despite different names*

```diff
@@ -663,20 +663,15 @@
             values = self._values.__name__
         else:
             values = repr(self._values)
         return f"AsArray({self.header}, {self.speedbump}, {values}, {self.inner_shape})"
 
     @property
     def cache_key(self):
-        return "AsArray({},{},{},{})".format(
-            self.header,
-            self.speedbump,
-            _content_cache_key(self._values),
-            self.inner_shape,
-        )
+        return f"AsArray({self.header},{self.speedbump},{_content_cache_key(self._values)},{self.inner_shape})"
 
     @property
     def typename(self):
         shape = "".join(f"[{d}]" for d in self.inner_shape)
         return _content_typename(self._values) + "[]" + shape
 
     def awkward_form(self, file, context):
@@ -865,15 +860,17 @@
     and :doc:`uproot.containers.AsSet`, which have the same ROOT serialization, but
     represent different runtime classes. The purpose of this superclass is just to
     consolidate implementations.
     """
 
     def __init__(self, header, values):
         self.header = header
-        if isinstance(values, AsContainer):
+        if isinstance(self, uproot.containers.AsBitSet):
+            self._items = numpy.dtype(numpy.bool_)
+        elif isinstance(values, AsContainer):
             self._items = values
         elif isinstance(values, type) and issubclass(
             values, (uproot.model.Model, uproot.model.DispatchByVersion)
         ):
             self._items = values
         else:
             self._items = numpy.dtype(values)
@@ -952,26 +949,22 @@
         if is_memberwise:
             if forth_obj is not None:
                 raise uproot.interpretation.objects.CannotBeForth()
 
             # FIXME: let's hard-code in logic for std::pair<T1,T2> for now
             if not _value_typename.startswith("pair"):
                 raise NotImplementedError(
-                    """memberwise serialization of {}({})
-    in file {}""".format(
-                        type(self).__name__, _value_typename, selffile.file_path
-                    )
+                    f"""memberwise serialization of {type(self).__name__}({_value_typename})
+    in file {selffile.file_path}"""
                 )
 
             if not issubclass(self._items, uproot.model.DispatchByVersion):
                 raise NotImplementedError(
-                    """streamerless memberwise serialization of class {}({})
-    in file {}""".format(
-                        type(self).__name__, _value_typename, selffile.file_path
-                    )
+                    f"""streamerless memberwise serialization of class {type(self).__name__}({_value_typename})
+    in file {selffile.file_path}"""
                 )
 
             # uninterpreted header
             cursor.skip(6)
 
             length = cursor.field(chunk, _stl_container_size, context)
 
@@ -1116,14 +1109,71 @@
         return self._items
 
     @property
     def _container_type(self):
         return STLVector
 
 
+class AsList(AsVectorLike):
+    """
+    Args:
+        header (bool): Sets the :ref:`uproot.containers.AsContainer.header`.
+        values (:doc:`uproot.model.Model` or :doc:`uproot.containers.Container`): Data
+            type for data nested in the container.
+    A :doc:`uproot.containers.AsContainer` for ``std::list``.
+    """
+
+    _specialpathitem_name = "list"
+
+    @property
+    def typename(self):
+        return f"std::list<{_content_typename(self.values)}>"
+
+    @property
+    def values(self):
+        """
+        Data type for data nested in the container.
+        """
+        return self._items
+
+    @property
+    def _container_type(self):
+        return STLList
+
+
+class AsBitSet(AsVectorLike):
+    """
+    Args:
+        header (bool): Sets the :ref:`uproot.containers.AsContainer.header`.
+        keys (:doc:`uproot.model.Model` or :doc:`uproot.containers.Container`): Data
+            type for data nested in the container.
+
+    A :doc:`uproot.containers.AsContainer` for ``std::bitset``.
+    """
+
+    _specialpathitem_name = "bitset"
+
+    @property
+    def typename(self):
+        return f"std::bitset<{_content_typename(self.keys)}>"
+
+    @property
+    def keys(self):
+        """
+        Data type for data nested in the container.
+        """
+        return self._items
+
+    _form_parameters = {"__array__": "bitset"}
+
+    @property
+    def _container_type(self):
+        return STLBitSet
+
+
 class AsSet(AsVectorLike):
     """
     Args:
         header (bool): Sets the :ref:`uproot.containers.AsContainer.header`.
         keys (:doc:`uproot.model.Model` or :doc:`uproot.containers.Container`): Data
             type for data nested in the container.
 
@@ -1216,25 +1266,19 @@
             values = self._values.__name__
         else:
             values = repr(self._values)
         return f"AsMap({self._header}, {keys}, {values})"
 
     @property
     def cache_key(self):
-        return "AsMap({},{},{})".format(
-            self._header,
-            _content_cache_key(self._keys),
-            _content_cache_key(self._values),
-        )
+        return f"AsMap({self._header},{_content_cache_key(self._keys)},{_content_cache_key(self._values)})"
 
     @property
     def typename(self):
-        return "std::map<{}, {}>".format(
-            _content_typename(self._keys), _content_typename(self._values)
-        )
+        return f"std::map<{_content_typename(self._keys)}, {_content_typename(self._values)}>"
 
     def awkward_form(self, file, context):
         awkward = uproot.extras.awkward()
         return awkward.forms.ListOffsetForm(
             context["index_format"],
             awkward.forms.RecordForm(
                 (
@@ -1501,14 +1545,70 @@
 
     def tolist(self):
         return [
             x.tolist() if isinstance(x, (Container, numpy.ndarray)) else x for x in self
         ]
 
 
+class STLList(Container, Sequence):
+    """
+    Args:
+        values (``numpy.ndarray`` or iterable): Contents of the ``std::list``.
+
+    Representation of a C++ ``std::list`` as a Python ``Sequence``.
+    """
+
+    def __init__(self, values):
+        if isinstance(values, types.GeneratorType):
+            values = numpy.asarray(list(values))
+        elif isinstance(values, Set):
+            values = numpy.asarray(list(values))
+        elif isinstance(values, (list, tuple)):
+            values = numpy.asarray(values)
+
+        self._values = values
+
+    def __str__(self, limit=85):
+        def tostring(i):
+            return _tostring(self._values[i])
+
+        return _str_with_ellipsis(tostring, len(self), "[", "]", limit)
+
+    def __repr__(self, limit=85):
+        return f"<STLList {self.__str__(limit=limit - 30)} at 0x{id(self):012x}>"
+
+    def __getitem__(self, where):
+        return self._values[where]
+
+    def __len__(self):
+        return len(self._values)
+
+    def __contains__(self, what):
+        return what in self._values
+
+    def __iter__(self):
+        return iter(self._values)
+
+    def __reversed__(self):
+        return STLList(self._values[::-1])
+
+    def __eq__(self, other):
+        if isinstance(other, STLList):
+            return self._values == other._values
+        elif isinstance(other, Sequence):
+            return self._values == other
+        else:
+            return False
+
+    def tolist(self):
+        return [
+            x.tolist() if isinstance(x, (Container, numpy.ndarray)) else x for x in self
+        ]
+
+
 class STLVector(Container, Sequence):
     """
     Args:
         values (``numpy.ndarray`` or iterable): Contents of the ``std::vector``.
 
     Representation of a C++ ``std::vector`` as a Python ``Sequence``.
     """
@@ -1560,14 +1660,57 @@
 
     def tolist(self):
         return [
             x.tolist() if isinstance(x, (Container, numpy.ndarray)) else x for x in self
         ]
 
 
+class STLBitSet(Container, Sequence):
+    """
+    Args:
+        values (``numpy.ndarray`` or iterable): Contents of the ``std::vector``.
+
+    Representation of a C++ ``std::bitset`` as a Python ``Sequence``.
+    """
+
+    def __init__(self, numbytes):
+        self._numbytes = numpy.asarray(numbytes)
+
+    def __str__(self, limit=85):
+        def tostring(i):
+            return _tostring(self._values[i])
+
+        return _str_with_ellipsis(tostring, len(self), "[", "]", limit)
+
+    def __repr__(self, limit=85):
+        return f"<STLBitSet {self.__str__(limit=limit - 30)} at 0x{id(self):012x}>"
+
+    def __getitem__(self, where):
+        return self._numbytes[where]
+
+    def __len__(self):
+        return self._numbytes
+
+    def __iter__(self):
+        return iter(self._numbytes)
+
+    def __eq__(self, other):
+        if isinstance(other, STLBitSet):
+            return self._numbytes == other._numbytes
+        elif isinstance(other, Sequence):
+            return self._numbytes == other
+        else:
+            return False
+
+    def tolist(self):
+        return [
+            x.tolist() if isinstance(x, (Container, numpy.ndarray)) else x for x in self
+        ]
+
+
 class STLSet(Container, Set):
     """
     Args:
         keys (``numpy.ndarray`` or iterable): Contents of the ``std::set``.
 
     Representation of a C++ ``std::set`` as a Python ``Set``.
     """
```

### Comparing `uproot-5.3.2rc1/src/uproot/deserialization.py` & `uproot-5.3.3/src/uproot/deserialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -169,17 +169,15 @@
 
     Raises a :doc:`uproot.deserialization.DeserializationError` on failure.
     """
     if num_bytes is not None:
         observed = stop_cursor.displacement(start_cursor)
         if observed != num_bytes:
             raise DeserializationError(
-                """expected {} bytes but cursor moved by {} bytes (through {})""".format(
-                    num_bytes, observed, classname
-                ),
+                f"""expected {num_bytes} bytes but cursor moved by {observed} bytes (through {classname})""",
                 chunk,
                 stop_cursor,
                 context,
                 file_path,
             )
```

### Comparing `uproot-5.3.2rc1/src/uproot/dynamic.py` & `uproot-5.3.3/src/uproot/dynamic.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/exceptions.py` & `uproot-5.3.3/src/uproot/exceptions.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/extras.py` & `uproot-5.3.3/src/uproot/extras.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,17 +32,15 @@
 to output as NumPy arrays, rather than Awkward arrays.
 """
         ) from err
     if parse_version(awkward.__version__) >= parse_version("2.4.6"):
         return awkward
     else:
         raise ModuleNotFoundError(
-            "Uproot 5.1+ can only be used with Awkward 2.4.6 or newer; you have Awkward {}".format(
-                awkward.__version__
-            )
+            f"Uproot 5.1+ can only be used with Awkward 2.4.6 or newer; you have Awkward {awkward.__version__}"
         )
 
 
 def pandas():
     """
     Imports and returns ``pandas``.
     """
@@ -324,17 +322,15 @@
 or
     conda install -c conda-forge dask dask-awkward"""
         ) from err
     if parse_version(dask_awkward.__version__) >= parse_version("2023.10.0"):
         return dask_awkward
     else:
         raise ModuleNotFoundError(
-            "Uproot 5.1+ can only be used with dask-awkward 2023.10.0 or newer; you have dask-awkward {}".format(
-                dask_awkward.__version__
-            )
+            f"Uproot 5.1+ can only be used with dask-awkward 2023.10.0 or newer; you have dask-awkward {dask_awkward.__version__}"
         )
 
 
 def awkward_pandas():
     """
     Imports and returns ``awkward_pandas``.
     """
```

### Comparing `uproot-5.3.2rc1/src/uproot/model.py` & `uproot-5.3.3/src/uproot/model.py`

 * *Files 0% similar despite different names*

```diff
@@ -100,14 +100,15 @@
     reload(uproot.models.TBranch)
     reload(uproot.models.TLeaf)
     reload(uproot.models.TBasket)
     reload(uproot.models.RNTuple)
     reload(uproot.models.TH)
     reload(uproot.models.TGraph)
     reload(uproot.models.TMatrixT)
+    reload(uproot.models.TTime)
 
 
 _root_alias_to_c_primitive = {
     "Bool_t": "bool",
     "Char_t": "char",
     "UChar_t": "unsigned char",
     "Short_t": "short",
@@ -1058,17 +1059,15 @@
         if self._deeply_writable:
             return self
         else:
             return self._to_writable(None)
 
     def _serialize(self, out, header, name, tobject_flags):
         raise NotImplementedError(
-            "can't write {} instances yet ('serialize' method not implemented)".format(
-                type(self).__name__
-            )
+            f"can't write {type(self).__name__} instances yet ('serialize' method not implemented)"
         )
 
     def serialize(self, name=None):
         """
         Serialize a object (from num_bytes and version onward) for writing into
         an output ROOT file.
 
@@ -1349,20 +1348,17 @@
             versioned_cls = cls.new_class(file, version)
 
         elif context.get("in_TBranch", False):
             versioned_cls = cls.new_class(file, "max")
 
         else:
             raise ValueError(
-                """Unknown version {} for class {} that cannot be skipped """
+                f"""Unknown version {version} for class {classname_decode(cls.__name__)[0]} that cannot be skipped """
                 """because its number of bytes is unknown.
-""".format(
-                    version,
-                    classname_decode(cls.__name__)[0],
-                )
+"""
             )
 
         # versioned_cls.read starts with numbytes_version again because move=False (above)
         temp_var = cls.postprocess(
             versioned_cls.read(
                 chunk, cursor, context, file, selffile, parent, concrete=concrete
             ),
@@ -1531,19 +1527,17 @@
         self._context = context
 
         if self._num_bytes is not None:
             cursor.skip(self._num_bytes - cursor.displacement(self._cursor))
 
         else:
             raise ValueError(
-                """unknown class {} that cannot be skipped because its """
-                """number of bytes is unknown
-in file {}""".format(
-                    self.classname, file.file_path
-                )
+                f"""unknown class {self.classname} that cannot be skipped because its """
+                f"""number of bytes is unknown
+in file {file.file_path}"""
             )
 
 
 class UnknownClassVersion(VersionedModel):
     """
     Placeholder for a C++ class instance that has no ``TStreamerInfo`` in the
     current :doc:`uproot.reading.ReadOnlyFile` to produce one.
@@ -1664,25 +1658,21 @@
         self._context = context
 
         if self._num_bytes is not None:
             cursor.skip(self._num_bytes - cursor.displacement(self._cursor))
 
         else:
             raise ValueError(
-                """class {} with unknown version {} cannot be skipped """
-                """because its number of bytes is unknown
-in file {}""".format(
-                    self.classname, self._instance_version, file.file_path
-                )
+                f"""class {self.classname} with unknown version {self._instance_version} cannot be skipped """
+                f"""because its number of bytes is unknown
+in file {file.file_path}"""
             )
 
     def __repr__(self):
-        return "<{} with unknown version {} at 0x{:012x}>".format(
-            self.classname, self._instance_version, id(self)
-        )
+        return f"<{self.classname} with unknown version {self._instance_version} at 0x{id(self):012x}>"
 
 
 class DynamicModel(VersionedModel):
     """
     A :doc:`uproot.model.VersionedModel` subclass generated by any attempt to
     extract it from the ``uproot.dynamic`` namespace in Python 3.7 and later.
```

### Comparing `uproot-5.3.2rc1/src/uproot/pyroot.py` & `uproot-5.3.3/src/uproot/pyroot.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/reading.py` & `uproot-5.3.3/src/uproot/reading.py`

 * *Files 1% similar despite different names*

```diff
@@ -891,18 +891,16 @@
                         isinstance(y, uproot.models.TObjString.Model_TObjString)
                         for y in x
                     ):
                         self._streamer_rules.extend([str(y) for y in x])
 
                     else:
                         raise ValueError(
-                            """unexpected type in TList of streamers and streamer rules: {}
-in file {}""".format(
-                                type(x), self._file_path
-                            )
+                            f"""unexpected type in TList of streamers and streamer rules: {type(x)}
+in file {self._file_path}"""
                         )
 
                 self.hook_after_interpret_streamers(
                     key_chunk=key_chunk,
                     key_cursor=key_cursor,
                     streamer_key=streamer_key,
                     streamer_cursor=streamer_cursor,
@@ -1104,14 +1102,24 @@
         cls = classes.get(classname)
 
         if cls is None:
             streamers = self.streamers_named(classname)
             if len(streamers) == 0 and self._custom_classes is not None:
                 cls = uproot.classes.get(classname)
 
+        if (
+            cls is None
+            and re.match(r"(std\s*::\s*)?(vector|list|map|set|bitset)\s*<", classname)
+            is not None
+        ):
+            cls = uproot.interpretation.identify.parse_typename(classname)
+            cls._header = False
+
+            return cls
+
         if cls is None:
             if len(streamers) == 0:
                 unknown_cls = uproot.unknown_classes.get(classname)
                 if unknown_cls is None:
                     unknown_cls = uproot._util.new_class(
                         uproot.model.classname_encode(classname, unknown=True),
                         (uproot.model.UnknownClass,),
@@ -2309,17 +2317,15 @@
         )
 
     def __repr__(self):
         if self._fName is None or self._fClassName is None:
             nameclass = ""
         else:
             nameclass = f" {self.name(cycle=True)}: {self.classname()}"
-        return "<ReadOnlyKey{} (seek pos {}) at 0x{:012x}>".format(
-            nameclass, self.data_cursor.index, id(self)
-        )
+        return f"<ReadOnlyKey{nameclass} (seek pos {self.data_cursor.index}) at 0x{id(self):012x}>"
 
     @property
     def cursor(self):
         """
         A :doc:`uproot.source.cursor.Cursor` pointing to the seek point in the
         file where this ``TKey`` starts (before its header fields).
         """
@@ -2494,15 +2500,15 @@
             )
 
         else:
             chunk, cursor = self.get_uncompressed_chunk_cursor()
             start_cursor = cursor.copy()
             context = {"breadcrumbs": (), "TKey": self}
 
-            if self._fClassName == "string":
+            if re.match(r"(std\s*::\s*)?string", self._fClassName):
                 return cursor.string(chunk, context)
 
             cls = self._file.class_named(self._fClassName)
 
             try:
                 out = cls.read(chunk, cursor, context, self._file, selffile, parent)
```

### Comparing `uproot-5.3.2rc1/src/uproot/serialization.py` & `uproot-5.3.3/src/uproot/serialization.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/streamers.py` & `uproot-5.3.3/src/uproot/streamers.py`

 * *Files 0% similar despite different names*

```diff
@@ -1124,15 +1124,15 @@
         ):
             self._bases[0]._members["fSize"] = 4
 
         elif self._bases[0]._members["fType"] in (
             uproot.const.kULong,
             uproot.const.kLong,
         ):
-            self._bases[0]._members["fSize"] = numpy.dtype(numpy.compat.long).itemsize
+            self._bases[0]._members["fSize"] = numpy.dtype(numpy.int64).itemsize
 
         elif self._bases[0]._members["fType"] in (
             uproot.const.kULong64,
             uproot.const.kLong64,
         ):
             self._bases[0]._members["fSize"] = 8
```

### Comparing `uproot-5.3.2rc1/src/uproot/behaviors/RooCurve.py` & `uproot-5.3.3/src/uproot/behaviors/RooCurve.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/behaviors/RooHist.py` & `uproot-5.3.3/src/uproot/behaviors/RooHist.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/behaviors/TAxis.py` & `uproot-5.3.3/src/uproot/behaviors/TAxis.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/behaviors/TBranch.py` & `uproot-5.3.3/src/uproot/behaviors/TBranch.py`

 * *Files 2% similar despite different names*

```diff
@@ -623,19 +623,15 @@
         if name_width < 3:
             raise ValueError("'name_width' must be at least 3")
         if typename_width < 3:
             raise ValueError("'typename_width' must be at least 3")
         if interpretation_width < 3:
             raise ValueError("'interpretation_width' must be at least 3")
 
-        formatter = "{{0:{0}.{0}}} | {{1:{1}.{1}}} | {{2:{2}.{2}}}".format(
-            name_width,
-            typename_width,
-            interpretation_width,
-        )
+        formatter = f"{{0:{name_width}.{name_width}}} | {{1:{typename_width}.{typename_width}}} | {{2:{interpretation_width}.{interpretation_width}}}"
 
         stream.write(formatter.format("name", "typename", "interpretation"))
         stream.write(
             "\n"
             + "-" * name_width
             + "-+-"
             + "-" * typename_width
@@ -788,22 +784,15 @@
             decompression_executor, interpretation_executor, self._file
         )
         array_cache = _regularize_array_cache(array_cache, self._file)
         library = uproot.interpretation.library._regularize_library(library)
 
         def get_from_cache(branchname, interpretation):
             if array_cache is not None:
-                cache_key = "{}:{}:{}:{}-{}:{}".format(
-                    self.cache_key,
-                    branchname,
-                    interpretation.cache_key,
-                    entry_start,
-                    entry_stop,
-                    library.name,
-                )
+                cache_key = f"{self.cache_key}:{branchname}:{interpretation.cache_key}:{entry_start}-{entry_stop}:{library.name}"
                 return array_cache.get(cache_key)
             else:
                 return None
 
         aliases = _regularize_aliases(self, aliases)
         arrays, expression_context, branchid_interpretation = _regularize_expressions(
             self,
@@ -861,22 +850,15 @@
             checked = set()
             for expression, context in expression_context:
                 for branch in context["branches"]:
                     if branch.cache_key not in checked:
                         checked.add(branch.cache_key)
                         interpretation = branchid_interpretation[branch.cache_key]
                         if branch is not None:
-                            cache_key = "{}:{}:{}:{}-{}:{}".format(
-                                self.cache_key,
-                                expression,
-                                interpretation.cache_key,
-                                entry_start,
-                                entry_stop,
-                                library.name,
-                            )
+                            cache_key = f"{self.cache_key}:{expression}:{interpretation.cache_key}:{entry_start}-{entry_stop}:{library.name}"
                         array_cache[cache_key] = arrays[branch.cache_key]
 
         output = language.compute_expressions(
             self,
             arrays,
             expression_context,
             keys,
@@ -1140,14 +1122,15 @@
         self,
         *,
         filter_name=no_filter,
         filter_typename=no_filter,
         filter_branch=no_filter,
         recursive=True,
         full_paths=True,
+        ignore_duplicates=False,
     ):
         """
         Args:
             filter_name (None, glob string, regex string in ``"/pattern/i"`` syntax, function of str \u2192 bool, or iterable of the above): A
                 filter to select ``TBranches`` by name.
             filter_typename (None, glob string, regex string in ``"/pattern/i"`` syntax, function of str \u2192 bool, or iterable of the above): A
                 filter to select ``TBranches`` by type.
@@ -1157,24 +1140,26 @@
                 included if the function returns True, excluded if it returns False.
             recursive (bool): If True, descend into any nested subbranches.
                 If False, only return the names of branches directly accessible
                 under this object.
             full_paths (bool): If True, include the full path to each subbranch
                 with slashes (``/``); otherwise, use the descendant's name as
                 the output name.
+            ignore_duplicates (bool): If True, return a set of the keys; otherwise, return the full list of keys.
 
         Returns the names of the subbranches as a list of strings.
         """
         return list(
             self.iterkeys(
                 filter_name=filter_name,
                 filter_typename=filter_typename,
                 filter_branch=filter_branch,
                 recursive=recursive,
                 full_paths=full_paths,
+                ignore_duplicates=ignore_duplicates,
             )
         )
 
     def values(
         self,
         *,
         filter_name=no_filter,
@@ -1293,14 +1278,15 @@
         self,
         *,
         filter_name=no_filter,
         filter_typename=no_filter,
         filter_branch=no_filter,
         recursive=True,
         full_paths=True,
+        ignore_duplicates=False,
     ):
         """
         Args:
             filter_name (None, glob string, regex string in ``"/pattern/i"`` syntax, function of str \u2192 bool, or iterable of the above): A
                 filter to select ``TBranches`` by name.
             filter_typename (None, glob string, regex string in ``"/pattern/i"`` syntax, function of str \u2192 bool, or iterable of the above): A
                 filter to select ``TBranches`` by type.
@@ -1310,23 +1296,26 @@
                 included if the function returns True, excluded if it returns False.
             recursive (bool): If True, descend into any nested subbranches.
                 If False, only return the names of branches directly accessible
                 under this object.
             full_paths (bool): If True, include the full path to each subbranch
                 with slashes (``/``); otherwise, use the descendant's name as
                 the output name.
+            ignore_duplicates (bool): If True, return a set of the keys; otherwise, return the full list of keys.
+
 
         Returns the names of the subbranches as an iterator over strings.
         """
         for k, _ in self.iteritems(
             filter_name=filter_name,
             filter_typename=filter_typename,
             filter_branch=filter_branch,
             recursive=recursive,
             full_paths=full_paths,
+            ignore_duplicates=ignore_duplicates,
         ):
             yield k
 
     def itervalues(
         self,
         *,
         filter_name=no_filter,
@@ -1367,14 +1356,15 @@
         self,
         *,
         filter_name=no_filter,
         filter_typename=no_filter,
         filter_branch=no_filter,
         recursive=True,
         full_paths=True,
+        ignore_duplicates=False,
     ):
         """
         Args:
             filter_name (None, glob string, regex string in ``"/pattern/i"`` syntax, function of str \u2192 bool, or iterable of the above): A
                 filter to select ``TBranches`` by name.
             filter_typename (None, glob string, regex string in ``"/pattern/i"`` syntax, function of str \u2192 bool, or iterable of the above): A
                 filter to select ``TBranches`` by type.
@@ -1384,55 +1374,65 @@
                 included if the function returns True, excluded if it returns False.
             recursive (bool): If True, descend into any nested subbranches.
                 If False, only return (name, branch) pairs for branches
                 directly accessible under this object.
             full_paths (bool): If True, include the full path to each subbranch
                 with slashes (``/``) in the name; otherwise, use the descendant's
                 name as the name without modification.
+            ignore_duplicates (bool): If True, return a set of the keys; otherwise, return the full list of keys.
+
 
         Returns (name, branch) pairs of the subbranches as an iterator over
         2-tuples of (str, :doc:`uproot.behaviors.TBranch.TBranch`).
         """
         filter_name = uproot._util.regularize_filter(filter_name)
         filter_typename = uproot._util.regularize_filter(filter_typename)
         if filter_branch is None:
             filter_branch = no_filter
         elif callable(filter_branch):
             pass
         else:
             raise TypeError(
-                "filter_branch must be None or a function: TBranch -> bool, not {}".format(
-                    repr(filter_branch)
-                )
+                f"filter_branch must be None or a function: TBranch -> bool, not {filter_branch!r}"
             )
 
+        keys_set = set()
+
         for branch in self.branches:
             if (
                 (
                     filter_name is no_filter
                     or _filter_name_deep(filter_name, self, branch)
                 )
                 and (filter_typename is no_filter or filter_typename(branch.typename))
                 and (filter_branch is no_filter or filter_branch(branch))
             ):
-                yield branch.name, branch
+                if ignore_duplicates and branch.name in keys_set:
+                    pass
+                else:
+                    keys_set.add(branch.name)
+                    yield branch.name, branch
 
             if recursive:
                 for k1, v in branch.iteritems(
                     recursive=recursive,
                     filter_name=no_filter,
                     filter_typename=filter_typename,
                     filter_branch=filter_branch,
                     full_paths=full_paths,
                 ):
                     k2 = f"{branch.name}/{k1}" if full_paths else k1
                     if filter_name is no_filter or _filter_name_deep(
                         filter_name, self, v
                     ):
-                        yield k2, v
+                        if ignore_duplicates and branch.name in keys_set:
+                            pass
+                        else:
+                            keys_set.add(k2)
+                            yield k2, v
 
     def itertypenames(
         self,
         *,
         filter_name=no_filter,
         filter_typename=no_filter,
         filter_branch=no_filter,
@@ -1697,17 +1697,15 @@
         my_branch["subbranch/subsubbranch"]
     """
 
     def __repr__(self):
         if len(self) == 0:
             return f"<{self.classname} {self.name!r} at 0x{id(self):012x}>"
         else:
-            return "<{} {} ({} subbranches) at 0x{:012x}>".format(
-                self.classname, repr(self.name), len(self), id(self)
-            )
+            return f"<{self.classname} {self.name!r} ({len(self)} subbranches) at 0x{id(self):012x}>"
 
     def array(
         self,
         interpretation=None,
         entry_start=None,
         entry_stop=None,
         *,
@@ -1777,22 +1775,15 @@
             decompression_executor, interpretation_executor, self._file
         )
         array_cache = _regularize_array_cache(array_cache, self._file)
         library = uproot.interpretation.library._regularize_library(library)
 
         def get_from_cache(branchname, interpretation):
             if array_cache is not None:
-                cache_key = "{}:{}:{}:{}-{}:{}".format(
-                    self.cache_key,
-                    branchname,
-                    interpretation.cache_key,
-                    entry_start,
-                    entry_stop,
-                    library.name,
-                )
+                cache_key = f"{self.cache_key}:{branchname}:{interpretation.cache_key}:{entry_start}-{entry_stop}:{library.name}"
                 return array_cache.get(cache_key)
             else:
                 return None
 
         arrays = {}
         expression_context = []
         branchid_interpretation = {}
@@ -1845,22 +1836,15 @@
             branchid_interpretation,
             library,
             None,
             ak_add_doc,
         )
 
         if array_cache is not None:
-            cache_key = "{}:{}:{}:{}-{}:{}".format(
-                self.cache_key,
-                self.name,
-                interpretation.cache_key,
-                entry_start,
-                entry_stop,
-                library.name,
-            )
+            cache_key = f"{self.cache_key}:{self.name}:{interpretation.cache_key}:{entry_start}-{entry_stop}:{library.name}"
             array_cache[cache_key] = arrays[self.cache_key]
 
         return arrays[self.cache_key]
 
     def __array__(self, *args, **kwargs):
         out = self.array(library="np")
         if args == () and kwargs == {}:
@@ -2000,22 +1984,17 @@
             out[-1] != self.num_entries
             and self.interpretation is not None
             and not isinstance(
                 self.interpretation, uproot.interpretation.grouped.AsGrouped
             )
         ):
             raise ValueError(
-                """entries in normal baskets ({}) plus embedded baskets ({}) """
-                """don't add up to expected number of entries ({})
-in file {}""".format(
-                    num_entries_normal,
-                    sum(basket.num_entries for basket in self.embedded_baskets),
-                    self.num_entries,
-                    self._file.file_path,
-                )
+                f"""entries in normal baskets ({num_entries_normal}) plus embedded baskets ({sum(basket.num_entries for basket in self.embedded_baskets)}) """
+                f"""don't add up to expected number of entries ({self.num_entries})
+in file {self._file.file_path}"""
             )
         else:
             return out
 
     def basket_entry_start_stop(self, basket_num):
         """
         The starting and stopping entry number for ``TBasket`` number ``basket_num``.
@@ -2037,19 +2016,17 @@
                 baskets_before += 1
                 entries_before += basket.num_entries
             else:
                 raise AssertionError
 
         else:
             raise IndexError(
-                """branch {} has {} baskets; cannot get starting entry """
-                """for basket {}
-in file {}""".format(
-                    repr(self.name), self.num_baskets, basket_num, self._file.file_path
-                )
+                f"""branch {self.name!r} has {self.num_baskets} baskets; cannot get starting entry """
+                f"""for basket {basket_num}
+in file {self._file.file_path}"""
             )
 
     @property
     def tree(self):
         """
         The ``TTree`` to which this ``TBranch`` belongs. The branch might be
         deeply nested; this property ascends all the way to the top.
@@ -2256,18 +2233,16 @@
             return uproot.models.TBasket.Model_TBasket.read(
                 chunk, cursor, {"basket_num": basket_num}, self._file, self._file, self
             )
         elif 0 <= basket_num < self.num_baskets:
             return self.embedded_baskets[basket_num - self._num_normal_baskets]
         else:
             raise IndexError(
-                """branch {} has {} baskets; cannot get basket {}
-in file {}""".format(
-                    repr(self.name), self.num_baskets, basket_num, self._file.file_path
-                )
+                f"""branch {self.name!r} has {self.num_baskets} baskets; cannot get basket {basket_num}
+in file {self._file.file_path}"""
             )
 
     def basket_chunk_cursor(self, basket_num):
         """
         Returns a :doc:`uproot.source.chunk.Chunk` and
         :doc:`uproot.source.cursor.Cursor` as a 2-tuple for a given
         ``basket_num``.
@@ -2282,30 +2257,23 @@
             start = self.member("fBasketSeek")[basket_num]
             stop = start + self.basket_compressed_bytes(basket_num)
             cursor = uproot.source.cursor.Cursor(start)
             chunk = self._file.source.chunk(start, stop)
             return chunk, cursor
         elif 0 <= basket_num < self.num_baskets:
             raise IndexError(
-                """branch {} has {} normal baskets; cannot get chunk and """
-                """cursor for basket {} because only normal baskets have cursors
-in file {}""".format(
-                    repr(self.name),
-                    self._num_normal_baskets,
-                    basket_num,
-                    self._file.file_path,
-                )
+                f"""branch {self.name!r} has {self._num_normal_baskets} normal baskets; cannot get chunk and """
+                f"""cursor for basket {basket_num} because only normal baskets have cursors
+in file {self._file.file_path}"""
             )
         else:
             raise IndexError(
-                """branch {} has {} baskets; cannot get cursor and chunk """
-                """for basket {}
-in file {}""".format(
-                    repr(self.name), self.num_baskets, basket_num, self._file.file_path
-                )
+                f"""branch {self.name!r} has {self.num_baskets} baskets; cannot get cursor and chunk """
+                f"""for basket {basket_num}
+in file {self._file.file_path}"""
             )
 
     def basket_compressed_bytes(self, basket_num):
         """
         The number of compressed bytes for the ``TBasket`` at ``basket_num``,
         including the TKey header.
 
@@ -2317,18 +2285,16 @@
             return int(self.member("fBasketBytes")[basket_num])
         elif 0 <= basket_num < self.num_baskets:
             return self.embedded_baskets[
                 basket_num - self._num_normal_baskets
             ].compressed_bytes
         else:
             raise IndexError(
-                """branch {} has {} baskets; cannot get basket chunk {}
-in file {}""".format(
-                    repr(self.name), self.num_baskets, basket_num, self._file.file_path
-                )
+                f"""branch {self.name!r} has {self.num_baskets} baskets; cannot get basket chunk {basket_num}
+in file {self._file.file_path}"""
             )
 
     def basket_uncompressed_bytes(self, basket_num):
         """
         The number of uncompressed bytes for the ``TBasket`` at ``basket_num``,
         including the TKey header.
 
@@ -2359,25 +2325,21 @@
 
             return uproot.reading.ReadOnlyKey(
                 chunk, cursor, {}, self._file, self, read_strings=False
             )
 
         elif 0 <= basket_num < self.num_baskets:
             raise ValueError(
-                "branch {} basket {} is an embedded basket, which has no TKey".format(
-                    repr(self.name), basket_num
-                )
+                f"branch {self.name!r} basket {basket_num} is an embedded basket, which has no TKey"
             )
 
         else:
             raise IndexError(
-                """branch {} has {} baskets; cannot get basket chunk {}
-in file {}""".format(
-                    repr(self.name), self.num_baskets, basket_num, self._file.file_path
-                )
+                f"""branch {self.name!r} has {self.num_baskets} baskets; cannot get basket chunk {basket_num}
+in file {self._file.file_path}"""
             )
 
     @property
     def embedded_baskets(self):
         """
         The ``TBaskets`` that are embedded within the ``TBranch`` metadata,
         usually because the ROOT process that was writing the file closed
@@ -2491,27 +2453,22 @@
         return self
 
     def _awkward_check(self, interpretation):
         try:
             interpretation.awkward_form(self.file)
         except uproot.interpretation.objects.CannotBeAwkward as err:
             raise ValueError(
-                """cannot produce Awkward Arrays for interpretation {} because
+                f"""cannot produce Awkward Arrays for interpretation {interpretation!r} because
 
-    {}
+    {err.because}
 
 instead, try library="np" rather than library="ak" or globally set uproot.default_library
 
-in file {}
-in object {}""".format(
-                    repr(interpretation),
-                    err.because,
-                    self.file.file_path,
-                    self.object_path,
-                )
+in file {self.file.file_path}
+in object {self.object_path}"""
             ) from err
 
     def debug(
         self,
         entry,
         skip_bytes=None,
         limit_bytes=None,
@@ -2747,18 +2704,15 @@
     if branch.cache_key in branchid_interpretation:
         if (
             branchid_interpretation[branch.cache_key].cache_key
             != interpretation.cache_key
         ):
             raise ValueError(
                 "a branch cannot be loaded with multiple interpretations: "
-                "{} and {}".format(
-                    repr(branchid_interpretation[branch.cache_key]),
-                    repr(interpretation),
-                )
+                f"{branchid_interpretation[branch.cache_key]!r} and {interpretation!r}"
             )
     else:
         branchid_interpretation[branch.cache_key] = interpretation
 
     c = {
         "is_primary": is_primary,
         "is_cut": is_cut,
@@ -3103,24 +3057,17 @@
                 context,
                 basket.member("fKeylen"),
                 library,
                 interp_options,
             )
             if basket.num_entries != len(basket_arrays[basket.basket_num]):
                 raise ValueError(
-                    """basket {} in tree/branch {} has the wrong number of entries """
-                    """(expected {}, obtained {}) when interpreted as {}
-    in file {}""".format(
-                        basket.basket_num,
-                        branch.object_path,
-                        basket.num_entries,
-                        len(basket_arrays[basket.basket_num]),
-                        interpretation,
-                        branch.file.file_path,
-                    )
+                    f"""basket {basket.basket_num} in tree/branch {branch.object_path} has the wrong number of entries """
+                    f"""(expected {basket.num_entries}, obtained {len(basket_arrays[basket.basket_num])}) when interpreted as {interpretation}
+    in file {branch.file.file_path}"""
                 )
 
             basket = None
 
             if len(basket_arrays) == branchid_num_baskets[branch.cache_key]:
                 arrays[branch.cache_key] = interpretation.final_array(
                     basket_arrays,
```

### Comparing `uproot-5.3.2rc1/src/uproot/behaviors/TBranchElement.py` & `uproot-5.3.3/src/uproot/behaviors/TBranchElement.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/behaviors/TGraph.py` & `uproot-5.3.3/src/uproot/behaviors/TGraph.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/behaviors/TGraphAsymmErrors.py` & `uproot-5.3.3/src/uproot/behaviors/TGraphAsymmErrors.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/behaviors/TH1.py` & `uproot-5.3.3/src/uproot/behaviors/TH1.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/behaviors/TH2.py` & `uproot-5.3.3/src/uproot/behaviors/TH2.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/behaviors/TH2Poly.py` & `uproot-5.3.3/src/uproot/behaviors/TH2Poly.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/behaviors/TH3.py` & `uproot-5.3.3/src/uproot/behaviors/TH3.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/behaviors/TParameter.py` & `uproot-5.3.3/src/uproot/behaviors/TParameter.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/behaviors/TProfile.py` & `uproot-5.3.3/src/uproot/behaviors/TProfile.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/behaviors/TProfile2D.py` & `uproot-5.3.3/src/uproot/behaviors/TProfile2D.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/behaviors/TProfile3D.py` & `uproot-5.3.3/src/uproot/behaviors/TProfile3D.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/behaviors/TTree.py` & `uproot-5.3.3/src/uproot/behaviors/TTree.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,17 +25,15 @@
         my_tree["branch/subbranch/subsubbranch"]
     """
 
     def __repr__(self):
         if len(self) == 0:
             return f"<TTree {self.name!r} at 0x{id(self):012x}>"
         else:
-            return "<TTree {} ({} branches) at 0x{:012x}>".format(
-                repr(self.name), len(self), id(self)
-            )
+            return f"<TTree {self.name!r} ({len(self)} branches) at 0x{id(self):012x}>"
 
     @property
     def name(self):
         """
         Name of the ``TTree``.
         """
         return self.member("fName")
```

### Comparing `uproot-5.3.2rc1/src/uproot/behaviors/__init__.py` & `uproot-5.3.3/src/uproot/behaviors/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/interpretation/__init__.py` & `uproot-5.3.3/src/uproot/interpretation/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/interpretation/grouped.py` & `uproot-5.3.3/src/uproot/interpretation/grouped.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/interpretation/identify.py` & `uproot-5.3.3/src/uproot/interpretation/identify.py`

 * *Files 0% similar despite different names*

```diff
@@ -960,15 +960,15 @@
         except ValueError:
             _parse_error(tokens[i + 2].start() + 1, typename, file)
         # std::bitset only ever has one argument
         _parse_expect(">", tokens, i + 3, typename, file)
         return (
             i + 4,
             _parse_maybe_quote(
-                f'uproot.containers.AsFIXME("std::bitset<{num_bits}>")',
+                f"uproot.containers.AsBitSet({header}, {num_bits})",
                 quote,
             ),
         )
 
     elif tokens[i].group(0) == "vector" or _simplify_token(tokens[i]) == "std::vector":
         _parse_expect("<", tokens, i + 1, typename, file)
         i, values = _parse_node(
@@ -980,14 +980,29 @@
             return (
                 i + 1,
                 f"uproot.containers.AsVector({header}, {values})",
             )
         else:
             return i + 1, uproot.containers.AsVector(header, values)
 
+    elif tokens[i].group(0) == "list" or _simplify_token(tokens[i]) == "std::list":
+        _parse_expect("<", tokens, i + 1, typename, file)
+        i, values = _parse_node(
+            tokens, i + 2, typename, file, quote, inner_header, inner_header
+        )
+        i = _parse_ignore_extra_arguments(tokens, i, typename, file, 1)
+        _parse_expect(">", tokens, i, typename, file)
+        if quote:
+            return (
+                i + 1,
+                f"uproot.containers.AsList({header}, {values})",
+            )
+        else:
+            return i + 1, uproot.containers.AsList(header, values)
+
     elif (
         tokens[i].group(0) == "RVec"
         or _simplify_token(tokens[i]) == "VecOps::RVec"
         or _simplify_token(tokens[i]) == "ROOT::VecOps::RVec"
     ):
         _parse_expect("<", tokens, i + 1, typename, file)
         i, values = _parse_node(
```

### Comparing `uproot-5.3.2rc1/src/uproot/interpretation/jagged.py` & `uproot-5.3.3/src/uproot/interpretation/jagged.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/interpretation/library.py` & `uproot-5.3.3/src/uproot/interpretation/library.py`

 * *Files 0% similar despite different names*

```diff
@@ -977,27 +977,23 @@
 
 def _regularize_library(library):
     if isinstance(library, Library):
         if library.name in _libraries:
             return _libraries[library.name]
         else:
             raise ValueError(
-                "library {} ({}) cannot be used in this function".format(
-                    type(library).__name__, repr(library.name)
-                )
+                f"library {type(library).__name__} ({library.name!r}) cannot be used in this function"
             )
 
     elif isinstance(library, type) and issubclass(library, Library):
         if library().name in _libraries:
             return _libraries[library().name]
         else:
             raise ValueError(
-                "library {} ({}) cannot be used in this function".format(
-                    library.__name__, repr(library().name)
-                )
+                f"library {library.__name__} ({library().name!r}) cannot be used in this function"
             )
 
     else:
         try:
             return _libraries[library]
         except KeyError as err:
             raise ValueError(
```

### Comparing `uproot-5.3.2rc1/src/uproot/interpretation/numerical.py` & `uproot-5.3.3/src/uproot/interpretation/numerical.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,15 +102,15 @@
 
                 elif entry_start < stop and start <= entry_stop:
                     basket_array = basket_arrays[basket_num]
                     output[start - entry_start : stop - entry_start] = basket_array
 
                 start = stop
 
-        output = output.newbyteorder("=")
+        output = output.view(output.dtype.newbyteorder("="))
         self.hook_before_library_finalize(
             basket_arrays=basket_arrays,
             entry_start=entry_start,
             entry_stop=entry_stop,
             entry_offsets=entry_offsets,
             library=library,
             branch=branch,
@@ -355,23 +355,17 @@
         )
 
         dtype, shape = _dtype_shape(self._from_dtype)
         try:
             output = data.view(dtype).reshape((-1, *shape))
         except ValueError as err:
             raise ValueError(
-                """basket {} in tree/branch {} has the wrong number of bytes ({}) """
-                """for interpretation {}
-in file {}""".format(
-                    basket.basket_num,
-                    branch.object_path,
-                    len(data),
-                    self,
-                    branch.file.file_path,
-                )
+                f"""basket {basket.basket_num} in tree/branch {branch.object_path} has the wrong number of bytes ({len(data)}) """
+                f"""for interpretation {self}
+in file {branch.file.file_path}"""
             ) from err
 
         self.hook_after_basket_array(
             data=data,
             byte_offsets=byte_offsets,
             basket=basket,
             branch=branch,
@@ -417,26 +411,22 @@
 
     def _prepare_output(self, library, length):
         """
         Specialized version of _prepare_output : re-use our target array kept in self._to_fill.
         """
         if library.name != "np":
             raise TypeError(
-                "AsDtypeInPlace can only be used with library 'np', not '{}'".format(
-                    library.name
-                )
+                f"AsDtypeInPlace can only be used with library 'np', not '{library.name}'"
             )
 
         output = self._to_fill.view(self.to_dtype)
 
         if length > len(output):
             raise ValueError(
-                "Requesting to fill an array of size {} (type {}) with input of size {} (type {})".format(
-                    len(output), self._to_dtype, length, self._from_dtype
-                )
+                f"Requesting to fill an array of size {len(output)} (type {self._to_dtype}) with input of size {length} (type {self._from_dtype})"
             )
         return output[:length]
 
 
 class AsSTLBits(Numerical):
     """
     Interpretation for ``std::bitset``.
@@ -537,17 +527,15 @@
 
     @property
     def numpy_dtype(self):
         return self.to_dtype
 
     @property
     def cache_key(self):
-        return "{}({},{},{},{})".format(
-            type(self).__name__, self._low, self._high, self._num_bits, self._to_dims
-        )
+        return f"{type(self).__name__}({self._low},{self._high},{self._num_bits},{self._to_dims})"
 
     def basket_array(
         self,
         data,
         byte_offsets,
         basket,
         branch,
@@ -567,24 +555,17 @@
             options=options,
         )
 
         try:
             raw = data.view(self.from_dtype)
         except ValueError as err:
             raise ValueError(
-                """basket {} in tree/branch {} has the wrong number of bytes ({}) """
-                """for interpretation {} (expecting raw array of {})
-in file {}""".format(
-                    basket.basket_num,
-                    branch.object_path,
-                    len(data),
-                    self,
-                    repr(self._from_dtype),
-                    branch.file.file_path,
-                )
+                f"""basket {basket.basket_num} in tree/branch {branch.object_path} has the wrong number of bytes ({len(data)}) """
+                f"""for interpretation {self} (expecting raw array of {self._from_dtype!r})
+in file {branch.file.file_path}"""
             ) from err
 
         if self.is_truncated:
             exponent = raw["exponent"].astype(numpy.int32)
             mantissa = raw["mantissa"].astype(numpy.int32)
 
             exponent <<= 23
```

### Comparing `uproot-5.3.2rc1/src/uproot/interpretation/objects.py` & `uproot-5.3.3/src/uproot/interpretation/objects.py`

 * *Files 1% similar despite different names*

```diff
@@ -828,23 +828,17 @@
             ]
             self._to_dtype = numpy.dtype(dtype)
         try:
             output = data.view(dtype).reshape((-1, *shape))
 
         except ValueError as err:
             raise ValueError(
-                """basket {} in tree/branch {} has the wrong number of bytes ({}) """
-                """for interpretation {}
-in file {}""".format(
-                    basket.basket_num,
-                    branch.object_path,
-                    len(data),
-                    self,
-                    branch.file.file_path,
-                )
+                f"""basket {basket.basket_num} in tree/branch {branch.object_path} has the wrong number of bytes ({len(data)}) """
+                f"""for interpretation {self}
+in file {branch.file.file_path}"""
             ) from err
         self.hook_after_basket_array(
             data=data,
             byte_offsets=byte_offsets,
             basket=basket,
             branch=branch,
             context=context,
@@ -921,22 +915,15 @@
         self._context = context
         self._byte_offsets = byte_offsets
         self._byte_content = byte_content
         self._cursor_offset = cursor_offset
         self._detached_file = self._branch.file.detached
 
     def __repr__(self):
-        return "ObjectArray({}, {}, {}, {}, {}, {})".format(
-            self._model,
-            self._branch,
-            self._context,
-            self._byte_offsets,
-            self._byte_content,
-            self._cursor_offset,
-        )
+        return f"ObjectArray({self._model}, {self._branch}, {self._context}, {self._byte_offsets}, {self._byte_content}, {self._cursor_offset})"
 
     @property
     def model(self):
         """
         The full Uproot deserialization model for the data
         (:doc:`uproot.model.Model` or :doc:`uproot.containers.AsContainer`).
         """
```

### Comparing `uproot-5.3.2rc1/src/uproot/interpretation/strings.py` & `uproot-5.3.3/src/uproot/interpretation/strings.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/language/__init__.py` & `uproot-5.3.3/src/uproot/language/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/language/python.py` & `uproot-5.3.3/src/uproot/language/python.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,17 +24,15 @@
         raise SyntaxError(
             err.args[0] + f"\nin file {file_path}\nin object {object_path}",
             err.args[1],
         ) from err
 
     if len(node.body) != 1 or not isinstance(node.body[0], ast.Expr):
         raise SyntaxError(
-            "expected a single expression\nin file {}\nin object {}".format(
-                file_path, object_path
-            )
+            f"expected a single expression\nin file {file_path}\nin object {object_path}"
         )
 
     return node
 
 
 def _attribute_to_dotted_name(node):
     if isinstance(node, ast.Attribute):
```

### Comparing `uproot-5.3.2rc1/src/uproot/models/RNTuple.py` & `uproot-5.3.3/src/uproot/models/RNTuple.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,47 +2,51 @@
 
 """
 This module defines a versionless model for ``ROOT::Experimental::RNTuple``.
 """
 from __future__ import annotations
 
 import struct
-import zlib
 from collections import defaultdict
 
 import numpy
 
 import uproot
 
-# https://github.com/root-project/root/blob/e9fa243af91217e9b108d828009c81ccba7666b5/tree/ntuple/v7/inc/ROOT/RMiniFile.hxx#L65
-_rntuple_format1 = struct.Struct(">IIIQIIQIIQ")
+# https://github.com/root-project/root/blob/aa513463b0b512517370cb91cca025e53a8b13a2/tree/ntuple/v7/inc/ROOT/RNTupleAnchor.hxx#L69
+_rntuple_anchor_format = struct.Struct(">HHHHQQQQQQQ")
 
-# https://github.com/jblomer/root/blob/ntuple-binary-format-v1/tree/ntuple/v7/doc/specifications.md#envelopes
+# https://github.com/root-project/root/blob/aa513463b0b512517370cb91cca025e53a8b13a2/tree/ntuple/v7/doc/specifications.md#envelopes
 _rntuple_feature_flag_format = struct.Struct("<Q")
-_rntuple_num_bytes_fields = struct.Struct("<II")
-_rntuple_field_description = struct.Struct("<IIIHH")
+_rntuple_env_header_format = struct.Struct("<Q")
+_rntuple_field_description_format = struct.Struct("<IIIHH")
+_rntuple_repetition_format = struct.Struct("<Q")
 _rntuple_column_record_format = struct.Struct("<HHII")
-_rntuple_alias_column = struct.Struct("<II")
-_rntuple_extra_type_info = struct.Struct("<III")
-_rntuple_record_size_format = struct.Struct("<I")
-_rntuple_frame_header = struct.Struct("<ii")
-_rntuple_cluster_group_format = struct.Struct("<I")
+_rntuple_alias_column_format = struct.Struct("<II")
+_rntuple_extra_type_info_format = struct.Struct("<III")
+_rntuple_record_size_format = struct.Struct("<q")
+_rntuple_frame_header_format = struct.Struct("<qi")
+_rntuple_cluster_group_format = struct.Struct("<qqi")
 _rntuple_locator_format = struct.Struct("<iQ")
 _rntuple_cluster_summary_format = struct.Struct("<QQ")
+_rntuple_checksum_format = struct.Struct("<Q")
+_rntuple_envlink_size_format = struct.Struct("<Q")
+_rntuple_page_num_elements_format = struct.Struct("<I")
+_rntuple_column_group_id_format = struct.Struct("<I")
 
 
 def from_zigzag(n):
     return n >> 1 ^ -(n & 1)
 
 
 def _envelop_header(chunk, cursor, context):
-    env_version, min_version = cursor.fields(
-        chunk, uproot.const._rntuple_frame_format, context
-    )
-    return {"env_version": env_version, "min_version": min_version}
+    env_data = cursor.field(chunk, _rntuple_env_header_format, context)
+    env_type_id = env_data & 0xFFFF
+    env_length = env_data >> 16
+    return {"env_type_id": env_type_id, "env_length": env_length}
 
 
 class Model_ROOT_3a3a_Experimental_3a3a_RNTuple(uproot.model.Model):
     """
     A versionless :doc:`uproot.model.Model` for ``ROOT::Experimental::RNTuple``.
     """
 
@@ -64,25 +68,26 @@
         if self.is_memberwise:
             raise NotImplementedError(
                 f"""memberwise serialization of {type(self).__name__}
 in file {self.file.file_path}"""
             )
 
         (
-            self._members["fCheckSum"],
-            self._members["fVersion"],
-            self._members["fSize"],
+            self.members["fVersionEpoch"],
+            self.members["fVersionMajor"],
+            self.members["fVersionMinor"],
+            self.members["fVersionPatch"],
             self._members["fSeekHeader"],
             self._members["fNBytesHeader"],
             self._members["fLenHeader"],
             self._members["fSeekFooter"],
             self._members["fNBytesFooter"],
             self._members["fLenFooter"],
-            self._members["fReserved"],
-        ) = cursor.fields(chunk, _rntuple_format1, context)
+            self._members["fChecksum"],
+        ) = cursor.fields(chunk, _rntuple_anchor_format, context)
 
         self._header_chunk_ready = False
         self._footer_chunk_ready = False
         self._header, self._footer = None, None
 
         self._field_names = None
         self._column_records = None
@@ -139,15 +144,14 @@
             if not self._header_chunk_ready:
                 self._prepare_header_chunk()
             context = {}
             cursor = self._header_cursor.copy()
 
             h = HeaderReader().read(self._header_chunk, cursor, context)
             self._header = h
-            assert h.crc32 == zlib.crc32(self._header_chunk.raw_data[:-4])
 
         return self._header
 
     @property
     def field_names(self):
         if self._field_names is None:
             self._field_names = [r.field_name for r in self.header.field_records]
@@ -163,24 +167,23 @@
             if not self._footer_chunk_ready:
                 self._prepare_footer_chunk()
             cursor = self._footer_cursor.copy()
             context = {}
 
             f = FooterReader().read(self._footer_chunk, cursor, context)
             assert (
-                f.header_crc32 == self.header.crc32
-            ), f"crc32={self.header.crc32}, header_crc32={f.header_crc32}"
-            assert f.crc32 == zlib.crc32(self._footer_chunk.raw_data[:-4])
+                f.header_checksum == self.header.checksum
+            ), f"checksum={self.header.checksum}, header_checksum={f.header_checksum}"
             self._footer = f
 
         return self._footer
 
     @property
     def cluster_summaries(self):
-        return self.footer.cluster_summaries
+        return self.page_list_envelopes.cluster_summaries
 
     # FIXME
     @property
     def _length(self):
         return sum(x.num_entries for x in self.cluster_summaries)
 
     def __len__(self):
@@ -262,15 +265,15 @@
         ):
             # string field splits->2 in col records
             inner = self.base_col_form(
                 rel_crs[1], rel_crs_idxs[-1], parameters={"__array__": "char"}
             )
             form_key = f"column-{rel_crs_idxs[0]}"
             return ak.forms.ListOffsetForm(
-                "u32", inner, form_key=form_key, parameters={"__array__": "string"}
+                "i64", inner, form_key=form_key, parameters={"__array__": "string"}
             )
         else:
             raise (RuntimeError(f"Missing special case: {field_id}"))
 
     def field_form(self, this_id, seen):
         ak = uproot.extras.awkward()
 
@@ -418,15 +421,18 @@
             n_elements = page_desc.num_elements
             tracker_end = tracker + n_elements
             self.read_pagedesc(
                 res[tracker:tracker_end], page_desc, dtype_str, dtype, nbits, split
             )
             tracker = tracker_end
 
-        if dtype_byte <= uproot.const.rntuple_col_type_to_num_dict["index32"]:
+        if (
+            dtype_byte <= uproot.const.rntuple_col_type_to_num_dict["index32"]
+            or 14 <= dtype_byte <= 15
+        ):
             res = numpy.insert(res, 0, 0)  # for offsets
         zigzag = 26 <= dtype_byte <= 28
         delta = 14 <= dtype_byte <= 15
         if zigzag:
             res = from_zigzag(res)
         elif delta:
             res = numpy.cumsum(res)
@@ -453,63 +459,57 @@
         )
         stop_cluster_idx = numpy.searchsorted(cluster_starts, entry_stop, side="right")
         cluster_num_entries = numpy.sum(
             [c.num_entries for c in clusters[start_cluster_idx:stop_cluster_idx]]
         )
 
         self._alias_columns_dict = {
-            el.field_id: el.physical_id
-            for i, el in enumerate(self.header.alias_columns)
+            el.field_id: el.physical_id for el in self.header.alias_columns
         }
         self._column_records_dict = {}
-        self._column_records_dict = {
-            el.field_id: {
-                "rel_crs": [
-                    *(self._column_records_dict.get(el.field_id) or {}).get(
-                        "rel_crs", []
-                    ),
-                    el,
-                ],
-                "rel_crs_idxs": [
-                    *(self._column_records_dict.get(el.field_id) or {}).get(
-                        "rel_crs_idxs", []
-                    ),
-                    i,
-                ],
-            }
-            for i, el in enumerate(self.header.column_records)
-        }
+        self._column_records_idx_to_id = {}
+        for i, cr in enumerate(self.header.column_records):
+            if cr.field_id not in self._column_records_dict:
+                self._column_records_dict[cr.field_id] = {
+                    "rel_crs": [cr],
+                    "rel_crs_idxs": [i],
+                }
+            else:
+                self._column_records_dict[cr.field_id]["rel_crs"].append(cr)
+                self._column_records_dict[cr.field_id]["rel_crs_idxs"].append(i)
+            self._column_records_idx_to_id[i] = cr.field_id
 
         self._related_ids = defaultdict(list)
         for i, el in enumerate(self.header.field_records):
             if el.parent_field_id != i:
                 self._related_ids[el.parent_field_id].append(i)
 
         form = self.to_akform().select_columns(filter_names)
         # only read columns mentioned in the awkward form
         target_cols = []
         container_dict = {}
         _recursive_find(form, target_cols)
         for key in target_cols:
             if "column" in key:
                 key_nr = int(key.split("-")[1])
-                if key_nr in self._column_records_dict:
-                    id = key_nr
+                key_fid = self._column_records_idx_to_id[key_nr]
+                if key_fid in self._column_records_dict:
+                    id = key_fid
                 elif key_nr in self._alias_columns_dict:
-                    id = self._alias_columns_dict[key_nr]
+                    id = self._alias_columns_dict[key_fid]
                 else:
                     raise (
                         RuntimeError(
                             f"The key: {key} is missing both from the columns records and the alias columns."
                         )
                     )
 
                 dtype_byte = self._column_records_dict[id]["rel_crs"][0].type
                 content = self.read_col_pages(
-                    id, range(start_cluster_idx, stop_cluster_idx)
+                    key_nr, range(start_cluster_idx, stop_cluster_idx)
                 )
                 if dtype_byte == uproot.const.rntuple_col_type_to_num_dict["switch"]:
                     kindex, tags = _split_switch_bits(content)
                     container_dict[f"{key}-index"] = kindex
                     container_dict[f"{key}-tags"] = tags
                 else:
                     # don't distinguish data and offsets
@@ -541,50 +541,37 @@
     if hasattr(form, "content") and issubclass(type(form.content), ak.forms.Form):
         _recursive_find(form.content, res)
 
 
 class PageDescription:
     def read(self, chunk, cursor, context):
         out = MetaData(type(self).__name__)
-        out.num_elements = cursor.field(chunk, struct.Struct("<I"), context)
+        out.num_elements = cursor.field(
+            chunk, _rntuple_page_num_elements_format, context
+        )
         out.locator = LocatorReader().read(chunk, cursor, context)
         return out
 
 
-class PageLinkInner:
-    def read(self, chunk, cursor, context):
-        local_cursor = cursor.copy()
-        num_bytes, num_pages = local_cursor.fields(
-            chunk, _rntuple_frame_header, context
-        )
-        assert num_bytes < 0, f"num_bytes={num_bytes}"
-        cursor.skip(-num_bytes)
-        return [
-            PageDescription().read(chunk, local_cursor, context)
-            for _ in range(num_pages)
-        ]
-
-
 class PageLink:
     def __init__(self):
-        self.top_most_list = ListFrameReader(  # top-most list
-            ListFrameReader(PageLinkInner())  # outer list (inner list)
+        self.list_cluster_summaries = ListFrameReader(
+            RecordFrameReader(ClusterSummaryReader())
+        )
+        self.nested_page_locations = ListFrameReader(
+            ListFrameReader(ListFrameReader(PageDescription()))
         )
 
     def read(self, chunk, cursor, context):
         out = MetaData(type(self).__name__)
         out.env_header = _envelop_header(chunk, cursor, context)
-        local_cursor = cursor.copy()
-        num_bytes, num_items = cursor.fields(chunk, _rntuple_frame_header, context)
-        if num_items == 0:
-            return out
-        out.pagelinklist = self.top_most_list.read(chunk, local_cursor, context)
-        cursor.skip(-num_bytes - 8)
-        out.crc32 = cursor.field(chunk, struct.Struct("<I"), context)
-        assert zlib.crc32(chunk.raw_data[:-4]) == out.crc32
+        out.header_checksum = cursor.field(chunk, _rntuple_checksum_format, context)
+        out.cluster_summaries = self.list_cluster_summaries.read(chunk, cursor, context)
+        out.pagelinklist = self.nested_page_locations.read(chunk, cursor, context)
+        out.checksum = cursor.field(chunk, _rntuple_checksum_format, context)
         return out
 
 
 class LocatorReader:
     def read(self, chunk, cursor, context):
         out = MetaData("Locator")
         out.num_bytes, out.offset = cursor.fields(
@@ -592,15 +579,15 @@
         )
         return out
 
 
 class EnvLinkReader:
     def read(self, chunk, cursor, context):
         out = MetaData("EnvLink")
-        out.env_uncomp_size = cursor.field(chunk, struct.Struct("<I"), context)
+        out.env_uncomp_size = cursor.field(chunk, _rntuple_envlink_size_format, context)
         out.locator = LocatorReader().read(chunk, cursor, context)
         return out
 
 
 class MetaData:
     def __init__(self, name, **kwargs):
         self.__dict__["_name"] = name
@@ -627,82 +614,82 @@
 class RecordFrameReader:
     def __init__(self, payload):
         self.payload = payload
 
     def read(self, chunk, cursor, context):
         local_cursor = cursor.copy()
         num_bytes = local_cursor.field(chunk, _rntuple_record_size_format, context)
+        assert num_bytes >= 0, f"num_bytes={num_bytes}"
         cursor.skip(num_bytes)
         return self.payload.read(chunk, local_cursor, context)
 
 
 class ListFrameReader:
     def __init__(self, payload):
         self.payload = payload
 
     def read(self, chunk, cursor, context):
         local_cursor = cursor.copy()
         num_bytes, num_items = local_cursor.fields(
-            chunk, _rntuple_frame_header, context
+            chunk, _rntuple_frame_header_format, context
         )
         assert num_bytes < 0, f"num_bytes={num_bytes}"
         cursor.skip(-num_bytes)
         return [
             self.payload.read(chunk, local_cursor, context) for _ in range(num_items)
         ]
 
 
-# https://github.com/jblomer/root/blob/ntuple-binary-format-v1/tree/ntuple/v7/doc/specifications.md#field-description
+# https://github.com/root-project/root/blob/aa513463b0b512517370cb91cca025e53a8b13a2/tree/ntuple/v7/doc/specifications.md#field-description
 class FieldRecordReader:
     def read(self, chunk, cursor, context):
         out = MetaData("FieldRecordFrame")
         (
             out.field_version,
             out.type_version,
             out.parent_field_id,
             out.struct_role,
             out.flags,
-        ) = cursor.fields(chunk, _rntuple_field_description, context)
+        ) = cursor.fields(chunk, _rntuple_field_description_format, context)
         if out.flags == 0x0001:
-            out.repetition = cursor.field(chunk, struct.Struct("Q"), context)
+            out.repetition = cursor.field(chunk, _rntuple_repetition_format, context)
         else:
             out.repetition = 0
-
         out.field_name, out.type_name, out.type_alias, out.field_desc = (
-            cursor.rntuple_string(chunk, context) for i in range(4)
+            cursor.rntuple_string(chunk, context) for _ in range(4)
         )
         return out
 
 
-# https://github.com/jblomer/root/blob/ntuple-binary-format-v1/tree/ntuple/v7/doc/specifications.md#column-description
+# https://github.com/root-project/root/blob/aa513463b0b512517370cb91cca025e53a8b13a2/tree/ntuple/v7/doc/specifications.md#column-description
 class ColumnRecordReader:
     def read(self, chunk, cursor, context):
         out = MetaData("ColumnRecordFrame")
         out.type, out.nbits, out.field_id, out.flags = cursor.fields(
             chunk, _rntuple_column_record_format, context
         )
         return out
 
 
 class AliasColumnReader:
     def read(self, chunk, cursor, context):
         out = MetaData("AliasColumn")
 
         out.physical_id, out.field_id = cursor.fields(
-            chunk, _rntuple_alias_column, context
+            chunk, _rntuple_alias_column_format, context
         )
         return out
 
 
 class ExtraTypeInfoReader:
     def read(self, chunk, cursor, context):
         out = MetaData("ExtraTypeInfoReader")
 
         out.type_ver_from, out.type_ver_to, out.content_id = cursor.fields(
-            chunk, _rntuple_extra_type_info, context
+            chunk, _rntuple_extra_type_info_format, context
         )
         out.type_name = cursor.rntuple_string(chunk, context)
         return out
 
 
 class HeaderReader:
     def __init__(self):
@@ -719,44 +706,50 @@
             RecordFrameReader(ExtraTypeInfoReader())
         )
 
     def read(self, chunk, cursor, context):
         out = MetaData(type(self).__name__)
         out.env_header = _envelop_header(chunk, cursor, context)
         out.feature_flag = cursor.field(chunk, _rntuple_feature_flag_format, context)
-        out.rc_tag = cursor.field(chunk, struct.Struct("I"), context)
         out.name, out.ntuple_description, out.writer_identifier = (
             cursor.rntuple_string(chunk, context) for _ in range(3)
         )
 
         out.field_records = self.list_field_record_frames.read(chunk, cursor, context)
         out.column_records = self.list_column_record_frames.read(chunk, cursor, context)
         out.alias_columns = self.list_alias_column_frames.read(chunk, cursor, context)
         out.extra_type_infos = self.list_extra_type_info_reader.read(
             chunk, cursor, context
         )
-        out.crc32 = cursor.field(chunk, struct.Struct("<I"), context)
+        out.checksum = cursor.field(chunk, _rntuple_checksum_format, context)
 
         return out
 
     def read_extension_header(self, out, chunk, cursor, context):
         out.field_records = self.list_field_record_frames.read(chunk, cursor, context)
         out.column_records = self.list_column_record_frames.read(chunk, cursor, context)
         out.alias_columns = self.list_alias_column_frames.read(chunk, cursor, context)
         out.extra_type_infos = self.list_extra_type_info_reader.read(
             chunk, cursor, context
         )
         return out
 
 
+class ColumnGroupIDReader:
+    def read(self, chunk, cursor, context):
+        out = MetaData("ColumnGroupID")
+        out.col_id = cursor.field(chunk, _rntuple_column_group_id_format, context)
+        return out
+
+
 class ColumnGroupRecordReader:
     def read(self, chunk, cursor, context):
-        out = MetaData("ClusterSummaryRecord")
-        out.num_first_entry, out.num_entries = cursor.fields(
-            chunk, self._cluster_summary_format, context
+        out = MetaData("ColumnGroupRecord")
+        out.column_ids = ListFrameReader(RecordFrameReader(ColumnGroupIDReader())).read(
+            chunk, cursor, context
         )
         return out
 
 
 class ClusterSummaryReader:
     def read(self, chunk, cursor, context):
         out = MetaData("ClusterSummaryRecord")
@@ -765,23 +758,26 @@
         )
         return out
 
 
 class ClusterGroupRecordReader:
     def read(self, chunk, cursor, context):
         out = MetaData("ClusterGroupRecord")
-        out.num_clusters = cursor.field(chunk, _rntuple_cluster_group_format, context)
+        out.min_entry_num, out.entry_span, out.num_clusters = cursor.fields(
+            chunk, _rntuple_cluster_group_format, context
+        )
         out.page_list_link = EnvLinkReader().read(chunk, cursor, context)
         return out
 
 
 class RNTupleSchemaExtension:
     def read(self, chunk, cursor, context):
         out = MetaData(type(self).__name__)
-        out.size = cursor.field(chunk, struct.Struct("<I"), context)
+        out.size = cursor.field(chunk, _rntuple_record_size_format, context)
+        assert out.size >= 0, f"size={out.size}"
         out.field_records = ListFrameReader(
             RecordFrameReader(FieldRecordReader())
         ).read(chunk, cursor, context)
         out.column_records = ListFrameReader(
             RecordFrameReader(ColumnRecordReader())
         ).read(chunk, cursor, context)
         out.alias_records = ListFrameReader(
@@ -792,41 +788,38 @@
         ).read(chunk, cursor, context)
         return out
 
 
 class FooterReader:
     def __init__(self):
         self.extension_header_links = RNTupleSchemaExtension()
-        # self.extension_header_links = ListFrameReader(EnvLinkReader())
         self.column_group_record_frames = ListFrameReader(
             RecordFrameReader(ColumnGroupRecordReader())
         )
         self.cluster_summary_frames = ListFrameReader(
             RecordFrameReader(ClusterSummaryReader())
         )
         self.cluster_group_record_frames = ListFrameReader(
             RecordFrameReader(ClusterGroupRecordReader())
         )
-        self.meta_data_links = ListFrameReader(EnvLinkReader())
+        self.meta_data_links = ListFrameReader(RecordFrameReader(EnvLinkReader()))
 
     def read(self, chunk, cursor, context):
         out = MetaData("Footer")
         out.env_header = _envelop_header(chunk, cursor, context)
         out.feature_flag = cursor.field(chunk, _rntuple_feature_flag_format, context)
-        out.header_crc32 = cursor.field(chunk, struct.Struct("<I"), context)
+        out.header_checksum = cursor.field(chunk, _rntuple_checksum_format, context)
         out.extension_links = self.extension_header_links.read(chunk, cursor, context)
-
         out.col_group_records = self.column_group_record_frames.read(
             chunk, cursor, context
         )
-        out.cluster_summaries = self.cluster_summary_frames.read(chunk, cursor, context)
         out.cluster_group_records = self.cluster_group_record_frames.read(
             chunk, cursor, context
         )
         out.meta_block_links = self.meta_data_links.read(chunk, cursor, context)
-        out.crc32 = cursor.field(chunk, struct.Struct("<I"), context)
+        out.checksum = cursor.field(chunk, _rntuple_checksum_format, context)
         return out
 
 
 uproot.classes["ROOT::Experimental::RNTuple"] = (
     Model_ROOT_3a3a_Experimental_3a3a_RNTuple
 )
```

### Comparing `uproot-5.3.2rc1/src/uproot/models/TArray.py` & `uproot-5.3.3/src/uproot/models/TArray.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/models/TAtt.py` & `uproot-5.3.3/src/uproot/models/TAtt.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/models/TBasket.py` & `uproot-5.3.3/src/uproot/models/TBasket.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,17 +27,15 @@
     Since this model is versionless and most of its functionality is internal
     (not to be directly accessed by most users), it is defined on the model
     instead of creating a behavior class to mix in functionality.
     """
 
     def __repr__(self):
         basket_num = self._basket_num if self._basket_num is not None else "(unknown)"
-        return "<TBasket {} of {} at 0x{:012x}>".format(
-            basket_num, repr(self._parent.name), id(self)
-        )
+        return f"<TBasket {basket_num} of {self._parent.name!r} at 0x{id(self):012x}>"
 
     @property
     def raw_data(self):
         """
         The raw but uncompressed data in the ``TBasket``, which combines data
         content with entry offsets, if the latter exists.
```

### Comparing `uproot-5.3.2rc1/src/uproot/models/TBranch.py` & `uproot-5.3.3/src/uproot/models/TBranch.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/models/TClonesArray.py` & `uproot-5.3.3/src/uproot/models/TClonesArray.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,17 +18,15 @@
     """
 
     def read_members(self, chunk, cursor, context, file):
         if uproot._awkwardforth.get_forth_obj(context) is not None:
             raise uproot.interpretation.objects.CannotBeForth()
         if self.is_memberwise:
             raise NotImplementedError(
-                "memberwise serialization of {}\nin file {}".format(
-                    type(self).__name__, self.file.file_path
-                )
+                f"memberwise serialization of {type(self).__name__}\nin file {self.file.file_path}"
             )
 
         self._bases.append(
             uproot.models.TObject.Model_TObject.read(
                 chunk,
                 cursor,
                 context,
```

### Comparing `uproot-5.3.2rc1/src/uproot/models/TDatime.py` & `uproot-5.3.3/src/uproot/models/TDatime.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/models/TGraph.py` & `uproot-5.3.3/src/uproot/models/TGraph.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,17 +35,15 @@
     behaviors = (uproot.behaviors.TGraph.TGraph,)
 
     def read_members(self, chunk, cursor, context, file):
         if uproot._awkwardforth.get_forth_obj(context) is not None:
             raise uproot.interpretation.objects.CannotBeForth()
         if self.is_memberwise:
             raise NotImplementedError(
-                "memberwise serialization of {}\nin file {}".format(
-                    type(self).__name__, self.file.file_path
-                )
+                f"memberwise serialization of {type(self).__name__}\nin file {self.file.file_path}"
             )
         self._bases.append(
             file.class_named("TNamed", 1).read(
                 chunk,
                 cursor,
                 context,
                 file,
@@ -363,17 +361,15 @@
     behaviors = (uproot.behaviors.TGraphErrors.TGraphErrors,)
 
     def read_members(self, chunk, cursor, context, file):
         if uproot._awkwardforth.get_forth_obj(context) is not None:
             raise uproot.interpretation.objects.CannotBeForth()
         if self.is_memberwise:
             raise NotImplementedError(
-                "memberwise serialization of {}\nin file {}".format(
-                    type(self).__name__, self.file.file_path
-                )
+                f"memberwise serialization of {type(self).__name__}\nin file {self.file.file_path}"
             )
         self._bases.append(
             file.class_named("TGraph", 4).read(
                 chunk,
                 cursor,
                 context,
                 file,
@@ -545,17 +541,15 @@
     behaviors = (uproot.behaviors.TGraphAsymmErrors.TGraphAsymmErrors,)
 
     def read_members(self, chunk, cursor, context, file):
         if uproot._awkwardforth.get_forth_obj(context) is not None:
             raise uproot.interpretation.objects.CannotBeForth()
         if self.is_memberwise:
             raise NotImplementedError(
-                "memberwise serialization of {}\nin file {}".format(
-                    type(self).__name__, self.file.file_path
-                )
+                f"memberwise serialization of {type(self).__name__}\nin file {self.file.file_path}"
             )
         self._bases.append(
             file.class_named("TGraph", 4).read(
                 chunk,
                 cursor,
                 context,
                 file,
```

### Comparing `uproot-5.3.2rc1/src/uproot/models/TH.py` & `uproot-5.3.3/src/uproot/models/TH.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/models/THashList.py` & `uproot-5.3.3/src/uproot/models/THashList.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/models/TLeaf.py` & `uproot-5.3.3/src/uproot/models/TLeaf.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/models/TList.py` & `uproot-5.3.3/src/uproot/models/TList.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/models/TMatrixT.py` & `uproot-5.3.3/src/uproot/models/TMatrixT.py`

 * *Files 4% similar despite different names*

```diff
@@ -22,17 +22,15 @@
     """
 
     def read_members(self, chunk, cursor, context, file):
         if uproot._awkwardforth.get_forth_obj(context) is not None:
             raise uproot.interpretation.objects.CannotBeForth()
         if self.is_memberwise:
             raise NotImplementedError(
-                "memberwise serialization of {}\nin file {}".format(
-                    type(self).__name__, self.file.file_path
-                )
+                f"memberwise serialization of {type(self).__name__}\nin file {self.file.file_path}"
             )
         self._bases.append(
             file.class_named("TObject", 1).read(
                 chunk,
                 cursor,
                 context,
                 file,
```

### Comparing `uproot-5.3.2rc1/src/uproot/models/TNamed.py` & `uproot-5.3.3/src/uproot/models/TNamed.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/models/TObjArray.py` & `uproot-5.3.3/src/uproot/models/TObjArray.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/models/TObjString.py` & `uproot-5.3.3/src/uproot/models/TObjString.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/models/TObject.py` & `uproot-5.3.3/src/uproot/models/TObject.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/models/TRef.py` & `uproot-5.3.3/src/uproot/models/TRef.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/models/TString.py` & `uproot-5.3.3/src/uproot/models/TString.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/models/TTable.py` & `uproot-5.3.3/src/uproot/models/TTable.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/models/TTree.py` & `uproot-5.3.3/src/uproot/models/TTree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/models/__init__.py` & `uproot-5.3.3/src/uproot/models/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/sink/__init__.py` & `uproot-5.3.3/src/uproot/sink/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/sink/file.py` & `uproot-5.3.3/src/uproot/sink/file.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,22 +194,14 @@
         """
         self._ensure()
         self._file.seek(location)
         out = self._file.read(num_bytes)
         if insist is True:
             if len(out) != num_bytes:
                 raise OSError(
-                    "could not read {} bytes from the file at position {}{}".format(
-                        num_bytes,
-                        location,
-                        self.in_path,
-                    )
+                    f"could not read {num_bytes} bytes from the file at position {location}{self.in_path}"
                 )
         elif isinstance(insist, numbers.Integral) and len(out) < insist:
             raise OSError(
-                "could not read {} bytes from the file at position {}{}".format(
-                    insist,
-                    location,
-                    self.in_path,
-                )
+                f"could not read {insist} bytes from the file at position {location}{self.in_path}"
             )
         return out
```

### Comparing `uproot-5.3.2rc1/src/uproot/source/__init__.py` & `uproot-5.3.3/src/uproot/source/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/source/chunk.py` & `uproot-5.3.3/src/uproot/source/chunk.py`

 * *Files 1% similar despite different names*

```diff
@@ -183,17 +183,15 @@
     :doc:`uproot.source.futures.ResourceThreadPoolExecutor`.
     """
 
     def __repr__(self):
         path = repr(self._file_path)
         if len(self._file_path) > 10:
             path = repr("..." + self._file_path[-10:])
-        return "<{} {} ({} workers) at 0x{:012x}>".format(
-            type(self).__name__, path, self.num_workers, id(self)
-        )
+        return f"<{type(self).__name__} {path} ({self.num_workers} workers) at 0x{id(self):012x}>"
 
     def chunk(self, start: int, stop: int) -> Chunk:
         self._num_requests += 1
         self._num_requested_chunks += 1
         self._num_requested_bytes += stop - start
 
         future = self.ResourceClass.future(self, start, stop)
```

### Comparing `uproot-5.3.2rc1/src/uproot/source/cursor.py` & `uproot-5.3.3/src/uproot/source/cursor.py`

 * *Files 0% similar despite different names*

```diff
@@ -382,15 +382,15 @@
         length = chunk.get(start, stop, self, context)[0]
         if length == 255:
             start = stop
             stop = start + 4
             length_data = chunk.get(start, stop, self, context)
             length = numpy.frombuffer(length_data, dtype=self._u1).view(self._i4)[0]
         start = stop
-        stop = start + length
+        stop = start + int(length)
         if move:
             self._index = stop
         return uproot._util.tobytes(chunk.get(start, stop, self, context))
 
     def string(
         self, chunk: uproot.source.chunk.Chunk, context: dict, move: bool = True
     ) -> str:
@@ -482,18 +482,16 @@
         """
         remainder = chunk.remainder(self._index, self, context)
         local_stop = 0
         char = None
         while char != 0:
             if local_stop > len(remainder):
                 raise OSError(
-                    """C-style string has no terminator (null byte) in Chunk {}:{}
-of file path {}""".format(
-                        self._start, self._stop, self._source.file_path
-                    )
+                    f"""C-style string has no terminator (null byte) in Chunk {self._start}:{self._stop}
+of file path {self._source.file_path}"""
                 )
             char = remainder[local_stop]
             local_stop += 1
 
         if move:
             self._index += local_stop
```

### Comparing `uproot-5.3.2rc1/src/uproot/source/file.py` & `uproot-5.3.3/src/uproot/source/file.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/source/fsspec.py` & `uproot-5.3.3/src/uproot/source/fsspec.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/source/futures.py` & `uproot-5.3.3/src/uproot/source/futures.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/source/http.py` & `uproot-5.3.3/src/uproot/source/http.py`

 * *Files 3% similar despite different names*

```diff
@@ -103,44 +103,38 @@
                 connection.request(
                     "HEAD", full_path(redirect_url), headers=auth_headers
                 )
                 response = connection.getresponse()
                 break
         else:
             raise http.client.HTTPException(
-                """remote server responded with status {} (redirect) without a 'location'
-for URL {}""".format(
-                    response.status, file_path
-                )
+                f"""remote server responded with status {response.status} (redirect) without a 'location'
+for URL {file_path}"""
             )
 
     if response.status == 404:
         connection.close()
         raise uproot._util._file_not_found(file_path, "HTTP(S) returned 404")
 
     if response.status != 200:
         connection.close()
         raise http.client.HTTPException(
-            """HTTP response was {}, rather than 200, in attempt to get file size
-in file {}""".format(
-                response.status, file_path
-            )
+            f"""HTTP response was {response.status}, rather than 200, in attempt to get file size
+in file {file_path}"""
         )
 
     for k, x in response.getheaders():
         if k.lower() == "content-length" and x.strip() != "0":
             connection.close()
             return int(x)
     else:
         connection.close()
         raise http.client.HTTPException(
-            """response headers did not include content-length: {}
-in file {}""".format(
-                dict(response.getheaders()), file_path
-            )
+            f"""response headers did not include content-length: {dict(response.getheaders())}
+in file {file_path}"""
         )
 
 
 class HTTPResource(uproot.source.chunk.Resource):
     """
     Args:
         file_path (str): A URL of the file to open.
@@ -213,27 +207,23 @@
                         headers=dict(
                             {"Range": f"bytes={start}-{stop - 1}"}, **self.auth_headers
                         ),
                     )
                     return self.get(redirect, start, stop)
 
             raise http.client.HTTPException(
-                """remote server responded with status {} (redirect) without a 'location'
-for URL {}""".format(
-                    response.status, self._file_path
-                )
+                f"""remote server responded with status {response.status} (redirect) without a 'location'
+for URL {self._file_path}"""
             )
 
         if response.status != 206:
             connection.close()
             raise http.client.HTTPException(
-                """remote server responded with status {}, rather than 206 (range requests)
-for URL {}""".format(
-                    response.status, self._file_path
-                )
+                f"""remote server responded with status {response.status}, rather than 206 (range requests)
+for URL {self._file_path}"""
             )
         try:
             return response.read()
         finally:
             connection.close()
 
     @staticmethod
@@ -319,18 +309,16 @@
                                     **source.auth_headers,
                                 },
                             )
                             task(resource)
                             return
 
                     raise http.client.HTTPException(
-                        """remote server responded with status {} (redirect) without a 'location'
-for URL {}""".format(
-                            response.status, source.file_path
-                        )
+                        f"""remote server responded with status {response.status} (redirect) without a 'location'
+for URL {source.file_path}"""
                     )
 
                 multipart_supported = resource.is_multipart_supported(ranges, response)
 
                 if not multipart_supported:
                     resource.handle_no_multipart(source, ranges, futures, results)
                 else:
@@ -425,19 +413,17 @@
             stop = last + 1
 
             length = stop - start
             data = response_buffer.read(length)
 
             if len(data) != length:
                 raise http.client.HTTPException(
-                    """wrong chunk length {} (expected {}) for byte range {} "
+                    f"""wrong chunk length {len(data)} (expected {length}) for byte range {range_string.decode()!r} "
                     "in HTTP multipart
-for URL {}""".format(
-                        len(data), length, repr(range_string.decode()), self._file_path
-                    )
+for URL {self._file_path}"""
                 )
 
             found = futures.pop((start, stop), None)
 
             if found is not None:
                 results[start, stop] = data
                 found._run(self)
@@ -451,21 +437,19 @@
                     ) in futures:
                         if now == future_start:
                             break
                     else:
                         range_string = range_string.decode("utf-8", "surrogateescape")
                         expecting = ", ".join(f"{a}-{b - 1}" for a, b in futures)
                         raise http.client.HTTPException(
-                            """unrecognized byte range in headers of HTTP multipart: {}
+                            f"""unrecognized byte range in headers of HTTP multipart: {range_string!r}
 
-    expecting: {}
+    expecting: {expecting}
 
-for URL {}""".format(
-                                repr(range_string), expecting, self._file_path
-                            )
+for URL {self._file_path}"""
                         )
                     subdata = data[
                         now - start : now + future_stop - future_start - start
                     ]
                     found = futures.pop((future_start, future_stop))
                     results[future_start, future_stop] = subdata
                     found._run(self)
```

### Comparing `uproot-5.3.2rc1/src/uproot/source/object.py` & `uproot-5.3.3/src/uproot/source/object.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/source/s3.py` & `uproot-5.3.3/src/uproot/source/s3.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/source/xrootd.py` & `uproot-5.3.3/src/uproot/source/xrootd.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/writing/__init__.py` & `uproot-5.3.3/src/uproot/writing/__init__.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/writing/_cascade.py` & `uproot-5.3.3/src/uproot/writing/_cascade.py`

 * *Files 3% similar despite different names*

```diff
@@ -214,26 +214,15 @@
         self._cycle = cycle
         self._parent_location = parent_location
         self._seek_location = seek_location
         self._created_on = datetime.datetime.now() if created_on is None else created_on
         self._big = big
 
     def __repr__(self):
-        return "{}({}, {}, {}, {}, {}, {}, {}, {}, {})".format(
-            type(self).__name__,
-            self._location,
-            self._uncompressed_bytes,
-            self._compressed_bytes,
-            repr(self._classname),
-            repr(self._name),
-            repr(self._title),
-            self._cycle,
-            self._parent_location,
-            self._seek_location,
-        )
+        return f"{type(self).__name__}({self._location}, {self._uncompressed_bytes}, {self._compressed_bytes}, {self._classname!r}, {self._name!r}, {self._title!r}, {self._cycle}, {self._parent_location}, {self._seek_location})"
 
     @property
     def allocation(self):
         return self.num_bytes
 
     @property
     def uncompressed_bytes(self):
@@ -421,19 +410,15 @@
             )
             version -= 1000
             position = location + uproot.reading._key_format_big.size
             big = True
 
         if version != cls.class_version:
             raise ValueError(
-                "Uproot can't read TKey version {} for writing, only version {}{}".format(
-                    version,
-                    cls.class_version,
-                    in_path,
-                )
+                f"Uproot can't read TKey version {version} for writing, only version {cls.class_version}{in_path}"
             )
 
         assert 0 < fNbytes <= fKeylen + fObjlen
         assert fCycle > 0
         if not is_directory_key:
             assert fSeekKey == location, f"fSeekKey {fSeekKey} location {location}"
             fSeekKey = None
@@ -577,19 +562,15 @@
                 version -= 1000
                 position += _free_format_big.size
             else:
                 position += _free_format_small.size
 
             if version != cls.class_version:
                 raise ValueError(
-                    "Uproot can't read TFree version {} for writing, only version {}{}".format(
-                        version,
-                        cls.class_version,
-                        in_path,
-                    )
+                    f"Uproot can't read TFree version {version} for writing, only version {cls.class_version}{in_path}"
                 )
 
             slices.append((fFirst, fLast + 1))
 
         end = slices.pop()[0]
 
         assert position == num_bytes
@@ -691,17 +672,15 @@
 
     @staticmethod
     def _another_slice(slices, original_start, original_stop):
         for start, stop in slices:
             if start <= original_start < stop or start < original_stop <= stop:
                 raise RuntimeError(
                     "segment of data to release overlaps one already marked as free: "
-                    "releasing [{}, {}) but [{}, {}) is free".format(
-                        original_start, original_stop, start, stop
-                    )
+                    f"releasing [{original_start}, {original_stop}) but [{start}, {stop}) is free"
                 )
 
         for i in range(len(slices) - 1):
             if slices[i][1] == original_start and original_stop == slices[i + 1][0]:
                 # These two slices need to be merged, including the newly released interval.
                 return (
                     slices[:i] + ((slices[i][0], slices[i + 1][1]),) + slices[i + 2 :]
@@ -796,17 +775,15 @@
 
     def __init__(self, location, data_bytes, num_entries):
         super().__init__(location, _tlistheader_format.size)
         self._data_bytes = data_bytes
         self._num_entries = num_entries
 
     def __repr__(self):
-        return "{}({}, {}, {})".format(
-            type(self).__name__, self._location, self._data_bytes, self._num_entries
-        )
+        return f"{type(self).__name__}({self._location}, {self._data_bytes}, {self._num_entries})"
 
     @property
     def data_bytes(self):
         return self._data_bytes
 
     @data_bytes.setter
     def data_bytes(self, value):
@@ -858,21 +835,15 @@
         return self._name
 
     @property
     def class_version(self):
         return self._class_version
 
     def __repr__(self):
-        return "{}({}, {}, {}, {})".format(
-            type(self).__name__,
-            self._location,
-            self._serialization,
-            repr(self._name),
-            self._class_version,
-        )
+        return f"{type(self).__name__}({self._location}, {self._serialization}, {self._name!r}, {self._class_version})"
 
     def copy_to(self, location):
         return RawStreamerInfo(
             location, self._serialization, self._name, self._class_version
         )
 
     def serialize(self):
@@ -919,22 +890,15 @@
         self._lookup = {
             (x.name, x.class_version)
             for x in self._rawstreamers
             if not isinstance(x, RawTListOfStrings)
         }
 
     def __repr__(self):
-        return "{}({}, {}, {}, {}, {})".format(
-            type(self).__name__,
-            self._allocation,
-            self._key,
-            self._header,
-            self._rawstreamers,
-            self._freesegments,
-        )
+        return f"{type(self).__name__}({self._allocation}, {self._key}, {self._header}, {self._rawstreamers}, {self._freesegments})"
 
     @property
     def allocation(self):
         return self._allocation
 
     @property
     def num_bytes(self):
@@ -1151,19 +1115,16 @@
         for key in keys:
             if key.name.string not in self._keys_by_name:
                 self._keys_by_name[key.name.string] = []
             self._keys_by_name[key.name.string].append(key)
         self._keys = keys
 
     def __repr__(self):
-        return "{}({}, {}, {})".format(
-            type(self).__name__,
-            self._location,
-            self._allocation,
-            self._keys,
+        return (
+            f"{type(self).__name__}({self._location}, {self._allocation}, {self._keys})"
         )
 
     @property
     def allocation(self):
         if self._allocation is None:
             self._allocation = self.num_bytes
         return self._allocation
@@ -1363,24 +1324,15 @@
         self._data_num_bytes = data_num_bytes
         self._parent_location = parent_location
         self._uuid = uuid
         self._created_on = datetime.datetime.now()
         self._modified_on = self._created_on
 
     def __repr__(self):
-        return "{}({}, {}, {}, {}, {}, {}, {})".format(
-            type(self).__name__,
-            self._location,
-            self._begin_location,
-            self._begin_num_bytes,
-            self._data_location,
-            self._data_num_bytes,
-            self._parent_location,
-            repr(self._uuid),
-        )
+        return f"{type(self).__name__}({self._location}, {self._begin_location}, {self._begin_num_bytes}, {self._data_location}, {self._data_num_bytes}, {self._parent_location}, {self._uuid!r})"
 
     @property
     def begin_location(self):
         return self._begin_location
 
     @begin_location.setter
     def begin_location(self, value):
@@ -1506,19 +1458,15 @@
                 raw_bytes[: uproot.reading._directory_format_big.size]
             )
             version -= 1000
             position = location + uproot.reading._directory_format_big.size
 
         if version != cls.class_version:
             raise ValueError(
-                "Uproot can't read TDirectory version {} for writing, only version {}{}".format(
-                    version,
-                    cls.class_version,
-                    in_path,
-                )
+                f"Uproot can't read TDirectory version {version} for writing, only version {cls.class_version}{in_path}"
             )
 
         # TUUID version 1
         assert raw_bytes[position - location : position - location + 2] == b"\x00\x01"
         uuid_bytes = raw_bytes[position - location + 2 : position - location + 18]
 
         out = DirectoryHeader(
@@ -1854,24 +1802,15 @@
         self._title = title
         self._header = header
         self._datakey = datakey
         self._data = data
         self._freesegments = freesegments
 
     def __repr__(self):
-        return "{}({}, {}, {}, {}, {}, {}, {})".format(
-            type(self).__name__,
-            self._key,
-            self._name,
-            self._title,
-            self._header,
-            self._datakey,
-            self._data,
-            self._freesegments,
-        )
+        return f"{type(self).__name__}({self._key}, {self._name}, {self._title}, {self._header}, {self._datakey}, {self._data}, {self._freesegments})"
 
     @property
     def key(self):
         return self._key
 
     @property
     def name(self):
@@ -1938,23 +1877,15 @@
         self._header = header
         self._datakey = datakey
         self._data = data
         self._parent = parent
         self._freesegments = freesegments
 
     def __repr__(self):
-        return "{}({}, {}, {}, {}, {}, {})".format(
-            type(self).__name__,
-            self._key,
-            self._header,
-            self._datakey,
-            self._data,
-            self._parent,
-            self._freesegments,
-        )
+        return f"{type(self).__name__}({self._key}, {self._header}, {self._datakey}, {self._data}, {self._parent}, {self._freesegments})"
 
     @property
     def key(self):
         return self._key
 
     @property
     def header(self):
@@ -2035,26 +1966,15 @@
         self._info_location = info_location
         self._info_num_bytes = info_num_bytes
         self._uuid = uuid
         self._version = None
         self._begin = 100
 
     def __repr__(self):
-        return "{}({}, {}, {}, {}, {}, {}, {}, {}, {})".format(
-            type(self).__name__,
-            self._end,
-            self._free_location,
-            self._free_num_bytes,
-            self._free_num_slices,
-            self._begin_num_bytes,
-            repr(self._compression),
-            self._info_location,
-            self._info_num_bytes,
-            repr(self._uuid),
-        )
+        return f"{type(self).__name__}({self._end}, {self._free_location}, {self._free_num_bytes}, {self._free_num_slices}, {self._begin_num_bytes}, {self._compression!r}, {self._info_location}, {self._info_num_bytes}, {self._uuid!r})"
 
     @property
     def end(self):
         return self._end
 
     @end.setter
     def end(self, value):
@@ -2286,21 +2206,15 @@
         self._fileheader = fileheader
         self._streamers = streamers
         self._freesegments = freesegments
         self._rootdirectory = rootdirectory
         self._tlist_of_streamers = tlist_of_streamers
 
     def __repr__(self):
-        return "{}({}, {}, {}, {})".format(
-            type(self).__name__,
-            self._fileheader,
-            self._streamers,
-            self._freesegments,
-            self._rootdirectory,
-        )
+        return f"{type(self).__name__}({self._fileheader}, {self._streamers}, {self._freesegments}, {self._rootdirectory})"
 
     @property
     def fileheader(self):
         return self._fileheader
 
     @property
     def streamers(self):
```

### Comparing `uproot-5.3.2rc1/src/uproot/writing/_cascadentuple.py` & `uproot-5.3.3/src/uproot/writing/_cascadentuple.py`

 * *Files 3% similar despite different names*

```diff
@@ -19,20 +19,20 @@
 
 import uproot
 import uproot.compression
 import uproot.const
 import uproot.reading
 import uproot.serialization
 from uproot.models.RNTuple import (
+    _rntuple_anchor_format,
     _rntuple_cluster_group_format,
     _rntuple_cluster_summary_format,
     _rntuple_column_record_format,
     _rntuple_feature_flag_format,
-    _rntuple_field_description,
-    _rntuple_format1,
+    _rntuple_field_description_format,
     _rntuple_locator_format,
     _rntuple_record_size_format,
 )
 from uproot.writing._cascade import CascadeLeaf, CascadeNode, Key, String
 
 _ak_primitive_to_typename_dict = {
     "i64": "std::int64_t",
@@ -166,29 +166,18 @@
         self.flags = flags
         self.field_name = field_name
         self.type_name = type_name
         self.type_alias = type_alias
         self.field_description = field_description
 
     def __repr__(self):
-        return "{}({}, {}, {}, {}, {}, {}, {}, {}, {})".format(
-            type(self).__name__,
-            repr(self.field_version),
-            repr(self.type_version),
-            repr(self.parent_field_id),
-            repr(self.struct_role),
-            repr(self.flags),
-            repr(self.field_name),
-            repr(self.type_name),
-            repr(self.type_alias),
-            repr(self.field_description),
-        )
+        return f"{type(self).__name__}({self.field_version!r}, {self.type_version!r}, {self.parent_field_id!r}, {self.struct_role!r}, {self.flags!r}, {self.field_name!r}, {self.type_name!r}, {self.type_alias!r}, {self.field_description!r})"
 
     def serialize(self):
-        header_bytes = _rntuple_field_description.pack(
+        header_bytes = _rntuple_field_description_format.pack(
             self.field_version,
             self.type_version,
             self.parent_field_id,
             self.struct_role,
             self.flags,
         )
         string_bytes = b"".join(
@@ -352,22 +341,15 @@
             NTuple_ClusterGroupRecord(0, NTuple_EnvLink(16, None))
         ]
         self.metadata_block_envelope_links = []
 
         super().__init__(location, None)
 
     def __repr__(self):
-        return "{}(extension_header_env_links = {}, column_group_record_frames = {}, cluster_summary_record_frames={}, cluster_group_record_frames{}, metadata_block_envelope_link = {})".format(
-            type(self).__name__,
-            self.extension_header_envelope_links,
-            self.column_group_record_frames,
-            self.cluster_summary_record_frames,
-            self.cluster_group_record_frames,
-            self.metadata_block_envelope_links,
-        )
+        return f"{type(self).__name__}(extension_header_env_links = {self.extension_header_envelope_links}, column_group_record_frames = {self.column_group_record_frames}, cluster_summary_record_frames={self.cluster_summary_record_frames}, cluster_group_record_frames{self.cluster_group_record_frames}, metadata_block_envelope_link = {self.metadata_block_envelope_links})"
 
     def serialize(self):
         env_header = uproot.const.rntuple_env_header
         out = []
         out.extend(
             [
                 env_header,
@@ -493,15 +475,15 @@
         fNBytesHeader,
         fLenHeader,
         fSeekFooter,
         fNBytesFooter,
         fLenFooter,
         fReserved,
     ):
-        aloc = _rntuple_format1.size
+        aloc = _rntuple_anchor_format.size
         super().__init__(location, aloc)
         self.fCheckSum = fCheckSum
         self.fVersion = fVersion
         self.fSize = fSize
         self.fSeekHeader = fSeekHeader
         self.fNBytesHeader = fNBytesHeader
         self.fLenHeader = fLenHeader
@@ -531,20 +513,20 @@
             self._location,
             ", ".join([repr(x) for x in self._fields]),
         )
 
     def serialize(self):
         # hardcoded unless version changes
         # version = 0
-        # aloc = _rntuple_format1.size
+        # aloc = _rntuple_anchor_format.size
         # uproot.serialization.numbytes_version(aloc, version)
-        out = _rntuple_format1.pack(*self._fields)
+        out = _rntuple_anchor_format.pack(*self._fields)
         crc32 = zlib.crc32(out)
         self.fCheckSum = crc32
-        out = _rntuple_format1.pack(*self._fields)
+        out = _rntuple_anchor_format.pack(*self._fields)
         return b"@\x00\x006\x00\x03" + out
 
 
 class Ntuple_PageLink:
     def __init__(self, num_bytes, offset):
         self.num_bytes = num_bytes
         self.offset = offset
@@ -595,25 +577,15 @@
         self._freesegments = freesegments
 
         self._key = None
         self._header_key = None
         self._num_entries = 0
 
     def __repr__(self):
-        return "{}({}, {}, {}, {}, {}, {}, {}, {})".format(
-            type(self).__name__,
-            self._directory,
-            self._name,
-            self._title,
-            self._header,
-            self._footer,
-            self._cluster_metadata,
-            self._anchor,
-            self._freesegments,
-        )
+        return f"{type(self).__name__}({self._directory}, {self._name}, {self._title}, {self._header}, {self._footer}, {self._cluster_metadata}, {self._anchor}, {self._freesegments})"
 
     @property
     def directory(self):
         return self._directory
 
     @property
     def key(self):
```

### Comparing `uproot-5.3.2rc1/src/uproot/writing/_cascadetree.py` & `uproot-5.3.3/src/uproot/writing/_cascadetree.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,15 +119,15 @@
                 try:
                     if uproot._util.from_module(branch_type, "awkward"):
                         raise TypeError
                     if isinstance(branch_type, str) and branch_type.strip() == "bytes":
                         raise TypeError
                     branch_dtype = numpy.dtype(branch_type)
 
-                except TypeError as err:
+                except (TypeError, ValueError) as err:
                     try:
                         awkward = uproot.extras.awkward()
                     except ModuleNotFoundError as err:
                         raise TypeError(
                             f"not a NumPy dtype and 'awkward' cannot be imported: {branch_type!r}"
                         ) from err
                     if isinstance(
@@ -162,17 +162,15 @@
 
                     for key, content in branch_dict.items():
                         subname = self._field_name(branch_name, key)
                         try:
                             dtype = numpy.dtype(content)
                         except Exception as err:
                             raise TypeError(
-                                "values of a dict must be NumPy types\n\n    key {} has type {}".format(
-                                    repr(key), repr(content)
-                                )
+                                f"values of a dict must be NumPy types\n\n    key {key!r} has type {content!r}"
                             ) from err
                         self._branch_lookup[subname] = len(self._branch_data)
                         self._branch_data.append(
                             self._branch_np(subname, content, dtype)
                         )
 
             elif branch_dtype is not None:
@@ -230,17 +228,15 @@
                             )
 
                             for key, cont in zip(keys, contents):
                                 subname = self._field_name(branch_name, key)
                                 dtype = self._branch_ak_to_np(cont)
                                 if dtype is None:
                                     raise TypeError(
-                                        "fields of a record must be NumPy types, though the record itself may be in a jagged array\n\n    field {} has type {}".format(
-                                            repr(key), str(cont)
-                                        )
+                                        f"fields of a record must be NumPy types, though the record itself may be in a jagged array\n\n    field {key!r} has type {cont!s}"
                                     )
                                 if subname not in self._branch_lookup:
                                     self._branch_lookup[subname] = len(
                                         self._branch_data
                                     )
                                     self._branch_data.append(
                                         self._branch_np(
@@ -248,17 +244,15 @@
                                         )
                                     )
 
                     else:
                         dt = self._branch_ak_to_np(content)
                         if dt is None:
                             raise TypeError(
-                                "cannot write Awkward Array type to ROOT file:\n\n    {}".format(
-                                    str(branch_datashape)
-                                )
+                                f"cannot write Awkward Array type to ROOT file:\n\n    {branch_datashape!s}"
                             )
                         if branch_name not in self._branch_lookup:
                             self._branch_lookup[branch_name] = len(self._branch_data)
                             self._branch_data.append(
                                 self._branch_np(branch_name, dt, dt, counter=counter)
                             )
 
@@ -280,29 +274,25 @@
                         )
 
                         for key, content in zip(keys, contents):
                             subname = self._field_name(branch_name, key)
                             dtype = self._branch_ak_to_np(content)
                             if dtype is None:
                                 raise TypeError(
-                                    "fields of a record must be NumPy types, though the record itself may be in a jagged array\n\n    field {} has type {}".format(
-                                        repr(key), str(content)
-                                    )
+                                    f"fields of a record must be NumPy types, though the record itself may be in a jagged array\n\n    field {key!r} has type {content!s}"
                                 )
                             if subname not in self._branch_lookup:
                                 self._branch_lookup[subname] = len(self._branch_data)
                                 self._branch_data.append(
                                     self._branch_np(subname, content, dtype)
                                 )
 
                 else:
                     raise TypeError(
-                        "cannot write Awkward Array type to ROOT file:\n\n    {}".format(
-                            str(branch_datashape)
-                        )
+                        f"cannot write Awkward Array type to ROOT file:\n\n    {branch_datashape!s}"
                     )
 
         self._num_entries = 0
         self._num_baskets = 0
 
         self._metadata_start = None
         self._metadata = {
@@ -659,18 +649,15 @@
         tofill = []
         num_entries = None
         for branch_name, branch_array in actual_branches.items():
             if num_entries is None:
                 num_entries = len(branch_array)
             elif num_entries != len(branch_array):
                 raise ValueError(
-                    "'extend' must fill every branch with the same number of entries; {} has {} entries".format(
-                        repr(branch_name),
-                        len(branch_array),
-                    )
+                    f"'extend' must fill every branch with the same number of entries; {branch_name!r} has {len(branch_array)} entries"
                 )
 
             datum = self._branch_data[self._branch_lookup[branch_name]]
             if datum["kind"] == "record":
                 continue
 
             if datum["counter"] is None:
```

### Comparing `uproot-5.3.2rc1/src/uproot/writing/_dask_write.py` & `uproot-5.3.3/src/uproot/writing/_dask_write.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/src/uproot/writing/identify.py` & `uproot-5.3.3/src/uproot/writing/identify.py`

 * *Files 1% similar despite different names*

```diff
@@ -216,17 +216,15 @@
     elif type(obj).__module__ == "cppyy.gbl":
         import ROOT
 
         if isinstance(obj, ROOT.TObject):
             return uproot.pyroot._PyROOTWritable(obj)
         else:
             raise TypeError(
-                "only instances of TObject can be written to files, not {}".format(
-                    type(obj).__name__
-                )
+                f"only instances of TObject can be written to files, not {type(obj).__name__}"
             )
 
     elif isinstance(obj, str):
         return to_TObjString(obj)
 
     elif (
         hasattr(obj, "axes")
@@ -915,17 +913,15 @@
         cls = uproot.models.TArray.Model_TArrayL
     elif issubclass(data.dtype.type, numpy.float32):
         cls = uproot.models.TArray.Model_TArrayF
     elif issubclass(data.dtype.type, numpy.float64):
         cls = uproot.models.TArray.Model_TArrayD
     else:
         raise ValueError(
-            "data to convert to TArray must have signed integer or floating-point type, not {}".format(
-                repr(data.dtype)
-            )
+            f"data to convert to TArray must have signed integer or floating-point type, not {data.dtype!r}"
         )
 
     tarray = cls.empty()
     tarray._deeply_writable = True
     tarray._members["fN"] = len(data)
     tarray._data = data.astype(data.dtype.newbyteorder(">"))
     return tarray
```

### Comparing `uproot-5.3.2rc1/src/uproot/writing/writable.py` & `uproot-5.3.3/src/uproot/writing/writable.py`

 * *Files 1% similar despite different names*

```diff
@@ -1230,18 +1230,16 @@
                     initial_directory_bytes,
                     self._file.uuid_function(),
                 ),
             )
 
         elif key.classname.string not in ("TDirectory", "TDirectoryFile"):
             raise TypeError(
-                """cannot make a directory named {} because a {} already has that name
-in file {} in directory {}""".format(
-                    repr(name), key.classname.string, self.file_path, self.path
-                )
+                f"""cannot make a directory named {name!r} because a {key.classname.string} already has that name
+in file {self.file_path} in directory {self.path}"""
             )
 
         else:
             directory = self._subdir(key)
 
         if tail is None:
             return directory
```

### Comparing `uproot-5.3.2rc1/tests/conftest.py` & `uproot-5.3.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0001_source_class.py` & `uproot-5.3.3/tests/test_0001_source_class.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0006_notify_when_downloaded.py` & `uproot-5.3.3/tests/test_0006_notify_when_downloaded.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0007_single_chunk_interface.py` & `uproot-5.3.3/tests/test_0007_single_chunk_interface.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0008_start_interpretation.py` & `uproot-5.3.3/tests/test_0008_start_interpretation.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0009_nested_directories.py` & `uproot-5.3.3/tests/test_0009_nested_directories.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0010_start_streamers.py` & `uproot-5.3.3/tests/test_0010_start_streamers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0011_generate_classes_from_streamers.py` & `uproot-5.3.3/tests/test_0011_generate_classes_from_streamers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0013_rntuple_anchor.py` & `uproot-5.3.3/tests/test_0013_rntuple_anchor.py`

 * *Files 14% similar despite different names*

```diff
@@ -11,68 +11,70 @@
 import uproot
 
 
 def test():
     filename = skhep_testdata.data_path("uproot-ntpl001_staff.root")
     with uproot.open(filename) as f:
         obj = f["Staff"]
-        assert obj.member("fVersion") == 0
-        assert obj.member("fSize") == 48
-        assert obj.member("fSeekHeader") == 854
-        assert obj.member("fNBytesHeader") == 537
-        assert obj.member("fLenHeader") == 2495
-        assert obj.member("fSeekFooter") == 72369
-        assert obj.member("fNBytesFooter") == 285
-        assert obj.member("fLenFooter") == 804
-        assert obj.member("fReserved") == 0
+        assert obj.member("fVersionEpoch") == 0
+        assert obj.member("fVersionMajor") == 2
+        assert obj.member("fVersionMinor") == 0
+        assert obj.member("fVersionPatch") == 0
+        assert obj.member("fSeekHeader") == 266
+        assert obj.member("fNBytesHeader") == 391
+        assert obj.member("fLenHeader") == 996
+        assert obj.member("fSeekFooter") == 36420
+        assert obj.member("fNBytesFooter") == 89
+        assert obj.member("fLenFooter") == 172
+        assert obj.member("fChecksum") == 12065027575882477574
 
         header_start = obj.member("fSeekHeader")
         header_stop = header_start + obj.member("fNBytesHeader")
         header_chunk = f.file.source.chunk(header_start, header_stop)
 
         # print("HEADER")
         # cursor = uproot.Cursor(header_start)
-        # cursor.debug(header_chunk, 80)
+        # cursor.debug(header_chunk, limit_bytes=80)
         # print("\n")
 
         notifications = queue.Queue()
         footer_start = obj.member("fSeekFooter")
         footer_stop = footer_start + obj.member("fNBytesFooter")
         header_chunk, footer_chunk = f.file.source.chunks(
             [(header_start, header_stop), (footer_start, footer_stop)],
             notifications,
         )
 
         # print("FOOTER")
         # cursor = uproot.Cursor(footer_start)
-        # cursor.debug(footer_chunk, 80)
+        # cursor.debug(footer_chunk, limit_bytes=80)
         # print("\n")
 
 
 # HEADER
 # --+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+-
-#  76  52   1  16   2   0 191   9   0 198  14 105   8  80  63  75 128 117   0   0
-#   L   4 --- --- --- --- --- --- --- --- ---   i ---   P   ?   K ---   u --- ---
+#  76  52   1 126   1   0 228   3   0 226  97  52  14 191  32 119  70  87   1   0
+#   L   4 ---   ~ --- --- --- --- --- ---   a   4 --- ---       w   F   W --- ---
 # --+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+-
-#   0   0 187   9   0   1   0 144   5   0   0   0  83 116  97 102 102  13   0 255
-# --- --- --- --- --- --- --- --- --- --- --- ---   S   t   a   f   f --- --- ---
+# 228   3   0   1   0 144   5   0   0   0  83 116  97 102 102  13   0 241   5  13
+# --- --- --- --- --- --- --- --- --- ---   S   t   a   f   f --- --- --- --- ---
 # --+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+-
-#   6  16   0   0   0 117 110 100 101 102 105 110 101 100  32  97 117 116 104 111
-# --- --- --- --- ---   u   n   d   e   f   i   n   e   d       a   u   t   h   o
+#   0   0   0  82  79  79  84  32 118  54  46  51  49  47  48  49 122 253 255   1
+# --- --- ---   R   O   O   T       v   6   .   3   1   /   0   1   z --- --- ---
 # --+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+-
-# 114   0   1   0   4  47  24   0   1   0   3  31  12  12   0   0   4   8   0 110
-#   r --- --- --- ---   / --- --- --- --- --- --- --- --- --- --- --- --- ---   n
+#   0 111  11   0   0   0  60   0   1   0   3 244  13   8   0   0   0  67  97 116
+# ---   o --- --- --- ---   < --- --- --- --- --- --- --- --- --- ---   C   a   t
 
 
 # FOOTER
 # --+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+-
-#  76  52   1  20   1   0  36   3   0  86 138 213  67  60 183  39 139  27   0   1
-#   L   4 --- --- --- ---   $ --- ---   V --- ---   C   < ---   ' --- --- --- ---
+#  76  52   1  80   0   0 172   0   0 143 248  61  98 249  16  31  87  72   2   0
+#   L   4 ---   P --- --- --- --- --- --- ---   =   b --- --- ---   W   H --- ---
 # --+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+-
-#   0  23   1  12   0  23  12  12   0  42  72   0   1   0  47  24   0   1   0   7
-# --- --- --- --- --- --- --- --- ---   *   H --- --- ---   / --- --- --- --- ---
+# 172   0   1   0 147 119 211 249  23 217  49  71 211  56  16   0  34 244 255   1
+# --- --- --- --- ---   w --- --- --- ---   1   G ---   8 --- ---   " --- --- ---
 # --+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+-
-#  34  26  13   8   0  34 145   5   8   0  34 213   9  86   0  27  13  84   0   0
-#   " --- --- --- ---   " --- --- --- ---   " --- ---   V --- --- ---   T --- ---
+#   0  15  12   0  33  19 196  12   0 106   1   0   0   0  48   0   1   0  34  26
+# --- --- --- ---   ! --- --- --- ---   j --- --- --- ---   0 --- --- ---   " ---
 # --+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+---+-
-#   1   0 102  52  26   0   0 148   1 124   0   0  16   0  34 102  15  17   0  34
-# --- ---   f   4 --- --- --- --- ---   | --- --- --- ---   "   f --- --- ---   "
+#  13   8   0   0  28   0  34  92   2  12   0 110 234   0   0   0  56 141 120   0
+# --- --- --- --- --- ---   "   \ --- --- ---   n --- --- --- ---   8 ---   x ---
```

### Comparing `uproot-5.3.2rc1/tests/test_0014_all_ttree_versions.py` & `uproot-5.3.3/tests/test_0014_all_ttree_versions.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0016_interpretations.py` & `uproot-5.3.3/tests/test_0016_interpretations.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0017_multi_basket_multi_branch_fetch.py` & `uproot-5.3.3/tests/test_0017_multi_basket_multi_branch_fetch.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0018_array_fetching_interface.py` & `uproot-5.3.3/tests/test_0018_array_fetching_interface.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0022_number_of_branches.py` & `uproot-5.3.3/tests/test_0022_number_of_branches.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0023_more_interpretations_1.py` & `uproot-5.3.3/tests/test_0023_more_interpretations_1.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0023_ttree_versions.py` & `uproot-5.3.3/tests/test_0023_ttree_versions.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0029_more_string_types.py` & `uproot-5.3.3/tests/test_0029_more_string_types.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0031_test_stl_containers.py` & `uproot-5.3.3/tests/test_0031_test_stl_containers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0033_more_interpretations_2.py` & `uproot-5.3.3/tests/test_0033_more_interpretations_2.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0034_generic_objects_in_ttrees.py` & `uproot-5.3.3/tests/test_0034_generic_objects_in_ttrees.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0035_datatype_generality.py` & `uproot-5.3.3/tests/test_0035_datatype_generality.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0038_memberwise_serialization.py` & `uproot-5.3.3/tests/test_0038_memberwise_serialization.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0043_iterate_function.py` & `uproot-5.3.3/tests/test_0043_iterate_function.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0044_concatenate_function.py` & `uproot-5.3.3/tests/test_0044_concatenate_function.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0046_histograms_bh_hist.py` & `uproot-5.3.3/tests/test_0046_histograms_bh_hist.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0053_parents_should_not_be_bases.py` & `uproot-5.3.3/tests/test_0053_parents_should_not_be_bases.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0058_detach_model_objects_from_files.py` & `uproot-5.3.3/tests/test_0058_detach_model_objects_from_files.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0067_common_entry_offsets.py` & `uproot-5.3.3/tests/test_0067_common_entry_offsets.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0081_dont_parse_colons.py` & `uproot-5.3.3/tests/test_0081_dont_parse_colons.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0087_memberwise_splitting_not_implemented_messages.py` & `uproot-5.3.3/tests/test_0087_memberwise_splitting_not_implemented_messages.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0088_read_with_http.py` & `uproot-5.3.3/tests/test_0088_read_with_http.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0099_read_from_file_object.py` & `uproot-5.3.3/tests/test_0099_read_from_file_object.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0112_fix_pandas_with_cut.py` & `uproot-5.3.3/tests/test_0112_fix_pandas_with_cut.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0118_fix_name_fetch_again.py` & `uproot-5.3.3/tests/test_0118_fix_name_fetch_again.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0167_use_the_common_histogram_interface.py` & `uproot-5.3.3/tests/test_0167_use_the_common_histogram_interface.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0173_empty_and_multiprocessing_bugs.py` & `uproot-5.3.3/tests/test_0173_empty_and_multiprocessing_bugs.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0182_complain_about_missing_files.py` & `uproot-5.3.3/tests/test_0182_complain_about_missing_files.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0220_contiguous_byte_ranges_in_http.py` & `uproot-5.3.3/tests/test_0220_contiguous_byte_ranges_in_http.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0228_read_TProfiles.py` & `uproot-5.3.3/tests/test_0228_read_TProfiles.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0240_read_TGraphAsymmErrors.py` & `uproot-5.3.3/tests/test_0240_read_TGraphAsymmErrors.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0278_specializations_for_TParameter.py` & `uproot-5.3.3/tests/test_0278_specializations_for_TParameter.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0302_pickle.py` & `uproot-5.3.3/tests/test_0302_pickle.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0303_empty_jagged_array.py` & `uproot-5.3.3/tests/test_0303_empty_jagged_array.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0320_start_working_on_ROOT_writing.py` & `uproot-5.3.3/tests/test_0320_start_working_on_ROOT_writing.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0322_writablefile_infrastructure.py` & `uproot-5.3.3/tests/test_0322_writablefile_infrastructure.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0329_update_existing_root_files.py` & `uproot-5.3.3/tests/test_0329_update_existing_root_files.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0341_manipulate_streamer_info.py` & `uproot-5.3.3/tests/test_0341_manipulate_streamer_info.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0344_writabledirectory_can_read.py` & `uproot-5.3.3/tests/test_0344_writabledirectory_can_read.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0345_bulk_copy_method.py` & `uproot-5.3.3/tests/test_0345_bulk_copy_method.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0349_write_TObjString.py` & `uproot-5.3.3/tests/test_0349_write_TObjString.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0350_read_RooCurve_RooHist.py` & `uproot-5.3.3/tests/test_0350_read_RooCurve_RooHist.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0351_write_TList.py` & `uproot-5.3.3/tests/test_0351_write_TList.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0352_write_THashList.py` & `uproot-5.3.3/tests/test_0352_write_THashList.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0384_move_behavior_of_and_fix_383.py` & `uproot-5.3.3/tests/test_0384_move_behavior_of_and_fix_383.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0398_dimensions_in_leaflist.py` & `uproot-5.3.3/tests/test_0398_dimensions_in_leaflist.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0405_write_a_histogram.py` & `uproot-5.3.3/tests/test_0405_write_a_histogram.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0406_write_a_ttree.py` & `uproot-5.3.3/tests/test_0406_write_a_ttree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0407_read_TDatime.py` & `uproot-5.3.3/tests/test_0407_read_TDatime.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0412_write_multidimensional_numpy_to_ttree.py` & `uproot-5.3.3/tests/test_0412_write_multidimensional_numpy_to_ttree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0414_write_jagged_arrays.py` & `uproot-5.3.3/tests/test_0414_write_jagged_arrays.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0416_writing_compressed_data.py` & `uproot-5.3.3/tests/test_0416_writing_compressed_data.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0418_read_TTable.py` & `uproot-5.3.3/tests/test_0418_read_TTable.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0420_pyroot_uproot_interoperability.py` & `uproot-5.3.3/tests/test_0420_pyroot_uproot_interoperability.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0422_hist_integration.py` & `uproot-5.3.3/tests/test_0422_hist_integration.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0438_TClonesArray_is_not_AsGrouped.py` & `uproot-5.3.3/tests/test_0438_TClonesArray_is_not_AsGrouped.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0442_regular_TClonesArray.py` & `uproot-5.3.3/tests/test_0442_regular_TClonesArray.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0472_tstreamerinfo_for_ttree.py` & `uproot-5.3.3/tests/test_0472_tstreamerinfo_for_ttree.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0475_remember_to_update_freesegments.py` & `uproot-5.3.3/tests/test_0475_remember_to_update_freesegments.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0487_implement_asdtypeinplace.py` & `uproot-5.3.3/tests/test_0487_implement_asdtypeinplace.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0498_create_leaf_branch_in_extend.py` & `uproot-5.3.3/tests/test_0498_create_leaf_branch_in_extend.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0576_unicode_in_names.py` & `uproot-5.3.3/tests/test_0576_unicode_in_names.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0578_dask_for_numpy.py` & `uproot-5.3.3/tests/test_0578_dask_for_numpy.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0580_round_trip_for_no_flow_histograms.py` & `uproot-5.3.3/tests/test_0580_round_trip_for_no_flow_histograms.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0589_explicitly_interpret_RVec_type.py` & `uproot-5.3.3/tests/test_0589_explicitly_interpret_RVec_type.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0603_dask_delayed_open.py` & `uproot-5.3.3/tests/test_0603_dask_delayed_open.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0609_num_enteries_func.py` & `uproot-5.3.3/tests/test_0609_num_enteries_func.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0610_awkward_form.py` & `uproot-5.3.3/tests/test_0610_awkward_form.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0630_rntuple_basics.py` & `uproot-5.3.3/tests/test_0630_rntuple_basics.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,25 +9,24 @@
 import skhep_testdata
 
 import uproot
 
 pytest.importorskip("awkward")
 
 
-@pytest.mark.skip(reason="RNTUPLE UPDATE: ignore test with previous file for now.")
 def test_flat():
     filename = skhep_testdata.data_path("test_ntuple_int_float.root")
     with uproot.open(filename) as f:
         R = f["ntuple"]
         assert R.keys() == ["one_integers", "two_floats"]
         assert [r.type_name for r in R.header.field_records] == [
             "std::int32_t",
             "float",
         ]
-        assert R.header.crc32 == R.footer.header_crc32
+        assert R.header.checksum == R.footer.header_checksum
         assert all(R.arrays(entry_stop=3)["one_integers"] == numpy.array([9, 8, 7]))
         assert all(
             R.arrays("one_integers", entry_stop=3)["one_integers"]
             == numpy.array([9, 8, 7])
         )
         assert all(
             R.arrays(entry_start=1, entry_stop=3)["one_integers"] == numpy.array([8, 7])
```

### Comparing `uproot-5.3.2rc1/tests/test_0637_setup_tests_for_AwkwardForth.py` & `uproot-5.3.3/tests/test_0637_setup_tests_for_AwkwardForth.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0643_reading_vector_pair_TLorentzVector_int.py` & `uproot-5.3.3/tests/test_0643_reading_vector_pair_TLorentzVector_int.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0651_implement_transformed_axis.py` & `uproot-5.3.3/tests/test_0651_implement_transformed_axis.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0652_dask_for_awkward.py` & `uproot-5.3.3/tests/test_0652_dask_for_awkward.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0662_rntuple_stl_containers.py` & `uproot-5.3.3/tests/test_0662_rntuple_stl_containers.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0692_fsspec_reading.py` & `uproot-5.3.3/tests/test_0692_fsspec_reading.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 # BSD 3-Clause License; see https://github.com/scikit-hep/uproot4/blob/main/LICENSE
 
-import pytest
-import uproot
-import uproot.source.fsspec
-import uproot.source.file
-import uproot.source.xrootd
-import uproot.source.s3
-
 from typing import BinaryIO
 import skhep_testdata
 import queue
 import fsspec
 import requests
 import os
 import sys
 
+import pytest
+
+import uproot
+import uproot.source.fsspec
+import uproot.source.file
+import uproot.source.xrootd
+import uproot.source.s3
+
 is_windows = sys.platform.startswith("win")
 
 
 @pytest.mark.parametrize(
     "urlpath, source_class",
     [
         ("file.root", uproot.source.fsspec.FSSpecSource),
@@ -239,15 +240,15 @@
             [(0, 100), (50, 55), (200, 400)], notifications=notifications
         )
         expected = {(chunk.start, chunk.stop): chunk for chunk in chunks}
         while len(expected) > 0:
             chunk = notifications.get()
             expected.pop((chunk.start, chunk.stop))
 
-        chunk_data_sum = {sum(chunk.raw_data) for chunk in chunks}
+        chunk_data_sum = {sum(map(int, chunk.raw_data)) for chunk in chunks}
         assert chunk_data_sum == {3967, 413, 10985}, "Chunk data does not match"
 
 
 def test_fsspec_memory():
     # read the file into memory
     with open(skhep_testdata.data_path("uproot-issue121.root"), "rb") as f:
         contents = f.read()
```

### Comparing `uproot-5.3.2rc1/tests/test_0692_fsspec_writing.py` & `uproot-5.3.3/tests/test_0692_fsspec_writing.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,20 +47,27 @@
 @pytest.mark.parametrize(
     "filename", ["file.root", "file%2Eroot", "my%E2%80%92file.root", "my%20file.root"]
 )
 @pytest.mark.parametrize(
     "slash_prefix",
     [""] if is_windows else ["", "/"],
 )
-def test_fsspec_writing_local_uri(tmp_path, scheme, slash_prefix, filename):
-    uri = scheme + slash_prefix + os.path.join(tmp_path, "some", "path", filename)
-    with uproot.create(uri) as f:
-        f["tree"] = {"x": np.array([1, 2, 3])}
-    with uproot.open(uri) as f:
-        assert f["tree"]["x"].array().tolist() == [1, 2, 3]
+def test_fsspec_writing_local_uri(tmp_path, scheme, slash_prefix, filename, request):
+    os.chdir(tmp_path)
+
+    try:
+        uri = scheme + slash_prefix + os.path.join(tmp_path, "some", "path", filename)
+
+        with uproot.create(uri) as f:
+            f["tree"] = {"x": np.array([1, 2, 3])}
+        with uproot.open(uri) as f:
+            assert f["tree"]["x"].array().tolist() == [1, 2, 3]
+
+    finally:
+        os.chdir(request.config.invocation_params.dir)
 
 
 @pytest.mark.parametrize(
     "input_value",
     [
         "\\file.root",
         "\\file%2Eroot",
```

### Comparing `uproot-5.3.2rc1/tests/test_0700_dask_empty_arrays.py` & `uproot-5.3.3/tests/test_0700_dask_empty_arrays.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0755_dask_awkward_column_projection.py` & `uproot-5.3.3/tests/test_0755_dask_awkward_column_projection.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0791_protect_uproot_project_columns_from_dask_node_names.py` & `uproot-5.3.3/tests/test_0791_protect_uproot_project_columns_from_dask_node_names.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0798_DAOD_PHYSLITE.py` & `uproot-5.3.3/tests/test_0798_DAOD_PHYSLITE.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0808_fix_awkward_form_for_AsStridedObjects.py` & `uproot-5.3.3/tests/test_0808_fix_awkward_form_for_AsStridedObjects.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0816_separate_AwkwardForth_machines_by_TBranch.py` & `uproot-5.3.3/tests/test_0816_separate_AwkwardForth_machines_by_TBranch.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0832_ak_add_doc_should_also_add_to_typetracer.py` & `uproot-5.3.3/tests/test_0832_ak_add_doc_should_also_add_to_typetracer.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0840_support_tleafG.py` & `uproot-5.3.3/tests/test_0840_support_tleafG.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0841_fix_814.py` & `uproot-5.3.3/tests/test_0841_fix_814.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0844_fix_delete_hist_from_root.py` & `uproot-5.3.3/tests/test_0844_fix_delete_hist_from_root.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0876_uproot_dask_blind_steps.py` & `uproot-5.3.3/tests/test_0876_uproot_dask_blind_steps.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0911_fix_interp_array_non_numerical_objs_issue_880.py` & `uproot-5.3.3/tests/test_0911_fix_interp_array_non_numerical_objs_issue_880.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0912_fix_pandas_and_double_nested_vectors_issue_885.py` & `uproot-5.3.3/tests/test_0912_fix_pandas_and_double_nested_vectors_issue_885.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0916_read_from_s3.py` & `uproot-5.3.3/tests/test_0916_read_from_s3.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0930_expressions_in_pandas.py` & `uproot-5.3.3/tests/test_0930_expressions_in_pandas.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0940_feat_add_TLeafC_string_support.py` & `uproot-5.3.3/tests/test_0940_feat_add_TLeafC_string_support.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0962_RNTuple_update.py` & `uproot-5.3.3/tests/test_0962_RNTuple_update.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,51 +4,46 @@
 import uproot
 import awkward as ak
 import skhep_testdata
 import numpy as np
 
 
 def test_new_support_RNTuple_split_int32_reading():
-    with uproot.open(
-        skhep_testdata.data_path("uproot_ntuple_int_5e4_629_01.root")
-    ) as f:
+    with uproot.open(skhep_testdata.data_path("test_ntuple_int_5e4.root")) as f:
         obj = f["ntuple"]
         df = obj.arrays()
         assert len(df) == 5e4
         assert len(df.one_integers) == 5e4
         assert np.all(df.one_integers == np.arange(5e4 + 1)[::-1][:-1])
 
 
 def test_new_support_RNTuple_bit_bool_reading():
-    with uproot.open(skhep_testdata.data_path("uproot_ntuple_bit_629_01.root")) as f:
+    with uproot.open(skhep_testdata.data_path("test_ntuple_bit.root")) as f:
         obj = f["ntuple"]
         df = obj.arrays()
         assert np.all(df.one_bit == np.asarray([1, 0, 0, 1, 0, 0, 1, 0, 0, 1]))
 
 
 def test_new_support_RNTuple_split_int16_reading():
     with uproot.open(
-        skhep_testdata.data_path("uproot_ntuple_int_multicluster_629_01.root")
+        skhep_testdata.data_path("test_ntuple_int_multicluster.root")
     ) as f:
         obj = f["ntuple"]
         df = obj.arrays()
         assert len(df.one_integers) == 1e8
         assert df.one_integers[0] == 2
         assert df.one_integers[-1] == 1
         assert np.all(np.unique(df.one_integers[: len(df.one_integers) // 2]) == [2])
         assert np.all(np.unique(df.one_integers[len(df.one_integers) / 2 + 1 :]) == [1])
 
 
 pytest.importorskip("cramjam")
 
 
-@pytest.mark.xfail(
-    reason="Uproot can now read the data from event files (CMS/Atlas), but this test fails because the column matching logic is wrong.",
-    strict=True,
-)
+@pytest.mark.skip(reason="Need to find a similar file in RNTuple RC2 format")
 def test_new_support_RNTuple_event_data():
     with uproot.open(
         "https://xrootd-local.unl.edu:1094//store/user/AGC/nanoaod-rntuple/zstd/TT_TuneCUETP8M1_13TeV-powheg-pythia8/cmsopendata2015_ttbar_19980_PU25nsData2015v1_76X_mcRun2_asymptotic_v12_ext3-v1_00000_0000.root"
     ) as f:
         obj = f["Events"]
         df = obj.arrays(["nTau"])
         assert len(df) == 1334428
```

### Comparing `uproot-5.3.2rc1/tests/test_0965_inverted_axes_variances_hist_888.py` & `uproot-5.3.3/tests/test_0965_inverted_axes_variances_hist_888.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_0976_path_object_split.py` & `uproot-5.3.3/tests/test_0976_path_object_split.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_1000-write-TProfiles.py` & `uproot-5.3.3/tests/test_1000-write-TProfiles.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_1058_dask_awkward_report.py` & `uproot-5.3.3/tests/test_1058_dask_awkward_report.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_1063_dask_distributed.py` & `uproot-5.3.3/tests/test_1063_dask_distributed.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_1085_dask_write.py` & `uproot-5.3.3/tests/test_1085_dask_write.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_1114_fix_attempt_to_concatenate_numpy_with_awkward.py` & `uproot-5.3.3/tests/test_1114_fix_attempt_to_concatenate_numpy_with_awkward.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_1127_fix_allow_colon_in_key_names.py` & `uproot-5.3.3/tests/test_1127_fix_allow_colon_in_key_names.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_1146_split_ranges_for_large_files_over_http.py` & `uproot-5.3.3/tests/test_1146_split_ranges_for_large_files_over_http.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_1154_classof_using_relative_path.py` & `uproot-5.3.3/tests/test_1154_classof_using_relative_path.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/test_1160_std_string_in_TDirectory.py` & `uproot-5.3.3/tests/test_1160_std_string_in_TDirectory.py`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/tests/samples/h_dynamic.pkl` & `uproot-5.3.3/tests/samples/h_dynamic.pkl`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/.gitignore` & `uproot-5.3.3/.gitignore`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/LICENSE` & `uproot-5.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/README.md` & `uproot-5.3.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -182,14 +182,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/HaarigerHarald"><img src="https://avatars.githubusercontent.com/u/8050292?v=4?s=100" width="100px;" alt="HaarigerHarald"/><br /><sub><b>HaarigerHarald</b></sub></a><br /><a href="https://github.com/scikit-hep/uproot5/commits?author=HaarigerHarald" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/bnavigator"><img src="https://avatars.githubusercontent.com/u/4623504?v=4?s=100" width="100px;" alt="Ben Greiner"/><br /><sub><b>Ben Greiner</b></sub></a><br /><a href="https://github.com/scikit-hep/uproot5/commits?author=bnavigator" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://tooldev.de"><img src="https://avatars.githubusercontent.com/u/1640386?v=4?s=100" width="100px;" alt="Robin Sonnabend"/><br /><sub><b>Robin Sonnabend</b></sub></a><br /><a href="https://github.com/scikit-hep/uproot5/commits?author=YSelfTool" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/bojohnson5"><img src="https://avatars.githubusercontent.com/u/20647190?v=4?s=100" width="100px;" alt="Bo Johnson"/><br /><sub><b>Bo Johnson</b></sub></a><br /><a href="https://github.com/scikit-hep/uproot5/commits?author=bojohnson5" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/milesgranger"><img src="https://avatars.githubusercontent.com/u/13764397?v=4?s=100" width="100px;" alt="Miles"/><br /><sub><b>Miles</b></sub></a><br /><a href="https://github.com/scikit-hep/uproot5/commits?author=milesgranger" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/djw9497"><img src="https://avatars.githubusercontent.com/u/51672890?v=4?s=100" width="100px;" alt="djw9497"/><br /><sub><b>djw9497</b></sub></a><br /><a href="https://github.com/scikit-hep/uproot5/commits?author=djw9497" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

### Comparing `uproot-5.3.2rc1/pyproject.toml` & `uproot-5.3.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `uproot-5.3.2rc1/PKG-INFO` & `uproot-5.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: uproot
-Version: 5.3.2rc1
+Version: 5.3.3
 Summary: ROOT I/O in pure Python and NumPy.
 Project-URL: Download, https://github.com/scikit-hep/uproot5/releases
 Project-URL: Homepage, https://github.com/scikit-hep/uproot5
 Author-email: Jim Pivarski <pivarski@princeton.edu>
 License-Expression: BSD-3-Clause
 License-File: LICENSE
 Classifier: Development Status :: 5 - Production/Stable
@@ -250,14 +250,15 @@
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/HaarigerHarald"><img src="https://avatars.githubusercontent.com/u/8050292?v=4?s=100" width="100px;" alt="HaarigerHarald"/><br /><sub><b>HaarigerHarald</b></sub></a><br /><a href="https://github.com/scikit-hep/uproot5/commits?author=HaarigerHarald" title="Code">💻</a></td>
     </tr>
     <tr>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/bnavigator"><img src="https://avatars.githubusercontent.com/u/4623504?v=4?s=100" width="100px;" alt="Ben Greiner"/><br /><sub><b>Ben Greiner</b></sub></a><br /><a href="https://github.com/scikit-hep/uproot5/commits?author=bnavigator" title="Tests">⚠️</a></td>
       <td align="center" valign="top" width="14.28%"><a href="http://tooldev.de"><img src="https://avatars.githubusercontent.com/u/1640386?v=4?s=100" width="100px;" alt="Robin Sonnabend"/><br /><sub><b>Robin Sonnabend</b></sub></a><br /><a href="https://github.com/scikit-hep/uproot5/commits?author=YSelfTool" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/bojohnson5"><img src="https://avatars.githubusercontent.com/u/20647190?v=4?s=100" width="100px;" alt="Bo Johnson"/><br /><sub><b>Bo Johnson</b></sub></a><br /><a href="https://github.com/scikit-hep/uproot5/commits?author=bojohnson5" title="Code">💻</a></td>
       <td align="center" valign="top" width="14.28%"><a href="https://github.com/milesgranger"><img src="https://avatars.githubusercontent.com/u/13764397?v=4?s=100" width="100px;" alt="Miles"/><br /><sub><b>Miles</b></sub></a><br /><a href="https://github.com/scikit-hep/uproot5/commits?author=milesgranger" title="Code">💻</a></td>
+      <td align="center" valign="top" width="14.28%"><a href="https://github.com/djw9497"><img src="https://avatars.githubusercontent.com/u/51672890?v=4?s=100" width="100px;" alt="djw9497"/><br /><sub><b>djw9497</b></sub></a><br /><a href="https://github.com/scikit-hep/uproot5/commits?author=djw9497" title="Code">💻</a></td>
     </tr>
   </tbody>
 </table>
 
 <!-- markdownlint-restore -->
 <!-- prettier-ignore-end -->
```

