---
title: サブドメインの SSL 証明書の更新
description: サブドメインの SSL 証明書の更新方法の詳細
translation-type: tm+mt
source-git-commit: 2c5a4f4f48e975bd9c9de4a86d2691cfddf58354

---


# サブドメインの SSL 証明書の更新 {#renewing-subdomains-ssl-certificates}

>[!NOTE]
>
>コントロールパネルからの証明書の更新は、1月末にベータ版で利用可能になります。

## 証明書の更新について {#about-certificate-renewal-process}

SSL 証明書の更新プロセスには、以下の 3 ステップがあります。

1. **証明書署名要求（CSR）の生成**
アドビカスタマーケアによって、CSRが生成されます。CSR を生成するために必要な情報（共通名、組織名および住所など）を提供する必要があります。
1. **SSL 証明書の購入**
CSR が生成されると、ダウンロードでき、会社が承認する認証局から SSL 証明書を購入する際に使用できます。
1. **SSL 証明書のインストール**
SSL 証明書を購入したら、目的のサブドメインにインストールできます。

>[!NOTE]
>
>コントロールパネルでのSSL証明書の更新は、完全に委任されたサブドメ **インに対してのみ** 利用できます。

## 証明書署名要求（CSR）の生成 {#generating-csr}

証明書署名要求（CSR）を生成するには、次の手順に従います。

1. 「**[!UICONTROL サブドメインおよび証明書]**」カードで、目的のインスタンスを選択してから、「**[!UICONTROL &#x200B;証明書を管理]**」ボタンをクリックします。

   ![](assets/renewal1.png)

1. 「**[!UICONTROL CSR を生成]**」を選択してから、「**[!UICONTROL &#x200B;次へ]**」をクリックし、CSR 生成プロセスの手順を示すウィザードを起動します。

   ![](assets/renewal2.png)

1. SSL 証明書を生成するために必要なすべての詳細と共に、フォームが表示されます。

   Make sure you fill in the requested information fully and accurately, otherwise the certificate may not be renewed (contact your internal team, Security and IT teams if necessary), then click **[!UICONTROL Next]**.

   * **[!UICONTROL 組織]**:正式な組織名。
   * **[!UICONTROL 組織単位]**:サブドメインにリンクされたユニット(例：マーケティング、IT)。
   * **[!UICONTROL インスタンス]**（事前入力済み）:サブドメインに関連付けられているCampaignインスタンスのURL。
   ![](assets/renewal3.png)

1. CSR に含めるサブドメインを選択し、「**[!UICONTROL OK]**」をクリックします。

   ![](assets/renewal4.png)

1. 選択したサブドメインがリストに表示されます。それぞれに対して、含めるサブドメインを選択し、「**[!UICONTROL 次へ]**」をクリックします。

   ![](assets/renewal5.png)

1. CSR に含めるサブドメインの概要が表示されます。「**[!UICONTROL 送信]**」をクリックし、要求を確認します。

   ![](assets/renewal6.png)

1. 選択項目に対応する .csr ファイルが自動的に生成され、ダウンロードされます。これで、会社が承認した認証局から SSL 証明書を購入するために使用できます。

## CSR を使用した証明書の購入 {#purchasing-certificate}

コントロールパネルから証明書署名要求（CSR）を取得した後、組織によって承認されている認証局から SSL 証明書を購入します。

## SSL 証明書のインストール {#installing-ssl-certificate}

SSL証明書を購入したら、その証明書をインスタンスにインストールできます。 先に進む前に、次の前提条件を確認してください。

* 証明書署名要求(CSR)は、コントロールパネルから生成されている必要があります。 そうしないと、コントロールパネルから証明書をインストールできなくなります。
* 証明書署名要求(CSR)が、アドビに委任されたサブドメインと一致することを確認します。 例えば、委任されたサブドメインを含めることはできません。
* 証明書には現在の日付が必要です。 日付が未来の証明書はインストールできません。

証明書をインストールするには、次の手順に従います。

1. 「**[!UICONTROL サブドメインおよび証明書]**」カードで、目的のインスタンスを選択してから、「**[!UICONTROL &#x200B;証明書を管理]**」ボタンをクリックします。

   ![](assets/renewal1.png)

1. 「**[!UICONTROL SSL 証明書をインストール]**」をクリックしてから、「**[!UICONTROL &#x200B;次へ]**」をクリックし、証明書のインストールプロセスの手順を示すウィザードを起動します。

   ![](assets/install1.png)

1. インストールする証明書が含まれている .zip ファイルを選択し、「**[!UICONTROL 送信]**」をクリックします。

   ![](assets/install2.png)

SSL証明書がインストールされると、証明書の有効期限とステータスアイコンが更新されます。

サブドメインのURLアドレスがhttp **から** httpsに変更されます ****。
