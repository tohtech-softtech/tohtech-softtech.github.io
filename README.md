## 概要
このウェブサイトは、`Jekyll`というブログサイト生成ツールを使って作成されています。`Jekyll`を自分のパソコン上で動かすには`Ruby`のインストールが必要です。お使いのOSに合わせて`Ruby`のインストールをお願いします。

ウェブサイトの構造自体は、HTMLやSCSSで書かれています。ただし、Jekyll特有の書き方もあるので[公式ドキュメント](https://jekyllrb-ja.github.io/docs/)を参考にしてください。

ブログの投稿はMarkdownファイルを使用するため、投稿の追加・変更・削除を簡単に行うことができます。

## 前提条件
- `Git`
- `Ruby`

この2つがインストールされていることを確認してください。

VSCodeなどのエディタがあると便利に編集ができます。

## 環境構築
1. リポジトリのクローン

リポジトリをクローンします。

```bash
git clone https://github.com/tohtech-softtech/tohtech-softtech.github.io.git
cd tohtech-softtech.github.io
```
2. Bundler, Jekyllのインストール

BundlerはRubyの依存関係を管理するツールです。以下のコマンドでインストールします。

```bash
gem install bundler jekyll
```
3. 依存関係のインストール

Gemfileに記載された依存関係をインストールします。

```bash
bundle install
```

4. ローカルサーバの起動

以下のコマンドでローカルサーバを起動し、サイトを表示します。

```bash
bundle exec jekyll serve
```
サーバが起動したら、ブラウザで http://localhost:4000 にアクセスしてください。

## ファイル構成図
```
tohtech-softtech.github.io:
│  .gitignore
│  404.html         # 404 ページの中身
│  about.md         # /about ページの中身
│  favicon.ico      # ウェブサイトのアイコン
│  gallery.md       # /works ページの中身
│  Gemfile          # Rubyの設定ファイル (基本いじらない)
│  Gemfile.lock     # Rubyの設定ファイル (基本いじらない)
│  index.md         # / ページの中身
│  README.md
│  _config.yml      # ウェブサイトの設定ファイル
├─admin             # DecapCMSの設定フォルダ (未設定)
├─_includes         # ホームページの共通部分のフォルダ
├─_layouts          # ホームページのレイアウトフォルダ
├─_posts            # ブログとして投稿するMarkdownのフォルダ
├─_sass
│  └─minima         # ホームページのSCSSのフォルダ
└─_site             # 生成される静的フォルダ (基本いじらない)
```

