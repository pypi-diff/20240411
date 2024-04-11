# Comparing `tmp/nelsie-0.5.0.tar.gz` & `tmp/nelsie-0.6.0.tar.gz`

## Comparing `nelsie-0.5.0.tar` & `nelsie-0.6.0.tar`

### file list

```diff
@@ -1,281 +1,298 @@
--rw-r--r--   0        0        0      899 1970-01-01 00:00:00.000000 nelsie-0.5.0/Cargo.toml
--rw-r--r--   0     1001      127       63 2024-03-31 15:28:13.000000 nelsie-0.5.0/.flake8
--rw-r--r--   0     1001      127     6576 2024-03-31 15:28:13.000000 nelsie-0.5.0/.github/workflows/build.yaml
--rw-r--r--   0     1001      127      159 2024-03-31 15:28:13.000000 nelsie-0.5.0/.gitignore
--rw-r--r--   0     1001      127      232 2024-03-31 15:28:13.000000 nelsie-0.5.0/CHANGELOG.md
--rw-r--r--   0     1001      127     1073 2024-03-31 15:28:13.000000 nelsie-0.5.0/LICENSE
--rw-r--r--   0     1001      127     2224 2024-03-31 15:28:13.000000 nelsie-0.5.0/README.md
--rw-r--r--   0     1001      127     1205 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/README.md
--rw-r--r--   0     1001      127       97 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/api.md
--rw-r--r--   0     1001      127      295 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/examples.md
--rw-r--r--   0     1001      127      474 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/getting_started.md
--rw-r--r--   0     1001      127     1610 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/guide/basics.md
--rw-r--r--   0     1001      127     4698 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/guide/box.md
--rw-r--r--   0     1001      127     5816 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/guide/code.md
--rw-r--r--   0     1001      127      462 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/guide/colors.md
--rw-r--r--   0     1001      127     2220 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/guide/counters.md
--rw-r--r--   0     1001      127     2099 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/guide/debug_layout.md
--rw-r--r--   0     1001      127     3094 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/guide/images.md
--rw-r--r--   0     1001      127     7477 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/guide/layout.md
--rw-r--r--   0     1001      127     5914 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/guide/layoutexpr.md
--rw-r--r--   0     1001      127     1758 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/guide/list.md
--rw-r--r--   0     1001      127     1393 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/guide/output.md
--rw-r--r--   0     1001      127     7692 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/guide/paths.md
--rw-r--r--   0     1001      127      647 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/guide/rendering.md
--rw-r--r--   0     1001      127     1305 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/guide/resources.md
--rw-r--r--   0     1001      127     7056 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/guide/steps.md
--rw-r--r--   0     1001      127     7119 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/guide/text.md
--rw-r--r--   0     1001      127     9616 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/imgs/layers.png
--rw-r--r--   0     1001      127    79667 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/imgs/nelsie-logo.jpg
--rw-r--r--   0     1001      127   336247 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/imgs/stepped_logo.ora
--rw-r--r--   0     1001      127    23211 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/imgs/steps/0-1.png
--rw-r--r--   0     1001      127    23190 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/imgs/steps/0-2.png
--rw-r--r--   0     1001      127    23008 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/imgs/steps/0-3.png
--rw-r--r--   0     1001      127    57229 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/imgs/steps/0-4.png
--rw-r--r--   0     1001      127      478 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/install.md
--rw-r--r--   0     1001      127     7036 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/mkdocs-nelsie-plugin/mkdocs_nelsie_plugin/__init__.py
--rw-r--r--   0     1001      127      439 2024-03-31 15:28:13.000000 nelsie-0.5.0/docs/mkdocs-nelsie-plugin/setup.py
--rw-r--r--   0     1001      127    14538 2024-03-31 15:28:13.000000 nelsie-0.5.0/examples/bigdemo/bigdemo.py
--rw-r--r--   0     1001      127     1225 2024-03-31 15:28:13.000000 nelsie-0.5.0/examples/bigdemo/imgs/knight.svg
--rw-r--r--   0     1001      127    17327 2024-03-31 15:28:13.000000 nelsie-0.5.0/examples/bigdemo/imgs/layers.svg
--rw-r--r--   0     1001      127   336247 2024-03-31 15:28:13.000000 nelsie-0.5.0/examples/bigdemo/imgs/stepped_logo.ora
--rw-r--r--   0     1001      127    92372 2024-03-31 15:28:13.000000 nelsie-0.5.0/examples/bigdemo/karla_font/Karla-Italic-VariableFont_wght.ttf
--rw-r--r--   0     1001      127    90404 2024-03-31 15:28:13.000000 nelsie-0.5.0/examples/bigdemo/karla_font/Karla-VariableFont_wght.ttf
--rw-r--r--   0     1001      127     4476 2024-03-31 15:28:13.000000 nelsie-0.5.0/examples/bigdemo/karla_font/OFL.txt
--rw-r--r--   0     1001      127     2450 2024-03-31 15:28:13.000000 nelsie-0.5.0/examples/bigdemo/karla_font/README.txt
--rw-r--r--   0     1001      127      149 2024-03-31 15:28:13.000000 nelsie-0.5.0/examples/minimal/minimal.py
--rw-r--r--   0     1001      127     1406 2024-03-31 15:28:13.000000 nelsie-0.5.0/mkdocs.yml
--rw-r--r--   0     1001      127       57 2024-03-31 15:28:13.000000 nelsie-0.5.0/pytest.ini
--rw-r--r--   0     1001      127      521 2024-03-31 15:28:13.000000 nelsie-0.5.0/python/nelsie/__init__.py
--rw-r--r--   0     1001      127      991 2024-03-31 15:28:13.000000 nelsie-0.5.0/python/nelsie/basictypes.py
--rw-r--r--   0     1001      127    16753 2024-03-31 15:28:13.000000 nelsie-0.5.0/python/nelsie/box.py
--rw-r--r--   0     1001      127     1952 2024-03-31 15:28:13.000000 nelsie-0.5.0/python/nelsie/helpers/list.py
--rw-r--r--   0     1001      127     2499 2024-03-31 15:28:13.000000 nelsie-0.5.0/python/nelsie/insteps.py
--rw-r--r--   0     1001      127     2169 2024-03-31 15:28:13.000000 nelsie-0.5.0/python/nelsie/layoutexpr.py
--rw-r--r--   0     1001      127        0 2024-03-31 15:28:13.000000 nelsie-0.5.0/python/nelsie/py.typed
--rw-r--r--   0     1001      127     2706 2024-03-31 15:28:13.000000 nelsie-0.5.0/python/nelsie/shapes.py
--rw-r--r--   0     1001      127     6035 2024-03-31 15:28:13.000000 nelsie-0.5.0/python/nelsie/slidedeck.py
--rw-r--r--   0     1001      127     1594 2024-03-31 15:28:13.000000 nelsie-0.5.0/python/nelsie/textstyle.py
--rw-r--r--   0     1001      127      153 2024-03-31 15:28:13.000000 nelsie-0.5.0/python/nelsie/utils.py
--rw-r--r--   0     1001      127       60 2024-03-31 15:28:13.000000 nelsie-0.5.0/ruff.toml
--rw-r--r--   0     1001      127     4931 2024-03-31 15:28:13.000000 nelsie-0.5.0/scripts/compare_tests.py
--rwxr-xr-x   0     1001      127      176 2024-03-31 15:28:13.000000 nelsie-0.5.0/scripts/format.sh
--rw-r--r--   0     1001      127        5 2024-03-31 15:28:13.000000 nelsie-0.5.0/scripts/requirements-check.txt
--rw-r--r--   0     1001      127       84 2024-03-31 15:28:13.000000 nelsie-0.5.0/scripts/requirements-doc.txt
--rw-r--r--   0     1001      127       14 2024-03-31 15:28:13.000000 nelsie-0.5.0/scripts/requirements-test.txt
--rw-r--r--   0     1001      127      725 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/common/error.rs
--rw-r--r--   0     1001      127      276 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/common/fileutils.rs
--rw-r--r--   0     1001      127       70 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/common/mod.rs
--rw-r--r--   0     1001      127      152 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/lib.rs
--rw-r--r--   0     1001      127     8360 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/model/image.rs
--rw-r--r--   0     1001      127      870 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/model/mod.rs
--rw-r--r--   0     1001      127     3250 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/model/node.rs
--rw-r--r--   0     1001      127     3069 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/model/resources.rs
--rw-r--r--   0     1001      127     1637 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/model/shapes.rs
--rw-r--r--   0     1001      127     5634 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/model/slidedeck.rs
--rw-r--r--   0     1001      127     3715 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/model/steps.rs
--rw-r--r--   0     1001      127     4030 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/model/text.rs
--rw-r--r--   0     1001      127     3348 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/model/textstyles.rs
--rw-r--r--   0     1001      127     4442 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/model/types.rs
--rw-r--r--   0     1001      127      546 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/parsers/mod.rs
--rw-r--r--   0     1001      127     3865 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/parsers/size.rs
--rw-r--r--   0     1001      127     3078 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/parsers/step_parser.rs
--rw-r--r--   0     1001      127     4011 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/parsers/syntaxhighlight.rs
--rw-r--r--   0     1001      127    18338 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/parsers/text.rs
--rw-r--r--   0     1001      127     1378 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/pyinterface/basictypes.rs
--rw-r--r--   0     1001      127    13406 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/pyinterface/box.rs
--rw-r--r--   0     1001      127     9807 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/pyinterface/deck.rs
--rw-r--r--   0     1001      127        1 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/pyinterface/error.rs
--rw-r--r--   0     1001      127     2603 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/pyinterface/insteps.rs
--rw-r--r--   0     1001      127     3239 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/pyinterface/layoutexpr.rs
--rw-r--r--   0     1001      127      947 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/pyinterface/mod.rs
--rw-r--r--   0     1001      127     3613 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/pyinterface/path.rs
--rw-r--r--   0     1001      127      938 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/pyinterface/resources.rs
--rw-r--r--   0     1001      127     5902 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/pyinterface/textstyle.rs
--rw-r--r--   0     1001      127     2706 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/render/core.rs
--rw-r--r--   0     1001      127     2682 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/render/counters.rs
--rw-r--r--   0     1001      127     4335 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/render/image.rs
--rw-r--r--   0     1001      127    16253 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/render/layout.rs
--rw-r--r--   0     1001      127     5178 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/render/mod.rs
--rw-r--r--   0     1001      127     8678 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/render/paths.rs
--rw-r--r--   0     1001      127     2322 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/render/pdf.rs
--rw-r--r--   0     1001      127     8712 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/render/rendering.rs
--rw-r--r--   0     1001      127     9781 2024-03-31 15:28:13.000000 nelsie-0.5.0/src/render/text.rs
--rw-r--r--   0     1001      127   705684 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/assets/fonts/DejaVuSans-Bold.ttf
--rw-r--r--   0     1001      127   643292 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/assets/fonts/DejaVuSans-BoldOblique.ttf
--rw-r--r--   0     1001      127   355380 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/assets/fonts/DejaVuSans-ExtraLight.ttf
--rw-r--r--   0     1001      127   635416 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/assets/fonts/DejaVuSans-Oblique.ttf
--rw-r--r--   0     1001      127   757076 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/assets/fonts/DejaVuSans.ttf
--rw-r--r--   0     1001      127   665028 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/assets/fonts/DejaVuSansCondensed-Bold.ttf
--rw-r--r--   0     1001      127   611836 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/assets/fonts/DejaVuSansCondensed-BoldOblique.ttf
--rw-r--r--   0     1001      127   599292 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/assets/fonts/DejaVuSansCondensed-Oblique.ttf
--rw-r--r--   0     1001      127   680264 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/assets/fonts/DejaVuSansCondensed.ttf
--rw-r--r--   0     1001      127   331992 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/assets/fonts/DejaVuSansMono-Bold.ttf
--rw-r--r--   0     1001      127   253580 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/assets/fonts/DejaVuSansMono-BoldOblique.ttf
--rw-r--r--   0     1001      127   251932 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/assets/fonts/DejaVuSansMono-Oblique.ttf
--rw-r--r--   0     1001      127   340712 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/assets/fonts/DejaVuSansMono.ttf
--rw-r--r--   0     1001      127     1225 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/assets/knight.svg
--rw-r--r--   0     1001      127    26005 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/assets/test.ora
--rw-r--r--   0     1001      127     4345 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/assets/test.svg
--rw-r--r--   0     1001      127    12711 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/assets/testimg.jpeg
--rw-r--r--   0     1001      127     4040 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/assets/testimg.png
--rw-r--r--   0     1001      127     1428 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/active_next_last_keywords/0-1.png
--rw-r--r--   0     1001      127     2382 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/active_next_last_keywords/0-2.png
--rw-r--r--   0     1001      127     4315 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/active_next_last_keywords/0-3.png
--rw-r--r--   0     1001      127     3558 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/active_next_last_keywords/0-4.png
--rw-r--r--   0     1001      127     2115 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/active_steps/0-1.png
--rw-r--r--   0     1001      127     2366 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/active_steps/0-2.png
--rw-r--r--   0     1001      127     2344 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/active_steps/0-3.png
--rw-r--r--   0     1001      127     2238 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/array_text_in_steps/0-1.png
--rw-r--r--   0     1001      127     2470 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/array_text_in_steps/0-2.png
--rw-r--r--   0     1001      127     2127 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/array_text_in_steps/0-3.png
--rw-r--r--   0     1001      127     1786 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/bg_color_opacity/0-1.png
--rw-r--r--   0     1001      127     2313 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/box_border_radius/0-1.png
--rw-r--r--   0     1001      127     4818 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/box_debug_frame/0-1.png
--rw-r--r--   0     1001      127    45677 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/chessboard/0-1.png
--rw-r--r--   0     1001      127    45258 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/chessboard/0-2.png
--rw-r--r--   0     1001      127    45532 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/chessboard/0-3.png
--rw-r--r--   0     1001      127    42985 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/chessboard/0-4.png
--rw-r--r--   0     1001      127     3818 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/code_language_default/0-1.png
--rw-r--r--   0     1001      127     3726 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/code_language_none/0-1.png
--rw-r--r--   0     1001      127    16236 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/code_rust_syntax_highlight/0-1.png
--rw-r--r--   0     1001      127    15726 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/code_rust_syntax_highlight/1-1.png
--rw-r--r--   0     1001      127     4323 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/code_style_delimiters/0-1.png
--rw-r--r--   0     1001      127    13720 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/code_syntax_highlight_anchors/0-1.png
--rw-r--r--   0     1001      127    21169 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/code_syntax_highlight_with_styles/0-1.png
--rw-r--r--   0     1001      127     1475 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/expr_x_y_weight_height/0-1.png
--rw-r--r--   0     1001      127    20994 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/fix_sizes/0-1.png
--rw-r--r--   0     1001      127    22070 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/layout_directions/0-1.png
--rw-r--r--   0     1001      127    22070 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/layout_directions/1-1.png
--rw-r--r--   0     1001      127    21057 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/layout_directions/2-1.png
--rw-r--r--   0     1001      127    21057 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/layout_directions/3-1.png
--rw-r--r--   0     1001      127     1904 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/layout_flex_grow/0-1.png
--rw-r--r--   0     1001      127     3062 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/layout_flex_wrap/0-1.png
--rw-r--r--   0     1001      127     2546 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/layout_gap/0-1.png
--rw-r--r--   0     1001      127     2557 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/layout_gap/1-1.png
--rw-r--r--   0     1001      127     1509 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/layout_gap/2-1.png
--rw-r--r--   0     1001      127     2546 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/layout_justify_content/0-1.png
--rw-r--r--   0     1001      127     2546 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/layout_justify_content/1-1.png
--rw-r--r--   0     1001      127     2546 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/layout_justify_content/2-1.png
--rw-r--r--   0     1001      127     2546 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/layout_justify_content/3-1.png
--rw-r--r--   0     1001      127     2520 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/layout_margin/0-1.png
--rw-r--r--   0     1001      127     3705 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/layout_padding/0-1.png
--rw-r--r--   0     1001      127     6414 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/layout_position/0-1.png
--rw-r--r--   0     1001      127     6414 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/layout_position/1-1.png
--rw-r--r--   0     1001      127     6417 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/layout_position/2-1.png
--rw-r--r--   0     1001      127     6204 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/layout_position/3-1.png
--rw-r--r--   0     1001      127     6414 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/layout_position/4-1.png
--rw-r--r--   0     1001      127     4193 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/layout_position_string/0-1.png
--rw-r--r--   0     1001      127     4337 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/line_box/0-1.png
--rw-r--r--   0     1001      127    18970 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/list/0-1.png
--rw-r--r--   0     1001      127     1601 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/m_xy_p_xy/0-1.png
--rw-r--r--   0     1001      127     1456 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/m_xy_p_xy/1-1.png
--rw-r--r--   0     1001      127    11462 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/path_arrows/0-1.png
--rw-r--r--   0     1001      127    11477 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/path_arrows/1-1.png
--rw-r--r--   0     1001      127     3937 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/path_box_positions/0-1.png
--rw-r--r--   0     1001      127     6528 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/path_close/0-1.png
--rw-r--r--   0     1001      127     1813 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/path_opacity/0-1.png
--rw-r--r--   0     1001      127     5840 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/path_oval/0-1.png
--rw-r--r--   0     1001      127     7711 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/path_text_line_positions/0-1.png
--rw-r--r--   0     1001      127     6424 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_cubic/0-1.png
--rw-r--r--   0     1001      127     9758 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_ora_image_no_steps/0-1.png
--rw-r--r--   0     1001      127    38467 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_ora_image_scale/0-1.png
--rw-r--r--   0     1001      127     5754 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_ora_image_steps/0-1.png
--rw-r--r--   0     1001      127     7923 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_ora_image_steps/0-2.png
--rw-r--r--   0     1001      127     7889 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_ora_image_steps/0-3.png
--rw-r--r--   0     1001      127     7892 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_path_dash/0-1.png
--rw-r--r--   0     1001      127     1793 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_path_steps/0-1.png
--rw-r--r--   0     1001      127     3026 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_path_steps/0-2.png
--rw-r--r--   0     1001      127     3026 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_path_steps/0-3.png
--rw-r--r--   0     1001      127     5328 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_path_steps/0-4.png
--rw-r--r--   0     1001      127     5468 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_paths/0-1.png
--rw-r--r--   0     1001      127    39065 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_raster_image_forced_size/0-1.png
--rw-r--r--   0     1001      127    16182 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_raster_image_forced_size/1-1.png
--rw-r--r--   0     1001      127    27612 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_raster_image_forced_size/2-1.png
--rw-r--r--   0     1001      127    24090 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_raster_image_forced_size/3-1.png
--rw-r--r--   0     1001      127    28336 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_raster_image_forced_size/4-1.png
--rw-r--r--   0     1001      127    38151 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_raster_image_native_size/0-1.png
--rw-r--r--   0     1001      127    21482 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_steps/0-1.png
--rw-r--r--   0     1001      127    19850 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_steps/0-2.png
--rw-r--r--   0     1001      127    19274 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_steps/0-3.png
--rw-r--r--   0     1001      127    15351 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_svg_image_no_steps/0-1.png
--rw-r--r--   0     1001      127     1815 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_svg_image_shift/0-1.png
--rw-r--r--   0     1001      127     1815 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_svg_image_shift/0-2.png
--rw-r--r--   0     1001      127     2700 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_svg_image_shift/0-3.png
--rw-r--r--   0     1001      127     3123 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_svg_image_shift/0-4.png
--rw-r--r--   0     1001      127     3418 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_svg_image_shift/0-5.png
--rw-r--r--   0     1001      127     3388 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_svg_image_shift/0-6.png
--rw-r--r--   0     1001      127     9784 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_svg_image_steps/0-1.png
--rw-r--r--   0     1001      127    12385 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_svg_image_steps/0-2.png
--rw-r--r--   0     1001      127    14217 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_svg_image_steps/0-3.png
--rw-r--r--   0     1001      127    13500 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_svg_image_steps/0-4.png
--rw-r--r--   0     1001      127    42050 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_text_basic/0-1.png
--rw-r--r--   0     1001      127    21950 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_text_basic/1-1.png
--rw-r--r--   0     1001      127    28923 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_text_basic/2-1.png
--rw-r--r--   0     1001      127    53754 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_text_basic/3-1.png
--rw-r--r--   0     1001      127     7237 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_text_steps/0-1.png
--rw-r--r--   0     1001      127     8842 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_text_steps/0-2.png
--rw-r--r--   0     1001      127    47559 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/render_text_unicode/0-1.png
--rw-r--r--   0     1001      127     3664 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/replace_steps/0-1.png
--rw-r--r--   0     1001      127     2918 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/replace_steps/0-2.png
--rw-r--r--   0     1001      127     3654 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/replace_steps/0-3.png
--rw-r--r--   0     1001      127     3725 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/replace_steps/0-4.png
--rw-r--r--   0     1001      127     1428 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/show_next_last_keywords/0-1.png
--rw-r--r--   0     1001      127     2382 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/show_next_last_keywords/0-2.png
--rw-r--r--   0     1001      127     4315 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/show_next_last_keywords/0-3.png
--rw-r--r--   0     1001      127     3558 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/show_next_last_keywords/0-4.png
--rw-r--r--   0     1001      127     1793 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/show_steps/0-1.png
--rw-r--r--   0     1001      127     2243 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/show_steps/0-2.png
--rw-r--r--   0     1001      127     2463 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/show_steps/0-3.png
--rw-r--r--   0     1001      127     2533 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/show_steps/0-4.png
--rw-r--r--   0     1001      127    21470 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/slide_decorator/0-1.png
--rw-r--r--   0     1001      127    12547 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/slide_decorator/1-1.png
--rw-r--r--   0     1001      127     1771 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/step_global_counter/0-1.png
--rw-r--r--   0     1001      127     1796 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/step_global_counter/0-2.png
--rw-r--r--   0     1001      127    12802 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/step_global_counter/1-1.png
--rw-r--r--   0     1001      127     2418 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/step_global_counter/2-1.png
--rw-r--r--   0     1001      127     3002 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/step_invalid_counter/0-1.png
--rw-r--r--   0     1001      127     1874 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/step_other_counter/0-1.png
--rw-r--r--   0     1001      127     1720 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/step_other_counter/1-1.png
--rw-r--r--   0     1001      127     1720 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/step_other_counter/2-1.png
--rw-r--r--   0     1001      127     1747 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/step_other_counter/3-1.png
--rw-r--r--   0     1001      127     1752 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/step_other_counter/3-2.png
--rw-r--r--   0     1001      127     1752 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/step_other_counter/4-1.png
--rw-r--r--   0     1001      127    11867 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/text_align/0-1.png
--rw-r--r--   0     1001      127     5586 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/text_anchor_points/0-1.png
--rw-r--r--   0     1001      127     5548 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/text_anchor_points/1-1.png
--rw-r--r--   0     1001      127     5614 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/text_anchor_points/2-1.png
--rw-r--r--   0     1001      127     9989 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/text_anchors_space_prefix/0-1.png
--rw-r--r--   0     1001      127     4269 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/text_anchors_styled_space_prefix/0-1.png
--rw-r--r--   0     1001      127     2264 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/text_boxes/0-1.png
--rw-r--r--   0     1001      127     5116 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/text_color_opacity/0-1.png
--rw-r--r--   0     1001      127    24861 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/text_descent_ascent1/0-1.png
--rw-r--r--   0     1001      127     9660 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/text_descent_ascent2/0-1.png
--rw-r--r--   0     1001      127     3135 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/text_in_steps/0-1.png
--rw-r--r--   0     1001      127     3383 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/text_in_steps/0-2.png
--rw-r--r--   0     1001      127     3998 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/text_in_steps/0-3.png
--rw-r--r--   0     1001      127     3007 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/text_kerning/0-1.png
--rw-r--r--   0     1001      127     4688 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/text_line_points1/0-1.png
--rw-r--r--   0     1001      127     7917 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/text_line_points2/0-1.png
--rw-r--r--   0     1001      127     4866 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/text_monospace/0-1.png
--rw-r--r--   0     1001      127     7640 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/text_stroke/0-1.png
--rw-r--r--   0     1001      127     9949 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/text_styling/0-1.png
--rw-r--r--   0     1001      127     1155 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/checks/z_level/0-1.png
--rw-r--r--   0     1001      127     1098 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/conftest.py
--rw-r--r--   0     1001      127       20 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/requirements.txt
--rw-r--r--   0     1001      127     2772 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/test_code.py
--rw-r--r--   0     1001      127     1128 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/test_complex.py
--rw-r--r--   0     1001      127      872 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/test_error.py
--rw-r--r--   0     1001      127     2131 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/test_image.py
--rw-r--r--   0     1001      127     7122 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/test_layout.py
--rw-r--r--   0     1001      127      782 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/test_list.py
--rw-r--r--   0     1001      127      886 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/test_others.py
--rw-r--r--   0     1001      127     5992 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/test_paths.py
--rw-r--r--   0     1001      127      279 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/test_resources.py
--rw-r--r--   0     1001      127     1930 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/test_slidedeck.py
--rw-r--r--   0     1001      127     4329 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/test_steps.py
--rw-r--r--   0     1001      127    12918 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/test_text.py
--rw-r--r--   0     1001      127     2708 2024-03-31 15:28:13.000000 nelsie-0.5.0/tests/testutils.py
--rw-r--r--   0     1001      127    37316 2024-03-31 15:28:13.000000 nelsie-0.5.0/Cargo.lock
--rw-r--r--   0     1001      127      472 2024-03-31 15:28:13.000000 nelsie-0.5.0/pyproject.toml
--rw-r--r--   0        0        0     2614 1970-01-01 00:00:00.000000 nelsie-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      899 1970-01-01 00:00:00.000000 nelsie-0.6.0/Cargo.toml
+-rw-r--r--   0     1001      127       63 2024-04-11 17:24:58.000000 nelsie-0.6.0/.flake8
+-rw-r--r--   0     1001      127     6576 2024-04-11 17:24:58.000000 nelsie-0.6.0/.github/workflows/build.yaml
+-rw-r--r--   0     1001      127      159 2024-04-11 17:24:58.000000 nelsie-0.6.0/.gitignore
+-rw-r--r--   0     1001      127      340 2024-04-11 17:24:58.000000 nelsie-0.6.0/CHANGELOG.md
+-rw-r--r--   0     1001      127     1073 2024-04-11 17:24:58.000000 nelsie-0.6.0/LICENSE
+-rw-r--r--   0     1001      127     2224 2024-04-11 17:24:58.000000 nelsie-0.6.0/README.md
+-rw-r--r--   0     1001      127     1205 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/README.md
+-rw-r--r--   0     1001      127       97 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/api.md
+-rw-r--r--   0     1001      127      295 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/examples.md
+-rw-r--r--   0     1001      127      474 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/getting_started.md
+-rw-r--r--   0     1001      127     1610 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/guide/basics.md
+-rw-r--r--   0     1001      127     4698 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/guide/box.md
+-rw-r--r--   0     1001      127     5951 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/guide/code.md
+-rw-r--r--   0     1001      127      462 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/guide/colors.md
+-rw-r--r--   0     1001      127     2406 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/guide/counters.md
+-rw-r--r--   0     1001      127     2099 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/guide/debug_layout.md
+-rw-r--r--   0     1001      127     3094 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/guide/images.md
+-rw-r--r--   0     1001      127     2024 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/guide/insert.md
+-rw-r--r--   0     1001      127     7477 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/guide/layout.md
+-rw-r--r--   0     1001      127     5914 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/guide/layoutexpr.md
+-rw-r--r--   0     1001      127     1758 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/guide/list.md
+-rw-r--r--   0     1001      127     1426 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/guide/output.md
+-rw-r--r--   0     1001      127     7692 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/guide/paths.md
+-rw-r--r--   0     1001      127      647 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/guide/rendering.md
+-rw-r--r--   0     1001      127     2363 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/guide/resources.md
+-rw-r--r--   0     1001      127     7056 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/guide/steps.md
+-rw-r--r--   0     1001      127     7119 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/guide/text.md
+-rw-r--r--   0     1001      127     9616 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/imgs/layers.png
+-rw-r--r--   0     1001      127    79667 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/imgs/nelsie-logo.jpg
+-rw-r--r--   0     1001      127   336247 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/imgs/stepped_logo.ora
+-rw-r--r--   0     1001      127    23211 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/imgs/steps/0-1.png
+-rw-r--r--   0     1001      127    23190 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/imgs/steps/0-2.png
+-rw-r--r--   0     1001      127    23008 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/imgs/steps/0-3.png
+-rw-r--r--   0     1001      127    57229 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/imgs/steps/0-4.png
+-rw-r--r--   0     1001      127      478 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/install.md
+-rw-r--r--   0     1001      127     7036 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/mkdocs-nelsie-plugin/mkdocs_nelsie_plugin/__init__.py
+-rw-r--r--   0     1001      127      439 2024-04-11 17:24:58.000000 nelsie-0.6.0/docs/mkdocs-nelsie-plugin/setup.py
+-rw-r--r--   0     1001      127    14538 2024-04-11 17:24:58.000000 nelsie-0.6.0/examples/bigdemo/bigdemo.py
+-rw-r--r--   0     1001      127     1225 2024-04-11 17:24:58.000000 nelsie-0.6.0/examples/bigdemo/imgs/knight.svg
+-rw-r--r--   0     1001      127    17327 2024-04-11 17:24:58.000000 nelsie-0.6.0/examples/bigdemo/imgs/layers.svg
+-rw-r--r--   0     1001      127   336247 2024-04-11 17:24:58.000000 nelsie-0.6.0/examples/bigdemo/imgs/stepped_logo.ora
+-rw-r--r--   0     1001      127    92372 2024-04-11 17:24:58.000000 nelsie-0.6.0/examples/bigdemo/karla_font/Karla-Italic-VariableFont_wght.ttf
+-rw-r--r--   0     1001      127    90404 2024-04-11 17:24:58.000000 nelsie-0.6.0/examples/bigdemo/karla_font/Karla-VariableFont_wght.ttf
+-rw-r--r--   0     1001      127     4476 2024-04-11 17:24:58.000000 nelsie-0.6.0/examples/bigdemo/karla_font/OFL.txt
+-rw-r--r--   0     1001      127     2450 2024-04-11 17:24:58.000000 nelsie-0.6.0/examples/bigdemo/karla_font/README.txt
+-rw-r--r--   0     1001      127      149 2024-04-11 17:24:58.000000 nelsie-0.6.0/examples/minimal/minimal.py
+-rw-r--r--   0     1001      127     1430 2024-04-11 17:24:58.000000 nelsie-0.6.0/mkdocs.yml
+-rw-r--r--   0     1001      127       57 2024-04-11 17:24:58.000000 nelsie-0.6.0/pytest.ini
+-rw-r--r--   0     1001      127      521 2024-04-11 17:24:58.000000 nelsie-0.6.0/python/nelsie/__init__.py
+-rw-r--r--   0     1001      127      991 2024-04-11 17:24:58.000000 nelsie-0.6.0/python/nelsie/basictypes.py
+-rw-r--r--   0     1001      127    16753 2024-04-11 17:24:58.000000 nelsie-0.6.0/python/nelsie/box.py
+-rw-r--r--   0     1001      127     1952 2024-04-11 17:24:58.000000 nelsie-0.6.0/python/nelsie/helpers/list.py
+-rw-r--r--   0     1001      127     2499 2024-04-11 17:24:58.000000 nelsie-0.6.0/python/nelsie/insteps.py
+-rw-r--r--   0     1001      127     2169 2024-04-11 17:24:58.000000 nelsie-0.6.0/python/nelsie/layoutexpr.py
+-rw-r--r--   0     1001      127        0 2024-04-11 17:24:58.000000 nelsie-0.6.0/python/nelsie/py.typed
+-rw-r--r--   0     1001      127     2706 2024-04-11 17:24:58.000000 nelsie-0.6.0/python/nelsie/shapes.py
+-rw-r--r--   0     1001      127     6764 2024-04-11 17:24:58.000000 nelsie-0.6.0/python/nelsie/slidedeck.py
+-rw-r--r--   0     1001      127     1594 2024-04-11 17:24:58.000000 nelsie-0.6.0/python/nelsie/textstyle.py
+-rw-r--r--   0     1001      127      153 2024-04-11 17:24:58.000000 nelsie-0.6.0/python/nelsie/utils.py
+-rw-r--r--   0     1001      127       60 2024-04-11 17:24:58.000000 nelsie-0.6.0/ruff.toml
+-rw-r--r--   0     1001      127     4931 2024-04-11 17:24:58.000000 nelsie-0.6.0/scripts/compare_tests.py
+-rwxr-xr-x   0     1001      127      176 2024-04-11 17:24:58.000000 nelsie-0.6.0/scripts/format.sh
+-rw-r--r--   0     1001      127        5 2024-04-11 17:24:58.000000 nelsie-0.6.0/scripts/requirements-check.txt
+-rw-r--r--   0     1001      127       84 2024-04-11 17:24:58.000000 nelsie-0.6.0/scripts/requirements-doc.txt
+-rw-r--r--   0     1001      127       14 2024-04-11 17:24:58.000000 nelsie-0.6.0/scripts/requirements-test.txt
+-rw-r--r--   0     1001      127      725 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/common/error.rs
+-rw-r--r--   0     1001      127      276 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/common/fileutils.rs
+-rw-r--r--   0     1001      127       70 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/common/mod.rs
+-rw-r--r--   0     1001      127      152 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/lib.rs
+-rw-r--r--   0     1001      127     8360 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/model/image.rs
+-rw-r--r--   0     1001      127      879 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/model/mod.rs
+-rw-r--r--   0     1001      127     3250 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/model/node.rs
+-rw-r--r--   0     1001      127     4261 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/model/resources.rs
+-rw-r--r--   0     1001      127     1637 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/model/shapes.rs
+-rw-r--r--   0     1001      127     5775 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/model/slidedeck.rs
+-rw-r--r--   0     1001      127     3715 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/model/steps.rs
+-rw-r--r--   0     1001      127     4030 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/model/text.rs
+-rw-r--r--   0     1001      127     3348 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/model/textstyles.rs
+-rw-r--r--   0     1001      127     4442 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/model/types.rs
+-rw-r--r--   0     1001      127      546 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/parsers/mod.rs
+-rw-r--r--   0     1001      127     3865 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/parsers/size.rs
+-rw-r--r--   0     1001      127     3078 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/parsers/step_parser.rs
+-rw-r--r--   0     1001      127     4011 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/parsers/syntaxhighlight.rs
+-rw-r--r--   0     1001      127    18338 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/parsers/text.rs
+-rw-r--r--   0     1001      127     1378 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/pyinterface/basictypes.rs
+-rw-r--r--   0     1001      127    13540 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/pyinterface/box.rs
+-rw-r--r--   0     1001      127    10114 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/pyinterface/deck.rs
+-rw-r--r--   0     1001      127        1 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/pyinterface/error.rs
+-rw-r--r--   0     1001      127     2603 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/pyinterface/insteps.rs
+-rw-r--r--   0     1001      127     3308 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/pyinterface/layoutexpr.rs
+-rw-r--r--   0     1001      127      965 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/pyinterface/mod.rs
+-rw-r--r--   0     1001      127     3613 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/pyinterface/path.rs
+-rw-r--r--   0     1001      127     1599 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/pyinterface/resources.rs
+-rw-r--r--   0     1001      127     6026 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/pyinterface/textstyle.rs
+-rw-r--r--   0     1001      127     3102 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/render/core.rs
+-rw-r--r--   0     1001      127     4169 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/render/counters.rs
+-rw-r--r--   0     1001      127     4335 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/render/image.rs
+-rw-r--r--   0     1001      127    16252 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/render/layout.rs
+-rw-r--r--   0     1001      127     5634 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/render/mod.rs
+-rw-r--r--   0     1001      127     8678 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/render/paths.rs
+-rw-r--r--   0     1001      127     2082 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/render/pdf.rs
+-rw-r--r--   0     1001      127     8711 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/render/rendering.rs
+-rw-r--r--   0     1001      127     9895 2024-04-11 17:24:58.000000 nelsie-0.6.0/src/render/text.rs
+-rw-r--r--   0     1001      127   705684 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/assets/fonts/DejaVuSans-Bold.ttf
+-rw-r--r--   0     1001      127   643292 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/assets/fonts/DejaVuSans-BoldOblique.ttf
+-rw-r--r--   0     1001      127   355380 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/assets/fonts/DejaVuSans-ExtraLight.ttf
+-rw-r--r--   0     1001      127   635416 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/assets/fonts/DejaVuSans-Oblique.ttf
+-rw-r--r--   0     1001      127   757076 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/assets/fonts/DejaVuSans.ttf
+-rw-r--r--   0     1001      127   665028 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/assets/fonts/DejaVuSansCondensed-Bold.ttf
+-rw-r--r--   0     1001      127   611836 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/assets/fonts/DejaVuSansCondensed-BoldOblique.ttf
+-rw-r--r--   0     1001      127   599292 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/assets/fonts/DejaVuSansCondensed-Oblique.ttf
+-rw-r--r--   0     1001      127   680264 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/assets/fonts/DejaVuSansCondensed.ttf
+-rw-r--r--   0     1001      127   331992 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/assets/fonts/DejaVuSansMono-Bold.ttf
+-rw-r--r--   0     1001      127   253580 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/assets/fonts/DejaVuSansMono-BoldOblique.ttf
+-rw-r--r--   0     1001      127   251932 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/assets/fonts/DejaVuSansMono-Oblique.ttf
+-rw-r--r--   0     1001      127   340712 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/assets/fonts/DejaVuSansMono.ttf
+-rw-r--r--   0     1001      127     1225 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/assets/knight.svg
+-rw-r--r--   0     1001      127    26005 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/assets/test.ora
+-rw-r--r--   0     1001      127     4345 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/assets/test.svg
+-rw-r--r--   0     1001      127     1638 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/assets/test.tmTheme
+-rw-r--r--   0     1001      127      161 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/assets/testC.sublime-syntax
+-rw-r--r--   0     1001      127    12711 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/assets/testimg.jpeg
+-rw-r--r--   0     1001      127     4040 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/assets/testimg.png
+-rw-r--r--   0     1001      127     1428 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/active_next_last_keywords/0-0-1.png
+-rw-r--r--   0     1001      127     2382 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/active_next_last_keywords/1-0-2.png
+-rw-r--r--   0     1001      127     4315 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/active_next_last_keywords/2-0-3.png
+-rw-r--r--   0     1001      127     3558 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/active_next_last_keywords/3-0-4.png
+-rw-r--r--   0     1001      127     2115 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/active_steps/0-0-1.png
+-rw-r--r--   0     1001      127     2366 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/active_steps/1-0-2.png
+-rw-r--r--   0     1001      127     2344 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/active_steps/2-0-3.png
+-rw-r--r--   0     1001      127     2238 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/array_text_in_steps/0-0-1.png
+-rw-r--r--   0     1001      127     2470 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/array_text_in_steps/1-0-2.png
+-rw-r--r--   0     1001      127     2127 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/array_text_in_steps/2-0-3.png
+-rw-r--r--   0     1001      127     1786 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/bg_color_opacity/0-0-1.png
+-rw-r--r--   0     1001      127     2313 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/box_border_radius/0-0-1.png
+-rw-r--r--   0     1001      127     4818 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/box_debug_frame/0-0-1.png
+-rw-r--r--   0     1001      127    45677 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/chessboard/0-0-1.png
+-rw-r--r--   0     1001      127    45258 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/chessboard/1-0-2.png
+-rw-r--r--   0     1001      127    45532 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/chessboard/2-0-3.png
+-rw-r--r--   0     1001      127    42985 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/chessboard/3-0-4.png
+-rw-r--r--   0     1001      127     3818 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/code_language_default/0-0-1.png
+-rw-r--r--   0     1001      127     3726 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/code_language_none/0-0-1.png
+-rw-r--r--   0     1001      127    16236 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/code_rust_syntax_highlight/0-0-1.png
+-rw-r--r--   0     1001      127    15726 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/code_rust_syntax_highlight/1-1-1.png
+-rw-r--r--   0     1001      127     4323 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/code_style_delimiters/0-0-1.png
+-rw-r--r--   0     1001      127    13720 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/code_syntax_highlight_anchors/0-0-1.png
+-rw-r--r--   0     1001      127    21169 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/code_syntax_highlight_with_styles/0-0-1.png
+-rw-r--r--   0     1001      127     1475 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/expr_x_y_weight_height/0-0-1.png
+-rw-r--r--   0     1001      127    20994 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/fix_sizes/0-0-1.png
+-rw-r--r--   0     1001      127    22070 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/layout_directions/0-0-1.png
+-rw-r--r--   0     1001      127    22070 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/layout_directions/1-1-1.png
+-rw-r--r--   0     1001      127    21057 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/layout_directions/2-2-1.png
+-rw-r--r--   0     1001      127    21057 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/layout_directions/3-3-1.png
+-rw-r--r--   0     1001      127     1904 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/layout_flex_grow/0-0-1.png
+-rw-r--r--   0     1001      127     3062 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/layout_flex_wrap/0-0-1.png
+-rw-r--r--   0     1001      127     2546 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/layout_gap/0-0-1.png
+-rw-r--r--   0     1001      127     2557 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/layout_gap/1-1-1.png
+-rw-r--r--   0     1001      127     1509 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/layout_gap/2-2-1.png
+-rw-r--r--   0     1001      127     2546 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/layout_justify_content/0-0-1.png
+-rw-r--r--   0     1001      127     2546 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/layout_justify_content/1-1-1.png
+-rw-r--r--   0     1001      127     2546 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/layout_justify_content/2-2-1.png
+-rw-r--r--   0     1001      127     2546 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/layout_justify_content/3-3-1.png
+-rw-r--r--   0     1001      127     2520 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/layout_margin/0-0-1.png
+-rw-r--r--   0     1001      127     3705 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/layout_padding/0-0-1.png
+-rw-r--r--   0     1001      127     6414 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/layout_position/0-0-1.png
+-rw-r--r--   0     1001      127     6414 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/layout_position/1-1-1.png
+-rw-r--r--   0     1001      127     6417 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/layout_position/2-2-1.png
+-rw-r--r--   0     1001      127     6204 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/layout_position/3-3-1.png
+-rw-r--r--   0     1001      127     6414 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/layout_position/4-4-1.png
+-rw-r--r--   0     1001      127     4193 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/layout_position_string/0-0-1.png
+-rw-r--r--   0     1001      127     4337 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/line_box/0-0-1.png
+-rw-r--r--   0     1001      127    18970 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/list/0-0-1.png
+-rw-r--r--   0     1001      127     1601 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/m_xy_p_xy/0-0-1.png
+-rw-r--r--   0     1001      127     1456 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/m_xy_p_xy/1-1-1.png
+-rw-r--r--   0     1001      127    11462 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/path_arrows/0-0-1.png
+-rw-r--r--   0     1001      127    11477 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/path_arrows/1-1-1.png
+-rw-r--r--   0     1001      127     3937 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/path_box_positions/0-0-1.png
+-rw-r--r--   0     1001      127     6528 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/path_close/0-0-1.png
+-rw-r--r--   0     1001      127     1813 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/path_opacity/0-0-1.png
+-rw-r--r--   0     1001      127     5840 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/path_oval/0-0-1.png
+-rw-r--r--   0     1001      127     7711 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/path_text_line_positions/0-0-1.png
+-rw-r--r--   0     1001      127     6424 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_cubic/0-0-1.png
+-rw-r--r--   0     1001      127     9758 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_ora_image_no_steps/0-0-1.png
+-rw-r--r--   0     1001      127    38467 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_ora_image_scale/0-0-1.png
+-rw-r--r--   0     1001      127     5754 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_ora_image_steps/0-0-1.png
+-rw-r--r--   0     1001      127     7923 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_ora_image_steps/1-0-2.png
+-rw-r--r--   0     1001      127     7889 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_ora_image_steps/2-0-3.png
+-rw-r--r--   0     1001      127     7892 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_path_dash/0-0-1.png
+-rw-r--r--   0     1001      127     1793 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_path_steps/0-0-1.png
+-rw-r--r--   0     1001      127     3026 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_path_steps/1-0-2.png
+-rw-r--r--   0     1001      127     3026 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_path_steps/2-0-3.png
+-rw-r--r--   0     1001      127     5328 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_path_steps/3-0-4.png
+-rw-r--r--   0     1001      127     5468 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_paths/0-0-1.png
+-rw-r--r--   0     1001      127    39065 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_raster_image_forced_size/0-0-1.png
+-rw-r--r--   0     1001      127    16182 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_raster_image_forced_size/1-1-1.png
+-rw-r--r--   0     1001      127    27612 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_raster_image_forced_size/2-2-1.png
+-rw-r--r--   0     1001      127    24090 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_raster_image_forced_size/3-3-1.png
+-rw-r--r--   0     1001      127    28336 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_raster_image_forced_size/4-4-1.png
+-rw-r--r--   0     1001      127    38151 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_raster_image_native_size/0-0-1.png
+-rw-r--r--   0     1001      127    21482 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_steps/0-0-1.png
+-rw-r--r--   0     1001      127    19850 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_steps/1-0-2.png
+-rw-r--r--   0     1001      127    19274 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_steps/2-0-3.png
+-rw-r--r--   0     1001      127    15351 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_svg_image_no_steps/0-0-1.png
+-rw-r--r--   0     1001      127     1815 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_svg_image_shift/0-0-1.png
+-rw-r--r--   0     1001      127     1815 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_svg_image_shift/1-0-2.png
+-rw-r--r--   0     1001      127     2700 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_svg_image_shift/2-0-3.png
+-rw-r--r--   0     1001      127     3123 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_svg_image_shift/3-0-4.png
+-rw-r--r--   0     1001      127     3418 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_svg_image_shift/4-0-5.png
+-rw-r--r--   0     1001      127     3388 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_svg_image_shift/5-0-6.png
+-rw-r--r--   0     1001      127     9784 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_svg_image_steps/0-0-1.png
+-rw-r--r--   0     1001      127    12385 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_svg_image_steps/1-0-2.png
+-rw-r--r--   0     1001      127    14217 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_svg_image_steps/2-0-3.png
+-rw-r--r--   0     1001      127    13500 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_svg_image_steps/3-0-4.png
+-rw-r--r--   0     1001      127    42050 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_text_basic/0-0-1.png
+-rw-r--r--   0     1001      127    21950 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_text_basic/1-1-1.png
+-rw-r--r--   0     1001      127    28923 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_text_basic/2-2-1.png
+-rw-r--r--   0     1001      127    53754 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_text_basic/3-3-1.png
+-rw-r--r--   0     1001      127     7237 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_text_steps/0-0-1.png
+-rw-r--r--   0     1001      127     8842 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_text_steps/1-0-2.png
+-rw-r--r--   0     1001      127    47559 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/render_text_unicode/0-0-1.png
+-rw-r--r--   0     1001      127     3664 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/replace_steps/0-0-1.png
+-rw-r--r--   0     1001      127     2918 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/replace_steps/1-0-2.png
+-rw-r--r--   0     1001      127     3654 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/replace_steps/2-0-3.png
+-rw-r--r--   0     1001      127     3725 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/replace_steps/3-0-4.png
+-rw-r--r--   0     1001      127     1428 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/show_next_last_keywords/0-0-1.png
+-rw-r--r--   0     1001      127     2382 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/show_next_last_keywords/1-0-2.png
+-rw-r--r--   0     1001      127     4315 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/show_next_last_keywords/2-0-3.png
+-rw-r--r--   0     1001      127     3558 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/show_next_last_keywords/3-0-4.png
+-rw-r--r--   0     1001      127     1793 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/show_steps/0-0-1.png
+-rw-r--r--   0     1001      127     2243 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/show_steps/1-0-2.png
+-rw-r--r--   0     1001      127     2463 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/show_steps/2-0-3.png
+-rw-r--r--   0     1001      127     2533 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/show_steps/3-0-4.png
+-rw-r--r--   0     1001      127    21470 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/slide_decorator/0-0-1.png
+-rw-r--r--   0     1001      127    12547 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/slide_decorator/1-1-1.png
+-rw-r--r--   0     1001      127     1771 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/step_global_counter/0-0-1.png
+-rw-r--r--   0     1001      127     1796 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/step_global_counter/1-0-2.png
+-rw-r--r--   0     1001      127    12802 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/step_global_counter/2-1-1.png
+-rw-r--r--   0     1001      127     2418 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/step_global_counter/3-2-1.png
+-rw-r--r--   0     1001      127     3002 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/step_invalid_counter/0-0-1.png
+-rw-r--r--   0     1001      127     1747 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/step_other_counter/0-0-1.png
+-rw-r--r--   0     1001      127     1745 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/step_other_counter/1-1-1.png
+-rw-r--r--   0     1001      127     1747 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/step_other_counter/2-2-1.png
+-rw-r--r--   0     1001      127     1773 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/step_other_counter/3-3-1.png
+-rw-r--r--   0     1001      127     1779 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/step_other_counter/4-3-2.png
+-rw-r--r--   0     1001      127     1794 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/step_other_counter/5-3-3.png
+-rw-r--r--   0     1001      127     1796 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/step_other_counter/6-4-1.png
+-rw-r--r--   0     1001      127     1796 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/step_other_counter/7-4-2.png
+-rw-r--r--   0     1001      127     1229 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/subslides/0-0-1.png
+-rw-r--r--   0     1001      127     1393 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/subslides/1-0-2.png
+-rw-r--r--   0     1001      127     1143 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/subslides/2-1-1.png
+-rw-r--r--   0     1001      127     1217 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/subslides/3-3-1.png
+-rw-r--r--   0     1001      127     1186 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/subslides/4-1-2.png
+-rw-r--r--   0     1001      127     1199 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/subslides/5-2-1.png
+-rw-r--r--   0     1001      127     1605 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/subslides/6-0-3.png
+-rw-r--r--   0     1001      127     1146 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/subslides/7-4-1.png
+-rw-r--r--   0     1001      127     1244 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/subslides_decorator/0-0-1.png
+-rw-r--r--   0     1001      127     1824 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/subslides_decorator/1-0-2.png
+-rw-r--r--   0     1001      127     1895 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/subslides_decorator/2-1-1.png
+-rw-r--r--   0     1001      127     2678 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/subslides_decorator/3-0-3.png
+-rw-r--r--   0     1001      127    11867 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/text_align/0-0-1.png
+-rw-r--r--   0     1001      127     5586 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/text_anchor_points/0-0-1.png
+-rw-r--r--   0     1001      127     5548 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/text_anchor_points/1-1-1.png
+-rw-r--r--   0     1001      127     5614 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/text_anchor_points/2-2-1.png
+-rw-r--r--   0     1001      127     9989 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/text_anchors_space_prefix/0-0-1.png
+-rw-r--r--   0     1001      127     4269 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/text_anchors_styled_space_prefix/0-0-1.png
+-rw-r--r--   0     1001      127     2264 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/text_boxes/0-0-1.png
+-rw-r--r--   0     1001      127     5116 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/text_color_opacity/0-0-1.png
+-rw-r--r--   0     1001      127    24861 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/text_descent_ascent1/0-0-1.png
+-rw-r--r--   0     1001      127     9660 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/text_descent_ascent2/0-0-1.png
+-rw-r--r--   0     1001      127     3135 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/text_in_steps/0-0-1.png
+-rw-r--r--   0     1001      127     3383 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/text_in_steps/1-0-2.png
+-rw-r--r--   0     1001      127     3998 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/text_in_steps/2-0-3.png
+-rw-r--r--   0     1001      127     3007 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/text_kerning/0-0-1.png
+-rw-r--r--   0     1001      127     4688 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/text_line_points1/0-0-1.png
+-rw-r--r--   0     1001      127     7917 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/text_line_points2/0-0-1.png
+-rw-r--r--   0     1001      127     4866 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/text_monospace/0-0-1.png
+-rw-r--r--   0     1001      127     7640 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/text_stroke/0-0-1.png
+-rw-r--r--   0     1001      127     9949 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/text_styling/0-0-1.png
+-rw-r--r--   0     1001      127     1155 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/checks/z_level/0-0-1.png
+-rw-r--r--   0     1001      127     1164 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/conftest.py
+-rw-r--r--   0     1001      127       20 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/requirements.txt
+-rw-r--r--   0     1001      127     2805 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/test_code.py
+-rw-r--r--   0     1001      127     1128 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/test_complex.py
+-rw-r--r--   0     1001      127      872 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/test_error.py
+-rw-r--r--   0     1001      127     2131 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/test_image.py
+-rw-r--r--   0     1001      127     7161 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/test_layout.py
+-rw-r--r--   0     1001      127      782 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/test_list.py
+-rw-r--r--   0     1001      127      886 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/test_others.py
+-rw-r--r--   0     1001      127     5992 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/test_paths.py
+-rw-r--r--   0     1001      127     1038 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/test_resources.py
+-rw-r--r--   0     1001      127     1938 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/test_slidedeck.py
+-rw-r--r--   0     1001      127     6040 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/test_steps.py
+-rw-r--r--   0     1001      127    12918 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/test_text.py
+-rw-r--r--   0     1001      127     2708 2024-04-11 17:24:58.000000 nelsie-0.6.0/tests/testutils.py
+-rw-r--r--   0     1001      127    37094 2024-04-11 17:24:58.000000 nelsie-0.6.0/Cargo.lock
+-rw-r--r--   0     1001      127      472 2024-04-11 17:24:58.000000 nelsie-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0     2614 1970-01-01 00:00:00.000000 nelsie-0.6.0/PKG-INFO
```

