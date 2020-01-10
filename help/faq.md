---
title: コントロールパネルのよくある質問
description: コントロールパネルに関するよくある質問
translation-type: ht
source-git-commit: b728dfe0289e44188adfa6e71aac2e9fc0abc1d2

---


# よくある質問{#faq}

## IMS Org ID{#ims-org-id}

**IMS Org ID とは何ですか？**

これは、初めて Adobe Experience Cloud にログインする際にインスタンスに割り当てられる一意の ID です。形式は xxx@AdobeOrg です。

詳しくは、[Adobe Experience Cloud のドキュメント](https://marketing.adobe.com/resources/help/ja_JP/mcloud/organizations.html)を参照してください。

**IMS Org ID はどこに行けばわかりますか？**


1 つは、[Adobe Experience Cloud のホーム](https://exc-login.experiencecloud.adobe.com/exc-content/login.html?prefixtenantid=amc)／**[!UICONTROL 管理]**に移動する方法です。IMS Org ID は、「**[!UICONTROL &#x200B;管理クイックアクセス]**」セクションの下部にあります。詳しくは、[Adobe Experience Cloud のドキュメント](https://marketing.adobe.com/resources/help/ja_JP/mcloud/organizations.html)を参照してください。

もう １ つの方法は、**Admin Console** を起動することです。IMS Org ID は、URL 内に、https://adminconsole.adobe.com/xxx@AdobeOrg/overview のような形式で表示されます。

**IMS Org ID を知る必要があるのはなぜですか？**

自分で自分のインスタンスの設定を管理するためです。会社で複数のインスタンスを使用している場合に、適切なインスタンスに対する適切な情報を取得する必要があります。

**複数の IMS Org ID がある場合はどうすればよいですか？**

複数のアドビソリューションへのアクセス権がある場合、2 つ以上の IMS Org ID がある可能性があります。この場合、使用すべき正しい IMS Org ID は、Adobe Campaign インスタンスの下に表示されるものです。

>[!NOTE]
>
>Adobe Campaign と Adobe Analytics で同じ IMS Org ID がある場合、これは望ましい状態です。Analytics と Campaign の間で 1 つの IMS Org ID を持つことは、買い物かごの放棄などの複雑な事例を活用するためにソリューションを統合する予定がある場合の要件です（AA + AC の場合）。
>
>Adobe Campaign と Adobe Analytics で異なる IMS Org ID がある場合、カスタマーケアに問い合わせ、ID を整合させてください。

**Adobe Campaign インスタンスが AWS でホストされているかどうかを知るにはどうすればよいですか？**

インスタンスが AWS でホストされているかどうかを確認するには、以下の手順に従います。

1. ログイン URL を取得します。ログイン URL は、Campaign インスタンスへのログインに利用する URL で、ほとんどの場合、「.campaign.adobe.com」で終わります。
1. ターミナルを開いて、ログイン URL に対して **[!DNL nslookup]**コマンドを実行します。

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

## コントロールパネル{#control-panel}

**コントロールパネルとは何ですか？**

コントロールパネルにより、製品管理者は、様々な設定を直接管理し、Adobe Campaign に接続された SFTP サーバーの容量を監視できます。

**コントロールパネルの現在の機能には何がありますか？**


コントロールパネルでは、ニーズやその他の操作に基づいて、SFTP サーバーに対し、ストレージの追跡、IP のホワイトリストへの登録、SSH 鍵の管理を自身でおこなうことができます。

詳しくは、コントロールパネルでサポートされる操作のドキュメントを参照してください。

**コントロールパネルは Adobe Campaign 専用ですか？**

はい、コントロールパネルで管理できるのは Adobe Campaign の設定のみです。

**誰がコントロールパネルを使用できますか？**

コントロールパネルを使用できるのは、Adobe Campaign を AWS でホストしている現在のお客様の製品管理者のみです。

管理者でないユーザーがアクセスを希望する場合は、製品管理者に問い合わせて、管理者として追加してもらう必要があります。

**コントロールパネルにはどのようにしてアクセスできますか？**

コントロールパネルへのアクセスのドキュメントに記載されている指示に従ってください。

**コントロールパネルの使用に追加料金はかかりますか？**

いいえ、Adobe Campaign の現在のお客様であれば、追加費用はかかりません。
