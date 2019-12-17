---
title: サブドメインのSSL証明書の更新
description: サブドメインのSSL証明書を更新する方法を説明します
translation-type: tm+mt
source-git-commit: 85bef8fa652be883bc2afbc42a2d893ea75a4e77

---


# サブドメインのSSL証明書の更新 {#renewing-subdomains-ssl-certificates}

## 証明書の更新について {#about-certificate-renewal-process}

SSL証明書の更新プロセスには3つの手順が含まれます。これらの手順はすべてコントロールパネルから直接実行されます。

1. **証明書署名要求(CSR)の生成アドビカス**&#x200B;タマーケアによって、CSRが生成されます。 CSR を生成するために必要な情報（共通名、組織名および住所など）を提供する必要があります。
1. **SSL証明書の購入CSRは**、生成後にダウンロードして、会社が承認する認証局からSSL証明書を購入する際に使用できます。
1. **SSL証明書のインストール** SSL証明書を購入すると、必要なサブドメインにインストールできます。

## 証明書署名要求の生成(CSR) {#generating-csr}

証明書署名要求(CSR)を生成するには、次の手順に従います。

1. 「サブドメ **[!UICONTROL インと証明書]**」カードで、必要なインスタンスを選択し、「証明書を管理**[!UICONTROL 」ボタンをク]** リックします。

   ![](assets/renewal1.png)

1. 「 **[!UICONTROL Generate a CSR]**」を選択し、「**[!UICONTROL  Next]** 」をクリックして、CSR生成プロセスの手順を示すウィザードを起動します。

   ![](assets/renewal2.png)

1. フォームが表示され、CSRの生成に必要なすべての詳細が表示されます。

   Make sure you fill in the requested information fully and accurately (contact your internal team, Security and IT teams if necessary), then click **[!UICONTROL Next]**.

   * **[!UICONTROL 整理]**:
   * **[!UICONTROL 組織単位]**:
   * **[!UICONTROL インスタンス]**:サブドメインに関連付けられているCampaignインスタンスのURL。
   ![](assets/renewal3.png)

1. CSRに含めるサブドメインを選択し、「 **[!UICONTROL OK」をクリックします]**。

   ![](assets/renewal4.png)

1. 選択したサブドメインがリストに表示されます。 それぞれに対して、含めるサブドメインを選択し、「次へ」をクリッ **[!UICONTROL クします]**。

   ![](assets/renewal5.png)

1. CSRに含めるサブドメインの概要が表示されます。 「送信」 **[!UICONTROL をクリックし]**、リクエストを確認します。

   ![](assets/renewal6.png)

1. 選択内容に対応する.csrファイルが自動的に生成され、ダウンロードされます。 これで、会社が承認した認証局からSSL証明書を購入できるようになりました。

## CSRを使用した証明書の購入 {#purchasing-certificate}

コントロールパネルから証明書署名要求CSRを取得した後、組織が承認した認証局からSSL証明書を購入します。

## SSL証明書のインストール {#installing-ssl-certificate}

SSL証明書を購入したら、次の手順に従ってインスタンスにインストールします。

1. 「サブドメ **[!UICONTROL インと証明書]**」カードで、必要なインスタンスを選択し、「証明書を管理**[!UICONTROL 」ボタンをク]** リックします。

   ![](assets/renewal1.png)

1. 「SSL証明 **[!UICONTROL 書のインストール]**」をクリックし**[!UICONTROL 、「次へ]** 」をクリックして、証明書のインストール手順を示すウィザードを起動します。

   ![](assets/install1.png)

1. インストールする証明書が含まれている.zipファイルを選択し、「送信」をクリッ **[!UICONTROL クします]**。

   ![](assets/install2.png)
