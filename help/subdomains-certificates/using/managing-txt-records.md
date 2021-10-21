---
product: campaign
solution: Campaign
title: TXT レコードの管理
description: ドメイン所有権検証用の TXT レコードを管理する方法を説明します。
feature: Control Panel
role: Architect
level: Experienced
exl-id: 547ca6f2-720f-4d58-b31b-5b2611ba9156
source-git-commit: 8dce5b9d1eb59b7ebc8ef1f73f7552dcf61077a1
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 95%

---

# TXT レコードの管理 {#managing-txt-records}

>[!CONTEXTUALHELP]
>id="cp_siteverification_add"
>title="TXT レコードの管理"
>abstract="Google などの一部のサービスでは、ドメインを所有していることを検証するために、ドメイン設定に TXT レコードを追加する必要があります。"
>additional-url="https://experienceleague.adobe.com/docs/control-panel/using/subdomains-and-certificates/setting-up-new-subdomain.html?lang=ja" text="新しいサブドメインのセットアップ"

## TXT レコードについて {#about-txt-records}

>[!AVAILABILITY]
>
>この機能は、Campaign v8 では使用できません。

TXT レコードは、ドメインに関するテキスト情報を提供するために使用される DNS レコードの一種で、外部ソースから読み取ることができます。

高い受信ボックス率および低いスパム率を確保するために、Google などの一部のサービスでは、ドメインを所有していることを検証するために、ドメイン設定に TXT レコードを追加する必要があります。

現在、Gmail は最も人気のある E メールアドレスプロバイダーの 1 つです。Adobe Campaign では、Gmail アドレス宛ての E メールの配信品質を確保して確実な配信をおこなうために、サブドメインに Google サイト検証用の特別な TXT レコードを追加して、サブドメインを確実に検証できます。

この機能を ![](assets/do-not-localize/how-to-video.png) [Campaign Classic](https://experienceleague.adobe.com/docs/campaign-classic-learn/control-panel/subdomains-and-certificates/google-txt-record-management.html#subdomains-and-certificates) 使用時または [Campaign Standard](https://experienceleague.adobe.com/docs/campaign-standard-learn/control-panel/subdomains-and-certificates/google-txt-record-management.html#subdomains-and-certificates) 使用時のビデオで確認

## サブドメイン用の Google TXT レコードの追加 {#adding-a-google-txt-record}

Gmail アドレス宛ての E メール送信に使用するサブドメインに Google TXT レコードを追加するには、次の手順に従います。

1. 「**[!UICONTROL サブドメインおよび証明書]**」カードに移動します。

1. インスタンスを選択し、DNS レコードを追加するサブドメインの詳細を開きます。

   ![](assets/txt_subdomaindetails.png)

1. 「**[!UICONTROL TXT レコードを追加]**」ボタンをクリックし、G Suite 管理ツールで生成した値を入力します。詳しくは、[G Suite 管理ヘルプ](https://support.google.com/a/answer/183895)を参照してください。

   ![](assets/txt_addtxt.png)

1. 「**[!UICONTROL 追加]**」ボタンをクリックして、確定します。

   ![](assets/txt_txtadded.png)

TXT レコードを追加したら、Google で検証する必要があります。それには、G Suite 管理ツールに移動し、検証手順を実行します（[G Suite 管理ヘルプ](https://support.google.com/a/answer/183895)を参照）。

レコードを削除するには、レコードリストからレコードを選択し、「削除」ボタンをクリックします。

>[!NOTE]
>
>DNS レコードリストから削除できるのは、以前に追加したレコードのみです（この例では Google TXT レコード）。
