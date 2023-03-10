---
product-area: projects
navigation-topic: approvals
title: 承認リクエストを委任
description: 承認リクエストを委任すると、休暇中に不在になる場合など、別のユーザーにリクエストを一定の期間承認するように割り当てることができます。
author: Courtney
feature: Work Management
exl-id: 01b76dd5-98cb-4f0d-97ff-7e665f843a9c
source-git-commit: d04afc0cc55a71e48c357af2ed4446c22dab1ba4
workflow-type: tm+mt
source-wordcount: '1203'
ht-degree: 0%

---

# 承認リクエストを委任

不在時に割り当てられた作業を一時的に委任できます。 タスクや問題の割り当てを委任したり、承認リクエストを委任したりできます。 この記事では、承認リクエストを委任する方法について説明します。 タスクの委任と問題の割り当てについて詳しくは、 [タスクと問題の委任を管理](../../manage-work/delegate-work/how-to-delegate-work.md).

>[!NOTE]
>
>承認を委任するスケジュールを設定した日付との不一致が生じないようにするには、ユーザープロファイルのタイムゾーンがスケジュールと一致するようにすることをお勧めします。 詳しくは、次の記事を参照してください。
>
>* [スケジュールの作成](../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md)
>* [ユーザーのプロファイルの編集](../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)
>


## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront plan*</p></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront license*</p></td> 
   <td> <p>レビュー以上</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプランまたはライセンスの種類を確認するには、Workfront管理者に問い合わせてください。

## 委任された承認のユーザーアクセスを理解します

指定された承認期間中、承認リクエストを委任したユーザーは、次の機能を持ちます。

* 決定がおこなわれていない既存の承認リクエストを承認または却下できます
* 指定した期間に受け取った新しい承認リクエストを承認および却下できます
* 承認待ちのオブジェクトに対するビュー・アクセス権が付与されます。

   >[!NOTE]
   >
   > Adobe Workfrontの管理者は、ユーザーが特定のオブジェクトタイプにアクセスできないように制限できます。 ユーザーがオブジェクト型にアクセスできず、その型の承認がユーザーに委任された場合、ユーザーはオブジェクトに対するビューアクセス権を持ちません。 ただし、ユーザーは、 **ホーム** ページ、 [作業の承認](../../review-and-approve-work/manage-approvals/approving-work.md).\
   例えば、ユーザー A はグループ A に属しています。Workfront管理者はグループ A のアクセス権を制限しているので、このグループのユーザーはWorkfront内のタスクを表示できません。 タスクの承認要求がユーザー A に委任されている場合、ユーザー A は承認が関連付けられているタスクを表示できません。 ただし、ユーザー A はホームページから承認リクエストを承認または却下できます。

   Workfront管理者がセットアップ内のオブジェクトタイプにアクセスを制限する方法について詳しくは、  [カスタムアクセスレベルの作成または変更](../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). 

承認の委任が停止またはキャンセルされた後、承認者として指定されたユーザーは、次の操作を実行します。

* 承認が必要な項目の作業を承認するアクセス権がなくなりました
* 作業項目に引き続き表示アクセス権を持ちます\
   承認委任経由でオブジェクトに対する表示アクセス権を付与されたユーザーは、承認委任が停止したり取り消されたりした後でも、その表示アクセス権を保持します。 承認が委任された間にユーザーがアクセスしたオブジェクトに対するビュー・アクセス権を削除するには、オブジェクトに移動し、そのオブジェクトから直接アクセス権を削除する必要があります。

## ホーム領域で承認リクエストを委任

