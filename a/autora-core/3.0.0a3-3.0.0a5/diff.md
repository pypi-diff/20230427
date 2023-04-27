# Comparing `tmp/autora-core-3.0.0a3.tar.gz` & `tmp/autora-core-3.0.0a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autora-core-3.0.0a3.tar", last modified: Wed Apr 26 21:15:31 2023, max compression
+gzip compressed data, was "autora-core-3.0.0a5.tar", last modified: Thu Apr 27 19:23:16 2023, max compression
```

## Comparing `autora-core-3.0.0a3.tar` & `autora-core-3.0.0a5.tar`

### file list

```diff
@@ -1,110 +1,101 @@
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.107550 autora-core-3.0.0a3/
--rw-r--r--   0 jholla10   (503) staff       (20)      291 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.editorconfig
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.088436 autora-core-3.0.0a3/.github/
--rw-r--r--   0 jholla10   (503) staff       (20)      363 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.github/dependabot.yml
--rw-r--r--   0 jholla10   (503) staff       (20)     2095 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.github/pull_request_template.md
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.089787 autora-core-3.0.0a3/.github/workflows/
--rw-r--r--   0 jholla10   (503) staff       (20)      426 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.github/workflows/publish-documentation-gh-pages.yml
--rw-r--r--   0 jholla10   (503) staff       (20)     1503 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.github/workflows/publish-package-anaconda-org.yml
--rw-r--r--   0 jholla10   (503) staff       (20)      712 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.github/workflows/publish-package-pypi.yml
--rw-r--r--   0 jholla10   (503) staff       (20)      548 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.github/workflows/test-conda-build.yml
--rw-r--r--   0 jholla10   (503) staff       (20)      440 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.github/workflows/test-poetry-build.yml
--rw-r--r--   0 jholla10   (503) staff       (20)      845 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.github/workflows/test-pre-commit-hooks.yml
--rw-r--r--   0 jholla10   (503) staff       (20)      775 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.github/workflows/test-pytest.yml
--rw-r--r--   0 jholla10   (503) staff       (20)     1009 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.gitignore
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.091087 autora-core-3.0.0a3/.idea/
--rw-r--r--   0 jholla10   (503) staff       (20)      176 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.idea/.gitignore
--rw-r--r--   0 jholla10   (503) staff       (20)     1654 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.idea/autora-core.iml
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.091248 autora-core-3.0.0a3/.idea/codeStyles/
--rw-r--r--   0 jholla10   (503) staff       (20)      149 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.idea/codeStyles/codeStyleConfig.xml
--rw-r--r--   0 jholla10   (503) staff       (20)      159 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.idea/encodings.xml
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.091795 autora-core-3.0.0a3/.idea/inspectionProfiles/
--rw-r--r--   0 jholla10   (503) staff       (20)      716 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.idea/inspectionProfiles/Project_Default.xml
--rw-r--r--   0 jholla10   (503) staff       (20)      228 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.idea/inspectionProfiles/profiles_settings.xml
--rw-r--r--   0 jholla10   (503) staff       (20)      310 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.idea/misc.xml
--rw-r--r--   0 jholla10   (503) staff       (20)      264 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.idea/modules.xml
--rw-r--r--   0 jholla10   (503) staff       (20)      186 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.idea/other.xml
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.091960 autora-core-3.0.0a3/.idea/runConfigurations/
--rw-r--r--   0 jholla10   (503) staff       (20)     1011 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.idea/runConfigurations/pytest_in_tests.xml
--rw-r--r--   0 jholla10   (503) staff       (20)      180 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.idea/vcs.xml
--rw-r--r--   0 jholla10   (503) staff       (20)      796 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.pre-commit-config.yaml
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.092572 autora-core-3.0.0a3/.vscode/
--rw-r--r--   0 jholla10   (503) staff       (20)        0 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.vscode/.gitignore
--rw-r--r--   0 jholla10   (503) staff       (20)      112 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.vscode/extensions.json
--rw-r--r--   0 jholla10   (503) staff       (20)      495 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/.vscode/launch.json
--rw-r--r--   0 jholla10   (503) staff       (20)     1100 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/LICENSE.md
--rw-r--r--   0 jholla10   (503) staff       (20)    19467 2023-04-26 21:15:31.107296 autora-core-3.0.0a3/PKG-INFO
--rw-r--r--   0 jholla10   (503) staff       (20)    18766 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/README.md
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.083509 autora-core-3.0.0a3/conda/
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.093117 autora-core-3.0.0a3/conda/autora/
--rw-r--r--   0 jholla10   (503) staff       (20)     1315 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/conda/autora/meta.yaml
--rw-r--r--   0 jholla10   (503) staff       (20)       26 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/conda/autora/run_test.sh
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.084007 autora-core-3.0.0a3/docs/
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.093351 autora-core-3.0.0a3/docs/cycle/
--rw-r--r--   0 jholla10   (503) staff       (20)   148488 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/docs/cycle/simple_cycle_bms_model_poppernet.ipynb
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.093795 autora-core-3.0.0a3/docs/experimentalists/
--rw-r--r--   0 jholla10   (503) staff       (20)     2779 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/docs/experimentalists/overview.md
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.084264 autora-core-3.0.0a3/docs/theorist/
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.095036 autora-core-3.0.0a3/docs/theorist/bms/
--rw-r--r--   0 jholla10   (503) staff       (20)    13470 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/docs/theorist/bms/example.ipynb
--rw-r--r--   0 jholla10   (503) staff       (20)     5203 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/docs/theorist/bms/search_space.ipynb
--rw-r--r--   0 jholla10   (503) staff       (20)  1572980 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/docs/theorist/bms/weber.ipynb
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.099016 autora-core-3.0.0a3/docs/theorist/bsr/
--rw-r--r--   0 jholla10   (503) staff       (20)     2231 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/docs/theorist/bsr/how_it_works.md
--rw-r--r--   0 jholla10   (503) staff       (20)    17622 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/docs/theorist/bsr/img.png
--rw-r--r--   0 jholla10   (503) staff       (20)      768 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/docs/theorist/bsr/introduction.md
--rw-r--r--   0 jholla10   (503) staff       (20)      951 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/docs/theorist/bsr/meta_parameters.md
--rw-r--r--   0 jholla10   (503) staff       (20)     1500 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/docs/theorist/bsr/search_space.md
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.099495 autora-core-3.0.0a3/docs/theorist/darts/
--rw-r--r--   0 jholla10   (503) staff       (20)    21418 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/docs/theorist/darts/example.ipynb
--rw-r--r--   0 jholla10   (503) staff       (20)   796078 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/docs/theorist/darts/weber.ipynb
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.084412 autora-core-3.0.0a3/mkdocs/
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.100544 autora-core-3.0.0a3/mkdocs/overrides/
--rw-r--r--   0 jholla10   (503) staff       (20)      660 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/mkdocs/overrides/main.html
--rw-r--r--   0 jholla10   (503) staff       (20)     2602 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/mkdocs.yml
--rw-r--r--   0 jholla10   (503) staff       (20)   178621 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/poetry.lock
--rw-r--r--   0 jholla10   (503) staff       (20)     1465 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/pyproject.toml
--rw-r--r--   0 jholla10   (503) staff       (20)       38 2023-04-26 21:15:31.107608 autora-core-3.0.0a3/setup.cfg
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.085443 autora-core-3.0.0a3/src/
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.085360 autora-core-3.0.0a3/src/autora/
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.101332 autora-core-3.0.0a3/src/autora/cycle/
--rw-r--r--   0 jholla10   (503) staff       (20)      197 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/cycle/__init__.py
--rw-r--r--   0 jholla10   (503) staff       (20)    20109 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/cycle/plot_utils.py
--rw-r--r--   0 jholla10   (503) staff       (20)    21619 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/cycle/simple.py
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.101852 autora-core-3.0.0a3/src/autora/experimentalist/
--rw-r--r--   0 jholla10   (503) staff       (20)    18310 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/experimentalist/pipeline.py
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.102305 autora-core-3.0.0a3/src/autora/experimentalist/pooler/
--rw-r--r--   0 jholla10   (503) staff       (20)      620 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/experimentalist/pooler/grid.py
--rw-r--r--   0 jholla10   (503) staff       (20)     1180 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/experimentalist/pooler/random_.py
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.103446 autora-core-3.0.0a3/src/autora/experimentalist/sampler/
--rw-r--r--   0 jholla10   (503) staff       (20)     2383 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/experimentalist/sampler/assumption.py
--rw-r--r--   0 jholla10   (503) staff       (20)     2841 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/experimentalist/sampler/dissimilarity.py
--rw-r--r--   0 jholla10   (503) staff       (20)     2252 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/experimentalist/sampler/model_disagreement.py
--rw-r--r--   0 jholla10   (503) staff       (20)     1666 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/experimentalist/sampler/nearest_value.py
--rw-r--r--   0 jholla10   (503) staff       (20)      497 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/experimentalist/sampler/random_.py
--rw-r--r--   0 jholla10   (503) staff       (20)     2052 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/experimentalist/sampler/uncertainty.py
--rw-r--r--   0 jholla10   (503) staff       (20)     4569 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/experimentalist/utils.py
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.103770 autora-core-3.0.0a3/src/autora/synthetic/
--rw-r--r--   0 jholla10   (503) staff       (20)     2642 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/synthetic/__init__.py
--rw-r--r--   0 jholla10   (503) staff       (20)     7338 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/synthetic/inventory.py
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.103927 autora-core-3.0.0a3/src/autora/theorist/
--rw-r--r--   0 jholla10   (503) staff       (20)        0 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/theorist/.gitkeep
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.104162 autora-core-3.0.0a3/src/autora/utils/
--rw-r--r--   0 jholla10   (503) staff       (20)        0 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/utils/__init__.py
--rw-r--r--   0 jholla10   (503) staff       (20)      441 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/utils/dictionary.py
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.104486 autora-core-3.0.0a3/src/autora/variable/
--rw-r--r--   0 jholla10   (503) staff       (20)     1866 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/variable/__init__.py
--rw-r--r--   0 jholla10   (503) staff       (20)     2511 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/src/autora/variable/time.py
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.105561 autora-core-3.0.0a3/src/autora_core.egg-info/
--rw-r--r--   0 jholla10   (503) staff       (20)    19467 2023-04-26 21:15:31.000000 autora-core-3.0.0a3/src/autora_core.egg-info/PKG-INFO
--rw-r--r--   0 jholla10   (503) staff       (20)     2449 2023-04-26 21:15:31.000000 autora-core-3.0.0a3/src/autora_core.egg-info/SOURCES.txt
--rw-r--r--   0 jholla10   (503) staff       (20)        1 2023-04-26 21:15:31.000000 autora-core-3.0.0a3/src/autora_core.egg-info/dependency_links.txt
--rw-r--r--   0 jholla10   (503) staff       (20)      350 2023-04-26 21:15:31.000000 autora-core-3.0.0a3/src/autora_core.egg-info/requires.txt
--rw-r--r--   0 jholla10   (503) staff       (20)        7 2023-04-26 21:15:31.000000 autora-core-3.0.0a3/src/autora_core.egg-info/top_level.txt
-drwxr-xr-x   0 jholla10   (503) staff       (20)        0 2023-04-26 21:15:31.106917 autora-core-3.0.0a3/tests/
--rw-r--r--   0 jholla10   (503) staff       (20)     1491 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/tests/README.md
--rw-r--r--   0 jholla10   (503) staff       (20)        0 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/tests/__init__.py
--rw-r--r--   0 jholla10   (503) staff       (20)    13298 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/tests/test_cycle_plots.py
--rw-r--r--   0 jholla10   (503) staff       (20)    10040 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/tests/test_experimentalist_pipeline.py
--rw-r--r--   0 jholla10   (503) staff       (20)     4193 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/tests/test_experimentalist_random.py
--rw-r--r--   0 jholla10   (503) staff       (20)      862 2023-04-26 21:12:29.000000 autora-core-3.0.0a3/tests/test_synthetic_inventory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.129517 autora-core-3.0.0a5/
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/.editorconfig
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.117517 autora-core-3.0.0a5/.github/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/.github/dependabot.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/.github/pull_request_template.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.117517 autora-core-3.0.0a5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1078 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/.github/workflows/publish-package-pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/.github/workflows/test-pytest.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.121517 autora-core-3.0.0a5/.idea/
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/.idea/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1589 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/.idea/autora-core.iml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.121517 autora-core-3.0.0a5/.idea/codeStyles/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/.idea/codeStyles/codeStyleConfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/.idea/encodings.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.121517 autora-core-3.0.0a5/.idea/inspectionProfiles/
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/.idea/inspectionProfiles/Project_Default.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/.idea/inspectionProfiles/profiles_settings.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/.idea/misc.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/.idea/modules.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/.idea/other.xml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.121517 autora-core-3.0.0a5/.idea/runConfigurations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/.idea/runConfigurations/pytest.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/.idea/vcs.xml
+-rw-r--r--   0 runner    (1001) docker     (123)      796 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/.pre-commit-config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.121517 autora-core-3.0.0a5/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/.vscode/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/.vscode/extensions.json
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/.vscode/launch.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)    19464 2023-04-27 19:23:16.129517 autora-core-3.0.0a5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    18766 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.117517 autora-core-3.0.0a5/conda/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.121517 autora-core-3.0.0a5/conda/autora/
+-rw-r--r--   0 runner    (1001) docker     (123)     1315 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/conda/autora/meta.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/conda/autora/run_test.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.117517 autora-core-3.0.0a5/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.121517 autora-core-3.0.0a5/docs/cycle/
+-rw-r--r--   0 runner    (1001) docker     (123)   148488 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/docs/cycle/simple_cycle_bms_model_poppernet.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.121517 autora-core-3.0.0a5/docs/experimentalists/
+-rw-r--r--   0 runner    (1001) docker     (123)     2779 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/docs/experimentalists/overview.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.117517 autora-core-3.0.0a5/docs/theorist/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.121517 autora-core-3.0.0a5/docs/theorist/bms/
+-rw-r--r--   0 runner    (1001) docker     (123)    13470 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/docs/theorist/bms/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     5203 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/docs/theorist/bms/search_space.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)  1572980 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/docs/theorist/bms/weber.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.125517 autora-core-3.0.0a5/docs/theorist/bsr/
+-rw-r--r--   0 runner    (1001) docker     (123)     2231 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/docs/theorist/bsr/how_it_works.md
+-rw-r--r--   0 runner    (1001) docker     (123)    17622 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/docs/theorist/bsr/img.png
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/docs/theorist/bsr/introduction.md
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/docs/theorist/bsr/meta_parameters.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1500 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/docs/theorist/bsr/search_space.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.125517 autora-core-3.0.0a5/docs/theorist/darts/
+-rw-r--r--   0 runner    (1001) docker     (123)    21418 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/docs/theorist/darts/example.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   796078 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/docs/theorist/darts/weber.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.117517 autora-core-3.0.0a5/mkdocs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.125517 autora-core-3.0.0a5/mkdocs/overrides/
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/mkdocs/overrides/main.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/mkdocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 19:23:16.129517 autora-core-3.0.0a5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.117517 autora-core-3.0.0a5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.117517 autora-core-3.0.0a5/src/autora/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.125517 autora-core-3.0.0a5/src/autora/cycle/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/src/autora/cycle/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20109 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/src/autora/cycle/plot_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21598 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/src/autora/cycle/simple.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.125517 autora-core-3.0.0a5/src/autora/experimentalist/
+-rw-r--r--   0 runner    (1001) docker     (123)    18310 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/src/autora/experimentalist/pipeline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.125517 autora-core-3.0.0a5/src/autora/experimentalist/pooler/
+-rw-r--r--   0 runner    (1001) docker     (123)      620 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/src/autora/experimentalist/pooler/grid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1180 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/src/autora/experimentalist/pooler/random_pooler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.125517 autora-core-3.0.0a5/src/autora/experimentalist/sampler/
+-rw-r--r--   0 runner    (1001) docker     (123)     2383 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/src/autora/experimentalist/sampler/assumption.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2841 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/src/autora/experimentalist/sampler/dissimilarity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/src/autora/experimentalist/sampler/model_disagreement.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/src/autora/experimentalist/sampler/nearest_value.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/src/autora/experimentalist/sampler/random_sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/src/autora/experimentalist/sampler/uncertainty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4502 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/src/autora/experimentalist/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.125517 autora-core-3.0.0a5/src/autora/synthetic/
+-rw-r--r--   0 runner    (1001) docker     (123)     7372 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/src/autora/synthetic/inventory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.125517 autora-core-3.0.0a5/src/autora/theorist/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/src/autora/theorist/.gitkeep
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.125517 autora-core-3.0.0a5/src/autora/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      441 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/src/autora/utils/dictionary.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.129517 autora-core-3.0.0a5/src/autora/variable/
+-rw-r--r--   0 runner    (1001) docker     (123)     1866 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/src/autora/variable/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2511 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/src/autora/variable/time.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.129517 autora-core-3.0.0a5/src/autora_core.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    19464 2023-04-27 19:23:16.000000 autora-core-3.0.0a5/src/autora_core.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2134 2023-04-27 19:23:16.000000 autora-core-3.0.0a5/src/autora_core.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 19:23:16.000000 autora-core-3.0.0a5/src/autora_core.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      350 2023-04-27 19:23:16.000000 autora-core-3.0.0a5/src/autora_core.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-27 19:23:16.000000 autora-core-3.0.0a5/src/autora_core.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 19:23:16.129517 autora-core-3.0.0a5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/tests/test_cycle_plots.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10040 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/tests/test_experimentalist_pipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4200 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/tests/test_experimentalist_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      773 2023-04-27 19:23:04.000000 autora-core-3.0.0a5/tests/test_synthetic_inventory.py
```

### Comparing `autora-core-3.0.0a3/.github/pull_request_template.md` & `autora-core-3.0.0a5/.github/pull_request_template.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/.github/workflows/test-pytest.yml` & `autora-core-3.0.0a5/.github/workflows/test-pytest.yml`

 * *Files 8% similar despite different names*

```diff
@@ -3,25 +3,27 @@
 
 name: Test with py.test
 
 on:
   pull_request:
   merge_group:
   workflow_call:
