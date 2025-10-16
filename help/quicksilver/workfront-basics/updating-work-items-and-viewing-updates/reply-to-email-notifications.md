---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: メール通知への返信
description: プロジェクト、タスク、イシューなどのオブジェクトに対するコメントから生成された Workfront のメール通知に応答して、Adobe Workfront アプリケーションで行われた元のコメントに返信を追加できます。
author: Nolan and Alina
feature: Get Started with Workfront
exl-id: fea88410-8f37-49d0-9f5d-9fbac4ab5de6
source-git-commit: 4ef71db5d93e314b746e8acdbf90fd041c6e71ae
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 89%

---

# メール通知への返信

<!-- Audited: April 2024-->

メール通知の設定によっては、アクセス権のある特定のオブジェクトに対して更新が行われた際にメール通知を受信する場合があります。

メール通知から更新に返信する方法は次のとおりです。

* メール内の「コメント」ボタンを使用して、Workfront に戻り、アップデートエリアの更新に返信します。
* 受信したメールに返信します。返信メールは、元のコメントに対する Workfront の返信として追加されます。

<!--
>[!NOTE]
>
>Replying to updates by email is not available for environments on Cluster 6.
-->

以下のオブジェクトに対するコメントから生成された Workfront メールに応答できます。

* プロジェクト
* タスク
* イシュー
* ドキュメント
* テンプレートとテンプレートタスク
* ポートフォリオ
* プログラム
* イテレーション
* タイムシート

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront パッケージ</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront プラン</strong></td> 
   <td> <p>イシューとドキュメントの場合：</p>

<ul><li><p>投稿者以上</p></li>
   <li><p>リクエスト以上</p></li></ul>

<p>その他すべてのオブジェクトの場合：</p>
   <ul><li><p>ライト以上</p></li>
   <li><p>レビュー以上</p></li></ul>

</td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定</strong></td> 
   <td> <p>返信を投稿するオブジェクトへの表示以上のアクセス</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>返信を投稿するオブジェクトに対する以上の権限を表示します</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

<!--Old:
<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan</strong></td> 
   <td> <p>Any</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>New: Contributor or higher for issues and documents; Light or higher for all other objects</p>
   <p>Current: Request or higher for issues and documents; Review or higher for all other objects</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Access level configuration</strong></td> 
   <td> <p>View or higher access to the objects where you want to post the reply</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Object permission</strong></td> 
   <td> <p>View or higher permissions to the objects where you want to post the reply</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## メール通知から更新に返信

メール通知を受け取ったら、メール通知から関連する Workfront オブジェクトをすばやく開き、応答を通信スレッドに直接追加できます。

1. Workfront の更新で生成されたメール通知を開きます。

   ![email.png](assets/email-350x202.png)
1. メール通知から「**コメント**」をクリックします。

   オブジェクトの詳細ページが Workfront で開きます。

1. 返信を追加する更新に移動します。

   会話に積極的に関わっているユーザーを見る以外に、各返信でタグ付けされたユーザーをその更新スレッドの上部で確認できます。これらのユーザーは、オブジェクトに登録しているユーザーとともに、オブジェクトに対して更新または返信が行われるたびに通知を受信します。さらに多くのユーザーをタグ付けするには、[更新時に他のユーザーにタグ付け](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md)を参照してください。

1. 「**返信**」をクリックして返信を入力し、「**返信**」をクリックします。

   応答は、新しいコメントとしてコメントスレッドに追加されます。

## メール通知に返信してオブジェクトに更新を追加する

Workfront のメール通知を受け取った場合、Workfront にログインすることなく、通信スレッドに更新をすばやく追加できます。

>[!IMPORTANT]
>
>* メール通知に返信するには、少なくとも更新をトリガーしたオブジェクトを表示する権限が必要です。
>
>* 送信エラーを避けるには、Outlook ユーザーは返信を入力する前に既存のメールコンテンツを削除する必要があります。

Workfront メールに更新を追加するには、以下の手順を実行します。

1. メールアプリケーションから、返信先の Workfront メールを開き、元のメールから返信メールウィンドウを開きます。

   >[!NOTE]
   >
   >    他のユーザーから転送されたメール通知には返信できません。


1. メールの返信に更新内容を入力します。

   添付ファイルは許可されておらず、メール内の更新に適用されたリッチテキスト書式は、「更新」タブで表示された場合、更新に表示されません。
1. 「**送信**」をクリックします。

   更新が、オブジェクトの通信スレッドへの応答として追加されます。
