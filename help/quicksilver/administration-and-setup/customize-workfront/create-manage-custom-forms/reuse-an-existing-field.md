---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: 従来のフォームビルダーでカスタムフォーム内のカスタムフィールドまたはアセットウィジェットを再利用
description: カスタムフォームを作成または編集する際に、別のカスタムフォームに既に追加されているカスタムフィールドまたはウィジェットを追加できます。
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 2c617909-48cb-4ee1-b0e8-002f2e57b0f0
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: ht
source-wordcount: '436'
ht-degree: 100%

---

# 従来のフォームビルダーでカスタムフォーム内のカスタムフィールドまたはアセットウィジェットを再利用

カスタムフォームを作成または編集する際に、別のカスタムフォームに既に追加されているカスタムフィールドまたはアセットウィジェットを追加できます。

また、カスタムフォームで既存の計算済みカスタムフィールドを再利用することもできます。手順については、[カスタムフォームで既存の計算済みカスタムフィールドを再利用](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)を参照してください。

カスタムフォームのカスタムフィールドおよびアセットウィジェットについて詳しくは、[カスタムフォームにカスタムフィールドを追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)および[カスタムフォームでのアセットウィジェットの追加または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)を参照してください。

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
   <td> <p>カスタムフォームへの管理アクセス権</p> <p>Workfront 管理者がこのアクセス権を付与する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">ユーザーへの特定のエリアに対する管理アクセス権の付与</a>を参照してください。</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセスレベル設定を確認するには、Workfront 管理者にお問い合わせください。

## 別のカスタムフォームで既に使用されているカスタムフィールドまたはウィジェットを再利用

1. カスタムフォームの作成または編集を開始します（[従来のフォームビルダーを使用してカスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)で説明されています）。
1. 「**フィールドを追加**」を選択し、「**フィールドライブラリ**」をクリックします。

1. カスタムフォームで必要なフィールドまたはウィジェットをここにドラッグします。
1. （オプション）前述の 2 つの手順を繰り返して、他のフィールドやウィジェットを追加します。

   >[!NOTE]
   >
   >1 つのカスタムフォームに最大 500 個のフィールドやウィジェットを追加できます。ただし、フォームに 100 を超えるフィールドやウィジェットが存在する場合は、その複雑さに応じてパフォーマンスの低下が生じる可能性があります。
   >
   >
   >複雑なフォームの例としては、カスケードパラメーターを含むフォーム、計算済みカスタムデータフィールドを含むフォーム、単一のフィールドに複数の値オプションを含むフォームなどがあります。

1. 他の方法でカスタムフォームの作成を続ける場合は、以下の記事のいずれかに進みます。

   * [従来のフォームビルダーを使用してカスタムフォームへカスタムフィールドを追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md#add2)
   * [従来のフォームビルダーを使用してカスタムフォームにセクション区切りを追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [レガシーフォームビルダーを使用してカスタムフォームでアセットウィジェットを追加または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [レガシーフォームビルダーを使用して計算データをカスタムフォームに追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [従来のフォームビルダーを使用してカスタムフォーム内でカスタムフィールドおよびウィジェットを配置](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [レガシーフォームビルダーを使用してカスタムフォームに表示ロジックとスキップロジックを追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [レガシーフォームビルダーを使用してカスタムフォームをプレビューし、完成させる](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)
