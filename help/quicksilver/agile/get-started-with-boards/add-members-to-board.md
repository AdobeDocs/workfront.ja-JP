---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: ボードからのメンバーの追加または削除
description: ユーザーがボードを表示したりカードに割り当てられたりする前に、ボードにメンバーとして追加する必要があります。
author: Lisa
feature: Agile
exl-id: 8a46846c-f9b8-45cb-9923-e7596854557b
source-git-commit: bf8d566ba9d24310e75d2fbaf523fe5464bb6657
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 60%

---

# ボードへのメンバーの追加または削除

{{highlighted-preview}}

ボードを表示できるようにするには、まず人物とチームをボードにメンバーとして追加する必要があります。

ボードの作成者は、デフォルトでは所有者です。 設定パネルでそのボードを削除したりフィルターを更新したりできるのは、ボードの所有者のみです。 <span class="preview"> ボード所有者を変更できるのは、システム管理者または現在のボード所有者のみです。</span>

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront]</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> 
   <p>新規：[!UICONTROL Contributor]以上</p> 
   <p>または</p>
   <p>現在：[!UICONTROL Request] 以上</p>
   </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ボードへのメンバーの追加

{{step1-to-boards}}

1. 新しいボードを作成するか、既存のボードを編集します。詳しくは、[ボードの作成または編集](../../agile/get-started-with-boards/create-edit-board.md)を参照してください。
1. **[!UICONTROL メンバーを追加]**&#x200B;アイコン ![メンバーを追加](assets/boards-addmember-spectrum-25x25.png) をクリックします。
1. 「**[!UICONTROL メンバーを追加]**」ボックスに名前を入力し、リストに表示されたら選択します。

   個々のメンバーまたはチームを選択できます。チームを選択すると、そのチームがボードに追加されます。

   >[!NOTE]
   >
   >ボードを表示するには、個々のユーザーは、「**[!UICONTROL 表示]**」または「**[!UICONTROL 編集]**」オプションをチームのアクセスレベルに設定する必要があります。


   ![ボードへのメンバーの追加](assets/boards-add-members.png)

## ボードからのメンバーの削除

{{step1-to-boards}}

1. 新しいボードを作成するか、既存のボードを編集します。詳しくは、[ボードの作成または編集](../../agile/get-started-with-boards/create-edit-board.md)を参照してください。
1. **[!UICONTROL メンバーを追加]**&#x200B;アイコン ![メンバーを追加](assets/boards-addmember-spectrum-25x25.png) をクリックします。
1. 「**[!UICONTROL メンバーを追加]**」ボックスで、個人名またはチーム名の横にある「X」をクリックして、ボードから削除します。

   ![ボードからのメンバーの削除](assets/boards-remove-member-from-board-350x367.png)

   ボードからメンバーを削除すると、そのメンバーは割り当てられていたカードから削除されます。接続されたカードの場合は、割り当ても [!DNL Workfront] タスクまたはイシューで更新されます。

   メンバーはこのボードからのみ削除されます。属している他のボードからは削除されません。

   >[!NOTE]
   >
   >ボードの所有者を削除することはできません。

<div class="preview">

## ボードの所有者の変更

>[!NOTE]
>
>システム管理者または現在のボード所有者のみがボード所有者を変更できます。 1 つのボードに設定できる所有者は 1 つだけです。
>
>ボード所有者を変更する機能は、基本、遡及、かんばんボードで使用できますが、動的なボードでは使用できません。

1. ボードにアクセスします。
1. ボード名の横にある **[!UICONTROL その他]** メニュー ![ その他メニュー ](assets/more-icon-spectrum.png) をクリックし、「**[!UICONTROL ボード所有者を変更]**」を選択します。
1. ボード所有者を変更ダイアログボックスで、所有者にするユーザーを検索して選択します。

   既にボードのメンバーになっているユーザーを検索することはできません。 既存のメンバーを所有者にするには、まずボードから削除する必要があります。 ユーザーをボードの所有者にすると、ユーザーはボードに追加されます。

   ボードの所有者にできるのはユーザーのみです。 チームは所有者にできません。

1. 「[!UICONTROL **更新**]」をクリックします。

</div>
