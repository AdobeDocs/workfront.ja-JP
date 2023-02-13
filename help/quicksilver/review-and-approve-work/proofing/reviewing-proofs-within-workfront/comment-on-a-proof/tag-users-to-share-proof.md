---
product-area: documents;user-management;resource-management
navigation-topic: comment-on-a-proof
title: 配達確認を共有するようユーザーにタグを付けます
description: 校正ビューアで配達確認にコメントを付ける際に、他のユーザーにタグを付けて、コメントに電子メールで注意を引き、配達確認のワークフローに追加することができます。
author: Courtney
feature: Digital Content and Documents
exl-id: 4efbfdeb-3834-48dd-aa5b-515891bac519
source-git-commit: 49950895440fec8cebdf12ec81191c6e890383cf
workflow-type: tm+mt
source-wordcount: '708'
ht-degree: 0%

---

# 配達確認を共有するようユーザーにタグを付けます

校正ビューアで配達確認にコメントを付ける際に、他のユーザーにタグを付けて、コメントに電子メールで注意を引き、配達確認のワークフローに追加することができます。

配達確認に対するコメントでユーザーにタグ付けする場合、タグ付けできるユーザーは、個々のユーザー権限や組織のメンバーシップなど、様々な要因によって異なる場合があります。

* 配達確認の作成者、所有者または特定の権限が有効になっている場合は、配達確認ワークフローの外部でユーザーにタグ付けし、配達確認をユーザーと共有できます。
* 外部ユーザーとして配達確認に追加され、異なる配達確認アカウントを持つ別の環境のメンバーである場合、元の環境からのユーザーのみにタグ付けできます。 <!--For more information, see [Proofing collaboration limitations with people outside of your organization](../../../../review-and-approve-work/proofing/tips-tricks-and-troubleshooting/collaboration-with-members-outside-of-your-organization.md)-->

## アクセス要件 {#access-requirements}

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>現在のプラン：Pro 以上</p> <p>または</p> <p>レガシープラン：プレミアム</p> <p>様々なプランでのアクセスの検証について詳しくは、 <a href="/help/quicksilver/administration-and-setup/manage-workfront/configure-proofing/access-to-proofing-functionality.md" class="MCXref xref">Workfrontの校正機能へのアクセス</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>現在のプラン：作業または計画</p> <p>レガシープラン：任意（ユーザーの校正が有効になっている必要があります）</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">配達確認の役割</td> 
   <td>作成者、モデレーター</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">プルーフ権限プロファイル </td> 
   <td>スーパーバイザーまたは管理者</td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、役割、配達確認権限プロファイルを確認するには、WorkfrontまたはWorkfrontの配達確認管理者に問い合わせてください。

## 配達確認を共有するようユーザーにタグを付けます

配達確認権限プロファイルまたは配達確認ロールが「 [アクセス要件](#access-requirements) 上記の節では、デフォルトで、配達確認を共有するようユーザーにタグを付けることができます。 また、配達確認の所有者または作成者の役割に関係なく、配達確認の権限プロファイルまたは配達確認の役割に関係なく、ユーザーに配達確認を共有するようタグを付けることもできます。 配達確認の作成時に、配達確認の権限プロファイルまたは配達確認の役割の低いユーザーに対して、配達確認を共有するようにユーザーにタグ付けできます。 詳しくは、 [ワークフローの設定とレビュー担当者の追加](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md#configur) セクション [基本ワークフローを使用した詳細な配達確認の作成](../../../../review-and-approve-work/proofing/creating-proofs-within-workfront/configure-basic-proof-workflow.md) 記事。

>[!NOTE]
>
>E メールアドレスを使用して外部の共同作業者にタグを付けることができるのは、次のいずれかに該当する場合のみです。>
>* 組織のWorkfrontアカウントのユーザーが、以前に共同作業者の E メールアドレスを配達確認に追加しています。
>* 共同作業者は、この電子メールアドレスを使用して、組織のWorkfrontアカウントで以前に配達確認を登録しています。
>


誰かにタグを付け、コメントで配達確認を共有するには：

1. 配達確認にコメントする際は、アットマーク (@) の後にユーザーの名前または電子メールアドレスを入力します。 入力を開始すると、使用可能な名前がドロップダウンリストに表示されます。
1. ドロップダウンリストに表示されたら、その人物の名前を選択します。

   >[!TIP]
   >
   >他のユーザーを選択せずにドロップダウンリストを閉じる場合は、 **Esc** キーを押すか、リストの外側の任意の場所をクリックします。

1. コメントにタグを付ける他のユーザーに対して、手順 1～2 を繰り返します。
1. コメントを終了し、「 **投稿**.
1. （条件付き）配達確認にまだ追加されていない人にタグを付けた場合は、 **配達確認の役割** および **E メールアラート** 表示されるボックスに一覧表示される各ユーザーの設定で、 **担当者の追加とコメントの投稿**.

   ![](assets/add-people-to-proof-350x220.png)

   配達確認の役割について詳しくは、を参照してください。 配達確認 E メールアラートについて詳しくは、この記事の「 」の節を参照してください。 [Workfront Proof での電子メール通知設定](../../../../workfront-proof/wp-emailsntfctns/email-alerts/config-email-notification-settings-wp.md).

   配達確認に自動ワークフローが含まれている場合、タグ付けしたユーザーが現在のステージに追加されます。 詳しくは、 [自動ワークフローの概要](../../../../review-and-approve-work/proofing/proofing-overview/automated-workflow.md).

   タグ付けするユーザーは、使用している配達確認 E メールのアラート設定に関係なく、配達確認のコメントに関する通知 E メールを受け取ります。

   * ユーザーが日別の概要または時間別の概要 E メールを受け取った場合、Workfrontは通知を個別に送信し、配達確認のコメントに関する情報を概要 E メールに含めます。
   * ユーザーがすべてのアクティビティに関するアラートを受け取った場合、またはユーザーのコメントに対する返信に関するアラートを受け取った場合は、それらのコメントおよび返信に関する通知が通知に置き換えられます。

配達確認にユーザーを追加するその他の方法について詳しくは、 [Adobe Workfront内での配達確認の共有](../../../../review-and-approve-work/proofing/managing-proofs-within-workfront/share-a-proof-in-workfront.md).