+  push:
+    branches:
+      - main
 
 jobs:
   test:
     strategy:
       fail-fast: true
       matrix:
-        python-version: ["3.8", "3.9", "3.10"]
+        python-version: ["3.8", "3.9", "3.10", "3.11"]
         os: [ubuntu-latest, macos-latest, windows-latest]
     runs-on: ${{ matrix.os }}
     steps:
     - uses: actions/checkout@v3
-    - run: pipx install poetry
     - uses: actions/setup-python@v4
       with:
         python-version: ${{ matrix.python-version }}
-        cache: "poetry"
-    - run: poetry install --only main,test
-    - run: poetry run pytest
+        cache: "pip"
+    - run: pip install ".[dev]"
+    - run: pytest --doctest-modules
```

### Comparing `autora-core-3.0.0a3/.gitignore` & `autora-core-3.0.0a5/.gitignore`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/.idea/autora-core.iml` & `autora-core-3.0.0a5/.idea/autora-core.iml`

 * *Files 10% similar despite different names*

#### Comparing `autora-core-3.0.0a3/.idea/autora-core.iml` & `autora-core-3.0.0a5/.idea/autora-core.iml`

```diff
@@ -9,29 +9,27 @@
       <excludeFolder url="file://$MODULE_DIR$/.venv"/>
       <excludeFolder url="file://$MODULE_DIR$/.vscode"/>
       <excludeFolder url="file://$MODULE_DIR$/site"/>
       <excludeFolder url="file://$MODULE_DIR$/example/studies/Weber Sampled/modeling"/>
       <excludeFolder url="file://$MODULE_DIR$/example/studies/Weber/modeling"/>
       <excludeFolder url="file://$MODULE_DIR$/venv"/>
     </content>
-    <orderEntry type="jdk" jdkName="Poetry (autora) (2)" jdkType="Python SDK"/>
     <orderEntry type="sourceFolder" forTests="false"/>
   </component>
   <component name="PackageRequirementsSettings">
     <option name="requirementsPath" value=""/>
   </component>
   <component name="PyDocumentationSettings">
     <option name="format" value="GOOGLE"/>
     <option name="myDocStringFormat" value="Google"/>
     <option name="renderExternalDocumentation" value="true"/>
   </component>
   <component name="PyNamespacePackagesService">
     <option name="namespacePackageFolders">
       <list>
         <option value="$MODULE_DIR$/src/autora"/>
+        <option value="$MODULE_DIR$/src/autora/synthetic"/>
+        <option value="$MODULE_DIR$/src/autora/experimentalist"/>
       </list>
     </option>
   </component>
-  <component name="TestRunnerService">
-    <option name="PROJECT_TEST_RUNNER" value="py.test"/>
-  </component>
 </module>
```

