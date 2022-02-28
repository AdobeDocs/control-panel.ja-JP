---
product: campaign
solution: Campaign
title: スループットと待ち時間の監視
description: コントロールパネルで Campaign インスタンスのスループットと待ち時間を監視する方法を説明します。
feature: Control Panel
role: Architect
level: Experienced
exl-id: eddef17f-0667-4b43-bc56-2b1aeeae61bb
source-git-commit: 7f7623a747bbc9c3b0816f12195068e04eee9b2f
workflow-type: ht
source-wordcount: '243'
ht-degree: 100%

---

# スループットと待ち時間の監視 {#throughputs-latency-monitoring}

>[!CONTEXTUALHELP]
>id="cp_performancemonitoring_throughputslatencies"
>title="スループットと待ち時間の監視について "
>abstract="このタブでは、インスタンスでの配信スループットと待ち時間の一定期間にわたるトレンドを監視できます。"

インスタンスの使用状況を把握し、良好なパフォーマンスを確保するには、一定期間にわたって配信スループットと待ち時間のトレンドを監視することが不可欠です。

この情報は、**[!UICONTROL パフォーマンス監視]**&#x200B;カード、「**[!UICONTROL スループットと待ち時間]**」タブにある各 Campaign インスタンスのコントロールパネルに表示されます（コントロールパネルは図を表示するのに最大 1 時間かかる場合があります）。

* **[!UICONTROL スループット]**&#x200B;領域には、使用資格のあるすべての通信チャネルについて、選択した Campaign インスタンスから 1 時間に送信されるメッセージの数に関する情報が表示されます。

* **[!UICONTROL 待ち時間]**&#x200B;領域には、リアルタイムトランザクション通信の送信時に、選択したインスタンスで発生した待ち時間に関する情報が表示されます。待ち時間は 95 と 99 のパーセンタイルでキャプチャおよび視覚化されます。つまり、リクエストの 95％と 99％は、指定された待ち時間よりも高速である必要があります。

![](assets/throughput-latencies-overview.png)

>[!NOTE]
>
>この領域に示されているすべての数値は概算であり、情報提供のみを目的としています。

デフォルトでは、現在の日付のデータが表示されます。表示期間は、「**[!UICONTROL 6 か月]**」、「**[!UICONTROL 30 日]**」、「**[!UICONTROL 7 日]**」のボタンを使用して変更できます。

グラフではなく並べ替え可能な列を持つ表形式で、情報を視覚化することもできます。これを行うには、「**[!UICONTROL ビジュアライゼーション設定]**」ボタンをクリックし、「**[!UICONTROL テーブル]**」を選択します。

![](assets/throughput-latencies-table.png)
