---
product-area: documents
navigation-topic: approvals
title: 新しいドキュメント バージョンをアップロードし、承認を要求する
description: 新しいドキュメントバージョンをアップロードし、Adobe Workfrontの他のユーザーの承認をリクエストできます。
author: Courtney
feature: Work Management, Digital Content and Documents
exl-id: 0eb8cfba-2317-419c-b28f-da2e7a99401c
source-git-commit: 42fbb40cb8a0f3c70e22fd04bd3d0ce625f58fec
workflow-type: tm+mt
source-wordcount: '488'
ht-degree: 25%

---

# 新しいドキュメント バージョンをアップロードし、承認を要求する

以前のレビューで「作業が必要」とマークされたドキュメントの場合、新しいバージョンを元のドキュメントにアップロードし、別の承認を開始することができます。 新しいバージョンのドキュメントをアップロードすると、以前のバージョンがロックされます。

新しいバージョンのファイル名が以前のバージョンのファイル名と異なる場合、Workfront は新しいファイル名を持つドキュメントを表示します。

承認が未処理のドキュメントに新しいバージョンが追加されると、以前のバージョンの承認は「取り消し」と表示されます。 一部の参加者がまだ決定を行っていない場合でも、前回の承認プロセスが終了します。

最新バージョンのドキュメントを削除しても、以前のバージョンはロックされたままになります。 以前のバージョンを編集する必要がある場合は、手動でロックを解除する必要があります。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p> 任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>リクエスト以上</p>
   <p>投稿者以上</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="/help/quicksilver/administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ドキュメントに関連付けられたオブジェクトへの編集アクセス権</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="/help/quicksilver/workfront-basics/grant-and-request-access-to-objects/grant-and-request-access-to-objects.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## ドラッグ＆ドロップを使用して新しいバージョンを追加する

>[!NOTE]
>
>Internet Explorer ではドラッグ＆ドロップは機能しません。


ドキュメントに対する別のラウンドのレビューと承認が必要な場合は、Workfrontで新しいドキュメントバージョンを作成できます。

以前の参加者、新しい参加者または両方を追加できます。 以前のバージョンと参加者に関する情報は、「ドキュメントの詳細」 ページで表示できます。

新しいバージョンを追加するには：

1. Workfrontのドキュメントに移動します。
1. 新しいファイルを前のドキュメントの上にドラッグ&amp;ドロップします。 これにより、新しいバージョンが自動的に作成されます。

1. ドキュメントのアップロードが完了したら、ドキュメントを選択し、「**ドキュメントの詳細**」をクリックします。
   ![ ドキュメントの詳細ページを開く ](assets/open-doc-details.png)


1. 左側のパネルで「**承認**」をクリックし、「**追加**」をクリックします。

1. 以前の参加者をすべて追加するには、「**すべてを追加**」をクリックします。 必要に応じて、新しい参加者を追加したり、以前の参加者を削除したりすることもできます。


1. 既存の承認テンプレートを追加するには、「テンプレート」ボタンをクリックしてテンプレート名の入力を開始します。

   >[!TIP]
   >
   >   Standard ライセンスを持つユーザーは、設定エリアから適切な承認テンプレートを作成できます。 詳しくは、[ アセットおよびドキュメントの承認テンプレートの作成 ](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-approval-template.md) を参照してください。


1. （任意）承認の期限を設定します。 ユーザーとチームには、指定した期限の 72 時間前と 24 時間前にメールで通知が届きます。

1. すべてのレビュー担当者と承認者を追加したら、「**リクエストを送信**」をクリックします。 参加者には、メールで通知されます。

   ![ 承認用に新しいバージョンを送信 ](assets/add-previous-participants.png)


