---
product-area: projects;user-management
keywords: アタッチ、適用
navigation-topic: work-with-custom-forms
title: オブジェクトにカスタムフォームを追加する
description: 以下に示す任意のオブジェクトに既存のカスタムフォームを追加できます。 カスタムフォームには、オブジェクトに関する情報を格納できるカスタムフィールドが含まれています。
author: Alina
feature: Get Started with Workfront
exl-id: c06666a7-ab78-4311-8fcb-1d1a68034133
source-git-commit: aec61210cf2c17775738db4975ae8d19223153cc
workflow-type: tm+mt
source-wordcount: '811'
ht-degree: 2%

---

# オブジェクトにカスタムフォームを追加する

<!--Audited: 12/2023-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available for all customers in the Preview environment and for a select group of customers in the Production environment.</span>-->

以下に示す任意のオブジェクトに既存のカスタムフォームを追加できます。 カスタムフォームには、オブジェクトに関する情報を格納できるカスタムフィールドが含まれています。

* プロジェクト（ビジネス事例を含む）
* タスク
* イシュー
* 会社
* ポートフォリオ
* プログラム
* ドキュメント
* ユーザー
* イテレーション
* 費用
* 請求記録

カスタムフォームは、フォームが作成されたオブジェクトのタイプにのみ追加できます。

## アクセス要件

この記事で説明する操作を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td> <p>任意 </p> </td> 
  </tr> 
<tr> 
  <td role="rowheader">Adobe Workfrontライセンス</td> 
  <td> <p>新規：寄稿者以上 </p>
 <p>または</p> 
<p>現在：リクエスト以降 </p> 
</td> 
 </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>カスタムフォームを管理するオブジェクトへのアクセスを編集します</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>カスタムフォームを添付するオブジェクトに対する権限を管理します。</p> <p>カスタムフォームに対する表示権限以上の権限 ( <b>カスタムデータに添付</b> オブジェクト（プロジェクト、タスク、問題）。 詳しくは、 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">カスタムフォームの共有</a>.</p> <p>重要：カスタムFormsへの管理アクセス権を持つプランライセンスをお持ちでない場合は、カスタムフォームを表示するための特定の権限が必要です。詳しくは、 <a href="../../administration-and-setup/customize-workfront/create-manage-custom-forms/share-access-to-a-custom-form.md" class="MCXref xref">カスタムフォームの共有</a>. フォームがシステム全体で表示されている場合でも、これらの権限をユーザーに付与する必要があります。 </p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報の詳細については、 [Workfrontドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

## 前提条件

Workfrontの管理者またはプランライセンスを持ち、カスタムフォームに管理者からアクセスできるユーザーは、環境内でカスタムフォームを作成してから、オブジェクトに追加する必要があります。 詳しくは、 [カスタムフォームの作成または編集](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## オブジェクトにカスタムフォームを追加する

カスタムフォームをオブジェクトに追加するには、次の 2 つの方法があります。

* [オブジェクトを編集してカスタムフォームをオブジェクトに追加する](#add-a-custom-form-to-an-object-by-editing-the-object)
* [「詳細」領域からオブジェクトにカスタムフォームを追加する](#add-a-custom-form-to-an-object-from-the-details-area)

### オブジェクトを編集してカスタムフォームをオブジェクトに追加する {#add-a-custom-form-to-an-object-by-editing-the-object}

1. カスタムフォームを追加するオブジェクトに移動します。
1. 次をクリック： **その他** メニュー ![](assets/more-icon.png)を選択し、次に **編集** ![](assets/edit-icon.png).
1. クリック **カスタムForms** > **Formsを追加**&#x200B;を選択し、ドロップダウンメニューから最大 10 個のフォームを選択します。

1. （オプション）カスタムフォームの編集可能フィールドの情報を更新します。

   追加するフォームのすべての必須フィールドを更新する必要があります。

1. 「**保存**」をクリックします。

### 「詳細」領域からオブジェクトにカスタムフォームを追加する {#add-a-custom-form-to-an-object-from-the-details-area}

1. カスタムフォームを追加するオブジェクトに移動します。
1. 次をクリック： **`<Object type>`詳細** 」セクションを使用して、 例えば、「 **プロジェクトの詳細** カスタムフォームをプロジェクトに追加するには、または **問題の詳細** をクリックして、カスタムフォームをイシューに追加します。
1. 次をクリック： **カスタムフォームを追加** フィールドを選択し、表示されるリストから最大 10 個のカスタムフォームを選択します。

   フォームに必須フィールド（赤いアスタリスクでマーク）が含まれている場合は、現時点で入力する必要はありません。

   選択したフォームが自動的にオブジェクトに添付されます。

1. （オプション）フォームのカスタムフィールドの情報を更新し、 **変更を保存**.

## 1 つのオブジェクト上の複数のカスタムフォーム

特定のオブジェクトに最大 10 個のカスタムフォームを追加でき、一部のユーザーや他のユーザーが使用できないようにしたり、複数のプロジェクトのフォーム要件をより適切に満たすことができます。

**例：** 既存のプロジェクトに既にカスタムフォームがあり、別のカスタムフォームに存在するこのプロジェクトに追加のカスタムフィールドが必要な場合は、既存のカスタムフォームにフィールドを追加する代わりに、追加のフィールドを使用して 2 つ目のフォームを追加できます。

## 複数のオブジェクトへのカスタムフォームの一括追加

カスタムフォームをリスト内で選択して、複数のオブジェクトに追加できます。

<!--
drafted for bulk-editing projects. When it releases to Prod for projects, take "in the preview environment" and the yellow tags out. Add additional objects here in the same way when they become available:-->

>[!NOTE]
>
>カスタムフォームをオブジェクトに追加する方法は、プロジェクト以外のすべてのオブジェクトで同じです。
>
>カスタムフォームを一括でプロジェクトに追加する方法については、この記事を参照してください。 [プロジェクトを編集](../../manage-work/projects/manage-projects/edit-projects.md).


1. オブジェクトのリストに移動します。
1. リスト内の複数のオブジェクトを選択します。

1. 次をクリック： **その他** メニュー ![](assets/more-icon.png)」、「 **編集** アイコン  ![](assets/edit-icon.png).

   または

   次をクリック： **編集** アイコン ![](assets/edit-icon.png) をクリックします。
1. クリック **カスタムForms** をクリックします。
1. （内） **選択を行う** ドロップダウンメニューから、選択したすべてのオブジェクトに関連付けるフォームを選択します。

   >[!NOTE]
   >
   >ドロップダウンメニューにフォームが表示されない場合は、1 つ以上のオブジェクトに、既にフォームが関連付けられていることを意味します。 フォームを残りのオブジェクトに追加する前に、どのオブジェクトを選択するかを決定し、選択から削除します。


1. 「**変更を保存**」をクリックします。

   フォームに必須フィールド（赤いアスタリスクでマーク）が含まれている場合は、現時点で入力する必要はありません。
