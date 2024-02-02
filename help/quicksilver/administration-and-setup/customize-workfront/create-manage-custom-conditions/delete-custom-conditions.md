---
title: カスタム条件の削除
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: カスタム条件を削除することができます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5fbd4989-460b-4380-a136-8a9f6b79787d
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: ht
source-wordcount: '267'
ht-degree: 100%

---

# カスタム条件の削除

## アクセス要件

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
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## カスタム条件の削除

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、**設定** ![](assets/gear-icon-settings.png) の順にクリックします。

1. **プロジェクト環境設定**／**条件**&#x200B;をクリックします。

   <!--
   <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Make sure it's this way also in QS</span>
   -->

1. オブジェクトタイプのタブ（「**プロジェクト**」タブ、「**タスク**」タブ、または「**イシュー**」タブ）を選択します。ここで、削除する条件を見つけることができます。

1. 削除する条件の上にポインタを合わせて、右端に表示される「**削除**」アイコン ![](assets/delete.png) をクリックします。
1. 表示される確認メッセージで、「**条件を削除**」をクリックします。

1. 表示される「**条件を削除**」ボックスで、削除しようとしている条件を使用しているすべてのプロジェクトのドロップダウンリストから、新しい条件を選択します。

   カスタム条件は、削除しようとしている条件と同じ組み込み条件に等しい場合にのみ、ドロップダウンリストで使用できます。例えば、「危険あり」に等しい条件を削除する場合、「危険あり」に等しいカスタム条件のみを選択できます。

1. 「**条件を削除**」をクリックします。

>[!NOTE]
>
>「目標どおり」、「危険あり」、「トラブル発生中」の組み込み条件は削除できません。ただし、名前と色は変更できます。

カスタム条件について詳しくは、[カスタム条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md)を参照してください。
