# Comparing `tmp/aiida-quantumespresso-4.2.0.tar.gz` & `tmp/aiida-quantumespresso-4.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiida-quantumespresso-4.2.0.tar", last modified: Thu Feb  2 21:57:35 2023, max compression
+gzip compressed data, was "aiida-quantumespresso-4.3.0.tar", last modified: Thu Apr 27 14:24:01 2023, max compression
```

## Comparing `aiida-quantumespresso-4.2.0.tar` & `aiida-quantumespresso-4.3.0.tar`

### file list

```diff
@@ -1,192 +1,206 @@
--rw-r--r--   0        0        0      148 2023-02-02 21:57:30.011762 aiida-quantumespresso-4.2.0/.github/config/code-ph.yaml
--rw-r--r--   0        0        0      148 2023-02-02 21:57:30.011762 aiida-quantumespresso-4.2.0/.github/config/code-pw.yaml
--rw-r--r--   0        0        0       43 2023-02-02 21:57:30.011762 aiida-quantumespresso-4.2.0/.github/config/localhost-config.yaml
--rw-r--r--   0        0        0      234 2023-02-02 21:57:30.011762 aiida-quantumespresso-4.2.0/.github/config/localhost-setup.yaml
--rw-r--r--   0        0        0      215 2023-02-02 21:57:30.011762 aiida-quantumespresso-4.2.0/.github/config/profile.yaml
--rw-r--r--   0        0        0     1922 2023-02-02 21:57:30.011762 aiida-quantumespresso-4.2.0/.github/scripts/run_documentation_scripts.py
--rw-r--r--   0        0        0     3009 2023-02-02 21:57:30.011762 aiida-quantumespresso-4.2.0/.github/workflows/cd.yml
--rw-r--r--   0        0        0     4135 2023-02-02 21:57:30.011762 aiida-quantumespresso-4.2.0/.github/workflows/ci.yml
--rw-r--r--   0        0        0     2291 2023-02-02 21:57:30.011762 aiida-quantumespresso-4.2.0/.github/workflows/nightly.yml
--rw-r--r--   0        0        0     1520 2023-02-02 21:57:30.011762 aiida-quantumespresso-4.2.0/.github/workflows/validate_release_tag.py
--rw-r--r--   0        0        0     1303 2023-02-02 21:57:30.011762 aiida-quantumespresso-4.2.0/.gitignore
--rw-r--r--   0        0        0     1323 2023-02-02 21:57:30.011762 aiida-quantumespresso-4.2.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0      239 2023-02-02 21:57:30.011762 aiida-quantumespresso-4.2.0/.readthedocs.yml
--rw-r--r--   0        0        0    28686 2023-02-02 21:57:30.011762 aiida-quantumespresso-4.2.0/CHANGELOG.md
--rw-r--r--   0        0        0     1273 2023-02-02 21:57:30.011762 aiida-quantumespresso-4.2.0/LICENSE.txt
--rw-r--r--   0        0        0    29595 2023-02-02 21:57:30.011762 aiida-quantumespresso-4.2.0/README.md
--rw-r--r--   0        0        0     7910 2023-02-02 21:57:30.019761 aiida-quantumespresso-4.2.0/pyproject.toml
--rw-r--r--   0        0        0      100 2023-02-02 21:57:30.019761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/__init__.py
--rw-r--r--   0        0        0    38525 2023-02-02 21:57:30.019761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/__init__.py
--rw-r--r--   0        0        0     2017 2023-02-02 21:57:30.019761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/base.py
--rw-r--r--   0        0        0     6658 2023-02-02 21:57:30.019761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/cp.py
--rw-r--r--   0        0        0     1539 2023-02-02 21:57:30.019761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/dos.py
--rw-r--r--   0        0        0    14071 2023-02-02 21:57:30.019761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/epw.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.019761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/functions/__init__.py
--rw-r--r--   0        0        0     1595 2023-02-02 21:57:30.019761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/functions/create_kpoints_from_distance.py
--rw-r--r--   0        0        0     1436 2023-02-02 21:57:30.019761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/functions/seekpath_structure_analysis.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.019761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/functions/xspectra/__init__.py
--rw-r--r--   0        0        0     4593 2023-02-02 21:57:30.019761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/functions/xspectra/get_powder_spectrum.py
--rw-r--r--   0        0        0     2624 2023-02-02 21:57:30.019761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/functions/xspectra/merge_spectra.py
--rw-r--r--   0        0        0    84796 2023-02-02 21:57:30.019761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.1.xml
--rw-r--r--   0        0        0    87073 2023-02-02 21:57:30.019761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.2.xml
--rw-r--r--   0        0        0    87073 2023-02-02 21:57:30.019761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.3.xml
--rw-r--r--   0        0        0    83767 2023-02-02 21:57:30.019761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.xml
--rw-r--r--   0        0        0    96224 2023-02-02 21:57:30.019761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.1.xml
--rw-r--r--   0        0        0    96319 2023-02-02 21:57:30.019761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.2.xml
--rw-r--r--   0        0        0    93230 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.xml
--rw-r--r--   0        0        0    96763 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.2.0.xml
--rw-r--r--   0        0        0    97862 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.2.1.xml
--rw-r--r--   0        0        0    97871 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.3.0.xml
--rw-r--r--   0        0        0    98698 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.4.0.xml
--rw-r--r--   0        0        0   109373 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.0.xml
--rw-r--r--   0        0        0   110988 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.1.xml
--rw-r--r--   0        0        0   112295 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.2.xml
--rw-r--r--   0        0        0   116180 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.3.xml
--rw-r--r--   0        0        0   118149 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.4.xml
--rw-r--r--   0        0        0    26623 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/__init__.py
--rw-r--r--   0        0        0     4696 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/matdyn.py
--rw-r--r--   0        0        0    10109 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/namelists.py
--rw-r--r--   0        0        0    17188 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/neb.py
--rw-r--r--   0        0        0    16661 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/ph.py
--rw-r--r--   0        0        0    11374 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/pp.py
--rw-r--r--   0        0        0     3843 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/projwfc.py
--rw-r--r--   0        0        0    13353 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/pw.py
--rw-r--r--   0        0        0     3578 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/pw2gw.py
--rw-r--r--   0        0        0     3052 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/pw2wannier90.py
--rw-r--r--   0        0        0    23331 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/pwimmigrant.py
--rw-r--r--   0        0        0     1977 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/q2r.py
--rw-r--r--   0        0        0     6026 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/xspectra.py
--rw-r--r--   0        0        0      609 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/__init__.py
--rw-r--r--   0        0        0      874 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/calculations/__init__.py
--rw-r--r--   0        0        0     2130 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/calculations/cp.py
--rwxr-xr-x   0        0        0     1992 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/calculations/dos.py
--rw-r--r--   0        0        0     3530 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/calculations/epw.py
--rw-r--r--   0        0        0     1418 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/calculations/matdyn.py
--rw-r--r--   0        0        0     3622 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/calculations/neb.py
--rw-r--r--   0        0        0     2118 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/calculations/ph.py
--rw-r--r--   0        0        0     1981 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/calculations/pp.py
--rwxr-xr-x   0        0        0     2012 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/calculations/projwfc.py
--rw-r--r--   0        0        0     4164 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/calculations/pw.py
--rwxr-xr-x   0        0        0     3060 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/calculations/pw2wannier90.py
--rw-r--r--   0        0        0     1794 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/calculations/q2r.py
--rw-r--r--   0        0        0      361 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/data/__init__.py
--rw-r--r--   0        0        0     1062 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/data/structure.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/utils/__init__.py
--rw-r--r--   0        0        0     1555 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/utils/defaults.py
--rw-r--r--   0        0        0     1530 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/utils/display.py
--rw-r--r--   0        0        0     1259 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/utils/launch.py
--rw-r--r--   0        0        0     6823 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/utils/options.py
--rw-r--r--   0        0        0     6150 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/utils/validate.py
--rw-r--r--   0        0        0      675 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/workflows/__init__.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/workflows/matdyn/__init__.py
--rwxr-xr-x   0        0        0     1666 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/workflows/matdyn/base.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/workflows/ph/__init__.py
--rwxr-xr-x   0        0        0     1568 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/workflows/ph/base.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/workflows/pw/__init__.py
--rwxr-xr-x   0        0        0     4024 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/workflows/pw/bands.py
--rwxr-xr-x   0        0        0     3109 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/workflows/pw/base.py
--rwxr-xr-x   0        0        0     3798 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/workflows/pw/relax.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/workflows/q2r/__init__.py
--rwxr-xr-x   0        0        0     1720 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/workflows/q2r/base.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/common/__init__.py
--rw-r--r--   0        0        0     1588 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/common/types.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/data/__init__.py
--rw-r--r--   0        0        0     9255 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/data/force_constants.py
--rw-r--r--   0        0        0      202 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/__init__.py
--rw-r--r--   0        0        0     2474 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/base.py
--rw-r--r--   0        0        0    16768 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/cp.py
--rw-r--r--   0        0        0     5575 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/dos.py
--rw-r--r--   0        0        0     4778 2023-02-02 21:57:30.023761 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/matdyn.py
--rw-r--r--   0        0        0    10493 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/neb.py
--rw-r--r--   0        0        0       71 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_raw/__init__.py
--rw-r--r--   0        0        0     6752 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_raw/base.py
--rw-r--r--   0        0        0     8844 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_raw/cp.py
--rw-r--r--   0        0        0    10943 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_raw/neb.py
--rw-r--r--   0        0        0    17956 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_raw/ph.py
--rw-r--r--   0        0        0    47165 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_raw/pw.py
--rw-r--r--   0        0        0     1890 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_raw/pw2gw.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/__init__.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/cp/__init__.py
--rw-r--r--   0        0        0    17305 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/cp/legacy.py
--rw-r--r--   0        0        0      309 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/exceptions.py
--rw-r--r--   0        0        0    21297 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/legacy.py
--rw-r--r--   0        0        0    24260 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/parse.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/pw/__init__.py
--rw-r--r--   0        0        0    16555 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/pw/legacy.py
--rw-r--r--   0        0        0      906 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/pw/parse.py
--rw-r--r--   0        0        0    39103 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes-1.0.xsd
--rw-r--r--   0        0        0    42863 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_030920.xsd
--rw-r--r--   0        0        0    41033 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_190304.xsd
--rw-r--r--   0        0        0    41135 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_191206.xsd
--rw-r--r--   0        0        0    42863 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_200420.xsd
--rw-r--r--   0        0        0    42863 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_210716.xsd
--rw-r--r--   0        0        0    49711 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_211101.xsd
--rw-r--r--   0        0        0    57806 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_220603.xsd
--rw-r--r--   0        0        0     4492 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/versions.py
--rw-r--r--   0        0        0     3119 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/ph.py
--rw-r--r--   0        0        0    15908 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/pp.py
--rw-r--r--   0        0        0    20459 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/projwfc.py
--rw-r--r--   0        0        0    27069 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/pw.py
--rw-r--r--   0        0        0     4210 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/pw2gw.py
--rw-r--r--   0        0        0     1316 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/pw2wannier90.py
--rw-r--r--   0        0        0     1250 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/q2r.py
--rw-r--r--   0        0        0    11344 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/xspectra.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/tools/__init__.py
--rw-r--r--   0        0        0     2840 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/tools/base.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/tools/calculations/__init__.py
--rw-r--r--   0        0        0     2288 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/tools/calculations/pw.py
--rw-r--r--   0        0        0     1035 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/tools/cpinputparser.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/tools/data/__init__.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/tools/data/orbital/__init__.py
--rw-r--r--   0        0        0     2981 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/tools/data/orbital/noncollinearhydrogen.py
--rw-r--r--   0        0        0     5427 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/tools/data/orbital/spinorbithydrogen.py
--rw-r--r--   0        0        0     6586 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/tools/pwinputparser.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/__init__.py
--rw-r--r--   0        0        0     3972 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/bands.py
--rw-r--r--   0        0        0     8343 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/convert.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/defaults/__init__.py
--rw-r--r--   0        0        0      610 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/defaults/calculation/__init__.py
--rw-r--r--   0        0        0     1032 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/linalg.py
--rw-r--r--   0        0        0     3672 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/mapping.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/protocols/__init__.py
--rw-r--r--   0        0        0    10193 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/protocols/pw.py
--rw-r--r--   0        0        0    14855 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/protocols/sssp_efficiency_1.0.json
--rw-r--r--   0        0        0    15000 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/protocols/sssp_efficiency_1.1.json
--rw-r--r--   0        0        0    14831 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/protocols/sssp_precision_1.0.json
--rw-r--r--   0        0        0    15000 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/protocols/sssp_precision_1.1.json
--rw-r--r--   0        0        0     9610 2023-02-02 21:57:30.027762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/resources.py
--rw-r--r--   0        0        0     2615 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/restart.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/validation/__init__.py
--rw-r--r--   0        0        0     3995 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/validation/trajectory.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/__init__.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/functions/__init__.py
--rw-r--r--   0        0        0      671 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/functions/create_kpoints_from_distance.py
--rw-r--r--   0        0        0      665 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/functions/seekpath_structure_analysis.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/matdyn/__init__.py
--rw-r--r--   0        0        0     2682 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/matdyn/base.py
--rw-r--r--   0        0        0    26001 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/pdos.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/ph/__init__.py
--rw-r--r--   0        0        0    11157 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/ph/base.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/protocols/__init__.py
--rw-r--r--   0        0        0     1125 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/protocols/core_hole_treatments.yaml
--rw-r--r--   0        0        0     1469 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/protocols/magnetization.yaml
--rw-r--r--   0        0        0     1982 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/protocols/pdos.yaml
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/protocols/ph/__init__.py
--rw-r--r--   0        0        0     1063 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/protocols/ph/base.yaml
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/protocols/pw/__init__.py
--rw-r--r--   0        0        0      631 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/protocols/pw/bands.yaml
--rw-r--r--   0        0        0     1803 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/protocols/pw/base.yaml
--rw-r--r--   0        0        0      839 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/protocols/pw/relax.yaml
--rw-r--r--   0        0        0     5838 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/protocols/utils.py
--rw-r--r--   0        0        0     1891 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/protocols/xspectra/base.yaml
--rw-r--r--   0        0        0      656 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/protocols/xspectra/core.yaml
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/pw/__init__.py
--rw-r--r--   0        0        0    16896 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/pw/bands.py
--rw-r--r--   0        0        0    33955 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/pw/base.py
--rw-r--r--   0        0        0    17980 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/pw/relax.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/q2r/__init__.py
--rw-r--r--   0        0        0     2649 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/q2r/base.py
--rw-r--r--   0        0        0        0 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/xspectra/__init__.py
--rw-r--r--   0        0        0    12841 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/xspectra/base.py
--rw-r--r--   0        0        0    34590 2023-02-02 21:57:30.031762 aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/xspectra/core.py
--rw-r--r--   0        0        0    31555 1970-01-01 00:00:00.000000 aiida-quantumespresso-4.2.0/PKG-INFO
+-rw-r--r--   0        0        0      148 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.github/config/code-ph.yaml
+-rw-r--r--   0        0        0      148 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.github/config/code-pw.yaml
+-rw-r--r--   0        0        0       43 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.github/config/localhost-config.yaml
+-rw-r--r--   0        0        0      234 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.github/config/localhost-setup.yaml
+-rw-r--r--   0        0        0      215 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.github/config/profile.yaml
+-rw-r--r--   0        0        0     1922 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.github/scripts/run_documentation_scripts.py
+-rw-r--r--   0        0        0     3009 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.github/workflows/cd.yml
+-rw-r--r--   0        0        0     4135 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.github/workflows/ci.yml
+-rw-r--r--   0        0        0     2291 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.github/workflows/nightly.yml
+-rw-r--r--   0        0        0     1520 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.github/workflows/validate_release_tag.py
+-rw-r--r--   0        0        0     1303 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.gitignore
+-rw-r--r--   0        0        0     1347 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      239 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/.readthedocs.yml
+-rw-r--r--   0        0        0    36108 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1273 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/LICENSE.txt
+-rw-r--r--   0        0        0    30387 2023-04-27 14:23:52.750428 aiida-quantumespresso-4.3.0/README.md
+-rw-r--r--   0        0        0     8567 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/pyproject.toml
+-rw-r--r--   0        0        0      100 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/__init__.py
+-rw-r--r--   0        0        0    39136 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/__init__.py
+-rw-r--r--   0        0        0     2017 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/base.py
+-rw-r--r--   0        0        0     6658 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/cp.py
+-rw-r--r--   0        0        0     1539 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/dos.py
+-rw-r--r--   0        0        0    14015 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/epw.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/__init__.py
+-rw-r--r--   0        0        0     1595 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/create_kpoints_from_distance.py
+-rw-r--r--   0        0        0     1226 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/merge_ph_outputs.py
+-rw-r--r--   0        0        0     1436 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/seekpath_structure_analysis.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/xspectra/__init__.py
+-rw-r--r--   0        0        0     4593 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/xspectra/get_powder_spectrum.py
+-rw-r--r--   0        0        0     4251 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/xspectra/get_spectra_by_element.py
+-rw-r--r--   0        0        0     5358 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/xspectra/get_xps_spectra.py
+-rw-r--r--   0        0        0     2624 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/xspectra/merge_spectra.py
+-rw-r--r--   0        0        0    84796 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.1.xml
+-rw-r--r--   0        0        0    87073 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.2.xml
+-rw-r--r--   0        0        0    87073 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.3.xml
+-rw-r--r--   0        0        0    83767 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.xml
+-rw-r--r--   0        0        0    96224 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.1.xml
+-rw-r--r--   0        0        0    96319 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.2.xml
+-rw-r--r--   0        0        0    93230 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.xml
+-rw-r--r--   0        0        0    96763 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.2.0.xml
+-rw-r--r--   0        0        0    97862 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.2.1.xml
+-rw-r--r--   0        0        0    97871 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.3.0.xml
+-rw-r--r--   0        0        0    98698 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.4.0.xml
+-rw-r--r--   0        0        0   109373 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.0.xml
+-rw-r--r--   0        0        0   110988 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.1.xml
+-rw-r--r--   0        0        0   112295 2023-04-27 14:23:52.758428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.2.xml
+-rw-r--r--   0        0        0   116180 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.3.xml
+-rw-r--r--   0        0        0   118149 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.4.xml
+-rw-r--r--   0        0        0    26623 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/__init__.py
+-rw-r--r--   0        0        0     4732 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/matdyn.py
+-rw-r--r--   0        0        0    10109 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/namelists.py
+-rw-r--r--   0        0        0    17188 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/neb.py
+-rw-r--r--   0        0        0     2058 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/open_grid.py
+-rw-r--r--   0        0        0    16652 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/ph.py
+-rw-r--r--   0        0        0    11374 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/pp.py
+-rw-r--r--   0        0        0     3843 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/projwfc.py
+-rw-r--r--   0        0        0    14592 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/pw.py
+-rw-r--r--   0        0        0     3578 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/pw2gw.py
+-rw-r--r--   0        0        0     3052 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/pw2wannier90.py
+-rw-r--r--   0        0        0    23331 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/pwimmigrant.py
+-rw-r--r--   0        0        0     1948 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/q2r.py
+-rw-r--r--   0        0        0     6062 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/xspectra.py
+-rw-r--r--   0        0        0      609 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/__init__.py
+-rw-r--r--   0        0        0      874 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/__init__.py
+-rw-r--r--   0        0        0     2130 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/cp.py
+-rwxr-xr-x   0        0        0     1992 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/dos.py
+-rw-r--r--   0        0        0     3530 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/epw.py
+-rw-r--r--   0        0        0     1418 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/matdyn.py
+-rw-r--r--   0        0        0     3622 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/neb.py
+-rw-r--r--   0        0        0     2118 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/ph.py
+-rw-r--r--   0        0        0     1981 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/pp.py
+-rwxr-xr-x   0        0        0     2012 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/projwfc.py
+-rw-r--r--   0        0        0     4121 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/pw.py
+-rwxr-xr-x   0        0        0     3060 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/pw2wannier90.py
+-rw-r--r--   0        0        0     1794 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/q2r.py
+-rw-r--r--   0        0        0      361 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/data/__init__.py
+-rw-r--r--   0        0        0     1062 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/data/structure.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/utils/__init__.py
+-rw-r--r--   0        0        0     1555 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/utils/defaults.py
+-rw-r--r--   0        0        0     1530 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/utils/display.py
+-rw-r--r--   0        0        0     1259 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/utils/launch.py
+-rw-r--r--   0        0        0     6820 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/utils/options.py
+-rw-r--r--   0        0        0     5435 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/utils/validate.py
+-rw-r--r--   0        0        0      675 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/matdyn/__init__.py
+-rwxr-xr-x   0        0        0     1666 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/matdyn/base.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/ph/__init__.py
+-rwxr-xr-x   0        0        0     1568 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/ph/base.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/pw/__init__.py
+-rwxr-xr-x   0        0        0     3526 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/pw/bands.py
+-rwxr-xr-x   0        0        0     2720 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/pw/base.py
+-rwxr-xr-x   0        0        0     3408 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/pw/relax.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/q2r/__init__.py
+-rwxr-xr-x   0        0        0     1720 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/q2r/base.py
+-rw-r--r--   0        0        0       84 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/common/__init__.py
+-rw-r--r--   0        0        0     6183 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/common/hubbard.py
+-rw-r--r--   0        0        0     1588 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/common/types.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/data/__init__.py
+-rw-r--r--   0        0        0     9253 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/data/force_constants.py
+-rw-r--r--   0        0        0     9221 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/data/hubbard_structure.py
+-rw-r--r--   0        0        0      202 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/__init__.py
+-rw-r--r--   0        0        0     2474 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/base.py
+-rw-r--r--   0        0        0    16768 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/cp.py
+-rw-r--r--   0        0        0     5575 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/dos.py
+-rw-r--r--   0        0        0     4778 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/matdyn.py
+-rw-r--r--   0        0        0    10493 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/neb.py
+-rw-r--r--   0        0        0     3061 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/open_grid.py
+-rw-r--r--   0        0        0       71 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_raw/__init__.py
+-rw-r--r--   0        0        0     6752 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_raw/base.py
+-rw-r--r--   0        0        0     8844 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_raw/cp.py
+-rw-r--r--   0        0        0    10943 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_raw/neb.py
+-rw-r--r--   0        0        0    20682 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_raw/ph.py
+-rw-r--r--   0        0        0    48436 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_raw/pw.py
+-rw-r--r--   0        0        0     1890 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_raw/pw2gw.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/cp/__init__.py
+-rw-r--r--   0        0        0    17305 2023-04-27 14:23:52.762428 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/cp/legacy.py
+-rw-r--r--   0        0        0      291 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/exceptions.py
+-rw-r--r--   0        0        0    21297 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/legacy.py
+-rw-r--r--   0        0        0    24260 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/parse.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/pw/__init__.py
+-rw-r--r--   0        0        0    16555 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/pw/legacy.py
+-rw-r--r--   0        0        0      906 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/pw/parse.py
+-rw-r--r--   0        0        0    39204 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes-1.0.xsd
+-rw-r--r--   0        0        0    42964 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_030920.xsd
+-rw-r--r--   0        0        0    41134 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_190304.xsd
+-rw-r--r--   0        0        0    41234 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_191206.xsd
+-rw-r--r--   0        0        0    42964 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_200420.xsd
+-rw-r--r--   0        0        0    42964 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_210716.xsd
+-rw-r--r--   0        0        0    49812 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_211101.xsd
+-rw-r--r--   0        0        0    57907 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_220603.xsd
+-rw-r--r--   0        0        0    58917 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_230310.xsd
+-rw-r--r--   0        0        0     4627 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/versions.py
+-rw-r--r--   0        0        0     3110 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/ph.py
+-rw-r--r--   0        0        0    15908 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/pp.py
+-rw-r--r--   0        0        0    20459 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/projwfc.py
+-rw-r--r--   0        0        0    29470 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/pw.py
+-rw-r--r--   0        0        0     4210 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/pw2gw.py
+-rw-r--r--   0        0        0     1316 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/pw2wannier90.py
+-rw-r--r--   0        0        0     1250 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/q2r.py
+-rw-r--r--   0        0        0    11344 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/xspectra.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/__init__.py
+-rw-r--r--   0        0        0     2840 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/base.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/calculations/__init__.py
+-rw-r--r--   0        0        0     2288 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/calculations/pw.py
+-rw-r--r--   0        0        0     1035 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/cpinputparser.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/data/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/data/orbital/__init__.py
+-rw-r--r--   0        0        0     2981 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/data/orbital/noncollinearhydrogen.py
+-rw-r--r--   0        0        0     5427 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/data/orbital/spinorbithydrogen.py
+-rw-r--r--   0        0        0     6586 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/pwinputparser.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/__init__.py
+-rw-r--r--   0        0        0     3972 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/bands.py
+-rw-r--r--   0        0        0     8343 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/convert.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/defaults/__init__.py
+-rw-r--r--   0        0        0      610 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/defaults/calculation/__init__.py
+-rw-r--r--   0        0        0    15021 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/hubbard.py
+-rw-r--r--   0        0        0     1032 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/linalg.py
+-rw-r--r--   0        0        0     3672 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/mapping.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/protocols/__init__.py
+-rw-r--r--   0        0        0    10193 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/protocols/pw.py
+-rw-r--r--   0        0        0    14855 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/protocols/sssp_efficiency_1.0.json
+-rw-r--r--   0        0        0    15000 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/protocols/sssp_efficiency_1.1.json
+-rw-r--r--   0        0        0    14831 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/protocols/sssp_precision_1.0.json
+-rw-r--r--   0        0        0    15000 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/protocols/sssp_precision_1.1.json
+-rw-r--r--   0        0        0     3050 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/resources.py
+-rw-r--r--   0        0        0     2615 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/restart.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/validation/__init__.py
+-rw-r--r--   0        0        0     5337 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/validation/trajectory.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/__init__.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/functions/__init__.py
+-rw-r--r--   0        0        0      671 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/functions/create_kpoints_from_distance.py
+-rw-r--r--   0        0        0    15977 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/functions/get_xspectra_structures.py
+-rw-r--r--   0        0        0      665 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/functions/seekpath_structure_analysis.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/matdyn/__init__.py
+-rw-r--r--   0        0        0     2682 2023-04-27 14:23:52.766429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/matdyn/base.py
+-rw-r--r--   0        0        0    26001 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/pdos.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/ph/__init__.py
+-rw-r--r--   0        0        0    13101 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/ph/base.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/__init__.py
+-rw-r--r--   0        0        0     1125 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/core_hole_treatments.yaml
+-rw-r--r--   0        0        0     1469 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/magnetization.yaml
+-rw-r--r--   0        0        0     1983 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/pdos.yaml
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/ph/__init__.py
+-rw-r--r--   0        0        0     1064 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/ph/base.yaml
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/pw/__init__.py
+-rw-r--r--   0        0        0     1045 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/pw/bands.yaml
+-rw-r--r--   0        0        0     1804 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/pw/base.yaml
+-rw-r--r--   0        0        0      840 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/pw/relax.yaml
+-rw-r--r--   0        0        0     5838 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/utils.py
+-rw-r--r--   0        0        0      538 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/xps.yaml
+-rw-r--r--   0        0        0     1892 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/xspectra/base.yaml
+-rw-r--r--   0        0        0      657 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/xspectra/core.yaml
+-rw-r--r--   0        0        0      599 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/xspectra/crystal.yaml
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/pw/__init__.py
+-rw-r--r--   0        0        0    16503 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/pw/bands.py
+-rw-r--r--   0        0        0    30947 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/pw/base.py
+-rw-r--r--   0        0        0    18141 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/pw/relax.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/q2r/__init__.py
+-rw-r--r--   0        0        0     2649 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/q2r/base.py
+-rw-r--r--   0        0        0    30756 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/xps.py
+-rw-r--r--   0        0        0        0 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/xspectra/__init__.py
+-rw-r--r--   0        0        0    12841 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/xspectra/base.py
+-rw-r--r--   0        0        0    34623 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/xspectra/core.py
+-rw-r--r--   0        0        0    30297 2023-04-27 14:23:52.770429 aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/xspectra/crystal.py
+-rw-r--r--   0        0        0    32371 1970-01-01 00:00:00.000000 aiida-quantumespresso-4.3.0/PKG-INFO
```

### Comparing `aiida-quantumespresso-4.2.0/.github/scripts/run_documentation_scripts.py` & `aiida-quantumespresso-4.3.0/.github/scripts/run_documentation_scripts.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/.github/workflows/cd.yml` & `aiida-quantumespresso-4.3.0/.github/workflows/cd.yml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/.github/workflows/ci.yml` & `aiida-quantumespresso-4.3.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/.github/workflows/nightly.yml` & `aiida-quantumespresso-4.3.0/.github/workflows/nightly.yml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/.github/workflows/validate_release_tag.py` & `aiida-quantumespresso-4.3.0/.github/workflows/validate_release_tag.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/.gitignore` & `aiida-quantumespresso-4.3.0/.gitignore`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/.pre-commit-config.yaml` & `aiida-quantumespresso-4.3.0/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -35,19 +35,21 @@
                 src/aiida_quantumespresso/calculations/pwimmigrant.*|
                 src/aiida_quantumespresso/parsers/.*|
                 docs/.*|
                 tests/.*(?<!\.py)$
             )$
         additional_dependencies: ['toml']
 
--   repo: https://github.com/PyCQA/pylint
-    rev: v2.12.2
+-   repo: local
     hooks:
     -   id: pylint
+        name: pylint
+        entry: pylint
         language: system
+        types: [python]
         exclude: *exclude_files
 
 -   repo: https://github.com/PyCQA/pydocstyle
     rev: '6.1.1'
     hooks:
     -   id: pydocstyle
         exclude: *exclude_files
```

