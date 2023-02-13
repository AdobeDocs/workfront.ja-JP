---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: メモレポートですべての更新を表示する
description: メモレポートですべての更新を表示する
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 923c9e25fbd73c9d6a6a20436333c6e7969e9538
workflow-type: tm+mt
source-wordcount: '393'
ht-degree: 0%

---

# メモレポートですべての更新を表示する

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

オブジェクトの「更新」領域には、デフォルトで最大 200 個の更新が表示されます。 任意のユーザーがオブジェクトに対して入力したすべての更新を確認するには、すべての更新を表示する「メモ」レポートを作成します。

>[!NOTE]
>
>レポートを作成して、ジャーナルエントリレポートを使用してプレビューでオブジェクトの更新を表示できます。 詳しくは、 [更新領域に関するレポート](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>計画</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>次へのアクセスを編集：</p> 
    <ul> 
     <li> <p>レポート、ダッシュボードおよびカレンダーの作成</p> </li> 
     <li> <p>フィルター、ビュー、グループの作成</p> </li> 
    </ul> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。<br>Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>ビュー</p> <p>注意：オブジェクトに対する表示権限がない場合、そのオブジェクトの情報はレポートに表示されません。</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## メモレポートの作成

どのオブジェクトのメモに関しても、レポートの作成は同じです。オブジェクトは関係ありません。

たとえば、プロジェクト上のすべてのメモに関するメモレポートを作成するには、次のようにします。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅にある

1. クリック **レポート**.
1. クリック **新しいレポート**&#x200B;を選択して、 **注意**.

1. （オプション）「 **件数**&#x200B;を、 **列を追加** を追加します。 **名前** の **プロジェクト** をクリックします。 

1. （オプション）「 **グループ化**&#x200B;を、 **グループを追加** グループ化する **プロジェクト名**&#x200B;複数のプロジェクトを同時にレポートする場合は、を選択します。\
   これにより、メモが各プロジェクトごとにグループ化され、レポートが読みやすくなります。 

1. （オプション）「 **フィルター、** その後 **フィルタールールを追加** 1 つのプロジェクトまたは特定のプロジェクトをフィルタリングする場合。

1. （条件付きおよびオプション） **プロジェクト名** as **次と等しい** 更新を表示するプロジェクトのプロジェクト名を指定します。  

1. クリック **保存して閉じる**.\
   少なくともプロジェクトの表示権限を持つすべてのユーザーがプロジェクトに入力したすべての更新が、レポートに表示されます。
