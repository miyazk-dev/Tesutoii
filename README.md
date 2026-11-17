# Nexora website

HTML / CSS / Vanilla JavaScript だけで動作する静的Webサイトです。Astro、npm、GitHubは不要です。

## ローカル確認

VS Codeでこのフォルダーを開き、Live Server拡張機能で `index.html` を開きます。もしくは `index.html` をブラウザで直接開いてください。

## Googleフォームの設定

1. Googleフォームを新規作成し、名前・メールアドレス・相談内容・プライバシーポリシー同意などを設定します。
2. 一般の回答者がアクセスできる公開設定にします。回答を1回に制限するとGoogleログインが必要になる点に注意してください。
3. フォームの回答通知を有効にします。
4. `js/config.js` の `contactFormUrl` に `https://docs.google.com/forms/...` のURLを設定します。
5. フォームを自分で送信して、通知と返信手順を確認してください。

## Xのリンク

`js/config.js` の `xUrl` に取得済みのXアカウントURLを設定してください。空欄ならリンクは表示されません。

## Xserverへの公開（後日）

ドメインとSSLを設定後、サイトのファイル一式（`index.html`、他のHTML、`css`、`js`、`assets`）を対象ドメインの `public_html` にアップロードします。既存ファイルは先にバックアップしてください。

## 公開前の必須確認

- Nexoraという名称の商標・既存事業者・ドメインの重複確認
- `meta robots` の `noindex,nofollow` を公開準備が整ってから削除
- 各ページのSEOメタ情報、canonical、OGP、サイトマップの設定
- 料金・税区分・契約条件の確定
- プライバシーポリシー、利用・取引条件、事業者情報の法務確認
- 未成年者による受注・契約について保護者との確認
- Googleフォームの設定・送信テスト
- Xアカウントの取得とURL設定
- スマホ、PC、キーボード操作、404の動作確認

※ 現在はローカル試作用です。公開用の完成版ではありません。
