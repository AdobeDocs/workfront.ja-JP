---
title: レガシーフォームビルダーを使用したカスタムフォームの作成または編集
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: 新しいカスタムフォームを作成または編集できます。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5712e82d-bd1d-4d8a-9a2a-1e19b562b9d1
source-git-commit: 8af1890b2e2ae613279b5191cf8f2190364fb524
workflow-type: tm+mt
source-wordcount: '922'
ht-degree: 0%

---

# レガシーフォームビルダーを使用したカスタムフォームの作成または編集

<!--Audited: 01/2024-->

新しいカスタムフォームを作成または編集できます。 両方のタスクについては、この記事で説明します。

既存のフォームから新しいカスタムフォームを作成する方法について詳しくは、 [カスタムフォームをコピーして、レガシーフォームビルダーを使用して新しいフォームを作成する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md).

ここでは、レガシーフォームビルダーを使用してカスタムフォームを作成する方法について説明します。 フォームデザイナーを使用したカスタムフォームの作成について詳しくは、 [フォームデザイナーを使用したフォームのデザイン](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

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
   <td><p>新規：標準</p>
   <p>現在：プラン</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>カスタムフォームへの管理アクセス</p> <p>Workfront管理者がこのアクセス権を付与する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定の領域に対する管理者アクセス権をユーザーに付与する</a>.</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスタイプ、アクセスレベル設定を確認するには、Workfront管理者に問い合わせてください。 アクセス要件について詳しくは、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


## カスタムフォームの作成を開始する

{{step-1-to-setup}}

1. クリック **カスタムForms** をクリックします。

   カスタムフォームはリストに表示されます。 組織で作成されたすべてのカスタムフォームおよびカスタムフィールドを確認できます。 また、各フォームの作成者、フォームに関連付けられているオブジェクト、およびフォームがアクティブかどうかも確認できます。

1. クリック **新規カスタムフォーム。**
1. カスタムフォームに関連付けるオブジェクトの種類を少なくとも 1 つ選択し、 **続行**.

   ![](assets/choose-object-type.jpg)

1. 次の日： **フォーム設定** 開いたタブに、 **フォームタイトル** およびオプション **説明** カスタムフォーム用。

1. （オプション）フォームにオブジェクトの種類を追加して、他のオブジェクトに添付できるようにする場合は、 **プラス** 次の後に署名 **オブジェクトタイプ**&#x200B;を選択し、表示されるメニューで目的のオブジェクトタイプを選択します。

   この操作を繰り返して、必要な数のオブジェクトタイプを追加できます。

1. （オプション） **X** をオンにすると、フォームから削除されます。

   保存済みのカスタムフォームからオブジェクトタイプを削除する方法については、「 [カスタムフォームのオブジェクトタイプの削除](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. クリック **完了** をクリックします。

   >[!TIP]
   >
   >次をクリックできます。 **適用** カスタムフォームの作成中はいつでも、変更内容を保存し、フォームを開いたままにすることができます。

1. 新しいカスタムフィールドをフォームに追加する場合は、次に進みます。 [カスタムフォームにカスタムフィールドを追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) または [カスタムフォームでカスタムフィールドまたはウィジェットを再利用する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   または

   他の方法でカスタムフォームの作成を続ける場合は、次の記事のいずれかに進みます。

   * [カスタムフォームでのアセットウィジェットの追加または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [カスタムフォーム内でのカスタムフィールドおよびウィジェットの配置](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [カスタムフォームにセクション区切りを追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [計算データをカスタムフォームに追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [カスタムフォームで既存の計算済みカスタムフィールドを再利用する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [表示ロジックの追加とカスタムフォームへのロジックのスキップ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)

## カスタムフォームの編集を開始

カスタムフォームは、作成後いつでも編集できます。

>[!CAUTION]
>
>ユーザーがフィールドに入力したデータが失われることなく、カスタムフォームからフィールドを削除する方法については、「 [ユーザーが入力したデータが失われることなく、カスタムフィールドを削除します](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md#remove) 記事内 [システムからカスタムフィールドまたはウィジェットを削除する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md).
>
>一般に、既に使用されているカスタムフォームを編集する回数は最小限に抑えることをお勧めします。 カスタムフォームを使用するユーザーに変更に関して警告を出す通知システムはありません。

{{step-1-to-setup}}

1. クリック **カスタムForms** をクリックします。

   カスタムフォームはリストに表示されます。 組織で作成されたすべてのカスタムフォームおよびカスタムフィールドを確認できます。 また、各フォームの作成者、フォームに関連付けられているオブジェクト、およびフォームがアクティブかどうかも確認できます。

1. 編集するカスタムフォームを選択し、 **編集**.
1. （オプション）カスタムフォームのタイトルと説明を変更するには、 **フォーム設定** 「 」タブに **フォームタイトル** および **説明**.

1. （オプション）フォームに他の種類のオブジェクトを追加して、他のオブジェクトに添付できるようにする場合は、プラス記号+ () **オブジェクトタイプ**&#x200B;を選択し、表示されるメニューで目的のタイプを選択します。

   ![](assets/add-object-type-existing-form.png)

   この操作を繰り返して、必要な数のオブジェクトタイプを追加できます。

   また、オブジェクトタイプの X をクリックして、フォームから削除することもできます。 この操作は、既に保存したカスタムフォームからオブジェクトタイプを削除する場合には、注意して行う必要があります。 詳しくは、 [カスタムフォームのオブジェクトタイプの削除](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md).

1. クリック **完了**.

   >[!TIP]
   >
   >次をクリックできます。 **適用** カスタムフォームの作成中はいつでも、変更内容を保存し、フォームを開いたままにすることができます。

1. 新しいカスタムフィールドをフォームに追加する場合は、次に進みます。 [カスタムフォームにカスタムフィールドを追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md) または [カスタムフォームでカスタムフィールドまたはウィジェットを再利用する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).

   または

   他の方法でカスタムフォームの作成を続ける場合は、次の記事のいずれかに進みます。

   * [カスタムフォームでのアセットウィジェットの追加または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [カスタムフォーム内でのカスタムフィールドおよびウィジェットの配置](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [カスタムフォームにセクション区切りを追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [計算データをカスタムフォームに追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [カスタムフォームで既存の計算済みカスタムフィールドを再利用する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [表示ロジックの追加とカスタムフォームへのロジックのスキップ](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