### Comparing `nelsie-0.5.0/Cargo.toml` & `nelsie-0.6.0/Cargo.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 [package]
 name = "nelsie"
-version = "0.5.0"
+version = "0.6.0"
 edition = "2021"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "nelsie"
 crate-type = ["cdylib"]
 
 [dependencies]
-pyo3 = { version = "0.20", features = ["abi3-py39"] }
+pyo3 = { version = "0.21", features = ["abi3-py39"] }
 taffy = "0.4"
 resvg = "0.38.0"
 svg2pdf = "0.10" # !! Must be synchronized with resvg
 ttf-parser = "0.20" # Not necessary same as resvg but nice to be a same as in resvg
 thiserror = "1"
 svgtypes = "0.13" # Not necessary same as resvg but nice to be a same as in resvg
 log = "0.4"
```

### Comparing `nelsie-0.5.0/.github/workflows/build.yaml` & `nelsie-0.6.0/.github/workflows/build.yaml`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/LICENSE` & `nelsie-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/README.md` & `nelsie-0.6.0/README.md`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/docs/README.md` & `nelsie-0.6.0/docs/README.md`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/docs/guide/basics.md` & `nelsie-0.6.0/docs/guide/basics.md`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/docs/guide/box.md` & `nelsie-0.6.0/docs/guide/box.md`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/docs/guide/code.md` & `nelsie-0.6.0/docs/guide/code.md`

 * *Files 5% similar despite different names*

