---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: コネクタ
navigation-topic: apps-and-their-modules
title: Slackモジュール
description: 内 [!DNL Adobe Workfront Fusion] シナリオの場合、Slackを使用するワークフローを自動化し、複数のサードパーティのアプリケーションやサービスに接続できます。
author: Becky
feature: Workfront Fusion
exl-id: ba5bad6a-3cb3-4024-82f7-d38ee9a8e0b5
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1775'
ht-degree: 1%

---

# [!DNL Slack] モジュール

内 [!DNL Adobe Workfront Fusion] シナリオを使用して、 [!DNL Slack]を使用して、複数のサードパーティのアプリケーションやサービスに接続できます。

シナリオの作成手順については、 [でのシナリオの作成 [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

モジュールについて詳しくは、 [のモジュール [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## アクセス要件

この記事の機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画*</td>
  <td> <p>[!UICONTROL Pro] 以降</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td>
   <td> <p>[!UICONTROL プラン ]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] ライセンス**</td> 
   <td>
   <p>現在のライセンス要件：いいえ [!DNL Workfront Fusion] ライセンス要件。</p>
   <p>または</p>
   <p>従来のライセンス要件：[!UICONTROL [!DNL Workfront Fusion] [ 作業の自動化と統合 ] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>
   <p>現在の製品要件：[!UICONTROL Select] または [!UICONTROL Prime] がある場合 [!DNL Adobe Workfront] プラン（組織で購入する必要がある） [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。 [!DNL Workfront Fusion] は、[!UICONTROL Ultimate] に含まれています [!DNL Workfront] プラン</p>
   <p>または</p>
   <p>従来の製品要件：組織で購入する必要があります [!DNL Adobe Workfront Fusion] 同様に [!DNL Adobe Workfront] を使用して、この記事で説明する機能を使用できます。</p>
   </td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

詳しくは、 [!DNL Adobe Workfront Fusion] ライセンス， 「 [[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## 前提条件

使用する [!DNL Slack] モジュールの場合、 [!DNL Slack] アカウント

## [!DNL Slack] モジュールとそのフィールド

設定時に [!DNL Slack] モジュール [!DNL Workfront Fusion] 以下のフィールドが表示されます。 これらに加えて、 [!DNL Slack] アプリまたはサービスのアクセスレベルなどの要因に応じて、フィールドが表示される場合があります。 モジュール内の太字のタイトルは、必須フィールドを示します。

フィールドまたは関数の上にマップボタンが表示されている場合は、このボタンを使用して、そのフィールドの変数や関数を設定できます。 詳しくは、 [のモジュール間で情報をマッピングする [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [メッセージ](#messages)
* [ファイル](#files)
* [チャネル](#channels)
* [反応](#reactions)
* [星](#stars)
* [保存済み項目](#saved-items)
* [ピン留め](#pins)
* [ユーザー](#users)
* [リマインダー](#reminders)
* [イベント](#events)
* [プロファイル](#profile)
* [その他](#other)

### メッセージ

+++**[!UICONTROL パブリックチャネルメッセージを見る]**

このトリガーモジュールは、新しいメッセージが公開チャネルに追加されると、シナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Slack] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL チャネル ] </td> 
   <td> <p>新しいメッセージを監視するパブリックチャネルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ] </td> 
   <td> <p>メッセージの最大数を設定 [!DNL Workfront Fusion] は、1 回の実行サイクルで返されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++**[!UICONTROL プライベートチャネルメッセージの視聴]**

このトリガーモジュールは、新しいメッセージがプライベートチャネル（グループ）に追加されると、シナリオを開始します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Slack] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL チャネル ] </td> 
   <td> <p>新しいメッセージを監視するプライベートチャネルを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ] </td> 
   <td> <p>メッセージの最大数を設定 [!DNL Workfront Fusion] は、1 回の実行サイクルで返されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

<!--

+++ **[!UICONTROL Watch Direct Messages]**

This trigger module starts the scenario when a new message is added to a direct message.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel] </td> 
   <td> <p>Select the direct message conversation you want to watch for new messages.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Set the maximum number of messages [!DNL Workfront Fusion] will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Watch Multiparty Direct Messages]**

This trigger module starts the scenario when a new message is added to a multiparty direct message channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel] </td> 
   <td> <p>Select the direct message conversation you want to watch for new messages.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Set the maximum number of messages [!DNL Workfront Fusion] will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Search for Message]**

This search module returns messages matching a search query.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query]</td> 
   <td> <p>Enter the query that you want to search by. </p> <p>For information on creating formulas from the mapping panel, see <a href="../../workfront-fusion/functions/map-using-functions.md" class="MCXref xref">Map items using functions in [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Set the maximum number of messages [!DNL Workfront Fusion] will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

-->

+++ **[!UICONTROL プライベートチャネルメッセージの取得]**

このアクションモジュールは、選択したチャネルからメッセージの詳細を取得します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Slack] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Channel ID]</p> </td> 
   <td> <p>チャネル ID を入力（マッピング）します。</p> <p>注意：チャネル ID は、[!UICONTROL リストチャネル ] モジュールを使用して取得できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL メッセージ ID （タイムスタンプ）]</p> </td> 
   <td> <p> 情報を取得するメッセージのメッセージタイムスタンプを入力またはマッピングします。</p> <p>注意：タイムスタンプは、[!UICONTROL 公開チャネルを監視 ] モジュールなど、別のモジュールを使用して取得できます。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL パブリックチャネルメッセージの取得]**

このアクションモジュールは、指定されたパブリックチャネルから指定された ID を持つメッセージを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Slack] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Channel ID]</p> </td> 
   <td> <p>チャネル ID を入力またはマッピングします。</p> <p>注意：チャネル ID は、[!UICONTROL リストチャネル ] モジュールを使用して取得できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メッセージ ID （タイムスタンプ）]</td> 
   <td> <p> 情報を取得するメッセージのメッセージタイムスタンプを入力またはマッピングします。</p> <p>注意：タイムスタンプは、[!UICONTROL 公開チャネルを監視 ] モジュールなど、別のモジュールを使用して取得できます。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

<!--

+++ **[!UICONTROL List replies]**

This action module retrieves a thread of messages posted to a conversation.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that contains the message that you want to retrieve replies for, then select the channel.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Parent message ID (Time stamp)]</td> 
   <td> <p> Enter or map the message time stamp of the message you want to retrieve replies for.</p> <p>Note: The time stamp can be retrieved using another module, such as the [!UICONTROL Watch Public Channel] module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of replies you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

-->

+++ **[!UICONTROL メッセージの作成]**

このアクションモジュールは、新しいメッセージを作成します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Slack] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL チャネル ID または名前を入力 ]</p> </td> 
   <td> <p>メッセージを作成するチャネルの選択方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>内 <strong>[!UICONTROL Channel ID または名前 ]</strong> 「 」フィールドに、メッセージを投稿するチャネルのチャネル ID または名前を入力またはマッピングします。</p> <p>注意：チャネル ID は、[!UICONTROL リストチャネル ] モジュールを使用して取得できます。</p> </li> 
     <li> <p><strong>[!UICONTROL リストから選択 ]</strong> </p> <p>チャネルのタイプを選択し、チャネルを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL テキスト ]</p> </td> 
   <td> <p>作成するメッセージのテキストコンテンツを入力します。</p> <p>注意：テキストの書式設定について詳しくは、 <a href="https://api.slack.com/reference/surfaces/formatting">アプリケーションサーフェスのテキストのフォーマット</a> 内 [!DNL Slack] ドキュメント。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ブロック ]</td> 
   <td>ブロックは、メッセージをカスタマイズおよび整理するために使用できる再利用可能なコンポーネントです。 ブロックの詳細については、 <a href="https://api.slack.com/block-kit">ブロックキット</a> 内 [!DNL Slack] ドキュメント。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL スレッドメッセージ ID （タイムスタンプ）]</td> 
   <td>新しいメッセージが返信の場合は、返信先のメッセージのタイムスタンプを入力します。 既に返信があるメッセージのタイムスタンプを入力しないでください。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 返信ブロードキャスト ]</td> 
   <td> <p>選択 <strong>[!UICONTROL はい ]</strong> 次の両方に該当する場合：</p> 
    <ul> 
     <li> <p>新しいメッセージは別のメッセージへの返信です</p> </li> 
     <li> <p>チャネル内の全員に新しいメッセージを表示する</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL リンク名 ]</p> </td> 
   <td> <p>名前とチャネルの使用を許可するには、このオプションを有効にします <code>@username</code> または <code>#channel</code> 形式 </p> <p>詳しくは、 <a href="https://api.slack.com/docs/formatting">アプリケーションサーフェスのテキストのフォーマット</a> 内 [!DNL Slack] ドキュメント。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL メッセージテキストを解析 ]</p> </td> 
   <td> <p>自動解析を許可するには、このオプションを有効にします。 </p> <p>詳しくは、 <a href="https://api.slack.com/docs/formatting">アプリケーションサーフェスのテキストのフォーマット</a> 内 [!DNL Slack] ドキュメント。</p> <p>注意：元のメッセージで [!UICONTROL リンク名 ] または [!UICONTROL メッセージテキストを解析 ] オプションを使用した場合は、[!UICONTROL メッセージの更新 ] モジュールの実行時にも指定する必要があります。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Markdown を使用 ]</p> </td> 
   <td> <p>このオプションを有効にして許可 [!DNL Slack] を使用して、テキスト内で markdown を使用します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL 主にテキストベースのコンテンツを展開する</p> </td> 
   <td> <p>主にテキストベースのコンテンツをアンフールする場合に、このオプションを有効にします。 </p> <p>でのファーリングの解除の詳細 [!DNL Slack]を参照してください。 <a href="https://api.slack.com/reference/messaging/link-unfurling">メッセージ内のリンクのアンフル</a> 内 [!DNL Slack] ドキュメント。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL メディアコンテンツを展開 ]</p> </td> 
   <td> <p>メディアコンテンツのアンフルを許可するには、このオプションを有効にします。 </p> <p>でのファーリングの解除の詳細 [!DNL Slack]を参照してください。 <a href="https://api.slack.com/reference/messaging/link-unfurling">メッセージ内のリンクのアンフル</a> 内 [!DNL Slack] ドキュメント。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL メッセージの更新]**

