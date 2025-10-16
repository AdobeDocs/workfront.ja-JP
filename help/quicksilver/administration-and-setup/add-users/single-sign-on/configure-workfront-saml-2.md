---
user-type: administrator
product-area: system-administration;setup
navigation-topic: single-sign-on-in-workfront
title: Adobe Workfront と SAML 2.0 の連携の設定
description: Adobe Workfront 管理者は、シングルサインオン（SSO）用の Security Assertion Markup Language（SAML）2.0 ソリューションと連携するように Workfront web アプリケーションおよびモバイルアプリケーションを設定できます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: cf09859c-7d6f-4bf0-9b7f-c57096233c94
source-git-commit: 22ae8b489c63ba6eea1472cf415f95e375a94773
workflow-type: tm+mt
source-wordcount: '1038'
ht-degree: 95%

---

# Adobe Workfront と SAML 2.0 の連携の設定

<!--
**DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.** </p>
-->

<!-- Audited: 12/2023 -->



>[!IMPORTANT]
>
>このページで説明する手順は、まだ Adobe Admin Console にオンボーディングされていない組織にのみ適用されます。
>
>Adobe Admin Consoleにオンボードされた組織内のユーザー属性をマッピングするには、「ユーザー属性のマッピング」の [Adobe統合エクスペリエンスでのユーザー属性のマッピング ](/help/quicksilver/administration-and-setup/add-users/create-and-manage-users/map-user-attributes.md#map-user-attributes-in-the-adobe-unified-experience) を参照してください。

Adobe Workfront 管理者は、シングルサインオン（SSO）用の Security Assertion Markup Language（SAML）2.0 ソリューションと連携するように Workfront web アプリケーションおよびモバイルアプリケーションを設定できます。

次の節の説明に従って、Workfront に SAML 2.0 を設定した後、[ID プロバイダーの SAML 2.0 メタデータの更新](../../../administration-and-setup/add-users/single-sign-on/update-saml-2-metadata-ip.md)の説明に従って設定を維持できます。

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
   <td> <p>Workfront 管理者である必要があります。</p> </p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## SAML 2.0 と連携する Workfront に対する認証の有効化

{{step-1-to-setup}}

1. **システム**／**シングルサインオン(SSO)** をクリックします。

1. **タイプ**&#x200B;のドロップダウンリストで、「**SAML 2.0.**」を選択します。

1. 表示されるオプションの上部付近にある「**SAML 2.0 メタデータのダウンロード**」をクリックして、お使いのコンピューターにファイルをダウンロードします。

   SAML 2.0 ID プロバイダーを利用するには、Workfront インスタンスで生成された情報を含んだ XML ファイルが必要です。ファイルをダウンロードした後、SAML 2.0 ID プロバイダーのサーバーにアクセスし、そこに Workfront SAML 2.0 メタデータ XML ファイルをアップロードする必要があります。

1. Workfront で次の情報を指定します。

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader">サービス プロバイダ ID </td>
      <td> この URL は既に入力されており、ID プロバイダーに対して Workfront を識別します。例：<code>&lt;yourcompany&gt;.com/SAML2</code></td>
     </tr>
     <tr>
      <td role="rowheader">バインド タイプ</span> </td>
      <td> <p>IDP サーバーでサポートされている、認証情報の送信方法を次の中から選択します。</p>
       <ul>
       <li>投稿する</li>
       <li>リダイレクト</li>
       </ul> </td>
     </tr>
     <tr>
      <td role="rowheader">IDプロバイダメタデータからフィールドを入力する </td> 
      <td>SAML 2.0 ID プロバイダーソリューションで、サービスプロバイダーメタデータ XML ファイルを書き出し、それをコンピューター上の一時的な場所に保存します。「<strong>ファイルの選択</strong>」を選択したあと、保存したファイルを見つけて選択し、Workfront 設定に追加します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ログイン ポータル URL</span> </td> 
      <td>組織の共通のログインポータルを入力します。これは、SAML 2.0 と統合されている Workfront アプリケーションおよびその他すべてのアプリケーションにアクセスするためにユーザーがログインする URL です。</td> 
     </tr>
     <tr>
      <td role="rowheader">サインアウト URL</span> </td> 
      <td> <p>IDP サーバーのログアウト URL を入力します。Workfront からログアウトする前に、Workfrontは この URL に HTTP リクエストを送信します。これにより、Workfront セッションが閉じると、リモートサーバー上のユーザーのセッションが閉じられます。</p> <p><b>メモ</b>：ユーザープロファイルで「<strong>SAML 2.0 認証のみを許可</strong>」オプションが有効になっている場合にのみ、ログアウト URL にリダイレクトされます。</p> </td>
     </tr>
     <tr>
      <td role="rowheader">パスワードの変更 URL </td> 
      <td> <p> パスワードを変更するためにユーザーがリダイレクトされる URL を指定します。 </p> <p>Workfront へのアクセスに SAML 2.0 資格情報が使用されるので、Workfront を通じてこのアクティビティを完了する代わりに、SAML 2.0 のパスワードを変更できるページにユーザーがリダイレクトされる必要があります。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">セキュア ハッシュ アルゴリズム </td> 
      <td> <p>IDP でサポートされているセキュアハッシュアルゴリズム（SHA）を次の中から選択します。</p> 
       <ul> 
       <li>SHA-1</li> 
       <li>SHA-256</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ユーザーを自動設定する</span> </td> 
      <td> <p>このオプションにより、新規ユーザーがディレクトリのユーザー名とパスワードを使用して初めて Workfront にログインしようとすると、システムにユーザーが自動的に作成されます。</p> <p>Workfront にユーザーを作成するには、Workfront データ属性をディレクトリプロバイダーの次のユーザーデータ属性とマッピングする必要があります。</p> 
       <ul> 
       <li>名</li> 
       <li>姓</li> 
       <li>メールアドレス</li> 
       </ul> 
       <p>このチェックボックスを選択すると、次のオプションが表示されます。</p> 
       <p> <img src="assets/saml-2.0-auto-provision-users-ui.png"> </p> 
       <p>マッピングする Workfront ユーザー属性をドロップダウンリストから選択し、ユーザーディレクトリにおける対応するディレクトリ属性を指定します。</p> 
       <p>「<strong>ディレクトリ属性</strong>」フィールドには、SAML 2.0 設定のテストに成功したときに保存したユーザー属性テーブルのディレクトリ属性名を指定する必要があります。</p> 
       <p>「<strong>デフォルト値</strong>」フィールドには、Workfront のデフォルト値を入力します。また、SAML 2.0 ID プロバイダーの値に基づいて、ルールを設定することもできます。</p> 
       <p><b>警告</b>：Workfront では、ユーザーがシステムにログインするたびに、以下に示す属性のマッピングを試みます。このため、アクセスレベルをマッピングすることはお勧めしません。属性が正しくマッピングされない場合は、管理アクセス権を容易に削除できます。「<strong>マッピングを追加</strong>」をクリックして、ルールを追加します。
       </p> 
       <p>次の Workfront 属性をマッピングできます。</p> 
      <ul> 
      <li> <p>アクセスレベル</p> </li> 
      <li> <p>住所</p> </li> 
      <li> <p>住所2</p> </li> 
      <li> <p>1時間当たりの請求</p> </li> 
      <li> <p>市区町村</p> </li> 
      <li> <p>会社</p> </li> 
      <li> <p>1時間当たりのコスト</p> </li> 
      <li> <p>メールアドレス</p> </li> 
      <li> <p>内線</p> </li> 
      <li> <p>名</p> </li> 
      <li> <p>ホーム グループ</p> </li> 
      <li> <p>ホーム チーム</p> </li> 
      <li> <p>担当業務</p> </li> 
      <li> <p>姓</p> </li> 
      <li> <p>レイアウトテンプレート</p> </li> 
      <li> <p>マネージャー</p> </li> 
      <li> <p>携帯電話</p> </li> 
      <li> <p>電話番号</p> </li> 
      <li> <p>郵便番号</p> </li> 
      <li> <p>スケジュール</p> </li> 
      <li> <p>状態</p> </li> 
      <li> <p>定期タイムシート</p> </li> 
      <li> <p>タイトル</p> </li> 
      </ul>
      <p>ユーザー属性のマッピングが終了したら、「<strong>保存</strong>」をクリックします。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">証明書 </td> 
      <td> <p>認証サービスと Workfront 間の安全な接続を確保するには、有効な SSL 証明書をアップロードします。OnDemand アカウントの場合は、証明書が常に必要です。この証明書は、SAML 2.0 システム管理者から取得できます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理の免除 </td> 
      <td> <p>Workfront 管理者が Workfront ログインを使用して Workfront にアクセスできるようにします。このオプションを選択しない場合、Workfront 管理者は SAML 2.0 のユーザー名とパスワードを使用する必要があります。</p> 
      <p>Workfront システム管理者のアクセスレベルを持つユーザーの場合、Workfront は、まず SAML 2.0 を使用して Workfront へのログインを試みます。SAML 2.0 認証が失敗した場合、Workfront は Workfront 管理者のローカル認証を使用します。</p> 
      <p>SAML 2.0 プロバイダーが一時的に使用できなくなった場合でも Workfront 管理者が Workfront にログインできるように、このオプションを常に選択しておくことをお勧めします。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">有効にする </td> 
      <td> <p>Workfront システムで SSO をアクティブ化します。ログイン手順がユーザーに伝わっていることを確認します。</p> <p>Workfront で SSO 設定を有効にした後、<strong>SAML 2.0 認証のみを許可</strong>設定をすべてのユーザーに対して有効にして、SSO を使用できるようにします。</p> <p>SSO のユーザーのアップデートについて詳しくは、<a href="../../../administration-and-setup/add-users/single-sign-on/update-users-sso.md" class="MCXref xref">シングルサインオンのユーザーをアップデート</a>を参照してください。</p> <p>ユーザー設定に関して詳しくは、<a href="../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md" class="MCXref xref">ユーザーのプロファイルの編集</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">構成の確認 </td> 
      <td> 
      <p>「<strong>接続をテスト</strong>」をクリックして、Workfront と SAML 2.0 ID プロバイダーが互いに通信できることを確認します。この接続は、XML ファイルを交換した場合にのみ成功します。
      </p> 
      <p>SAML 2.0 ID プロバイダーと Workfront 間のリンクのテストが成功すると、以下のような画面が表示されます。</p>
      <p><b>メモ</b>：この画面はブラウザーのポップアップに表示されるので、ブラウザーでポップアップブロッカーを無効にします。</p>
      <p>表に示される情報を保存して、後で使用できるようにします。</p>
      <p><img src="assets/success-table-saml-2.png"></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックして SAML 2.0 設定を保存します。
