---
title: サブドメインのブランディング
description: サブドメインのブランディングの詳細
translation-type: tm+mt
source-git-commit: 17f51b60310b4fbc89e2106eb4ee9251fd525a59
workflow-type: tm+mt
source-wordcount: '702'
ht-degree: 80%

---


# サブドメインのブランディング {#subdomains-branding}

>[!CONTEXTUALHELP]
>id="cp_certificate_management"
>title="サブドメインと SSL 証明書について"
>abstract="サブドメインと関連する SSL 証明書を監視します。"
>additional-url="https://docs.adobe.com/content/help/ja-JP/control-panel/using/subdomains-and-certificates/monitoring-ssl-certificates.html" text="サブドメインの SSL 証明書の監視方法"

>[!IMPORTANT]
>
>Campaign コントロールパネルのサブドメイン設定はベータ版で利用でき、頻繁な更新や変更が予告なく行われる場合があります。

## サブドメインを設定する理由 {#why-setting-up-subdomains}

サブドメインとは、ブランドや様々なタイプのトラフィック（トランザクションメッセージ、マーケティング情報など）を分離するために使用できるドメインの区分です。

トランザクションコミュニケーションとマーケティングコミュニケーションの両方を送信するために使用される「mybrand.com」ドメインの例を見てみましょう。この場合、2 つのサブドメインを設定することに決めることができます。

* トランザクションコミュニケーション（購入確認、パスワードリセットなど）用の「info.mybrand.com」サブドメイン
* 見込み客向けの E メール送信用の「marketing.mybrand.com」サブドメイン

そうすることで、ドメインおよび他のサブドメインの評価を守るのに役立ちます。例えば、配信品質が悪いために「marketing.mybrand.com」サブドメインがインターネットサービスプロバイダーによってブロックリストに追加された場合、「mybrand.com」ドメイン全体および「info.mybrand.com」サブドメインがブロックリストに追加されるのを防ぎます。

## サブドメイン設定メソッド {#subdomain-delegation-methods}

サブドメイン設定では、Adobe Campaignで使用するドメインのサブセクション（技術的には「DNSゾーン」）を構成できます。 使用可能な設定方法を次に示します。

* **Adobe Campaign への完全なサブドメインデリゲーション**（推奨）：サブドメインはアドビに完全にデリゲートされます。アドビは、E メールキャンペーンの配信、レンダリング、トラッキングに必要な DNS のあらゆる側面を制御し、維持することで、Campaign をマネージドサービスとして提供できます。

* **CNAMEの使用**:サブドメインを作成し、CNAMEを使用してAdobe固有のレコードを指定します。 この設定を使用すると、アドビとお客様の両方が DNS の維持に対する責任を共有します。

次の表に、これらの方法の動作と、労力の暗黙のレベルを示します。

| 設定方法 | 仕組み | 労力のレベル |
|---|---|---|
| **完全なデリゲーション** | サブドメインと名前空間レコードを作成します。次に、アドビは Adobe Campaign に必要なすべての DNS レコードを設定します。<br/><br/>この設定では、アドビは、サブドメインとすべての DNS レコードを管理するすべての責任を負います。 | 低 |
| **CNAME、カスタムメソッド** | サブドメインと名前空間レコードを作成します。次に、アドビは、DNS サーバーに配置されるレコードを提供し、対応する値を Adobe Campaign DNS サーバーに設定します。<br/><br/>この設定では、お客様とアドビの両方が DNS の維持に対する責任を共有します。 | 高 |

Additional information on domain configuration is available in [this documentation](https://helpx.adobe.com/jp/campaign/kb/domain-name-delegation.html).

サブドメインの設定方法について質問がある場合は、Adobeの配信品質チームにご連絡いただくか、最終的にカスタマーケアに連絡して配信品質のコンサルティングを依頼してください。

## サブドメインの使用例(Campaign Classic) (#subdomains-use-cases)

Campaign Classicインスタンスにサブドメインを設定する場合は、サブドメインを使用する使用例を選択する必要があります(を参照 [](../../subdomains-certificates/using/setting-up-new-subdomain.md))。

使用例を次に示します。

* **マーケティングコミュニケーション**：商用目的のコミュニケーション。例：販売の E メールキャンペーン。

* **トランザクションおよび運用コミュニケーション**：トランザクションコミュニケーションには、受信者が開始したプロセスの完了を目的とした情報が含まれます。例：購入確認、パスワードリセット用の E メール。組織のコミュニケーションには、商用目的でない組織内外の情報、アイデア、見解の交換が関係します。

**使用例に従ってサブドメインを分類することが、配信品質のベストプラクティスです。**&#x200B;これにより、各サブドメインの評価が分離され、保護されます。例えば、マーケティングコミュニケーション用のサブドメインがインターネットサービスプロバイダーによってブロックリストに追加された場合、トランザクションコミュニケーションサブドメインは影響を受けず、コミュニケーションを送信し続けることができます。

**マーケティングとトランザクションの両方の使用例に対してサブドメインを設定できます**。

* マーケティングの使用例では、サブドメインは **MID**（ミッドソーシング）インスタンスに設定します。
* トランザクションの使用例では、接続性を確保するために、サブドメインはすべての **RT**（Message Center／リアルタイムメッセージング）インスタンスに設定します。したがって、サブドメインはすべての RT インスタンスで動作します。

>[!NOTE]
>
>Campaign Classic を使用している場合、コントロールパネルで、使用しているマーケティングインスタンスに接続されている RT／MID インスタンスを確認できます。詳しくは、[インスタンスの詳細](../../instances-settings/using/instance-details.md)の節を参照してください。

**関連トピック：**

* [新しいサブドメインの設定](../../subdomains-certificates/using/setting-up-new-subdomain.md)
* [チュートリアルビデオ](https://docs.adobe.com/content/help/en/campaign-learn/campaign-standard-tutorials/administrating/control-panel/subdomain-delegation.html)
* [サブドメインの監視](../../subdomains-certificates/using/monitoring-subdomains.md)
