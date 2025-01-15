---
title: 'Docker Desktop for Macがマルウェア扱いされてしまう'
slug: '20250115231938'
description:
date: 2025-01-15T23:19:38+09:00
image: docker.png
math:
license:
hidden: false
comments: false
draft: false
categories:
  - 技術
tags:
  - Docker
  - MacOS
---

## Introduction

久々に MacBookAir を開いたら、Docker Desktop がマルウェア扱いされてゴミ箱送りにされる現象が起きた。

X で検索してみるとどうやら自分だけではないみたい。

詳細は[こちら](https://www.docker.com/ja-jp/blog/incident-update-docker-desktop-for-mac/)

自分の場合、以下の手順で解消することができた。

1. ゴミ箱内の Docker.app を削除する
2. [Docker Desktop](https://www.docker.com/ja-jp/products/docker-desktop/)公式サイトから dmg をダウンロードする
3. ダウンロードした dmg を開き、Docker.app をドラッグ&ドロップして Applications に格納する
4. [こちら](https://www.dockerstatus.com/pages/incident/533c6539221ae15e3f000031/677dd6e2108ba105c8d0258c)の Run the following commands に記載されているコマンドを実行する
5. Docker Desktop を再起動する

同じ現象が起きた方に役立ててほしい。
