---
title: カスタムフィールドとウィジェットの共有の設定
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: デフォルトでは、新しいカスタムフィールドまたはウィジェットをカスタムフォームに追加すると、カスタムフォームにアクセスできるシステム内の誰でも、その項目のラベルや名前などのプロパティを編集できます。 これを変更するには、共有相手を制御します。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 4f591fa3-2cb9-4a22-bfb1-1b50cedfcf3d
source-git-commit: 264419f747b1e975cda8843b37558e78501d93de
workflow-type: tm+mt
source-wordcount: '744'
ht-degree: 49%

---

# カスタムフィールドとウィジェットの共有の設定

デフォルトでは、新しいカスタムフィールドまたはウィジェットをカスタムフォームに追加すると、カスタムフォームにアクセスできるシステム内の誰でも、その項目のラベルや名前などのプロパティを編集できます。 これを変更するには、共有相手を制御します。

カスタムフォームのカスタムフィールドとウィジェットについて詳しくは、[ カスタムフォームの作成](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)を参照してください。

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
  <tr> 
   <td>アクセスレベル設定</td> 
   <td> <p>カスタムフォームへの管理アクセス権</p> </td> 
  </tr>  
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--

## Configure sharing a custom field or widget from the list of forms

{{step-1-to-setup}}

1. In the left panel, click **Custom Forms**.
1. Click **Fields** to open the Fields area.
1. Select the item you want to configure sharing for, then click ![Share icon](assets/share-icon.png).
1. In the Custom Field Access box that displays, specify who you want to share the item with and how you want to share it:

   1. Near the lower-left corner of the **Custom Field Access** box, under **Give custom field access to**, start typing the name of a user, team, job role, group, or company you want to share the item with, then click the name when it appears.

      ![Custom Field Access box](assets/share-field-give-access-to.jpg)

   1. If you want to be more specific about how you want to share the item, click the drop-down list to the right of the name, then use any of the following options:

      ![Sharing options](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">View it</td> 
         <td> <p>You can click <strong>Advanced Settings</strong> to specify whether you want the user or users to be able to use their access to add the item to a custom form or share it with other users.</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">Manage it</td> 
         <td> <p>Allows access to edit the custom field and to see it in the Field Library and on the page where you build custom forms.</p> <p>You can click <strong>Advanced Settings</strong> to specify whether you want the user or users to be able to use their access to delete the item from the system or share it with other users.</p> </td> 
        </tr> 
       </tbody> 
      </table>   

1. (Optional) Repeat the previous step to add other names to the list and configure their options.
1. (Optional) Click the gear icon ![Settings icon](assets/gear-icon-settings.png) in the top-right corner if you want to choose a system-wide sharing option for the field.

   Not all of the following options display in this drop-down menu at the same time. For example, the second one displays only when one of the other two are selected.

   * **Make this editable system-wide so that everyone in Workfront can edit it** (the default option)

     When you add a custom field or widget and you don't limit sharing for it, everyone in the system who has access to custom forms can view it and edit its properties.
   
   * **Remove system-wide edit access**

     Limits access to only those whom you added to the list. 
   
   * **Make this visible system-wide so that everyone in Workfront can see it**

1. Click **Save**.

-->

## カスタムフィールドまたはウィジェットの共有の設定

{{step-1-to-setup}}

1. 左側のパネルで、「**カスタムフォーム**」をクリックします。
1. フォームとフィールドのリストから共有するには：

   1. 「**フィールド**」をクリックしてフィールドエリアを開きます。
   1. 共有するフィールドを選択し、![共有アイコン ](assets/share-icon.png)をクリックします。

1. フォームデザイナーから共有するには：
   1. カスタムフォームを開くか、新しいカスタムフォームを作成します。
   1. フォームデザイナーで、共有するフィールドを選択し、右側のフィールド編集領域で「**共有**」をクリックします。

1. 共有ボックスの&#x200B;**フィールドに**&#x200B;へのアクセス権を付与の下で、アイテムを共有するユーザー、チーム、担当業務、グループ、会社、またはビジネスプロファイルの名前の入力を開始し、名前が表示されたら&#x200B;**Enter**&#x200B;を押します。
1. アイテムの共有方法をより具体的に説明する場合は、名前の右側にあるドロップダウンメニューをクリックし、次のいずれかのオプションを使用します。

   * **表示**: **詳細設定** アイコン ![詳細設定アイコン ](assets/configure-options-icon.png)をクリックして、ユーザーがカスタムフォームに項目を追加するか、他のユーザーと共有するかを指定します。
   * **管理**: カスタムフィールドを編集し、フィールドライブラリとフォームデザイナーの両方で表示するためのアクセスを許可します。 **詳細設定** アイコン ![詳細設定アイコン ](assets/configure-options-icon.png)をクリックして、ユーザーがシステムから項目を削除するか、他のユーザーと共有するかを指定します。

1. （オプション）手順5 ～ 6を繰り返して、他の名前をリストに追加し、そのオプションを設定します。
1. （オプション）フィールドのシステム全体の共有オプションを選択します。

   * **システム内のすべてのユーザーが**&#x200B;を編集できます（デフォルトのオプション）

     カスタムフィールドまたはウィジェットを追加し、共有を制限しない場合、カスタムフォームにアクセスできるシステム内のすべてのユーザーが、カスタムフォームを表示してプロパティを編集できます。

   * **システム内のすべてのユーザーが**&#x200B;を表示できます

     カスタムフォームにアクセスできるシステム内の全員が、フィールドを表示できますが、編集することはできません。

   * **招待されたユーザーのみが**&#x200B;にアクセスできます

     リストに追加したユーザーのみにアクセスを制限します。

   ![共有オプション ](assets/share-field-in-designer.png)

1. 「**保存**」をクリックします。

## カスタムフォームが共有されたときにカスタムフィールドおよびウィジェットに継承したアクセス

誰かがグループ、担当業務、チーム、会社、またはビジネスプロファイルでカスタムフォームを共有すると、受信者はフォーム上のカスタムフィールドとウィジェットへの表示アクセス権を継承します。 フォーム上のこれらの項目に対するこのレベルのアクセス権は常に保持されるので、フォームは、作成者の意図に従って受信者に対して機能します。 これは、フォームに対する編集アクセス権を持つ受信者でも同じです。

カスタムフィールドまたはウィジェットへのアクセス権を継承したユーザーを確認し、そのアクセス権を削除できます。

>[!NOTE]
>
>受信者が共有カスタムフォーム上のカスタムフィールドまたはウィジェットへの管理アクセス権を持っている場合、そのアクセス権は受信者に対して保持されます。

### カスタムフィールドまたはウィジェットへのアクセス権を継承したユーザーを確認する {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

{{step-1-to-setup}}

1. 左側のパネルで、「**カスタムフォーム**」をクリックします。
1. 「**フィールド**」をクリックし、フィールド、画像またはアクセスウィジェットを選択します。
1. 表示されるボックスで、「**継承した権限**」をクリックし、表示される名前を確認します。
1. 「**キャンセル**」をクリックします。

### 共有されたカスタムフォーム内のカスタムフィールドまたはウィジェットへのアクセスを削除する {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

共有されたカスタムフォーム内のカスタムフィールドまたはウィジェットへのアクセスを削除する必要がある場合は、フォームの共有を解除する必要があります。 手順については、[ カスタムフォームの共有](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)の記事[ カスタムフォームへのアクセスの削除](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#remove-access-to-a-custom-form)の節を参照してください。
