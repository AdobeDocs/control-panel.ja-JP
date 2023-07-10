---
title: リリースノート 2023
description: このページでは、コントロールパネルの 2023年リリースをすべて掲載しています。
exl-id: 9a83e32a-4c11-4784-a6fe-341ce9ebc7a7
source-git-commit: 40654418f0c5b298cc4fbd66a5d835355876a12c
workflow-type: tm+mt
source-wordcount: '242'
ht-degree: 100%

---

# リリースノート 2023 {#rn-2023}

## 2023年5月の改善点 {#june-2023}

**アドビへのサブドメインの SSL 証明書のデリゲーション**

サブドメインの SSL 証明書をアドビで管理できるようになりました。CNAME を使用してサブドメインを設定している場合、ドメインホスティングソリューションに証明書を生成するために、証明書レコードが自動的に生成および提供されます。

この機能は、新しいサブドメインを設定する場合にのみ使用できます。 既存のデリゲートされたサブドメインの証明書はデリゲートできません。[詳細情報](../subdomains-certificates/using/setting-up-new-subdomain.md)

>[!NOTE]
>
>アドビ管理の SSL は、ユーザーが無料で使用できる機能です。

## 2023年3月 {#march-2023}

**CNAME のサブドメインデリゲーションの削除**

CNAME を使用して設定されたサブドメインのデリゲーションを削除できるようになりました。[詳細情報](../subdomains-certificates/using/remove-delegated-subdomains.md)

## 2023年2月 {#february-2023}

**アドビにデリゲートされたサブドメインのデリゲーションの削除**

アドビに完全にデリゲートされたサブドメインのデリゲーションを削除できるようになりました。[詳細情報](../subdomains-certificates/using/remove-delegated-subdomains.md)

>[!NOTE]
>
>現在、デリゲーションの削除は、CNAME を使用して設定されたサブドメインでは使用できません。

**サービスカレンダー**

お使いのインスタンスで発生する重要なイベントを追跡するためのカレンダー表示がサービスカレンダーに追加されました。さらに、コントロールパネルのアラートを購読しているユーザーに送信される通知に関する情報が追加されました。[詳細情報](../service-events/service-events.md)

![](assets/do-not-localize/gif-calendar.gif)

## 2023年1月 {#january-2023}

**新しいハイブリッドホスティングモデル機能**

ハイブリッドホスティングモデルを使用しているお客様は、MID インスタンスにアクセスするための許可リストに IP アドレスを追加できるようになりました。[詳細情報](../instances-settings/using/ip-allow-listing-instance-access.md)

**証明書署名リクエスト（CSR）の機能強化**

証明書署名リクエストの生成時に、市区町村フィールドがオプションになりました。
