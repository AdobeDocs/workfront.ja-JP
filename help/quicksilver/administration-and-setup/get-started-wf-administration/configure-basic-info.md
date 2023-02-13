---
user-type: administrator
product-area: system-administration;setup
navigation-topic: start-with-workfront-administration
title: システムの基本情報を設定する
description: Adobe Workfrontシステムの設定の一環として、顧客情報ページの「基本情報」セクションで、組織に関する詳細を管理できます。
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: bad5e700-79a6-49ed-bcf9-f0b5b3eaa909
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '897'
ht-degree: 2%

---

# システムの基本情報を設定する

<!--DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.</p>-->

Adobe Workfrontシステムの設定の一環として、顧客情報ページの「基本情報」セクションで、組織に関する詳細を管理できます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> <col> 
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
   <td> <p>Workfront管理者である。 詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">ユーザーに完全な管理アクセス権を付与する</a>.</p> <p><b>注意</b>:まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 顧客情報にアクセス

顧客は、組織のWorkfrontインスタンスを表します。 この領域のオプションは、Workfrontをご利用のお客様に固有です。

顧客情報ページにアクセスするには：

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **システム** > **顧客情報**.

   購入したWorkfrontプランによっては、一部のセクションが顧客情報ページに表示されない場合があります。 組織で使用するWorkfrontプランを確認する必要がある場合は、アカウント担当者にお問い合わせください。

   「顧客情報」領域には、次のセクションがあります。

   * **基本情報**

      Workfrontでの基本情報の設定について詳しくは、 [基本情報を設定](#configure-basic-info).

   * **API キー設定**

      API キーの設定について詳しくは、 [API キーの管理](../../administration-and-setup/manage-workfront/security/manage-api-keys.md).

   * **IP 許可リスト**

      ユーザーがWorkfrontにアクセスできる場所に関する IP許可リストアドレスをに追加する方法について詳しくは、 [ファイアウォールの設定を許可リスト行う](../../administration-and-setup/get-started-wf-administration/configure-your-firewall.md).

   * **ライセンス**

      ライセンスについて詳しくは、 [システムで使用可能なライセンスを管理](../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

## 基本情報を設定 {#configure-basic-info}

顧客情報ページの「基本情報」領域内では、顧客に関する詳細がWorkfrontによって設定され、読み取り専用モードで表示されます。 その他の詳細は、ユーザーが設定できます。 この領域で編集できるすべてのオプションは、Workfrontのすべてのユーザーに全体的に影響します。

「Customer Info」領域で「Basic Info」セクションを設定するには：

1. 次をクリック： **メインメニュー** アイコン ![](assets/main-menu-icon.png) Adobe Workfrontの右上隅で、 **設定** ![](assets/gear-icon-settings.png).

1. 左側のパネルで、 **システム** > **顧客情報**.

1. 内 **基本情報** の上部にあるセクション **顧客情報** ページで、Workfrontのインスタンスに関する次の情報を見つけます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">名前</td> 
      <td>組織の名前。会社の名前とも一致します。 これはWorkfrontによって追加され、編集できません。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">クラスタ設定 </td> 
      <td>インスタンスのクラスター番号。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">管理者 E メール</td> 
      <td> <p>Workfront管理者の電子メールアドレス。 このフィールドを編集して、Workfront管理者の 1 人の E メールアドレスと一致させることができます。 この電子メールアドレスに関連付けられているユーザーは、WorkfrontシステムのメインのWorkfront管理者と見なされます。 Workfrontからのサイト全体での通信は、この電子メールアドレスに送信されるので、更新しておくことが重要です。</p> <p><b>注意</b>:管理者電子メールに関連付けられたユーザーのアクセスレベルを非アクティブ化、削除、変更することはできません。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ドメイン</td> 
      <td> <p>ドメインは、アカウントの作成時にWorkfrontによって設定されます。</p> <p>ドメインは、Workfrontにアクセスするために使用する URL の一意のサブドメインを識別します。<p>例えば、組織が「mycompany」ドメインを割り当てられている場合、Workfrontにアクセスするために使用する URL は「 <i>https://mycompany.my.workfront.com.</i></p><p>自分でドメインを編集することはできません。 ドメインを変更する場合は、Workfrontカスタマーサポートにお問い合わせください。 Workfrontカスタマーサポートへの問い合わせについて詳しくは、 <a href="../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md" class="MCXref xref">カスタマーサポートに連絡</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">タイムゾーン</td> 
      <td> <p>これは、Workfrontインスタンスのデフォルトのタイムゾーンです。 このフィールドを編集して、Workfrontの主要な場所のタイムゾーンに合わせることができます。 選択するタイムゾーンによって、次のことが決まります。 </p> 
       <ul> 
        <li>送信メールに表示される日時</li> 
        <li>新規ユーザー作成時のデフォルトのタイムゾーン</li> 
       </ul> <p>ユーザーは、自分のプロファイルの下のWorkfrontインスタンスのタイムゾーンを変更できます。 ユーザーがタイムゾーンを変更すると、Workfrontからの電子メールの日時がプロファイルの設定と一致します。 ユーザープロファイルの環境設定の変更について詳しくは、 <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">設定を行う</a>. 新しいスケジュールを作成する際に、デフォルトのタイムゾーンとして選択されます。 スケジュールの作成について詳しくは、 <a href="../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md" class="MCXref xref">スケジュールの作成</a>.</p> <p>タイムゾーンをまたいでWorkfrontでの共同作業に役立つスケジュールを使用する方法について詳しくは、 <a href="../../workfront-basics/tips-tricks-and-troubleshooting/working-across-timezones.md" class="MCXref xref">タイムゾーンをまたいでの作業</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">ロケール</td> 
      <td>送信電子メールメッセージで使用する言語、日付、および数値の形式を制御します。 ここで選択したロケールは、新しいユーザーが作成される際のデフォルトです。 ユーザーは、ユーザープロファイル内のロケールを変更できます。 ユーザーがロケールを変更すると、Workfrontからの電子メールの言語、日付、数値の形式が、プロファイルの環境設定と一致します。 プロファイル環境設定の変更について詳しくは、 <a href="../../workfront-basics/manage-your-account-and-profile/configuring-your-user-profile/configure-my-settings.md" class="MCXref xref">設定を行う</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">ストレージ割当</td> 
      <td> <p>Workfrontインスタンスで使用できるドキュメントストレージ領域の量です。<br>割り当てには、Workfrontに直接アップロードするドキュメントが含まれます。<br>次は含まれません。</p> 
       <ul> 
        <li>他のサードパーティのサービスプロバイダー (SharePoint、Google Drive、Webdam、Box、Dropbox、その他の Document Asset Management プロバイダー ) からWorkfrontにリンクするドキュメント。</li> 
        <li>Workfrontデータ（プロジェクト、タスク、問題、ユーザーなど）。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">製品バージョン</td> 
      <td>これは、割り当てられるWorkfrontインスタンスのタイプです。 ほとんどのWorkfrontユーザーの製品バージョンは、 <strong>大規模法人</strong>.</td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックします。
