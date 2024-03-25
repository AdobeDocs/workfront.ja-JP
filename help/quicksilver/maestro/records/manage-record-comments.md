---
title: レコードコメントの管理
description: レコードの右側のパネルにコメントや返信を追加することで、Adobe Workfront Planning レコードで共同作業できます。 また、この領域で、記録に加えられた他の変更や記録を表示することもできます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
source-git-commit: a0f12a016ae8ac73136f05bf3255f9882e2ce6d4
workflow-type: tm+mt
source-wordcount: '1147'
ht-degree: 12%

---

# レコードコメントの管理

{{maestro-important-intro}}

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Maestro records" should be there-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->

レコードの右側のパネルにコメントや返信を追加することで、Adobe Workfront Planning レコードで共同作業できます。 また、この領域で、記録に加えられた他の変更や記録を表示することもできます。

レコードの右側のパネルには、次のセクションが表示されます。

* **コメント**：ユーザーがレコードに追加したコメントおよび返信を表示します。
* **履歴**：ユーザーがレコードフィールドに対しておこなった、システムで記録された変更を表示します。 詳しくは、 [履歴セクションの概要](/help/quicksilver/maestro/records/history-section-overview.md).

## レコードにコメントする際の考慮事項

* レコードの「コメント」セクションで、Workfront計画のレコードにコメントや返信を追加できます。

* リンクされたレコードに追加されたコメントは、リンク元のレコードには表示されません。 例えば、Campaign レコードにリンクされているWorkfront Planning Product レコードにコメントすると、そのコメントはWorkfront Planning の Product レコードにのみ表示され、リンク元の Campaign レコードには表示されません。

* レコードと別のアプリケーションのオブジェクトとの接続の結果として作成されたWorkfront Planning レコードにコメントを追加できます。

  例えば、WorkfrontプロジェクトをWorkfront planning レコードに接続した後で、Project Workfront planning レコードにコメントを付けることができます。 詳しくは、 [レコードを接続](/help/quicksilver/maestro/records/connect-records.md).

* 他のアプリケーションでリンクされたオブジェクトに追加されたコメントは、Workfront計画では表示されず、Workfront計画でリンクされたオブジェクトに追加されたコメントは、他のアプリケーションでは表示されません。

  例えば、Workfrontでプロジェクトに追加したコメントは、Workfront計画のキャンペーンにリンクされた同じプロジェクトには表示されず、プロジェクトWorkfront計画レコードに追加したコメントはWorkfrontには表示されません。

* ユーザーにタグを付けて、更新に注意を向けることができます。 タグ付きユーザーは、アプリ内通知や更新に関する電子メールを受け取りません。 <!--this might change??-->

* レコードに更新を追加し、Workfront計画の次の領域で変更履歴を確認できます。

   * レコードの詳細ページから。

  <!--* From the table view.-->

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> 製品</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront協定</p></td>
   <td>
<p>組織がAdobe Workfront Planning ベータプログラムに登録されている必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront プラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront ライセンス</p></td>
   <td>
   <p>任意</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader"><p>アクセスレベルの設定</p></td>
   <td> <p>Workfront計画には、アクセスレベルの制御はありません。 </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに対する表示権限以上の権限</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfrontまたはグループ管理者は、レイアウトテンプレートに計画領域を追加する必要があります。 詳しくは、 <a href="../access/access-overview.md">アクセスの概要</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

### レコードに対するコメントの管理

{{step1-to-maestro}}

最後にアクセスしたワークスペースは、デフォルトで開きます。
1. 次の場所からテーブルビューを選択します。 **表示** ドロップダウンメニュー。
1. テーブルビューでレコードの名前をクリックします。

   レコードの **詳細** ページが開きます。 「コメント」領域は、デフォルトでは右側のパネルに開きます。

1. （条件付き）デフォルトで右側のパネルが開かない場合は、 **コメントを表示** ![](assets/show-comments-icon.png) アイコンを使用して、「コメント」セクションを開きます。

