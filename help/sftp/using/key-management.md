---
product: campaign
solution: Campaign
title: 鍵の管理
description: SFTP サーバーに接続するための鍵の管理方法
feature: Control Panel
role: Architect
level: Experienced
exl-id: 03815e01-6371-4e1c-b4b8-7abe25957cee
source-git-commit: 99861c898c216d2589f23bd52779db328ea47256
workflow-type: tm+mt
source-wordcount: '1081'
ht-degree: 35%

---

# キーの管理 {#key-management}

>[!CONTEXTUALHELP]
>id="cp_key_management"
>title="公開鍵管理について"
>abstract="このタブで、公開鍵を作成、管理および編集します。"
>additional-url="https://images-tv.adobe.com/mpcv3/8a977e03-d76c-44d3-853c-95d0b799c870_1560205338.1920x1080at3000_h264.mp4#t=166" text="デモビデオを見る"

アドビでは、すべての顧客が&#x200B;**公開鍵と秘密鍵のペア**&#x200B;を使用して SFTP サーバーへの接続を確立することを推奨します。

SFTP サーバーにアクセスするために SSH 公開鍵を生成して追加する手順および認証に関する推奨事項を以下に説明します。

サーバーへのアクセスを設定したら、忘れずにサーバーにアクセスする必要がある **** IP アドレスを許可リストに登録して、サーバーに接続できるようにしてください。詳しくは、[この節](../../instances-settings/using/ip-allow-listing-instance-access.md)を参照してください。

