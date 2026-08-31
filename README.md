# CopyGuard — Landing Page

**CopyGuard**（v1.1.0）の公式ランディングページです。

- Obsidian Sync 以外（iCloud / Dropbox / Remotely Save / Syncthing）で増える競合コピー・空ファイル・一時ファイルを見つける
- 選んだ項目だけ隔離フォルダ（既定 `K-Tech Trash Box`）へ移動し、削除は別の確認ステップ（既定は消さない）
- 免責事項を専用セクションで明記（無保証、誤検出の可能性、同期による他端末への影響、マージはしない、バックアップ推奨）
- 日本語 / English 切り替え、Buy Me a Coffee

このフォルダは静的サイトです（`index.html` 1枚 + 補助ファイル）。フレームワークは使いません。

## ステータス

公開済みです。GitHub リポジトリを作成・push 済み、Vercel にも https://copy-guard-lp.vercel.app/ でデプロイ済みです。

## ローカルで見る

```bash
cd "/Users/kimurashigeru/Documents/github/k-Tech CopyGuard_LP"
python3 -m http.server 8080
```

ブラウザで http://localhost:8080 を開きます。

## 公開先

| 項目 | 値 |
|------|-----|
| GitHub リポジトリ | https://github.com/crossbeat461-a11y/copy-guard-lp |
| Vercel | https://copy-guard-lp.vercel.app/ |
| GA4 測定 ID | `G-SCCSLDV8T8`（CopyGuard LP 専用。会社HPの `G-774DT6CW0W` は使わない） |
| Search Console 確認ファイル | `google8a8913465dda62dd.html`（他 LP と同一トークン） |

## OG 画像

`og.svg` を用意しています（1200×630 相当のベクター）。SNS カードの互換性を上げたい場合は、これを元に `og.png` を書き出して `index.html` の `og:image` / `twitter:image` を差し替えてください（`k-tech-update-guard-lp` の `og.png` と同じ手順）。

## バージョンを上げるとき

`index.html` の現在の版番号を置換:

- `<title>` と meta / JSON-LD
- ヒーローの `#version-badge`
- フッター
- `#changelog` の先頭に `.release` を追加（`latest` クラスを新しい方へ）

`og.svg` と `sitemap.xml` の日付も必要なら更新します。

## リンク

- プラグイン本体: https://github.com/crossbeat461-a11y/copy-guard
- Releases: https://github.com/crossbeat461-a11y/copy-guard/releases/latest
- K-Tech Studio: https://k-tech-lab.vercel.app/
- Buy Me a Coffee: https://buymeacoffee.com/k_tech_studio
