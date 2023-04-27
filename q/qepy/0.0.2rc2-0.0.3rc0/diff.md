# Comparing `tmp/qepy-0.0.2rc2.tar.gz` & `tmp/qepy-0.0.3rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "qepy-0.0.2rc2.tar", last modified: Tue Mar 28 19:15:21 2023, max compression
+gzip compressed data, was "qepy-0.0.3rc0.tar", last modified: Thu Apr 27 00:05:36 2023, max compression
```

## Comparing `qepy-0.0.2rc2.tar` & `qepy-0.0.3rc0.tar`

### file list

```diff
@@ -1,242 +1,249 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.648038 qepy-0.0.2rc2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.600037 qepy-0.0.2rc2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.604037 qepy-0.0.2rc2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1699 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/.github/workflows/wheels.yml
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1644 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/.gitlab-ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)       97 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/.gitmodules
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-03-28 19:15:21.648038 qepy-0.0.2rc2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1847 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.604037 qepy-0.0.2rc2/doc/
--rw-r--r--   0 runner    (1001) docker     (123)      995 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/doc/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/doc/make.bat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.604037 qepy-0.0.2rc2/doc/source/
--rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/doc/source/QEpy.bib
--rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/doc/source/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/doc/source/contact.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.604037 qepy-0.0.2rc2/doc/source/development/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/doc/source/development/development.rst
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/doc/source/development/documentation.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/doc/source/faq.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/doc/source/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/doc/source/install.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.608037 qepy-0.0.2rc2/doc/source/qepy/
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/doc/source/qepy/calculator.rst
--rw-r--r--   0 runner    (1001) docker     (123)      439 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/doc/source/qepy/driver.rst
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/doc/source/qepy/io.rst
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/doc/source/qepy/qepy.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.608037 qepy-0.0.2rc2/doc/source/static/
--rw-r--r--   0 runner    (1001) docker     (123)      436 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/doc/source/static/custom.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.608037 qepy-0.0.2rc2/doc/source/templates/
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/doc/source/templates/breadcrumbs.html
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/doc/source/templates/footer.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.608037 qepy-0.0.2rc2/doc/source/tutorials/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.608037 qepy-0.0.2rc2/doc/source/tutorials/jupyter/
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/doc/source/tutorials/jupyter/dirac_exchange.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    87060 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/doc/source/tutorials/jupyter/dos_band_graphene.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/doc/source/tutorials/jupyter/qepy_scf.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/doc/source/tutorials/jupyter/qepy_scf_iterative.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    17252 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/doc/source/tutorials/jupyter/test_ecutwfc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    23113 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/doc/source/tutorials/jupyter/test_eos_vc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/doc/source/tutorials/jupyter/test_kpoints.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/doc/source/tutorials/tutorials.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.608037 qepy-0.0.2rc2/examples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.608037 qepy-0.0.2rc2/examples/ase/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/ase/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/ase/qe_in.in
--rwxr-xr-x   0 runner    (1001) docker     (123)     1187 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/ase/test_ase_nvt.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3360 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/ase/test_ase_scf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      171 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/clean.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.600037 qepy-0.0.2rc2/examples/develop/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.612037 qepy-0.0.2rc2/examples/develop/pw/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/develop/pw/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/develop/pw/qe_in.in
--rwxr-xr-x   0 runner    (1001) docker     (123)      508 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/develop/pw/scf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1024 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/develop/pw/test_pwscf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      946 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/develop/pw/test_pwscf_scf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      786 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/develop/pw/tmp2energy.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1016 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/develop/pw/tmp2energy_pw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.600037 qepy-0.0.2rc2/examples/jupyter/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.612037 qepy-0.0.2rc2/examples/jupyter/DATA/
--rw-r--r--   0 runner    (1001) docker     (123)   964489 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/DATA/Al.pbe-nl-kjpaw_psl.1.0.0.UPF
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/DATA/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)   264541 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/DATA/C.pbe-rrkjus.UPF
--rw-r--r--   0 runner    (1001) docker     (123)    64999 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/DATA/H_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)    90153 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/DATA/O_ONCV_PBE-1.2.upf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.612037 qepy-0.0.2rc2/examples/jupyter/band/
--rw-r--r--   0 runner    (1001) docker     (123)   264541 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/band/C.pbe-rrkjus.UPF
--rw-r--r--   0 runner    (1001) docker     (123)    87060 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/band/dos_band_graphene.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.612037 qepy-0.0.2rc2/examples/jupyter/colab/
--rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/colab/qepy_colab.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.616037 qepy-0.0.2rc2/examples/jupyter/eos/
--rw-r--r--   0 runner    (1001) docker     (123)   964489 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/eos/Al.pbe-nl-kjpaw_psl.1.0.0.UPF
--rw-r--r--   0 runner    (1001) docker     (123)    23324 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/eos/test_eos_slow.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    23113 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/eos/test_eos_vc.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.616037 qepy-0.0.2rc2/examples/jupyter/ext/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/ext/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/ext/dftpy_xc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/ext/dirac_exchange.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.616037 qepy-0.0.2rc2/examples/jupyter/nvt/
--rw-r--r--   0 runner    (1001) docker     (123)    64999 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/nvt/H_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)    90153 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/nvt/O_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/nvt/ase_nvt.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      855 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/nvt/qe_in.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.620037 qepy-0.0.2rc2/examples/jupyter/scf/
--rw-r--r--   0 runner    (1001) docker     (123)   964489 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/scf/Al.pbe-nl-kjpaw_psl.1.0.0.UPF
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/scf/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/scf/dftpy_mixer.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)      926 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/scf/qe_in.in
--rw-r--r--   0 runner    (1001) docker     (123)    20039 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/scf/qepy_iterative.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     8394 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/scf/qepy_qeinput.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/scf/qepy_scf.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/scf/qepy_scf_iterative.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.620037 qepy-0.0.2rc2/examples/jupyter/testing/
--rw-r--r--   0 runner    (1001) docker     (123)   964489 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/testing/Al.pbe-nl-kjpaw_psl.1.0.0.UPF
--rw-r--r--   0 runner    (1001) docker     (123)    32639 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/testing/test_degauss.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    17252 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/testing/test_ecutwfc.ipynb
--rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/jupyter/testing/test_kpoints.ipynb
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.600037 qepy-0.0.2rc2/examples/opt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.624037 qepy-0.0.2rc2/examples/opt/ase/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.624037 qepy-0.0.2rc2/examples/opt/ase/out/
--rw-r--r--   0 runner    (1001) docker     (123)    74363 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/opt/ase/out/ase.out
--rw-r--r--   0 runner    (1001) docker     (123)    88204 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/opt/ase/out/qepy.out
--rw-r--r--   0 runner    (1001) docker     (123)   577736 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/opt/ase/si_pbe_v1.uspp.F.UPF
--rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/opt/ase/test_ase_opt.py
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/opt/ase/vcrelax.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.624037 qepy-0.0.2rc2/examples/opt/qe/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.624037 qepy-0.0.2rc2/examples/opt/qe/out/
--rw-r--r--   0 runner    (1001) docker     (123)    88204 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/opt/qe/out/qepy.out
--rw-r--r--   0 runner    (1001) docker     (123)    90822 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/opt/qe/out/ref.out
--rwxr-xr-x   0 runner    (1001) docker     (123)     2171 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/opt/qe/qe_relax.py
--rw-r--r--   0 runner    (1001) docker     (123)   577736 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/opt/qe/si_pbe_v1.uspp.F.UPF
--rw-r--r--   0 runner    (1001) docker     (123)      934 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/opt/qe/vcrelax.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.600037 qepy-0.0.2rc2/examples/original/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.624037 qepy-0.0.2rc2/examples/original/6.5/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/original/6.5/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/original/6.5/qe_in.in
--rwxr-xr-x   0 runner    (1001) docker     (123)      835 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/original/6.5/run_pwscf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.624037 qepy-0.0.2rc2/examples/original/6.8/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/original/6.8/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)      965 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/original/6.8/qe_in.in
--rwxr-xr-x   0 runner    (1001) docker     (123)      426 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/original/6.8/run_pwscf.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.628037 qepy-0.0.2rc2/examples/scf/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/scf/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/scf/qe_in.in
--rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/scf/test_pwscf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      708 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/scf/test_pwscf_iterative.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/scf/test_readfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      398 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/scf/test_readfile_pw.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.628037 qepy-0.0.2rc2/examples/tddft/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/tddft/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/tddft/qe_in.in
--rwxr-xr-x   0 runner    (1001) docker     (123)      743 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/tddft/test_ce_tddft.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/tddft/test_ce_tddft_restart.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.628037 qepy-0.0.2rc2/examples/test/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.628037 qepy-0.0.2rc2/examples/test/DATA/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/DATA/Al_ONCV_PBE-1.2.upf
--rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/DATA/al_md_3.traj
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.628037 qepy-0.0.2rc2/examples/test/DATA/oldxml/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.632037 qepy-0.0.2rc2/examples/test/DATA/oldxml/al_oldxml.save/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/DATA/oldxml/al_oldxml.save/Al_ONCV_PBE-1.2.upf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.632037 qepy-0.0.2rc2/examples/test/DATA/oldxml/al_oldxml.save/K00001/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/DATA/oldxml/al_oldxml.save/K00001/eigenval.xml
--rw-r--r--   0 runner    (1001) docker     (123)   266316 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/DATA/oldxml/al_oldxml.save/charge-density.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10312 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/DATA/oldxml/al_oldxml.save/data-file.xml
--rw-r--r--   0 runner    (1001) docker     (123)   804960 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/DATA/oldxml/al_oldxml.wfc1
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.604037 qepy-0.0.2rc2/examples/test/DATA/oldxml_collect/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.632037 qepy-0.0.2rc2/examples/test/DATA/oldxml_collect/al_oldxml.save/
--rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/DATA/oldxml_collect/al_oldxml.save/Al_ONCV_PBE-1.2.upf
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.636037 qepy-0.0.2rc2/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/eigenval.xml
--rw-r--r--   0 runner    (1001) docker     (123)   808502 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/evc.dat
--rw-r--r--   0 runner    (1001) docker     (123)    32091 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/gkvectors.dat
--rw-r--r--   0 runner    (1001) docker     (123)   266316 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/DATA/oldxml_collect/al_oldxml.save/charge-density.dat
--rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/DATA/oldxml_collect/al_oldxml.save/data-file.xml
--rw-r--r--   0 runner    (1001) docker     (123)   185540 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/DATA/oldxml_collect/al_oldxml.save/gvectors.dat
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/DATA/qe_fake.in
--rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/DATA/qe_in.in
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.636037 qepy-0.0.2rc2/examples/test/qe-6.5/
--rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/qe-6.5/test.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)     1855 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/qe-6.5/test_ce_tddft.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1613 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/qe-6.5/test_comm.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1335 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/qe-6.5/test_oldxml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1352 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/qe-6.5/test_pwscf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1336 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/qe-6.5/test_pwscf_scf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2008 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/qe-6.5/test_readfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/test.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/test_ase_md.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1711 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/test_ce_tddft.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      964 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/test_oldxml.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      859 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/test_pwscf.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      972 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/test_pwscf_iterative.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1022 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/examples/test/test_readfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.636037 qepy-0.0.2rc2/install/
--rw-r--r--   0 runner    (1001) docker     (123)     4013 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/install/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/install/Makefile.cetddft
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/install/kind_map.json
--rw-r--r--   0 runner    (1001) docker     (123)     1613 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/install/make.depend
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/install/make.depend.cetddft
--rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/install/make.qe.inc
--rwxr-xr-x   0 runner    (1001) docker     (123)      274 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/install/makedeps.sh
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.640037 qepy-0.0.2rc2/qepy/
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/qepy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/qepy/__new__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16271 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/qepy/calculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/qepy/core.py
--rw-r--r--   0 runner    (1001) docker     (123)    28129 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/qepy/driver.py
--rw-r--r--   0 runner    (1001) docker     (123)    11026 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/qepy/io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.640037 qepy-0.0.2rc2/qepy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2632 2023-03-28 19:15:21.000000 qepy-0.0.2rc2/qepy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6219 2023-03-28 19:15:21.000000 qepy-0.0.2rc2/qepy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 19:15:21.000000 qepy-0.0.2rc2/qepy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-28 19:15:21.000000 qepy-0.0.2rc2/qepy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      136 2023-03-28 19:15:21.000000 qepy-0.0.2rc2/qepy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-03-28 19:15:21.000000 qepy-0.0.2rc2/qepy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-28 19:15:21.648038 qepy-0.0.2rc2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     6828 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.604037 qepy-0.0.2rc2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.640037 qepy-0.0.2rc2/src/api/
--rw-r--r--   0 runner    (1001) docker     (123)     9213 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/api/qepy_common.f90
--rw-r--r--   0 runner    (1001) docker     (123)    18038 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/api/qepy_mod.f90
--rw-r--r--   0 runner    (1001) docker     (123)    50459 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/api/qepy_scatter_mod.f90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.640037 qepy-0.0.2rc2/src/ldau/
--rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/ldau/qepy_econf.ini
--rwxr-xr-x   0 runner    (1001) docker     (123)     6276 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/ldau/qepy_ldau_patch.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.644037 qepy-0.0.2rc2/src/oldxml/
--rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/oldxml/oldxml_io_rho_xml.f90
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/oldxml/oldxml_potinit.f90
--rw-r--r--   0 runner    (1001) docker     (123)   105084 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/oldxml/oldxml_pw_restart.f90
--rw-r--r--   0 runner    (1001) docker     (123)   176393 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/oldxml/oldxml_qexml.f90
--rw-r--r--   0 runner    (1001) docker     (123)    17352 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/oldxml/oldxml_read_file.f90
--rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/oldxml/oldxml_wfcinit.f90
--rw-r--r--   0 runner    (1001) docker     (123)    40621 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/oldxml/oldxml_xml_io_base.f90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.644037 qepy-0.0.2rc2/src/qe/
--rw-r--r--   0 runner    (1001) docker     (123)    65894 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/qe/funct.f90
--rw-r--r--   0 runner    (1001) docker     (123)     3844 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/qe/qepy_api.f90
--rw-r--r--   0 runner    (1001) docker     (123)    61641 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/qe/qepy_electrons.f90
--rw-r--r--   0 runner    (1001) docker     (123)    11079 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/qe/qepy_electrons_nscf.f90
--rw-r--r--   0 runner    (1001) docker     (123)    14985 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/qe/qepy_forces.f90
--rw-r--r--   0 runner    (1001) docker     (123)     2791 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/qe/qepy_hinit1.f90
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/qe/qepy_init_run.f90
--rw-r--r--   0 runner    (1001) docker     (123)     9711 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/qe/qepy_potinit.f90
--rw-r--r--   0 runner    (1001) docker     (123)    62688 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/qe/qepy_pw2casino_write.f90
--rw-r--r--   0 runner    (1001) docker     (123)    56822 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/qe/qepy_pw_restart_new.f90
--rw-r--r--   0 runner    (1001) docker     (123)     6116 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/qe/qepy_pwscf.f90
--rw-r--r--   0 runner    (1001) docker     (123)    11965 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/qe/qepy_read_file_new.f90
--rw-r--r--   0 runner    (1001) docker     (123)    16732 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/qe/qepy_run_pwscf.f90
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/qe/qepy_setlocal.f90
--rw-r--r--   0 runner    (1001) docker     (123)     7421 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/qe/qepy_stop_run.f90
--rw-r--r--   0 runner    (1001) docker     (123)    10470 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/qe/qepy_stress.f90
--rw-r--r--   0 runner    (1001) docker     (123)    44288 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/qe/qepy_sum_band.f90
--rw-r--r--   0 runner    (1001) docker     (123)    39006 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/qe/qepy_v_of_rho.f90
--rw-r--r--   0 runner    (1001) docker     (123)    12047 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/qe/qepy_wfcinit.f90
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-28 19:15:21.648038 qepy-0.0.2rc2/src/tddft/
--rw-r--r--   0 runner    (1001) docker     (123)    16063 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/tddft/qepy_molecule_optical_absorption.f90
--rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/tddft/qepy_tddft_common.f90
--rw-r--r--   0 runner    (1001) docker     (123)     6601 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/tddft/qepy_tddft_main.f90
--rw-r--r--   0 runner    (1001) docker     (123)      800 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/tddft/qepy_tddft_mod.f90
--rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/tddft/qepy_tddft_routines.f90
--rw-r--r--   0 runner    (1001) docker     (123)     4707 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/tddft/qepy_tddft_setup.f90
--rw-r--r--   0 runner    (1001) docker     (123)     6844 2023-03-28 19:14:49.000000 qepy-0.0.2rc2/src/tddft/qepy_update_ham.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.770805 qepy-0.0.3rc0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.674802 qepy-0.0.3rc0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.690802 qepy-0.0.3rc0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1364 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/.github/workflows/linux.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/.github/workflows/wheels.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1824 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/.gitlab-ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       97 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/.gitmodules
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-27 00:05:36.766805 qepy-0.0.3rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.690802 qepy-0.0.3rc0/doc/
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/make.bat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.690802 qepy-0.0.3rc0/doc/source/
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/QEpy.bib
+-rw-r--r--   0 runner    (1001) docker     (123)     1469 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/contact.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.694802 qepy-0.0.3rc0/doc/source/development/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/development/development.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/development/documentation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4345 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/faq.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1352 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3574 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/install.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.694802 qepy-0.0.3rc0/doc/source/qepy/
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/qepy/calculator.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/qepy/driver.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/qepy/io.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/qepy/qepy.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.694802 qepy-0.0.3rc0/doc/source/static/
+-rw-r--r--   0 runner    (1001) docker     (123)      436 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/static/custom.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.694802 qepy-0.0.3rc0/doc/source/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/templates/breadcrumbs.html
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/templates/footer.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.694802 qepy-0.0.3rc0/doc/source/tutorials/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.698803 qepy-0.0.3rc0/doc/source/tutorials/jupyter/
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/tutorials/jupyter/dirac_exchange.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    87060 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/tutorials/jupyter/dos_band_graphene.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/tutorials/jupyter/qepy_scf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/tutorials/jupyter/qepy_scf_iterative.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    17252 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/tutorials/jupyter/test_ecutwfc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    23113 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/tutorials/jupyter/test_eos_vc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/tutorials/jupyter/test_kpoints.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/doc/source/tutorials/tutorials.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.698803 qepy-0.0.3rc0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.698803 qepy-0.0.3rc0/examples/ase/
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/ase/Al_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/ase/qe_in.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1187 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/ase/test_ase_nvt.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3360 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/ase/test_ase_scf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      140 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/clean.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.678802 qepy-0.0.3rc0/examples/develop/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.702803 qepy-0.0.3rc0/examples/develop/pw/
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/develop/pw/Al_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)     1037 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/develop/pw/qe_in.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)      508 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/develop/pw/scf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1024 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/develop/pw/test_pwscf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      946 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/develop/pw/test_pwscf_scf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      786 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/develop/pw/tmp2energy.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1016 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/develop/pw/tmp2energy_pw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.678802 qepy-0.0.3rc0/examples/jupyter/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.706803 qepy-0.0.3rc0/examples/jupyter/DATA/
+-rw-r--r--   0 runner    (1001) docker     (123)   964489 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/DATA/Al.pbe-nl-kjpaw_psl.1.0.0.UPF
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/DATA/Al_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)   264541 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/DATA/C.pbe-rrkjus.UPF
+-rw-r--r--   0 runner    (1001) docker     (123)    64999 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/DATA/H_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)    90153 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/DATA/O_ONCV_PBE-1.2.upf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.706803 qepy-0.0.3rc0/examples/jupyter/band/
+-rw-r--r--   0 runner    (1001) docker     (123)   264541 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/band/C.pbe-rrkjus.UPF
+-rw-r--r--   0 runner    (1001) docker     (123)    87060 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/band/dos_band_graphene.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.706803 qepy-0.0.3rc0/examples/jupyter/colab/
+-rw-r--r--   0 runner    (1001) docker     (123)     8457 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/colab/qepy_colab.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.710803 qepy-0.0.3rc0/examples/jupyter/eos/
+-rw-r--r--   0 runner    (1001) docker     (123)   964489 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/eos/Al.pbe-nl-kjpaw_psl.1.0.0.UPF
+-rw-r--r--   0 runner    (1001) docker     (123)    23324 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/eos/test_eos_slow.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    23113 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/eos/test_eos_vc.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.710803 qepy-0.0.3rc0/examples/jupyter/ext/
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/ext/Al_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)     6303 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/ext/dftpy_xc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     4286 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/ext/dirac_exchange.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.714803 qepy-0.0.3rc0/examples/jupyter/nvt/
+-rw-r--r--   0 runner    (1001) docker     (123)    64999 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/nvt/H_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)    90153 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/nvt/O_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)     5511 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/nvt/ase_nvt.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      855 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/nvt/qe_in.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.714803 qepy-0.0.3rc0/examples/jupyter/pp/
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/pp/Al_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/pp/pp.in
+-rw-r--r--   0 runner    (1001) docker     (123)    33477 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/pp/qepy_elf_rdg.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8342 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/pp/qepy_parse_output.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    28575 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/pp/qepy_potentials.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.718803 qepy-0.0.3rc0/examples/jupyter/scf/
+-rw-r--r--   0 runner    (1001) docker     (123)   964489 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/scf/Al.pbe-nl-kjpaw_psl.1.0.0.UPF
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/scf/Al_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)     6044 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/scf/dftpy_mixer.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)      926 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/scf/qe_in.in
+-rw-r--r--   0 runner    (1001) docker     (123)    20039 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/scf/qepy_iterative.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     8394 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/scf/qepy_qeinput.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     6874 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/scf/qepy_scf.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     7510 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/scf/qepy_scf_iterative.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.722803 qepy-0.0.3rc0/examples/jupyter/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)   964489 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/testing/Al.pbe-nl-kjpaw_psl.1.0.0.UPF
+-rw-r--r--   0 runner    (1001) docker     (123)    32639 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/testing/test_degauss.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    17252 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/testing/test_ecutwfc.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)    16249 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/jupyter/testing/test_kpoints.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.678802 qepy-0.0.3rc0/examples/opt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.722803 qepy-0.0.3rc0/examples/opt/ase/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.726804 qepy-0.0.3rc0/examples/opt/ase/out/
+-rw-r--r--   0 runner    (1001) docker     (123)    74363 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/opt/ase/out/ase.out
+-rw-r--r--   0 runner    (1001) docker     (123)    88204 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/opt/ase/out/qepy.out
+-rw-r--r--   0 runner    (1001) docker     (123)   577736 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/opt/ase/si_pbe_v1.uspp.F.UPF
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1125 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/opt/ase/test_ase_opt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/opt/ase/vcrelax.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.726804 qepy-0.0.3rc0/examples/opt/qe/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.726804 qepy-0.0.3rc0/examples/opt/qe/out/
+-rw-r--r--   0 runner    (1001) docker     (123)    88204 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/opt/qe/out/qepy.out
+-rw-r--r--   0 runner    (1001) docker     (123)    90822 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/opt/qe/out/ref.out
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2171 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/opt/qe/qe_relax.py
+-rw-r--r--   0 runner    (1001) docker     (123)   577736 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/opt/qe/si_pbe_v1.uspp.F.UPF
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/opt/qe/vcrelax.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.682802 qepy-0.0.3rc0/examples/original/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.730804 qepy-0.0.3rc0/examples/original/6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/original/6.5/Al_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/original/6.5/qe_in.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)      835 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/original/6.5/run_pwscf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.730804 qepy-0.0.3rc0/examples/original/6.8/
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/original/6.8/Al_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)      965 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/original/6.8/qe_in.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)      426 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/original/6.8/run_pwscf.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.734804 qepy-0.0.3rc0/examples/scf/
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/scf/Al_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/scf/qe_in.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)      600 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/scf/test_pwscf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      708 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/scf/test_pwscf_iterative.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      369 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/scf/test_readfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      398 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/scf/test_readfile_pw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.734804 qepy-0.0.3rc0/examples/tddft/
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/tddft/Al_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/tddft/qe_in.in
+-rwxr-xr-x   0 runner    (1001) docker     (123)      743 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/tddft/test_ce_tddft.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      824 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/tddft/test_ce_tddft_restart.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.734804 qepy-0.0.3rc0/examples/test/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.738804 qepy-0.0.3rc0/examples/test/DATA/
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/Al_ONCV_PBE-1.2.upf
+-rw-r--r--   0 runner    (1001) docker     (123)     2754 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/al_md_3.traj
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.738804 qepy-0.0.3rc0/examples/test/DATA/oldxml/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.742804 qepy-0.0.3rc0/examples/test/DATA/oldxml/al_oldxml.save/
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/oldxml/al_oldxml.save/Al_ONCV_PBE-1.2.upf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.742804 qepy-0.0.3rc0/examples/test/DATA/oldxml/al_oldxml.save/K00001/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/oldxml/al_oldxml.save/K00001/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   266316 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/oldxml/al_oldxml.save/charge-density.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10312 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/oldxml/al_oldxml.save/data-file.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   804960 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/oldxml/al_oldxml.wfc1
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.682802 qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.742804 qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/
+-rw-r--r--   0 runner    (1001) docker     (123)    90193 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/Al_ONCV_PBE-1.2.upf
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.746804 qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/eigenval.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   808502 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/evc.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    32091 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/gkvectors.dat
+-rw-r--r--   0 runner    (1001) docker     (123)   266316 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/charge-density.dat
+-rw-r--r--   0 runner    (1001) docker     (123)    10735 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/data-file.xml
+-rw-r--r--   0 runner    (1001) docker     (123)   185540 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/gvectors.dat
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/qe_fake.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1127 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/DATA/qe_in.in
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.750805 qepy-0.0.3rc0/examples/test/qe-6.5/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      649 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/qe-6.5/test.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1799 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/qe-6.5/test_ce_tddft.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1613 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/qe-6.5/test_comm.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1461 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/qe-6.5/test_oldxml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1360 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/qe-6.5/test_pwscf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1364 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/qe-6.5/test_pwscf_scf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2110 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/qe-6.5/test_readfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      715 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/test.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      817 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/test_ase_md.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1711 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/test_ce_tddft.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      983 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/test_oldxml.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      871 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/test_pwscf.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      972 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/test_pwscf_iterative.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1022 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/examples/test/test_readfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.750805 qepy-0.0.3rc0/install/
+-rw-r--r--   0 runner    (1001) docker     (123)     4106 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/install/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1744 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/install/Makefile.cetddft
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/install/kind_map.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1820 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/install/make.depend
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/install/make.depend.cetddft
+-rw-r--r--   0 runner    (1001) docker     (123)     1324 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/install/make.qe.inc
+-rwxr-xr-x   0 runner    (1001) docker     (123)      274 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/install/makedeps.sh
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.754804 qepy-0.0.3rc0/qepy/
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/qepy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/qepy/__new__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16277 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/qepy/calculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/qepy/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34766 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/qepy/driver.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13504 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/qepy/io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.754804 qepy-0.0.3rc0/qepy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-04-27 00:05:36.000000 qepy-0.0.3rc0/qepy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6401 2023-04-27 00:05:36.000000 qepy-0.0.3rc0/qepy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 00:05:36.000000 qepy-0.0.3rc0/qepy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-27 00:05:36.000000 qepy-0.0.3rc0/qepy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      136 2023-04-27 00:05:36.000000 qepy-0.0.3rc0/qepy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-27 00:05:36.000000 qepy-0.0.3rc0/qepy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-27 00:05:36.770805 qepy-0.0.3rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     6827 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.686802 qepy-0.0.3rc0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.754804 qepy-0.0.3rc0/src/api/
+-rw-r--r--   0 runner    (1001) docker     (123)    10913 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/api/qepy_common.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    26027 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/api/qepy_mod.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.758805 qepy-0.0.3rc0/src/fix/
+-rw-r--r--   0 runner    (1001) docker     (123)    66035 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/fix/funct.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     9565 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/fix/potinit.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    56596 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/fix/pw_restart_new.f90
+-rw-r--r--   0 runner    (1001) docker     (123)   360829 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/fix/qes_read_module.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    12135 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/fix/read_file_new.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    50735 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/fix/scatter_mod.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    11723 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/fix/wfcinit.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.758805 qepy-0.0.3rc0/src/ldau/
+-rw-r--r--   0 runner    (1001) docker     (123)     3408 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/ldau/qepy_econf.ini
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6276 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/ldau/qepy_ldau_patch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.762805 qepy-0.0.3rc0/src/oldxml/
+-rw-r--r--   0 runner    (1001) docker     (123)     8045 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/oldxml/oldxml_io_rho_xml.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/oldxml/oldxml_potinit.f90
+-rw-r--r--   0 runner    (1001) docker     (123)   105084 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/oldxml/oldxml_pw_restart.f90
+-rw-r--r--   0 runner    (1001) docker     (123)   176393 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/oldxml/oldxml_qexml.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    17352 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/oldxml/oldxml_read_file.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    12941 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/oldxml/oldxml_wfcinit.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    40621 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/oldxml/oldxml_xml_io_base.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.766805 qepy-0.0.3rc0/src/qe/
+-rw-r--r--   0 runner    (1001) docker     (123)    61363 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/qe/qepy_electrons.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    11001 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/qe/qepy_electrons_nscf.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    14880 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/qe/qepy_forces.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     2711 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/qe/qepy_hinit1.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/qe/qepy_init_run.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    61917 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/qe/qepy_pw2casino_write.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/qe/qepy_pwscf.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    16516 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/qe/qepy_run_pwscf.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     3869 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/qe/qepy_setlocal.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     5983 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/qe/qepy_stop_run.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    10365 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/qe/qepy_stress.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    38870 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/qe/qepy_v_of_rho.f90
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-27 00:05:36.766805 qepy-0.0.3rc0/src/tddft/
+-rw-r--r--   0 runner    (1001) docker     (123)    16000 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/tddft/qepy_molecule_optical_absorption.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     1288 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/tddft/qepy_tddft_common.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     6736 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/tddft/qepy_tddft_main.f90
+-rw-r--r--   0 runner    (1001) docker     (123)      800 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/tddft/qepy_tddft_mod.f90
+-rw-r--r--   0 runner    (1001) docker     (123)    12519 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/tddft/qepy_tddft_routines.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/tddft/qepy_tddft_setup.f90
+-rw-r--r--   0 runner    (1001) docker     (123)     6664 2023-04-27 00:05:02.000000 qepy-0.0.3rc0/src/tddft/qepy_update_ham.f90
```

### Comparing `qepy-0.0.2rc2/.github/workflows/publish.yml` & `qepy-0.0.3rc0/.github/workflows/publish.yml`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Build wheels
+name: Publish to PyPI
 
 on:
   push:
     tags:
       - 'v*'
 jobs:
   publish:
@@ -42,19 +42,19 @@
 
       - name: Build a a source tarball
         if: steps.check-tag.outputs.match == 'true'
         run: |
           python -m pip install build
           python -m build --sdist
 
-      - name: Publish distribution to PyPI
+      - name: Publish distribution to Test PyPI
         if: steps.check-tag.outputs.match == 'true'
         uses: pypa/gh-action-pypi-publish@v1.7.1
         with:
-          password: ${{ secrets.PYPI_API_TOKEN }}
+          password: ${{ secrets.TEST_PYPI_API_TOKEN }}
+          repository_url: https://test.pypi.org/legacy/
 
-      - name: Publish distribution to Test PyPI
+      - name: Publish distribution to PyPI
         if: steps.check-tag.outputs.match == 'true'
         uses: pypa/gh-action-pypi-publish@v1.7.1
         with:
-          password: ${{ secrets.TEST_PYPI_API_TOKEN }}
-          repository_url: https://test.pypi.org/legacy/
+          password: ${{ secrets.PYPI_API_TOKEN }}
```

### Comparing `qepy-0.0.2rc2/.github/workflows/wheels.yml` & `qepy-0.0.3rc0/.github/workflows/wheels.yml`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/.gitlab-ci.yml` & `qepy-0.0.3rc0/.gitlab-ci.yml`

 * *Files 21% similar despite different names*

