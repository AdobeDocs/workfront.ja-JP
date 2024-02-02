---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「ビュー：タスクまたはプロジェクトレポート内の解決可能オブジェクト」
description: すべての解決可能オブジェクトのリストを、プロジェクト、タスクビューまたはレポートに表示できます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2b0d8e7c-9211-44e5-9d92-c87a2fe4336d
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: ht
source-wordcount: '331'
ht-degree: 100%

---

# ビュー：タスクまたはプロジェクトレポート内の解決可能なオブジェクト

すべての解決可能オブジェクトのリストを、プロジェクト、タスクビューまたはレポートに表示できます。

解決可能オブジェクトについて詳しくは、[解決オブジェクトと解決可能オブジェクトの概要](../../../manage-work/issues/convert-issues/resolving-and-resolvable-objects.md)を参照してください。

![list_of_resolvables_in_report.png](assets/list-of-resolvables-in-report-350x54.png)

このビューの適用方法は、タスクとプロジェクトで同じです。

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

## タスクまたはプロジェクトレポートでの解決可能オブジェクトの表示

1. イシューから変換されたタスクのリストに移動します。
1. **ビュー**&#x200B;ドロップダウンメニューから、「**新規ビュー**」を選択します。

1. **列プレビュー**&#x200B;エリアで、「**列を追加**」をクリックします。

1. 残りの列のヘッダーをクリックし、「**テキストモードに切り替え**」を選択します。
1. テキストモードエリアにポインタを合わせ、「**クリックしてテキストを編集**」をクリックします。
1. 「**テキストモード**」ボックスにあるテキストを削除し、次のコードに置き換えます。
   <pre>displayname=Resolvables<br>listdelimiter=<br><br>listmethod=nested(resolvables).lists<br>textmode=true<br>type=iterate<br>valuefield=name<br>valueformat=HTML<br></pre>

1. 「**ビューを保存**」をクリックします。\
   新しい列に、すべての解決可能オブジェクトのリストが表示されます。リスト内のオブジェクトの名前は、オブジェクトに直接リンクできません。
