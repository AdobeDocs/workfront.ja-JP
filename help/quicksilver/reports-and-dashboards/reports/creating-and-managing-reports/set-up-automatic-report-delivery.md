---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: レポートの自動配信のスケジュール設定
description: レポートの自動配信のスケジュール設定
author: Nolan
feature: Reports and Dashboards
exl-id: 5b8e382c-bfe8-43aa-aa09-a2aa0c4d56cc
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: ht
source-wordcount: '1164'
ht-degree: 100%

---

# レポートの自動配信のスケジュール設定

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: If this stays, fix links which now go to the reference article)</p>
-->

レポートをスケジュールして、定義したスケジュールに従ってユーザーに自動的に配信したり、1 回限りで手動でレポートを送信したりできます。Adobe Workfront からレポートを送信すると、ユーザーは Workfront レポートが添付されたメールが送信されます。

レポートの配信に影響を及ぼす可能性のあるサイズ制限などの情報について詳しくは、[レポート配信の概要](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md)を参照してください。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>プラン </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスの編集</p> <p>フィルター、ビュー、グループ化へのアクセスの編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限を管理します。</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 前提条件

開始する前に、レポートを作成する必要があります。レポートの作成について詳しくは、[カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)を参照してください。

## レポートの配信スケジュールの設定

レポートの自動配信スケジュールを設定したり、既存のレポート配信を編集または削除するには、次の手順に従います。

1. 配信スケジュールを設定するレポートに移動します。

   >[!NOTE]
   >
   >レポート配信にプロンプトは含まれていません。レポート配信のデータを制限する場合は、送信するレポートにフィルターを適用することをお勧めします。

1. **レポートのアクション**／**レポートを送信**&#x200B;をクリックします。

   **レポートを送信**&#x200B;ダイアログボックスが表示されます。

   >[!TIP]
   >
   >任意の時点でレポートを手動で送信するには、レポートに移動し、**レポートのアクション**／**レポートを送信**／**今すぐ送信**&#x200B;をクリックします。

