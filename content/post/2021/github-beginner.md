+++
title = "GitHub で初心者向けの Issue を探す"
date = 2021-02-07T21:30:00+09:00
categories = [ "Tech" ]
tags = [
    "GitHub",
]
+++

OSS に貢献したいときの検索方法。

<!--more-->

## 探し方

フリーワードで検索すると色々見つかりすぎてしまうので、初心者向けの修正を示すラベルで絞り込むのが良いです。

- [beginner](https://github.com/search?o=desc&q=state%3Aopen+label%3A%22beginner%22&s=created&type=Issues)
- [easy-fix](https://github.com/search?o=desc&q=state%3Aopen+label%3A%22easy-fix%22&s=created&state=open&type=Issues)
- [good first issue](https://github.com/search?o=desc&q=label%3A+%22good+first+issue%22&s=created&state=open&type=Issues)
- [up-for-grabs](https://github.com/search?o=desc&q=label%3A+%22up-for-grabs%22&s=created&state=open&type=Issues)

特定の言語に絞り込みたいときは、Languages から言語で絞り込めば、得意の言語だけを対象にできますね。

State は当然 Open、Sort は Newest にしておくと、反応をもらいやすくなりそうです。

## 参考リンク

- [Links for beginners willing to contribute to OpenSource projects](https://gist.github.com/stefanmaric/d5a03eeb89af81e5537e2efe7dd479cf)
