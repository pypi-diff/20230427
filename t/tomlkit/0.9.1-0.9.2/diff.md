# Comparing `tmp/tomlkit-0.9.1.tar.gz` & `tmp/tomlkit-0.9.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tomlkit-0.9.1.tar", max compression
+gzip compressed data, was "tomlkit-0.9.2.tar", max compression
```

## Comparing `tomlkit-0.9.1.tar` & `tomlkit-0.9.2.tar`

### file list

```diff
@@ -1,787 +1,787 @@
--rw-r--r--   0        0        0     1062 2022-02-07 08:21:06.829023 tomlkit-0.9.1/LICENSE
--rw-r--r--   0        0        0     1962 2022-02-07 08:21:06.829023 tomlkit-0.9.1/README.md
--rw-r--r--   0        0        0     1078 2022-02-07 08:21:06.829023 tomlkit-0.9.1/pyproject.toml
--rw-r--r--   0        0        0        0 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/__init__.py
--rw-r--r--   0        0        0     2957 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/conftest.py
--rw-r--r--   0        0        0      706 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/0.5.0.toml
--rw-r--r--   0        0        0      870 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/example.toml
--rw-r--r--   0        0        0      194 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/fruit.toml
--rw-r--r--   0        0        0     1405 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/hard.toml
--rw-r--r--   0        0        0       20 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/invalid/array_duplicate_comma.toml
--rw-r--r--   0        0        0       17 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/invalid/array_leading_comma.toml
--rw-r--r--   0        0        0       17 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/invalid/array_no_comma.toml
--rw-r--r--   0        0        0      141 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/invalid/array_with_invalid_chars.toml
--rw-r--r--   0        0        0       27 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/invalid/inline_table_duplicate_comma.toml
--rw-r--r--   0        0        0       21 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/invalid/inline_table_leading_comma.toml
--rw-r--r--   0        0        0       24 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/invalid/inline_table_no_comma.toml
--rw-r--r--   0        0        0       21 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/invalid/inline_table_trailing_comma.toml
--rw-r--r--   0        0        0       18 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/invalid/invalid_date.toml
--rw-r--r--   0        0        0       31 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/invalid/invalid_datetime.toml
--rw-r--r--   0        0        0       15 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/invalid/invalid_number.toml
--rw-r--r--   0        0        0       20 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/invalid/invalid_time.toml
--rw-r--r--   0        0        0      160 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/invalid/key_value_with_trailing_chars.toml
--rw-r--r--   0        0        0       24 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/invalid/newline_in_singleline_string.toml
--rw-r--r--   0        0        0       58 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/invalid/section_with_trailing_characters.toml
--rw-r--r--   0        0        0       38 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/invalid/string_slash_whitespace_char.toml
--rw-r--r--   0        0        0       29 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/invalid/trailing_comma.toml
--rw-r--r--   0        0        0      676 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/json/0.5.0.json
--rw-r--r--   0        0        0     3340 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/json/pyproject.json
--rw-r--r--   0        0        0      299 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/json/table_names.json
--rw-r--r--   0        0        0       53 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/newline_in_strings.toml
--rw-r--r--   0        0        0       26 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/preserve_quotes_in_string.toml
--rw-r--r--   0        0        0     1994 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/pyproject.toml
--rw-r--r--   0        0        0      100 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/sections_with_same_start.toml
--rw-r--r--   0        0        0       82 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/string_slash_whitespace_newline.toml
--rw-r--r--   0        0        0      143 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/table_names.toml
--rw-r--r--   0        0        0     1579 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/examples/test.toml
--rw-r--r--   0        0        0     9235 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/test_api.py
--rw-r--r--   0        0        0     3089 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/test_build.py
--rw-r--r--   0        0        0    13424 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/test_items.py
--rw-r--r--   0        0        0      962 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/test_parser.py
--rw-r--r--   0        0        0    16630 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/test_toml_document.py
--rw-r--r--   0        0        0     1638 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/test_toml_file.py
--rw-r--r--   0        0        0     3482 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/test_toml_spec_tests.py
--rw-r--r--   0        0        0     1571 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/test_toml_tests.py
--rw-r--r--   0        0        0     1402 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/test_utils.py
--rw-r--r--   0        0        0      437 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/test_write.py
--rw-r--r--   0        0        0       68 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/.gitattributes
--rw-r--r--   0        0        0      742 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/LICENSE
--rw-r--r--   0        0        0      638 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/README.md
--rw-r--r--   0        0        0       55 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/errors/array-of-tables-1.toml
--rw-r--r--   0        0        0      188 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/errors/array-of-tables-2.toml
--rw-r--r--   0        0        0       15 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/errors/bare-key-1.toml
--rw-r--r--   0        0        0       17 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/errors/bare-key-2.toml
--rw-r--r--   0        0        0        9 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/errors/bare-key-3.toml
--rw-r--r--   0        0        0       15 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/errors/comment-control-1.toml
--rw-r--r--   0        0        0       17 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/errors/comment-control-2.toml
--rw-r--r--   0        0        0       17 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/errors/comment-control-3.toml
--rw-r--r--   0        0        0       15 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/errors/comment-control-4.toml
--rw-r--r--   0        0        0       66 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/errors/inline-table-imutable-1.toml
--rw-r--r--   0        0        0       66 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/errors/inline-table-imutable-2.toml
--rw-r--r--   0        0        0       21 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/errors/inline-table-trailing-comma.toml
--rw-r--r--   0        0        0       11 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/errors/int-0-padded.toml
--rw-r--r--   0        0        0       12 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/errors/int-signed-bin.toml
--rw-r--r--   0        0        0       12 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/errors/int-signed-hex.toml
--rw-r--r--   0        0        0       12 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/errors/int-signed-oct.toml
--rw-r--r--   0        0        0       16 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/errors/key-value-pair-1.toml
--rw-r--r--   0        0        0       48 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/errors/key-value-pair-2.toml
--rw-r--r--   0        0        0      225 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/errors/multiple-dot-key.toml
--rw-r--r--   0        0        0       47 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/errors/multiple-key.toml
--rw-r--r--   0        0        0       27 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/errors/no-key-name.toml
--rw-r--r--   0        0        0       12 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/errors/string-basic-control-1.toml
--rw-r--r--   0        0        0       14 2022-02-07 08:21:06.829023 tomlkit-0.9.1/tests/toml-spec-tests/errors/string-basic-control-2.toml
--rw-r--r--   0        0        0       14 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/string-basic-control-3.toml
--rw-r--r--   0        0        0       12 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/string-basic-control-4.toml
--rw-r--r--   0        0        0       16 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/string-basic-multiline-control-1.toml
--rw-r--r--   0        0        0       16 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/string-basic-multiline-control-2.toml
--rw-r--r--   0        0        0       16 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/string-basic-multiline-control-3.toml
--rw-r--r--   0        0        0       16 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/string-basic-multiline-control-4.toml
--rw-r--r--   0        0        0       28 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/string-basic-multiline-invalid-backslash.toml
--rw-r--r--   0        0        0       21 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/string-basic-multiline-out-of-range-unicode-escape-1.toml
--rw-r--r--   0        0        0       21 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/string-basic-multiline-out-of-range-unicode-escape-2.toml
--rw-r--r--   0        0        0       50 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/string-basic-multiline-quotes.toml
--rw-r--r--   0        0        0       13 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/string-basic-multiline-unknown-escape.toml
--rw-r--r--   0        0        0       17 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/string-basic-out-of-range-unicode-escape-1.toml
--rw-r--r--   0        0        0       17 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/string-basic-out-of-range-unicode-escape-2.toml
--rw-r--r--   0        0        0        9 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/string-basic-unknown-escape.toml
--rw-r--r--   0        0        0       12 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/string-literal-control-1.toml
--rw-r--r--   0        0        0       12 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/string-literal-control-2.toml
--rw-r--r--   0        0        0       12 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/string-literal-control-3.toml
--rw-r--r--   0        0        0       12 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/string-literal-control-4.toml
--rw-r--r--   0        0        0       16 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/string-literal-multiline-control-1.toml
--rw-r--r--   0        0        0       16 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/string-literal-multiline-control-2.toml
--rw-r--r--   0        0        0       16 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/string-literal-multiline-control-3.toml
--rw-r--r--   0        0        0       16 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/string-literal-multiline-control-4.toml
--rw-r--r--   0        0        0       72 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/string-literal-multiline-quotes.toml
--rw-r--r--   0        0        0       67 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/table-1.toml
--rw-r--r--   0        0        0       81 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/table-2.toml
--rw-r--r--   0        0        0       79 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/table-3.toml
--rw-r--r--   0        0        0       85 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/table-4.toml
--rw-r--r--   0        0        0      242 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/table-invalid-1.toml
--rw-r--r--   0        0        0       55 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/table-invalid-2.toml
--rw-r--r--   0        0        0      265 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/table-invalid-3.toml
--rw-r--r--   0        0        0      262 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/errors/table-invalid-4.toml
--rw-r--r--   0        0        0    13018 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/values/qa-array-inline-1000.toml
--rw-r--r--   0        0        0    12014 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/values/qa-array-inline-1000.yaml
--rw-r--r--   0        0        0     2010 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/values/qa-array-inline-nested-1000.toml
--rw-r--r--   0        0        0     2011 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/values/qa-array-inline-nested-1000.yaml
--rw-r--r--   0        0        0    40015 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/values/qa-key-literal-40kb.toml
--rw-r--r--   0        0        0    40016 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/values/qa-key-literal-40kb.yaml
--rw-r--r--   0        0        0    40015 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/values/qa-key-string-40kb.toml
--rw-r--r--   0        0        0    40016 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/values/qa-key-string-40kb.yaml
--rw-r--r--   0        0        0    40013 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/values/qa-scalar-literal-40kb.toml
--rw-r--r--   0        0        0    41074 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/values/qa-scalar-literal-40kb.yaml
--rw-r--r--   0        0        0    40017 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/values/qa-scalar-literal-multiline-40kb.toml
--rw-r--r--   0        0        0    41155 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/values/qa-scalar-literal-multiline-40kb.yaml
--rw-r--r--   0        0        0    40013 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/values/qa-scalar-string-40kb.toml
--rw-r--r--   0        0        0    41074 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/values/qa-scalar-string-40kb.yaml
--rw-r--r--   0        0        0    40017 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/values/qa-scalar-string-multiline-40kb.toml
--rw-r--r--   0        0        0    41155 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/values/qa-scalar-string-multiline-40kb.yaml
--rw-r--r--   0        0        0    19913 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/values/qa-table-inline-1000.toml
--rw-r--r--   0        0        0    17911 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/values/qa-table-inline-1000.yaml
--rw-r--r--   0        0        0     8010 2022-02-07 08:21:06.833023 tomlkit-0.9.1/tests/toml-spec-tests/values/qa-table-inline-nested-1000.toml
--rw-r--r--   0        0        0  1006009 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/qa-table-inline-nested-1000.yaml
--rw-r--r--   0        0        0       23 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-array-1.toml
--rw-r--r--   0        0        0       22 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-array-1.yaml
--rw-r--r--   0        0        0       38 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-array-2.toml
--rw-r--r--   0        0        0       37 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-array-2.yaml
--rw-r--r--   0        0        0       46 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-array-3.toml
--rw-r--r--   0        0        0       45 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-array-3.yaml
--rw-r--r--   0        0        0       67 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-array-4.toml
--rw-r--r--   0        0        0       59 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-array-4.yaml
--rw-r--r--   0        0        0       51 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-array-5.toml
--rw-r--r--   0        0        0       50 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-array-5.yaml
--rw-r--r--   0        0        0       26 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-array-7.toml
--rw-r--r--   0        0        0       25 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-array-7.yaml
--rw-r--r--   0        0        0       39 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-array-8.toml
--rw-r--r--   0        0        0       38 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-array-8.yaml
--rw-r--r--   0        0        0       37 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-array-mixed-number-types.toml
--rw-r--r--   0        0        0       36 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-array-mixed-number-types.yaml
--rw-r--r--   0        0        0      138 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-array-more-mixed-types.toml
--rw-r--r--   0        0        0      135 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-array-more-mixed-types.yaml
--rw-r--r--   0        0        0      118 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-array-of-tables-1.toml
--rw-r--r--   0        0        0      105 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-array-of-tables-1.yaml
--rw-r--r--   0        0        0      252 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-array-of-tables-2.toml
--rw-r--r--   0        0        0      264 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-array-of-tables-2.yaml
--rw-r--r--   0        0        0      109 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-array-of-tables-3.toml
--rw-r--r--   0        0        0       97 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-array-of-tables-3.yaml
--rw-r--r--   0        0        0       13 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-boolean-1.toml
--rw-r--r--   0        0        0       12 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-boolean-1.yaml
--rw-r--r--   0        0        0       14 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-boolean-2.toml
--rw-r--r--   0        0        0       13 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-boolean-2.yaml
--rw-r--r--   0        0        0       46 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-case-sensitive.toml
--rw-r--r--   0        0        0       18 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-case-sensitive.yaml
--rw-r--r--   0        0        0      120 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-comment-mid-array.toml
--rw-r--r--   0        0        0      119 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-comment-mid-array.yaml
--rw-r--r--   0        0        0       36 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-comment-mid-string.toml
--rw-r--r--   0        0        0       35 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-comment-mid-string.yaml
--rw-r--r--   0        0        0      134 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-comment-tab.toml
--rw-r--r--   0        0        0       13 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-comment-tab.yaml
--rw-r--r--   0        0        0       85 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-comment.toml
--rw-r--r--   0        0        0       84 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-comment.yaml
--rw-r--r--   0        0        0       65 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-date-local-1.json
--rw-r--r--   0        0        0       17 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-date-local-1.toml
--rw-r--r--   0        0        0       28 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-date-time-1.toml
--rw-r--r--   0        0        0       27 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-date-time-1.yaml
--rw-r--r--   0        0        0       33 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-date-time-2.toml
--rw-r--r--   0        0        0       32 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-date-time-2.yaml
--rw-r--r--   0        0        0       40 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-date-time-3.toml
--rw-r--r--   0        0        0       39 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-date-time-3.yaml
--rw-r--r--   0        0        0       28 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-date-time-4.toml
--rw-r--r--   0        0        0       27 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-date-time-4.yaml
--rw-r--r--   0        0        0       32 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-date-time-5.toml
--rw-r--r--   0        0        0       31 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-date-time-5.yaml
--rw-r--r--   0        0        0       33 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-date-time-6.toml
--rw-r--r--   0        0        0       31 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-date-time-6.yaml
--rw-r--r--   0        0        0       89 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-date-time-local-1.json
--rw-r--r--   0        0        0       27 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-date-time-local-1.toml
--rw-r--r--   0        0        0       89 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-date-time-local-2.json
--rw-r--r--   0        0        0       34 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-date-time-local-2.toml
--rw-r--r--   0        0        0       92 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-dotted-keys-1.toml
--rw-r--r--   0        0        0       87 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-dotted-keys-1.yaml
--rw-r--r--   0        0        0       13 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-dotted-keys-2.toml
--rw-r--r--   0        0        0       11 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-dotted-keys-2.yaml
--rw-r--r--   0        0        0       14 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-dotted-keys-3.toml
--rw-r--r--   0        0        0       11 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-dotted-keys-3.yaml
--rw-r--r--   0        0        0       41 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-empty-key-name-1.toml
--rw-r--r--   0        0        0       12 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-empty-key-name-1.yaml
--rw-r--r--   0        0        0       41 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-empty-key-name-2.toml
--rw-r--r--   0        0        0       12 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-empty-key-name-2.yaml
--rw-r--r--   0        0        0      139 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-extend-dotted-object-1.toml
--rw-r--r--   0        0        0       45 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-extend-dotted-object-1.yaml
--rw-r--r--   0        0        0      156 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-extend-dotted-object-2.toml
--rw-r--r--   0        0        0      112 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-extend-dotted-object-2.yaml
--rw-r--r--   0        0        0      145 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-extend-dotted-object-3.toml
--rw-r--r--   0        0        0      112 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-extend-dotted-object-3.yaml
--rw-r--r--   0        0        0       12 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-1.toml
--rw-r--r--   0        0        0       10 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-1.yaml
--rw-r--r--   0        0        0       31 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-10.toml
--rw-r--r--   0        0        0       31 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-10.yaml
--rw-r--r--   0        0        0       31 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-11.toml
--rw-r--r--   0        0        0       31 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-11.yaml
--rw-r--r--   0        0        0       31 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-12.toml
--rw-r--r--   0        0        0       32 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-12.yaml
--rw-r--r--   0        0        0       66 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-13.toml
--rw-r--r--   0        0        0       66 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-13.yaml
--rw-r--r--   0        0        0       27 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-14.toml
--rw-r--r--   0        0        0       10 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-14.yaml
--rw-r--r--   0        0        0       63 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-15.toml
--rw-r--r--   0        0        0       10 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-15.yaml
--rw-r--r--   0        0        0       14 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-2.toml
--rw-r--r--   0        0        0       13 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-2.yaml
--rw-r--r--   0        0        0       13 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-3.toml
--rw-r--r--   0        0        0       12 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-3.yaml
--rw-r--r--   0        0        0       13 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-4.toml
--rw-r--r--   0        0        0       12 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-4.yaml
--rw-r--r--   0        0        0       12 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-5.toml
--rw-r--r--   0        0        0       10 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-5.yaml
--rw-r--r--   0        0        0       13 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-6.toml
--rw-r--r--   0        0        0       12 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-6.yaml
--rw-r--r--   0        0        0       17 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-7.toml
--rw-r--r--   0        0        0       16 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-7.yaml
--rw-r--r--   0        0        0       27 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-8.toml
--rw-r--r--   0        0        0       25 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-8.yaml
--rw-r--r--   0        0        0       12 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-9.toml
--rw-r--r--   0        0        0       11 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-float-9.yaml
--rw-r--r--   0        0        0       11 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-1.toml
--rw-r--r--   0        0        0        9 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-1.yaml
--rw-r--r--   0        0        0       10 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-2.toml
--rw-r--r--   0        0        0        9 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-2.yaml
--rw-r--r--   0        0        0        9 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-3.toml
--rw-r--r--   0        0        0        8 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-3.yaml
--rw-r--r--   0        0        0       10 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-3a.toml
--rw-r--r--   0        0        0        8 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-3a.yaml
--rw-r--r--   0        0        0       10 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-3b.toml
--rw-r--r--   0        0        0        8 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-3b.yaml
--rw-r--r--   0        0        0       11 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-4.toml
--rw-r--r--   0        0        0       10 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-4.yaml
--rw-r--r--   0        0        0       13 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-5.toml
--rw-r--r--   0        0        0       12 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-5.yaml
--rw-r--r--   0        0        0       17 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-6.toml
--rw-r--r--   0        0        0       16 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-6.yaml
--rw-r--r--   0        0        0       45 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-7.toml
--rw-r--r--   0        0        0       44 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-7.yaml
--rw-r--r--   0        0        0       18 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-bin1.toml
--rw-r--r--   0        0        0       10 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-bin1.yaml
--rw-r--r--   0        0        0       18 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-hex1.toml
--rw-r--r--   0        0        0       17 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-hex1.yaml
--rw-r--r--   0        0        0       18 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-hex2.toml
--rw-r--r--   0        0        0       17 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-hex2.yaml
--rw-r--r--   0        0        0       19 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-hex3.toml
--rw-r--r--   0        0        0       17 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-hex3.yaml
--rw-r--r--   0        0        0       67 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-max.json
--rw-r--r--   0        0        0       30 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-max.toml
--rw-r--r--   0        0        0       68 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-min.json
--rw-r--r--   0        0        0       31 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-min.toml
--rw-r--r--   0        0        0       18 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-oct1.toml
--rw-r--r--   0        0        0       13 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-oct1.yaml
--rw-r--r--   0        0        0       48 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-oct2.toml
--rw-r--r--   0        0        0       10 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-int-oct2.yaml
--rw-r--r--   0        0        0       14 2022-02-07 08:21:06.837023 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-key-value-pair-1.toml
--rw-r--r--   0        0        0       13 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-key-value-pair-1.yaml
--rw-r--r--   0        0        0       19 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-key-value-pair-2.toml
--rw-r--r--   0        0        0       18 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-key-value-pair-2.yaml
--rw-r--r--   0        0        0       19 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-key-value-pair-3.toml
--rw-r--r--   0        0        0       18 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-key-value-pair-3.yaml
--rw-r--r--   0        0        0       15 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-key-value-pair-4.toml
--rw-r--r--   0        0        0       16 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-key-value-pair-4.yaml
--rw-r--r--   0        0        0       13 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-key-value-pair-5.toml
--rw-r--r--   0        0        0       16 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-key-value-pair-5.yaml
--rw-r--r--   0        0        0        4 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-key-value-pair-6.toml
--rw-r--r--   0        0        0        6 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-key-value-pair-6.yaml
--rw-r--r--   0        0        0        4 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-key-value-pair-7.toml
--rw-r--r--   0        0        0        6 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-key-value-pair-7.yaml
--rw-r--r--   0        0        0       12 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-key-value-pair-8.toml
--rw-r--r--   0        0        0       14 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-key-value-pair-8.yaml
--rw-r--r--   0        0        0       15 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-key-value-pair-9.toml
--rw-r--r--   0        0        0       17 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-key-value-pair-9.yaml
--rw-r--r--   0        0        0       20 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-newline-1.toml
--rw-r--r--   0        0        0       18 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-newline-1.yaml
--rw-r--r--   0        0        0       22 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-newline-2.toml
--rw-r--r--   0        0        0       18 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-newline-2.yaml
--rw-r--r--   0        0        0       30 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-newline-3.toml
--rw-r--r--   0        0        0       27 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-newline-3.yaml
--rw-r--r--   0        0        0       19 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-quoted-basic-keys-1.toml
--rw-r--r--   0        0        0       18 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-quoted-basic-keys-1.yaml
--rw-r--r--   0        0        0       27 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-quoted-literal-keys-1.toml
--rw-r--r--   0        0        0       26 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-quoted-literal-keys-1.yaml
--rw-r--r--   0        0        0      545 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-readme-example.toml
--rw-r--r--   0        0        0      432 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-readme-example.yaml
--rw-r--r--   0        0        0       45 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-basic-multiline-1.toml
--rw-r--r--   0        0        0       40 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-basic-multiline-1.yaml
--rw-r--r--   0        0        0       70 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-basic-multiline-2.toml
--rw-r--r--   0        0        0       52 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-basic-multiline-2.yaml
--rw-r--r--   0        0        0       89 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-basic-multiline-3.toml
--rw-r--r--   0        0        0       52 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-basic-multiline-3.yaml
--rw-r--r--   0        0        0       22 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-basic-multiline-4.toml
--rw-r--r--   0        0        0       12 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-basic-multiline-4.yaml
--rw-r--r--   0        0        0       57 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-basic-multiline-5.toml
--rw-r--r--   0        0        0       44 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-basic-multiline-5.yaml
--rw-r--r--   0        0        0       62 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-basic-multiline-6.toml
--rw-r--r--   0        0        0       57 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-basic-multiline-6.yaml
--rw-r--r--   0        0        0       51 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-basic-multiline-7.toml
--rw-r--r--   0        0        0       45 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-basic-multiline-7.yaml
--rw-r--r--   0        0        0       69 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-basic-multiline-8.toml
--rw-r--r--   0        0        0       59 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-basic-multiline-8.yaml
--rw-r--r--   0        0        0       64 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-basic-multiline-9.toml
--rw-r--r--   0        0        0       59 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-basic-multiline-9.yaml
--rw-r--r--   0        0        0       26 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-basic-tab-multiline.toml
--rw-r--r--   0        0        0       22 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-basic-tab-multiline.yaml
--rw-r--r--   0        0        0       22 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-basic-tab.toml
--rw-r--r--   0        0        0       22 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-basic-tab.yaml
--rw-r--r--   0        0        0       75 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-basic.toml
--rw-r--r--   0        0        0       74 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-basic.yaml
--rw-r--r--   0        0        0        9 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-escape-1.toml
--rw-r--r--   0        0        0        8 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-escape-1.yaml
--rw-r--r--   0        0        0        9 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-escape-2.toml
--rw-r--r--   0        0        0        8 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-escape-2.yaml
--rw-r--r--   0        0        0        9 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-escape-3.toml
--rw-r--r--   0        0        0        8 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-escape-3.yaml
--rw-r--r--   0        0        0        9 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-escape-4.toml
--rw-r--r--   0        0        0        8 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-escape-4.yaml
--rw-r--r--   0        0        0        9 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-escape-5.toml
--rw-r--r--   0        0        0        8 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-escape-5.yaml
--rw-r--r--   0        0        0        9 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-escape-6.toml
--rw-r--r--   0        0        0        8 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-escape-6.yaml
--rw-r--r--   0        0        0        9 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-escape-7.toml
--rw-r--r--   0        0        0        8 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-escape-7.yaml
--rw-r--r--   0        0        0       13 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-escape-8.toml
--rw-r--r--   0        0        0       10 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-escape-8.yaml
--rw-r--r--   0        0        0       17 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-escape-9.toml
--rw-r--r--   0        0        0       10 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-escape-9.yaml
--rw-r--r--   0        0        0       39 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-literal-1.toml
--rw-r--r--   0        0        0       37 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-literal-1.yaml
--rw-r--r--   0        0        0       40 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-literal-2.toml
--rw-r--r--   0        0        0       39 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-literal-2.yaml
--rw-r--r--   0        0        0       39 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-literal-3.toml
--rw-r--r--   0        0        0       36 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-literal-3.yaml
--rw-r--r--   0        0        0       24 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-literal-4.toml
--rw-r--r--   0        0        0       20 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-literal-4.yaml
--rw-r--r--   0        0        0       44 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-literal-multiline-1.toml
--rw-r--r--   0        0        0       40 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-literal-multiline-1.yaml
--rw-r--r--   0        0        0      103 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-literal-multiline-2.toml
--rw-r--r--   0        0        0      100 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-literal-multiline-2.yaml
--rw-r--r--   0        0        0       65 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-literal-multiline-3.toml
--rw-r--r--   0        0        0       60 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-literal-multiline-3.yaml
--rw-r--r--   0        0        0       52 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-literal-multiline-4.toml
--rw-r--r--   0        0        0       47 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-string-literal-multiline-4.yaml
--rw-r--r--   0        0        0       88 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-table-1.toml
--rw-r--r--   0        0        0       89 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-table-1.yaml
--rw-r--r--   0        0        0       36 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-table-2.toml
--rw-r--r--   0        0        0       48 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-table-2.yaml
--rw-r--r--   0        0        0        8 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-table-3.toml
--rw-r--r--   0        0        0       18 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-table-3.yaml
--rw-r--r--   0        0        0       37 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-table-4.toml
--rw-r--r--   0        0        0       18 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-table-4.yaml
--rw-r--r--   0        0        0       37 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-table-5.toml
--rw-r--r--   0        0        0       18 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-table-5.yaml
--rw-r--r--   0        0        0       43 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-table-6.toml
--rw-r--r--   0        0        0       21 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-table-6.yaml
--rw-r--r--   0        0        0      120 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-table-7.toml
--rw-r--r--   0        0        0       27 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-table-7.yaml
--rw-r--r--   0        0        0      116 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-table-8.toml
--rw-r--r--   0        0        0       94 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-table-8.yaml
--rw-r--r--   0        0        0       50 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-table-inline-1.toml
--rw-r--r--   0        0        0       47 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-table-inline-1.yaml
--rw-r--r--   0        0        0       25 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-table-inline-2.toml
--rw-r--r--   0        0        0       25 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-table-inline-2.yaml
--rw-r--r--   0        0        0       32 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-table-inline-3.toml
--rw-r--r--   0        0        0       37 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-table-inline-3.yaml
--rw-r--r--   0        0        0        8 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-table.toml
--rw-r--r--   0        0        0       10 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-table.yaml
--rw-r--r--   0        0        0       67 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-time-1.json
--rw-r--r--   0        0        0       15 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-time-1.toml
--rw-r--r--   0        0        0       67 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-time-2.json
--rw-r--r--   0        0        0       22 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tests/toml-spec-tests/values/spec-time-2.toml
--rw-r--r--   0        0        0       43 2022-02-07 08:21:07.197030 tomlkit-0.9.1/tests/toml-test/.git
--rw-r--r--   0        0        0      762 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/.github/workflows/test.yml
--rw-r--r--   0        0        0       17 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/.gitignore
--rw-r--r--   0        0        0       43 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/.gogo-release
--rw-r--r--   0        0        0     1079 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/COPYING
--rw-r--r--   0        0        0     9153 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/README.md
--rw-r--r--   0        0        0     4590 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/cmd/toml-test/main.go
--rw-r--r--   0        0        0     3458 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/cmd/toml-test/usage.go
--rwxr-xr-x   0        0        0      390 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/gen-multi.py
--rw-r--r--   0        0        0      204 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/go.mod
--rw-r--r--   0        0        0     1338 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/go.sum
--rw-r--r--   0        0        0     6697 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/json.go
--rw-r--r--   0        0        0     9646 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/runner.go
--rw-r--r--   0        0        0       14 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/.gitattributes
--rw-r--r--   0        0        0       18 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/array/missing-separator.toml
--rw-r--r--   0        0        0       10 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/array/no-close-2.toml
--rw-r--r--   0        0        0       18 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/array/no-close-table-2.toml
--rw-r--r--   0        0        0       16 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/array/no-close-table.toml
--rw-r--r--   0        0        0       23 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/array/no-close.toml
--rw-r--r--   0        0        0       55 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/array/tables-1.toml
--rw-r--r--   0        0        0      188 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/array/tables-2.toml
--rw-r--r--   0        0        0       70 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/array/text-after-array-entries.toml
--rw-r--r--   0        0        0       71 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/array/text-before-array-separator.toml
--rw-r--r--   0        0        0       56 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/array/text-in-array.toml
--rw-r--r--   0        0        0       14 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/bool/mixed-case.toml
--rw-r--r--   0        0        0       10 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/bool/wrong-case-false.toml
--rw-r--r--   0        0        0        9 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/bool/wrong-case-true.toml
--rw-r--r--   0        0        0       25 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/control/comment-del.toml
--rw-r--r--   0        0        0       26 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/control/comment-lf.toml
--rw-r--r--   0        0        0       26 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/control/comment-null.toml
--rw-r--r--   0        0        0       26 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/control/comment-us.toml
--rw-r--r--   0        0        0      568 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/control/control.multi
--rw-r--r--   0        0        0       24 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/control/multi-del.toml
--rw-r--r--   0        0        0       23 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/control/multi-lf.toml
--rw-r--r--   0        0        0       25 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/control/multi-null.toml
--rw-r--r--   0        0        0       23 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/control/multi-us.toml
--rw-r--r--   0        0        0       27 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/control/rawmulti-del.toml
--rw-r--r--   0        0        0       26 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/control/rawmulti-lf.toml
--rw-r--r--   0        0        0       28 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/control/rawmulti-null.toml
--rw-r--r--   0        0        0       26 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/control/rawmulti-us.toml
--rw-r--r--   0        0        0       24 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/control/rawstring-del.toml
--rw-r--r--   0        0        0       23 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/control/rawstring-lf.toml
--rw-r--r--   0        0        0       25 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/control/rawstring-null.toml
--rw-r--r--   0        0        0       23 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/control/rawstring-us.toml
--rw-r--r--   0        0        0       25 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/control/string-bs.toml
--rw-r--r--   0        0        0       21 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/control/string-del.toml
--rw-r--r--   0        0        0       20 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/control/string-lf.toml
--rw-r--r--   0        0        0       22 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/control/string-null.toml
--rw-r--r--   0        0        0       20 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/control/string-us.toml
--rw-r--r--   0        0        0       25 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/datetime/impossible-date.toml
--rw-r--r--   0        0        0       36 2022-02-07 08:21:07.757160 tomlkit-0.9.1/tests/toml-test/tests/invalid/datetime/no-leads-with-milli.toml
--rw-r--r--   0        0        0       31 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/datetime/no-leads.toml
--rw-r--r--   0        0        0       28 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/datetime/no-secs.toml
--rw-r--r--   0        0        0       27 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/datetime/no-t.toml
--rw-r--r--   0        0        0       16 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/datetime/trailing-t.toml
--rw-r--r--   0        0        0      242 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/encoding/bad-utf8-at-end.toml
--rw-r--r--   0        0        0        4 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/encoding/bad-utf8-in-comment.toml
--rw-r--r--   0        0        0       67 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/encoding/bad-utf8-in-string.toml
--rw-r--r--   0        0        0       20 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/encoding/bom-not-at-start-1.toml
--rw-r--r--   0        0        0       21 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/encoding/bom-not-at-start-2.toml
--rw-r--r--   0        0        0       38 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/encoding/utf16-bom.toml
--rw-r--r--   0        0        0       42 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/encoding/utf16.toml
--rw-r--r--   0        0        0       22 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/double-point-1.toml
--rw-r--r--   0        0        0       23 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/double-point-2.toml
--rw-r--r--   0        0        0       22 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/exp-double-e-1.toml
--rw-r--r--   0        0        0       23 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/exp-double-e-2.toml
--rw-r--r--   0        0        0       23 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/exp-double-us.toml
--rw-r--r--   0        0        0       23 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/exp-leading-us.toml
--rw-r--r--   0        0        0       20 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/exp-point-1.toml
--rw-r--r--   0        0        0       19 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/exp-point-2.toml
--rw-r--r--   0        0        0       25 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/exp-trailing-us.toml
--rw-r--r--   0        0        0      697 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/float.multi
--rw-r--r--   0        0        0       22 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/inf-incomplete-1.toml
--rw-r--r--   0        0        0       23 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/inf-incomplete-2.toml
--rw-r--r--   0        0        0       23 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/inf-incomplete-3.toml
--rw-r--r--   0        0        0       22 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/inf_underscore.toml
--rw-r--r--   0        0        0       28 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/leading-point-neg.toml
--rw-r--r--   0        0        0       29 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/leading-point-plus.toml
--rw-r--r--   0        0        0       23 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/leading-point.toml
--rw-r--r--   0        0        0       18 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/leading-us.toml
--rw-r--r--   0        0        0       26 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/leading-zero-neg.toml
--rw-r--r--   0        0        0       27 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/leading-zero-plus.toml
--rw-r--r--   0        0        0       21 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/leading-zero.toml
--rw-r--r--   0        0        0       22 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/nan-incomplete-1.toml
--rw-r--r--   0        0        0       23 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/nan-incomplete-2.toml
--rw-r--r--   0        0        0       23 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/nan-incomplete-3.toml
--rw-r--r--   0        0        0       22 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/nan_underscore.toml
--rw-r--r--   0        0        0       25 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/trailing-point-min.toml
--rw-r--r--   0        0        0       26 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/trailing-point-plus.toml
--rw-r--r--   0        0        0       20 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/trailing-point.toml
--rw-r--r--   0        0        0       19 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/trailing-us.toml
--rw-r--r--   0        0        0       22 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/us-after-point.toml
--rw-r--r--   0        0        0       23 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/float/us-before-point.toml
--rw-r--r--   0        0        0       15 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/inline-table/double-comma.toml
--rw-r--r--   0        0        0        8 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/inline-table/empty.toml
--rw-r--r--   0        0        0      111 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/inline-table/linebreak-1.toml
--rw-r--r--   0        0        0       15 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/inline-table/linebreak-2.toml
--rw-r--r--   0        0        0       15 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/inline-table/linebreak-3.toml
--rw-r--r--   0        0        0       75 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/inline-table/linebreak-4.toml
--rw-r--r--   0        0        0       18 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/inline-table/no-comma.toml
--rw-r--r--   0        0        0      140 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/inline-table/trailing-comma.toml
--rw-r--r--   0        0        0       18 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/capital-bin.toml
--rw-r--r--   0        0        0       18 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/capital-hex.toml
--rw-r--r--   0        0        0       18 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/capital-oct.toml
--rw-r--r--   0        0        0       23 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/double-sign-nex.toml
--rw-r--r--   0        0        0       24 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/double-sign-plus.toml
--rw-r--r--   0        0        0       18 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/double-us.toml
--rw-r--r--   0        0        0      652 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/integer.multi
--rw-r--r--   0        0        0       21 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/invalid-bin.toml
--rw-r--r--   0        0        0       21 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/invalid-hex.toml
--rw-r--r--   0        0        0       20 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/invalid-oct.toml
--rw-r--r--   0        0        0       22 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/leading-us-bin.toml
--rw-r--r--   0        0        0       22 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/leading-us-hex.toml
--rw-r--r--   0        0        0       22 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/leading-us-oct.toml
--rw-r--r--   0        0        0       18 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/leading-us.toml
--rw-r--r--   0        0        0       20 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/leading-zero-1.toml
--rw-r--r--   0        0        0       20 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/leading-zero-2.toml
--rw-r--r--   0        0        0       26 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/leading-zero-sign-1.toml
--rw-r--r--   0        0        0       26 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/leading-zero-sign-2.toml
--rw-r--r--   0        0        0       27 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/negative-bin.toml
--rw-r--r--   0        0        0       21 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/negative-hex.toml
--rw-r--r--   0        0        0       21 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/negative-oct.toml
--rw-r--r--   0        0        0       27 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/positive-bin.toml
--rw-r--r--   0        0        0       21 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/positive-hex.toml
--rw-r--r--   0        0        0       21 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/positive-oct.toml
--rw-r--r--   0        0        0       33 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/text-after-integer.toml
--rw-r--r--   0        0        0       23 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/trailing-us-bin.toml
--rw-r--r--   0        0        0       23 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/trailing-us-hex.toml
--rw-r--r--   0        0        0       23 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/trailing-us-oct.toml
--rw-r--r--   0        0        0       19 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/trailing-us.toml
--rw-r--r--   0        0        0       20 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/us-after-bin.toml
--rw-r--r--   0        0        0       20 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/us-after-hex.toml
--rw-r--r--   0        0        0       20 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/us-after-oct.toml
--rw-r--r--   0        0        0       32 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/key/after-array.toml
--rw-r--r--   0        0        0       36 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/key/after-table.toml
--rw-r--r--   0        0        0       48 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/key/after-value.toml
--rw-r--r--   0        0        0       15 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/key/bare-invalid-character.toml
--rw-r--r--   0        0        0       76 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/key/dotted-redefine-table.toml
--rw-r--r--   0        0        0       25 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/key/duplicate-keys.toml
--rw-r--r--   0        0        0       47 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/key/duplicate.toml
--rw-r--r--   0        0        0        5 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/key/empty.toml
--rw-r--r--   0        0        0       45 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/key/escape.toml
--rw-r--r--   0        0        0        7 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/key/hash.toml
--rw-r--r--   0        0        0       19 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/key/multiline.toml
--rw-r--r--   0        0        0       17 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/key/newline.toml
--rw-r--r--   0        0        0       12 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/key/no-eol.toml
--rw-r--r--   0        0        0        9 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/key/open-bracket.toml
--rw-r--r--   0        0        0       20 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/key/partial-quoted.toml
--rw-r--r--   0        0        0        2 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/key/single-open-bracket.toml
--rw-r--r--   0        0        0        8 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/key/space.toml
--rw-r--r--   0        0        0       29 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/key/special-character.toml
--rw-r--r--   0        0        0       17 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/key/start-bracket.toml
--rw-r--r--   0        0        0        9 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/key/two-equals.toml
--rw-r--r--   0        0        0        5 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/key/two-equals2.toml
--rw-r--r--   0        0        0        6 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/key/two-equals3.toml
--rw-r--r--   0        0        0        4 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/key/without-value-1.toml
--rw-r--r--   0        0        0        7 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/key/without-value-2.toml
--rw-r--r--   0        0        0       17 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/bad-byte-escape.toml
--rw-r--r--   0        0        0       81 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/bad-codepoint.toml
--rw-r--r--   0        0        0       29 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/bad-concat.toml
--rw-r--r--   0        0        0       62 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/bad-escape.toml
--rw-r--r--   0        0        0       33 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/bad-multiline.toml
--rw-r--r--   0        0        0       62 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/bad-slash-escape.toml
--rw-r--r--   0        0        0       15 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/bad-uni-esc.toml
--rw-r--r--   0        0        0       16 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/basic-byte-escapes.toml
--rw-r--r--   0        0        0       21 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/basic-multiline-out-of-range-unicode-escape-1.toml
--rw-r--r--   0        0        0       21 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/basic-multiline-out-of-range-unicode-escape-2.toml
--rw-r--r--   0        0        0       50 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/basic-multiline-quotes.toml
--rw-r--r--   0        0        0       13 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/basic-multiline-unknown-escape.toml
--rw-r--r--   0        0        0       17 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/basic-out-of-range-unicode-escape-1.toml
--rw-r--r--   0        0        0       17 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/basic-out-of-range-unicode-escape-2.toml
--rw-r--r--   0        0        0        9 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/basic-unknown-escape.toml
--rw-r--r--   0        0        0       30 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/literal-multiline-quotes-1.toml
--rw-r--r--   0        0        0       42 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/literal-multiline-quotes-2.toml
--rw-r--r--   0        0        0       13 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/missing-quotes.toml
--rw-r--r--   0        0        0       28 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/multiline-escape-space.toml
--rw-r--r--   0        0        0        6 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/multiline-no-close-2.toml
--rw-r--r--   0        0        0       33 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/multiline-no-close.toml
--rw-r--r--   0        0        0       24 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/multiline-quotes-1.toml
--rw-r--r--   0        0        0       24 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/multiline-quotes-2.toml
--rw-r--r--   0        0        0       42 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/no-close.toml
--rw-r--r--   0        0        0       44 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/text-after-string.toml
--rw-r--r--   0        0        0       39 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/string/wrong-close.toml
--rw-r--r--   0        0        0       26 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/table/array-empty.toml
--rw-r--r--   0        0        0      622 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/table/array-implicit.toml
--rw-r--r--   0        0        0       31 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/table/array-missing-bracket.toml
--rw-r--r--   0        0        0       51 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/table/duplicate-key-table.toml
--rw-r--r--   0        0        0       14 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/table/duplicate-table-array.toml
--rw-r--r--   0        0        0       14 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/table/duplicate-table-array2.toml
--rw-r--r--   0        0        0       21 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/table/duplicate.toml
--rw-r--r--   0        0        0       19 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/table/empty-implicit-table.toml
--rw-r--r--   0        0        0        3 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/table/empty.toml
--rw-r--r--   0        0        0       11 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/table/equals-sign.toml
--rw-r--r--   0        0        0       11 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/table/llbrace.toml
--rw-r--r--   0        0        0       15 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/table/nested-brackets-close.toml
--rw-r--r--   0        0        0       15 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/table/nested-brackets-open.toml
--rw-r--r--   0        0        0       34 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/table/quoted-no-close.toml
--rw-r--r--   0        0        0       78 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/table/redefine.toml
--rw-r--r--   0        0        0       11 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/table/rrbrace.toml
--rw-r--r--   0        0        0       31 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/table/text-after-table.toml
--rw-r--r--   0        0        0       14 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/table/whitespace.toml
--rw-r--r--   0        0        0       24 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/invalid/table/with-pound.toml
--rw-r--r--   0        0        0      948 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/array.json
--rw-r--r--   0        0        0      205 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/array.toml
--rw-r--r--   0        0        0      131 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/bool.json
--rw-r--r--   0        0        0       18 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/bool.toml
--rw-r--r--   0        0        0       84 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/empty.json
--rw-r--r--   0        0        0       21 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/empty.toml
--rw-r--r--   0        0        0      444 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/hetergeneous.json
--rw-r--r--   0        0        0       41 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/hetergeneous.toml
--rw-r--r--   0        0        0      186 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/mixed-int-array.json
--rw-r--r--   0        0        0       53 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/mixed-int-array.toml
--rw-r--r--   0        0        0      144 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/mixed-int-float.json
--rw-r--r--   0        0        0       27 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/mixed-int-float.toml
--rw-r--r--   0        0        0      146 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/mixed-int-string.json
--rw-r--r--   0        0        0       30 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/mixed-int-string.toml
--rw-r--r--   0        0        0      393 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/mixed-string-table.json
--rw-r--r--   0        0        0      139 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/mixed-string-table.toml
--rw-r--r--   0        0        0      382 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/nested-double.json
--rw-r--r--   0        0        0       40 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/nested-double.toml
--rw-r--r--   0        0        0       43 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/nested-inline-table.json
--rw-r--r--   0        0        0       19 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/nested-inline-table.toml
--rw-r--r--   0        0        0      171 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/nested.json
--rw-r--r--   0        0        0       22 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/nested.toml
--rw-r--r--   0        0        0      190 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/nospaces.json
--rw-r--r--   0        0        0       15 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/nospaces.toml
--rw-r--r--   0        0        0       80 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/string-quote-comma-2.json
--rw-r--r--   0        0        0       20 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/string-quote-comma-2.toml
--rw-r--r--   0        0        0      167 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/string-quote-comma.json
--rw-r--r--   0        0        0       56 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/string-quote-comma.toml
--rw-r--r--   0        0        0      163 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/string-with-comma.json
--rw-r--r--   0        0        0       52 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/string-with-comma.toml
--rw-r--r--   0        0        0      273 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/strings.json
--rw-r--r--   0        0        0       67 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/strings.toml
--rw-r--r--   0        0        0      111 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/table-array-string-backslash.json
--rw-r--r--   0        0        0       31 2022-02-07 08:21:07.761160 tomlkit-0.9.1/tests/toml-test/tests/valid/array/table-array-string-backslash.toml
--rw-r--r--   0        0        0      112 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/bool/bool.json
--rw-r--r--   0        0        0       19 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/bool/bool.toml
--rw-r--r--   0        0        0       62 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/comment/at-eof.json
--rw-r--r--   0        0        0       85 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/comment/at-eof.toml
--rw-r--r--   0        0        0       62 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/comment/at-eof2.json
--rw-r--r--   0        0        0       85 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/comment/at-eof2.toml
--rw-r--r--   0        0        0      327 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/comment/everywhere.json
--rw-r--r--   0        0        0      556 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/comment/everywhere.toml
--rw-r--r--   0        0        0     1529 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/comment/tricky.json
--rw-r--r--   0        0        0      385 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/comment/tricky.toml
--rw-r--r--   0        0        0      159 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/datetime/datetime.json
--rw-r--r--   0        0        0       58 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/datetime/datetime.toml
--rw-r--r--   0        0        0       79 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/datetime/local-date.json
--rw-r--r--   0        0        0       25 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/datetime/local-date.toml
--rw-r--r--   0        0        0      157 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/datetime/local-time.json
--rw-r--r--   0        0        0       52 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/datetime/local-time.toml
--rw-r--r--   0        0        0      256 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/datetime/local.json
--rw-r--r--   0        0        0       88 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/datetime/local.toml
--rw-r--r--   0        0        0      351 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/datetime/milliseconds.json
--rw-r--r--   0        0        0      144 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/datetime/milliseconds.toml
--rw-r--r--   0        0        0      324 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/datetime/timezone.json
--rw-r--r--   0        0        0      134 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/datetime/timezone.toml
--rw-r--r--   0        0        0        3 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/empty-file.json
--rw-r--r--   0        0        0        0 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/empty-file.toml
--rw-r--r--   0        0        0      402 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/example.json
--rw-r--r--   0        0        0       91 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/example.toml
--rw-r--r--   0        0        0      489 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/float/exponent.json
--rw-r--r--   0        0        0      114 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/float/exponent.toml
--rw-r--r--   0        0        0      245 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/float/float.json
--rw-r--r--   0        0        0       59 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/float/float.toml
--rw-r--r--   0        0        0      374 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/float/inf-and-nan.json
--rw-r--r--   0        0        0      232 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/float/inf-and-nan.toml
--rw-r--r--   0        0        0      153 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/float/long.json
--rw-r--r--   0        0        0       58 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/float/long.toml
--rw-r--r--   0        0        0      196 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/float/underscore.json
--rw-r--r--   0        0        0       56 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/float/underscore.toml
--rw-r--r--   0        0        0      374 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/float/zero.json
--rw-r--r--   0        0        0       68 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/float/zero.toml
--rw-r--r--   0        0        0      206 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/implicit-and-explicit-after.json
--rw-r--r--   0        0        0       37 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/implicit-and-explicit-after.toml
--rw-r--r--   0        0        0      206 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/implicit-and-explicit-before.json
--rw-r--r--   0        0        0       37 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/implicit-and-explicit-before.toml
--rw-r--r--   0        0        0      138 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/implicit-groups.json
--rw-r--r--   0        0        0       20 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/implicit-groups.toml
--rw-r--r--   0        0        0      551 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/inline-table/array.json
--rw-r--r--   0        0        0      170 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/inline-table/array.toml
--rw-r--r--   0        0        0      141 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/inline-table/bool.json
--rw-r--r--   0        0        0       26 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/inline-table/bool.toml
--rw-r--r--   0        0        0      371 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/inline-table/empty.json
--rw-r--r--   0        0        0      157 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/inline-table/empty.toml
--rw-r--r--   0        0        0      251 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/inline-table/end-in-bool.json
--rw-r--r--   0        0        0       70 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/inline-table/end-in-bool.toml
--rw-r--r--   0        0        0      652 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/inline-table/inline-table.json
--rw-r--r--   0        0        0      157 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/inline-table/inline-table.toml
--rw-r--r--   0        0        0     2071 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/inline-table/key-dotted.json
--rw-r--r--   0        0        0      308 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/inline-table/key-dotted.toml
--rw-r--r--   0        0        0      304 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/inline-table/multiline.json
--rw-r--r--   0        0        0       88 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/inline-table/multiline.toml
--rw-r--r--   0        0        0      855 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/inline-table/nest.json
--rw-r--r--   0        0        0      372 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/inline-table/nest.toml
--rw-r--r--   0        0        0      247 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/integer/integer.json
--rw-r--r--   0        0        0       53 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/integer/integer.toml
--rw-r--r--   0        0        0      557 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/integer/literals.json
--rw-r--r--   0        0        0      151 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/integer/literals.toml
--rw-r--r--   0        0        0      168 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/integer/long.json
--rw-r--r--   0        0        0       69 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/integer/long.toml
--rw-r--r--   0        0        0      120 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/integer/underscore.json
--rw-r--r--   0        0        0       25 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/integer/underscore.toml
--rw-r--r--   0        0        0      663 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/integer/zero.json
--rw-r--r--   0        0        0      122 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/integer/zero.toml
--rw-r--r--   0        0        0      664 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/key/alphanum.json
--rw-r--r--   0        0        0      173 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/key/alphanum.toml
--rw-r--r--   0        0        0      633 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/key/case-sensitive.json
--rw-r--r--   0        0        0      203 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/key/case-sensitive.toml
--rw-r--r--   0        0        0     2017 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/key/dotted.json
--rw-r--r--   0        0        0      535 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/key/dotted.toml
--rw-r--r--   0        0        0       59 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/key/empty.json
--rw-r--r--   0        0        0       13 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/key/empty.toml
--rw-r--r--   0        0        0       63 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/key/equals-nospace.json
--rw-r--r--   0        0        0       10 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/key/equals-nospace.toml
--rw-r--r--   0        0        0      359 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/key/escapes.json
--rw-r--r--   0        0        0      149 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/key/escapes.toml
--rw-r--r--   0        0        0       78 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/key/numeric-dotted.json
--rw-r--r--   0        0        0        8 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/key/numeric-dotted.toml
--rw-r--r--   0        0        0       57 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/key/numeric.json
--rw-r--r--   0        0        0        6 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/key/numeric.toml
--rw-r--r--   0        0        0      476 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/key/quoted-dots.json
--rw-r--r--   0        0        0      112 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/key/quoted-dots.toml
--rw-r--r--   0        0        0       59 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/key/space.json
--rw-r--r--   0        0        0       10 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/key/space.toml
--rw-r--r--   0        0        0      106 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/key/special-chars.json
--rw-r--r--   0        0        0       42 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/key/special-chars.toml
--rw-r--r--   0        0        0      261 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/key/special-word.json
--rw-r--r--   0        0        0       73 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/key/special-word.toml
--rw-r--r--   0        0        0      121 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/newline-crlf.json
--rw-r--r--   0        0        0       30 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/newline-crlf.toml
--rw-r--r--   0        0        0      120 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/newline-lf.json
--rw-r--r--   0        0        0       27 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/newline-lf.toml
--rw-r--r--   0        0        0     1611 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/spec-example-1-compact.json
--rw-r--r--   0        0        0      376 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/spec-example-1-compact.toml
--rw-r--r--   0        0        0     1611 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/spec-example-1.json
--rw-r--r--   0        0        0      559 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/spec-example-1.toml
--rw-r--r--   0        0        0       65 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/double-quote-escape.json
--rw-r--r--   0        0        0       17 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/double-quote-escape.toml
--rw-r--r--   0        0        0       60 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/empty.json
--rw-r--r--   0        0        0       12 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/empty.toml
--rw-r--r--   0        0        0      621 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/escape-tricky.json
--rw-r--r--   0        0        0      328 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/escape-tricky.toml
--rw-r--r--   0        0        0       65 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/escaped-escape.json
--rw-r--r--   0        0        0       17 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/escaped-escape.toml
--rw-r--r--   0        0        0     1353 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/escapes.json
--rw-r--r--   0        0        0      771 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/escapes.toml
--rw-r--r--   0        0        0     1071 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/multiline-json
--rw-r--r--   0        0        0      736 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/multiline-quotes.json
--rw-r--r--   0        0        0      448 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/multiline-quotes.toml
--rw-r--r--   0        0        0      719 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/multiline-toml
--rw-r--r--   0        0        0      337 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/nl.json
--rw-r--r--   0        0        0      115 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/nl.toml
--rw-r--r--   0        0        0      323 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/raw-multiline.json
--rw-r--r--   0        0        0      195 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/raw-multiline.toml
--rw-r--r--   0        0        0      699 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/raw.json
--rw-r--r--   0        0        0      373 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/raw.toml
--rw-r--r--   0        0        0       95 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/simple.json
--rw-r--r--   0        0        0       47 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/simple.toml
--rw-r--r--   0        0        0      123 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/unicode-escape.json
--rw-r--r--   0        0        0       42 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/unicode-escape.toml
--rw-r--r--   0        0        0       62 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/unicode-literal.json
--rw-r--r--   0        0        0       14 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/unicode-literal.toml
--rw-r--r--   0        0        0      183 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/with-pound.json
--rw-r--r--   0        0        0      113 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/string/with-pound.toml
--rw-r--r--   0        0        0      147 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/array-implicit.json
--rw-r--r--   0        0        0       37 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/array-implicit.toml
--rw-r--r--   0        0        0      551 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/array-many.json
--rw-r--r--   0        0        0      163 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/array-many.toml
--rw-r--r--   0        0        0      754 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/array-nest.json
--rw-r--r--   0        0        0      262 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/array-nest.toml
--rw-r--r--   0        0        0      202 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/array-one.json
--rw-r--r--   0        0        0       58 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/array-one.toml
--rw-r--r--   0        0        0      339 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/array-table-array.json
--rw-r--r--   0        0        0      108 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/array-table-array.toml
--rw-r--r--   0        0        0       14 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/empty.json
--rw-r--r--   0        0        0        4 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/empty.toml
--rw-r--r--   0        0        0       58 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/keyword.json
--rw-r--r--   0        0        0       32 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/keyword.toml
--rw-r--r--   0        0        0      274 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/names.json
--rw-r--r--   0        0        0       90 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/names.toml
--rw-r--r--   0        0        0       18 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/no-eol.json
--rw-r--r--   0        0        0        8 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/no-eol.toml
--rw-r--r--   0        0        0       29 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/sub-empty.json
--rw-r--r--   0        0        0       10 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/sub-empty.toml
--rw-r--r--   0        0        0       22 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/whitespace.json
--rw-r--r--   0        0        0       14 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/whitespace.toml
--rw-r--r--   0        0        0      142 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/with-literal-string.json
--rw-r--r--   0        0        0       41 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/with-literal-string.toml
--rw-r--r--   0        0        0       92 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/with-pound.json
--rw-r--r--   0        0        0       26 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/with-pound.toml
--rw-r--r--   0        0        0      138 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/with-single-quotes.json
--rw-r--r--   0        0        0       37 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/with-single-quotes.toml
--rw-r--r--   0        0        0       71 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/without-super.json
--rw-r--r--   0        0        0      120 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/tests/valid/table/without-super.toml
--rw-r--r--   0        0        0     3162 2022-02-07 08:21:07.765161 tomlkit-0.9.1/tests/toml-test/toml.go
--rw-r--r--   0        0        0      952 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tomlkit/__init__.py
--rw-r--r--   0        0        0      527 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tomlkit/_compat.py
--rw-r--r--   0        0        0     3533 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tomlkit/_utils.py
--rw-r--r--   0        0        0     6137 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tomlkit/api.py
--rw-r--r--   0        0        0    27993 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tomlkit/container.py
--rw-r--r--   0        0        0     5064 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tomlkit/exceptions.py
--rw-r--r--   0        0        0    42197 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tomlkit/items.py
--rw-r--r--   0        0        0    36938 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tomlkit/parser.py
--rw-r--r--   0        0        0        0 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tomlkit/py.typed
--rw-r--r--   0        0        0     4920 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tomlkit/source.py
--rw-r--r--   0        0        0     1498 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tomlkit/toml_char.py
--rw-r--r--   0        0        0      103 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tomlkit/toml_document.py
--rw-r--r--   0        0        0      668 2022-02-07 08:21:06.841024 tomlkit-0.9.1/tomlkit/toml_file.py
--rw-r--r--   0        0        0     2574 2022-02-07 08:21:21.648804 tomlkit-0.9.1/setup.py
--rw-r--r--   0        0        0     2657 2022-02-07 08:21:21.649541 tomlkit-0.9.1/PKG-INFO
+-rw-r--r--   0        0        0     1062 2022-02-08 11:23:51.381533 tomlkit-0.9.2/LICENSE
+-rw-r--r--   0        0        0     1962 2022-02-08 11:23:51.381533 tomlkit-0.9.2/README.md
+-rw-r--r--   0        0        0     1078 2022-02-08 11:23:51.381533 tomlkit-0.9.2/pyproject.toml
+-rw-r--r--   0        0        0        0 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/__init__.py
+-rw-r--r--   0        0        0     2957 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/conftest.py
+-rw-r--r--   0        0        0      706 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/0.5.0.toml
+-rw-r--r--   0        0        0      870 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/example.toml
+-rw-r--r--   0        0        0      194 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/fruit.toml
+-rw-r--r--   0        0        0     1405 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/hard.toml
+-rw-r--r--   0        0        0       20 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/invalid/array_duplicate_comma.toml
+-rw-r--r--   0        0        0       17 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/invalid/array_leading_comma.toml
+-rw-r--r--   0        0        0       17 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/invalid/array_no_comma.toml
+-rw-r--r--   0        0        0      141 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/invalid/array_with_invalid_chars.toml
+-rw-r--r--   0        0        0       27 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/invalid/inline_table_duplicate_comma.toml
+-rw-r--r--   0        0        0       21 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/invalid/inline_table_leading_comma.toml
+-rw-r--r--   0        0        0       24 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/invalid/inline_table_no_comma.toml
+-rw-r--r--   0        0        0       21 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/invalid/inline_table_trailing_comma.toml
+-rw-r--r--   0        0        0       18 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/invalid/invalid_date.toml
+-rw-r--r--   0        0        0       31 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/invalid/invalid_datetime.toml
+-rw-r--r--   0        0        0       15 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/invalid/invalid_number.toml
+-rw-r--r--   0        0        0       20 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/invalid/invalid_time.toml
+-rw-r--r--   0        0        0      160 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/invalid/key_value_with_trailing_chars.toml
+-rw-r--r--   0        0        0       24 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/invalid/newline_in_singleline_string.toml
+-rw-r--r--   0        0        0       58 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/invalid/section_with_trailing_characters.toml
+-rw-r--r--   0        0        0       38 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/invalid/string_slash_whitespace_char.toml
+-rw-r--r--   0        0        0       29 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/invalid/trailing_comma.toml
+-rw-r--r--   0        0        0      676 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/json/0.5.0.json
+-rw-r--r--   0        0        0     3340 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/json/pyproject.json
+-rw-r--r--   0        0        0      299 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/json/table_names.json
+-rw-r--r--   0        0        0       53 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/newline_in_strings.toml
+-rw-r--r--   0        0        0       26 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/preserve_quotes_in_string.toml
+-rw-r--r--   0        0        0     1994 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/pyproject.toml
+-rw-r--r--   0        0        0      100 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/sections_with_same_start.toml
+-rw-r--r--   0        0        0       82 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/string_slash_whitespace_newline.toml
+-rw-r--r--   0        0        0      143 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/table_names.toml
+-rw-r--r--   0        0        0     1579 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/examples/test.toml
+-rw-r--r--   0        0        0     9495 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/test_api.py
+-rw-r--r--   0        0        0     3089 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/test_build.py
+-rw-r--r--   0        0        0    13424 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/test_items.py
+-rw-r--r--   0        0        0      962 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/test_parser.py
+-rw-r--r--   0        0        0    16630 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/test_toml_document.py
+-rw-r--r--   0        0        0     1638 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/test_toml_file.py
+-rw-r--r--   0        0        0     3482 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/test_toml_spec_tests.py
+-rw-r--r--   0        0        0     1571 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/test_toml_tests.py
+-rw-r--r--   0        0        0     1402 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/test_utils.py
+-rw-r--r--   0        0        0      437 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/test_write.py
+-rw-r--r--   0        0        0       68 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/.gitattributes
+-rw-r--r--   0        0        0      742 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/LICENSE
+-rw-r--r--   0        0        0      638 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/README.md
+-rw-r--r--   0        0        0       55 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/array-of-tables-1.toml
+-rw-r--r--   0        0        0      188 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/array-of-tables-2.toml
+-rw-r--r--   0        0        0       15 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/bare-key-1.toml
+-rw-r--r--   0        0        0       17 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/bare-key-2.toml
+-rw-r--r--   0        0        0        9 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/bare-key-3.toml
+-rw-r--r--   0        0        0       15 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/comment-control-1.toml
+-rw-r--r--   0        0        0       17 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/comment-control-2.toml
+-rw-r--r--   0        0        0       17 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/comment-control-3.toml
+-rw-r--r--   0        0        0       15 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/comment-control-4.toml
+-rw-r--r--   0        0        0       66 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/inline-table-imutable-1.toml
+-rw-r--r--   0        0        0       66 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/inline-table-imutable-2.toml
+-rw-r--r--   0        0        0       21 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/inline-table-trailing-comma.toml
+-rw-r--r--   0        0        0       11 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/int-0-padded.toml
+-rw-r--r--   0        0        0       12 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/int-signed-bin.toml
+-rw-r--r--   0        0        0       12 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/int-signed-hex.toml
+-rw-r--r--   0        0        0       12 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/int-signed-oct.toml
+-rw-r--r--   0        0        0       16 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/key-value-pair-1.toml
+-rw-r--r--   0        0        0       48 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/key-value-pair-2.toml
+-rw-r--r--   0        0        0      225 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/multiple-dot-key.toml
+-rw-r--r--   0        0        0       47 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/multiple-key.toml
+-rw-r--r--   0        0        0       27 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/no-key-name.toml
+-rw-r--r--   0        0        0       12 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/string-basic-control-1.toml
+-rw-r--r--   0        0        0       14 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/string-basic-control-2.toml
+-rw-r--r--   0        0        0       14 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/string-basic-control-3.toml
+-rw-r--r--   0        0        0       12 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/string-basic-control-4.toml
+-rw-r--r--   0        0        0       16 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/string-basic-multiline-control-1.toml
+-rw-r--r--   0        0        0       16 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/string-basic-multiline-control-2.toml
+-rw-r--r--   0        0        0       16 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/string-basic-multiline-control-3.toml
+-rw-r--r--   0        0        0       16 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/string-basic-multiline-control-4.toml
+-rw-r--r--   0        0        0       28 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/string-basic-multiline-invalid-backslash.toml
+-rw-r--r--   0        0        0       21 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/string-basic-multiline-out-of-range-unicode-escape-1.toml
+-rw-r--r--   0        0        0       21 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/string-basic-multiline-out-of-range-unicode-escape-2.toml
+-rw-r--r--   0        0        0       50 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/string-basic-multiline-quotes.toml
+-rw-r--r--   0        0        0       13 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/string-basic-multiline-unknown-escape.toml
+-rw-r--r--   0        0        0       17 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/string-basic-out-of-range-unicode-escape-1.toml
+-rw-r--r--   0        0        0       17 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/string-basic-out-of-range-unicode-escape-2.toml
+-rw-r--r--   0        0        0        9 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/string-basic-unknown-escape.toml
+-rw-r--r--   0        0        0       12 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/string-literal-control-1.toml
+-rw-r--r--   0        0        0       12 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/string-literal-control-2.toml
+-rw-r--r--   0        0        0       12 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/string-literal-control-3.toml
+-rw-r--r--   0        0        0       12 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/string-literal-control-4.toml
+-rw-r--r--   0        0        0       16 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/string-literal-multiline-control-1.toml
+-rw-r--r--   0        0        0       16 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/string-literal-multiline-control-2.toml
+-rw-r--r--   0        0        0       16 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/string-literal-multiline-control-3.toml
+-rw-r--r--   0        0        0       16 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/string-literal-multiline-control-4.toml
+-rw-r--r--   0        0        0       72 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/string-literal-multiline-quotes.toml
+-rw-r--r--   0        0        0       67 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/table-1.toml
+-rw-r--r--   0        0        0       81 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/table-2.toml
+-rw-r--r--   0        0        0       79 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/table-3.toml
+-rw-r--r--   0        0        0       85 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/table-4.toml
+-rw-r--r--   0        0        0      242 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/table-invalid-1.toml
+-rw-r--r--   0        0        0       55 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/table-invalid-2.toml
+-rw-r--r--   0        0        0      265 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/table-invalid-3.toml
+-rw-r--r--   0        0        0      262 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/errors/table-invalid-4.toml
+-rw-r--r--   0        0        0    13018 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/values/qa-array-inline-1000.toml
+-rw-r--r--   0        0        0    12014 2022-02-08 11:23:51.381533 tomlkit-0.9.2/tests/toml-spec-tests/values/qa-array-inline-1000.yaml
+-rw-r--r--   0        0        0     2010 2022-02-08 11:23:51.385533 tomlkit-0.9.2/tests/toml-spec-tests/values/qa-array-inline-nested-1000.toml
+-rw-r--r--   0        0        0     2011 2022-02-08 11:23:51.385533 tomlkit-0.9.2/tests/toml-spec-tests/values/qa-array-inline-nested-1000.yaml
+-rw-r--r--   0        0        0    40015 2022-02-08 11:23:51.385533 tomlkit-0.9.2/tests/toml-spec-tests/values/qa-key-literal-40kb.toml
+-rw-r--r--   0        0        0    40016 2022-02-08 11:23:51.385533 tomlkit-0.9.2/tests/toml-spec-tests/values/qa-key-literal-40kb.yaml
+-rw-r--r--   0        0        0    40015 2022-02-08 11:23:51.385533 tomlkit-0.9.2/tests/toml-spec-tests/values/qa-key-string-40kb.toml
+-rw-r--r--   0        0        0    40016 2022-02-08 11:23:51.385533 tomlkit-0.9.2/tests/toml-spec-tests/values/qa-key-string-40kb.yaml
+-rw-r--r--   0        0        0    40013 2022-02-08 11:23:51.385533 tomlkit-0.9.2/tests/toml-spec-tests/values/qa-scalar-literal-40kb.toml
+-rw-r--r--   0        0        0    41074 2022-02-08 11:23:51.385533 tomlkit-0.9.2/tests/toml-spec-tests/values/qa-scalar-literal-40kb.yaml
+-rw-r--r--   0        0        0    40017 2022-02-08 11:23:51.385533 tomlkit-0.9.2/tests/toml-spec-tests/values/qa-scalar-literal-multiline-40kb.toml
+-rw-r--r--   0        0        0    41155 2022-02-08 11:23:51.385533 tomlkit-0.9.2/tests/toml-spec-tests/values/qa-scalar-literal-multiline-40kb.yaml
+-rw-r--r--   0        0        0    40013 2022-02-08 11:23:51.385533 tomlkit-0.9.2/tests/toml-spec-tests/values/qa-scalar-string-40kb.toml
+-rw-r--r--   0        0        0    41074 2022-02-08 11:23:51.385533 tomlkit-0.9.2/tests/toml-spec-tests/values/qa-scalar-string-40kb.yaml
+-rw-r--r--   0        0        0    40017 2022-02-08 11:23:51.385533 tomlkit-0.9.2/tests/toml-spec-tests/values/qa-scalar-string-multiline-40kb.toml
+-rw-r--r--   0        0        0    41155 2022-02-08 11:23:51.385533 tomlkit-0.9.2/tests/toml-spec-tests/values/qa-scalar-string-multiline-40kb.yaml
+-rw-r--r--   0        0        0    19913 2022-02-08 11:23:51.385533 tomlkit-0.9.2/tests/toml-spec-tests/values/qa-table-inline-1000.toml
+-rw-r--r--   0        0        0    17911 2022-02-08 11:23:51.385533 tomlkit-0.9.2/tests/toml-spec-tests/values/qa-table-inline-1000.yaml
+-rw-r--r--   0        0        0     8010 2022-02-08 11:23:51.385533 tomlkit-0.9.2/tests/toml-spec-tests/values/qa-table-inline-nested-1000.toml
+-rw-r--r--   0        0        0  1006009 2022-02-08 11:23:51.385533 tomlkit-0.9.2/tests/toml-spec-tests/values/qa-table-inline-nested-1000.yaml
+-rw-r--r--   0        0        0       23 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-array-1.toml
+-rw-r--r--   0        0        0       22 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-array-1.yaml
+-rw-r--r--   0        0        0       38 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-array-2.toml
+-rw-r--r--   0        0        0       37 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-array-2.yaml
+-rw-r--r--   0        0        0       46 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-array-3.toml
+-rw-r--r--   0        0        0       45 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-array-3.yaml
+-rw-r--r--   0        0        0       67 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-array-4.toml
+-rw-r--r--   0        0        0       59 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-array-4.yaml
+-rw-r--r--   0        0        0       51 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-array-5.toml
+-rw-r--r--   0        0        0       50 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-array-5.yaml
+-rw-r--r--   0        0        0       26 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-array-7.toml
+-rw-r--r--   0        0        0       25 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-array-7.yaml
+-rw-r--r--   0        0        0       39 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-array-8.toml
+-rw-r--r--   0        0        0       38 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-array-8.yaml
+-rw-r--r--   0        0        0       37 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-array-mixed-number-types.toml
+-rw-r--r--   0        0        0       36 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-array-mixed-number-types.yaml
+-rw-r--r--   0        0        0      138 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-array-more-mixed-types.toml
+-rw-r--r--   0        0        0      135 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-array-more-mixed-types.yaml
+-rw-r--r--   0        0        0      118 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-array-of-tables-1.toml
+-rw-r--r--   0        0        0      105 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-array-of-tables-1.yaml
+-rw-r--r--   0        0        0      252 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-array-of-tables-2.toml
+-rw-r--r--   0        0        0      264 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-array-of-tables-2.yaml
+-rw-r--r--   0        0        0      109 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-array-of-tables-3.toml
+-rw-r--r--   0        0        0       97 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-array-of-tables-3.yaml
+-rw-r--r--   0        0        0       13 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-boolean-1.toml
+-rw-r--r--   0        0        0       12 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-boolean-1.yaml
+-rw-r--r--   0        0        0       14 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-boolean-2.toml
+-rw-r--r--   0        0        0       13 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-boolean-2.yaml
+-rw-r--r--   0        0        0       46 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-case-sensitive.toml
+-rw-r--r--   0        0        0       18 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-case-sensitive.yaml
+-rw-r--r--   0        0        0      120 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-comment-mid-array.toml
+-rw-r--r--   0        0        0      119 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-comment-mid-array.yaml
+-rw-r--r--   0        0        0       36 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-comment-mid-string.toml
+-rw-r--r--   0        0        0       35 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-comment-mid-string.yaml
+-rw-r--r--   0        0        0      134 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-comment-tab.toml
+-rw-r--r--   0        0        0       13 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-comment-tab.yaml
+-rw-r--r--   0        0        0       85 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-comment.toml
+-rw-r--r--   0        0        0       84 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-comment.yaml
+-rw-r--r--   0        0        0       65 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-date-local-1.json
+-rw-r--r--   0        0        0       17 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-date-local-1.toml
+-rw-r--r--   0        0        0       28 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-date-time-1.toml
+-rw-r--r--   0        0        0       27 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-date-time-1.yaml
+-rw-r--r--   0        0        0       33 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-date-time-2.toml
+-rw-r--r--   0        0        0       32 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-date-time-2.yaml
+-rw-r--r--   0        0        0       40 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-date-time-3.toml
+-rw-r--r--   0        0        0       39 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-date-time-3.yaml
+-rw-r--r--   0        0        0       28 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-date-time-4.toml
+-rw-r--r--   0        0        0       27 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-date-time-4.yaml
+-rw-r--r--   0        0        0       32 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-date-time-5.toml
+-rw-r--r--   0        0        0       31 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-date-time-5.yaml
+-rw-r--r--   0        0        0       33 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-date-time-6.toml
+-rw-r--r--   0        0        0       31 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-date-time-6.yaml
+-rw-r--r--   0        0        0       89 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-date-time-local-1.json
+-rw-r--r--   0        0        0       27 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-date-time-local-1.toml
+-rw-r--r--   0        0        0       89 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-date-time-local-2.json
+-rw-r--r--   0        0        0       34 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-date-time-local-2.toml
+-rw-r--r--   0        0        0       92 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-dotted-keys-1.toml
+-rw-r--r--   0        0        0       87 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-dotted-keys-1.yaml
+-rw-r--r--   0        0        0       13 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-dotted-keys-2.toml
+-rw-r--r--   0        0        0       11 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-dotted-keys-2.yaml
+-rw-r--r--   0        0        0       14 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-dotted-keys-3.toml
+-rw-r--r--   0        0        0       11 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-dotted-keys-3.yaml
+-rw-r--r--   0        0        0       41 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-empty-key-name-1.toml
+-rw-r--r--   0        0        0       12 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-empty-key-name-1.yaml
+-rw-r--r--   0        0        0       41 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-empty-key-name-2.toml
+-rw-r--r--   0        0        0       12 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-empty-key-name-2.yaml
+-rw-r--r--   0        0        0      139 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-extend-dotted-object-1.toml
+-rw-r--r--   0        0        0       45 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-extend-dotted-object-1.yaml
+-rw-r--r--   0        0        0      156 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-extend-dotted-object-2.toml
+-rw-r--r--   0        0        0      112 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-extend-dotted-object-2.yaml
+-rw-r--r--   0        0        0      145 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-extend-dotted-object-3.toml
+-rw-r--r--   0        0        0      112 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-extend-dotted-object-3.yaml
+-rw-r--r--   0        0        0       12 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-1.toml
+-rw-r--r--   0        0        0       10 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-1.yaml
+-rw-r--r--   0        0        0       31 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-10.toml
+-rw-r--r--   0        0        0       31 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-10.yaml
+-rw-r--r--   0        0        0       31 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-11.toml
+-rw-r--r--   0        0        0       31 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-11.yaml
+-rw-r--r--   0        0        0       31 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-12.toml
+-rw-r--r--   0        0        0       32 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-12.yaml
+-rw-r--r--   0        0        0       66 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-13.toml
+-rw-r--r--   0        0        0       66 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-13.yaml
+-rw-r--r--   0        0        0       27 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-14.toml
+-rw-r--r--   0        0        0       10 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-14.yaml
+-rw-r--r--   0        0        0       63 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-15.toml
+-rw-r--r--   0        0        0       10 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-15.yaml
+-rw-r--r--   0        0        0       14 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-2.toml
+-rw-r--r--   0        0        0       13 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-2.yaml
+-rw-r--r--   0        0        0       13 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-3.toml
+-rw-r--r--   0        0        0       12 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-3.yaml
+-rw-r--r--   0        0        0       13 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-4.toml
+-rw-r--r--   0        0        0       12 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-4.yaml
+-rw-r--r--   0        0        0       12 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-5.toml
+-rw-r--r--   0        0        0       10 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-5.yaml
+-rw-r--r--   0        0        0       13 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-6.toml
+-rw-r--r--   0        0        0       12 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-6.yaml
+-rw-r--r--   0        0        0       17 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-7.toml
+-rw-r--r--   0        0        0       16 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-7.yaml
+-rw-r--r--   0        0        0       27 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-8.toml
+-rw-r--r--   0        0        0       25 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-8.yaml
+-rw-r--r--   0        0        0       12 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-9.toml
+-rw-r--r--   0        0        0       11 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-float-9.yaml
+-rw-r--r--   0        0        0       11 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-1.toml
+-rw-r--r--   0        0        0        9 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-1.yaml
+-rw-r--r--   0        0        0       10 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-2.toml
+-rw-r--r--   0        0        0        9 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-2.yaml
+-rw-r--r--   0        0        0        9 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-3.toml
+-rw-r--r--   0        0        0        8 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-3.yaml
+-rw-r--r--   0        0        0       10 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-3a.toml
+-rw-r--r--   0        0        0        8 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-3a.yaml
+-rw-r--r--   0        0        0       10 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-3b.toml
+-rw-r--r--   0        0        0        8 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-3b.yaml
+-rw-r--r--   0        0        0       11 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-4.toml
+-rw-r--r--   0        0        0       10 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-4.yaml
+-rw-r--r--   0        0        0       13 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-5.toml
+-rw-r--r--   0        0        0       12 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-5.yaml
+-rw-r--r--   0        0        0       17 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-6.toml
+-rw-r--r--   0        0        0       16 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-6.yaml
+-rw-r--r--   0        0        0       45 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-7.toml
+-rw-r--r--   0        0        0       44 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-7.yaml
+-rw-r--r--   0        0        0       18 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-bin1.toml
+-rw-r--r--   0        0        0       10 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-bin1.yaml
+-rw-r--r--   0        0        0       18 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-hex1.toml
+-rw-r--r--   0        0        0       17 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-hex1.yaml
+-rw-r--r--   0        0        0       18 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-hex2.toml
+-rw-r--r--   0        0        0       17 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-hex2.yaml
+-rw-r--r--   0        0        0       19 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-hex3.toml
+-rw-r--r--   0        0        0       17 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-hex3.yaml
+-rw-r--r--   0        0        0       67 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-max.json
+-rw-r--r--   0        0        0       30 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-max.toml
+-rw-r--r--   0        0        0       68 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-min.json
+-rw-r--r--   0        0        0       31 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-min.toml
+-rw-r--r--   0        0        0       18 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-oct1.toml
+-rw-r--r--   0        0        0       13 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-oct1.yaml
+-rw-r--r--   0        0        0       48 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-oct2.toml
+-rw-r--r--   0        0        0       10 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-int-oct2.yaml
+-rw-r--r--   0        0        0       14 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-key-value-pair-1.toml
+-rw-r--r--   0        0        0       13 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-key-value-pair-1.yaml
+-rw-r--r--   0        0        0       19 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-key-value-pair-2.toml
+-rw-r--r--   0        0        0       18 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-key-value-pair-2.yaml
+-rw-r--r--   0        0        0       19 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-key-value-pair-3.toml
+-rw-r--r--   0        0        0       18 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-key-value-pair-3.yaml
+-rw-r--r--   0        0        0       15 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-key-value-pair-4.toml
+-rw-r--r--   0        0        0       16 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-key-value-pair-4.yaml
+-rw-r--r--   0        0        0       13 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-key-value-pair-5.toml
+-rw-r--r--   0        0        0       16 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-key-value-pair-5.yaml
+-rw-r--r--   0        0        0        4 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-key-value-pair-6.toml
+-rw-r--r--   0        0        0        6 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-key-value-pair-6.yaml
+-rw-r--r--   0        0        0        4 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-key-value-pair-7.toml
+-rw-r--r--   0        0        0        6 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-key-value-pair-7.yaml
+-rw-r--r--   0        0        0       12 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-key-value-pair-8.toml
+-rw-r--r--   0        0        0       14 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-key-value-pair-8.yaml
+-rw-r--r--   0        0        0       15 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-key-value-pair-9.toml
+-rw-r--r--   0        0        0       17 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-key-value-pair-9.yaml
+-rw-r--r--   0        0        0       20 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-newline-1.toml
+-rw-r--r--   0        0        0       18 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-newline-1.yaml
+-rw-r--r--   0        0        0       22 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-newline-2.toml
+-rw-r--r--   0        0        0       18 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-newline-2.yaml
+-rw-r--r--   0        0        0       30 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-newline-3.toml
+-rw-r--r--   0        0        0       27 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-newline-3.yaml
+-rw-r--r--   0        0        0       19 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-quoted-basic-keys-1.toml
+-rw-r--r--   0        0        0       18 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-quoted-basic-keys-1.yaml
+-rw-r--r--   0        0        0       27 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-quoted-literal-keys-1.toml
+-rw-r--r--   0        0        0       26 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-quoted-literal-keys-1.yaml
+-rw-r--r--   0        0        0      545 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-readme-example.toml
+-rw-r--r--   0        0        0      432 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-readme-example.yaml
+-rw-r--r--   0        0        0       45 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-basic-multiline-1.toml
+-rw-r--r--   0        0        0       40 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-basic-multiline-1.yaml
+-rw-r--r--   0        0        0       70 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-basic-multiline-2.toml
+-rw-r--r--   0        0        0       52 2022-02-08 11:23:51.389533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-basic-multiline-2.yaml
+-rw-r--r--   0        0        0       89 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-basic-multiline-3.toml
+-rw-r--r--   0        0        0       52 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-basic-multiline-3.yaml
+-rw-r--r--   0        0        0       22 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-basic-multiline-4.toml
+-rw-r--r--   0        0        0       12 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-basic-multiline-4.yaml
+-rw-r--r--   0        0        0       57 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-basic-multiline-5.toml
+-rw-r--r--   0        0        0       44 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-basic-multiline-5.yaml
+-rw-r--r--   0        0        0       62 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-basic-multiline-6.toml
+-rw-r--r--   0        0        0       57 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-basic-multiline-6.yaml
+-rw-r--r--   0        0        0       51 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-basic-multiline-7.toml
+-rw-r--r--   0        0        0       45 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-basic-multiline-7.yaml
+-rw-r--r--   0        0        0       69 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-basic-multiline-8.toml
+-rw-r--r--   0        0        0       59 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-basic-multiline-8.yaml
+-rw-r--r--   0        0        0       64 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-basic-multiline-9.toml
+-rw-r--r--   0        0        0       59 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-basic-multiline-9.yaml
+-rw-r--r--   0        0        0       26 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-basic-tab-multiline.toml
+-rw-r--r--   0        0        0       22 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-basic-tab-multiline.yaml
+-rw-r--r--   0        0        0       22 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-basic-tab.toml
+-rw-r--r--   0        0        0       22 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-basic-tab.yaml
+-rw-r--r--   0        0        0       75 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-basic.toml
+-rw-r--r--   0        0        0       74 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-basic.yaml
+-rw-r--r--   0        0        0        9 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-escape-1.toml
+-rw-r--r--   0        0        0        8 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-escape-1.yaml
+-rw-r--r--   0        0        0        9 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-escape-2.toml
+-rw-r--r--   0        0        0        8 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-escape-2.yaml
+-rw-r--r--   0        0        0        9 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-escape-3.toml
+-rw-r--r--   0        0        0        8 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-escape-3.yaml
+-rw-r--r--   0        0        0        9 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-escape-4.toml
+-rw-r--r--   0        0        0        8 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-escape-4.yaml
+-rw-r--r--   0        0        0        9 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-escape-5.toml
+-rw-r--r--   0        0        0        8 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-escape-5.yaml
+-rw-r--r--   0        0        0        9 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-escape-6.toml
+-rw-r--r--   0        0        0        8 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-escape-6.yaml
+-rw-r--r--   0        0        0        9 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-escape-7.toml
+-rw-r--r--   0        0        0        8 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-escape-7.yaml
+-rw-r--r--   0        0        0       13 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-escape-8.toml
+-rw-r--r--   0        0        0       10 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-escape-8.yaml
+-rw-r--r--   0        0        0       17 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-escape-9.toml
+-rw-r--r--   0        0        0       10 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-escape-9.yaml
+-rw-r--r--   0        0        0       39 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-literal-1.toml
+-rw-r--r--   0        0        0       37 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-literal-1.yaml
+-rw-r--r--   0        0        0       40 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-literal-2.toml
+-rw-r--r--   0        0        0       39 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-literal-2.yaml
+-rw-r--r--   0        0        0       39 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-literal-3.toml
+-rw-r--r--   0        0        0       36 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-literal-3.yaml
+-rw-r--r--   0        0        0       24 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-literal-4.toml
+-rw-r--r--   0        0        0       20 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-literal-4.yaml
+-rw-r--r--   0        0        0       44 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-literal-multiline-1.toml
+-rw-r--r--   0        0        0       40 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-literal-multiline-1.yaml
+-rw-r--r--   0        0        0      103 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-literal-multiline-2.toml
+-rw-r--r--   0        0        0      100 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-literal-multiline-2.yaml
+-rw-r--r--   0        0        0       65 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-literal-multiline-3.toml
+-rw-r--r--   0        0        0       60 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-literal-multiline-3.yaml
+-rw-r--r--   0        0        0       52 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-literal-multiline-4.toml
+-rw-r--r--   0        0        0       47 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-string-literal-multiline-4.yaml
+-rw-r--r--   0        0        0       88 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-table-1.toml
+-rw-r--r--   0        0        0       89 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-table-1.yaml
+-rw-r--r--   0        0        0       36 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-table-2.toml
+-rw-r--r--   0        0        0       48 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-table-2.yaml
+-rw-r--r--   0        0        0        8 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-table-3.toml
+-rw-r--r--   0        0        0       18 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-table-3.yaml
+-rw-r--r--   0        0        0       37 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-table-4.toml
+-rw-r--r--   0        0        0       18 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-table-4.yaml
+-rw-r--r--   0        0        0       37 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-table-5.toml
+-rw-r--r--   0        0        0       18 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-table-5.yaml
+-rw-r--r--   0        0        0       43 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-table-6.toml
+-rw-r--r--   0        0        0       21 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-table-6.yaml
+-rw-r--r--   0        0        0      120 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-table-7.toml
+-rw-r--r--   0        0        0       27 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-table-7.yaml
+-rw-r--r--   0        0        0      116 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-table-8.toml
+-rw-r--r--   0        0        0       94 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-table-8.yaml
+-rw-r--r--   0        0        0       50 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-table-inline-1.toml
+-rw-r--r--   0        0        0       47 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-table-inline-1.yaml
+-rw-r--r--   0        0        0       25 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-table-inline-2.toml
+-rw-r--r--   0        0        0       25 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-table-inline-2.yaml
+-rw-r--r--   0        0        0       32 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-table-inline-3.toml
+-rw-r--r--   0        0        0       37 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-table-inline-3.yaml
+-rw-r--r--   0        0        0        8 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-table.toml
+-rw-r--r--   0        0        0       10 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-table.yaml
+-rw-r--r--   0        0        0       67 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-time-1.json
+-rw-r--r--   0        0        0       15 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-time-1.toml
+-rw-r--r--   0        0        0       67 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-time-2.json
+-rw-r--r--   0        0        0       22 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tests/toml-spec-tests/values/spec-time-2.toml
+-rw-r--r--   0        0        0       43 2022-02-08 11:23:51.693548 tomlkit-0.9.2/tests/toml-test/.git
+-rw-r--r--   0        0        0      762 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/.github/workflows/test.yml
+-rw-r--r--   0        0        0       17 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/.gitignore
+-rw-r--r--   0        0        0       43 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/.gogo-release
+-rw-r--r--   0        0        0     1079 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/COPYING
+-rw-r--r--   0        0        0     9153 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/README.md
+-rw-r--r--   0        0        0     4590 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/cmd/toml-test/main.go
+-rw-r--r--   0        0        0     3458 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/cmd/toml-test/usage.go
+-rwxr-xr-x   0        0        0      390 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/gen-multi.py
+-rw-r--r--   0        0        0      204 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/go.mod
+-rw-r--r--   0        0        0     1338 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/go.sum
+-rw-r--r--   0        0        0     6697 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/json.go
+-rw-r--r--   0        0        0     9646 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/runner.go
+-rw-r--r--   0        0        0       14 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/.gitattributes
+-rw-r--r--   0        0        0       18 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/array/missing-separator.toml
+-rw-r--r--   0        0        0       10 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/array/no-close-2.toml
+-rw-r--r--   0        0        0       18 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/array/no-close-table-2.toml
+-rw-r--r--   0        0        0       16 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/array/no-close-table.toml
+-rw-r--r--   0        0        0       23 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/array/no-close.toml
+-rw-r--r--   0        0        0       55 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/array/tables-1.toml
+-rw-r--r--   0        0        0      188 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/array/tables-2.toml
+-rw-r--r--   0        0        0       70 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/array/text-after-array-entries.toml
+-rw-r--r--   0        0        0       71 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/array/text-before-array-separator.toml
+-rw-r--r--   0        0        0       56 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/array/text-in-array.toml
+-rw-r--r--   0        0        0       14 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/bool/mixed-case.toml
+-rw-r--r--   0        0        0       10 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/bool/wrong-case-false.toml
+-rw-r--r--   0        0        0        9 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/bool/wrong-case-true.toml
+-rw-r--r--   0        0        0       25 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/control/comment-del.toml
+-rw-r--r--   0        0        0       26 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/control/comment-lf.toml
+-rw-r--r--   0        0        0       26 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/control/comment-null.toml
+-rw-r--r--   0        0        0       26 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/control/comment-us.toml
+-rw-r--r--   0        0        0      568 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/control/control.multi
+-rw-r--r--   0        0        0       24 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/control/multi-del.toml
+-rw-r--r--   0        0        0       23 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/control/multi-lf.toml
+-rw-r--r--   0        0        0       25 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/control/multi-null.toml
+-rw-r--r--   0        0        0       23 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/control/multi-us.toml
+-rw-r--r--   0        0        0       27 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/control/rawmulti-del.toml
+-rw-r--r--   0        0        0       26 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/control/rawmulti-lf.toml
+-rw-r--r--   0        0        0       28 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/control/rawmulti-null.toml
+-rw-r--r--   0        0        0       26 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/control/rawmulti-us.toml
+-rw-r--r--   0        0        0       24 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/control/rawstring-del.toml
+-rw-r--r--   0        0        0       23 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/control/rawstring-lf.toml
+-rw-r--r--   0        0        0       25 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/control/rawstring-null.toml
+-rw-r--r--   0        0        0       23 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/control/rawstring-us.toml
+-rw-r--r--   0        0        0       25 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/control/string-bs.toml
+-rw-r--r--   0        0        0       21 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/control/string-del.toml
+-rw-r--r--   0        0        0       20 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/control/string-lf.toml
+-rw-r--r--   0        0        0       22 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/control/string-null.toml
+-rw-r--r--   0        0        0       20 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/control/string-us.toml
+-rw-r--r--   0        0        0       25 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/datetime/impossible-date.toml
+-rw-r--r--   0        0        0       36 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/datetime/no-leads-with-milli.toml
+-rw-r--r--   0        0        0       31 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/datetime/no-leads.toml
+-rw-r--r--   0        0        0       28 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/datetime/no-secs.toml
+-rw-r--r--   0        0        0       27 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/datetime/no-t.toml
+-rw-r--r--   0        0        0       16 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/datetime/trailing-t.toml
+-rw-r--r--   0        0        0      242 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/encoding/bad-utf8-at-end.toml
+-rw-r--r--   0        0        0        4 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/encoding/bad-utf8-in-comment.toml
+-rw-r--r--   0        0        0       67 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/encoding/bad-utf8-in-string.toml
+-rw-r--r--   0        0        0       20 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/encoding/bom-not-at-start-1.toml
+-rw-r--r--   0        0        0       21 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/encoding/bom-not-at-start-2.toml
+-rw-r--r--   0        0        0       38 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/encoding/utf16-bom.toml
+-rw-r--r--   0        0        0       42 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/encoding/utf16.toml
+-rw-r--r--   0        0        0       22 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/double-point-1.toml
+-rw-r--r--   0        0        0       23 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/double-point-2.toml
+-rw-r--r--   0        0        0       22 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/exp-double-e-1.toml
+-rw-r--r--   0        0        0       23 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/exp-double-e-2.toml
+-rw-r--r--   0        0        0       23 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/exp-double-us.toml
+-rw-r--r--   0        0        0       23 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/exp-leading-us.toml
+-rw-r--r--   0        0        0       20 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/exp-point-1.toml
+-rw-r--r--   0        0        0       19 2022-02-08 11:23:52.225574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/exp-point-2.toml
+-rw-r--r--   0        0        0       25 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/exp-trailing-us.toml
+-rw-r--r--   0        0        0      697 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/float.multi
+-rw-r--r--   0        0        0       22 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/inf-incomplete-1.toml
+-rw-r--r--   0        0        0       23 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/inf-incomplete-2.toml
+-rw-r--r--   0        0        0       23 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/inf-incomplete-3.toml
+-rw-r--r--   0        0        0       22 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/inf_underscore.toml
+-rw-r--r--   0        0        0       28 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/leading-point-neg.toml
+-rw-r--r--   0        0        0       29 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/leading-point-plus.toml
+-rw-r--r--   0        0        0       23 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/leading-point.toml
+-rw-r--r--   0        0        0       18 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/leading-us.toml
+-rw-r--r--   0        0        0       26 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/leading-zero-neg.toml
+-rw-r--r--   0        0        0       27 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/leading-zero-plus.toml
+-rw-r--r--   0        0        0       21 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/leading-zero.toml
+-rw-r--r--   0        0        0       22 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/nan-incomplete-1.toml
+-rw-r--r--   0        0        0       23 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/nan-incomplete-2.toml
+-rw-r--r--   0        0        0       23 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/nan-incomplete-3.toml
+-rw-r--r--   0        0        0       22 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/nan_underscore.toml
+-rw-r--r--   0        0        0       25 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/trailing-point-min.toml
+-rw-r--r--   0        0        0       26 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/trailing-point-plus.toml
+-rw-r--r--   0        0        0       20 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/trailing-point.toml
+-rw-r--r--   0        0        0       19 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/trailing-us.toml
+-rw-r--r--   0        0        0       22 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/us-after-point.toml
+-rw-r--r--   0        0        0       23 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/float/us-before-point.toml
+-rw-r--r--   0        0        0       15 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/inline-table/double-comma.toml
+-rw-r--r--   0        0        0        8 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/inline-table/empty.toml
+-rw-r--r--   0        0        0      111 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/inline-table/linebreak-1.toml
+-rw-r--r--   0        0        0       15 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/inline-table/linebreak-2.toml
+-rw-r--r--   0        0        0       15 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/inline-table/linebreak-3.toml
+-rw-r--r--   0        0        0       75 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/inline-table/linebreak-4.toml
+-rw-r--r--   0        0        0       18 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/inline-table/no-comma.toml
+-rw-r--r--   0        0        0      140 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/inline-table/trailing-comma.toml
+-rw-r--r--   0        0        0       18 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/capital-bin.toml
+-rw-r--r--   0        0        0       18 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/capital-hex.toml
+-rw-r--r--   0        0        0       18 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/capital-oct.toml
+-rw-r--r--   0        0        0       23 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/double-sign-nex.toml
+-rw-r--r--   0        0        0       24 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/double-sign-plus.toml
+-rw-r--r--   0        0        0       18 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/double-us.toml
+-rw-r--r--   0        0        0      652 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/integer.multi
+-rw-r--r--   0        0        0       21 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/invalid-bin.toml
+-rw-r--r--   0        0        0       21 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/invalid-hex.toml
+-rw-r--r--   0        0        0       20 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/invalid-oct.toml
+-rw-r--r--   0        0        0       22 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/leading-us-bin.toml
+-rw-r--r--   0        0        0       22 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/leading-us-hex.toml
+-rw-r--r--   0        0        0       22 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/leading-us-oct.toml
+-rw-r--r--   0        0        0       18 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/leading-us.toml
+-rw-r--r--   0        0        0       20 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/leading-zero-1.toml
+-rw-r--r--   0        0        0       20 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/leading-zero-2.toml
+-rw-r--r--   0        0        0       26 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/leading-zero-sign-1.toml
+-rw-r--r--   0        0        0       26 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/leading-zero-sign-2.toml
+-rw-r--r--   0        0        0       27 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/negative-bin.toml
+-rw-r--r--   0        0        0       21 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/negative-hex.toml
+-rw-r--r--   0        0        0       21 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/negative-oct.toml
+-rw-r--r--   0        0        0       27 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/positive-bin.toml
+-rw-r--r--   0        0        0       21 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/positive-hex.toml
+-rw-r--r--   0        0        0       21 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/positive-oct.toml
+-rw-r--r--   0        0        0       33 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/text-after-integer.toml
+-rw-r--r--   0        0        0       23 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/trailing-us-bin.toml
+-rw-r--r--   0        0        0       23 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/trailing-us-hex.toml
+-rw-r--r--   0        0        0       23 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/trailing-us-oct.toml
+-rw-r--r--   0        0        0       19 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/trailing-us.toml
+-rw-r--r--   0        0        0       20 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/us-after-bin.toml
+-rw-r--r--   0        0        0       20 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/us-after-hex.toml
+-rw-r--r--   0        0        0       20 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/us-after-oct.toml
+-rw-r--r--   0        0        0       32 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/key/after-array.toml
+-rw-r--r--   0        0        0       36 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/key/after-table.toml
+-rw-r--r--   0        0        0       48 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/key/after-value.toml
+-rw-r--r--   0        0        0       15 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/key/bare-invalid-character.toml
+-rw-r--r--   0        0        0       76 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/key/dotted-redefine-table.toml
+-rw-r--r--   0        0        0       25 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/key/duplicate-keys.toml
+-rw-r--r--   0        0        0       47 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/key/duplicate.toml
+-rw-r--r--   0        0        0        5 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/key/empty.toml
+-rw-r--r--   0        0        0       45 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/key/escape.toml
+-rw-r--r--   0        0        0        7 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/key/hash.toml
+-rw-r--r--   0        0        0       19 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/key/multiline.toml
+-rw-r--r--   0        0        0       17 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/key/newline.toml
+-rw-r--r--   0        0        0       12 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/key/no-eol.toml
+-rw-r--r--   0        0        0        9 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/key/open-bracket.toml
+-rw-r--r--   0        0        0       20 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/key/partial-quoted.toml
+-rw-r--r--   0        0        0        2 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/key/single-open-bracket.toml
+-rw-r--r--   0        0        0        8 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/key/space.toml
+-rw-r--r--   0        0        0       29 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/key/special-character.toml
+-rw-r--r--   0        0        0       17 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/key/start-bracket.toml
+-rw-r--r--   0        0        0        9 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/key/two-equals.toml
+-rw-r--r--   0        0        0        5 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/key/two-equals2.toml
+-rw-r--r--   0        0        0        6 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/key/two-equals3.toml
+-rw-r--r--   0        0        0        4 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/key/without-value-1.toml
+-rw-r--r--   0        0        0        7 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/key/without-value-2.toml
+-rw-r--r--   0        0        0       17 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/bad-byte-escape.toml
+-rw-r--r--   0        0        0       81 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/bad-codepoint.toml
+-rw-r--r--   0        0        0       29 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/bad-concat.toml
+-rw-r--r--   0        0        0       62 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/bad-escape.toml
+-rw-r--r--   0        0        0       33 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/bad-multiline.toml
+-rw-r--r--   0        0        0       62 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/bad-slash-escape.toml
+-rw-r--r--   0        0        0       15 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/bad-uni-esc.toml
+-rw-r--r--   0        0        0       16 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/basic-byte-escapes.toml
+-rw-r--r--   0        0        0       21 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/basic-multiline-out-of-range-unicode-escape-1.toml
+-rw-r--r--   0        0        0       21 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/basic-multiline-out-of-range-unicode-escape-2.toml
+-rw-r--r--   0        0        0       50 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/basic-multiline-quotes.toml
+-rw-r--r--   0        0        0       13 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/basic-multiline-unknown-escape.toml
+-rw-r--r--   0        0        0       17 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/basic-out-of-range-unicode-escape-1.toml
+-rw-r--r--   0        0        0       17 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/basic-out-of-range-unicode-escape-2.toml
+-rw-r--r--   0        0        0        9 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/basic-unknown-escape.toml
+-rw-r--r--   0        0        0       30 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/literal-multiline-quotes-1.toml
+-rw-r--r--   0        0        0       42 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/literal-multiline-quotes-2.toml
+-rw-r--r--   0        0        0       13 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/missing-quotes.toml
+-rw-r--r--   0        0        0       28 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/multiline-escape-space.toml
+-rw-r--r--   0        0        0        6 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/multiline-no-close-2.toml
+-rw-r--r--   0        0        0       33 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/multiline-no-close.toml
+-rw-r--r--   0        0        0       24 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/multiline-quotes-1.toml
+-rw-r--r--   0        0        0       24 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/multiline-quotes-2.toml
+-rw-r--r--   0        0        0       42 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/no-close.toml
+-rw-r--r--   0        0        0       44 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/text-after-string.toml
+-rw-r--r--   0        0        0       39 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/string/wrong-close.toml
+-rw-r--r--   0        0        0       26 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/table/array-empty.toml
+-rw-r--r--   0        0        0      622 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/table/array-implicit.toml
+-rw-r--r--   0        0        0       31 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/table/array-missing-bracket.toml
+-rw-r--r--   0        0        0       51 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/table/duplicate-key-table.toml
+-rw-r--r--   0        0        0       14 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/table/duplicate-table-array.toml
+-rw-r--r--   0        0        0       14 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/table/duplicate-table-array2.toml
+-rw-r--r--   0        0        0       21 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/table/duplicate.toml
+-rw-r--r--   0        0        0       19 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/table/empty-implicit-table.toml
+-rw-r--r--   0        0        0        3 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/table/empty.toml
+-rw-r--r--   0        0        0       11 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/table/equals-sign.toml
+-rw-r--r--   0        0        0       11 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/table/llbrace.toml
+-rw-r--r--   0        0        0       15 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/table/nested-brackets-close.toml
+-rw-r--r--   0        0        0       15 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/table/nested-brackets-open.toml
+-rw-r--r--   0        0        0       34 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/table/quoted-no-close.toml
+-rw-r--r--   0        0        0       78 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/table/redefine.toml
+-rw-r--r--   0        0        0       11 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/table/rrbrace.toml
+-rw-r--r--   0        0        0       31 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/table/text-after-table.toml
+-rw-r--r--   0        0        0       14 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/table/whitespace.toml
+-rw-r--r--   0        0        0       24 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/invalid/table/with-pound.toml
+-rw-r--r--   0        0        0      948 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/array.json
+-rw-r--r--   0        0        0      205 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/array.toml
+-rw-r--r--   0        0        0      131 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/bool.json
+-rw-r--r--   0        0        0       18 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/bool.toml
+-rw-r--r--   0        0        0       84 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/empty.json
+-rw-r--r--   0        0        0       21 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/empty.toml
+-rw-r--r--   0        0        0      444 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/hetergeneous.json
+-rw-r--r--   0        0        0       41 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/hetergeneous.toml
+-rw-r--r--   0        0        0      186 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/mixed-int-array.json
+-rw-r--r--   0        0        0       53 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/mixed-int-array.toml
+-rw-r--r--   0        0        0      144 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/mixed-int-float.json
+-rw-r--r--   0        0        0       27 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/mixed-int-float.toml
+-rw-r--r--   0        0        0      146 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/mixed-int-string.json
+-rw-r--r--   0        0        0       30 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/mixed-int-string.toml
+-rw-r--r--   0        0        0      393 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/mixed-string-table.json
+-rw-r--r--   0        0        0      139 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/mixed-string-table.toml
+-rw-r--r--   0        0        0      382 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/nested-double.json
+-rw-r--r--   0        0        0       40 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/nested-double.toml
+-rw-r--r--   0        0        0       43 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/nested-inline-table.json
+-rw-r--r--   0        0        0       19 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/nested-inline-table.toml
+-rw-r--r--   0        0        0      171 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/nested.json
+-rw-r--r--   0        0        0       22 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/nested.toml
+-rw-r--r--   0        0        0      190 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/nospaces.json
+-rw-r--r--   0        0        0       15 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/nospaces.toml
+-rw-r--r--   0        0        0       80 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/string-quote-comma-2.json
+-rw-r--r--   0        0        0       20 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/string-quote-comma-2.toml
+-rw-r--r--   0        0        0      167 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/string-quote-comma.json
+-rw-r--r--   0        0        0       56 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/string-quote-comma.toml
+-rw-r--r--   0        0        0      163 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/string-with-comma.json
+-rw-r--r--   0        0        0       52 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/string-with-comma.toml
+-rw-r--r--   0        0        0      273 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/strings.json
+-rw-r--r--   0        0        0       67 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/strings.toml
+-rw-r--r--   0        0        0      111 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/table-array-string-backslash.json
+-rw-r--r--   0        0        0       31 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/array/table-array-string-backslash.toml
+-rw-r--r--   0        0        0      112 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/bool/bool.json
+-rw-r--r--   0        0        0       19 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/bool/bool.toml
+-rw-r--r--   0        0        0       62 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/comment/at-eof.json
+-rw-r--r--   0        0        0       85 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/comment/at-eof.toml
+-rw-r--r--   0        0        0       62 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/comment/at-eof2.json
+-rw-r--r--   0        0        0       85 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/comment/at-eof2.toml
+-rw-r--r--   0        0        0      327 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/comment/everywhere.json
+-rw-r--r--   0        0        0      556 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/comment/everywhere.toml
+-rw-r--r--   0        0        0     1529 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/comment/tricky.json
+-rw-r--r--   0        0        0      385 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/comment/tricky.toml
+-rw-r--r--   0        0        0      159 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/datetime/datetime.json
+-rw-r--r--   0        0        0       58 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/datetime/datetime.toml
+-rw-r--r--   0        0        0       79 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/datetime/local-date.json
+-rw-r--r--   0        0        0       25 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/datetime/local-date.toml
+-rw-r--r--   0        0        0      157 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/datetime/local-time.json
+-rw-r--r--   0        0        0       52 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/datetime/local-time.toml
+-rw-r--r--   0        0        0      256 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/datetime/local.json
+-rw-r--r--   0        0        0       88 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/datetime/local.toml
+-rw-r--r--   0        0        0      351 2022-02-08 11:23:52.229574 tomlkit-0.9.2/tests/toml-test/tests/valid/datetime/milliseconds.json
+-rw-r--r--   0        0        0      144 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/datetime/milliseconds.toml
+-rw-r--r--   0        0        0      324 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/datetime/timezone.json
+-rw-r--r--   0        0        0      134 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/datetime/timezone.toml
+-rw-r--r--   0        0        0        3 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/empty-file.json
+-rw-r--r--   0        0        0        0 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/empty-file.toml
+-rw-r--r--   0        0        0      402 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/example.json
+-rw-r--r--   0        0        0       91 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/example.toml
+-rw-r--r--   0        0        0      489 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/float/exponent.json
+-rw-r--r--   0        0        0      114 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/float/exponent.toml
+-rw-r--r--   0        0        0      245 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/float/float.json
+-rw-r--r--   0        0        0       59 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/float/float.toml
+-rw-r--r--   0        0        0      374 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/float/inf-and-nan.json
+-rw-r--r--   0        0        0      232 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/float/inf-and-nan.toml
+-rw-r--r--   0        0        0      153 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/float/long.json
+-rw-r--r--   0        0        0       58 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/float/long.toml
+-rw-r--r--   0        0        0      196 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/float/underscore.json
+-rw-r--r--   0        0        0       56 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/float/underscore.toml
+-rw-r--r--   0        0        0      374 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/float/zero.json
+-rw-r--r--   0        0        0       68 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/float/zero.toml
+-rw-r--r--   0        0        0      206 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/implicit-and-explicit-after.json
+-rw-r--r--   0        0        0       37 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/implicit-and-explicit-after.toml
+-rw-r--r--   0        0        0      206 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/implicit-and-explicit-before.json
+-rw-r--r--   0        0        0       37 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/implicit-and-explicit-before.toml
+-rw-r--r--   0        0        0      138 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/implicit-groups.json
+-rw-r--r--   0        0        0       20 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/implicit-groups.toml
+-rw-r--r--   0        0        0      551 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/inline-table/array.json
+-rw-r--r--   0        0        0      170 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/inline-table/array.toml
+-rw-r--r--   0        0        0      141 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/inline-table/bool.json
+-rw-r--r--   0        0        0       26 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/inline-table/bool.toml
+-rw-r--r--   0        0        0      371 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/inline-table/empty.json
+-rw-r--r--   0        0        0      157 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/inline-table/empty.toml
+-rw-r--r--   0        0        0      251 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/inline-table/end-in-bool.json
+-rw-r--r--   0        0        0       70 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/inline-table/end-in-bool.toml
+-rw-r--r--   0        0        0      652 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/inline-table/inline-table.json
+-rw-r--r--   0        0        0      157 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/inline-table/inline-table.toml
+-rw-r--r--   0        0        0     2071 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/inline-table/key-dotted.json
+-rw-r--r--   0        0        0      308 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/inline-table/key-dotted.toml
+-rw-r--r--   0        0        0      304 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/inline-table/multiline.json
+-rw-r--r--   0        0        0       88 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/inline-table/multiline.toml
+-rw-r--r--   0        0        0      855 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/inline-table/nest.json
+-rw-r--r--   0        0        0      372 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/inline-table/nest.toml
+-rw-r--r--   0        0        0      247 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/integer/integer.json
+-rw-r--r--   0        0        0       53 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/integer/integer.toml
+-rw-r--r--   0        0        0      557 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/integer/literals.json
+-rw-r--r--   0        0        0      151 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/integer/literals.toml
+-rw-r--r--   0        0        0      168 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/integer/long.json
+-rw-r--r--   0        0        0       69 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/integer/long.toml
+-rw-r--r--   0        0        0      120 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/integer/underscore.json
+-rw-r--r--   0        0        0       25 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/integer/underscore.toml
+-rw-r--r--   0        0        0      663 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/integer/zero.json
+-rw-r--r--   0        0        0      122 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/integer/zero.toml
+-rw-r--r--   0        0        0      664 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/key/alphanum.json
+-rw-r--r--   0        0        0      173 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/key/alphanum.toml
+-rw-r--r--   0        0        0      633 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/key/case-sensitive.json
+-rw-r--r--   0        0        0      203 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/key/case-sensitive.toml
+-rw-r--r--   0        0        0     2017 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/key/dotted.json
+-rw-r--r--   0        0        0      535 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/key/dotted.toml
+-rw-r--r--   0        0        0       59 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/key/empty.json
+-rw-r--r--   0        0        0       13 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/key/empty.toml
+-rw-r--r--   0        0        0       63 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/key/equals-nospace.json
+-rw-r--r--   0        0        0       10 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/key/equals-nospace.toml
+-rw-r--r--   0        0        0      359 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/key/escapes.json
+-rw-r--r--   0        0        0      149 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/key/escapes.toml
+-rw-r--r--   0        0        0       78 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/key/numeric-dotted.json
+-rw-r--r--   0        0        0        8 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/key/numeric-dotted.toml
+-rw-r--r--   0        0        0       57 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/key/numeric.json
+-rw-r--r--   0        0        0        6 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/key/numeric.toml
+-rw-r--r--   0        0        0      476 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/key/quoted-dots.json
+-rw-r--r--   0        0        0      112 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/key/quoted-dots.toml
+-rw-r--r--   0        0        0       59 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/key/space.json
+-rw-r--r--   0        0        0       10 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/key/space.toml
+-rw-r--r--   0        0        0      106 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/key/special-chars.json
+-rw-r--r--   0        0        0       42 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/key/special-chars.toml
+-rw-r--r--   0        0        0      261 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/key/special-word.json
+-rw-r--r--   0        0        0       73 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/key/special-word.toml
+-rw-r--r--   0        0        0      121 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/newline-crlf.json
+-rw-r--r--   0        0        0       30 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/newline-crlf.toml
+-rw-r--r--   0        0        0      120 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/newline-lf.json
+-rw-r--r--   0        0        0       27 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/newline-lf.toml
+-rw-r--r--   0        0        0     1611 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/spec-example-1-compact.json
+-rw-r--r--   0        0        0      376 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/spec-example-1-compact.toml
+-rw-r--r--   0        0        0     1611 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/spec-example-1.json
+-rw-r--r--   0        0        0      559 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/spec-example-1.toml
+-rw-r--r--   0        0        0       65 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/double-quote-escape.json
+-rw-r--r--   0        0        0       17 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/double-quote-escape.toml
+-rw-r--r--   0        0        0       60 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/empty.json
+-rw-r--r--   0        0        0       12 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/empty.toml
+-rw-r--r--   0        0        0      621 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/escape-tricky.json
+-rw-r--r--   0        0        0      328 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/escape-tricky.toml
+-rw-r--r--   0        0        0       65 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/escaped-escape.json
+-rw-r--r--   0        0        0       17 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/escaped-escape.toml
+-rw-r--r--   0        0        0     1353 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/escapes.json
+-rw-r--r--   0        0        0      771 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/escapes.toml
+-rw-r--r--   0        0        0     1071 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/multiline-json
+-rw-r--r--   0        0        0      736 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/multiline-quotes.json
+-rw-r--r--   0        0        0      448 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/multiline-quotes.toml
+-rw-r--r--   0        0        0      719 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/multiline-toml
+-rw-r--r--   0        0        0      337 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/nl.json
+-rw-r--r--   0        0        0      115 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/nl.toml
+-rw-r--r--   0        0        0      323 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/raw-multiline.json
+-rw-r--r--   0        0        0      195 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/raw-multiline.toml
+-rw-r--r--   0        0        0      699 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/raw.json
+-rw-r--r--   0        0        0      373 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/raw.toml
+-rw-r--r--   0        0        0       95 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/simple.json
+-rw-r--r--   0        0        0       47 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/simple.toml
+-rw-r--r--   0        0        0      123 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/unicode-escape.json
+-rw-r--r--   0        0        0       42 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/unicode-escape.toml
+-rw-r--r--   0        0        0       62 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/unicode-literal.json
+-rw-r--r--   0        0        0       14 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/unicode-literal.toml
+-rw-r--r--   0        0        0      183 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/with-pound.json
+-rw-r--r--   0        0        0      113 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/string/with-pound.toml
+-rw-r--r--   0        0        0      147 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/array-implicit.json
+-rw-r--r--   0        0        0       37 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/array-implicit.toml
+-rw-r--r--   0        0        0      551 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/array-many.json
+-rw-r--r--   0        0        0      163 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/array-many.toml
+-rw-r--r--   0        0        0      754 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/array-nest.json
+-rw-r--r--   0        0        0      262 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/array-nest.toml
+-rw-r--r--   0        0        0      202 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/array-one.json
+-rw-r--r--   0        0        0       58 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/array-one.toml
+-rw-r--r--   0        0        0      339 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/array-table-array.json
+-rw-r--r--   0        0        0      108 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/array-table-array.toml
+-rw-r--r--   0        0        0       14 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/empty.json
+-rw-r--r--   0        0        0        4 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/empty.toml
+-rw-r--r--   0        0        0       58 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/keyword.json
+-rw-r--r--   0        0        0       32 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/keyword.toml
+-rw-r--r--   0        0        0      274 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/names.json
+-rw-r--r--   0        0        0       90 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/names.toml
+-rw-r--r--   0        0        0       18 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/no-eol.json
+-rw-r--r--   0        0        0        8 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/no-eol.toml
+-rw-r--r--   0        0        0       29 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/sub-empty.json
+-rw-r--r--   0        0        0       10 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/sub-empty.toml
+-rw-r--r--   0        0        0       22 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/whitespace.json
+-rw-r--r--   0        0        0       14 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/whitespace.toml
+-rw-r--r--   0        0        0      142 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/with-literal-string.json
+-rw-r--r--   0        0        0       41 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/with-literal-string.toml
+-rw-r--r--   0        0        0       92 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/with-pound.json
+-rw-r--r--   0        0        0       26 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/with-pound.toml
+-rw-r--r--   0        0        0      138 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/with-single-quotes.json
+-rw-r--r--   0        0        0       37 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/with-single-quotes.toml
+-rw-r--r--   0        0        0       71 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/without-super.json
+-rw-r--r--   0        0        0      120 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/tests/valid/table/without-super.toml
+-rw-r--r--   0        0        0     3162 2022-02-08 11:23:52.233574 tomlkit-0.9.2/tests/toml-test/toml.go
+-rw-r--r--   0        0        0      952 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tomlkit/__init__.py
+-rw-r--r--   0        0        0      527 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tomlkit/_compat.py
+-rw-r--r--   0        0        0     3533 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tomlkit/_utils.py
+-rw-r--r--   0        0        0     6137 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tomlkit/api.py
+-rw-r--r--   0        0        0    27993 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tomlkit/container.py
+-rw-r--r--   0        0        0     5064 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tomlkit/exceptions.py
+-rw-r--r--   0        0        0    42524 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tomlkit/items.py
+-rw-r--r--   0        0        0    36938 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tomlkit/parser.py
+-rw-r--r--   0        0        0        0 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tomlkit/py.typed
+-rw-r--r--   0        0        0     4920 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tomlkit/source.py
+-rw-r--r--   0        0        0     1498 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tomlkit/toml_char.py
+-rw-r--r--   0        0        0      103 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tomlkit/toml_document.py
+-rw-r--r--   0        0        0      668 2022-02-08 11:23:51.393533 tomlkit-0.9.2/tomlkit/toml_file.py
+-rw-r--r--   0        0        0     2574 2022-02-08 11:24:06.798769 tomlkit-0.9.2/setup.py
+-rw-r--r--   0        0        0     2657 2022-02-08 11:24:06.799511 tomlkit-0.9.2/PKG-INFO
```

### Comparing `tomlkit-0.9.1/LICENSE` & `tomlkit-0.9.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/README.md` & `tomlkit-0.9.2/README.md`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/pyproject.toml` & `tomlkit-0.9.2/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tomlkit"
-version = "0.9.1"
+version = "0.9.2"
 description = "Style preserving TOML library"
 authors = ["Sébastien Eustace <sebastien@eustace.io>"]
 license = "MIT"
 
 readme = "README.md"
 
 homepage = "https://github.com/sdispater/tomlkit"
```

