---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: スコアカードの作成
description: スコアカードは、プロジェクトがポートフォリオの以前に確立された条件にどの程度適合するかを測定します。 スコアカード管理者は、多くの場合、組織の使命、価値、および戦略目標を反映します。Portfolio管理者は、通常、スコアカードの質問と回答を定義し、プロジェクトの優先順位付けと選択の際に役立ち、価値があることを確認します。 An [!DNL Adobe Workfront] 管理者は、ポートフォリオマネージャーからの推奨に基づいてスコアカードを構築します。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 89c9b450-72a6-4b72-98d1-22956696543a
source-git-commit: 2fd772ffc667c4f32c6a7b0de9c87676ee6dd65b
workflow-type: tm+mt
source-wordcount: '578'
ht-degree: 0%

---

# スコアカードの作成

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.-->

スコアカードは、プロジェクトがポートフォリオの以前に確立された条件にどの程度適合するかを測定します。 スコアカードは、多くの場合、組織の使命、価値、戦略目標を反映しています。

Portfolio管理者は、通常、スコアカードの質問と回答を定義して、プロジェクトの優先順位付けと選択の際に、意味があり価値があるものにする必要があります。 An [!DNL Adobe Workfront] 管理者は、ポートフォリオマネージャーからの推奨に基づいてスコアカードを構築します。

スコアカードに対して選択した質問と回答は、異なるプロジェクトを比較するための整合値を提供するために、定量化可能である必要があります。

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] 計画</td> 
   <td> <p>[!UICONTROL Business] 以降</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] ライセンス</td> 
   <td>[!UICONTROL プラン ]</td> 
  </tr> 
 </tbody> 
</table>

## スコアカードの作成

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL 設定]** ![](assets/gear-icon-settings.png).

1. クリック **[!UICONTROL スコアカード]**&#x200B;を選択し、「 **[!UICONTROL 新しいスコアカード]** 新しいスコアカードを作成し、スコアカードビルダーを起動します。

1. を指定します。 **[!UICONTROL スコアカード名]** および **[!UICONTROL 説明]**.

   スコアカードをプロジェクトに関連付ける際に、名前が表示されます。 説明は、スコアカードリストのスコアカード名の横に表示されます。

1. 次をクリック： **[!UICONTROL 質問を追加]** ドロップダウンメニューを使用して、 [!UICONTROL スコアカードの質問] 「 」セクションで、質問に関する次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL 質問 ]</td> 
      <td>スコアカードに含める質問を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL ポイント ]</td> 
      <td>この質問に対して可能な最大ポイントを入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 負のポイント ]</td> 
      <td>このオプションを選択して、 [!DNL Workfront] は、可能なポイントの合計から減算する必要があります。 スコアカードの最大可能ポイント数に負のスコアを追加することはできません。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL 表示タイプ ]</td> 
      <td>選択 <strong>[!UICONTROL 値 (0-100)]</strong> ユーザーが 0 ～ 100 の任意の値を指定できるスコアカードに数値フィールドを表示する場合。<p>または、 <strong>[!UICONTROL ドロップダウン ]</strong> または <strong>[!UICONTROL ラジオボタン ]</strong> 回答を作成するには、ユーザーはこのコントロールを使用して指定できます。 クリック <strong>[!UICONTROL 回答を追加 ]</strong>を入力し、 <strong>[!UICONTROL 値 ]</strong> 満たされた場合に、この回答に対する割合ポイント。 100%を選択すると、この質問に割り当てられたポイント数が完全に達成されます。 この回答が、この質問に割り当てられたポイントの総数の一部のみを占めることを示す場合は、割合 (%) を低くします。 例えば、質問が 10 ポイントで評価され、この回答に 5 ポイントを含めたい場合、値として 50%を選択します。</p>
      <p>選択 <strong>[!UICONTROL デフォルト ]</strong> この回答がデフォルトの回答であることを示す場合。</strong></p>
     </tr> 
    </tbody> 
   </table>

1. クリック **[!UICONTROL 質問を追加]** スコアカードに質問や回答を追加するには、同じ手順に従います。

   >[!NOTE]
   >
   >スコアカード内の質問を正しい順序でドラッグ&amp;ドロップすることで並べ替えることができます。

1. クリック **[!UICONTROL 保存]** データの入力が終了したら、

## プロジェクトへのスコアカードの適用

を持つユーザー [!UICONTROL 管理] プロジェクトに対する権限は、スコアカードが [!DNL Workfront] 管理者。

プロジェクトのビジネスケースを作成する際に、スコアカードをプロジェクトに追加します。 プロジェクトへのスコアカードの追加の詳細については、「 [プロジェクトにスコアカードを適用し、線形スコアを生成する](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md).

スコアカードの作成の詳細については、 [スコアカードの作成](#create-a-scorecard).

プロジェクト権限の詳細については、 [でプロジェクトを共有 [!DNL Adobe Workfront]](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md).
