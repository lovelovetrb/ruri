---
marp: true
theme: ruri
paginate: true
header: 'プレゼンタイトルや発表名など'
footer: 'イベント名やCopyrightなど'
---

<!-- _class: title -->

# テーマタイトル
## サブタイトル・著者名など
### 2026-03-22

---

<!-- _class: lead -->

# 第1章
## チャプタータイトル

---

# 見出しレベル1（h1）

## 見出しレベル2（h2）

### 見出しレベル3（h3）

本文テキストのサンプルですわ。日本語と English が混在するケースも想定しています。
**太字テキスト**、*イタリック*、`インラインコード` の表示確認です。

---

# 箇条書き・リスト

## 順序なしリスト

- 第1項目
  - ネストされた項目
  - ネストされた項目2
- 第2項目
- 第3項目

## 順序付きリスト

1. ステップ1
2. ステップ2
   1. サブステップA
   2. サブステップB
3. ステップ3

---

# テーブル

| 列A | 列B | 列C |
|---|---|---|
| セル1 | セル2 | セル3 |
| セル4 | セル5 | セル6 |
| セル7 | セル8 | セル9 |

## 左・中央・右寄せ

| 左寄せ | 中央寄せ | 右寄せ |
|:---|:---:|---:|
| Left | Center | Right |
| テキスト | テキスト | テキスト |

---

# コードブロック

## インラインコード

変数 `x` に値を代入するには `x = 42` と書きます。

## ブロックコード（Python）

```python
def sentiment_direction(activations: list[float]) -> float:
    """Compute projection onto sentiment direction."""
    mean_pos = sum(activations[:len(activations)//2])
    mean_neg = sum(activations[len(activations)//2:])
    return mean_pos - mean_neg
```

## ブロックコード（bash）

```bash
marp --theme ruri.css --html slides.md -o slides.html
```

---

# 数式（KaTeX）

## インライン数式

残差ストリームの更新式は $\boldsymbol{x}_t^{L} = \boldsymbol{x}_t^{0} + \sum_{\ell=0}^{L-1}(\text{Attn}_\ell + \text{MLP}_\ell)$ で表されます。

## ディスプレイ数式

$$
\boldsymbol{o}_{\text{patched}} = \boldsymbol{o}_{\text{orig}}
  - (\boldsymbol{o}_{\text{orig}} \cdot \boldsymbol{d})\,\boldsymbol{d}
  + (\boldsymbol{o}_{\text{new}} \cdot \boldsymbol{d})\,\boldsymbol{d}
$$

$$
\text{Mean Difference} = \frac{1}{|\mathbb{P}|}\sum_{p \in \mathbb{P}} \boldsymbol{a}_p
  - \frac{1}{|\mathbb{N}|}\sum_{n \in \mathbb{N}} \boldsymbol{a}_n
$$

---

# 引用・強調

> これは引用ブロックのサンプルです。重要な定義を引用する際に使います。

---

## テキスト強調パターン

- **太字**で重要なキーワードを強調
- *イタリック*で用語・タイトルを示す
- ~~取り消し線~~で削除・修正を表現

---

# 2カラムレイアウト

<div style="display: grid; grid-template-columns: 1fr 1fr; gap: 2em;">

<div>

### 左カラム

- ポイントA
- ポイントB
- ポイントC

</div>

<div>

### 右カラム

| 項目 | 値 |
|---|---|
| 精度 | 89% |
| F1 | 0.91 |

</div>
</div>

---

# まとめスライド

## 主要な発見

1. **発見1** — 説明テキスト
2. **発見2** — 説明テキスト
3. **発見3** — 説明テキスト

## 方法論的な教訓

- 相関 → 因果の二段階検証が重要
- 複数手法の三角測量で実在性を担保

---

<!-- _class: lead -->

# ご清聴ありがとうございました

---

# 参考文献

- Author et al. (2023) "Paper Title" — 説明
- Author et al. (2022) "Paper Title" — 説明
- Author et al. (2021) "Paper Title" — 説明
