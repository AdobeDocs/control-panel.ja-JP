---
title: サブドメインの SSL 証明書の更新
description: サブドメインの SSL 証明書の更新方法の詳細
translation-type: tm+mt
source-git-commit: f08b0e68cf0a208b1385052510c06ca1eb679e63

---


# サブドメインの SSL 証明書の更新 {#renewing-subdomains-ssl-certificates}

>[!CONTEXTUALHELP]
>id=&quot;cp_add_ssl_certificate&quot;
>title=&quot;SSL 証明書の追加&quot;
>abstract=&quot;SSL 証明書を追加するには、CSR を生成し、サブドメイン用の SSL 証明書を購入して、証明書バンドルをインストールする必要があります。&quot;
>additional-url=&quot;https://docs.adobe.com/content/help/ja-JP/control-panel/using/subdomains-and-certificates/renewing-subdomain-certificate.html#generating-csr&quot; text=&quot;証明書署名要求（CSR）の生成&quot;
>additional-url=&quot;https://docs.adobe.com/content/help/ja-JP/control-panel/using/subdomains-and-certificates/renewing-subdomain-certificate.html#installing-ssl-certificate&quot; text=&quot;SSL 証明書のインストール方法&quot;

>[!IMPORTANT]
>
>コントロールパネルから使用できるサブドメインのデリゲーションは、ベータ版です。通知なしに頻繁に更新および変更される可能性があります。

## 証明書の更新について {#about-certificate-renewal-process}

SSL 証明書の更新プロセスには、以下の 3 ステップがあります。

1. **証明書署名要求（CSR）の生成**
アドビカスタマーケアによって、CSR が生成されます。CSR を生成するために必要な情報（共通名、組織名および住所など）を提供する必要があります。
1. **SSL 証明書の購入**
CSR が生成されると、ダウンロードでき、会社が承認する認証局から SSL 証明書を購入する際に使用できます。
1. **SSL 証明書のインストール**
SSL 証明書を購入したら、目的のサブドメインにインストールできます。

>[!NOTE]
>
>コントロールパネルでの SSL 証明書の更新は、**完全にデリゲートされたサブドメイン**&#x200B;に対してのみ利用できます。

## 証明書署名要求（CSR）の生成 {#generating-csr}

>[!CONTEXTUALHELP]
>id=&quot;cp_generate_csr&quot;
>title=&quot;CSR の生成&quot;
>abstract=&quot;証明書署名要求は、証明書を購入する前に、保護する予定のインスタンスおよびサブドメイン用に生成されする必要があります。&quot;

>[!CONTEXTUALHELP]
>id=&quot;cp_select_subdomains&quot;
>title=&quot;CSR のサブドメインの選択&quot;
>abstract=&quot;証明書署名要求に、すべてのサブドメインまたは特定のサブドメインのみを含めるよう選択できます。選択したサブドメインのみが、購入した SSL 証明書を通じて認証されます。&quot;
>additional-url=&quot;https://docs.adobe.com/content/help/ja-JP/control-panel/using/subdomains-and-certificates/renewing-subdomain-certificate.html#generating-csr&quot; text=&quot;証明書署名要求（CSR）の生成&quot;
>additional-url=&quot;https://docs.adobe.com/content/help/ja-JP/control-panel/using/subdomains-and-certificates/subdomains-branding.html&quot; text=&quot;サブドメインのブランディングについて&quot;

証明書署名要求（CSR）を生成するには、次の手順に従います。

1. カードで、 **[!UICONTROL Subdomains & Certificates]** 目的のインスタンスを選択し、ボタンをクリック **[!UICONTROL Manage Certificate]** します。

   ![](assets/renewal1.png)

1. Select **[!UICONTROL Generate a CSR]**, then click **[!UICONTROL Next]** to launch the wizard that will guide you through the CSR generation process.

   ![](assets/renewal2.png)

1. CSR を生成するために必要なすべての詳細と共に、フォームが表示されます。

   Make sure you fill in the requested information fully and accurately, otherwise the certificate may not be renewed (contact your internal team, Security and IT teams if necessary), then click **[!UICONTROL Next]**.

   * **[!UICONTROL Organization]**:正式な組織名。
   * **[!UICONTROL Organization Unit]**:サブドメインにリンクされたユニット(例：マーケティング、IT)。
   * **[!UICONTROL Instance]** （事前入力済み）:サブドメインに関連付けられているキャンペーンインスタンスのURL。
   ![](assets/renewal3.png)

