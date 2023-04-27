# Comparing `tmp/normalize_japanese_address-0.0.8.tar.gz` & `tmp/normalize_japanese_address-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "normalize_japanese_address-0.0.8.tar", max compression
+gzip compressed data, was "normalize_japanese_address-0.0.9.tar", max compression
```

## Comparing `normalize_japanese_address-0.0.8.tar` & `normalize_japanese_address-0.0.9.tar`

### file list

```diff
@@ -1,1928 +1,1913 @@
--rw-r--r--   0        0        0     1451 2021-06-17 21:50:23.138179 normalize_japanese_address-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0     1595 2021-06-18 01:21:31.327527 normalize_japanese_address-0.0.8/README.md
--rw-r--r--   0        0        0       80 2021-06-20 22:56:01.989645 normalize_japanese_address-0.0.8/normalize_japanese_address/__init__.py
--rw-r--r--   0        0        0     1903 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/いなべ市.json
--rw-r--r--   0        0        0      184 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/三重郡川越町.json
--rw-r--r--   0        0        0      229 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/三重郡朝日町.json
--rw-r--r--   0        0        0      532 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/三重郡菰野町.json
--rw-r--r--   0        0        0     1480 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/亀山市.json
--rw-r--r--   0        0        0     2293 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/伊勢市.json
--rw-r--r--   0        0        0     3199 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/伊賀市.json
--rw-r--r--   0        0        0      217 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/北牟婁郡紀北町.json
--rw-r--r--   0        0        0      220 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/南牟婁郡御浜町.json
--rw-r--r--   0        0        0      136 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/南牟婁郡紀宝町.json
--rw-r--r--   0        0        0     3562 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/名張市.json
--rw-r--r--   0        0        0      427 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/員弁郡東員町.json
--rw-r--r--   0        0        0     7435 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/四日市市.json
--rw-r--r--   0        0        0      433 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/多気郡多気町.json
--rw-r--r--   0        0        0      397 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/多気郡大台町.json
--rw-r--r--   0        0        0      514 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/多気郡明和町.json
--rw-r--r--   0        0        0      781 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/尾鷲市.json
--rw-r--r--   0        0        0      397 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/度会郡南伊勢町.json
--rw-r--r--   0        0        0      127 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/度会郡大紀町.json
--rw-r--r--   0        0        0      322 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/度会郡度会町.json
--rw-r--r--   0        0        0      295 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/度会郡玉城町.json
--rw-r--r--   0        0        0      709 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/志摩市.json
--rw-r--r--   0        0        0     4072 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/松阪市.json
--rw-r--r--   0        0        0     5695 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/桑名市.json
--rw-r--r--   0        0        0      379 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/桑名郡木曽岬町.json
--rw-r--r--   0        0        0     5707 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/津市.json
--rw-r--r--   0        0        0      895 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/熊野市.json
--rw-r--r--   0        0        0     5635 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/鈴鹿市.json
--rw-r--r--   0        0        0      433 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/鳥羽市.json
--rw-r--r--   0        0        0      250 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/与謝郡与謝野町.json
--rw-r--r--   0        0        0      250 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/与謝郡伊根町.json
--rw-r--r--   0        0        0      229 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/久世郡久御山町.json
--rw-r--r--   0        0        0       46 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/乙訓郡大山崎町.json
--rw-r--r--   0        0        0     4123 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/亀岡市.json
--rw-r--r--   0        0        0     3340 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京丹後市.json
--rw-r--r--   0        0        0    10582 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京田辺市.json
--rw-r--r--   0        0        0     8398 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京都市上京区.json
--rw-r--r--   0        0        0     7804 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京都市下京区.json
--rw-r--r--   0        0        0     7909 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京都市中京区.json
--rw-r--r--   0        0        0    13579 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京都市伏見区.json
--rw-r--r--   0        0        0     8887 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京都市北区.json
--rw-r--r--   0        0        0     6256 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京都市南区.json
--rw-r--r--   0        0        0    12802 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京都市右京区.json
--rw-r--r--   0        0        0     6034 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京都市山科区.json
--rw-r--r--   0        0        0    12220 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京都市左京区.json
--rw-r--r--   0        0        0     4111 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京都市東山区.json
--rw-r--r--   0        0        0     6592 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京都市西京区.json
--rw-r--r--   0        0        0     6052 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/八幡市.json
--rw-r--r--   0        0        0     2386 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/南丹市.json
--rw-r--r--   0        0        0       82 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/向日市.json
--rw-r--r--   0        0        0      115 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/城陽市.json
--rw-r--r--   0        0        0      976 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/宇治市.json
--rw-r--r--   0        0        0     1111 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/宮津市.json
--rw-r--r--   0        0        0     2449 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/木津川市.json
--rw-r--r--   0        0        0      106 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/相楽郡南山城村.json
--rw-r--r--   0        0        0      202 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/相楽郡和束町.json
--rw-r--r--   0        0        0       64 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/相楽郡笠置町.json
--rw-r--r--   0        0        0      634 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/相楽郡精華町.json
--rw-r--r--   0        0        0     3853 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/福知山市.json
--rw-r--r--   0        0        0       52 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/綴喜郡井手町.json
--rw-r--r--   0        0        0      184 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/綴喜郡宇治田原町.json
--rw-r--r--   0        0        0     1726 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/綾部市.json
--rw-r--r--   0        0        0     2494 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/舞鶴市.json
--rw-r--r--   0        0        0      673 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/船井郡京丹波町.json
--rw-r--r--   0        0        0     1315 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/長岡京市.json
--rw-r--r--   0        0        0      190 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/三養基郡みやき町.json
--rw-r--r--   0        0        0       61 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/三養基郡上峰町.json
--rw-r--r--   0        0        0      157 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/三養基郡基山町.json
--rw-r--r--   0        0        0     1768 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/伊万里市.json
--rw-r--r--   0        0        0     5440 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/佐賀市.json
--rw-r--r--   0        0        0     3898 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/唐津市.json
--rw-r--r--   0        0        0      271 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/多久市.json
--rw-r--r--   0        0        0      283 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/嬉野市.json
--rw-r--r--   0        0        0      589 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/小城市.json
--rw-r--r--   0        0        0      349 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/東松浦郡玄海町.json
--rw-r--r--   0        0        0       31 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/杵島郡大町町.json
--rw-r--r--   0        0        0      103 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/杵島郡江北町.json
--rw-r--r--   0        0        0      370 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/杵島郡白石町.json
--rw-r--r--   0        0        0      682 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/武雄市.json
--rw-r--r--   0        0        0      634 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/神埼市.json
--rw-r--r--   0        0        0       82 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/神埼郡吉野ヶ里町.json
--rw-r--r--   0        0        0      157 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/藤津郡太良町.json
--rw-r--r--   0        0        0      850 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/西松浦郡有田町.json
--rw-r--r--   0        0        0     1420 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/鳥栖市.json
--rw-r--r--   0        0        0      193 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/鹿島市.json
--rw-r--r--   0        0        0     3130 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/たつの市.json
--rw-r--r--   0        0        0     3877 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/三木市.json
--rw-r--r--   0        0        0     2659 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/三田市.json
--rw-r--r--   0        0        0     3346 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/丹波市.json
--rw-r--r--   0        0        0     2677 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/丹波篠山市.json
--rw-r--r--   0        0        0     7588 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/伊丹市.json
--rw-r--r--   0        0        0      973 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/佐用郡佐用町.json
--rw-r--r--   0        0        0     3814 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/加古川市.json
--rw-r--r--   0        0        0     1234 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/加古郡播磨町.json
--rw-r--r--   0        0        0      376 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/加古郡稲美町.json
--rw-r--r--   0        0        0      931 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/加東市.json
--rw-r--r--   0        0        0     1540 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/加西市.json
--rw-r--r--   0        0        0     1885 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/南あわじ市.json
--rw-r--r--   0        0        0     1108 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/多可郡多可町.json
--rw-r--r--   0        0        0    17533 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/姫路市.json
--rw-r--r--   0        0        0     2314 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/宍粟市.json
--rw-r--r--   0        0        0     5437 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/宝塚市.json
--rw-r--r--   0        0        0      835 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/小野市.json
--rw-r--r--   0        0        0     8926 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/尼崎市.json
--rw-r--r--   0        0        0     3334 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/川西市.json
--rw-r--r--   0        0        0      835 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/川辺郡猪名川町.json
--rw-r--r--   0        0        0      316 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/揖保郡太子町.json
--rw-r--r--   0        0        0     4303 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/明石市.json
--rw-r--r--   0        0        0     2101 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/朝来市.json
--rw-r--r--   0        0        0     1921 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/洲本市.json
--rw-r--r--   0        0        0      901 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/淡路市.json
--rw-r--r--   0        0        0     1480 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/相生市.json
--rw-r--r--   0        0        0      253 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/神崎郡市川町.json
--rw-r--r--   0        0        0      316 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/神崎郡神河町.json
--rw-r--r--   0        0        0      133 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/神崎郡福崎町.json
--rw-r--r--   0        0        0     7612 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市中央区.json
--rw-r--r--   0        0        0     6304 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市兵庫区.json
--rw-r--r--   0        0        0     6586 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市北区.json
--rw-r--r--   0        0        0     5734 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市垂水区.json
--rw-r--r--   0        0        0     4690 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市東灘区.json
--rw-r--r--   0        0        0     7615 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市灘区.json
--rw-r--r--   0        0        0     6052 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市西区.json
--rw-r--r--   0        0        0     8557 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市長田区.json
--rw-r--r--   0        0        0     6907 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市須磨区.json
--rw-r--r--   0        0        0      505 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/美方郡新温泉町.json
--rw-r--r--   0        0        0     1807 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/美方郡香美町.json
--rw-r--r--   0        0        0      754 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/芦屋市.json
--rw-r--r--   0        0        0     7846 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/西宮市.json
--rw-r--r--   0        0        0      874 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/西脇市.json
--rw-r--r--   0        0        0     4810 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/豊岡市.json
--rw-r--r--   0        0        0      949 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/赤穂市.json
--rw-r--r--   0        0        0      616 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/赤穂郡上郡町.json
--rw-r--r--   0        0        0     1360 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/養父市.json
--rw-r--r--   0        0        0     2971 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/高砂市.json
--rw-r--r--   0        0        0     1396 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/三笠市.json
--rw-r--r--   0        0        0      283 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡上川町.json
--rw-r--r--   0        0        0      151 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡下川町.json
--rw-r--r--   0        0        0      115 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡剣淵町.json
--rw-r--r--   0        0        0      244 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡和寒町.json
--rw-r--r--   0        0        0      904 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡当麻町.json
--rw-r--r--   0        0        0      169 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡愛別町.json
--rw-r--r--   0        0        0     4090 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡新得町.json
--rw-r--r--   0        0        0     1351 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡東川町.json
--rw-r--r--   0        0        0     2533 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡東神楽町.json
--rw-r--r--   0        0        0      739 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡比布町.json
--rw-r--r--   0        0        0     7729 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡清水町.json
--rw-r--r--   0        0        0     1582 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡美瑛町.json
--rw-r--r--   0        0        0     1069 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡鷹栖町.json
--rw-r--r--   0        0        0      241 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/上磯郡木古内町.json
--rw-r--r--   0        0        0      106 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/上磯郡知内町.json
--rw-r--r--   0        0        0      166 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/中川郡中川町.json
--rw-r--r--   0        0        0      973 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/中川郡幕別町.json
--rw-r--r--   0        0        0      469 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/中川郡本別町.json
--rw-r--r--   0        0        0     1258 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/中川郡池田町.json
--rw-r--r--   0        0        0     2989 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/中川郡美深町.json
--rw-r--r--   0        0        0      421 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/中川郡豊頃町.json
--rw-r--r--   0        0        0       67 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/中川郡音威子府村.json
--rw-r--r--   0        0        0      760 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/久遠郡せたな町.json
--rw-r--r--   0        0        0      958 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/亀田郡七飯町.json
--rw-r--r--   0        0        0      670 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/二海郡八雲町.json
--rw-r--r--   0        0        0      823 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/伊達市.json
--rw-r--r--   0        0        0     1156 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/余市郡仁木町.json
--rw-r--r--   0        0        0     1483 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/余市郡余市町.json
--rw-r--r--   0        0        0      145 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/余市郡赤井川村.json
--rw-r--r--   0        0        0     2935 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/函館市.json
--rw-r--r--   0        0        0       19 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/利尻郡利尻富士町.json
--rw-r--r--   0        0        0       22 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/利尻郡利尻町.json
--rw-r--r--   0        0        0      760 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/勇払郡むかわ町.json
--rw-r--r--   0        0        0      136 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/勇払郡占冠村.json
--rw-r--r--   0        0        0      352 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/勇払郡厚真町.json
--rw-r--r--   0        0        0      775 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/勇払郡安平町.json
--rw-r--r--   0        0        0     4669 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/北広島市.json
--rw-r--r--   0        0        0     1825 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/北斗市.json
--rw-r--r--   0        0        0     8485 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/北見市.json
--rw-r--r--   0        0        0     2011 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/十勝郡浦幌町.json
--rw-r--r--   0        0        0     5374 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/千歳市.json
--rw-r--r--   0        0        0     1528 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/厚岸郡厚岸町.json
--rw-r--r--   0        0        0     3028 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/厚岸郡浜中町.json
--rw-r--r--   0        0        0       88 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/古宇郡泊村.json
--rw-r--r--   0        0        0       58 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/古宇郡神恵内村.json
--rw-r--r--   0        0        0      187 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/古平郡古平町.json
--rw-r--r--   0        0        0     9880 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/名寄市.json
--rw-r--r--   0        0        0     1228 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/増毛郡増毛町.json
--rw-r--r--   0        0        0     9493 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/士別市.json
--rw-r--r--   0        0        0     1141 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/夕張市.json
--rw-r--r--   0        0        0      586 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/夕張郡栗山町.json
--rw-r--r--   0        0        0      253 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/夕張郡由仁町.json
--rw-r--r--   0        0        0     1549 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/夕張郡長沼町.json
--rw-r--r--   0        0        0     1630 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/天塩郡天塩町.json
--rw-r--r--   0        0        0      550 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/天塩郡幌延町.json
--rw-r--r--   0        0        0     2857 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/天塩郡豊富町.json
--rw-r--r--   0        0        0      319 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/天塩郡遠別町.json
--rw-r--r--   0        0        0      121 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/奥尻郡奥尻町.json
--rw-r--r--   0        0        0      199 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/宗谷郡猿払村.json
--rw-r--r--   0        0        0     2641 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/室蘭市.json
--rw-r--r--   0        0        0     1930 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/富良野市.json
--rw-r--r--   0        0        0      166 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/寿都郡寿都町.json
--rw-r--r--   0        0        0      316 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/寿都郡黒松内町.json
--rw-r--r--   0        0        0     2476 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/小樽市.json
--rw-r--r--   0        0        0      250 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/山越郡長万部町.json
--rw-r--r--   0        0        0      106 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/岩内郡共和町.json
--rw-r--r--   0        0        0      145 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/岩内郡岩内町.json
--rw-r--r--   0        0        0    19627 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/岩見沢市.json
--rw-r--r--   0        0        0      283 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/島牧郡島牧村.json
--rw-r--r--   0        0        0     1273 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/川上郡弟子屈町.json
--rw-r--r--   0        0        0     2404 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/川上郡標茶町.json
--rw-r--r--   0        0        0    41464 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/帯広市.json
--rw-r--r--   0        0        0      295 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/常呂郡佐呂間町.json
--rw-r--r--   0        0        0      181 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/常呂郡置戸町.json
--rw-r--r--   0        0        0      331 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/常呂郡訓子府町.json
--rw-r--r--   0        0        0      127 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/幌泉郡えりも町.json
--rw-r--r--   0        0        0      637 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/広尾郡大樹町.json
--rw-r--r--   0        0        0     4075 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/広尾郡広尾町.json
--rw-r--r--   0        0        0     3154 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/恵庭市.json
--rw-r--r--   0        0        0      238 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/斜里郡小清水町.json
--rw-r--r--   0        0        0      457 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/斜里郡斜里町.json
--rw-r--r--   0        0        0      133 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/斜里郡清里町.json
--rw-r--r--   0        0        0      319 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/新冠郡新冠町.json
--rw-r--r--   0        0        0     2110 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/日高郡新ひだか町.json
--rw-r--r--   0        0        0    57085 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/旭川市.json
--rw-r--r--   0        0        0      241 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/有珠郡壮瞥町.json
--rw-r--r--   0        0        0    26872 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市中央区.json
--rw-r--r--   0        0        0    28633 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市北区.json
--rw-r--r--   0        0        0     9436 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市南区.json
--rw-r--r--   0        0        0     5422 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市厚別区.json
--rw-r--r--   0        0        0     9232 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市手稲区.json
--rw-r--r--   0        0        0    32248 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市東区.json
--rw-r--r--   0        0        0     5356 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市清田区.json
--rw-r--r--   0        0        0    11434 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市白石区.json
--rw-r--r--   0        0        0    14980 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市西区.json
--rw-r--r--   0        0        0    13618 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市豊平区.json
--rw-r--r--   0        0        0      409 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/松前郡松前町.json
--rw-r--r--   0        0        0      217 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/松前郡福島町.json
--rw-r--r--   0        0        0      214 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/枝幸郡中頓別町.json
--rw-r--r--   0        0        0      535 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/枝幸郡枝幸町.json
--rw-r--r--   0        0        0     1843 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/枝幸郡浜頓別町.json
--rw-r--r--   0        0        0     3319 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/根室市.json
--rw-r--r--   0        0        0      310 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/様似郡様似町.json
--rw-r--r--   0        0        0    22342 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/標津郡中標津町.json
--rw-r--r--   0        0        0     2125 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/標津郡標津町.json
--rw-r--r--   0        0        0      136 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/樺戸郡新十津川町.json
--rw-r--r--   0        0        0      229 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/樺戸郡月形町.json
--rw-r--r--   0        0        0      106 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/樺戸郡浦臼町.json
--rw-r--r--   0        0        0      337 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/檜山郡上ノ国町.json
--rw-r--r--   0        0        0      328 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/檜山郡厚沢部町.json
--rw-r--r--   0        0        0      538 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/檜山郡江差町.json
--rw-r--r--   0        0        0      109 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/歌志内市.json
--rw-r--r--   0        0        0     2014 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/江別市.json
--rw-r--r--   0        0        0      223 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/沙流郡平取町.json
--rw-r--r--   0        0        0     1408 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/沙流郡日高町.json
--rw-r--r--   0        0        0     1153 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/河東郡上士幌町.json
--rw-r--r--   0        0        0     2647 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/河東郡士幌町.json
--rw-r--r--   0        0        0    11446 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/河東郡音更町.json
--rw-r--r--   0        0        0     2857 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/河東郡鹿追町.json
--rw-r--r--   0        0        0     3715 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/河西郡中札内村.json
--rw-r--r--   0        0        0       64 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/河西郡更別村.json
--rw-r--r--   0        0        0    10342 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/河西郡芽室町.json
--rw-r--r--   0        0        0     1255 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/浦河郡浦河町.json
--rw-r--r--   0        0        0      766 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/深川市.json
--rw-r--r--   0        0        0     3307 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/滝川市.json
--rw-r--r--   0        0        0      256 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/瀬棚郡今金町.json
--rw-r--r--   0        0        0      184 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/爾志郡乙部町.json
--rw-r--r--   0        0        0     2350 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/留萌市.json
--rw-r--r--   0        0        0      364 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/留萌郡小平町.json
--rw-r--r--   0        0        0     2635 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/登別市.json
--rw-r--r--   0        0        0     5524 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/白糠郡白糠町.json
--rw-r--r--   0        0        0      925 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/白老郡白老町.json
--rw-r--r--   0        0        0      295 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/目梨郡羅臼町.json
--rw-r--r--   0        0        0     4972 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/石狩市.json
--rw-r--r--   0        0        0      511 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/石狩郡当別町.json
--rw-r--r--   0        0        0      556 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/石狩郡新篠津村.json
--rw-r--r--   0        0        0    12733 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/砂川市.json
--rw-r--r--   0        0        0      382 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/磯谷郡蘭越町.json
--rw-r--r--   0        0        0       37 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/礼文郡礼文町.json
--rw-r--r--   0        0        0     1996 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/稚内市.json
--rw-r--r--   0        0        0      202 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/積丹郡積丹町.json
--rw-r--r--   0        0        0     8965 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/空知郡上富良野町.json
--rw-r--r--   0        0        0       85 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/空知郡上砂川町.json
--rw-r--r--   0        0        0      766 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/空知郡中富良野町.json
--rw-r--r--   0        0        0       82 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/空知郡南富良野町.json
--rw-r--r--   0        0        0     1036 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/空知郡南幌町.json
--rw-r--r--   0        0        0      238 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/空知郡奈井江町.json
--rw-r--r--   0        0        0     2755 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/紋別市.json
--rw-r--r--   0        0        0      427 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/紋別郡湧別町.json
--rw-r--r--   0        0        0     1042 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/紋別郡滝上町.json
--rw-r--r--   0        0        0      121 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/紋別郡興部町.json
--rw-r--r--   0        0        0      145 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/紋別郡西興部村.json
--rw-r--r--   0        0        0     2362 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/紋別郡遠軽町.json
--rw-r--r--   0        0        0      172 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/紋別郡雄武町.json
--rw-r--r--   0        0        0     6358 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/網走市.json
--rw-r--r--   0        0        0     2323 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/網走郡大空町.json
--rw-r--r--   0        0        0      427 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/網走郡津別町.json
--rw-r--r--   0        0        0     2437 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/網走郡美幌町.json
--rw-r--r--   0        0        0     7795 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/美唄市.json
--rw-r--r--   0        0        0     1372 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/芦別市.json
--rw-r--r--   0        0        0      100 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/苫前郡初山別村.json
--rw-r--r--   0        0        0     2017 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/苫前郡羽幌町.json
--rw-r--r--   0        0        0      217 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/苫前郡苫前町.json
--rw-r--r--   0        0        0     6766 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/苫小牧市.json
--rw-r--r--   0        0        0      874 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/茅部郡森町.json
--rw-r--r--   0        0        0       61 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/茅部郡鹿部町.json
--rw-r--r--   0        0        0      247 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/虻田郡ニセコ町.json
--rw-r--r--   0        0        0      154 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/虻田郡京極町.json
--rw-r--r--   0        0        0     3646 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/虻田郡倶知安町.json
--rw-r--r--   0        0        0      241 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/虻田郡喜茂別町.json
--rw-r--r--   0        0        0      244 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/虻田郡洞爺湖町.json
--rw-r--r--   0        0        0      127 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/虻田郡留寿都村.json
--rw-r--r--   0        0        0      184 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/虻田郡真狩村.json
--rw-r--r--   0        0        0      229 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/虻田郡豊浦町.json
--rw-r--r--   0        0        0     4417 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/赤平市.json
--rw-r--r--   0        0        0     1843 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/足寄郡足寄町.json
--rw-r--r--   0        0        0     1147 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/足寄郡陸別町.json
--rw-r--r--   0        0        0      847 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/野付郡別海町.json
--rw-r--r--   0        0        0    16138 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/釧路市.json
--rw-r--r--   0        0        0     4552 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/釧路郡釧路町.json
--rw-r--r--   0        0        0     1060 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/阿寒郡鶴居村.json
--rw-r--r--   0        0        0      112 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/雨竜郡北竜町.json
--rw-r--r--   0        0        0      127 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/雨竜郡妹背牛町.json
--rw-r--r--   0        0        0      361 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/雨竜郡幌加内町.json
--rw-r--r--   0        0        0      577 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/雨竜郡沼田町.json
--rw-r--r--   0        0        0      184 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/雨竜郡秩父別町.json
--rw-r--r--   0        0        0      415 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/雨竜郡雨竜町.json
--rw-r--r--   0        0        0      757 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/いすみ市.json
--rw-r--r--   0        0        0     3166 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/佐倉市.json
--rw-r--r--   0        0        0     2413 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/八千代市.json
--rw-r--r--   0        0        0      415 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/八街市.json
--rw-r--r--   0        0        0      514 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/勝浦市.json
--rw-r--r--   0        0        0      727 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/匝瑳市.json
--rw-r--r--   0        0        0     2176 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/千葉市中央区.json
--rw-r--r--   0        0        0     1156 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/千葉市稲毛区.json
--rw-r--r--   0        0        0     1462 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/千葉市緑区.json
--rw-r--r--   0        0        0      964 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/千葉市美浜区.json
--rw-r--r--   0        0        0     1585 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/千葉市花見川区.json
--rw-r--r--   0        0        0     1930 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/千葉市若葉区.json
--rw-r--r--   0        0        0     1561 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/南房総市.json
--rw-r--r--   0        0        0      814 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/印旛郡栄町.json
--rw-r--r--   0        0        0      556 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/印旛郡酒々井町.json
--rw-r--r--   0        0        0     3130 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/印西市.json
--rw-r--r--   0        0        0     2968 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/君津市.json
--rw-r--r--   0        0        0     1183 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/四街道市.json
--rw-r--r--   0        0        0      829 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/大網白里市.json
--rw-r--r--   0        0        0      601 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/夷隅郡大多喜町.json
--rw-r--r--   0        0        0      139 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/夷隅郡御宿町.json
--rw-r--r--   0        0        0      184 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/安房郡鋸南町.json
--rw-r--r--   0        0        0      886 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/富津市.json
--rw-r--r--   0        0        0      277 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/富里市.json
--rw-r--r--   0        0        0     1183 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/山武市.json
--rw-r--r--   0        0        0      163 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/山武郡九十九里町.json
--rw-r--r--   0        0        0      526 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/山武郡横芝光町.json
--rw-r--r--   0        0        0      235 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/山武郡芝山町.json
--rw-r--r--   0        0        0     6463 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/市原市.json
--rw-r--r--   0        0        0     4318 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/市川市.json
--rw-r--r--   0        0        0     2677 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/成田市.json
--rw-r--r--   0        0        0     2257 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/我孫子市.json
--rw-r--r--   0        0        0      634 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/旭市.json
--rw-r--r--   0        0        0     4060 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/木更津市.json
--rw-r--r--   0        0        0     1153 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/東金市.json
--rw-r--r--   0        0        0     4636 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/松戸市.json
--rw-r--r--   0        0        0     5671 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/柏市.json
--rw-r--r--   0        0        0     2725 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/流山市.json
--rw-r--r--   0        0        0     1531 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/浦安市.json
--rw-r--r--   0        0        0      814 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/白井市.json
--rw-r--r--   0        0        0     1846 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/習志野市.json
--rw-r--r--   0        0        0     6322 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/船橋市.json
--rw-r--r--   0        0        0     1330 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/茂原市.json
--rw-r--r--   0        0        0     1042 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/袖ヶ浦市.json
--rw-r--r--   0        0        0     1468 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/野田市.json
--rw-r--r--   0        0        0     2743 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/銚子市.json
--rw-r--r--   0        0        0     1777 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/鎌ヶ谷市.json
--rw-r--r--   0        0        0       97 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/長生郡一宮町.json
--rw-r--r--   0        0        0      130 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/長生郡白子町.json
--rw-r--r--   0        0        0      184 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/長生郡睦沢町.json
--rw-r--r--   0        0        0      328 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/長生郡長南町.json
--rw-r--r--   0        0        0      262 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/長生郡長柄町.json
--rw-r--r--   0        0        0      277 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/長生郡長生村.json
--rw-r--r--   0        0        0      709 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/館山市.json
--rw-r--r--   0        0        0     1585 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/香取市.json
--rw-r--r--   0        0        0      439 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/香取郡多古町.json
--rw-r--r--   0        0        0      253 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/香取郡東庄町.json
--rw-r--r--   0        0        0      181 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/香取郡神崎町.json
--rw-r--r--   0        0        0      781 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/鴨川市.json
--rw-r--r--   0        0        0      781 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/伊都郡かつらぎ町.json
--rw-r--r--   0        0        0      214 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/伊都郡九度山町.json
--rw-r--r--   0        0        0      307 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/伊都郡高野町.json
--rw-r--r--   0        0        0    11203 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/和歌山市.json
--rw-r--r--   0        0        0      436 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/岩出市.json
--rw-r--r--   0        0        0      349 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/御坊市.json
--rw-r--r--   0        0        0     1981 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/新宮市.json
--rw-r--r--   0        0        0      256 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/日高郡みなべ町.json
--rw-r--r--   0        0        0      406 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/日高郡印南町.json
--rw-r--r--   0        0        0      772 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/日高郡日高川町.json
--rw-r--r--   0        0        0      229 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/日高郡日高町.json
--rw-r--r--   0        0        0      211 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/日高郡由良町.json
--rw-r--r--   0        0        0       79 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/日高郡美浜町.json
--rw-r--r--   0        0        0      298 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/有田市.json
--rw-r--r--   0        0        0      247 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/有田郡広川町.json
--rw-r--r--   0        0        0     1435 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/有田郡有田川町.json
--rw-r--r--   0        0        0      103 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/有田郡湯浅町.json
--rw-r--r--   0        0        0      310 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/東牟婁郡串本町.json
--rw-r--r--   0        0        0       79 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/東牟婁郡北山村.json
--rw-r--r--   0        0        0      403 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/東牟婁郡古座川町.json
--rw-r--r--   0        0        0       31 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/東牟婁郡太地町.json
--rw-r--r--   0        0        0     1012 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/東牟婁郡那智勝浦町.json
--rw-r--r--   0        0        0     1828 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/橋本市.json
--rw-r--r--   0        0        0     1087 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/海南市.json
--rw-r--r--   0        0        0      556 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/海草郡紀美野町.json
--rw-r--r--   0        0        0     2551 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/田辺市.json
--rw-r--r--   0        0        0     1528 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/紀の川市.json
--rw-r--r--   0        0        0      307 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/西牟婁郡すさみ町.json
--rw-r--r--   0        0        0       82 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/西牟婁郡上富田町.json
--rw-r--r--   0        0        0      352 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/西牟婁郡白浜町.json
--rw-r--r--   0        0        0     1372 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市中央区.json
--rw-r--r--   0        0        0      505 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市北区.json
--rw-r--r--   0        0        0     1465 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市南区.json
--rw-r--r--   0        0        0     1066 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市大宮区.json
--rw-r--r--   0        0        0     2185 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市岩槻区.json
--rw-r--r--   0        0        0     1234 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市桜区.json
--rw-r--r--   0        0        0     1609 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市浦和区.json
--rw-r--r--   0        0        0     1201 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市緑区.json
--rw-r--r--   0        0        0      706 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市西区.json
--rw-r--r--   0        0        0     1303 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市見沼区.json
--rw-r--r--   0        0        0     2362 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/ふじみ野市.json
--rw-r--r--   0        0        0     1930 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/三郷市.json
--rw-r--r--   0        0        0     2425 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/上尾市.json
--rw-r--r--   0        0        0     2536 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/久喜市.json
--rw-r--r--   0        0        0      268 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/児玉郡上里町.json
--rw-r--r--   0        0        0      337 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/児玉郡神川町.json
--rw-r--r--   0        0        0      271 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/児玉郡美里町.json
--rw-r--r--   0        0        0     1732 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/入間市.json
--rw-r--r--   0        0        0      100 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/入間郡三芳町.json
--rw-r--r--   0        0        0      934 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/入間郡毛呂山町.json
--rw-r--r--   0        0        0      517 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/入間郡越生町.json
--rw-r--r--   0        0        0      787 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/八潮市.json
--rw-r--r--   0        0        0     2044 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/加須市.json
--rw-r--r--   0        0        0     2350 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/北本市.json
--rw-r--r--   0        0        0     1102 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/北葛飾郡杉戸町.json
--rw-r--r--   0        0        0      487 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/北葛飾郡松伏町.json
--rw-r--r--   0        0        0      652 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/北足立郡伊奈町.json
--rw-r--r--   0        0        0      967 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/南埼玉郡宮代町.json
--rw-r--r--   0        0        0     1636 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/吉川市.json
--rw-r--r--   0        0        0      568 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/和光市.json
--rw-r--r--   0        0        0     1765 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/坂戸市.json
--rw-r--r--   0        0        0      364 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/大里郡寄居町.json
--rw-r--r--   0        0        0     1231 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/富士見市.json
--rw-r--r--   0        0        0     5152 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/川口市.json
--rw-r--r--   0        0        0     4528 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/川越市.json
--rw-r--r--   0        0        0     1066 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/幸手市.json
--rw-r--r--   0        0        0      622 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/志木市.json
--rw-r--r--   0        0        0     1153 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/戸田市.json
--rw-r--r--   0        0        0     3043 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/所沢市.json
--rw-r--r--   0        0        0     1501 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/新座市.json
--rw-r--r--   0        0        0      970 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/日高市.json
--rw-r--r--   0        0        0     2242 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/春日部市.json
--rw-r--r--   0        0        0     1486 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/朝霞市.json
--rw-r--r--   0        0        0     2536 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/本庄市.json
--rw-r--r--   0        0        0     1225 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/東松山市.json
--rw-r--r--   0        0        0      820 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/桶川市.json
--rw-r--r--   0        0        0      286 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/比企郡ときがわ町.json
--rw-r--r--   0        0        0      859 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/比企郡吉見町.json
--rw-r--r--   0        0        0      748 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/比企郡小川町.json
--rw-r--r--   0        0        0      349 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/比企郡嵐山町.json
--rw-r--r--   0        0        0     1009 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/比企郡川島町.json
--rw-r--r--   0        0        0      406 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/比企郡滑川町.json
--rw-r--r--   0        0        0      460 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/比企郡鳩山町.json
--rw-r--r--   0        0        0     1666 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/深谷市.json
--rw-r--r--   0        0        0     3409 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/熊谷市.json
--rw-r--r--   0        0        0     1030 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/狭山市.json
--rw-r--r--   0        0        0      544 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/白岡市.json
--rw-r--r--   0        0        0      898 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/秩父市.json
--rw-r--r--   0        0        0      133 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/秩父郡小鹿野町.json
--rw-r--r--   0        0        0      109 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/秩父郡東秩父村.json
--rw-r--r--   0        0        0       37 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/秩父郡横瀬町.json
--rw-r--r--   0        0        0      166 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/秩父郡皆野町.json
--rw-r--r--   0        0        0      136 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/秩父郡長瀞町.json
--rw-r--r--   0        0        0     1423 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/羽生市.json
--rw-r--r--   0        0        0     2017 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/草加市.json
--rw-r--r--   0        0        0     1186 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/蓮田市.json
--rw-r--r--   0        0        0      523 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/蕨市.json
--rw-r--r--   0        0        0     1525 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/行田市.json
--rw-r--r--   0        0        0     3916 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/越谷市.json
--rw-r--r--   0        0        0     1351 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/飯能市.json
--rw-r--r--   0        0        0     2059 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/鴻巣市.json
--rw-r--r--   0        0        0      826 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/鶴ヶ島市.json
--rw-r--r--   0        0        0     2269 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/中津市.json
--rw-r--r--   0        0        0     2821 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/佐伯市.json
--rw-r--r--   0        0        0     1984 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/別府市.json
--rw-r--r--   0        0        0     1402 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/国東市.json
--rw-r--r--   0        0        0    11974 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/大分市.json
--rw-r--r--   0        0        0     4405 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/宇佐市.json
--rw-r--r--   0        0        0     1372 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/日田市.json
--rw-r--r--   0        0        0      241 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/東国東郡姫島村.json
--rw-r--r--   0        0        0      769 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/杵築市.json
--rw-r--r--   0        0        0      526 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/津久見市.json
--rw-r--r--   0        0        0      169 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/玖珠郡九重町.json
--rw-r--r--   0        0        0      229 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/玖珠郡玖珠町.json
--rw-r--r--   0        0        0     1084 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/由布市.json
--rw-r--r--   0        0        0     1366 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/竹田市.json
--rw-r--r--   0        0        0     1297 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/臼杵市.json
--rw-r--r--   0        0        0     2458 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/豊後大野市.json
--rw-r--r--   0        0        0      610 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/豊後高田市.json
--rw-r--r--   0        0        0      145 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/速見郡日出町.json
--rw-r--r--   0        0        0      706 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/三島郡島本町.json
--rw-r--r--   0        0        0     2752 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/交野市.json
--rw-r--r--   0        0        0    13480 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/八尾市.json
--rw-r--r--   0        0        0      163 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/南河内郡千早赤阪村.json
--rw-r--r--   0        0        0      157 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/南河内郡太子町.json
--rw-r--r--   0        0        0      562 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/南河内郡河南町.json
--rw-r--r--   0        0        0     3571 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/吹田市.json
--rw-r--r--   0        0        0     3130 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/和泉市.json
--rw-r--r--   0        0        0     1060 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/四條畷市.json
--rw-r--r--   0        0        0      634 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市中区.json
--rw-r--r--   0        0        0     1966 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市北区.json
--rw-r--r--   0        0        0     1534 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市南区.json
--rw-r--r--   0        0        0    10045 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市堺区.json
--rw-r--r--   0        0        0      757 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市東区.json
--rw-r--r--   0        0        0      634 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市美原区.json
--rw-r--r--   0        0        0     2971 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市西区.json
--rw-r--r--   0        0        0     2170 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大東市.json
--rw-r--r--   0        0        0     3805 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市中央区.json
--rw-r--r--   0        0        0     2098 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市住之江区.json
--rw-r--r--   0        0        0     2128 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市住吉区.json
--rw-r--r--   0        0        0     2281 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市北区.json
--rw-r--r--   0        0        0     1486 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市城東区.json
--rw-r--r--   0        0        0      988 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市大正区.json
--rw-r--r--   0        0        0     1189 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市天王寺区.json
--rw-r--r--   0        0        0     3049 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市平野区.json
--rw-r--r--   0        0        0      826 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市旭区.json
--rw-r--r--   0        0        0     2026 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市東住吉区.json
--rw-r--r--   0        0        0      904 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市東成区.json
--rw-r--r--   0        0        0     1687 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市東淀川区.json
--rw-r--r--   0        0        0     1174 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市此花区.json
--rw-r--r--   0        0        0     1255 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市浪速区.json
--rw-r--r--   0        0        0     1840 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市淀川区.json
--rw-r--r--   0        0        0     1096 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市港区.json
--rw-r--r--   0        0        0     1735 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市生野区.json
--rw-r--r--   0        0        0      763 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市福島区.json
--rw-r--r--   0        0        0     1195 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市西区.json
--rw-r--r--   0        0        0     1672 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市西成区.json
--rw-r--r--   0        0        0     1159 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市西淀川区.json
--rw-r--r--   0        0        0     1030 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市都島区.json
--rw-r--r--   0        0        0     1441 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市阿倍野区.json
--rw-r--r--   0        0        0     1114 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市鶴見区.json
--rw-r--r--   0        0        0     1693 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪狭山市.json
--rw-r--r--   0        0        0     3505 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/守口市.json
--rw-r--r--   0        0        0     3592 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/富田林市.json
--rw-r--r--   0        0        0     2863 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/寝屋川市.json
--rw-r--r--   0        0        0     2971 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/岸和田市.json
--rw-r--r--   0        0        0     1876 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/摂津市.json
--rw-r--r--   0        0        0    10141 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/東大阪市.json
--rw-r--r--   0        0        0     3406 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/松原市.json
--rw-r--r--   0        0        0     7948 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/枚方市.json
--rw-r--r--   0        0        0     1210 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/柏原市.json
--rw-r--r--   0        0        0     1384 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/池田市.json
--rw-r--r--   0        0        0     1684 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/河内長野市.json
--rw-r--r--   0        0        0     1879 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/泉佐野市.json
--rw-r--r--   0        0        0      520 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/泉北郡忠岡町.json
--rw-r--r--   0        0        0      940 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/泉南市.json
--rw-r--r--   0        0        0      178 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/泉南郡岬町.json
--rw-r--r--   0        0        0     2359 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/泉南郡熊取町.json
--rw-r--r--   0        0        0       94 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/泉南郡田尻町.json
--rw-r--r--   0        0        0     1528 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/泉大津市.json
--rw-r--r--   0        0        0     3442 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/箕面市.json
--rw-r--r--   0        0        0     2596 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/羽曳野市.json
--rw-r--r--   0        0        0     5485 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/茨木市.json
--rw-r--r--   0        0        0     1555 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/藤井寺市.json
--rw-r--r--   0        0        0     7237 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/豊中市.json
--rw-r--r--   0        0        0      304 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/豊能郡能勢町.json
--rw-r--r--   0        0        0      859 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/豊能郡豊能町.json
--rw-r--r--   0        0        0      976 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/貝塚市.json
--rw-r--r--   0        0        0     1261 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/門真市.json
--rw-r--r--   0        0        0      838 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/阪南市.json
--rw-r--r--   0        0        0     6973 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/高槻市.json
--rw-r--r--   0        0        0      997 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/高石市.json
--rw-r--r--   0        0        0     3037 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/五條市.json
--rw-r--r--   0        0        0      934 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/北葛城郡上牧町.json
--rw-r--r--   0        0        0      715 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/北葛城郡広陵町.json
--rw-r--r--   0        0        0      553 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/北葛城郡河合町.json
--rw-r--r--   0        0        0      820 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/北葛城郡王寺町.json
--rw-r--r--   0        0        0       61 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡上北山村.json
--rw-r--r--   0        0        0      151 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡下北山村.json
--rw-r--r--   0        0        0      322 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡下市町.json
--rw-r--r--   0        0        0      868 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡十津川村.json
--rw-r--r--   0        0        0      580 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡吉野町.json
--rw-r--r--   0        0        0      355 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡大淀町.json
--rw-r--r--   0        0        0      352 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡天川村.json
--rw-r--r--   0        0        0      385 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡川上村.json
--rw-r--r--   0        0        0      280 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡東吉野村.json
--rw-r--r--   0        0        0      214 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡野迫川村.json
--rw-r--r--   0        0        0      187 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡黒滝村.json
--rw-r--r--   0        0        0     1609 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/大和郡山市.json
--rw-r--r--   0        0        0     1237 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/大和高田市.json
--rw-r--r--   0        0        0     1036 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/天理市.json
--rw-r--r--   0        0        0    11953 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/奈良市.json
--rw-r--r--   0        0        0     2713 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/宇陀市.json
--rw-r--r--   0        0        0       64 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/宇陀郡御杖村.json
--rw-r--r--   0        0        0      139 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/宇陀郡曽爾村.json
--rw-r--r--   0        0        0      448 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/山辺郡山添村.json
--rw-r--r--   0        0        0     1078 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/御所市.json
--rw-r--r--   0        0        0     1645 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/桜井市.json
--rw-r--r--   0        0        0     1762 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/橿原市.json
--rw-r--r--   0        0        0     2020 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/生駒市.json
--rw-r--r--   0        0        0     1003 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/生駒郡三郷町.json
--rw-r--r--   0        0        0      148 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/生駒郡安堵町.json
--rw-r--r--   0        0        0     1240 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/生駒郡平群町.json
--rw-r--r--   0        0        0     1771 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/生駒郡斑鳩町.json
--rw-r--r--   0        0        0      109 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/磯城郡三宅町.json
--rw-r--r--   0        0        0       91 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/磯城郡川西町.json
--rw-r--r--   0        0        0      691 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/磯城郡田原本町.json
--rw-r--r--   0        0        0      412 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/葛城市.json
--rw-r--r--   0        0        0     1759 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/香芝市.json
--rw-r--r--   0        0        0      484 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/高市郡明日香村.json
--rw-r--r--   0        0        0      382 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/高市郡高取町.json
--rw-r--r--   0        0        0     1012 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/亘理郡亘理町.json
--rw-r--r--   0        0        0      223 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/亘理郡山元町.json
--rw-r--r--   0        0        0     3499 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/仙台市太白区.json
--rw-r--r--   0        0        0     3292 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/仙台市宮城野区.json
--rw-r--r--   0        0        0     3454 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/仙台市泉区.json
--rw-r--r--   0        0        0     2527 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/仙台市若林区.json
--rw-r--r--   0        0        0     5209 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/仙台市青葉区.json
--rw-r--r--   0        0        0     3661 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/伊具郡丸森町.json
--rw-r--r--   0        0        0     3961 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/刈田郡七ヶ宿町.json
--rw-r--r--   0        0        0      238 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/刈田郡蔵王町.json
--rw-r--r--   0        0        0    11290 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/加美郡加美町.json
--rw-r--r--   0        0        0      115 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/加美郡色麻町.json
--rw-r--r--   0        0        0     2173 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/名取市.json
--rw-r--r--   0        0        0     1414 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/塩竈市.json
--rw-r--r--   0        0        0     1270 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/多賀城市.json
--rw-r--r--   0        0        0     4492 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/大崎市.json
--rw-r--r--   0        0        0      454 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/宮城郡七ヶ浜町.json
--rw-r--r--   0        0        0      637 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/宮城郡利府町.json
--rw-r--r--   0        0        0       97 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/宮城郡松島町.json
--rw-r--r--   0        0        0     1114 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/富谷市.json
--rw-r--r--   0        0        0     1729 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/岩沼市.json
--rw-r--r--   0        0        0       40 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/本吉郡南三陸町.json
--rw-r--r--   0        0        0      388 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/東松島市.json
--rw-r--r--   0        0        0      910 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/柴田郡大河原町.json
--rw-r--r--   0        0        0      130 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/柴田郡川崎町.json
--rw-r--r--   0        0        0      121 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/柴田郡村田町.json
--rw-r--r--   0        0        0     1498 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/柴田郡柴田町.json
--rw-r--r--   0        0        0     2872 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/栗原市.json
--rw-r--r--   0        0        0     6532 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/気仙沼市.json
--rw-r--r--   0        0        0      349 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/牡鹿郡女川町.json
--rw-r--r--   0        0        0     6940 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/登米市.json
--rw-r--r--   0        0        0     1597 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/白石市.json
--rw-r--r--   0        0        0     5854 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/石巻市.json
--rw-r--r--   0        0        0      211 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/角田市.json
--rw-r--r--   0        0        0     1867 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/遠田郡涌谷町.json
--rw-r--r--   0        0        0     1009 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/遠田郡美里町.json
--rw-r--r--   0        0        0      940 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/黒川郡大和町.json
--rw-r--r--   0        0        0      178 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/黒川郡大衡村.json
--rw-r--r--   0        0        0      118 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/黒川郡大郷町.json
--rw-r--r--   0        0        0      481 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/えびの市.json
--rw-r--r--   0        0        0      328 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/串間市.json
--rw-r--r--   0        0        0       31 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/児湯郡川南町.json
--rw-r--r--   0        0        0      427 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/児湯郡新富町.json
--rw-r--r--   0        0        0       82 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/児湯郡木城町.json
--rw-r--r--   0        0        0      112 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/児湯郡西米良村.json
--rw-r--r--   0        0        0       16 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/児湯郡都農町.json
--rw-r--r--   0        0        0      103 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/児湯郡高鍋町.json
--rw-r--r--   0        0        0      139 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/北諸県郡三股町.json
--rw-r--r--   0        0        0     6895 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/宮崎市.json
--rw-r--r--   0        0        0      271 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/小林市.json
--rw-r--r--   0        0        0     5611 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/延岡市.json
--rw-r--r--   0        0        0     2404 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/日南市.json
--rw-r--r--   0        0        0     1834 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/日向市.json
--rw-r--r--   0        0        0       70 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/東臼杵郡椎葉村.json
--rw-r--r--   0        0        0      217 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/東臼杵郡美郷町.json
--rw-r--r--   0        0        0       34 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/東臼杵郡諸塚村.json
--rw-r--r--   0        0        0     1165 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/東臼杵郡門川町.json
--rw-r--r--   0        0        0      265 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/東諸県郡国富町.json
--rw-r--r--   0        0        0       46 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/東諸県郡綾町.json
--rw-r--r--   0        0        0       52 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/西臼杵郡五ヶ瀬町.json
--rw-r--r--   0        0        0       64 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/西臼杵郡日之影町.json
--rw-r--r--   0        0        0      160 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/西臼杵郡高千穂町.json
--rw-r--r--   0        0        0       67 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/西諸県郡高原町.json
--rw-r--r--   0        0        0     1069 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/西都市.json
--rw-r--r--   0        0        0     1618 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/都城市.json
--rw-r--r--   0        0        0      589 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/下新川郡入善町.json
--rw-r--r--   0        0        0      448 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/下新川郡朝日町.json
--rw-r--r--   0        0        0     1402 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/中新川郡上市町.json
--rw-r--r--   0        0        0     1405 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/中新川郡立山町.json
--rw-r--r--   0        0        0      109 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/中新川郡舟橋村.json
--rw-r--r--   0        0        0     3085 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/南砺市.json
--rw-r--r--   0        0        0    20935 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/富山市.json
--rw-r--r--   0        0        0     3928 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/射水市.json
--rw-r--r--   0        0        0     1393 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/小矢部市.json
--rw-r--r--   0        0        0     1207 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/氷見市.json
--rw-r--r--   0        0        0     1228 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/滑川市.json
--rw-r--r--   0        0        0     1807 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/砺波市.json
--rw-r--r--   0        0        0     5551 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/高岡市.json
--rw-r--r--   0        0        0     1579 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/魚津市.json
--rw-r--r--   0        0        0     1510 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/黒部市.json
--rw-r--r--   0        0        0     2305 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/下松市.json
--rw-r--r--   0        0        0    13816 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/下関市.json
--rw-r--r--   0        0        0     1927 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/光市.json
--rw-r--r--   0        0        0     5635 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/周南市.json
--rw-r--r--   0        0        0      565 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/大島郡周防大島町.json
--rw-r--r--   0        0        0     5422 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/宇部市.json
--rw-r--r--   0        0        0     4921 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/山口市.json
--rw-r--r--   0        0        0     1429 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/山陽小野田市.json
--rw-r--r--   0        0        0     5089 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/岩国市.json
--rw-r--r--   0        0        0      556 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/柳井市.json
--rw-r--r--   0        0        0       61 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/熊毛郡上関町.json
--rw-r--r--   0        0        0      187 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/熊毛郡平生町.json
--rw-r--r--   0        0        0      202 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/熊毛郡田布施町.json
--rw-r--r--   0        0        0      250 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/玖珂郡和木町.json
--rw-r--r--   0        0        0      655 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/美祢市.json
--rw-r--r--   0        0        0     1228 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/萩市.json
--rw-r--r--   0        0        0      370 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/長門市.json
--rw-r--r--   0        0        0     2194 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/防府市.json
--rw-r--r--   0        0        0      115 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/阿武郡阿武町.json
--rw-r--r--   0        0        0     1531 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/上山市.json
--rw-r--r--   0        0        0      238 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/北村山郡大石田町.json
--rw-r--r--   0        0        0      454 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/南陽市.json
--rw-r--r--   0        0        0     3094 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/天童市.json
--rw-r--r--   0        0        0     1426 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/寒河江市.json
--rw-r--r--   0        0        0     1027 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/尾花沢市.json
--rw-r--r--   0        0        0     8992 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/山形市.json
--rw-r--r--   0        0        0      556 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/新庄市.json
--rw-r--r--   0        0        0       61 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/最上郡大蔵村.json
--rw-r--r--   0        0        0      124 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/最上郡戸沢村.json
--rw-r--r--   0        0        0      184 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/最上郡最上町.json
--rw-r--r--   0        0        0      160 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/最上郡真室川町.json
--rw-r--r--   0        0        0       49 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/最上郡舟形町.json
--rw-r--r--   0        0        0      190 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/最上郡金山町.json
--rw-r--r--   0        0        0      124 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/最上郡鮭川村.json
--rw-r--r--   0        0        0      982 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/村山市.json
--rw-r--r--   0        0        0      148 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/東村山郡中山町.json
--rw-r--r--   0        0        0      424 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/東村山郡山辺町.json
--rw-r--r--   0        0        0     2629 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/東根市.json
--rw-r--r--   0        0        0      316 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/東田川郡三川町.json
--rw-r--r--   0        0        0      694 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/東田川郡庄内町.json
--rw-r--r--   0        0        0      358 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/東置賜郡川西町.json
--rw-r--r--   0        0        0      592 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/東置賜郡高畠町.json
--rw-r--r--   0        0        0     3418 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/米沢市.json
--rw-r--r--   0        0        0      577 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/西村山郡大江町.json
--rw-r--r--   0        0        0      439 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/西村山郡朝日町.json
--rw-r--r--   0        0        0      475 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/西村山郡河北町.json
--rw-r--r--   0        0        0      253 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/西村山郡西川町.json
--rw-r--r--   0        0        0     1573 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/西置賜郡小国町.json
--rw-r--r--   0        0        0      361 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/西置賜郡白鷹町.json
--rw-r--r--   0        0        0      349 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/西置賜郡飯豊町.json
--rw-r--r--   0        0        0     4861 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/酒田市.json
--rw-r--r--   0        0        0      655 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/長井市.json
--rw-r--r--   0        0        0      235 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/飽海郡遊佐町.json
--rw-r--r--   0        0        0     3841 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/鶴岡市.json
--rw-r--r--   0        0        0      319 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/上野原市.json
--rw-r--r--   0        0        0      295 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/中央市.json
--rw-r--r--   0        0        0      139 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/中巨摩郡昭和町.json
--rw-r--r--   0        0        0     1435 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/北杜市.json
--rw-r--r--   0        0        0       70 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/北都留郡丹波山村.json
--rw-r--r--   0        0        0      220 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/北都留郡小菅村.json
--rw-r--r--   0        0        0      709 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/南アルプス市.json
--rw-r--r--   0        0        0      133 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/南巨摩郡南部町.json
--rw-r--r--   0        0        0      232 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/南巨摩郡富士川町.json
--rw-r--r--   0        0        0      208 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/南巨摩郡早川町.json
--rw-r--r--   0        0        0      820 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/南巨摩郡身延町.json
--rw-r--r--   0        0        0      139 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/南都留郡富士河口湖町.json
--rw-r--r--   0        0        0       19 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/南都留郡山中湖村.json
--rw-r--r--   0        0        0       19 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/南都留郡忍野村.json
--rw-r--r--   0        0        0       31 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/南都留郡西桂町.json
--rw-r--r--   0        0        0     1138 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/南都留郡道志村.json
--rw-r--r--   0        0        0     1036 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/南都留郡鳴沢村.json
--rw-r--r--   0        0        0      895 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/大月市.json
--rw-r--r--   0        0        0     1969 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/富士吉田市.json
--rw-r--r--   0        0        0      712 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/山梨市.json
--rw-r--r--   0        0        0      808 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/甲州市.json
--rw-r--r--   0        0        0     3559 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/甲府市.json
--rw-r--r--   0        0        0      406 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/甲斐市.json
--rw-r--r--   0        0        0     1933 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/笛吹市.json
--rw-r--r--   0        0        0      241 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/西八代郡市川三郷町.json
--rw-r--r--   0        0        0      718 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/都留市.json
--rw-r--r--   0        0        0     1090 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/韮崎市.json
--rw-r--r--   0        0        0     1264 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/下呂市.json
--rw-r--r--   0        0        0      355 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/不破郡垂井町.json
--rw-r--r--   0        0        0      121 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/不破郡関ケ原町.json
--rw-r--r--   0        0        0      616 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/中津川市.json
--rw-r--r--   0        0        0       43 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/加茂郡七宗町.json
--rw-r--r--   0        0        0      130 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/加茂郡八百津町.json
--rw-r--r--   0        0        0      169 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/加茂郡坂祝町.json
--rw-r--r--   0        0        0       70 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/加茂郡富加町.json
--rw-r--r--   0        0        0      145 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/加茂郡川辺町.json
--rw-r--r--   0        0        0       28 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/加茂郡東白川村.json
--rw-r--r--   0        0        0      139 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/加茂郡白川町.json
--rw-r--r--   0        0        0     3187 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/可児市.json
--rw-r--r--   0        0        0      193 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/可児郡御嵩町.json
--rw-r--r--   0        0        0    16522 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/各務原市.json
--rw-r--r--   0        0        0     3577 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/土岐市.json
--rw-r--r--   0        0        0     9340 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/多治見市.json
--rw-r--r--   0        0        0    11977 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/大垣市.json
--rw-r--r--   0        0        0      361 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/大野郡白川村.json
--rw-r--r--   0        0        0      217 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/安八郡安八町.json
--rw-r--r--   0        0        0      373 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/安八郡神戸町.json
--rw-r--r--   0        0        0      208 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/安八郡輪之内町.json
--rw-r--r--   0        0        0      355 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/山県市.json
--rw-r--r--   0        0        0    43126 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/岐阜市.json
--rw-r--r--   0        0        0      928 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/恵那市.json
--rw-r--r--   0        0        0      466 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/揖斐郡大野町.json
--rw-r--r--   0        0        0      748 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/揖斐郡揖斐川町.json
--rw-r--r--   0        0        0      256 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/揖斐郡池田町.json
--rw-r--r--   0        0        0      913 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/本巣市.json
--rw-r--r--   0        0        0     1975 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/本巣郡北方町.json
--rw-r--r--   0        0        0     1501 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/海津市.json
--rw-r--r--   0        0        0     1642 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/瑞浪市.json
--rw-r--r--   0        0        0     1024 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/瑞穂市.json
--rw-r--r--   0        0        0     2260 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/美濃加茂市.json
--rw-r--r--   0        0        0      763 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/美濃市.json
--rw-r--r--   0        0        0     6301 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/羽島市.json
--rw-r--r--   0        0        0     2005 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/羽島郡岐南町.json
--rw-r--r--   0        0        0      640 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/羽島郡笠松町.json
--rw-r--r--   0        0        0     2248 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/郡上市.json
--rw-r--r--   0        0        0     5932 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/関市.json
--rw-r--r--   0        0        0     2953 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/飛騨市.json
--rw-r--r--   0        0        0      574 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/養老郡養老町.json
--rw-r--r--   0        0        0     6508 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/高山市.json
--rw-r--r--   0        0        0      277 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/久米郡久米南町.json
--rw-r--r--   0        0        0      658 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/久米郡美咲町.json
--rw-r--r--   0        0        0     1048 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/井原市.json
--rw-r--r--   0        0        0     6946 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/倉敷市.json
--rw-r--r--   0        0        0      586 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/備前市.json
--rw-r--r--   0        0        0      442 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/加賀郡吉備中央町.json
--rw-r--r--   0        0        0      223 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/勝田郡勝央町.json
--rw-r--r--   0        0        0      172 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/勝田郡奈義町.json
--rw-r--r--   0        0        0      370 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/和気郡和気町.json
--rw-r--r--   0        0        0      181 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/小田郡矢掛町.json
--rw-r--r--   0        0        0     2050 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/岡山市中区.json
--rw-r--r--   0        0        0     6463 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/岡山市北区.json
--rw-r--r--   0        0        0     1684 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/岡山市南区.json
--rw-r--r--   0        0        0     2131 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/岡山市東区.json
--rw-r--r--   0        0        0      760 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/新見市.json
--rw-r--r--   0        0        0     2197 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/津山市.json
--rw-r--r--   0        0        0      655 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/浅口市.json
--rw-r--r--   0        0        0       85 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/浅口郡里庄町.json
--rw-r--r--   0        0        0      781 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/瀬戸内市.json
--rw-r--r--   0        0        0     1378 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/玉野市.json
--rw-r--r--   0        0        0     1534 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/真庭市.json
--rw-r--r--   0        0        0      220 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/真庭郡新庄村.json
--rw-r--r--   0        0        0      799 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/笠岡市.json
--rw-r--r--   0        0        0      814 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/総社市.json
--rw-r--r--   0        0        0     1369 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/美作市.json
--rw-r--r--   0        0        0      589 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/苫田郡鏡野町.json
--rw-r--r--   0        0        0       91 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/英田郡西粟倉村.json
--rw-r--r--   0        0        0     1423 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/赤磐市.json
--rw-r--r--   0        0        0       37 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/都窪郡早島町.json
--rw-r--r--   0        0        0     1597 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/高梁市.json
--rw-r--r--   0        0        0     1831 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/一関市.json
--rw-r--r--   0        0        0      391 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/上閉伊郡大槌町.json
--rw-r--r--   0        0        0      220 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/下閉伊郡山田町.json
--rw-r--r--   0        0        0      181 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/下閉伊郡岩泉町.json
--rw-r--r--   0        0        0      874 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/下閉伊郡普代村.json
--rw-r--r--   0        0        0      403 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/下閉伊郡田野畑村.json
--rw-r--r--   0        0        0      922 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/久慈市.json
--rw-r--r--   0        0        0      145 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/九戸郡九戸村.json
--rw-r--r--   0        0        0       88 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/九戸郡洋野町.json
--rw-r--r--   0        0        0      154 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/九戸郡軽米町.json
--rw-r--r--   0        0        0       31 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/九戸郡野田村.json
--rw-r--r--   0        0        0      169 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/二戸市.json
--rw-r--r--   0        0        0      196 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/二戸郡一戸町.json
--rw-r--r--   0        0        0     1651 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/八幡平市.json
--rw-r--r--   0        0        0     2050 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/北上市.json
--rw-r--r--   0        0        0      622 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/和賀郡西和賀町.json
--rw-r--r--   0        0        0      145 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/大船渡市.json
--rw-r--r--   0        0        0     5386 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/奥州市.json
--rw-r--r--   0        0        0     2545 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/宮古市.json
--rw-r--r--   0        0        0      223 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/岩手郡岩手町.json
--rw-r--r--   0        0        0       28 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/岩手郡葛巻町.json
--rw-r--r--   0        0        0      631 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/岩手郡雫石町.json
--rw-r--r--   0        0        0       37 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/気仙郡住田町.json
--rw-r--r--   0        0        0     2794 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/滝沢市.json
--rw-r--r--   0        0        0     7174 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/盛岡市.json
--rw-r--r--   0        0        0      571 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/紫波郡矢巾町.json
--rw-r--r--   0        0        0      751 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/紫波郡紫波町.json
--rw-r--r--   0        0        0       49 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/胆沢郡金ケ崎町.json
--rw-r--r--   0        0        0     3088 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/花巻市.json
--rw-r--r--   0        0        0       19 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/西磐井郡平泉町.json
--rw-r--r--   0        0        0      886 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/遠野市.json
--rw-r--r--   0        0        0     1501 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/釜石市.json
--rw-r--r--   0        0        0       97 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/陸前高田市.json
--rw-r--r--   0        0        0      241 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/仁多郡奥出雲町.json
--rw-r--r--   0        0        0     3886 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/出雲市.json
--rw-r--r--   0        0        0     1201 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/大田市.json
--rw-r--r--   0        0        0     1462 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/安来市.json
--rw-r--r--   0        0        0     4555 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/松江市.json
--rw-r--r--   0        0        0      805 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/江津市.json
--rw-r--r--   0        0        0     1705 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/浜田市.json
--rw-r--r--   0        0        0     1510 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/益田市.json
--rw-r--r--   0        0        0      256 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/邑智郡川本町.json
--rw-r--r--   0        0        0      418 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/邑智郡美郷町.json
--rw-r--r--   0        0        0      352 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/邑智郡邑南町.json
--rw-r--r--   0        0        0      109 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/隠岐郡海士町.json
--rw-r--r--   0        0        0       97 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/隠岐郡知夫村.json
--rw-r--r--   0        0        0       61 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/隠岐郡西ノ島町.json
--rw-r--r--   0        0        0      391 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/隠岐郡隠岐の島町.json
--rw-r--r--   0        0        0     1816 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/雲南市.json
--rw-r--r--   0        0        0      202 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/飯石郡飯南町.json
--rw-r--r--   0        0        0      328 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/鹿足郡吉賀町.json
--rw-r--r--   0        0        0      346 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/鹿足郡津和野町.json
--rw-r--r--   0        0        0     4105 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/三原市.json
--rw-r--r--   0        0        0     2404 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/三次市.json
--rw-r--r--   0        0        0      601 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/世羅郡世羅町.json
--rw-r--r--   0        0        0    11413 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/呉市.json
--rw-r--r--   0        0        0     1273 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/大竹市.json
--rw-r--r--   0        0        0      718 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/安芸郡坂町.json
--rw-r--r--   0        0        0     1075 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/安芸郡府中町.json
--rw-r--r--   0        0        0      643 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/安芸郡海田町.json
--rw-r--r--   0        0        0     1291 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/安芸郡熊野町.json
--rw-r--r--   0        0        0      964 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/安芸高田市.json
--rw-r--r--   0        0        0     2362 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/尾道市.json
--rw-r--r--   0        0        0      673 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/山県郡北広島町.json
--rw-r--r--   0        0        0      433 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/山県郡安芸太田町.json
--rw-r--r--   0        0        0     1873 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/広島市中区.json
--rw-r--r--   0        0        0     3601 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/広島市佐伯区.json
--rw-r--r--   0        0        0     2551 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/広島市南区.json
--rw-r--r--   0        0        0     3016 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/広島市安佐北区.json
--rw-r--r--   0        0        0     3433 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/広島市安佐南区.json
--rw-r--r--   0        0        0     1432 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/広島市安芸区.json
--rw-r--r--   0        0        0     2752 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/広島市東区.json
--rw-r--r--   0        0        0     3025 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/広島市西区.json
--rw-r--r--   0        0        0     2038 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/庄原市.json
--rw-r--r--   0        0        0      688 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/府中市.json
--rw-r--r--   0        0        0     3376 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/廿日市市.json
--rw-r--r--   0        0        0     4276 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/東広島市.json
--rw-r--r--   0        0        0     1426 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/江田島市.json
--rw-r--r--   0        0        0      340 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/神石郡神石高原町.json
--rw-r--r--   0        0        0     8848 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/福山市.json
--rw-r--r--   0        0        0      919 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/竹原市.json
--rw-r--r--   0        0        0       64 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/豊田郡大崎上島町.json
--rw-r--r--   0        0        0     3064 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/三好市.json
--rw-r--r--   0        0        0       64 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/三好郡東みよし町.json
--rw-r--r--   0        0        0       73 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/勝浦郡上勝町.json
--rw-r--r--   0        0        0      121 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/勝浦郡勝浦町.json
--rw-r--r--   0        0        0     2884 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/吉野川市.json
--rw-r--r--   0        0        0       13 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/名東郡佐那河内村.json
--rw-r--r--   0        0        0       49 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/名西郡石井町.json
--rw-r--r--   0        0        0       49 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/名西郡神山町.json
--rw-r--r--   0        0        0      331 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/小松島市.json
--rw-r--r--   0        0        0    10192 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/徳島市.json
--rw-r--r--   0        0        0      148 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/板野郡上板町.json
--rw-r--r--   0        0        0       73 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/板野郡北島町.json
--rw-r--r--   0        0        0       97 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/板野郡松茂町.json
--rw-r--r--   0        0        0      142 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/板野郡板野町.json
--rw-r--r--   0        0        0       85 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/板野郡藍住町.json
--rw-r--r--   0        0        0      295 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/海部郡海陽町.json
--rw-r--r--   0        0        0      118 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/海部郡牟岐町.json
--rw-r--r--   0        0        0      184 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/海部郡美波町.json
--rw-r--r--   0        0        0      310 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/美馬市.json
--rw-r--r--   0        0        0       67 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/美馬郡つるぎ町.json
--rw-r--r--   0        0        0      799 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/那賀郡那賀町.json
--rw-r--r--   0        0        0     1309 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/阿南市.json
--rw-r--r--   0        0        0     2887 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/阿波市.json
--rw-r--r--   0        0        0     1090 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/鳴門市.json
--rw-r--r--   0        0        0      376 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/上浮穴郡久万高原町.json
--rw-r--r--   0        0        0     9199 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/今治市.json
--rw-r--r--   0        0        0      403 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/伊予市.json
--rw-r--r--   0        0        0      328 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/伊予郡松前町.json
--rw-r--r--   0        0        0      307 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/伊予郡砥部町.json
--rw-r--r--   0        0        0     1147 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/八幡浜市.json
--rw-r--r--   0        0        0      145 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/北宇和郡松野町.json
--rw-r--r--   0        0        0      622 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/北宇和郡鬼北町.json
--rw-r--r--   0        0        0      682 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/南宇和郡愛南町.json
--rw-r--r--   0        0        0      373 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/喜多郡内子町.json
--rw-r--r--   0        0        0     1210 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/四国中央市.json
--rw-r--r--   0        0        0     1108 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/大洲市.json
--rw-r--r--   0        0        0     4201 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/宇和島市.json
--rw-r--r--   0        0        0     3394 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/新居浜市.json
--rw-r--r--   0        0        0      280 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/東温市.json
--rw-r--r--   0        0        0    11143 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/松山市.json
--rw-r--r--   0        0        0     2023 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/西予市.json
--rw-r--r--   0        0        0      370 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/西宇和郡伊方町.json
--rw-r--r--   0        0        0     2188 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/西条市.json
--rw-r--r--   0        0        0      277 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/越智郡上島町.json
--rw-r--r--   0        0        0     1540 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/あま市.json
--rw-r--r--   0        0        0     1219 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/みよし市.json
--rw-r--r--   0        0        0     7714 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/一宮市.json
--rw-r--r--   0        0        0     1462 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/丹羽郡大口町.json
--rw-r--r--   0        0        0      109 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/丹羽郡扶桑町.json
--rw-r--r--   0        0        0     8101 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/刈谷市.json
--rw-r--r--   0        0        0      625 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/北名古屋市.json
--rw-r--r--   0        0        0      187 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/北設楽郡東栄町.json
--rw-r--r--   0        0        0      193 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/北設楽郡設楽町.json
--rw-r--r--   0        0        0       67 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/北設楽郡豊根村.json
--rw-r--r--   0        0        0    12397 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/半田市.json
--rw-r--r--   0        0        0     1084 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市中区.json
--rw-r--r--   0        0        0    10321 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市中川区.json
--rw-r--r--   0        0        0     7915 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市中村区.json
--rw-r--r--   0        0        0     6553 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市北区.json
--rw-r--r--   0        0        0     6577 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市千種区.json
--rw-r--r--   0        0        0     7198 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市南区.json
--rw-r--r--   0        0        0     3310 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市名東区.json
--rw-r--r--   0        0        0     2644 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市天白区.json
--rw-r--r--   0        0        0     2623 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市守山区.json
--rw-r--r--   0        0        0     5890 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市昭和区.json
--rw-r--r--   0        0        0     1573 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市東区.json
--rw-r--r--   0        0        0     7003 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市港区.json
--rw-r--r--   0        0        0     1795 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市熱田区.json
--rw-r--r--   0        0        0     6838 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市瑞穂区.json
--rw-r--r--   0        0        0     4048 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市緑区.json
--rw-r--r--   0        0        0     3661 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市西区.json
--rw-r--r--   0        0        0     3706 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/大府市.json
--rw-r--r--   0        0        0     2104 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/安城市.json
--rw-r--r--   0        0        0     3865 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/小牧市.json
--rw-r--r--   0        0        0     3997 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/尾張旭市.json
--rw-r--r--   0        0        0     5140 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/岡崎市.json
--rw-r--r--   0        0        0      724 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/岩倉市.json
--rw-r--r--   0        0        0     6946 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/常滑市.json
--rw-r--r--   0        0        0     5371 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/弥富市.json
--rw-r--r--   0        0        0      700 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/愛知郡東郷町.json
--rw-r--r--   0        0        0      892 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/愛西市.json
--rw-r--r--   0        0        0     1621 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/新城市.json
--rw-r--r--   0        0        0     1396 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/日進市.json
--rw-r--r--   0        0        0    10018 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/春日井市.json
--rw-r--r--   0        0        0     1225 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/東海市.json
--rw-r--r--   0        0        0     7138 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/江南市.json
--rw-r--r--   0        0        0     4894 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/津島市.json
--rw-r--r--   0        0        0      196 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/海部郡大治町.json
--rw-r--r--   0        0        0     1771 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/海部郡蟹江町.json
--rw-r--r--   0        0        0     1888 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/海部郡飛島村.json
--rw-r--r--   0        0        0     5755 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/清須市.json
--rw-r--r--   0        0        0     6481 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/瀬戸市.json
--rw-r--r--   0        0        0     6529 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/犬山市.json
--rw-r--r--   0        0        0     1093 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/田原市.json
--rw-r--r--   0        0        0     3178 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/知多市.json
--rw-r--r--   0        0        0      142 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/知多郡南知多町.json
--rw-r--r--   0        0        0       76 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/知多郡東浦町.json
--rw-r--r--   0        0        0     3064 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/知多郡武豊町.json
--rw-r--r--   0        0        0      538 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/知多郡美浜町.json
--rw-r--r--   0        0        0      508 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/知多郡阿久比町.json
--rw-r--r--   0        0        0     1570 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/知立市.json
--rw-r--r--   0        0        0    13207 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/碧南市.json
--rw-r--r--   0        0        0    10699 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/稲沢市.json
--rw-r--r--   0        0        0      751 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/蒲郡市.json
--rw-r--r--   0        0        0     5254 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/西尾市.json
--rw-r--r--   0        0        0       31 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/西春日井郡豊山町.json
--rw-r--r--   0        0        0     5860 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/豊川市.json
--rw-r--r--   0        0        0      403 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/豊明市.json
--rw-r--r--   0        0        0     6160 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/豊橋市.json
--rw-r--r--   0        0        0    22474 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/豊田市.json
--rw-r--r--   0        0        0     2590 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/長久手市.json
--rw-r--r--   0        0        0      274 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/額田郡幸田町.json
--rw-r--r--   0        0        0     2605 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/高浜市.json
--rw-r--r--   0        0        0      652 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/三島郡出雲崎町.json
--rw-r--r--   0        0        0     3595 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/三条市.json
--rw-r--r--   0        0        0    16429 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/上越市.json
--rw-r--r--   0        0        0      310 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/中魚沼郡津南町.json
--rw-r--r--   0        0        0     2113 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/五泉市.json
--rw-r--r--   0        0        0     4057 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/佐渡市.json
--rw-r--r--   0        0        0      346 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/刈羽郡刈羽村.json
--rw-r--r--   0        0        0     1216 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/加茂市.json
--rw-r--r--   0        0        0      439 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/北蒲原郡聖籠町.json
--rw-r--r--   0        0        0     4642 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/十日町市.json
--rw-r--r--   0        0        0      232 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/南蒲原郡田上町.json
--rw-r--r--   0        0        0     1822 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/南魚沼市.json
--rw-r--r--   0        0        0      166 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/南魚沼郡湯沢町.json
--rw-r--r--   0        0        0     3049 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/妙高市.json
--rw-r--r--   0        0        0     1246 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/小千谷市.json
--rw-r--r--   0        0        0       37 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/岩船郡粟島浦村.json
--rw-r--r--   0        0        0      754 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/岩船郡関川村.json
--rw-r--r--   0        0        0     9991 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市中央区.json
--rw-r--r--   0        0        0     2518 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市北区.json
--rw-r--r--   0        0        0     1927 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市南区.json
--rw-r--r--   0        0        0     4672 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市東区.json
--rw-r--r--   0        0        0     5107 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市江南区.json
--rw-r--r--   0        0        0     2224 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市秋葉区.json
--rw-r--r--   0        0        0     4291 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市西区.json
--rw-r--r--   0        0        0     1522 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市西蒲区.json
--rw-r--r--   0        0        0     3712 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/新発田市.json
--rw-r--r--   0        0        0     3106 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/村上市.json
--rw-r--r--   0        0        0      604 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/東蒲原郡阿賀町.json
--rw-r--r--   0        0        0     4306 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/柏崎市.json
--rw-r--r--   0        0        0     3370 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/燕市.json
--rw-r--r--   0        0        0     3130 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/糸魚川市.json
--rw-r--r--   0        0        0     1192 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/胎内市.json
--rw-r--r--   0        0        0      334 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/西蒲原郡弥彦村.json
--rw-r--r--   0        0        0     1570 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/見附市.json
--rw-r--r--   0        0        0    15622 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/長岡市.json
--rw-r--r--   0        0        0     2377 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/阿賀野市.json
--rw-r--r--   0        0        0     1408 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/魚沼市.json
--rw-r--r--   0        0        0      754 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/あきる野市.json
--rw-r--r--   0        0        0       58 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/三宅村.json
--rw-r--r--   0        0        0     1195 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/三鷹市.json
--rw-r--r--   0        0        0     5299 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/世田谷区.json
--rw-r--r--   0        0        0     2119 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/中央区.json
--rw-r--r--   0        0        0     1633 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/中野区.json
--rw-r--r--   0        0        0       73 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/八丈町.json
--rw-r--r--   0        0        0     3418 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/八王子市.json
--rw-r--r--   0        0        0     2248 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/北区.json
--rw-r--r--   0        0        0     2449 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/千代田区.json
--rw-r--r--   0        0        0     2044 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/台東区.json
--rw-r--r--   0        0        0     2578 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/品川区.json
--rw-r--r--   0        0        0     1390 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/国分寺市.json
--rw-r--r--   0        0        0      493 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/国立市.json
--rw-r--r--   0        0        0     1924 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/墨田区.json
--rw-r--r--   0        0        0     1633 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/多摩市.json
--rw-r--r--   0        0        0      133 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/大島町.json
--rw-r--r--   0        0        0     4411 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/大田区.json
--rw-r--r--   0        0        0     1627 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/小平市.json
--rw-r--r--   0        0        0       79 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/小笠原村.json
--rw-r--r--   0        0        0      907 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/小金井市.json
--rw-r--r--   0        0        0     2941 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/府中市.json
--rw-r--r--   0        0        0       19 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/御蔵島村.json
--rw-r--r--   0        0        0     1294 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/文京区.json
--rw-r--r--   0        0        0     2689 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/新宿区.json
--rw-r--r--   0        0        0      151 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/新島村.json
--rw-r--r--   0        0        0     2083 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/日野市.json
--rw-r--r--   0        0        0     1636 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/昭島市.json
--rw-r--r--   0        0        0     2860 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/杉並区.json
--rw-r--r--   0        0        0     1528 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/東久留米市.json
--rw-r--r--   0        0        0     1426 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/東大和市.json
--rw-r--r--   0        0        0     1135 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/東村山市.json
--rw-r--r--   0        0        0     2392 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/板橋区.json
--rw-r--r--   0        0        0     1177 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/武蔵村山市.json
--rw-r--r--   0        0        0     1108 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/武蔵野市.json
--rw-r--r--   0        0        0     4015 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/江戸川区.json
--rw-r--r--   0        0        0     2830 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/江東区.json
--rw-r--r--   0        0        0      829 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/清瀬市.json
--rw-r--r--   0        0        0     1507 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/渋谷区.json
--rw-r--r--   0        0        0     2296 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/港区.json
--rw-r--r--   0        0        0      862 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/狛江市.json
--rw-r--r--   0        0        0     3625 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/町田市.json
--rw-r--r--   0        0        0     1768 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/目黒区.json
--rw-r--r--   0        0        0      394 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/神津島村.json
--rw-r--r--   0        0        0      364 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/福生市.json
--rw-r--r--   0        0        0      406 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/稲城市.json
--rw-r--r--   0        0        0     1579 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/立川市.json
--rw-r--r--   0        0        0     4171 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/練馬区.json
--rw-r--r--   0        0        0      985 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/羽村市.json
--rw-r--r--   0        0        0     1081 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/荒川区.json
--rw-r--r--   0        0        0     3040 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/葛飾区.json
--rw-r--r--   0        0        0      139 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/西多摩郡奥多摩町.json
--rw-r--r--   0        0        0       34 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/西多摩郡日の出町.json
--rw-r--r--   0        0        0      127 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/西多摩郡檜原村.json
--rw-r--r--   0        0        0      454 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/西多摩郡瑞穂町.json
--rw-r--r--   0        0        0     2326 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/西東京市.json
--rw-r--r--   0        0        0     2407 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/調布市.json
--rw-r--r--   0        0        0     1639 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/豊島区.json
--rw-r--r--   0        0        0     5176 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/足立区.json
--rw-r--r--   0        0        0       22 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/青ヶ島村.json
--rw-r--r--   0        0        0     2722 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/青梅市.json
--rw-r--r--   0        0        0      754 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/さくら市.json
--rw-r--r--   0        0        0      871 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/下都賀郡壬生町.json
--rw-r--r--   0        0        0      157 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/下都賀郡野木町.json
--rw-r--r--   0        0        0     1222 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/下野市.json
--rw-r--r--   0        0        0     1582 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/佐野市.json
--rw-r--r--   0        0        0      382 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/塩谷郡塩谷町.json
--rw-r--r--   0        0        0      589 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/塩谷郡高根沢町.json
--rw-r--r--   0        0        0     1444 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/大田原市.json
--rw-r--r--   0        0        0     8506 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/宇都宮市.json
--rw-r--r--   0        0        0     3421 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/小山市.json
--rw-r--r--   0        0        0     1813 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/日光市.json
--rw-r--r--   0        0        0     2317 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/栃木市.json
--rw-r--r--   0        0        0      487 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/河内郡上三川町.json
--rw-r--r--   0        0        0     1918 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/真岡市.json
--rw-r--r--   0        0        0      472 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/矢板市.json
--rw-r--r--   0        0        0      271 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/芳賀郡市貝町.json
--rw-r--r--   0        0        0      343 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/芳賀郡益子町.json
--rw-r--r--   0        0        0      376 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/芳賀郡芳賀町.json
--rw-r--r--   0        0        0      628 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/芳賀郡茂木町.json
--rw-r--r--   0        0        0     2344 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/足利市.json
--rw-r--r--   0        0        0     2602 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/那須塩原市.json
--rw-r--r--   0        0        0      628 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/那須烏山市.json
--rw-r--r--   0        0        0      298 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/那須郡那珂川町.json
--rw-r--r--   0        0        0      439 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/那須郡那須町.json
--rw-r--r--   0        0        0     1810 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/鹿沼市.json
--rw-r--r--   0        0        0     1474 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/うるま市.json
--rw-r--r--   0        0        0      214 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/中頭郡中城村.json
--rw-r--r--   0        0        0      172 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/中頭郡北中城村.json
--rw-r--r--   0        0        0      292 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/中頭郡北谷町.json
--rw-r--r--   0        0        0      100 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/中頭郡嘉手納町.json
--rw-r--r--   0        0        0      343 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/中頭郡西原町.json
--rw-r--r--   0        0        0      286 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/中頭郡読谷村.json
--rw-r--r--   0        0        0       16 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/八重山郡与那国町.json
--rw-r--r--   0        0        0      169 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/八重山郡竹富町.json
--rw-r--r--   0        0        0      898 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/南城市.json
--rw-r--r--   0        0        0     1432 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/名護市.json
--rw-r--r--   0        0        0      253 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/国頭郡今帰仁村.json
--rw-r--r--   0        0        0       73 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/国頭郡伊江村.json
--rw-r--r--   0        0        0      244 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/国頭郡国頭村.json
--rw-r--r--   0        0        0      211 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/国頭郡大宜味村.json
--rw-r--r--   0        0        0       52 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/国頭郡宜野座村.json
--rw-r--r--   0        0        0      154 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/国頭郡恩納村.json
--rw-r--r--   0        0        0      346 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/国頭郡本部町.json
--rw-r--r--   0        0        0       76 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/国頭郡東村.json
--rw-r--r--   0        0        0       37 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/国頭郡金武町.json
--rw-r--r--   0        0        0     1408 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/宜野湾市.json
--rw-r--r--   0        0        0       49 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/宮古島市.json
--rw-r--r--   0        0        0       37 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/宮古郡多良間村.json
--rw-r--r--   0        0        0       61 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/島尻郡与那原町.json
--rw-r--r--   0        0        0      355 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/島尻郡久米島町.json
--rw-r--r--   0        0        0       64 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/島尻郡伊平屋村.json
--rw-r--r--   0        0        0       67 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/島尻郡伊是名村.json
--rw-r--r--   0        0        0      298 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/島尻郡八重瀬町.json
--rw-r--r--   0        0        0       43 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/島尻郡北大東村.json
--rw-r--r--   0        0        0       70 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/島尻郡南大東村.json
--rw-r--r--   0        0        0      154 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/島尻郡南風原町.json
--rw-r--r--   0        0        0       67 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/島尻郡座間味村.json
--rw-r--r--   0        0        0      433 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/島尻郡渡名喜村.json
--rw-r--r--   0        0        0       43 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/島尻郡渡嘉敷村.json
--rw-r--r--   0        0        0       28 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/島尻郡粟国村.json
--rw-r--r--   0        0        0     2641 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/沖縄市.json
--rw-r--r--   0        0        0     1393 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/浦添市.json
--rw-r--r--   0        0        0      373 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/石垣市.json
--rw-r--r--   0        0        0      655 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/糸満市.json
--rw-r--r--   0        0        0      406 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/豊見城市.json
--rw-r--r--   0        0        0     4318 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/那覇市.json
--rw-r--r--   0        0        0     9202 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/大津市.json
--rw-r--r--   0        0        0     1021 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/守山市.json
--rw-r--r--   0        0        0     1909 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/彦根市.json
--rw-r--r--   0        0        0      415 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/愛知郡愛荘町.json
--rw-r--r--   0        0        0     3679 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/東近江市.json
--rw-r--r--   0        0        0     1291 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/栗東市.json
--rw-r--r--   0        0        0     2545 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/湖南市.json
--rw-r--r--   0        0        0      607 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/犬上郡多賀町.json
--rw-r--r--   0        0        0      193 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/犬上郡甲良町.json
--rw-r--r--   0        0        0      256 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/犬上郡豊郷町.json
--rw-r--r--   0        0        0     3631 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/甲賀市.json
--rw-r--r--   0        0        0      967 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/米原市.json
--rw-r--r--   0        0        0     2575 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/草津市.json
--rw-r--r--   0        0        0     1060 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/蒲生郡日野町.json
--rw-r--r--   0        0        0      358 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/蒲生郡竜王町.json
--rw-r--r--   0        0        0     2947 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/近江八幡市.json
--rw-r--r--   0        0        0      652 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/野洲市.json
--rw-r--r--   0        0        0     4744 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/長浜市.json
--rw-r--r--   0        0        0     3100 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/高島市.json
--rw-r--r--   0        0        0      301 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/上天草市.json
--rw-r--r--   0        0        0      148 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/上益城郡嘉島町.json
--rw-r--r--   0        0        0      946 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/上益城郡山都町.json
--rw-r--r--   0        0        0      196 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/上益城郡御船町.json
--rw-r--r--   0        0        0      478 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/上益城郡甲佐町.json
--rw-r--r--   0        0        0      334 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/上益城郡益城町.json
--rw-r--r--   0        0        0      463 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/下益城郡美里町.json
--rw-r--r--   0        0        0     1039 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/人吉市.json
--rw-r--r--   0        0        0     3247 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/八代市.json
--rw-r--r--   0        0        0      172 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/八代郡氷川町.json
--rw-r--r--   0        0        0      106 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/合志市.json
--rw-r--r--   0        0        0     1687 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/天草市.json
--rw-r--r--   0        0        0       88 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/天草郡苓北町.json
--rw-r--r--   0        0        0      817 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/宇土市.json
--rw-r--r--   0        0        0     1423 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/宇城市.json
--rw-r--r--   0        0        0     1315 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/山鹿市.json
--rw-r--r--   0        0        0     1405 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/水俣市.json
--rw-r--r--   0        0        0     3601 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/熊本市中央区.json
--rw-r--r--   0        0        0     3277 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/熊本市北区.json
--rw-r--r--   0        0        0     3766 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/熊本市南区.json
--rw-r--r--   0        0        0     3766 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/熊本市東区.json
--rw-r--r--   0        0        0     2386 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/熊本市西区.json
--rw-r--r--   0        0        0      997 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/玉名市.json
--rw-r--r--   0        0        0      319 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/玉名郡南関町.json
--rw-r--r--   0        0        0      394 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/玉名郡和水町.json
--rw-r--r--   0        0        0      160 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/玉名郡玉東町.json
--rw-r--r--   0        0        0      193 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/玉名郡長洲町.json
--rw-r--r--   0        0        0      151 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/球磨郡あさぎり町.json
--rw-r--r--   0        0        0       19 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/球磨郡五木村.json
--rw-r--r--   0        0        0       82 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/球磨郡多良木町.json
--rw-r--r--   0        0        0       31 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/球磨郡山江村.json
--rw-r--r--   0        0        0       46 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/球磨郡水上村.json
--rw-r--r--   0        0        0       79 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/球磨郡球磨村.json
--rw-r--r--   0        0        0       82 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/球磨郡相良村.json
--rw-r--r--   0        0        0      100 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/球磨郡錦町.json
--rw-r--r--   0        0        0      904 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/荒尾市.json
--rw-r--r--   0        0        0     1012 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/菊池市.json
--rw-r--r--   0        0        0      409 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/菊池郡大津町.json
--rw-r--r--   0        0        0      649 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/菊池郡菊陽町.json
--rw-r--r--   0        0        0       85 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/葦北郡津奈木町.json
--rw-r--r--   0        0        0      724 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/葦北郡芦北町.json
--rw-r--r--   0        0        0      592 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/阿蘇市.json
--rw-r--r--   0        0        0       52 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/阿蘇郡南小国町.json
--rw-r--r--   0        0        0      166 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/阿蘇郡南阿蘇村.json
--rw-r--r--   0        0        0       91 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/阿蘇郡小国町.json
--rw-r--r--   0        0        0       76 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/阿蘇郡産山村.json
--rw-r--r--   0        0        0       76 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/阿蘇郡西原村.json
--rw-r--r--   0        0        0      217 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/阿蘇郡高森町.json
--rw-r--r--   0        0        0      670 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/かほく市.json
--rw-r--r--   0        0        0     3178 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/七尾市.json
--rw-r--r--   0        0        0     4507 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/加賀市.json
--rw-r--r--   0        0        0     4255 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/小松市.json
--rw-r--r--   0        0        0      967 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/河北郡内灘町.json
--rw-r--r--   0        0        0     1432 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/河北郡津幡町.json
--rw-r--r--   0        0        0     1291 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/珠洲市.json
--rw-r--r--   0        0        0     5479 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/白山市.json
--rw-r--r--   0        0        0      928 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/羽咋市.json
--rw-r--r--   0        0        0      508 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/羽咋郡宝達志水町.json
--rw-r--r--   0        0        0     1213 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/羽咋郡志賀町.json
--rw-r--r--   0        0        0     1570 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/能美市.json
--rw-r--r--   0        0        0      166 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/能美郡川北町.json
--rw-r--r--   0        0        0     3628 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/輪島市.json
--rw-r--r--   0        0        0     1843 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/野々市市.json
--rw-r--r--   0        0        0    15160 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/金沢市.json
--rw-r--r--   0        0        0      790 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/鳳珠郡穴水町.json
--rw-r--r--   0        0        0     1357 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/鳳珠郡能登町.json
--rw-r--r--   0        0        0      493 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/鹿島郡中能登町.json
--rw-r--r--   0        0        0      529 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/三浦市.json
--rw-r--r--   0        0        0       64 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/三浦郡葉山町.json
--rw-r--r--   0        0        0      289 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/中郡二宮町.json
--rw-r--r--   0        0        0      301 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/中郡大磯町.json
--rw-r--r--   0        0        0     1018 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/伊勢原市.json
--rw-r--r--   0        0        0      268 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/南足柄市.json
--rw-r--r--   0        0        0     2359 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/厚木市.json
--rw-r--r--   0        0        0     2452 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/大和市.json
--rw-r--r--   0        0        0     1993 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/小田原市.json
--rw-r--r--   0        0        0     1444 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市中原区.json
--rw-r--r--   0        0        0     1927 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市多摩区.json
--rw-r--r--   0        0        0     1480 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市宮前区.json
--rw-r--r--   0        0        0     2356 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市川崎区.json
--rw-r--r--   0        0        0     1165 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市幸区.json
--rw-r--r--   0        0        0     1258 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市高津区.json
--rw-r--r--   0        0        0     2350 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市麻生区.json
--rw-r--r--   0        0        0     2314 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/平塚市.json
--rw-r--r--   0        0        0     1387 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/座間市.json
--rw-r--r--   0        0        0      172 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/愛甲郡愛川町.json
--rw-r--r--   0        0        0       25 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/愛甲郡清川村.json
--rw-r--r--   0        0        0     4939 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市中区.json
--rw-r--r--   0        0        0     1060 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市保土ケ谷区.json
--rw-r--r--   0        0        0     3034 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市南区.json
--rw-r--r--   0        0        0      700 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市戸塚区.json
--rw-r--r--   0        0        0     1246 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市旭区.json
--rw-r--r--   0        0        0      925 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市栄区.json
--rw-r--r--   0        0        0     1246 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市泉区.json
--rw-r--r--   0        0        0     1999 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市港北区.json
--rw-r--r--   0        0        0     1696 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市港南区.json
--rw-r--r--   0        0        0     1078 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市瀬谷区.json
--rw-r--r--   0        0        0     1261 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市磯子区.json
--rw-r--r--   0        0        0     2194 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市神奈川区.json
--rw-r--r--   0        0        0     1228 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市緑区.json
--rw-r--r--   0        0        0     1309 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市西区.json
--rw-r--r--   0        0        0     1783 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市都筑区.json
--rw-r--r--   0        0        0     1873 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市金沢区.json
--rw-r--r--   0        0        0     1516 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市青葉区.json
--rw-r--r--   0        0        0     2500 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市鶴見区.json
--rw-r--r--   0        0        0     6814 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横須賀市.json
--rw-r--r--   0        0        0     1951 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/海老名市.json
--rw-r--r--   0        0        0     3028 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/相模原市中央区.json
--rw-r--r--   0        0        0     2488 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/相模原市南区.json
--rw-r--r--   0        0        0     1588 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/相模原市緑区.json
--rw-r--r--   0        0        0     1543 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/秦野市.json
--rw-r--r--   0        0        0     2443 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/綾瀬市.json
--rw-r--r--   0        0        0     2017 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/茅ヶ崎市.json
--rw-r--r--   0        0        0     4000 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/藤沢市.json
--rw-r--r--   0        0        0      148 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/足柄上郡中井町.json
--rw-r--r--   0        0        0       85 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/足柄上郡大井町.json
--rw-r--r--   0        0        0      148 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/足柄上郡山北町.json
--rw-r--r--   0        0        0       46 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/足柄上郡松田町.json
--rw-r--r--   0        0        0      190 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/足柄上郡開成町.json
--rw-r--r--   0        0        0      265 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/足柄下郡湯河原町.json
--rw-r--r--   0        0        0       16 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/足柄下郡真鶴町.json
--rw-r--r--   0        0        0      190 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/足柄下郡箱根町.json
--rw-r--r--   0        0        0      937 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/逗子市.json
--rw-r--r--   0        0        0     2779 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/鎌倉市.json
--rw-r--r--   0        0        0      562 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/高座郡寒川町.json
--rw-r--r--   0        0        0     1576 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/あわら市.json
--rw-r--r--   0        0        0      772 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/三方上中郡若狭町.json
--rw-r--r--   0        0        0      301 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/三方郡美浜町.json
--rw-r--r--   0        0        0     1054 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/丹生郡越前町.json
--rw-r--r--   0        0        0      469 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/今立郡池田町.json
--rw-r--r--   0        0        0     2272 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/勝山市.json
--rw-r--r--   0        0        0      568 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/南条郡南越前町.json
--rw-r--r--   0        0        0     1474 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/吉田郡永平寺町.json
--rw-r--r--   0        0        0     8296 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/坂井市.json
--rw-r--r--   0        0        0     2278 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/大野市.json
--rw-r--r--   0        0        0      604 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/大飯郡おおい町.json
--rw-r--r--   0        0        0      562 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/大飯郡高浜町.json
--rw-r--r--   0        0        0     1816 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/小浜市.json
--rw-r--r--   0        0        0     1942 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/敦賀市.json
--rw-r--r--   0        0        0    11728 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/福井市.json
--rw-r--r--   0        0        0     3541 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/越前市.json
--rw-r--r--   0        0        0     2533 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/鯖江市.json
--rw-r--r--   0        0        0      562 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/うきは市.json
--rw-r--r--   0        0        0      949 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/みやま市.json
--rw-r--r--   0        0        0      244 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/三井郡大刀洗町.json
--rw-r--r--   0        0        0      310 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/三潴郡大木町.json
--rw-r--r--   0        0        0     1447 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/中間市.json
--rw-r--r--   0        0        0     4222 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/久留米市.json
--rw-r--r--   0        0        0      796 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/京都郡みやこ町.json
--rw-r--r--   0        0        0      970 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/京都郡苅田町.json
--rw-r--r--   0        0        0      964 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/八女市.json
--rw-r--r--   0        0        0      199 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/八女郡広川町.json
--rw-r--r--   0        0        0     2272 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市八幡東区.json
--rw-r--r--   0        0        0     7804 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市八幡西区.json
--rw-r--r--   0        0        0     4000 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市小倉北区.json
--rw-r--r--   0        0        0     7045 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市小倉南区.json
--rw-r--r--   0        0        0     1501 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市戸畑区.json
--rw-r--r--   0        0        0     2770 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市若松区.json
--rw-r--r--   0        0        0     3481 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市門司区.json
--rw-r--r--   0        0        0     1201 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/古賀市.json
--rw-r--r--   0        0        0      142 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/嘉穂郡桂川町.json
--rw-r--r--   0        0        0      367 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/嘉麻市.json
--rw-r--r--   0        0        0      547 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/大川市.json
--rw-r--r--   0        0        0     4135 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/大牟田市.json
--rw-r--r--   0        0        0     2743 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/大野城市.json
--rw-r--r--   0        0        0     2239 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/太宰府市.json
--rw-r--r--   0        0        0     3106 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/宗像市.json
--rw-r--r--   0        0        0      313 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/宮若市.json
--rw-r--r--   0        0        0      829 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/小郡市.json
--rw-r--r--   0        0        0     5146 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/春日市.json
--rw-r--r--   0        0        0     1093 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/朝倉市.json
--rw-r--r--   0        0        0       73 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/朝倉郡東峰村.json
--rw-r--r--   0        0        0      355 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/朝倉郡筑前町.json
--rw-r--r--   0        0        0     1450 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/柳川市.json
--rw-r--r--   0        0        0      352 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/田川市.json
--rw-r--r--   0        0        0       37 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/田川郡大任町.json
--rw-r--r--   0        0        0       64 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/田川郡川崎町.json
--rw-r--r--   0        0        0      124 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/田川郡添田町.json
--rw-r--r--   0        0        0       64 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/田川郡福智町.json
--rw-r--r--   0        0        0       19 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/田川郡糸田町.json
--rw-r--r--   0        0        0       37 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/田川郡赤村.json
--rw-r--r--   0        0        0       97 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/田川郡香春町.json
--rw-r--r--   0        0        0      529 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/直方市.json
--rw-r--r--   0        0        0     2221 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市中央区.json
--rw-r--r--   0        0        0     2962 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市南区.json
--rw-r--r--   0        0        0     4048 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市博多区.json
--rw-r--r--   0        0        0     1726 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市城南区.json
--rw-r--r--   0        0        0     3064 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市早良区.json
--rw-r--r--   0        0        0     4573 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市東区.json
--rw-r--r--   0        0        0     2776 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市西区.json
--rw-r--r--   0        0        0     1942 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/福津市.json
--rw-r--r--   0        0        0      643 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/筑後市.json
--rw-r--r--   0        0        0     2983 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/筑紫野市.json
--rw-r--r--   0        0        0      304 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/築上郡上毛町.json
--rw-r--r--   0        0        0      154 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/築上郡吉富町.json
--rw-r--r--   0        0        0      673 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/築上郡築上町.json
--rw-r--r--   0        0        0       46 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/糟屋郡久山町.json
--rw-r--r--   0        0        0     1594 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/糟屋郡宇美町.json
--rw-r--r--   0        0        0     1303 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/糟屋郡志免町.json
--rw-r--r--   0        0        0     1165 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/糟屋郡新宮町.json
--rw-r--r--   0        0        0      169 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/糟屋郡篠栗町.json
--rw-r--r--   0        0        0      994 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/糟屋郡粕屋町.json
--rw-r--r--   0        0        0       94 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/糟屋郡須恵町.json
--rw-r--r--   0        0        0     2365 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/糸島市.json
--rw-r--r--   0        0        0     2116 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/行橋市.json
--rw-r--r--   0        0        0      877 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/豊前市.json
--rw-r--r--   0        0        0     1381 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/遠賀郡岡垣町.json
--rw-r--r--   0        0        0     1339 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/遠賀郡水巻町.json
--rw-r--r--   0        0        0      181 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/遠賀郡芦屋町.json
--rw-r--r--   0        0        0      643 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/遠賀郡遠賀町.json
--rw-r--r--   0        0        0     1915 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/那珂川市.json
--rw-r--r--   0        0        0       97 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/鞍手郡小竹町.json
--rw-r--r--   0        0        0      238 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/鞍手郡鞍手町.json
--rw-r--r--   0        0        0      994 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/飯塚市.json
--rw-r--r--   0        0        0     7375 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/いわき市.json
--rw-r--r--   0        0        0     4162 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/二本松市.json
--rw-r--r--   0        0        0     1816 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/伊達市.json
--rw-r--r--   0        0        0      328 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/伊達郡国見町.json
--rw-r--r--   0        0        0     1078 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/伊達郡川俣町.json
--rw-r--r--   0        0        0     1072 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/伊達郡桑折町.json
--rw-r--r--   0        0        0     5080 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/会津若松市.json
--rw-r--r--   0        0        0      352 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/南会津郡下郷町.json
--rw-r--r--   0        0        0      739 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/南会津郡南会津町.json
--rw-r--r--   0        0        0      373 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/南会津郡只見町.json
--rw-r--r--   0        0        0      256 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/南会津郡檜枝岐村.json
--rw-r--r--   0        0        0     4357 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/南相馬市.json
--rw-r--r--   0        0        0      307 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/双葉郡双葉町.json
--rw-r--r--   0        0        0      130 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/双葉郡大熊町.json
--rw-r--r--   0        0        0      478 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/双葉郡富岡町.json
--rw-r--r--   0        0        0       37 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/双葉郡川内村.json
--rw-r--r--   0        0        0      214 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/双葉郡広野町.json
--rw-r--r--   0        0        0      184 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/双葉郡楢葉町.json
--rw-r--r--   0        0        0      526 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/双葉郡浪江町.json
--rw-r--r--   0        0        0       64 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/双葉郡葛尾村.json
--rw-r--r--   0        0        0     3970 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/喜多方市.json
--rw-r--r--   0        0        0      199 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/大沼郡三島町.json
--rw-r--r--   0        0        0     2497 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/大沼郡会津美里町.json
--rw-r--r--   0        0        0      151 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/大沼郡昭和村.json
--rw-r--r--   0        0        0      280 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/大沼郡金山町.json
--rw-r--r--   0        0        0       19 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/安達郡大玉村.json
--rw-r--r--   0        0        0      211 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/岩瀬郡天栄村.json
--rw-r--r--   0        0        0      556 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/岩瀬郡鏡石町.json
--rw-r--r--   0        0        0      121 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/本宮市.json
--rw-r--r--   0        0        0      394 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/東白川郡塙町.json
--rw-r--r--   0        0        0      568 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/東白川郡棚倉町.json
--rw-r--r--   0        0        0      247 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/東白川郡矢祭町.json
--rw-r--r--   0        0        0      145 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/東白川郡鮫川村.json
--rw-r--r--   0        0        0     1837 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/河沼郡会津坂下町.json
--rw-r--r--   0        0        0      331 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/河沼郡柳津町.json
--rw-r--r--   0        0        0      184 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/河沼郡湯川村.json
--rw-r--r--   0        0        0     1063 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/田村市.json
--rw-r--r--   0        0        0     1531 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/田村郡三春町.json
--rw-r--r--   0        0        0      307 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/田村郡小野町.json
--rw-r--r--   0        0        0     3292 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/白河市.json
--rw-r--r--   0        0        0      709 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/相馬市.json
--rw-r--r--   0        0        0      115 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/相馬郡新地町.json
--rw-r--r--   0        0        0      190 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/相馬郡飯舘村.json
--rw-r--r--   0        0        0      124 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/石川郡古殿町.json
--rw-r--r--   0        0        0      214 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/石川郡平田村.json
--rw-r--r--   0        0        0      271 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/石川郡浅川町.json
--rw-r--r--   0        0        0      196 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/石川郡玉川村.json
--rw-r--r--   0        0        0     1033 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/石川郡石川町.json
--rw-r--r--   0        0        0     2503 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/福島市.json
--rw-r--r--   0        0        0       76 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/耶麻郡北塩原村.json
--rw-r--r--   0        0        0     3697 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/耶麻郡猪苗代町.json
--rw-r--r--   0        0        0       61 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/耶麻郡磐梯町.json
--rw-r--r--   0        0        0      367 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/耶麻郡西会津町.json
--rw-r--r--   0        0        0       97 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/西白河郡中島村.json
--rw-r--r--   0        0        0       85 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/西白河郡泉崎村.json
--rw-r--r--   0        0        0      958 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/西白河郡矢吹町.json
--rw-r--r--   0        0        0      328 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/西白河郡西郷村.json
--rw-r--r--   0        0        0     7645 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/郡山市.json
--rw-r--r--   0        0        0     1555 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/須賀川市.json
--rw-r--r--   0        0        0      445 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/にかほ市.json
--rw-r--r--   0        0        0      583 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/仙北市.json
--rw-r--r--   0        0        0      262 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/仙北郡美郷町.json
--rw-r--r--   0        0        0      865 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/北秋田市.json
--rw-r--r--   0        0        0       91 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/北秋田郡上小阿仁村.json
--rw-r--r--   0        0        0      562 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/南秋田郡五城目町.json
--rw-r--r--   0        0        0      148 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/南秋田郡井川町.json
--rw-r--r--   0        0        0      364 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/南秋田郡八郎潟町.json
--rw-r--r--   0        0        0      337 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/南秋田郡大潟村.json
--rw-r--r--   0        0        0     1795 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/大仙市.json
--rw-r--r--   0        0        0     2323 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/大館市.json
--rw-r--r--   0        0        0      178 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/山本郡三種町.json
--rw-r--r--   0        0        0      184 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/山本郡八峰町.json
--rw-r--r--   0        0        0       46 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/山本郡藤里町.json
--rw-r--r--   0        0        0     2506 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/横手市.json
--rw-r--r--   0        0        0     2611 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/湯沢市.json
--rw-r--r--   0        0        0      289 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/潟上市.json
--rw-r--r--   0        0        0     2956 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/由利本荘市.json
--rw-r--r--   0        0        0      838 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/男鹿市.json
--rw-r--r--   0        0        0    10048 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/秋田市.json
--rw-r--r--   0        0        0     2296 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/能代市.json
--rw-r--r--   0        0        0       34 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/雄勝郡東成瀬村.json
--rw-r--r--   0        0        0     1447 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/雄勝郡羽後町.json
--rw-r--r--   0        0        0      202 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/鹿角市.json
--rw-r--r--   0        0        0       67 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/鹿角郡小坂町.json
--rw-r--r--   0        0        0      424 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/みどり市.json
--rw-r--r--   0        0        0     1906 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/伊勢崎市.json
--rw-r--r--   0        0        0      406 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/佐波郡玉村町.json
--rw-r--r--   0        0        0      442 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/利根郡みなかみ町.json
--rw-r--r--   0        0        0      145 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/利根郡川場村.json
--rw-r--r--   0        0        0      115 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/利根郡昭和村.json
--rw-r--r--   0        0        0      220 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/利根郡片品村.json
--rw-r--r--   0        0        0     4900 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/前橋市.json
--rw-r--r--   0        0        0      130 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/北群馬郡吉岡町.json
--rw-r--r--   0        0        0       85 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/北群馬郡榛東村.json
--rw-r--r--   0        0        0      421 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/吾妻郡中之条町.json
--rw-r--r--   0        0        0      169 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/吾妻郡嬬恋村.json
--rw-r--r--   0        0        0      355 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/吾妻郡東吾妻町.json
--rw-r--r--   0        0        0       31 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/吾妻郡草津町.json
--rw-r--r--   0        0        0      184 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/吾妻郡長野原町.json
--rw-r--r--   0        0        0       31 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/吾妻郡高山村.json
--rw-r--r--   0        0        0      109 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/多野郡上野村.json
--rw-r--r--   0        0        0      229 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/多野郡神流町.json
--rw-r--r--   0        0        0     2131 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/太田市.json
--rw-r--r--   0        0        0     1096 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/安中市.json
--rw-r--r--   0        0        0      637 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/富岡市.json
--rw-r--r--   0        0        0     2134 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/桐生市.json
--rw-r--r--   0        0        0     1210 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/沼田市.json
--rw-r--r--   0        0        0      832 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/渋川市.json
--rw-r--r--   0        0        0      310 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/甘楽郡下仁田町.json
--rw-r--r--   0        0        0      190 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/甘楽郡南牧村.json
--rw-r--r--   0        0        0      196 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/甘楽郡甘楽町.json
--rw-r--r--   0        0        0      463 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/藤岡市.json
--rw-r--r--   0        0        0      220 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/邑楽郡千代田町.json
--rw-r--r--   0        0        0      955 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/邑楽郡大泉町.json
--rw-r--r--   0        0        0      166 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/邑楽郡明和町.json
--rw-r--r--   0        0        0      400 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/邑楽郡板倉町.json
--rw-r--r--   0        0        0      187 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/邑楽郡邑楽町.json
--rw-r--r--   0        0        0     1093 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/館林市.json
--rw-r--r--   0        0        0     3979 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/高崎市.json
--rw-r--r--   0        0        0      769 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/かすみがうら市.json
--rw-r--r--   0        0        0     1345 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/つくばみらい市.json
--rw-r--r--   0        0        0     3967 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/つくば市.json
--rw-r--r--   0        0        0     2335 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/ひたちなか市.json
--rw-r--r--   0        0        0      958 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/下妻市.json
--rw-r--r--   0        0        0      649 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/久慈郡大子町.json
--rw-r--r--   0        0        0      556 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/北相馬郡利根町.json
--rw-r--r--   0        0        0     1564 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/北茨城市.json
--rw-r--r--   0        0        0     2002 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/取手市.json
--rw-r--r--   0        0        0     1339 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/古河市.json
--rw-r--r--   0        0        0     3310 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/土浦市.json
--rw-r--r--   0        0        0      586 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/坂東市.json
--rw-r--r--   0        0        0     1495 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/守谷市.json
--rw-r--r--   0        0        0      544 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/小美玉市.json
--rw-r--r--   0        0        0     1336 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/常総市.json
--rw-r--r--   0        0        0      853 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/常陸大宮市.json
--rw-r--r--   0        0        0     1327 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/常陸太田市.json
--rw-r--r--   0        0        0     5428 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/日立市.json
--rw-r--r--   0        0        0      559 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/東茨城郡城里町.json
--rw-r--r--   0        0        0      112 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/東茨城郡大洗町.json
--rw-r--r--   0        0        0      694 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/東茨城郡茨城町.json
--rw-r--r--   0        0        0     1321 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/桜川市.json
--rw-r--r--   0        0        0     3763 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/水戸市.json
--rw-r--r--   0        0        0      622 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/潮来市.json
--rw-r--r--   0        0        0     1285 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/牛久市.json
--rw-r--r--   0        0        0      298 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/猿島郡五霞町.json
--rw-r--r--   0        0        0      448 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/猿島郡境町.json
--rw-r--r--   0        0        0     1906 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/石岡市.json
--rw-r--r--   0        0        0     1894 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/神栖市.json
--rw-r--r--   0        0        0     1015 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/稲敷市.json
--rw-r--r--   0        0        0      301 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/稲敷郡河内町.json
--rw-r--r--   0        0        0      553 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/稲敷郡美浦村.json
--rw-r--r--   0        0        0     1030 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/稲敷郡阿見町.json
--rw-r--r--   0        0        0      874 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/笠間市.json
--rw-r--r--   0        0        0     1846 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/筑西市.json
--rw-r--r--   0        0        0      940 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/結城市.json
--rw-r--r--   0        0        0      778 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/結城郡八千代町.json
--rw-r--r--   0        0        0      547 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/行方市.json
--rw-r--r--   0        0        0      433 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/那珂市.json
--rw-r--r--   0        0        0      604 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/那珂郡東海村.json
--rw-r--r--   0        0        0      664 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/鉾田市.json
--rw-r--r--   0        0        0      745 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/高萩市.json
--rw-r--r--   0        0        0     1528 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/鹿嶋市.json
--rw-r--r--   0        0        0     2146 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/龍ヶ崎市.json
--rw-r--r--   0        0        0     1717 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/五島市.json
--rw-r--r--   0        0        0     4723 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/佐世保市.json
--rw-r--r--   0        0        0      316 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/北松浦郡佐々町.json
--rw-r--r--   0        0        0      163 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/北松浦郡小値賀町.json
--rw-r--r--   0        0        0      811 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/南島原市.json
--rw-r--r--   0        0        0      547 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/南松浦郡新上五島町.json
--rw-r--r--   0        0        0     2710 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/壱岐市.json
--rw-r--r--   0        0        0     1567 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/大村市.json
--rw-r--r--   0        0        0     2341 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/対馬市.json
--rw-r--r--   0        0        0     2209 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/島原市.json
--rw-r--r--   0        0        0     1549 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/平戸市.json
--rw-r--r--   0        0        0      214 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/東彼杵郡川棚町.json
--rw-r--r--   0        0        0      304 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/東彼杵郡東彼杵町.json
--rw-r--r--   0        0        0      256 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/東彼杵郡波佐見町.json
--rw-r--r--   0        0        0      412 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/松浦市.json
--rw-r--r--   0        0        0      115 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/西彼杵郡時津町.json
--rw-r--r--   0        0        0      187 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/西彼杵郡長与町.json
--rw-r--r--   0        0        0     1285 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/西海市.json
--rw-r--r--   0        0        0     2734 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/諫早市.json
--rw-r--r--   0        0        0     7453 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/長崎市.json
--rw-r--r--   0        0        0     1429 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/雲仙市.json
--rw-r--r--   0        0        0       37 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/上伊那郡中川村.json
--rw-r--r--   0        0        0       22 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/上伊那郡南箕輪村.json
--rw-r--r--   0        0        0      145 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/上伊那郡宮田村.json
--rw-r--r--   0        0        0       88 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/上伊那郡箕輪町.json
--rw-r--r--   0        0        0      226 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/上伊那郡辰野町.json
--rw-r--r--   0        0        0       52 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/上伊那郡飯島町.json
--rw-r--r--   0        0        0      154 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/上水内郡信濃町.json
--rw-r--r--   0        0        0       67 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/上水内郡小川村.json
--rw-r--r--   0        0        0      286 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/上水内郡飯綱町.json
--rw-r--r--   0        0        0     1552 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/上田市.json
--rw-r--r--   0        0        0      157 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/上高井郡小布施町.json
--rw-r--r--   0        0        0       61 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/上高井郡高山村.json
--rw-r--r--   0        0        0       19 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡下條村.json
--rw-r--r--   0        0        0      259 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡喬木村.json
--rw-r--r--   0        0        0       61 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡売木村.json
--rw-r--r--   0        0        0       34 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡大鹿村.json
--rw-r--r--   0        0        0       28 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡天龍村.json
--rw-r--r--   0        0        0       88 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡平谷村.json
--rw-r--r--   0        0        0       43 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡松川町.json
--rw-r--r--   0        0        0      328 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡根羽村.json
--rw-r--r--   0        0        0      196 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡泰阜村.json
--rw-r--r--   0        0        0       31 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡豊丘村.json
--rw-r--r--   0        0        0       64 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡阿南町.json
--rw-r--r--   0        0        0       64 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡阿智村.json
--rw-r--r--   0        0        0       73 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡高森町.json
--rw-r--r--   0        0        0       43 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/下水内郡栄村.json
--rw-r--r--   0        0        0       79 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/下高井郡山ノ内町.json
--rw-r--r--   0        0        0       49 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/下高井郡木島平村.json
--rw-r--r--   0        0        0      112 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/下高井郡野沢温泉村.json
--rw-r--r--   0        0        0      817 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/中野市.json
--rw-r--r--   0        0        0      709 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/伊那市.json
--rw-r--r--   0        0        0      793 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/佐久市.json
--rw-r--r--   0        0        0      127 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/北佐久郡御代田町.json
--rw-r--r--   0        0        0      148 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/北佐久郡立科町.json
--rw-r--r--   0        0        0      136 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/北佐久郡軽井沢町.json
--rw-r--r--   0        0        0       67 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/北安曇郡小谷村.json
--rw-r--r--   0        0        0       40 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/北安曇郡松川村.json
--rw-r--r--   0        0        0       76 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/北安曇郡池田町.json
--rw-r--r--   0        0        0       31 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/北安曇郡白馬村.json
--rw-r--r--   0        0        0      742 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/千曲市.json
--rw-r--r--   0        0        0      169 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/南佐久郡佐久穂町.json
--rw-r--r--   0        0        0      148 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/南佐久郡北相木村.json
--rw-r--r--   0        0        0       97 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/南佐久郡南牧村.json
--rw-r--r--   0        0        0     3253 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/南佐久郡南相木村.json
--rw-r--r--   0        0        0       82 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/南佐久郡小海町.json
--rw-r--r--   0        0        0      127 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/南佐久郡川上村.json
--rw-r--r--   0        0        0       97 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/埴科郡坂城町.json
--rw-r--r--   0        0        0      712 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/塩尻市.json
--rw-r--r--   0        0        0       64 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/大町市.json
--rw-r--r--   0        0        0      292 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/安曇野市.json
--rw-r--r--   0        0        0       40 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/小県郡長和町.json
--rw-r--r--   0        0        0      109 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/小県郡青木村.json
--rw-r--r--   0        0        0     1474 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/小諸市.json
--rw-r--r--   0        0        0     2032 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/岡谷市.json
--rw-r--r--   0        0        0      373 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/木曽郡上松町.json
--rw-r--r--   0        0        0       28 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/木曽郡南木曽町.json
--rw-r--r--   0        0        0       58 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/木曽郡大桑村.json
--rw-r--r--   0        0        0       79 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/木曽郡木曽町.json
--rw-r--r--   0        0        0       46 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/木曽郡木祖村.json
--rw-r--r--   0        0        0      184 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/木曽郡王滝村.json
--rw-r--r--   0        0        0      199 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/東御市.json
--rw-r--r--   0        0        0       70 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/東筑摩郡山形村.json
--rw-r--r--   0        0        0       67 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/東筑摩郡朝日村.json
--rw-r--r--   0        0        0       85 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/東筑摩郡生坂村.json
--rw-r--r--   0        0        0       61 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/東筑摩郡筑北村.json
--rw-r--r--   0        0        0       13 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/東筑摩郡麻績村.json
--rw-r--r--   0        0        0     3763 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/松本市.json
--rw-r--r--   0        0        0      193 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/茅野市.json
--rw-r--r--   0        0        0      811 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/諏訪市.json
--rw-r--r--   0        0        0      856 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/諏訪郡下諏訪町.json
--rw-r--r--   0        0        0      166 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/諏訪郡原村.json
--rw-r--r--   0        0        0       46 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/諏訪郡富士見町.json
--rw-r--r--   0        0        0     5533 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/長野市.json
--rw-r--r--   0        0        0      790 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/須坂市.json
--rw-r--r--   0        0        0      436 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/飯山市.json
--rw-r--r--   0        0        0     3259 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/飯田市.json
--rw-r--r--   0        0        0      208 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/駒ヶ根市.json
--rw-r--r--   0        0        0     1516 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/つがる市.json
--rw-r--r--   0        0        0     1003 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/むつ市.json
--rw-r--r--   0        0        0      292 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/三戸郡三戸町.json
--rw-r--r--   0        0        0     2227 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/三戸郡五戸町.json
--rw-r--r--   0        0        0      430 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/三戸郡南部町.json
--rw-r--r--   0        0        0       31 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/三戸郡新郷村.json
--rw-r--r--   0        0        0      145 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/三戸郡田子町.json
--rw-r--r--   0        0        0      451 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/三戸郡階上町.json
--rw-r--r--   0        0        0     3400 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/三沢市.json
--rw-r--r--   0        0        0     2221 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/上北郡おいらせ町.json
--rw-r--r--   0        0        0     3532 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/上北郡七戸町.json
--rw-r--r--   0        0        0       88 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/上北郡六ヶ所村.json
--rw-r--r--   0        0        0      313 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/上北郡六戸町.json
--rw-r--r--   0        0        0     3058 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/上北郡東北町.json
--rw-r--r--   0        0        0      817 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/上北郡横浜町.json
--rw-r--r--   0        0        0     1543 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/上北郡野辺地町.json
--rw-r--r--   0        0        0       31 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/下北郡佐井村.json
--rw-r--r--   0        0        0       31 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/下北郡大間町.json
--rw-r--r--   0        0        0      196 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/下北郡東通村.json
--rw-r--r--   0        0        0       52 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/下北郡風間浦村.json
--rw-r--r--   0        0        0      148 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/中津軽郡西目屋村.json
--rw-r--r--   0        0        0     1855 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/五所川原市.json
--rw-r--r--   0        0        0     5323 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/八戸市.json
--rw-r--r--   0        0        0      283 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/北津軽郡中泊町.json
--rw-r--r--   0        0        0      511 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/北津軽郡板柳町.json
--rw-r--r--   0        0        0      277 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/北津軽郡鶴田町.json
--rw-r--r--   0        0        0     1201 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/十和田市.json
--rw-r--r--   0        0        0      241 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/南津軽郡大鰐町.json
--rw-r--r--   0        0        0      319 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/南津軽郡田舎館村.json
--rw-r--r--   0        0        0      544 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/南津軽郡藤崎町.json
--rw-r--r--   0        0        0      622 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/平川市.json
--rw-r--r--   0        0        0    11401 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/弘前市.json
--rw-r--r--   0        0        0      160 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/東津軽郡今別町.json
--rw-r--r--   0        0        0     2440 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/東津軽郡外ケ浜町.json
--rw-r--r--   0        0        0      433 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/東津軽郡平内町.json
--rw-r--r--   0        0        0      115 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/東津軽郡蓬田村.json
--rw-r--r--   0        0        0      388 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/西津軽郡深浦町.json
--rw-r--r--   0        0        0      583 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/西津軽郡鰺ヶ沢町.json
--rw-r--r--   0        0        0     5821 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/青森市.json
--rw-r--r--   0        0        0     2179 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/黒石市.json
--rw-r--r--   0        0        0     1282 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/三島市.json
--rw-r--r--   0        0        0      481 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/下田市.json
--rw-r--r--   0        0        0      964 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/伊東市.json
--rw-r--r--   0        0        0      481 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/伊豆の国市.json
--rw-r--r--   0        0        0      553 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/伊豆市.json
--rw-r--r--   0        0        0      208 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/周智郡森町.json
--rw-r--r--   0        0        0     1015 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/富士宮市.json
--rw-r--r--   0        0        0     2755 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/富士市.json
--rw-r--r--   0        0        0     2017 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/島田市.json
--rw-r--r--   0        0        0      139 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/御前崎市.json
--rw-r--r--   0        0        0      721 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/御殿場市.json
--rw-r--r--   0        0        0     2224 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/掛川市.json
--rw-r--r--   0        0        0       46 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/榛原郡吉田町.json
--rw-r--r--   0        0        0      217 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/榛原郡川根本町.json
--rw-r--r--   0        0        0     2191 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/沼津市.json
--rw-r--r--   0        0        0     3115 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市中区.json
--rw-r--r--   0        0        0     1216 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市北区.json
--rw-r--r--   0        0        0      760 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市南区.json
--rw-r--r--   0        0        0     1201 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市天竜区.json
--rw-r--r--   0        0        0      862 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市東区.json
--rw-r--r--   0        0        0      559 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市浜北区.json
--rw-r--r--   0        0        0      754 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市西区.json
--rw-r--r--   0        0        0      502 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/湖西市.json
--rw-r--r--   0        0        0     2170 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/焼津市.json
--rw-r--r--   0        0        0      526 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/熱海市.json
--rw-r--r--   0        0        0      508 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/牧之原市.json
--rw-r--r--   0        0        0      157 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/田方郡函南町.json
--rw-r--r--   0        0        0     2293 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/磐田市.json
--rw-r--r--   0        0        0      562 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/菊川市.json
--rw-r--r--   0        0        0     3517 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/藤枝市.json
--rw-r--r--   0        0        0     1525 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/袋井市.json
--rw-r--r--   0        0        0      385 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/裾野市.json
--rw-r--r--   0        0        0      256 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/賀茂郡南伊豆町.json
--rw-r--r--   0        0        0       49 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/賀茂郡東伊豆町.json
--rw-r--r--   0        0        0      217 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/賀茂郡松崎町.json
--rw-r--r--   0        0        0      145 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/賀茂郡河津町.json
--rw-r--r--   0        0        0       70 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/賀茂郡西伊豆町.json
--rw-r--r--   0        0        0     4327 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/静岡市清水区.json
--rw-r--r--   0        0        0     6016 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/静岡市葵区.json
--rw-r--r--   0        0        0     2902 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/静岡市駿河区.json
--rw-r--r--   0        0        0      235 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/駿東郡小山町.json
--rw-r--r--   0        0        0      145 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/駿東郡清水町.json
--rw-r--r--   0        0        0      178 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/駿東郡長泉町.json
--rw-r--r--   0        0        0      364 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/香川県/さぬき市.json
--rw-r--r--   0        0        0      751 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/香川県/三豊市.json
--rw-r--r--   0        0        0     2482 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/香川県/丸亀市.json
--rw-r--r--   0        0        0      286 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/香川県/仲多度郡まんのう町.json
--rw-r--r--   0        0        0      640 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/香川県/仲多度郡多度津町.json
--rw-r--r--   0        0        0       79 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/香川県/仲多度郡琴平町.json
--rw-r--r--   0        0        0      802 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/香川県/善通寺市.json
--rw-r--r--   0        0        0     1669 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/香川県/坂出市.json
--rw-r--r--   0        0        0      217 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/香川県/小豆郡土庄町.json
--rw-r--r--   0        0        0      232 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/香川県/小豆郡小豆島町.json
--rw-r--r--   0        0        0      202 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/香川県/木田郡三木町.json
--rw-r--r--   0        0        0      322 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/香川県/東かがわ市.json
--rw-r--r--   0        0        0      181 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/香川県/綾歌郡宇多津町.json
--rw-r--r--   0        0        0      157 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/香川県/綾歌郡綾川町.json
--rw-r--r--   0        0        0     1516 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/香川県/観音寺市.json
--rw-r--r--   0        0        0      598 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/香川県/香川郡直島町.json
--rw-r--r--   0        0        0     3817 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/香川県/高松市.json
--rw-r--r--   0        0        0     1495 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/南国市.json
--rw-r--r--   0        0        0      967 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/吾川郡いの町.json
--rw-r--r--   0        0        0      760 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/吾川郡仁淀川町.json
--rw-r--r--   0        0        0     2479 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/四万十市.json
--rw-r--r--   0        0        0      376 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/土佐市.json
--rw-r--r--   0        0        0      643 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/土佐清水市.json
--rw-r--r--   0        0        0      244 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/土佐郡土佐町.json
--rw-r--r--   0        0        0      172 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/土佐郡大川村.json
--rw-r--r--   0        0        0      745 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/安芸市.json
--rw-r--r--   0        0        0      301 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/安芸郡北川村.json
--rw-r--r--   0        0        0       19 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/安芸郡奈半利町.json
--rw-r--r--   0        0        0      268 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/安芸郡安田町.json
--rw-r--r--   0        0        0       76 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/安芸郡東洋町.json
--rw-r--r--   0        0        0     2269 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/安芸郡田野町.json
--rw-r--r--   0        0        0       58 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/安芸郡芸西村.json
--rw-r--r--   0        0        0       34 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/安芸郡馬路村.json
--rw-r--r--   0        0        0      145 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/室戸市.json
--rw-r--r--   0        0        0     1426 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/宿毛市.json
--rw-r--r--   0        0        0      220 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/幡多郡三原村.json
--rw-r--r--   0        0        0      418 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/幡多郡大月町.json
--rw-r--r--   0        0        0      397 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/幡多郡黒潮町.json
--rw-r--r--   0        0        0      556 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/長岡郡大豊町.json
--rw-r--r--   0        0        0      193 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/長岡郡本山町.json
--rw-r--r--   0        0        0      910 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/須崎市.json
--rw-r--r--   0        0        0     1237 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/香南市.json
--rw-r--r--   0        0        0     3604 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/香美市.json
--rw-r--r--   0        0        0      658 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/高岡郡中土佐町.json
--rw-r--r--   0        0        0      217 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/高岡郡佐川町.json
--rw-r--r--   0        0        0     1318 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/高岡郡四万十町.json
--rw-r--r--   0        0        0      115 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/高岡郡日高村.json
--rw-r--r--   0        0        0      571 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/高岡郡檮原町.json
--rw-r--r--   0        0        0      220 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/高岡郡津野町.json
--rw-r--r--   0        0        0      313 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/高岡郡越知町.json
--rw-r--r--   0        0        0     6865 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/高知市.json
--rw-r--r--   0        0        0     2248 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/倉吉市.json
--rw-r--r--   0        0        0      907 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/八頭郡八頭町.json
--rw-r--r--   0        0        0      652 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/八頭郡智頭町.json
--rw-r--r--   0        0        0      394 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/八頭郡若桜町.json
--rw-r--r--   0        0        0      619 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/境港市.json
--rw-r--r--   0        0        0      613 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/岩美郡岩美町.json
--rw-r--r--   0        0        0      319 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/日野郡日南町.json
--rw-r--r--   0        0        0      253 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/日野郡日野町.json
--rw-r--r--   0        0        0      286 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/日野郡江府町.json
--rw-r--r--   0        0        0      721 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/東伯郡三朝町.json
--rw-r--r--   0        0        0      262 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/東伯郡北栄町.json
--rw-r--r--   0        0        0      727 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/東伯郡湯梨浜町.json
--rw-r--r--   0        0        0      856 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/東伯郡琴浦町.json
--rw-r--r--   0        0        0     3937 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/米子市.json
--rw-r--r--   0        0        0      520 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/西伯郡伯耆町.json
--rw-r--r--   0        0        0      466 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/西伯郡南部町.json
--rw-r--r--   0        0        0      622 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/西伯郡大山町.json
--rw-r--r--   0        0        0       49 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/西伯郡日吉津村.json
--rw-r--r--   0        0        0     9094 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/鳥取市.json
--rw-r--r--   0        0        0      763 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/いちき串木野市.json
--rw-r--r--   0        0        0      571 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/伊佐市.json
--rw-r--r--   0        0        0      583 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/出水市.json
--rw-r--r--   0        0        0      118 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/出水郡長島町.json
--rw-r--r--   0        0        0      790 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/南さつま市.json
--rw-r--r--   0        0        0      559 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/南九州市.json
--rw-r--r--   0        0        0      289 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/垂水市.json
--rw-r--r--   0        0        0       91 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/大島郡与論町.json
--rw-r--r--   0        0        0      271 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/大島郡伊仙町.json
--rw-r--r--   0        0        0      307 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/大島郡和泊町.json
--rw-r--r--   0        0        0      490 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/大島郡喜界町.json
--rw-r--r--   0        0        0      181 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/大島郡大和村.json
--rw-r--r--   0        0        0      181 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/大島郡天城町.json
--rw-r--r--   0        0        0      196 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/大島郡宇検村.json
--rw-r--r--   0        0        0      154 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/大島郡徳之島町.json
--rw-r--r--   0        0        0      817 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/大島郡瀬戸内町.json
--rw-r--r--   0        0        0      322 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/大島郡知名町.json
--rw-r--r--   0        0        0      133 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/大島郡龍郷町.json
--rw-r--r--   0        0        0     1717 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/奄美市.json
--rw-r--r--   0        0        0      850 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/姶良市.json
--rw-r--r--   0        0        0      121 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/姶良郡湧水町.json
--rw-r--r--   0        0        0      403 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/志布志市.json
--rw-r--r--   0        0        0      673 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/指宿市.json
--rw-r--r--   0        0        0     1066 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/日置市.json
--rw-r--r--   0        0        0      742 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/曽於市.json
--rw-r--r--   0        0        0       94 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/曽於郡大崎町.json
--rw-r--r--   0        0        0     1069 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/枕崎市.json
--rw-r--r--   0        0        0       64 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/熊毛郡中種子町.json
--rw-r--r--   0        0        0       61 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/熊毛郡南種子町.json
--rw-r--r--   0        0        0      181 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/熊毛郡屋久島町.json
--rw-r--r--   0        0        0      139 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/肝属郡南大隅町.json
--rw-r--r--   0        0        0       52 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/肝属郡東串良町.json
--rw-r--r--   0        0        0       91 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/肝属郡肝付町.json
--rw-r--r--   0        0        0       55 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/肝属郡錦江町.json
--rw-r--r--   0        0        0     1444 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/薩摩川内市.json
--rw-r--r--   0        0        0      250 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/薩摩郡さつま町.json
--rw-r--r--   0        0        0      160 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/西之表市.json
--rw-r--r--   0        0        0      289 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/阿久根市.json
--rw-r--r--   0        0        0     2206 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/霧島市.json
--rw-r--r--   0        0        0     6250 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/鹿児島市.json
--rw-r--r--   0        0        0       49 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/鹿児島郡三島村.json
--rw-r--r--   0        0        0      145 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/鹿児島郡十島村.json
--rw-r--r--   0        0        0     1273 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/鹿屋市.json
--rw-r--r--   0        0        0    35201 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja.json
--rw-r--r--   0        0        0       46 2021-06-11 00:32:50.564787 normalize_japanese_address-0.0.8/normalize_japanese_address/lib/__init__.py
--rw-r--r--   0        0        0      205 2021-06-11 01:39:17.518711 normalize_japanese_address-0.0.8/normalize_japanese_address/lib/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     6532 2021-06-16 04:51:40.408733 normalize_japanese_address-0.0.8/normalize_japanese_address/lib/__pycache__/cacheRegexes.cpython-38.pyc
--rw-r--r--   0        0        0      788 2021-06-11 05:08:20.011650 normalize_japanese_address-0.0.8/normalize_japanese_address/lib/__pycache__/config.cpython-38.pyc
--rw-r--r--   0        0        0      609 2021-06-11 01:39:17.522711 normalize_japanese_address-0.0.8/normalize_japanese_address/lib/__pycache__/const.cpython-38.pyc
--rw-r--r--   0        0        0     7875 2021-06-16 03:52:25.112193 normalize_japanese_address-0.0.8/normalize_japanese_address/lib/__pycache__/dict.cpython-38.pyc
--rw-r--r--   0        0        0     1794 2021-06-16 04:50:05.258642 normalize_japanese_address-0.0.8/normalize_japanese_address/lib/__pycache__/kan2num.cpython-38.pyc
--rw-r--r--   0        0        0     1210 2021-06-12 02:48:10.863546 normalize_japanese_address-0.0.8/normalize_japanese_address/lib/__pycache__/num2kan.cpython-38.pyc
--rw-r--r--   0        0        0     1102 2021-06-16 04:59:14.523629 normalize_japanese_address-0.0.8/normalize_japanese_address/lib/__pycache__/patch_addr.cpython-38.pyc
--rw-r--r--   0        0        0      406 2021-06-11 01:45:54.779367 normalize_japanese_address-0.0.8/normalize_japanese_address/lib/__pycache__/zen2han.cpython-38.pyc
--rw-r--r--   0        0        0     6778 2021-06-23 03:43:25.249938 normalize_japanese_address-0.0.8/normalize_japanese_address/lib/cacheRegexes.py
--rw-r--r--   0        0        0      517 2021-06-23 03:49:28.414742 normalize_japanese_address-0.0.8/normalize_japanese_address/lib/config.py
--rw-r--r--   0        0        0      714 2021-06-17 03:50:15.441336 normalize_japanese_address-0.0.8/normalize_japanese_address/lib/const.py
--rw-r--r--   0        0        0     7047 2021-06-23 04:16:01.751262 normalize_japanese_address-0.0.8/normalize_japanese_address/lib/dict.py
--rw-r--r--   0        0        0     1043 2021-06-17 21:40:29.105979 normalize_japanese_address-0.0.8/normalize_japanese_address/lib/kan2num.py
--rw-r--r--   0        0        0      918 2021-06-11 05:08:19.331664 normalize_japanese_address-0.0.8/normalize_japanese_address/lib/num2kan.py
--rw-r--r--   0        0        0     1167 2021-06-17 03:53:16.329845 normalize_japanese_address-0.0.8/normalize_japanese_address/lib/patch_addr.py
--rw-r--r--   0        0        0      162 2021-05-25 10:18:26.072101 normalize_japanese_address-0.0.8/normalize_japanese_address/lib/zen2han.py
--rw-r--r--   0        0        0     4958 2021-06-21 00:33:02.507347 normalize_japanese_address-0.0.8/normalize_japanese_address/normalize.py
--rw-r--r--   0        0        0       37 2021-06-17 21:37:28.613563 normalize_japanese_address-0.0.8/normalize_japanese_address/tests/.pytest_cache/.gitignore
--rw-r--r--   0        0        0      194 2021-06-17 21:37:28.613563 normalize_japanese_address-0.0.8/normalize_japanese_address/tests/.pytest_cache/CACHEDIR.TAG
--rw-r--r--   0        0        0      295 2021-06-17 21:37:28.613563 normalize_japanese_address-0.0.8/normalize_japanese_address/tests/.pytest_cache/README.md
--rw-r--r--   0        0        0        2 2021-06-23 02:01:05.855628 normalize_japanese_address-0.0.8/normalize_japanese_address/tests/.pytest_cache/v/cache/lastfailed
--rw-r--r--   0        0        0       75 2021-06-23 04:15:41.191668 normalize_japanese_address-0.0.8/normalize_japanese_address/tests/.pytest_cache/v/cache/nodeids
--rw-r--r--   0        0        0        2 2021-06-23 04:15:41.191668 normalize_japanese_address-0.0.8/normalize_japanese_address/tests/.pytest_cache/v/cache/stepwise
--rw-r--r--   0        0        0       46 2021-06-16 22:52:08.527449 normalize_japanese_address-0.0.8/normalize_japanese_address/tests/__init__.py
--rw-r--r--   0        0        0    25144 2021-06-23 04:04:05.493407 normalize_japanese_address-0.0.8/normalize_japanese_address/tests/test_normalize_japanese_address.py
--rw-r--r--   0        0        0      624 2021-06-23 04:17:39.885325 normalize_japanese_address-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     6071 2021-06-23 04:17:47.800356 normalize_japanese_address-0.0.8/setup.py
--rw-r--r--   0        0        0     2432 2021-06-23 04:17:47.800654 normalize_japanese_address-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1451 2021-06-17 21:50:23.138179 normalize_japanese_address-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0     1595 2021-06-18 01:21:31.327527 normalize_japanese_address-0.0.9/README.md
+-rw-r--r--   0        0        0       80 2021-06-20 22:56:01.989645 normalize_japanese_address-0.0.9/normalize_japanese_address/__init__.py
+-rw-r--r--   0        0        0     1903 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/いなべ市.json
+-rw-r--r--   0        0        0      184 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/三重郡川越町.json
+-rw-r--r--   0        0        0      229 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/三重郡朝日町.json
+-rw-r--r--   0        0        0      532 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/三重郡菰野町.json
+-rw-r--r--   0        0        0     1480 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/亀山市.json
+-rw-r--r--   0        0        0     2293 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/伊勢市.json
+-rw-r--r--   0        0        0     3199 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/伊賀市.json
+-rw-r--r--   0        0        0      217 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/北牟婁郡紀北町.json
+-rw-r--r--   0        0        0      220 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/南牟婁郡御浜町.json
+-rw-r--r--   0        0        0      136 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/南牟婁郡紀宝町.json
+-rw-r--r--   0        0        0     3562 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/名張市.json
+-rw-r--r--   0        0        0      427 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/員弁郡東員町.json
+-rw-r--r--   0        0        0     7435 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/四日市市.json
+-rw-r--r--   0        0        0      433 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/多気郡多気町.json
+-rw-r--r--   0        0        0      397 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/多気郡大台町.json
+-rw-r--r--   0        0        0      514 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/多気郡明和町.json
+-rw-r--r--   0        0        0      781 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/尾鷲市.json
+-rw-r--r--   0        0        0      397 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/度会郡南伊勢町.json
+-rw-r--r--   0        0        0      127 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/度会郡大紀町.json
+-rw-r--r--   0        0        0      322 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/度会郡度会町.json
+-rw-r--r--   0        0        0      295 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/度会郡玉城町.json
+-rw-r--r--   0        0        0      709 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/志摩市.json
+-rw-r--r--   0        0        0     4072 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/松阪市.json
+-rw-r--r--   0        0        0     5695 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/桑名市.json
+-rw-r--r--   0        0        0      379 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/桑名郡木曽岬町.json
+-rw-r--r--   0        0        0     5707 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/津市.json
+-rw-r--r--   0        0        0      895 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/熊野市.json
+-rw-r--r--   0        0        0     5635 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/鈴鹿市.json
+-rw-r--r--   0        0        0      433 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/鳥羽市.json
+-rw-r--r--   0        0        0      250 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/与謝郡与謝野町.json
+-rw-r--r--   0        0        0      250 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/与謝郡伊根町.json
+-rw-r--r--   0        0        0      229 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/久世郡久御山町.json
+-rw-r--r--   0        0        0       46 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/乙訓郡大山崎町.json
+-rw-r--r--   0        0        0     4123 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/亀岡市.json
+-rw-r--r--   0        0        0     3340 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京丹後市.json
+-rw-r--r--   0        0        0    10582 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京田辺市.json
+-rw-r--r--   0        0        0     8398 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京都市上京区.json
+-rw-r--r--   0        0        0     7804 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京都市下京区.json
+-rw-r--r--   0        0        0     7909 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京都市中京区.json
+-rw-r--r--   0        0        0    13579 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京都市伏見区.json
+-rw-r--r--   0        0        0     8887 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京都市北区.json
+-rw-r--r--   0        0        0     6256 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京都市南区.json
+-rw-r--r--   0        0        0    12802 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京都市右京区.json
+-rw-r--r--   0        0        0     6034 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京都市山科区.json
+-rw-r--r--   0        0        0    12220 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京都市左京区.json
+-rw-r--r--   0        0        0     4111 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京都市東山区.json
+-rw-r--r--   0        0        0     6592 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京都市西京区.json
+-rw-r--r--   0        0        0     6052 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/八幡市.json
+-rw-r--r--   0        0        0     2386 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/南丹市.json
+-rw-r--r--   0        0        0       82 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/向日市.json
+-rw-r--r--   0        0        0      115 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/城陽市.json
+-rw-r--r--   0        0        0      976 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/宇治市.json
+-rw-r--r--   0        0        0     1111 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/宮津市.json
+-rw-r--r--   0        0        0     2449 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/木津川市.json
+-rw-r--r--   0        0        0      106 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/相楽郡南山城村.json
+-rw-r--r--   0        0        0      202 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/相楽郡和束町.json
+-rw-r--r--   0        0        0       64 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/相楽郡笠置町.json
+-rw-r--r--   0        0        0      634 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/相楽郡精華町.json
+-rw-r--r--   0        0        0     3853 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/福知山市.json
+-rw-r--r--   0        0        0       52 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/綴喜郡井手町.json
+-rw-r--r--   0        0        0      184 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/綴喜郡宇治田原町.json
+-rw-r--r--   0        0        0     1726 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/綾部市.json
+-rw-r--r--   0        0        0     2494 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/舞鶴市.json
+-rw-r--r--   0        0        0      673 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/船井郡京丹波町.json
+-rw-r--r--   0        0        0     1315 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/長岡京市.json
+-rw-r--r--   0        0        0      190 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/三養基郡みやき町.json
+-rw-r--r--   0        0        0       61 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/三養基郡上峰町.json
+-rw-r--r--   0        0        0      157 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/三養基郡基山町.json
+-rw-r--r--   0        0        0     1768 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/伊万里市.json
+-rw-r--r--   0        0        0     5440 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/佐賀市.json
+-rw-r--r--   0        0        0     3898 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/唐津市.json
+-rw-r--r--   0        0        0      271 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/多久市.json
+-rw-r--r--   0        0        0      283 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/嬉野市.json
+-rw-r--r--   0        0        0      589 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/小城市.json
+-rw-r--r--   0        0        0      349 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/東松浦郡玄海町.json
+-rw-r--r--   0        0        0       31 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/杵島郡大町町.json
+-rw-r--r--   0        0        0      103 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/杵島郡江北町.json
+-rw-r--r--   0        0        0      370 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/杵島郡白石町.json
+-rw-r--r--   0        0        0      682 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/武雄市.json
+-rw-r--r--   0        0        0      634 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/神埼市.json
+-rw-r--r--   0        0        0       82 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/神埼郡吉野ヶ里町.json
+-rw-r--r--   0        0        0      157 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/藤津郡太良町.json
+-rw-r--r--   0        0        0      850 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/西松浦郡有田町.json
+-rw-r--r--   0        0        0     1420 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/鳥栖市.json
+-rw-r--r--   0        0        0      193 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/鹿島市.json
+-rw-r--r--   0        0        0     3130 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/たつの市.json
+-rw-r--r--   0        0        0     3877 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/三木市.json
+-rw-r--r--   0        0        0     2659 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/三田市.json
+-rw-r--r--   0        0        0     3346 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/丹波市.json
+-rw-r--r--   0        0        0     2677 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/丹波篠山市.json
+-rw-r--r--   0        0        0     7588 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/伊丹市.json
+-rw-r--r--   0        0        0      973 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/佐用郡佐用町.json
+-rw-r--r--   0        0        0     3814 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/加古川市.json
+-rw-r--r--   0        0        0     1234 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/加古郡播磨町.json
+-rw-r--r--   0        0        0      376 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/加古郡稲美町.json
+-rw-r--r--   0        0        0      931 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/加東市.json
+-rw-r--r--   0        0        0     1540 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/加西市.json
+-rw-r--r--   0        0        0     1885 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/南あわじ市.json
+-rw-r--r--   0        0        0     1108 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/多可郡多可町.json
+-rw-r--r--   0        0        0    17533 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/姫路市.json
+-rw-r--r--   0        0        0     2314 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/宍粟市.json
+-rw-r--r--   0        0        0     5437 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/宝塚市.json
+-rw-r--r--   0        0        0      835 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/小野市.json
+-rw-r--r--   0        0        0     8926 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/尼崎市.json
+-rw-r--r--   0        0        0     3334 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/川西市.json
+-rw-r--r--   0        0        0      835 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/川辺郡猪名川町.json
+-rw-r--r--   0        0        0      316 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/揖保郡太子町.json
+-rw-r--r--   0        0        0     4303 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/明石市.json
+-rw-r--r--   0        0        0     2101 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/朝来市.json
+-rw-r--r--   0        0        0     1921 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/洲本市.json
+-rw-r--r--   0        0        0      901 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/淡路市.json
+-rw-r--r--   0        0        0     1480 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/相生市.json
+-rw-r--r--   0        0        0      253 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/神崎郡市川町.json
+-rw-r--r--   0        0        0      316 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/神崎郡神河町.json
+-rw-r--r--   0        0        0      133 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/神崎郡福崎町.json
+-rw-r--r--   0        0        0     7612 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市中央区.json
+-rw-r--r--   0        0        0     6304 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市兵庫区.json
+-rw-r--r--   0        0        0     6586 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市北区.json
+-rw-r--r--   0        0        0     5734 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市垂水区.json
+-rw-r--r--   0        0        0     4690 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市東灘区.json
+-rw-r--r--   0        0        0     7615 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市灘区.json
+-rw-r--r--   0        0        0     6052 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市西区.json
+-rw-r--r--   0        0        0     8557 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市長田区.json
+-rw-r--r--   0        0        0     6907 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市須磨区.json
+-rw-r--r--   0        0        0      505 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/美方郡新温泉町.json
+-rw-r--r--   0        0        0     1807 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/美方郡香美町.json
+-rw-r--r--   0        0        0      754 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/芦屋市.json
+-rw-r--r--   0        0        0     7846 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/西宮市.json
+-rw-r--r--   0        0        0      874 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/西脇市.json
+-rw-r--r--   0        0        0     4810 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/豊岡市.json
+-rw-r--r--   0        0        0      949 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/赤穂市.json
+-rw-r--r--   0        0        0      616 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/赤穂郡上郡町.json
+-rw-r--r--   0        0        0     1360 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/養父市.json
+-rw-r--r--   0        0        0     2971 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/高砂市.json
+-rw-r--r--   0        0        0     1396 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/三笠市.json
+-rw-r--r--   0        0        0      283 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡上川町.json
+-rw-r--r--   0        0        0      151 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡下川町.json
+-rw-r--r--   0        0        0      115 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡剣淵町.json
+-rw-r--r--   0        0        0      244 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡和寒町.json
+-rw-r--r--   0        0        0      904 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡当麻町.json
+-rw-r--r--   0        0        0      169 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡愛別町.json
+-rw-r--r--   0        0        0     4090 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡新得町.json
+-rw-r--r--   0        0        0     1351 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡東川町.json
+-rw-r--r--   0        0        0     2533 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡東神楽町.json
+-rw-r--r--   0        0        0      739 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡比布町.json
+-rw-r--r--   0        0        0     7729 2021-06-17 01:45:25.825508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡清水町.json
+-rw-r--r--   0        0        0     1582 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡美瑛町.json
+-rw-r--r--   0        0        0     1069 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡鷹栖町.json
+-rw-r--r--   0        0        0      241 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/上磯郡木古内町.json
+-rw-r--r--   0        0        0      106 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/上磯郡知内町.json
+-rw-r--r--   0        0        0      166 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/中川郡中川町.json
+-rw-r--r--   0        0        0      973 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/中川郡幕別町.json
+-rw-r--r--   0        0        0      469 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/中川郡本別町.json
+-rw-r--r--   0        0        0     1258 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/中川郡池田町.json
+-rw-r--r--   0        0        0     2989 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/中川郡美深町.json
+-rw-r--r--   0        0        0      421 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/中川郡豊頃町.json
+-rw-r--r--   0        0        0       67 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/中川郡音威子府村.json
+-rw-r--r--   0        0        0      760 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/久遠郡せたな町.json
+-rw-r--r--   0        0        0      958 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/亀田郡七飯町.json
+-rw-r--r--   0        0        0      670 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/二海郡八雲町.json
+-rw-r--r--   0        0        0      823 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/伊達市.json
+-rw-r--r--   0        0        0     1156 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/余市郡仁木町.json
+-rw-r--r--   0        0        0     1483 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/余市郡余市町.json
+-rw-r--r--   0        0        0      145 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/余市郡赤井川村.json
+-rw-r--r--   0        0        0     2935 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/函館市.json
+-rw-r--r--   0        0        0       19 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/利尻郡利尻富士町.json
+-rw-r--r--   0        0        0       22 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/利尻郡利尻町.json
+-rw-r--r--   0        0        0      760 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/勇払郡むかわ町.json
+-rw-r--r--   0        0        0      136 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/勇払郡占冠村.json
+-rw-r--r--   0        0        0      352 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/勇払郡厚真町.json
+-rw-r--r--   0        0        0      775 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/勇払郡安平町.json
+-rw-r--r--   0        0        0     4669 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/北広島市.json
+-rw-r--r--   0        0        0     1825 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/北斗市.json
+-rw-r--r--   0        0        0     8485 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/北見市.json
+-rw-r--r--   0        0        0     2011 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/十勝郡浦幌町.json
+-rw-r--r--   0        0        0     5374 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/千歳市.json
+-rw-r--r--   0        0        0     1528 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/厚岸郡厚岸町.json
+-rw-r--r--   0        0        0     3028 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/厚岸郡浜中町.json
+-rw-r--r--   0        0        0       88 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/古宇郡泊村.json
+-rw-r--r--   0        0        0       58 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/古宇郡神恵内村.json
+-rw-r--r--   0        0        0      187 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/古平郡古平町.json
+-rw-r--r--   0        0        0     9880 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/名寄市.json
+-rw-r--r--   0        0        0     1228 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/増毛郡増毛町.json
+-rw-r--r--   0        0        0     9493 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/士別市.json
+-rw-r--r--   0        0        0     1141 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/夕張市.json
+-rw-r--r--   0        0        0      586 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/夕張郡栗山町.json
+-rw-r--r--   0        0        0      253 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/夕張郡由仁町.json
+-rw-r--r--   0        0        0     1549 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/夕張郡長沼町.json
+-rw-r--r--   0        0        0     1630 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/天塩郡天塩町.json
+-rw-r--r--   0        0        0      550 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/天塩郡幌延町.json
+-rw-r--r--   0        0        0     2857 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/天塩郡豊富町.json
+-rw-r--r--   0        0        0      319 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/天塩郡遠別町.json
+-rw-r--r--   0        0        0      121 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/奥尻郡奥尻町.json
+-rw-r--r--   0        0        0      199 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/宗谷郡猿払村.json
+-rw-r--r--   0        0        0     2641 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/室蘭市.json
+-rw-r--r--   0        0        0     1930 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/富良野市.json
+-rw-r--r--   0        0        0      166 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/寿都郡寿都町.json
+-rw-r--r--   0        0        0      316 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/寿都郡黒松内町.json
+-rw-r--r--   0        0        0     2476 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/小樽市.json
+-rw-r--r--   0        0        0      250 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/山越郡長万部町.json
+-rw-r--r--   0        0        0      106 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/岩内郡共和町.json
+-rw-r--r--   0        0        0      145 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/岩内郡岩内町.json
+-rw-r--r--   0        0        0    19627 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/岩見沢市.json
+-rw-r--r--   0        0        0      283 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/島牧郡島牧村.json
+-rw-r--r--   0        0        0     1273 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/川上郡弟子屈町.json
+-rw-r--r--   0        0        0     2404 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/川上郡標茶町.json
+-rw-r--r--   0        0        0    41464 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/帯広市.json
+-rw-r--r--   0        0        0      295 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/常呂郡佐呂間町.json
+-rw-r--r--   0        0        0      181 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/常呂郡置戸町.json
+-rw-r--r--   0        0        0      331 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/常呂郡訓子府町.json
+-rw-r--r--   0        0        0      127 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/幌泉郡えりも町.json
+-rw-r--r--   0        0        0      637 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/広尾郡大樹町.json
+-rw-r--r--   0        0        0     4075 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/広尾郡広尾町.json
+-rw-r--r--   0        0        0     3154 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/恵庭市.json
+-rw-r--r--   0        0        0      238 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/斜里郡小清水町.json
+-rw-r--r--   0        0        0      457 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/斜里郡斜里町.json
+-rw-r--r--   0        0        0      133 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/斜里郡清里町.json
+-rw-r--r--   0        0        0      319 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/新冠郡新冠町.json
+-rw-r--r--   0        0        0     2110 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/日高郡新ひだか町.json
+-rw-r--r--   0        0        0    57085 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/旭川市.json
+-rw-r--r--   0        0        0      241 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/有珠郡壮瞥町.json
+-rw-r--r--   0        0        0    26872 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市中央区.json
+-rw-r--r--   0        0        0    28633 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市北区.json
+-rw-r--r--   0        0        0     9436 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市南区.json
+-rw-r--r--   0        0        0     5422 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市厚別区.json
+-rw-r--r--   0        0        0     9232 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市手稲区.json
+-rw-r--r--   0        0        0    32248 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市東区.json
+-rw-r--r--   0        0        0     5356 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市清田区.json
+-rw-r--r--   0        0        0    11434 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市白石区.json
+-rw-r--r--   0        0        0    14980 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市西区.json
+-rw-r--r--   0        0        0    13618 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市豊平区.json
+-rw-r--r--   0        0        0      409 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/松前郡松前町.json
+-rw-r--r--   0        0        0      217 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/松前郡福島町.json
+-rw-r--r--   0        0        0      214 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/枝幸郡中頓別町.json
+-rw-r--r--   0        0        0      535 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/枝幸郡枝幸町.json
+-rw-r--r--   0        0        0     1843 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/枝幸郡浜頓別町.json
+-rw-r--r--   0        0        0     3319 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/根室市.json
+-rw-r--r--   0        0        0      310 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/様似郡様似町.json
+-rw-r--r--   0        0        0    22342 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/標津郡中標津町.json
+-rw-r--r--   0        0        0     2125 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/標津郡標津町.json
+-rw-r--r--   0        0        0      136 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/樺戸郡新十津川町.json
+-rw-r--r--   0        0        0      229 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/樺戸郡月形町.json
+-rw-r--r--   0        0        0      106 2021-06-17 01:45:25.829508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/樺戸郡浦臼町.json
+-rw-r--r--   0        0        0      337 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/檜山郡上ノ国町.json
+-rw-r--r--   0        0        0      328 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/檜山郡厚沢部町.json
+-rw-r--r--   0        0        0      538 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/檜山郡江差町.json
+-rw-r--r--   0        0        0      109 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/歌志内市.json
+-rw-r--r--   0        0        0     2014 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/江別市.json
+-rw-r--r--   0        0        0      223 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/沙流郡平取町.json
+-rw-r--r--   0        0        0     1408 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/沙流郡日高町.json
+-rw-r--r--   0        0        0     1153 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/河東郡上士幌町.json
+-rw-r--r--   0        0        0     2647 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/河東郡士幌町.json
+-rw-r--r--   0        0        0    11446 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/河東郡音更町.json
+-rw-r--r--   0        0        0     2857 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/河東郡鹿追町.json
+-rw-r--r--   0        0        0     3715 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/河西郡中札内村.json
+-rw-r--r--   0        0        0       64 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/河西郡更別村.json
+-rw-r--r--   0        0        0    10342 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/河西郡芽室町.json
+-rw-r--r--   0        0        0     1255 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/浦河郡浦河町.json
+-rw-r--r--   0        0        0      766 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/深川市.json
+-rw-r--r--   0        0        0     3307 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/滝川市.json
+-rw-r--r--   0        0        0      256 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/瀬棚郡今金町.json
+-rw-r--r--   0        0        0      184 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/爾志郡乙部町.json
+-rw-r--r--   0        0        0     2350 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/留萌市.json
+-rw-r--r--   0        0        0      364 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/留萌郡小平町.json
+-rw-r--r--   0        0        0     2635 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/登別市.json
+-rw-r--r--   0        0        0     5524 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/白糠郡白糠町.json
+-rw-r--r--   0        0        0      925 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/白老郡白老町.json
+-rw-r--r--   0        0        0      295 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/目梨郡羅臼町.json
+-rw-r--r--   0        0        0     4972 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/石狩市.json
+-rw-r--r--   0        0        0      511 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/石狩郡当別町.json
+-rw-r--r--   0        0        0      556 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/石狩郡新篠津村.json
+-rw-r--r--   0        0        0    12733 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/砂川市.json
+-rw-r--r--   0        0        0      382 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/磯谷郡蘭越町.json
+-rw-r--r--   0        0        0       37 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/礼文郡礼文町.json
+-rw-r--r--   0        0        0     1996 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/稚内市.json
+-rw-r--r--   0        0        0      202 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/積丹郡積丹町.json
+-rw-r--r--   0        0        0     8965 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/空知郡上富良野町.json
+-rw-r--r--   0        0        0       85 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/空知郡上砂川町.json
+-rw-r--r--   0        0        0      766 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/空知郡中富良野町.json
+-rw-r--r--   0        0        0       82 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/空知郡南富良野町.json
+-rw-r--r--   0        0        0     1036 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/空知郡南幌町.json
+-rw-r--r--   0        0        0      238 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/空知郡奈井江町.json
+-rw-r--r--   0        0        0     2755 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/紋別市.json
+-rw-r--r--   0        0        0      427 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/紋別郡湧別町.json
+-rw-r--r--   0        0        0     1042 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/紋別郡滝上町.json
+-rw-r--r--   0        0        0      121 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/紋別郡興部町.json
+-rw-r--r--   0        0        0      145 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/紋別郡西興部村.json
+-rw-r--r--   0        0        0     2362 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/紋別郡遠軽町.json
+-rw-r--r--   0        0        0      172 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/紋別郡雄武町.json
+-rw-r--r--   0        0        0     6358 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/網走市.json
+-rw-r--r--   0        0        0     2323 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/網走郡大空町.json
+-rw-r--r--   0        0        0      427 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/網走郡津別町.json
+-rw-r--r--   0        0        0     2437 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/網走郡美幌町.json
+-rw-r--r--   0        0        0     7795 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/美唄市.json
+-rw-r--r--   0        0        0     1372 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/芦別市.json
+-rw-r--r--   0        0        0      100 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/苫前郡初山別村.json
+-rw-r--r--   0        0        0     2017 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/苫前郡羽幌町.json
+-rw-r--r--   0        0        0      217 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/苫前郡苫前町.json
+-rw-r--r--   0        0        0     6766 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/苫小牧市.json
+-rw-r--r--   0        0        0      874 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/茅部郡森町.json
+-rw-r--r--   0        0        0       61 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/茅部郡鹿部町.json
+-rw-r--r--   0        0        0      247 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/虻田郡ニセコ町.json
+-rw-r--r--   0        0        0      154 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/虻田郡京極町.json
+-rw-r--r--   0        0        0     3646 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/虻田郡倶知安町.json
+-rw-r--r--   0        0        0      241 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/虻田郡喜茂別町.json
+-rw-r--r--   0        0        0      244 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/虻田郡洞爺湖町.json
+-rw-r--r--   0        0        0      127 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/虻田郡留寿都村.json
+-rw-r--r--   0        0        0      184 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/虻田郡真狩村.json
+-rw-r--r--   0        0        0      229 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/虻田郡豊浦町.json
+-rw-r--r--   0        0        0     4417 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/赤平市.json
+-rw-r--r--   0        0        0     1843 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/足寄郡足寄町.json
+-rw-r--r--   0        0        0     1147 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/足寄郡陸別町.json
+-rw-r--r--   0        0        0      847 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/野付郡別海町.json
+-rw-r--r--   0        0        0    16138 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/釧路市.json
+-rw-r--r--   0        0        0     4552 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/釧路郡釧路町.json
+-rw-r--r--   0        0        0     1060 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/阿寒郡鶴居村.json
+-rw-r--r--   0        0        0      112 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/雨竜郡北竜町.json
+-rw-r--r--   0        0        0      127 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/雨竜郡妹背牛町.json
+-rw-r--r--   0        0        0      361 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/雨竜郡幌加内町.json
+-rw-r--r--   0        0        0      577 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/雨竜郡沼田町.json
+-rw-r--r--   0        0        0      184 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/雨竜郡秩父別町.json
+-rw-r--r--   0        0        0      415 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/雨竜郡雨竜町.json
+-rw-r--r--   0        0        0      757 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/いすみ市.json
+-rw-r--r--   0        0        0     3166 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/佐倉市.json
+-rw-r--r--   0        0        0     2413 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/八千代市.json
+-rw-r--r--   0        0        0      415 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/八街市.json
+-rw-r--r--   0        0        0      514 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/勝浦市.json
+-rw-r--r--   0        0        0      727 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/匝瑳市.json
+-rw-r--r--   0        0        0     2176 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/千葉市中央区.json
+-rw-r--r--   0        0        0     1156 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/千葉市稲毛区.json
+-rw-r--r--   0        0        0     1462 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/千葉市緑区.json
+-rw-r--r--   0        0        0      964 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/千葉市美浜区.json
+-rw-r--r--   0        0        0     1585 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/千葉市花見川区.json
+-rw-r--r--   0        0        0     1930 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/千葉市若葉区.json
+-rw-r--r--   0        0        0     1561 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/南房総市.json
+-rw-r--r--   0        0        0      814 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/印旛郡栄町.json
+-rw-r--r--   0        0        0      556 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/印旛郡酒々井町.json
+-rw-r--r--   0        0        0     3130 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/印西市.json
+-rw-r--r--   0        0        0     2968 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/君津市.json
+-rw-r--r--   0        0        0     1183 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/四街道市.json
+-rw-r--r--   0        0        0      829 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/大網白里市.json
+-rw-r--r--   0        0        0      601 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/夷隅郡大多喜町.json
+-rw-r--r--   0        0        0      139 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/夷隅郡御宿町.json
+-rw-r--r--   0        0        0      184 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/安房郡鋸南町.json
+-rw-r--r--   0        0        0      886 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/富津市.json
+-rw-r--r--   0        0        0      277 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/富里市.json
+-rw-r--r--   0        0        0     1183 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/山武市.json
+-rw-r--r--   0        0        0      163 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/山武郡九十九里町.json
+-rw-r--r--   0        0        0      526 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/山武郡横芝光町.json
+-rw-r--r--   0        0        0      235 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/山武郡芝山町.json
+-rw-r--r--   0        0        0     6463 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/市原市.json
+-rw-r--r--   0        0        0     4318 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/市川市.json
+-rw-r--r--   0        0        0     2677 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/成田市.json
+-rw-r--r--   0        0        0     2257 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/我孫子市.json
+-rw-r--r--   0        0        0      634 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/旭市.json
+-rw-r--r--   0        0        0     4060 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/木更津市.json
+-rw-r--r--   0        0        0     1153 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/東金市.json
+-rw-r--r--   0        0        0     4636 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/松戸市.json
+-rw-r--r--   0        0        0     5671 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/柏市.json
+-rw-r--r--   0        0        0     2725 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/流山市.json
+-rw-r--r--   0        0        0     1531 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/浦安市.json
+-rw-r--r--   0        0        0      814 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/白井市.json
+-rw-r--r--   0        0        0     1846 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/習志野市.json
+-rw-r--r--   0        0        0     6322 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/船橋市.json
+-rw-r--r--   0        0        0     1330 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/茂原市.json
+-rw-r--r--   0        0        0     1042 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/袖ヶ浦市.json
+-rw-r--r--   0        0        0     1468 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/野田市.json
+-rw-r--r--   0        0        0     2743 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/銚子市.json
+-rw-r--r--   0        0        0     1777 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/鎌ヶ谷市.json
+-rw-r--r--   0        0        0       97 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/長生郡一宮町.json
+-rw-r--r--   0        0        0      130 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/長生郡白子町.json
+-rw-r--r--   0        0        0      184 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/長生郡睦沢町.json
+-rw-r--r--   0        0        0      328 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/長生郡長南町.json
+-rw-r--r--   0        0        0      262 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/長生郡長柄町.json
+-rw-r--r--   0        0        0      277 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/長生郡長生村.json
+-rw-r--r--   0        0        0      709 2021-06-17 01:45:25.833508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/館山市.json
+-rw-r--r--   0        0        0     1585 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/香取市.json
+-rw-r--r--   0        0        0      439 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/香取郡多古町.json
+-rw-r--r--   0        0        0      253 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/香取郡東庄町.json
+-rw-r--r--   0        0        0      181 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/香取郡神崎町.json
+-rw-r--r--   0        0        0      781 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/鴨川市.json
+-rw-r--r--   0        0        0      781 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/伊都郡かつらぎ町.json
+-rw-r--r--   0        0        0      214 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/伊都郡九度山町.json
+-rw-r--r--   0        0        0      307 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/伊都郡高野町.json
+-rw-r--r--   0        0        0    11203 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/和歌山市.json
+-rw-r--r--   0        0        0      436 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/岩出市.json
+-rw-r--r--   0        0        0      349 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/御坊市.json
+-rw-r--r--   0        0        0     1981 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/新宮市.json
+-rw-r--r--   0        0        0      256 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/日高郡みなべ町.json
+-rw-r--r--   0        0        0      406 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/日高郡印南町.json
+-rw-r--r--   0        0        0      772 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/日高郡日高川町.json
+-rw-r--r--   0        0        0      229 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/日高郡日高町.json
+-rw-r--r--   0        0        0      211 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/日高郡由良町.json
+-rw-r--r--   0        0        0       79 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/日高郡美浜町.json
+-rw-r--r--   0        0        0      298 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/有田市.json
+-rw-r--r--   0        0        0      247 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/有田郡広川町.json
+-rw-r--r--   0        0        0     1435 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/有田郡有田川町.json
+-rw-r--r--   0        0        0      103 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/有田郡湯浅町.json
+-rw-r--r--   0        0        0      310 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/東牟婁郡串本町.json
+-rw-r--r--   0        0        0       79 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/東牟婁郡北山村.json
+-rw-r--r--   0        0        0      403 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/東牟婁郡古座川町.json
+-rw-r--r--   0        0        0       31 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/東牟婁郡太地町.json
+-rw-r--r--   0        0        0     1012 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/東牟婁郡那智勝浦町.json
+-rw-r--r--   0        0        0     1828 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/橋本市.json
+-rw-r--r--   0        0        0     1087 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/海南市.json
+-rw-r--r--   0        0        0      556 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/海草郡紀美野町.json
+-rw-r--r--   0        0        0     2551 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/田辺市.json
+-rw-r--r--   0        0        0     1528 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/紀の川市.json
+-rw-r--r--   0        0        0      307 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/西牟婁郡すさみ町.json
+-rw-r--r--   0        0        0       82 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/西牟婁郡上富田町.json
+-rw-r--r--   0        0        0      352 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/西牟婁郡白浜町.json
+-rw-r--r--   0        0        0     1372 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市中央区.json
+-rw-r--r--   0        0        0      505 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市北区.json
+-rw-r--r--   0        0        0     1465 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市南区.json
+-rw-r--r--   0        0        0     1066 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市大宮区.json
+-rw-r--r--   0        0        0     2185 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市岩槻区.json
+-rw-r--r--   0        0        0     1234 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市桜区.json
+-rw-r--r--   0        0        0     1609 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市浦和区.json
+-rw-r--r--   0        0        0     1201 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市緑区.json
+-rw-r--r--   0        0        0      706 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市西区.json
+-rw-r--r--   0        0        0     1303 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市見沼区.json
+-rw-r--r--   0        0        0     2362 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/ふじみ野市.json
+-rw-r--r--   0        0        0     1930 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/三郷市.json
+-rw-r--r--   0        0        0     2425 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/上尾市.json
+-rw-r--r--   0        0        0     2536 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/久喜市.json
+-rw-r--r--   0        0        0      268 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/児玉郡上里町.json
+-rw-r--r--   0        0        0      337 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/児玉郡神川町.json
+-rw-r--r--   0        0        0      271 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/児玉郡美里町.json
+-rw-r--r--   0        0        0     1732 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/入間市.json
+-rw-r--r--   0        0        0      100 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/入間郡三芳町.json
+-rw-r--r--   0        0        0      934 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/入間郡毛呂山町.json
+-rw-r--r--   0        0        0      517 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/入間郡越生町.json
+-rw-r--r--   0        0        0      787 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/八潮市.json
+-rw-r--r--   0        0        0     2044 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/加須市.json
+-rw-r--r--   0        0        0     2350 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/北本市.json
+-rw-r--r--   0        0        0     1102 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/北葛飾郡杉戸町.json
+-rw-r--r--   0        0        0      487 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/北葛飾郡松伏町.json
+-rw-r--r--   0        0        0      652 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/北足立郡伊奈町.json
+-rw-r--r--   0        0        0      967 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/南埼玉郡宮代町.json
+-rw-r--r--   0        0        0     1636 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/吉川市.json
+-rw-r--r--   0        0        0      568 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/和光市.json
+-rw-r--r--   0        0        0     1765 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/坂戸市.json
+-rw-r--r--   0        0        0      364 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/大里郡寄居町.json
+-rw-r--r--   0        0        0     1231 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/富士見市.json
+-rw-r--r--   0        0        0     5152 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/川口市.json
+-rw-r--r--   0        0        0     4528 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/川越市.json
+-rw-r--r--   0        0        0     1066 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/幸手市.json
+-rw-r--r--   0        0        0      622 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/志木市.json
+-rw-r--r--   0        0        0     1153 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/戸田市.json
+-rw-r--r--   0        0        0     3043 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/所沢市.json
+-rw-r--r--   0        0        0     1501 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/新座市.json
+-rw-r--r--   0        0        0      970 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/日高市.json
+-rw-r--r--   0        0        0     2242 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/春日部市.json
+-rw-r--r--   0        0        0     1486 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/朝霞市.json
+-rw-r--r--   0        0        0     2536 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/本庄市.json
+-rw-r--r--   0        0        0     1225 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/東松山市.json
+-rw-r--r--   0        0        0      820 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/桶川市.json
+-rw-r--r--   0        0        0      286 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/比企郡ときがわ町.json
+-rw-r--r--   0        0        0      859 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/比企郡吉見町.json
+-rw-r--r--   0        0        0      748 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/比企郡小川町.json
+-rw-r--r--   0        0        0      349 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/比企郡嵐山町.json
+-rw-r--r--   0        0        0     1009 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/比企郡川島町.json
+-rw-r--r--   0        0        0      406 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/比企郡滑川町.json
+-rw-r--r--   0        0        0      460 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/比企郡鳩山町.json
+-rw-r--r--   0        0        0     1666 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/深谷市.json
+-rw-r--r--   0        0        0     3409 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/熊谷市.json
+-rw-r--r--   0        0        0     1030 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/狭山市.json
+-rw-r--r--   0        0        0      544 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/白岡市.json
+-rw-r--r--   0        0        0      898 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/秩父市.json
+-rw-r--r--   0        0        0      133 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/秩父郡小鹿野町.json
+-rw-r--r--   0        0        0      109 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/秩父郡東秩父村.json
+-rw-r--r--   0        0        0       37 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/秩父郡横瀬町.json
+-rw-r--r--   0        0        0      166 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/秩父郡皆野町.json
+-rw-r--r--   0        0        0      136 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/秩父郡長瀞町.json
+-rw-r--r--   0        0        0     1423 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/羽生市.json
+-rw-r--r--   0        0        0     2017 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/草加市.json
+-rw-r--r--   0        0        0     1186 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/蓮田市.json
+-rw-r--r--   0        0        0      523 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/蕨市.json
+-rw-r--r--   0        0        0     1525 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/行田市.json
+-rw-r--r--   0        0        0     3916 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/越谷市.json
+-rw-r--r--   0        0        0     1351 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/飯能市.json
+-rw-r--r--   0        0        0     2059 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/鴻巣市.json
+-rw-r--r--   0        0        0      826 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/鶴ヶ島市.json
+-rw-r--r--   0        0        0     2269 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/中津市.json
+-rw-r--r--   0        0        0     2821 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/佐伯市.json
+-rw-r--r--   0        0        0     1984 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/別府市.json
+-rw-r--r--   0        0        0     1402 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/国東市.json
+-rw-r--r--   0        0        0    11974 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/大分市.json
+-rw-r--r--   0        0        0     4405 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/宇佐市.json
+-rw-r--r--   0        0        0     1372 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/日田市.json
+-rw-r--r--   0        0        0      241 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/東国東郡姫島村.json
+-rw-r--r--   0        0        0      769 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/杵築市.json
+-rw-r--r--   0        0        0      526 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/津久見市.json
+-rw-r--r--   0        0        0      169 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/玖珠郡九重町.json
+-rw-r--r--   0        0        0      229 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/玖珠郡玖珠町.json
+-rw-r--r--   0        0        0     1084 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/由布市.json
+-rw-r--r--   0        0        0     1366 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/竹田市.json
+-rw-r--r--   0        0        0     1297 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/臼杵市.json
+-rw-r--r--   0        0        0     2458 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/豊後大野市.json
+-rw-r--r--   0        0        0      610 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/豊後高田市.json
+-rw-r--r--   0        0        0      145 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/速見郡日出町.json
+-rw-r--r--   0        0        0      706 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/三島郡島本町.json
+-rw-r--r--   0        0        0     2752 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/交野市.json
+-rw-r--r--   0        0        0    13480 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/八尾市.json
+-rw-r--r--   0        0        0      163 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/南河内郡千早赤阪村.json
+-rw-r--r--   0        0        0      157 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/南河内郡太子町.json
+-rw-r--r--   0        0        0      562 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/南河内郡河南町.json
+-rw-r--r--   0        0        0     3571 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/吹田市.json
+-rw-r--r--   0        0        0     3130 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/和泉市.json
+-rw-r--r--   0        0        0     1060 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/四條畷市.json
+-rw-r--r--   0        0        0      634 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市中区.json
+-rw-r--r--   0        0        0     1966 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市北区.json
+-rw-r--r--   0        0        0     1534 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市南区.json
+-rw-r--r--   0        0        0    10045 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市堺区.json
+-rw-r--r--   0        0        0      757 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市東区.json
+-rw-r--r--   0        0        0      634 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市美原区.json
+-rw-r--r--   0        0        0     2971 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市西区.json
+-rw-r--r--   0        0        0     2170 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大東市.json
+-rw-r--r--   0        0        0     3805 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市中央区.json
+-rw-r--r--   0        0        0     2098 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市住之江区.json
+-rw-r--r--   0        0        0     2128 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市住吉区.json
+-rw-r--r--   0        0        0     2281 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市北区.json
+-rw-r--r--   0        0        0     1486 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市城東区.json
+-rw-r--r--   0        0        0      988 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市大正区.json
+-rw-r--r--   0        0        0     1189 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市天王寺区.json
+-rw-r--r--   0        0        0     3049 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市平野区.json
+-rw-r--r--   0        0        0      826 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市旭区.json
+-rw-r--r--   0        0        0     2026 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市東住吉区.json
+-rw-r--r--   0        0        0      904 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市東成区.json
+-rw-r--r--   0        0        0     1687 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市東淀川区.json
+-rw-r--r--   0        0        0     1174 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市此花区.json
+-rw-r--r--   0        0        0     1255 2021-06-17 01:45:25.837508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市浪速区.json
+-rw-r--r--   0        0        0     1840 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市淀川区.json
+-rw-r--r--   0        0        0     1096 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市港区.json
+-rw-r--r--   0        0        0     1735 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市生野区.json
+-rw-r--r--   0        0        0      763 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市福島区.json
+-rw-r--r--   0        0        0     1195 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市西区.json
+-rw-r--r--   0        0        0     1672 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市西成区.json
+-rw-r--r--   0        0        0     1159 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市西淀川区.json
+-rw-r--r--   0        0        0     1030 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市都島区.json
+-rw-r--r--   0        0        0     1441 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市阿倍野区.json
+-rw-r--r--   0        0        0     1114 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市鶴見区.json
+-rw-r--r--   0        0        0     1693 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪狭山市.json
+-rw-r--r--   0        0        0     3505 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/守口市.json
+-rw-r--r--   0        0        0     3592 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/富田林市.json
+-rw-r--r--   0        0        0     2863 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/寝屋川市.json
+-rw-r--r--   0        0        0     2971 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/岸和田市.json
+-rw-r--r--   0        0        0     1876 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/摂津市.json
+-rw-r--r--   0        0        0    10141 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/東大阪市.json
+-rw-r--r--   0        0        0     3406 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/松原市.json
+-rw-r--r--   0        0        0     7948 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/枚方市.json
+-rw-r--r--   0        0        0     1210 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/柏原市.json
+-rw-r--r--   0        0        0     1384 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/池田市.json
+-rw-r--r--   0        0        0     1684 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/河内長野市.json
+-rw-r--r--   0        0        0     1879 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/泉佐野市.json
+-rw-r--r--   0        0        0      520 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/泉北郡忠岡町.json
+-rw-r--r--   0        0        0      940 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/泉南市.json
+-rw-r--r--   0        0        0      178 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/泉南郡岬町.json
+-rw-r--r--   0        0        0     2359 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/泉南郡熊取町.json
+-rw-r--r--   0        0        0       94 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/泉南郡田尻町.json
+-rw-r--r--   0        0        0     1528 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/泉大津市.json
+-rw-r--r--   0        0        0     3442 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/箕面市.json
+-rw-r--r--   0        0        0     2596 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/羽曳野市.json
+-rw-r--r--   0        0        0     5485 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/茨木市.json
+-rw-r--r--   0        0        0     1555 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/藤井寺市.json
+-rw-r--r--   0        0        0     7237 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/豊中市.json
+-rw-r--r--   0        0        0      304 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/豊能郡能勢町.json
+-rw-r--r--   0        0        0      859 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/豊能郡豊能町.json
+-rw-r--r--   0        0        0      976 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/貝塚市.json
+-rw-r--r--   0        0        0     1261 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/門真市.json
+-rw-r--r--   0        0        0      838 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/阪南市.json
+-rw-r--r--   0        0        0     6973 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/高槻市.json
+-rw-r--r--   0        0        0      997 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/高石市.json
+-rw-r--r--   0        0        0     3037 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/五條市.json
+-rw-r--r--   0        0        0      934 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/北葛城郡上牧町.json
+-rw-r--r--   0        0        0      715 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/北葛城郡広陵町.json
+-rw-r--r--   0        0        0      553 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/北葛城郡河合町.json
+-rw-r--r--   0        0        0      820 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/北葛城郡王寺町.json
+-rw-r--r--   0        0        0       61 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡上北山村.json
+-rw-r--r--   0        0        0      151 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡下北山村.json
+-rw-r--r--   0        0        0      322 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡下市町.json
+-rw-r--r--   0        0        0      868 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡十津川村.json
+-rw-r--r--   0        0        0      580 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡吉野町.json
+-rw-r--r--   0        0        0      355 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡大淀町.json
+-rw-r--r--   0        0        0      352 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡天川村.json
+-rw-r--r--   0        0        0      385 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡川上村.json
+-rw-r--r--   0        0        0      280 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡東吉野村.json
+-rw-r--r--   0        0        0      214 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡野迫川村.json
+-rw-r--r--   0        0        0      187 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡黒滝村.json
+-rw-r--r--   0        0        0     1609 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/大和郡山市.json
+-rw-r--r--   0        0        0     1237 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/大和高田市.json
+-rw-r--r--   0        0        0     1036 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/天理市.json
+-rw-r--r--   0        0        0    11953 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/奈良市.json
+-rw-r--r--   0        0        0     2713 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/宇陀市.json
+-rw-r--r--   0        0        0       64 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/宇陀郡御杖村.json
+-rw-r--r--   0        0        0      139 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/宇陀郡曽爾村.json
+-rw-r--r--   0        0        0      448 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/山辺郡山添村.json
+-rw-r--r--   0        0        0     1078 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/御所市.json
+-rw-r--r--   0        0        0     1645 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/桜井市.json
+-rw-r--r--   0        0        0     1762 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/橿原市.json
+-rw-r--r--   0        0        0     2020 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/生駒市.json
+-rw-r--r--   0        0        0     1003 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/生駒郡三郷町.json
+-rw-r--r--   0        0        0      148 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/生駒郡安堵町.json
+-rw-r--r--   0        0        0     1240 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/生駒郡平群町.json
+-rw-r--r--   0        0        0     1771 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/生駒郡斑鳩町.json
+-rw-r--r--   0        0        0      109 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/磯城郡三宅町.json
+-rw-r--r--   0        0        0       91 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/磯城郡川西町.json
+-rw-r--r--   0        0        0      691 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/磯城郡田原本町.json
+-rw-r--r--   0        0        0      412 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/葛城市.json
+-rw-r--r--   0        0        0     1759 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/香芝市.json
+-rw-r--r--   0        0        0      484 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/高市郡明日香村.json
+-rw-r--r--   0        0        0      382 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/高市郡高取町.json
+-rw-r--r--   0        0        0     1012 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/亘理郡亘理町.json
+-rw-r--r--   0        0        0      223 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/亘理郡山元町.json
+-rw-r--r--   0        0        0     3499 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/仙台市太白区.json
+-rw-r--r--   0        0        0     3292 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/仙台市宮城野区.json
+-rw-r--r--   0        0        0     3454 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/仙台市泉区.json
+-rw-r--r--   0        0        0     2527 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/仙台市若林区.json
+-rw-r--r--   0        0        0     5209 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/仙台市青葉区.json
+-rw-r--r--   0        0        0     3661 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/伊具郡丸森町.json
+-rw-r--r--   0        0        0     3961 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/刈田郡七ヶ宿町.json
+-rw-r--r--   0        0        0      238 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/刈田郡蔵王町.json
+-rw-r--r--   0        0        0    11290 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/加美郡加美町.json
+-rw-r--r--   0        0        0      115 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/加美郡色麻町.json
+-rw-r--r--   0        0        0     2173 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/名取市.json
+-rw-r--r--   0        0        0     1414 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/塩竈市.json
+-rw-r--r--   0        0        0     1270 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/多賀城市.json
+-rw-r--r--   0        0        0     4492 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/大崎市.json
+-rw-r--r--   0        0        0      454 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/宮城郡七ヶ浜町.json
+-rw-r--r--   0        0        0      637 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/宮城郡利府町.json
+-rw-r--r--   0        0        0       97 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/宮城郡松島町.json
+-rw-r--r--   0        0        0     1114 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/富谷市.json
+-rw-r--r--   0        0        0     1729 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/岩沼市.json
+-rw-r--r--   0        0        0       40 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/本吉郡南三陸町.json
+-rw-r--r--   0        0        0      388 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/東松島市.json
+-rw-r--r--   0        0        0      910 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/柴田郡大河原町.json
+-rw-r--r--   0        0        0      130 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/柴田郡川崎町.json
+-rw-r--r--   0        0        0      121 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/柴田郡村田町.json
+-rw-r--r--   0        0        0     1498 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/柴田郡柴田町.json
+-rw-r--r--   0        0        0     2872 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/栗原市.json
+-rw-r--r--   0        0        0     6532 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/気仙沼市.json
+-rw-r--r--   0        0        0      349 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/牡鹿郡女川町.json
+-rw-r--r--   0        0        0     6940 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/登米市.json
+-rw-r--r--   0        0        0     1597 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/白石市.json
+-rw-r--r--   0        0        0     5854 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/石巻市.json
+-rw-r--r--   0        0        0      211 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/角田市.json
+-rw-r--r--   0        0        0     1867 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/遠田郡涌谷町.json
+-rw-r--r--   0        0        0     1009 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/遠田郡美里町.json
+-rw-r--r--   0        0        0      940 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/黒川郡大和町.json
+-rw-r--r--   0        0        0      178 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/黒川郡大衡村.json
+-rw-r--r--   0        0        0      118 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/黒川郡大郷町.json
+-rw-r--r--   0        0        0      481 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/えびの市.json
+-rw-r--r--   0        0        0      328 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/串間市.json
+-rw-r--r--   0        0        0       31 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/児湯郡川南町.json
+-rw-r--r--   0        0        0      427 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/児湯郡新富町.json
+-rw-r--r--   0        0        0       82 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/児湯郡木城町.json
+-rw-r--r--   0        0        0      112 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/児湯郡西米良村.json
+-rw-r--r--   0        0        0       16 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/児湯郡都農町.json
+-rw-r--r--   0        0        0      103 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/児湯郡高鍋町.json
+-rw-r--r--   0        0        0      139 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/北諸県郡三股町.json
+-rw-r--r--   0        0        0     6895 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/宮崎市.json
+-rw-r--r--   0        0        0      271 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/小林市.json
+-rw-r--r--   0        0        0     5611 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/延岡市.json
+-rw-r--r--   0        0        0     2404 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/日南市.json
+-rw-r--r--   0        0        0     1834 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/日向市.json
+-rw-r--r--   0        0        0       70 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/東臼杵郡椎葉村.json
+-rw-r--r--   0        0        0      217 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/東臼杵郡美郷町.json
+-rw-r--r--   0        0        0       34 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/東臼杵郡諸塚村.json
+-rw-r--r--   0        0        0     1165 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/東臼杵郡門川町.json
+-rw-r--r--   0        0        0      265 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/東諸県郡国富町.json
+-rw-r--r--   0        0        0       46 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/東諸県郡綾町.json
+-rw-r--r--   0        0        0       52 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/西臼杵郡五ヶ瀬町.json
+-rw-r--r--   0        0        0       64 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/西臼杵郡日之影町.json
+-rw-r--r--   0        0        0      160 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/西臼杵郡高千穂町.json
+-rw-r--r--   0        0        0       67 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/西諸県郡高原町.json
+-rw-r--r--   0        0        0     1069 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/西都市.json
+-rw-r--r--   0        0        0     1618 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/都城市.json
+-rw-r--r--   0        0        0      589 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/下新川郡入善町.json
+-rw-r--r--   0        0        0      448 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/下新川郡朝日町.json
+-rw-r--r--   0        0        0     1402 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/中新川郡上市町.json
+-rw-r--r--   0        0        0     1405 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/中新川郡立山町.json
+-rw-r--r--   0        0        0      109 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/中新川郡舟橋村.json
+-rw-r--r--   0        0        0     3085 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/南砺市.json
+-rw-r--r--   0        0        0    20935 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/富山市.json
+-rw-r--r--   0        0        0     3928 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/射水市.json
+-rw-r--r--   0        0        0     1393 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/小矢部市.json
+-rw-r--r--   0        0        0     1207 2021-06-17 01:45:25.841508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/氷見市.json
+-rw-r--r--   0        0        0     1228 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/滑川市.json
+-rw-r--r--   0        0        0     1807 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/砺波市.json
+-rw-r--r--   0        0        0     5551 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/高岡市.json
+-rw-r--r--   0        0        0     1579 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/魚津市.json
+-rw-r--r--   0        0        0     1510 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/黒部市.json
+-rw-r--r--   0        0        0     2305 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/下松市.json
+-rw-r--r--   0        0        0    13816 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/下関市.json
+-rw-r--r--   0        0        0     1927 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/光市.json
+-rw-r--r--   0        0        0     5635 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/周南市.json
+-rw-r--r--   0        0        0      565 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/大島郡周防大島町.json
+-rw-r--r--   0        0        0     5422 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/宇部市.json
+-rw-r--r--   0        0        0     4921 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/山口市.json
+-rw-r--r--   0        0        0     1429 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/山陽小野田市.json
+-rw-r--r--   0        0        0     5089 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/岩国市.json
+-rw-r--r--   0        0        0      556 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/柳井市.json
+-rw-r--r--   0        0        0       61 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/熊毛郡上関町.json
+-rw-r--r--   0        0        0      187 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/熊毛郡平生町.json
+-rw-r--r--   0        0        0      202 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/熊毛郡田布施町.json
+-rw-r--r--   0        0        0      250 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/玖珂郡和木町.json
+-rw-r--r--   0        0        0      655 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/美祢市.json
+-rw-r--r--   0        0        0     1228 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/萩市.json
+-rw-r--r--   0        0        0      370 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/長門市.json
+-rw-r--r--   0        0        0     2194 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/防府市.json
+-rw-r--r--   0        0        0      115 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/阿武郡阿武町.json
+-rw-r--r--   0        0        0     1531 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/上山市.json
+-rw-r--r--   0        0        0      238 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/北村山郡大石田町.json
+-rw-r--r--   0        0        0      454 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/南陽市.json
+-rw-r--r--   0        0        0     3094 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/天童市.json
+-rw-r--r--   0        0        0     1426 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/寒河江市.json
+-rw-r--r--   0        0        0     1027 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/尾花沢市.json
+-rw-r--r--   0        0        0     8992 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/山形市.json
+-rw-r--r--   0        0        0      556 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/新庄市.json
+-rw-r--r--   0        0        0       61 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/最上郡大蔵村.json
+-rw-r--r--   0        0        0      124 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/最上郡戸沢村.json
+-rw-r--r--   0        0        0      184 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/最上郡最上町.json
+-rw-r--r--   0        0        0      160 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/最上郡真室川町.json
+-rw-r--r--   0        0        0       49 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/最上郡舟形町.json
+-rw-r--r--   0        0        0      190 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/最上郡金山町.json
+-rw-r--r--   0        0        0      124 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/最上郡鮭川村.json
+-rw-r--r--   0        0        0      982 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/村山市.json
+-rw-r--r--   0        0        0      148 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/東村山郡中山町.json
+-rw-r--r--   0        0        0      424 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/東村山郡山辺町.json
+-rw-r--r--   0        0        0     2629 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/東根市.json
+-rw-r--r--   0        0        0      316 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/東田川郡三川町.json
+-rw-r--r--   0        0        0      694 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/東田川郡庄内町.json
+-rw-r--r--   0        0        0      358 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/東置賜郡川西町.json
+-rw-r--r--   0        0        0      592 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/東置賜郡高畠町.json
+-rw-r--r--   0        0        0     3418 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/米沢市.json
+-rw-r--r--   0        0        0      577 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/西村山郡大江町.json
+-rw-r--r--   0        0        0      439 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/西村山郡朝日町.json
+-rw-r--r--   0        0        0      475 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/西村山郡河北町.json
+-rw-r--r--   0        0        0      253 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/西村山郡西川町.json
+-rw-r--r--   0        0        0     1573 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/西置賜郡小国町.json
+-rw-r--r--   0        0        0      361 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/西置賜郡白鷹町.json
+-rw-r--r--   0        0        0      349 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/西置賜郡飯豊町.json
+-rw-r--r--   0        0        0     4861 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/酒田市.json
+-rw-r--r--   0        0        0      655 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/長井市.json
+-rw-r--r--   0        0        0      235 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/飽海郡遊佐町.json
+-rw-r--r--   0        0        0     3841 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/鶴岡市.json
+-rw-r--r--   0        0        0      319 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/上野原市.json
+-rw-r--r--   0        0        0      295 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/中央市.json
+-rw-r--r--   0        0        0      139 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/中巨摩郡昭和町.json
+-rw-r--r--   0        0        0     1435 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/北杜市.json
+-rw-r--r--   0        0        0       70 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/北都留郡丹波山村.json
+-rw-r--r--   0        0        0      220 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/北都留郡小菅村.json
+-rw-r--r--   0        0        0      709 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/南アルプス市.json
+-rw-r--r--   0        0        0      133 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/南巨摩郡南部町.json
+-rw-r--r--   0        0        0      232 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/南巨摩郡富士川町.json
+-rw-r--r--   0        0        0      208 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/南巨摩郡早川町.json
+-rw-r--r--   0        0        0      820 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/南巨摩郡身延町.json
+-rw-r--r--   0        0        0      139 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/南都留郡富士河口湖町.json
+-rw-r--r--   0        0        0       19 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/南都留郡山中湖村.json
+-rw-r--r--   0        0        0       19 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/南都留郡忍野村.json
+-rw-r--r--   0        0        0       31 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/南都留郡西桂町.json
+-rw-r--r--   0        0        0     1138 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/南都留郡道志村.json
+-rw-r--r--   0        0        0     1036 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/南都留郡鳴沢村.json
+-rw-r--r--   0        0        0      895 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/大月市.json
+-rw-r--r--   0        0        0     1969 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/富士吉田市.json
+-rw-r--r--   0        0        0      712 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/山梨市.json
+-rw-r--r--   0        0        0      808 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/甲州市.json
+-rw-r--r--   0        0        0     3559 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/甲府市.json
+-rw-r--r--   0        0        0      406 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/甲斐市.json
+-rw-r--r--   0        0        0     1933 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/笛吹市.json
+-rw-r--r--   0        0        0      241 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/西八代郡市川三郷町.json
+-rw-r--r--   0        0        0      718 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/都留市.json
+-rw-r--r--   0        0        0     1090 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/韮崎市.json
+-rw-r--r--   0        0        0     1264 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/下呂市.json
+-rw-r--r--   0        0        0      355 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/不破郡垂井町.json
+-rw-r--r--   0        0        0      121 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/不破郡関ケ原町.json
+-rw-r--r--   0        0        0      616 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/中津川市.json
+-rw-r--r--   0        0        0       43 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/加茂郡七宗町.json
+-rw-r--r--   0        0        0      130 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/加茂郡八百津町.json
+-rw-r--r--   0        0        0      169 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/加茂郡坂祝町.json
+-rw-r--r--   0        0        0       70 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/加茂郡富加町.json
+-rw-r--r--   0        0        0      145 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/加茂郡川辺町.json
+-rw-r--r--   0        0        0       28 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/加茂郡東白川村.json
+-rw-r--r--   0        0        0      139 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/加茂郡白川町.json
+-rw-r--r--   0        0        0     3187 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/可児市.json
+-rw-r--r--   0        0        0      193 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/可児郡御嵩町.json
+-rw-r--r--   0        0        0    16522 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/各務原市.json
+-rw-r--r--   0        0        0     3577 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/土岐市.json
+-rw-r--r--   0        0        0     9340 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/多治見市.json
+-rw-r--r--   0        0        0    11977 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/大垣市.json
+-rw-r--r--   0        0        0      361 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/大野郡白川村.json
+-rw-r--r--   0        0        0      217 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/安八郡安八町.json
+-rw-r--r--   0        0        0      373 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/安八郡神戸町.json
+-rw-r--r--   0        0        0      208 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/安八郡輪之内町.json
+-rw-r--r--   0        0        0      355 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/山県市.json
+-rw-r--r--   0        0        0    43126 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/岐阜市.json
+-rw-r--r--   0        0        0      928 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/恵那市.json
+-rw-r--r--   0        0        0      466 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/揖斐郡大野町.json
+-rw-r--r--   0        0        0      748 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/揖斐郡揖斐川町.json
+-rw-r--r--   0        0        0      256 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/揖斐郡池田町.json
+-rw-r--r--   0        0        0      913 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/本巣市.json
+-rw-r--r--   0        0        0     1975 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/本巣郡北方町.json
+-rw-r--r--   0        0        0     1501 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/海津市.json
+-rw-r--r--   0        0        0     1642 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/瑞浪市.json
+-rw-r--r--   0        0        0     1024 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/瑞穂市.json
+-rw-r--r--   0        0        0     2260 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/美濃加茂市.json
+-rw-r--r--   0        0        0      763 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/美濃市.json
+-rw-r--r--   0        0        0     6301 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/羽島市.json
+-rw-r--r--   0        0        0     2005 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/羽島郡岐南町.json
+-rw-r--r--   0        0        0      640 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/羽島郡笠松町.json
+-rw-r--r--   0        0        0     2248 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/郡上市.json
+-rw-r--r--   0        0        0     5932 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/関市.json
+-rw-r--r--   0        0        0     2953 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/飛騨市.json
+-rw-r--r--   0        0        0      574 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/養老郡養老町.json
+-rw-r--r--   0        0        0     6508 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/高山市.json
+-rw-r--r--   0        0        0      277 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/久米郡久米南町.json
+-rw-r--r--   0        0        0      658 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/久米郡美咲町.json
+-rw-r--r--   0        0        0     1048 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/井原市.json
+-rw-r--r--   0        0        0     6946 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/倉敷市.json
+-rw-r--r--   0        0        0      586 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/備前市.json
+-rw-r--r--   0        0        0      442 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/加賀郡吉備中央町.json
+-rw-r--r--   0        0        0      223 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/勝田郡勝央町.json
+-rw-r--r--   0        0        0      172 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/勝田郡奈義町.json
+-rw-r--r--   0        0        0      370 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/和気郡和気町.json
+-rw-r--r--   0        0        0      181 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/小田郡矢掛町.json
+-rw-r--r--   0        0        0     2050 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/岡山市中区.json
+-rw-r--r--   0        0        0     6463 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/岡山市北区.json
+-rw-r--r--   0        0        0     1684 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/岡山市南区.json
+-rw-r--r--   0        0        0     2131 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/岡山市東区.json
+-rw-r--r--   0        0        0      760 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/新見市.json
+-rw-r--r--   0        0        0     2197 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/津山市.json
+-rw-r--r--   0        0        0      655 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/浅口市.json
+-rw-r--r--   0        0        0       85 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/浅口郡里庄町.json
+-rw-r--r--   0        0        0      781 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/瀬戸内市.json
+-rw-r--r--   0        0        0     1378 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/玉野市.json
+-rw-r--r--   0        0        0     1534 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/真庭市.json
+-rw-r--r--   0        0        0      220 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/真庭郡新庄村.json
+-rw-r--r--   0        0        0      799 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/笠岡市.json
+-rw-r--r--   0        0        0      814 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/総社市.json
+-rw-r--r--   0        0        0     1369 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/美作市.json
+-rw-r--r--   0        0        0      589 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/苫田郡鏡野町.json
+-rw-r--r--   0        0        0       91 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/英田郡西粟倉村.json
+-rw-r--r--   0        0        0     1423 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/赤磐市.json
+-rw-r--r--   0        0        0       37 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/都窪郡早島町.json
+-rw-r--r--   0        0        0     1597 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/高梁市.json
+-rw-r--r--   0        0        0     1831 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/一関市.json
+-rw-r--r--   0        0        0      391 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/上閉伊郡大槌町.json
+-rw-r--r--   0        0        0      220 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/下閉伊郡山田町.json
+-rw-r--r--   0        0        0      181 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/下閉伊郡岩泉町.json
+-rw-r--r--   0        0        0      874 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/下閉伊郡普代村.json
+-rw-r--r--   0        0        0      403 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/下閉伊郡田野畑村.json
+-rw-r--r--   0        0        0      922 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/久慈市.json
+-rw-r--r--   0        0        0      145 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/九戸郡九戸村.json
+-rw-r--r--   0        0        0       88 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/九戸郡洋野町.json
+-rw-r--r--   0        0        0      154 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/九戸郡軽米町.json
+-rw-r--r--   0        0        0       31 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/九戸郡野田村.json
+-rw-r--r--   0        0        0      169 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/二戸市.json
+-rw-r--r--   0        0        0      196 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/二戸郡一戸町.json
+-rw-r--r--   0        0        0     1651 2021-06-17 01:45:25.845508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/八幡平市.json
+-rw-r--r--   0        0        0     2050 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/北上市.json
+-rw-r--r--   0        0        0      622 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/和賀郡西和賀町.json
+-rw-r--r--   0        0        0      145 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/大船渡市.json
+-rw-r--r--   0        0        0     5386 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/奥州市.json
+-rw-r--r--   0        0        0     2545 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/宮古市.json
+-rw-r--r--   0        0        0      223 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/岩手郡岩手町.json
+-rw-r--r--   0        0        0       28 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/岩手郡葛巻町.json
+-rw-r--r--   0        0        0      631 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/岩手郡雫石町.json
+-rw-r--r--   0        0        0       37 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/気仙郡住田町.json
+-rw-r--r--   0        0        0     2794 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/滝沢市.json
+-rw-r--r--   0        0        0     7174 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/盛岡市.json
+-rw-r--r--   0        0        0      571 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/紫波郡矢巾町.json
+-rw-r--r--   0        0        0      751 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/紫波郡紫波町.json
+-rw-r--r--   0        0        0       49 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/胆沢郡金ケ崎町.json
+-rw-r--r--   0        0        0     3088 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/花巻市.json
+-rw-r--r--   0        0        0       19 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/西磐井郡平泉町.json
+-rw-r--r--   0        0        0      886 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/遠野市.json
+-rw-r--r--   0        0        0     1501 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/釜石市.json
+-rw-r--r--   0        0        0       97 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/陸前高田市.json
+-rw-r--r--   0        0        0      241 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/仁多郡奥出雲町.json
+-rw-r--r--   0        0        0     3886 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/出雲市.json
+-rw-r--r--   0        0        0     1201 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/大田市.json
+-rw-r--r--   0        0        0     1462 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/安来市.json
+-rw-r--r--   0        0        0     4555 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/松江市.json
+-rw-r--r--   0        0        0      805 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/江津市.json
+-rw-r--r--   0        0        0     1705 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/浜田市.json
+-rw-r--r--   0        0        0     1510 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/益田市.json
+-rw-r--r--   0        0        0      256 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/邑智郡川本町.json
+-rw-r--r--   0        0        0      418 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/邑智郡美郷町.json
+-rw-r--r--   0        0        0      352 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/邑智郡邑南町.json
+-rw-r--r--   0        0        0      109 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/隠岐郡海士町.json
+-rw-r--r--   0        0        0       97 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/隠岐郡知夫村.json
+-rw-r--r--   0        0        0       61 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/隠岐郡西ノ島町.json
+-rw-r--r--   0        0        0      391 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/隠岐郡隠岐の島町.json
+-rw-r--r--   0        0        0     1816 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/雲南市.json
+-rw-r--r--   0        0        0      202 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/飯石郡飯南町.json
+-rw-r--r--   0        0        0      328 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/鹿足郡吉賀町.json
+-rw-r--r--   0        0        0      346 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/鹿足郡津和野町.json
+-rw-r--r--   0        0        0     4105 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/三原市.json
+-rw-r--r--   0        0        0     2404 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/三次市.json
+-rw-r--r--   0        0        0      601 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/世羅郡世羅町.json
+-rw-r--r--   0        0        0    11413 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/呉市.json
+-rw-r--r--   0        0        0     1273 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/大竹市.json
+-rw-r--r--   0        0        0      718 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/安芸郡坂町.json
+-rw-r--r--   0        0        0     1075 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/安芸郡府中町.json
+-rw-r--r--   0        0        0      643 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/安芸郡海田町.json
+-rw-r--r--   0        0        0     1291 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/安芸郡熊野町.json
+-rw-r--r--   0        0        0      964 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/安芸高田市.json
+-rw-r--r--   0        0        0     2362 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/尾道市.json
+-rw-r--r--   0        0        0      673 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/山県郡北広島町.json
+-rw-r--r--   0        0        0      433 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/山県郡安芸太田町.json
+-rw-r--r--   0        0        0     1873 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/広島市中区.json
+-rw-r--r--   0        0        0     3601 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/広島市佐伯区.json
+-rw-r--r--   0        0        0     2551 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/広島市南区.json
+-rw-r--r--   0        0        0     3016 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/広島市安佐北区.json
+-rw-r--r--   0        0        0     3433 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/広島市安佐南区.json
+-rw-r--r--   0        0        0     1432 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/広島市安芸区.json
+-rw-r--r--   0        0        0     2752 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/広島市東区.json
+-rw-r--r--   0        0        0     3025 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/広島市西区.json
+-rw-r--r--   0        0        0     2038 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/庄原市.json
+-rw-r--r--   0        0        0      688 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/府中市.json
+-rw-r--r--   0        0        0     3376 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/廿日市市.json
+-rw-r--r--   0        0        0     4276 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/東広島市.json
+-rw-r--r--   0        0        0     1426 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/江田島市.json
+-rw-r--r--   0        0        0      340 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/神石郡神石高原町.json
+-rw-r--r--   0        0        0     8848 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/福山市.json
+-rw-r--r--   0        0        0      919 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/竹原市.json
+-rw-r--r--   0        0        0       64 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/豊田郡大崎上島町.json
+-rw-r--r--   0        0        0     3064 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/三好市.json
+-rw-r--r--   0        0        0       64 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/三好郡東みよし町.json
+-rw-r--r--   0        0        0       73 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/勝浦郡上勝町.json
+-rw-r--r--   0        0        0      121 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/勝浦郡勝浦町.json
+-rw-r--r--   0        0        0     2884 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/吉野川市.json
+-rw-r--r--   0        0        0       13 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/名東郡佐那河内村.json
+-rw-r--r--   0        0        0       49 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/名西郡石井町.json
+-rw-r--r--   0        0        0       49 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/名西郡神山町.json
+-rw-r--r--   0        0        0      331 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/小松島市.json
+-rw-r--r--   0        0        0    10192 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/徳島市.json
+-rw-r--r--   0        0        0      148 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/板野郡上板町.json
+-rw-r--r--   0        0        0       73 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/板野郡北島町.json
+-rw-r--r--   0        0        0       97 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/板野郡松茂町.json
+-rw-r--r--   0        0        0      142 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/板野郡板野町.json
+-rw-r--r--   0        0        0       85 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/板野郡藍住町.json
+-rw-r--r--   0        0        0      295 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/海部郡海陽町.json
+-rw-r--r--   0        0        0      118 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/海部郡牟岐町.json
+-rw-r--r--   0        0        0      184 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/海部郡美波町.json
+-rw-r--r--   0        0        0      310 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/美馬市.json
+-rw-r--r--   0        0        0       67 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/美馬郡つるぎ町.json
+-rw-r--r--   0        0        0      799 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/那賀郡那賀町.json
+-rw-r--r--   0        0        0     1309 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/阿南市.json
+-rw-r--r--   0        0        0     2887 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/阿波市.json
+-rw-r--r--   0        0        0     1090 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/鳴門市.json
+-rw-r--r--   0        0        0      376 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/上浮穴郡久万高原町.json
+-rw-r--r--   0        0        0     9199 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/今治市.json
+-rw-r--r--   0        0        0      403 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/伊予市.json
+-rw-r--r--   0        0        0      328 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/伊予郡松前町.json
+-rw-r--r--   0        0        0      307 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/伊予郡砥部町.json
+-rw-r--r--   0        0        0     1147 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/八幡浜市.json
+-rw-r--r--   0        0        0      145 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/北宇和郡松野町.json
+-rw-r--r--   0        0        0      622 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/北宇和郡鬼北町.json
+-rw-r--r--   0        0        0      682 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/南宇和郡愛南町.json
+-rw-r--r--   0        0        0      373 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/喜多郡内子町.json
+-rw-r--r--   0        0        0     1210 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/四国中央市.json
+-rw-r--r--   0        0        0     1108 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/大洲市.json
+-rw-r--r--   0        0        0     4201 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/宇和島市.json
+-rw-r--r--   0        0        0     3394 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/新居浜市.json
+-rw-r--r--   0        0        0      280 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/東温市.json
+-rw-r--r--   0        0        0    11143 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/松山市.json
+-rw-r--r--   0        0        0     2023 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/西予市.json
+-rw-r--r--   0        0        0      370 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/西宇和郡伊方町.json
+-rw-r--r--   0        0        0     2188 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/西条市.json
+-rw-r--r--   0        0        0      277 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/越智郡上島町.json
+-rw-r--r--   0        0        0     1540 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/あま市.json
+-rw-r--r--   0        0        0     1219 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/みよし市.json
+-rw-r--r--   0        0        0     7714 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/一宮市.json
+-rw-r--r--   0        0        0     1462 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/丹羽郡大口町.json
+-rw-r--r--   0        0        0      109 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/丹羽郡扶桑町.json
+-rw-r--r--   0        0        0     8101 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/刈谷市.json
+-rw-r--r--   0        0        0      625 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/北名古屋市.json
+-rw-r--r--   0        0        0      187 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/北設楽郡東栄町.json
+-rw-r--r--   0        0        0      193 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/北設楽郡設楽町.json
+-rw-r--r--   0        0        0       67 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/北設楽郡豊根村.json
+-rw-r--r--   0        0        0    12397 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/半田市.json
+-rw-r--r--   0        0        0     1084 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市中区.json
+-rw-r--r--   0        0        0    10321 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市中川区.json
+-rw-r--r--   0        0        0     7915 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市中村区.json
+-rw-r--r--   0        0        0     6553 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市北区.json
+-rw-r--r--   0        0        0     6577 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市千種区.json
+-rw-r--r--   0        0        0     7198 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市南区.json
+-rw-r--r--   0        0        0     3310 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市名東区.json
+-rw-r--r--   0        0        0     2644 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市天白区.json
+-rw-r--r--   0        0        0     2623 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市守山区.json
+-rw-r--r--   0        0        0     5890 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市昭和区.json
+-rw-r--r--   0        0        0     1573 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市東区.json
+-rw-r--r--   0        0        0     7003 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市港区.json
+-rw-r--r--   0        0        0     1795 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市熱田区.json
+-rw-r--r--   0        0        0     6838 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市瑞穂区.json
+-rw-r--r--   0        0        0     4048 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市緑区.json
+-rw-r--r--   0        0        0     3661 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市西区.json
+-rw-r--r--   0        0        0     3706 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/大府市.json
+-rw-r--r--   0        0        0     2104 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/安城市.json
+-rw-r--r--   0        0        0     3865 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/小牧市.json
+-rw-r--r--   0        0        0     3997 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/尾張旭市.json
+-rw-r--r--   0        0        0     5140 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/岡崎市.json
+-rw-r--r--   0        0        0      724 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/岩倉市.json
+-rw-r--r--   0        0        0     6946 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/常滑市.json
+-rw-r--r--   0        0        0     5371 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/弥富市.json
+-rw-r--r--   0        0        0      700 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/愛知郡東郷町.json
+-rw-r--r--   0        0        0      892 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/愛西市.json
+-rw-r--r--   0        0        0     1621 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/新城市.json
+-rw-r--r--   0        0        0     1396 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/日進市.json
+-rw-r--r--   0        0        0    10018 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/春日井市.json
+-rw-r--r--   0        0        0     1225 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/東海市.json
+-rw-r--r--   0        0        0     7138 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/江南市.json
+-rw-r--r--   0        0        0     4894 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/津島市.json
+-rw-r--r--   0        0        0      196 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/海部郡大治町.json
+-rw-r--r--   0        0        0     1771 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/海部郡蟹江町.json
+-rw-r--r--   0        0        0     1888 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/海部郡飛島村.json
+-rw-r--r--   0        0        0     5755 2021-06-17 01:45:25.849508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/清須市.json
+-rw-r--r--   0        0        0     6481 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/瀬戸市.json
+-rw-r--r--   0        0        0     6529 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/犬山市.json
+-rw-r--r--   0        0        0     1093 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/田原市.json
+-rw-r--r--   0        0        0     3178 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/知多市.json
+-rw-r--r--   0        0        0      142 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/知多郡南知多町.json
+-rw-r--r--   0        0        0       76 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/知多郡東浦町.json
+-rw-r--r--   0        0        0     3064 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/知多郡武豊町.json
+-rw-r--r--   0        0        0      538 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/知多郡美浜町.json
+-rw-r--r--   0        0        0      508 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/知多郡阿久比町.json
+-rw-r--r--   0        0        0     1570 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/知立市.json
+-rw-r--r--   0        0        0    13207 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/碧南市.json
+-rw-r--r--   0        0        0    10699 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/稲沢市.json
+-rw-r--r--   0        0        0      751 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/蒲郡市.json
+-rw-r--r--   0        0        0     5254 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/西尾市.json
+-rw-r--r--   0        0        0       31 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/西春日井郡豊山町.json
+-rw-r--r--   0        0        0     5860 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/豊川市.json
+-rw-r--r--   0        0        0      403 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/豊明市.json
+-rw-r--r--   0        0        0     6160 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/豊橋市.json
+-rw-r--r--   0        0        0    22474 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/豊田市.json
+-rw-r--r--   0        0        0     2590 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/長久手市.json
+-rw-r--r--   0        0        0      274 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/額田郡幸田町.json
+-rw-r--r--   0        0        0     2605 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/高浜市.json
+-rw-r--r--   0        0        0      652 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/三島郡出雲崎町.json
+-rw-r--r--   0        0        0     3595 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/三条市.json
+-rw-r--r--   0        0        0    16429 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/上越市.json
+-rw-r--r--   0        0        0      310 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/中魚沼郡津南町.json
+-rw-r--r--   0        0        0     2113 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/五泉市.json
+-rw-r--r--   0        0        0     4057 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/佐渡市.json
+-rw-r--r--   0        0        0      346 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/刈羽郡刈羽村.json
+-rw-r--r--   0        0        0     1216 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/加茂市.json
+-rw-r--r--   0        0        0      439 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/北蒲原郡聖籠町.json
+-rw-r--r--   0        0        0     4642 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/十日町市.json
+-rw-r--r--   0        0        0      232 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/南蒲原郡田上町.json
+-rw-r--r--   0        0        0     1822 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/南魚沼市.json
+-rw-r--r--   0        0        0      166 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/南魚沼郡湯沢町.json
+-rw-r--r--   0        0        0     3049 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/妙高市.json
+-rw-r--r--   0        0        0     1246 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/小千谷市.json
+-rw-r--r--   0        0        0       37 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/岩船郡粟島浦村.json
+-rw-r--r--   0        0        0      754 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/岩船郡関川村.json
+-rw-r--r--   0        0        0     9991 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市中央区.json
+-rw-r--r--   0        0        0     2518 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市北区.json
+-rw-r--r--   0        0        0     1927 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市南区.json
+-rw-r--r--   0        0        0     4672 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市東区.json
+-rw-r--r--   0        0        0     5107 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市江南区.json
+-rw-r--r--   0        0        0     2224 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市秋葉区.json
+-rw-r--r--   0        0        0     4291 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市西区.json
+-rw-r--r--   0        0        0     1522 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市西蒲区.json
+-rw-r--r--   0        0        0     3712 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/新発田市.json
+-rw-r--r--   0        0        0     3106 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/村上市.json
+-rw-r--r--   0        0        0      604 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/東蒲原郡阿賀町.json
+-rw-r--r--   0        0        0     4306 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/柏崎市.json
+-rw-r--r--   0        0        0     3370 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/燕市.json
+-rw-r--r--   0        0        0     3130 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/糸魚川市.json
+-rw-r--r--   0        0        0     1192 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/胎内市.json
+-rw-r--r--   0        0        0      334 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/西蒲原郡弥彦村.json
+-rw-r--r--   0        0        0     1570 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/見附市.json
+-rw-r--r--   0        0        0    15622 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/長岡市.json
+-rw-r--r--   0        0        0     2377 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/阿賀野市.json
+-rw-r--r--   0        0        0     1408 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/魚沼市.json
+-rw-r--r--   0        0        0      754 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/あきる野市.json
+-rw-r--r--   0        0        0       58 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/三宅村.json
+-rw-r--r--   0        0        0     1195 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/三鷹市.json
+-rw-r--r--   0        0        0     5299 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/世田谷区.json
+-rw-r--r--   0        0        0     2119 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/中央区.json
+-rw-r--r--   0        0        0     1633 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/中野区.json
+-rw-r--r--   0        0        0       73 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/八丈町.json
+-rw-r--r--   0        0        0     3418 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/八王子市.json
+-rw-r--r--   0        0        0     2248 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/北区.json
+-rw-r--r--   0        0        0     2449 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/千代田区.json
+-rw-r--r--   0        0        0     2044 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/台東区.json
+-rw-r--r--   0        0        0     2578 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/品川区.json
+-rw-r--r--   0        0        0     1390 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/国分寺市.json
+-rw-r--r--   0        0        0      493 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/国立市.json
+-rw-r--r--   0        0        0     1924 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/墨田区.json
+-rw-r--r--   0        0        0     1633 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/多摩市.json
+-rw-r--r--   0        0        0      133 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/大島町.json
+-rw-r--r--   0        0        0     4411 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/大田区.json
+-rw-r--r--   0        0        0     1627 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/小平市.json
+-rw-r--r--   0        0        0       79 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/小笠原村.json
+-rw-r--r--   0        0        0      907 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/小金井市.json
+-rw-r--r--   0        0        0     2941 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/府中市.json
+-rw-r--r--   0        0        0       19 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/御蔵島村.json
+-rw-r--r--   0        0        0     1294 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/文京区.json
+-rw-r--r--   0        0        0     2689 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/新宿区.json
+-rw-r--r--   0        0        0      151 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/新島村.json
+-rw-r--r--   0        0        0     2083 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/日野市.json
+-rw-r--r--   0        0        0     1636 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/昭島市.json
+-rw-r--r--   0        0        0     2860 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/杉並区.json
+-rw-r--r--   0        0        0     1528 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/東久留米市.json
+-rw-r--r--   0        0        0     1426 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/東大和市.json
+-rw-r--r--   0        0        0     1135 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/東村山市.json
+-rw-r--r--   0        0        0     2392 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/板橋区.json
+-rw-r--r--   0        0        0     1177 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/武蔵村山市.json
+-rw-r--r--   0        0        0     1108 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/武蔵野市.json
+-rw-r--r--   0        0        0     4015 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/江戸川区.json
+-rw-r--r--   0        0        0     2830 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/江東区.json
+-rw-r--r--   0        0        0      829 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/清瀬市.json
+-rw-r--r--   0        0        0     1507 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/渋谷区.json
+-rw-r--r--   0        0        0     2296 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/港区.json
+-rw-r--r--   0        0        0      862 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/狛江市.json
+-rw-r--r--   0        0        0     3625 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/町田市.json
+-rw-r--r--   0        0        0     1768 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/目黒区.json
+-rw-r--r--   0        0        0      394 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/神津島村.json
+-rw-r--r--   0        0        0      364 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/福生市.json
+-rw-r--r--   0        0        0      406 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/稲城市.json
+-rw-r--r--   0        0        0     1579 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/立川市.json
+-rw-r--r--   0        0        0     4171 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/練馬区.json
+-rw-r--r--   0        0        0      985 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/羽村市.json
+-rw-r--r--   0        0        0     1081 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/荒川区.json
+-rw-r--r--   0        0        0     3040 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/葛飾区.json
+-rw-r--r--   0        0        0      139 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/西多摩郡奥多摩町.json
+-rw-r--r--   0        0        0       34 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/西多摩郡日の出町.json
+-rw-r--r--   0        0        0      127 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/西多摩郡檜原村.json
+-rw-r--r--   0        0        0      454 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/西多摩郡瑞穂町.json
+-rw-r--r--   0        0        0     2326 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/西東京市.json
+-rw-r--r--   0        0        0     2407 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/調布市.json
+-rw-r--r--   0        0        0     1639 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/豊島区.json
+-rw-r--r--   0        0        0     5176 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/足立区.json
+-rw-r--r--   0        0        0       22 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/青ヶ島村.json
+-rw-r--r--   0        0        0     2722 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/青梅市.json
+-rw-r--r--   0        0        0      754 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/さくら市.json
+-rw-r--r--   0        0        0      871 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/下都賀郡壬生町.json
+-rw-r--r--   0        0        0      157 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/下都賀郡野木町.json
+-rw-r--r--   0        0        0     1222 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/下野市.json
+-rw-r--r--   0        0        0     1582 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/佐野市.json
+-rw-r--r--   0        0        0      382 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/塩谷郡塩谷町.json
+-rw-r--r--   0        0        0      589 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/塩谷郡高根沢町.json
+-rw-r--r--   0        0        0     1444 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/大田原市.json
+-rw-r--r--   0        0        0     8506 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/宇都宮市.json
+-rw-r--r--   0        0        0     3421 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/小山市.json
+-rw-r--r--   0        0        0     1813 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/日光市.json
+-rw-r--r--   0        0        0     2317 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/栃木市.json
+-rw-r--r--   0        0        0      487 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/河内郡上三川町.json
+-rw-r--r--   0        0        0     1918 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/真岡市.json
+-rw-r--r--   0        0        0      472 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/矢板市.json
+-rw-r--r--   0        0        0      271 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/芳賀郡市貝町.json
+-rw-r--r--   0        0        0      343 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/芳賀郡益子町.json
+-rw-r--r--   0        0        0      376 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/芳賀郡芳賀町.json
+-rw-r--r--   0        0        0      628 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/芳賀郡茂木町.json
+-rw-r--r--   0        0        0     2344 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/足利市.json
+-rw-r--r--   0        0        0     2602 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/那須塩原市.json
+-rw-r--r--   0        0        0      628 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/那須烏山市.json
+-rw-r--r--   0        0        0      298 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/那須郡那珂川町.json
+-rw-r--r--   0        0        0      439 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/那須郡那須町.json
+-rw-r--r--   0        0        0     1810 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/鹿沼市.json
+-rw-r--r--   0        0        0     1474 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/うるま市.json
+-rw-r--r--   0        0        0      214 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/中頭郡中城村.json
+-rw-r--r--   0        0        0      172 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/中頭郡北中城村.json
+-rw-r--r--   0        0        0      292 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/中頭郡北谷町.json
+-rw-r--r--   0        0        0      100 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/中頭郡嘉手納町.json
+-rw-r--r--   0        0        0      343 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/中頭郡西原町.json
+-rw-r--r--   0        0        0      286 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/中頭郡読谷村.json
+-rw-r--r--   0        0        0       16 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/八重山郡与那国町.json
+-rw-r--r--   0        0        0      169 2021-06-17 01:45:25.853508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/八重山郡竹富町.json
+-rw-r--r--   0        0        0      898 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/南城市.json
+-rw-r--r--   0        0        0     1432 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/名護市.json
+-rw-r--r--   0        0        0      253 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/国頭郡今帰仁村.json
+-rw-r--r--   0        0        0       73 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/国頭郡伊江村.json
+-rw-r--r--   0        0        0      244 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/国頭郡国頭村.json
+-rw-r--r--   0        0        0      211 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/国頭郡大宜味村.json
+-rw-r--r--   0        0        0       52 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/国頭郡宜野座村.json
+-rw-r--r--   0        0        0      154 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/国頭郡恩納村.json
+-rw-r--r--   0        0        0      346 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/国頭郡本部町.json
+-rw-r--r--   0        0        0       76 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/国頭郡東村.json
+-rw-r--r--   0        0        0       37 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/国頭郡金武町.json
+-rw-r--r--   0        0        0     1408 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/宜野湾市.json
+-rw-r--r--   0        0        0       49 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/宮古島市.json
+-rw-r--r--   0        0        0       37 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/宮古郡多良間村.json
+-rw-r--r--   0        0        0       61 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/島尻郡与那原町.json
+-rw-r--r--   0        0        0      355 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/島尻郡久米島町.json
+-rw-r--r--   0        0        0       64 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/島尻郡伊平屋村.json
+-rw-r--r--   0        0        0       67 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/島尻郡伊是名村.json
+-rw-r--r--   0        0        0      298 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/島尻郡八重瀬町.json
+-rw-r--r--   0        0        0       43 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/島尻郡北大東村.json
+-rw-r--r--   0        0        0       70 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/島尻郡南大東村.json
+-rw-r--r--   0        0        0      154 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/島尻郡南風原町.json
+-rw-r--r--   0        0        0       67 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/島尻郡座間味村.json
+-rw-r--r--   0        0        0      433 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/島尻郡渡名喜村.json
+-rw-r--r--   0        0        0       43 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/島尻郡渡嘉敷村.json
+-rw-r--r--   0        0        0       28 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/島尻郡粟国村.json
+-rw-r--r--   0        0        0     2641 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/沖縄市.json
+-rw-r--r--   0        0        0     1393 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/浦添市.json
+-rw-r--r--   0        0        0      373 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/石垣市.json
+-rw-r--r--   0        0        0      655 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/糸満市.json
+-rw-r--r--   0        0        0      406 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/豊見城市.json
+-rw-r--r--   0        0        0     4318 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/那覇市.json
+-rw-r--r--   0        0        0     9202 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/大津市.json
+-rw-r--r--   0        0        0     1021 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/守山市.json
+-rw-r--r--   0        0        0     1909 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/彦根市.json
+-rw-r--r--   0        0        0      415 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/愛知郡愛荘町.json
+-rw-r--r--   0        0        0     3679 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/東近江市.json
+-rw-r--r--   0        0        0     1291 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/栗東市.json
+-rw-r--r--   0        0        0     2545 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/湖南市.json
+-rw-r--r--   0        0        0      607 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/犬上郡多賀町.json
+-rw-r--r--   0        0        0      193 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/犬上郡甲良町.json
+-rw-r--r--   0        0        0      256 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/犬上郡豊郷町.json
+-rw-r--r--   0        0        0     3631 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/甲賀市.json
+-rw-r--r--   0        0        0      967 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/米原市.json
+-rw-r--r--   0        0        0     2575 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/草津市.json
+-rw-r--r--   0        0        0     1060 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/蒲生郡日野町.json
+-rw-r--r--   0        0        0      358 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/蒲生郡竜王町.json
+-rw-r--r--   0        0        0     2947 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/近江八幡市.json
+-rw-r--r--   0        0        0      652 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/野洲市.json
+-rw-r--r--   0        0        0     4744 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/長浜市.json
+-rw-r--r--   0        0        0     3100 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/高島市.json
+-rw-r--r--   0        0        0      301 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/上天草市.json
+-rw-r--r--   0        0        0      148 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/上益城郡嘉島町.json
+-rw-r--r--   0        0        0      946 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/上益城郡山都町.json
+-rw-r--r--   0        0        0      196 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/上益城郡御船町.json
+-rw-r--r--   0        0        0      478 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/上益城郡甲佐町.json
+-rw-r--r--   0        0        0      334 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/上益城郡益城町.json
+-rw-r--r--   0        0        0      463 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/下益城郡美里町.json
+-rw-r--r--   0        0        0     1039 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/人吉市.json
+-rw-r--r--   0        0        0     3247 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/八代市.json
+-rw-r--r--   0        0        0      172 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/八代郡氷川町.json
+-rw-r--r--   0        0        0      106 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/合志市.json
+-rw-r--r--   0        0        0     1687 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/天草市.json
+-rw-r--r--   0        0        0       88 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/天草郡苓北町.json
+-rw-r--r--   0        0        0      817 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/宇土市.json
+-rw-r--r--   0        0        0     1423 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/宇城市.json
+-rw-r--r--   0        0        0     1315 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/山鹿市.json
+-rw-r--r--   0        0        0     1405 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/水俣市.json
+-rw-r--r--   0        0        0     3601 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/熊本市中央区.json
+-rw-r--r--   0        0        0     3277 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/熊本市北区.json
+-rw-r--r--   0        0        0     3766 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/熊本市南区.json
+-rw-r--r--   0        0        0     3766 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/熊本市東区.json
+-rw-r--r--   0        0        0     2386 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/熊本市西区.json
+-rw-r--r--   0        0        0      997 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/玉名市.json
+-rw-r--r--   0        0        0      319 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/玉名郡南関町.json
+-rw-r--r--   0        0        0      394 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/玉名郡和水町.json
+-rw-r--r--   0        0        0      160 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/玉名郡玉東町.json
+-rw-r--r--   0        0        0      193 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/玉名郡長洲町.json
+-rw-r--r--   0        0        0      151 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/球磨郡あさぎり町.json
+-rw-r--r--   0        0        0       19 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/球磨郡五木村.json
+-rw-r--r--   0        0        0       82 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/球磨郡多良木町.json
+-rw-r--r--   0        0        0       31 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/球磨郡山江村.json
+-rw-r--r--   0        0        0       46 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/球磨郡水上村.json
+-rw-r--r--   0        0        0       79 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/球磨郡球磨村.json
+-rw-r--r--   0        0        0       82 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/球磨郡相良村.json
+-rw-r--r--   0        0        0      100 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/球磨郡錦町.json
+-rw-r--r--   0        0        0      904 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/荒尾市.json
+-rw-r--r--   0        0        0     1012 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/菊池市.json
+-rw-r--r--   0        0        0      409 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/菊池郡大津町.json
+-rw-r--r--   0        0        0      649 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/菊池郡菊陽町.json
+-rw-r--r--   0        0        0       85 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/葦北郡津奈木町.json
+-rw-r--r--   0        0        0      724 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/葦北郡芦北町.json
+-rw-r--r--   0        0        0      592 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/阿蘇市.json
+-rw-r--r--   0        0        0       52 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/阿蘇郡南小国町.json
+-rw-r--r--   0        0        0      166 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/阿蘇郡南阿蘇村.json
+-rw-r--r--   0        0        0       91 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/阿蘇郡小国町.json
+-rw-r--r--   0        0        0       76 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/阿蘇郡産山村.json
+-rw-r--r--   0        0        0       76 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/阿蘇郡西原村.json
+-rw-r--r--   0        0        0      217 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/阿蘇郡高森町.json
+-rw-r--r--   0        0        0      670 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/かほく市.json
+-rw-r--r--   0        0        0     3178 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/七尾市.json
+-rw-r--r--   0        0        0     4507 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/加賀市.json
+-rw-r--r--   0        0        0     4255 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/小松市.json
+-rw-r--r--   0        0        0      967 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/河北郡内灘町.json
+-rw-r--r--   0        0        0     1432 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/河北郡津幡町.json
+-rw-r--r--   0        0        0     1291 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/珠洲市.json
+-rw-r--r--   0        0        0     5479 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/白山市.json
+-rw-r--r--   0        0        0      928 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/羽咋市.json
+-rw-r--r--   0        0        0      508 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/羽咋郡宝達志水町.json
+-rw-r--r--   0        0        0     1213 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/羽咋郡志賀町.json
+-rw-r--r--   0        0        0     1570 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/能美市.json
+-rw-r--r--   0        0        0      166 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/能美郡川北町.json
+-rw-r--r--   0        0        0     3628 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/輪島市.json
+-rw-r--r--   0        0        0     1843 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/野々市市.json
+-rw-r--r--   0        0        0    15160 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/金沢市.json
+-rw-r--r--   0        0        0      790 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/鳳珠郡穴水町.json
+-rw-r--r--   0        0        0     1357 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/鳳珠郡能登町.json
+-rw-r--r--   0        0        0      493 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/鹿島郡中能登町.json
+-rw-r--r--   0        0        0      529 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/三浦市.json
+-rw-r--r--   0        0        0       64 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/三浦郡葉山町.json
+-rw-r--r--   0        0        0      289 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/中郡二宮町.json
+-rw-r--r--   0        0        0      301 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/中郡大磯町.json
+-rw-r--r--   0        0        0     1018 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/伊勢原市.json
+-rw-r--r--   0        0        0      268 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/南足柄市.json
+-rw-r--r--   0        0        0     2359 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/厚木市.json
+-rw-r--r--   0        0        0     2452 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/大和市.json
+-rw-r--r--   0        0        0     1993 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/小田原市.json
+-rw-r--r--   0        0        0     1444 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市中原区.json
+-rw-r--r--   0        0        0     1927 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市多摩区.json
+-rw-r--r--   0        0        0     1480 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市宮前区.json
+-rw-r--r--   0        0        0     2356 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市川崎区.json
+-rw-r--r--   0        0        0     1165 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市幸区.json
+-rw-r--r--   0        0        0     1258 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市高津区.json
+-rw-r--r--   0        0        0     2350 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市麻生区.json
+-rw-r--r--   0        0        0     2314 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/平塚市.json
+-rw-r--r--   0        0        0     1387 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/座間市.json
+-rw-r--r--   0        0        0      172 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/愛甲郡愛川町.json
+-rw-r--r--   0        0        0       25 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/愛甲郡清川村.json
+-rw-r--r--   0        0        0     4939 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市中区.json
+-rw-r--r--   0        0        0     1060 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市保土ケ谷区.json
+-rw-r--r--   0        0        0     3034 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市南区.json
+-rw-r--r--   0        0        0      700 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市戸塚区.json
+-rw-r--r--   0        0        0     1246 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市旭区.json
+-rw-r--r--   0        0        0      925 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市栄区.json
+-rw-r--r--   0        0        0     1246 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市泉区.json
+-rw-r--r--   0        0        0     1999 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市港北区.json
+-rw-r--r--   0        0        0     1696 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市港南区.json
+-rw-r--r--   0        0        0     1078 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市瀬谷区.json
+-rw-r--r--   0        0        0     1261 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市磯子区.json
+-rw-r--r--   0        0        0     2194 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市神奈川区.json
+-rw-r--r--   0        0        0     1228 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市緑区.json
+-rw-r--r--   0        0        0     1309 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市西区.json
+-rw-r--r--   0        0        0     1783 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市都筑区.json
+-rw-r--r--   0        0        0     1873 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市金沢区.json
+-rw-r--r--   0        0        0     1516 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市青葉区.json
+-rw-r--r--   0        0        0     2500 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市鶴見区.json
+-rw-r--r--   0        0        0     6814 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横須賀市.json
+-rw-r--r--   0        0        0     1951 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/海老名市.json
+-rw-r--r--   0        0        0     3028 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/相模原市中央区.json
+-rw-r--r--   0        0        0     2488 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/相模原市南区.json
+-rw-r--r--   0        0        0     1588 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/相模原市緑区.json
+-rw-r--r--   0        0        0     1543 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/秦野市.json
+-rw-r--r--   0        0        0     2443 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/綾瀬市.json
+-rw-r--r--   0        0        0     2017 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/茅ヶ崎市.json
+-rw-r--r--   0        0        0     4000 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/藤沢市.json
+-rw-r--r--   0        0        0      148 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/足柄上郡中井町.json
+-rw-r--r--   0        0        0       85 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/足柄上郡大井町.json
+-rw-r--r--   0        0        0      148 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/足柄上郡山北町.json
+-rw-r--r--   0        0        0       46 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/足柄上郡松田町.json
+-rw-r--r--   0        0        0      190 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/足柄上郡開成町.json
+-rw-r--r--   0        0        0      265 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/足柄下郡湯河原町.json
+-rw-r--r--   0        0        0       16 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/足柄下郡真鶴町.json
+-rw-r--r--   0        0        0      190 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/足柄下郡箱根町.json
+-rw-r--r--   0        0        0      937 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/逗子市.json
+-rw-r--r--   0        0        0     2779 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/鎌倉市.json
+-rw-r--r--   0        0        0      562 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/高座郡寒川町.json
+-rw-r--r--   0        0        0     1576 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/あわら市.json
+-rw-r--r--   0        0        0      772 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/三方上中郡若狭町.json
+-rw-r--r--   0        0        0      301 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/三方郡美浜町.json
+-rw-r--r--   0        0        0     1054 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/丹生郡越前町.json
+-rw-r--r--   0        0        0      469 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/今立郡池田町.json
+-rw-r--r--   0        0        0     2272 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/勝山市.json
+-rw-r--r--   0        0        0      568 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/南条郡南越前町.json
+-rw-r--r--   0        0        0     1474 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/吉田郡永平寺町.json
+-rw-r--r--   0        0        0     8296 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/坂井市.json
+-rw-r--r--   0        0        0     2278 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/大野市.json
+-rw-r--r--   0        0        0      604 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/大飯郡おおい町.json
+-rw-r--r--   0        0        0      562 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/大飯郡高浜町.json
+-rw-r--r--   0        0        0     1816 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/小浜市.json
+-rw-r--r--   0        0        0     1942 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/敦賀市.json
+-rw-r--r--   0        0        0    11728 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/福井市.json
+-rw-r--r--   0        0        0     3541 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/越前市.json
+-rw-r--r--   0        0        0     2533 2021-06-17 01:45:25.857508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/鯖江市.json
+-rw-r--r--   0        0        0      562 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/うきは市.json
+-rw-r--r--   0        0        0      949 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/みやま市.json
+-rw-r--r--   0        0        0      244 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/三井郡大刀洗町.json
+-rw-r--r--   0        0        0      310 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/三潴郡大木町.json
+-rw-r--r--   0        0        0     1447 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/中間市.json
+-rw-r--r--   0        0        0     4222 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/久留米市.json
+-rw-r--r--   0        0        0      796 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/京都郡みやこ町.json
+-rw-r--r--   0        0        0      970 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/京都郡苅田町.json
+-rw-r--r--   0        0        0      964 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/八女市.json
+-rw-r--r--   0        0        0      199 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/八女郡広川町.json
+-rw-r--r--   0        0        0     2272 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市八幡東区.json
+-rw-r--r--   0        0        0     7804 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市八幡西区.json
+-rw-r--r--   0        0        0     4000 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市小倉北区.json
+-rw-r--r--   0        0        0     7045 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市小倉南区.json
+-rw-r--r--   0        0        0     1501 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市戸畑区.json
+-rw-r--r--   0        0        0     2770 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市若松区.json
+-rw-r--r--   0        0        0     3481 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市門司区.json
+-rw-r--r--   0        0        0     1201 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/古賀市.json
+-rw-r--r--   0        0        0      142 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/嘉穂郡桂川町.json
+-rw-r--r--   0        0        0      367 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/嘉麻市.json
+-rw-r--r--   0        0        0      547 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/大川市.json
+-rw-r--r--   0        0        0     4135 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/大牟田市.json
+-rw-r--r--   0        0        0     2743 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/大野城市.json
+-rw-r--r--   0        0        0     2239 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/太宰府市.json
+-rw-r--r--   0        0        0     3106 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/宗像市.json
+-rw-r--r--   0        0        0      313 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/宮若市.json
+-rw-r--r--   0        0        0      829 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/小郡市.json
+-rw-r--r--   0        0        0     5146 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/春日市.json
+-rw-r--r--   0        0        0     1093 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/朝倉市.json
+-rw-r--r--   0        0        0       73 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/朝倉郡東峰村.json
+-rw-r--r--   0        0        0      355 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/朝倉郡筑前町.json
+-rw-r--r--   0        0        0     1450 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/柳川市.json
+-rw-r--r--   0        0        0      352 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/田川市.json
+-rw-r--r--   0        0        0       37 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/田川郡大任町.json
+-rw-r--r--   0        0        0       64 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/田川郡川崎町.json
+-rw-r--r--   0        0        0      124 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/田川郡添田町.json
+-rw-r--r--   0        0        0       64 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/田川郡福智町.json
+-rw-r--r--   0        0        0       19 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/田川郡糸田町.json
+-rw-r--r--   0        0        0       37 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/田川郡赤村.json
+-rw-r--r--   0        0        0       97 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/田川郡香春町.json
+-rw-r--r--   0        0        0      529 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/直方市.json
+-rw-r--r--   0        0        0     2221 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市中央区.json
+-rw-r--r--   0        0        0     2962 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市南区.json
+-rw-r--r--   0        0        0     4048 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市博多区.json
+-rw-r--r--   0        0        0     1726 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市城南区.json
+-rw-r--r--   0        0        0     3064 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市早良区.json
+-rw-r--r--   0        0        0     4573 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市東区.json
+-rw-r--r--   0        0        0     2776 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市西区.json
+-rw-r--r--   0        0        0     1942 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/福津市.json
+-rw-r--r--   0        0        0      643 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/筑後市.json
+-rw-r--r--   0        0        0     2983 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/筑紫野市.json
+-rw-r--r--   0        0        0      304 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/築上郡上毛町.json
+-rw-r--r--   0        0        0      154 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/築上郡吉富町.json
+-rw-r--r--   0        0        0      673 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/築上郡築上町.json
+-rw-r--r--   0        0        0       46 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/糟屋郡久山町.json
+-rw-r--r--   0        0        0     1594 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/糟屋郡宇美町.json
+-rw-r--r--   0        0        0     1303 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/糟屋郡志免町.json
+-rw-r--r--   0        0        0     1165 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/糟屋郡新宮町.json
+-rw-r--r--   0        0        0      169 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/糟屋郡篠栗町.json
+-rw-r--r--   0        0        0      994 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/糟屋郡粕屋町.json
+-rw-r--r--   0        0        0       94 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/糟屋郡須恵町.json
+-rw-r--r--   0        0        0     2365 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/糸島市.json
+-rw-r--r--   0        0        0     2116 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/行橋市.json
+-rw-r--r--   0        0        0      877 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/豊前市.json
+-rw-r--r--   0        0        0     1381 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/遠賀郡岡垣町.json
+-rw-r--r--   0        0        0     1339 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/遠賀郡水巻町.json
+-rw-r--r--   0        0        0      181 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/遠賀郡芦屋町.json
+-rw-r--r--   0        0        0      643 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/遠賀郡遠賀町.json
+-rw-r--r--   0        0        0     1915 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/那珂川市.json
+-rw-r--r--   0        0        0       97 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/鞍手郡小竹町.json
+-rw-r--r--   0        0        0      238 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/鞍手郡鞍手町.json
+-rw-r--r--   0        0        0      994 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/飯塚市.json
+-rw-r--r--   0        0        0     7375 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/いわき市.json
+-rw-r--r--   0        0        0     4162 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/二本松市.json
+-rw-r--r--   0        0        0     1816 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/伊達市.json
+-rw-r--r--   0        0        0      328 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/伊達郡国見町.json
+-rw-r--r--   0        0        0     1078 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/伊達郡川俣町.json
+-rw-r--r--   0        0        0     1072 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/伊達郡桑折町.json
+-rw-r--r--   0        0        0     5080 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/会津若松市.json
+-rw-r--r--   0        0        0      352 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/南会津郡下郷町.json
+-rw-r--r--   0        0        0      739 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/南会津郡南会津町.json
+-rw-r--r--   0        0        0      373 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/南会津郡只見町.json
+-rw-r--r--   0        0        0      256 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/南会津郡檜枝岐村.json
+-rw-r--r--   0        0        0     4357 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/南相馬市.json
+-rw-r--r--   0        0        0      307 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/双葉郡双葉町.json
+-rw-r--r--   0        0        0      130 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/双葉郡大熊町.json
+-rw-r--r--   0        0        0      478 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/双葉郡富岡町.json
+-rw-r--r--   0        0        0       37 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/双葉郡川内村.json
+-rw-r--r--   0        0        0      214 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/双葉郡広野町.json
+-rw-r--r--   0        0        0      184 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/双葉郡楢葉町.json
+-rw-r--r--   0        0        0      526 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/双葉郡浪江町.json
+-rw-r--r--   0        0        0       64 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/双葉郡葛尾村.json
+-rw-r--r--   0        0        0     3970 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/喜多方市.json
+-rw-r--r--   0        0        0      199 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/大沼郡三島町.json
+-rw-r--r--   0        0        0     2497 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/大沼郡会津美里町.json
+-rw-r--r--   0        0        0      151 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/大沼郡昭和村.json
+-rw-r--r--   0        0        0      280 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/大沼郡金山町.json
+-rw-r--r--   0        0        0       19 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/安達郡大玉村.json
+-rw-r--r--   0        0        0      211 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/岩瀬郡天栄村.json
+-rw-r--r--   0        0        0      556 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/岩瀬郡鏡石町.json
+-rw-r--r--   0        0        0      121 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/本宮市.json
+-rw-r--r--   0        0        0      394 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/東白川郡塙町.json
+-rw-r--r--   0        0        0      568 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/東白川郡棚倉町.json
+-rw-r--r--   0        0        0      247 2021-06-17 01:45:25.861508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/東白川郡矢祭町.json
+-rw-r--r--   0        0        0      145 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/東白川郡鮫川村.json
+-rw-r--r--   0        0        0     1837 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/河沼郡会津坂下町.json
+-rw-r--r--   0        0        0      331 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/河沼郡柳津町.json
+-rw-r--r--   0        0        0      184 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/河沼郡湯川村.json
+-rw-r--r--   0        0        0     1063 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/田村市.json
+-rw-r--r--   0        0        0     1531 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/田村郡三春町.json
+-rw-r--r--   0        0        0      307 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/田村郡小野町.json
+-rw-r--r--   0        0        0     3292 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/白河市.json
+-rw-r--r--   0        0        0      709 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/相馬市.json
+-rw-r--r--   0        0        0      115 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/相馬郡新地町.json
+-rw-r--r--   0        0        0      190 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/相馬郡飯舘村.json
+-rw-r--r--   0        0        0      124 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/石川郡古殿町.json
+-rw-r--r--   0        0        0      214 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/石川郡平田村.json
+-rw-r--r--   0        0        0      271 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/石川郡浅川町.json
+-rw-r--r--   0        0        0      196 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/石川郡玉川村.json
+-rw-r--r--   0        0        0     1033 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/石川郡石川町.json
+-rw-r--r--   0        0        0     2503 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/福島市.json
+-rw-r--r--   0        0        0       76 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/耶麻郡北塩原村.json
+-rw-r--r--   0        0        0     3697 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/耶麻郡猪苗代町.json
+-rw-r--r--   0        0        0       61 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/耶麻郡磐梯町.json
+-rw-r--r--   0        0        0      367 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/耶麻郡西会津町.json
+-rw-r--r--   0        0        0       97 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/西白河郡中島村.json
+-rw-r--r--   0        0        0       85 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/西白河郡泉崎村.json
+-rw-r--r--   0        0        0      958 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/西白河郡矢吹町.json
+-rw-r--r--   0        0        0      328 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/西白河郡西郷村.json
+-rw-r--r--   0        0        0     7645 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/郡山市.json
+-rw-r--r--   0        0        0     1555 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/須賀川市.json
+-rw-r--r--   0        0        0      445 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/にかほ市.json
+-rw-r--r--   0        0        0      583 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/仙北市.json
+-rw-r--r--   0        0        0      262 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/仙北郡美郷町.json
+-rw-r--r--   0        0        0      865 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/北秋田市.json
+-rw-r--r--   0        0        0       91 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/北秋田郡上小阿仁村.json
+-rw-r--r--   0        0        0      562 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/南秋田郡五城目町.json
+-rw-r--r--   0        0        0      148 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/南秋田郡井川町.json
+-rw-r--r--   0        0        0      364 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/南秋田郡八郎潟町.json
+-rw-r--r--   0        0        0      337 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/南秋田郡大潟村.json
+-rw-r--r--   0        0        0     1795 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/大仙市.json
+-rw-r--r--   0        0        0     2323 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/大館市.json
+-rw-r--r--   0        0        0      178 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/山本郡三種町.json
+-rw-r--r--   0        0        0      184 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/山本郡八峰町.json
+-rw-r--r--   0        0        0       46 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/山本郡藤里町.json
+-rw-r--r--   0        0        0     2506 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/横手市.json
+-rw-r--r--   0        0        0     2611 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/湯沢市.json
+-rw-r--r--   0        0        0      289 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/潟上市.json
+-rw-r--r--   0        0        0     2956 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/由利本荘市.json
+-rw-r--r--   0        0        0      838 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/男鹿市.json
+-rw-r--r--   0        0        0    10048 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/秋田市.json
+-rw-r--r--   0        0        0     2296 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/能代市.json
+-rw-r--r--   0        0        0       34 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/雄勝郡東成瀬村.json
+-rw-r--r--   0        0        0     1447 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/雄勝郡羽後町.json
+-rw-r--r--   0        0        0      202 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/鹿角市.json
+-rw-r--r--   0        0        0       67 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/鹿角郡小坂町.json
+-rw-r--r--   0        0        0      424 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/みどり市.json
+-rw-r--r--   0        0        0     1906 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/伊勢崎市.json
+-rw-r--r--   0        0        0      406 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/佐波郡玉村町.json
+-rw-r--r--   0        0        0      442 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/利根郡みなかみ町.json
+-rw-r--r--   0        0        0      145 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/利根郡川場村.json
+-rw-r--r--   0        0        0      115 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/利根郡昭和村.json
+-rw-r--r--   0        0        0      220 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/利根郡片品村.json
+-rw-r--r--   0        0        0     4900 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/前橋市.json
+-rw-r--r--   0        0        0      130 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/北群馬郡吉岡町.json
+-rw-r--r--   0        0        0       85 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/北群馬郡榛東村.json
+-rw-r--r--   0        0        0      421 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/吾妻郡中之条町.json
+-rw-r--r--   0        0        0      169 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/吾妻郡嬬恋村.json
+-rw-r--r--   0        0        0      355 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/吾妻郡東吾妻町.json
+-rw-r--r--   0        0        0       31 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/吾妻郡草津町.json
+-rw-r--r--   0        0        0      184 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/吾妻郡長野原町.json
+-rw-r--r--   0        0        0       31 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/吾妻郡高山村.json
+-rw-r--r--   0        0        0      109 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/多野郡上野村.json
+-rw-r--r--   0        0        0      229 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/多野郡神流町.json
+-rw-r--r--   0        0        0     2131 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/太田市.json
+-rw-r--r--   0        0        0     1096 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/安中市.json
+-rw-r--r--   0        0        0      637 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/富岡市.json
+-rw-r--r--   0        0        0     2134 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/桐生市.json
+-rw-r--r--   0        0        0     1210 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/沼田市.json
+-rw-r--r--   0        0        0      832 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/渋川市.json
+-rw-r--r--   0        0        0      310 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/甘楽郡下仁田町.json
+-rw-r--r--   0        0        0      190 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/甘楽郡南牧村.json
+-rw-r--r--   0        0        0      196 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/甘楽郡甘楽町.json
+-rw-r--r--   0        0        0      463 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/藤岡市.json
+-rw-r--r--   0        0        0      220 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/邑楽郡千代田町.json
+-rw-r--r--   0        0        0      955 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/邑楽郡大泉町.json
+-rw-r--r--   0        0        0      166 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/邑楽郡明和町.json
+-rw-r--r--   0        0        0      400 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/邑楽郡板倉町.json
+-rw-r--r--   0        0        0      187 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/邑楽郡邑楽町.json
+-rw-r--r--   0        0        0     1093 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/館林市.json
+-rw-r--r--   0        0        0     3979 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/高崎市.json
+-rw-r--r--   0        0        0      769 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/かすみがうら市.json
+-rw-r--r--   0        0        0     1345 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/つくばみらい市.json
+-rw-r--r--   0        0        0     3967 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/つくば市.json
+-rw-r--r--   0        0        0     2335 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/ひたちなか市.json
+-rw-r--r--   0        0        0      958 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/下妻市.json
+-rw-r--r--   0        0        0      649 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/久慈郡大子町.json
+-rw-r--r--   0        0        0      556 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/北相馬郡利根町.json
+-rw-r--r--   0        0        0     1564 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/北茨城市.json
+-rw-r--r--   0        0        0     2002 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/取手市.json
+-rw-r--r--   0        0        0     1339 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/古河市.json
+-rw-r--r--   0        0        0     3310 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/土浦市.json
+-rw-r--r--   0        0        0      586 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/坂東市.json
+-rw-r--r--   0        0        0     1495 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/守谷市.json
+-rw-r--r--   0        0        0      544 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/小美玉市.json
+-rw-r--r--   0        0        0     1336 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/常総市.json
+-rw-r--r--   0        0        0      853 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/常陸大宮市.json
+-rw-r--r--   0        0        0     1327 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/常陸太田市.json
+-rw-r--r--   0        0        0     5428 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/日立市.json
+-rw-r--r--   0        0        0      559 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/東茨城郡城里町.json
+-rw-r--r--   0        0        0      112 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/東茨城郡大洗町.json
+-rw-r--r--   0        0        0      694 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/東茨城郡茨城町.json
+-rw-r--r--   0        0        0     1321 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/桜川市.json
+-rw-r--r--   0        0        0     3763 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/水戸市.json
+-rw-r--r--   0        0        0      622 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/潮来市.json
+-rw-r--r--   0        0        0     1285 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/牛久市.json
+-rw-r--r--   0        0        0      298 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/猿島郡五霞町.json
+-rw-r--r--   0        0        0      448 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/猿島郡境町.json
+-rw-r--r--   0        0        0     1906 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/石岡市.json
+-rw-r--r--   0        0        0     1894 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/神栖市.json
+-rw-r--r--   0        0        0     1015 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/稲敷市.json
+-rw-r--r--   0        0        0      301 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/稲敷郡河内町.json
+-rw-r--r--   0        0        0      553 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/稲敷郡美浦村.json
+-rw-r--r--   0        0        0     1030 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/稲敷郡阿見町.json
+-rw-r--r--   0        0        0      874 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/笠間市.json
+-rw-r--r--   0        0        0     1846 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/筑西市.json
+-rw-r--r--   0        0        0      940 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/結城市.json
+-rw-r--r--   0        0        0      778 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/結城郡八千代町.json
+-rw-r--r--   0        0        0      547 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/行方市.json
+-rw-r--r--   0        0        0      433 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/那珂市.json
+-rw-r--r--   0        0        0      604 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/那珂郡東海村.json
+-rw-r--r--   0        0        0      664 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/鉾田市.json
+-rw-r--r--   0        0        0      745 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/高萩市.json
+-rw-r--r--   0        0        0     1528 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/鹿嶋市.json
+-rw-r--r--   0        0        0     2146 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/龍ヶ崎市.json
+-rw-r--r--   0        0        0     1717 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/五島市.json
+-rw-r--r--   0        0        0     4723 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/佐世保市.json
+-rw-r--r--   0        0        0      316 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/北松浦郡佐々町.json
+-rw-r--r--   0        0        0      163 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/北松浦郡小値賀町.json
+-rw-r--r--   0        0        0      811 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/南島原市.json
+-rw-r--r--   0        0        0      547 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/南松浦郡新上五島町.json
+-rw-r--r--   0        0        0     2710 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/壱岐市.json
+-rw-r--r--   0        0        0     1567 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/大村市.json
+-rw-r--r--   0        0        0     2341 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/対馬市.json
+-rw-r--r--   0        0        0     2209 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/島原市.json
+-rw-r--r--   0        0        0     1549 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/平戸市.json
+-rw-r--r--   0        0        0      214 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/東彼杵郡川棚町.json
+-rw-r--r--   0        0        0      304 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/東彼杵郡東彼杵町.json
+-rw-r--r--   0        0        0      256 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/東彼杵郡波佐見町.json
+-rw-r--r--   0        0        0      412 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/松浦市.json
+-rw-r--r--   0        0        0      115 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/西彼杵郡時津町.json
+-rw-r--r--   0        0        0      187 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/西彼杵郡長与町.json
+-rw-r--r--   0        0        0     1285 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/西海市.json
+-rw-r--r--   0        0        0     2734 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/諫早市.json
+-rw-r--r--   0        0        0     7453 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/長崎市.json
+-rw-r--r--   0        0        0     1429 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/雲仙市.json
+-rw-r--r--   0        0        0       37 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/上伊那郡中川村.json
+-rw-r--r--   0        0        0       22 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/上伊那郡南箕輪村.json
+-rw-r--r--   0        0        0      145 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/上伊那郡宮田村.json
+-rw-r--r--   0        0        0       88 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/上伊那郡箕輪町.json
+-rw-r--r--   0        0        0      226 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/上伊那郡辰野町.json
+-rw-r--r--   0        0        0       52 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/上伊那郡飯島町.json
+-rw-r--r--   0        0        0      154 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/上水内郡信濃町.json
+-rw-r--r--   0        0        0       67 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/上水内郡小川村.json
+-rw-r--r--   0        0        0      286 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/上水内郡飯綱町.json
+-rw-r--r--   0        0        0     1552 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/上田市.json
+-rw-r--r--   0        0        0      157 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/上高井郡小布施町.json
+-rw-r--r--   0        0        0       61 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/上高井郡高山村.json
+-rw-r--r--   0        0        0       19 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡下條村.json
+-rw-r--r--   0        0        0      259 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡喬木村.json
+-rw-r--r--   0        0        0       61 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡売木村.json
+-rw-r--r--   0        0        0       34 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡大鹿村.json
+-rw-r--r--   0        0        0       28 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡天龍村.json
+-rw-r--r--   0        0        0       88 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡平谷村.json
+-rw-r--r--   0        0        0       43 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡松川町.json
+-rw-r--r--   0        0        0      328 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡根羽村.json
+-rw-r--r--   0        0        0      196 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡泰阜村.json
+-rw-r--r--   0        0        0       31 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡豊丘村.json
+-rw-r--r--   0        0        0       64 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡阿南町.json
+-rw-r--r--   0        0        0       64 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡阿智村.json
+-rw-r--r--   0        0        0       73 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/下伊那郡高森町.json
+-rw-r--r--   0        0        0       43 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/下水内郡栄村.json
+-rw-r--r--   0        0        0       79 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/下高井郡山ノ内町.json
+-rw-r--r--   0        0        0       49 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/下高井郡木島平村.json
+-rw-r--r--   0        0        0      112 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/下高井郡野沢温泉村.json
+-rw-r--r--   0        0        0      817 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/中野市.json
+-rw-r--r--   0        0        0      709 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/伊那市.json
+-rw-r--r--   0        0        0      793 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/佐久市.json
+-rw-r--r--   0        0        0      127 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/北佐久郡御代田町.json
+-rw-r--r--   0        0        0      148 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/北佐久郡立科町.json
+-rw-r--r--   0        0        0      136 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/北佐久郡軽井沢町.json
+-rw-r--r--   0        0        0       67 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/北安曇郡小谷村.json
+-rw-r--r--   0        0        0       40 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/北安曇郡松川村.json
+-rw-r--r--   0        0        0       76 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/北安曇郡池田町.json
+-rw-r--r--   0        0        0       31 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/北安曇郡白馬村.json
+-rw-r--r--   0        0        0      742 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/千曲市.json
+-rw-r--r--   0        0        0      169 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/南佐久郡佐久穂町.json
+-rw-r--r--   0        0        0      148 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/南佐久郡北相木村.json
+-rw-r--r--   0        0        0       97 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/南佐久郡南牧村.json
+-rw-r--r--   0        0        0     3253 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/南佐久郡南相木村.json
+-rw-r--r--   0        0        0       82 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/南佐久郡小海町.json
+-rw-r--r--   0        0        0      127 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/南佐久郡川上村.json
+-rw-r--r--   0        0        0       97 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/埴科郡坂城町.json
+-rw-r--r--   0        0        0      712 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/塩尻市.json
+-rw-r--r--   0        0        0       64 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/大町市.json
+-rw-r--r--   0        0        0      292 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/安曇野市.json
+-rw-r--r--   0        0        0       40 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/小県郡長和町.json
+-rw-r--r--   0        0        0      109 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/小県郡青木村.json
+-rw-r--r--   0        0        0     1474 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/小諸市.json
+-rw-r--r--   0        0        0     2032 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/岡谷市.json
+-rw-r--r--   0        0        0      373 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/木曽郡上松町.json
+-rw-r--r--   0        0        0       28 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/木曽郡南木曽町.json
+-rw-r--r--   0        0        0       58 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/木曽郡大桑村.json
+-rw-r--r--   0        0        0       79 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/木曽郡木曽町.json
+-rw-r--r--   0        0        0       46 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/木曽郡木祖村.json
+-rw-r--r--   0        0        0      184 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/木曽郡王滝村.json
+-rw-r--r--   0        0        0      199 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/東御市.json
+-rw-r--r--   0        0        0       70 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/東筑摩郡山形村.json
+-rw-r--r--   0        0        0       67 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/東筑摩郡朝日村.json
+-rw-r--r--   0        0        0       85 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/東筑摩郡生坂村.json
+-rw-r--r--   0        0        0       61 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/東筑摩郡筑北村.json
+-rw-r--r--   0        0        0       13 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/東筑摩郡麻績村.json
+-rw-r--r--   0        0        0     3763 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/松本市.json
+-rw-r--r--   0        0        0      193 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/茅野市.json
+-rw-r--r--   0        0        0      811 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/諏訪市.json
+-rw-r--r--   0        0        0      856 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/諏訪郡下諏訪町.json
+-rw-r--r--   0        0        0      166 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/諏訪郡原村.json
+-rw-r--r--   0        0        0       46 2021-06-17 01:45:25.865507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/諏訪郡富士見町.json
+-rw-r--r--   0        0        0     5533 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/長野市.json
+-rw-r--r--   0        0        0      790 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/須坂市.json
+-rw-r--r--   0        0        0      436 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/飯山市.json
+-rw-r--r--   0        0        0     3259 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/飯田市.json
+-rw-r--r--   0        0        0      208 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/駒ヶ根市.json
+-rw-r--r--   0        0        0     1516 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/つがる市.json
+-rw-r--r--   0        0        0     1003 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/むつ市.json
+-rw-r--r--   0        0        0      292 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/三戸郡三戸町.json
+-rw-r--r--   0        0        0     2227 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/三戸郡五戸町.json
+-rw-r--r--   0        0        0      430 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/三戸郡南部町.json
+-rw-r--r--   0        0        0       31 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/三戸郡新郷村.json
+-rw-r--r--   0        0        0      145 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/三戸郡田子町.json
+-rw-r--r--   0        0        0      451 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/三戸郡階上町.json
+-rw-r--r--   0        0        0     3400 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/三沢市.json
+-rw-r--r--   0        0        0     2221 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/上北郡おいらせ町.json
+-rw-r--r--   0        0        0     3532 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/上北郡七戸町.json
+-rw-r--r--   0        0        0       88 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/上北郡六ヶ所村.json
+-rw-r--r--   0        0        0      313 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/上北郡六戸町.json
+-rw-r--r--   0        0        0     3058 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/上北郡東北町.json
+-rw-r--r--   0        0        0      817 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/上北郡横浜町.json
+-rw-r--r--   0        0        0     1543 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/上北郡野辺地町.json
+-rw-r--r--   0        0        0       31 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/下北郡佐井村.json
+-rw-r--r--   0        0        0       31 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/下北郡大間町.json
+-rw-r--r--   0        0        0      196 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/下北郡東通村.json
+-rw-r--r--   0        0        0       52 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/下北郡風間浦村.json
+-rw-r--r--   0        0        0      148 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/中津軽郡西目屋村.json
+-rw-r--r--   0        0        0     1855 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/五所川原市.json
+-rw-r--r--   0        0        0     5323 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/八戸市.json
+-rw-r--r--   0        0        0      283 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/北津軽郡中泊町.json
+-rw-r--r--   0        0        0      511 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/北津軽郡板柳町.json
+-rw-r--r--   0        0        0      277 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/北津軽郡鶴田町.json
+-rw-r--r--   0        0        0     1201 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/十和田市.json
+-rw-r--r--   0        0        0      241 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/南津軽郡大鰐町.json
+-rw-r--r--   0        0        0      319 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/南津軽郡田舎館村.json
+-rw-r--r--   0        0        0      544 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/南津軽郡藤崎町.json
+-rw-r--r--   0        0        0      622 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/平川市.json
+-rw-r--r--   0        0        0    11401 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/弘前市.json
+-rw-r--r--   0        0        0      160 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/東津軽郡今別町.json
+-rw-r--r--   0        0        0     2440 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/東津軽郡外ケ浜町.json
+-rw-r--r--   0        0        0      433 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/東津軽郡平内町.json
+-rw-r--r--   0        0        0      115 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/東津軽郡蓬田村.json
+-rw-r--r--   0        0        0      388 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/西津軽郡深浦町.json
+-rw-r--r--   0        0        0      583 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/西津軽郡鰺ヶ沢町.json
+-rw-r--r--   0        0        0     5821 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/青森市.json
+-rw-r--r--   0        0        0     2179 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/黒石市.json
+-rw-r--r--   0        0        0     1282 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/三島市.json
+-rw-r--r--   0        0        0      481 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/下田市.json
+-rw-r--r--   0        0        0      964 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/伊東市.json
+-rw-r--r--   0        0        0      481 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/伊豆の国市.json
+-rw-r--r--   0        0        0      553 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/伊豆市.json
+-rw-r--r--   0        0        0      208 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/周智郡森町.json
+-rw-r--r--   0        0        0     1015 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/富士宮市.json
+-rw-r--r--   0        0        0     2755 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/富士市.json
+-rw-r--r--   0        0        0     2017 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/島田市.json
+-rw-r--r--   0        0        0      139 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/御前崎市.json
+-rw-r--r--   0        0        0      721 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/御殿場市.json
+-rw-r--r--   0        0        0     2224 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/掛川市.json
+-rw-r--r--   0        0        0       46 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/榛原郡吉田町.json
+-rw-r--r--   0        0        0      217 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/榛原郡川根本町.json
+-rw-r--r--   0        0        0     2191 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/沼津市.json
+-rw-r--r--   0        0        0     3115 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市中区.json
+-rw-r--r--   0        0        0     1216 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市北区.json
+-rw-r--r--   0        0        0      760 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市南区.json
+-rw-r--r--   0        0        0     1201 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市天竜区.json
+-rw-r--r--   0        0        0      862 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市東区.json
+-rw-r--r--   0        0        0      559 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市浜北区.json
+-rw-r--r--   0        0        0      754 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市西区.json
+-rw-r--r--   0        0        0      502 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/湖西市.json
+-rw-r--r--   0        0        0     2170 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/焼津市.json
+-rw-r--r--   0        0        0      526 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/熱海市.json
+-rw-r--r--   0        0        0      508 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/牧之原市.json
+-rw-r--r--   0        0        0      157 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/田方郡函南町.json
+-rw-r--r--   0        0        0     2293 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/磐田市.json
+-rw-r--r--   0        0        0      562 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/菊川市.json
+-rw-r--r--   0        0        0     3517 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/藤枝市.json
+-rw-r--r--   0        0        0     1525 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/袋井市.json
+-rw-r--r--   0        0        0      385 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/裾野市.json
+-rw-r--r--   0        0        0      256 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/賀茂郡南伊豆町.json
+-rw-r--r--   0        0        0       49 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/賀茂郡東伊豆町.json
+-rw-r--r--   0        0        0      217 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/賀茂郡松崎町.json
+-rw-r--r--   0        0        0      145 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/賀茂郡河津町.json
+-rw-r--r--   0        0        0       70 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/賀茂郡西伊豆町.json
+-rw-r--r--   0        0        0     4327 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/静岡市清水区.json
+-rw-r--r--   0        0        0     6016 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/静岡市葵区.json
+-rw-r--r--   0        0        0     2902 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/静岡市駿河区.json
+-rw-r--r--   0        0        0      235 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/駿東郡小山町.json
+-rw-r--r--   0        0        0      145 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/駿東郡清水町.json
+-rw-r--r--   0        0        0      178 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/駿東郡長泉町.json
+-rw-r--r--   0        0        0      364 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/香川県/さぬき市.json
+-rw-r--r--   0        0        0      751 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/香川県/三豊市.json
+-rw-r--r--   0        0        0     2482 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/香川県/丸亀市.json
+-rw-r--r--   0        0        0      286 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/香川県/仲多度郡まんのう町.json
+-rw-r--r--   0        0        0      640 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/香川県/仲多度郡多度津町.json
+-rw-r--r--   0        0        0       79 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/香川県/仲多度郡琴平町.json
+-rw-r--r--   0        0        0      802 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/香川県/善通寺市.json
+-rw-r--r--   0        0        0     1669 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/香川県/坂出市.json
+-rw-r--r--   0        0        0      217 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/香川県/小豆郡土庄町.json
+-rw-r--r--   0        0        0      232 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/香川県/小豆郡小豆島町.json
+-rw-r--r--   0        0        0      202 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/香川県/木田郡三木町.json
+-rw-r--r--   0        0        0      322 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/香川県/東かがわ市.json
+-rw-r--r--   0        0        0      181 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/香川県/綾歌郡宇多津町.json
+-rw-r--r--   0        0        0      157 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/香川県/綾歌郡綾川町.json
+-rw-r--r--   0        0        0     1516 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/香川県/観音寺市.json
+-rw-r--r--   0        0        0      598 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/香川県/香川郡直島町.json
+-rw-r--r--   0        0        0     3817 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/香川県/高松市.json
+-rw-r--r--   0        0        0     1495 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/南国市.json
+-rw-r--r--   0        0        0      967 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/吾川郡いの町.json
+-rw-r--r--   0        0        0      760 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/吾川郡仁淀川町.json
+-rw-r--r--   0        0        0     2479 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/四万十市.json
+-rw-r--r--   0        0        0      376 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/土佐市.json
+-rw-r--r--   0        0        0      643 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/土佐清水市.json
+-rw-r--r--   0        0        0      244 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/土佐郡土佐町.json
+-rw-r--r--   0        0        0      172 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/土佐郡大川村.json
+-rw-r--r--   0        0        0      745 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/安芸市.json
+-rw-r--r--   0        0        0      301 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/安芸郡北川村.json
+-rw-r--r--   0        0        0       19 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/安芸郡奈半利町.json
+-rw-r--r--   0        0        0      268 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/安芸郡安田町.json
+-rw-r--r--   0        0        0       76 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/安芸郡東洋町.json
+-rw-r--r--   0        0        0     2269 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/安芸郡田野町.json
+-rw-r--r--   0        0        0       58 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/安芸郡芸西村.json
+-rw-r--r--   0        0        0       34 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/安芸郡馬路村.json
+-rw-r--r--   0        0        0      145 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/室戸市.json
+-rw-r--r--   0        0        0     1426 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/宿毛市.json
+-rw-r--r--   0        0        0      220 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/幡多郡三原村.json
+-rw-r--r--   0        0        0      418 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/幡多郡大月町.json
+-rw-r--r--   0        0        0      397 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/幡多郡黒潮町.json
+-rw-r--r--   0        0        0      556 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/長岡郡大豊町.json
+-rw-r--r--   0        0        0      193 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/長岡郡本山町.json
+-rw-r--r--   0        0        0      910 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/須崎市.json
+-rw-r--r--   0        0        0     1237 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/香南市.json
+-rw-r--r--   0        0        0     3604 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/香美市.json
+-rw-r--r--   0        0        0      658 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/高岡郡中土佐町.json
+-rw-r--r--   0        0        0      217 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/高岡郡佐川町.json
+-rw-r--r--   0        0        0     1318 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/高岡郡四万十町.json
+-rw-r--r--   0        0        0      115 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/高岡郡日高村.json
+-rw-r--r--   0        0        0      571 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/高岡郡檮原町.json
+-rw-r--r--   0        0        0      220 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/高岡郡津野町.json
+-rw-r--r--   0        0        0      313 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/高岡郡越知町.json
+-rw-r--r--   0        0        0     6865 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/高知市.json
+-rw-r--r--   0        0        0     2248 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/倉吉市.json
+-rw-r--r--   0        0        0      907 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/八頭郡八頭町.json
+-rw-r--r--   0        0        0      652 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/八頭郡智頭町.json
+-rw-r--r--   0        0        0      394 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/八頭郡若桜町.json
+-rw-r--r--   0        0        0      619 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/境港市.json
+-rw-r--r--   0        0        0      613 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/岩美郡岩美町.json
+-rw-r--r--   0        0        0      319 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/日野郡日南町.json
+-rw-r--r--   0        0        0      253 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/日野郡日野町.json
+-rw-r--r--   0        0        0      286 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/日野郡江府町.json
+-rw-r--r--   0        0        0      721 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/東伯郡三朝町.json
+-rw-r--r--   0        0        0      262 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/東伯郡北栄町.json
+-rw-r--r--   0        0        0      727 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/東伯郡湯梨浜町.json
+-rw-r--r--   0        0        0      856 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/東伯郡琴浦町.json
+-rw-r--r--   0        0        0     3937 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/米子市.json
+-rw-r--r--   0        0        0      520 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/西伯郡伯耆町.json
+-rw-r--r--   0        0        0      466 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/西伯郡南部町.json
+-rw-r--r--   0        0        0      622 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/西伯郡大山町.json
+-rw-r--r--   0        0        0       49 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/西伯郡日吉津村.json
+-rw-r--r--   0        0        0     9094 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/鳥取市.json
+-rw-r--r--   0        0        0      763 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/いちき串木野市.json
+-rw-r--r--   0        0        0      571 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/伊佐市.json
+-rw-r--r--   0        0        0      583 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/出水市.json
+-rw-r--r--   0        0        0      118 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/出水郡長島町.json
+-rw-r--r--   0        0        0      790 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/南さつま市.json
+-rw-r--r--   0        0        0      559 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/南九州市.json
+-rw-r--r--   0        0        0      289 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/垂水市.json
+-rw-r--r--   0        0        0       91 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/大島郡与論町.json
+-rw-r--r--   0        0        0      271 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/大島郡伊仙町.json
+-rw-r--r--   0        0        0      307 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/大島郡和泊町.json
+-rw-r--r--   0        0        0      490 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/大島郡喜界町.json
+-rw-r--r--   0        0        0      181 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/大島郡大和村.json
+-rw-r--r--   0        0        0      181 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/大島郡天城町.json
+-rw-r--r--   0        0        0      196 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/大島郡宇検村.json
+-rw-r--r--   0        0        0      154 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/大島郡徳之島町.json
+-rw-r--r--   0        0        0      817 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/大島郡瀬戸内町.json
+-rw-r--r--   0        0        0      322 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/大島郡知名町.json
+-rw-r--r--   0        0        0      133 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/大島郡龍郷町.json
+-rw-r--r--   0        0        0     1717 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/奄美市.json
+-rw-r--r--   0        0        0      850 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/姶良市.json
+-rw-r--r--   0        0        0      121 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/姶良郡湧水町.json
+-rw-r--r--   0        0        0      403 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/志布志市.json
+-rw-r--r--   0        0        0      673 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/指宿市.json
+-rw-r--r--   0        0        0     1066 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/日置市.json
+-rw-r--r--   0        0        0      742 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/曽於市.json
+-rw-r--r--   0        0        0       94 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/曽於郡大崎町.json
+-rw-r--r--   0        0        0     1069 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/枕崎市.json
+-rw-r--r--   0        0        0       64 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/熊毛郡中種子町.json
+-rw-r--r--   0        0        0       61 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/熊毛郡南種子町.json
+-rw-r--r--   0        0        0      181 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/熊毛郡屋久島町.json
+-rw-r--r--   0        0        0      139 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/肝属郡南大隅町.json
+-rw-r--r--   0        0        0       52 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/肝属郡東串良町.json
+-rw-r--r--   0        0        0       91 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/肝属郡肝付町.json
+-rw-r--r--   0        0        0       55 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/肝属郡錦江町.json
+-rw-r--r--   0        0        0     1444 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/薩摩川内市.json
+-rw-r--r--   0        0        0      250 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/薩摩郡さつま町.json
+-rw-r--r--   0        0        0      160 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/西之表市.json
+-rw-r--r--   0        0        0      289 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/阿久根市.json
+-rw-r--r--   0        0        0     2206 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/霧島市.json
+-rw-r--r--   0        0        0     6250 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/鹿児島市.json
+-rw-r--r--   0        0        0       49 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/鹿児島郡三島村.json
+-rw-r--r--   0        0        0      145 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/鹿児島郡十島村.json
+-rw-r--r--   0        0        0     1273 2021-06-17 01:45:25.869507 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/鹿屋市.json
+-rw-r--r--   0        0        0    35201 2021-06-17 01:45:25.821508 normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja.json
+-rw-r--r--   0        0        0       46 2021-06-11 00:32:50.564787 normalize_japanese_address-0.0.9/normalize_japanese_address/lib/__init__.py
+-rw-r--r--   0        0        0     7571 2021-06-24 04:49:51.689299 normalize_japanese_address-0.0.9/normalize_japanese_address/lib/cacheRegexes.py
+-rw-r--r--   0        0        0      517 2021-06-23 23:29:20.172815 normalize_japanese_address-0.0.9/normalize_japanese_address/lib/config.py
+-rw-r--r--   0        0        0      714 2021-06-17 03:50:15.441336 normalize_japanese_address-0.0.9/normalize_japanese_address/lib/const.py
+-rw-r--r--   0        0        0     7097 2021-06-24 01:42:59.100642 normalize_japanese_address-0.0.9/normalize_japanese_address/lib/dict.py
+-rw-r--r--   0        0        0     1043 2021-06-17 21:40:29.105979 normalize_japanese_address-0.0.9/normalize_japanese_address/lib/kan2num.py
+-rw-r--r--   0        0        0      918 2021-06-11 05:08:19.331664 normalize_japanese_address-0.0.9/normalize_japanese_address/lib/num2kan.py
+-rw-r--r--   0        0        0     1167 2021-06-17 03:53:16.329845 normalize_japanese_address-0.0.9/normalize_japanese_address/lib/patch_addr.py
+-rw-r--r--   0        0        0      162 2021-05-25 10:18:26.072101 normalize_japanese_address-0.0.9/normalize_japanese_address/lib/zen2han.py
+-rw-r--r--   0        0        0     4958 2021-06-24 01:23:13.920206 normalize_japanese_address-0.0.9/normalize_japanese_address/normalize.py
+-rw-r--r--   0        0        0       46 2021-06-16 22:52:08.527449 normalize_japanese_address-0.0.9/normalize_japanese_address/tests/__init__.py
+-rw-r--r--   0        0        0    26202 2021-06-24 04:35:03.254614 normalize_japanese_address-0.0.9/normalize_japanese_address/tests/test_normalize_japanese_address.py
+-rw-r--r--   0        0        0      714 2021-06-24 02:02:52.000944 normalize_japanese_address-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     5971 2021-06-24 04:51:25.316981 normalize_japanese_address-0.0.9/setup.py
+-rw-r--r--   0        0        0     2469 2021-06-24 04:51:25.317378 normalize_japanese_address-0.0.9/PKG-INFO
```

### Comparing `normalize_japanese_address-0.0.8/LICENSE.txt` & `normalize_japanese_address-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/README.md` & `normalize_japanese_address-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/いなべ市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/いなべ市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/三重郡菰野町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/三重郡菰野町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/亀山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/亀山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/伊勢市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/伊勢市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/伊賀市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/伊賀市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/名張市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/名張市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/四日市市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/四日市市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/多気郡明和町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/多気郡明和町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/尾鷲市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/尾鷲市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/志摩市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/志摩市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/松阪市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/松阪市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/桑名市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/桑名市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/津市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/津市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/熊野市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/熊野市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/三重県/鈴鹿市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/三重県/鈴鹿市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/亀岡市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/亀岡市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京丹後市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京丹後市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京田辺市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京田辺市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京都市上京区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京都市上京区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京都市下京区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京都市下京区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京都市中京区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京都市中京区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京都市伏見区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京都市伏見区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京都市北区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京都市北区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京都市南区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京都市南区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京都市右京区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京都市右京区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京都市山科区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京都市山科区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京都市左京区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京都市左京区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京都市東山区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京都市東山区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/京都市西京区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/京都市西京区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/八幡市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/八幡市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/南丹市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/南丹市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/宇治市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/宇治市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/宮津市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/宮津市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/木津川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/木津川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/相楽郡精華町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/相楽郡精華町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/福知山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/福知山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/綾部市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/綾部市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/舞鶴市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/舞鶴市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/船井郡京丹波町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/船井郡京丹波町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/京都府/長岡京市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/京都府/長岡京市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/伊万里市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/伊万里市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/佐賀市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/佐賀市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/唐津市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/唐津市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/小城市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/小城市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/武雄市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/武雄市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/神埼市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/神埼市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/西松浦郡有田町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/西松浦郡有田町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/佐賀県/鳥栖市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/佐賀県/鳥栖市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/たつの市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/たつの市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/三木市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/三木市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/三田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/三田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/丹波市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/丹波市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/丹波篠山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/丹波篠山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/伊丹市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/伊丹市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/佐用郡佐用町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/佐用郡佐用町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/加古川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/加古川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/加古郡播磨町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/加古郡播磨町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/加東市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/加東市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/加西市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/加西市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/南あわじ市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/南あわじ市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/多可郡多可町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/多可郡多可町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/姫路市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/姫路市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/宍粟市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/宍粟市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/宝塚市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/宝塚市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/小野市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/小野市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/尼崎市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/尼崎市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/川西市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/川西市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/川辺郡猪名川町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/川辺郡猪名川町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/明石市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/明石市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/朝来市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/朝来市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/洲本市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/洲本市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/淡路市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/淡路市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/相生市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/相生市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市中央区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市中央区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市兵庫区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市兵庫区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市北区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市北区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市垂水区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市垂水区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市東灘区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市東灘区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市灘区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市灘区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市西区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市西区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市長田区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市長田区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市須磨区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/神戸市須磨区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/美方郡香美町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/美方郡香美町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/芦屋市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/芦屋市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/西宮市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/西宮市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/西脇市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/西脇市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/豊岡市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/豊岡市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/赤穂市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/赤穂市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/赤穂郡上郡町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/赤穂郡上郡町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/養父市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/養父市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/兵庫県/高砂市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/兵庫県/高砂市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/三笠市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/三笠市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡当麻町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡当麻町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡新得町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡新得町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡東川町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡東川町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡東神楽町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡東神楽町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡比布町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡比布町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡清水町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡清水町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡美瑛町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡美瑛町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡鷹栖町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/上川郡鷹栖町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/中川郡幕別町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/中川郡幕別町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/中川郡池田町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/中川郡池田町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/中川郡美深町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/中川郡美深町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/久遠郡せたな町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/久遠郡せたな町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/亀田郡七飯町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/亀田郡七飯町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/二海郡八雲町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/二海郡八雲町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/伊達市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/伊達市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/余市郡仁木町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/余市郡仁木町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/余市郡余市町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/余市郡余市町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/函館市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/函館市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/勇払郡むかわ町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/勇払郡むかわ町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/勇払郡安平町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/勇払郡安平町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/北広島市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/北広島市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/北斗市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/北斗市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/北見市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/北見市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/十勝郡浦幌町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/十勝郡浦幌町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/千歳市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/千歳市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/厚岸郡厚岸町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/厚岸郡厚岸町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/厚岸郡浜中町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/厚岸郡浜中町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/名寄市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/名寄市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/増毛郡増毛町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/増毛郡増毛町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/士別市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/士別市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/夕張市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/夕張市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/夕張郡栗山町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/夕張郡栗山町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/夕張郡長沼町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/夕張郡長沼町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/天塩郡天塩町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/天塩郡天塩町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/天塩郡幌延町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/天塩郡幌延町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/天塩郡豊富町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/天塩郡豊富町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/室蘭市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/室蘭市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/富良野市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/富良野市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/小樽市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/小樽市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/岩見沢市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/岩見沢市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/川上郡弟子屈町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/川上郡弟子屈町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/川上郡標茶町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/川上郡標茶町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/帯広市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/帯広市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/広尾郡大樹町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/広尾郡大樹町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/広尾郡広尾町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/広尾郡広尾町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/恵庭市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/恵庭市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/日高郡新ひだか町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/日高郡新ひだか町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/旭川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/旭川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市中央区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市中央区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市北区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市北区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市南区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市南区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市厚別区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市厚別区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市手稲区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市手稲区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市東区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市東区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市清田区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市清田区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市白石区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市白石区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市西区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市西区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市豊平区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/札幌市豊平区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/枝幸郡枝幸町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/枝幸郡枝幸町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/枝幸郡浜頓別町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/枝幸郡浜頓別町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/根室市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/根室市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/標津郡中標津町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/標津郡中標津町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/標津郡標津町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/標津郡標津町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/檜山郡江差町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/檜山郡江差町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/江別市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/江別市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/沙流郡日高町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/沙流郡日高町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/河東郡上士幌町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/河東郡上士幌町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/河東郡士幌町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/河東郡士幌町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/河東郡音更町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/河東郡音更町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/河東郡鹿追町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/河東郡鹿追町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/河西郡中札内村.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/河西郡中札内村.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/河西郡芽室町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/河西郡芽室町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/浦河郡浦河町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/浦河郡浦河町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/深川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/深川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/滝川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/滝川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/留萌市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/留萌市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/登別市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/登別市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/白糠郡白糠町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/白糠郡白糠町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/白老郡白老町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/白老郡白老町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/石狩市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/石狩市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/石狩郡新篠津村.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/石狩郡新篠津村.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/砂川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/砂川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/稚内市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/稚内市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/空知郡上富良野町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/空知郡上富良野町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/空知郡中富良野町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/空知郡中富良野町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/空知郡南幌町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/空知郡南幌町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/紋別市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/紋別市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/紋別郡滝上町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/紋別郡滝上町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/紋別郡遠軽町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/紋別郡遠軽町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/網走市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/網走市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/網走郡大空町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/網走郡大空町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/網走郡美幌町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/網走郡美幌町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/美唄市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/美唄市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/芦別市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/芦別市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/苫前郡羽幌町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/苫前郡羽幌町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/苫小牧市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/苫小牧市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/茅部郡森町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/茅部郡森町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/虻田郡倶知安町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/虻田郡倶知安町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/赤平市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/赤平市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/足寄郡足寄町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/足寄郡足寄町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/足寄郡陸別町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/足寄郡陸別町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/野付郡別海町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/野付郡別海町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/釧路市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/釧路市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/釧路郡釧路町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/釧路郡釧路町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/阿寒郡鶴居村.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/阿寒郡鶴居村.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/北海道/雨竜郡沼田町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/北海道/雨竜郡沼田町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/いすみ市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/いすみ市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/佐倉市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/佐倉市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/八千代市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/八千代市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/勝浦市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/勝浦市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/匝瑳市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/匝瑳市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/千葉市中央区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/千葉市中央区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/千葉市稲毛区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/千葉市稲毛区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/千葉市緑区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/千葉市緑区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/千葉市美浜区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/千葉市美浜区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/千葉市花見川区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/千葉市花見川区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/千葉市若葉区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/千葉市若葉区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/南房総市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/南房総市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/印旛郡栄町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/印旛郡栄町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/印旛郡酒々井町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/印旛郡酒々井町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/印西市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/印西市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/君津市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/君津市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/四街道市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/四街道市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/大網白里市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/大網白里市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/夷隅郡大多喜町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/夷隅郡大多喜町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/富津市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/富津市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/山武市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/山武市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/山武郡横芝光町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/山武郡横芝光町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/市原市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/市原市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/市川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/市川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/成田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/成田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/我孫子市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/我孫子市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/旭市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/旭市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/木更津市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/木更津市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/東金市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/東金市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/松戸市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/松戸市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/柏市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/柏市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/流山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/流山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/浦安市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/浦安市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/白井市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/白井市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/習志野市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/習志野市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/船橋市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/船橋市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/茂原市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/茂原市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/袖ヶ浦市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/袖ヶ浦市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/野田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/野田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/銚子市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/銚子市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/鎌ヶ谷市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/鎌ヶ谷市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/館山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/館山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/香取市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/香取市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/千葉県/鴨川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/千葉県/鴨川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/伊都郡かつらぎ町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/伊都郡かつらぎ町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/和歌山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/和歌山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/新宮市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/新宮市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/日高郡日高川町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/日高郡日高川町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/有田郡有田川町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/有田郡有田川町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/東牟婁郡那智勝浦町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/東牟婁郡那智勝浦町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/橋本市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/橋本市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/海南市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/海南市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/海草郡紀美野町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/海草郡紀美野町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/田辺市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/田辺市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/和歌山県/紀の川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/和歌山県/紀の川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市中央区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市中央区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市南区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市南区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市大宮区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市大宮区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市岩槻区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市岩槻区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市桜区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市桜区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市浦和区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市浦和区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市緑区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市緑区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市西区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市西区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市見沼区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/さいたま市見沼区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/ふじみ野市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/ふじみ野市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/三郷市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/三郷市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/上尾市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/上尾市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/久喜市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/久喜市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/入間市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/入間市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/入間郡毛呂山町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/入間郡毛呂山町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/入間郡越生町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/入間郡越生町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/八潮市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/八潮市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/加須市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/加須市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/北本市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/北本市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/北葛飾郡杉戸町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/北葛飾郡杉戸町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/北足立郡伊奈町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/北足立郡伊奈町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/南埼玉郡宮代町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/南埼玉郡宮代町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/吉川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/吉川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/和光市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/和光市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/坂戸市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/坂戸市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/富士見市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/富士見市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/川口市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/川口市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/川越市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/川越市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/幸手市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/幸手市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/志木市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/志木市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/戸田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/戸田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/所沢市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/所沢市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/新座市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/新座市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/日高市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/日高市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/春日部市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/春日部市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/朝霞市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/朝霞市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/本庄市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/本庄市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/東松山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/東松山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/桶川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/桶川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/比企郡吉見町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/比企郡吉見町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/比企郡小川町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/比企郡小川町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/比企郡川島町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/比企郡川島町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/深谷市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/深谷市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/熊谷市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/熊谷市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/狭山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/狭山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/白岡市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/白岡市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/秩父市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/秩父市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/羽生市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/羽生市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/草加市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/草加市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/蓮田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/蓮田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/蕨市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/蕨市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/行田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/行田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/越谷市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/越谷市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/飯能市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/飯能市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/鴻巣市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/鴻巣市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/埼玉県/鶴ヶ島市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/埼玉県/鶴ヶ島市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/中津市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/中津市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/佐伯市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/佐伯市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/別府市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/別府市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/国東市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/国東市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/大分市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/大分市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/宇佐市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/宇佐市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/日田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/日田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/杵築市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/杵築市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/津久見市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/津久見市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/由布市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/由布市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/竹田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/竹田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/臼杵市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/臼杵市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/豊後大野市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/豊後大野市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大分県/豊後高田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大分県/豊後高田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/三島郡島本町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/三島郡島本町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/交野市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/交野市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/八尾市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/八尾市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/南河内郡河南町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/南河内郡河南町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/吹田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/吹田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/和泉市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/和泉市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/四條畷市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/四條畷市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市中区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市中区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市北区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市北区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市南区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市南区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市堺区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市堺区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市東区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市東区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市美原区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市美原区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市西区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/堺市西区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大東市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大東市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市中央区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市中央区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市住之江区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市住之江区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市住吉区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市住吉区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市北区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市北区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市城東区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市城東区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市大正区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市大正区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市天王寺区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市天王寺区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市平野区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市平野区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市旭区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市旭区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市東住吉区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市東住吉区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市東成区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市東成区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市東淀川区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市東淀川区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市此花区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市此花区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市浪速区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市浪速区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市淀川区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市淀川区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市港区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市港区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市生野区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市生野区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市福島区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市福島区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市西区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市西区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市西成区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市西成区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市西淀川区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市西淀川区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市都島区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市都島区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市阿倍野区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市阿倍野区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市鶴見区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪市鶴見区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪狭山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/大阪狭山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/守口市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/守口市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/富田林市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/富田林市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/寝屋川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/寝屋川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/岸和田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/岸和田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/摂津市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/摂津市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/東大阪市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/東大阪市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/松原市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/松原市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/枚方市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/枚方市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/柏原市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/柏原市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/池田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/池田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/河内長野市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/河内長野市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/泉佐野市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/泉佐野市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/泉北郡忠岡町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/泉北郡忠岡町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/泉南市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/泉南市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/泉南郡熊取町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/泉南郡熊取町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/泉大津市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/泉大津市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/箕面市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/箕面市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/羽曳野市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/羽曳野市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/茨木市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/茨木市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/藤井寺市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/藤井寺市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/豊中市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/豊中市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/豊能郡豊能町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/豊能郡豊能町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/貝塚市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/貝塚市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/門真市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/門真市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/阪南市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/阪南市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/高槻市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/高槻市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/大阪府/高石市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/大阪府/高石市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/五條市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/五條市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/北葛城郡上牧町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/北葛城郡上牧町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/北葛城郡広陵町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/北葛城郡広陵町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/北葛城郡河合町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/北葛城郡河合町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/北葛城郡王寺町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/北葛城郡王寺町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡十津川村.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡十津川村.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡吉野町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/吉野郡吉野町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/大和郡山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/大和郡山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/大和高田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/大和高田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/天理市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/天理市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/奈良市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/奈良市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/宇陀市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/宇陀市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/御所市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/御所市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/桜井市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/桜井市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/橿原市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/橿原市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/生駒市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/生駒市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/生駒郡三郷町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/生駒郡三郷町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/生駒郡平群町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/生駒郡平群町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/生駒郡斑鳩町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/生駒郡斑鳩町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/磯城郡田原本町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/磯城郡田原本町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/奈良県/香芝市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/奈良県/香芝市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/亘理郡亘理町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/亘理郡亘理町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/仙台市太白区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/仙台市太白区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/仙台市宮城野区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/仙台市宮城野区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/仙台市泉区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/仙台市泉区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/仙台市若林区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/仙台市若林区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/仙台市青葉区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/仙台市青葉区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/伊具郡丸森町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/伊具郡丸森町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/刈田郡七ヶ宿町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/刈田郡七ヶ宿町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/加美郡加美町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/加美郡加美町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/名取市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/名取市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/塩竈市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/塩竈市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/多賀城市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/多賀城市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/大崎市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/大崎市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/宮城郡利府町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/宮城郡利府町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/富谷市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/富谷市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/岩沼市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/岩沼市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/柴田郡大河原町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/柴田郡大河原町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/柴田郡柴田町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/柴田郡柴田町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/栗原市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/栗原市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/気仙沼市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/気仙沼市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/登米市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/登米市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/白石市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/白石市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/石巻市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/石巻市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/遠田郡涌谷町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/遠田郡涌谷町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/遠田郡美里町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/遠田郡美里町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮城県/黒川郡大和町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮城県/黒川郡大和町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/宮崎市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/宮崎市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/延岡市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/延岡市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/日南市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/日南市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/日向市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/日向市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/東臼杵郡門川町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/東臼杵郡門川町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/西都市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/西都市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/宮崎県/都城市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/宮崎県/都城市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/下新川郡入善町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/下新川郡入善町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/中新川郡上市町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/中新川郡上市町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/中新川郡立山町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/中新川郡立山町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/南砺市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/南砺市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/富山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/富山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/射水市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/射水市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/小矢部市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/小矢部市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/氷見市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/氷見市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/滑川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/滑川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/砺波市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/砺波市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/高岡市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/高岡市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/魚津市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/魚津市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/富山県/黒部市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/富山県/黒部市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/下松市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/下松市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/下関市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/下関市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/光市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/光市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/周南市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/周南市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/大島郡周防大島町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/大島郡周防大島町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/宇部市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/宇部市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/山口市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/山口市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/山陽小野田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/山陽小野田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/岩国市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/岩国市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/柳井市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/柳井市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/美祢市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/美祢市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/萩市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/萩市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山口県/防府市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山口県/防府市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/上山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/上山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/天童市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/天童市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/寒河江市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/寒河江市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/尾花沢市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/尾花沢市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/山形市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/山形市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/新庄市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/新庄市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/村山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/村山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/東根市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/東根市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/東田川郡庄内町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/東田川郡庄内町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/東置賜郡高畠町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/東置賜郡高畠町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/米沢市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/米沢市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/西村山郡大江町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/西村山郡大江町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/西置賜郡小国町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/西置賜郡小国町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/酒田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/酒田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/長井市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/長井市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山形県/鶴岡市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山形県/鶴岡市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/北杜市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/北杜市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/南アルプス市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/南アルプス市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/南巨摩郡身延町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/南巨摩郡身延町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/南都留郡道志村.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/南都留郡道志村.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/南都留郡鳴沢村.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/南都留郡鳴沢村.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/大月市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/大月市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/富士吉田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/富士吉田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/山梨市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/山梨市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/甲州市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/甲州市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/甲府市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/甲府市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/笛吹市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/笛吹市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/都留市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/都留市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/山梨県/韮崎市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/山梨県/韮崎市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/下呂市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/下呂市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/中津川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/中津川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/可児市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/可児市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/各務原市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/各務原市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/土岐市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/土岐市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/多治見市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/多治見市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/大垣市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/大垣市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/岐阜市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/岐阜市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/恵那市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/恵那市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/揖斐郡揖斐川町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/揖斐郡揖斐川町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/本巣市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/本巣市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/本巣郡北方町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/本巣郡北方町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/海津市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/海津市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/瑞浪市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/瑞浪市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/瑞穂市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/瑞穂市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/美濃加茂市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/美濃加茂市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/美濃市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/美濃市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/羽島市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/羽島市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/羽島郡岐南町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/羽島郡岐南町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/羽島郡笠松町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/羽島郡笠松町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/郡上市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/郡上市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/関市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/関市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/飛騨市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/飛騨市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/養老郡養老町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/養老郡養老町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岐阜県/高山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岐阜県/高山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/久米郡美咲町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/久米郡美咲町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/井原市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/井原市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/倉敷市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/倉敷市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/備前市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/備前市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/岡山市中区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/岡山市中区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/岡山市北区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/岡山市北区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/岡山市南区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/岡山市南区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/岡山市東区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/岡山市東区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/新見市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/新見市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/津山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/津山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/浅口市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/浅口市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/瀬戸内市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/瀬戸内市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/玉野市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/玉野市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/真庭市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/真庭市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/笠岡市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/笠岡市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/総社市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/総社市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/美作市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/美作市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/苫田郡鏡野町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/苫田郡鏡野町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/赤磐市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/赤磐市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岡山県/高梁市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岡山県/高梁市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/一関市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/一関市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/下閉伊郡普代村.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/下閉伊郡普代村.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/久慈市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/久慈市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/八幡平市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/八幡平市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/北上市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/北上市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/和賀郡西和賀町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/和賀郡西和賀町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/奥州市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/奥州市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/宮古市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/宮古市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/岩手郡雫石町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/岩手郡雫石町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/滝沢市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/滝沢市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/盛岡市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/盛岡市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/紫波郡矢巾町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/紫波郡矢巾町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/紫波郡紫波町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/紫波郡紫波町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/花巻市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/花巻市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/遠野市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/遠野市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/岩手県/釜石市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/岩手県/釜石市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/出雲市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/出雲市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/大田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/大田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/安来市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/安来市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/松江市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/松江市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/江津市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/江津市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/浜田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/浜田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/益田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/益田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/島根県/雲南市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/島根県/雲南市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/三原市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/三原市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/三次市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/三次市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/世羅郡世羅町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/世羅郡世羅町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/呉市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/呉市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/大竹市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/大竹市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/安芸郡坂町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/安芸郡坂町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/安芸郡府中町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/安芸郡府中町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/安芸郡海田町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/安芸郡海田町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/安芸郡熊野町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/安芸郡熊野町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/安芸高田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/安芸高田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/尾道市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/尾道市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/山県郡北広島町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/山県郡北広島町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/広島市中区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/広島市中区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/広島市佐伯区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/広島市佐伯区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/広島市南区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/広島市南区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/広島市安佐北区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/広島市安佐北区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/広島市安佐南区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/広島市安佐南区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/広島市安芸区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/広島市安芸区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/広島市東区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/広島市東区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/広島市西区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/広島市西区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/庄原市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/庄原市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/府中市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/府中市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/廿日市市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/廿日市市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/東広島市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/東広島市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/江田島市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/江田島市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/福山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/福山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/広島県/竹原市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/広島県/竹原市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/三好市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/三好市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/吉野川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/吉野川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/徳島市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/徳島市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/那賀郡那賀町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/那賀郡那賀町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/阿南市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/阿南市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/阿波市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/阿波市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/徳島県/鳴門市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/徳島県/鳴門市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/今治市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/今治市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/八幡浜市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/八幡浜市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/北宇和郡鬼北町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/北宇和郡鬼北町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/南宇和郡愛南町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/南宇和郡愛南町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/四国中央市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/四国中央市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/大洲市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/大洲市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/宇和島市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/宇和島市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/新居浜市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/新居浜市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/松山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/松山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/西予市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/西予市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛媛県/西条市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛媛県/西条市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/あま市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/あま市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/みよし市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/みよし市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/一宮市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/一宮市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/丹羽郡大口町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/丹羽郡大口町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/刈谷市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/刈谷市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/北名古屋市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/北名古屋市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/半田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/半田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市中区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市中区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市中川区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市中川区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市中村区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市中村区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市北区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市北区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市千種区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市千種区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市南区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市南区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市名東区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市名東区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市天白区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市天白区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市守山区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市守山区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市昭和区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市昭和区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市東区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市東区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市港区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市港区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市熱田区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市熱田区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市瑞穂区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市瑞穂区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市緑区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市緑区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市西区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/名古屋市西区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/大府市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/大府市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/安城市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/安城市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/小牧市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/小牧市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/尾張旭市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/尾張旭市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/岡崎市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/岡崎市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/岩倉市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/岩倉市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/常滑市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/常滑市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/弥富市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/弥富市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/愛知郡東郷町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/愛知郡東郷町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/愛西市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/愛西市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/新城市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/新城市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/日進市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/日進市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/春日井市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/春日井市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/東海市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/東海市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/江南市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/江南市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/津島市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/津島市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/海部郡蟹江町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/海部郡蟹江町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/海部郡飛島村.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/海部郡飛島村.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/清須市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/清須市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/瀬戸市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/瀬戸市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/犬山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/犬山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/田原市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/田原市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/知多市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/知多市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/知多郡武豊町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/知多郡武豊町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/知多郡美浜町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/知多郡美浜町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/知立市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/知立市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/碧南市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/碧南市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/稲沢市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/稲沢市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/蒲郡市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/蒲郡市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/西尾市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/西尾市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/豊川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/豊川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/豊橋市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/豊橋市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/豊田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/豊田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/長久手市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/長久手市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/愛知県/高浜市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/愛知県/高浜市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/三島郡出雲崎町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/三島郡出雲崎町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/三条市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/三条市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/上越市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/上越市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/五泉市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/五泉市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/佐渡市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/佐渡市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/加茂市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/加茂市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/十日町市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/十日町市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/南魚沼市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/南魚沼市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/妙高市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/妙高市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/小千谷市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/小千谷市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/岩船郡関川村.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/岩船郡関川村.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市中央区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市中央区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市北区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市北区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市南区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市南区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市東区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市東区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市江南区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市江南区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市秋葉区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市秋葉区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市西区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市西区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市西蒲区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/新潟市西蒲区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/新発田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/新発田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/村上市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/村上市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/東蒲原郡阿賀町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/東蒲原郡阿賀町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/柏崎市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/柏崎市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/燕市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/燕市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/糸魚川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/糸魚川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/胎内市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/胎内市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/見附市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/見附市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/長岡市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/長岡市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/阿賀野市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/阿賀野市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/新潟県/魚沼市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/新潟県/魚沼市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/あきる野市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/あきる野市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/三鷹市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/三鷹市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/世田谷区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/世田谷区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/中央区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/中央区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/中野区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/中野区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/八王子市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/八王子市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/北区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/北区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/千代田区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/千代田区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/台東区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/台東区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/品川区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/品川区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/国分寺市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/国分寺市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/墨田区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/墨田区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/多摩市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/多摩市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/大田区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/大田区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/小平市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/小平市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/小金井市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/小金井市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/府中市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/府中市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/文京区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/文京区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/新宿区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/新宿区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/日野市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/日野市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/昭島市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/昭島市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/杉並区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/杉並区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/東久留米市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/東久留米市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/東大和市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/東大和市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/東村山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/東村山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/板橋区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/板橋区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/武蔵村山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/武蔵村山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/武蔵野市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/武蔵野市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/江戸川区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/江戸川区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/江東区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/江東区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/清瀬市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/清瀬市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/渋谷区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/渋谷区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/港区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/港区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/狛江市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/狛江市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/町田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/町田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/目黒区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/目黒区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/立川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/立川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/練馬区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/練馬区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/羽村市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/羽村市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/荒川区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/荒川区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/葛飾区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/葛飾区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/西東京市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/西東京市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/調布市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/調布市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/豊島区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/豊島区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/足立区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/足立区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/東京都/青梅市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/東京都/青梅市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/さくら市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/さくら市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/下都賀郡壬生町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/下都賀郡壬生町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/下野市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/下野市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/佐野市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/佐野市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/塩谷郡高根沢町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/塩谷郡高根沢町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/大田原市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/大田原市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/宇都宮市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/宇都宮市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/小山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/小山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/日光市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/日光市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/栃木市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/栃木市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/真岡市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/真岡市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/芳賀郡茂木町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/芳賀郡茂木町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/足利市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/足利市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/那須塩原市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/那須塩原市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/那須烏山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/那須烏山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/栃木県/鹿沼市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/栃木県/鹿沼市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/うるま市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/うるま市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/南城市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/南城市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/名護市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/名護市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/宜野湾市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/宜野湾市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/沖縄市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/沖縄市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/浦添市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/浦添市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/糸満市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/糸満市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/沖縄県/那覇市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/沖縄県/那覇市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/大津市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/大津市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/守山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/守山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/彦根市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/彦根市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/東近江市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/東近江市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/栗東市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/栗東市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/湖南市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/湖南市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/犬上郡多賀町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/犬上郡多賀町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/甲賀市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/甲賀市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/米原市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/米原市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/草津市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/草津市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/蒲生郡日野町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/蒲生郡日野町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/近江八幡市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/近江八幡市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/野洲市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/野洲市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/長浜市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/長浜市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/滋賀県/高島市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/滋賀県/高島市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/上益城郡山都町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/上益城郡山都町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/人吉市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/人吉市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/八代市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/八代市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/天草市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/天草市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/宇土市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/宇土市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/宇城市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/宇城市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/山鹿市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/山鹿市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/水俣市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/水俣市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/熊本市中央区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/熊本市中央区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/熊本市北区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/熊本市北区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/熊本市南区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/熊本市南区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/熊本市東区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/熊本市東区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/熊本市西区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/熊本市西区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/玉名市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/玉名市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/荒尾市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/荒尾市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/菊池市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/菊池市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/菊池郡菊陽町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/菊池郡菊陽町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/葦北郡芦北町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/葦北郡芦北町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/熊本県/阿蘇市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/熊本県/阿蘇市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/かほく市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/かほく市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/七尾市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/七尾市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/加賀市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/加賀市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/小松市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/小松市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/河北郡内灘町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/河北郡内灘町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/河北郡津幡町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/河北郡津幡町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/珠洲市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/珠洲市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/白山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/白山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/羽咋市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/羽咋市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/羽咋郡志賀町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/羽咋郡志賀町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/能美市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/能美市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/輪島市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/輪島市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/野々市市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/野々市市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/金沢市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/金沢市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/鳳珠郡穴水町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/鳳珠郡穴水町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/石川県/鳳珠郡能登町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/石川県/鳳珠郡能登町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/三浦市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/三浦市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/伊勢原市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/伊勢原市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/厚木市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/厚木市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/大和市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/大和市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/小田原市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/小田原市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市中原区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市中原区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市多摩区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市多摩区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市宮前区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市宮前区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市川崎区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市川崎区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市幸区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市幸区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市高津区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市高津区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市麻生区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/川崎市麻生区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/平塚市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/平塚市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/座間市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/座間市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市中区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市中区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市保土ケ谷区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市保土ケ谷区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市南区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市南区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市戸塚区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市戸塚区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市旭区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市旭区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市栄区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市栄区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市泉区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市泉区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市港北区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市港北区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市港南区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市港南区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市瀬谷区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市瀬谷区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市磯子区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市磯子区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市神奈川区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市神奈川区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市緑区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市緑区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市西区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市西区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市都筑区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市都筑区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市金沢区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市金沢区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市青葉区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市青葉区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市鶴見区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横浜市鶴見区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/横須賀市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/横須賀市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/海老名市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/海老名市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/相模原市中央区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/相模原市中央区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/相模原市南区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/相模原市南区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/相模原市緑区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/相模原市緑区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/秦野市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/秦野市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/綾瀬市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/綾瀬市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/茅ヶ崎市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/茅ヶ崎市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/藤沢市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/藤沢市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/逗子市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/逗子市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/鎌倉市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/鎌倉市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/神奈川県/高座郡寒川町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/神奈川県/高座郡寒川町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/あわら市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/あわら市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/三方上中郡若狭町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/三方上中郡若狭町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/丹生郡越前町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/丹生郡越前町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/勝山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/勝山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/南条郡南越前町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/南条郡南越前町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/吉田郡永平寺町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/吉田郡永平寺町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/坂井市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/坂井市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/大野市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/大野市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/大飯郡おおい町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/大飯郡おおい町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/大飯郡高浜町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/大飯郡高浜町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/小浜市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/小浜市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/敦賀市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/敦賀市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/福井市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/福井市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/越前市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/越前市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福井県/鯖江市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福井県/鯖江市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/うきは市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/うきは市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/みやま市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/みやま市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/中間市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/中間市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/久留米市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/久留米市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/京都郡みやこ町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/京都郡みやこ町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/京都郡苅田町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/京都郡苅田町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/八女市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/八女市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市八幡東区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市八幡東区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市八幡西区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市八幡西区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市小倉北区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市小倉北区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市小倉南区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市小倉南区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市戸畑区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市戸畑区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市若松区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市若松区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市門司区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/北九州市門司区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/古賀市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/古賀市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/大川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/大川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/大牟田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/大牟田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/大野城市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/大野城市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/太宰府市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/太宰府市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/宗像市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/宗像市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/小郡市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/小郡市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/春日市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/春日市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/朝倉市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/朝倉市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/柳川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/柳川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/直方市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/直方市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市中央区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市中央区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市南区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市南区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市博多区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市博多区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市城南区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市城南区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市早良区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市早良区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市東区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市東区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市西区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/福岡市西区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/福津市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/福津市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/筑後市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/筑後市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/筑紫野市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/筑紫野市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/築上郡築上町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/築上郡築上町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/糟屋郡宇美町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/糟屋郡宇美町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/糟屋郡志免町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/糟屋郡志免町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/糟屋郡新宮町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/糟屋郡新宮町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/糟屋郡粕屋町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/糟屋郡粕屋町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/糸島市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/糸島市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/行橋市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/行橋市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/豊前市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/豊前市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/遠賀郡岡垣町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/遠賀郡岡垣町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/遠賀郡水巻町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/遠賀郡水巻町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/遠賀郡遠賀町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/遠賀郡遠賀町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/那珂川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/那珂川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福岡県/飯塚市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福岡県/飯塚市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/いわき市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/いわき市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/二本松市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/二本松市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/伊達市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/伊達市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/伊達郡川俣町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/伊達郡川俣町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/伊達郡桑折町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/伊達郡桑折町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/会津若松市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/会津若松市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/南会津郡南会津町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/南会津郡南会津町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/南相馬市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/南相馬市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/双葉郡浪江町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/双葉郡浪江町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/喜多方市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/喜多方市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/大沼郡会津美里町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/大沼郡会津美里町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/岩瀬郡鏡石町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/岩瀬郡鏡石町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/東白川郡棚倉町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/東白川郡棚倉町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/河沼郡会津坂下町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/河沼郡会津坂下町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/田村市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/田村市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/田村郡三春町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/田村郡三春町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/白河市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/白河市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/相馬市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/相馬市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/石川郡石川町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/石川郡石川町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/福島市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/福島市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/耶麻郡猪苗代町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/耶麻郡猪苗代町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/西白河郡矢吹町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/西白河郡矢吹町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/郡山市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/郡山市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/福島県/須賀川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/福島県/須賀川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/仙北市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/仙北市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/北秋田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/北秋田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/南秋田郡五城目町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/南秋田郡五城目町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/大仙市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/大仙市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/大館市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/大館市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/横手市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/横手市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/湯沢市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/湯沢市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/由利本荘市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/由利本荘市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/男鹿市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/男鹿市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/秋田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/秋田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/能代市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/能代市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/秋田県/雄勝郡羽後町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/秋田県/雄勝郡羽後町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/伊勢崎市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/伊勢崎市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/前橋市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/前橋市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/太田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/太田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/安中市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/安中市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/富岡市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/富岡市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/桐生市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/桐生市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/沼田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/沼田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/渋川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/渋川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/邑楽郡大泉町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/邑楽郡大泉町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/館林市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/館林市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/群馬県/高崎市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/群馬県/高崎市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/かすみがうら市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/かすみがうら市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/つくばみらい市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/つくばみらい市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/つくば市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/つくば市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/ひたちなか市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/ひたちなか市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/下妻市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/下妻市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/久慈郡大子町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/久慈郡大子町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/北相馬郡利根町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/北相馬郡利根町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/北茨城市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/北茨城市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/取手市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/取手市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/古河市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/古河市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/土浦市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/土浦市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/坂東市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/坂東市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/守谷市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/守谷市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/小美玉市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/小美玉市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/常総市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/常総市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/常陸大宮市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/常陸大宮市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/常陸太田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/常陸太田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/日立市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/日立市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/東茨城郡城里町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/東茨城郡城里町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/東茨城郡茨城町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/東茨城郡茨城町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/桜川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/桜川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/水戸市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/水戸市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/潮来市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/潮来市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/牛久市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/牛久市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/石岡市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/石岡市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/神栖市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/神栖市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/稲敷市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/稲敷市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/稲敷郡美浦村.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/稲敷郡美浦村.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/稲敷郡阿見町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/稲敷郡阿見町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/笠間市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/笠間市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/筑西市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/筑西市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/結城市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/結城市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/結城郡八千代町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/結城郡八千代町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/行方市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/行方市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/那珂郡東海村.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/那珂郡東海村.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/鉾田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/鉾田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/高萩市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/高萩市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/鹿嶋市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/鹿嶋市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/茨城県/龍ヶ崎市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/茨城県/龍ヶ崎市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/五島市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/五島市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/佐世保市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/佐世保市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/南島原市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/南島原市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/南松浦郡新上五島町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/南松浦郡新上五島町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/壱岐市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/壱岐市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/大村市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/大村市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/対馬市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/対馬市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/島原市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/島原市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/平戸市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/平戸市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/西海市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/西海市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/諫早市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/諫早市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/長崎市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/長崎市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長崎県/雲仙市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長崎県/雲仙市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/上田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/上田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/中野市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/中野市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/伊那市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/伊那市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/佐久市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/佐久市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/千曲市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/千曲市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/南佐久郡南相木村.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/南佐久郡南相木村.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/塩尻市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/塩尻市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/小諸市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/小諸市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/岡谷市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/岡谷市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/松本市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/松本市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/諏訪市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/諏訪市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/諏訪郡下諏訪町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/諏訪郡下諏訪町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/長野市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/長野市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/須坂市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/須坂市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/長野県/飯田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/長野県/飯田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/つがる市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/つがる市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/むつ市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/むつ市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/三戸郡五戸町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/三戸郡五戸町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/三沢市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/三沢市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/上北郡おいらせ町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/上北郡おいらせ町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/上北郡七戸町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/上北郡七戸町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/上北郡東北町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/上北郡東北町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/上北郡横浜町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/上北郡横浜町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/上北郡野辺地町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/上北郡野辺地町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/五所川原市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/五所川原市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/八戸市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/八戸市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/十和田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/十和田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/南津軽郡藤崎町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/南津軽郡藤崎町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/平川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/平川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/弘前市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/弘前市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/東津軽郡外ケ浜町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/東津軽郡外ケ浜町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/西津軽郡鰺ヶ沢町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/西津軽郡鰺ヶ沢町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/青森市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/青森市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/青森県/黒石市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/青森県/黒石市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/三島市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/三島市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/伊東市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/伊東市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/伊豆市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/伊豆市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/富士宮市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/富士宮市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/富士市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/富士市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/島田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/島田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/御殿場市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/御殿場市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/掛川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/掛川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/沼津市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/沼津市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市中区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市中区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市北区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市北区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市南区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市南区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市天竜区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市天竜区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市東区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市東区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市浜北区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市浜北区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市西区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/浜松市西区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/焼津市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/焼津市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/熱海市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/熱海市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/磐田市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/磐田市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/菊川市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/菊川市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/藤枝市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/藤枝市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/袋井市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/袋井市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/静岡市清水区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/静岡市清水区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/静岡市葵区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/静岡市葵区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/静岡県/静岡市駿河区.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/静岡県/静岡市駿河区.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/香川県/三豊市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/香川県/三豊市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/香川県/丸亀市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/香川県/丸亀市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/香川県/仲多度郡多度津町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/香川県/仲多度郡多度津町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/香川県/善通寺市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/香川県/善通寺市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/香川県/坂出市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/香川県/坂出市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/香川県/観音寺市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/香川県/観音寺市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/香川県/香川郡直島町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/香川県/香川郡直島町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/香川県/高松市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/香川県/高松市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/南国市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/南国市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/吾川郡いの町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/吾川郡いの町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/吾川郡仁淀川町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/吾川郡仁淀川町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/四万十市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/四万十市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/土佐清水市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/土佐清水市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/安芸市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/安芸市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/安芸郡田野町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/安芸郡田野町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/宿毛市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/宿毛市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/長岡郡大豊町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/長岡郡大豊町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/須崎市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/須崎市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/香南市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/香南市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/香美市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/香美市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/高岡郡中土佐町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/高岡郡中土佐町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/高岡郡四万十町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/高岡郡四万十町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/高岡郡檮原町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/高岡郡檮原町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/高知県/高知市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/高知県/高知市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/倉吉市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/倉吉市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/八頭郡八頭町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/八頭郡八頭町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/八頭郡智頭町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/八頭郡智頭町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/境港市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/境港市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/岩美郡岩美町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/岩美郡岩美町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/東伯郡三朝町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/東伯郡三朝町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/東伯郡湯梨浜町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/東伯郡湯梨浜町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/東伯郡琴浦町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/東伯郡琴浦町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/米子市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/米子市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/西伯郡伯耆町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/西伯郡伯耆町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/西伯郡大山町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/西伯郡大山町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鳥取県/鳥取市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鳥取県/鳥取市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/いちき串木野市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/いちき串木野市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/伊佐市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/伊佐市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/出水市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/出水市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/南さつま市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/南さつま市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/南九州市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/南九州市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/大島郡瀬戸内町.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/大島郡瀬戸内町.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/奄美市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/奄美市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/姶良市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/姶良市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/指宿市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/指宿市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/日置市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/日置市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/曽於市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/曽於市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/枕崎市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/枕崎市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/薩摩川内市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/薩摩川内市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/霧島市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/霧島市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/鹿児島市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/鹿児島市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja/鹿児島県/鹿屋市.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja/鹿児島県/鹿屋市.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/japanese_address/api/ja.json` & `normalize_japanese_address-0.0.9/normalize_japanese_address/japanese_address/api/ja.json`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/lib/cacheRegexes.py` & `normalize_japanese_address-0.0.9/normalize_japanese_address/lib/cacheRegexes.py`

 * *Files 6% similar despite different names*

```diff
@@ -142,16 +142,28 @@
     cities: Tuple[str, ...] = tuple(prefectures.get(pref, tuple()))
     cityRegexes: Tuple[Tuple[str, str,]] = getCityRegexes(cities, option)
     return match_regexes(cityRegexes, addr)
 
 
 def normalizeTownName(addr: str, pref: str, city: str, config: Config, option: Option) -> Tuple[Optional[str], str]:
     townRegexes: Tuple[Tuple[str, str,]] = getTownRegexes(pref, city, config, option)
-    addr = re.sub('^大字', '', addr)
-    return match_regexes(townRegexes, addr)
+    _addr = re.sub('^(大)?字', '', addr)
+    # 大字、字を外した状態で突き合わせ
+    normalized_town_name, remaining_addr = match_regexes(townRegexes, _addr)
+    if normalized_town_name is None and addr != _addr:
+        # 大字、字を外して見つからない場合は、もとに戻して突き合わせ
+        normalized_town_name, remaining_addr = match_regexes(townRegexes, addr)
+    if normalized_town_name is None:
+        # それでも見つからない場合は機械的に分解
+        # addrに分解しきれない未知の住所があるケースに対処
+        m = re.match('([^\d\s]+)[\s]*([\d].*)', remaining_addr)
+        if m:
+            normalized_town_name = normalized_town_name+m.groups()[0] if normalized_town_name else m.groups()[0]
+            remaining_addr = m.groups()[1]
+    return normalized_town_name, remaining_addr
 
 
 # 都道府県名の推測
 def estimatePref(prefectures: Dict[str, Iterable[str]], addr: str, config: Config, option: Option) -> str:
     # 都道府県名が省略されている
     matched: List = []
     for _pref in prefectures:
```

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/lib/config.py` & `normalize_japanese_address-0.0.9/normalize_japanese_address/lib/config.py`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/lib/const.py` & `normalize_japanese_address-0.0.9/normalize_japanese_address/lib/const.py`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/lib/dict.py` & `normalize_japanese_address-0.0.9/normalize_japanese_address/lib/dict.py`

 * *Files 1% similar despite different names*

```diff
@@ -63,18 +63,18 @@
         ("藪|薮", '(藪|薮)'),
         ("渕|淵", '(渕|淵)'),
         ("エ|ヱ|え", '(エ|ヱ|え)'),
         ("曾|曽", '(曾|曽)'),
         ]
 COMPILED_REGEX_CUSTOM_PATTERNS = re.compile('|'.join([p for p, r in REGEX_CUSTOM_PATTERNS]))
 
-
 # 単純な住居表示変更
 SIMPLE_RENAMING_PATTERNS: Tuple[Tuple[str, str], ...] = (
         ('(筑紫郡)?那珂川町', '那珂川市'),
+        ('(丹波)?篠山市', '丹波篠山市'),
         ('(下都賀郡)?岩舟町', '栃木市岩舟町'),)
 
 
 def rep(s: str, search_pattern: str, replacee: str, replacement: Union[str, Callable]) -> str:
     matches: List[Tuple[Tuple[int, int], str]] = []
     for m in re.finditer(search_pattern, s):
         if isinstance(replacement, str):
```

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/lib/kan2num.py` & `normalize_japanese_address-0.0.9/normalize_japanese_address/lib/kan2num.py`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/lib/num2kan.py` & `normalize_japanese_address-0.0.9/normalize_japanese_address/lib/num2kan.py`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/lib/patch_addr.py` & `normalize_japanese_address-0.0.9/normalize_japanese_address/lib/patch_addr.py`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/normalize.py` & `normalize_japanese_address-0.0.9/normalize_japanese_address/normalize.py`

 * *Files identical despite different names*

### Comparing `normalize_japanese_address-0.0.8/normalize_japanese_address/tests/test_normalize_japanese_address.py` & `normalize_japanese_address-0.0.9/normalize_japanese_address/tests/test_normalize_japanese_address.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,34 +1,42 @@
 #!/usr/bin/env python
 # -*- coding: utf-8 -*-
 from typing import Dict, List, Tuple
-
+import sys
+print(sys.path)
 from ..lib.const import ADDRESS, CITY, LEVEL, PREF, TOWN
 from ..lib.config import DEFAULT_OPTION
 from ..normalize import normalize
 
 
 TEST_PATTERNS: List[Tuple[str, Dict[str, str]]] = [
 
-        # 追加テスト
+        # 追加テスト 
+        ('埼玉県鶴ヶ島市新町3-5', {PREF: "埼玉県", CITY: "鶴ヶ島市", TOWN: "新町三丁目", ADDRESS: "5", LEVEL: 3}),
+        ('宮城県加美郡加美町原八幡浦32', {PREF: "宮城県", CITY: "加美郡加美町", TOWN: "原八幡浦", ADDRESS: "32", LEVEL: 3}),
+        ('宮城県塩竈市向ケ丘18－1', {PREF: "宮城県", CITY: "塩竈市", TOWN: "向ケ丘", ADDRESS: "18-1", LEVEL: 3}),
         ('東京都府中市南町6-32', {PREF: "東京都", CITY: "府中市", TOWN: "南町", ADDRESS: "6", LEVEL: 3}),
         # 市制施行
-        ('福岡県筑紫郡那珂川町大字松木4', {PREF: "福岡県", CITY: "那珂川市", TOWN: "松木", ADDRESS: "4", LEVEL: 3}),
+        ('福岡県筑紫郡那珂川町大字松木6-2', {PREF: "福岡県", CITY: "那珂川市", TOWN: "松木六丁目", ADDRESS: "2", LEVEL: 3}),
         # 合併
         ('下都賀郡岩舟町大字静5132番地2', {PREF: "栃木県", CITY: "栃木市", TOWN: "岩舟町静", ADDRESS: "5132-2", LEVEL: 3}),
         # 該当データなし
         ('名古屋市瑞穂区彌富町字月見ケ岡32', {PREF: "愛知県", CITY: "名古屋市瑞穂区", TOWN: "弥富町月見ケ岡", ADDRESS: "32", LEVEL: 3}),
         ('愛知県名古屋市瑞穂区弥富町月見ケ岡32', {PREF: "愛知県", CITY: "名古屋市瑞穂区", TOWN: "弥富町月見ケ岡", ADDRESS: "32", LEVEL: 3}),
         # そのほか
+        ('龍ケ崎市藤ケ丘六丁目32', {PREF: "茨城県", CITY: "龍ヶ崎市", TOWN: "藤ケ丘六丁目", ADDRESS: "32", LEVEL: 3}),
+        ('新潟県北蒲原郡聖籠町大字三賀28', {PREF: "新潟県", CITY: "北蒲原郡聖籠町", TOWN: "大字三賀", ADDRESS: "28", LEVEL: 3}),
         ('宮崎県都城市北原町24', {PREF: "宮崎県", CITY: "都城市", TOWN: "北原町", ADDRESS: "24", LEVEL: 3}),
         ('都城市北原町24', {PREF: "宮崎県", CITY: "都城市", TOWN: "北原町", ADDRESS: "24", LEVEL: 3}),
         ('山梨県都留市上谷一丁目1番1号', {PREF: "山梨県", CITY: "都留市", TOWN: "上谷一丁目", ADDRESS: "1-1", LEVEL: 3}),
         ('広島県安芸郡府中町大通三丁目5番1号', {PREF: "広島県", CITY: "安芸郡府中町", TOWN: "大通三丁目", ADDRESS: "5-1", LEVEL: 3}),
         ('広島県府中市行縢町38', {PREF: "広島県", CITY: "府中市", TOWN: "行縢町", ADDRESS: "38", LEVEL: 3}),
-
+        ('長崎県諫早市東小路町7ｰ1', {PREF: "長崎県", CITY: "諫早市", TOWN: "東小路町", ADDRESS: "7-1", LEVEL: 3}),          
+        ('長崎県諌早市東小路町7ｰ1', {PREF: "長崎県", CITY: "諫早市", TOWN: "東小路町", ADDRESS: "7-1", LEVEL: 3}),
+        
         ### TrueScript版のテスト
         ('大阪府堺市北区新金岡町4丁1−8', {PREF: "大阪府", CITY: "堺市北区", TOWN: "新金岡町四丁", ADDRESS: "1-8", LEVEL: 3}),
         ('大阪府堺市北区新金岡町４丁１ー８', {PREF: "大阪府", CITY: "堺市北区", TOWN: "新金岡町四丁", ADDRESS: "1-8", LEVEL: 3}),
         ('和歌山県串本町串本1234', {PREF: "和歌山県", CITY: "東牟婁郡串本町", TOWN: "串本", ADDRESS: "1234", LEVEL: 3}),
         ('和歌山県東牟婁郡串本町串本1234', {PREF: "和歌山県", CITY: "東牟婁郡串本町", TOWN: "串本", ADDRESS: "1234", LEVEL: 3}),
         ('和歌山県東牟婁郡串本町串本千二百三十四', {PREF: "和歌山県", CITY: "東牟婁郡串本町", TOWN: "串本", ADDRESS: "1234", LEVEL: 3}),
         ('和歌山県東牟婁郡串本町串本一千二百三十四', {PREF: "和歌山県", CITY: "東牟婁郡串本町", TOWN: "串本", ADDRESS: "1234", LEVEL: 3}),
@@ -165,15 +173,15 @@
         ('北海道札幌市中央区北三条西３丁目１－５６マルゲンビル３Ｆ',
          {PREF: "北海道", CITY: "札幌市中央区", TOWN: "北三条西三丁目", ADDRESS: "1-56マルゲンビル3F", LEVEL: 3}),
         ('北海道札幌市北区北２４条西６丁目１−１', {PREF: "北海道", CITY: "札幌市北区", TOWN: "北二十四条西六丁目", ADDRESS: "1-1", LEVEL: 3}),
         ('堺市北区新金岡町4丁1−8', {PREF: "大阪府", CITY: "堺市北区", TOWN: "新金岡町四丁", ADDRESS: "1-8", LEVEL: 3}),
         ('串本町串本1234', {PREF: "和歌山県", CITY: "東牟婁郡串本町", TOWN: "串本", ADDRESS: "1234", LEVEL: 3}),
         ('広島県府中市府川町315', {PREF: "広島県", CITY: "府中市", TOWN: "府川町", ADDRESS: "315", LEVEL: 3}),
         ('府中市府川町315', {PREF: "広島県", CITY: "府中市", TOWN: "府川町", ADDRESS: "315", LEVEL: 3}),
-        ('府中市宮西町2丁目24番地', {PREF: "東京都", CITY: "府中市", TOWN: "宮西町二丁目", ADDRESS: "24", LEVEL: 3}),
+        ('東京都府中市宮西町2丁目24番地', {PREF: "東京都", CITY: "府中市", TOWN: "宮西町二丁目", ADDRESS: "24", LEVEL: 3}),
         ('三重県三重郡菰野町大字大強原2796', {PREF: "三重県", CITY: "三重郡菰野町", TOWN: "大字大強原", ADDRESS: "2796", LEVEL: 3}),
         ('三重県三重郡菰野町大強原2796', {PREF: "三重県", CITY: "三重郡菰野町", TOWN: "大字大強原", ADDRESS: "2796", LEVEL: 3}),
         ('福岡県北九州市小倉南区大字井手浦874', {PREF: "福岡県", CITY: "北九州市小倉南区", TOWN: "大字井手浦", ADDRESS: "874", LEVEL: 3}),
         ('福岡県北九州市小倉南区井手浦874', {PREF: "福岡県", CITY: "北九州市小倉南区", TOWN: "大字井手浦", ADDRESS: "874", LEVEL: 3}),
         ('沖縄県那覇市小禄１丁目５番２３号１丁目マンション３０１',
          {PREF: "沖縄県", CITY: "那覇市", TOWN: "小禄一丁目", ADDRESS: "5-23 一丁目マンション301", LEVEL: 3}),
         ('香川県仲多度郡まんのう町勝浦字家六２０９４番地１',
```

### Comparing `normalize_japanese_address-0.0.8/pyproject.toml` & `normalize_japanese_address-0.0.9/pyproject.toml`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,27 @@
 [tool.poetry]
 name = "normalize_japanese_address"
-version = "0.0.8"
+version = "0.0.9"
 authors = ["SAWADA takahiro <saw@computer.org>"]
 description = "To normalize Japanese address."
 license = "MIT"
 homepage = "https://github.com/fanannan/normalize-japanese-address"
 repository = "https://github.com/fanannan/normalize-japanese-address"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.8"
 kanjize = "^1.0.0"
 mojimoji = "^0.0.11"
 requests = "^2.25.1"
-pytest = "^6.2.4"
 neologdn = "^0.5.1"
 orjson = "^3.5.3"
+pytest = "^6.2.4"
+nose = "^1.3.7"
 
 [tool.poetry.dev-dependencies]
+pytest = "^6.2.4"
+black = {version = "^21.6b0", allow-prereleases = true}
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `normalize_japanese_address-0.0.8/setup.py` & `normalize_japanese_address-0.0.9/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -51,29 +51,28 @@
                                 'japanese_address/api/ja/長崎県/*',
                                 'japanese_address/api/ja/長野県/*',
                                 'japanese_address/api/ja/青森県/*',
                                 'japanese_address/api/ja/静岡県/*',
                                 'japanese_address/api/ja/香川県/*',
                                 'japanese_address/api/ja/高知県/*',
                                 'japanese_address/api/ja/鳥取県/*',
-                                'japanese_address/api/ja/鹿児島県/*'],
- 'normalize_japanese_address.tests': ['.pytest_cache/*',
-                                      '.pytest_cache/v/cache/*']}
+                                'japanese_address/api/ja/鹿児島県/*']}
 
 install_requires = \
 ['kanjize>=1.0.0,<2.0.0',
  'mojimoji>=0.0.11,<0.0.12',
  'neologdn>=0.5.1,<0.6.0',
+ 'nose>=1.3.7,<2.0.0',
  'orjson>=3.5.3,<4.0.0',
  'pytest>=6.2.4,<7.0.0',
  'requests>=2.25.1,<3.0.0']
 
 setup_kwargs = {
     'name': 'normalize-japanese-address',
-    'version': '0.0.8',
+    'version': '0.0.9',
     'description': 'To normalize Japanese address.',
     'long_description': "\nGeolonia様のオープンソースの住所正規化ライブラリ( https://github.com/geolonia/normalize-japanese-addresses )をPythonに移植したものです。\n現在まだ試作段階であり、Geolonia様のもとのライブラリと完全に同じ動作にはなっていません（テストのうち7.2%で失敗）。\nまた、仕様はすぐに変更する可能性があります。\n\n## インストール方法\n\n- Windows環境の場合は、インストールの前に環境変数を設定してください\n```\nset PYTHONUTF8=1\n```\n\n```\npip install --upgrade normalize_japanese_address\n```\n\n## 使い方\n```python\nfrom normalize_japanese_address.normalize import normalize\n\nresult = normalize('大阪府堺市北区新金岡町4丁1−8')\nprint(result)\n```\n\nとすると、resultに\n```python\n{'pref': '大阪府', 'city': '堺市北区', 'town': '新金岡町四丁', 'address': '1-8', 'level': 3}\n```\nを返します。levelは、住所文字列のどこまでを判別できたかを以下の数値で示しています。\n\n* `0` - 都道府県も判別できなかった。\n* `1` - 都道府県まで判別できた。\n* `2` - 市区町村まで判別できた。\n* `3` - 町丁目まで判別できた。\n\n## ライセンス、利用規約\n- 本プログラムは、下記のプログラムをもとに開発されています。住所データのライセンスは CC BY 4.0、それ以外はMITとされており、本プログラムもそれに従います。\n\nhttps://github.com/geolonia/normalize-japanese-addresses\nhttps://github.com/geolonia/japanese-addresses\n",
     'author': 'SAWADA takahiro',
     'author_email': 'saw@computer.org',
     'maintainer': None,
     'maintainer_email': None,
     'url': 'https://github.com/fanannan/normalize-japanese-address',
```

### Comparing `normalize_japanese_address-0.0.8/PKG-INFO` & `normalize_japanese_address-0.0.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: normalize-japanese-address
-Version: 0.0.8
+Version: 0.0.9
 Summary: To normalize Japanese address.
 Home-page: https://github.com/fanannan/normalize-japanese-address
 License: MIT
 Author: SAWADA takahiro
 Author-email: saw@computer.org
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Requires-Dist: kanjize (>=1.0.0,<2.0.0)
 Requires-Dist: mojimoji (>=0.0.11,<0.0.12)
 Requires-Dist: neologdn (>=0.5.1,<0.6.0)
+Requires-Dist: nose (>=1.3.7,<2.0.0)
 Requires-Dist: orjson (>=3.5.3,<4.0.0)
 Requires-Dist: pytest (>=6.2.4,<7.0.0)
 Requires-Dist: requests (>=2.25.1,<3.0.0)
 Project-URL: Repository, https://github.com/fanannan/normalize-japanese-address
 Description-Content-Type: text/markdown
```

