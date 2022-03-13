# コンペについて

## 気が付いたこと

* ladysのウェアが多い。
* Jersey funcyというブランドの売上が多い。


## 分からない特徴量

* customer.csvのFN, Active


* 協調フィルタリングメモ　https://receiptreward.jp/solution/column/collaborativefiltering.html
　- 協調フィルタリングには、3種類ある。
    - メモリベース、モデルベース、ハイブリッド
    - 今回はメモリベースの手法が適していると思う。
    - ただ、購入回数が少ない人は、メモリベースだと上手く購買特性を捉えられないと思うので、コンテンツベースフィルタリングを組み合わせたハイブリットベースが良いかも
        - メモリベースとハイブリットベースを購買頻度に応じて重み付してアンサンブルすると良いかも。

## やりたいことメモ

* EDAの方針
    - 個人ベースで見てみる。。
* 予測
    - public notebookにあるヒューリスティックな方法のモデルと、協調フィルタリングモデルを作りアンサンブルしたい。
    - 

## 役に立ちそうなリンク

 * レコメンドに画像の情報を活用する方法: https://techblog.zozo.com/entry/visual_recommend
 * AI による商品購買予測とアソシエーション分析:　https://www.murc.jp/wp-content/uploads/2020/12/cr_201204.pdf
    - 参考にしていたnotebook: https://www.kaggle.com/paulantoine/light-gbm-benchmark-0-3692/script ([Instacart Market Basket Analysis](https://www.kaggle.com/c/instacart-market-basket-analysis/overview/evaluation))


## 評価指標メモ

MAP@12
* 予測は一人の客に対し12件まで。
* testの週に何も買わなかった人は、評価の際に除外される。
* 関連していたらrel(K)が1になり、P(K)が加算される。
    - rel()では、商品名、色、カテゴリ等正解にある商品と関連していたら1になると思う。
    - P()では、商品名、商品種別、色等の要素が正解に近いほど高くなる感じだと思う。⇒IDから
* 実際に購入された商品数以上に多く予測しすぎてもペナルティはない。
*  P(k) is the precision at cutoff kは、

<br>

# ノートブックまとめ

## ノートブック[Recommend Items Purchased Together - [0.021]](https://www.kaggle.com/cdeotte/recommend-items-purchased-together-0-021) のメモ

1.最終購入日の1週間前から最終購入日までに買われた商品、2.1の商品と良く一緒に買われる商品、3. 人気商品12個の3つを次の週の購入予測商品としている。

## それぞれについてメモ
1. 最終購入日の1週間前から最終購入日までに買われた商品
    - 人によっては最終購入日が1年前。⇒ 1年間前買ったものを急にまた買うとはおもえない。
    - 代替案
        - 全期間で最も買われた商品上位5商品
        - あまり購入品が少ない人は、入れない。
2. 1の商品と良く一緒に買われる商品
    - 全ての商品を購入回数でソートして、上位1,000から1,030までの商品を買ったユーザが買った商品頻度順最大上位3つ。
        - なんで上位1,000から1,030なのかイマイチ分からない。
3. 人気商品12個
    - 購入回数が上位12。

## 改善案

* 1の商品を抜いて、2,3のみにする。
* 期間を1週間から、1年くらいに変える。
* 2の所を変える。
* テストデータの1年前に買った商品とその関連商品を入れる。

<br>

## ノートブック[Recommend Items Purchased Together - [0.021]](https://www.kaggle.com/cdeotte/recommend-items-purchased-together-0-021) のメモ