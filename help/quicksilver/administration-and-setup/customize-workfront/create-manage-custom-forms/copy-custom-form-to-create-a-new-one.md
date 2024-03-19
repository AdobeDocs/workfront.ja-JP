---
user-type: administrator
product-area: system-administration
keywords: 作成、カスタム、フォーム、コピー、ベース、別の
navigation-topic: create-and-manage-custom-forms
title: カスタムフォームをコピーして、従来のビルダーで新しく作成
description: 既存のフォームに基づく新しいカスタムフォームを作成できます。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 946a726e-af88-413c-abe3-55fbc7486380
source-git-commit: ccb2b6bb9fa63d29523ff396490f9580ad130bdd
workflow-type: tm+mt
source-wordcount: '493'
ht-degree: 89%

---

# カスタムフォームをコピーして、従来のビルダーで新しく作成

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべての顧客に対してプレビュー環境でのみ使用できるか、または迅速リリースを有効にした顧客の実稼動環境でのみ使用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

<span class="preview">現在のリリースについて詳しくは、 [2024 年第 2 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

既存のフォームに基づく新しいカスタムフォームを作成できます。

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
   <td>
   <p>新規：標準</p>
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

## カスタムフォームのコピーによる新規フォームの作成

{{step-1-to-setup}}

1. 「**カスタムフォーム**」をクリックします。
1. 新しいカスタムフォームの基礎として使用するカスタムフォームを選択し、 **コピー** <span class="preview">または ![コピーアイコン](assets/copy-icon.png).</span>
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
