---
user-type: administrator
product-area: system-administration;user-management;setup
navigation-topic: security
title: システム環境設定の指定
description: Adobe Workfront管理者は、セキュリティの環境設定など、Workfront システムの環境設定を指定できます。
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: f92ceed7-b191-425b-9fff-1b0947f32db8
source-git-commit: 6b93a6d7830d644520c38aa6010cd7df18c5a667
workflow-type: tm+mt
source-wordcount: '832'
ht-degree: 61%

---

# システム環境設定を指定

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>
-->

<!--Audited: 05/2024-->

<span class="preview">このページでハイライト表示されている情報は、まだ一般に利用できない機能を示します。すべてのお客様が、プレビュー環境でのみ使用できます。 実稼動環境への毎月のリリースの後、迅速なリリースを有効にしたお客様には、実稼動環境でも同じ機能を利用できます。</span>

<span class="preview">迅速リリースについて詳しくは、[組織での迅速リリースを有効または無効にする](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md)を参照してください。</span>

{{important-admin-console-onboard}}

Adobe Workfront管理者は、次のようなWorkfront システムの環境設定を行うことができます。

* モバイルアプリやその他の統合アプリケーションから Workfront にアクセス
* Iframe への Workfront の埋め込みルール

システム環境設定で行った変更は、システム内のすべてのユーザーと、Workfront でのユーザーのエクスペリエンスに影響します。

Workfront の実装中にシステム環境設定を指定し、後で再度アクセスすることをお勧めします。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

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
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td><p>新規：標準</p>
   <p>または</p>
   <p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p></td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## システム環境設定を指定

{{step-1-to-setup}}

1. 左側のパネルで、**システム**／**環境設定**&#x200B;をクリックします。

