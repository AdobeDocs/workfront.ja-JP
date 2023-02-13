---
product-area: reporting;setup
navigation-topic: create-and-manage-reports
title: 自動レポート配信のスケジュール設定
description: 自動レポート配信のスケジュール設定
author: Nolan
feature: Reports and Dashboards
exl-id: 5b8e382c-bfe8-43aa-aa09-a2aa0c4d56cc
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '1164'
ht-degree: 3%

---

# 自動レポート配信のスケジュール設定

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: If this stays, fix links which now go to the reference article)</p>
-->

レポートをスケジュールして、定義したスケジュールに従ってユーザーに自動的に配信したり、1 回限りに手動でレポートを送信したりできます。 Adobe Workfrontからレポートを送信すると、そのユーザーは、別の添付ファイルでWorkfrontレポートが記載された電子メールを受け取ります。

レポートの配信に影響を及ぼす可能性のあるサイズ制限などについて詳しくは、 [レポート配信の概要](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md).

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
   <td> <p>計画 </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>レポート、ダッシュボード、カレンダーへのアクセスを編集</p> <p>フィルター、ビュー、グループへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>レポートに対する権限の管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

開始する前に、レポートを作成する必要があります。 レポートの作成について詳しくは、 [カスタムレポートの作成](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

## レポートの配信スケジュールの設定

レポートの自動配信スケジュールを設定したり、既存のレポート配信を編集または削除するには、次の手順に従いま&#x200B;す。

1. 配信のスケジュールを設定するレポートに移動します。

   >[!NOTE]
   >
   >レポート配信にプロンプトは含まれていません。 レポート配信のデータを制限する場合は、送信するレポートにフィルターを適用することをお勧めします。

1. クリック **レポートのアクション**&#x200B;を、 **レポートの送信**.

   この **レポートの送信** ダイアログボックスが表示されます。

   >[!TIP]
   >
   >任意の時点でレポートを手動で送信するには、レポートに移動し、 **レポートのアクション** > **レポートの送信** > **今すぐ送信**.

1. を選択します。 **配信の繰り返し** タブをクリックします。
1. （条件付き）既存の繰り返しレポートの配信を変更するには、 **配信の繰り返し** 」セクションに入力します。
1. 次の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>送信先</p> </td> 
      <td> <p>レポートの送信先となるユーザー、グループ、チーム、または役割の名前を入力し、ドロップダウンリストに表示されたら名前をクリックします。</p> <p>または</p> <p>レポートにアクセスするWorkfrontシステム外のユーザーの電子メールアドレスを指定します。</p> <p>この手順を繰り返して、複数のユーザー、グループ、チームまたは役割にレポートを送信します。</p> <p>メモ:  <p>レポート配信の受信者を追加する際は、次の点を考慮してください。</p> 
        <ul> 
         <li>組織でWorkfront通知が特定の電子メールドメインに制限されている場合は、電子メールドメインに一覧表示されている電子メールアドレスにのみレポートを送信でき許可リストます。<p>Workfront管理者が E メール管理を更新する方法について詳しくは、「 許可リスト <a href="../../../administration-and-setup/get-started-wf-administration/configure-your-email-allowlist.md#configur" class="MCXref xref">電子メールの設定を許可リスト行う</a>.</p></li> 
         <li> <p>多数のユーザーを受信者として追加すると、配信が失敗する可能性があります。 配信に失敗した場合は、小さなユーザーグループと共に複数のレポート配信をスケジュールできます。</p> </li> 
        </ul> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>E メールの件名</p> </td> 
      <td> <p>電子メール通知の件名を指定します。</p> <p>デフォルトでは、電子メールの件名は次のようになります。</p> <p><em>Workfrontレポート：[ レポート名 ] [ 日付 ]</em> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>E メール メッセージ</p> </td> 
      <td> <p>電子メールに含めるメッセージを指定します。</p> <p>デフォルトでは、電子メールメッセージは次のようになります。</p> <p><em>[Date] にWorkfrontが生成した [report frequency] report [Name of the report] が添付されています。</em> </p> <p>注意：レポートが Excel ファイルとしてのみ配信される場合は、次のメッセージも電子メールに追加されます。「MS Excel (XLS) ファイルタイプでは、これらのファイルタイプがサポートするハイパーリンクの数に制限 (65,530) があることに注意してください。 これらの制限を超えると、ファイルは開かれず、ハイパーリンクなしで再送信することをお勧めします。 レポートスケジューラに戻って、ハイパーリンクを削除してレポートを再送信してください。 「レポートスケジューラに戻ってください」というフレーズは、レポートに戻るリンクです。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>次のアクセス権限でこの報告書を届ける</p> </td> 
      <td> <p>レポートにアクセスできるユーザーの名前を入力し始め、ドロップダウンリストに表示されたら名前をクリックします。 レポートを受け取るユーザーには、ここで指定するユーザーと同じレベルのレポートへのアクセス権が付与されます。<br> 詳しくは、 <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">別のユーザーのアクセス権を持つレポートの実行と配信</a>.</p> <p>注意：このフィールドではワイルドカードを使用できません。 例えば、ワイルドカード$$User.ID を使用しても、レポートを受け取ったユーザーのアクセス権を持つレポートは実行されません。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>形式</p> </td> 
      <td> <p>配信されるレポートの形式を選択します。</p> 
       <ul> 
        <li> <p>HTML</p> </li> 
        <li> <p>PDF</p> <p>これを選択した場合、 <strong>用紙サイズ</strong> および <strong>向き</strong> 表示されるオプション。</p> </li> 
        <li> <p>MS Excel (.xlsx)</p> </li> 
        <li> <p>TSV</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>リンクを含める</p> </td> 
      <td> <p>このオプションは、 <strong>MS Excel</strong> が <strong>形式</strong> ドロップダウンメニュー。 このオプションを有効にすると、書き出された Excel ドキュメントにハイパーリンクが含まれます。</p> <p>65,530 個を超えるリンクを含むドキュメントは開くことができません。 書き出すドキュメントに 65,530 個を超えるリンクが含まれている場合は、このオプションの選択を解除します。</p> <p>このオプションは、デフォルトで有効になっています。</p> </td> 
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
      <td> <p>配信の繰り返し頻度を選択します。 このオプションで選択する値は、 <strong>繰り返し</strong> 」ドロップダウンリストから選択できます。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>時間</p> </td> 
      <td> <p>配信を送信する時刻を選択します。</p> <p>ヒント：システムの負荷はレポートの配信時間に影響を与える可能性があるので、予定時間と実際の配信時間の間に遅延が生じる場合があります。 特定の時間までに配信するレポートが必要な場合は、必要な時間に配信をスケジュールすることをお勧めします。 例えば、配信のスケジュールを必要な日付の前に設定することをお勧めします。</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>曜日</p> </td> 
      <td> <p>このオプションは、 <strong>繰り返し</strong> オプションは次のいずれかに設定されます。 <strong>毎週</strong> または <strong>毎月</strong>:</p> 
       <ul> 
        <li> <p>次の場合に <strong>繰り返し</strong> オプションが <strong>毎週</strong>:配信を送信する曜日を選択します。</p> </li> 
        <li> <p>次の場合に <strong>繰り返し</strong> オプションが <strong>毎月</strong>:配信を月の当日、曜日、または月の最終日のどちらに送信するかを選択します ( これらのオプションでは <strong>開始日</strong> フィールド ) に書き込まれます。</p> </li> 
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
      <td>選択 <strong>なし</strong> スケジュールされた配信を無期限に継続する場合。</td> 
     </tr> 
    </tbody> 
   </table>

1. クリック **保存** をクリックして、レポート配信を保存します。

   レポートが **配信の繰り返し** セクション ( **レポートの送信** ダイアログボックスに表示されます )。スケジュールされた時刻に送信されます。

   レポートの配信に影響を与える可能性のあるサイズ制限について詳しくは、 [レポートの配信制限](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#understanding-export-limits) および [書き出し制限](../../../reports-and-dashboards/reports/creating-and-managing-reports/set-up-report-deliveries.md#export).

1. （オプション）予定されている配信を削除するには：

   1. 内 **配信の繰り返し** パネルで、予定されている配信をクリックしてから、 **削除**.
   1. クリック **削除** をクリックして確定します。

## ビデオウォークスルー

レポート配信のスケジュール方法については、次のビデオをご覧ください。 このビデオはWorkfront Classic で録画されました。 ただし、内容は新しいWorkfrontエクスペリエンスにも適用されます。

[ ![](assets/video-walk-through--350x197.png)](https://workfront-video.wistia.com/medias/45jffmll62)

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
