---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: 認証用のパスワードポリシーの設定
description: Adobe Workfront管理者は、パスワードポリシーオプションを設定して、Workfrontシステムに対する認証操作をカスタマイズできます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7832986b-a5e8-4f14-8802-d3b8e32b14bc
source-git-commit: 970cc86b00dc1afe0473ac3a387e7ce47e4a2433
workflow-type: tm+mt
source-wordcount: '706'
ht-degree: 1%

---

# 認証用のパスワードポリシーの設定

{{important-admin-console-onboard}}

Adobe Workfront管理者は、パスワードポリシーオプションを設定して、Workfrontシステムに対する認証操作をカスタマイズできます。

Workfrontの実装時に認証環境設定を指定し、後で再度アクセスすることをお勧めします。

パスワード管理機能の向上は、近日中に提供される予定です。また、既にご利用いただける可能性もあります。 組織が新しい認証エクスペリエンスにアクセスできるかどうかに応じて、次のセクションのいずれかを使用します。

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
   <td> <p>Workfront管理者である。</p> <p><b>注意</b>：まだアクセス権がない場合は、Workfront管理者に問い合わせて、アクセスレベルに追加の制限が設定されているかどうかを確認してください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 認証を設定（すべてのお客様が利用可能） {#configure-authentication-available-for-all-customers}

すべての顧客の認証オプションが表示されます。 パスワード管理機能の向上は、近日中に提供される予定です。または、組織で既に利用可能になっている可能性もあります (「 [（拡張認証の設定）](#configure-enhanced-authentication-coming-soon) 」を参照してください。

認証環境設定を構成するには、次の手順に従います。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **システム** > **認証**.

1. 組織の認証設定を確立するには、次のいずれかのフィールドを選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">次の間隔でユーザーにパスワードのリセットを強制 <em>&lt;value&gt;</em> 日</td> 
      <td>これにより、ユーザーがWorkfrontのパスワードをリセットする時間枠が設定されます。 デフォルトでは、このオプションは無効になっています。 有効にした場合は、30 日、60 日、90 日、120 日、180 日の間を選択できます。 デフォルトは 30 日です。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">以前のパスワードと同じパスワードをユーザーに設定しない <em>&lt;value&gt;</em> パスワード</td> 
      <td> <p>このフィールドでは、設定された数のリセットに対してユーザーがパスワードを再利用することを禁止します。 デフォルトでは、このフィールドは無効になっています。 有効にした場合、この値を 5、10 または 15 に設定すると、パスワードを再利用できるようになります。</p> <p>このオプションを選択した場合、ユーザーは指定した日に複数回パスワードをリセットできません</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">間違ったパスワードが 5 回連続して入力された場合は、次の項目でアカウントをロックします： <em>&lt;value&gt;</em> 分： </td> 
      <td> <p>誤ったパスワードを 5 回連続して入力した後、ユーザーがWorkfrontからロックアウトされる期間を選択します。 デフォルトでは、このオプションは有効になっており、待機時間は 10 分です。 アカウントは、10 分、30 分、1 時間、8 時間、24 時間の間、ロックできます。 </p> <p>ユーザーのパスワードを手動でリセットすると、このデフォルトの待機値が上書きされます。 <br>ユーザーは、ログイン画面からロックアウトされたときに、自分のパスワードをリセットできます。 パスワードを忘れた場合に、パスワードをリセットする方法について詳しくは、 <a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">パスワードをリセット</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">パスワードには少なくとも次を含める必要があります <em>&lt;value&gt;</em> 様々なタイプの文字：</td> 
      <td> <p>パスワードに必要なさまざまな種類の文字の数を選択できるようにすることで、ユーザーのパスワードの強度を決定します。</p> <p>認識可能な辞書の単語は、パスワードとして使用できません。<br>デフォルトでは、Workfrontでは、次の文字のうち少なくとも 2 つがパスワードに存在する必要があります（有効なパスワードには、これらの文字のうち 3 つが必要になる場合もあります）。 </p> 
       <ul> 
        <li>大文字</li> 
        <li>小文字</li> 
        <li>数字</li> 
        <li>シンボル</li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックします。

## 拡張認証の設定{#configure-enhanced-authentication-coming-soon}

この節では、組織でまだ使用できない可能性のある、拡張認証エクスペリエンスについて説明します。 組織が新しい認証エクスペリエンスに移行されていない場合は、認証設定を設定する必要があります。詳しくは、 [認証を設定（すべてのお客様が利用可能）](#configure-authentication-available-for-all-customers).

拡張認証環境設定を構成するには、次の手順に従います。

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. クリック **システム** > **認証の強化**.
1. Adobe Analytics の **パスワードの長さ** ボックスに、有効なパスワードに必要な最小文字数を入力します。

   Workfrontには 6 文字以上必要です。

1. （オプション） **パスワード要件** 」セクションで、ユーザーパスワードに必要な文字の種類を選択します。

   「パスワード要件」セクションの任意の種類またはすべての文字を必要とすることで、ユーザーパスワードの強度を高めることができます。 次のオプションを使用できます。

   | 小文字 | 少なくとも 1 文字の小文字を必要とします |
   |---|---|
   | 大文字 | 大文字を少なくとも 1 文字必要です |
   | 数字 | 少なくとも 1 つの数字が必要です |
   | 特殊文字 | 1 文字以上の特殊文字が必要です |

   {style="table-layout:auto"}

1. 「**保存**」をクリックします。
