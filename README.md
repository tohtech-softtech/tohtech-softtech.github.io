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
