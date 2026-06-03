# カトウ塗装工業 採用特設サイト

カトウ塗装工業株式会社の採用特設サイト。GitHub Pagesで公開。

## 募集職種

- **戸建て診断スタッフ** — 屋根に登って、写真を撮って、報告書を書く仕事
- **積算営業事務スタッフ** — 月次請求と見積下書きを担当

## 訴求軸

2026年中東情勢悪化によるシンナー不足を背景に、塗装職人転身者向けの採用も並走。

- 経験豊富な塗装職人（体力勝負からは引きたい方）
- シンナー不足で工事継続が困難になっている方
- 元施工管理・営業・損保鑑定人など住宅関連経験者

## 公開URL

GitHub Pages: `https://<username>.github.io/kato-recruit-site/`

## ファイル構成

```
kato-recruit-site/
├── index.html       # 採用サイト本体（HTML/CSS/JS一体型・単一ファイル）
├── README.md        # このファイル
├── .gitignore       # Git除外設定
└── .nojekyll        # GitHub PagesのJekyll処理を無効化
```

## デプロイ方法

### GitHub Pagesで公開する手順

1. GitHubで `kato-recruit-site` リポジトリを作成
2. このフォルダを `git push`
3. リポジトリの **Settings → Pages** へ
4. **Source**: `Deploy from a branch` を選択
5. **Branch**: `main` / `(root)` を選択 → Save
6. 数分後に `https://<username>.github.io/kato-recruit-site/` で公開

### コマンド例

```bash
cd kato-recruit-site
git init
git add .
git commit -m "初回公開"
git branch -M main
git remote add origin https://github.com/<username>/kato-recruit-site.git
git push -u origin main
```

## 構成上のポイント

- **単一HTML完結**:外部CSSやJSフレームワーク不要。`index.html`ひとつで完結
- **画像はBase64埋込**:加藤社長・佐藤さんの写真はHTMLに直接埋め込み済み
- **外部依存**:Google Fonts(Shippori Mincho / Noto Sans JP / Zen Old Mincho)、Instagram埋込(SnapWidget)
- **構造化データ**: JobPosting実装でGoogleしごと検索対応
- **レスポンシブ**: PC/タブレット/スマートフォン対応

## 更新方法

`index.html`を直接編集してpushすればOK。GitHub Actionsの設定は不要(GitHub Pagesが自動的にデプロイ)。

## 制作

株式会社メディレクション
