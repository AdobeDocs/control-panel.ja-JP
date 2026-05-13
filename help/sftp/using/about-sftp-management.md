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
TQID: https://experienceleague.adobe.com/UZHhTNCld6p1RFGh3DY-2r3VRiLNxCtP0anuPxPnWVE
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
source-git-commit: 06babfad697fb874f2b77c5204e30580c55cd0d1
workflow-type: tm+mt
source-wordcount: 168
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
