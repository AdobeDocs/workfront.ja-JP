---
product-area: portfolios;projects
navigation-topic: portfolio-optimizer
title: ポートフォリオオプティマイザーでのプロジェクトの最適化
description: '[!UICONTROL ポートフォリオオプティマイザー]を使用すると、スコアやその他の値に基づいてプロジェクトに優先順位を付けることができます。オプティマイザーは、コスト、調整、リスク、ROI などの重要なプロジェクト情報を考慮して、ユーザーにとって何がより重要であるかに従ってプロジェクトに優先順位を付けます。'
author: Alina
feature: Work Management, Strategic Planning
exl-id: 25debc5b-5d7d-453f-ab0a-9bf3fba05693
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 85%

---

# [!UICONTROL ポートフォリオオプティマイザー]でプロジェクトを最適化

[!UICONTROL ポートフォリオオプティマイザー]を使用すると、スコアやその他の値に基づいてプロジェクトに優先順位を付けることができます。[!UICONTROL オプティマイザー] は、コスト、調整、リスク、ROI などの重要なプロジェクト情報を考慮して、ユーザーとって何がより重要であるかに従ってプロジェクトに優先順位を付けます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。 

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] package</td> 
   <td> <p>Workfront Prime以降</p>
      <p>ワークフローのPrime以降</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>[!UICONTROL 編集 ] [!UICONTROL ポートフォリオ ] および [!UICONTROL プロジェクト ] へのアクセス</p>  </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ポートフォリオへの権限の [!UICONTROL Manage]</p>  </td> 
  </tr> 
 </tbody> 
</table>

*詳しくは、[Workfrontのアクセス要件ドキュメント ](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md) を参照してください。

+++

<!--Old
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront licenses*</td> 
   <td> <p>New: [!UICONTROL Standard] </p>
   <p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[!UICONTROL Edit] access to Projects and Portfolios</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio</p> <p>Contribute or higher permissions to the projects</p> 
   <p>You must have Manage permissions to all the projects in the list to be able to use <b>Set project priority</b>.</p>
    </td> 
  </tr> 
 </tbody> 
</table>-->

## ポートフォリオオプティマイザーでのプロジェクトの最適化

1. ポートフォリオを開き、左側のパネルで&#x200B;**[!UICONTROL ポートフォリオの最適化]**&#x200B;をクリックします。

   [!UICONTROL ポートフォリオオプティマイザー]が表示されます。

1. **[!UICONTROL 最適化]**&#x200B;アイコンをクリックします。

   ![ 最適化アイコン ](assets/optimize-icon-portfolio-optimizer.png)

   プロジェクトのスコア付けに使用できるカテゴリが、[!UICONTROL 最適化]アイコンの左側に表示されます。

1. スライドする円を使用して、次のいずれかのカテゴリの最適化を変更します。

   * **[!UICONTROL 低コスト]**：スライダーを右に移動すると、[!UICONTROL 予定コスト]が最も低いプロジェクトが表示されます。
   * **[!UICONTROL 整合性の高さ]**：スライダーを右に移動すると、[!UICONTROL スコアカード]に基づいて最も整合性が高いプロジェクトが表示されます。
   * **[!UICONTROL 価値の高さ]**：スライダーを右に移動すると、[!UICONTROL 純値]スコアが高いプロジェクトが表示されます。
   * **[!UICONTROL 利点に対するリスクの低さ]**：スライダーを右に動かすすと、利点に対すいてリスクが最も低いプロジェクトが表示されます。
   * **[!UICONTROL ROI の高さ]**：スライダーを右に移動すると、投資収益率（ROI）が高いプロジェクトが表示されます。

1. **x アイコン** をクリックして、最適化カテゴリを閉じます。

   これにより、**[!UICONTROL スコア]**&#x200B;列の各プロジェクトの[!UICONTROL スコア]値が更新されます。

   [!UICONTROL ポートフォリオオプティマイザー]スコアの詳細については、[[!UICONTROL ポートフォリオオプティマイザー]スコアの概要](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md)を参照してください。

1. **[!UICONTROL スコア]**&#x200B;列に正しい重みを設定したら、**[!UICONTROL スコア]**&#x200B;列のヘッダーをクリックして、この列で並べ替えます。最もスコアの高いプロジェクトがリストの先頭に表示されます。

1. （任意）プロジェクトを優先度順にドラッグ&amp;ドロップします。
これにより、[!UICONTROL ポートフォリオオプティマイザー]内のプロジェクトの順序が変更されます。
1. （オプション）**[!UICONTROL 優先度の設定]**&#x200B;をクリックして、プロジェクトの新しい優先度を保存します。

   >[!NOTE]
   >
   >   **プロジェクトの優先度を設定** を使用するには、リスト内のすべてのプロジェクトに対する管理権限が必要です。

   [!UICONTROL ポートフォリオオプティマイザー]でのプロジェクトの優先順位付けの詳細については、[[!UICONTROL ポートフォリオオプティマイザーでのプロジェクトの優先順位付け]](../../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md)を参照してください。

1. **[!UICONTROL 保存]**&#x200B;をクリックして、[!UICONTROL ポートフォリオオプティマイザー]を保存します。
