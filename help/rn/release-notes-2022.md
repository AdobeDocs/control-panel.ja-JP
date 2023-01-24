---
title: リリースノート 2022
description: このページでは、コントロールパネルの 2022年リリースをすべて掲載しています。
exl-id: 9fb18bb6-c4e4-48aa-849c-d9129add5266
source-git-commit: f617995e7313e7ac239116e0595d1746dfc7e51f
workflow-type: ht
source-wordcount: '580'
ht-degree: 100%

---

# リリースノート 2022 {#rn-2022}

## 2022年10月 {#october-2022}

SSL 証明書の 1 つが 30 日以内に期限切れになるときに、メールアラートで通知されるようになりました。[詳細情報](../performance-monitoring/using/email-alerting.md)

## 2022年9月 {#september-2022}

ハイブリッドホスティングモデルを使用するお客様は、新しいサブドメインを設定できるようになりました。 [詳細情報](../subdomains-certificates/using/setting-up-new-subdomain.md)

## 2022年8月 {#august-2022}

* ハイブリッドホスティングモデルを使用するお客様は、サブドメインを検証できるようになりました。 [詳細情報](../subdomains-certificates/using/monitoring-subdomains.md)
* 証明書署名リクエスト（CSR）の「組織単位（OU）」フィールドがオプションになりました。 [詳細情報](../subdomains-certificates/using/renewing-subdomain-certificate.md)

## 2022年7月 {#july-2022}

<table>
<thead>
<tr>
<th><strong>ハイブリッドホスティングモデルにおけるサブドメインの証明書のインストール</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p><p>ハイブリッドホスティングモデルを使用しているお客様は、サブドメインの SSL 証明書をコントロールパネルから更新できるようになりました。</p><p>詳しくは、<a href="../subdomains-certificates/using/renewing-subdomain-certificate.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

## 2022年6月 {#june-2022}

### 新機能

<table>
<thead>
<tr>
<th><strong>SFTP サーバーの容量を消費している上位 10 個のファイル</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>SFTP サーバー上で最も容量を消費している上位 10 個のファイルを特定できるようになりました。 <a href="../sftp/using/sftp-storage-management.md">詳細情報</a></p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>サービスカレンダーのリマインダー</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>サービスカレンダーで、インスタンスでイベントが発生する前にメールで通知を受け取れるよう、リマインダーを設定できるようになりました。<a href="../service-events/service-events.md">詳細情報</a></p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>サブドメインの CSR 生成の機能強化</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>CSR 生成プロセスのいくつかの機能が強化されました。 <a href="../subdomains-certificates/using/renewing-subdomain-certificate.md">詳細情報</a></p><ul><li>CSR を生成する際に、含まれるサブドメインの 1 つを共通名として選択できるようになりました。</li><li>これで、CSR を生成する前に CSR の概要をコピーできます。</li><li>CSR が生成されたら、ジョブのログから再度ダウンロードできます。この機能は、このリリースより前に生成された証明書には適用されません。</li></ul><p>

</td>
</tr>
</tbody>
</table>

### 改善点

**インスタンス設定**

* コントロールパネルの GPG キーの最大数が 60 個に増えました。 [詳細情報](../instances-settings/using/gpg-keys-management.md)

## 2022年5月 {#may-2022}

<table>
<thead>
<tr>
<th><strong>ハイブリッドホスティングモデルでのコントロールパネルの利用</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>ハイブリッドホスティングモデルを使用しているお客様が、コントロールパネルを利用できるようになりました。これらのお客様は、コントロールパネルでマーケティングインスタンスに設定した MID／RT インスタンス URL を指定することで、コントロールパネルの機能を活用できます。</p><p>詳しくは、<a href="../instances-settings/using/external-accounts.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>スループットと待ち時間の監視の更新</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>スループットと待ち時間の監視機能が強化されました。<ul><li>インスタンスのスループットに関与する上位 5 件の配信 ID を特定できるようになりました。</li><li>Campaign Classic v7／v8 のお客様は、特定のチャネルの待ち時間を視覚化できるようになりました。</p></li><p>詳しくは、<a href="../performance-monitoring/using/thoughputs-latencies.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>


## 2022年4月 {#april-2022}

<table>
<thead>
<tr>
<th><strong>インスタンスの主要連絡先とイベントの監視</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>使用しているインスタンス上での過去および今後のリリースやサービスレビューを監視できるようになりました。また、あらゆるリクエストや問題に関するアドビの主要連絡先の一覧にアクセスできるようになりました。</p><p>詳しくは、<a href="../service-events/service-events.md">詳細なドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>

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
<p>スループットと待ち時間の監視を、Campaign Standard および v8 のすべてのお客様と、スタンドアロンデプロイメント（ミッドインスタンスを除く）を持つビルド番号 9032、9330、9346 または 9349 の Campaign V7 のお客様が利用できるようになりました。</p><p>詳しくは、<a href="../performance-monitoring/using/thoughputs-latencies.md">詳細なドキュメント</a>を参照してください。</p>
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
<p>インスタンスに関する問題を回避するために、特に注意が必要となる可能性のあるワークフローパラメーターを監視できるようになりました。 </p><p>詳しくは、<a href="../performance-monitoring/using/workflow-monitoring.md">詳細ドキュメント</a>を参照してください。</p>
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
<p>インスタンスで最も長く実行されているクエリを、コントロールパネルから監視できるようになりました。</p><p>詳しくは、<a href="../performance-monitoring/using/database-active-queries.md">詳細ドキュメント</a>を参照してください。</p>
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
<p>インスタンスでの配信スループットと待ち時間の一定期間にわたるトレンドを監視できます。</p><p>詳しくは、<a href="../performance-monitoring/using/thoughputs-latencies.md">詳細ドキュメント</a>を参照してください。</p>
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
<p>配信品質の監査がまだ進行中の場合でも、新しく設定されたサブドメインで SSL 証明書の操作を実行できるようになりました。</p><p>詳しくは、<a href="../subdomains-certificates/using/renewing-subdomain-certificate.md">詳細ドキュメント</a>を参照してください。</p>
</td>
</tr>
</tbody>
</table>