```diff
@@ -11,14 +11,17 @@
   QTAGNEW: 'qepy-6.5g-dev'
   QEDIR: '/usr/src/app/q-e/'
   PUBLIC: 'package'
 
 
 build:
   stage: build
+  except:
+    - github
+    - action
   image: $CONTAINER_IMAGE:$QTAG
   script:
    - git clone https://github.com/dceresoli/ce-tddft.git src/ce-tddft
    - qedir=$QEDIR oldxml=yes tddft=yes python -m pip install .
    - mkdir $PUBLIC
    - cd $PUBLIC
    - PACKAGE=$(python -c 'import qepy, os; print(os.path.split(qepy.__path__[0])[0])')
@@ -30,34 +33,41 @@
     name: "QEpy-$CI_COMMIT_REF_SLUG-${CI_COMMIT_SHA::9}"
     paths:
       - $PUBLIC
 
 
 test:
   stage: test
+  except:
+    - github
+    - action
   image: $CONTAINER_IMAGE:$QTAG
   script:
    - cp -r $PUBLIC/* $PACKAGE
    - cd examples/test
    - bash test.sh
+   - export MPIRUN="mpirun --allow-run-as-root --oversubscribe"
+   - bash test.sh p
 
 qe65:
   stage: qe65
+  except:
+    - github
+    - action
   image: $CONTAINER_IMAGE:$QTAG
   script:
    - cp -r $PUBLIC/* $PACKAGE
    - cd examples/test/qe-6.5
    - bash test.sh
 
 
 docker_image:
   stage: deploy
   only:
-    refs:
-      - docker
+    - docker
   image: docker:stable
   services:
     - docker:dind
 
   variables:
     DOCKER_HOST: tcp://docker:2375
```

