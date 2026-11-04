+++
title = "Hugo で Shortcodes をエスケープする"
date = 2021-01-21T00:00:00+09:00
categories = [ "Tech" ]
tags = [
    "Hugo",
]
+++

Hugo のサイト上で `{{</* foo */>}}` と表示したい。

<!--more-->

## 背景

[昨日の記事]({{< ref "hugo-soundcloud.md" >}}) で、記事内に shortcodes の使い方のサンプルコードを貼ろうとしたら、サンプルコード自体が shortcodes と解釈されてしまうという問題でハマりました。

`\{\{< foo >\}\}` や `{{{{</* foo */>}}}}` のようにエスケープできるかと思ったけど、どちらもうまくいかず。。。

## 解決方法

いろいろ調べたところ、以下の記述でうまくいくとのこと。

```
{{</*/* foo */*/>}}
```

いやー、コレはムズいですね。

## 参考リンク

- [Escaping Hugo shortcodes](https://liatas.com/posts/escaping-hugo-shortcodes/)
