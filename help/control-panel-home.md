---
title: 製品ドキュメント
description: コントロールパネルのドキュメント。
feature: Control Panel
role: Architect
level: Beginner
exl-id: 2b2cfaed-e42e-4c3a-a8d8-224b936890ab
source-git-commit: 6a4db9712d3a92d8057758eb134b0178213f5ff8
workflow-type: tm+mt
source-wordcount: '290'
ht-degree: 62%

---

# ヘルプセンター {#control-panel-documentation}

>[!CONTEXTUALHELP]
>id="cp_overview"
>title="コントロールパネルについて"
>abstract="コントロールパネルホームページから、Campaign インスタンスで実行できるすべてのアクションにアクセスできます。"
>additional-url="https://experienceleague.adobe.com/docs/control-panel/using/discover-control-panel/accessing-control-panel.html?lang=ja" text="コントロールパネルへのアクセス"

![](assets/do-not-localize/banner.png)

Campaign コントロールパネルを使用すると、各 Campaign インスタンスの設定を管理したり使用状況を追跡したりできるので、 Campaign Standard および V7／v8 の製品管理者としての作業の効率を向上できます。

## 新機能

**ユーザーインターフェイス**

* Campaign コントロールパネルが追加の言語で利用できるようになりました。 [詳細情報](discover/using/discovering-the-interface.md#supported-languages-languages)

**アクティブなプロファイルの監視**

* 複数のインスタンスを使用している場合に、組織に対して使用可能なアクティブなプロファイルの数、およびすべてのインスタンス内で組織で使用されたプロファイルの総数を監視できるようになりました。 [詳細情報](performance-monitoring/using/active-profiles-monitoring.md)

**DMARC レコード**

* 複数の電子メールアドレスで、集計レポートと失敗レポートの電子メールを受け取れるようになりました。 [詳細情報](subdomains-certificates/using/dmarc.md)
* サブドメインに DMARC と BIMI の両方のレコードが存在する場合は、次の変更が行われています。

   * DMARC レコードは削除できません。 削除する場合は、まず BIMI レコードを削除する必要があります。
   * DMARC レコードは編集できますが、ポリシーを「なし」にダウングレードすることはできません。割合 (%) は 100 にする必要があります。

>[!CAUTION]
>
>* コントロールパネルは、管理者ユーザーに限定されています。[詳細情報](https://experienceleague.adobe.com/docs/control-panel/using/discover-control-panel/managing-permissions.html?lang=ja#discover-control-panel)
>
>* Campaign v7 の場合は、デプロイメントに制限があります。[詳細情報](faq.md#v7-restrictions)

## その他のリソース {#additional-resources}

<table>
    <tr>
        <td><b>Campaign Standard</b><br/>
        <ul>
            <li><a href="https://experienceleague.adobe.com/docs/campaign-standard-learn/control-panel/control-panel-overview.html?lang=ja">コントロールパネルのチュートリアルビデオ</a></li>
            <li><a href="https://experienceleague.adobe.com/docs/campaign-standard/using/campaign-standard-home.html?lang=ja">Campaign Standard 製品ドキュメント</a></li>
        </ul>
        </td>
        <td><b>Campaign v7</b><br/>
        <ul>
            <li><a href="https://experienceleague.adobe.com/docs/campaign-classic-learn/control-panel/control-panel-overview.html?lang=ja">コントロールパネルのチュートリアルビデオ</a></li>
            <li><a href="https://experienceleague.adobe.com/docs/campaign-classic/using/campaign-classic-home.html?lang=ja">Campaign v7 製品ドキュメント</a></li>
        </ul>
        </td>
        <td><b>Campaign v8</b><br/>
        <ul>
            <li><a href="https://experienceleague.adobe.com/docs/campaign-learn/control-panel/control-panel-overview.html?lang=ja">コントロールパネルのチュートリアルビデオ</a></li>
            <li><a href="https://experienceleague.adobe.com/docs/campaign/campaign-v8/campaign-home.html?lang=ja">Campaign v8 製品ドキュメント</a></li>
        </ul>
        </td>
    </tr>
</table>
