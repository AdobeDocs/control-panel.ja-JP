---
title: コントロールパネルのリリース
translation-type: tm+mt
source-git-commit: a83309bfb6e42db231fe970f47475fb85d6d441b
workflow-type: tm+mt
source-wordcount: '605'
ht-degree: 100%

---


# コントロールパネルのリリース {#control-panel-releases}

最新のコントロールパネルのリリースに関する情報は、次のとおりです。

>[!NOTE]
>
>コントロールパネルは、まだサポートされていないハイブリッド環境を除いて、AWS でホストされるお客様のみ利用できることに注意してください。コントロールパネルにアクセスするためにアップグレードする必要はありません。アクセスするには、管理者ユーザーであることを確認してください。

## 2020 年 6 月{#june-2020}

**サブドメイン配信品質の監査**

新しいサブドメインをデリゲートした後、コントロールパネルで配信品質チームが実行した監査を追跡できるようになりました。[詳細を表示](subdomains-certificates/using/setting-up-new-subdomain.md)

**GPG キー管理**

コントロールパネルで GPG キーのペアを生成できるようになりました。これにより、Campaign で受信する外部データを簡単に復号化できます。さらに、Campaign から送信されるデータを暗号化するための公開 GPG キーをインストールする機能も追加されました。[詳細を表示](instances-settings/using/gpg-keys-management.md)
* [Campaign Standard チュートリアルビデオ](https://docs.adobe.com/content/help/en/campaign-standard-learn/tutorials/administrating/control-panel/generating-and-installing-gpg-keys.html)
* [Campaign Classic チュートリアルビデオ](https://docs.adobe.com/content/help/en/campaign-classic-learn/tutorials/administrating/control-panel-acc/generating-and-installing-gpg-keys.html)

**「ホワイトリスト」と「ブラックリスト」の削除**

「ホワイトリスト」と「ブラックリスト」の両方の用語が Adobe Campaign ドキュメントから削除されました。これらの用語は、製品 UI、オプション名、内部コードにまだ存在する場合がありますが、今後の Campaign リリースでは「ブロックリスト」と「許可リスト」に置き換えられます。

**アクティブなプロファイルの監視**

コントロールパネルで、インスタンスが使用し、課金のためにカウントされるアクティブなプロファイルの数を監視できるようになりました。[詳細を表示](performance-monitoring/using/active-profiles-monitoring.md)

>[!IMPORTANT]
>
>コントロールパネルから使用できるアクティブなプロファイルの監視は、ベータ版です。通知なしに頻繁に更新および変更される可能性があります。
>
>この機能は、Campaign Standard 10368 のビルドおよび Campaign Classic 8931 のビルドで、AWS でホストされている顧客が使用できます。以前のビルドを使用している場合、この機能を使用するにはアップグレードする必要があります。

## 2020 年 5 月 {#may-2020}

**CNAME サブドメインの証明書管理**

CNAME メソッドでデリゲートされたサブドメインの SSL 証明書をコントロールパネルで更新できるようになりました。[詳細を表示](subdomains-certificates/using/renewing-subdomain-certificate.md)

## 2020 年 4 月 {#april-2020}

**Google TXT レコード管理**

Campaign コントロールパネルを使用して、Gmail アドレス宛ての E メール送信に使用するすべてのサブドメインに Google TXT サイト検証レコードを追加します。[詳細を表示](subdomains-certificates/using/managing-txt-records.md)

**データベース容量の監視**

Campaign コントロールパネルに、データベース監視機能が搭載されました。データベース容量の使用率をオンデマンドで表示でき、経時的変化も確認できます。[詳細を表示](performance-monitoring/using/database-monitoring.md)

**E メールアラート**

Campaign コントロールパネルに、リアルタイムの E メールアラート機能が搭載されました。コントロールパネルにログインして登録すると、システムパフォーマンス低下の危険がある場合や将来の高いパフォーマンスを確保するために特定のアクションが必要な場合に、アラートを受信できます。[詳細を表示](performance-monitoring/using/email-alerting.md)

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

管理者ユーザーが IP アドレスを許可リストに追加して Campaign Classic インスタンスに接続できる新しい機能を追加しました。
さらに管理者ユーザーは、Campaign Classic インスタンスと、ビルドのアップグレードの実施要件のリストを表示できるようになりました。

詳しくは、[該当するドキュメント](instances-settings/using/ip-whitelisting-instance-access.md)を参照してください。

## 2019 年 8 月{#august-2019}

管理者ユーザーがお使いのドメインの SSL 証明書の期限が切れる前に通知を受け取る新機能を追加しました。詳しくは、[詳細ドキュメント](subdomains-certificates/using/monitoring-ssl-certificates.md)を参照してください。

さらに、管理者ユーザーは、SFTP サーバーにアクセスするために追加された SSH キーを削除できるようになりました。

## 2019 年 7 月{#july-2019}

管理者ユーザーが Campaign Classic インスタンス設定の管理をさらに強化できるようにするための新しい機能が追加されました。新しいコントロールパネルの機能には、データ／ファイル転送用に Adobe Campaign が接続する URL を追加する機能が含まれます。

詳しくは、[詳細ドキュメント](instances-settings/using/url-permissions.md)を参照してください。