1. CSR に含めるサブドメインを選択し、「**[!UICONTROL OK]**」をクリックします。

   ![](assets/renewal4.png)

1. 選択したサブドメインがリストに表示されます。For each of them, select the subdomains to include, then click **[!UICONTROL Next]**.

   ![](assets/renewal5.png)

1. CSR に含めるサブドメインの概要が表示されます。Click **[!UICONTROL Submit]** to confirm your request.

   ![](assets/renewal6.png)

1. 選択項目に対応する .csr ファイルが自動的に生成され、ダウンロードされます。これで、会社が承認した認証局から SSL 証明書を購入するために使用できます。

   >[!NOTE]
   >
   >CSR は、保存またはダウンロードされない場合に失われ、再生成する必要があります。

## CSR を使用した証明書の購入 {#purchasing-certificate}

コントロールパネルから証明書署名要求（CSR）を取得した後、組織によって承認されている認証局から SSL 証明書を購入します。

## SSL 証明書のインストール {#installing-ssl-certificate}

>[!CONTEXTUALHELP]
>id=&quot;cp_install_ssl_certificate&quot;
>title=&quot;SSL 証明書のインストール&quot;
>abstract=&quot;組織が承認した認証局から購入した SSL 証明書をインストールします。&quot;
>additional-url=&quot;https://docs.adobe.com/content/help/ja-JP/control-panel/using/subdomains-and-certificates/subdomains-branding.html&quot; text=&quot;サブドメインのブランディングについて&quot;

SSL 証明書を購入したら、インスタンスにインストールできます。先に進む前に、次の前提条件を必ず確認してください。

* 証明書署名要求（CSR）は、コントロールパネルから生成されている必要があります。そうでない場合、コントロールパネルから証明書をインストールできなくなります。
* 証明書署名要求（CSR）は、アドビにデリゲートされたサブドメインと一致する必要があります。例えば、デリゲートされたもの以外のサブドメインを含めることはできません。
* 証明書の日付は現在の日付である必要があります。将来の日付になっている証明書はインストールできません。証明書は有効期限が切れていない（開始日と終了日が有効）必要があります。
* 証明書は、Comodo、DigiCert、GoDaddy などの信頼できる認証局（CA）によって発行される必要があります。
* 証明書のサイズは 2048 bit、アルゴリズムは RSA である必要があります。
* 証明書は X.509 PEM 形式である必要があります。
* SAN 証明書がサポートされています。
* ワイルドカード証明書はサポートされていません。
* ZIP ファイルまたは証明書をパスワードで保護しないでください。
* ZIP ファイルには、できれば個々のファイルに以下の項目のみを含める必要があります。
   * エンドエンティティ証明書。
   * 中間証明書チェーン（適切な順序で配列）。
   * ルート証明書（オプション）。

証明書をインストールするには、次の手順に従います。

1. カードで、 **[!UICONTROL Subdomains & Certificates]** 目的のインスタンスを選択し、ボタンをクリック **[!UICONTROL Manage Certificate]** します。

   ![](assets/renewal1.png)

1. Click **[!UICONTROL Install SSL Certificate]**, then **[!UICONTROL Next]** to launch the wizard that will guide you through the certificate installation process.

   ![](assets/install1.png)

1. Select the .zip file that contains the certificate to install, then click **[!UICONTROL Submit]**.

   ![](assets/install2.png)

>[!NOTE]
>
>証明書は、CSRに含まれるすべてのドメイン/サブドメインにインストールされます。 証明書に存在する追加のドメイン/サブドメインは考慮されません。

SSL 証明書がインストールされると、それに応じて証明書の有効期限とステータスアイコンが更新されます。

**関連トピック：**

* [SSL 証明書の追加（チュートリアルビデオ）](https://docs.adobe.com/content/help/en/campaign-learn/campaign-standard-tutorials/administrating/control-panel/adding-ssl-certificates.html)
* [サブドメインのブランディング](../../subdomains-certificates/using/subdomains-branding.md)
* [サブドメインの監視](../../subdomains-certificates/using/monitoring-subdomains.md)