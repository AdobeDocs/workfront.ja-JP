---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: フィルター：以前の校正バージョンを省略する校正承認レポート
description: プルーフの承認レポートでは、「現在のドキュメントのバージョン」フィルターを使用して、承認待ちのプルーフの現在のバージョンのみを含めることができるようになりました。
author: Courtney
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 6a6d3d47ed5741e3202c44b7240a2e67b687ea95
workflow-type: tm+mt
source-wordcount: '379'
ht-degree: 48%

---

# フィルター：プルーフの以前のバージョンを省略するプルーフの承認レポート

<!--Audited: 10/2024-->

校正承認レポートで、**現在のドキュメントバージョン**&#x200B;フィルターを使用して、承認待ちの校正の現在のバージョンのみを含めることができます。

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
   <p>フィルターの変更をコントリビューターまたはリクエスト </p>
   <p>レポートを変更するための「標準」または「プラン」</p>
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

校正承認レポートのフィルターを作成できます。

1. 既にプルーフの承認レポートがある場合は、そのレポートを開きます。

   または

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   独自の校正承認レポートを作成するには、右上隅の&#x200B;**メインメニュー**&#x200B;アイコン![メインメニューアイコン](assets/main-menu-icon.png)をクリックするか、左上隅の&#x200B;**メインメニュー**&#x200B;アイコン![メインメニュー行](assets/lines-main-menu.png)をクリックします（使用可能な場合）。**レポート** ![レポートアイコン](assets/reports-in-main-menu.png)をクリックします。

1. **新しいレポート**&#x200B;をクリックします。 オブジェクトタイプのリストが表示されます。
1. 一覧の[**承認の証明**]をクリックします。
レポートビルダーが開きます。
1. 「**フィルター**」、「**フィルタールールを追加**」の順にクリックします。

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. **レポートのフィルタールールを設定**&#x200B;ボックス内をクリックし、一覧から&#x200B;**承認の証明**&#x200B;を選択します。
1. **Proof Approval**&#x200B;オブジェクトの下のリストで、**現在のドキュメントバージョン**&#x200B;をクリックします。
1. フィルタモディファイヤで[等しい]を選択し、[はい]を選択します。
1. Adobe Workfrontの左下隅にある&#x200B;**保存+閉じる**&#x200B;をクリックし、表示されるボックスで「**適用**」をクリックします。

   校正承認レポートでは、校正承認がこのフィルタリング基準と一致する場合、文書の現在のバージョンに関連付けられた校正のみが表示されます。
