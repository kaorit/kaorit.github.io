---
title: “My Memoranda”
date: 2023-04-28T16:25:14+0900
draft: false
pin: false
summary: "pickup"
---
## 2023/05/01
### 不要になったローカルリポジトリの削除方法
mattnさんの回答を見つけたのでメモ

[不要になったローカルリポジトリの削除方法は](https://ja.stackoverflow.com/questions/5734/git-不要になったローカルリポジトリの削除方法は)
```
git branch --delete $(git branch --merged master | grep -v '^*\\|  master$')
```
> これでマスタに取り込まれたブランチが削除されます。
残ったブランチがマスタに取り込まれていないブランチです。それぞれリモートにpushされていないか確認すると良いです。OSS なら漏れなく push してしまうのに `git push --all`で良いかと思います。
>
> その後はディレクトリごと消してしまっていいと思います。

### Jack@Nostrの投稿から
> My programming hero:

[Welcome to cr.yp.to. Some popular subdomains:](http://cr.yp.to)


## 2023/04/29
### Markdown tutorial
[commonmark.org](https://commonmark.org/help/)

## 2023/04/28
### Openstack
[お家にクラウド環境を運用して10年経っていた話](https://light-of-moe.ddo.jp/~sakura/diary/?p=1528)
