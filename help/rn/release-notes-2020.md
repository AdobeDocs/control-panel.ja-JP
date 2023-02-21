---
title: リリースノート 2020
description: このページでは、コントロールパネルの 2020年リリースをすべて掲載しています。
exl-id: 70357a40-3dc1-486d-bba2-f500b3175d62
source-git-commit: 9be5a3ae48dccf74f509aa95fee29bbfdafddcdf
workflow-type: tm+mt
source-wordcount: '429'
ht-degree: 100%

---

# リリースノート 2020 {#rn-2020}

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
<p>アドビで使用するサブドメインを、コントロールパネルのインターフェイスから CNAME を使用して直接設定できるようになりました。</p><p>詳しくは、<a href="../subdomains-certificates/using/setting-up-new-subdomain.md">詳細ドキュメント</a>を参照してください。</p>
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
<p>データベース監視が強化されて指標が追加され、データベースの容量を消費しているリソースに関する詳細情報を取得できるようになりました。</p><p>詳しくは、<a href="../performance-monitoring/using/database-monitoring.md">詳細ドキュメント</a>を参照してください。</p>
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
<p>新しいサブドメインをデリゲートした後、コントロールパネルで配信品質チームが実行した監査を追跡できるようになりました。</p><p>詳しくは、<a href="../subdomains-certificates/using/setting-up-new-subdomain.md">詳細ドキュメント</a>を参照してください。</p>
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
<p>コントロールパネルで GPG キーのペアを生成できるようになりました。これにより、Campaign で受信する外部データを簡単に復号化できます。さらに、Campaign から送信されるデータを暗号化するための公開 GPG キーをインストールする機能も追加されました。</p><p>詳しくは、<a href="../instances-settings/using/gpg-keys-management.md">詳細ドキュメント</a>を参照してください。</p>
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
<p>コントロールパネルで、インスタンスが使用し、課金のためにカウントされるアクティブなプロファイルの数を監視できるようになりました。</p><p>詳しくは、<a href="../performance-monitoring/using/active-profiles-monitoring.md">詳細ドキュメント</a>を参照してください。</p>
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
<p>CNAME メソッドで設定されたサブドメインの SSL 証明書を、コントロールパネルで更新できるようになりました。</p><p>詳しくは、<a href="../subdomains-certificates/using/renewing-subdomain-certificate.md">詳細ドキュメント</a>を参照してください。</p>
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
<p>Campaign コントロールパネルを使用して、Gmail アドレス宛てのメール送信に使用するすべてのサブドメインに Google TXT サイト検証レコードを追加します。</p><p>詳しくは、<a href="../subdomains-certificates/using/managing-txt-records.md">詳細ドキュメント</a>を参照してください。</p>
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
<p>Campaign コントロールパネルに、データベース監視機能が搭載されました。データベース容量の使用率をオンデマンドで表示でき、経時的変化も確認できます。</p><p>詳しくは、<a href="../performance-monitoring/using/database-monitoring.md">詳細ドキュメント</a>を参照してください。</p>
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
<p>Campaign コントロールパネルに、リアルタイムのメールアラート機能が搭載されました。コントロールパネルにログインして登録すると、システムパフォーマンス低下の危険がある場合や、将来の高いパフォーマンスを確保するために特定のアクションが必要な場合に、アラートを受信できます。</p><p>詳しくは、<a href="../performance-monitoring/using/email-alerting.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

## 2020年1月 {#january-2020}

管理者ユーザーがサブドメインを設定し、Campaign コントロールパネルから SSL 証明書を更新するための新しい機能が追加されました。

詳しくは、以下のページを参照してください。
* [新しいサブドメインの設定](../subdomains-certificates/using/setting-up-new-subdomain.md)
* [サブドメインの SSL 証明書の更新](../subdomains-certificates/using/renewing-subdomain-certificate.md)

>[!IMPORTANT]
>
>これらの機能はベータ版であり、予告なく頻繁に更新や変更が行われる可能性があります。
