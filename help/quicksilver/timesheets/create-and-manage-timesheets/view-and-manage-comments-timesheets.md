---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: タイムシートのコメントの表示および管理
description: タイムシート、タイムシートに含まれる作業項目、およびログに記録する各時間エントリに対してコメントを付けることができます。
author: Alina
feature: Timesheets
exl-id: 6260d176-3cfb-4bc2-93cb-00687e030248
source-git-commit: 18dfb67626982d73ad33871b8afce4a3f0d4cdb3
workflow-type: tm+mt
source-wordcount: '847'
ht-degree: 100%

---

# タイムシートのコメントの表示および管理

<!-- Audited: April, 2024-->

タイムシート内の次の項目にコメントを付けることができます。

* タイムシート
* 時間エントリ
* タスクやイシューなど、個々の項目

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>新規：ライト以上 </p>
   <p>現在：レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベルの設定</td> 
   <td> <p>タスクとイシューへの閲覧またはそれ以上のアクセス権</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクとイシューに対する表示またはそれ以上の権限</p> </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスタイプまたはアクセス権を確認するには、Workfront 管理者にお問い合わせください。詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## タイムシートの時間エントリコメントを表示 {#view-hour-entry-comments-on-a-timesheet}

個々の時間エントリに対するコメントをタイムシートに表示するように設定できます。コメントの表示と非表示を切り替えるオプションは、タイムシート全体に対するコメントや、個々の項目に対するコメントには影響しません。詳しくは、[タイムシートにコメントする](#make-comments-on-a-timesheet)を参照してください。

デフォルトでは、タイムシートに初めてアクセスしたときはコメントが非表示になっています。

タイムシートにコメントを表示するには、次の手順を実行します。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックします。

1. 「**タイムシート**」をクリックします。
1. コメントを表示するタイムシートを開きます。
1. タイムシートの右上隅にある「**コメントの表示**」をクリックします。
時間エントリとコメントが記録された項目の下にコメントが表示されます。

   ![](assets/comments-expanded-under-tasks-redesigned-timesheet.png)


## タイムシートにコメントする {#make-comments-on-a-timesheet}

* [タイムシート全体に対するコメント](#comment-on-the-overall-timesheet)
* [タイムシートの個々の時間エントリに対するコメント](#comment-on-an-individual-hour-entry-in-a-timesheet)
* [タイムシートの作業項目に対するコメント](#comment-on-a-work-item-in-a-timesheet)

### タイムシート全体に対するコメント {#comment-on-the-overall-timesheet}

タイムシートに関する全般的なコメントを付けることができます。タイムシート全体に対するコメントは、他のオブジェクトに対するコメントと似ています。

1. 右上隅の&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、または（使用可能な場合は）左上隅または Workfront の&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/lines-main-menu.png) をクリックします。

1. 「**タイムシート**」をクリックします。
1. コメントを追加するタイムシートに移動します。
1. 左パネルの「**更新**」をクリックし、次に「**コメント**」タブをクリックします。
1. [作業の更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)の説明に従って、新しいコメントの追加を開始するか、既存のコメントに返信します。
1. （オプション）「**人物またはチームにタグ付け**」フィールドにユーザーまたはチームを追加して、他のユーザーを更新に含めます。詳しくは、[更新時の他のユーザーへのタグ付け](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)を参照してください。
1. （オプション）社内のユーザーだけに更新を表示する場合は、「**社外秘**」オプションを選択します。
1. コメントを入力してから、「**送信**」をクリックします。

   コメントがタイムシートの「[!UICONTROL 更新]」セクションの「コメント」タブに表示されます。

1. （オプション）「**システムアクティビティ**」タブをクリックして、システムによって生成された更新を確認します。

   または

   「**すべて**」タブをクリックすると、システムアクティビティおよびユーザーコメントが時系列で表示されます。

   >[!TIP]
   >
   >   「すべて」タブは読み取り専用タブで、ここからコメントに返信することはできません。


   詳しくは、[作業の更新](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md)を参照してください。

### タイムシートの個々の時間エントリに対するコメント {#comment-on-an-individual-hour-entry-in-a-timesheet}

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックします。

1. 「**タイムシート**」をクリックします。
1. コメントを追加するタイムシートに移動し、左側のパネルで「**タイムシート**」をクリックします。
1. コメントを追加する時間エントリフィールドをクリックし、「**コメント**」をクリックして時間エントリのコメントを追加します。

   >[!TIP]
   >
   >   時間入力ボックスをクリックした後で標準の QWERTY キーボードを使用する場合は、次のキーのセットを押してコメントボックスを開きます。
   >   * Windows コンピューターおよび Mac コンピューターの両方で Shift + F2 を押します。

   次のいずれかの操作を行います。

   * 新しいコメントを入力し、「**完了**」をクリックします。
   * 既存のコメントを編集して「**完了**」をクリックするか、「**キャンセル**」をクリックして変更を破棄します。
   * **削除**&#x200B;アイコン ![](assets/delete.png) をクリックして、保存したコメントを削除します。

     時間エントリボックスの右上隅に、時間エントリで記録されたコメントがあることを示す青いマーカーが表示されます。

   ![](assets/commment-button-on-hour-log-redesigned-timesheet.png)

   >[!TIP]
   >
   >   標準の QWERTY キーボードを使用する場合は、コメントボックス内から次のキーを押してコメントを保存します。
   >   * Windows コンピューターの場合は、Ctrl + Enter キーを押します。
   >   * Mac コンピューターの場合は Cmd + Return キーを押します。


1. （オプション）タイムシートに表示する時間エントリコメントを設定するには、この記事の[タイムシートに時間エントリコメントを表示](#view-hour-entry-comments-on-a-timesheet)を参照してください。

### タイムシートの作業項目に対するコメント {#comment-on-a-work-item-in-a-timesheet}

>[!TIP]
>
>タイムシート内の個々の項目にコメントを付け、その実際の開始日または条件を更新できます。更新は、ログに記録された時間に関連付けられたオブジェクトの「更新」エリアに表示されます。


タイムシート内では、タスクとイシューに対してのみコメントを付けることができます。プロジェクトや一般時間に対してコメントを付けることはできません。

1. Adobe Workfront の右上隅にある&#x200B;[!UICONTROL **メインメニュー**]&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックします。
1. 「[!UICONTROL **タイムシート**]」をクリックします。
1. コメントを追加するタイムシートに移動し、左側のパネルで「[!UICONTROL **タイムシート**]」をクリックします。
1. タスクまたはイシューの行をクリックし、「[!UICONTROL **概要を開く**]」をクリックします。
1. 概要パネルの&#x200B;[!UICONTROL **更新**]&#x200B;エリアで更新の入力を開始して、「[!UICONTROL **送信**]」をクリックします。
更新は、タスクとイシューの「更新」セクションに表示されます。
1. （オプション）「[!UICONTROL **概要を閉じる**]」をクリックして概要パネルを閉じます。

   概要パネルでのタスクとイシューの更新について詳しくは、[概要について](../../workfront-basics/the-new-workfront-experience/summary-overview.md)を参照してください。
