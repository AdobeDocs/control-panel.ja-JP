---
product: campaign
solution: Campaign
title: SFTP の管理について
description: コントロールパネルでの SFTP 管理の詳細
testing: SSECD-836 2
feature: Control Panel
role: Architect
level: Intermediate
exl-id: b2c3be80-0d1b-4998-87ab-5280c6213f3d
source-git-commit: 4fc34b07b497c743e2ca6c182e68d6ea5c180ac9
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 100%

---

# SFTP の管理について {#about-sftp-management}

コントロールパネルでは、アクセス権のある Campaign インスタンスに接続されているすべての SFTP サーバーを操作できます。ほとんどのインスタンスは SFTP サーバーに接続されています（場合によっては、開発インスタンスおよびステージインスタンスは、どの SFTP サーバーにも接続されていない可能性があります）。

SFTP サーバーへのアクセスは、SFTP クライアントソフトウェアを使用しておこなわれます。このソフトウェアは、オンラインで見つけてダウンロードできます。このようなクライアントアプリケーションや API を使用してサーバーに接続するには、SSH 公開鍵を設定して、SFTP サーバーに接続する IP アドレスを許可リストに追加する必要があります。

コントロールパネルを使用すると、以下の操作を実行して SFTP サーバーを管理できます。

* **ストレージ容量**&#x200B;を監視する。
* **IP アドレスの許可リストへの登録**&#x200B;を管理する。1 つまたは複数のサーバーの IP アドレス範囲を追加または削除します。
* サーバーにアクセスするための **SSH 公開鍵**&#x200B;を管理する。

これらの各操作について詳しくは、以下の節を参照してください。
