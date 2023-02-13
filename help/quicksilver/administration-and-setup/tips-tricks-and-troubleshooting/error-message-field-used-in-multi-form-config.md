---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration
navigation-topic: tips-tricks-troubleshooting-setup-admin
title: '''エラーメッセージ：問題が少しあります。 このフィールドは複数形式の設定で使用されます。'
description: カスタムフォームの計算カスタムフィールドの計算を変更し、エラーメッセージが表示されて、そのフィールドが複数フォーム設定で使用されていることがわかります。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 43668525-5572-4d82-8eed-0e320249f296
source-git-commit: c2bf6441e4ac8520a56d4005b3e87c48370dc065
workflow-type: tm+mt
source-wordcount: '1222'
ht-degree: 0%

---

# エラーメッセージ：問題が少しあります。 このフィールドは、マルチフォーム設定で使用されます

## 問題

カスタムフォームの計算カスタムフィールドの計算を変更する場合、 [!DNL Adobe Workfront] に次の警告が表示される場合があります。

若干の問題があります

[フィールド] を複数フォーム設定で使用する場合、この数式を変更するには、このフィールドを削除し、必要な計算を含む新しいフィールドに置き換える必要があります。

## 原因

変更しようとしている計算済みカスタムフィールドを含む 2 つ以上のカスタムフォームが、 [!DNL Workfront] インスタンス。

**例：** カスタムフォーム A と B はどちらも同じタスクに添付されます。 両方のフォームには、Profit という計算済みのカスタムフィールドが含まれています。 カスタムフォーム A の [ 利益 ] フィールドで計算を編集しようとすると、エラーが発生します。

一方のフォームのカスタムフィールドの計算式は、他方のフォームの同じフィールドの数式と競合するので、変更できません。
この競合を解決するには、同じ計算済みカスタムフィールドを持つ複数のフォームが添付されているオブジェクトを探し、次のいずれかの操作を行う必要があります。

* オブジェクトからフォームの 1 つを削除します。
* 必要に応じて計算を変更しますが、オブジェクトに添付されているすべてのカスタムフォームで変更します。
* オブジェクトに関連付けられているすべてのカスタムフォームで、必要な計算を含む新しい計算済みカスタムフィールドを追加し、古い計算済みカスタムフィールドを古い計算済みカスタムフィールドとしてマークします。

この記事では、オブジェクトを見つけて、問題を解決する方法を次の 3 つの方法のいずれかで説明します。

## カスタムフォームが添付されるオブジェクトを見つけます。 {#find-the-object-where-the-custom-forms-are-attached}

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![](assets/main-menu-icon.png) 右上隅に [!DNL Adobe Workfront]を選択し、「 **[!UICONTROL ユーザー]** ![](assets/users-icon-in-main-menu.png).

1. クリック **[!UICONTROL カスタムForms]** > **[!UICONTROL フィールド]**.
1. を適用します。 **[!UICONTROL フィールドリスト]** 変更しようとしている計算フィールドを表示し、そのフィールドが使用されるすべてのカスタムフォーム（フォーム 1、フォーム 2、フォーム 3 など）をメモします。
1. クリック **[!UICONTROL Forms]**&#x200B;を選択し、 **[!UICONTROL フォームリスト]** 表示
1. 次をクリック： **[!UICONTROL フィルター]** ドロップダウンリストから、 **[!UICONTROL 新しいフィルター]**.

1. クリック **[!UICONTROL フィルタールールを追加]**「custom form name」と入力し、リストに表示されたらこの値を選択します。
1. 選択 **[!UICONTROL 次と等しい]** フィルター修飾子に対して、手順 1 でメモした各フォームの名前を入力し、表示されたら選択します。

   **例：** カスタムフォーム名がフォーム 1、フォーム 2、フォーム 3 と等しい。

1. クリック **[!UICONTROL フィルターを保存]**&#x200B;次に、新しいフィルターに名前を付け、 **[!UICONTROL フィルターを保存]**.

1. フォームの一覧で、フィルターのオブジェクトの種類（Task や Issue など）をメモしておき、 **[!UICONTROL タイプ]** 列。
1. 手順 1 で見つかった各カスタムフォームで、新しいチェックボックスカスタムフィールドを作成し、デフォルト値を「はい」のみにします。

   **例：** フォーム 1 のフィールド 1 =はい、フォーム 2 のフィールド 2 =はい、フォーム 3 のフィールド 3 =はい。 つまり、「計算済みカスタムフィールドがフォーム 1 に存在する」または「計算済みカスタムフィールドがフォーム 2 に存在する」などという意味です。

1. 内 **[!UICONTROL 検索アイコン]** ![](assets/search-icon.png) 画面の右上隅にある **[!UICONTROL 詳細検索]**.
1. カスタムフォームのオブジェクト（「問題」など）をクリックし、 **[!UICONTROL 結果のフィルター]**&#x200B;を選択し、「 **[!UICONTROL フィルターの追加]**.
1. チェックボックスフィールドの名前を **[!UICONTROL フィールド名の入力を開始]** フィールドを選択し、リストに表示されたら選択して、 **[!UICONTROL 次と等しい]** と入力します。 **[!UICONTROL はい]** （引用符なし）を次のボックスに入力します。

   **例：** フィールド 1 が等しい（大文字と小文字を区別）はい。

1. クリック **[!UICONTROL フィルターの追加]** 「チェックボックス」フィールドをすべて詳細検索に追加します。

   可能な組み合わせをすべて探します。

   **例：** 次に示すように、見つけた組み合わせで複数のフィルターを作成します。 同じ計算フィールドを含む、添付された複数のカスタムフォームを持つオブジェクトが必要です。 次のシナリオが考えられます。

   * フィールド 1=はい+フィールド 2=はい+フィールド 3=はい（例：オブジェクトなし）
   * フィールド 1=はい+フィールド 2=はい（例：オブジェクトなし）
   * フィールド 1=はい+フィールド 3=はい（例：2 つのオブジェクト）

   つまり、対応するチェックボックスフィールド（フィールド 1 とフィールド 3）がこれらのオブジェクト上に存在するので、計算済みフィールドはフォーム 1 とフォーム 3 の両方に存在します。

   フィールド 2 =はい+フィールド 3 =はい（例：オブジェクトなし）

1. この記事では、次のセクションのいずれかに進みます。

   * [オブジェクトからカスタムフォームを 1 つ削除し、そこで計算を編集します](#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there)
   * [添付されたすべてのカスタムフォームで、計算内で同じ編集を行う](#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms)
   * [編集した計算を含む新しい計算フィールドを、添付されたカスタムフォームの 1 つまたはすべてに追加します](#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms)

## オブジェクトからカスタムフォームを 1 つ削除し、そこで計算を編集します {#remove-one-of-the-custom-forms-from-the-object-and-edit-the-calculation-there}

1. カスタムフォームが添付されるオブジェクトを見つけます。詳しくは、 [カスタムフォームが添付されるオブジェクトを見つけます。](#find-the-object-where-the-custom-forms-are-attached) この記事で、オブジェクトを開きます。
1. オブジェクトからいずれかのカスタムフォームを削除し、オブジェクトを保存します。

   >[!NOTE]
   >
   >オブジェクトから削除したフォームからフィールドを追加するには、オブジェクトに添付されたままのカスタムフォームを編集する必要がある場合があります。 この方法で、オブジェクト上のカスタムデータ情報を保持できます。

1. 削除したカスタムフォームで、最初に更新しようとしたカスタムフィールドの計算を編集し、「 **[!UICONTROL 保存]**.

   今回は [!DNL Workfront] 競合が発生しないようにする必要があります。

1. （オプション）カスタムフォームからチェックボックスフィールドを削除するか、 [!DNL Workfront].

## 添付されたすべてのカスタムフォームで、計算内で同じ編集を行う {#make-identical-edits-in-the-calculation-in-all-of-the-attached-custom-forms}

>[!IMPORTANT]
>
>これらの手順に従うと、カスタムフォームが既に添付されているオブジェクト内のデータが失われます。 ただし、計算フィールドではなく静的フィールドを参照する場合は、 [!UICONTROL カスタム式の再計算] 失われたデータを復元するオブジェクトのオプション

1. カスタムフォームが添付されるオブジェクトを見つけます。詳しくは、 [カスタムフォームが添付されるオブジェクトを見つけます。](#find-the-object-where-the-custom-forms-are-attached) 」を参照してください。
1. オブジェクトに添付されているすべてのカスタムフォームからフィールドを削除し、フォームを保存します。

1. 新しい計算を含むカスタムフィールドをカスタムフォームに戻します。

   >[!IMPORTANT]
   >
   >すべての添付されたカスタムフォームで、計算方法が同じである必要があります。

1. （オプション）フォームからチェックボックスフィールドを削除するか、 [!DNL Workfront].

## 編集した計算を含む新しい計算フィールドを、添付されたカスタムフォームの 1 つまたはすべてに追加します {#add-a-new-calculated-field-containing-the-edited-calculation-to-one-or-all-of-the-attached-custom-forms}

既存の計算済みカスタムフィールドのデータが失われないようにするか、または見つけたオブジェクトに添付されたカスタムフォームの 1 つで編集済みの計算が必要な場合は、次の手順に従います。

1. カスタムフォームが添付されるオブジェクトを見つけます。詳しくは、 [カスタムフォームが添付されるオブジェクトを見つけます。](#find-the-object-where-the-custom-forms-are-attached) 」を参照してください。
1. 1 つまたはすべてのフォームに必要な計算を含む新しい計算カスタムフィールドを追加します。
1. 古い計算済みカスタムフィールドの名前を変更 **廃止**.

   オブジェクトに添付されたすべてのフォーム上で、古い計算済みのカスタムフォームの履歴データは保持されますが、ユーザーは使用を停止します。

   >[!IMPORTANT]
   >
   >古いフィールドは他の計算カスタムフィールドで参照されている場合があるので、名前を変更した後にこれらの計算を更新する必要があります。

1. （オプション）フォームからチェックボックスフィールドを削除するか、Workfrontから削除します。

<!--
<blockquote data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Problem</h2>
<p>You get the following error while editing a calculated Custom Field on a custom form: </p>
<p><em>"<Name of custom field> field is used in a multi-form configuration, if you would like to change this formula you will need to remove this field and replace it with a new one containing the desired calculation."</em> </p>
<h2>Cause</h2>
<p>The error occurs because the following setup exists: currently you have at least one object in your system that has multiple custom forms attached. The calculated field you are editing exists on multiple forms attached to these objects.</p>
<p>You cannot have the same calculated field with different calculations on the same object. For this reason, the system does not allow you to make a change which will result in calculations being different.</p>
<p><a href="../../Resources/Images/Admin and setup/Tips, Tricks, and Troubleshooting/Calculated_field_error.png" class="MCXref xref" xrefformat="{para}"><img src="assets/calculated-field-error.png" alt="" width="542" height="272"></a> </p>
<p>For example, you have a task with custom forms A and B attached to it. Both forms contain the same calculated field, Field 1. You encounter this error when you try to edit the calculation for Field 1 on custom form A. </p>
<h2>Solution</h2>
<p>Remove the field from the custom form and replace it with a new one containing the desired calculation.  </p>
<p>To understand what custom forms are attached to objects, you can build a report for those objects and reference the Category Name field in the view of the report.<br>For more information about referencing custom forms in reports, see the "Referencing Custom Forms in a Report View (Column)" section in <a href="../../reports-and-dashboards/reports/creating-and-managing-reports/reference-custom-form-report.md" class="MCXref xref" xrefformat="{para}">Reference a custom form in a report</a>.</p>
<p>To understand what custom form contains a Custom Field, see the "Accessing Custom Forms and Fields" section in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md" class="MCXref xref" xrefformat="{para}">Custom forms overview</a>.</p>
<p>For more information about creating a custom form and adding or removing fields from it, see <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md" class="MCXref xref" xrefformat="{para}">Create or edit a custom form</a>.</p>
</blockquote>
-->
