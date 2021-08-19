---
product: campaign
solution: Campaign
title: サブドメインの SSL 証明書の監視
description: サブドメインの SSL 証明書の監視方法の詳細
feature: Campaign コントロールパネル
role: Architect
level: Experienced
exl-id: a7888e1c-259d-4601-951b-0f1062d90dc2
source-git-commit: 3bd3dcc0e09d887cab7d810d43f2c72bb4251ac9
workflow-type: tm+mt
source-wordcount: '405'
ht-degree: 98%

---

# サブドメインの SSL 証明書の監視 {#monitoring-ssl-certificates}

>[!AVAILABILITY]
>
>この機能は、Campaign v8では使用できません。

## SSL 証明書について {#about-ssl-certificates}

Adobe Campaign では、ランディングページ（特に、お客様の機密情報を収集するページ）をホストするサブドメインを保護することをお勧めします。

**SSL（Secure Socket Layer）暗号化**&#x200B;は、アドビのシステムで使用するように設定したサブドメインを確実に保護します。お客様が Web フォームに記入したり Adobe Campaign がホストするランディングページに訪問したりする場合、デフォルトでは、情報が保護されないプロトコル（HTTP）で送信されます。確実にセキュリティを強化するには、送信される情報を HTTPS プロトコルで保護します。例えば、「http://info.mywebsite.com/」サブドメインアドレスは、「https://info.mywebsite.com/」になります。

**SSL 証明書は、設定されたサブドメイン自体にはインストールされません**。関連するサブドメイン（主に、ランディングページやリソースページなどをホストするサブドメイン）にインストールされます。

**SSL 証明書は、一定期間提供されます**（1 年間、60 日間など）。証明書の期限が切れると、ランディングページにアクセスしたりサブドメインからリソースを使用したりする際に問題が発生する可能性があります。これを回避するために、コントロールパネルを使用して、サブドメインの SSL 証明書を監視したり、その更新プロセスを開始したりできます。

![](assets/no_certificate.png)

## SSL 証明書の監視 {#monitoring-certificates}

>[!CONTEXTUALHELP]
>id="cp_subdomain_details"
>title="サブドメインの詳細"
>abstract="サブドメインの情報を取得します。"

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

>[!IMPORTANT]
>
>コントロールパネルから使用できる証明書の更新は、ベータ版です。通知なしに頻繁に更新および変更される可能性があります。

**関連トピック：**

* [サブドメインの SSL 証明書の更新](../../subdomains-certificates/using/renewing-subdomain-certificate.md)
* [サブドメインのブランディング](../../subdomains-certificates/using/subdomains-branding.md)
