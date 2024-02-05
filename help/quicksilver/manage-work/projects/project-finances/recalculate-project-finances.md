---
title: プロジェクトの財務を再計算
product-area: projects
navigation-topic: financials
description: 財務は、プロジェクトで記録された時間数や、コストと収益の計算に使用される料金に変化が生じると、財務がプロジェクトに基づいて計算されます。
author: Alina
feature: Work Management
exl-id: 5a90c5a1-8b26-4b6f-b9ec-f446a2e94ff0
source-git-commit: bfe77796863bb2d7d324901721fda7fa045c2c0b
workflow-type: tm+mt
source-wordcount: '1620'
ht-degree: 92%

---

# プロジェクトの財務を再計算

財務は、プロジェクトで記録された時間数や、コストと収益の計算に使用される料金に変化が生じると、財務がプロジェクトに基づいて計算されます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトおよび財務データへのアクセスを編集する</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>財務を管理する権限を持つプロジェクトに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## Adobe Workfront での財務計算に関する検討事項

強化機能分析では、以下の方法で財務を計算します。

* プロジェクトの「財務の再計算」オプションを使用すると、プロジェクトのコストと収益を手動で再計算できます。
* また、一部のアクションは自動再計算をトリガーにしています。

プロジェクトの期間中にユーザーまたは役割の料金が変更されると、以下のことが起こる場合があります。

* 変更が行われると、時間数が記録され、財務情報が計算されると、更新された料金がその時点から使用されます。料金を変更しても、変更前の計算方法には影響しません。ログに記録されたすべての既存の時間数に対して、古い料金が財務情報の計算に使用されます。
* 「財務の再計算」オプションを使用すると、Adobe Workfront に対して、これまでに記録されたすべての時間数に遡って新しいレートを強制的に使用させることができます。これにより、Workfront は、以前に入力した時間数、予定コスト、売上高をすべて新しい料金情報に従って遡及的に再計算します。

>[!CAUTION]
>
>特定のプロジェクトの財務を手動で再計算する前に、以前の料金で既に計算された財務データを保持する必要がある場合があります。既存の情報に変更を加えていないことが確実な場合や、そのような変更が必要な場合にのみ、「財務の再計算」オプションを使用することをお勧めします。

## 既存の時間数を持つタスクの財務データを保持 {#preserve-financial-data-for-tasks-with-existing-hours}

プロジェクトの財務データが再計算されると、Workfront は、新規または更新された財務情報に従って、以前に記録されたすべての時間数、予定コスト、実際のコスト、予定収益と実収益を遡及的に再計算します。

