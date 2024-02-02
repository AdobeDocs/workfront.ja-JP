---
title: ユーザーログイン情報を表示
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
description: ユーザーのリストのビューまたはユーザーのレポートにこの情報を含めることを指定すると、ユーザーが Workfront にログインする頻度と最終ログイン時刻を確認できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7b37c34a-d628-4d9b-9688-e4b9f89c666b
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '570'
ht-degree: 100%

---

# ユーザーログイン情報を表示

ユーザーのリストのビューまたはユーザーのレポートにこの情報を含めることを指定すると、ユーザーが Adobe Workfront にログインする頻度と最後にログインした時刻を確認できます。

## アクセス要件

この記事の手順を実行するには、以下を保有している必要があります。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> <p>プラン </p>   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>次のいずれかが必要です。</p> 
    <ul> 
     <li> <p>システム管理者のアクセスレベル。詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与</a>を参照してください。 </p> </li> 
     <li> <p><b>編集</b>アクセスに設定されたアクセスレベルでの<b>ユーザー</b>設定には、<b>作成</b>および<b>設定を微調整</b> <img src="assets/gear-icon-in-access-levels.png"> の下で有効となる少なくとも 2 つのうち 1 つの<b>ユーザー管理者</b>オプションがあります。 </p> <p>この 2 つのオプションのうち、ユーザー<b>管理者（グループユーザー）</b>が有効になっている場合は、ユーザーがメンバーであるグループのグループ管理者である必要があります。</p> <p>アクセスレベルの<b>ユーザー</b>設定について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md" class="MCXref xref">ユーザーへのアクセス権を付与</a>を参照してください。</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

## Workfront によるログイン情報の記録方法

Workfront は、システムにログインしているユーザーに関する次の情報を記録します。

* **ログイン回数**：Workfront は 24 時間に 1 回、アプリケーションにログインするユーザーをカウントします。1 人のユーザーが異なるブラウザー、コンピューター、モバイルデバイスを複数回ログインした場合、Workfront は 1 日に発生したすべてのログインを 1 回のログインとしてカウントします。ログイン回数には、ユーザーが作成された日時で始まる情報が含まれます。
* **最終ログイン日**：ユーザーがログインした最後の日付。ブラウザー、モバイルデバイス、その他のアプリケーションからのすべてのログイン日が、このフィールドに記録されます。

次のいずれかの方法で Workfront にログインすると、Workfront へのログインとしてカウントされます。

* Workfront web アプリケーション
* Workfront モバイルアプリ（iOS または Android デバイス）
* サポートされている Workfront と別のサードパーティアプリケーション（Slack、Jira）の統合
* Workfront と他のサードパーティアプリケーションとのカスタム統合。
* Workfront API

  >[!NOTE]
  >
  >Workfront API を使用した Workfront へのログインは、まだ Adobe Business Platform にオンボーディングされていない組織でのみ使用できます。

## ユーザーリストまたはレポートに使用状況情報を表示する

ユーザーのリストのビューまたはユーザーのレポートに、「ログイン回数」フィールドと「最終ログイン日」フィールドを表示できます。\
レポートの作成について詳しくは、[カスタムレポートを作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。

ユーザーのリストのビューに使用状況情報を表示するには、次の手順に従います。

1. Workfront でユーザーのリストに移動します。
1. 「**表示**」ドロップダウンメニューから、「**新規ビュー**」を選択します。

1. 右下隅付くにある「**列を追加**」をクリックします。
1. 「**この列に表示**」フィールドに、「**ログイン回数**」の入力を開始し、「**ユーザー**」の下のリストに表示されたら選択します。

1. 「**列を追加**」を再度クリックします。
1. 「**この列に表示**」フィールドに、「**最終ログイン日**」の入力を開始し、「**ユーザー**」の下のリストに表示されたら選択します。

1. （オプション）「**詳細オプション**&#x200B;をクリックし、「**フィールド形式**」をドロップダウンメニューから選択して、最後ログインの時刻や日を列に含めます。

1. 「**ビューを保存**」をクリックします。\
   このビューには、ユーザーが何回ログインしたか、および最後にログインした日時に関する情報が表示されます。
