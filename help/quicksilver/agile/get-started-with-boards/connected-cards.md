---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: ボードでの接続済みカードの使用
description: Workfrontの既存のタスクやイシューに関連するカードをボードに追加できます。
author: Lisa
feature: Agile
exl-id: c6d979dd-e4a4-48a5-a91b-b31d7ef848d1
source-git-commit: 99e985642fff751ac67a9de562908bd2156b3812
workflow-type: tm+mt
source-wordcount: '1427'
ht-degree: 0%

---

# ボードでの接続済みカードの使用

{{preview-and-fast-release}}

既存のタスクとイシューに関連するカードをボードに追加できます。 [!DNL Workfront].

ある場所のカードについて、次のいずれかの詳細が更新されると、別の場所で自動的に更新されます。

* [!UICONTROL 名前]
* [!UICONTROL 説明]
* [!UICONTROL 割り当て先]
* [!UICONTROL ステータス]
* [!UICONTROL 完了予定日]
* [!UICONTROL 推定] / [!UICONTROL ストーリーポイント]
* <span class="preview">[!UICONTROL サブタスク]</span>
* <span class="preview">[!UICONTROL ドキュメント]</span>

>[!NOTE]
>
>1 つの接続されたタスクまたはイシューは、ボードごとに 1 回だけ追加できます。 同じタスクまたは問題を複数のボードに接続できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計画*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL リクエスト ] 以降</p> </td> 
  </tr> 
  <tr>
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td>
   <td><p>[!UICONTROL 表示 ] 以降のタスクおよび問題へのアクセス権</p></td>
  </tr>
  <tr>
   <td role="rowheader"><strong>オブジェクトの権限</strong></td>
   <td><p>Workfrontタスクまたはイシューに対する [!UICONTROL 表示 ] 以上の権限</p></td>
  </tr>
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## 接続されたカードを追加

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **[!UICONTROL ボード]**.
1. ボードにアクセスします。 詳しくは、 [ボードの作成または編集](../../agile/get-started-with-boards/create-edit-board.md).
1. クリック **[!UICONTROL カードを追加] > [!UICONTROL 接続済みカード]**.
1. プロジェクトを選択し、ボードにカードとして追加するタスクまたはイシューを選択します。

   複数のオブジェクトを選択でき、すべてが個別のカードとして追加されます。

   >[!NOTE]
   >
   >* サーチ結果には、自分が権限を持っているオブジェクトのみが表示されます。 項目が淡色表示の場合は、その項目は既にボードに追加されています。
   >* 次の条件でフィルターする場合： **[!UICONTROL 自分が所有するプロジェクト]** または **[!UICONTROL 自分がいるプロジェクト]**、「完了」、「無効」または「却下」のステータスに等しいプロジェクトは含まれません。 これらのプロジェクトは、引き続き **[!UICONTROL すべて]** フィルター。

1. クリック **[!UICONTROL 追加]**.

   ![接続するタスクまたはイシューを検索します](assets/boards-tasksissues-350x94.png)

   カードが一番左の列の下に追加されます。 接続された [!DNL Workfront] オブジェクトとその割り当て先がカードに表示されます。

   ![接続されているカード](assets/boards-connected-card-first-added.png)

1. クリック ![タスクまたは問題を開く](assets/boards-launch-icon.png) 開く [!DNL Workfront] 新しいブラウザータブのタスクまたはイシュー。
1. カードの詳細を編集するには、（カード名ではなく）カードをクリックします。

   または

   次をクリック： **[!UICONTROL その他]** メニュー ![その他のメニュー](assets/more-icon-spectrum.png) を選択し、 **[!UICONTROL 編集]**.