* [プロジェクトの収益を保持](#preserve-project-revenue)
* [プロジェクトのコストを保持](#preserve-project-cost)

### プロジェクトの収益を保持  {#preserve-project-revenue}

収益率は、プロジェクトの全期間中に変化する場合があります。

請求レートと収益について詳しくは、[請求と収益の概要](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md)の記事を参照してください。

収益率は、以下のレベルで変更できます。

* システムレベル（担当業務の場合）\
  システムレベルで請求レートを使用して担当業務を作成する方法について詳しくは、[担当業務を作成および管理](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)の記事を参照してください。

* ユーザーレベル\
  ユーザーの請求レート情報の変更について詳しくは、[ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)の記事を参照してください。

* 会社レベル（担当業務の場合）\
  詳しくは、[会社レベルでの担当業務請求レートの上書き](../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md)を参照してください。

* プロジェクトレベル（担当業務の場合）\
  プロジェクトレベルでの担当業務請求レートの上書きについて詳しくは、[プロジェクトでの担当業務請求レートの上書きと収益の計算の概要](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)の記事を参照してください。

例えば、プロジェクトの進行中にユーザーの請求レートが 1 時間あたり50 ドルから75 ドルに変わるが、既存のすべてのデータを古い料金（1 時間あたり50 ドル）で計算したままにしたいとします。しかし、プロジェクトの財務が再計算されると、既に既存の財務データを持つタスクの収益は、新しい請求レート（1 時間当たり 75 ドル）を反映して更新されます。

* [請求記録の作成によるプロジェクト収益の保持](#preserve-project-revenue-by-creating-a-billing-record)
* [複数の請求レートの上書きを使用してプロジェクト収益を保持](#preserve-project-revenue-by-using-multiple-billing-rate-overrides)

#### 請求記録の作成によるプロジェクト収益の保持 {#preserve-project-revenue-by-creating-a-billing-record}

請求レートが上記のレベルで変更された場合は、手動の「財務再計算」オプションを使用しないか、プロジェクトに記録された時間や古いレートを使用して請求済みステータスの請求記録に計算した時間をロックすることで、プロジェクトで既に計算済みの既存の収益を保持できます。

プロジェクト上の財務を再計算しない場合や、請求済み請求記録に記録された時間をロックした場合、レート変更後に記録された時間は新しいレートで計算され、コストレート変更前に記録された時間は古いレートで計算されます。

請求記録の作成について詳しくは、[請求記録の作成](../../../manage-work/projects/project-finances/create-billing-records.md)の記事を参照してください。

#### 複数の請求レートの上書きを使用してプロジェクト収益を保持 {#preserve-project-revenue-by-using-multiple-billing-rate-overrides}

プロジェクトレベルで担当業務の請求レートが変更された場合、指定期間内にロックされた複数の請求レートの上書きを使用して、プロジェクトで既に計算済みの既存の収益を保持できます。

複数の請求レートの上書きの使用について詳しくは、[担当業務請求レートの上書きとプロジェクトでの収益の計算の概要](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md)の記事を参照してください。

>[!NOTE]
>
>これは、プロジェクトレベルで変更された担当業務の請求レートにのみ適用されます。

### プロジェクトのコストを保持 {#preserve-project-cost}

コスト率は、次のレベルで変更できます。

* システムレベル（担当業務用）\
  システムレベルでコスト率を使用して担当業務を作成する方法について詳しくは、[担当業務の作成と管理](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md)の記事を参照してください。

* ユーザーレベル\
  ユーザーのコスト率情報の変更について詳しくは、[ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md)の記事を参照してください。

請求レートが上記のレベルで変更された場合は、プロジェクトに記録された時間や古いレートを使用して請求済みステータスの請求記録に計算した時間をロックすることで、プロジェクトで計算した既存のコストを保持できます。請求記録の作成について詳しくは、[請求記録の作成](../../../manage-work/projects/project-finances/create-billing-records.md)の記事を参照してください。

[プロジェクトの財務を手動で再計算](#manually-recalculate-finances-for-a-project)の節で説明したように、請求記録を作成したくない場合は、手動での「財務を再計算」オプションも使用しないでください。

プロジェクト上の財務を再計算しない場合や、請求済み請求記録に記録された時間をロックした場合、レート変更後に記録された時間は新しいレートで計算され、コストレート変更前に記録された時間は古いレートで計算されます。

## 手動でのプロジェクトの財務の再計算 {#manually-recalculate-finances-for-a-project}

プロジェクトの期間中にレートが変更され、コストと収益の計算に新しいレートを反映させる場合は、プロジェクトの財務を手動で再計算する必要があります。

>[!NOTE]
>
>この記事の[既存の時間のタスクの財務データを保持](#preserve-financial-data-for-tasks-with-existing-hours)の節内の手順に従って、財務を手動で再計算するときに、新しいレートを反映するために収益値が更新されないようにすることができます。プロジェクトの財務を手動で再計算する場合は、新しいレートを反映するようにコスト値が常に更新されます。

Workfront のプロジェクトの財務は、プロジェクトページからまたはプロジェクトリストやレポートから再計算できます。

一括編集中に財務を再計算できます。詳しくは、 [財務を一括で手動で再計算する](#manually-recalculate-finances-in-bulk) 」の節を参照してください。

1. 財務を再計算するプロジェクトに移動し、 **その他** アイコン ![](assets/qs-more-icon-on-an-object.png) をクリックします。

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   または

   プロジェクトリストまたはレポートに移動して 1 つまたは複数のプロジェクトを選択し、リストの上部にある&#x200B;**その他**&#x200B;アイコン ![](assets/qs-more-icon-on-an-object.png) をクリックします。

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >プロジェクトの複雑さに応じて、最適なパフォーマンスを確保するために、財務を一括で再計算する場合は、多数のプロジェクトを選択しないことをお勧めします。プロジェクトが複雑すぎる原因として考えられるものとしては、複数の依存関係や割り当てまたは多数のカスタムフィールドなどがあります。

1. クリック **財務の再計算**.

   プロジェクトのすべての予定コストと収益は、新しい情報で再計算されます。

   プロジェクトの財務が正常に再計算されたことをブラウザーの上部に確認するメッセージが表示されます。
ロックされていない既存のコスト値と一部の収益値は、新しいレートを反映するように更新されます。

## 財務を一括で手動で再計算する{#manually-recalculate-finances-in-bulk}

複数のプロジェクトの財務を一括編集することで、手動で再計算することができます。これにより、プロジェクトの収益が遡及的に再計算されます。

>[!IMPORTANT]
>
>この記事の[既存の時間のタスクの財務データを保持](#preserve-financial-data-for-tasks-with-existing-hours)の節内の手順に従って、財務を手動で再計算するときに、新しいレートを反映するために収益値が更新されないようにすることができます。プロジェクトの財務を手動で再計算する場合は、新しいレートを反映するようにコスト値が常に更新されます。

複数のプロジェクトの財務を手動で再計算するには、以下を実行します。

1. プロジェクトのリストに移動します。
1. リスト内の複数のプロジェクトを選択し、 **その他** アイコン ![](assets/qs-more-icon-on-an-object.png) をクリックします。

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >プロジェクトの複雑さに応じて、最適なパフォーマンスを確保するために、大量のプロジェクトを一括編集する際には選択しないことをお勧めします。プロジェクトが複雑すぎる原因として考えられるものとしては、複数の依存関係や割り当てまたは多数のカスタムフィールドなどがあります。

1. クリック **財務の再計算**.

   選択したプロジェクトのすべての計画原価と収益は、新しい情報で再計算されます。

   プロジェクトの財務が正常に再計算されたことをブラウザーの上部に確認する必要があります。

## 財務の自動再計算をトリガーするアクション

次のアクションは、Workfront のプロジェクトの財務の再計算をトリガーします。

* タスクステータスの変更
* 時間を含むタスクを別のプロジェクトに移動
* プロジェクトステータスを完了からアクティブステータスに変更

>[!NOTE]
>
>プロジェクトのステータスを変更すると、予定された値のみが再計算されます。

プロジェクトレベルの&#x200B;**その他**&#x200B;メニュー![](assets/qs-more-menu.png)で「**財務を再計算**」をクリックすると、財務を手動で再計算することもできます。
