---
title: レイアウトテンプレートを使用して詳細ビューをカスタマイズする
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Workfront 管理者は、タスク、イシュー、ドキュメント、プログラム、またはポートフォリオの表示中にユーザーが左側のパネルの「詳細」セクションを選択したときに表示される情報を、レイアウトテンプレートを使用して決定できます。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: 1474e1dd-9b10-476e-9526-6577efa8d1c2
source-git-commit: 7c624eff8931d206285b6c4d91083f4bf09a88b0
workflow-type: ht
source-wordcount: '558'
ht-degree: 100%

---

# レイアウトテンプレートを使用して詳細ビューをカスタマイズする

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

Workfront 管理者は、タスク、イシュー、ドキュメント、プログラム、またはポートフォリオの表示中にユーザーが左側のパネルの詳細アイコン ![](assets/project-details-icon.png) をクリックしたときに表示される情報を、レイアウトテンプレートを使用して決定できます。

<!--
or billing record
-->

また、この情報が表示される情報の順序を変更することもできます。例えば、ユーザーに表示されるすべてのタスクについて、カスタムフォーム情報をユーザーに表示されるすべてのタスクの詳細ビューの上部に移動できます。

レイアウトテンプレートの作成について詳しくは、[レイアウトテンプレートを作成および管理](../use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

グループのレイアウトテンプレートについて詳しくは、[グループのレイアウトテンプレートを作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)を参照してください。

レイアウトテンプレートを設定した後、変更を他のユーザーに表示するために、ユーザーに割り当てる必要があります。レイアウトテンプレートのユーザーへの割り当てについて詳しくは、[ユーザーをレイアウトテンプレートに割り当てる](../use-layout-templates/assign-users-to-layout-template.md)を参照してください。

オブジェクトの詳細ビューに加えた変更により、次のエリアでユーザーに表示されるフィールドの可用性と順序も決まります。


* 「オブジェクトを作成」ボックス（「タスクを作成」など）

  ![](assets/new-task-dialog.png)


* タスクを編集、イシューを編集、プロジェクトを編集など、オブジェクトの編集時の「オブジェクトを編集」画面

  ![](assets/edit-task-screen.png)


* オブジェクトを一括編集する際の「オブジェクトを編集」画面。現在、これはプロジェクトの一括編集でサポートされています。

  ![](assets/customize-edit-projects-in-bulk-box-with-layout-template.png)


* タスクとイシューのリストの概要 ![](assets/summary-panel-icon.png) パネル

  ![](assets/summary-area.png)

  >[!NOTE]
  >
  >レイアウトテンプレートの変更は、ログインしたユーザーに割り当てられたタスクとイシューに対してのみ、概要パネルのフィールドの順序と可用性に影響します。

* 「イシューをタスクに変換」ボックスや「イシューをプロジェクトに変換」ボックスなどの変換ボックス。

  ![「イシューをタスクに変換」ボックス](assets/convert-issue-to-task-box.png)

グループのレイアウトテンプレートについて詳しくは、[グループのレイアウトテンプレートを作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>これらの手順をシステムレベルで実行するには、システム管理者のアクセスレベルが必要です。
グループに対して実行するには、そのグループの管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 詳細ビューでユーザーに表示する項目をカスタマイズする

1. [レイアウトテンプレートを作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)で説明されるように、レイアウトテンプレート上での作業を開始します。
1. 「**ユーザーの表示項目をカスタマイズする**」で下矢印![](assets/dropdown-arrow-12x12.png)をクリックして、「**プロジェクト**」、「**タスク**」、「**イシュー**」、「**プログラム**」、または「**ポートフォリオ**」をクリックします。
<!--
, or billing record
-->

1. 「**詳細**」セクションで、次のいずれかの操作を行って、詳細ビューに表示する項目をカスタマイズします。

   * 任意のセクションヘッダー ![](assets/move-icon---dots.png) をドラッグして、順序を変更します。
   * **概要**&#x200B;および&#x200B;**カスタムフォーム**&#x200B;でオプションを有効または無効にして、それらを表示または非表示にします。

     これらのセクションの 1 つですべてのフィールドを非表示にした場合、セクション全体が非表示になります。

     すべてのフィールドは、デフォルトで有効になっています。

1. 引き続きレイアウトテンプレートをカスタマイズします。

   または

   カスタマイズが完了したら、「**保存**」をクリックします。

   >[!TIP]
   >
   >いつでも「保存」をクリックして進行状況を保存して、後でテンプレートの変更を続行できます。
