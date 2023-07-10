---
product: campaign
solution: Campaign
title: サブドメインの SSL 証明書の監視
description: サブドメインの SSL 証明書の監視方法の詳細
feature: Control Panel
role: Architect
level: Experienced
exl-id: a7888e1c-259d-4601-951b-0f1062d90dc2
source-git-commit: 40654418f0c5b298cc4fbd66a5d835355876a12c
workflow-type: tm+mt
source-wordcount: '419'
ht-degree: 100%

---

# サブドメインの SSL 証明書の監視 {#monitoring-ssl-certificates}

## SSL 証明書について {#about-ssl-certificates}

Adobe Campaign では、ランディングページ（特に、顧客の機密情報を収集するページ）をホストするサブドメインを保護することをお勧めします。

**SSL（Secure Socket Layer）暗号化**&#x200B;は、アドビのシステムで使用するように設定したサブドメインを確実に保護します。お客様が Web フォームに記入したり Adobe Campaign がホストするランディングページに訪問したりする場合、デフォルトでは、情報が保護されないプロトコル（HTTP）で送信されます。確実にセキュリティを強化するには、送信される情報を HTTPS プロトコルで保護します。例えば、「http://info.mywebsite.com/」サブドメインアドレスは、「https://info.mywebsite.com/」になります。

**SSL 証明書は、設定されたサブドメイン自体にはインストールされません**。関連するサブドメイン（主に、ランディングページやリソースページなどをホストするサブドメイン）にインストールされます。

**SSL 証明書は、一定期間提供されます**（1 年間、60 日間など）。証明書の期限が切れると、ランディングページにアクセスしたりサブドメインからリソースを使用したりする際に問題が発生する可能性があります。これを回避するために、コントロールパネルを使用して、サブドメインの SSL 証明書を監視したり、その更新プロセスを開始したりできます。

![](assets/no_certificate.png)

## アドビへのサブドメインの SSL 証明書のデリゲート

アドビで証明書を自動的に作成し、証明書の有効期限が切れる前に毎年更新するので、アドビへのサブドメインの SSL 証明書のデリゲートを強くお勧めします。[詳しくは、アドビへのサブドメインの SSL 証明書のデリゲート方法を参照してください](delegate-ssl.md)

## SSL 証明書の監視 {#monitoring-certificates}

>[!CONTEXTUALHELP]
>id="cp_subdomain_details"
>title="サブドメインの詳細"
>abstract="サブドメインの SSL 証明書に関する情報を取得します。"

「**[!UICONTROL サブドメインおよび証明書]**」カードを選択すると、サブドメインのリストからサブドメインの SSL 証明書のステータスに直接アクセスできます。

サブドメインは、有効期限の視覚的情報と共に、日数で数えて SSL 証明書の有効期限が近い順に表示されます。

* **緑**：サブドメインには、今後 60 日以内に期限が切れる証明書はありません。
* **オレンジ**：1 つ以上のサブドメインに、今後 60 日以内に期限が切れる証明書があります。
* **赤**：1 つ以上のサブドメインに、今後 30 日以内に期限が切れる証明書があります。
* **グレー**：サブドメイン用の証明書がインストールされていません。

![](assets/subdomains_list.png)

サブドメインの証明書の詳細を取得するには、**[!UICONTROL サブドメインの詳細]**&#x200B;ボタンをクリックします。関連するすべてのサブドメインのリストが表示されます。通常、ランディングページやリソースページなどのサブドメインが含まれます。

「**[!UICONTROL 送信者情報]**」タブには、設定済みの受信ボックス（送信者、返信先、エラー E メール）に関する情報が表示されます。

![](assets/subdomain_details.png)

サブドメインの SSL 証明書の 1 つに期限切れが近づいている場合、コントロールパネルから直接更新できます。詳しくは、[サブドメインの SSL 証明書の更新](../../subdomains-certificates/using/renewing-subdomain-certificate.md)を参照してください。

**関連トピック：**

* [サブドメインの SSL 証明書の更新](../../subdomains-certificates/using/renewing-subdomain-certificate.md)
* [サブドメインのブランディング](../../subdomains-certificates/using/subdomains-branding.md)
