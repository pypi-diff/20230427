# Comparing `tmp/robotcode_language_server-0.34.1.tar.gz` & `tmp/robotcode_language_server-0.35.0.tar.gz`

## Comparing `robotcode_language_server-0.34.1.tar` & `robotcode_language_server-0.35.0.tar`

### file list

```diff
@@ -1,89 +1,89 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/__init__.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/__main__.py
--rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/__version__.py
--rw-r--r--   0        0        0     7631 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/cli.py
--rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/py.typed
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/__init__.py
--rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/decorators.py
--rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/has_extend_capabilities.py
--rw-r--r--   0        0        0   233349 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/lsp_types.py
--rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/protocol.py
--rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/server.py
--rw-r--r--   0        0        0     9556 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/text_document.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/__init__.py
--rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/code_action.py
--rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/code_lens.py
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/commands.py
--rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/completion.py
--rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/declaration.py
--rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/definition.py
--rw-r--r--   0        0        0    21125 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/diagnostics.py
--rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/document_highlight.py
--rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/document_symbols.py
--rw-r--r--   0        0        0    14891 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/documents.py
--rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/folding_range.py
--rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/formatting.py
--rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/hover.py
--rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/implementation.py
--rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/inlay_hint.py
--rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/inline_value.py
--rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/linked_editing_ranges.py
--rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/protocol_part.py
--rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/references.py
--rw-r--r--   0        0        0     5798 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/rename.py
--rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/selection_range.py
--rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/semantic_tokens.py
--rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/signature_help.py
--rw-r--r--   0        0        0     9358 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/window.py
--rw-r--r--   0        0        0    19025 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/workspace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/__init__.py
--rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/configuration.py
--rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/languages.py
--rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/protocol.py
--rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/server.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/diagnostics/__init__.py
--rw-r--r--   0        0        0    38217 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
--rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/diagnostics/entities.py
--rw-r--r--   0        0        0    54371 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
--rw-r--r--   0        0        0    63728 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
--rw-r--r--   0        0        0    83656 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/diagnostics/namespace.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/__init__.py
--rw-r--r--   0        0        0    15251 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
--rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
--rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/codelens.py
--rw-r--r--   0        0        0    80273 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/completion.py
--rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/debugging_utils.py
--rw-r--r--   0        0        0    16885 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/diagnostics.py
--rw-r--r--   0        0        0    14470 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/discovering.py
--rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/document_highlight.py
--rw-r--r--   0        0        0     9890 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/document_symbols.py
--rw-r--r--   0        0        0    19277 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/documents_cache.py
--rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/folding_range.py
--rw-r--r--   0        0        0     7679 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/formatting.py
--rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/goto.py
--rw-r--r--   0        0        0    23517 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/hover.py
--rw-r--r--   0        0        0     8890 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/inlay_hint.py
--rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/inline_value.py
--rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/model_helper.py
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/protocol_part.py
--rw-r--r--   0        0        0    19656 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/references.py
--rw-r--r--   0        0        0    24970 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/rename.py
--rw-r--r--   0        0        0     6317 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
--rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/robot_workspace.py
--rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/selection_range.py
--rw-r--r--   0        0        0    40456 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
--rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/signature_help.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/utils/__init__.py
--rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/utils/_variables.py
--rw-r--r--   0        0        0     7975 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/utils/ast_utils.py
--rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/utils/async_ast.py
--rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/utils/markdownformatter.py
--rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/utils/match.py
--rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/utils/robot_path.py
--rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/utils/variables.py
--rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/utils/version.py
--rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/.gitignore
--rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/LICENSE.txt
--rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/README.md
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/pyproject.toml
--rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 robotcode_language_server-0.34.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/__init__.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/__main__.py
+-rw-r--r--   0        0        0       23 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/__version__.py
+-rw-r--r--   0        0        0     7631 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/cli.py
+-rw-r--r--   0        0        0       27 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/py.typed
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/__init__.py
+-rw-r--r--   0        0        0     2563 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/decorators.py
+-rw-r--r--   0        0        0      276 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/has_extend_capabilities.py
+-rw-r--r--   0        0        0   233349 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/lsp_types.py
+-rw-r--r--   0        0        0    11513 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/protocol.py
+-rw-r--r--   0        0        0      781 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/server.py
+-rw-r--r--   0        0        0     9556 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/text_document.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/__init__.py
+-rw-r--r--   0        0        0     4429 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/code_action.py
+-rw-r--r--   0        0        0     4257 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/code_lens.py
+-rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/commands.py
+-rw-r--r--   0        0        0     6224 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/completion.py
+-rw-r--r--   0        0        0     4666 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/declaration.py
+-rw-r--r--   0        0        0     4668 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/definition.py
+-rw-r--r--   0        0        0    21125 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/diagnostics.py
+-rw-r--r--   0        0        0     2707 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/document_highlight.py
+-rw-r--r--   0        0        0     5955 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/document_symbols.py
+-rw-r--r--   0        0        0    14891 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/documents.py
+-rw-r--r--   0        0        0     2802 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/folding_range.py
+-rw-r--r--   0        0        0     4417 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/formatting.py
+-rw-r--r--   0        0        0     2694 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/hover.py
+-rw-r--r--   0        0        0     4669 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/implementation.py
+-rw-r--r--   0        0        0     3876 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3675 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/inline_value.py
+-rw-r--r--   0        0        0     2748 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py
+-rw-r--r--   0        0        0      424 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/protocol_part.py
+-rw-r--r--   0        0        0     2860 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/references.py
+-rw-r--r--   0        0        0     5798 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/rename.py
+-rw-r--r--   0        0        0     2909 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/selection_range.py
+-rw-r--r--   0        0        0     6981 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/semantic_tokens.py
+-rw-r--r--   0        0        0     3647 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/signature_help.py
+-rw-r--r--   0        0        0     9358 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/window.py
+-rw-r--r--   0        0        0    19025 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/workspace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/__init__.py
+-rw-r--r--   0        0        0     3907 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/configuration.py
+-rw-r--r--   0        0        0      350 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/languages.py
+-rw-r--r--   0        0        0     8115 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/protocol.py
+-rw-r--r--   0        0        0      311 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/server.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/diagnostics/__init__.py
+-rw-r--r--   0        0        0    38217 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py
+-rw-r--r--   0        0        0     7957 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/diagnostics/entities.py
+-rw-r--r--   0        0        0    54371 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py
+-rw-r--r--   0        0        0    63728 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py
+-rw-r--r--   0        0        0    83656 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/__init__.py
+-rw-r--r--   0        0        0    15251 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py
+-rw-r--r--   0        0        0     7169 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py
+-rw-r--r--   0        0        0     6688 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/codelens.py
+-rw-r--r--   0        0        0    80273 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/completion.py
+-rw-r--r--   0        0        0     3719 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py
+-rw-r--r--   0        0        0    16885 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/diagnostics.py
+-rw-r--r--   0        0        0    14470 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/discovering.py
+-rw-r--r--   0        0        0     2647 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/document_highlight.py
+-rw-r--r--   0        0        0     9890 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/document_symbols.py
+-rw-r--r--   0        0        0    19277 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/documents_cache.py
+-rw-r--r--   0        0        0     4402 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/folding_range.py
+-rw-r--r--   0        0        0     7679 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/formatting.py
+-rw-r--r--   0        0        0    26526 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/goto.py
+-rw-r--r--   0        0        0    23517 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/hover.py
+-rw-r--r--   0        0        0     8890 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py
+-rw-r--r--   0        0        0     3438 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/inline_value.py
+-rw-r--r--   0        0        0    24273 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/model_helper.py
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/protocol_part.py
+-rw-r--r--   0        0        0    19656 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/references.py
+-rw-r--r--   0        0        0    24970 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/rename.py
+-rw-r--r--   0        0        0     6317 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py
+-rw-r--r--   0        0        0     8517 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py
+-rw-r--r--   0        0        0     2742 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/selection_range.py
+-rw-r--r--   0        0        0    40456 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py
+-rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/signature_help.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/__init__.py
+-rw-r--r--   0        0        0     1722 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/_variables.py
+-rw-r--r--   0        0        0     7975 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/ast_utils.py
+-rw-r--r--   0        0        0     3163 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/async_ast.py
+-rw-r--r--   0        0        0    11653 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py
+-rw-r--r--   0        0        0      268 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/match.py
+-rw-r--r--   0        0        0     1739 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/robot_path.py
+-rw-r--r--   0        0        0     1357 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/variables.py
+-rw-r--r--   0        0        0      482 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/version.py
+-rw-r--r--   0        0        0     4277 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/.gitignore
+-rw-r--r--   0        0        0    10280 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/LICENSE.txt
+-rw-r--r--   0        0        0      765 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/README.md
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/pyproject.toml
+-rw-r--r--   0        0        0     2152 2020-02-02 00:00:00.000000 robotcode_language_server-0.35.0/PKG-INFO
```

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/__main__.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/__main__.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/cli.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/cli.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/decorators.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/decorators.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/lsp_types.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/lsp_types.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/protocol.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/server.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/server.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/text_document.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/text_document.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/code_action.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/code_action.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/code_lens.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/code_lens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/commands.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/commands.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/completion.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/completion.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/declaration.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/declaration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/definition.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/definition.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/diagnostics.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/document_highlight.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/document_symbols.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/documents.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/documents.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/folding_range.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/formatting.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/hover.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/implementation.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/implementation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/inlay_hint.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/inline_value.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/linked_editing_ranges.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/linked_editing_ranges.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/references.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/rename.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/selection_range.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/semantic_tokens.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/signature_help.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/window.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/window.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/common/parts/workspace.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/common/parts/workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/configuration.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/configuration.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/protocol.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/protocol.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/diagnostics/analyzer.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/diagnostics/analyzer.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/diagnostics/entities.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/diagnostics/entities.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/diagnostics/imports_manager.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/diagnostics/library_doc.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/diagnostics/library_doc.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/diagnostics/namespace.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/diagnostics/namespace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/code_action_documentation.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/code_action_documentation.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/code_action_fixes.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/code_action_fixes.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/codelens.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/codelens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/completion.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/completion.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/debugging_utils.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/debugging_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/diagnostics.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/discovering.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/discovering.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/document_highlight.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/document_highlight.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/document_symbols.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/document_symbols.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/documents_cache.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/documents_cache.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/folding_range.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/folding_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/formatting.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/formatting.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/goto.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/goto.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/hover.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/hover.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/inlay_hint.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/inlay_hint.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/inline_value.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/inline_value.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/model_helper.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/model_helper.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/references.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/references.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/rename.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/rename.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/robocop_diagnostics.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/robot_workspace.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/robot_workspace.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/selection_range.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/selection_range.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/semantic_tokens.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/semantic_tokens.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/parts/signature_help.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/parts/signature_help.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/utils/_variables.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/_variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/utils/ast_utils.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/ast_utils.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/utils/async_ast.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/async_ast.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/utils/markdownformatter.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/markdownformatter.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/utils/robot_path.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/robot_path.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/src/robotcode/language_server/robotframework/utils/variables.py` & `robotcode_language_server-0.35.0/src/robotcode/language_server/robotframework/utils/variables.py`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/.gitignore` & `robotcode_language_server-0.35.0/.gitignore`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/LICENSE.txt` & `robotcode_language_server-0.35.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/README.md` & `robotcode_language_server-0.35.0/README.md`

 * *Files identical despite different names*

### Comparing `robotcode_language_server-0.34.1/pyproject.toml` & `robotcode_language_server-0.35.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,15 @@
   "Programming Language :: Python :: Implementation :: PyPy",
   "Operating System :: OS Independent",
   "Topic :: Utilities",
   "Typing :: Typed",
   "Framework :: Robot Framework",
   "Framework :: Robot Framework :: Tool",
 ]
