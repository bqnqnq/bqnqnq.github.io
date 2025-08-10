# Theme

## Theme の設定方法

### 配置

`./theme/` に各種ファイルを配置することで、自動的に優先してロードされる。
```
.   
└── theme
    ├── css
    │   ├── chrome.css
    │   ├── general.css
    │   └── variables.css
    ├── fonts
    │   ├── BIZUDGothic-Bold.ttf
    │   ├── BIZUDGothic-Regular.ttf
    │   ├── BIZUDPGothic-Bold.ttf
    │   ├── BIZUDPGothic-Regular.ttf
    │   └── fonts.css
    ├── highlight.css
    └── index.hbs
```

配置や名称はリポジトリを参考<br>
[https://github.com/rust-lang/mdBook/tree/master/crates/mdbook-html/front-end](https://github.com/rust-lang/mdBook/tree/master/crates/mdbook-html/front-end)

`./book.toml` に以下を記述することで任意のディレクトリが `./theme/` の代わりになる。

```toml:book.toml
[output.html]
theme = "dir/hogehoge"
```

### フォント

BIZ UDPGothic などのフォントも、 `./theme/fonts/` に配置することで追加できる。