このアクションモジュールを使用すると、既存のメッセージを編集できます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Slack] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL チャネル ID または名前を入力 ]</p> </td> 
   <td> <p>メッセージの選択方法を選択します。</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL 手動で入力 ]</strong> </p> <p>内 <strong>[!UICONTROL Channel ID または名前 ]</strong> 「 」フィールドに、メッセージが含まれているチャネル ID またはチャネルのチャネル ID を入力またはマッピングしてから、 <strong>[!UICONTROL タイムスタンプ（メッセージ ID）]</strong> メッセージの.</p> <p>注意：チャネル ID は、[!UICONTROL リストチャネル ] モジュールを使用して取得できます。</p> </li> 
     <li> <p><strong>[!UICONTROL リストから選択 ]</strong> </p> <p>チャネルのタイプを選択し、チャネルを選択して、メッセージを選択します。</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL テキスト ]</p> </td> 
   <td> <p>更新するメッセージの新しいテキストコンテンツを入力します。</p> <p>詳しくは、 <a href="https://api.slack.com/docs/formatting">アプリケーションサーフェスのテキストのフォーマット</a> 内 [!DNL Slack] ドキュメント。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ブロック ]</td> 
   <td>ブロックは、メッセージをカスタマイズおよび整理するために使用できる再利用可能なコンポーネントです。 ブロックの詳細については、 <a href="https://api.slack.com/block-kit">ブロックキット</a> 内 [!DNL Slack] ドキュメント。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL リンク名 ]</p> </td> 
   <td> <p>名前とチャネルの使用を許可するには、このオプションを有効にします <code>@username</code> または <code>#channel</code> 形式 </p> <p>詳しくは、 <a href="https://api.slack.com/docs/formatting">アプリケーションサーフェスのテキストのフォーマット</a> 内 [!DNL Slack] ドキュメント。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL メッセージテキストを解析 ]</p> </td> 
   <td> <p>自動解析を許可するには、このオプションを有効にします。 </p> <p> 詳しくは、 <a href="https://api.slack.com/docs/formatting">アプリケーションサーフェスのテキストのフォーマット</a> 内 [!DNL Slack] ドキュメント。</p> <p>注意：元のメッセージで [!UICONTROL リンク名 ] または [!UICONTROL メッセージテキストを解析 ] オプションを使用した場合は、メッセージの更新モジュールの実行時にも指定する必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL メッセージの削除]**

