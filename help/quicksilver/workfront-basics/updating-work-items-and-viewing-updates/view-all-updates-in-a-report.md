---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: メモレポートでのすべての更新の表示
description: ユーザーがオブジェクトに入力したすべての更新を表示するには、すべての更新を表示するメモレポートを作成します。
author: Alina
feature: Get Started with Workfront
exl-id: fa5b91e4-b88c-42f0-860c-6864105b4652
source-git-commit: abf5f21281b05dedfecbe71c6ffbf54ee69e2460
workflow-type: tm+mt
source-wordcount: '396'
ht-degree: 31%

---

# メモレポートでのすべての更新の表示

<!-- Audited: 6/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Alina: ***This is a report and it is in the Getting Started/ Updates section because I think it makes more sense to be in this area, where people want to view updates. - added this to this section from Reporting on 7/3/2018 ) </p>
-->

オブジェクトの「更新」領域には、デフォルトで最大 200 個の更新が表示されます。 ユーザーがオブジェクトに入力したすべての更新を表示するには、すべての更新を表示するメモレポートを作成します。

>[!NOTE]
>
>レポートを作成して、ジャーナルエントリレポートを使用してプレビューでオブジェクトの更新を表示できます。詳細については、[ 仕訳レポートを使用した更新領域のレポート ](../../reports-and-dashboards/reports/creating-and-managing-reports/create-journal-entry-report.md) を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>新規：標準 </p>
   <p>現在：プラン</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>次へのアクセスを編集：</p> 
    <ul> 
     <li> <p>レポート、ダッシュボードおよびカレンダーの作成</p> </li> 
     <li> <p>フィルター、ビュー、グループ化を作成</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>表示</p>
    <p>注記：オブジェクトに対する表示以上のパーミッションを持っていない場合、そのオブジェクトの情報はレポートに表示されません。</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## メモレポートの作成

どのオブジェクトのメモに関しても、レポートの作成は、オブジェクトに関係なく同じです。

例えば、プロジェクト上のすべてのメモに関するメモレポートを作成するには、次の手順を実行します。

{{step1-to-reports}}

1. ページの左上隅にある **新規レポート** をクリックし、「**メモ**」を選択します。

1. （任意）「**（列）表示**」をクリックして **「列の追加**」をクリックし、レポートのビューで **プロジェクト** の **名前** を追加します。 

1. （任意）同時に複数のプロジェクトに関するレポートを作成する場合は、**グループ化** をクリックし、**グループ化を追加** をクリックして、**プロジェクト** の **名前** でグループ化します。 これにより、メモが各プロジェクトでグループ化され、レポートが読みやすくなります。 

1. （任意）「**フィルター**」をクリックして、「**フィルタールールを追加**」をクリックします。
1. **メモ**/**メモテキスト**/**空白でない** のフィルターを追加します。

   ![](assets/note-note-text-not-blank-filter.png)

   >[!TIP]
   >
   >   プロジェクトフィールドが更新されても、更新時にメモが追加されなかった場合、更新の **メモテキスト** は **（更新にテキストが追加されていません）** と表示されます。


1. （任意） **プロジェクト**/**名前**/**次と等しい** の別のフィルターを追加し、メモを表示する 1 つまたは複数のプロジェクト名を追加します。
1. **保存して閉じる** をクリックします。 プロジェクトを表示する権限を持つすべてのユーザーがプロジェクトに入力したすべての更新がレポートに表示されます。
