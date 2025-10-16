---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 表示：FTE の空き時間に対するユーザーの担当業務の割合
description: ユーザーリストのビューに列を追加して、ユーザーが関連付けられている担当業務のリストと、ユーザープロファイルで定義されている各担当業務の FTE 使用可能時間の割合を表示できます。
author: Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '276'
ht-degree: 63%

---

# ビュー：FTE 使用可能時間のユーザー担当業務の割合

<!--Audited: 11/2024-->

ユーザーリストのビューに列を追加して、ユーザーが関連付けられている担当業務のリストと、ユーザープロファイルで定義されている各担当業務の FTE 使用可能時間の割合を表示できます。

ユーザーの FTE 使用可能時間の割合に関して詳しくは、[ユーザーのプロファイルを編集する](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

![user_with_percent_avialibility_per_role.png](assets/user-with-percent-avialbility-per-role-350x138.png)

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>ビューの投稿者または変更依頼 </p>
   <p>レポートを変更するための標準またはプラン</p>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルター、表示、グループ化へのアクセス権を編集して、表示を変更できるようにします。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。


+++

## FTE 使用可能時間のユーザー担当業務の割合を表示

1. ユーザーのリストに移動します。
1. **ビュー** ドロップダウンメニューから「**新規ビュー**」を選択します。

1. **列のプレビュー** 領域で、「**列を追加**」をクリックします。

1. 新しい列のヘッダーをクリックし、**テキストモードに切り替え**/**テキストモードを編集** をクリックします。
1. 「**テキストモードを編集**」ボックスで検索したテキストを削除し、次のコードに置き換えます。

   ```
   displayname=Roles Time Percentage
   listdelimiter=
   listmethod=nested(userRoles).lists
   textmode=true
   type=iterate
   valueexpression=CONCAT({role},'-',{timePercentage},'%')
   valueformat=HTML
   ```

1. 「**完了**」をクリックし、「**ビューを保存** をクリックします。

1. （オプション）ビュー名を更新し、「**ビューを保存**」をクリックします。