1. Adobe Analytics の **[!UICONTROL カードの詳細]** ボックスで、次の情報を追加または更新します。

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 名前 ]</strong></td> 
      <td>名前を変更すると、接続されたの名前も変更されます [!DNL Workfront] オブジェクト。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL 説明 ]</strong></td> 
      <td>説明を変更すると、接続されているの説明も変更されます [!DNL Workfront] オブジェクト。 説明に URL を追加すると、カードを保存する際にクリック可能なリンクになります。</td> 
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 列 ]</strong></td>
      <td>カードの列を選択します。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL ステータス ]</strong></td>
      <td><p>カードのステータスを選択します。 デフォルトは [!UICONTROL 新規 ]、[!UICONTROL In Progress]、[!UICONTROL Complete] ですが、 [!DNL Workfront] は、も使用できます。</p>
      <p>フィールド値の更新が有効な列ポリシーがある場合、カードのステータスを変更すると、カードは対応する列に自動的に移動します。 詳しくは、この記事の「列設定とポリシーの定義」を参照してください <a href="/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md" class="MCXref xref">ボード列を管理</a>.</p>
      <p>次をクリックした場合： <strong>[!UICONTROL 完了をマーク ]</strong> カードの上部にあるステータスは、自動的に「完了」に変わります。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 計画完了 ]</strong></td>
      <td>この日付を変更すると、接続された [!DNL Workfront] オブジェクト。</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>[!UICONTROL 推定 ]</strong></td>
      <td><p>カードが完了するまでの時間数。</p><p>見積もりを変更すると、接続されたストーリーポイントの値も変更されます [!DNL Workfront] オブジェクト。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 割り当て ]</strong></td>
      <td><p>カードに他の人やチームを割り当てるには、 <strong>[!UICONTROL 割り当てを追加 ]</strong> 検索フィールドに名前を入力し始めます。 次に、結果のリストに表示される場合に選択します。 個人とチームの両方を追加できます。 1 つの接続されたカードでは、1 つのチーム割り当てのみが許可されます。</p>
      <p>選択した担当者も、 [!DNL Workfront].</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL タグ ]</strong></td>
      <td><p>カードのタグを検索して選択します。</p>
      <p>新しいタグの作成について詳しくは、 <a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref">タグを追加</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL カスタムフィールド ]</strong></td>
      <td><p>追加したカスタムフィールドは、この領域に表示されます。</p>
      <p>詳しくは、 <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">カードに表示するフィールドのカスタマイズ</a>.</p></td>
     </tr>
     <tr>
     <tr>
      <td role="rowheader"><span class="preview"><strong>[!UICONTROL サブタスク ]</strong></span></td>
      <td><span class="preview"><p>タスクの既存のサブタスクは、このセクションに表示されます。 クリック <strong>[!UICONTROL サブタスクの追加 ]</strong> をクリックして、新しいサブタスクを追加します。</p>
      <p>セクションの上部にあるカウンターは、完了したサブタスクの数とサブタスクの合計数を示します。</p>
      <p>サブタスクの詳細については、 <a href="/help/quicksilver/agile/get-started-with-boards/manage-subtasks-on-boards.md">ボードでのサブタスクの管理</a>.</p></span></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL チェックリスト ]</strong></td>
      <td><p>クリック <strong>[!UICONTROL チェックリスト項目を追加 ]</strong>. 次に、項目のタイトルを入力し、Enter キーを押します。 別の項目が自動的に追加されます。 引き続きタイトルを入力して、さらに項目を追加します。</p>
      <p>チェックリストの上部にあるカウンターは、完了した項目の数と合計項目数を示します。</p> <p>チェックリスト項目の詳細については、「 <a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md">カードのチェックリスト項目を管理</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><span class="preview"><strong>[!UICONTROL ドキュメント ]</strong></span></td>
      <td><span class="preview">既存のドキュメントの場合は、ドキュメントのサムネールの上にマウスポインターを置いて、 <strong>プレビュー</strong> ファイルをブラウザーに表示するには、または <strong>ダウンロード</strong> をクリックして、ファイルをコンピューターにダウンロードします。 新しいドキュメントについては、 <a href="/help/quicksilver/agile/get-started-with-boards/add-documents-on-cards.md">カードへのドキュメントの追加</a>.</span></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL 時間 ]</strong></td>
      <td>下記の「接続されたカードでのログ時間」を参照してください。</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL コメント ]</strong></td>
      <td><p>をクリックします。 <strong>[!UICONTROL 新しいコメント ]</strong> フィールドに入力し、コメントを入力します。 書式設定ツールを使用してテキストの書式を設定し、 <strong>添付ファイルを追加</strong> アイコン <img src="assets/attachment-icon.png" alt="添付ファイルアイコン"> をクリックして、コメントにファイルを添付します。 個人またはチームにタグを付けるには、コメント領域の下部にある検索ボックスを使用します。 ユーザーは、ボード上のメンバーである必要はありません。 接続されたカードのタグ付きユーザーは、電子メール通知を受け取ります。</p><p>クリック <strong>[!UICONTROL 送信 ]</strong> をクリックして、コメントをカードに追加します。</p>
      <p><strong>注意：</strong> カードのコメント領域では、新しいAdobe Workfrontのコメント機能が使用されます。 詳しくは、 <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md">作業を更新</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL システムアクティビティ ]</strong></td> 
      <td><p>次の条件を満たしている場合： <strong>システムアクティビティ</strong> をカードセクションとして有効にすると、この領域にアクティビティが表示されます。</p> <p>詳しくは、 <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">カードに表示するフィールドのカスタマイズ</a> および <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md">システムで追跡された更新</a>.</p></td>
     </tr>     
    </tbody> 
   </table>

   左側のナビゲーションパネルを使用して、カード詳細上のフィールドのセクション間を移動します。

