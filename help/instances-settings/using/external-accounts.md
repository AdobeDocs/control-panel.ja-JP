---
product: campaign
solution: Campaign
title: MID/RT インスタンスの接続
description: MID/RT インスタンスをCampaign コントロールパネルに接続する方法を説明します。
feature: Control Panel
role: Architect
level: Intermediate
source-git-commit: 1b712300bd7a1ef8dc784fa977f938bacc4c5e5b
workflow-type: tm+mt
source-wordcount: '295'
ht-degree: 3%

---


# MID/RT インスタンスの接続

>[!CONTEXTUALHELP]
>id="cp_externalaccounts_url"
>title="サブドメインの詳細"
>abstract="この画面では、ハイブリッドホスティングモデルを使用しているお客様は、Campaign コントロールパネルで特定のアクションを実行するために、マーケティングインスタンスに MID/RT インスタンスを提供できます。"

Campaign コントロールパネルを使用すると、ハイブリッドホスティングモデルのお客様は、マーケティングインスタンスに MID/RT インスタンスを提供することで、Campaign コントロールパネルで特定のアクションを実行できます。 モデルのホスティングについて詳しくは、 [Campaign Classic文書](https://experienceleague.adobe.com/docs/campaign-classic/using/installing-campaign-classic/architecture-and-hosting-models/hosting-models-lp/hosting-models.html).

## MID/RT インスタンスの接続 {#connect}

>[!CONTEXTUALHELP]
>id="cp_externalaccounts_operator"
>title="サブドメインの詳細"
>abstract="マーケティングインスタンスに MID/RT インスタンスを追加するためにクライアントコンソールで使用されるオペレーターの ID。"

>[!CONTEXTUALHELP]
>id="cp_externalaccounts_password"
>title="サブドメインの詳細"
>abstract="マーケティングインスタンスに MID/RT インスタンスを追加するためにクライアントコンソールで使用されるオペレーターのパスワード。"

Campaign コントロールパネルに MID/RT インスタンスを指定するには、次の手順に従います。

1. 内 **[!UICONTROL インスタンス設定]** カードで、 **[!UICONTROL 外部アカウント]** タブをクリックします。

1. ドロップダウンリストからマーケティングインスタンスを選択し、 **[!UICONTROL 新しい URL を追加]**.

   ![](assets/external-account-addbutton.png)

1. 接続する MID/RT インスタンスに関する情報を指定します。
   * **[!UICONTROL URL]**:インスタンスの URL
   * **[!UICONTROL 演算子]** / **[!UICONTROL パスワード]**:マーケティングインスタンスに MID/RT インスタンスを追加するためにクライアントコンソールで使用されるオペレーターの資格情報。

   ![](assets/external-account-add.png)

1. 「**[!UICONTROL 保存]**」をクリックして確定します。

これで、インスタンスがCampaign コントロールパネルに接続されました。 接続は、リストから選択することで、いつでも削除または非アクティブ化できます。

![](assets/external-account-edit.png)

## MID/RT インスタンスで使用できる機能 {#capabilities}

MID/RT インスタンスがCampaign コントロールパネルに接続されると、以下に示す機能を利用して監視できます。

* [インスタンスの詳細を表示](../../instances-settings/using/instance-details.md),
* [インスタンスにアクセスする許可リストに IP アドレスを追加](../../instances-settings/using/ip-allow-listing-instance-access.md),
* [デリゲートされたサブドメインに関する情報の表示](../../subdomains-certificates/using/setting-up-new-subdomain.md),
* [SSL 証明書に関する情報の表示](../../subdomains-certificates/using/monitoring-ssl-certificates.md).
