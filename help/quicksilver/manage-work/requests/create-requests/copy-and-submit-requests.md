---
title: リクエストのコピーと送信
description: 同様のリクエストを頻繁に送信する場合は、既存の送信済みリクエストをコピーできます。この場合、既存のリクエストをコピーし、最小限の変更を加えて、新しいリクエストとして再送信できます。
author: Alina
feature: Work Management
role: User
topic: Collaboration
exl-id: 3d7581d0-e99c-4204-b1e5-04fde72251bb
source-git-commit: 3a2745437e00ac968f2a4590be2637dbc01594ad
workflow-type: tm+mt
source-wordcount: '1381'
ht-degree: 95%

---

# リクエストのコピーと送信

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span>-->

同様のリクエストを頻繁に送信する場合は、既存の送信済みリクエストをコピーできます。この場合、既存のリクエストをコピーし、最小限の変更を加えて、新しいリクエストとして再送信できます。

## アクセス要件

<!--drafted - replace table with P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td><p>Current license: Contributor or higher</p> 
   Or
   <p>Legacy license: Request or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Issues</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Access to add requests to a request queue</p> <p>View or higher permissions on the existing request</p> <p>For information on setting up a request queue, see <a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">Create a Request Queue</a>. </p> </td> 
  </tr> 
 </tbody> 
</table>
-->
この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>イシューへのアクセス権を編集</p> <p><b>メモ</b>

アクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>リクエストキューにリクエストを追加するためのアクセス権</p> <p>既存のリクエストに対する表示またはそれ以上の権限</p> <p>リクエストキューの設定について詳しくは、<a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">リクエストキューの作成</a>を参照してください。 </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 前提条件

自分または組織内の誰かが以前に送信したリクエストをコピーして再送信できる場合があります。リクエストが他のユーザーに属する場合、それをコピーして新しいリクエストとして送信するには、少なくともリクエストを表示できるアクセス権が必要です。

## リクエストをコピーし、新しいリクエストとして送信する際の考慮事項

* 送信済みのリクエストのコピーと送信のみ可能です。ドラフトのリクエストはコピーできません。
* コピーして送信できるリクエストは、もともと自分が送信したリクエストや、少なくとも表示できるアクセス権のある他のユーザーが送信したリクエストです。
* 自分自身のリクエストは、誰かにアクセス権を削除されない限り、常にコピーして送信することができます。
* 誰かが送信したリクエストを同じ会社の人が常にコピーして送信できるようにするには、リクエストキューの作成者が、キューの詳細エリアまたはプロジェクトの編集エリアで、「**同じ会社のユーザーがすべてのリクエストに対して同じ権限を継承する**」を有効にします。この設定を無効にすると、自分のリクエストを表示できるのはリクエストを行った本人だけになります。

  詳しくは、次の記事を参照してください。

   * [リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)
   * [プロジェクトの編集](../../../manage-work/projects/manage-projects/edit-projects.md)

* 元のリクエストをコピーして更新すると、新しいリクエストとして再送信できます。
* 元のリクエストを送信した後に次の変更が生じた場合は、コピーして再送信することはできません。

   * リクエストキューが削除された。
   * キュートピックが削除された。

     >[!TIP]
     >
     >リクエストキュー内にキュートピックさえあれば、そのリクエストはコピーして送信することができ、リクエストキューに保存されます。

   * リクエストキューは、ヘルプリクエストキューとして公開されなくなりました。詳しくは、[リクエストキューの作成](../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md)を参照してください。
   * リクエストキューにキュートピックがなく、元のリクエストが 2022年1月より前に送信された。

   * リクエストキューに関連付けられているプロジェクトのステータスが「現在」でなくなった。

* 変換を行ったリクエストが変換プロセスで保持されている場合は、そのリクエストをコピーして送信できます。詳しくは、[Adobe Workfront でのイシューの変換の概要](../../../manage-work/issues/convert-issues/convert-issues.md)を参照してください。

  >[!TIP]
  >
  >コピーされたリクエストが解決オブジェクトにリンクされていない。

## リクエストのコピーと送信

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、「**リクエスト**」をクリックします。
1. （条件付き）「送信済み」セクションがデフォルトで表示されない場合は、左パネルで「**送信済み**」をクリックします。

   >[!TIP]
   >
   >   Workfrontまたはグループ管理者がレイアウトテンプレートをカスタマイズし、環境のメインメニューまたは左パネルから領域を削除する場合があります。 この場合、これらは使用できない可能性があります。

1. 新規としてコピーして送信するリクエストを検索し、次のいずれかの操作を行います。

   * 選択して、送信済みのリクエストリストの左上隅で&#x200B;**コピー** ![](assets/copy-and-submit-as-new-requests-area-nwe.png) をクリックします。

   >[!TIP]
   >
   > 最初にリクエストを選択していない場合、コピーアイコンはグレー表示になります。

   * リクエスト名の右側にある「**その他**」メニュー ![](assets/more-icon.png)、「**新規としてコピーして送信**」の順にクリックします。

     または

     選択したリクエストを右クリックし、「**新規としてコピーして送信**」をクリックします。

     ![](assets/request-selected-more-menu-options-nwe-350x191.png)

     >[!TIP]
     >
     >イシューを作成するアクセス権がない場合は、管理者によってリクエストの作成が制限されたという警告が表示されます。

