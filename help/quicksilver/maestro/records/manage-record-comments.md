---
title: レコードのコメントの管理
description: レコードの右側のパネルにコメントや返信を追加することで、Adobe Workfront Planning レコードに関する共同作業を行うことができます。 また、レコードに加えられた他の変更や、システムによってこの領域に記録された変更も表示できます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
source-git-commit: 024c612d46848c55529e902a00d481588d261584
workflow-type: tm+mt
source-wordcount: '1153'
ht-degree: 29%

---

# レコードのコメントの管理

{{maestro-important-intro}}

<!--update the metadata with real information when making this available in TOC and in the left nav-->

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Maestro records" should be there-->

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. </span>

<span class="preview">For information about the current release schedule, see [First Quarter 2024 release overview](/help/quicksilver/product-announcements/product-releases/24-q1-release-activity/24-q1-release-overview.md).</span> -->

レコードの右側のパネルにコメントや返信を追加することで、Adobe Workfront Planning レコードに関する共同作業を行うことができます。 また、レコードに加えられた他の変更や、システムによってこの領域に記録された変更も表示できます。

レコードの右側のパネルには、次のセクションが表示されます。

* **コメント**：ユーザーがレコードに追加したコメントと返信を表示します。
* **履歴**：レコードフィールドに対してユーザーがおこなったシステム記録の変更を表示します。 詳しくは、[「履歴」セクションの概要](/help/quicksilver/maestro/records/history-section-overview.md)を参照してください。

## レコードに対するコメントに関する考慮事項

* Workfront Planning のレコードのコメントと返信は、レコードの「コメント」セクションに追加できます。

* リンク元のレコードには、リンクされたレコードに追加されたコメントは表示されません。 例えば、キャンペーンレコードにリンクされたWorkfront Planning の商品レコードにコメントを付けると、コメントはWorkfront Planning の商品レコードにのみ表示され、リンク元のキャンペーンレコードには表示されません。

* レコードと他のアプリケーションのオブジェクトとの関連付けの結果として作成されたWorkfront Planning レコードにコメントを追加できます。

  例えば、Workfront プロジェクトをWorkfront計画レコードと結び付けた後で、プロジェクト Workfront計画レコードにコメントできます。 詳しくは、[レコードの接続](/help/quicksilver/maestro/records/connect-records.md)を参照してください。

* 他のアプリケーションでリンク・オブジェクトに追加されたコメントはWorkfront Planning に表示されず、Workfront Planning でリンク・オブジェクトに追加されたコメントは他のアプリケーションでは表示されません。

  例えば、Workfrontのプロジェクトに追加されたコメントは、Workfront計画のキャンペーンにリンクされた同じプロジェクトには表示されず、プロジェクトのWorkfront計画レコードに追加されたコメントはWorkfrontには表示されません。

* ユーザーにタグを付けて、最新情報をユーザーに伝えることができます。 タグ付けされたユーザーには、アプリ内通知や更新に関するメールは届きません。 <!--this might change??-->

<!--replace the bullet above with this: * You can tag users to bring their attention to an update. Tagged users receive an in-app notification or an email notification about your update. 
   The following scenario exists:   

   * Adobe Unified Experience users receive both an in-app notification and an email notification. 
   * Users who are not in the Adobe Unified Experience receive only an email notification. 

      For information, see [Adobe Workfront Planning notifications: article index](/help/quicksilver/maestro/notifications/notifications-information.md)
   
      To determine whether your company is using the Adobe Unified Experience, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).
      -->

* レコードに更新を追加し、Workfront Planning の次の領域から変更履歴を確認できます。

   * レコードの詳細ページから。
   * ビューの「レコードの詳細」ボックスに移動します。

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
 <td role="rowheader"><p>Adobe Workfront の契約</p></td>
   <td>
<p>Adobe Workfront Planning ベータ版プログラムに登録されている必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
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
   <td> <p>Workfront Planning には、アクセス レベルのコントロールはありません。 </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>権限</p></td>
   <td> <p>ワークスペースに対する表示以上の権限</a> </p>  
   <p>システム管理者は、自身が作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>レイアウトテンプレート</p></td>
   <td> <p>Workfront管理者またはグループ管理者が、レイアウトテンプレートにプランニング エリアを追加する必要があります。 詳しくは、<a href="../access/access-overview.md">アクセス権の概要</a>を参照してください。 </p>  
</td>
  </tr>
 </tbody>
</table>

### レコードに対するコメントの管理

{{step1-to-maestro}}

最後にアクセスしたワークスペースは、デフォルトで開きます。
1. 「」からのテーブルビューの選択 **表示** ドロップダウンメニュー。
1. テーブル表示でレコードの名前をクリックします。

   レコードの **詳細** ページが開きます。 コメント領域は、デフォルトでは右側のパネルに開きます。