1. 「**定期配信**」タブを選択します。
1. （条件付き）既存のレポートの定期配信を変更するには、「**定期配信**」セクションでレポート配信を選択します。
1. 次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>送信先</p> </td> 
      <td> <p>レポートの送信先となるユーザー、グループ、チーム、または役割の名前を入力し、ドロップダウンリストに表示された名前をクリックします。</p> <p>または</p> <p>レポートにアクセスする Workfront システム外のユーザーのメールアドレスを指定します。</p> <p>この手順を繰り返して、複数のユーザー、グループ、チームまたは役割にレポートを送信します。</p> <p>メモ：  <p>レポート配信の受信者を追加する際は、次の点を考慮してください。</p> 
        <ul> 
         <li>組織で Workfront 通知が特定のメールドメインに制限されている場合、メール許可リストにリストされているメールアドレスにのみレポートを送信できる場合があります。<p>Workfront 管理者がメールの許可リストを更新する方法について詳しくは、<a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md#configur" class="MCXref xref">メールの許可リストの設定</a>の節を参照してください。</p></li> 
         <li> <p>多数のユーザーを受信者として追加すると、配信が失敗する可能性があります。配信に失敗した場合は、小さなユーザーグループに対して複数のレポート配信をスケジュールできます。</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>メールの件名</p> </td> 
      <td> <p>メール通知の件名を指定します。</p> <p>デフォルトでは、メールの件名は次のようになります。</p> <p><em>Workfront レポート：[Name of the report] [Date]</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>メールのメッセージ</p> </td> 
      <td> <p>メールに含めるメッセージを指定します。</p> <p>デフォルトでは、メールのメッセージは次のようになります。</p> <p><em>[Date] に Workfront が生成した [report frequency] レポート [Name of the report] が添付されています。</em> </p> <p>メモ：Excel ファイルとして配信されるレポートのみに、次のメッセージがメールに追加されます。「MS Excel（XLS）ファイルタイプでは、サポートするハイパーリンクの数に制限（65,530）があることに注意してください。これらの制限を超えた場合、ファイルを開くことができないので、ハイパーリンクなしで再送信することをお勧めします。レポートスケジューラーに戻って、ハイパーリンクを削除してからレポートを再送信してください。」「レポートスケジューラーに戻って」というフレーズは、レポートに戻るリンクです。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>次のアクセス権限でこのレポートを配信</p> </td> 
      <td> <p>レポートにアクセスできるユーザーの名前を入力し、ドロップダウンリストに表示された名前をクリックします。レポートを受け取るユーザーには、ここで指定するユーザーと同じレベルのレポートへのアクセス権が付与されます。<br>詳しくは、<a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">別のユーザーのアクセス権を持つレポートの実行と配信</a>を参照してください。</p> <p>メモ：このフィールドではワイルドカードはサポートされません。例えば、ワイルドカード $$User.ID を使用しても、レポートを受け取ったユーザーのアクセス権を持つレポートは実行されません。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>形式</p> </td> 
      <td> <p>配信されるレポートの形式を選択します。</p> 
       <ul> 
        <li> <p>HTML</p> </li> 
        <li> <p>PDF</p> <p>これを選択すると、表示される追加の<strong>用紙サイズ</strong>と<strong>向き</strong>を使用して出力をフォーマットできます。</p> </li> 
        <li> <p>MS Excel（.xlsx）</p> </li> 
        <li> <p>TSV</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>リンクを含める</p> </td> 
      <td> <p>このオプションは、<strong>形式</strong>ドロップダウンメニューで <strong>MS Excel</strong> が選択されている場合にのみ使用できます。このオプションを有効にすると、書き出された Excel ドキュメントにハイパーリンクが含まれます。</p> <p>65,530 個を超えるリンクを含むドキュメントは開くことができません。書き出すドキュメントに 65,530 個を超えるリンクが含まれている場合は、このオプションの選択を解除します。</p> <p>このオプションは、デフォルトで有効になっています。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>概要</p> </td> 
      <td> <p>配信を繰り返すタイミングの概要を表示します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>繰り返し</p> </td> 
      <td> <p>レポートを毎日、毎週、毎月、毎年のどれで配信するかを選択します。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>繰り返す間隔</p> </td> 
      <td> <p>配信の繰り返し頻度を選択します。このオプションに選択する値は、<strong>繰り返し</strong>ドロップダウンリストで選択したオプションに基づきます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>時間</p> </td> 
      <td> <p>配信を送信する時刻を選択します。</p> <p>ヒント：システムの負荷はレポートの配信時間に影響を与える可能性があるので、スケジュールされた時間と実際の配信時間の間に遅延が生じる場合があります。特定の時間までに配信するレポートが必要な場合は、必要な時間の前に配信をスケジュールすることをお勧めします。例えば、配信が必要な日の前日に配信をスケジュールすることをお勧めします。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>曜日</p> </td> 
      <td> <p>このオプションは、<strong>繰り返し</strong>オプションが<strong>毎週</strong>または<strong>毎月</strong>に設定されている場合に使用できます。</p> 
       <ul> 
        <li> <p><strong>繰り返し</strong>オプションが<strong>毎週</strong>に設定されている場合：配信を送信する曜日を選択します。</p> </li> 
        <li> <p><strong>繰り返し</strong>オプションが<strong>毎月</strong>に設定されている場合：配信を月の特定日、曜日、または月末のいずれに送信するかを選択します（これらのオプションでは「<strong>開始日</strong>」で選択した日付を利用します）。</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>開始日</p> </td> 
      <td>スケジュールされた配信を開始する日付を選択します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>終了日</p> </td> 
      <td>スケジュールされた配信が終了する日付を選択します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>実行しない</p> </td> 
      <td>スケジュールされた配信を無期限に継続する場合、「<strong>実行しない</strong>」を選択します。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「**保存**」をクリックして、レポート配信を保存します。

   レポートは「**繰り返し配信**」セクション（「**レポートの送信**」ダイアログボックス内）に表示され、スケジュールされた時間に送信されます。

   レポートの配信に影響を与える可能性のあるサイズ制限について詳しくは、[レポートの配信制限](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#understanding-export-limits)および[書き出し制限](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#export)を参照してください。

1. （オプション）スケジュールされている配信を削除するには：

   1. **繰り返し配信**&#x200B;パネルで、スケジュールされている配信をクリックしてから、「**削除**」をクリックします。
   1. 「**削除**」をクリックして確認します。

## ビデオウォークスルー

レポート配信のスケジュール方法については、次のビデオをご覧ください。このビデオは Workfront Classic で録画されました。ただし、内容は新しい Workfront エクスペリエンスにも適用されます。

[![](assets/video-walk-through--350x197.png)](https://workfront-video.wistia.com/medias/45jffmll62)

<!--
<h2 data-mc-conditions="QuicksilverOrClassic.Draft mode">Additional information</h2>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">See also:</p>
-->

<!--
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/learningpath2/workfront-reporting-20Y0z000000blhLEAQ" target="_blank">Learning Path for reports and dashboards</a> </li>
  -->

<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode"><a href="https://one.workfront.com/s/basic-report-creation-program">Basic Report Creation Program for the new Workfront experience</a> </p>
  -->
