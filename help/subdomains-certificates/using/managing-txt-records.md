---
product: campaign
solution: Campaign
title: サブドメインの Google サイト検証レコードの追加
description: ドメイン所有権の検証用に、サブドメインの Google サイト検証レコードを追加する方法を説明します。
feature: Control Panel, Subdomains and Certificates
role: Admin
level: Experienced
exl-id: 547ca6f2-720f-4d58-b31b-5b2611ba9156
TQID: 'https://experienceleague.adobe.com/TtF1W0tOklUuEpihvsYlxdszEujRrDXv-Ar0y3c7QX8'
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
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
source-wordcount: '323'
ht-degree: 100%
---
# Google サイト検証レコードを追加 {#adding-a-google-txt-record}

高い受信ボックス率および低いスパム率を確保するために、Google などの一部のサービスでは、ドメインを所有していることを検証するために、ドメイン設定に TXT レコードを追加する必要があります。

現在、Gmail は最も人気のあるメールアドレスプロバイダーの 1 つです。 Adobe Campaign では、Gmail アドレス宛てのメールの配信品質を確保して確実な配信をおこなうために、サブドメインに Google サイト検証用の特別な TXT レコードを追加して、サブドメインを確実に検証できます。

Gmail アドレス宛てのメール送信に使用するサブドメインに Google TXT レコードを追加するには、次の手順に従います。

1. サブドメインリストで、目的のサブドメインの横にある省略記号ボタンをクリックし、「**[!UICONTROL サブドメインの詳細]**」を選択します。

1. 「**[!UICONTROL TXT レコードを追加]**」ボタンをクリックし、「**[!UICONTROL レコードタイプ]**」ドロップダウンリストから「**[!UICONTROL Google サイト検証]**」を選択します。

1. G Suite 管理ツールで生成された値を入力します。 詳しくは、[G Suite 管理ヘルプ](https://support.google.com/a/answer/183895)を参照してください。

   ![](assets/txt_addtxt.png)

1. 「**[!UICONTROL 追加]**」ボタンをクリックして、確定します。

   ![](assets/txt_txtadded.png)

TXT レコードを追加したら、Google で検証する必要があります。 それには、G Suite 管理ツールに移動し、検証手順を実行します（[G Suite 管理ヘルプ](https://support.google.com/a/answer/183895)を参照）。

レコードを削除するには、レコードリストからレコードを選択し、「削除」ボタンをクリックします。

>[!NOTE]
>
>DNS レコードリストから削除できるのは、以前に追加したレコードのみです（この例では Google TXT レコード）。

![](assets/do-not-localize/how-to-video.png) この機能をビデオで確認（[Campaign v7／v8](https://experienceleague.adobe.com/docs/campaign-classic-learn/control-panel/subdomains-and-certificates/google-txt-record-management.html?lang=ja#subdomains-and-certificates) または [Campaign Standard](https://experienceleague.adobe.com/docs/campaign-standard-learn/control-panel/subdomains-and-certificates/google-txt-record-management.html?lang=ja#subdomains-and-certificates) を使用）
