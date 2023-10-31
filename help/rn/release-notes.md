---
title: 最新リリース
description: このページでは、コントロールパネルのすべての新機能と改善点を一覧表示しています。
feature: Control Panel, Release Notes
role: Admin
level: Experienced
exl-id: 13aceffb-ceaa-4cfe-8741-95d66c5c6caa
source-git-commit: a3485766791387bd9422b4f29daf86296efafb98
workflow-type: ht
source-wordcount: '148'
ht-degree: 100%

---

# 最新リリース {#control-panel-releases}

このページでは、コントロールパネルの新機能と改善点を一覧表示しています。

## 2023年10月 {#october-2023}

**ユーザーインターフェイス**

* コントロールパネルが追加の言語で使用できるようになりました。[詳細情報](../discover/using/discovering-the-interface.md#supported-languages-languages)

**アクティブなプロファイルの監視**

* 組織に対して使用権限が付与されているアクティブなプロファイルの数と、複数のインスタンスを使用している場合は、すべてのインスタンス内の組織で使用されているプロファイルの合計数を監視できるようになりました。[詳細情報](../performance-monitoring/using/active-profiles-monitoring.md)

**DMARC レコード**

* 複数のメールアドレスで集計レポートと失敗レポートのメールを受信できるようになりました。[詳細情報](../subdomains-certificates/using/dmarc.md)
* サブドメインに DMARC と BIMI の両方のレコードが存在する場合は、次の変更が行われています。

   * DMARC レコードは削除できません。削除する場合は、まず BIMI レコードを削除する必要があります。
   * DMARC レコードは編集できますが、「なし」へのポリシーのダウングレードは許可されておらず、その割合は 100 にする必要があります。

