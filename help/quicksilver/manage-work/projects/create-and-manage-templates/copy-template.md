---
product-area: templates
navigation-topic: templates-navigation-topic
title: プロジェクトテンプレートのコピー
description: プロジェクトテンプレートをゼロから作成するだけでなく、既存のテンプレートをコピーして修正することもできます。
author: Alina
feature: Work Management
exl-id: b2e0878b-8245-4e01-819d-c3746f553d95
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 44%

---

# プロジェクトテンプレートのコピー

<!--Audited: 5/2025-->

プロジェクトテンプレートをゼロから作成するだけでなく、既存のテンプレートをコピーしてAdobe Workfrontで変更することもできます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>標準</p> 
   <p>プラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>テンプレートへの編集アクセス</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>テンプレートに対する表示権限またはそれ以上の権限</p>  </td> 
  </tr> 
 </tbody> 
</table>

* 詳しくは、[Workfront ドキュメント &#x200B;](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)のアクセス要件を参照してください。

+++

<!--
Old:

 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td><p>New: Standard</p> 
   <p>Current: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>Edit access to Templates</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions to a template</p>  </td> 
  </tr> 
 </tbody> 
</table>
-->

## テンプレートのコピーに関する考慮事項

次の項目は、常に既存のテンプレートから新しいテンプレートにコピーされます。

* テンプレートタスク
* テンプレートタスクのデフォルト情報（タスクのデフォルトの承認プロセス、タスクのデフォルトのカスタムフォーム）
* カスタムフォーム
* リスク
* キューの設定情報
* ポートフォリオとプログラム
* 承認
* ドキュメント
* 元のテンプレートタスクの日数は、新規テンプレートに移行されます。必要に応じて、テンプレートの開始日または完了日を（スケジュールモードに応じて）変更し、テンプレートタスクの日付を更新する必要があります。

次の項目は、既存のテンプレートから新しいテンプレートにコピーされません。

* 請求レート
* ユーザーコメント

## テンプレートをコピーする

<!--ensure steps and casing on the fields and buttons is accurate with unshim-->

1. コピーするテンプレートに移動します。
1. ヘッダーのテンプレート名の右側にある&#x200B;**詳細** メニュー![詳細アイコン &#x200B;](assets/more-icon.png)をクリックし、**コピー**&#x200B;をクリックします。

   「**テンプレートをコピー**」ボックスが開きます。

   ![&#x200B; テンプレートボックスをコピー](assets/copy-template-box.png)

1. 「**新しいテンプレート名**」フィールドにテンプレートの名前を指定します。

   デフォルトでは、Workfrontは次のフォーマットに従って新しい名前を設定します：`Copy of Original template name`。

1. 元のテンプレートからすべてのタスクとテンプレートの割り当てを新しいテンプレートに移行する場合は、「**タスクとテンプレートに対するユーザーの割り当てを保持**」オプションを選択します。 テンプレートタスクの割り当て、およびテンプレート所有者とスポンサーがコピーされたテンプレートに転送されます。
1. 「**保存**」をクリックしてテンプレートのコピーを作成します。

   新しいテンプレートは、Workfrontのテンプレート領域のテンプレートリストに表示されます。
