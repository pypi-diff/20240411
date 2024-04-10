# Comparing `tmp/antsi-0.1.3.tar.gz` & `tmp/antsi-0.2.0.tar.gz`

## Comparing `antsi-0.1.3.tar` & `antsi-0.2.0.tar`

### file list

```diff
@@ -1,93 +1,94 @@
--rw-r--r--   0        0        0      572 1970-01-01 00:00:00.000000 antsi-0.1.3/Cargo.toml
--rw-r--r--   0     1001      127       22 2024-04-10 08:05:28.000000 antsi-0.1.3/.github/FUNDING.yml
--rw-r--r--   0     1001      127     4791 2024-04-10 08:05:28.000000 antsi-0.1.3/.github/workflows/distribution.yml
--rw-r--r--   0     1001      127      917 2024-04-10 08:05:28.000000 antsi-0.1.3/.github/workflows/lint.yml
--rw-r--r--   0     1001      127      685 2024-04-10 08:05:28.000000 antsi-0.1.3/.github/workflows/test.yml
--rw-r--r--   0     1001      127     5774 2024-04-10 08:05:28.000000 antsi-0.1.3/.gitignore
--rw-r--r--   0     1001      127      228 2024-04-10 08:05:28.000000 antsi-0.1.3/.yamllint.yml
--rw-r--r--   0     1001      127     1121 2024-04-10 08:05:28.000000 antsi-0.1.3/LICENSE.md
--rw-r--r--   0     1001      127     7645 2024-04-10 08:05:28.000000 antsi-0.1.3/README.md
--rw-r--r--   0     1001      127      402 2024-04-10 08:05:28.000000 antsi-0.1.3/antsi/__init__.py
--rw-r--r--   0     1001      127      133 2024-04-10 08:05:28.000000 antsi-0.1.3/antsi/_antsi.pyi
--rw-r--r--   0     1001      127        0 2024-04-10 08:05:28.000000 antsi-0.1.3/antsi/py.typed
--rw-r--r--   0     1001      127     7061 2024-04-10 08:05:28.000000 antsi-0.1.3/pdm.lock
--rw-r--r--   0     1001      127      107 2024-04-10 08:05:28.000000 antsi-0.1.3/renovate.json
--rw-r--r--   0     1001      127     2180 2024-04-10 08:05:28.000000 antsi-0.1.3/src/ast/color.rs
--rw-r--r--   0     1001      127     2071 2024-04-10 08:05:28.000000 antsi-0.1.3/src/ast/decoration.rs
--rw-r--r--   0     1001      127      271 2024-04-10 08:05:28.000000 antsi-0.1.3/src/ast/mod.rs
--rw-r--r--   0     1001      127    19008 2024-04-10 08:05:28.000000 antsi-0.1.3/src/ast/style.rs
--rw-r--r--   0     1001      127    14726 2024-04-10 08:05:28.000000 antsi-0.1.3/src/ast/token.rs
--rw-r--r--   0     1001      127    19103 2024-04-10 08:05:28.000000 antsi-0.1.3/src/color.rs
--rw-r--r--   0     1001      127     4554 2024-04-10 08:05:28.000000 antsi-0.1.3/src/error.rs
--rw-r--r--   0     1001      127     5386 2024-04-10 08:05:28.000000 antsi-0.1.3/src/escape.rs
--rw-r--r--   0     1001      127    11434 2024-04-10 08:05:28.000000 antsi-0.1.3/src/lexer.rs
--rw-r--r--   0     1001      127     3834 2024-04-10 08:05:28.000000 antsi-0.1.3/src/lib.rs
--rw-r--r--   0     1001      127     2401 2024-04-10 08:05:28.000000 antsi-0.1.3/src/macros.rs
--rw-r--r--   0     1001      127     8025 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/content.rs
--rw-r--r--   0     1001      127     4439 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/markup.rs
--rw-r--r--   0     1001      127      279 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__background_no_content.snap
--rw-r--r--   0     1001      127      347 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__decoration_multiple_styles_no_content.snap
--rw-r--r--   0     1001      127      319 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__decoration_single_style_no_content.snap
--rw-r--r--   0     1001      127      347 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__escaped_character_content.snap
--rw-r--r--   0     1001      127      278 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__foreground_no_content.snap
--rw-r--r--   0     1001      127      348 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__lowercase_alphabetic_content.snap
--rw-r--r--   0     1001      127      348 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__mixed_alphabetic_content.snap
--rw-r--r--   0     1001      127      671 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__nested_token.snap
--rw-r--r--   0     1001      127      800 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_and_trailing_content.snap
--rw-r--r--   0     1001      127      735 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_content.snap
--rw-r--r--   0     1001      127      736 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_trailing_content.snap
--rw-r--r--   0     1001      127      348 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__numeric_content.snap
--rw-r--r--   0     1001      127      349 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__special_character_content.snap
--rw-r--r--   0     1001      127      348 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__uppercase_alphabetic_content.snap
--rw-r--r--   0     1001      127      394 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__empty_token.snap
--rw-r--r--   0     1001      127     2007 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__kitchen_sink.snap
--rw-r--r--   0     1001      127      907 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__nested_token.snap
--rw-r--r--   0     1001      127      497 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_background.snap
--rw-r--r--   0     1001      127      496 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_foreground.snap
--rw-r--r--   0     1001      127      627 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_and_trailing_content.snap
--rw-r--r--   0     1001      127      562 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_content.snap
--rw-r--r--   0     1001      127      589 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_decorations.snap
--rw-r--r--   0     1001      127      694 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_styles.snap
--rw-r--r--   0     1001      127      553 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_single_decoration.snap
--rw-r--r--   0     1001      127      563 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_trailing_content.snap
--rw-r--r--   0     1001      127    23178 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/style.rs
--rw-r--r--   0     1001      127    16007 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser/text.rs
--rw-r--r--   0     1001      127    12184 2024-04-10 08:05:28.000000 antsi-0.1.3/src/parser.rs
--rw-r--r--   0     1001      127      314 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__lexer__tests__background_style_specifier.snap
--rw-r--r--   0     1001      127      310 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__lexer__tests__foreground_style_specifier.snap
--rw-r--r--   0     1001      127     2823 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__lexer__tests__many_tokens.snap
--rw-r--r--   0     1001      127      490 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__lexer__tests__multiple_decoration_style_specifiers.snap
--rw-r--r--   0     1001      127      317 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__lexer__tests__single_decoration_style_specifier.snap
--rw-r--r--   0     1001      127      261 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__empty_token.snap
--rw-r--r--   0     1001      127     1567 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__kitchen_sink.snap
--rw-r--r--   0     1001      127      670 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__nested_token.snap
--rw-r--r--   0     1001      127      230 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_bad_escape_character@errors.snap
--rw-r--r--   0     1001      127      111 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_bad_escape_character@result.snap
--rw-r--r--   0     1001      127      242 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_bad_escape_character_in_token@errors.snap
--rw-r--r--   0     1001      127      355 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_bad_escape_character_in_token@result.snap
--rw-r--r--   0     1001      127      157 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_text.snap
--rw-r--r--   0     1001      127      231 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_plaintext@errors.snap
--rw-r--r--   0     1001      127      107 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_plaintext@result.snap
--rw-r--r--   0     1001      127      245 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_token@errors.snap
--rw-r--r--   0     1001      127      385 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_token@result.snap
--rw-r--r--   0     1001      127      235 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_plaintext@errors.snap
--rw-r--r--   0     1001      127      109 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_plaintext@result.snap
--rw-r--r--   0     1001      127      620 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_token@errors.snap
--rw-r--r--   0     1001      127      112 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_token@result.snap
--rw-r--r--   0     1001      127      230 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_plaintext@errors.snap
--rw-r--r--   0     1001      127      107 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_plaintext@result.snap
--rw-r--r--   0     1001      127      614 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_token@errors.snap
--rw-r--r--   0     1001      127      112 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_token@result.snap
--rw-r--r--   0     1001      127      502 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_open_square_bracket_in_plaintext.snap
--rw-r--r--   0     1001      127      685 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_open_square_bracket_in_token.snap
--rw-r--r--   0     1001      127      338 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__token_with_background.snap
--rw-r--r--   0     1001      127      336 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__token_with_foreground.snap
--rw-r--r--   0     1001      127      438 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__token_with_leading_and_trailing_content.snap
--rw-r--r--   0     1001      127      388 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__token_with_leading_content.snap
--rw-r--r--   0     1001      127      414 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__token_with_multiple_decorations.snap
--rw-r--r--   0     1001      127      502 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__token_with_multiple_styles.snap
--rw-r--r--   0     1001      127      379 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__token_with_single_decoration.snap
--rw-r--r--   0     1001      127      390 2024-04-10 08:05:28.000000 antsi-0.1.3/src/snapshots/antsi__parser__tests__token_with_trailing_content.snap
--rw-r--r--   0     1001      127    15182 2024-04-10 08:05:28.000000 antsi-0.1.3/Cargo.lock
--rw-r--r--   0     1001      127     1056 2024-04-10 08:05:28.000000 antsi-0.1.3/pyproject.toml
--rw-r--r--   0        0        0     8248 1970-01-01 00:00:00.000000 antsi-0.1.3/PKG-INFO
+-rw-r--r--   0        0        0      590 1970-01-01 00:00:00.000000 antsi-0.2.0/Cargo.toml
+-rw-r--r--   0     1001      127       22 2024-04-10 23:04:29.000000 antsi-0.2.0/.github/FUNDING.yml
+-rw-r--r--   0     1001      127     4875 2024-04-10 23:04:29.000000 antsi-0.2.0/.github/workflows/distribution.yml
+-rw-r--r--   0     1001      127      917 2024-04-10 23:04:29.000000 antsi-0.2.0/.github/workflows/lint.yml
+-rw-r--r--   0     1001      127      685 2024-04-10 23:04:29.000000 antsi-0.2.0/.github/workflows/test.yml
+-rw-r--r--   0     1001      127     5774 2024-04-10 23:04:29.000000 antsi-0.2.0/.gitignore
+-rw-r--r--   0     1001      127      228 2024-04-10 23:04:29.000000 antsi-0.2.0/.yamllint.yml
+-rw-r--r--   0     1001      127     1121 2024-04-10 23:04:29.000000 antsi-0.2.0/LICENSE.md
+-rw-r--r--   0     1001      127     7995 2024-04-10 23:04:29.000000 antsi-0.2.0/README.md
+-rw-r--r--   0     1001      127      402 2024-04-10 23:04:29.000000 antsi-0.2.0/antsi/__init__.py
+-rw-r--r--   0     1001      127      158 2024-04-10 23:04:29.000000 antsi-0.2.0/antsi/_antsi.pyi
+-rw-r--r--   0     1001      127        0 2024-04-10 23:04:29.000000 antsi-0.2.0/antsi/py.typed
+-rw-r--r--   0     1001      127     7061 2024-04-10 23:04:29.000000 antsi-0.2.0/pdm.lock
+-rw-r--r--   0     1001      127      107 2024-04-10 23:04:29.000000 antsi-0.2.0/renovate.json
+-rw-r--r--   0     1001      127     2180 2024-04-10 23:04:29.000000 antsi-0.2.0/src/ast/color.rs
+-rw-r--r--   0     1001      127     2071 2024-04-10 23:04:29.000000 antsi-0.2.0/src/ast/decoration.rs
+-rw-r--r--   0     1001      127      271 2024-04-10 23:04:29.000000 antsi-0.2.0/src/ast/mod.rs
+-rw-r--r--   0     1001      127    19008 2024-04-10 23:04:29.000000 antsi-0.2.0/src/ast/style.rs
+-rw-r--r--   0     1001      127    14726 2024-04-10 23:04:29.000000 antsi-0.2.0/src/ast/token.rs
+-rw-r--r--   0     1001      127    19103 2024-04-10 23:04:29.000000 antsi-0.2.0/src/color.rs
+-rw-r--r--   0     1001      127     4554 2024-04-10 23:04:29.000000 antsi-0.2.0/src/error.rs
+-rw-r--r--   0     1001      127     5386 2024-04-10 23:04:29.000000 antsi-0.2.0/src/escape.rs
+-rw-r--r--   0     1001      127    11810 2024-04-10 23:04:29.000000 antsi-0.2.0/src/lexer.rs
+-rw-r--r--   0     1001      127     4329 2024-04-10 23:04:29.000000 antsi-0.2.0/src/lib.rs
+-rw-r--r--   0     1001      127     2401 2024-04-10 23:04:29.000000 antsi-0.2.0/src/macros.rs
+-rw-r--r--   0     1001      127     8025 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/content.rs
+-rw-r--r--   0     1001      127     4445 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/markup.rs
+-rw-r--r--   0     1001      127      279 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__background_no_content.snap
+-rw-r--r--   0     1001      127      347 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__decoration_multiple_styles_no_content.snap
+-rw-r--r--   0     1001      127      319 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__decoration_single_style_no_content.snap
+-rw-r--r--   0     1001      127      347 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__escaped_character_content.snap
+-rw-r--r--   0     1001      127      278 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__foreground_no_content.snap
+-rw-r--r--   0     1001      127      348 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__lowercase_alphabetic_content.snap
+-rw-r--r--   0     1001      127      348 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__mixed_alphabetic_content.snap
+-rw-r--r--   0     1001      127      671 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__nested_token.snap
+-rw-r--r--   0     1001      127      800 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_and_trailing_content.snap
+-rw-r--r--   0     1001      127      735 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_content.snap
+-rw-r--r--   0     1001      127      736 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_trailing_content.snap
+-rw-r--r--   0     1001      127      348 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__numeric_content.snap
+-rw-r--r--   0     1001      127      349 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__special_character_content.snap
+-rw-r--r--   0     1001      127      348 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__uppercase_alphabetic_content.snap
+-rw-r--r--   0     1001      127      394 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__empty_token.snap
+-rw-r--r--   0     1001      127     2007 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__kitchen_sink.snap
+-rw-r--r--   0     1001      127      907 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__nested_token.snap
+-rw-r--r--   0     1001      127      497 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_background.snap
+-rw-r--r--   0     1001      127      496 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_foreground.snap
+-rw-r--r--   0     1001      127      627 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_and_trailing_content.snap
+-rw-r--r--   0     1001      127      562 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_content.snap
+-rw-r--r--   0     1001      127      589 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_decorations.snap
+-rw-r--r--   0     1001      127      694 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_styles.snap
+-rw-r--r--   0     1001      127      553 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_single_decoration.snap
+-rw-r--r--   0     1001      127      563 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_trailing_content.snap
+-rw-r--r--   0     1001      127    28591 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/style.rs
+-rw-r--r--   0     1001      127    16007 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser/text.rs
+-rw-r--r--   0     1001      127    12470 2024-04-10 23:04:29.000000 antsi-0.2.0/src/parser.rs
+-rw-r--r--   0     1001      127      314 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__lexer__tests__background_style_specifier.snap
+-rw-r--r--   0     1001      127      310 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__lexer__tests__foreground_style_specifier.snap
+-rw-r--r--   0     1001      127     3257 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__lexer__tests__many_tokens.snap
+-rw-r--r--   0     1001      127      647 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__lexer__tests__mixed_whitespace_and_text.snap
+-rw-r--r--   0     1001      127      490 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__lexer__tests__multiple_decoration_style_specifiers.snap
+-rw-r--r--   0     1001      127      317 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__lexer__tests__single_decoration_style_specifier.snap
+-rw-r--r--   0     1001      127      261 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__empty_token.snap
+-rw-r--r--   0     1001      127     1567 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__kitchen_sink.snap
+-rw-r--r--   0     1001      127      670 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__nested_token.snap
+-rw-r--r--   0     1001      127      230 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_bad_escape_character@errors.snap
+-rw-r--r--   0     1001      127      111 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_bad_escape_character@result.snap
+-rw-r--r--   0     1001      127      242 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_bad_escape_character_in_token@errors.snap
+-rw-r--r--   0     1001      127      355 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_bad_escape_character_in_token@result.snap
+-rw-r--r--   0     1001      127      157 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_text.snap
+-rw-r--r--   0     1001      127      231 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_plaintext@errors.snap
+-rw-r--r--   0     1001      127      107 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_plaintext@result.snap
+-rw-r--r--   0     1001      127      245 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_token@errors.snap
+-rw-r--r--   0     1001      127      385 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_parenthesis_in_token@result.snap
+-rw-r--r--   0     1001      127      235 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_plaintext@errors.snap
+-rw-r--r--   0     1001      127      109 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_plaintext@result.snap
+-rw-r--r--   0     1001      127      620 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_token@errors.snap
+-rw-r--r--   0     1001      127      112 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_token@result.snap
+-rw-r--r--   0     1001      127      230 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_plaintext@errors.snap
+-rw-r--r--   0     1001      127      107 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_plaintext@result.snap
+-rw-r--r--   0     1001      127      614 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_token@errors.snap
+-rw-r--r--   0     1001      127      112 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_token@result.snap
+-rw-r--r--   0     1001      127      502 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_open_square_bracket_in_plaintext@errors.snap
+-rw-r--r--   0     1001      127      685 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_open_square_bracket_in_token@errors.snap
+-rw-r--r--   0     1001      127      338 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__token_with_background.snap
+-rw-r--r--   0     1001      127      336 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__token_with_foreground.snap
+-rw-r--r--   0     1001      127      438 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__token_with_leading_and_trailing_content.snap
+-rw-r--r--   0     1001      127      388 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__token_with_leading_content.snap
+-rw-r--r--   0     1001      127      414 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__token_with_multiple_decorations.snap
+-rw-r--r--   0     1001      127      502 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__token_with_multiple_styles.snap
+-rw-r--r--   0     1001      127      379 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__token_with_single_decoration.snap
+-rw-r--r--   0     1001      127      390 2024-04-10 23:04:29.000000 antsi-0.2.0/src/snapshots/antsi__parser__tests__token_with_trailing_content.snap
+-rw-r--r--   0     1001      127    15847 2024-04-10 23:04:29.000000 antsi-0.2.0/Cargo.lock
+-rw-r--r--   0     1001      127     1056 2024-04-10 23:04:29.000000 antsi-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     8598 1970-01-01 00:00:00.000000 antsi-0.2.0/PKG-INFO
```

