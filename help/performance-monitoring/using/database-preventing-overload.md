---
product: campaign
solution: Campaign
title: データベース容量超過の防止
description: Campaign ドキュメントに記載されているリソースにアクセスすると、インスタンス上のデータベース容量超過の防止に役立ちます。
feature: Control Panel
role: Architect
level: Experienced
exl-id: bb9e1ce3-2472-4bc1-a82a-a301c6bf830e
source-git-commit: 9accc4306bacab3bc27922f495c19138f905b1c5
workflow-type: tm+mt
source-wordcount: '189'
ht-degree: 100%

---

# データベース容量超過の防止 {#preventing-database-overload}

Campaign Standard および Campaign Classic では、様々な方法でデータベースのディスク容量の過剰消費を防ぐことができます。

以下の節では、データベース使用の最適化に役立つ Campaign ドキュメントのリソースを示します。

**ワークフローの監視**

* [ワークフローのベストプラクティス](https://experienceleague.adobe.com/docs/campaign-standard/using/managing-processes-and-data/workflow-general-operation/best-practices-workflows.html?lang=ja)（Campaign Standard）
* [監視ワークフローの実行](https://experienceleague.adobe.com/docs/campaign-classic/using/automating-with-workflows/monitoring-workflows/monitoring-workflow-execution.html?lang=ja)（Campaign Classic）

**データベースのメンテナンス**

* データベースクリーンアップのテクニカルワークフロー：[Campaign Standard](https://experienceleague.adobe.com/docs/campaign-standard/using/administrating/application-settings/technical-workflows.html?lang=ja#list-of-technical-workflows) - [Campaign Classic](https://experienceleague.adobe.com/docs/campaign-classic/using/monitoring-campaign-classic/data-processing/database-cleanup-workflow.html?lang=ja)
* [データベースメンテナンスガイド](https://experienceleague.adobe.com/docs/campaign-classic/using/monitoring-campaign-classic/database-maintenance/recommendations.html?lang=ja)（Campaign Classic）
* [データベースパフォーマンスのトラブルシューティング](https://experienceleague.adobe.com/docs/campaign-classic/using/monitoring-campaign-classic/troubleshooting-toc/database-issues-toc/database-performances.html?lang=ja)（Campaign Classic）
* [データベース関連オプション](https://experienceleague.adobe.com/docs/campaign-classic/using/installing-campaign-classic/appendices/configuring-campaign-options.html?lang=ja#database)（Campaign Classic）
* データ保持：[Campaign Standard](https://experienceleague.adobe.com/docs/campaign-standard/using/administrating/application-settings/data-retention.html?lang=ja) - [Campaign Classic](https://experienceleague.adobe.com/docs/campaign-classic/using/configuring-campaign-classic/data-model/data-model-best-practices.html?lang=ja#data-retention)

>[!NOTE]
>
>また、データベースの 1 つが最大容量に近づいた場合に通知を受け取ることもできます。これをおこなうには、[E メールアラート](../../performance-monitoring/using/email-alerting.md)を購読します。