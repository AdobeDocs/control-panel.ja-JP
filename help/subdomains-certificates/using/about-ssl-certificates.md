---
title: SSL 証明書について
description: SSL証明書の詳細
translation-type: tm+mt
source-git-commit: ce93b595f4fbc2b3d72aadd034f93392565cb0e2

---


# SSL 証明書について {#about-ssl-certificates}

Adobe Campaignでは、ランディングページをホストするサブドメイン、特に顧客の機密情報を収集するサブドメインを保護することをお勧めします。

**SSL（Secure Socket Layer）暗号化**&#x200B;は、Adobe にデリゲートしたサブドメインを確実に保護します。お客様が Web フォームに記入したり Adobe Campaign がホストするランディングページに訪問したりする場合、デフォルトでは、情報は非セキュアなプロトコル（HTTP）で送信されます。確実にセキュリティを強化するには、送信される情報を HTTPS プロトコルで保護します。例えば、「http://info.mywebsite.com/」サブドメインアドレスは「https://info.mywebsite.com/」になります。

**SSL 証明書は、デリゲートされたサブドメイン自体にはインストールされません**。主にランディングページやリソースページなどをホストするサブドメインにインストールされます。

**SSL証明書は、特定の期間** （1年、60日など）提供されます。 証明書の期限が切れると、ランディングページにアクセスしたりサブドメインからリソースを使用したりする際に問題が発生する可能性があります。これを回避するために、コントロールパネルを使用して、サブドメインの SSL 証明書を監視したり、その更新プロセスを開始したりできます。

More details on subdomain delegation is available [here](https://helpx.adobe.com/campaign/kb/domain-name-delegation.html).
