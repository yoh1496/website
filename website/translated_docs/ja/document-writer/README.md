---
id: README
title: Personium ドキュメント整備・改善への参加方法  
sidebar_label: Personium ドキュメント整備・改善への参加方法  
---

オープンソースプロジェクトPersoniumでは、コードだけでなくドキュメント貢献についても歓迎しております。  
ドキュメントの改善にご協力いただける方は、以下の手順に従ってお願い致します。

> __GitHubアカウントをご用意ください__

## ドキュメントの改善指摘

1. GitHubリポジトリ上のissuesに改善指摘を作成する
    1. [PersoniumドキュメントWebサイト issues](https://github.com/personium/website/issues)

上記を実施していただくことで、Personiumプロジェクトメンバもしくは他の参加者が指摘を元に修正・公開することができます。  

## ドキュメントの追加および更新

1. GitHubリポジトリをForkする
    1. [PersoniumドキュメントWebサイト](https://github.com/personium/website)
1. Localリポジトリにクローンする
1. [リポジトリREADME](https://github.com/personium/website)を参考にドキュメントを更新する
1. Forkした自身のGitHubリポジトリにPushし、Fork元の親リポジトリに対してPull Requestを発行する

上記の手順を実施していただくことで、Personiumプロジェクトメンバでレビューをし、適切な形で公開させていただきます。  
皆様のご協力をお待ちしております。  


***

> __ドキュメント記載時の注意点__

 * 文中の改行について  
  文中で改行したい場合は、`<br>`は使用せずに、半角スペース2つを入力し改行してください。  
  但し 、テーブル内において改行したい場合は`<br>`を使用してください。  
  記載例）
    ```markdown
    あいうえお  (←半角スペース2つ）  
    かきくけこ
    ```

 * MDからhtml変換時にURLのハイパーリンクを無効化する場合  
  MDファイルにhttp&#58;//～のような記載をした場合、html変換した際に自動的にURLへのハイパーリンクが張られてしまいます。  
  サンプルの中などへの記載で、ハイパーリンクを張りたくない場合には":"ではなく"`&#58;`"を記載してください。  
  記載例）
    ```markdown
    `http&#58;//~`
    ```

 * cURLコマンドサンプルの記述について  
  cURLコマンドサンプルの記述が**100文字以上**の長さとなる場合は、１行あたりの長さが100文字未満になるように改行してください。  
  改行する際は、改行位置に`\`（バックスラッシュ）を付けて改行してください。  
  記載例）
    ```markdown
    curl "https&#58;//{UnitFQDN}/__ctl/Cell" -X POST -i -H 'Authorization: Bearer {AccessToken}' `\`(←改行位置に\を付ける）
    -H 'Accept: application/json' -d '{"Name":"{CellName}"}'
    ```
