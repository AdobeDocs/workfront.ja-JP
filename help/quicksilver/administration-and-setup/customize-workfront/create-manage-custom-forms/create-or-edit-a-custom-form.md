---
title: 従来のフォームビルダーを使用したカスタムフォームの作成または編集
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: カスタムフォームを新規作成または編集できます。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 5712e82d-bd1d-4d8a-9a2a-1e19b562b9d1
source-git-commit: ccb2b6bb9fa63d29523ff396490f9580ad130bdd
workflow-type: tm+mt
source-wordcount: '956'
ht-degree: 74%

---

# 従来のフォームビルダーを使用したカスタムフォームの作成または編集

<!--Audited: 01/2024-->

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべての顧客に対してプレビュー環境でのみ使用できるか、または迅速リリースを有効にした顧客の実稼動環境でのみ使用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

<span class="preview">現在のリリースについて詳しくは、 [2024 年第 2 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

カスタムフォームを新規作成または編集できます。両方のタスクについては、この記事で説明します。

既存のフォームからカスタムフォームを新規作成する方法について詳しくは、[従来のフォームビルダーでカスタムフォームをコピーしてフォームを新規作成する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/copy-custom-form-to-create-a-new-one.md)を参照してください。

ここでは、レガシーフォームビルダーを使用してカスタムフォームを作成する方法について説明します。 フォームデザイナーを使用したカスタムフォームの作成について詳しくは、 [フォームデザイナーを使用したフォームのデザイン](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md).

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront プラン</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td><p>新規：標準</p>
   <p>または</p>
   <p>現在：プラン</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>カスタムフォームへの管理アクセス権</p> </td> 
  </tr>  
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## カスタムフォームの作成を開始

{{step-1-to-setup}}

1. 左側のパネルで「**カスタムフォーム**」をクリックします。

   カスタムフォームはリストに表示されます。 組織で作成されたすべてのカスタムフォームおよびカスタムフィールドを確認できます。 また、各フォームの作成者、フォームに関連付けられているオブジェクト、およびフォームがアクティブかどうかも確認できます。

1. 「**新規カスタムフォーム**」をクリックします。
1. カスタムフォームに関連付けるオブジェクトの種類を少なくとも 1 つ選択し、「**続行**」をクリックします。

   ![](assets/choose-object-type.jpg)

1. 次の日： **フォーム設定** 開いたタブに、 **フォームタイトル** およびオプション **説明** カスタムフォーム用。

1. （オプション）フォームにオブジェクトの種類を追加して、他のオブジェクトに添付できるようにする場合は、 **プラス** 次の後に署名 **オブジェクトタイプ**&#x200B;を選択し、表示されるメニューで目的のオブジェクトタイプを選択します。

   この操作を繰り返して、必要な数のオブジェクトタイプを追加できます。

1. （オプション） **X** をオンにすると、フォームから削除されます。

   保存済みのカスタムフォームからオブジェクトタイプを削除する方法について詳しくは、「[カスタムフォームのオブジェクトタイプの削除](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md)」を参照してください。

1. クリック **完了** をクリックします。

   >[!TIP]
   >
   >カスタムフォームの作成中に「**適用**」をクリックすると、変更内容を保存してフォームを開いたままにすることができます。

1. 新しいカスタムフィールドをフォームに追加する場合は、[カスタムフォームにカスタムフィールドを追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)または[カスタムフォームでカスタムフィールドまたはウィジェットを再利用する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)に進んでください。

   または

   他の方法でカスタムフォームの作成を続ける場合は、以下の記事のいずれかに進みます。

   * [カスタムフォームでのアセットウィジェットの追加または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [カスタムフォーム内にカスタムフィールドおよびウィジェットを配置](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [カスタムフォームにセクション区切りを追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [計算データをカスタムフォームに追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [カスタムフォームで既存の計算済みカスタムフィールドを再利用](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [カスタムフォームへの表示ロジックとスキップロジックを追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)

## カスタムフォームの編集を開始

カスタムフォームは、作成後いつでも編集できます。

>[!CAUTION]
>
>ユーザーがフィールドに入力したデータが失われることなく、カスタムフォームからフィールドを削除する方法について詳しくは、[システムからカスタムフィールドまたはウィジェットを削除する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md)の記事の[ユーザーが入力したデータが失われることなく、カスタムフィールドを削除する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-a-custom-field.md#remove)の節を参照してください。
>
>一般に、既に使用されているカスタムフォームを編集する回数は最小限に抑えることをお勧めします。カスタムフォームを使用するユーザーに変更に関して警告を出す通知システムはありません。

{{step-1-to-setup}}

1. 左側のパネルで「**カスタムフォーム**」をクリックします。

   カスタムフォームはリストに表示されます。 組織で作成されたすべてのカスタムフォームおよびカスタムフィールドを確認できます。 また、各フォームの作成者、フォームに関連付けられているオブジェクト、およびフォームがアクティブかどうかも確認できます。

1. 編集するカスタムフォームを選択し、 **編集** <span class="preview">または ![編集アイコン](assets/edit-icon.png).</span>
1. （オプション）カスタムフォームのタイトルと説明を変更するには「**フォーム設定**」タブをクリックして、**フォームタイトル**&#x200B;および&#x200B;**説明**&#x200B;を入力します。

1. （オプション）フォームに他のオブジェクトタイプを追加して、より多くのオブジェクトに添付できるようにする場合は、**オブジェクトタイプ**&#x200B;の後にあるプラス記号（+）をクリックし、表示されるメニューから必要なタイプを選択します。

   ![](assets/add-object-type-existing-form.png)

   この操作を繰り返して、必要な数のオブジェクトタイプを追加できます。

   また、オブジェクトタイプの X をクリックして、フォームから削除することもできます。この操作は、既に保存したカスタムフォームからオブジェクトタイプを削除する場合に注意が必要です。詳しくは、[カスタムフォームのオブジェクトタイプの削除](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/delete-object-type-on-a-custom-form.md)を参照してください。

1. 「**完了**」をクリックします。

   >[!TIP]
   >
   >カスタムフォームの作成中に「**適用**」をクリックすると、変更内容を保存してフォームを開いたままにすることができます。

1. 新しいカスタムフィールドをフォームに追加する場合は、[カスタムフォームにカスタムフィールドを追加する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)または[カスタムフォームでカスタムフィールドまたはウィジェットを再利用する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)に進んでください。

   または

   他の方法でカスタムフォームの作成を続ける場合は、以下の記事のいずれかに進みます。

   * [カスタムフォームでのアセットウィジェットの追加または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [カスタムフォーム内にカスタムフィールドおよびウィジェットを配置](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [カスタムフォームにセクション区切りを追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-section-break-to-a-custom-form.md)
   * [計算データをカスタムフォームに追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [カスタムフォームで既存の計算済みカスタムフィールドを再利用](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [カスタムフォームへの表示ロジックとスキップロジックを追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
