---
title: SFTP 管理について
description: コントロールパネルでの SFTP 管理の詳細
translation-type: tm+mt
source-git-commit: 3faeb9651681a9edd18cf889fff65b02644cb690
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 68%

---


# SFTP 管理について {#about-sftp-management}

コントロールパネルでは、アクセス権のある Campaign インスタンスに接続されているすべての SFTP サーバーを操作できます。ほとんどのインスタンスは SFTP サーバーに接続されています（場合によっては、開発インスタンスおよびステージインスタンスは、どの SFTP サーバーにも接続されていない可能性があります）。

SFTP サーバーへのアクセスは、SFTP クライアントソフトウェアを使用しておこなわれます。このソフトウェアは、オンラインで見つけてダウンロードできます。クライアントアプリケーションまたはAPIを介してサーバーに接続するには、公開SSHキーを設定し、SFTPサーバーに接続するIPアドレスを許可リストに追加する必要があります。

コントロールパネルを使用すると、以下の操作を実行して SFTP サーバーを管理できます。

* **ストレージ容量**&#x200B;を監視する。
* Manage **IP addresses allow listing**: add or delete IP addresses ranges for one or several servers,
* サーバーにアクセスするための **SSH 公開鍵**&#x200B;を管理する。

これらの各操作について詳しくは、以下の節を参照してください。