### Comparing `autora-core-3.0.0a3/.idea/inspectionProfiles/Project_Default.xml` & `autora-core-3.0.0a5/.idea/inspectionProfiles/Project_Default.xml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/.idea/runConfigurations/pytest_in_tests.xml` & `autora-core-3.0.0a5/.idea/runConfigurations/pytest.xml`

 * *Files 14% similar despite different names*

#### Comparing `autora-core-3.0.0a3/.idea/runConfigurations/pytest_in_tests.xml` & `autora-core-3.0.0a5/.idea/runConfigurations/pytest.xml`

```diff
@@ -1,20 +1,20 @@
 <?xml version="1.0" encoding="utf-8"?>
 <component name="ProjectRunConfigurationManager">
-  <configuration default="false" name="pytest in tests" type="tests" factoryName="py.test" nameIsGenerated="true">
-    <module name="autora"/>
+  <configuration default="false" name="pytest" type="tests" factoryName="py.test" nameIsGenerated="true">
+    <module name="autora-core"/>
     <option name="INTERPRETER_OPTIONS" value=""/>
     <option name="PARENT_ENVS" value="true"/>
     <option name="SDK_HOME" value=""/>
-    <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$/tests"/>
+    <option name="WORKING_DIRECTORY" value="$PROJECT_DIR$"/>
     <option name="IS_MODULE_SDK" value="true"/>
     <option name="ADD_CONTENT_ROOTS" value="true"/>
     <option name="ADD_SOURCE_ROOTS" value="true"/>
     <EXTENSION ID="PythonCoverageRunConfigurationExtension" runner="coverage.py"/>
     <option name="_new_keywords" value="&quot;&quot;"/>
     <option name="_new_parameters" value="&quot;&quot;"/>
-    <option name="_new_additionalArguments" value="&quot;&quot;"/>
-    <option name="_new_target" value="&quot;$PROJECT_DIR$/tests&quot;"/>
-    <option name="_new_targetType" value="&quot;PATH&quot;"/>
+    <option name="_new_additionalArguments" value="&quot;pytest --doctest-modules&quot;"/>
+    <option name="_new_target" value="&quot;&quot;"/>
+    <option name="_new_targetType" value="&quot;CUSTOM&quot;"/>
     <method v="2"/>
   </configuration>
 </component>
```

