---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: プルーフのコメントおよび校正判断に関する通知を管理
description: プルーフに関する作業を行う際に、Adobe Workfrontのユーザーであるか外部の共同作業者であるかを問わず、プルーフに関するコメントや決定を受け取るメール通知を指定できます。 詳しくは、プルーフのコメントおよび校正判断の通知の概要を参照してください。
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
TQID: https://experienceleague.adobe.com/2zcWEp77u5Eds1eB9r5UDdIAtNxSv9DdxGDIAd8b4Yw
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: bce87dde-a4ab-44c9-8a18-ad66e4ddb377
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 731
ht-degree: 28%

---

# プルーフのコメントおよび校正判断に関する通知を管理

<!-- Audited: 4/2025 -->

プルーフに関する作業を行う際に、Adobe Workfrontのユーザーであるか外部の共同作業者であるかを問わず、プルーフに関するコメントや決定を受け取るメール通知を指定できます。 詳しくは、[プルーフのコメントおよび校正判断の通知の概要](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md)を参照してください。

>[!NOTE]
>
>これらの通知は、レビュー担当者のプルーフのフローに関して受け取るメールアラートと、Workfrontで設定できるメールアラート設定とは異なります。

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
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">プルーフの役割 </td> 
   <td>レビュアー、レビュアー、承認者、作成者、モデレーター</td> 
  </tr> 
  <tr> 
   <td role="rowheader">プルーフ権限プロファイル </td> 
   <td>マネージャー以上</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## プルーフのコメントおよび校正判断に関する通知を管理

1. 通知を設定するプルーフを開きます。
1. 左側のツールバーが表示されない場合は、Web プルーフビューアの左上隅にある&#x200B;**メニュー** アイコンをクリックします。

   ![Menu_icon_in_Proofing_Viewer.png](assets/menu-icon-in-proofing-viewer-350x228.png)

1. 左側のツールバーで、**Settings** アイコン ![Settings_icon.png](assets/settings-icon.png)をクリックします。

1. 「**電子メール通知を送信**」セクションで、このプルーフの通知設定を選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">すべてのアクティビティ</td> 
      <td>新しいコメント、返信、決定など、プルーフに関するアクティビティが発生するたびに、レビュー担当者に電子メールが送信されます。<br><p>この設定は、プルーフプロセスを管理するユーザーがアクティビティを実際に確認できるため、推奨されます。 ユーザーは、自身のアクティビティ（コメント、返信、決定など）に関するメールアラートを受け取りません。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">自分のコメントへの返信</td> 
      <td>レビュー担当者に電子メールが送信されるのは、誰かが自分のコメントに直接返信した場合（自分のコメントに対する返信を除く）だけです。<p>この設定はクライアントに推奨されます。プルーフに対するコメントの返信のみが通知され、プルーフに対するその他のコメントは通知されませんが、プルーフビューアですべてのコメントを表示できます。</p>
      <p>詳しくは、<a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref"> プルーフコメントの表示と返信</a>を参照してください。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">決定</td> 
      <td>レビュー担当者が決定を下した場合にのみ、レビュー担当者に電子メールが送信されます。<br><p>このメールアラートは、承認プロセスを管理するユーザーがプルーフの進捗状況を監視し、どのユーザーが決定したかを確認できるため、承認プロセスを管理するユーザーにとって役立ちます。<br></p><p>決定を送信するときにメール確認オプションを選択しない限り、自分の決定は通知されません。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">最終決定</td> 
      <td>プルーフで最終決定が行われると、メールが送信されます。<br><p>このアラートは、デザイナーが実際のレビューの議論に参加する必要がないので、デザイナーがよく使用します。 最終的な決定が下されると、デザイナーに通知が届き、必要な変更に対してアクションを実行できます。<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">毎時の概要</td> 
      <td>1時間ごとに、過去1時間に起こったすべてのコメント、返信、決定の要約がレビュアーに送信されます。<br><p>メールは、過去 1 時間以内に自分以外のアクティビティが発生した場合にのみ送信されます。 他のユーザーからのアクティビティがない場合、メールは送信されません。<br></p><p>このアラートは、プロジェクトの進行状況を把握するのに最適な方法です。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">日次の概要</td> 
      <td>（デフォルト設定）：すべてのコメント、返信、決定が一覧表示されたメールが毎日送信されます。 これはあなた自身の以外に活動がある日にのみ送信されます。<br><p>このアラートは、1 日を通じて複数の更新で圧倒されることなく、プロジェクトの概要を確認するのに適しています。<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">メールなし</td> 
      <td>メールアラートは送信されません。<br><p>この設定は、参照目的でのみプルーフに追加され、変更の通知を受ける必要がないユーザーに役立ちます。</p><p>メモ： <p>このオプションは、プルーフのコメントや決定に関する電子メールアラートのみをオフにします。新しいプルーフやレイトプルーフの電子メールなど、プルーフのフローに関して受信できる電子メールアラートはオフにしません。 詳しくは、次の記事を参照してください。 </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">新規プルーフメール</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">新しいバージョンのメール</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">遅延プルーフメール</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">プルーフによるメール</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
