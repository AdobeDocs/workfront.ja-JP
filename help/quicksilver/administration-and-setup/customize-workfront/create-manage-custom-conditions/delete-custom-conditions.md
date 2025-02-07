---
title: カスタム条件の削除
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: カスタム条件を削除することができます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 5fbd4989-460b-4380-a136-8a9f6b79787d
source-git-commit: d2ca099e78d5adb707a0a5a53ccb2e6dd06698f8
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 81%

---

# カスタム条件の削除

不要になったカスタム条件は削除できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：プラン</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## カスタム条件の削除

{{step-1-to-setup}}

1. **プロジェクト環境設定**／**条件**&#x200B;をクリックします。

   <!--
   <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Make sure it's this way also in QS</span>
   -->

1. オブジェクトタイプのタブ（「**プロジェクト**」タブ、「**タスク**」タブ、または「**イシュー**」タブ）を選択します。ここで、削除する条件を見つけることができます。

1. 削除したい条件にカーソルを合わせ、右端に表示される **削除** アイコン ![ 削除 ](assets/delete.png) をクリックします。
1. 表示される確認メッセージで、「**条件を削除**」をクリックします。

1. 表示される「**条件を削除**」ボックスで、削除しようとしている条件を使用しているすべてのプロジェクトのドロップダウンリストから、新しい条件を選択します。

   カスタム条件は、削除しようとしている条件と同じ組み込み条件に等しい場合にのみ、ドロップダウンリストで使用できます。例えば、「危険あり」に等しい条件を削除する場合、「危険あり」に等しいカスタム条件のみを選択できます。

1. 「**条件を削除**」をクリックします。

>[!NOTE]
>
>「目標どおり」、「危険あり」、「トラブル発生中」の組み込み条件は削除できません。ただし、名前と色は変更できます。

カスタム条件について詳しくは、[カスタム条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md)を参照してください。
