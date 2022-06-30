---
product: campaign
solution: Campaign
title: サブドメインの SSL 証明書の更新
description: サブドメインの SSL 証明書の更新方法の詳細
feature: Control Panel
role: Architect
level: Experienced
source-git-commit: 5a5ac1a604fe5bdce07479ff84184abdb2e0ddba
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 94%

---

# SSL 証明書のインストール {#installing-ssl-certificate}

>[!CONTEXTUALHELP]
>id="cp_install_ssl_certificate"
>title="SSL 証明書のインストール"
>abstract="組織で承認された認証局から購入した SSL 証明書をインストールします。"
>additional-url="https://experienceleague.adobe.com/docs/control-panel/using/subdomains-and-certificates/subdomains-branding.html?lang=ja" text="サブドメインのブランディングについて"

SSL 証明書を購入したら、インスタンスにインストールできます。先に進む前に、次の前提条件を必ず確認してください。

* 証明書署名要求（CSR）は、コントロールパネルから生成されている必要があります。そうでない場合、コントロールパネルから証明書をインストールできなくなります。
* 証明書署名要求（CSR）は、アドビと機能するように設定されたサブドメインと一致する必要があります。例えば、設定済みのサブドメインより多くのサブドメインを含めることはできません。
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

1. 「**[!UICONTROL サブドメインおよび証明書]**」カードで、目的のインスタンスを選択してから、「**[!UICONTROL 証明書を管理]**」ボタンをクリックします。

   ![](assets/renewal1.png)

1. 「**[!UICONTROL 3 - 証明書バンドルのインストール]**」を選択してから、「**[!UICONTROL 次へ]**」をクリックし、証明書のインストールプロセスの手順を示すウィザードを起動します。

   ![](assets/install1.png)

1. インストールする証明書が含まれている .zip ファイルを選択し、「**[!UICONTROL 送信]**」をクリックします。

   ![](assets/install2.png)

>[!NOTE]
>
>CSR に含まれるすべてのドメイン／サブドメインに証明書がインストールされます。証明書内に記載されている追加のドメイン／サブドメインは考慮されません。

SSL 証明書がインストールされると、それに応じて証明書の有効期限とステータスアイコンが更新されます。
