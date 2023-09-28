---
product: campaign
solution: Campaign
title: TXT レコードの管理
description: ドメイン所有権検証用の TXT レコードを管理する方法を説明します。
feature: Control Panel
role: Architect
level: Experienced
source-git-commit: 118fa4d722980e507d15647453e96a8b6189f837
workflow-type: tm+mt
source-wordcount: '257'
ht-degree: 25%

---


# TXT レコードの基礎知識 {#managing-txt-records}

>[!CONTEXTUALHELP]
>id="cp_siteverification_add"
>title="TXT レコードの管理"
>abstract="TXT レコードは、ドメインに関するテキスト情報を提供するための一種の DNS レコードで、外部ソースから読み取ることができます。Campaign コントロールパネルを使用すると、Googleサイト検証、DMARC、BIMI の 3 種類のレコードをサブドメインに追加できます。"

## TXT レコードについて {#about}

TXT レコードは、ドメインに関するテキスト情報を提供するための一種の DNS レコードで、外部ソースから読み取ることができます。Campaign コントロールパネルでは、次の 3 種類のレコードをサブドメインに追加できます。

* **Google TXT レコード** を使用すると、ドメインを所有していることをテストでき、E メールの高い受信ボックス率と低いスパム率を確保できます。 [Google TXT レコードを追加する方法を説明します](managing-txt-records.md)
* **DMARC レコード** 送信者のドメインを認証し、悪意のある目的でのドメインの不正使用を防ぐ方法を提供します。 [DMARC レコードを追加する方法を説明します](dmarc.md)
* **BIMI レコード** メールボックスプロバイダーの受信ボックスで、メールの横に承認済みのロゴを表示して、ブランドの認知度と信頼性を高めることができます。 [BIMI レコードを追加する方法を説明します](bimi.md)

## サブドメインのレコードの監視 {#monitor}

サブドメインの詳細にアクセスして、各サブドメインに追加されたすべての TXT レコードを監視できます。

この画面には、選択したサブドメインのすべての TXT タイプのレコードが表示され、設定の「値」列に情報が表示されます。 Google TXT、DMARC または BIMI レコードを削除するには、省略記号ボタンをクリックし、「削除」を選択します。 必要に応じて、DMARC および BIMI レコードを編集することもできます。

![](assets/txt-records.png)
