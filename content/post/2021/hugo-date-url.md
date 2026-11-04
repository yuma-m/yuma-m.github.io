+++
title = "Hugo の URL に日付を入れる方法"
date = 2021-01-19T21:00:00+09:00
categories = [ "Tech" ]
tags = [
    "Hugo",
]
+++

Permalinks を使えば簡単。

<!--more-->

## やりたいこと

Hugo でブログポストの URL に日付を入れて、`post/YYYY/MM/DD/TITLE/` のようにしたい。

## やり方

- Bad: `content` 以下のディレクトリ構成を `post/YYYY/MM/DD/title.md` のようにする
- Good: [Permalinks](https://gohugo.io/content-management/urls/) を利用する

## 設定例

`config.toml` 内で設定する。

```toml
[permalinks]
post = "/:section/:year/:month/:day/:filename/"
```

## 所感

ちょっとしたことが設定 1 つでできるのは本当に便利。もっと Hugo を使いこなしたい。

## 参考リンク

- [URL Management | Hugo](https://gohugo.io/content-management/urls/)
