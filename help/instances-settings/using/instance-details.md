---
title: インスタンスの詳細
description: コントロールパネルでのインスタンスの詳細の監視方法
translation-type: tm+mt
source-git-commit: f22e356b283ee2601c948d5c1d514a9a59c58451

---


# インスタンスの詳細{#instance-details}

>[!CONTEXTUALHELP]
>id=&quot;cp_instancesettings_instancedetails&quot;
>title=&quot;インスタンスの詳細について&quot;
>abstract=&quot;Adobe Campaignインスタンスの詳細を表示します。タイプ、名前、ビルド情報、およびアップグレードの推奨事項を示します。」
>additional-url=&quot;https://docs.adobe.com/content/help/en/campaign-classic/using/release-notes/latest-release.html&quot; text=&quot;Campaign Classicリリースノート&quot;
>additional-url=&quot;https://docs.adobe.com/content/help/en/campaign-standard/using/release-notes/release-notes.html&quot; text=&quot;Campaign Standardリリースノート&quot;

>[!CAUTION]
>
>この機能は、Campaign Classic インスタンスでのみ使用できます。

## インスタンスの詳細について{#about-instance-details}

Adobe Campaign Classic インスタンスアーキテクチャには複数のサーバーを含めることができるので、柔軟なマーケティング活動が可能になります。例えば、マーケティングサーバー、リアルタイム（Message Center）サーバー、ミッドソーシングサーバーでインスタンスをサポートすることができます。

「インスタンスの詳細」機能を利用すると、インスタンスのフラットアーキテクチャを表示できます。サーバー情報が得られるほか、インスタンスのビルドが最新かどうかもわかります。さらに、必要に応じてアップグレードも提案されます。

>[!NOTE]
>
>パフォーマンスの低下を避け、Adobe Campaign Classic から提供される最新の機能や修正を活用できるようにするため、少なくとも年に 1 回はインスタンスをアップグレードすることをお勧めします。

**関連トピック：**

* [ビルドアップグレードの実行](https://docs.campaign.adobe.com/doc/AC/getting_started/EN/buildUpgrade.html)
* [Adobe Campaign の更新](https://docs.campaign.adobe.com/doc/AC/en/PRO_Updating_Adobe_Campaign_Introduction.html)

## インスタンスに関する情報の取得{#retrieving-information-about-instances}

お使いのインスタンスに接続しているサーバーに関する情報を取得するには、次の手順に従います。

1. カードを開 **[!UICONTROL Instances Settings]** いてタブにアクセス **[!UICONTROL Instance Details]** します。

   >[!NOTE]
   >
   >「インスタンス設定」カードがコントロールパネルのホームページに表示されない場合、お使いの IMS ORG ID は、Adobe Campaign Classic インスタンスに関連付けられていません。

1. 左側のパネルから目的の Campaign Classic インスタンスを選択します。

   >[!NOTE]
   >
   >左側のパネルのリストには、すべての Campaign インスタンスが表示されます。「インスタンスの詳細」機能は、Campaign Classic インスタンス専用です。Campaign Standard インスタンスを選択すると、「適用外のインスタンス」というメッセージが表示されます。

1. インスタンスに接続しているサーバーが表示されます。

   ![](assets/instance_details.png)

入手できる情報は次のとおりです。

* **[!UICONTROL Type]**:サーバーのタイプ。 値は MKT（マーケティング）、MID（ミッドソーシング）、RT（Message Center / リアルタイムメッセージング）のいずれかです。
* **[!UICONTROL Name]**:サーバーの名前。
* **[!UICONTROL Build:]** サーバーにインストールされているビルドバージョン。
* **[!UICONTROL Upgrade info]**:この列は、サーバーに更新が必要な場合に通知します。
   * 緑：サーバーは最新です。アップグレードは必要ありません。
   * 黄：アップグレードを検討する必要があります。最新の機能や修正を利用できません。
   * 赤：できるだけ早くアップグレードする必要があります。最新の機能を利用できないほか、サーバーのパフォーマンスが最適でない可能性があります。

サーバーのいずれかをアップグレードする必要がある場合は、[こちらのドキュメント](https://docs.campaign.adobe.com/doc/AC/getting_started/EN/buildUpgrade.html)を参照して、作業方法の詳細を確認してください。

## よくある質問{#common-questions}

**インスタンスアーキテクチャに MID サーバーが表示されないのですが、これは、インスタンスが正常に機能していないということですか？現時点ではできないことを実行するのに RT インスタンスが必要なのでしょうか？**

インスタンスの構成は、大幅に異なる場合があります。すべてのタイプのサーバーが含まれていないこともあれば、同じタイプのサーバーが複数含まれていることもあります。いずれかのタイプのサーバーが含まれていないからと言って、リアルタイムメッセージ送信やほかのタイプのアクティビティを実行できないわけではありません。サーバー処理能力の増強を依頼することも可能です。ただし、追加料金がかかります。

確かに一部のサーバーが「インスタンスの詳細」ページに表示されていないようでしたら、カスタマーサポートにお問い合わせください。その際には、具体的なインスタンス URL をメッセージに必ず記載してください。
