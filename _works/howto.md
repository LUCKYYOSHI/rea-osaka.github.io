---
layout: single
title: "環境整備のためのHowTo"
permalink: /works/howto/
toc: true
toc_label: "目次"
---

まずは、あなたのパソコンで、色んな事に挑戦するための環境を整備しましょう。

## GitHub

GitHubを利用して、交流しましょう。

### [アカウント作成](/works/howto/github/account/)

### [初めてのISSUEへの書き込み](/works/howto/github/issue/)


## R環境の整備

rea-osakaのリポジトリで紹介しているスクリプトはR言語で書かれているものがあります。
そこで、ここでは、これらR言語で書かれたスクリプトをWindows上で利用するための環境整備を紹介します。

### 1. 環境構築の選択肢

R言語の環境を構築するための選択肢としては、R Projectの一時配布先であるCRANから直接インストールするだけでなく、
データサイエンス環境を容易に構築するためのディストリビューションの一つである[Anaconda](https://www.anaconda.com)を利用することも可能です。
実際、パソコンの環境整備について余計な労力を避けるためデータサイエンティストの間ではAnacondaの人気が高いです。

このような選択肢がある中、現在の所、RでGIS（地図を扱うシステム）を扱う環境整備が過渡期にあり、
Rのバージョンが最新に近いバージョンでないとこれらGISと便利に連携する機能が使えないという事情があります。
そして、AnacondaディストリビューションにパッケージングされているR関連のバージョンは少し古いものなので、
現在の所、GISに関して最新の便利な機能が使えません（Windowsに関して）。

本来、AnacondaのRに関するパッケージを使えば、
以下で紹介する環境が全部簡単にインストールされますが、GISの連携便利機能が使えないので、
ここでは、AnacondaのR関連パッケージを使わず、それぞれの配布元から最新のR環境を構築する手順を紹介します。

### 2. Rの開発環境を整備する

まずRについて、CRANからのインストールを紹介します。

 - [Rのインストール](/works/howto/r/install/)

R言語は、基本的な機能以外の部分について、
「パッケージ」として後からインストールできるようになっています。
一般的に良く利用されるものや、
rea-osakaのリポジトリにあるスクリプトが利用していたりするパッケージを例にして
パッケージのインストールの手順を紹介します。

 - [パッケージのインストール](/works/howto/r/packageinstall/)

さて、Rは原始的にはコンソール上でコマンドを発行して実行します。

しかし、単純なコンソール上での作業は不便なので、
通常Rを使ってデータサイエンス作業をする場合、
統合開発環境や高級インタラクティブ環境を使います。

そこで、人気のあるＲの統合開発環境の一つである[RStudio](https://www.rstudio.com)と
ブラウザ上で動く高級インタラクティブ環境である[jupyter](http://jupyter.org/)の環境構築方法を紹介します。

 - [RStudioのインストール](/works/howto/r/rstudio_install/)
 - [RをJupyter Notebookで使うための環境の整備](/works/howto/r/jupyter_setting/)


## Anaconda環境の整備

Anacondaは、PythonとRを利用するための環境構築を容易にするディストリビューションです。

 - [Anacondaのインストール](/works/howto/anaconda/install/)
