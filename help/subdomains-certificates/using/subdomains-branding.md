---
product: campaign
solution: Campaign
title: サブドメインのブランディング
description: サブドメインのブランディングの詳細
feature: Control Panel
role: Architect
level: Intermediate
exl-id: a489d051-fb95-45cf-bb6d-33aef10b7795
source-git-commit: 46a4e13e8017c5406dcd65f21c9839374dd44aa7
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 100%

---

# サブドメインのブランディング {#subdomains-branding}

>[!CONTEXTUALHELP]
>id="cp_certificate_management"
>title="サブドメインと SSL 証明書について"
>abstract="サブドメインと関連する SSL 証明書を監視します。"
>additional-url="https://experienceleague.adobe.com/docs/control-panel/using/subdomains-and-certificates/monitoring-ssl-certificates.html?lang=ja" text="SSL 証明書の監視"

## サブドメインを設定する理由  {#why-setting-up-subdomains}

>[!IMPORTANT]
>
>コントロールパネルからサブドメインを設定できる機能はベータ版であり、予告なく頻繁に更新や変更が行われる可能性があります。

サブドメインとは、ブランドや様々なタイプのトラフィック（トランザクションメッセージ、マーケティング情報など）を分離するために使用できるドメインの区分です。

トランザクションコミュニケーションとマーケティングコミュニケーションの両方を送信するために使用される「mybrand.com」ドメインの例を見てみましょう。ここでは、2 つのサブドメインを設定します。

* トランザクションコミュニケーション（購入確認、パスワードリセットなど）用の「info.mybrand.com」サブドメイン
* 見込み客向けの E メール送信用の「marketing.mybrand.com」サブドメイン

この設定により、ドメインおよび他のサブドメインの評価を維持するのに役立ちます。例えば、配信品質が悪いために「marketing.mybrand.com」サブドメインがインターネットサービスプロバイダーによってブロックリストに追加された場合、「mybrand.com」ドメイン全体および「info.mybrand.com」サブドメインがブロックリストに追加されるのを防ぎます。

## サブドメイン設定方法 {#subdomain-delegation-methods}

サブドメイン設定を使用すると、Adobe Campaign で使用するためにドメインのサブセクション（技術的には「DNS ゾーン」）を設定できます。使用可能な設定方法を次に示します。

* **Adobe Campaign への完全なサブドメインデリゲーション**（推奨）：サブドメインはアドビに完全にデリゲートされます。アドビは、E メールキャンペーンの配信、レンダリング、トラッキングに必要な DNS のあらゆる側面を制御し、維持することで、Campaign をマネージドサービスとして提供できます。

* **CNAME の使用**：サブドメインを作成し、CNAME を使用してアドビ固有のレコードを指定します。この設定を使用すると、アドビとお客様の両方が DNS の維持に対する責任を共有します。

次の表に、これらの方法の動作と、労力の暗黙のレベルを示します。

| 設定方法 | 仕組み | 労力のレベル |
|---|---|---|
| **完全なデリゲーション** | サブドメインと名前空間レコードを作成します。次に、アドビは Adobe Campaign に必要なすべての DNS レコードを設定します。<br/><br/>この設定では、アドビは、サブドメインとすべての DNS レコードを管理するすべての責任を負います。 | 低 |
| **CNAME、カスタムメソッド** | サブドメインと名前空間レコードを作成します。次に、アドビは、DNS サーバーに配置されるレコードを提供し、対応する値を Adobe Campaign DNS サーバーに設定します。<br/><br/>この設定では、お客様とアドビの両方が DNS の維持に対する責任を共有します。 | 高 |

ドメイン設定に関するその他の詳細情報については、[このドキュメント](https://experienceleague.adobe.com/docs/deliverability-learn/deliverability-best-practice-guide/additional-resources/product-specific-resources/campaign/ac-domain-name-setup.html?lang=ja)を参照してください。

サブドメインの設定方法について質問がある場合は、アドビの配信品質チームにお問い合わせいただくか、最終的にはカスタマーケアに連絡して配信品質のコンサルティングを依頼してください。

## サブドメインの活用事例（Campaign Classic）{#subdomains-use-cases}

>[!CONTEXTUALHELP]
>id="cp_add_subdomain_usecase_selection"
>title="サブドメインのユースケースの選択"
>abstract="サブドメインをユースケース別に分類することが、配信品質を確保するためのベストプラクティスです。それにより、各サブドメインの評価が分離され、保護されます。"
>additional-url="https://experienceleague.adobe.com/docs/control-panel/using/subdomains-and-certificates/setting-up-new-subdomain.html?lang=ja" text="新しいサブドメインのセットアップ"
>additional-url="https://experienceleague.adobe.com/docs/control-panel/using/subdomains-and-certificates/subdomains-branding.html?lang=ja" text="サブドメインのブランディング"

Campaign Classic インスタンスにサブドメインを設定する場合は、サブドメインを使用する使用例を選択する必要があります（](../../subdomains-certificates/using/setting-up-new-subdomain.md)新しいサブドメインの設定[を参照）。

考えられる使用例は次のとおりです。

* **マーケティングコミュニケーション**：商用目的のコミュニケーション。例：販売の E メールキャンペーン。

* **トランザクションおよび運用コミュニケーション**：トランザクションコミュニケーションには、受信者が開始したプロセスの完了を目的とした情報が含まれます。（例：購入確認、パスワードリセット用の E メール）。組織のコミュニケーションには、商用目的でない組織内外の情報、アイデア、見解の交換が関係します。

**使用例に従ってサブドメインを分類することが、配信品質のベストプラクティスです。**&#x200B;これにより、各サブドメインの評価が分離され、保護されます。例えば、マーケティングコミュニケーション用のサブドメインがインターネットサービスプロバイダーによってブロックリストに追加された場合でも、トランザクションコミュニケーションサブドメインは影響を受けず、コミュニケーションを送信し続けることができます。

**サブドメインは、マーケティングとトランザクションの両方の使用例に対して設定できます**。

* マーケティングの使用例では、サブドメインは **MID**（ミッドソーシング）インスタンスに設定します。
* トランザクションの使用例では、接続性を確保するために、サブドメインはすべての **RT**（Message Center／リアルタイムメッセージング）インスタンスに設定します。したがって、サブドメインはすべての RT インスタンスで動作します。

>[!NOTE]
>
>Campaign Classic を使用している場合、コントロールパネルで、使用しているマーケティングインスタンスに接続されている RT／MID インスタンスを確認できます。詳しくは、[インスタンスの詳細](../../instances-settings/using/instance-details.md)の節を参照してください。

**関連トピック：**

* [新しいサブドメインの設定](../../subdomains-certificates/using/setting-up-new-subdomain.md)
* [サブドメインの監視](../../subdomains-certificates/using/monitoring-subdomains.md)
