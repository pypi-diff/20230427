# Comparing `tmp/client_GPT-0.0.1-py3-none-any.whl.zip` & `tmp/client_GPT-0.1.tar.gz`

 * *Command `'zipinfo {}'` failed with exit code 9. Standard output:*

 * *    Archive:  tmp/client_GPT-0.1.tar.gz*

 * *    […]*

 * *Archive contents identical but files differ, possibly due to different compression levels. Falling back to binary comparison.*

```diff
@@ -1,74 +1,77 @@
-00000000: 504b 0304 1400 0000 0800 9043 9b56 a65e  PK.........C.V.^
-00000010: 6b18 1301 0000 be01 0000 2300 0000 636c  k.........#...cl
-00000020: 6965 6e74 5f47 5054 2d30 2e30 2e31 2e64  ient_GPT-0.0.1.d
-00000030: 6973 742d 696e 666f 2f4d 4554 4144 4154  ist-info/METADAT
-00000040: 415d 90dd 4a03 3110 85ef 0379 8779 81dd  A]..J.1....y.y..
-00000050: ad16 bc08 282c 2da8 50a5 d8e2 fd74 77ba  ....(,-.P....tw.
-00000060: 1b9a 3f93 89a5 6f6f 56ab d85e e69c efe4  ..?...ooV..^....
-00000070: cccc 0b31 f6c8 58bd 534c da3b 05b7 f58d  ...1..X.SL.;....
-00000080: 14af 6849 4167 3439 ae1e d75b 29fe fc59  ..hIAg49...[)..Y
-00000090: 3d9b 884d b616 e349 410b 01bb 030e 047b  =..M...IA......{
-000000a0: 1fe1 e8e3 41bb 018e 9a47 2841 30e8 863c  ....A....G(A0..<
-000000b0: b9d6 f764 522d c593 b754 8522 2918 9943  ...dR-...T.")..C
-000000c0: 524d 3314 3aef eace dbc6 6866 4307 a739  RM3.:.....hfC..9
-000000d0: 25f6 f1d4 9c87 1802 4bd1 661e 7d54 700d  %.......K.f.}Tp.
-000000e0: 49b1 3098 92de 6b2a ee92 3ec9 f860 4b0c  I.0...k*..>..`K.
-000000f0: 368c 9c13 2805 73a8 a035 61c4 4bf8 d931  6...(.s..5a.K..1
-00000100: b99e 7a68 735f 8a3a 9ad8 f30f 65e5 4b78  ..zhs_.:....e.Kx
-00000110: eb83 ee26 60e3 f77c c448 175d 455f e95d  ...&`..|.H.]E_.]
-00000120: c4a8 e92a b78e 7e88 68ed 7499 d5ef 410a  ...*..~.h.t...A.
-00000130: be3e 957d dcf7 7452 bcd1 47d6 9152 f5a3  .>.}..tR..G..R..
-00000140: 2a78 b89f d777 fff4 a54e ac20 9627 252e  *x...w...N. .'%.
-00000150: 0d52 7c01 504b 0304 1400 0000 0800 9043  .R|.PK.........C
-00000160: 9b56 49a2 21cb 5c00 0000 5c00 0000 2000  .VI.!.\...\... .
-00000170: 0000 636c 6965 6e74 5f47 5054 2d30 2e30  ..client_GPT-0.0
-00000180: 2e31 2e64 6973 742d 696e 666f 2f57 4845  .1.dist-info/WHE
-00000190: 454c 0bcf 484d cdd1 0d4b 2d2a cecc cfb3  EL..HM...K-*....
-000001a0: 5230 d433 e072 4fcd 4b2d 4a2c c92f b252  R0.3.rO.K-J,./.R
-000001b0: 484a c92c 2e89 2f07 a951 d030 d033 31d0  HJ.,../..Q.0.31.
-000001c0: 33d0 e40a cacf 2fd1 f52c d60d 282d 4acd  3...../..,..(-J.
-000001d0: c94c b252 2829 2a4d e50a 494c b752 28a8  .L.R()*M..IL.R(.
-000001e0: 34d6 cdcb cf4b d54d ccab e4e2 0200 504b  4....K.M......PK
-000001f0: 0304 1400 0000 0800 9043 9b56 9306 d732  .........C.V...2
-00000200: 0300 0000 0100 0000 2800 0000 636c 6965  ........(...clie
-00000210: 6e74 5f47 5054 2d30 2e30 2e31 2e64 6973  nt_GPT-0.0.1.dis
-00000220: 742d 696e 666f 2f74 6f70 5f6c 6576 656c  t-info/top_level
-00000230: 2e74 7874 e302 0050 4b03 0414 0000 0008  .txt...PK.......
-00000240: 0090 439b 565c 0bef 11cf 0000 0034 0100  ..C.V\.......4..
-00000250: 0021 0000 0063 6c69 656e 745f 4750 542d  .!...client_GPT-
-00000260: 302e 302e 312e 6469 7374 2d69 6e66 6f2f  0.0.1.dist-info/
-00000270: 5245 434f 5244 7dcc 4b72 8230 0000 d0bd  RECORD}.Kr.0....
-00000280: 6749 a820 105d 7411 24e0 5014 878f 0e6c  gI. .]t.$.P....l
-00000290: 1808 51d3 3001 9b88 d6d3 77e5 b2be 033c  ..Q.0.....w....<
-000002a0: da73 2675 1dee 7338 37e6 8669 745c 69c8  .s&u..s87..it\i.
-000002b0: e569 f8d8 921c fb38 c740 5d1a cb71 3ff9  .i.....8.@]..q?.
-000002c0: 2e8b 13da 34d9 208e c891 4571 0d3a 3930  ....4. ...Eq.:90
-000002d0: efd7 cf1d bdc5 30aa cdf6 41af d345 15c0  ......0...A..E..
-000002e0: b6dd 19fd bf3e 6e08 895f ef28 a8ae ca67  .....>n.._.(...g
-000002f0: 91d9 b83c 48b7 8b20 5ab8 2889 2a3e 0516  ...<H.. Z.(.*>..
-00000300: 5ba6 78d5 d695 f7cd 4fe6 12ac ac77 ad1e  [.x.....O....w..
-00000310: c6ba 6713 eb0d fdd0 af1e b7e3 26a4 e7b8  ..g.........&...
-00000320: 8522 5551 28ef 0111 5aa0 db73 ac92 35f5  ."UQ(...Z..s..5.
-00000330: 4a64 c3d2 eb7e be0e a102 e6bb 3d25 eb24  Jd...~......=%.$
-00000340: f501 98fd 0150 4b01 0214 0014 0000 0008  .....PK.........
-00000350: 0090 439b 56a6 5e6b 1813 0100 00be 0100  ..C.V.^k........
-00000360: 0023 0000 0000 0000 0000 0000 00b6 8100  .#..............
-00000370: 0000 0063 6c69 656e 745f 4750 542d 302e  ...client_GPT-0.
-00000380: 302e 312e 6469 7374 2d69 6e66 6f2f 4d45  0.1.dist-info/ME
-00000390: 5441 4441 5441 504b 0102 1400 1400 0000  TADATAPK........
-000003a0: 0800 9043 9b56 49a2 21cb 5c00 0000 5c00  ...C.VI.!.\...\.
-000003b0: 0000 2000 0000 0000 0000 0000 0000 b681  .. .............
-000003c0: 5401 0000 636c 6965 6e74 5f47 5054 2d30  T...client_GPT-0
-000003d0: 2e30 2e31 2e64 6973 742d 696e 666f 2f57  .0.1.dist-info/W
-000003e0: 4845 454c 504b 0102 1400 1400 0000 0800  HEELPK..........
-000003f0: 9043 9b56 9306 d732 0300 0000 0100 0000  .C.V...2........
-00000400: 2800 0000 0000 0000 0000 0000 b681 ee01  (...............
-00000410: 0000 636c 6965 6e74 5f47 5054 2d30 2e30  ..client_GPT-0.0
-00000420: 2e31 2e64 6973 742d 696e 666f 2f74 6f70  .1.dist-info/top
-00000430: 5f6c 6576 656c 2e74 7874 504b 0102 1400  _level.txtPK....
-00000440: 1400 0000 0800 9043 9b56 5c0b ef11 cf00  .......C.V\.....
-00000450: 0000 3401 0000 2100 0000 0000 0000 0000  ..4...!.........
-00000460: 0000 b481 3702 0000 636c 6965 6e74 5f47  ....7...client_G
-00000470: 5054 2d30 2e30 2e31 2e64 6973 742d 696e  PT-0.0.1.dist-in
-00000480: 666f 2f52 4543 4f52 4450 4b05 0600 0000  fo/RECORDPK.....
-00000490: 0004 0004 0044 0100 0045 0300 0000 00    .....D...E.....
+00000000: 1f8b 0808 0e74 4664 02ff 636c 6965 6e74  .....tFd..client
+00000010: 5f47 5054 2d30 2e31 2e74 6172 00ed 9c5d  _GPT-0.1.tar...]
+00000020: 73da 3814 86b9 d60c ff41 4b2f 9acc 04e3  s.8......AK/....
+00000030: 0f6c 6799 6167 3369 36c9 b44d 3249 ba37  .lg.ag3i6..M2I.7
+00000040: 9d0e a360 e168 e2af da72 1afe fdca 360e  ...`.h...r....6.
+00000050: 8194 7cec 02db 96f7 bdc1 968e 241b 7cce  ..|.........$.|.
+00000060: e323 5b68 1dad f3e7 19bb 3be2 cce3 6963  .#[h......;...ic
+00000070: 25d2 2b2d fad4 75cb 9a6e 17e5 866e 1a46  %.+-..u..n...n.F
+00000080: 83de 35d6 a03c 932c 55c3 3736 53a6 4b43  ..5..<.,U.76S.KC
+00000090: 2942 de37 9c5d d3b2 7677 2d5d fbdd b06c  )B.7.]..vw-]...l
+000000a0: d320 0de8 d7d7 3010 3c92 83c3 b3cb b6ae  . ....0.<.......
+000000b0: 199d 95f9 bfeb ba8b fd5f 6d1b ddae 6974  ........._m...it
+000000c0: 5d53 37dc d2ff 5da7 416d f8ff caa5 21fe  ]S7...].Am....!.
+000000d0: 23fe 3f8a ffa6 6d9a 88ff 1b18 ffcf de1f  #.?...m.........
+000000e0: b68f 4ffe 3a5d baff 3b8e b3d0 ffed ae3b  ..O.:]..;......;
+000000f0: 17ff 8dae aefc 5f87 ffaf 5c1f b964 1e93  ......_...\..d..
+00000100: acfd 374f 3311 473d 6a6a 4693 9cb0 90f7  ..7O3.G=jjF.....
+00000110: e8f4 e268 92fb 7abd a83f 8a43 de4e 98af  ...h..z..?.C.N..
+00000120: 8cae a54c b25e a7e3 0b79 9d5f 69c3 38ec  ...L.^...y._i.8.
+00000130: 0442 ca80 df44 4266 998c d371 a7ea a8ed  .B...DBf...q....
+00000140: 27b2 49f6 7279 1da7 3d3a 6fd4 24fb 01cb  '.I.ry..=:o.$...
+00000150: 3231 125c d5be e3b7 3c88 9350 35a3 1792  21.\....<..P5...
+00000160: c93c a3bd 1eb5 689b ee05 c935 9b35 3e8e  .<....h....5.5>.
+00000170: 248f 3cee d1bd dc53 030d 7961 3be9 411d  $.<....S..ya;.A.
+00000180: f6ac f165 9c88 6161 7011 8fe4 3796 f299  ...e..aap...7...
+00000190: b154 f907 7195 b254 f0b9 7667 69ec a72c  .T..q..T..vgi..,
+000001a0: 0c45 e4d3 0f2c f273 75f6 85f9 d958 9d4f  .E...,.su....X.O
+000001b0: 541e 5d93 9cf3 afb9 4879 d6ae 4a7b f48f  T.].....Hy..J{..
+000001c0: bea5 39cd 1f37 96fe 10fc 379d c7fc b7c0  ..9..7....7.....
+000001d0: ffb5 f0df 7cc8 7fd3 ddb5 754d 07fa 3795  ....|.....uM..7.
+000001e0: ffe7 077b ef3e 1e68 a1b7 56fe 1be6 84ff  ...{.>.h..V.....
+000001f0: 4ab6 59f0 dfb6 6df0 7f1d 7af3 a6a6 bc82  J.Y...m...z.....
+00000200: 3321 97d7 9c2a 94d2 3ce3 291d b2a8 d8a0  3!...*..<.).....
+00000210: fba5 81ba 44a8 8ca9 e27b 9847 62c8 24a7  ....D....{.Gb.$.
+00000220: df14 f2a9 544d 0e2f 2d1a c61e 0fe8 288d  ....TM./-.....(.
+00000230: 437a 9af0 68ef 5823 44f5 2e22 f505 0701  Cz..h.X#D.."....
+00000240: a124 1149 bd37 33a6 3252 a310 5236 9d56  .$.I.73.2R..R6.V
+00000250: 5011 2671 2aa7 a313 c212 31b8 e163 daa7  P.&q*.....1..c..
+00000260: ad71 9ca7 83c9 7e8b 906a f0ba bcdc 1b08  .q....~..j......
+00000270: 4f55 54fd a99a fb6e b626 ad76 aa23 de56  OUT....n.&.v.#.V
+00000280: 8d79 9629 98ef a873 8b6e d5fd 0293 ea46  .y.)...s.n.....F
+00000290: 4735 57ad aae6 1acb 6eb6 5a47 3c08 e2df  G5W.....n.ZG<...
+000002a0: 5a3b f424 8eb8 6a96 a422 925b 93c6 db3f  Z;.$..j..".[...?
+000002b0: 69cc 44fe 8ffc ff71 feaf 23ff df4c fe4f  i.D....q..#..L.O
+000002c0: 7735 eefb 6d11 8de2 ce52 fcff 75f3 bf96  w5..m....R..u...
+000002d0: ebe8 98ff 45fe 87df 7fbd f95f 15ff 91ff  ....E......_....
+000002e0: 21fe 3f88 ffff 794e f875 f3bf cace b075  !.?...yN.u.....u
+000002f0: c744 feb7 0ebd 60fe b78d f95f ccff 82ff  .D....`...._....
+00000300: e03f b491 fcbf 38fd 74be 7f70 a1c9 3bb9  .?....8.t..p..;.
+00000310: 1afe 9bae 35cf 7fa7 8bf9 dfb5 e87e c29f  ....5........~..
+00000320: 645c e689 968c c953 f780 e499 0be4 bbf5  d\.....S........
+00000330: 1e4f 0a3c 47c3 f120 10d1 4db6 d030 9dd0  .O.<G.. ..M..0..
+00000340: 73a1 818c 9341 50d0 fadf 5f8c 10f8 0fff  s....AP..._.....
+00000350: 07ff a197 f2ff 7be1 7ba9 fcd7 7563 96ff  ......{.{...uc..
+00000360: a60a 09e0 ff5a 0457 07ff c17f f01f fc07  .....Z.W........
+00000370: ff17 f0ff 6156 b692 fc5f 37e6 f86f 3856  ....aV..._7..o8V
+00000380: d705 ffd7 a1e2 c7e5 99cc e0f2 e03f f80f  .............?..
+00000390: fe83 ffe0 ffb2 275d 5f9d ff1b 8ead aac1  ......']_.......
+000003a0: 7fe4 ffd0 26f0 1fef 7fff 7ffc c7ff 7f80  ....&...........
+000003b0: ff53 fe57 0f81 8723 7fd9 feff 24ff 6d73  .S.W...#....$.ms
+000003c0: eefd 6fe5 fe5d f07f 1dfa ac6e f306 c56d  ..o..].....n...m
+000003d0: de97 2691 cc1f 5ce5 2228 163e 557b 5eb1  ..&...\."(.>U{^.
+000003e0: caab 4ff5 2669 221c 80ff c8ff 7ffd fcdf  ..O.&i".........
+000003f0: 3491 ff6f 3aff 93f1 d2fd ff09 fe1b 33f3  4..o:.........3.
+00000400: ff7a 91ff 1bc5 7231 f07f 0d9a 2cb2 2e7f  .z....r1....,...
+00000410: 7719 c741 56a0 7eba a795 9b5b 4d42 9522  w..AV.~....[MB."
+00000420: a6e2 446b 7ac5 b476 aaf2 db6a 6940 bfa5  ..Dkz..v...ji@..
+00000430: aea0 ba8c 956f f9f7 5bf3 6ff9 d7f5 791a  .....o..[.o...y.
+00000440: f45b af5b 3a50 374d d8f0 86f9 3ceb 3f38  .[.[:P7M....<.?8
+00000450: cc91 88bc 415d b1b5 3db1 9cac 361f d44f  ....A]..=...6..O
+00000460: b0fa 9fab f242 adfa c947 dded 97c9 e7f0  .....B...G......
+00000470: fe9d ff59 fb67 5624 d4dd 94b6 cf2c 4898  ...Y.gV$.....,H.
+00000480: b17d f97a 8499 662f 588e 307f 6649 5935  .}.z..f/X.0.fIY5
+00000490: fd36 de96 8b13 deaa da6d dcde 4110 0441  .6.......m..A..A
+000004a0: 1004 4110 0441 1004 4110 0441 1004 4110  ..A..A..A..A..A.
+000004b0: 0441 1004 41d0 4fa8 7f00 0d8c 2e6e 0078  .A..A.O......n.x
+000004c0: 0000                                     ..
```

## Comparing `tmp/client_GPT-0.0.1-py3-none-any.whl.zip` & `tmp/client_GPT-0.1.tar.gz`

```diff
@@ -1,74 +1,77 @@
-00000000: 504b 0304 1400 0000 0800 9043 9b56 a65e  PK.........C.V.^
-00000010: 6b18 1301 0000 be01 0000 2300 0000 636c  k.........#...cl
-00000020: 6965 6e74 5f47 5054 2d30 2e30 2e31 2e64  ient_GPT-0.0.1.d
-00000030: 6973 742d 696e 666f 2f4d 4554 4144 4154  ist-info/METADAT
-00000040: 415d 90dd 4a03 3110 85ef 0379 8779 81dd  A]..J.1....y.y..
-00000050: ad16 bc08 282c 2da8 50a5 d8e2 fd74 77ba  ....(,-.P....tw.
-00000060: 1b9a 3f93 89a5 6f6f 56ab d85e e69c efe4  ..?...ooV..^....
-00000070: cccc 0b31 f6c8 58bd 534c da3b 05b7 f58d  ...1..X.SL.;....
-00000080: 14af 6849 4167 3439 ae1e d75b 29fe fc59  ..hIAg49...[)..Y
-00000090: 3d9b 884d b616 e349 410b 01bb 030e 047b  =..M...IA......{
-000000a0: 1fe1 e8e3 41bb 018e 9a47 2841 30e8 863c  ....A....G(A0..<
-000000b0: b9d6 f764 522d c593 b754 8522 2918 9943  ...dR-...T.")..C
-000000c0: 524d 3314 3aef eace dbc6 6866 4307 a739  RM3.:.....hfC..9
-000000d0: 25f6 f1d4 9c87 1802 4bd1 661e 7d54 700d  %.......K.f.}Tp.
-000000e0: 49b1 3098 92de 6b2a ee92 3ec9 f860 4b0c  I.0...k*..>..`K.
-000000f0: 368c 9c13 2805 73a8 a035 61c4 4bf8 d931  6...(.s..5a.K..1
-00000100: b99e 7a68 735f 8a3a 9ad8 f30f 65e5 4b78  ..zhs_.:....e.Kx
-00000110: eb83 ee26 60e3 f77c c448 175d 455f e95d  ...&`..|.H.]E_.]
-00000120: c4a8 e92a b78e 7e88 68ed 7499 d5ef 410a  ...*..~.h.t...A.
-00000130: be3e 957d dcf7 7452 bcd1 47d6 9152 f5a3  .>.}..tR..G..R..
-00000140: 2a78 b89f d777 fff4 a54e ac20 9627 252e  *x...w...N. .'%.
-00000150: 0d52 7c01 504b 0304 1400 0000 0800 9043  .R|.PK.........C
-00000160: 9b56 49a2 21cb 5c00 0000 5c00 0000 2000  .VI.!.\...\... .
-00000170: 0000 636c 6965 6e74 5f47 5054 2d30 2e30  ..client_GPT-0.0
-00000180: 2e31 2e64 6973 742d 696e 666f 2f57 4845  .1.dist-info/WHE
-00000190: 454c 0bcf 484d cdd1 0d4b 2d2a cecc cfb3  EL..HM...K-*....
-000001a0: 5230 d433 e072 4fcd 4b2d 4a2c c92f b252  R0.3.rO.K-J,./.R
-000001b0: 484a c92c 2e89 2f07 a951 d030 d033 31d0  HJ.,../..Q.0.31.
-000001c0: 33d0 e40a cacf 2fd1 f52c d60d 282d 4acd  3...../..,..(-J.
-000001d0: c94c b252 2829 2a4d e50a 494c b752 28a8  .L.R()*M..IL.R(.
-000001e0: 34d6 cdcb cf4b d54d ccab e4e2 0200 504b  4....K.M......PK
-000001f0: 0304 1400 0000 0800 9043 9b56 9306 d732  .........C.V...2
-00000200: 0300 0000 0100 0000 2800 0000 636c 6965  ........(...clie
-00000210: 6e74 5f47 5054 2d30 2e30 2e31 2e64 6973  nt_GPT-0.0.1.dis
-00000220: 742d 696e 666f 2f74 6f70 5f6c 6576 656c  t-info/top_level
-00000230: 2e74 7874 e302 0050 4b03 0414 0000 0008  .txt...PK.......
-00000240: 0090 439b 565c 0bef 11cf 0000 0034 0100  ..C.V\.......4..
-00000250: 0021 0000 0063 6c69 656e 745f 4750 542d  .!...client_GPT-
-00000260: 302e 302e 312e 6469 7374 2d69 6e66 6f2f  0.0.1.dist-info/
-00000270: 5245 434f 5244 7dcc 4b72 8230 0000 d0bd  RECORD}.Kr.0....
-00000280: 6749 a820 105d 7411 24e0 5014 878f 0e6c  gI. .]t.$.P....l
-00000290: 1808 51d3 3001 9b88 d6d3 77e5 b2be 033c  ..Q.0.....w....<
-000002a0: da73 2675 1dee 7338 37e6 8669 745c 69c8  .s&u..s87..it\i.
-000002b0: e569 f8d8 921c fb38 c740 5d1a cb71 3ff9  .i.....8.@]..q?.
-000002c0: 2e8b 13da 34d9 208e c891 4571 0d3a 3930  ....4. ...Eq.:90
-000002d0: efd7 cf1d bdc5 30aa cdf6 41af d345 15c0  ......0...A..E..
-000002e0: b6dd 19fd bf3e 6e08 895f ef28 a8ae ca67  .....>n.._.(...g
-000002f0: 91d9 b83c 48b7 8b20 5ab8 2889 2a3e 0516  ...<H.. Z.(.*>..
-00000300: 5ba6 78d5 d695 f7cd 4fe6 12ac ac77 ad1e  [.x.....O....w..
-00000310: c6ba 6713 eb0d fdd0 af1e b7e3 26a4 e7b8  ..g.........&...
-00000320: 8522 5551 28ef 0111 5aa0 db73 ac92 35f5  ."UQ(...Z..s..5.
-00000330: 4a64 c3d2 eb7e be0e a102 e6bb 3d25 eb24  Jd...~......=%.$
-00000340: f501 98fd 0150 4b01 0214 0014 0000 0008  .....PK.........
-00000350: 0090 439b 56a6 5e6b 1813 0100 00be 0100  ..C.V.^k........
-00000360: 0023 0000 0000 0000 0000 0000 00b6 8100  .#..............
-00000370: 0000 0063 6c69 656e 745f 4750 542d 302e  ...client_GPT-0.
-00000380: 302e 312e 6469 7374 2d69 6e66 6f2f 4d45  0.1.dist-info/ME
-00000390: 5441 4441 5441 504b 0102 1400 1400 0000  TADATAPK........
-000003a0: 0800 9043 9b56 49a2 21cb 5c00 0000 5c00  ...C.VI.!.\...\.
-000003b0: 0000 2000 0000 0000 0000 0000 0000 b681  .. .............
-000003c0: 5401 0000 636c 6965 6e74 5f47 5054 2d30  T...client_GPT-0
-000003d0: 2e30 2e31 2e64 6973 742d 696e 666f 2f57  .0.1.dist-info/W
-000003e0: 4845 454c 504b 0102 1400 1400 0000 0800  HEELPK..........
-000003f0: 9043 9b56 9306 d732 0300 0000 0100 0000  .C.V...2........
-00000400: 2800 0000 0000 0000 0000 0000 b681 ee01  (...............
-00000410: 0000 636c 6965 6e74 5f47 5054 2d30 2e30  ..client_GPT-0.0
-00000420: 2e31 2e64 6973 742d 696e 666f 2f74 6f70  .1.dist-info/top
-00000430: 5f6c 6576 656c 2e74 7874 504b 0102 1400  _level.txtPK....
-00000440: 1400 0000 0800 9043 9b56 5c0b ef11 cf00  .......C.V\.....
-00000450: 0000 3401 0000 2100 0000 0000 0000 0000  ..4...!.........
-00000460: 0000 b481 3702 0000 636c 6965 6e74 5f47  ....7...client_G
-00000470: 5054 2d30 2e30 2e31 2e64 6973 742d 696e  PT-0.0.1.dist-in
-00000480: 666f 2f52 4543 4f52 4450 4b05 0600 0000  fo/RECORDPK.....
-00000490: 0004 0004 0044 0100 0045 0300 0000 00    .....D...E.....
+00000000: 1f8b 0808 0e74 4664 02ff 636c 6965 6e74  .....tFd..client
+00000010: 5f47 5054 2d30 2e31 2e74 6172 00ed 9c5d  _GPT-0.1.tar...]
+00000020: 73da 3814 86b9 d60c ff41 4b2f 9acc 04e3  s.8......AK/....
+00000030: 0f6c 6799 6167 3369 36c9 b44d 3249 ba37  .lg.ag3i6..M2I.7
+00000040: 9d0e a360 e168 e2af da72 1afe fdca 360e  ...`.h...r....6.
+00000050: 8194 7cec 02db 96f7 bdc1 968e 241b 7cce  ..|.........$.|.
+00000060: e323 5b68 1dad f3e7 19bb 3be2 cce3 6963  .#[h......;...ic
+00000070: 25d2 2b2d fad4 75cb 9a6e 17e5 866e 1a46  %.+-..u..n...n.F
+00000080: 83de 35d6 a03c 932c 55c3 3736 53a6 4b43  ..5..<.,U.76S.KC
+00000090: 2942 de37 9c5d d3b2 7677 2d5d fbdd b06c  )B.7.]..vw-]...l
+000000a0: d320 0de8 d7d7 3010 3c92 83c3 b3cb b6ae  . ....0.<.......
+000000b0: 199d 95f9 bfeb ba8b fd5f 6d1b ddae 6974  ........._m...it
+000000c0: 5d53 37dc d2ff 5da7 416d f8ff caa5 21fe  ]S7...].Am....!.
+000000d0: 23fe 3f8a ffa6 6d9a 88ff 1b18 ffcf de1f  #.?...m.........
+000000e0: b68f 4ffe 3a5d baff 3b8e b3d0 ffed ae3b  ..O.:]..;......;
+000000f0: 17ff 8dae aefc 5f87 ffaf 5c1f b964 1e93  ......_...\..d..
+00000100: acfd 374f 3311 473d 6a6a 4693 9cb0 90f7  ..7O3.G=jjF.....
+00000110: e8f4 e268 92fb 7abd a83f 8a43 de4e 98af  ...h..z..?.C.N..
+00000120: 8cae a54c b25e a7e3 0b79 9d5f 69c3 38ec  ...L.^...y._i.8.
+00000130: 0442 ca80 df44 4266 998c d371 a7ea a8ed  .B...DBf...q....
+00000140: 27b2 49f6 7279 1da7 3d3a 6fd4 24fb 01cb  '.I.ry..=:o.$...
+00000150: 3231 125c d5be e3b7 3c88 9350 35a3 1792  21.\....<..P5...
+00000160: c93c a3bd 1eb5 689b ee05 c935 9b35 3e8e  .<....h....5.5>.
+00000170: 248f 3cee d1bd dc53 030d 7961 3be9 411d  $.<....S..ya;.A.
+00000180: f6ac f165 9c88 6161 7011 8fe4 3796 f299  ...e..aap...7...
+00000190: b154 f907 7195 b254 f0b9 7667 69ec a72c  .T..q..T..vgi..,
+000001a0: 0c45 e4d3 0f2c f273 75f6 85f9 d958 9d4f  .E...,.su....X.O
+000001b0: 541e 5d93 9cf3 afb9 4879 d6ae 4a7b f48f  T.].....Hy..J{..
+000001c0: bea5 39cd 1f37 96fe 10fc 379d c7fc b7c0  ..9..7....7.....
+000001d0: ffb5 f0df 7cc8 7fd3 ddb5 754d 07fa 3795  ....|.....uM..7.
+000001e0: ffe7 077b ef3e 1e68 a1b7 56fe 1be6 84ff  ...{.>.h..V.....
+000001f0: 4ab6 59f0 dfb6 6df0 7f1d 7af3 a6a6 bc82  J.Y...m...z.....
+00000200: 3321 97d7 9c2a 94d2 3ce3 291d b2a8 d8a0  3!...*..<.).....
+00000210: fba5 81ba 44a8 8ca9 e27b 9847 62c8 24a7  ....D....{.Gb.$.
+00000220: df14 f2a9 544d 0e2f 2d1a c61e 0fe8 288d  ....TM./-.....(.
+00000230: 437a 9af0 68ef 5823 44f5 2e22 f505 0701  Cz..h.X#D.."....
+00000240: a124 1149 bd37 33a6 3252 a310 5236 9d56  .$.I.73.2R..R6.V
+00000250: 5011 2671 2aa7 a313 c212 31b8 e163 daa7  P.&q*.....1..c..
+00000260: ad71 9ca7 83c9 7e8b 906a f0ba bcdc 1b08  .q....~..j......
+00000270: 4f55 54fd a99a fb6e b626 ad76 aa23 de56  OUT....n.&.v.#.V
+00000280: 8d79 9629 98ef a873 8b6e d5fd 0293 ea46  .y.)...s.n.....F
+00000290: 4735 57ad aae6 1acb 6eb6 5a47 3c08 e2df  G5W.....n.ZG<...
+000002a0: 5a3b f424 8eb8 6a96 a422 925b 93c6 db3f  Z;.$..j..".[...?
+000002b0: 69cc 44fe 8ffc ff71 feaf 23ff df4c fe4f  i.D....q..#..L.O
+000002c0: 7735 eefb 6d11 8de2 ce52 fcff 75f3 bf96  w5..m....R..u...
+000002d0: ebe8 98ff 45fe 87df 7fbd f95f 15ff 91ff  ....E......_....
+000002e0: 21fe 3f88 ffff 794e f875 f3bf cace b075  !.?...yN.u.....u
+000002f0: c744 feb7 0ebd 60fe b78d f95f ccff 82ff  .D....`...._....
+00000300: e03f b491 fcbf 38fd 74be 7f70 a1c9 3bb9  .?....8.t..p..;.
+00000310: 1afe 9bae 35cf 7fa7 8bf9 dfb5 e87e c29f  ....5........~..
+00000320: 645c e689 968c c953 f780 e499 0be4 bbf5  d\.....S........
+00000330: 1e4f 0a3c 47c3 f120 10d1 4db6 d030 9dd0  .O.<G.. ..M..0..
+00000340: 73a1 818c 9341 50d0 fadf 5f8c 10f8 0fff  s....AP..._.....
+00000350: 07ff a197 f2ff 7be1 7ba9 fcd7 7563 96ff  ......{.{...uc..
+00000360: a60a 09e0 ff5a 0457 07ff c17f f01f fc07  .....Z.W........
+00000370: ff17 f0ff 6156 b692 fc5f 37e6 f86f 3856  ....aV..._7..o8V
+00000380: d705 ffd7 a1e2 c7e5 99cc e0f2 e03f f80f  .............?..
+00000390: fe83 ffe0 ffb2 275d 5f9d ff1b 8ead aac1  ......']_.......
+000003a0: 7fe4 ffd0 26f0 1fef 7fff 7ffc c7ff 7f80  ....&...........
+000003b0: ff53 fe57 0f81 8723 7fd9 feff 24ff 6d73  .S.W...#....$.ms
+000003c0: eefd 6fe5 fe5d f07f 1dfa ac6e f306 c56d  ..o..].....n...m
+000003d0: de97 2691 cc1f 5ce5 2228 163e 557b 5eb1  ..&...\."(.>U{^.
+000003e0: caab 4ff5 2669 221c 80ff c8ff 7ffd fcdf  ..O.&i".........
+000003f0: 3491 ff6f 3aff 93f1 d2fd ff09 fe1b 33f3  4..o:.........3.
+00000400: ff7a 91ff 1bc5 7231 f07f 0d9a 2cb2 2e7f  .z....r1....,...
+00000410: 7719 c741 56a0 7eba a795 9b5b 4d42 9522  w..AV.~....[MB."
+00000420: a6e2 446b 7ac5 b476 aaf2 db6a 6940 bfa5  ..Dkz..v...ji@..
+00000430: aea0 ba8c 956f f9f7 5bf3 6ff9 d7f5 791a  .....o..[.o...y.
+00000440: f45b af5b 3a50 374d d8f0 86f9 3ceb 3f38  .[.[:P7M....<.?8
+00000450: cc91 88bc 415d b1b5 3db1 9cac 361f d44f  ....A]..=...6..O
+00000460: b0fa 9fab f242 adfa c947 dded 97c9 e7f0  .....B...G......
+00000470: fe9d ff59 fb67 5624 d4dd 94b6 cf2c 4898  ...Y.gV$.....,H.
+00000480: b17d f97a 8499 662f 588e 307f 6649 5935  .}.z..f/X.0.fIY5
+00000490: fd36 de96 8b13 deaa da6d dcde 4110 0441  .6.......m..A..A
+000004a0: 1004 4110 0441 1004 4110 0441 1004 4110  ..A..A..A..A..A.
+000004b0: 0441 1004 41d0 4fa8 7f00 0d8c 2e6e 0078  .A..A.O......n.x
+000004c0: 0000                                     ..
```

