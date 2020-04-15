---
title: E メールアラート
description: インスタンスに問題が発生した場合に電子メール通知を受信するキャンペーン
translation-type: tm+mt
source-git-commit: 77165e3f408f75dfb57434111b07b20ad9caab5e

---


# E メールアラート {#email-alerting}

>[!IMPORTANT]
>
>コントロール・パネルからの電子メール・アラートは、4月末までに利用可能になります。

## 電子メールアラートについて {#about-email-alerts}

作業を柔軟におこなえるよう、コントロールパネルにはリアルタイムの E メールアラート機能が備わっています。

これらのアラートを登録するには、次の手順に従います。

1. コントロール **[!UICONTROL Alerting notifications]** パネルの任意の場所で使用可能なボタンをクリックし、をクリックしま **[!UICONTROL Subscribe]**&#x200B;す。

   ![](assets/subscribing.png)

1. 電子メールが送信され、購読が

   ![](assets/email_subscription.png)

1. 購読後、コントロールパネルでシステムの問題が通知され、実行するアクションを推奨します。 E メールアラートは、管理者となっている&#x200B;**すべてのインスタンス**&#x200B;について登録したすべてのユーザーに送信されます。

   ![](assets/alert_sample.png)


アラートのリストは次のとおりです。

* **SFTPストレージの使用**:1台のSFTPサーバーの容量が80%以上に達しました。 See [SFTP storage management](../../sftp/using/sftp-storage-management.md).

* **データベースの使用**:インスタンスのデータベースの1つが、その容量の80%以上に達しました。 データベー [ス監視を参照](../../performance-monitoring/using/database-monitoring.md)。

* **SSL証明書の有効期限**:サブドメインのSSL証明書の1つが期限切れになったか、60日以内に期限切れになります。 See [Monitoring subdomains&#39; SSL certificates](../../subdomains-certificates/using/monitoring-ssl-certificates.md).

