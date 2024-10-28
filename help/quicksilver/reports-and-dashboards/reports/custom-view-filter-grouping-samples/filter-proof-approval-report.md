---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 「フィルター：以前のプルーフのバージョンを削除するプルーフ承認レポート」
description: プルーフの承認レポートでは、「現在のドキュメントのバージョン」フィルターを使用して、承認待ちのプルーフの現在のバージョンのみを含めることができるようになりました。
author: Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 7b25d3b5fe69f610e245db5ada116ea967f22c7b
workflow-type: tm+mt
source-wordcount: '385'
ht-degree: 48%

---

# フィルター：プルーフの以前のバージョンを省略するプルーフの承認レポート

<!--Audited: 10/2024-->

プルーフ承認レポートで「**現在のドキュメントバージョン**」フィルターを使用すると、プルーフの現在のバージョンのみが承認待ちに含められます。

これは、例えば、複数のバージョンを持つプルーフの承認を求められた場合に役に立ちます。「現在のドキュメントのバージョン」フィルターを使用してプルーフ承認レポートを実行すると、そのレポートには、承認を待っている各プルーフの現在のバージョンのみが一覧表示され、作業する必要がなくなった以前のバージョンは除外されます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> 
    <p>新規：</p>
   <ul><li><p>フィルターを変更するコントリビューター </p></li>
   <li><p>レポートを変更する場合は Standard</p></li> </ul>

<p>現在：</p>
   <ul><li><p>フィルターを変更する場合は「要求」 </p></li>
   <li><p>レポートを変更するためのプラン</p></li> </ul></td> 
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

*詳しくは、[Workfront ドキュメントのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

## プルーフ承認レポートをフィルタリングしてプルーフの以前のバージョンを除外

プルーフ承認レポートのフィルターを作成できます。

1. 既にプルーフの承認レポートがある場合は、そのレポートを開きます。

   または

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   独自のプルーフ承認レポートを作成するには、右上隅にある **メインメニュー** アイコン ![](assets/main-menu-icon.png)、または左上隅にある **メインメニュー** アイコン ![](assets/lines-main-menu.png) をクリックし（使用可能な場合）、「**レポート**」 ![](assets/reports-in-main-menu.png) をクリックします。

1. **新しいレポート** をクリックします。 オブジェクトタイプのリストが表示されます。
1. リストの **プルーフの承認** をクリックします。
Report Builder が開きます。
1. 「**フィルター**」、「**フィルタールールを追加**」の順にクリックします。

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. **レポートのフィルタールールを設定** ボックス内をクリックし、リストから **プルーフの承認** を選択します。
1. **プルーフの承認** オブジェクトの下のリストで **現在のドキュメントバージョン** をクリックします。
1. フィルター修飾子として「次と等しい」を選択し、「True」を選択します。
1. Adobe Workfrontの左下にある「**保存して閉じる**」をクリックし、表示されたボックスで **適用** をクリックします。

   プルーフ承認レポートは、プルーフの承認がこのフィルター条件に一致する場合、ドキュメントの現在のバージョンに関連付けられているプルーフのみを表示します。
