<!-- ELUCENIA technical documentation · indice-prognostico-de-nottingham · ja · no clinical/professional/rights approval -->

# Nottingham予後指数（NPI）

[条件・出典・許諾](https://elucenia.org/ja/tools/indice-prognostico-de-nottingham)

## 使い方

ポータルでツールを使用するか、ローカルHTTPサーバー経由でindex.htmlを開いてください。言語を選択し、項目を入力して計算してください。

## 入力項目と単位

### 浸潤性腫瘍の最大径（病理）

`tam`

cm · 範囲: 0.1–20

### 腋窩リンパ節

`lnd`

- `1` — 陰性
- `2` — 1～3個陽性
- `3` — 4個以上陽性

### 組織学的グレード（Nottingham/Elston-Ellis）

`grau`

- `1` — グレード 1
- `2` — グレード 2
- `3` — グレード 3

## 方法の版

NPI/Haybittle 1982/Galea 1992：0.2径cm+リンパ節1–3+グレード1–3

## 記載された計算式

NPI=0.2×径（cm）+リンパ節段階（1–3）+組織学的グレード（1–3）。

リンパ節段階：1=転移なし；2=1–3個；3=4個以上（原記載では腋窩頂部・内胸リンパ節転移も含む）。

## 限界・対象集団

NPIは、原発性乳がんの病理学的特徴を予後と関連付けます。合計には正しく定義されたリンパ節病期とグレードが必要です。現在の治療を決めるものではなく、個人の生存も保証しません。式、群、率は使用する版と集団に対応する必要があります。

## 参考文献

- [Haybittle JL et al. A prognostic index in primary breast cancer. Br J Cancer, 1982.](https://doi.org/10.1038/bjc.1982.62)

- [Galea MH et al. The Nottingham prognostic index in primary breast cancer. Breast Cancer Res Treat, 1992.](https://doi.org/10.1007/BF01840834)

- [Blamey RW et al. Survival of invasive breast cancer according to the Nottingham Prognostic Index in cases diagnosed in 1990-1999. Eur J Cancer, 2007.](https://doi.org/10.1016/j.ejca.2007.01.016)

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
