---
title: SFTP ストレージ管理
description: SFTPサーバーのストレージを監視および管理する方法を説明します。
translation-type: tm+mt
source-git-commit: 111c8fd461f6f1c567288acd7a83aee5ef7fce97

---


# SFTP ストレージ管理 {#sftp-storage-management}

契約条項によっては、異なるストレージ容量を SFTP サーバーでプロビジョニングしている可能性があります。

各 SFTP サーバーの使用可能容量を定期的に監視することが重要です。そうしないと、サーバーに追加のファイルを保存できなくなったり、このサーバーからの更新に依存するワークフローを正常に実行できなくなったりする可能性があります。

**関連トピック：**

* [Campaign Standard チュートリアルビデオ](https://docs.adobe.com/content/help/en/campaign-learn/campaign-standard-tutorials/administrating/control-panel/managing-sftp-servers.html)
* [Campaign Classic チュートリアルビデオ](https://docs.adobe.com/content/help/en/campaign-learn/campaign-classic-tutorials/administrating/control-panel-acc/managing-sftp-servers.html)

## ストレージ容量情報へのアクセス {#accessing-storage-capacity-information}

ヘッダーの「**[!UICONTROL 最も使用された SFTP ディスク容量]」セクションには、管理者アクセス権のあるインスタンスに接続されている、最も使用された上位 3 つのサーバーが含まれています。**&#x200B;この情報は、SFTP カードのすべてのタブにあります。

![](assets/control_panel_topspaceNEW.png)

Information about the space used by all instances you have access to is available in the **[!UICONTROL Storage]** tab of the SFTP card. ページが更新されるたびに、このタブも更新されます。

![](assets/control_panel_spaceNEW.png)

各インスタンスに対して、視覚的なアラートによって、ストレージが容量を超えた場合に通知されます。

* **オレンジ**:この事例はその能力の80%を超えた
* **赤**:インスタンスはその容量の90%を超えています。

ストレージが容量に近づいた場合の処理方法を知るのに役立つヒントもあります。

## ストレージ容量がなくなった場合のベストプラクティス {#best-practices-when-capacity-runs-out}

1. **古いファイルまたは不要なファイルからSFTPサーバーを消去します**。 SFTP サーバーフォルダーへのアクセス方法については、[この節](../../sftp/using/logging-into-sftp-server.md)を参照してください。
1. SFTP サーバーをクリーンにする&#x200B;**ワークフロー**&#x200B;が正常に実行されていることを確認します。For more on technical workflows in Adobe Campaign, refer to the dedicated [Campaign Classic](https://docs.campaign.adobe.com/doc/AC/en/WKF__General_operation_Building_a_workflow.html#Technical_workflows) and [Campaign Standard](https://helpx.adobe.com/campaign/standard/administration/using/technical-workflows.html) documentations.
1. アカウントチームに問い合わせて、**より多くのストレージをリクエスト**&#x200B;します（追加料金がかかる場合があります）。
1. 問題があると思われる場合は、**カスタマーケア**&#x200B;にお問い合わせください。
