---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: メモレポートでのすべての更新の表示
description: メモレポートでのすべての更新の表示
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: 36bdacb5f6d04245552aeeb4ab82d210597645a2
workflow-type: tm+mt
source-wordcount: '372'
ht-degree: 61%

---

# メモレポートでのすべての更新の表示

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

オブジェクトの「更新」領域には、デフォルトで最大 200 個の更新が表示されます。 ユーザーがオブジェクトに入力したすべての更新を表示するには、すべての更新を表示するメモレポートを作成します。

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
   <td role="rowheader"><strong>Adobe Workfront プラン</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン*</strong></td> 
   <td> <p>新規：標準 </p>
   <p>現在：プラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>次へのアクセスを編集：</p> 
    <ul> 
     <li> <p>レポート、ダッシュボードおよびカレンダーの作成</p> </li> 
     <li> <p>フィルター、ビュー、グループ化を作成</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>表示</p> <p><b>メモ</b></p>
   <p>オブジェクトに対する表示以上の権限を持っていない場合、そのオブジェクトの情報はレポートに表示されません。</p>  </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Adobe Workfrontのアクセス要件 ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

## メモレポートの作成

どのオブジェクトのメモに関しても、レポートの作成は、オブジェクトに関係なく同じです。

例えば、プロジェクト上のすべてのメモに関するメモレポートを作成するには、次の手順を実行します。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックします。

1. 「**レポート**」をクリックします。
1. 「**新規レポート**」をクリックし、「**メモ**」を選択します。

1. （オプション）「**ビュー**」をクリックし、「**列を追加**」をクリックして、レポートのビューに&#x200B;**プロジェクト**&#x200B;の&#x200B;**名前**&#x200B;を追加します。

1. （オプション）複数のプロジェクトを同時にレポートする場合は、「**グループ化**」をクリックし、「**グループ化を追加**」をクリックして、**プロジェクト名**&#x200B;でグループ化します。\
   これにより、メモが各プロジェクトごとにグループ化され、レポートが読みやすくなります。 

1. （任意）「**フィルター**」をクリックして、「**フィルタールールを追加**」をクリックします。
1. **メモ**/**メモテキスト**/**空白でない** のフィルターを追加します。

   ![](assets/note-note-text-not-blank-filter.png)

   >[!TIP]
   >
   >   プロジェクトフィールドが更新されても、更新時にメモが追加されなかった場合、更新の **メモテキスト** は **（更新にテキストが追加されていません）** と表示されます。


1. （任意） **プロジェクト**/**名前**/**次と等しい** の別のフィルターを追加し、メモを表示する 1 つまたは複数のプロジェクト名を追加します。
1. 「**保存して閉じる**」をクリックします。\
   プロジェクトに対して表示以上の権限を持つすべてのユーザーがプロジェクトに入力したすべての更新が、レポートに表示されます。
