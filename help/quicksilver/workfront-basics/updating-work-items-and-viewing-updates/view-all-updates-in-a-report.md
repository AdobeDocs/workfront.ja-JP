---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: メモレポートでのすべての更新の表示
description: メモレポートでのすべての更新の表示
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 923c9e25fbd73c9d6a6a20436333c6e7969e9538
workflow-type: ht
source-wordcount: '393'
ht-degree: 100%

---

# メモレポートでのすべての更新の表示

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

オブジェクトの更新エリアには、デフォルトで最大 200 件の更新が表示されます。任意のユーザーがオブジェクトに対して入力したすべての更新を確認するには、すべての更新を表示するメモレポートを作成します。

>[!NOTE]
>
>レポートを作成して、ジャーナルエントリレポートを使用してプレビューでオブジェクトの更新を表示できます。詳しくは、[更新エリアのレポート](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront ライセンス*</strong></td> 
   <td> <p>プラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>次へのアクセスを編集：</p> 
    <ul> 
     <li> <p>レポート、ダッシュボードおよびカレンダーの作成</p> </li> 
     <li> <p>フィルター、ビュー、グループ化を作成</p> </li> 
    </ul> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。<br>Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>表示</p> <p>メモ：オブジェクトに対する表示権限またはそれ以上の権限を持っていない場合、そのオブジェクトの情報はレポートに表示されません。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a> を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## メモレポートの作成

どのオブジェクトのメモに関しても、レポートの作成は、オブジェクトに関係なく同じです。

例えば、プロジェクト上のすべてのメモに関するメモレポートを作成するには、次の手順を実行します。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックします。

1. 「**レポート**」をクリックします。
1. 「**新規レポート**」をクリックし、「**メモ**」を選択します。

1. （オプション）「**ビュー**」をクリックし、「**列を追加**」をクリックして、レポートのビューに&#x200B;**プロジェクト**&#x200B;の&#x200B;**名前**&#x200B;を追加します。

1. （オプション）複数のプロジェクトを同時にレポートする場合は、「**グループ化**」をクリックし、「**グループ化を追加**」をクリックして、**プロジェクト名**&#x200B;でグループ化します。\
   これにより、メモが各プロジェクトごとにグループ化され、レポートが読みやすくなります。 

1. （オプション）「**フィルター**」、「**フィルタールールを追加**」をクリックして、1 つのプロジェクトのみまたは特定のプロジェクトをフィルタリングします。

1. （条件付きおよびオプション）「**プロジェクト名**」で、更新を表示するプロジェクトのプロジェクト名に対して「**次と等しい**」を設定します。

1. 「**保存して閉じる**」をクリックします。\
   プロジェクトに対して表示以上の権限を持つすべてのユーザーがプロジェクトに入力したすべての更新が、レポートに表示されます。
