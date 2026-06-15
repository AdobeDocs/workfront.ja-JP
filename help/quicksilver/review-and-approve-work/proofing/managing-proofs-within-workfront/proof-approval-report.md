---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: プルーフの承認レポートを使用する
description: プルーフの承認レポートを使用して、環境内のプルーフに関する情報を表示できます。
author: Courtney
feature: Digital Content and Documents
exl-id: 4f8c924e-7c33-43f3-a9d6-75c56af28527
TQID: https://experienceleague.adobe.com/ZU6Ej5QhI7v9zoAxurBz1YsFVIuVIh2a8tR2h6vYL18
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: a2241fa21f51f8146c1f3725d2ba2235f8458ab4
workflow-type: tm+mt
source-wordcount: 310
ht-degree: 77%

---

# プルーフの承認レポートを使用する

プルーフの承認レポートを使用して、環境内のプルーフに関する情報を表示できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Workfront パッケージ</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront プラン</p> </td> 
   <td> 
   <p>標準</p>
   <p>プラン</p>
   </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"><strong> アクセスレベル設定</strong> </td> 
   <td> <p>次へのアクセスを編集：</p> 
    <ul> 
     <li> <p>レポート、ダッシュボードおよびカレンダーの作成</p> </li> 
     <li> <p>フィルター、ビュー、グループ化を作成</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## プルーフの承認レポートを使用する

{{step1-to-reports}}

1. 「**新規レポート**」をクリックしてスクロールし、「**プルーフの承認**」を選択します。

   ![&#x200B; プルーフ承認レポート &#x200B;](assets/proof-approval-report.png)

1. （オプション）その他のフィールドを追加します。
1. 「**保存して閉じる**」をクリックします。

## その他のフィールド

以下のフィールドをプルーフの承認レポートに追加できます。

* **決定日**：承認者がプルーフに対して決定を行う日付が表示されます。 この日付は、プルーフの「サマリーを印刷」でも確認できます。
* **承認者ステージ**：現在のステージ情報が表示されます。
* **ワークフローテンプレート**：プルーフに添付されているワークフローテンプレートが表示されます。 テンプレートが添付されていない場合、列は空白になります。
* **決定待ち**：以下に該当する場合、最新バージョンで決定が下されていないことを示す「true」が表示されます。

   * プルーフがアーカイブされていない
   * 承認者がいるステージがアクティブになっている
   * プルーフが承認待ち

* **プルーフの期限**：プルーフの期限が表示されます。 このフィールドに値を入力するには、すべてのステージに期限を割り当てる必要があります。 このフィールドには、直近にアクティベートされたステージの期限が表示されます。

## 「承認者決定」フィールドについて

「承認者の決定」フィールドには、受信者がプルーフに対して行った決定が表示されます。 場合によっては、このフィールドには決定値の代わりにハイフン（ – ）が表示されます。これは、受信者がプルーフの意思決定の役割を果たしていないことを示します。 詳細については、「[承認者の決定で、承認のプルーフ レポートにハイフンが表示される](../tips-tricks-and-troubleshooting/approver-decision-shows-hyphen.md)」を参照してください。

 
