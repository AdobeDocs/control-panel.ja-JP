---
title: 最新リリース
description: このページでは、コントロールパネルのすべての新機能と改善点を一覧表示しています。
exl-id: 13aceffb-ceaa-4cfe-8741-95d66c5c6caa
source-git-commit: e0b0daba3a5820dc80b35d8c83ffc9143d547529
workflow-type: tm+mt
source-wordcount: '501'
ht-degree: 73%

---

# 最新リリース {#control-panel-releases}

このページでは、コントロールパネルのすべての新機能と改善点を一覧表示しています。

## 2022年6月 {#june-2022}

### 新機能?

<table>
<thead>
<tr>
<th><strong>SFTP サーバーの容量を消費する上位 10 個のファイル</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>SFTP サーバー上で最も容量を消費している上位 10 個のファイルを識別できるようになりました。 <a href="../sftp/using/sftp-storage-management.md">詳細情報</a></p>
<img src="../assets/do-not-localize/sftp.gif"/>
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
<p>サービスカレンダーで、インスタンスでイベントが発生する前に E メールで通知を受け取るようにリマインダーを設定できるようになりました。 <a href="../instances-settings/using/external-accounts.md">詳細情報</a></p>
<img src="../assets/do-not-localize/reminders.gif"/>
</td>
</tr>
</tbody>
</table>

<table>
<thead>
<tr>
<th><strong>サブドメインの CSR 生成の強化</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p>CSR 生成プロセスがいくつか強化されました。 <a href="../subdomains-certificates/using/renewing-subdomain-certificate.md">詳細情報</a></p><ul><li>CSR を生成する際に、含まれるサブドメインの 1 つを共通名として選択できるようになりました。</li><li>これで、CSR を生成する前に CSR の概要をコピーできます。</li><li>CSR が生成されたら、ジョブのログから再度ダウンロードできます。 この機能は、このリリースより前に生成された証明書には適用されません。</li></ul><p>
<img src="../assets/do-not-localize/CSR.gif"/>
</td>
</tr>
</tbody>
</table>

### 改善点

**インスタンス設定**

* Campaign コントロールパネルの GPG キーの最大数が 60 個に増えました。 [詳細情報](../instances-settings/using/gpg-keys-management.md)

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
