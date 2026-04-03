---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 'Filter: Proof Approval Report to Omit Previous Proof Versions'
description: プルーフの承認レポートでは、「現在のドキュメントのバージョン」フィルターを使用して、承認待ちのプルーフの現在のバージョンのみを含めることができるようになりました。
author: Courtney
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
last-update: 2026-04-01T18:03:50Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
source-git-commit: 18301970abddd8ed98abccf42562d950422bfa7c
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 48%

---

# フィルター：プルーフの以前のバージョンを省略するプルーフの承認レポート

<!--Audited: 10/2024-->

プルーフの承認レポートでは、**現在のドキュメントバージョン** フィルターを使用して、承認待ちのプルーフの現在のバージョンのみを含めることができます。

これは、例えば、複数のバージョンを持つプルーフの承認を求められた場合に役に立ちます。「現在のドキュメントのバージョン」フィルターを使用してプルーフ承認レポートを実行すると、そのレポートには、承認を待っている各プルーフの現在のバージョンのみが一覧表示され、作業する必要がなくなった以前のバージョンは除外されます。

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
   <p>コントリビューターまたはフィルターを変更するリクエスト </p>
   <p>レポートを修正する標準または計画</p>
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルターを変更する場合は、フィルター、ビュー、グループ化への編集アクセス権</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## プルーフ承認レポートをフィルタリングしてプルーフの以前のバージョンを除外

プルーフ承認レポートのフィルターを作成できます。

1. 既にプルーフの承認レポートがある場合は、そのレポートを開きます。

   または

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   独自のプルーフ承認レポートを作成するには、右上隅の&#x200B;**メインメニュー** アイコン ![ メインメニューアイコン ](assets/main-menu-icon.png)、または左上隅の&#x200B;**メインメニュー** アイコン ![ メインメニューライン ](assets/lines-main-menu.png)をクリックします。使用可能な場合は、**レポート** ![ レポートアイコン ](assets/reports-in-main-menu.png)をクリックします。

1. 「**新規レポート**」をクリックします。 オブジェクトタイプのリストが表示されます。
1. リストの&#x200B;**プルーフ承認**をクリックします。
レポートビルダーが開きます。
1. 「**フィルター**」、「**フィルタールールを追加**」の順にクリックします。

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. 「**フィルターのルールを設定」ボックス内をクリックし、リストから「** プルーフの承認&#x200B;**」を選択します。**
1. **プルーフ承認** オブジェクトのリストで、**現在のドキュメント バージョン**&#x200B;をクリックします。
1. フィルター修飾子に「等しい」を選択し、「True」を選択します。
1. Adobe Workfrontの左下隅にある&#x200B;**保存+閉じる**&#x200B;をクリックし、表示されるボックスで&#x200B;**適用**&#x200B;をクリックします。

   プルーフの承認がこのフィルター条件に一致する場合、プルーフの承認レポートには、ドキュメントの現在のバージョンに関連付けられたプルーフのみが表示されます。
