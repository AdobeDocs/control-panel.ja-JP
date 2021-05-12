---
product: campaign
solution: Campaign
title: Campaign コントロールパネルのリリース
description: Campaign コントロールパネルの最新のリリースノート。
feature: Campaign コントロールパネル
role: Architect
level: Beginner
exl-id: 13aceffb-ceaa-4cfe-8741-95d66c5c6caa
translation-type: ht
source-git-commit: 4c8347f7b0f4a776ea726f02029ea1c92a83406a
workflow-type: ht
source-wordcount: '631'
ht-degree: 100%

---

# Campaign コントロールパネルのリリース {#control-panel-releases}

最新の Campaign コントロールパネルのリリースに関する情報は、次のとおりです。

>[!NOTE]
>
>Campaign コントロールパネルは、すべての管理者ユーザーがアクセスできます。ユーザーに管理者アクセス権を付与する手順については、[この節](https://experienceleague.adobe.com/docs/control-panel/using/discover-control-panel/managing-permissions.html?lang=jp#discover-control-panel)を参照してください。
>
>Campaign Classic の場合、インスタンスは AWS でホストし、最新の [Gold Standard](https://experienceleague.adobe.com/docs/campaign-classic/using/release-notes/gs-release/gs-overview.html?lang=ja) ビルドまたは[最新の GA ビルド（21.1）](https://experienceleague.adobe.com/docs/campaign-classic/using/release-notes/latest-release.html?lang=ja#release-notes)でアップグレードする必要があります。 バージョンを確認する方法については、[この節](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/starting-with-adobe-campaign/launching-adobe-campaign.html?lang=ja#getting-your-campaign-version)を参照してください。インスタンスが AWS でホストされているかどうかを確認するには、[このページ](faq.md)で詳しく説明されている手順に従ってください。

## 2020 年 10 月 {#october-2020}

**CNAME を使用したサブドメインの設定**

CNAME を使用してアドビと機能するサブドメインを、Campaign コントロールパネルのインターフェイスから直接設定できるようになりました。[詳細を表示](subdomains-certificates/using/setting-up-new-subdomain.md)

**データベース監視の強化**

データベース監視が強化されて追加の指標が配置され、データベースの容量を消費しているリソースに関する詳細情報を取得できるようになりました。[詳細を表示](performance-monitoring/using/database-monitoring.md)

## 2020 年 6 月{#june-2020}

**サブドメイン配信品質の監査**

新しいサブドメインをデリゲートした後、コントロールパネルで配信品質チームが実行した監査を追跡できるようになりました。[詳細を表示](subdomains-certificates/using/setting-up-new-subdomain.md)

**GPG キー管理**

コントロールパネルで GPG キーのペアを生成できるようになりました。これにより、Campaign で受信する外部データを簡単に復号化できます。さらに、Campaign から送信されるデータを暗号化するための公開 GPG キーをインストールする機能も追加されました。[詳細を表示](instances-settings/using/gpg-keys-management.md)

**アクティブなプロファイルの監視**

コントロールパネルで、インスタンスが使用し、課金のためにカウントされるアクティブなプロファイルの数を監視できるようになりました。[詳細を表示](performance-monitoring/using/active-profiles-monitoring.md)

>[!IMPORTANT]
>
>Campaign コントロールパネルから使用できるアクティブなプロファイルの監視はベータ版です。通知なしに頻繁に更新および変更される可能性があります。

## 2020 年 5 月 {#may-2020}

**CNAME サブドメインの証明書管理**

CNAME メソッドで設定されたサブドメインの SSL 証明書を Campaign コントロールパネルで更新できるようになりました。[詳細を表示](subdomains-certificates/using/renewing-subdomain-certificate.md)

## 2020 年 4 月 {#april-2020}

**Google TXT レコード管理**

Campaign コントロールパネルを使用して、Gmail アドレス宛ての E メール送信に使用するすべてのサブドメインに Google TXT サイト検証レコードを追加します。[詳細を表示](subdomains-certificates/using/managing-txt-records.md)

**データベース容量の監視**

Campaign コントロールパネルに、データベース監視機能が搭載されました。データベース容量の使用率をオンデマンドで表示でき、経時的変化も確認できます。[詳細を表示](performance-monitoring/using/database-monitoring.md)

**E メールアラート**

Campaign コントロールパネルに、リアルタイムの E メールアラート機能が搭載されました。コントロールパネルにログインして登録すると、システムパフォーマンス低下の危険がある場合や将来の高いパフォーマンスを確保するために特定のアクションが必要な場合に、アラートを受信できます。[詳細を表示](performance-monitoring/using/email-alerting.md)

## 2020 年 1 月{#january-2020}

*2020 年 1 月 22 日*

管理者ユーザーがサブドメインを設定し、Campaign コントロールパネルから SSL 証明書を更新するための新しい機能が追加されました。

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

詳しくは、[該当するドキュメント](instances-settings/using/ip-allow-listing-instance-access.md)を参照してください。

## 2019 年 8 月{#august-2019}

管理者ユーザーがお使いのドメインの SSL 証明書の期限が切れる前に通知を受け取る新機能を追加しました。詳しくは、[詳細ドキュメント](subdomains-certificates/using/monitoring-ssl-certificates.md)を参照してください。

さらに、管理者ユーザーは、SFTP サーバーにアクセスするために追加された SSH キーを削除できるようになりました。

## 2019 年 7 月{#july-2019}

管理者ユーザーが Campaign Classic インスタンス設定の管理をさらに強化できるようにするための新しい機能が追加されました。新しいコントロールパネルの機能には、データ／ファイル転送用に Adobe Campaign が接続する URL を追加する機能が含まれます。

詳しくは、[詳細ドキュメント](instances-settings/using/url-permissions.md)を参照してください。
