---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「フィルター：2 つのフィールドを比較して、リスト内の項目を除外する」
description: 2 つのフィールドを比較することで、リストから項目をフィルタリングできます。例えば、タスクの実際の完了日が予定完了日よりも後のタスクのみを表示できます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 6a41db8e-1456-4031-bf2a-ca6d4111ad44
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: ht
source-wordcount: '290'
ht-degree: 100%

---

# フィルター：2 つのフィールドを比較して、リスト内の項目を除外する

2 つのフィールドを比較することで、リストから項目をフィルタリングできます。例えば、タスクの実際の完了日が予定完了日よりも後のタスクのみを表示できます。

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
   <td> <p>フィルターを変更する場合は「要求」 </p>
   <p>レポートを変更するためのプラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルターを変更する場合は、フィルター、ビュー、グループ化への編集アクセス権</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr>
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 2 つのフィールドの比較による項目のフィルタリング

1. タスクのリストに移動します。
1. **フィルター**&#x200B;ドロップダウンメニューから、「**新規フィルター**」を選択します。

1. 「**フィルタールールを追加**」をクリックし、**実際の完了日**／**より大きい**／**日付を選択**&#x200B;を追加します。

   >[!TIP]
   >
   >選択したフィールドに使用するフィルター修飾子を選択します（使用可能な場合）。

1. 「**テキストモードに切り替え**」をクリックします。
1. **レポートのフィルタールールを設定**&#x200B;領域に次のコードをペーストします。

   ```
   actualCompletionDate=FIELD:plannedCompletionDate<br>actualCompletionDate_Mod=gt
   ```

1. 「**完了**」をクリックして、「**フィルターを保存**」をクリックします。
