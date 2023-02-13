---
product-area: documents
navigation-topic: manage-documents
title: ドキュメントをチェックアウト
description: ドキュメントをチェックアウトすると、他のユーザーがドキュメントを削除したり、新しいバージョンのドキュメントをアップロードしたりするのを防ぐことができます。 一度に 1 人のユーザーだけがドキュメントをチェックアウトできます。 Adobe Workfrontにアップロードされたドキュメントや、サードパーティのドキュメントプロバイダー (Box、Dropbox、Google Drive、Webdam、Workfront DAM、SharePoint、その他のカスタムプロバイダー ) にリンクされたドキュメントをチェックアウトできます。
author: Courtney
feature: Digital Content and Documents
exl-id: 15d9ea43-1cee-4cb1-9365-4374a291c090
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '673'
ht-degree: 0%

---

# ドキュメントをチェックアウト

ドキュメントをチェックアウトすると、他のユーザーがドキュメントを削除したり、新しいバージョンのドキュメントをアップロードしたりするのを防ぐことができます。 一度に 1 人のユーザーだけがドキュメントをチェックアウトできます。 Adobe Workfrontにアップロードされたドキュメントや、サードパーティのドキュメントプロバイダー (Box、Dropbox、Google Drive、Webdam、Workfront DAM、SharePoint、その他のカスタムプロバイダー ) にリンクされたドキュメントをチェックアウトできます。 

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ドキュメントへのアクセスを管理</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## チェックアウトしたドキュメントで許可されるアクション

ドキュメントへのアクセスを管理するユーザーは、次の操作を実行できます。

* ドキュメント（ドキュメント名、説明、カスタムデータ）を編集
* ドキュメントを移動
* ドキュメントを共有
* ドキュメントをプレビュー
* ドキュメントをダウンロード

   >[!TIP]
   >
   > ユーザーは、別のユーザーがチェックアウトしたときにドキュメントをダウンロードできますが、ドキュメントが再びチェックインされるまで待ってからダウンロードすることをお勧めします。 ドキュメントがチェックアウトされると、多くの場合、ドキュメント上で作業がまだ実行中であることを示します。 ドキュメントが再びチェックインされてダウンロードされるのを待つと、ユーザーは最新のバージョンを使用していることが確認されます。

* ドキュメントを承認するか、ドキュメントに承認を適用します。
* 文書を校正ビューアで確認する

   校正について詳しくは、 [校正](../../review-and-approve-work/proofing/proofing.md)

## ドキュメントのチェックアウト

ドキュメントに対する管理権限を持っている場合は、ドキュメントに対する特定のアクションを禁止するために、ドキュメントをチェックアウトできます。 

1. ドキュメントが保存されている領域に移動し、ドキュメントを選択します。 

   ドキュメントの追加について詳しくは、 [ファイルシステムからAdobe Workfrontにドキュメントを追加する](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md).

1. 次をクリック： **チェックアウト** アイコン ![](assets/check-out-25x23.png).

1. ロックアイコン ![](assets/lock-icon-locked-qs.png) は、ドキュメント名の右側に表示されます。 Workfrontからログアウトした後も、ドキュメントはチェックアウトされたままになります。
1. ドキュメントをチェックアウトしたユーザー、またはWorkfront管理者のみが、ドキュメントをチェックインできます。

## チェックアウトしたドキュメントを管理

チェックアウトしたドキュメントについては、次の点を考慮してください。

* チェックアウトしたドキュメントが保存されているオブジェクトを削除する前に、ドキュメントを再度チェックインする必要があります。 
* Workfront管理者が自分が所有していないドキュメントをチェックアウトしたユーザーを削除した場合、Workfrontは自動的にそのドキュメントをチェックインします。
* Workfront管理者が所有するドキュメントをチェックアウトしたユーザーを削除し、そのドキュメントがオブジェクトにアップロードされた場合、そのドキュメントはチェックアウトされたままになります。 再度チェックインできるのは、Workfront管理者のみです。
* Workfront管理者が所有するドキュメントをチェックアウトしたユーザーを削除し、そのドキュメントが（オブジェクトではなく）ドキュメント領域にのみアップロードされた場合、そのドキュメントはユーザーと共に削除されます。

   ユーザーの削除について詳しくは、 [ユーザーの削除](../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md).

* Workfront管理者がユーザーを非アクティブ化した場合、チェックアウトしたドキュメントはチェックアウトされたままになります。 再度チェックインできるのは、Workfront管理者のみです。 

## ドキュメントをチェックインする

新しいバージョンをアップロードまたは削除する前に、ドキュメントを再度チェックインする必要があります。 

ドキュメントをチェックインするには：

1. ドキュメントが保存されている領域に移動し、ドキュメントを選択します。 

   ロックアイコン ![](assets/lock-icon-locked-qs.png) は、ドキュメント名の右側に表示されます。

1. 次をクリック： **チェックイン** アイコン ![](assets/check-in-25x22.png).
