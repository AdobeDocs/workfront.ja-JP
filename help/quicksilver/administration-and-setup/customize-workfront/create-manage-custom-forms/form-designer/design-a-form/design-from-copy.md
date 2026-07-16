---
title: コピーからのフォームの作成
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: フォームデザイナーを使用して、コピーからカスタムフォームを作成できます。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 578a8bd5-d93f-4327-bb4f-2c17b91b170a
TQID: https://experienceleague.adobe.com/WaLGsLpGDMXGvNd7W-8JzmgJYiCaxSd-gaMoGy6j-Zc
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 3e77f50ee2297a9c552e27bfcdf7f08a6a4c89b5
workflow-type: tm+mt
source-wordcount: 371
ht-degree: 79%

---

# コピーからのフォームの作成

既存のフォームに基づく新しいカスタムフォームをデザインできます。 カスタムフォームを様々な Workfront オブジェクトに添付して、これらのオブジェクトに関するデータを取り込むことができます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td><p>標準</p>
       <p>プラン</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>カスタムフォームへの管理アクセス権</p> </td> 
  </tr>  
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## カスタムフォームのコピーによる新規フォームの作成

{{step-1-to-setup}}

1. 「**カスタムフォーム**」をクリックします。
1. 新しいカスタムフォームのベースとして使用するカスタムフォームを選択し、![コピーアイコン](assets/copy-icon.png) をクリックします。
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
      <td> <p>「<b>フォームタイプ</b>」フィールドで、カスタムフォームで扱うオブジェクトタイプを選択し、削除するタイプの横にある「X」アイコンをクリックします。 既にフォームに関連付けられているタイプは、リストで無効になっています。</p> 
      <p><img src="assets/copy-form-obj-types-040524.png"></p> 
      <p>フォームは、少なくとも 1 つのオブジェクトタイプに関連付ける必要があります。</p> 
      </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**コピー**」をクリックします。

   元のフォームで、新しいフォームに追加するオブジェクトタイプと互換性のないフィールドを計算フィールドで参照している場合は、それらのフィールドの計算を変更するように求めるメッセージが表示されます。

   同様に、元のフォームのセクション区切りのアクセスオプションが、新しいフォームに追加するオブジェクトタイプと互換性がない場合は、オプションを調整するように求めるメッセージが表示されます。

1. 先ほどコピーしたフォームを選択し、![編集アイコン](assets/edit-icon.png) をクリックします。
1. [ カスタムフォームの作成](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)記事の次の節で説明しているように、フォームに変更を加えます。

   * [別のカスタムフォームで既に使用されている既存のフィールドまたはウィジェットの再利用](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#reuse-an-existing-field-or-widget-already-used-in-another-custom-form)
   * [テキストフィールドの追加](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-text-fields)
   * [計算フィールドの追加](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-calculated-fields)
   * [ラジオボタン、チェックボックスグループ、ドロップダウンの追加](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-radio-buttons-checkboxes-and-dropdowns)
   * [日付フィールドを追加](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-date-fields)
   * [画像、PDF、ビデオの追加](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-images-pdfs-and-videos)
   * [Adobe XD ファイルの追加](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-adobe-xd-files)
   * [Planning 接続フィールドの追加](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-planning-connection-fields)

1. （オプション）「**保存して閉じる**」をクリックした後、「[ カスタムフォームをオブジェクトに追加](/help/quicksilver/workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)」の説明に従って、フォームを使用するオブジェクトに添付します。
