---
title: サブドメインの SSL 証明書の監視
description: サブドメインの SSL 証明書の監視方法の詳細
translation-type: tm+mt
source-git-commit: c51a43fb310bbb8bd7570bc4ea668d708159535c

---


# サブドメインの監視 {#monitoring-subdomains}

サブドメインを監視して、Adobe Campaign で機能するようにすべてが正しく設定されていることを確認することが重要です。

各プロダクションインスタンスのサブドメインのリストには、「**[!UICONTROL サブドメインおよび証明書]**」カードを選択すると、直接アクセスできます。

The **[!UICONTROL Last verification]**column indicates when a subdomain was verified for the last time.**...**／**[!UICONTROL &#x200B;サブドメインを検証]**ボタンをクリックすることで、いつでも検証を開始できます。

![](assets/subdomain_verification.png)

>[!CAUTION]
>
>証明書の日付のないサブドメインは、これらのサブドメインに配信品質の問題がある可能性があるので、アドビでは推奨しません。

検証を起動すると、サブドメインが正しく設定されているかどうかを確認するために、いくつかの操作が実行されます（インスタンステナントの確認、電子メール送信テストなど）。

サブドメインの検証に失敗した場合は、アドビカスタマーケアにお問い合わせください。
