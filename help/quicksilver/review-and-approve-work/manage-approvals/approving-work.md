---
product-area: projects
navigation-topic: approvals
title: 作業の承認
description: 作業の承認
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6e43edbb-14dd-493d-a76b-84be6c3bef82
TQID: https://experienceleague.adobe.com/dr9JkMk-s8-aartIC4j1N0uZOYOZwx96-xYdXC01fkU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
  - id: f0dd7b45-76b5-49d4-afe3-39f436b6fbd3
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: a004cc84-67b9-4a33-a3a7-8ec7273ef4dc
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 829
ht-degree: 77%

---

# 作業の承認

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;From&nbsp;Courtney: Linked to Training sites/ articles , don't change title and link)</p>
-->

承認者として設定されている場合は、承認を待っている作業を定期的にレビューする必要があります。

承認プロセスの作成については、[作業アイテムの承認プロセスの作成](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md)を参照してください。

Workfront での作業への承認の関連付けについては、[新規または既存の承認プロセスと作業の関連付け](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md)を参照してください。

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
   <p>コントリビューター以上</p>
   <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>承認に関連付けられたオブジェクトに対する表示以上のアクセス権</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>承認に関連付けられたオブジェクトに対する表示以上の権限</p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## Adobe Workfront で承認を検索

Workfront の様々な領域で承認を表示または管理できます。

承認待ちの項目または自分で承認用に送信した項目の表示について詳しくは、[承認の表示](../../review-and-approve-work/manage-approvals/view-approvals.md)を参照してください。

## ホーム領域から作業項目を承認

1. 右上隅の&#x200B;**[!UICONTROL メインメニュー]** ![&#x200B; メインメニューアイコン &#x200B;](assets/main-menu-icon.png)をクリックし、**[!UICONTROL ホーム]**&#x200B;をクリックします。
1. （条件付き）「**カスタマイズ**」をクリックして、**自分の承認** ウィジェットを追加します。
1. （条件付き）「**フィルター**」ドロップダウンメニューをクリックし、**すべて**&#x200B;を選択して、自分に割り当てられた承認と委任された承認を表示します。

   >[!NOTE]
   >
   >担当業務またはグループに割り当てられた承認は、ホームに表示されません。 チームに割り当てられた承認は、各チームメンバーのマイ承認ウィジェットに表示されます。


