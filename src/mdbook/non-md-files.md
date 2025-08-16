# Markdownではない形式の場合の対処法

## ipynb (Jupyter)
未解決

### 1. CLIで手動で変換
```shell
jupyter nbconvert --to markdown my-notebook.ipynb
```
欠点
- 画像が組み込まれない
- 一部の表示が崩れる