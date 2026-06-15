*This project has been created as part of the life by KENTARO SADAYASU*

# -_loadto-
データ解析とPythonに関して学ぶためのリポジトリ。

## Data Science Learning
(データサイエンス学修リポジトリ)

データサイエンスの基礎および Python を用いたデータ解析のプロセスを学び、実践するためのリポジトリです。  
実行環境には主に Google Colab を想定しています。

## 学習の流れ

このリポジトリでは、データ解析を「表の扱い」から「可視化」、「回帰分析」へと少しずつ段階的に学んでいきます。

1. `Pandas_Step1.ipynb`
   - `pd.DataFrame` を用いた構造化データの生成
   - `.loc` によるラベル指定
   - `.iloc` によるインデックス番号指定
   - 列同士のベクトル演算による新しい特徴量の生成

2. 回帰分析の基礎
   - 散布図による相関の確認
   - 平均値を基準にした4象限の見方
   - `np.polyfit()` を使った単回帰分析
   - 傾きと切片を用いた未来予測

3. 重回帰分析への発展
   - 説明変数を1つから複数へ広げる
   - `sklearn.linear_model.LinearRegression` を使った学習
   - `coef_` と `intercept_` の確認
   - 予測値と誤差の確認
   - `X`（説明変数）と `y`（目的変数）の役割の理解
   - `fit(X, y)` でデータから式を学習し、`predict(X)` で予測する流れの理解
   - `df["誤差"].abs().mean()` による誤差の大きさの確認
   - `get_dummies()` を使ったカテゴリデータ（天気など）の数値化
   - `drop_first=True` によるダミー変数の基準列の扱いの理解
   - 学習時の列と予測時の列を `reindex()` でそろえる考え方の理解
   - 実データを使った1件予測の実践

## 学習で意識していること

- C言語との違いを対比しながら理解する
- 数学だけでなく、まずコードを動かして結果を見る
- `print` よりも、データ構造そのものの意味を重視する
- 1行で書かれた処理を分解して理解する

## 動作環境

- 言語: Python 3.x
- 主要ライブラリ: Pandas, NumPy, Matplotlib, scikit-learn
- 開発環境: Google Colaboratory / VS Code

## 今後の方針

- 第5回以降の重回帰分析を進める
- `student-math.csv` や `student-por.csv` を使った実データでの重回帰を深める
- 天気や曜日などのカテゴリデータの扱いを学ぶ
- クラスタ分析や主成分分析にもつなげる
