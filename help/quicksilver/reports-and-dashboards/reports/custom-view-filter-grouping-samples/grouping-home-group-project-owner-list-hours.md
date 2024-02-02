---
content-type: reference
product-area: reporting;projects;user-management
navigation-topic: custom-view-filter-and-grouping-samples
title: 「グループ化：時間数のリスト内のプロジェクト所有者のホームグループ」
description: プロジェクト所有者のホームグループの名前を時間リストまたはレポートに表示できます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6491ab9b-c09e-4bdb-99c2-56bb44f66947
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: ht
source-wordcount: '264'
ht-degree: 100%

---

# グループ化：時間数のリスト内のプロジェクト所有者のホームグループ

プロジェクト所有者のホームグループの名前を時間リストまたはレポートに表示できます。

グループ化は、プロジェクト所有者の名前やプロジェクト名でも結果をグループ化します。

![grouping_for_project_owner_home_group.png](assets/grouping-for-project-owner-home-group-350x51.png)

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
   <td> <p>グループ化を変更するためのリクエスト </p>
   <p>レポートを変更するためのプラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルター、ビュー、グループ化へのアクセス権を編集して、グループ化を変更できるようにします。</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 時間数のリスト内のプロジェクト所有者のホームグループによるグループ化

このグループ化を適用するには、次の操作を行います。

1. 時間のリストに移動します。
1. **グループ化**&#x200B;ドロップダウンメニューで「**新規グループ化**」を選択します。

1. 「**テキスト モードに切り替える**」をクリックします。
1. **レポートをグループ化**&#x200B;エリア内のテキストを削除します。
1. 次のコードでテキストを置き換えます。

   ```
   group.0.displayname=Home Group of Project Owner<br>group.0.valuefield=project:owner:homeGroup:name<br>group.0.valueformat=HTML<br>group.1.displayname=Project Owner<br>group.1.linkedname=projectOwnerMM<br>group.1.namekey=view.relatedcolumn<br>group.1.namekeyargkey.0=projectOwnerMM<br>group.1.namekeyargkey.1=name<br>group.1.valuefield=projectOwnerMM:name<br>group.1.valueformat=string<br>group.2.displayname=Project Name<br>group.2.linkedname=project<br>group.2.namekey=view.relatedcolumn<br>group.2.namekeyargkey.0=project<br>group.2.namekeyargkey.1=name<br>group.2.valuefield=project:name<br>group.2.valueformat=string<br>textmode=true
   ```

1. 「**グループ化を保存**」をクリックします。
