---
product-area: Canvas Dashboards
navigation-topic: report-types
title: カンバスダッシュボードでのレポートデータのグループ化
description: レポートの結果をグループ化する： グループ化の仕組みは、レポートタイプによって異なります。
author: Courtney
feature: Reports and Dashboards
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: aa2f3246-cb95-4b30-8899-fdf7d73550cc
    internal-label: Reporting
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 375d62fc12af075c2224f979d3ef87cdffdf03ea
workflow-type: tm+mt
source-wordcount: '484'
ht-degree: 14%
---
# カンバスダッシュボードでのレポートデータのグループ化

>[!IMPORTANT]
>
>Canvas ダッシュボード機能は現在、ベータ版ステージに参加しているユーザーのみが利用できます。 機能の一部が完了していないか、この段階で意図したとおりに動作しない可能性があります。 ご利用のエクスペリエンスに関するフィードバックは、Canvas ダッシュボードのベータ版の概要記事の「[ フィードバックを提供](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback)」セクションの手順に従って送信してください。<br>
>バグや技術的な問題についてフィードバックがある場合は、Workfront サポートにチケットを送信してください。 詳しくは、[カスタマーサポートに連絡](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)を参照してください。<br>
>このベータ版は、次のクラウドプロバイダーでは利用できないことに注意してください。
>
>* Amazon Web Services用に独自のキーを持ち込む
>* Azure
>* Google Cloud Platform

グループ化によってレポート結果が整理され、関連するレコードが一緒に表示されます。 グループ化の仕組みはレポートタイプによって異なるため、この記事では、それぞれのレポートについて個別のセクションを用意しています。

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
  </td> 
  </tr>  
        <tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td><p>ダッシュボードの権限の管理</p>
  </td> 
  </tr>
</tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。
+++

## 前提条件

データをグループ化する前に、ダッシュボードにレポートを作成するか、ダッシュボードを作成している必要があります。 詳しくは、[ キャンバスダッシュボードの作成](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md)を参照してください。

## 表レポートの行をグループ化

テーブル レポートでは、グループ化によってレポート自体の行が整理されます。

1. **設定** ダイアログボックスで、左側のパネルの&#x200B;**グループ設定** アイコンをクリックします。

1. 「**グループ化を追加**」をクリックし、グループ化するフィールドを選択します。 グループ化は、右側のプレビューに表示されます。

1. （オプション）を繰り返して、グループ化をさらに追加します。

## グラフおよびKPI レポートでのドリルダウン グループの設定

グラフおよびKPI レポートでは、メインのビジュアライゼーションはグループ化されません。 代わりに、ビューアが値をドリルダウンする際に、ドリルダウンテーブルをグループ化する方法を設定します。

1. **設定** ダイアログボックスで、左側のパネルの&#x200B;**ドリルダウングループ設定** アイコンをクリックします。

1. 「**グループ化を追加**」をクリックし、ドリルダウンテーブルをグループ化するフィールドを選択します。

## ピボットテーブルレポートでのセグメントの設定

ピボットテーブルレポートでは、グループ化は使用されません。 代わりに、ピボットの指標がグループ化され、合計されるカテゴリである、最大2つのセグメントを定義します。

1. **設定** ダイアログボックスで、左側のパネルの&#x200B;**セグメント** アイコンをクリックします。

1. 「**セグメントを追加**」をクリックし、必要なフィールドを選択します。 セグメントは、プレビューに列として表示されます。

1. （オプション）繰り返して2番目のセグメントを追加します。 最大2つのセグメントを追加できます。

## ダッシュボードでのグループ化されたデータの表示

レポートビューアーは、グループ化されたデータを展開、折りたたみ、並べ替えることができます。 詳しくは、[Canvas ダッシュボードを使用](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md)の「[ グループ化されたデータを使用したレポートの表示](/help/quicksilver/reports-and-dashboards/canvas-dashboards/use-canvas-dashboards.md#view-reports-with-grouped-data)」を参照してください。