このアクションモジュールは、指定されたメッセージを削除します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Slack] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Channel ID]</p> </td> 
   <td> <p>チャネル ID を入力またはマッピングします。</p> <p>注意：チャネル ID は、[!UICONTROL リストチャネル ] モジュールを使用して取得できます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メッセージ ID]</td> 
   <td> <p> 削除するメッセージのタイムスタンプを入力またはマッピングします。</p> <p>注意：タイムスタンプは、Watch Private Channel Module など、別のモジュールを使用して取得できます。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

<!--

### Files 

+++ **[!UICONTROL Watch Files]**

This trigger module starts a scenario when a new file is added.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type]</td> 
   <td>Select the type of file that you want the module to watch.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td> <p>Select the type of channel you want to watch for files, then select the channel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Enter or map the maximum number of files you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL List Files]**

This action module returns a list of files based on the specified filter.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Type] </td> 
   <td> <p>Select the type(s) of files you want to retrieve.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Channel type]</p> </td> 
   <td> <p>Select the type of channel representing the channel that you want to list files from, then select the channel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Created by]</td> 
   <td> <p>Select a user to return only files created by that user.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Date from]</td> 
   <td>Enter the earliest date that you want to return files from. For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Type coercion in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Date to]</td> 
   <td>Enter the latest date that you want to return files from. For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Type coercion in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Enter or map the maximum number of files you want the module to return during each scenario execution cycle.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Get a File]**

