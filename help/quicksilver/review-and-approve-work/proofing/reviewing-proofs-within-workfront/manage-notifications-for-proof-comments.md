---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: プルーフのコメントおよび校正判断に関する通知を管理
description: プルーフを操作する際に、Adobe Workfront ユーザーであるか外部の共同作業者であるかに関わらず、プルーフに対するコメントや校正判断に関して受け取るメール通知を指定できます。詳しくは、プルーフのコメントおよび校正判断の通知の概要を参照してください。
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: ht
source-wordcount: '983'
ht-degree: 100%

---

# プルーフのコメントおよび校正判断に関する通知を管理

プルーフを操作する際に、Adobe Workfront ユーザーであるか外部の共同作業者であるかに関わらず、プルーフに対するコメントや校正判断に関して受け取るメール通知を指定できます。詳しくは、[プルーフのコメントおよび校正判断の通知の概要](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md)を参照してください。

>[!NOTE]
>
>これらの通知は、レビュアー間のプルーフのフローに関して受け取るメールアラートとは異なります。また、Workfront で設定できるメールアラート設定とは異なります。 

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
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;ご利用のプラン、役割またはプルーフ権限プロファイルを確認するには、Workfront または Workfront Proof 管理者にお問い合わせください。

## プルーフのコメントおよび校正判断に関する通知を管理

1. 通知を設定するプルーフを開きます。
1. 左側のツールバーが表示されていない場合は、web プルーフビューアーの左上隅にある&#x200B;**メニュー**&#x200B;アイコンをクリックします。

   ![Menu_icon_in_Proofing_Viewer.png](assets/menu-icon-in-proofing-viewer-350x228.png)

1. 左側のツールバーで、**設定**&#x200B;アイコンをクリックします。![Settings_icon.png](assets/settings-icon.png)

1. 「**次の通知メールを自分宛に送信する**」の下のプルーフに必要な設定をクリックします。

   選択した設定は、開いているプルーフに対してのみ有効です。

   システムのデフォルトは&#x200B;**毎日の概要**&#x200B;です。自分または自分のレビューアが他の変更を加えない場合、すべてのプルーフにこの設定が適用されます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">すべてのアクティビティ</td> 
      <td>新しいコメント、返信、校正判断など、プルーフに関するアクティビティが発生するたびに、レビュアーにメールが送信されます。<br><p>これは、アクティビティの発生を確認できるので、プルーフプロセスを管理するユーザーにとって最適なオプションです。ユーザーには、自分のアクティビティ（コメント、返信、校正判断など）に関するメールアラートは送信されません。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">自分のコメントへの返信</td> 
      <td>誰かがコメントに明示的に返信した場合にのみ、メールがレビュアーに送信されます（これには、自分のコメントに対する自分の返信は含まれません）。これは、プルーフ上の誰かが新しいコメントを作成しても、レビュアーには通知されないことを意味します。<p>この設定は、プルーフ上のクライアントに推奨されます。これにより、プルーフ上の他のコメントは通知されず、自分のコメントに対する返信のみが通知されます。</p><p>このメール通知設定を使用しているレビュアーには、他の新しいコメントは通知されませんが、プルーフビューアでプルーフ上のすべてのコメントを表示できます。<br></p><p>詳しくは、<a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">プルーフのコメントの表示および返信</a>を参照してください。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">決定</td> 
      <td>レビュアーにメールが送信されるのは、誰かが校正判断したときに限ります。<br><p>このメールアラートは、承認プロセスを管理する人（プロジェクトマネージャーなど）にとって役に立ちます。承認プロセスを管理する人が、プルーフの進捗状況を監視し、どのユーザーが校正判断したかを確認できるからです。<br></p><p>決定を送信するときにメール確認オプションを選択しない限り、自分の決定は通知されません。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">最終決定</td> 
      <td>プルーフに関する最終的な校正判断が行われると（プルーフの最後の承認者が校正判断を行った際に）、メールが送信されます。<br><p>このアラートは多くの場合、デザイナーが実際のレビューディスカッションに参加する必要がないので、デザイナーによって使用されます。最終的な決定が下されると、デザイナーに通知が届き、必要な変更に対してアクションを実行できます。<br></p><p>また、このアラートは、レビュープロセスが完了した場合にのみ通知を受け取る必要がある部署のリーダーに対しても役立ちます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">毎時の概要</td> 
      <td>過去 1 時間に発生したすべてのコメント、返信および校正判断の概要を示したメールが、1 時間ごとにレビュアーに送信されます。<br><p>メールは、過去 1 時間以内に自分以外のアクティビティが発生した場合にのみ送信されます。他のユーザーが行ったアクティビティがない場合は、メールは送信されません。<br></p><p>このアラートは、プロジェクトの概要を確認するのに適しています。<br></p><p>この概要のユースケース例として、プロジェクトの概要を必要としながら、プルーフでのすべてのアクティビティについてすぐに通知される必要はない、シニアレビューアが挙げられます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">日次の概要</td> 
      <td>（デフォルト設定）：すべてのコメント、返信および校正判断が記載されたメールは毎日送信されます。メールは、自分以外のユーザーがアクティビティを行った日にのみ送信されます。<br><p>このアラートは、1 日を通じて複数の更新で圧倒されることなく、プロジェクトの概要を確認するのに適しています。<br></p><p>この概要のユースケースの例として、プロジェクトの全体的な進行状況の監視を担当する部門のリーダーが挙げられます。<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">メールなし</td> 
      <td>メールアラートは送信されません。<br><p>この設定は、参照のみの目的でプルーフに追加され、変更に関する通知を必要としないユーザーに役立ちます。</p><p>メモ： <p>このオプションでは、プルーフのコメントや校正判断に関して受け取ることができるメールアラートのみを無効にします。新規プルーフや遅延プルーフメールなど、プルーフのフローに関して受け取るメールアラートを無効にすることはありません。プルーフのフローに関するメールアラートについて詳しくは、次の記事を参照してください。 </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">新規プルーフメール</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">新しいバージョンのメール</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">遅延プルーフメール</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">プルーフによるメール</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