### Comparing `aiida-quantumespresso-4.2.0/CHANGELOG.md` & `aiida-quantumespresso-4.3.0/CHANGELOG.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,79 @@
+## v4.3.0
+
+Release version `4.3.0` comes with a lot of new features, improvements and bug fixes.
+Although this is technically a minor release, this new version does come with some _minor_ breaking changes:
+
+* The default value of `clean_workdir` was changed from `True` to `False`.
+* The `automatic_parallelization` feature of the `PwBaseWorkChain` was removed, as this was badly broken with no clear path to fixing it. Moreover, [v7.1 of Quantum ESPRESSO](https://gitlab.com/QEF/q-e/-/releases/qe-7.1) has implemented some basic automated parallelization for `pw.x` when no parallelization flags are specified.
+
+Support for Quantum ESPRESSO v7.2 `pw.x` parsing was added, as well as the `HubbardStructureData` data plugin and corresponding implementation in the `PwCalculation` plugin to support the [new input syntax for using Hubbard corrections](https://gitlab.com/QEF/q-e/-/releases/qe-7.1#incompatible-changes-in-71-version) in the `pw.x` code.
+
+For `ph.x`, the symmetry labels printed in the `stdout` after the mode frequencies are now parsed for each q-point.
+In the case of restarts in the `PhBaseWorkChain`, care has been taken to properly parse these symmetry labels from the separate output files and merge them, so the `output_parameters` are the same with or without restarts.
+
+The `XpsWorkChain` has been added to compute the XPS spectra using core-hole pseudo potentials and the `pw.x` code. The work chain can handle both molecules and crystals. The chemical shifts, as well as the cole-level binding energy can be obtained.
+
+Finally, improved error handling for the `PwBaseWorkChain` was implemented for several typical failure modes of the `pw.x` code, and the `CRASH` file is now also retrieved, as this will be the default location of error messages from Quantum ESPRESSO v7.2 onwards.
+
+### ‼️ Breaking changes
+
+* Protocols: Set `clean_workdir` default to `False` [[f8e512f](https://github.com/aiidateam/aiida-quantumespresso/commit/f8e512f9cb5404d702aa1d721e2369c7257f977f)]
+* `PwBaseWorkChain`: Remove `automatic_parallelization` input [[5cae75f](https://github.com/aiidateam/aiida-quantumespresso/commit/5cae75ff671268dc1e5684e1c84f801a10839e0b)]
+
+### ✨ New features
+
+* `PwBaseWorkChain`: Add `ERROR_IONIC_INTERRUPTED_PARTIAL_TRAJECTORY` handler [[9291f84](https://github.com/aiidateam/aiida-quantumespresso/commit/9291f841445800fa2b38d97b6957e98a2818b624)]
+* `PwCalculation`: Add exit code and handler for `scale_h` error [[d350d7e](https://github.com/aiidateam/aiida-quantumespresso/commit/d350d7eb5b7bfcf4682ee8f635c721708be1d1d7)]
+* `PwParser`: Add retrieval and parsing of `CRASH` file [[7f53c96](https://github.com/aiidateam/aiida-quantumespresso/commit/7f53c96bf744ed622fe7b1d13b0f7e9198ed5656)]
+* Add the `HubbardStructureData` data plugin [[355020c](https://github.com/aiidateam/aiida-quantumespresso/commit/355020ca9ea63db0803ecc5746f93a879f488696)]
+* `PwParser`: Add support for QE v7.2 [[57f5f8f](https://github.com/aiidateam/aiida-quantumespresso/commit/57f5f8ffa359ed5f5d937c43ae1f53cbc55eb314)]
+* `PhParser`: parse symmetry labels from the `stdout` of `ph.x` [[8a9950a](https://github.com/aiidateam/aiida-quantumespresso/commit/8a9950aa870a26badb24b572910f7b8526236f37)]
+* Add Feature: `XpsWorkChain` [[a9d124e](https://github.com/aiidateam/aiida-quantumespresso/commit/a9d124e2cfa5a5a5891affbe40515d38d1dd3913)]
+* Add Feature: `XspectraCrystalWorkChain` [[01e7593](https://github.com/aiidateam/aiida-quantumespresso/commit/01e759319552645072b7a89dd0347225ab14d635)]
+* Add `OpenGridCalculation` [[361ff04](https://github.com/aiidateam/aiida-quantumespresso/commit/361ff0413659b23f895747e04f8448f574811958)]
+* Feature/get xspectra structures [[bc63d56](https://github.com/aiidateam/aiida-quantumespresso/commit/bc63d5661a6e79e3cf599ada3fdfc8eb3cb8193d)]
+
+### 👌 Improvements
+
+* ``PwBaseWorkChain``: improve diagonalization handler [[cc29488](https://github.com/aiidateam/aiida-quantumespresso/commit/cc29488c9e450bac5af7d28ee3f79ab8bcb01b6a)]
+* `PwCalculation`: Add `ERROR_IONIC_INTERRUPTED_PARTIAL_TRAJECTORY` code [[92a6c6f](https://github.com/aiidateam/aiida-quantumespresso/commit/92a6c6fb00c02ace0f8afc0d06d8f938a0e2d221)]
+* `PwParser`: Keep scheduler parser error unless more specific available [[b8d6a3a](https://github.com/aiidateam/aiida-quantumespresso/commit/b8d6a3a489c8d24a06cfc58956a97b121ad92316)]
+* Protocols: consider `pbc` of `StructureData` [[ef21642](https://github.com/aiidateam/aiida-quantumespresso/commit/ef21642ba8c715b384e726628f866f7a3df63890)]
+* CLI: Simplify `cli.utils.validate_hubbard_parameters` and add tests [[74d25d1](https://github.com/aiidateam/aiida-quantumespresso/commit/74d25d1782cddb2801781999e6c708191f1cdae7)]
+* `PwCalculation`: Add exit codes, mostly related to diagonalization [[159b83e](https://github.com/aiidateam/aiida-quantumespresso/commit/159b83e5a96db258697fa821b48746adfbacd2ad)]
+* `PwParser`: Include path in exception when XML schema not found [[56fdb57](https://github.com/aiidateam/aiida-quantumespresso/commit/56fdb57643fa44e7bcff82640d9cbcb26f7759b3)]
+
+### 🐛 Bug Fixes
+
+* `PwCalculation`: Fix restart validation for `nscf`/`bands` [[29a0dfa](https://github.com/aiidateam/aiida-quantumespresso/commit/29a0dfa3257863f73de17a0347dfa578da5d292e)]
+* `PwParser`: Correct the `disk_io` type for all XML schemas [[89d39a4](https://github.com/aiidateam/aiida-quantumespresso/commit/89d39a47d4eae0f9b39ef93fe07404a5102c6ee7)]
+* `PwParser`: Fix trajectory verification for `fixed_coords` [[105670f](https://github.com/aiidateam/aiida-quantumespresso/commit/105670fd145c572213bb750069679ef6fca7a80d)]
+* `XspectraCoreWorkChain`: Ensure `overrides` respected in `get_builder_from_protocol()` [[7b2d701](https://github.com/aiidateam/aiida-quantumespresso/commit/7b2d701cb7f61719efa5a14f762b8f85078fb4dd)]
+* `PhCalculation`: Fix exception when `parent_folder` is on different computer [[24b3779](https://github.com/aiidateam/aiida-quantumespresso/commit/24b3779e0df2d30378898f89dd884b69593218e9)]
+
+### 📚 Documentation
+
+* Fix the intersphinx URL of the AiiDA documentation [[08532d8](https://github.com/aiidateam/aiida-quantumespresso/commit/08532d8f69d87bd1853bb2a9010854efbc6bbaee)]
+* `README.md`: Fix Build Status badge to point to `ci` action [[1e9c345](https://github.com/aiidateam/aiida-quantumespresso/commit/1e9c3454174807e115f48eb7667f928680a11dfc)]
+* Add developer section to README [[146bc57](https://github.com/aiidateam/aiida-quantumespresso/commit/146bc57d74b76a11d7205a0f8449ae39c7675110)]
+
+### 🔧 Maintenance
+
+* DevOps: Symlink `CRASH` and `data-file.xml` files, and reduce fixture file contents [[0a48533](https://github.com/aiidateam/aiida-quantumespresso/commit/0a48533f40e276e5423428e0ca9745bd0b789121)]
+
+### ⬆️ Update dependencies
+* Symlink `CRASH` and `data-file.xml` files, and reduce fixture file contents [[0a48533](https://github.com/aiidateam/aiida-quantumespresso/commit/0a48533f40e276e5423428e0ca9745bd0b789121)]
+* Devops: Update `pylint` version [[9f4142d](https://github.com/aiidateam/aiida-quantumespresso/commit/9f4142d4713b0d1c32042b3ca35905d725954bf4)]
+
+### ♻️ Refactor
+* Update `pylint` version [[9f4142d](https://github.com/aiidateam/aiida-quantumespresso/commit/9f4142d4713b0d1c32042b3ca35905d725954bf4)]
+* Protocols: Move all static work chain inputs to protocol [[01f1470](https://github.com/aiidateam/aiida-quantumespresso/commit/01f14701e6846338f84db25bf7e654fcdfb6f927)]
+
+
 ## v4.2.0
 
 ### Features
 - Add the `XspectraBaseWorkChain` [[#854]](https://github.com/aiidateam/aiida-quantumespresso/pull/854)
 - Add the `XspectraCoreWorkChain` [[#872]](https://github.com/aiidateam/aiida-quantumespresso/pull/872)
 
 ### Changes
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aiida-quantumespresso-4.2.0/LICENSE.txt` & `aiida-quantumespresso-4.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/README.md` & `aiida-quantumespresso-4.3.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # `aiida-quantumespresso`
 [![PyPI version](https://badge.fury.io/py/aiida-quantumespresso.svg)](https://badge.fury.io/py/aiida-quantumespresso)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-quantumespresso.svg)](https://pypi.python.org/pypi/aiida-quantumespresso)
-[![Build Status](https://github.com/aiidateam/aiida-quantumespresso/workflows/aiida-quantumespresso/badge.svg?branch=develop&event=push)](https://github.com/aiidateam/aiida-quantumespresso/actions)
+[![Build Status](https://github.com/aiidateam/aiida-quantumespresso/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/aiidateam/aiida-quantumespresso/actions)
 [![Docs status](https://readthedocs.org/projects/aiida-quantumespresso/badge)](http://aiida-quantumespresso.readthedocs.io/)
 
 This is the official AiiDA plugin for [Quantum ESPRESSO](https://www.quantum-espresso.org/).
 
 ## Compatibility matrix
 
 The matrix below assumes the user always install the latest patch release of the specified minor version, which is recommended.
@@ -82,20 +82,46 @@
 
     aiida-pseudo install sssp
 
 to install the default SSSP version.
 List the installed pseudopotential families with the command `aiida-pseudo list`.
 You can then use the name of any family in the command line using the `-F` flag.
 
+## Development
+
+### Running tests
+To run the tests, simply clone and install the package locally with the [tests] optional dependencies:
+
+```shell
+git clone https://github.com/aiidateam/aiida-quantumespresso .
+cd aiida-quantumespresso
+pip install -e .[tests]  # install extra dependencies for test
+pytest # run tests
+```
+
+You can also use `tox` to run the test set. Here you can also use the `-e` option to specify the Python version for the test run:
+```shell
+pip install tox
+tox -e py39 -- tests/calculations/test_pw.py
+```
+
+### Pre-commit
+To contribute to this repository, please enable pre-commit so the code in commits are conform to the standards.
+Simply install the repository with the `pre-commit` extra dependencies:
+```shell
+cd aiida-quantumespresso
+pip install -e .[pre-commit]
+pre-commit install
+```
 
 ## License
 The `aiida-quantumespresso` plugin package is released under the MIT license.
 See the `LICENSE.txt` file for more details.
 
-## Acknowlegements
+## Acknowledgements
 We acknowledge support from:
 * the [NCCR MARVEL](http://nccr-marvel.ch/) funded by the Swiss National Science Foundation;
 * the EU Centre of Excellence "[MaX – Materials Design at the Exascale](http://www.max-centre.eu/)" (Horizon 2020 EINFRA-5, Grant No. 676598; H2020-INFRAEDI-2018-1, Grant No. 824143; HORIZON-EUROHPC-JU-2021-COE-1, Grant No. 101093324);
 * the European Union's Horizon 2020 research and innovation programme (Grant No. 957189, [project BIG-MAP](https://www.big-map.eu), also part of the [BATTERY 2030+ initiative](https://battery2030.eu), Grant No. 957213);
 * the [swissuniversities P-5 project "Materials Cloud"](https://www.materialscloud.org/swissuniversities).
 
 <img src="https://raw.githubusercontent.com/aiidateam/aiida-quantumespresso/develop/docs/source/images/MARVEL.png" width="250px" height="131px"/>
```

### Comparing `aiida-quantumespresso-4.2.0/pyproject.toml` & `aiida-quantumespresso-4.3.0/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -18,20 +18,21 @@
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
     'Programming Language :: Python :: 3.11',
 ]
 keywords = ['aiida', 'workflows']
 requires-python = '>=3.8'
 dependencies = [
-    'aiida_core[atomic_tools]~=2.1',
+    'aiida_core[atomic_tools]~=2.3',
     'aiida-pseudo~=1.0',
     'click~=8.0',
     'importlib_resources',
     'jsonschema',
     'numpy',
+    'pydantic',
     'packaging',
     'qe-tools~=2.0',
     'xmlschema~=1.2,>=1.2.5'
 ]
 
 [project.urls]
 Home = 'https://github.com/aiidateam/aiida-quantumespresso'
@@ -46,15 +47,15 @@
     'sphinx-click~=4.0',
     'sphinx-design~=0.0.13',
     'sphinxcontrib-details-directive~=0.1.0',
     'sphinx-autoapi',
 ]
 pre-commit = [
     'pre-commit~=2.17',
-    'pylint~=2.12.2',
+    'pylint~=2.17.2',
     'pylint-aiida~=0.1.1',
     'toml',
 ]
 tests = [
     'pgtest~=1.3',
     'pytest~=6.0',
     'pytest-regressions~=2.3'
@@ -62,14 +63,15 @@
 
 [project.scripts]
 aiida-quantumespresso = 'aiida_quantumespresso.cli:cmd_root'
 
 [project.entry-points.'aiida.calculations']
 'quantumespresso.cp' = 'aiida_quantumespresso.calculations.cp:CpCalculation'
 'quantumespresso.create_kpoints_from_distance' = 'aiida_quantumespresso.calculations.functions.create_kpoints_from_distance:create_kpoints_from_distance'
+'quantumespresso.merge_ph_outputs' = 'aiida_quantumespresso.calculations.functions.merge_ph_outputs:merge_ph_outputs'
 'quantumespresso.dos' = 'aiida_quantumespresso.calculations.dos:DosCalculation'
 'quantumespresso.epw' = 'aiida_quantumespresso.calculations.epw:EpwCalculation'
 'quantumespresso.matdyn' = 'aiida_quantumespresso.calculations.matdyn:MatdynCalculation'
 'quantumespresso.namelists' = 'aiida_quantumespresso.calculations.namelists:NamelistsCalculation'
 'quantumespresso.neb' = 'aiida_quantumespresso.calculations.neb:NebCalculation'
 'quantumespresso.ph' = 'aiida_quantumespresso.calculations.ph:PhCalculation'
 'quantumespresso.pp' = 'aiida_quantumespresso.calculations.pp:PpCalculation'
@@ -77,31 +79,34 @@
 'quantumespresso.pw' = 'aiida_quantumespresso.calculations.pw:PwCalculation'
 'quantumespresso.pw2gw' = 'aiida_quantumespresso.calculations.pw2gw:Pw2gwCalculation'
 'quantumespresso.pw2wannier90' = 'aiida_quantumespresso.calculations.pw2wannier90:Pw2wannier90Calculation'
 'quantumespresso.pwimmigrant' = 'aiida_quantumespresso.calculations.pwimmigrant:PwimmigrantCalculation'
 'quantumespresso.q2r' = 'aiida_quantumespresso.calculations.q2r:Q2rCalculation'
 'quantumespresso.seekpath_structure_analysis' = 'aiida_quantumespresso.calculations.functions.seekpath_structure_analysis:seekpath_structure_analysis'
 'quantumespresso.xspectra' = 'aiida_quantumespresso.calculations.xspectra:XspectraCalculation'
+'quantumespresso.open_grid' = 'aiida_quantumespresso.calculations.open_grid:OpenGridCalculation'
 
 [project.entry-points.'aiida.data']
 'quantumespresso.force_constants' = 'aiida_quantumespresso.data.force_constants:ForceConstantsData'
+'quantumespresso.hubbard_structure' = 'aiida_quantumespresso.data.hubbard_structure:HubbardStructureData'
 
 [project.entry-points.'aiida.parsers']
 'quantumespresso.cp' = 'aiida_quantumespresso.parsers.cp:CpParser'
 'quantumespresso.dos' = 'aiida_quantumespresso.parsers.dos:DosParser'
 'quantumespresso.matdyn' = 'aiida_quantumespresso.parsers.matdyn:MatdynParser'
 'quantumespresso.neb' = 'aiida_quantumespresso.parsers.neb:NebParser'
 'quantumespresso.ph' = 'aiida_quantumespresso.parsers.ph:PhParser'
 'quantumespresso.pp' = 'aiida_quantumespresso.parsers.pp:PpParser'
 'quantumespresso.projwfc' = 'aiida_quantumespresso.parsers.projwfc:ProjwfcParser'
 'quantumespresso.pw' = 'aiida_quantumespresso.parsers.pw:PwParser'
 'quantumespresso.pw2gw' = 'aiida_quantumespresso.parsers.pw2gw:Pw2gwParser'
 'quantumespresso.q2r' = 'aiida_quantumespresso.parsers.q2r:Q2rParser'
 'quantumespresso.pw2wannier90' = 'aiida_quantumespresso.parsers.pw2wannier90:Pw2wannier90Parser'
 'quantumespresso.xspectra' = 'aiida_quantumespresso.parsers.xspectra:XspectraParser'
+'quantumespresso.open_grid' = 'aiida_quantumespresso.parsers.open_grid:OpenGridParser'
 
 [project.entry-points.'aiida.tools.calculations']
 'quantumespresso.pw' = 'aiida_quantumespresso.tools.calculations.pw:PwCalculationTools'
 
 [project.entry-points.'aiida.tools.data.orbitals']
 'spinorbithydrogen' = 'aiida_quantumespresso.tools.data.orbital.spinorbithydrogen:SpinorbitHydrogenOrbital'
 'noncollinearhydrogen' = 'aiida_quantumespresso.tools.data.orbital.noncollinearhydrogen:NoncollinearHydrogenOrbital'
@@ -111,15 +116,17 @@
 'quantumespresso.pw.base' = 'aiida_quantumespresso.workflows.pw.base:PwBaseWorkChain'
 'quantumespresso.pw.relax' = 'aiida_quantumespresso.workflows.pw.relax:PwRelaxWorkChain'
 'quantumespresso.pw.bands' = 'aiida_quantumespresso.workflows.pw.bands:PwBandsWorkChain'
 'quantumespresso.q2r.base' = 'aiida_quantumespresso.workflows.q2r.base:Q2rBaseWorkChain'
 'quantumespresso.matdyn.base' = 'aiida_quantumespresso.workflows.matdyn.base:MatdynBaseWorkChain'
 'quantumespresso.pdos' = 'aiida_quantumespresso.workflows.pdos:PdosWorkChain'
 'quantumespresso.xspectra.base' = 'aiida_quantumespresso.workflows.xspectra.base:XspectraBaseWorkChain'
+'quantumespresso.xps' = 'aiida_quantumespresso.workflows.xps:XpsWorkChain'
 'quantumespresso.xspectra.core' = 'aiida_quantumespresso.workflows.xspectra.core:XspectraCoreWorkChain'
+'quantumespresso.xspectra.crystal' = 'aiida_quantumespresso.workflows.xspectra.crystal:XspectraCrystalWorkChain'
 
 [tool.flit.module]
 name = 'aiida_quantumespresso'
 
 [tool.flit.sdist]
 exclude = [
     'docs/',
@@ -141,35 +148,36 @@
     'D104',
     'D202',
     'D203',
     'D213'
 ]
 
 [tool.pylint.master]
-load-plugins = ['pylint_aiida']
+load-plugins = ['pylint_aiida','pylint.extensions.no_self_use']
 
 [tool.pylint.format]
 max-line-length = 120
 
 [tool.pylint.tool-check]
 generated-members = 'self.exit_codes.*'
 
 [tool.pylint.messages_control]
 disable = [
-    'bad-continuation',
     'duplicate-code',
-    'locally-disabled',
-    'logging-format-interpolation',
+    'fixme',
     'inconsistent-return-statements',
     'import-outside-toplevel',
+    'locally-disabled',
+    'logging-format-interpolation',
     'no-else-raise',
     'too-many-arguments',
     'too-many-ancestors',
     'too-many-branches',
     'too-many-locals',
+    'use-dict-literal',
 ]
 
 [tool.pylint.basic]
 good-names = [
     'i',
     'j',
     'k',
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/__init__.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 # -*- coding: utf-8 -*-
 """Base `CalcJob` for implementations for pw.x and cp.x of Quantum ESPRESSO."""
 import abc
 import copy
-from functools import partial
 import numbers
 import os
 from types import MappingProxyType
 import warnings
 
 from aiida import orm
-from aiida.common import datastructures, exceptions
+from aiida.common import AttributeDict, datastructures, exceptions
 from aiida.common.lang import classproperty
 from aiida.common.warnings import AiidaDeprecationWarning
 from aiida.plugins import DataFactory
+import numpy
 from qe_tools.converters import get_parameters_from_cell
 
+from aiida_quantumespresso.data.hubbard_structure import HubbardStructureData
 from aiida_quantumespresso.utils.convert import convert_input_to_namelist_entry
+from aiida_quantumespresso.utils.hubbard import HubbardUtils
 
 from .base import CalcJob
 from .helpers import QEInputValidationError
 
 LegacyUpfData = DataFactory('core.upf')
 UpfData = DataFactory('pseudo.upf')
 
@@ -28,14 +30,15 @@
     """Base `CalcJob` for implementations for pw.x and cp.x of Quantum ESPRESSO."""
 
     _PSEUDO_SUBFOLDER = './pseudo/'
     _OUTPUT_SUBFOLDER = './out/'
     _PREFIX = 'aiida'
     _DEFAULT_INPUT_FILE = 'aiida.in'
     _DEFAULT_OUTPUT_FILE = 'aiida.out'
+    _CRASH_FILE = 'CRASH'
     _DATAFILE_XML_PRE_6_2 = 'data-file.xml'
     _DATAFILE_XML_POST_6_2 = 'data-file-schema.xml'
     _ENVIRON_INPUT_FILE_NAME = 'environ.in'
     _DEFAULT_IBRAV = 0
 
     # A mapping {flag_name: help_string} of parallelization flags
     # possible in QE codes. The flags that are actually implemented in a
@@ -157,17 +160,39 @@
 
         structure_kinds = set(value['structure'].get_kind_names())
         pseudo_kinds = set(value['pseudos'].keys())
 
         if structure_kinds != pseudo_kinds:
             return f'The `pseudos` specified and structure kinds do not match: {pseudo_kinds} vs {structure_kinds}'
 
+        if 'settings' in value:
+            settings = _uppercase_dict(value['settings'].get_dict(), dict_name='settings')
+
+            # Validate the FIXED_COORDS setting
+            fixed_coords = settings.get('FIXED_COORDS', None)
+
+            if fixed_coords is not None:
+
+                fixed_coords = numpy.array(fixed_coords)
+
+                if len(fixed_coords.shape) != 2 or fixed_coords.shape[1] != 3:
+                    return 'The `fixed_coords` setting must be a list of lists with length 3.'
+
+                if fixed_coords.dtype != bool:
+                    return 'All elements in the `fixed_coords` setting lists must be either `True` or `False`.'
+
+                if 'structure' in value:
+                    nsites = len(value['structure'].sites)
+
+                    if len(fixed_coords) != nsites:
+                        return f'Input structure has {nsites} sites, but fixed_coords has length {len(fixed_coords)}'
+
     @classmethod
     def validate_parallelization(cls, value, _):
-        """Validate the ``parallelization`` port."""
+        """Validate the ``parallelization`` input."""
         if value:
             value_dict = value.get_dict()
             unknown_flags = set(value_dict.keys()) - set(cls._ENABLED_PARALLELIZATION_FLAGS)
             if unknown_flags:
                 return (
                     f"Unknown flags in 'parallelization': {unknown_flags}, "
                     f'allowed flags are {cls._ENABLED_PARALLELIZATION_FLAGS}.'
@@ -310,14 +335,15 @@
         calcinfo.local_copy_list = local_copy_list
         calcinfo.remote_copy_list = remote_copy_list
         calcinfo.remote_symlink_list = remote_symlink_list
 
         # Retrieve by default the output file and the xml file
         calcinfo.retrieve_list = []
         calcinfo.retrieve_list.append(self.metadata.options.output_filename)
+        calcinfo.retrieve_list.append(self._CRASH_FILE)
         calcinfo.retrieve_list.extend(self.xml_filepaths)
         calcinfo.retrieve_list += settings.pop('ADDITIONAL_RETRIEVE_LIST', [])
         calcinfo.retrieve_list += self._internal_retrieve_list
 
         # Retrieve the k-point directories with the xml files to the temporary folder
         # to parse the band eigenvalues and occupations but not to have to save the raw files
         # if and only if the 'no_bands' key was not set to true in the settings
@@ -488,62 +514,51 @@
         # list, with the order of species used in the file
         mapping_species, sorted_atomic_species_card_list = list(zip(*sorted(zip(kind_names, atomic_species_card_list))))
         # The format of mapping_species required later is a dictionary, whose
         # values are the indices, so I convert to this format
         # Note the (idx+1) to convert to fortran 1-based lists
         mapping_species = {sp_name: (idx + 1) for idx, sp_name in enumerate(mapping_species)}
         # I add the first line
-        sorted_atomic_species_card_list = (['ATOMIC_SPECIES\n'] + list(sorted_atomic_species_card_list))
+        sorted_atomic_species_card_list = ['ATOMIC_SPECIES\n'] + list(sorted_atomic_species_card_list)
         atomic_species_card = ''.join(sorted_atomic_species_card_list)
         # Free memory
         del sorted_atomic_species_card_list
         del atomic_species_card_list
 
         # ------------ ATOMIC_POSITIONS -----------
-        # Check on validity of FIXED_COORDS
-        fixed_coords_strings = []
-        fixed_coords = settings.pop('FIXED_COORDS', None)
-        if fixed_coords is None:
-            # No fixed_coords specified: I store a list of empty strings
-            fixed_coords_strings = [''] * len(structure.sites)
+        coordinates = [site.position for site in structure.sites]
+        if use_fractional:
+            atomic_positions_card_header = 'ATOMIC_POSITIONS crystal\n'
+            coordinates = numpy.dot(coordinates, numpy.linalg.inv(numpy.array(structure.cell))).tolist()
         else:
-            if len(fixed_coords) != len(structure.sites):
-                raise exceptions.InputValidationError(
-                    f'Input structure contains {len(structure.sites)} sites, but fixed_coords has length '
-                    f'{len(fixed_coords)}'
-                )
-
-            for i, this_atom_fix in enumerate(fixed_coords):
-                if len(this_atom_fix) != 3:
-                    raise exceptions.InputValidationError(f'fixed_coords({i + 1:d}) has not length three')
-                for fixed_c in this_atom_fix:
-                    if not isinstance(fixed_c, bool):
-                        raise exceptions.InputValidationError(f'fixed_coords({i + 1:d}) has non-boolean elements')
+            atomic_positions_card_header = 'ATOMIC_POSITIONS angstrom\n'
 
-                if_pos_values = [cls._if_pos(_) for _ in this_atom_fix]
-                fixed_coords_strings.append('  {:d} {:d} {:d}'.format(*if_pos_values))  # pylint: disable=consider-using-f-string
+        atomic_positions_card_list = [
+            '{0} {1:18.10f} {2:18.10f} {3:18.10f}'.format(site.kind_name.ljust(6), *site_coords)  # pylint: disable=consider-using-f-string
+            for site, site_coords in zip(structure.sites, coordinates)
+        ]
 
-        abs_pos = [_.position for _ in structure.sites]
-        if use_fractional:
-            import numpy as np
-            atomic_positions_card_list = ['ATOMIC_POSITIONS crystal\n']
-            coordinates = np.dot(np.array(abs_pos), np.linalg.inv(np.array(structure.cell)))
-        else:
-            atomic_positions_card_list = ['ATOMIC_POSITIONS angstrom\n']
-            coordinates = abs_pos
+        fixed_coords = settings.pop('FIXED_COORDS', None)
 
-        for site, site_coords, fixed_coords_string in zip(structure.sites, coordinates, fixed_coords_strings):
-            atomic_positions_card_list.append(
-                '{0} {1:18.10f} {2:18.10f} {3:18.10f} {4}\n'.format(  # pylint: disable=consider-using-f-string
-                    site.kind_name.ljust(6), site_coords[0], site_coords[1], site_coords[2], fixed_coords_string
+        if fixed_coords is not None:
+            # Note that this check is also in the validation of the top-level namespace, but this is only checked in
+            # in case the structure is provided
+            if len(fixed_coords) != len(structure.sites):
+                raise exceptions.InputValidationError(
+                    f'Input structure has {len(structure.sites)} sites, but fixed_coords has length {len(fixed_coords)}'
                 )
-            )
+            fixed_coords_strings = [
+                ' {:d} {:d} {:d}'.format(*row) for row in numpy.int32(numpy.invert(fixed_coords)).tolist()  # pylint: disable=consider-using-f-string
+            ]
+            atomic_positions_card_list = [
+                atomic_pos_str + fixed_coords_str
+                for atomic_pos_str, fixed_coords_str in zip(atomic_positions_card_list, fixed_coords_strings)
+            ]
 
-        atomic_positions_card = ''.join(atomic_positions_card_list)
-        del atomic_positions_card_list
+        atomic_positions_card = atomic_positions_card_header + '\n'.join(atomic_positions_card_list) + '\n'
 
         # Optional ATOMIC_FORCES card
         atomic_forces = settings.pop('ATOMIC_FORCES', None)
         if atomic_forces is not None:
 
             # Checking that there are as many forces defined as there are sites in the structure
             if len(atomic_forces) != len(structure.sites):
@@ -605,14 +620,16 @@
             except ValueError as exc:
                 raise QEInputValidationError(f'Cannot get structure parameters from cell: {exc}') from exc
             input_params['SYSTEM'].update(structure_parameters)
         input_params['SYSTEM']['nat'] = len(structure.sites)
         input_params['SYSTEM']['ntyp'] = len(structure.kinds)
 
         # ============ I prepare the k-points =============
+        kpoints_card = ''
+
         if cls._use_kpoints:
             try:
                 mesh, offset = kpoints.get_kpoints_mesh()
                 has_mesh = True
                 force_kpoints_list = settings.pop('FORCE_KPOINTS_LIST', False)
                 if force_kpoints_list:
                     kpoints_list = kpoints.get_kpoints_mesh(print_list=True)
@@ -681,14 +698,18 @@
                     kpoints_card_list.append(
                         f'  {kpoint[0]:18.10f} {kpoint[1]:18.10f} {kpoint[2]:18.10f} {weight:18.10f}\n'
                     )
 
             kpoints_card = ''.join(kpoints_card_list)
             del kpoints_card_list
 
+        # HUBBARD CARD
+        hubbard_card = HubbardUtils(structure).get_hubbard_card() if isinstance(structure, HubbardStructureData) \
+            else None
+
         # =================== NAMELISTS AND CARDS ========================
         try:
             namelists_toprint = settings.pop('NAMELISTS')
             if not isinstance(namelists_toprint, list):
                 raise exceptions.InputValidationError(
                     "The 'NAMELISTS' value, if specified in the settings input "
                     'node, must be a list of strings'
@@ -721,42 +742,32 @@
             for key, value in sorted(namelist.items()):
                 inputfile += convert_input_to_namelist_entry(key, value, mapping=mapping_species)
             inputfile += '/\n'
 
         # Write cards now
         inputfile += atomic_species_card
         inputfile += atomic_positions_card
-        if cls._use_kpoints:
-            inputfile += kpoints_card
+        inputfile += kpoints_card
         inputfile += cell_parameters_card
+        if hubbard_card is not None:
+            inputfile += hubbard_card
 
         # Generate additional cards bases on input parameters and settings that are subclass specific
         tail = cls._generate_PWCP_input_tail(input_params=input_params, settings=settings)
         if tail:
             inputfile += f'\n{tail}'
 
         if input_params:
             raise exceptions.InputValidationError(
                 'The following namelists are specified in input_params, but are not valid namelists for the current '
                 f'type of calculation: {",".join(list(input_params.keys()))}'
             )
 
         return inputfile, local_copy_list_to_append
 
-    @staticmethod
-    def _if_pos(fixed):
-        """Return 0 if fixed is True, 1 otherwise.
-
-        Useful to convert from the boolean value of fixed_coords to the value required by Quantum Espresso as if_pos.
-        """
-        if fixed:
-            return 0
-
-        return 1
-
 
 def _lowercase_dict(dictionary, dict_name):
     return _case_transform_dict(dictionary, dict_name, '_lowercase_dict', str.lower)
 
 
 def _uppercase_dict(dictionary, dict_name):
     return _case_transform_dict(dictionary, dict_name, '_uppercase_dict', str.upper)
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/base.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/base.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/cp.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/cp.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/dos.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/dos.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/epw.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/epw.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,34 +53,35 @@
         spec.input('parameters', valid_type=orm.Dict, help='')
         spec.input('settings', valid_type=orm.Dict, required=False, help='')
         spec.input('parent_folder_nscf', valid_type=orm.RemoteData,
                  help='the folder of a completed nscf `PwCalculation`')
         spec.input('parent_folder_ph', valid_type=orm.RemoteData, help='the folder of a completed `PhCalculation`')
         # yapf: enable
 
-    def prepare_for_submission(self, folder):  # pylint: disable=too-many-statements,too-many-branches
+    def prepare_for_submission(self, folder):
         """Prepare the calculation job for submission by transforming input nodes into input files.
 
         In addition to the input files being written to the sandbox folder, a `CalcInfo` instance will be returned that
         contains lists of files that need to be copied to the remote machine before job submission, as well as file
         lists that are to be retrieved after job completion.
 
         :param folder: a sandbox folder to temporarily write files on disk.
         :return: :class:`~aiida.common.datastructures.CalcInfo` instance.
         """
 
+        # pylint: disable=too-many-statements,too-many-branches
+
         def test_offset(offset):
             """Check if the grid has an offset."""
             if any(i != 0. for i in offset):
                 raise NotImplementedError(
                     'Computation of electron-phonon on a mesh with non zero offset is not implemented, '
                     'at the level of epw.x'
                 )
 
-        # pylint: disable=too-many-statements,too-many-branches
         local_copy_list = []
         remote_copy_list = []
         remote_symlink_list = []
 
         if 'settings' in self.inputs:
             settings = _uppercase_dict(self.inputs.settings.get_dict(), dict_name='settings')
         else:
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/functions/create_kpoints_from_distance.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/create_kpoints_from_distance.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/functions/seekpath_structure_analysis.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/seekpath_structure_analysis.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/functions/xspectra/get_powder_spectrum.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/xspectra/get_powder_spectrum.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/functions/xspectra/merge_spectra.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/functions/xspectra/merge_spectra.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.1.xml` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.1.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.2.xml` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.2.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.3.xml` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.3.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.xml` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.0.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.1.xml` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.1.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.2.xml` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.2.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.xml` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.1.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.2.0.xml` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.2.0.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.2.1.xml` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.2.1.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.3.0.xml` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.3.0.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.4.0.xml` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-5.4.0.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.0.xml` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.0.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.1.xml` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.1.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.2.xml` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.2.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.3.xml` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.3.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.4.xml` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/INPUT_PW-6.4.xml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/helpers/__init__.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/matdyn.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/matdyn.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
             parameters = value['parameters'].get_dict()
         else:
             parameters = {}
 
         if parameters.get('INPUT', {}).get('flfrc', None) is not None:
             return '`INPUT.flfrc` is set automatically from the `force_constants` input.'
 
-    def generate_input_file(self, parameters):
+    def generate_input_file(self, parameters):  # pylint: disable=arguments-differ
         """Generate namelist input_file content given a dict of parameters.
 
         :param parameters: 'dict' containing the fortran namelists and parameters to be used.
           e.g.: {'CONTROL':{'calculation':'scf'}, 'SYSTEM':{'ecutwfc':30}}
         :return: 'str' containing the input_file content a plain text.
         """
         kpoints = self.inputs.kpoints
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/namelists.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/namelists.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/neb.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/neb.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/ph.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/ph.py`

 * *Files 0% similar despite different names*

```diff
@@ -112,16 +112,16 @@
 
         parent_calc = parent_calcs[0].node
 
         # If the parent calculation is a `PhCalculation` we are restarting
         restart_flag = parent_calc.process_type == 'aiida.calculations:quantumespresso.ph'
 
         # Also, the parent calculation must be on the same computer
-        if not self.node.computer.uuid == parent_calc.computer.uuid:
-            computer_label = parent_calc.computer.get_name()
+        if self.node.computer.uuid != parent_calc.computer.uuid:
+            computer_label = parent_calc.computer.label
             raise exceptions.InputValidationError(
                 f'Calculation has to be launched on the same computer as that of the parent: {computer_label}'
             )
 
         # put by default, default_parent_output_folder = ./out
         try:
             default_parent_output_folder = parent_calc.process_class._OUTPUT_SUBFOLDER  # pylint: disable=protected-access
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/pp.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/pp.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/projwfc.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/projwfc.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/pw.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/pw.py`

 * *Files 7% similar despite different names*

```diff
@@ -57,14 +57,15 @@
             filepaths.append(filepath)
 
         return filepaths
 
     @classmethod
     def define(cls, spec):
         """Define the process specification."""
+        # pylint: disable=too-many-statements
         # yapf: disable
         super().define(spec)
         spec.input('metadata.options.parser_name', valid_type=str, default='quantumespresso.pw')
         spec.input('metadata.options.without_xml', valid_type=bool, required=False, help='If set to `True` the parser '
             'will not fail if the XML file is missing in the retrieved folder.')
         spec.input('kpoints', valid_type=orm.KpointsData,
             help='kpoint mesh or kpoint path')
@@ -107,37 +108,52 @@
         spec.exit_code(322, 'ERROR_OUTPUT_XML_FORMAT',
             message='The XML output file has an unsupported format.')
         spec.exit_code(340, 'ERROR_OUT_OF_WALLTIME_INTERRUPTED',
             message='The calculation stopped prematurely because it ran out of walltime but the job was killed by the '
                     'scheduler before the files were safely written to disk for a potential restart.')
         spec.exit_code(350, 'ERROR_UNEXPECTED_PARSER_EXCEPTION',
             message='The parser raised an unexpected exception: {exception}')
+        spec.exit_code(360, 'ERROR_G_PAR',
+            message='The code failed in finding a valid reciprocal lattice vector.')
 
         # Significant errors but calculation can be used to restart
         spec.exit_code(400, 'ERROR_OUT_OF_WALLTIME',
             message='The calculation stopped prematurely because it ran out of walltime.')
         spec.exit_code(410, 'ERROR_ELECTRONIC_CONVERGENCE_NOT_REACHED',
             message='The electronic minimization cycle did not reach self-consistency.')
 
         spec.exit_code(461, 'ERROR_DEXX_IS_NEGATIVE',
             message='The code failed with negative dexx in the exchange calculation.')
         spec.exit_code(462, 'ERROR_COMPUTING_CHOLESKY',
             message='The code failed during the cholesky factorization.')
         spec.exit_code(463, 'ERROR_DIAGONALIZATION_TOO_MANY_BANDS_NOT_CONVERGED',
             message='Too many bands failed to converge during the diagonalization.')
+        spec.exit_code(464, 'ERROR_S_MATRIX_NOT_POSITIVE_DEFINITE',
+            message='The S matrix was found to be not positive definite.')
+        spec.exit_code(465, 'ERROR_ZHEGVD_FAILED',
+            message='The `zhegvd` failed in the PPCG diagonalization.')
+        spec.exit_code(466, 'ERROR_QR_FAILED',
+            message='The `[Q, R] = qr(X, 0)` failed in the PPCG diagonalization.')
+        spec.exit_code(467, 'ERROR_EIGENVECTOR_CONVERGENCE',
+            message='The eigenvector failed to converge.')
+        spec.exit_code(468, 'ERROR_BROYDEN_FACTORIZATION',
+            message='The factorization in the Broyden routine failed.')
 
         spec.exit_code(481, 'ERROR_NPOOLS_TOO_HIGH',
             message='The k-point parallelization "npools" is too high, some nodes have no k-points.')
 
         spec.exit_code(500, 'ERROR_IONIC_CONVERGENCE_NOT_REACHED',
             message='The ionic minimization cycle did not converge for the given thresholds.')
         spec.exit_code(501, 'ERROR_IONIC_CONVERGENCE_REACHED_EXCEPT_IN_FINAL_SCF',
             message='Then ionic minimization cycle converged but the thresholds are exceeded in the final SCF.')
         spec.exit_code(502, 'ERROR_IONIC_CYCLE_EXCEEDED_NSTEP',
             message='The ionic minimization cycle did not converge after the maximum number of steps.')
+        spec.exit_code(503, 'ERROR_IONIC_INTERRUPTED_PARTIAL_TRAJECTORY',
+            message='The ionic minimization cycle did not finish because the calculation was interrupted but a partial '
+                    'trajectory and output structure was successfully parsed which can be used for a restart.')
         spec.exit_code(510, 'ERROR_IONIC_CYCLE_ELECTRONIC_CONVERGENCE_NOT_REACHED',
             message='The electronic minimization cycle failed during an ionic minimization cycle.')
         spec.exit_code(511, 'ERROR_IONIC_CONVERGENCE_REACHED_FINAL_SCF_FAILED',
             message='The ionic minimization cycle converged, but electronic convergence was not reached in the '
                     'final SCF.')
         spec.exit_code(520, 'ERROR_IONIC_CYCLE_BFGS_HISTORY_FAILURE',
             message='The ionic minimization cycle terminated prematurely because of two consecutive failures in the '
@@ -146,52 +162,53 @@
             message='The ionic minimization cycle terminated prematurely because of two consecutive failures in the '
                     'BFGS algorithm and electronic convergence failed in the final SCF.')
 
         spec.exit_code(531, 'ERROR_CHARGE_IS_WRONG',
             message='The electronic minimization cycle did not reach self-consistency.')
         spec.exit_code(541, 'ERROR_SYMMETRY_NON_ORTHOGONAL_OPERATION',
             message='The variable cell optimization broke the symmetry of the k-points.')
+        spec.exit_code(542, 'ERROR_RADIAL_FFT_SIGNIFICANT_VOLUME_CONTRACTION',
+            message=('The cell relaxation caused a significant volume contraction '
+                     'and there is not enough space allocated for radial FFT.'))
 
         # Strong warnings about calculation results, but something tells us that you're ok with that
         spec.exit_code(710, 'WARNING_ELECTRONIC_CONVERGENCE_NOT_REACHED',
             message='The electronic minimization cycle did not reach self-consistency, but `scf_must_converge` '
                     'is `False` and/or `electron_maxstep` is 0.')
         # yapf: enable
 
     @staticmethod
     def validate_inputs_base(value, _):
         """Validate the top level namespace."""
         parameters = value['parameters'].get_dict()
         calculation_type = parameters.get('CONTROL', {}).get('calculation', 'scf')
 
-        # Check that the restart input parameters are set correctly
-        if calculation_type in ('nscf', 'bands'):
-            if parameters.get('ELECTRONS', {}).get('startingpot', 'file') != 'file':
-                return f'`startingpot` should be set to `file` for a `{calculation_type}` calculation.'
-            if parameters.get('CONTROL', {}).get('restart_mode', 'from_scratch') != 'from_scratch':
-                warnings.warn(f'`restart_mode` should be set to `from_scratch` for a `{calculation_type}` calculation.')
-        elif 'parent_folder' in value:
+        # If a `parent_folder` input is provided, make sure the inputs are set to restart
+        if 'parent_folder' in value and calculation_type not in ('nscf', 'bands'):
             if not any([
                 parameters.get('CONTROL', {}).get('restart_mode', None) == 'restart',
                 parameters.get('ELECTRONS', {}).get('startingpot', None) == 'file',
                 parameters.get('ELECTRONS', {}).get('startingwfc', None) == 'file'
             ]):
                 warnings.warn(
-                    '`parent_folder` input was provided for the `PwCalculation`, but no '
-                    'input parameters are set to restart from these files.'
+                    f'`parent_folder` input was provided for the `{calculation_type}` `PwCalculation`, but no input'
+                    'parameters were provided to restart from this folder.\n\n'
+                    'Please set one of the following in the input parameters:\n'
+                    "    parameters['CONTROL']['restart_mode'] = 'restart'\n"
+                    "    parameters['ELECTRONS']['startingpot'] = 'file'\n"
+                    "    parameters['ELECTRONS']['startingwfc'] = 'file'\n"
                 )
 
     @classmethod
     def validate_inputs(cls, value, port_namespace):
         """Validate the top level namespace.
 
         Check that the restart input parameters are set correctly. In case of 'nscf' and 'bands' calculations, this
-        means ``parent_folder`` is provided, ``startingpot`` is set to 'file' and ``restart_mode`` is 'from_scratch'.
-        For other calculations, if the ``parent_folder`` is provided, the restart settings must be set to use some of
-        the outputs.
+        means ``parent_folder`` is provided. For other calculations, if the ``parent_folder`` is provided, the restart
+        settings must be set to use some of the outputs.
 
         Note that the validator is split in two methods: ``validate_inputs`` and ``validate_inputs_base``. This is to
         facilitate work chains that wrap this calculation that will provide the ``parent_folder`` themselves and so do
         not require the user to provide it at launch of the work chain. This will fail because of the validation in this
         validator, however, which is why the rest of the logic is moved to ``validate_inputs_base``. The wrapping work
         chain can change the ``validate_input`` validator for ``validate_inputs_base`` thereby allowing the parent
         folder to be defined during the work chains runtime, while still keep the rest of the namespace validation.
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/pw2gw.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/pw2gw.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/pw2wannier90.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/pw2wannier90.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/pwimmigrant.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/pwimmigrant.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/q2r.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/q2r.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 # -*- coding: utf-8 -*-
 """`CalcJob` implementation for the q2r.x code of Quantum ESPRESSO."""
-import os
 
 from aiida import orm
 
 from aiida_quantumespresso.calculations.namelists import NamelistsCalculation
 from aiida_quantumespresso.calculations.ph import PhCalculation
 from aiida_quantumespresso.data.force_constants import ForceConstantsData
 
 
 class Q2rCalculation(NamelistsCalculation):
     """`CalcJob` implementation for the q2r.x code of Quantum ESPRESSO."""
 
     _FORCE_CONSTANTS_NAME = 'real_space_force_constants.dat'
     _OUTPUT_SUBFOLDER = PhCalculation._FOLDER_DYNAMICAL_MATRIX  # pylint: disable=protected-access
-    _INPUT_SUBFOLDER = os.path.join('.', PhCalculation._FOLDER_DYNAMICAL_MATRIX)  # pylint: disable=protected-access
+    _INPUT_SUBFOLDER = PhCalculation._FOLDER_DYNAMICAL_MATRIX  # pylint: disable=protected-access
     _default_parent_output_folder = PhCalculation._FOLDER_DYNAMICAL_MATRIX  # pylint: disable=protected-access
 
     _default_namelists = ['INPUT']
     _blocked_keywords = [
         ('INPUT', 'fildyn', PhCalculation._OUTPUT_DYNAMICAL_MATRIX_PREFIX),  # pylint: disable=protected-access
         ('INPUT', 'flfrc', _FORCE_CONSTANTS_NAME),  # Real space force constants
     ]
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/calculations/xspectra.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/calculations/xspectra.py`

 * *Files 0% similar despite different names*

```diff
@@ -91,15 +91,15 @@
         )
         spec.exit_code(
             331,
             'ERROR_READING_SPECTRUM_FILE_DATA',
             message='The spectrum data file could not be read using NumPy genfromtxt'
         )
 
-    def generate_input_file(self, parameters):
+    def generate_input_file(self, parameters):  # pylint: disable=arguments-differ
         """Add kpoint handling to the inherited method.
 
         This checks that the offset for the mesh is in a valid format, converts the offset
         from AiiDA format to QE format, and adds the kpoint mesh input to the end of the file.
 
         Essentially this copies the method used in prepare_for_submission from the
         BasePwCpInputGenerator class.
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/__init__.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/calculations/__init__.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/calculations/cp.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/cp.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/calculations/dos.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/dos.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/calculations/epw.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/epw.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/calculations/matdyn.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/matdyn.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/calculations/neb.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/neb.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/calculations/ph.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/ph.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/calculations/pp.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/pp.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/calculations/projwfc.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/projwfc.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/calculations/pw.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/pw.py`

 * *Files 5% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     '--unfolded-kpoints',
     'unfolded_kpoints',
     is_flag=True,
     help='Unfold the k-points grid to the whole grid without reducing it by symmetry (useful mainly for NSCF).'
 )
 @decorators.with_dbenv()
 def launch_calculation(
-    code, structure, pseudo_family, kpoints_mesh, ecutwfc, ecutrho, hubbard_u, hubbard_v, hubbard_file_pk,
+    code, structure, pseudo_family, kpoints_mesh, ecutwfc, ecutrho, hubbard_u, hubbard_v, hubbard_file,
     starting_magnetization, smearing, max_num_machines, max_wallclock_seconds, with_mpi, daemon, parent_folder, dry_run,
     mode, unfolded_kpoints
 ):
     """Run a PwCalculation."""
     from aiida.orm import Dict, KpointsData
     from aiida.plugins import CalculationFactory
 
@@ -69,17 +69,15 @@
         }
     }
 
     if mode in CALCS_REQUIRING_PARENT and not parent_folder:
         raise click.BadParameter(f"calculation '{mode}' requires a parent folder", param_hint='--parent-folder')
 
     try:
-        hubbard_file = validate.validate_hubbard_parameters(
-            structure, parameters, hubbard_u, hubbard_v, hubbard_file_pk
-        )
+        validate.validate_hubbard_parameters(structure, parameters, hubbard_u, hubbard_v, hubbard_file)
     except ValueError as exception:
         raise click.BadParameter(str(exception))
 
     try:
         validate.validate_starting_magnetization(structure, parameters, starting_magnetization)
     except ValueError as exception:
         raise click.BadParameter(str(exception))
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/calculations/pw2wannier90.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/pw2wannier90.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/calculations/q2r.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/calculations/q2r.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/data/structure.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/data/structure.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/utils/defaults.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/utils/defaults.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/utils/display.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/utils/display.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/utils/launch.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/utils/launch.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/utils/options.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/utils/options.py`

 * *Files 1% similar despite different names*

```diff
@@ -205,15 +205,15 @@
     help='Add a Hubbard V interaction between two sites.',
     metavar='<SITE SITE TYPE MAGNITUDE>...'
 )
 
 HUBBARD_FILE = OverridableOption(
     '-H',
     '--hubbard-file',
-    'hubbard_file_pk',
+    'hubbard_file',
     type=types.DataParamType(sub_classes=('aiida.data:core.singlefile',)),
     help='SinglefileData containing Hubbard parameters from a HpCalculation to use as input for Hubbard V.'
 )
 
 STARTING_MAGNETIZATION = OverridableOption(
     '--starting-magnetization',
     nargs=2,
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/utils/validate.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/utils/validate.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,10 @@
 # -*- coding: utf-8 -*-
 """Utility functions for validation of command line interface parameter inputs."""
 from aiida.cmdline.utils import decorators
-from aiida.common import exceptions
 import click
 
 
 @decorators.with_dbenv()
 def validate_kpoints_mesh(ctx, param, value):
     """Command line option validator for a kpoints mesh tuple.
 
@@ -32,43 +31,28 @@
     except ValueError as exception:
         raise click.BadParameter(f'failed to create a KpointsData mesh out of {value}\n{exception}')
 
     return kpoints
 
 
 @decorators.with_dbenv()
-def validate_hubbard_parameters(structure, parameters, hubbard_u=None, hubbard_v=None, hubbard_file_pk=None):
+def validate_hubbard_parameters(structure, parameters, hubbard_u=None, hubbard_v=None, hubbard_file=None):
     """Validate Hubbard input parameters and update the parameters input node accordingly.
 
-    If a valid hubbard_file_pk is provided, the node will be loaded and returned.
-
     :param structure: the StructureData node that will be used in the inputs
     :param parameters: the Dict node that will be used in the inputs
     :param hubbard_u: the Hubbard U inputs values from the cli
     :param hubbard_v: the Hubbard V inputs values from the cli
-    :param hubbard_file_pk: a pk referencing a SinglefileData with Hubbard parameters
-    :returns: the loaded SinglefileData node with Hubbard parameters if valid pk was defined, None otherwise
+    :param hubbard_file: a SinglefileData with Hubbard parameters
     :raises ValueError: if the input is invalid
     """
-    from aiida.orm import SinglefileData, load_node
-
-    if len([value for value in [hubbard_u, hubbard_v, hubbard_file_pk] if value]) > 1:
-        raise ValueError('the hubbard_u, hubbard_v and hubbard_file_pk options are mutually exclusive')
-
-    hubbard_file = None
+    if len([value for value in [hubbard_u, hubbard_v, hubbard_file] if value]) > 1:
+        raise ValueError('the hubbard_u, hubbard_v and hubbard_file options are mutually exclusive')
 
-    if hubbard_file_pk:
-
-        try:
-            hubbard_file = load_node(pk=hubbard_file_pk)
-        except exceptions.NotExistent:
-            ValueError(f'{hubbard_file_pk} is not a valid pk')
-        else:
-            if not isinstance(hubbard_file, SinglefileData):
-                ValueError(f'Node<{hubbard_file_pk}> is not a SinglefileData but {type(hubbard_file)}')
+    if hubbard_file:
 
         parameters['SYSTEM']['lda_plus_u'] = True
         parameters['SYSTEM']['lda_plus_u_kind'] = 2
         parameters['SYSTEM']['hubbard_parameters'] = 'file'
 
     elif hubbard_v:
 
@@ -91,16 +75,14 @@
         parameters['SYSTEM']['lda_plus_u'] = True
         parameters['SYSTEM']['lda_plus_u_kind'] = 0
         parameters['SYSTEM']['hubbard_u'] = {}
 
         for kind, value in hubbard_u:
             parameters['SYSTEM']['hubbard_u'][kind] = value
 
-    return hubbard_file
-
 
 def validate_starting_magnetization(structure, parameters, starting_magnetization=None):
     """Validate starting magnetization parameters and update the parameters input node accordingly.
 
     :param structure: the StructureData node that will be used in the inputs
     :param parameters: the Dict node that will be used in the inputs
     :param starting_magnetization: the starting magnetization inputs values from the cli
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/workflows/__init__.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/workflows/matdyn/base.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/matdyn/base.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/workflows/ph/base.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/ph/base.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/workflows/pw/bands.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/pw/bands.py`

 * *Files 9% similar despite different names*

```diff
@@ -17,32 +17,30 @@
 @options.ECUTWFC()
 @options.ECUTRHO()
 @options.HUBBARD_U()
 @options.HUBBARD_V()
 @options.HUBBARD_FILE()
 @options.STARTING_MAGNETIZATION()
 @options.SMEARING()
-@options.AUTOMATIC_PARALLELIZATION()
 @options.CLEAN_WORKDIR()
 @options.MAX_NUM_MACHINES()
 @options.MAX_WALLCLOCK_SECONDS()
 @options.WITH_MPI()
 @options.DAEMON()
 @decorators.with_dbenv()
 def launch_workflow(
-    code, structure, pseudo_family, kpoints_distance, ecutwfc, ecutrho, hubbard_u, hubbard_v, hubbard_file_pk,
-    starting_magnetization, smearing, automatic_parallelization, clean_workdir, max_num_machines, max_wallclock_seconds,
-    with_mpi, daemon
+    code, structure, pseudo_family, kpoints_distance, ecutwfc, ecutrho, hubbard_u, hubbard_v, hubbard_file,
+    starting_magnetization, smearing, clean_workdir, max_num_machines, max_wallclock_seconds, with_mpi, daemon
 ):
     """Run a `PwBandsWorkChain`."""
     # pylint: disable=too-many-statements
     from aiida.orm import Bool, Dict, Float
     from aiida.plugins import WorkflowFactory
 
-    from aiida_quantumespresso.utils.resources import get_automatic_parallelization_options, get_default_options
+    from aiida_quantumespresso.utils.resources import get_default_options
 
     builder = WorkflowFactory('quantumespresso.pw.bands').get_builder()
 
     cutoff_wfc, cutoff_rho = pseudo_family.get_recommended_cutoffs(structure=structure, unit='Ry')
 
     parameters = {
         'CONTROL': {
@@ -51,17 +49,15 @@
         'SYSTEM': {
             'ecutwfc': ecutwfc or cutoff_wfc,
             'ecutrho': ecutrho or cutoff_rho,
         },
     }
 
     try:
-        hubbard_file = validate.validate_hubbard_parameters(
-            structure, parameters, hubbard_u, hubbard_v, hubbard_file_pk
-        )
+        validate.validate_hubbard_parameters(structure, parameters, hubbard_u, hubbard_v, hubbard_file)
     except ValueError as exception:
         raise click.BadParameter(str(exception))
 
     try:
         validate.validate_starting_magnetization(structure, parameters, starting_magnetization)
     except ValueError as exception:
         raise click.BadParameter(str(exception))
@@ -89,22 +85,16 @@
     builder.bands.pw.pseudos = pseudos
 
     if hubbard_file:
         builder.relax.base.pw.hubbard_file = hubbard_file
         builder.scf.base.pw.hubbard_file = hubbard_file
         builder.bands.base.pw.hubbard_file = hubbard_file
 
-    if automatic_parallelization:
-        auto_para = Dict(get_automatic_parallelization_options(max_num_machines, max_wallclock_seconds))
-        builder.relax.base.automatic_parallelization = auto_para
-        builder.scf.automatic_parallelization = auto_para
-        builder.bands.automatic_parallelization = auto_para
-    else:
-        metadata_options = get_default_options(max_num_machines, max_wallclock_seconds, with_mpi)
-        builder.relax.base.pw.metadata.options = metadata_options
-        builder.scf.pw.metadata.options = metadata_options
-        builder.bands.pw.metadata.options = metadata_options
+    metadata_options = get_default_options(max_num_machines, max_wallclock_seconds, with_mpi)
+    builder.relax.base.pw.metadata.options = metadata_options
+    builder.scf.pw.metadata.options = metadata_options
+    builder.bands.pw.metadata.options = metadata_options
 
     if clean_workdir:
         builder.clean_workdir = Bool(True)
 
     launch.launch_process(builder, daemon)
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/workflows/pw/base.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/pw/relax.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,88 +1,101 @@
 # -*- coding: utf-8 -*-
-"""Command line scripts to launch a `PwBaseWorkChain` for testing and demonstration purposes."""
+"""Command line scripts to launch a `PwRelaxWorkChain` for testing and demonstration purposes."""
 from aiida.cmdline.params import options as options_core
 from aiida.cmdline.params import types
 from aiida.cmdline.utils import decorators
 import click
 
 from .. import cmd_launch
-from ...utils import defaults, launch, options, validate
+from ...utils import launch, options, validate
 
 
-@cmd_launch.command('pw-base')
+@cmd_launch.command('pw-relax')
 @options_core.CODE(required=True, type=types.CodeParamType(entry_point='quantumespresso.pw'))
-@options.STRUCTURE(default=defaults.get_structure)
+@options.STRUCTURE(required=True)
 @options.PSEUDO_FAMILY()
 @options.KPOINTS_DISTANCE()
 @options.ECUTWFC()
 @options.ECUTRHO()
 @options.HUBBARD_U()
 @options.HUBBARD_V()
 @options.HUBBARD_FILE()
 @options.STARTING_MAGNETIZATION()
 @options.SMEARING()
-@options.AUTOMATIC_PARALLELIZATION()
 @options.CLEAN_WORKDIR()
 @options.MAX_NUM_MACHINES()
 @options.MAX_WALLCLOCK_SECONDS()
 @options.WITH_MPI()
 @options.DAEMON()
+@click.option(
+    '-f',
+    '--final-scf',
+    is_flag=True,
+    default=False,
+    show_default=True,
+    help='Run a final scf calculation for the final relaxed structure.'
+)
 @decorators.with_dbenv()
 def launch_workflow(
-    code, structure, pseudo_family, kpoints_distance, ecutwfc, ecutrho, hubbard_u, hubbard_v, hubbard_file_pk,
-    starting_magnetization, smearing, automatic_parallelization, clean_workdir, max_num_machines, max_wallclock_seconds,
-    with_mpi, daemon
+    code, structure, pseudo_family, kpoints_distance, ecutwfc, ecutrho, hubbard_u, hubbard_v, hubbard_file,
+    starting_magnetization, smearing, clean_workdir, max_num_machines, max_wallclock_seconds, with_mpi, daemon,
+    final_scf
 ):
-    """Run a `PwBaseWorkChain`."""
-    from aiida.orm import Bool, Dict, Float
+    """Run a `PwRelaxWorkChain`."""
+    from aiida.orm import Bool, Dict, Float, Str
     from aiida.plugins import WorkflowFactory
 
-    from aiida_quantumespresso.utils.resources import get_automatic_parallelization_options, get_default_options
+    from aiida_quantumespresso.utils.resources import get_default_options
 
-    builder = WorkflowFactory('quantumespresso.pw.base').get_builder()
+    builder = WorkflowFactory('quantumespresso.pw.relax').get_builder()
 
     cutoff_wfc, cutoff_rho = pseudo_family.get_recommended_cutoffs(structure=structure, unit='Ry')
 
     parameters = {
+        'CONTROL': {
+            'calculation': 'relax',
+        },
         'SYSTEM': {
             'ecutwfc': ecutwfc or cutoff_wfc,
             'ecutrho': ecutrho or cutoff_rho,
         },
     }
 
     try:
-        hubbard_file = validate.validate_hubbard_parameters(
-            structure, parameters, hubbard_u, hubbard_v, hubbard_file_pk
-        )
+        validate.validate_hubbard_parameters(structure, parameters, hubbard_u, hubbard_v, hubbard_file)
     except ValueError as exception:
         raise click.BadParameter(str(exception))
 
     try:
         validate.validate_starting_magnetization(structure, parameters, starting_magnetization)
     except ValueError as exception:
         raise click.BadParameter(str(exception))
 
     try:
         validate.validate_smearing(parameters, smearing)
     except ValueError as exception:
         raise click.BadParameter(str(exception))
 
-    builder.pw.code = code
-    builder.pw.structure = structure
-    builder.pw.parameters = Dict(parameters)
-    builder.pw.pseudos = pseudo_family.get_pseudos(structure=structure)
-    builder.kpoints_distance = Float(kpoints_distance)
+    builder.structure = structure
+    builder.base.kpoints_distance = Float(kpoints_distance)
+    builder.base.pw.code = code
+    builder.base.pw.pseudos = pseudo_family.get_pseudos(structure=structure)
+    builder.base.pw.parameters = Dict(parameters)
 
     if hubbard_file:
-        builder.hubbard_file = hubbard_file
+        builder.base.pw.hubbard_file = hubbard_file
 
-    if automatic_parallelization:
-        automatic_parallelization = get_automatic_parallelization_options(max_num_machines, max_wallclock_seconds)
-        builder.automatic_parallelization = Dict(automatic_parallelization)
-    else:
-        builder.pw.metadata.options = get_default_options(max_num_machines, max_wallclock_seconds, with_mpi)
+    builder.base.pw.metadata.options = get_default_options(max_num_machines, max_wallclock_seconds, with_mpi)
 
     if clean_workdir:
         builder.clean_workdir = Bool(True)
 
+    if final_scf:
+        builder.base_final_scf.pseudo_family = Str(pseudo_family)
+        builder.base_final_scf.kpoints_distance = Float(kpoints_distance)
+        builder.base_final_scf.pw.code = code
+        builder.base_final_scf.pw.parameters = Dict(parameters)
+        builder.base_final_scf.pw.metadata.options = get_default_options(
+            max_num_machines, max_wallclock_seconds, with_mpi
+        )
+
     launch.launch_process(builder, daemon)
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/cli/workflows/q2r/base.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/cli/workflows/q2r/base.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/common/types.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/common/types.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/data/force_constants.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/data/force_constants.py`

 * *Files 0% similar despite different names*

```diff
@@ -174,15 +174,15 @@
                 line[2:] = [pos * celldm[0] * CONSTANTS.bohr_to_ang for pos in line[2:]]
             atom_list.append(tuple(line))
             current_line += 1
 
         parsed_data['atom_list'] = atom_list
 
         # read lrigid (flag for dielectric constant and effective charges
-        has_done_electric_field = (lines[current_line].split()[0] == 'T')
+        has_done_electric_field = lines[current_line].split()[0] == 'T'
         parsed_data['has_done_electric_field'] = has_done_electric_field
         current_line += 1
 
         if has_done_electric_field:
             # read dielectric tensor
             dielectric_tensor = tuple(tuple(float(c) for c in l.split()) for l in lines[current_line:current_line + 3])
             current_line += 3
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/base.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/base.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/cp.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/cp.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/dos.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/dos.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/matdyn.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/matdyn.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/neb.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/neb.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_raw/base.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_raw/base.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_raw/cp.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_raw/cp.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_raw/neb.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_raw/neb.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_raw/ph.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_raw/ph.py`

 * *Files 20% similar despite different names*

```diff
@@ -71,17 +71,25 @@
     # join dictionaries, there should not be any twice repeated key
     for key in out_data.keys():
         if key in list(tensor_data.keys()):
             raise AssertionError(f'{key} found in two dictionaries')
         if key in list(dynmat_data.keys()):
             raise AssertionError(f'{key} found in two dictionaries')
 
-    # I don't check the dynmat_data and parser_info keys
+    symmetry_labels = out_data.pop('symmetry_labels', {})
+
+    if len(dynmat_data) == 1 and 'dynamical_matrix_0' in dynmat_data:
+        dynmat_data['dynamical_matrix_1'] = dynmat_data.pop('dynamical_matrix_0')
+
     parsed_data = dict(list(dynmat_data.items()) + list(out_data.items()) + list(tensor_data.items()))
 
+    for q_index, q_symlabels in symmetry_labels.items():
+        if f'dynamical_matrix_{q_index}' in parsed_data:
+            parsed_data[f'dynamical_matrix_{q_index}'].update(q_symlabels)
+
     return parsed_data, logs
 
 
 def parse_ph_tensor(data):
     """Parse the xml tensor file of QE v5.0.3 data must be read from the file with the .read() function (avoid
     readlines)"""
     from xml.dom.minidom import parseString
@@ -168,61 +176,90 @@
 
         for marker, message in message_map['warning'].items():
             if marker in line:
                 if message is None:
                     message = line
                 logs.warning.append(message)
 
+    def parse_qpoints(lines):
+        """Parse the q-points from the corresponding lines in the stdout."""
+
+        return {int(line.split()[0]): [float(coord) for coord in line.split()[1:4]] for line in lines}
+
+    def parse_mode_symmetries(lines, num_atoms):
+        """Parse the mode symmetries from the block after diagonalization of the dynamical matrix."""
+
+        q_data = {}
+        symlabel_q_point = [float(i) for i in lines[2].split('q = (')[-1].split(')')[0].split()]
+
+        q_data['mode_symmetry'] = []
+
+        for line in lines:
+
+            if 'Mode symmetry' in line:
+                q_data['point_group'] = line.split('Mode symmetry,')[1].split('point group:')[0].strip()
+
+            if '-->' in line:
+                freq_start = int(line.split('(')[1].split(')')[0].split('-')[0])
+                freq_end = int(line.split('(')[1].split(')')[0].split('-')[1])
+
+                if line.split()[-1] == 'I':
+                    symm_label = line.split()[-2]
+                else:
+                    symm_label = line.split()[-1]
+
+                q_data['mode_symmetry'].extend([symm_label] * (freq_end - freq_start + 1))
+
+        # If the mode symmetries are not printed, set those for the non-symmetry case
+        if 'point_group' not in q_data:
+            q_data['point_group'] = 'C_1'
+            q_data['mode_symmetry'] = ['A'] * (3 * num_atoms)
+
+        return symlabel_q_point, q_data
+
     parsed_data = {}
 
     # Parse time, starting from the end because the time is written multiple times
     for line in reversed(lines):
         if 'PHONON' in line and 'WALL' in line:
             try:
-                time = line.split('CPU')[1].split('WALL')[0]
-                parsed_data['wall_time'] = time
-            except Exception:
-                logs.warning.append('Error while parsing wall time.')
-
-            try:
                 parsed_data['wall_time_seconds'] = \
-                    convert_qe_time_to_sec(parsed_data['wall_time'])
-            except ValueError:
-                raise QEOutputParsingError('Unable to convert wall_time in seconds.')
+                    convert_qe_time_to_sec(line.split('CPU')[1].split('WALL')[0])
+            except (ValueError, IndexError):
+                raise QEOutputParsingError('Error during parsing of walltime.')
             break
 
-    # Parse number of q-points and number of atoms
+    parsed_data['num_q_found'] = 0
+
     for count, line in enumerate(lines):
 
         detect_important_message(logs, line)
 
         if 'q-points for this run' in line:
             try:
-                num_qpoints = int(line.split('/')[1].split('q-points')[0])
-                if (
-                    'number_of_qpoints' in list(parsed_data.keys()) and num_qpoints != parsed_data['number_of_qpoints']
-                ):
-                    logs.warning.append('Number q-points found several times with different values')
-                else:
-                    parsed_data['number_of_qpoints'] = num_qpoints
-            except Exception:
-                logs.warning.append('Error while parsing number of q points.')
+                parsed_data['number_of_qpoints'] = int(line.split('/')[1].split('q-points')[0])
+                parsed_data['q_points'] = parse_qpoints(lines[count + 2:count + parsed_data['number_of_qpoints'] + 2])
+
+            except Exception as exc:
+                logs.warning.append(f'Error while parsing number of q points: {exc}')
 
         elif 'q-points)' in line:
             # case of a 'only_wfc' calculation
             try:
-                num_qpoints = int(line.split('q-points')[0].split('(')[1])
-                if (
-                    'number_of_qpoints' in list(parsed_data.keys()) and num_qpoints != parsed_data['number_of_qpoints']
-                ):
-                    logs.warning.append('Number q-points found several times with different values')
-                else:
-                    parsed_data['number_of_qpoints'] = num_qpoints
-            except Exception:
-                logs.warning.append('Error while parsing number of q points.')
+                parsed_data['number_of_qpoints'] = int(line.split('q-points')[0].split('(')[1])
+                parsed_data['q_points'] = parse_qpoints(lines[count + 2:count + parsed_data['number_of_qpoints'] + 2])
+
+            except Exception as exc:
+                logs.warning.append(f'Error while parsing number of q points: {exc}')
+
+        # In case a single q-point is provided at the end of the input file, there is no summary of the q-points at the
+        # start of the stdout. Then we have to parse the q-point further down the output file.
+        elif 'number_of_qpoints' not in parsed_data and 'Calculation of q =' in line:
+            parsed_data['number_of_qpoints'] = 1
+            parsed_data['q_points'] = {1: [float(coord) for coord in line.split('=')[-1].split()]}
 
         elif 'number of atoms/cell' in line:
             try:
                 num_atoms = int(line.split('=')[1])
                 parsed_data['number_of_atoms'] = num_atoms
             except Exception:
                 logs.warning.append('Error while parsing number of atoms.')
@@ -232,14 +269,40 @@
                 parsed_data['number_of_irr_representations_for_each_q'] = []
             try:
                 num_irr_repr = int(line.split('irreducible')[0].split('are')[1])
                 parsed_data['number_of_irr_representations_for_each_q'].append(num_irr_repr)
             except Exception:
                 pass
 
+        elif 'Diagonalizing the dynamical matrix' in line:
+
+            mode_count = count
+
+            while not 'Calculation' in lines[mode_count] and not 'CPU' in lines[mode_count]:
+                mode_count += 1
+
+            symlabel_q_point, q_data = parse_mode_symmetries(lines[count: mode_count], num_atoms)
+
+            for q_index, q_point in parsed_data['q_points'].items():
+                if numpy.isclose(
+                    numpy.array(q_point), numpy.array(symlabel_q_point), rtol=0, atol=1e-7
+                ).all():
+                    parsed_data.setdefault('symmetry_labels', {})
+                    parsed_data['symmetry_labels'][q_index] = q_data
+
+            parsed_data['num_q_found'] += 1
+
+    # Remove the q-points from the parsed data; these are only used to assign the symmetry labels to the right index
+    parsed_data.pop('q_points', None)
+
+    # Trim the number of irreps to the number of q-points finished in this run
+    parsed_data['number_of_irr_representations_for_each_q'] = parsed_data.get(
+        'number_of_irr_representations_for_each_q', []
+    )[:parsed_data.pop('num_q_found')]
+
     return parsed_data
 
 
 def parse_ph_dynmat(data, logs, lattice_parameter=None, also_eigenvectors=False, parse_header=False):
     """Parse frequencies and eigenvectors of a single dynamical matrix.
 
     :param data: the text read with the function readlines()
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_raw/pw.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_raw/pw.py`

 * *Files 2% similar despite different names*

```diff
@@ -246,14 +246,21 @@
             'history already reset at previous step: stopping': 'ERROR_IONIC_CYCLE_BFGS_HISTORY_FAILURE',
             'problems computing cholesky': 'ERROR_DIAGONALIZATION_CHOLESKY_DECOMPOSITION',
             'charge is wrong': 'ERROR_CHARGE_IS_WRONG',
             'not orthogonal operation': 'ERROR_SYMMETRY_NON_ORTHOGONAL_OPERATION',
             'problems computing cholesky': 'ERROR_COMPUTING_CHOLESKY',
             'dexx is negative': 'ERROR_DEXX_IS_NEGATIVE',
             'too many bands are not converged': 'ERROR_DIAGONALIZATION_TOO_MANY_BANDS_NOT_CONVERGED',
+            'S matrix not positive definite': 'ERROR_S_MATRIX_NOT_POSITIVE_DEFINITE',
+            'zhegvd failed': 'ERROR_ZHEGVD_FAILED',
+            '[Q, R] = qr(X, 0) failed': 'ERROR_QR_FAILED',
+            'probably because G_par is NOT a reciprocal lattice vector': 'ERROR_G_PAR',
+            'eigenvectors failed to converge': 'ERROR_EIGENVECTOR_CONVERGENCE',
+            'Error in routine broyden': 'ERROR_BROYDEN_FACTORIZATION',
+            'Not enough space allocated for radial FFT: try restarting with a larger cell_factor': 'ERROR_RADIAL_FFT_SIGNIFICANT_VOLUME_CONTRACTION',
             REG_ERROR_NPOOLS_TOO_HIGH: 'ERROR_NPOOLS_TOO_HIGH',
         },
         'warning': {
             'Warning:': None,
             'DEPRECATED:': None,
         }
     }
@@ -275,19 +282,20 @@
     for marker, message in message_map['warning'].items():
         if marker in line:
             if message is None:
                 message = line
             logs.warning.append(message)
 
 
-def parse_stdout(stdout, input_parameters, parser_options=None, parsed_xml=None):
+def parse_stdout(stdout, input_parameters, parser_options=None, parsed_xml=None, crash_file=None):
     """Parses the stdout content of a Quantum ESPRESSO `pw.x` calculation.
 
     :param stdout: the stdout content as a string
     :param input_parameters: dictionary with the input parameters
+    :param crash_file: the content of the ``CRASH`` file as a string if it was written, ``None`` otherwise.
     :param parser_options: the parser options from the settings input parameter node
     :param parsed_xml: dictionary with data parsed from the XML output file
     :returns: tuple of two dictionaries, with the parsed data and log messages, respectively
     """
     if parser_options is None:
         parser_options = {}
 
@@ -309,15 +317,16 @@
     marker_bfgs_converged = False
 
     # First check whether the `JOB DONE` message was written, otherwise the job was interrupted
     for line in data_lines:
         if 'JOB DONE' in line:
             break
     else:
-        logs.error.append('ERROR_OUTPUT_STDOUT_INCOMPLETE')
+        if crash_file is None:
+            logs.error.append('ERROR_OUTPUT_STDOUT_INCOMPLETE')
 
     # Determine whether the input switched on an electric field
     lelfield = input_parameters.get('CONTROL', {}).get('lelfield', False)
 
     # Find some useful quantities.
     if not parsed_xml.get('number_of_bands', None):
         try:
@@ -355,15 +364,15 @@
                 parsed_data['fft_grid'] = FFT_grid
                 parsed_data['smooth_fft_grid'] = smooth_FFT_grid
             except NameError:  # these are not crucial, so parsing does not fail if they are not found
                 pass
         except NameError:  # nat or other variables where not found, and thus not initialized
 
             # Try to get some error messages
-            lines = stdout.split('\n')
+            lines = stdout.split('\n') if crash_file is None else crash_file.split('\n')
 
             for line_number, line in enumerate(lines):
                 # Compare the line to the known set of error and warning messages and add them to the log container
                 detect_important_message(logs, line)
 
             if len(logs.error) or len(logs.warning) > 0:
                 parsed_data['trajectory'] = trajectory_data
@@ -836,30 +845,30 @@
 
         # End of trajectory frame, only keep last entries for dipole related values
         if lelfield is True:
 
             # For every property only get the last entry if possible
             try:
                 ed_cell = trajectory_frame['electronic_dipole_cell_average'].pop()
-            except IndexError:
+            except (IndexError, KeyError):
                 ed_cell = None
 
             try:
                 ed_axes = trajectory_frame['electronic_dipole_cartesian_axes'].pop()
-            except IndexError:
+            except (IndexError, KeyError):
                 ed_axes = None
 
             try:
                 id_cell = trajectory_frame['ionic_dipole_cell_average'].pop()
-            except IndexError:
+            except (IndexError, KeyError):
                 id_cell = None
 
             try:
                 id_axes = trajectory_frame['ionic_dipole_cartesian_axes'].pop()
-            except IndexError:
+            except (IndexError, KeyError):
                 id_axes = None
 
             # Only add them if all four properties were successfully parsed
             if all([value is not None for value in [ed_cell, ed_axes, id_cell, id_axes]]):
                 trajectory_data.setdefault('electronic_dipole_cell_average', []).append(ed_cell)
                 trajectory_data.setdefault('electronic_dipole_cartesian_axes', []).append(ed_axes)
                 trajectory_data.setdefault('ionic_dipole_cell_average', []).append(id_cell)
@@ -909,22 +918,31 @@
         logs.error.append('ERROR_IONIC_CONVERGENCE_NOT_REACHED')
 
     # Ionic calculation that hit the maximum number of ionic steps. Note: does not necessarily mean that convergence was
     # not reached as it could have occurred in the last step.
     if maximum_ionic_steps is not None and maximum_ionic_steps == parsed_data.get('number_ionic_steps', None):
         logs.warning.append('ERROR_MAXIMUM_IONIC_STEPS_REACHED')
 
-    # Remove duplicate log messages by turning it into a set. Then convert back to list as that is what is expected
-    logs.error = list(set(logs.error))
-    logs.warning = list(set(logs.warning))
-
     parsed_data['bands'] = bands_data
     parsed_data['structure'] = structure_data
     parsed_data['trajectory'] = trajectory_data
 
+    # Double check to detect error messages if CRASH is found
+    if crash_file is not None:
+        for line in crash_file.split('\n'):
+            # Compare the line to the known set of error and warning messages and add them to the log container
+            detect_important_message(logs, line)
+
+        if len(logs.error) == len(logs.warning) == 0:
+            raise QEOutputParsingError('Parser cannot load basic info.')
+
+    # Remove duplicate log messages by turning it into a set. Then convert back to list as that is what is expected
+    logs.error = list(set(logs.error))
+    logs.warning = list(set(logs.warning))
+
     return parsed_data, logs
 
 
 def grep_energy_from_line(line):
     try:
         return float(line.split('=')[1].split('Ry')[0]) * CONSTANTS.ry_to_ev
     except Exception:
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_raw/pw2gw.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_raw/pw2gw.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/cp/legacy.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/cp/legacy.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/legacy.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/legacy.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/parse.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/parse.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/pw/legacy.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/pw/legacy.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/pw/parse.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/pw/parse.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes-1.0.xsd` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes-1.0.xsd`

 * *Files 0% similar despite different names*

#### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes-1.0.xsd` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes-1.0.xsd`

```diff
@@ -166,15 +166,18 @@
       <enumeration value="from_scratch"/>
       <enumeration value="restart"/>
     </restriction>
   </simpleType>
   <simpleType name="lowhighType">
     <restriction base="string">
       <enumeration value="low"/>
+      <enumeration value="medium"/>
       <enumeration value="high"/>
+      <enumeration value="nowf"/>
+      <enumeration value="none"/>
     </restriction>
   </simpleType>
   <!-- INPUT TYPE -->
   <complexType name="atomic_speciesType">
     <sequence>
       <element type="qes:speciesType" name="species" maxOccurs="unbounded"/>
     </sequence>
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_030920.xsd` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_030920.xsd`

 * *Files 0% similar despite different names*

#### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_030920.xsd` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_030920.xsd`

```diff
@@ -184,15 +184,18 @@
       <enumeration value="from_scratch"/>
       <enumeration value="restart"/>
     </restriction>
   </simpleType>
   <simpleType name="lowhighType">
     <restriction base="string">
       <enumeration value="low"/>
+      <enumeration value="medium"/>
       <enumeration value="high"/>
+      <enumeration value="nowf"/>
+      <enumeration value="none"/>
     </restriction>
   </simpleType>
   <!-- INPUT TYPE -->
   <complexType name="atomic_speciesType">
     <sequence>
       <element type="qes:speciesType" name="species" maxOccurs="unbounded"/>
     </sequence>
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_190304.xsd` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_190304.xsd`

 * *Files 0% similar despite different names*

#### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_190304.xsd` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_190304.xsd`

```diff
@@ -184,15 +184,18 @@
       <enumeration value="from_scratch"/>
       <enumeration value="restart"/>
     </restriction>
   </simpleType>
   <simpleType name="lowhighType">
     <restriction base="string">
       <enumeration value="low"/>
+      <enumeration value="medium"/>
       <enumeration value="high"/>
+      <enumeration value="nowf"/>
+      <enumeration value="none"/>
     </restriction>
   </simpleType>
   <!-- INPUT TYPE -->
   <complexType name="atomic_speciesType">
     <sequence>
       <element type="qes:speciesType" name="species" maxOccurs="unbounded"/>
     </sequence>
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_191206.xsd` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_191206.xsd`

 * *Files 0% similar despite different names*

#### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_191206.xsd` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_191206.xsd`

```diff
@@ -184,15 +184,18 @@
       <enumeration value="from_scratch"/>
       <enumeration value="restart"/>
     </restriction>
   </simpleType>
   <simpleType name="lowhighType">
     <restriction base="string">
       <enumeration value="low"/>
+      <enumeration value="medium"/>
       <enumeration value="high"/>
+      <enumeration value="nowf"/>
+      <enumeration value="none"/>
     </restriction>
   </simpleType>
   <!-- INPUT TYPE -->
   <complexType name="atomic_speciesType">
     <sequence>
       <element type="qes:speciesType" name="species" maxOccurs="unbounded"/>
     </sequence>
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_200420.xsd` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_200420.xsd`

 * *Files 0% similar despite different names*

#### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_200420.xsd` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_200420.xsd`

```diff
@@ -184,15 +184,18 @@
       <enumeration value="from_scratch"/>
       <enumeration value="restart"/>
     </restriction>
   </simpleType>
   <simpleType name="lowhighType">
     <restriction base="string">
       <enumeration value="low"/>
+      <enumeration value="medium"/>
       <enumeration value="high"/>
+      <enumeration value="nowf"/>
+      <enumeration value="none"/>
     </restriction>
   </simpleType>
   <!-- INPUT TYPE -->
   <complexType name="atomic_speciesType">
     <sequence>
       <element type="qes:speciesType" name="species" maxOccurs="unbounded"/>
     </sequence>
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_210716.xsd` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_210716.xsd`

 * *Files 0% similar despite different names*

#### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_210716.xsd` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_210716.xsd`

```diff
@@ -184,15 +184,18 @@
       <enumeration value="from_scratch"/>
       <enumeration value="restart"/>
     </restriction>
   </simpleType>
   <simpleType name="lowhighType">
     <restriction base="string">
       <enumeration value="low"/>
+      <enumeration value="medium"/>
       <enumeration value="high"/>
+      <enumeration value="nowf"/>
+      <enumeration value="none"/>
     </restriction>
   </simpleType>
   <!-- INPUT TYPE -->
   <complexType name="atomic_speciesType">
     <sequence>
       <element type="qes:speciesType" name="species" maxOccurs="unbounded"/>
     </sequence>
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_211101.xsd` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_211101.xsd`

 * *Files 0% similar despite different names*

#### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_211101.xsd` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_211101.xsd`

```diff
@@ -187,15 +187,18 @@
       <enumeration value="from_scratch"/>
       <enumeration value="restart"/>
     </restriction>
   </simpleType>
   <simpleType name="lowhighType">
     <restriction base="string">
       <enumeration value="low"/>
+      <enumeration value="medium"/>
       <enumeration value="high"/>
+      <enumeration value="nowf"/>
+      <enumeration value="none"/>
     </restriction>
   </simpleType>
   <!-- INPUT TYPE -->
   <complexType name="atomic_speciesType">
     <sequence>
       <element type="qes:speciesType" name="species" maxOccurs="unbounded"/>
     </sequence>
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_220603.xsd` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_220603.xsd`

 * *Files 0% similar despite different names*

#### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_220603.xsd` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/schemas/qes_220603.xsd`

```diff
@@ -194,15 +194,18 @@
       <enumeration value="from_scratch"/>
       <enumeration value="restart"/>
     </restriction>
   </simpleType>
   <simpleType name="lowhighType">
     <restriction base="string">
       <enumeration value="low"/>
+      <enumeration value="medium"/>
       <enumeration value="high"/>
+      <enumeration value="nowf"/>
+      <enumeration value="none"/>
     </restriction>
   </simpleType>
   <!-- INPUT TYPE -->
   <complexType name="atomic_speciesType">
     <sequence>
       <element type="qes:speciesType" name="species" maxOccurs="unbounded"/>
     </sequence>
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/parse_xml/versions.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/parse_xml/versions.py`

 * *Files 3% similar despite different names*

```diff
@@ -13,35 +13,35 @@
     """An enum with the versions of XML output file known to exist for Quantum ESPRESSO."""
 
     PRE_6_2 = 0
     POST_6_2 = 1
 
 
 def get_xml_file_version(xml):
-    """Return the version of the Quantum ESPRESSO pw.x XML output file.
+    """Return the version of the Quantum ESPRESSO pw.x and cp.x XML output file.
 
     :param xml: the pre-parsed XML object
     :raises XMLUnsupportedFormatError: if the file cannot be read, parsed or if the version cannot be determined
     """
     if is_valid_post_6_2_version(xml):
         return QeXmlVersion.POST_6_2
     elif is_valid_pre_6_2_version(xml):
         return QeXmlVersion.PRE_6_2
     else:
-        raise XMLUnsupportedFormatError('unrecognized XML file version')
+        raise XMLUnsupportedFormatError(f'unrecognized XML file version: cannot find schema {get_schema_filename(xml)} in {os.path.join(os.path.dirname(os.path.abspath(__file__)), "schemas")}. You can look for it in https://github.com/QEF/qeschemas')
 
 
 def get_schema_filepath(xml):
     """Return the absolute filepath to the XML schema file that can be used to parse the given XML.
 
     :param xml: the pre-parsed XML object
     :return: the XSD absolute filepath
     """
     schema_directory = os.path.join(os.path.dirname(os.path.abspath(__file__)), 'schemas')
-    schema_filename = get_schema_filename(xml)  # if schema == 'pw' else 'qes_cp_devel_030920.xsd'
+    schema_filename = get_schema_filename(xml)
     schema_filepath = os.path.join(schema_directory, schema_filename)
 
     return schema_filepath
 
 
 def get_default_schema_filepath():
     """Return the absolute filepath to the default XML schema file.
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/ph.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/ph.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 import re
 import traceback
 
 from aiida import orm
 
 from aiida_quantumespresso.calculations.ph import PhCalculation
-from aiida_quantumespresso.parsers.parse_raw.ph import parse_raw_ph_output as parse_stdout
+from aiida_quantumespresso.parsers.parse_raw.ph import parse_raw_ph_output
 
 from .base import Parser
 
 
 class PhParser(Parser):
     """`Parser` implementation for the `PhCalculation` calculation job class."""
 
@@ -45,15 +45,15 @@
         for filename in sorted(retrieved.base.repository.list_object_names(dynmat_folder), key=natural_sort):
             if not filename.startswith(dynmat_prefix) or filename.endswith('.freq'):
                 continue
 
             dynmat_files.append(retrieved.base.repository.get_object_content(os.path.join(dynmat_folder, filename)))
 
         try:
-            parsed_data, logs = parse_stdout(stdout, tensor_file, dynmat_files)
+            parsed_data, logs = parse_raw_ph_output(stdout, tensor_file, dynmat_files)
         except Exception as exc:
             self.logger.error(traceback.format_exc())
             return self.exit(self.exit_codes.ERROR_UNEXPECTED_PARSER_EXCEPTION.format(exception=exc))
 
         self.emit_logs(logs)
         self.out('output_parameters', orm.Dict(parsed_data))
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/pp.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/pp.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/projwfc.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/projwfc.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/pw.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/pw.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 # -*- coding: utf-8 -*-
 """`Parser` implementation for the `PwCalculation` calculation job class."""
 import traceback
 
 from aiida import orm
 from aiida.common import exceptions
+from aiida.engine import ExitCode
 import numpy
 
+from aiida_quantumespresso.calculations.pw import PwCalculation
 from aiida_quantumespresso.utils.mapping import get_logging_container
 
 from .base import Parser
 from .parse_raw.pw import reduce_symmetries
 
 
 class PwParser(Parser):
@@ -18,15 +20,17 @@
     def parse(self, **kwargs):
         """Parse the retrieved files of a completed `PwCalculation` into output nodes.
 
         Two nodes that are expected are the default 'retrieved' `FolderData` node which will store the retrieved files
         permanently in the repository. The second required node is a filepath under the key `retrieved_temporary_files`
         which should contain the temporary retrieved files.
         """
+        # pylint: disable=too-many-statements
         dir_with_bands = None
+        crash_file = None
         self.exit_code_xml = None
         self.exit_code_stdout = None
         self.exit_code_parser = None
 
         try:
             settings = self.node.inputs.settings.get_dict()
         except exceptions.NotExistent:
@@ -38,17 +42,22 @@
         # Verify that the retrieved_temporary_folder is within the arguments if temporary files were specified
         if self.node.base.attributes.get('retrieve_temporary_list', None):
             try:
                 dir_with_bands = kwargs['retrieved_temporary_folder']
             except KeyError:
                 return self.exit(self.exit_codes.ERROR_NO_RETRIEVED_TEMPORARY_FOLDER)
 
+        # We check if the `CRASH` file was retrieved. If so, we parse its output
+        crash_file_filename = self.node.process_class._CRASH_FILE
+        if crash_file_filename in self.retrieved.base.repository.list_object_names():
+            crash_file = self.retrieved.base.repository.get_object_content(crash_file_filename)
+
         parameters = self.node.inputs.parameters.get_dict()
         parsed_xml, logs_xml = self.parse_xml(dir_with_bands, parser_options)
-        parsed_stdout, logs_stdout = self.parse_stdout(parameters, parser_options, parsed_xml)
+        parsed_stdout, logs_stdout = self.parse_stdout(parameters, parser_options, parsed_xml, crash_file)
 
         parsed_bands = parsed_stdout.pop('bands', {})
         parsed_structure = parsed_stdout.pop('structure', {})
         parsed_trajectory = parsed_stdout.pop('trajectory', {})
         parsed_parameters = self.build_output_parameters(parsed_stdout, parsed_xml)
 
         # Append the last frame of some of the smaller trajectory arrays to the parameters for easy querying
@@ -97,15 +106,34 @@
         # warnings from the schema parser about incomplete data, but that is to be expected in an initialization run.
         if settings.get('ONLY_INITIALIZATION', False):
             logs_xml.pop('error')
 
         ignore = ['Error while parsing ethr.', 'DEPRECATED: symmetry with ibrav=0, use correct ibrav instead']
         self.emit_logs([logs_stdout, logs_xml], ignore=ignore)
 
-        # First check for specific known problems that can cause a pre-mature termination of the calculation
+        # If either the stdout or XML were incomplete or corrupt investigate the potential cause
+        if self.exit_code_stdout or self.exit_code_xml:
+
+            # First check whether the scheduler already reported an exit code.
+            if self.node.exit_status is not None:
+
+                # The following scheduler errors should correspond to cases where we can simply restart the calculation
+                # and have a chance that the calculation will succeed as the error can be transient.
+                recoverable_scheduler_error = self.node.exit_status in [
+                    PwCalculation.exit_codes.ERROR_SCHEDULER_OUT_OF_WALLTIME.status,
+                    PwCalculation.exit_codes.ERROR_SCHEDULER_NODE_FAILURE.status,
+                ]
+
+                if self.get_calculation_type() in ['relax', 'vc-relax'] and recoverable_scheduler_error:
+                    return PwCalculation.exit_codes.ERROR_IONIC_INTERRUPTED_PARTIAL_TRAJECTORY
+
+                # Now it is unlikely we can provide a more specific exit code so we keep the scheduler one.
+                return ExitCode(self.node.exit_status, self.node.exit_message)
+
+        # Check for specific known problems that can cause a pre-mature termination of the calculation
         exit_code = self.validate_premature_exit(logs_stdout)
         if exit_code:
             return self.exit(exit_code)
 
         # If the both stdout and xml exit codes are set, there was a basic problem with both output files and there
         # is no need to investigate any further.
         if self.exit_code_stdout and self.exit_code_xml:
@@ -137,14 +165,21 @@
             'ERROR_OUT_OF_WALLTIME',
             'ERROR_CHARGE_IS_WRONG',
             'ERROR_SYMMETRY_NON_ORTHOGONAL_OPERATION',
             'ERROR_DEXX_IS_NEGATIVE',
             'ERROR_COMPUTING_CHOLESKY',
             'ERROR_NPOOLS_TOO_HIGH',
             'ERROR_DIAGONALIZATION_TOO_MANY_BANDS_NOT_CONVERGED',
+            'ERROR_S_MATRIX_NOT_POSITIVE_DEFINITE',
+            'ERROR_ZHEGVD_FAILED',
+            'ERROR_QR_FAILED',
+            'ERROR_G_PAR',
+            'ERROR_EIGENVECTOR_CONVERGENCE',
+            'ERROR_BROYDEN_FACTORIZATION',
+            'ERROR_RADIAL_FFT_SIGNIFICANT_VOLUME_CONTRACTION',
         ]:
             if error_label in logs['error']:
                 return self.exit_codes.get(error_label)
 
     def validate_electronic(self, trajectory, parameters, logs):
         """Analyze problems that are specific to `electronic` type calculations: i.e. `scf`, `nscf` and `bands`."""
         if self.get_calculation_type() not in ['scf', 'nscf', 'bands']:
@@ -223,36 +258,47 @@
         For a `relax` calculation this means the forces stored in the `trajectory` are all below the force convergence
         threshold which is retrieved from the input parameters. For a `vc-relax` calculation, the stress should also
         give a pressure that is below the pressure convergence threshold.
 
         :param trajectory: the output trajectory data
         :param except_final_scf: if True will return whether the calculation is converged except for the final scf.
         """
+        from aiida_quantumespresso.calculations import _uppercase_dict
         from aiida_quantumespresso.utils.defaults.calculation import pw
         from aiida_quantumespresso.utils.validation.trajectory import verify_convergence_trajectory
 
         relax_type = self.get_calculation_type()
         parameters = self.node.inputs.parameters.get_dict()
         threshold_forces = parameters.get('CONTROL', {}).get('forc_conv_thr', pw.forc_conv_thr)
         threshold_stress = parameters.get('CELL', {}).get('press_conv_thr', pw.press_conv_thr)
         external_pressure = parameters.get('CELL', {}).get('press', 0)
 
+        if 'settings' in self.node.inputs:
+            settings = _uppercase_dict(self.node.inputs.settings.get_dict(), dict_name='settings')
+
+        fixed_coords = settings.get('FIXED_COORDS', None)
+
         # Through the `cell_dofree` the degrees of freedom of the cell can be constrained, which makes the threshold on
         # the stress hard to interpret. Therefore, unless the `cell_dofree` is set to the default `all` where the cell
         # is fully unconstrained, the stress is ignored even if an explicit `press_conv_thr` is specified in the inputs.
         constrained_cell = parameters.get('CELL', {}).get('cell_dofree', 'all') != 'all'
 
         if constrained_cell:
             threshold_stress = None
 
         if relax_type == 'relax':
-            return verify_convergence_trajectory(trajectory, -1, *[threshold_forces, None])
+            return verify_convergence_trajectory(
+                trajectory=trajectory,
+                index=-1,
+                threshold_forces=threshold_forces,
+                fixed_coords=fixed_coords
+            )
 
         if relax_type == 'vc-relax':
-            values = [threshold_forces, threshold_stress, external_pressure]
+            values = [threshold_forces, threshold_stress, external_pressure, fixed_coords]
             converged_relax = verify_convergence_trajectory(trajectory, -2, *values)
             converged_final = verify_convergence_trajectory(trajectory, -1, *values)
 
             return converged_relax and (converged_final or except_final_scf)
 
         raise RuntimeError(f'unknown relax_type: {relax_type}')
 
@@ -292,15 +338,15 @@
             self.exit_code_xml = self.exit_codes.ERROR_OUTPUT_XML_FORMAT
         except Exception as exc:
             logs.critical.append(traceback.format_exc())
             self.exit_code_xml = self.exit_codes.ERROR_UNEXPECTED_PARSER_EXCEPTION.format(exception=exc)
 
         return parsed_data, logs
 
-    def parse_stdout(self, parameters, parser_options=None, parsed_xml=None):
+    def parse_stdout(self, parameters, parser_options=None, parsed_xml=None, crash_file=None):
         """Parse the stdout output file.
 
         :param parameters: the input parameters dictionary
         :param parser_options: optional dictionary with parser options
         :param parsed_xml: the raw parsed data from the XML output
         :return: tuple of two dictionaries, first with raw parsed data and second with log messages
         """
@@ -318,15 +364,15 @@
         try:
             stdout = self.retrieved.base.repository.get_object_content(filename_stdout)
         except IOError:
             self.exit_code_stdout = self.exit_codes.ERROR_OUTPUT_STDOUT_READ
             return parsed_data, logs
 
         try:
-            parsed_data, logs = parse_stdout(stdout, parameters, parser_options, parsed_xml)
+            parsed_data, logs = parse_stdout(stdout, parameters, parser_options, parsed_xml, crash_file)
         except Exception as exc:
             logs.critical.append(traceback.format_exc())
             self.exit_code_stdout = self.exit_codes.ERROR_UNEXPECTED_PARSER_EXCEPTION.format(exception=exc)
 
         # If the stdout was incomplete, most likely the job was interrupted before it could cleanly finish, so the
         # output files are most likely corrupt and cannot be restarted from
         if 'ERROR_OUTPUT_STDOUT_INCOMPLETE' in logs['error']:
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/pw2gw.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/pw2gw.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/pw2wannier90.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/pw2wannier90.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/q2r.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/q2r.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/parsers/xspectra.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/parsers/xspectra.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/tools/base.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/base.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/tools/calculations/pw.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/calculations/pw.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/tools/cpinputparser.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/cpinputparser.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/tools/data/orbital/noncollinearhydrogen.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/data/orbital/noncollinearhydrogen.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/tools/data/orbital/spinorbithydrogen.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/data/orbital/spinorbithydrogen.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/tools/pwinputparser.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/tools/pwinputparser.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/bands.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/bands.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/convert.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/convert.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/defaults/calculation/__init__.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/defaults/calculation/__init__.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/linalg.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/linalg.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/mapping.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/mapping.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/protocols/pw.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/protocols/pw.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/protocols/sssp_efficiency_1.0.json` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/protocols/sssp_efficiency_1.0.json`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/protocols/sssp_efficiency_1.1.json` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/protocols/sssp_efficiency_1.1.json`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/protocols/sssp_precision_1.0.json` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/protocols/sssp_precision_1.0.json`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/protocols/sssp_precision_1.1.json` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/protocols/sssp_precision_1.1.json`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/utils/restart.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/utils/restart.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/functions/create_kpoints_from_distance.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/functions/create_kpoints_from_distance.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/functions/seekpath_structure_analysis.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/functions/seekpath_structure_analysis.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/matdyn/base.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/matdyn/base.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/pdos.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/pdos.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/ph/base.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/ph/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,18 @@
 # -*- coding: utf-8 -*-
 """Workchain to run a Quantum ESPRESSO ph.x calculation with automated error handling and restarts."""
+from typing import Mapping
+
 from aiida import orm
 from aiida.common import AttributeDict
 from aiida.common.lang import type_check
 from aiida.engine import BaseRestartWorkChain, ProcessHandlerReport, process_handler, while_
 from aiida.plugins import CalculationFactory
 
+from aiida_quantumespresso.calculations.functions.merge_ph_outputs import merge_ph_outputs
 from aiida_quantumespresso.workflows.protocols.utils import ProtocolMixin
 
 PhCalculation = CalculationFactory('quantumespresso.ph')
 PwCalculation = CalculationFactory('quantumespresso.pw')
 
 
 class PhBaseWorkChain(ProtocolMixin, BaseRestartWorkChain):
@@ -34,22 +37,26 @@
             cls.setup,
             cls.validate_parameters,
             while_(cls.should_run_process)(
                 cls.prepare_process,
                 cls.run_process,
                 cls.inspect_process,
             ),
+            cls.create_merged_output,
             cls.results,
         )
         spec.expose_outputs(PhCalculation, exclude=('retrieved_folder',))
         spec.exit_code(204, 'ERROR_INVALID_INPUT_RESOURCES_UNDERSPECIFIED',
             message='The `metadata.options` did not specify both `resources.num_machines` and `max_wallclock_seconds`. '
                     'This exit status has been deprecated as the check it corresponded to was incorrect.')
         spec.exit_code(300, 'ERROR_UNRECOVERABLE_FAILURE',
             message='The calculation failed with an unrecoverable error.')
+        spec.exit_code(401, 'ERROR_MERGING_QPOINTS',
+            message='The work chain failed to merge the q-points data from multiple `PhCalculation`s because not all '
+                    'q-points were parsed.')
         # yapf: enable
 
     @classmethod
     def get_protocol_filepath(cls):
         """Return ``pathlib.Path`` to the ``.yaml`` file that defines the protocols."""
         from importlib_resources import files
 
@@ -142,14 +149,50 @@
         if max_wallclock_seconds is not None and 'max_seconds' not in self.ctx.inputs.parameters['INPUTPH']:
             self.set_max_seconds(max_wallclock_seconds)
 
         if self.ctx.restart_calc:
             self.ctx.inputs.parameters['INPUTPH']['recover'] = True
             self.ctx.inputs.parent_folder = self.ctx.restart_calc.outputs.remote_folder
 
+    def create_merged_output(self):
+        """Merge outputs from multiple ``PhCalculation`` runs called by the workchain if necessary."""
+        if self.inputs.only_initialization.value:
+            return
+
+        if len(self.ctx.children) == 1:
+            return
+
+        output_dict = {
+            'output_' + str(index + 1): child.outputs.output_parameters
+            for index, child in enumerate(self.ctx.children)
+        }
+
+        num_qpoints = self.ctx.children[0].outputs.output_parameters['number_of_qpoints']
+        num_qpoints = self.ctx.inputs.parameters['INPUTPH'].get('last_q', num_qpoints) \
+            - self.ctx.inputs.parameters['INPUTPH'].get('start_q', 1) + 1
+        num_qpoints_found = sum(
+            len(output['number_of_irr_representations_for_each_q']) for output in output_dict.values()
+        )
+
+        if num_qpoints_found == num_qpoints:
+            self.report(f'Merging {num_qpoints} q-points data from `PhCalculation`s.')
+            self.ctx.merged_output_parameters = merge_ph_outputs(**output_dict)
+        else:
+            self.report(f'Only {num_qpoints_found} of {num_qpoints} q-points were parsed.')
+            return self.exit_codes.ERROR_MERGING_QPOINTS
+
+    def get_outputs(self, node) -> Mapping[str, orm.Node]:
+        """Return a mapping of the outputs that should be attached as outputs to the work chain."""
+        outputs = super().get_outputs(node)
+
+        if 'merged_output_parameters' in self.ctx:
+            outputs['output_parameters'] = self.ctx.merged_output_parameters
+
+        return outputs
+
     def report_error_handled(self, calculation, action):
         """Report an action taken for a calculation that has failed.
 
         This should be called in a registered error handler if its condition is met and an action was taken.
 
         :param calculation: the failed calculation node
         :param action: a string message with the action taken
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/protocols/core_hole_treatments.yaml` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/core_hole_treatments.yaml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/protocols/magnetization.yaml` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/magnetization.yaml`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/protocols/pdos.yaml` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/pdos.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 default_inputs:
-    clean_workdir: True
+    clean_workdir: False
     scf:
         pw:
             parameters:
                 CONTROL:
                     restart_mode: from_scratch
     nscf:
         kpoints_distance: 0.10
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/protocols/ph/base.yaml` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/ph/base.yaml`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 default_inputs:
-    clean_workdir: True
+    clean_workdir: False
     ph:
         metadata:
             options:
                 resources:
                     num_machines: 1
                 max_wallclock_seconds: 43200  # Twelve hours
                 withmpi: True
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/protocols/pw/base.yaml` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/pw/base.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 default_inputs:
-    clean_workdir: True
+    clean_workdir: False
     kpoints_distance: 0.15
     kpoints_force_parity: False
     meta_parameters:
         conv_thr_per_atom: 0.2e-9
         etot_conv_thr_per_atom: 1.e-5
     pseudo_family: 'SSSP/1.2/PBEsol/efficiency'
     pw:
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/protocols/pw/relax.yaml` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/pw/relax.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 default_inputs:
-    clean_workdir: True
+    clean_workdir: False
     max_meta_convergence_iterations: 5
     meta_convergence: True
     volume_convergence: 0.02
     base:
         pw:
             parameters:
                 CELL:
                     press_conv_thr: 0.5
     base_final_scf:
         pw:
             parameters:
-                CELL:
-                    press_conv_thr: 0.5
+                CONTROL:
+                    calculation: scf
 default_protocol: moderate
 protocols:
     moderate:
         description: 'Protocol to perform a relaxation at normal precision at moderate computational cost.'
     precise:
         description: 'Protocol to perform a relaxation at high precision at higher computational cost.'
         volume_convergence: 0.01
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/protocols/utils.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/utils.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/protocols/xspectra/base.yaml` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/xspectra/base.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 default_inputs:
-    clean_workdir: True
+    clean_workdir: False
     kpoints_distance: 0.15
     kpoints_force_parity: False
     xspectra:
         parameters:
             INPUT_XSPECTRA:
                 calculation: xanes_dipole
                 xonly_plot: False
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/protocols/xspectra/core.yaml` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/protocols/xspectra/core.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 default_inputs:
     abs_atom_marker: X
-    clean_workdir: True
+    clean_workdir: False
     get_powder_spectrum: False
     run_replot: False
     eps_vectors:
         - [1., 0., 0.]
         - [0., 1., 0.]
         - [0., 0., 1.]
 default_protocol: moderate
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/pw/bands.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/pw/bands.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,21 @@
 # -*- coding: utf-8 -*-
 """Workchain to compute a band structure for a given structure using Quantum ESPRESSO pw.x."""
 from aiida import orm
 from aiida.common import AttributeDict
 from aiida.engine import ToContext, WorkChain, if_
-from aiida.plugins import WorkflowFactory
 
 from aiida_quantumespresso.calculations.functions.seekpath_structure_analysis import seekpath_structure_analysis
+from aiida_quantumespresso.calculations.pw import PwCalculation
 from aiida_quantumespresso.utils.mapping import prepare_process_inputs
+from aiida_quantumespresso.workflows.pw.base import PwBaseWorkChain
+from aiida_quantumespresso.workflows.pw.relax import PwRelaxWorkChain
 
 from ..protocols.utils import ProtocolMixin
 
-PwBaseWorkChain = WorkflowFactory('quantumespresso.pw.base')
-PwRelaxWorkChain = WorkflowFactory('quantumespresso.pw.relax')
-
 
 def validate_inputs(inputs, ctx=None):  # pylint: disable=unused-argument
     """Validate the inputs of the entire input namespace."""
     # pylint: disable=no-member
 
     if 'nbands_factor' in inputs and 'nbnd' in inputs['bands']['pw']['parameters'].base.attributes.get('SYSTEM', {}):
         return PwBandsWorkChain.exit_codes.ERROR_INVALID_INPUT_NUMBER_OF_BANDS.message
@@ -68,14 +67,15 @@
             help='If `True`, work directories of all called calculation will be cleaned at the end of execution.')
         spec.input('nbands_factor', valid_type=orm.Float, required=False,
             help='The number of bands for the BANDS calculation is that used for the SCF multiplied by this factor.')
         spec.input('bands_kpoints', valid_type=orm.KpointsData, required=False,
             help='Explicit kpoints to use for the BANDS calculation. Specify either this or `bands_kpoints_distance`.')
         spec.input('bands_kpoints_distance', valid_type=orm.Float, required=False,
             help='Minimum kpoints distance for the BANDS calculation. Specify either this or `bands_kpoints`.')
+        spec.inputs['bands']['pw'].validator = PwCalculation.validate_inputs_base
         spec.inputs.validator = validate_inputs
         spec.outline(
             cls.setup,
             if_(cls.should_run_relax)(
                 cls.run_relax,
                 cls.inspect_relax,
             ),
@@ -224,21 +224,20 @@
         self.out('seekpath_parameters', result['parameters'])
 
     def run_scf(self):
         """Run the PwBaseWorkChain in scf mode on the primitive cell of (optionally relaxed) input structure."""
         inputs = AttributeDict(self.exposed_inputs(PwBaseWorkChain, namespace='scf'))
         inputs.metadata.call_link_label = 'scf'
         inputs.pw.structure = self.ctx.current_structure
-        inputs.pw.parameters = inputs.pw.parameters.get_dict()
-        inputs.pw.parameters.setdefault('CONTROL', {})['calculation'] = 'scf'
 
         # Make sure to carry the number of bands from the relax workchain if it was run and it wasn't explicitly defined
         # in the inputs. One of the base workchains in the relax workchain may have changed the number automatically in
         #  the sanity checks on band occupations.
         if self.ctx.current_number_of_bands:
+            inputs.pw.parameters = inputs.pw.parameters.get_dict()
             inputs.pw.parameters.setdefault('SYSTEM', {}).setdefault('nbnd', self.ctx.current_number_of_bands)
 
         inputs = prepare_process_inputs(PwBaseWorkChain, inputs)
         running = self.submit(PwBaseWorkChain, **inputs)
 
         self.report(f'launching PwBaseWorkChain<{running.pk}> in scf mode')
 
@@ -263,21 +262,14 @@
         inputs.pw.structure = self.ctx.current_structure
         inputs.pw.parent_folder = self.ctx.current_folder
         inputs.pw.parameters = inputs.pw.parameters.get_dict()
         inputs.pw.parameters.setdefault('CONTROL', {})
         inputs.pw.parameters.setdefault('SYSTEM', {})
         inputs.pw.parameters.setdefault('ELECTRONS', {})
 
-        # The following flags always have to be set in the parameters, regardless of what caller specified in the inputs
-        inputs.pw.parameters['CONTROL']['calculation'] = 'bands'
-
-        # Only set the following parameters if not directly explicitly defined in the inputs
-        inputs.pw.parameters['ELECTRONS'].setdefault('diagonalization', 'cg')
-        inputs.pw.parameters['ELECTRONS'].setdefault('diago_full_acc', True)
-
         # If `nbands_factor` is defined in the inputs we set the `nbnd` parameter
         if 'nbands_factor' in self.inputs:
             factor = self.inputs.nbands_factor.value
             parameters = self.ctx.workchain_scf.outputs.output_parameters.get_dict()
             nbands = int(parameters['number_of_bands'])
             nelectron = int(parameters['number_of_electrons'])
             nbnd = max(int(0.5 * nelectron * factor), int(0.5 * nelectron) + 4, nbands)
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/pw/base.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/pw/base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,18 @@
 # -*- coding: utf-8 -*-
 """Workchain to run a Quantum ESPRESSO pw.x calculation with automated error handling and restarts."""
 from aiida import orm
 from aiida.common import AttributeDict, exceptions
 from aiida.common.lang import type_check
-from aiida.engine import BaseRestartWorkChain, ExitCode, ProcessHandlerReport, ToContext, if_, process_handler, while_
+from aiida.engine import BaseRestartWorkChain, ExitCode, ProcessHandlerReport, process_handler, while_
 from aiida.plugins import CalculationFactory, GroupFactory
 
 from aiida_quantumespresso.calculations.functions.create_kpoints_from_distance import create_kpoints_from_distance
 from aiida_quantumespresso.common.types import ElectronicType, RestartType, SpinType
 from aiida_quantumespresso.utils.defaults.calculation import pw as qe_defaults
-from aiida_quantumespresso.utils.mapping import prepare_process_inputs, update_mapping
-from aiida_quantumespresso.utils.resources import (
-    cmdline_remove_npools,
-    create_scheduler_resources,
-    get_default_options,
-    get_pw_parallelization_parameters,
-)
 
 from ..protocols.utils import ProtocolMixin
 
 PwCalculation = CalculationFactory('quantumespresso.pw')
 SsspFamily = GroupFactory('pseudo.family.sssp')
 PseudoDojoFamily = GroupFactory('pseudo.family.pseudo_dojo')
 CutoffsPseudoPotentialFamily = GroupFactory('pseudo.family.cutoffs')
@@ -54,52 +47,44 @@
         spec.input('kpoints_distance', valid_type=orm.Float, required=False,
             help='The minimum desired distance in 1/Å between k-points in reciprocal space. The explicit k-points will '
                  'be generated automatically by a calculation function based on the input structure.')
         spec.input('kpoints_force_parity', valid_type=orm.Bool, required=False,
             help='Optional input when constructing the k-points based on a desired `kpoints_distance`. Setting this to '
                  '`True` will force the k-point mesh to have an even number of points along each lattice vector except '
                  'for any non-periodic directions.')
-        spec.input('automatic_parallelization', valid_type=orm.Dict, required=False,
-            help='When defined, the work chain will first launch an initialization calculation to determine the '
-                 'dimensions of the problem, and based on this it will try to set optimal parallelization flags.')
 
         spec.outline(
             cls.setup,
             cls.validate_kpoints,
-            if_(cls.should_run_init)(
-                cls.validate_init_inputs,
-                cls.run_init,
-                cls.inspect_init,
-            ),
             while_(cls.should_run_process)(
                 cls.prepare_process,
                 cls.run_process,
                 cls.inspect_process,
             ),
             cls.results,
         )
 
         spec.expose_outputs(PwCalculation)
-        spec.output('automatic_parallelization', valid_type=orm.Dict, required=False,
-            help='The results of the automatic parallelization analysis if performed.')
 
         spec.exit_code(201, 'ERROR_INVALID_INPUT_PSEUDO_POTENTIALS',
             message='The explicit `pseudos` or `pseudo_family` could not be used to get the necessary pseudos.')
         spec.exit_code(202, 'ERROR_INVALID_INPUT_KPOINTS',
             message='Neither the `kpoints` nor the `kpoints_distance` input was specified.')
         spec.exit_code(203, 'ERROR_INVALID_INPUT_RESOURCES',
             message='Neither the `options` nor `automatic_parallelization` input was specified. '
                     'This exit status has been deprecated as the check it corresponded to was incorrect.')
         spec.exit_code(204, 'ERROR_INVALID_INPUT_RESOURCES_UNDERSPECIFIED',
             message='The `metadata.options` did not specify both `resources.num_machines` and `max_wallclock_seconds`. '
                     'This exit status has been deprecated as the check it corresponded to was incorrect.')
         spec.exit_code(210, 'ERROR_INVALID_INPUT_AUTOMATIC_PARALLELIZATION_MISSING_KEY',
-            message='Required key for `automatic_parallelization` was not specified.')
+            message='Required key for `automatic_parallelization` was not specified.'
+                    'This exit status has been deprecated as the automatic parallellization feature was removed.')
         spec.exit_code(211, 'ERROR_INVALID_INPUT_AUTOMATIC_PARALLELIZATION_UNRECOGNIZED_KEY',
-            message='Unrecognized keys were specified for `automatic_parallelization`.')
+            message='Unrecognized keys were specified for `automatic_parallelization`.'
+                    'This exit status has been deprecated as the automatic parallellization feature was removed.')
         spec.exit_code(300, 'ERROR_UNRECOVERABLE_FAILURE',
             message='The calculation failed with an unidentified unrecoverable error.')
         spec.exit_code(310, 'ERROR_KNOWN_UNRECOVERABLE_FAILURE',
             message='The calculation failed with a known unrecoverable error.')
         spec.exit_code(320, 'ERROR_INITIALIZATION_CALCULATION_FAILED',
             message='The initialization calculation failed.')
         spec.exit_code(501, 'ERROR_IONIC_CONVERGENCE_REACHED_EXCEPT_IN_FINAL_SCF',
@@ -191,14 +176,18 @@
         # Update the parameters based on the protocol inputs
         parameters = inputs['pw']['parameters']
         parameters['CONTROL']['etot_conv_thr'] = natoms * meta_parameters['etot_conv_thr_per_atom']
         parameters['ELECTRONS']['conv_thr'] = natoms * meta_parameters['conv_thr_per_atom']
         parameters['SYSTEM']['ecutwfc'] = cutoff_wfc
         parameters['SYSTEM']['ecutrho'] = cutoff_rho
 
+        #If the structure is 2D periodic in the x-y plane, we set assume_isolate to `2D`
+        if structure.pbc == (True, True, False):
+            parameters['SYSTEM']['assume_isolated'] = '2D'
+
         if electronic_type is ElectronicType.INSULATOR:
             parameters['SYSTEM']['occupations'] = 'fixed'
             parameters['SYSTEM'].pop('degauss')
             parameters['SYSTEM'].pop('smearing')
 
         if spin_type is SpinType.COLLINEAR:
             starting_magnetization = get_starting_magnetization(structure, pseudo_family, initial_magnetic_moments)
@@ -251,25 +240,17 @@
         super().setup()
         self.ctx.inputs = AttributeDict(self.exposed_inputs(PwCalculation, 'pw'))
 
         self.ctx.inputs.parameters = self.ctx.inputs.parameters.get_dict()
         self.ctx.inputs.parameters.setdefault('CONTROL', {})
         self.ctx.inputs.parameters.setdefault('ELECTRONS', {})
         self.ctx.inputs.parameters.setdefault('SYSTEM', {})
-        self.ctx.inputs.parameters['CONTROL'].setdefault('calculation', 'scf')
 
         self.ctx.inputs.settings = self.ctx.inputs.settings.get_dict() if 'settings' in self.ctx.inputs else {}
 
-        # If a ``parent_folder`` is specified, automatically set the parameters for a ``RestartType.Full`` unless the
-        # ``CONTROL.restart_mode`` has explicitly been set to ``from_scratch``. In that case, the user most likely set
-        # that, and we do not want to override it.
-        restart_mode = self.ctx.inputs.parameters['CONTROL'].get('restart_mode', None)
-        if 'parent_folder' in self.ctx.inputs and restart_mode != 'from_scratch':
-            self.set_restart_type(RestartType.FULL, self.ctx.inputs.parent_folder)
-
     def validate_kpoints(self):
         """Validate the inputs related to k-points.
 
         Either an explicit `KpointsData` with given mesh/path, or a desired k-points distance should be specified. In
         the case of the latter, the `KpointsData` will be constructed for the input `StructureData` using the
         `create_kpoints_from_distance` calculation function.
         """
@@ -287,23 +268,14 @@
                     'call_link_label': 'create_kpoints_from_distance'
                 }
             }
             kpoints = create_kpoints_from_distance(**inputs)  # pylint: disable=unexpected-keyword-arg
 
         self.ctx.inputs.kpoints = kpoints
 
-    def set_max_seconds(self, max_wallclock_seconds):
-        """Set the `max_seconds` to a fraction of `max_wallclock_seconds` option to prevent out-of-walltime problems.
-
-        :param max_wallclock_seconds: the maximum wallclock time that will be set in the scheduler settings.
-        """
-        max_seconds_factor = self.defaults.delta_factor_max_seconds
-        max_seconds = max_wallclock_seconds * max_seconds_factor
-        self.ctx.inputs.parameters['CONTROL']['max_seconds'] = max_seconds
-
     def set_restart_type(self, restart_type, parent_folder=None):
         """Set the restart type for the next iteration."""
 
         if parent_folder is None and restart_type != RestartType.FROM_SCRATCH:
             raise ValueError('When not restarting from scratch, a `parent_folder` must be provided.')
 
         if restart_type == RestartType.FROM_SCRATCH:
@@ -326,121 +298,21 @@
 
         elif restart_type == RestartType.FROM_WAVE_FUNCTIONS:
             self.ctx.inputs.parameters['CONTROL']['restart_mode'] = 'from_scratch'
             self.ctx.inputs.parameters['ELECTRONS'].pop('startingpot', None)
             self.ctx.inputs.parameters['ELECTRONS']['startingwfc'] = 'file'
             self.ctx.inputs.parent_folder = parent_folder
 
-    def should_run_init(self):
-        """Return whether an initialization calculation should be run.
-
-        :return: boolean, `True` if `automatic_parallelization` was specified in the inputs, `False` otherwise.
-        """
-        return 'automatic_parallelization' in self.inputs
-
-    def validate_init_inputs(self):
-        """Validate the inputs that are required for the initialization calculation.
-
-        The `automatic_parallelization` input expects a `Dict` node with the following keys:
-
-            * max_wallclock_seconds
-            * target_time_seconds
-            * max_num_machines
-
-        If any of these keys are not set or any superfluous keys are specified, the workchain will abort.
-        """
-        parallelization = self.inputs.automatic_parallelization.get_dict()
-
-        expected_keys = ['max_wallclock_seconds', 'target_time_seconds', 'max_num_machines']
-        received_keys = [(key, parallelization.get(key, None)) for key in expected_keys]
-        remaining_keys = [key for key in parallelization.keys() if key not in expected_keys]
-
-        for key, value in [(key, value) for key, value in received_keys if value is None]:
-            self.report(f'required key "{key}" in automatic_parallelization input not found')
-            return self.exit_codes.ERROR_INVALID_INPUT_AUTOMATIC_PARALLELIZATION_MISSING_KEY
-
-        if remaining_keys:
-            self.report(
-                f"detected unrecognized keys in the automatic_parallelization input: {' '.join(remaining_keys)}"
-            )
-            return self.exit_codes.ERROR_INVALID_INPUT_AUTOMATIC_PARALLELIZATION_UNRECOGNIZED_KEY
-
-        # Add the calculation mode to the automatic parallelization dictionary
-        self.ctx.automatic_parallelization = {
-            'max_wallclock_seconds': parallelization['max_wallclock_seconds'],
-            'target_time_seconds': parallelization['target_time_seconds'],
-            'max_num_machines': parallelization['max_num_machines'],
-            'calculation_mode': self.ctx.inputs.parameters['CONTROL']['calculation']
-        }
-
-        options = self.ctx.inputs.metadata['options']
-        options.setdefault('resources', {})['num_machines'] = parallelization['max_num_machines']
-        options['max_wallclock_seconds'] = parallelization['max_wallclock_seconds']
-
-    def run_init(self):
-        """Run an initialization `PwCalculation` that will exit after the preamble.
-
-        In the preamble, all the relevant dimensions of the problem are computed which allows us to make an estimate of
-        the required resources and what parallelization flags need to be set.
-        """
-        inputs = self.ctx.inputs
-
-        # Set the initialization flag and the initial default options
-        inputs.settings['ONLY_INITIALIZATION'] = True
-        inputs.metadata['options'] = update_mapping(inputs.metadata['options'], get_default_options())
-
-        # Prepare the final input dictionary
-        inputs = prepare_process_inputs(PwCalculation, inputs)
-        running = self.submit(PwCalculation, **inputs)
-
-        self.report(f'launching initialization {running.pk}<{self.ctx.process_name}>')
-
-        return ToContext(calculation_init=running)
-
-    def inspect_init(self):
-        """Use the initialization `PwCalculation` to determine the required resource and parallelization settings."""
-        calculation = self.ctx.calculation_init
-
-        if not calculation.is_finished_ok:
-            return self.exit_codes.ERROR_INITIALIZATION_CALCULATION_FAILED
-
-        # Get automated parallelization settings
-        parallelization = get_pw_parallelization_parameters(calculation, **self.ctx.automatic_parallelization)
-
-        # Note: don't do this at home, we are losing provenance here. This should be done by a calculation function
-        node = orm.Dict(parallelization).store()
-        self.out('automatic_parallelization', node)
-        self.report(f'results of automatic parallelization in {node.__class__.__name__}<{node.pk}>')
-
-        options = self.ctx.inputs.metadata['options']
-        base_resources = options.get('resources', {})
-        goal_resources = parallelization['resources']
-
-        scheduler = calculation.computer.get_scheduler()
-        resources = create_scheduler_resources(scheduler, base_resources, goal_resources)
-
-        cmdline = self.ctx.inputs.settings.get('cmdline', [])
-        cmdline = cmdline_remove_npools(cmdline)
-        cmdline.extend(['-nk', str(parallelization['npools'])])
-
-        # Set the new cmdline setting and resource options
-        self.ctx.inputs.settings['cmdline'] = cmdline
-        self.ctx.inputs.metadata['options'] = update_mapping(options, {'resources': resources})
-
-        # Remove the only initialization flag
-        self.ctx.inputs.settings.pop('ONLY_INITIALIZATION')
-
-        return
-
     def prepare_process(self):
         """Prepare the inputs for the next calculation."""
         max_wallclock_seconds = self.ctx.inputs.metadata.options.get('max_wallclock_seconds', None)
 
         if max_wallclock_seconds is not None and 'max_seconds' not in self.ctx.inputs.parameters['CONTROL']:
-            self.set_max_seconds(max_wallclock_seconds)
+            max_seconds = max_wallclock_seconds * self.defaults.delta_factor_max_seconds
+            self.ctx.inputs.parameters['CONTROL']['max_seconds'] = max_seconds
 
     def report_error_handled(self, calculation, action):
         """Report an action taken for a calculation that has failed.
 
         This should be called in a registered error handler if its condition is met and an action was taken.
 
         :param calculation: the failed calculation node
@@ -517,32 +389,47 @@
         return ProcessHandlerReport(True, self.exit_codes.ERROR_KNOWN_UNRECOVERABLE_FAILURE)
 
     @process_handler(
         priority=585,
         exit_codes=[
             PwCalculation.exit_codes.ERROR_COMPUTING_CHOLESKY,
             PwCalculation.exit_codes.ERROR_DIAGONALIZATION_TOO_MANY_BANDS_NOT_CONVERGED,
+            PwCalculation.exit_codes.ERROR_S_MATRIX_NOT_POSITIVE_DEFINITE,
+            PwCalculation.exit_codes.ERROR_ZHEGVD_FAILED,
+            PwCalculation.exit_codes.ERROR_QR_FAILED,
+            PwCalculation.exit_codes.ERROR_EIGENVECTOR_CONVERGENCE,
+            PwCalculation.exit_codes.ERROR_BROYDEN_FACTORIZATION,
         ]
     )
     def handle_diagonalization_errors(self, calculation):
         """Handle known issues related to the diagonalization.
 
-        Switch to ``diagonalization = 'cg'`` if not already running with this setting, and restart from the charge
-        density. In case the run already used conjugate gradient diagonalization, abort.
+        We use the following strategy. When a diagonalization algorithm fails, we try using an other one
+        still not used. Conjugate gradient (CG) is kept as last option, as it is the slowest among the
+        available ones, but on the contrary it is the most stable as well, thus kept as `last resort`.
+
+        Once the error handler has tried all ``diagonalization`` options, abort.
         """
-        if self.ctx.inputs.parameters['ELECTRONS'].get('diagonalization', None) == 'cg':
-            action = 'found diagonalization issues but already running with conjugate gradient algorithm, aborting...'
+        current = self.ctx.inputs.parameters['ELECTRONS'].get('diagonalization', 'david')
+
+        if 'diagonalizations' not in self.ctx:
+            # Initialize a list to track diagonalisations that haven't been tried in reverse order or preference
+            self.ctx.diagonalizations = [value for value in ['cg', 'paro', 'ppcg', 'david'] if value != current.lower()]
+
+        try:
+            new = self.ctx.diagonalizations.pop()
+            self.ctx.inputs.parameters['ELECTRONS']['diagonalization'] = new
+            action = f'found diagonalization issues for ``{current}``, switching to ``{new}`` diagonalization.'
+            self.report_error_handled(calculation, action)
+            return ProcessHandlerReport(True)
+        except IndexError:
+            action = 'found diagonalization issues but already exploited all supported algorithms, aborting...'
             self.report_error_handled(calculation, action)
             return ProcessHandlerReport(True, self.exit_codes.ERROR_KNOWN_UNRECOVERABLE_FAILURE)
 
-        self.ctx.inputs.parameters['ELECTRONS']['diagonalization'] = 'cg'
-        action = 'found diagonalization issues, switching to conjugate gradient diagonalization.'
-        self.report_error_handled(calculation, action)
-        return ProcessHandlerReport(True)
-
     @process_handler(priority=580, exit_codes=[
         PwCalculation.exit_codes.ERROR_OUT_OF_WALLTIME,
     ])
     def handle_out_of_walltime(self, calculation):
         """Handle `ERROR_OUT_OF_WALLTIME` exit code.
 
         In this case the calculation shut down neatly and we can simply restart. We consider two cases:
@@ -557,14 +444,29 @@
             self.report_error_handled(calculation, 'simply restart from the last calculation')
         else:
             self.set_restart_type(RestartType.FROM_SCRATCH)
             self.report_error_handled(calculation, 'out of walltime: structure changed so restarting from scratch')
 
         return ProcessHandlerReport(True)
 
+    @process_handler(priority=575, exit_codes=[
+        PwCalculation.exit_codes.ERROR_IONIC_INTERRUPTED_PARTIAL_TRAJECTORY,
+    ])
+    def handle_ionic_interrupted_partial_trajectory(self, calculation):
+        """Handle `ERROR_IONIC_INTERRUPTED_PARTIAL_TRAJECTORY` exit code.
+
+        In this case the calculation got interrupted during an ionic optimization due to a problem that is likely
+        transient, so we can restart from the last output structure. Note that since the job got interrupted the charge
+        density and wave functions are likely corrupt so those cannot be used in the restart.
+        """
+        self.ctx.inputs.structure = calculation.outputs.output_structure
+        self.set_restart_type(RestartType.FROM_SCRATCH)
+        self.report_error_handled(calculation, 'restarting from scratch from the last output structure')
+        return ProcessHandlerReport(True)
+
     @process_handler(
         priority=570, exit_codes=[
             PwCalculation.exit_codes.ERROR_IONIC_CONVERGENCE_REACHED_EXCEPT_IN_FINAL_SCF,
         ]
     )
     def handle_vcrelax_converged_except_final_scf(self, calculation):
         """Handle `ERROR_IONIC_CONVERGENCE_REACHED_EXCEPT_IN_FINAL_SCF` exit code.
@@ -596,14 +498,40 @@
         action = 'no ionic convergence but clean shutdown: restarting from scratch but using output structure.'
 
         self.set_restart_type(RestartType.FROM_SCRATCH)
         self.report_error_handled(calculation, action)
         return ProcessHandlerReport(True)
 
     @process_handler(
+        priority=559, exit_codes=[
+            PwCalculation.exit_codes.ERROR_RADIAL_FFT_SIGNIFICANT_VOLUME_CONTRACTION,
+        ]
+    )
+    def handle_vcrelax_recoverable_fft_significant_volume_contraction_error(self, calculation):
+        """Handle exit code for recoverable `vc-relax` calculations with significant volume contraction.
+
+        This exit code appears when a cell relaxation produces a significant volume scaling (contraction or expansion).
+        This means the pseudopotentials tables must be recalculated. This parameter is controlled by `CELL.cell_factor`.
+        The solution, as suggested by the QuantumESPRESSO error itself, is to restart with an increased `cell_factor`.
+        We then start from scratch using the last output structure and we double the cell factor.
+        """
+        self.ctx.inputs.structure = calculation.outputs.output_structure
+        self.ctx.inputs.parameters.setdefault('CELL', {})  # as it is not compulsory for ``vc-relax`` calculations
+        cell_factor = 2 * self.ctx.inputs.parameters['CELL'].get('cell_factor', 2)
+        self.ctx.inputs.parameters['CELL']['cell_factor'] = cell_factor
+
+        self.set_restart_type(RestartType.FROM_SCRATCH)
+        action = (
+            'significant volume scaling but clean shutdown: '
+            f'restarting from scratch using output structure and ``cell_factor = {cell_factor}``.'
+        )
+        self.report_error_handled(calculation, action)
+        return ProcessHandlerReport(True)
+
+    @process_handler(
         priority=550,
         exit_codes=[
             PwCalculation.exit_codes.ERROR_IONIC_CYCLE_ELECTRONIC_CONVERGENCE_NOT_REACHED,
             PwCalculation.exit_codes.ERROR_IONIC_CONVERGENCE_REACHED_FINAL_SCF_FAILED,
         ]
     )
     def handle_relax_recoverable_electronic_convergence_error(self, calculation):
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/pw/relax.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/pw/relax.py`

 * *Files 2% similar despite different names*

```diff
@@ -139,15 +139,26 @@
         if relax_type in (RelaxType.VOLUME, RelaxType.POSITIONS_VOLUME):
             base.pw.parameters['CELL']['cell_dofree'] = 'volume'
 
         if relax_type in (RelaxType.SHAPE, RelaxType.POSITIONS_SHAPE):
             base.pw.parameters['CELL']['cell_dofree'] = 'shape'
 
         if relax_type in (RelaxType.CELL, RelaxType.POSITIONS_CELL):
-            base.pw.parameters['CELL']['cell_dofree'] = 'all'
+
+            pbc_cell_dofree_map = {
+                (True, True, True): 'all',
+                (True, False, False): 'x',
+                (False, True, False): 'y',
+                (False, False, True): 'z',
+                (True, True, False): '2Dxy',
+            }
+            if structure.pbc in pbc_cell_dofree_map:
+                base.pw.parameters['CELL']['cell_dofree'] = pbc_cell_dofree_map[structure.pbc]
+            else:
+                raise ValueError(f'Structures with periodic boundary conditions `{structure.pbc}` are not supported.')
 
         builder = cls.get_builder()
         builder.base = base
         builder.base_final_scf = base_final_scf
         builder.structure = structure
         builder.clean_workdir = orm.Bool(inputs['clean_workdir'])
         builder.max_meta_convergence_iterations = orm.Int(inputs['max_meta_convergence_iterations'])
@@ -164,46 +175,42 @@
         self.ctx.is_converged = False
         self.ctx.iteration = 0
 
         self.ctx.relax_inputs = AttributeDict(self.exposed_inputs(PwBaseWorkChain, namespace='base'))
         self.ctx.relax_inputs.pw.parameters = self.ctx.relax_inputs.pw.parameters.get_dict()
 
         self.ctx.relax_inputs.pw.parameters.setdefault('CONTROL', {})
-        self.ctx.relax_inputs.pw.parameters['CONTROL']['restart_mode'] = 'from_scratch'
 
         # Set the meta_convergence and add it to the context
         self.ctx.meta_convergence = self.inputs.meta_convergence.value
         volume_cannot_change = (
-            self.ctx.relax_inputs.pw.parameters['CONTROL']['calculation'] in ('scf', 'relax') or
+            self.ctx.relax_inputs.pw.parameters['CONTROL'].get('calculation', 'scf') in ('scf', 'relax') or
             self.ctx.relax_inputs.pw.parameters.get('CELL', {}).get('cell_dofree', None) == 'shape'
         )
         if self.ctx.meta_convergence and volume_cannot_change:
             self.report(
                 'No change in volume possible for the provided base input parameters. Meta convergence is turned off.'
             )
             self.ctx.meta_convergence = False
 
         # Add the final scf inputs to the context if a final scf should be run
         if 'base_final_scf' in self.inputs:
             self.ctx.final_scf_inputs = AttributeDict(self.exposed_inputs(PwBaseWorkChain, namespace='base_final_scf'))
 
-            if self.ctx.relax_inputs.pw.parameters['CONTROL']['calculation'] == 'scf':
+            if self.ctx.relax_inputs.pw.parameters['CONTROL'].get('calculation', 'scf') == 'scf':
                 self.report(
                     'Work chain will not run final SCF when `calculation` is set to `scf` for the relaxation '
                     '`PwBaseWorkChain`.'
                 )
                 self.ctx.pop('final_scf_inputs')
 
             else:
                 self.ctx.final_scf_inputs.pw.parameters = self.ctx.final_scf_inputs.pw.parameters.get_dict()
 
                 self.ctx.final_scf_inputs.pw.parameters.setdefault('CONTROL', {})
-                self.ctx.final_scf_inputs.pw.parameters['CONTROL']['calculation'] = 'scf'
-                self.ctx.final_scf_inputs.pw.parameters['CONTROL']['restart_mode'] = 'from_scratch'
-                self.ctx.final_scf_inputs.pw.parameters.pop('CELL', None)
                 self.ctx.final_scf_inputs.metadata.call_link_label = 'final_scf'
 
     def should_run_relax(self):
         """Return whether a relaxation workchain should be run.
 
         This is the case as long as the volume change between two consecutive relaxation runs is larger than the volume
         convergence threshold value and the maximum number of meta convergence iterations is not exceeded.
```

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/q2r/base.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/q2r/base.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/xspectra/base.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/xspectra/base.py`

 * *Files identical despite different names*

### Comparing `aiida-quantumespresso-4.2.0/src/aiida_quantumespresso/workflows/xspectra/core.py` & `aiida-quantumespresso-4.3.0/src/aiida_quantumespresso/workflows/xspectra/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -331,15 +331,15 @@
         :param kwargs: additional keyword arguments that will be passed to the
             ``get_builder_from_protocol`` of all the sub processes that are called by this
             workchain.
         :return: a process builder instance with all inputs defined ready for launch.
         """
 
         inputs = cls.get_protocol_inputs(protocol, overrides)
-        pw_inputs = PwBaseWorkChain.get_protocol_inputs(protocol=protocol)
+        pw_inputs = PwBaseWorkChain.get_protocol_inputs(protocol=protocol, overrides=inputs.get('scf', {}))
         pw_params = pw_inputs['pw']['parameters']
         kinds_present = sorted([kind.name for kind in structure.kinds])
         # Get the default inputs from the PwBaseWorkChain and override them with those
         # required for the chosen core-hole treatment
         pw_params = recursive_merge(
             left=pw_params,
             right=cls.get_treatment_inputs(
```

### Comparing `aiida-quantumespresso-4.2.0/PKG-INFO` & `aiida-quantumespresso-4.3.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,41 +1,42 @@
 Metadata-Version: 2.1
 Name: aiida-quantumespresso
-Version: 4.2.0
+Version: 4.3.0
 Summary: The official AiiDA plugin for Quantum ESPRESSO
 Keywords: aiida,workflows
 Author-email: The AiiDA team <developers@aiida.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Framework :: AiiDA
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: aiida_core[atomic_tools]~=2.1
+Requires-Dist: aiida_core[atomic_tools]~=2.3
 Requires-Dist: aiida-pseudo~=1.0
 Requires-Dist: click~=8.0
 Requires-Dist: importlib_resources
 Requires-Dist: jsonschema
 Requires-Dist: numpy
+Requires-Dist: pydantic
 Requires-Dist: packaging
 Requires-Dist: qe-tools~=2.0
 Requires-Dist: xmlschema~=1.2,>=1.2.5
 Requires-Dist: sphinx~=4.1 ; extra == "docs"
 Requires-Dist: sphinx-copybutton~=0.5.0 ; extra == "docs"
 Requires-Dist: sphinx-book-theme~=0.3.2 ; extra == "docs"
 Requires-Dist: sphinx-click~=4.0 ; extra == "docs"
 Requires-Dist: sphinx-design~=0.0.13 ; extra == "docs"
 Requires-Dist: sphinxcontrib-details-directive~=0.1.0 ; extra == "docs"
 Requires-Dist: sphinx-autoapi ; extra == "docs"
 Requires-Dist: pre-commit~=2.17 ; extra == "pre-commit"
-Requires-Dist: pylint~=2.12.2 ; extra == "pre-commit"
+Requires-Dist: pylint~=2.17.2 ; extra == "pre-commit"
 Requires-Dist: pylint-aiida~=0.1.1 ; extra == "pre-commit"
 Requires-Dist: toml ; extra == "pre-commit"
 Requires-Dist: pgtest~=1.3 ; extra == "tests"
 Requires-Dist: pytest~=6.0 ; extra == "tests"
 Requires-Dist: pytest-regressions~=2.3 ; extra == "tests"
 Project-URL: Documentation, https://aiida-quantumespresso.readthedocs.io
 Project-URL: Home, https://github.com/aiidateam/aiida-quantumespresso
@@ -43,15 +44,15 @@
 Provides-Extra: docs
 Provides-Extra: pre-commit
 Provides-Extra: tests
 
 # `aiida-quantumespresso`
 [![PyPI version](https://badge.fury.io/py/aiida-quantumespresso.svg)](https://badge.fury.io/py/aiida-quantumespresso)
 [![PyPI pyversions](https://img.shields.io/pypi/pyversions/aiida-quantumespresso.svg)](https://pypi.python.org/pypi/aiida-quantumespresso)
-[![Build Status](https://github.com/aiidateam/aiida-quantumespresso/workflows/aiida-quantumespresso/badge.svg?branch=develop&event=push)](https://github.com/aiidateam/aiida-quantumespresso/actions)
+[![Build Status](https://github.com/aiidateam/aiida-quantumespresso/actions/workflows/ci.yml/badge.svg?branch=main)](https://github.com/aiidateam/aiida-quantumespresso/actions)
 [![Docs status](https://readthedocs.org/projects/aiida-quantumespresso/badge)](http://aiida-quantumespresso.readthedocs.io/)
 
 This is the official AiiDA plugin for [Quantum ESPRESSO](https://www.quantum-espresso.org/).
 
 ## Compatibility matrix
 
 The matrix below assumes the user always install the latest patch release of the specified minor version, which is recommended.
@@ -128,20 +129,46 @@
 
     aiida-pseudo install sssp
 
 to install the default SSSP version.
 List the installed pseudopotential families with the command `aiida-pseudo list`.
 You can then use the name of any family in the command line using the `-F` flag.
 
+## Development
+
+### Running tests
+To run the tests, simply clone and install the package locally with the [tests] optional dependencies:
+
+```shell
+git clone https://github.com/aiidateam/aiida-quantumespresso .
+cd aiida-quantumespresso
+pip install -e .[tests]  # install extra dependencies for test
+pytest # run tests
+```
+
+You can also use `tox` to run the test set. Here you can also use the `-e` option to specify the Python version for the test run:
+```shell
+pip install tox
+tox -e py39 -- tests/calculations/test_pw.py
+```
+
+### Pre-commit
+To contribute to this repository, please enable pre-commit so the code in commits are conform to the standards.
+Simply install the repository with the `pre-commit` extra dependencies:
+```shell
+cd aiida-quantumespresso
+pip install -e .[pre-commit]
+pre-commit install
+```
 
 ## License
 The `aiida-quantumespresso` plugin package is released under the MIT license.
 See the `LICENSE.txt` file for more details.
 
-## Acknowlegements
+## Acknowledgements
 We acknowledge support from:
 * the [NCCR MARVEL](http://nccr-marvel.ch/) funded by the Swiss National Science Foundation;
 * the EU Centre of Excellence "[MaX – Materials Design at the Exascale](http://www.max-centre.eu/)" (Horizon 2020 EINFRA-5, Grant No. 676598; H2020-INFRAEDI-2018-1, Grant No. 824143; HORIZON-EUROHPC-JU-2021-COE-1, Grant No. 101093324);
 * the European Union's Horizon 2020 research and innovation programme (Grant No. 957189, [project BIG-MAP](https://www.big-map.eu), also part of the [BATTERY 2030+ initiative](https://battery2030.eu), Grant No. 957213);
 * the [swissuniversities P-5 project "Materials Cloud"](https://www.materialscloud.org/swissuniversities).
 
 <img src="https://raw.githubusercontent.com/aiidateam/aiida-quantumespresso/develop/docs/source/images/MARVEL.png" width="250px" height="131px"/>
```

