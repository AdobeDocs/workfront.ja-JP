---
product-area: projects
navigation-topic: update-work-items-and-view-updates
title: 更新情報に返信
description: 作業オブジェクトの更新に対して、誰かが追加または返信すると、その返信がそのオブジェクトの [ 更新 ] タブの通信スレッドに表示されます。 オブジェクトに対するビューアクセス権を持っている場合は、更新に返信を追加したり、「いいね！」をクリックしたりできます。
author: Lisa and Alina
feature: Get Started with Workfront
exl-id: a8271f3c-7a08-4eb3-aaff-deb250f5af73
source-git-commit: 923c9e25fbd73c9d6a6a20436333c6e7969e9538
workflow-type: tm+mt
source-wordcount: '830'
ht-degree: 1%

---

# 更新情報に返信

作業オブジェクトの更新に対して、誰かが追加または返信すると、その返信がそのオブジェクトの [ 更新 ] タブの通信スレッドに表示されます。 オブジェクトに対するビューアクセス権を持っている場合は、更新に返信を追加したり、「いいね！」をクリックしたりできます。

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
   <td> <p>問題およびドキュメントの要求以上その他のすべてのオブジェクトを確認するか、それ以上の値を設定します</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>アクセスレベル設定*</strong></td> 
   <td> <p>問題およびドキュメントの要求者以上他のすべてのオブジェクトのレビュー担当者以上</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>オブジェクト権限</strong></td> 
   <td> <p>オブジェクトへのアクセスの表示</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 更新または返信に返信

1. 返信を追加するオブジェクトに移動します。
1. の **更新** タブで、返信先の更新または返信を探します。

   更新で画像を表示するには：

   * 次をクリック： **プレビュー** アイコン ![](assets/previewimageicon-31x31.png) 画像のサムネールで、フルサイズの画像を新しいブラウザータブで開きます。
   * 次をクリック： **ダウンロード** アイコン ![](assets/downloadimageicon.png) を画像のサムネールにドラッグして、画像をダウンロードします。

   会話に積極的に関わっているユーザーを見る以外に、各返信にタグ付けされたユーザーをその更新スレッドの上部で確認することができます。 これらのユーザーは、オブジェクトを購読しているユーザーと共に、オブジェクトに対して更新または返信がおこなわれるたびに通知を受け取ります。 さらに多くのユーザーにタグを付けて、返信に含めることもできます。  さらに多くのユーザーにタグを付けるには、 [更新時の他のユーザーへのタグ付け](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

   ![](assets/tagging-transparency-350x192.png)

1. クリック **返信** 更新時に、表示されるボックスに返信を入力します。
1. （オプション）返信に以前の更新のテキストを含めるには、 **詳細** 見積もりを行う更新または返信の横のメニューから、 **見積もりの返信**. 前回の更新のテキストが入力領域に灰色の線で示されます。
1. （オプション）書式と絵文字を使用し、リンクと画像を含めます (「 [作業項目に更新を追加する](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md#add) 記事内 [作業を更新](../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. クリック **返信** 返信を保存します。

   または

   クリック **完了** タスクまたはタスクのステータスが「完了」または「クローズ」の場合。

## 電子メール通知で更新に返信

電子メール通知の設定によっては、アクセス権のある特定のオブジェクトに対して更新が行われた際に電子メール通知を受け取る場合があります。

>[!NOTE]
>
>クラスター 6 上の環境では、電子メールによる更新への返信を利用できません。

以下は、タスクの「更新」タブでの更新の結果としてトリガーされる電子メール通知の例です。

![email.png](assets/email-350x202.png)

E メールから、Workfrontのオブジェクトの通信スレッドに直接返信を簡単に追加できます。 次のオブジェクトに対するコメントから生成された E メールに対して、Workfrontにログインせずに返信を追加することもできます。

* プロジェクト
* タスク
* 問題
* ドキュメント
* テンプレートとテンプレートタスク
* ポートフォリオ
* プログラム
* 反復
* タイムシート

### 電子メール通知から更新に返信

電子メール通知を受け取ったら、関連するWorkfrontオブジェクトをすばやく開き、応答を通信スレッドに直接追加できます。

1. クリック **コメント** 電子メール通知を受け取ります。

   オブジェクトの詳細ページがWorkfrontで開きます。

1. 返信を追加する更新に移動します。

   会話に積極的に関わっているユーザーを見る以外に、各返信でタグ付けされたユーザーをその更新スレッドの上部で確認できます。 これらのユーザーは、オブジェクトを購読しているユーザーと共に、オブジェクトに対して更新または返信がおこなわれるたびに通知を受け取ります。 さらに多くのユーザーにタグを付けるには、 [更新時の他のユーザーへのタグ付け](../../workfront-basics/updating-work-items-and-viewing-updates/tag-others-on-updates.md).

1. クリック **返信、** 返信を入力し、「 **返信**.

### Workfront以外のオブジェクトに更新を追加する

Workfrontの電子メール通知を受け取った場合、Workfrontにログインすることなく、通信スレッドに更新をすばやく追加できます。

Workfront E メールに更新を追加するには：

1. 電子メールアプリケーションから、返信先のWorkfront電子メールを開き、返信電子メールウィンドウを開きます。
1. 更新を入力します。\
   添付ファイルは許可されておらず、メール内の更新に適用されたリッチテキスト書式は、「更新」タブで表示された場合、更新に表示されません。
1. クリック **送信**.

   更新がオブジェクトの通信スレッドに追加されます。