```diff
@@ -102,18 +102,20 @@
 * "base16-eighties.dark"
 * "base16-mocha.dark"
 * "base16-ocean.light"
 * "InspiredGitHub"
 * "Solarized (dark)"
 * "Solarized (light)"
 
-This list is also programmatically available through [`Resources`](resources.md)
+Custom color themes can be added through [`Resources`](resources.md).
+This list is also programmatically available through [`Resources`](resources.md).
 
 ## The list of supported syntaxes
 
+Custom syntax can be added through [`Resources`](resources.md).
 This list is also programmatically available through [`Resources`](resources.md)
 
 * ASP (asa)
 * ActionScript (as)
 * AppleScript (applescript, script editor)
 * Batch File (bat, cmd)
 * BibTeX (bib)
```

### Comparing `nelsie-0.5.0/docs/guide/counters.md` & `nelsie-0.6.0/docs/guide/counters.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,16 +1,20 @@
 # Page counters
 
 Page counters serves to show information about the current page or the total number of pages on slides.
 
-The following variables can be used in any text on slide if parameter `parse_counters` of `.text()` (or `.code()`) is set to `True`. The `<NAME>` is a name of the actual counter.
+The following variables can be used in any text on slide if parameter `parse_counters` of `.text()` (or `.code()`) is
+set to `True`. The `<NAME>` is a name of the actual counter.
 
 * `$(<NAME>_page)` -- The current page index (counted from 1) for the given counter.
 * `$(<NAME>_pages)` -- The total number of pages of the counter.
-* `$(<NAME>_slide)` -- The current slide index (counted from 1) for the given counter. Note that a slide may produce more steps and therefore may have more pages. For all pages of the same slide, the slide index remains the same.
+* `$(<NAME>_slide)` -- The current slide index (counted from 1) for the given counter. Note that a slide may produce
+  more steps and therefore may have more pages. For all pages of the same slide, the slide index remains the same if
+  there is no inserted slided. In case of inserting a slide, switching back to the original slide also increases slide
+  index counter if the inserted slide was included in counter.
 * `$(<NAME>_slides)` -- The total number of slide for the given counter.
 
 The counter `global` always exists and it includes all slides.
 
 ```nelsie
 
 deck.set_style("default", TextStyle(size=80))
```

### Comparing `nelsie-0.5.0/docs/guide/debug_layout.md` & `nelsie-0.6.0/docs/guide/debug_layout.md`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/docs/guide/images.md` & `nelsie-0.6.0/docs/guide/images.md`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/docs/guide/layout.md` & `nelsie-0.6.0/docs/guide/layout.md`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/docs/guide/layoutexpr.md` & `nelsie-0.6.0/docs/guide/layoutexpr.md`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/docs/guide/list.md` & `nelsie-0.6.0/docs/guide/list.md`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/docs/guide/output.md` & `nelsie-0.6.0/docs/guide/output.md`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,52 @@
 # Output formats
 
 This section shows you how to get slides in PDF, SVG or PNG and how to render slides into files or
 how to get them as Python objects.
 
 ## Rendering into PDF
 
-By default, the `.render()` method on a slide deck takes a filename and creates a PDF file. 
+By default, the `.render()` method on a slide deck takes a filename and creates a PDF file.
 
 ```python
 from nelsie import SlideDeck
 
 deck = SlideDeck()
 
 # Add slides here
 
 deck.render("slides.pdf")
 ```
 
-
 ## Rendering into SVG or PNG
 
 By setting the second parameter to "svg" or "png", you can change the output format to SVG or PNG.
 
 ```python
 from nelsie import SlideDeck
 
 deck = SlideDeck()
 
 # Add slides here
 
-deck.render("output/path1", "svg") # Render slides to SVG 
+deck.render("output/path1", "svg")  # Render slides to SVG
 
-deck.render("output/path2", "png") # Render slides to PNG
+deck.render("output/path2", "png")  # Render slides to PNG
 ```
 
-Unlike PDF, the first parameter is not a path to a file, but to a directory where 
-Nelsie creates SVG (or PNG) images, one image per slide page. 
+Unlike PDF, the first parameter is not a path to a file, but to a directory where
+Nelsie creates SVG (or PNG) images, one image per slide page.
 Nelsie will create the target directory if it does not exist.
-Images are named in the format "X-Y.svg" (or "X-Y.png"), where X is the slide index and Y is a step. 
-
+Images are named in the format "X-Y-Z.svg" (or "X-Y-Z.png"), where X is the page index (zero padded), Y is the slide
+index and Z is a step.
 
 ## In-memory rendering
 
 If the first parameter of the `.render()` method is `None` then Nelsie does not create files but returns
 the images as Python objects. It returns a list of triplets (`slide_id`, `step`, `data`) where `data` are
 `bytes` instance with the image.
 
 ```python
-pages = deck.render(None, "png") 
+pages = deck.render(None, "png")
 
 print(pages)  # Print returned triplets with pages
 ```
