---
product-area: agile-and-teams;projects
navigation-topic: work-in-an-agile-environment
title: アジャイル ストーリーを移動
description: アジャイルストーリーは、別のイテレーション（スクラムチームの場合）またはバックログ（かんばんチームとスクラムチームの場合）に移動できます。
author: Lisa
feature: Agile
exl-id: 0058792e-66b8-4e54-8ce3-50171adff875
source-git-commit: 685177d3a8485aa60d8455e1c329de21cea4abb7
workflow-type: tm+mt
source-wordcount: '349'
ht-degree: 70%

---

# アジャイルストーリーの移動

アジャイルストーリーは、別のイテレーション（スクラムチームの場合）またはバックログ（かんばんチームとスクラムチームの場合）に移動できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>標準</p> 
   <p>ワークまたはそれ以上</p> </td> 
  </tr>
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td>ストーリーへのアクセスの管理</td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## イテレーションまたはかんばんボードからバックログにストーリーを移動

1. バックログに移動するストーリーが含まれる、イテレーションまたはかんばんボードに移動します。
1. ページ上部にあるイテレーションの見出しをクリックします。
1. 「**[!UICONTROL ストーリー]**」タブで、移動するストーリーを選択します。
1. **[!UICONTROL 詳細]**/**[!UICONTROL 移動先]** をクリックします。 **[!UICONTROL 移動先]** ダイアログボックスが表示されます。

   ![ストーリーを移動ダイアログ](assets/iteration-story-move.png)

1. **team_name のバックログ** を選択します。 上記の例では、チーム名は **マーケティング** です。

1. 「**[!UICONTROL 移動]**」をクリックします。

## ストーリーを別のイテレーションに移動

システム管理者またはイテレーションが関連付けられているチームのメンバーであれば、スクラムチームの別のイテレーションにストーリーを移動できます。

>[!NOTE]
>
> 「**[!UICONTROL 指定の場所に移動]**」オプションは、イテレーションの親ストーリーには使用できません。サブタスクは別のイテレーションにのみ移動できます。


1. 移動するストーリーを含むイテレーションに移動します。
1. ページ上部にあるイテレーションの見出しをクリックします。
1. 「**[!UICONTROL ストーリー]**」タブで、移動するストーリーを選択します。
1. **[!UICONTROL 詳細]**/**[!UICONTROL 移動先]** をクリックします。 **[!UICONTROL 移動先]** ダイアログボックスが表示されます。

   ![ストーリーを移動ダイアログ](assets/iteration-story-move.png)

1. **[!UICONTROL 別のイテレーション]** を選択します。
1. 表示されるドロップダウンメニューで、ストーリーの移動先のイテレーションを選択します。

   >[!NOTE]
   >
   >作業アイテムの[!UICONTROL 予定開始日]と[!UICONTROL 予定完了日]は、[!UICONTROL チームを編集]ページの設定の影響を受けます。詳しくは、[スクラムの設定](../../agile/get-started-with-agile-in-workfront/configure-scrum.md)の記事で[[!UICONTROL 作業アイテムをイテレーションに追加する際に日付を適用する方法の設定]](../../agile/get-started-with-agile-in-workfront/configure-scrum.md#configure-how-dates-are-applied-when-adding-work-items-to-an-iteration)を参照してください。

1. 「**[!UICONTROL 移動]**」をクリックします。
