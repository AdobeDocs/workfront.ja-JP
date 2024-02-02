---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: レガシーフォームビルダーでカスタムフィールドとウィジェットの共有を設定する
description: デフォルトでは、新しいカスタムフィールドまたはウィジェットをカスタムフォームに追加すると、カスタムフォームにアクセスできるシステム内の誰でも、その項目のラベルや名前などのプロパティを編集できます。これを変更するには、共有相手を制御します。
author: Caroline
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ae774e73-9798-40d1-a96d-a4511f729e7f
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: ht
source-wordcount: '963'
ht-degree: 100%

---

# レガシーフォームビルダーでカスタムフィールドとウィジェットの共有を設定する

デフォルトでは、新しいカスタムフィールドまたはウィジェットをカスタムフォームに追加すると、カスタムフォームにアクセスできるシステム内の誰でも、その項目のラベルや名前などのプロパティを編集できます。これを変更するには、共有相手を制御します。

カスタムフォームのカスタムフィールドとカスタムウィジェットについて詳しくは、[レガシーフォームビルダーを使用してカスタムフォームにカスタムフィールドを追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)および[レガシーフォームビルダーを使用してカスタムフォームでアセットウィジェットを追加または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront プラン*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td>プラン</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>カスタムフォームへの管理アクセス権</p> <p>Workfront 管理者がこのアクセス権を付与する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定のエリアに対する管理者アクセス権をユーザーに付与</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、ライセンスタイプまたはアクセスレベル設定を確認するには、Workfront 管理者にお問い合わせください。

## カスタムフィールドまたはウィジェットの共有を設定する

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) をクリックして、**設定** ![](assets/gear-icon-settings.png) をクリックします。

1. 左側のパネルで、「**カスタムフォーム**」をクリックします。
1. 組織の Workfront インスタンスのカスタムフィールドまたはウィジェットの共有を設定する場合は、以下の手順を実行します。

   1. 「**フィールド**」タブをクリックします。
   1. 共有を設定する項目を選択し、「**共有**」をクリックします。

   または、既存のカスタムフォームのカスタムフィールドまたはウィジェットの共有を設定する場合は、次の手順を実行します。

   1. カスタムフォームを選択し、「**編集**」をクリックします。
   1. 右側のフォーム編集エリアで、共有を設定する項目を選択します。
   1. 左側のパネルで、「**フィールドを共有**」を選択します。

1. 表示される「**カスタムフィールドアクセス**」ボックスで、アイテムを共有する相手と共有方法を指定します。

   1. 「**カスタムフィールドアクセス**」ボックスの左下隅近くの、「**カスタムフィールドアクセスを許可」**&#x200B;で、項目を共有するユーザー、チーム、担当業務、グループ、または会社の名前の入力を開始し、表示された名前をクリックします。

      ![](assets/share-field-give-access-to.jpg)

   1. 項目の共有方法をより具体的に指定する場合は、名前の右にあるドロップダウンリストをクリックし、次のいずれかのオプションを使用します。

      ![](assets/share-field-view-mng-options.jpg)

      <table style="table-layout:auto"> 
       <col> 
       <col> 
       <tbody> 
        <tr> 
         <td role="rowheader">それを表示</td> 
         <td> <p>「<strong>詳細設定</strong>」をクリックして、ユーザーがアクセス権を使用してアイテムをカスタムフォームに追加したり、他のユーザーと共有したりできるようにするかどうかを指定できます。</p> </td> 
        </tr> 
        <tr> 
         <td role="rowheader">それを管理</td> 
         <td> <p>カスタムフィールドを編集し、フィールドライブラリや、カスタムフォームを作成するページに表示するためのアクセスを許可します。</p> <p>「<strong>詳細設定</strong>」をクリックして、ユーザーがアクセス権を使用してアイテムをシステムから削除したり、他のユーザーと共有したりできるようにするかどうかを指定できます。</p> </td> 
        </tr> 
       </tbody> 
      </table>

1. （オプション）上記の手順を繰り返して、リストに他の名前を追加し、そのオプションを設定します。
1. （オプション）フィールドのシステム全体の共有オプションを選択する場合は、右上隅にある歯車アイコン ![](assets/gear-icon-settings.png) をクリックします。

   このドロップダウンメニューには、以下のすべてのオプションが同時に表示されるわけではありません。例えば、2 番目のものは、他の 2 つのうちの 1 つが選択されている場合にのみ表示されます。

   * **これをシステム全体で編集可能にして、Workfront の全員が編集できるようする**（デフォルトのオプション）

     カスタムフィールドまたはウィジェットを追加し、共有を制限しない場合、カスタムフォームにアクセスできるシステム内のすべてのユーザーが、カスタムフォームを表示してプロパティを編集できます。

   * **システム全体での編集アクセスを削除**

     リストに追加したユーザーのみにアクセスを制限します。

   * **Workfront 内のすべてのユーザーが確認できるようシステム全体で表示する**

1. 「**保存**」または「**保存して閉じる**」をクリックします。

## カスタムフォームが共有されたときにカスタムフィールドおよびウィジェットに継承したアクセス

ユーザーがグループ、担当業務、チーム、または会社とカスタムフォームを共有すると、フォーム上のカスタムフィールドおよびウィジェットへの表示アクセス権を継承します。フォーム上のこれらの項目に対するこのレベルのアクセス権は常に保持されるので、フォームは、作成者の意図に従って受信者に対して機能します。これは、フォームに対する編集アクセス権を持つ受信者でも同じです。

カスタムフィールドまたはウィジェットへのアクセス権を継承したユーザーを確認し、そのアクセス権を削除できます。

>[!NOTE]
>
>受信者が共有カスタムフォーム上のカスタムフィールドまたはウィジェットへの管理アクセス権を持っている場合、そのアクセス権は受信者に対して保持されます。

* [カスタムフィールドまたはウィジェットへのアクセス権を継承したユーザーを確認](#find-out-who-has-inherited-access-to-a-custom-field-or-widget)
* [共有されたカスタムフォーム内のカスタムフィールドまたはウィジェットへのアクセスを削除する](#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared)

### カスタムフィールドまたはウィジェットへのアクセス権を継承したユーザーを確認する {#find-out-who-has-inherited-access-to-a-custom-field-or-widget}

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png) 、**設定** ![](assets/gear-icon-settings.png) の順にクリックします。

1. 左側のパネルで、「**カスタムフォーム**」をクリックします。
1. 「**フィールド**」タブをクリックし、フィールド、画像、またはアクセスウィジェットを選択します。
1. 表示されるボックスで、「**継承した権限**」をクリックし、表示される名前を確認します。
1. 「**キャンセル**」をクリックします。

### 共有されたカスタムフォーム内のカスタムフィールドまたはウィジェットへのアクセスを削除する {#remove-access-to-a-custom-field-or-widget-in-a-custom-form-that-was-shared}

共有されたカスタムフォーム内のカスタムフィールドまたはウィジェットへのアクセスを削除する必要がある場合は、フォームの共有を解除する必要があります。手順については、[カスタムフォームを共有](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)の記事の[カスタムフォームへのアクセスを削除](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#unshare)の節を参照してください。
