---
content-type: reference
navigation-topic: boards
title: アジャイルチームのかんばんカードの Workfront ボードへの移行
description: 作業アイテムをアジャイルチームかんばんボードから新規または既存の Workfront ボードに移行できます。
author: Lisa
feature: Agile
exl-id: c40b6453-5869-437b-a1e0-f20dd833d2b8
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: ht
source-wordcount: '362'
ht-degree: 100%

---

# アジャイルチームのかんばんカードの Workfront ボードへの移行

作業アイテムをアジャイルチームかんばんボードから新規または既存の Workfront ボードに移行できます。移行を実行すると、かんばんボード上のすべてのカードが Workfront ボードにコピーされます。特定のカードを選択することはできません。

Workfront ボードでのカードの配置は、列ポリシーに基づいています。（例えば、ポリシーを使用すると、ステータスが「処理中」のすべてのカードを特定の列に移動できます。列ポリシーについて詳しくは、[ボード列を管理](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)を参照してください。）ポリシーがない場合や、カードがポリシーと一致しない場合、カードはボードの左端の列に配置されます。現時点では、レガシーボードのバックログ列のカードは Workfront ボードに追加されません。

カードはアジャイルチームかんばんボードからは削除されず、カードの状態の変更は両方のボードに同期します。Workfront ボードに切り替える準備が整うまで、両方のボードをアクティブにしておくことができます。

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

## かんばんカードを新しいボードに移行する

{{step1-to-team}}

1. かんばんボードにアクセスします。
1. 「[!UICONTROL **ボードに追加**]」をクリックして、「[!UICONTROL **新しいボード**]」を選択します。
1. [!UICONTROL 新しいボードに追加]ダイアログで、新しいボードの名前を入力し（現在の[!UICONTROL かんばん]ボードの名前が自動的に表示されます）、「[!UICONTROL **追加**]」をクリックします。

   ![新しいボードにかんばんカードを追加](assets/add-kanban-cards-to-new-board-dialog.png)

1. （オプション）表示される成功メッセージで、リンクをクリックして新しいボードを開きます。

## かんばんカードを既存のボードに移行する

{{step1-to-team}}

1. かんばんボードにアクセスします。
1. 「[!UICONTROL **ボードに追加**]」をクリックして、「[!UICONTROL **既存のボード**]」を選択します。
1. [!UICONTROL 既存のボードに追加]ダイアログで、カードを移行するボードを検索して選択します。次に、「[!UICONTROL **追加**]」をクリックします。

   ![かんばんカードを既存のボードに追加](assets/add-kanban-cards-to-existing-board-dialog.png)

1. （オプション）表示される成功メッセージで、リンクをクリックしてボードを開きます。
