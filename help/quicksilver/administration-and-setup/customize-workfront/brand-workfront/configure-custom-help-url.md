---
title: カスタムヘルプ URL の設定
user-type: administrator
product-area: system-administration
navigation-topic: brand-workfront
description: Workfrontの使用方法に関する情報を含んだカスタムの内部ヘルプサイトを作成する場合は、メインメニューヘルプ アイコンをクリックして、そのサイトに移動できます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d2b63508-1943-4f9e-888e-8f1bfb54c33e
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '274'
ht-degree: 47%

---

# カスタムヘルプ URL の設定

Workfrontの使用方法に関する情報を含んだカスタムの内部ヘルプサイトを作成する場合は、メインメニューヘルプ アイコンをクリックして、そのサイトに移動できます。

![](assets/custom-help-button.png)

このことは、Workfront全体でコンテキストに沿ったヘルプリンク（Workfrontのヘルプサイトにアクセスできる）には影響しません。

Workfrontで設定するカスタムヘルプ URL と通常のAdobe Workfront ヘルプサイトの両方にユーザーがアクセスする方法について詳しくは、[Workfront ヘルプへのアクセス ](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/access-workfront-help.md) を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：標準</p>
       <p>または</p>
       <p>現在：プラン</p></td>
  </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## カスタムヘルプ URL の設定

{{step-1-to-setup}}

1. **システム**／**環境設定**&#x200B;をクリックします。
1. 「**一般的な環境設定**」セクション内の「**ヘルプ URL**」フィールドに、カスタムヘルプサイトの URL を入力します。

   カスタムヘルプの場所でログイン資格情報が必要な場合は、ユーザーが Workfront からサイトにアクセスする際に、それらの資格情報が必要になります。シングルサインオン（SSO）を使用していない場合は、カスタムヘルプサイトへの資格情報を Workfront の資格情報とは別に管理する必要が生じる場合があります。

1. 「**保存**」をクリックします。

   カスタムヘルプ URL を保存したら、カスタム URL を削除して「**保存** をクリックすると、デフォルトのWorkfront ヘルプサイトに戻ることができます。
