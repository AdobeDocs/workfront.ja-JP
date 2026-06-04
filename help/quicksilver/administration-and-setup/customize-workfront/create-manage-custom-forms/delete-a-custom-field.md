---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: システムからカスタムフィールドまたはウィジェットを削除する
description: システムのパフォーマンスを向上させ、ユーザーにとってフォームを使いやすくするには、カスタムフィールドとウィジェットが使用されなくなった場合、システムからカスタムフィールドとウィジェットを削除します。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c22a7ced-da81-40b5-bb4d-69d59b855add
TQID: https://experienceleague.adobe.com/ArUsDbsxOsdzpdmBGFxs0PcRqBG3HstsZmde--rkQbA
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2: id: d87de1f9-8e24-4c4d-aa4c-a403075091a1
role_v2: id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2: id: aa2f3246-cb95-4b30-8899-fdf7d73550ccid: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 557
ht-degree: 93%

---

# システムからカスタムフィールドまたはウィジェットを削除

システムのパフォーマンスを向上させ、ユーザーにとってフォームを使いやすくするには、カスタムフィールドとウィジェットが使用されなくなった場合、システムからカスタムフィールドとウィジェットを削除します。

>[!CAUTION]
>
>また、カスタムフィールドを削除すると、オブジェクトに添付されたカスタムフォームに入力したユーザーがフィールドに入力したすべてのカスタムデータも削除されます。 削除されたデータは復元できません。 また、そのカスタムフォームを使用しているユーザーに対して、削除されたことを警告する通知システムはありません。
>
>削除するカスタムフィールドを使用するすべてのカスタムフォームおよびレポートを表示して、その影響を評価できます。 詳しくは、[特定のカスタムフィールドまたはウィジェットを使用するすべてのカスタムフォームの表示](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md)および[特定のカスタムフィールドまたはウィジェットを使用するすべてのレポートの表示](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-reports-that-use-a-particular-custom-field.md)を参照してください。
>
>また、使用されなくなったフィールドのデータの損失を防ぐために使用できる回避策について詳しくは、[ユーザーが入力したデータ損失なしでのカスタムフィールドの削除](#remove-a-custom-field-without-losing-data-that-users-have-entered)を参照してください。

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

## システムからカスタムフィールドまたはウィジェットを削除

{{step-1-to-setup}}

1. 「**カスタムフォーム**」をクリックします。
1. 「**フィールド**」をクリックして、フィールドエリアを開きます。
1. カスタムフィールドまたはウィジェットを選択し、「**削除**」をクリックします。
1. アイテムを完全に削除し、（カスタムフィールドの場合は）そのアイテムが添付されたオブジェクトに関連するすべてのデータを削除する場合は、「**はい、削除します**」をクリックします。

## ユーザーが入力したデータの損失なしでのカスタムフィールドの削除 {#remove-a-custom-field-without-losing-data-that-users-have-entered}

>[!CAUTION]
>
>500 個を超えるフィールドとウィジェットを持つカスタムフォームからのカスタムフィールドの削除は元に戻すことができません。 このフィールドを削除すると、フォームに含まれるフィールドとウィジェットの数が 500 個未満になるまで、再度追加することはできません。

1. 元のカスタムフォームから削除するカスタムフィールドを決定しますが、この時点では削除しないでください。
1. 新規カスタムフォームを作成するには、次の手順に従います。

   1. 元のカスタムフォームから削除する新しいフォームにカスタムフィールドを追加します。

      詳しくは、[ カスタムフォームの作成](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md)の「[ カスタムフォームに新規または既存のフィールドを追加](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-new-or-existing-fields-to-your-custom-form)」の節を参照してください。

   1. 新規カスタムフォームを保存します。

1. [カスタムフォームの共有](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)の説明に従って、カスタムフォームへのアクセスを管理者アクセス権を持つユーザーのみに制限します。
1. [オブジェクトにカスタムフォームを追加する](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)の説明に従って、元のカスタムフォームが既に適用されているオブジェクトに新規カスタムフォームを適用します。

   新規カスタムフォームをこれらのオブジェクトに適用することで、履歴レポートデータに影響を与えることはありません。

1. 元のカスタムフォームを変更し、新規フォームに追加したカスタムフィールドを削除します（手順 2）。

   元のカスタムフォームから削除したフィールドは、作成した新規カスタムフォームでのみ使用できるようになりました。 ユーザーはオブジェクト上のカスタムフォームを表示できますが、管理者アクセス権を持たないユーザーはカスタムフォームを変更できません。
