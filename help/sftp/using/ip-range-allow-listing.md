---
title: IP 範囲許可リストへの登録
description: SFTPサーバーがアクセスできるように許可リストにIP範囲を追加する方法を説明します
translation-type: tm+mt
source-git-commit: d96c044e83d37f020b5fd6ea55199c1223b9fa39
workflow-type: tm+mt
source-wordcount: '615'
ht-degree: 47%

---


# IP 範囲許可リストへの登録 {#ip-range-allow-listing}

>[!CONTEXTUALHELP]
>id="cp_ip_whitelist"
>title="IP 許可リストへの登録について"
>abstract="このタブでは、SFTPサーバーへの接続を確立するために、許可リストにIP範囲を追加できます。 アクセス権のある SFTP サーバーのみがここに表示されます。他の SFTP サーバーへのアクセス権をリクエストするには、管理者にお問い合わせください。"
>additional-url="https://images-tv.adobe.com/mpcv3/8a977e03-d76c-44d3-853c-95d0b799c870_1560205338.1920x1080at3000_h264.mp4#t=98" text="デモビデオを見る"

SFTP サーバーは保護されています。表示ファイルにアクセスしたり、新しいファイルを書き込んだりするには、サーバにアクセスするシステムまたはクライアントのパブリックIPアドレスを許可リストに追加する必要があります。

## CIDR 形式について{#about-cidr-format}

CIDR（Classless Inter-Domain Routing）は、コントロールパネルのインターフェイスで IP 範囲を追加する際にサポートされる形式です。

構文は、IP アドレスとそれに続く「/」（スラッシュ記号）および 10 進数で構成されます。形式とその構文について詳しくは、[この記事](https://whatismyipaddress.com/cidr)を参照してください。

管理している IP 範囲を CIDR 形式に変換するのに役立つ無料のオンラインツールをインターネットで検索できます。

## ベストプラクティス{#best-practices}

コントロールパネルで IP アドレスを許可リストに登録する場合は、必ず以下の推奨事項と制限に従ってください。

* **IP追加範囲は、単一のIPアドレスではなく、許可リスト** 。 1つのIPアドレスを許可リストに追加するには、「/32」を追加して、範囲に含めるIPアドレスが1つだけであることを示します。
* **> 265のIPアドレスなど**、許可リストにあまり広い範囲を追加しないでください。 コントロールパネルは、/0 ～ /23 の間の CIDR 形式の範囲を拒否します。
* 許可リストに追加できるのは **パブリックIPアドレス** のみです。
* 不要になったIPアドレスは **定期的に許可リストから削除し** 、

## 許可リストへのIPアドレスの追加 {#adding-ip-addresses-allow-list}

>[!CONTEXTUALHELP]
>id="cp_sftp_iprange_add"
>title="新しい IP 範囲の追加"
>abstract="SFTPサーバーに接続するために許可リストに追加するIP範囲を定義します。"

許可リストにIP範囲を追加するには、次の手順に従います。

1. **[!UICONTROL SFTP]** カードを開き、「 **[!UICONTROL IP Allow Listing]** 」タブを選択します。
1. 許可リスト上のIPアドレスのリストが、各インスタンスに対して表示されます。 左側のリストから目的のインスタンスを選択して、「**[!UICONTROL 新しい IP 範囲を追加]**」ボタンをクリックします。

   ![](assets/control_panel_add_range.png)

1. 許可リストに追加するIP範囲をCIDR形式で定義し、リストに表示するラベルを定義します。

   >[!NOTE]
   >
   >「ラベル」フィールドでは、以下の特殊文字を使用できます。
   > `. _ - : / ( ) # , @ [ ] + = & ; { } ! $`

   ![](assets/control_panel_add_range2.png)

   >[!IMPORTANT]
   >
   >IP範囲は、許可リスト上の既存の範囲と重複できません。 重複する場合は、まず、重複している IP を含む範囲を削除してください。
   >
   >複数のインスタンスに対して、許可リストに範囲を追加できます。 それには、下向き矢印キーを押すか目的のインスタンスの最初の文字を入力して、候補リストから選択します。

   ![](assets/control_panel_add_range3.png)

1. 「**[!UICONTROL 保存]**」ボタンをクリックします。要求が完全に処理されるまで、許可リストにIPを追加すると、「保留」と表示されます。 これにかかるのは、わずか数秒です。

許可リストから IP 範囲を削除するには、IP 範囲を選択して、**[!UICONTROL 「IP 範囲を削除]**」ボタンをクリックします。

![](assets/control_panel_delete_range2.png)

>[!NOTE]
>
>現在、許可リスト上の範囲を編集できません。 IP 範囲を変更するには、不要な IP 範囲を削除してから、必要な IP 範囲を新しく作成します。

## 変更の監視{#monitoring-changes}

The **[!UICONTROL Job Logs]** in the Control Panel home page let you monitor all changes that have been made to IP addresses on the allow list.

コントロールパネルのインターフェイスについて詳しくは、[この節](../../discover/using/discovering-the-interface.md)を参照してください。

![](assets/control_panel_ip_log.png)