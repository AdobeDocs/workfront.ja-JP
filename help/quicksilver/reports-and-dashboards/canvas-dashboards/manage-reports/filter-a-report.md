---
product-area: Canvas Dashboards
navigation-topic: report-types
title: カンバスダッシュボードでのレポートのフィルタリング
description: レポートにフィルターを追加または編集して、Canvas ダッシュボードに表示するデータを制御します。
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
source-git-commit: dc9caae8cc85543986eaefb1d3debdebfdf6ce96
workflow-type: tm+mt
source-wordcount: '434'
ht-degree: 23%
---
# カンバスダッシュボードでのレポートのフィルタリング

>[!IMPORTANT]
>
>Canvas ダッシュボード機能は現在、ベータ版ステージに参加しているユーザーのみが利用できます。 機能の一部が完了していないか、この段階で意図したとおりに動作しない可能性があります。 ご利用のエクスペリエンスに関するフィードバックは、Canvas ダッシュボードのベータ版の概要記事の「[ フィードバックを提供](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback)」セクションの手順に従って送信してください。<br>
>バグや技術的な問題についてフィードバックがある場合は、Workfront サポートにチケットを送信してください。 詳しくは、[カスタマーサポートに連絡](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)を参照してください。<br>
>このベータ版は、次のクラウドプロバイダーでは利用できないことに注意してください。
>
>* Amazon Web Services用に独自のキーを持ち込む
>* Azure
>* Google Cloud Platform

レポートをフィルタリングして、レポートの作成中と後の任意のタイミングの両方で、どのデータを表示するかを制御できます。 フィルタリングオプションと動作は、どちらの場合も同じです。

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

フィルターを適用する前に、ダッシュボードにレポートを作成するか、ダッシュボードを作成している必要があります。 詳しくは、[ キャンバスダッシュボードの作成](/help/quicksilver/reports-and-dashboards/canvas-dashboards/create-dashboards/create-dashboards.md)を参照してください。

## レポートフィルターの追加または編集

レポートにフィルターを追加または編集するには：

1. レポートのフィルターパネルを開きます。

   * レポートを作成する場合は、**設定** ダイアログボックスの左側のパネルにある&#x200B;**フィルター** アイコンをクリックします。
   * 既存のレポートを編集する場合は、右上隅の&#x200B;**詳細** アイコンをクリックし、**編集**&#x200B;を選択してから、**設定** ダイアログボックスの&#x200B;**フィルター** パネルをクリックします。

1. 「**フィルターを編集**」をクリックします。

1. 「**条件を追加**」をクリックし、条件を定義します。

   * 「**フィールドを選択**」をクリックし、フィルタリングするフィールドを選択します。
   * フィールドが満たす必要がある条件を定義する修飾子を選択します。
   * モディファイヤに値が必要な場合は、評価する値を入力または選択します。

   ![条件を追加](assets/add-condition.png)

1. （オプション）前の手順を繰り返して、さらに条件を追加します。

1. （オプション）「**フィルターグループを追加**」をクリックして、別のフィルター条件のセットを追加します。 セット間のデフォルトの演算子は AND です。 演算子をクリックして OR に変更します。

>[!NOTE]
>
>フィールド、演算子、ワイルドカードおよび特殊フィルタールールの完全なリストについては、[ カンバスダッシュボードのフィルターリファレンスのレポート ](/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-reports/filter-reference.md)を参照してください。

1. 「**保存**」をクリックします。
