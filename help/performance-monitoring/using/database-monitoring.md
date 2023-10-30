---
product: campaign
solution: Campaign
title: データベース監視について
description: コントロールパネルでの Campaign データベースの監視方法について
feature: Control Panel, Monitoring
role: Admin
level: Experienced
exl-id: 2bd7d2dd-97be-49bb-9f8e-7161d0742bc1
source-git-commit: a3485766791387bd9422b4f29daf86296efafb98
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 100%

---

# データベース監視について {#database-monitoring}

## インスタンスのデータベースについて {#about-instances-databases}

各 Campaign インスタンスには、契約に従って特定の容量のデータベースがプロビジョニングされます。データベースには、Adobe Campaign に保存されるすべての&#x200B;**アセット**、**ワークフロー**、**データ**&#x200B;が含まれます。

特に、格納されたリソースがインスタンスからまったく削除されていない場合や、一時停止状態のワークフローが多数ある場合には、時間の経過と共に、データベースが最大処理能力に達してしまう可能性があります。

インスタンスデータベースの容量が足りなくなると、複数の問題（ログインやメール送信ができないなど）が発生する可能性があります。したがって、最適なパフォーマンスを確保するには、インスタンスのデータベースを監視する必要があります。

[メールアラート](../../performance-monitoring/using/email-alerting.md)を購読している場合、いずれかのインスタンスでデータベースの処理能力が 80%以上に達すると、メールで通知が届きます。

## データベース使用量の監視{#monitoring-database-usage}

>[!CONTEXTUALHELP]
>id="cp_performancemonitoring_database"
>title="データベース監視について"
>abstract="このタブでは、Campaign インスタンスごとに、データベースの使用状況と変化の最新情報や履歴がリアルタイムで表示されます。"
>additional-url="https://experienceleague.adobe.com/docs/control-panel/using/performance-monitoring/about-performance-monitoring.html?lang=ja" text="パフォーマンス監視について"

コントロールパネルでは、各 Campaign インスタンスのデータベース使用量を監視できます。これをおこなうには、「**[!UICONTROL パフォーマンス監視]**」カードを開き、「**[!UICONTROL データベース]**」タブを選択します。

「**[!UICONTROL インスタンスリスト]**」から目的のインスタンスを選択し、インスタンスのデータベース処理能力と使用中の容量に関する情報を表示します。

>[!NOTE]
>
>コントロールパネルに示されている利用可能なデータベース容量が、契約で指定されている容量を反映していない場合は、カスタマーケアにお問い合わせください。

![](assets/databases_dashboard.png)

このダッシュボードのデータは、Campaign インスタンスで実行される&#x200B;**[!UICONTROL データベースクリーンアップテクニカルワークフロー]**（[Campaign Standard](https://experienceleague.adobe.com/docs/campaign-standard/using/administrating/application-settings/technical-workflows.html?lang=ja#list-of-technical-workflows) および [Campaign v7／v8](https://experienceleague.adobe.com/docs/campaign-classic/using/monitoring-campaign-classic/data-processing/database-cleanup-workflow.html?lang=ja) のドキュメントを参照）に基づいて更新されます。最後にワークフローが実行された時間は、「**[!UICONTROL 使用中の容量]**」および「**[!UICONTROL 提供された容量]**」指標の下で確認できます。ワークフローが 3 日を超えて実行されていない場合は、ワークフローが実行されない理由が調査されるように、アドビカスタマーケアに連絡することをお勧めします。

このダッシュボードでは、インスタンスのデータベースの使用状況を分析するのに役立つ追加の指標を利用できます。これらの詳細については以下の節で説明します。

* [データベース使用率](../../performance-monitoring/using/database-utilization.md)
* [ストレージの概要](../../performance-monitoring/using/database-storage-overview.md)
* [一時的リソース上位 10 位](../../performance-monitoring/using/database-top-ten-resources.md)
* [アクティブなクエリ](../../performance-monitoring/using/database-active-queries.md)

![](assets/do-not-localize/how-to-video.png)[Campaign v7／v8](https://experienceleague.adobe.com/docs/campaign-classic-learn/control-panel/performance-monitoring/monitoring-databases.html?lang=ja#performance-monitoring) または [Campaign Standard](https://experienceleague.adobe.com/docs/campaign-standard-learn/control-panel/performance-monitoring/monitoring-databases.html?lang=ja#performance-monitoring) を使用して、ビデオでこの機能を確認
