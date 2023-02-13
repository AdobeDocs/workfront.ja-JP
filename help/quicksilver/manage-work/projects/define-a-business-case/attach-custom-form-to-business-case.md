---
navigation-topic: business-case-and-scorecards
title: ビジネス事例にカスタムフォームを添付する
description: カスタムFormsは、既存のAdobe Workfrontフィールドに表示されない情報を収集するために使用されます。
author: Alina
feature: Work Management
exl-id: f781fd00-968c-4e5d-b82c-a74acedb2734
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '380'
ht-degree: 0%

---

# ビジネス事例にカスタムフォームを添付する

カスタムFormsは、既存のAdobe Workfrontフィールドに表示されない情報を収集するために使用されます。 

カスタムFormsの作成について詳しくは、 [カスタムフォームの作成または編集](../../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Pro 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>プロジェクトへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>プロジェクトに対する権限以上の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## プロジェクトへのカスタムFormsの添付

次の領域で、カスタムFormsをプロジェクトに添付できます。

* プロジェクトの編集時に、「プロジェクトの詳細」セクションで、
* プロジェクトの編集時に、「プロジェクトを編集」ボックスで、
* 複数のプロジェクトを一括編集する場合、プロジェクトのリストから。

   1 つまたは複数のプロジェクトを編集する際のプロジェクトへのカスタムフォームの添付について詳しくは、この記事を参照してください [プロジェクトを編集](../../../manage-work/projects/manage-projects/edit-projects.md).

* プロジェクトのビジネスケースを構築する際に、この記事で説明するビジネスケースを使用します。

カスタムフォームをオブジェクトに添付する方法について詳しくは、 [オブジェクトへのカスタムフォームの追加](../../../workfront-basics/work-with-custom-forms/add-a-custom-form-to-an-object.md).

## ビジネス事例へのカスタムFormsの添付

カスタムをからビジネスケースに追加するには、Workfront管理者がセットアップでこのオプションを選択する必要があります。 セットアップでカスタムフォームを有効にする方法について詳しくは、「 [システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md) 記事内 [システム全体のプロジェクト環境設定の指定](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

カスタムフォームを添付するには：

1. フォームの添付先のプロジェクトに移動し、「 **ビジネス事例** をクリックします。

   ビジネスケースが表示されます。

1. 内 **カスタムフォーム** 」セクションで、添付するカスタムフォームをドロップダウンメニューから選択します。

   ![](assets/custom-forms-drop-down-menu.png)

1. （オプション）「 」を選択します。 **カスタムフォームを編集**.\
   ![](assets/acf1-350x122.png)

1. （オプション）カスタムフォームのフィールドに情報を指定し、 **保存** .
