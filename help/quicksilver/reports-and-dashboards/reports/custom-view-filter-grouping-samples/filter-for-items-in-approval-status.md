---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'フィルター：承認ステータスの項目のみを表示'
description: 特定のステータスの項目（現在「承認待ち」にある項目）のみを表示できます。 これは、承認ステータスを持つ他のオブジェクトに対しても同じように機能します。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 1%

---

# フィルター：承認ステータスの項目のみを表示

特定のステータスの項目（現在「承認待ち」にある項目）のみを表示できます。 これは、承認ステータスを持つ他のオブジェクトに対しても同じように機能します。

次のオブジェクトを承認ステータスに配置できます。

* タスク
* 問題
* プロジェクト

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
   <td> <p>フィルターの変更リクエスト </p>
   <p>レポートの変更計画</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集して、レポートを変更します</p> <p>フィルター、ビュー、グループへのアクセスを編集してフィルターを変更します</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr>
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 承認ステータスの項目のみを表示

1. 例えば、プロジェクトのリスト用にカスタマイズするフィルターに移動します。
1. クリック **フィルタールールを追加** の **ステータス** リストのオブジェクトのフィールド。\
   例えば、プロジェクトレポートで、 **ステータス等しい計画**&#x200B;ステータスが「 」のプロジェクトのみを表示する場合は、 **計画 — 承認待ち**.

1. クリック **テキストモードに切り替え**.
1. を変更します。

   ```
   status
   ```

   行を追加して **:A** をステータスの 3 文字のキーに設定します。
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. クリック **完了**&#x200B;を、 **フィルターを保存**.

   このリストには、「計画 — 承認待ち」ステータスのプロジェクトのみが表示されます。
