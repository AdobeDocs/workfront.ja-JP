---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: ワークストリームの管理
description: ワークストリームは、作業時の共同作業用に設定可能なボードとカードのグループです。
author: Lisa
feature: Agile
exl-id: c46c42e8-e14d-414d-b883-c4d885338e42
source-git-commit: 4e5bff5ad62dce8766072e04e3a2b89371a90f03
workflow-type: tm+mt
source-wordcount: '915'
ht-degree: 98%

---

# ワークストリームの管理

>[!IMPORTANT]
>
>ワークストリームは、特定の顧客グループのみが使用できます。

ワークストリームは、作業時の共同作業用に設定可能なボードとカードのグループです。ワークストリームには、テンプレートから作成された様々なタイプのボードと作業アイテムのカードリストを含めることができます。ワークストリームでは、イテレーションまたはスプリントで作業を追跡できます。

詳しくは、[カードリストを使用](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md)および[ワークストリームでイテレーションを作成](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md)を参照してください。

ワークストリームは、アクセスできる、ワークストリームの一部ではない個々のボードとともにダッシュボードに表示されます。ボードダッシュボードについて詳しくは、[ボードダッシュボードを使用](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md)を参照してください。ダッシュボード上の任意のボード名をクリックして開くことができます。

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

## ワークストリームを作成する

{{step1-to-boards}}

1. ダッシュボードの[!UICONTROL ワークストリーム]エリアで「**[!UICONTROL ワークストリームを追加]**」をクリックします。
1. 「**[!UICONTROL 名称未設定のワークストリーム]**」を置き換える名前を入力し、Enter キーを押します。

   ワークストリームにボードを追加するか、「[!UICONTROL **すべてのボード**]」をクリックして、ダッシュボードに戻ります。

## ワークストリーム内に新しいボードを作成する

1. まだワークストリームにない場合は、「[!UICONTROL **ワークストリームを表示**]」をクリックして、既存のワークストリームを開きます。
1. ワークストリームの「[!UICONTROL ボード]」タブで「**[!UICONTROL ボードを追加]**」をクリックします。
1. ボードのテンプレートを選択します。

| テンプレート | 説明 |
|---------|----------|
| 基本ボード | 3 つのデフォルトの列がボード上に表示されます。新しい列を追加し、デフォルトの列の名前を変更または削除できます。 <p>列ポリシーは適用されません。 |
| かんばんボード | バックログ、新規、処理中、完了、および保留中の各列がボードに表示されます。新しい列を追加し、デフォルトの列の名前を変更または削除できます。<p>バックログを使用するには、取り込み列にフィルターを設定する必要があります。詳しくは、[ボードに取り込み列を追加](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md)を参照してください。 <p>各列のデフォルトのポリシーを確認するには、列の「[!UICONTROL **その他**」メニュー]をクリックし、「[!UICONTROL **編集**]」を選択します。これらの事前設定ポリシーはいずれも変更できます。詳しくは、[ボード列を管理](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)を参照してください。 |
| レトロボード | ボードには次の列が用意されています：うまくいったこと。改善すべき点賞賛すべき対象迅速化のためにできること新しい列を追加し、デフォルトの列の名前を変更または削除できます。 <p>列ポリシーは適用されません。 |
| イテレーションプロセス | これは、イテレーションを定義して実行するために使用されるボードです。 <p>バックログ、新規、処理中、完了、および保留中の各列がボードに表示されます。ボードに列を追加することはできません。 <p>各列のデフォルトのポリシーを確認するには、列の「[!UICONTROL **その他**]」メニューをクリックし、「[!UICONTROL **編集**]」を選択します。これらの事前設定ポリシーはいずれも変更できます。詳しくは、[ボード列を管理](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)を参照してください。 |

ボードの設定について詳しくは、[ボードを作成または編集](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md)を参照してください。

## ワークストリーム上のボードのリストをフィルタリングする

