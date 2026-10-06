---
title: 最新リリース
description: このページでは、コントロールパネルのすべての新機能と改善点を一覧表示しています。
feature: Control Panel, Release Notes
role: Admin
level: Experienced
exl-id: 13aceffb-ceaa-4cfe-8741-95d66c5c6caa
TQID: 'https://experienceleague.adobe.com/Q1kU0q1e-a-H0LvAyK-5yYhfrUpGco1hVHWUsz-syhY'
product_v2:
  - id: dfc56824-e8b9-499e-85d4-21aedb507314
    internal-label: Campaign
feature_v2:
  - id: ae9127b0-c11d-467b-903d-a84cef43f6ed
    internal-label: Control Panel
  - id: c5474392-5419-4296-9e41-f6f4ce4f6e9b
    internal-label: Administration
subfeature_v2:
  - id: e5e477db-ebc7-4368-ab0f-4d8fc2aed405
    internal-label: Release notes
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
level_v2:
  - id: d378ca77-2da1-4f39-ad92-1917fe974a38
    internal-label: Experienced
source-git-commit: b2723b0683a305a992b710a37a3e47927e1fb65e
workflow-type: tm+mt
source-wordcount: '150'
ht-degree: 100%
---
# 最新リリース {#control-panel-releases}

このページでは、コントロールパネルの新機能と改善点を一覧表示しています。

## 2023年10月 {#october-2023}

**ユーザーインターフェイス**

* コントロールパネルが追加の言語で使用できるようになりました。 [詳細情報](../discover/using/discovering-the-interface.md#supported-languages-languages)

**アクティブなプロファイルの監視**

* 組織に対して使用権限が付与されているアクティブなプロファイルの数と、複数のインスタンスを使用している場合は、すべてのインスタンス内の組織で使用されているプロファイルの合計数を監視できるようになりました。 [詳細情報](../performance-monitoring/using/active-profiles-monitoring.md)

**DMARC レコード**

* 複数のメールアドレスで集計レポートと失敗レポートのメールを受信できるようになりました。 [詳細情報](../subdomains-certificates/using/dmarc.md)
* サブドメインに DMARC と BIMI の両方のレコードが存在する場合は、次の変更が行われています。

  * DMARC レコードは削除できません。 削除する場合は、まず BIMI レコードを削除する必要があります。
  * DMARC レコードは編集できますが、「なし」へのポリシーのダウングレードは許可されておらず、その割合は 100 にする必要があります。

