---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: ボードでの接続済みカードの使用
description: Workfront の既存のタスクやイシューに接続するカードをボードに追加できます。
author: Lisa
feature: Agile
exl-id: c6d979dd-e4a4-48a5-a91b-b31d7ef848d1
source-git-commit: 246750d2a7a053d74df2ceb150f14fdb50f32ade
workflow-type: tm+mt
source-wordcount: '1447'
ht-degree: 88%

---

# ボードでの接続済みカードの使用

<!-- Audited: 2/2024 -->

[!DNL Workfront] の既存のタスクとイシューに接続するカードをボードに追加できます。

以下の詳細のいずれかが 1 つの場所でカードのために更新されると、自動的に他の場所でも更新されます。

* [!UICONTROL 名前]
* [!UICONTROL 説明]
* [!UICONTROL 割り当て先]
* [!UICONTROL ステータス]
* [!UICONTROL 完了予定日]
* [!UICONTROL 見積もり]／[!UICONTROL ストーリーポイント]
* [!UICONTROL サブタスク]
* [!UICONTROL ドキュメント]

>[!NOTE]
>
>1 つの接続したタスクまたはイシューは、ボードごとに 1 回だけ追加できます。同じタスクまたはイシューを複数のボードに接続できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] プラン</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス</strong></td> 
   <td>
   <p>新規：寄稿者以上</p>
   <p>または</p>
   <p>現在：リクエスト以降</p>
 </td> 
  </tr> 
  <tr>
   <td role="rowheader"><strong>アクセスレベル設定</strong></td>
   <td><p>タスクおよび問題へのアクセス権を表示または高くする</p></td>
  </tr>
  <tr>
   <td role="rowheader"><strong>オブジェクト権限</strong></td>
   <td><p>Workfrontのタスクまたは問題に対する権限を表示またはそれ以上に設定します</p></td>
  </tr>
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 接続されているカードを追加する

1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon.png)をクリックするか、または（使用可能な場合）左上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン![メインメニュー](/help/_includes/assets/main-menu-icon-left-nav.png)をクリックして、「**[!UICONTROL ボード]**」をクリックします。
1. ボードにアクセスします。詳しくは、[ボードを作成または編集](../../agile/get-started-with-boards/create-edit-board.md)を参照してください。
1. **[!UICONTROL カードを追加]／[!UICONTROL 接続されているカード]**&#x200B;をクリックします。
1. プロジェクトを選択し、ボードにカードとして追加するタスクまたはイシューを選択します。

   複数のオブジェクトを選択でき、すべてが個別のカードとして追加されます。

   >[!NOTE]
   >
   >* 検索結果には、自分が権限を持っているオブジェクトのみが表示されます。項目が淡色表示の場合は、その項目は既にボードに追加されています。
   >* **[!UICONTROL 所有プロジェクト]**&#x200B;または&#x200B;**[!UICONTROL 担当プロジェクト]**&#x200B;でフィルターすると、完了、無効、または却下ステータスに相当するプロジェクトは含まれません。**[!UICONTROL すべて]**&#x200B;フィルターを使用して、これらのプロジェクトを検索することもできます。

1. 「**[!UICONTROL 追加]**」をクリックします。

   ![接続するタスクまたはイシューを検索](assets/boards-tasksissues-350x94.png)

   カードが一番左の列の下に追加されます。接続された [!DNL Workfront] オブジェクトとその割り当て先がカードに表示されます。

   ![接続されているカード](assets/boards-connected-card-first-added.png)

1. 「![タスクまたはイシューを開く](assets/boards-launch-icon.png)」をクリックして、[!DNL Workfront] タスクまたはイシューを新しいブラウザータブで開きます。
1. カードの詳細を編集するには、（カード名ではなく）カードをクリックします。

   または

   カード上の&#x200B;**[!UICONTROL その他]**&#x200B;メニュー ![その他メニュー](assets/more-icon-spectrum.png) をクリックし、「**[!UICONTROL 編集]**」を選択します。

