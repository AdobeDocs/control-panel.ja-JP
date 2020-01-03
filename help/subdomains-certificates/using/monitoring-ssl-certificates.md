---
title: サブドメインのSSL証明書の監視
description: サブドメインのSSL証明書を監視する方法について説明します
translation-type: tm+mt
source-git-commit: 001064877594a10733c054f925f254545f93145d

---


# Monitoring subdomains&#39; SSL certificates {#monitoring-ssl-certificates}

## SSL 証明書について {#about-ssl-certificates}

Adobe Campaign では、ランディングページ（特に、お客様の機密情報を収集するページ）をホストするサブドメインを保護することをお勧めします。

**SSL（Secure Socket Layer）暗号化**&#x200B;は、Adobe にデリゲートしたサブドメインを確実に保護します。お客様が Web フォームに記入したり Adobe Campaign がホストするランディングページに訪問したりする場合、デフォルトでは、情報は保護されていないプロトコル（HTTP）で送信されます。確実にセキュリティを強化するには、送信される情報を HTTPS プロトコルで保護します。例えば、「http://info.mywebsite.com/」サブドメインアドレスは、「https://info.mywebsite.com/」になります。

**SSL 証明書は、デリゲートされたサブドメイン自体にはインストールされません**。関連するサブドメイン（主に、ランディングページやリソースページなどをホストするサブドメイン）にインストールされます。

**SSL 証明書は、一定期間提供されます**（1 年間、60 日間など）。証明書の期限が切れると、ランディングページにアクセスしたりサブドメインからリソースを使用したりする際に問題が発生する可能性があります。これを回避するために、コントロールパネルを使用して、サブドメインの SSL 証明書を監視したり、その更新プロセスを開始したりできます。

![](assets/no_certificate.png)

## SSL 証明書の監視 {#monitoring-certificates}

サブドメインと証明書カードを選択すると、サブドメインのリストから直接サブドメインのSSL証明書のステ **[!UICONTROL ータスを使用でき]**ます。

サブドメインは、有効期限の視覚的情報と共に、日数で数えてSSL 証明書の有効期限が近い順に表示されます。

* **緑**：サブドメインには、今後 60 日以内に期限が切れる証明書はありません。
* **オレンジ**：1 つ以上のサブドメインに、今後 60 日以内に期限が切れる証明書があります。
* **赤**：1 つ以上のサブドメインに、今後 30 日以内に期限が切れる証明書があります。
* **グレー**:サブドメインに対する証明書がインストールされていません。

![](assets/subdomains_list.png)

To get more details on a subdomain, click the **[!UICONTROL Subdomain Details]**button.
すべての関連サブドメインのリストが表示されます。 通常、ランディングページやリソースページなどのサブドメインが含まれます。

「送信 **[!UICONTROL 者情報]**」タブには、設定済みのinbox（送信者、返信、エラー電子メール）に関する情報が表示されます。

![](assets/subdomain_details.png)

サブドメインのSSL証明書の1つが期限切れになる前に、コントロールパネルから直接更新できます。 詳しくは、次の節を参照してください。サブド [メインのSSL証明書を更新します](../../subdomains-certificates/using/renewing-subdomain-certificate.md)。

>[!NOTE]
>
>コントロールパネルからの証明書の更新は、ベータ版で近日中にご利用いただける予定です。 それまでの間、コントロールパネル内 [の証明書を監視する方法について](https://helpx.adobe.com/campaign/kb/control-panel-subdomains-certificates.html) 、詳しくはこのページを参照してください。
