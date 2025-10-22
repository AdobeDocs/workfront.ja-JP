---
product-area: projects;user-management
keywords: 編集,フォーム,リッチ,テキスト,特殊,形式,フィールド,カスタム,情報,カスタマイズ,オブジェクト
navigation-topic: work-with-custom-forms
title: カスタムフォームフィールドの情報を編集する
description: フォームをオブジェクトに添付した後に、カスタムフォームの情報を編集できます。オブジェクトにカスタムフォームを追加する方法について詳しくは、「オブジェクトにカスタムフォームを追加する」を参照してください。
author: Alina
feature: Get Started with Workfront
exl-id: c2b6afde-91a8-4e17-8e1a-3428b48e500a
source-git-commit: 6ded38ef130fbcdde8d680f77f6db38fbd81efb4
workflow-type: tm+mt
source-wordcount: '1039'
ht-degree: 85%

---

# カスタムフォームフィールドの情報を編集する

<!--Audited: 10/2025-->

フォームをオブジェクトに添付した後に、カスタムフォームの情報を編集できます。カスタムフォームをオブジェクトに追加する方法について詳しくは、[オブジェクトにカスタムフォームを追加する](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront パッケージ</p> </td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront プラン</p> </td> 
   <td> <p>投稿者以上</p> 
   <p>リクエスト以上</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>カスタムフォームを編集するオブジェクトへのアクセスを編集します</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>オブジェクト権限</p> </td> 
   <td> 
    <ul> 
     <li> <p>カスタムフォームを編集するオブジェクトに対する参加以上の権限</p> </li> 
     <li><p>編集するフィールドに対する権限を表示します。</p></li> 
     <li><p>編集するフィールドが配置されているフォーム上のセクションに対する権限を編集</p></li> 
    </ul></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>Team or higher</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront licenses*</p> </td> 
   <td> <p>Request or higher</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Access level*</td> 
   <td> <p>Edit access to the object for which you want to edit the custom form</p> <p>Note: If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Object permissions</p> </td> 
   <td> 
    <ul> 
     <li> <p>Contribute or higher permissions on the object for which you want to edit the custom form</p> </li> 
     <li>View permissions on the fields you want to edit. For information about sharing permissions for custom fields, see <a href="/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/manage-a-form/share-custom-fields.md" class="MCXref xref">Configure sharing for custom fields and widgets</a>.</li> 
     <li> <p>Edit permissions for the sections on the form where the fields you want to edit are located</p> </li> 
    </ul> <p>For information on requesting additional access for objects, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 前提条件

* Workfront 管理者またはカスタムフォームへの管理者アクセス権を持つプランユーザーは、環境内でカスタムフォームを作成する必要があります。詳しくは、[&#x200B; カスタムフォームの作成 &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) を参照してください。
* オブジェクトには、カスタムフォームを添付する必要があります。

  カスタムフォームをオブジェクトに追加する方法について詳しくは、[オブジェクトにカスタムフォームを追加する](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md)を参照してください。

## カスタムフォームの情報を編集

オブジェクトに添付されたカスタムフォームに関する情報の編集は、すべてのオブジェクトで同じです。カスタムフォームを持つことのできるオブジェクトについて詳しくは、[カスタムフォームの概要](../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md)を参照してください。

1. カスタムフォームの情報を編集するオブジェクトに移動します。
1. 左パネルで「**`<Object type>`詳細**」をクリックします。

   例えば、プロジェクトのカスタムフォームに関する情報を編集する場合は、「**プロジェクト詳細**」をクリックします。

1. カスタムフォームまでスクロールします。オブジェクトにカスタムフォームが添付されている場合、フォームの名前は「詳細」セクションの領域として表示されます。
1. 必要に応じて、カスタムフォームの名前の左側にある矢印 ![](assets/expand-arrow-right.png) をクリックし展開します。
1. ページの右上隅にある編集アイコン ![](assets/edit-icon.png) をクリックします。
1. アクセス権のある任意のフィールドに情報を入力します。

   ![](assets/click-in-field-to-edit-info-350x132.png)

   または

   フォームに情報がまだ入力されていない場合は、アクセス権がある任意のフィールドで「**追加+**」をクリックし、情報の入力を開始します。

   ![](assets/plus-add-to-edit-info-350x180.png)

   オブジェクトに複数のカスタムフォームが添付されている場合は、各フォームに対してこれを実行できます。

   作業中のフィールドのタイプに応じて、次の点に注意してください。

   * ラジオボタンフィールドに選択できるオプションは 1 つだけです。
   * フォーム作成者がフィールドをどのように設定したかに応じて、チェックボックスフィールドで 1 つまたは複数のオプションを選択できます。
   * フォーム作成者がフィールドをどのように設定したかに応じて、複数選択ドロップダウンフィールドで 1 つまたは複数のオプションを選択できます。
   * テキストフィールド（太字、斜体、下線）の書式を設定できるのは、フォームを作成したユーザーが「書式設定」フィールドタイプのテキストフィールドとして設定した場合のみです。1 行のテキストフィールドと段落テキストフィールドは書式設定できません。
   * 日付フィールドタイプで時刻を更新できるのは、フォームを作成したユーザーがフィールドの作成時に時刻を含めている場合だけです。

   すべてのフィールドタイプについて詳しくは、[&#x200B; カスタムフォームの作成 &#x200B;](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) を参照してください。

1. 「**変更を保存**」をクリックします。

   >[!IMPORTANT]
   >
   >フォームを保存するには、まず、フォーム上のすべての必須フィールドに入力する必要があります。必須フィールドの名前の後には、アスタリスクが付きます。
   >
   >![](assets/nwe-required-custom-field.png)

   オブジェクト内の計算カスタムフィールドで参照される別のオブジェクト内のデータを変更した場合、その変更はオブジェクトに自動的には反映されません。オブジェクト内のすべての計算カスタムフィールドを手動で更新する方法については、[オブジェクトのすべての計算カスタムフィールドを再計算する方法](#recalculate-all-calculated-custom-fields-for-an-object)を参照してください。

   ページ上の依存フィールドを変更すると、カスタムフォームでの計算フィールドがリアルタイムで動的に再計算されます。フォームを保存せずに新しい計算フィールドの値を確認できますが、変更を保存するまで、実際にはフォームとオブジェクトに適用されません。これは、カスタムフォームだけでなくデフォルトフォームでの計算フィールドにも適用されます。

   また、オブジェクトをリスト内の他のオブジェクトと共に一括編集する際に、そのオブジェクトの計算カスタムフィールドをすべて手動で更新することもできます。手順については、この記事の[オブジェクトの編集時にリスト内の複数のオブジェクトの計算カスタムフィールドをすべて再計算する方法](#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects)を参照してください。

## オブジェクトのすべての計算カスタムフィールドを再計算する方法  {#recalculate-all-calculated-custom-fields-for-an-object}

>[!IMPORTANT]
>
>この節の手順を実行するには、計算フィールドを添付したカスタムフォームがオブジェクトに必要です。


1. 再計算するカスタムフィールドがあるオブジェクトのメインページに移動します。
1. オブジェクト名の右にある&#x200B;**その他**&#x200B;メニュー ![](assets/more-icon.png) をクリックし、「**式の再計算**」をクリックします。

   これにより、当該オブジェクトのフォーム上のすべてのカスタムフィールドが再計算されます。

## オブジェクトの編集時にリスト内の複数のオブジェクトの計算カスタムフィールドをすべて再計算する方法 {#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be edited when the bulk edit for objects update in NW)</p>
-->

カスタム式を再計算するオブジェクトに応じて、次の領域で再計算できます。

* オブジェクトのリストで、リスト上部の「その他」メニューから。
* 複数のオブジェクトを一括して選択および編集する場合は、[ 編集 ] ボックスで行います。

リストまたはレポートから複数のオブジェクトのカスタムフィールドを一括編集して、手動で再計算するには：

1. 計算フィールドがあるカスタムフォームを含んだオブジェクトのリストに移動します。
1. 更新する計算カスタムフィールドがあるオブジェクトを選択します。
1. **編集アイコン**&#x200B;をクリックします。
1. 左側のメニューで「**カスタムフォーム**」をクリックし、「**カスタム式の再計算**」を選択します。
1. 「**変更を**&#x200B;**保存**」をクリックします。

   選択したすべてのオブジェクトのすべてのカスタムフィールドが計算されます。

オブジェクトのリストからカスタム式を再計算するには：

1. プロジェクトリストまたはレポートに移動し、1 つまたは複数のプロジェクトを選択します。
1. **その他**&#x200B;メニュー ![](assets/more-icon.png) をクリックし、「**カスタム式の再計算**」をクリックします。

![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)

Workfrontは、選択されたすべてのプロジェクトのすべてのカスタムフィールドを直ちに計算します。
すべてのオブジェクトのすべてのリストにこの機能があるわけではありません。

>[!NOTE]
>
>プロジェクトの複雑さによっては、最適なパフォーマンスを確保するために計算カスタムフィールドを一括で再計算する場合は、多数のプロジェクトを選択しないことをお勧めします。プロジェクトが複雑すぎる原因として考えられるものとしては、複数の依存関係や割り当てまたは多数のカスタムフィールドなどがあります。

