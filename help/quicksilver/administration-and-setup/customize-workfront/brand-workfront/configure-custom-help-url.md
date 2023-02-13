---
title: カスタムヘルプ URL の設定
user-type: administrator
product-area: system-administration
navigation-topic: brand-workfront
description: 組織でのWorkfrontの使用方法に関する情報を含むカスタム内部ヘルプサイトを作成する場合は、メインメニューのヘルプアイコンを設定して、そのサイトに移動できます。 これは、メインメニューのメインヘルプリンクや、Workfront全体の状況に応じたヘルプリンクには影響しません。このリンクは、ユーザーがWorkfrontヘルプサイトにアクセスする際に使用します。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: d2b63508-1943-4f9e-888e-8f1bfb54c33e
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '317'
ht-degree: 4%

---

# カスタムヘルプ URL の設定

組織でのWorkfrontの使用方法に関する情報を含むカスタム内部ヘルプサイトを作成する場合は、メインメニューのヘルプアイコンを設定して、そのサイトに移動できます。

![](assets/custom-help-button.png)

これは、メインメニューのメインヘルプリンクや、Workfront全体の状況に応じたヘルプリンクには影響しません。このリンクは、ユーザーがWorkfrontヘルプサイトにアクセスする際に使用します。

![](assets/custom-help-url.png)

Workfrontで設定したカスタムヘルプ URL と通常のWorkfrontヘルプサイトの両方にユーザーがアクセスする方法について詳しくは、 [新しいAdobe WorkfrontエクスペリエンスでのWorkfrontヘルプへのアクセス](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/access-workfront-help.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

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
   <td>計画</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront管理者である。</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## カスタムヘルプ URL の設定

1. メインメニューアイコンをクリックします。 ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅にある「設定」をクリックします。
1. クリック **システム** > **環境設定**.
1. 内 **一般環境設定** セクション内の **カスタムヘルプ URL** 「 」フィールドに、カスタムヘルプサイトの URL を入力します。

   カスタムヘルプの場所でログイン資格情報が必要な場合は、ユーザーがWorkfrontからサイトにアクセスする際に、それらの資格情報が必要になります。 シングルサインオン (SSO) を使用しない場合は、カスタムヘルプサイトへの資格情報をWorkfrontの資格情報とは別に管理する必要が生じる場合があります。

1. 「**保存**」をクリックします。
