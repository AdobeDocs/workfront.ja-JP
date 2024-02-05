---
product-area: projects;user-management
keywords: 添付、適用
navigation-topic: work-with-custom-forms
title: カスタムフォームのオブジェクトへの追加
description: 既存のカスタムフォームを、以下にリストされているオブジェクトのいずれかに追加できます。カスタムフォームには、オブジェクトに関する情報を保存できるカスタムフィールドが含まれています。
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: aec61210cf2c17775738db4975ae8d19223153cc
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 86%

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
* 反復
* 費用
* 請求記録

カスタムフォームは、フォームが作成されたオブジェクトにのみ追加できます。

## アクセス要件

この記事で説明する操作を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
<tr> 
  <td role="rowheader">Adobe Workfront ライセンス</td> 
  <td> <p>新規：寄稿者以上 </p>
 <p>または</p> 
<p>現在：リクエスト以降 </p> 
</td> 
 </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>カスタムフォームを管理するオブジェクトへの編集アクセス権</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>カスタムフォームを添付するオブジェクトへの権限を管理します。</p> <p><b>カスタムデータに添付</b>オブジェクト（プロジェクト、タスク、イシュー）への権限がある、カスタムフォームの表示権限以上の権限。詳しくは、<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">カスタムフォームの共有</a>を参照してください。</p> <p>重要: カスタムフォームへの管理アクセス権がある Plan ライセンスを所有していない場合は、<a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">カスタムフォームの共有</a> で説明されているように、少なくともカスタムフォームを表示するための権限が必要です。これらの権限は、フォームがシステム全体で表示される場合でも付与する必要があります。 </p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへの利用申請</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 前提条件

カスタムフォームをオブジェクトに追加するには、Workfront 管理者または Plan ライセンスと、カスタムフォームへの管理アクセス権を持つユーザーが環境内にカスタムフォームを作成する必要があります。詳しくは、[カスタムフォームの作成または編集](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md)を参照してください。

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

**例：** 既存のプロジェクトに既にカスタムフォームがあり、別のカスタムフォームに存在するこのプロジェクトに追加のカスタムフィールドが必要な場合は、既存のカスタムフォームにフィールドを追加する代わりに、追加のフィールドを使用して 2 つ目のフォームを追加できます。

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

1. 次をクリック： **その他** メニュー ![](assets/more-icon.png)」、「 **編集** アイコン  ![](assets/edit-icon.png).

   または

   次をクリック： **編集** アイコン ![](assets/edit-icon.png) をクリックします。
1. 左側のパネルで「**カスタムフォーム**」をクリックします。
1. （内） **選択を行う** ドロップダウンメニューから、選択したすべてのオブジェクトに関連付けるフォームを選択します。

   >[!NOTE]
   >
   >ドロップダウンメニューにフォームが見つからない場合は、少なくとも 1 つのオブジェクトにフォームがすでに関連付けられていることを意味します。フォームを残りのオブジェクトに追加する前に、どのオブジェクトであるかを特定し、選択から削除してください。


1. 「**変更を保存**」をクリックします。

   フォームに必須フィールド（赤いアスタリスクが付いているフィールド）が含まれていても、現時点では入力する必要はありません。
