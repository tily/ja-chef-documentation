# chef ドキュメント翻訳作業用レポジトリ

## 作業メモ

jcd という ruby のコマンドで、Chef ドキュメント原文をダウンロード・プレビュー・アップロードしたりできるようになっています。

	export $PATH=PATH:/path/to/ja-chef-documentation/bin

とかやって、パスを通しておくとよい感じです。いくつかの ruby ライブラリに依存しているので、下記でインストールしておくといい感じです。

	gem install mechanize highline git-style-binaries launchy

なお、コマンドを実行するためには http://wiki.opscode.com のアカウントが必要です。

### jcd download

	jcd download PAGE_NAME
	jdc download "What is Chef?" # ページ原文・添付画像をダウンロードし git commit する

### jcd preview

	jcd preview PAGE_ID
        jcd preview 7274862 # "What is Chef?" の PAGE_ID=7274862 版をプレビューする (Win/Mac の場合はブラウザで開いてくれる)

### jcd upload

まだ実装していないので手動でアップロードしています。

## 翻訳メモ

 * 「もう 1 度」「2 度と」
 * business -> ビジネス

## TODO

 * ページ名を日本語にしたのでリンクも日本語にする必要あり
 * download、ページ名に "?" が入っているとダウンロードできない →page_id でもダウンロードできるようにする
 * preview、page_id も指定しないといけなくなるか、逆に page_id だけでいいか
 * upload、キャプチャ画像をダウンロードし表示した上で入力するようにする
 * wiki.opscode.com で実際に WikiName で各ページがリンクにできるか確認する

## 著作権

[CC BY-SA 3.0](http://creativecommons.org/licenses/by-sa/3.0/)

[Opscode Chef ドキュメント](http://wiki.opscode.com/display/chef/Home) の日本語訳です。
Share Alike なので原文と同じく BY-SA 3.0 で公開します。
