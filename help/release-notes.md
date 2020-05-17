---
title: コントロールパネルのリリース
translation-type: tm+mt
source-git-commit: 032a4bd28b7f246771b3f246768fca083afe487b
workflow-type: tm+mt
source-wordcount: '401'
ht-degree: 65%

---


# コントロールパネルのリリース {#control-panel-releases}

最新のコントロールパネルのリリースに関する情報は、次のとおりです。

>[!NOTE]
>
>コントロールパネルは、まだサポートされていないハイブリッド環境を除き、AWSでホストされるお客様のみ利用できます。 コントロールパネルにアクセスするためにアップグレードする必要はありません。アクセスするには、管理者ユーザーであることを確認してください。

## 2020年5月(#may-2020)

**GPG キー管理**

キャンペーンから送信されるデータを暗号化し、受信データを復号化するために、マーケティングインスタンスにGPGキーをインストールまたは生成します。 [詳細を表示](instances-settings/using/gpg-keys-management.md)

**CNAMEサブドメインの証明書管理**

コントロールパネルで、CNAMEメソッドで委任されたサブドメインのSSL証明書を更新できるようになりました。 [詳細を表示](subdomains-certificates/using/renewing-subdomain-certificate.md)

## 2020 年 4 月 {#april-2020}

**Google TXT レコード管理**

Campaign コントロールパネルを使用して、Gmail アドレス宛ての E メール送信に使用するすべてのサブドメインに Google TXT サイト検証レコードを追加します。[詳細を表示](subdomains-certificates/using/managing-txt-records.md)

**データベース容量の監視**

キャンペーンコントロールパネルには、データベース監視機能が備わっており、必要に応じて時間の経過とともにデータベースの使用率を表示できます。 [詳細を表示](performance-monitoring/using/database-monitoring.md)

**E メールアラート**

キャンペーンコントロールパネルには、リアルタイムの電子メール通知機能が備わっており、コントロールパネルにログインしてサインアップし、パフォーマンス低下の危険がある場合や、将来の高いパフォーマンスを確保するためにアラートを受け取ることができます。 [詳細を表示](performance-monitoring/using/email-alerting.md)

## 2020 年 1 月{#january-2020}

*2020 年 1 月 22 日*

管理者ユーザーがサブドメインをデリゲートし、コントロールパネルから SSL 証明書を更新するための新しい機能が追加されました。

詳しくは、次のページを参照してください。
* [新しいサブドメインの設定](subdomains-certificates/using/setting-up-new-subdomain.md)
* [サブドメインの SSL 証明書の更新](subdomains-certificates/using/renewing-subdomain-certificate.md)

>[!IMPORTANT]
>
>これらの機能はベータ版で利用可能になり、予告なしに頻繁に更新や変更がおこなわれます。

## 2019 年 9 月 {#september-2019}

*2019 年 9 月 16 日*

管理者ユーザーが Campaign Classic インスタンスに接続する IP アドレスをホワイトリストに登録するための新しい機能が追加されました。
さらに管理者ユーザーは、Campaign Classic インスタンスと、ビルドのアップグレードの実施要件のリストを表示できるようになりました。

詳しくは、[該当するドキュメント](instances-settings/using/ip-whitelisting-instance-access.md)を参照してください。

## 2019 年 8 月{#august-2019}

管理者ユーザーがお使いのドメインの SSL 証明書の期限が切れる前に通知を受け取る新機能を追加しました。詳しくは、[詳細ドキュメント](subdomains-certificates/using/monitoring-ssl-certificates.md)を参照してください。

さらに、管理者ユーザーは、SFTP サーバーにアクセスするために追加された SSH キーを削除できるようになりました。

## 2019 年 7 月{#july-2019}

管理者ユーザーが Campaign Classic インスタンス設定の管理をさらに強化できるようにするための新しい機能が追加されました。新しいコントロールパネルの機能には、データ／ファイル転送用に Adobe Campaign が接続する URL を追加する機能が含まれます。

詳しくは、[詳細ドキュメント](instances-settings/using/url-permissions.md)を参照してください。
