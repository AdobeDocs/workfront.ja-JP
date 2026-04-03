---
product-area: Canvas Dashboards
navigation-topic: report-types
title: キャンバスダッシュボードの作成
description: Canvas ダッシュボードでは、カスタマイズ可能なダッシュボードでレポートを作成し、追加することで、アカウントデータをすばやく視覚化できます。
author: Courtney
feature: Reports and Dashboards
exl-id: bd31e426-7c4a-4ff8-9432-c95dc8ee3743
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 17%

---

# キャンバスダッシュボードの作成

>[!IMPORTANT]
>
>Canvas ダッシュボード機能は現在、ベータ版ステージに参加しているユーザーのみが利用できます。 機能の一部が完了していないか、この段階で意図したとおりに動作しない可能性があります。 ご利用のエクスペリエンスに関するフィードバックは、Canvas ダッシュボードのベータ版の概要の記事の「[ フィードバックを提供](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback)」セクションの指示に従って送信してください。<br>
>バグや技術的な問題についてフィードバックがある場合は、Workfront サポートにチケットを送信してください。 詳しくは、[ カスタマーサポートにお問い合わせください](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>を参照してください
>このベータ版は、次のクラウドプロバイダーでは利用できないことに注意してください。
>
>* Amazon Web Services用に独自のキーを持ち込む
>* Azure
>* Google Cloud Platform

Canvas ダッシュボードでは、カスタマイズ可能なダッシュボードでレポートを作成し、追加することで、アカウントデータをすばやく視覚化できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront パッケージ</p></td> 
   <td> 
<p>任意 </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン</p></td> 
   <td> 
<p>標準 </p> 
<p>プラン</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベル設定</p></td> 
   <td><p>レポート、ダッシュボードおよびカレンダーへのアクセスを編集する</p>
  </td> 
  </tr>  
</tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。
+++

## 前提条件

カンバスダッシュボードは、左側のナビゲーション項目のダッシュボードページのレイアウトテンプレート設定で有効にする必要があります。

## ダッシュボードの作成

Canvas ダッシュボードには、ダッシュボードを作成するときに使用できる様々なオプションと設定が用意されています。 このセクションでは、ダッシュボードの作成の一般的なプロセスについて説明します。

{{step1-to-dashboards}}

1. 左側のパネルで、「**キャンバスダッシュボード**」をクリックします。

1. 右上隅の「**新しいダッシュボード**」をクリックします。

1. **ダッシュボードを作成** ボックスで，

1. 以下を指定します。

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>名前</strong></td>
      <td><p>ダッシュボードの名前を入力します。 互換性の問題を回避するために、UTF-8文字のみを使用することをお勧めします。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>説明（オプション）</strong></td>
      <td>ダッシュボードの説明を入力します。</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>通貨</strong></td>
      <td>ダッシュボードのデフォルトの通貨タイプを選択します。 <br>
      <br> ユーザーは、ダッシュボードをフィルタリングする際に、異なる通貨タイプを切り替えることができます。 詳しくは、<a href="/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/filter-canvas-dashboard.md">通貨タイプ別にダッシュボードをフィルタリング </a>するを参照してください。</td>
     </tr>
    </tbody>
   </table>

1. 「**作成**」をクリックします。**レポートを追加ボックス**&#x200B;が開きます。 ここから、新しいレポートを作成したり、既存のレポートをダッシュボードに追加したりできます。

## ダッシュボードへのレポートを追加

ダッシュボードを作成したら、次のステップはそのダッシュボードにレポートを追加することです。 これは、カンバスダッシュボードセクションでゼロからレポートを作成するか、既存のレポートを追加することで可能です。

Canvas ダッシュボードで作成できるレポートには、次の3つの種類があります。

* **KPI**：このレポートには、主要業績評価指標データが数値として表示されます。
詳しくは、[KPI レポートの作成](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-kpi-report.md)を参照してください。

* **グラフ**：このレポートには、データが棒グラフ、列グラフ、折れ線グラフまたは円グラフとして表示されます。
詳しくは、[ チャートレポートの作成](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md)を参照してください。

* **表**：このレポートでは、データが表形式で表示されます。
詳しくは、[ テーブルレポートの作成](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-table-report.md)を参照してください。

既存のレポートをダッシュボードに追加する方法について詳しくは、[既存のレポートをダッシュボードに追加](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/add-existing-report.md)を参照してください。