### Comparing `antsi-0.1.3/Cargo.toml` & `antsi-0.2.0/Cargo.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [package]
 name = "antsi"
-version = "0.1.3"
+version = "0.2.0"
 edition = "2021"
 description = "A quick and user-friendly way to style your text using ANSI codes"
 
 # See more keys and their definitions at https://doc.rust-lang.org/cargo/reference/manifest.html
 [lib]
 name = "antsi"
 crate-type = ["cdylib"]
@@ -12,14 +12,15 @@
 [dependencies]
 codespan-reporting = "0.11"
 indexmap = "2.2"
 logos = "0.14"
 pyo3 = { version = "0.21", features = ["extension-module", "abi3-py310"] }
 termcolor = "1"
 text-size = "1.1"
+textwrap = "0.16"
 
 [dev-dependencies]
-insta = "1.36.1"
+insta = "1.38.0"
 
 [profile.dev.package]
 insta.opt-level = 3
 similar.opt-level = 3
```

### Comparing `antsi-0.1.3/.github/workflows/distribution.yml` & `antsi-0.2.0/.github/workflows/distribution.yml`

 * *Files 4% similar despite different names*

```diff
@@ -146,14 +146,15 @@
     name: Release
     runs-on: ubuntu-latest
     needs: [ publish ]
     permissions:
       contents: write
       id-token: write
     steps:
