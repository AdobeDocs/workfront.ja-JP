---
user-type: administrator
product-area: system-administration
keywords: 作成、カスタム、フォーム、コピー、ベース、別の
navigation-topic: create-and-manage-custom-forms
title: カスタムフォームをコピーして、従来のビルダーで新しく作成
description: 既存のフォームに基づく新しいカスタムフォームを作成できます。
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 946a726e-af88-413c-abe3-55fbc7486380
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: ht
source-wordcount: '464'
ht-degree: 100%

---

# カスタムフォームをコピーして、従来のビルダーで新しく作成

既存のフォームに基づく新しいカスタムフォームを作成できます。

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
1. 次の記事で説明するように、フォームに変更を加えます。

   * [レガシーフォームビルダーを使用してカスタムフォームをコピーして新しいフォームを作成](#Add2)
   * [レガシーフォームビルダーを使用して計算データをカスタムフォームに追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md)
   * [レガシーフォームビルダーを使用してカスタムフォームにカスタムフィールドおよびウィジェットを配置](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/position-fields-in-a-custom-form.md)
   * [レガシーフォームビルダーを使用してカスタムフォームでアセットウィジェットを追加または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)
   * [レガシーフォームビルダーを使用してカスタムフォームで既存の計算済みカスタムフィールドを再利用](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/use-existing-calc-field-new-custom-form.md)
   * [レガシーフォームビルダーを使用してカスタムフォームに表示ロジックとスキップロジックを追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/display-or-skip-logic-custom-form.md)
   * [レガシーフォームビルダーを使用してカスタムフォームをプレビューし、完成させる](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/preview-and-complete-a-custom-form.md)

1. （オプション）「**保存して閉じる**」をクリックした後に、使用先のオブジェクトにフォームを添付します。詳しくは、[カスタムフォームをオブジェクトに追加](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)を参照してください。
