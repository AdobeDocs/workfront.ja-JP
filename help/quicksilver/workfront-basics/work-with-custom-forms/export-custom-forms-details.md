---
title: カスタムフォームとオブジェクトの詳細のエクスポート
description: カスタムフォームとオブジェクトの詳細のエクスポート
author: Alina
draft: Probably
feature: Get Started with Workfront
exl-id: 4dc32da0-9680-4b7f-a959-d4a0652618c5
source-git-commit: 1670edf153e57152e51adcfbda052eb74541d931
workflow-type: tm+mt
source-wordcount: '597'
ht-degree: 1%

---

# カスタムフォームとオブジェクトの詳細のエクスポート

オブジェクトの「詳細」セクションから概要とカスタムフォーム情報を書き出し、PDFファイルに書き出すことができます。 その後、他のユーザーとPDFを印刷または共有できます。

この機能は、次のオブジェクトでサポートされています。

* プロジェクト
* タスク
* 問題
* ポートフォリオ
* プログラム

<!--
* Billing records</p> <p>After you open a billing record on a project, you can use the Details area to attach a custom form to the record and fill it out. You can also export billing record information from the Details area.</p> </li>
  -->

>[!NOTE]
>
>Workfrontまたはグループ管理者がレイアウトテンプレートを使用して削除した「詳細」セクションのフィールドは表示されません。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront license*</p> </td> 
   <td> <p>問題に対するリクエスト以上</p> <p>プロジェクトとタスクのレビュー以上</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong> </td> 
   <td> <p>プロジェクト、タスクおよびタスクの表示以上</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>オブジェクト権限</p> </td> 
   <td> <p>フォームを書き出すプロジェクト、タスク、または問題に対する権限を表示または上限に設定します</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

開始する前に、次のすべてが必要です。

1. 書き出し元の特定のオブジェクトに対してカスタムフォームを作成します。
1. カスタムフォームをオブジェクトに添付する

   または

   カスタムフォームを添付し、フォーム上の情報を編集するための適切なアクセス権を持っている。

カスタムフォームの作成について詳しくは、 [カスタムフォームの作成または編集](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

オブジェクトへのフォームの添付について詳しくは、 [オブジェクトへのカスタムフォームの追加](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## 「詳細」セクションでの情報のエクスポート

オブジェクトの「詳細」(Details) セクションからの情報のエクスポートは、サポートされるすべてのオブジェクトで同じです。

1. 少なくとも表示権限を持つプロジェクト、タスク、ポートフォリオ、プログラム、またはイシューに移動します。
1. 次をクリック： **「詳細」項目** 左側のパネル（例： ） **タスクの詳細**.
1. （オプション）オブジェクトにカスタムフォームが添付されていない場合は、 **カスタムフォームフィールドを追加**&#x200B;をクリックし、リストに表示されたらクリックします。

   最大 10 個のフォームを追加できます。

1. （オプション）「詳細」セクションの情報を更新し、 **変更を保存**.
1. 次をクリック： **書き出し** 右上隅のドロップダウンメニューで、「 **概要**&#x200B;または書き出すフォームを選択し、 **書き出し**.

   また、 **すべて選択** 「概要」領域とすべてのカスタムフォームをエクスポートする場合。

   ![](assets/export-custom-form-button-menu.png)

   >[!TIP]
   >
   >次のシナリオが存在する場合があります。
   >
   >   
   >   
   >   * グループまたはWorkfrontの管理者が概要領域のすべてのフィールドの選択を解除し、オブジェクトにカスタムフォームが添付されている場合、「概要」セクションは表示されません。
   >   * グループまたはWorkfrontの管理者が「概要」領域のすべてのフィールドの選択を解除し、オブジェクトにカスタムフォームが添付されていない場合、「エクスポート」ドロップダウンメニューは表示されません。
   >   * オブジェクトにカスタムフォームが添付されていない場合は、「概要」領域のみを書き出すことができます。
   >   * ロジックの背後にあり、フォームに表示されないカスタムフィールドは、書き出しできません。 カスタムフォームにロジックを追加する方法について詳しくは、 [表示ロジックの追加とカスタムフォームへのロジックのスキップ](../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md).


   PDFファイルが作成され、コンピューターにダウンロードされます。 PDFファイルには、次の情報が含まれます。

   * フォームを添付するオブジェクトの名前
   * PDFをエクスポートしたユーザーの名前
   * PDFが作成された日時
   * 書き出したフォームの名前
   * フォームに入力されたフィールドからの情報
