---
product: campaign
solution: Campaign
title: 一時的リソース上位 10 位
description: Campaign データベース上のワークフローと配信で生成された一時的リソース上位 10 位をコントロールパネルで監視する方法を説明します。
feature: Control Panel, Monitoring
role: Admin
level: Experienced
exl-id: 2fa2ffbb-102b-42c4-8feb-b0263ee9c930
source-git-commit: a3485766791387bd9422b4f29daf86296efafb98
workflow-type: tm+mt
source-wordcount: '182'
ht-degree: 100%

---

# 一時的リソース上位 10 位 {#top-10}

**[!UICONTROL 一時的リソース上位 10 位]**&#x200B;領域には、ワークフローと配信によって生成された 10 個の最大の一時的リソースがリストされます。

大きな一時的リソースを作成しているワークフローや配信を監視することは、データベースを監視するための重要な手順です。一時的リソースがデータベース容量を消費しすぎる場合は、このワークフローまたは配信が必要であることを確認し、最終的にインスタンスに移動して停止します。

>[!IMPORTANT]
>
>一般的なレコメンデーションは、非標準リソースが **40 列を超えない**&#x200B;ようにすることです。ワークフローに多数のテーブルが存在する、またはデータベースサイズが大きい場合は、ワークフローを確認して、大量のデータが生成される理由を調べることをお勧めします。
>
>Campaign Standard と Classic のガイドラインは、[このページ](database-preventing-overload.md)を使用して、データベース容量超過を防ぐことができます。

![](assets/database-top10.png)

この「**[!UICONTROL すべて表示]**」ボタンをクリックすると、**[!UICONTROL ストレージの概要]**&#x200B;の詳細にアクセスしてこれらの一時的リソースの詳細情報を取得することができます。詳しくは、[このページ](database-storage-overview.md)を参照してください。
