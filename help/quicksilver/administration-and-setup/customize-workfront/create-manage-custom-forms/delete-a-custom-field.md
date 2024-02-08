---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: システムからカスタムフィールドまたはウィジェットを削除
description: システムのパフォーマンスを向上させ、ユーザーにとってフォームを使いやすくするには、カスタムフィールドとウィジェットが使用されなくなった場合、システムからカスタムフィールドとウィジェットを削除します。
author: Lisa
feature: System Setup and Administration, Custom Forms
role: Admin
exl-id: c22a7ced-da81-40b5-bb4d-69d59b855add
source-git-commit: 35de4535970d5cd15fcd68f79bf849803f94a77e
workflow-type: tm+mt
source-wordcount: '566'
ht-degree: 95%

---

# システムからカスタムフィールドまたはウィジェットを削除

システムのパフォーマンスを向上させ、ユーザーにとってフォームを使いやすくするには、カスタムフィールドとウィジェットが使用されなくなった場合、システムからカスタムフィールドとウィジェットを削除します。

>[!CAUTION]
>
>また、カスタムフィールドを削除すると、オブジェクトに添付されたカスタムフォームに入力したユーザーがフィールドに入力したすべてのカスタムデータも削除されます。その削除されたデータは復元できません。
>
>削除するカスタムフィールドを使用するすべてのカスタムフォームおよびレポートを表示して、その影響を評価できます。詳しくは、[特定のカスタムフィールドまたはウィジェットを使用するすべてのカスタムフォームの表示](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md)および[特定のカスタムフィールドまたはウィジェットを使用するすべてのレポートの表示](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-reports-that-use-a-particular-custom-field.md)を参照してください。
>
>また、使用されなくなったフィールドのデータの損失を防ぐために使用できる回避策について詳しくは、[ユーザーが入力したデータ損失なしでのカスタムフィールドの削除](#remove-a-custom-field-without-losing-data-that-users-have-entered)を参照してください。

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

## システムからカスタムフィールドまたはウィジェットを削除

{{step-1-to-setup}}

1. 「**カスタムフォーム**」をクリックします。
1. クリック **フィールド** をクリックして、「フィールド」領域を開きます。
1. カスタムフィールドまたはウィジェットを選択し、「**削除**」をクリックします。
1. アイテムを完全に削除し、（カスタムフィールドの場合は）そのアイテムが添付されたオブジェクトに関連するすべてのデータを削除する場合は、「**はい、削除します**」をクリックします。

## ユーザーが入力したデータの損失なしでのカスタムフィールドの削除 {#remove-a-custom-field-without-losing-data-that-users-have-entered}

>[!CAUTION]
>
>500 個を超えるフィールドとウィジェットを持つカスタムフォームからのカスタムフィールドの削除は元に戻すことができません。このフィールドを削除すると、フォームに含まれるフィールドとウィジェットの数が 500 個未満になるまで、再度追加することはできません。

1. 元のカスタムフォームから削除するカスタムフィールドを決定しますが、この時点では削除しないでください。
1. 新規カスタムフォームを作成するには、次の手順に従います。

   1. 元のカスタムフォームから削除する新しいフォームにカスタムフィールドを追加します。

      * カスタムフォームビルダーを使用している場合は、[カスタムフォームでのカスタムフィールドまたはウィジェットの再利用](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md)を参照してください。
      * フォームデザイナーを使用している場合は、[新規または既存のフィールドのカスタムフォームへの追加](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md#add-new-or-existing-fields-to-your-custom-form)を参照してください。

   1. 新規カスタムフォームを保存します。

1. [カスタムフォームの共有](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md)の説明に従って、カスタムフォームへのアクセスを管理者アクセス権を持つユーザーのみに制限します。
1. [オブジェクトにカスタムフォームを追加する](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)の説明に従って、元のカスタムフォームが既に適用されているオブジェクトに新規カスタムフォームを適用します。

   新規カスタムフォームをこれらのオブジェクトに適用することで、履歴レポートデータに影響を与えることはありません。

1. 元のカスタムフォームを変更し、新規フォームに追加したカスタムフィールドを削除します（手順 2）。

   元のカスタムフォームから削除したフィールドは、作成した新規カスタムフォームでのみ使用できるようになりました。ユーザーはオブジェクト上のカスタムフォームを表示できますが、管理者アクセス権を持たないユーザーはカスタムフォームを変更できません。
