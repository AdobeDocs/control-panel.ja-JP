---
title: SSL証明書について
description: SSL証明書の詳細
translation-type: tm+mt
source-git-commit: 6bc165f995d34d21b5bce379db3095317db10906

---


# SSL証明書について {#about-ssl-certificates}

Adobe Campaignでは、ランディングページをホストするサブドメイン、特に顧客の機密情報を収集するサブドメインを保護することをお勧めします。

**SSL(Secure Socket Layer)暗号化を使用すると** 、アドビに委任したサブドメインを安全に保護できます。 顧客がWebフォームに記入したり、Adobe Campaignでホストされるランディングページを訪問したりすると、デフォルトで、情報は安全でないプロトコル(HTTP)を使用して送信されます。 セキュリティを強化するために、HTTPSプロトコルを使用して情報をセキュリティで保護します。 例えば、「http://info.mywebsite.com/」サブドメインアドレスは「https://info.mywebsite.com/」になります。

**SSL証明書は、委任されたサブドメイン自体にはインストールされません**。 主にランディングページやリソースページなどをホストするサブドメインにインストールされます。

**SSL証明書は、特定の期間** （1年、60日など）提供されます。 証明書の有効期限が切れると、ランディングページにアクセスする場合やサブドメインのリソースを使用する場合に問題が発生する場合があります。 これを防ぐために、コントロールパネルでは、サブドメインのSSL証明書を監視し、更新プロセスを開始できます。

サブドメインの委任の詳細については、こちらを参照し [てくださ](https://helpx.adobe.com/campaign/kb/domain-name-delegation.html)い。