---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'グループ化：プロジェクト — 入力日別'
description: このカスタムプロジェクトグループでは、入口日の値でグループ化されたプロジェクトを表示できます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 511faad5-b5bd-4e2d-8daa-3fcde49a502c
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '249'
ht-degree: 2%

---

# グループ化：プロジェクト — 入力日別

このカスタムプロジェクトグループでは、入口日の値でグループ化されたプロジェクトを表示できます。

各グループは、次の範囲の入力日を持つプロジェクトを表示します。

* 過去 30 日間
* 30 ～ 60 日
* 60 日以上前

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>グループ化を変更するリクエスト </p>
   <p>レポートの変更計画</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートを変更します</p> <p>フィルター、ビュー、グループへのアクセスを編集してグループ化を変更します</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr>  
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## プロジェクトを入力日別にグループ化

このグループ化を適用するには：

1. 既存のプロジェクトレポートに移動するか、新しいプロジェクトレポートを作成します。\
   レポートの作成について詳しくは、 [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. 次の **グループ化** タブ、クリック **グループを追加**.

1. クリック **テキストモードに切り替え**.
1. 内のテキストを削除します。 **レポートをグループ化** 領域
1. 次のコードに置き換えます。

   ```
   group.0.linkedname=direct<br>
   ```

   ```
   group.0.name=Project Entry<br>
   ```

   ```
   group.0.valueexpression=IF(ABS(DATEDIFF({entryDate},$$TODAY))<=30,"Last 30 Days",IF(ABS(DATEDIFF({entryDate},$$TODAY))>30&&ABS(DATEDIFF({entryDate},$$TODAY))<=60,"30-60 Days","Older than 60 days"))<br>
   ```

   ```
   group.0.valueformat=atDateAsMonthString<br>
   ```

   ```
   textmode=true
   ```

1. 「**保存して閉じる**」をクリックします。
