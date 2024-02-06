---
content-type: reference
product-area: reporting
navigation-topic: custom-view-filter-and-grouping-samples
title: 「レポート：予算計上時間数」
description: 「レポート：予算計上時間数」
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: 2c0b60a6-fae4-4b29-8243-2a7f7d1f574b
source-git-commit: 332c744ab9b760268620461ed2cb2551caf383cf
workflow-type: tm+mt
source-wordcount: '657'
ht-degree: 94%

---

# レポート：予算計上時間数

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: From&nbsp;Alina: This is my article, but since it's about building a report, it is in the Reporting section. Please don't remove it -it's linked to Resource Management and it is super important.) </p>
-->

リソースプランナーへのアクセス権がない他のユーザーと予算計上時間数の情報を共有したい場合は、予算計上時間数のレポートを作成することで共有できます。そのレポートを他のユーザーと共有できます。

>[!IMPORTANT]
>
>予算時間は、通常、Adobe Workfrontデータベースで 1 時間ごとに更新されます（まれに、最大 3 時間かかる場合があります）。 レポートを更新しても、そのレポート内の時間数の情報は必ずしも更新されるわけではありません。前回のアップデート以降の経過時間は、それぞれの予算計上時間数のレポートの右上隅に表示されます。レポートを更新すると、前回のアップデートから 1 時間以上経過した場合にのみ、レポート内の情報がアップデートされます。
>
>![](assets/budgeted-hour-report-time-sync-warning-350x74.png)>

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
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集</p> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 予算計上時間数のレポートを作成

1. 右上隅にある&#x200B;**メインメニュー** ![](assets/main-menu-icon.png) をクリックし、「**レポート**」をクリックします。

1. **新規レポート／予算時間**&#x200B;の順にクリックします。

   デフォルトのビューがレポートに適用されます。

1. （オプション）レポートを読みやすくするには、**予算計上時間数**&#x200B;の列、「**テキストモードに切り替え**」の順にクリックし、続けて次の行を

   ```
   valuefield
   ```

   下記のように変更し

   ```
   valueexpreesion
   ```

   丸め式を入力します。

   これにより、予算時間数が指定した小数点以下の桁数に丸められます。

   Workfrontで数値を丸める方法について詳しくは、 [計算データ式の概要](../../../reports-and-dashboards/reports/calc-cstm-data-reports/calculated-data-expressions.md).

1. （オプション）「**列を追加**」をクリックして、列を追加します。
1. （オプション）レポートを読みやすくするために、そのレポートにグループ化を追加することをお勧めします。以下のグループ化をお勧めします。

   「**グループ化**」タブをクリックし、次の操作のいずれかを行います。

   1. 「**グループ化を追加**」をクリックして、「プロジェクト名」を入力し、リストに表示されたら選択します。
   1. 「**グループ化を追加**」をクリックして、「担当業務名」を入力し、リストに表示されたら選択します。
   1. 「**グループを追加**」をクリックして、「**配分日**」を入力し、リストに表示されたら選択します。さらに、「**日付をグループ化**」フィールドからグループ化する期間を選択します。

1. （オプション）「**フィルター**」をクリックして、レポートにフィルターを追加します。
1. （オプション）「**グラフ**」をクリックして、レポートにグラフを追加します。
1. 「**保存して閉じる**」をクリックします。

## 予算計上時間数のレポートを確認

デフォルトでは、以下の情報が予算計上時間数のレポートに表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">プロジェクト </td> 
   <td>予算計上時間数に関連付けられたプロジェクトの名前です。</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>担当業務</p> </td> 
   <td>予算計上時間数に関連付けられた担当業務の名前です。 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">ユーザー</td> 
   <td>予算計上時間数に関連付けられたユーザーの名前です。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">配分日</td> 
   <td> <p>配分日です。時間数を予算計上する週の最初の日（日曜日）です。</p> <p>ヒント：  <p>週が 2 か月にまたがる場合、レポートには 2 つの行が作成されます。1 行目は週の最初の日（最初の月の日曜日）に対応し、2 行目は 2 か月目の最初の日（任意の曜日）に対応します。</p> <p>例えば、あるユーザーに対して 6月30日（日曜日）～ 7月6日（土曜日）（PT）の週に 8 時間の予算を計上した場合、2 つの行には 6月30日と 7月1日の配分日が表示されます。</p> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">予算計上時間数</td> 
   <td>リソースプランナーのユーザーに割り当てられた予算計上時間数です。</td> 
  </tr> 
  <tr> 
   <td role="rowheader">予定予算計上時間数</td> 
   <td>これは、リソースプランナーで担当業務やプロジェクトに割り当てられている予算計上時間数です。</td> 
  </tr> 
 </tbody> 
</table>
