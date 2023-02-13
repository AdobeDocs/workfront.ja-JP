---
content-type: reference
product-area: reporting;projects
navigation-topic: custom-view-filter-and-grouping-samples
title: 'グループ化：タスクの割合の内訳 2'
description: '''このカスタムタスクグループでは、完了率の値の範囲でグループ化されたタスクを表示できます。 分類には、完了率の値が 10%ポイントの増分で表示されます。「1-10%、11-20%等」'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 7d5a40dd-d451-48c7-9323-af52aa387709
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '289'
ht-degree: 4%

---

# グループ化：タスクの割合の分類 2

このカスタムタスクグループでは、完了率の値の範囲でグループ化されたタスクを表示できます。 分類には、完了率の値が 10%ポイント増分されて表示されます。1～10%、11～20%など

次のグループでは、プロジェクトを完了率の値でグループ化し、いずれかのグループに分けています。

* 0%
* 1 - 10%
* 11-20%
* 21-30%
* 31-40%
* 41-50%
* 51-60%
* 61-70%
* 71-80%
* 81-90%
* 91-99%
* 100%

![task_10__breakdown_grouping.png](assets/task-10--breakdown-grouping-350x547.png)

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
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集</p> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## タスクの割合の分類別にグループ化

このグループ化を適用するには：

1. タスクのリストに移動します。
1. 次の **グループ化** ドロップダウンメニューで、「 **新しいグループ化**.

1. クリック **テキストモードに切り替え**.
1. 内のテキストを削除します。 **レポートをグループ化** 領域
1. 次のコードに置き換えます。

   <pre>group.0.linkedname=direct<br>group.0.name=Percent Breakdown<br>group.0.notime=false<br>group.0.valueexpression=IF({percentComplete}=0,"0 %",IF({percentComplete}&lt;=11,"1-10 %",IF({percentComplete}&lt;=21,"11-20 %",IF({percentComplete}&lt;=31,"21-30 %",IF({percentComplete}&lt;41,"31-40 %",IF({percentComplete}&lt;51,"41-50 %",IF({percentComplete}&lt;61,"51-60 %",IF({percentComplete}&lt;71"61,1-70 %",IF({percentComplete}&lt;81,"71-80 %",IF({percentComplete}&lt;91,"81-90 %",IF({percentComplete}&lt;100,"91-99 %","100 %")))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))())))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))()))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))))<br>textmode=true</pre>

1. クリック **グループ化を保存**.