1. （オプション）必要に応じて、次の情報を更新します。

   * **リクエストタイプ**：コピーしたリクエストが保存されるリクエストキュー。デフォルトでは、コピーされたリクエストは、元のリクエストのリクエストキューに保存されます。
   * **トピックグループ**&#x200B;および&#x200B;**トピックをキュー**（選択されている場合）。名前またはトピックグループとキューのトピックは、環境に合わせてカスタマイズされます。デフォルトでは、コピーしたリクエストは、元のリクエストのトピックグループおよびキューのトピックに保存されます。

     >[!TIP]
     >
     >パスが元のリクエストのパスから変更された場合、リクエストのキューの作成者はキューを変更しました。

1. （オプション）コピーしたリクエストの情報を更新します。プロジェクト上の「**キューの詳細**」サブタブの「**新しいイシューフィールド**」セクションで、リクエストキュー作成者がどのフィールドを有効にするかに応じて、次のフィールドのいずれかが表示されます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>件名</strong> </td> 
      <td>元のリクエストの名前を表示します。必要に応じて更新します。更新しない場合、Workfront は、コピーしたリクエストに <b>&lt;Name of original request&gt; のコピー</b>という名前を付けます。これは必須フィールドです。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>説明</strong> </td> 
      <td>元のリクエストの説明を表示します。必要に応じて更新します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>URL</strong> </td> 
      <td> <p>元のリクエストの URL を表示します。必要に応じて更新します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>優先度</strong> </td> 
      <td> <p>リクエストの優先順位を指定します。優先度は、このリクエストをどの程度の速度で解決すべきかを定義する必要があります。デフォルトのオプションは次のとおりです。</p> 
       <ul> 
        <li>なし</li> 
        <li>低</li> 
        <li>標準</li> 
        <li>高</li> 
        <li>緊急</li> 
       </ul> <p>優先順位の名前は、Workfront 管理者が変更できます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>重要度</strong> </td> 
      <td> <p>リクエストの重要度を指定します。重大度は、時間内に解決されない場合に、このリクエストが作業に与える影響を定義する必要があります。デフォルトのオプションは次のとおりです。</p> 
       <ul> 
        <li>一時回避</li> 
        <li>混乱を招く</li> 
        <li>対処策のあるバグ</li> 
        <li>対処策のないバグ</li> 
        <li>致命的なエラー</li> 
       </ul> <p>Workfront の管理者は重要度の名前を変更できます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>プライマリ連絡先</strong> </td> 
      <td>リクエストのプライマリ連絡先は、リクエストに関する質問に対処する時点の担当者なので、デフォルトでユーザーに設定されます。ただし、これを他の Workfront ユーザーに変更することはできます。</td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span><strong>割り当て</strong></span> </td> 
      <td> <p>リクエストを割り当てる必要があるアクティブなユーザー、担当業務、またはチームの名前を指定します。 </p> <p> 複数のユーザー、担当業務、またはチームを指定できます。 </p> <p>リクエストキューの設定によっては、リクエストを 3 つすべてではなく、1 つまたは 2 つのタイプのリソースにのみ割り当てることができます。 </p> <p>リクエストキューを適切なリソースに自動的にルーティングできるように、ルーティング規則をリクエストキューに使用することをお勧めします。 </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p><p style="font-weight: normal;">リクエストキューの設定によっては、リクエストに割り当てるリソースのタイプが 1 つ（例：ユーザー）に限られる場合があります。ルーティングルールもリクエストキューに関連付けられ、異なるタイプのリソース（チームなど）に自動的にルーティングする場合、リクエスト（ユーザー）の送信時に手動で指定したエンティティとルーティングルール（チーム）で指定したリソースの両方にリクエストが割り当てられます。</p> <p style="font-weight: normal;">詳しくは、次の記事を参照してください。</p> 
        <ul> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-request-queue.md" class="MCXref xref">リクエストキューの作成</a> </p> </li> 
         <li> <p><a href="../../../manage-work/requests/create-and-manage-request-queues/create-routing-rules.md" class="MCXref xref">ルーティング規則の作成</a> <br> </p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>予定時間数</strong> </td> 
      <td> <p>このリクエストの完了に要する時間を見積もります。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>予定開始日</strong> </td> 
      <td> <p>このリクエストでの作業を開始する日付。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>予定完了日</strong> </td> 
      <td>このリクエストを解決したい日付。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ステータス</strong> </td> 
      <td>新しいリクエストのデフォルトのステータスは「新規」です。Workfront管理者がこのステータスの名前を変更している可能性があります。 このドロップダウンメニューからステータスを別のものに変更することもできます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>ドキュメント</strong> </td> 
      <td> <p>リクエストにドキュメントを追加します。元のリクエストに添付されたドキュメントは、コピーされたリクエストに転送されません。</p> <p><b>ヒント</b>

   リクエストキューの設定に応じて、カスタムフィールドの前後に「ドキュメント」セクションが表示される場合があります。</p> <p> </p> </td>
   </tr> 
    </tbody> 
   </table>

1. （オプション）必要に応じて、添付されたカスタムフォームの情報を更新します。

   >[!TIP]
   >
   >* 元のリクエストに添付されたすべてのカスタムフォームと、カスタムフィールドに含まれる値は、コピーされたリクエストに転送されます。これには、ロジックを含むフィールドが含まれます。
   >* コピーしたリクエストからカスタムフォームを削除することはできません。

1. 「**送信**」をクリックします。

   コピーされたリクエストは、指定したリクエストキューで新しいリクエストとして送信されます。