This action module returns details about the specified file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td> <p>Enter or map the ID of the file that you want to retrieve. </p> <p>Note: The file ID can be retrieved using another module, such as the [!DNL Watch Files] Module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Download a File]**

This action module downloads a file from a URL. It must follow the [!UICONTROL Slack] >[!UICONTROL Get a File] module in a scenario.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL private download]</td> 
   <td> <p>Map the <b>[!UICONTROL URL Private download]</b> value from the [!DNL Slack] >[!UICONTROL Get a File] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Upload a File]**

This action module creates or uploads a file to [!DNL Slack]

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channels]</td> 
   <td> <p>For each channel you want to upload the file to, click <b>[!UICONTROL Add item]</b>, then select the channel type and channel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title]</td> 
   <td>Enter a title for the file you want to upload</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Thread ID (timestamp)]</td> 
   <td> <p>If you are uploading the file as a reply, enter or map the time stamp of the message you want to reply to.</p> <p>Note: The time stamp can be retrieved using another module, such as the [!UICONTROL Watch Private Channel] module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Initial Comment]</td> 
   <td> <p>Enter or map the text of the message that introduces the file.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Create a Text File]**

This action module creates a text file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channels]</td> 
   <td> <p>For each channel you want to upload the file to, click <b>[!UICONTROL Add item]</b>, then select the channel type and channel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file]</td> 
   <td>Select a source file from a previous module, or map the source file's name and data.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Title]</td> 
   <td>Enter a title for the file you want to upload</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Thread ID (timestamp)]</td> 
   <td> <p>If you are uploading the file as a reply, enter or map the time stamp of the message you want to reply to.</p> <p>Note: The time stamp can be retrieved using another module, such as the[!UICONTROL  Watch Private Channel] module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Initial Comment]</td> 
   <td> <p>Enter or map the text of the message that introduces the file.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Delete a File]**

This action module returns deletes the specified file.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td> <p>Enter or map the ID of the file that you want to delete. </p> <p>Note: The file ID can be retrieved using another module, such as the [!DNL Watch Files] Module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

-->

### チャネル

+++ **[!UICONTROL チャネルのリスト]**

この検索モジュールは、ワークスペース内のすべてのチャネルのリストを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Slack] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL アーカイブ済みを除外 ]</p> </td> 
   <td> <p>「 [!UICONTROL はい ] 」を選択して、結果のアーカイブ済みチャネルを除外します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL の種類 ] </td> 
   <td> <p>取得するチャネルのタイプを選択します。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ] </td> 
   <td> <p>チャネルの最大数を設定する [!DNL Workfront Fusion] は、1 回の実行サイクルで返されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL チャネルの取得]**

このアクションモジュールは、Workspace チャネルに関する情報を返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Slack] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Channel ID]</p> </td> 
   <td> <p>情報を取得するチャネルの ID を入力またはマッピングします。</p> <p>注意：チャネル ID は、[!UICONTROL リストチャネル ] モジュールを使用して取得できます。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL チャネル内のメンバーのリスト]**

