---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: システムの基本情報の設定
description: Adobe Workfront システムの設定の一環として、顧客情報ページの「基本情報」セクションで、組織に関する詳細を管理できます。
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: bad5e700-79a6-49ed-bcf9-f0b5b3eaa909
source-git-commit: 5f11e6ccda9fa3b37ec1300edb8f322521013a52
workflow-type: tm+mt
source-wordcount: '821'
ht-degree: 99%

---

# システムの基本情報の設定

<!-- Audited: 2/2024 -->

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>-->

Adobe Workfront システムの設定の一環として、顧客情報ページの「基本情報」セクションで、組織に関する詳細を管理できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>任意</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td>
   <p>新規：標準</p>
   または
   <p>現在：プラン</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>Workfront 管理者である必要があります。</p></td> 
  </tr> 
 </tbody> 
</table>

## 顧客情報にアクセス

顧客は、組織の Workfront インスタンスを表します。このエリアのオプションは、Workfront をご利用のお客様に固有です。

顧客情報ページにアクセスするには：

{{step-1-to-setup}}

1. 左側のパネルで、**システム**／**顧客情報**&#x200B;をクリックします。

   購入した Workfront プランによっては、一部のセクションが顧客情報ページに表示されない場合があります。組織で使用する Workfron tプランを確認する必要がある場合は、アカウント担当者にお問い合わせください。

   顧客情報エリアには、次のセクションがあります。

   * **基本情報**

     Workfront での基本情報の設定について詳しくは、[基本情報の設定](#configure-basic-info)を参照してください。

   * **API キー設定**

     API キーの設定について詳しくは、[API キーの管理](../../administration-and-setup/manage-workfront/security/manage-api-keys.md)を参照してください。

   * **IP 許可リスト**

     ユーザーが Workfront にアクセスするために許可リストに IP アドレスを追加する方法については、[ファイアウォールの許可リストの設定](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md)を参照してください。

   * **ライセンス**

     ライセンスについて詳しくは、[システムで使用可能なライセンスの管理](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md)を参照してください。

## 基本情報の設定 {#configure-basic-info}

顧客情報ページの基本情報エリア内では、顧客に関する詳細が Workfront によって設定され、読み取り専用モードで表示されます。その他の詳細は、ユーザーが設定できます。このエリアで編集できるすべてのオプションは、Workfront のすべてのユーザーに全体的に影響します。

顧客情報エリアで「基本情報」セクションを設定するには：

{{step-1-to-setup}}

1. 左側のパネルで、**システム**／**顧客情報**&#x200B;をクリックします。

1. **顧客情報**&#x200B;ページの上部にある「**基本情報**」セクションで、Workfront のインスタンスに関する次の情報を見つけます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名前</td> 
      <td>組織の名前（会社の名前とも一致）。Workfront によって追加され、編集できません。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">クラスタ設定 </td> 
      <td>インスタンスのクラスター番号。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理メール</td> 
      <td> <p>Workfront 管理者のメールアドレス。このフィールドを編集して、Workfront 管理者のうち 1 人のメールアドレスと一致させることができます。このメールアドレスに関連付けられているユーザーは、Workfront システムのメインのWorkfront 管理者と見なされます。Workfront からのサイト全体に対する通信は、このメールアドレスに送信されるので、更新しておくことが重要です。</p> <p><b>メモ</b>：管理者 E メールに関連付けられたユーザーのアクセスレベルを非アクティブ化、削除、変更することはできません。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ドメイン</td> 
      <td> <p>ドメインは、アカウントの作成時に Workfront によって設定されます。</p> <p>ドメインによって、Workfront へのアクセスに使用する URL の一意のサブドメインが決まります。<p>例えば、組織に「mycompany」ドメインが割り当てられている場合、Workfront へのアクセスに使用する URL は <i>https://mycompany.my.workfront.com.</i> となります。</p><p>自分でドメインを編集することはできません。ドメインを変更する場合は、Workfront カスタマーサポートにお問い合わせください。Workfront カスタマーサポートへのお問い合わせについて詳しくは、<a href="../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">カスタマーサポートに連絡</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">タイムゾーン</td> 
      <td> <p>これは、Workfront インスタンスのデフォルトのタイムゾーンです。このフィールドを編集して、Workfront のプライマリ地域のタイムゾーンに合わせることができます。選択するタイムゾーンによって、次のことが決まります。 </p> 
       <ul> 
        <li>送信メールに表示される日時</li> 
        <li>新規ユーザー作成時のデフォルトのタイムゾーン</li> 
       </ul> <p>ユーザーは、自分のプロファイルの下の Workfront インスタンスのタイムゾーンを変更できます。ユーザーがタイムゾーンを変更すると、Workfront からのメールの日時がプロファイルの環境設定と一致します。ユーザープロファイルの環境設定の変更について詳しくは、<a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">個人設定を指定</a>を参照してください。新しいスケジュールを作成する際に、デフォルトのタイムゾーンとして選択されます。スケジュールの作成について詳しくは、<a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">スケジュールを作成</a>を参照してください。</p> <p>ユーザーが Workfront でタイムゾーンをまたいで共同作業できるようにスケジュールを使用する方法について詳しくは、<a href="../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">タイムゾーンをまたいだ作業</a>を参照してください。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ロケール</td> 
      <td>送信メールメッセージで使用される言語、日付、数値の形式を変更します。ここで選択したロケールは、新規ユーザー作成時のデフォルトになります。ユーザーは、ユーザープロファイルでロケールを変更できます。ユーザーがロケールを変更すると、Workfront からのメールの言語、日付、数値の形式がプロファイルの環境設定と一致します。プロファイルの環境設定の変更について詳しくは、<a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">個人設定を指定</a>を参照してください。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ストレージ割当</td> 
      <td> <p>これは、Workfront インスタンスで使用可能なドキュメントストレージ容量です。<br>割り当て量には、Workfront に直接アップロードするドキュメントが含まれます。<br>次のものは含まれません。</p> 
       <ul> 
        <li>他のサードパーティのサービスプロバイダー（SharePoint、Google Drive、Webdam、Box、Dropbox、その他のドキュメントアセット管理プロバイダー）から Workfront にリンクするドキュメント。</li> 
        <li>Workfront データ（プロジェクト、タスク、イシュー、ユーザーなど）。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">製品バージョン</td> 
      <td>これは、ユーザーに割り当てられる Workfront インスタンスのタイプです。ほとんどの Workfront ユーザーの製品バージョンは、<strong>エンタープライズ</strong>です。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックします。