### Comparing `tomlkit-0.9.1/tests/conftest.py` & `tomlkit-0.9.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/examples/0.5.0.toml` & `tomlkit-0.9.2/tests/examples/0.5.0.toml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/examples/example.toml` & `tomlkit-0.9.2/tests/examples/example.toml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/examples/hard.toml` & `tomlkit-0.9.2/tests/examples/hard.toml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/examples/json/0.5.0.json` & `tomlkit-0.9.2/tests/examples/json/0.5.0.json`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/examples/json/pyproject.json` & `tomlkit-0.9.2/tests/examples/json/pyproject.json`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/examples/pyproject.toml` & `tomlkit-0.9.2/tests/examples/pyproject.toml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/examples/test.toml` & `tomlkit-0.9.2/tests/examples/test.toml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/test_api.py` & `tomlkit-0.9.2/tests/test_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -378,7 +378,17 @@
         "false{a=1}",
     ],
 )
 def test_value_rejects_values_with_appendage(raw):
     """Values that appear valid at the beginning but leave chars unparsed are rejected."""
     with pytest.raises(tomlkit.exceptions.ParseError):
         tomlkit.value(raw)
+
+
+def test_create_super_table_with_table():
+    data = {"foo": {"bar": {"a": 1}}}
+    assert dumps(data) == "[foo.bar]\na = 1\n"
+
+
+def test_create_super_table_with_aot():
+    data = {"foo": {"bar": [{"a": 1}]}}
+    assert dumps(data) == "[[foo.bar]]\na = 1\n"
```

### Comparing `tomlkit-0.9.1/tests/test_build.py` & `tomlkit-0.9.2/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/test_items.py` & `tomlkit-0.9.2/tests/test_items.py`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/test_parser.py` & `tomlkit-0.9.2/tests/test_parser.py`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/test_toml_document.py` & `tomlkit-0.9.2/tests/test_toml_document.py`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/test_toml_file.py` & `tomlkit-0.9.2/tests/test_toml_file.py`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/test_toml_spec_tests.py` & `tomlkit-0.9.2/tests/test_toml_spec_tests.py`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/test_toml_tests.py` & `tomlkit-0.9.2/tests/test_toml_tests.py`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/test_utils.py` & `tomlkit-0.9.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-spec-tests/LICENSE` & `tomlkit-0.9.2/tests/toml-spec-tests/LICENSE`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-spec-tests/README.md` & `tomlkit-0.9.2/tests/toml-spec-tests/README.md`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-spec-tests/values/qa-key-literal-40kb.toml` & `tomlkit-0.9.2/tests/toml-spec-tests/values/qa-key-literal-40kb.toml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-spec-tests/values/qa-key-literal-40kb.yaml` & `tomlkit-0.9.2/tests/toml-spec-tests/values/qa-key-literal-40kb.yaml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-spec-tests/values/qa-key-string-40kb.toml` & `tomlkit-0.9.2/tests/toml-spec-tests/values/qa-key-string-40kb.toml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-spec-tests/values/qa-key-string-40kb.yaml` & `tomlkit-0.9.2/tests/toml-spec-tests/values/qa-key-string-40kb.yaml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-spec-tests/values/qa-scalar-literal-40kb.toml` & `tomlkit-0.9.2/tests/toml-spec-tests/values/qa-scalar-literal-40kb.toml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-spec-tests/values/qa-scalar-literal-40kb.yaml` & `tomlkit-0.9.2/tests/toml-spec-tests/values/qa-scalar-literal-40kb.yaml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-spec-tests/values/qa-scalar-literal-multiline-40kb.toml` & `tomlkit-0.9.2/tests/toml-spec-tests/values/qa-scalar-literal-multiline-40kb.toml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-spec-tests/values/qa-scalar-literal-multiline-40kb.yaml` & `tomlkit-0.9.2/tests/toml-spec-tests/values/qa-scalar-literal-multiline-40kb.yaml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-spec-tests/values/qa-scalar-string-40kb.toml` & `tomlkit-0.9.2/tests/toml-spec-tests/values/qa-scalar-string-40kb.toml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-spec-tests/values/qa-scalar-string-40kb.yaml` & `tomlkit-0.9.2/tests/toml-spec-tests/values/qa-scalar-string-40kb.yaml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-spec-tests/values/qa-scalar-string-multiline-40kb.toml` & `tomlkit-0.9.2/tests/toml-spec-tests/values/qa-scalar-string-multiline-40kb.toml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-spec-tests/values/qa-scalar-string-multiline-40kb.yaml` & `tomlkit-0.9.2/tests/toml-spec-tests/values/qa-scalar-string-multiline-40kb.yaml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-spec-tests/values/qa-table-inline-1000.toml` & `tomlkit-0.9.2/tests/toml-spec-tests/values/qa-table-inline-1000.toml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-spec-tests/values/qa-table-inline-1000.yaml` & `tomlkit-0.9.2/tests/toml-spec-tests/values/qa-table-inline-1000.yaml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-spec-tests/values/spec-readme-example.toml` & `tomlkit-0.9.2/tests/toml-spec-tests/values/spec-readme-example.toml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/.github/workflows/test.yml` & `tomlkit-0.9.2/tests/toml-test/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/COPYING` & `tomlkit-0.9.2/tests/toml-test/COPYING`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/README.md` & `tomlkit-0.9.2/tests/toml-test/README.md`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/cmd/toml-test/main.go` & `tomlkit-0.9.2/tests/toml-test/cmd/toml-test/main.go`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/cmd/toml-test/usage.go` & `tomlkit-0.9.2/tests/toml-test/cmd/toml-test/usage.go`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/go.sum` & `tomlkit-0.9.2/tests/toml-test/go.sum`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/json.go` & `tomlkit-0.9.2/tests/toml-test/json.go`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/runner.go` & `tomlkit-0.9.2/tests/toml-test/runner.go`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/invalid/control/control.multi` & `tomlkit-0.9.2/tests/toml-test/tests/invalid/control/control.multi`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/invalid/float/float.multi` & `tomlkit-0.9.2/tests/toml-test/tests/invalid/float/float.multi`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/invalid/integer/integer.multi` & `tomlkit-0.9.2/tests/toml-test/tests/invalid/integer/integer.multi`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/invalid/table/array-implicit.toml` & `tomlkit-0.9.2/tests/toml-test/tests/invalid/table/array-implicit.toml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/valid/array/array.json` & `tomlkit-0.9.2/tests/toml-test/tests/valid/array/array.json`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/valid/comment/everywhere.toml` & `tomlkit-0.9.2/tests/toml-test/tests/valid/comment/everywhere.toml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/valid/comment/tricky.json` & `tomlkit-0.9.2/tests/toml-test/tests/valid/comment/tricky.json`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/valid/inline-table/array.json` & `tomlkit-0.9.2/tests/toml-test/tests/valid/inline-table/array.json`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/valid/inline-table/inline-table.json` & `tomlkit-0.9.2/tests/toml-test/tests/valid/inline-table/inline-table.json`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/valid/inline-table/key-dotted.json` & `tomlkit-0.9.2/tests/toml-test/tests/valid/inline-table/key-dotted.json`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/valid/inline-table/nest.json` & `tomlkit-0.9.2/tests/toml-test/tests/valid/inline-table/nest.json`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/valid/integer/literals.json` & `tomlkit-0.9.2/tests/toml-test/tests/valid/integer/literals.json`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/valid/integer/zero.json` & `tomlkit-0.9.2/tests/toml-test/tests/valid/integer/zero.json`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/valid/key/alphanum.json` & `tomlkit-0.9.2/tests/toml-test/tests/valid/key/alphanum.json`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/valid/key/case-sensitive.json` & `tomlkit-0.9.2/tests/toml-test/tests/valid/key/case-sensitive.json`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/valid/key/dotted.json` & `tomlkit-0.9.2/tests/toml-test/tests/valid/key/dotted.json`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/valid/key/dotted.toml` & `tomlkit-0.9.2/tests/toml-test/tests/valid/key/dotted.toml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/valid/spec-example-1-compact.json` & `tomlkit-0.9.2/tests/toml-test/tests/valid/spec-example-1-compact.json`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/valid/spec-example-1.json` & `tomlkit-0.9.2/tests/toml-test/tests/valid/spec-example-1.json`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/valid/spec-example-1.toml` & `tomlkit-0.9.2/tests/toml-test/tests/valid/spec-example-1.toml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/valid/string/escape-tricky.json` & `tomlkit-0.9.2/tests/toml-test/tests/valid/string/escape-tricky.json`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/valid/string/escapes.json` & `tomlkit-0.9.2/tests/toml-test/tests/valid/string/escapes.json`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/valid/string/escapes.toml` & `tomlkit-0.9.2/tests/toml-test/tests/valid/string/escapes.toml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/valid/string/multiline-json` & `tomlkit-0.9.2/tests/toml-test/tests/valid/string/multiline-json`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/valid/string/multiline-quotes.json` & `tomlkit-0.9.2/tests/toml-test/tests/valid/string/multiline-quotes.json`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/valid/string/multiline-toml` & `tomlkit-0.9.2/tests/toml-test/tests/valid/string/multiline-toml`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/valid/string/raw.json` & `tomlkit-0.9.2/tests/toml-test/tests/valid/string/raw.json`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/valid/table/array-many.json` & `tomlkit-0.9.2/tests/toml-test/tests/valid/table/array-many.json`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/tests/valid/table/array-nest.json` & `tomlkit-0.9.2/tests/toml-test/tests/valid/table/array-nest.json`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tests/toml-test/toml.go` & `tomlkit-0.9.2/tests/toml-test/toml.go`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tomlkit/__init__.py` & `tomlkit-0.9.2/tomlkit/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 from .api import string
 from .api import table
 from .api import time
 from .api import value
 from .api import ws
 
 
