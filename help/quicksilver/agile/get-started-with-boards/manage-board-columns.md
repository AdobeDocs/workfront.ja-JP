---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: ボードの列の管理
description: 新しいボードには、デフォルトで 3 つの列が含まれています。列の追加、列の順序の変更、列の名前の変更、不要な列の削除を行うことができます。
author: Lisa
feature: Agile
exl-id: a736cdfe-5ddc-4bf4-82a1-a78d16c0d70b
source-git-commit: 8097842fedb468d8f0e5c9eed94bf74d489edd2b
workflow-type: tm+mt
source-wordcount: '934'
ht-degree: 97%

---

# ボードの列の管理

新しいボードには、デフォルトで 3 つの列が含まれています。列の追加、列の順序の変更、列の名前の変更、不要な列の削除を行うことができます。

列設定にはポリシーが含まれ、カードをその列に移動したときにカードがどうなるかに関するオプションを定義できます。

列でのカードの並べ替えについて詳しくは、[ボード内でのフィルターと検索](/help/quicksilver/agile/get-started-with-boards/filter-search-in-board.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] プラン*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] ライセンス*</strong></td> 
   <td> <p>[!UICONTROL Request] 以降</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプ、アクセスを確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## ボードに列を追加

1. [!DNL Adobe Workfront] の右上隅にある&#x200B;**[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) をクリックし、次に「**[!UICONTROL ボード]**」をクリックします。
1. ボードにアクセスします。詳しくは、[ボードの作成または編集](../../agile/get-started-with-boards/create-edit-board.md)を参照してください。
1. 存在する列の右側にある「**[!UICONTROL 列を追加]**」をクリックします。
1. 新しい列に名前を入力し、「**[!UICONTROL 列を追加]**」をクリックします。

   ![新しい列を追加](assets/boards-add-column.png)

>[!TIP]
>
>取り込み列を追加するには、[ボードに取り込み列を追加](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md)を参照してください。

## ボード上の列の並べ替え

1. ボードにアクセスします。
1. 列を正しい順序にドラッグ＆ドロップします。列を別の場所にドラッグする前に、列の上部を必ず選択してください。

   ![列をドラッグ＆ドロップ](assets/boards-dragdropcolumn.png)

## ボード列の名前の変更

1. ボードにアクセスします。
1. 列名をクリックし、新しい名前を入力して、Enter キーを押します。

   または

   列上の&#x200B;**[!UICONTROL 詳細]**&#x200B;メニュー![詳細メニュー](assets/more-icon-spectrum.png)をクリックして、「**[!UICONTROL 編集]**」を選択します。設定エリアで、新しい名前を「**[!UICONTROL 列名]**」フィールドに入力して、「**[!UICONTROL 閉じる]**」をクリックします。

## ボード列の削除

ボードから列を削除した場合、その列は復元できません。

1. ボードにアクセスします。
1. 列上の&#x200B;**[!UICONTROL 詳細]**&#x200B;メニュー![詳細メニュー](assets/more-icon-spectrum.png)をクリックして、「**[!UICONTROL 削除]**」を選択します。

   >[!NOTE]
   >
   >アーカイブされたカードを含むカードを含む列は削除できません。カードを含む列を削除する場合は、それらのカード用に別の列を選択する必要があります。

## カードカウントの表示

設定を使用して、各列にあるカードの数を表示できます。

ある列に WIP 制限を使用している場合、別のカードカウンターは追加されません。WIP 制限について詳しくは、[ボード上での[!UICONTROL 進行中の作業]（WIP）制限の管理](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md)を参照してください。

1. ボードにアクセスします。
1. ボードの右側の「**[!UICONTROL 設定]**」をクリックして、設定パネルを開きます。
1. 「**[!UICONTROL 列]**」を展開します。
1. 「**[!UICONTROL 列カードのカウントを表示]**」をオンにします。

   ![カードカウンターをオンにする](assets/display-card-count.png)

   各列の上部にカードカウンターが表示されます。

1. 「**[!UICONTROL 設定を非表示]**」をクリックして「[!UICONTROL 設定]」パネルを閉じます。

## 列設定とポリシーの定義

