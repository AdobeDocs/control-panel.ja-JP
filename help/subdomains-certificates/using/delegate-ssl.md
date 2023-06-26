---
product: campaign
solution: Campaign
title: アドビへのサブドメインの SSL 証明書のデリゲート
description: サブドメインの SSL 証明書をAdobeにデリゲートする方法を説明します
feature: Control Panel
role: Architect
level: Experienced
source-git-commit: 0eefdbde25c955c84ee7534976256ca4df9a686c
workflow-type: tm+mt
source-wordcount: '309'
ht-degree: 45%

---

# アドビへのサブドメインの SSL 証明書のデリゲート {#delegate-ssl-certificates}

>[!CONTEXTUALHELP]
>id="cp_managed_ssl"
>title="アドビへのサブドメインの SSL 証明書のデリゲート"
>abstract="コントロールパネルでは、サブドメインの SSL 証明書をアドビで管理できます。CNAME を使用してサブドメインを設定している場合、ドメインホスティングソリューションに証明書を生成するために、証明書レコードが自動的に生成および提供されます。"

Adobeは証明書を自動的に作成し、証明書の期限が切れる前に毎年更新するので、サブドメインの SSL 証明書をAdobeにデリゲートすることを強くお勧めします。

CNAME を使用してサブドメインデリゲーションを設定している場合、アドビでは、証明書を生成するためにドメインホスティングソリューションに使用する証明書レコードを提供します。

SSL 証明書のAdobeへのデリゲーションは、新しいサブドメインを設定する際、または既にデリゲートされたサブドメインに対して実行できます。

>[!NOTE]
>
>アドビ管理の SSL は、ユーザーが無料で使用できる機能です。

## 新しいサブドメインの SSL 証明書をデリゲート {#new}

新しいサブドメインの設定時に SSL 証明書をデリゲートするには、 **[!UICONTROL サブドメインのAdobe管理 SSL のオプト]** オプションを使用します。 ホスティングソリューションにコピーする証明書レコードは、後で設定ウィザードで提供されます。 詳細な手順については、 [この節](setting-up-new-subdomain.md).

![](assets/cname-adobe-managed.png){width="70%" align="left"}

## 既にデリゲートされたサブドメインに対して SSL 証明書をデリゲート {#delegated}

既にデリゲートされたサブドメインに対して SSL 証明書をデリゲートするには、目的のサブドメインの横にある省略記号ボタンをクリックし、 **[!UICONTROL 管理 SSL に切り替え]**.

![](assets/delegate-ssl-list.png){width="70%" align="left"}

[Adobe] で自動的に生成された証明書レコードがダイアログボックスに表示されます。 これらのレコードを 1 つずつコピーするか、CSV ファイルをダウンロードしてから、ドメインホスティングソリューションに移動して、一致する証明書を生成します。

すべての証明書レコードがドメインホスティングソリューションに生成されていることを確認します。すべてが正しく設定されている場合は、レコードの作成を確認し、「 **[!UICONTROL 送信]**.

![](assets/delegate-ssl.png){width="70%" align="left"}
