---
title: レコードのコメントの管理
description: レコードの右側のパネルにコメントや返信を追加することで、Adobe Workfront Planning レコードに関する共同作業を行うことができます。また、レコードに加えられた他の変更やシステムにより記録された他の変更を、このエリアに表示することもできます。
feature: Workfront Planning
role: User
author: Alina
recommendations: noDisplay, noCatalog
exl-id: 215883a4-e882-438e-9c21-954c0b1d741b
source-git-commit: cf42511263ec1cffd90d1e4bdcd43521b7fe6a30
workflow-type: tm+mt
source-wordcount: '1269'
ht-degree: 88%

---

# レコードのコメントの管理

{{planning-important-intro}}

<!--update the system updates articles when we release to open beta - check the long commenting stream article list and see articles that document where in the system we have system updates; "Workfront Planning records" should be there-->

レコードの右側のパネルにコメントや返信を追加することで、Adobe Workfront Planning レコードに関する共同作業を行うことができます。また、レコードに加えられた他の変更やシステムにより記録された他の変更を、このエリアに表示することもできます。

レコードの右側のパネルには、次のセクションが表示されます。

* **コメント**：ユーザーがレコードに追加したコメントおよび返信を表示します。
* **履歴**：ユーザーがレコードフィールドに対して行った、システムで記録された変更を表示します。詳しくは、[「履歴」セクションの概要](/help/quicksilver/planning/records/history-section-overview.md)を参照してください。

## アクセス要件

+++ 展開すると、Workfront Planning のアクセス要件が表示されます。

Workfront Planning にアクセスするには、次のものが必要です：

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
   <ul><li><p> Adobe Workfront</p></li> 
   <li><p> Adobe Workfrontの計画<p></li></ul></td> 
  </tr>   
<tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td> 
<p>次のいずれかのWorkfront プラン：</p> 
<ul><li>選択</li> 
<li>Prime</li> 
<li>Ultimate</li></ul> 
<p>Workfront Planning は、従来のWorkfront プランでは使用できません</p> 
   </td> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront計画*</p></td> 
   <td> 
<p>任意 </p> 
<p>各Workfront Planning プランに含まれる内容の詳細については、<a href="https://business.adobe.com/products/workfront/pricing.html">Adobe Workfrontの価格とパッケージ </a> を参照してください。 </p> 
   </td> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront platform</p></td> 
   <td> 
<p>組織のWorkfront インスタンスは、Workfront Planning のすべての機能にアクセスできるように、Adobe Unified Experience にオンボーディングされる必要があります。</p> 
<p>詳しくは、<a href="/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md">Workfront の Adobe Unified Experience</a> を参照してください。 </p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Adobe Workfront プラン*</p></td> 
   <td><p> 共同作成者、ライト、または標準</p>
   <p>Workfront Planning は、従来のWorkfront ライセンスでは使用できません</p> 
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>アクセスレベルの設定</p></td> 
   <td> <p>Adobe Workfront Planning に対するアクセスレベルのコントロールはありません。</p>   
</td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>オブジェクト権限</p></td> 
   <td>   <p>ワークスペースに対する表示またはそれ以上の権限</a> </p>  
   <p>システム管理者は、作成しなかったワークスペースも含め、すべてのワークスペースに対する権限を持っています。</p> </td> 
  </tr> 
<tr> 
   <td role="rowheader"><p>レイアウトテンプレート</p></td> 
   <td> <p>Workfront の管理者を含むすべてのユーザーには、メインメニューの Planning エリアを含むレイアウトテンプレートを割り当てる必要があります。 </p> </td> 
  </tr> 
</tbody> 
</table>

*Workfront のアクセス要件について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--OLD: 

<table style="table-layout:auto">
 <col>
 </col>
 <col>
 </col>
 <tbody>
    <tr>
<tr>
<td>
   <p> Product</p> </td>
   <td>
   <p> Adobe Workfront</p> </td>
  </tr>  
 <td role="rowheader"><p>Adobe Workfront agreement</p></td>
   <td>
<p>Your organization must be enrolled in the early access stage for Workfront Planning </p>
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
   <td role="rowheader"><p>Access level configuration</p></td>
   <td> <p>There are no access level controls in Workfront Planning. </p>  
</td>
  </tr>
