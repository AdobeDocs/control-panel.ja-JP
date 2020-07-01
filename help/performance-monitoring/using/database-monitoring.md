---
title: データベース監視
description: コントロールパネルでの Campaign データベースの監視方法の詳細
translation-type: ht
source-git-commit: b2447b30314f4bd46b2b6e144f7f713ff2f1ec59
workflow-type: ht
source-wordcount: '450'
ht-degree: 100%

---


# データベース監視 {#database-monitoring}

## インスタンスデータベースについて {#about-instances-databases}

各 Campaign インスタンスには、契約に従って特定の容量のデータベースがプロビジョニングされます。

データベースには、Adobe Campaign に保存されるすべての&#x200B;**アセット**、**ワークフロー**、**データ**&#x200B;が含まれます。

特に、格納されたリソースがインスタンスからまったく削除されていない場合や、一時停止状態のワークフローが多数ある場合には、時間の経過と共に、データベースが最大容量に達してしまう可能性があります。

インスタンスデータベースの容量が足りなくなると、複数の問題（ログインや E メール送信ができないなど）が発生する可能性があります。したがって、最適なパフォーマンスを確保するには、インスタンスのデータベースを監視する必要があります。

>[!NOTE]
>
>Campaign コントロールパネルに表示されるデータベース容量は、契約で指定されたデータベース容量を反映していない場合があります。ほとんどの場合、システムのパフォーマンスを確保するために、大きなデータベース容量が一時的に提供されます。

## データベース使用状況の監視 {#monitoring-instances-database}

Campaign コントロールパネルでは、各 Campaign インスタンスのデータベースの使用状況を監視できます。それには、次の手順に従います。

1. 「**[!UICONTROL パフォーマンス監視]**」カードを開き、「**[!UICONTROL データベース]**」タブを選択します。

1. **[!UICONTROL インスタンスリスト]**&#x200B;から目的のインスタンスを選択します。

   上部に、インスタンスのデータベース容量および使用中の容量に関する情報が表示されます。

   ![](assets/databases_dashboard.png)

   下部に、過去 7 日間のデータベースの最小使用率、平均使用率、最大使用率のグラフが表示され、データベース使用率 90% のしきい値が赤い点線の曲線で示されます。

   右上隅にあるフィルターを使用すると、表示される期間を変更できます。

   グラフ内の 1 つまたは複数の曲線をハイライト表示して、読みやすくすることもできます。これをおこなうには、「**[!UICONTROL 集計タイプ]**」の凡例から曲線を選択します。

   グラフの上にマウスポインターを置くと、選択した期間についての詳細な情報を取得できます。

   ![](assets/databases_dashboard_detail.png)

>[!NOTE]
>
>また、このダッシュボードに加え、データベースが最大容量に近づいた場合に通知を受け取ることもできます。これをおこなうには、[E メールアラート](../../performance-monitoring/using/email-alerting.md)を購読します

## データベース容量超過の防止 {#preventing-database-overload}

Campaign Standard および Campaign Classic では、様々な方法でデータベースのディスク容量の過剰消費を防ぐことができます。

以下の節では、データベース使用の最適化に役立つ Campaign ドキュメントのリソースを示します。

**ワークフローの監視**

* [ワークフローのベストプラクティス](https://docs.adobe.com/content/help/ja-JP/campaign-standard/using/managing-processes-and-data/workflow-general-operation/best-practices-workflows.html)（Campaign Standard）
* [監視ワークフローの実行](https://docs.adobe.com/help/ja-JP/campaign-classic/using/automating-with-workflows/monitoring-workflows/monitoring-workflow-execution.html)（Campaign Classic）

**データベースのメンテナンス**

* データベースクリーンアップテクニカルワークフロー（[Campaign Standard](https://docs.adobe.com/help/ja-JP/campaign-standard/using/administrating/application-settings/technical-workflows.html#list-of-technical-workflows)／[Campaign Classic](https://docs.adobe.com/help/ja-JP/campaign-classic/using/monitoring-campaign-classic/data-processing/database-cleanup-workflow.html)）
* [データベースメンテナンスガイド](https://docs.adobe.com/content/help/ja-JP/campaign-classic/using/monitoring-campaign-classic/database-maintenance/recommendations.html)（Campaign Classic）
* [データベースパフォーマンスのトラブルシューティング](https://docs.adobe.com/content/help/ja-JP/campaign-classic/using/monitoring-campaign-classic/troubleshooting/database-performances.html)（Campaign Classic）
* [データベース関連オプション](https://docs.adobe.com/help/ja-JP/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options.html#database)（Campaign Classic）
