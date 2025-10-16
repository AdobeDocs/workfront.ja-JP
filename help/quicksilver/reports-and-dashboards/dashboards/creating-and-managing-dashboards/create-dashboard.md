---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: ダッシュボードの作成
description: ダッシュボードを作成して、Adobe Workfrontの情報にすばやくアクセスできます。レポート、カレンダー、外部ページをダッシュボードに追加して他の人たちと共有し、最適なコラボレーションを実現できます。
author: Nolan
feature: Reports and Dashboards
exl-id: 6a284df4-f011-4b4c-b44c-2e20918f643f
source-git-commit: c8b7ad473b0c2120ef5ea52374b3501ad6f553f1
workflow-type: tm+mt
source-wordcount: '494'
ht-degree: 81%

---

# ダッシュボードの作成

<!--Audited: 01/2025-->

ダッシュボードを作成して、Adobe Workfrontの情報にすばやくアクセスできます。最大 25 個の報告書、カレンダー、外部ページをダッシュボードに追加して、他のユーザーと共有して共同作業を最適化できます。

ダッシュボードについて詳しくは、[ダッシュボードの基本を学ぶ](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md)を参照してください。

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
   <td> 
      <p>標準</p>
      <p>プラン</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボードおよびカレンダーへのアクセスを編集する</p></td> 
  </tr>  
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>作成したダッシュボードに対する管理権限を取得します。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

次のオブジェクトのいずれかをダッシュボードに追加するには、まずそれらを作成する必要があります。

* **レポート**：レポートの作成については、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。

* **カレンダー**：カレンダーの作成については、[カレンダーレポートの概要](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md)を参照してください。

既存の外部ページをダッシュボードに追加することも、新しいダッシュボードからページを作成することもできます。外部ページの作成について詳しくは、[外部 web ページをダッシュボードに埋め込む](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)を参照してください。

## ダッシュボードの作成

{{step1-to-dashboards}}

1. 「**新規ダッシュボード**」をクリックします。\
   新規ダッシュボードダイアログボックスが表示されます。

1. 以下を指定します。

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>名前</strong></td>
      <td><p>これはダッシュボードの名前です。 互換性の問題を回避するには、UTF-8 文字のみを使用することをお勧めします。</p><p>名前を指定しない場合、ダッシュボード上の最初のレポートの名前がデフォルトでダッシュボードの名前になります。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>説明（オプション）</strong></td>
      <td>ダッシュボードの説明です。</td>
     </tr>
    </tbody>
   </table>

1. レイアウトを選択するには、**レイアウトを選択／レポートを追加／カレンダーを追加**&#x200B;セクションの上部にある、対応するラジオボタンをクリックします。これは、レポート、カレンダー、外部ページがダッシュボードに表示されるレイアウトです。

   1 列レイアウトがデフォルトになります。

   ダッシュボードのレポートレイアウトについては、[ダッシュボードでのレポートの表示について](../../../reports-and-dashboards/dashboards/understanding-dashboards/understand-how-reports-display-dashboard.md)を参照してください。

   <!--
   Consider adding the information from this article above here, at some point, instead of linking to it.)
   -->

1. [**利用可能な報告書とカレンダー**] セクションで、検索バーに報告書、カレンダー、または外部ページの名前を入力し始め、レイアウト ウィンドウで、右側に報告書、カレンダー、または外部ページをドラッグ アンド ドロップします。

   >[!NOTE]
   >
   >項目を検索すると、最近作成された 2,000 個のレポートから検索結果が返されます。Unicode 文字を含んだレポート名は、検索結果には含まれません。ベストプラクティスとしては、Workfront でオブジェクトに名前を付ける際に、名前を別のソースからコピー＆ペーストするのではなく手入力することで、Unicode 文字が含まれないようにします。

   ![レポートの検索](assets/unshimmed-dashboard-ui.png)

1. （オプション）「**外部ページを追加**」をクリックして、ダッシュボードに外部ページを追加します。

   外部ページの作成とダッシュボードへの埋め込みについて詳しくは、[ダッシュボードへの外部 web ページの埋め込み](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md)を参照してください。

1. 「**保存して閉じる**」をクリックします。

   ダッシュボードの右上隅にタイムスタンプが表示されます。このタイムスタンプには、ダッシュボードが最後に更新された日付、時刻およびタイムゾーンが含まれています。
