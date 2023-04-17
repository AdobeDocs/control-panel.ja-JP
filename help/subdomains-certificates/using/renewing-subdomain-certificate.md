---
product: campaign
solution: Campaign
title: サブドメインの SSL 証明書の更新
description: サブドメインの SSL 証明書の更新方法の詳細
feature: Control Panel
role: Architect
level: Experienced
exl-id: e9b7c67d-6afa-44f9-b19d-39c0ec9a7edd
source-git-commit: 963c2af5cdca80ebc2cd79e0708dc4dfe8c6ec1e
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# SSL 証明書の更新 {#renewing-subdomains-ssl-certificates}

>[!CONTEXTUALHELP]
>id="cp_add_ssl_certificate"
>title="SSL 証明書の更新"
>abstract="SSL 証明書を更新するには、CSR を生成し、サブドメインの SSL 証明書を購入して、証明書バンドルをインストールする必要があります。"
>additional-url="https://experienceleague.adobe.com/docs/control-panel/using/subdomains-and-certificates/renewing-subdomain-certificate.html?lang=ja#generating-csr" text="証明書署名リクエスト（CSR）の生成"
>additional-url="https://experienceleague.adobe.com/docs/control-panel/using/subdomains-and-certificates/renewing-subdomain-certificate.html?lang=ja#installing-ssl-certificate" text="SSL 証明書のインストール"

SSL 証明書の更新プロセスは、次の 3 ステップで構成されます。

1. **証明書署名要求（CSR）の生成**

   証明書署名要求は、証明書を購入する前に、保護する予定のインスタンスおよびサブドメイン用に生成する必要があります。CSR の生成に必要な情報（共通名、組織名、住所など）を提供する必要があります。[詳細情報](generate-csr.md)

1. **SSL 証明書の購入**

   CSR が生成されたら、それを使用して、会社が承認した認証局から SSL 証明書を購入できます。

1. **SSL 証明書のインストール**

   購入した SSL 証明書を目的のサブドメインにインストールして、サブドメインを保護します。 [詳細情報](install-ssl-certificate.md)

![](assets/do-not-localize/how-to-video.png) この機能をビデオで確認（[Campaign v7／v8](https://experienceleague.adobe.com/docs/campaign-classic-learn/control-panel/subdomains-and-certificates/adding-ssl-certificates.html?lang=ja#subdomains-and-certificates) または [Campaign Standard](https://experienceleague.adobe.com/docs/campaign-standard-learn/control-panel/subdomains-and-certificates/adding-ssl-certificates.html?lang=ja#adding-ssl-certificates) を使用）

**関連トピック：**

* [配信品質のベストプラクティスガイド - Adobe Campaign の SSL 証明書リクエストプロセス](https://experienceleague.adobe.com/docs/deliverability-learn/deliverability-best-practice-guide/additional-resources/campaign/ac-ssl-certificate-request.html?lang=ja)
* [サブドメインのブランディング](../../subdomains-certificates/using/subdomains-branding.md)
* [サブドメインの監視](../../subdomains-certificates/using/monitoring-subdomains.md)
