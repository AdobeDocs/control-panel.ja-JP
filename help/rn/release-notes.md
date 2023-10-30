---
title: 最新リリース
description: このページでは、コントロールパネルのすべての新機能と改善点を一覧表示しています。
feature: Control Panel, Release Notes
role: Admin
level: Experienced
exl-id: 13aceffb-ceaa-4cfe-8741-95d66c5c6caa
source-git-commit: a3485766791387bd9422b4f29daf86296efafb98
workflow-type: tm+mt
source-wordcount: '148'
ht-degree: 26%

---

# 最新リリース {#control-panel-releases}

このページでは、コントロールパネルの新機能と改善点を一覧表示しています。

## 2023年10月 {#october-2023}

**ユーザーインターフェイス**

* Campaign コントロールパネルが追加の言語で利用できるようになりました。 [詳細情報](../discover/using/discovering-the-interface.md#supported-languages-languages)

**アクティブなプロファイルの監視**

* 複数のインスタンスを使用している場合に、組織に対して使用可能なアクティブなプロファイルの数、およびすべてのインスタンス内で組織で使用されたプロファイルの総数を監視できるようになりました。 [詳細情報](../performance-monitoring/using/active-profiles-monitoring.md)

**DMARC レコード**

* 複数の電子メールアドレスで、集計レポートと失敗レポートの電子メールを受け取れるようになりました。 [詳細情報](../subdomains-certificates/using/dmarc.md)
* サブドメインに DMARC と BIMI の両方のレコードが存在する場合は、次の変更が行われています。

   * DMARC レコードは削除できません。 削除する場合は、まず BIMI レコードを削除する必要があります。
   * DMARC レコードは編集できますが、ポリシーを「なし」にダウングレードすることはできません。割合 (%) は 100 にする必要があります。

