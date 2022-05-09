---
product: campaign
solution: Campaign
title: コントロールパネルのよくある質問
description: コントロールパネルに関するよくある質問
feature: Control Panel
role: Architect
level: Intermediate
exl-id: 4f329764-ed8b-4939-affc-ed994fd6101d
source-git-commit: c1c80c03a351613ec0c6870a11ab39a634e8eab7
workflow-type: tm+mt
source-wordcount: '770'
ht-degree: 100%

---

# よくある質問 {#faq}

## コントロールパネル {#control-panel}

### コントロールパネルとは？

コントロールパネルは、製品の管理者が様々な設定を直接管理し、Adobe Campaign に接続された SFTP サーバーの容量を監視できるようにするものです。

### コントロールパネルには現在どのような機能がありますか？

コントロールパネルでは、ニーズやその他の操作に基づいて、SFTP サーバーに対し、ストレージの追跡、IP の許可リストへの登録、SSH 鍵の管理を自身でおこなうことができます。

詳しくは、コントロールパネルがサポートする操作のドキュメントを参照してください。

### Campaign Classic v7 で利用できる機能で、Campaign v8 ではまだサポートされていないものはありますか？{#v8-restrictions}

いいえ。Campaign v7 で使用可能なすべての機能は、サブドメインや証明書管理関連の機能を含め、Campaign v8 のコントロールパネルでもサポートされるようになりました。

### コントロールパネルは Adobe Campaign 専用ですか？

はい、コントロールパネルで管理できるのは Adobe Campaign の設定のみです。

### 誰がコントロールパネルを使用できますか？

コントロールパネルを使用できるのは、Adobe Campaign を AWS でホストしている現在のお客様の製品管理者のみです。ハイブリッド環境はまだサポートされていないことに注意してください。

管理者でないユーザーがアクセスを希望する場合は、製品の管理者に問い合わせて、管理者として追加してもらう必要があります。

### Campaign Classic v7 ユーザーの場合、コントロールパネルにアクセスする条件は何ですか？ {#v7-restrictions}

コントロールパネルは、管理者ユーザーに限定されています。[詳細情報](discover/using/managing-permissions.md)。

Campaign v7 の場合は、インスタンスを Amazon Web Services（AWS）でホストし、最新の [Campaign 安定ビルド](https://experienceleague.adobe.com/docs/campaign-classic/using/release-notes/rn-overview.html?lang=ja#rn-statuses)またはビルド 9032 以降にアップグレードする必要があります。Campaign Classic v7 のバージョンを確認する方法を、[この節](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/starting-with-adobe-campaign/launching-adobe-campaign.html?lang=ja#getting-your-campaign-version)で学習します。Campaign Classic のインスタンスが AWS でホストされているかどうかを確認するには、[この節](#hosted-aws)で説明している手順に従ってください。

### コントロールパネルにアクセスする方法は？

コントロールパネルへのアクセスのドキュメントに記載されている指示に従ってください。

### コントロールパネルの使用に追加料金はかかりますか？

いいえ、Adobe Campaign の現在のお客様であれば、追加費用はかかりません。

## IMS 組織 ID {#ims-org-id}

### IMS 組織 ID とは何ですか？

これは、初めて Adobe Experience Cloud にログインする際にインスタンスに割り当てられる一意の ID です。形式は xxx@AdobeOrg です。

詳しくは、[Adobe Experience Cloud のドキュメント](https://experienceleague.adobe.com/docs/core-services/interface/administration/organizations.html?lang=ja)を参照してください。

### IMS 組織 ID はどこにありますか？


1 つは、[Adobe Experience Cloud のホーム](https://experiencecloud.adobe.com/)／**[!UICONTROL 管理]**&#x200B;に移動する方法です。IMS 組織 ID は、「**[!UICONTROL 管理クイックアクセス]**」セクションの下部にあります。詳しくは、[Adobe Experience Cloud のドキュメント](https://experienceleague.adobe.com/docs/core-services/interface/administration/organizations.html)を参照してください。

もう 1 つの方法は、**Admin Console** を起動することです。IMS 組織 ID は、URL 内に、「https://adminconsole.adobe.com/xxx@AdobeOrg/overview」のような形式で表示されます。

### IMS 組織 ID を知る必要があるのはなぜですか？

自分のインスタンスの設定を管理するためです。会社で複数のインスタンスを使用している場合、適切なインスタンスに対する適切な情報を取得する必要があります。

### 複数の IMS 組織 ID がある場合はどうすればよいですか？

複数のアドビソリューションへのアクセス権がある場合、2 つ以上の IMS 組織 ID がある可能性があります。この場合、使用すべき正しい IMS 組織 ID は、Adobe Campaign インスタンスの下に表示されるものです。

>[!NOTE]
>
>Adobe Campaign と Adobe Analytics で同じ IMS 組織 ID がある場合、これは望ましい状態です。Analytics と Campaign の間で 1 つの IMS 組織 ID を持つことは、買い物かごの放棄などの複雑な使用例を活用するためにソリューションを統合する予定がある場合の要件です（AA + AC の場合）。
>
>Adobe Campaign と Adobe Analytics で異なる IMS 組織 ID がある場合、カスタマーケアに問い合わせ、ID を整合させてください。

### Adobe Campaign のインスタンスが AWS でホストされているかどうかを知るにはどうすればよいですか？{#hosted-aws}

インスタンスが AWS でホストされているかどうかを確認するには、以下の手順に従います。

1. ログイン URL を取得します。ログイン URL は、Campaign インスタンスへのログインに利用する URL で、ほとんどの場合、「.campaign.adobe.com」または「.neolane.net」で終わります。
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

1. 返された結果の「name」の値を確認します。「amazonaws.com」が含まれている場合は、インスタンスが AWS でホストされていることを意味します。

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
