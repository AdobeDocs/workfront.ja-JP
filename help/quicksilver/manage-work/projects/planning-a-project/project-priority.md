---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: プロジェクトの優先度の理解と更新
description: プロジェクトの優先順位度を使用する方法はいくつかありますが、それらは互いに通信しません。プロジェクトの重要度を分類する際には、ニーズに合ったプロジェクトの優先度の 1 つを選択し、それを参照することをお勧めします。
author: Alina
feature: Work Management
exl-id: b1e0b6c5-f2a7-455b-836b-6c0ead85e3ad
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: ht
source-wordcount: '599'
ht-degree: 100%

---

# プロジェクトの優先度の理解と更新

プロジェクトの優先順位度を使用する方法はいくつかありますが、それらは互いに通信しません。プロジェクトの重要度を分類する際には、ニーズに合ったプロジェクトの優先度の 1 つを選択し、それを参照することをお勧めします。 

## アクセス要件

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Standard </p>
   Or
   <p>Legacy license: Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to Projects</p> <p><b>NOTE</b> 
   
   If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>
-->
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
   <td> <p>プロジェクトへのアクセスを編集</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトの管理権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## Adobe Workfront のプロジェクト優先度のタイプ

Adobe Workfront でプロジェクトにランク付けするために使用できる優先度のタイプは以下のとおりです。

* **プロジェクト優先度フィールド**：手動でプロジェクトに優先度を割り当てることができます。

  「プロジェクト優先度」フィールドについて詳しくは、この記事の[プロジェクトの優先度に関する考慮事項](#considerations-about-project-priority)を参照してください。

* **ポートフォリオオプティマイザーでのプロジェクトの優先度**、プロジェクトがポートフォリオに関連付けられている場合は、以下のように行います。

  ポートフォリオオプティマイザーでのプロジェクトの優先度ついて詳しくは、[ポートフォリオオプティマイザーでのプロジェクトの優先順度付け](../../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md)の記事を参照してください。

* **リソースプランナーでのプロジェクトの優先度**：リソースプランナーでプロジェクトに手動で優先度を付けて、最初にリソースを受け取るプロジェクトを表示できます。

  リソースプランナーでのプロジェクトの優先度付けについて詳しくは、[リソースプランナーのナビゲーションの概要](../../../resource-mgmt/resource-planning/resource-planner-navigation.md)の記事にある「プロジェクト計画の優先度」の節を参照してください。

## プロジェクトの優先度に関する考慮事項 {#considerations-about-project-priority}

Workfront のプロジェクトに優先度を関連付けることができます。タスクとイシューにも優先度があります。プロジェクトの優先度を示すことで、そのプロジェクトがいかに重要であるかを、システム内の全員に伝えます。

プロジェクトの優先度を選択する際は、以下の点を考慮してください。

* Workfront 管理者が、Workfront で使用できる優先度を定義します。優先度の設定が確定すると、優先度フィールドでプロジェクトと関連付けることができます。 

  Workfront での優先度の作成について詳しくは、[イシューの優先度の作成およびカスタマイズ](../../../administration-and-setup/customize-workfront/creating-custom-status-and-priority-labels/create-customize-priorities.md)を参照してください。

* プロジェクトの「優先度」フィールドを更新しても、この優先度はポートフォリオオプティマイザーやリソースプランナーには転送されません。 
* プロジェクトの優先度の値は、主にレポートの目的で使用されます。

  例えば、このフィールドをプロジェクトフィルターで使用する場合と、優先度が緊急のすべてのプロジェクトを検索できます。 

* Workfront の以下のエリアでプロジェクトの優先度を更新できます。

   * **プロジェクトを編集**&#x200B;ダイアログボックス。
   * プロジェクトの「**プロジェクトの詳細**」タブをクリックします。
   * プロジェクトリストやレポート。

## プロジェクトの「優先度」フィールドを更新

1. 優先度を更新するプロジェクトに移動します。
1. 左側のパネルの「**プロジェクトの詳細**」をクリックします。
1. プロジェクトの詳細エリアの右上隅にある&#x200B;**編集**&#x200B;アイコン ![](assets/qs-edit-icon.png) をクリックし、続いて&#x200B;**概要**&#x200B;を選択します。

1. 「**優先度**」フィールドで、以下のオプションから選択します。

   * なし
   * 低
   * 標準

     これがデフォルトの優先度です。

   * 高
   * 緊急

   ![](assets/project-priority-picker-list-on-project-details-nwe-350x192.png)

1. 「**変更を保存**」をクリックします。

   他のユーザーとコミュニケーションを取り、プロジェクトのそれぞれの優先度の意味を理解する必要があります。
