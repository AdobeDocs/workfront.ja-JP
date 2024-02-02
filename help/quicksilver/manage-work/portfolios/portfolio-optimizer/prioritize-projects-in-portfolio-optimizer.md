---
title: ポートフォリオオプティマイザーでプロジェクトを最適化する
product-area: portfolios;projects
navigation-topic: portfolio-optimizer
description: ポートフォリオオプティマイザーでは、プロジェクトの完了順序を設定するために優先順位を付けることができます。
author: Alina
feature: Work Management, Strategic Planning
exl-id: 54e33746-5995-49de-8e21-bf973f0694a6
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: ht
source-wordcount: '557'
ht-degree: 100%

---

# [!UICONTROL ポートフォリオオプティマイザー]でのプロジェクトの優先順位付け

[!UICONTROL ポートフォリオオプティマイザー]では、プロジェクトの完了順序を設定するために優先順位を付けることができます。

[!UICONTROL ポートフォリオオプティマイザー]を使用する際には、次の点を考慮してください。

* [!UICONTROL ポートフォリオオプティマイザー]の上部にあるプロジェクトは、下部にあるものよりも重要であるとみなされます。 ポートフォリオを最適化するには、[!UICONTROL ポートフォリオオプティマイザー]での優先順位に従ってプロジェクトを完了する必要があります。
* [!UICONTROL ポートフォリオオプティマイザー]内のプロジェクトの優先度は、プロジェクトの「[!UICONTROL プロジェクトの詳細]」タブにある[!UICONTROL 優先度]フィールドとは無関係です。

  「[!UICONTROL プロジェクトの詳細]」タブの「[!UICONTROL 優先度]」フィールドは、プロジェクトの重要性の理解のために手動で指定する視覚的なフラグです。

* ポートフォリオオプティマイザー内のプロジェクトの優先度は、[!DNL Resource Planner] で有効になっている場合に表示されます。[!DNL Resource Planner] では、プロジェクトは[!UICONTROL ポートフォリオの優先度]ではなく、[!UICONTROL リソースプランナー]の優先度の順序でリソースを受け取ります。

  [!UICONTROL リソースプランナー]でのプロジェクトの優先順位付けについて詳しくは、[[!UICONTROL リソース プランナーでのプロジェクトの優先順位付け]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md)を参照してください。

* [!UICONTROL ポートフォリオオプティマイザー]の&#x200B;**[!UICONTROL プロジェクトの優先順位]**&#x200B;領域には、デフォルトで、[!UICONTROL 開始予定日]、[!UICONTROL 純価]の順にプロジェクトが表示されます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>[!UICONTROL Business] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトおよびポートフォリオへのアクセスの [!UICONTROL Edit]</p> <p>メモ：それでもアクセスできない場合は、アクセスレベルに追加の制限が設定されていないかどうかを [!DNL Workfront] 管理者にお問い合わせください。[!DNL Workfront] 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ポートフォリオへの権限の [!UICONTROL Manage]</p> <p>プロジェクトへの参加権限かそれ以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

## [!UICONTROL ポートフォリオオプティマイザー]内のプロジェクト優先度の変更

1. Adobe Workfront の右上隅にある&#x200B;**[!UICONTROL メインメニュー]**&#x200B;アイコン ![](assets/main-menu-icon.png)をクリックします。

1. 「**[!UICONTROL ポートフォリオ]**」をクリックします。
1. （オプション） **[!UICONTROL フィルター]**&#x200B;ドロップダウンメニューで正しいフィルターを選択すると、ポートフォリオの正しいリストが表示されます。
1. ポートフォリオの名前をクリックして開きます。
1. 左側のパネルで「**[!UICONTROL ポートフォリオの最適化]**」をクリックします。
1. [!UICONTROL プロジェクト最適化]領域で、プロジェクトの優先度を変更するには、優先度の高い順にプロジェクトをドラッグし、目的の表示位置にドロップします。

   ![](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

   プロジェクトの再配置が完了したら、プロジェクトの最適化領域で「**[!UICONTROL 優先度を設定]**」をクリックします。プロジェクトには、新しい順序に基づいて新しい番号が割り振られます。

1. 「**[!UICONTROL 保存]**」をクリックして、[!UICONTROL ポートフォリオオプティマイザー]に新しいプロジェクトの優先度を保存します。優先度は数値 **#** 列に数値として表示されます。

   >[!TIP]
   >
   >プロジェクトのリストは **#** 列以外の列で並べ替えられる可能性があるため、[!UICONTROL ポートフォリオオプティマイザー]でのプロジェクトの順序が必ずしも変更されるわけではありません。**#** 列ヘッダーをクリックして、プロジェクト優先度でリストを並べ替えます。

   リソースプランナーで「**[!UICONTROL ポートフォリオの優先度を表示]**」設定を有効にすると、リソースプランナーで[!UICONTROL ポートフォリオ オプティマイザー]に表示されるプロジェクトの優先度を確認できます。

   [!UICONTROL リソースプランナー] でのプロジェクトの優先順位付けについて詳しくは、[[!UICONTROL リソース プランナーでのプロジェクトの優先順位付け]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md)を参照してください。
