# Catcheez

トレーディングカード × Web3（IPO抽選 / ボンディングカーブ取引）プロトタイプ。
すべて単一ファイルの静的HTML（画像はdata URIで埋め込み済み、ビルド不要）。

## ページ
| ファイル | 内容 |
|---|---|
| `catcheez-app.html` | 統合版（SPA）。ヘッダーのタブで全ページを切り替え。**まずはこれを開く** |
| `catcheez-ipo-detail.html` | IPO抽選の詳細（$AURUM）。チケット購入モック・構成カードのポップアップ |
| `catcheez-psax-ipo.html` | IPO抽選の詳細（$PSAX / PSA10 Genesis Box） |
| `catcheez-ipo-results.html` | IPO当選結果（抽選番号の開封演出・当選者一覧・Claim） |
| `catcheez-market.html` | マーケット一覧（IPO抽選＋ボンディング）。CATCHEEZ風HUDカード |
| `catcheez-charizard-trade.html` | $CHZ 取引画面（ボンディングカーブ、取引で価格変動、コレクション） |
| `catcheez-gem10-trade.html` | $GEM10 取引画面 |
| `catcheez-account.html` | アカウント（保有・参加IPO・履歴・設定） |
| `index.html` | `catcheez-app.html` へのリダイレクト |

個別ページ同士のリンクは相対パス（`catcheez-*.html`）なので、同じフォルダに置いて開けば相互に移動できます。

## ローカルで開く
```bash
python3 -m http.server 8000   # → http://localhost:8000/catcheez-app.html
```

## デザインシステム
- フォント: Bricolage Grotesque / Plus Jakarta Sans / Black Ops One（数値）
- アクセント: `--accent #ffb300` / `--accent-deep #ff8a00`
- 象徴的な「HUD」パネル（ノッチ付き多角形＋ゴールドのコーナー＋ハッチ）
