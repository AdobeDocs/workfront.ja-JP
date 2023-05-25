---
content-type: reference
product-area: agile-and-teams
navigation-topic: boards
title: ワークストリームの管理
description: ワークストリームは、作業時の共同作業用に設定可能なボードとカードのグループです。
author: Lisa
feature: Agile
exl-id: c46c42e8-e14d-414d-b883-c4d885338e42
source-git-commit: dd1bd5a27a2ed29af29b88b028d8fd34a592aae2
workflow-type: tm+mt
source-wordcount: '905'
ht-degree: 2%

---

# ワークストリームの管理

ワークストリームは、作業時の共同作業用に設定可能なボードとカードのグループです。 ワークストリームには、テンプレートから作成された様々なタイプのボードや、作業項目のカードリストが含まれる場合があります。 ワークストリームでは、繰り返しまたはスプリントで作業を追跡できます。

詳しくは、 [カードリストを使用](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md) および [ワークストリームでの反復の作成](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

ワークストリームは、ワークストリームに含まれない個々のボードと共に、ダッシュボードに表示されます。 ボードダッシュボードについて詳しくは、 [ボードダッシュボードの使用](/help/quicksilver/agile/get-started-with-boards/use-boards-page.md). ダッシュボード上の任意のボード名をクリックして開くことができます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
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

## ワークストリームの作成

{{step1-to-boards}}

1. クリック **[!UICONTROL ワークストリームを追加]** 内 [!UICONTROL ワークストリーム] 領域に表示されます。
1. 置き換える名前を入力 **[!UICONTROL 名称未設定のワークストリーム]** をクリックし、Enter キーを押します。

   ワークストリームにボードを追加するか、 [!UICONTROL **すべてのボード**] をクリックして、ダッシュボードに戻ります。

## ワークストリーム内に新しいボードを作成します

1. まだワークストリームにない場合は、 [!UICONTROL **ワークストリームを表示**] をクリックして、既存のワークストリームを開きます。
1. クリック **[!UICONTROL ボードを追加]** の [!UICONTROL ボード] 」タブをクリックします。
1. ボードのテンプレートを選択します。

| テンプレート | 説明 |
|---------|----------|
| 基本ボード | 3 つのデフォルトの列がボード上に表示されます。 新しい列を追加し、デフォルトの列の名前を変更または削除できます。 <p>列ポリシーは適用されません。 |
| かんばんボード | 次の列がボードに表示されます。「バックログ」、「新規」、「処理中」、「完了」、「保留中」。 新しい列を追加し、デフォルトの列の名前を変更または削除できます。<p>バックログを使用するには、取り込みカラムのフィルタを設定する必要があります。 詳しくは、 [ボードに吸気柱を追加する](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md). <p>各列のデフォルトのポリシーを確認するには、 [!UICONTROL **詳細** メニュー] 列で、 [!UICONTROL **編集**]. これらの事前設定済みポリシーは任意に変更できます。 詳しくは、 [ボード列を管理](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |
| レトロボード | 次の列がボードに表示されます。何が上手く行った？ 改善すべき点? お祝いすべき対象? 迅速化のためにできること? 新しい列を追加し、デフォルトの列の名前を変更または削除できます。 <p>列ポリシーは適用されません。 |
| イテレーションプロセス | これは、反復を定義して実行するために使用されるボードです。 <p>次の列がボードに表示されます。「バックログ」、「新規」、「処理中」、「完了」、「保留中」。 ボードに列を追加することはできません。 <p>各列のデフォルトのポリシーを確認するには、 [!UICONTROL **詳細**] 列のメニューで「 」を選択し、 [!UICONTROL **編集**]. これらの事前設定済みポリシーは任意に変更できます。 詳しくは、 [ボード列を管理](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md). |

ボードの設定について詳しくは、 [ボードの作成または編集](/help/quicksilver/agile/get-started-with-boards/create-edit-board.md).

## ワークストリーム上のボードのリストをフィルター

既定以外のフィルタがボードリストに適用されると、フィルタアイコンにインジケータが表示されます ![適用されたフィルター](assets/boards-filterapplied-30x30.png). クリック [!UICONTROL **すべてクリア**] すべてのフィルタを削除するには、をクリックします。 [!UICONTROL **フィルターを非表示**] をクリックして、フィルターパネルを閉じます。

{{step1-to-boards}}

1. ダッシュボードで、 [!UICONTROL **ワークストリームを表示**] をクリックして、ワークストリームを開きます。
1. 次をクリック： [!UICONTROL **ボード**] タブが表示されていない場合は、「 」タブをクリックします。
1. クリック [!UICONTROL **フィルター**].
1. ステータス別に表示するボードを選択します（アーカイブされたボード、アクティブなボード、またはすべてのボード）。
1. テンプレート別に表示するボードを選択します。

## ワークストリームにメンバーを追加

ユーザーとチームは、ワークストリームとそのコンテンツを表示する前に、メンバーとしてワークストリームに追加する必要があります。 ワークストリームメンバは、ワークストリーム上のメンバを追加および削除し、ワークストリーム内のどのボードがあるかを確認することができます。

>[!NOTE]
>
>ワークストリームメンバは、その特定のボードにメンバーとして追加されるまで、ワークストリーム上のボードを開くことができません。

{{step1-to-boards}}

1. ダッシュボードで、 [!UICONTROL **ワークストリームを表示**] をクリックして、ワークストリームを開きます。
1. 次をクリック： **[!UICONTROL メンバーを追加]** アイコン ![メンバーを追加](assets/boards-addmember-spectrum-25x25.png) をクリックして、メンバーとチームをワークストリームに追加します。

   これは、ボードにメンバーを追加する場合と同じ手順です。 詳しくは、 [ボードに対するメンバーの追加または削除](/help/quicksilver/agile/get-started-with-boards/add-members-to-board.md).

## ワークストリームへのソースの追加

ソースは、ワークストリーム内のカードの送信元を決定します。

{{step1-to-boards}}

1. 次をクリック： [!UICONTROL **ソース**] アイコン ![ソースアイコン](assets/sources-icon.png) ：カードをワークストリームにインポートするソースを定義します。 現時点では、次のソースのみが利用可能です。 [!DNL Adobe Workfront].
1. タスクとイシューをWorkfrontからカードとして読み込むためのフィルターを追加しました。

   ワークストリームソースに対するフィルタの追加は、基本ボードまたはかんばんボードの取り込みカラムに対する詳細フィルタの追加と同じです。 詳しくは、 [ボードに吸気柱を追加する](/help/quicksilver/agile/use-boards-agile-planning-tools/add-intake-column-to-board.md).

## ワークストリームの設定

{{step1-to-boards}}

1. ダッシュボードで、 [!UICONTROL **ワークストリームを表示**] をクリックして、ワークストリームを開きます。
1. クリック [!UICONTROL **設定**] 開く [!UICONTROL ワークストリームの設定] パネル。
1. （オプション）展開 [!UICONTROL **Workstream**] ワークストリームの説明を入力します。 この説明は、ダッシュボードに表示されます。
1. （オプション）展開 [!UICONTROL **反復**] を使用して、このワークストリームの反復処理を定義します。

   カードの総数、指定されたカードの数、繰り返し回数が「カードリスト」セクションに表示されます。 クリック [!UICONTROL **リストを表示**] をクリックしてリストを開き、カードを追加します。 詳しくは、 [カードリストを使用](/help/quicksilver/agile/use-boards-agile-planning-tools/use-card-list.md).

   イテレーションが既に定義されている場合は、開始日、カード数、ポイント数が表示されます。 クリック [!UICONTROL **ボードを表示**] をクリックして、イテレーションボードを開きます。 詳しくは、 [ワークストリームでの反復の作成](/help/quicksilver/agile/use-boards-agile-planning-tools/create-an-iteration-in-workstream.md).

1. （オプション）展開 [!UICONTROL **タグ**] をクリックして、ワークストリームにタグを追加します。 タグを検索するか、検索ボックスに新しいタグ名を入力し、Enter キーを押して作成します。
