---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Adobe Workfrontと外部ドキュメントストレージプロバイダー間のリンクを削除する
description: 任意のサービスからドキュメントを初めてアップロードする際に、Adobe Workfrontは、ユーザーに対し、ドキュメントサービスへのアクセスを許可するように要求します。 ユーザーがログイン用のドキュメントサービス資格情報を指定すると、ドキュメントサービスは自身をWorkfrontにリンクします。
author: Courtney
feature: Digital Content and Documents
exl-id: fce8e8aa-fc48-49e1-a71d-c3933a179cf5
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '410'
ht-degree: 0%

---

# Adobe Workfrontと外部ドキュメントストレージプロバイダー間のリンクを削除する

任意のサービスからドキュメントを初めてアップロードする際に、Adobe Workfrontは、ユーザーに対し、ドキュメントサービスへのアクセスを許可するように要求します。 ユーザーがログイン用のドキュメントサービス資格情報を指定すると、ドキュメントサービスは自身をWorkfrontにリンクします。

外部ドキュメントサービスのWorkfrontへのリンクについて詳しくは、 [外部アプリケーションからのドキュメントのリンク](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md).

ドキュメントサービスはWorkfrontへのリンク権限を許可するものなので、Workfrontではドキュメントサービスから付与された権限を削除できません。 Document Service アプリケーション内から権限を削除するか、サポートチームに連絡して、サーバーからこのリンクを削除する必要があります。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p> 任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfrontライセンス*</td> 
   <td> <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## WorkfrontとDropbox間のリンクを削除

1. Dropbox
1. 右上隅のプロフィール画像をクリックし、 **設定**.
1. 次をクリック： **接続済みアプリ** 「 」タブから、下にスクロールして **リンクされたアプリ**.

1. 次をクリック： **X** Workfrontの隣に

## Workfrontと Box 間のリンクを削除

1. Box アカウントにログインします。
1. 右上隅のプロフィール画像をクリックします。
1. クリック **アカウント設定**、 **セキュリティ** タブをクリックします。

1. 検索 **MyWorkfront** をクリックし、 **X** をクリックします。

## WorkfrontとGoogle Drive 間のリンクを削除

1. Google Drive にログインします。
1. 右上隅の歯車アイコンをクリックし、 **設定**.
1. クリック **アプリを管理** 左側に **Workfront** を選択します。

1. オプションドロップダウンメニューで、 **ドライブから切断**.

## Workfrontと他のドキュメントストレージプロバイダー間のリンクを削除する

WorkfrontからMicrosoft One Drive または WebDAM を切断するには、サポートチームに連絡する必要があります。

サポートチームへの問い合わせについては、 [カスタマーサポートに連絡](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).
