---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Experience Manager Assets または Assets Essentials からのアセットおよびフォルダーのリンク
description: Experience Manager Assets または Assets Essentials からアセットまたはフォルダーをドキュメントをサポートする任意の Adobe Workfront オブジェクトにリンクできます。Assets Essentials から送信されたアセットは、Workfront のドキュメントストレージ全体にはカウントされません。Workfront から Assets Essentials にアップロードおよび送信されたドキュメントは、全体的なストレージにカウントされます。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: dbd19985-88b1-48ca-9cba-b7933ff2c191
source-git-commit: 8ecbca4d5d09b1f696f489148e960e0eeba2119e
workflow-type: ht
source-wordcount: '670'
ht-degree: 100%

---

# Experience Manager Assets または Assets Essentials からのアセットおよびフォルダーのリンク

Experience Manager Assets または Assets Essentials からアセットまたはフォルダーをドキュメントをサポートする任意の Adobe Workfront オブジェクトにリンクできます。Assets Essentials から送信されたアセットは、Workfront のドキュメントストレージ全体にはカウントされません。Workfront から Assets Essentials にアップロードおよび送信されたドキュメントは、全体的なストレージにカウントされます。

Workfront から Experience Manager Assets または Assets Essentials にアセットを送信する際、メタデータフィールドが最初にマッピングされます。Workfront 管理者がオブジェクトメタデータの同期を有効にしている場合、どちらかのアプリケーションで変更されたフィールドは最新の状態に保たれます。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p> 任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>Experience Manager as a Cloud Service または Assets Essentials を使用するには、Admin Console に製品にユーザーとして追加されている必要があります。</td> 
  </tr> 
   <tr> 
    <td role="rowheader">Experience Manager 権限</td> 
    <td>フォルダーへの書き込みアクセス権が必要です。</td> 
   </tr>
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>表示アクセス権またはそれ以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 前提条件

開始する前に、

* Workfront 管理者は、Experience Manager 統合を設定する必要があります。詳しくは、[Experience Manager Assets as a Cloud Service の統合を設定](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)または[Experience Manager Assets Essentials の統合を設定](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)を参照してください。

## Experience Manager Assets または Assets Essentials からのアセットのリンク

Experience Manager Assets または Assets Essentials から Workfront にアセットをリンクすることができます。アセットをリンクすると、次の操作が可能になります。

* [Experience Manager Assets または Assets Essentials のリンクされたアセットのプルーフ](../../documents/adobe-workfront-for-experience-manager-assets-essentials/proof-linked-asset-aem.md)
* [ドキュメントの新しいバージョンをアップロードする](../../documents/managing-documents/upload-new-document-version.md)

1. ドキュメントを追加する Workfront の&#x200B;**ドキュメント**&#x200B;エリアに移動します。
1. 「**新規追加**」を選択して、管理者が設定した Experience Manager 統合を選択します。

   >[!NOTE]
   >
   >Workfront 管理者は、この統合に対して任意の名前を選択できるので、Assets や Assets Essentials とは明記されていない場合があります。

1. 目的のアセットを選択します。

   ![](assets/select-an-asset.png)

1. 「**選択**」をクリックします。

## Experience Manager Assets または Assets Essentials からのフォルダーのリンク

フォルダー内の個々のアセットを表示する権限は、Experience Manager Assets または Assets Essentials 権限に依存します。

1. フォルダーを作成する Workfront の&#x200B;**ドキュメント**&#x200B;エリアに移動します。
1. 「**新規追加**」を選択して、管理者が設定した Experience Manager 統合を選択します。

   >[!NOTE]
   >
   >Workfront 管理者は、この統合の名前を任意に選択できるので、Assets や Assets Essentials とは明記されていない場合があります。

1. 目的のフォルダーを選択します。

   ![](assets/select-a-folder.png)

1. 「**選択**」をクリックします。

## Experience Manager Assets または Assets Essentials から新しいバージョンをリンク

新しいアセットを Assets Essentials から引き出し、新しいバージョンとして既存のアセットに追加できます。ドキュメントが既にリンクされていて、Assets Essentials で新しいバージョンが追加されている場合、新しいバージョンは Workfront に自動的に表示されます。

Assets Essentials から新しいバージョンをリンクするには、次の手順に従います。

1. ドキュメントを追加する Workfront の&#x200B;**ドキュメント**&#x200B;エリアに移動します。
1. 新しいバージョンに置き換えるアセットを選択します。リンクされたフォルダー内に新しいバージョンのアセットを作成することはできません。
1. **新規追加**／**バージョン**&#x200B;で、管理者が設定した Experience Manager 統合を選択します。

   >[!NOTE]
   >
   >Workfront 管理者は、この統合の名前を任意に選択できるので、Assets や Assets Essentials とは明記されていない場合があります。

1. 目的のアセットを選択します。

   ![](assets/select-an-asset.png)

1. 「**選択**」をクリックします。

>[!TIP]
>
>**ドキュメントの詳細**／**バージョン**&#x200B;に移動すると、アセットのすべてのバージョンを表示できます。
