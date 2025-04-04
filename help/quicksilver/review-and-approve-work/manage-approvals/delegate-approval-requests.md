---
product-area: projects
navigation-topic: approvals
title: 承認リクエストをデリゲート
description: 承認リクエストを委任すると、休暇でオフィスを離れる場合など、一定期間リクエストを承認する別のユーザーを割り当てることができます。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 01b76dd5-98cb-4f0d-97ff-7e665f843a9c
source-git-commit: 1e67375c12bc473130127887e6cd4fa474c4fb02
workflow-type: tm+mt
source-wordcount: '1209'
ht-degree: 78%

---

# 承認リクエストをデリゲート

不在時に割り当てられた作業を、一時的にデリゲートできます。タスクとイシューの割り当てを委任したり、承認リクエストを委任したりできます。 この記事では、承認リクエストをデリゲートする方法について説明します。タスクとイシューの割り当ての委任については、[ タスクとイシューの委任 ](../../manage-work/delegate-work/how-to-delegate-work.md) を参照してください。

承認の割り当て方法（直接自分に割り当てられたか、自分が所属するチームに割り当てられたか、自分の担当業務に割り当てられたか）に関係なく、以下のタイプの承認をデリゲートできます。

* プロジェクト承認
* タスク承認
* イシュー承認

タイムシート、ドキュメント、プルーフの承認はデリゲートできません。

