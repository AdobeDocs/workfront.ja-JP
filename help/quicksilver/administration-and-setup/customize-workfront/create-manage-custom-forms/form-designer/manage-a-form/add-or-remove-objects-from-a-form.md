---
title: フォームデザイナーを使用して既存のカスタムフォームに対してオブジェクトタイプの追加または削除を行う
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: フォームデザイナーを使用して、カスタムフォームに対してオブジェクトタイプを追加または削除できます。
author: Courtney
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c43ea6b2-7d5b-46f0-a092-f57128de60f0
source-git-commit: 7467e75cf468fa6a1dd14dbc0f4fdcda87de1b1e
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 98%

---

# フォームデザイナーを使用して既存のカスタムフォームに対してオブジェクトタイプの追加または削除を行う

フォームデザイナーを使用して、既存のカスタムフォームに対してオブジェクトタイプを追加または削除できます。

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
   <td><p>カスタムフォームへの管理アクセス権</p> <p>Workfront 管理者がこのアクセス権を付与する方法について詳しくは、<a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定のエリアに対する管理者アクセス権をユーザーに付与</a>を参照してください。</p></td> 
  </tr>  
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセスレベル設定を確認するには、Workfront 管理者にお問い合わせください。

## 既存のカスタムフォームにオブジェクトタイプを追加する

フォームにオブジェクトタイプを追加して、複数のオブジェクトに添付できるようにすることができます。

>[!NOTE]
>
>セクション区切りの権限は、オブジェクトタイプの影響を受ける場合があります。カスタムフォームセクションセクション区切りの制限付き編集権限は、プロジェクト、タスク、イシューおよびユーザーのオブジェクトタイプに対してのみ使用できます。
>
>詳しくは、[複数のオブジェクトタイプがセクション区切り権限に与える影響](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/organize-a-form.md#how-multiple-object-types-can-affect-section-break-permissions)を参照してください。


1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックして、**設定** ![](assets/gear-icon-settings.png) をクリックします。

1. 左側のパネルで「**カスタムフォーム**」をクリックします。

   表示されるビューで、組織用に作成されたすべてのカスタムフォームを確認できます。また、各フォームの作成者、対象となるオブジェクトタイプ、アクティブかどうかも確認できます。

1. オブジェクトタイプを追加するカスタムフォームを選択し、「**編集**」をクリックします。

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

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、「**設定**」![](assets/gear-icon-settings.png) をクリックします。

1. 左側のパネルで「**カスタムフォーム**」をクリックします。
1. 編集するカスタムフォームを選択し、「**編集**」をクリックします。
1. フォームから削除する&#x200B;**オブジェクトタイプ**&#x200B;の X をクリックし、表示される警告メッセージで「**削除**」をクリックします。

   ![](assets/delete-object-types.png)

1. （オプション）フォームから削除する他のオブジェクトタイプについて、前の手順を繰り返します。
1. 「**完了**」をクリックして、「**保存して閉じる**」をクリックします。
