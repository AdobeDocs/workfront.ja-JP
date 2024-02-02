---
product-area: templates
navigation-topic: templates-navigation-topic
title: プロジェクトテンプレートを削除
description: プロジェクトに関する履歴情報を長期にわたって保持できるように、使用しなくなったテンプレートは削除するのではなく、非アクティブ化することをお勧めします。テンプレートを非アクティブ化について詳しくは、プロジェクトテンプレートの編集を参照してください。
author: Alina
feature: Work Management
exl-id: 41e0979c-f8ef-4a07-8848-e4ee8cc212c5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '432'
ht-degree: 100%

---

# プロジェクトテンプレートを削除

プロジェクトに関する履歴情報を長期にわたって保持できるように、使用しなくなったテンプレートは削除するのではなく、非アクティブ化することをお勧めします。テンプレートの非アクティブ化について詳しくは、[プロジェクトテンプレートの編集](../../../manage-work/projects/create-and-manage-templates/edit-templates.md)を参照してください。

>[!IMPORTANT]
>
>テンプレートを削除しても、そのテンプレートを使用しているプロジェクトはまったく変更されません。ただし、プロジェクトのテンプレートフィールドに、元のテンプレートの名前が表示されなくなります。さらに、タスクビューでプロジェクト上のタスクのテンプレートタスクの名前を表示できなくなります。プロジェクト上のテンプレートフィールドとタスク上のテンプレートタスクフィールドは、プロジェクトに最初に関連付けられていたテンプレートが削除された後は空白のままです。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>削除へのアクセス権を含むテンプレートへの編集アクセス権</p> <p> <img src="assets/template-access-level-with-advanced-settings-350x113.png" style="width: 350;height: 113;"> </p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>テンプレートを削除する権限を含む、テンプレートへの管理権限</p> <p> <img src="assets/template-manage-permissions-with-advanced-settings-350x352.png" style="width: 350;height: 352;"> </p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## テンプレートの削除に関する考慮事項

* テンプレートが添付されたときにプロジェクトに追加されたタスクは、プロジェクトに残ります。ただし、タスクに関連付けられているテンプレートタスク情報は削除されます。
* テンプレートの名前は、プロジェクトの「**概要**」サブタブの「**テンプレート**」フィールドにリスト表示されなくなります。

* 最近削除したテンプレートはごみ箱から復元できます。ごみ箱からアイテムを復元する方法については、[削除したアイテムの復元](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md)を参照してください。

## テンプレートを削除

1. **メインメニュー** ![](assets/main-menu-icon.png) から、「**テンプレート**」をクリックします。これにより、テンプレートのリストが開きます

1. テンプレート名の左側にあるチェックボックスをクリックして、削除するテンプレートを選択し、**「削除」／「はい、削除します」**&#x200B;をクリックして削除を確定します。

   または

   テンプレートの名前をクリックしてアクセスし、**その他**&#x200B;メニュー ![](assets/qs-more-icon-on-an-object.png)、**「テンプレートを削除」／「はい、削除します」**&#x200B;の順にクリックします。

   テンプレートが利用できなくなり、プロジェクトに関連付けることができなくなります。
