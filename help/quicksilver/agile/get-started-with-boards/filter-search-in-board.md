---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: ボードでのフィルターと検索
description: ボードをフィルタリングして、特定のカードのみを表示できます。
author: Lisa
feature: Agile
exl-id: 26abce82-dcd9-4865-96f4-c710f7f0a0d8
source-git-commit: 05cac2441474e0f6ecf18aa777a5a66fefb2dba8
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 0%

---

# ボードでのフィルターと検索

{{highlighted-preview}}

ボードをフィルタリングして表示できます。

* 特定のユーザーに割り当てられたカード
* 特定のタグを含むカード
* 特定のステータスを持つカード
* 特定の期間内に期限が切れるカード
* アーカイブしたカード
* 特定のプロジェクトに接続されたカード

<span class="preview">ボードの並べ替えは、列のすべてのカードを並べ替えます。 1 つの列を並べ替えることはできません。また、backlog 列または intake 列は並べ替えられません。</span>

検索は、ボード上の特定のカードを探すのにも役立ちます。

フィルターを適用すると、ボードにインジケーターが表示されます ![ボードに適用するフィルター](assets/boards-filterapplied-30x30.png). クリック **[!UICONTROL すべてクリア]** すべてのフィルタをボードから削除するには、をクリックします。 **[!UICONTROL フィルターを非表示]** をクリックして、フィルターパネルを閉じます。

![フィルターパネル](assets/boards-all-filters-collapsed-1022.png)

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] 計画*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL リクエスト ] 以降</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスの種類、アクセス権を確認するには、 [!DNL Workfront] 管理者。

## 割り当て先によるボードのフィルタリング

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL ボード]**.
1. ボードにアクセスします。 詳しくは、 [ボードの作成または編集](../../agile/get-started-with-boards/create-edit-board.md).
1. クリック [!UICONTROL **フィルター**]、を展開します。 [!UICONTROL メンバー] 」セクションに移動し、表示する 1 人または複数のカードを持つユーザーを選択します。 未割り当てのカードを表示することもできます。

   ![メンバーでフィルター](assets/boards-filter-by-assignees-0822.png)

## タグでボードをフィルター

1. ボードにアクセスします。
1. クリック [!UICONTROL **フィルター**]、を展開します。 [!UICONTROL タグ] 」セクションで、表示するタグを選択します。

   ![タグでフィルター](assets/boards-filter-by-tags-0822.png)

## ステータスでボードをフィルター

1. ボードにアクセスします。
1. クリック [!UICONTROL **フィルター**]、を展開します。 [!UICONTROL ステータス] 」セクションで、表示するステータスのタイプを選択します。

   完成したカードを非表示にすることもできます。

   ![ステータスでフィルター](assets/boards-filter-by-status-0822.png)

## 期限別にボードをフィルター

1. ボードにアクセスします。
1. クリック [!UICONTROL **フィルター**]、を展開します。 [!UICONTROL 期限] 」セクションで、表示する日付オプションを選択します。

   選択した日付範囲のカードのみが表示されます。

   ![期限でフィルター](assets/boards-filter-by-due-date-0822.png)

## ボードをフィルターしてアーカイブされたカードを表示

デフォルトでは、アクティブなカードのみがボードに表示されます。 ボードをフィルタリングして、アーカイブしたカードも表示できます。

1. ボードにアクセスします。
1. クリック [!UICONTROL **フィルター**]、を展開します。 [!UICONTROL アーカイブ済みカード] セクションを選択し、 **[!UICONTROL アーカイブしたカード]** アーカイブされたカードを表示します。

   フィルターには、アーカイブされたカードの数が表示されます。

   ![アーカイブしたカードのフィルタリング](assets/boards-filter-by-archived-cards_0822.png)

1. 選択 **[!UICONTROL アーカイブしたカード]** を再びクリアし、アクティブなカードのみを表示します。

## ボードを接続でフィルター

1. ボードにアクセスします。
1. クリック [!UICONTROL **フィルター**]、を展開します。 [!UICONTROL 接続] セクションで、 [!DNL Workfront] 表示する接続済みカードのプロジェクトです。

   また、プロジェクトに接続されていないカードを表示することもできます。

   ![接続でフィルター](assets/boards-filter-by-connection.png)

<div class="preview">

## ボードでの並べ替え

並べ替えの基準となるオプションを選択すると、すべての列が並べ替えられます。 1 つの列を並べ替えることはできません。また、backlog 列または intake 列は並べ替えられません。

1. ボードにアクセスします。
1. クリック [!UICONTROL **並べ替え基準**] を選択し、 [!UICONTROL **名前**], [!UICONTROL **期限**], [!UICONTROL **推定**], [!UICONTROL **ステータス**]&#x200B;または [!UICONTROL **接続**].

   接続（プロジェクト名）は、接続されたカードにのみ適用され、その他のオプションは、接続されたカードとアドホックカードの両方を列で並べ替えます。

   「ユーザーの順序」オプションは、他の並べ替えオプションが適用される前に、手動で設定された順序にカードを返します。 列のデフォルトの並べ替えです。

1. 選択 [!UICONTROL **逆順**] をクリックして、並べ替えオプションの逆の順序で列を並べ替えます。

   並べ替えアイコンの矢印は、列が昇順または降順のどちらで並べ替えられているかを示します。

   デフォルト以外の並べ替えが適用されると、並べ替えアイコンにインジケーターが表示されます ![適用された並べ替え](assets/sort-applied-boards.png).

   ![ボード上の列で並べ替え](assets/sort-by-columns-in-board.png)

</div>

## ボードでの検索

1. ボードにアクセスします。
1. クリック [!UICONTROL **検索**] 検索語句を入力します。 次に、Enter キーを押します。

   検索語句を含むすべてのカードが表示されます。

   「 X 」をクリックして検索をクリアします。

   ![ボード内のカードの検索](assets/boards-searchbox.png)
