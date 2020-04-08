---
title: サブドメインの SSL 証明書の更新
description: サブドメインの SSL 証明書の更新方法の詳細
translation-type: ht
source-git-commit: f08b0e68cf0a208b1385052510c06ca1eb679e63

---


# サブドメインの SSL 証明書の更新 {#renewing-subdomains-ssl-certificates}

>[!CONTEXTUALHELP]
>id="cp_add_ssl_certificate"
>title="[!CONTEXTUALHELP]
>id=&quot;cp_add_ssl_certificate&quot;
>title=&quot;SSL 証明書の追加&quot;
>abstract=&quot;SSL 証明書を追加するには、CSR を生成し、サブドメイン用の SSL 証明書を購入して、証明書バンドルをインストールする必要があります。&quot;
>additional-url=&quot;https://docs.adobe.com/content/help/ja-JP/control-panel/using/subdomains-and-certificates/renewing-subdomain-certificate.html#generating-csr&quot; text=&quot;証明書署名要求（CSR）の生成&quot;
>additional-url=&quot;https://docs.adobe.com/content/help/ja-JP/control-panel/using/subdomains-and-certificates/renewing-subdomain-certificate.html#installing-ssl-certificate&quot; text=&quot;SSL 証明書のインストール方法&quot;"
>abstract="[!IMPORTANT]"
>additional-url="コントロールパネルから使用できるサブドメインのデリゲーションは、ベータ版です。通知なしに頻繁に更新および変更される可能性があります。" text="証明書の更新について {#about-certificate-renewal-process}"
>additional-url="SSL 証明書の更新プロセスには、以下の 3 ステップがあります。" text="**証明書署名要求（CSR）の生成**
アドビカスタマーケアによって、CSR が生成されます。CSR を生成するために必要な情報（共通名、組織名および住所など）を提供する必要があります。"

>**SSL 証明書の購入**
CSR が生成されると、ダウンロードでき、会社が承認する認証局から SSL 証明書を購入する際に使用できます。
>
>**SSL 証明書のインストール**
SSL 証明書を購入したら、目的のサブドメインにインストールできます。

## [!NOTE]

コントロールパネルでの SSL 証明書の更新は、**完全にデリゲートされたサブドメイン**&#x200B;に対してのみ利用できます。

1. 証明書署名要求（CSR）の生成 {#generating-csr}**
1. [!CONTEXTUALHELP]
>id=&quot;cp_generate_csr&quot;
>title=&quot;CSR の生成&quot;
>abstract=&quot;証明書署名要求は、証明書を購入する前に、保護する予定のインスタンスおよびサブドメイン用に生成されする必要があります。&quot;**
1. [!CONTEXTUALHELP]
>id=&quot;cp_select_subdomains&quot;
>title=&quot;CSR のサブドメインの選択&quot;
>abstract=&quot;証明書署名要求に、すべてのサブドメインまたは特定のサブドメインのみを含めるよう選択できます。選択したサブドメインのみが、購入した SSL 証明書を通じて認証されます。&quot;
>additional-url=&quot;https://docs.adobe.com/content/help/ja-JP/control-panel/using/subdomains-and-certificates/renewing-subdomain-certificate.html#generating-csr&quot; text=&quot;証明書署名要求（CSR）の生成&quot;
>additional-url=&quot;https://docs.adobe.com/content/help/ja-JP/control-panel/using/subdomains-and-certificates/subdomains-branding.html&quot; text=&quot;サブドメインのブランディングについて&quot;**

>[!NOTE]証明書署名要求（CSR）を生成するには、次の手順に従います。
>
>「**[!UICONTROL サブドメインおよび証明書]**」カードで、目的のインスタンスを選択してから、「**[!UICONTROL 証明書を管理]**」ボタンをクリックします。**

## ![](assets/renewal1.png)

>[!CONTEXTUALHELP]
>id="cp_generate_csr"
>title="「**[!UICONTROL CSR を生成]**」を選択してから、「**[!UICONTROL 次へ]**」をクリックし、CSR 生成プロセスの手順を示すウィザードを起動します。"
>abstract="![](assets/renewal2.png)"

>[!CONTEXTUALHELP]
>id="cp_select_subdomains"
>title="CSR を生成するために必要なすべての詳細と共に、フォームが表示されます。"
>abstract="証明書を確実に更新するために、要求された情報をすべて正確に入力していることを確認して（必要に応じて、社内チーム、セキュリティおよび IT チームに問い合わせます）から、「**[!UICONTROL 次へ]**」をクリックします。"
>additional-url="**[!UICONTROL 組織]**：正式な組織名。" text="**[!UICONTROL 組織単位]**：サブドメインにリンクされた単位（例：マーケティング、IT）。"
>additional-url="**[!UICONTROL インスタンス]**（事前入力済み）：サブドメインに関連付けられた Campaign インスタンスの URL。" text="![](assets/renewal3.png)"

CSR に含めるサブドメインを選択し、「**[!UICONTROL OK]**」をクリックします。

1. ![](assets/renewal4.png)]******

   選択したサブドメインがリストに表示されます。それぞれに対して、含めるサブドメインを選択し、「**[!UICONTROL 次へ]**」をクリックします。

