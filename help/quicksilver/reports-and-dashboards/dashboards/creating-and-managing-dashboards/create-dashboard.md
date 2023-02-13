---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: ダッシュボードの作成
description: ダッシュボードを作成して、レポート、カレンダー、外部ページの情報にすばやくアクセスできます。
author: Nolan
feature: Reports and Dashboards
exl-id: 6a284df4-f011-4b4c-b44c-2e20918f643f
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '459'
ht-degree: 0%

---

# ダッシュボードの作成

ダッシュボードを作成して、レポート、カレンダー、外部ページの情報にすばやくアクセスできます。

ダッシュボードについて詳しくは、 [ダッシュボードの概要](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## アクセス要件

以下が必要です。

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Adobe Workfront plan*</strong></p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Adobe Workfront license*</strong></p> </td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td><strong>アクセスレベル設定*</strong> </td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>オブジェクト権限</strong> </p> </td> 
   <td> <p>新しいダッシュボードに対する管理権限が取得されます</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.<br>ダッシュボードの権限について詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/permissions-reports-dashboards-calendars.md" class="MCXref xref">レポート、ダッシュボード、カレンダーの共有 </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

ダッシュボードに追加する前に、次のオブジェクトのいずれかを作成する必要があります。

* **レポート**:レポートの作成について詳しくは、 [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* **カレンダー**:カレンダーの作成について詳しくは、 [カレンダーレポートの概要](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

* **外部ページ**:外部ページの作成について詳しくは、 [外部 Web ページをダッシュボードに埋め込む](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## ダッシュボードの作成

1. メインメニューアイコンをクリックします。 ![](assets/main-menu-icon.png)を選択し、「 **ダッシュボード。**
1. クリック **新しいダッシュボード**.\
   [ 新しいダッシュボード ] ダイアログボックスが表示されます。

1. 以下を指定します。

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>名前</strong></td>
      <td><p>これは、ダッシュボードの名前です。</p><p>名前を指定しない場合、デフォルトでは、ダッシュボード上の最初のレポートの名前がダッシュボードの名前になります。</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>説明（オプション）</strong></td>
      <td>これは、ダッシュボードの説明です。</td>
     </tr>
    </tbody>
   </table>

1. レイアウトを選択するには、レイアウトの横にあるラジオボタンをクリックします。

   1 列のレイアウトがデフォルトです。

   ダッシュボードのレポートレイアウトについて詳しくは、 [ダッシュボードでのレポートの表示について](../../../reports-and-dashboards/dashboards/understanding-dashboards/understand-how-reports-display-dashboard.md).

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Consider adding the information from this article here, at some point, instead of linking to it.)
   </MadCap:conditionalText>
   -->

1. 既存のレポート、カレンダーまたは外部ページを検索して追加する **名前またはタイプで検索…** フィールドをドラッグし、リストに表示されたら、レイアウトペインにドラッグします。

   >[!NOTE]
   >
   >項目を検索すると、最近作成された 2,000 個のレポートのいずれかが返されます。 Unicode 文字を含むレポート名は、検索結果に返されません。 ベストプラクティスとして、別のソースから名前をコピー&amp;ペーストするのではなく、名前を入力して、Workfrontでオブジェクトに名前を付ける際に Unicode 文字を含めないでください。

   ![レポートの検索](assets/qs-new-dashboard-ui-0722.png)

1. （オプション）「 **外部ページを追加** をクリックして、ダッシュボードに外部ページを追加します。\
   外部ページの作成とダッシュボードへの埋め込みについて詳しくは、 [外部 Web ページをダッシュボードに埋め込む](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

1. クリック **保存して閉じる**.\
   ダッシュボードの右上隅にタイムスタンプが表示されます。 タイムスタンプには、ダッシュボードが最後に更新された日付、時間、タイムゾーンが含まれます。
