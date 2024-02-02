---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 「フィルター：承認ステータスの項目のみを表示」
description: 特定のステータスの項目（現在「承認待ち」にある項目）のみを表示できます。これは、承認ステータスを持つ他のオブジェクトに対しても同じように機能します。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: c1de5193-d3d5-406c-aa68-e6ba6d6751ae
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: ht
source-wordcount: '315'
ht-degree: 100%

---

# フィルター：承認ステータスの項目のみを表示

特定のステータスの項目（現在「承認待ち」にある項目）のみを表示できます。これは、承認ステータスを持つ他のオブジェクトに対しても同じように機能します。

次のオブジェクトを承認ステータスに配置できます。

* タスク
* イシュー
* プロジェクト

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

## 承認ステータスの項目のみを表示

1. 例えば、プロジェクトのリスト用にカスタマイズするフィルターに移動します。
1. リストのオブジェクトの「**ステータス**」フィールドに「**フィルター規則の追加**」をクリックします。\
   例えば、プロジェクトレポートで、ステータスが&#x200B;**計画 - 承認待ち**&#x200B;のプロジェクトのみを表示する場合は、**ステータスと計画が等しい**&#x200B;を追加します。

1. 「**テキストモードに切り替える**」をクリックします。
1. 行を変更するには、

   ```
   status
   ```

   ステータスの 3 文字のキーに「**:A**」を追加します。
   <pre>status=PLN:A<br>status_Mod=in</pre>

1. 「**完了**」をクリックして、「**フィルターを保存**」をクリックします。

   このリストには、計画 - 承認待ちのステータスのプロジェクトのみが表示されます。
