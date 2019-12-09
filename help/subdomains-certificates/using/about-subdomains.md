---
title: サブドメインについて
description: サブドメインの詳細
translation-type: tm+mt
source-git-commit: c2ef995d49118943bdd77e6d3c14ef7ec643e672

---


# サブドメインについて {#about-subdomains}

## サブドメインを設定する理由 {#why-setting-up-subdomains}

サブドメインは、様々なタイプのトラフィック（企業、マーケティング情報など）を分離するために使用できるドメインの分割です。

情報通信とマーケティング通信の両方を送信するために使用される「mybrand.com」ドメインの例を見てみましょう。

* info.mybrand.comを参照してください。
* marketing.mybrand.comを参照してください。

この場合、「marketing.mybrand.com」サブドメインをAdobe Campaignに委任することを決定できます。 これにより、ドメインや他のサブドメインの評判を保つのに役立ちます。 例えば、配信品質が悪いために「marketing.mybrand.com」サブドメインがインターネットサービスプロバイダーによってブラックリストに登録された場合、「mybrand.com」ドメインと「info.mybrand.com」サブドメイン全体がブロックされなくなります。

## サブドメイン委任メソッド {#subdomain-delegation-methods}

サブドメインの委任を使用すると、ドメインのサブセクション（技術的には「DNSゾーン」）をAdobe Campaignで使用するために委任できます。 使用可能な設定方法は次のとおりです。

* **Adobe Campaignへの完全なサブドメイン委任** （推奨）

   サブドメインは完全にアドビに委任されます。 アドビは、電子メールキャンペーンの配信、レンダリング、追跡に必要なDNSのあらゆる側面を制御し、保守することで、Campaignをマネージドサービスとして提供できます。

* **CNAMEの使用** （推奨されず、コントロールパネルではサポートされません）:

   サブドメインを作成し、CNAMEを使用してアドビ固有のレコードを参照します。 この設定を使用すると、アドビとお客様の両方がDNSの保守作業を共有できます。

各方法（黙示的な責任、要件など）の詳細については、本書を参照して [ください](https://helpx.adobe.com/campaign/kb/domain-name-delegation.html)。
