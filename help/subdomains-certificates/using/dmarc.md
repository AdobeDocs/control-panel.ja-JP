---
product: campaign
solution: Campaign
title: DMARC レコードの追加
description: サブドメインに DMARC レコードを追加する方法を説明します。
feature: Control Panel
role: Architect
level: Experienced
source-git-commit: f87a13c8553173e4303c9b95cfea5de05ff49cee
workflow-type: tm+mt
source-wordcount: '714'
ht-degree: 0%

---


# DMARC レコードの追加 {#dmarc}

## DMARC レコードについて {#about}

Domain Based Message Authentication, Reporting and Conformance(DMARC) は、組織が E メールドメインをフィッシング攻撃やスプーフィング攻撃から保護するのに役立つ、E メール認証プロトコル標準です。 SPF および DKIM チェックに失敗した E メールをメールボックスプロバイダーがどのように処理するかを決定でき、送信者のドメインを認証し、悪意のある目的でドメインが不正に使用されるのを防ぐ方法を提供できます。

<!--Detailed information on DMARC implementation is available in [Adobe Deliverability Best Practice Guide](https://experienceleague.adobe.com/docs/deliverability-learn/deliverability-best-practice-guide/additional-resources/technotes/implement-bimi.html)-->

## 制限事項と前提条件 {#limitations}

* SPF および DKIM レコードは、DMARC レコードを作成するための前提条件です。
* DMARC レコードは、完全なサブドメインデリゲーションを使用してサブドメインに対してのみ追加できます。 [サブドメイン設定メソッドの詳細を説明します](subdomains-branding.md#subdomain-delegation-methods)

## サブドメインの DMARC レコードの追加 {#add}

サブドメインに DMARC レコードを追加するには、次の手順に従います。

1. サブドメインリストで、目的のサブドメインの横にある省略記号ボタンをクリックし、「 」を選択します。 **[!UICONTROL サブドメインの詳細]**.

1. 次をクリック： **[!UICONTROL TXT レコードを追加]** 」ボタンをクリックし、「 **[!UICONTROL DMARC]** から **[!UICONTROL レコードタイプ]** 」ドロップダウンリストから選択できます。

   ![](assets/dmarc-add.png)

1. を選択します。 **[!UICONTROL ポリシータイプ]** 電子メールの 1 つに失敗した場合に受信者サーバーが従うように設定します。 使用可能なポリシーの種類は次のとおりです。

   * **[!UICONTROL なし]**,
   * **[!UICONTROL 強制隔離]** （スパムフォルダーの配置）、
   * **[!UICONTROL 拒否]** （E メールをブロック）。

   ベストプラクティスとして、DMARC の潜在的な影響を DMARC が把握できるように、DMARC ポリシーを p=none から p=quarantine にエスカレートし、p=reject にエスカレートすることで、DMARC の実装を徐々に展開することをお勧めします。

   * **手順 1:** 受け取り、使用したフィードバックを分析します (p=none)。これは、認証に失敗したメッセージに対して何のアクションも実行せず、送信者に電子メールレポートを送信するように受信者に指示します。 また、正当なメッセージが認証に失敗する場合は、SPF/DKIM の問題を確認して修正します。

   * **手順 2:** SPF と DKIM がすべての正当な E メールの認証を渡しているかどうかを確認し、ポリシーを (p=quarantine) に移動します。これは、受信側の E メールサーバーに、認証に失敗した E メールを強制隔離するよう指示します（通常は、スパムフォルダーにメッセージを配置します）。 ポリシーが強制隔離に設定されている場合は、E メールのごく一部から開始することを推奨します。

   * **手順 3:** ポリシーを (p=reject) に調整します。 注意：このポリシーは慎重に使用し、お客様の組織に適しているかどうかを判断してください。 p= reject ポリシーは、認証に失敗したドメインの E メールを受信者に対して完全に拒否（バウンス）するように指示します。 このポリシーを有効にすると、ドメインで 100%認証された電子メールのみがインボックスに配置される可能性もあります。

   >[!NOTE]
   >
   > DMARC レコードポリシーの種類が「なし」に設定されている場合、BIMI レコードの作成は利用できません。

1. DMARC レポートを受信する電子メールアドレスを入力します。 電子メールの 1 つが失敗した場合、DMARC レポートは自動的に選択した電子メールアドレスに送信されます。

   * 集計 — DMARC レポートは、例えば、特定の期間に失敗した電子メールの数など、高レベルの情報を提供します。
   * フォレンジック DMARC の失敗レポートには、例えば、失敗した E メールの送信元 IP アドレスなどの詳細情報が表示されます。

1. DMARC ポリシーが「なし」に設定されている場合は、100%のメールに適用される割合を入力します。

   ポリシーが「拒否」または「強制隔離」に設定されている場合は、E メールのごく一部から開始することをお勧めします。 ドメインからのメールが受信サーバーで認証を渡すのが増えるので、より高い割合でレコードを徐々に更新してください。

   >[!NOTE]
   >
   >ドメインで BIMI を使用している場合、DMARC ポリシーの割合は 100%にする必要があります。 BIMI は、この値が 100%未満に設定された DMARC ポリシーをサポートしていません。

   ![](assets/dmarc-add2.png)

1. DMARC レポートは 24 時間ごとに送信されます。 レポートの送信頻度は、 **[!UICONTROL レポート間隔]** フィールドに入力します。 許可された最小間隔は 1 時間で、許可された最大値は 2190 時間（3 ヶ月）です。

1. Adobe Analytics の **SPF** および **[!UICONTROL DKIM 識別子の整列]** フィールドで、E メールの SPF および DKIM 認証を確認する際の受信者サーバーの厳格度を指定します。

   * **[!UICONTROL 緩和]** mode：電子メールがサブドメインから送信された場合でもサーバーが認証を受け入れる
   * **[!UICONTROL Strict]** モードは、送信者ドメインが SPF および DKIM ドメインと完全に一致する場合にのみ認証を受け入れます。

   例えば、 `http://www.luma.com` ドメイン。 「リラックス」モードで、 `marketing.luma.com` サブドメインはサーバーによって許可されますが、「厳密」モードでは拒否されます。

1. クリック **[!UICONTROL 追加]** をクリックして、DMARC レコードの作成を確定します。

DMARC レコードの作成が処理され（約 5 分）、サブドメインの詳細画面に表示されます。 [サブドメインの TXT レコードの監視方法の詳細](gs-txt-records.md#monitor)