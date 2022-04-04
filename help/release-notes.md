---
product: campaign
solution: Campaign
title: コントロールパネルのリリース
description: このページでは、コントロールパネルのすべての新機能と改善点を一覧表示しています。
exl-id: 13aceffb-ceaa-4cfe-8741-95d66c5c6caa
source-git-commit: 35b849725711bfee9852cf8f503bc599f6d8eaff
workflow-type: ht
source-wordcount: '1022'
ht-degree: 100%

---

# コントロールパネルのリリース {#control-panel-releases}

このページでは、コントロールパネルのすべての新機能と改善点を一覧表示しています。

>[!NOTE]
>
>コントロールパネルは、管理者ユーザーからのみアクセスできます。権限について詳しくは、[この節](https://experienceleague.adobe.com/docs/control-panel/using/discover-control-panel/managing-permissions.html?lang=ja#discover-control-panel)を参照してください。
>
>Campaign v7 の場合は、インスタンスを Amazon Web Services（AWS）でホストし、最新の [Campaign 安定ビルド](https://experienceleague.adobe.com/docs/campaign-classic/using/release-notes/rn-overview.html?lang=ja#rn-statuses)（またはビルド 9032 以降）にアップグレードする必要があります。バージョンを確認する方法については、[この節](https://experienceleague.adobe.com/docs/campaign-classic/using/getting-started/starting-with-adobe-campaign/launching-adobe-campaign.html?lang=ja#getting-your-campaign-version)を参照してください。インスタンスが AWS でホストされているかどうかを確認するには、[このページ](faq.md#hosted-aws)に記載されている手順に従います。

## 2022年3月 {#march-2022}

<table>
<thead>
<tr>
<th><strong>スループットと待ち時間の監視の可用性</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>スループットと待ち時間の監視を、Campaign Standard および v8 のすべてのお客様と、スタンドアロンデプロイメント（ミッドインスタンスを除く）を持つビルド番号 9032、9330、9346 または 9349 の Campaign V7 のお客様が利用できるようになりました。</p><p>詳しくは、<a href="performance-monitoring/using/thoughputs-latencies.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

## 2022年2月 {#february-2022}

<table>
<thead>
<tr>
<th><strong>ワークフローパラメーターの監視</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>インスタンスに関する問題を回避するために、特に注意が必要となる可能性のあるワークフローパラメーターを監視できるようになりました。 </p><p>詳しくは、<a href="performance-monitoring/using/workflow-monitoring.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

## 2022年1月 {#january-2022}

<table>
<thead>
<tr>
<th><strong>アクティブクエリの監視</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>インスタンスで最も長く実行されているクエリを、コントロールパネルから監視できるようになりました。</p><p>詳しくは、<a href="performance-monitoring/using/database-active-queries.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>スループットと待ち時間の監視</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>インスタンスでの配信スループットと待ち時間の一定期間にわたるトレンドを監視できます。</p><p>詳しくは、<a href="performance-monitoring/using/thoughputs-latencies.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>新しいサブドメインでの SSL 証明書の操作</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>配信品質の監査がまだ進行中の場合でも、新しく設定されたサブドメインで SSL 証明書の操作を実行できるようになりました。</p><p>詳しくは、<a href="subdomains-certificates/using/renewing-subdomain-certificate.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

## 2021年10月 {#october-2021}

<table>
<thead>
<tr>
<th><strong>IP 範囲と公開鍵の有効期間</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>IP 範囲と公開鍵の有効期間を設定できるようになりました。  </p><p>詳しくは、<a href="sftp/using/ip-range-allow-listing.md#adding-ip-addresses-allow-list">IP 範囲許可リスト</a>および<a href="sftp/using/key-management.md#installing-ssh-key">鍵の管理</a>の節を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>IP 範囲と公開鍵の編集</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>作成した <a href="sftp/using/ip-range-allow-listing.md#editing-ip-ranges">IP 範囲</a>と<a href="sftp/using/key-management.md#editing-public-keys">公開鍵</a>を編集できるようになりました。この機能は、現在のコントロールパネルリリースより前に作成された項目には使用できないことに注意してください。
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>SFTP の IP 範囲と公開鍵の有効期限に関するアラート</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>メールアラート機能に、許可リストに対する SFTP IP アドレスの登録の有効期限と SFTP 公開鍵の有効期限に関するアラートが追加されました。</p><p>詳しくは、<a href="performance-monitoring/using/email-alerting.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>Campaign v8 でのフルサポート</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p><strong>サブドメイン</strong>と<strong>証明書</strong>の管理機能が Adobe Campaign v8 のコントロールパネルでサポートされるようになりました。</a></p>
</td>
</tr>
</tbody>
</table>

## 2021年8月 {#august-2021}

<table>
<thead>
<tr>
<th><strong>Campaign v8 でのサポート</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Adobe Campaign v8 でコントロールパネルが使用できるようになりました。ただし、<strong>サブドメイン</strong>と<strong>証明書</strong>の管理機能は、まだサポートされていません。</p><p>詳しくは、<a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/deploy/self-service.html?lang=ja" target="blank">Campaign v8 ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

## 2020年10月 {#october-2020}

<table>
<thead>
<tr>
<th><strong>CNAME を使用したサブドメインの設定</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>アドビで使用するサブドメインを、コントロールパネルのインターフェイスから CNAME を使用して直接設定できるようになりました。</p><p>詳しくは、<a href="subdomains-certificates/using/setting-up-new-subdomain.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>データベース監視の強化</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>データベース監視が強化されて指標が追加され、データベースの容量を消費しているリソースに関する詳細情報を取得できるようになりました。</p><p>詳しくは、<a href="performance-monitoring/using/database-monitoring.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

## 2020年6月 {#june-2020}

<table>
<thead>
<tr>
<th><strong>サブドメイン配信品質の監査</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>新しいサブドメインをデリゲートした後、コントロールパネルで配信品質チームが実行した監査を追跡できるようになりました。</p><p>詳しくは、<a href="subdomains-certificates/using/setting-up-new-subdomain.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>GPG キー管理</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>コントロールパネルで GPG キーのペアを生成できるようになりました。これにより、Campaign で受信する外部データを簡単に復号化できます。さらに、Campaign から送信されるデータを暗号化するための公開 GPG キーをインストールする機能も追加されました。</p><p>詳しくは、<a href="instances-settings/using/gpg-keys-management.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>アクティブなプロファイルの監視</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>コントロールパネルで、インスタンスが使用し、課金のためにカウントされるアクティブなプロファイルの数を監視できるようになりました。</p><p>詳しくは、<a href="performance-monitoring/using/active-profiles-monitoring.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

>[!IMPORTANT]
>
>コントロールパネルから使用できるアクティブなプロファイルの監視はベータ版です。通知なしに頻繁に更新および変更される可能性があります。

## 2020年5月 {#may-2020}

<table>
<thead>
<tr>
<th><strong>CNAME サブドメインの証明書管理</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>CNAME メソッドで設定されたサブドメインの SSL 証明書を、コントロールパネルで更新できるようになりました。</p><p>詳しくは、<a href="subdomains-certificates/using/renewing-subdomain-certificate.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

## 2020年4月 {#april-2020}

<table>
<thead>
<tr>
<th><strong>Google TXT レコード管理</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Campaign コントロールパネルを使用して、Gmail アドレス宛てのメール送信に使用するすべてのサブドメインに Google TXT サイト検証レコードを追加します。</p><p>詳しくは、<a href="subdomains-certificates/using/managing-txt-records.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>データベース容量の監視</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Campaign コントロールパネルに、データベース監視機能が搭載されました。データベース容量の使用率をオンデマンドで表示でき、経時的変化も確認できます。</p><p>詳しくは、<a href="performance-monitoring/using/database-monitoring.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>メールアラート</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>Campaign コントロールパネルに、リアルタイムのメールアラート機能が搭載されました。コントロールパネルにログインして登録すると、システムパフォーマンス低下の危険がある場合や、将来の高いパフォーマンスを確保するために特定のアクションが必要な場合に、アラートを受信できます。</p><p>詳しくは、<a href="performance-monitoring/using/email-alerting.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

## 2020年1月 {#january-2020}

管理者ユーザーがサブドメインを設定し、Campaign コントロールパネルから SSL 証明書を更新するための新しい機能が追加されました。

詳しくは、以下のページを参照してください。
* [新しいサブドメインの設定](subdomains-certificates/using/setting-up-new-subdomain.md)
* [サブドメインの SSL 証明書の更新](subdomains-certificates/using/renewing-subdomain-certificate.md)

>[!IMPORTANT]
>
>これらの機能はベータ版であり、予告なく頻繁に更新や変更が行われる可能性があります。

## 2019年9月 {#september-2019}

Campaign v7／v8 インスタンスに接続するために、管理者ユーザーが IP アドレスを許可リストに追加するための新機能を追加しました。
さらに管理者ユーザーは、Campaign v7／v8 インスタンスと、ビルドのアップグレードの実施要件のリストを表示できるようになりました。

詳しくは、[該当するドキュメント](instances-settings/using/ip-allow-listing-instance-access.md)を参照してください。

## 2019年8月 {#august-2019}

管理者ユーザーがお使いのドメインの SSL 証明書の期限が切れる前に通知を受け取る新機能を追加しました。詳しくは、[詳細ドキュメント](subdomains-certificates/using/monitoring-ssl-certificates.md)を参照してください。

さらに、管理者ユーザーは、SFTP サーバーにアクセスするために追加された SSH キーを削除できるようになりました。

## 2019年7月 {#july-2019}

管理者ユーザーが Campaign v7／v8 インスタンス設定をさらに詳細に管理できる新機能が追加されました。新しいコントロールパネルの機能には、データ／ファイル転送用に Adobe Campaign が接続する URL を追加する機能が含まれます。

詳しくは、[詳細ドキュメント](instances-settings/using/url-permissions.md)を参照してください。
