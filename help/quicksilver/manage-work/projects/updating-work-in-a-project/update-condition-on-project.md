---
product-area: projects
navigation-topic: update-work-in-a-project
title: プロジェクトの条件を更新
description: プロジェクトの「条件」は、プロジェクトに関連する作業がスムーズに進むかどうか、または道路ブロックが発生したかどうかを示すために、プロジェクトに配置されるフラグです。 これは、プロジェクトのステータスとは異なり、プロジェクトに対して積極的に作業を行っているかどうかを示します。
author: Alina
feature: Work Management
exl-id: 1f46386e-e1ae-4845-8cc4-09dd7d39076f
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 0%

---

# プロジェクトの条件を更新

プロジェクトの「条件」は、プロジェクトに関連する作業がスムーズに進むかどうか、または道路ブロックが発生したかどうかを示すために、プロジェクトに配置されるフラグです。 これは、プロジェクトのステータスとは異なり、プロジェクトに対して積極的に作業を行っているかどうかを示します。

プロジェクトの条件は、自動または手動で設定できます。 プロジェクトの条件を手動で変更するには、プロジェクトの所有者であるか、管理権限が必要です。

Adobe Workfront管理者は、 [カスタム条件の作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td><p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>

新しいライセンスの場合：
<p>標準</p>

現在のライセンスの場合：
<ul><li><p>計画</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトへの表示またはアクセス権の高さ</p> <p>タスクおよび問題へのアクセスを編集 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>タスクおよびタスクの条件を表示するタスクに対する権限を表示または上限に設定します</p>
   <p>条件を更新するためのタスクおよび問題に関する権限を管理します</p>
     </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。 詳しくは、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 条件を自動的に設定

プロジェクトの条件を自動的に設定するには、プロジェクトの条件タイプを使用します。 Workfrontがプロジェクトの条件を自動的に設定するには、「条件タイプ」を「進行状況ステータス」に設定する必要があります。

「設定」領域でプロジェクトの環境設定を行う場合、Workfrontまたはグループ管理者が、システム内の新規プロジェクトの「条件の種類」フィールドのデフォルトを決定します。 詳しくは、 [システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

プロジェクトを作成すると、その時点のプロジェクトの進捗状況ステータスに合わせて、プロジェクトの条件が自動的に設定されます。 プロジェクトの進捗状況ステータスは、プロジェクト上のタスクの進捗状況に基づきます。

プロジェクト条件と、進捗状況ステータスに基づく計算方法について詳しくは、 [プロジェクトの進行状況ステータスの概要](../../../manage-work/projects/planning-a-project/project-progress-status.md).

## プロジェクトの条件を手動で更新する

プロジェクトの条件の種類を進捗状況ステータスではなく手動に設定した場合は、手動でプロジェクトの条件を更新できます。

1. 条件を更新するプロジェクトに移動します。
1. 次をクリック： **プロジェクトの詳細** 」セクションを使用して、

1. 次の点を確認します。 **条件タイプ** フィールドが **手動**.

   ![](assets/project-details-overview-edit-enabled-with-condition-shot-nwe-350x251.png)

1. Adobe Analytics の **条件** 「 」フィールドで、以下のオプションから、関連する作業がスムーズに進むかどうか、または遅延が発生するかどうかを理解できるオプションを選択します。

   * **ターゲット時**
   * **危険にさらされて**
   * **問題が発生している**

   プロジェクト条件の詳細については、 [プロジェクト条件と条件タイプの概要](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

   >[!NOTE]
   >
   >条件は、お使いの環境に合わせてカスタマイズできるので、お使いの環境で条件に対して 3 つ以上のオプションを検索できます。 条件の名前は、上記の名前とは異なる場合があります。 Workfrontの条件のカスタマイズについて詳しくは、 [カスタム条件の作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md).

1. 「**変更を保存**」をクリックします。
