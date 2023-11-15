---
product-area: timesheets
navigation-topic: create-and-manage-timesheets
title: タイムシートのコメントの表示と管理
description: タイムシート、タイムシートに含まれる作業項目、およびログに記録する各時間エントリに対してコメントを付けることができます。
author: Alina
feature: Timesheets
exl-id: 6260d176-3cfb-4bc2-93cb-00687e030248
source-git-commit: 90c730bbab2e62bcc60bee37272edb1219b2afb4
workflow-type: tm+mt
source-wordcount: '841'
ht-degree: 0%

---

# タイムシートのコメントの表示と管理

タイムシート内の次の項目にコメントを付けることができます。

* タイムシート上
* 時間のエントリ
* タスクやイシューなどの個々の項目に対して

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>確認 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タスクおよび問題へのアクセス権以上の表示</p> <p>まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>タスクおよび問題に対する権限を表示または上限に設定する</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## タイムシートの時間入力コメントを表示します {#view-hour-entry-comments-on-a-timesheet}

タイムシートに表示する個々の時間エントリに対して行われるコメントを構成できます。 コメントの表示と非表示を切り替えるオプションは、タイムシート全体に対するコメントや、個々のアイテムに対するコメントには影響しません。 詳しくは、  [タイムシートにコメントを付ける](#make-comments-on-a-timesheet).

既定では、タイムシートに初めてアクセスしたときにコメントは非表示になります。

タイムシートにコメントを表示するには、次の手順に従います。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅にある

1. クリック **タイムシート**.
1. コメントを表示するタイムシートを開きます。
1. クリック **コメントを表示** タイムシートの右上隅に表示されます。
時間エントリとコメントが記録された項目の下にコメントが表示されます。

   ![](assets/comments-expanded-under-tasks-redesigned-timesheet.png)


## タイムシートにコメントを付ける {#make-comments-on-a-timesheet}

* [タイムシート全体に対するコメント](#comment-on-the-overall-timesheet)
* [タイムシートの個々の時間の入力に対するコメント](#comment-on-an-individual-hour-entry-in-a-timesheet)
* [タイムシートの作業項目に対するコメント](#comment-on-a-work-item-in-a-timesheet)

### タイムシート全体に対するコメント {#comment-on-the-overall-timesheet}

タイムシートに関する一般的なコメントを作成できます。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅にある

1. クリック **タイムシート**.
1. コメントを作成するタイムシートに移動します。
1. クリック **更新** 左のパネルで、 **コメント** タブをクリックします。
<!--
1. (Optional) Start typing a keyword or a the name of a user associated with a comment in the **Search** field, in the upper-right corner of the Comments tab. 

   If found, the keyword or user you searched for is highlighted and the comments associated with them display at the top of the Comments tab. -->
1. 更新を **新しいコメント** ボックス。
1. （オプション） **担当者またはチームのタグ付け** フィールドを使用して、他の項目を更新に含めます。 詳しくは、 [更新時の他のユーザーへのタグ付け](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).
1. （オプション）コメントにリッチテキスト書式を追加します。 詳しくは、 [作業を更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. （オプション） **私の会社に対してプライベート** 会社の担当者のみに更新を表示する場合は、オプションを使用します。
1. コメントを入力し、「 **送信**.

   コメントが [!UICONTROL 更新] タイムシートのセクション。

1. （オプション） **システムアクティビティ** タブをクリックして、システムで生成された更新を確認します。

   詳しくは、この記事の「システム更新の有効化または無効化」の節を参照してください [作業を更新](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

### タイムシートの個々の時間の入力に対するコメント {#comment-on-an-individual-hour-entry-in-a-timesheet}

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅にある

1. クリック **タイムシート**.
1. コメントを作成するタイムシートに移動し、[ ] をクリックします。 **タイムシート** をクリックします。
1. コメントを入力する時間入力フィールドをクリックし、 **コメント** をクリックして、1 時間のエントリにコメントを追加します。

   >[!TIP]
   >
   >   時間入力ボックスをクリックした後で標準の QWERTY キーボードを使用する場合は、次のキーのセットを押してコメントボックスを開きます。
   >   * Windows とMacの両方のコンピューターで Shift + F2 を押します。

   次のいずれかの操作を行います。

   * 新しいコメントを入力し、 **完了**.
   * 既存のコメントを編集し、「 **完了**&#x200B;または、「 **キャンセル** 変更を破棄します。
   * 次をクリック： **削除** アイコン ![](assets/delete.png) をクリックして、保存したコメントを削除します。

     時間入力ボックスの右上隅に、時間入力時に記録されたコメントがあることを示す青いマーカーが表示されます。

   ![](assets/commment-button-on-hour-log-redesigned-timesheet.png)

   >[!TIP]
   >
   >   標準の QWERTY キーボードを使用する場合は、コメントボックス内から次のキーを押してコメントを保存します。
   >   * Windows コンピューターの場合は、Ctrl + Enter キーを押します。
   >   * Macコンピューターの Cmd + Return キー。


1. （オプション）タイムシートに表示する時間入力コメントを構成するには、「 [タイムシートの時間入力コメントを表示します](#view-hour-entry-comments-on-a-timesheet) 」を参照してください。

### タイムシートの作業項目に対するコメント {#comment-on-a-work-item-in-a-timesheet}

>[!TIP]
>
>タイムシート内の個々の項目にコメントを付け、その [ 実績開始日 ] または [ 条件 ] を更新できます。 更新は、ログに記録された時間に関連付けられたオブジェクトの「更新」領域に表示されます。


タイムシートのタスクと問題に対してのみコメントを付けることができます。 プロジェクトや一般時間に対してコメントを付けることはできません。

1. 次をクリック： [!UICONTROL **メインメニュー**] アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅にある
1. クリック [!UICONTROL **タイムシート**].
1. コメントを作成するタイムシートに移動し、[ ] をクリックします。 [!UICONTROL **タイムシート**] をクリックします。
1. タスクまたはイシューの行をクリックし、「 [!UICONTROL **概要を開く**].
1. 更新の入力を開始するには、 [!UICONTROL **更新**] 「概要」パネルの領域で、「 [!UICONTROL **更新**].
更新は、タスクとイシューの「更新」セクションに表示されます。
1. （オプション）「 [!UICONTROL **概要を閉じる**] をクリックして、Summary パネルを閉じます。

   概要パネルでのタスクと問題の更新について詳しくは、 [概要の概要](../../workfront-basics/the-new-workfront-experience/summary-overview.md).
