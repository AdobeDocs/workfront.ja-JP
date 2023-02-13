---
title: カスタム条件の削除
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-conditions
description: カスタム条件は削除できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 5fbd4989-460b-4380-a136-8a9f6b79787d
source-git-commit: 02191d80ea58f80de2e7be2ff55f43663e415e31
workflow-type: tm+mt
source-wordcount: '267'
ht-degree: 0%

---

# カスタム条件の削除

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront管理者である。</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## カスタム条件の削除

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **プロジェクト環境設定** > **条件**.

   <!--
   <span data-mc-conditions="QuicksilverOrClassic.Draft mode">Make sure it's this way also in QS</span>
   -->

1. オブジェクトタイプのタブを選択します (**プロジェクト**, **タスク**&#x200B;または **問題**) をクリックします。

1. 削除する条件の上にマウスポインターを置いて、 **削除** アイコン ![](assets/delete.png) それは右端に現れる
1. 表示される確認メッセージで、 **条件を削除**.

1. 内 **条件を削除** 表示されるボックスで、削除する条件を使用しているすべてのプロジェクトのドロップダウンリストから新しい条件を選択します。

   カスタム条件は、削除する条件と同じ組み込み条件を持つ場合にのみ、ドロップダウンリストで使用できます。 例えば、「リスクあり」に等しい条件を削除する場合、「リスクあり」に等しいカスタム条件のみを選択できます。

1. クリック **条件を削除**.

>[!NOTE]
>
>「ターゲット上」、「危険な状態」、「問題が発生中」の組み込み条件は削除できません。 ただし、名前と色は変更できます。

カスタム条件について詳しくは、 [カスタム条件](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/custom-conditions.md).
