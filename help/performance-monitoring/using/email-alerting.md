---
title: E メールアラート
description: Campaign インスタンスに問題が発生した場合に E メール通知を受信する方法について説明します
translation-type: tm+mt
source-git-commit: e2ee8badd9fffdfadabbe6c659aef8504ee62e9d
workflow-type: tm+mt
source-wordcount: '169'
ht-degree: 100%

---


# E メールアラート {#email-alerting}

作業を柔軟におこなえるよう、コントロールパネルにはリアルタイムの E メールアラート機能が備わっています。

これらのアラートを購読するには、次の手順に従います。

1. Campaign コントロールパネルの任意の場所で「**[!UICONTROL アラート通知]**」ボタンをクリックし、「**[!UICONTROL 購読]**」をクリックします。

   ![](assets/subscribing.png)

1. 購読を確認する電子メールが送信されます。

   ![](assets/email_subscription.png)

1. 購読すると、Campaign コントロールパネルによってシステムの問題に関する通知が送信され、実行すべきアクションが推奨されます。E メールアラートは、管理者となっている&#x200B;**すべてのインスタンス**&#x200B;について登録したすべてのユーザーに送信されます。

   ![](assets/alert_sample.png)


アラートのリストを次に示します。

* **SFTP ストレージの使用**：1 台の SFTP サーバーの容量が 80％以上に到達しました。[SFTP ストレージ管理](../../sftp/using/sftp-storage-management.md)を参照してください。

* **データベースの使用**：1 台のインスタンスデータベースの容量が 80％以上に到達しました。[データベース監視](../../performance-monitoring/using/database-monitoring.md)を参照してください。

* **SSL 証明書の有効期限**：サブドメインの SSL 証明書の 1 つが期限切れになったか、60 日以内に期限切れになります。[サブドメインの SSL 証明書の監視](../../subdomains-certificates/using/monitoring-ssl-certificates.md)を参照してください。

