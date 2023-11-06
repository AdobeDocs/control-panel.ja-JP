---
product: campaign
solution: Campaign
title: アクティブなプロファイルの監視
description: 各キャンペーンインスタンスのアクティブなプロファイルの最新使用状況、使用履歴および変化に関するリアルタイム情報を取得する方法を説明します。
feature: Control Panel, Monitoring
role: Admin
level: Experienced
exl-id: a157cc27-577f-490f-8c4f-0f203219cfb5
source-git-commit: a3485766791387bd9422b4f29daf86296efafb98
workflow-type: ht
source-wordcount: '439'
ht-degree: 100%

---

# アクティブなプロファイルを監視 {#active-profiles-monitoring}

## アクティブなプロファイルについて {#about-active-profiles}

>[!IMPORTANT]
>
>コントロールパネルから使用できるアクティブなプロファイルの監視はベータ版です。通知なしに頻繁に更新および変更される可能性があります。Campaign Standard 10368 ビルドから利用できます。

各キャンペーンインスタンスには、契約に従って特定数のアクティブなプロファイルがプロビジョニングされ、課金のためその数がカウントされます。購入したアクティブなプロファイルの数については、最新の契約書を参照してください。

「プロファイル」とは、エンドユーザー、見込み客またはリードを表している情報のレコード（例：nmsRecipient テーブル内のレコードや、cookie ID、顧客 ID、モバイル ID、または特定のチャネルに関連するその他の情報が含まれている外部テーブル内のレコード）のことです。

過去 12 ヶ月間にいずれかのチャネルを介してターゲット設定されたまたは通信を受けたプロファイルが、アクティブなプロファイルと見なされます。

>[!NOTE]
>
>ただし、Facebook および Twitter チャネルは考慮されません。

アクティブなプロファイルについて詳しくは、[Campaign Standard](https://experienceleague.adobe.com/docs/campaign-standard/using/profiles-and-audiences/managing-profiles/active-profiles.html?lang=ja) と [Campaign v7／v8](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/profile-management/about-profiles.html?lang=ja#active-profiles) のドキュメントを参照してください。

## アクティブなプロファイルの使用状況の監視 {#monitoring-active-profiles}

>[!CONTEXTUALHELP]
>id="cp_performancemonitoring_active_profile"
>title="アクティブなプロファイルの監視について"
>abstract="このタブでは、Campaign インスタンスと組織ごとに、アクティブなプロファイルの使用状況と変化の最新情報や履歴がリアルタイムで表示されます。"

アクティブなプロファイルの使用状況に関連する情報は、インスタンスで毎日実行される専用の [!DNL Campaign] テクニカルワークフローに基づいて、コントロールパネルで更新されます。
* Campaign Standard の[「請求」](https://experienceleague.adobe.com/docs/campaign-standard/using/administrating/application-settings/technical-workflows.html?lang=ja)ワークフロー、
* Campaign v7／v8 の[「アクティブな請求プロファイルの数」](https://experienceleague.adobe.com/docs/campaign-classic/using/automating-with-workflows/advanced-management/about-technical-workflows.html?lang=ja)ワークフロー。


コントロールパネルでアクティブなプロファイルの使用状況を監視するには、「**[!UICONTROL パフォーマンス監視]**」カード／「**[!UICONTROL アクティブなプロファイル]**」タブに移動し、**[!UICONTROL インスタンスリスト]**&#x200B;から目的のインスタンスを選択します。

アクティブなプロファイルの使用状況に関する情報が表示されます。

![](assets/active-profiles-graph.png)

上部のセクションには、次の情報が表示されます。

* 選択したインスタンスで現在使用されているアクティブなプロファイルの数と、インスタンスに対する最新の請求ワークフロー実行のタイムスタンプ。

* すべてのインスタンス内の組織全体で使用されているアクティブなプロファイルの合計数。

  >[!NOTE]
  >
  >このセクションは、組織に複数のインスタンスが関連付けられている場合にのみ表示されます。

* 組織に割り当てられたアクティブなプロファイルの合計数。

下部のセクションには、過去 30 日間のアクティブなプロファイルの使用状況が視覚的に表示されます。右上隅にあるフィルターを使用して、この期間を 1 年に変更できます。右上隅にあるフィルターを使用すると、この時間枠を 1 年に変更できます。グラフにカーソルを合わせると、選択した期間に使用されたアクティブなプロファイルの正確な数を取得できます。
