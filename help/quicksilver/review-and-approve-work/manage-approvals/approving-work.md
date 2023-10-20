---
product-area: projects
navigation-topic: approvals
title: 作業の承認
description: 作業の承認
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 6e43edbb-14dd-493d-a76b-84be6c3bef82
source-git-commit: 95679dd71ef7e4991853e63573a387f26321159d
workflow-type: tm+mt
source-wordcount: '1134'
ht-degree: 0%

---

# 作業の承認

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;From&nbsp;Courtney: Linked to Training sites/ articles , don't change title and link)</p>
-->

承認者として設定されている場合は、承認を待っている作業を定期的に確認する必要があります。

承認プロセスの作成について詳しくは、 [作業項目の承認プロセスの作成](../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

Workfrontでの作業への承認の関連付けについて詳しくは、 [新規または既存の承認プロセスを作業に関連付ける](../../review-and-approve-work/manage-approvals/associate-approval-with-work.md).

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>承認に関連付けられたオブジェクトへの表示またはそれ以上のアクセス権</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限が設定されているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクトの権限</td> 
   <td> <p>承認に関連付けられたオブジェクトに対する権限を表示するか、それ以上に設定します</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## Adobe Workfrontで承認を検索

Workfrontの様々な領域で承認を表示および管理できます。

承認待ちの項目または自分で承認用に送信した項目の表示について詳しくは、 [承認を表示](../../review-and-approve-work/manage-approvals/view-approvals.md).

## [ ホーム ] 領域から作業を承認

1. 次をクリック： **ホーム** アイコン ![](assets/home-icon-30x29.png) Adobe Workfrontの左上隅に

   >[!NOTE]
   >
   >Workfront管理者は、お使いの環境のホームアイコンに次の変更を加えることができます。
   >
   >   
   >* 組織を説明するようにカスタマイズされた画像に置き換えます。 この場合、この記事に示すアイコンは異なります。
   >* リンクされたページを別のページに置き換えます。 この場合、 **メインメニュー** ![](assets/main-menu-icon.png) ページの右上隅にある「 **ホーム**.

1. 次をクリック： **フィルター** ドロップダウンメニュー。

   ![](assets/displaying-work-items-filters-nwe-350x401.png)

1. 選択 **承認**.\
   承認を必要とするすべての作業項目が表示されます。 

   >[!NOTE]
   >
   >ジョブの役割またはグループに割り当てられた承認は、ホームに表示されません。 チームに割り当てられた承認は、「チームリクエスト」グループのワークリストに表示されます。

1. （オプション）記事の「グループ化して日付、プロジェクトまたは優先度で並べ替える」の説明に従って、承認を表示する順序を変更します。 [[ ホーム ] 領域の [ 作業リスト ] に項目を表示する](../../workfront-basics/using-home/using-the-home-area/display-items-in-home-work-list.md).
1. 承認を決定する項目を選択します。

   ![](assets/task-approval-home-350x127.png)

1. 右側のパネルで承認を決定する際に、使用可能なオプションの 1 つをクリックします。 承認する項目のタイプに応じて、ページの右上隅に次のオプションが表示されます。

   * **プロジェクト：** クリック **承認** または **拒否**.

   * **タスク：** クリック **承認** または **拒否** .

   * **問題：** クリック **承認** または **拒否** .

   * **タイムシート：** クリック **承認** または **拒否** .

   * **ドキュメント：** クリック **承認**, **拒否**&#x200B;または **変更点**.\
      承認を表示する際は、次の点を考慮してください。

      * 記事の「配達確認リンクの共有」の節で説明されているように、配達確認の承認がユーザーと共有されると、ここに表示されます [Adobe Workfront内での配達確認の共有](../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).
      * 校正承認は、Workfront環境がWorkfront Proof Premium アカウントと統合されている場合にのみ、ホーム領域に表示されます。 ここで説明しているように、校正を使用できない場合は、Workfront管理者にお問い合わせください。
      * 承認の通知がアプリ内で送信され、校正の承認が通知されます。\
        アプリ内通知について詳しくは、 [アプリ内通知の表示と管理](../../workfront-basics/using-notifications/view-and-manage-in-app-notifications.md).

      * 承認をリクエストしたユーザーの名前が、ホーム領域のサムネール画像の横に、次のテキストと共に表示されます。\
        &quot;*ユーザー A* ......」

        <!--      
        <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">      
        (NOTE:&nbsp;From&nbsp;Courtney: Is this true?)      
        </MadCap:conditionalText>      
        -->

        ユーザー名が使用できない場合は、次のテキストが表示されます。\
        「新しいバージョンの配達確認を表示する準備が整いました」
      * 配達確認を承認するには、 **配達確認に移動**&#x200B;をクリックし、 **レビューを終了**&#x200B;をクリックし、使用可能なオプションの 1 つをクリックします。 配達確認を承認する際に使用できるオプションは次のとおりです。 **承認済み**, **承認済み、変更あり**, **変更が必要です**、および **関連なし**.

      * 配達確認に対して決定がおこなわれると、配達確認は「承認」タブに残り、「決定がおこなわれました」というテキストが表示されます ( **更新** 」ボタンをクリックするか、ブラウザーページを更新するまでクリックします。

        配達確認の確認について詳しくは、 [Adobe Workfront内での配達確認の確認](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

   * **アクセス：** で付与するアクセスレベルを選択します。 **アクセスを変更** ドロップダウンメニューから、 **アクセスを許可**. または、「 **無視**.

## プロジェクト、タスク、イシューから直接作業を承認する

プロジェクト、タスクまたはタスクが承認待ちの場合は、プロジェクト、タスクまたはタスクから直接承認を承認または却下できます。 また、承認プロセスに関する詳細も表示できます。

プロジェクト、タスクまたはイシューから直接作業を承認するには、次の手順に従います。

1. 承認が必要なプロジェクト、タスク、またはタスクに移動します。

   プロジェクト、タスクまたはイシューの現在の承認プロセスに関する承認情報が、アイテムのヘッダーに表示されます。

   ![](assets/current-approval-process-in-project-header-with-stages-nwe-350x92.png)

   次の承認情報が表示されます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">ステータス</td> 
      <td>プロジェクト、タスク、またはタスクの現在のステータス。 これは、承認待ちの項目の現在のステータスです。 承認プロセスの各ステージが承認されると、ステータスが承認されます。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">承認ステージ</td> 
      <td>承認プロセスのステージ。 <br>承認待ちの現在のステージは、「保留中」と表示されます。 既に承認済みのステージは「承認済み」と表示され、まだ承認されていないステージは「未開始」と表示されます。</td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **承認** または **拒否**&#x200B;承認プロセスを承認するか却下するかに応じて。\
   承認待ちだった承認ステージが承認され、承認プロセスが次のステージに移動します。 すべてのステージが承認されると、ステータスが承認されます。

## ドキュメントから直接ドキュメントを承認 

1. 承認を必要とするドキュメントが含まれているドキュメント領域に移動します。
1. ドキュメントを選択し、「 **承認**, **変更点**&#x200B;または **拒否**.\
   ![](assets/approval-approve-document-350x215.png)\
   ![](assets/document-approval-350x199.png)

1. （オプション）ドキュメントの配達確認が生成されている場合は、ドキュメントを承認するためのインターフェイスを使用します。詳しくは、 [配達確認からドキュメントを承認](#approve-a-document-from-a-proof).

## 承認通知 E メールからのドキュメントの承認

通知の設定に応じて、他のユーザーが承認を決定する必要があるドキュメントについて通知する電子メールを受け取る場合があります。 次の情報を含む E メールを受信した場合： **承認を決定する** 」ボタンをクリックすると、承認プロセスを電子メールから直接開始できます。

1. 電子メールで、 **承認を決定する** をクリックして、配達確認のドキュメントの詳細ページを開きます。
1. ドキュメントを確認するには、次のいずれかの操作を行います。

   * ドキュメントに関するメタデータを表示します。
   * マークアップとコメントを含むドキュメントのレビュー用に配達確認が作成されている場合は、 **配達確認を開く** ![](assets/open-proof-icon-qs.png) 右上隅近くにある「 」をクリックし、配達確認を確認します。

     <!--   
     <span style="color: #ff1493;" data-mc-conditions="QuicksilverOrClassic.Draft mode">[Andrzej, does it make sense to leave this here if it's s document approval?&nbsp;Would there never be a proof in that situation?]</span>   
     -->

     配達確認のレビューについて詳しくは、 [Adobe Workfront内での配達確認の確認](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/review-proofs-in-wf.md).

1. クリック **決定** オプションを使用して、ドキュメントを承認、変更を加えて承認、拒否することができます。

## 配達確認からドキュメントを承認 {#approve-a-document-from-a-proof}

校正ビューア内でドキュメントを承認できます。 詳しくは、 [校正ビューアで配達確認を決定する](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md) 記事内 [校正ビューアで配達確認を決定する](../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/make-a-decision-on-a-proof/make-decisions-on-proof.md).
