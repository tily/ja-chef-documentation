# chef ドキュメント翻訳作業用レポジトリ

## 作業メモ

	export $PATH=PATH:./bin
	jdc download "Fast Far Guide" # ページの textile と添付画像をダウンロードして git commit まで行う
	jdc preview page_id
	jdc upload page_id

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
