---
title: TXT レコードの管理
description: ドメイン所有権検証用の TXT レコードを管理する方法を説明します。
translation-type: tm+mt
source-git-commit: 5a70141e0198946928723b34c9097c5cf8a24f97

---


# TXT レコードの管理 {#managing-txt-records}

>[!CONTEXTUALHELP]
>id="cp_siteverification_add"
>title="TXT レコードの管理"
>abstract="Googleなどの一部のサービスでは、ドメインの所有者を確認するために、ドメイン設定にTXTレコードを追加する必要があります。"

>[!IMPORTANT]
>
>コントロールパネルからのTXTレコード管理は、4月末までに利用可能になります。

## TXT レコードについて {#about-txt-records}

TXT レコードは、ドメインに関するテキスト情報を提供するために使用される DNS レコードの一種で、外部ソースから読み取ることができます。

高い受信ボックス率および低いスパム率を確保するために、Google などの一部のサービスでは、ドメインを所有していることを検証するために、ドメイン設定に TXT レコードを追加する必要があります。

現在、Gmail は最も人気のある E メールアドレスプロバイダーの 1 つです。Adobe Campaign では、Gmail アドレス宛ての E メールの配信品質を確保して確実な配信をおこなうために、サブドメインに Google サイト検証用の特別な TXT レコードを追加して、サブドメインを確実に検証できます。

その他のリソース：

* [Campaign Standard チュートリアルビデオ](https://docs.adobe.com/content/help/en/campaign-standard-learn/tutorials/administrating/control-panel/google-txt-record-management.html)
* [Campaign Classic チュートリアルビデオ](https://docs.adobe.com/content/help/en/campaign-classic-learn/tutorials/administrating/control-panel-acc/google-txt-record-management.html)

## サブドメイン用の Google TXT レコードの追加 {#adding-a-google-txt-record}

Gmail アドレス宛ての E メール送信に使用するサブドメインに Google TXT レコードを追加するには、次の手順に従います。

1. カードに移動し **[!UICONTROL Subdomain and Certificates]** ます。

1. インスタンスを選択し、DNS レコードを追加するサブドメインの詳細を開きます。

   ![](assets/txt_subdomaindetails.png)

1. Click the **[!UICONTROL Add TXT record]** button, then enter the value generated in G Suite Admin tools. 詳しくは、[G Suite 管理ヘルプ](https://support.google.com/a/answer/183895)を参照してください。

   ![](assets/txt_addtxt.png)

1. Click the **[!UICONTROL Add]** button to confirm.

   ![](assets/txt_txtadded.png)

TXT レコードを追加したら、Google で検証する必要があります。それには、G Suite 管理ツールに移動し、検証手順を実行します（[G Suite 管理ヘルプ](https://support.google.com/a/answer/183895)を参照）。

レコードを削除するには、レコードリストからレコードを選択し、「削除」ボタンをクリックします。

>[!NOTE]
>
>DNS レコードリストから削除できるのは、以前に追加したレコードのみです（この例では Google TXT レコード）。


