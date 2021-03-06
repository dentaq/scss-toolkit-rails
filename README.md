# scss-toolkit-rails

Scss/compassを利用したMixinをまとめたGemです。

## Installation

### Railsユーザー向け

1) 以下のコードを`Gemfile`に追加してください:

```ruby
group :assets do
  gem 'sass-rails'
  gem 'compass-rails'
  gem 'scss-toolkit-rails'
end
```

2) 以下のコードを`application.css.sass`のようなファイルに追加して下さい:

```sass
@import compass/utilities
@import compass/css3
@import scss-toolkit
```

### Rails以外（Middlemanなど）でお使いの方向け

1) 以下のコマンドを実行して、ローカルに`_scss-toolkit.sass`をダウンロードして下さい:

```
curl https://raw.github.com/mahm/scss-toolkit-rails/master/vendor/assets/stylesheets/_scss-toolkit.sass > _scss-toolkit.sass
```

2) Compassの使える環境で`_scss-toolkit.sass`をインポートしてお使いください:

```sass
@import compass/utilities
@import compass/css3
@import scss-toolkit
```


## 使用例

* [Scss Toolkit Sample](http://scss-toolkit-sample.herokuapp.com/)
* [Scss Toolkit Sample(github)](https://github.com/dentaq/scss-toolkit-sample)


## その他

gem化にあたりましては
[https://github.com/mahm/zurui-sass-rails](https://github.com/mahm/zurui-sass-rails)
を参考にさせていただきました。ありがとうございました。
