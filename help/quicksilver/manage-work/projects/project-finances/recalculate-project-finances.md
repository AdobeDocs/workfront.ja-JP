---
title: プロジェクトの財務を再計算
product-area: projects
navigation-topic: financials
description: 財務は、プロジェクトに記録された時間に変更が発生したとき、またはコストと売上高の計算に使用された率で、プロジェクトで計算されます。
author: Alina
feature: Work Management
exl-id: 5a90c5a1-8b26-4b6f-b9ec-f446a2e94ff0
source-git-commit: bfe77796863bb2d7d324901721fda7fa045c2c0b
workflow-type: tm+mt
source-wordcount: '1620'
ht-degree: 0%

---

# プロジェクトの財務を再計算

財務は、プロジェクトに記録された時間に変更が発生したとき、またはコストと売上高の計算に使用された率で、プロジェクトで計算されます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトおよび財務データへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限が設定されているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>財務を管理する権限を持つプロジェクトに対する権限を管理します</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## Adobe Workfrontの財政計算に関する検討事項

Enhanced Analytics では、次の方法で財務を計算します。

* プロジェクトの「財務を再計算」オプションを使用すると、プロジェクトのコストと収益を手動で再計算できます。
* また、一部のアクションは自動再計算をトリガーにしています。

プロジェクトの期間中にユーザーまたは役割の割合が変更されると、次のことが起こる場合があります。

* 変更が行われると、時間が記録され、財務情報が計算されると、更新されたレートがその時点から使用されます。 レートを変更しても、変更前の計算方法には影響しません。 ログに記録されたすべての既存の時間に対して、古いレートが財務情報の計算に使用されます。
* 「財務の再計算」オプションを使用すると、Adobe Workfrontに対して、これまでに記録されたすべての時間に遡って新しいレートを強制的に使用させることができます。 これにより、Workfrontは、以前に入力した時間、計画コスト、売上高をすべて新しいレート情報に従って遡って再計算します。

>[!CAUTION]
>
>特定のプロジェクトの財務を手動で再計算する前に、以前のレートで既に計算された財務データを保持する必要がある場合があります。 「財務の再計算」オプションは、既存の情報に変更を加えていないことが確実な場合、またはそのような変更が必要な場合にのみ使用することをお勧めします。

## 既存の時間のタスクの財務データを保持 {#preserve-financial-data-for-tasks-with-existing-hours}

プロジェクトの財務データが再計算されると、Workfrontでは、新規または更新された財務情報に従って、以前に記録されたすべての時間、計画済み、実際のコスト、計画済みおよび実際の収益が遡って再計算されます。

