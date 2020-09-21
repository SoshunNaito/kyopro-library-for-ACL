# kyopro-library-for-ACL
ACLをさらに使いやすくしたライブラリです

- mod.cpp
	- MODの値に応じて、atcoder::static_modint<MOD>をmintとして使えます。<br>
	標準入出力に対応していたり、四則演算が比較的自由だったり、負のpowに対応していたり、小さい値ならO(1)でinv()が求められたりします。


- segtree.cpp
	- BIT: fenwick_treeをラッピングしました。<br>
	vectorによる初期化ができるほか、一点取得、一点更新がO(logN)でできます。
	- SegmentTree: (データ型、初期値、マージする関数)について、いくつかプリセットを用意してあります。<br>
	テンプレートの引数を事前に書いているため、宣言が楽になります。
	- LazySegmentTree: SegmentTree用のデータと、LazySegmentTree用の作用素のデータについて、いくつかプリセットを用意してあります。<br>
	こちらもテンプレートの引数を事前に書いているため、宣言が楽になります。
