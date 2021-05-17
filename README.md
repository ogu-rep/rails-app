# README

ruby 2.6.5

### Homebrewのupdate
```
brew update
```

### rbevのupdate

```
brew upgrade rbenv
```

### bundlerのupdate

```
sudo gem install bundler
```

### インストールできるRubyのバージョンを確認

```
rbenv install -l
```

### Ruby2.6.5のインストール

```
rbenv install 2.6.5
```

### rbenvにパスを通す

```
echo 'export PATH="$HOME/.rbenv/bin:$PATH"' >> ~/.bash_profile
```

```
echo 'eval "$(rbenv init -)"' >> ~/.bash_profile
```

```
source ~/.bash_profile
```


- which gemとwhich rubyのコマンドを打ってそれぞれが下記のようになっていたらOK

```
/Users/自分のパソコンの名前/.rbenv/shims/ruby
/Users/自分のパソコンの名前/.rbenv/shims/gem
```

### yarnのインストール

```
brew install yarn
```

### Railsの設定

- アプリを置きたい場所に空のディレクトリを作成

```
mkdir rails-app
```

```
cd test_app
```

```:rails-app
bundle init
```

```
# frozen_string_literal: true

source "https://rubygems.org"

git_source(:github) {|repo_name| "https://github.com/#{repo_name}" }

# gem "rails"  ←この行のコメントを外す
```

### Gemインストール
```
bundle install --path vendor/bundle
```

### rails new 

```
bundle exec rails new .
```

### サーバー起動

```
bundle exec rails s
```

[参考](https://qiita.com/tana18/items/203122272fdb730e7383)
