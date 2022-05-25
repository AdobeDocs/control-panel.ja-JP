---
product: campaign
solution: Campaign
title: インスタンスの詳細
description: コントロールパネルでのインスタンスの詳細の監視方法
feature: Control Panel
role: Architect
level: Experienced
exl-id: 02819bfc-9886-43fc-8014-9bfe64c42048
source-git-commit: 3f68145c40f40df3e69f4fdfd889f3a7a2e995ab
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 100%

---

# インスタンスの詳細 {#instance-details}

>[!CONTEXTUALHELP]
>id="cp_instancesettings_instancedetails"
>title="インスタンスの詳細について"
>abstract="Adobe Campaign インスタンスの詳細（タイプ、名前、ビルド情報および適用可能な推奨アップグレード）を表示します。"

## インスタンスの詳細について {#about-instance-details}

>[!IMPORTANT]
>
>この機能は、Campaign v7／v8 のインスタンスでのみ使用できます。

Adobe Campaign インスタンスアーキテクチャには複数のサーバーを含めることができるので、柔軟なマーケティング活動が可能になります。例えば、マーケティングサーバー、リアルタイム（Message Center）サーバー、ミッドソーシングサーバーをインスタンスと連係させることができます。

「インスタンスの詳細」機能を利用すると、インスタンスのフラットアーキテクチャを表示できます。サーバー情報が得られるほか、インスタンスのビルドが最新かどうかもわかります。さらに、必要に応じてアップグレードも提案されます。

>[!NOTE]
>
>パフォーマンスの低下を避け、Adobe Campaign v7／v8 から提供される最新の機能や修正を活用できるようにするため、少なくとも年に 1 回はインスタンスをアップグレードすることをお勧めします。

**関連トピック：**

* [ビルドアップグレードの実行](https://docs.campaign.adobe.com/doc/AC/getting_started/JA/buildUpgrade.html)
* [Adobe Campaign の更新](https://docs.campaign.adobe.com/doc/AC/en/PRO_Updating_Adobe_Campaign_Introduction.html)

## インスタンスに関する情報の取得 {#retrieving-information-about-instances}

お使いのインスタンスに接続しているサーバーに関する情報を取得するには、次の手順に従います。

1. 「**[!UICONTROL インスタンス設定]**」カードを開き、「**[!UICONTROL インスタンスの詳細]**」タブにアクセスします。

   >[!NOTE]
   >
   >インスタンスの設定カードがコントロールパネルのホームページに表示されない場合、IMS 組織 ID は、 Adobe Campaign v7／v8 インスタンスに関連付けられていません。

1. 左側のペインから目的の Campaign インスタンスを選択します。

   >[!NOTE]
   >
   >左側のペインのリストには、すべての Campaign インスタンスが表示されます。「インスタンスの詳細」機能は、Campaign v7／v8 インスタンス専用です。Campaign Standard インスタンスを選択すると、「適用外のインスタンス」というメッセージが表示されます。

1. インスタンスに接続しているサーバーが表示されます。

   ![](assets/instance_details.png)

入手できる情報は次のとおりです。

* **[!UICONTROL タイプ]**：サーバーのタイプ。値は MKT（マーケティング）、MID（ミッドソーシング）、RT（Message Center / リアルタイムメッセージング）のいずれかです。
* **[!UICONTROL 名前]**：サーバーの名前。
* **[!UICONTROL ビルド：]**&#x200B;サーバーにインストールされているビルドバージョン。
* **[!UICONTROL アップグレード情報]**：サーバーの更新が必要かどうかを示します。
   * 緑：サーバーは最新です。アップグレードは必要ありません。
   * 黄：アップグレードを検討する必要があります。最新の機能や修正を利用できません。
   * 赤：できるだけ早くアップグレードする必要があります。最新の機能を利用できないほか、サーバーのパフォーマンスが最適でない可能性があります。

サーバーのいずれかをアップグレードする必要がある場合は、[こちらのドキュメント](https://docs.campaign.adobe.com/doc/AC/getting_started/EN/buildUpgrade.html)を参照して、作業方法の詳細を確認してください。

## よくある質問 {#common-questions}

**インスタンスアーキテクチャに MID サーバーが表示されないのですが、これは、インスタンスが正常に機能していないということですか？現時点ではできない処理を実行するために RT インスタンスが必要なのでしょうか？**

インスタンスの構成は、大幅に異なる場合があります。すべてのタイプのサーバーが含まれていないこともあれば、同じタイプのサーバーが複数含まれていることもあります。いずれかのタイプのサーバーが含まれていないからと言って、リアルタイムメッセージ送信やほかのタイプのアクティビティを実行できないわけではありません。サーバー処理能力の増強を依頼することも可能です。ただし、追加料金がかかります。

一部のサーバーが「インスタンスの詳細」ページに表示されていないとお考えの場合は、カスタマーサポートにお問い合わせください。その際には、具体的なインスタンス URL をメッセージに必ず記載してください。
