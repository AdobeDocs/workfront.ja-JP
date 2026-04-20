---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: ユーザー属性の割り当て
description: シングルサインオン（SSO）を使用して、ID プロバイダーの Active Directory から Adobe Workfront ユーザーに属性を渡すことができます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 3d523584-dcb8-4aa6-8217-611f22dc1450
source-git-commit: d8ccdeac9a658ca7a2862781e98c2c3c6fa0e8a0
workflow-type: tm+mt
source-wordcount: '586'
ht-degree: 95%

---

# ユーザー属性を割り当て

<!--Audited 2/2024-->

シングルサインオン（SSO）を使用して、ID プロバイダーの Active Directory から Adobe Workfront ユーザーに属性を渡すことができます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td><p>任意</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>標準</p><p>プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td><p>あなたはWorkfrontの管理者でなければなりません</p></td>
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## 属性のマッピングに関するヒント

属性をマッピングする際は、次の点に留意してください。

* 必ず、プレビューサンドボックスまたはCustomer Refresh（CR）サンドボックスでテストしてください。
* 管理者アカウントと非管理者アカウントの両方でテストして、属性が正しくマッピングされていることを確認します。
* マッピングされた属性は、ユーザーがシングルサインオンでログインするたびに適用されます。

  例：「姓」をマッピングし、ID プロバイダーの値を更新せずに Workfront で名前を更新すると、次回ユーザーがサインインしたときに、ID プロバイダー内の値と一致するように姓が上書きされます。

## 組織のユーザー属性のマッピング

1. Adobe Workfrontの左上隅にある&#x200B;**メインメニュー** アイコン ![&#x200B; メインメニューアイコン &#x200B;](assets/main-menu-left.png)をクリックし、**セットアップ** ![&#x200B; ギア設定アイコン &#x200B;](assets/gear-icon-settings.png)をクリックします。

1. **システム**／**シングルサインオン(SSO)** をクリックします。

1. 「**アドビ**」タブを選択します。

1. （オプションおよび条件付き）組織の属性マッピングが従来のエクスペリエンスで設定されており、その属性マッピングを Adobe Unified Experience にコピーする場合は、「**マッピングを移行**」をクリックします。これらのマッピングは後で、破棄、削除または編集することができます。

   >[!NOTE]
   >
   >Adobe Unified Experience でマッピングを初めて設定する場合は、マッピングを移行することをお勧めします。後で再度移行しても害はありませんが、複数回移行する必要はありません。

1. 新しい属性マッピングを作成するには、「**マッピングを追加**」をクリックします。

1. Workfront フィールド名の横にある矢印をクリックし、マッピング先の [!DNL Workfront] フィールドを選択します。

1. （オプション）特定のフィールドに複数のルールを作成する場合は、「**常に**」の横にある矢印をクリックし、ルールで使用する演算子を選択します。

1. （条件付き）「常に」以外の演算子を選択した場合、その演算子を適用する Workfront フィールドと値を選択します。

   >[!NOTE]
   >
   >演算子 `Is Truthy` および `Is Falsy` には、値は不要です。

1. ID マネージャーの属性の値を Workfront フィールドに適用するか、特定の定数値を適用するかを選択します。

1. 適用する ID マネージャーフィールドの名前を入力するか、適用する定数値のテキストを入力します。

1. （オプション）同じ Workfront フィールドにさらにルールを追加するには、「**新規ルールを追加**」をクリックし、手順 4～9 に従います。

   >[!IMPORTANT]
   >
   > * 「常に」ルールより下のルールは無視されます。「常に」ルールがある場合は、そのルールをルールのリストの一番下に移動する必要があります。ルールの右側の 3 点メニューをクリックすると、リスト内でルールを上下に移動できます。
   > * リストの中央にルールを作成するには、新しいルールの上または下に配置するルールの横にある 3 点メニューをクリックし、「**上にルールを追加**」または「**下にルールを追加**」を選択します。

1. ルールを削除するには、削除するルールの横にある 3 点メニューをクリックし、「**削除**」を選択します。
1. マッピングを削除するには、そのマッピングのカード上にある&#x200B;**削除**&#x200B;アイコンをクリックします。

1. 保存するには、ページの上部までスクロールし、「**保存**」をクリックします。


