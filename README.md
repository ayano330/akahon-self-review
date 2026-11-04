# 赤本 自己分析ツール(生物)

生徒向けの静的 Web アプリ(サーバー・DB なし)。データは端末のブラウザ内のみ。

| ファイル | 用途 |
|---|---|
| `v3.html` | **現行版**(配布用 URL は基本これ) |
| `v2.html` / `index.html` | 比較用の旧版 |
| `akahon-icon-*.png` / `akahon-header-bg.jpg` | ホーム画面アイコンとヘッダーの背景画像 |
| `teachers/` | ホームに出す先生のミニキャラ画像(掲載許可を得たものだけ) |

公開URLに出るのは、`.github/workflows/pages.yml` で選んだファイルだけです(`docs/`・元画像は出ません)。

## 公開 URL(GitHub Pages)

リポジトリ名を `akahon-self-review`、ユーザー名を `YOUR_USER` とすると:

- **現行版:** `https://YOUR_USER.github.io/akahon-self-review/v3.html`
- v2: `https://YOUR_USER.github.io/akahon-self-review/v2.html`

初回は GitHub の **Settings → Pages → Build and deployment → Source: GitHub Actions** を有効にしてください(ワークフロー `Deploy to GitHub Pages` が push で走ります)。

## ローカル確認

```bash
python -m http.server 8123 --bind 127.0.0.1
```

→ http://127.0.0.1:8123/v3.html

## 設計メモ

`docs/design-memo.md`
