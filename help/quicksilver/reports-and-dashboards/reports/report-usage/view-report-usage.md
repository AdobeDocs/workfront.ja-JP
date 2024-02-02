---
product-area: reporting
navigation-topic: report-usage
title: レポートの使用状況を表示
description: レポートの使用状況を表示
author: Nolan
feature: Reports and Dashboards
exl-id: 51d9067c-8c55-433e-b560-7da241ef33ae
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: ht
source-wordcount: '997'
ht-degree: 100%

---

# レポートの使用状況を表示

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: : *** DO NOT CHANGE, REMOVE, CHANGE LINK, RENAME THIS ARTICLE- IT IS LINKED TO THE PENDO GUIDE FOR THE MAIN REPORTS AREA***)</p>
-->

システムでのレポートの広範な使用状況を把握するために、次の情報をレポートのリストに表示できます。

* レポートを閲覧した最近 10 人のユーザー
* 指定した時間枠内の閲覧数

  >[!NOTE]
  >
  >Adobe Workfront は、1 日に 1 人のユーザーにつき 1 回の表示とカウントします。ユーザーが同じレポートに 1 日に複数回アクセスしても、Workfront ではそのレポートを 1 回の表示とカウントします。同じ日に別のユーザーが同じレポートにアクセスすると、Workfront はこれを 2 人目のユーザーの新規表示としてカウントします。

* 最終表示日
* 最終表示者ユーザー
* レポートを含むダッシュボードのリスト\
  レポートのリストにレポートを追加できるダッシュボードの名前を表示する方法について詳しくは、[ダッシュボードでレポートを整理する方法](../../../reports-and-dashboards/reports/report-usage/understand-how-organize-reports-dashboard.md)の記事を参照してください。

この情報を表示できるレポートのリストのビューを作成できます。\
レポートのリストは、これらのフィールドの一部でフィルタリングできます。\
レポートにフィルターを適用する方法について詳しくは、[使用状況情報に基づいてレポートリストをフィルタリング](#filter-a-report-list-by-usage-information)を参照してください。

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
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスの編集</p> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## レポートの使用状況に関する情報を、レポートリストのビューに表示する

1. Workfront の右上隅で&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、「**レポート**」の順にクリックします。

1. レポートのリストで、**表示**&#x200B;ドロップダウンメニューをクリックします。
1. （オプション）**レポートの使用状況**&#x200B;ビューをクリックすると、最も一般的なレポート使用状況情報が表示されます。\
   または

1. 「**新しいビュー**」をクリックして、カスタムビューを作成します。
1. 「**列を追加**」をクリックします。
1. 次のフィールドのいずれかを入力し始め、**レポート**&#x200B;オブジェクトの下に表示されたらそれらを選択します。

   * **最近の 10 人のユーザー**：レポートを閲覧した直近 10 人のユーザーの名前が表示されます。
   * **件数**：次のいずれかの時間枠内のビュー数を表示します。

      * **現在の月／四半期／年を表示**
      * **先月、四半期、年**
      * **すべてのビュー**：レポートのすべてのビューの合計数を表示します

   * **最終表示者**：最後にレポートを表示したユーザーに関する情報を表示します
   * **最終表示日**：レポートが最後に表示された日付を表示します

1. 「**ビューを保存**」をクリックします。\
   レポートの使用状況情報が、ビューに追加した列に表示されます。\
   また、レポートオブジェクトのレポートを作成し、このビューをレポートで使用することもできます。\
   レポートの作成について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。\
   レポートを作成するには、アクセスレベルにレポートへの編集アクセス権が必要です。\
   レポートへのアクセス権について詳しくは、[レポート、ダッシュボードおよびカレンダーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)を参照してください。

## 使用情報によるレポートリストのフィルタリング {#filter-a-report-list-by-usage-information}

1. Workfront の右上隅で&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、次に「**報告書**」をクリックします。
1. レポートのリストで、**フィルター**&#x200B;ドロップダウンメニューをクリックします。
1. 「**新規フィルター**」をクリックし、次に「**フィルター規則の追加**」をクリックします。
1. 次のフィールドのいずれかに入力を開始し、**報告書**&#x200B;オブジェクトの下のリストに表示されたら、それらを選択して、新しいフィルター規則として追加します。

   * **ビュー**：次のいずれかの期間内のビューの件数を表示します。

      * **今月／今四半期／今年**
      * **先月、前四半期、昨年**
      * **すべてのビュー**

   * **最終表示者**：最後にレポートを表示したユーザーに関する情報を表示します
   * **最終表示日**：最後にレポートが表示された日付を表示します

1. フィールドの修飾子を選択し、プロンプトが表示されたら値を指定します。\
   ![](assets/qs-report-usage-filter-statistics-350x150.png)

1. 「**フィルターの保存**」をクリックします。\
   これにより、定義した使用情報に合致するレポートのリストが表示されます。\
   また、レポートオブジェクトのレポートを作成し、このフィルターをレポートで使用することもできます。\
   レポートの作成について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)の記事を参照してください。レポートを作成するには、アクセスレベルにレポートへの編集アクセス権が必要です。\
   レポートへのアクセス権について詳しくは、[レポート、ダッシュボード、カレンダーへのアクセス権の付与](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)の記事を参照してください。

## レポート使用情報を閲覧する際の例外

>[!IMPORTANT]
>
>レポート使用情報は、2018年3月以降に収集されています。この日付より前の情報は入手できません。

レポート使用情報を扱う際に留意すべき例外は次のとおりです。

* レポートがダッシュボードやカスタムタブに表示されるたびに、1 つのビューとしてカウントされます。そのレポートをダッシュボードに表示しているユーザーが「最終表示者」ユーザーとして表示され、ダッシュボードが表示された日付が最終表示日として表示されます。
* Workfront では、組み込みレポートの使用情報を収集しません。\
  Workfront の組み込みレポートについて詳しくは、[Adobe Workfront の組み込みレポートの使用](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)を参照してください。

* Workfront では、配信されたレポートの使用情報を収集しません。配信されたレポートは 1 つのビューとしてカウントされません。\
  配信されたレポートについて詳しくは、[レポート配信の概要](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)の記事を参照してください。

* システム管理者またはグループ管理者が別のユーザーとしてログインすると、ビューがカウントされ、そのシステム管理者またはグループ管理者に関連付けられます。
* Workfront では、レポートの使用情報をカスタム四半期ごとに収集しません。レポート使用フィールドでは、組み込みの標準四半期のみが参照されます。
* Workfront では、共有され公開されているレポートの使用情報を収集しません。ユーザーが Workfront にログインせずに公開レポートを閲覧した場合、そのレポートの表示回数はカウントされません。\
  レポートの共有について詳しくは、[Adobe Workfront でのレポートの共有](../../../reports-and-dashboards/reports/creating-and-managing-reports/share-report.md)の記事を参照してください。
