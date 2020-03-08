---
title: IP のホワイトリスト登録
description: インスタンスにアクセスするためのコントロールパネルでの IP アドレスのホワイトリスト登録の詳細
translation-type: tm+mt
source-git-commit: f22e356b283ee2601c948d5c1d514a9a59c58451

---


# IP のホワイトリスト登録{#ip-whitelisting}

>[!CONTEXTUALHELP]
>id=&quot;cp_instancesettings_iprange&quot;
>title=&quot;IPホワイトリストについて&quot;
>abstract=&quot;IPホワイトリストを管理してインスタンスにアクセスします。&quot;
>additional-url=&quot;https://images-tv.adobe.com/mpcv3/045cac99-f948-478e-ae04-f8c161dcb9e2_1568132508.1920x1080at3000_h264.mp4&quot; text=&quot;デモビデオを見る&quot;

>[!CAUTION]
>
>この機能は、Campaign Classic インスタンスでのみ使用できます。

## IP のホワイトリスト登録について{#about-ip-whitelisting}

デフォルトでは、様々な IP アドレスからAdobe Campaign Classic インスタンスにアクセスできるわけではありません。

お使いの IP アドレスがホワイトリストに登録されていない場合は、そのアドレスからインスタンスにログインすることはできません。同様に、お使いの Message Center インスタンスまたはマーケティングインスタンスのホワイトリストに IP アドレスが明示的に登録されていない場合、そのインスタンスに API を接続できません。

コントロールパネルでは、IP アドレスの範囲をホワイトリストに登録することで、インスタンスへの新しい接続をセットアップできます。それには、次の手順に従います。

IP アドレスがいったんホワイトリストに登録されれば、Campaign オペレーターを作成して IP アドレスにリンクできます。その結果、ユーザーがインスタンスにアクセスできるようになります。

## ベストプラクティス{#best-practices}

コントロールパネルで IP アドレスをホワイトリストに登録する場合は、必ず以下の推奨事項と制限に従ってください。

* RT サーバーまたは AEM セキュリティゾーンに接続する予定のない IP アドレスでは、**すべてのアクセスタイプへの IP アクセスを有効にしないでください**。
* **IP アドレスからのインスタンスへのアクセスを一時的に有効にした場合**、インスタンスへ接続する必要がなくなり次第、ホワイトリストに登録されている IP アドレスからその IP アドレスを必ず削除します。
* **公共の場所（空港やホテルなど）の IP アドレスをホワイトリストに登録することはお勧めしません**。インスタンスのセキュリティを常に確保するには、会社の VPN アドレスを使用してください。

## インスタンスにアクセスするための IP アドレスのホワイトリスト登録{#whistelisting-ip-addresses}

>[!CONTEXTUALHELP]
>id=&quot;cp_instancesettings_iprange_add&quot;
>title=&quot;Add New Ip Range&quot;
>abstract=&quot;インスタンスに接続するホワイトリストのIP範囲を定義します。&quot;

IP アドレスをホワイトリストに登録するには、次の手順に従います。

1. を開いて「IPホワ **[!UICONTROL Instances Settings card]** イトリスト」タブにアクセスし、をクリックしま **[!UICONTROL Add new IP Range]**&#x200B;す。

   >[!NOTE]
   >
   >「インスタンス設定」カードがコントロールパネルのホームページに表示されない場合、お使いの IMS ORG ID は、Adobe Campaign Classic インスタンスに関連付けられていません。

   ![](assets/ip_whitelist_list1.png)

1. ホワイトリストに登録する IP 範囲の情報を次のように入力します。

   ![](assets/ip_whitelist_add1.png)

   * **[!UICONTROL Instance(s)]**:IPアドレスが接続できるインスタンス。 複数のインスタンスを同時に操作できます。例えば、プロダクションインスタンスとステージインスタンスの IP ホワイトリスト登録を同じ手順で実行できます。
   * **[!UICONTROL IP Range]**:ホワイトリストにするIP範囲（CIDR形式）。 なお、IP 範囲は、既存のホワイトリストに登録された範囲と重複できません。重複する場合は、まず、重複している IP を含む範囲を削除してください。
   >[!NOTE]
   >
   >CIDR（Classless Inter-Domain Routing）は、コントロールパネルのインターフェイスで IP 範囲を追加する際にサポートされる形式です。構文は、IP アドレスとそれに続く「/」（スラッシュ記号）および 10 進数で構成されます。形式とその構文について詳しくは、[この記事](https://whatismyipaddress.com/cidr)を参照してください。
   >
   >管理している IP 範囲を CIDR 形式に変換するのに役立つ無料のオンラインツールをインターネットで検索できます。

   * **[!UICONTROL Label]**:ホワイトリストに登録されたIPアドレスの一覧に表示するラベルです。
   * **[!UICONTROL Name]**:この名前は、アクセスタイプ、インスタンス（外部API接続の場合）およびIPアドレスに対して一意である必要があります。


1. IP アドレスに許可するアクセスのタイプを指定します。

   * **[!UICONTROL Campaign Console Access]**:IPアドレスは、Campaign Classicコンソールに接続できます。 なお、コンソールアクセスはマーケティングインスタンスの場合にのみ有効です。MID および RT インスタンスへのアクセスは許可されないので、無効です。
   * **[!UICONTROL AEM connection]**:指定したAEM IPアドレスは、Marketingインスタンスへの接続を許可されます。
   * **[!UICONTROL External API connection]**:指定したIPアドレスを持つ外部APIは、マーケティングまたはMessage Center(RT)インスタンスに接続できます。 なお、RT インスタンスのコンソールへの接続は無効です。
   ![](assets/ip_whitelist_acesstype.png)

1. ボタンをクリッ **[!UICONTROL Save]** クします。 指定の IP 範囲がホワイトリストに登録された IP アドレスのリストに追加されます。

   ![](assets/ip_whitelist_added.png)

To delete whitelisted IP ranges, select them then click the **[!UICONTROL Delete IP range]** button.

**関連トピック：**
* [IP ホワイトリスト登録（チュートリアルビデオ）](https://docs.adobe.com/content/help/en/campaign-learn/campaign-classic-tutorials/administrating/control-panel-acc/ip-whitelisting.html)
* [セキュリティゾーンとオペレーターとのリンク](https://docs.campaign.adobe.com/doc/AC/en/INS_Additional_configurations_Configuring_Campaign_server.html#Linking_a_security_zone_to_an_operator)
