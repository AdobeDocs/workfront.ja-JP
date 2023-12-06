---
title: レコードコメントの管理
description: レコードの [ コメント ] 領域で、更新内容を追加し、質問や返信をすることで、Adobeの Maestro レコードに関する共同作業を行うことができます。
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
source-git-commit: 3ffb6fdebb54682abc737e55186850458a133f7c
workflow-type: tm+mt
source-wordcount: '957'
ht-degree: 0%

---


<!--update the metadata with real information when making this available in TOC and in the left nav-->

# レコードコメントの管理

レコードの [ コメント ] 領域で、更新内容を追加し、質問や返信をすることで、Adobeの Maestro レコードを共同で作業することができます。

## レコードにコメントする際の考慮事項

* レコードの [ コメント ] セクションで、Maestro のオペレーショナルレコードとタクソノミにコメントと返信を追加できます。

* リンクされたレコードに追加されたコメントは、リンク元のレコードには表示されません。 例えば、Campaign レコードにリンクされているプロジェクトにコメントする場合、コメントは Maestro のプロジェクトレコードにのみ表示され、リンク元のキャンペーンレコードには表示されません。

* 他のアプリケーションでリンクされたオブジェクトに追加されたコメントは、Maestro には表示されません。
Maestro でリンクされたオブジェクトに追加されたコメントは、他のアプリケーションには表示されません。\
  例えば、Workfrontのプロジェクトに追加されたコメントは、Maestro のキャンペーンにリンクされているのと同じプロジェクトには表示されません。

* ユーザーにタグを付けて、更新に注意を向けることができます。 タグ付きユーザーは、アプリ内通知や更新に関する電子メールを受け取りません。 Maestro コメント内のチームにタグを付けることはできません。

  >[!TIP]
  >
  >* コメントの所有者は、更新で自動的にタグ付けされません。
  >
  >* 返信時に、更新からタグ付きユーザーを削除することはできません。

* Maestro の次の領域からレコードに更新を追加できます。

   * 「詳細」ページから。

  <!--* From the table view.-->

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto">
 <col>
 <tbody>
<td>
   <p> Adobe産物</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront協定</p></td>
   <td>
<p>組織は、Maestro クローズ済みベータプログラムのAdobeに登録する必要があります。 この新しいオファーについては、アカウント担当者にお問い合わせください。 </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfrontプラン</p></td>
   <td>
<p>任意</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfrontライセンス</p></td>
   <td>
   <p>任意</p> 
  </td>
  </tr>

<tr>
   <td role="rowheader">アクセスレベル</td>
   <td> <p>任意</p>  
</td>
  </tr>
<tr>
   <td role="rowheader">レイアウトテンプレート</td>
   <td> <p>システム管理者は、レイアウトテンプレートに Maestro 領域を追加する必要があります。 詳しくは、 <a href="../access/grant-access.md">AdobeMaestro へのアクセスを許可</a>. </p>  
</td>
  </tr>
 </tbody>
</table>

<!--
After permissions - replace the table with: **************CHECK ON THE VIEW PERMISSIONS TO THE WORKSPACE; RIGHT NOW, WE SAY THAT VIEW USERS CAN COMMENT BUT THE PAGE BLOWS OUT WHEN I TRY - ASKED PM TO CONFIRM*****************

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Adobe product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the Adobe Maestro closed beta program. Contact your account representative to inquire about this new offering. </p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront plan</p></td>
   <td>
<p>Any</p>
   </td>
  </tr>
  <tr>
   <td role="rowheader"><p>Adobe Workfront license</p></td>
   <td>
   <p>Any</p> 
  </td>
  </tr>
  
  <tr>
   <td role="rowheader"><p>Access level</p></td>
   <td> <p>Any</p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Maestro area in your layout template. For information, see <a href="../access/grant-access.md">Grant access to Adobe Maestro</a>. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>
 </tbody>
</table>

-->


<!--Maybe enable this at GA - but Maestro is not supposed to have Access controls in the Workfront Access Level: 
>[!NOTE]
>
>If you don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can change your access level, see [Create or modify custom access levels](../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md). -->

<!-- Notes to add for the table: for the "Workfront plans" row: the above is only for closed beta; when going to GA - activate the following plans:    
<p>Current plan: Prime and Ultimate</p>
<p>Legacy plan: Enterprise</p>-->

<!-- Notes for the table: for the "Workfront access" row: <p>For more information, see <a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Adobe Workfront licenses overview</a>.</p>-->

### レコードに対するコメントの管理

1. 次をクリック： **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](assets/dots-main-menu.png) Adobe Workfrontの右上隅にある、または（使用可能な場合）、 **[!UICONTROL メインメニュー]** アイコン ![メインメニュー](assets/lines-main-menu.png) 左上隅で、「 **[!UICONTROL マエストロ]**.

   最後にアクセスしたワークスペースは、デフォルトで開きます。
1. 次の場所からテーブルビューを選択します。 **表示** ドロップダウンメニュー。
1. テーブルビューでレコードの名前をクリックします。

   レコードの **詳細** ページが開きます。

1. でコメントの入力を開始 **新しいコメント** ボックス。

   ![](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >コメントを入力して送信する前に「コメント」セクションから移動すると、ログオフしてログオンし直した後でも、ページ上のコメントはドラフトモードのままになります。 コメントに追加された画像も下書きに保存されます。 ドラフトは 7 日間保存され、その後は破棄され、復元できません。 下書きのコメントは、ユーザーが入力した場合にのみ表示されます。

1. （オプション）変更の取り消しまたはやり直しをおこなうには、次のショートカットキーを使用します。
   * Ctrl + Z( Macの場合は⌘+z)：変更を元に戻します。
   * Ctrl + Y( Macの場合は⌘+y)：変更をやり直します。
1. （オプション） **@** 更新時に、誰かにタグを付けるユーザーの名前が続きます。
1. （オプション）リッチテキストツールバーのオプションを使用して、テキストの書式設定、絵文字、リンク、画像を更新に追加し、コンテンツを拡張できます。 詳しくは、この記事の「Workfrontの更新でのリッチテキストの使用」の節を参照してください [作業を更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).

   >[!TIP]
   >
   >別のユーザーが、更新しようとしている同じ項目にコメントを送信した場合、赤い線に「新規」インジケータが表示され、新しいコメントが通知されます。
   >
   >インジケーターは、コメントがアイテムに送信された後にのみ表示され、コメントがまだ構成されている場合は表示されません。
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
   * **本文テキストをコピー** t：コメントのテキストをクリップボードにコピーします。
   * **見積もりの返信**：コメントの内容を新しい返信にコピーします。 コピーされた返信に画像は含まれません。

   詳しくは、 [作業を更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. （オプション） **その他** アイコン ![](assets/more-menu.png) コメントの右上隅で、 **削除** をクリックしてコメントを削除します。

