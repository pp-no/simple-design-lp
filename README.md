# デザインまるっと便 LP

バナー・LP・パンフレット・Webサイトのデザイン制作サービス「デザインまるっと便」のランディングページです。

Claude Design でモックアップを作成し、Claude Code で実装しました。

## 技術スタック

- **HTML / CSS / JavaScript** — フレームワーク不使用、バニラで実装
- **Google Fonts** — Noto Sans JP / Quicksand / Caveat
- **アセット** — Claude Design からエクスポートした素材画像（`assets/` 以下）

## ページ構成

| セクション | 内容 |
|---|---|
| Header | スティッキーナビ、資料DL・無料相談ボタン |
| Hero | キャッチコピー、人物イラスト、モニターアート |
| Ticker | サービス名の無限スクロール帯 |
| Problems | お悩み4パターン（カードグリッド） |
| Reasons | 選ばれる3つの理由 |
| Flow | ご利用の流れ（6ステップ） |
| Works / Voice | 制作実績 + お客様の声（2カラム） |
| Pricing | 料金プラン3種（スタンダード強調） |
| FAQ + CTA | よくある質問 + ピンクの問い合わせカード |
| Footer | イエロー背景、電話番号、ナビリンク |

## カラーパレット

| 変数 | カラーコード | 用途 |
|---|---|---|
| `--pink` | `#FF4D8F` | メインアクセント、CTAボタン |
| `--yellow` | `#FFD93D` | サブアクセント、フッター背景 |
| `--teal` | `#3DCCC7` | アイコン、チェックマーク |
| `--blue` | `#BCDDFF` | 背景装飾 |
| `--ink` | `#1F2937` | 本文テキスト |

## フォント

- **Noto Sans JP** — 本文・見出し（和文）
- **Quicksand** — 数字・英字アクセント（丸みのあるサンセリフ）
- **Caveat** — ヒーローのモニター内手書きテキスト

## ディレクトリ構成

```
simple-design-lp/
├── index.html        # メインページ（全セクション込み）
└── assets/           # 画像素材（90点）
    ├── illust_*.png  # 人物・キャラクターイラスト
    ├── deco_*.png    # 装飾パーツ（星・雲・ドットなど）
    ├── step_*.png    # ご利用の流れ用画像
    ├── reason_*.png  # 選ばれる理由用画像
    ├── icon_*.png    # アイコン類
    ├── abstract_*.png# 抽象的な装飾パターン
    ├── button_*.png  # ボタン素材
    ├── callout_*.png # 吹き出し素材
    ├── card_*.png    # カード素材
    └── 0*_*.png      # セクション別参考画像・LP全体画像
```

## ローカルでの確認

ファイルをブラウザで直接開くだけで動作します。

```bash
open index.html
```

サーバーが必要な場合は任意のHTTPサーバーを使用してください。

```bash
# Python
python3 -m http.server 8080

# Node.js (npx)
npx serve .
```

## 制作メモ

- デザインモックは [Claude Design](https://claude.ai/design) で作成
- コード実装は [Claude Code](https://claude.ai/code) で実施
- ビューポートは `width=1200` 固定（レスポンシブ未対応）
- FAQは `<details>` / `<summary>` でJS不使用のアコーディオン実装
