# Comparing `tmp/gradio_tools-0.0.5.tar.gz` & `tmp/gradio_tools-0.0.6.tar.gz`

## Comparing `gradio_tools-0.0.5.tar` & `gradio_tools-0.0.6.tar`

### file list

```diff
@@ -1,98 +1,143 @@
--rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/.DS_Store
--rw-r--r--   0        0        0     6679 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/README.md
--rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/temp.log
--rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/.ruff_cache/.gitignore
--rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/.ruff_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/162952a0-7147-4f52-ab58-f852bc5c0561/captions.json
--rw-r--r--   0        0        0   109150 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/162952a0-7147-4f52-ab58-f852bc5c0561/tmp09966smi.jpg
--rw-r--r--   0        0        0    79996 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/162952a0-7147-4f52-ab58-f852bc5c0561/tmpf213r3ou.jpg
--rw-r--r--   0        0        0    99128 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/162952a0-7147-4f52-ab58-f852bc5c0561/tmpjpgr84co.jpg
--rw-r--r--   0        0        0   101966 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/162952a0-7147-4f52-ab58-f852bc5c0561/tmpo84_x1ra.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/330d40a3-cc6a-41ce-96c2-002bc67df326/captions.json
--rw-r--r--   0        0        0   105846 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpj7ygzwvr.jpg
--rw-r--r--   0        0        0   126760 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpqdvz5be9.jpg
--rw-r--r--   0        0        0   119178 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/330d40a3-cc6a-41ce-96c2-002bc67df326/tmprmxi0obh.jpg
--rw-r--r--   0        0        0   108581 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpyo33vqhb.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/captions.json
--rw-r--r--   0        0        0    99607 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmp26bprpby.jpg
--rw-r--r--   0        0        0   131260 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmp5u2z8292.jpg
--rw-r--r--   0        0        0   116900 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmpmdu7tfxc.jpg
--rw-r--r--   0        0        0    80104 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmpy8rnr6lx.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/508529be-bc20-48b9-b0b7-003e7a21db62/captions.json
--rw-r--r--   0        0        0   122753 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/508529be-bc20-48b9-b0b7-003e7a21db62/tmp1rbaj9ih.jpg
--rw-r--r--   0        0        0    86812 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/508529be-bc20-48b9-b0b7-003e7a21db62/tmpgo3ghi7z.jpg
--rw-r--r--   0        0        0   105885 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/508529be-bc20-48b9-b0b7-003e7a21db62/tmpppnjp9oh.jpg
--rw-r--r--   0        0        0   117917 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/508529be-bc20-48b9-b0b7-003e7a21db62/tmpvgae85c7.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/captions.json
--rw-r--r--   0        0        0   106965 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpmsy7r5s4.jpg
--rw-r--r--   0        0        0   126635 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpotr65fvw.jpg
--rw-r--r--   0        0        0   103678 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpr4__qxcx.jpg
--rw-r--r--   0        0        0    94221 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpx4p7b1ft.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/6a6c3f15-5217-462c-9d28-39f1b2f07676/captions.json
--rw-r--r--   0        0        0   135053 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmpj6tqr3fx.jpg
--rw-r--r--   0        0        0   108105 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmpodtfruna.jpg
--rw-r--r--   0        0        0   137541 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmppg3kuayo.jpg
--rw-r--r--   0        0        0   103154 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmps600nxhc.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/70a06453-f83c-4866-89a1-d8f5c9a052d7/captions.json
--rw-r--r--   0        0        0    77205 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpjnq5cw1k.jpg
--rw-r--r--   0        0        0    92290 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmps6bqlq3v.jpg
--rw-r--r--   0        0        0   120803 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpvhwji69q.jpg
--rw-r--r--   0        0        0    89928 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpxap7ybtb.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/75c113a2-7d4f-4f14-abe9-23259df50dfb/captions.json
--rw-r--r--   0        0        0    96910 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmp9wfer_02.jpg
--rw-r--r--   0        0        0    81978 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpiyhb0oay.jpg
--rw-r--r--   0        0        0   112268 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpluez_al7.jpg
--rw-r--r--   0        0        0    78187 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpp4qnbcqi.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/captions.json
--rw-r--r--   0        0        0    93851 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmp74tk8cfs.jpg
--rw-r--r--   0        0        0   115711 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpk_wbbklr.jpg
--rw-r--r--   0        0        0    89571 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpvufkgo26.jpg
--rw-r--r--   0        0        0   112338 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpz6lir7im.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/aa3ee281-8672-4993-bb3e-09335e1de70e/captions.json
--rw-r--r--   0        0        0   122186 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/aa3ee281-8672-4993-bb3e-09335e1de70e/tmp4i1fupac.jpg
--rw-r--r--   0        0        0    93863 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/aa3ee281-8672-4993-bb3e-09335e1de70e/tmp9px6fa06.jpg
--rw-r--r--   0        0        0   121362 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/aa3ee281-8672-4993-bb3e-09335e1de70e/tmpceochm5g.jpg
--rw-r--r--   0        0        0    80154 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/aa3ee281-8672-4993-bb3e-09335e1de70e/tmpqjthh1r6.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/aa9874d1-dc09-4c04-bf37-55c556e61e83/captions.json
--rw-r--r--   0        0        0   111564 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmp5myeybsm.jpg
--rw-r--r--   0        0        0    98332 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmpd3ufb_2o.jpg
--rw-r--r--   0        0        0   112096 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmpdlfj8cj_.jpg
--rw-r--r--   0        0        0   109146 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmps0tx8a8q.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/ac2f6e03-9430-4c22-a559-354225a49357/captions.json
--rw-r--r--   0        0        0    79381 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/ac2f6e03-9430-4c22-a559-354225a49357/tmp2ye34bli.jpg
--rw-r--r--   0        0        0   105896 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/ac2f6e03-9430-4c22-a559-354225a49357/tmp5ufb0844.jpg
--rw-r--r--   0        0        0    92696 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/ac2f6e03-9430-4c22-a559-354225a49357/tmp_h1cp6t2.jpg
--rw-r--r--   0        0        0   112587 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/ac2f6e03-9430-4c22-a559-354225a49357/tmpvqywwmzc.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/captions.json
--rw-r--r--   0        0        0    93651 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmp7n9_771q.jpg
--rw-r--r--   0        0        0    83077 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpgaejg5rz.jpg
--rw-r--r--   0        0        0   101925 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpl3n0u99v.jpg
--rw-r--r--   0        0        0   122576 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpuylgwvrf.jpg
--rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/captions.json
--rw-r--r--   0        0        0    99572 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmphp1_2bwe.jpg
--rw-r--r--   0        0        0   115349 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmplv4pugrr.jpg
--rw-r--r--   0        0        0    91136 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmpsvh8rgjz.jpg
--rw-r--r--   0        0        0    91363 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmpvtinxpmw.jpg
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/examples/langchain/document_qa.py
--rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/examples/langchain/example.py
--rw-r--r--   0        0        0    74752 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/examples/langchain/florida-drivers-license.jpeg
--rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/examples/minichain/agent.pmpt.tpl
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/examples/minichain/agent.py
--rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/examples/minichain/example.py
--rw-r--r--   0        0        0      679 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/gradio_tools/__init__.py
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/gradio_tools/tools/__init__.py
--rw-r--r--   0        0        0     1024 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/gradio_tools/tools/clip_interrogator.py
--rw-r--r--   0        0        0     1102 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/gradio_tools/tools/document_qa.py
--rw-r--r--   0        0        0     3783 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/gradio_tools/tools/gradio_tool.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/gradio_tools/tools/image_captioning.py
--rw-r--r--   0        0        0     1136 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/gradio_tools/tools/image_to_music.py
--rw-r--r--   0        0        0      977 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/gradio_tools/tools/prompt_generator.py
--rw-r--r--   0        0        0     1320 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/gradio_tools/tools/stable_diffusion.py
--rw-r--r--   0        0        0      970 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/gradio_tools/tools/text_to_video.py
--rw-r--r--   0        0        0      986 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/gradio_tools/tools/whisper.py
--rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/scripts/format.sh
--rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/scripts/lint.sh
--rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/.gitignore
--rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/LICENSE
--rw-r--r--   0        0        0     1695 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     8596 2020-02-02 00:00:00.000000 gradio_tools-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     6148 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/.DS_Store
+-rw-r--r--   0        0        0     6711 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/README.md
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/passwords.txt
+-rw-r--r--   0        0        0      314 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/temp.log
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/.pytest_cache/README.md
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0        1 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/.ruff_cache/.gitignore
+-rw-r--r--   0        0        0       43 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/.ruff_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      143 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/.vscode/settings.json
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/162952a0-7147-4f52-ab58-f852bc5c0561/captions.json
+-rw-r--r--   0        0        0   109150 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/162952a0-7147-4f52-ab58-f852bc5c0561/tmp09966smi.jpg
+-rw-r--r--   0        0        0    79996 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/162952a0-7147-4f52-ab58-f852bc5c0561/tmpf213r3ou.jpg
+-rw-r--r--   0        0        0    99128 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/162952a0-7147-4f52-ab58-f852bc5c0561/tmpjpgr84co.jpg
+-rw-r--r--   0        0        0   101966 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/162952a0-7147-4f52-ab58-f852bc5c0561/tmpo84_x1ra.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/1ce5c1e8-1308-4a24-bebb-27ee49bbcbf1/captions.json
+-rw-r--r--   0        0        0   143165 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/1ce5c1e8-1308-4a24-bebb-27ee49bbcbf1/tmpd4fe9ahm.jpg
+-rw-r--r--   0        0        0    97772 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/1ce5c1e8-1308-4a24-bebb-27ee49bbcbf1/tmpe0qa0lhx.jpg
+-rw-r--r--   0        0        0    94365 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/1ce5c1e8-1308-4a24-bebb-27ee49bbcbf1/tmpnvmcs9su.jpg
+-rw-r--r--   0        0        0    71624 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/1ce5c1e8-1308-4a24-bebb-27ee49bbcbf1/tmpwvlf4c_7.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/27195f48-ea83-46b0-be72-39e76f1432a3/captions.json
+-rw-r--r--   0        0        0   140326 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/27195f48-ea83-46b0-be72-39e76f1432a3/tmp0364mijl.jpg
+-rw-r--r--   0        0        0    63032 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/27195f48-ea83-46b0-be72-39e76f1432a3/tmpn8vk75sg.jpg
+-rw-r--r--   0        0        0    90188 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/27195f48-ea83-46b0-be72-39e76f1432a3/tmpp4x_v2hp.jpg
+-rw-r--r--   0        0        0   139229 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/27195f48-ea83-46b0-be72-39e76f1432a3/tmpvswx2fg1.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/2dd3f23c-4b73-4041-bc64-49c2f9487cbd/captions.json
+-rw-r--r--   0        0        0   123839 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/2dd3f23c-4b73-4041-bc64-49c2f9487cbd/tmp37n48nis.jpg
+-rw-r--r--   0        0        0    74284 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/2dd3f23c-4b73-4041-bc64-49c2f9487cbd/tmp6_fdz6c8.jpg
+-rw-r--r--   0        0        0   110328 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/2dd3f23c-4b73-4041-bc64-49c2f9487cbd/tmp_kkj0za7.jpg
+-rw-r--r--   0        0        0   110178 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/2dd3f23c-4b73-4041-bc64-49c2f9487cbd/tmpbjq5o1s2.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/330d40a3-cc6a-41ce-96c2-002bc67df326/captions.json
+-rw-r--r--   0        0        0   105846 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpj7ygzwvr.jpg
+-rw-r--r--   0        0        0   126760 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpqdvz5be9.jpg
+-rw-r--r--   0        0        0   119178 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/330d40a3-cc6a-41ce-96c2-002bc67df326/tmprmxi0obh.jpg
+-rw-r--r--   0        0        0   108581 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpyo33vqhb.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/captions.json
+-rw-r--r--   0        0        0    99607 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmp26bprpby.jpg
+-rw-r--r--   0        0        0   131260 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmp5u2z8292.jpg
+-rw-r--r--   0        0        0   116900 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmpmdu7tfxc.jpg
+-rw-r--r--   0        0        0    80104 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmpy8rnr6lx.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/508529be-bc20-48b9-b0b7-003e7a21db62/captions.json
+-rw-r--r--   0        0        0   122753 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/508529be-bc20-48b9-b0b7-003e7a21db62/tmp1rbaj9ih.jpg
+-rw-r--r--   0        0        0    86812 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/508529be-bc20-48b9-b0b7-003e7a21db62/tmpgo3ghi7z.jpg
+-rw-r--r--   0        0        0   105885 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/508529be-bc20-48b9-b0b7-003e7a21db62/tmpppnjp9oh.jpg
+-rw-r--r--   0        0        0   117917 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/508529be-bc20-48b9-b0b7-003e7a21db62/tmpvgae85c7.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/captions.json
+-rw-r--r--   0        0        0   106965 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpmsy7r5s4.jpg
+-rw-r--r--   0        0        0   126635 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpotr65fvw.jpg
+-rw-r--r--   0        0        0   103678 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpr4__qxcx.jpg
+-rw-r--r--   0        0        0    94221 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpx4p7b1ft.jpg
+-rw-r--r--   0        0        0      206 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/5b6efdad-3ce5-4de9-a2b6-ded17b234523/captions.json
+-rw-r--r--   0        0        0   141280 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/5b6efdad-3ce5-4de9-a2b6-ded17b234523/tmpjumozfel.jpg
+-rw-r--r--   0        0        0   111566 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/5b6efdad-3ce5-4de9-a2b6-ded17b234523/tmppfkjroq_.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/6a6c3f15-5217-462c-9d28-39f1b2f07676/captions.json
+-rw-r--r--   0        0        0   135053 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmpj6tqr3fx.jpg
+-rw-r--r--   0        0        0   108105 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmpodtfruna.jpg
+-rw-r--r--   0        0        0   137541 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmppg3kuayo.jpg
+-rw-r--r--   0        0        0   103154 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmps600nxhc.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/70a06453-f83c-4866-89a1-d8f5c9a052d7/captions.json
+-rw-r--r--   0        0        0    77205 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpjnq5cw1k.jpg
+-rw-r--r--   0        0        0    92290 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmps6bqlq3v.jpg
+-rw-r--r--   0        0        0   120803 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpvhwji69q.jpg
+-rw-r--r--   0        0        0    89928 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpxap7ybtb.jpg
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/7530e9db-63aa-46f5-b72c-d8ea7f96fc37/captions.json
+-rw-r--r--   0        0        0    99904 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/7530e9db-63aa-46f5-b72c-d8ea7f96fc37/tmp0bq293n9.jpg
+-rw-r--r--   0        0        0    75479 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/7530e9db-63aa-46f5-b72c-d8ea7f96fc37/tmphhgdi5d9.jpg
+-rw-r--r--   0        0        0    96797 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/7530e9db-63aa-46f5-b72c-d8ea7f96fc37/tmpjgndeko_.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/75c113a2-7d4f-4f14-abe9-23259df50dfb/captions.json
+-rw-r--r--   0        0        0    96910 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmp9wfer_02.jpg
+-rw-r--r--   0        0        0    81978 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpiyhb0oay.jpg
+-rw-r--r--   0        0        0   112268 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpluez_al7.jpg
+-rw-r--r--   0        0        0    78187 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpp4qnbcqi.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/captions.json
+-rw-r--r--   0        0        0    93851 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmp74tk8cfs.jpg
+-rw-r--r--   0        0        0   115711 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpk_wbbklr.jpg
+-rw-r--r--   0        0        0    89571 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpvufkgo26.jpg
+-rw-r--r--   0        0        0   112338 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpz6lir7im.jpg
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/90c5b713-cf18-4fde-aefb-92b2d1b2f1ec/captions.json
+-rw-r--r--   0        0        0    47561 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/90c5b713-cf18-4fde-aefb-92b2d1b2f1ec/tmpnu2s0p5c.jpg
+-rw-r--r--   0        0        0   104221 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/90c5b713-cf18-4fde-aefb-92b2d1b2f1ec/tmpsvafzhhw.jpg
+-rw-r--r--   0        0        0    73088 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/90c5b713-cf18-4fde-aefb-92b2d1b2f1ec/tmpx8aicgye.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/aa3ee281-8672-4993-bb3e-09335e1de70e/captions.json
+-rw-r--r--   0        0        0   122186 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/aa3ee281-8672-4993-bb3e-09335e1de70e/tmp4i1fupac.jpg
+-rw-r--r--   0        0        0    93863 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/aa3ee281-8672-4993-bb3e-09335e1de70e/tmp9px6fa06.jpg
+-rw-r--r--   0        0        0   121362 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/aa3ee281-8672-4993-bb3e-09335e1de70e/tmpceochm5g.jpg
+-rw-r--r--   0        0        0    80154 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/aa3ee281-8672-4993-bb3e-09335e1de70e/tmpqjthh1r6.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/aa9874d1-dc09-4c04-bf37-55c556e61e83/captions.json
+-rw-r--r--   0        0        0   111564 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmp5myeybsm.jpg
+-rw-r--r--   0        0        0    98332 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmpd3ufb_2o.jpg
+-rw-r--r--   0        0        0   112096 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmpdlfj8cj_.jpg
+-rw-r--r--   0        0        0   109146 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmps0tx8a8q.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/ac2f6e03-9430-4c22-a559-354225a49357/captions.json
+-rw-r--r--   0        0        0    79381 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/ac2f6e03-9430-4c22-a559-354225a49357/tmp2ye34bli.jpg
+-rw-r--r--   0        0        0   105896 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/ac2f6e03-9430-4c22-a559-354225a49357/tmp5ufb0844.jpg
+-rw-r--r--   0        0        0    92696 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/ac2f6e03-9430-4c22-a559-354225a49357/tmp_h1cp6t2.jpg
+-rw-r--r--   0        0        0   112587 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/ac2f6e03-9430-4c22-a559-354225a49357/tmpvqywwmzc.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/c11e5ee0-e17c-4d0e-9950-09e0c437c3b2/captions.json
+-rw-r--r--   0        0        0   103101 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/c11e5ee0-e17c-4d0e-9950-09e0c437c3b2/tmpg2htn2w7.jpg
+-rw-r--r--   0        0        0    81958 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/c11e5ee0-e17c-4d0e-9950-09e0c437c3b2/tmpkoqyldk0.jpg
+-rw-r--r--   0        0        0    55884 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/c11e5ee0-e17c-4d0e-9950-09e0c437c3b2/tmpnru9hk2q.jpg
+-rw-r--r--   0        0        0    83078 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/c11e5ee0-e17c-4d0e-9950-09e0c437c3b2/tmpvxkwhzbo.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/captions.json
+-rw-r--r--   0        0        0    93651 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmp7n9_771q.jpg
+-rw-r--r--   0        0        0    83077 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpgaejg5rz.jpg
+-rw-r--r--   0        0        0   101925 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpl3n0u99v.jpg
+-rw-r--r--   0        0        0   122576 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpuylgwvrf.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/d52f969d-6985-461d-bf02-080c86e36628/captions.json
+-rw-r--r--   0        0        0   133445 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/d52f969d-6985-461d-bf02-080c86e36628/tmpe6rm8dhh.jpg
+-rw-r--r--   0        0        0    76358 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/d52f969d-6985-461d-bf02-080c86e36628/tmpk6ugfnjb.jpg
+-rw-r--r--   0        0        0    67170 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/d52f969d-6985-461d-bf02-080c86e36628/tmpnmfnsc82.jpg
+-rw-r--r--   0        0        0    79654 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/d52f969d-6985-461d-bf02-080c86e36628/tmpy8mg_mm2.jpg
+-rw-r--r--   0        0        0      412 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/captions.json
+-rw-r--r--   0        0        0    99572 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmphp1_2bwe.jpg
+-rw-r--r--   0        0        0   115349 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmplv4pugrr.jpg
+-rw-r--r--   0        0        0    91136 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmpsvh8rgjz.jpg
+-rw-r--r--   0        0        0    91363 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmpvtinxpmw.jpg
+-rw-r--r--   0        0        0     1014 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/examples/langchain/bark_example.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/examples/langchain/document_qa.py
+-rw-r--r--   0        0        0     1037 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/examples/langchain/example.py
+-rw-r--r--   0        0        0    74752 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/examples/langchain/florida-drivers-license.jpeg
+-rw-r--r--   0        0        0     1876 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/examples/minichain/agent.pmpt.tpl
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/examples/minichain/agent.py
+-rw-r--r--   0        0        0     1378 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/examples/minichain/example.py
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/gradio_tools/__init__.py
+-rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/gradio_tools/tools/__init__.py
+-rw-r--r--   0        0        0     2592 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/gradio_tools/tools/bark.py
+-rw-r--r--   0        0        0     1059 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/gradio_tools/tools/clip_interrogator.py
+-rw-r--r--   0        0        0     1137 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/gradio_tools/tools/document_qa.py
+-rw-r--r--   0        0        0     3881 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/gradio_tools/tools/gradio_tool.py
+-rw-r--r--   0        0        0     1123 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/gradio_tools/tools/image_captioning.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/gradio_tools/tools/image_to_music.py
+-rw-r--r--   0        0        0     1013 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/gradio_tools/tools/prompt_generator.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/gradio_tools/tools/stable_diffusion.py
+-rw-r--r--   0        0        0     1006 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/gradio_tools/tools/text_to_video.py
+-rw-r--r--   0        0        0     1022 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/gradio_tools/tools/whisper.py
+-rw-r--r--   0        0        0       82 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/scripts/format.sh
+-rw-r--r--   0        0        0      112 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/scripts/lint.sh
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/tests/test_tools.py
+-rw-r--r--   0        0        0       76 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1071 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/LICENSE
+-rw-r--r--   0        0        0     1705 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     8667 2020-02-02 00:00:00.000000 gradio_tools-0.0.6/PKG-INFO
```

