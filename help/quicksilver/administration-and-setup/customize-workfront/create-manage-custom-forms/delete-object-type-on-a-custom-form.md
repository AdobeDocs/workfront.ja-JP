---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: カスタムフォームのオブジェクトタイプの削除
description: 既存のカスタムフォームで、フォームに関連付けられているオブジェクトタイプを削除できます。この操作を行うと、ユーザーはそのタイプのオブジェクトにフォームを添付できなくなります。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ca6565c4-3d9e-4a11-a7b6-fce701923bf2
source-git-commit: d32f274390f6ffc5fdd01c2c9b4b2abd99d7cb10
workflow-type: tm+mt
source-wordcount: '304'
ht-degree: 100%

---

# カスタムフォームのオブジェクトタイプの削除

{{form-designer-default}}

既存のカスタムフォームで、フォームに関連付けられているオブジェクトタイプを削除できます。この操作を行うと、ユーザーはそのタイプのオブジェクトにフォームを添付できなくなります。

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
   <td role="rowheader">Adobe Workfront プラン</td> 
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

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## カスタムフォームのオブジェクトタイプの削除

既存のカスタムフォームからオブジェクトタイプを削除できます。

カスタムフォームには、少なくとも 1 つのオブジェクトタイプが必要です。

>[!CAUTION]
>
>削除するタイプのオブジェクトにユーザーが既にカスタムフォームを添付しており、データを追加している場合、フォーム上でそのオブジェクトタイプを削除すると、そのデータは完全に削除されます。ユーザーが後で必要とする履歴情報が含まれている場合があります。
>
>一般に、既に使用されているカスタムフォームを編集する回数は最小限に抑えることをお勧めします。カスタムフォームを使用するユーザーに変更に関して警告を出す通知システムはありません。

{{step-1-to-setup}}

1. 左側のパネルで「**カスタムフォーム**」をクリックします。
1. 編集するカスタムフォームを選択し、![編集アイコン](assets/edit-icon.png) をクリックします。
1. フォームから削除する&#x200B;**オブジェクトタイプ**&#x200B;の X をクリックし、表示される警告メッセージで「**削除**」をクリックします。

   ![](assets/click-x-object-types.jpg)

1. （オプション）フォームから削除する他のオブジェクトタイプについて、前の手順を繰り返します。
1. 「**完了**」をクリックし、「**保存して閉じる**」をクリックします。
