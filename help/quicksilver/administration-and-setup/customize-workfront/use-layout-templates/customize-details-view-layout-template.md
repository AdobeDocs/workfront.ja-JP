---
title: レイアウトテンプレートを使用した詳細ビューのカスタマイズ
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Workfront 管理者は、タスク、イシュー、ドキュメント、プログラム、またはポートフォリオの表示中にユーザーが左側のパネルの「詳細」セクションを選択したときに表示される情報を、レイアウトテンプレートを使用して決定できます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 1474e1dd-9b10-476e-9526-6577efa8d1c2
source-git-commit: e5416fab4f4ad1f2c31edf962554ddd6a4c2f1e5
workflow-type: tm+mt
source-wordcount: '631'
ht-degree: 65%

---

# レイアウトテンプレートを使用して詳細ビューをカスタマイズする

{{preview-fast-release-general}}

Adobe Workfront管理者は、レイアウトテンプレートを使用して、タスク、イシュー、ドキュメント、プログラム、ポートフォリオを表示している際に、左側のパネルの詳細アイコン ![&#x200B; 詳細アイコン &#x200B;](assets/project-details-icon.png) をクリックしたときに表示される情報を指定できます。

<!--
or billing record
-->

また、この情報が表示される情報の順序を変更することもできます。例えば、ユーザーに表示されるすべてのタスクについて、カスタムフォーム情報をユーザーに表示されるすべてのタスクの詳細ビューの上部に移動できます。

レイアウトテンプレートの作成について詳しくは、[レイアウトテンプレートを作成および管理](../use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

グループのレイアウトテンプレートについて詳しくは、[グループのレイアウトテンプレートを作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)を参照してください。

レイアウトテンプレートを設定した後、変更を他のユーザーに表示するために、ユーザーに割り当てる必要があります。レイアウトテンプレートのユーザーへの割り当てについて詳しくは、[ユーザーをレイアウトテンプレートに割り当てる](../use-layout-templates/assign-users-to-layout-template.md)を参照してください。

オブジェクトの詳細ビューに加えた変更により、次のエリアでユーザーに表示されるフィールドの可用性と順序も決まります。


* 「オブジェクトを作成」ボックス（「タスクを作成」など）

  ![&#x200B; 新規タスクダイアログ &#x200B;](assets/new-task-dialog.png)


* タスクを編集、イシューを編集、プロジェクトを編集など、オブジェクトの編集時の「オブジェクトを編集」画面

  ![&#x200B; タスクを編集画面 &#x200B;](assets/edit-task-screen.png)


* オブジェクトを一括編集する際の「オブジェクトを編集」画面。現在、これはプロジェクトの一括編集でサポートされています。

  ![&#x200B; プロジェクトの編集のカスタマイズ &#x200B;](assets/customize-edit-projects-in-bulk-box-with-layout-template.png)


* タスクおよび問題のリストの概要パネル ![&#x200B; 概要パネル &#x200B;](assets/summary-panel-icon.png)

  ![&#x200B; 概要領域 &#x200B;](assets/summary-area.png)

  >[!NOTE]
  >
  >レイアウトテンプレートの変更は、ログインしたユーザーに割り当てられたタスクとイシューに対してのみ、概要パネルのフィールドの順序と可用性に影響します。

* 「イシューをタスクに変換」ボックスや「イシューをプロジェクトに変換」ボックスなどの変換ボックス。

  ![「イシューをタスクに変換」ボックス](assets/convert-issue-to-task-box.png)

グループのレイアウトテンプレートについて詳しくは、[グループのレイアウトテンプレートを作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td><p>標準</p>
       <p>プラン</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>これらの手順をシステムレベルで実行するには、システム管理者のアクセスレベルが必要です。</p>
        <p>グループに対して実行するには、そのグループの管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 詳細ビューでユーザーに表示する項目をカスタマイズする

1. [レイアウトテンプレートを作成と管理](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)で説明されるように、レイアウトテンプレート上での作業を開始します。
1. ![&#x200B; ユーザーに表示するものをカスタマイズ &#x200B;](assets/dropdown-arrow-12x12.png) の下の下向き矢印 **下向き矢印** をクリックし、**プロジェクト**、**タスク**、**イシュー**、**プログラム**、**Portfolio**<!--, or billing record--> のいずれかをクリックします。
1. 「**詳細**」セクションで、次のいずれかの操作を行って、詳細ビューに表示する項目をカスタマイズします。

   * セクションヘッダー ![&#x200B; 移動アイコン &#x200B;](assets/move-icon---dots.png) をドラッグして、順序を変更します。
   * 様々な領域（「概要」 **、「財務**、「カスタムForms **&#x200B;**&#x200B;など **の下にあるオプションを有効または無効にして、表示と非表示を切り替** ます。

     これらのセクションの 1 つですべてのフィールドを非表示にした場合、セクション全体が非表示になります。

     すべてのフィールドは、デフォルトで有効になっています。 ある領域の **すべてを選択** チェックボックスをオンまたはオフにして、その領域のすべてのフィールドを表示または非表示にすることができます。

   <span class="preview"> プレビュー環境のサンプル画像：</span>
   ![&#x200B; レイアウトテンプレートの詳細ビュー &#x200B;](assets/layout-template-details-view-updated-save-buttons.png)

   本番環境のサンプル画像：
   ![&#x200B; レイアウトテンプレートの詳細ビュー &#x200B;](assets/layout-template-details-view.png)

1. <span class="preview"> プレビュー環境の場合：レイアウトテンプレートのカスタマイズを続行します。 「**適用**」をクリックすると、いつでも進捗を保存できます。</span>

   <span class="preview">または</span>

   <span class="preview"> カスタマイズが終了したら、「**保存して閉じる** をクリックします。</span>

1. 実稼動環境の場合：レイアウトテンプレートのカスタマイズを続行します。

   または

   カスタマイズが終了したら、「**保存**」をクリックします。

   >[!TIP]
   >
   >いつでも「**保存**」をクリックして進行状況を保存して、後でテンプレートの変更を続行できます。
