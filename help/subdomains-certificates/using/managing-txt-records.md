---
title: TXT レコードの管理
description: ドメイン所有権検証用の TXT レコードを管理する方法を説明します。
translation-type: ht
source-git-commit: 3ce9f62be9df0f6e6a61c16ddaf3ab8ae58712ce

---


# TXT レコードの管理 {#managing-txt-records}

>[!CONTEXTUALHELP]
>id="cp_siteverification_add"
>title="[!CONTEXTUALHELP]
>id=&quot;cp_siteverification_add&quot;
>title=&quot;TXT レコードの管理&quot;
>abstract=&quot;Google などの一部のサービスでは、ドメインを所有していることを検証するために、ドメイン設定に TXT レコードを追加する必要があります。&quot;"
>abstract="TXT レコードについて {#about-txt-records}"

## TXT レコードは、ドメインに関するテキスト情報を提供するために使用される DNS レコードの一種で、外部ソースから読み取ることができます。{#about-txt-records}

高い受信ボックス率および低いスパム率を確保するために、Google などの一部のサービスでは、ドメインを所有していることを検証するために、ドメイン設定に TXT レコードを追加する必要があります。

現在、Gmail は最も人気のある E メールアドレスプロバイダーの 1 つです。Adobe Campaign では、Gmail アドレス宛ての E メールの配信品質を確保して確実な配信をおこなうために、サブドメインに Google サイト検証用の特別な TXT レコードを追加して、サブドメインを確実に検証できます。

サブドメイン用の Google TXT レコードの追加 {#adding-a-google-txt-record}

## Gmail アドレス宛ての E メール送信に使用するサブドメインに Google TXT レコードを追加するには、次の手順に従います。{#adding-a-google-txt-record}

「**[!UICONTROL サブドメインおよび証明書]**」カードに移動します。

1. インスタンスを選択し、DNS レコードを追加するサブドメインの詳細を開きます。****

1. ![](assets/txt_subdomaindetails.png)

   「**[!UICONTROL TXT レコードを追加]**」ボタンをクリックし、G Suite 管理ツールで生成した値を入力します。詳しくは、[G Suite 管理ヘルプ[#$tu15]を参照してください。

1. 

   「**[!UICONTROL 追加]**」ボタンをクリックして、確定します。

1. ![](assets/txt_txtadded.png)]**

   TXT レコードを追加したら、Google で検証する必要があります。それには、G Suite 管理ツールに移動し、検証手順を実行します（[G Suite 管理ヘルプ[#$tu20]を参照）。




[!NOTE]

>[!NOTE]DNS レコードリストから削除できるのは、以前に追加したレコードのみです（この例では Google TXT レコード）。
>
>The only record that you can delete from the DNS records list is the one that you have previously added (in our case the Google TXT record).
