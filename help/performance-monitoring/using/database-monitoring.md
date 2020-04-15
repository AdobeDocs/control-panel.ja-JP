---
title: データベース監視
description: コントロールパネルでの Campaign データベースの監視方法の詳細
translation-type: tm+mt
source-git-commit: 77165e3f408f75dfb57434111b07b20ad9caab5e

---


# データベース監視 {#database-monitoring}

>[!IMPORTANT]
>
>コントロール・パネルでのデータベース監視は、4月末までに利用可能になります。

## インスタンスデータベースについて {#about-instances-databases}

各 Campaign インスタンスには、契約に従って特定の容量のデータベースがプロビジョニングされます。

データベースには、Adobe Campaign に保存されるすべての&#x200B;**アセット**、**ワークフロー**、**データ**&#x200B;が含まれます。

特に、格納されたリソースがインスタンスからまったく削除されていない場合や、一時停止状態のワークフローが多数ある場合には、時間の経過と共に、データベースが最大容量に達してしまう可能性があります。

インスタンスデータベースの容量が足りなくなると、複数の問題（ログインや E メール送信ができないなど）が発生する可能性があります。したがって、最適なパフォーマンスを確保するには、インスタンスのデータベースを監視する必要があります。

>[!NOTE]
>
>コントロールパネルに表示されるデータベース領域の量は、契約で指定されたデータベース領域の量を反映していない場合があります。 ほとんどの場合、システムのパフォーマンスを確保するために、大きなデータベース領域が一時的に提供されます。

## データベース使用状況の監視 {#monitoring-instances-database}

コントロールパネルでは、各データベースインスタンスのデータベースの使用状況をキャンペーンできます。 それには、次の手順に従います。

1. カードを **[!UICONTROL Performance Monitoring]** 開き、タブを選択し **[!UICONTROL Databases]** ます。

1. Select the desired instance from the **[!UICONTROL Instance List]**.

   上部に、インスタンスのデータベース容量および使用中の容量に関する情報が表示されます。

   ![](assets/databases_dashboard.png)

   下の領域には、過去7日間のデータベースの最小使用率、平均使用率、最大使用率のグラフが表示され、データベース使用率の90%のしきい値が赤い点線の曲線で示されます。

   右上隅にあるフィルターを使用すると、表示される期間を変更できます。

   グラフ内の1つまたは複数のカーブをハイライト表示して、読みやすくすることもできます。 これを行うには、凡例から選択し **[!UICONTROL Aggregation Type]** ます。

   グラフの上にマウスポインターを置くと、選択した期間についての詳細な情報を取得できます。

   ![](assets/databases_dashboard_detail.png)

>[!NOTE]
>
>また、このダッシュボードに加えて、データベースの1つがその容量に達した場合に通知を受け取ることもできます。 これを行うには、電子メールアラートを [登録します](../../performance-monitoring/using/email-alerting.md)

## データベース容量超過の防止 {#preventing-database-overload}

Campaign Standard および Campaign Classic では、様々な方法でデータベースのディスク容量の過剰消費を防ぐことができます。

以下の節では、データベース使用の最適化に役立つ Campaign ドキュメントのリソースを示します。

**ワークフローの監視**

* [ワークフローのベストプラクティス](https://docs.adobe.com/content/help/ja-JP/campaign-standard/using/managing-processes-and-data/workflow-general-operation/best-practices-workflows.html)（Campaign Standard）
* [監視ワークフローの実行](https://docs.adobe.com/help/ja-JP/campaign-classic/using/automating-with-workflows/monitoring-workflows/monitoring-workflow-execution.html)（Campaign Classic）

**データベースのメンテナンス**

* データベースクリーンアップテクニカルワークフロー（[Campaign Standard](https://docs.adobe.com/help/en/campaign-standard/using/administrating/application-settings/technical-workflows.html#list-of-technical-workflows)／[Campaign Classic](https://docs.adobe.com/help/ja-JP/campaign-classic/using/monitoring-campaign-classic/data-processing/database-cleanup-workflow.html)）
* [データベースメンテナンスガイド](https://docs.adobe.com/content/help/ja-JP/campaign-classic/using/monitoring-campaign-classic/database-maintenance/recommendations.html)（Campaign Classic）
* [データベースパフォーマンスのトラブルシューティング](https://docs.adobe.com/content/help/ja-JP/campaign-classic/using/monitoring-campaign-classic/troubleshooting/database-performances.html)（Campaign Classic）
* [データベース関連オプション](https://docs.adobe.com/help/ja-JP/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options.html#database)（Campaign Classic）
