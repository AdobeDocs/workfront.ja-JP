---
product-area: documents
navigation-topic: approvals
title: レガシードキュメントの承認をリクエスト
description: Adobe Workfront のドキュメントに対して、管理者または他のユーザーの承認をリクエストできます。 Workfront 管理者がこの機能を有効にしている場合は、「システムセキュリティの環境設定の指定」の説明にあるように、Workfront アカウントを持たないユーザーからドキュメントの承認をリクエストすることもできます。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: f54a221b-4bf0-414e-b2f3-ace861d85496
TQID: https://experienceleague.adobe.com/NQgXFcbc-4DiObeNE2nRgaW9iKeCKRD5v7J1PRfHkHU
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
feature_v2:
  - id: a0dacc9f-0e23-495b-8e9f-a77c2e60b40c
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
subfeature_v2:
  - id: b04e3dc0-3a59-45b1-aa02-b0b6d5f87eff
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
topic_v2:
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
source-git-commit: 55a9d9feae8cc1128e3427a8874414ba734dd467
workflow-type: tm+mt
source-wordcount: 530
ht-degree: 95%

---

# レガシードキュメントの承認をリクエスト

Adobe Workfront のドキュメントに対して、管理者または他のユーザーの承認をリクエストできます。 Workfront 管理者がこの機能を有効にしている場合は、[システムセキュリティの環境設定の指定](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)の説明にあるように、Workfront アカウントを持たないユーザーからドキュメントの承認をリクエストすることもできます。

>[!NOTE]
>
>この記事の情報は、レガシードキュメントの承認に関するものです。<br>
>新しい統合レビューと承認について詳しくは、[統合レビューと承認の概要](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/document-approvals-overview.md)を参照してください。


## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。


<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン</td> 
   <td>
   <p>貢献度以上</p>
   <p>レビュー以上</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>プロジェクト、タスク、タスク、タスク、テンプレート、ポートフォリオ、プログラム、レポート、ダッシュボード、カレンダー、ドキュメントへの表示アクセス権、またはより高いレベルのアクセス権</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>リクエストのアクセスまたは承認に関連付けられたオブジェクトへのアクセス管理 </p></td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ドキュメントの承認をリクエスト

1. ドキュメントを含むプロジェクト、タスクまたはイシューに移動し、「**ドキュメント**」を選択します。
1. 必要なドキュメントを見つけます。

1. 概要で「**承認**」セクションまで下にスクロールし、「**承認者を追加**」テキストボックスに入力します。 Workfront ユーザーを名前で追加することも、外部ユーザーをメールで追加することもできます。

1. [システムセキュリティの環境設定の指定](../../administration-and-setup/manage-workfront/security/configure-security-preferences.md)で説明されているように、Adobe Workfront 管理者が Workfront を使用しないユーザーと共同作業する機能を有効にしている場合は、そのユーザーのメールアドレスを入力してそのユーザーを含めることができます。

   チームやグループから承認をリクエストすることはできません。

1. 前の手順を繰り返して、他の承認者を追加します。

## 新しいバージョンに対する承認を再送信

新しいバージョンをアップロードしても、ドキュメントの承認決定は自動的にはリセットされません。 例えば、ドキュメントが加えた変更と併せて承認された場合、指定された変更を含む新しいバージョンをアップロードした場合でも、決定には決定として「変更」と表示されます。 手動で承認を再送信した場合は、新しいバージョンに対する決定をクリアできます。

1. ドキュメントを含むプロジェクト、タスクまたはイシューに移動し、「**ドキュメント**」を選択します。
1. 必要なドキュメントを見つけます。

1. 概要で「**承認**」セクションまで下にスクロールして、その他アイコン、「再送信」の順にクリックします。

   ![承認の再送信](assets/nwe-resubmit-approval-350x149.png)

## ドキュメント承認リクエストを削除

1. ドキュメントを含むプロジェクト、タスクまたはイシューに移動し、「**ドキュメント**」を選択します。
1. 必要なドキュメントを見つけます。

1. 概要で「**承認**」セクションまで下にスクロールして、**詳細**&#x200B;メニューを承認者の名前と併せてインラインでクリックし、「**削除**」を選択します。

   承認リクエストが削除され、承認者は、承認が必要なくなったという通知を受け取ります。 承認関連の共有アクセスも削除されます。

## 承認者にリマインダーを送信

メッセージを送信して、フィードバックを待っていることを承認者に通知することができます。

1. ドキュメントを含むプロジェクト、タスクまたはイシューに移動し、「**ドキュメント**」を選択します。
1. 必要なドキュメントを見つけます。

1. 概要で「**承認**」セクションまで下にスクロールして、**詳細**&#x200B;メニューを承認者の名前と併せてインラインでクリックし、「**通知**」を選択します。

   承認者は、承認がまだ保留中であるという通知を受け取ります。 有効にしている場合は、リマインダーメールを受け取る場合もあります。
