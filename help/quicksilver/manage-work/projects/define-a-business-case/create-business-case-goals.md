---
navigation-topic: business-case-and-scorecards
title: ビジネスケースの目標を作成
description: ビジネスケースの作成の一環として、一連の目標を作成し、プロジェクトの目標を定義できます。ビジネスケースの目的は、プロジェクトを完了する目的をポートフォリオマネージャーまたはプロジェクトスポンサーに伝えるために使用されます。
author: Alina
feature: Work Management
exl-id: c5f4c095-ea21-4205-a747-e8923de7030f
source-git-commit: b38c98ec79617a78c76510bcb109da2ff83247af
workflow-type: tm+mt
source-wordcount: '504'
ht-degree: 59%

---

# ビジネスケースの目標を作成

<!-- Audited: 4/2025 -->

ビジネスケースの作成の一環として、一連の目標を作成し、プロジェクトの目標を定義できます。これらの目標は、プロジェクトを完了する目的をPortfolioマネージャーまたはプロジェクトスポンサーに伝えるために使用されます。

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: below snippet: NWE only, not classic)</p>
-->

>[!TIP]
>
>プロジェクトの個々のビジネスケースに関連していない組織の戦略目標を作成できます。戦略的目標を作成するには、Adobe Workfront Goals へのアクセス権が必要です。 その後、ビジネスケース外のプロジェクトに接続できます。Workfront Goals を使用した目標の作成について詳しくは、[Adobe Workfront Goals の概要](../../../workfront-goals/goal-management/wf-goals-overview.md)を参照してください。

プロジェクトのビジネスケース目標を作成する際は、次の点を考慮してください。

* ビジネスケースの目標は、プロジェクト固有です。あるプロジェクトから別のプロジェクトに目標をコピーしたり、システムレベルで目標を設定したりすることはできません。これらの目標は、各プロジェクトのレベルで定義する必要があります。
* Adobe Workfront管理者またはグループ管理者は、プロジェクトの「目標」セクションがビジネスケースに表示される前に、そのセクションを有効にする必要があります。 プロジェクトに対してビジネスケースフィールドを有効にする方法につては、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

* 目標は、プロジェクトのビジネスケースの必須セクションではありません。

  プロジェクトは、Portfolio Optimizer で優先順位付けされるスコアを受け取ることができます（目標セクションが定義されていない場合でも）。

  ポートフォリオオプティマイザーのスコアについて詳しくは、[プロジェクトにスコアカードを適用し、整合性スコアを生成](../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md)を参照してください。

* ビジネスケースの目標をレポートすることはできません。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>Pro 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td>
   <td> 
   <p>新規：標準</p> 
   <p>または</p>
   <p>現在：プラン </p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する管理以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## プロジェクトのビジネスケースに目標を追加する

{{step1-to-projects}}

1. プロジェクトリストで、ビジネスケースの目標を定義するプロジェクトを選択します。
1. 左側のパネルで、「ビジネスケース **をクリック** ます。 **ビジネスケース** セクションが表示されます。

   ![ ビジネスケース情報 ](assets/business-case-page-info-goals-expenses-nwe-350x123.png)

1. 「**目標**」セクションで「**目標を編集**」をクリックします。

1. 最初のフィールドに目標の説明を入力します。

1. **重要度** ドロップダウンメニューで、この目標の重要度（優先度）を選択します。

   * 最高
   * 高
   * 中
   * 低
   * 最低

     ![ 重要度 ](assets/g1-350x76.png)

     >[!NOTE]
     >
     >目標の重要度レベルをカスタマイズすることはできません。

1. （任意）別の目標を追加するには、「**別の目標を追加** をクリックし、手順 5～6 を繰り返します。

1. **保存**&#x200B;をクリックします。
