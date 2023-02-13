---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: 配達確認の進行状況とステータスの概要
description: レビュープロセスでの配達確認の進行状況に関する情報を「ドキュメント」領域で表示し、配達確認の判定ステータスの全体的な概要を確認できます。
author: Courtney
feature: Digital Content and Documents
exl-id: 78e81070-ff82-4d82-90a3-6e0cd176b290
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '367'
ht-degree: 2%

---

# 配達確認の進行状況とステータスの概要

レビュープロセスでの配達確認の進行状況に関する情報を「ドキュメント」領域で表示し、配達確認の判定ステータスの全体的な概要を確認できます。

## 配達確認の進行状況の概要

配達確認の進行状況は、受信者に配達確認を送信した時点から配達確認を決定した時点までの間に、配達確認に対しておこなわれる作業を示します。 配達確認名の横に、進行状況アイコン（S、O、C および D）が表示され、配達確認の進行状況に関する情報が示されます。

![](assets/proof-edit-existing-progress-350x62.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <td> <p><strong>進行状況アイコン</strong> </p> </td> 
   <td> <p><strong>説明</strong> </p> </td> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-sent-icon.png" alt=""> </p> <p><strong>送信済み</strong> </p> </td> 
   <td> <p>配達確認は、割り当てられた受信者に送信されました。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong></strong> </p> <p><strong>開封済み</strong> </p> </td> 
   <td> <p>割り当てられたすべての受信者が、配達確認または配達確認の詳細ページを開きます。</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong></strong> </p> <p><strong>コメントが行われました</strong> </p> </td> 
   <td> <p>割り当てられたすべての受信者が、配達確認に対して 1 つ以上のコメントを記入します。</p> <p>配達確認にレビュー担当者が割り当てられていない場合は、 <strong>C</strong> アイコンがプログレスバーに表示されない。</p> </td> 
  </tr> 
  <tr> 
   <td> <p> <img src="assets/proof-progress-decision-icon.png" alt=""> </p> <p><strong>決定</strong> </p> </td> 
   <td> <p>割り当てられたすべての承認者が配達確認に対して決定を行います。配達確認の作成者が 1 つの決定のみを指定しない限り、割り当てられたすべての承認者は配達確認に対して決定を行います。</p> <p>配達確認の承認者（意思決定者）が指定されていない場合、 <strong>D</strong> アイコンがプログレスバーに表示されない。 </p> </td> 
  </tr> 
 </tbody> 
</table>

配達確認の進行状況に関する特定の情報を示す進行状況アイコンが、次の色で表示されます。

* **緑**:完了。
* **白**:未完了。
* **オレンジ**：未完了で、期限が 24 時間未満です。
* **赤**:完了せず、期限を過ぎていません。

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode">Levels of proof progress</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Workfront Proof uses the progress icons to track a proof's progress at each of the following levels:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For each reviewer, based on that person's activity on the proof.&nbsp;</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For each stage, based on the progress the reviewer on the stage who is most behind in the proofing process.&nbsp;To learn more about stages, see <a href="../../../review-and-approve-work/proofing/proofing-overview/stages.md" class="MCXref xref">Automated Workflow Stages overview</a>.</li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">For the proof, based on the progress of the stage (group of reviewers) who is the most behind in the proofing process.</li>
  -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For an example of how Workfront Proof determines progress using the reviewer or stage that is most behind,&nbsp;suppose three reviewers on a proof need to make a&nbsp;decision. If two of them have made their&nbsp;decision&nbsp;but the third has not, the progress bar for the proof does not show&nbsp;the D in green because of the outstanding&nbsp;decision.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">If the Primary Decision Maker setting is selected on a proof and the primary decision maker submits a decision, the D in the proof progress bar turns&nbsp;green for all reviewers because no other decisions are required.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Similarly, if the Only One Decision Required setting is selected on a proof and any reviewer submits a decision, the D in the proof progress bar turns&nbsp;green for all reviewers because no other decisions are required.</p>
-->

## 配達確認ステータスの概要

配達確認ステータスには、配達確認に必要な決定のステータスが表示されます。 配達確認のステータスは、「最悪のケース」の参加者によって決まります。 例えば、配達確認に関して 3 つの決定があるとします。2 人は～の地位を持っている **許可済み** そして一人は **却下**. の「最悪のケース」の決定 **却下** 過剰ルール他の決定と配達確認の全体的なステータスは、次のように表示されます。 **却下**. 

![](assets/proof-edit-existing-progress-350x62.png)

標準のステータスオプションを次に示します。

* 保留中
* 承認済み
* 変更も承認済み
* 変更が必要です
* 関連なし

アカウントでカスタムの決定が設定されている場合、ステータスオプションはカスタムの決定設定を反映します。

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Viewing proof progress and status</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"> You can view the progress and status of proofs for individual documents. </p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#view-proof-progress-and-status-for-a-document" class="MCXref xref">View proof progress and status&nbsp;for a document</a> </li>
  -->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="#view-proof-approval-information-in-home" class="MCXref xref">View proof approval information&nbsp;in Home</a> </li>
  -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="view-proof-progress-and-status-for-a-document">View proof progress and status&nbsp;for a document</h3>
-->

<!--
   <li value="1" data-mc-conditions="QuicksilverOrClassic.Draft mode">If a proof has not already been generated for the document in Adobe Workfront, generate it, as described in the articles.</li>
   -->

<!--
   <li value="2" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the Documents area, under the proof's name, click <strong>Proof Details</strong>.</li>
   -->

<!--
   <li value="3" data-mc-conditions="QuicksilverOrClassic.Draft mode">In the <strong>Proofing Details</strong> box that appears, the proof's progress for each stage, then click <strong>Done</strong>.</li>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Under the proof's name, click <strong>Proofing Workflow</strong>.</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
   <img src="assets/click-proofing-workflow-qs-350x149.png" style="width: 350;height: 149;" data-mc-conditions="QuicksilverOrClassic.Draft mode">
   -->
<!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   These screenshots will need to change with new terminology ("Review Workflow" for this one?)
   </MadCap:conditionalText>
   <br> </p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">In the Workflow information that appears, scroll down to see the proof's progress for each stage:</p>
   -->

<!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode"> <img src="assets/scroll-to-see-socd-for-stages-qs-350x152.png" style="width: 350;height: 152;"> </p>
   -->

<!--
<h3 data-mc-conditions="QuicksilverOrClassic.Draft mode" id="view-proof-approval-information-in-home">View proof approval information&nbsp;in Home</h3>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You can view information about proofs that you have submitted for approval. Proof approval information is displayed in the Home area only while the proof is pending approval.&nbsp;For information about how to view information about proof approvals in the Home area, see&nbsp;<a href="../../../review-and-approve-work/manage-approvals/view-approvals.md" class="MCXref xref">View approvals </a>.</p>
-->
