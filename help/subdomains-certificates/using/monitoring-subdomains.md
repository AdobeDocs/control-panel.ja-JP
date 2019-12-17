---
title: サブドメインのSSL証明書の監視
description: サブドメインのSSL証明書を監視する方法について説明します
translation-type: tm+mt
source-git-commit: 85bef8fa652be883bc2afbc42a2d893ea75a4e77

---


# サブドメインの監視 {#monitoring-subdomains}

サブドメインを監視して、Adobe Campaignで動作するようにすべてが正しく設定されていることを確認する必要があります。

The list of subdomains for each of your production instances is accessible directly when selecting the **[!UICONTROL Subdomains &amp; Certificates]**card.

![](assets/subdomains_list.png)

To get more details on a subdomain, click the **[!UICONTROL Subdomain Details]**button.
すべての関連サブドメインのリストが表示されます。 通常、ランディングページやリソースページなどのサブドメインが含まれます。

「送信 **[!UICONTROL 者情報]**」タブには、設定済みのinbox（送信者、返信、エラー電子メール）に関する情報が表示されます。

![](assets/subdomain_details.png)


サブドメインリストの「最後の検証 ****」列には、サブドメインが最後に検証された日時が示されます。** 検証は、次をクリックするといつでも開始で **きます。/サブド**[!UICONTROL &#x200B;メインを検証]** ボタン。

>[!CAUTION]
>
>検証日のないサブドメインは、配信品質の問題がある可能性があるので、アドビでは推奨しません。

![](assets/subdomain_verification.png)

検証を起動すると、サブドメインが正しく設定されていることを確認するために、いくつかの操作が実行されます。

1. コントロールパネルで、サブドメインがインスタンステナントに属しているかどうかを確認します。
1. そのサブドメインを使用してインスタンスから、「250ok」（サードパーティの電子メール分析および配信品質プラットフォーム）のテスト受信者のセットに電子メールが送信されます。
1. 電子メールを受け取った後、250okは電子メールヘッダを読み取り、SPFとDKIMが設定され、有効であるかどうかを確認します。
1. コントロールパネルでは、250 OKから約20分間、配信状態のポーリングを継続して行います。 SPFとDKIMが渡される場合は、要求されたサブドメインが検証済みで、電子メールの送信に使用する準備が完全に整っていることを意味します。
