---
product-area: documents;setup
navigation-topic: review-a-proof
title: 校正ビューアの設定を行う
description: Web 校正ビューアとデスクトップ校正ビューアの両方の設定を構成できます。
author: Courtney
feature: Digital Content and Documents
exl-id: 3993cd67-90a9-4d7e-bbc0-7b9bd1057f54
source-git-commit: ae80999fc7ea7e35097560aa99baa435bcd31b74
workflow-type: tm+mt
source-wordcount: '1408'
ht-degree: 0%

---

# 校正ビューアの設定を行う

Web 校正ビューアとデスクトップ校正ビューアの両方で、次の設定を構成できます。

* コメントのマークアップとピンを配達確認に表示するかどうかを指定します。
* マークアップツールが校正ビューアの上部に表示されるか、ドロップダウンメニューに表示されるかを指定します。
* 開いている配達確認のレビュー担当者として受け取る電子メール通知。

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the Desktop Proofing Viewer is the default viewer for all types of proofs (static and video, as well as interactive).</li>
  -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">For comparative information about the Web Proofing Viewer and the Desktop Proofing Viewer, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p>
-->

デスクトップ校正ビューアに対して、次の設定を構成できます。

* Web サイトのコンテンツ内のリンクをビューアで開く方法。

  <!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode">Whether the background color of the Desktop Proofing Viewer is the default near-black color or white.</li>
  -->

* 新しいブラウザータブまたはウィンドウで開くように設定されているリンクをクリックしたときの動作。
* ポップアップ（ブラウザーのキャッシュデータによってブロックされる可能性がある）などのコンテンツをビューアに表示できるようにするには、表示中の配達確認と共に保存されるキャッシュデータをクリアします。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>現在のプラン： Pro 以上</p> <p>または</p> <p>レガシープラン： Select または Premium</p> <p>様々なプランでのアクセスの検証について詳しくは、 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfrontの校正機能へのアクセス</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>現在のプラン：作業またはプラン</p> <p>レガシープラン：任意（ユーザーの校正が有効になっている必要があります）</p> </td> 
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

## 校正ビューアの設定を行う

校正ビューアを設定するには：

1. 次のいずれかの方法で、Web 校正ビューアまたはデスクトップ校正ビューアを開きます。

   * Adobe Workfront内で配達確認を行う場合は、表示する配達確認を含むドキュメントリストに移動し、ドキュメントの上にマウスポインターを置いて、「 **配達確認を開く**.
   * Workfront Proof を使用する場合は、 **配達確認に移動** ダッシュボードまたは表示リストの配達確認のアイコン ![](assets/go-to-proof-blue-icon.png).

1. 左側のツールバーが表示されていない場合は、 **メニュー** アイコン（Web 校正ビューアの左上隅）

   ![](assets/menu-icon-in-proofing-viewer-350x228.png)

1. 左側のツールバーで、 **設定** アイコン ![](assets/settings-icon-in-pv.png).