* [別のユーザーに承認を委任](#delegate-your-approvals-to-another-user)
* [承認委任の更新または停止](#update-or-stop-an-approval-delegation)
* [委任された承認の表示](#view-delegated-approvals)

### 別のユーザーに承認を委任 {#delegate-your-approvals-to-another-user}

承認の割り当て方法 ( 直接自分に割り当てられたか、自分が所属するチームに割り当てられたか、自分の職務の役割に割り当てられたかに関係なく、次の種類の承認を委任できます。

* プロジェクト承認
* タスク承認
* 問題の承認

タイムシートとドキュメントの承認を委任することはできません。 

承認を委任する際は、次の点を考慮してください。

* 承認を委任すると、すべての承認が委任されます。 個々の承認リクエストを委任することはできません。
* 承認は 1 人のユーザーにのみ委任できます。複数のユーザーに同時に承認を委任することはできません。\
   すべてのプロジェクト、タスクおよびタスクに対するすべての承認は、指定したユーザーに委任されます。
* 同じユーザーに同時に承認を委任できるユーザーは最大 5 人です。 つまり、1 人のユーザーを同時に 5 人以上のユーザーの一時承認者に指定することはできません。
* 承認に関するアクティビティは、「更新」タブに表示されます。 [ システム更新の表示 ] を有効にしておく必要があります。 承認を委任するユーザーと承認を委任されるユーザーの両方に、承認アクティビティに関する電子メール通知が届きます。

別のユーザーに承認を委任する手順は、次のとおりです。

1. 次をクリック： **ホーム** アイコン ![](assets/home-icon-30x29.png) Adobe Workfrontの左上隅に

   >[!NOTE]
   Workfront管理者は、お使いの環境のホームアイコンに次の変更を加えることができます。
   * 組織を説明するようにカスタマイズされた画像に置き換えます。 この場合、この記事に示すアイコンは異なります。
   * リンクされたページを別のページに置き換えます。 この場合、 **メインメニュー** ![](assets/main-menu-icon.png) ページの右上隅にある「 **ホーム**.


   または

   次をクリック： **メインメニュー** アイコン/ **あなたの名前** > **オフの時間** をクリックします。

1. （オプションおよび条件付き）「Home」領域で、 **フィルター** ドロップダウンメニューで、 **承認**.

1. （条件付き）クリック **自分の承認を委任**

   または

   システムまたはグループ管理者がタスクと問題の委任を有効にした場合は、 **委任**&#x200B;を選択し、「 **承認を委任**.

   ![](assets/delegate-approvals-nwe.png)

1. 「自分の承認を委任」セクションで、次の情報を指定します。

   * **名前**:承認を委任するユーザーの名前を入力し、ドロップダウンメニューに表示されたら名前をクリックします。
   * **開始日**:転送を開始する承認の日付を選択します。 転送は選択した日の午前 12 時から開始します。\
      開始日は、現在の日付または将来の日付にする必要があります。
   * **終了日**：次のいずれかの操作を行います。

      * 転送を停止する承認の日付を選択します。 転送は選択した日の午後 11 時 59 分に終了します。
      * 選択 **終了日がありません** 承認を無期限に委任するようにWorkfrontを設定する場合。

1. 「**保存**」をクリックします。

### 承認委任の更新または停止 {#update-or-stop-an-approval-delegation}

1. 次をクリック： **ホーム** アイコン ![](assets/home-icon-30x29.png) Adobe Workfrontの左上隅に

   >[!NOTE]
   Workfront管理者は、お使いの環境のホームアイコンに次の変更を加えることができます。
   * 組織を説明するようにカスタマイズされた画像に置き換えます。 この場合、この記事に示すアイコンは異なります。
   * リンクされたページを別のページに置き換えます。 この場合、 **メインメニュー** ![](assets/main-menu-icon.png) ページの右上隅にある「 **ホーム**.


1. 次をクリック： **フィルター** ドロップダウンメニューで、 **承認**.

1. （条件付き）クリック **委任を編集**

   または

   システムまたはグループ管理者がタスクと問題の委任を有効にした場合は、 **委任を編集**&#x200B;を選択し、「 **承認を委任**.

1. （条件付き）次のいずれかの操作を行います。

   * 既存の承認委任を更新するには：表示される情報を変更し、「 **保存**.

   * 既存の委任を停止するには：クリック **委任を停止**&#x200B;を選択し、「 **委任を停止** をクリックして確定します。

      ![](assets/stop-delegation-nwe.png)

### 委任された承認の表示 {#view-delegated-approvals}

作業リストには、次のタイプの承認委任のみ表示できます。

* プロジェクト承認
* タスク承認
* 問題の承認

委任承認を表示する手順は、次のとおりです。

1. 次をクリック： **ホーム** アイコン ![](assets/home-icon-30x29.png) Adobe Workfrontの左上隅に

   >[!NOTE]
   Workfront管理者は、お使いの環境のホームアイコンに次の変更を加えることができます。
   * 組織を説明するようにカスタマイズされた画像に置き換えます。 この場合、この記事に示すアイコンは異なります。
   * リンクされたページを別のページに置き換えます。 この場合、 **メインメニュー** ![](assets/main-menu-icon.png) ページの右上隅にある「 **ホーム**.


1. 次をクリック： **フィルター** ドロップダウンメニューで、 **承認**.\
   自分に割り当てられた承認や自分に委任された承認を含め、すべての承認がデフォルトでリストに表示されます。

   ![](assets/delegated-to-me-nwe-350x93.png)