```

### Comparing `nelsie-0.5.0/docs/guide/paths.md` & `nelsie-0.6.0/docs/guide/paths.md`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/docs/guide/rendering.md` & `nelsie-0.6.0/docs/guide/rendering.md`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/docs/guide/resources.md` & `nelsie-0.6.0/docs/guide/resources.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,44 +1,85 @@
-
 # Resources
 
-An instance of the Resources class holds information about fonts and loaded images.
+An instance of the Resources class holds information about fonts, code syntaxes and themes, and loaded images.
 By default, an instance of SlideDeck creates its own instance of Resources,
 but you can create your own instance and pass it to the SlideDeck constructor.
 
 There are two main scenarios where it is useful to create your own instance of `Resources'.
 
-* You want to register your own fonts
-* You create more instances of `SlideDeck` and you want to skip some initialization related to font detection or to skip loading the same images repeatedly.
+* You want to register your own fonts, code syntaxes, or code themes
+* You create more instances of `SlideDeck` and you want to skip some initialization or to skip
+  loading the same images repeatedly.
 
 `Resources` instance can also provide a list of available syntaxes and syntax highlighting themes.
 
-## Example: Registering own fonts
+## Registering own fonts
 
 ```python
 from nelsie import Resources, SlideDeck
 
 resources = Resources()
 resources.load_fonts_dir("path/to/fonts")
 
 deck = SlideDeck(resources=resources)
 ```
 
+## Loading custom code syntaxes
+
+Nelsie supports loading syntax files from Sublime editor (files with `.sublime-syntax` extension).
+
+```python
+from nelsie import Resources, SlideDeck
+
+resources = Resources(default_code_syntaxes=False)
+resources.load_code_syntax_dir("path/to/syntaxes")
+
+deck = SlideDeck(resources=resources)
+```
+
+!!! warning "Known bug"
+
+    If you want to add custom syntax definitions, you have to disable loading default
+    syntaxes (`default_code_syntaxes=False`)
+    otherwise `.load_code_syntax_dir()` will not work.
 
-## Example: Reusing resources in more slide decks
+## Loading custom code color themes
+
+Nelsie supports loading color theme `thTheme` (files with `.thTheme` extension).
+
+```python
+from nelsie import Resources, SlideDeck
+
+resources = Resources()
+resources.load_code_theme_dir("path/to/themes")
+
+deck = SlideDeck(resources=resources)
+```
+
+## Reusing resources in more slide decks
 
 ```python
 from nelsie import Resources, SlideDeck
 
 resources = Resources()
 
 deck1 = SlideDeck(resources=resources)
 deck2 = SlideDeck(resources=resources)
 ```
 
+## Disable loading defaults
+
+```python
+from nelsie import Resources
+
+resources = Resources(system_fonts=False,
+                      default_code_syntaxes=False,
+                      default_code_themes=False)
+```
+
 ## List of syntaxes
 
 ```python
 from nelsie import Resources
 
 resources = Resources()
 print(resources.syntaxes())
```

### Comparing `nelsie-0.5.0/docs/guide/steps.md` & `nelsie-0.6.0/docs/guide/steps.md`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/docs/guide/text.md` & `nelsie-0.6.0/docs/guide/text.md`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/docs/imgs/layers.png` & `nelsie-0.6.0/docs/imgs/layers.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/docs/imgs/nelsie-logo.jpg` & `nelsie-0.6.0/docs/imgs/nelsie-logo.jpg`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/docs/imgs/stepped_logo.ora` & `nelsie-0.6.0/docs/imgs/stepped_logo.ora`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/docs/imgs/steps/0-1.png` & `nelsie-0.6.0/docs/imgs/steps/0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/docs/imgs/steps/0-2.png` & `nelsie-0.6.0/docs/imgs/steps/0-2.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/docs/imgs/steps/0-3.png` & `nelsie-0.6.0/docs/imgs/steps/0-3.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/docs/imgs/steps/0-4.png` & `nelsie-0.6.0/docs/imgs/steps/0-4.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/docs/mkdocs-nelsie-plugin/mkdocs_nelsie_plugin/__init__.py` & `nelsie-0.6.0/docs/mkdocs-nelsie-plugin/mkdocs_nelsie_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/examples/bigdemo/bigdemo.py` & `nelsie-0.6.0/examples/bigdemo/bigdemo.py`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/examples/bigdemo/imgs/knight.svg` & `nelsie-0.6.0/examples/bigdemo/imgs/knight.svg`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/examples/bigdemo/imgs/layers.svg` & `nelsie-0.6.0/examples/bigdemo/imgs/layers.svg`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/examples/bigdemo/imgs/stepped_logo.ora` & `nelsie-0.6.0/examples/bigdemo/imgs/stepped_logo.ora`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/examples/bigdemo/karla_font/Karla-Italic-VariableFont_wght.ttf` & `nelsie-0.6.0/examples/bigdemo/karla_font/Karla-Italic-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/examples/bigdemo/karla_font/Karla-VariableFont_wght.ttf` & `nelsie-0.6.0/examples/bigdemo/karla_font/Karla-VariableFont_wght.ttf`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/examples/bigdemo/karla_font/OFL.txt` & `nelsie-0.6.0/examples/bigdemo/karla_font/OFL.txt`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/examples/bigdemo/karla_font/README.txt` & `nelsie-0.6.0/examples/bigdemo/karla_font/README.txt`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/mkdocs.yml` & `nelsie-0.6.0/mkdocs.yml`

 * *Files 1% similar despite different names*

```diff
@@ -19,14 +19,15 @@
       - guide/steps.md
       - guide/text.md
       - guide/code.md
       - guide/images.md
       - guide/paths.md
       - guide/layoutexpr.md
       - guide/rendering.md
+      - guide/insert.md
       - guide/counters.md
       - guide/output.md
       - guide/debug_layout.md
       - guide/resources.md
       - guide/box.md
       - guide/colors.md
       - guide/list.md
```

### Comparing `nelsie-0.5.0/python/nelsie/__init__.py` & `nelsie-0.6.0/python/nelsie/__init__.py`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/python/nelsie/basictypes.py` & `nelsie-0.6.0/python/nelsie/basictypes.py`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/python/nelsie/box.py` & `nelsie-0.6.0/python/nelsie/box.py`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/python/nelsie/helpers/list.py` & `nelsie-0.6.0/python/nelsie/helpers/list.py`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/python/nelsie/insteps.py` & `nelsie-0.6.0/python/nelsie/insteps.py`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/python/nelsie/layoutexpr.py` & `nelsie-0.6.0/python/nelsie/layoutexpr.py`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/python/nelsie/shapes.py` & `nelsie-0.6.0/python/nelsie/shapes.py`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/python/nelsie/slidedeck.py` & `nelsie-0.6.0/python/nelsie/slidedeck.py`

 * *Files 11% similar despite different names*

