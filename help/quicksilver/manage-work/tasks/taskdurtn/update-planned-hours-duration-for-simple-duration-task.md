---
product-area: projects
navigation-topic: task-duration
title: タスクの予定時間と期間をシンプルな期間タイプで更新する
description: デフォルトでは、Adobe Workfrontは、予定時間数に基づいて、「シンプルな期間」タイプのタスクの期間を計算します。 ただし、Workfrontの特定の領域で、計画時間数タスクとシンプルな期間タスクの期間を手動で編集することもできます。
author: Alina
feature: Work Management
exl-id: 47a9b095-2b7d-4ed0-8cb6-e6bd5e37ce9c
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '486'
ht-degree: 1%

---

# タスクの予定時間と期間をシンプルな期間タイプで更新する

デフォルトでは、Adobe Workfrontは、予定時間数に基づいて、「シンプルな期間」タイプのタスクの期間を計算します。 ただし、Workfrontの特定の領域で、計画時間数タスクとシンプルな期間タスクの期間を手動で編集することもできます。

タスクの予定時間と期間は、[ 簡易期間の種類 ] をインラインに設定して編集するか、[ 割り当て ] 領域のタスクレベルで編集することができます。

情報をインラインで編集する方法について詳しくは、 [Adobe Workfrontのリスト内の項目をインライン編集する](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md).

この記事では、[ 割り当て ] 領域で、タスクレベルの [ 簡易期間の種類 ] でタスクの [ 予定時間 ] と [ 期間 ] を更新する方法について説明します。

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
   <td> <p>仕事以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>タスクへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## タスクの予定時間と期間をシンプルな期間タイプで更新する

>[!IMPORTANT]
>
>シンプルな期間タスクで期間を手動で更新すると、Workfrontは、計画時間に基づいて期間の計算を停止します。

[ 詳細な割り当て ] ボックスの [ 標準期間の種類 ] でタスクの予定時間と期間を編集するには、次の手順に従います。

1. タスクの一覧で、期間の種類を変更するタスクの名前をクリックします。
1. 次のいずれかの操作を行います。

   * 次をクリック： **詳細** アイコン ![](assets/qs-more-icon-on-an-object.png) タスク名の横にある **編集**&#x200B;を、 **割り当て**.
   * 次をクリック： **割り当て先** タスクヘッダーの「割り当て」領域で割り当ての名前を選択し、 **詳細**.

1. の合計値を入力 **予定時間** すべての割り当て（例： 10 時間）に対して。 計画時間の合計数は、タスクに割り当てられたすべてのリソース間で均等に配分されます。
1. （オプション）タスクに割り当てられた各リソースの予定時間を手動で調整します。 リソースに個別に割り当てられた新しい時間を反映するタスクの更新予定時間の合計数です。
1. タスクの値を入力 **期間**（例：2 日）

   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. 「**保存**」をクリックします。
