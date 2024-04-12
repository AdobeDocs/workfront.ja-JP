---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: ユーザー属性を割り当て
description: シングルサインオン（SSO）を使用して、ID プロバイダーの Active Directory から Adobe Workfront ユーザーに属性を渡すことができます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 3d523584-dcb8-4aa6-8217-611f22dc1450
source-git-commit: 20f9e9468c85235c0afadfee4d925a796ff89c54
workflow-type: tm+mt
source-wordcount: '952'
ht-degree: 100%

---

# ユーザー属性を割り当て

<!--Audited 2/2024-->

シングルサインオン（SSO）を使用して、ID プロバイダーの Active Directory から Adobe Workfront ユーザーに属性を渡すことができます。

## アクセス要件

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
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td><p>新規：標準</p><p>または</p><p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

## 属性のマッピングに関するヒント

属性をマッピングする際は、次の点に留意してください。

* 必ず、プレビューサンドボックスまたはCustomer Refresh（CR）サンドボックスでテストしてください。
* 管理者アカウントと非管理者アカウントの両方でテストして、属性が正しくマッピングされていることを確認します。
* マッピングされた属性は、ユーザーがシングルサインオンでログインするたびに適用されます。

  例：「姓」をマッピングし、ID プロバイダーの値を更新せずに Workfront で名前を更新すると、次回ユーザーがサインインしたときに、ID プロバイダー内の値と一致するように姓が上書きされます。

## 組織のユーザー属性のマッピング

属性をマッピングする手順は、組織が Adobe Unified Experience を使用しているかどうかによって異なります。

組織が Adobe Unified Experience を使用しているかどうかを判断するには、Workfront へのアクセスに使用する URL を調べます。

| URL | Adobe Experience |
|---|---|
| (CompanyName).my.workfront.com | 従来のエクスペリエンス |
| experience.adobe.com | Adobe Unified Experience |

* [従来のエクスペリエンスでユーザー属性をマッピング](#map-user-attributes-in-the-classic-experience)
* [Adobe Unified Experience でユーザー属性をマッピング](#map-user-attributes-in-the-adobe-unified-experience)

### 従来のエクスペリエンスでユーザー属性をマッピング

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、**設定** ![](assets/gear-icon-settings.png) の順にクリックします。

1. **システム**／**シングルサインオン(SSO)** をクリックします。

1. **タイプ**&#x200B;ドロップダウンリストで、「**SAML 2.0**」をクリックします。

1. 「**ユーザー属性の割り当て**」をクリックします。

   ![](assets/map-user-attributes.png)

1. 表示されるオプションの行で、必要な属性を Workfront ユーザーにマッピングします。

   住所、マネージャー、担当業務、ホームグループなどの属性をマッピングできます。

   属性マッピングは 1:1 の比率で機能します。例えば、ユーザーが所属するすべてのグループを設定することはできず、設定できるのは 1 人のユーザーにつき 1 つのみです。

   >[!IMPORTANT]
   >
   >属性マッピングでアクセスレベルをマッピングすることはお勧めしません。それを行う場合は、デフォルト値を設定する際に、管理者アクセス権を誤って削除しないように注意してください。

   属性のマッピングに使用できるフィールドを次の表に示します。

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader">Workfront ユーザー属性</td> 
      <td>マッピングする属性の名前を選択します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ディレクトリの属性</td> 
      <td>使用する SSO 属性ラベルを入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">既定値</td> 
      <td> <p>「Workfront ユーザー属性」を選択した後、接続中に値が NULL の場合、このフィールドはシステムの対応するデフォルト値が入力されます。属性マッピングルールを適用する場合にのみ、ここに値を入力します（手順 7 を参照）。デフォルト値は、これらのルールの例外として機能します。</td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）「**ルール**」をクリックして、属性にルールを追加します。

   1. ドロップダウンで、使用する属性修飾子を選択します。
   1. 右側の 2 つのフィールドに、ディレクトリ属性値と、置き換える値を入力します。

      ![](assets/rule-fields.png)

   「**ルールを追加**」をクリックして、属性にルールを追加します。

1. （オプション）さらにユーザー属性をマッピングするには、「**マッピングを追加**」をクリックして、手順 6～7 を繰り返します。
1. 「**保存**」をクリックします。

### Adobe Unified Experience でユーザー属性をマッピング

1. Adobe Workfront の左上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-left.png) をクリックし、続いて&#x200B;**設定**&#x200B;アイコン ![](assets/gear-icon-settings.png) をクリックします。

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