![](assets/do-not-localize/how-to-video.png) [Campaign Classic](https://experienceleague.adobe.com/docs/campaign-classic-learn/control-panel/sftp-management/generate-ssh-key.html#sftp-management) または [Campaign Standard ](https://experienceleague.adobe.com/docs/campaign-standard-learn/control-panel/sftp-management/generate-ssh-key.html#sftp-management) を使用してこの機能をビデオで確認する

## ベストプラクティス {#best-practices}

**SSH 公開鍵について**

必ず、常に同じ認証を使用してサーバーに接続し、対応する形式の鍵を使用してください。

**ユーザー名とパスワードによる API 統合**

ごくまれに、一部の SFTP サーバーでパスワードベースの認証が有効になっています。 Adobeでは、より効率的で安全な、キーベースの認証を使用することをお勧めします。 キーベースの認証への切り替えをリクエストするには、カスタマーケアに問い合わせます。

>[!IMPORTANT]
>
>パスワードの期限が切れると、システムに鍵がインストールされていても、SFTP アカウントにログインできなくなります。

## SSH 鍵のインストール {#installing-ssh-key}

>[!CONTEXTUALHELP]
>id="cp_sftp_publickey_add"
>title="公開鍵の追加"
>abstract="インスタンスの SSH 公開鍵を生成し、SFTP サーバーにアクセスするためにCampaign コントロールパネルに追加します。"

>[!IMPORTANT]
>
>SSH 鍵に関する組織のガイドラインに従う必要があります。 以下の手順は、SSH 鍵の作成方法の一例です。要件をチームまたは内部ネットワークグループに伝える際の参考資料として役立ちます。

1. 「**[!UICONTROL 鍵管理]**」タブに移動し、「**[!UICONTROL 新しい公開鍵を追加]**」ボタンをクリックします。

   ![](assets/key0.png)

1. 開いたダイアログボックスで、公開鍵を作成するユーザー名および鍵を有効にするサーバーを選択します。

   ![](assets/key1.png)

   >[!NOTE]
   >
   >Campaign コントロールパネルは、特定のユーザー名が特定のインスタンスでアクティブかどうかを確認し、1 つまたは複数のインスタンスでキーをアクティブにできるようにします。
   >
   >各ユーザーには 1 つ以上の SSH 公開鍵を追加できます。

1. 公開鍵をより適切に管理するには、各鍵が使用可能になる期間を設定します。 それには、**[!UICONTROL タイプ]** ドロップダウンリストで単位を選択し、対応するフィールドで期間を定義します。 公開鍵の有効期限について詳しくは、[ この節 ](#expiry) を参照してください。

   ![](assets/key_expiry.png)

   >[!NOTE]
   >
   >デフォルトでは、**[!UICONTROL 型]** フィールドは **[!UICONTROL 無制限]** に設定されています。これは、公開鍵の有効期限が無期限になることを意味します。

1. 「**[!UICONTROL コメント]**」フィールドに、この公開鍵を追加する理由（なぜ誰に対してかなど）を入力できます。

1. 「**[!UICONTROL 公開鍵]**」フィールドに入力するには、SSH 公開鍵を生成する必要があります。 ご使用のオペレーティングシステムに応じて、次の手順に従います。

   **Linux および Mac の場合：**

   ターミナルを使用して公開鍵と秘密鍵のペアを生成します。
   1. コマンド `ssh-keygen -m pem -t rsa -b 2048 -C "your_email@example.com"` を入力します。
   1. プロンプトが表示されたら、鍵に名前を付けます。.ssh ディレクトリが存在しない場合は、システムによって作成されます。
   1. プロンプトが表示されたら、パスフレーズを入力し、もう一度入力します。空欄のままにすることもできます。
   1. 「name」および「name.pub」の鍵のペアがシステムによって作成されます。「name.pub」ファイルを検索して開きます。指定した電子メールアドレスで終わる英数字の文字列が含まれているはずです。

   **Windows の場合：**

   秘密鍵と公開鍵のペアを同じ「name.pub」形式で生成するのに役立つ、サードパーティのツールをインストールする必要が生じる場合があります。

1. .pub ファイルを開き、「ssh...」で始まる文字列全体をコントロールパネルにコピー＆ペーストします。

   ![](assets/publickey.png)

   >[!NOTE]
   >
   >**[!UICONTROL 「公開鍵]**」フィールドは、OpenSSH 形式のみを受け入れます。 SSH 公開鍵のサイズは、**2048 ビット**&#x200B;である必要があります。

1. 「**[!UICONTROL 保存]**」ボタンをクリックして、鍵を作成します。Campaign コントロールパネルは、SHA256 形式で暗号化された公開鍵とそれに関連するフィンガープリントを保存します。

>[!IMPORTANT]
>
>作成したキーを使用して、選択した SFTP サーバーに接続したことのないシステムとの接続を確立する場合、SFTP サーバーでこのシステムを使用する前に、そのシステムのパブリック IP を許可リストに追加する必要があります。 詳しくは、[この節](ip-range-allow-listing.md)を参照してください。

フィンガープリントを使用して、コンピューターに保存されている秘密鍵と、Campaign コントロールパネルに保存されている対応する公開鍵を照合できます。

![](assets/fingerprint_compare.png)

「**...**」ボタンをクリックすると、既存の鍵を削除したり、関連付けられているフィンガープリントをクリップボードにコピーできます。

![](assets/key_options.png)

## 公開鍵の管理 {#managing-public-keys}

作成した公開鍵は「**[!UICONTROL 鍵管理]**」タブに表示されます。

作成日または編集日、作成または編集したユーザー、IP 範囲の有効期限に基づいて項目を並べ替えることができます。

また、名前やコメントの入力を開始して、公開鍵を検索することもできます。

![](assets/control_panel_key_management_sort.png)

1 つ以上の IP 範囲を編集するには、[ この節 ](#editing-public-keys) を参照してください。

リストから 1 つ以上の公開鍵を削除するには、公開鍵を選択し、「**[!UICONTROL 公開鍵を削除]**」ボタンをクリックします。

![](assets/control_panel_delete_key.png)

### 有効期限 {#expiry}

**[!UICONTROL Expires]** 列には、公開鍵の有効期限が切れるまでの残り日数が表示されます。

[ 電子メールアラート ](../../performance-monitoring/using/email-alerting.md) を購読すると、公開鍵の有効期限が切れる 10 日と 5 日前、および期限が切れる日に、電子メールで通知を受け取ります。 アラートを受け取ったら、[ 公開鍵 ](#editing-public-keys) を編集して、必要に応じて有効期間を延長できます。

有効期限切れの公開鍵は、7 日後に自動的に削除されます。 **[!UICONTROL 有効期限]** 列に **[!UICONTROL 期限切れ]** と表示されます。 この 7 日間以内：

* 期限切れの公開鍵を SFTP サーバーへの接続に使用することはできなくなりました。

* 有効期限切れの公開鍵を [ 編集 ](#editing-public-keys) し、その期間を更新して再び使用可能にすることができます。

* リストから削除できます。

## 公開鍵の編集 {#editing-public-keys}

>[!CONTEXTUALHELP]
>id="cp_sftp_publickey_update"
>title="公開鍵の編集"
>abstract="選択した公開鍵を更新して、SFTP サーバーにアクセスします。"

公開鍵を編集するには、次の手順に従います。

>[!NOTE]
>
>編集できるのは、2021 年 10 月のリリース以降に作成された公開Campaign コントロールパネルのみです。

1. **[!UICONTROL キー管理]** リストから 1 つ以上の項目を選択します。
1. 「**[!UICONTROL 公開鍵を更新]**」ボタンをクリックします。

   ![](assets/control_panel_edit_key.png)

1. 編集できるのは、公開鍵の有効期限を編集したり、新しいコメントを追加したりするだけです。

   >[!NOTE]
   >
   >ユーザー名、インスタンス、公開鍵を OpenSSH 形式で変更するには、公開鍵を削除し、必要に応じて新しく作成します。

1. 変更を保存します。
