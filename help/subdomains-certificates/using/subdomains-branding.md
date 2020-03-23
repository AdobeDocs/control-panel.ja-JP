---
title: サブドメインのブランディング
description: サブドメインのブランディングの詳細
translation-type: ht
source-git-commit: f22e356b283ee2601c948d5c1d514a9a59c58451

---


# サブドメインのブランディング {#subdomains-branding}

>[!CONTEXTUALHELP]
>id=&quot;cp_certificate_management&quot;
>title=&quot;サブドメインと SSL 証明書について&quot;
>abstract=&quot;サブドメインと関連する SSL 証明書を監視します。&quot;
>additional-url=&quot;https://docs.adobe.com/content/help/ja-JP/control-panel/using/subdomains-and-certificates/monitoring-ssl-certificates.html&quot; text=&quot;サブドメインの SSL 証明書の監視方法&quot;

>[!IMPORTANT]
>
>コントロールパネルから使用できるサブドメインのデリゲーションは、ベータ版です。通知なしに頻繁に更新および変更される可能性があります。

## サブドメインを設定する理由 {#why-setting-up-subdomains}

サブドメインとは、ブランドや様々なタイプのトラフィック（トランザクションメッセージ、マーケティング情報など）を分離するために使用できるドメインの区分です。

トランザクションコミュニケーションとマーケティングコミュニケーションの両方を送信するために使用される「mybrand.com」ドメインの例を見てみましょう。この場合、2 つのサブドメインを設定することに決めることができます。

* トランザクションコミュニケーション（購入確認、パスワードリセットなど）用の「info.mybrand.com」サブドメイン
* 見込み客向けの E メール送信用の「marketing.mybrand.com」サブドメイン

そうすることで、ドメインおよび他のサブドメインの評価を守るのに役立ちます。例えば、配信品質が悪いために「marketing.mybrand.com」サブドメインがインターネットサービスプロバイダーによってブラックリストに登録された場合、「mybrand.com」ドメイン全体および「info.mybrand.com」サブドメインがブラックリストに登録されるのを防ぎます。

## サブドメインのデリゲート方法 {#subdomain-delegation-methods}

サブドメインデリゲーションを使用すると、Adobe Campaign で使用するためにドメインのサブセクション（技術的には「DNS ゾーン」）をデリゲーションできます。使用可能な設定方法を次に示します。

* **Adobe Campaign への完全なサブドメインデリゲーション**（推奨）：サブドメインはアドビに完全にデリゲートされます。アドビは、E メールキャンペーンの配信、レンダリング、トラッキングに必要な DNS のあらゆる側面を制御し、維持することで、Campaign をマネージドサービスとして提供できます。

* **CNAME の使用**（非推奨、コントロールパネルではサポートされません）：サブドメインを作成し、CNAME を使用してアドビ専用のレコードを指します。この設定を使用すると、アドビとお客様の両方が DNS の維持に対する責任を共有します。

次の表に、これらの方法の動作と、労力の暗黙のレベルを示します。

| デリゲート方法 | 仕組み | 労力のレベル |
|---|---|---|
| **完全なデリゲーション** | サブドメインと名前空間レコードを作成します。次に、アドビは Adobe Campaign に必要なすべての DNS レコードを設定します。<br/><br/>この設定では、アドビは、サブドメインとすべての DNS レコードを管理するすべての責任を負います。 | 低 |
| **CNAME、カスタムメソッド** | サブドメインと名前空間レコードを作成します。次に、アドビは、DNS サーバーに配置されるレコードを提供し、対応する値を Adobe Campaign DNS サーバーに設定します。<br/><br/>この設定では、お客様とアドビの両方が DNS の維持に対する責任を共有します。 | 高 |

ドメインデリゲーションに関する追加情報については、[このドキュメント](https://helpx.adobe.com/jp/campaign/kb/domain-name-delegation.html)を参照してください。

サブドメインのデリゲート方法について質問がある場合は、アドビの配信品質チームにお問い合わせいただくか、最終的にはカスタマーケアに連絡して配信品質のコンサルティングを依頼してください。

**関連トピック：**

* [新しいサブドメインの設定](../../subdomains-certificates/using/setting-up-new-subdomain.md)
* [サブドメインデリゲーション（チュートリアルビデオ）](https://docs.adobe.com/content/help/en/campaign-learn/campaign-standard-tutorials/administrating/control-panel/subdomain-delegation.html)
* [サブドメインの監視](../../subdomains-certificates/using/monitoring-subdomains.md)