### Comparing `gradio_tools-0.0.5/.DS_Store` & `gradio_tools-0.0.6/.DS_Store`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/README.md` & `gradio_tools-0.0.6/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -14,40 +14,37 @@
 2. ImageCaptionTool - Caption an image by providing a filepath based on Niels Rogge's [HuggingFace Space](https://huggingface.co/spaces/nielsr/comparing-captioning-models)
 3. ImageToMusicTool - Create an audio clip that matches the style of a given image file based on Sylvain Filoni's [HuggingFace Space](https://huggingface.co/spaces/fffiloni/img-to-music)
 4. StableDiffusionPromptGeneratorTool - Use this tool to improve a prompt for stable diffusion and other image generators based on this [HuggingFace Space](https://huggingface.co/spaces/microsoft/Promptist)
 5. TextToVideoTool - A tool for creating short videos from text. Based on this [HuggingFace Space](https://huggingface.co/spaces/damo-vilab/modelscope-text-to-video-synthesis)
 6. WhisperAudioTranscriptionTool - A tool for transcribing audio with Whisper. Based on this [HuggingFace Space](https://huggingface.co/spaces/abidlabs/whisper)
 7. ClipInterrogatorTool - A tool for reverse engineering a prompt from a source image. Based on this [HuggingFace Space](https://huggingface.co/spaces/pharma/CLIP-Interrogator)
 8. DocQueryDocumentAnsweringTool - A tool for answering questions about a document from the from the image of the document. Based on this [HuggingFace Space](https://huggingface.co/spaces/abidlabs/docquery)
+9. BarkTextToSpeechTool - A tool for text-to-speech. Based on this [HuggingFace Space](https://huggingface.co/spaces/suno/bark)
 
 We welcome more contributions!
 
 ## Example Usage
 
-Simply import the desired tools from `gradio_tool` (or create your own!) and pass to `initialize_agent` from LangChain.
+Simply import the desired tools from `gradio_tools` (or create your own!) and pass to `initialize_agent` from LangChain.
 
 In this example, we use some pre-built tools to generate images, caption them, and create a video!
 
 Read the [How It Works](#how-it-works) section to learn how to create your own tools! We welcome any new tools to the library!
 
 ```python
-import os
-
-if not os.getenv("OPENAI_API_KEY"):
-    raise ValueError("OPENAI_API_KEY must be set")
-
-from langchain.agents import initialize_agent
-from langchain.llms import OpenAI
 from gradio_tools import (StableDiffusionTool, ImageCaptioningTool, StableDiffusionPromptGeneratorTool,
                           TextToVideoTool)
 
+from langchain.agents import initialize_agent
+from langchain.llms import OpenAI
 from langchain.memory import ConversationBufferMemory
 
 llm = OpenAI(temperature=0)
 memory = ConversationBufferMemory(memory_key="chat_history")
+
 tools = [StableDiffusionTool().langchain, ImageCaptioningTool().langchain,
          StableDiffusionPromptGeneratorTool().langchain, TextToVideoTool().langchain]
 
 
 agent = initialize_agent(tools, llm, memory=memory, agent="conversational-react-description", verbose=True)
 output = agent.run(input=("Please create a photo of a dog riding a skateboard "
                           "but improve my prompt prior to using an image generator."
@@ -76,15 +73,15 @@
     def postprocess(self, output: Tuple[Any] | Any) -> str:
         pass
 ```
 
 The requirements are:
 1. The name for your tool
 2. The description for your tool. This is crucial! Agents decide which tool to use based on their description. Be precise and be sure to inclue example of what the input and the output of the tool should look like.
-3. The url or space id, e.g. `freddyaboulton/calculator`, of the Gradio application. Based on this value, `gradio_tool` will create a [gradio client](https://github.com/gradio-app/gradio/blob/main/client/python/README.md) instance to query the upstream application via API. Be sure to click the link and learn more about the gradio client library if you are not familiar with it.
+3. The url or space id, e.g. `freddyaboulton/calculator`, of the Gradio application. Based on this value, `gradio_tools` will create a [gradio client](https://github.com/gradio-app/gradio/blob/main/client/python/README.md) instance to query the upstream application via API. Be sure to click the link and learn more about the gradio client library if you are not familiar with it.
 4. create_job - Given a string, this method should parse that string and return a job from the client. Most times, this is as simple as passing the string to the `submit` function of the client. More info on creating jobs [here](https://github.com/gradio-app/gradio/blob/main/client/python/README.md#making-a-prediction)
 5. postprocess - Given the result of the job, convert it to a string the LLM can display to the user.
 6. *Optional* - Some libraries, e.g. [MiniChain](https://github.com/srush/MiniChain/tree/main), may need some info about the underlying gradio input and output types used by the tool. By default, this will return gr.Textbox() but 
 if you'd like to provide more accurate info, implement the `_block_input(self, gr)` and `_block_output(self, gr)` methods of the tool. The `gr` variable is the gradio module (the result of `import gradio as gr`). It will be
 automatically imported by the `GradiTool` parent class and passed to the `_block_input` and `_block_output` methods.
 
 And that's it!
```

### Comparing `gradio_tools-0.0.5/162952a0-7147-4f52-ab58-f852bc5c0561/tmp09966smi.jpg` & `gradio_tools-0.0.6/162952a0-7147-4f52-ab58-f852bc5c0561/tmp09966smi.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/162952a0-7147-4f52-ab58-f852bc5c0561/tmpf213r3ou.jpg` & `gradio_tools-0.0.6/162952a0-7147-4f52-ab58-f852bc5c0561/tmpf213r3ou.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/162952a0-7147-4f52-ab58-f852bc5c0561/tmpjpgr84co.jpg` & `gradio_tools-0.0.6/162952a0-7147-4f52-ab58-f852bc5c0561/tmpjpgr84co.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/162952a0-7147-4f52-ab58-f852bc5c0561/tmpo84_x1ra.jpg` & `gradio_tools-0.0.6/162952a0-7147-4f52-ab58-f852bc5c0561/tmpo84_x1ra.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpj7ygzwvr.jpg` & `gradio_tools-0.0.6/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpj7ygzwvr.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpqdvz5be9.jpg` & `gradio_tools-0.0.6/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpqdvz5be9.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/330d40a3-cc6a-41ce-96c2-002bc67df326/tmprmxi0obh.jpg` & `gradio_tools-0.0.6/330d40a3-cc6a-41ce-96c2-002bc67df326/tmprmxi0obh.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpyo33vqhb.jpg` & `gradio_tools-0.0.6/330d40a3-cc6a-41ce-96c2-002bc67df326/tmpyo33vqhb.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmp26bprpby.jpg` & `gradio_tools-0.0.6/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmp26bprpby.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmp5u2z8292.jpg` & `gradio_tools-0.0.6/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmp5u2z8292.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmpmdu7tfxc.jpg` & `gradio_tools-0.0.6/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmpmdu7tfxc.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmpy8rnr6lx.jpg` & `gradio_tools-0.0.6/46a3cc03-6b89-4125-a0de-4caa7c83ca9f/tmpy8rnr6lx.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/508529be-bc20-48b9-b0b7-003e7a21db62/tmp1rbaj9ih.jpg` & `gradio_tools-0.0.6/508529be-bc20-48b9-b0b7-003e7a21db62/tmp1rbaj9ih.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/508529be-bc20-48b9-b0b7-003e7a21db62/tmpgo3ghi7z.jpg` & `gradio_tools-0.0.6/508529be-bc20-48b9-b0b7-003e7a21db62/tmpgo3ghi7z.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/508529be-bc20-48b9-b0b7-003e7a21db62/tmpppnjp9oh.jpg` & `gradio_tools-0.0.6/508529be-bc20-48b9-b0b7-003e7a21db62/tmpppnjp9oh.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/508529be-bc20-48b9-b0b7-003e7a21db62/tmpvgae85c7.jpg` & `gradio_tools-0.0.6/508529be-bc20-48b9-b0b7-003e7a21db62/tmpvgae85c7.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpmsy7r5s4.jpg` & `gradio_tools-0.0.6/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpmsy7r5s4.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpotr65fvw.jpg` & `gradio_tools-0.0.6/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpotr65fvw.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpr4__qxcx.jpg` & `gradio_tools-0.0.6/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpr4__qxcx.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpx4p7b1ft.jpg` & `gradio_tools-0.0.6/5a0328c5-2a80-41de-bb5f-ffd81dbf1742/tmpx4p7b1ft.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmpj6tqr3fx.jpg` & `gradio_tools-0.0.6/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmpj6tqr3fx.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmpodtfruna.jpg` & `gradio_tools-0.0.6/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmpodtfruna.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmppg3kuayo.jpg` & `gradio_tools-0.0.6/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmppg3kuayo.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmps600nxhc.jpg` & `gradio_tools-0.0.6/6a6c3f15-5217-462c-9d28-39f1b2f07676/tmps600nxhc.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpjnq5cw1k.jpg` & `gradio_tools-0.0.6/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpjnq5cw1k.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmps6bqlq3v.jpg` & `gradio_tools-0.0.6/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmps6bqlq3v.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpvhwji69q.jpg` & `gradio_tools-0.0.6/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpvhwji69q.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpxap7ybtb.jpg` & `gradio_tools-0.0.6/70a06453-f83c-4866-89a1-d8f5c9a052d7/tmpxap7ybtb.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmp9wfer_02.jpg` & `gradio_tools-0.0.6/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmp9wfer_02.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpiyhb0oay.jpg` & `gradio_tools-0.0.6/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpiyhb0oay.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpluez_al7.jpg` & `gradio_tools-0.0.6/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpluez_al7.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpp4qnbcqi.jpg` & `gradio_tools-0.0.6/75c113a2-7d4f-4f14-abe9-23259df50dfb/tmpp4qnbcqi.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmp74tk8cfs.jpg` & `gradio_tools-0.0.6/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmp74tk8cfs.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpk_wbbklr.jpg` & `gradio_tools-0.0.6/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpk_wbbklr.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpvufkgo26.jpg` & `gradio_tools-0.0.6/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpvufkgo26.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpz6lir7im.jpg` & `gradio_tools-0.0.6/82d2c01a-6cf2-4fbf-9b8f-cae4d457e51c/tmpz6lir7im.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/aa3ee281-8672-4993-bb3e-09335e1de70e/tmp4i1fupac.jpg` & `gradio_tools-0.0.6/aa3ee281-8672-4993-bb3e-09335e1de70e/tmp4i1fupac.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/aa3ee281-8672-4993-bb3e-09335e1de70e/tmp9px6fa06.jpg` & `gradio_tools-0.0.6/aa3ee281-8672-4993-bb3e-09335e1de70e/tmp9px6fa06.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/aa3ee281-8672-4993-bb3e-09335e1de70e/tmpceochm5g.jpg` & `gradio_tools-0.0.6/aa3ee281-8672-4993-bb3e-09335e1de70e/tmpceochm5g.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/aa3ee281-8672-4993-bb3e-09335e1de70e/tmpqjthh1r6.jpg` & `gradio_tools-0.0.6/aa3ee281-8672-4993-bb3e-09335e1de70e/tmpqjthh1r6.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmp5myeybsm.jpg` & `gradio_tools-0.0.6/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmp5myeybsm.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmpd3ufb_2o.jpg` & `gradio_tools-0.0.6/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmpd3ufb_2o.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmpdlfj8cj_.jpg` & `gradio_tools-0.0.6/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmpdlfj8cj_.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmps0tx8a8q.jpg` & `gradio_tools-0.0.6/aa9874d1-dc09-4c04-bf37-55c556e61e83/tmps0tx8a8q.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/ac2f6e03-9430-4c22-a559-354225a49357/tmp2ye34bli.jpg` & `gradio_tools-0.0.6/ac2f6e03-9430-4c22-a559-354225a49357/tmp2ye34bli.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/ac2f6e03-9430-4c22-a559-354225a49357/tmp5ufb0844.jpg` & `gradio_tools-0.0.6/ac2f6e03-9430-4c22-a559-354225a49357/tmp5ufb0844.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/ac2f6e03-9430-4c22-a559-354225a49357/tmp_h1cp6t2.jpg` & `gradio_tools-0.0.6/ac2f6e03-9430-4c22-a559-354225a49357/tmp_h1cp6t2.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/ac2f6e03-9430-4c22-a559-354225a49357/tmpvqywwmzc.jpg` & `gradio_tools-0.0.6/ac2f6e03-9430-4c22-a559-354225a49357/tmpvqywwmzc.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmp7n9_771q.jpg` & `gradio_tools-0.0.6/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmp7n9_771q.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpgaejg5rz.jpg` & `gradio_tools-0.0.6/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpgaejg5rz.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpl3n0u99v.jpg` & `gradio_tools-0.0.6/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpl3n0u99v.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpuylgwvrf.jpg` & `gradio_tools-0.0.6/d516a0b0-d8dd-4321-b2f2-162eabaa7c82/tmpuylgwvrf.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmphp1_2bwe.jpg` & `gradio_tools-0.0.6/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmphp1_2bwe.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmplv4pugrr.jpg` & `gradio_tools-0.0.6/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmplv4pugrr.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmpsvh8rgjz.jpg` & `gradio_tools-0.0.6/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmpsvh8rgjz.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmpvtinxpmw.jpg` & `gradio_tools-0.0.6/ecef1bdd-7ee6-4f57-9d84-202a039dd8d2/tmpvtinxpmw.jpg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/examples/langchain/document_qa.py` & `gradio_tools-0.0.6/examples/langchain/document_qa.py`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/examples/langchain/example.py` & `gradio_tools-0.0.6/examples/langchain/example.py`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/examples/langchain/florida-drivers-license.jpeg` & `gradio_tools-0.0.6/examples/langchain/florida-drivers-license.jpeg`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/examples/minichain/agent.pmpt.tpl` & `gradio_tools-0.0.6/examples/minichain/agent.pmpt.tpl`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/examples/minichain/agent.py` & `gradio_tools-0.0.6/examples/minichain/agent.py`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/examples/minichain/example.py` & `gradio_tools-0.0.6/examples/minichain/example.py`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/gradio_tools/tools/__init__.py` & `gradio_tools-0.0.6/gradio_tools/tools/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from gradio_tools.tools.bark import BarkTextToSpeechTool
 from gradio_tools.tools.clip_interrogator import ClipInterrogatorTool
 from gradio_tools.tools.document_qa import DocQueryDocumentAnsweringTool
 from gradio_tools.tools.gradio_tool import GradioTool
 from gradio_tools.tools.image_captioning import ImageCaptioningTool
 from gradio_tools.tools.image_to_music import ImageToMusicTool
 from gradio_tools.tools.prompt_generator import \
     StableDiffusionPromptGeneratorTool
@@ -15,8 +16,9 @@
     "ClipInterrogatorTool",
     "ImageCaptioningTool",
     "ImageToMusicTool",
     "WhisperAudioTranscriptionTool",
     "StableDiffusionPromptGeneratorTool",
     "TextToVideoTool",
     "DocQueryDocumentAnsweringTool",
+    "BarkTextToSpeechTool",
 ]
```

### Comparing `gradio_tools-0.0.5/gradio_tools/tools/clip_interrogator.py` & `gradio_tools-0.0.6/gradio_tools/tools/whisper.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,34 +1,35 @@
+from __future__ import annotations
+
 from typing import TYPE_CHECKING
 
 from gradio_client.client import Job
 
 from gradio_tools.tools.gradio_tool import GradioTool
 
 if TYPE_CHECKING:
     import gradio as gr
 
 
-class ClipInterrogatorTool(GradioTool):
+class WhisperAudioTranscriptionTool(GradioTool):
     def __init__(
         self,
-        name="ClipInterrogator",
+        name="WhisperAudioTranscription",
         description=(
-            "A tool for reverse engineering a prompt from a source image. "
-            "Use this tool to create a prompt for StableDiffusion that matches the "
-            "input image. The imput is a path to an image. The output is a text string."
+            "A tool for transcribing audio. Use this tool to transcribe an audio file. "
+            "track from an image. Input will be a path to an audio file. "
+            "The output will the text transcript of that file."
         ),
-        src="pharma/CLIP-Interrogator",
+        src="abidlabs/whisper",
         hf_token=None,
+        duplicate=False,
     ) -> None:
-        super().__init__(name, description, src, hf_token)
+        super().__init__(name, description, src, hf_token, duplicate)
 
     def create_job(self, query: str) -> Job:
-        return self.client.submit(
-            query, "ViT-L (best for Stable Diffusion 1.*)", "best", fn_index=3
-        )
+        return self.client.submit(query, api_name="/predict")
 
     def postprocess(self, output: str) -> str:
         return output
 
     def _block_input(self, gr) -> "gr.components.Component":
-        return gr.Image()
+        return gr.Audio()
```

### Comparing `gradio_tools-0.0.5/gradio_tools/tools/document_qa.py` & `gradio_tools-0.0.6/gradio_tools/tools/document_qa.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,16 +14,17 @@
         name="DocQuery",
         description=(
             "A tool for answering questions about a document from the from the image of the document. Input will be a two strings separated by a comma: the first will be the path or URL to an image of a document. The second will be your question about the document."
             "The output will the text answer to your question."
         ),
         src="abidlabs/docquery",
         hf_token=None,
+        duplicate=True,
     ) -> None:
-        super().__init__(name, description, src, hf_token)
+        super().__init__(name, description, src, hf_token, duplicate)
 
     def create_job(self, query: str) -> Job:
         img, question = query.split(",")
         return self.client.submit(img.strip(), question.strip(), api_name="/predict")
 
     def postprocess(self, output: str) -> str:
         return output
```

### Comparing `gradio_tools-0.0.5/gradio_tools/tools/gradio_tool.py` & `gradio_tools-0.0.6/gradio_tools/tools/gradio_tool.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,24 +15,29 @@
     LANGCHAIN_INSTALLED = True
 except (ModuleNotFoundError, ImportError):
     LANGCHAIN_INSTALLED = False
 
 
 class GradioTool:
     def __init__(
-        self, name: str, description: str, src: str, hf_token: str | None = None
+        self,
+        name: str,
+        description: str,
+        src: str,
+        hf_token: str | None = None,
+        duplicate: bool = True,
     ) -> None:
         self.name = name
         self.description = description
-        if hf_token and self._is_space(src):
+        if hf_token and self._is_space(src) and duplicate:
             self.client = grc.Client.duplicate(from_id=src, hf_token=hf_token)
             self.src = self.client.space_id
         else:
             self.src = src
-            self.client = grc.Client(self.src)
+            self.client = grc.Client(self.src, hf_token=hf_token)
         self.description += (
             "If the output is the string QUEUE_FULL you "
             "should try this action again and never stop until you "
             "don't see this message."
         )
         self._block = None
```

### Comparing `gradio_tools-0.0.5/gradio_tools/tools/image_captioning.py` & `gradio_tools-0.0.6/gradio_tools/tools/image_captioning.py`

 * *Files 10% similar despite different names*

```diff
@@ -19,16 +19,17 @@
         description=(
             "An image captioner. Use this to create a caption for an image. "
             "Input will be a path to an image file. "
             "The output will be a caption of that image."
         ),
         src="taesiri/BLIP-2",
         hf_token=None,
+        duplicate=True,
     ) -> None:
-        super().__init__(name, description, src, hf_token)
+        super().__init__(name, description, src, hf_token, duplicate)
 
     def create_job(self, query: str) -> Job:
         return self.client.submit(query.strip("'"), "Beam Search", fn_index=0)
 
     def postprocess(self, output: str) -> str:
         return output  # type: ignore
```

### Comparing `gradio_tools-0.0.5/gradio_tools/tools/image_to_music.py` & `gradio_tools-0.0.6/gradio_tools/tools/image_to_music.py`

 * *Files 7% similar despite different names*

```diff
@@ -15,16 +15,17 @@
         description=(
             "A tool for creating music from images. Use this tool to create a musical "
             "track from an image. Input will be a path to an image file. "
             "The output will be an audio file generated from that image."
         ),
         src="fffiloni/img-to-music",
         hf_token=None,
+        duplicate=False,
     ) -> None:
-        super().__init__(name, description, src, hf_token)
+        super().__init__(name, description, src, hf_token, duplicate)
 
     def create_job(self, query: str) -> Job:
         return self.client.submit(
             query.strip("'"), 15, "medium", "loop", None, fn_index=0
         )
 
     def postprocess(self, output: Union[Tuple[Any], Any]) -> str:
```

### Comparing `gradio_tools-0.0.5/gradio_tools/tools/prompt_generator.py` & `gradio_tools-0.0.6/gradio_tools/tools/prompt_generator.py`

 * *Files 14% similar despite different names*

```diff
@@ -13,15 +13,16 @@
             "Use this tool to improve a prompt for stable diffusion and other image and video generators. "
             "This tool will refine your prompt to include key words and phrases that make "
             "stable diffusion and other art generation algorithms perform better. The input is a prompt text string "
             "and the output is a prompt text string"
         ),
         src="microsoft/Promptist",
         hf_token=None,
+        duplicate=False,
     ) -> None:
-        super().__init__(name, description, src, hf_token)
+        super().__init__(name, description, src, hf_token, duplicate)
 
     def create_job(self, query: str) -> Job:
         return self.client.submit(query, api_name="/predict")
 
     def postprocess(self, output: str) -> str:
         return output
```

### Comparing `gradio_tools-0.0.5/gradio_tools/tools/stable_diffusion.py` & `gradio_tools-0.0.6/gradio_tools/tools/stable_diffusion.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,16 +20,17 @@
         description=(
             "An image generator. Use this to generate images based on "
             "text input. Input should be a description of what the image should "
             "look like. The output will be a path to an image file."
         ),
         src="gradio-client-demos/stable-diffusion",
         hf_token=None,
+        duplicate=False,
     ) -> None:
-        super().__init__(name, description, src, hf_token)
+        super().__init__(name, description, src, hf_token, duplicate)
 
     def create_job(self, query: str) -> Job:
         return self.client.submit(query, "", 9, fn_index=1)
 
     def postprocess(self, output: Tuple[Any] | Any) -> str:
         assert isinstance(output, str)
         return [
```

### Comparing `gradio_tools-0.0.5/gradio_tools/tools/text_to_video.py` & `gradio_tools-0.0.6/gradio_tools/tools/text_to_video.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,16 +16,17 @@
             "A tool for creating videos from text."
             "Use this tool to create videos from text prompts. "
             "Input will be a text prompt describing a video scene. "
             "The output will be a path to a video file."
         ),
         src="damo-vilab/modelscope-text-to-video-synthesis",
         hf_token=None,
+        duplicate=False,
     ) -> None:
-        super().__init__(name, description, src, hf_token)
+        super().__init__(name, description, src, hf_token, duplicate)
 
     def create_job(self, query: str) -> Job:
         return self.client.submit(query, -1, 16, 25, fn_index=1)
 
     def postprocess(self, output: str) -> str:
         return output
```

### Comparing `gradio_tools-0.0.5/LICENSE` & `gradio_tools-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `gradio_tools-0.0.5/pyproject.toml` & `gradio_tools-0.0.6/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling", "hatch-requirements-txt", "hatch-fancy-pypi-readme>=22.5.0"]
 build-backend = "hatchling.build"
 
 [project]
 name = "gradio_tools"
-version = "0.0.5"
+version = "0.0.6"
 description = "Use Gradio Apps as tools for LLM Agents"
 requires-python = ">=3.8"
 license = "MIT"
 authors = [
     { name = "Freddy Boulton", email = "alfonsoboulton@gmail.com" },
 ]
 classifiers = [
@@ -35,15 +35,15 @@
 dependencies = [
     "gradio_client>=0.1.2",
 ]
 [project.optional-dependencies]
 minichain = ["gradio", "minichain>=0.3.3"]
 langchain = ["langchain", "openai"]
 all = ["gradio_tools[langchain]", "gradio_tools[minichain]"]
-test = ["ruff==0.0.260", "pyright==1.1.298", "isort >=5.0.6,<6.0.0", "black==22.6.0"]
+test = ["ruff==0.0.260", "pyright==1.1.298", "isort >=5.0.6,<6.0.0", "black==22.6.0", "pytest"]
 dev = ["gradio_tools[all]", "gradio_tools[test]"]
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = "text/markdown"
 fragments = [
   { path = "README.md"},
 ]
```

### Comparing `gradio_tools-0.0.5/PKG-INFO` & `gradio_tools-0.0.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gradio_tools
-Version: 0.0.5
+Version: 0.0.6
 Summary: Use Gradio Apps as tools for LLM Agents
 Author-email: Freddy Boulton <alfonsoboulton@gmail.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Information Technology
@@ -37,14 +37,15 @@
 Provides-Extra: minichain
 Requires-Dist: gradio; extra == 'minichain'
 Requires-Dist: minichain>=0.3.3; extra == 'minichain'
 Provides-Extra: test
 Requires-Dist: black==22.6.0; extra == 'test'
 Requires-Dist: isort<6.0.0,>=5.0.6; extra == 'test'
 Requires-Dist: pyright==1.1.298; extra == 'test'
+Requires-Dist: pytest; extra == 'test'
 Requires-Dist: ruff==0.0.260; extra == 'test'
 Description-Content-Type: text/markdown
 
 # Gradio Tools: Gradio 🤝 LLM Agents
 
 There are many 1000s of [Gradio](https://github.com/gradio-app/gradio) apps on [Hugging Face Spaces](https://huggingface.co/spaces). This library puts them at the tips of your LLM's fingers 🦾
 
@@ -60,40 +61,37 @@
 2. ImageCaptionTool - Caption an image by providing a filepath based on Niels Rogge's [HuggingFace Space](https://huggingface.co/spaces/nielsr/comparing-captioning-models)
 3. ImageToMusicTool - Create an audio clip that matches the style of a given image file based on Sylvain Filoni's [HuggingFace Space](https://huggingface.co/spaces/fffiloni/img-to-music)
 4. StableDiffusionPromptGeneratorTool - Use this tool to improve a prompt for stable diffusion and other image generators based on this [HuggingFace Space](https://huggingface.co/spaces/microsoft/Promptist)
 5. TextToVideoTool - A tool for creating short videos from text. Based on this [HuggingFace Space](https://huggingface.co/spaces/damo-vilab/modelscope-text-to-video-synthesis)
 6. WhisperAudioTranscriptionTool - A tool for transcribing audio with Whisper. Based on this [HuggingFace Space](https://huggingface.co/spaces/abidlabs/whisper)
 7. ClipInterrogatorTool - A tool for reverse engineering a prompt from a source image. Based on this [HuggingFace Space](https://huggingface.co/spaces/pharma/CLIP-Interrogator)
 8. DocQueryDocumentAnsweringTool - A tool for answering questions about a document from the from the image of the document. Based on this [HuggingFace Space](https://huggingface.co/spaces/abidlabs/docquery)
+9. BarkTextToSpeechTool - A tool for text-to-speech. Based on this [HuggingFace Space](https://huggingface.co/spaces/suno/bark)
 
 We welcome more contributions!
 
 ## Example Usage
 
-Simply import the desired tools from `gradio_tool` (or create your own!) and pass to `initialize_agent` from LangChain.
+Simply import the desired tools from `gradio_tools` (or create your own!) and pass to `initialize_agent` from LangChain.
 
 In this example, we use some pre-built tools to generate images, caption them, and create a video!
 
 Read the [How It Works](#how-it-works) section to learn how to create your own tools! We welcome any new tools to the library!
 
 ```python
-import os
-
-if not os.getenv("OPENAI_API_KEY"):
-    raise ValueError("OPENAI_API_KEY must be set")
-
-from langchain.agents import initialize_agent
-from langchain.llms import OpenAI
 from gradio_tools import (StableDiffusionTool, ImageCaptioningTool, StableDiffusionPromptGeneratorTool,
                           TextToVideoTool)
 
+from langchain.agents import initialize_agent
+from langchain.llms import OpenAI
 from langchain.memory import ConversationBufferMemory
 
 llm = OpenAI(temperature=0)
 memory = ConversationBufferMemory(memory_key="chat_history")
+
 tools = [StableDiffusionTool().langchain, ImageCaptioningTool().langchain,
          StableDiffusionPromptGeneratorTool().langchain, TextToVideoTool().langchain]
 
 
 agent = initialize_agent(tools, llm, memory=memory, agent="conversational-react-description", verbose=True)
 output = agent.run(input=("Please create a photo of a dog riding a skateboard "
                           "but improve my prompt prior to using an image generator."
@@ -122,15 +120,15 @@
     def postprocess(self, output: Tuple[Any] | Any) -> str:
         pass
 ```
 
 The requirements are:
 1. The name for your tool
 2. The description for your tool. This is crucial! Agents decide which tool to use based on their description. Be precise and be sure to inclue example of what the input and the output of the tool should look like.
-3. The url or space id, e.g. `freddyaboulton/calculator`, of the Gradio application. Based on this value, `gradio_tool` will create a [gradio client](https://github.com/gradio-app/gradio/blob/main/client/python/README.md) instance to query the upstream application via API. Be sure to click the link and learn more about the gradio client library if you are not familiar with it.
+3. The url or space id, e.g. `freddyaboulton/calculator`, of the Gradio application. Based on this value, `gradio_tools` will create a [gradio client](https://github.com/gradio-app/gradio/blob/main/client/python/README.md) instance to query the upstream application via API. Be sure to click the link and learn more about the gradio client library if you are not familiar with it.
 4. create_job - Given a string, this method should parse that string and return a job from the client. Most times, this is as simple as passing the string to the `submit` function of the client. More info on creating jobs [here](https://github.com/gradio-app/gradio/blob/main/client/python/README.md#making-a-prediction)
 5. postprocess - Given the result of the job, convert it to a string the LLM can display to the user.
 6. *Optional* - Some libraries, e.g. [MiniChain](https://github.com/srush/MiniChain/tree/main), may need some info about the underlying gradio input and output types used by the tool. By default, this will return gr.Textbox() but 
 if you'd like to provide more accurate info, implement the `_block_input(self, gr)` and `_block_output(self, gr)` methods of the tool. The `gr` variable is the gradio module (the result of `import gradio as gr`). It will be
 automatically imported by the `GradiTool` parent class and passed to the `_block_input` and `_block_output` methods.
 
 And that's it!
```

