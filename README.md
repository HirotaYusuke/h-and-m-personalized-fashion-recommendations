# h-and-m-personalized-fashion-recommendations

Kaggle [H&M Personalized Fashion Recommendations](https://www.kaggle.com/c/h-and-m-personalized-fashion-recommendations) に参加．


## Member

チーム名 しまむら

* Hirota Yusuke
* Hiroshige Aoki

## Overview

### Description


[H&Mグループ](https://www.hmgroup.com/)は，53のオンラインマーケットと約4,850の店舗を持つブランドとビジネスのファミリーです．オンラインストアでは，買い物客に豊富な品揃えの中から好きなものを選んでもらうことができます．しかし，選択肢が多すぎるとお客様は興味のあるものや探しているものをすぐに見つけることができず，最終的に購入に至らないこともあります．ショッピング体験を向上させるためには，商品のレコメンデーションが重要な鍵となります．さらに重要なことは，お客様の正しい選択を支援することは，返品を減らし，それによって輸送に伴う排出を最小限に抑えるという，サステナビリティにも良い影響を与えるということです．

このコンペティションでは，H&Mグループが過去の取引データ，および顧客と商品のメタデータを基にした商品推奨を開発することを募集しています．メタデータは，衣服の種類やお客様の年齢などの単純なものから，商品説明のテキストデータ，衣服画像の画像データなど，多岐にわたります．


### Evaluation


Submissions are evaluated according to the Mean Average Precision @ 12 (MAP@12):

![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/400/004D.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/400/0041.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/400/0050.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Main/Regular/400/0040.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Main/Regular/400/0031.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Main/Regular/400/0032.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Main/Regular/400/003D.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Main/Regular/400/0031.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/400/0055.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Size2/Regular/400/2211.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/283/0075.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Main/Regular/283/003D.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Main/Regular/283/0031.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/283/0055.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Size2/Regular/400/2211.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/283/006B.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Main/Regular/283/003D.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Main/Regular/283/0031.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/283/006D.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/283/0069.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/283/006E.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Main/Regular/283/0028.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/283/006E.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Main/Regular/283/002C.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Main/Regular/283/0031.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Main/Regular/283/0032.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Main/Regular/283/0029.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/400/0050.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Main/Regular/400/0028.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/400/006B.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Main/Regular/400/0029.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Main/Regular/400/00D7.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/400/0072.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/400/0065.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/400/006C.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Main/Regular/400/0028.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/400/006B.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Main/Regular/400/0029.png?V=2.7.9)MAP@12=1U∑u=1U∑k=1min(n,12)P(k)×rel(k)

where ![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/400/0055.png?V=2.7.9)U is the number of customers, ![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/400/0050.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Main/Regular/400/0028.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/400/006B.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Main/Regular/400/0029.png?V=2.7.9)P(k) is the precision at cutoff ![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/400/006B.png?V=2.7.9)k, ![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/400/006E.png?V=2.7.9)n is the number predictions per customer, and ![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/400/0072.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/400/0065.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/400/006C.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Main/Regular/400/0028.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/400/006B.png?V=2.7.9)![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Main/Regular/400/0029.png?V=2.7.9)rel(k) is an indicator function equaling 1 if the item at rank ![](https://www.kaggleusercontent.com/static/mathjax/2.7.9/fonts/HTML-CSS/TeX/png/Math/Italic/400/006B.png?V=2.7.9)k is a relevant (correct) label, zero otherwise.

**Notes:**

* 学習データから，購入したかどうかに関わらず，提供されたすべてのcustomer_idの値に対して購入予測を行う．
* テスト期間中に購入しなかった顧客は，得点の対象から除外される．
* 12個未満の注文の顧客に対して，12個の予測をフルに使ってもペナルティはない．したがって，顧客ごとに12個の予測をするのが有利である．


### Timeline


* **2022/02/07** - コンペティション開始日
* **2022/05/09** - コンペティション終了日


## Data

この課題では，顧客の購入履歴とそれを裏付けるメタデータが与えられる．このコンペティションでは，学習データが終了した直後の7日間に，各顧客がどのような記事を購入するかを予測する．その間に何も購入しなかった顧客は、スコアリングから除外される．

**Files**

* **images/** - 各 article_id に対応する画像のフォルダ．画像は，article_id の最初の 3 桁で始まるサブフォルダに配置される．ただし，すべての article_id 値が対応する画像を持つわけではない．
* **articles.csv** - 購入可能な各article_idの詳細メタデータ．
* **customers.csv** - データセットの各顧客IDのメタデータ
* **transactions_train.csv** - 各顧客が各日付で購入した商品とその追加情報からなる学習データである．重複する行は，同じ商品を複数回購入したことに対応する．このコンペティションでは，各顧客が学習データ期間の直後の7日間に購入するarticle_idを予測することである．
