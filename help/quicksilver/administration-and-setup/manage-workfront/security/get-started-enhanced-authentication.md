---
title: 拡張認証の概要
description: 検索および左のナビゲーションで非表示
hidefromtoc: true
hide: true
feature: System Setup and Administration
role: Admin
exl-id: bf3c6c6f-ddd5-42d0-9efe-b5eb94549f85
source-git-commit: 50fa63474cfd40706e74507c3e4c231c1d97d463
workflow-type: tm+mt
source-wordcount: '580'
ht-degree: 3%

---

# 拡張認証の概要

<!-- enhanced authentication is no longer available for workfront customers -->

{{important-admin-console-onboard}}

Adobe Workfrontはユーザーとパスワードのシステム管理を変更しています。 これらの変更は、次の段階的リリースで公開されます。 **認証の強化** エクスペリエンス。 拡張認証により、すべてのWorkfront製品およびサービスにわたって、より一貫性のある安全なログインエクスペリエンスをユーザーに提供します。

次の表に、現在および将来の機能の詳細を示します。

>[!IMPORTANT]
>
>ほとんどのお客様は現在レガシー認証を使用しており、一部のお客様は拡張認証 1.0 を使用しています。
> 
>現在使用している認証の種類を確認するには、に移動します。 *your_domain*.my.workfront.com/login. /auth/login にリダイレクトされた場合は、Enhanced Authentication 1.0 を使用しています。
> 
>https://login-a-xx.workfront.com/にリダイレクトされる場合は、「xx」は、お使いの場所/プラットフォームに応じて米国（米国）、EU（ヨーロッパ）、GCP(Google Cloud Platform) のいずれかです。拡張認証 2.0 を使用しています。
>
>すべてのお客様は、2021 年末までに拡張認証 2.0 に移行します。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col data-mc-conditions=""> 
 <thead> 
  <tr> 
   <th> <p><strong>機能</strong> </p> </th> 
   <th><strong>従来の認証</strong> </th> 
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
   <td> <p>トレーニング、サポートなど、すべてのWorkfront製品およびサービスで 1 人のユーザー名を使用できるようにします</p> </td> 
   <td>利用不可</td> 
   <td> <p>利用不可</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Workfrontインスタンス間で同じ電子メールアドレスを使用することを許可</p> </td> 
   <td> <p>✓</p> <p>2019.3 リリース以降で利用可能</p> </td> 
   <td> <p>✓</p> <p>2019.3 リリース以降で利用可能</p> </td> 
   <td> <p>✓</p> <p>2019.3 リリース以降で利用可能</p> </td> 
  </tr> 
  <tr> 
   <td> <p>E メールアドレスでは大文字と小文字が区別されません</p> </td> 
   <td> <p>✓</p> <p>2019.3 リリース以降で利用可能</p> </td> 
   <td> <p>✓</p> <p>アドレスが大文字と小文字のみ異なる場合、複数のユーザーが同じ電子メールアドレスを持つことはできません。 </p> </td> 
   <td> <p>✓</p> <p>アドレスが大文字と小文字のみ異なる場合、複数のユーザーが同じ電子メールアドレスを持つことはできません。 </p> <p>Workfrontの管理者には、重複した電子メールアドレスの修正を開始するための 2019 年末の通知が届きます。</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>パスワード管理オプション</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>Workfront管理者としてのユーザーのパスワードリセット用電子メールを設定する</p> </td> 
   <td> <p>利用不可 </p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>ユーザーの一時パスワードをWorkfront管理者として設定する</p> </td> 
   <td> <p>✓</p> </td> 
   <td> <p>未計画</p> <p>この機能はセキュリティ上のベストプラクティスではありません</p> </td> 
   <td> <p>未計画</p> <p>この機能はセキュリティ上のベストプラクティスではありません</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>パスワードポリシーの要件</strong> </p> </td> 
   <td> <p> </p> </td> 
  </tr> 
  <tr> 
   <td> <p>特定の期間の経過後にパスワードをリセットするようユーザに要求する</p> </td> 
   <td>✓</td> 
   <td> <p>未計画</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>以前のパスワードを使用することを制限する </p> </td> 
   <td>✓</td> 
   <td>未計画 </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>パスワードの誤った入力試行から保護 </p> </td> 
   <td> <p>✓ </p> <p>パスワードの入力が 5 回正しく行われなかった場合に、アカウントをロックします。 ロックアウト後に必要な待機時間は、Workfront管理者が設定します</p> </td> 
   <td> <p>✓</p> <p>業界のベストプラクティスに基づいて、パスワードが連続して正しくない場合は待ち時間が急激に増加します。Workfrontの管理者は、必要な時間を設定できません</p> </td> 
   <td> <p>✓</p> <p>様々な疑わしい動作をプロアクティブにブロックするロックアウトアルゴリズムを使用します。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>小文字、大文字、数字、特殊文字を組み合わせる必要があります</p> </td> 
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
   <td> ✓ </td> 
   <td> <p> 非推奨</p> <p>Active Directory、Azure、LDAP の各システムでは、SAML 2.0 を使用する必要があります。</p> </td> 
   <td> <p>非推奨</p> <p>Active Directory、Azure、LDAP の各システムは、暗号化された SAML 2.0 または OpenID Connect を使用して構成できます。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>SAML 2.0 に準拠する SSO プロトコルをサポート </p> </td> 
   <td>✓</td> 
   <td> ✓ </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>オープン ID 接続プロトコルをサポート</p> </td> 
   <td> <p>利用不可</p> </td> 
   <td> <p>利用不可</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p> Workfrontログインページが常に ID プロバイダーのログインページにリダイレクトされるように設定する </p> </td> 
   <td> デフォルトで有効になっており、無効にできません</td> 
   <td> <p>✓</p> <p>Workfrontの管理者は、ログインページを設定して id プロバイダーのログインページにリダイレクトしたり、ログインボタン（複数可）を設定したりできます。</p> </td> 
   <td> <p>✓</p> <p> Workfrontの管理者は、ログインページを設定して id プロバイダーのログインページにリダイレクトしたり、ログインボタン（複数可）を設定したりできます。</p> </td> 
  </tr> 
  <tr> 
   <td> <p>各インスタンスで複数の SSO プロバイダーを有効にできます</p> </td> 
   <td> <p>該当なし</p> </td> 
   <td> <p>未計画</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td colspan="3"> <p><strong>環境のサポート</strong> </p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>プレビュー環境用の 1 人のユーザー名とパスワード</p> </td> 
   <td> <p>利用不可</p> </td> 
   <td> <p>利用不可</p> </td> 
   <td> <p>✓</p> </td> 
  </tr> 
  <tr> 
   <td> <p>サンドボックス環境用の単一のユーザー名とパスワード</p> </td> 
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
