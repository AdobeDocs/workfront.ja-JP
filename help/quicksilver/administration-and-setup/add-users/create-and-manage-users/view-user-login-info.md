---
title: ユーザーログイン情報の表示
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: ユーザーのリスト表示またはユーザーのレポートにこの情報を含めることを示すことで、ユーザーがWorkfrontにログインした頻度や最後にログインした時間を確認できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7b37c34a-d628-4d9b-9688-e4b9f89c666b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '570'
ht-degree: 0%

---

# ユーザーログイン情報の表示

ユーザーのリスト表示またはユーザーのレポートにこの情報を含めることを示すことで、ユーザーがAdobe Workfrontにログインした頻度や最後にログインした時間を確認できます。

## アクセス要件

この記事の手順を実行するには、次の手順を実行する必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfrontプラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス</td> 
   <td> <p>計画 </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>次のいずれかが必要です。</p> 
    <ul> 
     <li> <p>システム管理者のアクセスレベル。 詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>. </p> </li> 
     <li> <p><b>ユーザー</b> 設定を <b>編集</b> アクセス、 <b>作成</b> そして少なくとも 2 つのうち 1 つは <b>ユーザー管理者</b> 以下で有効になるオプション <b>設定を微調整する</b> <img src="assets/gear-icon-in-access-levels.png">. </p> <p>この 2 つのオプションのうち、ユーザー <b>管理者（グループユーザー）</b> が有効になっている場合は、ユーザーがメンバーであるグループのグループ管理者である必要があります。</p> <p>詳しくは、 <b>ユーザー</b> アクセスレベルでの設定については、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権の付与</a>.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Workfrontによるログイン情報の記録方法

Workfrontは、システムにログインしているユーザーに関する次の情報を記録します。

* **ログイン数**:Workfrontは、24 時間に 1 回、アプリケーションにログインするユーザーをカウントします。 1 人のユーザーが異なるブラウザー、コンピューター、モバイルデバイスを複数回ログインした場合、Workfrontは 1 日に発生したすべてのログインを 1 回のログインとしてカウントします。 ログイン数には、ユーザーが作成された日時で始まる情報が含まれます。
* **最終ログイン日**:ユーザーがログインした最後の日付。 ブラウザー、モバイルデバイス、その他のアプリケーションからのすべてのログイン日が、このフィールドに記録されます。

次のいずれかの方法でWorkfrontにログインすると、Workfrontへのログインとしてカウントされます。

* Workfront Web アプリケーション
* Workfrontモバイルアプリ (iOSまたは Android デバイス )
* サポートされるWorkfrontと他のサードパーティアプリケーション (Slack、Jira) との統合
* Workfrontと他のサードパーティアプリケーションとのカスタム統合。
* Workfront API

   >[!NOTE]
   >
   >Workfront API を使用したWorkfrontへのログインは、まだAdobeビジネスプラットフォームにオンボーディングされていない組織でのみ使用できます。

## ユーザーリストまたはレポートに使用状況情報を表示する

ユーザーのリストの表示、またはユーザーのレポートに、「ログイン数」フィールドと「最終ログイン日」フィールドを表示できます。\
レポートの作成について詳しくは、 [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

ユーザーのリストのビューに使用状況情報を表示するには：

1. Workfrontでユーザーのリストに移動します。
1. 次の **表示** ドロップダウンメニューで、「 **新しいビュー**.

1. クリック **列を追加** 画面の右下隅付近にあります。
1. 内 **この列に表示** フィールド、入力を開始 **ログイン数**&#x200B;を選択し、リストの下に表示されたら選択します。 **ユーザー**.

1. クリック **列を追加** 再び
1. 内 **列に表示** フィールド、入力を開始 **最終ログイン日**&#x200B;を選択し、リストの下に表示されたら選択します。 **ユーザー**.

1. （オプション）「 **詳細オプション**&#x200B;を選択し、 **フィールドの形式** をドロップダウンメニューから選択し、最後のログインの時刻や曜日を列に含めます。

1. クリック **ビューを保存**.\
   このビューには、ユーザーが何回ログインしたか、および最後にログインした日時に関する情報が表示されます。
