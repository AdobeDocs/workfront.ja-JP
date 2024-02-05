---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: 認証用のパスワードポリシーの設定
description: Adobe Workfront 管理者は、パスワードポリシーオプションを設定すると、Workfront システムの認証操作をカスタマイズできます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 7832986b-a5e8-4f14-8802-d3b8e32b14bc
source-git-commit: 970cc86b00dc1afe0473ac3a387e7ce47e4a2433
workflow-type: tm+mt
source-wordcount: '724'
ht-degree: 95%

---

# 認証用のパスワードポリシーの設定

{{important-admin-console-onboard}}

Adobe Workfront 管理者は、パスワードポリシーオプションを設定すると、Workfront システムの認証操作をカスタマイズできます。

Workfront の実装時に認証環境設定を指定し、後で再度アクセスすることをお勧めします。

改善されたパスワード管理機能は、近日中に提供される予定です。または、組織で既にご利用いただける可能性もあります。組織が新しい認証操作にアクセスできるかどうかに応じて、次の節のいずれかを使用してください。

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
   <td>プラン</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p> <p><b>メモ</b>：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

## 認証を設定（すべての顧客が利用可能） {#configure-authentication-available-for-all-customers}

すべての顧客に対して認証オプションが表示されます。パスワード管理機能の向上は、近日中に提供される予定です。または、組織で既に利用可能になっている可能性もあります (「 [（拡張認証の設定）](#configure-enhanced-authentication-coming-soon) 」を参照してください。

認証環境設定を行うには、次の手順に従います。

1. Adobe Workfront の右上隅で、**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、「**設定** ![](assets/gear-icon-settings.png)」の順にクリックします。

1. **システム**／**認証**&#x200B;をクリックします。

1. 次のいずれかのフィールドを選択して、組織の認証設定を確立します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><em>&lt;value&gt;</em> 日ごとにパスワードをリセットするようユーザーを強制する</td> 
      <td>これにより、ユーザーが Workfront のパスワードをリセットする時間枠が設定されます。デフォルトでは、このオプションは無効になっています。有効にすると、30、60、90、120、180 日から選択できます。デフォルトは 30 日です。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ユーザーが過去に設定した <em>&lt;value&gt;</em> つのパスワードと同じパスワードを設定できないようにする</td> 
      <td> <p>このフィールドでは、設定されたリセット数に対してユーザーがパスワードを再利用することを禁止します。デフォルトでは、このフィールドは無効になっています。有効にすると、パスワードを再利用できるようになるまでに、この値を 5、10、15 のリセット数に設定できます。</p> <p>このオプションを選択すると、ユーザーは 1 日に複数回パスワードをリセットできません</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">間違ったパスワードを 5 回連続して入力した場合、アカウントを <em>&lt;value&gt;</em> 分間ロックする。 </td> 
      <td> <p>間違ったパスワードを 5 回連続して入力した場合に、ユーザーが Workfront からロックアウトされる期間を選択します。デフォルトでこのオプションは有効になっており、待機時間は 10 分です。アカウントは、10 分、30 分、1 時間、8 時間、24 時間ロックできます。 </p> <p>ユーザーのパスワードを手動でリセットすると、このデフォルトの待機値が上書きされます。<br>ユーザーは、ログイン画面からロックアウトされると、自分のパスワードをリセットできます。パスワードを忘れた場合にパスワードをリセットする方法について詳しくは、<a href="../../../workfront-basics/manage-your-account-and-profile/managing-your-workfront-account/reset-your-password.md" class="MCXref xref">パスワードをリセットする</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">パスワードには少なくとも <em>&lt;value&gt;</em> 種類の文字を含める必要がある。</td> 
      <td> <p>パスワードに必要な様々な種類の文字の数を選択できるようにすることで、ユーザーのパスワードの強度を決定します。</p> <p>認識可能な辞書の単語は、パスワードとして使用できません。<br>デフォルトの Workfront では、次の文字のうち少なくとも 2 つがパスワードに存在する必要があります（有効なパスワードには、これらの文字のうち 3 つが必要になる場合もあります）。 </p> 
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

この節では、組織でまだ使用できない可能性のある、拡張認証エクスペリエンスについて説明します。組織が新しい認証エクスペリエンスに移行していない場合は、[認証を設定（すべての顧客が利用可能）](#configure-authentication-available-for-all-customers)の説明に従って認証設定を行う必要があります。

拡張認証環境設定を行うには、次の手順に従います。

1. Adobe Workfront の右上隅にある&#x200B;**メインメニュー**&#x200B;アイコン ![](assets/main-menu-icon.png)、**設定** ![](assets/gear-icon-settings.png) の順にクリックします。

1. **システム**／**拡張認証**&#x200B;をクリックします。
1. 「**パスワードの長さ**」ボックスに、有効なパスワードに必要な最小文字数を入力します。

   Workfront には 6 文字以上必要です。

1. （オプション）「**パスワード要件**」セクションで、ユーザーパスワードに必要な文字の種類を選択します。

   「パスワード要件」セクションの任意の種類またはすべての文字を必要とすることで、ユーザーパスワードの強度を高めることができます。次のオプションを使用できます。

   | 小文字 | 少なくとも小文字が 1 文字必要です |
   |---|---|
   | 大文字 | 少なくとも大文字が 1 文字必要です |
   | 数字 | 少なくとも数字が 1 つ必要です |
   | 特殊文字 | 少なくとも特殊文字が 1 つ必要です |

   {style="table-layout:auto"}

1. 「**保存**」をクリックします。
