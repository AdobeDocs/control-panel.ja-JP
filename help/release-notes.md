---
product: campaign
solution: Campaign
title: コントロールパネルのリリース
description: Campaign コントロールパネルの最新のリリースノート。
feature: Control Panel
role: Architect
level: Beginner
exl-id: 13aceffb-ceaa-4cfe-8741-95d66c5c6caa
source-git-commit: 69f01abc8003a46e50082ea68b67df2d660f9bb7
workflow-type: tm+mt
source-wordcount: '792'
ht-degree: 78%

---

# コントロールパネルのリリース {#control-panel-releases}

コントロールパネルの最新リリースに関する情報は、次のとおりです。

>[!NOTE]
>
>Campaign コントロールパネルは、すべての管理者ユーザーがアクセスできます。ユーザーに管理者アクセス権を付与する手順については、[この節](https://experienceleague.adobe.com/docs/control-panel/using/discover-control-panel/managing-permissions.html#discover-control-panel)を参照してください。
>
>Campaign Classic v7 の場合、インスタンスを AWS でホストし、最新の [Gold Standard](https://experienceleague.adobe.com/docs/campaign-classic/using/release-notes/gs-release/gs-overview.html?lang=ja) ビルド、または最新の [GA ビルド（21.1）](https://experienceleague.adobe.com/docs/campaign-classic/using/release-notes/latest-release.html?lang=ja#release-notes) でアップグレードする必要があります。バージョンを確認する方法については、[この節](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/starting-with-adobe-campaign/launching-adobe-campaign.html?lang=ja#getting-your-campaign-version)を参照してください。インスタンスが AWS でホストされているかどうかを確認するには、[このページ](faq.md)に記載されている手順に従います。

## 2021年10月 {#october-2021}

**IP 範囲と公開鍵の編集**

作成する [IP 範囲 ](sftp/using/ip-range-allow-listing.md#editing-ip-ranges) と [ 公開鍵 ](sftp/using/key-management.md#editing-public-keys) を編集できるようになりました。 この機能は、現在のリリースより前に作成された項目には使用できないことに注意してください。Campaign コントロールパネル

**IP 範囲と公開鍵の有効期間**

IP 範囲と公開鍵が使用可能な期間を設定できるようになりました。 詳しくは、[IP 範囲許可リスト ](sftp/using/ip-range-allow-listing.md#adding-ip-addresses-allow-list) と [ キー管理 ](sftp/using/key-management.md#installing-ssh-key) の節を参照してください。

**SFTP IP 範囲および公開鍵の有効期限に関する警告**

電子メールアラート機能に、SFTP IP 許可リストの有効期限と SFTP 公開鍵の有効期限に関するアラートが含まれるようになりました。 [詳細情報](performance-monitoring/using/email-alerting.md)

**Campaign v8 での完全なサポート**

**サブドメイン** および **証明書** の管理機能が、Adobe Campaign v8 のCampaign コントロールパネルでサポートされるようになりました。

## 2021 年 8 月 {#august-2021}

**Campaign v8 のサポート**

Adobe Campaign v8 でCampaign コントロールパネルが使用できるようになりました。ただし、**Subdomain** および **Certificate** 管理機能はまだサポートされていません。 詳しくは、[Campaign v8 ドキュメント ](https://experienceleague.adobe.com/docs/campaign/campaign-v8/deploy/self-service.html){target=&quot;_blank&quot;} を参照してください

## 2020年10月 {#october-2020}

**CNAME を使用したサブドメインの設定**

アドビで使用するサブドメインを、Campaign コントロールパネルのインターフェイスから CNAME を使用して直接設定できるようになりました。[詳細を表示](subdomains-certificates/using/setting-up-new-subdomain.md)

**データベース監視の強化**

データベース監視が強化されて指標が追加され、データベースの容量を消費しているリソースに関する詳細情報を取得できるようになりました。[詳細情報](performance-monitoring/using/database-monitoring.md)

## 2020 年 6 月 {#june-2020}

**サブドメイン配信品質の監査**

新しいサブドメインをデリゲートした後、コントロールパネルで配信品質チームが実行した監査を追跡できるようになりました。[詳細を表示](subdomains-certificates/using/setting-up-new-subdomain.md)

**GPG キー管理**

コントロールパネルで GPG キーのペアを生成できるようになりました。これにより、Campaign で受信する外部データを簡単に復号化できます。さらに、Campaign から送信されるデータを暗号化するための公開 GPG キーをインストールする機能も追加されました。[詳細を表示](instances-settings/using/gpg-keys-management.md)

**アクティブなプロファイルの監視**

コントロールパネルで、インスタンスが使用し、課金のためにカウントされるアクティブなプロファイルの数を監視できるようになりました。[詳細を表示](performance-monitoring/using/active-profiles-monitoring.md)

>[!IMPORTANT]
>
>Campaign コントロールパネルから使用できるアクティブなプロファイルの監視はベータ版です。通知なしに頻繁に更新および変更される可能性があります。

## 2020年5月 {#may-2020}

**CNAME サブドメインの証明書管理**

CNAME メソッドで設定されたサブドメインの SSL 証明書を Campaign コントロールパネルで更新できるようになりました。[詳細情報](subdomains-certificates/using/renewing-subdomain-certificate.md)

## 2020 年 4 月 {#april-2020}

**Google TXT レコード管理**

Campaign コントロールパネルを使用して、Gmail アドレス宛ての E メール送信に使用するすべてのサブドメインに Google TXT サイト検証レコードを追加します。[詳細を表示](subdomains-certificates/using/managing-txt-records.md)

**データベース容量の監視**

Campaign コントロールパネルに、データベース監視機能が搭載されました。データベース容量の使用率をオンデマンドで表示でき、経時的変化も確認できます。[詳細を表示](performance-monitoring/using/database-monitoring.md)

**E メールアラート**

Campaign コントロールパネルに、リアルタイムの E メールアラート機能が搭載されました。コントロールパネルにログインして登録すると、システムパフォーマンス低下の危険がある場合や、将来の高いパフォーマンスを確保するために特定のアクションが必要な場合に、アラートを受信できます。[詳細情報](performance-monitoring/using/email-alerting.md)

## 2020 年 1 月 {#january-2020}

*2020年1月22日*

管理者ユーザーがサブドメインを設定し、Campaign コントロールパネルから SSL 証明書を更新するための新しい機能が追加されました。

詳しくは、以下のページを参照してください。
* [新しいサブドメインの設定](subdomains-certificates/using/setting-up-new-subdomain.md)
* [サブドメインの SSL 証明書の更新](subdomains-certificates/using/renewing-subdomain-certificate.md)

>[!IMPORTANT]
>
>これらの機能はベータ版であり、予告なく頻繁に更新や変更が行われる可能性があります。

## 2019年9月 {#september-2019}

*2019年9月16日*

Campaign Classic インスタンスに接続するために、管理者ユーザーが IP アドレスを許可リストに追加するための新機能を追加しました。さらに管理者ユーザーは、Campaign Classic インスタンスと、ビルドのアップグレードの実施要件のリストを表示できるようになりました。

詳しくは、[該当するドキュメント](instances-settings/using/ip-allow-listing-instance-access.md)を参照してください。

## 2019年8月 {#august-2019}

管理者ユーザーがお使いのドメインの SSL 証明書の期限が切れる前に通知を受け取る新機能を追加しました。詳しくは、[詳細ドキュメント](subdomains-certificates/using/monitoring-ssl-certificates.md)を参照してください。

さらに、管理者ユーザーは、SFTP サーバーにアクセスするために追加された SSH キーを削除できるようになりました。

## 2019年7月 {#july-2019}

管理者ユーザーが Campaign Classic インスタンス設定をさらに詳細に管理するための新機能が追加されました。新しいコントロールパネルの機能には、データ／ファイル転送用に Adobe Campaign が接続する URL を追加する機能が含まれます。

詳しくは、[詳細ドキュメント](instances-settings/using/url-permissions.md)を参照してください。
