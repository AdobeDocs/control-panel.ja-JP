---
title: インスタンスの詳細
description: コントロールパネルでのインスタンスの詳細の監視方法
translation-type: ht
source-git-commit: a2c19296894ff893987290cb287dc7002ab999e5

---


# インスタンスの詳細{#instance-details}

>[!CONTEXTUALHELP]
>id="cp_instancesettings_instancedetails"
>title="[!CONTEXTUALHELP]
>id=&quot;cp_instancesettings_instancedetails&quot;
>title=&quot;インスタンスの詳細について&quot;
>abstract=&quot;Adobe Campaign インスタンスの詳細（タイプ、名前、ビルド情報および利用可能な推奨アップグレード）を表示します。&quot;
>additional-url=&quot;https://docs.adobe.com/content/help/ja-JP/campaign-classic/using/release-notes/latest-release.html&quot; text=&quot;Campaign Classic リリースノート&quot;
>additional-url=&quot;https://docs.adobe.com/content/help/ja-JP/campaign-standard/using/release-notes/release-notes.html&quot; text=&quot;Campaign Standard リリースノート&quot;"
>abstract="[!IMPORTANT]"
>additional-url="この機能は、Campaign Classic インスタンスでのみ使用できます。" text="インスタンスの詳細について{#about-instance-details}"
>additional-url="Adobe Campaign Classic インスタンスアーキテクチャには複数のサーバーを含めることができるので、柔軟なマーケティング活動が可能になります。例えば、マーケティングサーバー、リアルタイム（Message Center）サーバー、ミッドソーシングサーバーでインスタンスをサポートすることができます。" text="「インスタンスの詳細」機能を利用すると、インスタンスのフラットアーキテクチャを表示できます。サーバー情報が得られるほか、インスタンスのビルドが最新かどうかもわかります。さらに、必要に応じてアップグレードも提案されます。"

>[!NOTE]
>
>パフォーマンスの低下を避け、Adobe Campaign Classic から提供される最新の機能や修正を活用できるようにするため、少なくとも年に 1 回はインスタンスをアップグレードすることをお勧めします。

## **関連トピック：**

[ビルドアップグレードの実行[#$tu14]



>
>
>



* 
* 

## 左側のパネルから目的の Campaign Classic インスタンスを選択します。{#retrieving-information-about-instances}

[!NOTE]

1. 左側のパネルのリストには、すべての Campaign インスタンスが表示されます。「インスタンスの詳細」機能は、Campaign Classic インスタンス専用です。Campaign Standard インスタンスを選択すると、「適用外のインスタンス」というメッセージが表示されます。********

   >[!NOTE]インスタンスに接続しているサーバーが表示されます。
   >
   >![](assets/instance_details.png)

1. 入手できる情報は次のとおりです。

   >**[!UICONTROL タイプ]**：サーバーのタイプ。値は MKT（マーケティング）、MID（ミッドソーシング）、RT（Message Center / リアルタイムメッセージング）のいずれかです。
   >
   >**[!UICONTROL 名前]**：サーバーの名前。

1. **[!UICONTROL ビルド：]**&#x200B;サーバーにインストールされているビルドバージョン。

   **[!UICONTROL アップグレード情報]**：サーバーの更新が必要かどうかを示します。

緑：サーバーは最新です。アップグレードは必要ありません。

* **[!UICONTROL 黄：アップグレードを検討する必要があります。最新の機能や修正を利用できません。]**
* **[!UICONTROL 赤：できるだけ早くアップグレードする必要があります。最新の機能を利用できないほか、サーバーのパフォーマンスが最適でない可能性があります。]**
* サーバーのいずれかをアップグレードする必要がある場合は、[こちらのドキュメント[#$tu36]を参照して、作業方法の詳細を確認してください。]**
* 
   * 
   * 
   * 

If one of your servers requires to be upgraded, refer to [this documentation-ERR:REF-NOT-FOUND- for more details on how to proceed.

## Common questions {#common-questions}

**I do not see the MID server on my instance architecture, does it mean my instances are not functioning correctly? Do I need the RT instance for something I am not able to do today?**

Your own instance can look very different, and it may not have all types of servers, or it can have several of the same server. Not having one type of the server or another does not mean you cannot send a real-time message or perform other kinds of activities. You can request additional server capacity, additional fees will apply.

Please contact Customer Care if you believe some servers are not showing in the &quot;Instance Details&quot; page. Make sure you note the specific instance URL in your message.
