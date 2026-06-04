---
product-area: projects;agile-and-teams
navigation-topic: manage-projects
title: ボードビューでのアジャイルプロジェクトの管理
description: アジャイル手法に伴う管理上の課題（チームのバックログの管理やイテレーションの作成など）に悩まされることなく、プロジェクトにアジャイル機能を活用することができます。
author: Alina, Courtney
feature: Work Management
exl-id: fc633fd6-35b4-4949-8045-22c775002436
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: https://experienceleague.adobe.com/Pw5yN5HjeNXviuTZS0L0Q5iM66zQl8ffX3-SeJ-eMno
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: be65ef36-43e4-48e1-a062-caa3778e15be
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 314
ht-degree: 44%

---

# ボードビューでのアジャイルプロジェクトの管理

<!-- Audited: 11/2025 -->

アジャイル手法に伴う管理上の課題（チームのバックログの管理やイテレーションの作成など）に悩まされることなく、プロジェクトにアジャイル機能を活用することができます。

チームのバックログを使用し、バックログ上のタスクからイテレーションを作成できるアジャイル環境で作業できます。

詳しくは、[&#x200B; アジャイル環境での作業](../../../agile/work-in-an-agile-environment/work-in-an-agile-environment.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

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
   <td> <p>明るいまたはそれ以上</p>
   <p>レビュー以上</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>次のエリアへの編集アクセス権：</p> 
    <ul> 
     <li> <p>プロジェクト</p> </li> 
     <li> <p>レポート、ダッシュボード、カレンダー</p> </li> 
     <li> <p>フィルター、ビュー、グループ化</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトの表示権限</p>  </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--
old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license</td> 
   <td> <p>Current: Review or higher</p> 
   <p>New: Contributor or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configuration</td> 
   <td> <p>Edit access to the following areas:</p> 
    <ul> 
     <li> <p>Projects</p> </li> 
     <li> <p>Reports, Dashboards, Calendars</p> </li> 
     <li> <p>Filters, Views, Groupings</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View permissions to the project</p>  </td> 
  </tr> 
 </tbody> 
</table>
-->


## ボードビューでのプロジェクトの表示

アジャイル機能をプロジェクト開発に活用するには、リストではなくボードビューでプロジェクトのタスクとイシューの両方を表示できます。

1. アジャイル手法に従って管理するプロジェクトに移動し、左側のパネルで「**タスク**」または「**問題**」をクリックします。
1. **ボードビュー**&#x200B;アイコン ![ボードアイコン](assets/board-icon-for-agile-view.png) をクリックします。

   プロジェクトのボードビューがデフォルトで表示されます。

   ![プロジェクトのボードビュー](assets/project-agile-board-view.png)


1. （オプション）「**設定**」をクリックして、列とカードのオプションを設定します。

   詳しくは、[ボード列の管理](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md)と[カードに表示されるフィールドのカスタマイズ](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md)を参照してください。 プロジェクトのボードビューでは列ポリシーを定義できないことに注意してください。

1. （オプション）リスト表示に戻るには、**リスト** アイコン ![&#x200B; リストアイコン &#x200B;](assets/list-icon.png)をクリックします。

   タスクまたは問題のリストが表示されます。
