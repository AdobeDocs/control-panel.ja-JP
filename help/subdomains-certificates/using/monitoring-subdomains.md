---
title: サブドメインのSSL証明書の監視
description: サブドメインのSSL証明書を監視する方法について説明します
translation-type: tm+mt
source-git-commit: 52f155bbbecec9edabc66cbc28756f9579b81f04

---


# サブドメインの監視 {#monitoring-subdomains}

サブドメインを監視して、Adobe Campaignで動作するようにすべてが正しく設定されていることを確認する必要があります。

The list of subdomains for each of your production instances is accessible directly when selecting the **[!UICONTROL Subdomains &amp; Certificates]**card.

![](assets/subdomains_list.png)

サブドメインリストの「最後の検証 ****」列には、サブドメインが最後に検証された日時が示されます。** 検証は、次をクリックするといつでも開始で **きます。/サブド**[!UICONTROL &#x200B;メインを検証]** ボタン。

![](assets/subdomain_verification.png)

>[!CAUTION]
>
>検証日のないサブドメインは、配信品質の問題がある可能性があるので、アドビでは推奨しません。

検証を起動すると、サブドメインが正しく設定されているかどうかを確認するために、いくつかの操作が実行されます（インスタンステナントの確認、電子メール送信テストなど）。

サブドメインの検証に失敗した場合は、アドビカスタマーケアにお問い合わせください。