>[!NOTE]
>
>承認をデリゲートするようにスケジュールした日付に不一致が発生しないように、ユーザープロファイルのタイムゾーンをスケジュールのタイムゾーンと一致させることをお勧めします。詳しくは、次の記事を参照してください。
>
>* [スケジュールを作成](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [ユーザーのプロファイルを編集](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td> <p>レビュー以上</p> </td> 
  </tr> 
 </tbody> 
</table>

お持ちのプランやライセンスの種類を確認するには、Workfront管理者にお問い合わせください。

+++

## デリゲートされた承認のユーザーのアクセス権について

指定された承認期間中、承認リクエストをデリゲートされたユーザーは、以下の能力を持ちます。

* 決定が下されていない既存の承認リクエストを承認または却下できます
* 指定した期間中に受け取った新しい承認リクエストを承認および却下できます
* 承認待ちのオブジェクトに対する表示アクセス権が付与されます

  >[!NOTE]
  >
  >Adobe Workfront の管理者は、特定のオブジェクトタイプにアクセスできないように、ユーザーを制限できます。ユーザーがオブジェクトタイプに対するアクセス権を持たず、そのタイプの承認がユーザーに委任された場合、ユーザーはオブジェクトに対する表示アクセス権を持ちません。ただし、[作業の承認](../../review-and-approve-work/manage-approvals/approving-work.md)で説明されているように、ユーザーは&#x200B;**ホーム**&#x200B;ページから承認リクエストを承認または拒否することができます。\
  >例えば、ユーザー A はグループ A に属しています。Workfront 管理者がグループ A のアクセス権を制限したため、このグループのユーザーは Workfront 内のタスクを表示できません。タスクの承認リクエストがユーザー A に委任されている場合、ユーザー A は承認が関連付けられているタスクを表示できません。ただし、ユーザー A はホームページから承認リクエストを承認または却下できます。

  Workfront 管理者が設定内のオブジェクトタイプへのアクセスを制限する方法について詳しくは、[カスタムアクセスレベルを作成または変更](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。

承認の委任が停止またはキャンセルされた後、承認者として指定されたユーザーは、以下の状態になります。

* 承認が必要な項目の作業を承認するアクセス権がなくなりました
* 作業アイテムに対しては、引き続き表示アクセス権があります\
  承認の委任経由でオブジェクトに対する表示アクセス権を付与されたユーザーは、承認の委任が停止したり取り消されたりした後でも、その表示アクセス権を保持します。承認が委任されている期間中に、ユーザーがアクセス権を持つオブジェクトに対する表示アクセス権を削除するには、オブジェクトに移動し、そのオブジェクトから直接アクセス権を削除する必要があります。

## 別のユーザーに承認をデリゲート {#delegate-your-approvals-to-another-user}

承認の割り当て方法（直接自分に割り当てられたか、自分が所属するチームに割り当てられたか、自分の担当業務に割り当てられたか）に関係なく、以下のタイプの承認をデリゲートできます。

* プロジェクト承認
* タスク承認
* イシュー承認

タイムシート、ドキュメント、プルーフの承認はデリゲートできません。

承認をデリゲートする際は、以下の点を考慮してください。

* 承認をデリゲートすると、すべての承認がデリゲートされます。個別の承認リクエストをデリゲートすることはできません。
* 承認は、1 名のユーザーに対してのみデリゲートできます。同時に複数のユーザーに承認をデリゲートすることはできません。\
  すべてのプロジェクト、タスクおよびイシューの承認はすべて、指定したユーザーに委任されます。
* 最大 5 名のユーザーが、同時に同じユーザーに承認を委任できます。つまり、1 人のユーザーを同時に 6 人以上のユーザーの一時的な承認者に指定することはできません。
* 承認に関するアクティビティは、「更新」タブに表示されます。「システム更新を表示」を有効にしておく必要があります。承認を委任したユーザーと承認を委任されたユーザーの両方に、承認アクティビティに関するメール通知が届きます。

### ホームエリアからの承認の委任


別のユーザーに承認を委任するには、次の手順に従います。

1. 右上隅の **[!UICONTROL メインメニュー]**![ メインメニューアイコン ](assets/main-menu-icon.png) をクリックし、**[!UICONTROL ホーム]** をクリックします。
1. （条件付き） **カスタマイズ** をクリックして **マイ承認** ウィジェットを追加します。
1. マイ承認ウィジェットに移動し、「**マイ承認をデリゲート**」をクリックします。

   >[!NOTE]
   >
   >Workfront管理者は、設定エリアから承認の委任を無効にすることができます。 承認委任が無効になっている場合、「承認を委任」ボタンは表示されません。

   ![ ホームでの承認の委任 ](assets/delegate-approvals-home.png)

1. 「マイ承認を委任」セクションで、次の情報を指定します。

   * **名前**：承認の委任先となるユーザーの名前を入力していき、ドロップダウンメニューに表示される名前をクリックします。
   * **開始日**：承認の転送が開始される日付を選択します。選択した日の午前 12:00 に転送が始まります。\
     開始日は、現在の日付または将来の日付にする必要があります。
   * **終了日**：次のいずれかの操作を行います。
      * 承認の転送を停止する日付を選択します。選択した日の午後 11:59 に転送が終了します。
      * 「**終了日なし**」を選択して、承認を無期限に委任するように Workfront を設定します。

1. 「**保存**」をクリックします。

### ユーザープロファイルからの承認の委任

1. 左パネルで&#x200B;**メインメニュー**&#x200B;アイコン／**[自分の名前]**／**休暇**&#x200B;をクリックします。
1. **承認を委任** をクリックします。

   >[!NOTE]
   >
   >Workfront管理者は、設定エリアから承認の委任を無効にすることができます。 承認委任が無効になっている場合、「承認を委任」ボタンは表示されません。
1. 「マイ承認を委任」セクションで、次の情報を指定します。

   * **名前**：承認の委任先となるユーザーの名前を入力していき、ドロップダウンメニューに表示される名前をクリックします。
   * **開始日**：承認の転送が開始される日付を選択します。選択した日の午前 12:00 に転送が始まります。\
     開始日は、現在の日付または将来の日付にする必要があります。
   * **終了日**：次のいずれかの操作を行います。
      * 承認の転送を停止する日付を選択します。選択した日の午後 11:59 に転送が終了します。
      * 「**終了日なし**」を選択して、承認を無期限に委任するように Workfront を設定します。

## 承認委任の更新または停止 {#update-or-stop-an-approval-delegation}

1. 右上隅の **[!UICONTROL メインメニュー]**![ メインメニューアイコン ](assets/main-menu-icon.png) をクリックし、**[!UICONTROL ホーム]** をクリックします。
1. （条件付き） **カスタマイズ** をクリックして **マイ承認** ウィジェットを追加します。

1. 自分の承認ウィジェットに移動し、「**委任を編集**」をクリックします。
   ![ 委任を編集 ](assets/edit-delegations.png)
<!--
   Or

   If your system or group administrator enabled task and issue delegation, click **Edit delegation**, then click **Delegate approvals**.   -->

1. （条件付き）次のいずれかを行います。

   * 既存の承認委任を更新するには、表示されている情報を変更し、「**保存**」をクリックします。

   * 既存の委任を停止するには、「**委任を停止**」をクリックしたあと、「**委任を停止**」をクリックして確定します。

## 委任された承認の表示 {#view-delegated-approvals}

自分の承認ウィジェットで表示できる承認委任のタイプは、次に示すとおりになります。

* プロジェクト承認
* タスク承認
* イシュー承認

委任された承認を表示するには、次の手順に従います。

1. 右上隅の **[!UICONTROL メインメニュー]**![ メインメニューアイコン ](assets/main-menu-icon.png) をクリックし、**[!UICONTROL ホーム]** をクリックします。
1. （条件付き） **カスタマイズ** をクリックして **マイ承認** ウィジェットを追加します。
1. **マイ承認** ウィジェットで「**フィルター**」ドロップダウンメニューをクリックし、「**委任済み承認**」をクリックします。\
   自分に委任されたすべての承認がリストに表示されます。