### Comparing `qepy-0.0.2rc2/PKG-INFO` & `qepy-0.0.3rc0/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qepy
-Version: 0.0.2rc2
+Version: 0.0.3rc0
 Summary: QEpy: Quantum ESPRESSO Python interface
 Home-page: https://gitlab.com/shaoxc/qepy
 Author: Pavanello Research Group
 Author-email: m.pavanello@rutgers.edu
 License: GPL
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -38,37 +38,38 @@
 ## Requirements
  - [Python](https://www.python.org/) (>=3.7)
  - [NumPy](https://docs.scipy.org/doc/numpy/reference/) (>=1.18.0)
  - [f90wrap](https://github.com/jameskermode/f90wrap) (>=0.2.8)
  - [Quantum ESPRESSO ](https://gitlab.com/QEF/q-e/-/releases/qe-6.5) (=6.5)
  - Compiler ([GNU](https://gcc.gnu.org/fortran/)(Recommended) or [Intel](https://software.intel.com/content/www/us/en/develop/tools/oneapi/components/fortran-compiler.html))
 
-## Install
+## Installation
+### Pip
+   Using pip can easy install the release version (serial) of QEpy from [PyPI](https://pypi.org/project/qepy).
+
+```shell
+python -m pip install qepy
+```
+
+### Source
+
  - **QE**
 
-	All static libraries should be compiled with the `-fPIC` compuiler option. Add `-fPIC` to the configuration options. E.g.,
+	All source codes should be compiled with the `-fPIC` compuiler option. Add `-fPIC` to the configuration options. E.g.,
 
      ```shell
 	 ./configure CFLAGS=-fPIC FFLAGS=-fPIC try_foxflags=-fPIC MPIF90=mpif90
+	  make pwall
+	  export qedir=`pwd`
      ```
 
-	Intel compiler:
-
-
-     ```shell
-	 ./configure CFLAGS=-fPIC FFLAGS=-fPIC try_foxflags=-fPIC MPIF90=mpiifort
-	 ```
-
-   + `make pw` or `make pwlibs`.
-
  - **QEpy**
 
      ```shell
 	 git clone --recurse-submodules https://gitlab.com/shaoxc/qepy.git
-     qedir=${QE} oldxml=yes ldau=yes tddft=yes python -m pip install -U ./qepy
+     oldxml=yes ldau=yes tddft=yes python -m pip install -U ./qepy
 	 ```
 
 ## Manual and Tutorials
-
   See [QEpy's website](http://qepy.rutgers.edu) for details.
```

### Comparing `qepy-0.0.2rc2/README.md` & `qepy-0.0.3rc0/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -16,35 +16,36 @@
 ## Requirements
  - [Python](https://www.python.org/) (>=3.7)
  - [NumPy](https://docs.scipy.org/doc/numpy/reference/) (>=1.18.0)
  - [f90wrap](https://github.com/jameskermode/f90wrap) (>=0.2.8)
  - [Quantum ESPRESSO ](https://gitlab.com/QEF/q-e/-/releases/qe-6.5) (=6.5)
  - Compiler ([GNU](https://gcc.gnu.org/fortran/)(Recommended) or [Intel](https://software.intel.com/content/www/us/en/develop/tools/oneapi/components/fortran-compiler.html))
 
-## Install
+## Installation
+### Pip
+   Using pip can easy install the release version (serial) of QEpy from [PyPI](https://pypi.org/project/qepy).
+
+```shell
+python -m pip install qepy
+```
+
+### Source
+
  - **QE**
 
-	All static libraries should be compiled with the `-fPIC` compuiler option. Add `-fPIC` to the configuration options. E.g.,
+	All source codes should be compiled with the `-fPIC` compuiler option. Add `-fPIC` to the configuration options. E.g.,
 
      ```shell
 	 ./configure CFLAGS=-fPIC FFLAGS=-fPIC try_foxflags=-fPIC MPIF90=mpif90
+	  make pwall
+	  export qedir=`pwd`
      ```
 
-	Intel compiler:
-
-
-     ```shell
-	 ./configure CFLAGS=-fPIC FFLAGS=-fPIC try_foxflags=-fPIC MPIF90=mpiifort
-	 ```
-
-   + `make pw` or `make pwlibs`.
-
  - **QEpy**
 
      ```shell
 	 git clone --recurse-submodules https://gitlab.com/shaoxc/qepy.git
-     qedir=${QE} oldxml=yes ldau=yes tddft=yes python -m pip install -U ./qepy
+     oldxml=yes ldau=yes tddft=yes python -m pip install -U ./qepy
 	 ```
 
 ## Manual and Tutorials
-
   See [QEpy's website](http://qepy.rutgers.edu) for details.
```

### Comparing `qepy-0.0.2rc2/doc/Makefile` & `qepy-0.0.3rc0/doc/Makefile`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/doc/make.bat` & `qepy-0.0.3rc0/doc/make.bat`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/doc/source/QEpy.bib` & `qepy-0.0.3rc0/doc/source/QEpy.bib`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/doc/source/conf.py` & `qepy-0.0.3rc0/doc/source/conf.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/doc/source/contact.rst` & `qepy-0.0.3rc0/doc/source/contact.rst`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/doc/source/development/documentation.rst` & `qepy-0.0.3rc0/doc/source/development/documentation.rst`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/doc/source/faq.rst` & `qepy-0.0.3rc0/doc/source/faq.rst`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/doc/source/index.rst` & `qepy-0.0.3rc0/doc/source/index.rst`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/doc/source/install.rst` & `qepy-0.0.3rc0/doc/source/install.rst`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/doc/source/qepy/calculator.rst` & `qepy-0.0.3rc0/doc/source/qepy/calculator.rst`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/doc/source/templates/breadcrumbs.html` & `qepy-0.0.3rc0/doc/source/templates/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/doc/source/templates/footer.html` & `qepy-0.0.3rc0/doc/source/templates/footer.html`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/doc/source/tutorials/jupyter/dirac_exchange.ipynb` & `qepy-0.0.3rc0/doc/source/tutorials/jupyter/dirac_exchange.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/doc/source/tutorials/jupyter/dos_band_graphene.ipynb` & `qepy-0.0.3rc0/doc/source/tutorials/jupyter/dos_band_graphene.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/doc/source/tutorials/jupyter/qepy_scf.ipynb` & `qepy-0.0.3rc0/doc/source/tutorials/jupyter/qepy_scf.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/doc/source/tutorials/jupyter/qepy_scf_iterative.ipynb` & `qepy-0.0.3rc0/doc/source/tutorials/jupyter/qepy_scf_iterative.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/doc/source/tutorials/jupyter/test_ecutwfc.ipynb` & `qepy-0.0.3rc0/doc/source/tutorials/jupyter/test_ecutwfc.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/doc/source/tutorials/jupyter/test_eos_vc.ipynb` & `qepy-0.0.3rc0/doc/source/tutorials/jupyter/test_eos_vc.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/doc/source/tutorials/jupyter/test_kpoints.ipynb` & `qepy-0.0.3rc0/doc/source/tutorials/jupyter/test_kpoints.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/ase/Al_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/ase/Al_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/ase/qe_in.in` & `qepy-0.0.3rc0/examples/ase/qe_in.in`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/ase/test_ase_nvt.py` & `qepy-0.0.3rc0/examples/ase/test_ase_nvt.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/ase/test_ase_scf.py` & `qepy-0.0.3rc0/examples/ase/test_ase_scf.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/develop/pw/Al_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/develop/pw/Al_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/develop/pw/qe_in.in` & `qepy-0.0.3rc0/examples/develop/pw/qe_in.in`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/develop/pw/test_pwscf.py` & `qepy-0.0.3rc0/examples/develop/pw/test_pwscf.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/develop/pw/test_pwscf_scf.py` & `qepy-0.0.3rc0/examples/develop/pw/test_pwscf_scf.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/develop/pw/tmp2energy.py` & `qepy-0.0.3rc0/examples/develop/pw/tmp2energy.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/develop/pw/tmp2energy_pw.py` & `qepy-0.0.3rc0/examples/develop/pw/tmp2energy_pw.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/DATA/Al.pbe-nl-kjpaw_psl.1.0.0.UPF` & `qepy-0.0.3rc0/examples/jupyter/DATA/Al.pbe-nl-kjpaw_psl.1.0.0.UPF`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/DATA/Al_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/jupyter/DATA/Al_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/DATA/C.pbe-rrkjus.UPF` & `qepy-0.0.3rc0/examples/jupyter/DATA/C.pbe-rrkjus.UPF`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/DATA/H_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/jupyter/DATA/H_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/DATA/O_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/jupyter/DATA/O_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/band/C.pbe-rrkjus.UPF` & `qepy-0.0.3rc0/examples/jupyter/band/C.pbe-rrkjus.UPF`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/band/dos_band_graphene.ipynb` & `qepy-0.0.3rc0/examples/jupyter/band/dos_band_graphene.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/colab/qepy_colab.ipynb` & `qepy-0.0.3rc0/examples/jupyter/colab/qepy_colab.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/eos/Al.pbe-nl-kjpaw_psl.1.0.0.UPF` & `qepy-0.0.3rc0/examples/jupyter/eos/Al.pbe-nl-kjpaw_psl.1.0.0.UPF`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/eos/test_eos_slow.ipynb` & `qepy-0.0.3rc0/examples/jupyter/eos/test_eos_slow.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/eos/test_eos_vc.ipynb` & `qepy-0.0.3rc0/examples/jupyter/eos/test_eos_vc.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/ext/Al_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/jupyter/ext/Al_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/ext/dftpy_xc.ipynb` & `qepy-0.0.3rc0/examples/jupyter/ext/dftpy_xc.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/ext/dirac_exchange.ipynb` & `qepy-0.0.3rc0/examples/jupyter/ext/dirac_exchange.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/nvt/H_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/jupyter/nvt/H_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/nvt/O_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/jupyter/nvt/O_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/nvt/ase_nvt.ipynb` & `qepy-0.0.3rc0/examples/jupyter/nvt/ase_nvt.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/nvt/qe_in.in` & `qepy-0.0.3rc0/examples/jupyter/nvt/qe_in.in`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/scf/Al.pbe-nl-kjpaw_psl.1.0.0.UPF` & `qepy-0.0.3rc0/examples/jupyter/scf/Al.pbe-nl-kjpaw_psl.1.0.0.UPF`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/scf/Al_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/jupyter/pp/Al_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/scf/dftpy_mixer.ipynb` & `qepy-0.0.3rc0/examples/jupyter/scf/dftpy_mixer.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/scf/qe_in.in` & `qepy-0.0.3rc0/examples/jupyter/scf/qe_in.in`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/scf/qepy_iterative.ipynb` & `qepy-0.0.3rc0/examples/jupyter/scf/qepy_iterative.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/scf/qepy_qeinput.ipynb` & `qepy-0.0.3rc0/examples/jupyter/scf/qepy_qeinput.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/scf/qepy_scf.ipynb` & `qepy-0.0.3rc0/examples/jupyter/scf/qepy_scf.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/scf/qepy_scf_iterative.ipynb` & `qepy-0.0.3rc0/examples/jupyter/scf/qepy_scf_iterative.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/testing/Al.pbe-nl-kjpaw_psl.1.0.0.UPF` & `qepy-0.0.3rc0/examples/jupyter/testing/Al.pbe-nl-kjpaw_psl.1.0.0.UPF`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/testing/test_degauss.ipynb` & `qepy-0.0.3rc0/examples/jupyter/testing/test_degauss.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/testing/test_ecutwfc.ipynb` & `qepy-0.0.3rc0/examples/jupyter/testing/test_ecutwfc.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/jupyter/testing/test_kpoints.ipynb` & `qepy-0.0.3rc0/examples/jupyter/testing/test_kpoints.ipynb`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/opt/ase/out/ase.out` & `qepy-0.0.3rc0/examples/opt/ase/out/ase.out`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/opt/ase/out/qepy.out` & `qepy-0.0.3rc0/examples/opt/ase/out/qepy.out`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/opt/ase/si_pbe_v1.uspp.F.UPF` & `qepy-0.0.3rc0/examples/opt/ase/si_pbe_v1.uspp.F.UPF`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/opt/ase/test_ase_opt.py` & `qepy-0.0.3rc0/examples/opt/ase/test_ase_opt.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/opt/ase/vcrelax.in` & `qepy-0.0.3rc0/examples/opt/ase/vcrelax.in`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/opt/qe/out/qepy.out` & `qepy-0.0.3rc0/examples/opt/qe/out/qepy.out`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/opt/qe/out/ref.out` & `qepy-0.0.3rc0/examples/opt/qe/out/ref.out`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/opt/qe/qe_relax.py` & `qepy-0.0.3rc0/examples/opt/qe/qe_relax.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/opt/qe/si_pbe_v1.uspp.F.UPF` & `qepy-0.0.3rc0/examples/opt/qe/si_pbe_v1.uspp.F.UPF`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/opt/qe/vcrelax.in` & `qepy-0.0.3rc0/examples/opt/qe/vcrelax.in`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/original/6.5/Al_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/jupyter/scf/Al_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/original/6.5/qe_in.in` & `qepy-0.0.3rc0/examples/original/6.5/qe_in.in`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/original/6.5/run_pwscf.py` & `qepy-0.0.3rc0/examples/original/6.5/run_pwscf.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/original/6.8/Al_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/original/6.5/Al_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/original/6.8/qe_in.in` & `qepy-0.0.3rc0/examples/original/6.8/qe_in.in`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/scf/Al_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/original/6.8/Al_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/scf/qe_in.in` & `qepy-0.0.3rc0/examples/scf/qe_in.in`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/scf/test_pwscf.py` & `qepy-0.0.3rc0/examples/scf/test_pwscf.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/scf/test_pwscf_iterative.py` & `qepy-0.0.3rc0/examples/scf/test_pwscf_iterative.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/tddft/Al_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/scf/Al_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/tddft/qe_in.in` & `qepy-0.0.3rc0/examples/tddft/qe_in.in`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/tddft/test_ce_tddft.py` & `qepy-0.0.3rc0/examples/tddft/test_ce_tddft.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/tddft/test_ce_tddft_restart.py` & `qepy-0.0.3rc0/examples/tddft/test_ce_tddft_restart.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/test/DATA/Al_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/tddft/Al_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/test/DATA/al_md_3.traj` & `qepy-0.0.3rc0/examples/test/DATA/al_md_3.traj`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/test/DATA/oldxml/al_oldxml.save/Al_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/test/DATA/Al_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/test/DATA/oldxml/al_oldxml.save/K00001/eigenval.xml` & `qepy-0.0.3rc0/examples/test/DATA/oldxml/al_oldxml.save/K00001/eigenval.xml`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/test/DATA/oldxml/al_oldxml.save/charge-density.dat` & `qepy-0.0.3rc0/examples/test/DATA/oldxml/al_oldxml.save/charge-density.dat`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/test/DATA/oldxml/al_oldxml.save/data-file.xml` & `qepy-0.0.3rc0/examples/test/DATA/oldxml/al_oldxml.save/data-file.xml`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/test/DATA/oldxml/al_oldxml.wfc1` & `qepy-0.0.3rc0/examples/test/DATA/oldxml/al_oldxml.wfc1`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/test/DATA/oldxml_collect/al_oldxml.save/Al_ONCV_PBE-1.2.upf` & `qepy-0.0.3rc0/examples/test/DATA/oldxml/al_oldxml.save/Al_ONCV_PBE-1.2.upf`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/eigenval.xml` & `qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/eigenval.xml`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/evc.dat` & `qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/evc.dat`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/gkvectors.dat` & `qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/K00001/gkvectors.dat`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/test/DATA/oldxml_collect/al_oldxml.save/charge-density.dat` & `qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/charge-density.dat`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/test/DATA/oldxml_collect/al_oldxml.save/data-file.xml` & `qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/data-file.xml`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/test/DATA/oldxml_collect/al_oldxml.save/gvectors.dat` & `qepy-0.0.3rc0/examples/test/DATA/oldxml_collect/al_oldxml.save/gvectors.dat`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/test/DATA/qe_fake.in` & `qepy-0.0.3rc0/examples/test/DATA/qe_fake.in`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/test/DATA/qe_in.in` & `qepy-0.0.3rc0/examples/test/DATA/qe_in.in`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/test/qe-6.5/test.sh` & `qepy-0.0.3rc0/examples/test/qe-6.5/test.sh`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/test/qe-6.5/test_ce_tddft.py` & `qepy-0.0.3rc0/examples/test/qe-6.5/test_ce_tddft.py`

 * *Files 4% similar despite different names*

```diff
@@ -26,33 +26,32 @@
 
         etotal = qepy.ener.get_etot()
         self.assertTrue(np.isclose(etotal, -552.93477389, atol = 1E-6))
 
         qepy.punch('all')
 
     def test_1_tddft_continue(self):
-        embed = qepy.qepy_common.embed_base()
         qepy.qepy_tddft_readin(inputfile)
-        qepy.qepy_tddft_main_setup(embed)
-        qepy.qepy_molecule_optical_absorption(embed)
+        qepy.qepy_tddft_main_setup()
+        qepy.qepy_molecule_optical_absorption()
         qepy.qepy_stop_run(0, print_flag=0, what='no', finalize=False)
         qepy.qepy_stop_tddft(0)
 
     def test_2_tddft_iterative(self):
-        qepy.qepy_tddft_main_initial(inputfile, commf)
-        qepy.read_file()
         embed = qepy.qepy_common.embed_base()
+        qepy.qepy_tddft_main_initial(inputfile, commf, embed = embed)
+        qepy.read_file()
         embed.tddft.iterative = True
-        qepy.qepy_tddft_main_setup(embed)
+        qepy.qepy_tddft_main_setup()
 
         for i in range(5):
-            qepy.qepy_molecule_optical_absorption(embed)
+            qepy.qepy_molecule_optical_absorption()
         dip = qepy.qepy_tddft_common.get_array_dipole().copy()
         embed.tddft.finish = True
-        qepy.qepy_molecule_optical_absorption(embed)
+        qepy.qepy_molecule_optical_absorption()
         qepy.qepy_stop_tddft(0)
 
         assert(abs(dip[0, 0] - 0.54355)<1E-3)
 
     def test_9_clean(self):
         if comm and comm.rank == 0 :
             path = pathlib.Path('.')
```

### Comparing `qepy-0.0.2rc2/examples/test/qe-6.5/test_comm.py` & `qepy-0.0.3rc0/examples/test/qe-6.5/test_comm.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/test/qe-6.5/test_oldxml.py` & `qepy-0.0.3rc0/examples/test/qe-6.5/test_oldxml.py`

 * *Files 7% similar despite different names*

```diff
@@ -4,43 +4,46 @@
 
 try:
     from mpi4py import MPI
     comm = MPI.COMM_WORLD
 except Exception:
     comm = None
 
-path = pathlib.Path(__file__).resolve().parent / 'DATA/oldxml'
-path = pathlib.Path(__file__).resolve().parent / 'DATA/oldxml_collect'
 
 def test_oldxml():
+    path = pathlib.Path(__file__).resolve().parent / 'DATA/oldxml'
+    if comm and comm.size > 1 : return
     inputobj = qepy.qepy_common.input_base()
     inputobj.prefix = 'al_oldxml'
     inputobj.tmp_dir = str(path) + '/'
     if comm : inputobj.my_world_comm = comm.py2f()
-    qepy.qepy_initial(inputobj)
-    qepy.oldxml_read_file()
     embed = qepy.qepy_common.embed_base()
-    qepy.qepy_calc_energies(embed)
+    qepy.qepy_initial(inputobj, embed = embed)
+    qepy.oldxml_read_file()
+    qepy.qepy_calc_energies()
     energy = embed.etotal
     assert np.isclose(energy, -552.93477389, atol = 1E-6)
     qepy.qepy_stop_run(0, what = 'no')
 
 def test_oldxml_collect():
+    path = pathlib.Path(__file__).resolve().parent / 'DATA/oldxml_collect'
     inputobj = qepy.qepy_common.input_base()
     inputobj.prefix = 'al_oldxml'
     inputobj.tmp_dir = str(path) + '/'
     if comm : inputobj.my_world_comm = comm.py2f()
+    embed = qepy.qepy_common.embed_base()
+    qepy.qepy_common.set_embed(embed)
     qepy.qepy_initial(inputobj)
     qepy.oldxml_read_file()
+    qepy.qepy_calc_energies()
     # 
-    wfc = path / 'al_oldxml.wfc1'
-    if wfc.is_file(): wfc.unlink()
+    if qepy.io_global.get_ionode():
+        for f in path.glob('al_oldxml.wfc*'):
+            f.unlink()
     # 
-    embed = qepy.qepy_common.embed_base()
-    qepy.qepy_calc_energies(embed)
     energy = embed.etotal
     assert np.isclose(energy, -552.93477389, atol = 1E-6)
     qepy.qepy_stop_run(0, what = 'no')
 
 if __name__ == "__main__":
     test_oldxml()
     test_oldxml_collect()
```

### Comparing `qepy-0.0.2rc2/examples/test/qe-6.5/test_pwscf.py` & `qepy-0.0.3rc0/examples/test/qe-6.5/test_pwscf.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,17 @@
 
 path = pathlib.Path(__file__).resolve().parent / 'DATA'
 inputfile = path / 'qe_in.in'
 
 
 class Test(unittest.TestCase):
     def test_scf(self):
-        qepy.qepy_pwscf(inputfile, commf)
         embed = qepy.qepy_common.embed_base()
-        qepy.qepy_electrons_scf(2, 0, embed)
+        qepy.qepy_pwscf(inputfile, commf, embed = embed)
+        qepy.qepy_electrons_scf(2, 0)
 
         conv_flag = bool(qepy.control_flags.get_conv_elec())
         self.assertTrue(conv_flag)
 
         etotal = embed.etotal
         self.assertTrue(np.isclose(etotal, -552.93477389, atol = 1E-6))
```

### Comparing `qepy-0.0.2rc2/examples/test/qe-6.5/test_pwscf_scf.py` & `qepy-0.0.3rc0/examples/test/qe-6.5/test_pwscf_scf.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,23 +13,24 @@
 
 path = pathlib.Path(__file__).resolve().parent / 'DATA'
 inputfile = path / 'qe_in.in'
 
 
 class Test(unittest.TestCase):
     def test_scf(self):
-        qepy.qepy_pwscf(inputfile, commf)
         embed = qepy.qepy_common.embed_base()
+        qepy.qepy_common.set_embed(embed)
+        qepy.qepy_pwscf(inputfile, commf)
         # embed.ldescf = True # add scf correction energy
         embed.iterative = True
         for i in range(60):
             embed.mix_coef = -1.0
-            qepy.qepy_electrons_scf(2, 0, embed)
+            qepy.qepy_electrons_scf(2, 0)
             embed.mix_coef = 0.7
-            qepy.qepy_electrons_scf(2, 0, embed)
+            qepy.qepy_electrons_scf(2, 0)
             if qepy.control_flags.get_conv_elec() : break
 
         conv_flag = bool(qepy.control_flags.get_conv_elec())
         self.assertTrue(conv_flag)
 
         etotal = embed.etotal
         self.assertTrue(np.isclose(etotal, -552.93477389, atol = 1E-6))
```

### Comparing `qepy-0.0.2rc2/examples/test/test.sh` & `qepy-0.0.3rc0/examples/test/test.sh`

 * *Files 14% similar despite different names*

```diff
@@ -3,14 +3,21 @@
 	if [ $1 -ne 0 ]
 	then
 		echo "!!!ERROR: something wrong in the test : exit code = $1"
 		exit $1
 	fi
 }
 
+if [ -z "$MPIRUN" ]
+then
+	mpirun=mpirun
+else
+	mpirun=$MPIRUN
+fi
+
 serial='y'
 parallel=''
 if [ $# -gt 1 ]
 then
 	parallel='y'
 elif [ $# -eq 1 ]
 then
@@ -30,11 +37,11 @@
 	done
 fi
 
 if [ $parallel ]; then
 	echo "####################Test MPI version#######################"
 	for f in *py
 	do
-		mpirun -n 2 python3 -m pytest --with-mpi $f
+		$mpirun -n 2 python3 -m pytest --with-mpi $f
 		check_exit $?
 	done
 fi
```

### Comparing `qepy-0.0.2rc2/examples/test/test_ase_md.py` & `qepy-0.0.3rc0/examples/test/test_ase_md.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/test/test_ce_tddft.py` & `qepy-0.0.3rc0/examples/test/test_ce_tddft.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/test/test_oldxml.py` & `qepy-0.0.3rc0/examples/test/test_oldxml.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,32 +1,35 @@
+import qepy
 from qepy.driver import Driver
 import numpy as np
 import pathlib
 
 try:
     from mpi4py import MPI
     comm = MPI.COMM_WORLD
 except Exception:
     comm = None
 
 def test_oldxml():
+    if comm and comm.size > 1 : return
     path = pathlib.Path(__file__).resolve().parent / 'DATA/oldxml'
     driver = Driver(comm = comm, prefix = 'al_oldxml', outdir=path, task = 'nscf')
     energy = driver.get_energy()
     assert np.isclose(energy, -552.93477389, atol = 1E-6)
     driver.stop(what = 'no')
 
 def test_oldxml_collect():
     path = pathlib.Path(__file__).resolve().parent / 'DATA/oldxml_collect'
     driver = Driver(comm = comm, prefix = 'al_oldxml', outdir=path, task = 'nscf')
-    wfc = path / 'al_oldxml.wfc1'
-    if wfc.is_file(): wfc.unlink()
-    wfc = path / 'al_oldxml.wfc'
-    if wfc.is_file(): wfc.unlink()
     energy = driver.get_energy()
+    #
+    if driver.is_root :
+        for f in path.glob('al_oldxml.wfc*'):
+            f.unlink()
+    #
     assert np.isclose(energy, -552.93477389, atol = 1E-6)
     driver.stop(what = 'no')
 
 
 if __name__ == "__main__":
     test_oldxml()
     test_oldxml_collect()
```

### Comparing `qepy-0.0.2rc2/examples/test/test_pwscf.py` & `qepy-0.0.3rc0/examples/test/test_pwscf.py`

 * *Files 10% similar despite different names*

```diff
@@ -25,7 +25,9 @@
         print('forces :\n', forces)
         print('stress :\n', stress)
     assert converged
     assert np.isclose(energy, -552.93477389, atol = 1E-6)
     assert np.isclose(forces[0, 0], -0.00835135, atol = 1E-3)
     assert np.isclose(stress[1, 1], -0.00256059, atol = 1E-3)
     driver.stop()
+
+test_scf()
```

### Comparing `qepy-0.0.2rc2/examples/test/test_pwscf_iterative.py` & `qepy-0.0.3rc0/examples/test/test_pwscf_iterative.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/examples/test/test_readfile.py` & `qepy-0.0.3rc0/examples/test/test_readfile.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/install/Makefile` & `qepy-0.0.3rc0/install/Makefile`

 * *Files 7% similar despite different names*

```diff
@@ -1,31 +1,32 @@
 include make.qe.inc
 
 SRC_DIRS := ./
 PY_SRC_DIR := ./
 PYTHON := $(or ${PYTHON}, python)
 
 QEMODS := $(wildcard ${QEDIR}/*/*.a) $(wildcard ${QEDIR}/*/*/*.a)
-QEMODS := ${QEDIR}/PW/src/libpw.a ${QEDIR}/Modules/libqemod.a $(filter-out ${QEDIR}/Modules/libqemod.a, $(QEMODS))
+QEMODS := ${QEDIR}/PW/src/libpw.a ${QEDIR}/Modules/libqemod.a $(filter-out ${QEDIR}/Modules/libqemod.a, $(QEMODS)) ${QEDIR}/Modules/libqemod.a 
 #$(info 'QEMODS', ${QEMODS})
 
 QEINC := $(wildcard ${QEDIR}/*/Makefile) $(wildcard ${QEDIR}/*/*/Makefile)
 QEINC := $(addprefix -I, ${QEINC})
 QEINC := $(QEINC:%/Makefile=%/) -I.
 
 TDDFT_SOURCES = tddft_module.f90
 TDDFT_FILES = ${TDDFT_SOURCES}
 
-QEPY_ADD := qepy_scatter_mod.f90 qepy_common.f90 qepy_mod.f90 funct.f90
+QEPY_ADD := qepy_common.f90 qepy_mod.f90 \
+			scatter_mod.f90 funct.f90 potinit.f90 wfcinit.f90\
+			pw_restart_new.f90 read_file_new.f90 qes_read_module.f90
 
 QEPY_SOURCES := qepy_setlocal.f90 qepy_v_of_rho.f90 qepy_pw2casino_write.f90 \
-              qepy_hinit1.f90 qepy_potinit.f90 qepy_wfcinit.f90 qepy_pw_restart_new.f90 \
               qepy_init_run.f90 qepy_pwscf.f90 qepy_run_pwscf.f90 qepy_electrons.f90 \
-              qepy_forces.f90 qepy_stress.f90 qepy_stop_run.f90 qepy_api.f90 \
-              qepy_read_file_new.f90 qepy_electrons_nscf.f90 qepy_sum_band.f90
+              qepy_electrons_nscf.f90 qepy_hinit1.f90 qepy_forces.f90 qepy_stop_run.f90 \
+              qepy_stress.f90 
 
 OLDXML_SOURCES := oldxml_qexml.f90 oldxml_xml_io_base.f90 \
                 oldxml_io_rho_xml.f90 oldxml_pw_restart.f90 \
                 oldxml_wfcinit.f90 oldxml_potinit.f90 oldxml_read_file.f90
 
 QEPY_TDDFT_SOURCES := qepy_tddft_common.f90 \
                     qepy_molecule_optical_absorption.f90 qepy_tddft_main.f90 \
@@ -72,14 +73,17 @@
 F90WRAP_FILES = f90wrap_*.f90
 
 WRAP_FPP_FILES = $(notdir $(WRAP_FILES:%.f90=%.fpp))
 
 $(info 'F90FLAGS', ${F90FLAGS})
 F2FLAGS = $(F90FLAGS) $(QEINC) $(FOLDXML)
 #$(info 'F2FLAGS', ${F2FLAGS})
+export LDFLAGS := ${LDFLAGS}
+# For the old version numpy (e.g 1.17.3)
+export NPY_DISTUTILS_APPEND_FLAGS=1
 
 ifeq ($(findstring -D__MPI, ${F2FLAGS}), -D__MPI)
    GOAL=mpi
 else
    GOAL=serial
 endif
```

### Comparing `qepy-0.0.2rc2/install/Makefile.cetddft` & `qepy-0.0.3rc0/install/Makefile.cetddft`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/install/kind_map.json` & `qepy-0.0.3rc0/install/kind_map.json`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/install/make.depend` & `qepy-0.0.3rc0/install/make.depend`

 * *Files 21% similar despite different names*

```diff
@@ -1,44 +1,54 @@
-apply_efield.o : tddft_module.o
-molecule_operators.o : tddft_module.o
-molecule_optical_absorption.o : tddft_module.o
+local_dos.o : pw_restart_new.o
+local_dos_mag.o : pw_restart_new.o
+oldxml_io_rho_xml.o : funct.o
 oldxml_io_rho_xml.o : oldxml_xml_io_base.o
+oldxml_potinit.o : funct.o
 oldxml_potinit.o : oldxml_io_rho_xml.o
 oldxml_potinit.o : oldxml_xml_io_base.o
+oldxml_pw_restart.o : funct.o
 oldxml_pw_restart.o : oldxml_io_rho_xml.o
 oldxml_pw_restart.o : oldxml_qexml.o
 oldxml_pw_restart.o : oldxml_xml_io_base.o
+oldxml_read_file.o : funct.o
 oldxml_read_file.o : oldxml_io_rho_xml.o
 oldxml_read_file.o : oldxml_pw_restart.o
 oldxml_read_file.o : oldxml_xml_io_base.o
 oldxml_wfcinit.o : oldxml_pw_restart.o
-qepy_api.o : qepy_common.o
+oldxml_wfcinit.o : pw_restart_new.o
+potinit.o : funct.o
+pw_restart_new.o : funct.o
+qepy_electrons.o : funct.o
 qepy_electrons.o : qepy_common.o
 qepy_electrons_nscf.o : qepy_common.o
-qepy_energy.o : qepy_common.o
 qepy_forces.o : qepy_common.o
+qepy_init_run.o : funct.o
+qepy_init_run.o : qepy_common.o
+qepy_mod.o : funct.o
+qepy_mod.o : pw_restart_new.o
 qepy_mod.o : qepy_common.o
-qepy_mod.o : qepy_scatter_mod.o
+qepy_mod.o : scatter_mod.o
 qepy_molecule_optical_absorption.o : qepy_common.o
 qepy_molecule_optical_absorption.o : qepy_tddft_common.o
 qepy_molecule_optical_absorption.o : tddft_module.o
+qepy_pw2casino_write.o : funct.o
 qepy_pw2casino_write.o : qepy_common.o
 qepy_pwscf.o : qepy_common.o
-qepy_read_file_new.o : qepy_pw_restart_new.o
+qepy_run_pwscf.o : funct.o
 qepy_run_pwscf.o : qepy_common.o
+qepy_setlocal.o : qepy_common.o
+qepy_stress.o : funct.o
 qepy_stress.o : qepy_common.o
 qepy_tddft_main.o : qepy_common.o
 qepy_tddft_main.o : tddft_module.o
 qepy_tddft_mod.o : tddft_module.o
 qepy_tddft_routines.o : tddft_module.o
 qepy_tddft_setup.o : qepy_common.o
 qepy_tddft_setup.o : tddft_module.o
 qepy_update_ham.o : qepy_common.o
 qepy_update_ham.o : tddft_module.o
+qepy_v_of_rho.o : funct.o
 qepy_v_of_rho.o : qepy_common.o
-tddft_ch_psi_all.o : tddft_module.o
-tddft_main.o : tddft_module.o
-tddft_main.o : tddft_version.o
-tddft_routines.o : tddft_module.o
-tddft_setup.o : tddft_module.o
-update_ham.o : tddft_module.o
-wavepacket.o : tddft_module.o
+read_file_new.o : funct.o
+read_file_new.o : pw_restart_new.o
+wfcinit.o : funct.o
+wfcinit.o : pw_restart_new.o
```

### Comparing `qepy-0.0.2rc2/install/make.qe.inc` & `qepy-0.0.3rc0/install/make.qe.inc`

 * *Files 20% similar despite different names*

```diff
@@ -4,22 +4,28 @@
 
 MODULES_SOURCES = constants.f90 cell_base.f90 ions_base.f90 wavefunctions.f90 \
 				  recvec.f90 control_flags.f90 io_global.f90 check_stop.f90 \
 				  deviatoric.f90 qexsd.f90 environment.f90 read_input.f90 \
 				  mp_pools.f90 mp_bands.f90 mp_global.f90 mp_world.f90 uspp.f90
 MODULES_FILES = $(addprefix ${QEDIR}/Modules/,${MODULES_SOURCES})
 
-PW_SOURCES = pwcom.f90 scf_mod.f90 read_file_new.f90 punch.f90 \
+PW_SOURCES = pwcom.f90 scf_mod.f90 punch.f90 \
 			 atomic_wfc_mod.f90 close_files.f90 stress.f90 electrons.f90 \
 			 scale_h.f90 pw2casino.f90 forces.f90 update_pot.f90 move_ions.f90 \
 			 add_qexsd_step.f90 hinit1.f90 run_pwscf.f90 stop_run.f90 \
-			 sum_band.f90 non_scf.f90
+			 sum_band.f90 non_scf.f90 v_of_rho.f90
 PW_FILES = $(addprefix ${QEDIR}/PW/src/,${PW_SOURCES})
 
 LAXLIB_SOURCES = mp_diag.f90 la_helper.f90
 LAXLIB_FILES = $(addprefix ${QEDIR}/LAXlib/,${LAXLIB_SOURCES})
 
+PP_SOURCES = elf.f90 local_dos.f90 local_dos_mag.f90
+PP_FILES = $(addprefix ${QEDIR}/PP/src/,${PP_SOURCES})
+
 UTILXLIB_SOURCES = set_mpi_comm_4_solvers.f90
 UTILXLIB_FILES = $(addprefix ${QEDIR}/UtilXlib/,${UTILXLIB_SOURCES})
 
+FFTXLIB_SOURCES = fft_types.f90
+FFTXLIB_FILES = $(addprefix ${QEDIR}/FFTXlib/,${FFTXLIB_SOURCES})
+
 # QE_FILES is the final list to wrap
-QE_FILES = ${MODULES_FILES} ${PW_FILES} ${LAXLIB_FILES} ${UTILXLIB_FILES}
+QE_FILES = ${MODULES_FILES} ${PW_FILES} ${LAXLIB_FILES} ${UTILXLIB_FILES} ${FFTXLIB_FILES} ${PP_FILES}
```

### Comparing `qepy-0.0.2rc2/qepy/__init__.py` & `qepy-0.0.3rc0/qepy/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,17 +17,17 @@
                     attr = mod + '.' + item
                     operator.attrgetter(attr)(qepy).clear()
 
 
 qepy_clean_saved()
 __author__ = "Pavanello Research Group"
 __contact__ = "m.pavanello@rutgers.edu"
-__version__ = "0.0.2rc2"
+__version__ = "0.0.3rc0"
 __license__ = "GPL"
-__date__ = "2023-03-28"
+__date__ = "2023-04-26"
 
 try:
     from importlib.metadata import version # python >= 3.8
 except Exception :
     try:
         from importlib_metadata import version
     except Exception :
```

### Comparing `qepy-0.0.2rc2/qepy/__new__.py` & `qepy-0.0.3rc0/qepy/__new__.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/qepy/calculator.py` & `qepy-0.0.3rc0/qepy/calculator.py`

 * *Files 1% similar despite different names*

```diff
@@ -381,17 +381,17 @@
         """See :func:`qepy.driver.Driver.get_k_point_weights`"""
         return self.driver.get_k_point_weights()
 
     def get_pseudo_density(self, spin=None, pad=True, gather = False):
         """See :func:`qepy.driver.Driver.get_pseudo_density`"""
         return self.driver.get_pseudo_density(spin=spin, pad=pad, gather=gather) / (units['Bohr'] ** 3)
 
-    def get_effective_potential(self, spin=0, pad=True):
-        """See :func:`qepy.driver.Driver.get_effective_potential`"""
-        return self.driver.get_effective_potential(spin=spin, pad=pad)
+    # def get_effective_potential(self, spin=0, pad=True):
+        # """See :func:`qepy.driver.Driver.get_effective_potential`"""
+        # return self.driver.get_effective_potential(spin=spin, pad=pad)
 
     def get_pseudo_wave_function(self, band=None, kpt=0, spin=0, broadcast=True,
                                  pad=True):
         """See :func:`qepy.driver.Driver.get_pseudo_wave_function`"""
         return self.driver.get_pseudo_wave_function(band=band, kpt=kpt, spin=spin, broadcast=broadcast, pad=pad)
 
     def get_eigenvalues(self, kpt=0, spin=0):
```

### Comparing `qepy-0.0.2rc2/qepy/core.py` & `qepy-0.0.3rc0/qepy/core.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/qepy/driver.py` & `qepy-0.0.3rc0/qepy/driver.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,15 +1,39 @@
 import numpy as np
 import tempfile
 import os
+from functools import wraps
 import qepy
 from qepy.core import env
 from qepy.io import QEInput
 from qepy import constants
 
+def gathered(function):
+    @wraps(function)
+    def wrapper(self, **kwargs):
+        out = kwargs.get('out', None)
+        gather = kwargs.get('gather', True)
+        if out is None : out = self.create_array(gather=gather, kind='rho')
+        if gather and self.nproc > 1 :
+            arr = self.create_array(gather=False, kind='rho')
+        else :
+            arr = out
+        #
+        kwargs['out'] = arr
+        results = function(self, **kwargs)
+        #
+        if gather and self.nproc > 1 :
+            qepy.qepy_mod.qepy_get_value(arr, out, gather = True)
+            if isinstance(results, (tuple, list)):
+                results = out, *results[1:]
+            else :
+                results = out
+        return results
+    return wrapper
+
 class Driver(object) :
     """
     The driver of QEpy.
 
     Parameters
     ----------
     inputfile : str
@@ -65,28 +89,29 @@
              + potential : Ry
              + density : 1.0/Bohr**3
 
     """
 
     def __init__(self, inputfile = None, comm = None, ldescf = False, iterative = False,
              task = 'scf', embed = None, prefix = None, outdir = None, logfile = None,
-             qe_options = None, prog = 'pw', progress = False, **kwargs):
+             qe_options = None, prog = 'pw', progress = False, atoms = None, **kwargs):
         if embed is None :
             embed = qepy.qepy_common.embed_base()
         self.task = task
         self.embed = embed
         self.comm = comm
         self.inputfile = inputfile
         self.iterative = iterative
         self.prefix = prefix
         self.outdir = outdir
         self.logfile = logfile
         self.qe_options = qe_options
         self.prog = prog
         self.progress = progress
+        self.atoms = atoms
         #
         self.embed.ldescf = ldescf
         #
         self.comm = comm
         self.qepy = qepy
         self.qeinput = QEInput()
         #
@@ -117,14 +142,41 @@
     def comm(self, value):
         self._comm = value
         if self.comm is not None and hasattr(self.comm, 'py2f') :
             self.commf = self.comm.py2f()
         else :
             self.commf = self.comm
 
+    @property
+    def is_root(self):
+        """Whether it is the root.
+
+        If the comm is set, root is rank == 0.
+        Otherwise root is ionode of QE.
+        """
+        if hasattr(self.comm, 'rank'):
+            return self.comm.rank == 0
+        else :
+            return qepy.io_global.get_ionode()
+
+    @property
+    def nproc(self):
+        if hasattr(self.comm, 'size'):
+            return self.comm.size
+        else :
+            return qepy.mp_world.get_nproc()
+
+    @property
+    def qe_is_mpi(self):
+        return qepy.qepy_common.get_is_mpi()
+
+    @property
+    def qe_is_openmp(self):
+        return qepy.qepy_common.get_is_openmp()
+
     def restart(self, prog=None, **kwargs):
         prog = prog or self.prog
         self.driver_initialize()
 
     def driver_initialize(self, **kwargs):
         """ Initialize the driver
 
@@ -149,98 +201,99 @@
         """
         # stop the last driver and save new driver
         if not self.progress :
             if hasattr(env['DRIVER'], 'stop'): env['DRIVER'].stop()
             env['DRIVER'] = self
         #
         self._init_log()
+        qepy.qepy_common.set_embed(self.embed)
         #
         inputfile=self.inputfile
         commf=self.commf
         task=self.task
         qe_options = self.qe_options
         prog = self.prog
         #
         if qe_options :
             inputfile, basefile = 'input_tmp.in', inputfile
-            self.qeinput.write_qe_input(inputfile, basefile=basefile, qe_options=qe_options, prog=prog)
+            self.qeinput.write_qe_input(inputfile, atoms = self.atoms, basefile=basefile, qe_options=qe_options, prog=prog)
         #
         if task == 'optical' :
-            self.tddft_initialize(inputfile=inputfile, commf = commf, embed = self.embed, **kwargs)
+            self.tddft_initialize(inputfile=inputfile, commf = commf, **kwargs)
         elif task == 'nscf' :
             inputobj = qepy.qepy_common.input_base()
             if self.prefix : inputobj.prefix = self.prefix
             if self.outdir : inputobj.tmp_dir = str(self.outdir) + '/'
             if commf : inputobj.my_world_comm = commf
             qepy.qepy_initial(inputobj)
             tmpdir = inputobj.tmp_dir.decode().strip() + inputobj.prefix.decode().strip() + '.save' + '/'
             if os.path.isfile(tmpdir + 'data-file.xml'): # only works for qe-6.5 !
+                if not hasattr(qepy, 'oldxml_read_file') :
+                    raise AttributeError("Please reinstall the QEpy with 'oldxml=yes'.")
                 qepy.oldxml_read_file()
             else :
-                qepy.qepy_read_file()
+                qepy.read_file()
+            qepy.qepy_mod.qepy_open_files()
         else :
-            qepy.qepy_pwscf(inputfile, commf, embed = self.embed)
+            qepy.qepy_pwscf(inputfile, commf)
             self.embed.iterative = self.iterative
             if self.embed.iterative :
                 qepy.control_flags.set_niter(1)
         #
         self.density = np.zeros((1, 1))
         self.iter = 0
 
-    def tddft_initialize(self, inputfile = None, commf = None, embed = None, **kwargs):
+    def tddft_initialize(self, inputfile = None, commf = None, **kwargs):
         """ Initialize the tddft
 
         Parameters
         ----------
         inputfile : str
             Name of QE input file, which also contains `&inputtddft` section.
         commf : object
             Parallel communicator (Fortran)
-        embed : object (Fortran)
-            embed object for QE
         """
         if inputfile is None : inputfile = self.inputfile
         if commf is None : commf = self.commf
-        if embed is None : embed = self.embed
         #
         if self.progress :
             qepy.wvfct.get_array_g2kin()
             qepy.qepy_tddft_readin(inputfile)
         else :
             qepy.qepy_tddft_main_initial(inputfile, commf)
             qepy.read_file()
-        qepy.qepy_tddft_main_setup(embed)
+        qepy.qepy_tddft_main_setup()
         self.embed.tddft.iterative = self.iterative
 
     def diagonalize(self, print_level = 2, **kwargs):
         """Diagonalize the hamiltonian
 
         Parameters
         ----------
         print_level :
             The level of output of QE
         """
         self.iter += 1
         if self.task == 'optical' :
-            qepy.qepy_molecule_optical_absorption(self.embed)
+            qepy.qepy_molecule_optical_absorption()
         else :
             self.embed.mix_coef = -1.0
-            qepy.qepy_electrons_scf(print_level, 0, self.embed)
+            qepy.qepy_electrons_scf(print_level, 0)
 
     def mix(self, mix_coef = 0.7, print_level = 2):
         """Mixing the density
 
         Parameters
         ----------
         print_level :
             The level of output of QE
         """
         if self.task == 'optical' : return
         self.embed.mix_coef = mix_coef
-        qepy.qepy_electrons_scf(print_level, 0, self.embed)
+        qepy.qepy_electrons_scf(print_level, 0)
 
     def check_convergence(self, **kwargs):
         """Check the convergence of the SCF"""
         converged = bool(qepy.control_flags.get_conv_elec())
         if converged and not self.embed.initial : self.end_scf()
         return converged
 
@@ -259,20 +312,20 @@
             return qepy.control_flags.get_n_scf_steps()
 
     def scf(self, print_level = 2, maxiter = None, original = False, **kwargs):
         """Run the scf/tddft until converged or maximum number of iterations"""
         if maxiter is not None and not self.embed.iterative :
             qepy.control_flags.set_niter(maxiter)
         if self.task == 'optical' :
-            qepy.qepy_molecule_optical_absorption(self.embed)
+            qepy.qepy_molecule_optical_absorption()
         elif not self.embed.iterative and self.embed.exttype < 2 :
             # Use electrons to support hybrid xc functional
             return self.electrons(original=original)
         else :
-            qepy.qepy_electrons_scf(print_level, 0, self.embed)
+            qepy.qepy_electrons_scf(print_level, 0)
         return self.embed.etotal
 
     def non_scf(self, **kwargs):
         # fix some saved variables from last scf calculations
         qepy.control_flags.set_lscf(0)
         qepy.control_flags.set_lbfgs(0)
         qepy.control_flags.set_lmd(0)
@@ -281,22 +334,22 @@
         qepy.non_scf()
         return qepy.ener.get_etot()
 
     def electrons(self, original = False, **kwargs):
         if original :
             qepy.electrons()
         else :
-            qepy.qepy_electrons(self.embed)
+            qepy.qepy_electrons()
         return qepy.ener.get_etot()
 
     def end_scf(self, **kwargs):
         """End the scf and clean the scf workspace. Only need run it in iterative mode"""
         if self.embed.iterative :
             self.embed.finish = True
-            qepy.qepy_electrons_scf(0, 0, self.embed)
+            qepy.qepy_electrons_scf(0, 0)
 
     def stop(self, exit_status = 0, what = 'all', print_flag = 0, **kwargs):
         """stop.
 
         Parameters
         ----------
         exit_status : int
@@ -329,15 +382,15 @@
         qepy.qepy_tddft_mod.qepy_cetddft_wfc2rho()
         if istep is not None :
             self.embed.tddft.istep = istep
 
     def tddft_stop(self, exit_status = 0, what = 'no', print_flag = 0, **kwargs):
         if self.embed.tddft.iterative :
             self.embed.tddft.finish = True
-            qepy.qepy_molecule_optical_absorption(self.embed)
+            qepy.qepy_molecule_optical_absorption()
         #! Do not save the PW files, otherwise the initial wfcs will be overwritten.
         qepy.qepy_stop_run(exit_status, print_flag = print_flag, what = 'no', finalize = False)
         qepy.qepy_stop_tddft(exit_status)
 
     def save(self, what = 'all', **kwargs):
         """
         Save the QE data to the disk
@@ -372,15 +425,15 @@
             energy = self.embed.etotal
         else :
             energy = self.calc_energy(**kwargs)
         return energy
 
     def calc_energy(self, **kwargs):
         """Calculate the energy with the pw2casino of QE."""
-        qepy.qepy_calc_energies(self.embed)
+        qepy.qepy_calc_energies()
         return self.embed.etotal
 
     def update_ions(self, positions = None, lattice = None, update = 0, **kwargs):
         """update the ions of QE
 
         Parameters
         ----------
@@ -394,19 +447,19 @@
 
         """
         positions = positions.T
         if lattice is not None :
             lattice = lattice.T
             if not qepy.cellmd.get_lmovecell():
                 raise ValueError(" Lattice update only works for variable-cell simulations.\n Please restart the QEpy with calculation= 'vc-relax' or 'vc-md'")
-            qepy.qepy_api.qepy_update_ions(self.embed, positions, update, lattice)
+            qepy.qepy_mod.qepy_update_ions(positions, update, lattice)
         else :
-            qepy.qepy_api.qepy_update_ions(self.embed, positions, update)
+            qepy.qepy_mod.qepy_update_ions(positions, update)
 
-    def pwscf_restart(self, oldxml=False):
+    def pwscf_restart(self, oldxml=False, starting_pot='file', starting_wfc='file'):
         """Read PW ouput/restart files.
 
         Parameters
         ----------
         oldxml : bool
              - True : read the old format xml file (qe<6.4)
              - False : read the new format xml file (qe>6.3)
@@ -414,79 +467,57 @@
         if oldxml :
             if not hasattr(qepy, 'oldxml_pw_restart') :
                 raise AttributeError("Please reinstall the QEpy with 'oldxml=yes'.")
             qepy.oldxml_pw_restart.pw_readfile('header')
             qepy.oldxml_pw_restart.pw_readfile('reset')
             qepy.oldxml_pw_restart.pw_readfile('dim')
             qepy.oldxml_pw_restart.pw_readfile('bs')
-            if qepy.basis.get_starting_pot().strip() != 'file' :
-                qepy.oldxml_potinit(starting = 'file')
-            if qepy.basis.get_starting_wfc().strip() != 'file' :
-                qepy.oldxml_wfcinit(starting = 'file')
-        else :
-            qepy.qepy_pw_restart_new.qepy_read_xml_file(alloc=False)
-            if qepy.basis.get_starting_pot().strip() != 'file' :
-                qepy.qepy_potinit(starting = 'file')
-            if qepy.basis.get_starting_wfc().strip() != 'file' :
-                qepy.qepy_wfcinit(starting = 'file')
-
-    @property
-    def is_root(self):
-        """Whether it is the root.
-
-        If the comm is set, root is rank == 0.
-        Otherwise root is ionode of QE.
-        """
-        if hasattr(self.comm, 'rank'):
-            return self.comm.rank == 0
+            if qepy.basis.get_starting_pot().strip() != starting_pot :
+                qepy.basis.set_starting_pot(starting_pot)
+                qepy.oldxml_potinit()
+            if qepy.basis.get_starting_wfc().strip() != starting_wfc :
+                qepy.basis.set_starting_wfc(starting_wfc)
+                qepy.oldxml_wfcinit()
+        else :
+            qepy.qepy_mod.qepy_restart_from_xml()
+            if qepy.basis.get_starting_pot().strip() != starting_pot :
+                qepy.basis.set_starting_pot(starting_pot)
+                qepy.potinit()
+            if qepy.basis.get_starting_wfc().strip() != starting_wfc :
+                qepy.basis.set_starting_wfc(starting_wfc)
+                qepy.wfcinit()
+
+    def create_array(self, gather = True, kind = 'rho'):
+        """Return an empty array in real space."""
+        if kind == 'rho' :
+            nspin = qepy.lsda_mod.get_nspin()
+            if gather and self.nproc > 1 :
+                nr = self.get_number_of_grid_points(gather = gather)
+                if self.is_root :
+                    out = np.zeros((np.prod(nr), nspin), order = 'F')
+                else :
+                    out = np.zeros((1, nspin), order = 'F')
+            else :
+                nnr = self.embed.dfftp.nnr
+                out = np.zeros((nnr, nspin), order = 'F')
         else :
-            return qepy.io_global.get_ionode()
-
-    @staticmethod
-    def get_ions_lattice():
-        """Return the lattice of ions."""
-        alat = qepy.cell_base.get_alat()
-        lattice = qepy.cell_base.get_array_at() * alat
-        return lattice.T
-
-    @staticmethod
-    def get_ions_positions():
-        """Return the cartesian positions of ions."""
-        alat = qepy.cell_base.get_alat()
-        pos = qepy.ions_base.get_array_tau().T * alat
-        return pos
+            raise ValueError('Only support "rho"')
+        return out
 
-    @staticmethod
-    def get_ions_symbols():
-        """Return the symbols of ions."""
-        ityp = qepy.ions_base.get_array_ityp() - 1
-        nat = qepy.ions_base.get_nat()
-        ntyp = qepy.ions_base.get_nsp()
-        label = qepy.ions_base.get_array_atm().T.view('S3')[:,0].astype('U3')[:ntyp]
-        label = [x.strip() for x in label]
-        symbols = []
-        for i in range(nat):
-            symbols.append(label[ityp[i]])
-        return symbols
+    def get_density(self, gather = True, out = None):
+        """Return density array in real space."""
+        if out is None : out = self.create_array(gather=gather, kind='rho')
+        qepy.qepy_mod.qepy_get_rho(out, gather = gather)
+        return out
 
-    def get_density(self, gather = True):
+    def get_kinetic_energy_density(self, gather = True, out = None):
         """Return density array in real space."""
-        nr = self.get_number_of_grid_points(gather = gather)
-        nspin = qepy.lsda_mod.get_nspin()
-        if gather :
-            if self.is_root :
-                if np.prod(nr) != self.density.shape[0] or nspin != self.density.shape[1] :
-                    self.density = np.empty((np.prod(nr), nspin), order = 'F')
-            else :
-                self.density = np.empty((1, nspin), order = 'F')
-        else :
-            if np.prod(nr) != self.density.shape[0] or nspin != self.density.shape[1] :
-                self.density = np.empty((np.prod(nr), nspin), order = 'F')
-        qepy.qepy_mod.qepy_get_rho(self.density, gather = gather)
-        return self.density
+        if out is None : out = self.create_array(gather=gather, kind='rho')
+        qepy.qepy_mod.qepy_get_tau(out, gather = gather)
+        return out
 
     def get_wave_function(self, band=None, kpt=0):
         """Return wave-function array in real space."""
         qepy.qepy_mod.qepy_get_evc(kpt + 1)
         nrs = np.zeros(3, dtype = 'int32')
         qepy.qepy_mod.qepy_get_grid_smooth(nrs)
         if self.is_root :
@@ -500,18 +531,14 @@
             if band.ndim == 0 : band = [band]
         wfs = []
         for ibnd in band :
             qepy.qepy_mod.qepy_get_wf(kpt + 1, ibnd + 1, wf)
             wfs.append(wf.copy())
         return wfs
 
-    def get_number_of_k_points(self):
-        """Return the number of kpoints."""
-        return qepy.klist.get_nks()
-
     def get_dipole_tddft(self):
         """Return the total dipole of tddft task."""
         # dipole = qepy.qepy_tddft_common.get_array_dipole().copy()
         dipole = self.embed.tddft.dipole
         return dipole
 
     def set_external_potential(self, potential, exttype = None, gather = True, extene  = None, **kwargs):
@@ -544,15 +571,15 @@
             self.embed.extene = extene
         else :
             self.embed.extene = 0.0
         #
         if potential is None : potential = np.zeros((1, 1))
         if potential.ndim != 2 : raise ValueError("The array should be 2-d.")
         #
-        qepy.qepy_mod.qepy_set_extpot(self.embed, potential, gather = gather)
+        qepy.qepy_mod.qepy_set_extpot(potential, gather = gather)
 
     def get_output(self):
         """Return the output of QE.
 
         It depends on the `logfile` of the initialization of the driver :
 
           - None : return None.
@@ -571,14 +598,101 @@
                 return lines
             else :
                 self.fileobj.seek(0)
                 return self.fileobj.readlines()
         else :
             return None
 
+    @gathered
+    def get_elf(self, gather = True, out = None, **kwargs):
+        """Return electron localization function."""
+        qepy.do_elf(out)
+        return out
+
+    @gathered
+    def get_rdg(self, gather = True, out = None, **kwargs):
+        """Return electron localization function."""
+        qepy.do_rdg(out)
+        return out
+#-----------------------------------------------------------------------
+
+    @gathered
+    def get_local_pp(self, gather = True, out = None, **kwargs):
+        """Return local component of the pseudopotential."""
+        for i in range(out.shape[1]):
+            out[:, i] = qepy.scf.get_array_vltot()
+        return out
+
+    @gathered
+    def get_hartree(self, gather = True, out = None, add=False, **kwargs):
+        """Return hartree information."""
+        if not add : out[:] = 0.0
+        ehart, charge = qepy.v_h(self.embed.rho.of_g[:,0], out)
+        return out, ehart, charge
+
+    @gathered
+    def get_exchange_correlation(self, gather = True, out = None, tau=None, **kwargs):
+        """Return exchange-correlation information.
+
+        TODO :
+            The interface will changed in the new version of QE!
+
+        Note :
+            For metaGGA, only return scattered tau
+        """
+        etxc = vtxc = 0.0
+        rho_obj = self.embed.rho
+        rho_core = qepy.scf.get_array_rho_core()
+        rhog_core = qepy.scf.get_array_rhog_core()
+        if qepy.funct.dft_is_meta():
+            if tau is None : tau = out*0.0
+            qepy.v_xc_meta(rho_obj, rho_core, rhog_core, etxc, vtxc, out, tau)
+            return out, etxc, vtxc, tau
+        else :
+            etxc, vtxc = qepy.v_xc(rho_obj, rho_core, rhog_core, out)
+            return out, etxc, vtxc
+
+    @gathered
+    def get_density_functional(self, gather = True, out = None, add = False, **kwargs):
+        """Return effective potential information.
+
+        Note :
+            Then final potential is saved in the v_obj
+        """
+        rho_obj = self.embed.rho
+        rho_core = qepy.scf.get_array_rho_core()
+        rhog_core = qepy.scf.get_array_rhog_core()
+        v_obj = self.embed.v
+        etotefield = 0.0
+        #
+        v_obj.of_r[:] = 0.0
+        ehart, etxc, vtxc, eth, charge = qepy.qepy_v_of_rho(rho_obj, rho_core, rhog_core, etotefield, v_obj)
+        info = [ehart, etxc, vtxc, eth, etotefield, charge]
+        if add :
+            out += v_obj.of_r
+        else :
+            out[:] = v_obj.of_r
+        return out, *info
+
+    def get_hartree_potential(self, gather = True, out = None, **kwargs):
+        return self.get_hartree(gather=gather, out=out, **kwargs)[0]
+
+    def get_exchange_correlation_potential(self, gather = True, out = None, **kwargs):
+        return self.get_exchange_correlation(gather=gather, out=out, **kwargs)[0]
+
+    def get_density_functional_potential(self, gather = True, out = None, **kwargs):
+        return self.get_density_functional(gather=gather, out=out, **kwargs)[0]
+
+    def get_effective_potential(self, gather = True, out = None, **kwargs):
+        out = self.get_local_pp(gather=gather, out=out, **kwargs)
+        out = self.get_density_functional_potential(gather=gather, out=out, add = True, **kwargs)
+        return out
+#-----------------------------------------------------------------------
+
+#-----------------------------------------------------------------------
     #ASE Calculator
     def get_potential_energy(self, **kwargs):
         """Return the potential energy."""
         return self.get_energy()
 
     def get_forces(self, icalc = 0, **kwargs):
         """Return the total forces. (n, 3)
@@ -596,100 +710,107 @@
               3   no ewald + local              011
               4   no nlcc                       100
               5   no ewald + nlcc               101
               6   no local + nlcc               110
               7   no ewald + local + nlcc       111
             ===== ============================= ===
         """
-        qepy.qepy_forces(icalc, self.embed)
+        qepy.qepy_forces(icalc)
         forces = qepy.force_mod.get_array_force().T
         return forces
 
-    def get_stress(self, **kwargs):
+    @classmethod
+    def get_stress(cls, **kwargs):
         """Return the stress (3, 3)."""
         stress = np.zeros((3, 3), order='F')
         qepy.stress(stress)
-        # qepy.qepy_stress(stress, 0, self.embed)
         return stress
 
     #ASE DFTCalculator
-    def get_number_of_bands(self):
+    @classmethod
+    def get_number_of_bands(cls):
         """Return the number of bands."""
         return qepy.wvfct.get_nbnd()
 
-    def get_xc_functional(self):
+    @classmethod
+    def get_xc_functional(cls):
         """Return the XC-functional identifier.
 
         'LDA', 'PBE', ..."""
         return qepy.funct.get_dft_short().decode("utf-8")
 
-    def get_bz_k_points(self):
+    @classmethod
+    def get_bz_k_points(cls):
         """Return all the k-points in the 1. Brillouin zone.
 
         The coordinates are relative to reciprocal latice vectors."""
         return qepy.klist.get_array_xk()
 
-    def get_number_of_spins(self):
+    @classmethod
+    def get_number_of_spins(cls):
         """Return the number of spins in the calculation.
 
         Spin-paired calculations: 1, spin-polarized calculation: 2."""
         return qepy.lsda_mod.get_nspin()
 
-    def get_spin_polarized(self):
+    @classmethod
+    def get_spin_polarized(cls):
         """Is it a spin-polarized calculation?"""
         return bool(qepy.lsda_mod.get_lsda())
 
-    def get_ibz_k_points(self):
+    @classmethod
+    def get_ibz_k_points(cls):
         """Return k-points in the irreducible part of the Brillouin zone.
 
         The coordinates are relative to reciprocal latice vectors."""
-        xk = qepy.klist.get_array_xk()[:, :self.get_number_of_k_points()].T
+        xk = qepy.klist.get_array_xk()[:, :cls.get_number_of_k_points()].T
         return xk @ qepy.cell_base.get_array_at()
 
-    def get_k_point_weights(self):
+    @classmethod
+    def get_k_point_weights(cls):
         """Weights of the k-points.
 
         The sum of all weights is one."""
-        return qepy.klist.get_array_wk()[:self.get_number_of_k_points()]
+        return qepy.klist.get_array_wk()[:cls.get_number_of_k_points()]
 
     def get_pseudo_density(self, spin=None, pad=True, gather = True):
         """Return pseudo-density array.
 
         If *spin* is not given, then the total density is returned.
         Otherwise, the spin up or down density is returned (spin=0 or
         1)."""
         density = self.get_density(gather = gather)
         if spin is None :
             return density.sum(axis=1)
         else :
             return density[:, spin]
 
-    def get_effective_potential(self, spin=0, pad=True):
-        """Return pseudo-effective-potential array."""
-        return qepy.scf.get_array_vrs()
-
-    def get_pseudo_wave_function(self, band=None, kpt=0, spin=0, broadcast=True,
+    @classmethod
+    def get_pseudo_wave_function(cls, band=None, kpt=0, spin=0, broadcast=True,
                                  pad=True):
         """Return pseudo-wave-function array."""
         qepy.qepy_mod.qepy_get_evc(kpt + 1)
         evc = qepy.wavefunctions.get_array_evc()
         if band is None :
             return evc
         else :
             return evc[:, band]
 
-    def get_eigenvalues(self, kpt=0, spin=0):
+    @classmethod
+    def get_eigenvalues(cls, kpt=0, spin=0):
         """Return eigenvalue array."""
         return qepy.wvfct.get_array_et()[:, kpt]
 
-    def get_occupation_numbers(self, kpt=0, spin=0):
+    @classmethod
+    def get_occupation_numbers(cls, kpt=0, spin=0):
         """Return occupation number array."""
         return qepy.wvfct.get_array_wg()[:, kpt]
 
-    def get_fermi_level(self):
+    @classmethod
+    def get_fermi_level(cls):
         """Return the Fermi level."""
         return qepy.ener.get_ef()
 
     # def initial_wannier(self, initialwannier, kpointgrid, fixedstates,
                         # edf, spin, nbands):
         # """Initial guess for the shape of wannier functions.
 
@@ -699,57 +820,128 @@
         # raise NotImplementedError
 
     # def get_wannier_localization_matrix(self, nbands, dirG, kpoint,
                                         # nextkpoint, G_I, spin):
         # """Calculate integrals for maximally localized Wannier functions."""
         # raise NotImplementedError
 
-    def get_magnetic_moment(self, **kwargs):
+    @classmethod
+    def get_magnetic_moment(cls, **kwargs):
         """Return the total magnetic moment."""
         return qepy.lsda_mod.get_magtot()
 
-    def get_number_of_grid_points(self, gather = True):
+    @classmethod
+    def get_number_of_grid_points(cls, gather = True):
         """Return the shape of arrays."""
         nr = np.zeros(3, dtype = 'int32')
         qepy.qepy_mod.qepy_get_grid(nr, gather)
         return nr
     #ASE DFTCalculator END
+#-----------------------------------------------------------------------
 
-    def get_volume(self):
+    @classmethod
+    def get_number_of_k_points(cls):
+        """Return the number of kpoints."""
+        return qepy.klist.get_nks()
+
+    @classmethod
+    def get_volume(cls):
         """Return the volume."""
         return qepy.cell_base.get_omega()
 
-    def get_ecutrho(self):
+    @classmethod
+    def get_ecutrho(cls):
         """Return the cutoff for density."""
         return qepy.gvect.get_ecutrho()
 
-    def data2field(self, data, cell = None, grid = None):
-        """QE data to dftpy DirectField, please call it in serial."""
+    @classmethod
+    def get_ions_lattice(cls):
+        """Return the lattice of ions."""
+        alat = qepy.cell_base.get_alat()
+        lattice = qepy.cell_base.get_array_at() * alat
+        return lattice.T
+
+    @classmethod
+    def get_ions_positions(cls):
+        """Return the cartesian positions of ions."""
+        alat = qepy.cell_base.get_alat()
+        pos = qepy.ions_base.get_array_tau().T * alat
+        return pos
+
+    @classmethod
+    def get_ions_symbols(cls):
+        """Return the symbols of ions."""
+        ityp = qepy.ions_base.get_array_ityp() - 1
+        nat = qepy.ions_base.get_nat()
+        ntyp = qepy.ions_base.get_nsp()
+        label = qepy.ions_base.get_array_atm().T.view('S3')[:,0].astype('U3')[:ntyp]
+        label = [x.strip() for x in label]
+        symbols = []
+        for i in range(nat):
+            symbols.append(label[ityp[i]])
+        return symbols
+
+    @classmethod
+    def data2field(cls, data, cell = None, grid = None, rank = None):
+        """QE data to dftpy DirectField.
+        If data is None or small temporary array will return np.zeros(1).
+        """
         from dftpy.field import DirectField
         from dftpy.grid import DirectGrid
         #
-        if cell is None : cell = self.get_ions_lattice()
-        if grid is None : grid = DirectGrid(lattice=cell, nr=self.get_number_of_grid_points(), ecut=self.get_ecutrho())
-        field = DirectField(grid=grid, data=data.ravel(order='C'), order='F', rank=self.get_number_of_spins())
+        if data is None or data.size < 8 : return np.zeros(1)
+        #
+        if cell is None : cell = cls.get_ions_lattice()
+        if grid is None : grid = DirectGrid(lattice=cell, nr=cls.get_number_of_grid_points(), ecut=cls.get_ecutrho())
+        if not rank :
+            rank = data.shape[1] if data.ndim == 2 else 1
+        #
+        if data.size != grid.nnrR*rank :
+            raise ValueError('The size of data not match the grid,\
+                    please check the data or set another grid', data.size, grid.nnrR*rank)
+        #
+        field = DirectField(grid=grid, data=data.ravel(order='C'), order='F', rank=rank)
         return field
 
-    def field2data(self, field, data = None):
-        """dftpy DirectField to QE data, please call it in serial."""
-        nspin = self.get_number_of_spins()
-        if data is None :
-            nnrR = np.prod(self.get_number_of_grid_points())
-            data = np.empty((nnrR, nspin))
+    @classmethod
+    def field2data(cls, field, data = None):
+        """dftpy DirectField to QE data.
+        If the input field is not 3d array, will return np.zeros((1, 1)).
+        """
+        #
+        if field is None or field.ndim < 3 : return np.zeros((1, 1))
         #
         ns = field.shape[0] if field.ndim == 4 else 1
+        if data is None :
+            nnrR = np.prod(cls.get_number_of_grid_points())
+            data = np.empty((nnrR, ns))
+        #
+        if data.size != field.size :
+            raise ValueError('The size of field is different with data,\
+                    please check the field or set another data', field.size, data.size)
+        #
         if ns == 1 : field = [field]
-        for i in range(nspin):
+        for i in range(ns):
             data[:, i] = field[i].ravel(order = 'F')
         return data
 
     @classmethod
+    def get_dftpy_grid(cls, nr = None, cell = None, mp = None, **kwargs):
+        """Return the dftpy DirectGrid from QE."""
+        from dftpy.grid import DirectGrid
+        if cell is None : cell = cls.get_ions_lattice()
+        if nr is None :
+            nr = cls.get_number_of_grid_points()
+            ecut = cls.get_ecutrho()
+        else :
+            ecut = None
+        grid = DirectGrid(lattice=cell, nr=nr, ecut=ecut, mp=mp, **kwargs)
+        return grid
+
+    @classmethod
     def get_ase_atoms(cls):
         """Return the atom.Atoms from QE."""
         from ase.atoms import Atoms
         units_Bohr = constants.BOHR_RADIUS_SI * 1E10
         #
         symbols = cls.get_ions_symbols()
         positions = cls.get_ions_positions() * units_Bohr
@@ -760,38 +952,43 @@
     @classmethod
     def get_dftpy_ions(cls):
         """Return the dftpy.Ions from QE."""
         from dftpy.ions import Ions
         atoms = cls.get_ase_atoms()
         return Ions.from_ase(atoms)
 
-    def set_density(self, density, gather = True, **kwargs):
+    @classmethod
+    def set_density(cls, density, gather = True, **kwargs):
         """Set density array in real space."""
         #
         if density is None : density = np.zeros((1, 1))
         if density.ndim != 2 : raise ValueError("The array should be 2-d.")
         #
         qepy.qepy_mod.qepy_set_rho(density, gather = gather)
 
-    @staticmethod
-    def switch_nlpp(nhm=0, nbetam=0, nkb=0, nh=None, **kwargs):
+    @classmethod
+    def switch_nlpp(cls, nhm=0, nbetam=0, nkb=0, nh=None, **kwargs):
         nhm_ = qepy.uspp_param.get_nhm()
         nbetam_ = qepy.uspp_param.get_nbetam()
         nh_ = qepy.uspp_param.get_array_nh().copy()
         nkb_ = qepy.uspp.get_nkb()
 
         if nh is None: nh = nh_ * 0
 
-        print('nnn', nhm, type(nhm))
         qepy.uspp_param.set_nhm(nhm)
         qepy.uspp_param.set_nbetam(nbetam)
         qepy.uspp.set_nkb(nkb)
         qepy.uspp_param.set_array_nh(nh)
 
         pp_options = {
             'nhm' : nhm_,
             'nbetam' : nbetam_,
             'nh': nh_,
             'nkb': nkb_,
         }
 
         return pp_options
+
+    @classmethod
+    def update_exchange_correlation(cls, xc=None, libxc=None, **kwargs):
+        if libxc : xc = None
+        qepy.qepy_mod.qepy_set_dft(xc)
```

### Comparing `qepy-0.0.2rc2/qepy.egg-info/PKG-INFO` & `qepy-0.0.3rc0/qepy.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qepy
-Version: 0.0.2rc2
+Version: 0.0.3rc0
 Summary: QEpy: Quantum ESPRESSO Python interface
 Home-page: https://gitlab.com/shaoxc/qepy
 Author: Pavanello Research Group
 Author-email: m.pavanello@rutgers.edu
 License: GPL
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
@@ -38,37 +38,38 @@
 ## Requirements
  - [Python](https://www.python.org/) (>=3.7)
  - [NumPy](https://docs.scipy.org/doc/numpy/reference/) (>=1.18.0)
  - [f90wrap](https://github.com/jameskermode/f90wrap) (>=0.2.8)
  - [Quantum ESPRESSO ](https://gitlab.com/QEF/q-e/-/releases/qe-6.5) (=6.5)
  - Compiler ([GNU](https://gcc.gnu.org/fortran/)(Recommended) or [Intel](https://software.intel.com/content/www/us/en/develop/tools/oneapi/components/fortran-compiler.html))
 
-## Install
+## Installation
+### Pip
+   Using pip can easy install the release version (serial) of QEpy from [PyPI](https://pypi.org/project/qepy).
+
+```shell
+python -m pip install qepy
+```
+
+### Source
+
  - **QE**
 
-	All static libraries should be compiled with the `-fPIC` compuiler option. Add `-fPIC` to the configuration options. E.g.,
+	All source codes should be compiled with the `-fPIC` compuiler option. Add `-fPIC` to the configuration options. E.g.,
 
      ```shell
 	 ./configure CFLAGS=-fPIC FFLAGS=-fPIC try_foxflags=-fPIC MPIF90=mpif90
+	  make pwall
+	  export qedir=`pwd`
      ```
 
-	Intel compiler:
-
-
-     ```shell
-	 ./configure CFLAGS=-fPIC FFLAGS=-fPIC try_foxflags=-fPIC MPIF90=mpiifort
-	 ```
-
-   + `make pw` or `make pwlibs`.
-
  - **QEpy**
 
      ```shell
 	 git clone --recurse-submodules https://gitlab.com/shaoxc/qepy.git
-     qedir=${QE} oldxml=yes ldau=yes tddft=yes python -m pip install -U ./qepy
+     oldxml=yes ldau=yes tddft=yes python -m pip install -U ./qepy
 	 ```
 
 ## Manual and Tutorials
-
   See [QEpy's website](http://qepy.rutgers.edu) for details.
```

### Comparing `qepy-0.0.2rc2/qepy.egg-info/SOURCES.txt` & `qepy-0.0.3rc0/qepy.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 .gitignore
 .gitlab-ci.yml
 .gitmodules
 README.md
 pyproject.toml
 setup.py
+.github/workflows/linux.yml
 .github/workflows/publish.yml
 .github/workflows/wheels.yml
 doc/Makefile
 doc/make.bat
 doc/source/QEpy.bib
 doc/source/conf.py
 doc/source/contact.rst
@@ -57,14 +58,19 @@
 examples/jupyter/ext/Al_ONCV_PBE-1.2.upf
 examples/jupyter/ext/dftpy_xc.ipynb
 examples/jupyter/ext/dirac_exchange.ipynb
 examples/jupyter/nvt/H_ONCV_PBE-1.2.upf
 examples/jupyter/nvt/O_ONCV_PBE-1.2.upf
 examples/jupyter/nvt/ase_nvt.ipynb
 examples/jupyter/nvt/qe_in.in
+examples/jupyter/pp/Al_ONCV_PBE-1.2.upf
+examples/jupyter/pp/pp.in
+examples/jupyter/pp/qepy_elf_rdg.ipynb
+examples/jupyter/pp/qepy_parse_output.ipynb
+examples/jupyter/pp/qepy_potentials.ipynb
 examples/jupyter/scf/Al.pbe-nl-kjpaw_psl.1.0.0.UPF
 examples/jupyter/scf/Al_ONCV_PBE-1.2.upf
 examples/jupyter/scf/dftpy_mixer.ipynb
 examples/jupyter/scf/qe_in.in
 examples/jupyter/scf/qepy_iterative.ipynb
 examples/jupyter/scf/qepy_qeinput.ipynb
 examples/jupyter/scf/qepy_scf.ipynb
@@ -147,43 +153,42 @@
 qepy.egg-info/SOURCES.txt
 qepy.egg-info/dependency_links.txt
 qepy.egg-info/not-zip-safe
 qepy.egg-info/requires.txt
 qepy.egg-info/top_level.txt
 src/api/qepy_common.f90
 src/api/qepy_mod.f90
-src/api/qepy_scatter_mod.f90
+src/fix/funct.f90
+src/fix/potinit.f90
+src/fix/pw_restart_new.f90
+src/fix/qes_read_module.f90
+src/fix/read_file_new.f90
+src/fix/scatter_mod.f90
+src/fix/wfcinit.f90
 src/ldau/qepy_econf.ini
 src/ldau/qepy_ldau_patch.py
 src/oldxml/oldxml_io_rho_xml.f90
 src/oldxml/oldxml_potinit.f90
 src/oldxml/oldxml_pw_restart.f90
 src/oldxml/oldxml_qexml.f90
 src/oldxml/oldxml_read_file.f90
 src/oldxml/oldxml_wfcinit.f90
 src/oldxml/oldxml_xml_io_base.f90
-src/qe/funct.f90
-src/qe/qepy_api.f90
 src/qe/qepy_electrons.f90
 src/qe/qepy_electrons_nscf.f90
 src/qe/qepy_forces.f90
 src/qe/qepy_hinit1.f90
 src/qe/qepy_init_run.f90
-src/qe/qepy_potinit.f90
 src/qe/qepy_pw2casino_write.f90
-src/qe/qepy_pw_restart_new.f90
 src/qe/qepy_pwscf.f90
-src/qe/qepy_read_file_new.f90
 src/qe/qepy_run_pwscf.f90
 src/qe/qepy_setlocal.f90
 src/qe/qepy_stop_run.f90
 src/qe/qepy_stress.f90
-src/qe/qepy_sum_band.f90
 src/qe/qepy_v_of_rho.f90
-src/qe/qepy_wfcinit.f90
 src/tddft/qepy_molecule_optical_absorption.f90
 src/tddft/qepy_tddft_common.f90
 src/tddft/qepy_tddft_main.f90
 src/tddft/qepy_tddft_mod.f90
 src/tddft/qepy_tddft_routines.f90
 src/tddft/qepy_tddft_setup.f90
 src/tddft/qepy_update_ham.f90
```

### Comparing `qepy-0.0.2rc2/setup.py` & `qepy-0.0.3rc0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -97,15 +97,15 @@
             res = subprocess.run(["./configure"] + qe_install_flags, cwd=qedir, env = env, check=False, capture_output=True)
             stderr=res.stderr.decode()
             if 'error' in stderr:
                 print('Some errors happened in configure...')
                 subprocess.run(["cat", "install/config.log"], cwd=qedir, env = env, check = False)
                 print(stderr)
                 exit()
-            subprocess.check_call(["make", "pwlibs"] + build_args, cwd=qedir, env = env)
+            subprocess.check_call(["make", "pwall"] + build_args, cwd=qedir, env = env)
             env['qedir'] = os.path.abspath(qedir)
 
         if env.get('tddft', 'no').lower() == 'yes' :
             subprocess.check_call(['make', '-f', 'Makefile.cetddft'] + build_args, cwd=self.build_temp, env = env)
 
         subprocess.check_call(['make', '-f', 'Makefile'] + build_args, cwd=self.build_temp, env = env)
```

### Comparing `qepy-0.0.2rc2/src/api/qepy_common.f90` & `qepy-0.0.3rc0/src/api/qepy_common.f90`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,28 @@
 MODULE qepy_common
-   USE kinds,                ONLY : DP
+   USE kinds,               ONLY : DP
+   !
+   USE fft_types,           ONLY : fft_type_descriptor
+   USE scf,                 ONLY : scf_type
+   !
    IMPLICIT NONE
    PRIVATE
    !
-   PUBLIC :: arr2pointer
+   PUBLIC :: arr2pointer, set_embed
+   !
+#if defined(__MPI)
+   logical, public :: is_mpi = .TRUE.
+#else
+   logical, public :: is_mpi = .FALSE.
+#endif
+#if defined(_OPENMP)
+   logical, public :: is_openmp = .TRUE.
+#else
+   logical, public :: is_openmp = .FALSE.
+#endif
    !
    type, public :: input_base
       INTEGER            :: my_world_comm = 0
       LOGICAL            :: start_images = .false.
       CHARACTER(len=256) :: filename = ''
       CHARACTER(len=256) :: code = 'QEPY'
       CHARACTER(len=256) :: tmp_dir = './'
@@ -67,51 +82,97 @@
    end type energies_base
    !
    type, public :: embed_base
       type(input_base)                :: input
       type(tddft_base)                :: tddft
       type(energies_base)             :: energies
       real(kind=dp), allocatable      :: extpot(:,:)
-      real(kind=dp)                   :: extene = 0.0
+      real(kind=dp)                   :: extene = 0.d0
       integer                         :: exttype = 0
       real(kind=dp), allocatable      :: extforces(:,:)
-      real(kind=dp)                   :: extstress(3,3)
+      real(kind=dp)                   :: extstress(3,3) = 0.d0
       logical                         :: initial = .true.
-      real(kind=dp)                   :: mix_coef = -1.0
+      real(kind=dp)                   :: mix_coef = -1.d0
       logical                         :: finish = .false.
-      real(kind=dp)                   :: etotal = 0.0
-      real(kind=dp)                   :: dnorm = 1.0
+      real(kind=dp)                   :: etotal = 0.d0
+      real(kind=dp)                   :: dnorm = 1.d0
       logical                         :: lewald = .true.
       logical                         :: nlpp = .true.
       real(kind=dp)                   :: diag_conv = 1.D-2
       logical                         :: ldescf = .false.
       !! add scf correction energy
       logical                         :: iterative = .false.
       !! add correction for variational energy
       logical                         :: lmovecell = .false.
       !! allow change the cell
       logical                         :: oldxml = .false.
       !! Olderversion QE (XML file name is 'data-file.xml')
+      !!
+      !!
+      type(fft_type_descriptor),pointer :: dfftp
+      type(fft_type_descriptor),pointer :: dffts
+      type(scf_type),pointer            :: rho
+      type(scf_type),pointer            :: v
+      type(scf_type),pointer            :: vnew
    CONTAINS
       !--------------------------------------------------------------------------------
       PROCEDURE :: allocate_extpot
       PROCEDURE :: allocate_extforces
       PROCEDURE :: free => free_embed
    end type embed_base
    !
    !
-   TYPE ( embed_base ), public :: messenger
+   TYPE ( embed_base ), public, pointer :: embed
+   TYPE ( embed_base ), public, target  :: messenger
    !
    !
    INTERFACE arr2pointer
       MODULE PROCEDURE arr2pointer_real_1, arr2pointer_real_2, arr2pointer_real_3, arr2pointer_real_4
    END INTERFACE
    !
 CONTAINS
    !
+   SUBROUTINE set_embed(obj)
+      !
+      USE fft_base,             ONLY : dfftp, dffts
+      USE scf,                  ONLY : rho, vnew, v
+      IMPLICIT NONE
+      TYPE(embed_base), INTENT(INOUT), TARGET :: obj
+      !
+      embed => obj
+      call set_target_dfft(obj, dfftp, dffts)
+      call set_target_scf(obj, rho, vnew, v)
+      !
+   END SUBROUTINE
+   !
+   SUBROUTINE set_target_dfft(obj, dfftp, dffts)
+      USE fft_types,           ONLY : fft_type_descriptor
+      !
+      IMPLICIT NONE
+      TYPE(fft_type_descriptor), INTENT(IN), TARGET :: dfftp, dffts
+      TYPE(embed_base), INTENT(INOUT) :: obj
+      !
+      obj%dfftp => dfftp
+      obj%dffts => dffts
+      !
+   END SUBROUTINE
+   !
+   SUBROUTINE set_target_scf(obj, rho, v, vnew)
+      USE scf,                 ONLY : scf_type
+      !
+      IMPLICIT NONE
+      TYPE(scf_type), INTENT(IN), TARGET :: rho, v, vnew
+      TYPE(embed_base), INTENT(INOUT) :: obj
+      !
+      obj%rho => rho
+      obj%v => v
+      obj%vnew => vnew
+      !
+   END SUBROUTINE
+   !
    SUBROUTINE free_embed(obj)
       !
       IMPLICIT NONE
       CLASS(embed_base), INTENT(INOUT) :: obj
       !
       IF (ALLOCATED(obj%extpot)) DEALLOCATE(obj%extpot)
       IF (ALLOCATED(obj%extforces)) DEALLOCATE(obj%extforces)
```

### Comparing `qepy-0.0.2rc2/src/api/qepy_mod.f90` & `qepy-0.0.3rc0/src/api/qepy_mod.f90`

 * *Files 27% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 MODULE qepy_mod
    USE kinds,                   ONLY : DP
-   USE qepy_scatter_mod,        ONLY : gather_grid, scatter_grid
-   USE qepy_common,             ONLY : embed_base, input_base
+   USE scatter_mod,             ONLY : gather_grid, scatter_grid
+   USE qepy_common,             ONLY : embed
    USE fft_base,                ONLY : dfftp
    !
    IMPLICIT NONE
    PUBLIC
    !
    INTERFACE mp_gather
       MODULE PROCEDURE mp_gather_real, mp_gather_complex
@@ -88,23 +88,26 @@
       IMPLICIT NONE
       real(DP), INTENT(IN)        :: fin(:)
       real(DP), INTENT(OUT)       :: fout(:)
       LOGICAL,INTENT(in),OPTIONAL :: gather
       LOGICAL,INTENT(in),OPTIONAL :: scatter
       !
       INTEGER                     :: nnr
-      LOGICAL                     :: gather_ = .FALSE.
-      LOGICAL                     :: scatter_ = .FALSE.
+      LOGICAL                     :: gather_
+      LOGICAL                     :: scatter_
+      !
+      gather_ = .FALSE.
+      scatter_ = .FALSE.
       !
       IF ( present(gather) ) gather_ = gather
       IF ( present(scatter) ) scatter_ = scatter
       !
-      IF ( gather ) THEN
+      IF ( gather_ ) THEN
          CALL mp_gather(fin, fout)
-      ELSE IF ( scatter ) THEN
+      ELSE IF ( scatter_ ) THEN
          CALL mp_scatter(fin, fout)
       ELSE
          !nnr = dfftp%nr1x* dfftp%my_nr2p* dfftp%my_nr3p
          nnr = size(fin)
          fout(1:nnr) = fin
          fout(nnr:size(fout)) = 0.0_DP
       ENDIF
@@ -117,16 +120,19 @@
       IMPLICIT NONE
       real(DP), INTENT(IN)        :: fin(:,:)
       real(DP), INTENT(OUT)       :: fout(:,:)
       LOGICAL,INTENT(in),OPTIONAL :: gather
       LOGICAL,INTENT(in),OPTIONAL :: scatter
       !
       INTEGER                     :: ispin, nspin
-      LOGICAL                     :: gather_ = .FALSE.
-      LOGICAL                     :: scatter_ = .FALSE.
+      LOGICAL                     :: gather_
+      LOGICAL                     :: scatter_
+      !
+      gather_ = .FALSE.
+      scatter_ = .FALSE.
       !
       IF ( present(gather) ) gather_ = gather
       IF ( present(scatter) ) scatter_ = scatter
       !
       nspin = size(fin, 2)
       DO ispin = 1, nspin
          call qepy_get_value_real_1(fin(:, ispin), fout(:, ispin), gather_, scatter_)
@@ -140,16 +146,17 @@
       USE fft_base,             ONLY : dfftp, dffts
       USE lsda_mod,             ONLY : lsda, nspin, current_spin, isk
       !
       IMPLICIT NONE
       REAL(DP), INTENT(OUT) :: rhor(:,:)
       LOGICAL,INTENT(in),OPTIONAL :: gather
       !
-      LOGICAL :: gather_ = .true.
+      LOGICAL :: gather_
       !
+      gather_ = .true.
       IF ( present(gather) ) gather_ = gather
       !
       IF (nspin > 1) CALL rhoz_or_updw( rho, 'only_r', '->updw' )
       !
       call qepy_get_value(rho%of_r, rhor, gather = gather_)
       !
       IF (nspin > 1) CALL rhoz_or_updw( rho, 'only_r', '->rhoz' )
@@ -162,16 +169,17 @@
       use scf,                  ONLY : rho, rhoz_or_updw
       USE lsda_mod,             ONLY : lsda, nspin, current_spin, isk
       !
       IMPLICIT NONE
       REAL(DP), INTENT(IN) :: rhor(:,:)
       LOGICAL,INTENT(in),OPTIONAL :: gather
       !
-      LOGICAL :: gather_ = .true.
+      LOGICAL :: gather_
       !
+      gather_ = .true.
       IF ( present(gather) ) gather_ = gather
       !
       IF (nspin > 1) CALL rhoz_or_updw( rho, 'only_r', '->updw' )
       !
       call qepy_get_value(rhor, rho%of_r, scatter = gather_)
       !
       IF (nspin > 1) CALL rhoz_or_updw( rho, 'only_r', '->rhoz' )
@@ -182,53 +190,55 @@
       USE kinds,                ONLY : DP
       use scf,                  ONLY : rho_core !! the core charge in real space
       USE fft_base,             ONLY : dfftp, dffts
       IMPLICIT NONE
       REAL(DP), INTENT(OUT) :: rhoc(:)
       LOGICAL,INTENT(in),OPTIONAL :: gather
       !
-      LOGICAL :: gather_ = .true.
+      LOGICAL :: gather_
       !
+      gather_ = .true.
       IF ( present(gather) ) gather_ = gather
       !
       call qepy_get_value(rho_core, rhoc, gather = gather_)
       !
    END SUBROUTINE
 
    SUBROUTINE qepy_set_rho_core(rhoc, gather)
       USE kinds,                ONLY : DP
       use scf,                  ONLY : rho_core !! the core charge in real space
       USE fft_base,             ONLY : dfftp, dffts
       IMPLICIT NONE
       REAL(DP), INTENT(IN) :: rhoc(:)
       LOGICAL,INTENT(in),OPTIONAL :: gather
       !
-      LOGICAL :: gather_ = .true.
+      LOGICAL :: gather_
       !
+      gather_ = .true.
       IF ( present(gather) ) gather_ = gather
       !
       call qepy_get_value(rhoc, rho_core, scatter = gather_)
       !
    END SUBROUTINE
 
-   SUBROUTINE qepy_set_extpot(embed, vin, gather)
+   SUBROUTINE qepy_set_extpot(vin, gather)
       USE kinds,                ONLY : DP
       USE fft_rho,              ONLY : rho_g2r, rho_r2g
       USE fft_base,             ONLY : dfftp, dffts
       USE lsda_mod,             ONLY : lsda, nspin, current_spin, isk
       USE mp,                   ONLY : mp_bcast
       !
       IMPLICIT NONE
-      TYPE(embed_base), INTENT(INOUT) :: embed
       REAL(DP), INTENT(IN) :: vin(:,:)
       LOGICAL,INTENT(in),OPTIONAL :: gather
       !
       INTEGER :: ispin, ns
-      LOGICAL :: gather_ = .true.
+      LOGICAL :: gather_
       !
+      gather_ = .true.
       IF ( present(gather) ) gather_ = gather
       !
       call embed%allocate_extpot()
       !
       ns = size(vin,2)
       CALL mp_bcast(ns, dfftp%root, dfftp%comm)
       !
@@ -263,17 +273,18 @@
       USE kinds,                ONLY : DP
       USE fft_types,            ONLY : fft_type_descriptor
       !
       IMPLICIT NONE
       TYPE(fft_type_descriptor),INTENT(IN) :: dfft
       LOGICAL,INTENT(in),OPTIONAL          :: gather
       !
-      LOGICAL                              :: gather_ = .true.
+      LOGICAL                              :: gather_
       INTEGER                              :: nrw(3)
       !
+      gather_ = .true.
       IF ( present(gather) ) gather_ = gather
       !
       IF ( gather_ ) THEN
          nrw =(/dfft%nr1, dfft%nr2, dfft%nr3/)
       ELSE
          nrw =(/dfft%nr1x, dfft%my_nr2p, dfft%my_nr3p/)
       ENDIF
@@ -376,37 +387,38 @@
       !
       IMPLICIT NONE
       INTEGER,INTENT(IN) :: ik, ibnd
       COMPLEX(DP), INTENT(OUT) :: wf(:)
       LOGICAL,INTENT(in),OPTIONAL :: gather
       !
       INTEGER :: j, nnr, npw
-      LOGICAL :: gather_ = .true.
+      LOGICAL :: gather_
       !
+      gather_ = .true.
       IF ( present(gather) ) gather_ = gather
       !
       IF ( dffts%has_task_groups ) THEN
          call errore('qepy_get_wf', 'Sorry this one not support task-group version', 1)
       ENDIF
       !
       IF ( nks > 1 .OR. lelfield ) CALL get_buffer ( evc, nwordwfc, iunwfc, ik )
-      !$omp parallel
       psic(:) = (0.0_DP, 0.0_DP)
       npw = ngk(ik)
-      !$omp do
       IF ( gamma_only ) THEN
          psic(dffts%nl (1:npw))  = evc(1:npw,ibnd)
          psic(dffts%nlm(1:npw)) = CONJG( evc(1:npw,ibnd) )
       ELSE
+         !$omp parallel
+         !$omp do
          DO j = 1, npw
             psic(dffts%nl(igk_k(j,ik))) = evc(j,ibnd)
          ENDDO
+         !$omp end do nowait
+         !$omp end parallel
       END IF
-      !$omp end do nowait
-      !$omp end parallel
       CALL invfft ('Wave', psic, dffts)
       !
       IF ( gather_ ) THEN
          CALL mp_gather(psic(1:dffts%nnr), wf)
       ELSE
          nnr = min(size(wf), dffts%nnr)
          wf(1:nnr) = psic(1:nnr)
@@ -427,108 +439,108 @@
       !
       IMPLICIT NONE
       INTEGER,INTENT(IN) :: ik
       COMPLEX(DP), INTENT(OUT) :: vk(:,:)
       LOGICAL,INTENT(in),OPTIONAL :: gather
       !
       INTEGER :: i, j, nnr, npw
-      LOGICAL :: gather_ = .true.
+      LOGICAL :: gather_
       !
+      gather_ = .true.
       IF ( present(gather) ) gather_ = gather
       !
       IF ( dffts%has_task_groups ) THEN
          call errore('qepy_get_vkb', 'Sorry this one not support task-group version', 1)
       ENDIF
       !
       IF ( nkb > 0 ) CALL init_us_2( ngk(ik), igk_k(1,ik), xk(1,ik), vkb )
       !
       vk(:,:) = (0.0_DP, 0.0_DP)
       DO i = 1, nkb
-         !$omp parallel
          psic(:) = (0.0_DP, 0.0_DP)
          npw = ngk(ik)
-         !$omp do
          IF ( gamma_only ) THEN
             psic(dffts%nl (1:npw))  = vkb(1:npw,i)
             psic(dffts%nlm(1:npw)) = CONJG( vkb(1:npw,i) )
          ELSE
+            !$omp parallel
+            !$omp do
             DO j = 1, npw
                psic(dffts%nl(igk_k(j,ik))) = vkb(j,i)
             ENDDO
+            !$omp end do nowait
+            !$omp end parallel
          END IF
-         !$omp end do nowait
-         !$omp end parallel
          CALL invfft ('Wave', psic, dffts)
          !
          IF ( gather_ ) THEN
             CALL mp_gather(psic(1:dffts%nnr), vk(:, i))
          ELSE
             nnr = min(size(vk, 1), dffts%nnr)
             vk(1:nnr, i) = psic(1:nnr)
          ENDIF
       ENDDO
    END SUBROUTINE
 
-   SUBROUTINE qepy_set_extforces(embed, forces)
+   SUBROUTINE qepy_set_extforces(forces)
       USE kinds,                ONLY : DP
       USE ions_base,            ONLY : nat, ntyp => nsp
       !
       IMPLICIT NONE
-      TYPE(embed_base), INTENT(INOUT) :: embed
       REAL(DP), INTENT(IN) :: forces(:,:)
       !
       call embed%allocate_extforces()
       embed%extforces(:,:) = forces(:,1:nat)
       !
    END SUBROUTINE
 
-   SUBROUTINE qepy_calc_effective_potential(embed, potential, gather)
+   SUBROUTINE qepy_calc_effective_potential(potential, gather)
       USE kinds,                ONLY : DP
       USE ions_base,            ONLY : nat, ntyp => nsp
       USE scf,                  ONLY : rho, rho_core, rhog_core, v, vltot, vrs
       USE ener,                 ONLY : etot, hwf_energy, eband, deband, ehart, &
                                        vtxc, etxc, etxcc, ewld, demet, epaw, &
                                        elondon, edftd3, ef_up, ef_dw
       USE ldaU,                 ONLY : eth
       USE extfield,             ONLY : tefield, etotefield
       USE lsda_mod,             ONLY : nspin
       !
       IMPLICIT NONE
-      TYPE(embed_base), INTENT(INOUT) :: embed
       REAL(DP), INTENT(OUT),OPTIONAL  :: potential(:,:)
       LOGICAL,INTENT(in),OPTIONAL     :: gather
       !
       REAL(DP) :: charge
       !
-      LOGICAL :: gather_ = .true.
+      LOGICAL :: gather_
       !
+      gather_ = .true.
       IF ( present(gather) ) gather_ = gather
       !
       CALL qepy_v_of_rho_all( rho, rho_core, rhog_core, &
-         ehart, etxc, vtxc, eth, etotefield, charge, v, embed)
+         ehart, etxc, vtxc, eth, etotefield, charge, v)
       !
       IF ( present(potential) ) THEN
          call qepy_get_value(vrs, potential, gather = gather_)
       ENDIF
       !
    END SUBROUTINE
 
-   SUBROUTINE qepy_set_effective_potential(embed, potential, gather)
+   SUBROUTINE qepy_set_effective_potential(potential, gather)
       USE kinds,                ONLY : DP
       USE scf,                  ONLY : kedtau, v, vltot, vrs
       USE lsda_mod,             ONLY : nspin
       USE gvecs,                ONLY : doublegrid
       !
       IMPLICIT NONE
-      TYPE(embed_base), INTENT(INOUT) :: embed
       REAL(DP),INTENT(IN)             :: potential(:,:)
       LOGICAL,INTENT(in),OPTIONAL     :: gather
       !
-      LOGICAL :: gather_ = .true.
+      LOGICAL :: gather_
       !
+      gather_ = .true.
       IF ( present(gather) ) gather_ = gather
       !
       call qepy_get_value(potential, vrs, gather = gather_)
       !
       CALL interpolate_vrs( dfftp%nnr, nspin, doublegrid, kedtau, v%kin_r, vrs )
       !
    END SUBROUTINE
@@ -571,8 +583,236 @@
       IF ( lelfield ) THEN
          CALL c_bands_efield( it )
       ELSE
          CALL c_bands( it )
       ENDIF
    END SUBROUTINE
 
+   SUBROUTINE qepy_update_ions(pos, ikind, lattice)
+      !-----------------------------------------------------------------------
+      ! This is function Combined 'run_pwscf' and 'move_ions'.
+      !***********************************************************************
+      ! pos:
+      !   ionic positions in bohr
+      ! ikind:
+      !   ikind = 0  all
+      !   ikind = 1  atomic configuration dependent information
+      ! lattice:
+      !   lattice parameter in bohr
+      !***********************************************************************
+      !-----------------------------------------------------------------------
+      USE mp_images,            ONLY : intra_image_comm
+      USE extrapolation,        ONLY : update_file, update_pot
+      USE io_global,            ONLY : ionode_id, ionode
+      USE ions_base,            ONLY : nat, ityp, tau
+      USE symm_base,            ONLY : checkallsym
+      USE mp,                   ONLY : mp_bcast
+      USE control_flags,        ONLY : treinit_gvecs
+      USE cell_base,            ONLY : alat, at, bg, omega, cell_force, &
+                                     fix_volume, fix_area, ibrav, enforce_ibrav
+      USE cellmd,               ONLY : omega_old, at_old, press, lmovecell, calc, cell_factor
+      !
+      !
+      INTEGER                  :: ierr
+      REAL(DP), INTENT(IN) :: pos(:,:)
+      INTEGER,INTENT(IN),OPTIONAL  :: ikind
+      REAL(DP), INTENT(IN), OPTIONAL  :: lattice(3,3)
+      !
+      INTEGER   :: iflag
+      LOGICAL :: lmovecell_
+      !
+      IF ( present(ikind) ) THEN
+         iflag = ikind
+      ELSE
+         iflag = 0
+      ENDIF
+      !
+      IF ( present(lattice) ) THEN
+         IF (.not. lmovecell) THEN
+            call errore("qepy_update_ions","lattice update only works for calculation= 'vc-relax' and 'vc-md'.",1)
+            ! This is due to the `gshells` function in the initialization will set `ngl`, which is one of the shape of `vloc`.
+         ENDIF
+         lmovecell_ = .TRUE.
+      ELSE
+         lmovecell_ = .FALSE.
+      ENDIF
+
+      CALL update_file()
+
+      IF ( ionode ) THEN
+         tau(:,:)=pos(:,:) / alat
+         IF ( lmovecell_ ) THEN
+            !
+            IF (ALLOCATED(embed%extpot)) DEALLOCATE(embed%extpot)
+            !
+            at_old = at
+            omega_old = omega
+            IF (fix_volume) CALL impose_deviatoric_strain( alat*at, lattice )
+            IF (fix_area)   CALL impose_deviatoric_strain_2d( alat*at, lattice )
+            at = lattice / alat
+            IF(enforce_ibrav) CALL remake_cell( ibrav, alat, at(1,1),at(1,2),at(1,3) )
+            CALL recips( at(1,1),at(1,2),at(1,3), bg(1,1),bg(1,2),bg(1,3) )
+            CALL volume( alat, at(1,1),at(1,2),at(1,3), omega )
+            !
+         ENDIF
+         CALL checkallsym( nat, tau, ityp)
+      ENDIF
+      !
+      CALL mp_bcast( tau, ionode_id, intra_image_comm )
+      !
+      IF ( lmovecell_ ) THEN
+         !
+         CALL mp_bcast( at,        ionode_id, intra_image_comm )
+         CALL mp_bcast( at_old,    ionode_id, intra_image_comm )
+         CALL mp_bcast( omega,     ionode_id, intra_image_comm )
+         CALL mp_bcast( omega_old, ionode_id, intra_image_comm )
+         CALL mp_bcast( bg,        ionode_id, intra_image_comm )
+         !
+      ENDIF
+      IF (iflag == 0 ) THEN
+         CALL punch( 'config-nowf' )
+         IF ( treinit_gvecs ) THEN
+            CALL reset_gvectors()
+         ELSE
+            CALL update_pot()
+            CALL hinit1()
+         END IF
+      ELSE IF (iflag == 1 ) THEN
+         CALL set_rhoc()
+         CALL hinit1()
+      END IF
+   END SUBROUTINE
+
+   SUBROUTINE qepy_restart_from_xml()
+      USE symm_base,            ONLY : irt
+      USE force_mod,            ONLY : force
+      USE ions_base,            ONLY : extfor
+      USE extfield,             ONLY : forcefield, forcegate
+      USE pw_restart_new,       ONLY : read_xml_file
+      !
+      LOGICAL              :: wfc_is_collected
+      !
+      IF (ALLOCATED(irt)) DEALLOCATE(irt)
+      IF (ALLOCATED(force)) DEALLOCATE(force)
+      IF (ALLOCATED(extfor)) DEALLOCATE(extfor)
+      IF (ALLOCATED(forcefield)) DEALLOCATE(forcefield)
+      IF (ALLOCATED(forcegate)) DEALLOCATE(forcegate)
+      !
+      CALL read_xml_file(wfc_is_collected)
+      !
+   END SUBROUTINE
+
+   SUBROUTINE qepy_sum_band(occupations)
+      USE fixed_occ,            ONLY : tfixed_occ, f_inp
+      !
+      REAL(DP),INTENT(in),OPTIONAL :: occupations(:,:)
+      !
+      IF ( present(occupations) ) THEN
+         IF (ALLOCATED(f_inp)) DEALLOCATE(f_inp)
+         ALLOCATE(f_inp(size(occupations,1), size(occupations,2)))
+         f_inp(:,:) = occupations(:,:)
+         tfixed_occ = .TRUE.
+      ELSE
+         tfixed_occ = .FALSE.
+         IF (ALLOCATED(f_inp)) DEALLOCATE(f_inp)
+      ENDIF
+      !
+      CALL sum_band()
+      !
+   END SUBROUTINE
+
+   SUBROUTINE qepy_get_tau(tau, gather)
+      USE kinds,                ONLY : DP
+      use scf,                  ONLY : rho
+      USE wavefunctions,        ONLY : psic
+      USE fft_base,                ONLY : dfftp
+      USE lsda_mod,             ONLY : nspin
+      USE fft_interfaces,       ONLY : invfft
+      USE control_flags,        ONLY : diago_full_acc, gamma_only, lxdm, tqr
+      !
+      IMPLICIT NONE
+      REAL(DP), INTENT(OUT) :: tau(:,:)
+      LOGICAL,INTENT(in),OPTIONAL :: gather
+      !
+      LOGICAL :: gather_
+      INTEGER :: is
+      !
+      gather_ = .true.
+      IF ( present(gather) ) gather_ = gather
+      !
+      !DO is = 1, nspin
+         !psic(:) = ( 0.D0, 0.D0 )
+         !psic(dfftp%nl(:)) = rho%kin_g(:,is)
+         !IF ( gamma_only ) psic(dfftp%nlm(:)) = CONJG( rho%kin_g(:,is) )
+         !CALL invfft ('Rho', psic, dfftp)
+         !rho%kin_r(:,is) = psic(:)
+      !END DO
+      !
+      call qepy_get_value(rho%kin_r, tau, gather = gather_)
+   END SUBROUTINE
+
+   SUBROUTINE qepy_open_files(io_level)
+      USE kinds,                ONLY : DP
+      USE io_files,             ONLY : nwordwfc, iunwfc
+      USE control_flags,        ONLY : io_level_ => io_level
+      USE buffers,              ONLY : open_buffer
+      !
+      IMPLICIT NONE
+      INTEGER,INTENT(in),OPTIONAL :: io_level
+      !
+      INTEGER                     :: level
+      LOGICAL :: exst_mem, exst_file, opnd
+      !
+      IF ( present(io_level) ) THEN
+         level = io_level
+      ELSE
+         level = io_level_
+      ENDIF
+      !
+      INQUIRE( UNIT = iunwfc, OPENED = opnd )
+      IF ( .not. opnd ) CALL open_buffer( iunwfc, 'wfc', nwordwfc, level, exst_mem, exst_file )
+      !
+   END SUBROUTINE
+
+   SUBROUTINE qepy_set_dft(dft)
+      USE kinds,                ONLY : DP
+      USE funct,                ONLY : dft_is_meta, enforce_input_dft
+      USE fft_base,             ONLY : dffts
+      USE lsda_mod,             ONLY : nspin
+      USE gvect,                ONLY : ngm
+      USE scf,                  ONLY : rho, vnew, v, kedtau
+      !
+      IMPLICIT NONE
+      CHARACTER(LEN=*),INTENT(IN),OPTIONAL  :: dft
+      !
+      LOGICAL :: is_meta
+      !
+      is_meta = dft_is_meta()
+      IF ( present(dft) ) THEN
+         call enforce_input_dft(dft)
+      ELSE
+         call enforce_input_dft('M06L')
+      ENDIF
+      !
+      IF ( dft_is_meta() .and. (.not. is_meta) ) THEN
+         IF (ALLOCATED(kedtau)) DEALLOCATE(kedtau)
+         ALLOCATE( kedtau(dffts%nnr,nspin) )
+         !
+         IF (ALLOCATED(rho%kin_r)) DEALLOCATE(rho%kin_r)
+         IF (ALLOCATED(rho%kin_g)) DEALLOCATE(rho%kin_g)
+         ALLOCATE( rho%kin_r(dfftp%nnr,nspin) )
+         ALLOCATE( rho%kin_g(ngm,nspin) )
+         !
+         IF (ALLOCATED(v%kin_r)) DEALLOCATE(v%kin_r)
+         IF (ALLOCATED(v%kin_g)) DEALLOCATE(v%kin_g)
+         ALLOCATE( v%kin_r(dfftp%nnr,nspin) )
+         ALLOCATE( v%kin_g(ngm,nspin) )
+         !
+         IF (ALLOCATED(vnew%kin_r)) DEALLOCATE(vnew%kin_r)
+         IF (ALLOCATED(vnew%kin_g)) DEALLOCATE(vnew%kin_g)
+         ALLOCATE( vnew%kin_r(dfftp%nnr,nspin) )
+         ALLOCATE( vnew%kin_g(ngm,nspin) )
+      ENDIF
+      !
+   END SUBROUTINE
+
 END MODULE qepy_mod
```

### Comparing `qepy-0.0.2rc2/src/api/qepy_scatter_mod.f90` & `qepy-0.0.3rc0/src/fix/scatter_mod.f90`

 * *Files 2% similar despite different names*

```diff
@@ -9,20 +9,22 @@
 !----------------------------------------------------------------------
 ! FFT base Module.
 ! Written by Carlo Cavazzoni, modified by Paolo Giannozzi
 ! Rewritten by Stefano de Gironcoli
 !----------------------------------------------------------------------
 !
 !=----------------------------------------------------------------------=!
-   MODULE qepy_scatter_mod
+   MODULE scatter_mod
 !=----------------------------------------------------------------------=!
 
         USE fft_types, ONLY: fft_type_descriptor
         USE fft_param
+        !qepy fix --> import 
         USE mp,                   ONLY : mp_bcast
+        !qepy fix <-- import 
 
         IMPLICIT NONE
 
         INTERFACE gather_grid
            MODULE PROCEDURE gather_real_grid, gather_complex_grid
         END INTERFACE
 
@@ -715,15 +717,17 @@
   !write (6,*) 'gather grid ok 4'
   CALL fftx_error__( ' gather_real_grid', 'info<>0', info )
   !
   ! ... the following check should be performed only on processor dfft%root
   ! ... otherwise f_out must be allocated on all processors even if not used
   !
   info = size( f_out ) - displs( dfft%nproc3-1 ) - recvcount( dfft%nproc3-1 )
+  !qepy --> only check root processor
   CALL mp_bcast( info, dfft%root, dfft%comm)
+  !qepy <-- only check root processor
   IF( info < 0 ) &
      CALL fftx_error__( ' gather_real_grid ', ' f_out too small ', -info )
   !
   DEALLOCATE ( f_aux )
   !
   CALL stop_clock( 'rgather_grid' )
   !
@@ -794,15 +798,17 @@
   !
   ! ... the following check should be performed only on processor dfft%root
   ! ... otherwise f_out must be allocated on all processors even if not used
   !
   !write (*,*) 'gcgather_grid 2*size(f_out)',2*size(f_out) ; FLUSH(6)
   !write (*,*) 'gcgather_grid displ+recv',dfft%nproc3, displs(dfft%nproc3-1) + recvcount(dfft%nproc3-1); FLUSH(6)
   info = 2*size( f_out ) - displs( dfft%nproc3 - 1 ) - recvcount( dfft%nproc3-1 ) ; FLUSH(6)
+  !qepy --> only check root processor
   CALL mp_bcast( info, dfft%root, dfft%comm)
+  !qepy <-- only check root processor
   IF( info < 0 ) CALL fftx_error__( ' gather_complex_grid ', ' f_out too small ', -info )
 
   info = 0
   !write (6,*) 'gather grid ok 3'
   CALL MPI_GATHERV( f_aux, recvcount(dfft%mype3), MPI_DOUBLE_PRECISION, &
                     f_out, recvcount, displs, MPI_DOUBLE_PRECISION, dfft%root,      &
                     dfft%comm3, info )
@@ -852,15 +858,17 @@
   ! 1) scatter within the comm3 communicator 
   displs = 0
   DO proc = 0, ( dfft%nproc3 - 1 )
      sendcount(proc) = dfft%nr1x * dfft%nr2x * dfft%nr3p(proc+1) 
      if (proc > 0) displs(proc) = displs(proc-1) + sendcount(proc-1)
   ENDDO
   info = size( f_in ) - displs( dfft%nproc3 - 1 ) - sendcount( dfft%nproc3 - 1 )
+  !qepy --> only check root processor
   CALL mp_bcast( info, dfft%root, dfft%comm)
+  !qepy <-- only check root processor
   IF( info < 0 ) CALL fftx_error__( ' scatter_real_grid ', ' f_in too small ', -info )
   info = 0
   !write (6,*) 'scatter grid ok 1'
   CALL MPI_SCATTERV( f_in, sendcount, displs, MPI_DOUBLE_PRECISION,   &
                      f_aux, sendcount(dfft%mype3), MPI_DOUBLE_PRECISION, &
                      dfft%root, dfft%comm3, info )
   !write (6,*) 'scatter grid ok 2'
@@ -932,15 +940,17 @@
      sendcount(proc) = 2 * dfft%nr1x * dfft%nr2x * dfft%nr3p(proc+1) 
      if (proc > 0) displs(proc) = displs(proc-1) + sendcount(proc-1)
   ENDDO
   !
   !write(*,*) 'cscatter_grid 2*size(f_in) ', 2*size(f_in); FLUSH(6)
   !write(*,*) 'cscatter_grid displ+send ', dfft%nproc3, displs(dfft%nproc3-1) + sendcount(dfft%nproc3-1); FLUSH(6)
   info = 2*size( f_in ) - displs( dfft%nproc3 - 1 ) - sendcount( dfft%nproc3 - 1 )
+  !qepy --> only check root processor
   CALL mp_bcast( info, dfft%root, dfft%comm)
+  !qepy <-- only check root processor
   IF( info < 0 ) &
      CALL fftx_error__( ' scatter_complex_grid ', ' f_in too small ', -info )
   !
   info = 0
   !write (6,*) 'scatter grid ok 1'
   CALL MPI_SCATTERV( f_in, sendcount, displs, MPI_DOUBLE_PRECISION,   &
                      f_aux, sendcount(dfft%mype3), MPI_DOUBLE_PRECISION, &
@@ -1285,91 +1295,91 @@
   !
   RETURN
   !
 END SUBROUTINE cscatter_sym_many
 
 
 !=----------------------------------------------------------------------=!
-   END MODULE qepy_scatter_mod
+   END MODULE scatter_mod
 !=----------------------------------------------------------------------=!
 !
 !
 !---------------------------------------------------------------------
-!subroutine fftsort (n, ia)  
-  !!---------------------------------------------------------------------
-  !! sort an integer array ia(1:n) into ascending order using heapsort algorithm.
-  !! n is input, ia is replaced on output by its sorted rearrangement.
-  !! create an index table (ind) by making an exchange in the index array
-  !! whenever an exchange is made on the sorted data array (ia).
-  !! in case of equal values in the data array (ia) the values in the
-  !! index array (ind) are used to order the entries.
-  !! if on input ind(1)  = 0 then indices are initialized in the routine,
-  !! if on input ind(1) != 0 then indices are assumed to have been
-  !!                initialized before entering the routine and these
-  !!                indices are carried around during the sorting process
-  !!
-  !! no work space needed !
-  !! free us from machine-dependent sorting-routines !
-  !!
-  !! adapted from Numerical Recipes pg. 329 (new edition)
-  !!
-  !implicit none  
-  !!-input/output variables
-  !integer :: n  
-  !integer :: ia (2,n)  
-  !!-local variables
-  !integer :: i, ir, j, l
-  !integer :: iia(2)  
-  !! nothing to order
-  !if (n.lt.2) return  
-  !! initialize indices for hiring and retirement-promotion phase
-  !l = n / 2 + 1  
-  !ir = n  
-!10 continue  
-  !! still in hiring phase
-  !if (l.gt.1) then  
-     !l = l - 1  
-     !iia(:) = ia (:,l)  
-     !! in retirement-promotion phase.
-  !else  
-     !! clear a space at the end of the array
-     !iia(:) = ia (:,ir)  
-     !!
-     !! retire the top of the heap into it
-     !ia (:,ir) = ia (:,1)  
-     !!
-     !! decrease the size of the corporation
-     !ir = ir - 1  
-     !! done with the last promotion
-     !if (ir.eq.1) then  
-        !! the least competent worker at all !
-        !ia (:,1) = iia(:)  
-        !!
-        !return  
-     !endif
-  !endif
-  !! wheter in hiring or promotion phase, we
-  !i = l  
-  !! set up to place iia in its proper level
-  !j = l + l  
-  !!
-  !do while (j.le.ir)  
-     !if (j.lt.ir) then  
-        !if (ia (1,j) .lt. ia (1,j + 1) ) then  
-           !j = j + 1  
-        !endif
-     !endif
-     !! demote iia
-     !if (iia(1).lt.ia (1,j) ) then  
-        !ia (:,i) = ia (:,j)  
-        !i = j  
-        !j = j + j  
-     !else  
-        !! set j to terminate do-while loop
-        !j = ir + 1  
-     !endif
-  !enddo
-  !ia (:,i) = iia(:)  
-  !goto 10  
-  !!
-!end subroutine fftsort
+subroutine fftsort (n, ia)  
+  !---------------------------------------------------------------------
+  ! sort an integer array ia(1:n) into ascending order using heapsort algorithm.
+  ! n is input, ia is replaced on output by its sorted rearrangement.
+  ! create an index table (ind) by making an exchange in the index array
+  ! whenever an exchange is made on the sorted data array (ia).
+  ! in case of equal values in the data array (ia) the values in the
+  ! index array (ind) are used to order the entries.
+  ! if on input ind(1)  = 0 then indices are initialized in the routine,
+  ! if on input ind(1) != 0 then indices are assumed to have been
+  !                initialized before entering the routine and these
+  !                indices are carried around during the sorting process
+  !
+  ! no work space needed !
+  ! free us from machine-dependent sorting-routines !
+  !
+  ! adapted from Numerical Recipes pg. 329 (new edition)
+  !
+  implicit none  
+  !-input/output variables
+  integer :: n  
+  integer :: ia (2,n)  
+  !-local variables
+  integer :: i, ir, j, l
+  integer :: iia(2)  
+  ! nothing to order
+  if (n.lt.2) return  
+  ! initialize indices for hiring and retirement-promotion phase
+  l = n / 2 + 1  
+  ir = n  
+10 continue  
+  ! still in hiring phase
+  if (l.gt.1) then  
+     l = l - 1  
+     iia(:) = ia (:,l)  
+     ! in retirement-promotion phase.
+  else  
+     ! clear a space at the end of the array
+     iia(:) = ia (:,ir)  
+     !
+     ! retire the top of the heap into it
+     ia (:,ir) = ia (:,1)  
+     !
+     ! decrease the size of the corporation
+     ir = ir - 1  
+     ! done with the last promotion
+     if (ir.eq.1) then  
+        ! the least competent worker at all !
+        ia (:,1) = iia(:)  
+        !
+        return  
+     endif
+  endif
+  ! wheter in hiring or promotion phase, we
+  i = l  
+  ! set up to place iia in its proper level
+  j = l + l  
+  !
+  do while (j.le.ir)  
+     if (j.lt.ir) then  
+        if (ia (1,j) .lt. ia (1,j + 1) ) then  
+           j = j + 1  
+        endif
+     endif
+     ! demote iia
+     if (iia(1).lt.ia (1,j) ) then  
+        ia (:,i) = ia (:,j)  
+        i = j  
+        j = j + j  
+     else  
+        ! set j to terminate do-while loop
+        j = ir + 1  
+     endif
+  enddo
+  ia (:,i) = iia(:)  
+  goto 10  
+  !
+end subroutine fftsort
```

### Comparing `qepy-0.0.2rc2/src/ldau/qepy_econf.ini` & `qepy-0.0.3rc0/src/ldau/qepy_econf.ini`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/src/ldau/qepy_ldau_patch.py` & `qepy-0.0.3rc0/src/ldau/qepy_ldau_patch.py`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/src/oldxml/oldxml_io_rho_xml.f90` & `qepy-0.0.3rc0/src/oldxml/oldxml_io_rho_xml.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/src/oldxml/oldxml_potinit.f90` & `qepy-0.0.3rc0/src/oldxml/oldxml_potinit.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/src/oldxml/oldxml_pw_restart.f90` & `qepy-0.0.3rc0/src/oldxml/oldxml_pw_restart.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/src/oldxml/oldxml_qexml.f90` & `qepy-0.0.3rc0/src/oldxml/oldxml_qexml.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/src/oldxml/oldxml_read_file.f90` & `qepy-0.0.3rc0/src/oldxml/oldxml_read_file.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/src/oldxml/oldxml_wfcinit.f90` & `qepy-0.0.3rc0/src/oldxml/oldxml_wfcinit.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/src/oldxml/oldxml_xml_io_base.f90` & `qepy-0.0.3rc0/src/oldxml/oldxml_xml_io_base.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/src/qe/funct.f90` & `qepy-0.0.3rc0/src/fix/funct.f90`

 * *Files 0% similar despite different names*

```diff
@@ -1102,18 +1102,25 @@
     !! \(\textrm{set_dft_from_name}\) to return without changing them.
     !
     IMPLICIT NONE
     !
     CHARACTER(LEN=*), INTENT(IN) :: dft_
     LOGICAL, INTENT(IN), OPTIONAL :: nomsg
     !
-    !qepy --> reset values
+    !qepy fix --> reset values
     dft = 'not set'
     discard_input_dft = .FALSE.
-    !qepy <-- reset values
+    iexch = notset
+    icorr = notset
+    igcx  = notset
+    igcc  = notset
+    imeta = notset
+    imetac= notset
+    inlc  = notset
+    !qepy fix <-- reset values
 
     CALL set_dft_from_name( dft_ )
     IF (dft == 'not set') CALL errore( 'enforce_input_dft', 'cannot fix unset dft', 1 )
     discard_input_dft = .TRUE.
     !
     IF ( PRESENT(nomsg) ) RETURN
     !
```

### Comparing `qepy-0.0.2rc2/src/qe/qepy_electrons.f90` & `qepy-0.0.3rc0/src/qe/qepy_electrons.f90`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 !
 !----------------------------------------------------------------------------
 ! TB
 ! included gate related energy
 !----------------------------------------------------------------------------
 !
 !----------------------------------------------------------------------------
-SUBROUTINE qepy_electrons(embed)
+SUBROUTINE qepy_electrons()
   !----------------------------------------------------------------------------
   !! General self-consistency loop, also for hybrid functionals
   !! For non-hybrid functionals it just calls "electron_scf"
   !
   USE kinds,                ONLY : DP
   USE check_stop,           ONLY : check_stop_now, stopped_by_user
   USE io_global,            ONLY : stdout, ionode
@@ -47,20 +47,18 @@
   USE paw_variables,        ONLY : okpaw, ddd_paw, total_core_energy, only_paw
   USE paw_onecenter,        ONLY : PAW_potential
   USE paw_symmetry,         ONLY : PAW_symmetrize_ddd
   USE ions_base,            ONLY : nat
   USE loc_scdm,             ONLY : use_scdm, localize_orbitals
   USE loc_scdm_k,           ONLY : localize_orbitals_k
   !
-  USE qepy_common,          ONLY : embed_base
+  USE qepy_common,          ONLY : embed
   !
   IMPLICIT NONE
   !
-  type(embed_base), intent(inout)    :: embed
-  !
   ! ... a few local variables
   !
   REAL(DP) :: charge
   !! the total charge
   REAL(DP) :: exxen
   !! used to compute exchange energy
   REAL(DP), EXTERNAL :: exxenergyace
@@ -156,15 +154,15 @@
   DO idum=1,niter
      !
      iter = iter + 1
      !
      ! ... Self-consistency loop. For hybrid functionals the exchange potential
      ! ... is calculated with the orbitals at previous step (none at first step)
      !
-     CALL qepy_electrons_scf ( printout, exxen, embed )
+     CALL qepy_electrons_scf ( printout, exxen)
      !
      IF ( .NOT. dft_is_hybrid() ) RETURN
      !
      ! ... From now on: hybrid DFT only
      !
      IF ( stopped_by_user .OR. .NOT. conv_elec ) THEN
         conv_elec=.FALSE.
@@ -210,15 +208,15 @@
         exxen = 0.50d0*fock2 
         etot = etot - etxc 
         !
         ! Recalculate potential because XC functional has changed,
         ! start self-consistency loop on exchange
         !
         CALL qepy_v_of_rho( rho, rho_core, rhog_core, &
-             ehart, etxc, vtxc, eth, etotefield, charge, v, embed)
+             ehart, etxc, vtxc, eth, etotefield, charge, v)
         etot = etot + etxc + exxen
         !
         IF (okpaw) CALL PAW_potential(rho%bec, ddd_PAW, epaw,etot_cmp_paw)
         CALL set_vrs( vrs, vltot, v%of_r, kedtau, v%kin_r, dfftp%nnr, &
              nspin, doublegrid )
         !
      ELSE
@@ -348,15 +346,15 @@
 9101 FORMAT(/'     EXX self-consistency reached' )
 9120 FORMAT(/'     EXX convergence NOT achieved after ',i3,' iterations: stopping' )
 9121 FORMAT(/'     scf convergence threshold =',1PE17.1,' Ry' )
   !
 END SUBROUTINE qepy_electrons
 !
 !----------------------------------------------------------------------------
-SUBROUTINE qepy_electrons_scf ( printout, exxen, embed)
+SUBROUTINE qepy_electrons_scf ( printout, exxen)
   !----------------------------------------------------------------------------
   !! This routine is a driver of the self-consistent cycle.
   !! It uses the routine c_bands for computing the bands at fixed
   !! Hamiltonian, the routine sum_band to compute the charge density,
   !! the routine v_of_rho to compute the new potential and the routine
   !! mix_rho to mix input and output charge densities.
   !
@@ -420,24 +418,23 @@
   USE dfunct,               ONLY : newd
   USE esm,                  ONLY : do_comp_esm, esm_printpot, esm_ewald
   USE fcp_variables,        ONLY : lfcpopt, lfcpdyn
   USE wrappers,             ONLY : memstat
   !
   USE plugin_variables,     ONLY : plugin_etot
   !
-  USE qepy_common,          ONLY : embed_base
+  USE qepy_common,          ONLY : embed
   !
   IMPLICIT NONE
   !
   INTEGER, INTENT (IN) :: printout
   !! * If printout>0, prints on output the total energy;
   !! * if printout>1, also prints decomposition into energy contributions.
   REAL(DP),INTENT (IN) :: exxen
   !! current estimate of the exchange energy
-  type(embed_base), intent(inout)    :: embed
   !
   ! ... local variables
   !
   REAL(DP),save :: dr2
   !! the norm of the diffence between potential
   REAL(DP) :: charge
   !! the total charge
@@ -523,15 +520,15 @@
      ewld = esm_ewald()
   ELSE
      ewld = ewald( alat, nat, nsp, ityp, zv, at, bg, tau, &
                 omega, g, gg, ngm, gcutm, gstart, gamma_only, strf )
   ENDIF
   endif
   if (iand(embed%exttype,1) == 1) then
-     call qepy_setlocal(embed%exttype)
+     call qepy_setlocal()
   endif
   !
   IF ( llondon ) THEN
      elondon = energy_london( alat , nat , ityp , at ,bg , tau )
   ELSE
      elondon = 0.d0
   ENDIF
@@ -567,15 +564,15 @@
   end if ! if (embed%initial)
   !
   !%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
   !%%%%%%%%%%%%%%%%%%%%          iterate !          %%%%%%%%%%%%%%%%%%%%%
   !%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%%
   !
   CALL qepy_v_of_rho_all( rho, rho_core, rhog_core, &
-     ehart, etxc, vtxc, eth, etotefield, charge, v, embed)
+     ehart, etxc, vtxc, eth, etotefield, charge, v)
 
   if ( add_descf .and. embed%mix_coef<0.0_DP ) then
      descf = qepy_delta_escf(rho, rho_prev)
      goto 112
   endif
   if (.not. embed%ldescf) descf = 0._dp
 
@@ -812,15 +809,15 @@
         !
         IF ( .NOT. conv_elec ) THEN
            !
            ! ... no convergence yet: calculate new potential from mixed
            ! ... charge density (i.e. the new estimate)
            !
            CALL qepy_v_of_rho_all( rhoin, rho_core, rhog_core, &
-              ehart, etxc, vtxc, eth, etotefield, charge, v, embed)
+              ehart, etxc, vtxc, eth, etotefield, charge, v)
            !CALL v_of_rho( rhoin, rho_core, rhog_core, &
            !               ehart, etxc, vtxc, eth, etotefield, charge, v)
            !!
            !IF (okpaw) THEN
            !   CALL PAW_potential( rhoin%bec, ddd_paw, epaw,etot_cmp_paw )
            !   CALL PAW_symmetrize_ddd( ddd_paw )
            !ENDIF
@@ -842,18 +839,16 @@
         ELSE 
            !
            ! ... convergence reached:
            ! ... 1) the output HXC-potential is saved in v
            ! ... 2) vnew contains V(out)-V(in) ( used to correct the forces ).
            !
            vnew%of_r(:,:) = v%of_r(:,:)
-           !CALL v_of_rho( rho,rho_core,rhog_core, &
-           !           ehart, etxc, vtxc, eth, etotefield, charge, v)
            CALL qepy_v_of_rho_all( rho, rho_core, rhog_core, &
-              ehart, etxc, vtxc, eth, etotefield, charge, v, embed)
+                          ehart, etxc, vtxc, eth, etotefield, charge, v)
            vnew%of_r(:,:) = v%of_r(:,:) - vnew%of_r(:,:)
            !
            !IF (okpaw) THEN
            !   CALL PAW_potential( rho%bec, ddd_paw, epaw, etot_cmp_paw )
            !   CALL PAW_symmetrize_ddd( ddd_paw )
            !ENDIF
            !
```

### Comparing `qepy-0.0.2rc2/src/qe/qepy_electrons_nscf.f90` & `qepy-0.0.3rc0/src/qe/qepy_electrons_nscf.f90`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ! Copyright (C) 2001-2016 Quantum ESPRESSO group
 ! This file is distributed under the terms of the
 ! GNU General Public License. See the file `License'
 ! in the root directory of the present distribution,
 ! or http://www.gnu.org/copyleft/gpl.txt .
 !
 !----------------------------------------------------------------------------
-SUBROUTINE qepy_electrons_nscf ( printout, exxen, embed)
+SUBROUTINE qepy_electrons_nscf ( printout, exxen)
   !----------------------------------------------------------------------------
   !! This routine is a driver of the self-consistent cycle.
   !! It uses the routine c_bands for computing the bands at fixed
   !! Hamiltonian, the routine sum_band to compute the charge density,
   !! the routine v_of_rho to compute the new potential and the routine
   !! mix_rho to mix input and output charge densities.
   !
@@ -74,24 +74,23 @@
   USE dfunct,               ONLY : newd
   USE esm,                  ONLY : do_comp_esm, esm_printpot, esm_ewald
   USE fcp_variables,        ONLY : lfcpopt, lfcpdyn
   USE wrappers,             ONLY : memstat
   !
   USE plugin_variables,     ONLY : plugin_etot
   !
-  USE qepy_common,          ONLY : embed_base
+  USE qepy_common,          ONLY : embed
   !
   IMPLICIT NONE
   !
   INTEGER, INTENT (IN) :: printout
   !! * If printout>0, prints on output the total energy;
   !! * if printout>1, also prints decomposition into energy contributions.
   REAL(DP),INTENT (IN) :: exxen
   !! current estimate of the exchange energy
-  type(embed_base), intent(inout)    :: embed
   !
   ! ... local variables
   !
   REAL(DP),save :: dr2
   !! the norm of the diffence between potential
   REAL(DP) :: charge
   !! the total charge
@@ -166,23 +165,24 @@
   CALL start_clock( 'electrons' )
   !
   FLUSH( stdout )
   !
   ! ... calculates the ewald contribution to total energy
   !
   !if (embed%initial) then
-  if (embed%exttype<1) then
+  if (embed%lewald) then
   IF ( do_comp_esm ) THEN
      ewld = esm_ewald()
   ELSE
      ewld = ewald( alat, nat, nsp, ityp, zv, at, bg, tau, &
                 omega, g, gg, ngm, gcutm, gstart, gamma_only, strf )
   ENDIF
-  else if (iand(embed%exttype,1) == 1) then
-     call qepy_setlocal(embed%exttype)
+  endif
+  if (iand(embed%exttype,1) == 1) then
+     call qepy_setlocal()
   endif
   !
   IF ( llondon ) THEN
      elondon = energy_london( alat , nat , ityp , at ,bg , tau )
   ELSE
      elondon = 0.d0
   ENDIF
@@ -207,15 +207,15 @@
   FLUSH( stdout )
   !
   else
   dr2 = embed%dnorm
   end if ! if (embed%initial)
   !
   CALL qepy_v_of_rho_all( rho, rho_core, rhog_core, &
-     ehart, etxc, vtxc, eth, etotefield, charge, v, embed)
+     ehart, etxc, vtxc, eth, etotefield, charge, v)
 
   IF ( check_stop_now() ) THEN
      conv_elec=.FALSE.
      CALL save_in_electrons (iter, dr2, ethr, et )
      GO TO 10
   ENDIF
```

### Comparing `qepy-0.0.2rc2/src/qe/qepy_forces.f90` & `qepy-0.0.3rc0/src/qe/qepy_forces.f90`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 !
 !----------------------------------------------------------------------------
 ! TB
 ! included gate related forces
 !----------------------------------------------------------------------------
 !
 !----------------------------------------------------------------------------
-SUBROUTINE qepy_forces(icalc, embed)
+SUBROUTINE qepy_forces(icalc)
   !----------------------------------------------------------------------------
   !! This routine is a driver routine which computes the forces
   !! acting on the atoms. The complete expression of the forces
   !! contains four parts which are computed by different routines:
   !!
   !!  a)  force_lc,     local contribution to the forces
   !!  b)  force_cc,     contribution due to NLCC
@@ -53,20 +53,19 @@
 
   USE xdm_module,        ONLY : force_xdm
   USE tsvdw_module,      ONLY : FtsvdW
   USE esm,               ONLY : do_comp_esm, esm_bc, esm_force_ew
   USE qmmm,              ONLY : qmmm_mode
   !
   USE becmod, ONLY: becp, deallocate_bec_type, is_allocated_bec_type
-  USE qepy_common,          ONLY : embed_base
+  USE qepy_common,          ONLY : embed
   !
   IMPLICIT NONE
   !
   integer,intent(in),optional             :: icalc
-  type(embed_base),intent(inout),optional :: embed
   integer                                 :: calctype
   !
   REAL(DP), ALLOCATABLE :: forcenl(:,:),   &
                            forcelc(:,:),   &
                            forcecc(:,:),   &
                            forceion(:,:),  &
                            force_disp(:,:),&
@@ -200,17 +199,15 @@
   END IF
   !
   ! ... call void routine for user define/ plugin patches on internal forces
   !
   CALL plugin_int_forces()
   !
   !qepy --> add external forces
-  if (present(embed)) then
-     if (allocated(embed%extforces)) force(:,:) = force(:,:) + embed%extforces
-  endif
+  if (allocated(embed%extforces)) force(:,:) = force(:,:) + embed%extforces
   !qepy <-- add external forces
   !
   ! ... Berry's phase electric field terms
   !
   IF (lelfield) THEN
      ALLOCATE( forces_bp_efield(3,nat) )
      forces_bp_efield(:,:)=0.d0
@@ -297,15 +294,14 @@
   !
   IF( textfor ) force(:,:) = force(:,:) + extfor(:,:)
   !
   ! ... call void routine for user define/ plugin patches on external forces
   !
   CALL plugin_ext_forces()
   !
-  !
   ! ... write on output the forces
   !
   WRITE( stdout, '(/,5x,"Forces acting on atoms (cartesian axes, Ry/au):", / )')
   DO na = 1, nat
      WRITE( stdout, 9035) na, ityp(na), force(:,na)
   END DO
   !
```

### Comparing `qepy-0.0.2rc2/src/qe/qepy_hinit1.f90` & `qepy-0.0.3rc0/src/qe/qepy_hinit1.f90`

 * *Files 6% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ! Copyright (C) 2001-2011 Quantum ESPRESSO group
 ! This file is distributed under the terms of the
 ! GNU General Public License. See the file `License'
 ! in the root directory of the present distribution,
 ! or http://www.gnu.org/copyleft/gpl.txt .
 !
 !----------------------------------------------------------------------------
-SUBROUTINE qepy_hinit1(exttype)
+SUBROUTINE qepy_hinit1()
   !----------------------------------------------------------------------------
   !! Atomic configuration dependent hamiltonian initialization,
   !! potential, wavefunctions for Hubbard U.  
   !! Important note: it does not recompute structure factors and core charge,
   !! they must be computed before this routine is called.
   !
   USE ions_base,           ONLY : nat, nsp, ityp, tau
@@ -29,25 +29,23 @@
   USE paw_variables,       ONLY : okpaw, ddd_paw
   USE paw_onecenter,       ONLY : paw_potential
   USE paw_symmetry,        ONLY : paw_symmetrize_ddd
   USE dfunct,              ONLY : newd
   !
   IMPLICIT NONE
   !
-  integer,                         intent(in)      :: exttype
-  !
   ! these routines can be used to patch quantities that are dependent
   ! on the ions and cell parameters
   !
   CALL plugin_init_ions()
   CALL plugin_init_cell()
   !
   ! ... calculate the total local potential
   !
-  CALL qepy_setlocal(exttype)
+  CALL qepy_setlocal()
   !
   IF ( tqr ) CALL generate_qpointlist()
   !
   IF ( real_space ) THEN
      CALL betapointlist()
      CALL init_realspace_vars()
   ENDIF
```

### Comparing `qepy-0.0.2rc2/src/qe/qepy_init_run.f90` & `qepy-0.0.3rc0/src/qe/qepy_init_run.f90`

 * *Files 3% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ! Copyright (C) 2001-2006 Quantum ESPRESSO group
 ! This file is distributed under the terms of the
 ! GNU General Public License. See the file `License'
 ! in the root directory of the present distribution,
 ! or http://www.gnu.org/copyleft/gpl.txt .
 !
 !----------------------------------------------------------------------------
-SUBROUTINE qepy_init_run(oldxml)
+SUBROUTINE qepy_init_run()
   !----------------------------------------------------------------------------
   !
   USE klist,              ONLY : nkstot
   USE symme,              ONLY : sym_rho_init
   USE wvfct,              ONLY : nbnd, et, wg, btype
   USE control_flags,      ONLY : lmd, gamma_only, smallmem, ts_vdw
   USE gvect,              ONLY : g, gg, mill, gcutm, ig_l2g, ngm, ngm_g, &
@@ -32,25 +32,22 @@
   USE recvec_subs,        ONLY : ggen, ggens
   USE wannier_new,        ONLY : use_wannier    
   USE dfunct,             ONLY : newd
   USE esm,                ONLY : do_comp_esm, esm_init
   USE tsvdw_module,       ONLY : tsvdw_initialize
   USE Coul_cut_2D,        ONLY : do_cutoff_2D, cutoff_fact 
   !
+  USE qepy_common,        ONLY : embed
+  !
   IMPLICIT NONE
-  LOGICAL, INTENT(IN), OPTIONAL :: oldxml
-  LOGICAL               :: oldver
+  LOGICAL               :: oldxml
   !
-  if (present(oldxml)) then
-     oldver = oldxml
-  else
-     oldver = .FALSE.
-  endif
+  oldxml = embed%oldxml
 #if !defined (__OLDXML) 
-if (oldver) then
+if (oldxml) then
    CALL errore( 'qepy_init_run', 'Do no use oldxml in normal version. Please rebuild with -D__OLDXML.', 1 )
 endif
 #endif
   !
   CALL start_clock( 'init_run' )
   !
   ! ... calculate limits of some indices, used in subsequent allocations
@@ -124,37 +121,35 @@
   !
   CALL allocate_wfc_k()
   CALL openfil()
   !
   CALL hinit0()
   !
   CALL mp_barrier( intra_image_comm ) ! for oldxml
-  if (oldver) then
+  if (oldxml) then
 #if defined (__OLDXML) 
      call oldxml_potinit()
 #else
    CALL errore( 'qepy_init_run', 'Do no use oldxml in normal version. Please rebuild with -D__OLDXML.', 1 )
 #endif
   else
-  !CALL potinit()
-  CALL qepy_potinit('')
+  CALL potinit()
   endif
   !
   CALL newd()
   !
   CALL mp_barrier( intra_image_comm ) ! for oldxml
-  if (oldver) then
+  if (oldxml) then
 #if defined (__OLDXML) 
      call oldxml_wfcinit()
 #else
    CALL errore( 'qepy_init_run', 'Do no use oldxml in normal version. Please rebuild with -D__OLDXML.', 1 )
 #endif
   else
-  !CALL wfcinit()
-  CALL qepy_wfcinit('')
+  CALL wfcinit()
   endif
   !
   IF(use_wannier) CALL wannier_init()
   !
 #if defined(__MPI)
   ! Cleanup PAW arrays that are only used for init
   IF (okpaw) CALL paw_post_init() ! only parallel!
```

### Comparing `qepy-0.0.2rc2/src/qe/qepy_potinit.f90` & `qepy-0.0.3rc0/src/fix/potinit.f90`

 * *Files 8% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ! This file is distributed under the terms of the
 ! GNU General Public License. See the file `License'
 ! in the root directory of the present distribution,
 ! or http://www.gnu.org/copyleft/gpl.txt .
 !
 !
 !----------------------------------------------------------------------------
-SUBROUTINE qepy_potinit(starting)
+SUBROUTINE potinit()
   !----------------------------------------------------------------------------
   !
   ! ... This routine initializes the self consistent potential in the array
   ! ... vr. There are three possible cases:
   !
   ! ... a) the code is restarting from a broken run:
   ! ...    read rho from data stored during the previous run
@@ -52,40 +52,35 @@
   USE fft_rho,              ONLY : rho_g2r, rho_r2g
   !
   USE uspp,                 ONLY : becsum
   USE paw_variables,        ONLY : okpaw, ddd_PAW
   USE paw_init,             ONLY : PAW_atomic_becsum
   USE paw_onecenter,        ONLY : PAW_potential
   !
+  !qepy fix --> import module
   USE klist,                ONLY : nelup, neldw
-  !
+  !qepy fix --> import module
   IMPLICIT NONE
   !
   REAL(DP)              :: charge           ! the starting charge
   REAL(DP)              :: etotefield       !
   REAL(DP)              :: fact
   INTEGER               :: is
   LOGICAL               :: exst 
   CHARACTER(LEN=320)    :: filename
   !
-  CHARACTER(LEN=*), INTENT(IN), OPTIONAL :: starting
-  !
   CALL start_clock('potinit')
   !
   filename = TRIM (restart_dir( )) // 'charge-density'
 #if defined __HDF5
   exst     =  check_file_exist( TRIM(filename) // '.hdf5' )
 #else 
   exst     =  check_file_exist( TRIM(filename) // '.dat' )
 #endif
   !
-  IF (present(starting)) THEN
-     IF (len_trim(starting)>1) starting_pot = trim(starting)
-  ENDIF
-  !
   IF ( starting_pot == 'file' .AND. exst ) THEN
      !
      ! ... Cases a) and b): the charge density is read from file
      ! ... this also reads rho%ns if lda+U, rho%bec if PAW, rho%kin if metaGGA
      !
      IF ( .NOT.lforcet ) THEN
         CALL read_scf ( rho, nspin, gamma_only )
@@ -180,19 +175,19 @@
      ENDIF
      !
   ELSE IF ( .NOT. lscf .AND. ABS( charge - nelec ) > (1.D-3 * charge ) ) THEN
      !
      CALL errore( 'potinit', 'starting and expected charges differ', 1 )
      !
   END IF
-  !qepy --> scale charge for spin
+  !qepy fix --> scale charge for spin
   IF ( nspin == 2 ) THEN
      rho%of_g(1,2) = (nelup-neldw) / omega
   ENDIF
-  !qepy <-- scale charge for spin
+  !qepy fix <-- scale charge for spin
   !
   ! ... bring starting rho from G- to R-space
   !
   CALL rho_g2r (dfftp, rho%of_g, rho%of_r)
   !
   IF  ( dft_is_meta() ) THEN
      IF (starting_pot /= 'file') THEN
@@ -248,43 +243,43 @@
   IF ( report /= 0 .AND. &
        noncolin .AND. domag .AND. lscf ) CALL report_mag()
   !
   CALL stop_clock('potinit')
   !
   RETURN
   !
-END SUBROUTINE qepy_potinit
+END SUBROUTINE potinit
 !
 !-------------
-!SUBROUTINE nc_magnetization_from_lsda ( ngm, nspin, rho )
-!  !-------------
-!  !
-!  USE kinds,     ONLY: dp
-!  USE constants, ONLY: pi
-!  USE io_global, ONLY: stdout
-!  USE noncollin_module, ONLY: angle1, angle2
-!  !
-!  IMPLICIT NONE
-!  INTEGER, INTENT (in):: ngm, nspin
-!  COMPLEX(dp), INTENT (inout):: rho(ngm,nspin)
-!  !---  
-!  !  set up noncollinear m_x,y,z from collinear m_z (AlexS) 
-!  !
-!  WRITE(stdout,*)
-!  WRITE(stdout,*) '-----------'
-!  WRITE(stdout,'("Spin angles Theta, Phi (degree) = ",2f8.4)') &
-!       angle1(1)/PI*180.d0, angle2(1)/PI*180.d0 
-!  WRITE(stdout,*) '-----------'
-!  !
-!  ! now set rho(2)=magn*sin(theta)*cos(phi)   x
-!  !         rho(3)=magn*sin(theta)*sin(phi)   y
-!  !         rho(4)=magn*cos(theta)            z
-!  !
-!  rho(:,2) = rho(:,4)*sin(angle1(1))
-!  rho(:,3) = rho(:,2)*sin(angle2(1))
-!  rho(:,4) = rho(:,4)*cos(angle1(1))
-!  rho(:,2) = rho(:,2)*cos(angle2(1))
-!  !
-!  RETURN
-!  !
-!END SUBROUTINE nc_magnetization_from_lsda
+SUBROUTINE nc_magnetization_from_lsda ( ngm, nspin, rho )
+  !-------------
+  !
+  USE kinds,     ONLY: dp
+  USE constants, ONLY: pi
+  USE io_global, ONLY: stdout
+  USE noncollin_module, ONLY: angle1, angle2
+  !
+  IMPLICIT NONE
+  INTEGER, INTENT (in):: ngm, nspin
+  COMPLEX(dp), INTENT (inout):: rho(ngm,nspin)
+  !---  
+  !  set up noncollinear m_x,y,z from collinear m_z (AlexS) 
+  !
+  WRITE(stdout,*)
+  WRITE(stdout,*) '-----------'
+  WRITE(stdout,'("Spin angles Theta, Phi (degree) = ",2f8.4)') &
+       angle1(1)/PI*180.d0, angle2(1)/PI*180.d0 
+  WRITE(stdout,*) '-----------'
+  !
+  ! now set rho(2)=magn*sin(theta)*cos(phi)   x
+  !         rho(3)=magn*sin(theta)*sin(phi)   y
+  !         rho(4)=magn*cos(theta)            z
+  !
+  rho(:,2) = rho(:,4)*sin(angle1(1))
+  rho(:,3) = rho(:,2)*sin(angle2(1))
+  rho(:,4) = rho(:,4)*cos(angle1(1))
+  rho(:,2) = rho(:,2)*cos(angle2(1))
+  !
+  RETURN
+  !
+END SUBROUTINE nc_magnetization_from_lsda
```

### Comparing `qepy-0.0.2rc2/src/qe/qepy_pw2casino_write.f90` & `qepy-0.0.3rc0/src/qe/qepy_pw2casino_write.f90`

 * *Files 1% similar despite different names*

```diff
@@ -316,15 +316,15 @@
    !IF(blip)CALL pw2blip_cleanup
    !DEALLOCATE (igtog, g_l, evc_l )
    !IF(blip.or.gather) DEALLOCATE ( ngtot_d, ngtot_cumsum, g_g, evc_g )
    !IF(dowrite.and..not.blip) DEALLOCATE (indx)
 
 !CONTAINS
 
-   SUBROUTINE qepy_calc_energies(embed)
+   SUBROUTINE qepy_calc_energies()
       USE becmod, ONLY: becp, calbec, allocate_bec_type, deallocate_bec_type, is_allocated_bec_type
       USE exx,    ONLY : exxenergy2, fock2
       USE funct,  ONLY : dft_is_hybrid
       USE kinds, ONLY: DP,sgl
       USE ions_base, ONLY : nat, ntyp => nsp, ityp, tau, zv, atm
       USE cell_base, ONLY: omega, alat, tpiba2, at, bg
       USE run_info,  ONLY: title    ! title of the run
@@ -348,20 +348,20 @@
       USE io_global, ONLY: stdout, ionode, ionode_id
       USE io_files, ONLY: nd_nmbr, nwordwfc, iunwfc, prefix, tmp_dir, seqopn
       USE wavefunctions, ONLY : evc
       USE funct, ONLY : dft_is_meta
       USE mp_pools, ONLY: inter_pool_comm, intra_pool_comm, nproc_pool, me_pool
       USE mp_bands, ONLY: intra_bgrp_comm
       USE mp, ONLY: mp_sum, mp_gather, mp_bcast, mp_get
-      USE buffers,              ONLY : get_buffer
+      USE buffers,              ONLY : get_buffer, open_buffer
 
       USE pw2blip
       !
       !qepy --> import more
-      USE qepy_common,          ONLY : embed_base
+      USE qepy_common,          ONLY : embed
       USE ener,                 ONLY : etot, hwf_energy, eband, deband, ehart, &
                                        vtxc, etxc, etxcc, ewld, demet, epaw, &
                                        elondon, edftd3, ef_up, ef_dw, exdm, ef
       USE control_flags,        ONLY : mixing_beta, tr2, ethr, niter, nmix, &
                                        iprint, conv_elec, &
                                        restart, io_level, do_makov_payne,  &
                                        iverbosity, textfor,     &
@@ -390,16 +390,14 @@
       USE noncollin_module,     ONLY : noncolin, magtot_nc, i_cons,  bfield, &
                                        lambda, report
       USE lsda_mod,             ONLY : lsda, nspin, magtot, absmag, isk
       USE spin_orb,             ONLY : domag
       !qepy <-- import more
       !
       IMPLICIT NONE
-
-      type(embed_base), intent(inout)    :: embed
       !
       COMPLEX(DP), ALLOCATABLE :: aux(:)
       INTEGER :: npw, ibnd, j, ig, ik,ikk, ispin, na, nt, ijkb0, ikb,jkb, ih,jh
       REAL(dp), ALLOCATABLE :: g2kin(:)
       !qepy --> remove etotefield
       !REAL(DP) :: charge, etotefield, elocg
       REAL(DP) :: charge, elocg
@@ -430,17 +428,17 @@
          !nbndup = nbnd
          !nbnddown = 0
          nk = nks
          !     nspin = 1
       ENDIF
 
       ALLOCATE (aux(dfftp%nnr))
-      !qepy
+      !qepy add --> fix
       if (is_allocated_bec_type(becp)) call deallocate_bec_type(becp)
-      !
+      !qepy add <-- fix
       CALL allocate_bec_type ( nkb, nbnd, becp )
 
       ek  = 0.d0
       eloc= 0.d0
       enl = 0.d0
       demet=0.d0
       fock2=0.d0
@@ -753,77 +751,52 @@
       embed%energies%fock2            = fock2                      !'EXX energy'
       embed%energies%demet            = demet                      !'Smearing (-TS)'
       !
       embed%energies%ehf              = ehf
       !
       IF (llondon) THEN
          embed%energies%elondon       = elondon                    !'Dispersion Correction'
-      ELSE
-         embed%energies%elondon       = 0.d0
       ENDIF
       IF (ldftd3) THEN
          embed%energies%edftd3        = edftd3                     !'DFT-D3 Dispersion'
-      ELSE
-         embed%energies%edftd3        = 0.d0
       ENDIF
       IF (lxdm) THEN
          embed%energies%exdm          = exdm                       !'Dispersion XDM Correction'
-      ELSE
-         embed%energies%exdm          = 0.d0
       ENDIF
       IF (ts_vdw) THEN
          embed%energies%etsvdw        = 2.0d0*EtsvdW               !'Dispersion T-S Correction'
-      ELSE
-         embed%energies%etsvdw        = 0.d0
       ENDIF
       IF( textfor ) THEN
          embed%energies%eext          = eext                       !'External forces energy'
-      ELSE
-         embed%energies%eext          = 0.d0
       ENDIF
       IF ( tefield ) THEN
          embed%energies%etotefield    = etotefield                 !'electric field correction'
-      ELSE
-         embed%energies%etotefield    = 0.d0
       ENDIF
       IF ( gate) THEN
          embed%energies%etotgatefield = etotgatefield              !'gate field correction'
-      ELSE
-         embed%energies%etotgatefield = 0.d0
       ENDIF
       IF ( lda_plus_u ) THEN
          embed%energies%eth           = eth                        !'Hubbard energy'
-      ELSE
-         embed%energies%eth           = 0.d0
       ENDIF
       IF (okpaw) THEN
          embed%energies%epaw          = epaw                       !'one-center paw contrib.'
-      ELSE
-         embed%energies%epaw          = 0.d0
       ENDIF
       IF ( lfcpopt .or. lfcpdyn ) THEN
          embed%energies%ept           = ef * tot_charge            !'potentiostat contribution'
-      ELSE
-         embed%energies%ept           = 0.d0
       ENDIF
       !
       embed%energies%extene           = extene                     !'External energy0'
       ! some energies details -->
       embed%energies%etxc             = etxc                       ! the exchange and correlation energy
       embed%energies%etxcc            = etxcc                      ! the nlcc exchange and correlation
       IF (okpaw) THEN
          embed%energies%paw_ehart_ae  = SUM(etot_cmp_paw(:,1,1))   !'PAW hartree energy AE'
          embed%energies%paw_ehart_ps  = SUM(etot_cmp_paw(:,1,2))   !'PAW hartree energy PS'
          embed%energies%paw_exc_ae    = SUM(etot_cmp_paw(:,2,1))   !'PAW xc energy AE'
          embed%energies%paw_exc_ps    = SUM(etot_cmp_paw(:,2,2))   !'PAW xc energy PS'
-      ELSE
-         embed%energies%paw_ehart_ae  = 0.d0
-         embed%energies%paw_ehart_ps  = 0.d0
-         embed%energies%paw_exc_ae    = 0.d0
-         embed%energies%paw_exc_ps    = 0.d0
       ENDIF
       ! <--
 
    END SUBROUTINE qepy_calc_energies
 
 
    !SUBROUTINE test_overlap
```

### Comparing `qepy-0.0.2rc2/src/qe/qepy_pw_restart_new.f90` & `qepy-0.0.3rc0/src/fix/pw_restart_new.f90`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ! Copyright (C) 2016 Quantum ESPRESSO group
 ! This file is distributed under the terms of the
 ! GNU General Public License. See the file `License'
 ! in the root directory of the present distribution,
 ! or http://www.gnu.org/copyleft/gpl.txt .
 !
 !----------------------------------------------------------------------------
-MODULE qepy_pw_restart_new
+MODULE pw_restart_new
 !----------------------------------------------------------------------------
   !
   ! ... New PWscf I/O using xml schema and (optionally) hdf5 binaries
   ! ... Parallel execution: the xml file is written by one processor only
   ! ... ("ionode_id"), read by all processors ;
   ! ... the wavefunction files are written / read by one processor per pool,
   ! ... collected on / distributed to all other processors in pool
@@ -45,16 +45,15 @@
   USE io_files,  ONLY : iunpun, xmlfile
   !
   IMPLICIT NONE
   !
   CHARACTER(LEN=6), EXTERNAL :: int_to_char
   PRIVATE
   PUBLIC :: pw_write_schema, pw_write_binaries
-  !PUBLIC :: read_xml_file, read_collected_wfc
-  PUBLIC :: qepy_read_xml_file, read_collected_wfc
+  PUBLIC :: read_xml_file, read_collected_wfc
   !
   CONTAINS
     !------------------------------------------------------------------------
     SUBROUTINE pw_write_schema( only_init, wf_collect )
       !------------------------------------------------------------------------
       !
       ! only_init  = T  write only variables that are known after the 
@@ -892,15 +891,15 @@
       DEALLOCATE( itmp, igwk_ )
       !
       RETURN
       !
     END SUBROUTINE gk_l2gmap_kdip
     !
     !--------------------------------------------------------------------------
-    SUBROUTINE qepy_read_xml_file ( wfc_is_collected, alloc )
+    SUBROUTINE read_xml_file ( wfc_is_collected )
       !------------------------------------------------------------------------
       !
       ! ... This routine allocates space for all quantities already computed
       ! ... in the pwscf program and reads them from the data file.
       ! ... All quantities that are initialized in subroutine "setup" when
       ! ... starting from scratch should be initialized here when restarting
       !
@@ -957,47 +956,39 @@
       USE basis,           ONLY : natomwfc
       USE uspp,            ONLY : okvan
       USE paw_variables,   ONLY : okpaw
       !
       USE mp_images,       ONLY : intra_image_comm
       USE mp,              ONLY : mp_bcast
       !
-      !qepy --> other parameters
+      !qepy fix --> other parameters
       USE tsvdw_module,         ONLY : vdw_econv_thr
       USE input_parameters,     ONLY : verbosity, calculation, ion_dynamics, starting_ns_eigenvalue, &
                                        vdw_corr, london, k_points, assume_isolated, &  
                                        input_parameters_occupations => occupations, dftd3_threebody, &
                                        dftd3_version
-      !qepy <-- other parameters
+      !qepy fix <-- other parameters
       !
       IMPLICIT NONE
       LOGICAL, INTENT(OUT) :: wfc_is_collected
       !
-      LOGICAL, INTENT(IN), OPTIONAL :: alloc
-      LOGICAL :: lalloc
-      !
       INTEGER  :: i, is, ik, ierr, dum1,dum2,dum3
       LOGICAL  :: magnetic_sym, lvalid_input, lfixed
-      !qepy --> 
+      !qepy fix --> declare vdw
       !CHARACTER(LEN=20) :: dft_name, vdw_corr, occupations
       CHARACTER(LEN=20) :: dft_name, occupations
-      !qepy <-- 
+      INTEGER           :: npwx_g
+      !qepy fix <-- declare vdw
       CHARACTER(LEN=320):: filename
       REAL(dp) :: exx_fraction, screening_parameter
       TYPE (output_type)        :: output_obj 
       TYPE (parallel_info_type) :: parinfo_obj
       TYPE (general_info_type ) :: geninfo_obj
       TYPE (input_type)         :: input_obj
       !
-      if (present(alloc)) then
-         lalloc = alloc
-      else
-         lalloc = .TRUE.
-      endif
-      !
       !
       filename = xmlfile ( )
       !
       IF (ionode) CALL qexsd_readschema ( filename, &
            ierr, output_obj, parinfo_obj, geninfo_obj, input_obj)
       CALL mp_bcast(ierr, ionode_id, intra_image_comm)
       IF ( ierr > 0 ) CALL errore ( 'read_xml_file', 'fatal error reading xml file', ierr ) 
@@ -1032,22 +1023,22 @@
       !
       at = at / alat
       tau(:,1:nat) = tau(:,1:nat)/alat  
       CALL at2celldm (ibrav,alat,at(:,1),at(:,2),at(:,3),celldm)
       CALL volume (alat,at(:,1),at(:,2),at(:,3),omega)
       !!
       !! Basis set section
-      if (lalloc) then
-      !qepy: Here, npwx is npwx_g, which is greater than npwx in mpi
+      !qepy fix --> npwx is npwx_g
+      !Here, npwx is npwx_g, which is greater than npwx in mpi
       CALL qexsd_copy_basis_set ( output_obj%basis_set, gamma_only, ecutwfc,&
            ecutrho, dffts%nr1,dffts%nr2,dffts%nr3, dfftp%nr1,dfftp%nr2,dfftp%nr3, &
-           dum1,dum2,dum3, ngm_g, ngms_g, npwx, bg(:,1), bg(:,2), bg(:,3) )
+           dum1,dum2,dum3, ngm_g, ngms_g, npwx_g, bg(:,1), bg(:,2), bg(:,3) )
       ecutwfc = ecutwfc*e2
       ecutrho = ecutrho*e2
-      endif
+      !qepy fix <-- npwx is npwx_g
       dual = ecutrho/ecutwfc
       ! FIXME: next line ensures exact consistency between reciprocal and
       ! direct lattice vectors, preventing weird phonon symmetry errors
       ! (due to lousy algorithms, extraordinarily sensitive to tiny errors)
       CALL recips ( at(1,1), at(1,2), at(1,3), bg(1,1), bg(1,2), bg(1,3) )
       !!
       !! DFT section
@@ -1100,17 +1091,15 @@
       CALL set_occupations( occupations, smearing, degauss, &
            lfixed, ltetra, tetra_type, lgauss, ngauss )
       IF (ltetra) ntetra = 6* nk1 * nk2 * nk3 
       IF (lfixed) CALL errore('read_file','bad occupancies',1)
       IF ( lsda ) &
            CALL set_nelup_neldw(tot_magnetization, nelec, nelup, neldw) 
       !! Symmetry section
-      if (lalloc) then
       ALLOCATE ( irt(48,nat) )
-      endif
       IF ( lvalid_input ) THEN 
          CALL qexsd_copy_symmetry ( output_obj%symmetries, &
               nsym, nrot, s, ft, sname, t_rev, invsym, irt, &
               noinv, nosym, no_t_rev, input_obj%symmetry_flags )
          
          CALL qexsd_copy_efield ( input_obj%electric_field, &
               tefield, dipfield, edir, emaxpos, eopreg, eamp, &
@@ -1128,39 +1117,37 @@
       CALL s_axis_to_cart()
       !! symmetry check - FIXME: is this needed?
       IF (nat > 0) CALL checkallsym( nat, tau, ityp)
       !! Algorithmic info
       do_cutoff_2D = (output_obj%boundary_conditions%assume_isolated == "2D")
       CALL qexsd_copy_algorithmic_info ( output_obj%algorithmic_info, &
            real_space, tqr, okvan, okpaw )
-      !qepy --> additional parameters
+      !qepy fix --> additional parameters
       dftd3_version   = output_obj%dft%vdW%dftd3_version
       dftd3_threebody = output_obj%dft%vdW%dftd3_threebody
       !vdw_econv_thr   = output_obj%dft%vdW%ts_vdw_econv_thr
       !!ts_vdw_econv_thr not in output but in input
       vdw_econv_thr   = input_obj%dft%vdW%ts_vdw_econv_thr
-      !qepy <-- additional parameters
+      !qepy fix <-- additional parameters
       !
       ! ... xml data no longer needed, can be discarded
       !
       CALL qes_reset  ( output_obj )
       CALL qes_reset  ( geninfo_obj )
       CALL qes_reset  ( parinfo_obj )
       IF ( TRIM(input_obj%tagname) == "input") CALL qes_reset ( input_obj) 
       !
       ! END OF READING VARIABLES FROM XML DATA FILE
       !
-      if (lalloc) then
       ALLOCATE( force ( 3, nat ) )
       ALLOCATE( extfor( 3, nat ) )
       IF ( tefield ) ALLOCATE( forcefield( 3, nat ) )
       IF ( gate ) ALLOCATE( forcegate( 3, nat ) )
-      endif
       !
-    END SUBROUTINE qepy_read_xml_file
+    END SUBROUTINE read_xml_file
     !
     !------------------------------------------------------------------------
     SUBROUTINE read_collected_wfc ( dirname, ik, evc )
       !------------------------------------------------------------------------
       !
       ! ... reads from directory "dirname" (new file format) for k-point "ik"
       ! ... wavefunctions from collected format into distributed array "evc"
@@ -1272,8 +1259,8 @@
       END IF
       !
       RETURN
       !
     END SUBROUTINE read_collected_wfc
     !
     !------------------------------------------------------------------------
-  END MODULE qepy_pw_restart_new
+  END MODULE pw_restart_new
```

### Comparing `qepy-0.0.2rc2/src/qe/qepy_pwscf.f90` & `qepy-0.0.3rc0/src/qe/qepy_pwscf.f90`

 * *Files 5% similar despite different names*

```diff
@@ -42,15 +42,15 @@
   USE mp_world,             ONLY : world_comm
   USE mp_pools,             ONLY : intra_pool_comm
   USE mp_bands,             ONLY : intra_bgrp_comm, inter_bgrp_comm
   USE mp_diag,              ONLY : mp_start_diag
   USE mp_exx,               ONLY : negrp
   USE read_input,           ONLY : read_input_file
   USE command_line_options, ONLY : input_file_, command_line, ndiag_
-  USE qepy_common,          ONLY : embed_base, messenger
+  USE qepy_common,          ONLY : embed_base, set_embed, messenger, p_embed => embed
   !
   IMPLICIT NONE
   !
   CHARACTER(len=*) :: infile
   INTEGER, INTENT(IN), OPTIONAL :: my_world_comm
   LOGICAL, INTENT(IN), OPTIONAL :: oldxml
   type(embed_base), intent(inout), optional :: embed
@@ -69,14 +69,16 @@
   !
   if (present(oldxml)) then
      oldver = oldxml
   else
      oldver = .FALSE.
   endif
   !
+  if (present(embed)) call set_embed(embed)
+  if (.not. associated(p_embed)) call set_embed(messenger)
   !
   IF ( PRESENT(my_world_comm)) THEN
      CALL mp_startup(my_world_comm=my_world_comm, start_images=.TRUE. )
   ELSE
      CALL mp_startup( start_images=.TRUE. )
   ENDIF
   !
@@ -127,46 +129,47 @@
      !CALL read_input_file('PW+iPi', input_file_ )
      !CALL run_driver( srvaddress, exit_status )
      !!
   !ENDIF
   !
   input_file_=trim(infile)
   CALL read_input_file( 'PW', input_file_ )
-  if (present(embed)) then
-     call qepy_run_pwscf(exit_status, oldver, embed)
-  else
-     call qepy_run_pwscf(exit_status, oldver, messenger)
-  endif
+  call qepy_run_pwscf(exit_status, oldver)
 END SUBROUTINE qepy_pwscf
    !
 SUBROUTINE qepy_pwscf_finalise()
    IMPLICIT NONE
    INTEGER :: exit_status
 
    CALL laxlib_free_ortho_group()
    CALL qepy_stop_run( exit_status )
    !CALL do_stop( exit_status )
 END SUBROUTINE qepy_pwscf_finalise
 
-SUBROUTINE qepy_initial(input)
+SUBROUTINE qepy_initial(input, embed)
   !
   USE io_global,   ONLY : ionode
   USE mp_global,   ONLY : mp_startup
   USE environment, ONLY : environment_start, environment_end
   USE qepy_common, ONLY : input_base
   USE io_files,    ONLY : tmp_dir, prefix
   USE check_stop,  ONLY : check_stop_init
+  USE qepy_common, ONLY : embed_base, set_embed, messenger, p_embed => embed
   !
   IMPLICIT NONE
   !
   TYPE(input_base), OPTIONAL :: input
+  type(embed_base), intent(inout), optional :: embed
   !
   LOGICAL            :: start_images = .false.
   !CHARACTER(len=256) :: code = 'QEPY'
   !
+  if (present(embed)) call set_embed(embed)
+  if (.not. associated(p_embed)) call set_embed(messenger)
+  !
   IF (PRESENT(input)) THEN
      start_images = input%start_images
   ENDIF
   !
   IF ( PRESENT(input)) THEN
      IF (input%my_world_comm /= 0 ) THEN
         CALL mp_startup(my_world_comm=input%my_world_comm, start_images=start_images )
@@ -180,15 +183,14 @@
   IF (PRESENT(input)) THEN
      prefix = input%prefix
      tmp_dir = input%tmp_dir
      CALL environment_start ( input%code )
   ENDIF
   !
   CALL check_stop_init()
-  !
 END SUBROUTINE qepy_initial
 
 SUBROUTINE qepy_finalise_end(input)
   !
   USE environment, ONLY : environment_start, environment_end
   USE qepy_common, ONLY : input_base
   USE mp_global,   ONLY : mp_global_end
```

### Comparing `qepy-0.0.2rc2/src/qe/qepy_read_file_new.f90` & `qepy-0.0.3rc0/src/fix/read_file_new.f90`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ! Copyright (C) 2016-2019 Quantum ESPRESSO group
 ! This file is distributed under the terms of the
 ! GNU General Public License. See the file `License'
 ! in the root directory of the present distribution,
 ! or http://www.gnu.org/copyleft/gpl.txt .
 !
 !----------------------------------------------------------------------------
-SUBROUTINE qepy_read_file()
+SUBROUTINE read_file()
   !----------------------------------------------------------------------------
   !
   ! Wrapper routine, for backwards compatibility
   !
   USE io_global,        ONLY : stdout
   USE control_flags,    ONLY : io_level
   USE buffers,          ONLY : open_buffer, close_buffer, save_buffer
@@ -23,15 +23,15 @@
   !
   IMPLICIT NONE
   !
   INTEGER :: ik
   LOGICAL :: exst, wfc_is_collected
   !
   wfc_is_collected = .true.
-  CALL qepy_read_file_new( wfc_is_collected )
+  CALL read_file_new( wfc_is_collected )
   !
   ! ... Open unit iunwfc, for Kohn-Sham orbitals - we assume that wfcs
   ! ... have been written to tmp_dir, not to a different directory!
   ! ... io_level = 1 so that a real file is opened
   !
   nwordwfc = nbnd*npwx*npol
   io_level = 1
@@ -49,57 +49,57 @@
      END DO
      !
   ELSE
      WRITE( stdout, '(5x,A)') &
           'read_file: Wavefunctions in collected format not available'
   END IF
   !
-  !CALL close_buffer  ( iunwfc, 'KEEP' )
+  CALL close_buffer  ( iunwfc, 'KEEP' )
   !
-END SUBROUTINE qepy_read_file
+END SUBROUTINE read_file
 !
 !----------------------------------------------------------------------------
-SUBROUTINE qepy_read_file_new ( needwf )
+SUBROUTINE read_file_new ( needwf )
   !----------------------------------------------------------------------------
   !
   ! Reads xml data file produced by pw.x or cp.x, performs initializations
   ! related to the contents of the xml file
   ! If needwf=.t. performs wavefunction-related initialization as well
   ! Does not read wfcs but returns in "wfc_is_collected" info on the wfc file
   !
   USE io_global,      ONLY : stdout
   USE io_files,       ONLY : nwordwfc, iunwfc, wfc_dir, tmp_dir, restart_dir
   USE gvect,          ONLY : ngm, g
   USE gvecw,          ONLY : gcutw
   USE klist,          ONLY : nkstot, nks, xk, wk
   USE lsda_mod,       ONLY : isk
   USE wvfct,          ONLY : nbnd, et, wg
-  USE qepy_pw_restart_new, ONLY : qepy_read_xml_file
+  USE pw_restart_new, ONLY : read_xml_file
   !
   IMPLICIT NONE
   !
   LOGICAL, INTENT(INOUT) :: needwf
   !
   LOGICAL :: wfc_is_collected
   !
   WRITE( stdout, '(/,5x,A)') &
        'Reading xml data from directory:', TRIM( restart_dir() )
   !
   ! ... Read the contents of the xml data file
   !
-  CALL qepy_read_xml_file ( wfc_is_collected )
+  CALL read_xml_file ( wfc_is_collected )
   !
   ! ... more initializations: pseudopotentials / G-vectors / FFT arrays /
   ! ... charge density / potential / ... , but not KS orbitals
   !
-  CALL qepy_post_xml_init ( )
+  CALL post_xml_init ( )
   !
   IF ( needwf ) THEN
      IF ( .NOT. wfc_is_collected ) WRITE( stdout, '(5x,A)') &
-          'qepy_read_file_new: Wavefunctions not in collected format?!?'
+          'read_file_new: Wavefunctions not in collected format?!?'
      !
      ! ... initialization of KS orbitals
      !
      wfc_dir = tmp_dir ! this is likely obsolete and no longer used
      !
      ! ... distribute across pools k-points and related variables.
      ! ... nks is defined by the following routine as the number 
@@ -113,17 +113,17 @@
      ! ... FIXME: the latter should be read from file, not recomputed
      !
      CALL allocate_wfc_k()
      !
   END IF
   needwf = wfc_is_collected
   !
-END SUBROUTINE qepy_read_file_new
+END SUBROUTINE read_file_new
 !----------------------------------------------------------------------------
-SUBROUTINE qepy_post_xml_init (  )
+SUBROUTINE post_xml_init (  )
   !----------------------------------------------------------------------------
   !
   ! ... Various initializations needed to start a calculation:
   ! ... pseudopotentials, G vectors, FFT arrays, rho, potential
   !
   USE kinds,                ONLY : DP
   USE io_global,            ONLY : stdout
@@ -156,15 +156,15 @@
   USE noncollin_module,     ONLY : noncolin
   USE spin_orb,             ONLY : lspinorb
   USE cell_base,            ONLY : at, bg, set_h_ainv
   USE symm_base,            ONLY : d1, d2, d3
   USE realus,               ONLY : betapointlist, generate_qpointlist, &
                                    init_realspace_vars,real_space
   !
-  !qepy --> import
+  !qepy fix --> import
   USE control_flags,        ONLY : mixing_beta, tr2, ethr, niter, nmix, &
                                    iprint, conv_elec, &
                                    restart, io_level, do_makov_payne,  &
                                    iverbosity, textfor,     &
                                    llondon, ldftd3, scf_must_converge, lxdm
   
   USE london_module,        ONLY : energy_london, init_london, C6_ij
@@ -173,24 +173,25 @@
                                    get_atomic_number, dftd3_input, &
                                    dftd3_calc
   USE dftd3_qe,             ONLY : dftd3, dftd3_in, energy_dftd3, dftd3_xc, dftd3_printout
   USE xdm_module,           ONLY : energy_xdm, init_xdm
   USE input_parameters,     ONLY : dftd3_threebody, dftd3_version
   USE funct,                ONLY : get_dft_short
   USE tsvdw_module,         ONLY : tsvdw_initialize
-  !qepy <-- import
+  USE funct,                ONLY : dft_is_meta
+  !qepy fix <-- import
   IMPLICIT NONE
   !
   INTEGER  :: inlc
   REAL(DP) :: ehart, etxc, vtxc, etotefield, charge
   CHARACTER(LEN=20) :: dft_name
-  !qepy --> variablesi
+  !qepy fix --> variables
   CHARACTER(LEN=256):: dft_
   REAL (DP), EXTERNAL :: get_clock
-  !qepy <-- variables
+  !qepy fix <-- variables
   !
   ! ... set G cutoffs and cell factor (FIXME: from setup.f90?)
   !
   CALL set_gcut()
   if (cell_factor == 0.d0) cell_factor = 1.D0
   nbndx = nbnd
   !
@@ -234,14 +235,19 @@
   ! ... read the charge density in G-space
   !
   CALL read_scf( rho, nspin, gamma_only )
   !
   ! ... bring the charge density to real space
   !
   CALL rho_g2r ( dfftp, rho%of_g, rho%of_r )
+  !qepy fix --> tau to real space
+  IF  ( dft_is_meta() ) THEN
+     CALL rho_g2r (dfftp, rho%kin_g, rho%kin_r)
+  ENDIF
+  !qepy fix <-- tau to real space
   !
   ! ... re-compute the local part of the pseudopotential vltot and
   ! ... the core correction charge (if any) - from hinit0.f90
   !
   CALL init_vloc()
   IF (tbeta_smoothing) CALL init_us_b0()
   IF (tq_smoothing) CALL init_us_0()
@@ -261,19 +267,19 @@
      CALL betapointlist()
      CALL init_realspace_vars()
      WRITE (stdout,'(5X,"Real space initialisation completed")')    
   ENDIF
   !
   ! ... recalculate the potential - FIXME: couldn't make ts-vdw work
   !
-  !qepy --> init vdw
+  !qepy fix --> init vdw
   IF ( ts_vdw) THEN
       CALL tsvdw_initialize()
       CALL set_h_ainv()
-     !CALL infomsg('qepy_read_file_new','*** vdW-TS term will be missing in potential ***')
+     !CALL infomsg('qepy fix_read_file_new','*** vdW-TS term will be missing in potential ***')
      !ts_vdw = .false.
   END IF
   !
   !IF ( llondon ) THEN
   !   IF ( .NOT. ALLOCATED(C6_ij)) CALL init_london()
   !ENDIF
   !IF (lxdm) THEN
@@ -287,15 +293,15 @@
      dftd3_in%threebody = dftd3_threebody
      CALL dftd3_init(dftd3, dftd3_in)
      CALL dftd3_printout(dftd3, dftd3_in)
      dft_ = get_dft_short( )
      dft_ = dftd3_xc ( dft_ )
      CALL dftd3_set_functional(dftd3, func=dft_, version=dftd3_version,tz=.false.)
   ENDIF
-  !qepy <-- init
+  !qepy fix <-- init vdw
   CALL v_of_rho( rho, rho_core, rhog_core, &
        ehart, etxc, vtxc, eth, etotefield, charge, v )
   !
   ! ... More PAW and USPP initializations
   !
   IF (okpaw) THEN
      becsum = rho%bec
@@ -334,8 +340,8 @@
          gcutms = 4.D0 * ecutwfc / tpiba2
       ELSE
          gcutms = gcutm
       END IF
       !
     END SUBROUTINE set_gcut
     !
-  END SUBROUTINE qepy_post_xml_init
+  END SUBROUTINE post_xml_init
```

### Comparing `qepy-0.0.2rc2/src/qe/qepy_run_pwscf.f90` & `qepy-0.0.3rc0/src/qe/qepy_run_pwscf.f90`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 ! Copyright (C) 2013-2017 Quantum ESPRESSO group
 ! This file is distributed under the terms of the
 ! GNU General Public License. See the file `License'
 ! in the root directory of the present distribution,
 ! or http://www.gnu.org/copyleft/gpl.txt .
 !
 !----------------------------------------------------------------------------
-SUBROUTINE qepy_run_pwscf( exit_status, oldxml, embed )
+SUBROUTINE qepy_run_pwscf( exit_status )
   !----------------------------------------------------------------------------
   !! Author: Paolo Giannozzi  
   !! License: GNU  
   !! Summary: Run an instance of the Plane Wave Self-Consistent Field code
   !
   !! Run an instance of the Plane Wave Self-Consistent Field code 
   !! MPI initialization and input data reading is performed in the 
@@ -50,15 +50,15 @@
   USE qmmm,                 ONLY : qmmm_initialization, qmmm_shutdown, &
                                    qmmm_update_positions, qmmm_update_forces
   USE qexsd_module,         ONLY : qexsd_set_status
   USE funct,                ONLY : dft_is_hybrid, stop_exx 
   USE mp_world, ONLY: world_comm
   !
   USE kinds,                ONLY : DP
-  USE qepy_common,          ONLY : embed_base
+  USE qepy_common,          ONLY : embed
   !
   IMPLICIT NONE
   !
   INTEGER, INTENT(OUT) :: exit_status
   !! Gives the exit status at the end
   !
   LOGICAL, EXTERNAL :: matches
@@ -69,25 +69,21 @@
   INTEGER :: idone 
   ! counter of electronic + ionic steps done in this run
   INTEGER :: ions_status = 3
   ! ions_status =  3  not yet converged
   ! ions_status =  2  converged, restart with nonzero magnetization
   ! ions_status =  1  converged, final step with current cell needed
   ! ions_status =  0  converged, exiting
-  LOGICAL, INTENT(IN), OPTIONAL :: oldxml
-  type(embed_base), intent(inout), optional :: embed
   !
   exit_status = 0
   IF ( ionode ) WRITE( UNIT = stdout, FMT = 9010 ) ntypx, npk, lmaxx
   !
   !qepy --> lmovecell
-  if (present(embed)) then
-     if (.not. lmovecell) then
-        lmovecell = embed%lmovecell
-     endif
+  if (.not. lmovecell) then
+     lmovecell = embed%lmovecell
   endif
   if (lmovecell) then
      if (cell_factor < 1.2d0 ) cell_factor = 2.d0
   endif
   !qepy <-- lmovecell
   IF (ionode) CALL plugin_arguments()
   CALL plugin_arguments_bcast( ionode_id, intra_image_comm )
@@ -133,31 +129,27 @@
      CALL qexsd_set_status(255)
      CALL punch( 'config-init' )
      exit_status = 255
      RETURN
   ENDIF
   !
   !CALL init_run()
-  if (present(oldxml)) then
-  CALL qepy_init_run(oldxml)
-  else
-  CALL qepy_init_run(.FALSE.)
-  endif
+  CALL qepy_init_run()
   !
   IF ( check_stop_now() ) THEN
      CALL qexsd_set_status( 255 )
      CALL punch( 'config' )
      exit_status = 255
      RETURN
   ENDIF
   exit_status = 255
-  !qepy -->
+  !qepy --> init force
   !fix: force allocate with NaN
   force=0.0_dp
-  !qepy <--
+  !qepy <-- init force
   !
   !main_loop: DO idone = 1, nstep
      !!
      !! ... electronic self-consistency or band structure calculation
      !!
      !IF ( .NOT. lscf) THEN
         !CALL non_scf()
```

### Comparing `qepy-0.0.2rc2/src/qe/qepy_setlocal.f90` & `qepy-0.0.3rc0/src/qe/qepy_setlocal.f90`

 * *Files 3% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 !
 !----------------------------------------------------------------------------
 ! TB
 ! setup of the gate, search for 'TB'
 !----------------------------------------------------------------------------
 !
 !----------------------------------------------------------------------
-SUBROUTINE qepy_setlocal(exttype)
+SUBROUTINE qepy_setlocal()
   !----------------------------------------------------------------------
   !! This routine computes the local potential in real space vltot(ir).
   !
   USE io_global,         ONLY : stdout
   USE kinds,             ONLY : DP
   USE constants,         ONLY : eps8
   USE ions_base,         ONLY : zv, ntyp => nsp
@@ -32,27 +32,26 @@
   USE mp_bands,          ONLY : intra_bgrp_comm
   USE mp,                ONLY : mp_sum
   USE martyna_tuckerman, ONLY : wg_corr_loc, do_comp_mt
   USE esm,               ONLY : esm_local, esm_bc, do_comp_esm
   USE qmmm,              ONLY : qmmm_add_esf
   USE Coul_cut_2D,       ONLY : do_cutoff_2D, cutoff_local 
   !
+  USE qepy_common,       ONLY : embed
+  !
   IMPLICIT NONE
   !
   COMPLEX(DP), ALLOCATABLE :: aux(:), v_corr(:)
   ! auxiliary variable
   INTEGER :: nt, ng
   ! counter on atom types
   ! counter on g vectors
-  integer, intent(in), optional      :: exttype
   logical              :: have = .true.
   !
-  if (present(exttype)) then
-     if (iand(exttype,1) == 1) have = .false.
-  endif
+  if (iand(embed%exttype,1) == 1) have = .false.
   !
   if (have) then
   ALLOCATE( aux(dfftp%nnr) )
   aux(:) = (0.d0,0.d0)
   !
   IF (do_comp_mt) THEN
      ALLOCATE( v_corr(ngm) )
```

### Comparing `qepy-0.0.2rc2/src/qe/qepy_stop_run.f90` & `qepy-0.0.3rc0/src/qe/qepy_stop_run.f90`

 * *Files 12% similar despite different names*

```diff
@@ -2,63 +2,14 @@
 ! Copyright (C) 2001-2009 Quantum ESPRESSO group
 ! This file is distributed under the terms of the
 ! GNU General Public License. See the file `License'
 ! in the root directory of the present distribution,
 ! or http://www.gnu.org/copyleft/gpl.txt .
 !
 !----------------------------------------------------------------------------
-!SUBROUTINE stop_run( exit_status )
-  !!----------------------------------------------------------------------------
-  !!! Close all files and synchronize processes before stopping:
-  !!
-  !!! * exit_status = 0: successfull execution, remove temporary files;
-  !!! * exit_status =-1: code stopped by user request;
-  !!! * exit_status = 1: convergence not achieved.
-  !!
-  !!! Do not remove temporary files needed for restart.
-  !!
-  !USE io_global,          ONLY : ionode
-  !USE mp_global,          ONLY : mp_global_end
-  !USE environment,        ONLY : environment_end
-  !USE io_files,           ONLY : iuntmp, seqopn
-  !!
-  !IMPLICIT NONE
-  !!
-  !INTEGER, INTENT(IN) :: exit_status
-  !LOGICAL             :: exst, opnd, lflag
-  !!
-  !lflag = ( exit_status == 0 ) 
-  !IF ( lflag ) THEN
-     !! 
-     !! ... remove files needed only to restart
-     !!
-     !CALL seqopn( iuntmp, 'restart', 'UNFORMATTED', exst )
-     !CLOSE( UNIT = iuntmp, STATUS = 'DELETE' )
-     !!
-     !IF ( ionode ) THEN
-        !CALL seqopn( iuntmp, 'update', 'FORMATTED', exst )
-        !CLOSE( UNIT = iuntmp, STATUS = 'DELETE' )
-        !CALL seqopn( iuntmp, 'para', 'FORMATTED', exst )
-        !CLOSE( UNIT = iuntmp, STATUS = 'DELETE' )
-     !ENDIF
-     !!
-  !ENDIF
-  !!
-  !CALL close_files( lflag )
-  !!
-  !CALL print_clock_pw()
-  !!
-  !CALL clean_pw( .TRUE. )
-  !!
-  !CALL environment_end( 'PWSCF' )
-  !!
-  !CALL mp_global_end()
-  !!
-!END SUBROUTINE stop_run
-
 SUBROUTINE qepy_stop_run( exit_status, print_flag, what, finalize )
   !----------------------------------------------------------------------------
   !! Close all files and synchronize processes before stopping:
   !
   !! * exit_status = 0: successfull execution, remove temporary files;
   !! * exit_status =-1: code stopped by user request;
   !! * exit_status = 1: convergence not achieved.
```

### Comparing `qepy-0.0.2rc2/src/qe/qepy_stress.f90` & `qepy-0.0.3rc0/src/qe/qepy_stress.f90`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ! This file is distributed under the terms of the
 ! GNU General Public License. See the file `License'
 ! in the root directory of the present distribution,
 ! or http://www.gnu.org/copyleft/gpl.txt .
 !
 !
 !----------------------------------------------------------------------
-SUBROUTINE qepy_stress(sigma, icalc, embed)
+SUBROUTINE qepy_stress(sigma, icalc)
   !----------------------------------------------------------------------
   !! Computes the total stress.
   !
   USE io_global,        ONLY : stdout
   USE kinds,            ONLY : DP
   USE cell_base,        ONLY : omega, alat, at, bg
   USE ions_base,        ONLY : nat, ntyp => nsp, ityp, tau, zv, atm
@@ -35,15 +35,15 @@
   USE exx,              ONLY : exx_stress
   USE funct,            ONLY : dft_is_hybrid
   USE tsvdw_module,     ONLY : HtsvdW
   USE ener,             ONLY : etot ! for ESM stress
   USE esm,              ONLY : do_comp_esm, esm_bc ! for ESM stress
   USE esm,              ONLY : esm_stres_har, esm_stres_ewa, esm_stres_loclong ! for ESM stress
   !
-  USE qepy_common,          ONLY : embed_base
+  USE qepy_common,      ONLY : embed
   !
   IMPLICIT NONE
   !
   REAL(DP), INTENT(OUT) :: sigma(3,3)
   !! The stress tensor
   !
   ! ... local variables
@@ -60,15 +60,14 @@
   !
   INTEGER  :: atnum(1:nat)
   REAL(DP) :: latvecs(3,3)
   REAL(DP) :: stress_dftd3(3,3)
   REAL(DP), ALLOCATABLE :: force_d3(:,:)
   !
   integer, intent(in), optional   :: icalc
-  type(embed_base),intent(inout),optional :: embed
   !
   integer                       :: calctype
   !
   if ( present(icalc) ) then
      calctype = icalc
   else
      calctype = 0
@@ -204,17 +203,15 @@
      sigmaexx = exx_stress()
      CALL symmatrix( sigmaexx )
      sigma(:,:) = sigma(:,:) + sigmaexx(:,:)
   ELSE
      sigmaexx = 0.d0
   ENDIF
   !qepy --> add extstress
-  if (present(embed)) then
-     sigma(:,:) = sigma(:,:) + embed%extstress
-  endif
+  sigma(:,:) = sigma(:,:) + embed%extstress
   !qepy <-- add extstress
   ! Resymmetrize the total stress. This should not be strictly necessary,
   ! but prevents loss of symmetry in long vc-bfgs runs
 
   CALL symmatrix( sigma )
   !
   ! write results in Ry/(a.u.)^3 and in kbar
```

### Comparing `qepy-0.0.2rc2/src/qe/qepy_v_of_rho.f90` & `qepy-0.0.3rc0/src/qe/qepy_v_of_rho.f90`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ! This file is distributed under the terms of the
 ! GNU General Public License. See the file `License'
 ! in the root directory of the present distribution,
 ! or http://www.gnu.org/copyleft/gpl.txt .
 !
 !----------------------------------------------------------------------------
 SUBROUTINE qepy_v_of_rho_all( rho, rho_core, rhog_core, &
-                     ehart, etxc, vtxc, eth, etotefield, charge, v, embed)
+                     ehart, etxc, vtxc, eth, etotefield, charge, v)
   !----------------------------------------------------------------------------
   !! This routine computes the Hartree and Exchange and Correlation
   !! potential and energies which corresponds to a given charge density
   !! The XC potential is computed in real space, while the
   !! Hartree potential is computed in reciprocal space.
   !
   USE kinds,            ONLY : DP
@@ -31,20 +31,18 @@
   USE plugin_variables,     ONLY : plugin_etot
   USE dfunct,               ONLY : newd
   USE paw_variables,        ONLY : okpaw, ddd_paw, total_core_energy, only_paw
   USE paw_onecenter,        ONLY : PAW_potential
   USE paw_symmetry,         ONLY : PAW_symmetrize_ddd
   USE ener,                 ONLY : epaw
   !
-  USE qepy_common,             ONLY : embed_base
+  USE qepy_common,          ONLY : embed
   !
   IMPLICIT NONE
   !
-  TYPE(embed_base), INTENT(INOUT)    :: embed
-  !
   TYPE(scf_type), INTENT(INOUT) :: rho
   !! the valence charge
   TYPE(scf_type), INTENT(INOUT) :: v
   !! the scf (Hxc) potential 
   !=================> NB: NOTE that in F90 derived data type must be INOUT and 
   !=================> not just OUT because otherwise their allocatable or pointer
   !=================> components are NOT defined 
@@ -67,28 +65,27 @@
   !
   INTEGER :: is, ir
   LOGICAL :: conv_elec
   REAL(DP) :: dr2
   REAL(DP) :: etot_cmp_paw(nat,2,2)
 
   call qepy_v_of_rho( rho, rho_core, rhog_core, &
-                     ehart, etxc, vtxc, eth, etotefield, charge, v, embed)
+                     ehart, etxc, vtxc, eth, etotefield, charge, v)
   IF (okpaw) THEN
      CALL PAW_potential( rho%bec, ddd_paw, epaw, etot_cmp_paw )
      CALL PAW_symmetrize_ddd( ddd_paw )
   ENDIF
 
   CALL plugin_scf_energy(plugin_etot,rho)
   !
   CALL plugin_scf_potential(rho,conv_elec,dr2,vltot)
   !
   ! ... define the total local potential (external + scf)
   !
-  CALL embed%allocate_extpot()
-  v%of_r = v%of_r + embed%extpot
+  IF (ALLOCATED(embed%extpot)) v%of_r = v%of_r + embed%extpot
   !
   CALL sum_vrs( dfftp%nnr, nspin, vltot, v%of_r, vrs )
   !
   ! ... interpolate the total local potential
   !
   CALL interpolate_vrs( dfftp%nnr, nspin, doublegrid, kedtau, v%kin_r, vrs )
   !
@@ -96,15 +93,15 @@
   ! ... term in the nonlocal potential
   ! ... PAW: newd contains PAW updates of NL coefficients
   !
   CALL newd()
   END SUBROUTINE 
 !----------------------------------------------------------------------------
 SUBROUTINE qepy_v_of_rho( rho, rho_core, rhog_core, &
-                     ehart, etxc, vtxc, eth, etotefield, charge, v, embed)
+                     ehart, etxc, vtxc, eth, etotefield, charge, v)
   !----------------------------------------------------------------------------
   !! This routine computes the Hartree and Exchange and Correlation
   !! potential and energies which corresponds to a given charge density
   !! The XC potential is computed in real space, while the
   !! Hartree potential is computed in reciprocal space.
   !
   USE kinds,            ONLY : DP
@@ -114,20 +111,18 @@
   USE ions_base,        ONLY : nat, tau
   USE ldaU,             ONLY : lda_plus_U 
   USE funct,            ONLY : dft_is_meta, get_meta
   USE scf,              ONLY : scf_type
   USE cell_base,        ONLY : alat
   USE control_flags,    ONLY : ts_vdw
   USE tsvdw_module,     ONLY : tsvdw_calculate, UtsvdW
-  USE qepy_common,         ONLY : embed_base
+  USE qepy_common,      ONLY : embed
   !
   IMPLICIT NONE
   !
-  type(embed_base), intent(in)    :: embed
-  !
   TYPE(scf_type), INTENT(INOUT) :: rho
   !! the valence charge
   TYPE(scf_type), INTENT(INOUT) :: v
   !! the scf (Hxc) potential 
   !=================> NB: NOTE that in F90 derived data type must be INOUT and 
   !=================> not just OUT because otherwise their allocatable or pointer
   !=================> components are NOT defined
```

### Comparing `qepy-0.0.2rc2/src/qe/qepy_wfcinit.f90` & `qepy-0.0.3rc0/src/fix/wfcinit.f90`

 * *Files 7% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ! This file is distributed under the terms of the
 ! GNU General Public License. See the file `License'
 ! in the root directory of the present distribution,
 ! or http://www.gnu.org/copyleft/gpl.txt .
 !
 !
 !----------------------------------------------------------------------------
-SUBROUTINE qepy_wfcinit(starting)
+SUBROUTINE wfcinit()
   !----------------------------------------------------------------------------
   !
   ! ... This routine computes an estimate of the starting wavefunctions
   ! ... from superposition of atomic wavefunctions and/or random wavefunctions.
   ! ... It also open needed files or memory buffers
   !
   USE io_global,            ONLY : stdout, ionode, ionode_id
@@ -39,19 +39,14 @@
   IMPLICIT NONE
   !
   INTEGER :: ik, ierr
   LOGICAL :: exst, exst_mem, exst_file, opnd_file, twfcollect_file = .FALSE.
   CHARACTER (LEN=256)  :: dirname
   TYPE ( output_type ) :: output_obj
   !
-  CHARACTER(LEN=*), INTENT(IN), OPTIONAL :: starting
-  !
-  IF (present(starting)) THEN
-     IF (len_trim(starting)>1) starting_wfc= trim(starting)
-  ENDIF
   !
   CALL start_clock( 'wfcinit' )
   !
   ! ... Orthogonalized atomic functions needed for LDA+U and other cases
   !
   IF ( use_wannier .OR. one_atom_occupations ) CALL orthoatwfc ( use_wannier )
   IF ( lda_plus_u ) CALL orthoUwfc()
@@ -160,185 +155,185 @@
      !
      IF ( nks > 1 .AND. lda_plus_u .AND. (U_projection .NE. 'pseudo') ) &
         CALL get_buffer( wfcU, nwordwfcU, iunhub, ik )
      !
      ! ... calculate starting wavefunctions (calls Hpsi)
      !
      CALL init_wfc ( ik )
-     !qepy --> lsda up==down
+     !qepy fix --> lsda up==down
      IF ( lsda .and. ik > nks/2) &
          CALL get_buffer ( evc, nwordwfc, iunwfc, ik-nks/2 )
-     !qepy <-- lsda up==down
+     !qepy fix <-- lsda up==down
      !
      ! ... write  starting wavefunctions to file
      !
      IF ( nks > 1 .OR. (io_level > 1) .OR. lelfield ) &
          CALL save_buffer ( evc, nwordwfc, iunwfc, ik )
      !
   END DO
   !
   CALL stop_clock( 'wfcinit' )
   RETURN
   !
-END SUBROUTINE qepy_wfcinit
+END SUBROUTINE wfcinit
 !
 !----------------------------------------------------------------------------
-!SUBROUTINE init_wfc ( ik )
-!  !----------------------------------------------------------------------------
-!  !
-!  ! ... This routine computes starting wavefunctions for k-point ik
-!  !
-!  USE kinds,                ONLY : DP
-!  USE bp,                   ONLY : lelfield
-!  USE becmod,               ONLY : allocate_bec_type, deallocate_bec_type, &
-!                                   bec_type, becp
-!  USE constants,            ONLY : tpi
-!  USE cell_base,            ONLY : tpiba2
-!  USE basis,                ONLY : natomwfc, starting_wfc
-!  USE gvect,                ONLY : g, gstart
-!  USE klist,                ONLY : xk, ngk, igk_k
-!  USE wvfct,                ONLY : nbnd, npwx, et
-!  USE uspp,                 ONLY : nkb, okvan
-!  USE noncollin_module,     ONLY : npol
-!  USE wavefunctions, ONLY : evc
-!  USE random_numbers,       ONLY : randy
-!  USE mp_bands,             ONLY : intra_bgrp_comm, inter_bgrp_comm, &
-!                                   nbgrp, root_bgrp_id
-!  USE mp,                   ONLY : mp_bcast
-!  USE funct,                ONLY : dft_is_hybrid, stop_exx
-!  !
-!  IMPLICIT NONE
-!  !
-!  INTEGER, INTENT(in) :: ik
-!  !
-!  INTEGER :: ibnd, ig, ipol, n_starting_wfc, n_starting_atomic_wfc
-!  LOGICAL :: lelfield_save
-!  !
-!  REAL(DP) :: rr, arg
-!  REAL(DP), ALLOCATABLE :: etatom(:) ! atomic eigenvalues
-!  !
-!  COMPLEX(DP), ALLOCATABLE :: wfcatom(:,:,:) ! atomic wfcs for initialization
-!  !
-!  !
-!  IF ( starting_wfc(1:6) == 'atomic' ) THEN
-!     !
-!     n_starting_wfc = MAX( natomwfc, nbnd )
-!     n_starting_atomic_wfc = natomwfc
-!     !
-!  ELSE IF ( starting_wfc == 'random' ) THEN
-!     !
-!     n_starting_wfc = nbnd
-!     n_starting_atomic_wfc = 0
-!     !
-!  ELSE
-!     !
-!     ! ...case 'file' should not be done here
-!     !
-!     CALL errore ( 'init_wfc', &
-!          'invalid value for startingwfc: ' // TRIM ( starting_wfc ) , 1 )
-!     !
-!  END IF
-!  !
-!  ALLOCATE( wfcatom( npwx, npol, n_starting_wfc ) )
-!  !
-!  IF ( starting_wfc(1:6) == 'atomic' ) THEN
-!     !
-!     CALL start_clock( 'wfcinit:atomic' ); !write(*,*) 'start wfcinit:atomic' ; FLUSH(6)
-!     CALL atomic_wfc( ik, wfcatom )
-!     CALL stop_clock( 'wfcinit:atomic' ); !write(*,*) 'stop wfcinit:atomic' ; FLUSH(6)
-!     !
-!     IF ( starting_wfc == 'atomic+random' .AND. &
-!         n_starting_wfc == n_starting_atomic_wfc ) THEN
-!         !
-!         ! ... in this case, introduce a small randomization of wavefunctions
-!         ! ... to prevent possible "loss of states"
-!         !
-!         DO ibnd = 1, n_starting_atomic_wfc
-!            !
-!            DO ipol = 1, npol
-!               !
-!               DO ig = 1, ngk(ik)
-!                  !
-!                  rr  = randy()
-!                  arg = tpi * randy()
-!                  !
-!                  wfcatom(ig,ipol,ibnd) = wfcatom(ig,ipol,ibnd) * &
-!                     ( 1.0_DP + 0.05_DP * CMPLX( rr*COS(arg), rr*SIN(arg) ,kind=DP) ) 
-!                  !
-!               END DO
-!               !
-!            END DO
-!            !
-!         END DO
-!         !
-!     END IF
-!     !
-!  END IF
-!  !
-!  ! ... if not enough atomic wfc are available,
-!  ! ... fill missing wfcs with random numbers
-!  !
-!  DO ibnd = n_starting_atomic_wfc + 1, n_starting_wfc
-!     !
-!     DO ipol = 1, npol
-!        ! 
-!        wfcatom(:,ipol,ibnd) = (0.0_dp, 0.0_dp)
-!        !
-!        DO ig = 1, ngk(ik)
-!           !
-!           rr  = randy()
-!           arg = tpi * randy()
-!           !
-!           wfcatom(ig,ipol,ibnd) = &
-!                CMPLX( rr*COS( arg ), rr*SIN( arg ) ,kind=DP) / &
-!                       ( ( xk(1,ik) + g(1,igk_k(ig,ik)) )**2 + &
-!                         ( xk(2,ik) + g(2,igk_k(ig,ik)) )**2 + &
-!                         ( xk(3,ik) + g(3,igk_k(ig,ik)) )**2 + 1.0_DP )
-!        END DO
-!        !
-!     END DO
-!     !
-!  END DO
+SUBROUTINE init_wfc ( ik )
+  !----------------------------------------------------------------------------
+  !
+  ! ... This routine computes starting wavefunctions for k-point ik
+  !
+  USE kinds,                ONLY : DP
+  USE bp,                   ONLY : lelfield
+  USE becmod,               ONLY : allocate_bec_type, deallocate_bec_type, &
+                                   bec_type, becp
+  USE constants,            ONLY : tpi
+  USE cell_base,            ONLY : tpiba2
+  USE basis,                ONLY : natomwfc, starting_wfc
+  USE gvect,                ONLY : g, gstart
+  USE klist,                ONLY : xk, ngk, igk_k
+  USE wvfct,                ONLY : nbnd, npwx, et
+  USE uspp,                 ONLY : nkb, okvan
+  USE noncollin_module,     ONLY : npol
+  USE wavefunctions, ONLY : evc
+  USE random_numbers,       ONLY : randy
+  USE mp_bands,             ONLY : intra_bgrp_comm, inter_bgrp_comm, &
+                                   nbgrp, root_bgrp_id
+  USE mp,                   ONLY : mp_bcast
+  USE funct,                ONLY : dft_is_hybrid, stop_exx
+  !
+  IMPLICIT NONE
+  !
+  INTEGER, INTENT(in) :: ik
+  !
+  INTEGER :: ibnd, ig, ipol, n_starting_wfc, n_starting_atomic_wfc
+  LOGICAL :: lelfield_save
+  !
+  REAL(DP) :: rr, arg
+  REAL(DP), ALLOCATABLE :: etatom(:) ! atomic eigenvalues
+  !
+  COMPLEX(DP), ALLOCATABLE :: wfcatom(:,:,:) ! atomic wfcs for initialization
+  !
+  !
+  IF ( starting_wfc(1:6) == 'atomic' ) THEN
+     !
+     n_starting_wfc = MAX( natomwfc, nbnd )
+     n_starting_atomic_wfc = natomwfc
+     !
+  ELSE IF ( starting_wfc == 'random' ) THEN
+     !
+     n_starting_wfc = nbnd
+     n_starting_atomic_wfc = 0
+     !
+  ELSE
+     !
+     ! ...case 'file' should not be done here
+     !
+     CALL errore ( 'init_wfc', &
+          'invalid value for startingwfc: ' // TRIM ( starting_wfc ) , 1 )
+     !
+  END IF
+  !
+  ALLOCATE( wfcatom( npwx, npol, n_starting_wfc ) )
+  !
+  IF ( starting_wfc(1:6) == 'atomic' ) THEN
+     !
+     CALL start_clock( 'wfcinit:atomic' ); !write(*,*) 'start wfcinit:atomic' ; FLUSH(6)
+     CALL atomic_wfc( ik, wfcatom )
+     CALL stop_clock( 'wfcinit:atomic' ); !write(*,*) 'stop wfcinit:atomic' ; FLUSH(6)
+     !
+     IF ( starting_wfc == 'atomic+random' .AND. &
+         n_starting_wfc == n_starting_atomic_wfc ) THEN
+         !
+         ! ... in this case, introduce a small randomization of wavefunctions
+         ! ... to prevent possible "loss of states"
+         !
+         DO ibnd = 1, n_starting_atomic_wfc
+            !
+            DO ipol = 1, npol
+               !
+               DO ig = 1, ngk(ik)
+                  !
+                  rr  = randy()
+                  arg = tpi * randy()
+                  !
+                  wfcatom(ig,ipol,ibnd) = wfcatom(ig,ipol,ibnd) * &
+                     ( 1.0_DP + 0.05_DP * CMPLX( rr*COS(arg), rr*SIN(arg) ,kind=DP) ) 
+                  !
+               END DO
+               !
+            END DO
+            !
+         END DO
+         !
+     END IF
+     !
+  END IF
+  !
+  ! ... if not enough atomic wfc are available,
+  ! ... fill missing wfcs with random numbers
+  !
+  DO ibnd = n_starting_atomic_wfc + 1, n_starting_wfc
+     !
+     DO ipol = 1, npol
+        ! 
+        wfcatom(:,ipol,ibnd) = (0.0_dp, 0.0_dp)
+        !
+        DO ig = 1, ngk(ik)
+           !
+           rr  = randy()
+           arg = tpi * randy()
+           !
+           wfcatom(ig,ipol,ibnd) = &
+                CMPLX( rr*COS( arg ), rr*SIN( arg ) ,kind=DP) / &
+                       ( ( xk(1,ik) + g(1,igk_k(ig,ik)) )**2 + &
+                         ( xk(2,ik) + g(2,igk_k(ig,ik)) )**2 + &
+                         ( xk(3,ik) + g(3,igk_k(ig,ik)) )**2 + 1.0_DP )
+        END DO
+        !
+     END DO
+     !
+  END DO
   
-!  ! when band parallelization is active, the first band group distributes
-!  ! the wfcs to the others making sure all bgrp have the same starting wfc
-!  ! FIXME: maybe this should be done once evc are computed, not here?
-!  !
-!  IF( nbgrp > 1 ) CALL mp_bcast( wfcatom, root_bgrp_id, inter_bgrp_comm )
-!  !
-!  ! ... Diagonalize the Hamiltonian on the basis of atomic wfcs
-!  !
-!  ALLOCATE( etatom( n_starting_wfc ) )
-!  !
-!  ! ... Allocate space for <beta|psi>
-!  !
-!  CALL allocate_bec_type ( nkb, n_starting_wfc, becp, intra_bgrp_comm )
-!  !
-!  ! ... the following trick is for electric fields with Berry's phase:
-!  ! ... by setting lelfield = .false. one prevents the calculation of
-!  ! ... electric enthalpy in the Hamiltonian (cannot be calculated
-!  ! ... at this stage: wavefunctions at previous step are missing)
-!  ! 
-!  lelfield_save = lelfield
-!  lelfield = .FALSE.
-!  !
-!  ! ... subspace diagonalization (calls Hpsi)
-!  !
-!  IF ( dft_is_hybrid()  ) CALL stop_exx() 
-!  CALL start_clock( 'wfcinit:wfcrot' ); !write(*,*) 'start wfcinit:wfcrot' ; FLUSH(6)
-!  CALL rotate_wfc ( npwx, ngk(ik), n_starting_wfc, gstart, nbnd, wfcatom, npol, okvan, evc, etatom )
-!  CALL stop_clock( 'wfcinit:wfcrot' ); !write(*,*) 'stop wfcinit:wfcrot' ; FLUSH(6)
-!  !
-!  lelfield = lelfield_save
-!  !
-!  ! ... copy the first nbnd eigenvalues
-!  ! ... eigenvectors are already copied inside routine rotate_wfc
-!  !
-!  et(1:nbnd,ik) = etatom(1:nbnd)
-!  !
-!  CALL deallocate_bec_type ( becp )
-!  DEALLOCATE( etatom )
-!  DEALLOCATE( wfcatom )
-!  !
-!  RETURN
-!  !
-!END SUBROUTINE init_wfc
+  ! when band parallelization is active, the first band group distributes
+  ! the wfcs to the others making sure all bgrp have the same starting wfc
+  ! FIXME: maybe this should be done once evc are computed, not here?
+  !
+  IF( nbgrp > 1 ) CALL mp_bcast( wfcatom, root_bgrp_id, inter_bgrp_comm )
+  !
+  ! ... Diagonalize the Hamiltonian on the basis of atomic wfcs
+  !
+  ALLOCATE( etatom( n_starting_wfc ) )
+  !
+  ! ... Allocate space for <beta|psi>
+  !
+  CALL allocate_bec_type ( nkb, n_starting_wfc, becp, intra_bgrp_comm )
+  !
+  ! ... the following trick is for electric fields with Berry's phase:
+  ! ... by setting lelfield = .false. one prevents the calculation of
+  ! ... electric enthalpy in the Hamiltonian (cannot be calculated
+  ! ... at this stage: wavefunctions at previous step are missing)
+  ! 
+  lelfield_save = lelfield
+  lelfield = .FALSE.
+  !
+  ! ... subspace diagonalization (calls Hpsi)
+  !
+  IF ( dft_is_hybrid()  ) CALL stop_exx() 
+  CALL start_clock( 'wfcinit:wfcrot' ); !write(*,*) 'start wfcinit:wfcrot' ; FLUSH(6)
+  CALL rotate_wfc ( npwx, ngk(ik), n_starting_wfc, gstart, nbnd, wfcatom, npol, okvan, evc, etatom )
+  CALL stop_clock( 'wfcinit:wfcrot' ); !write(*,*) 'stop wfcinit:wfcrot' ; FLUSH(6)
+  !
+  lelfield = lelfield_save
+  !
+  ! ... copy the first nbnd eigenvalues
+  ! ... eigenvectors are already copied inside routine rotate_wfc
+  !
+  et(1:nbnd,ik) = etatom(1:nbnd)
+  !
+  CALL deallocate_bec_type ( becp )
+  DEALLOCATE( etatom )
+  DEALLOCATE( wfcatom )
+  !
+  RETURN
+  !
+END SUBROUTINE init_wfc
```

### Comparing `qepy-0.0.2rc2/src/tddft/qepy_molecule_optical_absorption.f90` & `qepy-0.0.3rc0/src/tddft/qepy_molecule_optical_absorption.f90`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ! This file is distributed under the terms of the
 ! GNU General Public License. See the file `License'
 ! in the root directory of the present distribution,
 ! or http://www.gnu.org/copyleft/gpl.txt .
 !
 
 !-----------------------------------------------------------------------
-subroutine qepy_molecule_optical_absorption(embed)
+subroutine qepy_molecule_optical_absorption()
   !----------------------------------------------------------------------
   !  ... Compute optical absorption spectrum by real-time TDDFT 
   !  ... References:
   !      (1) Phys. Rev. B 73, 035408 (2006)
   !      (2) http://www.netlib.org/linalg/html_templates/Templates.html
   !                                             Xiaofeng Qian, MIT (2008)
   !----------------------------------------------------------------------
@@ -33,15 +33,15 @@
   USE buffers,                     ONLY : get_buffer, save_buffer
   USE fixed_occ,                   ONLY : tfixed_occ 
   USE uspp,                        ONLY : nkb, vkb
   USE dynamics_module,             ONLY : vel, verlet, allocate_dyn_vars, deallocate_dyn_vars
   USE pwcom
   USE tddft_module
   !
-  USE qepy_common,             ONLY : embed_base
+  USE qepy_common,             ONLY : embed
   USE qepy_tddft_common,       ONLY : tddft_psi, b, &
                                       tddft_hpsi, tddft_spsi, &
                                       tddft_Ppsi, &
                                       charge, dipole, quadrupole, &
                                       circular, circular_local
   USE uspp,                    ONLY : nkb, vkb, okvan
   !
@@ -58,15 +58,14 @@
   integer :: ik, is, ibnd
   complex(dp),save :: ee                     ! i*dt/2
   real(dp),save :: anorm, wclock
   integer, external :: find_free_unit
   real(dp), external :: get_clock
   external tddft_ch_psi_all
   !
-  TYPE(embed_base), INTENT(INOUT)    :: embed
   INTEGER :: iter
   !
   INTEGER :: iuntemp ! unit for swap
 
   ! TODO: restart
   IF (embed%tddft%finish) goto 111
   IF (embed%tddft%initial) THEN
@@ -105,15 +104,15 @@
      !qepy <--
      ! replace the iunwfc with iunevcn for sum_band
      iuntemp = iunwfc
      iunwfc = iunevcn
      if (okvan .and. is_allocated_bec_type(becp)) call deallocate_bec_type(becp)
      call sum_band()
      !qepy -->
-     call qepy_update_hamiltonian(-1, embed)
+     call qepy_update_hamiltonian(-1)
      iunwfc = iuntemp
  
      if (iverbosity > 0) write(stdout,'(5X,''Done with restart'')')
   else
      embed%tddft%istep = 0
   endif
```

### Comparing `qepy-0.0.2rc2/src/tddft/qepy_tddft_common.f90` & `qepy-0.0.3rc0/src/tddft/qepy_tddft_common.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/src/tddft/qepy_tddft_main.f90` & `qepy-0.0.3rc0/src/tddft/qepy_tddft_main.f90`

 * *Files 7% similar despite different names*

```diff
@@ -3,26 +3,26 @@
 ! This file is distributed under the terms of the
 ! GNU General Public License. See the file `License'
 ! in the root directory of the present distribution,
 ! or http://www.gnu.org/copyleft/gpl.txt .
 !
 
 !-----------------------------------------------------------------------
-!PROGRAM tddft_main
-SUBROUTINE qepy_tddft_main_initial(infile, my_world_comm)
+SUBROUTINE qepy_tddft_main_initial(infile, my_world_comm, embed)
   !-----------------------------------------------------------------------
   !
   ! ... This is the main driver of the real time TDDFT propagation.
   ! ... Authors: Xiaofeng Qian and Davide Ceresoli
   ! ...
   ! ... References:
   ! ...   Xiaofeng Qian, Ju Li, Xi Lin, and Sidney Yip, PRB 73, 035408 (2006)
   ! ...
   USE kinds,           ONLY : DP
   USE io_global,       ONLY : stdout, meta_ionode, meta_ionode_id
+  !USE mp,              ONLY : mp_bcast
   USE tddft_module,    ONLY : job, molecule, max_seconds
   USE check_stop,      ONLY : check_stop_init
   USE control_flags,   ONLY : io_level, gamma_only, use_para_diag
   USE mp_global,       ONLY : mp_startup
   USE mp_bands,        ONLY : nbgrp
   USE mp_world,        ONLY : world_comm
   USE environment,     ONLY : environment_start, environment_end
@@ -32,25 +32,31 @@
   ! for pluginization
   USE input_parameters, ONLY : nat_ => nat, ntyp_ => ntyp
   USE input_parameters, ONLY : assume_isolated_ => assume_isolated, &
                                ibrav_ => ibrav
   USE ions_base,        ONLY : nat, ntyp => nsp
   USE cell_base,        ONLY : ibrav
   !USE tddft_version
+  USE qepy_common,      ONLY : embed_base, set_embed, messenger, p_embed => embed
   USE iotk_module  
   !------------------------------------------------------------------------
   IMPLICIT NONE
   CHARACTER (LEN=9)   :: code = 'TDDFT'
   LOGICAL, EXTERNAL  :: check_para_diag
   !
   CHARACTER(len=*) :: infile
   INTEGER, INTENT(IN), OPTIONAL :: my_world_comm
+  type(embed_base), intent(inout), optional :: embed
   !------------------------------------------------------------------------
 
   ! begin with the initialization part
+  !
+  if (present(embed)) call set_embed(embed)
+  if (.not. associated(p_embed)) call set_embed(messenger)
+  !
 #ifdef __MPI
   IF ( PRESENT(my_world_comm)) THEN
      CALL mp_startup(my_world_comm=my_world_comm, start_images=.TRUE. )
   ELSE
      CALL mp_startup( start_images=.TRUE. )
   ENDIF
 #else
@@ -79,19 +85,19 @@
   write(stdout,*)
 
   call qepy_tddft_readin(infile)
   !call check_stop_init( max_seconds )
 
   io_level = 1
  
-  !! read ground state wavefunctions
+  ! read ground state wavefunctions
   !call read_file
 END SUBROUTINE qepy_tddft_main_initial
 !
-SUBROUTINE qepy_tddft_main_setup(embed)
+SUBROUTINE qepy_tddft_main_setup()
   !-----------------------------------------------------------------------
   !
   ! ... This is the main driver of the real time TDDFT propagation.
   ! ... Authors: Xiaofeng Qian and Davide Ceresoli
   ! ...
   ! ... References:
   ! ...   Xiaofeng Qian, Ju Li, Xi Lin, and Sidney Yip, PRB 73, 035408 (2006)
@@ -114,22 +120,19 @@
   USE input_parameters, ONLY : assume_isolated_ => assume_isolated, &
                                ibrav_ => ibrav
   USE ions_base,        ONLY : nat, ntyp => nsp
   USE cell_base,        ONLY : ibrav
   !USE tddft_version
   USE iotk_module  
   !
-  USE qepy_common,             ONLY : embed_base
-  !
   !------------------------------------------------------------------------
   IMPLICIT NONE
   CHARACTER (LEN=9)   :: code = 'TDDFT'
   LOGICAL, EXTERNAL  :: check_para_diag
   !
-  TYPE(embed_base), INTENT(INOUT)    :: embed
   !------------------------------------------------------------------------
 #ifdef __MPI
   use_para_diag = check_para_diag(nbnd)
 #else
   use_para_diag = .false.
 #endif
 
@@ -146,26 +149,26 @@
 
   nat_ = nat
   ntyp_ = ntyp
   ibrav_ = ibrav
   assume_isolated_ = 'none'
   call plugin_read_input()
   call qepy_tddft_allocate()
-  call qepy_tddft_setup(embed)
+  call qepy_tddft_setup()
   call tddft_summary()
 
 #ifdef __BANDS
   call init_parallel_over_band(inter_bgrp_comm, nbnd)
 #endif
 
   ! calculation
   !select case (trim(job))
   !case ('optical')
   !   if (molecule) then
-  !      call qepy_molecule_optical_absorption(embed)
+  !      call qepy_molecule_optical_absorption()
   !   else
   !      call errore('tddft_main', 'solids are not yet implemented', 1)
   !   endif
 
   !case default
   !   call errore('tddft_main', 'wrong or undefined job in input', 1)
 
@@ -191,10 +194,10 @@
   call qepy_tddft_closefil
   IF ( iprint > 0 .and. iprint<10 ) THEN
   call print_clock_tddft
   call environment_end(code)
   ENDIF
   !call stop_code( .true. )
   !STOP
+
 END SUBROUTINE qepy_stop_tddft
 
-!END PROGRAM tddft_main
```

### Comparing `qepy-0.0.2rc2/src/tddft/qepy_tddft_mod.f90` & `qepy-0.0.3rc0/src/tddft/qepy_tddft_mod.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/src/tddft/qepy_tddft_routines.f90` & `qepy-0.0.3rc0/src/tddft/qepy_tddft_routines.f90`

 * *Files identical despite different names*

### Comparing `qepy-0.0.2rc2/src/tddft/qepy_tddft_setup.f90` & `qepy-0.0.3rc0/src/tddft/qepy_tddft_setup.f90`

 * *Files 10% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ! This file is distributed under the terms of the
 ! GNU General Public License. See the file `License'
 ! in the root directory of the present distribution,
 ! or http://www.gnu.org/copyleft/gpl.txt .
 !
 
 !-----------------------------------------------------------------------
-SUBROUTINE qepy_tddft_setup(embed)
+SUBROUTINE qepy_tddft_setup
   !-----------------------------------------------------------------------
   !
   ! ... TDDFT setup
   !
   USE kinds,         ONLY : dp
   USE io_global,     ONLY : stdout
   USE wvfct,         ONLY : nbnd, et, wg
@@ -26,33 +26,29 @@
   USE mp_pools,      ONLY : inter_pool_comm 
   USE mp,            ONLY : mp_max, mp_min 
   USE dfunct,        ONLY : newd
   USE pwcom,         ONLY : ef
   USE constants,     ONLY : rytoev
   USE tddft_module
   !
-  USE qepy_common,             ONLY : embed_base
+  USE qepy_common,             ONLY : embed
   !
 
   implicit none
   integer :: ik, ibnd
   real(dp) :: emin, emax, xmax, small, fac, target
-  !
-  TYPE(embed_base), INTENT(INOUT)    :: embed
-  !
     
   call start_clock ('tddft_setup')
     
   ! initialize pseudopotentials and projectors for LDA+U
   call init_us_1
   call init_at_1
 
   ! computes the total local potential (external+scf) on the smooth grid
-  !call setlocal
-  call qepy_setlocal(embed%exttype)
+  call qepy_setlocal()
   call set_vrs (vrs, vltot, v%of_r, kedtau, v%kin_r, dfftp%nnr, nspin, doublegrid)
     
   ! compute the D for the pseudopotentials
   call newd
     
   !! set non linear core correction stuff (IS THIS REALLY NEEDED?)
   !! nlcc_any = ANY ( upf(1:ntyp)%nlcc )
@@ -146,14 +142,14 @@
 
   ! wavepacket
   if (wavepacket) then
      call setup_wavepacket
   endif
 
   ! initialize hamiltonian
-  call qepy_update_hamiltonian(-1, embed)
+  call qepy_update_hamiltonian(-1)
 
   call stop_clock('tddft_setup')
   
 END SUBROUTINE qepy_tddft_setup
```

### Comparing `qepy-0.0.2rc2/src/tddft/qepy_update_ham.f90` & `qepy-0.0.3rc0/src/tddft/qepy_update_ham.f90`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 ! This file is distributed under the terms of the
 ! GNU General Public License. See the file `License'
 ! in the root directory of the present distribution,
 ! or http://www.gnu.org/copyleft/gpl.txt .
 !
 
 !-----------------------------------------------------------------------
-SUBROUTINE qepy_update_hamiltonian(istep, embed)
+SUBROUTINE qepy_update_hamiltonian(istep)
   !-----------------------------------------------------------------------
   !
   ! ... Update the hamiltonian
   !
   USE kinds,         ONLY : dp
   USE ldaU,          ONLY : lda_plus_U
   USE scf,           ONLY : rho, rho_core, rhog_core, vltot, v, kedtau, vrs
@@ -29,23 +29,20 @@
   USE gvect,         ONLY : ngm, gstart, g, gg, gcutm
   USE control_flags, ONLY : gamma_only
   USE becmod,        ONLY : becp, calbec, allocate_bec_type, &
                             is_allocated_bec_type, deallocate_bec_type
   USE uspp,          ONLY : nkb
   USE pwcom
   !
-  USE qepy_common,             ONLY : embed_base
+  USE qepy_common,             ONLY : embed
   !
   implicit none
   integer, intent(in) :: istep
   real(dp) :: charge, eth, etotefield
   real(dp), external :: ewald, delta_eband
-  !
-  TYPE(embed_base), INTENT(INOUT)    :: embed
-  !
 
   call start_clock('updateH')
   
   ! calculate total charge density
   !rho%of_g(:,:) = (0.d0,0.d0)
   !rho%of_r(:,:) = 0.d0
   !call sum_band()
@@ -53,24 +50,22 @@
 
   if (lda_plus_U) then
     call new_ns
     if (iverbosity > 10) call write_ns()
   end if
     
   ! calculate HXC-potential
-  !call v_of_rho( rho, rho_core, rhog_core, ehart, etxc, vtxc, eth, etotefield, charge, v )
-  call qepy_v_of_rho( rho, rho_core, rhog_core, ehart, etxc, vtxc, eth, etotefield, charge, v, embed)
+  call qepy_v_of_rho( rho, rho_core, rhog_core, ehart, etxc, vtxc, eth, etotefield, charge, v)
     
   ! calculate total local potential (external + scf)
   !call setlocal
   !call set_vrs(vrs, vltot, v%of_r, kedtau, v%kin_r, dfftp%nnr, nspin, doublegrid)    
-  call qepy_setlocal(embed%exttype)
+  call qepy_setlocal()
   !
-  call embed%allocate_extpot()
-  v%of_r = v%of_r + embed%extpot
+  IF (ALLOCATED(embed%extpot)) v%of_r = v%of_r + embed%extpot
   !
   CALL sum_vrs( dfftp%nnr, nspin, vltot, v%of_r, vrs )
   !
   ! ... interpolate the total local potential
   !
   CALL interpolate_vrs( dfftp%nnr, nspin, doublegrid, kedtau, v%kin_r, vrs )
```

