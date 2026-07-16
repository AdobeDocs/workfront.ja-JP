---
content-type: overview
product-area: templates
navigation-topic: financials
title: レートカードのテンプレートへの添付
description: レートカードをテンプレートに割り当てると、そのレートカードは、テンプレートから作成されたすべてのプロジェクトに添付されます。
author: Lisa
feature: Work Management
source-git-commit: ace9a01e852e6d99ddc6f150c0ac34bd4ef44817
workflow-type: tm+mt
source-wordcount: '644'
ht-degree: 10%

---

# レートカードのテンプレートへの添付

レートカードをテンプレートに割り当てると、そのレートカードは、テンプレートから作成されたすべてのプロジェクトに添付されます。 レートカードはプロジェクトのデフォルトになりますが、必要に応じて上書きできます。

レートカードについて詳しくは、[ レートカードの管理](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md)を参照してください。

プロジェクトテンプレートについて詳しくは、[ プロジェクトテンプレートの概要](/help/quicksilver/manage-work/projects/create-and-manage-templates/project-template-overview.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td>ワークフロー Ultimate</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td>標準</td> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>テンプレートへの編集アクセス</td> 
  </tr> 
  <tr> 
   <td>オブジェクト権限</td> 
   <td>請求レートを編集する権限を持つレートカードへの権限を管理します</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 前提条件

テンプレートに割り当てるレートカードは、Workfrontで作成する必要があります。 詳しくは、[評価カードの管理](/help/quicksilver/administration-and-setup/manage-enterprise-operations/manage-rate-cards.md)を参照してください。

レイアウトテンプレートのテンプレートに対して、**レートカード** フィールドを有効にする必要があります。

1. レイアウトテンプレートで、**ユーザーに表示される内容をカスタマイズ**&#x200B;の下にある下向き矢印をクリックし、**テンプレート**&#x200B;をクリックします。
1. **詳細** セクションで、**概要** エリアの&#x200B;**レートカード** フィールドを選択します。

   詳しくは、[ レイアウトテンプレートを使用した詳細ビューのカスタマイズ ](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md)を参照してください。

## レートカードのテンプレートへの添付

{{step1-to-templates}}

1. 新しいテンプレートを作成するか、既存のテンプレートを編集します。
1. テンプレートの詳細/概要/テンプレートの関連付けセクションで、**レートカード** フィールドでレートカードを選択します。

   権限を持つレートカードのみが選択できます。
レートカードの名前を入力して、結果のリストを絞り込むことができます。

   ![ テンプレートでレートカードを選択](assets/select-rate-card-on-template.png)

1. 編集が終了したら、テンプレートを保存します。

   テンプレートの作成について詳しくは、[ プロジェクトテンプレートの作成](/help/quicksilver/manage-work/projects/create-and-manage-templates/create-template.md)を参照してください。

   テンプレートの編集について詳しくは、[ プロジェクトテンプレートの編集](/help/quicksilver/manage-work/projects/create-and-manage-templates/edit-templates.md)を参照してください。

## テンプレートのプロジェクトへの適用

1. テンプレートを使用してプロジェクトを作成します。

   テンプレートからプロジェクトを作成する方法はいくつかあります。 詳しくは、次の記事を参照してください。

   * [テンプレートを使用したプロジェクトの作成](/help/quicksilver/manage-work/projects/create-projects/create-project-from-template.md)
   * [タスクをプロジェクトに変換](/help/quicksilver/manage-work/tasks/manage-tasks/convert-task-to-project.md)
   * [イシューをプロジェクトに変換](/help/quicksilver/manage-work/issues/convert-issues/convert-issue-to-project.md)

   レートカードは自動的にプロジェクトに保存されます。 「新規プロジェクト」ボックスの「概要」/「プロジェクトの関連付け」セクションで、レートカードを削除するか、「**レートカード**」フィールドで別のレートカードを選択できます。

   ![ テンプレートのレートカードがプロジェクトの詳細に表示される](assets/create-project-from-template-rate-card.png)

   レートカードと関連するレートがプロジェクトレート領域に表示されます。

   プロジェクトからレートカードを削除したり、「レート」エリアに別のレートカードを添付したりすることもできます。 詳しくは、[ プロジェクトへのレートカードの添付](/help/quicksilver/manage-work/projects/project-finances/attach-rate-card-to-project.md)を参照してください。

   ![ プロジェクトのテンプレートからのカードの評価](assets/template-rates-on-project.png)

   >[!NOTE]
   >
   >個々のレートがテンプレートにあり、レートカードもテンプレートに添付されている場合、テンプレートからプロジェクトを作成すると、個々のレートとレートカードの両方がレートのリストに表示されます。

1. （オプション）既存のプロジェクトにレートカードを適用するには、テンプレートをプロジェクトに添付します。

   テンプレートのプレビューで「**カスタマイズして添付**」オプションを使用する場合、「テンプレートを添付/オプション」セクションの「**レートカード**」項目を選択して、レートカードをプロジェクトに追加できます。 プロジェクトへの転送からレートカードを除外するには、チェックボックスをオフにします。

   詳しくは、[ プロジェクトへのテンプレートの添付](/help/quicksilver/manage-work/projects/create-and-manage-templates/attach-template-to-project.md)を参照してください。

1. （オプション）特定のプロジェクトのレートカードをテンプレートに保存するには、プロジェクトをテンプレートとして保存します。

   「テンプレートとして保存」ボックスの「オプション」セクションで、**レートカード** アイテムを選択して、レートカードをテンプレートに追加できます。 テンプレートへの転送からレートカードを除外するには、チェックボックスをオフにします。

   詳しくは、[ プロジェクトをテンプレートとして保存](/help/quicksilver/manage-work/projects/manage-projects/save-project-as-template.md)を参照してください。