```diff
@@ -43,14 +43,22 @@
     def set_n_steps(self, value: int):
         assert value >= 1
         self.deck._deck.set_n_steps(self._slide_id, value)
 
     def get_n_steps(self) -> int:
         return self.deck._deck.get_n_steps(self._slide_id)
 
+    def new_slide_at(self, step: int, **slide_kwargs):
+        slide_kwargs["parent_slide"] = (self._slide_id, step)
+        return self.deck.new_slide(**slide_kwargs)
+
+    def slide_at(self, step: int, **slide_kwargs):
+        slide_kwargs["parent_slide"] = (self._slide_id, step)
+        return self.deck.slide(**slide_kwargs)
+
 
 class SlideDeck:
     def __init__(
         self,
         *,
         width: float = 1024,
         height: float = 768,
@@ -103,46 +111,50 @@
         self._deck.set_style(self.resources, name, style, True, None, None)
 
     def get_style(self, name: str, step: int = 1) -> TextStyle:
         return _data_to_text_style(self._deck.get_style(name, step, None, None))
 
     def new_slide(
         self,
+        *,
         width: float | None = None,
         height: float | None = None,
         bg_color: str | None = None,
         image_directory: str | None = None,
         name: str = "",
         debug_layout: bool | str = False,
         counters: list[str] | None = None,
+        parent_slide: tuple[Slide, int] | None = None,
     ) -> Slide:
         """
         Creates a new slide in the slide deck.
         """
         if width is None:
             width = self.width
         if height is None:
             height = self.height
         if bg_color is None:
             bg_color = self.bg_color
         if image_directory is None:
             image_directory = self.image_directory
         debug_layout = parse_debug_layout(debug_layout)
-        slide_id = self._deck.new_slide(width, height, bg_color, name, counters)
+        slide_id = self._deck.new_slide(width, height, bg_color, name, counters, parent_slide)
         return Slide(self, slide_id, name, image_directory, debug_layout)
 
     def slide(
         self,
+        *,
         width: float | None = None,
         height: float | None = None,
         bg_color: str | None = None,
         image_directory: str | None = None,
         name: str = "",
         debug_layout: bool | str = False,
         counters: list[str] | None = None,
+        parent_slide: tuple[Slide, int] | None = None,
     ):
         """
         Decorator for creating new slide.
         It immediately calls the decorated function that should define content of the slide.
         Slide is automatically added into the deck.
 
         Example:
@@ -152,16 +164,26 @@
         @deck.slide()
         def my_first_slide(slide):
             slide.text("Hello!")
         ```
         """
 
         def helper(fn):
-            slide = self.new_slide(width, height, bg_color, image_directory, name, debug_layout, counters)
-            return fn(slide)
+            slide = self.new_slide(
+                width=width,
+                height=height,
+                bg_color=bg_color,
+                image_directory=image_directory,
+                name=name,
+                debug_layout=debug_layout,
+                counters=counters,
+                parent_slide=parent_slide,
+            )
+            fn(slide)
+            return slide
 
         return helper
 
     def render(
         self,
         path: str | pathlib.Path | None,
         output_format: Literal["pdf"] | Literal["svg"] | Literal["png"] = "pdf",
```

### Comparing `nelsie-0.5.0/python/nelsie/textstyle.py` & `nelsie-0.6.0/python/nelsie/textstyle.py`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/scripts/compare_tests.py` & `nelsie-0.6.0/scripts/compare_tests.py`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/src/common/error.rs` & `nelsie-0.6.0/src/common/error.rs`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/src/model/image.rs` & `nelsie-0.6.0/src/model/image.rs`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/src/model/mod.rs` & `nelsie-0.6.0/src/model/mod.rs`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 pub(crate) use self::image::{
     ImageManager, LoadedImageData, NodeContentImage, OraImageData, SvgImageData,
 };
 pub(crate) use self::node::{Node, NodeChild, NodeContent};
 pub(crate) use self::resources::Resources;
 pub(crate) use self::shapes::{Arrow, Drawing, Path, PathPart};
-pub(crate) use self::slidedeck::{Slide, SlideDeck};
+pub(crate) use self::slidedeck::{Slide, SlideDeck, SlideId};
 pub(crate) use self::steps::{Step, StepValue};
 pub(crate) use self::text::{
     InTextAnchor, InTextAnchorId, InTextAnchorPoint, NodeContentText, ParsedText, Span, StyledLine,
     StyledText, TextAlign,
 };
 pub(crate) use self::textstyles::{
     merge_stepped_styles, FontData, PartialTextStyle, StyleMap, TextStyle,
```

### Comparing `nelsie-0.5.0/src/model/node.rs` & `nelsie-0.6.0/src/model/node.rs`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/src/model/shapes.rs` & `nelsie-0.6.0/src/model/shapes.rs`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/src/model/slidedeck.rs` & `nelsie-0.6.0/src/model/slidedeck.rs`

 * *Files 2% similar despite different names*

```diff
@@ -8,39 +8,44 @@
 use std::collections::HashMap;
 use std::sync::Arc;
 use svg2pdf::usvg;
 use taffy::prelude as tf;
 use taffy::style::FlexWrap;
 use usvg::FontStretch;
 
+pub(crate) type SlideId = u32;
+
 #[derive(Debug)]
 pub(crate) struct Slide {
     pub(crate) width: f32,
     pub(crate) height: f32,
     pub(crate) node: Node,
     pub(crate) n_steps: Step,
     pub(crate) bg_color: Color,
     pub(crate) counters: Vec<String>,
+    pub(crate) parent: Option<(SlideId, Step)>,
     node_id_counter: NodeId,
 }
 
 impl Slide {
     pub fn new(
         width: f32,
         height: f32,
         name: String,
         bg_color: Color,
         styles: Arc<StyleMap>,
         counters: Vec<String>,
+        parent: Option<(SlideId, Step)>,
     ) -> Self {
         Slide {
             width,
             height,
             bg_color,
             counters,
+            parent,
             node: Node {
                 styles,
                 name,
                 node_id: NodeId::new(0),
                 children: vec![],
                 replace_steps: Default::default(),
                 active: StepValue::new_const(true),
```

### Comparing `nelsie-0.5.0/src/model/steps.rs` & `nelsie-0.6.0/src/model/steps.rs`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/src/model/text.rs` & `nelsie-0.6.0/src/model/text.rs`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/src/model/textstyles.rs` & `nelsie-0.6.0/src/model/textstyles.rs`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/src/model/types.rs` & `nelsie-0.6.0/src/model/types.rs`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/src/parsers/mod.rs` & `nelsie-0.6.0/src/parsers/mod.rs`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/src/parsers/size.rs` & `nelsie-0.6.0/src/parsers/size.rs`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/src/parsers/step_parser.rs` & `nelsie-0.6.0/src/parsers/step_parser.rs`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/src/parsers/syntaxhighlight.rs` & `nelsie-0.6.0/src/parsers/syntaxhighlight.rs`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/src/parsers/text.rs` & `nelsie-0.6.0/src/parsers/text.rs`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/src/pyinterface/basictypes.rs` & `nelsie-0.6.0/src/pyinterface/basictypes.rs`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/src/pyinterface/box.rs` & `nelsie-0.6.0/src/pyinterface/box.rs`

 * *Files 2% similar despite different names*

```diff
@@ -10,19 +10,21 @@
     parse_length, parse_length_auto, parse_length_or_expr, parse_position, parse_styled_text,
     parse_styled_text_from_plain_text, run_syntax_highlighting, StyleOrName,
 };
 use crate::pyinterface::basictypes::{PyStringOrFloat, PyStringOrFloatOrExpr};
 use crate::pyinterface::insteps::{InSteps, ValueOrInSteps};
 use crate::pyinterface::textstyle::PyTextStyleOrName;
 use std::collections::BTreeMap;
+use std::ops::Deref;
 
 use pyo3::exceptions::PyValueError;
 use pyo3::{FromPyObject, PyAny, PyResult};
 
 use crate::common::error::NelsieError;
+use pyo3::pybacked::PyBackedStr;
 use std::path::PathBuf;
 use std::str::FromStr;
 use std::sync::Arc;
 use taffy::prelude::{AlignContent, AlignItems};
 use taffy::style::FlexWrap;
 
 #[derive(Debug, FromPyObject)]
@@ -211,32 +213,32 @@
                 enable_steps: image.enable_steps,
                 shift_steps: image.shift_steps,
             })
         }
     })
 }
 
-fn parse_align_items(value: Option<&str>) -> crate::Result<Option<AlignItems>> {
+fn parse_align_items(value: Option<PyBackedStr>) -> crate::Result<Option<AlignItems>> {
     value
-        .map(|v| match v {
+        .map(|v| match v.deref() {
             "start" => Ok(AlignItems::Start),
             "end" => Ok(AlignItems::End),
             "flex-start" => Ok(AlignItems::FlexStart),
             "flex-end" => Ok(AlignItems::FlexEnd),
             "center" => Ok(AlignItems::Center),
             "stretch" => Ok(AlignItems::Stretch),
             "baseline" => Ok(AlignItems::Baseline),
             _ => Err(NelsieError::parsing_err("Invalid AlignItems")),
         })
         .transpose()
 }
 
-fn parse_align_content(value: Option<&str>) -> crate::Result<Option<AlignContent>> {
+fn parse_align_content(value: Option<PyBackedStr>) -> crate::Result<Option<AlignContent>> {
     value
-        .map(|v| match v {
+        .map(|v| match v.deref() {
             "start" => Ok(AlignContent::Start),
             "end" => Ok(AlignContent::End),
             "flex-start" => Ok(AlignContent::FlexStart),
             "flex-end" => Ok(AlignContent::FlexEnd),
             "center" => Ok(AlignContent::Center),
             "stretch" => Ok(AlignContent::Stretch),
             "space-between" => Ok(AlignContent::SpaceBetween),
@@ -280,23 +282,23 @@
     x: ValueOrInSteps<Option<PyStringOrFloatOrExpr>>,
     y: ValueOrInSteps<Option<PyStringOrFloatOrExpr>>,
     width: ValueOrInSteps<Option<PyStringOrFloatOrExpr>>,
     height: ValueOrInSteps<Option<PyStringOrFloatOrExpr>>,
     border_radius: ValueOrInSteps<f32>,
     row: ValueOrInSteps<bool>,
     reverse: ValueOrInSteps<bool>,
-    flex_wrap: ValueOrInSteps<&str>,
+    flex_wrap: ValueOrInSteps<PyBackedStr>,
     flex_grow: ValueOrInSteps<f32>,
     flex_shrink: ValueOrInSteps<f32>,
 
-    align_items: ValueOrInSteps<Option<&str>>,
-    align_self: ValueOrInSteps<Option<&str>>,
-    justify_self: ValueOrInSteps<Option<&str>>,
-    align_content: ValueOrInSteps<Option<&str>>,
-    justify_content: ValueOrInSteps<Option<&str>>,
+    align_items: ValueOrInSteps<Option<PyBackedStr>>,
+    align_self: ValueOrInSteps<Option<PyBackedStr>>,
+    justify_self: ValueOrInSteps<Option<PyBackedStr>>,
+    align_content: ValueOrInSteps<Option<PyBackedStr>>,
+    justify_content: ValueOrInSteps<Option<PyBackedStr>>,
     gap: ValueOrInSteps<(PyStringOrFloat, PyStringOrFloat)>,
 
     p_left: ValueOrInSteps<PyStringOrFloat>,
     p_right: ValueOrInSteps<PyStringOrFloat>,
     p_top: ValueOrInSteps<PyStringOrFloat>,
     p_bottom: ValueOrInSteps<PyStringOrFloat>,
     m_left: ValueOrInSteps<PyStringOrFloat>,
@@ -311,15 +313,15 @@
 ) -> PyResult<(Node, Step)> {
     let mut n_steps = 1;
     let mut n_steps2 = 1;
     let content = content
         .map(|c| process_content(c, nc_env, &styles, &mut n_steps2))
         .transpose()?;
     n_steps = n_steps.max(n_steps2);
-    let flex_wrap = flex_wrap.parse(&mut n_steps, |f| match f {
+    let flex_wrap = flex_wrap.parse(&mut n_steps, |f| match f.deref() {
         "nowrap" => Ok(FlexWrap::NoWrap),
         "wrap" => Ok(FlexWrap::Wrap),
         "wrap-reverse" => Ok(FlexWrap::WrapReverse),
         _ => Err(PyValueError::new_err("Invalid wrap value")),
     })?;
     let bg_color = bg_color.parse(&mut n_steps, |v| {
         v.as_deref().map(Color::from_str).transpose()
```

### Comparing `nelsie-0.5.0/src/pyinterface/deck.rs` & `nelsie-0.6.0/src/pyinterface/deck.rs`

 * *Files 3% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 use itertools::Itertools;
 use pyo3::exceptions::{PyException, PyValueError};
 use pyo3::{pyclass, pymethods, PyObject, PyResult, Python, ToPyObject};
 use std::collections::BTreeMap;
 use std::str::FromStr;
 
 use crate::pyinterface::basictypes::{PyStringOrFloat, PyStringOrFloatOrExpr};
+use pyo3::pybacked::PyBackedStr;
 use pyo3::types::{PyBytes, PyNone};
 use std::sync::Arc;
 
 #[pyclass]
 pub(crate) struct Deck {
     deck: SlideDeck,
 }
@@ -59,23 +60,30 @@
     fn new_slide(
         &mut self,
         width: f32,
         height: f32,
         bg_color: &str,
         name: String,
         counters: Option<Vec<String>>,
+        parent: Option<(SlideId, Step)>,
     ) -> PyResult<SlideId> {
         let slide_id = self.deck.slides.len() as SlideId;
+        if let Some((_, step)) = parent {
+            if step == 0 {
+                return Err(PyException::new_err("Invalid step"));
+            }
+        }
         self.deck.slides.push(Slide::new(
             width,
             height,
             name,
             Color::from_str(bg_color)?,
             self.deck.global_styles.clone(),
             counters.unwrap_or_default(),
+            parent,
         ));
         Ok(slide_id)
     }
 
     fn draw(
         &mut self,
         slide_id: SlideId,
@@ -104,23 +112,23 @@
         x: ValueOrInSteps<Option<PyStringOrFloatOrExpr>>,
         y: ValueOrInSteps<Option<PyStringOrFloatOrExpr>>,
         width: ValueOrInSteps<Option<PyStringOrFloatOrExpr>>,
         height: ValueOrInSteps<Option<PyStringOrFloatOrExpr>>,
         border_radius: ValueOrInSteps<f32>,
         row: ValueOrInSteps<bool>,
         reverse: ValueOrInSteps<bool>,
-        flex_wrap: ValueOrInSteps<&str>,
+        flex_wrap: ValueOrInSteps<PyBackedStr>,
         flex_grow: ValueOrInSteps<f32>,
         flex_shrink: ValueOrInSteps<f32>,
 
-        align_items: ValueOrInSteps<Option<&str>>,
-        align_self: ValueOrInSteps<Option<&str>>,
-        justify_self: ValueOrInSteps<Option<&str>>,
-        align_content: ValueOrInSteps<Option<&str>>,
-        justify_content: ValueOrInSteps<Option<&str>>,
+        align_items: ValueOrInSteps<Option<PyBackedStr>>,
+        align_self: ValueOrInSteps<Option<PyBackedStr>>,
+        justify_self: ValueOrInSteps<Option<PyBackedStr>>,
+        align_content: ValueOrInSteps<Option<PyBackedStr>>,
+        justify_content: ValueOrInSteps<Option<PyBackedStr>>,
         gap: ValueOrInSteps<(PyStringOrFloat, PyStringOrFloat)>,
 
         p_left: ValueOrInSteps<PyStringOrFloat>,
         p_right: ValueOrInSteps<PyStringOrFloat>,
         p_top: ValueOrInSteps<PyStringOrFloat>,
         p_bottom: ValueOrInSteps<PyStringOrFloat>,
         m_left: ValueOrInSteps<PyStringOrFloat>,
@@ -287,17 +295,17 @@
                     path: path.map(std::path::Path::new),
                     format,
                 },
                 verbose_level,
             )
         })?;
         if result.is_empty() {
-            Ok(PyNone::get(py).to_object(py))
+            Ok(PyNone::get_bound(py).to_object(py))
         } else {
             Ok(result
                 .iter()
-                .map(|(slide_idx, step, data)| (slide_idx, step, PyBytes::new(py, data)))
+                .map(|(slide_idx, step, data)| (slide_idx, step, PyBytes::new_bound(py, data)))
                 .collect_vec()
                 .to_object(py))
         }
     }
 }
```

### Comparing `nelsie-0.5.0/src/pyinterface/insteps.rs` & `nelsie-0.6.0/src/pyinterface/insteps.rs`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/src/pyinterface/layoutexpr.rs` & `nelsie-0.6.0/src/pyinterface/layoutexpr.rs`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 use crate::model::{LayoutExpr, NodeId};
 use pyo3::exceptions::PyValueError;
+use pyo3::pybacked::PyBackedStr;
 use pyo3::{FromPyObject, PyAny, PyResult};
+use std::ops::Deref;
 
 #[derive(Debug)]
 pub(crate) struct PyLayoutExpr(LayoutExpr);
 
 impl From<PyLayoutExpr> for LayoutExpr {
     fn from(value: PyLayoutExpr) -> Self {
         value.0
@@ -17,16 +19,16 @@
     }
 }
 
 fn extract_layout_expr(obj: &PyAny) -> PyResult<LayoutExpr> {
     if let Ok(value) = obj.extract() {
         return Ok(LayoutExpr::ConstValue { value });
     }
-    let name: &str = obj.get_item(0)?.extract()?;
-    match name {
+    let name: PyBackedStr = obj.get_item(0)?.extract()?;
+    match name.deref() {
         "x" => Ok(LayoutExpr::X {
             node_id: NodeId::new(obj.get_item(1)?.extract()?),
         }),
         "y" => Ok(LayoutExpr::Y {
             node_id: NodeId::new(obj.get_item(1)?.extract()?),
         }),
         "width" => Ok(LayoutExpr::Width {
```

### Comparing `nelsie-0.5.0/src/pyinterface/mod.rs` & `nelsie-0.6.0/src/pyinterface/mod.rs`

 * *Files 9% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 mod resources;
 mod textstyle;
 
 use crate::pyinterface::resources::Resources;
 use deck::Deck;
 use pyo3::exceptions::PyException;
 use pyo3::types::PyModule;
-use pyo3::{pymodule, PyErr, PyResult, Python};
+use pyo3::{pymodule, Bound, PyErr, PyResult, Python};
 
 impl From<crate::NelsieError> for PyErr {
     fn from(err: crate::NelsieError) -> PyErr {
         PyException::new_err(err.to_string())
     }
 }
 
@@ -30,13 +30,13 @@
 // #[pyfunction]
 // fn test_abc(a: ValueOrInSteps<StringOrInt>) -> PyResult<String> {
 //     Ok(format!("{:?}", a))
 // }
 
 /// A Python module implemented in Rust.
 #[pymodule]
-fn nelsie(_py: Python, m: &PyModule) -> PyResult<()> {
+fn nelsie(_py: Python, m: &Bound<'_, PyModule>) -> PyResult<()> {
     //m.add_function(wrap_pyfunction!(test_abc, m)?)?;
     m.add_class::<Deck>()?;
     m.add_class::<Resources>()?;
     Ok(())
 }
```

### Comparing `nelsie-0.5.0/src/pyinterface/path.rs` & `nelsie-0.6.0/src/pyinterface/path.rs`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/src/pyinterface/textstyle.rs` & `nelsie-0.6.0/src/pyinterface/textstyle.rs`

 * *Files 7% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 use crate::model::{Color, PartialTextStyle, Resources, Stroke};
 
 use crate::pyinterface::insteps::ValueOrInSteps;
 use pyo3::exceptions::PyValueError;
+use pyo3::pybacked::PyBackedStr;
 use pyo3::{FromPyObject, PyAny, PyObject, PyResult, Python, ToPyObject};
 use std::collections::HashMap;
+use std::ops::Deref;
 use std::str::FromStr;
 use std::sync::Arc;
 use svg2pdf::usvg;
 use usvg::FontStretch;
 
 #[derive(Debug, Default)]
 pub(crate) struct PyTextStyle {
@@ -44,15 +46,16 @@
             kerning: self.kerning,
         })
     }
 }
 
 impl<'py> FromPyObject<'py> for Color {
     fn extract(ob: &'py PyAny) -> PyResult<Self> {
-        Ok(Color::from_str(ob.extract()?)?)
+        let s: PyBackedStr = ob.extract()?;
+        Ok(Color::from_str(s.deref())?)
     }
 }
 
 impl<'py> FromPyObject<'py> for PyTextStyle {
     fn extract(ob: &'py PyAny) -> PyResult<Self> {
         let stretch_idx: Option<u32> = ob.getattr("stretch")?.extract()?;
         let stretch = stretch_idx
@@ -67,26 +70,26 @@
                 8 => Ok(FontStretch::ExtraExpanded),
                 9 => Ok(FontStretch::UltraExpanded),
                 _ => Err(PyValueError::new_err("Invalid font stretch")),
             })
             .transpose()?;
         let color = ob
             .getattr("color")?
-            .extract::<Option<&str>>()?
+            .extract::<Option<PyBackedStr>>()?
             .map(|c| -> PyResult<_> {
                 if c.trim() == "empty" {
                     Ok(None)
                 } else {
-                    Ok(Some(Color::from_str(c)?))
+                    Ok(Some(Color::from_str(c.deref())?))
                 }
             })
             .transpose()?;
         let stroke_attr = ob.getattr("stroke")?;
-        let stroke = if let Ok(s) = stroke_attr.extract::<&str>() {
-            if s == "empty" {
+        let stroke = if let Ok(s) = stroke_attr.extract::<PyBackedStr>() {
+            if s.deref() == "empty" {
                 Some(None)
             } else {
                 return Err(PyValueError::new_err("Invalid stroke value"));
             }
         } else {
             stroke_attr.extract::<Option<Stroke>>()?.map(Some)
         };
```

### Comparing `nelsie-0.5.0/src/render/core.rs` & `nelsie-0.6.0/src/render/core.rs`

 * *Files 10% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-use crate::model::{FontData, Resources, Slide, Step};
+use crate::model::{FontData, Resources, Slide, SlideId, Step};
 use crate::render::counters::CountersMap;
 use crate::render::rendering::render_to_svg_tree;
 use crate::render::OutputFormat;
 use crate::NelsieError;
 use crate::Result;
 use resvg::tiny_skia;
 use std::path::Path;
@@ -10,15 +10,15 @@
 use svg2pdf::usvg;
 use svg2pdf::usvg::{PostProcessingSteps, TreePostProc};
 use usvg::{TreeWriting, XmlOptions};
 
 pub(crate) struct RenderConfig<'a> {
     pub resources: &'a Resources,
     pub slide: &'a Slide,
-    pub slide_idx: usize,
+    pub slide_id: SlideId,
     pub step: Step,
     pub default_font: &'a Arc<FontData>,
     pub output_format: OutputFormat,
     pub output_path: Option<&'a Path>,
     pub counter_values: &'a CountersMap<'a>,
 }
 
@@ -55,19 +55,28 @@
                     .map_err(|e| NelsieError::Generic(e.to_string()))?,
             )
         }
     };
 
     if let Some(path) = render_cfg.output_path {
         if let RenderingResult::BytesData(data) = result {
+            let counter = render_cfg.counter_values.get("global").unwrap();
+            let page_idx = counter
+                .indices
+                .get(&(render_cfg.slide_id, render_cfg.step))
+                .unwrap()
+                .page_idx;
+            let padding = counter.n_pages.to_string().len();
             let final_path = path.join(format!(
-                "{}-{}.{}",
-                render_cfg.slide_idx,
+                "{:0padding$}-{}-{}.{}",
+                page_idx,
+                render_cfg.slide_id,
                 render_cfg.step,
-                render_cfg.output_format.extension()
+                render_cfg.output_format.extension(),
+                padding = padding,
             ));
             std::fs::write(&final_path, data).map_err(|e| {
                 NelsieError::Generic(format!(
                     "Cannot write output file: {}: {}",
                     final_path.display(),
                     e
                 ))
```

### Comparing `nelsie-0.5.0/src/render/image.rs` & `nelsie-0.6.0/src/render/image.rs`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/src/render/layout.rs` & `nelsie-0.6.0/src/render/layout.rs`

 * *Files 0% similar despite different names*

```diff
@@ -230,15 +230,15 @@
 ) -> (f32, f32) {
     match content {
         NodeContent::Text(text) => {
             let mut t = text.text_style_at_step(step);
             if text.parse_counters {
                 // Here we do not "step" but "self.config.step" as we want to escape "replace_steps"
                 // for counters
-                replace_counters(config.counter_values, &mut t, config.slide_idx, config.step);
+                replace_counters(config.counter_values, &mut t, config.slide_id, config.step);
             }
             let (width, height, text_layout) = get_text_layout(
                 config.resources,
                 &t,
                 text.text_align,
                 &text.parsed_text.at_step(step).anchors,
             );
```

### Comparing `nelsie-0.5.0/src/render/mod.rs` & `nelsie-0.6.0/src/render/mod.rs`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 mod pdf;
 mod rendering;
 mod text;
 
 use crate::common::error::NelsieError;
 use crate::common::fileutils::ensure_directory;
 
-use crate::model::{FontData, Resources, Slide, SlideDeck};
+use crate::model::{FontData, Resources, Slide, SlideDeck, SlideId};
 use crate::render::core::RenderingResult;
 pub(crate) use core::{render_slide_step, RenderConfig};
 pub(crate) use pdf::PdfBuilder;
 
 use crate::render::counters::{compute_counters, CountersMap};
 use std::path::Path;
 use std::sync::Arc;
@@ -62,26 +62,26 @@
         }
     }
 }
 
 fn render_slide(
     resources: &Resources,
     output_cfg: &OutputConfig,
-    slide_idx: usize,
+    slide_id: SlideId,
     slide: &Slide,
     default_font: &Arc<FontData>,
     counter_values: &CountersMap,
 ) -> crate::Result<Vec<RenderingResult>> {
-    log::debug!("Rendering slide {}", slide_idx);
+    log::debug!("Rendering slide {}", slide_id);
     (1..=slide.n_steps)
         .map(|step| {
             let render_cfg = RenderConfig {
                 resources,
                 slide,
-                slide_idx,
+                slide_id,
                 step,
                 default_font,
                 output_format: output_cfg.format,
                 output_path: output_cfg.path,
                 counter_values,
             };
             render_slide_step(&render_cfg)
@@ -100,17 +100,17 @@
         println!(
             "Slides construction: {:.2}s",
             (start_time - slide_deck.creation_time).as_secs_f32()
         );
     }
 
     let counter_values = compute_counters(slide_deck);
-    let n_pages = counter_values.get("global").unwrap().n_pages;
+    let global_counter = counter_values.get("global").unwrap();
     let mut pdf_builder = if let OutputFormat::Pdf = output_cfg.format {
-        Some(PdfBuilder::new(n_pages))
+        Some(PdfBuilder::new(global_counter.n_pages))
     } else {
         if let Some(dir) = output_cfg.path {
             log::debug!("Ensuring output directory: {}", dir.display());
             ensure_directory(dir).map_err(|e| {
                 NelsieError::Generic(format!(
                     "Cannot create directory for output files: {}: {}",
                     dir.display(),
@@ -119,43 +119,56 @@
             })?;
         }
         None
     };
 
     let mut result_data = Vec::new();
 
+    if output_cfg.path.is_none() {
+        result_data.resize(global_counter.n_pages as usize, (0, 0, Vec::new()))
+    }
+
     let mut pdf_compose_time = Duration::ZERO;
 
     let progress_bar = if verbose_level.is_normal_or_more() {
-        Some(indicatif::ProgressBar::new(n_pages.into()))
+        Some(indicatif::ProgressBar::new(global_counter.n_pages.into()))
     } else {
         None
     };
 
     for (slide_idx, slide) in slide_deck.slides.iter().enumerate() {
         for (step_idx, result) in render_slide(
             resources,
             output_cfg,
-            slide_idx,
+            slide_idx as SlideId,
             slide,
             &slide_deck.default_font,
             &counter_values,
         )?
         .into_iter()
         .enumerate()
         {
+            let page_idx = global_counter
+                .indices
+                .get(&(slide_idx as u32, (step_idx + 1) as u32))
+                .unwrap()
+                .page_idx as usize;
+
             match result {
                 RenderingResult::None => { /* Do nothing */ }
                 RenderingResult::Tree(tree) => {
                     let s = std::time::Instant::now();
-                    pdf_builder.as_mut().unwrap().add_page_from_svg(tree);
+                    pdf_builder
+                        .as_mut()
+                        .unwrap()
+                        .add_page_from_svg(page_idx, tree);
                     pdf_compose_time += std::time::Instant::now() - s;
                 }
                 RenderingResult::BytesData(data) => {
-                    result_data.push((slide_idx, step_idx, data));
+                    result_data[page_idx] = (slide_idx, step_idx, data);
                 }
             }
             if let Some(bar) = &progress_bar {
                 bar.inc(1);
             }
         }
     }
```

### Comparing `nelsie-0.5.0/src/render/paths.rs` & `nelsie-0.6.0/src/render/paths.rs`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/src/render/pdf.rs` & `nelsie-0.6.0/src/render/pdf.rs`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,14 @@
 use pdf_writer::{Content, Name, Rect, Ref};
 use std::path::Path;
 use svg2pdf::usvg;
 
 pub(crate) struct PdfBuilder {
     pdf: pdf_writer::Pdf,
     page_ids: Vec<Ref>,
-    page_idx: usize,
     alloc_ref: Ref,
     page_tree_id: Ref,
 }
 
 impl PdfBuilder {
     pub fn new(n_pages: u32) -> Self {
         let mut pdf = pdf_writer::Pdf::new();
@@ -26,36 +25,29 @@
         pdf.pages(page_tree_id)
             .kids(page_ids.iter().copied())
             .count(page_ids.len() as i32);
 
         PdfBuilder {
             pdf,
             page_ids,
-            page_idx: 0,
             alloc_ref,
             page_tree_id,
         }
     }
 
-    pub fn add_page_from_svg(&mut self, tree: usvg::Tree) {
-        let page_id = self.page_ids[self.page_idx];
+    pub fn add_page_from_svg(&mut self, page_idx: usize, tree: usvg::Tree) {
+        let page_id = self.page_ids[page_idx];
 
         let content_id = self.alloc_ref.bump();
         let mut page = self.pdf.page(page_id);
         page.media_box(Rect::new(0.0, 0.0, tree.size.width(), tree.size.height()));
         page.parent(self.page_tree_id);
-        // page.group()
-        //     .transparency()
-        //     .isolated(true)
-        //     .knockout(false)
-        //     .color_space()
-        //     .srgb();
         page.contents(content_id);
 
-        let name_str = format!("S{}", self.page_idx);
+        let name_str = format!("S{}", page_idx);
         let svg_name = Name(name_str.as_bytes());
         let mut resources = page.resources();
 
         let svg_id = self.alloc_ref.bump(); // !!! no .bump has to occur until convert_tree_into !!!
 
         resources.x_objects().pair(svg_name, svg_id);
         resources.finish();
@@ -64,16 +56,14 @@
         self.alloc_ref =
             svg2pdf::convert_tree_into(&tree, svg2pdf::Options::default(), &mut self.pdf, svg_id);
         let mut content = Content::new();
         content
             .transform([tree.size.width(), 0.0, 0.0, tree.size.height(), 0.0, 0.0])
             .x_object(svg_name);
         self.pdf.stream(content_id, &content.finish());
-
-        self.page_idx += 1;
     }
 
     pub fn write(self, path: &Path) -> crate::Result<()> {
         std::fs::write(path, self.pdf.finish())?;
         Ok(())
     }
 }
```

### Comparing `nelsie-0.5.0/src/render/rendering.rs` & `nelsie-0.6.0/src/render/rendering.rs`

 * *Files 0% similar despite different names*

```diff
@@ -136,15 +136,15 @@
                         let mut t = text.text_style_at_step(step);
                         if text.parse_counters {
                             // Here we do not "step" but "self.config.step" as we want to escape "replace_steps"
                             // for counters
                             replace_counters(
                                 self.config.counter_values,
                                 &mut t,
-                                self.config.slide_idx,
+                                self.config.slide_id,
                                 self.config.step,
                             );
                         }
                         self.svg_node.children.push(render_text(
                             &t,
                             match text.text_align {
                                 TextAlign::Start => rect.x,
```

### Comparing `nelsie-0.5.0/src/render/text.rs` & `nelsie-0.6.0/src/render/text.rs`

 * *Files 2% similar despite different names*

```diff
@@ -127,14 +127,17 @@
     };
 
     (width, text.height(), result)
 }
 
 fn get_text_width(resources: &Resources, text: &StyledText) -> f32 {
     assert_eq!(text.styled_lines.len(), 1);
+    if text.styled_lines[0].text.is_empty() {
+        return 0f32;
+    }
     let text_node = render_text(text, 0.0, 0.0, TextAlign::Start);
     let mut root_node = usvg::Group::default();
     root_node.children.push(text_node);
     let size = usvg::Size::from_wh(8000.0, 6000.0).unwrap();
     let mut tree = Tree {
         size,
         view_box: usvg::ViewBox {
@@ -170,16 +173,16 @@
         } else {
             break;
         }
     }
     width
 }
 
-fn create_svg_span(text_styles: &[TextStyle], chunk: &Span, start: usize) -> (TextSpan, usize) {
-    let text_style = &text_styles[chunk.style_idx as usize];
+fn create_svg_span(text_styles: &[TextStyle], span: &Span, start: usize) -> (TextSpan, usize) {
+    let text_style = &text_styles[span.style_idx as usize];
     let fill = text_style.color.as_ref().map(|color| Fill {
         paint: usvg::Paint::Color(color.into()),
         opacity: color.opacity(),
         rule: Default::default(),
     });
     let font = Font {
         families: vec![text_style.font.family_name.clone()],
@@ -193,15 +196,15 @@
     };
     let decoration = TextDecoration {
         underline: None,
         overline: None,
         line_through: None,
     };
     let stroke = text_style.stroke.as_ref().map(|s| stroke_to_usvg_stroke(s));
-    let end = start + chunk.length as usize;
+    let end = start + span.length as usize;
     (
         TextSpan {
             start,
             end,
             fill,
             stroke,
             paint_order: PaintOrder::FillAndStroke,
@@ -234,14 +237,15 @@
     TextChunk {
         x: Some(x),
         y: Some(y),
         anchor,
         spans: styled_line
             .spans
             .iter()
+            .filter(|span| span.length > 0)
             .map(|span| {
                 let (span, new_pos) = create_svg_span(text_styles, span, pos);
                 pos = new_pos;
                 span
             })
             .collect(),
         text_flow: TextFlow::Linear,
```

### Comparing `nelsie-0.5.0/tests/assets/fonts/DejaVuSans-Bold.ttf` & `nelsie-0.6.0/tests/assets/fonts/DejaVuSans-Bold.ttf`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/assets/fonts/DejaVuSans-BoldOblique.ttf` & `nelsie-0.6.0/tests/assets/fonts/DejaVuSans-BoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/assets/fonts/DejaVuSans-ExtraLight.ttf` & `nelsie-0.6.0/tests/assets/fonts/DejaVuSans-ExtraLight.ttf`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/assets/fonts/DejaVuSans-Oblique.ttf` & `nelsie-0.6.0/tests/assets/fonts/DejaVuSans-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/assets/fonts/DejaVuSans.ttf` & `nelsie-0.6.0/tests/assets/fonts/DejaVuSans.ttf`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/assets/fonts/DejaVuSansCondensed-Bold.ttf` & `nelsie-0.6.0/tests/assets/fonts/DejaVuSansCondensed-Bold.ttf`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/assets/fonts/DejaVuSansCondensed-BoldOblique.ttf` & `nelsie-0.6.0/tests/assets/fonts/DejaVuSansCondensed-BoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/assets/fonts/DejaVuSansCondensed-Oblique.ttf` & `nelsie-0.6.0/tests/assets/fonts/DejaVuSansCondensed-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/assets/fonts/DejaVuSansCondensed.ttf` & `nelsie-0.6.0/tests/assets/fonts/DejaVuSansCondensed.ttf`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/assets/fonts/DejaVuSansMono-Bold.ttf` & `nelsie-0.6.0/tests/assets/fonts/DejaVuSansMono-Bold.ttf`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/assets/fonts/DejaVuSansMono-BoldOblique.ttf` & `nelsie-0.6.0/tests/assets/fonts/DejaVuSansMono-BoldOblique.ttf`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/assets/fonts/DejaVuSansMono-Oblique.ttf` & `nelsie-0.6.0/tests/assets/fonts/DejaVuSansMono-Oblique.ttf`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/assets/fonts/DejaVuSansMono.ttf` & `nelsie-0.6.0/tests/assets/fonts/DejaVuSansMono.ttf`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/assets/knight.svg` & `nelsie-0.6.0/tests/assets/knight.svg`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/assets/test.ora` & `nelsie-0.6.0/tests/assets/test.ora`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/assets/test.svg` & `nelsie-0.6.0/tests/assets/test.svg`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/assets/testimg.jpeg` & `nelsie-0.6.0/tests/assets/testimg.jpeg`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/assets/testimg.png` & `nelsie-0.6.0/tests/assets/testimg.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/active_next_last_keywords/0-1.png` & `nelsie-0.6.0/tests/checks/active_next_last_keywords/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/active_next_last_keywords/0-2.png` & `nelsie-0.6.0/tests/checks/active_next_last_keywords/1-0-2.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/active_next_last_keywords/0-3.png` & `nelsie-0.6.0/tests/checks/active_next_last_keywords/2-0-3.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/active_next_last_keywords/0-4.png` & `nelsie-0.6.0/tests/checks/active_next_last_keywords/3-0-4.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/active_steps/0-1.png` & `nelsie-0.6.0/tests/checks/active_steps/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/active_steps/0-2.png` & `nelsie-0.6.0/tests/checks/active_steps/1-0-2.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/active_steps/0-3.png` & `nelsie-0.6.0/tests/checks/active_steps/2-0-3.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/array_text_in_steps/0-1.png` & `nelsie-0.6.0/tests/checks/array_text_in_steps/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/array_text_in_steps/0-2.png` & `nelsie-0.6.0/tests/checks/array_text_in_steps/1-0-2.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/array_text_in_steps/0-3.png` & `nelsie-0.6.0/tests/checks/array_text_in_steps/2-0-3.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/bg_color_opacity/0-1.png` & `nelsie-0.6.0/tests/checks/bg_color_opacity/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/box_border_radius/0-1.png` & `nelsie-0.6.0/tests/checks/box_border_radius/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/box_debug_frame/0-1.png` & `nelsie-0.6.0/tests/checks/box_debug_frame/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/chessboard/0-1.png` & `nelsie-0.6.0/tests/checks/chessboard/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/chessboard/0-2.png` & `nelsie-0.6.0/tests/checks/chessboard/1-0-2.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/chessboard/0-3.png` & `nelsie-0.6.0/tests/checks/chessboard/2-0-3.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/chessboard/0-4.png` & `nelsie-0.6.0/tests/checks/chessboard/3-0-4.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/code_language_default/0-1.png` & `nelsie-0.6.0/tests/checks/code_language_default/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/code_language_none/0-1.png` & `nelsie-0.6.0/tests/checks/code_language_none/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/code_rust_syntax_highlight/0-1.png` & `nelsie-0.6.0/tests/checks/code_rust_syntax_highlight/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/code_rust_syntax_highlight/1-1.png` & `nelsie-0.6.0/tests/checks/code_rust_syntax_highlight/1-1-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/code_style_delimiters/0-1.png` & `nelsie-0.6.0/tests/checks/code_style_delimiters/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/code_syntax_highlight_anchors/0-1.png` & `nelsie-0.6.0/tests/checks/code_syntax_highlight_anchors/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/code_syntax_highlight_with_styles/0-1.png` & `nelsie-0.6.0/tests/checks/code_syntax_highlight_with_styles/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/expr_x_y_weight_height/0-1.png` & `nelsie-0.6.0/tests/checks/expr_x_y_weight_height/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/fix_sizes/0-1.png` & `nelsie-0.6.0/tests/checks/fix_sizes/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/layout_directions/0-1.png` & `nelsie-0.6.0/tests/checks/layout_directions/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/layout_directions/1-1.png` & `nelsie-0.6.0/tests/checks/layout_directions/1-1-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/layout_directions/2-1.png` & `nelsie-0.6.0/tests/checks/layout_directions/2-2-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/layout_directions/3-1.png` & `nelsie-0.6.0/tests/checks/layout_directions/3-3-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/layout_flex_grow/0-1.png` & `nelsie-0.6.0/tests/checks/layout_flex_grow/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/layout_flex_wrap/0-1.png` & `nelsie-0.6.0/tests/checks/layout_flex_wrap/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/layout_gap/0-1.png` & `nelsie-0.6.0/tests/checks/layout_gap/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/layout_gap/1-1.png` & `nelsie-0.6.0/tests/checks/layout_gap/1-1-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/layout_gap/2-1.png` & `nelsie-0.6.0/tests/checks/layout_gap/2-2-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/layout_justify_content/0-1.png` & `nelsie-0.6.0/tests/checks/layout_justify_content/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/layout_justify_content/1-1.png` & `nelsie-0.6.0/tests/checks/layout_justify_content/1-1-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/layout_justify_content/2-1.png` & `nelsie-0.6.0/tests/checks/layout_justify_content/2-2-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/layout_justify_content/3-1.png` & `nelsie-0.6.0/tests/checks/layout_justify_content/3-3-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/layout_margin/0-1.png` & `nelsie-0.6.0/tests/checks/layout_margin/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/layout_padding/0-1.png` & `nelsie-0.6.0/tests/checks/layout_padding/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/layout_position/0-1.png` & `nelsie-0.6.0/tests/checks/layout_position/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/layout_position/1-1.png` & `nelsie-0.6.0/tests/checks/layout_position/1-1-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/layout_position/2-1.png` & `nelsie-0.6.0/tests/checks/layout_position/2-2-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/layout_position/3-1.png` & `nelsie-0.6.0/tests/checks/layout_position/3-3-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/layout_position/4-1.png` & `nelsie-0.6.0/tests/checks/layout_position/4-4-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/layout_position_string/0-1.png` & `nelsie-0.6.0/tests/checks/layout_position_string/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/line_box/0-1.png` & `nelsie-0.6.0/tests/checks/line_box/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/list/0-1.png` & `nelsie-0.6.0/tests/checks/list/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/m_xy_p_xy/0-1.png` & `nelsie-0.6.0/tests/checks/m_xy_p_xy/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/m_xy_p_xy/1-1.png` & `nelsie-0.6.0/tests/checks/m_xy_p_xy/1-1-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/path_arrows/0-1.png` & `nelsie-0.6.0/tests/checks/path_arrows/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/path_arrows/1-1.png` & `nelsie-0.6.0/tests/checks/path_arrows/1-1-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/path_box_positions/0-1.png` & `nelsie-0.6.0/tests/checks/path_box_positions/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/path_close/0-1.png` & `nelsie-0.6.0/tests/checks/path_close/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/path_opacity/0-1.png` & `nelsie-0.6.0/tests/checks/path_opacity/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/path_oval/0-1.png` & `nelsie-0.6.0/tests/checks/path_oval/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/path_text_line_positions/0-1.png` & `nelsie-0.6.0/tests/checks/path_text_line_positions/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_cubic/0-1.png` & `nelsie-0.6.0/tests/checks/render_cubic/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_ora_image_no_steps/0-1.png` & `nelsie-0.6.0/tests/checks/render_ora_image_no_steps/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_ora_image_scale/0-1.png` & `nelsie-0.6.0/tests/checks/render_ora_image_scale/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_ora_image_steps/0-1.png` & `nelsie-0.6.0/tests/checks/render_ora_image_steps/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_ora_image_steps/0-2.png` & `nelsie-0.6.0/tests/checks/render_ora_image_steps/1-0-2.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_ora_image_steps/0-3.png` & `nelsie-0.6.0/tests/checks/render_ora_image_steps/2-0-3.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_path_dash/0-1.png` & `nelsie-0.6.0/tests/checks/render_path_dash/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_path_steps/0-1.png` & `nelsie-0.6.0/tests/checks/render_path_steps/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_path_steps/0-2.png` & `nelsie-0.6.0/tests/checks/render_path_steps/1-0-2.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_path_steps/0-3.png` & `nelsie-0.6.0/tests/checks/render_path_steps/2-0-3.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_path_steps/0-4.png` & `nelsie-0.6.0/tests/checks/render_path_steps/3-0-4.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_paths/0-1.png` & `nelsie-0.6.0/tests/checks/render_paths/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_raster_image_forced_size/0-1.png` & `nelsie-0.6.0/tests/checks/render_raster_image_forced_size/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_raster_image_forced_size/1-1.png` & `nelsie-0.6.0/tests/checks/render_raster_image_forced_size/1-1-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_raster_image_forced_size/2-1.png` & `nelsie-0.6.0/tests/checks/render_raster_image_forced_size/2-2-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_raster_image_forced_size/3-1.png` & `nelsie-0.6.0/tests/checks/render_raster_image_forced_size/3-3-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_raster_image_forced_size/4-1.png` & `nelsie-0.6.0/tests/checks/render_raster_image_forced_size/4-4-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_raster_image_native_size/0-1.png` & `nelsie-0.6.0/tests/checks/render_raster_image_native_size/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_steps/0-1.png` & `nelsie-0.6.0/tests/checks/render_steps/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_steps/0-2.png` & `nelsie-0.6.0/tests/checks/render_steps/1-0-2.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_steps/0-3.png` & `nelsie-0.6.0/tests/checks/render_steps/2-0-3.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_svg_image_no_steps/0-1.png` & `nelsie-0.6.0/tests/checks/render_svg_image_no_steps/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_svg_image_shift/0-1.png` & `nelsie-0.6.0/tests/checks/render_svg_image_shift/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_svg_image_shift/0-2.png` & `nelsie-0.6.0/tests/checks/render_svg_image_shift/1-0-2.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_svg_image_shift/0-3.png` & `nelsie-0.6.0/tests/checks/render_svg_image_shift/2-0-3.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_svg_image_shift/0-4.png` & `nelsie-0.6.0/tests/checks/render_svg_image_shift/3-0-4.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_svg_image_shift/0-5.png` & `nelsie-0.6.0/tests/checks/render_svg_image_shift/4-0-5.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_svg_image_shift/0-6.png` & `nelsie-0.6.0/tests/checks/render_svg_image_shift/5-0-6.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_svg_image_steps/0-1.png` & `nelsie-0.6.0/tests/checks/render_svg_image_steps/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_svg_image_steps/0-2.png` & `nelsie-0.6.0/tests/checks/render_svg_image_steps/1-0-2.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_svg_image_steps/0-3.png` & `nelsie-0.6.0/tests/checks/render_svg_image_steps/2-0-3.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_svg_image_steps/0-4.png` & `nelsie-0.6.0/tests/checks/render_svg_image_steps/3-0-4.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_text_basic/0-1.png` & `nelsie-0.6.0/tests/checks/render_text_basic/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_text_basic/1-1.png` & `nelsie-0.6.0/tests/checks/render_text_basic/1-1-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_text_basic/2-1.png` & `nelsie-0.6.0/tests/checks/render_text_basic/2-2-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_text_basic/3-1.png` & `nelsie-0.6.0/tests/checks/render_text_basic/3-3-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_text_steps/0-1.png` & `nelsie-0.6.0/tests/checks/render_text_steps/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_text_steps/0-2.png` & `nelsie-0.6.0/tests/checks/render_text_steps/1-0-2.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/render_text_unicode/0-1.png` & `nelsie-0.6.0/tests/checks/render_text_unicode/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/replace_steps/0-1.png` & `nelsie-0.6.0/tests/checks/replace_steps/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/replace_steps/0-2.png` & `nelsie-0.6.0/tests/checks/replace_steps/1-0-2.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/replace_steps/0-3.png` & `nelsie-0.6.0/tests/checks/replace_steps/2-0-3.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/replace_steps/0-4.png` & `nelsie-0.6.0/tests/checks/replace_steps/3-0-4.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/show_next_last_keywords/0-1.png` & `nelsie-0.6.0/tests/checks/show_next_last_keywords/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/show_next_last_keywords/0-2.png` & `nelsie-0.6.0/tests/checks/show_next_last_keywords/1-0-2.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/show_next_last_keywords/0-3.png` & `nelsie-0.6.0/tests/checks/show_next_last_keywords/2-0-3.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/show_next_last_keywords/0-4.png` & `nelsie-0.6.0/tests/checks/show_next_last_keywords/3-0-4.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/show_steps/0-1.png` & `nelsie-0.6.0/tests/checks/show_steps/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/show_steps/0-2.png` & `nelsie-0.6.0/tests/checks/show_steps/1-0-2.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/show_steps/0-3.png` & `nelsie-0.6.0/tests/checks/show_steps/2-0-3.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/show_steps/0-4.png` & `nelsie-0.6.0/tests/checks/show_steps/3-0-4.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/slide_decorator/0-1.png` & `nelsie-0.6.0/tests/checks/slide_decorator/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/slide_decorator/1-1.png` & `nelsie-0.6.0/tests/checks/slide_decorator/1-1-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/step_global_counter/0-1.png` & `nelsie-0.6.0/tests/checks/step_global_counter/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/step_global_counter/0-2.png` & `nelsie-0.6.0/tests/checks/step_global_counter/1-0-2.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/step_global_counter/1-1.png` & `nelsie-0.6.0/tests/checks/step_global_counter/2-1-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/step_global_counter/2-1.png` & `nelsie-0.6.0/tests/checks/step_global_counter/3-2-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/step_invalid_counter/0-1.png` & `nelsie-0.6.0/tests/checks/step_invalid_counter/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/step_other_counter/0-1.png` & `nelsie-0.6.0/tests/checks/step_other_counter/6-4-1.png`

 * *Files 24% similar despite different names*

#### sng

```diff
@@ -15,24 +15,24 @@
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 787878ff 606060ff 686868ff 808080ff 808080ff 808080ff 808080ff 808080ff 707070ff 707070ff 808080ff 707070ff 606060ff 606060ff 787878ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 787878ff 606060ff 707070ff 808080ff 808080ff 808080ff 808080ff 808080ff 707070ff 707070ff 808080ff 686868ff 606060ff 606060ff 707070ff 808080ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 686868ff 101010ff 282828ff 101010ff 303030ff 808080ff 808080ff 808080ff 808080ff 303030ff 505050ff 484848ff 080808ff 202020ff 202020ff 080808ff 606060ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 505050ff 101010ff 282828ff 101010ff 383838ff 808080ff 808080ff 808080ff 808080ff 282828ff 585858ff 606060ff 101010ff 202020ff 202020ff 000000ff 505050ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 101010ff 484848ff 808080ff 787878ff 080808ff 686868ff 808080ff 808080ff 808080ff 080808ff 787878ff 707070ff 808080ff 808080ff 808080ff 484848ff 181818ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 101010ff 585858ff 808080ff 787878ff 000000ff 707070ff 808080ff 808080ff 787878ff 080808ff 808080ff 808080ff 808080ff 808080ff 808080ff 505050ff 101010ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 686868ff 000000ff 808080ff 808080ff 808080ff 303030ff 404040ff 808080ff 808080ff 585858ff 282828ff 808080ff 808080ff 808080ff 808080ff 808080ff 585858ff 080808ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 606060ff 000000ff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 585858ff 303030ff 808080ff 808080ff 808080ff 808080ff 808080ff 585858ff 101010ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 606060ff 080808ff 808080ff 808080ff 808080ff 404040ff 282828ff 808080ff 808080ff 383838ff 505050ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 383838ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 606060ff 202020ff 808080ff 808080ff 808080ff 404040ff 404040ff 808080ff 808080ff 303030ff 505050ff 808080ff 808080ff 808080ff 404040ff 282828ff 181818ff 686868ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 606060ff 101010ff 808080ff 808080ff 808080ff 404040ff 202020ff 808080ff 808080ff 101010ff 707070ff 808080ff 808080ff 808080ff 808080ff 303030ff 181818ff 787878ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 505050ff 202020ff 808080ff 808080ff 808080ff 404040ff 303030ff 808080ff 808080ff 080808ff 787878ff 808080ff 808080ff 808080ff 404040ff 404040ff 101010ff 404040ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 606060ff 000000ff 808080ff 808080ff 808080ff 404040ff 404040ff 808080ff 686868ff 181818ff 808080ff 808080ff 808080ff 808080ff 303030ff 181818ff 787878ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 606060ff 080808ff 808080ff 808080ff 808080ff 303030ff 404040ff 808080ff 585858ff 282828ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 707070ff 000000ff 787878ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 787878ff 080808ff 686868ff 808080ff 808080ff 181818ff 505050ff 808080ff 383838ff 484848ff 808080ff 808080ff 808080ff 303030ff 181818ff 787878ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 787878ff 000000ff 707070ff 808080ff 808080ff 101010ff 585858ff 808080ff 383838ff 484848ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 707070ff 000000ff 787878ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 383838ff 181818ff 606060ff 383838ff 101010ff 808080ff 808080ff 181818ff 686868ff 808080ff 808080ff 484848ff 000000ff 383838ff 404040ff 404040ff 404040ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 383838ff 181818ff 606060ff 303030ff 181818ff 808080ff 808080ff 101010ff 707070ff 808080ff 808080ff 585858ff 484848ff 606060ff 585858ff 181818ff 282828ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 484848ff 282828ff 383838ff 787878ff 808080ff 707070ff 101010ff 808080ff 808080ff 808080ff 606060ff 404040ff 404040ff 404040ff 404040ff 404040ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 484848ff 282828ff 383838ff 787878ff 808080ff 686868ff 181818ff 808080ff 808080ff 808080ff 686868ff 303030ff 202020ff 282828ff 505050ff 808080ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 606060ff 606060ff 707070ff 808080ff 808080ff 808080ff 808080ff 808080ff 707070ff 707070ff 808080ff 707070ff 606060ff 606060ff 787878ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 606060ff 707070ff 808080ff 808080ff 808080ff 808080ff 707070ff 707070ff 808080ff 808080ff 808080ff 787878ff 606060ff 787878ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 686868ff 080808ff 202020ff 202020ff 080808ff 404040ff 808080ff 808080ff 808080ff 808080ff 303030ff 505050ff 484848ff 080808ff 202020ff 202020ff 080808ff 606060ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 484848ff 000000ff 404040ff 808080ff 808080ff 808080ff 808080ff 282828ff 585858ff 808080ff 808080ff 808080ff 202020ff 000000ff 606060ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 707070ff 707070ff 808080ff 808080ff 686868ff 000000ff 707070ff 808080ff 808080ff 808080ff 080808ff 787878ff 707070ff 808080ff 808080ff 808080ff 484848ff 181818ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 707070ff 181818ff 181818ff 404040ff 808080ff 808080ff 808080ff 787878ff 080808ff 808080ff 808080ff 808080ff 484848ff 383838ff 000000ff 606060ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 808080ff 808080ff 000000ff 606060ff 808080ff 808080ff 585858ff 282828ff 808080ff 808080ff 808080ff 808080ff 808080ff 585858ff 080808ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 606060ff 202020ff 404040ff 808080ff 808080ff 808080ff 585858ff 303030ff 808080ff 808080ff 707070ff 101010ff 787878ff 000000ff 606060ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 808080ff 484848ff 101010ff 808080ff 808080ff 808080ff 383838ff 505050ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 383838ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 484848ff 282828ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 303030ff 505050ff 808080ff 808080ff 282828ff 585858ff 808080ff 000000ff 606060ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 606060ff 080808ff 686868ff 808080ff 808080ff 808080ff 101010ff 707070ff 808080ff 808080ff 808080ff 808080ff 303030ff 181818ff 787878ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 787878ff 101010ff 787878ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 080808ff 787878ff 808080ff 585858ff 282828ff 808080ff 808080ff 000000ff 606060ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 686868ff 101010ff 686868ff 808080ff 808080ff 808080ff 686868ff 181818ff 808080ff 808080ff 808080ff 808080ff 303030ff 181818ff 787878ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 404040ff 202020ff 404040ff 404040ff 101010ff 202020ff 505050ff 808080ff 585858ff 282828ff 808080ff 808080ff 080808ff 303030ff 404040ff 404040ff 000000ff 303030ff 606060ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 686868ff 101010ff 686868ff 808080ff 808080ff 808080ff 808080ff 383838ff 484848ff 808080ff 808080ff 808080ff 303030ff 181818ff 787878ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 606060ff 404040ff 404040ff 404040ff 101010ff 202020ff 505050ff 808080ff 383838ff 484848ff 808080ff 808080ff 404040ff 404040ff 404040ff 404040ff 000000ff 303030ff 606060ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 707070ff 080808ff 282828ff 404040ff 404040ff 404040ff 707070ff 808080ff 181818ff 686868ff 808080ff 808080ff 484848ff 000000ff 383838ff 404040ff 404040ff 404040ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 101010ff 707070ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 000000ff 606060ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 707070ff 404040ff 404040ff 404040ff 404040ff 404040ff 707070ff 707070ff 101010ff 808080ff 808080ff 808080ff 606060ff 404040ff 404040ff 404040ff 404040ff 404040ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 505050ff 606060ff 808080ff 686868ff 181818ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 404040ff 707070ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 585858ff 484848ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 505050ff 505050ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff
```

### Comparing `nelsie-0.5.0/tests/checks/step_other_counter/1-1.png` & `nelsie-0.6.0/tests/checks/step_other_counter/0-0-1.png`

 * *Files 17% similar despite different names*

#### sng

```diff
@@ -15,24 +15,24 @@
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 606060ff 707070ff 808080ff 808080ff 808080ff 808080ff 808080ff 707070ff 707070ff 808080ff 707070ff 606060ff 606060ff 787878ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 606060ff 707070ff 808080ff 808080ff 808080ff 808080ff 808080ff 707070ff 707070ff 808080ff 686868ff 606060ff 606060ff 707070ff 808080ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 303030ff 000000ff 000000ff 404040ff 808080ff 808080ff 808080ff 808080ff 808080ff 303030ff 505050ff 484848ff 080808ff 202020ff 202020ff 080808ff 606060ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 303030ff 000000ff 000000ff 404040ff 808080ff 808080ff 808080ff 808080ff 808080ff 282828ff 585858ff 606060ff 101010ff 202020ff 202020ff 000000ff 505050ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 686868ff 787878ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 808080ff 080808ff 787878ff 707070ff 808080ff 808080ff 808080ff 484848ff 181818ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 686868ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 787878ff 080808ff 808080ff 808080ff 808080ff 808080ff 808080ff 505050ff 101010ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 585858ff 282828ff 808080ff 808080ff 808080ff 808080ff 808080ff 585858ff 080808ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 585858ff 303030ff 808080ff 808080ff 808080ff 808080ff 808080ff 585858ff 101010ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 383838ff 505050ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 383838ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 303030ff 505050ff 808080ff 808080ff 808080ff 404040ff 282828ff 181818ff 686868ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 101010ff 707070ff 808080ff 808080ff 808080ff 808080ff 303030ff 181818ff 787878ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 080808ff 787878ff 808080ff 808080ff 808080ff 404040ff 404040ff 101010ff 404040ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 686868ff 181818ff 808080ff 808080ff 808080ff 808080ff 303030ff 181818ff 787878ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 585858ff 282828ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 707070ff 000000ff 787878ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 383838ff 484848ff 808080ff 808080ff 808080ff 303030ff 181818ff 787878ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 383838ff 484848ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 707070ff 000000ff 787878ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 505050ff 404040ff 101010ff 202020ff 404040ff 606060ff 808080ff 181818ff 686868ff 808080ff 808080ff 484848ff 000000ff 383838ff 404040ff 404040ff 404040ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 505050ff 404040ff 101010ff 202020ff 404040ff 707070ff 808080ff 101010ff 707070ff 808080ff 808080ff 585858ff 484848ff 606060ff 585858ff 181818ff 282828ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 505050ff 404040ff 404040ff 404040ff 404040ff 606060ff 707070ff 101010ff 808080ff 808080ff 808080ff 606060ff 404040ff 404040ff 404040ff 404040ff 404040ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 505050ff 404040ff 404040ff 404040ff 404040ff 707070ff 686868ff 181818ff 808080ff 808080ff 808080ff 686868ff 303030ff 202020ff 282828ff 505050ff 808080ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 606060ff 707070ff 808080ff 808080ff 808080ff 808080ff 808080ff 707070ff 707070ff 808080ff 707070ff 606060ff 606060ff 787878ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 606060ff 707070ff 808080ff 808080ff 808080ff 808080ff 808080ff 707070ff 707070ff 808080ff 808080ff 808080ff 787878ff 606060ff 787878ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 303030ff 000000ff 000000ff 404040ff 808080ff 808080ff 808080ff 808080ff 808080ff 303030ff 505050ff 484848ff 080808ff 202020ff 202020ff 080808ff 606060ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 303030ff 000000ff 000000ff 404040ff 808080ff 808080ff 808080ff 808080ff 808080ff 282828ff 585858ff 808080ff 808080ff 808080ff 202020ff 000000ff 606060ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 686868ff 787878ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 808080ff 080808ff 787878ff 707070ff 808080ff 808080ff 808080ff 484848ff 181818ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 686868ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 787878ff 080808ff 808080ff 808080ff 808080ff 484848ff 383838ff 000000ff 606060ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 585858ff 282828ff 808080ff 808080ff 808080ff 808080ff 808080ff 585858ff 080808ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 585858ff 303030ff 808080ff 808080ff 707070ff 101010ff 787878ff 000000ff 606060ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 383838ff 505050ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 383838ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 303030ff 505050ff 808080ff 808080ff 282828ff 585858ff 808080ff 000000ff 606060ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 101010ff 707070ff 808080ff 808080ff 808080ff 808080ff 303030ff 181818ff 787878ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 080808ff 787878ff 808080ff 585858ff 282828ff 808080ff 808080ff 000000ff 606060ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 686868ff 181818ff 808080ff 808080ff 808080ff 808080ff 303030ff 181818ff 787878ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 585858ff 282828ff 808080ff 808080ff 080808ff 303030ff 404040ff 404040ff 000000ff 303030ff 606060ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 383838ff 484848ff 808080ff 808080ff 808080ff 303030ff 181818ff 787878ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 383838ff 484848ff 808080ff 808080ff 404040ff 404040ff 404040ff 404040ff 000000ff 303030ff 606060ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 505050ff 404040ff 101010ff 202020ff 404040ff 606060ff 808080ff 181818ff 686868ff 808080ff 808080ff 484848ff 000000ff 383838ff 404040ff 404040ff 404040ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 505050ff 404040ff 101010ff 202020ff 404040ff 707070ff 808080ff 101010ff 707070ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 000000ff 606060ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 505050ff 404040ff 404040ff 404040ff 404040ff 606060ff 707070ff 101010ff 808080ff 808080ff 808080ff 606060ff 404040ff 404040ff 404040ff 404040ff 404040ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 505050ff 404040ff 404040ff 404040ff 404040ff 707070ff 686868ff 181818ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 404040ff 707070ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 585858ff 484848ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 505050ff 505050ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff
```

### Comparing `nelsie-0.5.0/tests/checks/step_other_counter/2-1.png` & `nelsie-0.6.0/tests/checks/step_other_counter/2-2-1.png`

 * *Files 17% similar despite different names*

#### sng

```diff
@@ -15,24 +15,24 @@
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 606060ff 707070ff 808080ff 808080ff 808080ff 808080ff 808080ff 707070ff 707070ff 808080ff 707070ff 606060ff 606060ff 787878ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 606060ff 707070ff 808080ff 808080ff 808080ff 808080ff 808080ff 707070ff 707070ff 808080ff 686868ff 606060ff 606060ff 707070ff 808080ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 303030ff 000000ff 000000ff 404040ff 808080ff 808080ff 808080ff 808080ff 808080ff 303030ff 505050ff 484848ff 080808ff 202020ff 202020ff 080808ff 606060ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 303030ff 000000ff 000000ff 404040ff 808080ff 808080ff 808080ff 808080ff 808080ff 282828ff 585858ff 606060ff 101010ff 202020ff 202020ff 000000ff 505050ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 686868ff 787878ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 808080ff 080808ff 787878ff 707070ff 808080ff 808080ff 808080ff 484848ff 181818ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 686868ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 787878ff 080808ff 808080ff 808080ff 808080ff 808080ff 808080ff 505050ff 101010ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 585858ff 282828ff 808080ff 808080ff 808080ff 808080ff 808080ff 585858ff 080808ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 585858ff 303030ff 808080ff 808080ff 808080ff 808080ff 808080ff 585858ff 101010ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 383838ff 505050ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 383838ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 303030ff 505050ff 808080ff 808080ff 808080ff 404040ff 282828ff 181818ff 686868ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 101010ff 707070ff 808080ff 808080ff 808080ff 808080ff 303030ff 181818ff 787878ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 080808ff 787878ff 808080ff 808080ff 808080ff 404040ff 404040ff 101010ff 404040ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 686868ff 181818ff 808080ff 808080ff 808080ff 808080ff 303030ff 181818ff 787878ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 585858ff 282828ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 707070ff 000000ff 787878ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 383838ff 484848ff 808080ff 808080ff 808080ff 303030ff 181818ff 787878ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 383838ff 484848ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 707070ff 000000ff 787878ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 505050ff 404040ff 101010ff 202020ff 404040ff 606060ff 808080ff 181818ff 686868ff 808080ff 808080ff 484848ff 000000ff 383838ff 404040ff 404040ff 404040ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 505050ff 404040ff 101010ff 202020ff 404040ff 707070ff 808080ff 101010ff 707070ff 808080ff 808080ff 585858ff 484848ff 606060ff 585858ff 181818ff 282828ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
-ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 505050ff 404040ff 404040ff 404040ff 404040ff 606060ff 707070ff 101010ff 808080ff 808080ff 808080ff 606060ff 404040ff 404040ff 404040ff 404040ff 404040ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 505050ff 404040ff 404040ff 404040ff 404040ff 707070ff 686868ff 181818ff 808080ff 808080ff 808080ff 686868ff 303030ff 202020ff 282828ff 505050ff 808080ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 606060ff 707070ff 808080ff 808080ff 808080ff 808080ff 808080ff 707070ff 707070ff 808080ff 707070ff 606060ff 606060ff 787878ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 606060ff 707070ff 808080ff 808080ff 808080ff 808080ff 808080ff 707070ff 707070ff 808080ff 808080ff 808080ff 787878ff 606060ff 787878ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 303030ff 000000ff 000000ff 404040ff 808080ff 808080ff 808080ff 808080ff 808080ff 303030ff 505050ff 484848ff 080808ff 202020ff 202020ff 080808ff 606060ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 303030ff 000000ff 000000ff 404040ff 808080ff 808080ff 808080ff 808080ff 808080ff 282828ff 585858ff 808080ff 808080ff 808080ff 202020ff 000000ff 606060ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 686868ff 787878ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 808080ff 080808ff 787878ff 707070ff 808080ff 808080ff 808080ff 484848ff 181818ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 686868ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 787878ff 080808ff 808080ff 808080ff 808080ff 484848ff 383838ff 000000ff 606060ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 585858ff 282828ff 808080ff 808080ff 808080ff 808080ff 808080ff 585858ff 080808ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 585858ff 303030ff 808080ff 808080ff 707070ff 101010ff 787878ff 000000ff 606060ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 383838ff 505050ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 383838ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 303030ff 505050ff 808080ff 808080ff 282828ff 585858ff 808080ff 000000ff 606060ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 101010ff 707070ff 808080ff 808080ff 808080ff 808080ff 303030ff 181818ff 787878ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 808080ff 080808ff 787878ff 808080ff 585858ff 282828ff 808080ff 808080ff 000000ff 606060ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 686868ff 181818ff 808080ff 808080ff 808080ff 808080ff 303030ff 181818ff 787878ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 585858ff 282828ff 808080ff 808080ff 080808ff 303030ff 404040ff 404040ff 000000ff 303030ff 606060ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 383838ff 484848ff 808080ff 808080ff 808080ff 303030ff 181818ff 787878ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 202020ff 404040ff 808080ff 808080ff 808080ff 383838ff 484848ff 808080ff 808080ff 404040ff 404040ff 404040ff 404040ff 000000ff 303030ff 606060ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 505050ff 404040ff 101010ff 202020ff 404040ff 606060ff 808080ff 181818ff 686868ff 808080ff 808080ff 484848ff 000000ff 383838ff 404040ff 404040ff 404040ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 505050ff 404040ff 101010ff 202020ff 404040ff 707070ff 808080ff 101010ff 707070ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 000000ff 606060ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
+ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 505050ff 404040ff 404040ff 404040ff 404040ff 606060ff 707070ff 101010ff 808080ff 808080ff 808080ff 606060ff 404040ff 404040ff 404040ff 404040ff 404040ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 505050ff 404040ff 404040ff 404040ff 404040ff 707070ff 686868ff 181818ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 404040ff 707070ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 585858ff 484848ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 505050ff 505050ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff dfdfdfff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff 808080ff dfdfdfff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff 
 ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff ffffffff
```

### Comparing `nelsie-0.5.0/tests/checks/text_align/0-1.png` & `nelsie-0.6.0/tests/checks/text_align/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/text_anchor_points/0-1.png` & `nelsie-0.6.0/tests/checks/text_anchor_points/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/text_anchor_points/1-1.png` & `nelsie-0.6.0/tests/checks/text_anchor_points/1-1-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/text_anchor_points/2-1.png` & `nelsie-0.6.0/tests/checks/text_anchor_points/2-2-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/text_anchors_space_prefix/0-1.png` & `nelsie-0.6.0/tests/checks/text_anchors_space_prefix/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/text_anchors_styled_space_prefix/0-1.png` & `nelsie-0.6.0/tests/checks/text_anchors_styled_space_prefix/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/text_boxes/0-1.png` & `nelsie-0.6.0/tests/checks/text_boxes/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/text_color_opacity/0-1.png` & `nelsie-0.6.0/tests/checks/text_color_opacity/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/text_descent_ascent1/0-1.png` & `nelsie-0.6.0/tests/checks/text_descent_ascent1/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/text_descent_ascent2/0-1.png` & `nelsie-0.6.0/tests/checks/text_descent_ascent2/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/text_in_steps/0-1.png` & `nelsie-0.6.0/tests/checks/text_in_steps/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/text_in_steps/0-2.png` & `nelsie-0.6.0/tests/checks/text_in_steps/1-0-2.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/text_in_steps/0-3.png` & `nelsie-0.6.0/tests/checks/text_in_steps/2-0-3.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/text_kerning/0-1.png` & `nelsie-0.6.0/tests/checks/text_kerning/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/text_line_points1/0-1.png` & `nelsie-0.6.0/tests/checks/text_line_points1/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/text_line_points2/0-1.png` & `nelsie-0.6.0/tests/checks/text_line_points2/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/text_monospace/0-1.png` & `nelsie-0.6.0/tests/checks/text_monospace/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/text_stroke/0-1.png` & `nelsie-0.6.0/tests/checks/text_stroke/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/text_styling/0-1.png` & `nelsie-0.6.0/tests/checks/text_styling/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/checks/z_level/0-1.png` & `nelsie-0.6.0/tests/checks/z_level/0-0-1.png`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/conftest.py` & `nelsie-0.6.0/tests/conftest.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,23 +10,27 @@
 ASSETS_DIR = os.path.join(PYTEST_DIR, "assets")
 
 sys.path.insert(0, os.path.join(ROOT_DIR, "nelsie-api"))
 
 from nelsie import Resources, SlideDeck  # noqa
 
 
-@pytest.fixture(scope="session")
-def resources():
-    resources = Resources()
+def new_resources(**kwargs):
+    resources = Resources(**kwargs)
 
     # Let us fix the fonts, so we have the same results across all OSs
     resources.load_fonts_dir(os.path.join(ASSETS_DIR, "fonts"))
     return resources
 
 
+@pytest.fixture(scope="session")
+def resources():
+    return new_resources()
+
+
 @pytest.fixture()
 def deck_builder(resources):
     def helper(**kwargs):
         kwargs.setdefault("image_directory", ASSETS_DIR)
         kwargs.setdefault("default_font", "DejaVu Sans")
         kwargs.setdefault("default_monospace_font", "DejaVu Sans Mono")
         kwargs.setdefault("resources", resources)
```

### Comparing `nelsie-0.5.0/tests/test_code.py` & `nelsie-0.6.0/tests/test_code.py`

 * *Files 12% similar despite different names*

```diff
@@ -93,15 +93,19 @@
 
 
 @check()
 def test_code_style_delimiters(deck):
     slide = deck.new_slide(width=300, height=50)
     slide.set_style("big", TextStyle(size=20, color="orange"))
     slide.code(
-        "print('$big<Hello> world!')", "Python", style=TextStyle(size=12), parse_styles=True, style_delimiters="$<>"
+        "print('$big<Hello> world!')",
+        "Python",
+        style=TextStyle(size=12),
+        parse_styles=True,
+        style_delimiters="$<>",
     )
 
 
 @check()
 def test_code_language_none(deck):
     slide = deck.new_slide(width=200, height=30)
     slide.code("print('Hello world!')", None, style=TextStyle(size=12))
```

### Comparing `nelsie-0.5.0/tests/test_complex.py` & `nelsie-0.6.0/tests/test_complex.py`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/test_error.py` & `nelsie-0.6.0/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/test_image.py` & `nelsie-0.6.0/tests/test_image.py`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/test_layout.py` & `nelsie-0.6.0/tests/test_layout.py`

 * *Files 2% similar despite different names*

```diff
@@ -194,27 +194,27 @@
     assert e._expr == ("sum", ("x", 123), 10)
     e2 = e - 20.0
     assert e2._expr == ("sum", ("x", 123), 10, -20.0)
 
 
 @check()
 def test_expr_x_y_weight_height(deck):
-    slide = deck.new_slide(200, 80)
+    slide = deck.new_slide(width=200, height=80)
     box = slide.box(width=180, height=40, bg_color="green")
     slide.box(
         x=box.x(0.33),
         y=box.y(),
         width=box.width(0.33),
         height=box.height(0.5),
         bg_color="blue",
     )
 
 
 @check(n_slides=2)
 def test_m_xy_p_xy(deck):
-    slide = deck.new_slide(100, 100)
+    slide = deck.new_slide(width=100, height=100)
     box = slide.box(bg_color="green")
     box.box(width=30, height=30, m_x=10, m_y=20, bg_color="red")
 
-    slide = deck.new_slide(100, 100)
+    slide = deck.new_slide(width=100, height=100)
     box = slide.box(bg_color="green", p_x=20, p_y=10)
     box.box(width=30, height=30, bg_color="red")
```

### Comparing `nelsie-0.5.0/tests/test_list.py` & `nelsie-0.6.0/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/test_others.py` & `nelsie-0.6.0/tests/test_others.py`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/test_paths.py` & `nelsie-0.6.0/tests/test_paths.py`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/test_slidedeck.py` & `nelsie-0.6.0/tests/test_slidedeck.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,39 +14,39 @@
     slide.box(width=None, height=None, bg_color="black")
 
     svg_data = deck.render(None, "svg")
     assert len(svg_data) == 2
 
     assert deck.render(out_svg, "svg") is None
 
-    with open(out_svg / "0-1.svg", "rb") as f:
+    with open(out_svg / "0-0-1.svg", "rb") as f:
         data = f.read()
         assert data.startswith(
             b"""<svg width="1024" height="768" viewBox="0 0 1024 768" xmlns="http://www.w3.org/2000/svg">"""
         )
         assert svg_data[0] == (0, 0, data)
 
-    with open(out_svg / "1-1.svg", "rb") as f:
+    with open(out_svg / "1-1-1.svg", "rb") as f:
         data = f.read()
         assert data.startswith(
             b"""<svg width="1024" height="768" viewBox="0 0 1024 768" xmlns="http://www.w3.org/2000/svg">"""
         )
         assert svg_data[1] == (1, 0, data)
 
     png_data = deck.render(None, "png")
     assert len(png_data) == 2
 
     deck.render(out_png, "png")
 
-    with open(out_png / "0-1.png", "rb") as f:
+    with open(out_png / "0-0-1.png", "rb") as f:
         data = f.read()
         assert data[:4] == b"\x89PNG"
         assert png_data[0] == (0, 0, data)
 
-    with open(out_png / "1-1.png", "rb") as f:
+    with open(out_png / "1-1-1.png", "rb") as f:
         data = f.read()
         assert data[:4] == b"\x89PNG"
         assert png_data[1] == (1, 0, data)
 
     deck.render(out_pdf, "pdf")
 
     with open(out_pdf, "rb") as f:
```

### Comparing `nelsie-0.5.0/tests/test_text.py` & `nelsie-0.6.0/tests/test_text.py`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/tests/testutils.py` & `nelsie-0.6.0/tests/testutils.py`

 * *Files identical despite different names*

### Comparing `nelsie-0.5.0/Cargo.lock` & `nelsie-0.6.0/Cargo.lock`

 * *Files 1% similar despite different names*

```diff
@@ -6,17 +6,17 @@
 name = "adler"
 version = "1.0.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f26201604c87b1e01bd3d98f8d5d9a8fcbb815e8cedb41ffccbeb4bf593a35fe"
 
 [[package]]
 name = "aho-corasick"
-version = "1.1.2"
+version = "1.1.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b2969dcb958b36655471fc61f7e416fa76033bdd4bfed0678d8fee1e2d07a1f0"
+checksum = "8e60d3430d3a69478ad0993f19238d2df97c507009a52b3c10addcd7f6bcb916"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "anstream"
 version = "0.6.13"
@@ -75,17 +75,17 @@
 name = "arrayvec"
 version = "0.7.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "96d30a06541fbafbc7f82ed10c06164cfbd2c401138f6addd8404629c4b16711"
 
 [[package]]
 name = "autocfg"
-version = "1.1.0"
+version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "d468802bab17cbc0cc575e9b053f41e72aa36bfa6b7f55e3529ffa43161b97fa"
+checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
 
 [[package]]
 name = "base64"
 version = "0.21.7"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9d297deb1925b89f2ccc13d7635fa0714f12c87adce1c75356b39ca9b7178567"
 
@@ -117,17 +117,17 @@
 name = "bitflags"
 version = "1.3.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "bef38d45163c2f1dde094a7dfd33ccf595c92905c8f8f4fdc18d06fb1037718a"
 
 [[package]]
 name = "bitflags"
-version = "2.4.2"
+version = "2.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ed570934406eb16438a4e976b1b4500774099c13b8cb96eec99f620f05090ddf"
+checksum = "cf4b9d6a944f767f8e5e0db018570623c85f3d925ac718db4e06d0187adb21c1"
 
 [[package]]
 name = "bytemuck"
 version = "1.15.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5d6d68c57235a3a081186990eca2867354726650f42f7516ca50c28d6281fd15"
 
@@ -366,17 +366,17 @@
 name = "imagesize"
 version = "0.12.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "029d73f573d8e8d63e6d5020011d3255b28c3ba85d6cf870a07184ed23de9284"
 
 [[package]]
 name = "indexmap"
-version = "2.2.5"
+version = "2.2.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7b0b929d511467233429c45a44ac1dcaa21ba0f5ba11e4879e6ed28ddb4f9df4"
+checksum = "168fb715dda47215e360912c096649d23d58bf392ac62f73919e831745e40f26"
 dependencies = [
  "equivalent",
  "hashbrown",
 ]
 
 [[package]]
 name = "indicatif"
@@ -389,17 +389,17 @@
  "number_prefix",
  "portable-atomic",
  "unicode-width",
 ]
 
 [[package]]
 name = "indoc"
-version = "2.0.4"
+version = "2.0.5"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "1e186cfbae8084e513daff4240b4797e342f988cecda4fb6c939150f96315fd8"
+checksum = "b248f5224d1d606005e02c97f5aa4e88eeb230488bcc03bc9ca4d7991399f2b5"
 
 [[package]]
 name = "instant"
 version = "0.1.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "7a5bbe824c507c5da5956355e86a746d82e0e1464f65d862cc5e71da70e94b2c"
 dependencies = [
@@ -413,17 +413,17 @@
 checksum = "ba291022dbbd398a455acf126c1e341954079855bc60dfdda641363bd6922569"
 dependencies = [
  "either",
 ]
 
 [[package]]
 name = "itoa"
-version = "1.0.10"
+version = "1.0.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b1a46d1a171d865aa5f83f92695765caa047a9b4cbae2cbf37dbd613a793fd4c"
+checksum = "49f1f14873335454500d59611f1cf4a4b0f786f9ac11f4312a78e4cf2566695b"
 
 [[package]]
 name = "jpeg-decoder"
 version = "0.3.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f5d4a7da358eff58addd2877a45865158f0d78c911d43a5784ceb7bbf52833b0"
 
@@ -446,20 +446,17 @@
 name = "libc"
 version = "0.2.153"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "9c198f91728a82281a64e1f4f9eeb25d82cb32a5de251c6bd1b5154d63a8e7bd"
 
 [[package]]
 name = "line-wrap"
-version = "0.1.1"
+version = "0.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "f30344350a2a51da54c1d53be93fade8a237e545dbcc4bdbe635413f2117cab9"
-dependencies = [
- "safemem",
-]
+checksum = "dd1bc4d24ad230d21fb898d1116b1801d7adfc449d42026475862ab48b11e70e"
 
 [[package]]
 name = "linked-hash-map"
 version = "0.5.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "0717cef1bc8b636c6e1c1bbdefc09e6322da8a9321966e8928ef80d20f7f770f"
 
@@ -477,32 +474,32 @@
 name = "log"
 version = "0.4.21"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "90ed8c1e510134f979dbc4f070f87d4313098b704861a105fe34231c70a3901c"
 
 [[package]]
 name = "memchr"
-version = "2.7.1"
+version = "2.7.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "523dc4f511e55ab87b694dc30d0f820d60906ef06413f93d4d7a1385599cc149"
+checksum = "6c8640c5d730cb13ebd907d8d04b52f55ac9a2eec55b440c8892f40d56c76c1d"
 
 [[package]]
 name = "memmap2"
 version = "0.9.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "fe751422e4a8caa417e13c3ea66452215d7d63e19e604f4980461212f3ae1322"
 dependencies = [
  "libc",
 ]
 
 [[package]]
 name = "memoffset"
-version = "0.9.0"
+version = "0.9.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "5a634b1c61a95585bd15607c6ab0c4e5b226e695ff2800ba0cdccddf208c406c"
+checksum = "488016bfae457b036d996092f6cb448677611ce4449e970ceaf42695203f218a"
 dependencies = [
  "autocfg",
 ]
 
 [[package]]
 name = "miniz_oxide"
 version = "0.7.2"
@@ -511,15 +508,15 @@
 dependencies = [
  "adler",
  "simd-adler32",
 ]
 
 [[package]]
 name = "nelsie"
-version = "0.5.0"
+version = "0.6.0"
 dependencies = [
  "env_logger",
  "imagesize",
  "indicatif",
  "itertools",
  "log",
  "pdf-writer",
@@ -600,17 +597,17 @@
 name = "pico-args"
 version = "0.5.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5be167a7af36ee22fe3115051bc51f6e6c7054c9348e28deb4f49bd6f705a315"
 
 [[package]]
 name = "plist"
-version = "1.6.0"
+version = "1.6.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e5699cc8a63d1aa2b1ee8e12b9ad70ac790d65788cd36101fa37f87ea46c4cef"
+checksum = "d9d34169e64b3c7a80c8621a48adaf44e0cf62c78a9b25dd9dd35f1881a17cf9"
 dependencies = [
  "base64",
  "indexmap",
  "line-wrap",
  "quick-xml",
  "serde",
  "time",
@@ -648,17 +645,17 @@
 checksum = "e835ff2298f5721608eb1a980ecaee1aef2c132bf95ecc026a11b7bf3c01c02e"
 dependencies = [
  "unicode-ident",
 ]
 
 [[package]]
 name = "pyo3"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "53bdbb96d49157e65d45cc287af5f32ffadd5f4761438b527b055fb0d4bb8233"
+checksum = "a7a8b1990bd018761768d5e608a13df8bd1ac5f678456e0f301bb93e5f3ea16b"
 dependencies = [
  "cfg-if",
  "indoc",
  "libc",
  "memoffset",
  "parking_lot",
  "portable-atomic",
@@ -666,49 +663,49 @@
  "pyo3-ffi",
  "pyo3-macros",
  "unindent",
 ]
 
 [[package]]
 name = "pyo3-build-config"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "deaa5745de3f5231ce10517a1f5dd97d53e5a2fd77aa6b5842292085831d48d7"
+checksum = "650dca34d463b6cdbdb02b1d71bfd6eb6b6816afc708faebb3bac1380ff4aef7"
 dependencies = [
  "once_cell",
  "target-lexicon",
 ]
 
 [[package]]
 name = "pyo3-ffi"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "62b42531d03e08d4ef1f6e85a2ed422eb678b8cd62b762e53891c05faf0d4afa"
+checksum = "09a7da8fc04a8a2084909b59f29e1b8474decac98b951d77b80b26dc45f046ad"
 dependencies = [
  "libc",
  "pyo3-build-config",
 ]
 
 [[package]]
 name = "pyo3-macros"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7305c720fa01b8055ec95e484a6eca7a83c841267f0dd5280f0c8b8551d2c158"
+checksum = "4b8a199fce11ebb28e3569387228836ea98110e43a804a530a9fd83ade36d513"
 dependencies = [
  "proc-macro2",
  "pyo3-macros-backend",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "pyo3-macros-backend"
-version = "0.20.3"
+version = "0.21.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7c7e9b68bb9c3149c5b0cade5d07f953d6d125eb4337723c4ccdb665f1f96185"
+checksum = "93fbbfd7eb553d10036513cb122b888dcd362a945a00b06c165f2ab480d4cc3b"
 dependencies = [
  "heck",
  "proc-macro2",
  "pyo3-build-config",
  "quote",
  "syn",
 ]
@@ -720,17 +717,17 @@
 checksum = "1004a344b30a54e2ee58d66a71b32d2db2feb0a31f9a2d302bf0536f15de2a33"
 dependencies = [
  "memchr",
 ]
 
 [[package]]
 name = "quote"
-version = "1.0.35"
+version = "1.0.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "291ec9ab5efd934aaf503a6466c5d5251535d108ee747472c3977cc5acc868ef"
+checksum = "0fa76aaf39101c457836aec0ce2316dbdc3ab723cdda1c6bd4e6ad4208acaca7"
 dependencies = [
  "proc-macro2",
 ]
 
 [[package]]
 name = "redox_syscall"
 version = "0.4.1"
@@ -738,17 +735,17 @@
 checksum = "4722d768eff46b75989dd134e5c353f0d6296e5aaa3132e776cbdb56be7731aa"
 dependencies = [
  "bitflags 1.3.2",
 ]
 
 [[package]]
 name = "regex"
-version = "1.10.3"
+version = "1.10.4"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b62dbe01f0b06f9d8dc7d49e05a0785f153b00b2c227856282f671e0318c9b15"
+checksum = "c117dbdfde9c8308975b6a18d71f3f385c89461f7b3fb054288ecf2a2058ba4c"
 dependencies = [
  "aho-corasick",
  "memchr",
  "regex-automata",
  "regex-syntax",
 ]
 
@@ -761,17 +758,17 @@
  "aho-corasick",
  "memchr",
  "regex-syntax",
 ]
 
 [[package]]
 name = "regex-syntax"
-version = "0.8.2"
+version = "0.8.3"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c08c74e62047bb2de4ff487b251e4a92e24f48745648451635cec7d591162d9f"
+checksum = "adad44e29e4c806119491a7f06f03de4d1af22c3a680dd47f1e6e179439d1f56"
 
 [[package]]
 name = "resvg"
 version = "0.38.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "5c34501046959e06470ba62a2dc7f31c15f94ac250d842a45f9e012f4ee40c1e"
 dependencies = [
@@ -803,15 +800,15 @@
 
 [[package]]
 name = "rustybuzz"
 version = "0.12.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f0ae5692c5beaad6a9e22830deeed7874eae8a4e3ba4076fb48e12c56856222c"
 dependencies = [
- "bitflags 2.4.2",
+ "bitflags 2.5.0",
  "bytemuck",
  "smallvec",
  "ttf-parser",
  "unicode-bidi-mirroring",
  "unicode-ccc",
  "unicode-properties",
  "unicode-script",
@@ -820,20 +817,14 @@
 [[package]]
 name = "ryu"
 version = "1.0.17"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e86697c916019a8588c99b5fac3cead74ec0b4b819707a682fd4d23fa0ce1ba1"
 
 [[package]]
-name = "safemem"
-version = "0.3.3"
-source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "ef703b7cb59335eae2eb93ceb664c0eb7ea6bf567079d843e09420219668e072"
-
-[[package]]
 name = "same-file"
 version = "1.0.6"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "93fc1dc3aaa9bfed95e02e6eadabb4baf7e3078b0bd1b4d7b6b0b68378900502"
 dependencies = [
  "winapi-util",
 ]
@@ -862,17 +853,17 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "serde_json"
-version = "1.0.114"
+version = "1.0.115"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c5f09b1bd632ef549eaa9f60a1f8de742bdbc698e6cee2095fc84dde5f549ae0"
+checksum = "12dc5c46daa8e9fdf4f5e71b6cf9a53f2487da0e86e55808e2d35539666497dd"
 dependencies = [
  "itoa",
  "ryu",
  "serde",
 ]
 
 [[package]]
@@ -903,17 +894,17 @@
 checksum = "dbff4acf519f630b3a3ddcfaea6c06b42174d9a44bc70c620e9ed1649d58b82a"
 dependencies = [
  "version_check",
 ]
 
 [[package]]
 name = "smallvec"
-version = "1.13.1"
+version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "e6ecd384b10a64542d77071bd64bd7b231f4ed5940fba55e98c3de13824cf3d7"
+checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
 name = "strict-num"
 version = "0.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "6637bab7722d379c8b41ba849228d680cc12d0a45ba1fa2b48f2a30577a06731"
 dependencies = [
@@ -943,17 +934,17 @@
 dependencies = [
  "kurbo",
  "siphasher",
 ]
 
 [[package]]
 name = "syn"
-version = "2.0.52"
+version = "2.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "b699d15b36d1f02c3e7c69f8ffef53de37aefae075d8488d4ba1a7788d574a07"
+checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
 dependencies = [
  "proc-macro2",
  "quote",
  "unicode-ident",
 ]
 
 [[package]]
@@ -976,17 +967,17 @@
  "thiserror",
  "walkdir",
  "yaml-rust",
 ]
 
 [[package]]
 name = "taffy"
-version = "0.4.0"
+version = "0.4.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "fddbee94e20bc4612dcb789953324236eebd4fc6a08c650ccbf7f615e59a0d6a"
+checksum = "b3f8d105ace27c48b9d214e18a2bce0504aa9a31fda1425d151c84e04c9bd8aa"
 dependencies = [
  "arrayvec",
  "grid",
  "num-traits",
  "serde",
  "slotmap",
 ]
@@ -1015,17 +1006,17 @@
  "proc-macro2",
  "quote",
  "syn",
 ]
 
 [[package]]
 name = "time"
-version = "0.3.34"
+version = "0.3.36"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "c8248b6521bb14bc45b4067159b9b6ad792e2d6d754d6c41fb50e29fefe38749"
+checksum = "5dfd88e563464686c916c7e46e623e520ddc6d79fa6641390f2e3fa86e83e885"
 dependencies = [
  "deranged",
  "itoa",
  "num-conv",
  "powerfmt",
  "serde",
  "time-core",
@@ -1036,17 +1027,17 @@
 name = "time-core"
 version = "0.1.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "ef927ca75afb808a4d64dd374f00a2adf8d0fcff8e7b184af886c3c87ec4a3f3"
 
 [[package]]
 name = "time-macros"
-version = "0.2.17"
+version = "0.2.18"
 source = "registry+https://github.com/rust-lang/crates.io-index"
-checksum = "7ba3a3ef41e6672a2f0f001392bb5dcd3ff0a9992d618ca761a11c3121547774"
+checksum = "3f252a68540fde3a3877aeea552b832b40ab9a69e318efd078774a01ddee1ccf"
 dependencies = [
  "num-conv",
  "time-core",
 ]
 
 [[package]]
 name = "tiny-skia"
```

### Comparing `nelsie-0.5.0/PKG-INFO` & `nelsie-0.6.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: nelsie
-Version: 0.5.0
+Version: 0.6.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE
 Author-email: Ada Böhm <ada@kreatrix.org>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown; charset=UTF-8; variant=GFM
```

