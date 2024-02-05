---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Experience Manager Assets または Assets Essentials へのドキュメントの送信
description: Workfront から Experience Manager Assets または Assets Essentials にドキュメントを送信できます。Workfront から Assets Essentials にアップロードおよび送信されたドキュメントは、引き続きドキュメントストレージ全体に対してカウントされます。Assets Essentials からリンクされたアセットは、全体のストレージにはカウントされません。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: 706e531be6f6269a927f94fee4d2c37d9367c9af
workflow-type: tm+mt
source-wordcount: '864'
ht-degree: 100%

---

# Experience Manager Assets または Assets Essentials へのドキュメントの送信

Workfront から Experience Manager Assets または Assets Essentials にドキュメントを送信できます。Workfront から Assets Essentials にアップロードおよび送信されたドキュメントは、引き続きドキュメントストレージ全体に対してカウントされます。Assets Essentials からリンクされたアセットは、全体のストレージにはカウントされません。

Workfront から Experience Manager Assets または Assets Essentials にアセットを送信する際、メタデータフィールドが最初にマッピングされます。親オブジェクトに対してマッピングするように設定されたメタデータも送信されます。メタデータマッピングの設定について詳しくは、[Experience Manager Assets as a Cloud Service 統合の設定](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)または [Experience Manager Assets Essentials 統合の設定](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)を参照してください。

>[!INFO]
>
>**例**：タスクに添付された Assets Essentials を最初に送信すると、タスクメタデータは Experience Manager Assets またはアセットにマッピングされ、親オブジェクト（プロジェクト、ポートフォリオ、プログラムなど）からマッピングされたメタデータにもマッピングされます。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront プラン</a>*</td> 
   <td> <p> 任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">従来のライセンスの概要</a>*</td> 
   <td> <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>Experience Manager as a Cloud Service または Assets Essentials を使用するには、Admin Console に製品にユーザーとして追加されている必要があります。
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>メモ：まだアクセス権がない場合は、アクセスレベルに追加の制限が設定されていないかどうか Workfront 管理者にお問い合わせください。Workfront 管理者がアクセスレベルを変更する方法について詳しくは、<a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>を参照してください。</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ドキュメントの表示アクセス権またはそれ以上の権限</p> <p>追加のアクセス権のリクエストについて詳しくは、<a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセス権のリクエスト</a>を参照してください。</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有するプラン、ライセンスタイプ、アクセス権を確認するには、Workfront 管理者に問い合わせてください。

## 前提条件

開始する前に、

* Workfront 管理者は、Experience Manager 統合を設定する必要があります。詳細については、[Experience Manager Assets as a Cloud Service 統合の設定](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md)または[Experience Manager Assets Essentials 統合の設定](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)を参照してください。


## Workfront からドキュメントを送信

Workfront から Experience Manager Assets または Assets Essentials にユーザーがドキュメントを送信すると、マッピングされたメタデータはドキュメントに沿って転送されます。ドキュメントの送信後、Workfront でドキュメントのメタデータに加えた変更は、Assets や Assets Essentials には反映されません。Workfront でマッピングされたフィールドが変更された場合、更新されたメタデータを含む新しいバージョンのドキュメントを Assets またはAssets Essentials に送信する必要があります。メタデータを設定または編集するには、[Experience Manager Assets as a Cloud Service 統合の設定](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) または [Experience Manager Assets Essentials 統合の設定](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md)を参照してください。

ドキュメントを送信するには：

1. **ドキュメント**&#x200B;に移動して、Workfront エリアに移動し、送信するドキュメントを選択します。
1. 「**送信先**」をクリックして、管理者が設定した Experience Manager 統合を選択します。

   >[!NOTE]
   >
   >Workfront 管理者は、この統合に対して任意の名前を選択できるので、Assets や Assets Essentials とは明記されていない場合があります。

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. アセットの保存先を選択し、「**フォルダーを選択**」をクリックします。
1. 目的の宛先が見つかったら、「**保存**」をクリックします。

## 新しいバージョンを送信

以前に Workfront にアップロードしたドキュメントに新しいバージョンを追加できます。詳しくは、[新しいバージョンのドキュメントのアップロード](../../documents/managing-documents/upload-new-document-version.md)を参照してください。最新バージョンがアップロードされたら、そのバージョンを Assets Essentials に送信できます。Workfront でマッピングされたフィールドが変更された場合、新しいバージョンは、送信時に Assets Essentials のメタデータを更新します。

>[!IMPORTANT]
>
>新しいバージョンを Workfront にアップロードする前に、ファイル名を変更することをお勧めします。以前のバージョンと同じファイル名を持つ新しいバージョンをアップロードした場合、Workfront からダウンロードできるのは最新バージョンのみです。Experience Manager Assets または Assets Essentials からは、ファイル名に関係なく、すべてのバージョンをダウンロードできます。

最新バージョンを送信するには、次の手順に従います。

1. Workfront の&#x200B;**ドキュメント**&#x200B;エリアに移動して、ドキュメントを探します。
1. 「**送信先**」を選択し、管理者が設定した Experience Manager 統合を選択します。

   >[!NOTE]
   >
   >Workfront 管理者は、この統合の名前を任意に選択できるので、Assets や Assets Essentials とは明記されていない場合があります。

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. 「**保存**」をクリックします。新しいバージョンは、以前のバージョンと同じ場所に保存されます。

## リンクされた Experience Manager Assets フォルダーへのドキュメントの移動

>[!NOTE]
>
>この機能は、Experience Manager Assets as a Cloud Service でのみ使用できます。Experience Manager Assets Essentials では使用できません。

ドキュメントおよびリンクされたフォルダーがどちらも同じドキュメントリスト（プロジェクトのドキュメントエリアなど）にある場合は、ドキュメントを Experience Manager Assets 内のリンクされたフォルダーに移動できます。

1. 移動するドキュメントを見つけます。
1. ドキュメントの移動先となるリンクされた Experience Manager Assets フォルダーに、ドキュメントをドラッグ＆ドロップします。

ドキュメントの移動中は、ドキュメントオプションは使用できません。ドキュメントは、Experience Manager Assets に移動すると、Workfront のドキュメントリストには表示されなくなります。

>[!NOTE]
>
> ドキュメントの移動中にドキュメントに対して行ったアクションや編集は、Experience Manager Assets 内のドキュメントには反映されないので、失われます。

