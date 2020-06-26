---
id: appdev-introduction
title: アプリを開発する
sidebar_label: はじめに
---

本章ではサンプルアプリの開発の流れを通して、PersoniumのAPIを使用したアプリの開発方法を説明します。

## サンプルアプリの開発

サンプルアプリ(Personium Trails)はGoogle上に蓄積した移動履歴データをPersoniumに格納して、そのデータの一部を他の人に共有するものです。アプリケーションの種類としてはブラウザ上で稼働するWebアプリケーションです。

以下は完成したサンプルアプリのスクリーンショットとなります。

TODO: アプリのスクリーンショットを掲載

完成されたサンプルアプリのコードは以下のリンク先にあります。

[app-personium-trails](https://github.com/personium/app-personium-trails)

## 事前知識

以下の事前知識があることを想定しています。

* 基本的なWebアプリケーション開発
* フロントエンド開発 (Html, JavaScript, CSS)
* REST API

## 事前準備

サンプルアプリでは、2つのCell作成とCellに関連するAccount, Role, ACL設定を事前に行っています。Personiumを使ったアプリを開発する場合、同様のことを行います。Cell作成と関連する設定方法は[前章チュートリアル](../unit-administrator/tutorial.md)を参考にしてください。  

サンプルアプリでの2つのCellの用途と詳細の設定は以下の表の通りとなります。

|用途|Cell名|Account名|AccountにリンクするRole名|Roleの権限設定|
|----|---|---------|-----------------------|--------------|
|データ主体用Cell|alice|me|admin|root|
|アプリ用Cell|sample-app|app|admin|root|

自身のアプリを開発する場合、それぞれのCell, Account, Roleの名前は任意なので表の通りでなくてもかまいません。