1. **[!UICONTROL カードの詳細]**&#x200B;ボックスに、以下の情報を追加または更新します。

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Name]</strong></td> 
      <td>名前を変更すると、接続された [!DNL Workfront] オブジェクトの名前も変更されます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td> 
      <td>説明を変更すると、接続された [!DNL Workfront] オブジェクトの説明も変更されます。説明に URL を追加すると、カードの保存時にクリック可能なリンクになります。</td> 
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Column]</strong></td>
      <td>カードの列を選択します。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Status]</strong></td>
      <td><p>カードのステータスを選択します。デフォルトは [!UICONTROL New]、[!UICONTROL In Progress]、[!UICONTROL Complete] ですが、[!DNL Workfront] で項目に定義されたカスタムステータスも使用できます。</p>
      <p>フィールド値の更新に対して列ポリシーが有効になっている場合、カードのステータスを変更すると、対応する列にカードが自動的に移動します。詳しくは、<a href="/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md" class="MCXref xref">ボード列を管理</a>の記事の「列設定とポリシーを定義」を参照してください。</p>
      <p>カードの上部にある「<strong>[!UICONTROL Mark Complete]</strong>」をクリックすると、ステータスが自動的に完了に変わります。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Planned Completion]</strong></td>
      <td>この日付を変更すると、接続された [!DNL Workfront] オブジェクトの予定完了日も変更されます。</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimation]</strong></td>
      <td><p>カードが完了するまでの時間数。</p><p>見積もりを変更すると、接続された [!DNL Workfront] オブジェクトのストーリーポイントの値も変更されます。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Assignments]</strong></td>
      <td><p>カードに他の人やチームを割り当てるには、 <strong>[!UICONTROL 割り当てを追加 ]</strong> 検索フィールドに名前を入力し始めます。 次に、結果のリストに表示される場合に選択します。 個人とチームの両方を追加できます。1 つの接続されたカードでは、1 つのチーム割り当てのみが許可されます。</p>
      <p>選択した割り当て先は、[!DNL Workfront] でのタスクまたはイシューにも割り当てられます。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Tags]</strong></td>
      <td><p>カードのタグを検索して選択します。</p>
      <p>タグの新規作成について詳しくは、<a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref">タグを追加</a>を参照してください。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom fields]</strong></td>
      <td><p>追加したカスタムフィールドは、このエリアに表示されます。</p>
      <p>詳しくは、<a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">カードに表示するフィールドのカスタマイズ</a>を参照してください。</p></td>
     </tr>
     <tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Subtask]</strong></td>
      <td><p>タスクの既存のサブタスクは、このセクションに表示されます。 クリック <strong>[!UICONTROL サブタスクの追加 ]</strong> をクリックして、新しいサブタスクを追加します。</p>
      <p>セクションの上部にあるカウンターは、完了したサブタスクの数とサブタスクの合計数を示します。</p>
      <p>サブタスクの詳細については、 <a href="/help/quicksilver/agile/get-started-with-boards/manage-subtasks-on-boards.md">ボードでのサブタスクの管理</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL チェックリスト ]</strong></td>
      <td><p>「<strong>[!UICONTROL Add checklist item]</strong>」をクリックします。次に、項目のタイトルを入力し、Enter キーを押します。別の項目が自動的に追加されます。引き続きタイトルを入力して、さらに項目を追加します。</p>
      <p>チェックリストの上部にあるカウンターは、完了した項目の数と合計項目数を示します。</p> <p>チェックリスト項目について詳しくは、<a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md">カードのチェックリスト項目の管理</a>を参照してください。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Documents]</strong></td>
      <td>既存のドキュメントの場合は、ドキュメントのサムネールの上にマウスポインターを置いて、 <strong>プレビュー</strong> ファイルをブラウザーに表示するには、または <strong>ダウンロード</strong> をクリックして、ファイルをコンピューターにダウンロードします。 新しいドキュメントについては、 <a href="/help/quicksilver/agile/get-started-with-boards/add-documents-on-cards.md">カードへのドキュメントの追加</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Hours]</strong></td>
      <td>下記の「接続されたカードでの時間の記録」を参照してください。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Comments]</strong></td>
      <td><p>「<strong>[!UICONTROL New comment]</strong>」フィールド内をクリックして、コメントを入力します。書式設定ツールを使用してテキストの書式を設定し、<strong>添付ファイルを追加</strong>アイコン <img src="assets/attachment-icon.png" alt="添付ファイルアイコン"> をクリックして、コメントにファイルを添付します。ユーザーまたはチームにタグ付けするには、コメントエリアの下部にある検索ボックスを使用します。ユーザーは、ボード上のメンバーである必要はありません。接続されたカードのタグ付きユーザーは、メール通知を受け取ります。</p><p>「<strong>[!UICONTROL Submit]</strong>」をクリックして、コメントをカードに追加します。</p>
      <p><strong>メモ：</strong> カードのコメントエリアでは、Adobe Workfront の新しいコメント機能が使用されます。詳しくは、<a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md">作業の更新</a>を参照してください。</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL System activity]</strong></td> 
      <td><p><strong>システムアクティビティ</strong>をカードセクションとして有効にすると、このエリアにアクティビティが表示されます。</p> <p>詳しくは、<a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">カードに表示するフィールドのカスタマイズ</a>および<a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md">システムトラッキングによるアップデート</a>を参照してください。</p></td>
     </tr>     
    </tbody> 
   </table>

   左のナビゲーションパネルを使用すると、カードの詳細でフィールドのセクション間を移動できます。

