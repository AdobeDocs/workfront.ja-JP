---
product-area: documents;workfront-integrations
navigation-topic: adobe-workfront-for-experince-manager-asset-essentials
title: Experience Manager AssetsまたはAssets Essentialsにドキュメントを送信する
description: ドキュメントは、WorkfrontからExperience Manager AssetsまたはAssets Essentialsに送信できます。 WorkfrontからAssets Essentialsにアップロードされて送信されたドキュメントは、引き続きドキュメントストレージ全体に対してカウントされます。 Assets Essentialsからリンクされたアセットは、全体のストレージにはカウントされません。
author: Courtney
feature: Digital Content and Documents, Workfront Integrations and Apps
exl-id: 7942e77b-9466-4dff-9737-97b17647ac48
source-git-commit: 5469598d57fec1a744ddb44cf2accb94e1f70941
workflow-type: tm+mt
source-wordcount: '709'
ht-degree: 0%

---

# Experience Manager AssetsまたはAssets Essentialsにドキュメントを送信する


ドキュメントは、WorkfrontからExperience Manager AssetsまたはAssets Essentialsに送信できます。 WorkfrontからAssets Essentialsにアップロードされて送信されたドキュメントは、引き続きドキュメントストレージ全体に対してカウントされます。 Assets Essentialsからリンクされたアセットは、全体のストレージにはカウントされません。

アセットをWorkfrontからExperience Manager AssetsまたはAssets Essentialsに送信する際に、メタデータフィールドが最初にマッピングされます。 親オブジェクトに対してマッピングするように設定されたメタデータも送信されます。 メタデータマッピングの設定について詳しくは、 [Experience Manager Assets統合の設定](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) または [Experience Manager Assets Essentials 統合の設定](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

>[!INFO]
>
>**例** タスクにアタッチされたアセットを最初に送信すると、タスクメタデータはExperience Manager AssetsまたはAssets Essentialsにマッピングされ、親オブジェクト（プロジェクト、ポートフォリオ、プログラムなど）からマッピングされたメタデータもにマッピングされます。

## アクセス要件

以下が必要です。

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfrontプラン</a>*</td> 
   <td> <p> 任意</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">レガシーライセンスの概要</a>*</td> 
   <td> <p>リクエスト以上</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">製品</td> 
   <td>as a Cloud ServiceのExperience ManagerまたはAssets Essentialsがあり、ユーザーとして製品に追加されている必要があります。Admin Console。
</td> 
  </tr> 
  <tr> 
   <td role="rowheader">アクセスレベル設定*</td> 
   <td> <p>ドキュメントへのアクセスを編集</p> <p>注意：まだアクセス権がない場合は、Workfront管理者に、アクセスレベルに追加の制限を設定しているかどうかを問い合わせてください。 Workfront管理者がアクセスレベルを変更する方法について詳しくは、 <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">カスタムアクセスレベルの作成または変更</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">オブジェクト権限</td> 
   <td> <p>ドキュメントのアクセス権以上の表示</p> <p>追加のアクセス権のリクエストについて詳しくは、 <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">オブジェクトへのアクセスのリクエスト </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;保有しているプラン、ライセンスの種類、アクセス権を確認するには、Workfront管理者に問い合わせてください。

## 前提条件

始める前に

* Workfront管理者は、統合を設定する必要があります。 詳しくは、 [Experience Manager Assets統合の設定](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) または [Experience Manager Assets Essentials 統合の設定](/help/quicksilver/documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).


## Workfrontからドキュメントを送信

ユーザーがWorkfrontからExperience Manager AssetsまたはAssets Essentialsにドキュメントを送信すると、マッピングされたメタデータはドキュメントに沿って転送されます。 ドキュメントの送信後、Workfrontでドキュメントのメタデータに加えた変更は、Assets やAssets Essentialsには反映されません。 Workfrontでマッピングされたフィールドが変更された場合は、更新されたメタデータを含む新しいバージョンのドキュメントを Assets またはAssets Essentialsに送信する必要があります。 メタデータを設定または編集するには、 [Experience Manager Assets統合の設定](/help/quicksilver/administration-and-setup/configure-integrations/configure-aacs-integration.md) または [Experience Manager Assets Essentials 統合の設定](../../documents/adobe-workfront-for-experience-manager-assets-essentials/setup-asset-essentials.md).

ドキュメントを送信するには：

1. 次に移動： **ドキュメント** 「Workfront」領域に移動し、送信するドキュメントを選択します。
1. クリック **送信先**」で、管理者が設定したExperience Manager統合を選択します。

   >[!NOTE]
   >
   >Workfrontの管理者は、この統合に対して任意の名前を選択できるので、Assets やAssets Essentialsについては特に言及できません。

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. アセットの移動先を選択し、「 **フォルダーを選択**.
1. 目的の宛先が見つかったら、 **保存**.

## 新しいバージョンを送信

以前にWorkfrontにアップロードしたドキュメントに新しいバージョンを追加できます。 詳しくは、 [新しいバージョンのドキュメントをアップロード](../../documents/managing-documents/upload-new-document-version.md). 最新バージョンがアップロードされたら、Assets Essentialsに送信できます。 Workfrontでマッピングされたフィールドが変更された場合、新しいバージョンは、送信時にAssets Essentialsのメタデータを更新します。

>[!IMPORTANT]
>
>新しいバージョンをWorkfrontにアップロードする前に、ファイル名を変更することをお勧めします。 以前のバージョンと同じファイル名を持つ新しいバージョンをアップロードした場合、Workfrontからダウンロードできるのは最新バージョンのみです。 ファイル名に関係なく、すべてのバージョンをExperience Manager AssetsまたはAssets Essentialsからダウンロードできます。

最新バージョンを送信するには：

1. 次に移動： **ドキュメント** 領域内のWorkfrontをクリックし、ドキュメントを探します。
1. 選択 **送信先**」で、管理者が設定したExperience Manager統合を選択します。

   >[!NOTE]
   >
   >Workfrontの管理者は、この統合に対して任意の名前を選択できるので、Assets やAssets Essentialsについては特に言及しない場合があります。

   ![](assets/copy-of-send-to-in-toolbar-350x149.png)

1. 「**保存**」をクリックします。新しいバージョンは、以前のバージョンと同じ場所に保存されます。
