---
title: 拡張認証の概要
description: 検索および左側のナビゲーションで非表示にする
hidefromtoc: true
hide: true
feature: System Setup and Administration
role: Admin
exl-id: bf3c6c6f-ddd5-42d0-9efe-b5eb94549f85
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: ht
source-wordcount: '580'
ht-degree: 100%

---

# 拡張認証の概要

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Adobe Workfront では、ユーザーとパスワードのシステム管理が変更されます。これらの変更は、**拡張認証**&#x200B;エクスペリエンスと呼ばれる段階的リリースで公開されます。拡張認証により、すべての Workfront 製品およびサービスで、一貫性と安全性の高いログインエクスペリエンスをユーザーに提供します。

次の表に、現在および将来の機能の詳細を示します。

>[!IMPORTANT]
>
>ほとんどの顧客は現在レガシー認証を使用していますが、拡張認証 1.0 を使用している顧客も一部存在します。
> 
>現在使用している認証の種類を確認するには、*your_domain*.my.workfront.com/login に移動します。ここで /auth/login にリダイレクトされる場合は、拡張認証 1.0 を使用しています。
> 
>https://login-a-xx.workfront.com/ にリダイレクトされる場合は、拡張認証 2.0 を使用しています。なお、「xx」には、お使いの場所やプラットフォームに応じて US（米国）、EU（ヨーロッパ）、GCP（Google Cloud Platform）のいずれかが入ります。
>
>すべてのお客様は、2021年末までに拡張認証 2.0 に移行します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p><strong>機能</strong> </p> </th> 
   <th><strong>レガシー認証</strong> </th> 
   <th><strong>拡張認証 1.0</strong> </th> 
   <th> <p>拡張認証 2.0</p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td colspan="3"> <p><strong>ログインオプション</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>1 件のユーザー名を、トレーニング、サポートなど、すべての Workfront 製品およびサービスで使用できるようにする</p> </td> 
   <td>利用不可</td> 
   <td> <p>利用不可</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Workfront インスタンス間で同じメールアドレスを使用することを許可</p> </td> 
   <td> <p>✓</p> <p>2019.3 リリース以降で利用可能</p> </td> 
   <td> <p>✓</p> <p>2019.3 リリース以降で利用可能</p> </td> 
   <td> <p>✓</p> <p>2019.3 リリース以降で利用可能</p> </td> 
  </tr> 
  <tr> 
   <td> <p>メールアドレスでは大文字と小文字が区別されない</p> </td> 
   <td> <p>✓</p> <p>2019.3 リリース以降で利用可能</p> </td> 
   <td> <p>✓</p> <p>複数のユーザーが、大文字と小文字の違いがあるだけで、あとは同じであるメールアドレスを使用することはできません。 </p> </td> 
   <td> <p>✓</p> <p>複数のユーザーが、大文字と小文字の違いがあるだけで、あとは同じであるメールアドレスを使用することはできません。 </p> <p>Workfront 管理者には、2019 年末頃に、重複するメールアドレスを修正を開始するよう通知されます。</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>パスワード管理オプション</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Workfront 管理者としてユーザーのパスワードリセット用メールを設定する</p> </td> 
   <td> <p>利用不可 </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Workfront 管理者としてユーザーの一時パスワードを設定する</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>予定なし</p> <p>この機能はセキュリティ上のベストプラクティスではありません</p> </td> 
   <td> <p>予定なし</p> <p>この機能はセキュリティ上のベストプラクティスではありません</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>パスワードポリシーの要件</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>特定の期間の経過後にパスワードをリセットするようユーザーに要求する</p> </td> 
   <td>✓</td> 
   <td> <p>予定なし</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>ユーザーが以前のパスワードを使用することを制限する </p> </td> 
   <td>✓</td> 
   <td>予定なし </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>誤ったパスワードの入力試行から保護 </p> </td> 
   <td> <p>✓ </p> <p>パスワードの入力が 5 回失敗した場合に、アカウントをロックします。ロック後に必要な待機時間は Workfront 管理者が設定する</p> </td> 
   <td> <p>✓</p> <p>業界のベストプラクティスに基づいて、誤ったパスワードを連続して入力すると待ち時間が急激に増加します。必要な待機時間は Workfront 管理者が設定する項目ではありません</p> </td> 
   <td> <p>✓</p> <p>さまざまな疑わしい行動をプロアクティブにブロックするロックアウトアルゴリズムを使用します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>小文字、大文字、数字および特殊文字を組み合わせる必要があります</p> </td> 
   <td>✓</td> 
   <td> <p>✓ </p> <p>特定の要件を選択する際の柔軟性の向上</p> </td> 
   <td> <p>✓</p> <p> 
     </p> </td> 
  </tr> 
  <tr> 
   <td> <p>パスワードの最小長を設定 </p> </td> 
   <td> 利用不可 </td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <!--
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td>Restrict users from using more than 2 identical characters in a row</td> 
    <td>Not available</td> 
    <td>Not available</td> 
    <td> <p>✓</p> </td> 
   </tr>
  --> 
  <tr> 
   <td colspan="3"> <p><strong>シングルサインオンプロトコルのサポート</strong></p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Active Directory および LDAP プロトコルに準拠する SSO 統合をサポート</p> </td> 
   <td> ✓</td> 
   <td> <p> 廃止</p> <p>Active Directory、Azure、LDAP の各システムでは、SAML 2.0 を使用する必要があります</p> </td> 
   <td> <p>廃止</p> <p>Active Directory、Azure、LDAP の各システムは、暗号化された SAML 2.0 または OpenID Connect を使用して設定できます。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>SAML 2.0 に準拠する SSO プロトコルをサポート</p> </td> 
   <td>✓</td> 
   <td> ✓</td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>OpenID Connect プロトコルをサポート</p> </td> 
   <td> <p>利用不可</p> </td> 
   <td> <p>利用不可</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p> 常に ID プロバイダーのログインページにリダイレクトされるように Workfront ログインページを設定 </p> </td> 
   <td> デフォルトで有効になっており、無効にできません</td> 
   <td> <p>✓</p> <p>Workfront 管理者は、ID プロバイダーのログインページにリダイレクトされるようにログインページを設定したり、ログインボタン（複数可）を設定したりできます。</p> </td> 
   <td> <p>✓</p> <p> Workfront 管理者は、ID プロバイダーのログインページにリダイレクトされるようにログインページを設定したり、ログインボタン（複数可）を設定したりできます。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>各インスタンスで複数の SSO プロバイダーを有効にできるようにする</p> </td> 
   <td> <p>該当なし</p> </td> 
   <td> <p>予定なし</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>環境のサポート</strong> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>プレビュー環境の単一のユーザー名とパスワード</p> </td> 
   <td> <p>利用不可</p> </td> 
   <td> <p>利用不可</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>サンドボックス環境の単一のユーザー名とパスワード</p> </td> 
   <td> <p>利用不可</p> </td> 
   <td> <p>利用不可</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <!--
   <tr> 
    <td> <p>Available for Production environments</p> </td> 
    <td>✓</td> 
    <td> ✓&nbsp;</td> 
    <td> <p>✓</p> </td> 
   </tr>
   <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
    <td> Available for Preview and Sandbox environments&nbsp;</td> 
    <td> ✓&nbsp;</td> 
    <td> ✓</td> 
    <td> <p>✓</p> </td> 
   </tr>
  --> 
 </tbody> 
</table>
