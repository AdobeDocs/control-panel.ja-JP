---
title: サブドメインの SSL 証明書の監視
description: サブドメインの SSL 証明書の監視方法の詳細
translation-type: tm+mt
source-git-commit: 762c445713e6e728fc1a45d5fcf8c9c1cb0dcdf6

---


# サブドメインの監視 {#monitoring-subdomains}

サブドメインを監視して、Adobe Campaign で機能するようにすべてが正しく設定されていることを確認することが重要です。

各プロダクションインスタンスのサブドメインのリストには、「**[!UICONTROL サブドメインおよび証明書]**」カードを選択すると、直接アクセスできます。

「**[!UICONTROL 前回の検証日]**」列には、サブドメインが最後に検証された日が示されます。**...**／**[!UICONTROL &#x200B;サブドメインを検証]**ボタンをクリックすることで、いつでも検証を開始できます。

![](assets/subdomain_verification.png)

>[!CAUTION]
>
>アドビでは、証明日のないサブドメインの使用は、配信品質の問題がある可能性があるので、お勧めしません。

検証を開始すると、サブドメインが正しく設定されていることを確認するために、いくつかの操作が実行されます（インスタンステナントの確認、E メール送信テストなど）。

サブドメインの検証に失敗した場合は、さらに検証するためにアドビカスタマーケアにお問い合わせください。

**関連トピック：**

* [SSL証明書の追加（チュートリアルビデオ）](https://docs.adobe.com/content/help/en/campaign-learn/campaign-standard-tutorials/administrating/control-panel/adding-ssl-certificates.html)
* [サブドメインの SSL 証明書の更新](../..help/subdomains-certificates/using/renewing-subdomain-certificate.md)
* [サブドメインのブランド化](../../subdomains-certificates/using/subdomains-branding.md)
