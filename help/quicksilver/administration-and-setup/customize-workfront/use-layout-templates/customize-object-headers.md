---
title: レイアウトテンプレートを使用したオブジェクトヘッダーのカスタマイズ
user-type: administrator
product-area: system-administration;templates;setup
navigation-topic: layout-templates
description: Adobe Workfront 管理者またはグループ管理者は、レイアウトテンプレートを使用して、ユーザーがオブジェクトページを開いた際にオブジェクトヘッダーに表示されるフィールドを設定できます。
author: Alina
feature: System Setup and Administration
role: Admin
exl-id: cbeaa0d7-a61a-4806-a871-96663d9ce124
source-git-commit: 7ee96045e5673c51c3ce348f395226857686a923
workflow-type: ht
source-wordcount: '512'
ht-degree: 100%

---

# レイアウトテンプレートを使用したオブジェクトヘッダーのカスタマイズ

Adobe Workfront 管理者またはグループ管理者は、レイアウトテンプレートを使用して、ユーザーがオブジェクトのページを開いた際にオブジェクトヘッダーに表示されるフィールドを設定できます。

>[!IMPORTANT]
>
>オブジェクトヘッダーのカスタマイズは、現在、プロジェクト、タスクおよびイシューに対して使用できます。

![](assets/object-header-fields.png)

レイアウトテンプレートの作成について詳しくは、[レイアウトテンプレートの作成と管理](../use-layout-templates/create-and-manage-layout-templates.md)を参照してください。

グループのレイアウトテンプレートについて詳しくは、[グループのレイアウトテンプレートの作成と変更](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md)を参照してください。

レイアウトテンプレートを設定した後、変更を他のユーザーに表示するために、ユーザーに割り当てる必要があります。レイアウトテンプレートのユーザーへの割り当てについて詳しくは、[ユーザーのレイアウトテンプレートへの割り当て](../use-layout-templates/assign-users-to-layout-template.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。


<table>
  <tr>
   <td><strong>Adobe Workfront プラン</strong>
   </td>
   <td>任意
   </td>
  </tr>
  <tr>
   <td><strong>Adobe Workfront ライセンス</strong>
   </td>
   <td>プラン
   </td>
  </tr>
  <tr>
   <td><strong>アクセスレベル設定</strong>
   </td>
   <td>Workfront 管理者またはグループの管理者である必要があります。
<p>
   </td>
  </tr>
</table>

まだアクセス権がない場合は、Workfront 管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、[カスタムアクセスレベルの作成または変更](../../add-users/configure-and-grant-access/create-modify-access-levels.md)を参照してください。

## オブジェクトヘッダーをカスタマイズ

1. [レイアウトテンプレートの作成と管理](../../customize-workfront/use-layout-templates/create-and-manage-layout-templates.md)で説明されるように、レイアウトテンプレート上での作業を開始します。
1. **ユーザーの表示項目をカスタマイズする**&#x200B;ドロップダウンメニューで、「**プロジェクト**」、「**タスク**」または「**イシュー**」を選択します。

   <!--when this will be possible for more than 3 objects, at production, make this more general: update the sentence above to say "select an object you want to customize in the Customize what users see drop-down menu). -->

1. 「[!UICONTROL ヘッダーフィールド]」セクションで、表示されたフィールドにポインタを合わせ、次のいずれかの操作を行います。
   * **x** アイコンをクリックしてフィールドを削除

     または

   * **つかむ**&#x200B;アイコンをクリックしたまま、そのフィールドを新しい場所にドラッグ＆ドロップ

   <!--(NOTE: make sure the default names of these fields have not changed; otherwise, update screen shot)-->

   ![](assets/object-header-field-x-and-grab-icons-in-lt.png)

1. 1 つのオブジェクトのヘッダーには、最大 5 つのフィールドを含めることができます。
既に 5 つのフィールドが選択されている場合、新しいフィールドを追加する前に、1 つのフィールドを削除する必要があります。
1. 「**フィールドを追加**」ボックスで、追加する編集不可能な Workfront フィールドの名前を入力し、リストに表示されたら選択します。このフィールドは、「フィールドを追加」ボックスの右隣に追加され、オブジェクトのヘッダーの左上隅に一番目のフィールドとして表示されます。

   >[!TIP]
   >
   >* オブジェクトの「詳細」セクションの概要エリアに表示されていて、編集不可能なフィールドだけを追加できます。編集不可能なフィールドは、ユーザーが手動で編集できないフィールドです。これらは Workfront で自動的に計算されます。
   >
   >* 既にデフォルトのヘッダーに含まれている編集可能フィールド（プロジェクト所有者、ステータス、完了率、割り当てなど）を追加できます。
   >
   >* イシューのヘッダーに「解決オブジェクト」フィールドを追加すると、イシューに関連付けられた解決オブジェクトがある場合、そのフィールドは「解決するイシュー、タスク、またはプロジェクト」に変わります。


   ![](assets/add-field-to-header-in-lt-list.png)


1. （オプション）追加したフィールドを、別の順序でドラッグ＆ドロップします。

1. 引き続きレイアウトテンプレートをカスタマイズします。

   または

   カスタマイズが完了したら、「**保存**」をクリックします。

   >[!TIP]
   >
   >いつでも「保存」をクリックして進行状況を保存して、後でテンプレートの変更を続行できます。
