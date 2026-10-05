---
product: campaign
solution: Campaign
title: アドビへのサブドメインの SSL 証明書のデリゲート
description: アドビへのサブドメインの SSL 証明書のデリゲート方法を学ぶ
feature: Control Panel, Subdomains and Certificates
role: Admin
level: Experienced
exl-id: a2b3d409-704b-4e81-ae40-b734f755b598
TQID: 'https://experienceleague.adobe.com/rkz8m-EBdNJEiimWc3YVlgsXSHYR9aA4R6y6cnZqRiw'
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: a075b2c1-7748-4328-b7f6-343aa314616a
    internal-label: Campaigns
  - id: ae9127b0-c11d-467b-903d-a84cef43f6ed
    internal-label: Control Panel
  - id: a7760dfc-5c44-4d77-bb68-c50b1e265c93
    internal-label: Security and privacy
subfeature_v2:
  - id: f807e46f-d823-43a9-98be-82e0b2f3a05c
    internal-label: Subdomains and certificates
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
source-git-commit: b2723b0683a305a992b710a37a3e47927e1fb65e
workflow-type: tm+mt
source-wordcount: '485'
ht-degree: 100%
---
# アドビへのサブドメインの SSL 証明書のデリゲート {#delegate-ssl-certificates}

>[!CONTEXTUALHELP]
>id="cp_managed_ssl"
>title="アドビへのサブドメインの SSL 証明書のデリゲート"
>abstract="コントロールパネルでは、サブドメインの SSL 証明書をアドビで管理できます。 CNAME を使用してサブドメインを設定している場合、ドメインホスティングソリューションに証明書を生成するために、証明書レコードが自動的に生成および提供されます。"

アドビで証明書を自動的に作成し、証明書の有効期限が切れる前に毎年更新するので、アドビへのサブドメインの SSL 証明書の管理のデリゲートを強くお勧めします。

CNAME を使用してサブドメインデリゲーションを設定している場合、アドビでは、証明書を生成するためにドメインホスティングソリューションに使用する証明書レコードを提供します。

アドビへの SSL 証明書のデリゲーションは、新しいサブドメインを設定する際や、既にデリゲートされたサブドメインに対して実行できます。

>[!NOTE]
>
>アドビ管理の SSL は、ユーザーが無料で使用できる機能です。 アドビへのサブドメインの証明書のデリゲートは透過的であり、キャンペーンや配信品質に影響はありません。 [詳しくは、SSL 証明書の管理を参照してください](monitoring-ssl-certificates.md#management)


## 新しいサブドメインの SSL 証明書のデリゲート {#new}

新しいサブドメインを設定する際に SSL 証明書をデリゲートするには、サブドメイン設定ウィザードの「**[!UICONTROL サブドメインのアドビ管理の SSL を選択]**」オプションを有効にします。 証明書の生成プロセスは、サブドメインのデリゲーション方法によって異なります。

* **完全なサブドメインのデリゲーション**：SSL 証明書は、ユーザーからのアクションを必要とせずに、アドビにより自動的にリクエストおよびインストールされます。 サブドメインの設定を送信すると、サブドメイン設定ワークフローの一部として証明書のインストールリクエストがすぐに処理されます。 [完全なサブドメインのデリゲーションの詳細情報](setting-up-new-subdomain.md#full-subdomain-delegation)

* **CNAME のデリゲーション**：ホスティングソリューションにコピーする証明書レコードは、後の設定ウィザードで提供されます。 サブドメインの設定を送信する前に、ドメインホスティングソリューションでこれらの証明書レコードを生成する必要があります。 [CNAME のデリゲーションの詳細情報](setting-up-new-subdomain.md#use-cnames)

![](assets/cname-adobe-managed.png){width="70%"}

## 既にデリゲートされたサブドメインに対する SSL 証明書のデリゲート {#delegated}

既にデリゲートされたサブドメインに対して SSL 証明書をデリゲートするには、目的のサブドメインの横にある省略記号ボタンをクリックし、「**[!UICONTROL 管理 SSL に切り替え]**」をクリックします。

![](assets/delegate-ssl-list.png){width="70%"}

証明書の生成プロセスは、サブドメインが最初にどのように設定されたかによって異なります。

### 完全にデリゲートされたサブドメイン

完全なサブドメインのデリゲーション（Adobe ネームサーバーを使用）を使用して設定されたサブドメインの場合、SSL 証明書はアドビにより自動的にリクエストおよびインストールされます。 「**[!UICONTROL 管理 SSL に切り替え]**」をクリックして確認すると、ユーザーからの追加のアクションを必要とせずに、証明書のインストールリクエストがすぐに送信されます。

### CNAME のデリゲートされたサブドメイン

CNAME のデリゲーションを使用して設定されたサブドメインの場合、アドビにより自動的に生成された証明書レコードを含むダイアログボックスが表示されます。 これらのレコードを 1 つずつコピーするか、CSV ファイルをダウンロードしてから、ドメインホスティングソリューションに移動して、一致する証明書を生成します。

すべての証明書レコードがドメインホスティングソリューションに生成されていることを確認します。 すべてが正しく設定されている場合は、レコードの作成を確認し、「**[!UICONTROL 送信]**」をクリックします。

![](assets/delegate-ssl.png){width="70%"}