### Comparing `autora-core-3.0.0a3/.pre-commit-config.yaml` & `autora-core-3.0.0a5/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/LICENSE.md` & `autora-core-3.0.0a5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/PKG-INFO` & `autora-core-3.0.0a5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: autora-core
-Version: 3.0.0a3
+Version: 3.0.0a5
 Summary: Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process. 
 Author-email: Sebastian Musslick <sebastian_musslick@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>
 Project-URL: homepage, https://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-theorist-template
 Project-URL: documentation, https://autoresearch.github.io/autora/
-Requires-Python: <3.11,>=3.8.10
+Requires-Python: <4,>=3.8.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: build
 Provides-Extra: notebook
 Provides-Extra: docs
 License-File: LICENSE.md
```

### Comparing `autora-core-3.0.0a3/README.md` & `autora-core-3.0.0a5/README.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/conda/autora/meta.yaml` & `autora-core-3.0.0a5/conda/autora/meta.yaml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/docs/cycle/simple_cycle_bms_model_poppernet.ipynb` & `autora-core-3.0.0a5/docs/cycle/simple_cycle_bms_model_poppernet.ipynb`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/docs/experimentalists/overview.md` & `autora-core-3.0.0a5/docs/experimentalists/overview.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/docs/theorist/bms/example.ipynb` & `autora-core-3.0.0a5/docs/theorist/bms/example.ipynb`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/docs/theorist/bms/search_space.ipynb` & `autora-core-3.0.0a5/docs/theorist/bms/search_space.ipynb`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/docs/theorist/bms/weber.ipynb` & `autora-core-3.0.0a5/docs/theorist/bms/weber.ipynb`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/docs/theorist/bsr/how_it_works.md` & `autora-core-3.0.0a5/docs/theorist/bsr/how_it_works.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/docs/theorist/bsr/img.png` & `autora-core-3.0.0a5/docs/theorist/bsr/img.png`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/docs/theorist/bsr/introduction.md` & `autora-core-3.0.0a5/docs/theorist/bsr/introduction.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/docs/theorist/bsr/meta_parameters.md` & `autora-core-3.0.0a5/docs/theorist/bsr/meta_parameters.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/docs/theorist/bsr/search_space.md` & `autora-core-3.0.0a5/docs/theorist/bsr/search_space.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/docs/theorist/darts/example.ipynb` & `autora-core-3.0.0a5/docs/theorist/darts/example.ipynb`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/docs/theorist/darts/weber.ipynb` & `autora-core-3.0.0a5/docs/theorist/darts/weber.ipynb`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/mkdocs/overrides/main.html` & `autora-core-3.0.0a5/mkdocs/overrides/main.html`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/mkdocs.yml` & `autora-core-3.0.0a5/mkdocs.yml`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/pyproject.toml` & `autora-core-3.0.0a5/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 name = "autora-core"
 description = "Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process. "
 authors = [
     { name="Sebastian Musslick", email="sebastian_musslick@brown.edu" },
     { name="John Gerrard Holland", email="john_holland1@brown.edu" },
 ]
 readme = "README.md"
-requires-python = ">=3.8.10,<3.11"
+requires-python = ">=3.8.10,<4"
 dynamic = ["version"]
 
 dependencies = [
     "numpy",
     "matplotlib",
     "pandas",
     "scikit-learn"
```

