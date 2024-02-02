---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: レガシーフォームビルダーを使用してカスタムフォームにカスタムフィールドおよびウィジェットを配置する
description: カスタムフォーム内のカスタムフィールドとウィジェットの位置を変更できます。
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: f96425e3-8e20-43ac-8340-915538ae5886
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: ht
source-wordcount: '449'
ht-degree: 100%

---

# レガシーフォームビルダーを使用してカスタムフォームにカスタムフィールドおよびウィジェットを配置する

カスタムフォーム内のカスタムフィールドとウィジェットの位置を変更できます。

カスタムフォームのカスタムフィールドとウィジェットについて詳しくは、[カスタムフォームにカスタムフィールドを追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)および[カスタムフォームでのアセットウィジェットの追加または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront プラン*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td>プラン</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>カスタムフォームへの管理アクセス権</p> <p>Workfront 管理者がこのアクセス権を付与する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定のエリアに対する管理者アクセス権をユーザーに付与</a>を参照してください。</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセスレベル設定を確認するには、Workfront 管理者にお問い合わせください。

## カスタムフォーム内にカスタムフィールドおよびウィジェットを配置する

1. [レガシーフォームビルダーを使用してカスタムフォームを作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)の説明に従って、カスタムフォームの作成または編集を開始します。
1. [レガシーフォームビルダーを使用してカスタムフィールドをカスタムフォームに追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)および[レガシーフォームビルダーを使用してカスタムフォームでアセットウィジェットを追加または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)の説明に従って、カスタムフィールドとウィジェットをフォームに追加します。

1. （オプション）カスタムフィールドとウィジェットを同じ行に配置するには、その間に行が表示されるまで、隣り合わせにドラッグします。

<!--
Courtney, this is a story that got postponed after I did the work. Slated for some time in 22.4 (https://hub.workfront.adobe.com/task/6220d425000140d7f7d3ea68cc9529c8/documents)
   You can drag multiple items. Press the following keys while you select the items, then drag the items together to the new row:
   * Mac: Command+Shift [Courtney, double-check these commands]
   * Windows: Ctrl+Shift

   When you drop the custom field or widget, a gray box displays around the two items to indicate that they share a row.
-->

>[!NOTE]
>
>* 右下隅の&#x200B;**プレビュー**&#x200B;ボタンを使用すると、カスタムフィールドとウィジェットがフォームにどのように表示されるかを確認できます。
>* 説明テキストフィールドで行を共有することはできません。
>* ユーザーが表示しているときに使用可能な画面スペースの量に応じて、カスタムフィールドとウィジェットがフォームで同じように表示されない場合があります。例えば、水平方向のスペースが限られている場合、フィールドの行の 3 番目のフィールドが次のフィールドの行に折り返されることがあります。

1. （オプション）カスタムフィールドまたはウィジェットを別のフィールドの上または下に配置するには、項目の間に青い水平線が表示されるまで、上または下にドラッグします。
1. 「**適用**」をクリックします。
1. 他の方法でカスタムフォームの作成を続ける場合は、以下の記事のいずれかに進みます。

   * [レガシーフォームビルダーを使用してカスタムフォームにカスタムフィールドを追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2)
   * [レガシーフォームビルダーを使用してカスタムフォームでアセットウィジェットを追加または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [レガシーフォームビルダーを使用して計算データをカスタムフォームに追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [レガシーフォームビルダーを使用してカスタムフォームにセクション区切りを追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [レガシーフォームビルダーを使用してカスタムフォームに表示ロジックとスキップロジックを追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [レガシーフォームビルダーを使用してカスタムフォームをプレビューし、完成させる](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
