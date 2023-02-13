---
title: カスタムフォームに追加されたカスタムフォームとウィジェットのリストと編集
description: 組織のカスタムフォームと、それらに追加されたカスタムフィールドおよびウィジェットのリストを表示する場合、ツールバーのオプションを使用して、プロパティの編集、プロパティの共有者の制限、コピー、削除をおこなうことができます。 また、各カスタムフォームに関連付けられているオブジェクトタイプなど、表示される列のその他の情報を表示することもできます。
author: Caroline
source-git-commit: 49d4de3455fc1156efc8a88e8d2bee329c375279
workflow-type: tm+mt
source-wordcount: '560'
ht-degree: 0%

---

# カスタムフォームに追加されたカスタムフォームとウィジェットのリストと編集

組織のカスタムフォームと、それらに追加されたカスタムフィールドおよびウィジェットのリストを表示する場合、ツールバーのオプションを使用して、プロパティの編集、プロパティの共有者の制限、コピー、削除をおこなうことができます。 また、各カスタムフォームに関連付けられているオブジェクトタイプなど、表示される列のその他の情報を表示することもできます。

カスタムフォームのカスタムフィールドとウィジェットについて詳しくは、 [カスタムフォームにカスタムフィールドを追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) および [カスタムフォームでのアセットウィジェットの追加または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md).

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

## カスタムフォームに追加されたカスタムフォームおよび項目の一覧と編集

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **カスタムForms**.

   を使用 **Forms** 「 」タブが選択されると、組織のすべてのカスタムフォームがその説明と共に表示され、関連付けられたオブジェクトタイプ、作成したユーザーの名前、システム内でアクティブかどうかが表示されます。

   リストでカスタムフォームを選択する際に実行できる操作について詳しくは、次の記事を参照してください。

   * [カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)
   * [カスタムフォームの共有](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)
   * [カスタムフォームをコピーして新しいフォームを作成する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md)
   * [カスタムフォームの削除または非アクティブ化](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-or-deactivate-a-custom-form.md)

1. 次をクリック： **フィールド** タブをクリックします。

   このタブには、システム内のユーザーがカスタムフォームに追加したカスタムフィールドとウィジェット、および各アイテムの種類に関する情報、手順と詳細、およびそれを含むカスタムフォームのリストが表示されます。

   このリストには、次の条件の 1 つ以上を満たすカスタムフォーム項目のみが含まれます。

   * システム全体で編集可能
   * システム全体で表示可能
   * 作成者
   * 表示または管理アクセス権を持つ共有済み

   >[!NOTE]
   >
   >セクション区切りは、「フィールド」タブには表示されません。

   リスト内の項目を選択した場合に実行できる操作について詳しくは、次の記事を参照してください。

   * [カスタムフォーム内のカスタムフィールド、セクション区切り、またはウィジェットのプロパティを編集する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/edit-a-custom-field.md)
   * [カスタムフィールドとウィジェットの共有を設定する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md)
   * [システムからカスタムフィールドまたはウィジェットを削除する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md)


1. を選択します。 **セクション** 」タブに移動して、 **パラメータグループ** が **表示** リストの

   このビューには、すべての断面の破断が表示され、各断面の破断を含むカスタムフォームのリストも表示されます。

   リストで選択したカスタムセクションの編集について詳しくは、 [カスタムフォームにセクション区切りを追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md).

