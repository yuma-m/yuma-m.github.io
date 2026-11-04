+++
title = "Hugo へ移行しました"
date = 2021-01-18T23:30:00+09:00
categories = [ "Tech" ]
tags = [
    "Hugo",
    "GitHub",
]
+++

ポートフォリオサイトを HTML ベタ書きから Hugo に移行しました。

<!--more-->

## きっかけ

自身のポートフォリオサイトである <https://yuma.cloud/> では、今までは HTML をゴリゴリ書いて作っていおりました。でも最近 Hugo 製のサイトが増えているなーと感じていたのと、サイトのコンテンツがスカスカなので、ついでにブログを統合してしまいたいと思いまして、思い切って Hugo で書き直しました。

とはいっても、HTML を Markdown に変換して、体裁を整えたくらいなので、コンテンツの移行に要した時間は 2 時間弱。HTML を書き直すことを考えたら、随分とお手軽に移行が済んだものです。お仕事でも Hugo を使ってハンズオンサイトを作ったりしていたので、Hugo 慣れしていたおかげというのもありそうです。

## 所感

Hugo のテーマの豊富さや使い勝手の良さもさることながら、何より GitHub Actions を用いて GitHub Pages にデプロイするのが簡単すぎてビックリしました。コマンド 1 行も書かなくても、YAML の設定だけで勝手にワークフローが完了するのサイコーすぎます。

ハマりポイントとしては、独自ドメインを使っている場合は `gh-pages.yml` で `cname` の設定を忘れないように。

## 参考リンク

- [Hugo Themes Anatole](https://themes.gohugo.io/anatole/)
- [GitHub Actions による GitHub Pages への自動デプロイ](https://qiita.com/peaceiris/items/d401f2e5724fdcb0759d)
