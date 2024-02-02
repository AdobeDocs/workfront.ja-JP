---
product-area: documents
navigation-topic: manage-proofs-within-workfront
title: プルーフのレビュアーにメールメッセージを送信する
description: レビューおよび承認プロセス中に、プルーフの 1 人またはすべてのレビュアーにメッセージを送信できます。メッセージは、プルーフのレビューを完了するか、プルーフに関連するその他の情報を提供するようにレビュアーに通知する簡単な方法です。
author: Courtney
feature: Digital Content and Documents
exl-id: e7d60d6f-b6bd-4082-b50c-e42d4b72c149
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: ht
source-wordcount: '439'
ht-degree: 100%

---

# プルーフのレビュアーにメールメッセージを送信する

レビューおよび承認プロセス中に、プルーフの 1 人またはすべてのレビュアーにメッセージを送信できます。メッセージは、プルーフのレビューを完了するか、プルーフに関連するその他の情報を提供するようにレビュアーに通知する簡単な方法です。

一般的なリマインダーメールを送信するか、特定のステージに関連付けられた 1 人またはすべてのユーザーにカスタマイズされたメッセージを送信するかを選択できます。

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
   <td role="rowheader">プルーフの役割</td> 
   <td>作成者またはモデレーター</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、役割、またはプルーフ権限プロファイルを確認するには、Workfront または Workfront プルーフの管理者に問い合わせてください。

## プルーフのユーザーにメールメッセージを送信

1. メッセージを送信するユーザーが含まれるプルーフのドキュメントを検索します。
1. ドキュメントにポインタを合わせ、「**プルーフのワークフロー**」をクリックします。

   ![](assets/proof-workflow-doc-list-350x92.png)

1. ステージ上のすべてのユーザーにメッセージを送信するには、ステージ上の&#x200B;**その他**&#x200B;メニューをクリックし、「**全員にメッセージを送信**」を選択します。

   ![](assets/message-stage-350x122.png)

1. 個々のユーザーにメッセージを送信するには、ユーザーの横にある&#x200B;**その他**&#x200B;メニューをクリックし、「**メッセージ**」を選択します。

   ![](assets/message-user-350x121.png)

1. 「**メッセージの詳細**」セクションで、以下の情報を指定します。

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">メールで担当者に通知</td> 
      <td>このオプションは選択解除できません。すべてのユーザーがメールでメッセージを受け取ります。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">カスタムメッセージを破棄</td> 
      <td> <p>デフォルトのメールコンテンツのみを含める場合は、「<strong>カスタムメッセージを破棄</strong>」をクリックします。</p> <p>デフォルトのリマインダーメールには、次の情報が含まれます。</p> 
       <ul> 
        <li>プルーフ画像のプルーフ <br> サムネールへの個人リンク<br></li> 
        <li>以下のプルーフの詳細：プルーフの名前、バージョン番号、フォルダー名（該当する場合）、レビュアーとプルーフに関する進捗状況のリスト。</li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">件名</td> 
      <td>メッセージの件名を入力します。</td> 
     </tr> 
     <tr> 
      <td role="rowheader">メッセージ</td> 
      <td>メッセージのコンテンツを入力します。</td> 
     </tr> 
    </tbody> 
   </table>

1. 「**送信**」をクリックします。
