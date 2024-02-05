---
title: フォームデザイナーを使用したコピーからのフォームのデザイン
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: フォームデザイナーを使用して、コピーからカスタムフォームをデザインできます。
author: Courtney
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 578a8bd5-d93f-4327-bb4f-2c17b91b170a
source-git-commit: 7467e75cf468fa6a1dd14dbc0f4fdcda87de1b1e
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 98%

---

# フォームデザイナーを使用したコピーからのフォームのデザイン

既存のフォームに基づく新しいカスタムフォームをデザインできます。カスタムフォームを様々な Workfront オブジェクトに添付して、これらのオブジェクトに関するデータを取り込むことができます。

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
   <td>
   <p>新規プラン：標準</p>
   <p>または</p>
   <p>現在のプラン：プラン</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>カスタムフォームへの管理アクセス権</p> <p>Workfront 管理者がこのアクセス権を付与する方法について詳しくは、<a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定のエリアに対する管理者アクセス権をユーザーに付与</a>を参照してください。</p> </td> 
  </tr>  
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセスレベル設定を確認するには、Workfront 管理者にお問い合わせください。

## カスタムフォームのコピーによる新規フォームの作成

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、**設定** ![](assets/gear-icon-settings.png) の順にクリックします。

1. 「**カスタムフォーム**」をクリックします。
1. 新しいカスタムフォームのベースとして使用するカスタムフォームを選択し、「**コピー**」をクリックします。
1. 表示される&#x200B;**カスタム フォーム コピー**&#x200B;ダイアログボックスで、次の情報を入力します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">フォーム名</td> 
      <td>コピー元のフォームの名前を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">フォームタイプ </p> </td> 
      <td> <p>「<b>フォームタイプ</b>」フィールドで、カスタムフォームで扱うオブジェクトタイプを選択し、削除するタイプの横にある「X」アイコンをクリックします。既にフォームに関連付けられているタイプは、リストで無効になっています。</p> 
      <p><img src="assets/copy-form-obj-types.png"></p> 
      <p>フォームは、少なくとも 1 つのオブジェクトタイプに関連付ける必要があります。</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**フォームをコピー**」をクリックします。

   元のフォームで、新しいフォームに追加するオブジェクトタイプと互換性のないフィールドを計算フィールドで参照している場合は、それらのフィールドの計算を変更するように求めるメッセージが表示されます。

   同様に、元のフォームのセクション区切りのアクセスオプションが、新しいフォームに追加するオブジェクトタイプと互換性がない場合は、オプションを調整するように求めるメッセージが表示されます。

1. 先ほどコピーしたフォームを選択し、「**編集**」をクリックします。
1. [フォームのデザイン](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)の記事の以下の節における説明に従って、フォームに変更を加えます。

* [別のカスタムフォームで既に使用されている既存のフィールドまたはウィジェットの再利用](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [テキストフィールドの追加](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-text-fields)
   * [計算フィールドの追加](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-calculated-fields)
   * [ラジオボタン、チェックボックスグループ、ドロップダウンの追加](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-radio-buttons-checkboxes-and-dropdowns)
   * [先行入力フィールドと日付フィールドの追加](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-typeahead-and-date-fields)
   * [画像、PDF、ビデオの追加](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-images-pdfs-and-videos)
   * [Adobe XD ファイルの追加](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-adobe-xd-files)

1. （オプション）「**保存して閉じる**」をクリックした後に、使用先のオブジェクトにフォームを添付します。詳しくは、[オブジェクトへのカスタムフォームの追加](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)を参照してください。
