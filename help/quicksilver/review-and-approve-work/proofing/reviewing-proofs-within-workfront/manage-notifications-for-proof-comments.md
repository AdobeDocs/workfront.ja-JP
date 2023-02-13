---
product-area: documents
navigation-topic: review-proofs-within-workfront
title: 配達確認コメントおよび決定に関する通知を管理
description: 配達確認を操作する際に、Adobe Workfrontユーザーであるか外部の共同作業者であるかに関わらず、配達確認に対するコメントや決定に関して受け取る電子メール通知を指定できます。 詳しくは、配達確認用コメントおよび決定の通知の概要を参照してください。
author: Courtney
feature: Digital Content and Documents
exl-id: c38e005c-8984-4e99-9527-94a0a6b1071d
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '983'
ht-degree: 0%

---

# 配達確認コメントおよび決定に関する通知を管理

配達確認を操作する際に、Adobe Workfrontユーザーであるか外部の共同作業者であるかに関わらず、配達確認に対するコメントや決定に関して受け取る電子メール通知を指定できます。 詳しくは、 [配達確認コメントおよび決定の通知の概要](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

>[!NOTE]
>
>これらの通知は、レビュー担当者間の配達確認のフローに関して受け取る E メールアラートとは異なります。 また、Workfrontで設定できる電子メールアラート設定とは異なります。 

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
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、役割、配達確認権限プロファイルを確認するには、WorkfrontまたはWorkfrontの配達確認管理者に問い合わせてください。

## 配達確認コメントおよび決定に関する通知を管理

1. 通知を設定する配達確認を開きます。
1. 左側のツールバーが表示されていない場合は、 **メニュー** アイコン（Web 校正ビューアの左上隅）

   ![Menu_icon_in_Proofing_Viewer.png](assets/menu-icon-in-proofing-viewer-350x228.png)

1. 左側のツールバーで、 **設定** アイコン ![Settings_icon.png](assets/settings-icon.png)

1. の下 **次に関する電子メール通知を受け取る**、配達確認に必要な設定をクリックします。

   選択した設定は、開いている配達確認に対してのみ有効です。

   システムのデフォルトはです。 **日別概要**. 自分または自分のレビュー担当者が他の変更を加えない場合、すべての配達確認にこの設定が適用されます。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">すべてのアクティビティ</td> 
      <td>新しいコメント、返信、決定など、配達確認に関するアクティビティが発生するたびに、レビュー担当者に E メールが送信されます。<br><p>これは、アクティビティの発生を確認できるので、校正プロセスを管理するユーザーにとって最適なオプションです。 ユーザーは、自分のアクティビティ（コメント、返信、決定など）に関する電子メールアラートを受け取りません。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">コメントに返信</td> 
      <td>メールは、誰かが自分のコメントに明示的に返信した場合（自分のコメントに対する自分の返信を除く）にのみ、レビュー担当者に送信されます。 つまり、配達確認の担当者が新しいコメントを作成した場合、レビュー担当者には通知されません。<p>この設定は、配達確認に関する他のコメントが通知されないように、また、自分のコメントに対する返信のみが通知されるように、配達確認のクライアントに対して推奨されます。</p><p>この電子メールアラート設定を持つレビュー担当者は、他の新しいコメントについては通知されませんが、校正ビューアでは、配達確認に関するすべてのコメントを表示できます。<br></p><p>詳しくは、 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">配達確認コメントを表示して返信します</a>.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">決定</td> 
      <td>レビュー担当者に電子メールが送信されるのは、誰かが決定したときだけです。<br><p>この電子メールアラートは、承認プロセスを管理する人（プロジェクトマネージャーなど）にとって役に立ちます。承認プロセスを管理する人が、配達確認の進行状況を監視し、どのユーザーが決定したかを確認できるからです。<br></p><p>決定を送信する際に電子メールの確認オプションを選択しない限り、自分の決定に関する通知は送信されません。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">最終決定</td> 
      <td>配達確認に関する最終決定がおこなわれると（配達確認の最後の承認者が決定を下したとき）、E メールが送信されます。<br><p>この警告は多くの場合、設計者が実際のレビューディスカッションに参加する必要がないので、設計者が使用します。 最終的な決定が下されると、デザイナーに通知が届き、必要な変更に対して対処できます。<br></p><p>このアラートは、レビュープロセスが完了した場合にのみ通知を受け取る必要がある部署のリーダーにも役立ちます。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">時間別サマリ</td> 
      <td>1 時間ごとにレビュー担当者に電子メールが送信され、過去 1 時間に発生したすべてのコメント、返信および決定の概要が記載されます。<br><p>この E メールは、過去 1 時間以内に自分自身のアクティビティが発生した場合にのみ送信されます。 他のユーザーからのアクティビティがない場合、E メールは送信されません。<br></p><p>このアラートは、プロジェクトの概要を確認するのに適しています。<br></p><p>この概要の使用例としては、プロジェクトの概要を必要とする上級レビュー担当者が挙げられますが、配達確認のすべてのアクティビティをすぐに通知する必要はありません。</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">日別概要</td> 
      <td>（デフォルト設定）:すべてのコメント、返信、決定が記載された電子メールが毎日送信されます。 メールは、自分以外にアクティビティがある日にのみ送信されます。<br><p>このアラートは、1 日を通じて複数の更新で圧倒されることなく、プロジェクトの概要を確認するのに適しています。<br></p><p>このサマリの使用例の 1 つに、部門のリーダーがプロジェクトの全体的な進行状況を監視する場合があります。<br></p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">メールなし</td> 
      <td>E メールアラートは送信されません。<br><p>この設定は、参照用としてのみ配達確認に追加され、変更を通知する必要がない人に役立ちます。</p><p>メモ: <p>このオプションは、配達確認のコメントや決定に関して受け取ることができる E メールアラートのみを無効にします。 新しい配達確認や遅延配達確認 E メールなど、配達確認のフローに関して受け取る E メールアラートを無効にすることはありません。 配達確認のフローに関する E メールアラートについて詳しくは、次の記事を参照してください。 </p>
        <ul>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-proof-email.md" class="MCXref xref">新しい配達確認 E メール</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/new-version-email.md" class="MCXref xref">新しいバージョンの電子メール</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/late-proof-email.md" class="MCXref xref">配達確認遅延 E メール</a></li>
         <li><a href="../../../workfront-proof/wp-emailsntfctns/proof-notifications-and-reminders/proof-made-email.md" class="MCXref xref">配達確認が E メールを送信しました</a></li>
        </ul></p></td> 
     </tr> 
    </tbody> 
   </table>
