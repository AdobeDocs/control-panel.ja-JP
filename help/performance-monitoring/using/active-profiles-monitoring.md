---
title: アクティブなプロファイルの監視
description: 各キャンペーンインスタンスの最新および過去のアクティブプロファイルの使用状況と進化状況に関するリアルタイム情報を取得する方法を説明します。
translation-type: tm+mt
source-git-commit: 024eb750021ff2446b34d648b5abfb016eabc289
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 17%

---


# アクティブなプロファイルの監視 {#active-profiles-monitoring}

>[!IMPORTANT]
>
>コントロールパネルでのアクティブなプロファイルの監視は、ベータ版で利用できます。通常、更新や変更が予告なく行われます。
>
>この機能は、Campaign Standard10368のビルドとCampaign Classic8931のビルドから、AWSでホストされるお客様が利用できます。 以前のビルドを使用している場合は、この機能を使用するにはアップグレードする必要があります。

## アクティブなプロファイルについて {#about-active-profiles}

契約に従って、各キャンペーンインスタンスには、請求の目的でカウントされる特定の量のアクティブなプロファイルがプロビジョニングされます。 購入したアクティブなプロファイルの数については、最新の契約書を参照してください。

「プロファイル」とは、エンドユーザー、見込み客またはリードを表している情報のレコード（例：nmsRecipient テーブル内のレコードや、cookie ID、顧客 ID、モバイル ID、または特定のチャネルに関連するその他の情報が含まれている外部テーブル内のレコード）のことです。

プロファイルが、過去12か月間に何らかのチャネルを介してターゲット設定または通信を受けた場合、アクティブと見なされます。

>[!NOTE]
>
>ただし、Facebook および Twitter チャネルは考慮されません。

アクティブなプロファイルについて詳しくは、 [Campaign Standard](https://docs.adobe.com/content/help/en/campaign-standard/using/profiles-and-audiences/managing-profiles/active-profiles.html) および [Campaign Classicのドキュメントを参照してください](https://docs.adobe.com/content/help/en/campaign-classic/using/getting-started/profile-management/about-profiles.html#active-profiles) 。

## アクティブなプロファイルの監視 {#monitoring-active-profiles}

コントロールパネルでは、各キャンペーンインスタンスのアクティブなプロファイルの使用状況を監視できます。

それには、次の手順に従います。

1. Open the **[!UICONTROL Performance Monitoring]** card, then select the **[!UICONTROL Active Profiles]** tab.

1. **[!UICONTROL インスタンスリスト]**&#x200B;から目的のインスタンスを選択します。

1. インスタンスが使用するアクティブなプロファイルの数、および最後に請求ワークフローがインスタンスで実行された時間が表示されます。

![](assets/active-profiles-graph.png)

>[!NOTE]
>
>アクティブなプロファイルは、インスタンスで毎日実行される専用のテクニカルワークフローに基づいてカウントされます。
>
>* Campaign Standard [のための「請求」](https://docs.adobe.com/help/ja-JP/campaign-standard/using/administrating/application-settings/technical-workflows.html) ワークフロー、
>* Campaign Classicのた [めの「アクティブな請求プロファイルの数」](https://docs.adobe.com/content/help/en/campaign-classic/using/automating-with-workflows/technical-workflows/deliveries.html) ワークフロー。


下の領域には、過去30日間のアクティブなプロファイルの使用状況がグラフィカルに表示されます。 右上隅のフィルターを使用して、表示期間を1年に変更できます。

グラフのバーの1つにカーソルを重ねると、選択した期間に使用されたアクティブなプロファイルの正確な数を取得できます。