### Comparing `autora-core-3.0.0a3/src/autora/cycle/plot_utils.py` & `autora-core-3.0.0a5/src/autora/cycle/plot_utils.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/src/autora/cycle/simple.py` & `autora-core-3.0.0a5/src/autora/cycle/simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,15 @@
         >>> import numpy as np
         >>> def get_example_synthetic_experiment_runner():
         ...     rng = np.random.default_rng(seed=180)
         ...     def runner(x):
         ...         return ground_truth(x) + rng.normal(0, 0.1, x.shape)
         ...     return runner
         >>> example_synthetic_experiment_runner = get_example_synthetic_experiment_runner()
-        >>> example_synthetic_experiment_runner(np.ndarray([1]))
+        >>> example_synthetic_experiment_runner(np.array([1.]))
         array([2.04339546])
 
         The theorist "tries" to work out the best theory.
         We use a trivial scikit-learn regressor.
         >>> from sklearn.linear_model import LinearRegression
         >>> example_theorist = LinearRegression()
 
@@ -139,22 +139,22 @@
         ...     metadata=metadata_0,
         ...     theorist=example_theorist,
         ...     experimentalist=example_experimentalist,
         ...     experiment_runner=example_synthetic_experiment_runner,
         ...     monitor=lambda data: print(f"Generated {len(data.theories)} theories"),
         ... )
         >>> cycle # doctest: +ELLIPSIS
