# Wacker#30

---

<div align="left">
  <small>
  Wacker #30　2018/08/20(日) <br>
  </small>
</div>

<br>

### 機械学習 Google ColaboratoryでKaggleの課題チャレンジ

<div>
  ![画像](img/top.jpg)
</div>

<br>

<div align="right"> Yohei Taniguchi </div>

<div align="right">
  <small>

    [Wacker](http://wacker.io/)

  </small>
</div>

<div align="right">

  [![CC BY-SA 4.0](https://i.creativecommons.org/l/by-sa/4.0/88x31.png "CC BY-SA 4.0")](http://creativecommons.org/licenses/by-sa/4.0/)

</div>

---

## はじめに <hr>

- 前回に引き続き、機械学習のハンズオンを行います。今回はKaggleチュートリアル「タイタニック生存者予測」を行います。

---

## 環境<hr>

- GoogleColablatory
- Kaggleアカウント
- Kaggleチュートリアル「Titanic: Machine Learning from Disaster」
  - https://www.kaggle.com/c/titanic

---

## GoogleColablatoryとは<hr>

- Colaboratory は、機械学習の教育や研究に利用できる研究ツールです。特別な設定なしで、Jupyter Notebook 環境をご利用いただけます。
- JupyterをWeb上で利用・共有できるようにしたもの

---

## Kaggleとは<hr>

- Kaggleは企業や研究者がデータを投稿し、世界中の統計家やデータ分析家がその最適モデルを競い合う、予測モデリング及び分析手法関連プラットフォーム及びその運営会社である。

参考: https://ja.wikipedia.org/wiki/Kaggle


---

## AIと機械学習 <hr>

---

### 強いAIと弱いAI<hr>

- 強いAI = 人間の知能そのものをもつ機械を作ろうとする立場
- 弱いAI = 人間が知能を使ってすることを機械にさせようとする立場

---

### 研究分野<hr>

![研究分野](./img/overview.jpg)

参照：人工知能学会 What's AIより

---

### 機械学習の機能の種類 <hr>

![](img/scikit-learn.png)

参考：Scikit-Learn

---

#### 分類（classification）

与えられたデータがどのクラスに属するかを判別するものです。教師あり学習の分類問題を解くアルゴリズムと表現できます。

---

#### 回帰（regression）

与えられたデータをもとに、目的とする値を予測するものです。教師あり学習の回帰問題を解くアルゴリズムと表現できます

---

#### クラスタリング（clustering）

与えられたデータを、なんらかの規則に則って分けるものです。教師なし学習のクラスタリング問題を解くアルゴリズムと表現できます

---


### 機械学習の学習方法<hr>

- 機械学習によって、人が行う学習と推論によって、分類と推測を行う

 1. 教師なし
 2. 教師あり
 3. 強化学習

---

### 教師なし <hr>

未知のデータや新たなデータ構造の発見を行う

- K平均法

![K平均法](img/kmeans.png)

---

### 教師あり <hr>

事前の学習データを元に分類、推測を行う手法

- 決定木、ランダムフォレスト
- パーセプトロン、ニューラルネットワーク

![教師あり](img/teacher.png)

---

### 強化学習 <hr>

教師あり学習で行った結果に良い悪いの重み付けをして行う手法

- Q学習
- CPにゲームをさせるケースに使われる

![](img/trophy_school_girl.png)


---

### 機械学習の手法 <hr>

---

#### 決定木<hr>

- 決定木（けっていぎ、英: decision tree）は、（リスクマネジメントなどの）決定理論の分野において、 決定を行う為のグラフであり、計画を立案して目標に到達するために用いられる。 決定木は、意志決定を助けることを目的として作られる。 決定木は木構造の特別な形である。

![](img/Decision_tree_model_ja.png)

---

#### ランダムフォレスト<hr>

- 決定木を弱学習器とする集団学習アルゴリズム
- 弱学習器＝精度の高くない学習器
- 集団（アンサンブル）学習：多数決などで最終的な予測を行うもの

---

#### MLP（多層パーセプトロン）<hr>

![](img/MLP.png)

---

#### CNN（畳み込みニューラルネット）1/3 <hr>

![](img/convolve.png)

---

#### CNN（畳み込みニューラルネット）2/3 <hr>

![](img/lena.jpg)

---

#### CNN（畳み込みニューラルネット）3/3 <hr>

![](img/CNN.jpg)

---

#### RNN（再帰型ニューラルネット）<hr>

文字入力の候補を予測して出す

![](img/SimpleRNN01.jpg)

---

## プログラミングにおける機械学習のフレームワーク <hr>

---

### フレームワーク <hr>

- [TensorFlow](https://www.tensorflow.org/?hl=ja)
- [Keras](https://keras.io/ja/)
- [sklearn](http://scikit-learn.org/)

---

### その他、主なフレームワーク <hr>

- [CNTK](https://docs.microsoft.com/ja-jp/cognitive-toolkit/):MS,C++,Python
- [Chainer](https://chainer.org/):Preferred Networks,Python
- [Pytorch](https://pytorch.org/):FB + NVIDIA,Python,ChainerのForkでCaffe2とマージ

---

#### 主なデータセット <hr>

- [Kaggle](https://www.kaggle.com/)
- [UCI](http://archive.ics.uci.edu/ml/index.php)
- [datamarket](https://datamarket.com/data/)
- スクレイピング

---

## チュートリアル <hr>

---

### Cats vs. Dogs <hr>

https://www.kaggle.com/c/skoltech-cats-vs-dogs/data

---

### MNIST <hr>

- 60,000点の訓練データ(mnist.train)と10,000点のテストデータ(minist.test)

---

### ハンズオン:Taitanic生存者予測 <hr>

- [Titanic: Machine Learning from Disaster](https://www.kaggle.com/c/titanic)

---

## 参考情報

- [Google Colaboratory](https://colab.research.google.com/)
- [Google Colaboratory Github](https://github.com/googlecolab)

- [いちばんやさしいディープラーニング入門](https://www.amazon.co.jp/%E3%81%84%E3%81%A1%E3%81%B0%E3%82%93%E3%82%84%E3%81%95%E3%81%97%E3%81%84-%E3%83%87%E3%82%A3%E3%83%BC%E3%83%97%E3%83%A9%E3%83%BC%E3%83%8B%E3%83%B3%E3%82%B0-%E5%85%A5%E9%96%80%E6%95%99%E5%AE%A4-%E8%B0%B7%E5%B2%A1-%E5%BA%83%E6%A8%B9/dp/4800711878)

- 人工知能学会 What's AI : [http://www.ai-gakkai.or.jp/whatsai/AIresearch.html](http://www.ai-gakkai.or.jp/whatsai/AIresearch.html)
- [kaggle](https://www.codexa.net/what-is-kaggle/)
- https://www.kaggle.com/kojitakahashi6/titanic-koji
- https://www.codexa.net/kaggle-titanic-beginner/
