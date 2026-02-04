---
product-area: Canvas Dashboards
navigation-topic: report-types
title: キャンバスダッシュボードでの通貨フィールドの使用
description: キャンバスダッシュボードで通貨フィールドを使用できます。
author: Courtney
feature: Reports and Dashboards
source-git-commit: f8c41105607e972d3395cf8d89fb1fdf29f0da85
workflow-type: tm+mt
source-wordcount: '630'
ht-degree: 10%

---


# キャンバスダッシュボードでの通貨フィールドの使用

>[!IMPORTANT]
>
>キャンバスダッシュボード機能は現在、ベータ版のステージに参加しているユーザーのみが利用できます。 この段階では、フィーチャの一部が完全でない、または意図したとおりに動作しない可能性があります。 キャンバスダッシュボードベータ版の概要記事の [ フィードバックの提供 ](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) の節の手順に従って、エクスペリエンスに関するフィードバックをお送りください。<br>
>バグまたは技術的な問題の可能性に関するご意見がある場合は、Workfront サポートにチケットを送信してください。 詳しくは、[ カスタマーサポートへのお問い合わせ ](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md) を参照してください。<br>
>このベータ版は、次のクラウドプロバイダーでは利用できません。
>
>* Amazon Web Services用に独自のキーを持参
>* Azure
>* Google Cloud Platform

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
<p>標準</p> 
<p>プラン</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベル設定</p></td> 
   <td><p>レポート、ダッシュボードおよびカレンダーへのアクセスを編集する</p>
   <p>財務データへのアクセスの表示</p>
  </td> 
  </tr> 
    </tr>  
        <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td><p>ダッシュボードの権限管理</p>
  </td> 
  </tr> 
</tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。
+++

## 前提条件

1. この記事に記載されている機能を使用するには、Workfront インスタンスに複数の通貨タイプを設定する必要があります。 詳しくは、「[ 為替レートの設定 ](/help/quicksilver/administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md) を参照してください。

   >[!IMPORTANT]
   >
   >この記事で説明されている機能は、ネイティブ通貨フィールドにのみ適用されます。 通貨の為替レートがある場合、カスタム通貨フィールドのサポートは近日中に設定されます。


## キャンバスダッシュボードのデフォルト通貨の設定

キャンバスダッシュボードを作成する際に、ダッシュボードのデフォルトの通貨を設定できます。 通貨フィールドがレポートレベルでロックされていない限り、この通貨は、ダッシュボードのレポートにすべてのネイティブ通貨フィールドを表示するために使用されます。

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
      <br> ユーザーは、ダッシュボードをフィルタリングする際に、異なる通貨タイプを切り替えることができます。</td>
     </tr>
    </tbody>
   </table>


## キャンバスダッシュボードの通貨の切り替え

ダッシュボードレベルで様々な通貨タイプを切り替えることができます。 通貨フィールドを含む報告書は、選択した通貨タイプを反映するように更新されます。

通貨フィールドは、レポートレベルでロックできます。 通貨フィールドがロックされている場合、ダッシュボードの通貨タイプを変更しても、そのレポートの通貨タイプは変更されません。

ダッシュボードの通貨タイプを変更するには、

1. ダッシュボードの詳細ページの右上隅にある「通貨」ドロップダウンメニューをクリックします。
1. リストから目的の通貨タイプを選択します。

   ![ 通貨ドロップダウンの変更 ](assets/filter-by-currency.png)


## 制限事項

次の表は、「設定」の「為替レート」領域で通貨を定義した場合の制限事項を示しています。

<table> 
<tr>
<td></td>
<td>ユーザーは次のことができます</td>
<td>ユーザーができません</td>
</tr>
<tr> 
<td>単一通貨が定義されている</td>
<td>
<ul>
<li>キャンバスグラフ、KPI、テーブルレポートでのネイティブ通貨フィールドの使用</li>
<li>キャンバスグラフ、KPI およびグラフレポートでのカスタム通貨フィールドの使用</li>
</ul>
</td>
<td>
<ul>
<li>（作成時またはダッシュボードの編集時に）デフォルト通貨をダッシュボードに割り当てる</li>
<li>ダッシュボードレベルの通貨切り替えを確認して使用します</li>
<li>キャンバスグラフ、KPI またはテーブルレポートで表示する特定の通貨をロック</li>
<li>キャンバス・チャート、KPI および表レポートでの計画通貨フィールドの使用</li>
</ul>
</td> 
</tr>
</td> 
</tr> 
<tr>
<td>多通貨が定義されています</td>
<td>
<ul>
  <li>キャンバスグラフ、KPI、テーブルレポートでのネイティブ通貨フィールドの使用</li>
  <li>（作成時またはダッシュボードの編集時に）ダッシュボードのデフォルト通貨を設定します</li>
  <li>ダッシュボードレベルの通貨切り替えを確認して使用します</li>
  <li>キャンバスグラフ、KPI またはテーブルレポートで表示する特定の通貨をロックして、ダッシュボードの通貨切り替えの環境設定を無視する</li>
</ul>
</td>
<td><ul>
  <li>キャンバスグラフ、KPI、テーブルレポートでのカスタムデータ通貨フィールドの使用</li>
  <li>キャンバス・チャート、KPI および表レポートでの計画通貨フィールドの使用</li>
</ul>
</td>
</tr></table>





