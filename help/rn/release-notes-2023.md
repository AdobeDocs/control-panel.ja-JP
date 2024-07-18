---
title: リリースノート 2023
description: このページでは、コントロールパネルの 2023年リリースをすべて掲載しています。
feature: Control Panel, Release Notes
role: Admin
level: Experienced
exl-id: 9a83e32a-4c11-4784-a6fe-341ce9ebc7a7
source-git-commit: a3485766791387bd9422b4f29daf86296efafb98
workflow-type: tm+mt
source-wordcount: '350'
ht-degree: 100%

---

# リリースノート 2023 {#rn-2023}

## 2023年9月 {#september-2023}

<table>
<thead>
<tr>
<th><strong>DMARC および BIMI レコードの管理</strong><br/></th>
</tr>
</thead>
<tbody>
<tr>
<td>
<p><p>DMARC および BIMI レコードをコントロールパネルから直接追加できるようになりました。

<ul><li><strong>DMARC レコード</strong>は、送信者のドメインを認証し、悪意のある目的でのドメインの不正使用を防ぐ方法を提供します。<a href="../subdomains-certificates/using/dmarc.md">DMARC レコードの追加方法を学ぶ</a></li>
<li><strong>BIMI レコード</strong>は、メールボックスプロバイダーの受信ボックスで、メールの横に承認済みのロゴを表示して、ブランドの認知度と信頼性を高めることができます。<a href="../subdomains-certificates/using/bimi.md">BIMI レコードの追加方法を学ぶ</a></li></ul>
</td>
</tr>
</tbody>
</table>

## 2023年6月 {#june-2023}

* 既にデリゲートされたサブドメインの SSL 証明書を、サブドメインリストから直接アドビにデリゲートできるようになりました。[詳細情報](../subdomains-certificates/using/delegate-ssl.md)

* アラートメールの送信者を `"alert@notifications.campaign.adobe.com"` に変更しました。

## 2023年5月の改善点 {#may-2023}

**アドビへのサブドメインの SSL 証明書のデリゲーション**

サブドメインの SSL 証明書をアドビで管理できるようになりました。CNAME を使用してサブドメインを設定している場合、ドメインホスティングソリューションに証明書を生成するために、証明書レコードが自動的に生成および提供されます。

この機能は、新しいサブドメインを設定する場合にのみ使用できます。 既存のデリゲートされたサブドメインの証明書はデリゲートできません。[詳細情報](../subdomains-certificates/using/setting-up-new-subdomain.md)

>[!NOTE]
>
>アドビ管理の SSL は、ユーザーが無料で使用できる機能です。

## 2023年3月 {#march-2023}

**CNAME のサブドメインデリゲーションの削除**

CNAME を使用して設定されたサブドメインのデリゲーションを削除できるようになりました。[詳細情報](../subdomains-certificates/using/remove-delegated-subdomains.md)

## 2023年2月 {#february-2023}

**アドビにデリゲートされたサブドメインのデリゲーションの削除**

アドビに完全にデリゲートされたサブドメインのデリゲーションを削除できるようになりました。[詳細情報](../subdomains-certificates/using/remove-delegated-subdomains.md)

>[!NOTE]
>
>現在、デリゲーションの削除は、CNAME を使用して設定されたサブドメインでは使用できません。

**サービスカレンダー**

お使いのインスタンスで発生する重要なイベントを追跡するためのカレンダー表示がサービスカレンダーに追加されました。さらに、コントロールパネルのアラートを購読しているユーザーに送信される通知に関する情報が追加されました。[詳細情報](../service-events/service-events.md)

![](assets/do-not-localize/gif-calendar.gif)

## 2023年1月 {#january-2023}

**新しいハイブリッドホスティングモデル機能**

ハイブリッドホスティングモデルを使用しているお客様は、MID インスタンスにアクセスするための許可リストに IP アドレスを追加できるようになりました。[詳細情報](../instances-settings/using/ip-allow-listing-instance-access.md)

**証明書署名リクエスト（CSR）の機能強化**

証明書署名リクエストの生成時に、市区町村フィールドがオプションになりました。
