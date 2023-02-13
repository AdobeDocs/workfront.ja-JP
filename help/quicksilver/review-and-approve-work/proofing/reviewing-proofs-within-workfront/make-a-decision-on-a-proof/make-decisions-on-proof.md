---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: 校正ビューアで配達確認を決定する
description: 配達確認に関する決定は、校正ビューアで直接おこなうことができます。
author: Courtney
feature: Digital Content and Documents
exl-id: cf74ac54-b8c1-4404-b35f-2aa94831ecad
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '391'
ht-degree: 3%

---

# 校正ビューアで配達確認を決定する

配達確認に関する決定は、校正ビューアで直接おこなうことができます。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>現在のプラン：Pro 以上</p> <p>または</p> <p>レガシープラン：選択またはプレミアム</p> <p>様々なプランでのアクセスの検証について詳しくは、 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfrontの校正機能へのアクセス</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>現在のプラン：作業または計画</p> <p>レガシープラン：任意（ユーザーの校正が有効になっている必要があります）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">プルーフ権限プロファイル </td> 
   <td>マネージャ以降</td> 
  </tr> 
  <tr> 
   <td role="rowheader">配達確認の役割</td> 
   <td>承認者、レビュー担当者、承認者、作成者、モデレーター</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、役割、配達確認権限プロファイルを確認するには、WorkfrontまたはWorkfrontの配達確認管理者に問い合わせてください。

## 校正ビューアで配達確認を決定する

1. ドキュメントを含むプロジェクト、タスクまたはイシューに移動し、「 」を選択します。 **ドキュメント**.
1. 必要な配達確認を見つけて、「 **配達確認を開く**.

1. クリック **決定を下す** をクリックします。

1. 内 **配達確認の決定** 表示されるボックスで、次のいずれかの決定をクリックします。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">承認済み</td> 
      <td>配達確認は、自動ワークフローの次のステージに移る準備が整いました。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">変更して承認済み</td> 
      <td>配達確認には変更が必要ですが、自動ワークフローの次のステージに移る前にリビジョンを確認する必要はありません。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">変更が必要です</td> 
      <td>配達確認は変更が必要です。自動ワークフローの次のステージに移る前に、別のリビジョンを確認する必要があります。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">無関係</td> 
      <td>配達確認はユーザーに関係なく、ユーザーが決定する必要はありません。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">カスタムの決定</td> 
      <td> <p>Select プランと Premium プランでは、Workfront管理者またはWorkfront Proof 管理者が、決定の名前変更、並べ替えおよび非表示をおこなうことができます。 詳しくは、 <a href="../../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md" class="MCXref xref">Workfront Proof での承認決定オプションの設定</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. （条件付き） Adobe Workfront管理者またはWorkfront Proof 管理者が「理由」セクションを追加した場合、決定に適用される理由を選択します。 管理者が決定理由を設定する方法について詳しくは、  [Workfront Proof での承認決定オプションの設定](../../../../workfront-proof/wp-acct-admin/account-settings/configure-approval-decision-in-wp.md).
1. （オプション）「 」を選択します。 **確認メールを送信** ：決定の確認を電子メールで受け取ります。
1. クリック **決定を下す**.

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