<tr>
   <td role="rowheader"><p>Permissions</p></td>
   <td> <p>View or higher permissions to a workspace</a> </p>  
   <p>System Administrators have permissions to all workspaces, including the ones they did not create</p>
</td>
  </tr>

<tr>
   <td role="rowheader"><p>Layout template</p></td>
   <td> <p>Your Workfront or group administrator must add the Planning area in your layout template. For information, see <a href="/help/quicksilver/planning/access/access-overview.md">Access overview</a>. </p>  
</td>
  </tr>
 </tbody>
</table>
-->

## レコードへのコメントに関する考慮事項

* レコードの「コメント」セクションで、Workfront Planning のレコードにコメントや返信を追加できます。

* リンク先のレコードに追加されたコメントは、リンク元のレコードには表示されません。例えば、キャンペーンレコードにリンクされている Workfront Planning の製品レコードにコメントを付けると、そのコメントは Workfront Planning の製品レコードにのみ表示され、リンク元のキャンペーンレコードには表示されません。

* レコードと別のアプリケーションのオブジェクトとの接続の結果として作成された Workfront Planning レコードにコメントを追加できます。

  例えば、Workfront プロジェクトを Workfront Planning レコードと接続した後で、プロジェクトの Workfront Planning レコードにコメントを付けることができます。詳しくは、[レコードの接続](/help/quicksilver/planning/records/connect-records.md)を参照してください。

* 他のアプリケーションでリンク先のオブジェクトに追加されたコメントは Workfront Planning には表示されず、Workfront Planning でリンク先のオブジェクトに追加されたコメントは他のアプリケーションには表示されません。

  例えば、Workfront のプロジェクトに追加されたコメントは、Workfront Planning のキャンペーンにリンクされている同じプロジェクトには表示されず、プロジェクトの Workfront Planning レコードに追加されたコメントは Workfront には表示されません。

* ユーザーにタグ付けして、更新に注意を向けさせることができます。タグ付きユーザーには、更新に関するアプリ内通知およびメールが届きません。<!--this might change??-->

<!--replace the bullet above with this: * You can tag users to bring their attention to an update. Tagged users receive an in-app notification or an email notification about your update. 
   The following scenario exists:   

   * Adobe Unified Experience users receive both an in-app notification and an email notification. 
   * Users who are not in the Adobe Unified Experience receive only an email notification. 

      For information, see [Adobe Workfront Planning notifications: article index](/help/quicksilver/planning/notifications/notifications-information.md)
   
      To determine whether your company is using the Adobe Unified Experience, see [Adobe Unified Experience for Workfront](/help/quicksilver/workfront-basics/navigate-workfront/workfront-navigation/adobe-unified-experience.md).
      -->

* Workfront Planning の次のエリアから、レコードに更新を追加したり、変更履歴を確認したりできます。

   * レコードの詳細ページから。
   * ビューの「レコードの詳細」ボックスに移動します。

### レコードに対するコメントの管理

{{step1-to-planning}}

1. ワークスペースのカードをクリックします。

   ワークスペースが開き、カードにレコードタイプが表示されます。

1. レコードタイプのカードをクリックします。
レコードタイプのページが開き、そのタイプのすべてのレコードが表示されます。

1. 「**表示**」ドロップダウンメニューからテーブルビューを選択します。
1. テーブルビューでレコードの名前をクリックします。

   レコードの&#x200B;**詳細**&#x200B;ページが開きます。デフォルトではコメントエリアが右側のパネルに開きます。

1. （条件付き）デフォルトで右側のパネルが開かない場合は、右上隅の&#x200B;**コメントを表示** ![](assets/show-comments-icon.png) アイコンをクリックして、「コメント」セクションを開きます。

1. **新しいコメント**&#x200B;ボックスにコメントを入力します。

   ![](assets/empty-comment-box-on-record.png)

   >[!TIP]
   >
   >コメント入力を完了して送信する前に「コメント」セクションから移動すると、ログオフしてログオンし直した後でも、ページ上のコメントはドラフトモードのままです。コメントに追加された画像も下書きに保存されます。ドラフトは 7 日間保存され、その後は破棄され、復元できません。下書きのコメントは、入力したユーザーのみに表示されます。

