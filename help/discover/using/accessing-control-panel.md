---
product: campaign
solution: Campaign
title: コントロールパネルへのアクセス
description: コントロールパネルへのアクセス方法の詳細
feature: Control Panel, Access Management
role: Admin
level: Experienced
exl-id: eb67af6e-a64e-49a7-9656-782f91bc1d67
TQID: https://experienceleague.adobe.com/Ug0vHjgyTK-BRO4IMdCwSQuiwO--XagzjW-MFTPcZrY
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 57345245341bf2d04b9b01611d502532ba8f175b
workflow-type: tm+mt
source-wordcount: 353
ht-degree: 83%

---

# コントロールパネルへのアクセス {#accessing-control-panel}

コントロールパネルには、Experience Cloud から直接アクセスすることも、製品自体からアクセスすることもできます。

## 前提条件 {#prerequisites}

Campaign v7／v8 の場合は、インスタンスを Amazon Web Services（AWS）でホストし、最新の [Campaign 安定ビルド](https://experienceleague.adobe.com/docs/campaign-classic/using/release-notes/rn-overview.html?lang=ja#rn-statuses)またはビルド 9032 以降にアップグレードする必要があります。 バージョンを確認する方法については、[この節](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/starting-with-adobe-campaign/launching-adobe-campaign.html?lang=ja#getting-your-campaign-version)を参照してください。 インスタンスが AWS でホストされているかどうかを確認するには、[このページ](../../faq.md#hosted-aws)で詳しく説明されている手順に従ってください。

Microsoft AzureでホストされているCampaign v8 インスタンスは、Campaign コントロールパネル機能のサブセットにもアクセスできます。[&#x200B; インスタンスアクセスのIP許可リスト &#x200B;](../../instances-settings/using/ip-allow-listing-instance-access.md)、[SFTP サーバーのIP許可リスト &#x200B;](../../sftp/using/ip-range-allow-listing.md)、[&#x200B; カスタマー管理のSSL証明書管理](../../subdomains-certificates/using/renewing-subdomain-certificate.md)。

>[!IMPORTANT]
>
>デフォルトでは、コントロールパネルは、「Administrators」製品プロファイルに属する管理者ユーザーがアクセスできます。 組織の設定に応じて、製品プロファイルに異なる名前を付けることができます（「admin」、「admins」、「approval admin」など）。 **名前に「admin」という単語が含まれている製品プロファイルは、Campaign コントロールパネル**&#x200B;へのアクセス権を自動的に付与します。 製品プロファイルの命名を慎重に確認し、認証されたユーザーのみがコントロールパネルにアクセスできるようにします。 [Campaign コントロールパネルに対する権限を管理する方法について説明します](../../discover/using/managing-permissions.md)。

## Experience Cloud Platform からのアクセス {#access-experience-cloud-platform}

Adobe Experience Cloud Platform からコントロールパネルにアクセスするには、次の手順に従います。

1. [Experience Cloud ホームページ](https://experiencecloud.adobe.com/){target="_blank"}に移動します。

1. 「**クイックアクセス**」セクションの専用リンクをクリックします。

   ![](assets/do-not-localize/quickaccess.png)

コントロールパネルには、Experience Cloud Platform の&#x200B;**ソリューションピッカー**&#x200B;からもアクセスできます。

1. [Adobe Experience Cloud ホームページ](https://experiencecloud.adobe.com/){target="_blank"}で、「**クイックアクセス**」セクションまたは右側の上部メニューから「**Campaign**」を選択します。

   ![](assets/do-not-localize/control_panel_access1.png)

1. Campaign インスタンスのリストが表示されます。 **コントロールパネル**&#x200B;カードをクリックして起動します。

   ![](assets/do-not-localize/control_panel_access2.png)

## 製品からのアクセス {#access-product}

>[!NOTE]
>
>製品内からのアクセスは、[Campaign Standard](https://experienceleague.adobe.com/docs/campaign-standard/using/campaign-standard-home.html?lang=ja){target="_blank"} でのみ可能です。

1. Campaign Standard 製品を起動します。

1. **ナビゲーション**&#x200B;ペインから&#x200B;**[!UICONTROL 管理]**&#x200B;メニューを選択します。

   ![](assets/control_panel_access3.png)

1. 「**[!UICONTROL コントロールパネル]**」アイコンをクリックします。

   ![](assets/control_panel_access4.png)
