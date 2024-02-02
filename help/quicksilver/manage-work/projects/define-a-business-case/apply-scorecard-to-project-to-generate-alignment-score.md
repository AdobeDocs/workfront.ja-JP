---
navigation-topic: business-case-and-scorecards
title: プロジェクトにスコアカードを適用し、整合性スコアを生成
description: スコアカードを使用して、プロジェクトが以前に確立されたポートフォリオの条件にどの程度適合しているかを測定できます。スコアカードは、多くの場合、組織の使命、価値、戦略的目標を反映しています。
author: Alina
feature: Work Management
exl-id: 21cf5493-147d-4b8d-8b16-2891eb7e0491
source-git-commit: 78878fa3578e4f3a33baec3806298282d3909d8d
workflow-type: ht
source-wordcount: '1292'
ht-degree: 100%

---

# プロジェクトにスコアカードを適用し、整合性スコアを生成

スコアカードを使用して、プロジェクトが以前に確立されたポートフォリオの条件にどの程度適合しているかを測定できます。スコアカードは、多くの場合、組織の使命、価値、戦略的目標を反映しています。

スコアカードとその作成方法について詳しくは、[スコアカードを作成](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>ビジネス以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> <p>ポートフォリオに対する表示またはそれ以上のアクセス権</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対して権限を管理</p> <p>ポートフォリオに対する表示またはそれ以上の権限 </p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## プロジェクトのスコアカード {#project-scorecards}

* [スコアカードの概要](#scorecards-overview)
* [プロジェクトのスコアカード](#project-scorecards)

### スコアカードの概要 {#scorecards-overview}

通常、プロジェクトマネージャーがスコアカード情報をすべて入力し、プロジェクトの整合性の値を 0～100 で生成します。この生成された値は、後でポートフォリオマネージャーがポートフォリオオプティマイザー内のプロジェクトをレビューして比較する際に使用されます。

ポートフォリオ最適化について詳しくは、[ポートフォリオオプティマイザーの概要](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)を参照してください。

### プロジェクトへのスコアカードの適用

プランライセンスを持ち、プロジェクトに対する管理権限を持つユーザーは、プロジェクトにスコアカードを添付できます。

プロジェクト権限について詳しくは、[Adobe Workfront でプロジェクトを共有](../../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md)を参照してください。

プロジェクトのビジネスケースを作成する一環として、プロジェクトにスコアカードを追加できます。

ビジネスケースの作成について詳しくは、[プロジェクトのビジネスケースを作成](../../../manage-work/projects/define-a-business-case/create-business-case.md)を参照してください。

ビジネスケースからスコアカードにアクセスするには、Adobe Workfront 管理者またはグループ管理者が、プロジェクトのビジネスケースエリアの「スコアカード」セクションを有効にする必要があります。プロジェクトの環境設定とビジネスケースのエリアの有効化について詳しくは、[システム全体のプロジェクト環境を設定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

プロジェクトにスコアカードを適用する手順は、次のとおりです。

1. スコアカードを適用するプロジェクトに移動します。
1. 左パネルの「**ビジネスケース**」をクリックします。
1. ビジネスケースの「**スコアカード**」セクションを探します。\
   ビジネスケースに「**スコアカード**」セクションを表示するには、スコアカードを作成する必要があります。

   スコアカードの作成について詳しくは、[スコアカードを作成](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md)を参照してください。

1. ドロップダウンメニューから「スコアカード」を選択します。

   ![new_scorecard.png](assets/new-scorecard-350x149.png)

1. スコアカード内のすべての質問に対する回答を指定します。

   Workfront は、回答した各質問にスコアを適用し、全質問の個々のスコアに基づいてプロジェクト全体のスコアを計算します。

   プロジェクト全体の整合性スコアの生成について詳しくは、[プロジェクトの整合性スコアを生成](#generate-an-alignment-score-for-a-project)を参照してください。

1. 「**保存**」をクリックして、スコアカードを保存し、プロジェクトにスコアを付けます。

   スコアカードがプロジェクトに関連付けられ、プロジェクトにスコアが付きます。

<!--This functionality was removed when we redesigned bulk editing projects with 23.2: 

1. (Conditional) When changes occur in the values of scorecard questions, you must recalculate the scorecard to reflect the new values for the project score. To recaulate the scorecard, do the following: 

   1. Go to a list of projects and select all projects in the list. 
   1. Click the **Edit** icon at the top of the list. 
   1. Click **Settings** in the left panel, then check the **Recalculate Scorecards** option at the end of the Settings area. 
   1. Click Save. This recalculates the score value based on the scorecards attached for all the selected projects.  

      >[!NOTE]
      >
      >   The option to recalculate scorecards has been removed from the Preview environment, when editing projects in bulk. 

-->

## 整合性スコアを生成

* [プロジェクトの整合性スコアを生成](#generate-an-alignment-score-for-a-project)
* [ポートフォリオの整合性スコアを生成](#generate-an-alignment-score-for-a-portfolio)

### プロジェクトの整合性スコアを生成 {#generate-an-alignment-score-for-a-project}

整合性スコアは、スコアカードの入力後に生成される値です。

スコアカードには質問と回答の選択肢が含まれており、回答には整合性ポイントと呼ばれる数値が割り当てられています。これらのポイントは、プロジェクトが組織とどの程度整合しているかを決定するために使用されます。各質問の整合性ポイントには、0 ～ 100 の数値が含まれています。

スコアカードが完成すると、Workfront は、プロジェクトの整合性スコアをパーセンテージで計算します。計算には次の式を使用します。

```
Project Alignment Score = The sum of the question points from the scorecard met at a given time/ The sum of the possible points on the scorecard
```

詳しくは、[スコアカードの作成](../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md)を参照してください。

### ポートフォリオの整合性スコアを生成 {#generate-an-alignment-score-for-a-portfolio}

ポートフォリオの整合性スコアは、ポートフォリオ内のすべてのプロジェクトの整合性スコアの平均です。

各プロジェクトのスコアカードが完了すると、Workfront はそれらの値を使用して、ポートフォリオの整合性スコアをパーセンテージで計算します。計算には次の式を使用します。

ポートフォリオの整合性スコア = プロジェクトの整合性スコアのパーセンテージの合計／ポートフォリオ内のプロジェクトの数

>[!NOTE]
>
>プロジェクトにスコアカードが関連付けられておらず、そのため整合性スコアが存在しない場合は、ポートフォリオ内で整合性が 0％ と見なされます。このプロジェクトは、ポートフォリオ内のプロジェクトの数にカウントされます。

## 整合性スコアを確認

プロジェクトの整合性スコアは、プロジェクトレベルで、またはポートフォリオオプティマイザーで確認できます。

* [プロジェクトで整合性スコアを確認](#View%20the)
* [ポートフォリオオプティマイザーでプロジェクトやポートフォリオの整合性スコアを確認](#View%20the2)

### プロジェクトの整合性スコアを確認

プロジェクトに対する参加権限を持っている場合は、プロジェクトレベルでプロジェクトの整合性スコアを確認できます。

1. 整合性スコアを確認するプロジェクトに移動します。
1. 左側のパネルの「**ビジネスケース**」をクリックします。
1. 画面右側の&#x200B;**ビジネスケース概要**&#x200B;に移動します。

   整合性スコアは、ビジネスケース概要の「**整合済み**」の値にあります。

   ![alignment_score_on_a_project.png](assets/alignment-score-on-a-project.png)

### ポートフォリオオプティマイザーでプロジェクトやポートフォリオの整合性スコアを確認

ポートフォリオに対する管理権限を持っている場合は、プロジェクトやポートフォリオの整合性スコアをポートフォリオオプティマイザーで確認できます。

ポートフォリオオプティマイザーに表示される情報について詳しくは、[ポートフォリオオプティマイザーの概要](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-overview.md)を参照してください。

* [ポートフォリオオプティマイザーでプロジェクトの整合性スコアを見つける](#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer)
* [ポートフォリオオプティマイザーでポートフォリオの整合性スコアを見つける](#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer)

  ![](assets/alignment-score-in-portfolio-optimizer-nwe-350x97.png)

#### ポートフォリオオプティマイザーでプロジェクトの整合性スコアを見つける {#locate-the-alignment-score-of-the-project-in-the-portfolio-optimizer}

1. **メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックし、「**ポートフォリオ**」をクリックします。

1. ポートフォリオの名前をクリックします。
1. 左側のパネルで「**ポートフォリオ最適化**」をクリックします。

   ポートフォリオオプティマイザーが表示されます。

1. プロジェクトの整合性スコアは、ポートフォリオオプティマイザーの「**整合性**」に、パーセンテージで表示されます。

   これは、プロジェクトに関連付けられたスコアカードに基づくプロジェクトの整合性スコアです。

#### ポートフォリオオプティマイザーでポートフォリオの整合性スコアを見つける  {#locate-the-alignment-score-of-the-portfolio-in-the-portfolio-optimizer}

1. グローバルナビゲーションバーで「**プロジェクト**」エリアに移動します。
1. 「**ポートフォリオ**」タブを選択します。
1. ポートフォリオの名前をクリックします。
1. 「**ポートフォリオ最適化**」タブを選択します。
1. ポートフォリオオプティマイザーの上部で、ポートフォリオの整合性スコアを示す「**整合済み**」の値や「**整合性**」ゲージを探します。

   これは、ポートフォリオの整合性スコアです。

   ポートフォリオの整合性スコアの生成方法について詳しくは、[ポートフォリオの整合性スコアを生成](#generate-an-alignment-score-for-a-portfolio)を参照してください。

## ポートフォリオオプティマイザーのスコアの概要

プロジェクトの整合性スコアとポートフォリオオプティマイザーのスコアには違いがあります。

プロジェクトの整合性スコアは、スコアカードの完了後に取得したポイントに基づいて計算されます。このスコアは、ポートフォリオ整合性スコアの決定に使用されます。整合性スコアは、割合で表示されます。

プロジェクトの整合性スコアは、ポートフォリオオプティマイザーの&#x200B;**整合性**&#x200B;列に表示されます。

ポートフォリオオプティマイザーのスコアは、ポートフォリオオプティマイザーで自動的に計算され、プロジェクトの優先順位付けに使用できるランキングです。ポートフォリオオプティマイザーのスコアは、数字が付いたインジケーターアイコンとして表示され、ポートフォリオオプティマイザーの&#x200B;**スコア**&#x200B;列に表示されます。ポートフォリオオプティマイザーのスコアは、目標を除きビジネスケースのすべてのセクションが入力されている場合にのみ生成されます。

プロジェクトのビジネスケースの作成について詳しくは、[プロジェクトのビジネスケースを作成](../../../manage-work/projects/define-a-business-case/create-business-case.md)を参照してください。

プロジェクトのポートフォリオオプティマイザースコアの計算について詳しくは、[ポートフォリオオプティマイザーのスコアの概要](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md)を参照してください。
