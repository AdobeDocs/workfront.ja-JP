---
title: カスタムのFormsとオブジェクトの詳細の書き出し
description: オブジェクトの「詳細」セクションから概要とカスタムフォーム情報を PDF ファイルに書き出すことができます。その後、PDF を印刷または他のユーザーと共有できます。
author: Alina
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: 187505de92f9a912547018865f2742bfecec77ad
workflow-type: tm+mt
source-wordcount: '579'
ht-degree: 90%

---

# カスタムフォームとオブジェクトの詳細の書き出し

<!--Audited: 10/2025-->

オブジェクトの「詳細」セクションから概要とカスタムフォーム情報を PDF ファイルに書き出すことができます。その後、PDF を印刷または他のユーザーと共有できます。

この機能は、次のオブジェクトでサポートされています。

* プロジェクト
* タスク
* イシュー
* ポートフォリオ
* プログラム

<!--
* Billing records</p> <p>After you open a billing record on a project, you can use the Details area to attach a custom form to the record and fill it out. You can also export billing record information from the Details area.</p> </li>
  -->

>[!NOTE]
>
>Workfront 管理者またはグループ管理者がレイアウトテンプレートを使用して削除した「詳細」セクションのフィールドは表示されません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront パッケージ</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront プラン</p> </td> 
   <td><p>問題の場合：</p>
   <ul><li><p>投稿者以上</p></li>
   <li><p>要求者以上</p> </li></ul>
   <p>プロジェクトおよびタスクの場合：</p>
   <ul><li><p>ライト以上</p></li>
   <li><p>Reviewer 以上</p></li></ul>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクト、タスクおよびイシューの表示またはそれ以上の権限</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>オブジェクト権限</p> </td> 
   <td> <p>フォームを書き出すプロジェクト、タスクまたはイシューの表示またはそれ以上の権限</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront license*</p> </td> 
   <td> <p>Request or higher for issues</p> <p>Review or higher for projects and tasks</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>Access level configurations*</strong> </td> 
   <td> <p>View or higher for Projects, Tasks, and Issues</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Object permissions</p> </td> 
   <td> <p>View or higher permissions to the project, task, or issue whose form you want to export</p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 前提条件

開始する前に、以下のものがすべて必要です。

1. 書き出し元の特定のオブジェクト用に作成されたカスタムフォーム
1. オブジェクトに添付されたカスタムフォーム

   または

   カスタムフォームを添付しフォーム上の情報を編集するための適切なアクセス権

カスタムフォームの作成について詳しくは、「[ カスタムフォームの作成 ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)」を参照してください。

オブジェクトへのフォームの添付については、[オブジェクトへのカスタムフォームの追加](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)を参照してください。

## 「詳細」セクションの情報を書き出し

オブジェクトの「詳細」セクションからの情報の書き出しは、サポートされているどのオブジェクトでも同じです。

1. 少なくとも表示権限のあるプロジェクト、タスク、ポートフォリオ、プログラムまたはイシューに移動します。
1. 左パネルで&#x200B;**「詳細」項目**（「**タスクの詳細**」など）をクリックします。
1. （オプション）オブジェクトにカスタムフォームが添付されていない場合は、「**カスタムフォームを追加**」フィールドにカスタムフォームの名前を入力していき、目的の名前がリストに表示されたらクリックします。

   最大 10 個のフォームを追加できます。

1. （オプション）「詳細」セクションの情報を更新したあと、「**変更を保存**」をクリックします。
1. 右上隅の&#x200B;**書き出し**&#x200B;ドロップダウンメニューをクリックし、「**概要**」または書き出すフォームを選択して、「**書き出し**」をクリックします。

   概要エリアとすべてのカスタムフォームを書き出す場合は、「**すべて選択**」を選択することもできます。

   ![ 「カスタムフォームを書き出し」ボタン ](assets/export-custom-form-button-menu.png)

   >[!TIP]
   >
   >次のシナリオが存在する可能性があります。
   >
   >   * グループ管理者または Workfront 管理者が概要エリアのすべてのフィールドを選択解除し、オブジェクトにカスタムフォームが添付されている場合は、「概要」セクションが表示されません。
   >   * グループ管理者または Workfront 管理者が概要エリアのすべてのフィールドを選択解除し、オブジェクトにカスタムフォームが添付されていない場合は、「書き出し」ドロップダウンメニューが表示されません。
   >   * オブジェクトにカスタムフォームが添付されていない場合は、概要エリアのみを書き出すことができます。
   >   * ロジックの裏で動作しフォームに表示されないカスタムフィールドは、書き出されません。カスタムフォームへのロジックの追加について詳しくは、[ カスタムフォームとフィールドへのロジックルールの追加 ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md) を参照してください。

   PDF ファイルが生成され、お使いのコンピューターにダウンロードされます。この PDF ファイルには、次の情報が含まれています。

   * フォームが添付されているオブジェクトの名前
   * PDF を書き出したユーザーの名前
   * PDF が生成された日時
   * 書き出されたフォームの名前
   * フォームに入力されたフィールドの情報
