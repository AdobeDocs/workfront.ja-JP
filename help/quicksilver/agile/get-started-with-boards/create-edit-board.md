---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: ボードを作成または編集
description: '[!UICONTROL ボード]ダッシュボードから、ボードを新規作成したり、既存のボードを編集したりすることができます。'
author: Lisa
feature: Agile
exl-id: 5f755177-c8ea-4509-a34f-57ffcfd8ba7f
source-git-commit: efe636e14964cc8705839c9f534a9947327803d7
workflow-type: tm+mt
source-wordcount: '824'
ht-degree: 91%

---

# ボードの作成または編集

<!-- Audited: 12/2023 -->

[!UICONTROL ボード]ダッシュボードから、ボードを新規作成したり、既存のボードを編集したりすることができます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> <p>新規：Contributor 以上 </p>
 <p>または</p> 
<p>現在：[!UICONTROL Request] 以上 </p> 
</td> 
  </tr>
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ボードを新規作成

{{step1-to-boards}}

1. 「**[!UICONTROL ボードを追加]**」をクリックします。

1. ボードのテンプレートを選択します。

   | テンプレート | 説明 |
   |---------|----------|
   | 基本ボード | 3 つのデフォルトの列がボード上に表示されます。新しい列を追加し、デフォルトの列の名前を変更または削除できます。 <p>3 つのデフォルトの列がボード上に表示されます。新しい列を追加し、デフォルトの列の名前を変更または削除できます。 |
   | かんばんボード | バックログ、新規、処理中、完了、および保留中の各列がボードに表示されます。新しい列を追加し、デフォルトの列の名前を変更または削除できます。<p>バックログを使用するには、取り込み列にフィルターを設定する必要があります。詳しくは、[ボードに取り込み列を追加](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md)を参照してください。 <p>各列のデフォルトのポリシーを確認するには、列の「[!UICONTROL **その他**」メニュー]をクリックし、「[!UICONTROL **編集**]」を選択します。これらの事前設定ポリシーはいずれも変更できます。詳しくは、[ボード列を管理](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)を参照してください。 |
   | レトロボード | ボードには次の列が用意されています：うまくいったこと。改善すべき点賞賛すべき対象迅速化のためにできること新しい列を追加し、デフォルトの列の名前を変更または削除できます。 <p>列ポリシーは適用されません。 |
   | 動的なボード | ボードには、未選択、新規、処理中、保留中および完了の列が表示されます。新しい列を追加し、デフォルトの列の名前を変更または削除できます。（未選択の列は、名前を変更できますが、削除はできません。この列には、他のどの列のステータスとも一致しないステータスを持つすべてのカードがが保持されます。) <p>デフォルトの列ポリシーでは、ステータスに基づいてカードが列に割り当てられます。詳しくは、[ボード列を管理](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)を参照してください。 |

1. 動的なボードの場合のみ、セットアップウィザードの手順に従います。

   1. ボードの名前を入力して「[!UICONTROL **次へ**]」をクリックします。
   1. [!DNL Workfront] [!UICONTROL **プロジェクト**]&#x200B;を検索して選択し、タスクとイシューをボードに取り込みます。
   1. [!UICONTROL **割り当て**]&#x200B;を検索として選択し、タスクとイシューをボードに取り込みます。

      すべてのオブジェクトは、接続されたカードとしてボード上に表示されます。

      [!UICONTROL **追加中のカード**]&#x200B;カウンターは、ボードに表示されるカードの数を示します。例えば、100 個のタスクとイシューを含むプロジェクトを選択した場合、カウンターには 100 と表示されます。ユーザー割り当てを追加し、そのユーザーがプロジェクトにある 5 つのタスクに割り当てられている場合、カウンターには 5 と表示されます。

      >[!NOTE]
      >
      >ダイナミックボードのカード上限は、700 件のタスクと 700 件のイシューで、合計 1,400 枚のカードです。ボード上のカード数が多いと、ボードのパフォーマンスに影響を与える可能性があります。 アーカイブされたすべてのカードは、非表示と表示の両方で、この制限にカウントされます。

   1. （オプション）「[!UICONTROL **完了したカードをアーカイブしない**]」を選択すると、ボード上に完了したタスクとイシューが「完了」列にカードとして表示されます。このオプションを選択しない場合、ボード作成時に完了したカードは、アーカイブされたカードとしてボードに取り込まれます。

      >[!NOTE]
      >
      >デフォルトでは、アーカイブされたカードは、ボード上に表示されません。アーカイブされたカードを表示するには、構成設定をオンにしてから、ボードをフィルタリングして、アーカイブされたカードを表示する必要があります。詳しくは、[カードに表示するフィールドのカスタマイズ](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md)と[ボード内でのフィルターと検索](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md)を参照してください。

   1. （オプション）「[!UICONTROL **詳細フィルターの使用**]」をクリックして、追加のフィルターオプションを表示します。

      これは、取り込み列にフィルターを作成するのと同じ手順です。詳しくは、[ボードに取り込み列を追加する](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md)を参照してください。

      動的ボードを作成した後に動的ボードのフィルターを更新すると、Workfrontのタスクまたはイシューに含まれていないカード設定（タグなど）はリセットされます。

   1. フィルターを追加したら、[!UICONTROL **ボードを作成**]&#x200B;を参照してください。

1. ボードの名前を&#x200B;**[!UICONTROL ボード]**&#x200B;フィールドに入力し、Enter キーを押します。
1. 必要に応じて、ボードを設定します。

   詳しくは、[ボードに対するメンバーの追加または削除](../../agile/get-started-with-boards/add-members-to-board.md)、[ボード列を管理](../../agile/get-started-with-boards/manage-board-columns.md)、[ボードへのアドホックカードの追加](../../agile/get-started-with-boards/add-card-to-board.md)、および[ボードでの接続済みカードの使用](/help/quicksilver/agile/get-started-with-boards/connected-cards.md)を参照してください。

1. **[!UICONTROL すべてのボード]**&#x200B;をクリックして、ボードダッシュボードに戻ります。

   また、現在のボードの名前でラベル付けされたドロップダウンメニューを検索し、クリックして別のボードに切り替えることもできます。

   ![ボードのリスト](assets/boards-button-list-of-boards-350x188.png)

## 既存のボードの編集

{{step1-to-boards}}

1. ダッシュボードで、ボードを選択して開きます。
1. 必要に応じて、ボードを編集します。ボード名をクリックして名前を変更できます。

   詳しくは、[ボードに対するメンバーの追加または削除](../../agile/get-started-with-boards/add-members-to-board.md)、[ボード列を管理](../../agile/get-started-with-boards/manage-board-columns.md)、および[ボードへのカードの追加](../../agile/get-started-with-boards/add-card-to-board.md)を参照してください。

1. 「**[!UICONTROL すべてのボード]**」をクリックして、ボードダッシュボードに戻ります。

   また、現在のボードの名前でラベル付けされたドロップダウンメニューを検索し、クリックして別のボードに切り替えることもできます。

