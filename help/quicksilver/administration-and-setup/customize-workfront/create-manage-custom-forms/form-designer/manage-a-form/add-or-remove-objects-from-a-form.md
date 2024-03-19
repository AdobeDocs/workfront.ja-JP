---
title: フォームデザイナーを使用して既存のカスタムフォームに対してオブジェクトタイプの追加または削除を行う
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: フォームデザイナーを使用して、カスタムフォームに対してオブジェクトタイプを追加または削除できます。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c43ea6b2-7d5b-46f0-a092-f57128de60f0
source-git-commit: ccb2b6bb9fa63d29523ff396490f9580ad130bdd
workflow-type: tm+mt
source-wordcount: '539'
ht-degree: 83%

---

# フォームデザイナーを使用して既存のカスタムフォームに対してオブジェクトタイプの追加または削除を行う

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべての顧客に対してプレビュー環境でのみ使用できるか、または迅速リリースを有効にした顧客の実稼動環境でのみ使用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

<span class="preview">現在のリリースについて詳しくは、 [2024 年第 2 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

フォームデザイナーを使用して、既存のカスタムフォームに対してオブジェクトタイプを追加または削除できます。

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
   <td role="rowheader">アクセスレベル設定*</td> 
   <td><p>カスタムフォームへの管理アクセス権</p></td> 
  </tr>  
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 既存のカスタムフォームにオブジェクトタイプを追加する

フォームにオブジェクトタイプを追加して、複数のオブジェクトに添付できるようにすることができます。

>[!NOTE]
>
>セクション区切りの権限は、オブジェクトタイプの影響を受ける場合があります。カスタムフォームセクションセクション区切りの制限付き編集権限は、プロジェクト、タスク、イシューおよびユーザーのオブジェクトタイプに対してのみ使用できます。
>
>詳しくは、[複数のオブジェクトタイプがセクション区切り権限に与える影響](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md#how-multiple-object-types-can-affect-section-break-permissions)を参照してください。


{{step-1-to-setup}}

1. 左側のパネルで「**カスタムフォーム**」をクリックします。

   表示されるビューで、組織用に作成されたすべてのカスタムフォームを確認できます。また、各フォームの作成者、対象となるオブジェクトタイプ、アクティブかどうかも確認できます。

1. オブジェクトタイプを追加するカスタムフォームを選択し、「 **編集** <span class="preview">または ![編集アイコン](assets/edit-icon.png).</span>

1. フォームの上部で、**オブジェクトタイプ**&#x200B;の後にあるプラス記号（+）をクリックし、表示されるメニューから必要なタイプを選択します。この操作を繰り返して、必要な数のオブジェクトタイプを追加できます。

   ![](assets/add-new-object.png)

1. 「**保存して閉じる**」をクリックします。

   >[!TIP]
   >
   >カスタムフォームの作成中はいつでも「**適用**」をクリックして、変更内容を保存し、フォームを開いたままにすることができます。

## カスタムフォームのオブジェクトタイプの削除

既存のカスタムフォームからオブジェクトタイプを削除できます。カスタムフォームには、少なくとも 1 つのオブジェクトタイプが必要です。

>[!CAUTION]
>
>削除するタイプのオブジェクトにユーザーが既にカスタムフォームを添付しており、データを追加している場合、フォーム上でそのオブジェクトタイプを削除すると、そのデータは完全に削除されます。ユーザーが後で必要とする履歴情報が含まれている場合があります。
>
>一般に、既に使用されているカスタムフォームを編集する回数は最小限に抑えることをお勧めします。カスタムフォームを使用するユーザーに変更に関して警告を出す通知システムはありません。

オブジェクトタイプを削除するには、以下の手順を実行します。

{{step-1-to-setup}}

1. 左側のパネルで「**カスタムフォーム**」をクリックします。
1. 編集するカスタムフォームを選択し、 **編集** <span class="preview">または ![編集アイコン](assets/edit-icon.png).</span>
1. 任意の **オブジェクトタイプ** をフォームから削除します。

   ![](assets/delete-object-types.png)

1. （オプション）フォームから削除する他のオブジェクトタイプについて、前の手順を繰り返します。
1. クリック **完了**&#x200B;を選択し、次に **保存して閉じる**.
