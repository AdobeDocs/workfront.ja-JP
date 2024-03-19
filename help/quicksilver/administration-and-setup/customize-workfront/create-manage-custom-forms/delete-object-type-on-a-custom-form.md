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
source-git-commit: ccb2b6bb9fa63d29523ff396490f9580ad130bdd
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 85%

---

# カスタムフォームのオブジェクトタイプの削除

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべての顧客に対してプレビュー環境でのみ使用できるか、または迅速リリースを有効にした顧客の実稼動環境でのみ使用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

<span class="preview">現在のリリースについて詳しくは、 [2024 年第 2 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

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
1. 編集するカスタムフォームを選択し、 **編集** <span class="preview">または ![編集アイコン](assets/edit-icon.png).</span>
1. フォームから削除する&#x200B;**オブジェクトタイプ**&#x200B;の X をクリックし、表示される警告メッセージで「**削除**」をクリックします。

   ![](assets/click-x-object-types.jpg)

1. （オプション）フォームから削除する他のオブジェクトタイプについて、前の手順を繰り返します。
1. クリック **完了**&#x200B;を選択し、次に **保存して閉じる**.
