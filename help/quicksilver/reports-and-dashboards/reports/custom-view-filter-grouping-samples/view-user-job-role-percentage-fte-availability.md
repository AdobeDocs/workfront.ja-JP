---
content-type: reference
product-area: reporting;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 「ビュー：FTE 使用可能時間に対するユーザー担当業務の割合」
description: ユーザーリストのビューに列を追加して、ユーザーが関連付けられている担当業務のリストと、ユーザープロファイルで定義されている各担当業務の FTE 使用可能時間の割合を表示できます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: d479b0b1-8ad5-47d6-8ef8-80261b46ecea
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: ht
source-wordcount: '358'
ht-degree: 100%

---

# ビュー：FTE 使用可能時間のユーザー担当業務の割合

ユーザーリストのビューに列を追加して、ユーザーが関連付けられている担当業務のリストと、ユーザープロファイルで定義されている各担当業務の FTE 使用可能時間の割合を表示できます。

ユーザーの FTE 使用可能時間の割合に関して詳しくは、[ユーザーのプロファイルを編集する](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)を参照してください。

![user_with_percent_avialibility_per_role.png](assets/user-with-percent-avialbility-per-role-350x138.png)

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>表示の変更をリクエスト </p>
   <p>レポートを変更するためのプラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルター、表示、グループ化へのアクセス権を編集して、表示を変更できるようにします。</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr>   
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## FTE 使用可能時間のユーザー担当業務の割合を表示

1. ユーザーのリストに移動します。
1. **ビュー**&#x200B;ドロップダウンメニューから、「**新規ビュー**」を選択します。

1. **列プレビュー**&#x200B;エリアで、「**列を追加**」をクリックします。

1. 残りの列のヘッダーをクリックし、「**テキストモードに切り替え**」を選択します。
1. テキストモードエリアにポインタを合わせ、「**クリックしてテキストを編集**」をクリックします。
1. 「**テキストモード**」ボックスにあるテキストを削除し、次のコードに置き換えます。
   <pre>displayname=Roles Time Percentage<br>listdelimiter=<p><br>listmethod=nested(userRoles).lists<br>textmode=true<br>type=iterate<br>valueexpression=CONCAT({role},'-',{timePercentage},'%')<br>valueformat=HTML</pre>

1. 「**保存**」、「**ビューを保存**」の順にクリックします。

1. （オプション）ビューの名前を指定し、「**ビューを保存**」をクリックします。
