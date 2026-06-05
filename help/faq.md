---
product: campaign
solution: Campaign
title: コントロールパネルのよくある質問
description: コントロールパネルに関するよくある質問
feature: Control Panel
role: Admin
level: Intermediate
exl-id: 4f329764-ed8b-4939-affc-ed994fd6101d
TQID: https://experienceleague.adobe.com/QzCaKeB3zqjFQTyDXRI5JQ2YoM98F5pZxOoMK1J9bjE
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
feature_v2:
  - id: c5474392-5419-4296-9e41-f6f4ce4f6e9b
subfeature_v2:
  - id: e3988c18-3cfa-4f16-b812-ac2d2b1056fa
  - id: e739ee2b-6228-412e-878f-45de0791417d
  - id: eff19c99-440a-4318-b319-444edc4d8d8f
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
level_v2:
  - id: b5a62a22-46f7-4f0d-b151-3fc640bef588
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 57345245341bf2d04b9b01611d502532ba8f175b
workflow-type: ht
source-wordcount: 801
ht-degree: 100%

---

# よくある質問 {#faq}

## コントロールパネル {#control-panel}

### コントロールパネルとは？

コントロールパネルは、製品の管理者が様々な設定を直接管理し、Adobe Campaign に接続された SFTP サーバーの容量を監視できるようにするものです。

### コントロールパネルには現在どのような機能がありますか？

コントロールパネルでは、ニーズやその他のアクションに基づいて、SFTP サーバーに対し、ストレージの追跡、IP の許可リストへの登録、SSH 鍵の管理を自身で行うことができます。

詳しくは、コントロールパネルでサポートされる操作のドキュメントを参照してください。

### Campaign Classic v7 で利用できる機能で、Campaign v8 ではまだサポートされていないものはありますか？{#v8-restrictions}

いいえ。 Campaign v7 で使用可能なすべての機能は、サブドメインや証明書管理関連の機能を含め、Campaign v8 のコントロールパネルでもサポートされるようになりました。

### コントロールパネルは Adobe Campaign 専用ですか？

はい、コントロールパネルで管理できるのは Adobe Campaign の設定のみです。

### 誰がコントロールパネルを使用できますか？

コントロールパネルを使用できるのは、Adobe Campaign を AWS でホストしている顧客の製品管理者です。また、Microsoft Azure でホストされる Campaign v8 インスタンスは、コントロールパネル機能のサブセット（インスタンス アクセス用の IP 許可リストへの登録、SFTP サーバー用の IP 許可リストへの登録、お客様が管理する SSL 証明書の管理）にもアクセスできます。

コントロールパネルでは、ハイブリッドホスティングモデルを使用するお客様は、特定のコントロールパネル機能を利用できます。 これを行うには、コントロールパネルでマーケティングインスタンスに設定した MID／RT インスタンス URL を指定する必要があります。 [詳細情報](instances-settings/using/external-accounts.md)

管理者でないユーザーがアクセスを希望する場合は、製品の管理者に問い合わせて、管理者として追加してもらう必要があります。

### Campaign Classic v7 ユーザーの場合、コントロールパネルにアクセスする条件は何ですか？ {#v7-restrictions}

コントロールパネルは、管理者ユーザーに限定されています。 [詳細情報](discover/using/managing-permissions.md)。

