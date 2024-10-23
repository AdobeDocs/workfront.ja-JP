---
title: カスタムフォームとオブジェクトの詳細の書き出し
description: カスタムフォームとオブジェクトの詳細の書き出し
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: 7697327455a7ffdc1a15bfa1676c3a0b091abd04
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 94%

---

# カスタムフォームとオブジェクトの詳細の書き出し

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

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront プラン*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront ライセンス*</p> </td> 
   <td> <p>イシューの場合はリクエスト以上</p> <p>プロジェクトとタスクのレビューまたはそれ以上の権限</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong> </td> 
   <td> <p>プロジェクト、タスクおよびイシューの表示またはそれ以上の権限</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>オブジェクト権限</p> </td> 
   <td> <p>フォームを書き出すプロジェクト、タスクまたはイシューの表示またはそれ以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

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

   ![](assets/export-custom-form-button-menu.png)

   >[!TIP]
   >
   >次のシナリオが存在する可能性があります。
   >
   >   
   >   
   >   * グループ管理者または Workfront 管理者が概要エリアのすべてのフィールドを選択解除し、オブジェクトにカスタムフォームが添付されている場合は、「概要」セクションが表示されません。
   >   * グループ管理者または Workfront 管理者が概要エリアのすべてのフィールドを選択解除し、オブジェクトにカスタムフォームが添付されていない場合は、「書き出し」ドロップダウンメニューが表示されません。
   >   * オブジェクトにカスタムフォームが添付されていない場合は、概要エリアのみを書き出すことができます。
   >   * ロジックの裏で動作しフォームに表示されないカスタムフィールドは、書き出されません。カスタムフォームにロジックを追加する方法について詳しくは、「[ フォームに表示ロジックを追加し、スキップロジックを追加する ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/display-skip-logic-form-designer.md)」を参照してください。
   >   
   >

   PDF ファイルが生成され、お使いのコンピューターにダウンロードされます。この PDF ファイルには、次の情報が含まれています。

   * フォームが添付されているオブジェクトの名前
   * PDF を書き出したユーザーの名前
   * PDF が生成された日時
   * 書き出されたフォームの名前
   * フォームに入力されたフィールドの情報