1. （条件付き）デフォルトで右側のパネルが開かない場合は、 **コメントを表示** ![](assets/show-comments-icon.png) 右上隅のアイコンで「コメント」セクションを開きます。

1. **新しいコメント**&#x200B;ボックスにコメントを入力します。

   ![](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >入力を完了してコメントを送信する前に「コメント」セクションから移動すると、ログオフしてログオンし直した後も、コメントがドラフトモードでページに保持されます。 コメントに追加された画像も下書きに保存されます。ドラフトは 7 日間保存され、その後は破棄され、復元できません。下書きのコメントは、入力したユーザーのみに表示されます。

1. （オプション）変更の取り消しまたはやり直しを行うには、以下のショートカットキーを使用します。
   * Ctrl + Z（Mac の場合は ⌘+z）で、変更を元に戻します
   * Ctrl + Y（Mac の場合は ⌘+y）で、変更をやり直します
1. （任意）追加 **@** に続き、更新内のユーザーをタグ付けするユーザーの名前。

   <!--Adobe Unified Experience users can receive an in-app and an email notification when they are tagged. All other users receive an email when they are tagged. For more information, see the section [Considerations about commenting on a record](#considerations-about-commenting-on-a-record) in this article. -->

1. （オプション）リッチテキストツールバーのオプションを使用すると、テキストの書式設定や、更新への絵文字、リンクまたは画像の追加を行って、コンテンツを拡充できます。詳しくは、「Workfrontの更新でのリッチテキストの使用」の節を参照してください [作業の更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   >[!TIP]
   >
   >更新中のアイテムに別のユーザーがコメントを送信した場合、「新規」インジケーターと赤い線が表示され、新しいコメントが通知されます。
   >
   >インジケーターは、コメントが項目に送信された後にのみ表示され、コメントがまだ構成されている場合は表示されません。
   >
   >![](assets/new-line-indicator-comments.png)

1. クリック **Submit** をクリックして、レコードに更新を追加します。
1. （オプション）コメントを編集するには、コメントの右上隅にある&#x200B;**その他**&#x200B;メニュー ![](assets/more-menu.png) をクリックして、「**編集**」をクリックします。

   >[!IMPORTANT]
   >
   >コメントは送信後の 15 分間のみ編集できます。

1. コメント内の情報の編集、画像の追加や削除、タグ付きユーザーの削除を行います。コメントの左側に「編集済み」インジケーターが追加されます。

   >[!TIP]
   >
   >当年からのコメントでは、日付スタンプに年は表示されません。タイムスタンプにポインタを合わせると、年を含む完全な日付が表示されます。

1. （オプションおよび条件付き）既存のコメントを検索するには、の右上隅にある検索ボックスにキーワードを入力します **コメント** 領域。

   ![](assets/search-box-for-comments-area.png)

1. （任意）クリック **返信** または、でコメントの入力を開始します **返信を追加…** 既存のコメントに返信するには、上記の手順 4～8 に従います。 <!--(**************accurate??***********)-->

1. （条件付きおよびオプション）他のユーザーがコメントを追加している場合に、コメントを追加する際に [ コメント ] セクションの表示エリア外に表示されるコメントを追加するには、をクリックします **表示** 内 **新しいコメントバナー** これらのコメントを画面の下部に表示します。

   ![](assets/new-comments-banner-on-record.png)

   追加のコメントが画面の下部に表示されます。

1. （任意） **類似** 更新を気に入るか、読んだことを確認するアイコン。 アイコンは「いいね！」の数に応じて更新されます。
1. （条件付きおよびオプション）コメントに追加の人物を含めた場合、更新に含まれるユーザーのアバターをクリックして、コメントが共有されるユーザーのリストを表示します。
1. （任意） **詳細** アイコン ![](assets/more-menu.png) コメントの右上隅にある次のいずれかのオプションをクリックして、コメントから情報をコピーします。

   * **リンクをコピー**：コメントへのリンクをクリップボードにコピーします。
   * **本文をコピー**：コメントのテキストをクリップボードにコピーします。
   * **見積の返信**：コメントの内容を新しい返信にコピーします。 コピーした返信には画像は含まれません。

   詳しくは、[作業の更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md)を参照してください。
1. （任意） **詳細** アイコン ![](assets/more-menu.png) コメントの右上隅のをクリックし、 **削除** コメントを削除します。
1. （任意） **コメントを非表示** アイコン ![](assets/hide-comments-icon.png) をクリックして、右パネルを閉じます。

## 履歴セクションの概要

レコードに加えられた変更は、レコードの右側のパネルの「履歴」セクションで確認できます。

詳しくは、[「履歴」セクションの概要](/help/quicksilver/maestro/records/history-section-overview.md)を参照してください。
