---
title: IPホワイトリスト
description: コントロールパネルでのインスタンスアクセスに関するIPホワイトリストの詳細
translation-type: tm+mt
source-git-commit: 8ee999b89af88a1a59956838d5722ce8fc6b3955

---


# IP whitelisting {#ip-whitelisting}

>[!CAUTION]
>
>この機能は、Campaign Classicインスタンスでのみ使用できます。

## IP のホワイトリスト登録について {#about-ip-whitelisting}

デフォルトでは、Adobe Campaign Classicインスタンスは様々なIPアドレスからアクセスできません。

お使いの IP アドレスがホワイトリストに登録されていない場合は、そのアドレスからインスタンスにログインすることはできません。同様に、IPアドレスがインスタンスに対して明示的にホワイトリストに登録されていない場合、APIをMessage Centerまたはマーケティングインスタンスに接続できない可能性があります。

コントロールパネルでは、IP アドレスの範囲をホワイトリストに登録することで、インスタンスへの新しい接続をセットアップできます。それには、次の手順に従います。

IP アドレスがいったんホワイトリストに登録されれば、Campaign オペレーターを作成して IP アドレスにリンクできます。その結果、ユーザーがインスタンスにアクセスできるようになります。

## ベストプラクティス {#best-practices}

コントロールパネルで IP アドレスをホワイトリストに登録する場合は、必ず以下の推奨事項と制限に従ってください。

* IP アドレスから RT サーバーまたは AEM セキュリティゾーンに接続しない場合は、**すべてのアクセスタイプで IP アクセスを無効にします**。
* **IPアドレスに対するインスタンスへのアクセスを一時的に有効にした場合**、インスタンスに接続する必要がなくなったら、ホワイトリストに登録されたIPアドレスからIPアドレスを削除してください。
* **公共の場所** （空港、ホテルなど）のIPアドレスをホワイトリストに登録しないことをお勧めします。 インスタンスのセキュリティを常に確保するには、会社の VPN アドレスを使用してください。

## インスタンスにアクセスするための IP アドレスのホワイトリスト登録 {#whistelisting-ip-addresses}

IPアドレスをホワイトリストに登録するには、次の手順に従います。

1. **[!UICONTROL 「インスタンス設定」カード]**&#x200B;を開いて「IP ホワイトリスト」タブにアクセスし、「**[!UICONTROL 新しい IP 範囲を追加]**」をクリックします。

   >[!NOTE]
   >
   >インスタンス設定カードが、コントロールパネルのホームページに表示されない場合、お使いの IMS ORG ID は、Adobe Campaign Classic インスタンスに関連付けられていません。

   ![](assets/ip_whitelist_list1.png)

1. ホワイトリストに登録する IP 範囲の情報を次のように入力します。

   ![](assets/ip_whitelist_add1.png)

   * **[!UICONTROL インスタンス]**:IPアドレスが接続できるインスタンス。 複数のインスタンスを同時に操作できます。例えば、プロダクションインスタンスとステージインスタンスの IP ホワイトリスト登録を同じ手順で実行できます。
   * **[!UICONTROL IP範囲]**:ホワイトリストにするIP範囲（CIDR形式）。 なお、IP 範囲は、ホワイトリストに登録されている既存の範囲と重複できません。重複する場合は、まず、重複している IP を含む範囲を削除してください。
   >[!NOTE]
   >
   >CIDR（Classless Inter-Domain Routing）は、コントロールパネルのインターフェイスで IP 範囲を追加する場合にサポートされる形式です。構文は、IP アドレスとそれに続く「/」（スラッシュ記号）および 10 進数で構成されます。形式とその構文について詳しくは、[この記事](https://whatismyipaddress.com/cidr)を参照してください。
   >
   >管理している IP 範囲を CIDR 形式に変換するのに役立つ無料のオンラインツールをインターネットで検索できます。

   * **!UICONTROL ラベル]**:ホワイトリストに登録されたIPアドレスの一覧に表示するラベルです。
   * **[!UICONTROL 名前]**:この名前は、アクセスタイプ、インスタンス（外部API接続の場合）およびIPアドレスに対して一意である必要があります。


1. IPアドレスに付与するアクセスの種類を指定します。

   * **[!UICONTROL キャンペーンコンソールアクセス]**:IPアドレスは、Campaign Classicコンソールに接続できます。 なお、コンソールアクセスはマーケティングインスタンスの場合にのみ有効です。MID および RT インスタンスへのアクセスは許可されないので、無効です。
   * **[!UICONTROL AEM接続]**:指定したAEM IPアドレスは、マーケティングインスタンスへの接続を許可されます。
   * **[!UICONTROL 外部API接続]**:指定したIPアドレスを持つ外部APIは、マーケティングおよびメッセージセンター(RT)インスタンスに接続できます。 なお、RT インスタンスのコンソールへの接続は無効です。
   ![](assets/ip_whitelist_acesstype.png)

1. 「**[!UICONTROL 保存]」ボタンをクリックします。**&#x200B;ホワイトリストに登録されている IP アドレスのリストに指定の IP 範囲が追加されます。

   ![](assets/ip_whitelist_added.png)

To delete whitelisted IP ranges, select them then click the **[!UICONTROL Delete IP range]** button.

**関連トピック：**
* [IP ホワイトリスト登録（チュートリアルビデオ）](https://docs.adobe.com/content/help/en/campaign-learn/campaign-classic-tutorials/administrating/control-panel-acc/ip-whitelisting.html)
* [セキュリティゾーンとオペレーターとのリンク](https://docs.campaign.adobe.com/doc/AC/en/INS_Additional_configurations_Configuring_Campaign_server.html#Linking_a_security_zone_to_an_operator)
