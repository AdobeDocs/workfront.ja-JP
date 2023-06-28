---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: システムセキュリティの環境設定の構成
description: Adobe Workfront管理者は、Workfrontシステムのセキュリティ環境設定を設定できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: 281712542566aec87c51a2eccb301dd3a83a94b3
workflow-type: tm+mt
source-wordcount: '747'
ht-degree: 3%

---

# システム環境設定の指定

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

{{important-admin-console-onboard}}

Adobe Workfront管理者は、Workfrontシステムの環境設定を設定できます。

* モバイルアプリやその他の統合アプリケーションからWorkfrontにアクセス
* iframe へのWorkfrontの埋め込みルール

システム環境設定で行った変更は、システム内のすべてのユーザーと、Workfrontでのユーザーのエクスペリエンスに影響します。

Workfrontの実装時にシステム環境設定を指定し、その後は再度設定することをお勧めします。

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

## システム環境設定を設定する

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **システム** > **環境設定**.

1. 組織の設定を指定するには、次のいずれかのフィールドを選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>の埋め込みを許可 <strong>Workfront</strong> iframe 内</p> </td> 
      <td>iframe にWorkfrontを埋め込むことができます。<p>このオプションはデフォルトでは無効になっています。</p><p><b>重要</b>:Web ベースのアプリケーションを iframe で表示すると、アプリケーションでクリックジャックのセキュリティ脆弱性の影響を受けやすくなります。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Office 365 アドインで SAML 2.0 認証を許可する</td> 
      <td> <p>Workfrontが SAML 2.0 シングルサインオンソリューションと統合されている場合、Workfrontを Office 365 アドイン用にのみ iframe に埋め込むことができます。 </p> <p>このオプションは、デフォルトで有効になっています。</p> <p><b>注意</b>:上記のオプションを有効にした場合、 <strong>iframe へのWorkfrontの埋め込みを許可</strong>、オプション <strong>Office 365 アドインで SAML 2.0 認証を許可する</strong> が有効になっていて、淡色表示になっている。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">外部ページの URL を作成する際にセッション情報を使用できるようにする</td> 
      <td> <p>ユーザーがダッシュボードに外部ページを追加する際に、サイトのセッション ID 情報を使用できるようにします。</p> <p>ダッシュボードへの外部ページの追加について詳しくは、 <a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">外部 Web ページをダッシュボードに埋め込む</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ユーザーがWorkfrontのモバイルアプリケーションと <strong>Workfront</strong> Outlook アドイン</td> 
      <td> <p>ユーザーがモバイルアプリ (iPadおよび携帯電話アプリ用のWorkfront View) およびWorkfront Outlook アプリにアクセスできるようにします。</p> <p>このオプションは、デフォルトで有効になっています。 </p> <p>Workfront View について詳しくは、 <a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Adobe Workfront View を使用</a>. モバイルアプリについて詳しくは、 <a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Adobe Workfrontモバイルアプリの使用</a>.</p> <p>Outlook プラグインの詳細については、「 <a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">Outlook 用のAdobe Workfrontのセットアップ</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>電子メールアドレスを使用して、Workfrontアカウントを持たないユーザーと共同作業する</p> </td> 
      <td>Workfrontのユーザーが、名前の代わりに電子メールアドレスを含めることで、Workfrontアカウントを持たないユーザーと特定の項目を共有できるようにします。 ユーザーは、電子メールアドレスを使用して、次の項目を外部ユーザーと共有できます。
       <ul>
        <li>ドキュメント<br></li>
        <li>ドキュメントリクエスト<br></li>
        <li>ドキュメントの承認</li>
        <li>カレンダー</li>
       </ul><p>このオプションは、デフォルトで有効になっています。</p> <p><b>重要</b>:このオプションが無効になっている場合、Workfrontインスタンスでは「外部ユーザー」アクセスレベルを使用できません。 詳しくは、 <a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">Workfrontの組み込みアクセスレベル</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">外部ユーザーにパスワードの登録を要求</td> 
      <td> <p>Workfrontで項目を表示するには、外部ユーザーが登録する必要があります。 デフォルトでは、このオプションは無効になっています。 このオプションを有効にすると、Workfrontアカウントを持たないユーザーが電子メールアドレスで特定の更新を受け取った場合、そのユーザーが含まれる項目を表示する前にアカウントの作成を求められます。 これにより、外部ユーザーアカウントが作成されます。</p> <p>このオプションはデフォルトでは無効になっています。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">次の場合にユーザーを自動的にログアウトする</td> 
      <td> 無操作状態が続いた後にユーザーがWorkfrontからログアウトする日時を指定できます。 デフォルトでは、ユーザーは 8 時間操作が実行されなかった場合にログアウトされます。 <p>このオプションは、シングルサインオンソリューションを使用しているWorkfrontのお客様にも影響します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">次の場合にモバイルユーザーを自動的にログアウトする：  </td> 
      <td>無操作状態が続いた後にユーザーがWorkfrontアプリケーションからログアウトする時間を指定できます。 デフォルトでは、ユーザーは 7 日間操作が実行されなかった場合にログアウトされます。 <p>このオプションは、シングルサインオンソリューションを使用しているWorkfrontのお客様にも影響します。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">システムのユーザーには、新しいホームエクスペリエンスがデフォルトで表示されます </td> 
      <td>ユーザーがデフォルトで新しいホームエクスペリエンスを表示するかどうかを指定できます。 いずれの場合も、ユーザーは、新しいホームの有効化または無効化を個別に選択できます。 このオプションは、デフォルトで有効になっています。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックします。

   ここで保存した変更は、Workfrontのすべてのユーザーと、外部ユーザーとして操作するすべてのユーザーのエクスペリエンスに影響します。