1. （オプション）変更の取り消しまたはやり直しを行うには、以下のショートカットキーを使用します。
   * Ctrl + Z（Mac の場合は ⌘+z）で、変更を元に戻します
   * Ctrl + Y（Mac の場合は ⌘+y）で、変更をやり直します
1. （オプション）**@** をユーザーの名前の後に追加して、更新時に誰かにタグを付けます。

   <!--Adobe Unified Experience users can receive an in-app and an email notification when they are tagged. All other users receive an email when they are tagged. For more information, see the section [Considerations about commenting on a record](#considerations-about-commenting-on-a-record) in this article. -->

1. （オプション）リッチテキストツールバーのオプションを使用すると、テキストの書式設定、絵文字やリンク、画像の更新への追加を行い、コンテンツを拡充できます。詳しくは、[更新作業](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md)の記事の「Workfront の更新でのリッチテキストの使用」の節を参照してください。

   >[!TIP]
   >
   >別のユーザーが、更新しようとしている同じ項目にコメントを送信すると、赤い線に「新規」インジケーターが表示され、新しいコメントが通知されます。
   >
   >インジケーターは、コメントが項目に送信された後にのみ表示され、コメントがまだ構成されている場合は表示されません。
   >
   >![](assets/new-line-indicator-comments.png)

1. 「**送信**」をクリックして、レコードに更新を追加します。
1. （オプション）コメントを編集するには、コメントの右上隅にある&#x200B;**その他**&#x200B;メニュー![](assets/more-menu.png)をクリックして、「**編集**」をクリックします。

   >[!IMPORTANT]
   >
   >コメントは送信後の 15 分間のみ編集できます。

1. コメント内の情報の編集、画像の追加や削除、タグ付きユーザーの削除を行います。コメントの左側に「編集済み」のインジケーターが追加されます。

   >[!TIP]
   >
   >当年からのコメントでは、日付スタンプに年は表示されません。タイムスタンプにポインタを合わせると、年を含む完全な日付が表示されます。

1. （オプションおよび条件付き）既存のコメントを検索するには、**コメント**&#x200B;エリアの右上隅にある検索ボックスでキーワードの入力を開始します。

   ![](assets/search-box-for-comments-area.png)

1. （オプション）「**返信**」をクリックするか、**返信を追加...** エリアでコメントの入力を開始して既存のコメントに返信し、上記の手順 4～8 に従います。<!--(**************accurate??***********)-->

1. （条件付きおよびオプション）「コメント」セクションで表示エリアの外側に表示されるコメントを他のユーザーが追加した場合、画面の下部にある「**新しいコメントバナー**」内の「**表示**」をクリックして、これらのコメントを表示します。

   ![](assets/new-comments-banner-on-record.png)

   追加のコメントが画面の下部に表示されます。

1. （オプション）**いいね！**&#x200B;アイコンをクリックして、更新に「いいね！」したり、自分が読んだことを確認したりします。アイコンは「いいね！」の数に応じて更新されます。
1. （条件付きおよびオプション）コメントに追加のユーザーを含める場合は、更新に含まれるメンバーの数をクリックして、入力したコメントが共有されているユーザーのリストを表示します。
1. （オプション）コメントの右上隅で&#x200B;**その他**&#x200B;アイコン![](assets/more-menu.png)をクリックし、次のいずれかのオプションをクリックして、コメントから情報をコピーします。

   * **リンクのコピー**：コメントへのリンクをクリップボードにコピーします。
   * **本文をコピー**：コメントのテキストをクリップボードにコピーします。
   * **引用返信**：コメントの内容を新しい返信にコピーします。コピーされた返信に画像は含まれません。

   詳しくは、[作業の更新](/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md)を参照してください。
1. （オプション）コメントの右上隅にある&#x200B;**その他**&#x200B;アイコン![](assets/more-menu.png)をクリックし、「**削除**」をクリックしてコメントを削除します。
1. （オプション）**コメントの非表示**&#x200B;アイコン![](assets/hide-comments-icon.png)をクリックして、右側のパネルを閉じます。

## 履歴セクションの概要

レコードに加えられた変更は、レコードの右パネルの「履歴」セクションで確認できます。

詳しくは、[「履歴」セクションの概要](/help/quicksilver/planning/records/history-section-overview.md)を参照してください。
