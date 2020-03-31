---
title: データベースの監視
description: コントロールパネルでキャンペーンデータベースを監視する方法
translation-type: tm+mt
source-git-commit: f995e0dc51fd95d00fdcaa2eb347b2aedfdef60d

---


# データベースの監視 {#database-monitoring}

## インスタンスデータベースについて {#about-instances-databases}

契約に従って、各データベースインスタンスには、キャンペーンの特定の容量のデータベースがプロビジョニングされます。

データベースには、Adobe Campaignに保 **存されている****ワークフロー****** 、アセット、データ、データがすべて含まれます。

データベースの最大容量に達するまで時間がかかります。特に、格納されたリソースがインスタンスから削除されない場合や、一時停止状態のワークフローが多い場合には、データベースが最大容量に達します。

インスタンスデータベースをオーバーフローすると、いくつかの問題（ログインできない、電子メールの送信など）が発生する可能性があります。 したがって、最適なパフォーマンスを確保するには、インスタンスのデータベースを監視する必要があります。

>[!NOTE]
>
>パフォーマンスを高めるために、現在のデータベースの容量と、異なる期間に指定した容量との間に多少の相違が生じる可能性があります。

## データベースの使用状況の監視 {#monitoring-instances-database}

1. カードを **[!UICONTROL Health Monitoring]** 開き、タブを選択し **[!UICONTROL Databases]** ます。

1. から目的のインスタンスを選択しま **[!UICONTROL Instance List]**&#x200B;す。

   上の領域は、インスタンスのデータベース容量と使用領域に関する情報を提供します。

   ![](assets/databases_dashboard.png)

   下の領域には、過去7日間のデータベースの使用率が図式的に表示されます。 右上隅の使用可能なフィルターを使用して、表示期間を変更できます。

   グラフの上にマウスポインターを置くと、選択した期間の詳細情報を取得できます。

   ![](assets/databases_dashboard_detail.png)

## データベースの過負荷の防止 {#preventing-database-overload}

Campaign Standardと従来のオファーでは、データベースのディスク領域の過剰消費を防ぐ様々な方法を使用します。

以下の節では、データベースの使用を最適化するのに役立つキャンペーンドキュメントのリソースを示します。

**ワークフロー監視**

* [ワークフローのベストプラクティス](https://docs.adobe.com/content/help/en/campaign-standard/using/managing-processes-and-data/workflow-general-operation/best-practices-workflows.html) (Campaign Standard)
* [監視ワークフローの実行](https://docs.adobe.com/help/en/campaign-classic/using/automating-with-workflows/monitoring-workflows/monitoring-workflow-execution.html) (Campaign Classic)

**データベースメンテナンス**

* データベースのクリーンアップ技術ワ[ークフ](https://docs.adobe.com/help/en/campaign-standard/using/administrating/application-settings/technical-workflowshtml#list-of-technical-workflows) ロー [(](https://docs.adobe.com/help/en/campaign-classic/using/monitoring-campaign-classic/data-processing/database-cleanup-workflow.html)Campaign Standard/Campaign Classic)
* [データベースメンテナンスガイド](https://docs.adobe.com/content/help/en/campaign-classic/using/monitoring-campaign-classic/database-maintenance/recommendations.html) (Campaign Classic)
* [データベースのパフォーマンスのトラブルシューティング](https://docs.adobe.com/content/help/en/campaign-classic/using/monitoring-campaign-classic/troubleshooting/database-performances.html) (Campaign Classic)
* [データベース関連のオプション](https://docs.adobe.com/help/en/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options.html#database) (Campaign Classic)