1. **新しいコメント**&#x200B;ボックスにコメントを入力します。

   ![](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >コメントを入力して送信する前に「コメント」セクションから移動すると、ログオフしてログオンし直した後でも、ページ上のコメントはドラフトモードのままになります。 コメントに追加された画像も下書きに保存されます。ドラフトは 7 日間保存され、その後は破棄され、復元できません。下書きのコメントは、入力したユーザーのみに表示されます。

1. （オプション）変更の取り消しまたはやり直しを行うには、以下のショートカットキーを使用します。
   * Ctrl + Z（Mac の場合は ⌘+z）で、変更を元に戻します
   * Ctrl + Y（Mac の場合は ⌘+y）で、変更をやり直します
1. （オプション） **@** 更新時に、誰かにタグを付けるユーザーの名前が続きます。
1. （オプション）リッチテキストツールバーのオプションを使用して、テキストの書式設定、絵文字、リンク、画像を更新に追加し、コンテンツを拡張できます。 詳しくは、この記事の「Workfrontの更新でのリッチテキストの使用」の節を参照してください [作業を更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   >[!TIP]
   >
   >別のユーザーが、更新しようとしている同じ項目にコメントを送信した場合、赤い線に「新規」インジケータが表示され、新しいコメントが通知されます。
   >
   >インジケーターは、コメントが項目に送信された後にのみ表示され、コメントがまだ構成されている場合は表示されません。
   >
   >![](assets/new-line-indicator-comments.png)

1. クリック **送信** をクリックして、レコードに更新を追加します。
1. （オプション）コメントを編集するには、 **その他** メニュー ![](assets/more-menu.png) コメントの右上隅で、 **編集**.

   >[!IMPORTANT]
   >
   >コメントは送信後 15 分以内にのみ編集できます。

1. コメント内の情報の編集、画像の追加や削除、タグ付きユーザーの削除をおこないます。 コメントの左側に「編集済み」のインジケーターが追加されます。

   >[!TIP]
   >
   >現在の年からのコメントでは、日付スタンプに年は表示されません。 タイムスタンプの上にマウスポインターを置くと、年を含む完全な日付が表示されます。

1. （オプションおよび条件付き）既存のコメントを検索するには、まず、 **コメント** 領域。

   ![](assets/search-box-for-comments-area.png)

1. （オプション）「 **返信** または、 **返信を追加…** 領域に移動し、既存のコメントに返信するには、上記の手順 4～8 に従います。 <!--(**************accurate??***********)-->

1. （条件付きおよびオプション）コメントの追加中に「コメント」セクションの表示領域の外側に表示されるコメントを他のユーザーが追加した場合は、「 **表示** 内側 **新しいコメントバナー** をクリックして、これらのコメントを表示します。

   ![](assets/new-comments-banner-on-record.png)

   追加のコメントが画面の下部に表示されます。

1. （オプション） **次に類似** アイコンをクリックして、更新を「いいね！」にしたり、自分が読んだことを確認したりします。 アイコンは「いいね！」の数に応じて更新されます。
1. （条件付きおよびオプション）コメントに追加の人を含める場合は、更新に含まれるユーザーのアバターをクリックして、コメントの共有先ユーザーのリストを表示します。
1. （オプション） **その他** アイコン ![](assets/more-menu.png) コメントの右上隅で、次のいずれかのオプションをクリックして、コメントから情報をコピーします。

   * **リンクをコピー**：コメントへのリンクをクリップボードにコピーします。
   * **本文をコピー**：コメントのテキストをクリップボードにコピーします。
   * **見積もりの返信**：コメントの内容を新しい返信にコピーします。 コピーされた返信に画像は含まれません。

   詳しくは、[作業の更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)を参照してください。
1. （オプション） **その他** アイコン ![](assets/more-menu.png) コメントの右上隅で、 **削除** をクリックしてコメントを削除します。
1. （オプション） **注釈を非表示** アイコン ![](assets/hide-comments-icon.png) をクリックして、右側のパネルを閉じます。

## 履歴セクションの概要

レコードに加えた変更は、レコードの右側のパネルの「履歴」セクションで確認できます。

詳しくは、 [履歴セクションの概要](/help/quicksilver/maestro/records/history-section-overview.md).