-        <simple.SimpleCycle object at 0x...>
+        <...SimpleCycle object at 0x...>
 
         We can run the cycle by calling the run method:
         >>> cycle.run(num_cycles=3)  # doctest: +ELLIPSIS
         Generated 1 theories
         Generated 2 theories
         Generated 3 theories
-        <simple.SimpleCycle object at 0x...>
+        <...SimpleCycle object at 0x...>
 
         We can now interrogate the results. The first set of conditions which went into the
         experiment runner were:
         >>> cycle.data.conditions[0]
         array([ 0,  1,  2,  3,  4,  5,  6,  7,  8,  9, 10])
 
         The observations include the conditions and the results:
@@ -192,23 +192,23 @@
         'y = 0.9989 x + 1.0292'
 
         This is close to the ground truth theory of x -> (x + 1)
 
         We can also run the cycle with more control over the execution flow:
         >>> next(cycle) # doctest: +ELLIPSIS
         Generated 4 theories
-        <simple.SimpleCycle object at 0x...>
+        <...SimpleCycle object at 0x...>
 
         >>> next(cycle) # doctest: +ELLIPSIS
         Generated 5 theories
-        <simple.SimpleCycle object at 0x...>
+        <...SimpleCycle object at 0x...>
 
         >>> next(cycle) # doctest: +ELLIPSIS
         Generated 6 theories
-        <simple.SimpleCycle object at 0x...>
+        <...SimpleCycle object at 0x...>
 
         We can continue to run the cycle as long as we like,
         with a simple arbitrary stopping condition like the number of theories generated:
         >>> from itertools import takewhile
         >>> _ = list(takewhile(lambda c: len(c.data.theories) < 9, cycle))
         Generated 7 theories
         Generated 8 theories
