---
title: カスタムフィールドとウィジェットの共有の設定
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
description: デフォルトでは、新しいカスタムフィールドまたはウィジェットをカスタムフォームに追加すると、カスタムフォームにアクセスできるシステム内の誰もが、その項目のラベルやAPI名などのプロパティを編集できます。 これを変更するには、共有相手を制御します。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: 4f591fa3-2cb9-4a22-bfb1-1b50cedfcf3d
TQID: 'https://experienceleague.adobe.com/KyrIWEpIQQb-f8YODUPz3-RbP5wFww8Vu7Ffy33wUog'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: d5896d07-2812-5418-8b18-8957a0d7f0fb
    internal-label: System Setup and Administration
subfeature_v2:
  - id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
    internal-label: Custom forms
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
    internal-label: Admin
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: ecee8b1aadd804a45ff0830e04e77981a3269cff
workflow-type: tm+mt
source-wordcount: '746'
ht-degree: 39%
---
# カスタムフィールドとウィジェットの共有の設定

デフォルトでは、新しいカスタムフィールドまたはウィジェットをカスタムフォームに追加すると、カスタムフォームにアクセスできるシステム内の誰もが、その項目のラベルやAPI名などのプロパティを編集できます。 これを変更するには、共有相手を制御します。

カスタムフォームのカスタムフィールドとウィジェットについて詳しくは、[&#x200B; カスタムフォームの作成](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)を参照してください。

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

## カスタムフィールドまたはウィジェットの共有の設定

{{step-1-to-setup}}

1. 左側のパネルで、「**カスタムフォーム**」をクリックします。
1. フォームとフィールドのリストから共有するには：

   1. 「**フィールド**」をクリックしてフィールドエリアを開きます。
   1. 共有するフィールドを選択し、![共有アイコン &#x200B;](assets/share-icon.png)をクリックします。

1. フォームデザイナーから共有するには：
   1. カスタムフォームを開くか、新しいカスタムフォームを作成します。
   1. フォームデザイナーで、共有するフィールドを選択し、右側のフィールド編集領域で「**共有**」をクリックします。

1. 共有ボックスの&#x200B;**フィールドに**&#x200B;へのアクセス権を付与の下で、アイテムを共有するユーザー、チーム、担当業務、グループ、会社、またはビジネスプロファイルの名前の入力を開始し、名前が表示されたら&#x200B;**Enter**&#x200B;を押します。
1. アイテムの共有方法をより具体的に説明する場合は、名前の右側にあるドロップダウンメニューをクリックし、次のいずれかのオプションを使用します。

   * **表示**: **詳細設定** アイコン ![詳細設定アイコン &#x200B;](assets/configure-options-icon.png)をクリックして、ユーザーがカスタムフォームに項目を追加するか、他のユーザーと共有するかを指定します。
   * **管理**: カスタムフィールドを編集し、フィールドライブラリとフォームデザイナーの両方で表示するためのアクセスを許可します。 **詳細設定** アイコン ![詳細設定アイコン &#x200B;](assets/configure-options-icon.png)をクリックして、ユーザーがシステムから項目を削除するか、他のユーザーと共有するかを指定します。

1. （オプション）手順5 ～ 6を繰り返して、他の名前をリストに追加し、そのオプションを設定します。
1. （オプション）フィールドのシステム全体の共有オプションを選択します。

   * **システム内のすべてのユーザーが**&#x200B;を編集できます（デフォルトのオプション）

     カスタムフィールドまたはウィジェットを追加し、共有を制限しない場合、カスタムフォームにアクセスできるシステム内のすべてのユーザーが、カスタムフォームを表示してプロパティを編集できます。

   * **システム内のすべてのユーザーが**&#x200B;を表示できます

     カスタムフォームにアクセスできるシステム内の全員が、フィールドを表示できますが、編集することはできません。

   * **招待されたユーザーのみが**&#x200B;にアクセスできます

     リストに追加したユーザーのみにアクセスを制限します。

   ![共有オプション &#x200B;](assets/share-field-in-designer.png)

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

共有されたカスタムフォーム内のカスタムフィールドまたはウィジェットへのアクセスを削除する必要がある場合は、フォームの共有を解除する必要があります。 手順については、[&#x200B; カスタムフォームの共有](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)の記事[&#x200B; カスタムフォームへのアクセスの削除](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md#remove-access-to-a-custom-form)の節を参照してください。


