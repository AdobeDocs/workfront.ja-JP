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
TQID: https://experienceleague.adobe.com/syB-759yDrJy14crtZfCKYIKWB6eh-bFr6Gt1INGUdc
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 576
ht-degree: 69%

---

# レイアウトテンプレートを使用して詳細ビューをカスタマイズする

Adobe Workfront管理者は、レイアウトテンプレートを使用して、タスク、イシュー、ドキュメント、プログラムまたはポートフォリオを表示する際に、左側のパネルの詳細アイコン ![詳細アイコン &#x200B;](assets/project-details-icon.png)をクリックしたときに表示される情報を決定できます。

また、この情報が表示される情報の順序を変更することもできます。 例えば、ユーザーに表示されるすべてのタスクについて、カスタムフォーム情報をユーザーに表示されるすべてのタスクの詳細ビューの上部に移動できます。

レイアウトテンプレートの作成について詳しくは、[レイアウトテンプレートを作成および管理](../use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

グループのレイアウトテンプレートについて詳しくは、[グループのレイアウトテンプレートの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)を参照してください。

レイアウトテンプレートを設定した後、変更を他のユーザーに表示するために、ユーザーに割り当てる必要があります。 レイアウトテンプレートのユーザーへの割り当てについて詳しくは、[ユーザーをレイアウトテンプレートに割り当てる](../use-layout-templates/assign-users-to-layout-template.md)を参照してください。

オブジェクトの詳細ビューに加えた変更により、次のエリアでユーザーに表示されるフィールドの可用性と順序も決まります。


* 「オブジェクトを作成」ボックス（「タスクを作成」など）

  ![新しいタスクダイアログ &#x200B;](assets/new-task-dialog.png)


* タスクを編集、イシューを編集、プロジェクトを編集など、オブジェクトの編集時の「オブジェクトを編集」画面

  ![&#x200B; タスク画面を編集](assets/edit-task-screen.png)


* オブジェクトを一括編集する際の「オブジェクトを編集」画面。 現在、これはプロジェクトの一括編集でサポートされています。

  ![&#x200B; プロジェクトの編集をカスタマイズ &#x200B;](assets/customize-edit-projects-in-bulk-box-with-layout-template.png)


* タスクと問題のリストの概要パネル ![概要パネル &#x200B;](assets/summary-panel-icon.png)

  ![概要領域](assets/summary-area.png)

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
1. **ユーザーに表示される内容をカスタマイズ**&#x200B;の下の下向き矢印![下向き矢印](assets/dropdown-arrow-12x12.png)をクリックし、**プロジェクト**、**タスク**、**イシュー**、**プログラム**、または&#x200B;**Portfolio**<!--, or billing record-->&#x200B;をクリックします。
1. 「**詳細**」セクションで、次のいずれかの操作を行って、詳細ビューに表示する項目をカスタマイズします。

   * 任意のセクション ヘッダー![移動アイコン &#x200B;](assets/move-icon---dots.png)をドラッグして、順序を変更します。
   * 様々な領域（**Overview**、**Finance**、**カスタム Forms**&#x200B;など）でオプションを有効または無効にして、表示または非表示にします。

     これらのセクションの 1 つですべてのフィールドを非表示にした場合、セクション全体が非表示になります。

     すべてのフィールドはデフォルトで有効になっています。 領域の「**すべてを選択**」チェックボックスを選択またはオフにすると、その領域のすべてのフィールドを表示または非表示にできます。

     ![&#x200B; レイアウトテンプレートの詳細ビュー](assets/layout-template-details-view-updated-save-buttons.png)

1. レイアウトテンプレートのカスタマイズを続行します。 「**適用**」はいつでもクリックして、進行状況を保存できます。

   または

   カスタマイズが完了したら、**保存して閉じる**&#x200B;をクリックします。