1. クリック **[!UICONTROL 閉じる]** ボードに戻る
接続されたオブジェクト、割り当て先、タグ、期限、チェックリストカウンター、推定時間、ステータスがカードに表示されます。

   ![カードがボードに追加されました](assets/boards-connected-card-details-110922.png)

## 接続されたカードを取り外す

接続されたカードをWorkfrontオブジェクトから切断すると、そのカードは編集可能なアドホックカードとしてボードに残ります。

ボードレベルで切断するには：

1. ボードにアクセスします。
1. 次をクリック： **[!UICONTROL その他]** メニュー ![その他のメニュー](assets/more-icon-spectrum.png) 接続されたカードで、を選択します。 **[!UICONTROL 連携解除]**.
1. クリック **[!UICONTROL 連携解除]** をクリックします。

カードレベルで切断するには：

1. ボードにアクセスし、接続されたカードを開きます。
1. 次をクリック： **[!UICONTROL その他]** メニュー ![その他のメニュー](assets/more-icon-spectrum.png) カードの詳細の「接続」領域で、「 」を選択します。 **[!UICONTROL 連携解除]**.
1. クリック **[!UICONTROL 連携解除]** をクリックします。

## アドホックカードを接続済みカードに変換する

アドホックカードを作成したら、接続されたカードに変換できます。 アドホックカードについて詳しくは、 [ボードへのアドホックカードの追加](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

1. ボードにアクセスし、アドホックカードを開きます。
1. カードの名前と説明を確認します。 これらは、 [!DNL Workfront].
1. Adobe Analytics の [!UICONTROL 接続] カードの詳細の領域で、 **[!UICONTROL Workfrontとの接続]**.
1. 次の日： [!UICONTROL カードを接続] ウィンドウで、タスクを作成するかイシューを作成するかを選択します。
1. タスクまたはイシューを追加するプロジェクトを検索して選択します。

   >[!NOTE]
   >
   >* サーチ結果には、自分が権限を持っているオブジェクトのみが表示されます。
   >* 次の条件でフィルターする場合： **[!UICONTROL 自分が所有するプロジェクト]** または **[!UICONTROL 自分がいるプロジェクト]**、に等しいプロジェクト [!UICONTROL 完了], [!UICONTROL Dead]または [!UICONTROL 却下] ステータスが含まれていません。 これらのプロジェクトは、引き続き **[!UICONTROL すべて]** フィルター。

1. クリック **[!UICONTROL 接続]**.

   ![アドホックカードをWorkfrontに接続](assets/boards-connect-ad-hoc-card.png)

   プロジェクト名は、カードの詳細の「接続」領域に表示されます。

1. クリック **[!UICONTROL 閉じる]** ボードに戻る

## 接続されたカードでのログ時間

接続されたタスクまたは問題に関する時間を記録するには、適切な権限が必要です。

デフォルトでは、接続されたカードにタイムログフィールドが表示されません。 有効にする必要があります [!UICONTROL **時間**] （内） [!UICONTROL 設定] 下の領域 [!UICONTROL カード]. 詳しくは、 [カードに表示するフィールドのカスタマイズ](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. タスクまたはタスクの発行時間数を入力します。
1. を選択します。 [!UICONTROL 時間タイプ] デフォルトと異なる場合は、ドロップダウンメニューから。
1. クリック [!UICONTROL **ログ時間**].

   ![カードに記録する時間数](assets/log-hours-on-card.png)

   カードに記録された時間は、接続されたタスクまたはイシューにも保存されます。

カードのログ記録時間は、タスクまたは問題のログ記録時間と同じです。 詳細については、この記事の「プロジェクト、タスク、または問題に対するログの記録」を参照してください。 [ログ時間](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

