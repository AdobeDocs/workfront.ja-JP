---
product-area: projects;user-management
keywords: 添付、適用
navigation-topic: work-with-custom-forms
title: カスタムフォームのオブジェクトへの追加
description: 既存のカスタムフォームを、以下にリストされているオブジェクトのいずれかに追加できます。カスタムフォームには、オブジェクトに関する情報を保存できるカスタムフィールドが含まれています。
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '730'
ht-degree: 93%

---

# カスタムフォームのオブジェクトへの追加

<!--Audited: 12/2023-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

既存のカスタムフォームを、以下にリストされているオブジェクトのいずれかに追加できます。カスタムフォームには、オブジェクトに関する情報を保存できるカスタムフィールドが含まれています。

* プロジェクト（ビジネスケースを含む）
* タスク
* イシュー
* 会社
* ポートフォリオ
* プログラム
* ドキュメント
* ユーザー
* グループ
* 反復
* 費用
* 請求記録

カスタムフォームは、フォームが作成されたオブジェクトにのみ追加できます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
<tr> 
  <td role="rowheader">Adobe Workfront プラン</td> 
  <td> <p>投稿者以上</p>
 <p>リクエスト以上</p> 
</td> 
 </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>カスタムフォームを管理するオブジェクトへの編集アクセス権</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>カスタムフォームを添付するオブジェクトへの権限を管理します。</p> <p><b> カスタムデータに添付 </b> オブジェクト（プロジェクト、タスク、イシュー）への権限を持つ、カスタムフォームへの表示以上の権限。</td> 
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
   <td role="rowheader">Adobe Workfront plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
<tr> 
  <td role="rowheader">Adobe Workfront license</td> 
  <td> <p>New: Contributor or higher </p>
 <p>or</p> 
<p>Current: Request or higher </p> 
</td> 
 </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>Edit access to the objects for which you manage custom forms</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to the object for which you want to attach a custom form.</p> <p>View or higher permissions to the custom form, with permission to <b>Attach to Custom Data</b> objects (projects, tasks, and issues). For more information, see <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Share a custom form</a>.</p> <p>Important: If you do not have a Plan license with administrative access to&nbsp;Custom&nbsp;Forms, you must have specific permissions to at least view the custom form, as described in <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">Share a custom form</a>. These permissions must be granted to you even if the form is visible system-wide. </p> <p>For information on requesting additional access, see <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## 前提条件

カスタムフォームをオブジェクトに追加するには、Workfront 管理者または Plan ライセンスと、カスタムフォームへの管理アクセス権を持つユーザーが環境内にカスタムフォームを作成する必要があります。詳しくは、[ カスタムフォームの作成 ](/help/quicksilver/administration-and-setup/customize-workfront/create-manage-custom-forms/form-designer/design-a-form/design-a-form.md) を参照してください。

## カスタムフォームのオブジェクトへの追加

カスタムフォームをオブジェクトに追加するには、次の 2 つの方法があります。

* [オブジェクトを編集してカスタムフォームをオブジェクトに追加](#add-a-custom-form-to-an-object-by-editing-the-object)
* [詳細領域からオブジェクトにカスタムフォームを追加](#add-a-custom-form-to-an-object-from-the-details-area)

### オブジェクトを編集してカスタムフォームをオブジェクトに追加 {#add-a-custom-form-to-an-object-by-editing-the-object}

1. カスタムフォームを追加するオブジェクトに移動します。
1. **その他**&#x200B;メニュー![](assets/more-icon.png)を選択し、「**編集**」![](assets/edit-icon.png)をクリックします。
1. **カスタムフォーム**／**フォームを追加**&#x200B;をクリックし、ドロップダウンメニューから最大 10 個のフォームを選択します。

1. （オプション）カスタムフォームの編集可能なフィールドの情報を更新します。

   追加するフォームのすべての必須フィールドを更新する必要があります。

1. 「**保存**」をクリックします。

### 詳細領域からオブジェクトにカスタムフォームを追加 {#add-a-custom-form-to-an-object-from-the-details-area}

1. カスタムフォームを追加するオブジェクトに移動します。
1. 左側のパネルで、**`<Object type>`詳細**&#x200B;セクションをクリックします。例えば、**プロジェクトの詳細**&#x200B;をクリックしてカスタムフォームをプロジェクトに追加するか、**イシューの詳細**&#x200B;をクリックしてカスタムフォームをイシューに追加します。
1. 右上隅の「**カスタムフォームを追加**」フィールドをクリックし、表示されるリストから最大 10 個のカスタムフォームを選択します。

   フォームに必須フィールド（赤いアスタリスクが付いているフィールド）が含まれていても、現時点では入力する必要はありません。

   選択したフォームは自動的にオブジェクトに添付されます。

1. （オプション）フォームのカスタムフィールドの情報を更新し、「**変更を保存**」をクリックします。

## オブジェクトの複数のカスタムフォーム

特定のオブジェクトに最大 10 個のカスタムフォームを追加できるため、一部のユーザーにはフィールドの使用を許可し、他のユーザーにはフィールドの使用を許可しないなど、複数のプロジェクトのフォーム要件をより適切に満たすことができます。

**例：**&#x200B;既存のプロジェクトに既にカスタムフォームがあり、別のカスタムフォームに存在するカスタムフィールドがこのプロジェクトで必要となった場合、既存のカスタムフォームにフィールドを追加するのではなく、2 番目のフォームを追加フィールドとしてプロジェクトに追加することができます。

## 複数のオブジェクトにカスタム フォームを一括で追加

リストからオブジェクトを選択することで、複数のオブジェクトにカスタムフォームを追加できます。

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>オブジェクトにカスタムフォームを追加する方法は、プロジェクトを除くすべてのオブジェクトで同じです。
>
>カスタムフォームをプロジェクトに一括で追加する方法については、[プロジェクトの編集](../../manage-work/projects/manage-projects/edit-projects.md)を参照してください。


1. オブジェクトのリストに移動します。
1. リスト内の複数のオブジェクトを選択します。

1. **その他**&#x200B;メニュー ![](assets/more-icon.png)、**編集**&#x200B;アイコン ![](assets/edit-icon.png) の順にクリックします。

   または

   リストの上部にある&#x200B;**編集**&#x200B;アイコン ![](assets/edit-icon.png) をクリックします。
1. 左側のパネルで「**カスタムフォーム**」をクリックします。
1. **選択**&#x200B;ドロップダウンメニューで、選択したすべてのオブジェクトに関連付けるフォームを選択します。

   >[!NOTE]
   >
   >ドロップダウンメニューにフォームが見つからない場合は、少なくとも 1 つのオブジェクトにフォームがすでに関連付けられていることを意味します。フォームを残りのオブジェクトに追加する前に、どのオブジェクトであるかを特定し、選択から削除してください。


1. 「**変更を保存**」をクリックします。

   フォームに必須フィールド（赤いアスタリスクが付いているフィールド）が含まれていても、現時点では入力する必要はありません。
