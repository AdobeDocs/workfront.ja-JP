---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 電子メール通知に返信
description: プロジェクト、タスク、イシューなどのオブジェクトに対するコメントから生成されたWorkfrontの電子メール通知に応答して、Adobe Workfrontアプリケーションでおこなわれた元のコメントに返信を追加できます。
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: fea88410-8f37-49d0-9f5d-9fbac4ab5de6
source-git-commit: 413e5ff710b4c77b7ea2d870b34bb0627a4fcd86
workflow-type: tm+mt
source-wordcount: '595'
ht-degree: 1%

---

# 電子メール通知に返信

電子メール通知の設定によっては、アクセス権のある特定のオブジェクトに対して更新が行われた際に電子メール通知を受け取る場合があります。

電子メール通知から更新に返信する方法は次のとおりです。

元のコメントに返信します。

* E メール内の「コメント」ボタンを使用して、Workfrontに戻り、「更新」領域の更新に返信します。
* 受信した電子メールに返信します。 返信メールがWorkfrontとして追加されました



>[!NOTE]
>
>クラスター 6 上の環境では、電子メールによる更新への返信を利用できません。

以下のオブジェクトに対するコメントから生成されたWorkfront E メールに応答できます。

* プロジェクト
* タスク
* 問題
* ドキュメント
* テンプレートとテンプレートタスク
* ポートフォリオ
* プログラム
* 反復
* タイムシート

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront plan*</strong></td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront license*</strong></td> 
   <td> <p>問題およびドキュメントに対する要求以上、その他のすべてのオブジェクトに対する確認以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>問題およびドキュメントに対して要求者以上、その他すべてのオブジェクトに対してレビュー担当者以上</p> <p><b>メモ</b>

まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクトの権限</strong></td> 
   <td> <p>オブジェクトへのアクセスの表示</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## 電子メール通知から更新に返信

電子メール通知を受け取ったら、電子メール通知から関連するWorkfrontオブジェクトをすばやく開き、応答を通信スレッドに直接追加できます。

1. Workfrontの更新で生成された電子メール通知を開きます。

   ![email.png](assets/email-350x202.png)
1. クリック **コメント** 電子メール通知から。

   オブジェクトの詳細ページがWorkfrontで開きます。

1. 返信を追加する更新に移動します。

   会話に積極的に関わっているユーザーを見る以外に、各返信でタグ付けされたユーザーをその更新スレッドの上部で確認できます。 これらのユーザーは、オブジェクトを購読しているユーザーと共に、オブジェクトに対して更新または返信がおこなわれるたびに通知を受け取ります。 さらに多くのユーザーにタグを付けるには、 [更新時の他のユーザーへのタグ付け](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

1. クリック **返信、** 返信を入力し、「 **返信**.

   応答は、新しいコメントとしてコメントスレッドに追加されます。

## 電子メール通知に返信してオブジェクトに更新を追加

Workfrontの電子メール通知を受け取った場合、Workfrontにログインすることなく、通信スレッドに更新をすばやく追加できます。

>[!IMPORTANT]
>
>* 電子メール通知に返信する前に、更新をトリガーしたオブジェクトを表示する権限が必要です。
>
>* 送信エラーを避けるには、Outlook ユーザーは返信を入力する前に既存の電子メールコンテンツを削除する必要があります。

Workfront E メールに更新を追加するには：

1. 電子メールアプリケーションから、返信先のWorkfront電子メールを開き、元の電子メールから返信電子メールウィンドウを開きます。

   >[!NOTE]
   >
   >    他のユーザーから転送された電子メール通知には返信できません。


1. メールの返信に更新内容を入力します。

   添付ファイルは許可されておらず、メール内の更新に適用されたリッチテキスト書式は、「更新」タブで表示された場合、更新に表示されません。
1. クリック **送信**.

   更新が、オブジェクトの通信スレッドへの応答として追加されます。
