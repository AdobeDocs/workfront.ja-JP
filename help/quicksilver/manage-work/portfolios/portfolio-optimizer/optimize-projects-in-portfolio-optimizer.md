---
product-area: portfolios;projects
navigation-topic: portfolio-optimizer
title: ポートフォリオオプティマイザーでのプロジェクトの最適化
description: '[!UICONTROL ポートフォリオオプティマイザー]を使用すると、スコアやその他の値に基づいてプロジェクトに優先順位を付けることができます。オプティマイザーは、コスト、調整、リスク、ROI などの重要なプロジェクト情報を考慮して、ユーザーにとって何がより重要であるかに従ってプロジェクトに優先順位を付けます。'
author: Alina
feature: Work Management, Strategic Planning
exl-id: 25debc5b-5d7d-453f-ab0a-9bf3fba05693
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: ht
source-wordcount: '490'
ht-degree: 100%

---

# [!UICONTROL ポートフォリオオプティマイザー]でプロジェクトを最適化

[!UICONTROL ポートフォリオオプティマイザー]を使用すると、スコアやその他の値に基づいてプロジェクトに優先順位を付けることができます。[!UICONTROL オプティマイザー] は、コスト、調整、リスク、ROI などの重要なプロジェクト情報を考慮して、ユーザーとって何がより重要であるかに従ってプロジェクトに優先順位を付けます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!UICONTROL Business] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>[!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトおよびポートフォリオへのアクセスの [!UICONTROL Edit]</p> <p>メモ：まだアクセス権がない場合は、[!DNL Workfront] 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ポートフォリオへの権限の [!UICONTROL Manage]</p> <p>プロジェクトへの参加権限かそれ以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## ポートフォリオオプティマイザーでのプロジェクトの最適化

1. ポートフォリオを開き、左側のパネルで&#x200B;**[!UICONTROL ポートフォリオの最適化]**&#x200B;をクリックします。

   [!UICONTROL ポートフォリオオプティマイザー]が表示されます。

1. **[!UICONTROL 最適化]**&#x200B;アイコンをクリックします。

   ![](assets/optimize-icon-portfolio-optimizer.png)\
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

1. （オプション）優先度に従ってプロジェクトをドラッグ＆ドロップします。\
   これにより、[!UICONTROL ポートフォリオオプティマイザー]内のプロジェクトの順序が変更されます。
1. （オプション）**[!UICONTROL 優先度の設定]**&#x200B;をクリックして、プロジェクトの新しい優先度を保存します。\
   [!UICONTROL ポートフォリオオプティマイザー]でのプロジェクトの優先順位付けの詳細については、[[!UICONTROL ポートフォリオオプティマイザーでのプロジェクトの優先順位付け]](../../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md)を参照してください。

1. **[!UICONTROL 保存]**&#x200B;をクリックして、[!UICONTROL ポートフォリオオプティマイザー]を保存します。
