+++
title = "Hugo に SoundCloud のウィジェットを埋め込む"
date = 2021-01-20T00:00:00+09:00
categories = [ "Tech" ]
tags = [
    "Hugo",
    "SoundCloud",
]
+++

Hugo 製のサイトに SoundCloud の Player ウィジェットを埋め込む方法。

<!--more-->

## できたもの

{{< soundcloud 63874417 >}}

## やり方

以下のファイルを `layouts/shortcodes/soundcloud.html` として保存します。

```html
<iframe
  width="100%"
  height="450"
  scrolling="no"
  frameborder="no"
  allow="autoplay"
  src="https://w.soundcloud.com/player/?url=https%3A//api.soundcloud.com/users/{{ index .Params 0 }}&color=%23ff5500&auto_play=false&hide_related=false&show_comments=true&show_user=true&show_reposts=false&show_teaser=true"
>
</iframe>
```

呼び出したいページからは以下のように呼び出します。`ユーザID` は数値型で、`username` とは異なります。[SoundCloud の API](https://developers.soundcloud.com/docs/api/reference#me) から取得できそうです。

```markdown
{{</* soundcloud ユーザID */>}}
```

## 2021/02/01 追記

使い方を含めて[GitHub](https://github.com/yuma-m/hugo-shortcodes-soundcloud)に上げました。

## 参考リンク

- [Hugo Soundcloud shortcode](https://janikvonrotz.ch/2018/07/09/hugo-soundcloud-shortcode/)
