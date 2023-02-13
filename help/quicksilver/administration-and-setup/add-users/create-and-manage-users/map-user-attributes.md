---
user-type: administrator
content-type: tips-tricks-troubleshooting
product-area: system-administration;user-management
navigation-topic: create-and-manage-users
title: ユーザー属性のマッピングと新しいユーザーの自動プロビジョニング
description: シングルサインオン (SSO) を使用して、ID プロバイダーの Active Directory からAdobe Workfrontユーザーに属性を渡すことができます。 また、自動プロビジョニングオプション（ジャストインタイムプロビジョニングまたは JIT とも呼ばれます）を使用して、新しいユーザーをWorkfrontに追加することもできます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 3d523584-dcb8-4aa6-8217-611f22dc1450
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '563'
ht-degree: 3%

---

# ユーザー属性のマッピングと新しいユーザーの自動プロビジョニング

シングルサインオン (SSO) を使用して、ID プロバイダーの Active Directory からAdobe Workfrontユーザーに属性を渡すことができます。 また、自動プロビジョニングオプション（ジャストインタイムプロビジョニングまたは JIT とも呼ばれます）を使用して、新しいユーザーをWorkfrontに追加することもできます。

>[!NOTE]
>
>組織がAdobe Admin Consoleにオンボーディングされている場合は、この機能を使用できません。 詳細については、ネットワークまたは IT 管理者にお問い合わせください。


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

## 属性のマッピングに関するヒント

属性をマッピングする際は、次の点に注意してください。

* 必ず、プレビューサンドボックスまたは顧客更新 (CR) サンドボックスでテストしてください。
* 管理者アカウントと非管理者アカウントの両方でテストし、属性が正しくマッピングされていることを確認します。
* 属性は、ユーザーが自動プロビジョニング中だけでなく、SSO 経由でWorkfrontにサインインするたびにマッピングされます。

## ユーザー属性のマッピングと新しいユーザーの自動プロビジョニング

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **システム** > **シングルサインオン (SSO)**.

1. 内 **タイプ** ドロップダウンで、 **SAML 2.0**.

1. クリック **ユーザ属性をマッピング**.

   ![](assets/map-user-attributes.png)

1. （オプション）Workfrontで Active Directory から新しいユーザーを自動的に作成する場合は、 **ユーザーの自動プロビジョニング**.

   この機能には属性マッピングが必要です。

1. 表示されるオプションの行で、Workfrontユーザーに必要な属性をマッピングします。

   住所、マネージャ、職務の役割、ホームグループなどの属性をマッピングできます。

   属性マッピングは 1:1 の比率で機能します。 例えば、ユーザーが属するすべてのグループを設定することはできません。1 人のユーザーにつき 1 つのみ設定できます。

   >[!IMPORTANT]
   >
   >各ユーザーには、次の属性が必要です。
   >      
   >* 名
   >* 姓
   >* E メール アドレス

   >      
   >属性マッピングでアクセスレベルをマッピングすることはお勧めしません。 その場合は、デフォルト値を設定する際に、誤って管理者アクセスを削除しないように注意してください。

   次の表に、属性のマッピングに使用できるフィールドを示します。

   <table style="table-layout:auto"> 
    <col data-mc-conditions=""> 
    <col data-mc-conditions=""> 
    <tbody> 
     <tr> 
      <td role="rowheader">Workfront ユーザー属性</td> 
      <td>マッピングする属性の名前を選択します</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ディレクトリの属性</td> 
      <td>使用する SSO 属性ラベルを入力します。/td&gt; 
     </tr> 
     <tr> 
      <td role="rowheader">既定値</td> 
      <td> <p>Workfrontユーザー属性を選択した後、接続中に値が NULL の場合、このフィールドはシステムの対応するデフォルト値で入力されます。 属性マッピングルールを適用する場合にのみ、ここに値を入力します（手順 7 を参照）。 デフォルト値は、これらのルールの例外として機能します。</td> 
     </tr> 
    </tbody> 
   </table>

1. （オプション）「 **ルール** をクリックして、属性にルールを追加します。

   1. ドロップダウンで、使用する属性修飾子を選択します。
   1. 右側の 2 つのフィールドに、ディレクトリ属性値と、置き換える値を入力します。

      ![](assets/rule-fields.png)
   次をクリックできます。 **ルールを追加** をクリックして、属性にルールを追加します。

1. （オプション）さらにユーザー属性をマッピングするには、 **マッピングを追加** 手順 6～7 を繰り返します。
1. 「**保存**」をクリックします。
