---
product: campaign
solution: Campaign
title: ストレージの概要
description: インスタンス上のデータベース容量を消費している様々な Campaign リソースをコントロールパネルで監視する方法を説明します。
feature: Control Panel, Monitoring
role: Admin
level: Experienced
exl-id: bb9e1ce3-2472-4bc1-a82a-a301c6bf830e
source-git-commit: a3485766791387bd9422b4f29daf86296efafb98
workflow-type: ht
source-wordcount: '0'
ht-degree: 100%

---

# ストレージの概要 {#storage-overview}

>[!CONTEXTUALHELP]
>id="cp_dbdetails_storagedetails"
>title="ストレージの概要について"
>abstract="このタブでは、データベース容量を消費している様々な Campaign リソースの詳細が表示されます。"

**[!UICONTROL ストレージの概要]**&#x200B;領域には、以下が占める容量のグラフが表示されます。

* **[!UICONTROL システムリソース]**

  システムリソースがデータベース容量の大部分を消費している場合は、カスタマーケアに連絡することをお勧めします。

* デフォルトで Campaign インスタンスに付属している&#x200B;**[!UICONTROL 標準のテーブル]**
* ワークフローと配信によって作成される&#x200B;**[!UICONTROL 一時的テーブル]**
* カスタムリソースの作成後に生成される&#x200B;**[!UICONTROL 非標準のテーブル]**

![](assets/database-storage-overview.png)

データベース容量を消費している様々なアセットの詳細を表示するには、「**[!UICONTROL 詳細を表示]**」ボタンをクリックします。

ドロップダウンリストを使用して検索を絞り込み、特定のアセットタイプ（ワークフロー、配信、受信者）のテーブルのみを表示できます。

![](assets/database-storage-details.png)

またこの画面では、インスタンスに関する問題を回避するために、特に注意が必要となる可能性のあるワークフローパラメーターを監視できます。 詳しくは、[このページ](workflow-monitoring.md)を参照してください。
