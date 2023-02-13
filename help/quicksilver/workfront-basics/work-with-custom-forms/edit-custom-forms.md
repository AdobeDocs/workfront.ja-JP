---
product-area: projects;user-management
keywords: 編集，フォーム，リッチ，テキスト，特殊，書式，フィールド，カスタム，情報，カスタマイズ，オブジェクト
navigation-topic: work-with-custom-forms
title: カスタムフォームフィールドの情報を編集
description: フォームをオブジェクトに添付した後、カスタムフォームの情報を編集できます。 オブジェクトにカスタムフォームを追加する方法については、「オブジェクトにカスタムフォームを追加する」を参照してください。
author: Alina
feature: Get Started with Workfront
exl-id: c2b6afde-91a8-4e17-8e1a-3428b48e500a
source-git-commit: 6580fec18982215dbc2535d5f2ab159fc32ac3f5
workflow-type: tm+mt
source-wordcount: '982'
ht-degree: 0%

---

# カスタムフォームフィールドの情報を編集

フォームをオブジェクトに添付した後、カスタムフォームの情報を編集できます。 カスタムフォームをオブジェクトに追加する方法について詳しくは、 [オブジェクトへのカスタムフォームの追加](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfront plan*</p> </td> 
   <td>チーム以上</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Adobe Workfrontライセンス*</p> </td> 
   <td> <p>リクエスト以上</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル*</td> 
   <td> <p>カスタムフォームを編集するオブジェクトへのアクセスを編集します</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>オブジェクト権限</p> </td> 
   <td> 
    <ul> 
     <li> <p>カスタムフォームを編集するオブジェクトに対する権限を付与するか、それ以上に設定します。</p> </li> 
     <li>編集するフィールドに対する権限を表示します。 カスタムフィールドの共有権限について詳しくは、 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/configure-sharing-for-a-custom-field.md" class="MCXref xref">カスタムフィールドとウィジェットの共有を設定する</a>.</li> 
     <li> <p>編集するフィールドが配置されているフォーム上のセクションに対する権限の編集</p> </li> 
    </ul> <p>オブジェクトの追加アクセス権のリクエストについては、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

* Workfront管理者またはカスタムフォームへの管理者アクセス権を持つプランユーザーは、環境内でカスタムフォームを作成する必要があります。 詳しくは、 [カスタムフォームの作成または編集](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).
* オブジェクトには、カスタムフォームを添付する必要があります。

   オブジェクトにカスタムフォームを適用する方法について詳しくは、 [オブジェクトへのカスタムフォームの追加](../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## カスタムフォームの情報の編集

オブジェクトに添付されたカスタムフォームに関する情報の編集は、すべてのオブジェクトで同じです。 カスタムフォームを持つことのできるオブジェクトについて詳しくは、 [カスタムフォームの概要](../../administration-and-setup/customize-workfront/create-manage-custom-forms/custom-forms-overview.md).

1. カスタムフォームの情報を編集するオブジェクトに移動します。
1. クリック **`<Object type>`詳細** をクリックします。

   例えば、プロジェクトのカスタムフォームに関する情報を編集する場合は、 **プロジェクトの詳細**.

1. カスタムフォームまでスクロールします。 オブジェクトにカスタムフォームが添付されている場合、フォームの名前は「詳細」セクションの領域として表示されます。
1. 必要に応じて、矢印をクリックします。 ![](assets/expand-arrow-right.png) をクリックし、カスタムフォームの名前の左側に表示されます。
1. ページの右上隅にある編集アイコンをクリックします。 ![](assets/edit-icon.png).
1. アクセス権のある任意のフィールドに情報を入力します。

   ![](assets/click-in-field-to-edit-info-350x132.png)

   または

   フォームに情報がまだ入力されていない場合は、 **追加+** アクセス権を持つフィールドの情報を入力し始めます。

   ![](assets/plus-add-to-edit-info-350x180.png)

   オブジェクトに複数のカスタムフォームが添付されている場合は、各フォームに対してこれを実行できます。

   作業中のフィールドのタイプに応じて、次の点に注意してください。

   * ラジオボタンフィールドに選択できるオプションは 1 つだけです。
   * フォーム作成者がフィールドをどのように設定したかに応じて、チェックボックスフィールドで 1 つまたは複数のオプションを選択できます。
   * フォーム作成者がフィールドをどのように設定したかに応じて、複数選択ドロップダウンフィールドで 1 つまたは複数のオプションを選択できます。
   * テキストフィールド（太字、斜体、下線）の書式を設定できるのは、フォームを作成したユーザーが「書式設定」フィールドタイプのテキストフィールドとして設定した場合のみです。 1 行のテキストフィールドと段落のテキストフィールドは書式設定できません。
   * 日付フィールドタイプで時刻を更新できるのは、フォームを作成したユーザーがフィールドの作成時に時刻を含めている場合だけです。

   すべてのフィールドタイプについて詳しくは、 [カスタムフォームの作成または編集](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

1. クリック **保存** 変更点です。

   >[!IMPORTANT]
   >
   >
   >
   ><!--   >
   ><p style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This is true in "Edit custom forms" but not in "Add a custom form to an object." This snippet is used in both articles. The whole snippet is conditioned for classic only in "Add" but not in "Edit." Don't remove the NWE conditioning in the snippet because it is needed in "Edit."</p>   >
   >-->   >
   >
   >フォームを保存する前に、フォーム上のすべての必須フィールドに入力する必要があります。 必須フィールドの名前の後にアスタリスクが付きます。
   ![](assets/nwe-required-custom-field.png)   >

   オブジェクト内の計算カスタムフィールドで参照される別のオブジェクト内のデータを変更した場合、その変更はオブジェクトに自動的には反映されません。 オブジェクト内のすべての計算済みカスタムフィールドを手動で更新する方法については、 [オブジェクトの計算済みカスタムフィールドをすべて再計算する](#recalculate-all-calculated-custom-fields-for-an-object) 」を参照してください。

   また、オブジェクトをリスト内の他のオブジェクトと共に一括編集する際に、そのオブジェクトの計算済みカスタムフィールドをすべて手動で更新することもできます。 手順については、 [オブジェクトの編集時に、リスト内の複数のオブジェクトの計算済みカスタムフィールドをすべて再計算する](#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects) 」を参照してください。

## オブジェクトの計算済みカスタムフィールドをすべて再計算する  {#recalculate-all-calculated-custom-fields-for-an-object}

1. 再計算するユーザー設定フィールドを持つオブジェクトのメインページに移動します。
1. 次をクリック： **詳細** メニュー ![](assets/more-icon.png) オブジェクト名の右側にあるをクリックし、 **式を再計算**.

   これにより、オブジェクトのフォーム上のすべてのカスタムフィールドが再計算されます。

## オブジェクトの編集時に、リスト内の複数のオブジェクトの計算済みカスタムフィールドをすべて再計算する {#recalculate-all-calculated-custom-fields-for-multiple-objects-in-a-list-when-editing-the-objects}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this will need to be edited when the bulk edit for objects update in NW)</p>
-->

複数のオブジェクトのカスタムフィールドをリストまたはレポートから一括編集することで、手動で再計算することができます。

1. 計算フィールドを含むカスタムフォームを含むオブジェクトのリストに移動します。
1. 更新する計算カスタムフィールドを持つオブジェクトを選択します。
1. 次をクリック： **編集アイコン**.
1. クリック **カスタムForms** 左側のメニューで、「 **カスタム式の再計算**.
1. クリック **保存** **変更点**.

   Workfrontは、選択したすべてのオブジェクトのすべてのカスタムフィールドを計算します。

>[!TIP]
プロジェクトの複雑さに応じて、最適なパフォーマンスを確保するために計算済みのカスタムフィールドを一括で再計算する場合は、多数のプロジェクトを選択しないことをお勧めします。 プロジェクトが複雑すぎる可能性があるものには、複数の依存関係や割り当て、または多数のカスタムフィールドがあるものがあります。
プロジェクトのリストからカスタム式を一括して再計算するには、次の手順に従います。
1. プロジェクトリストまたはレポートに移動し、1 つまたは複数のプロジェクトを選択します。
1. 次をクリック： **詳細** メニュー ![](assets/more-icon.png)を選択し、「 **カスタム式の再計算**.
![](assets/recalculate-expressions-timeline-finances-drop-down-in-project-list-nwe.png)
Workfrontは、選択したすべてのプロジェクトのすべてのカスタムフィールドを計算します。
