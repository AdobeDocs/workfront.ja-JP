---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: ボードの作成または編集
description: 次の [!UICONTROL ボード] ダッシュボードを使用すると、新しいボードを作成したり、既存のボードを編集したりできます。
author: Lisa
feature: Agile
exl-id: 5f755177-c8ea-4509-a34f-57ffcfd8ba7f
source-git-commit: 966a88b8c7761b257a1ad0b2fdb3400f78c5d4f7
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# ボードの作成または編集

{{highlighted-preview}}

次の [!UICONTROL ボード] ダッシュボードを使用すると、新しいボードを作成したり、既存のボードを編集したりできます。

ワークストリームにボードを追加するには、 [ワークストリームの管理](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

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

## 新しいボードを作成

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL ボード]**.
1. スタンドアロンボードを作成するには、 **[!UICONTROL ボードを追加]** 内 [!UICONTROL ボード] 領域 ワークストリームにボードを追加するには、 [ワークストリームの管理](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-collections.md).

1. ボードのテンプレートを選択します。

   | テンプレート | 説明 |
   |---------|----------|
   | 基本ボード | 3 つのデフォルトの列がボード上に表示されます。 新しい列を追加し、デフォルトの列の名前を変更または削除できます。 <p>3 つのデフォルトの列がボード上に表示されます。 新しい列を追加し、デフォルトの列の名前を変更または削除できます。 |
   | かんばんボード | 次の列がボードに表示されます。「バックログ」、「新規」、「処理中」、「完了」、「保留中」。 新しい列を追加し、デフォルトの列の名前を変更または削除できます。<p>バックログを使用するには、取り込みカラムのフィルタを設定する必要があります。 詳しくは、 [ボードに吸気柱を追加する](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>各列のデフォルトのポリシーを確認するには、 [!UICONTROL **詳細** メニュー] 列で、 [!UICONTROL **編集**]. これらの事前設定済みポリシーは任意に変更できます。 詳しくは、 [ボード列を管理](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
   | レトロボード | 次の列がボードに表示されます。何が上手く行った？ 改善すべき点? お祝いすべき対象? 迅速化のためにできること? 新しい列を追加し、デフォルトの列の名前を変更または削除できます。 <p>列ポリシーは適用されません。 |
   | <span class="preview">動的なボード</span> | <span class="preview">次の列がボードに表示されます。未選択、新規、進行中、保留中、完了。 新しい列を追加し、デフォルトの列の名前を変更または削除できます。 (「未選択」列は、名前を変更できますが、削除はできません。 この列には、ステータスが他の列のステータスのどれとも一致しないすべてのカードが含まれます。) <p>デフォルトの列ポリシーでは、ステータスに基づいてカードが列に割り当てられます。 詳しくは、 [ボード列を管理](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).</span> |

1. <span class="preview">ダイナミックボードの場合のみ、セットアップウィザードの手順に従います。</span>

   <div class="preview">

   1. ボードの名前を入力し、 [!UICONTROL **次へ**].
   1. クリック [!UICONTROL **ソースを追加**].
   1. クリック [!UICONTROL **ソースをフィルター**] を選択し、 [!UICONTROL **タスク**] または [!UICONTROL **問題**].

      >[!NOTE]
      >
      >ボードをフィルタリングしてタスクとイシューの両方を含めることができますが、オブジェクトタイプごとに個別にフィルターを設定する必要があります。
      >
      >また、保存済みのフィルターとシステムのデフォルトのフィルターも選択できます。

   1. フィルターを作成して、ボードに接続されたカードとして取り込むオブジェクトを定義します。

      これは、吸気カラムにフィルタを作成するのと同じ手順です。 詳しくは、 [ボードに吸気柱を追加する](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

   1. フィルターを追加したら、 [!UICONTROL **ボードを作成**].

   </div>

1. ボードの名前を **[!UICONTROL ボード]** フィールドに入力し、Enter キーを押します。
1. 必要に応じて、ボードを設定します。

   詳しくは、 [ボードに対するメンバーの追加または削除](../../agile/get-started-with-boards/add-members-to-board.md), [ボード列を管理](../../agile/get-started-with-boards/manage-board-columns.md), [ボードへのアドホックカードの追加](../../agile/get-started-with-boards/add-card-to-board.md)、および [ボードでの接続済みカードの使用](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

1. クリック **[!UICONTROL すべてのボード]** をクリックして、ボードダッシュボードに戻ります。

   また、現在のボードの名前でラベル付けされたドロップダウンメニューを見つけ、それをクリックして別のボードに切り替えることもできます。

   ![ボードのリスト](assets/boards-button-list-of-boards-350x188.png)

## 既存のボードの編集

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL ボード]**.
1. ダッシュボードで、開くボードを選択します。
1. 必要に応じて、ボードを編集します。 ボード名をクリックして名前を変更できます。

   詳しくは、 [ボードに対するメンバーの追加または削除](../../agile/get-started-with-boards/add-members-to-board.md), [ボード列を管理](../../agile/get-started-with-boards/manage-board-columns.md)、および [ボードへのカードの追加](../../agile/get-started-with-boards/add-card-to-board.md).

1. クリック **[!UICONTROL すべてのボード]** をクリックして、ボードダッシュボードに戻ります。

   また、現在のボードの名前でラベル付けされたドロップダウンメニューを見つけ、それをクリックして別のボードに切り替えることもできます。