この検索モジュールは、選択したチャネルのユーザーのリストを返します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Slack] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL チャネルタイプ ]</td> 
   <td>リストするメンバーのリストを含むチャネルのタイプを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 公開 ] / [!UICONTROL 非公開チャネル ]</td> 
   <td>メンバーのリストを表示するチャネルを選択します。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 制限 ] </td> 
   <td> <p>メンバーの最大数を設定 [!DNL Workfront Fusion] は、1 回の実行サイクルで返されます。</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

<!--

+++ **[!UICONTROL Set the Topic of a Channel]**

This action module changes the topic of a channel

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want to change the topic for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL Multiple IM Channel] / [!UICONTROL User]</td> 
   <td>Select the channel or user that you want to change the topic for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Topic]</td> 
   <td>Enter or map the new topic of the channel. This field does not support formatting or links.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Set the Purpose of a Channel]**

This action module changes the purpose of a channel

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want to change the purpose for.</td> 
  </tr> 
  <tr> 
>[!MORELIKETHIS]
>
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL Multiple IM Channel] / User</td> 

   <td>Select the channel or user that you want to change the purpose for.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Purpose]</td> 
   <td>Enter or map the new purpose of the channel. This field does not support formatting or links.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Join a Channel]**

This action module joins the user to a channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Channel ID]</p> </td> 
   <td> <p>Enter or map the ID of the channel that you want to join.</p> <p>Note: The Channel ID can be retrieved using the [!UICONTROL List Channels] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Leave a Channel]**

This action module removes the user from a channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Channel ID]</p> </td> 
   <td> <p>Enter or map the ID of the channel that you want to leave.</p> <p>Note: The Channel ID can be retrieved using the [!UICONTROL List Channels] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Create a Channel]**

This action module creates a new channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Name]</p> </td> 
   <td> <p>Enter or map a name for the new channel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Is private]</td> 
   <td>Enable this option to set the new channel as private.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Archive a Channel]**

This action module archives a  channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Channel ID]</p> </td> 
   <td> <p>Enter or map the ID of the channel that you want to archive.</p> <p>Note: The Channel ID can be retrieved using the [!UICONTROL List Channels] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Unarchive a Channel]**

This action module unarchives a channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Channel ID]</p> </td> 
   <td> <p>Enter or map the ID of the channel that you want to unarchive.</p> <p>Note: The Channel ID can be retrieved using the [!UICONTROL List Channels] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Reactions

+++ **[!UICONTROL List reactions]**

This action module returns reactions that a user made.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL User]</p> </td> 
   <td> <p>Select the user that made the reactions that you want to list.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Enter or map the maximum number of reactions you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Add a reaction]**

This action module adds a reaction to an item.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want to add a reaction to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL Multiple IM channel] / [!UICONTROL User]</td> 
   <td>Select the channel or user that you want to add a reaction to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Enter or map the time stamp of the message you want to add a reaction to.</p> <p>Note: The time stamp can be retrieved using another module, such as the [!UICONTROL Watch Private Channel] module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reaction (emoji) name]</td> 
   <td>Enter or map the name of the emoji that you want to use for a reaction. Example: <code>thumbsup</code>. </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Remove a reaction]**

This action module adds a reaction to an item.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want to remove a reaction from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL Multiple IM channel] / [!UICONTROL User]</td> 
   <td>Select the channel or user that you want to add a reaction from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Enter or map the time stamp of the message you want to add a reaction to.</p> <p>Note: The time stamp can be retrieved using another module, such as the [!UICONTROL Watch Private Channel] module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Reaction (emoji) name]</td> 
   <td>Enter or map the name of the emoji that you want to remove from the message. Example: <code>thumbsup</code>. </td> 
  </tr> 
 </tbody> 
</table>

+++

### Stars 

+++ **[!UICONTROL Add a star]**

This action module makes a channel a starred channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want to add a star to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL IM] / [!UICONTROL Multiple IM channel]</td> 
   <td>Select the channel or user that you want to add a star to.</td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Remove a star]**

This action module removed the star from a starred channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want to add a star to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL IM] / [!UICONTROL Multiple IM channel]</td> 
   <td>Select the channel or user that you want to add a star to.</td> 
  </tr> 
 </tbody> 
</table>

+++

