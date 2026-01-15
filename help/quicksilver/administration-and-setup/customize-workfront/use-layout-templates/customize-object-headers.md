---
title: レイアウトテンプレートを使用したオブジェクトヘッダーのカスタマイズ
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Adobe Workfront 管理者またはグループ管理者は、レイアウトテンプレートを使用して、ユーザーがオブジェクトページを開いた際にオブジェクトヘッダーに表示されるフィールドを設定できます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: cbeaa0d7-a61a-4806-a871-96663d9ce124
source-git-commit: c037b4f9e5530d8dd796bed25021f7073f16061f
workflow-type: tm+mt
source-wordcount: '532'
ht-degree: 58%

---

# レイアウトテンプレートを使用したオブジェクトヘッダーのカスタマイズ

Adobe Workfront 管理者またはグループ管理者は、レイアウトテンプレートを使用して、ユーザーがオブジェクトのページを開いた際にオブジェクトヘッダーに表示されるフィールドを設定できます。

>[!IMPORTANT]
>
>オブジェクトヘッダーのカスタマイズは、現在、プロジェクト、タスクおよびイシューに対して使用できます。

![&#x200B; オブジェクトヘッダーフィールド &#x200B;](assets/object-header-fields.png)

レイアウトテンプレートの作成について詳しくは、[レイアウトテンプレートを作成および管理](../use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

グループのレイアウトテンプレートについて詳しくは、[グループのレイアウトテンプレートを作成および変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)を参照してください。

レイアウトテンプレートを設定した後、変更を他のユーザーに表示するために、ユーザーに割り当てる必要があります。レイアウトテンプレートのユーザーへの割り当てについて詳しくは、[ユーザーのレイアウトテンプレートへの割り当て](../use-layout-templates/assign-users-to-layout-template.md)を参照してください。

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

## オブジェクトヘッダーをカスタマイズ

1. [レイアウトテンプレートの作成と管理](../../customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)で説明されるように、レイアウトテンプレート上での作業を開始します。
1. **ユーザーに表示する項目をカスタマイズ** ドロップダウンメニューで、**プロジェクト**、**タスク** または **イシュー** を選択します。

   <!--when this will be possible for more than 3 objects, at production, make this more general: update the sentence above to say "select an object you want to customize in the Customize what users see drop-down menu). -->

1. [!UICONTROL &#x200B; ヘッダーフィールド &#x200B;] セクションで、現在のフィールドの上にマウスポインターを置いて、次のいずれかの操作を行います。
   * **x** アイコンをクリックしてフィールドを削除

     または

   * **つかむ**&#x200B;アイコンをクリックしたまま、そのフィールドを新しい場所にドラッグ＆ドロップ

   <!--(NOTE: make sure the default names of these fields have not changed; otherwise, update screen shot)-->

   ![&#x200B; オブジェクトヘッダーフィールドの非表示および移動アイコン &#x200B;](assets/object-header-field-x-and-grab-icons-in-lt.png)

1. 1 つのオブジェクトのヘッダーには、最大 5 つのフィールドを含めることができます。
既に 5 つのフィールドが選択されている場合、新しいフィールドを追加する前に、1 つのフィールドを削除する必要があります。
1. 「**フィールドを追加**」ボックスに、追加するカスタムフィールドまたはネイティブのWorkfront フィールドの名前の入力を開始し、リストに表示されたら選択します。 フィールドは「フィールドを追加」ボックスのすぐ右に追加され、オブジェクトのヘッダーの右上隅にある最初のフィールドとして表示されます。

   >[!TIP]
   >
   >* 任意のカスタムフィールドか、オブジェクトの「詳細」セクションの「概要」領域で使用可能な任意のネイティブフィールドを追加できます。 例えば、イシューにのみ「重要度」フィールドがあり、そのフィールドはプロジェクトやタスクに追加できません。
   >
   >* ユーザーがヘッダーのカスタムフィールドを編集し、オブジェクトに添付されていないカスタムフォームにフィールドが含まれている場合、カスタムフォームは自動的にオブジェクトに追加されます。
   >
   >* イシューのヘッダーに「解決オブジェクト」フィールドを追加すると、イシューに関連付けられた解決オブジェクトがある場合、そのフィールドは「解決するイシュー、タスク、またはプロジェクト」に変わります。

   ![&#x200B; ヘッダーにフィールドを追加 &#x200B;](assets/add-field-to-header-in-lt-list.png)

1. （任意）フィールドを別の順序でドラッグ&amp;ドロップします。

1. レイアウトテンプレートのカスタマイズを続行します。 「**適用**」をクリックすると、いつでも進捗を保存できます。

   または

   カスタマイズが終了したら、「保存して閉じる **をクリックし** す。