-__version__ = "0.9.1"
+__version__ = "0.9.2"
 __all__ = [
     "aot",
     "array",
     "boolean",
     "comment",
     "date",
     "datetime",
```

### Comparing `tomlkit-0.9.1/tomlkit/_compat.py` & `tomlkit-0.9.2/tomlkit/_compat.py`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tomlkit/_utils.py` & `tomlkit-0.9.2/tomlkit/_utils.py`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tomlkit/api.py` & `tomlkit-0.9.2/tomlkit/api.py`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tomlkit/container.py` & `tomlkit-0.9.2/tomlkit/container.py`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tomlkit/exceptions.py` & `tomlkit-0.9.2/tomlkit/exceptions.py`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tomlkit/items.py` & `tomlkit-0.9.2/tomlkit/items.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,14 +86,22 @@
         table_constructor = InlineTable if isinstance(_parent, Array) else Table
         val = table_constructor(Container(), Trivia(), False)
         for k, v in sorted(
             value.items(),
             key=lambda i: (isinstance(i[1], dict), i[0] if _sort_keys else 1),
         ):
             val[k] = item(v, _parent=val, _sort_keys=_sort_keys)
+        only_child = len(value) == 1 and val[next(iter(value))]
+        if (
+            table_constructor is Table
+            and only_child
+            and isinstance(only_child, (AoT, Table))
+        ):
+            # The table becomes super table if the only child is a table or AoT.
+            val._is_super_table = True
 
         return val
     elif isinstance(value, (list, tuple)):
         if value and all(isinstance(v, dict) for v in value):
             a = AoT([])
             table_constructor = Table
         else:
```

### Comparing `tomlkit-0.9.1/tomlkit/parser.py` & `tomlkit-0.9.2/tomlkit/parser.py`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tomlkit/source.py` & `tomlkit-0.9.2/tomlkit/source.py`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tomlkit/toml_char.py` & `tomlkit-0.9.2/tomlkit/toml_char.py`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/tomlkit/toml_file.py` & `tomlkit-0.9.2/tomlkit/toml_file.py`

 * *Files identical despite different names*

### Comparing `tomlkit-0.9.1/setup.py` & `tomlkit-0.9.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 ['tomlkit']
 
 package_data = \
 {'': ['*']}
 
 setup_kwargs = {
     'name': 'tomlkit',
-    'version': '0.9.1',
+    'version': '0.9.2',
     'description': 'Style preserving TOML library',
     'long_description': '[github_release]: https://img.shields.io/github/release/sdispater/tomlkit.svg?logo=github&logoColor=white\n[pypi_version]: https://img.shields.io/pypi/v/tomlkit.svg?logo=python&logoColor=white\n[python_versions]: https://img.shields.io/pypi/pyversions/tomlkit.svg?logo=python&logoColor=white\n[github_license]: https://img.shields.io/github/license/sdispater/tomlkit.svg?logo=github&logoColor=white\n[github_action]: https://github.com/sdispater/tomlkit/actions/workflows/tests.yml/badge.svg\n\n[![GitHub Release][github_release]](https://github.com/sdispater/tomlkit/releases/)\n[![PyPI Version][pypi_version]](https://pypi.org/project/tomlkit/)\n[![Python Versions][python_versions]](https://pypi.org/project/tomlkit/)\n[![License][github_license]](https://github.com/sdispater/tomlkit/blob/master/LICENSE)\n<br>\n[![Tests][github_action]](https://github.com/sdispater/tomlkit/actions/workflows/tests.yml)\n\n# TOML Kit - Style-preserving TOML library for Python\n\nTOML Kit is a **1.0.0-compliant** [TOML](https://toml.io/) library.\n\nIt includes a parser that preserves all comments, indentations, whitespace and internal element ordering,\nand makes them accessible and editable via an intuitive API.\n\nYou can also create new TOML documents from scratch using the provided helpers.\n\nPart of the implementation as been adapted, improved and fixed from [Molten](https://github.com/LeopoldArkham/Molten).\n\n## Usage\n\nSee the [documentation](docs/quickstart.rst) for more information.\n\n## Installation\n\nIf you are using [Poetry](https://poetry.eustace.io),\nadd `tomlkit` to your `pyproject.toml` file by using:\n\n```bash\npoetry add tomlkit\n```\n\nIf not, you can use `pip`:\n\n```bash\npip install tomlkit\n```\n\n## Running tests\n\nPlease clone the repo with submodules with the following command\n`git clone --recurse-submodules https://github.com/sdispater/tomlkit.git`.\nWe need the submodule - `toml-test` for running the tests.\n\nYou can run the tests with `poetry run pytest -q tests`\n',
     'author': 'Sébastien Eustace',
     'author_email': 'sebastien@eustace.io',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/sdispater/tomlkit',
```

### Comparing `tomlkit-0.9.1/PKG-INFO` & `tomlkit-0.9.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tomlkit
-Version: 0.9.1
+Version: 0.9.2
 Summary: Style preserving TOML library
 Home-page: https://github.com/sdispater/tomlkit
 License: MIT
 Author: Sébastien Eustace
 Author-email: sebastien@eustace.io
 Requires-Python: >=3.6,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

