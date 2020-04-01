---
title: IP 範囲のホワイトリスト登録
description: SFTP サーバーにアクセスするための IP 範囲のホワイトリスト登録方法
translation-type: tm+mt
source-git-commit: a2c19296894ff893987290cb287dc7002ab999e5

---


# IP 範囲のホワイトリスト登録 {#ip-range-whitelisting}

>[!CONTEXTUALHELP]
>id=&quot;cp_ip_whitelist&quot;
>title=&quot;IP のホワイトリスト登録について&quot;
>abstract=&quot;このタブでは、SFTP サーバーへの接続を確立するための IP 範囲をホワイトリストに登録できます。アクセス権のある SFTP サーバーのみがここに表示されます。他の SFTP サーバーへのアクセス権をリクエストするには、管理者にお問い合わせください。&quot;
>additional-url=&quot;https://images-tv.adobe.com/mpcv3/8a977e03-d76c-44d3-853c-95d0b799c870_1560205338.1920x1080at3000_h264.mp4#t=98&quot; text=&quot;デモビデオを見る&quot;

SFTP サーバーは保護されています。ファイルを表示したり新しいファイルを書き込んだりするために SFTP サーバーにアクセスするには、サーバーにアクセスするシステムまたはクライアントのパブリック IP アドレスをホワイトリストに登録する必要があります。

## CIDR 形式について{#about-cidr-format}

CIDR（Classless Inter-Domain Routing）は、コントロールパネルのインターフェイスで IP 範囲を追加する際にサポートされる形式です。

構文は、IP アドレスとそれに続く「/」（スラッシュ記号）および 10 進数で構成されます。形式とその構文について詳しくは、[この記事](https://whatismyipaddress.com/cidr)を参照してください。

管理している IP 範囲を CIDR 形式に変換するのに役立つ無料のオンラインツールをインターネットで検索できます。

## ベストプラクティス{#best-practices}

コントロールパネルで IP アドレスをホワイトリストに登録する場合は、必ず以下の推奨事項と制限に従ってください。

* **単一の IP アドレスではなく、IP 範囲**&#x200B;をホワイトリストに登録します。単一の IP アドレスをホワイトリストに登録するには、その範囲が単一の IP のみを含むことを示すために「/32」を追加します。
* **ホワイトリストに登録する範囲を広げすぎないようにします**（例えば 265 件を超える IP アドレスは多すぎます）。コントロールパネルは、/0 ～ /23 の間の CIDR 形式の範囲を拒否します。
* ホワイトリストに登録できるのは、**パブリック IP アドレス**&#x200B;のみです。
* 必要なくなった **IP アドレスは定期的にホワイトリストから削除**&#x200B;します。

## IP アドレスのホワイトリスト登録{#whitelisting-ip-addresses}

>[!CONTEXTUALHELP]
>id=&quot;cp_sftp_iprange_add&quot;
>title=&quot;新しい IP 範囲の追加&quot;
>abstract=&quot;SFTP サーバーに接続するためにホワイトリストに登録したい IP 範囲を定義します。&quot;

IP 範囲をホワイトリストに登録するには、次の手順に従います。

1. カードを **[!UICONTROL SFTP]** 開き、タブを選択し **[!UICONTROL IP Whistelisting]** ます。
1. 各インスタンスについて、ホワイトリストに登録された IP アドレスのリストが表示されます。Select the desired instance from the left-hand side list, then click the **[!UICONTROL Add new IP range]** button.

   ![](assets/control_panel_add_range.png)

1. ホワイトリストに登録する IP 範囲を CIDR 形式で定義してから、リストに表示されるラベルを定義します。

   >[!NOTE]
   >
   >「ラベル」フィールドでは、以下の特殊文字を使用できます。
   > `. _ - : / ( ) # , @ [ ] + = & ; { } ! $`

   ![](assets/control_panel_add_range2.png)

   >[!IMPORTANT]
   >
   >IP 範囲は、既存のホワイトリストに登録された範囲と重複できません。重複する場合は、まず、重複している IP を含む範囲を削除してください。
   >
   >複数のインスタンスを対象に同じ範囲をホワイトリストに登録することができます。それには、下向き矢印キーを押すか目的のインスタンスの最初の文字を入力して、候補リストから選択します。

   ![](assets/control_panel_add_range3.png)

1. ボタンをクリッ **[!UICONTROL Save]** クします。 IP のホワイトリストへの追加は、リクエストが完全に処理されるまで、保留中として表示されます。これにかかるのは、わずか数秒です。

To delete whitelisted IP ranges, select them then click the **[!UICONTROL Delete IP range]** button.

![](assets/control_panel_delete_range2.png)

>[!NOTE]
>
>現在のところ、ホワイトリストに登録されている範囲を編集することはできません。IP 範囲を変更するには、不要な IP 範囲を削除してから、必要な IP 範囲を新しく作成します。

## 変更の監視{#monitoring-changes}

The **[!UICONTROL Job Logs]** in the Control Panel home page let you monitor all changes that have been made to whitelisted IP addresses.

コントロールパネルのインターフェイスについて詳しくは、[この節](../../discover/using/discovering-the-interface.md)を参照してください。

![](assets/control_panel_ip_log.png)
