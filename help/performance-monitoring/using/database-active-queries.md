---
product: campaign
solution: Campaign
title: アクティブなクエリの監視
description: コントロールパネルで Campaign インスタンス上のアクティブなクエリを監視する方法を説明します。
feature: Control Panel
role: Architect
level: Experienced
source-git-commit: 12e9326ba220776874654705587152bf3978949c
workflow-type: tm+mt
source-wordcount: '123'
ht-degree: 52%

---

# アクティブなクエリの監視 {#long-running-queries}

「**[!UICONTROL データベース]**」タブの「**[!UICONTROL アクティブなクエリ]**」領域には、選択したインスタンスで最も長く実行されている 5 つのクエリが一覧表示されます。

![](assets/active-queries.png)

「**[!UICONTROL 期間]**」列は、クエリがインスタンス上で実行されている期間を示します。期間は `hh:mm:ss.ms` の形式で表示されます。

>[!IMPORTANT]
>
>いずれかのクエリが 24 時間以上アクティブな場合、を購読している場合は E メールで通知されます。 [メールアラート](email-alerting.md).
>
>その場合は、カスタマーケアに問い合わせて、問題を特定して解決してもらってください。 ユーザーに **[!UICONTROL PID]** 列の値。クエリの一意の識別子です。
