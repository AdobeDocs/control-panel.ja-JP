---
product: campaign
solution: Campaign
title: MID/RT インスタンスの追加（ハイブリッドモデル）
description: ハイブリッドホスティングモデルで MID/RT インスタンスをCampaign コントロールパネルに追加する方法を説明します。
feature: Control Panel
role: Architect
level: Intermediate
source-git-commit: 2458263ef5981a16d983912b498e320501df7889
workflow-type: tm+mt
source-wordcount: '482'
ht-degree: 38%

---


# MID/RT インスタンスの追加（ハイブリッドモデル）

>[!CONTEXTUALHELP]
>id="cp_externalaccounts"
>title="外部アカウント"
>abstract="この画面では、ハイブリッドホスティングモデルを使用するお客様は、Campaign コントロールパネル機能を活用するために、Campaign コントロールパネルのマーケティングインスタンスで設定された MID/RT インスタンス URL を指定できます。"

Campaign コントロールパネルを使用すると、ハイブリッドホスティングモデルを使用して、特定のCampaign コントロールパネル機能を利用できます。 これをおこなうには、Campaign コントロールパネルでマーケティングインスタンスに設定した MID/RT インスタンス URL を指定する必要があります。

モデルのホスティングについて詳しくは、[Campaign Classic ドキュメント](https://experienceleague.adobe.com/docs/campaign-classic/using/installing-campaign-classic/architecture-and-hosting-models/hosting-models-lp/hosting-models.html?lang=ja)を参照してください。

## MID/RT インスタンスを追加 {#add}

>[!CONTEXTUALHELP]
>id="cp_externalaccounts_url"
>title="URL"
>abstract="インスタンスの URL。Campaign クライアントコンソールの管理/プラットフォーム/外部アカウントメニューにあります。"

>[!CONTEXTUALHELP]
>id="cp_externalaccounts_operator"
>title="演算子"
>abstract="Adobe管理者による最初のプロビジョニング後に提供されたオペレーターの ID。"

>[!CONTEXTUALHELP]
>id="cp_externalaccounts_password"
>title="パスワード"
>abstract="Adobe管理者による最初のプロビジョニング後に指定されたオペレーターのパスワード。"

ハイブリッド顧客は、Experience Cloudを通じてCampaign コントロールパネルに接続する必要があります。 初めてコントロールパネルにアクセスする場合、ホームページには 2 枚のカードのみが表示されます。

![](assets/hybrid-homepage.png)

>[!NOTE]
>
>コントロールパネルにアクセスする際に問題が発生した場合は、マーケティングインスタンスがまだ組織 ID にマッピングされていない可能性が高くなります。 詳しくは、カスタマーケアにお問い合わせいただき、この設定を完了してください。 接続に成功すると、Campaign コントロールパネルのホームページが表示されます。

コントロールパネルの機能を利用するには、MID／RT インスタンス情報を&#x200B;**[!UICONTROL インスタンス設定]**&#x200B;カードで指定する必要があります。それには、次の手順に従います。

1. **[!UICONTROL インスタンス設定]**&#x200B;カードで、「**[!UICONTROL 外部アカウント]**」タブを選択します。

1. ドロップダウンリストから目的のマーケティングインスタンスを選択して、「**[!UICONTROL 新しい URL を追加]**」をクリックします。

   ![](assets/external-account-addbutton.png)

1. 追加する MID/RT インスタンスに関する情報を提供します。

   ![](assets/external-account-add.png)

   * **[!UICONTROL URL]**:インスタンスの URL。Campaign クライアントコンソールの **[!UICONTROL 管理]** > **[!UICONTROL Platform]** > **[!UICONTROL 外部アカウント]** メニュー

      ![](assets/external-account-url.png)

   * **[!UICONTROL オペレーター]**／**[!UICONTROL パスワード]**：アドビ管理者による初期プロビジョニング後に提供されたオペレーターの資格情報。

      >[!NOTE]
      >
      >これらの詳細が不明な場合は、カスタマーケアにお問い合わせください。

1. 「**[!UICONTROL 保存]**」をクリックして確定します。

MID／RT URL を追加する際は、非同期プロセスがトリガーされて、URL が正確かどうかが検証されます。この処理には数分かかる場合があります。 MID/RT インスタンス URL が検証されるまで、ジョブは保留中になります。 検証が完了した場合にのみ、コントロールパネルの主な機能を利用できます。

![](assets/external-account-pending.png)

リストから選択することで、MID／RT インスタンス URL をいつでも削除または無効化できます。

![](assets/external-account-edit.png)

なお、 **[!UICONTROL 外部アカウント]** MID/RT インスタンス URL の「 」タブを **[!UICONTROL ジョブのログ]**:

![](assets/external-account-logs.png)

## ハイブリッド顧客に使用できる機能 {#capabilities}

MID/RT インスタンスをCampaign コントロールパネルに追加すると、以下に示す機能を利用できます。

* [主要連絡先とイベントの監視](../../service-events/service-events.md)
* [インスタンスの詳細の表示](../../instances-settings/using/instance-details.md)、
* [許可リストへの IP アドレスの追加](../../instances-settings/using/ip-allow-listing-instance-access.md) （RT インスタンスの場合）、
* [デリゲートされたサブドメインに関する情報の表示](../../subdomains-certificates/using/monitoring-subdomains.md)、
* [SSL 証明書に関する情報の表示](../../subdomains-certificates/using/monitoring-ssl-certificates.md)。