---
product-area: projects
navigation-topic: task-duration
title: シンプル期間タイプでタスクの予定時間数と期間を更新します
description: デフォルトでは、予定時間数に基づいてシンプル期間タイプでタスクの期間が計算されます。ただし、Workfront の特定のエリアでは、予定時間数タスクとシンプル期間のタスクの期間を手動で編集することもできます。
author: Alina
feature: Work Management
exl-id: 47a9b095-2b7d-4ed0-8cb6-e6bd5e37ce9c
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '439'
ht-degree: 80%

---

# タスクの予定時間数と期間のシンプルな期間タイプでの更新

デフォルトでは、予定時間数に基づいてシンプル期間タイプでタスクの期間が計算されます。ただし、Workfront の特定のエリアでは、予定時間数タスクとシンプル期間のタスクの期間を手動で編集することもできます。

タスクの予定時間数と期間は、「割り当て」のシンプル期間タイプのインラインまたはタスクレベルで編集できます。

情報をインラインで編集する方法について詳しくは、[Adobe Workfront のリスト内の項目のインライン編集](../../../workfront-basics/navigate-workfront/use-lists/inline-edit-objects.md)を参照してください。

この記事では、「割り当て」のタスクレベルでシンプル期間タイプを使って、タスクの予定時間数と期間を更新する方法について説明します。

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
   <td><p>Standard 以上</p> 
   <p>ワークまたはそれ以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトに対する表示以上のアクセス権</p> <p>タスクへのアクセスを編集</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>タスクへのアクセスを管理 </p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Work or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Tasks</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the task</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## タスクの予定時間数と期間のシンプルな期間タイプでの更新

>[!IMPORTANT]
>
>シンプルな期間タスクで期間を手動で更新すると、予定時間数に基づく期間の計算が停止します。

「高度な割り当て」ボックスでシンプル期間タイプを使って、タスクの予定時間数と期間を編集するには：

1. タスクのリストで、期間タイプを変更するタスクの名前をクリックします。
1. 次のいずれかの操作を行います。

   * タスクの名前の横にある&#x200B;**その他**&#x200B;アイコン ![](assets/qs-more-icon-on-an-object.png) をクリックし、「**編集**」、「**割り当て**」の順にクリックします。
   * タスクヘッダーの「割り当て先」領域で **割り当て先** または割り当ての名前をクリックし、**詳細** をクリックします。

1. すべての割り当ての **予定時間数**&#x200B;の合計値を入力します（例：10 時間）。予定時間数の合計は、タスクに割り当てられたすべてのリソースに均等に配分されます。
1. （オプション）タスクに割り当てられた各リソースの予定時間数を手動で調整します。 リソースに個別に割り当てられた新しい時間を反映するためにタスクの更新を行う予定時間の合計数です。
1. タスクの&#x200B;**期間**&#x200B;の値を入力します（例：2 日）。

   ![](assets/advanced-assignments-simple-duration-multiple-resources-nwe-350x198.png)

1. 「**保存**」をクリックします。
