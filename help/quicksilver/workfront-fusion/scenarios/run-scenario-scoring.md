---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Adobe Workfront Fusion でシナリオスコアリングエキスパートを実行します
description: シナリオスコアリングエキスパートは、ベストプラクティスに従ってシナリオが確実に設定されるようにするのに役立ちます。 シナリオをチェックし、構造と組織に関する推奨事項を提供します。
author: Becky
feature: Workfront Fusion
exl-id: 144c8dbd-a3e9-4267-b3db-0768dac8f384
source-git-commit: 2b455fb2d3892c6bb796aa7ea57a60c861c3d599
workflow-type: tm+mt
source-wordcount: '327'
ht-degree: 22%

---

# Adobe Workfront Fusion でシナリオスコアリングエキスパートを実行します

シナリオスコアリングエキスパートは、ベストプラクティスに従ってシナリオが確実に設定されるようにするのに役立ちます。 シナリオをチェックし、構造と組織に関する推奨事項を提供します。

## アクセス要件

この記事で説明している機能を使用するには、次のアクセス権が必要です。

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] プラン*</td> 
   <td> <p>[!DNL Pro] またはそれ以降</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス*</td> 
   <td> <p>[!UICONTROL Plan]、[!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] ライセンス**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration] </p><p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>この記事で説明されている機能を使用するには、組織で [!DNL Adobe Workfront Fusion] と [!DNL Adobe Workfront] を購入する必要があります。</td> 
  </tr> 
 </tbody> 
</table>

ご利用のプラン、ライセンスタイプまたはアクセス権を確認するには、[!DNL Workfront] 管理者にお問い合わせください。

[!DNL Adobe Workfront Fusion] ライセンスについて詳しくは、[[!DNL Adobe Workfront Fusion] ライセンス](../../workfront-fusion/get-started/license-automation-vs-integration.md)を参照してください。

シナリオスコアリングエキスパートの実行

1. 左側のパネルで「**[!UICONTROL シナリオ]**」タブをクリックします。
1. シナリオ・スコアリング・エキスパートを実行するシナリオを選択します。
1. シナリオの任意の場所をクリックして、シナリオエディターに移動します。
1. 画面の下部付近にあるシナリオスコアリングエキスパートアイコン ![ シナリオスコアリングエキスパート ](assets/scoring-expert-icon.png) をクリックします。

   シナリオスコアリングエキスパートパネルが開きます。
1. **評価** をクリックします。

シナリオスコアリングエキスパートは、10 点中のスコアを返し、どのチェックに合格または失敗したかを示します。 チェックが失敗した場合、シナリオのスコアリング・エキスパートは、シナリオがこれらのチェックを確実に満たす方法の推奨事項を提供します。

![ シナリオスコア ](assets/scenario-score.png)

## シナリオスコアリングチェック

シナリオスコアリングエキスパートでは、次のチェックを使用します。

* シナリオに名前を付ける必要があります。
* すべてのモジュールにラベルを付ける必要があります。
* シナリオは、設定されたスケジュールで実行する必要があります。

  手順については、[ シナリオのスケジュール設定 ](/help/quicksilver/workfront-fusion/scenarios/schedule-a-scenario.md) を参照してください。
* シナリオのブループリントのサイズは 5 MB 未満にする必要があります。

  詳しくは、[Fusion パフォーマンスガードレール ](/help/quicksilver/workfront-fusion/get-started/fusion-performance-guardrails.md#scenarios) を参照してください。
* Workfront インスタントトリガーモジュールを使用する場合は、フィルタリングする必要があります。

  手順については、[ イベントを監視  [!DNL Workfront]  モジュールの [!UICONTROL  イベント購読フィルター ] を参照してください ](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#event-subscription-filters-in-the-workfront--watch-events-module)。

