---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: プルーフのコメントおよび校正判断に関する通知を管理
description: プルーフで作業する際は、Adobe Workfront ユーザーであるか外部共同作業者であるかに関わらず、プルーフに対するコメントと決定に関して受け取るメール通知を指定できます。 詳しくは、プルーフのコメントおよび校正判断の通知の概要を参照してください。
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
source-git-commit: c79d030ff2d05487e5f7e3457bf98df591822a80
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 26%

---

# プルーフのコメントおよび校正判断に関する通知を管理

<!-- Audited: 4/2025 -->

プルーフで作業する際は、Adobe Workfront ユーザーであるか外部共同作業者であるかに関わらず、プルーフに対するコメントと決定に関して受け取るメール通知を指定できます。 詳しくは、[プルーフのコメントおよび校正判断の通知の概要](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md)を参照してください。

>[!NOTE]
>
>これらの通知は、レビュー担当者間でのプルーフのフローに関して受け取るメールアラートや、Workfrontで指定できるメールアラート設定とは異なります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

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
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>現在のプラン：ワークまたはプラン</p> <p>従来のプラン：任意（ユーザーのプルーフ機能が有効になっている必要があります）</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">プルーフ権限プロファイル </td> 
   <td>マネージャー以上</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、役割またはプルーフ権限プロファイルを確認するには、Workfront または Workfront Proof 管理者にお問い合わせください。

+++

## プルーフのコメントおよび校正判断に関する通知を管理

1. 通知を設定するプルーフを開きます。
1. 左側のツールバーが表示されていない場合は、Web プルーフビューアの左上隅にある **メニュー** アイコンをクリックします。

   ![Menu_icon_in_Proofing_Viewer.png](assets/menu-icon-in-proofing-viewer-350x228.png)

1. 左側のツールバーで、**設定** アイコン ![Settings_icon.png](assets/settings-icon.png) をクリックします。

1. 「**メール通知の送信先** セクションで、このプルーフの通知設定を選択します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">すべてのアクティビティ</td> 
      <td>新しいコメント、返信、決定など、プルーフに対するアクティビティがあるたびに、レビュー担当者にメールが送信されます。<br><p>プルーフプロセスを管理するユーザーは、この設定を使用するとアクティビティを確認できるので、この設定をお勧めします。 ユーザーが自分のアクティビティに関する電子メールアラート（コメント、返信、決定など）を受け取ることはありません。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">自分のコメントへの返信</td> 
      <td>自分のコメントに直接返信した場合（自分のコメントに対する返信を除く）にのみ、レビュー担当者にメールが送信されます。<p>この設定は、自分のコメントへの返信のみがクライアントに通知され、プルーフに対して行われた他のコメントについては通知されませんが、プルーフビューアではすべてのコメントを表示できるよう、推奨されています。</p>
      <p>詳しくは、<a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref"> プルーフコメントの表示と返信 </a> を参照してください。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">決定</td> 
      <td>レビュー担当者に対しては、何らかの決定が下された場合にのみメールが送信されます。<br><p>このメールアラートは、承認プロセスを管理するユーザーがプルーフの進捗状況を監視したり、どのユーザーが決定を下したかを確認したりできるので、承認プロセスを管理するユーザーにとって便利です。<br></p><p>決定を送信するときにメール確認オプションを選択しない限り、自分の決定は通知されません。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">最終決定</td> 
      <td>プルーフに対する最終的な決定が下されると、メールが送信されます。<br><p>このアラートは、デザイナーが実際のレビューディスカッションに参加する必要がないために、デザイナーがよく使用します。 最終決定が行われると、デザイナーに通知が送信され、必要な変更を加えることができます。<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">毎時の概要</td> 
      <td>1 時間ごとに、過去 1 時間に発生したすべてのコメント、返信、決定の概要を記載したメールがレビュー担当者に送信されます。<br><p>メールは、自分以外のアクティビティが過去 1 時間以内に発生した場合にのみ送信されます。 他のユーザーのアクティビティがない場合、メールは送信されません。<br></p><p>このアラートは、プロジェクトの進行の概要を確認するのに役立ちます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">日次の概要</td> 
      <td>（デフォルト設定）：すべてのコメント、返信、決定がリストされたメールが毎日送信されます。 これは、自分以外のアクティビティがある日にのみ送信されます。<br><p>このアラートを使用すると、1 日を通じて複数の更新に圧倒されることなく、プロジェクトの概要を確認できます。<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">メールなし</td> 
      <td>メールアラートは送信されません。<br><p>この設定は、参照目的でのみプルーフに追加され、変更の通知を受ける必要がないユーザーに役立ちます。</p><p>メモ： <p>このオプションは、プルーフのコメントと決定に関するメールアラートをオフにするだけです。新しいプルーフや遅延プルーフのメールなど、プルーフのフローに関して受け取れるメールアラートはオフにしません。 詳しくは、次の記事を参照してください。 </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">新規プルーフメール</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">新しいバージョンのメール</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">遅延プルーフメール</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">プルーフによるメール</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
