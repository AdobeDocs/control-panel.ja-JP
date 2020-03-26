---
title: サブドメインの SSL 証明書の監視
description: サブドメインの SSL 証明書の監視方法の詳細
translation-type: tm+mt
source-git-commit: a2c19296894ff893987290cb287dc7002ab999e5

---


# サブドメインの監視 {#monitoring-subdomains}

サブドメインを監視して、Adobe Campaign で機能するようにすべてが正しく設定されていることを確認することが重要です。

The list of subdomains for each of your production instances is accessible directly when selecting the **[!UICONTROL Subdomains & Certificates]** card.

The **[!UICONTROL Last verification]** column indicates when a subdomain was verified for the last time. You can launch a verification at any time by clicking the **...** / **[!UICONTROL Verify subdomain]** button.

![](assets/subdomain_verification.png)

>[!IMPORTANT]
>
>アドビでは、証明日のないサブドメインの使用は、配信品質の問題がある可能性があるので、お勧めしません。

検証を開始すると、サブドメインが正しく設定されていることを確認するために、いくつかの操作が実行されます（インスタンステナントの確認、E メール送信テストなど）。

サブドメインの検証に失敗した場合は、さらに検証するためにアドビカスタマーケアにお問い合わせください。

**関連トピック：**

* [SSL 証明書の追加（チュートリアルビデオ）](https://docs.adobe.com/content/help/en/campaign-learn/campaign-standard-tutorials/administrating/control-panel/adding-ssl-certificates.html)
* [サブドメインの SSL 証明書の更新](../../subdomains-certificates/using/renewing-subdomain-certificate.md)
* [サブドメインのブランディング](../../subdomains-certificates/using/subdomains-branding.md)