1. ボードにアクセスします。
1. 列上の&#x200B;**[!UICONTROL 詳細]**&#x200B;メニュー ![詳細メニュー](assets/more-icon-spectrum.png) をクリックしてから、「**[!UICONTROL 編集]**」を選択します。

   「[!UICONTROL 設定]」エリアが表示されます。「**[!UICONTROL 列名]**」を見ると、設定を定義する列がわかります。

1. 「**[!UICONTROL 自動的にフィールドの値を更新]**」ポリシーを有効にします。これにより、カードがこの列に移動されたときに、特定のフィールド値が自動的に変更されます。

   ![列設定とポリシー](assets/boards-column-policies-enabled.png)

1. （オプション）カードのステータスの値を設定します。

   1. 「**[!UICONTROL ステータス]**」チェックボックスを選択します。

   1. カードがこの列に移動されたときにカードに適用するステータスを選択します。

      ![列のステータス](assets/boards-column-status.png)

      接続されたカードのステータス変換オプションも表示されます。（ステータス変換は、アドホックカードには適用されません）。これらのオプションは、接続されたカードがこの列に移動されたときに [!DNL Workfront] のタスクまたはイシューに適用されるカスタムステータスを決定します。

   1. タスクおよびイシューのカードに適用する「[!UICONTROL **カスタム**]」ステータスを選択します。

      カードがこの列に移動されたとき、[!DNL Workfront] は最初に、カスタムステータス（「解決済み」など）の適用を試みます。選択したカスタムステータスがそのカードで使用できない場合は、システムステータスに対応する別のステータスを選択するよう求められます（上記の手順 b）。ステータスについて詳しくは、[ステータスの概要](/help/quicksilver/administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/statuses-overview.md)を参照してください。

      また、接続されたタスクまたはイシューのステータスが列ポリシーで設定されたカスタムステータスまたはシステムステータスに変更された場合、カードは自動的に列に移動します。

1. （オプション）カードの割り当て先の値を設定します。

   1. 「**[!UICONTROL 割り当て先]**」チェックボックスを選択します。
   1. アクションを選択します。

      * **[!UICONTROL 割り当て先に追加]：**&#x200B;カードをこの列に移動したときに、選択した割り当て先が、カード上の既存の割り当て先リストに追加されます。
      * **[!UICONTROL 割り当て先を上書き]：**&#x200B;カードをこの列に移動したときに、選択した割り当て先が他のすべての割り当て先を上書きし、カード上の唯一の割り当て先になります。

   1. クリック [!UICONTROL **割り当てを追加**] ユーザーを検索します。 検索結果から担当者を選択します。 すべてのWorkfrontユーザーおよびチームは、から選択できます。

      ![列の割り当て先](assets/boards-column-assignees.png)

1. （オプション）カードタグの値を設定します。

   1. 「**[!UICONTROL カード]**」チェックボックスを選択します。
   1. アクションを選択します。

      * **[!UICONTROL タグに追加]：**&#x200B;カードをこの列に移動したときに、選択したタグが、カード上の既存のタグリストに追加されます。
      * **[!UICONTROL タグを上書き]：**&#x200B;カードをこの列に移動したときに、選択したタグが他のすべてのタグを上書きし、カード上の唯一のタグになります。

   1. ドロップダウンリストからタグを選択します。[!UICONTROL タグマネージャー]で既に作成されているタグのみが選択可能です。新しいタグの追加について詳しくは、[タグを追加](/help/quicksilver/agile/get-started-with-boards/add-tags.md)を参照してください。

      ![列のタグ](assets/boards-column-tags.png)

1. 「**[!UICONTROL 処理中の作業の制限]**」ポリシーを有効にして、列に追加できるカードの数を制限します。次に、制限値を「**[!UICONTROL 制限を設定]**」フィールドに入力します。

   ![列の WIP 制限](assets/boards-wip-limit-in-column.png)

   詳しくは、[ボードでの進行中の作業（WIP）の上限の管理](/help/quicksilver/agile/use-boards-agile-planning-tools/manage-wip-limit-on-board.md)を参照してください。

1. 「**[!UICONTROL 閉じる]**」をクリックして「設定」エリアを終了し、列とそのカードを表示します。
