---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Web リンクをドキュメントとして追加
description: Adobe Workfrontにweb サイトをweb リンクとして追加し、承認を依頼できます。
author: Courtney
feature: Digital Content and Documents
role_v2:
  - id: b69b2659-1057-424e-8fc5-ed9e016dc554
    internal-label: User
product_v2:
  - id: c4a86a5d-6562-4fc6-aa00-bfa25833aed9
    internal-label: Workfront
source-git-commit: 5e37582fe161e1a4689c35773cb1b3f6ead5a859
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 9%
---
# Web リンクをドキュメントとして追加

新しいドキュメント領域からweb リンクとしてAdobe Workfrontにweb サイトを追加できます。 追加した後は、アップロードしたファイルの承認をリクエストするのと同じように、ライブ web ページで承認をリクエストできます。

組織でAdobe クラウドストレージを使用している場合、Workfrontでドキュメントにアクセスすると、新しいドキュメント エリアが表示されます。 Adobe クラウドストレージについて詳しくは、[Adobe クラウドストレージの概要](/help/quicksilver/review-and-approve-work/esm-overview.md)を参照してください。

## アクセス要件

+++ 展開すると、この記事の機能のアクセス要件が表示されます。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront パッケージ</td> 
   <td> <p>従来のWorkfront ストレージを使用してドキュメントを管理するWorkfront パッケージ</p>
<p>Adobe クラウドストレージを使用してドキュメントを管理するワークフローパッケージ</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス</td> 
   <td> 
   <p>コントリビューター以上</p> 
   <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>従来のWorkfront ストレージ：ドキュメントへのアクセスを編集する</p> 
   <p>Adobe クラウドストレージ：ドキュメントへの編集アクセスはデフォルトで有効になっており、変更できません</p>
   </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## Web リンクをドキュメントとして追加

Web リンクとしてhtml web ページをWorkfrontにアップロードできます。 追加した後は、アップロードしたファイルの承認をリクエストするのと同じように、ライブ web ページで承認をリクエストできます。 Frame.ioでのweb リンクの処理方法について詳しくは、[Frame.io web リンク ](https://support.frame.io/hc/en-us/articles/360041187574-Frame-io-Web-Links)を参照してください。

<!--
>[!IMPORTANT]
>
>A web page behind single sign-on or a login page can't be displayed for review.
-->

Web リンクを追加するには：

1. Web サイトを追加するプロジェクト、タスク、またはイシューに移動し、左側のパネルで「**ドキュメント**」を選択します。
1. 「**新規**」をクリックし、「**Web リンク**」を選択します。
1. **ドキュメント名** フィールドに名前を入力し、**URL** フィールドにweb サイトのアドレスを入力します。
1. 「**追加**」をクリックします。
   ![Web リンクをドキュメントとして追加](assets/web-url.png)

Web リンクで承認を要求するには、[ ドキュメント承認ワークフローの作成](/help/quicksilver/review-and-approve-work/document-reviews-and-approvals/manage-document-approvals/create-a-document-approval.md)を参照してください。

## 既知の制限事項

* Frame.ioで作成されたweb リンクドキュメントに一時的な問題があります。 Frame.ioでweb リンクを作成し、そのweb リンクをWorkfrontで作成した場合、その文書はFrame.ioで開きません。 Workfrontで作成されたWeb リンクは影響を受けません。 この問題が解決するまで、承認を開始する前に、Workfrontでweb リンクドキュメントを作成します。
* 現在、Frame.ioで新しいバージョンのweb リンクドキュメントを作成することはできません。 Web リンクドキュメントの新しいバージョンを作成する必要がある場合は、Workfrontで新しいバージョンを作成します。