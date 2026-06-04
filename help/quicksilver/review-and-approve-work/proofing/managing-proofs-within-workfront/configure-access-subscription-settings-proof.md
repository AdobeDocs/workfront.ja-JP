---
product-area: documents;system-administration;setup
navigation-topic: manage-proofs-within-workfront
title: プルーフのアクセスおよびサブスクリプション設定を行う
description: ユーザーにログインを要求するかどうか、ユーザーにプルーフのサブスクリプションを許可するかどうかなど、個々のプルーフの特定のアクセスおよびサブスクリプション設定を行うことができます。 プルーフのアクセスおよびサブスクリプション設定は、作成時に行うことも、Workfront に既に存在するプルーフに行うこともできます。
author: Courtney
feature: Digital Content and Documents
exl-id: f242887b-d768-4d56-b530-a1ac6294b2d4
TQID: https://experienceleague.adobe.com/lcalyeMjj8Vj7hcdgwQx03101gSgocB82uWXHaZCacQ
product_v2: id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2: id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2: id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2: id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 823
ht-degree: 94%

---

# プルーフのアクセスおよびサブスクリプション設定を行う

ユーザーにログインを要求するかどうか、ユーザーにプルーフのサブスクリプションを許可するかどうかなど、個々のプルーフの特定のアクセスおよびサブスクリプション設定を行うことができます。 プルーフのアクセスおよびサブスクリプション設定は、作成時に行うことも、Workfront に既に存在するプルーフに行うこともできます。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td> 
   <p>標準</p>
   <p>作業または計画</p> 
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">プルーフ権限プロファイル </td> 
   <td>マネージャー以上</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>ドキュメントへのアクセスを編集</p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

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
      <td>このオプションを選択すると、プルーフに明示的に追加されていないユーザーは、プルーフを購読できます。プルーフを購読するユーザーには、次の設定で定義した役割と電子メールが付与されます。
       <ul>
        <li><p><strong>サブスクライバーの役割：</strong>プルーフを購読するすべてのレビュアーに割り当てられる、デフォルトのプルーフの役割です。 </p><p>重要：Workfront Proof 設定で<strong>共有を許可</strong>が<strong>全員</strong>以外に設定されている場合、サブスクリプションは組織内のユーザーに対してのみ機能します。 詳しくは、<a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Workfront Proof でのサブスクリプション設定</a>を参照してください。</p></li>
        <li><strong>サブスクライバー向けのメールアラート設定：</strong>プルーフを購入するすべてのレビュアーに割り当てられるデフォルトのメールアラートです。</li>
       </ul><p>
        <ul>
         <li><strong>必要なメールリンクでプルーフへのアクセス：</strong>プルーフへのリンクを含むメールをサブスクライバーが受信するかどうかを設定します。 「<strong>メールなし</strong>」（プルーフにアクセスするには、メールリンクを必要としません）、「<strong>プルーフ通知メールのみ</strong>」（サブスクライバーが、確認なしでメールでプルーフへのリンクを受け取る）、または「<strong>検証およびプルーフ通知メール</strong>」（サブスクライバーは、メールでプルーフへのリンクを受け取り、リンクをクリックしてプルーフにアクセスする必要があります。このオプションの目的は、ユーザーがアクセスできる正しいメールアドレスを入力したことを確認することです）を選択できます。</li>
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
      <td>このオプションを選択すると、プルーフに明示的に追加されていないユーザーは、プルーフを購読できます。プルーフを購読するユーザーには、次の設定で定義した役割と電子メールが付与されます。
       <ul>
        <li><p><strong>サブスクライバーの役割：</strong>プルーフを購読するすべてのレビュアーに割り当てられる、デフォルトのプルーフの役割です。 </p><p>重要：Workfront Proof 設定で<strong>共有を許可</strong>が<strong>全員</strong>以外に設定されている場合、サブスクリプションは組織内のユーザーに対してのみ機能します。 詳しくは、<a href="../../../workfront-proof/wp-work-proofsfiles/manage-your-work/configure-proof-settings.md" class="MCXref xref">Workfront Proof でのサブスクリプション設定</a>を参照してください。</p></li>
        <li><strong>サブスクライバー向けのメールアラート設定：</strong>プルーフを購入するすべてのレビュアーに割り当てられるデフォルトのメールアラートです。</li>
       </ul><p>
        <ul>
         <li><strong>必要なメールリンクでプルーフへのアクセス：</strong>プルーフへのリンクを含むメールをサブスクライバーが受信するかどうかを設定します。 「<strong>メールなし</strong>」（プルーフにアクセスするには、メールリンクを必要としません）、「<strong>プルーフ通知メールのみ</strong>」（サブスクライバーが、確認なしでメールでプルーフへのリンクを受け取る）、または「<strong>検証およびプルーフ通知メール</strong>」（サブスクライバーは、メールでプルーフへのリンクを受け取り、リンクをクリックしてプルーフにアクセスする必要があります。このオプションの目的は、ユーザーがアクセスできる正しいメールアドレスを入力したことを確認することです）を選択できます。</li>
        </ul><p>メモ：プルーフに自動ワークフローがすべて添付されている場合、すべての購読がプルーフの所有者に確認メールを生成するので、プルーフの所有者は、ユーザーを追加するステージを決定できます。<br></p></p></td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックします。
