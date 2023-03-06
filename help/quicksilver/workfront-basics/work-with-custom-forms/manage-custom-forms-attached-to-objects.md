---
product-area: projects;user-management
navigation-topic: work-with-custom-forms
title: オブジェクトに添付されたカスタムフォームの管理
description: 1 つのオブジェクトに添付されたカスタムフォームの表示順を更新したり、それらを削除したり、複数のオブジェクトでのカスタムフォームの表示方法を一括編集したりできます。
author: Alina
feature: Get Started with Workfront
exl-id: e5570a09-32cb-43e3-9c1d-4421db42fa24
source-git-commit: 78de23b4d5814e5e2ead6bb61a80bba7bd2aed33
workflow-type: tm+mt
source-wordcount: '1080'
ht-degree: 0%

---

# オブジェクトに添付されたカスタムフォームの管理

<!--
<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span>  -->

1 つのオブジェクトに添付されたカスタムフォームの表示順を更新したり、それらを削除したり、複数のオブジェクトでのカスタムフォームの表示方法を一括編集したりできます。

## アクセス要件

この記事で説明する操作を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>カスタムフォームを管理するオブジェクトへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>カスタムフォームを管理するオブジェクトに対する権限以上の貢献</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

* Workfront管理者またはカスタムフォームへの管理者アクセス権を持つプランユーザーは、環境内でカスタムフォームを作成する必要があります。 詳しくは、 [カスタムフォームの作成または編集](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
* オブジェクトには、カスタムフォームを添付する必要があります。

   オブジェクトにカスタムフォームを適用する方法について詳しくは、 [オブジェクトへのカスタムフォームの追加](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## オブジェクトに添付された複数のカスタムフォームの並べ替え {#reorder-multiple-custom-forms-attached-to-an-object}

1. 追加したカスタムフォームの順序を変更するオブジェクトに移動し、オブジェクトの編集を開始します。

   **例：** 例えば、プロジェクトのカスタムフォームを管理するには、プロジェクトに移動し、 **詳細** メニュー ![](assets/more-icon.png)を選択し、「 **編集** .

1. 内 **カスタムForms** [ プロジェクト、タスク、およびタスク ] セクションで、 ![](assets/move-icon---dots.png) カスタムフォーム名の横にあるアイコン。 その他のすべてのオブジェクトに対して、 **Formsを管理**. このオプションは、少なくとも 1 つのカスタムフォームがオブジェクトに添付されている場合にのみ表示されます。
1. フォームをドラッグ ![](assets/move-icon---dots.png) をリストの新しい場所に追加します。
1. プロジェクト、タスクおよび問題のカスタムフォームの場合は、 **保存**.

   その他のすべてのオブジェクトに対して、 **管理は終わった** > **変更を保存**.

## オブジェクトからカスタムフォームを削除する {#remove-a-custom-form-from-an-object}

>[!IMPORTANT]
>
>オブジェクトからカスタムフォームを削除すると、フォームのカスタムフィールドに取り込まれたすべての情報が失われ、復元できなくなります。

1. カスタムフォームを削除するオブジェクトに移動し、オブジェクトの編集を開始します。

   例えば、プロジェクトに移動し、 **詳細** メニュー ![](assets/more-icon.png)を選択し、「 **編集** .

1. クリック **カスタムForms**.
1. プロジェクト、タスクおよび問題のカスタムフォームの場合、 **X** アイコンを使用してフォームをオブジェクトから削除します。

   その他のすべてのオブジェクトに対して、 **Formsを管理**」、「 **X** アイコンを使用してフォームをオブジェクトから削除します。

1. 「**保存**」をクリックします。

## 同じカスタムフィールドを含む複数のカスタムフォームの管理

同じオブジェクトに添付された複数のカスタムフォームで、同じフィールドが表示される場合があります。 この場合、次の点に注意してください。

* フィールドの値は、すべてのフォームで同じです。

   同じオブジェクトにアタッチされた異なるフォーム上の同じフィールドに異なる値を設定することはできません。

* 2 つの異なるオブジェクトに同じ計算フィールドがある場合、エラーを避けるために、計算方法が同じである必要があります。 複数のフォームを含むカスタムフォームへの計算フィールドの追加について詳しくは、 [計算データをカスタムフォームに追加する](../../administration-and-setup/customize-workfront/create-manage-custom-forms/add-calculated-data-to-custom-form.md) .

## オブジェクトの一括編集時に複数のカスタムフォームを管理する

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:

>[!NOTE]
>
><span class="preview">For information about managing custom forms on projects in bulk in the Preview environment, see the article [Edit projects](../../manage-work/projects/manage-projects/edit-projects.md)</span>.

-->

複数のカスタムフォームが適用されたオブジェクトを一括編集する場合は、それらのオブジェクトに対するカスタムフォームの表示方法を編集したり、カスタムフォーム間の共通フィールドを編集したりできます。

一括編集で編集できるのは、選択したすべてのオブジェクトに添付されているカスタムフォームだけです。

オブジェクトを一括編集する際に複数のカスタムフォームを編集するには：

1. リストオブジェクトで、カスタムフォームが添付されるオブジェクトを選択し、 **編集** アイコン ![](assets/edit-icon.png).
1. クリック **カスタムForms**.

   選択したすべてのオブジェクトに添付されているカスタムフォームのみを編集できます。

   一部のオブジェクトにのみ添付されたカスタムフォームは表示されません。

1. カスタムフォームのフィールドの編集を開始します。

   フィールドが編集されると、フィールドに視覚的なインジケーターが表示され、フィールドが編集されたことが示されます。

   1 つのフィールドが複数のカスタムフォームに含まれている場合、いずれかのフォームでフィールドを更新すると、それらのフィールドのすべての値が各フォームで更新されます。

1. 次をクリック： **選択を行う** ドロップダウンメニューから追加フォームを選択し、選択したすべてのオブジェクトに追加します。

   追加のフォームを適用する際は、以下の点を考慮してください。

   * オブジェクトには、最大 10 個のカスタムフォームを含めることができます。
   * フォームを適用できるのは、編集中のオブジェクトにフォームがまだ適用されていない場合のみです。 オブジェクトの 1 つに既に添付されているフォームは、ドロップダウンメニューに表示されません。
   * 追加のフォームを適用すると、フォームが他のフォームと共通するフィールドは、 **共通のフィールド** セクションで参照し、編集できます。

1. （オプション）すべてのオブジェクトにカスタムフォームを追加したが、オブジェクトをまだ保存していない場合は、オブジェクトに表示するカスタムフォームの順序を変更できます。

   フォームの順序の変更について詳しくは、 [オブジェクトに添付された複数のカスタムフォームの並べ替え](#reorder-multiple-custom-forms-attached-to-an-object) 」を参照してください。

1. クリック **フォームを削除** をクリックして、オブジェクトからカスタムフォームを削除します。

   オブジェクトからカスタムフォームを削除する方法について詳しくは、 [オブジェクトからカスタムフォームを削除する](#remove-a-custom-form-from-an-object).

   複数のオブジェクトから一括でフォームを削除する場合は、次の点を考慮してください。

   * フォームに変更を加えている場合は、削除すると変更内容が失われ、復元できなくなります。
   * フォームを削除すると、そのフォームから **共通のフィールド** セクションはこのセクションから削除され、ここでは編集できなくなりました。

1. クリック **フォームを復元** フォームを編集前の状態に戻す場合。
1. （オプション）フォーム名の横にある折りたたみ矢印をクリックして、一度に 1 つのフォームを折りたたみます。

   または

   クリック **折りたたみForms** をクリックして、すべてのフォームを同時に折りたたみます。

1. （オプション）フォーム名の横にある展開矢印をクリックして、一度に 1 つのフォームを展開します。

   または

   クリック **Formsを展開** をクリックして、すべてのフォームを同時に展開します。 

1. クリック **変更を保存**.
