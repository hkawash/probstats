# 前半で押さえておきたいポイント

- 用語とその意味内容については重点的に復習し，説明できるようにしておくこと．
- [(トップページへ戻る)](index)

## 第9回

- 第一種の過誤と第二種の過誤の意味
  - 両者はトレードオフ
  - 検出力
- 抽出方法
  - 多段抽出，系統抽出，層化抽出，クラスタ(集落)抽出
- 代表的なバイアスとその意味
  - 選択バイアス，交絡，情報バイアス
- エビデンスレベル
  - ランダム化比較試験 (RCT)，コホート研究，ケース・コントロール研究
- フィッシャーの三原則
  - 反復，無作為化，局所管理（この意味）
  - 乱塊法 (randomized block design)
- バイアスへの対応
  - 選択バイアスへの対応 - ランダム化（無作為化），マッチング
  - 交絡への対応 - 交絡因子による層別化
  - 情報バイアスへの対応 - 盲検法

## 第10回

- 標本比率はどのような分布になるか？（標本抽出を仮想的に何度も行ったとき）
  - コイン投げのモデルとは？
  - 平均，分散，および分布は？（母数 $p$，標本サイズ $n$を用いて表すことができるか？）
  - 標本比率も標本平均の一種
- 母比率の差の検定（二つの母比率に差があるか？）
  - 帰無仮説は？
  - 標本比率の差の従う分布は？
  - 検定統計量 $Z$はどう計算する？
  - $Z$の分母の計算に必要な $p$ は，2群の度数の合計から推定
- 母比率の区間推定，母比率の差の区間推定
  - 母比率の区間推定：観測された比率 $\pm$ 1.96標準誤差
  - 母比率の差の区間推定：観測された比率の差 $\pm$ 1.96標準誤差
  - 式は覚えなくてもよいが標準誤差の導出の流れは見ておく

## 第11回

- 適合度のカイ二乗検定と独立性のカイ二乗検定のそれぞれにおいて，以下が分かるか？
  - 帰無仮説は？
  - 期待度数の計算ができるか？
  - 標本の観測度数が与えられた時に $\chi^2$ 値はどう計算する？
  - どの自由度のカイ二乗分布を考えればよいか？
    - （例）$r \times c$ の分割表で独立性の検定を行う場合の自由度は？
  - $\chi^2$分布のパーセント点の表が与えられた時に，標本から計算された$\chi^2$より帰無仮説を棄却するか否かが判定できるか？
- 分割表における独立性の意味は？
  - 分割表から2つの事象の同時確率や条件付き確率が計算できるか？

## 第12回

- 第一種の過誤，第二種の過誤と標本サイズの関係
  - 第一種の過誤，第二種の過誤を説明できるか？
  - $\chi^2$分布を例に，$\alpha$や$\beta$がどのような確率かを説明できるか？
  - 検出力を説明できるか？
  - 標本サイズと$\alpha$や$\beta$の関係について説明できるか？
  - 帰無仮説が誤りであり，実際には差があるとする．同じ検出力を実現するには，差が小さいほど$n$はどうすればよい？
- 区間推定で，実現したい区間の幅が与えられた時に，必要となる$n$を計算できるか？
- フィッシャーの正確検定は超幾何分布を使う
  - フィッシャーの正確検定はどのようなときに用いるか？
  - 超幾何分布とはどのような分布か？

## 第13回

- 相関と回帰の違い
- 相関係数および共分散の定義
- 無相関検定の考え方：標本相関係数$r$から統計量$t$ を計算する式，および具体的な$r$の値が与えられた時に，無相関検定ができるか？
  - 帰無仮説は？
  - 適切な自由度の選択ができるか？
    - 自由度$n-2$の$t$分布を利用すること．例：$n=54$なら自由度52など
  - 基本は両側検定を用いること
  - その他，$t$検定の基本を知っているか？（前半の復習）
    - $t$が棄却域にはいるか or $p$値が有意水準より小さいか
    - 帰無仮説が棄却できたとき，できなかったときの，それぞれの結論
- （試験範囲からは外しますが）相関係数の区間推定ではFisherの$z$変換を使う
- スピアマンの順位相関係数
  - 考え方：順位に変換してから通常の相関係数を用いること
  - 通常の相関係数はピアソンの積率相関係数と呼ぶことなども
- そのほか相関に関すること
  - 2変数に関係があるけど無相関な例（$y=x^2$など）
  - 相関関係は因果関係を含意しない
  - 見かけ上の相関（第9回も参照のこと）
- 単回帰分析における最小二乗法の考え方
  - 何を最小化するのか？
    - 残差とは？
  - 回帰係数の求め方
    - 少なくとも切片での偏微分とそこから得られる式 $a = \bar{y} - b\bar{x}$
    - 傾きは「$x$と$y$の共分散」を「$x$の分散」で割ったものと一致

## 第14回

- 重回帰とは何か?
- 3次元散布図の見方
- 決定係数 $R^2$ は回帰式全体の性能を見る
  - 目的変数の変動 $\sum_i (y_i - \bar{y})^2$ を，回帰式で何パーセント説明できているかを表す
  - 自由度調整済み決定係数は，言葉としては知っておこう
- 回帰係数の検定
  - 母回帰式を考える
  - 帰無仮説は，母回帰式の回帰係数（母回帰係数）がゼロ
- 多項式回帰とは何か?
- ダミー変数とは何か?
  - 質的変数を説明変数に入れる時に用いる 0, 1のいずれかの値を取る変数
  - 質的変数の値によって，モデル（切片，もしくは切片と傾きの両方）が切り替わる
- ロジスティック回帰
  - シグモイド関数が最後にかかる
  - 目的変数が(2値の)質的変数の場合に利用できる

## 第15回（試験範囲外）

