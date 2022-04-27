---
product: campaign
solution: Campaign
title: 主要連絡先とイベントの監視
description: インスタンスで発生したイベントを特定する方法やアドビの主要連絡先について説明します。
feature: Control Panel
role: Architect
level: Intermediate
exl-id: d230aae6-4f0e-4201-bb3c-0e3f83a7c1b8
source-git-commit: 281a1a5fc677c4e98fe32c53e0f2fe69e8c72888
workflow-type: ht
source-wordcount: '340'
ht-degree: 100%

---

# 主要連絡先とイベントの監視 {#keycontacts-events}

>[!CONTEXTUALHELP]
>id="cp_servicecalendar_serviceevents"
>title="サービスカレンダー"
>abstract="「主要連絡先」セクションには、インスタンスに関するあらゆるリクエストや問題について連絡できるアドビの担当者が一覧表示されます。 「サービスイベントカレンダー」セクションでは、選択したインスタンスの過去および今後のすべてのリリースやサービスレビューを特定できます。"

>[!IMPORTANT]
>
>サービスカレンダーはベータ版であり、予告なく頻繁に更新や変更が行われる可能性があります。

Campaign インスタンスの監視では、インスタンスで予定されているイベントの特定が不可欠です。

コントロールパネルでは、インスタンスで行われるリリースやサービスレビューを監視したり、あらゆるリクエストや問題に関するアドビの主要連絡先の一覧にアクセスしたりできます。

これらの情報には、コントロールパネルのホームページにある&#x200B;**[!UICONTROL サービスカレンダー]**&#x200B;カードからアクセスできます。

## 主要連絡先 {#key-contacts}

「**[!UICONTROL 主要連絡先]**」セクションには、インスタンスに関するあらゆるリクエストや問題について連絡できるアドビの担当者が一覧表示されます。

>[!NOTE]
>
>このセクションには、Managed Service アカウントに関する情報のみが表示されます。

![](assets/service-events-contacts.png)

主要連絡先には、次の役割が含まれています。

* **[!UICONTROL TAM]**：テクニカルアカウントマネージャー
* **[!UICONTROL CSM]**：カスタマーサクセスマネージャー
* **[!UICONTROL 配信品質]**：配信品質業務に関する連絡先
* **[!UICONTROL トランジションマネージャー]**：Managed Services のトランジションマネージャー（Managed Services アカウントのみ）
* **[!UICONTROL オンボーディングスペシャリスト]**：Campaign Classic へのオンボーディングを支援するためにアカウントに割り当てられたスペシャリスト（Managed Services アカウントのみ）

## イベント {#events}

「**[!UICONTROL サービスイベントカレンダー]**」セクションには、選択したインスタンスの過去および今後のすべてのリリースやサービスレビューが表示されます。

![](assets/service-events-calendar.png)

「**[!UICONTROL メモ]**」列には、各リリースのステータスに関する情報が表示されます。

* **[!UICONTROL 一般提供（GA）]**：入手可能な最新の安定ビルドです。
* **[!UICONTROL 限定提供（LA）]**：オンデマンドデプロイメントのみ。
* **[!UICONTROL リリース候補（RC）]**：エンジニアリング部門により検証済みです。本番環境での検証待ちです。
* **[!UICONTROL プレリリース]**：お客様の特定のニーズに対応するための先行提供です。
* **[!UICONTROL 使用できなくなりました]**：このビルドに重大な問題はありませんが、追加のバグ修正が含まれている新しいビルドが提供されています。アップグレードが必要です。
* **[!UICONTROL 非推奨（廃止予定）]**：既知の不具合が含まれるビルドです。
このビルドのサポートは終了しています。アップグレードが必須です。

今後の 1 つまたは複数のイベントにフラグを割り当てて、それらのイベントを追跡することができます。 それには、イベント名の横にある省略記号ボタンをクリックします。

![](assets/service-events-flag.png)