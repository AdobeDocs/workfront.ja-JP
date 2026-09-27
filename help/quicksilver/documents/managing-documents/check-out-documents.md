---
product-area: documents
navigation-topic: manage-documents
title: ドキュメントのチェックアウト
description: ドキュメントをチェックアウトすると、他のユーザーがドキュメントを削除したり、新しいバージョンのドキュメントをアップロードしたりするのを防ぐことができます。 一度に 1 人のユーザーだけがドキュメントをチェックアウトできます。 Adobe Workfront にアップロードされたドキュメントだけでなく、サードパーティのドキュメントプロバイダー（Box、Dropbox、Google Drive、Webdam、Workfront DAM、SharePoint、その他のカスタムプロバイダー）にリンクされているドキュメントをチェックアウトできます。
author: Courtney
feature: Digital Content and Documents
exl-id: 15d9ea43-1cee-4cb1-9365-4374a291c090
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/kkWxK2NzQtSfeRqsd0vEB-2AUYFrO6WIU3A752w7kM4'
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
feature_v2:
  - id: d968a1bc-9a90-4926-a531-bcf272c32aad
    internal-label: Administration
  - id: e14a7f57-c82c-4874-a495-5d036cbbdc3d
    internal-label: Resource management
subfeature_v2:
  - id: b70a979b-965d-47a9-a360-e7ec2a19b8c1
    internal-label: Digital content and documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
topic_v2:
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '686'
ht-degree: 86%
---
# ドキュメントのチェックアウト

ドキュメントをチェックアウトすると、他のユーザーがドキュメントを削除したり、新しいバージョンのドキュメントをアップロードしたりするのを防ぐことができます。 一度に 1 人のユーザーだけがドキュメントをチェックアウトできます。 Adobe Workfront にアップロードされたドキュメントだけでなく、サードパーティのドキュメントプロバイダー（Box、Dropbox、Google Drive、Webdam、Workfront DAM、SharePoint、その他のカスタムプロバイダー）にリンクされているドキュメントをチェックアウトできます。 

>[!NOTE]
>
>この機能は、新規ドキュメント領域では使用できません。<br>
>組織でAdobe クラウドストレージを使用している場合、Workfrontでドキュメントにアクセスすると、新しいドキュメント エリアが表示されます。 Adobe クラウドストレージについて詳しくは、[Adobe クラウドストレージの概要](/help/quicksilver/review-and-approve-work/esm-overview.md)を参照してください。

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
   <p>コントリビューター以上</p>
   <p>レビュー以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>ドキュメントへのアクセスを編集</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ドキュメントへのアクセス権を管理</p> </td> 
  </tr> 
 </tbody> 
</table>

この表の情報について詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## チェックアウトしたドキュメントで可能なアクション

ドキュメントへの管理アクセスを持つユーザーは、次の操作を実行できます。

* ドキュメントの編集（ドキュメント名、説明、カスタムデータ）
* ドキュメントの移動
* ドキュメントの共有
* ドキュメントのプレビュー
* ドキュメントのダウンロード

  >[!TIP]
  >
  > 別のユーザーがチェックアウトしている場合、そのドキュメントをダウンロードできますが、ドキュメントが再びチェックインされるまで待ってからダウンロードすることをお勧めします。 ドキュメントがチェックアウトされているとき、多くの場合、ドキュメントに対して作業がまだ行われていることを示します。 ドキュメントが再びチェックインされるのを待ってからダウンロードすることで、ユーザーは確実に最新のバージョンを入手できます。

* ドキュメントを承認するか、ドキュメントに承認を適用します。
* プルーフビューアでドキュメントを確認

  プルーフについて詳しくは、[プルーフ](../../review-and-approve-work/proofing/proofing.md)を参照してください。

## ドキュメントをチェックアウト

ドキュメントに対する管理権限を持っている場合は、ドキュメントをチェックアウトして、ドキュメントに対する特定のアクションを禁止することができます。 

1. ドキュメントが保存されているエリアに移動し、ドキュメントを選択します。 

   ドキュメントの追加について詳しくは、[ファイルシステムから Adobe Workfront にドキュメントを追加](../../documents/adding-documents-to-workfront/add-documents-from-file-system.md)を参照してください。

1. **チェックアウト** アイコン ![&#x200B; チェックアウトアイコン &#x200B;](assets/check-out-25x23.png)をクリックします。

1. ドキュメント名の右側に、ロックアイコン ![&#x200B; ロックアイコン &#x200B;](assets/lock-icon-locked-qs.png)が表示されます。 Workfront からログアウトした後でも、ドキュメントはチェックアウトされたままになります。
1. ドキュメントをチェックアウトしたユーザーか、Workfront 管理者のみが、ドキュメントをチェックインできます。

## チェックアウトしたドキュメントを管理

チェックアウトしたドキュメントについては、次の点を考慮してください。

* チェックアウトしたドキュメントが保存されているオブジェクトを削除する前に、ドキュメントを再度チェックインする必要があります。 
* Workfront 管理者が所有していないドキュメントをユーザーがチェックアウトし、そのユーザーを Workfront 管理者が削除した場合、Workfront は自動的にそのドキュメントをチェックインします。
* Workfront 管理者が所有するドキュメントをユーザーがチェックアウトし、そのユーザーを Workfront 管理者が削除して、さらにそのドキュメントがオブジェクトにアップロードされている場合、そのドキュメントはチェックアウトされたままになります。 再度チェックインできるのは、Workfront 管理者のみです。
* Workfront 管理者が所有するドキュメントをユーザーがチェックアウトし、そのユーザーを Workfront 管理者が削除して、さらにそのドキュメントが（オブジェクト上ではなく）ドキュメントエリアにのみアップロードされている場合、そのドキュメントはユーザーと一緒に削除されます。

  ユーザーの削除について詳しくは、[ユーザーの削除](../../administration-and-setup/add-users/create-and-manage-users/delete-a-user.md)を参照してください。

* Workfront 管理者がユーザーを非アクティブ化した場合、そのユーザーがチェックアウトしているドキュメントは、チェックアウトされたままになります。 再度チェックインできるのは、Workfront 管理者のみです。 

## ドキュメントをチェックイン

ドキュメントの新しいバージョンをアップロードするか、ドキュメントを削除する前に、ドキュメントを再度チェックインする必要があります。 

ドキュメントをチェックインするには、次の操作を実行します。

1. ドキュメントが保存されているエリアに移動し、ドキュメントを選択します。 

   ドキュメント名の右側に、ロックアイコン ![&#x200B; ロックアイコン &#x200B;](assets/lock-icon-locked-qs.png)が表示されます。

1. **チェックイン** アイコン ![&#x200B; チェックインアイコン &#x200B;](assets/check-in-25x22.png)をクリックします。
