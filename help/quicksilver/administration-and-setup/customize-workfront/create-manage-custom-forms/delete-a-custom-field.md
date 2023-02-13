---
user-type: administrator
product-area: system-administration
navigation-topic: create-and-manage-custom-forms
title: システムからカスタムフィールドまたはウィジェットを削除する
description: システムのパフォーマンスを向上させ、フォームをユーザーが使いやすくするために、カスタムフィールドとウィジェットが使用されなくなったときに、システムからカスタムフィールドとウィジェットを削除することができます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: c22a7ced-da81-40b5-bb4d-69d59b855add
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '576'
ht-degree: 0%

---

# システムからカスタムフィールドまたはウィジェットを削除する

システムのパフォーマンスを向上させ、フォームをユーザーが使いやすくするために、カスタムフィールドとウィジェットが使用されなくなったときに、システムからカスタムフィールドとウィジェットを削除することができます。

>[!CAUTION]
>
>また、カスタムフィールドを削除すると、オブジェクトに添付されたカスタムフォームに入力したユーザーがフィールドに入力したすべてのカスタムデータも削除されます。 その削除されたデータは復元できません。
>
>削除するカスタムフィールドを使用するすべてのカスタムフォームおよびレポートを表示して、その影響を評価できます。 詳しくは、 [特定のカスタムフィールドまたはウィジェットを使用するすべてのカスタムフォームを表示する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-custom-forms-that-use-a-particular-custom-field.md) および [特定のカスタムフィールドまたはウィジェットを使用するすべてのレポートを表示する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/view-all-reports-that-use-a-particular-custom-field.md).
>
>また、使用されなくなったフィールドのデータの損失を防ぐために使用できる回避策については、 [ユーザーが入力したデータが失われることなく、カスタムフィールドを削除します](#remove-a-custom-field-without-losing-data-that-users-have-entered) 」を参照してください。

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td>計画</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>カスタムフォームへの管理アクセス</p> <p>Workfront管理者がこのアクセス権を付与する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref">特定の領域に対する管理者アクセス権をユーザーに付与する</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスタイプ、アクセスレベル設定を確認するには、Workfront管理者に問い合わせてください。

## システムからカスタムフィールドまたはウィジェットを削除する

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **カスタムForms。**
1. 次をクリック： **フィールド** タブをクリックします。
1. カスタムフィールドまたはウィジェットを選択し、 **削除**.
1. アイテムを完全に削除し、（カスタムフィールドの場合は）そのアイテムが添付されたオブジェクトに関連するすべてのデータを削除する場合は、 **はい、削除します**.

## ユーザーが入力したデータが失われることなく、カスタムフィールドを削除します {#remove-a-custom-field-without-losing-data-that-users-have-entered}

>[!CAUTION]
>
>500 個を超えるフィールドとウィジェットを持つカスタムフォームからのカスタムフィールドの削除は元に戻すことができません。 このフィールドを削除すると、フォームに含まれるフィールドとウィジェットの数が 500 個未満になるまで、再度追加することはできません。

1. 元のカスタムフォームから削除するカスタムフィールドを決定しますが、この時点では削除しないでください。
1. 新しいカスタムフォームを作成します。 [カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

   1. 元のカスタムフォームから削除する新しいフォームにカスタムフィールドを追加します。詳しくは、 [カスタムフォームでカスタムフィールドまたはウィジェットを再利用する](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/reuse-an-existing-field.md).
   1. 新しいカスタムフォームを保存します。

1. カスタムフォームへのアクセスを、管理者アクセス権を持つユーザーのみに制限します。詳しくは、 [カスタムフォームの共有](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md).
1. 元のカスタムフォームが既に適用されているオブジェクトに新しいカスタムフォームを適用します。詳しくは、 [オブジェクトへのカスタムフォームの追加](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

   新しいカスタムフォームをこれらのオブジェクトに適用すると、履歴レポートデータに影響を与えません。

1. 元のカスタムフォームを変更し、新しいフォームに追加したカスタムフィールドを削除します（手順 2）。

   元のカスタムフォームから削除したフィールドは、作成した新しいカスタムフォームでのみ使用できるようになりました。 ユーザーはオブジェクト上のカスタムフォームを表示できますが、管理者アクセス権を持たないユーザーはカスタムフォームを変更できません。
