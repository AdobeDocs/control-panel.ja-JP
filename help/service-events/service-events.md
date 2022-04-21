---
product: campaign
solution: Campaign
title: 主要な連絡先とイベントの監視
description: 'Adobe時にインスタンスや主要連絡先で発生したイベントを識別する方法を説明します。 '
feature: Control Panel
role: Architect
level: Intermediate
source-git-commit: da68420340ea8605f6e1347e86797c9e6a790ea6
workflow-type: tm+mt
source-wordcount: '340'
ht-degree: 2%

---

# 主要な連絡先とイベントの監視 {#keycontacts-events}

>[!CONTEXTUALHELP]
>id="cp_servicecalendar_serviceevents"
>title="サービスカレンダー"
>abstract="「主要連絡先」セクションには、インスタンスに関するリクエストや問題に関して連絡を取るAdobeの人物が一覧表示されます。 「サービスイベントカレンダー」セクションでは、選択したインスタンスの過去および今後のすべてのリリースおよびサービスレビューを特定できます。"

>[!IMPORTANT]
>
>サービスカレンダーはベータ版で利用でき、予告なしに頻繁に更新や変更がおこなわれます。

Campaign インスタンスを監視するには、インスタンスで計画されているイベントを識別する必要があります。

Campaign コントロールパネルを使用すると、インスタンスで発生したリリースやサービスレビューを監視し、Adobe時に要求や問題に関する主要連絡先のリストにアクセスできます。

これらの情報には、 **[!UICONTROL サービスカレンダー]** カード (Campaign コントロールパネルのホームページ )

## 主要連絡先 {#key-contacts}

この **[!UICONTROL 主要連絡先]** 「 」セクションには、インスタンスに関するあらゆるリクエストや問題について連絡できるAdobeの担当者が一覧表示されます。

>[!NOTE]
>
>このセクションには、Managed Service Accounts の情報のみが表示されます。

![](assets/service-events-contacts.png)

主な連絡先には、次の役割が含まれます。

* **[!UICONTROL TAM]**:テクニカルアカウントマネージャ
* **[!UICONTROL CSM]**:カスタマーサクセスマネージャー
* **[!UICONTROL 配信品質]**:配信品質操作の連絡先、
* **[!UICONTROL 遷移マネージャ]**:Managed Services Transition Manager(Managed Servicesアカウントのみ )
* **[!UICONTROL オンボーディングスペシャリスト]**:Campaign Classicへのオンボーディングを支援するためにアカウントに割り当てられたスペシャリスト (Managed Servicesアカウントのみ )。

## イベント {#events}

この **[!UICONTROL サービスイベントカレンダー]** 「 」セクションには、選択したインスタンスの過去および今後のリリースとサービスレビューがすべて表示されます。

![](assets/service-events-calendar.png)

この **[!UICONTROL 注意]** 列には、各リリースのステータスに関する情報が表示されます。

* **[!UICONTROL 一般公開]**:最新の安定したビルド。
* **[!UICONTROL 限定的な可用性]**:オンデマンドデプロイメントのみ。
* **[!UICONTROL リリース候補]**:エンジニアリングが検証されました。 本番環境での検証待ちです。
* **[!UICONTROL プレリリース]**:お客様の特定のニーズに対応するための以前の可用性。
* **[!UICONTROL 利用できなくなりました]**:ビルドには大きな問題はありませんが、新しい問題が追加のバグ修正で利用できます。 アップグレードが必要です。
* **[!UICONTROL 非推奨]**:既知の不具合を埋め込むビルド。
ビルドはサポートされなくなりました。 アップグレードは必須です。

1 つまたは複数の今後のイベントにフラグを割り当てて、イベントを追跡することができます。 これをおこなうには、イベント名の横にある楕円形のボタンをクリックします。

![](assets/service-events-flag.png)