-dependencies = ["robotframework>=4.1.0", "robotcode-jsonrpc2==0.34.1"]
+dependencies = ["robotframework>=4.1.0", "robotcode-jsonrpc2==0.35.0"]
 dynamic = ["version"]
 
 [project.scripts]
 'robotcode.language_server' = 'robotcode.language_server.__main__:main'
 
 [project.urls]
 Homepage = "https://robotcode.io"
```

### Comparing `robotcode_language_server-0.34.1/PKG-INFO` & `robotcode_language_server-0.35.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robotcode-language-server
-Version: 0.34.1
+Version: 0.35.0
 Summary: RobotCode Language Server for Robot Framework
 Project-URL: Homepage, https://robotcode.io
 Project-URL: Donate, https://github.com/sponsors/d-biehl
 Project-URL: Documentation, https://github.com/d-biehl/robotcode#readme
 Project-URL: Changelog, https://github.com/d-biehl/robotcode/blob/main/CHANGELOG.md
 Project-URL: Issues, https://github.com/d-biehl/robotcode/issues
 Project-URL: Source, https://github.com/d-biehl/robotcode
@@ -21,15 +21,15 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Utilities
 Classifier: Typing :: Typed
 Requires-Python: >=3.8
-Requires-Dist: robotcode-jsonrpc2==0.34.1
+Requires-Dist: robotcode-jsonrpc2==0.35.0
 Requires-Dist: robotframework>=4.1.0
 Description-Content-Type: text/markdown
 
 # robotcode-language-server
 
 [![PyPI - Version](https://img.shields.io/pypi/v/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
 [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/robotcode-language-server.svg)](https://pypi.org/project/robotcode-language-server)
```

