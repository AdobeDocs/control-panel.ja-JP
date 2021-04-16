---
product: campaign
solution: Campaign
title: サブドメインの SSL 証明書の監視
description: サブドメインの SSL 証明書の監視方法の詳細
feature: Campaign コントロールパネル
role: Architect
level: Experienced
exl-id: edd55d07-bf0b-44b0-8281-be69c698d5e8
translation-type: ht
source-git-commit: 4fc34b07b497c743e2ca6c182e68d6ea5c180ac9
workflow-type: ht
source-wordcount: '150'
ht-degree: 100%

---

# サブドメインの監視 {#monitoring-subdomains}

サブドメインを監視して、Adobe Campaign で機能するようにすべてが正しく設定されていることを確認することが重要です。

各プロダクションインスタンスのサブドメインのリストには、「**[!UICONTROL サブドメインおよび証明書]**」カードを選択すると、直接アクセスできます。

「**[!UICONTROL 前回の検証日]**」列には、サブドメインが最後に検証された日が示されます。**...**／**[!UICONTROL サブドメインを検証]**&#x200B;ボタンをクリックすることで、いつでも検証を開始できます。

![](assets/subdomain_verification.png)

>[!IMPORTANT]
>
>アドビでは、証明日のないサブドメインの使用は、配信品質の問題がある可能性があるので、お勧めしません。

検証を開始すると、サブドメインが正しく設定されていることを確認するために、いくつかの操作が実行されます（インスタンステナントの確認、E メール送信テストなど）。

サブドメインの検証に失敗した場合は、さらに検証するためにアドビカスタマーケアにお問い合わせください。

**関連トピック：**

* [サブドメインの SSL 証明書の更新](../../subdomains-certificates/using/renewing-subdomain-certificate.md)
* [サブドメインのブランディング](../../subdomains-certificates/using/subdomains-branding.md)