1. 次のいずれかを設定します。 **設定** 表示されます。

   使用できる設定は、開いている配達確認の種類によって異なる場合があります。

   * **マークアップを表示** （常に Web 校正ビューアおよびデスクトップ校正ビューアで使用可能）：校正者がマークアップツールを使用する際に校正に追加するコメントマークです。 無効にした場合でも、コメントリストでコメントをクリックすると、そのコメントが表示されます。

     この設定は、開いているすべての配達確認に影響します。

   * **ピンを表示** （常に Web 校正ビューアおよびデスクトップ校正ビューアで使用可能）：校正者がマークアップツールを使用する際に配達確認に追加する番号付きのピンです。 レビュー担当者がコメントを追加した場所と順序を示します。 無効にした場合でも、コメントリストでコメントをクリックすると、そのコメントが表示されます。

     この設定は、開いているすべての配達確認に影響します。

   * **拡張マークアップツールを使用** （常に Web 校正ビューアおよびデスクトップ校正ビューアで使用可能）：既定では、校正ビューアの上部にマークアップツールのオプションが表示されます。 これらを、クリックしたときにのみ開く縦並びのメニューに表示するように設定できます。

     この設定は、開いているすべての配達確認に対して有効です。

   * **次に関する電子メール通知を受け取る** （常に Web 校正ビューアおよびデスクトップ校正ビューアで使用可能）：以下のオプションの 1 つをクリックします。 この設定は、開いている配達確認にのみ影響します。 詳しくは、 [配達確認コメントおよび決定の通知の概要](../../../review-and-approve-work/proofing/proofing-overview/notifications-proof-comments-decisions.md).

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">すべてのアクティビティ</td> 
        <td>Workfrontは、新しいコメント、返信、決定など、配達確認に関するアクティビティが発生するたびにレビュー担当者に電子メールを送信します。 <p>これは、アクティビティの発生を確認できるので、校正プロセスを管理するユーザーにとって最適なオプションです。 </p><p>ユーザーは、自分のアクティビティに関する電子メールアラートを受け取りません。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">自分のコメントへの返信</td> 
        <td>メールは、誰かが自分のコメントに明示的に返信した場合（自分のコメントに対する自分の返信を除く）にのみ、レビュー担当者に送信されます。 つまり、配達確認の担当者が新しいコメントを作成した場合、レビュー担当者には通知されません。<p>この設定は、配達確認に関する他のコメントが通知されないように、また、自分のコメントに対する返信のみが通知されるように、配達確認のクライアントに対して推奨されます。</p><p>この電子メールアラート設定を持つレビュー担当者は、他の新しいコメントについては通知されませんが、校正ビューアでは、配達確認に関するすべてのコメントを表示できます。</p><p>コメントについて詳しくは、 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/comment-on-a-proof/view-proof-comments.md" class="MCXref xref">配達確認コメントを表示して返信します</a>.</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">決定</td> 
        <td>Workfrontは、誰かが決定した場合にのみ、レビュー担当者に電子メールを送信します。<p>これは、承認プロセスを管理し、配達確認の進行状況を監視し、どのユーザーが決定したかを確認する必要がある人（プロジェクトマネージャーなど）に役立ちます。</p><p>決定を送信する際に電子メールの確認オプションを選択しない限り、自分の決定に関する通知は送信されません。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">最終決定</td> 
        <td>Workfrontは、配達確認の最後の承認者が決定したときに電子メールを送信します。<p>この警告は多くの場合、実際のレビューディスカッションに参加する必要がないデザイナーが使用します。 最終的な決定が下されると、デザイナーに通知が届き、必要な変更に対して対処できます。</p><p>このアラートは、レビュープロセスが完了した場合にのみ通知を受け取る必要がある部署のリーダーにも役立ちます。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">時間別サマリ</td> 
        <td>Workfrontは、1 時間ごとにレビュー担当者に電子メールを送信し、1 時間ごとに発生したすべてのコメント、返信および決定の概要を記載します。<p>この E メールは、過去 1 時間以内に自分自身のアクティビティが発生した場合にのみ送信されます。 </p><p>このアラートは、プロジェクトの概要を確認するのに適しています。</p><p>この概要の使用例としては、プロジェクトの概要を必要とする上級レビュー担当者が挙げられますが、配達確認のすべてのアクティビティをすぐに通知する必要はありません。</p></td> 
       </tr> 
       <tr> 
        <td role="rowheader">日別サマリ</td> 
        <td>Workfrontは、自分の以外にアクティビティがある日にのみ、すべてのコメント、返信および決定を記載した 1 つの電子メールを送信します。<p>このアラートは、1 日を通じて複数の更新で圧倒されることなく、プロジェクトの概要を確認するのに適しています。</p><p>このサマリの使用例の 1 つに、部門のリーダーがプロジェクトの全体的な進行状況を監視する場合があります。</p><p>詳しくは、 <a href="../../../review-and-approve-work/proofing/reviewing-proofs-within-workfront/manage-notifications-for-proof-comments.md" class="MCXref xref">配達確認のコメントおよび決定に関する通知を管理</a>.</p></td> 
       </tr> 
       <tr data-mc-conditions=""> 
        <td role="rowheader">メールなし</td> 
        <td>Workfrontは電子メールアラートを送信しません。<br>これは、参照用としてのみ配達確認に追加され、変更を通知する必要がない人に役立ちます。<p>システムのデフォルトは、「毎日の概要」（「未設定」とも呼ばれます）です。 自分または自分のレビュー担当者が他の変更を加えない場合、すべての配達確認にこの設定が適用されます。</p></td> 
       </tr> 
      </tbody> 
     </table>

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p><strong>Use desktop app as default</strong>: By default, static and video proofs open in the Web Proofing Viewer in your web browser, and interactive proofs open in the Desktop Proofing Viewer app. This setting lets you configure the Desktop Proofing Viewer as the default viewer for all types of proofs (static and video, as well as interactive). For more information about this setting, see in the article . For comparative information about the two viewers, see <a href="../../../review-and-approve-work/proofing/proofing-overview/understand-differences-between-web-viewer.md" class="MCXref xref">Differences between the Web Proofing Viewer and the Desktop Proofing Viewer overview</a>.</p> </li>   
     -->

   * **配達確認のハイパーリンクをクリックするとき** （デスクトップ校正ビューアでのみ使用可能）：新しいブラウザのタブまたはウィンドウで開くように設定されたリンクをクリックしたときにデスクトップ校正ビューアで行う処理を指定するオプションを選択します。

     この設定は、開いているすべてのインタラクティブな配達確認に対して有効です。

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">校正ビューア内で開く</td> 
        <td>リンクは常にデスクトップ校正ビューア内で開き、リンクされたコンテンツを校正できます。 </td> 
       </tr> 
       <tr> 
        <td role="rowheader">ブラウザーで開く</td> 
        <td>リンクは常にブラウザー内で開き、校正ビューアーでは開きません。 リンクされたコンテンツの配達確認を実行できません。</td> 
       </tr> 
       <tr> 
        <td role="rowheader">毎回確認する</td> 
        <td> <p>デスクトップ校正ビューア内でリンクを開くか、ブラウザでリンクを開くかを尋ねるメッセージが表示されます。 デスクトップ校正ビューア内でリンクを開くと、リンクされたコンテンツを校正できます。 ブラウザーでリンクを開くと、リンクされたコンテンツの配達確認ができなくなります。</p> <p> <img src="assets/proof-desktop-alwaysask-350x243.png" alt="proof_desktop_alwaysask.png" style="width: 350;height: 243;"> </p> <p>この設定は、開いている配達確認にのみ影響します。</p> </td> 
       </tr> 
      </tbody> 
     </table>

     <!--   
     <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><strong>Background color</strong> (available when you open interactive content in the Desktop Proofing Viewer or Web Proofing Viewer): Change the background color of the Desktop Proofing Viewer from the default near-black color to white. This can make it easier to see interactive content that has a transparent background instead of a white background.</li>   
     -->

   * **キャッシュをクリア**：表示中のインタラクティブ配達確認と共に保存される可能性のあるブラウザーキャッシュデータをクリアします。 これにより、ポップアップなどのコンテンツ（ブラウザーのキャッシュデータによってブロックできる）をデスクトップ校正ビューアに表示できます。

     クリアされるデータには、HTTP キャッシュ（次のページの更新後に再利用される画像など）と Web ストレージデータキャッシュ（ユーザーを識別する Cookie やデータなど）が含まれます。

     この設定は、開いている配達確認にのみ影響します。
