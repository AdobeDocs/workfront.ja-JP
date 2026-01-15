---
product-area: Canvas Dashboards
navigation-topic: report-types
title: キャンバスダッシュボードの作成
description: キャンバスダッシュボードを使用すると、カスタマイズ可能なダッシュボードにレポートを作成および追加して、アカウントデータをすばやく視覚化できます。
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: bd31e426-7c4a-4ff8-9432-c95dc8ee3743
source-git-commit: 507cb64eb21c2798cdafe184794c0d9ed7ebc0c6
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 15%

---

# キャンバスダッシュボードの作成

>[!IMPORTANT]
>
>キャンバスダッシュボード機能は現在、ベータ版のステージに参加しているユーザーのみが利用できます。 この段階では、フィーチャの一部が完全でない、または意図したとおりに動作しない可能性があります。 キャンバスダッシュボードベータ版の概要記事の [&#x200B; フィードバックの提供 &#x200B;](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) の節の手順に従って、エクスペリエンスに関するフィードバックをお送りください。<br>
>バグまたは技術的な問題の可能性に関するご意見がある場合は、Workfront サポートにチケットを送信してください。 詳しくは、[&#x200B; カスタマーサポートへのお問い合わせ &#x200B;](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md) を参照してください。<br>
>このベータ版は、次のクラウドプロバイダーでは利用できません。
>
>* Amazon Web Services用に独自のキーを持参
>* Azure
>* Google Cloud Platform

キャンバスダッシュボードを使用すると、カスタマイズ可能なダッシュボードにレポートを作成および追加して、アカウントデータをすばやく視覚化できます。

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

キャンバスダッシュボードは、ダッシュボード ページの左側のナビゲーション項目のレイアウトテンプレート設定で有効にする必要があります。

## ダッシュボードの作成

キャンバスダッシュボードには、ダッシュボードの作成時に使用できる様々なオプションと設定が用意されています。 この節では、ダッシュボードを作成するための一般的なプロセスを説明します。

{{step1-to-dashboards}}

1. 左側のパネルで、「**キャンバスダッシュボード**」をクリックします。

1. 右上隅の **新規ダッシュボード** をクリックします。

1. **ダッシュボードを作成** ボックスで、

1. 以下を指定します。

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>名前</strong></td>
      <td><p>ダッシュボードの名前を入力します。 互換性の問題を回避するには、UTF-8 文字のみを使用することをお勧めします。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>説明（オプション）</strong></td>
      <td>ダッシュボードの説明を入力します。</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>通貨</strong></td>
      <td>ダッシュボードのデフォルトの通貨タイプを選択します。 <br>
      <br> ユーザーは、ダッシュボードをフィルタリングする際に、異なる通貨タイプを切り替えることができます。 詳しくは、<a href="/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/filter-canvas-dashboard.md"> 通貨タイプでダッシュボードをフィルタリングする </a> を参照してください。</td>
     </tr>
    </tbody>
   </table>

1. 「**作成**」をクリックします。**レポートを追加ボックス** が開きます。 ここから、新しいレポートを作成したり、既存のレポートをダッシュボードに追加したりできます。

## ダッシュボードへのレポートを追加

ダッシュボードを作成したら、次の手順でレポートを追加します。 これを行うには、「キャンバスダッシュボード」セクションでゼロからレポートを作成するか、既存のレポートを追加します。

キャンバスダッシュボードで作成できるレポートは 3 種類あります。

* **KPI**：このレポートには、主要業績評価指標データが数値で表示されます。
詳しくは、[KPI レポートの作成 &#x200B;](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-kpi-report.md) を参照してください。

* **グラフ**：このレポートは、データを棒グラフ、列グラフ、折れ線グラフ、円グラフとして表示します。
詳しくは、[&#x200B; グラフレポートの作成 &#x200B;](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md) を参照してください。

* **表**：このレポートは、データを表形式で表示します。
詳しくは、[&#x200B; テーブルレポートの作成 &#x200B;](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-table-report.md) を参照してください。

ダッシュボードに既存のレポートを追加する方法については、「[&#x200B; ダッシュボードに既存のレポートを追加する &#x200B;](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/add-existing-report.md)」を参照してください。