```

### Comparing `autora-core-3.0.0a3/src/autora/experimentalist/pipeline.py` & `autora-core-3.0.0a5/src/autora/experimentalist/pipeline.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/src/autora/experimentalist/pooler/grid.py` & `autora-core-3.0.0a5/src/autora/experimentalist/pooler/grid.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/src/autora/experimentalist/pooler/random_.py` & `autora-core-3.0.0a5/src/autora/experimentalist/pooler/random_pooler.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/src/autora/experimentalist/sampler/assumption.py` & `autora-core-3.0.0a5/src/autora/experimentalist/sampler/assumption.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/src/autora/experimentalist/sampler/dissimilarity.py` & `autora-core-3.0.0a5/src/autora/experimentalist/sampler/dissimilarity.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/src/autora/experimentalist/sampler/model_disagreement.py` & `autora-core-3.0.0a5/src/autora/experimentalist/sampler/model_disagreement.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/src/autora/experimentalist/sampler/nearest_value.py` & `autora-core-3.0.0a5/src/autora/experimentalist/sampler/nearest_value.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/src/autora/experimentalist/sampler/uncertainty.py` & `autora-core-3.0.0a5/src/autora/experimentalist/sampler/uncertainty.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/src/autora/experimentalist/utils.py` & `autora-core-3.0.0a5/src/autora/experimentalist/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,20 +21,19 @@
         For mixed datatypes, the highest-level type common to all the inputs will be used, so
         consider using [_sequence_to_recarray][autora.experimentalist.utils._sequence_to_recarray]
         instead.
         >>> sequence_to_array(zip(range(5), "abcde"))  # doctest: +NORMALIZE_WHITESPACE
         array([['0', 'a'], ['1', 'b'], ['2', 'c'], ['3', 'd'], ['4', 'e']],  dtype='<U21')
 
         Single strings are broken into characters:
-        >>> sequence_to_array("abcde",array_type="numpy.array")  # doctest: +NORMALIZE_WHITESPACE
+        >>> sequence_to_array("abcde")  # doctest: +NORMALIZE_WHITESPACE
         array([['a'], ['b'], ['c'], ['d'], ['e']], dtype='<U1')
 
         Multiple strings are treated as individual entries:
