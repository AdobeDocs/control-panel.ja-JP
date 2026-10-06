---
product: campaign
solution: Campaign
title: アクティブなクエリの監視
description: コントロールパネルで Campaign インスタンス上のアクティブなクエリを監視する方法を説明します。
feature: Control Panel, Monitoring
role: Admin
level: Experienced
exl-id: a1ea14f9-ec1d-4e10-89ef-846065512e8c
TQID: 'https://experienceleague.adobe.com/9lSAwCefSWAZ37fBHpu-1rUWppKTrnXcBSACJ3JthQg'
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: ae9127b0-c11d-467b-903d-a84cef43f6ed
    internal-label: Control Panel
  - id: c5474392-5419-4296-9e41-f6f4ce4f6e9b
    internal-label: Administration
subfeature_v2:
  - id: e519a22f-a06a-42fc-9d09-d78a3ab2c434
    internal-label: Monitoring guidelines
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
source-git-commit: b2723b0683a305a992b710a37a3e47927e1fb65e
workflow-type: tm+mt
source-wordcount: '109'
ht-degree: 100%
---
# アクティブなクエリの監視 {#long-running-queries}

「**[!UICONTROL データベース]**」タブの「**[!UICONTROL アクティブなクエリ]**」領域には、選択したインスタンスで最も長く実行されている 5 つのクエリが一覧表示されます。

![](assets/active-queries.png)

「**[!UICONTROL 期間]**」列は、クエリがインスタンス上で実行されている期間を示します。 期間は `hh:mm:ss.ms` の形式で表示されます。

>[!IMPORTANT]
>
>いずれかのクエリが 24 時間以上アクティブな場合は、カスタマーケアに問い合わせて、問題を特定し解決してもらってください。 クエリの一意の ID である **[!UICONTROL PID]** 列の値を伝える必要があります。
