---
product: campaign
solution: Campaign
title: メールアラート
description: Campaign インスタンスに問題が発生した場合に E メール通知を受信する方法について説明します
feature: Control Panel
role: Architect
level: Experienced
exl-id: 7942d2b1-d28f-4760-aa25-5ba94a627fd0
source-git-commit: 6249776ef4981cd3d706bf1946be0e054b471fb6
workflow-type: tm+mt
source-wordcount: '222'
ht-degree: 100%

---

# メールアラート {#email-alerting}

作業を柔軟に行えるように、コントロールパネルにはリアルタイムのメールアラート機能が備わっています。

これらのアラートを購読するには、次の手順に従います。

1. Campaign コントロールパネルの任意の場所で「**[!UICONTROL アラート通知]**」ボタンをクリックし、「**[!UICONTROL 購読]**」をクリックします。

   ![](assets/subscribing.png)

1. 購読を確認する電子メールが送信されます。

   ![](assets/email_subscription.png)

1. 購読すると、Campaign コントロールパネルによってシステムの問題に関する通知が送信され、実行すべきアクションが推奨されます。E メールアラートは、管理者となっている&#x200B;**すべてのインスタンス**&#x200B;について登録したすべてのユーザーに送信されます。

   ![](assets/alert_sample.png)

アラートのリストを次に示します。

* **SFTP ストレージの使用**：1 台の SFTP サーバーの容量が 80％以上に到達しました。[SFTP ストレージ管理](../../sftp/using/sftp-storage-management.md)を参照してください。

* **データベース使用量**：1 台のインスタンスデータベースの容量が 80％以上に到達しました。[データベース監視](../../performance-monitoring/using/database-monitoring.md)を参照してください。

* **SSL 証明書の有効期限**：サブドメインの SSL 証明書の 1 つが期限切れになったか、60 日以内に期限切れになります。[サブドメインの SSL 証明書の監視](../../subdomains-certificates/using/monitoring-ssl-certificates.md)を参照してください。

* **SFTP IP 許可リストの有効期限**：定義した IP 範囲のいずれかが期限切れになっているか、10 日以内に期限切れになります。[IP 範囲許可リストへの登録](../../sftp/using/ip-range-allow-listing.md)を参照してください。

* **SFTP 公開鍵の有効期限**：定義した公開鍵のいずれかが期限切れになったか、10 日以内に期限切れになります。[鍵の管理](../../sftp/using/key-management.md)を参照してください。