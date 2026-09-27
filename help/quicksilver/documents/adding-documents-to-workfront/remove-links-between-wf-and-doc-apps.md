---
product-area: documents
navigation-topic: add-documents-to-workfront
title: Adobe Workfront と外部ドキュメントストレージプロバイダー間のリンクを削除する
description: 任意のサービスからドキュメントを初めてアップロードする際に、Adobe Workfront は、ドキュメントサービスにアクセスするための許可をユーザーに要求します。 ユーザーがログイン用のドキュメントサービス資格情報を提供すると、ドキュメントサービスは自身を Workfront にリンクします。
author: Courtney
feature: Digital Content and Documents
exl-id: fce8e8aa-fc48-49e1-a71d-c3933a179cf5
last-update: 2026-04-01T18:03:50.000Z
git-commit-file: b03dbe8e217593e0f3a6fcd522148dcd8b7670b8
TQID: 'https://experienceleague.adobe.com/wDii-Gr-3a0NfMhc9VPfbiUNSTyJaJuFHeXACI26NxU'
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
  - id: d095671a-1355-40aa-8b5f-06c33c68080b
    internal-label: Security
  - id: eddd9b14-83bd-4ff4-9072-54a4a484abb7
    internal-label: Administration
source-git-commit: 4c642a8ef31f3b9a03288f2d74e704be6ee86c55
workflow-type: tm+mt
source-wordcount: '424'
ht-degree: 88%
---
# Adobe Workfront と外部ドキュメントストレージプロバイダー間のリンクを削除する

任意のサービスからドキュメントを初めてアップロードする際に、Adobe Workfront は、ドキュメントサービスにアクセスするための許可をユーザーに要求します。 ユーザーがログイン用のドキュメントサービス資格情報を提供すると、ドキュメントサービスは自身を Workfront にリンクします。

外部ドキュメントサービスの Workfront へのリンクについて詳しくは、[外部アプリケーションからのドキュメントのリンク](../../documents/adding-documents-to-workfront/link-documents-from-external-apps.md)を参照してください。

ドキュメントサービスは Workfront へのリンク権限を許可するものなので、Workfront ではドキュメントサービスから付与された権限を削除できません。 ドキュメントサービスアプリケーション内から権限を削除するか、サポートチームに連絡して、サーバーからこのリンクを削除する必要があります。

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
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> 
   <p>コントリビューター以上</p>
   <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定</td> 
   <td> <p>ドキュメントへのアクセスを編集</p>  </td> 
  </tr> 
 </tbody> 
</table>

詳しくは、[Workfront ドキュメントのアクセス要件](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md)を参照してください。

+++

## Workfront と Dropbox 間のリンクを削除する

1. Dropbox にログインします。
1. 右上隅のプロフィール画像をクリックし、「**設定**」をクリックします。
1. 「**接続済みアプリ**」タブをクリックして、「**リンクされたアプリ**」まで下にスクロールします。

1. Workfront の横にある「**X**」をクリックします。

## Workfrontと Box 間のリンクを削除する

1. Box アカウントにログインします。
1. 右上隅のプロフィール画像をクリックします。
1. 「**アカウント設定**」をクリックして、「**セキュリティ**」タブをクリックします。

1. **MyWorkfront** を見つけて、「アプリを忘れる」の下の「**X**」をクリックします。

## Workfront と Google Drive 間のリンクを削除する

1. Google Drive にログインします。
1. 右上隅の歯車アイコンをクリックし、「**設定**」をクリックします。
1. 左側にある「**アプリの管理**」をクリックし、リストに **Workfront** を見つけます。

1. 「オプション」ドロップダウンメニューで、「**ドライブから切断**」をクリックします。

## Workfront とその他のドキュメントストレージプロバイダー間のリンクを削除する

Workfront から Microsoft One Drive または WebDAM を切断するには、サポートチームに連絡する必要があります。

サポートチームへのお問い合わせについて詳しくは、[カスタマーサポートへのお問い合わせ](../../workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md)を参照してください。