### Saved Items

+++ **[!UICONTROL Save an Item]**

This action module adds an item to saved items.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID (Time stamp)]</td> 
   <td> <p> Enter or map the time stamp of the message you want to save.</p> <p>Note: The time stamp can be retrieved using another module, such as the [!UICONTROL Watch Private Channel] module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td> <p>Enter or map the file that you want to save.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Remove Saved Item]**

This action module adds an item to saved items.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID (Time stamp)]</td> 
   <td> <p> Enter or map the time stamp of the message you want to remove from saved items.</p> <p>Note: The time stamp can be retrieved using another module, such as the [!UICONTROL Watch Private Channel] module.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File ID]</td> 
   <td> <p>Enter or map the file you want to remove from saved items.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Pins

+++ **[!UICONTROL Pin an Item]**

This action module pins an item, such as a file or file comment, to a channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want to pin an item to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL Multiple IM channel] / [!UICONTROL User]</td> 
   <td>Select the channel or user that you want to pin an item to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Enter or map the time stamp of the message you want to pin.</p> <p>Note: The time stamp can be retrieved using another module, such as the [!UICONTROL Watch Private Channel] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Unpin an Item]**

This action module unpins an item from a channel. You can unpin files, file comments, channel messages, or group messages.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want to unpin an item from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL Multiple IM channel] / [!UICONTROL User]</td> 
   <td>Select the channel or user that you want to unpin an item from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Message ID]</td> 
   <td> <p> Enter or map the time stamp of the message you want to unpin.</p> <p>Note: The time stamp can be retrieved using another module, such as the [!UICONTROL Watch Private Channel] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Users 

+++ **[!UICONTROL Watch Users]**

This trigger module starts the scenario when a new user is added to the [!DNL Slack] workspace.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Set the maximum number of users [!DNL Workfront Fusion] will return during one execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Search for User]**

This action module retrieves details about a single user, by using their email address.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Email] </p> </td> 
   <td> <p>Enter or map the email address of the user you want to retrieve details about.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL List Users]**

This action module returns a list of all users in a workspace.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Limit]</p> </td> 
   <td> <p>Enter or map the maximum number of users you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Get a User]**

This action module retrieves details about a member of a workspace.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL User ID]</p> </td> 
   <td> <p>Enter or map the User ID of the user you want to retrieve details for.</p> <p>Note: The User ID can be retrieved using another module, such as the [!DNL List Users] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Invite Users]**

This action module invites 1-30 users to a public or private channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want invite users to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private] / [!UICONTROL Multiple IM channel] / [!UICONTROL User]</td> 
   <td>Select the channel or user that you want to invite users to.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Users]</td> 
   <td> <p>Select the users that you want to add to the channel.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Kick a User]**

This action module removes a user from a channel.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Channel type]</td> 
   <td>Select the type of channel that you want remove a user from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Public] / [!UICONTROL Private channel]</td> 
   <td>Select the channel that you want to remove a user from.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Users]</td> 
   <td> <p>Select the user that you want to remove from the channel.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Reminders

+++ **[!UICONTROL List Reminders]**

This action module returns a list of all reminders created by or given to the currently authenticated user.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Limit]</p> </td> 
   <td> <p>Enter or map the maximum number of reminders you want the module to return during each scenario execution cycle.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Get a Reminder]**

This action module retrieves details about a specific reminder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Reminder ID]</p> </td> 
   <td> <p>Enter or map the Reminder ID of the reminder you want to retrieve details for.</p> <p>Note: The Reminder ID can be retrieved using another module, such as the [!UICONTROL List Reminders] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Create a Reminder]**

This action module creates a reminder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Text]</td> 
   <td>Enter or map the content of the reminder</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Time]</td> 
   <td> <p>Enter or map the date and time when this reminder should happen. Enter one of the following: </p> 
    <ul> 
     <li> <p>The Unix timestamp (up to five years from now)</p> </li> 
     <li> <p>The number of seconds until the reminder (if within 24 hours) </p> </li> 
     <li> <p>A natural language description (Examples: "in 15 minutes" or "every Thursday")</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL User] </p> </td> 
   <td> <p>Select the user that receives the reminder.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Complete a Reminder]**

