<!-- ELUCENIA technical documentation · scorad · ja · no clinical/professional/rights approval -->

# SCORAD

[条件・出典・許諾](https://elucenia.org/ja/tools/scorad)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 範囲（A）：9の法則による罹患面積

`area`

% · 範囲: 0–100

### 紅斑

`eritema`

- `0` — 0 なし
- `1` — 1 軽度
- `2` — 2 中等度
- `3` — 3 強い

### 浮腫・丘疹

`edema`

- `0` — 0 なし
- `1` — 1 軽度
- `2` — 2 中等度
- `3` — 3 強い

### 滲出・痂皮

`exsudacao`

- `0` — 0 なし
- `1` — 1 軽度
- `2` — 2 中等度
- `3` — 3 強い

### 掻破痕

`escoriacao`

- `0` — 0 なし
- `1` — 1 軽度
- `2` — 2 中等度
- `3` — 3 強い

### 苔癬化

`liquen`

- `0` — 0 なし
- `1` — 1 軽度
- `2` — 2 中等度
- `3` — 3 強い

### 皮膚乾燥（病変のない皮膚）

`xerose`

- `0` — 0 なし
- `1` — 1 軽度
- `2` — 2 中等度
- `3` — 3 強い

### 過去3日間のそう痒（0～10）

`prurido`

範囲: 0–10

### 過去3日間の睡眠障害（0～10）

`sono`

範囲: 0–10

## 方法の版

SCORAD/ETFAD 1993：範囲/5+3.5強度+症状、客観的はCなし、Oranje 2007閾値

## 記載された計算式

SCORAD = A/5 + 7B/2 + C; A = 範囲 (0–100%), B = 6強度の合計 (0–18), C = かゆみ+睡眠喪失 (0–20). 最大： 103.

客観的SCORAD = A/5 + 7B/2 (最大： 83).

## 限界・対象集団

SCORADはアトピー性皮膚炎の重症度を測定し、徴候、広がり、主観症状の評価に依存します。元の開発には訓練された評価者が参加し、合計点で疾患の診断を確立するものではありません。客観的SCORAD、完全な指数、後年の閾値には、それぞれの定義と出典が必要です。

## 参考文献

- [European Task Force on Atopic Dermatitis. Severity scoring of atopic dermatitis: the SCORAD index. Dermatology, 1993.](https://doi.org/10.1159/000247298)

- [Kunz B et al. Clinical validation and guidelines for the SCORAD index: consensus report of the European Task Force on Atopic Dermatitis. Dermatology, 1997.](https://doi.org/10.1159/000245677)

- [Oranje AP et al. Practical issues on interpretation of scoring atopic dermatitis: the SCORAD index, objective SCORAD and the three-item severity score. Br J Dermatol, 2007.](https://doi.org/10.1111/j.1365-2133.2007.08112.x)

## 技術テストの再現

このリポジトリのルートディレクトリでnode test.cjsを実行すると、記録された合成ケースを再実行できます。元の入力、期待結果、許容誤差は保持されています。技術テストは臨床的検証を意味しません。

```sh
node test.cjs
```

tool.jsonには出典、版、確認範囲が記録されています。examples.jsonには合成入力と期待結果が保持され、results.jsonには実際に得られた結果が記録されています。

[記録・参考文献](../tool.json) · [JavaScriptコード](../calculator.js) · [参照ケース](../examples.json) · [results.json](../results.json)

## 確認状況と使用条件

独立した臨床レビューは実施されていません。

このインターフェースは独自に作成した翻訳であり、公式版や認証済みの版ではありません。独立した臨床レビュー、専門家による言語レビュー、評価尺度等の権利許諾の確認は実施されていません。

式または分類の結果です。解釈、対応、適用可能性は専門家による評価と選択した出典に依存します。

## ライセンスと帰属表示

Apache-2.0はELUCENIAのコードにのみ適用されます。評価尺度等、出版物、翻訳、データの権利は、それぞれの権利者に帰属します。LICENSEとNOTICEを保持してください。

ELUCENIA · Felipe Guedes · Copyright © 2026
