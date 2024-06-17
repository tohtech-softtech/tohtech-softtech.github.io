## 使用技術
- Ruby
- Jekyll

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