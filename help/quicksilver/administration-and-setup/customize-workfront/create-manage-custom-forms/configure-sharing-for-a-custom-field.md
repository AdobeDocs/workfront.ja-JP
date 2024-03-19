---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: レガシーフォームビルダーでカスタムフィールドとウィジェットの共有を設定する
description: デフォルトでは、新しいカスタムフィールドまたはウィジェットをカスタムフォームに追加すると、カスタムフォームにアクセスできるシステム内の誰でも、その項目のラベルや名前などのプロパティを編集できます。これを変更するには、共有相手を制御します。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: ae774e73-9798-40d1-a96d-a4511f729e7f
source-git-commit: ccb2b6bb9fa63d29523ff396490f9580ad130bdd
workflow-type: tm+mt
source-wordcount: '1003'
ht-degree: 93%

---

# レガシーフォームビルダーでカスタムフィールドとウィジェットの共有を設定する

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべての顧客に対してプレビュー環境でのみ使用できるか、または迅速リリースを有効にした顧客の実稼動環境でのみ使用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

<span class="preview">現在のリリースについて詳しくは、 [2024 年第 2 四半期リリースの概要](/help/quicksilver/product-announcements/product-releases/24-q2-release-activity/24-q2-release-overview.md).</span>

デフォルトでは、新しいカスタムフィールドまたはウィジェットをカスタムフォームに追加すると、カスタムフォームにアクセスできるシステム内の誰でも、その項目のラベルや名前などのプロパティを編集できます。これを変更するには、共有相手を制御します。

カスタムフォームのカスタムフィールドとカスタムウィジェットについて詳しくは、[レガシーフォームビルダーを使用してカスタムフォームにカスタムフィールドを追加](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-a-custom-field-to-a-custom-form.md)および[レガシーフォームビルダーを使用してカスタムフォームでアセットウィジェットを追加または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-widget-or-edit-its-properties-in-a-custom-form.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront プラン</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td>
   <p>新規：標準</p>
   <p>または</p>
   <p>現在：プラン</p></td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>カスタムフォームへの管理アクセス権</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## カスタムフィールドまたはウィジェットの共有を設定する

{{step-1-to-setup}}

1. 左側のパネルで、「**カスタムフォーム**」をクリックします。
1. 組織の Workfront インスタンスのカスタムフィールドまたはウィジェットの共有を設定する場合は、以下の手順を実行します。

   1. クリック **フィールド** をクリックして、「フィールド」領域を開きます。
   1. 共有を設定する項目を選択し、「 **共有** <span class="preview">または ![共有アイコン](assets/share-icon.png).</span>

   または、既存のカスタムフォームのカスタムフィールドまたはウィジェットの共有を設定する場合は、次の手順を実行します。

   1. カスタムフォームを選択し、「 **編集** <span class="preview">または ![編集アイコン](assets/edit-icon.png).</span>
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