1. 承認する項目を選択します。

   ![自分の承認ウィジェット &#x200B;](assets/my-approvals-widget.png)

1. 右側のパネルで承認を決定する際に、使用可能なオプションの 1 つをクリックします。 承認する項目のタイプに応じて、ページの右上隅に次のオプションが表示されます。

   <table>
   <tr>
      <td>
      <p><strong>アクセス</strong></p>
      </td>
      <td>
      <p><strong>作業項目</strong></p>
      </td>
      <td>
      <p><strong>ドキュメント</strong></p>
      </td>
      <td>
      <p><strong>プルーフ</strong></p>
      </td>
   </tr>
   <tr>
      <td>
       <ul>
      <li>付与</li>
      <li>無視</li>
      </ul>
      必要に応じて、<b> アクセス権の変更</b> ドロップダウンメニューでアクセス権のレベルを調整できます。
      </td>
      <td>
         <ul>
         <li>承認</li>
         <li>Reject</li>
         </ul>
      決定ボタンのドロップダウンメニューをクリックして、決定にコメントを残すことができます。
      </td>
      <td>
   承認者として割り当てられた
         <ul>
         <li>承認</li>
         <li>変更して承認</li>
         <li>作業が必要</li>
         </ul>
   レビュアーとして割り当てられました
         <ul>
         <li>レビューの完了</li>
         </ul>
      この列のオプションは、統合承認にのみ適用されます。レガシードキュメントの承認は、作業項目の承認と同じように表示されます。 
      </td>
      <td>
         <ul>
         <li>プルーフを見る</li>
         </ul>
         プルーフビューアで決定します。プルーフのレビューについて詳しくは、<a href="../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md">Adobe Workfront内のプルーフのレビュー</a>を参照してください。
      </td>
   </tr>
   </table>

決定を行うと、承認はマイ承認ウィジェットから削除されます。


## プロジェクト、タスク、イシューから直接作業を承認

プロジェクト、タスク、イシューが承認保留中の場合、プロジェクト、タスク、イシューから直接承認または却下できます。 また、承認プロセスに関する詳細も表示できます。

プロジェクト、タスク、イシューから直接作業を承認するには、次の手順に従います。

1. 承認が必要なプロジェクト、タスク、イシューに移動します。

   プロジェクト、タスク、イシューの現在の承認プロセスに関する承認情報が、項目のヘッダーに表示されます。

   ![&#x200B; プロジェクトヘッダーの現在の承認プロセス &#x200B;](assets/current-approval-process-in-project-header-with-stages-nwe-350x92.png)

   次の承認情報が表示されます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">ステータス</td> 
      <td>プロジェクト、タスク、イシューの現在のステータス。 これは、承認待ちの項目の現在のステータスです。 承認プロセスの各ステージが承認されると、ステータスが承認済みになります。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">承認ステージ</td> 
      <td>承認プロセスのステージ。 <br>承認待ちの現在のステージは、「保留」と表示されます。 既に承認済みのステージは「承認済み」と表示され、まだ承認されていないステージは「開始前」と表示されます。</td> 
     </tr> 
    </tbody> 
   </table>

1. 承認プロセスを承認するか却下するかに応じて、「**承認**」または「**却下**」をクリックします。\
   承認待ちだった承認ステージが承認され、承認プロセスが次のステージに移動します。 すべてのステージが承認されると、ステータスが承認済みになります。

## ドキュメントから直接ドキュメントを承認

1. 承認を必要とするドキュメントが含まれているドキュメントエリアに移動します。
1. ドキュメントを選択し、「**承認**」、「**変更**」、または「**却下**」をクリックします。\
   ![文書を承認](assets/approval-approve-document-350x215.png)\
   ![文書の承認](assets/document-approval-350x199.png)

1. （オプション）ドキュメントのプルーフが生成されている場合は、プルーフインターフェイス内でドキュメントを承認できます（[プルーフからのドキュメントの承認](#approve-a-document-from-a-proof)参照）。

## 承認通知メールからのドキュメントの承認

通知設定に応じて、他のユーザーがあなたによる承認決定を必要としているドキュメントについて通知するメールを受け取る場合があります。 「**承認決定する**」ボタンを含むメールを受信した場合は、そのメールから直接承認プロセスを開始できます。

1. メールで「**承認決定する**」をクリックすると、プルーフのドキュメントの詳細ページが開きます。
1. ドキュメントをレビューするには、次のいずれかの操作を行います。

   * ドキュメントに関するメタデータを表示します。
   * マークアップとコメントを含むドキュメントを確認するためのプルーフが作成されている場合は、右上隅付近にある「**プルーフを開く** ![&#x200B; プルーフを開く](assets/open-proof-icon-qs.png)」をクリックして、プルーフを確認します。

     <!--   
     <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">[Andrzej, does it make sense to leave this here if it's s document approval?&nbsp;Would there never be a proof in that situation?]</span>   
     -->

     プルーフの確認について詳しくは、[Adobe Workfront でのプルーフのレビュー](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md)を参照してください。

1. 右上隅にある「**決定**」オプションをクリックして、ドキュメントを承認、変更して承認、または却下します。

## プルーフからのドキュメントの承認 {#approve-a-document-from-a-proof}

プルーフビューア内でプルーフを承認できます。 詳しくは、[プルーフビューアでのプルーフの決定](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)の記事の[プルーフビューアでのプルーフの決定](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md)を参照してください。
