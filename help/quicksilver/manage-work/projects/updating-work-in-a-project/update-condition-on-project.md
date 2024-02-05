---
product-area: projects
navigation-topic: update-work-in-a-project
title: プロジェクトの状況の更新
description: プロジェクトの状況は、プロジェクトに関連する作業がスムーズに進んでいるかどうか、または何らかの課題が発生したかどうかを示すために、プロジェクトに付けられるフラグです。これは、プロジェクトに対して積極的に取り組んでいるかどうかを示す、プロジェクトのステータスとは異なります。
author: Alina
feature: Work Management
exl-id: 1f46386e-e1ae-4845-8cc4-09dd7d39076f
source-git-commit: 31ee3259167532e1e1efa75d635786762f6e476e
workflow-type: tm+mt
source-wordcount: '550'
ht-degree: 88%

---

# プロジェクトの状況の更新

プロジェクトの状況は、プロジェクトに関連する作業がスムーズに進んでいるかどうか、または何らかの課題が発生したかどうかを示すために、プロジェクトに付けられるフラグです。これは、プロジェクトに対して積極的に取り組んでいるかどうかを示す、プロジェクトのステータスとは異なります。

プロジェクトの状況は、自動または手動で設定できます。プロジェクトの状況を手動で変更するには、プロジェクト所有者であるか、プロジェクトの管理権限が必要です。

Adobe Workfront 管理者は、環境にカスタムの状況を作成できます。詳しくは、[カスタム状況の作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td>

新しいライセンスの場合：
<p>標準</p>

現在のライセンスの場合：
<ul><li><p>プラン</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクトに対する表示以上のアクセス権</p> <p>タスクおよびイシューに対する編集アクセス権 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>状況を表示するための、タスクおよびイシューに対する表示以上の権限</p>
   <p>状況を更新するための、タスクおよびイシューに対する管理権限</p>
     </td> 
  </tr> 
 </tbody> 
</table>

*保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者にお問い合わせください。 詳しくは、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 状況の自動設定

プロジェクトの状況を自動的に設定するかどうかは、プロジェクトの状況タイプで決まります。Workfront でプロジェクトの状況を自動的に設定するには、状況タイプを「進捗ステータス」に設定する必要があります。

システム内の新規プロジェクトの「状況タイプ」フィールドのデフォルトは、設定エリアでプロジェクトの環境設定を指定する際に、Workfront 管理者またはグループ管理者が決定します。詳しくは、[システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md)を参照してください。

プロジェクトを作成すると、その時点のプロジェクトの進捗ステータスに合わせて、プロジェクトの状況が自動的に設定されます。プロジェクトの進捗ステータスは、プロジェクトのタスクの進捗に基づいています。

プロジェクト状況と、進捗ステータスに基づくその計算方法については、[プロジェクトの進捗ステータスの概要](../../../manage-work/projects/planning-a-project/project-progress-status.md)を参照してください。

## プロジェクトの状況の手動更新

プロジェクトの条件の種類を進捗状況ステータスではなく手動に設定した場合は、手動でプロジェクトの条件を更新できます。

1. 状況を更新するプロジェクトに移動します。
1. 次をクリック： **プロジェクトの詳細** 」セクションを使用して、

1. 「**状況タイプ**」フィールドが「**手動**」に設定されていることを確認します。

   ![](assets/project-details-overview-edit-enabled-with-condition-shot-nwe-350x251.png)

1. 「**状況**」フィールドで、関連する作業が順調に進んでいるかどうかや遅延があるかどうかについての理解に一致するものを、次のオプションから選択します。

   * **目標どおり**
   * **危険あり**
   * **トラブル発生中**

   プロジェクト状況について詳しくは、[プロジェクト状況と状況タイプの概要](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md)を参照してください。

   >[!NOTE]
   >
   >状況は環境に合わせてカスタマイズできるので、お使いの環境で状況の選択肢が 4 つ以上ある場合もあります。状況の名前は、上記の名前とは異なる場合があります。Workfront での状況のカスタマイズについては、[カスタム状況の作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-conditions/create-edit-custom-conditions.md)を参照してください。

1. 「**変更を保存**」をクリックします。
