---
content-type: tips-tricks-troubleshooting
product-area: reporting;user-management
navigation-topic: tips-tricks-and-troubleshooting-reports
title: '''フィルター：以前の配達確認バージョンを省略する配達確認の承認レポート'
description: 配達確認の承認レポートでは、「現在のドキュメントのバージョンです」フィルターを使用して、承認を待機している配達確認の現在のバージョンのみを含めることができます。
author: Lisa and Nolan
feature: Reports and Dashboards
exl-id: e844d3ed-75ee-4a0f-a28c-a3d22f203502
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '339'
ht-degree: 0%

---

# フィルター：配達確認の以前のバージョンを省略する配達確認の承認レポート

配達確認の承認レポートでは、 **現在のドキュメントのバージョン** フィルターを使用して、承認待ちの配達確認の現在のバージョンのみを含めます。

これは、例えば、複数のバージョンを持つ配達確認を承認するように求められた場合に便利です。 「現在のドキュメントのバージョン」フィルターを使用して配達確認の承認レポートを実行すると、レポートには各配達確認の現在のバージョンのみがリスト表示され、以前のバージョンでは作業する必要がなくなります。 

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集</p> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 配達確認の承認レポートをフィルターして、以前の配達確認バージョンを省略します

1. 既に配達確認の承認レポートがある場合は、それを開きます。

   または

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Sarah: Add sub bullets for report creation.</p>
   -->

   独自の配達確認の承認レポートを作成するには、メインメニュー ![](assets/main-menu-icon.png)を選択し、「 **レポート** ![](assets/reports-in-main-menu.png). クリック **新しいレポート**. 表示されるリストで、スクロールしてをクリックします。 **配達確認の承認**. クリック **保存して閉じる**, type **レポート名** （オプション）」を選択し、「 **レポートを保存**.

1. クリック **レポートアクション/編集**.
1. クリック **フィルター**&#x200B;を選択し、「 **フィルタールールを追加**.

   <!--
   <p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">Tell Proof Lehi this isn't visible unless you scroll to it over on the right, not at all obvious. When on a laptop.</p>
   -->

1. クリック **配達確認の承認**.
1. 表示されるリストで、 **現在のドキュメントのバージョン**.
1. クリック **保存して閉じる** Adobe Workfrontの左下隅で、 **レポートを保存** をクリックします。
