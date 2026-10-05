---
product: campaign
solution: Campaign
title: SFTP の管理について
description: コントロールパネルでの SFTP 管理の詳細
testing: SSECD-836 2
feature: Control Panel, SFTP Management
role: Admin
level: Intermediate
exl-id: b2c3be80-0d1b-4998-87ab-5280c6213f3d
TQID: 'https://experienceleague.adobe.com/UZHhTNCld6p1RFGh3DY-2r3VRiLNxCtP0anuPxPnWVE'
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: ae9127b0-c11d-467b-903d-a84cef43f6ed
    internal-label: Control Panel
  - id: c5474392-5419-4296-9e41-f6f4ce4f6e9b
    internal-label: Administration
subfeature_v2:
  - id: e8445399-14db-4931-a0bb-477780230387
    internal-label: SFTP Management
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
    internal-label: Intermediate
source-git-commit: b2723b0683a305a992b710a37a3e47927e1fb65e
workflow-type: tm+mt
source-wordcount: '168'
ht-degree: 100%
---
# SFTP の管理について {#about-sftp-management}

コントロールパネルでは、アクセス権のある Campaign インスタンスに接続されているすべての SFTP サーバーを操作できます。 ほとんどのインスタンスは SFTP サーバーに接続されています（場合によっては、開発インスタンスおよびステージインスタンスは、どの SFTP サーバーにも接続されていない可能性があります）。

SFTP サーバーへのアクセスは、SFTP クライアントソフトウェアを使用しておこなわれます。このソフトウェアは、オンラインで見つけてダウンロードできます。 このようなクライアントアプリケーションや API を使用してサーバーに接続するには、SSH 公開鍵を設定して、SFTP サーバーに接続する IP アドレスを許可リストに追加する必要があります。

コントロールパネルを使用すると、以下のアクションを実行して SFTP サーバーを管理できます。

* **ストレージ容量**&#x200B;を監視する。
* **IP アドレスの許可リストへの登録**&#x200B;を管理する。1 つまたは複数のサーバーの IP アドレス範囲を追加または削除します。
* サーバーにアクセスするための **SSH 公開鍵**&#x200B;を管理する。

これらの各アクションについて詳しくは、以下の節を参照してください。