Campaign v7 の場合は、インスタンスを Amazon Web Services（AWS）でホストし、最新の [Campaign 安定ビルド](https://experienceleague.adobe.com/docs/campaign-classic/using/release-notes/rn-overview.html?lang=ja#rn-statuses)またはビルド 9032 以降にアップグレードする必要があります。 Campaign Classic v7 のバージョンを確認する方法を、[この節](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/starting-with-adobe-campaign/launching-adobe-campaign.html?lang=ja#getting-your-campaign-version)で学習します。 Campaign Classic のインスタンスが AWS でホストされているかどうかを確認するには、[この節](#hosted-aws)で説明している手順に従ってください。

### コントロールパネルにアクセスする方法は？

コントロールパネルへのアクセスのドキュメントに記載されている指示に従ってください。

### コントロールパネルの使用に追加料金はかかりますか？

いいえ、Adobe Campaign の現在のお客様であれば、追加費用はかかりません。

## 組織 ID {#ims-org-id}

### 組織 ID とは何ですか？

これは、初めて Adobe Experience Cloud にログインする際にインスタンスに割り当てられる一意の ID です。 形式は xxx@AdobeOrg です。

詳しくは、[Adobe Experience Cloud のドキュメント](https://experienceleague.adobe.com/docs/core-services/interface/administration/organizations.html?lang=ja)を参照してください。

### 組織 ID はどこにありますか？

ID を見つける方法の 1 つとして、[Adobe Experience Cloud のホーム](https://experiencecloud.adobe.com/)／**[!UICONTROL 管理]**&#x200B;に移動します。 組織 ID は、「**[!UICONTROL 管理クイックアクセス]**」セクションの下部にあります。 詳しくは、[Adobe Experience Cloud のドキュメント](https://experienceleague.adobe.com/docs/core-services/interface/administration/organizations.html?lang=ja)を参照してください。

もう 1 つの方法は、**Admin Console** を起動することです。 組織 ID は、URL 内に、「https://adminconsole.adobe.com/xxx@AdobeOrg/overview」のような形式で表示されます。

### 組織 ID を知る必要があるのはなぜですか？

自分のインスタンスの設定を管理するためです。会社で複数のインスタンスを使用している場合、適切なインスタンスに対する適切な情報を取得する必要があります。

### 複数の組織 ID がある場合はどうすればよいですか？

Analytics と Campaign の間で 1 つの組織 ID を使用することは、買い物かごの放棄などの複雑なユースケースを活用できるようソリューションを統合する予定がある場合の要件です（Adobe Analytics + Adobe Campaign の場合）。 複数のアドビソリューションへのアクセス権がある場合、2 つ以上の組織 ID がある可能性があります。 この場合、使用すべき正しい組織 ID は、Adobe Campaign インスタンスの下に表示されるものです。

<!--
>[!NOTE]
>
>If you have different organization IDs for Adobe Campaign and Adobe Analytics, please reach out to Customer Care to get them aligned.
-->

### Adobe Campaign のインスタンスが AWS でホストされているかどうかを知るにはどうすればよいですか？{#hosted-aws}

インスタンスが AWS でホストされているかどうかを確認するには、以下の手順に従います。

1. ログイン URL を取得します。 ログイン URL は、Campaign インスタンスへのログインに利用する URL で、ほとんどの場合、「.campaign.adobe.com」または「.neolane.net」で終わります。
1. ターミナルを開いて、ログイン URL に対して **[!DNL nslookup]** コマンドを実行します。

   `doe-macOS% nslookup myinstance.campaign.adobe.com`

1. 応答で、インスタンスに関する情報が返されます。

   ```
   doe-macOS% nslookup myinstance.campaign.adobe.com
   Server:     12.34.5.678
   Address:    12.34.5.678#99
   
   Non-authoritative answer:
   myinstance.campaign.adobe.com
   canonical name = myinstance-mkt-prod1.campaign.adobe.com.
   myinstance-mkt-prod1.campaign.adobe.com
   canonical name = myinstance-mkt-prod1-1.campaign.adobe.com.
   Name: myinstance-mkt-prod1-1.campaign.adobe.com
   Address: 12.34.567.89
   ```

1. 返された IP アドレスに対して **nslookup** コマンドを実行します。

   `doe-macOS% nslookup 12.34.567.89`

1. 返された結果の「name」の値を確認します。 「amazonaws.com」が含まれている場合は、インスタンスが AWS でホストされていることを意味します。

   ```
   doe-macOS% nslookup 12.34.567.89
   Server:     12.34.5.678
   Address:    12.34.5.678#99
   
   Non-authoritative answer:
   89.567.34.12.in-addr.arpa   name = ec2-12-34-567-89.address.amazonaws.com.
   ```

>[!NOTE]
>
>AWS に移行したい場合は、カスタマーサクセスマネージャーに問い合わせて、プロセスを開始してください。