1. 「**[!UICONTROL 閉じる]**」をクリックしてボードに戻ります。
接続されたオブジェクト、割り当て先、タグ、期限、チェックリストカウンター、推定時間、ステータスがカードに表示されます。

   ![カードがボードに追加されました](assets/boards-connected-card-details-110922.png)

## 接続されたカードの接続を解除する

接続されたカードを Workfront オブジェクトから解除すると、そのカードは編集可能なアドホックカードとしてボードに残ります。

ボードレベルで接続を解除するには：

1. ボードにアクセスします。
1. 接続されたカードの&#x200B;**[!UICONTROL その他]**&#x200B;メニュー![その他メニュー](assets/more-icon-spectrum.png)をクリックし、**[!UICONTROL 接続解除]**&#x200B;を選択します。
1. 「**[!UICONTROL 接続解除]**」をクリックします。

カードレベルで接続解除するには：

1. ボードにアクセスし、接続されたカードを開きます。
1. カード詳細の接続エリアにある&#x200B;**[!UICONTROL その他]**&#x200B;メニュー![その他メニュー](assets/more-icon-spectrum.png)をクリックし、**[!UICONTROL 接続解除]**&#x200B;を選択します。
1. 確認メッセージで「**[!UICONTROL 接続解除]**」をクリックします。

## アドホックカードを接続済みカードに変換する

作成したアドホックカードを接続されたカードに変換できます。アドホックカードについて詳しくは、[ボードへのアドホックカードの追加](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md)を参照してください。

1. ボードにアクセスし、アドホックカードを開きます。
1. カードの名前と説明を確認します。これらは [!DNL Workfront] で作成したタスクやイシューに追加されます。
1. カードの詳細の[!UICONTROL 接続]エリアで、「**[!UICONTROL Workfront に接続]**」をクリックします。
1. 「[!UICONTROL カードを接続]」ウィンドウで、タスクを作成するかイシューを作成するかを選択します。
1. タスクまたはイシューを追加するプロジェクトを検索して選択します。

   >[!NOTE]
   >
   >* 検索結果には、自分が権限を持っているオブジェクトのみが表示されます。
   >* **[!UICONTROL 所有プロジェクト]**&#x200B;または&#x200B;**[!UICONTROL 担当プロジェクト]**&#x200B;でフィルターすると、「[!UICONTROL 完了]」、「[!UICONTROL 無効]」、または「[!UICONTROL 却下]」ステータスに相当するプロジェクトは含まれません。**[!UICONTROL すべて]**&#x200B;フィルターを使用して、これらのプロジェクトを検索することもできます。

1. 「**[!UICONTROL 接続]**」をクリックします。

   ![アドホックカードを Workfront に接続](assets/boards-connect-ad-hoc-card.png)

   プロジェクト名は、カードの詳細の接続エリアに表示されます。

1. 「**[!UICONTROL 閉じる]**」をクリックしてボードに戻ります。

## 接続されたカードに時間を記録する

接続されたタスクまたはイシューに関する時間を記録するには、適切な権限が必要です。

デフォルトでは、接続されたカードにタイムログフィールドが表示されません。[!UICONTROL カード]の[!UICONTROL 設定]エリアで「[!UICONTROL **時間**]」を有効にする必要があります。詳しくは、「[カードに表示するフィールドのカスタマイズ](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md)」を参照してください。

1. タスクまたはイシューの時間数を入力します。
1. デフォルトと異なる場合は、ドロップダウンメニューから「[!UICONTROL 時間タイプ]」を選択します。
1. 「[!UICONTROL **時間を記録**]」をクリックします。

   ![カードに時間を記録](assets/log-hours-on-card.png)

   カードに記録された時間は、接続されたタスクまたはイシューにも保存されます。

カードに記録する時間は、タスクまたはイシューに記録する時間と同じです。詳しくは、[時間を記録](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md)の記事の「プロジェクト、タスク、またはイシューに時間を記録」を参照してください。

