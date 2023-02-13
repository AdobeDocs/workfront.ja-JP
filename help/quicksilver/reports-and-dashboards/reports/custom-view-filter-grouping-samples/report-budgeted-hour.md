---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 'レポート：予算時間'
description: 'レポート：予算時間'
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '640'
ht-degree: 1%

---

# レポート：予算時間

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resouce Management and it is super important.) </p>
-->

予算時間情報を、リソース・プランナにアクセスできない他のユーザーと共有する場合は、予算時間レポートを作成します。 その後、レポートをユーザーと共有できます。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This info is also added and drafted in the article "View Budget Hours in a report" in the Resource Planning section. Consider deleting this article?!)</p>
-->

>[!IMPORTANT]
>
>予算時間は、Adobe Workfrontデータベースの 1 時間ごとに更新されます。 レポートを更新しても、そのレポート内の時間情報は必ずしも更新されるわけではありません。 前回の更新以降の経過時間を、各予算時間レポートの右上隅に表示できます。 レポートを更新すると、前回の更新から 1 時間以上経過した場合にのみ、レポート内の情報が更新されます。
>
>![](assets/budgeted-hour-report-time-sync-warning-350x74.png)>

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

## 予算時間レポートの作成

1. 次をクリック： **メインメニュー** ![](assets/main-menu-icon.png) 右上隅で、「 **レポート**.

1. クリック **新規レポート/予算時間**.

   デフォルトのビューがレポートに適用されます。

1. （オプション）レポートを読みやすくするには、 **予算時間** 列、 **テキストモードに切り替え**&#x200B;をクリックし、

   ```
   valuefield
   ```

   行

   ```
   valueexpreesion
   ```

   丸め式を入力します。

   予算時間数を指定した小数に丸めます。

   Workfrontで数値を丸める方法について詳しくは、 [計算データ式](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. （オプション）「 **列を追加** をクリックして、列を追加します。
1. （オプション）レポートを読みやすくするために、そのレポートにグループを追加することをお勧めします。 次のグループ化をお勧めします。

   次をクリック： **グループ化** 」タブに移動し、次のいずれかの操作を行います。

   1. クリック **グループを追加** 「プロジェクト名」と入力し、リストに表示されたら選択します。
   1. クリック **グループを追加** 「Job Role Name」と入力し、リストに表示されたら選択します。
   1. クリック **グループを追加** 入力を開始 **配分日**&#x200B;を選択し、リストに表示されるタイミングを選択して、グループ化する期間を **日付のグループ化基準** フィールドに入力します。

1. （オプション）「 **フィルター** ：レポートにフィルターを追加します。
1. （オプション）「 **グラフ** をクリックして、レポートにグラフを追加します。
1. クリック **保存して閉じる**.

## 予算時間レポートの確認

デフォルトでは、次の情報が予算時間レポートに表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">プロジェクト </td> 
   <td>これは、予算時間に関連付けられたプロジェクトの名前です。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>ジョブの役割</p> </td> 
   <td>予算時間に関連付けられたジョブ・ロールの名前です。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ユーザー</td> 
   <td>これは、予算時間に関連付けられたユーザーの名前です。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">配分日</td> 
   <td> <p>これは配分日です。 時間を予算化する週の最初の日（日曜日）です。</p> <p>ヒント：  <p>週が 2 か月にわたる場合、レポートには 2 行が表示されます。1 つは週の最初の日（最初の月の日曜日）に対応する日、もう 1 つは 2 番目の月の最初の日（どの曜日でもかまいません）に対応する日です。</p> <p>例えば、6 月 30 日（日曜日）～7 月 6 日（土曜日）の週にユーザーの 8 時間を予算した場合、2 つの行には「配分日」が 6 月 30 日と 7 月 1 日と表示されます。</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">予算計上時間数</td> 
   <td>これは、リソース・プランナのユーザーに割り当てられた予算時間です。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">プラン 予算計上時間数</td> 
   <td>これは、リソース・プランナのジョブ・ロールまたはプロジェクトに割り当てられる予算時間です。</td> 
  </tr> 
 </tbody> 
</table>