1. ![](assets/renewal5.png)]******

   CSR に含めるサブドメインの概要が表示されます。「**[!UICONTROL 送信]**」をクリックし、要求を確認します。

1. ![](assets/renewal6.png)

   選択項目に対応する .csr ファイルが自動的に生成され、ダウンロードされます。これで、会社が承認した認証局から SSL 証明書を購入するために使用できます。****

   * [!NOTE]]**
   * **[!UICONTROL CSR は、保存またはダウンロードされない場合に失われ、再生成する必要があります。]**
   * CSR を使用した証明書の購入 {#purchasing-certificate}]**
   ![](assets/renewal3.png)コントロールパネルから証明書署名要求（CSR）を取得した後、組織によって承認されている認証局から SSL 証明書を購入します。

1. SSL 証明書のインストール {#installing-ssl-certificate}]**

   [!CONTEXTUALHELP]
>id=&quot;cp_install_ssl_certificate&quot;
>title=&quot;SSL 証明書のインストール&quot;
>abstract=&quot;組織が承認した認証局から購入した SSL 証明書をインストールします。&quot;
>additional-url=&quot;https://docs.adobe.com/content/help/ja-JP/control-panel/using/subdomains-and-certificates/subdomains-branding.html&quot; text=&quot;サブドメインのブランディングについて&quot;

1. SSL 証明書を購入したら、インスタンスにインストールできます。先に進む前に、次の前提条件を必ず確認してください。****

   ![](assets/renewal5.png)証明書署名要求（CSR）は、コントロールパネルから生成されている必要があります。そうでない場合、コントロールパネルから証明書をインストールできなくなります。

1. 証明書署名要求（CSR）は、アドビにデリゲートされたサブドメインと一致する必要があります。例えば、デリゲートされたもの以外のサブドメインを含めることはできません。****

   ![](assets/renewal6.png)証明書の日付は現在の日付である必要があります。将来の日付になっている証明書はインストールできません。証明書は有効期限が切れていない（開始日と終了日が有効）必要があります。

1. 証明書は、Comodo、DigiCert、GoDaddy などの信頼できる認証局（CA）によって発行される必要があります。

   >[!NOTE]証明書のサイズは 2048 bit、アルゴリズムは RSA である必要があります。
   >
   >証明書は X.509 PEM 形式である必要があります。

## SAN 証明書がサポートされています。{#purchasing-certificate}

ワイルドカード証明書はサポートされていません。

## ZIP ファイルまたは証明書をパスワードで保護しないでください。{#installing-ssl-certificate}

>[!CONTEXTUALHELP]
>id="cp_install_ssl_certificate"
>title="ZIP ファイルには、できれば個々のファイルに以下の項目のみを含める必要があります。"
>abstract="エンドエンティティ証明書。"
>additional-url="中間証明書チェーン（適切な順序で配列）。" text="ルート証明書（オプション）。"

証明書をインストールするには、次の手順に従います。

* 「**[!UICONTROL サブドメインおよび証明書]**」カードで、目的のインスタンスを選択してから、「**[!UICONTROL 証明書を管理]**」ボタンをクリックします。
* ![](assets/renewal1.png)
* 「**[!UICONTROL SSL 証明書をインストール]**」をクリックしてから、「**[!UICONTROL 次へ]**」をクリックし、証明書のインストールプロセスの手順を示すウィザードを起動します。
* ![](assets/install1.png)
* インストールする証明書が含まれている .zip ファイルを選択し、「**[!UICONTROL 送信]**」をクリックします。
* ![](assets/install2.png)
* [!NOTE]
* CSR に含まれるすべてのドメイン／サブドメインに証明書がインストールされます。証明書に存在する追加のドメイン／サブドメインは考慮されません。
* SSL 証明書がインストールされると、それに応じて証明書の有効期限とステータスアイコンが更新されます。
* **関連トピック：**
   * [SSL 証明書の追加（チュートリアルビデオ）[#$tu67]
   * 
   * 

To install the certificate, follow these steps:

1. In the **[!UICONTROL Subdomains &amp; Certificates]** card, select the desired instance, then click the **[!UICONTROL Manage Certificate]** button.

   ![](assets/renewal1.png)

1. Click **[!UICONTROL Install SSL Certificate]**, then **[!UICONTROL Next]** to launch the wizard that will guide you through the certificate installation process.

   ![](assets/install1.png)

1. Select the .zip file that contains the certificate to install, then click **[!UICONTROL Submit]**.

   ![](assets/install2.png)

>[!NOTE]
>
>The certificate will get installed on all domains/subdomains included in the CSR. Any additional domain/subdomain present in the certificate will not be taken into account.

Once the SSL certificate is installed, the certificate&#39;s expiration date and status icon are updated accordingly.

**Related topics:**

* [Adding SSL certificates (tutorial video)-ERR:REF-NOT-FOUND-
* [Subdomains branding](../../subdomains-certificates/using/subdomains-branding.md)
* [Monitoring your subdomains](../../subdomains-certificates/using/monitoring-subdomains.md)