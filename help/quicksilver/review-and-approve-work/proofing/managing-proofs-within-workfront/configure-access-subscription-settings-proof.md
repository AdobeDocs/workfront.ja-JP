---
product-area: documents;system-administration;setup
navigation-topic: manage-proofs-within-workfront
title: プルーフのアクセスおよびサブスクリプション設定を行う
description: ユーザーにログインを要求するかどうか、ユーザーにプルーフのサブスクリプションを許可するかどうかなど、個々のプルーフの特定のアクセスおよびサブスクリプション設定を行うことができます。プルーフのアクセスおよびサブスクリプション設定は、作成時に行うことも、Workfront に既に存在するプルーフに行うこともできます。
author: Courtney
feature: Digital Content and Documents
exl-id: f242887b-d768-4d56-b530-a1ac6294b2d4
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: ht
source-wordcount: '949'
ht-degree: 100%

---

# プルーフのアクセスおよびサブスクリプション設定を行う

ユーザーにログインを要求するかどうか、ユーザーにプルーフのサブスクリプションを許可するかどうかなど、個々のプルーフの特定のアクセスおよびサブスクリプション設定を行うことができます。プルーフのアクセスおよびサブスクリプション設定は、作成時に行うことも、Workfront に既に存在するプルーフに行うこともできます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>現在のプラン：Pro 以上</p> <p>または</p> <p>従来のプラン：Premium</p> <p>様々なプランでのプルーフ機能へのアクセスについて詳しくは、<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront のプルーフ機能へのアクセス</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>現在のプラン：ワークまたはプラン</p> <p>従来のプラン：任意（ユーザーのプルーフ機能が有効になっている必要があります）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">プルーフ権限プロファイル </td> 
   <td>マネージャー以上</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、役割、またはプルーフ権限プロファイルを確認するには、Workfront または Workfront プルーフの管理者に問い合わせてください。

## プルーフの作成時にアクセスおよびサブスクリプション設定を行う

プルーフの作成時に、プルーフのアクセスおよびサブスクリプション設定を行うには、次の手順を実行します。

1. プルーフが必要なプロジェクト、タスク、またはイシューに移動し、「**ドキュメント**」セクションをクリックします。
1. 右上のエリアにある「**新規追加**」をクリックします。
1. **新しいプルーフ**&#x200B;ページの右下隅にある「**プルーフの設定**」セクションにスクロールします。

1. 次の設定を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>パブリック URL または埋め込みコード経由によるプルーフの共有を許可する</strong> </td> 
      <td>このオプションを選択した場合、プルーフは公開 URL または埋め込みコード経由で共有できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>パブリック URL または埋め込みコード経由によるプルーフの登録を許可する</strong> </td> 
      <td>このオプションを選択すると、プルーフに明示的に追加されていないユーザーもプルーフを購読できます。プルーフを購読しているユーザーには、次の設定で定義した役割とメールが付与されます。
       <ul>
        <li><p><strong>サブスクライバーの役割：</strong>プルーフを購読するすべてのレビュアーに割り当てられる、デフォルトのプルーフの役割です。</p><p>重要：Workfront Proof 設定で<strong>共有を許可</strong>が<strong>全員</strong>以外に設定されている場合、サブスクリプションは組織内のユーザーに対してのみ機能します。詳しくは、<a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Workfront Proof でのサブスクリプション設定</a>を参照してください。</p></li>
        <li><strong>サブスクライバー向けのメールアラート設定：</strong>プルーフを購入するすべてのレビュアーに割り当てられるデフォルトのメールアラートです。</li>
       </ul><p>
        <ul>
         <li><strong>次の場合に必要なメールリンクを使用したプルーフへのアクセス：</strong>プルーフへのリンクを含むメールをサブスクライバーが受信するかどうかを設定します。次の項目を選択できます。<strong>メールなし</strong>（プルーフにアクセスするには、メールリンクは必要ありません）、<strong>プルーフ通知メールのみ</strong>（サブスクライバーが、確認なしでメールでプルーフへのリンクを受け取る）、または<strong>検証およびプルーフ通知メール</strong>（サブスクライバーは、メールでプルーフへのリンクを受け取り、リンクをクリックしてプルーフにアクセスする必要があります。このオプションの目的は、ユーザーがアクセスできる正しいメールアドレスを入力したことを確認することです）。</li>
        </ul><p>メモ：プルーフに自動ワークフローがすべて添付されている場合、すべての購読がプルーフの所有者に確認メールを生成するので、プルーフの所有者は、ユーザーを追加するステージを決定できます。<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 引き続きプルーフを作成します。

## 既存のプルーフのアクセスおよびサブスクリプション設定を行う

Workfront に既に存在するプルーフのアクセスおよびサブスクリプション設定を行うには、次の手順を実行します。

1. ドキュメントエリアで、設定を行うプルーフを含むドキュメントを選択し、「**ドキュメントの詳細**」をクリックします。
1. 左側のパネルで、「**プルーフビューアーの設定**」をクリックします。
1. 次の設定を行います。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>パブリック URL または埋め込みコード経由によるプルーフの共有を許可する</strong><strong></strong> </td> 
      <td>このオプションを選択した場合、プルーフは公開 URL または埋め込みコード経由で共有できます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>パブリック URL または埋め込みコード経由によるプルーフの登録を許可する</strong> </td> 
      <td>このオプションを選択すると、プルーフに明示的に追加されていないユーザーもプルーフを購読できます。プルーフを購読しているユーザーには、次の設定で定義した役割とメールが付与されます。
       <ul>
        <li><p><strong>サブスクライバーの役割：</strong>プルーフを登録するすべてのレビュアーに割り当てられる、デフォルトのプルーフの役割です。</p><p>重要：Workfront Proof 設定で<strong>共有を許可</strong>が<strong>全員</strong>以外に設定されている場合、サブスクリプションは組織内のユーザーに対してのみ機能します。詳しくは、<a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Workfront Proof でのプルーフ設定</a>を参照してください。</p></li>
        <li><strong>プルーフに参加した際のメールアラート：</strong> プルーフを購読するすべてのレビュアーに割り当てられるデフォルトのメールアラートです。</li>
       </ul><p>
        <ul>
         <li><strong>メールのリンクからプルーフにアクセスする必要があります：</strong>プルーフへのリンクを含むメールをサブスクライバーが受信するかどうかを設定します。次の項目を選択できます。<strong>メールなし</strong>（プルーフにアクセスするには、メールリンクは必要ありません）、<strong>プルーフ通知メールのみ</strong>（サブスクライバーが、確認なしでメールでプルーフへのリンクを受け取る）、または <strong>検証およびプルーフ通知メール</strong>（サブスクライバーは、メールでプルーフへのリンクを受け取り、リンクをクリックしてプルーフにアクセスする必要があります。このオプションの目的は、ユーザーがアクセスできる正しいメールアドレスを入力したことを確認することです）</li>
        </ul><p>メモ：プルーフに自動ワークフローがすべて添付されている場合、すべての購読がプルーフの所有者に確認メールを生成するので、プルーフの所有者は、ユーザーを追加するステージを決定できます。<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックします。
