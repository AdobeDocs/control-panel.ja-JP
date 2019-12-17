---
title: サブドメインのSSL証明書の監視
description: サブドメインのSSL証明書を監視する方法について説明します
translation-type: tm+mt
source-git-commit: 85bef8fa652be883bc2afbc42a2d893ea75a4e77

---


# Monitoring subdomains&#39; SSL certificates {#monitoring-ssl-certificates}

Adobe Campaign では、ランディングページ（特に、お客様の機密情報を収集するページ）をホストするサブドメインを保護することをお勧めします。

**SSL（Secure Socket Layer）暗号化**&#x200B;は、Adobe にデリゲートしたサブドメインを確実に保護します。お客様が Web フォームに記入したり Adobe Campaign がホストするランディングページに訪問したりする場合、デフォルトでは、情報は保護されていないプロトコル（HTTP）で送信されます。確実にセキュリティを強化するには、送信される情報を HTTPS プロトコルで保護します。例えば、「http://info.mywebsite.com/」サブドメインアドレスは、「https://info.mywebsite.com/」になります。

**SSL 証明書は、デリゲートされたサブドメイン自体にはインストールされません**。関連するサブドメイン（主に、ランディングページやリソースページなどをホストするサブドメイン）にインストールされます。

**SSL 証明書は、一定期間提供されます**（1 年間、60 日間など）。証明書の期限が切れると、ランディングページにアクセスしたりサブドメインからリソースを使用したりする際に問題が発生する可能性があります。これを回避するために、コントロールパネルを使用して、サブドメインの SSL 証明書を監視したり、その更新プロセスを開始したりできます。

![](assets/no_certificate.png)

サブドメインのSSL証明書の1つが期限切れになる前に、コントロールパネルから直接更新できます。 詳しくは、次の節を参照してください。サブド [メインのSSL証明書を更新します](../../subdomains-certificates/using/renewing-subdomain-certificate.md)。
