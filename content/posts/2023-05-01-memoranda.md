---
title: "不要になったローカルリポジトリ削除で困った話 - My Memoranda"
date: 2023-05-01
Toc: false
---

mattnさんの回答をStack Over Flow で見つけたのでメモ
<!--more-->
## 不要になったローカルリポジトリの削除方法

[不要になったローカルリポジトリの削除方法は](https://ja.stackoverflow.com/questions/5734/git-不要になったローカルリポジトリの削除方法は)
```
git branch --delete $(git branch --merged master | grep -v '^*\\|  master$')
```
> これでマスタに取り込まれたブランチが削除されます。
残ったブランチがマスタに取り込まれていないブランチです。それぞれリモートにpushされていないか確認すると良いです。OSS なら漏れなく push してしまうのに `git push --all`で良いかと思います。
>
> その後はディレクトリごと消してしまっていいと思います。


## Jack@Nostrの投稿から
> My programming hero:

[Welcome to cr.yp.to. Some popular subdomains:](http://cr.yp.to)
