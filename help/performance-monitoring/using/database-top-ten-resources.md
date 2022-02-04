---
product: campaign
solution: Campaign
title: 一時的リソース上位 10 位
description: Campaign データベース上のワークフローと配信で生成された一時的リソース上位 10 位をコントロールパネルで監視する方法を説明します。
feature: Control Panel
role: Architect
level: Experienced
exl-id: bb9e1ce3-2472-4bc1-a82a-a301c6bf830e
source-git-commit: 9accc4306bacab3bc27922f495c19138f905b1c5
workflow-type: ht
source-wordcount: '291'
ht-degree: 100%

---

# 一時的リソース上位 10 位 {#top-10}

**[!UICONTROL 一時的リソース上位 10 位]**&#x200B;領域には、ワークフローと配信によって生成された 10 個の最大の一時的リソースがリストされます。

大きな一時的リソースを作成しているワークフローや配信を監視することは、データベースを監視するための重要な手順です。一時的リソースがデータベース容量を消費しすぎる場合は、このワークフローまたは配信が必要であることを確認し、最終的にインスタンスに移動して停止します。

>[!IMPORTANT]
>
>一般的に、非標準リソースが **40 列を超えない**&#x200B;ようにすることが推奨されます。

![](assets/database-top10.png)

>[!NOTE]
>
>ワークフローに多数のテーブルが存在するまたはデータベースサイズが大きい場合は、ワークフローを確認して、大量のデータが生成される理由を調べることをお勧めします。
>
>また、このページの最後には、データベース容量超過を防ぐための Campaign Standard および Campaign Classic のリソースが提供されています。

「**[!UICONTROL すべて表示]**」ボタンを使用すると、これらの一時的リソースの詳細情報にアクセスできます。

![](assets/database-top10-view.png)

「**[!UICONTROL 中間結果を保持]**」列の値は、Campaign でこのオプションが有効（「1」）と無効（「0」）のどちらであるかを示します。このオプションを使用すると、ワークフローの様々なアクティビティ間のトランジションの結果を保存できます（[Campaign Standard](https://experienceleague.adobe.com/docs/campaign-standard/using/managing-processes-and-data/executing-a-workflow/managing-execution-options.html?lang=ja) および [Campaign Classic](https://experienceleague.adobe.com/docs/campaign-classic/using/automating-with-workflows/introduction/workflow-best-practices.html?lang=ja#logs) のドキュメントを参照）。

>[!IMPORTANT]
>
>このオプションは、本番ワークフローでは絶対にオンにしないでください。これは結果の分析に使用され、テスト目的でのみ設計されているので、開発環境またはステージング環境に限定して使用する必要があります。
>
>コントロールパネルの値が、ワークフローの 1 つに対してこのオプションが有効になっていることを示している場合は、Campaign でこのオプションをオフにすることを強くお勧めします。