デフォルト以外のフィルターがカードリストに適用されている場合、フィルターアイコン ![適用されたフィルター](assets/boards-filterapplied-30x30.png) にインジケーターが表示されます。すべてのフィルターを削除するには、「[!UICONTROL **すべてクリア**]」をクリックし、フィルターパネルを閉じるには、「[!UICONTROL **フィルターを非表示**]」をクリックします。

{{step1-to-boards}}

1. ダッシュボードで、「[!UICONTROL **ワークストリームを表示**]」をクリックして、ワークストリームを開きます。
1. まだ表示されていない場合は、「[!UICONTROL **ボード**]」タブをクリックします。
1. 「[!UICONTROL **フィルター**]」をクリックします。
1. ステータス別に表示するボードを選択します（アーカイブされたボード、アクティブなボード、またはすべてのボード）。
1. テンプレート別に表示するボードを選択します。

## ワークストリームにメンバーを追加する

ユーザーとチームは、ワークストリームとそのコンテンツを表示する前に、メンバーとしてワークストリームに追加する必要があります。ワークストリームメンバーは、ワークストリーム上でメンバーを追加および削除したり、ワークストリームにどのボードがあるかを確認したりできます。

>[!NOTE]
>
>ワークストリームメンバーは、その特定のボードにメンバーとして追加されるまで、ワークストリーム上のボードを開くことができません。

{{step1-to-boards}}

1. ダッシュボードで、「[!UICONTROL **ワークストリームを表示**]」をクリックして、ワークストリームを開きます。
1. **[!UICONTROL メンバーを追加]**&#x200B;アイコン ![メンバーを追加](assets/boards-addmember-spectrum-25x25.png) をクリックして、メンバーとチームをワークストリームに追加します。

   これは、ボードにメンバーを追加する場合と同じ手順です。詳しくは、[ボードのメンバーの追加または削除](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md)を参照してください。

## ワークストリームへのソースの追加

ソースは、ワークストリーム内のカードの送信元を決定します。

{{step1-to-boards}}

1. [!UICONTROL **ソース**]&#x200B;アイコン ![ソースアイコン](assets/sources-icon.png) をクリックして、ワークストリームにカードを読み込むソースを定義します。現時点では、利用可能なソースは [!DNL Adobe Workfront] のみです。
1. Workfront からタスクとイシューをカードとして読み込むためのフィルターを追加します。

   ワークストリームのソースにフィルターを追加することは、基本ボードまたはカンバンボードの取り込み列に詳細なフィルターを追加することと同じです。詳しくは、[ボードに取り込み列を追加する](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md)を参照してください。

## ワークストリームの設定

{{step1-to-boards}}

1. ダッシュボードで「[!UICONTROL **ワークストリームを表示**]」をクリックしてワークストリームを開きます。
1. 「[!UICONTROL **設定**]」をクリックして、[!UICONTROL ワークストリームの設定]パネルを開きます。
1. （オプション）[!UICONTROL **ワークストリーム**]&#x200B;を展開し、ワークストリームの説明を入力します。この説明は、ダッシュボードに表示されます。
1. （オプション）[!UICONTROL **イテレーション**]&#x200B;を展開し、ワークストリームの反復処理を定義します。

   カードの総数、指定されたカードの数、イテレーションの数が「カードリスト」セクションに表示されます。「[!UICONTROL **リストを表示**]」をクリックしてリストを開き、カードを追加します。詳しくは、[カードリストを使用](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md)を参照してください。

   イテレーションが既に定義されている場合は、開始日、カード数、ポイント数が表示されます。「[!UICONTROL **ボードを表示**]」をクリックして、イテレーションボードを開きます。詳しくは、[ワークストリームでのイテレーションの作成](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md)を参照してください。

1. （オプション）[!UICONTROL **タグ**]&#x200B;を展開し、ワークストリームにタグを追加します。タグを検索するか、検索ボックスに新しいタグ名を入力して Enter キーを押して作成します。
