---
title: カスタムヘルプ URLの設定
user-type: administrator
product-area: system-administration
navigation-topic: brand-workfront
description: 組織でのWorkfrontの使用方法に関する情報を含むカスタム内部ヘルプサイトを作成する場合は、メインメニューヘルプアイコンを設定して、そのサイトに移動できます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: d2b63508-1943-4f9e-888e-8f1bfb54c33e
TQID: https://experienceleague.adobe.com/sQ0-5jDNs4Pr8icC-mYCp0QFec5g1i-e0XkTz78WEWQ
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: c66ffd68-0f65-42bb-aa23-b4020f12e0bd
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 256
ht-degree: 37%

---

# カスタムヘルプ URL の設定

組織でのWorkfrontの使用方法に関する情報を含むカスタム内部ヘルプサイトを作成する場合は、メインメニューヘルプアイコンを設定して、そのサイトに移動できます。

![&#x200B; カスタムヘルプボタン &#x200B;](assets/custom-help-with-left-menu.png)

これは、Workfront ヘルプサイトに移動するWorkfront全体のコンテクストに応じたヘルプリンクには影響しません。

Workfrontで設定したカスタムヘルプ URLと通常のWorkfront ヘルプサイトの両方にユーザーがアクセスする方法について詳しくは、[Adobe Workfront ヘルプへのアクセス &#x200B;](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/access-workfront-help.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront プラン</td> 
   <td><p>標準</p>
       <p>プラン</p></td>
  </tr> 
  <tr> 
   <td>アクセスレベル設定</td> 
   <td>システム管理者</td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## カスタムヘルプ URL の設定

{{step-1-to-setup}}

1. **システム**／**環境設定**&#x200B;をクリックします。
1. **一般設定** セクションの&#x200B;**カスタムヘルプ URL** フィールドに、カスタムヘルプサイトが配置されているURLを入力します。

   カスタムヘルプの場所でログイン資格情報が必要な場合は、ユーザーが Workfront からサイトにアクセスする際に、それらの資格情報が必要になります。 シングルサインオン（SSO）を使用していない場合は、カスタムヘルプサイトへの資格情報を Workfront の資格情報とは別に管理する必要が生じる場合があります。

1. 「**保存**」をクリックします。

   カスタムのヘルプ URLを保存したら、カスタム URLを削除して「**保存**」をクリックし、デフォルトのWorkfront ヘルプサイトを使用して戻ることができます。