1. 組織の設定を確定するには、以下のフィールドのいずれかを選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>迅速リリースプロセスを有効にする</p> </td> 
      <td>四半期ごとのリリースの代わりに、組織の毎月の Workfront リリースを有効にできます。</p><p>迅速リリースプロセスについて詳しくは、<a href="/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md" class="MCXref xref">組織での迅速リリースを有効化または無効化</a>を参照してください。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>iframe へのWorkfrontの埋め込みを許可</p> </td> 
      <td>Iframe に Workfront を埋め込むことができます。<p>このオプションはデフォルトでは無効になっています。</p><p><b>重要</b>：Iframe で web ベースのアプリケーションを表示すると、アプリケーションでクリックジャックのセキュリティの脆弱性の問題が生じやすくなります。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Office 365 アドインで SAML 2.0 認証を許可する</td> 
      <td> <p>Workfrontが SAML 2.0 シングルサインオンソリューションと統合されている場合、Workfront を Office 365 アドイン用にのみ Iframe に埋め込むことができます。 </p> <p>このオプションは、デフォルトで有効になっています。</p> <p><b>メモ</b>：上記のオプション「<strong>Iframe への Workfront の埋め込みを許可</strong>」を有効にする場合、オプション「<strong>Office 365 アドインでの SAML 2.0 認証を許可</strong>」が有効になり、グレー表示になります。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">外部ページ URL を作成する際に、セッション情報の使用を有効にします。</td> 
      <td> <p>ユーザーがダッシュボードに外部ページを追加する際に、ユーザーがサイトのセッション ID 情報を使用できるようにします。</p> <p>このオプションは安全ではなく、デフォルトでオフになっています。統合には、代わりに OAuth を使用することをお勧めします。</p> <p>ダッシュボードへの外部ページの追加について詳しくは、<a href="../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md" class="MCXref xref">外部 web ページをダッシュボードに埋め込み</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Workfrontのモバイル アプリケーションとWorkfront Outlook アドインを使わせる</td> 
      <td> <p>ユーザーがモバイルアプリ（iPad 用 Workfront View および携帯電話アプリ）および Workfront Outlook アプリにアクセスできるようにします。</p> <p>このオプションは、デフォルトで有効になっています。 </p> <p>Workfront View について詳しくは、<a href="../../../workfront-basics/mobile-apps/using-workfront-view/use-workfront-view.md" class="MCXref xref">Adobe Workfront View を使用</a>を参照してください。モバイルアプリについて詳しくは、<a href="../../../workfront-basics/mobile-apps/using-the-workfront-mobile-app/use-the-mobile-app.md" class="MCXref xref">Adobe Workfront モバイルアプリの使用：記事インデックス </a> を参照してください。</p> <p>Outlook プラグインについて詳しくは、<a href="../../../workfront-integrations-and-apps/using-workfront-with-outlook/set-up-workfront-for-outlook.md" class="MCXref xref">Adobe Workfront を Outlook 用に設定</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>メールアドレスを使用して、Workfront アカウントを持たないユーザーと共同作業</p> </td> 
      <td>Workfront ユーザーは、名前の代わりにメールアドレスを含めることにより、Workfront アカウントを持たないユーザーと特定の項目を共有できます。ユーザーは、メールアドレスを使用して、以下の項目を外部ユーザーと共有できます。
       <ul>
        <li>ドキュメント<br></li>
        <li>ドキュメントリクエスト<br></li>
        <li>ドキュメントの承認</li>
        <li>カレンダー</li>
       </ul><p>このオプションは、デフォルトで有効になっています。</p> <p><b>重要</b>：このオプションが無効になっている場合、外部ユーザーアクセスレベルは、Workfront インスタンスでは使用できません。詳しくは、<a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/default-access-levels-in-workfront.md" class="MCXref xref">ビルトインのアクセスレベル</a>を参照してください。</p> </td> 
     </tr> 
     <!--<tr> 
      <td role="rowheader">Require external users to register with a password</td> 
      <td> <p>Requires external users to register before they are able to view items in Workfront. By default, this option is disabled. When you enable this option, people without a Workfront account who are included in certain updates by their email address, will be prompted to create an account before they can view the item they are included on. This creates an External User account for them.</p> <p>This option is disabled by default.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log users out after</td> 
      <td> Lets you specify when a user is logged out of Workfront, after a period of inactivity. By default, users are logged out after 8 hours of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Automatically log mobile users out after </td> 
      <td>Lets you specify when a user is logged out of the Workfront application, after a period of inactivity. By default, users are logged out after 7 days of inactivity. <p>This option also affects Workfront customers who are using a single sign-on solution.</p> <p>This setting is not available to organizations that have been migrated to Adobe IMS.</p></td> 
     </tr> -->
     <tr> 
      <td role="rowheader">ヘルプ URL</td> 
      <td>メインメニューヘルプアイコンの移動先の内部カスタムヘルプサイトを定義できます。 詳しくは、<a href="/help/quicksilver/administration-and-setup/customize-workfront/brand-workfront/configure-custom-help-url.md"> カスタムヘルプ URL の設定 </a> を参照してください。</p></td> 
     </tr>
     <tr> 
      <td role="rowheader">優先度ワークリストを有効にする </td> 
      <td>ユーザーの優先度ワークリストのエクスペリエンスを有効または無効にすることを選択できます。 Workfrontには引き続き「優先度」アイコンが表示されますが、機能にはアクセスできません。 優先度の詳細については、「<a href="/help/quicksilver/administration-and-setup/set-up-workfront/workfront-testing-environments/wf-preview-sandbox-environment.md"> 優先度の概要 </a> を参照してください。</td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">AI を有効にする </span> </td> 
      <td><span class="preview">AI アシスタントを含む AI を有効にすることを選択できます。 <p><b> メモ </b>:AI を有効にするには、組織が特定の要件を満たす必要があります。 要件を含む、AI について詳しくは、<a href="/help/quicksilver/workfront-basics/ai-assistant/ai-assistant-overview.md">AI アシスタントの概要 </a> を参照してください。</p></span></td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">フォームのオートコンプリート </span></td> 
      <td><span class="preview">以前のリクエストデータに基づいてリクエストフォームをオートコンプリートする機能を有効にするかどうかを選択できます。 フォームのオートコンプリートについて詳しくは、<a href="/help/quicksilver/manage-work/requests/create-requests/autofill-suggestions-from-previous.md"> 以前のデータからのリクエストの自動入力 </a> を参照してください。</span></td> 
     </tr>
     <tr> 
      <td role="rowheader"><span class="preview">AI ベータ版のオプトイン </span></td> 
      <td><span class="preview">現在Betaにある AI 機能を有効にすることができます。 このオプションを有効にした場合、有効にする AI Beta機能を選択できます。 各 AI Beta機能について詳しくは、その機能の横にある情報アイコンをクリックしてください。</span></td> 
     </tr>
     <tr> 
      <td role="rowheader">テスト環境</td> 
      <td>Workfront テスト環境にアクセスできます。 詳しくは、<a href="/help/quicksilver/workfront-basics/priorities/get-started-with-priorities.md">Adobe Workfront のプレビューサンドボックス環境</a>を参照してください。</p></td> 
    </tbody> 
   </table>

1. **保存**&#x200B;をクリックします。

   ここで保存した変更は、Workfrontのすべてのユーザーおよび外部ユーザーとしてシステムを操作するすべてのユーザーのエクスペリエンスに影響を与えます。
