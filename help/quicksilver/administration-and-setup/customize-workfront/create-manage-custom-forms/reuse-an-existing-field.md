---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 従来のフォームビルダーでカスタムフォーム内のカスタムフィールドまたはアセットウィジェットを再利用する
description: カスタムフォームを作成または編集する際に、別のカスタムフォームに既に追加されているカスタムフィールドまたはウィジェットを追加できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 2c617909-48cb-4ee1-b0e8-002f2e57b0f0
source-git-commit: ac5b7e0237dbcaea14010eda658f7d5a6be089cc
workflow-type: tm+mt
source-wordcount: '436'
ht-degree: 0%

---

# 従来のフォームビルダーでカスタムフォーム内のカスタムフィールドまたはアセットウィジェットを再利用する

カスタムフォームを作成または編集する際に、別のカスタムフォームに既に追加されているカスタムフィールドまたはアセットウィジェットを追加できます。

また、カスタムフォームで既存の計算済みカスタムフィールドを再利用することもできます。 手順については、 [カスタムフォームで既存の計算済みカスタムフィールドを再利用する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md).

カスタムフォームのカスタムフィールドおよびアセットウィジェットについて詳しくは、 [カスタムフォームにカスタムフィールドを追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) および [カスタムフォームでのアセットウィジェットの追加または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>計画</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>カスタムフォームへの管理アクセス</p> <p>Workfront管理者がこのアクセス権を付与する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定の領域に対する管理者アクセス権をユーザーに付与する</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスタイプ、アクセスレベル設定を確認するには、Workfront管理者に問い合わせてください。

## 別のカスタムフォームで既に使用されているカスタムフィールドまたはウィジェットを再利用する

1. カスタムフォームの作成または編集を開始します ( [レガシーフォームビルダーを使用したカスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
1. を使用 **フィールドを追加** 選択済み、クリック **フィールドライブラリ**.

1. カスタムフォームで必要なフィールドまたはウィジェットをここにドラッグします。
1. （オプション）前の 2 つの手順を繰り返して、他のフィールドやウィジェットを追加します。

   >[!NOTE]
   >
   >1 つのカスタムフォームに最大 500 個のフィールドとウィジェットを追加できます。 ただし、フォームの複雑さに応じて 100 を超える場合は、パフォーマンスの低下が生じる可能性があります。
   >
   >
   >複雑なフォームの例としては、カスケードパラメーターを持つフォーム、計算済みカスタムデータフィールド、単一のフィールドに複数の値を入力するオプションなどがあります。

1. 他の方法でカスタムフォームの作成を続ける場合は、次の記事のいずれかに進みます。

   * [レガシーフォームビルダーを使用したカスタムフォームへのカスタムフィールドの追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2)
   * [レガシーフォームビルダーを使用したカスタムフォームへのセクション区切りの追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [レガシーフォームビルダーを使用したカスタムフォームでのアセットウィジェットの追加または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [レガシーフォームビルダーを使用して計算データをカスタムフォームに追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [従来のフォームビルダーを使用したカスタムフォーム内でのカスタムフィールドおよびウィジェットの配置](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [従来のフォームビルダーを使用して、表示ロジックを追加し、ロジックをカスタムフォームにスキップします](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [レガシーフォームビルダーを使用してカスタムフォームをプレビューし、完成させます](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