This action module completes a specific reminder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Reminder ID]</p> </td> 
   <td> <p>Enter or map the Reminder ID of the reminder you want to complete.</p> <p>Note: The Reminder ID can be retrieved using another module, such as the [!UICONTROL List Reminders] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Delete a Reminder]**

This action module deletes a specific reminder.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Reminder ID]</p> </td> 
   <td> <p>Enter or map the Reminder ID of the reminder you want to delete.</p> <p>Note: The Reminder ID can be retrieved using another module, such as the [!UICONTROL List Reminders] module.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Events

+++ **[!UICONTROL New Event]**

This instant trigger starts a scenario when a new message or other event is created.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Webhook]</p> </td> 
   <td> <p>Select the webhook you want to use.</p> <p>Or</p> <p>Create a new webhook.</p> 
    <ol> 
     <li value="1"> <p>Click <b>[!UICONTROL Add]</b>.</p> </li> 
     <li value="2"> <p>Select the event type.</p> </li> 
     <li value="3"> <p>Select or add a connection. For instructions about connecting your [!DNL Slack] account to [!UICONTROL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!UICONTROL Adobe Workfront Fusion] - Basic instructions</a></p> </li> 
     <li value="4"> <p>If prompted, select the channel that you want to watch.</p> </li> 
     <li value="5"> <p>Click <b>[!UICONTROL Save]</b> to save the webhook and return to the module.</p> </li> 
    </ol> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Profile

+++ **[!UICONTROL Set a status]**

This action module updates a user's current status.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>For instructions about connecting your [!DNL Slack] account to [!DNL Workfront Fusion], see <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Create a connection to [!DNL Adobe Workfront Fusion] - Basic instructions</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Status text]</p> </td> 
   <td> <p>Enter or map the status text. Consider the following:</p> 
    <ul> 
     <li> <p>You can enter up to 100 characters.</p> </li> 
     <li> <p>You can use markup or other formatting, such as user mentions.</p> </li> 
     <li> <p>You can include emojis in the status text by using the format <code>:emojiname:</code>.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status Emoji]</td> 
   <td> <p>Enter or map the emoji that you want to use to represent your status. Use the format <code>:emojiname:</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Status expiration]</td> 
   <td>Enter or map the date and time you want the status to expire. For a list of supported date and time formats, see <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref" data-mc-variable-override="">Type coercion in [!DNL Adobe Workfront Fusion]</a>.</td> 
  </tr> 
 </tbody> 
</table>

+++

-->

### その他

+++ **[!UICONTROL API 呼び出しを実行する]**

このアクションモジュールを使用すると、 [!DNL Slack] API これにより、他のユーザーが達成できないデータフローの自動化を作成できます [!DNL Slack] モジュール。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL 接続 ] </td> 
   <td> <p>接続方法 [!DNL Slack] アカウント [!DNL Workfront Fusion]を参照してください。 <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">への接続の作成 [!DNL Adobe Workfront Fusion]  — 基本手順</a></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>相対パスを入力 <code>https://slack.com/api/</code>. 例: <code>/users/identity</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL メソッド ]</td> 
   td&gt; <p>API 呼び出しを設定する必要がある HTTP リクエストメソッドを選択します。 詳しくは、 <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">の HTTP リクエストメソッド [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>標準の JSON オブジェクトの形式でリクエストのヘッダーを追加します。</p> <p>以下に例を挙げます。 <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] によって認証ヘッダーが追加されます。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL クエリ文字列 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しのクエリを追加します。</p> <p>例： <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL 本文 ]</td> 
   <td> <p>標準の JSON オブジェクトの形式で、API 呼び出しの本文のコンテンツを追加します。</p> <p>メモ:  <p>条件文 ( <code>if</code> JSON で、条件文の外側に引用符を置きます。</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ベース URL]</td> 
   <td>API 呼び出しに使用するベース URL を選択します。</td> 
  </tr> 
 </tbody> 
</table>

+++

## 用語

次の用語は、 [!DNL Slack] モジュール：

* **DM**: [!UICONTROL ダイレクトメッセージ]
* **IM**: [!UICONTROL インスタントメッセージ]
* **プライベートチャネル**:former [!UICONTROL グループ]
* **ダイレクトメッセージ**:former [!UICONTROL IM]
* **チャネル**: [!UICONTROL 会話] （API ドキュメント内） [!UICONTROL チャネル] 内 [!DNL Slack] アプリを使用します。