+      - uses: actions/checkout@v4
       - uses: actions/download-artifact@v4
         with:
           path: artifacts/
 
       - name: Relocate distribution files
         run: |
           mkdir ./dist
@@ -166,21 +167,23 @@
             ./dist/*.whl
 
       - name: Get version
         id: version
         run: |
           pipx install yq
           version=$(tomlq -r .package.version Cargo.toml)
-          echo "version=$version" >> "$GITHUB_OUTPUT"
+          echo "version=v$version" >> "$GITHUB_OUTPUT"
 
       - name: Create release
+        env:
+          GH_TOKEN: ${{ github.token }}
         run: >-
           gh release create
           ${{ steps.version.outputs.version }}
           --generate-notes --latest
-        env:
-          GITHUB_TOKEN: ${{ github.token }}
 
       - name: Upload assets
+        env:
+          GH_TOKEN: ${{ github.token }}
         run: >-
           gh release upload
           ${{ steps.version.outputs.version }} dist/**
```

### Comparing `antsi-0.1.3/.github/workflows/lint.yml` & `antsi-0.2.0/.github/workflows/lint.yml`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/.github/workflows/test.yml` & `antsi-0.2.0/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/.gitignore` & `antsi-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/LICENSE.md` & `antsi-0.2.0/LICENSE.md`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/README.md` & `antsi-0.2.0/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -43,35 +43,39 @@
 ```
 
 For example, `Hello [fg:green](there), user!` which will make only "there" be colored green. Everything else will be the
 default text color.
 
 ### Content
 
-The content following a style specifier must always be wrapped in parentheses and is whitespace sensitive. Any
-whitespace within the content will be emitted as-is unless [escaped](#escape-sequences) using a backslash
-(<code>&bsol;</code>).
+The content is what the style specifier applies to. It always immediately follows a style specifier and must be wrapped
+in parentheses. Any whitespace within the content will be emitted as-is unless [escaped](#escape-sequences) using a
+backslash (<code>&bsol;</code>).
 
 > [!IMPORTANT]
 >
-> Putting any character between the style specifier and content is explicitly disallowed.
+> Putting any character(s) between the style specifier and content is explicitly disallowed.
 
 The content can contain any characters, and it can even contain other styled markup! If you want to use any square
 brackets or parentheses in the content, they must be [escaped](#escape-sequences).
 
 > [!TIP]
 >
 > When nesting styled markup, the styles of the parent markup will also be applied unless explicitly overridden.
 > However, there is currently no way to remove text decorations from the children of nested markup.
 
 ### Style Specifiers
 
 Style specifiers are surrounded by square brackets (`[]`) and contain the directives for applying style to the content
 immediately following them. They are essentially a list of key-value pairs, where the key denotes the type of style.
 
+The styles within a specifier will ignore whitespace to facilitate readability. However, whitespace cannot exist in the
+middle of a key or value (i.e. `bl ue` will cause an error). The benefit of this is that `[ fg: red ; bg: blue ]`
+will be parsed the same as `[fg:red;bg:blue]`, so use whatever style you prefer.
+
 Examples:
 
 | Style Specifier                 | Meaning                                                    |
 |---------------------------------|------------------------------------------------------------|
 | `[fg:red]`                      | Red foreground                                             |
 | `[bg:blue]`                     | Blue background                                            |
 | `[deco:bold]`                   | Bold text                                                  |
@@ -169,9 +173,11 @@
 greatly appreciated!
 
 ## License
 
 Licensed under the [MIT license](LICENSE.md) (or <http://opensource.org/licenses/MIT>).
 
 [latest-release]: https://github.com/akrantz01/antsi/releases
+
 [pypi]: https://pypi.org/p/antsi
+
 [sponsorship]: https://github.com/sponsors/akrantz01
```

### Comparing `antsi-0.1.3/pdm.lock` & `antsi-0.2.0/pdm.lock`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/src/ast/color.rs` & `antsi-0.2.0/src/ast/color.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/src/ast/decoration.rs` & `antsi-0.2.0/src/ast/decoration.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/src/ast/style.rs` & `antsi-0.2.0/src/ast/style.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/src/ast/token.rs` & `antsi-0.2.0/src/ast/token.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/src/color.rs` & `antsi-0.2.0/src/color.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/src/error.rs` & `antsi-0.2.0/src/error.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/src/escape.rs` & `antsi-0.2.0/src/escape.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/src/lexer.rs` & `antsi-0.2.0/src/lexer.rs`

 * *Files 1% similar despite different names*

```diff
@@ -83,17 +83,20 @@
 
     #[regex(r#"\\[^ \r\n\t]"#)]
     EscapeCharacter,
 
     #[regex(r#"\\[ \r\n\t]+"#)]
     EscapeWhitespace,
 
+    #[regex(r#"[ \r\n\t]+"#, priority = 3)]
+    Whitespace,
+
     // as a temporary fix until https://github.com/maciejhirsz/logos/issues/265 is resolved, the
     // tokens `:` `;` and `,` are considered stop characters for words
-    #[regex(r#"[^\\\[\]():;,]+"#, priority = 2)]
+    #[regex(r#"[^\\\[\]() \r\n\t:;,]+"#, priority = 2)]
     Text,
 
     Unknown,
     Eof,
 }
 
 impl SyntaxKind {
@@ -110,14 +113,15 @@
             Self::ForegroundSpecifier => "foreground specifier",
             Self::BackgroundSpecifier => "background specifier",
             Self::DecorationSpecifier => "decoration specifier",
             Self::Color => "color",
             Self::Decoration => "decoration",
             Self::EscapeCharacter => "escape character",
             Self::EscapeWhitespace => "escape whitespace",
+            Self::Whitespace => "whitespace",
             Self::Text => "text",
             Self::Unknown => "unknown",
             Self::Eof => "end of file",
         }
     }
 }
 
@@ -142,14 +146,16 @@
     fn check(input: &str, kind: SyntaxKind) {
         let mut lexer = Lexer::new(input);
 
         let token = lexer.next().unwrap();
         assert_eq!(token.kind, kind);
         assert_eq!(token.text, input);
         assert_ne!(token.span.len(), TextSize::new(0));
+
+        assert!(lexer.next().is_none());
     }
 
     #[test]
     fn square_bracket_open() {
         check("[", SyntaxKind::SquareBracketOpen);
     }
 
@@ -180,20 +186,20 @@
 
     #[test]
     fn comma() {
         check(",", SyntaxKind::Comma);
     }
 
     #[test]
-    fn lowerascii_case_alphabetic_text() {
+    fn lower_ascii_case_alphabetic_text() {
         check("abcdefghijklmnopqrstuvwxyz", SyntaxKind::Text);
     }
 
     #[test]
-    fn upperascii_case_alphabetic_text() {
+    fn upper_ascii_case_alphabetic_text() {
         check("ABCDEFGHIJKLMNOPQRSTUVWXYZ", SyntaxKind::Text);
     }
 
     #[test]
     fn mixed_ascii_case_alphabetic_text() {
         check(
             "AaBbCcDdEeFfGgHhIiJjKkLlMmNnOoPpQqRrSsTtUuVvWwXxYyZz",
@@ -223,16 +229,16 @@
 
     #[test]
     fn decoration_specifier() {
         check("deco", SyntaxKind::DecorationSpecifier);
     }
 
     #[test]
-    fn whitespace_text() {
-        check("  \n\t", SyntaxKind::Text);
+    fn whitespace() {
+        check("  \n\t", SyntaxKind::Whitespace);
     }
 
     #[test]
     fn color_black() {
         check("black", SyntaxKind::Color);
     }
 
@@ -490,14 +496,21 @@
     #[test]
     fn multiple_decoration_style_specifiers() {
         let tokens = Lexer::new("deco:bold,italic").collect::<Vec<_>>();
         insta::assert_debug_snapshot!(tokens);
     }
 
     #[test]
+    fn mixed_whitespace_and_text() {
+        let tokens = Lexer::new(" a\n\tbcd5\r\n test ").collect::<Vec<_>>();
+        assert_eq!(tokens.len(), 7);
+        insta::assert_debug_snapshot!(tokens);
+    }
+
+    #[test]
     fn many_tokens() {
         let tokens = Lexer::new(
             "leading [fg:red](styled one) \\[middle\\) [bg:blue;deco:bold,italic](styled two) \\\n trailing",
         ).collect::<Vec<_>>();
         insta::assert_debug_snapshot!(tokens);
     }
 }
```

### Comparing `antsi-0.1.3/src/lib.rs` & `antsi-0.2.0/src/lib.rs`

 * *Files 8% similar despite different names*

```diff
@@ -1,8 +1,10 @@
+use pyo3::exceptions::PyTypeError;
 use pyo3::{create_exception, exceptions::PyException, prelude::*};
+use textwrap::Options;
 
 #[cfg(test)]
 #[macro_use]
 mod macros;
 mod ast;
 mod color;
 mod error;
@@ -33,14 +35,17 @@
 
 /// Convert styled markup to ANSI escape codes.
 ///
 /// Converts styled markup within the source text to ANSI escape codes allowing text to be formatted
 /// on the command line. If a string has no styled markup, it will be passed through unchanged. Any
 /// invalid/unparseable markup will cause an exception.
 ///
+/// Text wrapping is also supported when the `wrap` parameter is passed with the desired width. The
+/// wrap width must be greater than zero.
+///
 /// Styled markup is defined as follows:
 /// ```text
 /// [ <style specifiers> ]( <content> )
 ///
 /// <style specifiers> ::= <style specifier>;+
 ///  <style specifier> ::= <tag> : <value>
 ///          <content> ::= any character except \, [, ], (, )
@@ -95,17 +100,27 @@
 /// # Notes
 ///
 /// - If tags are repeated in a style specifier, the value of the last tag takes precedence
 /// - When nesting styled markup, styles of the parent will be applied unless overridden
 /// - There is currently no way to remove text decorations from the children of nested markup
 #[pyfunction]
 #[pyo3(name = "colorize")]
-#[pyo3(signature = (source, file="inline"))]
-fn py_colorize(source: &str, file: &str) -> PyResult<String> {
-    colorize(source).map_err(|errors| ColorizeError::from_report(errors.into(), source, file))
+#[pyo3(signature = (source, file="inline", wrap=None))]
+fn py_colorize(source: &str, file: &str, wrap: Option<usize>) -> PyResult<String> {
+    if let Some(0) = wrap {
+        return Err(PyTypeError::new_err("wrap width must be greater than 0"));
+    }
+
+    let styled = colorize(source)
+        .map_err(|errors| ColorizeError::from_report(errors.into(), source, file))?;
+
+    Ok(match wrap {
+        Some(width) => textwrap::fill(&styled, Options::new(width)),
+        None => styled,
+    })
 }
 
 /// Escape all styled markup in a piece of text
 #[pyfunction]
 #[pyo3(name = "escape")]
 fn py_escape(source: &str) -> String {
     escape(source)
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_g8u851a7_/tmp1hk4ny6m_TarContainer/0/23.rs", line 123, column 0: CDATA terminal not found*

```diff
@@ -1,13 +1,16 @@
-use pyo3::{create_exception, exceptions::PyException, prelude::*}; #[cfg(test)]
-#[macro_use] mod macros; mod ast; mod color; mod error; mod escape; mod lexer;
-mod parser; use color::colorize; use error::ErrorReport; use escape::escape;
-create_exception!( antsi, ColorizeError, PyException, "A report of all the
-issues found when applying styling to a piece of text" ); impl ColorizeError
-{ /// Create a new error from a report fn from_report(report: ErrorReport,
-source: &str, file: &str) -> PyErr { match report.emit(file, source, false)
-{ Ok(formatted) => Self::new_err(formatted), Err(e) => PyErr::from(e), } } } //
-/ Convert styled markup to ANSI escape codes. /// /// Converts styled markup
-within the source text to ANSI escape codes allowing text to be formatted //
-/ on the command line. If a string has no styled markup, it will be passed
-through unchanged. Any /// invalid/unparseable markup will cause an exception.
-/// /// Styled markup is defined as follows: /// ```text /// [
+use pyo3::exceptions::PyTypeError; use pyo3::{create_exception, exceptions::
+PyException, prelude::*}; use textwrap::Options; #[cfg(test)] #[macro_use] mod
+macros; mod ast; mod color; mod error; mod escape; mod lexer; mod parser; use
+color::colorize; use error::ErrorReport; use escape::escape; create_exception!
+( antsi, ColorizeError, PyException, "A report of all the issues found when
+applying styling to a piece of text" ); impl ColorizeError { /// Create a new
+error from a report fn from_report(report: ErrorReport, source: &str, file:
+&str) -> PyErr { match report.emit(file, source, false) { Ok(formatted) =>
+Self::new_err(formatted), Err(e) => PyErr::from(e), } } } /// Convert styled
+markup to ANSI escape codes. /// /// Converts styled markup within the source
+text to ANSI escape codes allowing text to be formatted /// on the command
+line. If a string has no styled markup, it will be passed through unchanged.
+Any /// invalid/unparseable markup will cause an exception. /// /// Text
+wrapping is also supported when the `wrap` parameter is passed with the desired
+width. The /// wrap width must be greater than zero. /// /// Styled markup is
+defined as follows: /// ```text /// [
```

### Comparing `antsi-0.1.3/src/macros.rs` & `antsi-0.2.0/src/macros.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/src/parser/content.rs` & `antsi-0.2.0/src/parser/content.rs`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/src/parser/markup.rs` & `antsi-0.2.0/src/parser/markup.rs`

 * *Files 0% similar despite different names*

```diff
@@ -151,13 +151,13 @@
     fn content_does_not_immediately_follow_style_specifiers() {
         let mut parser = Parser::new("[fg:red] (content)");
         assert_eq!(markup(&mut parser), None);
         assert_eq!(
             parser.errors,
             vec![Error {
                 span: Some(span!(8..9)),
-                at: SyntaxKind::Text,
+                at: SyntaxKind::Whitespace,
                 reason: Reason::Expected(vec![SyntaxKind::ParenthesisOpen])
             }]
         );
     }
 }
```

### Comparing `antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__nested_token.snap` & `antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__nested_token.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_and_trailing_content.snap` & `antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_and_trailing_content.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_content.snap` & `antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_leading_content.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_trailing_content.snap` & `antsi-0.2.0/src/parser/snapshots/antsi__parser__markup__tests__nested_token_with_trailing_content.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__kitchen_sink.snap` & `antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__kitchen_sink.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__nested_token.snap` & `antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__nested_token.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_and_trailing_content.snap` & `antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_and_trailing_content.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_content.snap` & `antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_leading_content.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_decorations.snap` & `antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_decorations.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_styles.snap` & `antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_multiple_styles.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_single_decoration.snap` & `antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_single_decoration.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/src/parser/snapshots/antsi__parser__text__tests__token_with_trailing_content.snap` & `antsi-0.2.0/src/parser/snapshots/antsi__parser__text__tests__token_with_trailing_content.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/src/parser/style.rs` & `antsi-0.2.0/src/parser/style.rs`

 * *Files 16% similar despite different names*

```diff
@@ -10,69 +10,86 @@
 pub(crate) fn style(p: &mut Parser) -> Option<Style> {
     p.expect(SyntaxKind::SquareBracketOpen)?;
 
     let mut style = Style::default();
     let mut first_specifier = true;
 
     loop {
+        p.consume_whitespace();
+
         if !first_specifier {
             if p.at(SyntaxKind::Semicolon) {
                 p.bump();
+                p.consume_whitespace();
             } else {
                 break;
             }
         }
 
-        if p.at(SyntaxKind::ForegroundSpecifier) {
-            let color = color_specifier(p, SyntaxKind::ForegroundSpecifier)?;
-            style.foreground = Some(color);
-        } else if p.at(SyntaxKind::BackgroundSpecifier) {
-            let color = color_specifier(p, SyntaxKind::BackgroundSpecifier)?;
-            style.background = Some(color);
-        } else if p.at(SyntaxKind::DecorationSpecifier) {
-            let decorations = decorations_specifier(p, SyntaxKind::DecorationSpecifier)?;
-            style.decoration = Some(decorations);
-        } else {
-            p.error(Reason::Expected(vec![
-                SyntaxKind::ForegroundSpecifier,
-                SyntaxKind::BackgroundSpecifier,
-                SyntaxKind::DecorationSpecifier,
-            ]));
-            return None;
-        };
+        match p.peek() {
+            Some(SyntaxKind::ForegroundSpecifier) => {
+                let color = color_specifier(p, SyntaxKind::ForegroundSpecifier)?;
+                style.foreground = Some(color);
+            }
+            Some(SyntaxKind::BackgroundSpecifier) => {
+                let color = color_specifier(p, SyntaxKind::BackgroundSpecifier)?;
+                style.background = Some(color);
+            }
+            Some(SyntaxKind::DecorationSpecifier) => {
+                let decorations = decorations_specifier(p, SyntaxKind::DecorationSpecifier)?;
+                style.decoration = Some(decorations);
+            }
+            _ => {
+                p.error(Reason::Expected(vec![
+                    SyntaxKind::ForegroundSpecifier,
+                    SyntaxKind::BackgroundSpecifier,
+                    SyntaxKind::DecorationSpecifier,
+                ]));
+                return None;
+            }
+        }
 
         first_specifier = false;
     }
 
     p.expect(SyntaxKind::SquareBracketClose)?;
 
     Some(style)
 }
 
 /// Parse a specifier with a [`Color`] value
 fn color_specifier(p: &mut Parser, tag: SyntaxKind) -> Option<Color> {
     p.expect(tag)?;
+    p.consume_whitespace();
+
     p.expect(SyntaxKind::Colon)?;
+    p.consume_whitespace();
 
     let token = p.expect(SyntaxKind::Color)?;
     Some(Color::from_str(token.text).expect("invalid color"))
 }
 
 /// Parse a specifier with a [`Decoration`]s value
 fn decorations_specifier(p: &mut Parser, tag: SyntaxKind) -> Option<IndexSet<Decoration>> {
     p.expect(tag)?;
+    p.consume_whitespace();
+
     p.expect(SyntaxKind::Colon)?;
+    p.consume_whitespace();
 
     let mut decorations = IndexSet::with_capacity(1);
     let mut first_decoration = true;
 
     loop {
+        p.consume_whitespace();
+
         if !first_decoration {
             if p.at(SyntaxKind::Comma) {
                 p.bump();
+                p.consume_whitespace();
             } else {
                 break;
             }
         }
 
         let token = p.expect(SyntaxKind::Decoration)?;
         decorations.insert(Decoration::from_str(token.text).expect("invalid decoration"));
@@ -190,14 +207,39 @@
                 at: SyntaxKind::Text,
                 reason: Reason::Expected(vec![SyntaxKind::Color])
             }]
         );
     }
 
     #[test]
+    fn color_specifier_whitespace_before_colon() {
+        let mut parser = Parser::new("fg :red");
+        let result = color_specifier(&mut parser, SyntaxKind::ForegroundSpecifier);
+        assert_eq!(result, Some(Color::Red));
+        assert!(parser.errors.is_empty());
+    }
+
+    #[test]
+    fn color_specifier_whitespace_after_colon() {
+        let mut parser = Parser::new("fg: red");
+        let result = color_specifier(&mut parser, SyntaxKind::ForegroundSpecifier);
+        assert_eq!(result, Some(Color::Red));
+        assert!(parser.errors.is_empty());
+    }
+
+    #[test]
+    fn color_specifier_trailing_whitespace() {
+        let mut parser = Parser::new("fg:red ");
+        let result = color_specifier(&mut parser, SyntaxKind::ForegroundSpecifier);
+        assert_eq!(result, Some(Color::Red));
+        assert!(parser.errors.is_empty());
+        assert!(parser.at(SyntaxKind::Whitespace));
+    }
+
+    #[test]
     fn decoration_specifier_single_decoration() {
         let mut parser = Parser::new("deco:bold");
         let result = decorations_specifier(&mut parser, SyntaxKind::DecorationSpecifier);
         assert_eq!(result, Some(set! { Decoration::Bold }));
     }
 
     #[test]
@@ -318,14 +360,54 @@
     fn decoration_specifier_stops_consuming_after_non_comma() {
         let mut parser = Parser::new("deco:bold;italic");
         let result = decorations_specifier(&mut parser, SyntaxKind::DecorationSpecifier);
         assert_eq!(result, Some(set! { Decoration::Bold }));
     }
 
     #[test]
+    fn decoration_specifier_whitespace_before_colon() {
+        let mut parser = Parser::new("deco :bold");
+        let result = decorations_specifier(&mut parser, SyntaxKind::DecorationSpecifier);
+        assert_eq!(result, Some(set! { Decoration::Bold }));
+        assert!(parser.errors.is_empty());
+    }
+
+    #[test]
+    fn decoration_specifier_whitespace_after_colon() {
+        let mut parser = Parser::new("deco: bold");
+        let result = decorations_specifier(&mut parser, SyntaxKind::DecorationSpecifier);
+        assert_eq!(result, Some(set! { Decoration::Bold }));
+        assert!(parser.errors.is_empty());
+    }
+
+    #[test]
+    fn decoration_specifier_trailing_whitespace() {
+        let mut parser = Parser::new("deco:bold ");
+        let result = decorations_specifier(&mut parser, SyntaxKind::DecorationSpecifier);
+        assert_eq!(result, Some(set! { Decoration::Bold }));
+        assert!(parser.errors.is_empty());
+    }
+
+    #[test]
+    fn decoration_specifier_whitespace_before_comma() {
+        let mut parser = Parser::new("deco:bold ,italic");
+        let result = decorations_specifier(&mut parser, SyntaxKind::DecorationSpecifier);
+        assert_eq!(result, Some(set! { Decoration::Bold, Decoration::Italic }));
+        assert!(parser.errors.is_empty());
+    }
+
+    #[test]
+    fn decoration_specifier_whitespace_after_comma() {
+        let mut parser = Parser::new("deco:bold, italic");
+        let result = decorations_specifier(&mut parser, SyntaxKind::DecorationSpecifier);
+        assert_eq!(result, Some(set! { Decoration::Bold, Decoration::Italic }));
+        assert!(parser.errors.is_empty());
+    }
+
+    #[test]
     fn style_foreground() {
         let mut parser = Parser::new("[fg:red]");
         let result = style(&mut parser);
         assert_eq!(result, Some(style!(fg: Red;)));
     }
 
     #[test]
@@ -681,8 +763,78 @@
                     SyntaxKind::ForegroundSpecifier,
                     SyntaxKind::BackgroundSpecifier,
                     SyntaxKind::DecorationSpecifier
                 ])
             }]
         )
     }
+
+    #[test]
+    fn style_whitespace_before_foreground_specifier() {
+        let mut parser = Parser::new("[ fg:red]");
+        assert_eq!(style(&mut parser), Some(style!(fg: Red;)));
+        assert!(parser.errors.is_empty());
+    }
+
+    #[test]
+    fn style_whitespace_before_background_specifier() {
+        let mut parser = Parser::new("[ bg:blue]");
+        assert_eq!(style(&mut parser), Some(style!(bg: Blue;)));
+        assert!(parser.errors.is_empty());
+    }
+
+    #[test]
+    fn style_whitespace_before_decoration_specifier_with_single() {
+        let mut parser = Parser::new("[ deco:bold]");
+        assert_eq!(style(&mut parser), Some(style!(deco: Bold;)));
+        assert!(parser.errors.is_empty());
+    }
+
+    #[test]
+    fn style_whitespace_before_decoration_specifier_with_multiple() {
+        let mut parser = Parser::new("[ deco:bold,italic]");
+        assert_eq!(style(&mut parser), Some(style!(deco: Bold, Italic;)));
+        assert!(parser.errors.is_empty());
+    }
+
+    #[test]
+    fn style_whitespace_after_foreground_specifier() {
+        let mut parser = Parser::new("[fg:red ]");
+        assert_eq!(style(&mut parser), Some(style!(fg: Red;)));
+        assert!(parser.errors.is_empty());
+    }
+
+    #[test]
+    fn style_whitespace_after_background_specifier() {
+        let mut parser = Parser::new("[bg:blue ]");
+        assert_eq!(style(&mut parser), Some(style!(bg: Blue;)));
+        assert!(parser.errors.is_empty());
+    }
+
+    #[test]
+    fn style_whitespace_after_decoration_specifier_with_single() {
+        let mut parser = Parser::new("[deco:bold ]");
+        assert_eq!(style(&mut parser), Some(style!(deco: Bold;)));
+        assert!(parser.errors.is_empty());
+    }
+
+    #[test]
+    fn style_whitespace_after_decoration_specifier_with_multiple() {
+        let mut parser = Parser::new("[deco:bold,italic ]");
+        assert_eq!(style(&mut parser), Some(style!(deco: Bold, Italic;)));
+        assert!(parser.errors.is_empty());
+    }
+
+    #[test]
+    fn style_whitespace_before_semicolon() {
+        let mut parser = Parser::new("[fg:red ;bg:blue]");
+        assert_eq!(style(&mut parser), Some(style!(fg: Red; bg: Blue;)));
+        assert!(parser.errors.is_empty());
+    }
+
+    #[test]
+    fn style_whitespace_after_semicolon() {
+        let mut parser = Parser::new("[fg:red; bg:blue]");
+        assert_eq!(style(&mut parser), Some(style!(fg: Red; bg: Blue;)));
+        assert!(parser.errors.is_empty());
+    }
 }
```

### Comparing `antsi-0.1.3/src/parser/text.rs` & `antsi-0.2.0/src/parser/text.rs`

 * *Files 0% similar despite different names*

```diff
@@ -390,15 +390,15 @@
     #[test]
     fn unescaped_open_square_bracket_in_plaintext() {
         let mut parser = Parser::new("before [ after");
         assert_eq!(text(&mut parser), None);
         assert_eq!(
             parser.errors,
             vec![Error {
-                span: Some(span!(8..14)),
+                span: Some(span!(9..14)),
                 at: SyntaxKind::Text,
                 reason: Reason::Expected(vec![
                     SyntaxKind::ForegroundSpecifier,
                     SyntaxKind::BackgroundSpecifier,
                     SyntaxKind::DecorationSpecifier,
                 ])
             }]
@@ -448,15 +448,15 @@
     #[test]
     fn unescaped_open_square_bracket_in_token() {
         let mut parser = Parser::new("[fg:red](before [ after)");
         assert_eq!(text(&mut parser), None);
         assert_eq!(
             parser.errors,
             vec![Error {
-                span: Some(span!(17..23)),
+                span: Some(span!(18..23)),
                 at: SyntaxKind::Text,
                 reason: Reason::Expected(vec![
                     SyntaxKind::ForegroundSpecifier,
                     SyntaxKind::BackgroundSpecifier,
                     SyntaxKind::DecorationSpecifier,
                 ])
             }]
```

### Comparing `antsi-0.1.3/src/parser.rs` & `antsi-0.2.0/src/parser.rs`

 * *Files 5% similar despite different names*

```diff
@@ -83,14 +83,21 @@
             Some(self.bump())
         } else {
             self.error(Reason::Expected(vec![kind]));
             None
         }
     }
 
+    /// Consume lexemes until a non-whitespace lexeme is reached
+    pub(crate) fn consume_whitespace(&mut self) {
+        while let Some(SyntaxKind::Whitespace) = self.peek() {
+            self.bump();
+        }
+    }
+
     /// Report an error during parsing
     pub(crate) fn error(&mut self, reason: Reason) {
         let (span, at) = match self.peek_lexeme() {
             Some(lexeme) => (Some(lexeme.span), lexeme.kind),
             None => (None, SyntaxKind::Eof),
         };
 
@@ -349,15 +356,15 @@
         });
     }
 
     #[test]
     fn parse_unescaped_open_square_bracket_in_plaintext() {
         with_source!("before [ after", |result, errors| {
             assert_eq!(result, vec![]);
-            assert_snapshot!(errors);
+            assert_snapshot!({ snapshot_suffix => "errors" }, errors);
         });
     }
 
     #[test]
     fn parse_unescaped_close_square_bracket_in_plaintext() {
         with_source!("before ] after", |result, errors| {
             assert_snapshot!({ snapshot_suffix => "result" }, result);
@@ -381,15 +388,15 @@
         });
     }
 
     #[test]
     fn parse_unescaped_open_square_bracket_in_token() {
         with_source!("[fg:red](before [ after)", |result, errors| {
             assert_eq!(result, vec![]);
-            assert_snapshot!(errors);
+            assert_snapshot!({ snapshot_suffix => "errors" }, errors);
         });
     }
 
     #[test]
     fn parse_unescaped_close_square_bracket_in_token() {
         with_source!("[fg:red](before ] after)", |result, errors| {
             assert_snapshot!({ snapshot_suffix => "result" }, result);
```

### Comparing `antsi-0.1.3/src/snapshots/antsi__lexer__tests__many_tokens.snap` & `antsi-0.2.0/src/snapshots/antsi__lexer__tests__many_tokens.snap`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,21 @@
 ---
 source: src/lexer.rs
 expression: tokens
 ---
 [
     Lexeme {
         kind: Text,
-        text: "leading ",
-        span: 0..8,
+        text: "leading",
+        span: 0..7,
+    },
+    Lexeme {
+        kind: Whitespace,
+        text: " ",
+        span: 7..8,
     },
     Lexeme {
         kind: SquareBracketOpen,
         text: "[",
         span: 8..9,
     },
     Lexeme {
@@ -36,24 +41,34 @@
     Lexeme {
         kind: ParenthesisOpen,
         text: "(",
         span: 16..17,
     },
     Lexeme {
         kind: Text,
-        text: "styled one",
-        span: 17..27,
+        text: "styled",
+        span: 17..23,
+    },
+    Lexeme {
+        kind: Whitespace,
+        text: " ",
+        span: 23..24,
+    },
+    Lexeme {
+        kind: Text,
+        text: "one",
+        span: 24..27,
     },
     Lexeme {
         kind: ParenthesisClose,
         text: ")",
         span: 27..28,
     },
     Lexeme {
-        kind: Text,
+        kind: Whitespace,
         text: " ",
         span: 28..29,
     },
     Lexeme {
         kind: EscapeCharacter,
         text: "\\[",
         span: 29..31,
@@ -65,15 +80,15 @@
     },
     Lexeme {
         kind: EscapeCharacter,
         text: "\\)",
         span: 37..39,
     },
     Lexeme {
-        kind: Text,
+        kind: Whitespace,
         text: " ",
         span: 39..40,
     },
     Lexeme {
         kind: SquareBracketOpen,
         text: "[",
         span: 40..41,
@@ -131,24 +146,34 @@
     Lexeme {
         kind: ParenthesisOpen,
         text: "(",
         span: 66..67,
     },
     Lexeme {
         kind: Text,
-        text: "styled two",
-        span: 67..77,
+        text: "styled",
+        span: 67..73,
+    },
+    Lexeme {
+        kind: Whitespace,
+        text: " ",
+        span: 73..74,
+    },
+    Lexeme {
+        kind: Text,
+        text: "two",
+        span: 74..77,
     },
     Lexeme {
         kind: ParenthesisClose,
         text: ")",
         span: 77..78,
     },
     Lexeme {
-        kind: Text,
+        kind: Whitespace,
         text: " ",
         span: 78..79,
     },
     Lexeme {
         kind: EscapeWhitespace,
         text: "\\\n ",
         span: 79..82,
```

### Comparing `antsi-0.1.3/src/snapshots/antsi__parser__tests__kitchen_sink.snap` & `antsi-0.2.0/src/snapshots/antsi__parser__tests__kitchen_sink.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/src/snapshots/antsi__parser__tests__nested_token.snap` & `antsi-0.2.0/src/snapshots/antsi__parser__tests__nested_token.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_token@errors.snap` & `antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_close_square_bracket_in_token@errors.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_token@errors.snap` & `antsi-0.2.0/src/snapshots/antsi__parser__tests__parse_unescaped_open_parenthesis_in_token@errors.snap`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/Cargo.lock` & `antsi-0.2.0/Cargo.lock`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # This file is automatically @generated by Cargo.
 # It is not intended for manual editing.
 version = 3
 
 [[package]]
 name = "antsi"
-version = "0.1.3"
+version = "0.2.0"
 dependencies = [
  "codespan-reporting",
  "indexmap",
  "insta",
  "logos",
  "pyo3",
  "termcolor",
  "text-size",
+ "textwrap",
 ]
 
 [[package]]
 name = "autocfg"
 version = "1.2.0"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f1fdabc7756949593fe60f30ec81974b613357de856987752631dea1e3394c80"
@@ -335,14 +336,20 @@
 [[package]]
 name = "smallvec"
 version = "1.13.2"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3c5e1a9a646d36c3599cd173a41282daf47c44583ad367b8e6837255952e5c67"
 
 [[package]]
+name = "smawk"
+version = "0.3.2"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "b7c388c1b5e93756d0c740965c41e8822f866621d41acbdf6336a6a168f8840c"
+
+[[package]]
 name = "syn"
 version = "2.0.58"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "44cfb93f38070beee36b3fef7d4f5a16f27751d94b187b666a5cc5e9b0d30687"
 dependencies = [
  "proc-macro2",
  "quote",
@@ -367,20 +374,37 @@
 [[package]]
 name = "text-size"
 version = "1.1.1"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "f18aa187839b2bdb1ad2fa35ead8c4c2976b64e4363c386d45ac0f7ee85c9233"
 
 [[package]]
+name = "textwrap"
+version = "0.16.1"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "23d434d3f8967a09480fb04132ebe0a3e088c173e6d0ee7897abbdf4eab0f8b9"
+dependencies = [
+ "smawk",
+ "unicode-linebreak",
+ "unicode-width",
+]
+
+[[package]]
 name = "unicode-ident"
 version = "1.0.12"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "3354b9ac3fae1ff6755cb6db53683adb661634f67557942dea4facebec0fee4b"
 
 [[package]]
+name = "unicode-linebreak"
+version = "0.1.5"
+source = "registry+https://github.com/rust-lang/crates.io-index"
+checksum = "3b09c83c3c29d37506a3e260c08c03743a6bb66a9cd432c6934ab501a190571f"
+
+[[package]]
 name = "unicode-width"
 version = "0.1.11"
 source = "registry+https://github.com/rust-lang/crates.io-index"
 checksum = "e51733f11c9c4f72aa0c160008246859e340b00807569a0da0e7a1079b27ba85"
 
 [[package]]
 name = "unindent"
```

### Comparing `antsi-0.1.3/pyproject.toml` & `antsi-0.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `antsi-0.1.3/PKG-INFO` & `antsi-0.2.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.3
 Name: antsi
-Version: 0.1.3
+Version: 0.2.0
 Classifier: Programming Language :: Rust
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE.md
 Summary: A quick and user-friendly way to style your text using ANSI codes
 Author-email: Alex Krantz <alex@krantz.dev>
 License: MIT
@@ -58,35 +58,39 @@
 ```
 
 For example, `Hello [fg:green](there), user!` which will make only "there" be colored green. Everything else will be the
 default text color.
 
 ### Content
 
-The content following a style specifier must always be wrapped in parentheses and is whitespace sensitive. Any
-whitespace within the content will be emitted as-is unless [escaped](#escape-sequences) using a backslash
-(<code>&bsol;</code>).
+The content is what the style specifier applies to. It always immediately follows a style specifier and must be wrapped
+in parentheses. Any whitespace within the content will be emitted as-is unless [escaped](#escape-sequences) using a
+backslash (<code>&bsol;</code>).
 
 > [!IMPORTANT]
 >
-> Putting any character between the style specifier and content is explicitly disallowed.
+> Putting any character(s) between the style specifier and content is explicitly disallowed.
 
 The content can contain any characters, and it can even contain other styled markup! If you want to use any square
 brackets or parentheses in the content, they must be [escaped](#escape-sequences).
 
 > [!TIP]
 >
 > When nesting styled markup, the styles of the parent markup will also be applied unless explicitly overridden.
 > However, there is currently no way to remove text decorations from the children of nested markup.
 
 ### Style Specifiers
 
 Style specifiers are surrounded by square brackets (`[]`) and contain the directives for applying style to the content
 immediately following them. They are essentially a list of key-value pairs, where the key denotes the type of style.
 
+The styles within a specifier will ignore whitespace to facilitate readability. However, whitespace cannot exist in the
+middle of a key or value (i.e. `bl ue` will cause an error). The benefit of this is that `[ fg: red ; bg: blue ]`
+will be parsed the same as `[fg:red;bg:blue]`, so use whatever style you prefer.
+
 Examples:
 
 | Style Specifier                 | Meaning                                                    |
 |---------------------------------|------------------------------------------------------------|
 | `[fg:red]`                      | Red foreground                                             |
 | `[bg:blue]`                     | Blue background                                            |
 | `[deco:bold]`                   | Bold text                                                  |
@@ -184,10 +188,12 @@
 greatly appreciated!
 
 ## License
 
 Licensed under the [MIT license](LICENSE.md) (or <http://opensource.org/licenses/MIT>).
 
 [latest-release]: https://github.com/akrantz01/antsi/releases
+
 [pypi]: https://pypi.org/p/antsi
+
 [sponsorship]: https://github.com/sponsors/akrantz01
```

#### html2text {}

 * *error from `html2text {}`:*

 * *File "/tmp/diffoscope_g8u851a7_/tmp1hk4ny6m_TarContainer/0/92", line 194, column 0: CDATA terminal not found*

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.3 Name: antsi Version: 0.1.3 Classifier: Programming
+Metadata-Version: 2.3 Name: antsi Version: 0.2.0 Classifier: Programming
 Language :: Rust Classifier: Programming Language :: Python :: Implementation
 :: CPython Classifier: Programming Language :: Python :: Implementation :: PyPy
 License-File: LICENSE.md Summary: A quick and user-friendly way to style your
 text using ANSI codes Author-email: Alex Krantz
 krantz.dev> License: MIT Requires-Python: >=3.10 Description-Content-Type:
 text/markdown; charset=UTF-8; variant=GFM Project-URL: homepage, https://
 github.com/akrantz01/antsi Project-URL: issues, https://github.com/akrantz01/
```