* [プロジェクトの収益を保持](#preserve-project-revenue)
* [プロジェクトコストを保持](#preserve-project-cost)

### プロジェクトの収益を保持  {#preserve-project-revenue}

収益率は、プロジェクトの有効期間中に変化する場合があります。

請求率と売上高について詳しくは、 [請求と売上高の概要](../../../manage-work/projects/project-finances/billing-and-revenue-overview.md).

収益率は、次のレベルで変更できます。

* システムレベル（ジョブロールの場合）\
  システムレベルで請求率を使用してジョブロールを作成する方法の詳細は、この記事を参照してください。 [ジョブの役割の作成と管理](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* ユーザーレベル\
  ユーザーの請求率情報の変更について詳しくは、 [ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* 会社レベル（ジョブロールの場合）\
  詳しくは、 [会社レベルでのジョブロール請求率の上書き](../../../administration-and-setup/set-up-workfront/organizational-setup/override-job-role-billing-rates-company-level.md).

* プロジェクトレベル（ジョブロールの場合）\
  プロジェクトレベルでのジョブの役割率の上書きの詳細は、この記事を参照してください [ジョブ・ロール請求率の上書きとプロジェクトでの収益の計算の概要](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

例えば、プロジェクトの進行中にユーザーの請求率が 1 時間あたり$50 から$75 に変わり、既存のすべてのデータを古い料金（$50 と時間）で計算したままにしたいとします。 ただし、プロジェクトの財務が再計算されると、既に既存の財務データを持つタスクの収益は、新しい請求率（1 時間当たり 75 ドル）を反映して更新されます。

* [請求レコードの作成によるプロジェクト収益の保持](#preserve-project-revenue-by-creating-a-billing-record)
* [複数の請求レート上書きを使用してプロジェクト収益を保持](#preserve-project-revenue-by-using-multiple-billing-rate-overrides)

#### 請求レコードの作成によるプロジェクト収益の保持 {#preserve-project-revenue-by-creating-a-billing-record}

請求レートが上記のレベルで変更された場合は、手動の「財務再計算」オプションを使用しないか、古いレートを使用して計算した請求レコードを「請求」ステータスの請求レコードにロックすることで、プロジェクトで既に計算済の既存の収益を保持できます。

プロジェクト上の財務を再計算しない場合や、請求済請求レコードに記録された時間をロックした場合、レート変更後に記録された時間は新しいレートで計算され、原価レート変更前に記録された時間は古いレートで計算されます。

請求レコードの作成について詳しくは、 [請求レコードの作成](../../../manage-work/projects/project-finances/create-billing-records.md).

#### 複数の請求レート上書きを使用してプロジェクト収益を保持 {#preserve-project-revenue-by-using-multiple-billing-rate-overrides}

プロジェクト・レベルでジョブ・ロールの請求レートが変更された場合、指定期間内にロックされた複数の請求レート上書きを使用して、プロジェクトで既に計算済の既存の収益を保持できます。

複数の請求率の上書きの使用について詳しくは、 [ジョブ・ロール請求率の上書きとプロジェクトでの収益の計算の概要](../../../manage-work/projects/project-finances/override-role-billing-rates-and-calculate-project-revenue.md).

>[!NOTE]
>
>これは、プロジェクトレベルで変更されたジョブロールの請求率にのみ適用されます。

### プロジェクトコストを保持 {#preserve-project-cost}

コストレートは、次のレベルで変更できます。

* システムレベル（ジョブロール用）\
  システムレベルでコストレートを使用してジョブロールを作成する方法の詳細については、「 [ジョブの役割の作成と管理](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

* ユーザーレベル\
  ユーザーのコストレート情報の変更の詳細については、「 [ユーザーのプロファイルの編集](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

請求率が上記のレベルで変更された場合は、プロジェクトに記録された時間をロックし、古いレートを使用して計算した既存のコストを「請求」ステータスの請求レコードに保持できます。 請求レコードの作成について詳しくは、 [請求レコードの作成](../../../manage-work/projects/project-finances/create-billing-records.md).

請求レコードを作成しない場合は、「財務の再計算」オプションを使用しないでください。詳しくは、「 [プロジェクトの財務を手動で再計算する](#manually-recalculate-finances-for-a-project) 」を参照してください。

プロジェクト上の財務を再計算しない場合や、請求済請求レコードに記録された時間をロックした場合、レート変更後に記録された時間は新しいレートで計算され、原価レート変更前に記録された時間は古いレートで計算されます。

## プロジェクトの財務を手動で再計算する {#manually-recalculate-finances-for-a-project}

プロジェクトの期間中にレートが変更され、コストと収益の計算に新しいレートを反映させる場合は、プロジェクトの財政を手動で再計算する必要があります。

>[!NOTE]
>
>財務を手動で再計算する場合は、「」セクションの手順に従って、収益値が更新されて新しいレートが反映されないようにできます [既存の時間のタスクの財務データを保持](#preserve-financial-data-for-tasks-with-existing-hours) 」を参照してください。 プロジェクト上の財務を手動で再計算する場合は、新しいレートを反映するようにコスト値が常に更新されます。

プロジェクトの財務は、プロジェクトページ、またはプロジェクトリストまたはレポートから、Workfrontで再計算できます。

一括編集中に財務を再計算できます。 詳しくは、 [財務を一括で手動で再計算する](#manually-recalculate-finances-in-bulk) 」の節を参照してください。

1. 財務を再計算するプロジェクトに移動し、 **その他** アイコン ![](assets/qs-more-icon-on-an-object.png) をクリックします。

   ![](assets/project-level-more-drop-down-expanded-nwe-350x516.png)

   または

   プロジェクトリストまたはレポートに移動して、1 つまたは複数のプロジェクトを選択し、 **その他** アイコン ![](assets/qs-more-icon-on-an-object.png) をクリックします。

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >プロジェクトの複雑さに応じて、最適なパフォーマンスを確保するために財務を一括再計算する場合は、多数のプロジェクトを選択しないことをお勧めします。 プロジェクトが複雑すぎる可能性があるものには、複数の依存関係や割り当て、または多数のカスタムフィールドがあるものがあります。

1. クリック **財務の再計算**.

   プロジェクトのすべての計画済みコストと収益は、新しい情報で再計算されます。

   プロジェクトの財務が正常に再計算されたことをブラウザーの上部に確認するメッセージが表示されます。
既存のコスト値と、新しいレートを反映するように更新がロックされていない一部の売上高値。

## 財務を一括で手動で再計算する{#manually-recalculate-finances-in-bulk}

複数のプロジェクトの財務を一括編集することで、手動で再計算できます。 これにより、プロジェクトの売上高が遡って再計算されます。

>[!IMPORTANT]
>
>財務を手動で再計算する場合は、「」セクションの手順に従って、収益値が更新されて新しいレートが反映されないようにできます [既存の時間のタスクの財務データを保持](#preserve-financial-data-for-tasks-with-existing-hours) 」を参照してください。 プロジェクトの財務を手動で再計算する場合は、新しいレートを反映するようにコスト値が常に更新されます。

複数のプロジェクトの財務を手動で再計算する手順は、次のとおりです。

1. プロジェクトのリストに移動します。
1. リスト内の複数のプロジェクトを選択し、 **その他** アイコン ![](assets/qs-more-icon-on-an-object.png) をクリックします。

   ![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

   >[!TIP]
   >
   >プロジェクトの複雑さに応じて、最適なパフォーマンスを確保するために、大量のプロジェクトを一括編集する際には選択しないことをお勧めします。 プロジェクトが複雑すぎる可能性があるものには、複数の依存関係や割り当て、または多数のカスタムフィールドがあるものがあります。

1. クリック **財務の再計算**.

   選択したプロジェクトのすべての計画原価と収益は、新しい情報で再計算されます。

   プロジェクトの財務が正常に再計算されたことをブラウザーの上部に確認する必要があります。

## 財政の自動再計算をトリガーする行為

次のアクションは、Workfrontのプロジェクトの財務的な再計算をトリガーします。

* タスクステータスの変更
* 時間を含むタスクを別のプロジェクトに移動する
* プロジェクトステータスを完了からアクティブステータスに変更する

>[!NOTE]
>
>プロジェクトのステータスを変更すると、計画された値のみが再計算されます。

また、 **その他** メニュー ![](assets/qs-more-menu.png) プロジェクトレベルで、 **財政を再計算**.
