---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: 「フィルター：プルーフの以前のバージョンを省略するプルーフの承認レポート」
description: プルーフの承認レポートでは、「現在のドキュメントのバージョン」フィルターを使用して、承認待ちのプルーフの現在のバージョンのみを含めることができるようになりました。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 661f925b4e485069122ef4278b2914d206387974
workflow-type: ht
source-wordcount: '356'
ht-degree: 100%

---

# フィルター：プルーフの以前のバージョンを省略するプルーフの承認レポート

プルーフ承認レポートでは、**現在のドキュメントバージョン**&#x200B;フィルターを使用して、承認待ちのプルーフの現在のバージョンだけを含めることができます。

これは、例えば、複数のバージョンを持つプルーフの承認を求められた場合に役に立ちます。「現在のドキュメントのバージョン」フィルターを使用してプルーフ承認レポートを実行すると、そのレポートには、承認を待っている各プルーフの現在のバージョンのみが一覧表示され、作業する必要がなくなった以前のバージョンは除外されます。 

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
   <td> <p>フィルターを変更する場合は「要求」 </p>
   <p>レポートを変更するためのプラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセス権を編集して、レポートを変更できるようにします。</p> <p>フィルターを変更する場合は、フィルター、ビュー、グループ化への編集アクセス権</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## プルーフ承認レポートをフィルタリングしてプルーフの以前のバージョンを除外

1. 既にプルーフの承認レポートがある場合は、そのレポートを開きます。

   または

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   独自のプルーフの承認レポートを作成するには、メインメニュー![](assets/main-menu-icon.png)を選択し、次に「**レポート**」![](assets/reports-in-main-menu.png)をクリックします。「**新しいレポート**」をクリックします。表示されたリストで、**プルーフの承認**&#x200B;までスクロールし、クリックします。「**保存して閉じる**」をクリックし、「**レポート名**（オプション）」入力して、「**レポートを保存**」をクリックします。

1. **レポートアクション／編集**&#x200B;をクリックします。
1. 「**フィルター**」、「**フィルタールールを追加**」の順にクリックします。

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. 「**プルーフの承認**」をクリックします。
1. 表示されるリストで、**現在のドキュメントのバージョン**&#x200B;をクリックします。
1. 「**保存して閉じる**」をクリックし、Adobe Workfront の左下隅で、表示されたボックス内で「**レポートを保存**」をクリックします。
