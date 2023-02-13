---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 配達確認の承認レポートを使用
description: 配達確認の承認レポートを使用して、環境内の配達確認に関する情報を表示できます。
author: Courtney
feature: Digital Content and Documents
exl-id: 4f8c924e-7c33-43f3-a9d6-75c56af28527
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '300'
ht-degree: 1%

---

# 配達確認の承認レポートを使用

配達確認の承認レポートを使用して、環境内の配達確認に関する情報を表示できます。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Workfront plan*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfrontライセンスの概要*</p> </td> 
   <td> <p>計画</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong>アクセスレベル*</strong> </td> 
   <td> <p>次へのアクセスを編集：</p> 
    <ul> 
     <li> <p>レポート、ダッシュボードおよびカレンダーの作成</p> </li> 
     <li> <p>フィルター、ビュー、グループの作成</p> </li> 
    </ul> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 配達確認の承認レポートを使用

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **レポート**.
1. クリック **新しいレポート**&#x200B;をクリックし、スクロールして「 」を選択します。 **配達確認の承認**.

   ![](assets/proof-approval-report.png)

1. （オプション）その他のフィールドを追加します。
1. クリック **保存して閉じる**.

## 追加のフィールド

次のフィールドを配達確認の承認レポートに追加できます。

* **決定日**:承認者が配達確認を決定した日付が表示されます。 この日付は、配達確認の印刷の概要でも確認できます。
* **承認者ステージ**:現在のステージ情報を表示します。
* **ワークフローテンプレート**:配達確認に関連付けられているワークフローテンプレートを表示します。 テンプレートが添付されていない場合、列は空白になります。
* **決定待ち**:次の条件に該当する場合、最新バージョンで決定が満たされていないことを示す場合、true を表示します。

   * 配達確認はアーカイブされていません
   * 承認者がいるステージがアクティブです
   * 配達確認は承認待ちです

* **配達確認期限**:配達確認の期限を表示します。 このフィールドに値を入力するには、すべてのステージに期限を割り当てる必要があります。 「 」フィールドには、最近アクティブ化されたステージの期限が表示されます。

 
