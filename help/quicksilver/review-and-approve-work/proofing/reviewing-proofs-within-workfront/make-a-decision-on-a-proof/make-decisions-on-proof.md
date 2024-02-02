---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: プルーフビューアでのプルーフに関する意思決定
description: プルーフに関する決定をプルーフビューアで直接下すことができます。
author: Courtney
feature: Digital Content and Documents
exl-id: cf74ac54-b8c1-4404-b35f-2aa94831ecad
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: ht
source-wordcount: '391'
ht-degree: 100%

---

# プルーフビューアでのプルーフに関する意思決定

プルーフに関する決定をプルーフビューアで直接下すことができます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>現在のプラン：Pro 以上</p> <p>または</p> <p>従来のプラン：Select または Premium</p> <p>様々なプランでのプルーフ機能へのアクセスについて詳しくは、<a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfront のプルーフ機能へのアクセス</a>を参照してください。</p> </td> 
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
   <td role="rowheader">プルーフの役割</td> 
   <td>承認者、レビュアー兼承認者、作成者、モデレーター</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、役割、またはプルーフ権限プロファイルを確認するには、Workfront または Workfront プルーフの管理者に問い合わせてください。

## プルーフビューアでのプルーフに関する意思決定

1. ドキュメントを含むプロジェクト、タスクまたはイシューに移動し、「**ドキュメント**」を選択します。
1. 必要なプルーフを見つけて、「**プルーフを開く**」をクリックします。

1. プルーフビューアの中央上部にある「**決定する**」をクリックします。

1. 表示された「**プルーフ決定**」ボックスで、以下の決定のいずれかをクリックします。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">承認済み</td> 
      <td>プルーフは、自動化ワークフローの次の段階に進む準備ができています。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">変更後承認</td> 
      <td>プルーフにはいくつかの変更が必要ですが、自動化ワークフローの次の段階に進める前にリビジョンを確認する必要はありません。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">変更が必要です</td> 
      <td>プルーフにはいくつかの変更が必要であり、自動化ワークフローの次の段階に進める前にリビジョンを確認する必要があります。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">無関係</td> 
      <td>関係のないプルーフであり、決定を下す必要はありません。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">カスタム校正判断</td> 
      <td> <p>Select プランと Premium プランでは、Workfront 管理者や Workfront Proof 管理者が決定の名前変更、並べ替えおよび非表示を行えます。詳しくは、<a href="../../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md" class="MCXref xref">Workfront Proof での承認決定オプションの設定</a>を参照してください。</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （条件付き）Adobe Workfront 管理者や Workfront Proof 管理者が「理由」セクションを追加した場合は、当てはまる決定理由を選択します。管理者が決定理由を設定する方法について詳しくは、[Workfront Proof での承認決定オプションの設定](../../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md)を参照してください。
1. （オプション）「**確認メールを自分に送信**」を選択して、自分が下した決定の確認をメールで受け取ります。
1. 「**決定する**」をクリックします。

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Make a decision when the proof is configured with an approval process</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can make decisions on a proof when it is configured with an approval process (within Workfront) and&nbsp;a user has sent you a document approval request, as described in <a href="../../../../review-and-approve-work/manage-approvals/request-document-approvals.md" class="MCXref xref">Request document approvals</a>.</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#make-a-workfront-approval-decision-in-a-proof" class="MCXref xref">Make a Workfront approval decision in a proof</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#change-your-workfront-approval-decision-in-a-proof" class="MCXref xref">Change your Workfront approval decision in a proof</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="make-a-workfront-approval-decision-in-a-proof">Make a Workfront approval decision in a proof</h3>
-->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Open the proof of the document that you want to make a decision on.</p>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the proofing viewer, select whether you want to <strong>Approve</strong>, require <strong>Changes</strong>, or <strong>Reject</strong> the approval request.</li>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="change-your-workfront-approval-decision-in-a-proof">Change your Workfront approval decision in a proof</h3>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Open the proof of the document where you want to change your Workfront approval decision.</li>
<li value="2"> <p>At the top-center of the proofing viewer, click the decision you made previously.</p> </li>
<li value="3">In the <strong>Proof decision</strong> box that appears, select whether you want to <strong>Approve</strong>, require <strong>Changes</strong>, or <strong>Reject</strong> the approval request.</li>
</ol>
-->
