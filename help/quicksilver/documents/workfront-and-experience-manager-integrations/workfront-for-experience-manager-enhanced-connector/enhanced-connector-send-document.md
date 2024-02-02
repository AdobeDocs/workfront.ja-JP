---
product-area: documents;workfront-integrations
navigation-topic: workfront-for-experience-manager-enhanced-connector
title: 拡張コネクタを使用してドキュメントを送信
description: Workfront から Experience Manager Assets にドキュメントを送信できます。Workfront から Experience Manager Asset にアップロードおよび送信されたドキュメントは、引き続きドキュメントストレージ全体に対してカウントされます。Experience Manager からリンクされたアセットは、全体のストレージにはカウントされません。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: d687d2db-28e0-45e8-9d60-8419921f02e9
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: ht
source-wordcount: '453'
ht-degree: 100%

---

# 拡張コネクタを使用してドキュメントを送信

Workfront から Experience Manager Assets にドキュメントを送信できます。Workfront から Experience Manager Asset にアップロードおよび送信されたドキュメントは、引き続きドキュメントストレージ全体に対してカウントされます。Experience Manager からリンクされたアセットは、全体のストレージにはカウントされません。

## アクセス要件

この記事の手順を実行するには、次のアクセス権が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront プラン*</td> 
   <td> <p>Pro 以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront ライセンス*</td> 
   <td> <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>Experience Manager Assets </td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ドキュメントの表示アクセス権またはそれ以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 前提条件

開始する前に、

* Workfront for Experience Manager 拡張コネクタのインストール。

## Experience Manager Assets へのドキュメントの送信

Workfront から Experience Manager Assets にユーザーがドキュメントを送信すると、マッピングされたメタデータはドキュメントに沿って転送されます。構成されている場合、メタデータは変更が行われるたびに継続的に同期されます。

ドキュメントを送信するには：

1. **ドキュメント**&#x200B;に移動して、Workfront エリアに移動し、送信するドキュメントを選択します。
1. 「**送信先**」をクリックして、管理者が設定した Experience Manager Assets 統合を選択します。

   >[!NOTE]
   >
   >この統合には任意の名前を選択できるため、Experience Manager Assets について特に言及されていない場合があります。

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. アセットの保存先を選択し、「**フォルダーを選択**」をクリックします。
1. 目的の宛先が見つかったら、「**保存**」をクリックします。

## 新しいバージョンを Experience Manager Assets に送信

以前に Workfront にアップロードしたドキュメントに新しいバージョンを追加できます。詳しくは、[新しいバージョンのドキュメントをアップロード](../../../documents/managing-documents/upload-new-document-version.md)を参照してください。最新バージョンがアップロードされたら、それを Experience Manager Assets に送信できます。Workfront でマッピングされたフィールドが変更された場合、新しいバージョンは、送信時に Experience Manager Assets のメタデータを更新します。

最新バージョンを送信するには、次の手順に従います。

1. Workfront の&#x200B;**ドキュメント**&#x200B;エリアに移動して、ドキュメントを探します。
1. 「**送信先**」をクリックして、管理者が設定した Experience Manager Assets 統合を選択します。

   >[!NOTE]
   >
   >この統合には任意の名前を選択できるため、Experience Manager Assets について特に言及されていない場合があります。

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. 「**保存**」をクリックします。新しいバージョンは、以前のバージョンと同じ場所に保存されます。
