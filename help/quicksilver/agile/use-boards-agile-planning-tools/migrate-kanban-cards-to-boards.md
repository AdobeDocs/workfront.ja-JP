---
content-type: reference
navigation-topic: boards
title: アジャイルチームのカンバンカードをWorkfront ボードに移行する
description: 作業項目をアジャイルチームのカンバンボードから新規または既存のWorkfront ボードに移行できます。
author: Courtney
feature: Agile
exl-id: 72e3902b-af9a-497c-817f-63630c4fb73b
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/RXk7PYF6JsdF71pRVwEA-Wk23h-UqbgLPXSyNR7VX5Y'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
    internal-label: Work management
subfeature_v2:
  - id: be65ef36-43e4-48e1-a062-caa3778e15be
    internal-label: Agile
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '360'
ht-degree: 72%
---
# アジャイルチームのかんばんカードの Workfront ボードへの移行

作業項目をアジャイルチームのカンバンボードから新規または既存のWorkfront ボードに移行できます。 移行を実行すると、かんばんボード上のすべてのカードが Workfront ボードにコピーされます。 特定のカードを選択することはできません。

Workfront ボードでのカードの配置は、列ポリシーに基づいています。 （例えば、ポリシーを使用すると、ステータスが「処理中」のすべてのカードを特定の列に移動できます。 列ポリシーについて詳しくは、[&#x200B; ボード列の管理](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)を参照してください。） ポリシーがない場合、またはカードがポリシーと一致しない場合、カードはボードの一番左の列に配置されます。 現時点では、レガシーボードのバックログ列のカードは Workfront ボードに追加されません。

カードはアジャイルチームのカンバンボードから削除されないため、カードのステータスの変更は両方のボードに同期されます。 Workfront ボードに切り替える準備が整うまで、両方のボードをアクティブにしておくことができます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>コントリビューター以上</p> 
   <p>リクエスト以上</p>
   </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

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
1. [!UICONTROL 既存のボードに追加]ダイアログで、カードを移行するボードを検索して選択します。 次に、「[!UICONTROL **追加**]」をクリックします。

   ![かんばんカードを既存のボードに追加](assets/add-kanban-cards-to-existing-board-dialog.png)

1. （オプション）表示される成功メッセージで、リンクをクリックしてボードを開きます。