-        >>> sequence_to_array(["abc", "de"],array_type="numpy.array"
-        ...     )  # doctest: +NORMALIZE_WHITESPACE
+        >>> sequence_to_array(["abc", "de"])  # doctest: +NORMALIZE_WHITESPACE
         array([['abc'], ['de']], dtype='<U3')
 
     """
     deque = collections.deque(iterable)
     array = np.array(deque).reshape((len(deque), -1))
     return array
```

### Comparing `autora-core-3.0.0a3/src/autora/synthetic/inventory.py` & `autora-core-3.0.0a5/src/autora/synthetic/inventory.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,17 @@
 Examples:
     To add and recover a new model from the inventory, we need to define it using a function
     (closure).
     We start by importing the modules we'll need:
     >>> from functools import partial
     >>> import matplotlib.pyplot as plt
     >>> import numpy as np
-    >>> from autora.synthetic import register, retrieve, describe, SyntheticExperimentCollection
+    >>> from autora.synthetic.inventory import (
+    ...     register, retrieve, describe, SyntheticExperimentCollection
+    ... )
     >>> from autora.variable import IV, DV, VariableCollection
 
     Then we can define the function. We define all the arguments we want and add them to a
     dictionary. The closure – in this case `sinusoid_experiment` – is the scope for all
     the parameters we need.
     >>> def sinusoid_experiment(omega=np.pi/3, delta=np.pi/2., m=0.3, resolution=1000,
     ...                         rng=np.random.default_rng()):
```

### Comparing `autora-core-3.0.0a3/src/autora/variable/__init__.py` & `autora-core-3.0.0a5/src/autora/variable/__init__.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/src/autora/variable/time.py` & `autora-core-3.0.0a5/src/autora/variable/time.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/src/autora_core.egg-info/PKG-INFO` & `autora-core-3.0.0a5/src/autora_core.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: autora-core
-Version: 3.0.0a3
+Version: 3.0.0a5
 Summary: Autonomous Research Assistant (AutoRA) is a framework for automating steps of the empirical research process. 
 Author-email: Sebastian Musslick <sebastian_musslick@brown.edu>, John Gerrard Holland <john_holland1@brown.edu>
 Project-URL: homepage, https://www.empiricalresearch.ai
 Project-URL: repository, https://github.com/AutoResearch/autora-theorist-template
 Project-URL: documentation, https://autoresearch.github.io/autora/
-Requires-Python: <3.11,>=3.8.10
+Requires-Python: <4,>=3.8.10
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 Provides-Extra: test
 Provides-Extra: build
 Provides-Extra: notebook
 Provides-Extra: docs
 License-File: LICENSE.md
```

### Comparing `autora-core-3.0.0a3/src/autora_core.egg-info/SOURCES.txt` & `autora-core-3.0.0a5/src/autora_core.egg-info/SOURCES.txt`

 * *Files 16% similar despite different names*

```diff
@@ -1,35 +1,29 @@
 .editorconfig
 .gitignore
 .pre-commit-config.yaml
 LICENSE.md
 README.md
 mkdocs.yml
-poetry.lock
 pyproject.toml
 .github/dependabot.yml
 .github/pull_request_template.md
-.github/workflows/publish-documentation-gh-pages.yml
-.github/workflows/publish-package-anaconda-org.yml
 .github/workflows/publish-package-pypi.yml
-.github/workflows/test-conda-build.yml
-.github/workflows/test-poetry-build.yml
-.github/workflows/test-pre-commit-hooks.yml
 .github/workflows/test-pytest.yml
 .idea/.gitignore
 .idea/autora-core.iml
 .idea/encodings.xml
 .idea/misc.xml
 .idea/modules.xml
 .idea/other.xml
 .idea/vcs.xml
 .idea/codeStyles/codeStyleConfig.xml
 .idea/inspectionProfiles/Project_Default.xml
 .idea/inspectionProfiles/profiles_settings.xml
-.idea/runConfigurations/pytest_in_tests.xml
+.idea/runConfigurations/pytest.xml
 .vscode/.gitignore
 .vscode/extensions.json
 .vscode/launch.json
 conda/autora/meta.yaml
 conda/autora/run_test.sh
 docs/cycle/simple_cycle_bms_model_poppernet.ipynb
 docs/experimentalists/overview.md
@@ -46,32 +40,29 @@
 mkdocs/overrides/main.html
 src/autora/cycle/__init__.py
 src/autora/cycle/plot_utils.py
 src/autora/cycle/simple.py
 src/autora/experimentalist/pipeline.py
 src/autora/experimentalist/utils.py
 src/autora/experimentalist/pooler/grid.py
-src/autora/experimentalist/pooler/random_.py
+src/autora/experimentalist/pooler/random_pooler.py
 src/autora/experimentalist/sampler/assumption.py
 src/autora/experimentalist/sampler/dissimilarity.py
 src/autora/experimentalist/sampler/model_disagreement.py
 src/autora/experimentalist/sampler/nearest_value.py
-src/autora/experimentalist/sampler/random_.py
+src/autora/experimentalist/sampler/random_sampler.py
 src/autora/experimentalist/sampler/uncertainty.py
-src/autora/synthetic/__init__.py
 src/autora/synthetic/inventory.py
 src/autora/theorist/.gitkeep
-src/autora/utils/__init__.py
 src/autora/utils/dictionary.py
 src/autora/variable/__init__.py
 src/autora/variable/time.py
 src/autora_core.egg-info/PKG-INFO
 src/autora_core.egg-info/SOURCES.txt
 src/autora_core.egg-info/dependency_links.txt
 src/autora_core.egg-info/requires.txt
 src/autora_core.egg-info/top_level.txt
 tests/README.md
-tests/__init__.py
 tests/test_cycle_plots.py
 tests/test_experimentalist_pipeline.py
 tests/test_experimentalist_random.py
 tests/test_synthetic_inventory.py
```

### Comparing `autora-core-3.0.0a3/tests/README.md` & `autora-core-3.0.0a5/tests/README.md`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/tests/test_cycle_plots.py` & `autora-core-3.0.0a5/tests/test_cycle_plots.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,15 @@
     plot_cycle_score,
     plot_results_panel_2d,
     plot_results_panel_3d,
 )
 from autora.cycle.plot_utils import _check_replace_default_kw
 from autora.experimentalist.pipeline import Pipeline
 from autora.experimentalist.pooler.grid import grid_pool
-from autora.experimentalist.sampler.random_ import random_sampler
+from autora.experimentalist.sampler.random_sampler import random_sampler
 from autora.variable import Variable, VariableCollection
 
 
 @pytest.fixture
 def ground_truth_1x():
     def ground_truth(xs):
         return xs + 1.0
```

### Comparing `autora-core-3.0.0a3/tests/test_experimentalist_pipeline.py` & `autora-core-3.0.0a5/tests/test_experimentalist_pipeline.py`

 * *Files identical despite different names*

### Comparing `autora-core-3.0.0a3/tests/test_experimentalist_random.py` & `autora-core-3.0.0a5/tests/test_experimentalist_random.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from functools import partial
 
 import numpy as np
 import pytest
 
 from autora.experimentalist.pipeline import make_pipeline
 from autora.experimentalist.pooler.grid import grid_pool
-from autora.experimentalist.sampler.random_ import random_sampler
+from autora.experimentalist.sampler.random_sampler import random_sampler
 from autora.variable import DV, IV, ValueType, VariableCollection
 
 
 def weber_filter(values):
     return filter(lambda s: s[0] <= s[1], values)
```

### Comparing `autora-core-3.0.0a3/tests/test_synthetic_inventory.py` & `autora-core-3.0.0a5/tests/test_synthetic_inventory.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,22 +1,21 @@
-import autora.synthetic
-from autora.synthetic.inventory import SyntheticExperimentCollection
+from autora.synthetic.inventory import SyntheticExperimentCollection, retrieve, register
 from autora.variable import VariableCollection
 
 
 def test_model_registration_retrieval():
     # We can register a model and retrieve it
-    autora.synthetic.register("empty", lambda: SyntheticExperimentCollection())
-    empty = autora.synthetic.retrieve("empty")
+    register("empty", lambda: SyntheticExperimentCollection())
+    empty = retrieve("empty")
     assert empty.name is None
 
     # We can register another model and retrieve it as well
-    autora.synthetic.register(
+    register(
         "only_metadata",
         lambda: SyntheticExperimentCollection(metadata=VariableCollection()),
     )
-    only_metadata = autora.synthetic.retrieve("only_metadata")
+    only_metadata = retrieve("only_metadata")
     assert only_metadata.metadata is not None
 
     # We can still retrieve the first model, and it is equal to the first version
-    empty_copy = autora.synthetic.retrieve("empty")
+    empty_copy = retrieve("empty")
     assert empty_copy == empty
```

